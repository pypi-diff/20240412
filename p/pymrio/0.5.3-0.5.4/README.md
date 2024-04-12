# Comparing `tmp/pymrio-0.5.3.tar.gz` & `tmp/pymrio-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymrio-0.5.3.tar", last modified: Sat Oct 21 21:14:00 2023, max compression
+gzip compressed data, was "pymrio-0.5.4.tar", last modified: Fri Apr 12 10:48:01 2024, max compression
```

## Comparing `pymrio-0.5.3.tar` & `pymrio-0.5.4.tar`

### file list

```diff
@@ -1,159 +1,159 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 21:14:00.198257 pymrio-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)     7375 2023-10-21 21:13:15.000000 pymrio-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      154 2023-10-21 21:13:15.000000 pymrio-0.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9069 2023-10-21 21:14:00.198257 pymrio-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6343 2023-10-21 21:13:15.000000 pymrio-0.5.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 21:14:00.182257 pymrio-0.5.3/pymrio/
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 21:14:00.182257 pymrio-0.5.3/pymrio/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22836 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    33413 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/core/fileio.py
--rw-r--r--   0 runner    (1001) docker     (127)    92621 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/core/mriosystem.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 21:14:00.182257 pymrio-0.5.3/pymrio/mrio_models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 21:14:00.182257 pymrio-0.5.3/pymrio/mrio_models/exio2_ixi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_ixi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 21:14:00.186257 pymrio-0.5.3/pymrio/mrio_models/exio2_ixi/concordance/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_ixi/concordance/ALL.txt
--rw-r--r--   0 runner    (1001) docker     (127)      244 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_ixi/concordance/Africa.txt
--rw-r--r--   0 runner    (1001) docker     (127)      255 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_ixi/concordance/America.txt
--rw-r--r--   0 runner    (1001) docker     (127)      296 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_ixi/concordance/AsiaPacific.txt
--rw-r--r--   0 runner    (1001) docker     (127)      240 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_ixi/concordance/BRIC.txt
--rw-r--r--   0 runner    (1001) docker     (127)      330 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_ixi/concordance/EU.txt
--rw-r--r--   0 runner    (1001) docker     (127)      300 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_ixi/concordance/Europe.txt
--rw-r--r--   0 runner    (1001) docker     (127)      851 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_ixi/concordance/ISIC_A.txt
--rw-r--r--   0 runner    (1001) docker     (127)      817 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_ixi/concordance/ISIC_B.txt
--rw-r--r--   0 runner    (1001) docker     (127)      845 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_ixi/concordance/ISIC_C.txt
--rw-r--r--   0 runner    (1001) docker     (127)      937 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_ixi/concordance/ISIC_D.txt
--rw-r--r--   0 runner    (1001) docker     (127)      849 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_ixi/concordance/ISIC_E.txt
--rw-r--r--   0 runner    (1001) docker     (127)      819 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_ixi/concordance/ISIC_F.txt
--rw-r--r--   0 runner    (1001) docker     (127)      835 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_ixi/concordance/ISIC_G_H.txt
--rw-r--r--   0 runner    (1001) docker     (127)      831 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_ixi/concordance/ISIC_I.txt
--rw-r--r--   0 runner    (1001) docker     (127)      847 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_ixi/concordance/ISIC_J_K.txt
--rw-r--r--   0 runner    (1001) docker     (127)      819 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_ixi/concordance/ISIC_L.txt
--rw-r--r--   0 runner    (1001) docker     (127)      965 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_ixi/concordance/ISIC_M_N_O.txt
--rw-r--r--   0 runner    (1001) docker     (127)      817 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_ixi/concordance/ISIC_P.txt
--rw-r--r--   0 runner    (1001) docker     (127)      258 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_ixi/concordance/MiddleEast.txt
--rw-r--r--   0 runner    (1001) docker     (127)      240 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_ixi/concordance/OECD.txt
--rw-r--r--   0 runner    (1001) docker     (127)      235 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_ixi/concordance/RoW.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_ixi/concordance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_ixi/concordance/orig_regions.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_A.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_B.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_C.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_D.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_E.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_F.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_G_H.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_I.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_J_K.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_L.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_M_N_O.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_P.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 21:14:00.186257 pymrio-0.5.3/pymrio/mrio_models/exio2_ixi/misc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_ixi/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_ixi/misc/population.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 21:14:00.186257 pymrio-0.5.3/pymrio/mrio_models/exio2_pxp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_pxp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 21:14:00.190257 pymrio-0.5.3/pymrio/mrio_models/exio2_pxp/concordance/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_pxp/concordance/ALL.txt
--rw-r--r--   0 runner    (1001) docker     (127)      244 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_pxp/concordance/Africa.txt
--rw-r--r--   0 runner    (1001) docker     (127)      255 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_pxp/concordance/America.txt
--rw-r--r--   0 runner    (1001) docker     (127)      296 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_pxp/concordance/AsiaPacific.txt
--rw-r--r--   0 runner    (1001) docker     (127)      240 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_pxp/concordance/BRIC.txt
--rw-r--r--   0 runner    (1001) docker     (127)      330 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_pxp/concordance/EU.txt
--rw-r--r--   0 runner    (1001) docker     (127)      300 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_pxp/concordance/Europe.txt
--rw-r--r--   0 runner    (1001) docker     (127)      851 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_pxp/concordance/ISIC_A.txt
--rw-r--r--   0 runner    (1001) docker     (127)      817 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_pxp/concordance/ISIC_B.txt
--rw-r--r--   0 runner    (1001) docker     (127)      845 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_pxp/concordance/ISIC_C.txt
--rw-r--r--   0 runner    (1001) docker     (127)      937 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_pxp/concordance/ISIC_D.txt
--rw-r--r--   0 runner    (1001) docker     (127)      849 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_pxp/concordance/ISIC_E.txt
--rw-r--r--   0 runner    (1001) docker     (127)      819 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_pxp/concordance/ISIC_F.txt
--rw-r--r--   0 runner    (1001) docker     (127)      835 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_pxp/concordance/ISIC_G_H.txt
--rw-r--r--   0 runner    (1001) docker     (127)      831 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_pxp/concordance/ISIC_I.txt
--rw-r--r--   0 runner    (1001) docker     (127)      847 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_pxp/concordance/ISIC_J_K.txt
--rw-r--r--   0 runner    (1001) docker     (127)      819 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_pxp/concordance/ISIC_L.txt
--rw-r--r--   0 runner    (1001) docker     (127)      965 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_pxp/concordance/ISIC_M_N_O.txt
--rw-r--r--   0 runner    (1001) docker     (127)      817 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_pxp/concordance/ISIC_P.txt
--rw-r--r--   0 runner    (1001) docker     (127)      258 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_pxp/concordance/MiddleEast.txt
--rw-r--r--   0 runner    (1001) docker     (127)      240 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_pxp/concordance/OECD.txt
--rw-r--r--   0 runner    (1001) docker     (127)      235 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_pxp/concordance/RoW.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_pxp/concordance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_pxp/concordance/orig_regions.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_A.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_B.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_C.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_D.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_E.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_F.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_G_H.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_I.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_J_K.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_L.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_M_N_O.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_P.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 21:14:00.190257 pymrio-0.5.3/pymrio/mrio_models/exio2_pxp/misc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_pxp/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio2_pxp/misc/population.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 21:14:00.190257 pymrio-0.5.3/pymrio/mrio_models/exio3_ixi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio3_ixi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio3_ixi/finaldemand.tsv
--rw-r--r--   0 runner    (1001) docker     (127)    19783 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio3_ixi/sectors.tsv
--rw-r--r--   0 runner    (1001) docker     (127)      913 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio3_ixi/valueadded.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 21:14:00.194257 pymrio-0.5.3/pymrio/mrio_models/exio3_pxp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio3_pxp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio3_pxp/finaldemand.tsv
--rw-r--r--   0 runner    (1001) docker     (127)    14758 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio3_pxp/sectors.tsv
--rw-r--r--   0 runner    (1001) docker     (127)      913 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/exio3_pxp/valueadded.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 21:14:00.194257 pymrio-0.5.3/pymrio/mrio_models/test_mrio/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/test_mrio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 21:14:00.194257 pymrio-0.5.3/pymrio/mrio_models/test_mrio/concordance/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/test_mrio/concordance/EU.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/test_mrio/concordance/OECD.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/test_mrio/concordance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/test_mrio/concordance/emissions_charact.tsv
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/test_mrio/concordance/orig_regions.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/test_mrio/concordance/orig_sectors.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/test_mrio/concordance/sector1.txt
--rw-r--r--   0 runner    (1001) docker     (127)      122 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/test_mrio/concordance/sector2.txt
--rw-r--r--   0 runner    (1001) docker     (127)      122 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/test_mrio/concordance/sector3.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/test_mrio/concordance/supreg1.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/test_mrio/concordance/supreg2.txt
--rw-r--r--   0 runner    (1001) docker     (127)      369 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/test_mrio/finaldemand.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 21:14:00.194257 pymrio-0.5.3/pymrio/mrio_models/test_mrio/mrio_data/
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/test_mrio/mrio_data/FDemissions.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/test_mrio/mrio_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/test_mrio/mrio_data/emissions.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/test_mrio/mrio_data/factor_input.txt
--rw-r--r--   0 runner    (1001) docker     (127)    19990 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/test_mrio/mrio_data/finald_demand_Y.txt
--rw-r--r--   0 runner    (1001) docker     (127)      225 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/test_mrio/mrio_data/metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/test_mrio/mrio_data/population.txt
--rw-r--r--   0 runner    (1001) docker     (127)      180 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/test_mrio/mrio_data/readme.txt
--rw-r--r--   0 runner    (1001) docker     (127)    24805 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/test_mrio/mrio_data/trade_flows_Z.txt
--rw-r--r--   0 runner    (1001) docker     (127)      215 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/mrio_models/test_mrio/sectors.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 21:14:00.194257 pymrio-0.5.3/pymrio/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3071 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/tools/ioclass.py
--rw-r--r--   0 runner    (1001) docker     (127)    24975 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/tools/iodownloader.py
--rw-r--r--   0 runner    (1001) docker     (127)    14448 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/tools/iomath.py
--rw-r--r--   0 runner    (1001) docker     (127)    16201 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/tools/iometadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    67316 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/tools/ioparser.py
--rw-r--r--   0 runner    (1001) docker     (127)    21204 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/tools/ioutil.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-10-21 21:13:15.000000 pymrio-0.5.3/pymrio/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 21:14:00.182257 pymrio-0.5.3/pymrio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9069 2023-10-21 21:13:59.000000 pymrio-0.5.3/pymrio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6384 2023-10-21 21:14:00.000000 pymrio-0.5.3/pymrio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-21 21:13:59.000000 pymrio-0.5.3/pymrio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      134 2023-10-21 21:13:59.000000 pymrio-0.5.3/pymrio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-10-21 21:13:59.000000 pymrio-0.5.3/pymrio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-21 21:14:00.198257 pymrio-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2023-10-21 21:13:15.000000 pymrio-0.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 21:14:00.198257 pymrio-0.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8253 2023-10-21 21:13:15.000000 pymrio-0.5.3/tests/test_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (127)    15544 2023-10-21 21:13:15.000000 pymrio-0.5.3/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5672 2023-10-21 21:13:15.000000 pymrio-0.5.3/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    18874 2023-10-21 21:13:15.000000 pymrio-0.5.3/tests/test_math.py
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2023-10-21 21:13:15.000000 pymrio-0.5.3/tests/test_outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8270 2023-10-21 21:13:15.000000 pymrio-0.5.3/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8019 2023-10-21 21:13:15.000000 pymrio-0.5.3/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:48:01.789086 pymrio-0.5.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     7375 2024-04-12 10:47:35.000000 pymrio-0.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-12 10:47:35.000000 pymrio-0.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9069 2024-04-12 10:48:01.789086 pymrio-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6343 2024-04-12 10:47:35.000000 pymrio-0.5.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:48:01.773086 pymrio-0.5.4/pymrio/
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:48:01.773086 pymrio-0.5.4/pymrio/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22836 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33413 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/core/fileio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    93820 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/core/mriosystem.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:48:01.773086 pymrio-0.5.4/pymrio/mrio_models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:48:01.773086 pymrio-0.5.4/pymrio/mrio_models/exio2_ixi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_ixi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:48:01.777086 pymrio-0.5.4/pymrio/mrio_models/exio2_ixi/concordance/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_ixi/concordance/ALL.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_ixi/concordance/Africa.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_ixi/concordance/America.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_ixi/concordance/AsiaPacific.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_ixi/concordance/BRIC.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_ixi/concordance/EU.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_ixi/concordance/Europe.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_ixi/concordance/ISIC_A.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_ixi/concordance/ISIC_B.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_ixi/concordance/ISIC_C.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_ixi/concordance/ISIC_D.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_ixi/concordance/ISIC_E.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_ixi/concordance/ISIC_F.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_ixi/concordance/ISIC_G_H.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_ixi/concordance/ISIC_I.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_ixi/concordance/ISIC_J_K.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_ixi/concordance/ISIC_L.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_ixi/concordance/ISIC_M_N_O.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_ixi/concordance/ISIC_P.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_ixi/concordance/MiddleEast.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_ixi/concordance/OECD.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_ixi/concordance/RoW.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_ixi/concordance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_ixi/concordance/orig_regions.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_A.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_B.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_C.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_D.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_E.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_F.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_G_H.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_I.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_J_K.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_L.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_M_N_O.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_P.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:48:01.777086 pymrio-0.5.4/pymrio/mrio_models/exio2_ixi/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_ixi/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_ixi/misc/population.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:48:01.777086 pymrio-0.5.4/pymrio/mrio_models/exio2_pxp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_pxp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:48:01.785086 pymrio-0.5.4/pymrio/mrio_models/exio2_pxp/concordance/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_pxp/concordance/ALL.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_pxp/concordance/Africa.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_pxp/concordance/America.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_pxp/concordance/AsiaPacific.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_pxp/concordance/BRIC.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_pxp/concordance/EU.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_pxp/concordance/Europe.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_pxp/concordance/ISIC_A.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_pxp/concordance/ISIC_B.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_pxp/concordance/ISIC_C.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_pxp/concordance/ISIC_D.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_pxp/concordance/ISIC_E.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_pxp/concordance/ISIC_F.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_pxp/concordance/ISIC_G_H.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_pxp/concordance/ISIC_I.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_pxp/concordance/ISIC_J_K.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_pxp/concordance/ISIC_L.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_pxp/concordance/ISIC_M_N_O.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_pxp/concordance/ISIC_P.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_pxp/concordance/MiddleEast.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_pxp/concordance/OECD.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_pxp/concordance/RoW.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_pxp/concordance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_pxp/concordance/orig_regions.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_A.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_B.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_C.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_D.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_E.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_F.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_G_H.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_I.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_J_K.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_L.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_M_N_O.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_P.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:48:01.785086 pymrio-0.5.4/pymrio/mrio_models/exio2_pxp/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_pxp/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio2_pxp/misc/population.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:48:01.785086 pymrio-0.5.4/pymrio/mrio_models/exio3_ixi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio3_ixi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio3_ixi/finaldemand.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)    19783 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio3_ixi/sectors.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio3_ixi/valueadded.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:48:01.785086 pymrio-0.5.4/pymrio/mrio_models/exio3_pxp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio3_pxp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio3_pxp/finaldemand.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)    14758 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio3_pxp/sectors.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/exio3_pxp/valueadded.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:48:01.785086 pymrio-0.5.4/pymrio/mrio_models/test_mrio/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/test_mrio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:48:01.785086 pymrio-0.5.4/pymrio/mrio_models/test_mrio/concordance/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/test_mrio/concordance/EU.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/test_mrio/concordance/OECD.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/test_mrio/concordance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/test_mrio/concordance/emissions_charact.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/test_mrio/concordance/orig_regions.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/test_mrio/concordance/orig_sectors.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/test_mrio/concordance/sector1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/test_mrio/concordance/sector2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/test_mrio/concordance/sector3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/test_mrio/concordance/supreg1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/test_mrio/concordance/supreg2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/test_mrio/finaldemand.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:48:01.789086 pymrio-0.5.4/pymrio/mrio_models/test_mrio/mrio_data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/test_mrio/mrio_data/FDemissions.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/test_mrio/mrio_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/test_mrio/mrio_data/emissions.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/test_mrio/mrio_data/factor_input.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    19990 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/test_mrio/mrio_data/finald_demand_Y.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/test_mrio/mrio_data/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/test_mrio/mrio_data/population.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/test_mrio/mrio_data/readme.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    24805 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/test_mrio/mrio_data/trade_flows_Z.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/mrio_models/test_mrio/sectors.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:48:01.789086 pymrio-0.5.4/pymrio/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/tools/ioclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26346 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/tools/iodownloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18861 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/tools/iomath.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16201 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/tools/iometadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67599 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/tools/ioparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21205 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/tools/ioutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-12 10:47:35.000000 pymrio-0.5.4/pymrio/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:48:01.773086 pymrio-0.5.4/pymrio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9069 2024-04-12 10:48:01.000000 pymrio-0.5.4/pymrio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6384 2024-04-12 10:48:01.000000 pymrio-0.5.4/pymrio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 10:48:01.000000 pymrio-0.5.4/pymrio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-12 10:48:01.000000 pymrio-0.5.4/pymrio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 10:48:01.000000 pymrio-0.5.4/pymrio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 10:48:01.789086 pymrio-0.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-04-12 10:47:35.000000 pymrio-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:48:01.789086 pymrio-0.5.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-04-12 10:47:35.000000 pymrio-0.5.4/tests/test_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15544 2024-04-12 10:47:35.000000 pymrio-0.5.4/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5672 2024-04-12 10:47:35.000000 pymrio-0.5.4/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22799 2024-04-12 10:47:35.000000 pymrio-0.5.4/tests/test_math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-12 10:47:35.000000 pymrio-0.5.4/tests/test_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8270 2024-04-12 10:47:35.000000 pymrio-0.5.4/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8019 2024-04-12 10:47:35.000000 pymrio-0.5.4/tests/test_util.py
```

### Comparing `pymrio-0.5.3/LICENSE` & `pymrio-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pymrio-0.5.3/PKG-INFO` & `pymrio-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pymrio
-Version: 0.5.3
+Version: 0.5.4
 Summary: A python module for automating input output calculations and generating reports
 Home-page: https://github.com/IndEcol/pymrio
 Author: Konstantin Stadler
 Author-email: konstantin.stadler@ntnu.no
 License: UNKNOWN
 Description: ############
         Pymrio
```

### Comparing `pymrio-0.5.3/README.rst` & `pymrio-0.5.4/README.rst`

 * *Files identical despite different names*

### Comparing `pymrio-0.5.3/pymrio/__init__.py` & `pymrio-0.5.4/pymrio/__init__.py`

 * *Files identical despite different names*

### Comparing `pymrio-0.5.3/pymrio/core/constants.py` & `pymrio-0.5.4/pymrio/core/constants.py`

 * *Files identical despite different names*

### Comparing `pymrio-0.5.3/pymrio/core/fileio.py` & `pymrio-0.5.4/pymrio/core/fileio.py`

 * *Files identical despite different names*

### Comparing `pymrio-0.5.3/pymrio/core/mriosystem.py` & `pymrio-0.5.4/pymrio/core/mriosystem.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,19 +28,22 @@
     GENERIC_NAMES,
     MISSING_AGG_ENTRY,
     STORAGE_FORMAT,
 )
 from pymrio.tools.iomath import (
     calc_A,
     calc_accounts,
+    calc_As,
     calc_F,
     calc_F_Y,
+    calc_G,
     calc_gross_trade,
     calc_L,
     calc_M,
+    calc_M_down,
     calc_S,
     calc_S_Y,
     calc_x,
     calc_x_from_L,
     calc_Z,
     recalc_M,
 )
@@ -734,14 +737,16 @@
         Extension of final demand with columns a y and index as F
     S : pandas.DataFrame
         Direct impact (extensions) coefficients with multiindex as F
     S_Y : pandas.DataFrame
         Direct impact (extensions) coefficients of final demand. Index as F_Y
     M : pandas.DataFrame
         Multipliers with multiindex as F
+    M_down : pandas.DataFrame
+        Downstream multipliers with multiindex as F
     D_cba : pandas.DataFrame
         Footprint of consumption,  further specification with
         _reg (per region) or _cap (per capita) possible
     D_pba : pandas.DataFrame
         Territorial accounts, further specification with _reg (per region) or
         _cap (per capita) possible
     D_imp : pandas.DataFrame
@@ -772,28 +777,30 @@
         self,
         name,
         F=None,
         F_Y=None,
         S=None,
         S_Y=None,
         M=None,
+        M_down=None,
         D_cba=None,
         D_pba=None,
         D_imp=None,
         D_exp=None,
         unit=None,
         **kwargs,
     ):
         """Init function - see docstring class"""
         self.name = name
         self.F = F
         self.F_Y = F_Y
         self.S = S
         self.S_Y = S_Y
         self.M = M
+        self.M_down = M_down
         self.D_cba = D_cba
         self.D_pba = D_pba
         self.D_imp = D_imp
         self.D_exp = D_exp
         self.unit = unit
 
         for ext in kwargs:
@@ -838,25 +845,25 @@
         for acc in self.__D_accounts__:
             if acc not in self.__dict__:
                 setattr(self, acc, None)
 
     def __str__(self):
         return super().__str__("Extension {} with parameters: ").format(self.name)
 
-    def calc_system(self, x, Y, Y_agg=None, L=None, population=None):
+    def calc_system(self, x, Y, Y_agg=None, L=None, G=None, population=None):
         """Calculates the missing part of the extension plus accounts
 
         This method allows to specify an aggregated Y_agg for the
         account calculation (see Y_agg below). However, the full Y needs
         to be specified for the calculation of F_Y or S_Y.
 
         Calculates:
 
         - for each sector and country:
-            S, S_Y (if F_Y available), M, D_cba, D_pba_sector, D_imp_sector,
+            S, S_Y (if F_Y available), M, M_down, D_cba, D_pba_sector, D_imp_sector,
             D_exp_sector
         - for each region:
             D_cba_reg, D_pba_reg, D_imp_reg, D_exp_reg,
         - for each region (if population vector is given):
             D_cba_cap, D_pba_cap, D_imp_cap, D_exp_cap
 
         Notes
@@ -874,14 +881,17 @@
             The final demand aggregated (one category per country).  Can be
             used to restrict the calculation of CBA of a specific category
             (e.g. households). Default: y is aggregated over all categories
         L : pandas.DataFrame or numpy.array, optional
             Leontief input output table L. If this is not given,
             the method recalculates M based on D_cba (must be present in
             the extension).
+        G : pandas.DataFrame or numpy.array, optional
+            Ghosh input output table G. If this is not given,
+            M_down is not calculated.
         population : pandas.DataFrame or np.array, optional
             Row vector with population per region
         """
 
         # TODO: This should only be used for calculating the full system.
         # TODO There needs to be a new method for calculating the system for a different demand vector
 
@@ -923,14 +933,25 @@
                         "{} - M calculated based on " "D_cba and Y".format(self.name)
                     )
                 except Exception as ex:
                     logging.debug(
                         "Recalculation of M not possible - cause: {}".format(ex)
                     )
 
+        if self.M_down is None:
+            if G is not None:
+                self.M_down = calc_M_down(self.S, G)
+                logging.debug("{} - M_down calculated based on G".format(self.name))
+            else:
+                logging.debug(
+                    "Calculation of M_down not possible because G is not available.".format(
+                        self.name
+                    )
+                )
+
         F_Y_agg = 0
         if self.F_Y is not None:
             # F_Y_agg = ioutil.agg_columns(
             # ext['F_Y'], self.get_Y_categories().size)
             try:
                 F_Y_agg = self.F_Y.groupby(level="region", axis=1, sort=False).sum()
             except (AssertionError, KeyError):
@@ -1695,16 +1716,18 @@
     """
 
     def __init__(
         self,
         Z=None,
         Y=None,
         A=None,
+        As=None,
         x=None,
         L=None,
+        G=None,
         unit=None,
         population=None,
         system=None,
         version=None,
         year=None,
         price=None,
         meta=None,
@@ -1713,15 +1736,17 @@
         **kwargs,
     ):
         """Init function - see docstring class"""
         self.Z = Z
         self.Y = Y
         self.x = x
         self.A = A
+        self.As = As
         self.L = L
+        self.G = G
         self.unit = unit
         self.population = population
 
         if meta:
             self.meta = meta
             self.meta.change_meta("name", name)
             self.meta.change_meta("system", system)
@@ -1791,15 +1816,15 @@
         """
         return calc_gross_trade(Z=self.Z, Y=self.Y)
 
     def calc_all(self):
         """
         Calculates missing parts of the IOSystem and all extensions.
 
-        This method call calc_system and calc_extensions
+        This method calls calc_system and calc_extensions
 
         """
         self.calc_system()
         self.calc_extensions()
         return self
 
     def calc_system(self):
@@ -1838,18 +1863,26 @@
             self.x = calc_x(self.Z, self.Y)
             self.meta._add_modify("Industry output x calculated")
 
         if self.A is None:
             self.A = calc_A(self.Z, self.x)
             self.meta._add_modify("Coefficient matrix A calculated")
 
+        if self.As is None:
+            self.As = calc_As(self.Z, self.x)
+            self.meta._add_modify("Coefficient matrix As calculated")
+
         if self.L is None:
             self.L = calc_L(self.A)
             self.meta._add_modify("Leontief matrix L calculated")
 
+        if self.G is None:
+            self.G = calc_G(self.As)
+            self.meta._add_modify("Ghosh matrix G calculated")
+
         return self
 
     def calc_extensions(self, extensions=None, Y_agg=None):
         """Calculates the extension and their accounts
 
         For the calculation, y is aggregated across specified y categories
         The method calls .calc_system of each extension (or these given in the
@@ -1873,15 +1906,20 @@
 
         for ext_name in extensions:
             self.meta._add_modify(
                 "Calculating accounts for extension {}".format(ext_name)
             )
             ext = getattr(self, ext_name)
             ext.calc_system(
-                x=self.x, Y=self.Y, L=self.L, Y_agg=Y_agg, population=self.population
+                x=self.x,
+                Y=self.Y,
+                L=self.L,
+                G=self.G,
+                Y_agg=Y_agg,
+                population=self.population,
             )
         return self
 
     def report_accounts(
         self,
         path,
         per_region=True,
```

### Comparing `pymrio-0.5.3/pymrio/mrio_models/exio2_ixi/misc/population.txt` & `pymrio-0.5.4/pymrio/mrio_models/exio2_ixi/misc/population.txt`

 * *Files identical despite different names*

### Comparing `pymrio-0.5.3/pymrio/mrio_models/exio2_pxp/misc/population.txt` & `pymrio-0.5.4/pymrio/mrio_models/exio2_pxp/misc/population.txt`

 * *Files identical despite different names*

### Comparing `pymrio-0.5.3/pymrio/mrio_models/exio3_ixi/sectors.tsv` & `pymrio-0.5.4/pymrio/mrio_models/exio3_ixi/sectors.tsv`

 * *Files identical despite different names*

### Comparing `pymrio-0.5.3/pymrio/mrio_models/exio3_ixi/valueadded.tsv` & `pymrio-0.5.4/pymrio/mrio_models/exio3_ixi/valueadded.tsv`

 * *Files identical despite different names*

### Comparing `pymrio-0.5.3/pymrio/mrio_models/exio3_pxp/sectors.tsv` & `pymrio-0.5.4/pymrio/mrio_models/exio3_pxp/sectors.tsv`

 * *Files identical despite different names*

### Comparing `pymrio-0.5.3/pymrio/mrio_models/exio3_pxp/valueadded.tsv` & `pymrio-0.5.4/pymrio/mrio_models/exio3_pxp/valueadded.tsv`

 * *Files identical despite different names*

### Comparing `pymrio-0.5.3/pymrio/mrio_models/test_mrio/mrio_data/FDemissions.txt` & `pymrio-0.5.4/pymrio/mrio_models/test_mrio/mrio_data/FDemissions.txt`

 * *Files identical despite different names*

### Comparing `pymrio-0.5.3/pymrio/mrio_models/test_mrio/mrio_data/emissions.txt` & `pymrio-0.5.4/pymrio/mrio_models/test_mrio/mrio_data/emissions.txt`

 * *Files identical despite different names*

### Comparing `pymrio-0.5.3/pymrio/mrio_models/test_mrio/mrio_data/factor_input.txt` & `pymrio-0.5.4/pymrio/mrio_models/test_mrio/mrio_data/factor_input.txt`

 * *Files identical despite different names*

### Comparing `pymrio-0.5.3/pymrio/mrio_models/test_mrio/mrio_data/finald_demand_Y.txt` & `pymrio-0.5.4/pymrio/mrio_models/test_mrio/mrio_data/finald_demand_Y.txt`

 * *Files identical despite different names*

### Comparing `pymrio-0.5.3/pymrio/mrio_models/test_mrio/mrio_data/trade_flows_Z.txt` & `pymrio-0.5.4/pymrio/mrio_models/test_mrio/mrio_data/trade_flows_Z.txt`

 * *Files identical despite different names*

### Comparing `pymrio-0.5.3/pymrio/tools/ioclass.py` & `pymrio-0.5.4/pymrio/tools/ioclass.py`

 * *Files identical despite different names*

### Comparing `pymrio-0.5.3/pymrio/tools/iodownloader.py` & `pymrio-0.5.4/pymrio/tools/iodownloader.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,14 +88,21 @@
         "v2021": {
             "1995-1999": "https://stats.oecd.org/wbos/fileview2.aspx?IDFile=91d8e84b-7406-46b9-af5f-ec096242755c",
             "2000-2004": "https://stats.oecd.org/wbos/fileview2.aspx?IDFile=8adf89dd-18b4-40fe-bc7f-c822052eb961",
             "2005-2009": "https://stats.oecd.org/wbos/fileview2.aspx?IDFile=fe218690-0a3b-44aa-a82c-b3e3da6d24db",
             "2010-2014": "https://stats.oecd.org/wbos/fileview2.aspx?IDFile=2c2f499f-5703-4034-9457-2f7518e8f2fc",
             "2015-2018": "https://stats.oecd.org/wbos/fileview2.aspx?IDFile=59a3d7f2-3f23-40d5-95ca-48da84c0f861",
         },
+        "v2023": {
+            "1995-2000": "http://stats.oecd.org/wbos/fileview2.aspx?IDFile=d26ad811-5b58-4f0c-a4e3-06a1469e475c",
+            "2001-2005": "http://stats.oecd.org/wbos/fileview2.aspx?IDFile=7cb93dae-e491-4cfd-ac67-889eb7016a4a",
+            "2006-2010": "http://stats.oecd.org/wbos/fileview2.aspx?IDFile=ea165bfb-3a85-4e0a-afee-6ba8e6c16052",
+            "2011-2015": "http://stats.oecd.org/wbos/fileview2.aspx?IDFile=1f791bc6-befb-45c5-8b34-668d08a1702a",
+            "2016-2020": "http://stats.oecd.org/wbos/fileview2.aspx?IDFile=d1ab2315-298c-4e93-9a81-c6f2273139fe",
+        },
     },
 }
 
 GLORIA_CONFIG = {"datafiles": GLORIA_URLS}
 
 
 def _get_url_datafiles(
@@ -194,15 +201,15 @@
         downlog_handler._add_fileio("Downloaded {} to {}".format(url, filename))
         downlog_handler.save()
 
     return downlog_handler
 
 
 def download_oecd(
-    storage_folder, version="v2021", years=None, overwrite_existing=False
+    storage_folder, version="v2023", years=None, overwrite_existing=False
 ):
     """Downloads the OECD ICIO tables
 
     Parameters
     ----------
     storage_folder: str, valid path
         Location to store the download, folder will be created if
@@ -238,45 +245,43 @@
     # b/c the 2018 version is coded as aspx fileview property
     # in the html source - instead a hardcoded dict is used
     # to select the url for download
 
     os.makedirs(storage_folder, exist_ok=True)
 
     if type(version) is int:
-        version = str(version)
+        version = "v" + str(version)
 
-    if ("8" in version) or ("4" in version):
-        version = "v2018"
-    elif ("3" in version) or ("6" in version):
-        version = "v2016"
-    elif "21" in version:
-        version = "v2021"
-    else:
+    if not version in ("v2016", "v2018", "v2021", "v2023"):
         raise ValueError("Version not understood")
 
-    v2021_years = ["1995-1999", "2000-2004", "2005-2009", "2010-2014", "2015-2018"]
-
     if type(years) is int or type(years) is str:
         years = [years]
 
+    if version == "v2021":
+        bundle_years = ["1995-1999", "2000-2004", "2005-2009", "2010-2014", "2015-2018"]
+    elif version == "v2023":
+        bundle_years = ["1995-2000", "2001-2005", "2006-2010", "2011-2015", "2016-2020"]
+
     if not years:
         if version == "v2018":
             years = range(2005, 2016)
         elif version == "v2021":
-            years = v2021_years
-
+            years = bundle_years.copy()
+        elif version == "v2023":
+            years = bundle_years.copy()
         else:
             years = range(1995, 2012)
 
     years = [str(yy) for yy in years]
 
-    if version == "v2021":
+    if version == "v2021" or version == "v2023":
         for index, year in enumerate(years):
-            if year not in v2021_years:
-                for yr in v2021_years:
+            if year not in bundle_years:
+                for yr in bundle_years:
                     if int(yr[:4]) <= int(year) <= int(yr[-4:]):
                         years[index] = yr
 
     downlog = MRIOMetaData._make_download_log(
         location=storage_folder,
         description="OECD-ICIO download",
         name="OECD-ICIO",
@@ -294,28 +299,42 @@
             if version == "v2021":
                 filenames = [
                     f"ICIO{version.lstrip('v')}_{str(yr)}.csv"
                     for yr in range(int(yy[:4]), int(yy[-4:]) + 1)
                 ]
                 if set(filenames).issubset(os.listdir(storage_folder)):
                     continue
+            if version == "v2023":
+                filename = "ICIO-" + yy + "-extended.zip"
+                filenames = [f"{yr}.zip" for yr in range(int(yy[:4]), int(yy[-4:]) + 1)]
+
             elif filename in os.listdir(storage_folder):
                 continue
 
         req = ssl_fix(OECD_CONFIG["datafiles"][version][yy], stream=True)
         storage_file = os.path.join(storage_folder, filename)
 
         with open(storage_file, "wb") as lf:
             for chunk in req.iter_content(1024 * 5):
                 lf.write(chunk)
 
-        if version == "v2021":
+        if version == "v2021" or version == "v2023":
             with zipfile.ZipFile(storage_file, "r") as zip_ref:
                 zip_ref.extractall(storage_folder)
             os.remove(storage_file)
+            if version == "v2023":
+                for file in os.listdir(storage_folder):
+                    absolute_path = os.path.join(storage_folder, file)
+                    os.rename(
+                        os.path.join(storage_folder, file),
+                        os.path.join(
+                            storage_folder,
+                            "ICIO2023_" + file.replace("_SML", ""),
+                        ),
+                    )
 
         downlog._add_fileio(
             "Downloaded {} to {}".format(
                 OECD_CONFIG["datafiles"][version][yy], filename
             )
         )
```

### Comparing `pymrio-0.5.3/pymrio/tools/iomath.py` & `pymrio-0.5.4/pymrio/tools/iomath.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """ Mathematical functions for input output calculations
 
 All methods here should follow the functional programming paradigm
 
 Note
 ----
-To avoid namespace pollution everythin here starts with calc_
+To avoid namespace pollution everything here starts with calc_
 
 """
 
 import typing
 import warnings
 from collections import namedtuple
 
@@ -148,14 +148,58 @@
     # return Z.dot(np.diagflat(recix))
     if type(Z) is pd.DataFrame:
         return pd.DataFrame(Z.values * recix, index=Z.index, columns=Z.columns)
     else:
         return Z * recix
 
 
+def calc_As(Z, x):
+    """Calculate the As matrix (coefficients) from Z and x
+
+    As is a normalized version of the industrial flows of the transpose of Z, which quantifies the input to downstream
+    sectors.
+
+    Parameters
+    ----------
+    Z : pandas.DataFrame or numpy.array
+        Symmetric input output table (flows)
+    x : pandas.DataFrame or numpy.array
+        Industry output column vector
+
+    Returns
+    -------
+    pandas.DataFrame or numpy.array
+        Symmetric input output table (coefficients) As
+        The type is determined by the type of Z.
+        If DataFrame index/columns as Z
+
+    """
+    if (type(x) is pd.DataFrame) or (type(x) is pd.Series):
+        x = x.values
+    if (type(x) is not np.ndarray) and (x == 0):
+        recix = 0
+    else:
+        with warnings.catch_warnings():
+            # catch the divide by zero warning
+            # we deal wit that by setting to 0 afterwards
+            warnings.simplefilter("ignore")
+            recix = 1 / x
+        recix[recix == np.inf] = 0
+        recix = recix.reshape((1, -1))
+    # use numpy broadcasting - factor ten faster
+    # Mathematical form - slow
+    # return Z.dot(np.diagflat(recix))
+    if type(Z) is pd.DataFrame:
+        return pd.DataFrame(
+            np.transpose(Z.values) * recix, index=Z.index, columns=Z.columns
+        )
+    else:
+        return np.transpose(Z) * recix
+
+
 def calc_L(A):
     """Calculate the Leontief L from A
 
     L = inverse matrix of (I - A)
 
     Where I is an identity matrix of same shape as A
 
@@ -184,14 +228,73 @@
     I = np.eye(A.shape[0])  # noqa
     if type(A) is pd.DataFrame:
         return pd.DataFrame(np.linalg.inv(I - A), index=A.index, columns=A.columns)
     else:
         return np.linalg.inv(I - A)
 
 
+def calc_G(As, L=None, x=None):
+    """Calculate the Ghosh inverse matrix G either from As (high computation effor) or from Leontief matrix L and x
+    (low computation effort)
+
+    G = inverse matrix of (I - As) = hat(x)^{-1} *  L^T * hat(x)
+
+    where I is an identity matrix of same shape as As, and hat(x) is the diagonal matrix with values of x on the
+    diagonal.
+
+    Note that we define G as the transpose of the Ghosh inverse matrix, so that we can apply the factors of
+    production intensities from the left-hand-side for both Leontief and Ghosh attribution. In this way the
+    multipliers have the same (vector) dimensions and can be added.
+
+    Parameters
+    ----------
+    As : pandas.DataFrame or numpy.array
+        Symmetric input output table (coefficients)
+
+    Returns
+    -------
+    pandas.DataFrame or numpy.array
+        Ghosh input output table G
+        The type is determined by the type of As.
+        If DataFrame index/columns as As
+
+    """
+    # if L has already been calculated, then G can be derived from it with low computational cost.
+    if L is not None and x is not None:
+        if (type(x) is pd.DataFrame) or (type(x) is pd.Series):
+            x = x.values
+        if (type(x) is not np.ndarray) and (x == 0):
+            recix = 0
+        else:
+            with warnings.catch_warnings():
+                # catch the divide by zero warning
+                # we deal wit that by setting to 0 afterwards
+                warnings.simplefilter("ignore")
+                recix = 1 / x
+            recix[recix == np.inf] = 0
+            recix = recix.reshape((1, -1))
+
+        if type(L) is pd.DataFrame:
+            return pd.DataFrame(
+                recix * np.transpose(L.values * x), index=Z.index, columns=Z.columns
+            )
+        else:
+            # G = hat(x)^{-1} *  L^T * hat(x) in mathematical form np.linalg.inv(hatx).dot(L.transpose()).dot(hatx).
+            # it is computationally much faster to multiply element-wise because hatx is a diagonal matrix.
+            return recix * np.transpose(L * x)
+    else:  # calculation of the inverse of I-As has a high computational cost.
+        I = np.eye(As.shape[0])  # noqa
+        if type(As) is pd.DataFrame:
+            return pd.DataFrame(
+                np.linalg.inv(I - As), index=As.index, columns=As.columns
+            )
+        else:
+            return np.linalg.inv(I - As)  # G = inverse matrix of (I - As)
+
+
 def calc_S(F, x):
     """Calculate extensions/factor inputs coefficients
 
     Parameters
     ----------
     F : pandas.DataFrame or numpy.array
         Total direct impacts
@@ -304,21 +407,46 @@
     S : pandas.DataFrame or numpy.array
         Direct impact coefficients
 
     Returns
     -------
     pandas.DataFrame or numpy.array
         Multipliers M
-        The type is determined by the type of D.
-        If DataFrame index/columns as D
+        The type is determined by the type of S.
+        If DataFrame index/columns as S
 
     """
     return S.dot(L)
 
 
+def calc_M_down(S, G):
+    """Calculate downstream multipliers of the extensions
+
+    M_down = S * ( G - I )
+
+    Where I is an identity matrix of same shape as G
+
+    Parameters
+    ----------
+    G : pandas.DataFrame or numpy.array
+        Ghosh input output table G
+    S : pandas.DataFrame or numpy.array
+        Direct impact coefficients
+
+    Returns
+    -------
+    pandas.DataFrame or numpy.array
+        Downstream multipliers M
+        The type is determined by the type of S.
+        If DataFrame index/columns as S
+
+    """
+    return S.dot(G - np.eye(G.shape[0]))
+
+
 def calc_e(M, Y):
     """Calculate total impacts (footprints of consumption Y)
 
     Parameters
     ----------
     M : pandas.DataFrame or numpy.array
         Multipliers
@@ -329,15 +457,17 @@
 
     Returns
     -------
     pandas.DataFrame or numpy.array
         Multipliers m
         The type is determined by the type of M.
         If DataFrame index/columns as M
-    The calcubased on multipliers M and finald demand Y"""
+        The calculation is based on multipliers M and final demand Y
+
+    """
 
     return M.dot(Y)
 
 
 def recalc_M(S, D_cba, Y):
     """Calculate Multipliers based on footprints.
 
@@ -353,16 +483,14 @@
     Returns
     -------
 
     pandas.DataFrame or numpy.array
         Multipliers M
         The type is determined by the type of D_cba.
         If DataFrame index/columns as D_cba
-
-
     """
 
     Y_diag = ioutil.diagonalize_columns_to_sectors(Y)
     Y_inv = np.linalg.inv(Y_diag)
     M = D_cba.dot(Y_inv)
     if type(D_cba) is pd.DataFrame:
         M.columns = D_cba.columns
@@ -468,15 +596,14 @@
         A NamedTuple with two fields:
 
             - bilat_flows: df with rows: exporting country and sector,
               columns: importing countries
             - totals: df with gross total imports and exports per sector
               and region
 
-
     """
 
     Z_trade_blocks = ioutil.set_dom_block(Z, value=0)
     Y_trade_blocks = ioutil.set_dom_block(Y, value=0)
 
     level_spec_Z = "region" if "region" in Z.columns.names else 0
     level_spec_Y = "region" if "region" in Y.columns.names else 0
```

### Comparing `pymrio-0.5.3/pymrio/tools/iometadata.py` & `pymrio-0.5.4/pymrio/tools/iometadata.py`

 * *Files identical despite different names*

### Comparing `pymrio-0.5.3/pymrio/tools/ioparser.py` & `pymrio-0.5.4/pymrio/tools/ioparser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1531,15 +1531,15 @@
     FileNotFoundError
         If the specified data file could not be found.
 
     """
 
     path = os.path.abspath(os.path.normpath(str(path)))
 
-    oecd_file_starts = ["ICIO2016_", "ICIO2018_", "ICIO2021_"]
+    oecd_file_starts = ["ICIO2016_", "ICIO2018_", "ICIO2021_", "ICIO2023_"]
 
     # determine which oecd file to be parsed
     if not os.path.isdir(path):
         # 1. case - one file specified in path
         oecd_file = path
         path = os.path.split(oecd_file)[0]
     else:
@@ -1605,30 +1605,34 @@
     oecd_totals_col = ["TOTAL"]
     oecd_totals_row = ["OUT", "OUTPUT"]
 
     oecd_raw.drop(oecd_totals_col, axis=1, errors="ignore", inplace=True)
     oecd_raw.drop(oecd_totals_row, axis=0, errors="ignore", inplace=True)
 
     # Important - these must not match any country or industry name
-    factor_input = oecd_raw.filter(regex="VALU|TAX", axis=0)
+    factor_input_exact = oecd_raw.filter(items=["TLS", "VA"], axis=0)
+    factor_input_regex = oecd_raw.filter(regex="VALU|TAX", axis=0)
+    factor_input = pd.concat([factor_input_exact, factor_input_regex], axis=0)
     final_demand = oecd_raw.filter(
-        regex="HFCE|NPISH|NPS|GGFC|GFCF|INVNT|INV|DIRP|DPABR|FD|P33|DISC", axis=1
+        regex="HFCE|NPISH|NPS|GGFC|GFCF|INVNT|INV|DIRP|DPABR|FD|P33|DISC|OUT", axis=1
     )
 
     Z = oecd_raw.loc[
         oecd_raw.index.difference(factor_input.index),
         oecd_raw.columns.difference(final_demand.columns),
     ]
     F_factor_input = factor_input.loc[
         :, factor_input.columns.difference(final_demand.columns)
     ]
     F_Y_factor_input = factor_input.loc[:, final_demand.columns]
     Y = final_demand.loc[final_demand.index.difference(F_factor_input.index), :]
 
-    Z_index = pd.MultiIndex.from_tuples(tuple(ll) for ll in Z.index.str.split("_"))
+    Z_index = pd.MultiIndex.from_tuples(
+        tuple(ll) for ll in Z.index.map(lambda x: x.split("_", maxsplit=1))
+    )
     Z_columns = Z_index.copy()
     Z_index.names = IDX_NAMES["Z_row"]
     Z_columns.names = IDX_NAMES["Z_col"]
     Z.index = Z_index
     Z.columns = Z_columns
 
     _midx = []
@@ -1867,24 +1871,26 @@
                     indices_file = zipfile.ZipFile(indices_loc)
                 except:
                     raise ValueError(
                         f"{filename} is not available in the zip file and no indices.zip file is available in the directory provided"
                     )
 
         eora_data = {
-            key: pd.read_csv(
-                zip_file.open(filename),
-                sep=eora_sep,
-                header=None,
-            )
-            if filename in zip_file.namelist()
-            else pd.read_csv(
-                indices_file.open(filename),
-                sep=eora_sep,
-                header=None,
+            key: (
+                pd.read_csv(
+                    zip_file.open(filename),
+                    sep=eora_sep,
+                    header=None,
+                )
+                if filename in zip_file.namelist()
+                else pd.read_csv(
+                    indices_file.open(filename),
+                    sep=eora_sep,
+                    header=None,
+                )
             )
             for key, filename in eora_files.items()
         }
         zip_file.close()
     else:
         eora_data = {
             key: pd.read_csv(
```

### Comparing `pymrio-0.5.3/pymrio/tools/ioutil.py` & `pymrio-0.5.4/pymrio/tools/ioutil.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Utility function for pymrio
 
 KST 20140502
 """
+
 import json
 import logging
 import os
 import re
 import ssl
 import zipfile
 from collections import namedtuple
```

### Comparing `pymrio-0.5.3/pymrio.egg-info/PKG-INFO` & `pymrio-0.5.4/pymrio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pymrio
-Version: 0.5.3
+Version: 0.5.4
 Summary: A python module for automating input output calculations and generating reports
 Home-page: https://github.com/IndEcol/pymrio
 Author: Konstantin Stadler
 Author-email: konstantin.stadler@ntnu.no
 License: UNKNOWN
 Description: ############
         Pymrio
```

### Comparing `pymrio-0.5.3/pymrio.egg-info/SOURCES.txt` & `pymrio-0.5.4/pymrio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymrio-0.5.3/setup.py` & `pymrio-0.5.4/setup.py`

 * *Files identical despite different names*

### Comparing `pymrio-0.5.3/tests/test_aggregation.py` & `pymrio-0.5.4/tests/test_aggregation.py`

 * *Files identical despite different names*

### Comparing `pymrio-0.5.3/tests/test_core.py` & `pymrio-0.5.4/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `pymrio-0.5.3/tests/test_integration.py` & `pymrio-0.5.4/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `pymrio-0.5.3/tests/test_math.py` & `pymrio-0.5.4/tests/test_math.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,20 +12,23 @@
 TESTPATH = os.path.dirname(os.path.abspath(__file__))
 sys.path.append(os.path.join(TESTPATH, ".."))
 
 
 # the function which should be tested here
 from pymrio.tools.iomath import calc_A  # noqa
 from pymrio.tools.iomath import calc_accounts  # noqa
+from pymrio.tools.iomath import calc_As  # noqa
 from pymrio.tools.iomath import calc_e  # noqa
 from pymrio.tools.iomath import calc_F  # noqa
 from pymrio.tools.iomath import calc_F_Y  # noqa
+from pymrio.tools.iomath import calc_G  # noqa
 from pymrio.tools.iomath import calc_gross_trade  # noqa
 from pymrio.tools.iomath import calc_L  # noqa
 from pymrio.tools.iomath import calc_M  # noqa
+from pymrio.tools.iomath import calc_M_down  # noqa
 from pymrio.tools.iomath import calc_S  # noqa
 from pymrio.tools.iomath import calc_S_Y  # noqa
 from pymrio.tools.iomath import calc_x  # noqa
 from pymrio.tools.iomath import calc_x_from_L  # noqa
 from pymrio.tools.iomath import calc_Z  # noqa
 
 
@@ -228,14 +231,34 @@
                     0.2564102564102564,
                 ],  # noqa
             ],
             index=_Z_multiindex,
             columns=_Z_multiindex,
         )
 
+        As = pd.DataFrame(
+            data=[
+                [0.19607843, 0.0, 0.17241379, 0.1, 0.0, 0.12820513],  # noqa
+                [0.09803922, 0.13333333, 0.05172414, 0.0, 0.19230769, 0.0],  # noqa
+                [0.01960784, 0.0, 0.34482759, 0.0, 0.01923077, 0.0],  # noqa
+                [0.11764706, 0.0, 0.06896552, 0.02, 0.0, 0.02564103],  # noqa
+                [
+                    0.09803922,
+                    0.33333333,
+                    0.03448276,
+                    0.2,
+                    0.38461538,
+                    0.25641026,
+                ],  # noqa
+                [0.1372549, 0.2, 0.0, 0.18, 0.01923077, 0.25641026],  # noqa
+            ],
+            index=_Z_multiindex,
+            columns=_Z_multiindex,
+        )
+
         L = pd.DataFrame(
             data=[
                 [
                     1.3387146304736708,
                     0.9689762471208287,
                     0.05036622549592462,
                     0.17820960407435948,
@@ -283,14 +306,69 @@
                     1.4849251515157111,
                 ],  # noqa
             ],
             index=_Z_multiindex,
             columns=_Z_multiindex,
         )
 
+        G = pd.DataFrame(
+            data=[
+                [
+                    1.33871463,
+                    0.07482651,
+                    0.38065717,
+                    0.19175489,
+                    0.04316348,
+                    0.25230906,
+                ],  # noqa
+                [
+                    0.28499301,
+                    1.37164729,
+                    0.22311379,
+                    0.15732254,
+                    0.44208094,
+                    0.20700334,
+                ],  # noqa
+                [
+                    0.05727924,
+                    0.02969614,
+                    1.54929428,
+                    0.02349465,
+                    0.05866155,
+                    0.03091401,
+                ],  # noqa
+                [
+                    0.1747153,
+                    0.02185805,
+                    0.15941084,
+                    1.05420074,
+                    0.01404088,
+                    0.07131676,
+                ],  # noqa
+                [
+                    0.58648041,
+                    0.93542302,
+                    0.39473223,
+                    0.60492361,
+                    1.95452858,
+                    0.79595212,
+                ],  # noqa
+                [
+                    0.38121958,
+                    0.41222074,
+                    0.17907022,
+                    0.34854312,
+                    0.18081884,
+                    1.48492515,
+                ],  # noqa
+            ],
+            index=_Z_multiindex,
+            columns=_Z_multiindex,
+        )
+
         x = pd.DataFrame(
             data=[
                 [51],
                 [15],
                 [58],
                 [50],
                 [52],
@@ -342,14 +420,37 @@
                     0.6031791628984159,
                 ],  # noqa
             ],
             index=["ext_type_1", "ext_type_2"],
             columns=_Z_multiindex,
         )
 
+        M_down = pd.DataFrame(
+            data=[
+                [
+                    0.48172779,
+                    0.48999986,
+                    0.74944707,
+                    0.38438353,
+                    0.48030952,
+                    0.50914162,
+                ],  # noqa
+                [
+                    0.26832875,
+                    0.25724662,
+                    0.28759602,
+                    0.18651650,
+                    0.21856841,
+                    0.25216408,
+                ],  # noqa
+            ],
+            index=["ext_type_1", "ext_type_2"],
+            columns=_Z_multiindex,
+        )
+
         D_cba = pd.DataFrame(
             data=[
                 [
                     14.059498889254174,
                     18.863255551508175,
                     17.32012296814962,
                     8.71616437964097,
@@ -532,14 +633,25 @@
     x_Tvalues = td_small_MRIO.x.T.values
     x_series = pd.Series(td_small_MRIO.x.iloc[:, 0])
     pdt.assert_frame_equal(td_small_MRIO.A, calc_A(td_small_MRIO.Z, x_series))
     pdt.assert_frame_equal(td_small_MRIO.A, calc_A(td_small_MRIO.Z, x_values))
     pdt.assert_frame_equal(td_small_MRIO.A, calc_A(td_small_MRIO.Z, x_Tvalues))
 
 
+def test_calc_As_MRIO(td_small_MRIO):
+    pdt.assert_frame_equal(td_small_MRIO.As, calc_As(td_small_MRIO.Z, td_small_MRIO.x))
+    # we also test the different methods to provide x:
+    x_values = td_small_MRIO.x.values
+    x_Tvalues = td_small_MRIO.x.T.values
+    x_series = pd.Series(td_small_MRIO.x.iloc[:, 0])
+    pdt.assert_frame_equal(td_small_MRIO.As, calc_As(td_small_MRIO.Z, x_series))
+    pdt.assert_frame_equal(td_small_MRIO.As, calc_As(td_small_MRIO.Z, x_values))
+    pdt.assert_frame_equal(td_small_MRIO.As, calc_As(td_small_MRIO.Z, x_Tvalues))
+
+
 def test_calc_Z_MRIO(td_small_MRIO):
     pdt.assert_frame_equal(td_small_MRIO.Z, calc_Z(td_small_MRIO.A, td_small_MRIO.x))
     # we also test the different methods to provide x:
     x_values = td_small_MRIO.x.values
     x_Tvalues = td_small_MRIO.x.T.values
     x_series = pd.Series(td_small_MRIO.x.iloc[:, 0])
     pdt.assert_frame_equal(td_small_MRIO.Z, calc_Z(td_small_MRIO.A, x_series))
@@ -547,14 +659,18 @@
     pdt.assert_frame_equal(td_small_MRIO.Z, calc_Z(td_small_MRIO.A, x_Tvalues))
 
 
 def test_calc_L_MRIO(td_small_MRIO):
     pdt.assert_frame_equal(td_small_MRIO.L, calc_L(td_small_MRIO.A))
 
 
+def test_calc_G_MRIO(td_small_MRIO):
+    pdt.assert_frame_equal(td_small_MRIO.G, calc_G(td_small_MRIO.As))
+
+
 def test_calc_S_MRIO(td_small_MRIO):
     pdt.assert_frame_equal(td_small_MRIO.S, calc_S(td_small_MRIO.F, td_small_MRIO.x))
 
 
 def test_calc_S_Y_MRIO(td_small_MRIO):
     pdt.assert_frame_equal(
         td_small_MRIO.S_Y, calc_S_Y(td_small_MRIO.F_Y, td_small_MRIO.Y.sum(axis=0))
@@ -568,14 +684,20 @@
     )
 
 
 def test_calc_M_MRIO(td_small_MRIO):
     pdt.assert_frame_equal(td_small_MRIO.M, calc_M(td_small_MRIO.S, td_small_MRIO.L))
 
 
+def test_calc_M_down_MRIO(td_small_MRIO):
+    pdt.assert_frame_equal(
+        td_small_MRIO.M_down, calc_M_down(td_small_MRIO.S, td_small_MRIO.G)
+    )
+
+
 def test_calc_gross_trade_MRIO(td_small_MRIO):
     gt = calc_gross_trade(td_small_MRIO.Z, td_small_MRIO.Y)
 
     reg1sec2trade = (
         td_small_MRIO.Z.loc[("reg1", "sector2"), "reg2"].sum()
         + td_small_MRIO.Y.loc[("reg1", "sector2"), "reg2"].sum()
     )
```

### Comparing `pymrio-0.5.3/tests/test_outputs.py` & `pymrio-0.5.4/tests/test_outputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,14 @@
     for testing. Regression tests against plotted graphs,
     as provided by image_comparison decorator of matplotlib,
     are not used since this is deprecated and also not consistent
     across different plotting engines.
 
 """
 
-
 import os
 import sys
 
 import pytest
 
 TESTPATH = os.path.dirname(os.path.abspath(__file__))
 sys.path.append(os.path.join(TESTPATH, ".."))
```

### Comparing `pymrio-0.5.3/tests/test_parsers.py` & `pymrio-0.5.4/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `pymrio-0.5.3/tests/test_util.py` & `pymrio-0.5.4/tests/test_util.py`

 * *Files identical despite different names*

