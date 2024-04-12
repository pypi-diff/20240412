# Comparing `tmp/cubids-1.0.9.tar.gz` & `tmp/cubids-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubids-1.0.9.tar", last modified: Mon Jul 31 06:47:31 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `cubids-1.0.9.tar` & `cubids-1.1.0.tar`

### file list

```diff
@@ -1,286 +1,269 @@
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.479490 cubids-1.0.9/
--rw-r--r--   0 scovitz    (502) staff       (20)      409 2023-05-04 11:48:08.000000 cubids-1.0.9/AUTHORS.rst
--rw-r--r--   0 scovitz    (502) staff       (20)     3508 2023-06-05 12:52:08.000000 cubids-1.0.9/CONTRIBUTING.rst
--rw-r--r--   0 scovitz    (502) staff       (20)       89 2023-05-04 11:48:08.000000 cubids-1.0.9/HISTORY.rst
--rw-r--r--   0 scovitz    (502) staff       (20)     1102 2023-05-04 11:48:08.000000 cubids-1.0.9/LICENSE
--rw-r--r--   0 scovitz    (502) staff       (20)      298 2023-05-04 11:48:08.000000 cubids-1.0.9/MANIFEST.in
--rw-r--r--   0 scovitz    (502) staff       (20)     2428 2023-07-31 06:47:31.479580 cubids-1.0.9/PKG-INFO
--rw-r--r--   0 scovitz    (502) staff       (20)     1546 2023-05-04 11:48:08.000000 cubids-1.0.9/README.rst
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.436551 cubids-1.0.9/cubids/
--rw-r--r--   0 scovitz    (502) staff       (20)      148 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/__init__.py
--rw-r--r--   0 scovitz    (502) staff       (20)    39368 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/cli.py
--rw-r--r--   0 scovitz    (502) staff       (20)      423 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/config.py
--rw-r--r--   0 scovitz    (502) staff       (20)      711 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/constants.py
--rw-r--r--   0 scovitz    (502) staff       (20)    62321 2023-06-05 12:53:20.000000 cubids-1.0.9/cubids/cubids.py
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.437586 cubids-1.0.9/cubids/data/
--rw-r--r--   0 scovitz    (502) staff       (20)    10942 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/data/config.yml
--rw-r--r--   0 scovitz    (502) staff       (20)     9908 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/metadata_merge.py
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.437703 cubids-1.0.9/cubids/testdata/
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.437986 cubids-1.0.9/cubids/testdata/BIDS_Dataset/
--rw-r--r--   0 scovitz    (502) staff       (20)      368 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/README
--rw-r--r--   0 scovitz    (502) staff       (20)      189 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/dataset_description.json
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.428965 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.429232 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.438233 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/anat/
--rw-r--r--   0 scovitz    (502) staff       (20)     1067 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/anat/sub-01_ses-phdiff_T1w.json
--rw-r--r--   0 scovitz    (502) staff       (20)   123172 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/anat/sub-01_ses-phdiff_T1w.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.438771 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/dwi/
--rw-r--r--   0 scovitz    (502) staff       (20)       44 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.bval
--rw-r--r--   0 scovitz    (502) staff       (20)      245 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.bvec
--rw-r--r--   0 scovitz    (502) staff       (20)     2011 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.json
--rw-r--r--   0 scovitz    (502) staff       (20)     6084 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.439710 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/fmap/
--rw-r--r--   0 scovitz    (502) staff       (20)     1675 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude1.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2107 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude1.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     1698 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude2.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2107 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude2.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     1787 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_phasediff.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2106 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_phasediff.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     2106 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_dir-PA_epi.json
--rw-r--r--   0 scovitz    (502) staff       (20)     1502 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_dir-PA_epi.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.439957 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/func/
--rw-r--r--   0 scovitz    (502) staff       (20)     2234 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/func/sub-01_ses-phdiff_task-rest_bold.json
--rw-r--r--   0 scovitz    (502) staff       (20)    30889 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/func/sub-01_ses-phdiff_task-rest_bold.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.429355 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.429623 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.440253 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/anat/
--rw-r--r--   0 scovitz    (502) staff       (20)     1036 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/anat/sub-02_ses-phdiff_T1w.json
--rw-r--r--   0 scovitz    (502) staff       (20)   123172 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/anat/sub-02_ses-phdiff_T1w.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.440791 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/dwi/
--rw-r--r--   0 scovitz    (502) staff       (20)      283 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.bval
--rw-r--r--   0 scovitz    (502) staff       (20)     1685 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.bvec
--rw-r--r--   0 scovitz    (502) staff       (20)     2042 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.json
--rw-r--r--   0 scovitz    (502) staff       (20)    30889 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.441801 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/fmap/
--rw-r--r--   0 scovitz    (502) staff       (20)     1675 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude1.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2107 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude1.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     1698 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude2.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2107 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude2.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     1787 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_phasediff.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2106 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_phasediff.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     2012 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_dir-PA_epi.json
--rw-r--r--   0 scovitz    (502) staff       (20)     1502 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_dir-PA_epi.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.442044 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/func/
--rw-r--r--   0 scovitz    (502) staff       (20)     2168 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/func/sub-02_ses-phdiff_task-rest_bold.json
--rw-r--r--   0 scovitz    (502) staff       (20)    30889 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/func/sub-02_ses-phdiff_task-rest_bold.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.429751 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.430012 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.442298 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/anat/
--rw-r--r--   0 scovitz    (502) staff       (20)     1036 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/anat/sub-03_ses-phdiff_T1w.json
--rw-r--r--   0 scovitz    (502) staff       (20)   123172 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/anat/sub-03_ses-phdiff_T1w.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.442841 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/dwi/
--rw-r--r--   0 scovitz    (502) staff       (20)      283 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.bval
--rw-r--r--   0 scovitz    (502) staff       (20)     1685 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.bvec
--rw-r--r--   0 scovitz    (502) staff       (20)     1975 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.json
--rw-r--r--   0 scovitz    (502) staff       (20)    30889 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.443814 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/fmap/
--rw-r--r--   0 scovitz    (502) staff       (20)     1675 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude1.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2107 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude1.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     1698 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude2.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2107 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude2.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     1787 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_phasediff.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2106 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_phasediff.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     2106 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_dir-PA_epi.json
--rw-r--r--   0 scovitz    (502) staff       (20)     1502 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_dir-PA_epi.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.444053 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/func/
--rw-r--r--   0 scovitz    (502) staff       (20)     2202 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/func/sub-03_ses-phdiff_task-rest_bold.json
--rw-r--r--   0 scovitz    (502) staff       (20)    30889 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/func/sub-03_ses-phdiff_task-rest_bold.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.430132 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.430392 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.444306 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/anat/
--rw-r--r--   0 scovitz    (502) staff       (20)     1036 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/anat/sub-04_ses-phdiff_T1w.json
--rw-r--r--   0 scovitz    (502) staff       (20)   123172 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/anat/sub-04_ses-phdiff_T1w.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.444884 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/dwi/
--rw-r--r--   0 scovitz    (502) staff       (20)      283 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/dwi/sub-04_ses-phdiff_acq-HASC55AP_dwi.bval
--rw-r--r--   0 scovitz    (502) staff       (20)     1685 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/dwi/sub-04_ses-phdiff_acq-HASC55AP_dwi.bvec
--rw-r--r--   0 scovitz    (502) staff       (20)     2007 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/dwi/sub-04_ses-phdiff_acq-HASC55AP_dwi.json
--rw-r--r--   0 scovitz    (502) staff       (20)    30889 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/dwi/sub-04_ses-phdiff_acq-HASC55AP_dwi.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.445847 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/fmap/
--rw-r--r--   0 scovitz    (502) staff       (20)     1675 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_acq-v4_magnitude1.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2107 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_acq-v4_magnitude1.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     1698 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_acq-v4_magnitude2.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2107 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_acq-v4_magnitude2.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     1787 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_acq-v4_phasediff.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2106 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_acq-v4_phasediff.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     2106 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_dir-PA_epi.json
--rw-r--r--   0 scovitz    (502) staff       (20)     1502 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_dir-PA_epi.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.446087 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/func/
--rw-r--r--   0 scovitz    (502) staff       (20)     2202 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/func/sub-04_ses-phdiff_task-rest_bold.json
--rw-r--r--   0 scovitz    (502) staff       (20)    30889 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/func/sub-04_ses-phdiff_task-rest_bold.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)    69774 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/BIDS_Dataset.zip
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.446332 cubids-1.0.9/cubids/testdata/complete/
--rw-r--r--   0 scovitz    (502) staff       (20)       73 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/README
--rw-r--r--   0 scovitz    (502) staff       (20)      189 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/dataset_description.json
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.430589 cubids-1.0.9/cubids/testdata/complete/sub-01/
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.430850 cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.446563 cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/anat/
--rw-r--r--   0 scovitz    (502) staff       (20)      963 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/anat/sub-01_ses-phdiff_T1w.json
--rw-r--r--   0 scovitz    (502) staff       (20)   123172 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/anat/sub-01_ses-phdiff_T1w.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.447103 cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/dwi/
--rw-r--r--   0 scovitz    (502) staff       (20)      283 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.bval
--rw-r--r--   0 scovitz    (502) staff       (20)     1685 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.bvec
--rw-r--r--   0 scovitz    (502) staff       (20)     1780 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.json
--rw-r--r--   0 scovitz    (502) staff       (20)    30889 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.449349 cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/fmap/
--rw-r--r--   0 scovitz    (502) staff       (20)     1508 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude1.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2107 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude1.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     1529 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude2.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2107 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude2.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     1604 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_phasediff.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2106 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_phasediff.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     1867 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_dir-PA_epi.json
--rw-r--r--   0 scovitz    (502) staff       (20)     1502 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_dir-PA_epi.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.449792 cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/func/
--rw-r--r--   0 scovitz    (502) staff       (20)     1970 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/func/sub-01_ses-phdiff_task-rest_bold.json
--rw-r--r--   0 scovitz    (502) staff       (20)    30889 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/func/sub-01_ses-phdiff_task-rest_bold.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.430971 cubids-1.0.9/cubids/testdata/complete/sub-02/
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.431246 cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.450186 cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/anat/
--rw-r--r--   0 scovitz    (502) staff       (20)      963 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/anat/sub-02_ses-phdiff_T1w.json
--rw-r--r--   0 scovitz    (502) staff       (20)   123172 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/anat/sub-02_ses-phdiff_T1w.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.451000 cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/dwi/
--rw-r--r--   0 scovitz    (502) staff       (20)      283 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.bval
--rw-r--r--   0 scovitz    (502) staff       (20)     1685 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.bvec
--rw-r--r--   0 scovitz    (502) staff       (20)     1780 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.json
--rw-r--r--   0 scovitz    (502) staff       (20)    30889 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.452605 cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/fmap/
--rw-r--r--   0 scovitz    (502) staff       (20)     1508 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude1.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2107 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude1.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     1529 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude2.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2107 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude2.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     1610 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_phasediff.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2106 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_phasediff.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     1867 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_dir-PA_epi.json
--rw-r--r--   0 scovitz    (502) staff       (20)     1502 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_dir-PA_epi.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.452952 cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/func/
--rw-r--r--   0 scovitz    (502) staff       (20)     1970 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/func/sub-02_ses-phdiff_task-rest_bold.json
--rw-r--r--   0 scovitz    (502) staff       (20)    30889 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/func/sub-02_ses-phdiff_task-rest_bold.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.431394 cubids-1.0.9/cubids/testdata/complete/sub-03/
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.431782 cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.453314 cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/anat/
--rw-r--r--   0 scovitz    (502) staff       (20)      963 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/anat/sub-03_ses-phdiff_T1w.json
--rw-r--r--   0 scovitz    (502) staff       (20)   123172 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/anat/sub-03_ses-phdiff_T1w.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.454075 cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/dwi/
--rw-r--r--   0 scovitz    (502) staff       (20)      283 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.bval
--rw-r--r--   0 scovitz    (502) staff       (20)     1685 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.bvec
--rw-r--r--   0 scovitz    (502) staff       (20)     1780 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.json
--rw-r--r--   0 scovitz    (502) staff       (20)    30889 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.455740 cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/fmap/
--rw-r--r--   0 scovitz    (502) staff       (20)     1508 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude1.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2107 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude1.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     1529 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude2.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2107 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude2.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     1610 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_phasediff.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2106 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_phasediff.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     1867 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_dir-PA_epi.json
--rw-r--r--   0 scovitz    (502) staff       (20)     1502 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_dir-PA_epi.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.456291 cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/func/
--rw-r--r--   0 scovitz    (502) staff       (20)     1970 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/func/sub-03_ses-phdiff_task-rest_bold.json
--rw-r--r--   0 scovitz    (502) staff       (20)    30889 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/func/sub-03_ses-phdiff_task-rest_bold.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.456698 cubids-1.0.9/cubids/testdata/inconsistent/
--rw-r--r--   0 scovitz    (502) staff       (20)      368 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/README
--rw-r--r--   0 scovitz    (502) staff       (20)      189 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/dataset_description.json
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.431989 cubids-1.0.9/cubids/testdata/inconsistent/sub-01/
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.432260 cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.457140 cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/anat/
--rw-r--r--   0 scovitz    (502) staff       (20)      963 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/anat/sub-01_ses-phdiff_T1w.json
--rw-r--r--   0 scovitz    (502) staff       (20)   123172 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/anat/sub-01_ses-phdiff_T1w.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.457843 cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/dwi/
--rw-r--r--   0 scovitz    (502) staff       (20)      283 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.bval
--rw-r--r--   0 scovitz    (502) staff       (20)     1685 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.bvec
--rw-r--r--   0 scovitz    (502) staff       (20)     1780 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.json
--rw-r--r--   0 scovitz    (502) staff       (20)    30889 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.459082 cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/fmap/
--rw-r--r--   0 scovitz    (502) staff       (20)     1508 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude1.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2107 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude1.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     1529 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude2.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2107 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude2.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     1610 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_phasediff.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2106 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_phasediff.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     1867 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_dir-PA_epi.json
--rw-r--r--   0 scovitz    (502) staff       (20)     1502 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_dir-PA_epi.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.459354 cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/func/
--rw-r--r--   0 scovitz    (502) staff       (20)     1970 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/func/sub-01_ses-phdiff_task-rest_bold.json
--rw-r--r--   0 scovitz    (502) staff       (20)    30889 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/func/sub-01_ses-phdiff_task-rest_bold.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.432379 cubids-1.0.9/cubids/testdata/inconsistent/sub-02/
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.432667 cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.459893 cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/anat/
--rw-r--r--   0 scovitz    (502) staff       (20)      963 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/anat/sub-02_ses-phdiff_T1w.json
--rw-r--r--   0 scovitz    (502) staff       (20)   123172 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/anat/sub-02_ses-phdiff_T1w.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.460764 cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/dwi/
--rw-r--r--   0 scovitz    (502) staff       (20)      283 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.bval
--rw-r--r--   0 scovitz    (502) staff       (20)     1685 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.bvec
--rw-r--r--   0 scovitz    (502) staff       (20)     1761 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.json
--rw-r--r--   0 scovitz    (502) staff       (20)    30889 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.462304 cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/fmap/
--rw-r--r--   0 scovitz    (502) staff       (20)     1508 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude1.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2107 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude1.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     1529 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude2.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2107 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude2.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     1610 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_phasediff.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2106 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_phasediff.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     1782 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_dir-PA_epi.json
--rw-r--r--   0 scovitz    (502) staff       (20)     1502 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_dir-PA_epi.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.462947 cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/func/
--rw-r--r--   0 scovitz    (502) staff       (20)     1937 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/func/sub-02_ses-phdiff_task-rest_bold.json
--rw-r--r--   0 scovitz    (502) staff       (20)    30889 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/func/sub-02_ses-phdiff_task-rest_bold.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.432794 cubids-1.0.9/cubids/testdata/inconsistent/sub-03/
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.433048 cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.463273 cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/anat/
--rw-r--r--   0 scovitz    (502) staff       (20)      963 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/anat/sub-03_ses-phdiff_T1w.json
--rw-r--r--   0 scovitz    (502) staff       (20)   123172 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/anat/sub-03_ses-phdiff_T1w.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.464267 cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/dwi/
--rw-r--r--   0 scovitz    (502) staff       (20)      283 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.bval
--rw-r--r--   0 scovitz    (502) staff       (20)     1685 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.bvec
--rw-r--r--   0 scovitz    (502) staff       (20)     1780 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.json
--rw-r--r--   0 scovitz    (502) staff       (20)    30889 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.467015 cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/fmap/
--rw-r--r--   0 scovitz    (502) staff       (20)     1508 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude1.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2107 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude1.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     1529 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude2.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2107 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude2.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     1610 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_phasediff.json
--rw-r--r--   0 scovitz    (502) staff       (20)     2106 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_phasediff.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     1867 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_dir-PA_epi.json
--rw-r--r--   0 scovitz    (502) staff       (20)     1502 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_dir-PA_epi.nii.gz
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.467597 cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/func/
--rw-r--r--   0 scovitz    (502) staff       (20)     1971 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/func/sub-03_ses-phdiff_task-rest_bold.json
--rw-r--r--   0 scovitz    (502) staff       (20)    30889 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/func/sub-03_ses-phdiff_task-rest_bold.nii.gz
--rw-r--r--   0 scovitz    (502) staff       (20)     3694 2023-05-04 11:48:08.000000 cubids-1.0.9/cubids/validator.py
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.437471 cubids-1.0.9/cubids.egg-info/
--rw-r--r--   0 scovitz    (502) staff       (20)     2428 2023-07-31 06:47:31.000000 cubids-1.0.9/cubids.egg-info/PKG-INFO
--rw-r--r--   0 scovitz    (502) staff       (20)    15549 2023-07-31 06:47:31.000000 cubids-1.0.9/cubids.egg-info/SOURCES.txt
--rw-r--r--   0 scovitz    (502) staff       (20)        1 2023-07-31 06:47:31.000000 cubids-1.0.9/cubids.egg-info/dependency_links.txt
--rw-r--r--   0 scovitz    (502) staff       (20)      579 2023-07-31 06:47:31.000000 cubids-1.0.9/cubids.egg-info/entry_points.txt
--rw-r--r--   0 scovitz    (502) staff       (20)        1 2023-07-31 06:47:31.000000 cubids-1.0.9/cubids.egg-info/not-zip-safe
--rw-r--r--   0 scovitz    (502) staff       (20)      522 2023-07-31 06:47:31.000000 cubids-1.0.9/cubids.egg-info/requires.txt
--rw-r--r--   0 scovitz    (502) staff       (20)        7 2023-07-31 06:47:31.000000 cubids-1.0.9/cubids.egg-info/top_level.txt
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.469891 cubids-1.0.9/docs/
--rw-r--r--   0 scovitz    (502) staff       (20)      607 2023-05-04 11:48:08.000000 cubids-1.0.9/docs/Makefile
--rw-r--r--   0 scovitz    (502) staff       (20)     1383 2023-05-04 11:48:08.000000 cubids-1.0.9/docs/README.rst
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.476728 cubids-1.0.9/docs/_static/
--rw-r--r--   0 scovitz    (502) staff       (20)    94377 2023-05-04 11:48:08.000000 cubids-1.0.9/docs/_static/checked_dataset_into_datalad.png
--rw-r--r--   0 scovitz    (502) staff       (20)    63002 2023-05-04 11:48:08.000000 cubids-1.0.9/docs/_static/cubids_workflow.png
--rw-r--r--   0 scovitz    (502) staff       (20)   121910 2023-05-04 11:48:08.000000 cubids-1.0.9/docs/_static/screenshot_1.png
--rw-r--r--   0 scovitz    (502) staff       (20)   183503 2023-05-04 11:48:08.000000 cubids-1.0.9/docs/_static/screenshot_2.png
--rw-r--r--   0 scovitz    (502) staff       (20)   140263 2023-05-04 11:48:08.000000 cubids-1.0.9/docs/_static/screenshot_3.png
--rw-r--r--   0 scovitz    (502) staff       (20)   186964 2023-05-04 11:48:08.000000 cubids-1.0.9/docs/_static/screenshot_4.png
--rw-r--r--   0 scovitz    (502) staff       (20)   189860 2023-05-04 11:48:08.000000 cubids-1.0.9/docs/_static/screenshot_5.png
--rw-r--r--   0 scovitz    (502) staff       (20)   218126 2023-05-04 11:48:08.000000 cubids-1.0.9/docs/_static/screenshot_6.png
--rw-r--r--   0 scovitz    (502) staff       (20)   359707 2023-05-04 11:48:08.000000 cubids-1.0.9/docs/_static/screenshot_7.png
--rw-r--r--   0 scovitz    (502) staff       (20)   434468 2023-05-04 11:48:08.000000 cubids-1.0.9/docs/_static/screenshot_8.png
--rw-r--r--   0 scovitz    (502) staff       (20)     3934 2023-05-04 11:48:08.000000 cubids-1.0.9/docs/about.rst
--rw-r--r--   0 scovitz    (502) staff       (20)       28 2023-05-04 11:48:08.000000 cubids-1.0.9/docs/authors.rst
--rwxr-xr-x   0 scovitz    (502) staff       (20)     5579 2023-05-04 11:48:08.000000 cubids-1.0.9/docs/conf.py
--rw-r--r--   0 scovitz    (502) staff       (20)       33 2023-05-04 11:48:08.000000 cubids-1.0.9/docs/contributing.rst
--rw-r--r--   0 scovitz    (502) staff       (20)    17209 2023-05-04 11:48:08.000000 cubids-1.0.9/docs/example.rst
--rw-r--r--   0 scovitz    (502) staff       (20)       28 2023-05-04 11:48:08.000000 cubids-1.0.9/docs/history.rst
--rw-r--r--   0 scovitz    (502) staff       (20)      194 2023-05-04 11:48:08.000000 cubids-1.0.9/docs/index.rst
--rw-r--r--   0 scovitz    (502) staff       (20)     2427 2023-05-04 11:48:08.000000 cubids-1.0.9/docs/installation.rst
--rw-r--r--   0 scovitz    (502) staff       (20)      768 2023-05-04 11:48:08.000000 cubids-1.0.9/docs/make.bat
--rw-r--r--   0 scovitz    (502) staff       (20)    12979 2023-05-04 11:48:08.000000 cubids-1.0.9/docs/usage.rst
--rw-r--r--   0 scovitz    (502) staff       (20)       60 2023-05-04 11:48:08.000000 cubids-1.0.9/pyproject.toml
--rw-r--r--   0 scovitz    (502) staff       (20)     1501 2023-07-31 06:47:31.480097 cubids-1.0.9/setup.cfg
--rw-r--r--   0 scovitz    (502) staff       (20)     2102 2023-07-31 06:45:34.000000 cubids-1.0.9/setup.py
-drwxr-xr-x   0 scovitz    (502) staff       (20)        0 2023-07-31 06:47:31.479020 cubids-1.0.9/tests/
--rw-r--r--   0 scovitz    (502) staff       (20)    37792 2023-05-04 11:48:08.000000 cubids-1.0.9/tests/test_bond.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 cubids-1.1.0/.dockerignore
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 cubids-1.1.0/.gitignore
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 cubids-1.1.0/.readthedocs.yml
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 cubids-1.1.0/AUTHORS.rst
+-rw-r--r--   0        0        0     4143 2020-02-02 00:00:00.000000 cubids-1.1.0/CITATION.cff
+-rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 cubids-1.1.0/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     3096 2020-02-02 00:00:00.000000 cubids-1.1.0/HISTORY.rst
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 cubids-1.1.0/LICENSE
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 cubids-1.1.0/MANIFEST.in
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 cubids-1.1.0/Makefile
+-rw-r--r--   0        0        0     2960 2020-02-02 00:00:00.000000 cubids-1.1.0/README.rst
+-rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 cubids-1.1.0/neurodebian.gpg
+-rw-r--r--   0        0        0     4373 2020-02-02 00:00:00.000000 cubids-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 cubids-1.1.0/.circleci/config.yml
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 cubids-1.1.0/.github/dependabot.yml
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 cubids-1.1.0/.github/pull_request_template.md
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 cubids-1.1.0/.github/release.yml
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 cubids-1.1.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 cubids-1.1.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 cubids-1.1.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 cubids-1.1.0/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/__about__.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/__init__.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/_version.py
+-rw-r--r--   0        0        0    21184 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/cli.py
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/config.py
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/constants.py
+-rw-r--r--   0        0        0    67133 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/cubids.py
+-rw-r--r--   0        0        0    11748 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/metadata_merge.py
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/utils.py
+-rw-r--r--   0        0        0     4570 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/validator.py
+-rw-r--r--   0        0        0    28472 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/workflows.py
+-rw-r--r--   0        0        0    12157 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/data/config.yml
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/coverage.cfg
+-rw-r--r--   0        0        0    35618 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/test_bond.py
+-rw-r--r--   0        0        0     2957 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/test_cli.py
+-rw-r--r--   0        0        0     7530 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/test_cubids.py
+-rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/utils.py
+-rw-r--r--   0        0        0    69774 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset.zip
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/README
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/dataset_description.json
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-01/ses-phdiff/anat/sub-01_ses-phdiff_T1w.json
+-rw-r--r--   0        0        0   123172 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-01/ses-phdiff/anat/sub-01_ses-phdiff_T1w.nii.gz
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.bval
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.bvec
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.json
+-rw-r--r--   0        0        0     6084 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.nii.gz
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude1.json
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude1.nii.gz
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude2.json
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude2.nii.gz
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_phasediff.json
+-rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_phasediff.nii.gz
+-rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_dir-PA_epi.json
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_dir-PA_epi.nii.gz
+-rw-r--r--   0        0        0     2234 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-01/ses-phdiff/func/sub-01_ses-phdiff_task-rest_bold.json
+-rw-r--r--   0        0        0    30889 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-01/ses-phdiff/func/sub-01_ses-phdiff_task-rest_bold.nii.gz
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-02/ses-phdiff/anat/sub-02_ses-phdiff_T1w.json
+-rw-r--r--   0        0        0   123172 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-02/ses-phdiff/anat/sub-02_ses-phdiff_T1w.nii.gz
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.bval
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.bvec
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.json
+-rw-r--r--   0        0        0    30889 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.nii.gz
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude1.json
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude1.nii.gz
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude2.json
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude2.nii.gz
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_phasediff.json
+-rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_phasediff.nii.gz
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_dir-PA_epi.json
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_dir-PA_epi.nii.gz
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-02/ses-phdiff/func/sub-02_ses-phdiff_task-rest_bold.json
+-rw-r--r--   0        0        0    30889 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-02/ses-phdiff/func/sub-02_ses-phdiff_task-rest_bold.nii.gz
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-03/ses-phdiff/anat/sub-03_ses-phdiff_T1w.json
+-rw-r--r--   0        0        0   123172 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-03/ses-phdiff/anat/sub-03_ses-phdiff_T1w.nii.gz
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.bval
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.bvec
+-rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.json
+-rw-r--r--   0        0        0    30889 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.nii.gz
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude1.json
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude1.nii.gz
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude2.json
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude2.nii.gz
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_phasediff.json
+-rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_phasediff.nii.gz
+-rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_dir-PA_epi.json
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_dir-PA_epi.nii.gz
+-rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-03/ses-phdiff/func/sub-03_ses-phdiff_task-rest_bold.json
+-rw-r--r--   0        0        0    30889 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-03/ses-phdiff/func/sub-03_ses-phdiff_task-rest_bold.nii.gz
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-04/ses-phdiff/anat/sub-04_ses-phdiff_T1w.json
+-rw-r--r--   0        0        0   123172 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-04/ses-phdiff/anat/sub-04_ses-phdiff_T1w.nii.gz
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-04/ses-phdiff/dwi/sub-04_ses-phdiff_acq-HASC55AP_dwi.bval
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-04/ses-phdiff/dwi/sub-04_ses-phdiff_acq-HASC55AP_dwi.bvec
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-04/ses-phdiff/dwi/sub-04_ses-phdiff_acq-HASC55AP_dwi.json
+-rw-r--r--   0        0        0    30889 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-04/ses-phdiff/dwi/sub-04_ses-phdiff_acq-HASC55AP_dwi.nii.gz
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_acq-v4_magnitude1.json
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_acq-v4_magnitude1.nii.gz
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_acq-v4_magnitude2.json
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_acq-v4_magnitude2.nii.gz
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_acq-v4_phasediff.json
+-rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_acq-v4_phasediff.nii.gz
+-rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_dir-PA_epi.json
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_dir-PA_epi.nii.gz
+-rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-04/ses-phdiff/func/sub-04_ses-phdiff_task-rest_bold.json
+-rw-r--r--   0        0        0    30889 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-04/ses-phdiff/func/sub-04_ses-phdiff_task-rest_bold.nii.gz
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/CuBIDS_Toy_Dataset_Curation/no_ped.txt
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/CuBIDS_Toy_Dataset_Curation/too_low_vols.txt
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/CuBIDS_Toy_Dataset_Curation/v0_AcqGroupInfo.txt
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/CuBIDS_Toy_Dataset_Curation/v0_AcqGrouping.csv
+-rw-r--r--   0        0        0     5979 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/CuBIDS_Toy_Dataset_Curation/v0_files.csv
+-rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/CuBIDS_Toy_Dataset_Curation/v0_summary.csv
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/CuBIDS_Toy_Dataset_Curation/v0_validation.csv
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/CuBIDS_Toy_Dataset_Curation/v1_AcqGroupInfo.txt
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/CuBIDS_Toy_Dataset_Curation/v1_AcqGrouping.csv
+-rw-r--r--   0        0        0     5691 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/CuBIDS_Toy_Dataset_Curation/v1_files.csv
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/CuBIDS_Toy_Dataset_Curation/v1_summary.csv
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/CuBIDS_Toy_Dataset_Curation/v2_AcqGroupInfo.txt
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/CuBIDS_Toy_Dataset_Curation/v2_AcqGrouping.csv
+-rw-r--r--   0        0        0     5808 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/CuBIDS_Toy_Dataset_Curation/v2_files.csv
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/CuBIDS_Toy_Dataset_Curation/v2_full_cmd.sh
+-rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/CuBIDS_Toy_Dataset_Curation/v2_summary.csv
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/complete/README
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/complete/dataset_description.json
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/complete/sub-01/ses-phdiff/anat/sub-01_ses-phdiff_T1w.json
+-rw-r--r--   0        0        0   123172 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/complete/sub-01/ses-phdiff/anat/sub-01_ses-phdiff_T1w.nii.gz
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/complete/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.bval
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/complete/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.bvec
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/complete/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.json
+-rw-r--r--   0        0        0    30889 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/complete/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.nii.gz
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude1.json
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude1.nii.gz
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude2.json
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude2.nii.gz
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_phasediff.json
+-rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_phasediff.nii.gz
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_dir-PA_epi.json
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_dir-PA_epi.nii.gz
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/complete/sub-01/ses-phdiff/func/sub-01_ses-phdiff_task-rest_bold.json
+-rw-r--r--   0        0        0    30889 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/complete/sub-01/ses-phdiff/func/sub-01_ses-phdiff_task-rest_bold.nii.gz
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/complete/sub-02/ses-phdiff/anat/sub-02_ses-phdiff_T1w.json
+-rw-r--r--   0        0        0   123172 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/complete/sub-02/ses-phdiff/anat/sub-02_ses-phdiff_T1w.nii.gz
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/complete/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.bval
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/complete/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.bvec
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/complete/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.json
+-rw-r--r--   0        0        0    30889 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/complete/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.nii.gz
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude1.json
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude1.nii.gz
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude2.json
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude2.nii.gz
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_phasediff.json
+-rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_phasediff.nii.gz
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_dir-PA_epi.json
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_dir-PA_epi.nii.gz
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/complete/sub-02/ses-phdiff/func/sub-02_ses-phdiff_task-rest_bold.json
+-rw-r--r--   0        0        0    30889 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/complete/sub-02/ses-phdiff/func/sub-02_ses-phdiff_task-rest_bold.nii.gz
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/complete/sub-03/ses-phdiff/anat/sub-03_ses-phdiff_T1w.json
+-rw-r--r--   0        0        0   123172 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/complete/sub-03/ses-phdiff/anat/sub-03_ses-phdiff_T1w.nii.gz
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/complete/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.bval
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/complete/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.bvec
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/complete/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.json
+-rw-r--r--   0        0        0    30889 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/complete/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.nii.gz
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude1.json
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude1.nii.gz
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude2.json
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude2.nii.gz
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_phasediff.json
+-rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_phasediff.nii.gz
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_dir-PA_epi.json
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_dir-PA_epi.nii.gz
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/complete/sub-03/ses-phdiff/func/sub-03_ses-phdiff_task-rest_bold.json
+-rw-r--r--   0        0        0    30889 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/complete/sub-03/ses-phdiff/func/sub-03_ses-phdiff_task-rest_bold.nii.gz
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/inconsistent/README
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/inconsistent/dataset_description.json
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/inconsistent/sub-01/ses-phdiff/anat/sub-01_ses-phdiff_T1w.json
+-rw-r--r--   0        0        0   123172 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/inconsistent/sub-01/ses-phdiff/anat/sub-01_ses-phdiff_T1w.nii.gz
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/inconsistent/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.bval
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/inconsistent/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.bvec
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/inconsistent/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.json
+-rw-r--r--   0        0        0    30889 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/inconsistent/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.nii.gz
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude1.json
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude1.nii.gz
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude2.json
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude2.nii.gz
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_phasediff.json
+-rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_phasediff.nii.gz
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_dir-PA_epi.json
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_dir-PA_epi.nii.gz
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/inconsistent/sub-01/ses-phdiff/func/sub-01_ses-phdiff_task-rest_bold.json
+-rw-r--r--   0        0        0    30889 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/inconsistent/sub-01/ses-phdiff/func/sub-01_ses-phdiff_task-rest_bold.nii.gz
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/inconsistent/sub-02/ses-phdiff/anat/sub-02_ses-phdiff_T1w.json
+-rw-r--r--   0        0        0   123172 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/inconsistent/sub-02/ses-phdiff/anat/sub-02_ses-phdiff_T1w.nii.gz
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/inconsistent/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.bval
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/inconsistent/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.bvec
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/inconsistent/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.json
+-rw-r--r--   0        0        0    30889 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/inconsistent/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.nii.gz
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude1.json
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude1.nii.gz
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude2.json
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude2.nii.gz
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_phasediff.json
+-rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_phasediff.nii.gz
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_dir-PA_epi.json
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_dir-PA_epi.nii.gz
+-rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/inconsistent/sub-02/ses-phdiff/func/sub-02_ses-phdiff_task-rest_bold.json
+-rw-r--r--   0        0        0    30889 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/inconsistent/sub-02/ses-phdiff/func/sub-02_ses-phdiff_task-rest_bold.nii.gz
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/inconsistent/sub-03/ses-phdiff/anat/sub-03_ses-phdiff_T1w.json
+-rw-r--r--   0        0        0   123172 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/inconsistent/sub-03/ses-phdiff/anat/sub-03_ses-phdiff_T1w.nii.gz
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/inconsistent/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.bval
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/inconsistent/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.bvec
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/inconsistent/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.json
+-rw-r--r--   0        0        0    30889 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/inconsistent/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.nii.gz
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude1.json
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude1.nii.gz
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude2.json
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude2.nii.gz
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_phasediff.json
+-rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_phasediff.nii.gz
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_dir-PA_epi.json
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_dir-PA_epi.nii.gz
+-rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/inconsistent/sub-03/ses-phdiff/func/sub-03_ses-phdiff_task-rest_bold.json
+-rw-r--r--   0        0        0    30889 2020-02-02 00:00:00.000000 cubids-1.1.0/cubids/tests/data/inconsistent/sub-03/ses-phdiff/func/sub-03_ses-phdiff_task-rest_bold.nii.gz
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 cubids-1.1.0/docs/Makefile
+-rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 cubids-1.1.0/docs/about.rst
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 cubids-1.1.0/docs/api.rst
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 cubids-1.1.0/docs/cli.rst
+-rwxr-xr-x   0        0        0     9303 2020-02-02 00:00:00.000000 cubids-1.1.0/docs/conf.py
+-rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 cubids-1.1.0/docs/example.rst
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 cubids-1.1.0/docs/examples.rst
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 cubids-1.1.0/docs/glossary.rst
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 cubids-1.1.0/docs/index.rst
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 cubids-1.1.0/docs/installation.rst
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 cubids-1.1.0/docs/links.rst
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 cubids-1.1.0/docs/make.bat
+-rw-r--r--   0        0        0    12276 2020-02-02 00:00:00.000000 cubids-1.1.0/docs/usage.rst
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 cubids-1.1.0/docs/_static/No_PED.txt
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 cubids-1.1.0/docs/_static/PNC_example_edited.csv
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 cubids-1.1.0/docs/_static/PNC_example_unedited.csv
+-rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 cubids-1.1.0/docs/_static/PNC_post_apply_summary.csv
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 cubids-1.1.0/docs/_static/PNC_pre_apply_summary_dwi_run1.csv
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 cubids-1.1.0/docs/_static/PNC_pre_apply_summary_dwi_run1_deletion.csv
+-rw-r--r--   0        0        0    94377 2020-02-02 00:00:00.000000 cubids-1.1.0/docs/_static/checked_dataset_into_datalad.png
+-rw-r--r--   0        0        0    63002 2020-02-02 00:00:00.000000 cubids-1.1.0/docs/_static/cubids_workflow.png
+-rw-r--r--   0        0        0   121910 2020-02-02 00:00:00.000000 cubids-1.1.0/docs/_static/screenshot_1.png
+-rw-r--r--   0        0        0   183503 2020-02-02 00:00:00.000000 cubids-1.1.0/docs/_static/screenshot_2.png
+-rw-r--r--   0        0        0   140263 2020-02-02 00:00:00.000000 cubids-1.1.0/docs/_static/screenshot_3.png
+-rw-r--r--   0        0        0   186964 2020-02-02 00:00:00.000000 cubids-1.1.0/docs/_static/screenshot_4.png
+-rw-r--r--   0        0        0   189860 2020-02-02 00:00:00.000000 cubids-1.1.0/docs/_static/screenshot_5.png
+-rw-r--r--   0        0        0   218126 2020-02-02 00:00:00.000000 cubids-1.1.0/docs/_static/screenshot_6.png
+-rw-r--r--   0        0        0   359707 2020-02-02 00:00:00.000000 cubids-1.1.0/docs/_static/screenshot_7.png
+-rw-r--r--   0        0        0   434468 2020-02-02 00:00:00.000000 cubids-1.1.0/docs/_static/screenshot_8.png
+-rw-r--r--   0        0        0     2631 2020-02-02 00:00:00.000000 cubids-1.1.0/docs/_static/v0_edited_summary.csv
+-rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 cubids-1.1.0/docs/_static/v0_summary.csv
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 cubids-1.1.0/docs/_static/v0_validation.csv
+-rw-r--r--   0        0        0     8578 2020-02-02 00:00:00.000000 cubids-1.1.0/docs/notebooks/Fieldmaps.ipynb
+-rw-r--r--   0        0        0     5544 2020-02-02 00:00:00.000000 cubids-1.1.0/docs/notebooks/FirstProofofConcept.ipynb
+-rw-r--r--   0        0        0    23136 2020-02-02 00:00:00.000000 cubids-1.1.0/docs/notebooks/HTML_param_groups.ipynb
+-rw-r--r--   0        0        0    32530 2020-02-02 00:00:00.000000 cubids-1.1.0/docs/notebooks/JSON_PoC_read_write.ipynb
+-rw-r--r--   0        0        0    11433 2020-02-02 00:00:00.000000 cubids-1.1.0/docs/notebooks/Key_and_Param_Groups.ipynb
+-rw-r--r--   0        0        0    21172 2020-02-02 00:00:00.000000 cubids-1.1.0/docs/notebooks/PofC_Key_Values2.ipynb
+-rw-r--r--   0        0        0    71319 2020-02-02 00:00:00.000000 cubids-1.1.0/docs/notebooks/keyparamgrouptest.ipynb
+-rw-r--r--   0        0        0    17682 2020-02-02 00:00:00.000000 cubids-1.1.0/docs/notebooks/metadata_image_param.ipynb
+-rw-r--r--   0        0        0   107751 2020-02-02 00:00:00.000000 cubids-1.1.0/docs/notebooks/rename_files_work.ipynb
+-rw-r--r--   0        0        0    34282 2020-02-02 00:00:00.000000 cubids-1.1.0/docs/notebooks/workwithtestdata.ipynb
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 cubids-1.1.0/docs/notebooks/Tests/datatype-anat_reconstruction-refaced_suffix-T1w.csv
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 cubids-1.1.0/docs/notebooks/Tests/datatype-func_run-1_suffix-bold_task-rest.csv
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 cubids-1.1.0/docs/notebooks/Tests/datatype-func_run-2_suffix-bold_task-rest.csv
+-rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 cubids-1.1.0/docs/sphinxext/github_link.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 cubids-1.1.0/.gitignore
+-rw-r--r--   0        0        0     3924 2020-02-02 00:00:00.000000 cubids-1.1.0/PKG-INFO
```

### Comparing `cubids-1.0.9/CONTRIBUTING.rst` & `cubids-1.1.0/CONTRIBUTING.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .. highlight:: shell
 
 ============
 Contributing
 ============
 
-Contributions are welcome, and they are greatly appreciated! Every little bit
-helps, and credit will always be given.
+Contributions are welcome, and they are greatly appreciated!
+Every little bit helps, and credit will always be given.
 
 You can contribute in many ways:
 
 Types of Contributions
 ----------------------
 
 Report Bugs
@@ -22,29 +22,28 @@
 * Your operating system name and version.
 * Any details about your local setup that might be helpful in troubleshooting.
 * Detailed steps to reproduce the bug.
 
 Fix Bugs
 ~~~~~~~~
 
-Look through the GitHub issues for bugs. Anything tagged with "bug" and "help
-wanted" is open to whoever wants to implement it.
+Look through the GitHub issues for bugs.
+Anything tagged with "bug" and "help wanted" is open to whoever wants to implement it.
 
 Implement Features
 ~~~~~~~~~~~~~~~~~~
 
-Look through the GitHub issues for features. Anything tagged with "enhancement"
-and "help wanted" is open to whoever wants to implement it.
+Look through the GitHub issues for features.
+Anything tagged with "enhancement" and "help wanted" is open to whoever wants to implement it.
 
 Write Documentation
 ~~~~~~~~~~~~~~~~~~~
 
-CuBIDS could always use more documentation, whether as part of the
-official CuBIDS docs, in docstrings, or even on the web in blog posts,
-articles, and such.
+CuBIDS could always use more documentation, whether as part of the official CuBIDS docs,
+in docstrings, or even on the web in blog posts, articles, and such.
 
 Submit Feedback
 ~~~~~~~~~~~~~~~
 
 The best way to send feedback is to file an issue at https://github.com/PennLINC/cubids/issues.
 
 If you are proposing a feature:
@@ -55,75 +54,77 @@
   are welcome :)
 
 Get Started!
 ------------
 
 Ready to contribute? Here's how to set up `cubids` for local development.
 
-1. Fork the `cubids` repo on GitHub.
-2. Clone your fork locally::
+1.  Fork the `cubids` repo on GitHub.
+2.  Clone your fork locally::
 
     $ git clone git@github.com:your_name_here/cubids.git
 
-3. Install your local copy into a virtualenv. Assuming you have virtualenvwrapper installed, this is how you set up your fork for local development::
+3.  Install your local copy into a virtualenv.
+    Assuming you have virtualenvwrapper installed,
+    this is how you set up your fork for local development::
 
     $ mkvirtualenv cubids
     $ cd cubids/
     $ python setup.py develop
 
-4. Create a branch for local development::
+4.  Create a branch for local development::
 
     $ git checkout -b name-of-your-bugfix-or-feature
 
    Now you can make your changes locally.
 
-5. When you're done making changes, check that your changes pass flake8 and the
-   tests, including testing other Python versions with tox::
+5.  When you're done making changes, check that your changes pass flake8 and the
+    tests, including testing other Python versions with tox::
 
     $ flake8 cubids tests
     $ python setup.py test or pytest
     $ tox
 
-   To get flake8 and tox, just pip install them into your virtualenv.
+    To get flake8 and tox, just pip install them into your virtualenv.
 
-6. Commit your changes and push your branch to GitHub::
+6.  Commit your changes and push your branch to GitHub::
 
     $ git add .
     $ git commit -m "Your detailed description of your changes."
     $ git push origin name-of-your-bugfix-or-feature
 
-7. Submit a pull request through the GitHub website.
+7.  Submit a pull request through the GitHub website.
 
 Pull Request Guidelines
 -----------------------
 
 Before you submit a pull request, check that it meets these guidelines:
 
-1. The pull request should include tests.
-2. If the pull request adds functionality, the docs should be updated. Put
-   your new functionality into a function with a docstring, and add the
-   feature to the list in README.rst.
-3. The pull request should work for 5, 3.6, 3.7 and 3.8, and for PyPy. Check
-   https://circleci.com/gh/PennLINC/CuBIDS
-   and make sure that the tests pass for all supported Python versions.
+1.  The pull request should include tests.
+2.  If the pull request adds functionality, the docs should be updated. Put
+    your new functionality into a function with a docstring, and add the
+    feature to the list in README.rst.
+3.  The pull request should work for Python 3.5, 3.6, 3.7 and 3.8, and for PyPy.
+    Check https://circleci.com/gh/PennLINC/CuBIDS
+    and make sure that the tests pass for all supported Python versions.
 
 Tips
 ----
 
 To run a subset of tests::
 
-$ cd PATH/TO/LOCAL/CuBIDS/CLONE
-$ py.test -sv --pdb tests
+    $ cd PATH/TO/LOCAL/CuBIDS/CLONE
+    $ py.test -sv --pdb tests
 
 
 Deploying
 ---------
 
 A reminder for the maintainers on how to deploy.
 Make sure all your changes are committed (including an entry in HISTORY.rst).
 Then run::
 
-$ bump2version patch # possible: major / minor / patch
-$ git push
-$ git push --tags
+    $ bump2version patch # possible: major / minor / patch
+    $ git push
+    $ git push --tags
 
 CircleCI will then deploy to PyPI if tests pass.
```

### Comparing `cubids-1.0.9/LICENSE` & `cubids-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/PKG-INFO` & `cubids-1.1.0/README.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,68 +1,73 @@
-Metadata-Version: 2.1
-Name: cubids
-Version: 1.0.9
-Summary: BIDS Curation Tool
-Home-page: https://github.com/pennlinc/cubids
-Author: Neuroinformatics Team of PennLINC
-Author-email: sydney.covitz@pennmecidine.upenn.edu
-Maintainer: Sydney Covitz
-License: MIT License
-Keywords: cubids
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.5
-Provides-Extra: datalad
-Provides-Extra: doc
-Provides-Extra: docs
-Provides-Extra: tests
-Provides-Extra: all
-License-File: LICENSE
-License-File: AUTHORS.rst
-
 ========================
 CuBIDS: Curation of BIDS
 ========================
 
-
 .. image:: https://img.shields.io/pypi/v/cubids.svg
-        :target: https://pypi.python.org/pypi/cubids
+    :target: https://pypi.python.org/pypi/cubids
+    :alt: Latest Version
 
-.. image:: https://circleci.com/gh/PennLINC/CuBIDS.svg?style=svg
-        :target: https://circleci.com/gh/PennLINC/CuBIDS
+.. image:: https://img.shields.io/badge/Source%20Code-pennlinc%2Fcubids-purple
+   :target: https://github.com/PennLINC/CuBIDS
+   :alt: GitHub Repository
 
 .. image:: https://readthedocs.org/projects/cubids/badge/?version=latest
-        :target: https://cubids.readthedocs.io/en/latest/?badge=latest
-        :alt: Documentation Status
+    :target: https://cubids.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
+
+.. image:: https://circleci.com/gh/PennLINC/CuBIDS.svg?style=svg
+    :target: https://circleci.com/gh/PennLINC/CuBIDS
+    :alt: Test Status
+
+.. image:: https://codecov.io/gh/PennLINC/CuBIDS/branch/main/graph/badge.svg
+   :target: https://app.codecov.io/gh/PennLINC/CuBIDS/tree/main
+   :alt: Codecov
+
+.. image:: https://img.shields.io/badge/NeuroImage-10.1016%2Fj.neuroimage.2022.119609-purple
+   :target: https://doi.org/10.1016/j.neuroimage.2022.119609
+   :alt: Publication DOI
+
+.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.6514881.svg
+   :target: https://doi.org/10.5281/zenodo.6514881
+   :alt: Zenodo DOI
+
+.. image:: https://img.shields.io/badge/License-MIT-green
+   :target: https://opensource.org/licenses/MIT
+   :alt: License
+
 
 About
 -----
 
-Curation of BIDS, or ``CuBIDS``, is a workflow and software package designed to facilitate
+``CuBIDS`` (Curation of BIDS) is a workflow and software package designed to facilitate
 reproducible curation of neuroimaging `BIDS <https://bids-specification.readthedocs.io/>`_ datasets.
-CuBIDS breaks down BIDS dataset curation into four main components and addresses each one using 
-various command line programs complete with version control capabilities. These components are not necessarily linear but all are critical 
-in the process of preparing BIDS data for successful preprocessing and analysis pipeline runs. 
-
-  1. CuBIDS facilitates the validation of BIDS data.
-  2. CuBIDS visualizes and summarizes the heterogeneity in a BIDS dataset. 
-  3. CuBIDS helps users test pipelines on the entire parameter space of a BIDS dataset.
-  4. CuBIDS allows users to perform metadata-based quality control on their BIDS data.
+CuBIDS breaks down BIDS dataset curation into four main components and addresses each one using
+various command line programs complete with version control capabilities.
+These components are not necessarily linear but all are critical
+in the process of preparing BIDS data for successful preprocessing and analysis pipeline runs.
+
+  1.    CuBIDS facilitates the validation of BIDS data.
+  2.    CuBIDS visualizes and summarizes the heterogeneity in a BIDS dataset.
+  3.    CuBIDS helps users test pipelines on the entire parameter space of a BIDS dataset.
+  4.    CuBIDS allows users to perform metadata-based quality control on their BIDS data.
+  5.    CuBIDS helps users clean protected information in BIDS datasets,
+        in order to prepare them for public sharing.
 
 .. image:: https://github.com/PennLINC/CuBIDS/raw/main/docs/_static/cubids_workflow.png
    :width: 600
 
-For full documentation, please visit our `ReadTheDocs <https://cubids.readthedocs.io/en/latest/?badge=latest>`_ 
+For full documentation, please visit our
+`ReadTheDocs <https://cubids.readthedocs.io/en/latest/?badge=latest>`_.
+
+
+Citing CuBIDS
+-------------
 
-=======
-History
-=======
+If you use CuBIDS in your research, please cite the following paper:
 
-0.1.0 (2020-10-07)
-------------------
+    Covitz, S., Tapera, T. M., Adebimpe, A., Alexander-Bloch, A. F., Bertolero, M. A., Feczko, E.,
+    ... & Satterthwaite, T. D. (2022).
+    Curation of BIDS (CuBIDS): A workflow and software package for streamlining reproducible curation of large BIDS datasets.
+    NeuroImage, 263, 119609.
+    doi:10.1016/j.neuroimage.2022.119609.
 
-* First release on PyPI.
+Please also cite the Zenodo DOI for the version you used.
```

### Comparing `cubids-1.0.9/cubids/cubids.py` & `cubids-1.1.0/cubids/cubids.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,177 +1,276 @@
 """Main module."""
-import warnings
-from collections import defaultdict
-import subprocess
-import bids
-import bids.layout
-import json
+
 import csv
+import json
 import os
 import re
+import subprocess
+import warnings
+from collections import defaultdict
 from pathlib import Path
-from bids.layout import parse_file_entities
-from bids.utils import listify
+from shutil import copyfile, copytree
+
+import bids
+import bids.layout
+import datalad.api as dlapi
+import nibabel as nb
 import numpy as np
 import pandas as pd
-import nibabel as nb
-import datalad.api as dlapi
-from shutil import copytree, copyfile
+from bids.layout import parse_file_entities
+from bids.utils import listify
 from sklearn.cluster import AgglomerativeClustering
 from tqdm import tqdm
-from .constants import ID_VARS, NON_KEY_ENTITIES
-from .config import load_config
-from .metadata_merge import (
-    check_merging_operations, group_by_acquisition_sets)
-warnings.simplefilter(action='ignore', category=FutureWarning)
-bids.config.set_option('extension_initial_dot', True)
+
+from cubids.config import load_config
+from cubids.constants import ID_VARS, NON_KEY_ENTITIES
+from cubids.metadata_merge import check_merging_operations, group_by_acquisition_sets
+
+warnings.simplefilter(action="ignore", category=FutureWarning)
+bids.config.set_option("extension_initial_dot", True)
 
 
 class CuBIDS(object):
+    """The main CuBIDS class.
 
-    def __init__(self, data_root, use_datalad=False, acq_group_level='subject',
-                 grouping_config=None, force_unlock=False):
+    Parameters
+    ----------
+    data_root : :obj:`str`
+        Path to the root of the BIDS dataset.
+    use_datalad : :obj:`bool`, optional
+        If True, use datalad to track changes to the BIDS dataset.
+        Default is False.
+    acq_group_level : :obj:`str`, optional
+        The level at which to group scans. Default is "subject".
+    grouping_config : :obj:`str`, optional
+        Path to the grouping config file.
+        Default is None, in which case the default config in CuBIDS is used.
+    force_unlock : :obj:`bool`, optional
+        If True, force unlock all files in the BIDS dataset.
+        Default is False.
+
+    Attributes
+    ----------
+    path : :obj:`str`
+        Path to the root of the BIDS dataset.
+    _layout : :obj:`bids.layout.BIDSLayout`
+        The BIDSLayout object.
+    keys_files : :obj:`dict`
+        A dictionary of key groups and the files that belong to them.
+    fieldmaps_cached : :obj:`bool`
+        If True, the fieldmaps have been cached.
+    datalad_ready : :obj:`bool`
+        If True, the datalad dataset has been initialized.
+    datalad_handle : :obj:`datalad.api.Dataset`
+        The datalad dataset handle.
+    old_filenames : :obj:`list`
+        A list of old filenames.
+    new_filenames : :obj:`list`
+        A list of new filenames.
+    IF_rename_paths : :obj:`list`
+        A list of IntendedFor paths that have been renamed.
+    grouping_config : :obj:`dict`
+        The grouping config dictionary.
+    acq_group_level : :obj:`str`
+        The level at which to group scans.
+    scans_txt : :obj:`str`
+        Path to the .txt file that lists the scans
+        you want to be deleted from the dataset, along
+        with their associations.
+    force_unlock : :obj:`bool`
+        If True, force unlock all files in the BIDS dataset.
+    cubids_code_dir : :obj:`bool`
+        If True, the CuBIDS code directory exists.
+    data_dict : :obj:`dict`
+        A data dictionary for TSV outputs.
+    use_datalad : :obj:`bool`
+        If True, use datalad to track changes to the BIDS dataset.
+    """
 
+    def __init__(
+        self,
+        data_root,
+        use_datalad=False,
+        acq_group_level="subject",
+        grouping_config=None,
+        force_unlock=False,
+    ):
         self.path = os.path.abspath(data_root)
         self._layout = None
         self.keys_files = {}
         self.fieldmaps_cached = False
         self.datalad_ready = False
         self.datalad_handle = None
         self.old_filenames = []  # files whose key groups changed
         self.new_filenames = []  # new filenames for files to change
         self.IF_rename_paths = []  # fmap jsons with rename intended fors
         self.grouping_config = load_config(grouping_config)
         self.acq_group_level = acq_group_level
         self.scans_txt = None  # txt file of scans to purge (for purge only)
         self.force_unlock = force_unlock  # force unlock for add-nifti-info
-        self.cubids_code_dir = Path(self.path + '/code/CuBIDS').is_dir()
+        self.cubids_code_dir = Path(self.path + "/code/CuBIDS").is_dir()
         self.data_dict = {}  # data dictionary for TSV outputs
         self.use_datalad = use_datalad  # True if flag set, False if flag unset
         if self.use_datalad:
             self.init_datalad()
 
-        if self.acq_group_level == 'session':
+        if self.acq_group_level == "session":
             NON_KEY_ENTITIES.remove("session")
 
     @property
     def layout(self):
+        """Return the BIDSLayout object.
+
+        If the BIDSLayout object has not been created, create it.
+        """
         if self._layout is None:
             # print("SETTING LAYOUT OBJECT")
             self.reset_bids_layout()
             # print("LAYOUT OBJECT SET")
         return self._layout
 
     def reset_bids_layout(self, validate=False):
+        """Reset the BIDS layout.
+
+        This sets the ``_layout`` attribute to a new :obj:`bids.layout.BIDSLayout` object.
+
+        Parameters
+        ----------
+        validate : :obj:`bool`, optional
+            If True, validate the BIDS dataset. Default is False.
+        """
         # create BIDS Layout Indexer class
 
-        ignores = ["code", "stimuli", "sourcedata", "models",
-                   re.compile(r'^\.'), re.compile(r'/\.')]
+        ignores = [
+            "code",
+            "stimuli",
+            "sourcedata",
+            "models",
+            re.compile(r"^\."),
+            re.compile(r"/\."),
+        ]
 
-        indexer = bids.BIDSLayoutIndexer(validate=validate, ignore=ignores,
-                                         index_metadata=False)
+        indexer = bids.BIDSLayoutIndexer(validate=validate, ignore=ignores, index_metadata=False)
 
-        self._layout = bids.BIDSLayout(self.path,
-                                       validate=validate,
-                                       indexer=indexer)
+        self._layout = bids.BIDSLayout(self.path, validate=validate, indexer=indexer)
 
     def create_cubids_code_dir(self):
+        """Create CuBIDS code directory.
+
+        This creates the CuBIDS code directory at self.path/code/CuBIDS.
+
+        Returns
+        -------
+        :obj:`str`
+            Path to the CuBIDS code directory.
+
+        Notes
+        -----
+        Why not use ``os.makedirs``?
+        """
         # check if BIDS_ROOT/code/CuBIDS exists
         if not self.cubids_code_dir:
-            subprocess.run(['mkdir', self.path + '/code'])
-            subprocess.run(['mkdir', self.path + '/code/CuBIDS/'])
+            subprocess.run(["mkdir", self.path + "/code"])
+            subprocess.run(["mkdir", self.path + "/code/CuBIDS/"])
             self.cubids_code_dir = True
         return self.cubids_code_dir
 
     def init_datalad(self):
-        """Initializes a datalad Dataset at self.path.
+        """Initialize a datalad Dataset at self.path.
 
-        Parameters:
-        -----------
-
-            save: bool
-                Run datalad save to add any untracked files
-            message: str or None
-                Message to add to
+        This creates a datalad dataset at self.path and sets the
+        ``datalad_ready`` attribute to True.
+        It also sets the ``datalad_handle`` attribute to the datalad.Dataset object.
         """
         self.datalad_ready = True
 
         self.datalad_handle = dlapi.Dataset(self.path)
         if not self.datalad_handle.is_installed():
-            self.datalad_handle = dlapi.create(self.path,
-                                               cfg_proc='text2git',
-                                               force=True,
-                                               annex=True)
+            self.datalad_handle = dlapi.create(
+                self.path, cfg_proc="text2git", force=True, annex=True
+            )
 
     def datalad_save(self, message=None):
-        """Performs a DataLad Save operation on the BIDS tree.
+        """Perform a DataLad Save operation on the BIDS tree.
 
         Additionally a check for an active datalad handle and that the
         status of all objects after the save is "ok".
 
         Parameters:
         -----------
-            message : str or None
-                Commit message to use with datalad save
+        message : str or None
+            Commit message to use with datalad save.
         """
-
         if not self.datalad_ready:
-            raise Exception(
-                "DataLad has not been initialized. use datalad_init()")
+            raise Exception("DataLad has not been initialized. use datalad_init()")
+
         statuses = self.datalad_handle.save(message=message or "CuBIDS Save")
-        saved_status = set([status['status'] for status in statuses])
+        saved_status = set([status["status"] for status in statuses])
         if not saved_status == set(["ok"]):
             raise Exception("Failed to save in DataLad")
 
     def is_datalad_clean(self):
-        """If True, no changes are detected in the datalad dataset."""
+        """If True, no changes are detected in the datalad dataset.
+
+        Returns
+        -------
+        :obj:`bool`
+            True if the datalad dataset is clean, False otherwise.
+
+        Raises
+        ------
+        Exception
+            If datalad has not been initialized.
+        """
         if not self.datalad_ready:
-            raise Exception(
-                "Datalad not initialized, can't determine status")
-        statuses = set([status['state'] for status in
-                        self.datalad_handle.status()])
+            raise Exception("Datalad not initialized, can't determine status")
+        statuses = set([status["state"] for status in self.datalad_handle.status()])
         return statuses == set(["clean"])
 
     def datalad_undo_last_commit(self):
         """Revert the most recent commit, remove it from history.
 
         Uses git reset --hard to revert to the previous commit.
+
+        Raises
+        ------
+        Exception
+            If there are untracked changes in the datalad dataset.
         """
         if not self.is_datalad_clean():
-            raise Exception("Untracked changes present. "
-                            "Run clear_untracked_changes first")
-        reset_proc = subprocess.run(
-            ["git", "reset", "--hard", "HEAD~1"], cwd=self.path)
+            raise Exception("Untracked changes present. Run clear_untracked_changes first")
+        reset_proc = subprocess.run(["git", "reset", "--hard", "HEAD~1"], cwd=self.path)
         reset_proc.check_returncode()
 
-    def add_nifti_info(self, raise_on_error=True):
-        """Adds info from nifti files to json sidecars."""
+    def add_nifti_info(self):
+        """Add info from nifti files to json sidecars."""
         # check if force_unlock is set
         if self.force_unlock:
             # CHANGE TO SUBPROCESS.CALL IF NOT BLOCKING
             subprocess.run(["datalad", "unlock"], cwd=self.path)
 
         # loop through all niftis in the bids dir
         for path in Path(self.path).rglob("sub-*/**/*.*"):
             # ignore all dot directories
-            if '/.' in str(path):
+            if "/." in str(path):
                 continue
+
             if str(path).endswith(".nii") or str(path).endswith(".nii.gz"):
                 try:
                     img = nb.load(str(path))
                 except Exception:
                     print("Empty Nifti File: ", str(path))
                     continue
+
                 # get important info from niftis
-                obliquity = np.any(nb.affines.obliquity(img.affine)
-                                   > 1e-4)
+                obliquity = np.any(nb.affines.obliquity(img.affine) > 1e-4)
                 voxel_sizes = img.header.get_zooms()
                 matrix_dims = img.shape
                 # add nifti info to corresponding sidecars​
-                sidecar = img_to_new_ext(str(path), '.json')
+                sidecar = img_to_new_ext(str(path), ".json")
                 if Path(sidecar).exists():
                     try:
                         with open(sidecar) as f:
                             data = json.load(f)
                     except Exception:
                         print("Error parsing this sidecar: ", sidecar)
 
@@ -192,471 +291,490 @@
                     if "NumVolumes" not in data.keys():
                         if img.ndim == 4:
                             data["NumVolumes"] = matrix_dims[3]
                         elif img.ndim == 3:
                             data["NumVolumes"] = 1
                     if "ImageOrientation" not in data.keys():
                         orient = nb.orientations.aff2axcodes(img.affine)
-                        joined = ''.join(orient) + '+'
+                        joined = "".join(orient) + "+"
                         data["ImageOrientation"] = joined
-                    with open(sidecar, 'w') as file:
+
+                    with open(sidecar, "w") as file:
                         json.dump(data, file, indent=4)
 
         if self.use_datalad:
             self.datalad_save(message="Added nifti info to sidecars")
+
         self.reset_bids_layout()
 
-    def apply_tsv_changes(self, summary_tsv, files_tsv, new_prefix,
-                          raise_on_error=True):
-        """Applies changes documented in the edited _summary tsv
-        and generates the new tsv files.
+    def apply_tsv_changes(self, summary_tsv, files_tsv, new_prefix, raise_on_error=True):
+        """Apply changes documented in the edited summary tsv and generate the new tsv files.
 
         This function looks at the RenameKeyGroup and MergeInto
-        columns and modifies the bids datset according to the
+        columns and modifies the bids dataset according to the
         specified changs.
 
-        Parameters:
-        -----------
-            orig_prefix : str
-                Path prefix and file stem for the original
-                _summary and _files tsvs.
-                For example, if orig_prefix is
-                '/cbica/projects/HBN/old_tsvs' then the paths to
-                the summary and files tsvs will be
-                '/cbica/projects/HBN/old_tsvs_summary.tsv' and
-                '/cbica/projects/HBN/old_tsvs_files.tsv' respectively.
-            new_prefix : str
-                Path prefix and file stem for the new summary and
-                files tsvs.
+        Parameters
+        ----------
+        summary_tsv : :obj:`str`
+            Path to the edited summary tsv file.
+        files_tsv : :obj:`str`
+            Path to the edited files tsv file.
+        new_prefix : :obj:`str`
+            Path prefix to the new tsv files.
+        raise_on_error : :obj:`bool`
+            If True, raise an error if the MergeInto column contains invalid merges.
         """
         # reset lists of old and new filenames
         self.old_filenames = []
         self.new_filenames = []
 
-        if '/' not in str(summary_tsv):
+        if "/" not in str(summary_tsv):
             if not self.cubids_code_dir:
                 self.create_cubids_code_dir()
-            summary_tsv = self.path + '/code/CuBIDS/' + summary_tsv
-        if '/' not in str(files_tsv):
+            summary_tsv = self.path + "/code/CuBIDS/" + summary_tsv
+
+        if "/" not in str(files_tsv):
             if not self.cubids_code_dir:
                 self.create_cubids_code_dir()
-            files_tsv = self.path + '/code/CuBIDS/' + files_tsv
+            files_tsv = self.path + "/code/CuBIDS/" + files_tsv
 
         summary_df = pd.read_table(summary_tsv)
         files_df = pd.read_table(files_tsv)
 
         # Check that the MergeInto column only contains valid merges
-        ok_merges, deletions = check_merging_operations(
-            summary_tsv, raise_on_error=raise_on_error)
+        ok_merges, deletions = check_merging_operations(summary_tsv, raise_on_error=raise_on_error)
 
         merge_commands = []
         for source_id, dest_id in ok_merges:
-            dest_files = files_df.loc[
-                (files_df[["ParamGroup", "KeyGroup"]] == dest_id).all(1)]
-            source_files = files_df.loc[
-                (files_df[["ParamGroup", "KeyGroup"]] == source_id).all(1)]
+            dest_files = files_df.loc[(files_df[["ParamGroup", "KeyGroup"]] == dest_id).all(1)]
+            source_files = files_df.loc[(files_df[["ParamGroup", "KeyGroup"]] == source_id).all(1)]
 
             # Get a source json file
             img_full_path = self.path + source_files.iloc[0].FilePath
-            source_json = img_to_new_ext(img_full_path, '.json')
+            source_json = img_to_new_ext(img_full_path, ".json")
             for dest_nii in dest_files.FilePath:
-                dest_json = img_to_new_ext(self.path + dest_nii, '.json')
+                dest_json = img_to_new_ext(self.path + dest_nii, ".json")
                 if Path(dest_json).exists() and Path(source_json).exists():
-                    merge_commands.append(
-                        'bids-sidecar-merge %s %s'
-                        % (source_json, dest_json))
+                    merge_commands.append(f"bids-sidecar-merge {source_json} {dest_json}")
 
         # Get the delete commands
         # delete_commands = []
         to_remove = []
         for rm_id in deletions:
-            files_to_rm = files_df.loc[
-                (files_df[["ParamGroup", "KeyGroup"]] == rm_id).all(1)]
+            files_to_rm = files_df.loc[(files_df[["ParamGroup", "KeyGroup"]] == rm_id).all(1)]
 
             for rm_me in files_to_rm.FilePath:
                 if Path(self.path + rm_me).exists():
                     to_remove.append(self.path + rm_me)
                     # delete_commands.append("rm " + rm_me)
 
         # call purge associations on list of files to remove
         self._purge_associations(to_remove)
 
         # Now do the file renaming
         change_keys_df = summary_df[summary_df.RenameKeyGroup.notnull()]
         move_ops = []
         # return if nothing to change
         if len(change_keys_df) > 0:
-
             key_groups = {}
 
             for i in range(len(change_keys_df)):
-                new_key = change_keys_df.iloc[i]['RenameKeyGroup']
-                old_key_param = change_keys_df.iloc[i]['KeyParamGroup']
+                new_key = change_keys_df.iloc[i]["RenameKeyGroup"]
+                old_key_param = change_keys_df.iloc[i]["KeyParamGroup"]
 
                 # add to dictionary
                 key_groups[old_key_param] = new_key
 
             # orig key/param tuples that will have new key group
             to_change = list(key_groups.keys())
 
             for row in range(len(files_df)):
-                file_path = self.path + files_df.loc[row, 'FilePath']
-                if Path(file_path).exists() and '/fmap/' not in file_path:
-
-                    key_param_group = files_df.loc[row, 'KeyParamGroup']
+                file_path = self.path + files_df.loc[row, "FilePath"]
+                if Path(file_path).exists() and "/fmap/" not in file_path:
+                    key_param_group = files_df.loc[row, "KeyParamGroup"]
 
                     if key_param_group in to_change:
-
-                        orig_key_param = files_df.loc[row, 'KeyParamGroup']
+                        orig_key_param = files_df.loc[row, "KeyParamGroup"]
 
                         new_key = key_groups[orig_key_param]
 
                         new_entities = _key_group_to_entities(new_key)
 
                         # generate new filenames according to new key group
                         self.change_filename(file_path, new_entities)
 
             # create string of mv command ; mv command for dlapi.run
-            for from_file, to_file in zip(self.old_filenames,
-                                          self.new_filenames):
-
+            for from_file, to_file in zip(self.old_filenames, self.new_filenames):
                 if Path(from_file).exists():
                     # if using datalad, we want to git mv instead of mv
                     if self.use_datalad:
-                        move_ops.append('git mv %s %s' % (from_file, to_file))
+                        move_ops.append(f"git mv {from_file} {to_file}")
                     else:
-                        move_ops.append('mv %s %s' % (from_file, to_file))
+                        move_ops.append(f"mv {from_file} {to_file}")
+
         full_cmd = "\n".join(merge_commands + move_ops)
         if full_cmd:
-            # write full_cmd to a .sh file
-            # Open file for writing
-            fileObject = open(new_prefix + "_full_cmd.sh", "w")
-            fileObject.write("#!/bin/bash\n")
-            fileObject.write(full_cmd)
-            # Close the file
-            fileObject.close()
+            renames = new_prefix + "_full_cmd.sh"
 
-            renames = new_prefix + '_full_cmd.sh'
+            # write full_cmd to a .sh file
+            with open(renames, "w") as fo:
+                fo.write("#!/bin/bash\n")
+                fo.write(full_cmd)
 
             if self.use_datalad:
-
                 # first check if IntendedFor renames need to be saved
                 if not self.is_datalad_clean():
                     s1 = "Renamed IntendedFor references to "
                     s2 = "Variant Group scans"
                     IF_rename_msg = s1 + s2
                     self.datalad_handle.save(message=IF_rename_msg)
 
                 s1 = "Renamed Variant Group scans according to their variant "
                 s2 = "parameters"
 
                 rename_commit = s1 + s2
 
-                self.datalad_handle.run(cmd=["bash", renames],
-                                        message=rename_commit)
+                self.datalad_handle.run(cmd=["bash", renames], message=rename_commit)
             else:
-                subprocess.run(["bash", renames],
-                               stdout=subprocess.PIPE,
-                               cwd=str(Path(new_prefix).parent))
+                subprocess.run(
+                    ["bash", renames],
+                    stdout=subprocess.PIPE,
+                    cwd=str(Path(new_prefix).parent),
+                )
         else:
             print("Not running any commands")
 
         self.reset_bids_layout()
-        self.get_TSVs(new_prefix)
+        self.get_tsvs(new_prefix)
 
         # remove renames file that gets created under the hood
-        subprocess.run(['rm', '-rf', 'renames'])
+        subprocess.run(["rm", "-rf", "renames"])
 
     def change_filename(self, filepath, entities):
-        """Applies changes to a filename based on the renamed
-        key groups.
+        """Apply changes to a filename based on the renamed key groups.
+
         This function takes into account the new key group names
         and renames all files whose key group names changed.
-        Parameters:
-        -----------
-            filepath : str
-                Path prefix to a file in the affected key group change
-            entities : dictionary
-                A pybids dictionary of entities parsed from the new key
-                group name.
+
+        Parameters
+        ----------
+        filepath : :obj:`str`
+            Path prefix to a file in the affected key group change.
+        entities : :obj:`dict`
+            A pybids dictionary of entities parsed from the new key group name.
+
+        Notes
+        -----
+        This is the function I need to spend the most time on, since it has entities hardcoded.
         """
         exts = Path(filepath).suffixes
-        old_ext = ""
-        for ext in exts:
-            old_ext += ext
+        old_ext = "".join(exts)
 
-        suffix = entities['suffix']
+        suffix = entities["suffix"]
         entity_file_keys = []
-        file_keys = ['task', 'acquisition', 'direction',
-                     'reconstruction', 'run']
+
+        # Entities that may be in the filename?
+        file_keys = ["task", "acquisition", "direction", "reconstruction", "run"]
 
         for key in file_keys:
             if key in list(entities.keys()):
                 entity_file_keys.append(key)
 
-        sub = get_key_name(filepath, 'sub')
-        ses = get_key_name(filepath, 'ses')
-        sub_ses = sub + '_' + ses
-
-        if 'run' in list(entities.keys()) and 'run-0' in filepath:
-            entities['run'] = '0' + str(entities['run'])
-
-        filename = "_".join(["{}-{}".format(key, entities[key])
-                             for key in entity_file_keys])
-        filename = filename.replace('acquisition', 'acq') \
-            .replace('direction', 'dir') \
-            .replace('reconstruction', 'rec')
+        sub = get_key_name(filepath, "sub")
+        ses = get_key_name(filepath, "ses")
+        sub_ses = sub + "_" + ses
+
+        if "run" in list(entities.keys()) and "run-0" in filepath:
+            # XXX: This adds an extra leading zero to run.
+            entities["run"] = "0" + str(entities["run"])
+
+        filename = "_".join([f"{key}-{entities[key]}" for key in entity_file_keys])
+        filename = (
+            filename.replace("acquisition", "acq")
+            .replace("direction", "dir")
+            .replace("reconstruction", "rec")
+        )
         if len(filename) > 0:
-            filename = sub_ses + '_' + filename + '_' + suffix + old_ext
+            filename = sub_ses + "_" + filename + "_" + suffix + old_ext
         else:
-            filename = sub_ses + filename + '_' + suffix + old_ext
+            raise ValueError(f"Could not construct new filename for {filepath}")
 
         # CHECK TO SEE IF DATATYPE CHANGED
-        dtypes = ['anat', 'func', 'perf', 'fmap', 'dwi']
-        old = ''
+        # datatype may be overridden/changed if the original file is located in the wrong folder.
+        dtypes = ["anat", "func", "perf", "fmap", "dwi"]
+        dtype_orig = ""
         for dtype in dtypes:
             if dtype in filepath:
-                old = dtype
+                dtype_orig = dtype
 
-        if 'datatype' in entities.keys():
-            dtype = entities['datatype']
-            if entities['datatype'] != old:
+        if "datatype" in entities.keys():
+            dtype_new = entities["datatype"]
+            if entities["datatype"] != dtype_orig:
                 print("WARNING: DATATYPE CHANGE DETECETD")
         else:
-            dtype = old
-        new_path = str(self.path) + '/' + sub + '/' + ses \
-            + '/' + dtype + '/' + filename
+            dtype_new = dtype_orig
 
-        # add the scan path + new path to the lists of old, new filenames
+        # Construct the new filename
+        new_path = str(self.path) + "/" + sub + "/" + ses + "/" + dtype_new + "/" + filename
+
+        # Add the scan path + new path to the lists of old, new filenames
         self.old_filenames.append(filepath)
         self.new_filenames.append(new_path)
 
-        # NOW NEED TO RENAME ASSOCIATIONS
+        # NOW NEED TO RENAME ASSOCIATED FILES
         # bids_file = self.layout.get_file(filepath)
         bids_file = filepath
         # associations = bids_file.get_associations()
         associations = self.get_nifti_associations(str(bids_file))
         for assoc_path in associations:
             # assoc_path = assoc.path
             if Path(assoc_path).exists():
                 # print("FILE: ", filepath)
                 # print("ASSOC: ", assoc.path)
                 # ensure assoc not an IntendedFor reference
-                if '.nii' not in str(assoc_path):
+                if ".nii" not in str(assoc_path):
                     self.old_filenames.append(assoc_path)
-                    new_ext_path = img_to_new_ext(new_path,
-                                                  ''.join(Path(assoc_path)
-                                                          .suffixes))
+                    new_ext_path = img_to_new_ext(new_path, "".join(Path(assoc_path).suffixes))
                     self.new_filenames.append(new_ext_path)
 
         # MAKE SURE THESE AREN'T COVERED BY get_associations!!!
-        if '/dwi/' in filepath:
+        # Update DWI-specific files
+        if "/dwi/" in filepath:
             # add the bval and bvec if there
-            if Path(img_to_new_ext(filepath, '.bval')).exists() \
-                    and img_to_new_ext(filepath, '.bval') \
-                    not in self.old_filenames:
-                self.old_filenames.append(img_to_new_ext(filepath,
-                                                         '.bval'))
-                self.new_filenames.append(img_to_new_ext(new_path,
-                                                         '.bval'))
-
-            if Path(img_to_new_ext(filepath, '.bvec')).exists() \
-                    and img_to_new_ext(filepath, '.bvec') \
-                    not in self.old_filenames:
-                self.old_filenames.append(img_to_new_ext(filepath,
-                                                         '.bvec'))
-                self.new_filenames.append(img_to_new_ext(new_path,
-                                                         '.bvec'))
+            bval_old = img_to_new_ext(filepath, ".bval")
+            bval_new = img_to_new_ext(new_path, ".bval")
+            if Path(bval_old).exists() and bval_old not in self.old_filenames:
+                self.old_filenames.append(bval_old)
+                self.new_filenames.append(bval_new)
+
+            bvec_old = img_to_new_ext(filepath, ".bvec")
+            bvec_new = img_to_new_ext(new_path, ".bvec")
+            if Path(bvec_old).exists() and bvec_old not in self.old_filenames:
+                self.old_filenames.append(bvec_old)
+                self.new_filenames.append(bvec_new)
 
+        # Update func-specific files
         # now rename _events and _physio files!
-        old_suffix = parse_file_entities(filepath)['suffix']
-        scan_end = '_' + old_suffix + old_ext
+        old_suffix = parse_file_entities(filepath)["suffix"]
+        scan_end = "_" + old_suffix + old_ext
 
-        if '_task-' in filepath:
-            old_events = filepath.replace(scan_end, '_events.tsv')
-            old_ejson = filepath.replace(scan_end, '_events.json')
+        if "_task-" in filepath:
+            old_events = filepath.replace(scan_end, "_events.tsv")
             if Path(old_events).exists():
                 self.old_filenames.append(old_events)
-                new_scan_end = '_' + suffix + old_ext
-                new_events = new_path.replace(new_scan_end, '_events.tsv')
+                new_scan_end = "_" + suffix + old_ext
+                new_events = new_path.replace(new_scan_end, "_events.tsv")
                 self.new_filenames.append(new_events)
+
+            old_ejson = filepath.replace(scan_end, "_events.json")
             if Path(old_ejson).exists():
                 self.old_filenames.append(old_ejson)
-                new_scan_end = '_' + suffix + old_ext
-                new_ejson = new_path.replace(new_scan_end, '_events.json')
+                new_scan_end = "_" + suffix + old_ext
+                new_ejson = new_path.replace(new_scan_end, "_events.json")
                 self.new_filenames.append(new_ejson)
 
-        old_physio = filepath.replace(scan_end, '_physio.tsv.gz')
+        old_physio = filepath.replace(scan_end, "_physio.tsv.gz")
         if Path(old_physio).exists():
             self.old_filenames.append(old_physio)
-            new_scan_end = '_' + suffix + old_ext
-            new_physio = new_path.replace(new_scan_end, '_physio.tsv.gz')
+            new_scan_end = "_" + suffix + old_ext
+            new_physio = new_path.replace(new_scan_end, "_physio.tsv.gz")
             self.new_filenames.append(new_physio)
 
+        # Update ASL-specific files
+        if "/perf/" in filepath:
+            old_context = filepath.replace(scan_end, "_aslcontext.tsv")
+            if Path(old_context).exists():
+                self.old_filenames.append(old_context)
+                new_scan_end = "_" + suffix + old_ext
+                new_context = new_path.replace(new_scan_end, "_aslcontext.tsv")
+                self.new_filenames.append(new_context)
+
+            old_m0scan = filepath.replace(scan_end, "_m0scan.nii.gz")
+            if Path(old_m0scan).exists():
+                self.old_filenames.append(old_m0scan)
+                new_scan_end = "_" + suffix + old_ext
+                new_m0scan = new_path.replace(new_scan_end, "_m0scan.nii.gz")
+                self.new_filenames.append(new_m0scan)
+
+            old_mjson = filepath.replace(scan_end, "_m0scan.json")
+            if Path(old_mjson).exists():
+                self.old_filenames.append(old_mjson)
+                new_scan_end = "_" + suffix + old_ext
+                new_mjson = new_path.replace(new_scan_end, "_m0scan.json")
+                self.new_filenames.append(new_mjson)
+
+            old_labeling = filepath.replace(scan_end, "_asllabeling.jpg")
+            if Path(old_labeling).exists():
+                self.old_filenames.append(old_labeling)
+                new_scan_end = "_" + suffix + old_ext
+                new_labeling = new_path.replace(new_scan_end, "_asllabeling.jpg")
+                self.new_filenames.append(new_labeling)
+
         # RENAME INTENDED FORS!
-        ses_path = self.path + '/' + sub + '/' + ses
-        for path in Path(ses_path).rglob("fmap/*.json"):
-            self.IF_rename_paths.append(str(path))
-            # json_file = self.layout.get_file(str(path))
+        ses_path = self.path + "/" + sub + "/" + ses
+        files_with_if = []
+        files_with_if += Path(ses_path).rglob("fmap/*.json")
+        files_with_if += Path(ses_path).rglob("perf/*_m0scan.json")
+        for path_with_if in files_with_if:
+            filename_with_if = str(path_with_if)
+            self.IF_rename_paths.append(filename_with_if)
+            # json_file = self.layout.get_file(filename_with_if)
             # data = json_file.get_dict()
-            data = get_sidecar_metadata(str(path))
+            data = get_sidecar_metadata(filename_with_if)
             if data == "Erroneous sidecar":
-                print('Error parsing sidecar: ', str(path))
+                print("Error parsing sidecar: ", filename_with_if)
                 continue
 
-            if 'IntendedFor' in data.keys():
-                # check if IntendedFor field is a str or list
-                if isinstance(data['IntendedFor'], str):
-                    if data['IntendedFor'] == \
-                            _get_intended_for_reference(filepath):
-                        # replace old filename with new one (overwrite string)
-                        data['IntendedFor'] = \
-                                _get_intended_for_reference(new_path)
-
-                        # update the json with the new data dictionary
-                        _update_json(str(path), data)
-
-                if isinstance(data['IntendedFor'], list):
-                    for item in data['IntendedFor']:
-                        if item in _get_intended_for_reference(filepath):
-
-                            # remove old filename
-                            data['IntendedFor'].remove(item)
-                            # add new filename
-                            data['IntendedFor'].append(
-                                    _get_intended_for_reference(new_path))
+            if "IntendedFor" in data.keys():
+                # Coerce IntendedFor to a list.
+                data["IntendedFor"] = listify(data["IntendedFor"])
+                for item in data["IntendedFor"]:
+                    if item in _get_intended_for_reference(filepath):
+                        # remove old filename
+                        data["IntendedFor"].remove(item)
+                        # add new filename
+                        data["IntendedFor"].append(_get_intended_for_reference(new_path))
 
-                        # update the json with the new data dictionary
-                        _update_json(str(path), data)
+                # update the json with the new data dictionary
+                _update_json(filename_with_if, data)
 
         # save IntendedFor purges so that you can datalad run the
         # remove association file commands on a clean dataset
         # if self.use_datalad:
         #     if not self.is_datalad_clean():
         #         self.datalad_save(message="Renamed IntendedFors")
         #         self.reset_bids_layout()
-            # else:
-            #     print("No IntendedFor References to Rename")
+        # else:
+        #     print("No IntendedFor References to Rename")
 
-    def copy_exemplars(self, exemplars_dir, exemplars_tsv, min_group_size,
-                       raise_on_error=True):
-        """Copies one subject from each Acquisition Group into a new directory
-        for testing *preps, raises an error if the subjects are not unlocked,
+    def copy_exemplars(self, exemplars_dir, exemplars_tsv, min_group_size):
+        """Copy one subject from each Acquisition Group into a new directory for testing preps.
+
+        Raises an error if the subjects are not unlocked,
         unlocks each subject before copying if --force_unlock is set.
 
-        Parameters:
-        -----------
-            exemplars_dir: str
-                path to the directory that will contain one subject
-                from each Acqusition Gorup (*_AcqGrouping.tsv)
-                example path: /Users/Covitz/tsvs/CCNP_Acq_Groups/
-
-            exemplars_tsv: str
-                path to the .tsv file that lists one subject
-                from each Acqusition Group (*_AcqGrouping.tsv
-                from the cubids-group output)
-                example path: /Users/Covitz/tsvs/CCNP_Acq_Grouping.tsv
+        Parameters
+        ----------
+        exemplars_dir : :obj:`str`
+            path to the directory that will contain one subject
+            from each Acqusition Group (*_AcqGrouping.tsv)
+            example path: /Users/Covitz/tsvs/CCNP_Acq_Groups/
+        exemplars_tsv : :obj:`str`
+            path to the .tsv file that lists one subject
+            from each Acqusition Group (*_AcqGrouping.tsv
+            from the cubids-group output)
+            example path: /Users/Covitz/tsvs/CCNP_Acq_Grouping.tsv
+        min_group_size : :obj:`int`
+            Minimum number of subjects in an acq group for it to be included
+            in the exemplar dataset.
         """
         # create the exemplar ds
         if self.use_datalad:
-            subprocess.run(['datalad', '--log-level', 'error', 'create', '-c',
-                            'text2git', exemplars_dir])
+            subprocess.run(
+                [
+                    "datalad",
+                    "--log-level",
+                    "error",
+                    "create",
+                    "-c",
+                    "text2git",
+                    exemplars_dir,
+                ]
+            )
 
         # load the exemplars tsv
         subs = pd.read_table(exemplars_tsv)
 
         # if min group size flag set, drop acq groups with less than min
-        if int(min_group_size) > 1:
+        if min_group_size > 1:
             for row in range(len(subs)):
-                acq_group = subs.loc[row, 'AcqGroup']
-                size = int(subs['AcqGroup'].value_counts()[acq_group])
-                if size < int(min_group_size):
+                acq_group = subs.loc[row, "AcqGroup"]
+                size = int(subs["AcqGroup"].value_counts()[acq_group])
+                if size < min_group_size:
                     subs = subs.drop([row])
 
         # get one sub from each acq group
         unique = subs.drop_duplicates(subset=["AcqGroup"])
 
         # cast list to a set to drop duplicates, then convert back to list
-        unique_subs = list(set(unique['subject'].tolist()))
+        unique_subs = list(set(unique["subject"].tolist()))
         for subid in unique_subs:
-            source = str(self.path) + '/' + subid
-            dest = exemplars_dir + '/' + subid
+            source = str(self.path) + "/" + subid
+            dest = exemplars_dir + "/" + subid
             # Copy the content of source to destination
             copytree(source, dest)
 
         # Copy the dataset_description.json
-        copyfile(str(self.path) + '/' + 'dataset_description.json',
-                 exemplars_dir + '/' + 'dataset_description.json')
+        copyfile(
+            str(self.path) + "/" + "dataset_description.json",
+            exemplars_dir + "/" + "dataset_description.json",
+        )
 
         s1 = "Copied one subject from each Acquisition Group "
         s2 = "into the Exemplar Dataset"
         msg = s1 + s2
         if self.use_datalad:
-            subprocess.run(['datalad', 'save', '-d', exemplars_dir,
-                            '-m', msg])
+            subprocess.run(["datalad", "save", "-d", exemplars_dir, "-m", msg])
 
-    def purge(self, scans_txt, raise_on_error=True):
-        """Purges all associations of desired scans from a bids dataset.
+    def purge(self, scans_txt):
+        """Purge all associations of desired scans from a bids dataset.
 
-        Parameters:
-        -----------
-            scans_txt: str
-                path to the .txt file that lists the scans
-                you want to be deleted from the dataset, along
-                with thier associations.
-                example path: /Users/Covitz/CCNP/scans_to_delete.txt
+        Parameters
+        ----------
+        scans_txt : str
+            path to the .txt file that lists the scans
+            you want to be deleted from the dataset, along
+            with thier associations.
+            example path: /Users/Covitz/CCNP/scans_to_delete.txt
         """
-
         self.scans_txt = scans_txt
 
         scans = []
-        with open(scans_txt, 'r') as fd:
+        with open(scans_txt, "r") as fd:
             reader = csv.reader(fd)
             for row in reader:
-                scans.append(self.path + '/' + str(row[0]))
+                scans.append(self.path + "/" + str(row[0]))
 
         # check to ensure scans are all real files in the ds!
 
         self._purge_associations(scans)
 
     def _purge_associations(self, scans):
+        """Purge field map JSONs' IntendedFor references.
 
-        # PURGE FMAP JSONS' INTENDED FOR REFERENCES
-
+        Parameters
+        ----------
+        scans : :obj:`list` of :obj:`str`
+            List of file paths to remove from field map JSONs.
+        """
         # truncate all paths to intendedfor reference format
         # sub, ses, modality only (no self.path)
         if_scans = []
         for scan in scans:
             if_scans.append(_get_intended_for_reference(self.path + scan))
 
         for path in Path(self.path).rglob("sub-*/*/fmap/*.json"):
-
             # json_file = self.layout.get_file(str(path))
             # data = json_file.get_dict()
             data = get_sidecar_metadata(str(path))
             if data == "Erroneous sidecar":
-                print('Error parsing sidecar: ', str(path))
+                print("Error parsing sidecar: ", str(path))
                 continue
 
             # remove scan references in the IntendedFor
-            if 'IntendedFor' in data.keys():
-                # check if IntendedFor field value is a list or a string
-                if isinstance(data['IntendedFor'], str):
-                    if data['IntendedFor'] in if_scans:
-                        data['IntendedFor'] = []
-                        # update the json with the new data dictionary
-                        _update_json(str(path), data)
-
-                if isinstance(data['IntendedFor'], list):
-                    for item in data['IntendedFor']:
-                        if item in if_scans:
-                            data['IntendedFor'].remove(item)
+            if "IntendedFor" in data.keys():
+                data["IntendedFor"] = listify(data["IntendedFor"])
 
-                            # update the json with the new data dictionary
-                            _update_json(str(path), data)
+                for item in data["IntendedFor"]:
+                    if item in if_scans:
+                        data["IntendedFor"].remove(item)
+
+                # update the json with the new data dictionary
+                _update_json(str(path), data)
 
         # save IntendedFor purges so that you can datalad run the
         # remove association file commands on a clean dataset
         if self.use_datalad:
             if not self.is_datalad_clean():
                 s1 = "Purged IntendedFor references to files "
                 s2 = "requested for removal"
@@ -665,114 +783,114 @@
                 self.reset_bids_layout()
 
         # NOW WE WANT TO PURGE ALL ASSOCIATIONS
 
         to_remove = []
 
         for path in Path(self.path).rglob("sub-*/**/*.nii.gz"):
-
             if str(path) in scans:
                 # bids_file = self.layout.get_file(str(path))
                 # associations = bids_file.get_associations()
                 associations = self.get_nifti_associations(str(path))
                 for assoc in associations:
                     to_remove.append(assoc)
                     # filepath = assoc.path
 
             # ensure association is not an IntendedFor reference!
-            if '.nii' not in str(path):
-
-                if '/dwi/' in str(path):
+            if ".nii" not in str(path):
+                if "/dwi/" in str(path):
                     # add the bval and bvec if there
-                    if Path(img_to_new_ext(str(path), '.bval')).exists():
-                        to_remove.append(img_to_new_ext(str(path), '.bval'))
-                    if Path(img_to_new_ext(str(path), '.bvec')).exists():
-                        to_remove.append(img_to_new_ext(str(path), '.bvec'))
-                if '/func/' in str(path):
+                    if Path(img_to_new_ext(str(path), ".bval")).exists():
+                        to_remove.append(img_to_new_ext(str(path), ".bval"))
+                    if Path(img_to_new_ext(str(path), ".bvec")).exists():
+                        to_remove.append(img_to_new_ext(str(path), ".bvec"))
+
+                if "/func/" in str(path):
                     # add tsvs
-                    tsv = img_to_new_ext(str(path), '.tsv').replace(
-                            '_bold', '_events')
+                    tsv = img_to_new_ext(str(path), ".tsv").replace("_bold", "_events")
                     if Path(tsv).exists():
                         to_remove.append(tsv)
                     # add tsv json (if exists)
-                    if Path(tsv.replace('.tsv', '.json')).exists():
-                        to_remove.append(tsv.replace('.tsv', '.json'))
+                    if Path(tsv.replace(".tsv", ".json")).exists():
+                        to_remove.append(tsv.replace(".tsv", ".json"))
+
         to_remove += scans
 
         # create rm commands for all files that need to be purged
         purge_commands = []
         for rm_me in to_remove:
             if Path(rm_me).exists():
                 purge_commands.append("rm " + rm_me)
 
         # datalad run the file deletions (purges)
         full_cmd = "\n".join(purge_commands)
         if full_cmd:
-
             # write full_cmd to a .sh file
             # Open file for writing
 
             path_prefix = str(Path(self.path).parent)
 
-            fileObject = open(path_prefix + "/" + "_full_cmd.sh", "w")
-            fileObject.write("#!/bin/bash\n")
-            fileObject.write(full_cmd)
-            # Close the file
-            fileObject.close()
+            with open(path_prefix + "/" + "_full_cmd.sh", "w") as fo:
+                fo.write("#!/bin/bash\n")
+                fo.write(full_cmd)
+
             if self.scans_txt:
-                cmt = "Purged scans listed in %s from dataset" % self.scans_txt
+                cmt = f"Purged scans listed in {self.scans_txt} from dataset"
             else:
                 cmt = "Purged Parameter Groups marked for removal"
-            purge_file = path_prefix + "/" + '_full_cmd.sh'
+
+            purge_file = path_prefix + "/" + "_full_cmd.sh"
             if self.use_datalad:
-                self.datalad_handle.run(cmd=["bash", purge_file],
-                                        message=cmt)
+                self.datalad_handle.run(cmd=["bash", purge_file], message=cmt)
             else:
-                subprocess.run(["bash", path_prefix + "/" + "_full_cmd.sh"],
-                               stdout=subprocess.PIPE,
-                               cwd=path_prefix)
+                subprocess.run(
+                    ["bash", path_prefix + "/" + "_full_cmd.sh"],
+                    stdout=subprocess.PIPE,
+                    cwd=path_prefix,
+                )
+
             self.reset_bids_layout()
+
         else:
             print("Not running any association removals")
 
     def get_nifti_associations(self, nifti):
+        """Get nifti associations.
+
+        This uses globbing to find files with the same path, entities, and suffix as the NIfTI,
+        but with a different extension.
+        """
         # get all assocation files of a nifti image
-        no_ext_file = str(nifti).split('/')[-1].split('.')[0]
+        no_ext_file = str(nifti).split("/")[-1].split(".")[0]
         associations = []
-        for path in Path(self.path).rglob("sub-*/**/*.*"):
-            if no_ext_file in str(path) and '.nii.gz' not in str(path):
+        for path in Path(self.path).rglob(f"sub-*/**/{no_ext_file}.*"):
+            if ".nii.gz" not in str(path):
                 associations.append(str(path))
+
         return associations
 
     def _cache_fieldmaps(self):
-        """Searches all fieldmaps and creates a lookup for each file.
-
-        Returns:
-        -----------
-            misfits : list
-                A list of fmap filenames for whom CuBIDS has not detected
-                an IntnededFor.
-        """
-
-        suffix = '(phase1|phasediff|epi|fieldmap)'
-        fmap_files = self.layout.get(suffix=suffix, regex_search=True,
-                                     extension=['.nii.gz', '.nii'])
+        """Search all fieldmaps and create a lookup for each file."""
+        suffix = "(phase1|phasediff|epi|fieldmap)"
+        fmap_files = self.layout.get(
+            suffix=suffix, regex_search=True, extension=[".nii.gz", ".nii"]
+        )
 
         misfits = []
         files_to_fmaps = defaultdict(list)
         for fmap_file in tqdm(fmap_files):
             # intentions = listify(fmap_file.get_metadata().get("IntendedFor"))
-            fmap_json = img_to_new_ext(fmap_file.path, '.json')
+            fmap_json = img_to_new_ext(fmap_file.path, ".json")
             metadata = get_sidecar_metadata(fmap_json)
             if metadata == "Erroneous sidecar":
-                print('Error parsing sidecar: ', str(fmap_json))
+                print("Error parsing sidecar: ", str(fmap_json))
                 continue
             if_list = metadata.get("IntendedFor")
             intentions = listify(if_list)
-            subject_prefix = "sub-%s" % fmap_file.entities['subject']
+            subject_prefix = f"sub-{fmap_file.entities['subject']}"
 
             if intentions is not None:
                 for intended_for in intentions:
                     full_path = Path(self.path) / subject_prefix / intended_for
                     files_to_fmaps[str(full_path)].append(fmap_file)
 
             # fmap file detected, no intended for found
@@ -783,92 +901,95 @@
         self.fieldmaps_cached = True
 
         # return a list of all filenames where fmap file detected,
         # no intended for found
         return misfits
 
     def get_param_groups_from_key_group(self, key_group):
-        """Splits key groups into param groups based on json metadata.
+        """Split key groups into param groups based on json metadata.
 
-        Parameters:
-        -----------
-            key_group : str
-                Key group name.
-
-        Returns:
-        -----------
-            ret : tuple of two DataFrames
-                1. A data frame with one row per file where the ParamGroup
-                column indicates the group to which each scan belongs.
-                2. A data frame with param group summaries
+        Parameters
+        ----------
+        key_group : str
+            Key group name.
+
+        Returns
+        -------
+        ret : tuple of two DataFrames
+            1. A data frame with one row per file where the ParamGroup
+            column indicates the group to which each scan belongs.
+            2. A data frame with param group summaries
         """
         if not self.fieldmaps_cached:
-            raise Exception(
-                "Fieldmaps must be cached to find parameter groups.")
+            raise Exception("Fieldmaps must be cached to find parameter groups.")
         key_entities = _key_group_to_entities(key_group)
         key_entities["extension"] = ".nii[.gz]*"
 
-        matching_files = self.layout.get(return_type="file", scope="self",
-                                         regex_search=True, **key_entities)
+        matching_files = self.layout.get(
+            return_type="file", scope="self", regex_search=True, **key_entities
+        )
 
         # ensure files who's entities contain key_entities but include other
         # entities do not also get added to matching_files
         to_include = []
         for filepath in matching_files:
             f_key_group = _file_to_key_group(filepath)
 
             if f_key_group == key_group:
                 to_include.append(filepath)
 
         # get the modality associated with the key group
-        modalities = ['/dwi/', '/anat/', '/func/', '/perf/', '/fmap/']
-        modality = ''
+        modalities = ["/dwi/", "/anat/", "/func/", "/perf/", "/fmap/"]
+        modality = ""
         for mod in modalities:
             if mod in filepath:
-                modality = mod.replace('/', '').replace('/', '')
-        if modality == '':
+                modality = mod.replace("/", "").replace("/", "")
+
+        if modality == "":
             print("Unusual Modality Detected")
-            modality = 'other'
+            modality = "other"
 
         ret = _get_param_groups(
-            to_include, self.layout, self.fieldmap_lookup, key_group,
-            self.grouping_config, modality, self.keys_files)
+            to_include,
+            self.fieldmap_lookup,
+            key_group,
+            self.grouping_config,
+            modality,
+            self.keys_files,
+        )
 
         if ret == "erroneous sidecar found":
             return "erroneous sidecar found"
 
-        # add modality to the retun tuple
+        # add modality to the return tuple
         l_ret = list(ret)
         l_ret.append(modality)
         tup_ret = tuple(l_ret)
         return tup_ret
 
     def create_data_dictionary(self):
-
-        sidecar_params = self.grouping_config.get('sidecar_params')
+        """Create a data dictionary."""
+        sidecar_params = self.grouping_config.get("sidecar_params")
         for mod in sidecar_params.keys():
             mod_dict = sidecar_params[mod]
             for s_param in mod_dict.keys():
                 if s_param not in self.data_dict.keys():
-                    self.data_dict[s_param] = {"Description":
-                                               "Scanning Parameter"}
+                    self.data_dict[s_param] = {"Description": "Scanning Parameter"}
 
-        relational_params = self.grouping_config.get('relational_params')
+        relational_params = self.grouping_config.get("relational_params")
         for r_param in relational_params.keys():
             if r_param not in self.data_dict.keys():
-                self.data_dict[r_param] = {"Description":
-                                           "Scanning Parameter"}
+                self.data_dict[r_param] = {"Description": "Scanning Parameter"}
 
-        derived_params = self.grouping_config.get('derived_params')
+        derived_params = self.grouping_config.get("derived_params")
         for mod in derived_params.keys():
             mod_dict = derived_params[mod]
             for d_param in mod_dict.keys():
                 if d_param not in self.data_dict.keys():
-                    self.data_dict[d_param] = {"Description":
-                                               "NIfTI Header Parameter"}
+                    self.data_dict[d_param] = {"Description": "NIfTI Header Parameter"}
 
         # Manually add non-sidecar columns/descriptions to data_dict
         desc1 = "Column where users mark groups to manually check"
         self.data_dict["ManualCheck"] = {}
         self.data_dict["ManualCheck"]["Description"] = desc1
         desc2 = "Column to mark notes about the param group"
         self.data_dict["Notes"] = {}
@@ -901,32 +1022,26 @@
         self.data_dict["ParamGroup"]["Description"] = desc81 + desc82 + desc83
         desc91 = "Key Group name and Param Group number separated by a double"
         desc92 = " underscore"
         self.data_dict["KeyParamGroup"] = {}
         self.data_dict["KeyParamGroup"]["Description"] = desc91 + desc92
 
     def get_data_dictionary(self, df):
-        """Creates a BIDS data dictionary from dataframe columns
+        """Create a BIDS data dictionary from dataframe columns.
 
-        Parameters:
-        -----------
-
-            name: str
-                Data dictionary name (should be identical to filename of TSV)
-
-            df: Pandas DataFrame
-                Pre export TSV that will be converted to a json dictionary
-
-        Returns:
-        -----------
-
-            data_dict: dictionary
-                Python dictionary in BIDS data dictionary format
+        Parameters
+        ----------
+        df : Pandas DataFrame
+            Pre export TSV that will be converted to a json dictionary
+
+        Returns
+        -------
+        data_dict : dictionary
+            Python dictionary in BIDS data dictionary format
         """
-
         json_dict = {}
 
         # Build column dictionary
         col_list = df.columns.values.tolist()
 
         data_dict_keys = self.data_dict.keys()
 
@@ -948,469 +1063,461 @@
         # # Build top level dictionary
         # data_dict = {}
         # data_dict[name] = header_dict
 
         return json_dict
 
     def get_param_groups_dataframes(self):
-        '''Creates DataFrames of files x param groups and a summary'''
-
+        """Create DataFrames of files x param groups and a summary."""
         key_groups = self.get_key_groups()
         labeled_files = []
         param_group_summaries = []
         for key_group in key_groups:
             try:
-                labeled_file_params, param_summary, modality = \
-                    self.get_param_groups_from_key_group(key_group)
+                (
+                    labeled_file_params,
+                    param_summary,
+                    modality,
+                ) = self.get_param_groups_from_key_group(key_group)
             except Exception:
                 continue
             if labeled_file_params is None:
                 continue
             param_group_summaries.append(param_summary)
             labeled_files.append(labeled_file_params)
 
         big_df = _order_columns(pd.concat(labeled_files, ignore_index=True))
 
         # make Filepaths relative to bids dir
         for row in range(len(big_df)):
-            long_name = big_df.loc[row, 'FilePath']
-            big_df.loc[row, 'FilePath'] = long_name.replace(self.path, '')
+            long_name = big_df.loc[row, "FilePath"]
+            big_df.loc[row, "FilePath"] = long_name.replace(self.path, "")
 
-        summary = _order_columns(pd.concat(param_group_summaries,
-                                 ignore_index=True))
+        summary = _order_columns(pd.concat(param_group_summaries, ignore_index=True))
 
         # create new col that strings key and param group together
-        summary["KeyParamGroup"] = summary["KeyGroup"] \
-            + '__' + summary["ParamGroup"].map(str)
+        summary["KeyParamGroup"] = summary["KeyGroup"] + "__" + summary["ParamGroup"].map(str)
 
         # move this column to the front of the dataframe
         key_param_col = summary.pop("KeyParamGroup")
         summary.insert(0, "KeyParamGroup", key_param_col)
 
         # do the same for the files df
-        big_df["KeyParamGroup"] = big_df["KeyGroup"] \
-            + '__' + big_df["ParamGroup"].map(str)
+        big_df["KeyParamGroup"] = big_df["KeyGroup"] + "__" + big_df["ParamGroup"].map(str)
 
         # move this column to the front of the dataframe
         key_param_col = big_df.pop("KeyParamGroup")
         big_df.insert(0, "KeyParamGroup", key_param_col)
 
         summary.insert(0, "RenameKeyGroup", np.nan)
         summary.insert(0, "MergeInto", np.nan)
         summary.insert(0, "ManualCheck", np.nan)
         summary.insert(0, "Notes", np.nan)
 
         # Now automate suggested rename based on variant params
         # loop though imaging and derived param keys
 
-        sidecar = self.grouping_config.get('sidecar_params')
+        sidecar = self.grouping_config.get("sidecar_params")
         sidecar = sidecar[modality]
 
-        relational = self.grouping_config.get('relational_params')
+        relational = self.grouping_config.get("relational_params")
 
         # list of columns names that we account for in suggested renaming
-        summary['RenameKeyGroup'] = summary['RenameKeyGroup'].apply(str)
+        summary["RenameKeyGroup"] = summary["RenameKeyGroup"].apply(str)
 
         rename_cols = []
         tolerance_cols = []
         for col in sidecar.keys():
-            if 'suggest_variant_rename' in sidecar[col].keys():
-                if sidecar[col]['suggest_variant_rename'] \
-                        and col in summary.columns:
+            if "suggest_variant_rename" in sidecar[col].keys():
+                if sidecar[col]["suggest_variant_rename"] and col in summary.columns:
                     rename_cols.append(col)
-                    if 'tolerance' in sidecar[col].keys():
+                    if "tolerance" in sidecar[col].keys():
                         tolerance_cols.append(col)
 
         # deal with Fmap!
-        if 'FieldmapKey' in relational:
-            if 'suggest_variant_rename' in relational['FieldmapKey'].keys():
-                if relational['FieldmapKey']['suggest_variant_rename']:
+        if "FieldmapKey" in relational:
+            if "suggest_variant_rename" in relational["FieldmapKey"].keys():
+                if relational["FieldmapKey"]["suggest_variant_rename"]:
                     # check if 'bool' or 'columns'
-                    if relational['FieldmapKey']['display_mode'] == 'bool':
+                    if relational["FieldmapKey"]["display_mode"] == "bool":
                         rename_cols.append("HasFieldmap")
 
         # deal with IntendedFor Key!
-        if 'IntendedForKey' in relational:
-            if 'suggest_variant_rename' in relational['IntendedForKey'].keys():
-                if relational['FieldmapKey']['suggest_variant_rename']:
+        if "IntendedForKey" in relational:
+            if "suggest_variant_rename" in relational["IntendedForKey"].keys():
+                if relational["FieldmapKey"]["suggest_variant_rename"]:
                     # check if 'bool' or 'columns'
-                    if relational['IntendedForKey']['display_mode'] == 'bool':
+                    if relational["IntendedForKey"]["display_mode"] == "bool":
                         rename_cols.append("UsedAsFieldmap")
 
         dom_dict = {}
         # loop through summary tsv and create dom_dict
         for row in range(len(summary)):
             # if 'NumVolumes' in summary.columns \
             #         and str(summary.loc[row, "NumVolumes"]) == 'nan':
             #     summary.at[row, "NumVolumes"] = 1.0
 
             # if dominant group identified
-            if str(summary.loc[row, 'ParamGroup']) == '1':
+            if str(summary.loc[row, "ParamGroup"]) == "1":
                 val = {}
                 # grab col, all vals send to dict
                 key = summary.loc[row, "KeyGroup"]
                 for col in rename_cols:
                     summary[col] = summary[col].apply(str)
                     val[col] = summary.loc[row, col]
                 dom_dict[key] = val
 
         # now loop through again and ID variance
         for row in range(len(summary)):
             # check to see if renaming has already happened
             renamed = False
             entities = _key_group_to_entities(summary.loc[row, "KeyGroup"])
-            if 'VARIANT' in summary.loc[row, 'KeyGroup']:
+            if "VARIANT" in summary.loc[row, "KeyGroup"]:
                 renamed = True
 
             # if NumVolumes is nan, set to 1.0
             # if 'NumVolumes' in summary.columns \
             #         and str(summary.loc[row, "NumVolumes"]) == 'nan':
             #     summary.at[row, "NumVolumes"] = 1.0
 
             if summary.loc[row, "ParamGroup"] != 1 and not renamed:
-                acq_str = 'VARIANT'
+                acq_str = "VARIANT"
                 # now we know we have a deviant param group
                 # check if TR is same as param group 1
                 key = summary.loc[row, "KeyGroup"]
                 for col in rename_cols:
                     summary[col] = summary[col].apply(str)
                     if summary.loc[row, col] != dom_dict[key][col]:
-
-                        if col == 'HasFieldmap':
-                            if dom_dict[key][col] == 'True':
-                                acq_str = acq_str + 'NoFmap'
+                        if col == "HasFieldmap":
+                            if dom_dict[key][col] == "True":
+                                acq_str = acq_str + "NoFmap"
                             else:
-                                acq_str = acq_str + 'HasFmap'
-                        elif col == 'UsedAsFieldmap':
-                            if dom_dict[key][col] == 'True':
-                                acq_str = acq_str + 'Unused'
+                                acq_str = acq_str + "HasFmap"
+                        elif col == "UsedAsFieldmap":
+                            if dom_dict[key][col] == "True":
+                                acq_str = acq_str + "Unused"
                             else:
-                                acq_str = acq_str + 'IsUsed'
+                                acq_str = acq_str + "IsUsed"
                         else:
                             acq_str = acq_str + col
 
-                if acq_str == 'VARIANT':
-                    acq_str = acq_str + 'Other'
+                if acq_str == "VARIANT":
+                    acq_str = acq_str + "Other"
 
-                if 'acquisition' in entities.keys():
-                    acq = 'acquisition-%s' % entities['acquisition'] + acq_str
+                if "acquisition" in entities.keys():
+                    acq = f"acquisition-{entities['acquisition'] + acq_str}"
 
                     new_name = summary.loc[row, "KeyGroup"].replace(
-                            'acquisition-%s' % entities['acquisition'], acq)
+                        f"acquisition-{entities['acquisition']}",
+                        acq,
+                    )
                 else:
-                    acq = 'acquisition-%s' % acq_str
-                    new_name = acq + '_' + summary.loc[row, "KeyGroup"]
+                    acq = f"acquisition-{acq_str}"
+                    new_name = acq + "_" + summary.loc[row, "KeyGroup"]
 
-                summary.at[row, 'RenameKeyGroup'] = new_name
+                summary.at[row, "RenameKeyGroup"] = new_name
 
             # convert all "nan" to empty str
             # so they don't show up in the summary tsv
-            if summary.loc[row, "RenameKeyGroup"] == 'nan':
-                summary.at[row, "RenameKeyGroup"] = ''
+            if summary.loc[row, "RenameKeyGroup"] == "nan":
+                summary.at[row, "RenameKeyGroup"] = ""
 
             for col in rename_cols:
-                if summary.loc[row, col] == 'nan':
-                    summary.at[row, col] = ''
+                if summary.loc[row, col] == "nan":
+                    summary.at[row, col] = ""
 
         return (big_df, summary)
 
-    def get_TSVs(self, path_prefix):
-        """Creates the _summary and _files tsvs for the bids dataset.
+    def get_tsvs(self, path_prefix):
+        """Create the _summary and _files tsvs for the bids dataset.
 
-        Parameters:
-        -----------
-            prefix_path: str
-                prefix of the path to the directory where you want
-                to save your tsvs
-                example path: /Users/Covitz/PennLINC/RBC/CCNP/
+        Parameters
+        ----------
+        path_prefix : str
+            prefix of the path to the directory where you want
+            to save your tsvs
+            example path: /Users/Covitz/PennLINC/RBC/CCNP/
         """
-
         self._cache_fieldmaps()
 
         # check if path_prefix is absolute or relative
         # if relative, put output in BIDS_ROOT/code/CuBIDS/ dir
-        if '/' not in path_prefix:
+        if "/" not in path_prefix:
             # path is relative
             # first check if code/CuBIDS dir exits
             # if not, create it
             self.create_cubids_code_dir()
             # send outputs to code/CuBIDS in BIDS tree
-            path_prefix = self.path + '/code/CuBIDS/' + path_prefix
+            path_prefix = self.path + "/code/CuBIDS/" + path_prefix
 
         big_df, summary = self.get_param_groups_dataframes()
 
-        summary = summary.sort_values(by=['Modality', 'KeyGroupCount'],
-                                      ascending=[True, False])
-        big_df = big_df.sort_values(by=['Modality', 'KeyGroupCount'],
-                                    ascending=[True, False])
+        summary = summary.sort_values(by=["Modality", "KeyGroupCount"], ascending=[True, False])
+        big_df = big_df.sort_values(by=["Modality", "KeyGroupCount"], ascending=[True, False])
 
         # Create json dictionaries for summary and files tsvs
         self.create_data_dictionary()
         files_dict = self.get_data_dictionary(big_df)
         summary_dict = self.get_data_dictionary(summary)
 
         # Save data dictionaires as JSONs
-        with open(path_prefix + "_files.json", "w") as outfile:
+        with open(f"{path_prefix}_files.json", "w") as outfile:
             json.dump(files_dict, outfile, indent=4)
 
-        with open(path_prefix + "_summary.json", "w") as outfile:
+        with open(f"{path_prefix}_summary.json", "w") as outfile:
             json.dump(summary_dict, outfile, indent=4)
 
-        big_df.to_csv(path_prefix + "_files.tsv", sep="\t", index=False)
+        big_df.to_csv(f"{path_prefix}_files.tsv", sep="\t", index=False)
 
-        summary.to_csv(path_prefix + "_summary.tsv", sep="\t", index=False)
+        summary.to_csv(f"{path_prefix}_summary.tsv", sep="\t", index=False)
 
         # Calculate the acq groups
-        group_by_acquisition_sets(path_prefix + "_files.tsv", path_prefix,
-                                  self.acq_group_level)
+        group_by_acquisition_sets(f"{path_prefix}_files.tsv", path_prefix, self.acq_group_level)
 
-        print("CuBIDS detected " + str(len(summary)) + " Parameter Groups.")
+        print(f"CuBIDS detected {len(summary)} Parameter Groups.")
 
     def get_key_groups(self):
-        '''Identifies the key groups for the bids dataset'''
-
+        """Identify the key groups for the bids dataset."""
         # reset self.keys_files
         self.keys_files = {}
 
         key_groups = set()
 
         for path in Path(self.path).rglob("sub-*/**/*.*"):
             # ignore all dot directories
-            if '/.' in str(path):
+            if "/." in str(path):
                 continue
 
             if str(path).endswith(".nii") or str(path).endswith(".nii.gz"):
                 key_groups.update((_file_to_key_group(path),))
 
                 # Fill the dictionary of key group, list of filenames pairrs
                 ret = _file_to_key_group(path)
 
                 if ret not in self.keys_files.keys():
-
                     self.keys_files[ret] = []
 
                 self.keys_files[ret].append(path)
 
         return sorted(key_groups)
 
-    def change_metadata(self, filters, pattern, metadata):
+    def change_metadata(self, filters, metadata):
+        """Change metadata.
 
-        files_to_change = self.layout.get(return_type='object', **filters)
+        NOTE: Appears unused.
+        """
+        files_to_change = self.layout.get(return_type="object", **filters)
 
         for bidsfile in files_to_change:
             # get the sidecar file
             # bidsjson_file = bidsfile.get_associations()
-            bidsjson_file = img_to_new_ext(str(bidsfile), '.json')
+            bidsjson_file = img_to_new_ext(str(bidsfile), ".json")
             if not bidsjson_file:
                 print("NO JSON FILES FOUND IN ASSOCIATIONS")
                 continue
 
-            json_file = [x for x in bidsjson_file if 'json' in x.filename]
+            json_file = [x for x in bidsjson_file if "json" in x.filename]
             if not len(json_file) == 1:
                 print("FOUND IRREGULAR ASSOCIATIONS")
 
             else:
                 # get the data from it
                 json_file = json_file[0]
 
                 sidecar = json_file.get_dict()
                 sidecar.update(metadata)
 
                 # write out
                 _update_json(json_file.path, sidecar)
 
     def get_all_metadata_fields(self):
-        ''' Returns all metadata fields in a bids directory'''
-
+        """Return all metadata fields in a bids directory."""
         found_fields = set()
         for json_file in Path(self.path).rglob("*.json"):
-            if '.git' not in str(json_file):
+            if ".git" not in str(json_file):
                 with open(json_file, "r") as jsonr:
                     metadata = json.load(jsonr)
                 found_fields.update(metadata.keys())
         return sorted(found_fields)
 
     def remove_metadata_fields(self, fields_to_remove):
-        '''Removes specific fields from all metadata files.'''
-
+        """Remove specific fields from all metadata files."""
         remove_fields = set(fields_to_remove)
         if not remove_fields:
             return
+
         for json_file in tqdm(Path(self.path).rglob("*.json")):
             # Check for offending keys in the json file
-            if '.git' not in str(json_file):
+            if ".git" not in str(json_file):
                 with open(json_file, "r") as jsonr:
                     metadata = json.load(jsonr)
+
                 offending_keys = remove_fields.intersection(metadata.keys())
                 # Quit if there are none in there
                 if not offending_keys:
                     continue
 
                 # Remove the offending keys
                 for key in offending_keys:
                     del metadata[key]
                 # Write the cleaned output
                 with open(json_file, "w") as jsonr:
                     json.dump(metadata, jsonr, indent=4)
 
     # # # # FOR TESTING # # # #
     def get_filenames(self):
+        """Get filenames."""
         return self.keys_files
 
     def get_fieldmap_lookup(self):
+        """Get fieldmap lookup."""
         return self.fieldmap_lookup
 
     def get_layout(self):
+        """Get layout."""
         return self.layout
 
 
-def _validateJSON(json_file):
+def _validate_json():
+    """Validate a JSON file's contents.
+
+    This is currently not implemented, but would accept metadata as its param.
+    """
     # TODO: implement this or delete ???
     return True
 
 
 def _update_json(json_file, metadata):
-
-    if _validateJSON(metadata):
-        with open(json_file, 'w', encoding='utf-8') as f:
+    if _validate_json():
+        with open(json_file, "w", encoding="utf-8") as f:
             json.dump(metadata, f, ensure_ascii=False, indent=4)
     else:
         print("INVALID JSON DATA")
 
 
 def _key_group_to_entities(key_group):
-    '''Splits a key_group name into a pybids dictionary of entities.'''
-
+    """Split a key_group name into a pybids dictionary of entities."""
     return dict([group.split("-") for group in key_group.split("_")])
 
 
 def _entities_to_key_group(entities):
-    '''Converts a pybids entities dictionary into a key group name.'''
-
+    """Convert a pybids entities dictionary into a key group name."""
     group_keys = sorted(entities.keys() - NON_KEY_ENTITIES)
-    return "_".join(
-        ["{}-{}".format(key, entities[key]) for key in group_keys])
+    return "_".join([f"{key}-{entities[key]}" for key in group_keys])
 
 
 def _file_to_key_group(filename):
-    '''Identifies and returns the key group of a bids valid filename.'''
-
+    """Identify and return the key group of a bids valid filename."""
     entities = parse_file_entities(str(filename))
     return _entities_to_key_group(entities)
 
 
 def _get_intended_for_reference(scan):
-    return '/'.join(Path(scan).parts[-3:])
-
+    return "/".join(Path(scan).parts[-3:])
 
-def _get_param_groups(files, layout, fieldmap_lookup, key_group_name,
-                      grouping_config, modality, keys_files):
 
-    """Finds a list of *parameter groups* from a list of files.
+def _get_param_groups(
+    files,
+    fieldmap_lookup,
+    key_group_name,
+    grouping_config,
+    modality,
+    keys_files,
+):
+    """Find a list of *parameter groups* from a list of files.
 
     For each file in `files`, find critical parameters for metadata. Then find
     unique sets of these critical parameters.
 
-    Parameters:
-    -----------
-    files : list
+    Parameters
+    ----------
+    files : :obj:`list` of :obj:`str`
         List of file names
-
-    layout : bids.BIDSLayout
-        PyBIDS BIDSLayout object where `files` come from
-
-    fieldmap_lookup : defaultdict
+    fieldmap_lookup : :obj:`dict`
         mapping of filename strings relative to the bids root
         (e.g. "sub-X/ses-Y/func/sub-X_ses-Y_task-rest_bold.nii.gz")
-
-    grouping_config : dict
+    grouping_config : :obj:`dict`
         configuration for defining parameter groups
 
-    Returns:
-    --------
-    labeled_files : pd.DataFrame
+    Returns
+    -------
+    labeled_files : :obj:`pandas.DataFrame`
         A data frame with one row per file where the ParamGroup column
         indicates which group each scan is a part of.
-
-    param_groups_with_counts : pd.DataFrame
-        A data frame with param group summaries
-
+    param_groups_with_counts : :obj:`pandas.DataFrame`
+        A data frame with param group summaries.
     """
-
     if not files:
         print("WARNING: no files for", key_group_name)
         return None, None
 
     # Split the config into separate parts
-    imaging_params = grouping_config.get('sidecar_params', {})
+    imaging_params = grouping_config.get("sidecar_params", {})
     imaging_params = imaging_params[modality]
 
-    relational_params = grouping_config.get('relational_params', {})
+    relational_params = grouping_config.get("relational_params", {})
 
-    derived_params = grouping_config.get('derived_params')
+    derived_params = grouping_config.get("derived_params")
     derived_params = derived_params[modality]
 
     imaging_params.update(derived_params)
 
     dfs = []
     # path needs to be relative to the root with no leading prefix
 
     for path in files:
         # metadata = layout.get_metadata(path)
-        metadata = get_sidecar_metadata(img_to_new_ext(path, '.json'))
+        metadata = get_sidecar_metadata(img_to_new_ext(path, ".json"))
         if metadata == "Erroneous sidecar":
-            print('Error parsing sidecar: ', img_to_new_ext(path, '.json'))
+            print("Error parsing sidecar: ", img_to_new_ext(path, ".json"))
         else:
             intentions = metadata.get("IntendedFor", [])
             slice_times = metadata.get("SliceTiming", [])
 
             wanted_keys = metadata.keys() & imaging_params
             example_data = {key: metadata[key] for key in wanted_keys}
             example_data["KeyGroup"] = key_group_name
 
             # Get the fieldmaps out and add their types
-            if 'FieldmapKey' in relational_params:
-                fieldmap_types = sorted([_file_to_key_group(fmap.path) for
-                                        fmap in fieldmap_lookup[path]])
+            if "FieldmapKey" in relational_params:
+                fieldmap_types = sorted(
+                    [_file_to_key_group(fmap.path) for fmap in fieldmap_lookup[path]]
+                )
 
                 # check if config says columns or bool
-                if relational_params['FieldmapKey']['display_mode'] == \
-                        'bool':
+                if relational_params["FieldmapKey"]["display_mode"] == "bool":
                     if len(fieldmap_types) > 0:
-                        example_data['HasFieldmap'] = True
+                        example_data["HasFieldmap"] = True
                     else:
-                        example_data['HasFieldmap'] = False
+                        example_data["HasFieldmap"] = False
                 else:
                     for fmap_num, fmap_type in enumerate(fieldmap_types):
-                        example_data['FieldmapKey%02d' % fmap_num] = fmap_type
+                        example_data[f"FieldmapKey{fmap_num:02d}"] = fmap_type
 
             # Add the number of slice times specified
             if "NSliceTimes" in derived_params:
                 example_data["NSliceTimes"] = len(slice_times)
 
             example_data["FilePath"] = path
 
             # If it's a fieldmap, see what key group it's intended to correct
             if "IntendedForKey" in relational_params:
-                intended_key_groups = sorted([_file_to_key_group(intention) for
-                                             intention in intentions])
+                intended_key_groups = sorted(
+                    [_file_to_key_group(intention) for intention in intentions]
+                )
 
                 # check if config says columns or bool
-                if relational_params['IntendedForKey']['display_mode'] == \
-                        'bool':
+                if relational_params["IntendedForKey"]["display_mode"] == "bool":
                     if len(intended_key_groups) > 0:
                         example_data["UsedAsFieldmap"] = True
                     else:
                         example_data["UsedAsFieldmap"] = False
                 else:
-                    for intention_num, intention_key_group in \
-                            enumerate(intended_key_groups):
-                        example_data[
-                            "IntendedForKey%02d" % intention_num] = \
-                                    intention_key_group
+                    for intention_num, intention_key_group in enumerate(intended_key_groups):
+                        example_data[f"IntendedForKey{intention_num:02d}"] = intention_key_group
 
             dfs.append(example_data)
 
     # Assign each file to a ParamGroup
 
     # round param groups based on precision
     df = round_params(pd.DataFrame(dfs), grouping_config, modality)
@@ -1418,20 +1525,20 @@
     # cluster param groups based on tolerance
     df = format_params(df, grouping_config, modality)
     # param_group_cols = list(set(df.columns.to_list()) - set(["FilePath"]))
 
     # get the subset of columns to drop duplicates by
     check_cols = []
     for col in list(df.columns):
-        if "Cluster_" + col not in list(df.columns) and col != 'FilePath':
+        if f"Cluster_{col}" not in list(df.columns) and col != "FilePath":
             check_cols.append(col)
 
     # Find the unique ParamGroups and assign ID numbers in "ParamGroup"\
     try:
-        deduped = df.drop('FilePath', axis=1)
+        deduped = df.drop("FilePath", axis=1)
     except Exception:
         return "erroneous sidecar found"
 
     deduped = deduped.drop_duplicates(subset=check_cols, ignore_index=True)
     deduped["ParamGroup"] = np.arange(deduped.shape[0]) + 1
 
     # add the modality as a column
@@ -1442,129 +1549,182 @@
 
     # Add the ParamGroup to the whole list of files
     labeled_files = pd.merge(df, deduped, on=check_cols)
 
     value_counts = labeled_files.ParamGroup.value_counts()
 
     param_group_counts = pd.DataFrame(
-        {"Counts": value_counts.to_numpy(),
-         "ParamGroup": value_counts.index.to_numpy()})
+        {"Counts": value_counts.to_numpy(), "ParamGroup": value_counts.index.to_numpy()}
+    )
 
-    param_groups_with_counts = pd.merge(
-        deduped, param_group_counts, on=["ParamGroup"])
+    param_groups_with_counts = pd.merge(deduped, param_group_counts, on=["ParamGroup"])
 
     # Sort by counts and relabel the param groups
-    param_groups_with_counts.sort_values(by=['Counts'], inplace=True,
-                                         ascending=False)
-    param_groups_with_counts["ParamGroup"] = np.arange(
-        param_groups_with_counts.shape[0]) + 1
+    param_groups_with_counts.sort_values(by=["Counts"], inplace=True, ascending=False)
+    param_groups_with_counts["ParamGroup"] = np.arange(param_groups_with_counts.shape[0]) + 1
 
     # Send the new, ordered param group ids to the files list
-    ordered_labeled_files = pd.merge(df, param_groups_with_counts,
-                                     on=check_cols, suffixes=('_x', ''))
+    ordered_labeled_files = pd.merge(
+        df, param_groups_with_counts, on=check_cols, suffixes=("_x", "")
+    )
 
     # sort ordered_labeled_files by param group
-    ordered_labeled_files.sort_values(by=['Counts'], inplace=True,
-                                      ascending=False)
+    ordered_labeled_files.sort_values(by=["Counts"], inplace=True, ascending=False)
 
     # now get rid of cluster cols from deduped and df
     for col in list(ordered_labeled_files.columns):
-        if col.startswith('Cluster_'):
+        if col.startswith("Cluster_"):
             ordered_labeled_files = ordered_labeled_files.drop(col, axis=1)
-            param_groups_with_counts = param_groups_with_counts.drop(col,
-                                                                     axis=1)
-        if col.endswith('_x'):
+            param_groups_with_counts = param_groups_with_counts.drop(col, axis=1)
+        if col.endswith("_x"):
             ordered_labeled_files = ordered_labeled_files.drop(col, axis=1)
 
     return ordered_labeled_files, param_groups_with_counts
 
 
 def round_params(param_group_df, config, modality):
-    to_format = config['sidecar_params'][modality]
-    to_format.update(config['derived_params'][modality])
+    """Round columns' values in DataFrame according to requested precision."""
+    to_format = config["sidecar_params"][modality]
+    to_format.update(config["derived_params"][modality])
 
     for column_name, column_fmt in to_format.items():
         if column_name not in param_group_df:
             continue
-        if 'precision' in column_fmt:
+
+        if "precision" in column_fmt:
             if isinstance(param_group_df[column_name], float):
-                param_group_df[column_name] = \
-                    param_group_df[column_name].round(column_fmt['precision'])
+                param_group_df[column_name] = param_group_df[column_name].round(
+                    column_fmt["precision"]
+                )
 
     return param_group_df
 
 
 def get_sidecar_metadata(json_file):
-    # get all metadata values in a file's sidecar
-    # transform json dictionary to python dictionary
+    """Get all metadata values in a file's sidecar.
+
+    Transform json dictionary to Python dictionary.
+    """
     try:
         with open(json_file) as json_file:
             data = json.load(json_file)
             return data
     except Exception:
         # print("Error loading sidecar: ", json_filename)
         return "Erroneous sidecar"
 
 
 def format_params(param_group_df, config, modality):
-    '''Run AgglomerativeClustering on param groups, add columns to dataframe'''
+    """Run AgglomerativeClustering on param groups and add columns to dataframe.
 
-    to_format = config['sidecar_params'][modality]
-    to_format.update(config['derived_params'][modality])
+    Parameters
+    ----------
+    param_group_df : :obj:`pandas.DataFrame`
+        A data frame with one row per file where the ParamGroup column
+        indicates which group each scan is a part of.
+    config : :obj:`dict`
+        Configuration for defining parameter groups.
+        This dictionary has two keys: ``'sidecar_params'`` and ``'derived_params'``.
+    modality : :obj:`str`
+        Modality of the scan.
+        This is used to select the correct configuration from the config dict.
+
+    Returns
+    -------
+    param_group_df : :obj:`pandas.DataFrame`
+        An updated version of the input data frame,
+        with a new column added for each element in the modality's
+        ``'sidecar_params'`` and ``'derived_params'`` dictionaries.
+        The new columns will have the name ``'Cluster_' + column_name``,
+        and will contain the cluster labels for each parameter group.
+
+    Notes
+    -----
+    ``'sidecar_params'`` is a dictionary of dictionaries, where keys are modalities.
+    The modality-wise dictionary's keys are names of BIDS fields to directly include
+    in the Parameter Groupings,
+    and the values describe the parameters by which those BIDS' fields are compared.
+    For example,
+    {"RepetitionTime": {"tolerance": 0.000001, "precision": 6, "suggest_variant_rename": True}
+    means that the RepetitionTime field should be compared across files and flagged as a
+    variant if it differs from others by 0.000001 or more.
+
+    ``'derived_params'`` is a dictionary of dictionaries, where keys are modalities.
+    The modality-wise dictionary's keys are names of BIDS fields to derive from the
+    NIfTI header and include in the Parameter Groupings.
+    """
+    to_format = config["sidecar_params"][modality]
+    to_format.update(config["derived_params"][modality])
 
     for column_name, column_fmt in to_format.items():
         if column_name not in param_group_df:
             continue
-        if 'tolerance' in column_fmt and len(param_group_df) > 1:
+
+        if "tolerance" in column_fmt and len(param_group_df) > 1:
             array = param_group_df[column_name].to_numpy().reshape(-1, 1)
 
             for i in range(len(array)):
                 if np.isnan(array[i, 0]):
                     array[i, 0] = -999
 
-            tolerance = to_format[column_name]['tolerance']
-            clustering = AgglomerativeClustering(n_clusters=None,
-                                                 distance_threshold=tolerance,
-                                                 linkage='complete').fit(array)
+            tolerance = to_format[column_name]["tolerance"]
+            clustering = AgglomerativeClustering(
+                n_clusters=None, distance_threshold=tolerance, linkage="complete"
+            ).fit(array)
+
             for i in range(len(array)):
                 if array[i, 0] == -999:
                     array[i, 0] = np.nan
 
             # now add clustering_labels as a column
-            param_group_df['Cluster_' + column_name] = clustering.labels_
+            param_group_df[f"Cluster_{column_name}"] = clustering.labels_
 
     return param_group_df
 
 
 def _order_columns(df):
-    '''Organizes columns of the summary and files DataFrames so that
-    KeyGroup and ParamGroup are the first two columns, FilePath is
-    the last, and the others are sorted alphabetically.'''
+    """Organize columns of the summary and files DataFrames.
 
+    This ensures that KeyGroup and ParamGroup are the first two columns,
+    FilePath is the last, and the others are sorted alphabetically.
+
+    Notes
+    -----
+    This is the only place where the constant ID_VARS is used,
+    and the strings in that constant are hardcoded here,
+    so we might not need that constant at all.
+    """
     cols = set(df.columns.to_list())
     non_id_cols = cols - ID_VARS
     new_columns = ["KeyGroup", "ParamGroup"] + sorted(non_id_cols)
     if "FilePath" in cols:
         new_columns.append("FilePath")
 
     df = df[new_columns]
 
     return df[new_columns]
 
 
 def img_to_new_ext(img_path, new_ext):
+    """Convert img to new extension.
+
+    Notes
+    -----
+    The hardcoded suffix associated with each extension may not be comprehensive.
+    BIDS has been extended a lot in recent years.
+    """
     # handle .tsv edge case
-    if new_ext == '.tsv':
+    if new_ext == ".tsv":
         # take out suffix
-        return img_path.rpartition('_')[0] + '_events' + new_ext
-    if new_ext == '.tsv.gz':
-        return img_path.rpartition('_')[0] + '_physio' + new_ext
+        return img_path.rpartition("_")[0] + "_events" + new_ext
+    elif new_ext == ".tsv.gz":
+        return img_path.rpartition("_")[0] + "_physio" + new_ext
     else:
         return img_path.replace(".nii.gz", "").replace(".nii", "") + new_ext
 
 
 def get_key_name(path, key):
-    # given a filepath and BIDS key name, return value
+    """Given a filepath and BIDS key name, return value."""
     parts = Path(path).parts
     for part in parts:
-        if part.startswith(key + '-'):
+        if part.startswith(key + "-"):
             return part
```

### Comparing `cubids-1.0.9/cubids/data/config.yml` & `cubids-1.1.0/cubids/data/config.yml`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,42 @@
 # These are non-BIDS fields that can be added by CuBIDS
 derived_params:
   anat:
+    # Number of voxels in first dimension
     Dim1Size:
       suggest_variant_rename: yes
+    # Number of voxels in second dimension
     Dim2Size:
       suggest_variant_rename: yes
+    # Number of voxels in third dimension
     Dim3Size:
       suggest_variant_rename: yes
+    # Number of slice time values
     NSliceTimes:
       suggest_variant_rename: yes
+    # Number of volumes
     NumVolumes:
       suggest_variant_rename: yes
+    # Boolean indicating oblique acquisition
     Obliquity:
       suggest_variant_rename: yes
+    # String describing image orientation (e.g., LAS+)
     ImageOrientation:
       suggest_variant_rename: yes
+    # Size of voxels in first dimension, in mm
     VoxelSizeDim1:
       tolerance: 0.001
       precision: 3
       suggest_variant_rename: yes
+    # Size of voxels in second dimension, in mm
     VoxelSizeDim2:
       tolerance: 0.001
       precision: 3
       suggest_variant_rename: yes
+    # Size of voxels in third dimension, in mm
     VoxelSizeDim3:
       tolerance: 0.001
       precision: 3
       suggest_variant_rename: yes
   dwi:
     Dim1Size:
       suggest_variant_rename: yes
@@ -329,48 +339,77 @@
       precision: 3
       suggest_variant_rename: yes
     VolumeTiming:
       tolerance: 0.000001
       precision: 6
       suggest_variant_rename: yes
   perf:
+    ArterialSpinLabelingType:
+      suggest_variant_rename: yes
+    BackgroundSuppression:
+      suggest_variant_rename: yes
+    BackgroundSuppressionNumberPulses:
+      suggest_variant_rename: yes
+    BolusCutOffFlag:
+      suggest_variant_rename: yes
+    BolusCutOffTechnique:
+      suggest_variant_rename: yes
+    CASLType:
+      suggest_variant_rename: yes
     EchoTime:
       tolerance: 0.001
       precision: 3
       suggest_variant_rename: yes
     EffectiveEchoSpacing:
       tolerance: 0.00001
       precision: 5
       suggest_variant_rename: yes
     FlipAngle:
       suggest_variant_rename: yes
+    LabelingDistance:
+      tolerance: 0.1
+      suggest_variant_rename: yes
+    LabelingEfficiency:
+      tolerance: 0.001
+      precision: 3
+      suggest_variant_rename: yes
+    LookLocker:
+      suggest_variant_rename: yes
+    M0Type:
+      suggest_variant_rename: yes
     MultibandAccelerationFactor:
       suggest_variant_rename: yes
     NumberOfVolumesDiscardedByScanner:
       suggest_variant_rename: yes
     NumberOfVolumesDiscardedByUser:
       suggest_variant_rename: yes
     ParallelAcquisitionTechnique:
       suggest_variant_rename: yes
     ParallelReductionFactorInPlane:
       suggest_variant_rename: yes
     PartialFourier:
       suggest_variant_rename: yes
+    PASLType:
+      suggest_variant_rename: yes
+    PCASLType:
+      suggest_variant_rename: yes
     PhaseEncodingDirection:
       suggest_variant_rename: yes
     RepetitionTime:
       tolerance: 0.000001
       precision: 6
       suggest_variant_rename: yes
     SliceEncodingDirection:
       suggest_variant_rename: yes
     TotalReadoutTime:
       tolerance: 0.001
       precision: 3
       suggest_variant_rename: yes
+    VascularCrushing:
+      suggest_variant_rename: yes
     VolumeTiming:
       tolerance: 0.000001
       precision: 6
       suggest_variant_rename: yes
   other:
     EchoTime:
       tolerance: 0.001
@@ -405,8 +444,8 @@
     TotalReadoutTime:
       tolerance: 0.001
       precision: 3
       suggest_variant_rename: yes
     VolumeTiming:
       tolerance: 0.000001
       precision: 6
-      suggest_variant_rename: yes
+      suggest_variant_rename: yes
```

### Comparing `cubids-1.0.9/cubids/metadata_merge.py` & `cubids-1.1.0/cubids/metadata_merge.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,214 +1,312 @@
-"""Main module."""
+"""Tools for merging metadata."""
+
 import json
 from collections import defaultdict
+from copy import deepcopy
+from math import isnan, nan
+
 import numpy as np
 import pandas as pd
-from copy import deepcopy
-from math import nan, isnan
-from .constants import IMAGING_PARAMS
+
+from cubids.constants import IMAGING_PARAMS
+
 DIRECT_IMAGING_PARAMS = IMAGING_PARAMS - set(["NSliceTimes"])
 
 
 def check_merging_operations(action_tsv, raise_on_error=False):
-    """Checks that the merges in an action tsv are possible.
+    """Check that the merges in an action tsv are possible.
 
-    To be mergable the
+    Parameters
+    ----------
+    action_tsv : :obj:`str`
+        Path to the action tsv file.
+    raise_on_error : :obj:`bool`, optional
+        Whether to raise an exception if there are errors.
+
+    Returns
+    -------
+    ok_merges : :obj:`list`
+        List of tuples of ok merges.
+    deletions : :obj:`list`
+        List of tuples of deletions.
+
+    Raises
+    ------
+    :obj:`Exception`
+        If there are errors and ``raise_on_error`` is ``True``.
     """
     actions = pd.read_table(action_tsv)
     ok_merges = []
     deletions = []
     overwrite_merges = []
     sdc_incompatible = []
 
-    sdc_cols = set([col for col in actions.columns if
-                    col.startswith("IntendedForKey") or
-                    col.startswith("FieldmapKey")])
+    sdc_cols = set(
+        [
+            col
+            for col in actions.columns
+            if col.startswith("IntendedForKey") or col.startswith("FieldmapKey")
+        ]
+    )
 
     def _check_sdc_cols(meta1, meta2):
-        return {key: meta1[key] for key in sdc_cols} == \
-               {key: meta2[key] for key in sdc_cols}
+        return {key: meta1[key] for key in sdc_cols} == {key: meta2[key] for key in sdc_cols}
 
-    needs_merge = actions[np.isfinite(actions['MergeInto'])]
+    needs_merge = actions[np.isfinite(actions["MergeInto"])]
     for _, row_needs_merge in needs_merge.iterrows():
         source_param_key = tuple(row_needs_merge[["MergeInto", "KeyGroup"]])
         dest_param_key = tuple(row_needs_merge[["ParamGroup", "KeyGroup"]])
         dest_metadata = row_needs_merge.to_dict()
-        source_row = actions.loc[
-            (actions[["ParamGroup", "KeyGroup"]] == source_param_key).all(1)]
+        source_row = actions.loc[(actions[["ParamGroup", "KeyGroup"]] == source_param_key).all(1)]
 
         if source_param_key[0] == 0:
             print("going to delete ", dest_param_key)
             deletions.append(dest_param_key)
             continue
+
         if not source_row.shape[0] == 1:
             raise Exception("Could not identify a unique source group")
+
         source_metadata = source_row.iloc[0].to_dict()
         merge_id = (source_param_key, dest_param_key)
         # Check for compatible fieldmaps
         if not _check_sdc_cols(source_metadata, dest_metadata):
             sdc_incompatible.append(merge_id)
             continue
 
-        if not merge_without_overwrite(source_metadata, dest_metadata,
-                                       raise_on_error=raise_on_error):
+        if not merge_without_overwrite(
+            source_metadata, dest_metadata, raise_on_error=raise_on_error
+        ):
             overwrite_merges.append(merge_id)
             continue
+
         # add to the list of ok merges if there are no conflicts
         ok_merges.append(merge_id)
 
-    error_message = "\n\nProblems were found in the requested merge.\n" \
-                    "===========================================\n\n"
+    error_message = (
+        "\n\nProblems were found in the requested merge.\n"
+        "===========================================\n\n"
+    )
     if sdc_incompatible:
-        error_message += "Some merges are incompatible due to differing " \
-                         "distortion correction strategies. Check that " \
-                         "fieldmaps exist and have the correct " \
-                         "\"IntendedFor\" in their sidecars. These merges " \
-                         "could not be completed:\n"
+        error_message += (
+            "Some merges are incompatible due to differing "
+            "distortion correction strategies. Check that "
+            "fieldmaps exist and have the correct "
+            '"IntendedFor" in their sidecars. These merges '
+            "could not be completed:\n"
+        )
         error_message += print_merges(sdc_incompatible) + "\n\n"
 
     if overwrite_merges:
-        error_message += "Some merges are incompatible because the metadata " \
-                         "in the destination json conflicts with the values " \
-                         "in the source json. Merging should only be used " \
-                         "to fill in missing metadata. The following " \
-                         "merges could not be completed:\n\n"
+        error_message += (
+            "Some merges are incompatible because the metadata "
+            "in the destination json conflicts with the values "
+            "in the source json. Merging should only be used "
+            "to fill in missing metadata. The following "
+            "merges could not be completed:\n\n"
+        )
         error_message += print_merges(overwrite_merges)
 
     if overwrite_merges or sdc_incompatible:
         if raise_on_error:
             raise Exception(error_message)
+
         print(error_message)
+
     return ok_merges, deletions
 
 
 def merge_without_overwrite(source_meta, dest_meta_orig, raise_on_error=False):
-    """Performs a safe metadata copy.
+    """Perform a safe metadata copy.
 
     Here, "safe" means that no non-NaN values in `dest_meta` are
     overwritten by the merge. If any overwrites occur an empty
     dictionary is returned.
+
+    Parameters
+    ----------
+    source_meta : :obj:`dict`
+        The metadata to merge from.
+    dest_meta_orig : :obj:`dict`
+        The metadata to merge into.
+    raise_on_error : :obj:`bool`, optional
+        Whether to raise an exception if there are errors.
+
+    Returns
+    -------
+    :obj:`dict`
+        The merged metadata.
+
+    Raises
+    ------
+    :obj:`Exception`
+        If there are errors and ``raise_on_error`` is ``True``.
     """
     # copy the original json params
     dest_meta = deepcopy(dest_meta_orig)
 
     if not source_meta.get("NSliceTimes") == dest_meta.get("NSliceTimes"):
         if raise_on_error:
-            raise Exception("Value for NSliceTimes is %d in destination "
-                            "but %d in source"
-                            % (source_meta.get("NSliceTimes"),
-                               source_meta.get("NSliceTimes")))
+            raise Exception(
+                "Value for NSliceTimes is %d in destination "
+                "but %d in source"
+                % (source_meta.get("NSliceTimes"), source_meta.get("NSliceTimes"))
+            )
         return {}
+
     for parameter in DIRECT_IMAGING_PARAMS:
         source_value = source_meta.get(parameter, nan)
         dest_value = dest_meta.get(parameter, nan)
 
         # cannot merge num --> num
         # exception should only be raised
         # IF someone tries to replace a num (dest)
         # with a num (src)
         if not is_nan(source_value):
             # need to figure out if we can merge
             if not is_nan(dest_value) and source_value != dest_value:
                 if raise_on_error:
-                    raise Exception("Value for %s is %s in destination "
-                                    "but %s in source"
-                                    % (parameter, str(dest_value),
-                                       str(source_value)))
+                    raise Exception(
+                        f"Value for {parameter} is {dest_value} in destination "
+                        f"but {source_value} in source"
+                    )
+
                 return {}
+
         dest_meta[parameter] = source_value
+
     return dest_meta
 
 
 def is_nan(val):
-    '''Returns True if val is nan'''
+    """Return True if val is NaN."""
     if not isinstance(val, float):
         return False
+
     return isnan(val)
 
 
 def print_merges(merge_list):
-    """Print formatted text of merges"""
-    return "\n\t" + "\n\t".join(
-        ["%s \n\t\t-> %s" % ("%s:%d" % src_id[::-1],
-         "%s:%d" % dest_id[::-1]) for
-         src_id, dest_id in merge_list])
-
-
-def merge_json_into_json(from_file, to_file,
-                         raise_on_error=False):
-    print("Merging imaging metadata from %s to %s"
-          % (from_file, to_file))
+    """Print formatted text of merges."""
+    merge_strings = []
+    for src_id, dest_id in merge_list:
+        src_id_str = f"{src_id[-1]}:{src_id[0]}"
+        dest_id_str = f"{dest_id[-1]}:{dest_id[0]}"
+        merge_str = f"{src_id_str} \n\t\t-> {dest_id_str}"
+        merge_strings.append(merge_str)
+
+    return "\n\t" + "\n\t".join(merge_strings)
+
+
+def merge_json_into_json(from_file, to_file, raise_on_error=False):
+    """Merge imaging metadata into JSON.
+
+    Parameters
+    ----------
+    from_file : :obj:`str`
+        Path to the JSON file to merge from.
+    to_file : :obj:`str`
+        Path to the JSON file to merge into.
+    raise_on_error : :obj:`bool`, optional
+        Whether to raise an exception if there are errors.
+        Defaults to ``False``.
+
+    Returns
+    -------
+    :obj:`int`
+        Exit code.
+        Either 255 if there was an error or 0 if there was not.
+    """
+    print(f"Merging imaging metadata from {from_file} to {to_file}")
     with open(from_file, "r") as fromf:
         source_metadata = json.load(fromf)
 
     with open(to_file, "r") as tof:
         dest_metadata = json.load(tof)
     orig_dest_metadata = deepcopy(dest_metadata)
 
     merged_metadata = merge_without_overwrite(
-        source_metadata, dest_metadata, raise_on_error=raise_on_error)
+        source_metadata,
+        dest_metadata,
+        raise_on_error=raise_on_error,
+    )
 
     if not merged_metadata:
         return 255
 
     # Only write if the data has changed
     if not merged_metadata == orig_dest_metadata:
         print("OVERWRITING", to_file)
         with open(to_file, "w") as tofw:
             json.dump(merged_metadata, tofw, indent=4)
 
     return 0
 
 
-def get_acq_dictionary(df):
-    """Creates a BIDS data dictionary from dataframe columns
-
-    Parameters:
-    -----------
+def get_acq_dictionary():
+    """Create a BIDS data dictionary from dataframe columns.
 
-        df: Pandas DataFrame
-            Pre export TSV that will be converted to a json dictionary
-
-    Returns:
-    -----------
-
-        acq_dict: dictionary
-            Python dictionary in BIDS data dictionary format
+    Parameters
+    ----------
+    df : :obj:`pandas.DataFrame`
+        Pre export TSV that will be converted to a json dictionary.
+
+    Returns
+    -------
+    acq_dict : :obj:`dict`
+        Python dictionary in BIDS data dictionary format
     """
     acq_dict = {}
     acq_dict["subject"] = {"Description": "Participant ID"}
     acq_dict["session"] = {"Description": "Session ID"}
     docs = " https://cubids.readthedocs.io/en/latest/about.html#definitions"
     desc = "Acquisition Group. See Read the Docs for more information"
     acq_dict["AcqGroup"] = {"Description": desc + docs}
 
     return acq_dict
 
 
 def group_by_acquisition_sets(files_tsv, output_prefix, acq_group_level):
-    '''Finds unique sets of Key/Param groups across subjects.
-    '''
-    from bids.layout import parse_file_entities
+    """Find unique sets of Key/Param groups across subjects.
+
+    This writes out the following files:
+    - <output_prefix>_AcqGrouping.tsv: A tsv with the mapping of subject/session to
+      acquisition group.
+    - <output_prefix>_AcqGrouping.json: A data dictionary for the AcqGrouping.tsv.
+    - <output_prefix>_AcqGroupInfo.txt: A text file with the summary of acquisition.
+    - <output_prefix>_AcqGroupInfo.json: A data dictionary for the AcqGroupInfo.txt.
+
+    Parameters
+    ----------
+    files_tsv : :obj:`str`
+        Path to the files tsv.
+    output_prefix : :obj:`str`
+        Prefix for output files.
+    acq_group_level : {"subject", "session"}
+        Level at which to group acquisitions.
+    """
     from bids import config
-    config.set_option('extension_initial_dot', True)
+    from bids.layout import parse_file_entities
+
+    config.set_option("extension_initial_dot", True)
 
-    files_df = pd.read_table(files_tsv, )
+    files_df = pd.read_table(
+        files_tsv,
+    )
     acq_groups = defaultdict(list)
     for _, row in files_df.iterrows():
         file_entities = parse_file_entities(row.FilePath)
 
-        if acq_group_level == 'subject':
-            acq_id = (file_entities.get("subject"),
-                      file_entities.get("session"))
+        if acq_group_level == "subject":
+            acq_id = (file_entities.get("subject"), file_entities.get("session"))
             acq_groups[acq_id].append((row.KeyGroup, row.ParamGroup))
         else:
             acq_id = (file_entities.get("subject"), None)
-            acq_groups[acq_id].append((row.KeyGroup, row.ParamGroup,
-                                       file_entities.get("session")))
+            acq_groups[acq_id].append((row.KeyGroup, row.ParamGroup, file_entities.get("session")))
 
     # Map the contents to a list of subjects/sessions
     contents_to_subjects = defaultdict(list)
     for key, value in acq_groups.items():
         contents_to_subjects[tuple(sorted(value))].append(key)
 
     # Sort them based on how many have that group
@@ -221,42 +319,38 @@
     descending_order = np.argsort(content_id_counts)[::-1]
 
     # Create a dataframe with the subject, session, groupnum
     grouped_sub_sess = []
     acq_group_info = []
     for groupnum, content_id_row in enumerate(descending_order, start=1):
         content_id = content_ids[content_id_row]
-        acq_group_info.append(
-            (groupnum, content_id_counts[content_id_row]) + content_id)
+        acq_group_info.append((groupnum, content_id_counts[content_id_row]) + content_id)
         for subject, session in contents_to_subjects[content_id]:
             grouped_sub_sess.append(
-                {"subject": 'sub-' + subject,
-                 "session": session,
-                 "AcqGroup": groupnum})
+                {"subject": "sub-" + subject, "session": session, "AcqGroup": groupnum}
+            )
 
     # Write the mapping of subject/session to
     acq_group_df = pd.DataFrame(grouped_sub_sess)
-    acq_group_df.to_csv(output_prefix + "_AcqGrouping.tsv", sep="\t",
-                        index=False)
+    acq_group_df.to_csv(output_prefix + "_AcqGrouping.tsv", sep="\t", index=False)
 
     # Create data dictionary for acq group tsv
-    acq_dict = get_acq_dictionary(acq_group_df)
+    acq_dict = get_acq_dictionary()
     with open(output_prefix + "_AcqGrouping.json", "w") as outfile:
         json.dump(acq_dict, outfile, indent=4)
 
     # Write the summary of acq groups to a text file
     with open(output_prefix + "_AcqGroupInfo.txt", "w") as infotxt:
-        infotxt.write(
-            "\n".join([" ".join(map(str, line)) for line in acq_group_info]))
+        infotxt.write("\n".join([" ".join(map(str, line)) for line in acq_group_info]))
 
     # Create and save AcqGroupInfo data dictionary
     header_dict = {}
-    header_dict['Long Description'] = 'Acquisition Group Info'
-    description = 'https://cubids.readthedocs.io/en/latest/usage.html'
-    header_dict['Description'] = description
-    header_dict['Version'] = 'CuBIDS v1.0.5'
+    header_dict["Long Description"] = "Acquisition Group Info"
+    description = "https://cubids.readthedocs.io/en/latest/usage.html"
+    header_dict["Description"] = description
+    header_dict["Version"] = "CuBIDS v1.0.5"
 
     acq_info_dict = {}
-    acq_info_dict['AcqGroupInfo.txt Data Dictionary'] = header_dict
+    acq_info_dict["AcqGroupInfo.txt Data Dictionary"] = header_dict
 
     with open(output_prefix + "_AcqGroupInfo.json", "w") as outfile:
         json.dump(acq_info_dict, outfile, indent=4)
```

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/anat/sub-01_ses-phdiff_T1w.json` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-01/ses-phdiff/anat/sub-01_ses-phdiff_T1w.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/anat/sub-01_ses-phdiff_T1w.nii.gz` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-01/ses-phdiff/anat/sub-01_ses-phdiff_T1w.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.json` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.nii.gz` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude1.json` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude1.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude1.nii.gz` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude1.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude2.json` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude2.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude2.nii.gz` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude2.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_phasediff.json` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_phasediff.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_phasediff.nii.gz` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_phasediff.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_dir-PA_epi.json` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_dir-PA_epi.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_dir-PA_epi.nii.gz` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_dir-PA_epi.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/func/sub-01_ses-phdiff_task-rest_bold.json` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-01/ses-phdiff/func/sub-01_ses-phdiff_task-rest_bold.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-01/ses-phdiff/func/sub-01_ses-phdiff_task-rest_bold.nii.gz` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-01/ses-phdiff/func/sub-01_ses-phdiff_task-rest_bold.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/anat/sub-02_ses-phdiff_T1w.json` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-02/ses-phdiff/anat/sub-02_ses-phdiff_T1w.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/anat/sub-02_ses-phdiff_T1w.nii.gz` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-02/ses-phdiff/anat/sub-02_ses-phdiff_T1w.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.bvec` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.bvec`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.json` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.nii.gz` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude1.json` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude1.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude1.nii.gz` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude1.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude2.json` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude2.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude2.nii.gz` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude2.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_phasediff.json` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_phasediff.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_phasediff.nii.gz` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_phasediff.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_dir-PA_epi.json` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_dir-PA_epi.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_dir-PA_epi.nii.gz` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_dir-PA_epi.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/func/sub-02_ses-phdiff_task-rest_bold.json` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-02/ses-phdiff/func/sub-02_ses-phdiff_task-rest_bold.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-02/ses-phdiff/func/sub-02_ses-phdiff_task-rest_bold.nii.gz` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-02/ses-phdiff/func/sub-02_ses-phdiff_task-rest_bold.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/anat/sub-03_ses-phdiff_T1w.json` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-03/ses-phdiff/anat/sub-03_ses-phdiff_T1w.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/anat/sub-03_ses-phdiff_T1w.nii.gz` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-03/ses-phdiff/anat/sub-03_ses-phdiff_T1w.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.bvec` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.bvec`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.json` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.nii.gz` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude1.json` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude1.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude1.nii.gz` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude1.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude2.json` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude2.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude2.nii.gz` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude2.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_phasediff.json` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_phasediff.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_phasediff.nii.gz` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_phasediff.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_dir-PA_epi.json` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_dir-PA_epi.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_dir-PA_epi.nii.gz` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_dir-PA_epi.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/func/sub-03_ses-phdiff_task-rest_bold.json` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-03/ses-phdiff/func/sub-03_ses-phdiff_task-rest_bold.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-03/ses-phdiff/func/sub-03_ses-phdiff_task-rest_bold.nii.gz` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-03/ses-phdiff/func/sub-03_ses-phdiff_task-rest_bold.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/anat/sub-04_ses-phdiff_T1w.json` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-04/ses-phdiff/anat/sub-04_ses-phdiff_T1w.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/anat/sub-04_ses-phdiff_T1w.nii.gz` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-04/ses-phdiff/anat/sub-04_ses-phdiff_T1w.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/dwi/sub-04_ses-phdiff_acq-HASC55AP_dwi.bvec` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-04/ses-phdiff/dwi/sub-04_ses-phdiff_acq-HASC55AP_dwi.bvec`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/dwi/sub-04_ses-phdiff_acq-HASC55AP_dwi.json` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-04/ses-phdiff/dwi/sub-04_ses-phdiff_acq-HASC55AP_dwi.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/dwi/sub-04_ses-phdiff_acq-HASC55AP_dwi.nii.gz` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-04/ses-phdiff/dwi/sub-04_ses-phdiff_acq-HASC55AP_dwi.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_acq-v4_magnitude1.json` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_acq-v4_magnitude1.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_acq-v4_magnitude1.nii.gz` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_acq-v4_magnitude1.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_acq-v4_magnitude2.json` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_acq-v4_magnitude2.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_acq-v4_magnitude2.nii.gz` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_acq-v4_magnitude2.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_acq-v4_phasediff.json` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_acq-v4_phasediff.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_acq-v4_phasediff.nii.gz` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_acq-v4_phasediff.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_dir-PA_epi.json` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_dir-PA_epi.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_dir-PA_epi.nii.gz` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-04/ses-phdiff/fmap/sub-04_ses-phdiff_dir-PA_epi.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/func/sub-04_ses-phdiff_task-rest_bold.json` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-04/ses-phdiff/func/sub-04_ses-phdiff_task-rest_bold.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset/sub-04/ses-phdiff/func/sub-04_ses-phdiff_task-rest_bold.nii.gz` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset/sub-04/ses-phdiff/func/sub-04_ses-phdiff_task-rest_bold.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/BIDS_Dataset.zip` & `cubids-1.1.0/cubids/tests/data/BIDS_Dataset.zip`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/anat/sub-01_ses-phdiff_T1w.json` & `cubids-1.1.0/cubids/tests/data/complete/sub-01/ses-phdiff/anat/sub-01_ses-phdiff_T1w.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/anat/sub-01_ses-phdiff_T1w.nii.gz` & `cubids-1.1.0/cubids/tests/data/complete/sub-01/ses-phdiff/anat/sub-01_ses-phdiff_T1w.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.bvec` & `cubids-1.1.0/cubids/tests/data/complete/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.bvec`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.json` & `cubids-1.1.0/cubids/tests/data/complete/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.nii.gz` & `cubids-1.1.0/cubids/tests/data/complete/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude1.json` & `cubids-1.1.0/cubids/tests/data/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude1.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude1.nii.gz` & `cubids-1.1.0/cubids/tests/data/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude1.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude2.json` & `cubids-1.1.0/cubids/tests/data/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude2.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude2.nii.gz` & `cubids-1.1.0/cubids/tests/data/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude2.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_phasediff.json` & `cubids-1.1.0/cubids/tests/data/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_phasediff.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_phasediff.nii.gz` & `cubids-1.1.0/cubids/tests/data/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_phasediff.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_dir-PA_epi.json` & `cubids-1.1.0/cubids/tests/data/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_dir-PA_epi.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_dir-PA_epi.nii.gz` & `cubids-1.1.0/cubids/tests/data/complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_dir-PA_epi.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/func/sub-01_ses-phdiff_task-rest_bold.json` & `cubids-1.1.0/cubids/tests/data/complete/sub-01/ses-phdiff/func/sub-01_ses-phdiff_task-rest_bold.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/complete/sub-01/ses-phdiff/func/sub-01_ses-phdiff_task-rest_bold.nii.gz` & `cubids-1.1.0/cubids/tests/data/complete/sub-01/ses-phdiff/func/sub-01_ses-phdiff_task-rest_bold.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/anat/sub-02_ses-phdiff_T1w.json` & `cubids-1.1.0/cubids/tests/data/complete/sub-02/ses-phdiff/anat/sub-02_ses-phdiff_T1w.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/anat/sub-02_ses-phdiff_T1w.nii.gz` & `cubids-1.1.0/cubids/tests/data/complete/sub-02/ses-phdiff/anat/sub-02_ses-phdiff_T1w.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.bvec` & `cubids-1.1.0/cubids/tests/data/complete/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.bvec`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.json` & `cubids-1.1.0/cubids/tests/data/complete/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.nii.gz` & `cubids-1.1.0/cubids/tests/data/complete/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude1.json` & `cubids-1.1.0/cubids/tests/data/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude1.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude1.nii.gz` & `cubids-1.1.0/cubids/tests/data/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude1.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude2.json` & `cubids-1.1.0/cubids/tests/data/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude2.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude2.nii.gz` & `cubids-1.1.0/cubids/tests/data/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude2.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_phasediff.json` & `cubids-1.1.0/cubids/tests/data/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_phasediff.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_phasediff.nii.gz` & `cubids-1.1.0/cubids/tests/data/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_phasediff.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_dir-PA_epi.json` & `cubids-1.1.0/cubids/tests/data/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_dir-PA_epi.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_dir-PA_epi.nii.gz` & `cubids-1.1.0/cubids/tests/data/complete/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_dir-PA_epi.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/func/sub-02_ses-phdiff_task-rest_bold.json` & `cubids-1.1.0/cubids/tests/data/complete/sub-02/ses-phdiff/func/sub-02_ses-phdiff_task-rest_bold.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/complete/sub-02/ses-phdiff/func/sub-02_ses-phdiff_task-rest_bold.nii.gz` & `cubids-1.1.0/cubids/tests/data/complete/sub-02/ses-phdiff/func/sub-02_ses-phdiff_task-rest_bold.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/anat/sub-03_ses-phdiff_T1w.json` & `cubids-1.1.0/cubids/tests/data/complete/sub-03/ses-phdiff/anat/sub-03_ses-phdiff_T1w.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/anat/sub-03_ses-phdiff_T1w.nii.gz` & `cubids-1.1.0/cubids/tests/data/complete/sub-03/ses-phdiff/anat/sub-03_ses-phdiff_T1w.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.bvec` & `cubids-1.1.0/cubids/tests/data/complete/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.bvec`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.json` & `cubids-1.1.0/cubids/tests/data/complete/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.nii.gz` & `cubids-1.1.0/cubids/tests/data/complete/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude1.json` & `cubids-1.1.0/cubids/tests/data/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude1.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude1.nii.gz` & `cubids-1.1.0/cubids/tests/data/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude1.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude2.json` & `cubids-1.1.0/cubids/tests/data/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude2.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude2.nii.gz` & `cubids-1.1.0/cubids/tests/data/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude2.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_phasediff.json` & `cubids-1.1.0/cubids/tests/data/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_phasediff.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_phasediff.nii.gz` & `cubids-1.1.0/cubids/tests/data/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_phasediff.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_dir-PA_epi.json` & `cubids-1.1.0/cubids/tests/data/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_dir-PA_epi.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_dir-PA_epi.nii.gz` & `cubids-1.1.0/cubids/tests/data/complete/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_dir-PA_epi.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/func/sub-03_ses-phdiff_task-rest_bold.json` & `cubids-1.1.0/cubids/tests/data/complete/sub-03/ses-phdiff/func/sub-03_ses-phdiff_task-rest_bold.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/complete/sub-03/ses-phdiff/func/sub-03_ses-phdiff_task-rest_bold.nii.gz` & `cubids-1.1.0/cubids/tests/data/complete/sub-03/ses-phdiff/func/sub-03_ses-phdiff_task-rest_bold.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/anat/sub-01_ses-phdiff_T1w.json` & `cubids-1.1.0/cubids/tests/data/inconsistent/sub-01/ses-phdiff/anat/sub-01_ses-phdiff_T1w.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/anat/sub-01_ses-phdiff_T1w.nii.gz` & `cubids-1.1.0/cubids/tests/data/inconsistent/sub-01/ses-phdiff/anat/sub-01_ses-phdiff_T1w.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.bvec` & `cubids-1.1.0/cubids/tests/data/inconsistent/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.bvec`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.json` & `cubids-1.1.0/cubids/tests/data/inconsistent/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.nii.gz` & `cubids-1.1.0/cubids/tests/data/inconsistent/sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude1.json` & `cubids-1.1.0/cubids/tests/data/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude1.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude1.nii.gz` & `cubids-1.1.0/cubids/tests/data/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude1.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude2.json` & `cubids-1.1.0/cubids/tests/data/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude2.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude2.nii.gz` & `cubids-1.1.0/cubids/tests/data/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude2.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_phasediff.json` & `cubids-1.1.0/cubids/tests/data/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_phasediff.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_phasediff.nii.gz` & `cubids-1.1.0/cubids/tests/data/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_phasediff.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_dir-PA_epi.json` & `cubids-1.1.0/cubids/tests/data/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_dir-PA_epi.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_dir-PA_epi.nii.gz` & `cubids-1.1.0/cubids/tests/data/inconsistent/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_dir-PA_epi.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/func/sub-01_ses-phdiff_task-rest_bold.json` & `cubids-1.1.0/cubids/tests/data/inconsistent/sub-01/ses-phdiff/func/sub-01_ses-phdiff_task-rest_bold.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/inconsistent/sub-01/ses-phdiff/func/sub-01_ses-phdiff_task-rest_bold.nii.gz` & `cubids-1.1.0/cubids/tests/data/inconsistent/sub-01/ses-phdiff/func/sub-01_ses-phdiff_task-rest_bold.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/anat/sub-02_ses-phdiff_T1w.json` & `cubids-1.1.0/cubids/tests/data/inconsistent/sub-02/ses-phdiff/anat/sub-02_ses-phdiff_T1w.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/anat/sub-02_ses-phdiff_T1w.nii.gz` & `cubids-1.1.0/cubids/tests/data/inconsistent/sub-02/ses-phdiff/anat/sub-02_ses-phdiff_T1w.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.bvec` & `cubids-1.1.0/cubids/tests/data/inconsistent/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.bvec`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.json` & `cubids-1.1.0/cubids/tests/data/inconsistent/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.nii.gz` & `cubids-1.1.0/cubids/tests/data/inconsistent/sub-02/ses-phdiff/dwi/sub-02_ses-phdiff_acq-HASC55AP_dwi.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude1.json` & `cubids-1.1.0/cubids/tests/data/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude1.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude1.nii.gz` & `cubids-1.1.0/cubids/tests/data/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude1.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude2.json` & `cubids-1.1.0/cubids/tests/data/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude2.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude2.nii.gz` & `cubids-1.1.0/cubids/tests/data/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_magnitude2.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_phasediff.json` & `cubids-1.1.0/cubids/tests/data/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_phasediff.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_phasediff.nii.gz` & `cubids-1.1.0/cubids/tests/data/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_acq-v4_phasediff.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_dir-PA_epi.json` & `cubids-1.1.0/cubids/tests/data/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_dir-PA_epi.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_dir-PA_epi.nii.gz` & `cubids-1.1.0/cubids/tests/data/inconsistent/sub-02/ses-phdiff/fmap/sub-02_ses-phdiff_dir-PA_epi.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/func/sub-02_ses-phdiff_task-rest_bold.json` & `cubids-1.1.0/cubids/tests/data/inconsistent/sub-02/ses-phdiff/func/sub-02_ses-phdiff_task-rest_bold.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/inconsistent/sub-02/ses-phdiff/func/sub-02_ses-phdiff_task-rest_bold.nii.gz` & `cubids-1.1.0/cubids/tests/data/inconsistent/sub-02/ses-phdiff/func/sub-02_ses-phdiff_task-rest_bold.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/anat/sub-03_ses-phdiff_T1w.json` & `cubids-1.1.0/cubids/tests/data/inconsistent/sub-03/ses-phdiff/anat/sub-03_ses-phdiff_T1w.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/anat/sub-03_ses-phdiff_T1w.nii.gz` & `cubids-1.1.0/cubids/tests/data/inconsistent/sub-03/ses-phdiff/anat/sub-03_ses-phdiff_T1w.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.bvec` & `cubids-1.1.0/cubids/tests/data/inconsistent/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.bvec`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.json` & `cubids-1.1.0/cubids/tests/data/inconsistent/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.nii.gz` & `cubids-1.1.0/cubids/tests/data/inconsistent/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude1.json` & `cubids-1.1.0/cubids/tests/data/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude1.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude1.nii.gz` & `cubids-1.1.0/cubids/tests/data/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude1.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude2.json` & `cubids-1.1.0/cubids/tests/data/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude2.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude2.nii.gz` & `cubids-1.1.0/cubids/tests/data/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_magnitude2.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_phasediff.json` & `cubids-1.1.0/cubids/tests/data/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_phasediff.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_phasediff.nii.gz` & `cubids-1.1.0/cubids/tests/data/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_acq-v4_phasediff.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_dir-PA_epi.json` & `cubids-1.1.0/cubids/tests/data/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_dir-PA_epi.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_dir-PA_epi.nii.gz` & `cubids-1.1.0/cubids/tests/data/inconsistent/sub-03/ses-phdiff/fmap/sub-03_ses-phdiff_dir-PA_epi.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/func/sub-03_ses-phdiff_task-rest_bold.json` & `cubids-1.1.0/cubids/tests/data/inconsistent/sub-03/ses-phdiff/func/sub-03_ses-phdiff_task-rest_bold.json`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/testdata/inconsistent/sub-03/ses-phdiff/func/sub-03_ses-phdiff_task-rest_bold.nii.gz` & `cubids-1.1.0/cubids/tests/data/inconsistent/sub-03/ses-phdiff/func/sub-03_ses-phdiff_task-rest_bold.nii.gz`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/cubids/validator.py` & `cubids-1.1.0/cubids/validator.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,134 +1,172 @@
-import subprocess
+"""Methods for validating BIDS datasets."""
+
+import glob
 import json
 import logging
 import os
-import glob
 import pathlib
-import pandas as pd
+import subprocess
 
-logger = logging.getLogger('cubids-cli')
+import pandas as pd
 
+logger = logging.getLogger("cubids-cli")
 
-def build_validator_call(path, ignore_headers=False, ignore_subject=True):
-    """Build a subprocess command to the bids validator"""
 
+def build_validator_call(path, ignore_headers=False):
+    """Build a subprocess command to the bids validator."""
     # build docker call
-    command = ['bids-validator', '--verbose', '--json']
+    # CuBIDS automatically ignores subject consistency.
+    command = ["bids-validator", "--verbose", "--json", "--ignoreSubjectConsistency"]
 
     if ignore_headers:
-        command.append('--ignoreNiftiHeaders')
-    if ignore_subject:
-        command.append('--ignoreSubjectConsistency')
+        command.append("--ignoreNiftiHeaders")
 
     command.append(path)
 
     return command
 
 
 def build_subject_paths(bids_dir):
-    """Build a list of BIDS dirs with 1 subject each"""
-
+    """Build a list of BIDS dirs with 1 subject each."""
     bids_dir = str(bids_dir)
     if not bids_dir.endswith("/"):
         bids_dir += "/"
 
     root_files = [x for x in glob.glob(bids_dir + "*") if os.path.isfile(x)]
 
     bids_dir += "sub-*/"
 
     subjects = glob.glob(bids_dir)
 
     if len(subjects) < 1:
-
-        raise ValueError("Couldn't find any subjects "
-                         "in the specified directory:\n" +
-                         bids_dir)
+        raise ValueError("Couldn't find any subjects in the specified directory:\n" + bids_dir)
 
     subjects_dict = {}
 
     for sub in subjects:
         purepath = pathlib.PurePath(sub)
         sub_label = purepath.name
 
-        files = [x for x in glob.glob(sub + '**', recursive=True)
-                 if os.path.isfile(x)]
+        files = [x for x in glob.glob(sub + "**", recursive=True) if os.path.isfile(x)]
         files.extend(root_files)
         subjects_dict[sub_label] = files
 
     return subjects_dict
 
 
-def run_validator(call, verbose=True):
-    """Run the validator with subprocess"""
+def run_validator(call):
+    """Run the validator with subprocess.
+
+    Parameters
+    ----------
+    call : :obj:`list`
+        List of strings to pass to subprocess.run().
+
+    Returns
+    -------
+    :obj:`subprocess.CompletedProcess`
+        The result of the subprocess call.
+    """
     # if verbose:
     #     logger.info("Running the validator with call:")
     #     logger.info('\"' + ' '.join(call) + '\"')
 
-    ret = subprocess.run(call, stdout=subprocess.PIPE,
-                         stderr=subprocess.PIPE)
-    return (ret)
+    ret = subprocess.run(call, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+    return ret
 
 
 def parse_validator_output(output):
-    """Parse the JSON output of the BIDS validator into a pandas dataframe
-    Parameters:
-    -----------
-        - path : string
-            Path to JSON file of BIDS validator output
+    """Parse the JSON output of the BIDS validator into a pandas dataframe.
+
+    Parameters
+    ----------
+    output : :obj:`str`
+        Path to JSON file of BIDS validator output
+
     Returns
-    -----------
-        - Pandas DataFrame
+    -------
+    df : :obj:`pandas.DataFrame`
+        Dataframe of validator output.
     """
 
     def get_nested(dct, *keys):
+        """Get a nested value from a dictionary.
+
+        Parameters
+        ----------
+        dct : :obj:`dict`
+            Dictionary to get value from.
+        keys : :obj:`list`
+            List of keys to get value from.
+
+        Returns
+        -------
+        :obj:`dict`
+            The nested value.
+        """
         for key in keys:
             try:
                 dct = dct[key]
             except (KeyError, TypeError):
                 return None
         return dct
 
     data = json.loads(output)
 
-    issues = data['issues']
+    issues = data["issues"]
 
     def parse_issue(issue_dict):
+        """Parse a single issue from the validator output.
 
+        Parameters
+        ----------
+        issue_dict : :obj:`dict`
+            Dictionary of issue.
+
+        Returns
+        -------
+        return_dict : :obj:`dict`
+            Dictionary of parsed issue.
+        """
         return_dict = {}
-        return_dict['files'] = [
-            get_nested(x, 'file', 'relativePath')
-            for x in issue_dict.get('files', '')
-            ]
-        return_dict['type'] = issue_dict.get('key' '')
-        return_dict['severity'] = issue_dict.get('severity', '')
-        return_dict['description'] = issue_dict.get('reason', '')
-        return_dict['code'] = issue_dict.get('code', '')
-        return_dict['url'] = issue_dict.get('helpUrl', '')
+        return_dict["files"] = [
+            get_nested(x, "file", "relativePath") for x in issue_dict.get("files", "")
+        ]
+        return_dict["type"] = issue_dict.get("key", "")
+        return_dict["severity"] = issue_dict.get("severity", "")
+        return_dict["description"] = issue_dict.get("reason", "")
+        return_dict["code"] = issue_dict.get("code", "")
+        return_dict["url"] = issue_dict.get("helpUrl", "")
 
-        return (return_dict)
+        return return_dict
 
     df = pd.DataFrame()
 
-    for warn in issues['warnings']:
-
+    for warn in issues["warnings"]:
         parsed = parse_issue(warn)
         parsed = pd.DataFrame(parsed)
         df = pd.concat([df, parsed], ignore_index=True)
 
-    for err in issues['errors']:
-
+    for err in issues["errors"]:
         parsed = parse_issue(err)
         parsed = pd.DataFrame(parsed)
         df = pd.concat([df, parsed], ignore_index=True)
 
     return df
 
 
-def get_val_dictionary(df):
+def get_val_dictionary():
+    """Get value dictionary.
+
+    Returns
+    -------
+    val_dict : dict
+        Dictionary of values.
+    """
     val_dict = {}
     val_dict["files"] = {"Description": "File with warning orerror"}
     val_dict["type"] = {"Description": "BIDS validation warning or error"}
     val_dict["severity"] = {"Description": "gravity of problem (warning/error"}
     val_dict["description"] = {"Description": "Description of warning/error"}
     val_dict["code"] = {"Description": "BIDS validator issue code number"}
     val_dict["url"] = {"Description": "Link to the issue's neurostars thread"}
```

### Comparing `cubids-1.0.9/docs/Makefile` & `cubids-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/docs/_static/checked_dataset_into_datalad.png` & `cubids-1.1.0/docs/_static/checked_dataset_into_datalad.png`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/docs/_static/cubids_workflow.png` & `cubids-1.1.0/docs/_static/cubids_workflow.png`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/docs/_static/screenshot_1.png` & `cubids-1.1.0/docs/_static/screenshot_1.png`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/docs/_static/screenshot_2.png` & `cubids-1.1.0/docs/_static/screenshot_2.png`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/docs/_static/screenshot_3.png` & `cubids-1.1.0/docs/_static/screenshot_3.png`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/docs/_static/screenshot_4.png` & `cubids-1.1.0/docs/_static/screenshot_4.png`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/docs/_static/screenshot_5.png` & `cubids-1.1.0/docs/_static/screenshot_5.png`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/docs/_static/screenshot_6.png` & `cubids-1.1.0/docs/_static/screenshot_6.png`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/docs/_static/screenshot_7.png` & `cubids-1.1.0/docs/_static/screenshot_7.png`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/docs/_static/screenshot_8.png` & `cubids-1.1.0/docs/_static/screenshot_8.png`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/docs/example.rst` & `cubids-1.1.0/docs/example.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,380 +1,406 @@
+.. include:: links.rst
+
 ===================
 Example Walkthrough
 ===================
 
-The ``CuBIDS`` workflow is currently being used in neuroimaging labs at a number of institutions 
-including University of Pennsylvania, Children's Hospital of Philadelphia, the Child Mind Institute, 
-and University of Minnesota's Masonic Institute for the Developing Brain. To demonstrate the utility of
-``CuBIDS``, here we apply the software to a small example dataset that is included `in our Github repo <https://github.com/PennLINC/CuBIDS/tree/main/cubids/testdata/BIDS_Dataset>`_.
-This example dataset does not contain any PHI. 
+The ``CuBIDS`` workflow is currently being used in neuroimaging labs at a number of institutions
+including University of Pennsylvania, Children's Hospital of Philadelphia, the Child Mind Institute,
+and University of Minnesota's Masonic Institute for the Developing Brain.
+To demonstrate the utility of ``CuBIDS``,
+here we apply the software to a small example dataset that is included
+`in our Github repo <https://github.com/PennLINC/CuBIDS/tree/main/cubids/testdata/BIDS_Dataset>`_.
+This example dataset does not contain any PHI.
 
 Following the installation instructions at :doc:`the installation page <installation>`,
 you should have successfully installed ``CuBIDS``, ``DataLad``, and the ``bids-validator`` inside a
-conda environment titled "cubids". In this example, we use validator version ``1.7.2``.
-Using a different version of the validator may result in slightly different validation
-tsv outputs, but the example should still be useful. 
-
-Throughout this example, we use ``DataLad`` for version control. Although ``DataLad``
-is an optional dependency of ``CuBIDS``, we use it here to demonstrate its
-powerful integration with ``CuBIDS`` and the benefits it can provide its users. 
-
-Now that we have installed CuBIDS and all necessary dependencies, we are ready to begin the curation 
-process on our example dataset. We create a ``CuBIDS_Test`` directory to function as our working directory 
-and navigate to it as follows:
+conda environment titled "cubids".
+In this example, we use validator version ``1.7.2``.
+Using a different version of the validator may result in slightly different validation tsv outputs,
+but the example should still be useful.
+
+Throughout this example, we use ``DataLad`` for version control.
+Although ``DataLad`` is an optional dependency of ``CuBIDS``,
+we use it here to demonstrate its powerful integration with ``CuBIDS`` and the benefits
+it can provide its users.
 
-mkdir $PWD/CuBIDS_Test 
-cd CuBIDS_Test
+Now that we have installed CuBIDS and all necessary dependencies,
+we are ready to begin the curation process on our example dataset.
+We create a ``CuBIDS_Test`` directory to function as our working directory and navigate to it as follows.
 
 .. code-block:: console
 
-    $ conda activate cubids
-    $ mkdir -p $PWD/CuBIDS_Test
+    $ mkdir $PWD/CuBIDS_Test
     $ cd CuBIDS_Test
+    $ conda activate cubids
 
 Now, download and unzip the example data (you can also do this in your Finder window):
 
 .. code-block:: console
-    
+
     $ curl -sSLO https://github.com/PennLINC/CuBIDS/raw/main/cubids/testdata/BIDS_Dataset.zip
     $ unzip BIDS_Dataset.zip
     $ rm BIDS_Dataset.zip
 
-Identifying and removing PHI 
-------------------------------------------
+Identifying and removing PHI
+----------------------------
 
 As a first step, we use CuBIDS to identify the metadata fields present in the dataset,
-and remove any protected health information (PHI) or other sensitive fields. We want to do this *before* implementing any
-``DataLad`` commands, as we must ensure PHI is not tracked as part of version control.
+and remove any protected health information (PHI) or other sensitive fields.
+We want to do this *before* implementing any ``DataLad`` commands,
+as we must ensure PHI is not tracked as part of version control.
 
 This is accomplished with the following command:
 
 .. code-block:: console
 
-    $ cubids-print-metadata-fields BIDS_Dataset
+    $ cubids print-metadata-fields BIDS_Dataset
 
-This command returns a total of 66 fields, including acquisition parameters and other metadata 
-fields present in the dataset's JSON sidecars. From the output we can see that the dataset contains
-(simulated) PHI — the `PatientName` field, which we wish to remove. 
+This command returns a total of 66 fields, including acquisition parameters and other metadata
+fields present in the dataset's JSON sidecars.
+From the output we can see that the dataset contains (simulated) PHI — the `PatientName` field,
+which we wish to remove.
 To remove the `PatientName` field from the sidecars, we can use the command:
 
 .. code-block:: console
 
-    $ cubids-remove-metadata-fields BIDS_Dataset --fields PatientName
+    $ cubids remove-metadata-fields BIDS_Dataset --fields PatientName
 
 This command should succeed silently.
 
+
 Checking the BIDS dataset into DataLad
--------------------------------------------
+--------------------------------------
 
-Now that all PHI has been removed from the metadata, we are ready to check our dataset into ``datalad``. 
+Now that all PHI has been removed from the metadata, we are ready to check our dataset into ``datalad``.
 To do this, we run the following command:
 
 .. code-block:: console
 
     $ datalad create -c text2git BIDS_Dataset_DataLad
 
 This command creates a new directory called ``BIDS_Dataset_DataLad`` where
 ``DataLad`` will begin implementing version control and provenance tracking while
 we implement the rest of our ``CuBIDS`` workflow.
-The creation of our ``datalad`` dataset is accordingly reflected in the dataset's version control 
-history, accessible with ``git log``. At any point in the ``CuBIDS`` workflow,
+The creation of our ``datalad`` dataset is accordingly reflected in the dataset's version control history,
+accessible with ``git log``.
+At any point in the ``CuBIDS`` workflow,
 we can view a summary of our dataset's version history by running the following commands:
 
-.. code-block:: console 
+.. code-block:: console
 
     $ cd BIDS_Dataset_DataLad
     $ git log --oneline
     $ cd ..
 
-This command will write the following to the terminal: 
+This command will write the following to the terminal:
 
 .. image:: _static/screenshot_1.png
 
-Next, we copy the contents of our BIDS dataset into the newly created and currently empty DataLad 
-dataset and save the changes. 
+Next, we copy the contents of our BIDS dataset into the newly created and currently empty DataLad
+dataset and save the changes.
 
 .. code-block:: console
 
     $ cd ..
     $ cp -r BIDS_Dataset/* BIDS_Dataset_DataLad
 
-In addition to being able to access the version history of our data, any point in this workflow, we can 
-also check the status of untracked (not yet saved) changes using the datalad status command, as seen 
-below: 
+In addition to being able to access the version history of our data, any point in this workflow,
+we can also check the status of untracked (not yet saved) changes using the datalad status command,
+as seen below:
 
-.. code-block:: console 
+.. code-block:: console
 
     $ cd BIDS_Dataset_DataLad && datalad status
     $ cd ..
 
-This command produces a description of the changes we have made to the data since the last commit 
+This command produces a description of the changes we have made to the data since the last commit
 (see below)
 
 .. image:: _static/screenshot_2.png
 
-The command above shows all files untracked, as we have copied the BIDS data into 
-``~/CuBIDS_Test/BIDS_Dataset_DataLad`` but have not yet saved those changes. Our next step is to 
-run save. It is best practice to provide a detailed commit message, for example:
+The command above shows all files untracked, as we have copied the BIDS data into
+``~/CuBIDS_Test/BIDS_Dataset_DataLad`` but have not yet saved those changes.
+Our next step is to run save.
+It is best practice to provide a detailed commit message, for example:
 
 .. code-block:: console
 
     $ datalad save -d ~/CuBIDS_Test/BIDS_Dataset_DataLad -m "checked dataset into datalad"
 
 At this stage, we also recommend removing the ``BIDS_Dataset`` directory — its contents are
 safely copied into and tracked in ``BIDS_Dataset_DataLad``.
-We can check our ``git`` history to be sure, which will display the version history of our dataset 
-thus far, with the following command: 
+We can check our ``git`` history to be sure,
+which will display the version history of our dataset thus far,
+with the following command:
 
 .. code-block:: console
 
     $ cd BIDS_Dataset_DataLad/
     $ git log --oneline
     $ cd ..
 
-which will produce the following: 
+which will produce the following:
 
 .. image:: _static/screenshot_3.png
 
-As seen above, the creation of our DataLad dataset is now reflected in the dataset’s version control 
-history. Note that it is best practice to provide a detailed commit message with each change made to
-the data. 
+As seen above,
+the creation of our DataLad dataset is now reflected in the dataset's version control history.
+Note that it is best practice to provide a detailed commit message with each change made to the data.
 
 
 Adding NIfTI Information to JSON Sidecars
--------------------------------------------
+-----------------------------------------
 
 Next, we seek to add more image parameters to our sidecars so that we can better define our Key Groups.
 Historically, only a subset of parameters in the NIfTI image header have been included in a BIDS sidecar...
-Parameters such as image dimensions, number of volumes, image obliquity, and voxel sizes — all important
-data that can change how our pipelines will eventually run!
+Parameters such as image dimensions, number of volumes, image obliquity, and voxel sizes —
+all important data that can change how our pipelines will eventually run!
 
 To add them to the sidecar metadata, run:
 
 .. code-block:: console
 
-    $ cubids-add-nifti-info BIDS_Dataset_DataLad --use-datalad
-
-This command adds the NIfTI header information to the JSON sidecars and saves those changes. In order 
-to ensure that this command has been executed properly, we can run ``cubids-print-metadata-fields`` 
-once more, which reveals that new NIfTI header information has been successfully included in the metadata. 
-Since we ran ``cubids-add-nifti-info`` with the ``--use-datalad`` flag set, ``CuBIDS`` automatically saves
-the changes made to the dataset to the git log as follows:
+    $ cubids add-nifti-info BIDS_Dataset_DataLad --use-datalad
 
+This command adds the NIfTI header information to the JSON sidecars and saves those changes.
+In order to ensure that this command has been executed properly,
+we can run ``cubids print-metadata-fields`` once more,
+which reveals that new NIfTI header information has been successfully included in the metadata.
+Since we ran ``cubids add-nifti-info`` with the ``--use-datalad`` flag set,
+``CuBIDS`` automatically saves the changes made to the dataset to the git log as follows:
 
 .. image:: _static/screenshot_4.png
 
-BIDS validation 
-----------------
+
+BIDS validation
+---------------
 
 The next step in the ``CuBIDS`` workflow is to run BIDS validation
-to detect potential curation errors using ``cubids-validate``.
+to detect potential curation errors using ``cubids validate``.
 
 .. code-block:: console
 
-    $ cubids-validate BIDS_Dataset_DataLad v0 --sequential
+    $ cubids validate BIDS_Dataset_DataLad v0 --sequential
 
-.. note::  The use of the ``--sequential`` flag forces the validator to treat each participant as its own BIDS dataset. This can be helpful for identifying heterogeneous elements, but can be slowed down by extremely large datasets.
+.. note::
+    The use of the ``--sequential`` flag forces the validator to treat each participant as its
+    own BIDS dataset.
+    This can be helpful for identifying heterogeneous elements,
+    but can be slowed down by extremely large datasets.
 
-This command produces the following tsv: 
+This command produces the following tsv:
 
 .. csv-table:: v0_validation.tsv
    :file: _static/v0_validation.csv
    :widths: 10, 10, 10, 10, 10, 40, 10
    :header-rows: 1
 
 This initial validation run reveals firstly that Phase Encoding Direction (PED) is not specified
-for one of the task-rest BOLD scans. This is an important parameter
-for `fieldmap correction in fMRIPRep <nipreps.org/sdcflows/master/index.html>`_, 
+for one of the task-rest BOLD scans.
+This is an important parameter for
+`fieldmap correction in fMRIPRep <nipreps.org/sdcflows/master/index.html>`_,
 so knowing this ahead of time is valuable information.
-To resolve this, we could either find the PED for this scan elsewhere and 
-edit its sidecar to include it, or remove that scan from the dataset.
-For the purpose of this demonstration, we elect to remove 
-the scan. To do this, we run the ``cubids-purge`` command.
-
-``cubids-purge`` requires as input a list of files to cleanly 
-"purge" from the dataset. You can create this file in any
-text editor, as long as it is saved as plain text ``.txt``. For this example, we created the following file: 
+To resolve this,
+we could either find the PED for this scan elsewhere and edit its sidecar to include it,
+or remove that scan from the dataset.
+For the purposes of this demonstration,
+we elect to remove the scan.
+To do this, we run the ``cubids purge`` command.
+
+``cubids purge`` requires as input a list of files to cleanly "purge" from the dataset.
+You can create this file in any text editor,
+as long as it is saved as plain text ``.txt``.
+For this example, we created the following file:
 
 .. code-block:: console
-    
+
     $ cat no_ped.txt
-    
+
     /AN/EXAMPLE/PATH/CuBIDS_Test/BIDS_Dataset_Datalad/sub-02/ses-phdiff/func/sub-02_ses-phdiff_task-rest_bold.nii.gz
 
 
-and saved it in our ``CuBIDS_Test directory``. 
+and saved it in our ``CuBIDS_Test directory``.
 
 To safely purge this file from the dataset, run:
 
 .. code-block:: console
 
-    $ cubids-purge BIDS_Dataset_DataLad no_ped.txt --use-datalad 
+    $ cubids purge BIDS_Dataset_DataLad no_ped.txt --use-datalad
 
-We elect to use ``cubids-purge`` instead of simply removing the scan
-due to the fact that purge will ensure all associations,
-such as sidecars and IntendedFor references in fieldmaps, are
-also safely deleted. ``CuBIDS`` will reflect these deletions in the
-``git`` history:
+We elect to use ``cubids purge`` instead of simply removing the scan due to the fact that
+purge will ensure all associations,
+such as sidecars and IntendedFor references in fieldmaps,
+are also safely deleted.
+``CuBIDS`` will reflect these deletions in the ``git`` history:
 
 .. image:: _static/screenshot_5.png
 
 
-Returning again to ``v0_validation.tsv``, we can also see that there is one DWI scan missing 
-TotalReadoutTime, a metadata field necessary for 
-`fieldmap correction <nipreps.org/sdcflows/master/index.html>`_.
-After conferring with our MR physicist and the scanner technician, we determine 
-that TotalReadoutTime (TRT) was erroneously omitted from the DWI sidecars!
-After some digging, the technician provided us with the correct value, so it's now our job to manually 
-add it to the sidecar for which it is missing. Once we have this value, we manually add it to the sidecar 
-for which it is missing by opening ``BIDS_Dataset_DataLad/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.json`` 
-in an editor and adding the following line: 
+Returning again to ``v0_validation.tsv``,
+we can also see that there is one DWI scan missing TotalReadoutTime,
+a metadata field necessary for `fieldmap correction <nipreps.org/sdcflows/master/index.html>`_.
+After conferring with our MR physicist and the scanner technician,
+we determine that TotalReadoutTime (TRT) was erroneously omitted from the DWI sidecars!
+After some digging, the technician provided us with the correct value,
+so it's now our job to manually add it to the sidecar for which it is missing.
+Once we have this value, we manually add it to the sidecar for which it is missing by opening
+``BIDS_Dataset_DataLad/sub-03/ses-phdiff/dwi/sub-03_ses-phdiff_acq-HASC55AP_dwi.json``
+in an editor and adding the following line:
 
-.. code-block:: console 
+.. code-block:: console
 
     "TotalReadoutTime": 0.0717598,
 
-on a new line anywhere inside the curly braces between lines containing parameters and their values, 
-save the changes, and close the JSON file. We then save the latest changes to the dataset with a 
-detailed commit message as follows:
+on a new line anywhere inside the curly braces between lines containing parameters and their values,
+save the changes, and close the JSON file.
+We then save the latest changes to the dataset with a detailed commit message as follows:
 
 .. code-block:: console
 
     $ datalad save -d BIDS_Dataset_DataLad -m "Added TotalReadoutTime to sub-03_ses-phdiff_acq-HASC55AP_dwi.nii.json"
 
 This change will be reflected in the git history.
 
 .. image:: _static/screenshot_6.png
 
 To verify that there are no remaining validation errors, we rerun validation with the following command:
 
 .. code-block:: console
 
-    $ cubids-validate BIDS_Dataset_DataLad v1 --sequential
+    $ cubids validate BIDS_Dataset_DataLad v1 --sequential
 
-This command should produce no tsv output, and instead print “No issues/warnings parsed, your dataset is 
-BIDS valid” to the terminal, which indicates that the dataset is now free from BIDS validation errors 
-and warnings.
+This command should produce no tsv output, and instead print “No issues/warnings parsed,
+your dataset is BIDS valid” to the terminal,
+which indicates that the dataset is now free from BIDS validation errors and warnings.
 
 Visualizing metadata heterogeneity
------------------------------------
+----------------------------------
 
-Next, we'll use ``CuBIDS`` to gain some insight on the
-dataset's structure, heterogeneity, and metadata errors.
-We'll do this with ``cubids-group``.
-
-Large datasets almost inevitably contain multiple validation and metadata 
-errors, so it's useful to run both ``cubids-validate`` and ``cubids-group``
-in parallel, as validation errors are better understood within the context of a dataset's heterogeneity. Being able to see 
-both metadata errors (such as missing or incorrectly specified
-sidecar parameters) that grouping reveals alongside BIDS errors that
-the validator catches, gives users a more comprehensive view of
-the issues they will need to fix during the curation process. Note that if users
-choose to provide just a pass in just a filename prefix (e.g. V1) for the second argument, 
-then CuBIDS will put the four grouping outputs in ``bids_dir/code/CuBIDS``. If users 
-provide a path (e.g. ``/Users/scovitz/BIDS/V1``), then output files will go to the 
-specified location. An example command for running the grouping function as follows:
+Next, we'll use ``CuBIDS`` to gain some insight on the dataset's structure, heterogeneity,
+and metadata errors.
+We'll do this with ``cubids group``.
+
+Large datasets almost inevitably contain multiple validation and metadata errors,
+so it's useful to run both ``cubids validate`` and ``cubids group`` in parallel,
+as validation errors are better understood within the context of a dataset's heterogeneity.
+Being able to see both metadata errors
+(such as missing or incorrectly specified sidecar parameters)
+that grouping reveals alongside BIDS errors that the validator catches,
+gives users a more comprehensive view of the issues they will need to fix during the curation process.
+Note that if users choose to provide just a pass in just a filename prefix (e.g. V1)
+for the second argument,
+then CuBIDS will put the four grouping outputs in ``bids_dir/code/CuBIDS``.
+If users provide a path (e.g., ``/Users/scovitz/BIDS/V1``),
+then output files will go to the specified location.
+An example command for running the grouping function as follows:
 
 .. code-block:: console
 
-    $ cubids-group BIDS_Dataset_DataLad v0
-
-This command will produce four tables that describe the dataset's
-heterogeneity in different ways.
-
-#. ``v0_summary.tsv`` contains all detected Key and Parameter groups and provides a high-level overview of the heterogeneity in the entire dataset.
-#. ``v0_files.tsv`` maps each imaging file in the BIDS directory to a Key and Parameter group.
-#. ``v0_AcqGrouping.tsv`` maps each session in the dataset to an Acquisition Group.
-#. ``v0_AcqGroupInfo.txt`` lists the set of scanning parameters present in each Acquisition Group.
-
-By first examining ``v0_summary.tsv`` users are given he opportunity to
-conduct metadata quality assurance (QA). The file can help identify
-instances of incomplete, incorrect, or unusable parameter groups,
-based on acquisition fields such as dimension and voxel sizes, number of volumes, obliquity, and more. 
-
-While ``v0_validation.tsv`` identified all the BIDS validation errors 
-present in the dataset, it did not identify any potential issues that
-might be present within the sidecars' metadata. Below, we see insances of missing
-metadata fields in a handful of sidecars, which may impact successful execution of BIDS Apps. 
+    $ cubids group BIDS_Dataset_DataLad v0
+
+This command will produce four tables that describe the dataset's heterogeneity in different ways.
+
+#.  ``v0_summary.tsv`` contains all detected Key and Parameter groups and provides a high-level
+    overview of the heterogeneity in the entire dataset.
+#.  ``v0_files.tsv`` maps each imaging file in the BIDS directory to a Key and Parameter group.
+#.  ``v0_AcqGrouping.tsv`` maps each session in the dataset to an Acquisition Group.
+#.  ``v0_AcqGroupInfo.txt`` lists the set of scanning parameters present in each Acquisition Group.
+
+By first examining ``v0_summary.tsv`` users are given he opportunity to conduct metadata
+quality assurance (QA).
+The file can help identify instances of incomplete, incorrect, or unusable parameter groups,
+based on acquisition fields such as dimension and voxel sizes, number of volumes, obliquity, and more.
+
+While ``v0_validation.tsv`` identified all the BIDS validation errors present in the dataset,
+it did not identify any potential issues that might be present within the sidecars' metadata.
+Below, we see insances of missing metadata fields in a handful of sidecars,
+which may impact successful execution of BIDS Apps.
 
 .. csv-table:: v0_summary.tsv
    :file: _static/v0_summary.csv
    :widths: 3, 3, 3, 3, 3, 3, 3, 3, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4
    :header-rows: 1
 
-Examining ``v0_summary.tsv`` we can see that one DWI Parameter Group — ``acquisition-HASC55AP_datatype-dwi_suffix-dwi__2`` — contains
-only one scan (see "Counts" column) with only 10 volumes (see 
-"NumVolumes" column). Since the majority of DWI scans in this dataset 
-have 61 volumes, ``CuBIDS`` assigns this single scan to a "Variant"
-(i.e. non-dominant) Parameter Group, and automatically populates
-that Parameter Group's "RenameKeyGroup" column in ``v0_summary.tsv``
+Examining ``v0_summary.tsv`` we can see that one DWI Parameter Group —
+``acquisition-HASC55AP_datatype-dwi_suffix-dwi__2`` —
+contains only one scan (see "Counts" column) with only 10 volumes
+(see "NumVolumes" column).
+Since the majority of DWI scans in this dataset have 61 volumes,
+``CuBIDS`` assigns this single scan to a "Variant" (i.e. non-dominant) Parameter Group,
+and automatically populates that Parameter Group's "RenameKeyGroup" column in ``v0_summary.tsv``
 with a suggested name: ``acquisition-HASC55APVARIANTNumVolumes_datatype-dwi_suffix-dwi``.
-This time, though, we elect to remove this scan because it does not have enough volumes to be usable for most analyses. 
-To do this, we can either use ``cubids-purge`` again, *or* we could
-edit v0_summary.tsv by adding ``0`` to the ``MergeInto`` column
-in the row (Parameter Group) we want to remove. This will ensure all
-scans in that Parameter Group (in this example, just one scan) are removed. 
+This time, though,
+we elect to remove this scan because it does not have enough volumes to be usable for most analyses.
+To do this, we can either use ``cubids purge`` again,
+*or* we could edit v0_summary.tsv by adding ``0`` to the ``MergeInto`` column in the row
+(Parameter Group) we want to remove.
+This will ensure all scans in that Parameter Group (in this example, just one scan) are removed.
 
-Make this change and save this edited version of ``v0_summary.tsv`` as ``v0_edited_summary.tsv``, which will be passed to ``cubids-apply`` in our next 
-curation step. 
+Make this change and save this edited version of ``v0_summary.tsv`` as ``v0_edited_summary.tsv``,
+which will be passed to ``cubids apply`` in our next curation step.
 
 .. csv-table:: v0_edited_summary.tsv
    :file: _static/v0_edited_summary.csv
    :widths: 3, 3, 3, 3, 3, 3, 3, 3, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4
    :header-rows: 1
 
+
 Applying changes
------------------
+----------------
 
-Now that all metadata issues have been addressed — both validation and
-``CuBIDS`` summary — we are ready to rename our files based on their
-RenameKeyGroup values and apply the requested deletion in ``v0_edited_summary.tsv``. The ``cubids-apply`` 
-function renames scans in each Variant Parameter Group according to the metadata parameters with a flag “VARIANT”, which is useful 
-because the user will then be able to see, in each scan’s filename, which metadata parameters associated with that scan vary from 
-those in the acquisition’s Dominant Group. If the edited summary and files tsvs are located in
-the ``bids_dir/code/CuBIDS`` directory, the user may just pass in those filenames. 
+Now that all metadata issues have been addressed —
+both validation and ``CuBIDS`` summary —
+we are ready to rename our files based on their RenameKeyGroup values and
+apply the requested deletion in ``v0_edited_summary.tsv``.
+The ``cubids apply`` function renames scans in each Variant Parameter Group according
+to the metadata parameters with a flag “VARIANT”,
+which is useful because the user will then be able to see, in each scan's filename,
+which metadata parameters associated with that scan vary from those in the acquisition's Dominant Group.
+If the edited summary and files tsvs are located in the ``bids_dir/code/CuBIDS`` directory,
+the user may just pass in those filenames.
 Otherwise, specifying the path to those files is necessary.
-We can execute cubids-apply with the following command:
+We can execute ``cubids apply`` with the following command:
 
 .. code-block:: console
 
-    $ cubids-apply BIDS_Dataset_DataLad v0_edited_summary.tsv v0_files.tsv v1 --use-datalad
-
+    $ cubids apply BIDS_Dataset_DataLad v0_edited_summary.tsv v0_files.tsv v1 --use-datalad
 
 Checking our git log, we can see that our changes from apply have been saved.
 
 .. image:: _static/screenshot_7.png
 
-We can check the four grouping tsvs ``cubids-apply`` produces (``v1_*``) to ensure they look as 
-expected — that all files with variant scanning parameters have been renamed to indicate the parameters 
+We can check the four grouping tsvs ``cubids apply`` produces (``v1_*``) to ensure they look as expected —
+that all files with variant scanning parameters have been renamed to indicate the parameters
 that vary in the acquisition fields of their filenames.
 
+
 Exemplar testing
------------------
+----------------
 
-The curation of the dataset is complete; finally, it's time
-for pre-processing. To streamline this step, and as an added measure
-for reproducibility and quality assurance, ``CuBIDS`` facilitates this
-subsequent step through the creation of an *Exemplar Dataset*: a subset
-of the full dataset that spans the full variation of acquisitions and
+The curation of the dataset is complete; finally,
+it's time for pre-processing.
+To streamline this step, and as an added measure for reproducibility and quality assurance,
+``CuBIDS`` facilitates this subsequent step through the creation of an *Exemplar Dataset*:
+a subset of the full dataset that spans the full variation of acquisitions and
 parameters by including one subject from each Acquisition Group.
-By testing only one subject per Acquisition Group, users are able to
-pinpoint specific metadata values and scans that may trigger
-pipeline failures. These acquisition groups could then be evaluated in
-more detail and flagged for remediation or exclusion. The *Exemplar 
-Dataset* can easily be created with the ``cubids-copy-exemplars``
-command, to which we pass in ``v2_AcqGrouping.tsv`` as input
-(the post ``cubids-apply`` acquisition grouping tsv).
+By testing only one subject per Acquisition Group,
+users are able to pinpoint specific metadata values and scans that may trigger pipeline failures.
+These acquisition groups could then be evaluated in more detail and flagged for remediation or exclusion.
+The *Exemplar Dataset* can easily be created with the ``cubids copy-exemplars`` command,
+to which we pass in ``v2_AcqGrouping.tsv`` as input
+(the post ``cubids apply`` acquisition grouping tsv).
 
 .. code-block:: console
 
-    $ cubids-copy-exemplars BIDS_Dataset_DataLad Exemplar_Dataset v1_AcqGrouping.tsv --use-datalad
+    $ cubids copy-exemplars BIDS_Dataset_DataLad Exemplar_Dataset v1_AcqGrouping.tsv --use-datalad
 
-Since we used the ``use-datalad`` flag, ``Exemplar_Dataset`` is a DataLad dataset with the version history 
-tracked in its git log (see below): 
+Since we used the ``use-datalad`` flag,
+``Exemplar_Dataset`` is a DataLad dataset with the version history tracked in its git log (see below):
 
 .. image:: _static/screenshot_8.png
 
-Once a preprocessing pipeline completes successfully on the Exemplar Dataset, 
-the full dataset can be executed with confidence, as a pipeline's
-behavior on the full range of metadata heterogeneity in the dataset 
-will have already been discovered during exemplar testing. 
+Once a preprocessing pipeline completes successfully on the Exemplar Dataset,
+the full dataset can be executed with confidence,
+as a pipeline's behavior on the full range of metadata heterogeneity in the dataset
+will have already been discovered during exemplar testing.
```

### Comparing `cubids-1.0.9/docs/installation.rst` & `cubids-1.1.0/docs/installation.rst`

 * *Files 5% similar despite different names*

```diff
@@ -2,66 +2,73 @@
 
 .. _installationpage:
 
 ============
 Installation
 ============
 
-.. note::  We **strongly recommend** using ``CuBIDS`` with environment management. For this, we recommend 
-           `miniconda <https://docs.conda.io/en/latest/miniconda.html>`_ 
-           (`miniforge <https://github.com/conda-forge/miniforge>`_ for M1 Chip Mac Machines).
+.. note::
+    We **strongly recommend** using ``CuBIDS`` with environment management.
+    For this, we recommend `miniconda <https://docs.conda.io/en/latest/miniconda.html>`_
+    (`miniforge <https://github.com/conda-forge/miniforge>`_ for M1 Chip Mac Machines).
 
-Once you've installed conda, initialize a new conda environment (for example, named ``cubids``) as follows:
+Once you've installed conda,
+initialize a new conda environment (for example, named ``cubids``) as follows:
 
 .. code-block:: console
 
-    $ conda create -n cubids python=3.8
+    $ conda create -n cubids python=3.8 pip
     $ conda activate cubids
 
-You are now ready to install CuBIDS. You can do so in one of two ways. 
+You are now ready to install CuBIDS.
+You can do so in one of two ways.
 
 To obtain ``CuBIDS`` locally, we can use ``pip`` to download our software from the
 `Python Package Manager (Pypi) <https://pypi.org/project/cubids/>`_ by running the following commands:
 
 .. code-block:: console
 
     $ pip install CuBIDS
 
-Alternatively, you can clone the source code for ``CuBIDS`` from our `GitHub repository`_ 
-using the following command: 
+Alternatively,
+you can clone the source code for ``CuBIDS`` from our `GitHub repository`_ using the following command:
 
 .. code-block:: console
 
     $ git clone https://github.com/PennLINC/CuBIDS.git
 
 Once you have a copy of the source, you can install it with:
 
 .. code-block:: console
 
     $ cd CuBIDS
     $ pip install -e .
 
-
-We will now need to install some dependencies of ``CuBIDS``. To do this, we first must install 
-nodejs. We can accomplish this using the following command:
+We will now need to install some dependencies of ``CuBIDS``.
+To do this, we first must install nodejs.
+We can accomplish this using the following command:
 
 .. code-block:: console
 
     $ conda install nodejs
 
-Now that we have npm installed, we can install the ``bids-validator`` using the following command:
+Now that we have npm installed, we can install ``bids-validator`` using the following command:
 
 .. code-block:: console
 
     $ npm install -g bids-validator@1.7.2
 
-In our example walkthrough, we use ``bids-validator`` v1.7.2. using a different version of the 
-validator may result in slightly different validation tsv printouts, but ``CuBIDS`` is compatible with all 
-versions of the validator at or above v1.6.2.
-
-We also recommend using ``CuBIDS`` with the optional ``DatLad`` version control capabilities.
-We use ``DataLad`` throughout our walkthrough of the CuBIDS Workflow on :doc:`the Example Walkthrough page <example>`.
-To leverage the version control capabilities, you will need to install both ``DataLad`` and ``git-annex``, 
-the large file storage software ``DataLad`` runs under the hood. Installation instructions 
-for ``DataLad`` and ``git-annex`` can be found `here <https://handbook.datalad.org/en/latest/intro/installation.html>`_
+In our example walkthrough,
+we use ``bids-validator`` v1.7.2. using a different version of the
+validator may result in slightly different validation tsv printouts,
+but ``CuBIDS`` is compatible with all versions of the validator at or above v1.6.2.
+
+We also recommend using ``CuBIDS`` with the optional ``DataLad`` version control capabilities.
+We use ``DataLad`` throughout our walkthrough of the CuBIDS Workflow on
+:doc:`the Example Walkthrough page <example>`.
+To leverage the version control capabilities,
+you will need to install both ``DataLad`` and ``git-annex``,
+the large file storage software ``DataLad`` runs under the hood.
+Installation instructions for ``DataLad`` and ``git-annex`` can be found
+`here <https://handbook.datalad.org/en/latest/intro/installation.html>`_.
 
-.. _GitHub repository: https://github.com/PennLINC/CuBIDS
+.. _GitHub repository: https://github.com/PennLINC/CuBIDS
```

### Comparing `cubids-1.0.9/docs/make.bat` & `cubids-1.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cubids-1.0.9/docs/usage.rst` & `cubids-1.1.0/docs/usage.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,258 +1,282 @@
-==========================================
-Commands & Actions
-==========================================
+========================
+General Usage Guidelines
+========================
 
 Before we implement a ``CuBIDS`` workflow, let's define the terminology
 and take a look at some of the commands available in the software.
 
+
 More definitions
------------------
+----------------
+
 
 .. _keygroup:
 
 Key Group
 ~~~~~~~~~
 
-A *Key Group* is a unique set of BIDS key-value pairs, excluding identifiers such as
-subject and session. For example the files::
+A :term:`Key Group` is a unique set of BIDS key-value pairs,
+excluding identifiers such as subject and session.
+For example, the files::
 
     bids-root/sub-1/ses-1/func/sub-1_ses-1_acq-mb_dir-PA_task-rest_bold.nii.gz
     bids-root/sub-1/ses-2/func/sub-1_ses-2_acq-mb_dir_PA_task-rest_bold.nii.gz
     bids-root/sub-2/ses-1/func/sub-2_ses-1_acq-mb_dir-PA_task-rest_bold.nii.gz
 
-Would all share the same Key Group. If these scans were all acquired as a part of the same
-study on the same scanner with exactly the same acquisition parameters, this
-naming convention would suffice.
-
-However, in large multi-scanner, multi-site, or longitudinal studies where acquisition
-parameters change over time, it's possible that the same Key Group could comprise of
-scans that differ in important ways.
+Would all share the same Key Group.
+If these scans were all acquired as a part of the same study on the same scanner with
+exactly the same acquisition parameters,
+this naming convention would suffice.
+
+However, in large multi-scanner, multi-site,
+or longitudinal studies where acquisition parameters change over time,
+it's possible that the same Key Group could contain scans that differ in important ways.
 
 ``CuBIDS`` examines all acquisitions within a Key Group to see if there are any images
-that differ in a set of important acquisition parameters. The subsets of consistent
-acquisition parameter sets within a Key Group are called a :ref:`paramgroup`.
+that differ in a set of important acquisition parameters.
+The subsets of consistent acquisition parameter sets within a Key Group are called a :ref:`paramgroup`.
 
 
 .. _paramgroup:
 
 Parameter Group
 ~~~~~~~~~~~~~~~
 
-Even though two images may belong to the same Key Group and are valid BIDS, they
-may have images with different acquisition parameters. There is nothing fundamentally
-wrong with this — the ``bids-validator`` will often simply flag these differences,
-with a ``Warning``, but not necessarily suggest changes. That being said,
+A :term:`Parameter Group` is a subset of a Key Group that contains images with the same
+acquisition parameters.
+
+Even though two images may belong to the same Key Group and are valid BIDS,
+they may have images with different acquisition parameters.
+There is nothing fundamentally wrong with this —
+the ``bids-validator`` will often simply flag these differences with a ``Warning``,
+but not necessarily suggest changes.
+That being said,
 there can be detrimental consequences downstream if the different parameters cause the
 same preprocessing pipelines to configure differently to images of the same Key Group.
 
-Acquisition Group
-~~~~~~~~~~~~~~~~~
-
-Acquisition Groups are sets of subjects who's images belong to all the same Key and Parameter Groups. The Acquistion Groups that subjects belong to are listed in ``_AcqGrouping.csv``, while the Key Groups and Parameter Groups that define each Acquisition Group are noted in ``_AcqGroupingInfo.txt``.
-
 
 .. _acquisitiongroup:
 
 Acquisition Group
-~~~~~~~~~~~~~~~~~~
+~~~~~~~~~~~~~~~~~
+
+We define an :term:`Acquisition Group` as a collection of sessions across participants that
+contain the exact same set of Key and Parameter Groups.
+Since Key Groups are based on the BIDS filenames—
+and therefore both MRI image type and acquisition specific—
+each BIDS session directory contains images that belong to a set of Parameter Groups.
+CuBIDS assigns each session, or set of Parameter Groups,
+to an Acquisition Group such that all sessions in an Acquisition Group possesses an identical set of
+scan acquisitions and metadata parameters across all image modalities present in the dataset.
+We find Acquisition Groups to be a particularly useful categorization of BIDS data,
+as they identify homogeneous sets of sessions (not individual scans) in a large dataset.
+They are also useful for expediting the testing of pipelines;
+if a BIDS App runs successfully on a single subject from each Acquisition Group,
+one can be confident that it will handle all combinations of scanning parameters in the entire dataset.
+
+The Acquisition Groups that subjects belong to are listed in ``_AcqGrouping.csv``,
+while the Key Groups and Parameter Groups that define each Acquisition Group are noted in
+``_AcqGroupingInfo.txt``.
 
-We define an “Acquisition Group” as a collection of sessions across participants that contain the exact 
-same set of Key and Parameter Groups. Since Key Groups are based on the BIDS filenames—and therefore both 
-MRI image type and acquisition specific—each BIDS session directory contains images that belong to a set of 
-Parameter Groups. CuBIDS assigns each session––or set of Parameter Groups––to an Acquisition Group 
-such that all sessions in an Acquisition Group possesses an identical set of scan acquisitions and 
-metadata parameters across all image modalities present in the dataset. We find Acquisition Groups to be 
-a particularly useful categorization of BIDS data, as they identify homogeneous sets of sessions (not 
-individual scans) in a large dataset. They are also useful for expediting the testing of pipelines; if a 
-BIDS App runs successfully on a single subject from each Acquisition Group, one can be confident that it 
-will handle all combinations of scanning parameters in the entire dataset.
 
 .. _summaryfile:
 
 The ``_summary.tsv`` File
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
-This file contains all the detected Key Groups and Parameter Groups. It provides
-an opportunity to evaluate your data and decide how to handle heterogeneity.
+This file contains all the detected Key Groups and Parameter Groups.
+It provides an opportunity to evaluate your data and decide how to handle heterogeneity.
 
-Below is an example ``_summary.tsv`` of the run-1 DWI Key Group in the PNC [#f1]_. This
-reflects the original data that has been converted to BIDS using a heuristic. It is
-similar to what you will see when you first use this functionality:
+Below is an example ``_summary.tsv`` of the run-1 DWI Key Group in the PNC [#f1]_.
+This reflects the original data that has been converted to BIDS using a heuristic.
+It is similar to what you will see when you first use this functionality:
 
 .. csv-table:: Pre Apply Groupings
     :file: _static/PNC_pre_apply_summary_dwi_run1.csv
     :widths: 3, 3, 3, 3, 3, 3, 3, 3, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 3
     :header-rows: 1
 
 
 .. _filelistfile:
 
 The ``_files.tsv`` file
-~~~~~~~~~~~~~~~~~~~~~~~~~
+~~~~~~~~~~~~~~~~~~~~~~~
 
-This file contains one row per imaging file in the BIDS directory. You won't need to edit this file
-directly, but it keeps track of every file's assignment to Key and Parameter Groups.
+This file contains one row per imaging file in the BIDS directory.
+You won't need to edit this file directly,
+but it keeps track of every file's assignment to Key and Parameter Groups.
 
 
 .. _acqgrouptsv:
 
 Modifying Key and Parameter Group Assignments
 ---------------------------------------------
 
 Sometimes we see that there are important differences in acquisition parameters within a Key Group.
-If these differences impact how a pipeline will process the data, it makes sense to assign the scans
-in that Parameter Group to a different Key Group (i.e. assign them a different BIDS name). This can
-be accomplished by editing the empty columns in the `_summary.csv` file produced by ``cubids-group``.
+If these differences impact how a pipeline will process the data,
+it makes sense to assign the scans in that Parameter Group to a different Key Group
+(i.e., assign them a different BIDS name).
+This can be accomplished by editing the empty columns in the `_summary.csv` file produced by
+``cubids group``.
 
 Once the columns have been edited you can apply the changes to BIDS data using
 
 .. code-block:: console
 
-    $ cubids-apply /bids/dir keyparam_edited new_keyparam_prefix
+    $ cubids apply /bids/dir keyparam_edited new_keyparam_prefix
 
 The changes in ``keyparam_edited_summary.csv`` will be applied to the BIDS data in ``/bids/dir``
-and the new Key and Parameter groups will be saved to csv files starting with ``new_keyparam_prefix``. Note:
-fieldmaps keygroups with variant parameters will be identified but not renamed. 
-
+and the new Key and Parameter groups will be saved to csv files starting with ``new_keyparam_prefix``.
+Note: fieldmaps keygroups with variant parameters will be identified but not renamed.
 
 
 The ``_AcqGrouping.tsv`` file
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
+The ``_AcqGrouping.tsv`` file organizes the dataset by session and tags each one with its
+Acquisition Group number.
 
-The ``_AcqGrouping.tsv`` file organizes the dataset by session and tags each one with its Acquisition Group number.
 
 .. _acqgrouptxt:
 
 The ``_AcqGroupInfo.txt`` file
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-The ``_AcqGroupInfo.txt`` file lists all Key Groups that belong to a given Acquisition Group along with \
-the number of sessions each group possesses.
+The ``_AcqGroupInfo.txt`` file lists all Key Groups that belong to a given Acquisition Group
+along with the number of sessions each group possesses.
 
-Visualizing and summarizing metadata heterogenaity
-----------------------------------------------------
 
-Use ``cubids-group`` to generate your dataset's Key Groups and Parameter Groups:
+Visualizing and summarizing metadata heterogeneity
+--------------------------------------------------
+
+Use ``cubids group`` to generate your dataset's Key Groups and Parameter Groups:
 
 .. code-block:: console
 
-    $ cubids-group FULL/PATH/TO/BIDS/DIR FULL/PATH/TO/v0
+    $ cubids group FULL/PATH/TO/BIDS/DIR FULL/PATH/TO/v0
 
-This will output four files, including the summary and files tsvs described above, 
+This will output four files, including the summary and files tsvs described above,
 prefixed by the second argument ``v0``.
 
-Applying changes 
-------------------
 
-The ``cubids-apply`` program provides an easy way for users to manipulate their datasets. 
-Specifically, ``cubids-apply`` can rename files according to the users’ specification in a tracked 
-and organized way. Here, the summary.tsv functions as an interface modifications; users can mark 
-``Parameter Groups`` they want to rename (or delete) in a dedicated column of the summary.tsv and 
-pass that edited tsv as an argument to ``cubids-apply``.
+Applying changes
+----------------
+
+The ``cubids apply`` program provides an easy way for users to manipulate their datasets.
+Specifically,
+``cubids apply`` can rename files according to the users' specification in a tracked and organized way.
+Here, the summary.tsv functions as an interface modifications; users can mark
+``Parameter Groups`` they want to rename (or delete) in a dedicated column of the summary.tsv and
+pass that edited tsv as an argument to ``cubids apply``.
+
 
 Detecting Variant Groups
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+~~~~~~~~~~~~~~~~~~~~~~~~
+
+Additionally, ``cubids apply`` can automatically rename files in :term:`Variant Groups <Variant Group>`
+based on their scanning parameters that vary from those in their Key Groups'
+:term:`Dominant Parameter Groups <Dominant Group>`.
+Renaming is automatically suggested when the summary.tsv is generated from a ``cubids group`` run,
+with the suggested new name listed in the tsv's :term:`Rename Key Group` column.
+CuBIDS populates this column for all Variant Groups
+(e.g., every Parameter Group except the Dominant one).
+Specifically, CuBIDS will suggest renaming all non-dominant Parameter Group to include ``VARIANT*``
+in their acquisition field where ``*`` is the reason
+the Parameter Group varies from the Dominant Group.
+For example, when CuBIDS encounters a Parameter Group with a repetition time that varies from
+the one present in the Dominant Group,
+it will automatically suggest renaming all scans in that Variant Group to include
+``acquisition-VARIANTRepetitionTime`` in their filenames.
+When the user runs ``cubids apply``,
+filenames will get renamed according to the auto-generated names in the “Rename Key Group” column
+in the summary.tsv
 
-Additionally, cubids-apply can automatically rename files in ``Variant Groups`` based on their 
-scanning parameters that vary from those in their Key Groups’ Dominant Parameter Groups. Renaming 
-is automatically suggested when the summary.tsv is generated from a cubids-group run, with the suggested 
-new name listed in the tsv’s “Rename Key Group” column. CuBIDS populates this column for all Variant 
-Groups—e.g., every Parameter Group except the Dominant one. Specifically, CuBIDS will suggest renaming 
-all non-dominant Parameter Group to include VARIANT* in their acquisition field where * is the reason 
-the Parameter Group varies from the Dominant Group. For example, when CuBIDS encounters a Parameter 
-Group with a repetition time that varies from the one present in the Dominant Group, it will automatically 
-suggest renaming all scans in that Variant Group to include ``acquisition-VARIANTRepetitionTime`` in their 
-filenames. When the user runs ``cubids-apply``, filenames will get renamed according to the auto-generated 
-names in the “Rename Key Group” column in the summary.tsv
 
 Deleting a mistake
-~~~~~~~~~~~~~~~~~~~~~~
+~~~~~~~~~~~~~~~~~~
 
-To remove files in a Parameter Group from your BIDS data, you simply set the ``MergeInto`` value
-to ``0``. We see in our data that there is a strange scan that has a ``RepetitionTime`` of 12.3
-seconds and is also variant with respect to EffectiveEchoSpacing and EchoTime. We elect to remove this scan from 
-our dataset because we do not want these parameters to affect our analyses.
-To remove these files from your BIDS data, add a ``0`` to ``MergeInto`` and save the new tsv as ``v0_edited_summary.tsv``
+To remove files in a Parameter Group from your BIDS data,
+you simply set the ``MergeInto`` value to ``0``.
+We see in our data that there is a strange scan that has a ``RepetitionTime`` of 12.3
+seconds and is also variant with respect to EffectiveEchoSpacing and EchoTime.
+We elect to remove this scan from our dataset because we do not want these parameters to affect our
+analyses.
+To remove these files from your BIDS data,
+add a ``0`` to ``MergeInto`` and save the new tsv as ``v0_edited_summary.tsv``
 
 .. csv-table:: Pre Apply Groupings with Deletion Requested
     :file: _static/PNC_pre_apply_summary_dwi_run1_deletion.csv
     :widths: 3, 3, 3, 3, 3, 3, 3, 3, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 3
     :header-rows: 1
 
 In this example, users can apply the changes to BIDS data using the following command:
 
 .. code-block:: console
 
-    $ cubids-apply FULL/PATH/TO/BIDS/DIR FULL/PATH/TO/v0_edited_summary.tsv FULL/PATH/TO/v0_files.tsv FULL/PATH/TO/v1
+    $ cubids apply FULL/PATH/TO/BIDS/DIR FULL/PATH/TO/v0_edited_summary.tsv FULL/PATH/TO/v0_files.tsv FULL/PATH/TO/v1
 
 The changes in ``v0_edited_summary.tsv`` will be applied to the BIDS data
 and the new Key and Parameter Groups will be saved to tsv files starting with ``v1``.
 
 Applying these changes we would see:
 
 .. csv-table:: Post Apply Groupings
     :file: _static/PNC_post_apply_summary.csv
     :widths: 3, 3, 3, 3, 3, 3, 3, 3, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 3
     :header-rows: 1
-    
-	
-Command line tools
--------------------
-
-With that brief introduction done, we can introduce the full gamut
-of ``CuBIDS`` command line tools:
-
-.. autofunction:: cubids.cli.cubids_add_nifti_info
-.. autofunction:: cubids.cli.cubids_apply
-.. autofunction:: cubids.cli.cubids_copy_exemplars
-.. autofunction:: cubids.cli.cubids_datalad_save
-.. autofunction:: cubids.cli.cubids_group
-.. autofunction:: cubids.cli.cubids_print_metadata_fields
-.. autofunction:: cubids.cli.cubids_purge
-.. autofunction:: cubids.cli.cubids_remove_metadata_fields
-.. autofunction:: cubids.cli.cubids_undo
-.. autofunction:: cubids.cli.cubids_validate
 
 
 Customizable configuration
----------------------------
-``CuBIDS`` also features an optional, customizable, MRI image type-specific configuration file. 
-This file can be passed as an argument to cubids-group and cubids-apply using the ``–-config`` flag 
-and allows users to customize grouping settings based on MRI image type and parameter. Each ``Key Group`` 
-is associated with one (and only one) MRI image type, as BIDS filenames include MRI image type-specific values 
-as their suffixes. This easy-to-modify configuration file provides several benefits to curation. 
-First, it allows users to add and remove metadata parameters from the set that determines groupings. 
-This can be very useful if a user deems a specific metadata parameter irrelevant and wishes to collapse 
-variation based on that parameter into a single Parameter Group. Second, the configuration file allows 
-users to apply tolerances for parameters with numerical values. This functionality allows users to avoid 
-very small differences in scanning parameters (i.e., a TR of 3.0s vs 3.0001s) being split into different 
-``Parameter Groups``. Third, the configuration file allows users to determine which scanning parameters 
+--------------------------
+
+``CuBIDS`` also features an optional, customizable, MRI image type-specific configuration file.
+This file can be passed as an argument to ``cubids group`` and ``cubids apply``
+using the ``--config`` flag and allows users to customize grouping settings based on
+MRI image type and parameter.
+Each ``Key Group`` is associated with one (and only one) MRI image type,
+as BIDS filenames include MRI image type-specific values as their suffixes.
+
+This easy-to-modify configuration file provides several benefits to curation.
+First, it allows users to add and remove metadata parameters from the set that determines groupings.
+This can be very useful if a user deems a specific metadata parameter irrelevant and wishes to collapse
+variation based on that parameter into a single Parameter Group.
+Second, the configuration file allows users to apply tolerances for parameters with numerical values.
+This functionality allows users to avoid very small differences in scanning parameters
+(i.e., a TR of 3.0s vs 3.0001s)
+being split into different ``Parameter Groups``.
+Third, the configuration file allows users to determine which scanning parameters
 are listed in the acquisition field when auto-renaming is applied to ``Variant Groups``.
 
 
 Exemplar testing
------------------
-In addition to facilitating curation of large, heterogeneous BIDS datasets, ``CuBIDS`` also prepares 
-datasets for testing BIDS Apps. This portion of the ``CuBIDS`` workflow relies on the concept of the 
-Acquisition Group: a set of sessions that have identical scan types and metadata across all imaging 
-modalities present in the session set. Specifically, ``cubids-copy-exemplars`` copies one subject from each 
-Acquisition Group into a separate directory, which we call an ``Exemplar Dataset``. Since the ``Exemplar Dataset`` 
-contains one randomly selected subject from each unique Acquisition Group in the dataset, it will be a 
-valid BIDS dataset that spans the entire metadata parameter space of the full study. If users run 
-``cubids-copy-exemplars`` with the ``–-use-datalad`` flag, the program will ensure that the ``Exemplar Dataset`` 
-is tracked and saved in ``DataLad``. If the user chooses to forgo this flag, the ``Exemplar Dataset`` 
-will be a standard directory located on the filesystem. Once the ``Exemplar Dataset`` has been created, 
-a user can test it with a BIDS App (e.g., fMRIPrep or QSIPrep) to ensure that each unique set of scanning 
-parameters will pass through the pipelines successfully. Because BIDS Apps auto-configure workflows based 
-on the metadata encountered, they will process all scans in each ``Acquisition Group`` in the same way. By 
-first verifying that BIDS Apps perform as intended on the small sub-sample of participants present in the 
-``Exemplar Dataset`` (that spans the full variation of the metadata), users can confidently move forward 
-processing the data of the complete BIDS dataset. 
+----------------
 
+In addition to facilitating curation of large, heterogeneous BIDS datasets,
+``CuBIDS`` also prepares datasets for testing BIDS Apps.
+This portion of the ``CuBIDS`` workflow relies on the concept of the Acquisition Group:
+a set of sessions that have identical scan types and metadata across all imaging
+modalities present in the session set.
+Specifically, ``cubids copy-exemplars`` copies one subject from each
+Acquisition Group into a separate directory,
+which we call an ``Exemplar Dataset``.
+Since the ``Exemplar Dataset`` contains one randomly selected subject from each unique
+Acquisition Group in the dataset,
+it will be a valid BIDS dataset that spans the entire metadata parameter space of the full study.
+If users run ``cubids copy-exemplars`` with the ``--use-datalad`` flag,
+the program will ensure that the ``Exemplar Dataset`` is tracked and saved in ``DataLad``.
+If the user chooses to forgo this flag,
+the ``Exemplar Dataset`` will be a standard directory located on the filesystem.
+Once the ``Exemplar Dataset`` has been created,
+a user can test it with a BIDS App (e.g., fMRIPrep or QSIPrep)
+to ensure that each unique set of scanning parameters will pass through the pipelines successfully.
+Because BIDS Apps auto-configure workflows based on the metadata encountered,
+they will process all scans in each ``Acquisition Group`` in the same way.
+By first verifying that BIDS Apps perform as intended on the small sub-sample of participants
+present in the ``Exemplar Dataset`` (that spans the full variation of the metadata),
+users can confidently move forward processing the data of the complete BIDS dataset.
 
 In the next section, we'll introduce ``DataLad`` and walk through a real example.
 
 .. rubric:: Footnotes
 
-.. [#f1] PNC: `The Philadelphia Developmental Cohort <https://www.med.upenn.edu/bbl/philadelphianeurodevelopmentalcohort.html>`_.
+.. [#f1] PNC: `The Philadelphia Developmental Cohort <https://www.med.upenn.edu/bbl/philadelphianeurodevelopmentalcohort.html>`_.
```

### Comparing `cubids-1.0.9/tests/test_bond.py` & `cubids-1.1.0/cubids/tests/test_bond.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,165 +1,221 @@
-#!/usr/bin/env python
-
 """Tests for `cubids` package."""
-import sys
-sys.path.append("..")
-import shutil
-from copy import deepcopy
-import hashlib
+
 import json
-from pathlib import Path
-from pkg_resources import resource_filename as pkgrf
-import pytest
-from cubids import CuBIDS
-from cubids.validator import (build_validator_call,
-                       run_validator, parse_validator_output)
-from cubids.metadata_merge import (
-    merge_without_overwrite, merge_json_into_json)
-from math import nan
-import subprocess
-import csv
 import os
-import filecmp
-import nibabel as nb
+import subprocess
+from copy import deepcopy
+from pathlib import Path
+
 import numpy as np
 import pandas as pd
-import subprocess
+import pytest
 
-TEST_DATA = pkgrf("cubids", "testdata")
+from cubids.cubids import CuBIDS
+from cubids.metadata_merge import merge_json_into_json, merge_without_overwrite
+from cubids.tests.utils import (
+    _add_deletion,
+    _add_ext_files,
+    _edit_a_json,
+    _edit_a_nifti,
+    _get_json_string,
+    _remove_a_json,
+    file_hash,
+    get_data,
+)
+from cubids.validator import build_validator_call, parse_validator_output, run_validator
 
 COMPLETE_KEY_GROUPS = [
-    'acquisition-HASC55AP_datatype-dwi_suffix-dwi',
-    'acquisition-v4_datatype-fmap_fmap-magnitude1_suffix-magnitude1',
-    'acquisition-v4_datatype-fmap_fmap-magnitude2_suffix-magnitude2',
-    'acquisition-v4_datatype-fmap_fmap-phasediff_suffix-phasediff',
-    'datatype-anat_suffix-T1w',
-    'datatype-fmap_direction-PA_fmap-epi_suffix-epi',
-    'datatype-func_suffix-bold_task-rest']
-
-
-def get_data(tmp_path):
-    """Copy testing data to a local directory"""
-    data_root = tmp_path / "testdata"
-    shutil.copytree(TEST_DATA, str(data_root))
-    return data_root
+    "acquisition-HASC55AP_datatype-dwi_suffix-dwi",
+    "acquisition-v4_datatype-fmap_fmap-magnitude1_suffix-magnitude1",
+    "acquisition-v4_datatype-fmap_fmap-magnitude2_suffix-magnitude2",
+    "acquisition-v4_datatype-fmap_fmap-phasediff_suffix-phasediff",
+    "datatype-anat_suffix-T1w",
+    "datatype-fmap_direction-PA_fmap-epi_suffix-epi",
+    "datatype-func_suffix-bold_task-rest",
+]
 
 
 def test_ok_json_merge(tmp_path):
+    """Test ok_json_merge."""
     data_root = get_data(tmp_path)
 
     # Test that a successful merge can happen
-    dest_json = data_root / "inconsistent" / "sub-02" / \
-        "ses-phdiff" / "dwi" / "sub-02_ses-phdiff_acq-HASC55AP_dwi.json"
+    dest_json = (
+        data_root
+        / "inconsistent"
+        / "sub-02"
+        / "ses-phdiff"
+        / "dwi"
+        / "sub-02_ses-phdiff_acq-HASC55AP_dwi.json"
+    )
     orig_dest_json_content = _get_json_string(dest_json)
-    source_json = data_root / "inconsistent" / "sub-03" / \
-        "ses-phdiff" / "dwi" / "sub-03_ses-phdiff_acq-HASC55AP_dwi.json"
+    source_json = (
+        data_root
+        / "inconsistent"
+        / "sub-03"
+        / "ses-phdiff"
+        / "dwi"
+        / "sub-03_ses-phdiff_acq-HASC55AP_dwi.json"
+    )
 
     merge_return = merge_json_into_json(source_json, dest_json)
     assert merge_return == 0
     assert not _get_json_string(dest_json) == orig_dest_json_content
 
 
 def test_ok_json_merge_cli(tmp_path):
+    """Test ok_json_merge_cli."""
     data_root = get_data(tmp_path)
 
     # Test that a successful merge can happen
-    dest_json = data_root / "inconsistent" / "sub-02" / \
-        "ses-phdiff" / "dwi" / "sub-02_ses-phdiff_acq-HASC55AP_dwi.json"
+    dest_json = (
+        data_root
+        / "inconsistent"
+        / "sub-02"
+        / "ses-phdiff"
+        / "dwi"
+        / "sub-02_ses-phdiff_acq-HASC55AP_dwi.json"
+    )
     orig_dest_json_content = _get_json_string(dest_json)
-    source_json = data_root / "inconsistent" / "sub-03" / \
-        "ses-phdiff" / "dwi" / "sub-03_ses-phdiff_acq-HASC55AP_dwi.json"
-
-    merge_proc = subprocess.run(
-        ['bids-sidecar-merge', str(source_json), str(dest_json)])
+    source_json = (
+        data_root
+        / "inconsistent"
+        / "sub-03"
+        / "ses-phdiff"
+        / "dwi"
+        / "sub-03_ses-phdiff_acq-HASC55AP_dwi.json"
+    )
+
+    assert os.path.isfile(source_json)
+    assert os.path.isfile(dest_json)
+    merge_proc = subprocess.run(["bids-sidecar-merge", str(source_json), str(dest_json)])
     assert merge_proc.returncode == 0
     assert not _get_json_string(dest_json) == orig_dest_json_content
 
+
 def test_get_param_groups(tmp_path):
+    """Test get_param_groups."""
     data_root = get_data(tmp_path)
     bod = CuBIDS(data_root / "inconsistent", use_datalad=True)
-    tsv_prefix = str(tmp_path / "tsvs")
     key_groups = bod.get_key_groups()
     bod._cache_fieldmaps()
 
     for key_group in key_groups:
         ret = bod.get_param_groups_from_key_group(key_group)
-        assert sum(ret[1].Counts) == ret[1].loc[0, 'KeyGroupCount']
+        assert sum(ret[1].Counts) == ret[1].loc[0, "KeyGroupCount"]
+
 
 def test_copy_exemplars(tmp_path):
+    """Test copy_exemplars."""
     data_root = get_data(tmp_path)
     bod = CuBIDS(data_root / "complete", use_datalad=True)
     tsv_prefix = str(tmp_path / "tsvs")
-    bod.get_TSVs(tsv_prefix)
+    bod.get_tsvs(tsv_prefix)
     acq_group_tsv = tsv_prefix + "_AcqGrouping.tsv"
     print("ACQ GROUP PATH: ", acq_group_tsv)
     exemplars_dir = str(tmp_path / "exemplars")
-    print('EXEMPLARS DIR: ', exemplars_dir)
+    print("EXEMPLARS DIR: ", exemplars_dir)
     df = pd.read_table(acq_group_tsv)
 
     bod.copy_exemplars(exemplars_dir, acq_group_tsv, min_group_size=1)
 
     # check exemplar dir got created and has the correct number of subs
     cntr = 0
     for path in Path(exemplars_dir).glob("sub-*"):
         cntr += 1
     assert cntr == len(df.drop_duplicates(subset=["AcqGroup"]))
 
     # check that dataset_description.json got added
-    assert Path(exemplars_dir + '/dataset_description.json').exists()
+    assert Path(exemplars_dir + "/dataset_description.json").exists()
+
 
 def test_purge_no_datalad(tmp_path):
+    """Test purge_no_datalad."""
     data_root = get_data(tmp_path)
     scans = []
     scan_name = "sub-03/ses-phdiff/func/sub-03_ses-phdiff_task-rest_bold.nii.gz"
-    json_name = data_root / "complete" / "sub-03" / "ses-phdiff" \
-        / "func" / "sub-03_ses-phdiff_task-rest_bold.json"
+    json_name = (
+        data_root
+        / "complete"
+        / "sub-03"
+        / "ses-phdiff"
+        / "func"
+        / "sub-03_ses-phdiff_task-rest_bold.json"
+    )
     scans.append(scan_name)
     scans.append("sub-01/ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.nii.gz")
 
     # create and save .txt with list of scans
     purge_path = str(tmp_path / "purge_scans.txt")
-    with open(purge_path, 'w') as filehandle:
+    with open(purge_path, "w") as filehandle:
         for listitem in scans:
-            filehandle.write('%s\n' % listitem)
+            filehandle.write(f"{listitem}\n")
+
     bod = CuBIDS(data_root / "complete", use_datalad=False)
 
     assert Path(data_root / "complete" / scan_name).exists()
     assert Path(json_name).exists()
 
     # Check that IntendedFor purge worked
-    with open(str(data_root / "complete" / "sub-01" / "ses-phdiff" / "fmap" / "sub-01_ses-phdiff_acq-v4_phasediff.json")) as f:
+    with open(
+        str(
+            data_root
+            / "complete"
+            / "sub-01"
+            / "ses-phdiff"
+            / "fmap"
+            / "sub-01_ses-phdiff_acq-v4_phasediff.json"
+        )
+    ) as f:
         j_dict = json.load(f)
 
     assert "ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.nii.gz" in j_dict.values()
-    assert isinstance(j_dict['IntendedFor'], str)
+    assert isinstance(j_dict["IntendedFor"], str)
     # PURGE
     bod.purge(purge_path)
 
-    with open(str(data_root / "complete" / "sub-01" / "ses-phdiff" / "fmap" / "sub-01_ses-phdiff_acq-v4_phasediff.json")) as f:
+    with open(
+        str(
+            data_root
+            / "complete"
+            / "sub-01"
+            / "ses-phdiff"
+            / "fmap"
+            / "sub-01_ses-phdiff_acq-v4_phasediff.json"
+        )
+    ) as f:
         purged_dict = json.load(f)
 
     assert not Path(data_root / "complete" / scan_name).exists()
     assert not Path(json_name).exists()
     assert "ses-phdiff/dwi/sub-01_ses-phdiff_acq-HASC55AP_dwi.nii.gz" not in purged_dict.values()
-    assert isinstance(purged_dict['IntendedFor'], list)
-    assert purged_dict['IntendedFor'] == []
+    assert isinstance(purged_dict["IntendedFor"], list)
+    assert purged_dict["IntendedFor"] == []
+
 
 def test_purge(tmp_path):
+    """Test purge."""
     data_root = get_data(tmp_path)
     scans = []
     scan_name = "sub-03/ses-phdiff/func/sub-03_ses-phdiff_task-rest_bold.nii.gz"
-    json_name = data_root / "complete" / "sub-03" / "ses-phdiff" \
-        / "func" / "sub-03_ses-phdiff_task-rest_bold.json"
+    json_name = (
+        data_root
+        / "complete"
+        / "sub-03"
+        / "ses-phdiff"
+        / "func"
+        / "sub-03_ses-phdiff_task-rest_bold.json"
+    )
     scans.append(scan_name)
     purge_path = str(tmp_path / "purge_scans.txt")
 
-    with open(purge_path, 'w') as filehandle:
+    with open(purge_path, "w") as filehandle:
         for listitem in scans:
-            filehandle.write('%s\n' % listitem)
+            filehandle.write(f"{listitem}\n")
     bod = CuBIDS(data_root / "complete", use_datalad=True)
     bod.datalad_save()
 
     assert bod.is_datalad_clean()
     assert Path(data_root / "complete" / scan_name).exists()
     assert Path(json_name).exists()
 
@@ -167,264 +223,294 @@
     bod.purge(purge_path)
 
     assert not Path(scan_name).exists()
     assert not Path(json_name).exists()
 
 
 def test_bad_json_merge(tmp_path):
+    """Test bad_json_merge."""
     data_root = get_data(tmp_path)
 
     # Test that a successful merge can happen
-    dest_json = data_root / "inconsistent" / "sub-02" / \
-        "ses-phdiff" / "dwi" / "sub-02_ses-phdiff_acq-HASC55AP_dwi.json"
+    dest_json = (
+        data_root
+        / "inconsistent"
+        / "sub-02"
+        / "ses-phdiff"
+        / "dwi"
+        / "sub-02_ses-phdiff_acq-HASC55AP_dwi.json"
+    )
     orig_dest_json_content = _get_json_string(dest_json)
-    invalid_source_json = data_root / "inconsistent" / "sub-01" / \
-        "ses-phdiff" / "dwi" / "sub-01_ses-phdiff_acq-HASC55AP_dwi.json"
+    invalid_source_json = (
+        data_root
+        / "inconsistent"
+        / "sub-01"
+        / "ses-phdiff"
+        / "dwi"
+        / "sub-01_ses-phdiff_acq-HASC55AP_dwi.json"
+    )
 
     assert merge_json_into_json(invalid_source_json, dest_json) > 0
     assert _get_json_string(dest_json) == orig_dest_json_content
 
 
 def test_bad_json_merge_cli(tmp_path):
+    """Test bade_json_merge_cli."""
     data_root = get_data(tmp_path)
 
     # Test that a successful merge can happen
-    dest_json = data_root / "inconsistent" / "sub-02" / \
-        "ses-phdiff" / "dwi" / "sub-02_ses-phdiff_acq-HASC55AP_dwi.json"
+    dest_json = (
+        data_root
+        / "inconsistent"
+        / "sub-02"
+        / "ses-phdiff"
+        / "dwi"
+        / "sub-02_ses-phdiff_acq-HASC55AP_dwi.json"
+    )
     orig_dest_json_content = _get_json_string(dest_json)
-    invalid_source_json = data_root / "inconsistent" / "sub-01" / \
-        "ses-phdiff" / "dwi" / "sub-01_ses-phdiff_acq-HASC55AP_dwi.json"
+    invalid_source_json = (
+        data_root
+        / "inconsistent"
+        / "sub-01"
+        / "ses-phdiff"
+        / "dwi"
+        / "sub-01_ses-phdiff_acq-HASC55AP_dwi.json"
+    )
 
-    merge_proc = subprocess.run(
-        ['bids-sidecar-merge', str(invalid_source_json), str(dest_json)])
+    merge_proc = subprocess.run(["bids-sidecar-merge", str(invalid_source_json), str(dest_json)])
     assert merge_proc.returncode > 0
     assert _get_json_string(dest_json) == orig_dest_json_content
 
+
 def test_add_nifti_info_datalad(tmp_path):
+    """Test add_nifti_info_datalad."""
     data_root = get_data(tmp_path)
     bod = CuBIDS(data_root / "complete", use_datalad=True, force_unlock=True)
     tsv_prefix = str(tmp_path / "tsvs")
-    bod.get_TSVs(tsv_prefix)
+    bod.get_tsvs(tsv_prefix)
     summary_tsv = tsv_prefix + "_summary.tsv"
     summary_df = pd.read_table(summary_tsv)
     l_cols = summary_df.columns.tolist()
-    assert 'NumVolumes' not in l_cols
-    assert 'Obliquity' not in l_cols
+    assert "NumVolumes" not in l_cols
+    assert "Obliquity" not in l_cols
 
     # now add nifti info
     bod.add_nifti_info()
 
     found_fields = set()
     for json_file in Path(bod.path).rglob("*.json"):
-        if '.git' not in str(json_file):
+        if ".git" not in str(json_file):
             with open(json_file, "r") as jsonr:
                 metadata = json.load(jsonr)
             found_fields.update(metadata.keys())
-    assert 'NumVolumes' in found_fields
-    assert 'Obliquity' in found_fields
-    assert 'ImageOrientation' in found_fields
+    assert "NumVolumes" in found_fields
+    assert "Obliquity" in found_fields
+    assert "ImageOrientation" in found_fields
 
     # nifti_tsv_prefix = str(tmp_path / "nifti_tsvs")
-    # bod.get_TSVs(nifti_tsv_prefix)
+    # bod.get_tsvs(nifti_tsv_prefix)
     # nifti_summary_tsv = nifti_tsv_prefix + "_summary.tsv"
     # nifti_summary_df = pd.read_table(nifti_summary_tsv)
     # nifti_l_cols = nifti_summary_df.columns.tolist()
     # assert 'NumVolumes' in nifti_l_cols
     # assert 'Obliquity' in nifti_l_cols
     # assert 'ImageOrientation' in nifti_l_cols
 
+
 def test_add_nifti_info_no_datalad(tmp_path):
+    """Test add_nifti_info_no_datalad."""
     data_root = get_data(tmp_path)
     bod = CuBIDS(data_root / "complete", use_datalad=False, force_unlock=False)
     bod.add_nifti_info()
 
     found_fields = set()
     for json_file in Path(bod.path).rglob("*.json"):
-        if '.git' not in str(json_file):
+        if ".git" not in str(json_file):
             with open(json_file, "r") as jsonr:
                 metadata = json.load(jsonr)
             found_fields.update(metadata.keys())
-    assert 'NumVolumes' in found_fields
-    assert 'Obliquity' in found_fields
-    assert 'ImageOrientation' in found_fields
+    assert "NumVolumes" in found_fields
+    assert "Obliquity" in found_fields
+    assert "ImageOrientation" in found_fields
 
     # tsv_prefix = str(tmp_path / "tsvs")
-    # bod.get_TSVs(tsv_prefix)
+    # bod.get_tsvs(tsv_prefix)
     # summary_tsv = tsv_prefix + "_summary.tsv"
     # summary_df = pd.read_table(summary_tsv)
     # l_cols = summary_df.columns.tolist()
     # assert 'NumVolumes' in l_cols
     # assert 'Obliquity' in l_cols
 
-#TODO: add tests that return an error for invalid merge
+
+# TODO: add tests that return an error for invalid merge
+
+
 def test_tsv_merge_no_datalad(tmp_path):
+    """Test tsv_merge_no_datalad."""
     data_root = get_data(tmp_path)
     bod = CuBIDS(data_root / "inconsistent", use_datalad=False)
 
     # Get an initial grouping summary and files list
     tsv_prefix = str(tmp_path / "originals")
-    bod.get_TSVs(tsv_prefix)
+    bod.get_tsvs(tsv_prefix)
     original_summary_tsv = tsv_prefix + "_summary.tsv"
     original_files_tsv = tsv_prefix + "_files.tsv"
 
     # give tsv with no changes (make sure it does nothing)
-    bod.apply_tsv_changes(original_summary_tsv,
-                          original_files_tsv,
-                          str(tmp_path / "unmodified"))
+    bod.apply_tsv_changes(original_summary_tsv, original_files_tsv, str(tmp_path / "unmodified"))
 
     # these will not actually be equivalent because of the auto renames
-    assert file_hash(original_summary_tsv) != \
-           file_hash(tmp_path / "unmodified_summary.tsv")
+    assert file_hash(original_summary_tsv) != file_hash(tmp_path / "unmodified_summary.tsv")
 
     # Find the dwi with no FlipAngle
     summary_df = pd.read_table(original_summary_tsv)
-    fa_nan_dwi_row, = np.flatnonzero(
-        np.isnan(summary_df.FlipAngle) &
-        summary_df.KeyGroup.str.fullmatch(
-            "acquisition-HASC55AP_datatype-dwi_suffix-dwi"))
+    (fa_nan_dwi_row,) = np.flatnonzero(
+        np.isnan(summary_df.FlipAngle)
+        & summary_df.KeyGroup.str.fullmatch("acquisition-HASC55AP_datatype-dwi_suffix-dwi")
+    )
     # Find the dwi with and EchoTime ==
-    complete_dwi_row, = np.flatnonzero(
-        summary_df.KeyGroup.str.fullmatch(
-            "acquisition-HASC55AP_datatype-dwi_suffix-dwi") &
-        (summary_df.FlipAngle == 90.) &
-        (summary_df.EchoTime > 0.05))
-    cant_merge_echotime_dwi_row, = np.flatnonzero(
-        summary_df.KeyGroup.str.fullmatch(
-            "acquisition-HASC55AP_datatype-dwi_suffix-dwi") &
-        (summary_df.FlipAngle == 90.) &
-        (summary_df.EchoTime < 0.05))
+    (complete_dwi_row,) = np.flatnonzero(
+        summary_df.KeyGroup.str.fullmatch("acquisition-HASC55AP_datatype-dwi_suffix-dwi")
+        & (summary_df.FlipAngle == 90.0)
+        & (summary_df.EchoTime > 0.05)
+    )
+    (cant_merge_echotime_dwi_row,) = np.flatnonzero(
+        summary_df.KeyGroup.str.fullmatch("acquisition-HASC55AP_datatype-dwi_suffix-dwi")
+        & (summary_df.FlipAngle == 90.0)
+        & (summary_df.EchoTime < 0.05)
+    )
 
     # Set a legal MergeInto value. This effectively fills in data
     # where there was previously as missing FlipAngle
-    summary_df.loc[fa_nan_dwi_row, "MergeInto"] = summary_df.ParamGroup[
-        complete_dwi_row]
+    summary_df.loc[fa_nan_dwi_row, "MergeInto"] = summary_df.ParamGroup[complete_dwi_row]
 
     valid_tsv_file = tsv_prefix + "_valid_summary.tsv"
     summary_df.to_csv(valid_tsv_file, sep="\t", index=False)
 
     # about to apply merges!
 
-    bod.apply_tsv_changes(valid_tsv_file,
-                          original_files_tsv,
-                          str(tmp_path / "ok_modified"))
+    bod.apply_tsv_changes(valid_tsv_file, original_files_tsv, str(tmp_path / "ok_modified"))
 
-    assert not file_hash(original_summary_tsv) == \
-           file_hash(tmp_path / "ok_modified_summary.tsv")
+    assert not file_hash(original_summary_tsv) == file_hash(tmp_path / "ok_modified_summary.tsv")
 
     # Add an illegal merge to MergeInto
     summary_df.loc[cant_merge_echotime_dwi_row, "MergeInto"] = summary_df.ParamGroup[
-        complete_dwi_row]
+        complete_dwi_row
+    ]
     invalid_tsv_file = tsv_prefix + "_invalid_summary.tsv"
     summary_df.to_csv(invalid_tsv_file, sep="\t", index=False)
 
     with pytest.raises(Exception):
-        bod.apply_tsv_changes(invalid_tsv_file,
-                              str(tmp_path / "originals_files.tsv"),
-                              str(tmp_path / "ok_modified"))
+        bod.apply_tsv_changes(
+            invalid_tsv_file, str(tmp_path / "originals_files.tsv"), str(tmp_path / "ok_modified")
+        )
+
 
 def test_tsv_merge_changes(tmp_path):
+    """Test tsv_merge_changes."""
     data_root = get_data(tmp_path)
     bod = CuBIDS(data_root / "inconsistent", use_datalad=True)
     bod.datalad_save()
     assert bod.is_datalad_clean()
 
     # Get an initial grouping summary and files list
     tsv_prefix = str(tmp_path / "originals")
-    bod.get_TSVs(tsv_prefix)
+    bod.get_tsvs(tsv_prefix)
     original_summary_tsv = tsv_prefix + "_summary.tsv"
     original_files_tsv = tsv_prefix + "_files.tsv"
 
     # give tsv with no changes (make sure it does nothing except rename)
-    bod.apply_tsv_changes(original_summary_tsv,
-                          original_files_tsv,
-                          str(tmp_path / "unmodified"))
+    bod.apply_tsv_changes(original_summary_tsv, original_files_tsv, str(tmp_path / "unmodified"))
     orig = pd.read_table(original_summary_tsv)
     # TEST RenameKeyGroup column got populated CORRECTLY
     for row in range(len(orig)):
-        if orig.loc[row, 'ParamGroup'] != 1:
-            assert str(orig.loc[row, 'RenameKeyGroup']) != 'nan'
+        if orig.loc[row, "ParamGroup"] != 1:
+            assert str(orig.loc[row, "RenameKeyGroup"]) != "nan"
 
     # TESTING RENAMES GOT APPLIED
     applied = pd.read_table(str(tmp_path / "unmodified_summary.tsv"))
 
     applied_f = pd.read_table(str(tmp_path / "unmodified_files.tsv"))
     odd = []
     for row in range(len(applied_f)):
-        if 'VARIANT' in applied_f.loc[row, 'FilePath'] and 'VARIANT' not in applied_f.loc[row, 'KeyParamGroup']:
-            odd.append((applied_f.loc[row, 'FilePath']))
+        if (
+            "VARIANT" in applied_f.loc[row, "FilePath"]
+            and "VARIANT" not in applied_f.loc[row, "KeyParamGroup"]
+        ):
+            odd.append((applied_f.loc[row, "FilePath"]))
 
     occurrences = {}
     for row in range(len(applied_f)):
-        if applied_f.loc[row, 'FilePath'] in odd:
-            if applied_f.loc[row, 'FilePath'] in occurrences.keys():
-                occurrences[applied_f.loc[row, 'FilePath']].append(applied_f.loc[row, 'KeyParamGroup'])
+        if applied_f.loc[row, "FilePath"] in odd:
+            if applied_f.loc[row, "FilePath"] in occurrences.keys():
+                occurrences[applied_f.loc[row, "FilePath"]].append(
+                    applied_f.loc[row, "KeyParamGroup"]
+                )
             else:
-                occurrences[applied_f.loc[row, 'FilePath']] = [applied_f.loc[row, 'KeyParamGroup']]
+                occurrences[applied_f.loc[row, "FilePath"]] = [applied_f.loc[row, "KeyParamGroup"]]
 
     assert len(orig) == len(applied)
 
     renamed = True
-    new_keys = applied['KeyGroup'].tolist()
+    new_keys = applied["KeyGroup"].tolist()
     for row in range(len(orig)):
-        if orig.loc[row, 'Modality'] != 'fmap':
-            if str(orig.loc[row, 'RenameKeyGroup']) != 'nan' \
-                    and str(orig.loc[row, 'RenameKeyGroup']) not in new_keys:
-                print(orig.loc[row, 'RenameKeyGroup'])
+        if orig.loc[row, "Modality"] != "fmap":
+            if (
+                str(orig.loc[row, "RenameKeyGroup"]) != "nan"
+                and str(orig.loc[row, "RenameKeyGroup"]) not in new_keys
+            ):
+                print(orig.loc[row, "RenameKeyGroup"])
                 renamed = False
 
-    assert renamed == True
+    assert renamed
 
     # will no longer be equal because of auto rename!
-    assert file_hash(original_summary_tsv)!= \
-           file_hash(tmp_path / "unmodified_summary.tsv")
+    assert file_hash(original_summary_tsv) != file_hash(tmp_path / "unmodified_summary.tsv")
 
     # Find the dwi with no FlipAngle
     summary_df = pd.read_table(original_summary_tsv)
-    fa_nan_dwi_row, = np.flatnonzero(
-        np.isnan(summary_df.FlipAngle) &
-        summary_df.KeyGroup.str.fullmatch(
-            "acquisition-HASC55AP_datatype-dwi_suffix-dwi"))
+    (fa_nan_dwi_row,) = np.flatnonzero(
+        np.isnan(summary_df.FlipAngle)
+        & summary_df.KeyGroup.str.fullmatch("acquisition-HASC55AP_datatype-dwi_suffix-dwi")
+    )
     # Find the dwi with and EchoTime ==
-    complete_dwi_row, = np.flatnonzero(
-        summary_df.KeyGroup.str.fullmatch(
-            "acquisition-HASC55AP_datatype-dwi_suffix-dwi") &
-        (summary_df.FlipAngle == 90.) &
-        (summary_df.EchoTime > 0.05))
-    cant_merge_echotime_dwi_row, = np.flatnonzero(
-        summary_df.KeyGroup.str.fullmatch(
-            "acquisition-HASC55AP_datatype-dwi_suffix-dwi") &
-        (summary_df.FlipAngle == 90.) &
-        (summary_df.EchoTime < 0.05))
+    (complete_dwi_row,) = np.flatnonzero(
+        summary_df.KeyGroup.str.fullmatch("acquisition-HASC55AP_datatype-dwi_suffix-dwi")
+        & (summary_df.FlipAngle == 90.0)
+        & (summary_df.EchoTime > 0.05)
+    )
+    (cant_merge_echotime_dwi_row,) = np.flatnonzero(
+        summary_df.KeyGroup.str.fullmatch("acquisition-HASC55AP_datatype-dwi_suffix-dwi")
+        & (summary_df.FlipAngle == 90.0)
+        & (summary_df.EchoTime < 0.05)
+    )
 
     # Set a legal MergeInto value. This effectively fills in data
     # where there was previously as missing FlipAngle
-    summary_df.loc[fa_nan_dwi_row, "MergeInto"] = summary_df.ParamGroup[
-        complete_dwi_row]
+    summary_df.loc[fa_nan_dwi_row, "MergeInto"] = summary_df.ParamGroup[complete_dwi_row]
 
     valid_tsv_file = tsv_prefix + "_valid_summary.tsv"
     summary_df.to_csv(valid_tsv_file, sep="\t", index=False)
 
     # about to merge
-    bod.apply_tsv_changes(valid_tsv_file,
-                          original_files_tsv,
-                          str(tmp_path / "ok_modified"))
+    bod.apply_tsv_changes(valid_tsv_file, original_files_tsv, str(tmp_path / "ok_modified"))
 
-    assert not file_hash(original_summary_tsv) == \
-           file_hash(tmp_path / "ok_modified_summary.tsv")
+    assert not file_hash(original_summary_tsv) == file_hash(tmp_path / "ok_modified_summary.tsv")
 
     # Add an illegal merge to MergeInto
     summary_df.loc[cant_merge_echotime_dwi_row, "MergeInto"] = summary_df.ParamGroup[
-        complete_dwi_row]
+        complete_dwi_row
+    ]
     invalid_tsv_file = tsv_prefix + "_invalid_summary.tsv"
     summary_df.to_csv(invalid_tsv_file, sep="\t", index=False)
 
     with pytest.raises(Exception):
-        bod.apply_tsv_changes(invalid_tsv_file,
-                              str(tmp_path / "originals_files.tsv"),
-                              str(tmp_path / "ok_modified"))
+        bod.apply_tsv_changes(
+            invalid_tsv_file, str(tmp_path / "originals_files.tsv"), str(tmp_path / "ok_modified")
+        )
 
     # Make sure MergeInto == 0 deletes the param group and all associations
     # summary_df = pd.read_table(original_summary_tsv)
     # summary_df.loc[fa_nan_dwi_row, "MergeInto"] = 0
     # delete_group = summary_df.loc[fa_nan_dwi_row, "KeyParamGroup"]
 
     # # files_df = pd.read_table(original_files_tsv)
@@ -444,51 +530,54 @@
     # del_summary_tsv = str(tmp_path / "ok_deleted")
 
     # original_summary_tsv = tsv_prefix + "_summary.tsv"
     # original_files_tsv = tsv_prefix + "_files.tsv"
 
     # assert delete_group not in tmp_path / "ok_deleted_summary.tsv"
 
+
 def test_merge_without_overwrite():
+    """Test merge_without_overwrite."""
     meta1 = {
-        'ManualCheck': 1.0,
-        'RenameKeyGroup': np.nan,
-        'MergeInto': 2.0,
-        'KeyGroup': 'datatype-func_suffix-bold_task-rest',
-        'ParamGroup': 12,
-        'Counts': 2,
-        'DwellTime': 2.6e-06,
-        'EchoTime': 0.03,
-        'EffectiveEchoSpacing': 0.000580013,
-        'FieldmapKey00': 'acquisition-fMRI_datatype-fmap_direction-AP_fmap-epi_suffix-epi',
-        'FieldmapKey01': 'acquisition-fMRI_datatype-fmap_direction-PA_fmap-epi_run-1_suffix-epi',
-        'FieldmapKey02': 'acquisition-fMRI_datatype-fmap_direction-PA_fmap-epi_run-2_suffix-epi',
-        'FieldmapKey03': np.nan,
-        'FieldmapKey04': np.nan,
-        'FieldmapKey05': np.nan,
-        'FieldmapKey06': np.nan,
-        'FieldmapKey07': np.nan,
-        'FlipAngle': 31.0,
-        'IntendedForKey00': np.nan,
-        'IntendedForKey01': np.nan,
-        'IntendedForKey02': np.nan,
-        'IntendedForKey03': np.nan,
-        'IntendedForKey04': np.nan,
-        'IntendedForKey05': np.nan,
-        'IntendedForKey06': np.nan,
-        'IntendedForKey07': np.nan,
-        'IntendedForKey08': np.nan,
-        'IntendedForKey09': np.nan,
-        'MultibandAccelerationFactor': 6.0,
-        'NSliceTimes': 60,
-        'ParallelReductionFactorInPlane': np.nan,
-        'PartialFourier': 1.0,
-        'PhaseEncodingDirection': 'j-',
-        'RepetitionTime': 0.8,
-        'TotalReadoutTime': 0.0481411}
+        "ManualCheck": 1.0,
+        "RenameKeyGroup": np.nan,
+        "MergeInto": 2.0,
+        "KeyGroup": "datatype-func_suffix-bold_task-rest",
+        "ParamGroup": 12,
+        "Counts": 2,
+        "DwellTime": 2.6e-06,
+        "EchoTime": 0.03,
+        "EffectiveEchoSpacing": 0.000580013,
+        "FieldmapKey00": "acquisition-fMRI_datatype-fmap_direction-AP_fmap-epi_suffix-epi",
+        "FieldmapKey01": "acquisition-fMRI_datatype-fmap_direction-PA_fmap-epi_run-1_suffix-epi",
+        "FieldmapKey02": "acquisition-fMRI_datatype-fmap_direction-PA_fmap-epi_run-2_suffix-epi",
+        "FieldmapKey03": np.nan,
+        "FieldmapKey04": np.nan,
+        "FieldmapKey05": np.nan,
+        "FieldmapKey06": np.nan,
+        "FieldmapKey07": np.nan,
+        "FlipAngle": 31.0,
+        "IntendedForKey00": np.nan,
+        "IntendedForKey01": np.nan,
+        "IntendedForKey02": np.nan,
+        "IntendedForKey03": np.nan,
+        "IntendedForKey04": np.nan,
+        "IntendedForKey05": np.nan,
+        "IntendedForKey06": np.nan,
+        "IntendedForKey07": np.nan,
+        "IntendedForKey08": np.nan,
+        "IntendedForKey09": np.nan,
+        "MultibandAccelerationFactor": 6.0,
+        "NSliceTimes": 60,
+        "ParallelReductionFactorInPlane": np.nan,
+        "PartialFourier": 1.0,
+        "PhaseEncodingDirection": "j-",
+        "RepetitionTime": 0.8,
+        "TotalReadoutTime": 0.0481411,
+    }
 
     # Suppose User tries to overwrite num with NaN (allowed)
     meta_NaN = deepcopy(meta1)
     meta_NaN["FlipAngle"] = np.nan
     valid_merge = merge_without_overwrite(meta_NaN, meta1)
     assert valid_merge
 
@@ -510,14 +599,15 @@
     slices_bad["PartialFourier"] = np.nan
     slices_bad["NSliceTimes"] = meta1["NSliceTimes"] + 5
     bad_slice_merge = merge_without_overwrite(meta1, slices_bad)
     assert not bad_slice_merge
 
 
 def test_keygroups(tmp_path):
+    """Test keygroups."""
     data_root = get_data(tmp_path)
 
     # Test the complete data
     complete_bod = CuBIDS(data_root / "complete")
     complete_misfit_fmaps = complete_bod._cache_fieldmaps()
     # There should be no unpaired fieldmaps
     assert len(complete_misfit_fmaps) == 0
@@ -533,167 +623,160 @@
 
     # There will still be the same number of key groups
     ikey_groups = ibod.get_key_groups()
     assert ikey_groups == COMPLETE_KEY_GROUPS
 
 
 def test_tsv_creation(tmp_path):
-    """Test the Key Group and Parameter Group creation on sample data.
-    """
+    """Test the Key Group and Parameter Group creation on sample data."""
     data_root = get_data(tmp_path)
 
     # Test the complete data
     complete_bod = CuBIDS(data_root / "complete")
     complete_misfit_fmaps = complete_bod._cache_fieldmaps()
     # There should be no unpaired fieldmaps
     assert len(complete_misfit_fmaps) == 0
 
     # Test that the correct key groups are found
     key_groups = complete_bod.get_key_groups()
     assert key_groups == COMPLETE_KEY_GROUPS
 
     # Get the tsvs from the complete data
-    cfiles_df, csummary_df = \
-        complete_bod.get_param_groups_dataframes()
+    cfiles_df, csummary_df = complete_bod.get_param_groups_dataframes()
 
     # Make sure we got all 21 of the files
     assert cfiles_df.shape[0] == 21
 
     # This data should have the same number of param
     # groups as key groups
     assert csummary_df.shape[0] == len(COMPLETE_KEY_GROUPS)
 
     # check IntendedForXX and FieldmapKeyXX are boolean now
     bool_IF = False
     bool_FMAP = False
     for row in range(len(csummary_df)):
         if str(csummary_df.loc[row, "UsedAsFieldmap"]) == "True":
             bool_IF = True
+
         if str(csummary_df.loc[row, "HasFieldmap"]) == "True":
             bool_FMAP = True
-    assert bool_IF == True
-    assert bool_FMAP == True
+
+    assert bool_IF
+    assert bool_FMAP
 
     # Test the incomplete
     ibod = CuBIDS(data_root / "inconsistent")
     inc_misfit_fmaps = ibod._cache_fieldmaps()
     assert len(inc_misfit_fmaps) == 1
 
     # There will still be the same number of key groups
     ikey_groups = ibod.get_key_groups()
     assert ikey_groups == COMPLETE_KEY_GROUPS
 
     # Get the tsvs from the inconsistent data
-    ifiles_df, isummary_df = \
-        ibod.get_param_groups_dataframes()
+    ifiles_df, isummary_df = ibod.get_param_groups_dataframes()
 
     # There are still 21 files
     assert ifiles_df.shape[0] == 21
 
     # But now there are more parameter groups
     assert isummary_df.shape[0] == 12
 
     # check that summary tsv param group nums are in the right order
     # and check that param groups are sorted by count vals
-    for i, (index, row) in enumerate(isummary_df.iterrows()):
-        if i == len(isummary_df) -1:
+    for i, (_, row) in enumerate(isummary_df.iterrows()):
+        if i == len(isummary_df) - 1:
             break
         # if key groups in rows i and i+1 are the same
-        if isummary_df.iloc[i]['KeyGroup'] == \
-            isummary_df.iloc[i+1]['KeyGroup']:
+        if isummary_df.iloc[i]["KeyGroup"] == isummary_df.iloc[i + 1]["KeyGroup"]:
             # param group i = param group i+1
-            assert isummary_df.iloc[i]['ParamGroup'] == \
-                isummary_df.iloc[i+1]['ParamGroup'] - 1
+            assert isummary_df.iloc[i]["ParamGroup"] == isummary_df.iloc[i + 1]["ParamGroup"] - 1
             # and count i < count i + 1
-            assert isummary_df.iloc[i]['Counts'] >= \
-                isummary_df.iloc[i+1]['Counts']
+            assert isummary_df.iloc[i]["Counts"] >= isummary_df.iloc[i + 1]["Counts"]
 
     # check that files tsv param group nums are in the right order
-    for i, (index, row) in enumerate(ifiles_df.iterrows()):
-        if i == len(ifiles_df) -1:
+    for i, (_, row) in enumerate(ifiles_df.iterrows()):
+        if i == len(ifiles_df) - 1:
             break
         # if key groups in rows i and i+1 are the same
-        if ifiles_df.iloc[i]['KeyGroup'] == \
-            ifiles_df.iloc[i+1]['KeyGroup']:
+        if ifiles_df.iloc[i]["KeyGroup"] == ifiles_df.iloc[i + 1]["KeyGroup"]:
             # param group i = param group i+1
-            assert ifiles_df.iloc[i]['ParamGroup'] <= \
-                ifiles_df.iloc[i+1]['ParamGroup']
+            assert ifiles_df.iloc[i]["ParamGroup"] <= ifiles_df.iloc[i + 1]["ParamGroup"]
 
 
 def test_apply_tsv_changes(tmp_path):
+    """Test apply_tsv_changes."""
     # set up like narrative of user using this
     # similar to test tsv creation
     # open the tsv, rename a key group
     # save tsv
     # call change key groups
     # give tsv with no changes (make sure it does nothing)
     # make sure files you wanted to rename exist in the bids dir
 
     data_root = get_data(tmp_path)
     bids_dir = str(data_root / "complete")
-    for scan in Path(bids_dir).rglob('sub-*/*/*/*.nii.gz'):
-
+    for scan in Path(bids_dir).rglob("sub-*/*/*/*.nii.gz"):
         # add extension files
         _add_ext_files(str(scan))
 
-    # path_to_img = str(data_root / "complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude1.nii.gz")
+    # path_to_img = str(
+    #    data_root / "complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude1.nii.gz"
+    # )
     # _add_ext_files(path_to_img)
 
-    has_events = False
-    has_physio = False
-
-    # check if events and physio files
-    if Path(data_root /
-            "complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_events.tsv").exists():
-        has_events = True
-    if Path(data_root /
-            "complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_physio.tsv.gz").exists():
-        has_physio = True
-
-
     complete_cubids = CuBIDS(data_root / "complete", use_datalad=True)
     complete_cubids.datalad_save()
 
-    complete_cubids.get_TSVs(str(tmp_path / "originals"))
+    complete_cubids.get_tsvs(str(tmp_path / "originals"))
 
     # give tsv with no changes (make sure it does nothing)
-    complete_cubids.apply_tsv_changes(str(tmp_path / "originals_summary.tsv"),
-                                    str(tmp_path / "originals_files.tsv"),
-                                    str(tmp_path / "modified1"))
+    complete_cubids.apply_tsv_changes(
+        str(tmp_path / "originals_summary.tsv"),
+        str(tmp_path / "originals_files.tsv"),
+        str(tmp_path / "modified1"),
+    )
 
     og_path = tmp_path / "originals_summary.tsv"
     with og_path.open("r") as f:
         og_content = "".join(f.readlines())
 
     mod1_path = tmp_path / "modified1_summary.tsv"
     with mod1_path.open("r") as f:
         mod1_content = "".join(f.readlines())
 
     assert og_content == mod1_content
 
     # edit the tsv, add a RenameKeyGroup
 
     # _edit_tsv(str(tmp_path / "originals_summary.tsv"))
-    complete_cubids.apply_tsv_changes(str(tmp_path / "originals_summary.tsv"),
-                                    str(tmp_path / "originals_files.tsv"),
-                                    str(tmp_path / "modified2"))
+    complete_cubids.apply_tsv_changes(
+        str(tmp_path / "originals_summary.tsv"),
+        str(tmp_path / "originals_files.tsv"),
+        str(tmp_path / "modified2"),
+    )
 
     # check files df to make sure extension files also got renmaed
-    mod_files = tmp_path / "modified2_files.tsv"
+    # mod_files = tmp_path / "modified2_files.tsv"
     # ensure fmap didn't get renamed
-    # assert Path(data_root /
-    #     "complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v5_magnitude1.json").exists() == False
-    assert Path(data_root /
-        "complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude1.json").exists() == True
+    # assert not Path(
+    #    data_root /
+    #    "complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v5_magnitude1.json"
+    # ).exists()
+    assert Path(
+        data_root / "complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_magnitude1.json"
+    ).exists()
 
     # check that old names are gone!
-    # assert Path(data_root /
-    #     "complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v5_physio.tsv.gz").exists() == True
-    assert Path(data_root /
-        "complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_physio.tsv.gz").exists() == True
+    # assert Path(
+    #    data_root / "complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v5_physio.tsv.gz"
+    # ).exists()
+    assert Path(
+        data_root / "complete/sub-01/ses-phdiff/fmap/sub-01_ses-phdiff_acq-v4_physio.tsv.gz"
+    ).exists()
 
     mod2_path = tmp_path / "modified2_summary.tsv"
     with mod2_path.open("r") as f:
         mod2_content = "".join(f.readlines())
 
     assert og_content == mod2_content
 
@@ -704,30 +787,30 @@
     # check to delete keyparam  exist
     mod2_files = tmp_path / "modified2_files.tsv"
     with mod2_files.open("r") as f:
         mod2_f_content = "".join(f.readlines())
     assert deleted_keyparam in mod2_f_content
 
     # check scans and associations to be deleted are currently in the bids dir
-    mod2_summary_df = pd.read_table(mod2_path)
+    # mod2_summary_df = pd.read_table(mod2_path)
     mod2_files_df = pd.read_table(str(tmp_path / "modified2_files.tsv"))
     deleted_f = []
 
     for row in range(len(mod2_files_df)):
-        if mod2_files_df.loc[row, 'KeyParamGroup'] == deleted_keyparam:
-            deleted_f.append(mod2_files_df.loc[row, 'FilePath'])
+        if mod2_files_df.loc[row, "KeyParamGroup"] == deleted_keyparam:
+            deleted_f.append(mod2_files_df.loc[row, "FilePath"])
 
     for f in deleted_f:
-        assert Path(str(data_root / "complete") + f).exists() == True
-        assert Path(str(data_root / "complete") + f.replace('nii.gz', 'json')).exists() == True
+        assert Path(str(data_root / "complete") + f).exists()
+        assert Path(str(data_root / "complete") + f.replace("nii.gz", "json")).exists()
 
     # apply deletion
-    complete_cubids.apply_tsv_changes(mod2_path,
-                                    str(tmp_path / "modified2_files.tsv"),
-                                    str(tmp_path / "deleted"))
+    complete_cubids.apply_tsv_changes(
+        mod2_path, str(tmp_path / "modified2_files.tsv"), str(tmp_path / "deleted")
+    )
 
     # make sure deleted_keyparam gone from files_tsv
     deleted = tmp_path / "deleted_summary.tsv"
     with deleted.open("r") as f:
         deleted_content = "".join(f.readlines())
     assert deleted_keyparam not in deleted_content
 
@@ -735,171 +818,119 @@
     deleted_files = tmp_path / "deleted_files.tsv"
     with deleted_files.open("r") as f:
         deleted_f_content = "".join(f.readlines())
     assert deleted_keyparam not in deleted_f_content
 
     # make sure deleted files are gone
     for f in deleted_f:
-        assert Path(f).exists() == False
-        assert Path(f.replace('nii.gz', 'json')).exists() == False
+        assert not Path(f).exists()
+        assert not Path(f.replace("nii.gz", "json")).exists()
 
 
 def test_session_apply(tmp_path):
+    """Test session_apply."""
     # set up like narrative of user using this
     # similar to test tsv creation
     # open the tsv, rename a key group
     # save tsv
     # call change key groups
     # give tsv with no changes (make sure it does nothing)
     # make sure files you wanted to rename exist in the bids dir
 
     data_root = get_data(tmp_path)
-    bids_dir = str(data_root / "inconsistent")
 
-    ses_cubids = CuBIDS(data_root / "inconsistent", acq_group_level='session', use_datalad=True)
+    ses_cubids = CuBIDS(data_root / "inconsistent", acq_group_level="session", use_datalad=True)
 
-    ses_cubids.get_TSVs(str(tmp_path / "originals"))
+    ses_cubids.get_tsvs(str(tmp_path / "originals"))
 
     # give tsv and make sure 'session' is in summary both pre and post apply
-    ses_cubids.apply_tsv_changes(str(tmp_path / "originals_summary.tsv"),
-                                    str(tmp_path / "originals_files.tsv"),
-                                    str(tmp_path / "modified1"))
+    ses_cubids.apply_tsv_changes(
+        str(tmp_path / "originals_summary.tsv"),
+        str(tmp_path / "originals_files.tsv"),
+        str(tmp_path / "modified1"),
+    )
 
     og_path = tmp_path / "originals_summary.tsv"
     with og_path.open("r") as f:
         og_content = "".join(f.readlines())
 
     mod1_path = tmp_path / "modified1_summary.tsv"
     with mod1_path.open("r") as f:
         mod1_content = "".join(f.readlines())
 
-    assert 'session-' in og_content
-    assert 'session-' in mod1_content
-
-
-
-def _add_deletion(summary_tsv):
-    df = pd.read_table(summary_tsv)
-    df.loc[3, 'MergeInto'] = 0
-    df.to_csv(summary_tsv, sep="\t", index=False)
-    return df.loc[3, 'KeyParamGroup']
-
-
-# def _edit_tsv(summary_tsv):
-#     df = pd.read_table(summary_tsv)
-#     df['RenameKeyGroup'] = df['RenameKeyGroup'].apply(str)
-#     df['KeyGroup'] = df['KeyGroup'].apply(str)
-#     for row in range(len(df)):
-#         if df.loc[row, 'KeyGroup'] == \
-#             "acquisition-v4_datatype-fmap_fmap-magnitude1_suffix-magnitude1":
-#             df.at[row, 'RenameKeyGroup'] = \
-#                 "acquisition-v5_datatype-fmap_fmap-magnitude1_suffix-magnitude1"
-#     df.to_csv(summary_tsv)
-
-def _add_ext_files(img_path):
-    # add and save extension files in
-    dwi_exts = ['.bval', '.bvec']
-
-    # everyone gets a physio file
-    no_suffix = img_path.rpartition('_')[0]
-    physio_file = no_suffix + '_physio' + '.tsv.gz'
-    # save ext file in img_path's parent dir
-    Path(physio_file).touch()
-
-    if '/dwi/' in img_path:
-        # add bval and bvec
-        for ext in dwi_exts:
-            dwi_ext_file = img_path.replace(".nii.gz", "").replace(".nii", "") + ext
-            Path(dwi_ext_file).touch()
-    if 'bold' in img_path:
-        no_suffix = img_path.rpartition('_')[0]
-        bold_ext_file = no_suffix + '_events' + '.tsv'
-        Path(bold_ext_file).touch()
-
-
-def _edit_a_json(json_file):
-    """Open a json file, write something to it and save it to the same name."""
-    with open(json_file, "r") as metadatar:
-        metadata = json.load(metadatar)
-
-    metadata["THIS_IS_A_TEST"] = True
-    with open(json_file, "w") as metadataw:
-        json.dump(metadata, metadataw)
-
-
-def _edit_a_nifti(nifti_file):
-    img = nb.load(nifti_file)
-    new_img = nb.Nifti1Image(np.random.rand(*img.shape),
-                             affine=img.affine,
-                             header=img.header)
-    new_img.to_filename(nifti_file)
-
-
-def file_hash(file_name):
-    with open(str(file_name), 'rb') as fcheck:
-        data = fcheck.read()
-    return hashlib.md5(data).hexdigest()
-
-
-def _get_json_string(json_path):
-    with json_path.open("r") as f:
-        content = "".join(f.readlines())
-    return content
+    assert "session-" in og_content
+    assert "session-" in mod1_content
 
 
 def test_remove_fields(tmp_path):
     """Test that we metadata fields are detected and removed."""
     data_root = get_data(tmp_path)
     bod = CuBIDS(data_root, use_datalad=False)
 
     # Get the metadata fields
     metadata_fields = bod.get_all_metadata_fields()
     assert metadata_fields
 
     # Simulate some fields we might want to remove
-    fields_to_remove = ["DeviceSerialNumber", "AcquisitionTime",
-                        "InstitutionAddress", "InstitutionName",
-                        "StationName", "NotARealField"]
+    fields_to_remove = [
+        "DeviceSerialNumber",
+        "AcquisitionTime",
+        "InstitutionAddress",
+        "InstitutionName",
+        "StationName",
+        "NotARealField",
+    ]
 
     bod.remove_metadata_fields(fields_to_remove)
     new_fields = bod.get_all_metadata_fields()
     assert not set(new_fields).intersection(fields_to_remove)
 
 
 def test_datalad_integration(tmp_path):
-    """Test that datalad works for basic file modification operations.
-    """
+    """Test that datalad works for basic file modification operations."""
     data_root = get_data(tmp_path)
 
     # Test that an uninitialized CuBIDS raises exceptions
     uninit_cubids = CuBIDS(data_root / "complete", use_datalad=False)
 
     # Ensure an exception is raised if trying to use datalad without
     # initializing
     with pytest.raises(Exception):
         uninit_cubids.is_datalad_clean()
 
     # initialize the datalad repository and try again
     uninit_cubids.init_datalad()
-    uninit_cubids.datalad_save('Test save')
+    uninit_cubids.datalad_save("Test save")
     assert uninit_cubids.is_datalad_clean()
 
     # Now, the datalad repository is initialized and saved.
     # Make sure if we make a new CuBIDS object it recognizes that
     # the datalad status is OK
     complete_bod = CuBIDS(data_root / "complete", use_datalad=True)
 
     assert complete_bod.datalad_ready
     assert complete_bod.is_datalad_clean()
 
     # Test clean and revert functionality
-    test_file = data_root / "complete" / "sub-03" / "ses-phdiff" \
-        / "func" / "sub-03_ses-phdiff_task-rest_bold.json"
-    test_binary = data_root / "complete" / "sub-03" / "ses-phdiff" \
-        / "func" / "sub-03_ses-phdiff_task-rest_bold.nii.gz"
+    test_file = (
+        data_root
+        / "complete"
+        / "sub-03"
+        / "ses-phdiff"
+        / "func"
+        / "sub-03_ses-phdiff_task-rest_bold.json"
+    )
+    test_binary = (
+        data_root
+        / "complete"
+        / "sub-03"
+        / "ses-phdiff"
+        / "func"
+        / "sub-03_ses-phdiff_task-rest_bold.nii.gz"
+    )
 
     # Try editing a locked file - it should fail
     with pytest.raises(Exception):
         _edit_a_nifti(test_binary)
 
     # Unlock the files so we can access their content
     complete_bod.datalad_handle.unlock(test_binary)
@@ -945,83 +976,87 @@
     restored_binary_content = file_hash(test_binary)
 
     # Check that the file content has returned to its original state
     assert original_content == restored_content
     assert original_binary_content == restored_binary_content
 
 
-def _remove_a_json(json_file):
-
-    os.remove(json_file)
-
-
 def test_validator(tmp_path):
-
+    """Test validator."""
     data_root = get_data(tmp_path)
 
     # test the validator in valid dataset
     call = build_validator_call(str(data_root) + "/complete")
     ret = run_validator(call)
 
     assert ret.returncode == 0
-    parsed = parse_validator_output(ret.stdout.decode('UTF-8'))
-
+    parsed = parse_validator_output(ret.stdout.decode("UTF-8"))
 
     # change this assert
     # assert parsed.shape[1] < 1
 
-
     # bungle some data and test
 
     # get data
-    test_file = data_root / "complete" / "sub-03" / "ses-phdiff" \
-        / "func" / "sub-03_ses-phdiff_task-rest_bold.json"
-    test_binary = data_root / "complete" / "sub-03" / "ses-phdiff" \
-        / "func" / "sub-03_ses-phdiff_task-rest_bold.nii.gz"
+    test_file = (
+        data_root
+        / "complete"
+        / "sub-03"
+        / "ses-phdiff"
+        / "func"
+        / "sub-03_ses-phdiff_task-rest_bold.json"
+    )
+    test_binary = (
+        data_root
+        / "complete"
+        / "sub-03"
+        / "ses-phdiff"
+        / "func"
+        / "sub-03_ses-phdiff_task-rest_bold.nii.gz"
+    )
 
     # Edit the files
     _edit_a_nifti(test_binary)
     _remove_a_json(test_file)
 
     call = build_validator_call(str(data_root) + "/complete")
     ret = run_validator(call)
 
     assert ret.returncode == 1
 
-    parsed = parse_validator_output(ret.stdout.decode('UTF-8'))
+    parsed = parse_validator_output(ret.stdout.decode("UTF-8"))
 
-    assert type(parsed) == pd.core.frame.DataFrame
+    assert isinstance(parsed, pd.DataFrame)
 
 
 def test_docker():
-    """Verify that docker is installed and the user has permission to
-    run docker images.
+    """Verify that docker is installed and the user has permission to run docker images.
+
     Returns
     -------
     -1  Docker can't be found
      0  Docker found, but user can't connect to daemon
      1  Test run OK
-     """
+    """
     try:
-
         return_status = 1
-        ret = subprocess.run(['docker', 'version'], stdout=subprocess.PIPE,
-                             stderr=subprocess.PIPE)
+        ret = subprocess.run(["docker", "version"], stdout=subprocess.PIPE, stderr=subprocess.PIPE)
     except OSError as e:
         from errno import ENOENT
+
         if e.errno == ENOENT:
             print("Cannot find Docker engine!")
             return_status = 0
         raise e
     if ret.stderr.startswith(b"Cannot connect to the Docker daemon."):
         print("Cannot connect to Docker daemon!")
         return_status = 0
     assert return_status
 
 
 # def test_image(image='pennlinc/bond:latest'):
-#     """Check whether image is present on local system"""
+#     """Check whether image is present on local system."""
 #     ret = subprocess.run(['docker', 'images', '-q', image],
 #                          stdout=subprocess.PIPE)
 
 #     return_status = ret.stdout.decode('UTF-8')
 #     assert return_status
```

