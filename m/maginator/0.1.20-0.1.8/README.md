# Comparing `tmp/maginator-0.1.20.tar.gz` & `tmp/maginator-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/maginator-0.1.20.tar", last modified: Fri Apr 12 08:53:27 2024, max compression
+gzip compressed data, was "dist/maginator-0.1.8.tar", last modified: Thu Dec 15 11:14:01 2022, max compression
```

## Comparing `maginator-0.1.20.tar` & `maginator-0.1.8.tar`

### file list

```diff
@@ -1,58 +1,55 @@
-drwxr-xr-x   0 trizac   (198224) cu_10108  (1335)        0 2024-04-12 08:53:27.000000 maginator-0.1.20/
--rw-r--r--   0 trizac   (198224) cu_10108  (1335)       39 2024-04-12 08:43:45.000000 maginator-0.1.20/MANIFEST.in
--rw-r--r--   0 trizac   (198224) cu_10108  (1335)    13123 2024-04-12 08:53:27.000000 maginator-0.1.20/PKG-INFO
--rw-r--r--   0 trizac   (198224) cu_10108  (1335)    10965 2024-04-12 08:43:45.000000 maginator-0.1.20/README.md
-drwxr-xr-x   0 trizac   (198224) cu_10108  (1335)        0 2024-04-12 08:53:27.000000 maginator-0.1.20/maginator/
--rw-r--r--   0 trizac   (198224) cu_10108  (1335)       42 2024-04-12 08:43:45.000000 maginator-0.1.20/maginator/__init__.py
--rw-r--r--   0 trizac   (198224) cu_10108  (1335)     5587 2024-04-12 08:43:45.000000 maginator-0.1.20/maginator/controller.py
--rwxr-xr-x   0 trizac   (198224) cu_10108  (1335)     9851 2024-04-12 08:45:34.000000 maginator-0.1.20/maginator/main.py
--rw-r--r--   0 trizac   (198224) cu_10108  (1335)     2912 2024-04-12 08:43:45.000000 maginator-0.1.20/maginator/messages.py
-drwxr-xr-x   0 trizac   (198224) cu_10108  (1335)        0 2024-04-12 08:53:27.000000 maginator-0.1.20/maginator/workflow/
--rw-r--r--   0 trizac   (198224) cu_10108  (1335)     1354 2024-04-12 08:43:46.000000 maginator-0.1.20/maginator/workflow/alignment.Snakefile
-drwxr-xr-x   0 trizac   (198224) cu_10108  (1335)        0 2024-04-12 08:53:27.000000 maginator-0.1.20/maginator/workflow/envs/
--rw-r--r--   0 trizac   (198224) cu_10108  (1335)      102 2024-04-12 08:43:46.000000 maginator-0.1.20/maginator/workflow/envs/filter_geneclusters.yaml
--rw-r--r--   0 trizac   (198224) cu_10108  (1335)      185 2024-04-12 08:43:46.000000 maginator-0.1.20/maginator/workflow/envs/filter_gtdbtk.yaml
--rw-r--r--   0 trizac   (198224) cu_10108  (1335)      225 2024-04-12 08:43:46.000000 maginator-0.1.20/maginator/workflow/envs/phylo.yaml
--rw-r--r--   0 trizac   (198224) cu_10108  (1335)      248 2024-04-12 08:43:46.000000 maginator-0.1.20/maginator/workflow/envs/signature_genes.yaml
--rw-r--r--   0 trizac   (198224) cu_10108  (1335)     1152 2024-04-12 08:43:46.000000 maginator-0.1.20/maginator/workflow/filter.Snakefile
--rw-r--r--   0 trizac   (198224) cu_10108  (1335)     2636 2024-04-12 08:43:46.000000 maginator-0.1.20/maginator/workflow/filter_geneclusters.Snakefile
--rw-r--r--   0 trizac   (198224) cu_10108  (1335)     2618 2024-04-12 08:43:46.000000 maginator-0.1.20/maginator/workflow/gene_count_mat.Snakefile
--rw-r--r--   0 trizac   (198224) cu_10108  (1335)     2582 2024-04-12 08:43:46.000000 maginator-0.1.20/maginator/workflow/gene_tax.Snakefile
--rw-r--r--   0 trizac   (198224) cu_10108  (1335)     1652 2024-04-12 08:43:46.000000 maginator-0.1.20/maginator/workflow/gtdbtk.Snakefile
--rw-r--r--   0 trizac   (198224) cu_10108  (1335)     4921 2024-04-12 08:43:46.000000 maginator-0.1.20/maginator/workflow/outgroup.Snakefile
--rw-r--r--   0 trizac   (198224) cu_10108  (1335)     3165 2024-04-12 08:43:46.000000 maginator-0.1.20/maginator/workflow/parse_gtdbtk.Snakefile
--rw-r--r--   0 trizac   (198224) cu_10108  (1335)     1700 2024-04-12 08:43:46.000000 maginator-0.1.20/maginator/workflow/phylo.Snakefile
--rw-r--r--   0 trizac   (198224) cu_10108  (1335)     1321 2024-04-12 08:43:46.000000 maginator-0.1.20/maginator/workflow/pileup.Snakefile
--rw-r--r--   0 trizac   (198224) cu_10108  (1335)     2197 2024-04-12 08:46:12.000000 maginator-0.1.20/maginator/workflow/pileup_parse.Snakefile
--rw-r--r--   0 trizac   (198224) cu_10108  (1335)     3097 2024-04-12 08:43:46.000000 maginator-0.1.20/maginator/workflow/prescreening_genes.Snakefile
--rw-r--r--   0 trizac   (198224) cu_10108  (1335)    13552 2024-04-12 08:43:46.000000 maginator-0.1.20/maginator/workflow/reads_to_bins.Snakefile
-drwxr-xr-x   0 trizac   (198224) cu_10108  (1335)        0 2024-04-12 08:53:27.000000 maginator-0.1.20/maginator/workflow/scripts/
--rw-r--r--   0 trizac   (198224) cu_10108  (1335)     8844 2024-04-12 08:43:46.000000 maginator-0.1.20/maginator/workflow/scripts/Functions_v4.R
--rw-r--r--   0 trizac   (198224) cu_10108  (1335)     1067 2024-04-12 08:43:46.000000 maginator-0.1.20/maginator/workflow/scripts/MGS_counts.R
--rw-r--r--   0 trizac   (198224) cu_10108  (1335)    12658 2024-04-12 08:43:46.000000 maginator-0.1.20/maginator/workflow/scripts/SG_refinement.R
--rw-r--r--   0 trizac   (198224) cu_10108  (1335)     4608 2024-04-12 08:43:46.000000 maginator-0.1.20/maginator/workflow/scripts/abundance_profiles.R
--rw-r--r--   0 trizac   (198224) cu_10108  (1335)     2650 2024-04-12 08:46:51.000000 maginator-0.1.20/maginator/workflow/scripts/allele_frequency_mat.R
--rwxr-xr-x   0 trizac   (198224) cu_10108  (1335)     2154 2024-04-12 08:43:46.000000 maginator-0.1.20/maginator/workflow/scripts/concat.py
--rw-r--r--   0 trizac   (198224) cu_10108  (1335)     1445 2024-04-12 08:43:46.000000 maginator-0.1.20/maginator/workflow/scripts/filter.py
--rwxr-xr-x   0 trizac   (198224) cu_10108  (1335)     4156 2024-04-12 08:43:46.000000 maginator-0.1.20/maginator/workflow/scripts/gene_cluster2tax.py
--rw-r--r--   0 trizac   (198224) cu_10108  (1335)     4254 2024-04-12 08:43:46.000000 maginator-0.1.20/maginator/workflow/scripts/gene_refinement_plots.R
--rwxr-xr-x   0 trizac   (198224) cu_10108  (1335)    11347 2024-04-12 08:43:46.000000 maginator-0.1.20/maginator/workflow/scripts/marker_genes.py
--rw-r--r--   0 trizac   (198224) cu_10108  (1335)     1830 2024-04-12 08:43:46.000000 maginator-0.1.20/maginator/workflow/scripts/matrix2SG_formatconversion.R
--rwxr-xr-x   0 trizac   (198224) cu_10108  (1335)    20417 2024-04-12 08:43:46.000000 maginator-0.1.20/maginator/workflow/scripts/mpileup.py
--rw-r--r--   0 trizac   (198224) cu_10108  (1335)     5511 2024-04-12 08:43:46.000000 maginator-0.1.20/maginator/workflow/scripts/parse_gtdbtk.py
--rw-r--r--   0 trizac   (198224) cu_10108  (1335)     2878 2024-04-12 08:43:46.000000 maginator-0.1.20/maginator/workflow/scripts/prescreening_genes.R
--rw-r--r--   0 trizac   (198224) cu_10108  (1335)     1015 2024-04-12 08:43:46.000000 maginator-0.1.20/maginator/workflow/scripts/sort_gene_mat.py
--rw-r--r--   0 trizac   (198224) cu_10108  (1335)     3032 2024-04-12 08:43:46.000000 maginator-0.1.20/maginator/workflow/scripts/species_collections.py
--rwxr-xr-x   0 trizac   (198224) cu_10108  (1335)     1891 2024-04-12 08:43:46.000000 maginator-0.1.20/maginator/workflow/scripts/synteny.py
--rw-r--r--   0 trizac   (198224) cu_10108  (1335)     3991 2024-04-12 08:43:46.000000 maginator-0.1.20/maginator/workflow/signature_genes.Snakefile
--rw-r--r--   0 trizac   (198224) cu_10108  (1335)     4282 2024-04-12 08:43:46.000000 maginator-0.1.20/maginator/workflow.py
-drwxr-xr-x   0 trizac   (198224) cu_10108  (1335)        0 2024-04-12 08:53:27.000000 maginator-0.1.20/maginator.egg-info/
--rw-r--r--   0 trizac   (198224) cu_10108  (1335)    13123 2024-04-12 08:53:26.000000 maginator-0.1.20/maginator.egg-info/PKG-INFO
--rw-r--r--   0 trizac   (198224) cu_10108  (1335)     1868 2024-04-12 08:53:26.000000 maginator-0.1.20/maginator.egg-info/SOURCES.txt
--rw-r--r--   0 trizac   (198224) cu_10108  (1335)        1 2024-04-12 08:53:26.000000 maginator-0.1.20/maginator.egg-info/dependency_links.txt
--rw-r--r--   0 trizac   (198224) cu_10108  (1335)       50 2024-04-12 08:53:26.000000 maginator-0.1.20/maginator.egg-info/entry_points.txt
--rw-r--r--   0 trizac   (198224) cu_10108  (1335)        1 2024-04-12 08:53:26.000000 maginator-0.1.20/maginator.egg-info/not-zip-safe
--rw-r--r--   0 trizac   (198224) cu_10108  (1335)       11 2024-04-12 08:53:26.000000 maginator-0.1.20/maginator.egg-info/requires.txt
--rw-r--r--   0 trizac   (198224) cu_10108  (1335)       10 2024-04-12 08:53:26.000000 maginator-0.1.20/maginator.egg-info/top_level.txt
--rw-r--r--   0 trizac   (198224) cu_10108  (1335)       38 2024-04-12 08:53:27.000000 maginator-0.1.20/setup.cfg
--rw-r--r--   0 trizac   (198224) cu_10108  (1335)     1136 2024-04-12 08:44:29.000000 maginator-0.1.20/setup.py
+drwxrwxr-x   0 jakrus   (23790) cu_10108  (1335)        0 2022-12-15 11:14:01.000000 maginator-0.1.8/
+-rw-r--r--   0 jakrus   (23790) cu_10108  (1335)       39 2022-08-12 13:39:00.000000 maginator-0.1.8/MANIFEST.in
+-rw-rw-r--   0 jakrus   (23790) cu_10108  (1335)     8389 2022-12-15 11:14:01.000000 maginator-0.1.8/PKG-INFO
+-rw-rw-r--   0 jakrus   (23790) cu_10108  (1335)     6810 2022-12-12 10:01:51.000000 maginator-0.1.8/README.md
+drwxrwxr-x   0 jakrus   (23790) cu_10108  (1335)        0 2022-12-15 11:14:01.000000 maginator-0.1.8/maginator/
+-rw-rw-r--   0 jakrus   (23790) cu_10108  (1335)       42 2022-05-11 10:03:11.000000 maginator-0.1.8/maginator/__init__.py
+-rw-rw-r--   0 jakrus   (23790) cu_10108  (1335)     5499 2022-12-14 11:04:15.000000 maginator-0.1.8/maginator/controller.py
+-rwxrwxr-x   0 jakrus   (23790) cu_10108  (1335)     9113 2022-12-09 20:14:59.000000 maginator-0.1.8/maginator/main.py
+-rw-r--r--   0 jakrus   (23790) cu_10108  (1335)     2912 2022-12-14 08:21:01.000000 maginator-0.1.8/maginator/messages.py
+drwxrwxr-x   0 jakrus   (23790) cu_10108  (1335)        0 2022-12-15 11:14:01.000000 maginator-0.1.8/maginator/workflow/
+-rw-rw-r--   0 jakrus   (23790) cu_10108  (1335)     1340 2022-11-28 15:59:15.000000 maginator-0.1.8/maginator/workflow/alignment.Snakefile
+drwxrwxr-x   0 jakrus   (23790) cu_10108  (1335)        0 2022-12-15 11:14:01.000000 maginator-0.1.8/maginator/workflow/envs/
+-rw-rw-r--   0 jakrus   (23790) cu_10108  (1335)      102 2022-10-24 13:10:29.000000 maginator-0.1.8/maginator/workflow/envs/filter_geneclusters.yaml
+-rw-rw-r--   0 jakrus   (23790) cu_10108  (1335)      167 2022-10-24 13:10:29.000000 maginator-0.1.8/maginator/workflow/envs/filter_gtdbtk.yaml
+-rw-rw-r--   0 jakrus   (23790) cu_10108  (1335)      225 2022-12-09 15:01:57.000000 maginator-0.1.8/maginator/workflow/envs/phylo.yaml
+-rw-rw-r--   0 jakrus   (23790) cu_10108  (1335)      248 2022-10-24 13:10:29.000000 maginator-0.1.8/maginator/workflow/envs/signature_genes.yaml
+-rw-rw-r--   0 jakrus   (23790) cu_10108  (1335)     1092 2022-12-14 11:03:01.000000 maginator-0.1.8/maginator/workflow/filter.Snakefile
+-rw-rw-r--   0 jakrus   (23790) cu_10108  (1335)     2621 2022-11-29 19:14:46.000000 maginator-0.1.8/maginator/workflow/filter_geneclusters.Snakefile
+-rw-rw-r--   0 jakrus   (23790) cu_10108  (1335)     2594 2022-11-29 12:04:28.000000 maginator-0.1.8/maginator/workflow/gene_count_mat.Snakefile
+-rw-rw-r--   0 jakrus   (23790) cu_10108  (1335)     2564 2022-12-09 17:10:21.000000 maginator-0.1.8/maginator/workflow/gene_tax.Snakefile
+-rw-rw-r--   0 jakrus   (23790) cu_10108  (1335)     1344 2022-12-13 20:43:55.000000 maginator-0.1.8/maginator/workflow/gtdbtk.Snakefile
+-rw-rw-r--   0 jakrus   (23790) cu_10108  (1335)     4873 2022-12-06 11:16:49.000000 maginator-0.1.8/maginator/workflow/outgroup.Snakefile
+-rw-rw-r--   0 jakrus   (23790) cu_10108  (1335)     3132 2022-12-14 11:03:53.000000 maginator-0.1.8/maginator/workflow/parse_gtdbtk.Snakefile
+-rw-rw-r--   0 jakrus   (23790) cu_10108  (1335)     1689 2022-11-30 11:13:56.000000 maginator-0.1.8/maginator/workflow/phylo.Snakefile
+-rw-rw-r--   0 jakrus   (23790) cu_10108  (1335)     1308 2022-11-29 12:02:15.000000 maginator-0.1.8/maginator/workflow/pileup.Snakefile
+-rw-rw-r--   0 jakrus   (23790) cu_10108  (1335)     1567 2022-12-09 20:13:36.000000 maginator-0.1.8/maginator/workflow/pileup_parse.Snakefile
+-rw-rw-r--   0 jakrus   (23790) cu_10108  (1335)     2981 2022-11-29 12:05:08.000000 maginator-0.1.8/maginator/workflow/prescreening_genes.Snakefile
+drwxrwxr-x   0 jakrus   (23790) cu_10108  (1335)        0 2022-12-15 11:14:01.000000 maginator-0.1.8/maginator/workflow/scripts/
+-rw-rw-r--   0 jakrus   (23790) cu_10108  (1335)     8844 2022-11-14 19:28:09.000000 maginator-0.1.8/maginator/workflow/scripts/Functions_v4.R
+-rw-rw-r--   0 jakrus   (23790) cu_10108  (1335)     1067 2022-11-14 19:28:09.000000 maginator-0.1.8/maginator/workflow/scripts/MGS_counts.R
+-rw-rw-r--   0 jakrus   (23790) cu_10108  (1335)    11430 2022-11-29 12:14:51.000000 maginator-0.1.8/maginator/workflow/scripts/SG_refinement.R
+-rw-rw-r--   0 jakrus   (23790) cu_10108  (1335)     4549 2022-11-22 15:34:34.000000 maginator-0.1.8/maginator/workflow/scripts/abundance_profiles.R
+-rwxrwxr-x   0 jakrus   (23790) cu_10108  (1335)     2154 2022-11-28 20:30:52.000000 maginator-0.1.8/maginator/workflow/scripts/concat.py
+-rw-rw-r--   0 jakrus   (23790) cu_10108  (1335)     1445 2022-08-22 19:30:30.000000 maginator-0.1.8/maginator/workflow/scripts/filter.py
+-rwxr-xr-x   0 jakrus   (23790) cu_10108  (1335)     4156 2022-12-09 18:29:09.000000 maginator-0.1.8/maginator/workflow/scripts/gene_cluster2tax.py
+-rwxrwxr-x   0 jakrus   (23790) cu_10108  (1335)    11347 2022-11-29 10:54:29.000000 maginator-0.1.8/maginator/workflow/scripts/marker_genes.py
+-rw-rw-r--   0 jakrus   (23790) cu_10108  (1335)     1806 2022-11-22 11:03:56.000000 maginator-0.1.8/maginator/workflow/scripts/matrix2SG_formatconversion.R
+-rwxrwxr-x   0 jakrus   (23790) cu_10108  (1335)    20417 2022-12-09 20:13:44.000000 maginator-0.1.8/maginator/workflow/scripts/mpileup.py
+-rw-rw-r--   0 jakrus   (23790) cu_10108  (1335)     5310 2022-12-14 10:51:45.000000 maginator-0.1.8/maginator/workflow/scripts/parse_gtdbtk.py
+-rw-rw-r--   0 jakrus   (23790) cu_10108  (1335)     2832 2022-12-15 09:51:39.000000 maginator-0.1.8/maginator/workflow/scripts/prescreening_genes.R
+-rw-rw-r--   0 jakrus   (23790) cu_10108  (1335)     1015 2022-10-24 13:10:29.000000 maginator-0.1.8/maginator/workflow/scripts/sort_gene_mat.py
+-rw-rw-r--   0 jakrus   (23790) cu_10108  (1335)     3032 2022-11-25 18:10:20.000000 maginator-0.1.8/maginator/workflow/scripts/species_collections.py
+-rwxr-xr-x   0 jakrus   (23790) cu_10108  (1335)     1891 2022-12-09 14:17:30.000000 maginator-0.1.8/maginator/workflow/scripts/synteny.py
+-rw-rw-r--   0 jakrus   (23790) cu_10108  (1335)     2757 2022-11-29 11:54:50.000000 maginator-0.1.8/maginator/workflow/signature_genes.Snakefile
+-rw-r--r--   0 jakrus   (23790) cu_10108  (1335)     4268 2022-12-13 11:34:04.000000 maginator-0.1.8/maginator/workflow.py
+drwxrwxr-x   0 jakrus   (23790) cu_10108  (1335)        0 2022-12-15 11:14:01.000000 maginator-0.1.8/maginator.egg-info/
+-rw-rw-r--   0 jakrus   (23790) cu_10108  (1335)     8389 2022-12-15 11:14:00.000000 maginator-0.1.8/maginator.egg-info/PKG-INFO
+-rw-rw-r--   0 jakrus   (23790) cu_10108  (1335)     1724 2022-12-15 11:14:00.000000 maginator-0.1.8/maginator.egg-info/SOURCES.txt
+-rw-rw-r--   0 jakrus   (23790) cu_10108  (1335)        1 2022-12-15 11:14:00.000000 maginator-0.1.8/maginator.egg-info/dependency_links.txt
+-rw-rw-r--   0 jakrus   (23790) cu_10108  (1335)       50 2022-12-15 11:14:00.000000 maginator-0.1.8/maginator.egg-info/entry_points.txt
+-rw-rw-r--   0 jakrus   (23790) cu_10108  (1335)        1 2022-12-15 11:14:00.000000 maginator-0.1.8/maginator.egg-info/not-zip-safe
+-rw-rw-r--   0 jakrus   (23790) cu_10108  (1335)       11 2022-12-15 11:14:00.000000 maginator-0.1.8/maginator.egg-info/requires.txt
+-rw-rw-r--   0 jakrus   (23790) cu_10108  (1335)       10 2022-12-15 11:14:00.000000 maginator-0.1.8/maginator.egg-info/top_level.txt
+-rw-rw-r--   0 jakrus   (23790) cu_10108  (1335)       38 2022-12-15 11:14:01.000000 maginator-0.1.8/setup.cfg
+-rw-rw-r--   0 jakrus   (23790) cu_10108  (1335)     1085 2022-12-13 09:51:10.000000 maginator-0.1.8/setup.py
```

### Comparing `maginator-0.1.20/PKG-INFO` & `maginator-0.1.8/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: maginator
-Version: 0.1.20
+Version: 0.1.8
 Summary: MAGinator: Abundance, strain, and functional profiling of MAGs
 Home-page: https://github.com/Russel88/MAGinator
-Author: Jakob Russel & Trine Zachariasen
-Author-email: russel2620@gmail.com,trine_zachariasen@hotmail.com
+Author: Jakob Russel
+Author-email: russel2620@gmail.com
 License: UNKNOWN
 Description: [![Project Status: Active - The project has reached a stable, usable state and is being actively developed.](http://www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/#active)
         
         # MAGinator
         
         Combining the strengths of contig and gene based methods to provide:
         
@@ -24,128 +24,65 @@
         ## Installation
         
         All you need for running MAGinator is snakemake and mamba. Other dependencies will be installed by snakemake automatically.
         
         ```sh
         conda create -n maginator -c bioconda -c conda-forge snakemake mamba
         conda activate maginator
-        pip install maginator
+        git clone https://github.com/Russel88/MAGinator.git
+        cd MAGinator
+        pip install .
         ```
         
-        Furthermore, MAGinator also needs the GTDB-tk database downloaded. Here we download release 214. If you don't already have it, you can run the following:
+        Furthermore, MAGinator also needs the GTDB-tk database version R207_v2 downloaded. If you don't already have it, you can run the following:
         ```sh
-        wget https://data.ace.uq.edu.au/public/gtdb/data/releases/release214/214.1/auxillary_files/gtdbtk_r214_data.tar.gz
-        tar xvzf *.tar.gz
+        wget https://data.gtdb.ecogenomic.org/releases/latest/auxillary_files/gtdbtk_v2_data.tar.gz
+        tar xvzf gtdbtk_v2_data.tar.gz
         ```
         
         ## Usage
         
         MAGinator needs 3 input files:
         
         * The clusters.tsv files from [VAMB](https://github.com/RasmussenLab/vamb)
         * A fasta file with sequences of all contigs, with unique names
         * A comma-separated file giving the position of the fastq files with your sequencing reads formatted as: SampleName,PathToForwardReads,PathToReverseReads
         
         Run MAGinator:
         ```sh
-        maginator -v vamb_clusters.tsv -r reads.csv -c contigs.fasta -o my_output -g "/path/to/GTDB-Tk/database/release214/"
+        maginator -v vamb_clusters.tsv -r reads.csv -c contigs.fasta -o my_output -g "/path/to/GTDB-Tk/database/release207_v2/"
         ```
         
-        A testset can be found in the test_data directory. 
-        1. Download the 3 samples used for the test at SRA: https://www.ncbi.nlm.nih.gov/sra?LinkName=bioproject_sra_all&from_uid=715601 with the ID's dfc99c_A, f9d84e_A and 221641_A
-        2. Change the paths to the read-files in reads.csv
-        3. Unzip the contigs.fasta.gz 
-        4. Run MAGinator
-        
         ### Run on a compute cluster
         MAGinator can run on compute clusters using qsub (torque), sbatch (slurm), or drmaa structures. The --cluster argument toggles the type of compute cluster infrastructure. The --cluster_info argument toggles the information given to the submission command, and it has to contain the following keywords {cores}, {memory}, {runtime}, which are used to forward resource information to the cluster.
         
         A qsub MAGinator can for example be run with the following command (... indicates required arguments, see above):
         ```sh
         maginator ... --cluster qsub --cluster_info "-l nodes=1:ppn={cores}:thinnode,mem={memory}gb,walltime={runtime}"
         ```
         
-        ## Test data
-        
-        A test set can be found in the maginator/test_data directory. 
-        1. Download the 3 samples used for the test at SRA: https://www.ncbi.nlm.nih.gov/sra?LinkName=bioproject_sra_all&from_uid=715601 with the ID's dfc99c_A, f9d84e_A and 221641_A
-        2. Clone repo: git clone https://github.com/Russel88/MAGinator.git
-        3. Change the paths to the read-files in reads.csv
-        4. Unzip the contigs.fasta.gz 
-        5. Run MAGinator
-        
-        MAGinator can been run on the test data on a slurm server with the following command:
-        ```sh
-        maginator --vamb_clusters clusters.tsv --reads reads.csv --contigs contigs.fasta --gtdb_db data/release214/ --output test_out --cluster slurm --cluster_info "-n {cores} --mem {mem_gb}gb -t {runtime}" --max_mem 180
-        ```
-        The expected output can be found as a zipped file on Zenodo: https://doi.org/10.5281/zenodo.8279036. MAGinator has been run on the test data (using GTDB-tk db release207_v2) on a slurm server.
-        
-        On the compute cluster each job have had access to 180gb RAM, with the following time consumption: 
-        real	72m27.379s
-        user	0m18.830s
-        sys	1m0.454s
-        
-        If you run on a smaller server you can set the parameters --max_cores and --max_mem.
-        
-        ## Recommended workflow 
-        
-        To generate the input files to run MAGinator we have created a recommended workflow, with preprocessing, assembly and binning* of your metagenomics reads (the rules for binning have been copied from VAMB (https://github.com/RasmussenLab/vamb/blob/master/workflow/)). 
-        It has been setup as a snakefile in recommended_workflow/reads_to_bins.Snakefile.
-        
-        The input to the workflow is the reads.csv file. The workflow can be run using snakemake:
-        ```
-        snakemake --use-conda -s reads_to_bins.Snakefile --resources mem_gb=180 --config reads=reads.csv --cores 10 --printshellcmds 
-        ```
-        
-        Preparing data for MAGinator run
-        ```
-        sed 's/@/_/g' assembly/all_assemblies.fasta > all_assemblies.fasta
-        sed 's/@/_/g' vamb/clusters.tsv > clusters.tsv
-        ```
-        
-        Now you are ready to run MAGinator.
-        
-        ## Functional Annotation
-        
-        To generate the functional annotation of the genes we recommend using EggNOG mapper (https://github.com/eggnogdb/eggnog-mapper).
-        
-        You can download it and try to run it on the test data
-        ```sh
-        mkdir test_out/functional_annotation
-        emapper.py -i test/genes/all_genes_rep_seq.fasta --output test_out/functional_annotation -m diamond --cpu 38
-        ```
-        
-        The eggNOG output can be merged with clusters.tsv and further processed to obtain functional annotations of the MAG, cluster or sample levels with the following command:
-        ```sh
-        (echo -e '#sample\tMAG_cluster\tMAG\tfunction'; join -1 1 -2 1 <(awk '{print $2 "\t" $1}' clusters.tsv | sort) <(tail -n +6 annotations.tsv | head -n -3 | cut -f1,15 | grep -v '\-$' | sed 's/_[[:digit:]]\+\t/\t/' | sed 's/,/\n/g' | perl -lane '{$q = $F[0] if $#F > 0; unshift(@F, $q) if $#F == 0}; print "$F[0]\t$F[1]"' | sed 's/\tko:/\t/' | sort) | awk '{print $2 "\t" $2 "\t" $3}' | sed 's/_/\t/' | sort -k1,1 -k2,2n) > MAGfunctions.tsv
-        ```
-        In this case the KEGG ortholog column 15 was picked from the eggNOG-mapper output. But by cutting e.g. column number 13, one would obtain GO terms instead. Refer to the header of the eggNOG-mapper output for other available functional annotations e.g. KEGG pathways, Pfam, CAZy, COGs, etc.
-        
-        
         ## MAGinator workflow
         
         This is what MAGinator does with your input (if you want to see all parameters run maginator --help):
         * Filter bins by size
             * Use --binsize to control the cutoff
         * Run GTDB-tk to taxonomically annotate bins and call open reading frames (ORFs)
         * Group your VAMB clusters into metagenomic species (MGS) based on the taxonomic annotation. (Unannotated VAMB clusters are kept in the pipeline, but left unchanged)
             * Use --no_mgs to disable this
             * Use --annotation_prevalence to change how prevalent an annotation has to be in a VAMB cluster to call taxonomic consensus
         * Cluster your ORFs into gene clusters to get a non-redundant gene catalogue
             * Use --clustering_min_seq_id to toggle the clustering identity
             * Use --clustering_coverage to toggle the clustering coverage
             * Use --clustering_type to toggle whether to cluster on amino acid or nucleotide level
         * Map reads to the non-redundant gene catalogue and create a matrix with gene counts for each sample
-        * Pick non-redundant genes that are only found in one MAG cluster each
-        * Fit signature gene model and use the resulting signature genes to get the abundance of each MAG cluster
-            * Use --min_mapped_signature_genes to change minimum number of signature genes to be detected in the sample to be included in the analysis
-            * Use --min_samples to alter the number of samples with the MAG cluster present in order to perform signature gene refinement
-        * Prepare for generation of phylogenies for each MAG cluster by finding outgroups and marker genes which will be used for rooting the phylogenies
+        * Pick non-redundant genes that are only found in one MGS each
+        * Fit signature gene model and use the resulting signature genes to get the abundance of each MGS
+        * Prepare for generation of phylogenies for each MGS by finding outgroups and marker genes which will be used for rooting the phylogenies
         * Use the read mappings to collect SNV information for each signature gene and marker gene for each sample
-        * Align signature and marker genes, concatenate alignments and infer phylogenetic trees for each MAG cluster
+        * Align signature and marker genes, concatenate alignments and infer phylogenetic trees for each MGS
             * Use --phylo to toggle whether use fasttree (fast, approximate) or iqtree (slow, precise) to infer phylogenies
         * Infer the taxonomic scope of each gene cluster. That is, at what taxonomic level are genes from a given gene cluster found in
             * Use --tax_scope_threshold to toggle the threshold for how to find the taxonomic scope consensus
         * Cluster gene clusters into synteny clusters based on how often they are found adjacent on contigs
         
         
         ## Output
@@ -157,38 +94,35 @@
         * genes/
             * all_genes.faa - Amino acid sequences of all ORFs
             * all_genes.fna - Nucletotide sequences of all ORFs
             * all_genes_nonredundant.fasta - Nucleotide sequences of gene cluster representatives
             * all_genes_cluster.tsv - Gene clusters
             * matrix/
                 * gene_count_matrix.tsv - Read count for each gene cluster for each sample
-                * small_gene_count_matrix.tsv - Read count matrix only containing the genes, that does not cluster across MAG cluster
             * synteny/ - Intermediate files for synteny clustering of gene clusters
         * gtdbtk/
             * <cluster>/ - GTDB-tk taxonomic annotation for each VAMB cluster
         * logs/ - Log files
         * mapped_reads/
             * bams/ - Bam files for mapping reads to gene clusters
         * phylo/
             * alignments/ - Alignments for each signature gene
-            * cluster_alignments/ - Concatenated alignments for each MAG cluster
-            * pileup/ - SNV information for each MAG cluster and each sample
-            * trees/ - Phylogenetic trees for each MAG cluster
+            * cluster_alignments/ - Concatenated alignments for each MGS
+            * pileup/ - SNV information for each MGS and each sample
+            * trees/ - Phylogenetic trees for each MGS
             * stats.tab - Mapping information such as non-N fraction, number of signature genes and marker genes, read depth, and number of bases not reaching allele frequency cutoff 
             * stats_genes.tab - Same as above but the information is split per gene
-        * signature_genes/ 
-            * \- R data files with signature gene optimization
-            * read-count_detected-genes.pdf - Figure for each MAG cluster displaying number of identified SG's in each sample along with the number of reads mapped.
+        * signature_genes/ - R data files with signature gene optimization
         * tabs/
             * gene_cluster_bins.tab - Table listing which bins each gene cluster was found in
             * gene_cluster_tax_scope.tab - Table listing the taxonomic scope of each gene cluster
-            * metagenomicspecies.tab - Table listing which, if any, clusters where merged in MAG cluster and the taxonomy of those
-            * signature_genes_cluster.tsv - Table with the signature genes for each MAG cluster
+            * metagenomicspecies.tab - Table listing which, if any, clusters where merged in MGS and the taxonomy of those
+            * signature_genes_cluster.tsv - Table with the signature genes for each MGS/cluster
             * synteny_clusters.tab - Table listing the synteny cluster association for the gene clusters. Gene clusters from the same synteny cluster are genomically adjacent.
-            * tax_matrix.tsv - Table with taxonomy information for MAG cluster
+            * tax_matrix.tsv - Table with taxonomy information for MGS
             
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

### Comparing `maginator-0.1.20/README.md` & `maginator-0.1.8/maginator.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,180 +1,132 @@
-[![Project Status: Active - The project has reached a stable, usable state and is being actively developed.](http://www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/#active)
-
-# MAGinator
-
-Combining the strengths of contig and gene based methods to provide:
-
-* Accurate abundances of species using de novo signature genes
-    * MAGinator uses a statistical model to find the best genes for calculating accurate abundances
-* SNV-level resolution phylogenetic trees based on signature genes
-    * MAGinator creates a phylogenetic tree for each species so you can associate your metadata with subspecies/strain level differences
-* Connect accessory genome to the species annotation by getting a taxonomic scope for gene clusters
-    * MAGinator clusters all ORFs into gene clusters and for each gene cluster you will know which taxonomic level it is specific to
-* Improve your functional annotation by grouping your genes in synteny clusters based on genomic adjacency
-    * MAGinator clusters gene clusters into synteny clusters - Syntenic genes are usually part of the same pathway or have similar functions 
-
-## Installation
-
-All you need for running MAGinator is snakemake and mamba. Other dependencies will be installed by snakemake automatically.
-
-```sh
-conda create -n maginator -c bioconda -c conda-forge snakemake mamba
-conda activate maginator
-pip install maginator
-```
-
-Furthermore, MAGinator also needs the GTDB-tk database downloaded. Here we download release 214. If you don't already have it, you can run the following:
-```sh
-wget https://data.ace.uq.edu.au/public/gtdb/data/releases/release214/214.1/auxillary_files/gtdbtk_r214_data.tar.gz
-tar xvzf *.tar.gz
-```
-
-## Usage
-
-MAGinator needs 3 input files:
-
-* The clusters.tsv files from [VAMB](https://github.com/RasmussenLab/vamb)
-* A fasta file with sequences of all contigs, with unique names
-* A comma-separated file giving the position of the fastq files with your sequencing reads formatted as: SampleName,PathToForwardReads,PathToReverseReads
-
-Run MAGinator:
-```sh
-maginator -v vamb_clusters.tsv -r reads.csv -c contigs.fasta -o my_output -g "/path/to/GTDB-Tk/database/release214/"
-```
-
-A testset can be found in the test_data directory. 
-1. Download the 3 samples used for the test at SRA: https://www.ncbi.nlm.nih.gov/sra?LinkName=bioproject_sra_all&from_uid=715601 with the ID's dfc99c_A, f9d84e_A and 221641_A
-2. Change the paths to the read-files in reads.csv
-3. Unzip the contigs.fasta.gz 
-4. Run MAGinator
-
-### Run on a compute cluster
-MAGinator can run on compute clusters using qsub (torque), sbatch (slurm), or drmaa structures. The --cluster argument toggles the type of compute cluster infrastructure. The --cluster_info argument toggles the information given to the submission command, and it has to contain the following keywords {cores}, {memory}, {runtime}, which are used to forward resource information to the cluster.
-
-A qsub MAGinator can for example be run with the following command (... indicates required arguments, see above):
-```sh
-maginator ... --cluster qsub --cluster_info "-l nodes=1:ppn={cores}:thinnode,mem={memory}gb,walltime={runtime}"
-```
-
-## Test data
-
-A test set can be found in the maginator/test_data directory. 
-1. Download the 3 samples used for the test at SRA: https://www.ncbi.nlm.nih.gov/sra?LinkName=bioproject_sra_all&from_uid=715601 with the ID's dfc99c_A, f9d84e_A and 221641_A
-2. Clone repo: git clone https://github.com/Russel88/MAGinator.git
-3. Change the paths to the read-files in reads.csv
-4. Unzip the contigs.fasta.gz 
-5. Run MAGinator
-
-MAGinator can been run on the test data on a slurm server with the following command:
-```sh
-maginator --vamb_clusters clusters.tsv --reads reads.csv --contigs contigs.fasta --gtdb_db data/release214/ --output test_out --cluster slurm --cluster_info "-n {cores} --mem {mem_gb}gb -t {runtime}" --max_mem 180
-```
-The expected output can be found as a zipped file on Zenodo: https://doi.org/10.5281/zenodo.8279036. MAGinator has been run on the test data (using GTDB-tk db release207_v2) on a slurm server.
-
-On the compute cluster each job have had access to 180gb RAM, with the following time consumption: 
-real	72m27.379s
-user	0m18.830s
-sys	1m0.454s
-
-If you run on a smaller server you can set the parameters --max_cores and --max_mem.
-
-## Recommended workflow 
-
-To generate the input files to run MAGinator we have created a recommended workflow, with preprocessing, assembly and binning* of your metagenomics reads (the rules for binning have been copied from VAMB (https://github.com/RasmussenLab/vamb/blob/master/workflow/)). 
-It has been setup as a snakefile in recommended_workflow/reads_to_bins.Snakefile.
-
-The input to the workflow is the reads.csv file. The workflow can be run using snakemake:
-```
-snakemake --use-conda -s reads_to_bins.Snakefile --resources mem_gb=180 --config reads=reads.csv --cores 10 --printshellcmds 
-```
-
-Preparing data for MAGinator run
-```
-sed 's/@/_/g' assembly/all_assemblies.fasta > all_assemblies.fasta
-sed 's/@/_/g' vamb/clusters.tsv > clusters.tsv
-```
-
-Now you are ready to run MAGinator.
-
-## Functional Annotation
-
-To generate the functional annotation of the genes we recommend using EggNOG mapper (https://github.com/eggnogdb/eggnog-mapper).
-
-You can download it and try to run it on the test data
-```sh
-mkdir test_out/functional_annotation
-emapper.py -i test/genes/all_genes_rep_seq.fasta --output test_out/functional_annotation -m diamond --cpu 38
-```
-
-The eggNOG output can be merged with clusters.tsv and further processed to obtain functional annotations of the MAG, cluster or sample levels with the following command:
-```sh
-(echo -e '#sample\tMAG_cluster\tMAG\tfunction'; join -1 1 -2 1 <(awk '{print $2 "\t" $1}' clusters.tsv | sort) <(tail -n +6 annotations.tsv | head -n -3 | cut -f1,15 | grep -v '\-$' | sed 's/_[[:digit:]]\+\t/\t/' | sed 's/,/\n/g' | perl -lane '{$q = $F[0] if $#F > 0; unshift(@F, $q) if $#F == 0}; print "$F[0]\t$F[1]"' | sed 's/\tko:/\t/' | sort) | awk '{print $2 "\t" $2 "\t" $3}' | sed 's/_/\t/' | sort -k1,1 -k2,2n) > MAGfunctions.tsv
-```
-In this case the KEGG ortholog column 15 was picked from the eggNOG-mapper output. But by cutting e.g. column number 13, one would obtain GO terms instead. Refer to the header of the eggNOG-mapper output for other available functional annotations e.g. KEGG pathways, Pfam, CAZy, COGs, etc.
-
-
-## MAGinator workflow
-
-This is what MAGinator does with your input (if you want to see all parameters run maginator --help):
-* Filter bins by size
-    * Use --binsize to control the cutoff
-* Run GTDB-tk to taxonomically annotate bins and call open reading frames (ORFs)
-* Group your VAMB clusters into metagenomic species (MGS) based on the taxonomic annotation. (Unannotated VAMB clusters are kept in the pipeline, but left unchanged)
-    * Use --no_mgs to disable this
-    * Use --annotation_prevalence to change how prevalent an annotation has to be in a VAMB cluster to call taxonomic consensus
-* Cluster your ORFs into gene clusters to get a non-redundant gene catalogue
-    * Use --clustering_min_seq_id to toggle the clustering identity
-    * Use --clustering_coverage to toggle the clustering coverage
-    * Use --clustering_type to toggle whether to cluster on amino acid or nucleotide level
-* Map reads to the non-redundant gene catalogue and create a matrix with gene counts for each sample
-* Pick non-redundant genes that are only found in one MAG cluster each
-* Fit signature gene model and use the resulting signature genes to get the abundance of each MAG cluster
-    * Use --min_mapped_signature_genes to change minimum number of signature genes to be detected in the sample to be included in the analysis
-    * Use --min_samples to alter the number of samples with the MAG cluster present in order to perform signature gene refinement
-* Prepare for generation of phylogenies for each MAG cluster by finding outgroups and marker genes which will be used for rooting the phylogenies
-* Use the read mappings to collect SNV information for each signature gene and marker gene for each sample
-* Align signature and marker genes, concatenate alignments and infer phylogenetic trees for each MAG cluster
-    * Use --phylo to toggle whether use fasttree (fast, approximate) or iqtree (slow, precise) to infer phylogenies
-* Infer the taxonomic scope of each gene cluster. That is, at what taxonomic level are genes from a given gene cluster found in
-    * Use --tax_scope_threshold to toggle the threshold for how to find the taxonomic scope consensus
-* Cluster gene clusters into synteny clusters based on how often they are found adjacent on contigs
-
-
-## Output
-
-* abundance/
-    * abundance_phyloseq.RData - Phyloseq object for R, with abundance and taxonomic data
-* clusters/
-    * <cluster>/<bin>.fa - Fasta files with nucleotide sequence of bins
-* genes/
-    * all_genes.faa - Amino acid sequences of all ORFs
-    * all_genes.fna - Nucletotide sequences of all ORFs
-    * all_genes_nonredundant.fasta - Nucleotide sequences of gene cluster representatives
-    * all_genes_cluster.tsv - Gene clusters
-    * matrix/
-        * gene_count_matrix.tsv - Read count for each gene cluster for each sample
-        * small_gene_count_matrix.tsv - Read count matrix only containing the genes, that does not cluster across MAG cluster
-    * synteny/ - Intermediate files for synteny clustering of gene clusters
-* gtdbtk/
-    * <cluster>/ - GTDB-tk taxonomic annotation for each VAMB cluster
-* logs/ - Log files
-* mapped_reads/
-    * bams/ - Bam files for mapping reads to gene clusters
-* phylo/
-    * alignments/ - Alignments for each signature gene
-    * cluster_alignments/ - Concatenated alignments for each MAG cluster
-    * pileup/ - SNV information for each MAG cluster and each sample
-    * trees/ - Phylogenetic trees for each MAG cluster
-    * stats.tab - Mapping information such as non-N fraction, number of signature genes and marker genes, read depth, and number of bases not reaching allele frequency cutoff 
-    * stats_genes.tab - Same as above but the information is split per gene
-* signature_genes/ 
-    * \- R data files with signature gene optimization
-    * read-count_detected-genes.pdf - Figure for each MAG cluster displaying number of identified SG's in each sample along with the number of reads mapped.
-* tabs/
-    * gene_cluster_bins.tab - Table listing which bins each gene cluster was found in
-    * gene_cluster_tax_scope.tab - Table listing the taxonomic scope of each gene cluster
-    * metagenomicspecies.tab - Table listing which, if any, clusters where merged in MAG cluster and the taxonomy of those
-    * signature_genes_cluster.tsv - Table with the signature genes for each MAG cluster
-    * synteny_clusters.tab - Table listing the synteny cluster association for the gene clusters. Gene clusters from the same synteny cluster are genomically adjacent.
-    * tax_matrix.tsv - Table with taxonomy information for MAG cluster
-    
+Metadata-Version: 2.1
+Name: maginator
+Version: 0.1.8
+Summary: MAGinator: Abundance, strain, and functional profiling of MAGs
+Home-page: https://github.com/Russel88/MAGinator
+Author: Jakob Russel
+Author-email: russel2620@gmail.com
+License: UNKNOWN
+Description: [![Project Status: Active - The project has reached a stable, usable state and is being actively developed.](http://www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/#active)
+        
+        # MAGinator
+        
+        Combining the strengths of contig and gene based methods to provide:
+        
+        * Accurate abundances of species using de novo signature genes
+            * MAGinator uses a statistical model to find the best genes for calculating accurate abundances
+        * SNV-level resolution phylogenetic trees based on signature genes
+            * MAGinator creates a phylogenetic tree for each species so you can associate your metadata with subspecies/strain level differences
+        * Connect accessory genome to the species annotation by getting a taxonomic scope for gene clusters
+            * MAGinator clusters all ORFs into gene clusters and for each gene cluster you will know which taxonomic level it is specific to
+        * Improve your functional annotation by grouping your genes in synteny clusters based on genomic adjacency
+            * MAGinator clusters gene clusters into synteny clusters - Syntenic genes are usually part of the same pathway or have similar functions 
+        
+        ## Installation
+        
+        All you need for running MAGinator is snakemake and mamba. Other dependencies will be installed by snakemake automatically.
+        
+        ```sh
+        conda create -n maginator -c bioconda -c conda-forge snakemake mamba
+        conda activate maginator
+        git clone https://github.com/Russel88/MAGinator.git
+        cd MAGinator
+        pip install .
+        ```
+        
+        Furthermore, MAGinator also needs the GTDB-tk database version R207_v2 downloaded. If you don't already have it, you can run the following:
+        ```sh
+        wget https://data.gtdb.ecogenomic.org/releases/latest/auxillary_files/gtdbtk_v2_data.tar.gz
+        tar xvzf gtdbtk_v2_data.tar.gz
+        ```
+        
+        ## Usage
+        
+        MAGinator needs 3 input files:
+        
+        * The clusters.tsv files from [VAMB](https://github.com/RasmussenLab/vamb)
+        * A fasta file with sequences of all contigs, with unique names
+        * A comma-separated file giving the position of the fastq files with your sequencing reads formatted as: SampleName,PathToForwardReads,PathToReverseReads
+        
+        Run MAGinator:
+        ```sh
+        maginator -v vamb_clusters.tsv -r reads.csv -c contigs.fasta -o my_output -g "/path/to/GTDB-Tk/database/release207_v2/"
+        ```
+        
+        ### Run on a compute cluster
+        MAGinator can run on compute clusters using qsub (torque), sbatch (slurm), or drmaa structures. The --cluster argument toggles the type of compute cluster infrastructure. The --cluster_info argument toggles the information given to the submission command, and it has to contain the following keywords {cores}, {memory}, {runtime}, which are used to forward resource information to the cluster.
+        
+        A qsub MAGinator can for example be run with the following command (... indicates required arguments, see above):
+        ```sh
+        maginator ... --cluster qsub --cluster_info "-l nodes=1:ppn={cores}:thinnode,mem={memory}gb,walltime={runtime}"
+        ```
+        
+        ## MAGinator workflow
+        
+        This is what MAGinator does with your input (if you want to see all parameters run maginator --help):
+        * Filter bins by size
+            * Use --binsize to control the cutoff
+        * Run GTDB-tk to taxonomically annotate bins and call open reading frames (ORFs)
+        * Group your VAMB clusters into metagenomic species (MGS) based on the taxonomic annotation. (Unannotated VAMB clusters are kept in the pipeline, but left unchanged)
+            * Use --no_mgs to disable this
+            * Use --annotation_prevalence to change how prevalent an annotation has to be in a VAMB cluster to call taxonomic consensus
+        * Cluster your ORFs into gene clusters to get a non-redundant gene catalogue
+            * Use --clustering_min_seq_id to toggle the clustering identity
+            * Use --clustering_coverage to toggle the clustering coverage
+            * Use --clustering_type to toggle whether to cluster on amino acid or nucleotide level
+        * Map reads to the non-redundant gene catalogue and create a matrix with gene counts for each sample
+        * Pick non-redundant genes that are only found in one MGS each
+        * Fit signature gene model and use the resulting signature genes to get the abundance of each MGS
+        * Prepare for generation of phylogenies for each MGS by finding outgroups and marker genes which will be used for rooting the phylogenies
+        * Use the read mappings to collect SNV information for each signature gene and marker gene for each sample
+        * Align signature and marker genes, concatenate alignments and infer phylogenetic trees for each MGS
+            * Use --phylo to toggle whether use fasttree (fast, approximate) or iqtree (slow, precise) to infer phylogenies
+        * Infer the taxonomic scope of each gene cluster. That is, at what taxonomic level are genes from a given gene cluster found in
+            * Use --tax_scope_threshold to toggle the threshold for how to find the taxonomic scope consensus
+        * Cluster gene clusters into synteny clusters based on how often they are found adjacent on contigs
+        
+        
+        ## Output
+        
+        * abundance/
+            * abundance_phyloseq.RData - Phyloseq object for R, with abundance and taxonomic data
+        * clusters/
+            * <cluster>/<bin>.fa - Fasta files with nucleotide sequence of bins
+        * genes/
+            * all_genes.faa - Amino acid sequences of all ORFs
+            * all_genes.fna - Nucletotide sequences of all ORFs
+            * all_genes_nonredundant.fasta - Nucleotide sequences of gene cluster representatives
+            * all_genes_cluster.tsv - Gene clusters
+            * matrix/
+                * gene_count_matrix.tsv - Read count for each gene cluster for each sample
+            * synteny/ - Intermediate files for synteny clustering of gene clusters
+        * gtdbtk/
+            * <cluster>/ - GTDB-tk taxonomic annotation for each VAMB cluster
+        * logs/ - Log files
+        * mapped_reads/
+            * bams/ - Bam files for mapping reads to gene clusters
+        * phylo/
+            * alignments/ - Alignments for each signature gene
+            * cluster_alignments/ - Concatenated alignments for each MGS
+            * pileup/ - SNV information for each MGS and each sample
+            * trees/ - Phylogenetic trees for each MGS
+            * stats.tab - Mapping information such as non-N fraction, number of signature genes and marker genes, read depth, and number of bases not reaching allele frequency cutoff 
+            * stats_genes.tab - Same as above but the information is split per gene
+        * signature_genes/ - R data files with signature gene optimization
+        * tabs/
+            * gene_cluster_bins.tab - Table listing which bins each gene cluster was found in
+            * gene_cluster_tax_scope.tab - Table listing the taxonomic scope of each gene cluster
+            * metagenomicspecies.tab - Table listing which, if any, clusters where merged in MGS and the taxonomy of those
+            * signature_genes_cluster.tsv - Table with the signature genes for each MGS/cluster
+            * synteny_clusters.tab - Table listing the synteny cluster association for the gene clusters. Gene clusters from the same synteny cluster are genomically adjacent.
+            * tax_matrix.tsv - Table with taxonomy information for MGS
+            
+        
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Development Status :: 4 - Beta
+Requires-Python: >=3.5
+Description-Content-Type: text/markdown
```

### Comparing `maginator-0.1.20/maginator/controller.py` & `maginator-0.1.8/maginator/controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,33 +19,32 @@
 
         # Force consistency
         self.output = os.path.join(self.output, '')
 
         # Check cluster info input
         if self.cluster is not None:
             if self.cluster_info is not None:
-                if len(re.findall('{cores}|{mem_gb}|{runtime}', self.cluster_info)) != 3 or len(re.findall('{.*?}', self.cluster_info)) != 3: 
-                    logging.error('cluster_info has to contain the following special strings: {cores}, {mem_gb}, and {runtime}')
+                if len(re.findall('{cores}|{memory}|{runtime}', self.cluster_info)) != 3 or len(re.findall('{.*?}', self.cluster_info)) != 3: 
+                    logging.error('cluster_info has to contain the following special strings: {cores}, {memory}, and {runtime}')
                     sys.exit()
                 else:
-                    tmp_info = re.sub('{cores}|{mem_gb}|{runtime}','',self.cluster_info)
+                    tmp_info = re.sub('{cores}|{memory}|{runtime}','',self.cluster_info)
                     if not bool(re.match('^[a-zA-Z0-9-_ =:,.]+$', tmp_info)):
                         logging.error('Invalid characters in cluster_info')
                         sys.exit()
             else:
                 logging.error('cluster_info is required when running on a compute cluster')
                 sys.exit()
 
         # Check input and output
         self.check_params()
         self.check_out()
-        if not any([self.unlock, self.only_conda, self.snake is not None]):
-            self.check_vamb()
-            self.check_reads()
-            self.check_contigs()
+        self.check_vamb()
+        self.check_reads()
+        self.check_contigs()
         self.write_params(args)
 
     def check_params(self):
         '''
         Return error if parameters are not allowed
         '''
```

### Comparing `maginator-0.1.20/maginator/main.py` & `maginator-0.1.8/maginator/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,48 +41,42 @@
     apr.add_argument('-c', '--contigs', help='Fasta file with contig sequences. Fasta headers should match the 2nd column in the clusters.tsv file', required=True)
     apr.add_argument('-o', '--output', help='Prefix for output directory', required=True)
     apr.add_argument('-g', '--gtdb_db', help='Path to GTDB-tk database', type=str, required=True)
 
     # Cluster arguments
     apc = ap.add_argument_group('compute cluster arguments')
     apc.add_argument('--cluster', help='Cluster compute structure [%(default)s]', default=None, type=str, choices=[None,'qsub','slurm','drmaa'])
-    apc.add_argument('--cluster_info', help='Cluster scheduler arguments when submitting cluster jobs.\nHas to contain the following special strings:\n{mem_gb}, {cores}, and {runtime}.\nThese special strings will be substituted by maginator to indicate resources for each job.\n{mem_gb} is substituted for the mem_gb in GB.\n{runtime} is substituted with the time in the following format: DD:HH:MM:SS.\nCan also contain user names, groups, etc. required by the cluster scheduler', default=None, type=str)
+    apc.add_argument('--cluster_info', help='Cluster scheduler arguments when submitting cluster jobs.\nHas to contain the following special strings:\n{memory}, {cores}, and {runtime}.\nThese special strings will be substituted by maginator to indicate resources for each job.\n{memory} is substituted for the memory in GB.\n{runtime} is substituted with the time in the following format: DD:HH:MM:SS.\nCan also contain user names, groups, etc. required by the cluster scheduler', default=None, type=str)
     apc.add_argument('--max_jobs', help='Maximum number of cluster jobs [%(default)s]', default=500, type=int)
     
     # Optional
     apo = ap.add_argument_group('optional arguments')
-    apo.add_argument('-V','--version', action='version', version='MAGinator version {}'.format(pkg_resources.require("maginator")[0].version))
     apo.add_argument("-h", "--help", action="help", help="show this help message and exit")
     apo.add_argument('--max_cores', help='Maximum number of cores [%(default)s]', default=40, type=int)
-    apo.add_argument('--max_mem', help='Maximum mem_gb in GB [%(default)s]', default=180, type=int)
+    apo.add_argument('--max_mem', help='Maximum memory in GB [%(default)s]', default=180, type=int)
     apo.add_argument('--log_lvl', help='Logging level [%(default)s].', default='INFO', type=str, choices=['DEBUG','INFO','WARNING','ERROR'])
     apo.add_argument('--only_conda', help='Only install conda environments, then exit', action='store_true')
     apo.add_argument('--snake', help='Only run specific snakemake command. For debug purposes', type=str)
     apo.add_argument('--unlock', help='Unlock snakemake directory in case of unexpected exists, then exit', action='store_true')
 
     # Parameters
     app = ap.add_argument_group('parameters')
     app.add_argument('--binsize', help='Minimum bin size for inclusion [%(default)s].', default=200000, type=int)
-    app.add_argument('--mgs_collections', help='If set, bin clusters will be aggregated to metagenomic species.', action='store_true')
+    app.add_argument('--no_mgs', help='If set, bin clusters will not be aggregated to metagenomic species, but treated separately.', action='store_true')
     app.add_argument('--annotation_prevalence', help='Minimum prevalence of taxonomic assignment in a cluster of bins to call consensus [%(default)s]', default=0.75, type=float)
-    app.add_argument('--clustering_coverage', help='Alignment coverage for clustering of genes with MMseqs2 [%(default)s]', default=0.8, type=float)
+    app.add_argument('--clustering_coverage', help='Alignment coverage for clustering of genes with MMseqs2 [%(default)s]', default=0.95, type=float)
     app.add_argument('--clustering_min_seq_id', help='Sequence identity threshold for clustering of genes with MMseqs2 [%(default)s]', default=0.95, type=float)
     app.add_argument('--clustering_type', help='Sequence type for gene clustering with MMseqs2. Nucleotide- or protein-level [%(default)s]', default='protein', type=str, choices=['nucleotide', 'protein'])
     app.add_argument('--min_gtdb_markers', help='Minimum GTDBtk marker genes shared between MGS and outgroup for rooting trees [%(default)s]', default=10, type=int)
     app.add_argument('--marker_gene_cluster_prevalence', help='Minimum prevalence of marker genes to be selected for rooting of MGS trees [%(default)s]', default=0.5, type=float)
-
-    app.add_argument('--min_mapped_signature_genes', help='Minimum number of signature genes with reads mapped for the sample to be included in the refinement [%(default)s]', default=3, type=int)
-    app.add_argument('--min_samples', help='Minimum number of samples containing the MAG cluster (more than "min_mapped_signature_genes" present) for the MAG cluster to identidy SG [%(default)s]', default=3, type=int)
-
     app.add_argument('--min_af', help='Minimim allele frequency for calling a base when creating phylogenies [%(default)s]', default=0.8, type=float)
     app.add_argument('--min_depth', help='Minimim read depth for calling a base when creating phylogenies [%(default)s]', default=2, type=int)
     app.add_argument('--min_nonN', help='Minimum fraction of non-N characters of a sample to be included in a phylogeny [%(default)s]', default=0.5, type=float)
     app.add_argument('--min_marker_genes', help='Minimum marker genes to be detected for inclusion of a sample in a phylogeny [%(default)s]', default=2, type=int)
     app.add_argument('--min_signature_genes', help='Minimum signature genes to be detected for inclusion of a sample in a phylogeny [%(default)s]', default=50, type=int)
-    app.add_argument('--af_cutoff', help='Cutoff for average median allele frequency of SG alignment for determining mixed/pure population of a MAG in a sample [%(default)s]', default=0, type=float)
     app.add_argument('--phylo', help='Software for phylogeny inference. Either fast (fasttree) or slow and more accurate (iqtree) [%(default)s]', default='fasttree', type=str, choices=['fasttree', 'iqtree'])
     app.add_argument('--tax_scope_threshold', help='Threshold for assigning the taxonomic scope of a gene cluster [%(default)s]', default=0.9, type=float)
     app.add_argument('--synteny_adj_cutoff', help='Minimum number of times gene clusters should be adjacent to be included in synteny graph [%(default)s]', default=1, type=int)
     app.add_argument('--synteny_mcl_inflation', help='Inflation parameter for mcl clustering of synteny graph. Usually between 1.2 and 5. Higher values produce smaller clusters [%(default)s]', default=5, type=float)
 
     ########## Workflow ##########
     master = Controller(ap)
```

### Comparing `maginator-0.1.20/maginator/messages.py` & `maginator-0.1.8/maginator/messages.py`

 * *Files identical despite different names*

### Comparing `maginator-0.1.20/maginator/workflow/alignment.Snakefile` & `maginator-0.1.8/maginator/workflow/alignment.Snakefile`

 * *Files 9% similar despite different names*

```diff
@@ -19,16 +19,16 @@
         os.path.join(WD, 'phylo', 'fastas', '{cluster}')
     output:
         directory(os.path.join(WD, 'phylo', 'alignments', '{cluster}'))
     conda:
         "envs/phylo.yaml"
     resources:
         cores=1,
-        mem_gb=4,
-        runtime='36000' #10h in s
+        memory=4,
+        runtime='10:00:00'
     shell:
         """
         mkdir -p {output}
         for gene in {input}/*.fna; do mafft --ep 0.123 $gene > {output}/$(basename $gene); done
         """
 
 rule concat:
@@ -37,15 +37,15 @@
         expand(os.path.join(WD, 'phylo', 'alignments', '{cluster}'), cluster=CLUSTERS)
     output:
         directory(os.path.join(WD, 'phylo', 'cluster_alignments'))
     conda:
         "envs/phylo.yaml"
     resources:
         cores=10,
-        mem_gb=40,
-        runtime='36000' #10h in s
+        memory=40,
+        runtime='10:00:00'
     params:
         ali_dir=os.path.join(WD, 'phylo', 'alignments')
     script:
         "scripts/concat.py"
```

### Comparing `maginator-0.1.20/maginator/workflow/filter.Snakefile` & `maginator-0.1.8/maginator/workflow/filter.Snakefile`

 * *Files 24% similar despite different names*

```diff
@@ -13,20 +13,20 @@
     fl = [x.strip().split() for x in fh.readlines()]
 param_dict = {x[0]: x[1] for x in fl}
 
 # Adaptive resource usage
 ## Get lines in vamb file
 out = subprocess.Popen(['wc', '-l', VAMB], stdout=subprocess.PIPE, stderr=subprocess.STDOUT).communicate()[0]
 n_contigs = int(out.partition(b' ')[0])
-## mem_gb is 30gb per million contigs
+## memory is 30gb per million contigs
 mem = math.ceil(n_contigs/1000000)*30
 if mem > int(param_dict['max_mem']):
     mem = int(param_dict['max_mem'])
 ## time is 1 hour per million
-tim = str(max(1800, min(math.ceil(n_contigs/100000)*60*60, 72000))) # runtime in seconds, max 20h, min 30min
+tim = str(math.ceil(n_contigs/1000000))+':00:00'
 
 rule all:
     input:
         F_DIR
 
 rule bin_filter:
     input:
@@ -36,12 +36,12 @@
         directory(F_DIR),
     params:
         binsize=param_dict['binsize']
     conda:
         "envs/filter_gtdbtk.yaml"
     resources:
         cores=1,
-        mem_gb=mem,
+        memory=mem,
         runtime=tim
     script:
         "scripts/filter.py"
```

### Comparing `maginator-0.1.20/maginator/workflow/filter_geneclusters.Snakefile` & `maginator-0.1.8/maginator/workflow/filter_geneclusters.Snakefile`

 * *Files 4% similar despite different names*

```diff
@@ -32,31 +32,31 @@
         clusters = os.path.join(WD, 'genes', 'all_genes_cluster.tsv')
     output:
         os.path.join(WD, 'genes', 'all_genes_nonredundant.fasta')
     conda:
         "envs/filter_gtdbtk.yaml"
     resources:
         cores = 1,
-        mem_gb = 50,
-        runtime = '43200' #12h in s
+        memory = 50,
+        runtime = '12:00:00'
     shell:
         "perl -ne 'if(/^>(\S+)/){{$c=$i{{$1}}}}$c?print:chomp;$i{{$_}}=1 if @ARGV' <(cut -f1 {input.clusters} | uniq) {input.genecat} | awk '{{print $1}}' > {output}"
 
 # Indexing the genes for mapping
 rule bwa_index:
     input: 
         fasta=os.path.join(WD, 'genes', 'all_genes_nonredundant.fasta')
     output: 
         index=os.path.join(WD, 'genes', 'all_genes_nonredundant')
     conda:
         "envs/filter_gtdbtk.yaml" 
     resources:
         cores = 40,
-        mem_gb = 188, 
-        runtime = '86400' #1d in s
+        memory = 188, 
+        runtime = '1:00:00:00'
     shell:
         "bwa-mem2 index -p {output.index} {input.fasta}; samtools faidx {input.fasta}; touch {output.index}"
 
 # Readmapping
 rule bwa_readmap:
     input:
         index = os.path.join(WD, 'genes', 'all_genes_nonredundant'),
@@ -67,11 +67,11 @@
         sample = SAMPLES
     output:
         bam = os.path.join(WD, 'mapped_reads', 'bams', 'gene_counts_{sample}.bam')
     conda:
         "envs/filter_gtdbtk.yaml"
     resources:
         cores = 40,
-        mem_gb = 188,
-        runtime = '86400' #1d in s
+        memory = 188,
+        runtime = '1:00:00:00'
     shell:
         "bwa-mem2 mem -t {resources.cores} {input.index} {input.fastq1} {input.fastq2} | samtools view -T {input.fasta} -F 3584  -b --threads {resources.cores} | samtools sort --threads {resources.cores} > {output.bam}; samtools index {output.bam}"
```

### Comparing `maginator-0.1.20/maginator/workflow/gene_count_mat.Snakefile` & `maginator-0.1.8/maginator/workflow/gene_count_mat.Snakefile`

 * *Files 10% similar despite different names*

```diff
@@ -22,47 +22,47 @@
         os.path.join(WD, 'mapped_reads', 'bams', 'gene_counts_{sample}.bam')
     output:
         readcounts = os.path.join(WD, 'mapped_reads', 'counts', '{sample}.counts')
     conda:
         "envs/filter_geneclusters.yaml"
     resources:
         cores = 1,
-        mem_gb = 20,
-        runtime = '7200' #2h in s
+        memory = 20,
+        runtime = '2:00:00'
     shell:
         "samtools idxstats {input} | cut -f3 > {output.readcounts}"
 
 # Create the gene index
 rule gene_names:
     input:
         os.path.join(WD, 'mapped_reads', 'bams', 'gene_counts_{sample}.bam')
     output:
         os.path.join(WD, 'mapped_reads', 'gene_names_{sample}')
     wildcard_constraints:
         sample=SAMPLES[0]
     conda:
-        "envs/filter_geneclusters.yaml"
+       	"envs/filter_geneclusters.yaml"
     resources:
         cores = 1,
-        mem_gb = 20,
-        runtime = '3600' #1h in s
+        memory = 20,
+        runtime = '1:00:00'
     shell:
         "samtools idxstats {input} | cut -f1 > {output}"
 
 
 # Create the header for the gene count matrix
 rule create_header:
     input: 
         expand(os.path.join(WD, 'mapped_reads', 'counts', '{sample}.counts'), sample=SAMPLES)
     output:
         header = os.path.join(WD, 'mapped_reads', 'header.txt')
     resources:
         cores = 1,
-        mem_gb = 188,
-        runtime = '3600' #1h in s
+        memory = 188,
+        runtime = '1:00:00'
     run:
         header = "Gene"
         for f in input:
             sample_name = f.split("/")[-1].split(".")[0]
             header = header + "\t" + sample_name
         header = header + "\n"
         with open(output.header, "w") as out:
@@ -74,14 +74,14 @@
     input:
         readcounts = expand(os.path.join(WD, 'mapped_reads', 'counts', '{sample}.counts'), sample=SAMPLES),
         gene_names = expand(os.path.join(WD, 'mapped_reads', 'gene_names_{sample}'), sample=SAMPLES[0]),
         header = os.path.join(WD, 'mapped_reads', 'header.txt')
     output:
         os.path.join(WD, 'genes', 'matrix', 'gene_count_matrix.tsv')
     conda:
-        "envs/filter_geneclusters.yaml"
+       	"envs/filter_geneclusters.yaml"
     resources:
         cores = 1,
-        mem_gb = 188,
-        runtime = '3600' #1h in s
+        memory = 188,
+        runtime = '1:00:00'
     shell:
         "paste {input.gene_names} {input.readcounts} | cat {input.header} - > {output}; sed -i '$d' {output}"
```

### Comparing `maginator-0.1.20/maginator/workflow/gene_tax.Snakefile` & `maginator-0.1.8/maginator/workflow/gene_tax.Snakefile`

 * *Files 13% similar despite different names*

```diff
@@ -26,32 +26,32 @@
         os.path.join(WD, 'tabs', 'gene_cluster_bins.tab')
     params:
         cutoff = param_dict['tax_scope_threshold']
     conda:
         "envs/phylo.yaml"
     resources:
         cores = 1,
-        mem_gb = 80,
-        runtime = '7200' #2h in s
+        memory = 10,
+        runtime = '02:00:00'
     script:
         "scripts/gene_cluster2tax.py"
 
 rule synteny_graph:
     input:
         cluster=os.path.join(WD, 'genes', 'all_genes_cluster.tsv'),
         faa=os.path.join(WD, 'genes', 'all_genes.faa')
     output:
         graph=os.path.join(WD, 'genes', 'synteny', 'graph.tab'),
         index=os.path.join(WD, 'genes', 'synteny', 'graph_index.tab')
     conda:
         "envs/phylo.yaml"
     resources:
         cores = 1,
-        mem_gb = 40,
-        runtime = '36000' #10h in s
+        memory = 40,
+        runtime = '10:00:00'
     script:
         "scripts/synteny.py"
 
 rule synteny_mcl:
     input:
         graph=os.path.join(WD, 'genes', 'synteny', 'graph.tab'),
         index=os.path.join(WD, 'genes', 'synteny', 'graph_index.tab')
@@ -62,16 +62,16 @@
     conda:
         "envs/phylo.yaml"
     params:
         cutoff=param_dict['synteny_adj_cutoff'],
         i=param_dict['synteny_mcl_inflation']
     resources:
         cores = 40,
-        mem_gb = 180,
-        runtime = '86400' #1d in s
+        memory = 180,
+        runtime = '24:00:00'
     shell:
         """
         join -1 2 -2 1 <(join -j1 <(sed 's/.*(//;s/)//;s/,//;s/\.0$//' {input.graph} | sort -k1,1) <(sort -k1,1 {input.index}) | sort -k2,2) <(sort -k1,1 {input.index}) \
                         | awk '{{print $4,$5,$3}}' > {output.abc}
         mcl <(awk '$3 > {params.cutoff}' {output.abc}) --abc -I {params.i} -te {resources.cores} -o {output.mcl}
         awk '{{gsub("$",";"NR)}}1' {output.mcl} | awk '{{gsub(/\\t/,";"NR"\\n")}}1' | sed 's/;/\t/' > {output.tab}
         """
```

### Comparing `maginator-0.1.20/maginator/workflow/outgroup.Snakefile` & `maginator-0.1.8/maginator/workflow/outgroup.Snakefile`

 * *Files 13% similar despite different names*

```diff
@@ -27,77 +27,77 @@
     params:
         min_gtdb_markes=param_dict['min_gtdb_markers'],
         marker_gene_cluster_prevalence=param_dict['marker_gene_cluster_prevalence']
     conda:
         "envs/phylo.yaml"
     resources:
         cores=1,
-        mem_gb=10,
-        runtime='36000' #10h in s
+        memory=10,
+        runtime='10:00:00'
     script:
         "scripts/marker_genes.py"
 
 rule fasta1:
     input:
         tab=os.path.join(WD, 'phylo', 'intermediate',  'clusterID_markerGene_geneCluster_rootGene.tsv'),
         fasta=os.path.join(WD, 'genes', 'all_genes_nonredundant.fasta')
     output:
         os.path.join(WD, 'phylo', 'intermediate', 'markers_clusters.fna')
     conda:
         "envs/phylo.yaml"
     resources:
         cores=1,
-        mem_gb=10,
-        runtime='36000' #10h in s
+        memory=10,
+        runtime='10:00:00'
     shell:
         "perl -ne 'if(/^>(\S+)/){{$c=$i{{$1}}}}$c?print:chomp;$i{{$_}}=1 if @ARGV' <(cut -f4 {input.tab} | sort | uniq) {input.fasta} > {output}"
 
 rule fasta2:
     input:
         tab=os.path.join(WD, 'phylo', 'intermediate',  'clusterID_markerGene_geneCluster_rootGene.tsv'),
         fasta=os.path.join(WD, 'genes', 'all_genes.fna')
     output:
         os.path.join(WD, 'phylo', 'intermediate', 'markers_roots.fna')
     conda:
         "envs/phylo.yaml"
     resources:
         cores=1,
-        mem_gb=10,
-        runtime='36000' #10h in s
+        memory=10,
+        runtime='10:00:00'
     shell:
         "perl -ne 'if(/^>(\S+)/){{$c=$i{{$1}}}}$c?print:chomp;$i{{$_}}=1 if @ARGV' <(cut -f5 {input.tab} | sort | uniq) {input.fasta} > {output}"
 
 rule fasta3:
     input:
         tab=os.path.join(WD, 'tabs',  'signature_genes_cluster.tsv'),
         fasta=os.path.join(WD, 'genes', 'all_genes_nonredundant.fasta')
     output:
         os.path.join(WD, 'genes', 'signature_genes.fasta')
     conda:
         "envs/phylo.yaml"
     resources:
         cores=1,
-        mem_gb=10,
-        runtime='36000' #10h in s
+        memory=10,
+        runtime='10:00:00'
     shell:
         "perl -ne 'if(/^>(\S+)/){{$c=$i{{$1}}}}$c?print:chomp;$i{{$_}}=1 if @ARGV' <(cut -f1 {input.tab}) {input.fasta} > {output}"
 
 rule bed:
     input:
         sig=os.path.join(WD, 'tabs',  'signature_genes_cluster.tsv'),
         tab=os.path.join(WD, 'phylo', 'intermediate',  'clusterID_markerGene_geneCluster_rootGene.tsv')
     output:
         beds=os.path.join(WD, 'phylo', 'intermediate',  'signature_genes.bed'),
         bedm=os.path.join(WD, 'phylo', 'intermediate',  'marker_genes.bed')
     conda:
         "envs/phylo.yaml"
     resources:
         cores=1,
-        mem_gb=10,
-        runtime='36000' #10h in s
+        memory=10,
+        runtime='10:00:00'
     shell:
         """
         awk '{{print $1"\t0\t1000000"}}' {input.sig} > {output.beds}
         cut -f4 {input.tab} | sort | uniq | awk '{{print $1"\t0\t1000000"}}' > {output.bedm}
         """
 
 rule uniq:
@@ -109,16 +109,16 @@
     output:
         bed=os.path.join(WD, 'phylo', 'intermediate',  'cluster_genes.bed'),
         fasta=os.path.join(WD, 'phylo', 'intermediate',  'cluster_genes.fna')
     conda:
         "envs/phylo.yaml"
     resources:
         cores=1,
-        mem_gb=10,
-        runtime='36000' #10h in s
+        memory=10,
+        runtime='10:00:00'
     shell:
         """
         cat {input.beds} {input.bedm} | sort | uniq > {output.bed}
         cat {input.fastas} {input.fastac} | awk '/^>/{{f=!d[$1];d[$1]=1}}f' > {output.fasta}
         """
 
 rule index:
@@ -126,13 +126,14 @@
         os.path.join(WD, 'phylo', 'intermediate',  'cluster_genes.fna')
     output:
         os.path.join(WD, 'phylo', 'intermediate',  'cluster_genes.fna.fai')
     conda:
         "envs/phylo.yaml"
     resources:
         cores=1,
-        mem_gb=10,
-        runtime='36000' #10h in s
+        memory=10,
+        runtime='10:00:00'
     shell:
         """
         samtools faidx {input}
         """
+
```

### Comparing `maginator-0.1.20/maginator/workflow/parse_gtdbtk.Snakefile` & `maginator-0.1.8/maginator/workflow/parse_gtdbtk.Snakefile`

 * *Files 12% similar despite different names*

```diff
@@ -25,21 +25,21 @@
         os.path.join(WD, 'phylo', 'intermediate', 'gtdb_markers.tab'),
         os.path.join(WD, 'phylo', 'intermediate', 'gtdb_unique_bac_markers.tab'),
         os.path.join(WD, 'phylo', 'intermediate', 'gtdb_unique_ar_markers.tab'),
         os.path.join(WD, 'genes', 'all_genes.faa')
     params:
         param_dict['annotation_prevalence'],
         VAMB,
-        distutils.util.strtobool(param_dict['mgs_collections'])
+        distutils.util.strtobool(param_dict['no_mgs'])
     conda:
         "envs/filter_gtdbtk.yaml"
     resources:
         cores=1,
-        mem_gb=32,
-        runtime='36000' #10h in s
+        memory=32,
+        runtime='10:00:00'
     script:
         "scripts/parse_gtdbtk.py"
 
 # identifying the sequence type which will be the basis for the gene clustering
 if param_dict["clustering_type"] == "protein":
     sequence_type_cluster = os.path.join(WD, 'genes', 'all_genes.faa')
 elif param_dict["clustering_type"] == "nucleotide":
@@ -50,16 +50,16 @@
 rule repres_genes:
     input:
         sequence_type_cluster
     output:
         tsv = os.path.join(WD, 'genes', 'all_genes_cluster.tsv')
     resources:
         cores = 14,
-        mem_gb = 50,
-        runtime = '172800' #2d in s 
+        memory = 50,
+        runtime = '2:00:00:00' 
     params:
         tmp_dir = os.path.join(WD, 'tmp'),
         out_prefix = os.path.join(WD, 'genes', 'all_genes'),
         cov = param_dict["clustering_coverage"],
         seq_id = param_dict["clustering_min_seq_id"]
     conda:
         "envs/filter_gtdbtk.yaml"
@@ -72,24 +72,24 @@
     input:
         gtdb = os.path.join(WD, 'phylo', 'intermediate', 'gtdb_markers.tab'),
         cluster = os.path.join(WD, 'genes', 'all_genes_cluster.tsv')
     output:
         os.path.join(WD, 'phylo', 'intermediate', 'gtdb_markers_bins_geneID.tsv')
     resources:
         cores = 1,
-        mem_gb = 20,
-        runtime = '86400' #1d in s
+        memory = 20,
+        runtime = '24:00:00'
     shell:
         "join -1 1 -2 2 <(sort -k1,1 {input.gtdb}) <(sort -k2,2 {input.cluster}) > {output}"
 
 # Collect GTDB-tk summary info
 rule collect:
     input:
         os.path.join(WD, 'gtdbtk')
     output:
         os.path.join(WD, 'phylo', 'intermediate', 'gtdbtk_summary.tsv')
     resources:
         cores = 1,
-        mem_gb = 20,
-        runtime = '86400' #1d in s
+        memory = 20,
+        runtime = '24:00:00'
     shell:
         "for i in {input}/*/*summary.tsv; do tail -n+2 $i; done | cut -f1,2 > {output}"
```

### Comparing `maginator-0.1.20/maginator/workflow/phylo.Snakefile` & `maginator-0.1.8/maginator/workflow/phylo.Snakefile`

 * *Files 10% similar despite different names*

```diff
@@ -20,16 +20,16 @@
             os.path.join(WD, 'phylo', 'cluster_alignments', '{cluster}.fna')
         output:
             os.path.join(WD, 'phylo', 'trees', '{cluster}.nwk')
         conda:
             "envs/phylo.yaml"
         resources:
             cores=1,
-            mem_gb=32,
-            runtime='43200' #12h in s
+            memory=32,
+            runtime='12:00:00'
         shell:
             """
             fasttree -nt {input} > {output}
             """
 
 # IQtree
 if param_dict['phylo'] == 'iqtree':
@@ -41,13 +41,13 @@
             os.path.join(WD, 'phylo', 'trees', '{cluster}.nwk')
         conda:
             "envs/phylo.yaml"
         params:
             prefix=os.path.join(WD, 'phylo', 'trees', '{cluster}'),
         resources:
             cores=40,
-            mem_gb=180,
-            runtime='172800' #2d in s
+            memory=180,
+            runtime='02:00:00:00'
         shell:
             """
             iqtree -T {resources.cores} -s {input.fna} -p {input.part} -o Outgroup --prefix {params.prefix} || true && if [ -f {params.prefix}.treefile ]; then mv {params.prefix}.treefile {output}; else touch {output}; fi
             """
```

### Comparing `maginator-0.1.20/maginator/workflow/pileup.Snakefile` & `maginator-0.1.8/maginator/workflow/pileup.Snakefile`

 * *Files 8% similar despite different names*

```diff
@@ -20,27 +20,27 @@
         bam=os.path.join(WD, 'mapped_reads', 'bams', 'gene_counts_{sample}.bam')
     output:
         os.path.join(WD, 'mapped_reads', 'bams', 'subset', '{sample}.bam')
     conda:
         "envs/phylo.yaml"
     resources:
         cores = 1,
-        mem_gb = 20,
-        runtime = '43200' #12h in s
+        memory = 20,
+        runtime = '12:00:00'
     shell:
         "samtools view -b -L {input.bed} {input.bam} | samtools sort -o {output}"
 
 rule pileup:
     input:
         fna=os.path.join(WD, 'phylo', 'intermediate', 'cluster_genes.fna'),
         bam=os.path.join(WD, 'mapped_reads', 'bams', 'subset', '{sample}.bam')
     output:
         os.path.join(WD, 'phylo', 'pileup', '{sample}.mp')
     conda:
-        "envs/phylo.yaml"
+       	"envs/phylo.yaml"
     resources:
         cores = 1,
-        mem_gb = 20,
-        runtime = '86400' #1d in s
+        memory = 20,
+        runtime = '24:00:00'
     shell:
         "samtools mpileup -A -x -f {input.fna} {input.bam} -o {output}"
```

### Comparing `maginator-0.1.20/maginator/workflow/pileup_parse.Snakefile` & `maginator-0.1.8/maginator/workflow/pileup_parse.Snakefile`

 * *Files 10% similar despite different names*

```diff
@@ -33,31 +33,12 @@
         min_nonN = param_dict['min_nonN'], 
         min_marker_genes = param_dict['min_marker_genes'], 
         min_signature_genes = param_dict['min_signature_genes']
     conda:
         "envs/phylo.yaml"
     resources:
         cores = 40,
-        mem_gb = 180,
-        runtime = '172800' #2d in s
+        memory = 180,
+        runtime = '02:00:00:00'
     script:
         "scripts/mpileup.py"
 
-rule allele_frequencies:
-    input:
-        stat=os.path.join(WD, 'phylo', 'stats.tab'),
-        gene=os.path.join(WD, 'phylo', 'stats_genes.tab')
-    output:
-        af_matrix=os.path.join(WD,'tabs','allele_frequencies.tab')
-    params:
-        af_cutoff = param_dict['af_cutoff'],
-        min_signature_genes = param_dict['min_signature_genes'],
-        min_nonN = param_dict['min_nonN'],
-        min_marker_genes = param_dict['min_marker_genes']
-    conda:
-        "envs/signature_genes.yaml"
-    resources:
-        cores=2,
-        mem_gb=190,
-        runtime='172800'
-    script:
-        "scripts/allele_frequency_mat.R"
```

### Comparing `maginator-0.1.20/maginator/workflow/prescreening_genes.Snakefile` & `maginator-0.1.8/maginator/workflow/signature_genes.Snakefile`

 * *Files 16% similar despite different names*

```diff
@@ -1,95 +1,78 @@
-
 import os
 
 WD = config['wd']
 PARAMS = config['params']
-cluster_DIR = os.path.join(WD, 'signature_genes', 'clusters')
 
 with open(PARAMS, 'r') as fh:
     fl = [x.strip().split() for x in fh.readlines()]
 param_dict = {x[0]: x[1] for x in fl}
 
-
 with open(param_dict['reads']) as f:
     SAMPLES = ([row.split(',')[0] for row in f])
 
-SAMPLES=set(SAMPLES)
-
+CLUSTERS = set(glob_wildcards(os.path.join(WD, 'signature_genes', 'clusters', 'Cluster{cluster}.RDS')).cluster)
+CLUSTERS = {x for x in CLUSTERS if x.isdigit()}
 
 rule all:
     input:
-        os.path.join(WD, 'genes', 'representative_genes.tsv'),
-        os.path.join(WD, 'signature_genes', 'clusters_sorted.RDS')
+        os.path.join(WD, 'abundance', 'abundance_phyloseq.RData')
+
 
-# Identifying the genes that cluster across the metagenomic species / species collections
-rule geneID_collectionID:
-    input: 
-        os.path.join(WD, 'tabs', 'metagenomicspecies.tab'),
-        os.path.join(WD, 'genes', 'all_genes_cluster.tsv'),
-        param_dict['vamb_clusters']
+# Identifying the refined sets of signature genes using the gene count matrix and gene lengths
+rule refinement:
+    input:
+        clusters_dir = os.path.join(WD, 'signature_genes', 'clusters', 'Cluster{cluster}.RDS'),
+        clusters_sorted = os.path.join(WD, 'signature_genes', 'clusters_sorted.RDS'),
+        gene_lengths = os.path.join(WD, 'signature_genes', 'gene_lengths.RDS')
     output:
-        os.path.join(WD, 'genes', 'representative_genes.tsv'),
-        os.path.join(WD, 'genes', 'gene_lists', 'geneID_collectionID.tsv')
+        cluster_screened = os.path.join(WD, 'signature_genes', 'screened', 'cluster_{cluster}_screened.RDS'),
     conda:
         "envs/signature_genes.yaml"
+    params:
+        functions = "Functions_v4.R"
     resources:
         cores = 1,
-        mem_gb = 188,
-        runtime = '43200' #12h in s
+        memory = 188,
+        runtime = '12:00:00'
     script: 
-        "scripts/species_collections.py"
-
-# creating a gene count matrix only containing the genes, that does not cluster across metagenomic species / species collection
-rule sort_genes_across_MGS:
-    input: 
-        os.path.join(WD, 'genes', 'matrix', 'gene_count_matrix.tsv'),
-        os.path.join(WD, 'genes', 'representative_genes.tsv')
-    output:
-        os.path.join(WD, 'genes', 'matrix', 'small_gene_count_matrix.tsv')
-    conda:
-        "envs/signature_genes.yaml" 
-    resources:
-        cores = 1, 
-        mem_gb = 188,
-        runtime = '43200' #12h in s
-    script:
-        "scripts/sort_gene_mat.py"
+        "scripts/SG_refinement.R"
 
 
-#Converting the gene count matrix to cluster-matrices in R dataformat 
-rule format_conversion:
+# insert rule for creating the MGS_object.RDS
+rule gene_counts:
     input:
-        gene_clusters = os.path.join(WD, 'genes', 'gene_lists', 'geneID_collectionID.tsv'),
-        matrix = os.path.join(WD, 'genes', 'matrix', 'small_gene_count_matrix.tsv'),
-        gene_lengths = os.path.join(WD, 'genes', 'all_genes_nonredundant.fasta.fai')
+        cluster_screened = os.path.join(WD, 'signature_genes', 'screened', 'cluster_{cluster}_screened.RDS'),
+        gene_lengths = os.path.join(WD, 'signature_genes', 'gene_lengths.RDS'),
+        clusters_sorted = os.path.join(WD, 'signature_genes', 'clusters_sorted.RDS')
     output:
-        R_clusters = os.path.join(WD, 'signature_genes', 'cluster.RDS'),
-        R_gene_lengths = os.path.join(WD, 'signature_genes', 'gene_lengths.RDS'),
-        clusters_dir = (directory(cluster_DIR))
+        cluster_counts = os.path.join(WD, 'signature_genes','counts', 'cluster_{cluster}_counts.RDS')
     conda:
-        "envs/signature_genes.yaml" 
+        "envs/signature_genes.yaml"
     resources:
         cores = 1,
-        mem_gb = 188,
-        runtime = '86400' #1d in s
+        memory = 188,
+        runtime = '12:00:00'
     script:
-        "scripts/matrix2SG_formatconversion.R"
+        "scripts/MGS_counts.R"
 
 
-# sorting the genes according to the CCP
-rule prescreening_genes:
+
+# Creating abundance profiles from the SG
+rule abundance_profile:
     input:
-        clusters = os.path.join(WD, 'signature_genes', 'cluster.RDS'),
-        gene_lengths = os.path.join(WD, 'signature_genes', 'gene_lengths.RDS')
+        R_gene_lengths = os.path.join(WD, 'signature_genes', 'gene_lengths.RDS'),
+        screened_clusters = expand(os.path.join(WD, 'signature_genes', 'screened', 'cluster_{cluster}_screened.RDS'), cluster=CLUSTERS),
+        R_clusters = os.path.join(WD, 'signature_genes', 'cluster.RDS'),
+        annotation = os.path.join(WD, 'tabs', 'metagenomicspecies.tab')
     output:
-        clusters_sorted = os.path.join(WD, 'signature_genes', 'clusters_sorted.RDS'),
-    params:
-        min_mapped_signature_genes = param_dict['min_mapped_signature_genes']
+        physeq_abundance = os.path.join(WD, 'abundance', 'abundance_phyloseq.RData'),
+        tax_matrix = os.path.join(WD, 'tabs', 'tax_matrix.tsv'),
+        sg_cluster = os.path.join(WD, 'tabs', 'signature_genes_cluster.tsv')
     conda:
         "envs/signature_genes.yaml"
     resources:
-        cores = 1,
-        mem_gb = 188,
-        runtime = '86400' #1d in s
-    script: 
-        "scripts/prescreening_genes.R"
+        cores = 6,
+        memory = 188,
+        runtime = '12:00:00'
+    script:
+        "scripts/abundance_profiles.R"
```

### Comparing `maginator-0.1.20/maginator/workflow/scripts/Functions_v4.R` & `maginator-0.1.8/maginator/workflow/scripts/Functions_v4.R`

 * *Files identical despite different names*

### Comparing `maginator-0.1.20/maginator/workflow/scripts/MGS_counts.R` & `maginator-0.1.8/maginator/workflow/scripts/MGS_counts.R`

 * *Files identical despite different names*

### Comparing `maginator-0.1.20/maginator/workflow/scripts/SG_refinement.R` & `maginator-0.1.8/maginator/workflow/scripts/SG_refinement.R`

 * *Files 4% similar despite different names*

```diff
@@ -16,16 +16,15 @@
 
 snakemake@source(snakemake@params[["functions"]])
 
 #Number of signature genes
 n.genes <- 100
 
 #minimum number of mapped genes required
-n.mapped.minimum <- as.integer(snakemake@params[["min_mapped_signature_genes"]])
-n.minimum.samples <- as.integer(snakemake@params[["min_samples"]])
+n.mapped.minimum <- 3
 
 ids <- names(Clusterlist) #the ids of the MGS
 id <- tail(strsplit(strsplit(snakemake@input[["clusters_dir"]], ".RDS")[[1]], "/")[[1]], n=1)
 
 # initializing objects to keep track of stats throughout the process
 mse.before <- rep(0, length(ids)) # MSE of the initial signature gene set according to the expected distribution
 names(mse.before)  <- ids
@@ -56,20 +55,20 @@
   if (length(Clusterlist[[id]][,1])<=n.genes){
 #    print(c("Not enough genes in the cluster. The number is", length(Clusterlist[[id]][,1])))
     return()
   }
 
   #colsum is the amount mapped genes in any given sample
   colsum <- colSums(Clusterlist[[id]][1:n.genes, ])
-  # extracting only the samples which contains above n.mapped.minimum mapped reads -- if there are above n.mapped.minimum reads we believe this is a true detection
+  # extracting only the samples which contains above 3 mapped reads -- if there are 3 reads we believe this is a true detection
   mapped <- colsum[colsum >= n.mapped.minimum]
   
   n_samples <- setNames(c(n_samples, sum(colsum>=n.mapped.minimum)), c(names(n_samples), id))
-  #if less than n.minimum.samples are mapped to the MGS, the MGS should be skipped
-  if (length(mapped) < n.minimum.samples){
+  #if less than 3 samples are mapped to the MGS, the MGS should be skipped
+  if (length(mapped) < 3){
 #    print("Not enough samples are mapped to the cluster")
     return()}
   genes <- names(Clusterlist[[id]][1:n.genes, 1])
   
   best.genes.step.zero <- genes
   ####################################################### The mean gene refinement #########################################################
   # loop over different threshold values for mean rank
@@ -148,21 +147,14 @@
                                n.genes,mapped = mapped)
       }
       
       if (length(init.genes$good.genes) < 10){ # if there is below 10 good genes it is impossible to fit model and there is no reason to keep going, hence the break
         MSE <- init.genes$mse
         break
       }
-
-      if ((min(500, length(Clusterlist[[id]][, 1]))-n.genes)<(n.genes-length(init.genes$good.genes))){ ##check if there is enough potential replacement genes in the geneset
-        MSE <- init.genes$mse
-        best.model <- init.genes
-        best.genes <- genes
-        break
-      }
       
       #if all the genes meet the threshold set up before then we are done
       #if we have 100 good genes then there is no reason to keep going
       if (length(init.genes$good.genes) == n.genes){
         MSE <- init.genes$mse
         best.model <- init.genes
         best.genes <- init.genes$good.genes
@@ -175,20 +167,14 @@
         MSE.old <- init.genes$mse
         mse.before[id] <- init.genes$mse
         
         #if not, then update the old MSE as the MSE of the from the previous iteration
       } else {
         MSE.old <- rotation$mse
       }
-    if ((n.genes+1)==min(500, length(Clusterlist[[id]][, 1]))){ # if there is only one gene to rotate it is not enough
-        MSE <- init.genes$mse
-        best.model <- init.genes
-        best.genes <- init.genes$good.genes
-        break
-      } 
     
       rotation <- rank.mat(id = id,
                            gene.names = init.genes$good.genes,
                            step = "mean",
                            phase = "rotation",
                            threshold = t,
                            t.start = n.genes,
@@ -285,27 +271,14 @@
         MSE <- init.quant$mse
         if (MSE < best.model$mse){
           best.model <- init.quant
           best.genes <- init.quant$good.genes}
         break
       }
       
-      if ((min(500, length(Clusterlist[[id]][, 1]))-n.genes)<(n.genes-length(init.quant$good.genes))){ # if there is not more new genes than genes required for rotation
-        best.model <- init.quant
-        best.genes <- new.genes
-        break
-      }
-
-    if ((n.genes+1)==min(500, length(Clusterlist[[id]][, 1]))){ # if there is only one gene to rotate it is not enough
-        MSE <- init.genes$mse
-        best.model <- init.genes
-        best.genes <- init.genes$good.genes
-        break
-      }
-
       # if there is only 5 good genes it is impossible to fit model
       if (length(init.quant$good.genes) < 5){ # if there is only 5 good gene it is impossible to fit model
         if (init.quant$mse < best.model$mse){#ØP: and if that model, using 5 or fewer, is still better, then use that?
           best.model <- init.quant
           best.genes <- new.genes
         }
         #print(c("There are not enough good genes to fit the model, the numer of good genes is:", length(init.quant$good.genes)))
```

### Comparing `maginator-0.1.20/maginator/workflow/scripts/abundance_profiles.R` & `maginator-0.1.8/maginator/workflow/scripts/abundance_profiles.R`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 taxonomy <- read.csv(snakemake@input[["annotation"]], header=FALSE, sep="\t") # the taxonomy 
 colnames(taxonomy) <- c("Cluster","Taxonomy")
 
 
 #setting important variables
 gene_index <- seq(1,length(GeneLengths))
 gene_names <- names(GeneLengths)
-n.mapped.minimum <- as.integer(snakemake@params[["min_mapped_signature_genes"]]) #The number of genes that needs reads that map to count the cluster as present
+n.mapped.minimum <- 3 #The number of genes that needs reads that map to count the cluster as present
 n.genes <- 100 # number of signature genes
 
 # inserting NA for the Clusters that do not have a annotation
 taxmat <- matrix("NA", nrow = length(names(Clusterlist)), ncol = 7)
 colnames(taxmat) <- c("Domain", "Phylum", "Class", "Order", "Family", "Genus", "Species")
 rownames(taxmat) <- names(Clusterlist)
 MGSids <- unlist(lapply(str_split(taxonomy$Cluster,","), '[[',1))
```

### Comparing `maginator-0.1.20/maginator/workflow/scripts/concat.py` & `maginator-0.1.8/maginator/workflow/scripts/concat.py`

 * *Files identical despite different names*

### Comparing `maginator-0.1.20/maginator/workflow/scripts/filter.py` & `maginator-0.1.8/maginator/workflow/scripts/filter.py`

 * *Files identical despite different names*

### Comparing `maginator-0.1.20/maginator/workflow/scripts/gene_cluster2tax.py` & `maginator-0.1.8/maginator/workflow/scripts/gene_cluster2tax.py`

 * *Files identical despite different names*

### Comparing `maginator-0.1.20/maginator/workflow/scripts/marker_genes.py` & `maginator-0.1.8/maginator/workflow/scripts/marker_genes.py`

 * *Files identical despite different names*

### Comparing `maginator-0.1.20/maginator/workflow/scripts/matrix2SG_formatconversion.R` & `maginator-0.1.8/maginator/workflow/scripts/matrix2SG_formatconversion.R`

 * *Files 12% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 cluster_names <- c()
 dir.create(snakemake@output[["clusters_dir"]])
 
 for (i in cluster_order){
   gene_names <- gene_clusters[gene_clusters$CLUSTERID == i,1] # getting the gene names of the cluster
   
   # Sort the gene count matrix of the MSP according to correlation
-  AbuMatrix <- as.matrix(genemat[gene_names,, drop=FALSE])
+  AbuMatrix <- as.matrix(genemat[gene_names,])
   Median_profile <- colMedians(AbuMatrix)
   pcc2MedianProfile <-cor(t(AbuMatrix) , Median_profile )
   gene_order <- row.names(pcc2MedianProfile)[order(pcc2MedianProfile, decreasing = TRUE)]
-  ordered_AbuMatrix <- AbuMatrix[gene_order,, drop=FALSE]
+  ordered_AbuMatrix <- AbuMatrix[gene_order,]
   
   m_name <- paste('Cluster', i, sep = "")
   cluster_mat <- paste('Cluster', i, sep = "")
   cluster_mat <- ordered_AbuMatrix
   assign(m_name, ordered_AbuMatrix)
   cluster_names <- c(cluster_names, m_name)
```

### Comparing `maginator-0.1.20/maginator/workflow/scripts/mpileup.py` & `maginator-0.1.8/maginator/workflow/scripts/mpileup.py`

 * *Files identical despite different names*

### Comparing `maginator-0.1.20/maginator/workflow/scripts/parse_gtdbtk.py` & `maginator-0.1.8/maginator/workflow/scripts/parse_gtdbtk.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,39 +33,35 @@
 tax_list = []
 gene_path_list = []
 gene_path_prot_list = []
 for clust in os.listdir(snakemake.input[0]):
 
     # Try reading both bacterial and archaeal summaries.
     try:
-        tax_bac = pd.read_csv(glob.glob(os.path.join(snakemake.input[0], clust, 'gtdbtk.bac*.summary.tsv'))[0], sep='\t', header=0)  
-        if tax_bac.iloc[0,1]=='Unclassified':
-            tax_bac=None
-        elif tax_bac.iloc[0,1]=='Unclassified Bacteria':
-            tax_bac=None
-    except (IndexError, FileNotFoundError):
+        tax_bac = pd.read_csv(os.path.join(snakemake.input[0], clust, 'gtdbtk.bac120.summary.tsv'), sep='\t', header=0)  
+    except FileNotFoundError:
         tax_bac = None
     try: 
-        tax_ar = pd.read_csv(glob.glob(os.path.join(snakemake.input[0], clust, 'gtdbtk.ar*.summary.tsv'))[0], sep='\t', header=0)  
-    except (IndexError, FileNotFoundError):
+        tax_ar = pd.read_csv(os.path.join(snakemake.input[0], clust, 'gtdbtk.ar122.summary.tsv'), sep='\t', header=0)  
+    except FileNotFoundError:
         tax_ar = None
 
     # Combine
     try:
         tax = pd.concat([tax_bac, tax_ar])
     except Exception:
         tax = None
 
     if tax is not None:
         
         classification = [x.split(';') for x in tax['classification']]
         
         # Remove unclassified
         classification = [x for x in classification if len(x) == 7]
-        
+       
         # Traverse from species annotation and up
         # Pick the annotation if the most common annotation is above prevalence set by parameter
         level = 6
         while level >= 0:
             annot = [x[level] for x in classification]
             cons = most_common(annot)
             if cons[1] >= float(snakemake.params[0])*len(annot):
@@ -88,29 +84,29 @@
         gene_path_list.append(os.path.join(gene_path, bin_id, bin_id+'_protein.fna'))
         gene_path_prot_list.append(os.path.join(gene_path, bin_id, bin_id+'_protein.faa'))
 
 # If similar at species level, then aggregate
 species_list = []
 mgs_list = []
 for clust in tax_list:
-    # If vamb_cluster parameter is not set, aggregate if species annotation is similar
+    # vamb_cluster parameter is set, not clusters are aggregated
     if bool(snakemake.params[2]):
+        mgs_list.append(clust)
+    # If vamb_cluster parameter is not set, aggregate if species annotation is similar
+    else:
         # If not species annotation, just add to final list
         if bool(re.search('s__$', clust[1])):
             mgs_list.append(clust)
         # If species annotation, check if it's already added to list - if False add to final list. If True append to existing
         else:
             if clust[1] in species_list:
                 mgs_list[[x[1] for x in mgs_list].index(clust[1])][0] += clust[0]
             else:
                 mgs_list.append(clust)
                 species_list.append(clust[1])
-    # vamb_cluster parameter is set, clusters are not aggregated
-    else:
-        mgs_list.append(clust)
 
 # Write metagenomicspecies file
 with open(snakemake.output[0], 'w') as fh:
     for mgs in mgs_list:
         rep = min([int(x) for x in mgs[0]])
         fh.write('{}\t{}\t{}\n'.format(str(rep), mgs[1], ','.join(mgs[0])))
 
@@ -143,18 +139,18 @@
                     line = ll.strip().split()
                     wfh.write(line[0]+'\t'+re.sub(',.*', '', line[1])+'\t'+vamb[re.sub('_[0-9]*$', '', line[0])]+'\n')
                 nl += 1
 
 # Collect all unique markers for phylogenetic analyses
 def unique_gtdb(domain, output):
     with open(output, 'w') as wfh:
-        for f in glob.glob(os.path.join(snakemake.input[0], '*', 'identify', 'gtdbtk.'+domain+'*.markers_summary.tsv')):
+        for f in glob.glob(os.path.join(snakemake.input[0], '*', 'identify', 'gtdbtk.'+domain+'.markers_summary.tsv')):
             with open(f, 'r') as rfh:
                 nl = 0
                 for ll in rfh:
                     if nl > 0:
                         line = ll.strip().split()
                         wfh.write(line[0]+'\t'+line[5]+'\n')
                     nl += 1
 
-unique_gtdb('bac', snakemake.output[3])
-unique_gtdb('ar', snakemake.output[4])
+unique_gtdb('bac120', snakemake.output[3])
+unique_gtdb('ar122', snakemake.output[4])
```

### Comparing `maginator-0.1.20/maginator/workflow/scripts/prescreening_genes.R` & `maginator-0.1.8/maginator/workflow/scripts/prescreening_genes.R`

 * *Files 8% similar despite different names*

```diff
@@ -6,29 +6,31 @@
 Clusterlist <- readRDS(snakemake@input[["clusters"]])
 GeneLengths <- readRDS(snakemake@input[["gene_lengths"]])
 
 #Number of signature genes
 n.genes <- 100
 
 #minimum number of mapped genes required
-n.mapped.minimum <- as.integer(snakemake@params[["min_mapped_signature_genes"]])
+n.mapped.minimum <- 3
 
 ids <- names(Clusterlist) #the ids of the MGS
 
 
 # identifying the names of genes in all MGS the dataset
 Cluster_gene_names <- c()
 for(Cluster in names(Clusterlist)){
   Cluster_gene_names <- c(Cluster_gene_names, rownames(Clusterlist[[Cluster]]))
 }
 present_genes <- GeneLengths[names(GeneLengths) %in% Cluster_gene_names]
 
 #preselecting genes
 for(id in ids){
   
+  print(id)
+
   genes_r <- Clusterlist[[id]]
   final.reads <- round(genes_r / (present_genes[rownames(genes_r)] * 10^-3))
   
   #finds the frequency of each gene. We want a ´p_sig_gene~1/n_signature_gene
   frequency_of_genes <- rowSums(final.reads>0, na.rm = T)
   
   #So, we want to choose a set of genes we can purify on that 1) are usually found in high frequency and 2) are relatively consisent with each other.
```

### Comparing `maginator-0.1.20/maginator/workflow/scripts/sort_gene_mat.py` & `maginator-0.1.8/maginator/workflow/scripts/sort_gene_mat.py`

 * *Files identical despite different names*

### Comparing `maginator-0.1.20/maginator/workflow/scripts/species_collections.py` & `maginator-0.1.8/maginator/workflow/scripts/species_collections.py`

 * *Files identical despite different names*

### Comparing `maginator-0.1.20/maginator/workflow/scripts/synteny.py` & `maginator-0.1.8/maginator/workflow/scripts/synteny.py`

 * *Files identical despite different names*

### Comparing `maginator-0.1.20/maginator/workflow.py` & `maginator-0.1.8/maginator/workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,28 +14,28 @@
         for key, val in vars(obj).items():
             setattr(self, key, val)
         
     def add_info(self, x):
         
         # Substitute resource information
         x = re.sub('{cores}', '{resources.cores}', x)
-        x = re.sub('{mem_gb}', '{resources.mem_gb}', x)
+        x = re.sub('{memory}', '{resources.memory}', x)
         x = re.sub('{runtime}', '{resources.runtime}', x)
    
         return x
 
     def run(self, snakefile):
 
         # Start message instance
         messages = Message(self)
 
         # Define core snakemake command
         cmd = ['snakemake',
                '--use-conda',
-               '--latency-wait', '150',
+               '--latency-wait', '20',
                '-s', snakefile,
                '--config',
                'wd='+self.output,
                'reads='+self.reads,
                'contigs='+self.contigs,
                'vamb='+self.vamb_clusters,
                'params='+self.params]
@@ -76,15 +76,15 @@
 
             # Final snakemake command
             cmd += ['--cluster', cluster_cmd]
 
         if self.cluster == 'slurm':
             
             cluster_cmd = 'sbatch' + ' ' + self.cluster_info
-            cluster_cmd = cluster_cmd + ' -e ' + self.output + 'logs/cluster_err/%j.err' + ' -o ' + self.output + 'logs/cluster_out/%j.out'
+            cluster_cmd = cluster_cmd + ' -e ' + self.output + 'logs/cluster_err' + ' -o ' + self.output + 'logs/cluster_out'
             cluster_cmd = self.add_info(cluster_cmd)
             
             # Final snakemake command
             cmd += ['--cluster', cluster_cmd]
 
         if self.cluster == 'drmaa':
             
@@ -93,15 +93,15 @@
             # Final snakemake command
             cmd += ['--cluster', cluster_cmd,
                     '--drmaa-log-dir', self.output+'logs/drmaa']
         
         # Only install conda envs if only_conda
         if self.only_conda:
             logging.info('Only creating conda environments.')
-            cmd.append('--conda-create-envs-only')
+            cmd.append(' --conda-create-envs-only')
 
         # If unlocking
         if self.unlock:
             logging.info('Unlocking working directory.')
             cmd.append('--unlock')
 
         logging.debug(' '.join(cmd))
```

### Comparing `maginator-0.1.20/maginator.egg-info/SOURCES.txt` & `maginator-0.1.8/maginator.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -21,29 +21,26 @@
 maginator/workflow/gtdbtk.Snakefile
 maginator/workflow/outgroup.Snakefile
 maginator/workflow/parse_gtdbtk.Snakefile
 maginator/workflow/phylo.Snakefile
 maginator/workflow/pileup.Snakefile
 maginator/workflow/pileup_parse.Snakefile
 maginator/workflow/prescreening_genes.Snakefile
-maginator/workflow/reads_to_bins.Snakefile
 maginator/workflow/signature_genes.Snakefile
 maginator/workflow/envs/filter_geneclusters.yaml
 maginator/workflow/envs/filter_gtdbtk.yaml
 maginator/workflow/envs/phylo.yaml
 maginator/workflow/envs/signature_genes.yaml
 maginator/workflow/scripts/Functions_v4.R
 maginator/workflow/scripts/MGS_counts.R
 maginator/workflow/scripts/SG_refinement.R
 maginator/workflow/scripts/abundance_profiles.R
-maginator/workflow/scripts/allele_frequency_mat.R
 maginator/workflow/scripts/concat.py
 maginator/workflow/scripts/filter.py
 maginator/workflow/scripts/gene_cluster2tax.py
-maginator/workflow/scripts/gene_refinement_plots.R
 maginator/workflow/scripts/marker_genes.py
 maginator/workflow/scripts/matrix2SG_formatconversion.R
 maginator/workflow/scripts/mpileup.py
 maginator/workflow/scripts/parse_gtdbtk.py
 maginator/workflow/scripts/prescreening_genes.R
 maginator/workflow/scripts/sort_gene_mat.py
 maginator/workflow/scripts/species_collections.py
```

### Comparing `maginator-0.1.20/setup.py` & `maginator-0.1.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="maginator", 
-    version="0.1.20",
-    author="Jakob Russel & Trine Zachariasen",
-    author_email="russel2620@gmail.com,trine_zachariasen@hotmail.com",
+    version="0.1.8",
+    author="Jakob Russel",
+    author_email="russel2620@gmail.com",
     description="MAGinator: Abundance, strain, and functional profiling of MAGs",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Russel88/MAGinator",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
```

