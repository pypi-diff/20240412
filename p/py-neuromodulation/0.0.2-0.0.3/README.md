# Comparing `tmp/py_neuromodulation-0.0.2.tar.gz` & `tmp/py_neuromodulation-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_neuromodulation-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "py_neuromodulation-0.0.3.tar", last modified: Fri Apr 12 13:30:15 2024, max compression
```

## Comparing `py_neuromodulation-0.0.2.tar` & `py_neuromodulation-0.0.3.tar`

### file list

```diff
@@ -1,73 +1,265 @@
--rw-r--r--   0        0        0     1139 2021-03-10 22:04:21.284906 py_neuromodulation-0.0.2/LICENSE
--rw-r--r--   0        0        0     3910 2023-10-25 13:06:48.013160 py_neuromodulation-0.0.2/README.rst
--rw-r--r--   0        0        0    18597 2023-08-17 08:53:22.177106 py_neuromodulation-0.0.2/py_neuromodulation/FieldTrip.py
--rw-r--r--   0        0        0      296 2023-08-17 08:53:22.177106 py_neuromodulation-0.0.2/py_neuromodulation/__init__.py
--rw-r--r--   0        0        0      714 2023-09-08 09:17:00.742417 py_neuromodulation-0.0.2/py_neuromodulation/data/README
--rw-r--r--   0        0        0      130 2023-09-08 09:17:00.742417 py_neuromodulation-0.0.2/py_neuromodulation/data/dataset_description.json
--rw-r--r--   0        0        0    78507 2023-08-31 13:04:09.034721 py_neuromodulation-0.0.2/py_neuromodulation/data/derivatives/sub-testsub_ses-EphysMedOff_task-gripforce_run-0/MOV_aligned_features_ch_ECOG_RIGHT_0_all.png
--rw-r--r--   0        0        0   113368 2023-08-31 13:04:11.015901 py_neuromodulation-0.0.2/py_neuromodulation/data/derivatives/sub-testsub_ses-EphysMedOff_task-gripforce_run-0/all_feature_plt.pdf
--rw-r--r--   0        0        0   229130 2023-08-31 13:04:07.811491 py_neuromodulation-0.0.2/py_neuromodulation/data/derivatives/sub-testsub_ses-EphysMedOff_task-gripforce_run-0/sub-testsub_ses-EphysMedOff_task-gripforce_run-0_FEATURES.csv
--rw-r--r--   0        0        0  1027034 2023-08-31 13:04:12.566728 py_neuromodulation-0.0.2/py_neuromodulation/data/derivatives/sub-testsub_ses-EphysMedOff_task-gripforce_run-0/sub-testsub_ses-EphysMedOff_task-gripforce_run-0_LM_ML_RES.p
--rw-r--r--   0        0        0     6694 2023-08-31 13:04:07.811491 py_neuromodulation-0.0.2/py_neuromodulation/data/derivatives/sub-testsub_ses-EphysMedOff_task-gripforce_run-0/sub-testsub_ses-EphysMedOff_task-gripforce_run-0_SETTINGS.json
--rw-r--r--   0        0        0       97 2023-08-31 13:04:07.760182 py_neuromodulation-0.0.2/py_neuromodulation/data/derivatives/sub-testsub_ses-EphysMedOff_task-gripforce_run-0/sub-testsub_ses-EphysMedOff_task-gripforce_run-0_SIDECAR.json
--rw-r--r--   0        0        0    93276 2023-08-31 13:04:13.405740 py_neuromodulation-0.0.2/py_neuromodulation/data/derivatives/sub-testsub_ses-EphysMedOff_task-gripforce_run-0/sub-testsub_ses-EphysMedOff_task-gripforce_run-0_decoding_performance.png
--rw-r--r--   0        0        0      634 2023-08-31 13:04:07.811491 py_neuromodulation-0.0.2/py_neuromodulation/data/derivatives/sub-testsub_ses-EphysMedOff_task-gripforce_run-0/sub-testsub_ses-EphysMedOff_task-gripforce_run-0_nm_channels.csv
--rw-r--r--   0        0        0      788 2023-09-08 09:17:00.742417 py_neuromodulation-0.0.2/py_neuromodulation/data/participants.json
--rw-r--r--   0        0        0       79 2023-09-08 09:17:00.742417 py_neuromodulation-0.0.2/py_neuromodulation/data/participants.tsv
--rw-r--r--   0        0        0      123 2023-09-08 09:17:00.742417 py_neuromodulation-0.0.2/py_neuromodulation/data/sub-testsub/ses-EphysMedOff/ieeg/sub-testsub_ses-EphysMedOff_space-mni_coordsystem.json
--rw-r--r--   0        0        0      733 2023-09-08 09:17:00.750562 py_neuromodulation-0.0.2/py_neuromodulation/data/sub-testsub/ses-EphysMedOff/ieeg/sub-testsub_ses-EphysMedOff_space-mni_electrodes.tsv
--rw-r--r--   0        0        0      790 2023-09-08 09:17:00.750562 py_neuromodulation-0.0.2/py_neuromodulation/data/sub-testsub/ses-EphysMedOff/ieeg/sub-testsub_ses-EphysMedOff_task-gripforce_run-0_channels.tsv
--rw-r--r--   0        0        0   760040 2023-09-08 09:17:00.762404 py_neuromodulation-0.0.2/py_neuromodulation/data/sub-testsub/ses-EphysMedOff/ieeg/sub-testsub_ses-EphysMedOff_task-gripforce_run-0_ieeg.eeg
--rw-r--r--   0        0        0      492 2023-09-08 09:17:00.765920 py_neuromodulation-0.0.2/py_neuromodulation/data/sub-testsub/ses-EphysMedOff/ieeg/sub-testsub_ses-EphysMedOff_task-gripforce_run-0_ieeg.json
--rw-r--r--   0        0        0     1023 2023-09-08 09:17:00.765920 py_neuromodulation-0.0.2/py_neuromodulation/data/sub-testsub/ses-EphysMedOff/ieeg/sub-testsub_ses-EphysMedOff_task-gripforce_run-0_ieeg.vhdr
--rw-r--r--   0        0        0      553 2023-09-08 09:17:00.769928 py_neuromodulation-0.0.2/py_neuromodulation/data/sub-testsub/ses-EphysMedOff/ieeg/sub-testsub_ses-EphysMedOff_task-gripforce_run-0_ieeg.vmrk
--rw-r--r--   0        0        0       91 2023-09-08 09:17:00.770947 py_neuromodulation-0.0.2/py_neuromodulation/data/sub-testsub/ses-EphysMedOff/sub-testsub_ses-EphysMedOff_scans.tsv
--rw-r--r--   0        0        0      683 2023-08-17 08:53:22.371225 py_neuromodulation-0.0.2/py_neuromodulation/grid_cortex.tsv
--rw-r--r--   0        0        0    25842 2023-08-17 08:53:22.373224 py_neuromodulation-0.0.2/py_neuromodulation/grid_subcortex.tsv
--rw-r--r--   0        0        0     2510 2023-09-08 09:17:00.770947 py_neuromodulation-0.0.2/py_neuromodulation/helper.py
--rw-r--r--   0        0        0     2603 2023-08-17 08:53:22.374729 py_neuromodulation-0.0.2/py_neuromodulation/nm_EpochStream.py
--rw-r--r--   0        0        0    12713 2023-09-08 09:17:00.770947 py_neuromodulation-0.0.2/py_neuromodulation/nm_IO.py
--rw-r--r--   0        0        0     7594 2023-09-08 09:17:00.770947 py_neuromodulation-0.0.2/py_neuromodulation/nm_RMAP.py
--rw-r--r--   0        0        0    38690 2023-08-17 08:53:22.381245 py_neuromodulation-0.0.2/py_neuromodulation/nm_across_patient_decoding.py
--rw-r--r--   0        0        0    38509 2023-09-08 09:17:00.770947 py_neuromodulation-0.0.2/py_neuromodulation/nm_analysis.py
--rw-r--r--   0        0        0     5617 2023-10-09 13:32:57.938531 py_neuromodulation-0.0.2/py_neuromodulation/nm_bispectra.py
--rw-r--r--   0        0        0     7295 2023-10-25 13:00:56.113847 py_neuromodulation-0.0.2/py_neuromodulation/nm_bursts.py
--rw-r--r--   0        0        0     7420 2023-08-21 07:44:23.696175 py_neuromodulation-0.0.2/py_neuromodulation/nm_coherence.py
--rw-r--r--   0        0        0    16643 2023-09-08 09:17:00.770947 py_neuromodulation-0.0.2/py_neuromodulation/nm_cohortwrapper.py
--rw-r--r--   0        0        0    35645 2023-09-08 09:17:00.780680 py_neuromodulation-0.0.2/py_neuromodulation/nm_decode.py
--rw-r--r--   0        0        0    11074 2023-11-14 10:20:09.825341 py_neuromodulation-0.0.2/py_neuromodulation/nm_define_nmchannels.py
--rw-r--r--   0        0        0     8800 2023-08-17 08:53:22.392167 py_neuromodulation-0.0.2/py_neuromodulation/nm_eval_timing.py
--rw-r--r--   0        0        0     3436 2023-10-09 13:32:57.938531 py_neuromodulation-0.0.2/py_neuromodulation/nm_features.py
--rw-r--r--   0        0        0      917 2023-08-17 08:53:22.394675 py_neuromodulation-0.0.2/py_neuromodulation/nm_features_abc.py
--rw-r--r--   0        0        0     6437 2023-09-11 13:40:21.641813 py_neuromodulation-0.0.2/py_neuromodulation/nm_filter.py
--rw-r--r--   0        0        0     5607 2023-09-08 09:17:00.781957 py_neuromodulation-0.0.2/py_neuromodulation/nm_fooof.py
--rw-r--r--   0        0        0     1088 2023-10-09 13:32:57.938531 py_neuromodulation-0.0.2/py_neuromodulation/nm_generator.py
--rw-r--r--   0        0        0     2180 2023-08-21 07:44:23.707523 py_neuromodulation-0.0.2/py_neuromodulation/nm_hjorth_raw.py
--rw-r--r--   0        0        0     2006 2023-08-17 08:53:22.401017 py_neuromodulation-0.0.2/py_neuromodulation/nm_kalmanfilter.py
--rw-r--r--   0        0        0      954 2023-08-17 08:53:22.403019 py_neuromodulation-0.0.2/py_neuromodulation/nm_linelength.py
--rw-r--r--   0        0        0     3895 2023-09-08 09:17:00.790990 py_neuromodulation-0.0.2/py_neuromodulation/nm_mne_connectivity.py
--rw-r--r--   0        0        0     3660 2023-08-21 07:44:23.710527 py_neuromodulation-0.0.2/py_neuromodulation/nm_nolds.py
--rw-r--r--   0        0        0     8019 2023-08-17 08:53:22.407547 py_neuromodulation-0.0.2/py_neuromodulation/nm_normalization.py
--rw-r--r--   0        0        0    12450 2023-08-21 07:44:23.711526 py_neuromodulation-0.0.2/py_neuromodulation/nm_oscillatory.py
--rw-r--r--   0        0        0    17688 2023-10-09 10:21:50.076345 py_neuromodulation-0.0.2/py_neuromodulation/nm_plots.py
--rw-r--r--   0        0        0    15309 2023-09-08 09:17:00.790990 py_neuromodulation-0.0.2/py_neuromodulation/nm_projection.py
--rw-r--r--   0        0        0     3167 2023-09-08 09:17:00.790990 py_neuromodulation-0.0.2/py_neuromodulation/nm_rereference.py
--rw-r--r--   0        0        0     1122 2023-09-08 09:18:00.412231 py_neuromodulation-0.0.2/py_neuromodulation/nm_resample.py
--rw-r--r--   0        0        0    14607 2023-10-25 13:00:49.575158 py_neuromodulation-0.0.2/py_neuromodulation/nm_run_analysis.py
--rw-r--r--   0        0        0     6981 2023-10-09 13:32:57.938531 py_neuromodulation-0.0.2/py_neuromodulation/nm_settings.json
--rw-r--r--   0        0        0     1775 2023-08-21 07:44:23.716986 py_neuromodulation-0.0.2/py_neuromodulation/nm_settings.py
--rw-r--r--   0        0        0    17493 2023-09-08 09:17:00.800773 py_neuromodulation-0.0.2/py_neuromodulation/nm_sharpwaves.py
--rw-r--r--   0        0        0    15876 2023-09-08 09:17:00.802009 py_neuromodulation-0.0.2/py_neuromodulation/nm_stats.py
--rw-r--r--   0        0        0     7576 2023-09-08 09:33:49.159879 py_neuromodulation-0.0.2/py_neuromodulation/nm_stream_abc.py
--rw-r--r--   0        0        0     7835 2023-10-25 13:00:49.579159 py_neuromodulation-0.0.2/py_neuromodulation/nm_stream_offline.py
--rw-r--r--   0        0        0   124526 2023-08-17 08:53:22.428688 py_neuromodulation-0.0.2/py_neuromodulation/plots/STN_surf.mat
--rw-r--r--   0        0        0  3709780 2023-08-17 08:53:22.478138 py_neuromodulation-0.0.2/py_neuromodulation/plots/Vertices.mat
--rw-r--r--   0        0        0  2859245 2023-08-17 08:53:22.514629 py_neuromodulation-0.0.2/py_neuromodulation/plots/faces.mat
--rw-r--r--   0        0        0      775 2023-08-17 08:53:22.515633 py_neuromodulation-0.0.2/py_neuromodulation/plots/grid.mat
--rw-r--r--   0        0        0     4651 2023-08-09 10:08:10.326733 py_neuromodulation-0.0.2/py_neuromodulation/py_neuromodulation.egg-info/PKG-INFO
--rw-r--r--   0        0        0        0 2023-08-09 10:08:10.331738 py_neuromodulation-0.0.2/py_neuromodulation/py_neuromodulation.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2023-08-09 10:08:10.328465 py_neuromodulation-0.0.2/py_neuromodulation/py_neuromodulation.egg-info/dependency_links.txt
--rw-r--r--   0        0        0      281 2023-08-09 10:08:10.329738 py_neuromodulation-0.0.2/py_neuromodulation/py_neuromodulation.egg-info/requires.txt
--rw-r--r--   0        0        0       19 2023-08-09 10:08:10.330737 py_neuromodulation-0.0.2/py_neuromodulation/py_neuromodulation.egg-info/top_level.txt
--rw-r--r--   0        0        0     1663 2023-11-14 15:25:55.114793 py_neuromodulation-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     5311 1970-01-01 00:00:00.000000 py_neuromodulation-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:15.018954 py_neuromodulation-0.0.3/
+-rw-rw-rw-   0        0        0     1139 2024-03-11 17:49:34.000000 py_neuromodulation-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     7213 2024-04-12 13:30:15.018954 py_neuromodulation-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4176 2024-04-11 13:31:40.000000 py_neuromodulation-0.0.3/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.523411 py_neuromodulation-0.0.3/docs/
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.514243 py_neuromodulation-0.0.3/docs/build/
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.514243 py_neuromodulation-0.0.3/docs/build/_downloads/
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.564671 py_neuromodulation-0.0.3/docs/build/_downloads/09df217f95985497f45d69e2d4bdc5b1/
+-rw-rw-rw-   0        0        0     2332 2023-08-31 07:56:55.000000 py_neuromodulation-0.0.3/docs/build/_downloads/09df217f95985497f45d69e2d4bdc5b1/plot_2_example_add_feature.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.568660 py_neuromodulation-0.0.3/docs/build/_downloads/3b4900a2b2818ff30362215b76f7d5eb/
+-rw-rw-rw-   0        0        0     6908 2023-08-31 13:04:03.000000 py_neuromodulation-0.0.3/docs/build/_downloads/3b4900a2b2818ff30362215b76f7d5eb/plot_1_example_BIDS.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.569665 py_neuromodulation-0.0.3/docs/build/_downloads/7e92dd2e6cc86b239d14cafad972ae4f/
+-rw-rw-rw-   0        0        0     9620 2023-08-31 13:04:14.000000 py_neuromodulation-0.0.3/docs/build/_downloads/7e92dd2e6cc86b239d14cafad972ae4f/plot_3_example_sharpwave_analysis.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.571665 py_neuromodulation-0.0.3/docs/build/_downloads/c2db0bf2b334d541b00662b991682256/
+-rw-rw-rw-   0        0        0     4847 2023-08-31 07:56:55.000000 py_neuromodulation-0.0.3/docs/build/_downloads/c2db0bf2b334d541b00662b991682256/plot_6_real_time_demo.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.573665 py_neuromodulation-0.0.3/docs/build/_downloads/ce3914826f782cbd1ea8fd024eaf0ac3/
+-rw-rw-rw-   0        0        0     2844 2023-08-31 13:38:09.000000 py_neuromodulation-0.0.3/docs/build/_downloads/ce3914826f782cbd1ea8fd024eaf0ac3/plot_5_example_rmap_computing.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.574664 py_neuromodulation-0.0.3/docs/build/_downloads/da36848a41e6a3235d91fb7cfb6d59b4/
+-rw-rw-rw-   0        0        0     7687 2023-08-31 07:56:57.000000 py_neuromodulation-0.0.3/docs/build/_downloads/da36848a41e6a3235d91fb7cfb6d59b4/plot_0_first_demo.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.576664 py_neuromodulation-0.0.3/docs/build/_downloads/eaa4305c75b19a1e2eea941f742a6331/
+-rw-rw-rw-   0        0        0     8105 2023-08-31 07:57:19.000000 py_neuromodulation-0.0.3/docs/build/_downloads/eaa4305c75b19a1e2eea941f742a6331/plot_4_example_gridPointProjection.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.514243 py_neuromodulation-0.0.3/docs/build/html/
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.522411 py_neuromodulation-0.0.3/docs/build/html/_downloads/
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.577666 py_neuromodulation-0.0.3/docs/build/html/_downloads/09df217f95985497f45d69e2d4bdc5b1/
+-rw-rw-rw-   0        0        0     2332 2023-08-31 07:56:55.000000 py_neuromodulation-0.0.3/docs/build/html/_downloads/09df217f95985497f45d69e2d4bdc5b1/plot_2_example_add_feature.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.579665 py_neuromodulation-0.0.3/docs/build/html/_downloads/3b4900a2b2818ff30362215b76f7d5eb/
+-rw-rw-rw-   0        0        0     6937 2023-11-14 15:20:55.000000 py_neuromodulation-0.0.3/docs/build/html/_downloads/3b4900a2b2818ff30362215b76f7d5eb/plot_1_example_BIDS.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.582172 py_neuromodulation-0.0.3/docs/build/html/_downloads/7e92dd2e6cc86b239d14cafad972ae4f/
+-rw-rw-rw-   0        0        0     9620 2023-08-31 13:04:14.000000 py_neuromodulation-0.0.3/docs/build/html/_downloads/7e92dd2e6cc86b239d14cafad972ae4f/plot_3_example_sharpwave_analysis.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.585273 py_neuromodulation-0.0.3/docs/build/html/_downloads/c2db0bf2b334d541b00662b991682256/
+-rw-rw-rw-   0        0        0     4847 2023-08-31 07:56:55.000000 py_neuromodulation-0.0.3/docs/build/html/_downloads/c2db0bf2b334d541b00662b991682256/plot_6_real_time_demo.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.585273 py_neuromodulation-0.0.3/docs/build/html/_downloads/ce3914826f782cbd1ea8fd024eaf0ac3/
+-rw-rw-rw-   0        0        0     2844 2023-08-31 13:38:09.000000 py_neuromodulation-0.0.3/docs/build/html/_downloads/ce3914826f782cbd1ea8fd024eaf0ac3/plot_5_example_rmap_computing.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.585273 py_neuromodulation-0.0.3/docs/build/html/_downloads/da36848a41e6a3235d91fb7cfb6d59b4/
+-rw-rw-rw-   0        0        0     7687 2023-08-31 07:56:57.000000 py_neuromodulation-0.0.3/docs/build/html/_downloads/da36848a41e6a3235d91fb7cfb6d59b4/plot_0_first_demo.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.585273 py_neuromodulation-0.0.3/docs/build/html/_downloads/eaa4305c75b19a1e2eea941f742a6331/
+-rw-rw-rw-   0        0        0     8105 2023-08-31 07:57:19.000000 py_neuromodulation-0.0.3/docs/build/html/_downloads/eaa4305c75b19a1e2eea941f742a6331/plot_4_example_gridPointProjection.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.585273 py_neuromodulation-0.0.3/docs/source/
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.524410 py_neuromodulation-0.0.3/docs/source/_build/
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.525413 py_neuromodulation-0.0.3/docs/source/_build/html/
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.537396 py_neuromodulation-0.0.3/docs/source/_build/html/_downloads/
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.585273 py_neuromodulation-0.0.3/docs/source/_build/html/_downloads/09df217f95985497f45d69e2d4bdc5b1/
+-rw-rw-rw-   0        0        0     2353 2023-12-15 13:49:14.000000 py_neuromodulation-0.0.3/docs/source/_build/html/_downloads/09df217f95985497f45d69e2d4bdc5b1/plot_2_example_add_feature.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.585273 py_neuromodulation-0.0.3/docs/source/_build/html/_downloads/0d0d0a76e8f648d5d3cbc47da6351932/
+-rw-rw-rw-   0        0        0     4847 2023-08-29 14:12:24.000000 py_neuromodulation-0.0.3/docs/source/_build/html/_downloads/0d0d0a76e8f648d5d3cbc47da6351932/plot_real_time_demo.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.602994 py_neuromodulation-0.0.3/docs/source/_build/html/_downloads/3b4900a2b2818ff30362215b76f7d5eb/
+-rw-rw-rw-   0        0        0     6967 2024-02-15 10:13:17.000000 py_neuromodulation-0.0.3/docs/source/_build/html/_downloads/3b4900a2b2818ff30362215b76f7d5eb/plot_1_example_BIDS.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.602994 py_neuromodulation-0.0.3/docs/source/_build/html/_downloads/5d73cadc59a8805c47e3b84063afc157/
+-rw-rw-rw-   0        0        0     6901 2023-08-29 14:12:53.000000 py_neuromodulation-0.0.3/docs/source/_build/html/_downloads/5d73cadc59a8805c47e3b84063afc157/plot_example_BIDS.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.602994 py_neuromodulation-0.0.3/docs/source/_build/html/_downloads/7660317fa5a6bfbd12fcca9961457fc4/
+-rw-rw-rw-   0        0        0     2859 2023-08-30 11:58:03.000000 py_neuromodulation-0.0.3/docs/source/_build/html/_downloads/7660317fa5a6bfbd12fcca9961457fc4/plot_example_rmap_computing.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.602994 py_neuromodulation-0.0.3/docs/source/_build/html/_downloads/7e92dd2e6cc86b239d14cafad972ae4f/
+-rw-rw-rw-   0        0        0     9620 2023-08-31 13:04:14.000000 py_neuromodulation-0.0.3/docs/source/_build/html/_downloads/7e92dd2e6cc86b239d14cafad972ae4f/plot_3_example_sharpwave_analysis.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.602994 py_neuromodulation-0.0.3/docs/source/_build/html/_downloads/839e5b319379f7fd9e867deb00fd797f/
+-rw-rw-rw-   0        0        0     8105 2023-08-29 14:12:45.000000 py_neuromodulation-0.0.3/docs/source/_build/html/_downloads/839e5b319379f7fd9e867deb00fd797f/plot_example_gridPointProjection.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.602994 py_neuromodulation-0.0.3/docs/source/_build/html/_downloads/ae8be19afe5e559f011fc9b138968ba0/
+-rw-rw-rw-   0        0        0     7687 2023-08-30 13:29:34.000000 py_neuromodulation-0.0.3/docs/source/_build/html/_downloads/ae8be19afe5e559f011fc9b138968ba0/plot_first_demo.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.619357 py_neuromodulation-0.0.3/docs/source/_build/html/_downloads/b8b06cacc17969d3725a0b6f1d7741c5/
+-rw-rw-rw-   0        0        0     9640 2023-08-29 14:13:01.000000 py_neuromodulation-0.0.3/docs/source/_build/html/_downloads/b8b06cacc17969d3725a0b6f1d7741c5/plot_example_sharpwave_analysis.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.621100 py_neuromodulation-0.0.3/docs/source/_build/html/_downloads/c2db0bf2b334d541b00662b991682256/
+-rw-rw-rw-   0        0        0     4938 2023-12-15 13:49:15.000000 py_neuromodulation-0.0.3/docs/source/_build/html/_downloads/c2db0bf2b334d541b00662b991682256/plot_6_real_time_demo.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.621100 py_neuromodulation-0.0.3/docs/source/_build/html/_downloads/c31a86c0b68cb4167d968091ace8080d/
+-rw-rw-rw-   0        0        0     2332 2023-08-29 14:12:24.000000 py_neuromodulation-0.0.3/docs/source/_build/html/_downloads/c31a86c0b68cb4167d968091ace8080d/plot_example_add_feature.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.621100 py_neuromodulation-0.0.3/docs/source/_build/html/_downloads/ce3914826f782cbd1ea8fd024eaf0ac3/
+-rw-rw-rw-   0        0        0     2844 2023-08-31 13:38:09.000000 py_neuromodulation-0.0.3/docs/source/_build/html/_downloads/ce3914826f782cbd1ea8fd024eaf0ac3/plot_5_example_rmap_computing.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.621100 py_neuromodulation-0.0.3/docs/source/_build/html/_downloads/da36848a41e6a3235d91fb7cfb6d59b4/
+-rw-rw-rw-   0        0        0     7650 2023-12-15 13:44:41.000000 py_neuromodulation-0.0.3/docs/source/_build/html/_downloads/da36848a41e6a3235d91fb7cfb6d59b4/plot_0_first_demo.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.635469 py_neuromodulation-0.0.3/docs/source/_build/html/_downloads/eaa4305c75b19a1e2eea941f742a6331/
+-rw-rw-rw-   0        0        0     8105 2023-08-30 13:46:30.000000 py_neuromodulation-0.0.3/docs/source/_build/html/_downloads/eaa4305c75b19a1e2eea941f742a6331/plot_4_example_gridPointProjection.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.648056 py_neuromodulation-0.0.3/docs/source/auto_examples/
+-rw-rw-rw-   0        0        0     7650 2023-12-15 13:44:41.000000 py_neuromodulation-0.0.3/docs/source/auto_examples/plot_0_first_demo.py
+-rw-rw-rw-   0        0        0     6967 2024-02-15 10:13:17.000000 py_neuromodulation-0.0.3/docs/source/auto_examples/plot_1_example_BIDS.py
+-rw-rw-rw-   0        0        0     2353 2023-12-15 13:49:14.000000 py_neuromodulation-0.0.3/docs/source/auto_examples/plot_2_example_add_feature.py
+-rw-rw-rw-   0        0        0     9620 2023-08-31 13:04:14.000000 py_neuromodulation-0.0.3/docs/source/auto_examples/plot_3_example_sharpwave_analysis.py
+-rw-rw-rw-   0        0        0     8105 2023-08-31 07:57:19.000000 py_neuromodulation-0.0.3/docs/source/auto_examples/plot_4_example_gridPointProjection.py
+-rw-rw-rw-   0        0        0     2844 2023-08-31 13:38:09.000000 py_neuromodulation-0.0.3/docs/source/auto_examples/plot_5_example_rmap_computing.py
+-rw-rw-rw-   0        0        0     4938 2023-12-15 13:49:15.000000 py_neuromodulation-0.0.3/docs/source/auto_examples/plot_6_real_time_demo.py
+-rw-rw-rw-   0        0        0     3109 2024-03-25 16:32:23.000000 py_neuromodulation-0.0.3/docs/source/conf.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.664826 py_neuromodulation-0.0.3/examples/
+-rw-rw-rw-   0        0        0     7650 2024-03-25 16:32:23.000000 py_neuromodulation-0.0.3/examples/plot_0_first_demo.py
+-rw-rw-rw-   0        0        0     6967 2024-03-25 16:32:23.000000 py_neuromodulation-0.0.3/examples/plot_1_example_BIDS.py
+-rw-rw-rw-   0        0        0     2353 2024-03-25 16:32:23.000000 py_neuromodulation-0.0.3/examples/plot_2_example_add_feature.py
+-rw-rw-rw-   0        0        0     9620 2024-03-25 16:32:23.000000 py_neuromodulation-0.0.3/examples/plot_3_example_sharpwave_analysis.py
+-rw-rw-rw-   0        0        0     8105 2024-03-25 16:32:23.000000 py_neuromodulation-0.0.3/examples/plot_4_example_gridPointProjection.py
+-rw-rw-rw-   0        0        0     2844 2024-03-25 16:32:23.000000 py_neuromodulation-0.0.3/examples/plot_5_example_rmap_computing.py
+-rw-rw-rw-   0        0        0     4938 2024-03-25 16:32:23.000000 py_neuromodulation-0.0.3/examples/plot_6_real_time_demo.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.543397 py_neuromodulation-0.0.3/packages/
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.541396 py_neuromodulation-0.0.3/packages/realtime_decoding/
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.541396 py_neuromodulation-0.0.3/packages/realtime_decoding/build/
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.542398 py_neuromodulation-0.0.3/packages/realtime_decoding/build/lib/
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.680986 py_neuromodulation-0.0.3/packages/realtime_decoding/build/lib/realtime_decoding/
+-rw-rw-rw-   0        0        0      127 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/realtime_decoding/build/lib/realtime_decoding/__init__.py
+-rw-rw-rw-   0        0        0     3229 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/realtime_decoding/build/lib/realtime_decoding/decoder.py
+-rw-rw-rw-   0        0        0     6021 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/realtime_decoding/build/lib/realtime_decoding/features.py
+-rw-rw-rw-   0        0        0      337 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/realtime_decoding/build/lib/realtime_decoding/helpers.py
+-rw-rw-rw-   0        0        0    11950 2023-03-20 09:53:22.000000 py_neuromodulation-0.0.3/packages/realtime_decoding/build/lib/realtime_decoding/run_decoding.py
+-rw-rw-rw-   0        0        0     1536 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/realtime_decoding/build/lib/realtime_decoding/trainer.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.544124 py_neuromodulation-0.0.3/packages/tmsi/
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.544882 py_neuromodulation-0.0.3/packages/tmsi/build/
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.680986 py_neuromodulation-0.0.3/packages/tmsi/build/lib/
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.680986 py_neuromodulation-0.0.3/packages/tmsi/build/lib/TMSiFileFormats/
+-rw-rw-rw-   0        0        0     1076 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/TMSiFileFormats/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.705744 py_neuromodulation-0.0.3/packages/tmsi/build/lib/TMSiFileFormats/file_formats/
+-rw-rw-rw-   0        0        0     1136 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/TMSiFileFormats/file_formats/__init__.py
+-rw-rw-rw-   0        0        0     6987 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/TMSiFileFormats/file_formats/lsl_stream_writer.py
+-rw-rw-rw-   0        0        0    17298 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/TMSiFileFormats/file_formats/poly5_file_writer.py
+-rw-rw-rw-   0        0        0     9221 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/TMSiFileFormats/file_formats/poly5_to_edf_converter.py
+-rw-rw-rw-   0        0        0    39017 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/TMSiFileFormats/file_formats/xdf_file_writer.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.711103 py_neuromodulation-0.0.3/packages/tmsi/build/lib/TMSiFileFormats/file_readers/
+-rw-rw-rw-   0        0        0     1060 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/TMSiFileFormats/file_readers/__init__.py
+-rw-rw-rw-   0        0        0     4090 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/TMSiFileFormats/file_readers/edf_reader.py
+-rw-rw-rw-   0        0        0    10297 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/TMSiFileFormats/file_readers/poly5reader.py
+-rw-rw-rw-   0        0        0     8579 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/TMSiFileFormats/file_readers/xdf_reader.py
+-rw-rw-rw-   0        0        0     3482 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/TMSiFileFormats/file_writer.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.713143 py_neuromodulation-0.0.3/packages/tmsi/build/lib/TMSiPlotters/
+-rw-rw-rw-   0        0        0       43 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/TMSiPlotters/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.716144 py_neuromodulation-0.0.3/packages/tmsi/build/lib/TMSiPlotters/gui/
+-rw-rw-rw-   0        0        0     1219 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/TMSiPlotters/gui/__init__.py
+-rw-rw-rw-   0        0        0    10981 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/TMSiPlotters/gui/_plotter_gui.py
+-rw-rw-rw-   0        0        0    21679 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/TMSiPlotters/gui/plotting_gui.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.722829 py_neuromodulation-0.0.3/packages/tmsi/build/lib/TMSiPlotters/plotters/
+-rw-rw-rw-   0        0        0     1318 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/TMSiPlotters/plotters/__init__.py
+-rw-rw-rw-   0        0        0    20868 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/TMSiPlotters/plotters/hd_emg_plotter.py
+-rw-rw-rw-   0        0        0    28170 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/TMSiPlotters/plotters/impedance_plotter.py
+-rw-rw-rw-   0        0        0    56052 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/TMSiPlotters/plotters/signal_plotter.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.728041 py_neuromodulation-0.0.3/packages/tmsi/build/lib/TMSiSDK/
+-rw-rw-rw-   0        0        0     1637 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/TMSiSDK/__init__.py
+-rw-rw-rw-   0        0        0    18540 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/TMSiSDK/device.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.728041 py_neuromodulation-0.0.3/packages/tmsi/build/lib/TMSiSDK/devices/
+-rw-rw-rw-   0        0        0      987 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/TMSiSDK/devices/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.748687 py_neuromodulation-0.0.3/packages/tmsi/build/lib/TMSiSDK/devices/saga/
+-rw-rw-rw-   0        0        0    64350 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/TMSiSDK/devices/saga/TMSi_Device_API.py
+-rw-rw-rw-   0        0        0     1104 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/TMSiSDK/devices/saga/__init__.py
+-rw-rw-rw-   0        0        0    56014 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/TMSiSDK/devices/saga/saga_device.py
+-rw-rw-rw-   0        0        0    19323 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/TMSiSDK/devices/saga/saga_types.py
+-rw-rw-rw-   0        0        0     5811 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/TMSiSDK/devices/saga/xml_saga_config.py
+-rw-rw-rw-   0        0        0     3969 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/TMSiSDK/error.py
+-rw-rw-rw-   0        0        0     2078 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/TMSiSDK/sample_data.py
+-rw-rw-rw-   0        0        0     3179 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/TMSiSDK/sample_data_server.py
+-rw-rw-rw-   0        0        0     1303 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/TMSiSDK/settings.py
+-rw-rw-rw-   0        0        0     3872 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/TMSiSDK/tmsi_device.py
+-rw-rw-rw-   0        0        0      145 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.752215 py_neuromodulation-0.0.3/packages/tmsi/build/lib/apex_sdk/
+-rw-rw-rw-   0        0        0     1029 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/apex_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.768930 py_neuromodulation-0.0.3/packages/tmsi/build/lib/apex_sdk/device/
+-rw-rw-rw-   0        0        0     1317 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/apex_sdk/device/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.552063 py_neuromodulation-0.0.3/packages/tmsi/build/lib/apex_sdk/device/devices/
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.785584 py_neuromodulation-0.0.3/packages/tmsi/build/lib/apex_sdk/device/devices/apex/
+-rw-rw-rw-   0        0        0    39789 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/apex_sdk/device/devices/apex/apex_API.py
+-rw-rw-rw-   0        0        0     6480 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/apex_sdk/device/devices/apex/apex_API_enums.py
+-rw-rw-rw-   0        0        0    19330 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/apex_sdk/device/devices/apex/apex_API_structures.py
+-rw-rw-rw-   0        0        0    66903 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/apex_sdk/device/devices/apex/apex_device.py
+-rw-rw-rw-   0        0        0     1094 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/apex_sdk/device/devices/apex/apex_dongle.py
+-rw-rw-rw-   0        0        0     1847 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/apex_sdk/device/devices/apex/apex_event_reader.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.799534 py_neuromodulation-0.0.3/packages/tmsi/build/lib/apex_sdk/device/devices/apex/apex_structures/
+-rw-rw-rw-   0        0        0     1479 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/apex_sdk/device/devices/apex/apex_structures/apex_channel.py
+-rw-rw-rw-   0        0        0     5607 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/apex_sdk/device/devices/apex/apex_structures/apex_config.py
+-rw-rw-rw-   0        0        0     1000 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/apex_sdk/device/devices/apex/apex_structures/apex_const.py
+-rw-rw-rw-   0        0        0     1616 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/apex_sdk/device/devices/apex/apex_structures/apex_impedance_channel.py
+-rw-rw-rw-   0        0        0     3280 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/apex_sdk/device/devices/apex/apex_structures/apex_info.py
+-rw-rw-rw-   0        0        0     1123 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/apex_sdk/device/devices/apex/apex_structures/dongle_info.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.802111 py_neuromodulation-0.0.3/packages/tmsi/build/lib/apex_sdk/device/devices/apex/measurements/
+-rw-rw-rw-   0        0        0     2628 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/apex_sdk/device/devices/apex/measurements/download_measurement.py
+-rw-rw-rw-   0        0        0     6110 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/apex_sdk/device/devices/apex/measurements/eeg_measurement.py
+-rw-rw-rw-   0        0        0     5040 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/apex_sdk/device/devices/apex/measurements/impedance_measurement.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.802111 py_neuromodulation-0.0.3/packages/tmsi/build/lib/apex_sdk/device/threads/
+-rw-rw-rw-   0        0        0     1604 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/apex_sdk/device/threads/conversion_thread.py
+-rw-rw-rw-   0        0        0     1565 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/apex_sdk/device/threads/sampling_thread.py
+-rw-rw-rw-   0        0        0     2349 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/apex_sdk/device/tmsi_channel.py
+-rw-rw-rw-   0        0        0     7904 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/apex_sdk/device/tmsi_device.py
+-rw-rw-rw-   0        0        0     2182 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/apex_sdk/device/tmsi_device_enums.py
+-rw-rw-rw-   0        0        0     1207 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/apex_sdk/device/tmsi_dongle.py
+-rw-rw-rw-   0        0        0     1475 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/apex_sdk/device/tmsi_event_reader.py
+-rw-rw-rw-   0        0        0     3996 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/apex_sdk/device/tmsi_measurement.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.817759 py_neuromodulation-0.0.3/packages/tmsi/build/lib/apex_sdk/sample_data_server/
+-rw-rw-rw-   0        0        0      986 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/apex_sdk/sample_data_server/__init__.py
+-rw-rw-rw-   0        0        0     1180 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/apex_sdk/sample_data_server/event_data.py
+-rw-rw-rw-   0        0        0     1416 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/apex_sdk/sample_data_server/sample_data.py
+-rw-rw-rw-   0        0        0     4816 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/apex_sdk/sample_data_server/sample_data_server.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.817759 py_neuromodulation-0.0.3/packages/tmsi/build/lib/apex_sdk/tmsi_errors/
+-rw-rw-rw-   0        0        0     5047 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/apex_sdk/tmsi_errors/error.py
+-rw-rw-rw-   0        0        0     4208 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/apex_sdk/tmsi_sdk.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.838563 py_neuromodulation-0.0.3/packages/tmsi/build/lib/apex_sdk/tmsi_utilities/
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.838563 py_neuromodulation-0.0.3/packages/tmsi/build/lib/apex_sdk/tmsi_utilities/apex/
+-rw-rw-rw-   0        0        0     5414 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/apex_sdk/tmsi_utilities/apex/apex_structure_generator.py
+-rw-rw-rw-   0        0        0     1782 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/apex_sdk/tmsi_utilities/decorators.py
+-rw-rw-rw-   0        0        0     1150 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/apex_sdk/tmsi_utilities/logger_filter.py
+-rw-rw-rw-   0        0        0     1196 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/apex_sdk/tmsi_utilities/singleton.py
+-rw-rw-rw-   0        0        0     1949 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/apex_sdk/tmsi_utilities/support_functions.py
+-rw-rw-rw-   0        0        0     3459 2023-03-17 14:50:18.000000 py_neuromodulation-0.0.3/packages/tmsi/build/lib/apex_sdk/tmsi_utilities/tmsi_logger.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.935447 py_neuromodulation-0.0.3/py_neuromodulation/
+-rw-rw-rw-   0        0        0    18597 2024-03-11 17:49:34.000000 py_neuromodulation-0.0.3/py_neuromodulation/FieldTrip.py
+-rw-rw-rw-   0        0        0      296 2024-03-11 17:49:34.000000 py_neuromodulation-0.0.3/py_neuromodulation/__init__.py
+-rw-rw-rw-   0        0        0     2530 2024-03-25 16:32:23.000000 py_neuromodulation-0.0.3/py_neuromodulation/_write_example_dataset_helper.py
+-rw-rw-rw-   0        0        0     2595 2024-03-25 16:32:23.000000 py_neuromodulation-0.0.3/py_neuromodulation/nm_EpochStream.py
+-rw-rw-rw-   0        0        0    11688 2024-03-25 16:32:23.000000 py_neuromodulation-0.0.3/py_neuromodulation/nm_IO.py
+-rw-rw-rw-   0        0        0    15791 2024-04-11 13:31:40.000000 py_neuromodulation-0.0.3/py_neuromodulation/nm_RMAP.py
+-rw-rw-rw-   0        0        0    38690 2024-03-11 17:49:34.000000 py_neuromodulation-0.0.3/py_neuromodulation/nm_across_patient_decoding.py
+-rw-rw-rw-   0        0        0    38528 2024-03-25 16:32:23.000000 py_neuromodulation-0.0.3/py_neuromodulation/nm_analysis.py
+-rw-rw-rw-   0        0        0      692 2024-03-25 16:32:23.000000 py_neuromodulation-0.0.3/py_neuromodulation/nm_artifacts.py
+-rw-rw-rw-   0        0        0     6322 2024-03-25 16:32:23.000000 py_neuromodulation-0.0.3/py_neuromodulation/nm_bispectra.py
+-rw-rw-rw-   0        0        0     7710 2024-04-12 12:53:13.000000 py_neuromodulation-0.0.3/py_neuromodulation/nm_bursts.py
+-rw-rw-rw-   0        0        0     7435 2024-03-25 16:32:23.000000 py_neuromodulation-0.0.3/py_neuromodulation/nm_coherence.py
+-rw-rw-rw-   0        0        0    16643 2024-03-11 17:49:34.000000 py_neuromodulation-0.0.3/py_neuromodulation/nm_cohortwrapper.py
+-rw-rw-rw-   0        0        0    35645 2024-03-11 17:49:34.000000 py_neuromodulation-0.0.3/py_neuromodulation/nm_decode.py
+-rw-rw-rw-   0        0        0    11074 2024-03-25 16:32:23.000000 py_neuromodulation-0.0.3/py_neuromodulation/nm_define_nmchannels.py
+-rw-rw-rw-   0        0        0     8800 2024-03-11 17:49:34.000000 py_neuromodulation-0.0.3/py_neuromodulation/nm_eval_timing.py
+-rw-rw-rw-   0        0        0     3527 2024-03-25 16:32:23.000000 py_neuromodulation-0.0.3/py_neuromodulation/nm_features.py
+-rw-rw-rw-   0        0        0      917 2024-03-11 17:49:34.000000 py_neuromodulation-0.0.3/py_neuromodulation/nm_features_abc.py
+-rw-rw-rw-   0        0        0     7542 2024-03-25 16:32:23.000000 py_neuromodulation-0.0.3/py_neuromodulation/nm_filter.py
+-rw-rw-rw-   0        0        0     3366 2024-03-25 16:32:23.000000 py_neuromodulation-0.0.3/py_neuromodulation/nm_filter_preprocessing.py
+-rw-rw-rw-   0        0        0     6147 2024-03-25 16:32:23.000000 py_neuromodulation-0.0.3/py_neuromodulation/nm_fooof.py
+-rw-rw-rw-   0        0        0     1088 2024-04-11 13:31:40.000000 py_neuromodulation-0.0.3/py_neuromodulation/nm_generator.py
+-rw-rw-rw-   0        0        0     2180 2024-03-11 17:49:34.000000 py_neuromodulation-0.0.3/py_neuromodulation/nm_hjorth_raw.py
+-rw-rw-rw-   0        0        0     2006 2024-03-11 17:49:34.000000 py_neuromodulation-0.0.3/py_neuromodulation/nm_kalmanfilter.py
+-rw-rw-rw-   0        0        0      954 2024-03-11 17:49:34.000000 py_neuromodulation-0.0.3/py_neuromodulation/nm_linelength.py
+-rw-rw-rw-   0        0        0     3907 2024-03-25 16:32:23.000000 py_neuromodulation-0.0.3/py_neuromodulation/nm_mne_connectivity.py
+-rw-rw-rw-   0        0        0     3660 2024-03-11 17:49:34.000000 py_neuromodulation-0.0.3/py_neuromodulation/nm_nolds.py
+-rw-rw-rw-   0        0        0     7574 2024-03-25 16:32:23.000000 py_neuromodulation-0.0.3/py_neuromodulation/nm_normalization.py
+-rw-rw-rw-   0        0        0    16476 2024-03-25 16:32:23.000000 py_neuromodulation-0.0.3/py_neuromodulation/nm_oscillatory.py
+-rw-rw-rw-   0        0        0    17869 2024-03-25 16:32:23.000000 py_neuromodulation-0.0.3/py_neuromodulation/nm_plots.py
+-rw-rw-rw-   0        0        0    15309 2024-03-25 16:32:23.000000 py_neuromodulation-0.0.3/py_neuromodulation/nm_projection.py
+-rw-rw-rw-   0        0        0     3381 2024-03-25 16:32:23.000000 py_neuromodulation-0.0.3/py_neuromodulation/nm_rereference.py
+-rw-rw-rw-   0        0        0     1122 2024-03-25 16:32:23.000000 py_neuromodulation-0.0.3/py_neuromodulation/nm_resample.py
+-rw-rw-rw-   0        0        0    15046 2024-03-25 16:32:23.000000 py_neuromodulation-0.0.3/py_neuromodulation/nm_run_analysis.py
+-rw-rw-rw-   0        0        0     1775 2024-03-11 17:49:34.000000 py_neuromodulation-0.0.3/py_neuromodulation/nm_settings.py
+-rw-rw-rw-   0        0        0    16891 2024-03-25 16:32:23.000000 py_neuromodulation-0.0.3/py_neuromodulation/nm_sharpwaves.py
+-rw-rw-rw-   0        0        0    16029 2024-03-25 16:32:23.000000 py_neuromodulation-0.0.3/py_neuromodulation/nm_stats.py
+-rw-rw-rw-   0        0        0     7755 2024-03-25 16:32:23.000000 py_neuromodulation-0.0.3/py_neuromodulation/nm_stream_abc.py
+-rw-rw-rw-   0        0        0    12366 2024-04-11 13:31:40.000000 py_neuromodulation-0.0.3/py_neuromodulation/nm_stream_offline.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:14.966246 py_neuromodulation-0.0.3/py_neuromodulation/utils/
+-rw-rw-rw-   0        0        0        0 2024-03-25 16:32:23.000000 py_neuromodulation-0.0.3/py_neuromodulation/utils/__init__.py
+-rw-rw-rw-   0        0        0      738 2024-04-11 13:31:40.000000 py_neuromodulation-0.0.3/py_neuromodulation/utils/_logging.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:15.018954 py_neuromodulation-0.0.3/py_neuromodulation.egg-info/
+-rw-rw-rw-   0        0        0     7213 2024-04-12 13:30:14.000000 py_neuromodulation-0.0.3/py_neuromodulation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    10483 2024-04-12 13:30:14.000000 py_neuromodulation-0.0.3/py_neuromodulation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 13:30:14.000000 py_neuromodulation-0.0.3/py_neuromodulation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      374 2024-04-12 13:30:14.000000 py_neuromodulation-0.0.3/py_neuromodulation.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       75 2024-04-12 13:30:14.000000 py_neuromodulation-0.0.3/py_neuromodulation.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2230 2024-04-12 13:29:54.000000 py_neuromodulation-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-12 13:30:15.018954 py_neuromodulation-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-12 13:30:15.016987 py_neuromodulation-0.0.3/tests/
+-rw-rw-rw-   0        0        0        0 2024-03-11 17:49:34.000000 py_neuromodulation-0.0.3/tests/__init__.py
+-rw-rw-rw-   0        0        0     3107 2024-03-25 16:32:23.000000 py_neuromodulation-0.0.3/tests/conftest.py
+-rw-rw-rw-   0        0        0      285 2024-03-25 16:32:23.000000 py_neuromodulation-0.0.3/tests/test_all_examples.py
+-rw-rw-rw-   0        0        0     1708 2024-03-25 16:32:23.000000 py_neuromodulation-0.0.3/tests/test_all_features.py
+-rw-rw-rw-   0        0        0     1599 2024-03-25 16:32:23.000000 py_neuromodulation-0.0.3/tests/test_bispectra.py
+-rw-rw-rw-   0        0        0     2806 2024-03-25 16:32:23.000000 py_neuromodulation-0.0.3/tests/test_bursts.py
+-rw-rw-rw-   0        0        0     4377 2024-03-25 16:32:23.000000 py_neuromodulation-0.0.3/tests/test_feature_sampling_rates.py
+-rw-rw-rw-   0        0        0      601 2024-03-25 16:32:23.000000 py_neuromodulation-0.0.3/tests/test_fooof.py
+-rw-rw-rw-   0        0        0     1326 2024-03-25 16:32:23.000000 py_neuromodulation-0.0.3/tests/test_initalization_offline_stream.py
+-rw-rw-rw-   0        0        0     2020 2024-03-25 16:32:23.000000 py_neuromodulation-0.0.3/tests/test_multiprocessing.py
+-rw-rw-rw-   0        0        0      808 2024-03-25 16:32:23.000000 py_neuromodulation-0.0.3/tests/test_nan_values.py
+-rw-rw-rw-   0        0        0     3050 2024-03-25 16:32:23.000000 py_neuromodulation-0.0.3/tests/test_nm_filter.py
+-rw-rw-rw-   0        0        0     2104 2024-03-11 17:49:34.000000 py_neuromodulation-0.0.3/tests/test_nm_resample.py
+-rw-rw-rw-   0        0        0     3981 2024-03-25 16:32:23.000000 py_neuromodulation-0.0.3/tests/test_normalization_settings.py
+-rw-rw-rw-   0        0        0      987 2024-03-11 17:49:34.000000 py_neuromodulation-0.0.3/tests/test_notch_filter.py
+-rw-rw-rw-   0        0        0    13046 2024-03-25 16:32:23.000000 py_neuromodulation-0.0.3/tests/test_osc_features.py
+-rw-rw-rw-   0        0        0     5622 2024-03-25 16:32:23.000000 py_neuromodulation-0.0.3/tests/test_preprocessing_filter.py
+-rw-rw-rw-   0        0        0     5174 2024-03-25 16:32:23.000000 py_neuromodulation-0.0.3/tests/test_rereference.py
+-rw-rw-rw-   0        0        0     2000 2024-03-25 16:32:23.000000 py_neuromodulation-0.0.3/tests/test_sampling.py
+-rw-rw-rw-   0        0        0     2262 2024-03-25 16:32:23.000000 py_neuromodulation-0.0.3/tests/test_settings_change_after_init.py
+-rw-rw-rw-   0        0        0     5588 2024-03-11 17:49:34.000000 py_neuromodulation-0.0.3/tests/test_sharpwave.py
+-rw-rw-rw-   0        0        0     3045 2024-03-25 16:32:23.000000 py_neuromodulation-0.0.3/tests/test_target_channel_add.py
+-rw-rw-rw-   0        0        0     2592 2024-03-25 16:32:23.000000 py_neuromodulation-0.0.3/tests/test_timing.py
```

### Comparing `py_neuromodulation-0.0.2/LICENSE` & `py_neuromodulation-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `py_neuromodulation-0.0.2/README.rst` & `py_neuromodulation-0.0.3/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -36,20 +36,32 @@
 
 py_neuromodulation requires at least python 3.10. For installation you can use pip:
 
 .. code-block::
 
     pip install py-neuromodulation
 
-We recommend however installing the package in a new new conda environment:
+
+We recommend however installing the package using `rye <https://rye-up.com/guide/installation/>`_:
 
 .. code-block::
 
     git clone https://github.com/neuromodulation/py_neuromodulation.git
-    conda create -n pynm-test python=3.10
+    rye pin 3.11
+    rye sync
+
+And then activating the virtual environment e.g. in Windows using:
+
+.. code-block::
+
+    .\.venv\Scripts\activate
+
+Alternatively you can also install the package in a conda environment:
+
+    conda create -n pynm-test python=3.11
     conda activate pynm-test
 
 Then install the packages listed in the `pyproject.toml`:
 
 .. code-block::
 
     pip install .
@@ -61,35 +73,35 @@
 
     ipython kernel install --user --name=pynm-test
 
 Then *py_neuromodulation* can be imported via:
 
 .. code-block::
 
-    import py_neuromodulation as py_nm
+    import py_neuromodulation as nm
 
 Basic Usage
 ===========
 
 .. code-block:: python
     
-    import py_neuromodulation as pn
+    import py_neuromodulation as nm
     import numpy as np
     
     NUM_CHANNELS = 5
     NUM_DATA = 10000
     sfreq = 1000  # Hz
-    feature_freq = 3  # Hz
+    sampling_rate_features_hz = 3  # Hz
 
     data = np.random.random([NUM_CHANNELS, NUM_DATA])
 
-    stream = pn.Stream(sfreq=sfreq, data=data, sampling_rate_features_hz=sampling_rate_features_hz)
+    stream = nm.Stream(sfreq=sfreq, data=data, sampling_rate_features_hz=sampling_rate_features_hz)
     features = stream.run()
 
-Check the `Usage <https://py-neuromodulation.readthedocs.io/en/latest/usage.html>`_ and `First examples <https://py-neuromodulation.readthedocs.io/en/latest/auto_examples/plot_first_demo.html>`_ for further introduction.
+Check the `Usage <https://py-neuromodulation.readthedocs.io/en/latest/usage.html>`_ and `First examples <https://py-neuromodulation.readthedocs.io/en/latest/auto_examples/plot_0_first_demo.html>`_ for further introduction.
 
 Contact information
 -------------------
 For any question or suggestion please find my contact
 information at `my GitHub profile <https://github.com/timonmerk>`_.
 
 References
```

### Comparing `py_neuromodulation-0.0.2/py_neuromodulation/FieldTrip.py` & `py_neuromodulation-0.0.3/py_neuromodulation/FieldTrip.py`

 * *Files identical despite different names*

### Comparing `py_neuromodulation-0.0.2/py_neuromodulation/helper.py` & `py_neuromodulation-0.0.3/py_neuromodulation/_write_example_dataset_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import mne
 import mne_bids
-import pybv
+import pybv  # pip install pybv
 import os
 
 
 def set_chtypes(vhdr_raw):
     """
     define MNE RawArray channel types
     """
```

### Comparing `py_neuromodulation-0.0.2/py_neuromodulation/nm_EpochStream.py` & `py_neuromodulation-0.0.3/py_neuromodulation/nm_EpochStream.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import os
 import pickle
 
 import numpy as np
 import pandas as pd
 
-import py_neuromodulation as py_nm
+import py_neuromodulation as nm
 from py_neuromodulation import nm_generator
 
 
-class EpochStream(py_nm.nm_stream.PNStream):
+class EpochStream(nm.nm_stream.PNStream):
     def __init__(self) -> None:
         super().__init__()
 
     def read_epoch_data(self, path_epoch) -> None:
         """Read npy array of epochs. Shape is assumed to be (samples, channels, time)
 
         Parameters
@@ -39,15 +39,14 @@
         """
         for n_batch in range(self.data.shape[0]):
             yield self.data[n_batch, :, :]
 
     def run(
         self,
     ):
-
         self._set_run()
         # shape is n, channels=7, 800 Hz
 
         self.feature_arr = pd.DataFrame()
         self.feature_arr_list = []
         epoch_gen = self.get_data()
         idx_epoch = 0
```

### Comparing `py_neuromodulation-0.0.2/py_neuromodulation/nm_IO.py` & `py_neuromodulation-0.0.3/py_neuromodulation/nm_IO.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 import json
 import os
 import sys
 from pathlib import Path
+import logging
+
+logger = logging.getLogger("PynmLogger")
+
 
 import mne
 import mne_bids
 import numpy as np
 import pandas as pd
 from scipy import io
 
+import pyarrow
+from pyarrow import csv
+
 import py_neuromodulation
 
 _PathLike = str | os.PathLike
 
 
 def load_nm_channels(
     nm_channels: pd.DataFrame | _PathLike,
@@ -23,26 +30,26 @@
     ch_types (list),
     bads (list)
     used_types (list)
     target_keywords (list)
     reference Union[list, str]
     """
 
-    
     if isinstance(nm_channels, pd.DataFrame):
         nm_ch_return = nm_channels
     elif nm_channels:
         if not os.path.isfile(nm_channels):
             raise ValueError(
                 "PATH_NM_CHANNELS is not a valid file. Got: " f"{nm_channels}"
             )
         nm_ch_return = pd.read_csv(nm_channels)
 
     return nm_ch_return
 
+
 def read_BIDS_data(
     PATH_RUN: _PathLike | mne_bids.BIDSPath,
     BIDS_PATH: _PathLike | None = None,
     datatype: str = "ieeg",
     line_noise: int = 50,
 ) -> tuple[mne.io.Raw, np.ndarray, int | float, int, list | None, list | None]:
     """Given a run path and bids data path, read the respective data
@@ -66,18 +73,16 @@
         bids_path = mne_bids.get_bids_path_from_fname(PATH_RUN)
 
     raw_arr = mne_bids.read_raw_bids(bids_path)
     coord_list, coord_names = get_coord_list(raw_arr)
     if raw_arr.info["line_freq"] is not None:
         line_noise = int(raw_arr.info["line_freq"])
     else:
-        print(
-            "Line noise is not available in the data, using value of {} Hz.".format(
-                line_noise
-            )
+        logger.info(
+            f"Line noise is not available in the data, using value of {line_noise} Hz."
         )
     return (
         raw_arr,
         raw_arr.get_data(),
         raw_arr.info["sfreq"],
         line_noise,
         coord_list,
@@ -116,36 +121,36 @@
         )
     return grid
 
 
 def get_annotations(
     PATH_ANNOTATIONS: str, PATH_RUN: str, raw_arr: mne.io.RawArray
 ):
-
     try:
         annot = mne.read_annotations(
             Path(PATH_ANNOTATIONS) / (os.path.basename(PATH_RUN)[:-5] + ".txt")
         )
         raw_arr.set_annotations(annot)
 
         # annotations starting with "BAD" are omitted with reject_by_annotations 'omit' param
         annot_data = raw_arr.get_data(reject_by_annotation="omit")
     except FileNotFoundError:
-        print("Annotations file could not be found")
-        print(
-            "expected location: "
+        logger.critical(
+            "Annotations file could not be found"
+            + "expected location: "
             + str(
-                Path(PATH_ANNOTATIONS) / (os.path.basename(PATH_RUN)[:-5] + ".txt")
+                Path(PATH_ANNOTATIONS)
+                / (os.path.basename(PATH_RUN)[:-5] + ".txt")
             )
         )
     return annot, annot_data, raw_arr
 
 
 def read_plot_modules(
-    PATH_PLOT: _PathLike = Path(__file__).absolute().parent / "plots"
+    PATH_PLOT: _PathLike = Path(__file__).absolute().parent / "plots",
 ):
     """Read required .mat files for plotting
 
     Parameters
     ----------
     PATH_PLOT : regexp, optional
         path to plotting files, by default
@@ -176,63 +181,14 @@
         z_ecog,
         x_stn,
         y_stn,
         z_stn,
     )
 
 
-def add_labels(
-    features: pd.DataFrame,
-    settings: dict,
-    nm_channels: pd.DataFrame,
-    raw_arr_data: np.ndarray,
-    fs: int | float,
-) -> pd.DataFrame | None:
-    """Given a constructed feature data frame, resample the target labels and add to dataframe
-
-    Parameters
-    ----------
-    features : pd.DataFrame
-        computed feature dataframe
-    settings_wrapper : settings.py
-        initialized settings used for feature estimation
-    raw_arr_data : np.ndarray
-        raw data including target
-
-    Returns
-    -------
-    pd.DataFrame | None
-        computed feature dataframe including resampled features
-    """
-    # resample_label
-    ind_label = np.where(nm_channels.target == 1)[0]
-    if ind_label.shape[0] == 0:
-        print("no target specified")
-        return None
-
-    offset_time = settings["segment_length_features_ms"]
-
-    offset_start = np.ceil(offset_time / 1000 * fs).astype(int)
-    data = raw_arr_data[ind_label, offset_start:]
-    if data.ndim == 1:
-        data = np.expand_dims(data, axis=0)
-    label_downsampled = data[
-        :,
-        :: int(np.ceil(fs / settings["sampling_rate_features_hz"])),
-    ]
-
-    # and add to df
-    if features.shape[0] == label_downsampled.shape[1]:
-        for idx, label_ch in enumerate(nm_channels.name[ind_label]):
-            features[label_ch] = label_downsampled[idx, :]
-    else:
-        print("label dimensions don't match, saving downsampled label extra")
-    return features
-
-
 def save_features_and_settings(
     df_features,
     run_analysis,
     folder_name,
     out_path,
     settings,
     nm_channels,
@@ -252,65 +208,75 @@
     folder_name : string
         output path
     settings_wrapper : settings.py object
     """
 
     # create out folder if doesn't exist
     if not os.path.exists(os.path.join(out_path, folder_name)):
-        print("Creating output folder: " + str(folder_name))
+        logger.Info(f"Creating output folder: {folder_name}")
         os.makedirs(os.path.join(out_path, folder_name))
 
     dict_sidecar = {"fs": fs, "coords": coords, "line_noise": line_noise}
 
     save_sidecar(dict_sidecar, out_path, folder_name)
     save_features(df_features, out_path, folder_name)
     save_settings(settings, out_path, folder_name)
     save_nm_channels(nm_channels, out_path, folder_name)
 
 
+def write_csv(df, path_out):
+    """
+    Function to save Pandas dataframes to disk as CSV using
+    PyArrow (almost 10x faster than Pandas)
+    Difference with pandas.df.to_csv() is that it does not
+    write an index column by default
+    """
+    csv.write_csv(pyarrow.Table.from_pandas(df), path_out)
+
+
 def save_settings(
     settings: dict, path_out: _PathLike, folder_name: str | None = None
 ) -> None:
     path_out = _pathlike_to_str(path_out)
     if folder_name is not None:
         path_out = os.path.join(
             path_out, folder_name, folder_name + "_SETTINGS.json"
         )
 
     with open(path_out, "w") as f:
         json.dump(settings, f, indent=4)
-    print("settings.json saved to " + path_out)
+    logger.info(f"settings.json saved to {path_out}")
 
 
 def save_nm_channels(
     nmchannels: pd.DataFrame,
     path_out: _PathLike,
     folder_name: str | None = None,
 ) -> None:
     path_out = _pathlike_to_str(path_out)
     if folder_name is not None:
         path_out = os.path.join(
             path_out, folder_name, folder_name + "_nm_channels.csv"
         )
-    nmchannels.to_csv(path_out)
-    print("nm_channels.csv saved to " + path_out)
+    write_csv(nmchannels, path_out)
+    logger.info(f"nm_channels.csv saved to {path_out}")
 
 
 def save_features(
     df_features: pd.DataFrame,
     path_out: _PathLike,
     folder_name: str | None = None,
 ) -> None:
     path_out = _pathlike_to_str(path_out)
     if folder_name is not None:
         path_out = os.path.join(
             path_out, folder_name, folder_name + "_FEATURES.csv"
         )
-    df_features.to_csv(path_out)
-    print("FEATURES.csv saved to " + str(path_out))
+    write_csv(df_features, path_out)
+    logger.info(f"FEATURES.csv saved to {str(path_out)}")
 
 
 def save_sidecar(
     sidecar: dict, path_out: _PathLike, folder_name: str | None = None
 ) -> None:
     path_out = _pathlike_to_str(path_out)
     save_general_dict(sidecar, path_out, "_SIDECAR.json", folder_name)
@@ -329,15 +295,15 @@
         json.dump(
             dict_,
             f,
             default=default_json_convert,
             indent=4,
             separators=(",", ": "),
         )
-    print(f"{str_add} saved to " + str(path_out))
+    logger.info(f"{str_add} saved to " + str(path_out))
 
 
 def default_json_convert(obj) -> list | int | float:
     if isinstance(obj, np.ndarray):
         return obj.tolist()
     if isinstance(obj, pd.DataFrame):
         return obj.to_numpy().tolist()
@@ -355,19 +321,19 @@
 
 def read_settings(PATH: str) -> dict:
     with open(PATH if ".json" in PATH else PATH + "_SETTINGS.json") as f:
         return json.load(f)
 
 
 def read_features(PATH: str) -> pd.DataFrame:
-    return pd.read_csv(PATH + "_FEATURES.csv", index_col=0)
+    return pd.read_csv(PATH + "_FEATURES.csv", engine="pyarrow")
 
 
 def read_nm_channels(PATH: str) -> pd.DataFrame:
-    return pd.read_csv(PATH + "_nm_channels.csv", index_col=0)
+    return pd.read_csv(PATH + "_nm_channels.csv")
 
 
 def get_run_list_indir(PATH: str) -> list:
     f_files = []
     for dirpath, _, files in os.walk(PATH):
         for x in files:
             if "FEATURES" in x:
@@ -401,15 +367,22 @@
     datatype = "ieeg"
 
     # Define run name and access paths in the BIDS format.
     RUN_NAME = f"sub-{sub}_ses-{ses}_task-{task}_run-{run}"
 
     PATH_BIDS = Path(SCRIPT_DIR) / "data"
 
-    PATH_RUN = Path(SCRIPT_DIR) / "data" / f"sub-{sub}" / f"ses-{ses}" / datatype / RUN_NAME
+    PATH_RUN = (
+        Path(SCRIPT_DIR)
+        / "data"
+        / f"sub-{sub}"
+        / f"ses-{ses}"
+        / datatype
+        / RUN_NAME
+    )
 
     # Provide a path for the output data.
     PATH_OUT = PATH_BIDS / "derivatives"
 
     return RUN_NAME, PATH_RUN, PATH_BIDS, PATH_OUT, datatype
```

### Comparing `py_neuromodulation-0.0.2/py_neuromodulation/nm_across_patient_decoding.py` & `py_neuromodulation-0.0.3/py_neuromodulation/nm_across_patient_decoding.py`

 * *Files identical despite different names*

### Comparing `py_neuromodulation-0.0.2/py_neuromodulation/nm_analysis.py` & `py_neuromodulation-0.0.3/py_neuromodulation/nm_analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -217,15 +217,15 @@
     ) -> pd.DataFrame:
         """Normalize feature_arr feature columns
 
         Returns:
             pd.DataFrame: z-scored feature_arr
         """
         cols_norm = [c for c in self.feature_arr.columns if "time" not in c]
-        feature_arr_norm = stats.zscore(self.feature_arr[cols_norm])
+        feature_arr_norm = stats.zscore(self.feature_arr[cols_norm], nan_policy="omit")
         feature_arr_norm["time"] = self.feature_arr["time"]
         return feature_arr_norm
 
     def plot_cort_projection(self) -> None:
         """_summary_
         """
```

### Comparing `py_neuromodulation-0.0.2/py_neuromodulation/nm_bispectra.py` & `py_neuromodulation-0.0.3/py_neuromodulation/nm_bispectra.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from typing import Iterable
 import numpy as np
 from pybispectra import compute_fft, get_example_data_paths, WaveShape
 
 from py_neuromodulation import nm_features_abc
 
-class Bispectra(nm_features_abc.Feature):
 
-    def __init__(self, settings: dict, ch_names: Iterable[str], sfreq: int | float) -> None:
+class Bispectra(nm_features_abc.Feature):
+    def __init__(
+        self, settings: dict, ch_names: Iterable[str], sfreq: int | float
+    ) -> None:
         super().__init__(settings, ch_names, sfreq)
         self.sfreq = sfreq
         self.ch_names = ch_names
         self.s = settings
         self.f1s = settings["bispectrum"]["f1s"]
         self.f2s = settings["bispectrum"]["f2s"]
 
@@ -36,79 +38,103 @@
             ), f"second frequency range value needs to be higher than first one, got {filter_range}"
             assert filter_range[0] < sfreq and filter_range[1] < sfreq, (
                 "filter frequency range has to be smaller than sfreq, "
                 f"got sfreq {sfreq} and filter range {filter_range}"
             )
 
         test_range("f1s", s["bispectrum"]["f1s"])
-        test_range("f2s", s["bispectrum"]["f2s"])            
+        test_range("f2s", s["bispectrum"]["f2s"])
 
-        for feature_name, val in s["bispectrum"][
-            "components"
-        ].items():
+        for feature_name, val in s["bispectrum"]["components"].items():
             assert isinstance(
                 val, bool
             ), f"bispectrum component {feature_name} has to be of type bool, got {val}"
-        
-        for feature_name, val in s["bispectrum"][
-            "bispectrum_features"
-        ].items():
+
+        for feature_name, val in s["bispectrum"]["bispectrum_features"].items():
             assert isinstance(
                 val, bool
             ), f"bispectrum feature {feature_name} has to be of type bool, got {val}"
 
         assert (
             f_band_bispectrum in s["frequency_ranges_hz"]
             for f_band_bispectrum in s["bispectrum"]["frequency_bands"]
         ), (
             "bispectrum selected frequency bands don't match the ones"
             "specified in s['frequency_ranges_hz']"
             f"bispectrum frequency bands: {s['bispectrum']['frequency_bands']}"
             f"specified frequency_ranges_hz: {s['frequency_ranges_hz']}"
         )
 
-    def compute_bs_features(self, spectrum_ch: np.array, features_compute: dict, ch_name: str, component: str, f_band: str) -> dict:
-        
+    def compute_bs_features(
+        self,
+        spectrum_ch: np.array,
+        features_compute: dict,
+        ch_name: str,
+        component: str,
+        f_band: str,
+    ) -> dict:
         for bispectrum_feature in self.s["bispectrum"]["bispectrum_features"]:
-            
             if bispectrum_feature == "mean":
                 func = np.nanmean
             if bispectrum_feature == "sum":
                 func = np.nansum
             if bispectrum_feature == "var":
                 func = np.nanvar
 
             if f_band is not None:
-                str_feature = "_".join([ch_name, "Bispectrum", component, bispectrum_feature, f_band])
+                str_feature = "_".join(
+                    [
+                        ch_name,
+                        "Bispectrum",
+                        component,
+                        bispectrum_feature,
+                        f_band,
+                    ]
+                )
             else:
-                str_feature = "_".join([ch_name, "Bispectrum", component, bispectrum_feature, "whole_fband_range"])
+                str_feature = "_".join(
+                    [
+                        ch_name,
+                        "Bispectrum",
+                        component,
+                        bispectrum_feature,
+                        "whole_fband_range",
+                    ]
+                )
 
             features_compute[str_feature] = func(spectrum_ch)
 
         return features_compute
 
     def calc_feature(self, data: np.array, features_compute: dict) -> dict:
         for ch_idx, ch_name in enumerate(self.ch_names):
             fft_coeffs, freqs = compute_fft(
-                data=np.expand_dims(data[ch_idx, :], axis=(0,1)),
+                data=np.expand_dims(data[ch_idx, :], axis=(0, 1)),
                 sampling_freq=self.sfreq,
                 n_points=data.shape[1],
-            verbose=False,
+                verbose=False,
             )
 
-            f_spectrum_range = freqs[np.logical_and(freqs >= np.min([self.f1s, self.f2s]), freqs <= np.max([self.f1s, self.f2s]))]
+            f_spectrum_range = freqs[
+                np.logical_and(
+                    freqs >= np.min([self.f1s, self.f2s]),
+                    freqs <= np.max([self.f1s, self.f2s]),
+                )
+            ]
 
             waveshape = WaveShape(
                 data=fft_coeffs,
-                freqs=freqs.astype(int),
+                freqs=freqs,
                 sampling_freq=self.sfreq,
                 verbose=False,
             )
 
-            waveshape.compute(f1s=tuple(self.f1s), f2s=tuple(self.f2s))
+            waveshape.compute(
+                f1s=(self.f1s[0], self.f1s[-1]), f2s=(self.f2s[0], self.f2s[-1])
+            )
 
             bispectrum = np.squeeze(waveshape.results._data)
 
             for component in self.s["bispectrum"]["components"]:
                 if self.s["bispectrum"]["components"][component]:
                     if component == "real":
                         spectrum_ch = bispectrum.real
@@ -116,18 +142,27 @@
                         spectrum_ch = bispectrum.imag
                     if component == "absolute":
                         spectrum_ch = np.abs(bispectrum)
                     if component == "phase":
                         spectrum_ch = np.angle(bispectrum)
 
                 for fb in self.s["bispectrum"]["frequency_bands"]:
-                    range_ = (f_spectrum_range >= self.s["frequency_ranges_hz"][fb][0]) \
-                        & (f_spectrum_range <= self.s["frequency_ranges_hz"][fb][1])
-                    #waveshape.results.plot()
-                    data_bs = spectrum_ch[range_, range_]        
-
-                    features_compute = self.compute_bs_features(data_bs, features_compute, ch_name, component, fb)
-
-                if self.s["bispectrum"]["compute_features_for_whole_fband_range"]:
-                    features_compute = self.compute_bs_features(spectrum_ch, features_compute, ch_name, component, None)
+                    range_ = (
+                        f_spectrum_range >= self.s["frequency_ranges_hz"][fb][0]
+                    ) & (
+                        f_spectrum_range <= self.s["frequency_ranges_hz"][fb][1]
+                    )
+                    # waveshape.results.plot()
+                    data_bs = spectrum_ch[range_, range_]
+
+                    features_compute = self.compute_bs_features(
+                        data_bs, features_compute, ch_name, component, fb
+                    )
+
+                if self.s["bispectrum"][
+                    "compute_features_for_whole_fband_range"
+                ]:
+                    features_compute = self.compute_bs_features(
+                        spectrum_ch, features_compute, ch_name, component, None
+                    )
 
         return features_compute
```

### Comparing `py_neuromodulation-0.0.2/py_neuromodulation/nm_bursts.py` & `py_neuromodulation-0.0.3/py_neuromodulation/nm_bursts.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 import enum
 import numpy as np
 from typing import Iterable
+from scipy import signal
 
 from py_neuromodulation import nm_features_abc, nm_filter
 
 
 class Burst(nm_features_abc.Feature):
     def __init__(
         self, settings: dict, ch_names: Iterable[str], sfreq: float
     ) -> None:
-
         self.s = settings
         self.sfreq = sfreq
         self.ch_names = ch_names
         self.threshold = self.s["burst_settings"]["threshold"]
         self.time_duration_s = self.s["burst_settings"]["time_duration_s"]
+        self.samples_overlap = int(
+            self.sfreq
+            * (self.s["segment_length_features_ms"] / 1000)
+            / self.s["sampling_rate_features_hz"]
+        )
 
         self.fband_names = self.s["burst_settings"]["frequency_bands"]
         self.f_ranges = [
             self.s["frequency_ranges_hz"][fband_name]
             for fband_name in self.fband_names
         ]
         self.seglengths = np.floor(
@@ -30,17 +35,19 @@
                         fband
                     ]
                     for fband in self.fband_names
                 ]
             )
         ).astype(int)
 
-        self.num_max_samples_ring_buffer = int(self.sfreq * self.time_duration_s)
+        self.num_max_samples_ring_buffer = int(
+            self.sfreq * self.time_duration_s
+        )
 
-        self.bandpass_filter = nm_filter.BandPassFilter(
+        self.bandpass_filter = nm_filter.MNEFilter(
             f_ranges=self.f_ranges,
             sfreq=self.sfreq,
             filter_length=self.sfreq - 1,
             verbose=False,
         )
 
         # create dict with fband, channel specific data store
@@ -58,52 +65,61 @@
         self.data_buffer = init_ch_fband_dict()
 
     def test_settings(
         settings: dict,
         ch_names: Iterable[str],
         sfreq: int | float,
     ):
-        assert (
-            isinstance(settings["burst_settings"]["threshold"], (float, int))
+        assert isinstance(
+            settings["burst_settings"]["threshold"], (float, int)
         ), f"burst settings threshold needs to be type int or float, got: {settings['burst_settings']['threshold']}"
         assert (
             0 < settings["burst_settings"]["threshold"] < 100
         ), f"burst setting threshold needs to be between 0 and 100, got: {settings['burst_settings']['threshold']}"
-        assert (
-            isinstance(settings["burst_settings"]["time_duration_s"], (float, int))
+        assert isinstance(
+            settings["burst_settings"]["time_duration_s"], (float, int)
         ), f"burst settings time_duration_s needs to be type int or float, got: {settings['burst_settings']['time_duration_s']}"
         assert (
             settings["burst_settings"]["time_duration_s"] > 0
         ), f"burst setting time_duration_s needs to be greater than 0, got: {settings['burst_settings']['time_duration_s']}"
 
         for fband_burst in settings["burst_settings"]["frequency_bands"]:
-            assert (
-                fband_burst in list(settings["frequency_ranges_hz"].keys())
+            assert fband_burst in list(
+                settings["frequency_ranges_hz"].keys()
             ), f"bursting {fband_burst} needs to be defined in settings['frequency_ranges_hz']"
 
-        for burst_feature in settings["burst_settings"]["burst_features"].keys():
+        for burst_feature in settings["burst_settings"][
+            "burst_features"
+        ].keys():
             assert isinstance(
-                settings["burst_settings"]["burst_features"][burst_feature], bool
+                settings["burst_settings"]["burst_features"][burst_feature],
+                bool,
             ), (
                 f"bursting feature {burst_feature} needs to be type bool, "
                 f"got: {settings['burst_settings']['burst_features'][burst_feature]}"
             )
-    def calc_feature(self, data: np.array, features_compute: dict) -> dict:
 
+    def calc_feature(self, data: np.array, features_compute: dict) -> dict:
         # filter_data returns (n_channels, n_fbands, n_samples)
-        filtered_data = self.bandpass_filter.filter_data(data)
+        filtered_data = np.abs(
+            signal.hilbert(self.bandpass_filter.filter_data(data), axis=2)
+        )
         for ch_idx, ch_name in enumerate(self.ch_names):
             for fband_idx, fband_name in enumerate(self.fband_names):
                 new_dat = filtered_data[ch_idx, fband_idx, :]
                 if self.data_buffer[ch_name][fband_name] is None:
                     self.data_buffer[ch_name][fband_name] = new_dat
                 else:
                     self.data_buffer[ch_name][fband_name] = np.concatenate(
-                        (self.data_buffer[ch_name][fband_name], new_dat), axis=0
-                    )[-self.num_max_samples_ring_buffer:]
+                        (
+                            self.data_buffer[ch_name][fband_name],
+                            new_dat[-self.samples_overlap :],
+                        ),
+                        axis=0,
+                    )[-self.num_max_samples_ring_buffer :]
 
                 # calc features
                 burst_thr = np.percentile(
                     self.data_buffer[ch_name][fband_name], q=self.threshold
                 )
 
                 burst_amplitude, burst_length = self.get_burst_amplitude_length(
@@ -141,44 +157,42 @@
                     else 0
                 )
 
                 in_burst = False
                 if self.data_buffer[ch_name][fband_name][-1] > burst_thr:
                     in_burst = True
 
-                features_compute[
-                    f"{ch_name}_bursts_{fband_name}_in_burst"
-                ] = in_burst
+                features_compute[f"{ch_name}_bursts_{fband_name}_in_burst"] = (
+                    in_burst
+                )
         return features_compute
 
     @staticmethod
     def get_burst_amplitude_length(
         beta_averp_norm, burst_thr: float, sfreq: float
     ):
         """
         Analysing the duration of beta burst
         """
         bursts = np.zeros((beta_averp_norm.shape[0] + 1), dtype=bool)
         bursts[1:] = beta_averp_norm >= burst_thr
         deriv = np.diff(bursts)
-        isburst = False
         burst_length = []
         burst_amplitude = []
-        burst_start = 0
 
-        for index, burst_state in enumerate(deriv):
-            if burst_state == True:
-                if isburst == True:
-                    burst_length.append(index - burst_start)
-                    burst_amplitude.append(beta_averp_norm[burst_start:index])
+        burst_time_points = np.where(deriv == True)[0]
 
-                    isburst = False
-                else:
-                    burst_start = index
-                    isburst = True
+        for i in range(burst_time_points.size // 2):
+            burst_length.append(
+                burst_time_points[2 * i + 1] - burst_time_points[2 * i]
+            )
+            burst_amplitude.append(
+                beta_averp_norm[
+                    burst_time_points[2 * i] : burst_time_points[2 * i + 1]
+                ]
+            )
 
         # the last burst length (in case isburst == True) is omitted,
         # since the true burst length cannot be estimated
-
         burst_length = np.array(burst_length) / sfreq
 
         return burst_amplitude, burst_length
```

### Comparing `py_neuromodulation-0.0.2/py_neuromodulation/nm_coherence.py` & `py_neuromodulation-0.0.3/py_neuromodulation/nm_coherence.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,22 +107,23 @@
                 )
                 features_compute[feature_name] = feature_calc
         return features_compute
 
 
 class NM_Coherence(nm_features_abc.Feature):
 
-    coherence_objects: Iterable[CoherenceObject] = []
+    
 
     def __init__(
         self, settings: dict, ch_names: Iterable[str], sfreq: float
     ) -> None:
         self.s = settings
         self.sfreq = sfreq
         self.ch_names = ch_names
+        self.coherence_objects: Iterable[CoherenceObject] = []
 
         for idx_coh in range(len(self.s["coherence"]["channels"])):
             fband_names = self.s["coherence"]["frequency_bands"]
             fband_specs = []
             for band_name in fband_names:
                 fband_specs.append(self.s["frequency_ranges_hz"][band_name])
```

### Comparing `py_neuromodulation-0.0.2/py_neuromodulation/nm_cohortwrapper.py` & `py_neuromodulation-0.0.3/py_neuromodulation/nm_cohortwrapper.py`

 * *Files identical despite different names*

### Comparing `py_neuromodulation-0.0.2/py_neuromodulation/nm_decode.py` & `py_neuromodulation-0.0.3/py_neuromodulation/nm_decode.py`

 * *Files identical despite different names*

### Comparing `py_neuromodulation-0.0.2/py_neuromodulation/nm_define_nmchannels.py` & `py_neuromodulation-0.0.3/py_neuromodulation/nm_define_nmchannels.py`

 * *Files identical despite different names*

### Comparing `py_neuromodulation-0.0.2/py_neuromodulation/nm_eval_timing.py` & `py_neuromodulation-0.0.3/py_neuromodulation/nm_eval_timing.py`

 * *Files identical despite different names*

### Comparing `py_neuromodulation-0.0.2/py_neuromodulation/nm_features.py` & `py_neuromodulation-0.0.3/py_neuromodulation/nm_features.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     nm_coherence,
     nm_fooof,
     nm_nolds,
     nm_features_abc,
     nm_oscillatory,
     nm_bursts,
     nm_linelength,
-    nm_bispectra
+    nm_bispectra,
 )
 
 
 class Features:
     """Class for calculating features."""
 
     features: list[nm_features_abc.Feature] = []
@@ -52,14 +52,16 @@
                     FeatureClass = nm_hjorth_raw.Raw
                 case "bandpass_filter":
                     FeatureClass = nm_oscillatory.BandPower
                 case "stft":
                     FeatureClass = nm_oscillatory.STFT
                 case "fft":
                     FeatureClass = nm_oscillatory.FFT
+                case "welch":
+                    FeatureClass = nm_oscillatory.Welch
                 case "sharpwave_analysis":
                     FeatureClass = nm_sharpwaves.SharpwaveAnalyzer
                 case "fooof":
                     FeatureClass = nm_fooof.FooofAnalyzer
                 case "nolds":
                     FeatureClass = nm_nolds.Nolds
                 case "coherence":
@@ -107,8 +109,8 @@
 
         for feature in self.features:
             features_compute = feature.calc_feature(
                 data,
                 features_compute,
             )
 
-        return features_compute
+        return features_compute
```

### Comparing `py_neuromodulation-0.0.2/py_neuromodulation/nm_features_abc.py` & `py_neuromodulation-0.0.3/py_neuromodulation/nm_features_abc.py`

 * *Files identical despite different names*

### Comparing `py_neuromodulation-0.0.2/py_neuromodulation/nm_filter.py` & `py_neuromodulation-0.0.3/py_neuromodulation/nm_filter.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 """Module for filter functionality."""
+
+import logging
+
+logger = logging.getLogger("PynmLogger")
+
 import mne
 from mne.filter import _overlap_add_filter
 import numpy as np
 
 
-class BandPassFilter:
-    """Bandpass filters data in given frequency ranges.
+class MNEFilter:
+    """mne.filter wrapper
 
     This class stores for given frequency band ranges the filter
     coefficients with length "filter_len".
     The filters can then be used sequentially for band power estimation with
     apply_filter().
+    Note that this filter can be a bandpass, bandstop, lowpass, or highpass filter
+    depending on the frequency ranges given (see further details in mne.filter.create_filter).
 
     Parameters
     ----------
     f_ranges : list of lists
         Frequency ranges. Inner lists must be of length 2.
     sfreq : int | float
         Sampling frequency.
@@ -31,38 +38,52 @@
     ----------
     filter_bank: np.ndarray shape (n,)
         Factor to upsample by.
     """
 
     def __init__(
         self,
-        f_ranges: list[list[int | float | None]],
+        f_ranges: list[list[int | float | None]] | list[int | float | None],
         sfreq: int | float,
         filter_length: str | float = "999ms",
         l_trans_bandwidth: int | float | str = 4,
         h_trans_bandwidth: int | float | str = 4,
         verbose: bool | int | str | None = None,
     ) -> None:
         filter_bank = []
-        # mne create_filter function only accepts str and int
+        # mne create_filter function only accepts str and int for filter_length
         if isinstance(filter_length, float):
             filter_length = int(filter_length)
 
+        if not isinstance(f_ranges[0], list):
+            f_ranges = [f_ranges]
+
         for f_range in f_ranges:
-            filt = mne.filter.create_filter(
-                None,
-                sfreq,
-                l_freq=f_range[0],
-                h_freq=f_range[1],
-                fir_design="firwin",
-                l_trans_bandwidth=l_trans_bandwidth,  # type: ignore
-                h_trans_bandwidth=h_trans_bandwidth,  # type: ignore
-                filter_length=filter_length,  # type: ignore
-                verbose=verbose,
-            )
+            try:
+                filt = mne.filter.create_filter(
+                    None,
+                    sfreq,
+                    l_freq=f_range[0],
+                    h_freq=f_range[1],
+                    fir_design="firwin",
+                    l_trans_bandwidth=l_trans_bandwidth,  # type: ignore
+                    h_trans_bandwidth=h_trans_bandwidth,  # type: ignore
+                    filter_length=filter_length,  # type: ignore
+                    verbose=verbose,
+                )
+            except:
+                filt = mne.filter.create_filter(
+                    None,
+                    sfreq,
+                    l_freq=f_range[0],
+                    h_freq=f_range[1],
+                    fir_design="firwin",
+                    verbose=verbose,
+                    # filter_length=filter_length,
+                )
             filter_bank.append(filt)
         self.filter_bank = np.vstack(filter_bank)
 
     def filter_data(self, data: np.ndarray) -> np.ndarray:
         """Apply previously calculated (bandpass) filters to data.
 
         Parameters
@@ -73,35 +94,45 @@
             Output of calc_bandpass_filters.
 
         Returns
         -------
         np.ndarray, shape (n_channels, n_fbands, n_samples)
             Filtered data.
 
-        Raises
-        ------
-        ValueError
-            If data.ndim > 2
         """
         if data.ndim > 2:
             raise ValueError(
                 f"Data must have one or two dimensions. Got:"
                 f" {data.ndim} dimensions."
             )
         if data.ndim == 1:
             data = np.expand_dims(data, axis=0)
+
         filtered = np.array(
             [
                 [
-                    np.convolve(flt, chan, mode="same")
-                    for flt in self.filter_bank
+                    np.convolve(filt, chan, mode="same")
+                    for filt in self.filter_bank
                 ]
                 for chan in data
             ]
         )
+
+        # ensure here that the output dimension matches the input dimension
+        if data.shape[1] != filtered.shape[-1]:
+            # select the middle part of the filtered data
+            middle_index = filtered.shape[-1] // 2
+            filtered = filtered[
+                :,
+                :,
+                middle_index
+                - data.shape[1] // 2 : middle_index
+                + data.shape[1] // 2,
+            ]
+
         return filtered
 
 
 class NotchFilter:
     def __init__(
         self,
         sfreq: int | float,
@@ -121,15 +152,15 @@
         if freqs.size > 0:
             if freqs[-1] >= sfreq / 2:
                 freqs = freqs[:-1]
 
         # Code is copied from filter.py notch_filter
         if freqs.size == 0:
             self.filter_bank = None
-            print(
+            logger.warning(
                 "WARNING: notch_filter is activated but data is not being"
                 f" filtered. This may be due to a low sampling frequency or"
                 f" incorrect specifications. Make sure your settings are"
                 f" correct. Got: {sfreq = }, {line_noise = }, {freqs = }."
             )
             return
 
@@ -166,23 +197,23 @@
             l_trans_bandwidth=tb_half,  # type: ignore
             h_trans_bandwidth=tb_half,  # type: ignore
             method="fir",
             iir_params=None,
             phase="zero",
             fir_window="hamming",
             fir_design="firwin",
-            verbose=False
+            verbose=False,
         )
 
     def process(self, data: np.ndarray) -> np.ndarray:
         if self.filter_bank is None:
             return data
         return _overlap_add_filter(
-                x=data,
-                h=self.filter_bank,
-                n_fft=None,
-                phase="zero",
-                picks=None,
-                n_jobs=1,
-                copy=True,
-                pad="reflect_limited",
-            )
+            x=data,
+            h=self.filter_bank,
+            n_fft=None,
+            phase="zero",
+            picks=None,
+            n_jobs=1,
+            copy=True,
+            pad="reflect_limited",
+        )
```

### Comparing `py_neuromodulation-0.0.2/py_neuromodulation/nm_fooof.py` & `py_neuromodulation-0.0.3/py_neuromodulation/nm_fooof.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+import logging
+from typing import Iterable
+
 import numpy as np
 from fooof import FOOOF
 from scipy import fft
-from typing import Iterable
 
 from py_neuromodulation import nm_features_abc
 
 
 class FooofAnalyzer(nm_features_abc.Feature):
     def __init__(
         self, settings: dict, ch_names: Iterable[str], sfreq: float
@@ -14,23 +16,14 @@
         self.sfreq = sfreq
         self.ch_names = ch_names
 
         self.freq_range = self.settings_fooof["freq_range_hz"]
         self.ap_mode = "knee" if self.settings_fooof["knee"] else "fixed"
         self.max_n_peaks = self.settings_fooof["max_n_peaks"]
 
-        self.fm = FOOOF(
-            aperiodic_mode=self.ap_mode,
-            peak_width_limits=self.settings_fooof["peak_width_limits"],
-            max_n_peaks=self.settings_fooof["max_n_peaks"],
-            min_peak_height=self.settings_fooof["min_peak_height"],
-            peak_threshold=self.settings_fooof["peak_threshold"],
-            verbose=False,
-        )
-
         self.num_samples = int(
             self.settings_fooof["windowlength_ms"] * sfreq / 1000
         )
 
         self.f_vec = np.arange(0, int(self.num_samples / 2) + 1, 1)
 
     def test_settings(
@@ -71,62 +64,87 @@
         data: np.array,
         features_compute: dict,
     ) -> dict:
         for ch_idx, ch_name in enumerate(self.ch_names):
             spectrum = self._get_spectrum(data[ch_idx, :])
 
             try:
-                self.fm.fit(self.f_vec, spectrum, self.freq_range)
+                fm = FOOOF(
+                    aperiodic_mode=self.ap_mode,
+                    peak_width_limits=self.settings_fooof["peak_width_limits"],
+                    max_n_peaks=self.settings_fooof["max_n_peaks"],
+                    min_peak_height=self.settings_fooof["min_peak_height"],
+                    peak_threshold=self.settings_fooof["peak_threshold"],
+                    verbose=False,
+                )
+                fm.fit(self.f_vec, spectrum, self.freq_range)
             except Exception as e:
-                print(e)
-                print(f"failing spectrum: {spectrum}")
+                logging.critical(e, exc_info=True)
+
+            if fm.fooofed_spectrum_ is None:
+                FIT_PASSED = False
+            else:
+                FIT_PASSED = True
+
             if self.settings_fooof["aperiodic"]["exponent"]:
                 features_compute[f"{ch_name}_fooof_a_exp"] = (
-                    np.nan_to_num(self.fm.get_params("aperiodic_params", "exponent"))
-                    if self.fm.fooofed_spectrum_ is not None
+                    np.nan_to_num(fm.get_params("aperiodic_params", "exponent"))
+                    if FIT_PASSED is True
                     else None
                 )
 
             if self.settings_fooof["aperiodic"]["offset"]:
                 features_compute[f"{ch_name}_fooof_a_offset"] = (
-                    np.nan_to_num(self.fm.get_params("aperiodic_params", "offset"))
-                    if self.fm.fooofed_spectrum_ is not None
+                    np.nan_to_num(fm.get_params("aperiodic_params", "offset"))
+                    if FIT_PASSED is True
                     else None
                 )
-            
+
             if self.settings_fooof["aperiodic"]["knee"]:
-                features_compute[f"{ch_name}_fooof_a_knee"] = (
-                    np.nan_to_num(self.fm.get_params("aperiodic_params", "knee"))
-                    if self.fm.fooofed_spectrum_ is not None
-                    else None
+                if FIT_PASSED is False:
+                    knee_freq = None
+                else:
+                    if fm.get_params("aperiodic_params", "exponent") != 0:
+                        knee_fooof = fm.get_params("aperiodic_params", "knee")
+                        knee_freq = np.nan_to_num(
+                            knee_fooof
+                            ** (
+                                1
+                                / fm.get_params("aperiodic_params", "exponent")
+                            )
+                        )
+                    else:
+                        knee_freq = None
+
+                features_compute[f"{ch_name}_fooof_a_knee_frequency"] = (
+                    knee_freq
                 )
 
             peaks_bw = (
-                self.fm.get_params("peak_params", "BW")
-                if self.fm.fooofed_spectrum_ is not None
+                fm.get_params("peak_params", "BW")
+                if FIT_PASSED is True
                 else None
             )
             peaks_cf = (
-                self.fm.get_params("peak_params", "CF")
-                if self.fm.fooofed_spectrum_ is not None
+                fm.get_params("peak_params", "CF")
+                if FIT_PASSED is True
                 else None
             )
             peaks_pw = (
-                self.fm.get_params("peak_params", "PW")
-                if self.fm.fooofed_spectrum_ is not None
+                fm.get_params("peak_params", "PW")
+                if FIT_PASSED is True
                 else None
             )
 
             if type(peaks_bw) is np.float64 or peaks_bw is None:
                 peaks_bw = [peaks_bw]
                 peaks_cf = [peaks_cf]
                 peaks_pw = [peaks_pw]
 
             for peak_idx in range(self.max_n_peaks):
-
                 if self.settings_fooof["periodic"]["band_width"]:
                     features_compute[f"{ch_name}_fooof_p_{peak_idx}_bw"] = (
                         peaks_bw[peak_idx] if peak_idx < len(peaks_bw) else None
                     )
 
                 if self.settings_fooof["periodic"]["center_frequency"]:
                     features_compute[f"{ch_name}_fooof_p_{peak_idx}_cf"] = (
```

### Comparing `py_neuromodulation-0.0.2/py_neuromodulation/nm_generator.py` & `py_neuromodulation-0.0.3/py_neuromodulation/nm_generator.py`

 * *Files identical despite different names*

### Comparing `py_neuromodulation-0.0.2/py_neuromodulation/nm_hjorth_raw.py` & `py_neuromodulation-0.0.3/py_neuromodulation/nm_hjorth_raw.py`

 * *Files identical despite different names*

### Comparing `py_neuromodulation-0.0.2/py_neuromodulation/nm_kalmanfilter.py` & `py_neuromodulation-0.0.3/py_neuromodulation/nm_kalmanfilter.py`

 * *Files identical despite different names*

### Comparing `py_neuromodulation-0.0.2/py_neuromodulation/nm_linelength.py` & `py_neuromodulation-0.0.3/py_neuromodulation/nm_linelength.py`

 * *Files identical despite different names*

### Comparing `py_neuromodulation-0.0.2/py_neuromodulation/nm_mne_connectivity.py` & `py_neuromodulation-0.0.3/py_neuromodulation/nm_mne_connectivity.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
             tmax=epoch_length,
             baseline=None,
             reject_by_annotation=True,
         )
         if epochs.events.shape[0] < 2:
             raise Exception(
                 f"A minimum of 2 epochs is required for mne_connectivity,"
-                f" got only {epochs.events.shape[0]}. Increase settings['segment_length']"
+                f" got only {epochs.events.shape[0]}. Increase settings['segment_length_features_ms']"
             )
         return epochs
 
     def estimate_connectivity(self, epochs: mne.Epochs):
         # n_jobs is here kept to 1, since setup of the multiprocessing Pool 
         # takes longer than most batch computing sizes
```

### Comparing `py_neuromodulation-0.0.2/py_neuromodulation/nm_nolds.py` & `py_neuromodulation-0.0.3/py_neuromodulation/nm_nolds.py`

 * *Files identical despite different names*

### Comparing `py_neuromodulation-0.0.2/py_neuromodulation/nm_normalization.py` & `py_neuromodulation-0.0.3/py_neuromodulation/nm_normalization.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 """Module for real-time data normalization."""
 from enum import Enum
 
 from sklearn import preprocessing
 import numpy as np
-
-
 class NORM_METHODS(Enum):
     MEAN = "mean"
     MEDIAN = "median"
     ZSCORE = "zscore"
     ZSCORE_MEDIAN = "zscore-median"
     QUANTILE = "quantile"
     POWER = "power"
@@ -134,99 +132,77 @@
             description="feature",
         )
         if self.previous.shape[0] >= self.num_samples_normalize:
             self.previous = self.previous[1:]
 
         return data
 
+"""
+Functions to check for NaN's before deciding which Numpy function to call
+"""
+def nan_mean(data, axis):
+    return np.nanmean(data, axis=axis) if np.any(np.isnan(sum(data))) else np.mean(data, axis=axis)
+
+def nan_std(data, axis):
+    return np.nanstd(data, axis=axis) if np.any(np.isnan(sum(data))) else np.std(data, axis=axis)
+
+def nan_median(data, axis):
+    return np.nanmedian(data, axis=axis) if np.any(np.isnan(sum(data))) else np.median(data, axis=axis)
 
 def _normalize_and_clip(
     current: np.ndarray,
     previous: np.ndarray,
     method: str,
     clip: int | float | bool,
     description: str,
 ) -> tuple[np.ndarray, np.ndarray]:
     """Normalize data."""
-    if method == NORM_METHODS.MEAN.value:
-        mean = np.nanmean(previous, axis=0)
-        current = (current - mean) / mean
-    elif method == NORM_METHODS.MEDIAN.value:
-        median = np.nanmedian(previous, axis=0)
-        current = (current - median) / median
-    elif method == NORM_METHODS.ZSCORE.value:
-        mean = np.nanmean(previous, axis=0)
-        current = (current - mean) / np.nanstd(previous, axis=0)
-    elif method == NORM_METHODS.ZSCORE_MEDIAN.value:
-        current = (current - np.nanmedian(previous, axis=0)) / np.nanstd(
-            previous, axis=0
-        )
-    # For the following methods we check for the shape of current
-    # when current is a 1D array, then it is the post-processing normalization,
-    # and we need to expand, and take the [0, :] component
-    # When current is a 2D array, then it is pre-processing normalization, and
-    # there's no need for expanding.
-    elif method == NORM_METHODS.QUANTILE.value:
-        if len(current.shape) == 1:
-            current = (
-                preprocessing.QuantileTransformer(n_quantiles=300)
-                .fit(np.nan_to_num(previous))
-                .transform(np.expand_dims(current, axis=0))[0, :]
-            )
-        else:
-            current = (
-                preprocessing.QuantileTransformer(n_quantiles=300)
-                .fit(np.nan_to_num(previous))
-                .transform(current)
-            )
-    elif method == NORM_METHODS.ROBUST.value:
-        if len(current.shape) == 1:
-            current = (
-                preprocessing.RobustScaler()
-                .fit(np.nan_to_num(previous))
-                .transform(np.expand_dims(current, axis=0))[0, :]
-            )
-        else:
-            current = (
-                preprocessing.RobustScaler()
-                .fit(np.nan_to_num(previous))
-                .transform(current)
-            )
-
-    elif method == NORM_METHODS.MINMAX.value:
-        if len(current.shape) == 1:
-            current = (
-                preprocessing.MinMaxScaler()
-                .fit(np.nan_to_num(previous))
-                .transform(np.expand_dims(current, axis=0))[0, :]
-            )
-        else:
-            current = (
-                preprocessing.MinMaxScaler()
-                .fit(np.nan_to_num(previous))
-                .transform(current)
+    match method:
+        case NORM_METHODS.MEAN.value:
+            mean = nan_mean(previous, axis=0)
+            current = (current - mean) / mean
+        case NORM_METHODS.MEDIAN.value:
+            median = nan_median(previous, axis=0)
+            current = (current - median) / median
+        case NORM_METHODS.ZSCORE.value:
+            current = (current - nan_mean(previous, axis=0)) / nan_std(previous, axis=0)
+        case NORM_METHODS.ZSCORE_MEDIAN.value:
+            current = (current - nan_median(previous, axis=0)) / nan_std(previous, axis=0)
+        # For the following methods we check for the shape of current
+        # when current is a 1D array, then it is the post-processing normalization,
+        # and we need to expand, and remove the extra dimension afterwards
+        # When current is a 2D array, then it is pre-processing normalization, and
+        # there's no need for expanding.
+        case (NORM_METHODS.QUANTILE.value | 
+              NORM_METHODS.ROBUST.value | 
+              NORM_METHODS.MINMAX.value | 
+              NORM_METHODS.POWER.value):
+            
+            norm_methods = {
+                NORM_METHODS.QUANTILE.value : lambda: preprocessing.QuantileTransformer(n_quantiles=300),
+                NORM_METHODS.ROBUST.value : preprocessing.RobustScaler,
+                NORM_METHODS.MINMAX.value : preprocessing.MinMaxScaler,
+                NORM_METHODS.POWER.value : preprocessing.PowerTransformer
+            }
+                
+            current = (
+                norm_methods[method]()
+                .fit(np.nan_to_num(previous))
+                .transform(
+                    # if post-processing: pad dimensions to 2
+                    np.reshape(current, (2-len(current.shape))*(1,) + current.shape)
+                    )
+                .squeeze() # if post-processing: remove extra dimension
+            )
+            
+        case _:
+            raise ValueError(
+                f"Only {[e.value for e in NORM_METHODS]} are supported as "
+                f"{description} normalization methods. Got {method}."
             )
-    elif method == NORM_METHODS.POWER.value:
-        if len(current.shape) == 1:
-            current = (
-                preprocessing.PowerTransformer()
-                .fit(np.nan_to_num(previous))
-                .transform(np.expand_dims(current, axis=0))[0, :]
-            )
-        else:
-            current = (
-                preprocessing.PowerTransformer()
-                .fit(np.nan_to_num(previous))
-                .transform(current)
-            )
-    else:
-        raise ValueError(
-            f"Only {[e.value for e in NORM_METHODS]} are supported as "
-            f"{description} normalization methods. Got {method}."
-        )
 
     if clip:
         current = _clip(data=current, clip=clip)
     return current, previous
 
 
 def _clip(data: np.ndarray, clip: bool | int | float) -> np.ndarray:
```

### Comparing `py_neuromodulation-0.0.2/py_neuromodulation/nm_oscillatory.py` & `py_neuromodulation-0.0.3/py_neuromodulation/nm_oscillatory.py`

 * *Files 16% similar despite different names*

```diff
@@ -34,30 +34,33 @@
             f"got sfreq = {sfreq} and fband ranges {s['frequency_ranges_hz']}"
         )
 
         if osc_feature_name != "bandpass_filter_settings":
             assert isinstance(
                 s[osc_feature_name]["windowlength_ms"], int
             ), f"windowlength_ms needs to be type int, got {s[osc_feature_name]['windowlength_ms']}"
+
+            assert (
+                s[osc_feature_name]["windowlength_ms"]
+                <= s["segment_length_features_ms"]
+            ), (
+                f"oscillatory feature windowlength_ms = ({s[osc_feature_name]['windowlength_ms']})"
+                f"needs to be smaller than"
+                f"s['segment_length_features_ms'] = {s['segment_length_features_ms']}",
+            )
         else:
             for seg_length in s[osc_feature_name][
                 "segment_lengths_ms"
             ].values():
                 assert isinstance(
                     seg_length, int
                 ), f"segment length has to be type int, got {seg_length}"
         assert isinstance(
             s[osc_feature_name]["log_transform"], bool
         ), f"log_transform needs to be type bool, got {s[osc_feature_name]['log_transform']}"
-        assert isinstance(
-            s[osc_feature_name]["kalman_filter"], bool
-        ), f"kalman_filter needs to be type bool, got {s[osc_feature_name]['kalman_filter']}"
-
-        if s[osc_feature_name]["kalman_filter"] is True:
-            nm_kalmanfilter.test_kf_settings(s, ch_names, sfreq)
 
         assert isinstance(s["frequency_ranges_hz"], dict)
 
         assert (
             isinstance(value, list)
             for value in s["frequency_ranges_hz"].values()
         )
@@ -91,108 +94,222 @@
     def update_KF(self, feature_calc: float, KF_name: str) -> float:
         if KF_name in self.KF_dict:
             self.KF_dict[KF_name].predict()
             self.KF_dict[KF_name].update(feature_calc)
             feature_calc = self.KF_dict[KF_name].x[0]
         return feature_calc
 
+    def estimate_osc_features(
+        self,
+        features_compute: dict,
+        data: np.ndarray,
+        feature_name: np.ndarray,
+        est_name: str,
+    ):
+        for feature_est_name in list(self.s[est_name]["features"].keys()):
+            if self.s[est_name]["features"][feature_est_name] is True:
+                # switch case for feature_est_name
+                match feature_est_name:
+                    case "mean":
+                        features_compute[
+                            f"{feature_name}_{feature_est_name}"
+                        ] = np.nanmean(data)
+                    case "median":
+                        features_compute[
+                            f"{feature_name}_{feature_est_name}"
+                        ] = np.nanmedian(data)
+                    case "std":
+                        features_compute[
+                            f"{feature_name}_{feature_est_name}"
+                        ] = np.nanstd(data)
+                    case "max":
+                        features_compute[
+                            f"{feature_name}_{feature_est_name}"
+                        ] = np.nanmax(data)
+
+        return features_compute
+
 
 class FFT(OscillatoryFeature):
     def __init__(
         self,
         settings: dict,
         ch_names: Iterable[str],
         sfreq: float,
     ) -> None:
         super().__init__(settings, ch_names, sfreq)
-        if self.s["fft_settings"]["kalman_filter"]:
-            self.init_KF("fft")
 
         if self.s["fft_settings"]["log_transform"]:
             self.log_transform = True
         else:
             self.log_transform = False
 
         window_ms = self.s["fft_settings"]["windowlength_ms"]
         self.window_samples = int(-np.floor(window_ms / 1000 * sfreq))
-        freqs = fft.rfftfreq(-self.window_samples, 1 / np.floor(self.sfreq))
+        self.freqs = fft.rfftfreq(
+            -self.window_samples, 1 / np.floor(self.sfreq)
+        )
 
         self.feature_params = []
         for ch_idx, ch_name in enumerate(self.ch_names):
             for fband, f_range in self.f_ranges_dict.items():
                 idx_range = np.where(
-                    (freqs >= f_range[0]) & (freqs < f_range[1])
+                    (self.freqs >= f_range[0]) & (self.freqs < f_range[1])
                 )[0]
                 feature_name = "_".join([ch_name, "fft", fband])
                 self.feature_params.append((ch_idx, feature_name, idx_range))
 
     @staticmethod
     def test_settings(s: dict, ch_names: Iterable[str], sfreq: int | float):
         OscillatoryFeature.test_settings_osc(s, ch_names, sfreq, "fft_settings")
 
     def calc_feature(self, data: np.ndarray, features_compute: dict) -> dict:
         data = data[:, self.window_samples :]
         Z = np.abs(fft.rfft(data))
+
+        if self.log_transform:
+            Z = np.log10(Z)
+
         for ch_idx, feature_name, idx_range in self.feature_params:
             Z_ch = Z[ch_idx, idx_range]
-            feature_calc = np.mean(Z_ch)
 
-            if self.log_transform:
-                feature_calc = np.log(feature_calc)
+            features_compute = self.estimate_osc_features(
+                features_compute, Z_ch, feature_name, "fft_settings"
+            )
+
+        for ch_idx, ch_name in enumerate(self.ch_names):
+            if self.s["fft_settings"]["return_spectrum"]:
+                features_compute.update(
+                    {
+                        f"{ch_name}_fft_psd_{str(f)}": Z[ch_idx][idx]
+                        for idx, f in enumerate(self.freqs.astype(int))
+                    }
+                )
+
+        return features_compute
+
+
+class Welch(OscillatoryFeature):
+    def __init__(
+        self,
+        settings: dict,
+        ch_names: Iterable[str],
+        sfreq: float,
+    ) -> None:
+        super().__init__(settings, ch_names, sfreq)
+
+        self.log_transform = self.s["welch_settings"]["log_transform"]
+
+        self.feature_params = []
+        for ch_idx, ch_name in enumerate(self.ch_names):
+            for fband, f_range in self.f_ranges_dict.items():
+                feature_name = "_".join([ch_name, "welch", fband])
+                self.feature_params.append((ch_idx, feature_name, f_range))
+
+    @staticmethod
+    def test_settings(s: dict, ch_names: Iterable[str], sfreq: int | float):
+        OscillatoryFeature.test_settings_osc(
+            s, ch_names, sfreq, "welch_settings"
+        )
+
+    def calc_feature(self, data: np.ndarray, features_compute: dict) -> dict:
+        freqs, Z = signal.welch(
+            data,
+            fs=self.sfreq,
+            window="hann",
+            nperseg=self.sfreq,
+            noverlap=None,
+        )
 
-            if self.KF_dict:
-                feature_calc = self.update_KF(feature_calc, feature_name)
+        if self.log_transform:
+            Z = np.log10(Z)
+
+        for ch_idx, feature_name, f_range in self.feature_params:
+            Z_ch = Z[ch_idx]
+
+            idx_range = np.where((freqs >= f_range[0]) & (freqs <= f_range[1]))[
+                0
+            ]
+
+            features_compute = self.estimate_osc_features(
+                features_compute,
+                Z_ch[idx_range],
+                feature_name,
+                "welch_settings",
+            )
+
+        for ch_idx, ch_name in enumerate(self.ch_names):
+            if self.s["welch_settings"]["return_spectrum"]:
+                features_compute.update(
+                    {
+                        f"{ch_name}_welch_psd_{str(f)}": Z[ch_idx][idx]
+                        for idx, f in enumerate(freqs.astype(int))
+                    }
+                )
 
-            features_compute[feature_name] = feature_calc
         return features_compute
 
 
 class STFT(OscillatoryFeature):
     def __init__(
         self,
         settings: dict,
         ch_names: Iterable[str],
         sfreq: float,
     ) -> None:
         super().__init__(settings, ch_names, sfreq)
-        if self.s["stft_settings"]["kalman_filter"]:
-            self.init_KF("stft")
 
         self.nperseg = int(self.s["stft_settings"]["windowlength_ms"])
+        self.log_transform = self.s["stft_settings"]["log_transform"]
 
         self.feature_params = []
         for ch_idx, ch_name in enumerate(self.ch_names):
             for fband, f_range in self.f_ranges_dict.items():
                 feature_name = "_".join([ch_name, "stft", fband])
                 self.feature_params.append((ch_idx, feature_name, f_range))
 
     @staticmethod
     def test_settings(s: dict, ch_names: Iterable[str], sfreq: int | float):
         OscillatoryFeature.test_settings_osc(
             s, ch_names, sfreq, "stft_settings"
         )
 
     def calc_feature(self, data: np.ndarray, features_compute: dict) -> dict:
-        f, _, Zxx = signal.stft(
+        freqs, _, Zxx = signal.stft(
             data,
             fs=self.sfreq,
             window="hamming",
             nperseg=self.nperseg,
             boundary="even",
         )
         Z = np.abs(Zxx)
+        if self.log_transform:
+            Z = np.log10(Z)
         for ch_idx, feature_name, f_range in self.feature_params:
             Z_ch = Z[ch_idx]
-            idx_range = np.where((f >= f_range[0]) & (f <= f_range[1]))[0]
-            feature_calc = np.mean(Z_ch[idx_range, :])  # 1. dim: f, 2. dim: t
-
-            if self.KF_dict:
-                feature_calc = self.update_KF(feature_calc, feature_name)
+            idx_range = np.where((freqs >= f_range[0]) & (freqs <= f_range[1]))[
+                0
+            ]
+
+            features_compute = self.estimate_osc_features(
+                features_compute,
+                Z_ch[idx_range, :],
+                feature_name,
+                "stft_settings",
+            )
 
-            features_compute[feature_name] = feature_calc
+        for ch_idx, ch_name in enumerate(self.ch_names):
+            if self.s["stft_settings"]["return_spectrum"]:
+                Z_ch_mean = Z[ch_idx].mean(axis=1)
+                features_compute.update(
+                    {
+                        f"{ch_name}_stft_psd_{str(f)}": Z_ch_mean[idx]
+                        for idx, f in enumerate(freqs.astype(int))
+                    }
+                )
 
         return features_compute
 
 
 class BandPower(OscillatoryFeature):
     def __init__(
         self,
@@ -200,15 +317,15 @@
         ch_names: Iterable[str],
         sfreq: float,
         use_kf: bool = None,
     ) -> None:
         super().__init__(settings, ch_names, sfreq)
         bp_settings = self.s["bandpass_filter_settings"]
 
-        self.bandpass_filter = nm_filter.BandPassFilter(
+        self.bandpass_filter = nm_filter.MNEFilter(
             f_ranges=list(self.f_ranges_dict.values()),
             sfreq=self.sfreq,
             filter_length=self.sfreq - 1,
             verbose=False,
         )
 
         self.log_transform = bp_settings["log_transform"]
@@ -261,47 +378,50 @@
         assert any(
             value is True
             for value in s["bandpass_filter_settings"][
                 "bandpower_features"
             ].values()
         ), "Set at least one bandpower_feature to True."
 
-        for fband_name, seg_length_fband in s["bandpass_filter_settings"]["segment_lengths_ms"].items():
+        for fband_name, seg_length_fband in s["bandpass_filter_settings"][
+            "segment_lengths_ms"
+        ].items():
             assert isinstance(seg_length_fband, int), (
                 f"bandpass segment_lengths_ms for {fband_name} "
                 f"needs to be of type int, got {seg_length_fband}"
             )
 
             assert seg_length_fband <= s["segment_length_features_ms"], (
                 f"segment length {seg_length_fband} needs to be smaller than "
                 f" s['segment_length_features_ms'] = {s['segment_length_features_ms']}"
             )
- 
+
         for fband_name in list(s["frequency_ranges_hz"].keys()):
-            assert fband_name in list(s["bandpass_filter_settings"]["segment_lengths_ms"].keys()), (
+            assert fband_name in list(
+                s["bandpass_filter_settings"]["segment_lengths_ms"].keys()
+            ), (
                 f"frequency range {fband_name} "
                 "needs to be defined in s['bandpass_filter_settings']['segment_lengths_ms']"
             )
 
     def calc_feature(self, data: np.ndarray, features_compute: dict) -> dict:
-
         data = self.bandpass_filter.filter_data(data)
 
         for (
             ch_idx,
             ch_name,
             f_band,
             f_band_idx,
             seglen,
             bp_feature,
             feature_name,
         ) in self.feature_params:
             if bp_feature == "activity":
                 if self.log_transform:
-                    feature_calc = np.log(
+                    feature_calc = np.log10(
                         np.var(data[ch_idx, f_band_idx, -seglen:])
                     )
                 else:
                     feature_calc = np.var(data[ch_idx, f_band_idx, -seglen:])
             elif bp_feature == "mobility":
                 deriv_variance = np.var(
                     np.diff(data[ch_idx, f_band_idx, -seglen:])
```

### Comparing `py_neuromodulation-0.0.2/py_neuromodulation/nm_plots.py` & `py_neuromodulation-0.0.3/py_neuromodulation/nm_plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 import os
 import numpy as np
 from matplotlib import pyplot as plt
 from matplotlib import gridspec
 from typing import Optional
 import seaborn as sb
 import pandas as pd
+import logging
+
+logger = logging.getLogger("PynmLogger")
 
 from py_neuromodulation import nm_IO, nm_stats
 
 
 def plot_df_subjects(
     df,
     x_col="sub",
@@ -83,15 +86,17 @@
     sfreq: int = 10,
     str_title: str = None,
     str_label: str = None,
     ytick_labelsize: float = None,
 ):
     if z_score is None:
         X_epoch = stats.zscore(
-            np.nan_to_num(np.nanmean(np.squeeze(X_epoch), axis=0)), axis=0
+            np.nan_to_num(np.nanmean(np.squeeze(X_epoch), axis=0)),
+            axis=0,
+            nan_policy="omit",
         ).T
     y_epoch = np.stack(np.array(y_epoch))
     plt.figure(figsize=(6, 6))
     plt.subplot(211)
     plt.imshow(X_epoch, aspect="auto")
     plt.yticks(
         np.arange(0, len(feature_names), 1), feature_names, size=ytick_labelsize
@@ -233,15 +238,15 @@
             # feature_name=feature_names.__str__,  # This here raises an error in os.path.join in line 251
         )
     if save_plot and save_plot_name is not None:
         plt_path = os.path.join(OUT_PATH, save_plot_name)
 
     if save_plot:
         plt.savefig(plt_path, bbox_inches="tight")
-        print("Correlation matrix figure saved to " + str(plt_path))
+        logger.info(f"Correlation matrix figure saved to {plt_path}")
 
     if show_plot is False:
         plt.close()
 
     plt.tight_layout()
 
     return plt.gca()
@@ -325,15 +330,15 @@
                 i[len(ch_name) + 1 :]
                 for i in list(feature_names)
                 if ch_name in i
             ]
 
     if normalize_data:
         X_epoch_mean = stats.zscore(
-            np.nanmean(np.squeeze(X_epoch), axis=0), axis=0
+            np.nanmean(np.squeeze(X_epoch), axis=0), axis=0, nan_policy="omit"
         ).T
     else:
         X_epoch_mean = np.nanmean(np.squeeze(X_epoch), axis=0).T
 
     if len(X_epoch_mean.shape) == 1:
         X_epoch_mean = np.expand_dims(X_epoch_mean, axis=0)
 
@@ -381,15 +386,15 @@
             OUT_PATH,
             feature_file,
             ch_name,
             str_plt_type="MOV_aligned_features",
             feature_name=feature_str_add,
         )
         plt.savefig(plt_path, bbox_inches="tight")
-        print("Feature epoch average figure saved to: " + str(plt_path))
+        logger.info(f"Feature epoch average figure saved to: {str(plt_path)}")
     if show_plot is False:
         plt.close()
 
 
 def plot_grid_elec_3d(
     cortex_grid: np.ndarray | None = None,
     ecog_strip: np.ndarray | None = None,
@@ -437,23 +442,22 @@
     clim_low: float = None,
     clim_high: float = None,
     save: bool = False,
     title="all_feature_plt.pdf",
     OUT_PATH: str = None,
     feature_file: str = None,
 ):
-
     if time_limit_high_s is not None:
         df = df[df["time"] < time_limit_high_s * 1000]
     if time_limit_low_s is not None:
         df = df[df["time"] > time_limit_low_s * 1000]
 
     cols_plt = [c for c in df.columns if c != "time"]
     if normalize is True:
-        data_plt = stats.zscore(df[cols_plt])
+        data_plt = stats.zscore(df[cols_plt], nan_policy="omit")
     else:
         data_plt = df[cols_plt]
 
     plt.figure()  # figsize=(7, 5), dpi=300
     plt.imshow(data_plt.T, aspect="auto")
     plt.xlabel("Time [s]")
     plt.ylabel("Feature Names")
@@ -483,15 +487,14 @@
         self,
         ecog_strip: np.ndarray | None = None,
         grid_cortex: np.ndarray | None = None,
         grid_subcortex: np.ndarray | None = None,
         sess_right: Optional[bool] = False,
         proj_matrix_cortex: np.ndarray | None = None,
     ) -> None:
-
         self.grid_cortex = grid_cortex
         self.grid_subcortex = grid_subcortex
         self.ecog_strip = ecog_strip
         self.sess_right = sess_right
         self.proj_matrix_cortex = proj_matrix_cortex
 
         (
@@ -506,15 +509,14 @@
             self.z_ecog,
             self.x_stn,
             self.y_stn,
             self.z_stn,
         ) = nm_IO.read_plot_modules()
 
     def plot_grid_elec_3d(self) -> None:
-
         plot_grid_elec_3d(np.array(self.grid_cortex), np.array(self.ecog_strip))
 
     def plot_cortex(
         self,
         grid_cortex: Optional[np.ndarray] = None,
         grid_color: Optional[np.ndarray] = None,
         ecog_strip: Optional[np.ndarray] = None,
@@ -548,15 +550,14 @@
             grid_cortex[0, :] = grid_cortex[0, :] * -1
 
         fig, axes = plt.subplots(1, 1, facecolor=(1, 1, 1), figsize=(14, 9))
         axes.scatter(self.x_ecog, self.y_ecog, c="gray", s=0.01)
         axes.axes.set_aspect("equal", anchor="C")
 
         if grid_cortex is not None:
-
             grid_color = (
                 np.ones(grid_cortex.shape[0])
                 if grid_color is None
                 else grid_color
             )
 
             pos_ecog = axes.scatter(
@@ -600,10 +601,12 @@
                 OUT_PATH,
                 feature_file,
                 ch_name=None,
                 str_plt_type="PLOT_CORTEX",
                 feature_name=feature_str_add,
             )
             plt.savefig(plt_path, bbox_inches="tight")
-            print("Feature epoch average figure saved to: " + str(plt_path))
+            logger.info(
+                f"Feature epoch average figure saved to: {str(plt_path)}"
+            )
         if show_plot is False:
             plt.close()
```

### Comparing `py_neuromodulation-0.0.2/py_neuromodulation/nm_projection.py` & `py_neuromodulation-0.0.3/py_neuromodulation/nm_projection.py`

 * *Files identical despite different names*

### Comparing `py_neuromodulation-0.0.2/py_neuromodulation/nm_rereference.py` & `py_neuromodulation-0.0.3/py_neuromodulation/nm_rereference.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 """Re-referencing Module."""
 import numpy as np
 import pandas as pd
 
 
 class ReReferencer:
-
     ref_matrix: np.ndarray
 
-
     def __init__(
         self,
         sfreq: int | float,
         nm_channels: pd.DataFrame,
     ) -> None:
         """Initialize real-time rereference information.
 
@@ -24,19 +22,23 @@
             specified in nm_channels.csv.
 
 
         Raises:
             ValueError: rereferencing using undefined channel
             ValueError: rereferencing to same channel
         """
-        (channels_used,) = np.where((nm_channels.used == 1))
+        nm_channels = nm_channels[nm_channels["used"] == 1].reset_index(
+            drop=True
+        )
+        # (channels_used,) = np.where((nm_channels.used == 1))
 
         ch_names = nm_channels["name"].tolist()
 
-        if len(ch_names) == 1:
+        # no re-referencing is being performed when there is a single channel present only
+        if nm_channels.shape[0] in (0, 1):
             self.ref_matrix = None
             return
 
         ch_types = nm_channels["type"]
         refs = nm_channels["rereference"]
 
         type_map = {}
@@ -44,16 +46,16 @@
             type_map[ch_type] = np.where(
                 (ch_types == ch_type) & (nm_channels["status"] == "good")
             )[0]
 
         ref_matrix = np.zeros((len(nm_channels), len(nm_channels)))
         for ind in range(len(nm_channels)):
             ref_matrix[ind, ind] = 1
-            if ind not in channels_used:
-                continue
+            # if ind not in channels_used:
+            #    continue
             ref = refs[ind]
             if ref.lower() == "none" or pd.isnull(ref):
                 ref_idx = None
                 continue
             if ref.lower() == "average":
                 ch_type = ch_types[ind]
                 ref_idx = type_map[ch_type][type_map[ch_type] != ind]
@@ -80,14 +82,14 @@
         """Rereference data according to the initialized ReReferencer class.
 
         Args:
             data (numpy ndarray) :
                 shape(n_channels, n_samples) - data to be rereferenced.
 
         Returns:
-            reref_data (numpy ndarray): 
+            reref_data (numpy ndarray):
             shape(n_channels, n_samples) - rereferenced data
         """
         if self.ref_matrix is not None:
             return self.ref_matrix @ data
         else:
-            return data
+            return data
```

### Comparing `py_neuromodulation-0.0.2/py_neuromodulation/nm_resample.py` & `py_neuromodulation-0.0.3/py_neuromodulation/nm_resample.py`

 * *Files identical despite different names*

### Comparing `py_neuromodulation-0.0.2/py_neuromodulation/nm_run_analysis.py` & `py_neuromodulation-0.0.3/py_neuromodulation/nm_run_analysis.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 """This module contains the class to process a given batch of data."""
+
 from enum import Enum
 import math
 import os
 from time import time
 from typing import Protocol, Type
+import logging
+
+logger = logging.getLogger("PynmLogger")
 
 import numpy as np
 import pandas as pd
 
 from py_neuromodulation import (
     nm_features,
     nm_filter,
     nm_IO,
     nm_normalization,
     nm_projection,
     nm_rereference,
     nm_resample,
+    nm_filter_preprocessing,
 )
 
 _PathLike = str | os.PathLike
 
 
 class Preprocessor(Protocol):
     def process(self, data: np.ndarray) -> np.ndarray:
         pass
 
-    def test_settings(self, settings: dict):
-        ...
+    def test_settings(self, settings: dict): ...
 
 
 _PREPROCESSING_CONSTRUCTORS = [
     "notch_filter",
     "re_referencing",
     "raw_normalization",
     "raw_resample",
@@ -69,15 +73,15 @@
         projection : projection.py object
             projection object (needs to be initialized beforehand), by default None
         resample : resample.py object
             Resample object (needs to be initialized beforehand), by default None
         notch_filter : nm_filter.NotchFilter,
             Notch Filter object, needs to be instantiated beforehand
         verbose : boolean
-            if True, print out signal processed and computation time
+            if True, log signal processed and computation time
         """
         self.settings = self._load_settings(settings)
         self.nm_channels = self._load_nm_channels(nm_channels)
 
         self.sfreq_features = self.settings["sampling_rate_features_hz"]
         self._sfreq_raw_orig = sfreq
         self.sfreq_raw = math.floor(sfreq)
@@ -115,14 +119,20 @@
                 case "raw_normalization":
                     preprocessor = nm_normalization.RawNormalizer(
                         sfreq=self.sfreq_raw,
                         sampling_rate_features_hz=self.sfreq_features,
                         **self.settings.get(settings_str, {}),
                     )
                     self.preprocessors.append(preprocessor)
+                case "preprocessing_filter":
+                    preprocessor = nm_filter_preprocessing.PreprocessingFilter(
+                        settings=self.settings,
+                        sfreq=self.sfreq_raw,
+                    )
+                    self.preprocessors.append(preprocessor)
                 case _:
                     raise ValueError(
                         "Invalid preprocessing method. Must be one of"
                         f" {_PREPROCESSING_CONSTRUCTORS}. Got"
                         f" {preprocessing_method}"
                     )
 
@@ -327,26 +337,31 @@
         pandas Series
             Features calculated from current data
         """
         start_time = time()
 
         nan_channels = np.isnan(data).any(axis=1)
 
-        data = np.nan_to_num(data)  # [self.feature_idx, :]needs to be before preprocessing
+        data = np.nan_to_num(data)[self.feature_idx, :]
 
         for processor in self.preprocessors:
             data = processor.process(data)
 
         # calculate features
         features_dict = self.features.estimate_features(data)
 
         # normalize features
         if self.settings["postprocessing"]["feature_normalization"]:
-            normed_features = self.feature_normalizer.process(np.fromiter(features_dict.values(), dtype="float"))
-            features_dict = {key: normed_features[idx] for idx, key in enumerate(features_dict.keys())}
+            normed_features = self.feature_normalizer.process(
+                np.fromiter(features_dict.values(), dtype="float")
+            )
+            features_dict = {
+                key: normed_features[idx]
+                for idx, key in enumerate(features_dict.keys())
+            }
 
         features_current = pd.Series(
             data=list(features_dict.values()),
             index=list(features_dict.keys()),
             dtype=np.float64,
         )
 
@@ -360,15 +375,15 @@
         if nan_channels.sum() > 0:
             for ch in list(np.array(self.ch_names_used)[nan_channels]):
                 features_current.loc[
                     features_current.index.str.contains(ch)
                 ] = np.nan
 
         if self.verbose is True:
-            print(
+            logger.info(
                 "Last batch took: "
                 + str(np.round(time() - start_time, 2))
                 + " seconds"
             )
 
         return features_current
 
@@ -386,22 +401,22 @@
             "final_fs": self.sfreq_raw,
             "sfreq": self.sfreq_features,
         }
         if self.projection:
             sidecar["coords"] = self.projection.coords
             if self.settings["postprocessing"]["project_cortex"]:
                 sidecar["grid_cortex"] = self.projection.grid_cortex
-                sidecar[
-                    "proj_matrix_cortex"
-                ] = self.projection.proj_matrix_cortex
+                sidecar["proj_matrix_cortex"] = (
+                    self.projection.proj_matrix_cortex
+                )
             if self.settings["postprocessing"]["project_subcortex"]:
                 sidecar["grid_subcortex"] = self.projection.grid_subcortex
-                sidecar[
-                    "proj_matrix_subcortex"
-                ] = self.projection.proj_matrix_subcortex
+                sidecar["proj_matrix_subcortex"] = (
+                    self.projection.proj_matrix_subcortex
+                )
         if additional_args is not None:
             sidecar = sidecar | additional_args
 
         nm_IO.save_sidecar(sidecar, out_path_root, folder_name)
 
     def save_settings(self, out_path_root: _PathLike, folder_name: str) -> None:
         nm_IO.save_settings(self.settings, out_path_root, folder_name)
```

### Comparing `py_neuromodulation-0.0.2/py_neuromodulation/nm_settings.py` & `py_neuromodulation-0.0.3/py_neuromodulation/nm_settings.py`

 * *Files identical despite different names*

### Comparing `py_neuromodulation-0.0.2/py_neuromodulation/nm_sharpwaves.py` & `py_neuromodulation-0.0.3/py_neuromodulation/nm_sharpwaves.py`

 * *Files 10% similar despite different names*

```diff
@@ -101,31 +101,20 @@
         -------
         peak_left_idx (np.ndarray): index of left peak
         peak_right_idx (np.ndarray): index of right peak
         peak_left_val (np.ndarray): value of left peak
         peak_right_val (np.ndarray): value of righ peak
         """
 
-        ind_greater = np.where(arr_ind_peaks > trough_ind)[0]
-        if ind_greater.shape[0] == 0:
-            raise NoValidTroughException("No valid trough")
-        val_ind_greater = arr_ind_peaks[ind_greater]
-        peak_right_idx = arr_ind_peaks[
-            ind_greater[np.argsort(val_ind_greater)[0]]
-        ]
-
-        ind_smaller = np.where(arr_ind_peaks < trough_ind)[0]
-        if ind_smaller.shape[0] == 0:
-            raise NoValidTroughException("No valid trough")
-
-        val_ind_smaller = arr_ind_peaks[ind_smaller]
-        peak_left_idx = arr_ind_peaks[
-            ind_smaller[np.argsort(val_ind_smaller)[-1]]
-        ]
+        try: peak_right_idx = arr_ind_peaks[arr_ind_peaks > trough_ind][0]
+        except IndexError: raise NoValidTroughException("No valid trough")
 
+        try: peak_left_idx  = arr_ind_peaks[arr_ind_peaks < trough_ind][-1]
+        except IndexError: raise NoValidTroughException("No valid trough")
+       
         return (
             peak_left_idx,
             peak_right_idx,
             filtered_dat[peak_left_idx],
             filtered_dat[peak_right_idx],
         )
 
@@ -146,20 +135,18 @@
 
         Returns
         -------
         features_compute (dict): set features for Features.py object
         """
         for ch_idx, ch_name in enumerate(self.ch_names):
             for filter_name, filter in self.list_filter:
-                if filter_name == "no_filter":
-                    self.data_process_sw = data[ch_idx, :]
-                else:
-                    self.data_process_sw = signal.convolve(
-                        data[ch_idx, :], filter, mode="same"
-                    )
+                self.data_process_sw = (data[ch_idx, :] 
+                    if filter_name == "no_filter" 
+                    else signal.fftconvolve(data[ch_idx, :], filter, mode="same")
+                )
 
                 # check settings if troughs and peaks are analyzed
 
                 dict_ch_features = {}
 
                 for detect_troughs in [False, True]:
 
@@ -263,131 +250,111 @@
             distance=self.sw_settings["detect_troughs"]["distance_peaks_ms"],
         )[0]
         troughs = signal.find_peaks(
             -self.data_process_sw,
             distance=self.sw_settings["detect_troughs"]["distance_troughs_ms"],
         )[0]
 
-        for trough_idx in troughs:
-            try:
-                (
-                    peak_idx_left,
-                    peak_idx_right,
-                    peak_left,
-                    peak_right,
-                ) = self._get_peaks_around(
-                    trough_idx, peaks, self.data_process_sw
-                )
-            except NoValidTroughException:
-                # in this case there are no adjacent two peaks around this trough
-                # str(e) could print the exception error message
-                # print(str(e))
+        """ Find left and right peak indexes for each trough """
+        peak_pointer = 0
+        peak_idx_left = []
+        peak_idx_right = []
+        first_valid = last_valid = 0
+
+        for i, trough_idx in enumerate(troughs):
+            
+            # Locate peak right of current trough
+            while peak_pointer < peaks.size and peaks[peak_pointer] < trough_idx:
+                peak_pointer += 1
+
+            if peak_pointer - 1 < 0: 
+                # If trough has no peak to it's left, it's not valid 
+                first_valid = i + 1 # Try with next one
                 continue
 
-            trough = self.data_process_sw[trough_idx]
-            self.trough.append(trough)
-            self.troughs_idx.append(trough_idx)
-
-            if self.sw_settings["sharpwave_features"]["interval"] is True:
-                if len(self.troughs_idx) > 1:
-                    # take the last identified trough idx
-                    # corresponds here to second last trough_idx
-
-                    interval = (trough_idx - self.troughs_idx[-2]) * (
-                        1000 / self.sfreq
-                    )
-                else:
-                    # set first interval to zero
-                    interval = 0
-                self.interval.append(interval)
-
-            if self.sw_settings["sharpwave_features"]["peak_left"] is True:
-                self.peak_left.append(peak_left)
-
-            if self.sw_settings["sharpwave_features"]["peak_right"] is True:
-                self.peak_right.append(peak_right)
-
-            if self.sw_settings["sharpwave_features"]["sharpness"] is True:
-                # check if sharpness can be calculated
-                # trough_idx 5 ms need to be consistent
-                if (trough_idx - int(5 * (1000 / self.sfreq)) <= 0) or (
-                    trough_idx + int(5 * (1000 / self.sfreq))
-                    >= self.data_process_sw.shape[0]
-                ):
-                    continue
-
-                sharpness = (
-                    (
-                        self.data_process_sw[trough_idx]
-                        - self.data_process_sw[
-                            trough_idx - int(5 * (1000 / self.sfreq))
-                        ]
-                    )
-                    + (
-                        self.data_process_sw[trough_idx]
-                        - self.data_process_sw[
-                            trough_idx + int(5 * (1000 / self.sfreq))
-                        ]
-                    )
-                ) / 2
-
-                self.sharpness.append(sharpness)
-
-            if self.sw_settings["sharpwave_features"]["rise_steepness"] is True:
-                # steepness is calculated as the first derivative
-                # from peak/trough to trough/peak
-                # here  + 1 due to python syntax, s.t. the last element is included
-                rise_steepness = np.max(
-                    np.diff(
-                        self.data_process_sw[peak_idx_left : trough_idx + 1]
-                    )
-                )
-                self.rise_steepness.append(rise_steepness)
-
-            if (
-                self.sw_settings["sharpwave_features"]["decay_steepness"]
-                is True
-            ):
-                decay_steepness = np.max(
-                    np.diff(
-                        self.data_process_sw[trough_idx : peak_idx_right + 1]
-                    )
-                )
-                self.decay_steepness.append(decay_steepness)
-
-            if (
-                self.sw_settings["sharpwave_features"]["rise_steepness"] is True
-                and self.sw_settings["sharpwave_features"]["decay_steepness"]
-                is True
-                and self.sw_settings["sharpwave_features"]["slope_ratio"]
-                is True
-            ):
-                self.slope_ratio.append(rise_steepness - decay_steepness)
-
-            if self.sw_settings["sharpwave_features"]["prominence"] is True:
-                self.prominence.append(
-                    np.abs(
-                        (peak_right + peak_left) / 2
-                        - self.data_process_sw[trough_idx]
-                    )
-                )
-
-            if self.sw_settings["sharpwave_features"]["decay_time"] is True:
-                self.decay_time.append(
-                    (peak_idx_left - trough_idx) * (1000 / self.sfreq)
-                )  # ms
-
-            if self.sw_settings["sharpwave_features"]["rise_time"] is True:
-                self.rise_time.append(
-                    (peak_idx_right - trough_idx) * (1000 / self.sfreq)
-                )  # ms
-
-            if self.sw_settings["sharpwave_features"]["width"] is True:
-                self.width.append(peak_idx_right - peak_idx_left)  # ms
+            if peak_pointer == peaks.size:
+                # If we went past the end of the peaks list, trough had no peak to its right
+                continue
 
+            last_valid = i
+            peak_idx_left.append(peaks[peak_pointer - 1])
+            peak_idx_right.append(peaks[peak_pointer])
+
+        troughs = troughs[first_valid:last_valid + 1] # Remove non valid troughs
+        
+        peak_idx_left = np.array(peak_idx_left, dtype=np.integer)
+        peak_idx_right = np.array(peak_idx_right, dtype=np.integer)
+
+        peak_left = self.data_process_sw[peak_idx_left]
+        peak_right = self.data_process_sw[peak_idx_right]
+        trough_values = self.data_process_sw[troughs]
+
+        # No need to store trough data as it is not used anywhere else in the program
+        # self.trough.append(trough)
+        # self.troughs_idx.append(trough_idx)
+         
+        """ Calculate features (vectorized) """
+        
+        if self.sw_settings["sharpwave_features"]["interval"]:
+            self.interval = np.concatenate(([0], np.diff(troughs))) * (1000 / self.sfreq)
+
+        if self.sw_settings["sharpwave_features"]["peak_left"]:
+            self.peak_left = peak_left
+
+        if self.sw_settings["sharpwave_features"]["peak_right"]:
+            self.peak_right = peak_right
+
+        if self.sw_settings["sharpwave_features"]["sharpness"]:
+            # sharpess is calculated on a +- 5 ms window
+            # valid troughs need 5 ms of margin on both siddes
+            troughs_valid = troughs[np.logical_and(
+                                troughs - int(5 * (1000 / self.sfreq)) > 0, 
+                                troughs + int(5 * (1000 / self.sfreq)) < self.data_process_sw.shape[0])]
+
+            self.sharpness = (
+                        (self.data_process_sw[troughs_valid] - self.data_process_sw[troughs_valid - int(5 * (1000 / self.sfreq))]) +
+                        (self.data_process_sw[troughs_valid] - self.data_process_sw[troughs_valid + int(5 * (1000 / self.sfreq))])
+                        ) / 2
+
+        if (self.sw_settings["sharpwave_features"]["rise_steepness"] or
+            self.sw_settings["sharpwave_features"]["decay_steepness"]):
+            
+            # steepness is calculated as the first derivative
+            steepness = np.concatenate(([0],np.diff(self.data_process_sw)))
+
+            if self.sw_settings["sharpwave_features"]["rise_steepness"]: # left peak -> trough
+                # + 1 due to python syntax, s.t. the last element is included
+                self.rise_steepness = np.array([
+                    np.max(np.abs(steepness[peak_idx_left[i] : troughs[i] + 1]))
+                    for i in range(trough_idx.size)
+                ])
+                
+            if self.sw_settings["sharpwave_features"]["decay_steepness"]: # trough -> right peak
+                self.decay_steepness = np.array([
+                    np.max(np.abs(steepness[troughs[i] : peak_idx_right[i] + 1]))
+                    for i in range(trough_idx.size)
+                ])
+
+            if (self.sw_settings["sharpwave_features"]["rise_steepness"] and
+                self.sw_settings["sharpwave_features"]["decay_steepness"] and
+                self.sw_settings["sharpwave_features"]["slope_ratio"]):
+                self.slope_ratio = self.rise_steepness - self.decay_steepness
+
+        if self.sw_settings["sharpwave_features"]["prominence"]:
+            self.prominence = np.abs((peak_right + peak_left) / 2 - trough_values)
+
+        if self.sw_settings["sharpwave_features"]["decay_time"]:
+            self.decay_time = (peak_idx_left - troughs) * (1000 / self.sfreq) # ms
+
+        if self.sw_settings["sharpwave_features"]["rise_time"]:
+            self.rise_time = (peak_idx_right - troughs) * (1000 / self.sfreq) # ms
+
+        if self.sw_settings["sharpwave_features"]["width"]:
+            self.width = peak_idx_right - peak_idx_left  # ms
+    
     @staticmethod
     def test_settings(
         s: dict,
         ch_names: Iterable[str],
         sfreq: int | float,
     ):
         for filter_range in s["sharpwave_analysis_settings"][
```

### Comparing `py_neuromodulation-0.0.2/py_neuromodulation/nm_stats.py` & `py_neuromodulation-0.0.3/py_neuromodulation/nm_stats.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import random
 import copy
 
 import matplotlib.pyplot as plt
+
 # from numba import njit
 import numpy as np
 import pandas as pd
 import scipy.stats as stats
 
 
 from skimage import measure
@@ -29,15 +30,15 @@
     for i, (train, test) in enumerate(kfold.split(x, y)):
         model.fit(x.iloc[train, :], y.iloc[train, :])
         score = model.score(x.iloc[test, :], y.iloc[test, :])
         # mdl = fitlm(np.squeeze(y.iloc[test,:].transpose()), np.squeeze(model.predict(x.iloc[test, :])))
         scores.append(score)
         coeffs = np.vstack((coeffs, model.coef_))
     coeffs = list(np.delete(coeffs, 0))
-    return scores, coeffs, model, ['scores', 'coeffs', 'model']
+    return scores, coeffs, model, ["scores", "coeffs", "model"]
 
 
 def zscore(data):
     return (data - data.mean()) / data.std()
 
 
 def permutationTestSpearmansRho(x, y, plot_distr=True, x_unit=None, p=5000):
@@ -72,22 +73,22 @@
         random.shuffle(args_order_2)
         # Compute permuted absolute difference of your two sampled
         # distributions and store it in pD:
         pD.append(stats.spearmanr(pV[0, args_order], pV[1, args_order_2])[0])
 
     # calculate p value
     if gT < 0:
-        p_val = len(np.where(pD <= gT)[0])/p
+        p_val = len(np.where(pD <= gT)[0]) / p
     else:
-        p_val = len(np.where(pD >= gT)[0])/p
+        p_val = len(np.where(pD >= gT)[0]) / p
 
     if plot_distr is True:
         plt.hist(pD, bins=30, label="permutation results")
         plt.axvline(gT, color="orange", label="ground truth")
-        plt.title("ground truth " + x_unit + "="+str(gT) + " p=" + str(p_val))
+        plt.title("ground truth " + x_unit + "=" + str(gT) + " p=" + str(p_val))
         plt.xlabel(x_unit)
         plt.legend()
         plt.show()
     return gT, p_val
 
 
 def permutationTest(x, y, plot_distr=True, x_unit=None, p=5000):
@@ -116,27 +117,31 @@
     pD = []
     # Permutation loop:
     for i in range(0, p):
         # Shuffle the data:
         random.shuffle(pS)
         # Compute permuted absolute difference of your two sampled
         # distributions and store it in pD:
-        pD.append(np.abs(np.average(pS[0:int(len(pS)/2)]) - np.average(
-            pS[int(len(pS)/2):])))
+        pD.append(
+            np.abs(
+                np.average(pS[0 : int(len(pS) / 2)])
+                - np.average(pS[int(len(pS) / 2) :])
+            )
+        )
 
     # Calculate p-value
     if gT < 0:
-        p_val = len(np.where(pD <= gT)[0])/p
+        p_val = len(np.where(pD <= gT)[0]) / p
     else:
-        p_val = len(np.where(pD >= gT)[0])/p
+        p_val = len(np.where(pD >= gT)[0]) / p
 
     if plot_distr is True:
         plt.hist(pD, bins=30, label="permutation results")
         plt.axvline(gT, color="orange", label="ground truth")
-        plt.title("ground truth "+x_unit+"="+str(gT)+" p="+str(p_val))
+        plt.title("ground truth " + x_unit + "=" + str(gT) + " p=" + str(p_val))
         plt.xlabel(x_unit)
         plt.legend()
         plt.show()
     return gT, p_val
 
 
 def permutationTest_relative(x, y, plot_distr=True, x_unit=None, p=5000):
@@ -161,25 +166,28 @@
     for i in range(0, p):
         l_ = []
         for i in range(x.shape[0]):
             if random.randint(0, 1) == 1:
                 l_.append((x[i], y[i]))
             else:
                 l_.append((y[i], x[i]))
-        pD.append(np.abs(np.average(np.array(l_)[:, 0]) - np.average(
-            np.array(l_)[:, 1])))
+        pD.append(
+            np.abs(
+                np.average(np.array(l_)[:, 0]) - np.average(np.array(l_)[:, 1])
+            )
+        )
     if gT < 0:
-        p_val = len(np.where(pD <= gT)[0])/p
+        p_val = len(np.where(pD <= gT)[0]) / p
     else:
-        p_val = len(np.where(pD >= gT)[0])/p
+        p_val = len(np.where(pD >= gT)[0]) / p
 
     if plot_distr is True:
         plt.hist(pD, bins=30, label="permutation results")
         plt.axvline(gT, color="orange", label="ground truth")
-        plt.title("ground truth "+x_unit+"="+str(gT)+" p="+str(p_val))
+        plt.title("ground truth " + x_unit + "=" + str(gT) + " p=" + str(p_val))
         plt.xlabel(x_unit)
         plt.legend()
         plt.show()
 
     return gT, p_val
 
 
@@ -207,30 +215,31 @@
     float
         Estimated difference of distribution from baseline
     float
         P-value of permutation test
     """
     if two_tailed is True:
         zeroed = x - y
-        print(zeroed)
         z = np.abs(np.mean(zeroed))
         p = np.empty(n_perm)
         # Run the simulation n_perm times
         for i in np.arange(n_perm):
             sign = np.random.choice(
-                a=np.array([-1., 1.]), size=len(x), replace=True)
+                a=np.array([-1.0, 1.0]), size=len(x), replace=True
+            )
             p[i] = np.abs(np.mean(zeroed * sign))
     else:
         zeroed = x - y
         z = np.mean(zeroed)
         p = np.empty(n_perm)
         # Run the simulation n_perm times
         for i in np.arange(n_perm):
             sign = np.random.choice(
-                a=np.array([-1., 1.]), size=len(x), replace=True)
+                a=np.array([-1.0, 1.0]), size=len(x), replace=True
+            )
             p[i] = np.mean(zeroed * sign)
         # Return p-value
     return z, (np.sum(p >= z)) / n_perm
 
 
 # @njit
 def permutation_numba_twosample(x, y, n_perm, two_tailed=True):
@@ -307,40 +316,44 @@
     # loop through clusters of p_val series or image
     index_cluster = {}
     p_cluster_sum = np.zeros(num_clusters)
     for cluster_i in np.arange(num_clusters):
         # first cluster is assigned to be 1 from measure.label
         index_cluster[cluster_i] = np.where(labels == cluster_i + 1)[0]
         p_cluster_sum[cluster_i] = np.sum(
-            np.array(1 - p_arr)[index_cluster[cluster_i]])
+            np.array(1 - p_arr)[index_cluster[cluster_i]]
+        )
     # p_min corresponds to the most unlikely cluster
     p_min = np.max(p_cluster_sum)
 
     p_min_index = index_cluster[np.argmax(p_cluster_sum)]
 
     # loop through random permutation cycles
     r_per_arr = np.zeros(num_permutations)
     for r in range(num_permutations):
-        r_per = np.random.randint(low=0, high=p_arr.shape[0],
-                                  size=p_arr.shape[0])
-
-        labels, num_clusters = measure.label(p_arr[r_per] <= p_sig,
-                                             return_num=True)
+        r_per = np.random.randint(
+            low=0, high=p_arr.shape[0], size=p_arr.shape[0]
+        )
+
+        labels, num_clusters = measure.label(
+            p_arr[r_per] <= p_sig, return_num=True
+        )
 
         index_cluster = {}
         if num_clusters == 0:
             r_per_arr[r] = 0
         else:
             p_cluster_sum = np.zeros(num_clusters)
             for cluster_i in np.arange(num_clusters):
-                index_cluster[cluster_i] = np.where(
-                    labels == cluster_i + 1)[
-                    0]  # first cluster is assigned to be 1 from measure.label
+                index_cluster[cluster_i] = np.where(labels == cluster_i + 1)[
+                    0
+                ]  # first cluster is assigned to be 1 from measure.label
                 p_cluster_sum[cluster_i] = np.sum(
-                    np.array(1 - p_arr[r_per])[index_cluster[cluster_i]])
+                    np.array(1 - p_arr[r_per])[index_cluster[cluster_i]]
+                )
             # corresponds to the most unlikely cluster
             r_per_arr[r] = np.max(p_cluster_sum)
 
     sorted_r = np.sort(r_per_arr)
 
     def find_arg_nearest(array, value):
         array = np.asarray(array)
@@ -428,27 +441,28 @@
         r_per_arr : numpy array
             Null distribution of shape (n_perm_)
         """
         # loop through random permutation cycles
         r_per_arr = np.zeros(n_perm_)
         for r in range(n_perm_):
             r_per = np.random.randint(
-                low=0, high=p_arr_.shape[0], size=p_arr_.shape[0])
+                low=0, high=p_arr_.shape[0], size=p_arr_.shape[0]
+            )
             labels_, n_clusters = cluster(p_arr_[r_per] <= p_sig_)
 
             cluster_ind = {}
             if n_clusters == 0:
                 r_per_arr[r] = 0
             else:
                 p_sum = np.zeros(n_clusters)
                 for ind in range(n_clusters):
-                    cluster_ind[ind] = \
-                        np.where(labels_ == ind + 1)[0]
+                    cluster_ind[ind] = np.where(labels_ == ind + 1)[0]
                     p_sum[ind] = np.sum(
-                        np.asarray(1 - p_arr_[r_per])[cluster_ind[ind]])
+                        np.asarray(1 - p_arr_[r_per])[cluster_ind[ind]]
+                    )
                 r_per_arr[r] = np.max(p_sum)
         return r_per_arr
 
     labels, num_clusters = cluster(p_arr <= p_sig)
 
     null_distr = calculate_null_distribution(p_arr, p_sig, n_perm)
     # Loop through clusters of p_val series or image
```

### Comparing `py_neuromodulation-0.0.2/py_neuromodulation/nm_stream_abc.py` & `py_neuromodulation-0.0.3/py_neuromodulation/nm_stream_abc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 """Module that contains PNStream ABC."""
+
 from abc import ABC, abstractmethod
 import os
 import pathlib
 import _pickle as cPickle
 
+from .utils import _logging  # logger initialization
+
+# Logger use in different modules: logger = logging.getLogger("PynmLogger")
+
+
 import pandas as pd
 from sklearn import base
 
 from py_neuromodulation import (
     nm_features,
     nm_IO,
     nm_plots,
     nm_run_analysis,
-    nm_settings
+    nm_settings,
 )
 
 _PathLike = str | os.PathLike
 
 
 class PNStream(ABC):
 
@@ -68,15 +74,17 @@
             coordinates in the form [[coord_1_x, coord_1_y, coord_1_z], [coord_2_x, coord_2_y, coord_2_z],], by default None
         verbose : bool, optional
             print out stream computation time information, by default True
         """
         self.settings = self._load_settings(settings)
 
         if sampling_rate_features_hz is not None:
-            self.settings["sampling_rate_features_hz"] = sampling_rate_features_hz
+            self.settings["sampling_rate_features_hz"] = (
+                sampling_rate_features_hz
+            )
 
         self.nm_channels = self._load_nm_channels(nm_channels)
         if path_grids is None:
             path_grids = pathlib.Path(__file__).parent.resolve()
         self.path_grids = path_grids
         self.verbose = verbose
         self.sfreq = sfreq
@@ -134,26 +142,28 @@
         )
 
     @staticmethod
     def _load_nm_channels(
         nm_channels: pd.DataFrame | _PathLike,
     ) -> pd.DataFrame:
         if not isinstance(nm_channels, pd.DataFrame):
-            nm_channels =  nm_IO.load_nm_channels(nm_channels)
-        
-        if nm_channels.query("used == 1 and target == 0").shape[0]  == 0:
-            raise ValueError("No channels selected for analysis that have column 'used' = 1 and 'target' = 0. Please check your nm_channels")
+            nm_channels = nm_IO.load_nm_channels(nm_channels)
+
+        if nm_channels.query("used == 1 and target == 0").shape[0] == 0:
+            raise ValueError(
+                "No channels selected for analysis that have column 'used' = 1 and 'target' = 0. Please check your nm_channels"
+            )
 
         return nm_channels
 
     @staticmethod
     def _load_settings(settings: dict | _PathLike | None) -> dict:
         if isinstance(settings, dict):
             return settings
-        if settings is None: 
+        if settings is None:
             return nm_settings.get_default_settings()
         return nm_IO.read_settings(str(settings))
 
     def load_model(self, model_name: _PathLike) -> None:
         """Load sklearn model, that utilizes predict"""
         with open(model_name, "rb") as fid:
             self.model = cPickle.load(fid)
@@ -192,17 +202,15 @@
         nm_IO.save_features(feature_arr, out_path_root, folder_name)
 
     def save_nm_channels(
         self, out_path_root: _PathLike, folder_name: str
     ) -> None:
         self.run_analysis.save_nm_channels(out_path_root, folder_name)
 
-    def save_settings(
-        self, out_path_root: _PathLike, folder_name: str
-    ) -> None:
+    def save_settings(self, out_path_root: _PathLike, folder_name: str) -> None:
         self.run_analysis.save_settings(out_path_root, folder_name)
 
     def save_sidecar(self, out_path_root: _PathLike, folder_name: str) -> None:
         """Save sidecar incduing fs, coords, sess_right to
         out_path_root and subfolder 'folder_name'"""
         additional_args = {"sess_right": self.sess_right}
         self.run_analysis.save_sidecar(
```

