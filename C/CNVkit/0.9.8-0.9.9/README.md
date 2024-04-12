# Comparing `tmp/CNVkit-0.9.8.tar.gz` & `tmp/CNVkit-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/CNVkit-0.9.8.tar", last modified: Sun Dec 13 22:02:31 2020, max compression
+gzip compressed data, was "dist/CNVkit-0.9.9.tar", last modified: Fri May 28 07:11:51 2021, max compression
```

## Comparing `CNVkit-0.9.8.tar` & `CNVkit-0.9.9.tar`

### file list

```diff
@@ -1,91 +1,92 @@
-drwxr-xr-x   0 etalevich   (502) staff       (20)        0 2020-12-13 22:02:31.000000 CNVkit-0.9.8/
-drwxr-xr-x   0 etalevich   (502) staff       (20)        0 2020-12-13 22:02:31.000000 CNVkit-0.9.8/CNVkit.egg-info/
--rw-r--r--   0 etalevich   (502) staff       (20)     1170 2020-12-13 22:02:31.000000 CNVkit-0.9.8/CNVkit.egg-info/PKG-INFO
--rw-r--r--   0 etalevich   (502) staff       (20)     2113 2020-12-13 22:02:31.000000 CNVkit-0.9.8/CNVkit.egg-info/SOURCES.txt
--rw-r--r--   0 etalevich   (502) staff       (20)        1 2020-12-13 22:02:31.000000 CNVkit-0.9.8/CNVkit.egg-info/dependency_links.txt
--rw-r--r--   0 etalevich   (502) staff       (20)      150 2020-12-13 22:02:31.000000 CNVkit-0.9.8/CNVkit.egg-info/requires.txt
--rw-r--r--   0 etalevich   (502) staff       (20)       16 2020-12-13 22:02:31.000000 CNVkit-0.9.8/CNVkit.egg-info/top_level.txt
--rw-r--r--   0 etalevich   (502) staff       (20)     1170 2020-12-13 22:02:31.000000 CNVkit-0.9.8/PKG-INFO
--rw-r--r--   0 etalevich   (502) staff       (20)     6743 2020-08-24 20:51:54.000000 CNVkit-0.9.8/README.rst
--rwxr-xr-x   0 etalevich   (502) staff       (20)      289 2020-08-24 20:51:54.000000 CNVkit-0.9.8/cnvkit.py
-drwxr-xr-x   0 etalevich   (502) staff       (20)        0 2020-12-13 22:02:31.000000 CNVkit-0.9.8/cnvlib/
--rw-r--r--   0 etalevich   (502) staff       (20)      180 2020-08-24 20:51:54.000000 CNVkit-0.9.8/cnvlib/__init__.py
--rw-r--r--   0 etalevich   (502) staff       (20)       22 2020-12-13 22:02:05.000000 CNVkit-0.9.8/cnvlib/_version.py
--rw-r--r--   0 etalevich   (502) staff       (20)     5436 2020-08-24 20:51:54.000000 CNVkit-0.9.8/cnvlib/access.py
--rw-r--r--   0 etalevich   (502) staff       (20)     5712 2020-08-24 20:51:54.000000 CNVkit-0.9.8/cnvlib/antitarget.py
--rw-r--r--   0 etalevich   (502) staff       (20)     7639 2020-12-13 16:17:56.000000 CNVkit-0.9.8/cnvlib/autobin.py
--rw-r--r--   0 etalevich   (502) staff       (20)    10835 2020-12-13 16:17:56.000000 CNVkit-0.9.8/cnvlib/batch.py
--rw-r--r--   0 etalevich   (502) staff       (20)     4661 2020-08-24 20:51:54.000000 CNVkit-0.9.8/cnvlib/bintest.py
--rw-r--r--   0 etalevich   (502) staff       (20)    12160 2020-08-24 20:51:54.000000 CNVkit-0.9.8/cnvlib/call.py
--rw-r--r--   0 etalevich   (502) staff       (20)     9435 2020-08-24 20:51:54.000000 CNVkit-0.9.8/cnvlib/cluster.py
--rw-r--r--   0 etalevich   (502) staff       (20)     3636 2020-08-24 20:51:54.000000 CNVkit-0.9.8/cnvlib/cmdutil.py
--rw-r--r--   0 etalevich   (502) staff       (20)    21762 2020-08-24 20:51:54.000000 CNVkit-0.9.8/cnvlib/cnary.py
--rw-r--r--   0 etalevich   (502) staff       (20)    91532 2020-12-13 16:17:56.000000 CNVkit-0.9.8/cnvlib/commands.py
--rw-r--r--   0 etalevich   (502) staff       (20)     4253 2020-08-24 20:51:54.000000 CNVkit-0.9.8/cnvlib/core.py
--rw-r--r--   0 etalevich   (502) staff       (20)     9176 2020-12-13 16:17:56.000000 CNVkit-0.9.8/cnvlib/coverage.py
--rw-r--r--   0 etalevich   (502) staff       (20)     8397 2020-08-24 20:51:54.000000 CNVkit-0.9.8/cnvlib/descriptives.py
--rw-r--r--   0 etalevich   (502) staff       (20)     9591 2020-08-24 20:51:54.000000 CNVkit-0.9.8/cnvlib/diagram.py
--rw-r--r--   0 etalevich   (502) staff       (20)    22737 2020-08-24 20:51:54.000000 CNVkit-0.9.8/cnvlib/export.py
--rw-r--r--   0 etalevich   (502) staff       (20)    15248 2020-12-13 16:17:56.000000 CNVkit-0.9.8/cnvlib/fix.py
--rw-r--r--   0 etalevich   (502) staff       (20)     6172 2020-08-24 20:51:54.000000 CNVkit-0.9.8/cnvlib/heatmap.py
--rw-r--r--   0 etalevich   (502) staff       (20)     4553 2020-08-24 20:51:54.000000 CNVkit-0.9.8/cnvlib/import_rna.py
--rw-r--r--   0 etalevich   (502) staff       (20)     4347 2020-08-24 20:51:54.000000 CNVkit-0.9.8/cnvlib/importers.py
--rw-r--r--   0 etalevich   (502) staff       (20)     2087 2020-08-24 20:51:54.000000 CNVkit-0.9.8/cnvlib/metrics.py
--rw-r--r--   0 etalevich   (502) staff       (20)     2141 2020-08-24 20:51:54.000000 CNVkit-0.9.8/cnvlib/parallel.py
--rw-r--r--   0 etalevich   (502) staff       (20)      524 2020-08-24 20:51:54.000000 CNVkit-0.9.8/cnvlib/params.py
--rw-r--r--   0 etalevich   (502) staff       (20)    10378 2020-08-24 20:51:54.000000 CNVkit-0.9.8/cnvlib/plots.py
--rw-r--r--   0 etalevich   (502) staff       (20)    20954 2020-08-24 20:51:54.000000 CNVkit-0.9.8/cnvlib/reference.py
--rw-r--r--   0 etalevich   (502) staff       (20)     7036 2020-08-24 20:51:54.000000 CNVkit-0.9.8/cnvlib/reports.py
--rw-r--r--   0 etalevich   (502) staff       (20)    17009 2020-08-24 20:51:54.000000 CNVkit-0.9.8/cnvlib/rna.py
--rw-r--r--   0 etalevich   (502) staff       (20)     4371 2020-12-13 16:17:56.000000 CNVkit-0.9.8/cnvlib/samutil.py
--rw-r--r--   0 etalevich   (502) staff       (20)    23486 2020-08-24 20:51:54.000000 CNVkit-0.9.8/cnvlib/scatter.py
--rw-r--r--   0 etalevich   (502) staff       (20)     6736 2020-08-24 20:51:54.000000 CNVkit-0.9.8/cnvlib/segfilters.py
-drwxr-xr-x   0 etalevich   (502) staff       (20)        0 2020-12-13 22:02:31.000000 CNVkit-0.9.8/cnvlib/segmentation/
--rw-r--r--   0 etalevich   (502) staff       (20)    11917 2020-08-24 20:51:54.000000 CNVkit-0.9.8/cnvlib/segmentation/__init__.py
--rw-r--r--   0 etalevich   (502) staff       (20)     1592 2020-08-24 20:51:54.000000 CNVkit-0.9.8/cnvlib/segmentation/cbs.py
--rw-r--r--   0 etalevich   (502) staff       (20)      800 2020-08-24 20:51:54.000000 CNVkit-0.9.8/cnvlib/segmentation/flasso.py
--rw-r--r--   0 etalevich   (502) staff       (20)    19891 2020-08-24 20:51:54.000000 CNVkit-0.9.8/cnvlib/segmentation/haar.py
--rwxr-xr-x   0 etalevich   (502) staff       (20)     9459 2020-08-24 20:51:54.000000 CNVkit-0.9.8/cnvlib/segmentation/hmm.py
--rw-r--r--   0 etalevich   (502) staff       (20)      835 2020-08-24 20:51:54.000000 CNVkit-0.9.8/cnvlib/segmentation/none.py
--rw-r--r--   0 etalevich   (502) staff       (20)     8166 2020-08-24 20:51:54.000000 CNVkit-0.9.8/cnvlib/segmetrics.py
--rw-r--r--   0 etalevich   (502) staff       (20)    11785 2020-08-24 20:51:54.000000 CNVkit-0.9.8/cnvlib/smoothing.py
--rw-r--r--   0 etalevich   (502) staff       (20)     3456 2020-08-24 20:51:54.000000 CNVkit-0.9.8/cnvlib/target.py
--rw-r--r--   0 etalevich   (502) staff       (20)     7605 2020-08-24 20:51:54.000000 CNVkit-0.9.8/cnvlib/vary.py
-drwxr-xr-x   0 etalevich   (502) staff       (20)        0 2020-12-13 22:02:31.000000 CNVkit-0.9.8/scripts/
--rwxr-xr-x   0 etalevich   (502) staff       (20)      962 2020-08-24 20:51:55.000000 CNVkit-0.9.8/scripts/cnv_annotate.py
--rw-r--r--   0 etalevich   (502) staff       (20)     4318 2020-08-24 20:51:55.000000 CNVkit-0.9.8/scripts/cnv_expression_correlate.py
--rwxr-xr-x   0 etalevich   (502) staff       (20)     2314 2020-08-24 20:51:55.000000 CNVkit-0.9.8/scripts/cnv_updater.py
--rwxr-xr-x   0 etalevich   (502) staff       (20)    10383 2020-12-13 16:17:56.000000 CNVkit-0.9.8/scripts/guess_baits.py
--rwxr-xr-x   0 etalevich   (502) staff       (20)     1139 2020-08-24 20:51:55.000000 CNVkit-0.9.8/scripts/reference2targets.py
--rwxr-xr-x   0 etalevich   (502) staff       (20)     3378 2020-08-24 20:51:55.000000 CNVkit-0.9.8/scripts/skg_convert.py
--rw-r--r--   0 etalevich   (502) staff       (20)       67 2020-12-13 22:02:31.000000 CNVkit-0.9.8/setup.cfg
--rwxr-xr-x   0 etalevich   (502) staff       (20)     2055 2020-08-24 20:51:55.000000 CNVkit-0.9.8/setup.py
-drwxr-xr-x   0 etalevich   (502) staff       (20)        0 2020-12-13 22:02:31.000000 CNVkit-0.9.8/skgenome/
--rw-r--r--   0 etalevich   (502) staff       (20)       51 2020-08-24 20:51:55.000000 CNVkit-0.9.8/skgenome/__init__.py
--rw-r--r--   0 etalevich   (502) staff       (20)     1859 2020-08-24 20:51:55.000000 CNVkit-0.9.8/skgenome/chromsort.py
--rw-r--r--   0 etalevich   (502) staff       (20)     1484 2020-08-24 20:51:55.000000 CNVkit-0.9.8/skgenome/combiners.py
--rw-r--r--   0 etalevich   (502) staff       (20)    27628 2020-08-24 20:51:55.000000 CNVkit-0.9.8/skgenome/gary.py
--rw-r--r--   0 etalevich   (502) staff       (20)     8404 2020-10-16 04:22:45.000000 CNVkit-0.9.8/skgenome/intersect.py
--rw-r--r--   0 etalevich   (502) staff       (20)     7988 2020-08-24 20:51:55.000000 CNVkit-0.9.8/skgenome/merge.py
--rw-r--r--   0 etalevich   (502) staff       (20)     2219 2020-08-24 20:51:55.000000 CNVkit-0.9.8/skgenome/rangelabel.py
--rw-r--r--   0 etalevich   (502) staff       (20)     2058 2020-08-24 20:51:55.000000 CNVkit-0.9.8/skgenome/subdivide.py
--rw-r--r--   0 etalevich   (502) staff       (20)     2586 2020-08-24 20:51:55.000000 CNVkit-0.9.8/skgenome/subtract.py
-drwxr-xr-x   0 etalevich   (502) staff       (20)        0 2020-12-13 22:02:31.000000 CNVkit-0.9.8/skgenome/tabio/
--rw-r--r--   0 etalevich   (502) staff       (20)     9595 2020-08-24 20:51:55.000000 CNVkit-0.9.8/skgenome/tabio/__init__.py
--rw-r--r--   0 etalevich   (502) staff       (20)     3932 2020-08-24 20:51:55.000000 CNVkit-0.9.8/skgenome/tabio/bedio.py
--rw-r--r--   0 etalevich   (502) staff       (20)     6647 2020-08-24 20:51:55.000000 CNVkit-0.9.8/skgenome/tabio/genepred.py
--rw-r--r--   0 etalevich   (502) staff       (20)     2693 2020-08-24 20:51:55.000000 CNVkit-0.9.8/skgenome/tabio/gff.py
--rw-r--r--   0 etalevich   (502) staff       (20)     2484 2020-08-24 20:51:55.000000 CNVkit-0.9.8/skgenome/tabio/picard.py
--rw-r--r--   0 etalevich   (502) staff       (20)     7977 2020-08-24 20:51:55.000000 CNVkit-0.9.8/skgenome/tabio/seg.py
--rw-r--r--   0 etalevich   (502) staff       (20)     1332 2020-08-24 20:51:55.000000 CNVkit-0.9.8/skgenome/tabio/seqdict.py
--rw-r--r--   0 etalevich   (502) staff       (20)      934 2020-08-24 20:51:55.000000 CNVkit-0.9.8/skgenome/tabio/tab.py
--rw-r--r--   0 etalevich   (502) staff       (20)      895 2020-08-24 20:51:55.000000 CNVkit-0.9.8/skgenome/tabio/textcoord.py
--rw-r--r--   0 etalevich   (502) staff       (20)      275 2020-08-24 20:51:55.000000 CNVkit-0.9.8/skgenome/tabio/util.py
--rw-r--r--   0 etalevich   (502) staff       (20)    12157 2020-08-24 20:51:55.000000 CNVkit-0.9.8/skgenome/tabio/vcfio.py
--rw-r--r--   0 etalevich   (502) staff       (20)     3326 2020-08-24 20:51:55.000000 CNVkit-0.9.8/skgenome/tabio/vcfsimple.py
-drwxr-xr-x   0 etalevich   (502) staff       (20)        0 2020-12-13 22:02:31.000000 CNVkit-0.9.8/test/
--rwxr-xr-x   0 etalevich   (502) staff       (20)     6169 2020-08-24 20:51:55.000000 CNVkit-0.9.8/test/test_cnvlib.py
--rw-r--r--   0 etalevich   (502) staff       (20)    22535 2020-08-24 20:51:55.000000 CNVkit-0.9.8/test/test_commands.py
--rwxr-xr-x   0 etalevich   (502) staff       (20)    19988 2020-08-24 20:51:55.000000 CNVkit-0.9.8/test/test_genome.py
--rwxr-xr-x   0 etalevich   (502) staff       (20)     5474 2020-08-24 20:51:55.000000 CNVkit-0.9.8/test/test_io.py
--rwxr-xr-x   0 etalevich   (502) staff       (20)     1568 2020-08-24 20:51:55.000000 CNVkit-0.9.8/test/test_r.py
+drwxr-xr-x   0 erictalevich   (501) staff       (20)        0 2021-05-28 07:11:51.000000 CNVkit-0.9.9/
+-rw-r--r--   0 erictalevich   (501) staff       (20)     1170 2021-05-28 07:11:51.000000 CNVkit-0.9.9/PKG-INFO
+drwxr-xr-x   0 erictalevich   (501) staff       (20)        0 2021-05-28 07:11:51.000000 CNVkit-0.9.9/skgenome/
+-rw-r--r--   0 erictalevich   (501) staff       (20)     2224 2021-05-24 04:54:38.000000 CNVkit-0.9.9/skgenome/rangelabel.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)     7988 2021-04-05 17:40:15.000000 CNVkit-0.9.9/skgenome/merge.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)     2058 2021-04-05 17:40:15.000000 CNVkit-0.9.9/skgenome/subdivide.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)     2586 2021-04-05 17:40:15.000000 CNVkit-0.9.9/skgenome/subtract.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)     1484 2021-04-05 17:40:15.000000 CNVkit-0.9.9/skgenome/combiners.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)     1859 2021-04-05 17:40:15.000000 CNVkit-0.9.9/skgenome/chromsort.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)       51 2021-04-05 17:40:15.000000 CNVkit-0.9.9/skgenome/__init__.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)     8611 2021-04-05 17:40:15.000000 CNVkit-0.9.9/skgenome/intersect.py
+drwxr-xr-x   0 erictalevich   (501) staff       (20)        0 2021-05-28 07:11:51.000000 CNVkit-0.9.9/skgenome/tabio/
+-rw-r--r--   0 erictalevich   (501) staff       (20)    12157 2021-04-05 17:40:15.000000 CNVkit-0.9.9/skgenome/tabio/vcfio.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)     2484 2021-04-05 17:40:15.000000 CNVkit-0.9.9/skgenome/tabio/picard.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)      275 2021-04-05 17:40:15.000000 CNVkit-0.9.9/skgenome/tabio/util.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)     9594 2021-05-28 06:22:46.000000 CNVkit-0.9.9/skgenome/tabio/__init__.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)     6647 2021-04-05 17:40:15.000000 CNVkit-0.9.9/skgenome/tabio/genepred.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)     1331 2021-05-28 06:23:40.000000 CNVkit-0.9.9/skgenome/tabio/seqdict.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)      894 2021-05-28 06:23:51.000000 CNVkit-0.9.9/skgenome/tabio/textcoord.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)     7977 2021-04-05 17:40:15.000000 CNVkit-0.9.9/skgenome/tabio/seg.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)     3325 2021-05-28 06:24:01.000000 CNVkit-0.9.9/skgenome/tabio/vcfsimple.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)     2693 2021-04-05 17:40:15.000000 CNVkit-0.9.9/skgenome/tabio/gff.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)      934 2021-04-05 17:40:15.000000 CNVkit-0.9.9/skgenome/tabio/tab.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)     3931 2021-05-28 06:23:01.000000 CNVkit-0.9.9/skgenome/tabio/bedio.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)    27628 2021-04-05 17:40:15.000000 CNVkit-0.9.9/skgenome/gary.py
+drwxr-xr-x   0 erictalevich   (501) staff       (20)        0 2021-05-28 07:11:51.000000 CNVkit-0.9.9/test/
+-rwxr-xr-x   0 erictalevich   (501) staff       (20)     6169 2021-04-05 17:40:15.000000 CNVkit-0.9.9/test/test_cnvlib.py
+-rwxr-xr-x   0 erictalevich   (501) staff       (20)    19988 2021-04-05 17:40:15.000000 CNVkit-0.9.9/test/test_genome.py
+-rwxr-xr-x   0 erictalevich   (501) staff       (20)     5474 2021-04-05 17:40:15.000000 CNVkit-0.9.9/test/test_io.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)    22535 2021-04-05 17:40:15.000000 CNVkit-0.9.9/test/test_commands.py
+-rwxr-xr-x   0 erictalevich   (501) staff       (20)     1568 2021-04-05 17:40:15.000000 CNVkit-0.9.9/test/test_r.py
+drwxr-xr-x   0 erictalevich   (501) staff       (20)        0 2021-05-28 07:11:51.000000 CNVkit-0.9.9/CNVkit.egg-info/
+-rw-r--r--   0 erictalevich   (501) staff       (20)     1170 2021-05-28 07:11:51.000000 CNVkit-0.9.9/CNVkit.egg-info/PKG-INFO
+-rw-r--r--   0 erictalevich   (501) staff       (20)     2172 2021-05-28 07:11:51.000000 CNVkit-0.9.9/CNVkit.egg-info/SOURCES.txt
+-rw-r--r--   0 erictalevich   (501) staff       (20)      175 2021-05-28 07:11:51.000000 CNVkit-0.9.9/CNVkit.egg-info/requires.txt
+-rw-r--r--   0 erictalevich   (501) staff       (20)       16 2021-05-28 07:11:51.000000 CNVkit-0.9.9/CNVkit.egg-info/top_level.txt
+-rw-r--r--   0 erictalevich   (501) staff       (20)        1 2021-05-28 07:11:51.000000 CNVkit-0.9.9/CNVkit.egg-info/dependency_links.txt
+-rwxr-xr-x   0 erictalevich   (501) staff       (20)     2453 2021-05-28 06:40:51.000000 CNVkit-0.9.9/setup.py
+drwxr-xr-x   0 erictalevich   (501) staff       (20)        0 2021-05-28 07:11:51.000000 CNVkit-0.9.9/cnvlib/
+-rw-r--r--   0 erictalevich   (501) staff       (20)     6736 2021-04-05 17:40:15.000000 CNVkit-0.9.9/cnvlib/segfilters.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)     2087 2021-04-05 17:40:15.000000 CNVkit-0.9.9/cnvlib/metrics.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)     5712 2021-04-05 17:40:15.000000 CNVkit-0.9.9/cnvlib/antitarget.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)     6172 2021-04-05 17:40:15.000000 CNVkit-0.9.9/cnvlib/heatmap.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)      524 2021-04-05 17:40:15.000000 CNVkit-0.9.9/cnvlib/params.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)     9591 2021-04-05 17:40:15.000000 CNVkit-0.9.9/cnvlib/diagram.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)     8397 2021-04-05 17:40:15.000000 CNVkit-0.9.9/cnvlib/descriptives.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)       22 2021-05-28 07:09:26.000000 CNVkit-0.9.9/cnvlib/_version.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)     7692 2021-05-24 16:48:44.000000 CNVkit-0.9.9/cnvlib/autobin.py
+drwxr-xr-x   0 erictalevich   (501) staff       (20)        0 2021-05-28 07:11:51.000000 CNVkit-0.9.9/cnvlib/segmentation/
+-rw-r--r--   0 erictalevich   (501) staff       (20)      835 2021-04-05 17:40:15.000000 CNVkit-0.9.9/cnvlib/segmentation/none.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)    11917 2021-04-05 17:40:15.000000 CNVkit-0.9.9/cnvlib/segmentation/__init__.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)    19903 2021-05-24 04:54:38.000000 CNVkit-0.9.9/cnvlib/segmentation/haar.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)     1592 2021-04-05 17:40:15.000000 CNVkit-0.9.9/cnvlib/segmentation/cbs.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)      800 2021-04-05 17:40:15.000000 CNVkit-0.9.9/cnvlib/segmentation/flasso.py
+-rwxr-xr-x   0 erictalevich   (501) staff       (20)     9459 2021-04-05 17:40:15.000000 CNVkit-0.9.9/cnvlib/segmentation/hmm.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)     3636 2021-04-05 17:40:15.000000 CNVkit-0.9.9/cnvlib/cmdutil.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)     7605 2021-04-05 17:40:15.000000 CNVkit-0.9.9/cnvlib/vary.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)    10835 2021-04-05 17:40:15.000000 CNVkit-0.9.9/cnvlib/batch.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)     5436 2021-04-05 17:40:15.000000 CNVkit-0.9.9/cnvlib/access.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)      180 2021-04-05 17:40:15.000000 CNVkit-0.9.9/cnvlib/__init__.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)     4253 2021-04-05 17:40:15.000000 CNVkit-0.9.9/cnvlib/core.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)     8973 2021-05-24 04:54:38.000000 CNVkit-0.9.9/cnvlib/coverage.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)     4553 2021-04-05 17:40:15.000000 CNVkit-0.9.9/cnvlib/import_rna.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)    22737 2021-04-05 17:40:15.000000 CNVkit-0.9.9/cnvlib/export.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)     4347 2021-04-05 17:40:15.000000 CNVkit-0.9.9/cnvlib/importers.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)    17009 2021-04-05 17:40:15.000000 CNVkit-0.9.9/cnvlib/rna.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)    10378 2021-04-05 17:40:15.000000 CNVkit-0.9.9/cnvlib/plots.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)     9435 2021-04-05 17:40:15.000000 CNVkit-0.9.9/cnvlib/cluster.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)    15248 2021-04-05 17:40:15.000000 CNVkit-0.9.9/cnvlib/fix.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)    23737 2021-05-24 04:54:38.000000 CNVkit-0.9.9/cnvlib/scatter.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)     4371 2021-04-05 17:40:15.000000 CNVkit-0.9.9/cnvlib/samutil.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)     7036 2021-04-05 17:40:15.000000 CNVkit-0.9.9/cnvlib/reports.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)    20954 2021-04-05 17:40:15.000000 CNVkit-0.9.9/cnvlib/reference.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)     3456 2021-04-05 17:40:15.000000 CNVkit-0.9.9/cnvlib/target.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)    12500 2021-05-24 04:54:38.000000 CNVkit-0.9.9/cnvlib/smoothing.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)    12160 2021-04-05 17:40:15.000000 CNVkit-0.9.9/cnvlib/call.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)     2141 2021-04-05 17:40:15.000000 CNVkit-0.9.9/cnvlib/parallel.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)    91857 2021-05-24 04:54:38.000000 CNVkit-0.9.9/cnvlib/commands.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)     4661 2021-04-05 17:40:15.000000 CNVkit-0.9.9/cnvlib/bintest.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)     8166 2021-04-05 17:40:15.000000 CNVkit-0.9.9/cnvlib/segmetrics.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)    21724 2021-05-24 04:54:38.000000 CNVkit-0.9.9/cnvlib/cnary.py
+-rwxr-xr-x   0 erictalevich   (501) staff       (20)      289 2021-04-05 17:40:15.000000 CNVkit-0.9.9/cnvkit.py
+drwxr-xr-x   0 erictalevich   (501) staff       (20)        0 2021-05-28 07:11:51.000000 CNVkit-0.9.9/scripts/
+-rw-r--r--   0 erictalevich   (501) staff       (20)     4318 2021-04-05 17:40:15.000000 CNVkit-0.9.9/scripts/cnv_expression_correlate.py
+-rwxr-xr-x   0 erictalevich   (501) staff       (20)     3378 2021-04-05 17:40:15.000000 CNVkit-0.9.9/scripts/skg_convert.py
+-rwxr-xr-x   0 erictalevich   (501) staff       (20)     1139 2021-04-05 17:40:15.000000 CNVkit-0.9.9/scripts/reference2targets.py
+-rwxr-xr-x   0 erictalevich   (501) staff       (20)      962 2021-04-05 17:40:15.000000 CNVkit-0.9.9/scripts/cnv_annotate.py
+-rwxr-xr-x   0 erictalevich   (501) staff       (20)     2314 2021-04-05 17:40:15.000000 CNVkit-0.9.9/scripts/cnv_updater.py
+-rwxr-xr-x   0 erictalevich   (501) staff       (20)    10375 2021-04-05 17:40:15.000000 CNVkit-0.9.9/scripts/guess_baits.py
+-rwxr-xr-x   0 erictalevich   (501) staff       (20)     2000 2021-05-28 06:36:46.000000 CNVkit-0.9.9/scripts/genome_instability_index.py
+-rw-r--r--   0 erictalevich   (501) staff       (20)       67 2021-05-28 07:11:51.000000 CNVkit-0.9.9/setup.cfg
+-rw-r--r--   0 erictalevich   (501) staff       (20)     6743 2021-05-28 07:02:16.000000 CNVkit-0.9.9/README.rst
```

### Comparing `CNVkit-0.9.8/CNVkit.egg-info/PKG-INFO` & `CNVkit-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: CNVkit
-Version: 0.9.8
+Version: 0.9.9
 Summary: Copy number variation toolkit for high-throughput sequencing.
 Home-page: http://github.com/etal/cnvkit
 Author: Eric Talevich
 Author-email: eric.talevich@ucsf.edu
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `CNVkit-0.9.8/CNVkit.egg-info/SOURCES.txt` & `CNVkit-0.9.9/CNVkit.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 README.rst
 setup.cfg
 setup.py
 ./cnvkit.py
 ./scripts/cnv_annotate.py
 ./scripts/cnv_expression_correlate.py
 ./scripts/cnv_updater.py
+./scripts/genome_instability_index.py
 ./scripts/guess_baits.py
 ./scripts/reference2targets.py
 ./scripts/skg_convert.py
-/Users/etalevich/code/cnvkit/cnvkit.py
-/Users/etalevich/code/cnvkit/scripts/cnv_annotate.py
-/Users/etalevich/code/cnvkit/scripts/cnv_expression_correlate.py
-/Users/etalevich/code/cnvkit/scripts/cnv_updater.py
-/Users/etalevich/code/cnvkit/scripts/guess_baits.py
-/Users/etalevich/code/cnvkit/scripts/reference2targets.py
-/Users/etalevich/code/cnvkit/scripts/skg_convert.py
+/Users/erictalevich/code/cnvkit/cnvkit.py
+/Users/erictalevich/code/cnvkit/scripts/cnv_annotate.py
+/Users/erictalevich/code/cnvkit/scripts/cnv_expression_correlate.py
+/Users/erictalevich/code/cnvkit/scripts/cnv_updater.py
+/Users/erictalevich/code/cnvkit/scripts/guess_baits.py
+/Users/erictalevich/code/cnvkit/scripts/reference2targets.py
+/Users/erictalevich/code/cnvkit/scripts/skg_convert.py
 CNVkit.egg-info/PKG-INFO
 CNVkit.egg-info/SOURCES.txt
 CNVkit.egg-info/dependency_links.txt
 CNVkit.egg-info/requires.txt
 CNVkit.egg-info/top_level.txt
 cnvlib/__init__.py
 cnvlib/_version.py
```

### Comparing `CNVkit-0.9.8/PKG-INFO` & `CNVkit-0.9.9/CNVkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: CNVkit
-Version: 0.9.8
+Version: 0.9.9
 Summary: Copy number variation toolkit for high-throughput sequencing.
 Home-page: http://github.com/etal/cnvkit
 Author: Eric Talevich
 Author-email: eric.talevich@ucsf.edu
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `CNVkit-0.9.8/README.rst` & `CNVkit-0.9.9/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 ======
 
 A command-line toolkit and Python library for detecting copy number variants
 and alterations genome-wide from high-throughput sequencing.
 
 Read the full documentation at: http://cnvkit.readthedocs.io
 
-.. image:: https://travis-ci.org/etal/cnvkit.svg?branch=master
-    :target: https://travis-ci.org/etal/cnvkit
+.. image:: https://travis-ci.com/etal/cnvkit.svg?branch=master
+    :target: https://travis-ci.com/etal/cnvkit
     :alt: Build status
 
 .. image:: https://landscape.io/github/etal/cnvkit/master/landscape.svg
     :target: https://landscape.io/github/etal/cnvkit/master
     :alt: Code health
 
 .. image::   https://codecov.io/github/etal/cnvkit/coverage.svg?branch=master
```

### Comparing `CNVkit-0.9.8/cnvlib/access.py` & `CNVkit-0.9.9/cnvlib/access.py`

 * *Files identical despite different names*

### Comparing `CNVkit-0.9.8/cnvlib/antitarget.py` & `CNVkit-0.9.9/cnvlib/antitarget.py`

 * *Files identical despite different names*

### Comparing `CNVkit-0.9.8/cnvlib/autobin.py` & `CNVkit-0.9.9/cnvlib/autobin.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 
 
 def midsize_file(fnames):
     """Select the median-size file from several given filenames.
 
     If an even number of files is given, selects the file just below the median.
     """
-    return sorted(fnames, key=lambda f: os.stat(f).st_size
-                 )[len(fnames) // 2 - 1]
+    assert fnames, 'No files provided to calculate the median size.'
+    return sorted(fnames, key=lambda f: os.stat(f).st_size)[(len(fnames) - 1) // 2]
 
 
 def do_autobin(bam_fname, method, targets=None, access=None,
                bp_per_bin=100000., target_min_size=20, target_max_size=50000,
                antitarget_min_size=500, antitarget_max_size=1000000, fasta=None):
     """Quickly calculate reasonable bin sizes from BAM read counts.
```

### Comparing `CNVkit-0.9.8/cnvlib/batch.py` & `CNVkit-0.9.9/cnvlib/batch.py`

 * *Files identical despite different names*

### Comparing `CNVkit-0.9.8/cnvlib/bintest.py` & `CNVkit-0.9.9/cnvlib/bintest.py`

 * *Files identical despite different names*

### Comparing `CNVkit-0.9.8/cnvlib/call.py` & `CNVkit-0.9.9/cnvlib/call.py`

 * *Files identical despite different names*

### Comparing `CNVkit-0.9.8/cnvlib/cluster.py` & `CNVkit-0.9.9/cnvlib/cluster.py`

 * *Files identical despite different names*

### Comparing `CNVkit-0.9.8/cnvlib/cmdutil.py` & `CNVkit-0.9.9/cnvlib/cmdutil.py`

 * *Files identical despite different names*

### Comparing `CNVkit-0.9.8/cnvlib/cnary.py` & `CNVkit-0.9.9/cnvlib/cnary.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,36 +79,35 @@
 
         Yields
         ------
         tuple
             Pairs of: (gene name, CNA of rows with same name)
         """
         ignore += params.ANTITARGET_ALIASES
-        start_idx = end_idx = None
         for _chrom, subgary in self.by_chromosome():
             prev_idx = 0
             for gene, gene_idx in subgary._get_gene_map().items():
                 if gene not in ignore:
                     if not len(gene_idx):
                         logging.warning("Specified gene name somehow missing: "
                                         "%s", gene)
                         continue
                     start_idx = gene_idx[0]
                     end_idx = gene_idx[-1] + 1
                     if prev_idx < start_idx:
                         # Include intergenic regions
                         yield params.ANTITARGET_NAME, subgary.as_dataframe(
-                                subgary.data.iloc[prev_idx:start_idx])
+                                subgary.data.loc[prev_idx:start_idx])
                     yield gene, subgary.as_dataframe(
-                            subgary.data.iloc[start_idx:end_idx])
+                            subgary.data.loc[start_idx:end_idx])
                     prev_idx = end_idx
             if prev_idx < len(subgary) - 1:
                 # Include the telomere
                 yield params.ANTITARGET_NAME, subgary.as_dataframe(
-                        subgary.data.iloc[prev_idx:])
+                        subgary.data.loc[prev_idx:])
 
     # Manipulation
 
     def center_all(self, estimator=pd.Series.median, by_chrom=True,
                    skip_low=False, verbose=False):
         """Re-center log2 values to the autosomes' average (in-place).
```

### Comparing `CNVkit-0.9.8/cnvlib/commands.py` & `CNVkit-0.9.9/cnvlib/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -375,26 +375,26 @@
 
     # Create & write BED files
     target_out_arr = target.do_target(access_arr if args.method == 'wgs'
                                       else tgt_arr,
                                       args.annotate, args.short_names,
                                       do_split=True, avg_size=tgt_bin_size)
     tgt_name_base = tgt_arr.sample_id if tgt_arr else core.fbase(bam_fname)
-    target_bed = tgt_name_base + '.target.bed'
+    target_bed = args.target_output_bed or tgt_name_base + '.target.bed'
     tabio.write(target_out_arr, target_bed, "bed4")
     if args.method == "hybrid" and anti_bin_size:
         # Build antitarget BED from the given targets
         anti_arr = antitarget.do_antitarget(target_out_arr,
                                             access=access_arr,
                                             avg_bin_size=anti_bin_size,
                                             min_bin_size=args.antitarget_min_size)
     else:
         # No antitargets for wgs, amplicon
         anti_arr = _GA([])
-    antitarget_bed = tgt_name_base + '.antitarget.bed'
+    antitarget_bed = args.antitarget_output_bed or tgt_name_base + '.antitarget.bed'
     tabio.write(anti_arr, antitarget_bed, "bed4")
 
     # Print depths & bin sizes as a table on stdout
     labels = ("Target", "Antitarget")
     width = max(map(len, labels)) + 1
     print(" " * width, "Depth", "Bin size", sep='\t')
     for label, (depth, binsize) in zip(labels, fields):
@@ -436,23 +436,32 @@
 P_autobin.add_argument('--antitarget-max-size', metavar="BASES",
         type=int, default=500000,
         help="Maximum size of antitarget bins. [Default: %(default)s]")
 P_autobin.add_argument('--antitarget-min-size', metavar="BASES",
         type=int, default=500,
         help="Minimum size of antitarget bins. [Default: %(default)s]")
 
-P_autobin.add_argument('--annotate', metavar="FILENAME",
-        help="""Use gene models from this file to assign names to the target
-                regions. Format: UCSC refFlat.txt or ensFlat.txt file
-                (preferred), or BED, interval list, GFF, or similar.""")
-P_autobin.add_argument('--short-names', action='store_true',
-        help="Reduce multi-accession bait labels to be short and consistent.")
-    # Option: --dry-run to not write BED files?
-
-#  P_autobin.add_argument('-o', '--output', help="Output filename.")
+P_autobin.add_argument(
+    '--annotate', metavar='FILENAME',
+    help="""Use gene models from this file to assign names to the target regions. Format: UCSC refFlat.txt or 
+            ensFlat.txt file (preferred), or BED, interval list, GFF, or similar."""
+)
+P_autobin.add_argument(
+    '--short-names', action='store_true',
+    help='Reduce multi-accession bait labels to be short and consistent.'
+)
+P_autobin.add_argument(
+    '--target-output-bed', metavar='FILENAME',
+    help='Filename for target BED output. If not specified, constructed from the input file basename.'
+)
+P_autobin.add_argument(
+    '--antitarget-output-bed', metavar='FILENAME',
+    help='Filename for antitarget BED output. If not specified, constructed from the input file basename.'
+)
+# Option: --dry-run to not write BED files?
 P_autobin.set_defaults(func=_cmd_autobin)
 
 
 # coverage --------------------------------------------------------------------
 
 do_coverage = public(coverage.do_coverage)
 
@@ -658,15 +667,15 @@
                                            variants=variants,
                                            skip_low=args.drop_low_coverage,
                                            skip_outliers=args.drop_outliers,
                                            save_dataframe=bool(args.dataframe),
                                            rscript_path=args.rscript_path,
                                            processes=args.processes,
                                            smooth_cbs=args.smooth_cbs)
-	
+
     if args.dataframe:
         segments, dframe = results
         with open(args.dataframe, 'w') as handle:
             handle.write(dframe)
         logging.info("Wrote %s", args.dataframe)
     else:
         segments = results
@@ -1652,15 +1661,15 @@
                 [Default: %(default)s]""")
 P_export_bed.add_argument('-y', '--male-reference', '--haploid-x-reference',
         action='store_true',
         help="""Was a male reference used?  If so, expect half ploidy on
                 chrX and chrY; otherwise, only chrY has half ploidy.  In CNVkit,
                 if a male reference was used, the "neutral" copy number (ploidy)
                 of chrX is 1; chrY is haploid for either reference sex.""")
-P_export_bed.add_argument('-o', '--output', metavar="FILENAME", 
+P_export_bed.add_argument('-o', '--output', metavar="FILENAME",
         help="Output file name.")
 P_export_bed.set_defaults(func=_cmd_export_bed)
 
 
 # SEG special case: segment coords don't match across samples
 def _cmd_export_seg(args):
     """Convert segments to SEG format.
```

### Comparing `CNVkit-0.9.8/cnvlib/core.py` & `CNVkit-0.9.9/cnvlib/core.py`

 * *Files identical despite different names*

### Comparing `CNVkit-0.9.8/cnvlib/coverage.py` & `CNVkit-0.9.9/cnvlib/coverage.py`

 * *Files 4% similar despite different names*

```diff
@@ -135,20 +135,15 @@
 
     count = 0
     bases = 0
     for read in bamfile.fetch(reference=chrom, start=start, end=end):
         if filter_read(read):
             count += 1
             # Only count the bases aligned to the region
-            rlen = read.query_alignment_length
-            if read.pos < start:
-                rlen -= start - read.pos
-            if read.pos + read.query_alignment_length > end:
-                rlen -= read.pos + read.query_alignment_length - end
-            bases += rlen
+            bases += sum([1 for p in read.positions if start <= p < end])
     depth = bases / (end - start) if end > start else 0
     row = (chrom, start, end, gene,
            math.log(depth, 2) if depth else NULL_LOG2_COVERAGE,
            depth)
     return count, row
```

### Comparing `CNVkit-0.9.8/cnvlib/descriptives.py` & `CNVkit-0.9.9/cnvlib/descriptives.py`

 * *Files identical despite different names*

### Comparing `CNVkit-0.9.8/cnvlib/diagram.py` & `CNVkit-0.9.9/cnvlib/diagram.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     elif segarr:
         # Both segments and bin-level ratios
         rows = reports.gene_metrics_by_segment(cnarr, segarr, threshold)
         probes_attr = 'segment_probes'
     else:
         # Only bin-level ratios (.cnr)
         rows = reports.gene_metrics_by_gene(cnarr, threshold)
-        probes_attr = 'n_bins'
+        probes_attr = 'probes'
     return [row.gene for row in rows if getattr(row, probes_attr) >= min_probes]
 
 
 def build_chrom_diagram(features, chr_sizes, sample_id, title=None):
     """Create a PDF of color-coded features on chromosomes."""
     max_chr_len = max(chr_sizes.values())
```

### Comparing `CNVkit-0.9.8/cnvlib/export.py` & `CNVkit-0.9.9/cnvlib/export.py`

 * *Files identical despite different names*

### Comparing `CNVkit-0.9.8/cnvlib/fix.py` & `CNVkit-0.9.9/cnvlib/fix.py`

 * *Files identical despite different names*

### Comparing `CNVkit-0.9.8/cnvlib/heatmap.py` & `CNVkit-0.9.9/cnvlib/heatmap.py`

 * *Files identical despite different names*

### Comparing `CNVkit-0.9.8/cnvlib/import_rna.py` & `CNVkit-0.9.9/cnvlib/import_rna.py`

 * *Files identical despite different names*

### Comparing `CNVkit-0.9.8/cnvlib/importers.py` & `CNVkit-0.9.9/cnvlib/importers.py`

 * *Files identical despite different names*

### Comparing `CNVkit-0.9.8/cnvlib/metrics.py` & `CNVkit-0.9.9/cnvlib/metrics.py`

 * *Files identical despite different names*

### Comparing `CNVkit-0.9.8/cnvlib/parallel.py` & `CNVkit-0.9.9/cnvlib/parallel.py`

 * *Files identical despite different names*

### Comparing `CNVkit-0.9.8/cnvlib/params.py` & `CNVkit-0.9.9/cnvlib/params.py`

 * *Files identical despite different names*

### Comparing `CNVkit-0.9.8/cnvlib/plots.py` & `CNVkit-0.9.9/cnvlib/plots.py`

 * *Files identical despite different names*

### Comparing `CNVkit-0.9.8/cnvlib/reference.py` & `CNVkit-0.9.9/cnvlib/reference.py`

 * *Files identical despite different names*

### Comparing `CNVkit-0.9.8/cnvlib/reports.py` & `CNVkit-0.9.9/cnvlib/reports.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
     rows = list(rows)
     columns = (rows[0].index if len(rows) else cnarr._required_columns)
     columns = ["gene"] + [col for col in columns if col != "gene"]
     table = pd.DataFrame.from_records(rows).reindex(columns=columns)
     if min_probes and len(table):
         n_probes = (table.segment_probes
                     if 'segment_probes' in table.columns
-                    else table.n_bins)
+                    else table.probes)
         table = table[n_probes >= min_probes]
     return table
 
 
 def gene_metrics_by_gene(cnarr, threshold, skip_low=False):
     """Identify genes where average bin copy ratio value exceeds `threshold`.
 
@@ -157,15 +157,15 @@
         segmean = segment_mean(rows, skip_low)
         if segmean is None:
             continue
         outrow = rows[0].copy()
         outrow["end"] = rows.end.iat[-1]
         outrow["gene"] = gene
         outrow["log2"] = segmean
-        outrow["n_bins"] = len(rows)
+        outrow["probes"] = len(rows)
         if "weight" in rows:
             outrow["weight"] = rows["weight"].sum()
             if "depth" in rows:
                 outrow["depth"] = np.average(rows["depth"],
                                              weights=rows["weight"])
         elif "depth" in rows:
             outrow["depth"] = rows["depth"].mean()
```

### Comparing `CNVkit-0.9.8/cnvlib/rna.py` & `CNVkit-0.9.9/cnvlib/rna.py`

 * *Files identical despite different names*

### Comparing `CNVkit-0.9.8/cnvlib/samutil.py` & `CNVkit-0.9.9/cnvlib/samutil.py`

 * *Files identical despite different names*

### Comparing `CNVkit-0.9.8/cnvlib/scatter.py` & `CNVkit-0.9.9/cnvlib/scatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,23 +127,24 @@
         if probes and chrom in chrom_probes:
             subprobes = chrom_probes[chrom]
             x = 0.5 * (subprobes['start'] + subprobes['end']) + x_offset
             axis.scatter(x, subprobes['log2'], marker='.',
                          color=POINT_COLOR, edgecolor='none', alpha=0.2)
             if do_trend:
                 # ENH break trendline by chromosome arm boundaries?
-                axis.plot(x, subprobes.smooth_log2(),  #window_size),
-                        color=POINT_COLOR, linewidth=2, zorder=-1)
+                # Here and in subsequent occurrences, it's important to use snap=False to avoid short lines/segment
+                # disappearing when saving as PNG. See also https://github.com/etal/cnvkit/issues/604.
+                axis.plot(x, subprobes.smooth_log2(), color=POINT_COLOR, linewidth=2, zorder=-1, snap=False)
 
         if chrom in chrom_segs:
             for seg in chrom_segs[chrom]:
                 color = choose_segment_color(seg, segment_color)
                 axis.plot((seg.start + x_offset, seg.end + x_offset),
                           (seg.log2, seg.log2),
-                          color=color, linewidth=3, solid_capstyle='round')
+                          color=color, linewidth=3, solid_capstyle='round', snap=False)
     return axis
 
 def snv_on_genome(axis, variants, chrom_sizes, segments, do_trend, segment_color):
     """Plot a scatter-plot of SNP chromosomal positions and shifts."""
     axis.set_ylim(0.0, 1.0)
     axis.set_ylabel("VAF")
     x_starts = plots.plot_x_dividers(axis, chrom_sizes)
@@ -179,15 +180,15 @@
                                                  default_bright=False)
                 else:
                     posn = [snvs.start.iat[0] + x_offset,
                             snvs.start.iat[-1] + x_offset]
                     color = TREND_COLOR
                 axis.plot(posn, [v_freq, v_freq],
                           color=color, linewidth=2, zorder=-1,
-                          solid_capstyle='round')
+                          solid_capstyle='round', snap=False)
     return axis
 
 # === Chromosome-level scatter plots ===
 
 def chromosome_scatter(cnarr, segments, variants, show_range, show_gene,
                        antitarget_marker, do_trend, by_bin, window_width,
                        y_min, y_max, title, segment_color):
@@ -403,23 +404,23 @@
         axis.scatter(x_fg, y_fg, w_fg, color=POINT_COLOR, alpha=0.4, marker='o')
         axis.scatter(x_bg, y_bg, color=POINT_COLOR, alpha=0.5,
                      marker=antitarget_marker)
 
     # Add a local trend line
     if do_trend:
         axis.plot(x, probes.smooth_log2(),  #.1),
-                  color=POINT_COLOR, linewidth=2, zorder=-1)
+                  color=POINT_COLOR, linewidth=2, zorder=-1, snap=False)
 
     # Draw segments as horizontal lines
     if segments:
         for row in segments:
             color = choose_segment_color(row, segment_color)
             axis.plot((row.start * MB, row.end * MB),
                       (row.log2, row.log2),
-                      color=color, linewidth=4, solid_capstyle='round')
+                      color=color, linewidth=4, solid_capstyle='round', snap=False)
     return axis
 
 def snv_on_chromosome(axis, variants, segments, genes, do_trend, by_bin,
                       segment_color):
     # TODO set x-limits if not already done for probes/segments
     # set_xlim_from(axis, None, segments, variants)
     # setup_chromosome(axis, 0.0, 1.0, "VAF")
@@ -445,15 +446,15 @@
                 color = choose_segment_color(seg, segment_color,
                                              default_bright=False)
             else:
                 posn = [variants.start.iat[0] * MB, variants.start.iat[-1] * MB]
                 color = TREND_COLOR
             axis.plot(posn, [v_freq, v_freq],
                       color=color, linewidth=2, zorder=1,
-                      solid_capstyle='round')
+                      solid_capstyle='round', snap=False)
 
     if genes:
         highlight_genes(axis, genes, .9)
     return axis
 
 def set_xlim_from(axis, probes=None, segments=None, variants=None):
     """Configure axes for plotting a single chromosome's data.
```

### Comparing `CNVkit-0.9.8/cnvlib/segfilters.py` & `CNVkit-0.9.9/cnvlib/segfilters.py`

 * *Files identical despite different names*

### Comparing `CNVkit-0.9.8/cnvlib/segmentation/__init__.py` & `CNVkit-0.9.9/cnvlib/segmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `CNVkit-0.9.8/cnvlib/segmentation/cbs.py` & `CNVkit-0.9.9/cnvlib/segmentation/cbs.py`

 * *Files identical despite different names*

### Comparing `CNVkit-0.9.8/cnvlib/segmentation/flasso.py` & `CNVkit-0.9.9/cnvlib/segmentation/flasso.py`

 * *Files identical despite different names*

### Comparing `CNVkit-0.9.8/cnvlib/segmentation/haar.py` & `CNVkit-0.9.9/cnvlib/segmentation/haar.py`

 * *Files 0% similar despite different names*

```diff
@@ -567,12 +567,12 @@
 
     logging.info("%s", seg_table)
 
     from matplotlib import pyplot
     indices = np.arange(len(noisy_data))
     pyplot.scatter(indices, noisy_data, alpha=0.2, color='gray')
     x, y = table2coords(seg_table)
-    pyplot.plot(x, y, color='r', marker='x', lw=2)
+    pyplot.plot(x, y, color='r', marker='x', lw=2, snap=False)
     pyplot.show()
 
     # # The complete segmented signal
     # lines(seg.data$Segmented, col="red", lwd=3)
```

### Comparing `CNVkit-0.9.8/cnvlib/segmentation/hmm.py` & `CNVkit-0.9.9/cnvlib/segmentation/hmm.py`

 * *Files identical despite different names*

### Comparing `CNVkit-0.9.8/cnvlib/segmentation/none.py` & `CNVkit-0.9.9/cnvlib/segmentation/none.py`

 * *Files identical despite different names*

### Comparing `CNVkit-0.9.8/cnvlib/segmetrics.py` & `CNVkit-0.9.9/cnvlib/segmetrics.py`

 * *Files identical despite different names*

### Comparing `CNVkit-0.9.8/cnvlib/smoothing.py` & `CNVkit-0.9.9/cnvlib/smoothing.py`

 * *Files 7% similar despite different names*

```diff
@@ -170,31 +170,45 @@
     Fitted polynomial order is typically much less than half the window width.
 
     `total_width` overrides `n_iter`.
     """
     if len(x) < 2:
         return x
 
-    if total_width:
-        n_iter = max(1, min(1000, total_width // window_width))
-    else:
+    # If the effective (total) window width is not specified explicitly, compute it.
+    if total_width is None:
         total_width = n_iter * window_width
-    logging.debug("Smoothing in %d iterations for effective bandwidth %d",
-                  n_iter, total_width)
 
-    # Apply signal smoothing
+    # Pad the signal.
     if weights is None:
         x, total_wing, signal = check_inputs(x, total_width, False)
+    else:
+        x, total_wing, signal, weights = check_inputs(x, total_width, False, weights)
+
+    # If the signal is short, the effective window length originally requested may not be possible. Because of this, we
+    # recalculate it given the actual wing length obtained.
+    total_width = 2 * total_wing + 1
+
+    # In case the signal is *very* short, the smoothing parameters will have to be adjusted as well.
+    window_width = min(window_width, total_width)
+    order = min(order, window_width // 2)
+
+    # Given the adjusted window widths (one-iteration and total), calculate the number of iterations we can do.
+    n_iter = max(1, min(1000, total_width // window_width))
+
+    # Apply signal smoothing.
+    logging.debug('Smoothing in {} iterations with window width {} and order {} for effective bandwidth {}'.format(
+        n_iter, window_width, order, total_width))
+    if weights is None:
         y = signal
         for _i in range(n_iter):
             y = savgol_filter(y, window_width, order, mode='interp')
         # y = convolve_unweighted(window, signal, wing)
     else:
         # TODO fit edges here, too
-        x, total_wing, signal, weights = check_inputs(x, total_width, False, weights)
         window = savgol_coeffs(window_width, order)
         y, w = convolve_weighted(window, signal, weights, n_iter)
     # Safety
     bad_idx = (y > x.max()) | (y < x.min())
     if bad_idx.any():
         logging.warning("Smoothing overshot at {} / {} indices: "
                         "({}, {}) vs. original ({}, {})"
```

### Comparing `CNVkit-0.9.8/cnvlib/target.py` & `CNVkit-0.9.9/cnvlib/target.py`

 * *Files identical despite different names*

### Comparing `CNVkit-0.9.8/cnvlib/vary.py` & `CNVkit-0.9.9/cnvlib/vary.py`

 * *Files identical despite different names*

### Comparing `CNVkit-0.9.8/scripts/cnv_annotate.py` & `CNVkit-0.9.9/scripts/cnv_annotate.py`

 * *Files identical despite different names*

### Comparing `CNVkit-0.9.8/scripts/cnv_expression_correlate.py` & `CNVkit-0.9.9/scripts/cnv_expression_correlate.py`

 * *Files identical despite different names*

### Comparing `CNVkit-0.9.8/scripts/cnv_updater.py` & `CNVkit-0.9.9/scripts/cnv_updater.py`

 * *Files identical despite different names*

### Comparing `CNVkit-0.9.8/scripts/guess_baits.py` & `CNVkit-0.9.9/scripts/guess_baits.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,15 +200,15 @@
                     help="""Filename to output average coverage depths in .cnn
                     format.""")
     AP.add_argument('-p', '--processes', metavar='CPU',
                     nargs='?', type=int, const=0, default=1,
                     help="""Number of subprocesses to segment in parallel.
                     If given without an argument, use the maximum number
                     of available CPUs. [Default: use 1 process]""")
-    P_coverage.add_argument('-f', '--fasta', metavar="FILENAME",
+    AP.add_argument('-f', '--fasta', metavar="FILENAME",
             help="Reference genome, FASTA format (e.g. UCSC hg19.fa)")
 
     AP_x = AP.add_mutually_exclusive_group(required=True)
     AP_x.add_argument('-t', '--targets', metavar='TARGET_BED',
                     help="""Potentially targeted genomic regions, e.g. all known
                     exons in the reference genome, in BED format. Each of these
                     regions will be tested as a whole for enrichment. (Faster
```

### Comparing `CNVkit-0.9.8/scripts/reference2targets.py` & `CNVkit-0.9.9/scripts/reference2targets.py`

 * *Files identical despite different names*

### Comparing `CNVkit-0.9.8/scripts/skg_convert.py` & `CNVkit-0.9.9/scripts/skg_convert.py`

 * *Files identical despite different names*

### Comparing `CNVkit-0.9.8/setup.py` & `CNVkit-0.9.9/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 #!/usr/bin/env python
 """Copy number variation toolkit for high-throughput sequencing."""
-import sys
+
 from os.path import dirname, join
 from glob import glob
 
 from setuptools import setup
 
 setup_args = {}
 
 # Dependencies for easy_install and pip:
-install_requires=[
-        'biopython >= 1.62',
-        'pomegranate >= 0.9.0',
-        'matplotlib >= 1.3.1',
-        'numpy >= 1.9',
-        'pandas >= 0.23.3',
-        'pyfaidx >= 0.4.7',
-        'pysam >= 0.10.0',
-        'reportlab >= 3.0',
-        'scikit-learn',
-        'scipy >= 0.15.0',
+install_requires = [
+    'biopython >= 1.62',
+    'matplotlib >= 1.3.1',
+    'numpy >= 1.9',
+    'pandas >= 0.23.3',
+    'pomegranate >= 0.9.0',
+    'pyfaidx >= 0.4.7',
+    'pysam >= 0.10.0',
+    'reportlab >= 3.0',
+    'scikit-learn',
+    'scipy >= 0.15.0',
+
+    # TODO: This is not a direct dependency of CNVkit. It is required for the correct operation of the `pomegranate`
+    # TODO: library in Python 3.9. Once the issue is resolved in `pomegranate`, this can be removed. See also
+    # TODO: https://github.com/etal/cnvkit/issues/606 and https://github.com/jmschrei/pomegranate/issues/909.
+    'networkx >= 2.4',
+    # TODO: Similarly: https://github.com/etal/cnvkit/issues/589
+    'joblib < 1.0',
 ]
 
 DIR = (dirname(__file__) or '.')
 with open(join(DIR, 'cnvlib', '_version.py')) as handle:
     VERSION = handle.readline().split('=')[-1].strip().replace('"','')
 
 setup_args.update(
```

### Comparing `CNVkit-0.9.8/skgenome/chromsort.py` & `CNVkit-0.9.9/skgenome/chromsort.py`

 * *Files identical despite different names*

### Comparing `CNVkit-0.9.8/skgenome/combiners.py` & `CNVkit-0.9.9/skgenome/combiners.py`

 * *Files identical despite different names*

### Comparing `CNVkit-0.9.8/skgenome/gary.py` & `CNVkit-0.9.9/skgenome/gary.py`

 * *Files identical despite different names*

### Comparing `CNVkit-0.9.8/skgenome/intersect.py` & `CNVkit-0.9.9/skgenome/intersect.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,18 @@
                 yield bin_row, subrange
         elif keep_empty:
             for bin_row in bin_rows.itertuples(index=False):
                 yield bin_row, []  # ENH: empty dframe matching table
 
 
 def by_shared_chroms(table, other, keep_empty=True):
-    if table['chromosome'].is_unique and other['chromosome'].is_unique:
+    # When both `table` and `other` contain only one chromosome each, and it's
+    # the same chromosome, we can just return the original tables.
+    table_chr, other_chr = set(table['chromosome']), set(other['chromosome'])
+    if len(table_chr) == 1 and table_chr == other_chr:
         yield table['chromosome'].iat[0], table, other
         # yield None, table, other
     else:
         other_chroms = {c: o for c, o in other.groupby(['chromosome'], sort=False)}
         for chrom, ctable in table.groupby(['chromosome'], sort=False):
             if chrom in other_chroms:
                 otable = other_chroms[chrom]
```

### Comparing `CNVkit-0.9.8/skgenome/merge.py` & `CNVkit-0.9.9/skgenome/merge.py`

 * *Files identical despite different names*

### Comparing `CNVkit-0.9.8/skgenome/rangelabel.py` & `CNVkit-0.9.9/skgenome/rangelabel.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 import collections
 import re
 
 Region = collections.namedtuple('Region', 'chromosome start end')
 NamedRegion = collections.namedtuple('NamedRegion', 'chromosome start end gene')
 
-re_label = re.compile(r'(\w+)?:(\d+)?-(\d+)?\s*(\S+)?')
+re_label = re.compile(r'(\w[\w.]*)?:(\d+)?-(\d+)?\s*(\S+)?')
 
 
 def from_label(text, keep_gene=True):
     """Parse a chromosomal range specification.
 
     Parameters
     ----------
```

### Comparing `CNVkit-0.9.8/skgenome/subdivide.py` & `CNVkit-0.9.9/skgenome/subdivide.py`

 * *Files identical despite different names*

### Comparing `CNVkit-0.9.8/skgenome/subtract.py` & `CNVkit-0.9.9/skgenome/subtract.py`

 * *Files identical despite different names*

### Comparing `CNVkit-0.9.8/skgenome/tabio/__init__.py` & `CNVkit-0.9.9/skgenome/tabio/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -217,15 +217,15 @@
         ext = ext.lstrip('.')
         # if ext in known_extensions:
         if ext[1:] in format_patterns:
             fname_fmt = ext[1:]
 
     # Fallback: regex detection
     # has_track = False
-    with as_handle(infile, 'rU') as handle:
+    with as_handle(infile, 'r') as handle:
         for line in handle:
             if not line.strip():
                 # Skip blank lines
                 continue
             if line.startswith('track'):
                 # NB: Could be UCSC BED or Ensembl GFF
                 # has_track = True
```

### Comparing `CNVkit-0.9.8/skgenome/tabio/bedio.py` & `CNVkit-0.9.9/skgenome/tabio/bedio.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             if not firstline.startswith("track"):
                 yield firstline
             for line in handle:
                 if line.startswith("track"):
                     break
                 yield line
 
-    with as_handle(infile, 'rU') as handle:
+    with as_handle(infile, 'r') as handle:
         rows = map(_parse_line, track2track(handle))
         return pd.DataFrame.from_records(rows, columns=["chromosome", "start",
                                                         "end", "gene", "strand"])
 
 
 def read_bed3(infile):
     """3-column BED format: chromosome, start, end."""
```

### Comparing `CNVkit-0.9.8/skgenome/tabio/genepred.py` & `CNVkit-0.9.9/skgenome/tabio/genepred.py`

 * *Files identical despite different names*

### Comparing `CNVkit-0.9.8/skgenome/tabio/gff.py` & `CNVkit-0.9.9/skgenome/tabio/gff.py`

 * *Files identical despite different names*

### Comparing `CNVkit-0.9.8/skgenome/tabio/picard.py` & `CNVkit-0.9.9/skgenome/tabio/picard.py`

 * *Files identical despite different names*

### Comparing `CNVkit-0.9.8/skgenome/tabio/seg.py` & `CNVkit-0.9.9/skgenome/tabio/seg.py`

 * *Files identical despite different names*

### Comparing `CNVkit-0.9.8/skgenome/tabio/seqdict.py` & `CNVkit-0.9.9/skgenome/tabio/seqdict.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import pandas as pd
 from Bio.File import as_handle
 
 
 def read_dict(infile):
     colnames = ["chromosome", "start", "end", # "file", "md5"
                ]
-    with as_handle(infile, 'rU') as handle:
+    with as_handle(infile, 'r') as handle:
         rows = _parse_lines(handle)
         return pd.DataFrame.from_records(rows, columns=colnames)
 
 
 def _parse_lines(lines):
     for line in lines:
         if line.startswith("@SQ"):
```

### Comparing `CNVkit-0.9.8/skgenome/tabio/tab.py` & `CNVkit-0.9.9/skgenome/tabio/tab.py`

 * *Files identical despite different names*

### Comparing `CNVkit-0.9.8/skgenome/tabio/textcoord.py` & `CNVkit-0.9.9/skgenome/tabio/textcoord.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     """Text coordinate format: "chr:start-end", one per line.
 
     Or sometimes: "chrom:start-end gene" or "chrom:start-end REF>ALT"
 
     Coordinate indexing is assumed to be from 1.
     """
     parse_line = report_bad_line(from_label)
-    with as_handle(infile, 'rU') as handle:
+    with as_handle(infile, 'r') as handle:
         rows = [parse_line(line) for line in handle]
     table = pd.DataFrame.from_records(rows, columns=["chromosome", "start",
                                                      "end", "gene"])
     table['gene'] = table['gene'].replace('', '-')
     return table
```

### Comparing `CNVkit-0.9.8/skgenome/tabio/vcfio.py` & `CNVkit-0.9.9/skgenome/tabio/vcfio.py`

 * *Files identical despite different names*

### Comparing `CNVkit-0.9.8/skgenome/tabio/vcfsimple.py` & `CNVkit-0.9.9/skgenome/tabio/vcfsimple.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 # TODO save VCF header (as string, the whole text block) in meta{header=}
 def read_vcf_simple(infile):
     """Read VCF file w/o samples."""
     # ENH: Make all readers return a tuple (header_string, body_table)
     # ENH: usecols -- need to trim dtypes dict to match?
     header_lines = []
-    with as_handle(infile, 'rU') as handle:
+    with as_handle(infile, 'r') as handle:
         for line in handle:
             if line.startswith('##'):
                 header_lines.append(line)
             else:
                 assert line.startswith('#CHR')
                 header_line = line
                 header_lines.append(line)
```

### Comparing `CNVkit-0.9.8/test/test_cnvlib.py` & `CNVkit-0.9.9/test/test_cnvlib.py`

 * *Files identical despite different names*

### Comparing `CNVkit-0.9.8/test/test_commands.py` & `CNVkit-0.9.9/test/test_commands.py`

 * *Files identical despite different names*

### Comparing `CNVkit-0.9.8/test/test_genome.py` & `CNVkit-0.9.9/test/test_genome.py`

 * *Files identical despite different names*

### Comparing `CNVkit-0.9.8/test/test_io.py` & `CNVkit-0.9.9/test/test_io.py`

 * *Files identical despite different names*

### Comparing `CNVkit-0.9.8/test/test_r.py` & `CNVkit-0.9.9/test/test_r.py`

 * *Files identical despite different names*

