# Comparing `tmp/Simba-UW-tf-dev-1.89.7.tar.gz` & `tmp/Simba-UW-tf-dev-1.89.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Simba-UW-tf-dev-1.89.7.tar", last modified: Fri Apr 12 00:28:53 2024, max compression
+gzip compressed data, was "dist/Simba-UW-tf-dev-1.89.8.tar", last modified: Fri Apr 12 20:23:20 2024, max compression
```

## Comparing `Simba-UW-tf-dev-1.89.7.tar` & `Simba-UW-tf-dev-1.89.8.tar`

### file list

```diff
@@ -1,637 +1,639 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 00:28:53.000000 Simba-UW-tf-dev-1.89.7/
--rw-r--r--   0 simon      (501) staff       (20)     2797 2024-04-12 00:28:53.000000 Simba-UW-tf-dev-1.89.7/PKG-INFO
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 00:28:53.000000 Simba-UW-tf-dev-1.89.7/simba/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 00:28:53.000000 Simba-UW-tf-dev-1.89.7/simba/ui/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-28 13:50:53.000000 Simba-UW-tf-dev-1.89.7/simba/ui/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 00:28:53.000000 Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/
--rw-r--r--   0 simon      (501) staff       (20)    11467 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/mutual_exclusivity_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4070 2024-03-29 20:30:28.000000 Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1676 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/csv_2_parquet_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2566 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/quick_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2873 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/batch_preprocess_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8835 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/heatmap_location_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9734 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/clf_probability_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3456 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/movement_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4631 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    11362 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/clf_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    24905 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1184 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/remove_roi_features_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6692 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/targeted_annotation_clips_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3340 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2174 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/roi_size_standardizer_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     6997 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5068 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/roi_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7898 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/outlier_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9048 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/gantt_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6293 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/clf_validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8529 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/severity_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3221 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/fsttc_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4231 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/kleinberg_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7979 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9785 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/spontaneous_alternation_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6076 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/pose_reorganizer_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3437 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/animal_directing_other_animals_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3402 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3468 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/clf_by_timebins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9153 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/heatmap_clf_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9235 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/data_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    11785 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/roi_features_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9118 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/pup_retrieval_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5577 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/boolean_conditional_slicer_pup_up.py
--rw-r--r--   0 simon      (501) staff       (20)      584 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/about_simba_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5451 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    10747 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1795 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7312 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/directing_animal_to_bodypart_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6546 2024-02-16 01:12:37.000000 Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    66309 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/video_processing_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7800 2024-04-04 16:47:32.000000 Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6160 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/clf_by_roi_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2741 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/make_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3622 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/direction_animal_to_bodypart_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6166 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1072 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/archive_files_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4716 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/pose_bp_drop_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    12174 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/distance_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4673 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3290 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4134 2024-03-31 17:07:13.000000 Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    16701 2024-02-08 00:53:55.000000 Simba-UW-tf-dev-1.89.7/simba/ui/video_info_ui.py
--rw-r--r--   0 simon      (501) staff       (20)     6573 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.89.7/simba/ui/user_defined_pose_creator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/ui/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    14374 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.89.7/simba/ui/create_project_ui.py
--rw-r--r--   0 simon      (501) staff       (20)    14487 2024-02-08 00:53:55.000000 Simba-UW-tf-dev-1.89.7/simba/ui/tkinter_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    38870 2024-04-04 16:45:40.000000 Simba-UW-tf-dev-1.89.7/simba/ui/machine_model_settings_ui.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 00:28:53.000000 Simba-UW-tf-dev-1.89.7/simba/labelling/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/labelling/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    24423 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/labelling/labelling_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     2362 2024-02-21 02:33:04.000000 Simba-UW-tf-dev-1.89.7/simba/labelling/targeted_annotations_clips.py
--rw-r--r--   0 simon      (501) staff       (20)     3974 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/labelling/extract_labelled_frames.py
--rw-r--r--   0 simon      (501) staff       (20)    31269 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/labelling/labelling_advanced_interface.py
--rw-r--r--   0 simon      (501) staff       (20)    10012 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/labelling/play_annotation_video.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 00:28:53.000000 Simba-UW-tf-dev-1.89.7/simba/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)    15004 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.89.7/simba/unsupervised/dbcv_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5077 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.89.7/simba/unsupervised/cluster_validation_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3645 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.89.7/simba/unsupervised/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-03 14:33:55.000000 Simba-UW-tf-dev-1.89.7/simba/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     9036 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.89.7/simba/unsupervised/cluster_video_visualizer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 00:28:53.000000 Simba-UW-tf-dev-1.89.7/simba/unsupervised/pop_ups/
--rw-r--r--   0 simon      (501) staff       (20)     4642 2024-03-26 23:50:53.000000 Simba-UW-tf-dev-1.89.7/simba/unsupervised/pop_ups/cluster_videos_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     4027 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.89.7/simba/unsupervised/pop_ups/transform_cluster_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     5048 2024-02-15 23:45:22.000000 Simba-UW-tf-dev-1.89.7/simba/unsupervised/pop_ups/embedding_correlations_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-02 14:39:26.000000 Simba-UW-tf-dev-1.89.7/simba/unsupervised/pop_ups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     4070 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.89.7/simba/unsupervised/pop_ups/transform_dim_reduction_popup.py
--rw-r--r--   0 simon      (501) staff       (20)    11182 2024-02-15 23:45:22.000000 Simba-UW-tf-dev-1.89.7/simba/unsupervised/pop_ups/fit_dim_reduction_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     2546 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.89.7/simba/unsupervised/pop_ups/data_extractor_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     4536 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.89.7/simba/unsupervised/pop_ups/cluster_validation_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9305 2024-02-15 23:45:22.000000 Simba-UW-tf-dev-1.89.7/simba/unsupervised/pop_ups/fit_cluster_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     2574 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.89.7/simba/unsupervised/pop_ups/clusterer_comparison_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     6527 2024-03-26 23:50:53.000000 Simba-UW-tf-dev-1.89.7/simba/unsupervised/pop_ups/grid_search_visualizer_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     4332 2024-03-28 20:02:59.000000 Simba-UW-tf-dev-1.89.7/simba/unsupervised/pop_ups/cluster_xai_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     3820 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.89.7/simba/unsupervised/pop_ups/cluster_frequentist_stats_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     2355 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.89.7/simba/unsupervised/pop_ups/print_embedding_info_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     9946 2024-04-02 18:34:25.000000 Simba-UW-tf-dev-1.89.7/simba/unsupervised/dataset_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    12982 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.89.7/simba/unsupervised/unsupervised_main.py
--rw-r--r--   0 simon      (501) staff       (20)    10175 2024-03-27 12:56:51.000000 Simba-UW-tf-dev-1.89.7/simba/unsupervised/grid_search_visualizers.py
--rw-r--r--   0 simon      (501) staff       (20)    16005 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.89.7/simba/unsupervised/data_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     5241 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.89.7/simba/unsupervised/outlier_detector.py
--rw-r--r--   0 simon      (501) staff       (20)    10397 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.89.7/simba/unsupervised/cluster_frequentist_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5798 2024-03-27 12:56:51.000000 Simba-UW-tf-dev-1.89.7/simba/unsupervised/embedding_correlation_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/unsupervised/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18194 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.89.7/simba/unsupervised/cluster_xai_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    15581 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.89.7/simba/unsupervised/umap_embedder.py
--rw-r--r--   0 simon      (501) staff       (20)     5582 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.89.7/simba/unsupervised/clusterer_comparison_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     4652 2024-03-26 19:09:58.000000 Simba-UW-tf-dev-1.89.7/simba/unsupervised/bout_aggregator.py
--rw-r--r--   0 simon      (501) staff       (20)     2188 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/unsupervised/data_map.yaml
--rw-r--r--   0 simon      (501) staff       (20)    14765 2024-03-26 19:09:58.000000 Simba-UW-tf-dev-1.89.7/simba/unsupervised/hdbscan_clusterer.py
--rw-r--r--   0 simon      (501) staff       (20)     3862 2024-02-15 21:37:53.000000 Simba-UW-tf-dev-1.89.7/simba/unsupervised/tsne.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 00:28:53.000000 Simba-UW-tf-dev-1.89.7/simba/bounding_box_tools/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/bounding_box_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8511 2024-02-08 00:53:55.000000 Simba-UW-tf-dev-1.89.7/simba/bounding_box_tools/agg_boundary_stats.py
--rw-r--r--   0 simon      (501) staff       (20)    27255 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/bounding_box_tools/boundary_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    10064 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/bounding_box_tools/boundary_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     7146 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/bounding_box_tools/find_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    12066 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/bounding_box_tools/visualize_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    18436 2024-04-10 01:59:19.000000 Simba-UW-tf-dev-1.89.7/simba/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 00:28:53.000000 Simba-UW-tf-dev-1.89.7/simba/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)    57052 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/feature_extractors/feature_extractor_14bp.py
--rw-r--r--   0 simon      (501) staff       (20)    28094 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/feature_extractors/feature_extractor_7bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 00:28:53.000000 Simba-UW-tf-dev-1.89.7/simba/feature_extractors/misc/
--rw-r--r--   0 simon      (501) staff       (20)     1757 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.89.7/simba/feature_extractors/misc/doctests.py
--rw-r--r--   0 simon      (501) staff       (20)    29328 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.89.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
--rw-r--r--   0 simon      (501) staff       (20)     2705 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.89.7/simba/feature_extractors/misc/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2689 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.89.7/simba/feature_extractors/misc/peaks.py
--rw-r--r--   0 simon      (501) staff       (20)    16727 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.89.7/simba/feature_extractors/misc/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     2144 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.89.7/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     5762 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.89.7/simba/feature_extractors/misc/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)    26425 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.89.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
--rw-r--r--   0 simon      (501) staff       (20)     7535 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.89.7/simba/feature_extractors/misc/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)     1274 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.89.7/simba/feature_extractors/misc/count_values_in_range.py
--rw-r--r--   0 simon      (501) staff       (20)     5011 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.89.7/simba/feature_extractors/misc/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.89.7/simba/feature_extractors/misc/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)      736 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.89.7/simba/feature_extractors/misc/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     2883 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.89.7/simba/feature_extractors/misc/video_color.py
--rw-r--r--   0 simon      (501) staff       (20)     2055 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.89.7/simba/feature_extractors/misc/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.89.7/simba/feature_extractors/misc/video_rotator.py
--rw-r--r--   0 simon      (501) staff       (20)     2932 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.89.7/simba/feature_extractors/misc/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.89.7/simba/feature_extractors/misc/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)    37024 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.89.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
--rw-r--r--   0 simon      (501) staff       (20)     1613 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.89.7/simba/feature_extractors/misc/time_stamp_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.89.7/simba/feature_extractors/misc/video_rotator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    37022 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.89.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
--rw-r--r--   0 simon      (501) staff       (20)     2068 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.89.7/simba/feature_extractors/misc/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)    36307 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/feature_extractors/feature_extractor_8bps_2_animals.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-02-21 02:05:27.000000 Simba-UW-tf-dev-1.89.7/simba/feature_extractors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     4091 2024-02-16 21:14:07.000000 Simba-UW-tf-dev-1.89.7/simba/feature_extractors/perimeter_jit.py
--rw-r--r--   0 simon      (501) staff       (20)    26471 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/feature_extractors/feature_subsets.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/feature_extractors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    10043 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/feature_extractors/feature_extractor_user_defined.py
--rw-r--r--   0 simon      (501) staff       (20)    61607 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/feature_extractors/feature_extractor_16bp.py
--rw-r--r--   0 simon      (501) staff       (20)    37328 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/feature_extractors/feature_extractor_9bp.py
--rw-r--r--   0 simon      (501) staff       (20)    31163 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/feature_extractors/feature_extractor_8bp.py
--rw-r--r--   0 simon      (501) staff       (20)    21427 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/feature_extractors/feature_extractor_4bp.py
--rw-r--r--   0 simon      (501) staff       (20)    65534 2024-03-01 16:55:51.000000 Simba-UW-tf-dev-1.89.7/simba/feature_extractors/amber_feature_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     1033 2024-04-11 12:52:35.000000 Simba-UW-tf-dev-1.89.7/simba/requirements.txt
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 00:28:53.000000 Simba-UW-tf-dev-1.89.7/simba/mixins/
--rw-r--r--   0 simon      (501) staff       (20)    40917 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/mixins/annotator_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    84153 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.89.7/simba/mixins/timeseries_features_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-03 14:38:30.000000 Simba-UW-tf-dev-1.89.7/simba/mixins/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    53232 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.89.7/simba/mixins/pop_up_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    48428 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.89.7/simba/mixins/config_reader.py
--rw-r--r--   0 simon      (501) staff       (20)    56305 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.89.7/simba/mixins/circular_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    32080 2024-03-14 19:32:58.000000 Simba-UW-tf-dev-1.89.7/simba/mixins/network_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/mixins/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    24046 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.89.7/simba/mixins/pose_importer_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     3020 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/mixins/video_processing_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    35642 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.89.7/simba/mixins/feature_extraction_supplement_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)   149080 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.89.7/simba/mixins/statistics_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    44711 2024-03-14 19:32:58.000000 Simba-UW-tf-dev-1.89.7/simba/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    87052 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.89.7/simba/mixins/plotting_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)      391 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/mixins/abstract_classes.py
--rw-r--r--   0 simon      (501) staff       (20)    56806 2024-03-07 19:24:42.000000 Simba-UW-tf-dev-1.89.7/simba/mixins/image_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)      880 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.89.7/simba/mixins/unsupervised_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)   132883 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.89.7/simba/mixins/train_model_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)   166028 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.89.7/simba/mixins/geometry_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    24978 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/mixins/feature_extraction_circular_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 00:28:53.000000 Simba-UW-tf-dev-1.89.7/simba/third_party_label_appenders/
--rw-r--r--   0 simon      (501) staff       (20)     6639 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/third_party_label_appenders/deepethogram_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    12306 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/third_party_label_appenders/BORIS_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     9739 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/third_party_label_appenders/observer_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-22 19:49:42.000000 Simba-UW-tf-dev-1.89.7/simba/third_party_label_appenders/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     5508 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/third_party_label_appenders/boris_source_cleaner.py
--rw-r--r--   0 simon      (501) staff       (20)    18982 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/third_party_label_appenders/tools.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/third_party_label_appenders/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18852 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/third_party_label_appenders/third_party_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     9215 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/third_party_label_appenders/ethovision_import.py
--rw-r--r--   0 simon      (501) staff       (20)     7456 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/third_party_label_appenders/BENTO_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     5662 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/third_party_label_appenders/solomon_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 00:28:53.000000 Simba-UW-tf-dev-1.89.7/simba/cue_light_tools/
--rw-r--r--   0 simon      (501) staff       (20)     8841 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/cue_light_tools/cue_light_clf_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    14451 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/cue_light_tools/cue_light_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    18274 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/cue_light_tools/cue_light_menues.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/cue_light_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1921 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/cue_light_tools/cue_light_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    19237 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/cue_light_tools/cue_light_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    15278 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/cue_light_tools/cue_light_movement_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 00:28:53.000000 Simba-UW-tf-dev-1.89.7/simba/utils/
--rw-r--r--   0 simon      (501) staff       (20)    13211 2024-02-16 01:12:37.000000 Simba-UW-tf-dev-1.89.7/simba/utils/config_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    26038 2024-03-27 13:42:19.000000 Simba-UW-tf-dev-1.89.7/simba/utils/enums.py
--rw-r--r--   0 simon      (501) staff       (20)    10420 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.89.7/simba/utils/custom_feature_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-28 13:50:53.000000 Simba-UW-tf-dev-1.89.7/simba/utils/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7737 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.89.7/simba/utils/warnings.py
--rw-r--r--   0 simon      (501) staff       (20)    49585 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.89.7/simba/utils/checks.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/utils/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    77219 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.89.7/simba/utils/read_write.py
--rw-r--r--   0 simon      (501) staff       (20)    15357 2024-04-08 15:44:21.000000 Simba-UW-tf-dev-1.89.7/simba/utils/lookups.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 00:28:53.000000 Simba-UW-tf-dev-1.89.7/simba/utils/cli/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/utils/cli/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7129 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/utils/cli/cli_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    17086 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/utils/errors.py
--rw-r--r--   0 simon      (501) staff       (20)    44962 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.89.7/simba/utils/data.py
--rw-r--r--   0 simon      (501) staff       (20)      717 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.89.7/simba/utils/keyboard_listener.py
--rw-r--r--   0 simon      (501) staff       (20)     4205 2024-02-21 03:51:46.000000 Simba-UW-tf-dev-1.89.7/simba/utils/printing.py
--rw-r--r--   0 simon      (501) staff       (20)   243998 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/SimBA_logo.ico
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 00:28:53.000000 Simba-UW-tf-dev-1.89.7/simba/pose_processors/
--rw-r--r--   0 simon      (501) staff       (20)     8626 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/pose_processors/reorganize_keypoint.py
--rw-r--r--   0 simon      (501) staff       (20)     5840 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/pose_processors/remove_keypoints.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/pose_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2872 2024-02-15 23:39:58.000000 Simba-UW-tf-dev-1.89.7/simba/pose_processors/pose_reset.py
--rw-r--r--   0 simon      (501) staff       (20)     6313 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/pose_processors/reverse_pose.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 00:28:53.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/
--rw-r--r--   0 simon      (501) staff       (20)      786 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/doctests.py
--rw-r--r--   0 simon      (501) staff       (20)    29328 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/fish_feature_extractor_2023_version_3.py
--rw-r--r--   0 simon      (501) staff       (20)     2387 2024-03-08 14:35:02.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/dprime.py
--rw-r--r--   0 simon      (501) staff       (20)     2516 2024-03-18 17:01:43.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/linear_fretchet.py
--rw-r--r--   0 simon      (501) staff       (20)     2705 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2391 2024-03-14 12:45:59.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/piotr_120324 3.py.zip
--rw-r--r--   0 simon      (501) staff       (20)     2036 2024-03-28 18:29:59.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/dunn_index.py
--rw-r--r--   0 simon      (501) staff       (20)     3640 2024-04-08 13:30:56.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/hausdorff.py
--rw-r--r--   0 simon      (501) staff       (20)     2689 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/peaks.py
--rw-r--r--   0 simon      (501) staff       (20)    16727 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     3494 2024-04-03 13:42:02.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/colinear_features.py
--rw-r--r--   0 simon      (501) staff       (20)     8921 2024-03-22 13:56:46.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/spontaneous_alternation_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    21658 2024-04-10 16:31:38.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/horizontal_videos_concat.py
--rw-r--r--   0 simon      (501) staff       (20)     2144 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     1103 2024-03-29 16:26:34.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/silhouette_score.py
--rw-r--r--   0 simon      (501) staff       (20)     3607 2024-04-09 14:21:58.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/two_fish_feature_extractor_040924.py.zip
--rw-r--r--   0 simon      (501) staff       (20)    33092 2024-02-22 15:57:45.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/cuda_jit.ipynb
--rw-r--r--   0 simon      (501) staff       (20)     5762 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)     1867 2024-03-12 19:23:40.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/directed_hausdorff.py
--rw-r--r--   0 simon      (501) staff       (20)      963 2024-03-13 18:20:52.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/shannon_diversity_index.py
--rw-r--r--   0 simon      (501) staff       (20)     3726 2024-03-12 13:31:58.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/sequential_lag_analysis.py
--rw-r--r--   0 simon      (501) staff       (20)     1254 2024-03-13 16:09:50.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/wilcoxon.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-09 15:37:24.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3328 2024-03-08 15:05:36.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/data.npy
--rw-r--r--   0 simon      (501) staff       (20)    12626 2024-03-25 20:59:27.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/distances.py
--rw-r--r--   0 simon      (501) staff       (20)    26425 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/fish_feature_extractor_2023_version_2.py
--rw-r--r--   0 simon      (501) staff       (20)     2699 2024-03-10 16:29:57.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/cohens_kappa.py
--rw-r--r--   0 simon      (501) staff       (20)     2465 2024-03-08 17:38:19.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/paths.py
--rw-r--r--   0 simon      (501) staff       (20)     1048 2024-03-13 14:41:23.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/outliers_tietjen.py
--rw-r--r--   0 simon      (501) staff       (20)     1424 2024-02-26 15:46:14.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/train_model.py
--rw-r--r--   0 simon      (501) staff       (20)     3171 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/amber_tests.py
--rw-r--r--   0 simon      (501) staff       (20)     3590 2024-03-11 17:05:31.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/line_locate_point.py
--rw-r--r--   0 simon      (501) staff       (20)     3182 2024-02-24 20:57:19.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/multifrm_to_points.py
--rw-r--r--   0 simon      (501) staff       (20)       69 2024-03-18 18:17:24.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/lcs.py
--rw-r--r--   0 simon      (501) staff       (20)    12448 2024-04-09 14:14:37.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/two_fish_feature_extractor_040924.py
--rw-r--r--   0 simon      (501) staff       (20)     7535 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)     2350 2024-03-12 17:58:33.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/add_body_part.py
--rw-r--r--   0 simon      (501) staff       (20)     1008 2024-03-12 13:29:20.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/grubbs_test.py
--rw-r--r--   0 simon      (501) staff       (20)     3399 2024-02-16 01:12:37.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/slide_circ_mean.py
--rw-r--r--   0 simon      (501) staff       (20)     1835 2024-03-28 22:56:59.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/calinski_harabasz.py
--rw-r--r--   0 simon      (501) staff       (20)     1282 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/roi_feature_visualizer_example.py
--rw-r--r--   0 simon      (501) staff       (20)    10076 2024-03-22 16:51:40.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/spontaneuous_alternation_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)      895 2024-03-12 14:09:55.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/runs_test.py
--rw-r--r--   0 simon      (501) staff       (20)     2516 2024-04-06 11:33:24.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/pct_counts_in_top_N.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:46:33.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2287 2024-03-25 16:45:04.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/total_variation_distance.py
--rw-r--r--   0 simon      (501) staff       (20)     3056 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/crop_single_polygon.py
--rw-r--r--   0 simon      (501) staff       (20)     8010 2024-03-24 19:48:22.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/joint_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     2552 2024-04-02 14:48:59.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/elliptic_envelope.py
--rw-r--r--   0 simon      (501) staff       (20)     1016 2024-03-14 14:57:29.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/roi_definition_csvs_to_h5.py.zip
--rw-r--r--   0 simon      (501) staff       (20)     1276 2024-03-12 17:58:38.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/add_body_part.py.zip
--rw-r--r--   0 simon      (501) staff       (20)      921 2024-02-26 15:46:14.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/roi_feature_visualizer_example.py.zip
--rw-r--r--   0 simon      (501) staff       (20)     2631 2024-04-05 16:23:07.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/sliding_crosscorrelation.py
--rw-r--r--   0 simon      (501) staff       (20)     1274 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/count_values_in_range.py
--rw-r--r--   0 simon      (501) staff       (20)     2174 2024-03-14 14:56:26.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/roi_definition_csvs_to_h5.py
--rw-r--r--   0 simon      (501) staff       (20)     1656 2024-03-30 18:32:44.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/distance_velocity.py
--rw-r--r--   0 simon      (501) staff       (20)     5011 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     5666 2024-04-11 15:28:58.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/line_plot_plotly.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)     1351 2024-03-26 21:10:40.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/unsupervised_lof.py
--rw-r--r--   0 simon      (501) staff       (20)     2553 2024-03-11 15:09:38.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/siegel_tukey.py
--rw-r--r--   0 simon      (501) staff       (20)      958 2024-03-13 18:05:08.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/berger_parker.py
--rw-r--r--   0 simon      (501) staff       (20)     4177 2024-04-10 01:56:43.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/isolation_forest.py
--rw-r--r--   0 simon      (501) staff       (20)     2845 2024-03-28 19:23:54.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/davis_bouldin.py
--rw-r--r--   0 simon      (501) staff       (20)     4094 2024-04-10 14:09:54.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/vertical_video_concatenator.py
--rw-r--r--   0 simon      (501) staff       (20)     2770 2024-04-07 19:14:13.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/batch_video_to_greyscale.py
--rw-r--r--   0 simon      (501) staff       (20)     7215 2024-02-26 15:46:14.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/crop_circles_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1410 2024-03-19 12:49:24.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/heading.py
--rw-r--r--   0 simon      (501) staff       (20)     2243 2024-03-13 18:35:02.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/piotr_120324 2.py.zip
--rw-r--r--   0 simon      (501) staff       (20)      736 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     2907 2024-03-14 19:31:25.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/grangercausalitytests.py
--rw-r--r--   0 simon      (501) staff       (20)     2432 2024-03-19 20:48:43.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/multiframe_is_shape_covered.py
--rw-r--r--   0 simon      (501) staff       (20)      592 2024-02-27 21:31:33.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/redis.py
--rw-r--r--   0 simon      (501) staff       (20)     2893 2024-02-26 20:49:33.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/video_color.py
--rw-r--r--   0 simon      (501) staff       (20)     2055 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     6186 2024-03-18 12:44:45.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/piotr_120324.py
--rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/video_rotator.py
--rw-r--r--   0 simon      (501) staff       (20)     1004 2024-03-12 13:11:45.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/hartley_fmax.py
--rw-r--r--   0 simon      (501) staff       (20)       84 2024-04-03 17:05:23.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/calc_N_degree_direction_switches.py
--rw-r--r--   0 simon      (501) staff       (20)     2307 2024-02-27 21:31:33.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/fix_clahe.py
--rw-r--r--   0 simon      (501) staff       (20)     1836 2024-03-10 15:38:46.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/cochran_q.py
--rw-r--r--   0 simon      (501) staff       (20)      682 2024-03-13 19:19:43.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/menhinicks_index.py
--rw-r--r--   0 simon      (501) staff       (20)     2932 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)    13575 2024-03-20 11:47:11.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/spontanous_alternations.py
--rw-r--r--   0 simon      (501) staff       (20)     2268 2024-03-13 13:59:07.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/piotr_120324.py.zip
--rw-r--r--   0 simon      (501) staff       (20)     4655 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/velocity_aggregator.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)     4478 2024-04-08 20:43:42.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/abod.py
--rw-r--r--   0 simon      (501) staff       (20)    37024 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/fish_feature_extractor_2023_version_5.py
--rw-r--r--   0 simon      (501) staff       (20)     1073 2024-03-13 16:46:16.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/simpson_diversity_index.py
--rw-r--r--   0 simon      (501) staff       (20)     2396 2024-03-17 16:55:38.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/piotr_120324 4.py.zip
--rw-r--r--   0 simon      (501) staff       (20)     5336 2024-02-10 20:28:08.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/geometry_ex.py
--rw-r--r--   0 simon      (501) staff       (20)     1613 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/time_stamp_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     1505 2024-03-28 14:36:24.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/line_plot.py
--rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/video_rotator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15996 2024-04-09 13:41:30.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/unsupervised_outliers.py
--rw-r--r--   0 simon      (501) staff       (20)     5690 2024-02-10 20:28:08.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/statistics_ex.py
--rw-r--r--   0 simon      (501) staff       (20)     1391 2024-03-18 23:21:46.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/sliding_displacement.py
--rw-r--r--   0 simon      (501) staff       (20)      925 2024-03-11 13:06:04.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/wald_wolfowitz.py
--rw-r--r--   0 simon      (501) staff       (20)     1814 2024-04-05 14:36:58.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/sliding_autoc.py
--rw-r--r--   0 simon      (501) staff       (20)     2369 2024-03-14 17:07:10.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/linestring_path.py
--rw-r--r--   0 simon      (501) staff       (20)     2233 2024-03-18 15:20:48.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/cronbach_alpha.py
--rw-r--r--   0 simon      (501) staff       (20)     2809 2024-03-08 21:15:58.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/mcnamar.py
--rw-r--r--   0 simon      (501) staff       (20)    37022 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/fish_feature_extractor_2023_version_4.py
--rw-r--r--   0 simon      (501) staff       (20)     6220 2024-02-24 20:57:19.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/AmberFeatureExtractor.py.zip
--rw-r--r--   0 simon      (501) staff       (20)     1933 2024-04-10 15:09:25.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/mosaic.py
--rw-r--r--   0 simon      (501) staff       (20)    69423 2024-02-20 14:30:23.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/amber_featurizer.py
--rw-r--r--   0 simon      (501) staff       (20)      837 2024-03-13 18:56:21.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/margalef_diversification_index.py
--rw-r--r--   0 simon      (501) staff       (20)      997 2024-03-17 17:49:00.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/biweight_midcorrelation.py
--rw-r--r--   0 simon      (501) staff       (20)     2186 2024-03-18 15:31:23.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/madmedianrule.py
--rw-r--r--   0 simon      (501) staff       (20)     2915 2024-04-01 14:12:59.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/adjusted_rand_score.py
--rw-r--r--   0 simon      (501) staff       (20)     2068 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/sandbox/convex_hull_scratch_2.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 00:28:53.000000 Simba-UW-tf-dev-1.89.7/simba/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     8538 2024-02-23 18:25:51.000000 Simba-UW-tf-dev-1.89.7/simba/plotting/directing_animals_to_bodypart_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    10127 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/plotting/gantt_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 00:28:53.000000 Simba-UW-tf-dev-1.89.7/simba/plotting/tools/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:43:56.000000 Simba-UW-tf-dev-1.89.7/simba/plotting/tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     5946 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/plotting/tools/tkinter_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    17927 2024-04-04 16:23:22.000000 Simba-UW-tf-dev-1.89.7/simba/plotting/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-28 13:50:53.000000 Simba-UW-tf-dev-1.89.7/simba/plotting/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    19270 2024-03-31 17:21:01.000000 Simba-UW-tf-dev-1.89.7/simba/plotting/shap_agg_stats_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    11178 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/plotting/gantt_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15819 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/plotting/heat_mapper_clf_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    10376 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/plotting/probability_plot_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     8467 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/plotting/circular_plotting.py
--rw-r--r--   0 simon      (501) staff       (20)    16868 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/plotting/plot_clf_results.py
--rw-r--r--   0 simon      (501) staff       (20)    16620 2024-02-27 15:29:59.000000 Simba-UW-tf-dev-1.89.7/simba/plotting/plot_clf_results_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    22893 2024-02-21 04:33:19.000000 Simba-UW-tf-dev-1.89.7/simba/plotting/ROI_feature_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    13622 2024-02-21 04:25:14.000000 Simba-UW-tf-dev-1.89.7/simba/plotting/heat_mapper_location.py
--rw-r--r--   0 simon      (501) staff       (20)    11075 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/plotting/probability_plot_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/plotting/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     5253 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/plotting/interactive_probability_grapher.py
--rw-r--r--   0 simon      (501) staff       (20)     6517 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/plotting/plot_pose_in_dir.py
--rw-r--r--   0 simon      (501) staff       (20)    20950 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.89.7/simba/plotting/single_run_model_validation_video.py
--rw-r--r--   0 simon      (501) staff       (20)     8732 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.89.7/simba/plotting/frame_mergerer_ffmpeg.py
--rw-r--r--   0 simon      (501) staff       (20)    10667 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.89.7/simba/plotting/pose_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     9368 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/plotting/directing_animals_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    14389 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/plotting/clf_validator.py
--rw-r--r--   0 simon      (501) staff       (20)    22754 2024-03-06 18:18:21.000000 Simba-UW-tf-dev-1.89.7/simba/plotting/path_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    14075 2024-02-24 20:34:51.000000 Simba-UW-tf-dev-1.89.7/simba/plotting/ROI_feature_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    10774 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/plotting/data_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13091 2024-03-26 23:49:10.000000 Simba-UW-tf-dev-1.89.7/simba/plotting/spontaneous_alternation_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    23178 2024-02-21 17:08:03.000000 Simba-UW-tf-dev-1.89.7/simba/plotting/path_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     9311 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/plotting/ez_lineplot.py
--rw-r--r--   0 simon      (501) staff       (20)    16812 2024-04-12 00:22:58.000000 Simba-UW-tf-dev-1.89.7/simba/plotting/distance_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    22994 2024-02-21 04:08:15.000000 Simba-UW-tf-dev-1.89.7/simba/plotting/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    10034 2024-03-19 12:54:07.000000 Simba-UW-tf-dev-1.89.7/simba/plotting/geometry_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    16661 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/plotting/clf_validator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    14224 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/plotting/heat_mapper_clf.py
--rw-r--r--   0 simon      (501) staff       (20)    11994 2024-04-11 22:38:54.000000 Simba-UW-tf-dev-1.89.7/simba/plotting/distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    19073 2024-04-11 20:26:33.000000 Simba-UW-tf-dev-1.89.7/simba/plotting/single_run_model_validation_video_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    12286 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/plotting/directing_animals_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    11453 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/plotting/circular_feature_overlay_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    14576 2024-02-21 04:11:21.000000 Simba-UW-tf-dev-1.89.7/simba/plotting/heat_mapper_location_mp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 00:28:53.000000 Simba-UW-tf-dev-1.89.7/simba/dash_app/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:44:15.000000 Simba-UW-tf-dev-1.89.7/simba/dash_app/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    72715 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/dash_app/SimBA_dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     4965 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/dash_app/run_dash_tkinter.py
--rw-r--r--   0 simon      (501) staff       (20)    47546 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/dash_app/dash_app.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 00:28:53.000000 Simba-UW-tf-dev-1.89.7/simba/data_processors/
--rw-r--r--   0 simon      (501) staff       (20)    14926 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.89.7/simba/data_processors/spontaneous_alternation_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    11813 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/data_processors/agg_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-28 13:50:53.000000 Simba-UW-tf-dev-1.89.7/simba/data_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    13224 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/data_processors/severity_bout_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    39110 2024-03-19 12:54:07.000000 Simba-UW-tf-dev-1.89.7/simba/data_processors/interpolation_smoothing.py
--rw-r--r--   0 simon      (501) staff       (20)    10968 2024-02-21 19:10:40.000000 Simba-UW-tf-dev-1.89.7/simba/data_processors/directing_animal_to_bodypart.py
--rw-r--r--   0 simon      (501) staff       (20)     9580 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/data_processors/timebins_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    20288 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/data_processors/fsttc_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/data_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     4793 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/data_processors/boolean_conditional_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     7117 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/data_processors/interpolate_pose.py
--rw-r--r--   0 simon      (501) staff       (20)    16335 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/data_processors/directing_other_animals_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8957 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/data_processors/gibbs_sampler.py
--rw-r--r--   0 simon      (501) staff       (20)    10054 2024-04-04 16:23:22.000000 Simba-UW-tf-dev-1.89.7/simba/data_processors/timebins_movement_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5255 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/data_processors/severity_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    18517 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/data_processors/pup_retrieval_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3118 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/data_processors/pybursts_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    13660 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/data_processors/severity_frame_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8738 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/data_processors/mutual_exclusivity_corrector.py
--rw-r--r--   0 simon      (501) staff       (20)    12919 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/data_processors/kleinberg_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    10196 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/data_processors/movement_calculator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 00:28:53.000000 Simba-UW-tf-dev-1.89.7/simba/model/
--rw-r--r--   0 simon      (501) staff       (20)    23779 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.89.7/simba/model/train_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     4969 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/model/inference_batch.py
--rw-r--r--   0 simon      (501) staff       (20)    14036 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/model/train_multiclass_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3937 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/model/inference_multiclass_batch.py
--rw-r--r--   0 simon      (501) staff       (20)    15931 2024-02-20 14:30:06.000000 Simba-UW-tf-dev-1.89.7/simba/model/grid_search_multiclass_rf.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:41:19.000000 Simba-UW-tf-dev-1.89.7/simba/model/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    16987 2024-02-22 11:58:09.000000 Simba-UW-tf-dev-1.89.7/simba/model/grid_search_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3768 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/model/inference_validation.py
--rw-r--r--   0 simon      (501) staff       (20)     6872 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/model/train_multilabel_rf.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 00:28:53.000000 Simba-UW-tf-dev-1.89.7/simba/roi_tools/
--rw-r--r--   0 simon      (501) staff       (20)    12190 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.89.7/simba/roi_tools/ROI_time_bin_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     1803 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/roi_tools/ROI_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-22 19:49:42.000000 Simba-UW-tf-dev-1.89.7/simba/roi_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    50018 2024-03-11 20:20:39.000000 Simba-UW-tf-dev-1.89.7/simba/roi_tools/ROI_define.py
--rw-r--r--   0 simon      (501) staff       (20)     3616 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/roi_tools/ROI_reset.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/roi_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     9876 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/roi_tools/ROI_size_standardizer.py
--rw-r--r--   0 simon      (501) staff       (20)    30615 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.89.7/simba/roi_tools/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    15704 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/roi_tools/ROI_feature_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     4386 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/roi_tools/ROI_multiply.py
--rw-r--r--   0 simon      (501) staff       (20)     2313 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/roi_tools/ROI_size_calculations.py
--rw-r--r--   0 simon      (501) staff       (20)     3716 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/roi_tools/ROI_zoom.py
--rw-r--r--   0 simon      (501) staff       (20)    13394 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/roi_tools/ROI_directing_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    11974 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/roi_tools/ROI_move_shape.py
--rw-r--r--   0 simon      (501) staff       (20)     5470 2024-02-21 03:51:46.000000 Simba-UW-tf-dev-1.89.7/simba/roi_tools/ROI_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    16129 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/roi_tools/ROI_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    29730 2024-03-14 14:41:12.000000 Simba-UW-tf-dev-1.89.7/simba/roi_tools/ROI_image.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 00:28:53.000000 Simba-UW-tf-dev-1.89.7/simba/pose_importers/
--rw-r--r--   0 simon      (501) staff       (20)    10711 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.89.7/simba/pose_importers/sleap_csv_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 00:28:53.000000 Simba-UW-tf-dev-1.89.7/simba/pose_importers/misc/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:31.000000 Simba-UW-tf-dev-1.89.7/simba/pose_importers/misc/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8084 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/pose_importers/misc/apt_trk_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     2577 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/pose_importers/read_DANNCE_mat.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-22 19:49:42.000000 Simba-UW-tf-dev-1.89.7/simba/pose_importers/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    14268 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.89.7/simba/pose_importers/sleap_h5_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     8161 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/pose_importers/madlc_importer.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/pose_importers/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    13672 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.89.7/simba/pose_importers/sleap_slp_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     8645 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/pose_importers/import_mars.py
--rw-r--r--   0 simon      (501) staff       (20)     7464 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/pose_importers/dlc_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     8417 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/pose_importers/trk_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 00:28:53.000000 Simba-UW-tf-dev-1.89.7/simba/pose_configurations/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2024-03-19 18:18:43.000000 Simba-UW-tf-dev-1.89.7/simba/pose_configurations/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 00:28:53.000000 Simba-UW-tf-dev-1.89.7/simba/pose_configurations/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:10.000000 Simba-UW-tf-dev-1.89.7/simba/pose_configurations/bp_names/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     4485 2024-03-04 19:10:54.000000 Simba-UW-tf-dev-1.89.7/simba/pose_configurations/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 00:28:53.000000 Simba-UW-tf-dev-1.89.7/simba/pose_configurations/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       27 2024-03-04 19:10:54.000000 Simba-UW-tf-dev-1.89.7/simba/pose_configurations/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:18.000000 Simba-UW-tf-dev-1.89.7/simba/pose_configurations/no_animals/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:05.000000 Simba-UW-tf-dev-1.89.7/simba/pose_configurations/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 00:28:53.000000 Simba-UW-tf-dev-1.89.7/simba/pose_configurations/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:14.000000 Simba-UW-tf-dev-1.89.7/simba/pose_configurations/configuration_names/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)      273 2024-03-04 19:10:54.000000 Simba-UW-tf-dev-1.89.7/simba/pose_configurations/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 00:28:53.000000 Simba-UW-tf-dev-1.89.7/simba/pose_configurations/schematics/
--rw-r--r--   0 simon      (501) staff       (20)    39805 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/pose_configurations/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/pose_configurations/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/pose_configurations/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    34231 2024-02-20 18:50:39.000000 Simba-UW-tf-dev-1.89.7/simba/pose_configurations/schematics/13.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/pose_configurations/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/pose_configurations/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/pose_configurations/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/pose_configurations/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/pose_configurations/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/pose_configurations/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/pose_configurations/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/pose_configurations/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/pose_configurations/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 00:28:53.000000 Simba-UW-tf-dev-1.89.7/simba/video_processors/
--rw-r--r--   0 simon      (501) staff       (20)   113176 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.89.7/simba/video_processors/video_processing.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-26 15:01:23.000000 Simba-UW-tf-dev-1.89.7/simba/video_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     5577 2024-04-08 11:29:52.000000 Simba-UW-tf-dev-1.89.7/simba/video_processors/roi_selector_circle.py
--rw-r--r--   0 simon      (501) staff       (20)     9073 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/video_processors/px_to_mm.py
--rw-r--r--   0 simon      (501) staff       (20)    35053 2024-02-26 15:42:07.000000 Simba-UW-tf-dev-1.89.7/simba/video_processors/batch_process_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    11439 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/video_processors/multi_cropper.py
--rw-r--r--   0 simon      (501) staff       (20)     3066 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/video_processors/extract_frames.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/video_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6598 2024-02-26 21:50:01.000000 Simba-UW-tf-dev-1.89.7/simba/video_processors/roi_selector.py
--rw-r--r--   0 simon      (501) staff       (20)    10007 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/video_processors/calculate_px_dist.py
--rw-r--r--   0 simon      (501) staff       (20)     5963 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.89.7/simba/video_processors/roi_selector_polygon.py
--rw-r--r--   0 simon      (501) staff       (20)     4926 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/video_processors/extract_seqframes.py
--rw-r--r--   0 simon      (501) staff       (20)    15117 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.89.7/simba/video_processors/batch_process_create_ffmpeg_commands.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 00:28:53.000000 Simba-UW-tf-dev-1.89.7/simba/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     7837 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/outlier_tools/outlier_corrector_movement.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/outlier_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    14462 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/outlier_tools/outlier_corrector_location_advanced.py
--rw-r--r--   0 simon      (501) staff       (20)    13117 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/outlier_tools/outlier_corrector_movement_advanced.py
--rw-r--r--   0 simon      (501) staff       (20)    10396 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/outlier_tools/outlier_corrector_location.py
--rw-r--r--   0 simon      (501) staff       (20)     2751 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/outlier_tools/skip_outlier_correction.py
--rw-r--r--   0 simon      (501) staff       (20)    81222 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.89.7/simba/SimBA.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 00:28:53.000000 Simba-UW-tf-dev-1.89.7/simba/assets/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 00:28:53.000000 Simba-UW-tf-dev-1.89.7/simba/assets/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)   109483 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/unsupervised/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:36.000000 Simba-UW-tf-dev-1.89.7/simba/assets/unsupervised/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    14175 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/unsupervised/features.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 00:28:53.000000 Simba-UW-tf-dev-1.89.7/simba/assets/shap/
--rw-r--r--   0 simon      (501) staff       (20)     1177 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/shap/down_arrow.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1733 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/shap/intruder_shape.jpg
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 00:28:53.000000 Simba-UW-tf-dev-1.89.7/simba/assets/shap/feature_categories/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:25.000000 Simba-UW-tf-dev-1.89.7/simba/assets/shap/feature_categories/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    17420 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/shap/feature_categories/shap_feature_categories.csv
--rw-r--r--   0 simon      (501) staff       (20)     1665 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/shap/resident_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2415 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/shap/resident_intruder_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2012 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/shap/animal_distances.jpg
--rw-r--r--   0 simon      (501) staff       (20)     4422 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/shap/baseline_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:21.000000 Simba-UW-tf-dev-1.89.7/simba/assets/shap/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)   353824 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/shap/ubuntu.regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     6672 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/shap/side_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   189004 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/shap/UbuntuMono-Regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     2737 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/shap/side_scale_5.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1785 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/shap/intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1435 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/shap/resident_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     3134 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/shap/color_bar.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2120 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/shap/resident_intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)    10244 2024-04-09 23:07:16.000000 Simba-UW-tf-dev-1.89.7/simba/assets/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 00:28:53.000000 Simba-UW-tf-dev-1.89.7/simba/assets/lookups/
--rw-r--r--   0 simon      (501) staff       (20)   270783 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/lookups/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)     2987 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/lookups/feature_extraction_headers.csv
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:11.000000 Simba-UW-tf-dev-1.89.7/simba/assets/lookups/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    26256 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/lookups/critical_values_05.pickle
--rw-r--r--   0 simon      (501) staff       (20)    14175 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/lookups/features.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/lookups/unsupervised_example_x.csv
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:41:54.000000 Simba-UW-tf-dev-1.89.7/simba/assets/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 00:28:53.000000 Simba-UW-tf-dev-1.89.7/simba/assets/stl/
--rw-r--r--   0 simon      (501) staff       (20)   551576 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/stl/operant_tray.stl
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:31.000000 Simba-UW-tf-dev-1.89.7/simba/assets/stl/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    67647 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/stl/operant_lever.stl
--rw-r--r--   0 simon      (501) staff       (20)    92896 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/stl/operant_walls.stl
--rw-r--r--   0 simon      (501) staff       (20)  4759984 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/stl/grid_floor.stl
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 00:28:53.000000 Simba-UW-tf-dev-1.89.7/simba/assets/img/
--rw-r--r--   0 simon      (501) staff       (20)   489479 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/img/splash_2024.mp4
--rw-r--r--   0 simon      (501) staff       (20)    79863 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/img/bg_2024.png
--rw-r--r--   0 simon      (501) staff       (20)   399272 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/img/about_me.png
--rw-r--r--   0 simon      (501) staff       (20)   117108 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/img/splash.mp4
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:02.000000 Simba-UW-tf-dev-1.89.7/simba/assets/img/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)   322242 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/img/bg_2.png
--rw-r--r--   0 simon      (501) staff       (20)      165 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/img/~$splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)    69267 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/img/splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)   204362 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/img/bg.png
--rw-r--r--   0 simon      (501) staff       (20)   189004 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/UbuntuMono-Regular.ttf
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 00:28:53.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/
--rw-r--r--   0 simon      (501) staff       (20)     1350 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/factory.png
--rw-r--r--   0 simon      (501) staff       (20)     1413 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/cluster.png
--rw-r--r--   0 simon      (501) staff       (20)     1340 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/load.png
--rw-r--r--   0 simon      (501) staff       (20)     4507 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/gif.png
--rw-r--r--   0 simon      (501) staff       (20)     4566 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/pose.png
--rw-r--r--   0 simon      (501) staff       (20)     1943 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/features.png
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-09 15:42:22.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     4896 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/settings.png
--rw-r--r--   0 simon      (501) staff       (20)     2090 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/stopwatch.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/link.png
--rw-r--r--   0 simon      (501) staff       (20)    14250 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/dash_simba.css
--rw-r--r--   0 simon      (501) staff       (20)      917 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/documentation.png
--rw-r--r--   0 simon      (501) staff       (20)     4503 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/fps.png
--rw-r--r--   0 simon      (501) staff       (20)     1299 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/dimensionality_reduction.png
--rw-r--r--   0 simon      (501) staff       (20)     4823 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/roi.png
--rw-r--r--   0 simon      (501) staff       (20)   171446 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/simba_logo_2.png
--rw-r--r--   0 simon      (501) staff       (20)      920 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/superimpose.png
--rw-r--r--   0 simon      (501) staff       (20)     1136 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/label.png
--rw-r--r--   0 simon      (501) staff       (20)     1016 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/change.png
--rw-r--r--   0 simon      (501) staff       (20)    59896 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/readthedocs_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     1124 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/crop.png
--rw-r--r--   0 simon      (501) staff       (20)     2146 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/rotate.png
--rw-r--r--   0 simon      (501) staff       (20)     1921 2024-02-26 14:29:54.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/circle.png
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:44:37.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1057 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/path.png
--rw-r--r--   0 simon      (501) staff       (20)     1148 2024-02-26 20:39:14.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/polygon.png
--rw-r--r--   0 simon      (501) staff       (20)      950 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/clip.png
--rw-r--r--   0 simon      (501) staff       (20)     2121 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/restart.png
--rw-r--r--   0 simon      (501) staff       (20)     4653 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/calipher.png
--rw-r--r--   0 simon      (501) staff       (20)     1291 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/add_on.png
--rw-r--r--   0 simon      (501) staff       (20)     4695 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/create.png
--rw-r--r--   0 simon      (501) staff       (20)    78182 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/SimBA_logo.ico
--rw-r--r--   0 simon      (501) staff       (20)     1067 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/print.png
--rw-r--r--   0 simon      (501) staff       (20)     4653 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/clf.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 00:28:53.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/concat_icons/
--rw-r--r--   0 simon      (501) staff       (20)     6027 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/concat_icons/mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     5654 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/concat_icons/vertical.png
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:44:45.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/concat_icons/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     5542 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/concat_icons/horizontal.png
--rw-r--r--   0 simon      (501) staff       (20)     5939 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/concat_icons/mixed_mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     2060 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/merge.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/clean.png
--rw-r--r--   0 simon      (501) staff       (20)     4725 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/clf_2.png
--rw-r--r--   0 simon      (501) staff       (20)     4795 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/visualize.png
--rw-r--r--   0 simon      (501) staff       (20)     2142 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/concat.png
--rw-r--r--   0 simon      (501) staff       (20)     1474 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/boris.png
--rw-r--r--   0 simon      (501) staff       (20)     4804 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/frames.png
--rw-r--r--   0 simon      (501) staff       (20)     2425 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/video.png
--rw-r--r--   0 simon      (501) staff       (20)     2089 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/sample.png
--rw-r--r--   0 simon      (501) staff       (20)     1471 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/metrics.png
--rw-r--r--   0 simon      (501) staff       (20)     4555 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/grey.png
--rw-r--r--   0 simon      (501) staff       (20)      930 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/exit.png
--rw-r--r--   0 simon      (501) staff       (20)     4751 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/outlier.png
--rw-r--r--   0 simon      (501) staff       (20)     4392 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/clahe.png
--rw-r--r--   0 simon      (501) staff       (20)     4637 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/trash.png
--rw-r--r--   0 simon      (501) staff       (20)     1239 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/about.png
--rw-r--r--   0 simon      (501) staff       (20)     4666 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/convert.png
--rw-r--r--   0 simon      (501) staff       (20)    93229 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/SimBA_logo.icns
--rw-r--r--   0 simon      (501) staff       (20)      991 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/reorganize.png
--rw-r--r--   0 simon      (501) staff       (20)     4784 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/browse.png
--rw-r--r--   0 simon      (501) staff       (20)    30707 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/SimBA_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     2293 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/ethovision.png
--rw-r--r--   0 simon      (501) staff       (20)     1018 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/icons/close.png
--rw-r--r--   0 simon      (501) staff       (20)    13672 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/dash_simba_base.css
--rw-r--r--   0 simon      (501) staff       (20)    31812 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.7/simba/assets/TheGoldenLab.PNG
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 00:28:53.000000 Simba-UW-tf-dev-1.89.7/Simba_UW_tf_dev.egg-info/
--rw-r--r--   0 simon      (501) staff       (20)     2797 2024-04-12 00:28:52.000000 Simba-UW-tf-dev-1.89.7/Simba_UW_tf_dev.egg-info/PKG-INFO
--rw-r--r--   0 simon      (501) staff       (20)    23031 2024-04-12 00:28:52.000000 Simba-UW-tf-dev-1.89.7/Simba_UW_tf_dev.egg-info/SOURCES.txt
--rw-r--r--   0 simon      (501) staff       (20)       44 2024-04-12 00:28:52.000000 Simba-UW-tf-dev-1.89.7/Simba_UW_tf_dev.egg-info/entry_points.txt
--rw-r--r--   0 simon      (501) staff       (20)      797 2024-04-12 00:28:52.000000 Simba-UW-tf-dev-1.89.7/Simba_UW_tf_dev.egg-info/requires.txt
--rw-r--r--   0 simon      (501) staff       (20)        6 2024-04-12 00:28:52.000000 Simba-UW-tf-dev-1.89.7/Simba_UW_tf_dev.egg-info/top_level.txt
--rw-r--r--   0 simon      (501) staff       (20)        1 2024-04-12 00:28:52.000000 Simba-UW-tf-dev-1.89.7/Simba_UW_tf_dev.egg-info/dependency_links.txt
--rw-r--r--   0 simon      (501) staff       (20)    35127 2024-02-07 18:56:10.000000 Simba-UW-tf-dev-1.89.7/LICENSE
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 00:28:53.000000 Simba-UW-tf-dev-1.89.7/tests/
--rw-r--r--   0 simon      (501) staff       (20)     4753 2024-04-11 20:40:04.000000 Simba-UW-tf-dev-1.89.7/tests/test_data_processors.py
--rw-r--r--   0 simon      (501) staff       (20)    13415 2024-03-01 16:43:04.000000 Simba-UW-tf-dev-1.89.7/tests/test_circlular_stats.py
--rw-r--r--   0 simon      (501) staff       (20)    13399 2024-04-11 20:36:51.000000 Simba-UW-tf-dev-1.89.7/tests/test_stats.py
--rw-r--r--   0 simon      (501) staff       (20)     5374 2024-04-11 22:48:09.000000 Simba-UW-tf-dev-1.89.7/tests/test_distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    11863 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.89.7/tests/test_train_model_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     6525 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.89.7/tests/test_feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     1739 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.89.7/tests/test_utils_data.py
--rw-r--r--   0 simon      (501) staff       (20)     8120 2024-03-01 19:06:25.000000 Simba-UW-tf-dev-1.89.7/tests/test_config_reader_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     1070 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.89.7/tests/test_outlier_correctors.py
--rw-r--r--   0 simon      (501) staff       (20)     4435 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.89.7/tests/test_visualize_directing_animals.py
--rw-r--r--   0 simon      (501) staff       (20)     1596 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.89.7/tests/test_featurizers.py
--rw-r--r--   0 simon      (501) staff       (20)     8570 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.89.7/tests/test_video_processors.py
--rw-r--r--   0 simon      (501) staff       (20)     3554 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.89.7/tests/test_thirdparty_appenders.py
--rw-r--r--   0 simon      (501) staff       (20)     3021 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.89.7/tests/test_validation_clips.py
--rw-r--r--   0 simon      (501) staff       (20)     3992 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.89.7/tests/test_roi_tools.py
--rw-r--r--   0 simon      (501) staff       (20)      318 2024-03-04 20:16:28.000000 Simba-UW-tf-dev-1.89.7/MANIFEST.in
--rw-r--r--   0 simon      (501) staff       (20)    18403 2024-02-12 00:49:21.000000 Simba-UW-tf-dev-1.89.7/README.md
--rw-r--r--   0 simon      (501) staff       (20)     1426 2024-04-12 00:28:51.000000 Simba-UW-tf-dev-1.89.7/setup.py
--rw-r--r--   0 simon      (501) staff       (20)       38 2024-04-12 00:28:53.000000 Simba-UW-tf-dev-1.89.7/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 20:23:20.000000 Simba-UW-tf-dev-1.89.8/
+-rw-r--r--   0 simon      (501) staff       (20)     2797 2024-04-12 20:23:20.000000 Simba-UW-tf-dev-1.89.8/PKG-INFO
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 20:23:19.000000 Simba-UW-tf-dev-1.89.8/simba/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 20:23:20.000000 Simba-UW-tf-dev-1.89.8/simba/ui/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-28 13:50:53.000000 Simba-UW-tf-dev-1.89.8/simba/ui/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 20:23:20.000000 Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/
+-rw-r--r--   0 simon      (501) staff       (20)    11467 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/mutual_exclusivity_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4070 2024-03-29 20:30:28.000000 Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1676 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/csv_2_parquet_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2566 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/quick_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2873 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/batch_preprocess_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8835 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/heatmap_location_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9734 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/clf_probability_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3456 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/movement_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4631 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    11362 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/clf_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    24905 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1184 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/remove_roi_features_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6692 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/targeted_annotation_clips_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3340 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2174 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/roi_size_standardizer_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     6997 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5068 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/roi_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7898 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/outlier_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9048 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/gantt_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6293 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/clf_validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8529 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/severity_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3221 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/fsttc_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4231 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/kleinberg_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7979 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9785 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/spontaneous_alternation_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6076 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/pose_reorganizer_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3437 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/animal_directing_other_animals_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3402 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3468 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/clf_by_timebins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9154 2024-04-12 00:32:53.000000 Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/heatmap_clf_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9235 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/data_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    11785 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/roi_features_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9118 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/pup_retrieval_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5577 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/boolean_conditional_slicer_pup_up.py
+-rw-r--r--   0 simon      (501) staff       (20)      584 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/about_simba_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5451 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    10747 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1795 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7312 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/directing_animal_to_bodypart_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6546 2024-02-16 01:12:37.000000 Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    66309 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/video_processing_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7800 2024-04-04 16:47:32.000000 Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6160 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/clf_by_roi_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2741 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/make_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3622 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/direction_animal_to_bodypart_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6166 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1072 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/archive_files_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4716 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/pose_bp_drop_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    12174 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/distance_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4673 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3290 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4134 2024-03-31 17:07:13.000000 Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    16701 2024-02-08 00:53:55.000000 Simba-UW-tf-dev-1.89.8/simba/ui/video_info_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     6573 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.89.8/simba/ui/user_defined_pose_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/ui/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    14374 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.89.8/simba/ui/create_project_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)    14487 2024-02-08 00:53:55.000000 Simba-UW-tf-dev-1.89.8/simba/ui/tkinter_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    38870 2024-04-04 16:45:40.000000 Simba-UW-tf-dev-1.89.8/simba/ui/machine_model_settings_ui.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 20:23:19.000000 Simba-UW-tf-dev-1.89.8/simba/labelling/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/labelling/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    24423 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/labelling/labelling_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     2362 2024-02-21 02:33:04.000000 Simba-UW-tf-dev-1.89.8/simba/labelling/targeted_annotations_clips.py
+-rw-r--r--   0 simon      (501) staff       (20)     3974 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/labelling/extract_labelled_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)    31269 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/labelling/labelling_advanced_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)    10012 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/labelling/play_annotation_video.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 20:23:20.000000 Simba-UW-tf-dev-1.89.8/simba/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)    15004 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.89.8/simba/unsupervised/dbcv_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5077 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.89.8/simba/unsupervised/cluster_validation_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3645 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.89.8/simba/unsupervised/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-03 14:33:55.000000 Simba-UW-tf-dev-1.89.8/simba/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     9036 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.89.8/simba/unsupervised/cluster_video_visualizer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 20:23:20.000000 Simba-UW-tf-dev-1.89.8/simba/unsupervised/pop_ups/
+-rw-r--r--   0 simon      (501) staff       (20)     4642 2024-03-26 23:50:53.000000 Simba-UW-tf-dev-1.89.8/simba/unsupervised/pop_ups/cluster_videos_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     4027 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.89.8/simba/unsupervised/pop_ups/transform_cluster_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     5048 2024-02-15 23:45:22.000000 Simba-UW-tf-dev-1.89.8/simba/unsupervised/pop_ups/embedding_correlations_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-02 14:39:26.000000 Simba-UW-tf-dev-1.89.8/simba/unsupervised/pop_ups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     4070 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.89.8/simba/unsupervised/pop_ups/transform_dim_reduction_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)    11182 2024-02-15 23:45:22.000000 Simba-UW-tf-dev-1.89.8/simba/unsupervised/pop_ups/fit_dim_reduction_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     2546 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.89.8/simba/unsupervised/pop_ups/data_extractor_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     4536 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.89.8/simba/unsupervised/pop_ups/cluster_validation_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9305 2024-02-15 23:45:22.000000 Simba-UW-tf-dev-1.89.8/simba/unsupervised/pop_ups/fit_cluster_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     2574 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.89.8/simba/unsupervised/pop_ups/clusterer_comparison_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     6527 2024-03-26 23:50:53.000000 Simba-UW-tf-dev-1.89.8/simba/unsupervised/pop_ups/grid_search_visualizer_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     4332 2024-03-28 20:02:59.000000 Simba-UW-tf-dev-1.89.8/simba/unsupervised/pop_ups/cluster_xai_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     3820 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.89.8/simba/unsupervised/pop_ups/cluster_frequentist_stats_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     2355 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.89.8/simba/unsupervised/pop_ups/print_embedding_info_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     9946 2024-04-02 18:34:25.000000 Simba-UW-tf-dev-1.89.8/simba/unsupervised/dataset_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12982 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.89.8/simba/unsupervised/unsupervised_main.py
+-rw-r--r--   0 simon      (501) staff       (20)    10175 2024-03-27 12:56:51.000000 Simba-UW-tf-dev-1.89.8/simba/unsupervised/grid_search_visualizers.py
+-rw-r--r--   0 simon      (501) staff       (20)    16005 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.89.8/simba/unsupervised/data_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     5241 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.89.8/simba/unsupervised/outlier_detector.py
+-rw-r--r--   0 simon      (501) staff       (20)    10397 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.89.8/simba/unsupervised/cluster_frequentist_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5798 2024-03-27 12:56:51.000000 Simba-UW-tf-dev-1.89.8/simba/unsupervised/embedding_correlation_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/unsupervised/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18194 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.89.8/simba/unsupervised/cluster_xai_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    15581 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.89.8/simba/unsupervised/umap_embedder.py
+-rw-r--r--   0 simon      (501) staff       (20)     5582 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.89.8/simba/unsupervised/clusterer_comparison_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     4652 2024-03-26 19:09:58.000000 Simba-UW-tf-dev-1.89.8/simba/unsupervised/bout_aggregator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2188 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/unsupervised/data_map.yaml
+-rw-r--r--   0 simon      (501) staff       (20)    14765 2024-03-26 19:09:58.000000 Simba-UW-tf-dev-1.89.8/simba/unsupervised/hdbscan_clusterer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3862 2024-02-15 21:37:53.000000 Simba-UW-tf-dev-1.89.8/simba/unsupervised/tsne.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 20:23:19.000000 Simba-UW-tf-dev-1.89.8/simba/bounding_box_tools/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/bounding_box_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8511 2024-02-08 00:53:55.000000 Simba-UW-tf-dev-1.89.8/simba/bounding_box_tools/agg_boundary_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)    27255 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/bounding_box_tools/boundary_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    10064 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/bounding_box_tools/boundary_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     7146 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/bounding_box_tools/find_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    12066 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/bounding_box_tools/visualize_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    18436 2024-04-10 01:59:19.000000 Simba-UW-tf-dev-1.89.8/simba/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 20:23:19.000000 Simba-UW-tf-dev-1.89.8/simba/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)    57052 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/feature_extractors/feature_extractor_14bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    28094 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/feature_extractors/feature_extractor_7bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 20:23:19.000000 Simba-UW-tf-dev-1.89.8/simba/feature_extractors/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     1757 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.89.8/simba/feature_extractors/misc/doctests.py
+-rw-r--r--   0 simon      (501) staff       (20)    29328 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.89.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     2705 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.89.8/simba/feature_extractors/misc/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2689 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.89.8/simba/feature_extractors/misc/peaks.py
+-rw-r--r--   0 simon      (501) staff       (20)    16727 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.89.8/simba/feature_extractors/misc/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     2144 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.89.8/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.89.8/simba/feature_extractors/misc/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)    26425 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.89.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     7535 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.89.8/simba/feature_extractors/misc/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)     1274 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.89.8/simba/feature_extractors/misc/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     5011 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.89.8/simba/feature_extractors/misc/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.89.8/simba/feature_extractors/misc/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)      736 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.89.8/simba/feature_extractors/misc/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     2883 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.89.8/simba/feature_extractors/misc/video_color.py
+-rw-r--r--   0 simon      (501) staff       (20)     2055 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.89.8/simba/feature_extractors/misc/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.89.8/simba/feature_extractors/misc/video_rotator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2932 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.89.8/simba/feature_extractors/misc/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.89.8/simba/feature_extractors/misc/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)    37024 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.89.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
+-rw-r--r--   0 simon      (501) staff       (20)     1613 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.89.8/simba/feature_extractors/misc/time_stamp_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.89.8/simba/feature_extractors/misc/video_rotator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    37022 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.89.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
+-rw-r--r--   0 simon      (501) staff       (20)     2068 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.89.8/simba/feature_extractors/misc/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    36307 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/feature_extractors/feature_extractor_8bps_2_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-02-21 02:05:27.000000 Simba-UW-tf-dev-1.89.8/simba/feature_extractors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     4091 2024-02-16 21:14:07.000000 Simba-UW-tf-dev-1.89.8/simba/feature_extractors/perimeter_jit.py
+-rw-r--r--   0 simon      (501) staff       (20)    26471 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/feature_extractors/feature_subsets.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/feature_extractors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    10043 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/feature_extractors/feature_extractor_user_defined.py
+-rw-r--r--   0 simon      (501) staff       (20)    61607 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/feature_extractors/feature_extractor_16bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    37328 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/feature_extractors/feature_extractor_9bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    31163 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/feature_extractors/feature_extractor_8bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21427 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/feature_extractors/feature_extractor_4bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    65534 2024-03-01 16:55:51.000000 Simba-UW-tf-dev-1.89.8/simba/feature_extractors/amber_feature_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     1033 2024-04-11 12:52:35.000000 Simba-UW-tf-dev-1.89.8/simba/requirements.txt
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 20:23:19.000000 Simba-UW-tf-dev-1.89.8/simba/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)    40917 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/mixins/annotator_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    84153 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.89.8/simba/mixins/timeseries_features_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-03 14:38:30.000000 Simba-UW-tf-dev-1.89.8/simba/mixins/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    53232 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.89.8/simba/mixins/pop_up_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    48428 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.89.8/simba/mixins/config_reader.py
+-rw-r--r--   0 simon      (501) staff       (20)    56305 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.89.8/simba/mixins/circular_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    32080 2024-03-14 19:32:58.000000 Simba-UW-tf-dev-1.89.8/simba/mixins/network_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/mixins/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    24046 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.89.8/simba/mixins/pose_importer_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     3020 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/mixins/video_processing_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    35642 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.89.8/simba/mixins/feature_extraction_supplement_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)   149080 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.89.8/simba/mixins/statistics_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    44711 2024-03-14 19:32:58.000000 Simba-UW-tf-dev-1.89.8/simba/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    87038 2024-04-12 15:37:04.000000 Simba-UW-tf-dev-1.89.8/simba/mixins/plotting_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)      391 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/mixins/abstract_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)    56806 2024-03-07 19:24:42.000000 Simba-UW-tf-dev-1.89.8/simba/mixins/image_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)      880 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.89.8/simba/mixins/unsupervised_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)   132883 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.89.8/simba/mixins/train_model_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)   166028 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.89.8/simba/mixins/geometry_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    24978 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/mixins/feature_extraction_circular_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 20:23:20.000000 Simba-UW-tf-dev-1.89.8/simba/third_party_label_appenders/
+-rw-r--r--   0 simon      (501) staff       (20)     6639 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/third_party_label_appenders/deepethogram_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12306 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/third_party_label_appenders/BORIS_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     9739 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/third_party_label_appenders/observer_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-22 19:49:42.000000 Simba-UW-tf-dev-1.89.8/simba/third_party_label_appenders/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     5508 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/third_party_label_appenders/boris_source_cleaner.py
+-rw-r--r--   0 simon      (501) staff       (20)    18982 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/third_party_label_appenders/tools.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/third_party_label_appenders/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18852 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/third_party_label_appenders/third_party_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     9215 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/third_party_label_appenders/ethovision_import.py
+-rw-r--r--   0 simon      (501) staff       (20)     7456 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/third_party_label_appenders/BENTO_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     5662 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/third_party_label_appenders/solomon_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 20:23:19.000000 Simba-UW-tf-dev-1.89.8/simba/cue_light_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     8841 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/cue_light_tools/cue_light_clf_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    14451 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/cue_light_tools/cue_light_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    18274 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/cue_light_tools/cue_light_menues.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/cue_light_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1921 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/cue_light_tools/cue_light_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    19237 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/cue_light_tools/cue_light_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    15278 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/cue_light_tools/cue_light_movement_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 20:23:20.000000 Simba-UW-tf-dev-1.89.8/simba/utils/
+-rw-r--r--   0 simon      (501) staff       (20)    13211 2024-02-16 01:12:37.000000 Simba-UW-tf-dev-1.89.8/simba/utils/config_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    26038 2024-03-27 13:42:19.000000 Simba-UW-tf-dev-1.89.8/simba/utils/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)    10420 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.89.8/simba/utils/custom_feature_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-28 13:50:53.000000 Simba-UW-tf-dev-1.89.8/simba/utils/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7737 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.89.8/simba/utils/warnings.py
+-rw-r--r--   0 simon      (501) staff       (20)    49867 2024-04-12 18:22:48.000000 Simba-UW-tf-dev-1.89.8/simba/utils/checks.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/utils/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    77219 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.89.8/simba/utils/read_write.py
+-rw-r--r--   0 simon      (501) staff       (20)    15356 2024-04-12 00:53:11.000000 Simba-UW-tf-dev-1.89.8/simba/utils/lookups.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 20:23:20.000000 Simba-UW-tf-dev-1.89.8/simba/utils/cli/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/utils/cli/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7129 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/utils/cli/cli_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    17086 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/utils/errors.py
+-rw-r--r--   0 simon      (501) staff       (20)    44962 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.89.8/simba/utils/data.py
+-rw-r--r--   0 simon      (501) staff       (20)      717 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.89.8/simba/utils/keyboard_listener.py
+-rw-r--r--   0 simon      (501) staff       (20)     4205 2024-02-21 03:51:46.000000 Simba-UW-tf-dev-1.89.8/simba/utils/printing.py
+-rw-r--r--   0 simon      (501) staff       (20)   243998 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/SimBA_logo.ico
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 20:23:19.000000 Simba-UW-tf-dev-1.89.8/simba/pose_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     8626 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/pose_processors/reorganize_keypoint.py
+-rw-r--r--   0 simon      (501) staff       (20)     5840 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/pose_processors/remove_keypoints.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/pose_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2872 2024-02-15 23:39:58.000000 Simba-UW-tf-dev-1.89.8/simba/pose_processors/pose_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)     6313 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/pose_processors/reverse_pose.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 20:23:20.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/
+-rw-r--r--   0 simon      (501) staff       (20)      786 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/doctests.py
+-rw-r--r--   0 simon      (501) staff       (20)    29328 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/fish_feature_extractor_2023_version_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     2387 2024-03-08 14:35:02.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/dprime.py
+-rw-r--r--   0 simon      (501) staff       (20)     2516 2024-03-18 17:01:43.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/linear_fretchet.py
+-rw-r--r--   0 simon      (501) staff       (20)     2705 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2391 2024-03-14 12:45:59.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/piotr_120324 3.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)     2036 2024-03-28 18:29:59.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/dunn_index.py
+-rw-r--r--   0 simon      (501) staff       (20)     3640 2024-04-08 13:30:56.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/hausdorff.py
+-rw-r--r--   0 simon      (501) staff       (20)     2689 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/peaks.py
+-rw-r--r--   0 simon      (501) staff       (20)    16727 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     3494 2024-04-03 13:42:02.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/colinear_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     8921 2024-03-22 13:56:46.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/spontaneous_alternation_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    21658 2024-04-10 16:31:38.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/horizontal_videos_concat.py
+-rw-r--r--   0 simon      (501) staff       (20)     2144 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     1103 2024-03-29 16:26:34.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/silhouette_score.py
+-rw-r--r--   0 simon      (501) staff       (20)     3607 2024-04-09 14:21:58.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/two_fish_feature_extractor_040924.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)    33092 2024-02-22 15:57:45.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/cuda_jit.ipynb
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)     1867 2024-03-12 19:23:40.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/directed_hausdorff.py
+-rw-r--r--   0 simon      (501) staff       (20)      963 2024-03-13 18:20:52.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/shannon_diversity_index.py
+-rw-r--r--   0 simon      (501) staff       (20)     3726 2024-03-12 13:31:58.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/sequential_lag_analysis.py
+-rw-r--r--   0 simon      (501) staff       (20)     1254 2024-03-13 16:09:50.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/wilcoxon.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-09 15:37:24.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3328 2024-03-08 15:05:36.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/data.npy
+-rw-r--r--   0 simon      (501) staff       (20)    12626 2024-03-25 20:59:27.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/distances.py
+-rw-r--r--   0 simon      (501) staff       (20)    26425 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     2699 2024-03-10 16:29:57.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/cohens_kappa.py
+-rw-r--r--   0 simon      (501) staff       (20)     2465 2024-03-08 17:38:19.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/paths.py
+-rw-r--r--   0 simon      (501) staff       (20)     1048 2024-03-13 14:41:23.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/outliers_tietjen.py
+-rw-r--r--   0 simon      (501) staff       (20)     1424 2024-02-26 15:46:14.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/train_model.py
+-rw-r--r--   0 simon      (501) staff       (20)     3171 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/amber_tests.py
+-rw-r--r--   0 simon      (501) staff       (20)     3590 2024-03-11 17:05:31.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/line_locate_point.py
+-rw-r--r--   0 simon      (501) staff       (20)     3182 2024-02-24 20:57:19.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/multifrm_to_points.py
+-rw-r--r--   0 simon      (501) staff       (20)       69 2024-03-18 18:17:24.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/lcs.py
+-rw-r--r--   0 simon      (501) staff       (20)    12448 2024-04-09 14:14:37.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/two_fish_feature_extractor_040924.py
+-rw-r--r--   0 simon      (501) staff       (20)     7535 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)     2350 2024-03-12 17:58:33.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/add_body_part.py
+-rw-r--r--   0 simon      (501) staff       (20)     1008 2024-03-12 13:29:20.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/grubbs_test.py
+-rw-r--r--   0 simon      (501) staff       (20)     3399 2024-02-16 01:12:37.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/slide_circ_mean.py
+-rw-r--r--   0 simon      (501) staff       (20)     1835 2024-03-28 22:56:59.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/calinski_harabasz.py
+-rw-r--r--   0 simon      (501) staff       (20)     1282 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/roi_feature_visualizer_example.py
+-rw-r--r--   0 simon      (501) staff       (20)    10076 2024-03-22 16:51:40.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/spontaneuous_alternation_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)      895 2024-03-12 14:09:55.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/runs_test.py
+-rw-r--r--   0 simon      (501) staff       (20)     2516 2024-04-06 11:33:24.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/pct_counts_in_top_N.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:46:33.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2287 2024-03-25 16:45:04.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/total_variation_distance.py
+-rw-r--r--   0 simon      (501) staff       (20)     3056 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/crop_single_polygon.py
+-rw-r--r--   0 simon      (501) staff       (20)     8010 2024-03-24 19:48:22.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/joint_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     2552 2024-04-02 14:48:59.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/elliptic_envelope.py
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2024-03-14 14:57:29.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/roi_definition_csvs_to_h5.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)     1276 2024-03-12 17:58:38.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/add_body_part.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)      921 2024-02-26 15:46:14.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/roi_feature_visualizer_example.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)     2631 2024-04-05 16:23:07.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/sliding_crosscorrelation.py
+-rw-r--r--   0 simon      (501) staff       (20)     1274 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     2174 2024-03-14 14:56:26.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/roi_definition_csvs_to_h5.py
+-rw-r--r--   0 simon      (501) staff       (20)     1656 2024-03-30 18:32:44.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/distance_velocity.py
+-rw-r--r--   0 simon      (501) staff       (20)     5011 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5666 2024-04-11 15:28:58.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/line_plot_plotly.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)     1351 2024-03-26 21:10:40.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/unsupervised_lof.py
+-rw-r--r--   0 simon      (501) staff       (20)     2553 2024-03-11 15:09:38.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/siegel_tukey.py
+-rw-r--r--   0 simon      (501) staff       (20)      958 2024-03-13 18:05:08.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/berger_parker.py
+-rw-r--r--   0 simon      (501) staff       (20)     4177 2024-04-10 01:56:43.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/isolation_forest.py
+-rw-r--r--   0 simon      (501) staff       (20)     2845 2024-03-28 19:23:54.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/davis_bouldin.py
+-rw-r--r--   0 simon      (501) staff       (20)     4094 2024-04-10 14:09:54.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/vertical_video_concatenator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2770 2024-04-07 19:14:13.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/batch_video_to_greyscale.py
+-rw-r--r--   0 simon      (501) staff       (20)     7215 2024-02-26 15:46:14.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/crop_circles_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1410 2024-03-19 12:49:24.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/heading.py
+-rw-r--r--   0 simon      (501) staff       (20)     2243 2024-03-13 18:35:02.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/piotr_120324 2.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)      736 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     2907 2024-03-14 19:31:25.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/grangercausalitytests.py
+-rw-r--r--   0 simon      (501) staff       (20)     2432 2024-03-19 20:48:43.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/multiframe_is_shape_covered.py
+-rw-r--r--   0 simon      (501) staff       (20)      592 2024-02-27 21:31:33.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/redis.py
+-rw-r--r--   0 simon      (501) staff       (20)     2893 2024-02-26 20:49:33.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/video_color.py
+-rw-r--r--   0 simon      (501) staff       (20)     2055 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     6186 2024-03-18 12:44:45.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/piotr_120324.py
+-rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/video_rotator.py
+-rw-r--r--   0 simon      (501) staff       (20)     1004 2024-03-12 13:11:45.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/hartley_fmax.py
+-rw-r--r--   0 simon      (501) staff       (20)       84 2024-04-03 17:05:23.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/calc_N_degree_direction_switches.py
+-rw-r--r--   0 simon      (501) staff       (20)     2307 2024-02-27 21:31:33.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/fix_clahe.py
+-rw-r--r--   0 simon      (501) staff       (20)     1836 2024-03-10 15:38:46.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/cochran_q.py
+-rw-r--r--   0 simon      (501) staff       (20)      682 2024-03-13 19:19:43.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/menhinicks_index.py
+-rw-r--r--   0 simon      (501) staff       (20)     2932 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)    13575 2024-03-20 11:47:11.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/spontanous_alternations.py
+-rw-r--r--   0 simon      (501) staff       (20)     2268 2024-03-13 13:59:07.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/piotr_120324.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)     4655 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/velocity_aggregator.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)     4478 2024-04-08 20:43:42.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/abod.py
+-rw-r--r--   0 simon      (501) staff       (20)    37024 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/fish_feature_extractor_2023_version_5.py
+-rw-r--r--   0 simon      (501) staff       (20)     1073 2024-03-13 16:46:16.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/simpson_diversity_index.py
+-rw-r--r--   0 simon      (501) staff       (20)     2396 2024-03-17 16:55:38.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/piotr_120324 4.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)     5336 2024-02-10 20:28:08.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/geometry_ex.py
+-rw-r--r--   0 simon      (501) staff       (20)     1613 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/time_stamp_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     1505 2024-03-28 14:36:24.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/line_plot.py
+-rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/video_rotator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15996 2024-04-09 13:41:30.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/unsupervised_outliers.py
+-rw-r--r--   0 simon      (501) staff       (20)     5690 2024-02-10 20:28:08.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/statistics_ex.py
+-rw-r--r--   0 simon      (501) staff       (20)     1391 2024-03-18 23:21:46.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/sliding_displacement.py
+-rw-r--r--   0 simon      (501) staff       (20)      925 2024-03-11 13:06:04.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/wald_wolfowitz.py
+-rw-r--r--   0 simon      (501) staff       (20)     1814 2024-04-05 14:36:58.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/sliding_autoc.py
+-rw-r--r--   0 simon      (501) staff       (20)     2369 2024-03-14 17:07:10.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/linestring_path.py
+-rw-r--r--   0 simon      (501) staff       (20)     2233 2024-03-18 15:20:48.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/cronbach_alpha.py
+-rw-r--r--   0 simon      (501) staff       (20)     2809 2024-03-08 21:15:58.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/mcnamar.py
+-rw-r--r--   0 simon      (501) staff       (20)    37022 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/fish_feature_extractor_2023_version_4.py
+-rw-r--r--   0 simon      (501) staff       (20)     6220 2024-02-24 20:57:19.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/AmberFeatureExtractor.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)     1933 2024-04-10 15:09:25.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/mosaic.py
+-rw-r--r--   0 simon      (501) staff       (20)      441 2024-04-12 17:03:24.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/bouts_df
+-rw-r--r--   0 simon      (501) staff       (20)    69423 2024-02-20 14:30:23.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/amber_featurizer.py
+-rw-r--r--   0 simon      (501) staff       (20)      837 2024-03-13 18:56:21.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/margalef_diversification_index.py
+-rw-r--r--   0 simon      (501) staff       (20)      997 2024-03-17 17:49:00.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/biweight_midcorrelation.py
+-rw-r--r--   0 simon      (501) staff       (20)     2186 2024-03-18 15:31:23.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/madmedianrule.py
+-rw-r--r--   0 simon      (501) staff       (20)     2915 2024-04-01 14:12:59.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/adjusted_rand_score.py
+-rw-r--r--   0 simon      (501) staff       (20)     2068 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     1957 2024-04-12 14:55:03.000000 Simba-UW-tf-dev-1.89.8/simba/sandbox/plotly_gantt.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 20:23:19.000000 Simba-UW-tf-dev-1.89.8/simba/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     8538 2024-02-23 18:25:51.000000 Simba-UW-tf-dev-1.89.8/simba/plotting/directing_animals_to_bodypart_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10127 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/plotting/gantt_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 20:23:19.000000 Simba-UW-tf-dev-1.89.8/simba/plotting/tools/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:43:56.000000 Simba-UW-tf-dev-1.89.8/simba/plotting/tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     5946 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/plotting/tools/tkinter_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    17927 2024-04-04 16:23:22.000000 Simba-UW-tf-dev-1.89.8/simba/plotting/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-28 13:50:53.000000 Simba-UW-tf-dev-1.89.8/simba/plotting/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    19270 2024-03-31 17:21:01.000000 Simba-UW-tf-dev-1.89.8/simba/plotting/shap_agg_stats_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11322 2024-04-12 17:03:35.000000 Simba-UW-tf-dev-1.89.8/simba/plotting/gantt_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15819 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/plotting/heat_mapper_clf_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    10376 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/plotting/probability_plot_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8467 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/plotting/circular_plotting.py
+-rw-r--r--   0 simon      (501) staff       (20)    16868 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/plotting/plot_clf_results.py
+-rw-r--r--   0 simon      (501) staff       (20)    16620 2024-02-27 15:29:59.000000 Simba-UW-tf-dev-1.89.8/simba/plotting/plot_clf_results_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    22893 2024-02-21 04:33:19.000000 Simba-UW-tf-dev-1.89.8/simba/plotting/ROI_feature_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    13622 2024-02-21 04:25:14.000000 Simba-UW-tf-dev-1.89.8/simba/plotting/heat_mapper_location.py
+-rw-r--r--   0 simon      (501) staff       (20)    11075 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/plotting/probability_plot_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/plotting/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     5253 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/plotting/interactive_probability_grapher.py
+-rw-r--r--   0 simon      (501) staff       (20)     6517 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/plotting/plot_pose_in_dir.py
+-rw-r--r--   0 simon      (501) staff       (20)    20950 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.89.8/simba/plotting/single_run_model_validation_video.py
+-rw-r--r--   0 simon      (501) staff       (20)     8732 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.89.8/simba/plotting/frame_mergerer_ffmpeg.py
+-rw-r--r--   0 simon      (501) staff       (20)    10667 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.89.8/simba/plotting/pose_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     9368 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/plotting/directing_animals_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    14389 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/plotting/clf_validator.py
+-rw-r--r--   0 simon      (501) staff       (20)    22754 2024-03-06 18:18:21.000000 Simba-UW-tf-dev-1.89.8/simba/plotting/path_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    14075 2024-02-24 20:34:51.000000 Simba-UW-tf-dev-1.89.8/simba/plotting/ROI_feature_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    10774 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/plotting/data_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13091 2024-03-26 23:49:10.000000 Simba-UW-tf-dev-1.89.8/simba/plotting/spontaneous_alternation_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    23178 2024-02-21 17:08:03.000000 Simba-UW-tf-dev-1.89.8/simba/plotting/path_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     9311 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/plotting/ez_lineplot.py
+-rw-r--r--   0 simon      (501) staff       (20)    16812 2024-04-12 00:22:58.000000 Simba-UW-tf-dev-1.89.8/simba/plotting/distance_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    22994 2024-02-21 04:08:15.000000 Simba-UW-tf-dev-1.89.8/simba/plotting/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    10034 2024-03-19 12:54:07.000000 Simba-UW-tf-dev-1.89.8/simba/plotting/geometry_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    16661 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/plotting/clf_validator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    14224 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/plotting/heat_mapper_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)    11994 2024-04-11 22:38:54.000000 Simba-UW-tf-dev-1.89.8/simba/plotting/distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    19073 2024-04-11 20:26:33.000000 Simba-UW-tf-dev-1.89.8/simba/plotting/single_run_model_validation_video_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    12286 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/plotting/directing_animals_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11453 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/plotting/circular_feature_overlay_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    14576 2024-02-21 04:11:21.000000 Simba-UW-tf-dev-1.89.8/simba/plotting/heat_mapper_location_mp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 20:23:19.000000 Simba-UW-tf-dev-1.89.8/simba/dash_app/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:44:15.000000 Simba-UW-tf-dev-1.89.8/simba/dash_app/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    72715 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/dash_app/SimBA_dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     4965 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/dash_app/run_dash_tkinter.py
+-rw-r--r--   0 simon      (501) staff       (20)    47546 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/dash_app/dash_app.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 20:23:19.000000 Simba-UW-tf-dev-1.89.8/simba/data_processors/
+-rw-r--r--   0 simon      (501) staff       (20)    14926 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.89.8/simba/data_processors/spontaneous_alternation_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    11813 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/data_processors/agg_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-28 13:50:53.000000 Simba-UW-tf-dev-1.89.8/simba/data_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    13224 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/data_processors/severity_bout_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    39110 2024-03-19 12:54:07.000000 Simba-UW-tf-dev-1.89.8/simba/data_processors/interpolation_smoothing.py
+-rw-r--r--   0 simon      (501) staff       (20)    10968 2024-02-21 19:10:40.000000 Simba-UW-tf-dev-1.89.8/simba/data_processors/directing_animal_to_bodypart.py
+-rw-r--r--   0 simon      (501) staff       (20)     9580 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/data_processors/timebins_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    20288 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/data_processors/fsttc_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/data_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     4793 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/data_processors/boolean_conditional_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     7117 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/data_processors/interpolate_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)    16335 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/data_processors/directing_other_animals_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8957 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/data_processors/gibbs_sampler.py
+-rw-r--r--   0 simon      (501) staff       (20)    10054 2024-04-04 16:23:22.000000 Simba-UW-tf-dev-1.89.8/simba/data_processors/timebins_movement_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5255 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/data_processors/severity_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    18517 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/data_processors/pup_retrieval_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3118 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/data_processors/pybursts_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    13660 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/data_processors/severity_frame_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8738 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/data_processors/mutual_exclusivity_corrector.py
+-rw-r--r--   0 simon      (501) staff       (20)    12919 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/data_processors/kleinberg_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    10196 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/data_processors/movement_calculator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 20:23:19.000000 Simba-UW-tf-dev-1.89.8/simba/model/
+-rw-r--r--   0 simon      (501) staff       (20)    23779 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.89.8/simba/model/train_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     4969 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/model/inference_batch.py
+-rw-r--r--   0 simon      (501) staff       (20)    14036 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/model/train_multiclass_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3937 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/model/inference_multiclass_batch.py
+-rw-r--r--   0 simon      (501) staff       (20)    15931 2024-02-20 14:30:06.000000 Simba-UW-tf-dev-1.89.8/simba/model/grid_search_multiclass_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:41:19.000000 Simba-UW-tf-dev-1.89.8/simba/model/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    16987 2024-02-22 11:58:09.000000 Simba-UW-tf-dev-1.89.8/simba/model/grid_search_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3768 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/model/inference_validation.py
+-rw-r--r--   0 simon      (501) staff       (20)     6872 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/model/train_multilabel_rf.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 20:23:19.000000 Simba-UW-tf-dev-1.89.8/simba/roi_tools/
+-rw-r--r--   0 simon      (501) staff       (20)    12190 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.89.8/simba/roi_tools/ROI_time_bin_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     1803 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/roi_tools/ROI_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-22 19:49:42.000000 Simba-UW-tf-dev-1.89.8/simba/roi_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    50018 2024-03-11 20:20:39.000000 Simba-UW-tf-dev-1.89.8/simba/roi_tools/ROI_define.py
+-rw-r--r--   0 simon      (501) staff       (20)     3616 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/roi_tools/ROI_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/roi_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     9876 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/roi_tools/ROI_size_standardizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    30615 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.89.8/simba/roi_tools/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    15704 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/roi_tools/ROI_feature_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     4386 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/roi_tools/ROI_multiply.py
+-rw-r--r--   0 simon      (501) staff       (20)     2313 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/roi_tools/ROI_size_calculations.py
+-rw-r--r--   0 simon      (501) staff       (20)     3716 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/roi_tools/ROI_zoom.py
+-rw-r--r--   0 simon      (501) staff       (20)    13394 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/roi_tools/ROI_directing_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11974 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/roi_tools/ROI_move_shape.py
+-rw-r--r--   0 simon      (501) staff       (20)     5470 2024-02-21 03:51:46.000000 Simba-UW-tf-dev-1.89.8/simba/roi_tools/ROI_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    16129 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/roi_tools/ROI_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    29730 2024-03-14 14:41:12.000000 Simba-UW-tf-dev-1.89.8/simba/roi_tools/ROI_image.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 20:23:19.000000 Simba-UW-tf-dev-1.89.8/simba/pose_importers/
+-rw-r--r--   0 simon      (501) staff       (20)    10711 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.89.8/simba/pose_importers/sleap_csv_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 20:23:19.000000 Simba-UW-tf-dev-1.89.8/simba/pose_importers/misc/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:31.000000 Simba-UW-tf-dev-1.89.8/simba/pose_importers/misc/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8084 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/pose_importers/misc/apt_trk_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     2577 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/pose_importers/read_DANNCE_mat.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-22 19:49:42.000000 Simba-UW-tf-dev-1.89.8/simba/pose_importers/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    14268 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.89.8/simba/pose_importers/sleap_h5_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     8161 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/pose_importers/madlc_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/pose_importers/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.89.8/simba/pose_importers/sleap_slp_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     8645 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/pose_importers/import_mars.py
+-rw-r--r--   0 simon      (501) staff       (20)     7464 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/pose_importers/dlc_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     8417 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/pose_importers/trk_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 20:23:19.000000 Simba-UW-tf-dev-1.89.8/simba/pose_configurations/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2024-03-19 18:18:43.000000 Simba-UW-tf-dev-1.89.8/simba/pose_configurations/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 20:23:19.000000 Simba-UW-tf-dev-1.89.8/simba/pose_configurations/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:10.000000 Simba-UW-tf-dev-1.89.8/simba/pose_configurations/bp_names/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     4485 2024-03-04 19:10:54.000000 Simba-UW-tf-dev-1.89.8/simba/pose_configurations/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 20:23:19.000000 Simba-UW-tf-dev-1.89.8/simba/pose_configurations/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       27 2024-03-04 19:10:54.000000 Simba-UW-tf-dev-1.89.8/simba/pose_configurations/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:18.000000 Simba-UW-tf-dev-1.89.8/simba/pose_configurations/no_animals/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:05.000000 Simba-UW-tf-dev-1.89.8/simba/pose_configurations/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 20:23:19.000000 Simba-UW-tf-dev-1.89.8/simba/pose_configurations/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:14.000000 Simba-UW-tf-dev-1.89.8/simba/pose_configurations/configuration_names/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)      273 2024-03-04 19:10:54.000000 Simba-UW-tf-dev-1.89.8/simba/pose_configurations/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 20:23:19.000000 Simba-UW-tf-dev-1.89.8/simba/pose_configurations/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/pose_configurations/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/pose_configurations/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/pose_configurations/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    34231 2024-02-20 18:50:39.000000 Simba-UW-tf-dev-1.89.8/simba/pose_configurations/schematics/13.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/pose_configurations/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/pose_configurations/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/pose_configurations/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/pose_configurations/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/pose_configurations/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/pose_configurations/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/pose_configurations/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/pose_configurations/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/pose_configurations/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 20:23:20.000000 Simba-UW-tf-dev-1.89.8/simba/video_processors/
+-rw-r--r--   0 simon      (501) staff       (20)   115520 2024-04-12 18:22:48.000000 Simba-UW-tf-dev-1.89.8/simba/video_processors/video_processing.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-26 15:01:23.000000 Simba-UW-tf-dev-1.89.8/simba/video_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     5577 2024-04-08 11:29:52.000000 Simba-UW-tf-dev-1.89.8/simba/video_processors/roi_selector_circle.py
+-rw-r--r--   0 simon      (501) staff       (20)     9073 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/video_processors/px_to_mm.py
+-rw-r--r--   0 simon      (501) staff       (20)    35053 2024-02-26 15:42:07.000000 Simba-UW-tf-dev-1.89.8/simba/video_processors/batch_process_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    11439 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/video_processors/multi_cropper.py
+-rw-r--r--   0 simon      (501) staff       (20)     3066 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/video_processors/extract_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/video_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6598 2024-02-26 21:50:01.000000 Simba-UW-tf-dev-1.89.8/simba/video_processors/roi_selector.py
+-rw-r--r--   0 simon      (501) staff       (20)    10007 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/video_processors/calculate_px_dist.py
+-rw-r--r--   0 simon      (501) staff       (20)     5963 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.89.8/simba/video_processors/roi_selector_polygon.py
+-rw-r--r--   0 simon      (501) staff       (20)     4926 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/video_processors/extract_seqframes.py
+-rw-r--r--   0 simon      (501) staff       (20)    15117 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.89.8/simba/video_processors/batch_process_create_ffmpeg_commands.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 20:23:19.000000 Simba-UW-tf-dev-1.89.8/simba/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     7837 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/outlier_tools/outlier_corrector_movement.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/outlier_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    14462 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/outlier_tools/outlier_corrector_location_advanced.py
+-rw-r--r--   0 simon      (501) staff       (20)    13117 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/outlier_tools/outlier_corrector_movement_advanced.py
+-rw-r--r--   0 simon      (501) staff       (20)    10396 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/outlier_tools/outlier_corrector_location.py
+-rw-r--r--   0 simon      (501) staff       (20)     2751 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/outlier_tools/skip_outlier_correction.py
+-rw-r--r--   0 simon      (501) staff       (20)    81222 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.89.8/simba/SimBA.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 20:23:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 20:23:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)   109483 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/unsupervised/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:36.000000 Simba-UW-tf-dev-1.89.8/simba/assets/unsupervised/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/unsupervised/features.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 20:23:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/shap/
+-rw-r--r--   0 simon      (501) staff       (20)     1177 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/shap/down_arrow.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1733 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/shap/intruder_shape.jpg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 20:23:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/shap/feature_categories/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:25.000000 Simba-UW-tf-dev-1.89.8/simba/assets/shap/feature_categories/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    17420 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/shap/feature_categories/shap_feature_categories.csv
+-rw-r--r--   0 simon      (501) staff       (20)     1665 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/shap/resident_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2415 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/shap/resident_intruder_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2012 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/shap/animal_distances.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     4422 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/shap/baseline_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:21.000000 Simba-UW-tf-dev-1.89.8/simba/assets/shap/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)   353824 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/shap/ubuntu.regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     6672 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/shap/side_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/shap/UbuntuMono-Regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     2737 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/shap/side_scale_5.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1785 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/shap/intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1435 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/shap/resident_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     3134 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/shap/color_bar.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2120 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/shap/resident_intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2024-04-09 23:07:16.000000 Simba-UW-tf-dev-1.89.8/simba/assets/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 20:23:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/lookups/
+-rw-r--r--   0 simon      (501) staff       (20)   270783 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/lookups/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)     2987 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/lookups/feature_extraction_headers.csv
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:11.000000 Simba-UW-tf-dev-1.89.8/simba/assets/lookups/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    26256 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/lookups/critical_values_05.pickle
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/lookups/features.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/lookups/unsupervised_example_x.csv
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:41:54.000000 Simba-UW-tf-dev-1.89.8/simba/assets/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 20:23:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/stl/
+-rw-r--r--   0 simon      (501) staff       (20)   551576 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/stl/operant_tray.stl
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:31.000000 Simba-UW-tf-dev-1.89.8/simba/assets/stl/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    67647 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/stl/operant_lever.stl
+-rw-r--r--   0 simon      (501) staff       (20)    92896 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/stl/operant_walls.stl
+-rw-r--r--   0 simon      (501) staff       (20)  4759984 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/stl/grid_floor.stl
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 20:23:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/img/
+-rw-r--r--   0 simon      (501) staff       (20)   489479 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/img/splash_2024.mp4
+-rw-r--r--   0 simon      (501) staff       (20)    79863 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/img/bg_2024.png
+-rw-r--r--   0 simon      (501) staff       (20)   399272 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/img/about_me.png
+-rw-r--r--   0 simon      (501) staff       (20)   117108 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/img/splash.mp4
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:02.000000 Simba-UW-tf-dev-1.89.8/simba/assets/img/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)   322242 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/img/bg_2.png
+-rw-r--r--   0 simon      (501) staff       (20)      165 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/img/~$splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)    69267 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/img/splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)   204362 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/img/bg.png
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/UbuntuMono-Regular.ttf
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 20:23:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/
+-rw-r--r--   0 simon      (501) staff       (20)     1350 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/factory.png
+-rw-r--r--   0 simon      (501) staff       (20)     1413 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/cluster.png
+-rw-r--r--   0 simon      (501) staff       (20)     1340 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/load.png
+-rw-r--r--   0 simon      (501) staff       (20)     4507 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/gif.png
+-rw-r--r--   0 simon      (501) staff       (20)     4566 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/pose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1943 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/features.png
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-09 15:42:22.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     4896 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/settings.png
+-rw-r--r--   0 simon      (501) staff       (20)     2090 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/stopwatch.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/link.png
+-rw-r--r--   0 simon      (501) staff       (20)    14250 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/dash_simba.css
+-rw-r--r--   0 simon      (501) staff       (20)      917 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/documentation.png
+-rw-r--r--   0 simon      (501) staff       (20)     4503 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/fps.png
+-rw-r--r--   0 simon      (501) staff       (20)     1299 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/dimensionality_reduction.png
+-rw-r--r--   0 simon      (501) staff       (20)     4823 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/roi.png
+-rw-r--r--   0 simon      (501) staff       (20)   171446 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/simba_logo_2.png
+-rw-r--r--   0 simon      (501) staff       (20)      920 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/superimpose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1136 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/label.png
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/change.png
+-rw-r--r--   0 simon      (501) staff       (20)    59896 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/readthedocs_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     1124 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/crop.png
+-rw-r--r--   0 simon      (501) staff       (20)     2146 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/rotate.png
+-rw-r--r--   0 simon      (501) staff       (20)     1921 2024-02-26 14:29:54.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/circle.png
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:44:37.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1057 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/path.png
+-rw-r--r--   0 simon      (501) staff       (20)     1148 2024-02-26 20:39:14.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/polygon.png
+-rw-r--r--   0 simon      (501) staff       (20)      950 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/clip.png
+-rw-r--r--   0 simon      (501) staff       (20)     2121 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/restart.png
+-rw-r--r--   0 simon      (501) staff       (20)     4653 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/calipher.png
+-rw-r--r--   0 simon      (501) staff       (20)     1291 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/add_on.png
+-rw-r--r--   0 simon      (501) staff       (20)     4695 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/create.png
+-rw-r--r--   0 simon      (501) staff       (20)    78182 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/SimBA_logo.ico
+-rw-r--r--   0 simon      (501) staff       (20)     1067 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/print.png
+-rw-r--r--   0 simon      (501) staff       (20)     4653 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/clf.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 20:23:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/concat_icons/
+-rw-r--r--   0 simon      (501) staff       (20)     6027 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/concat_icons/mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     5654 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/concat_icons/vertical.png
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:44:45.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/concat_icons/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     5542 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/concat_icons/horizontal.png
+-rw-r--r--   0 simon      (501) staff       (20)     5939 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/concat_icons/mixed_mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     2060 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/merge.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/clean.png
+-rw-r--r--   0 simon      (501) staff       (20)     4725 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/clf_2.png
+-rw-r--r--   0 simon      (501) staff       (20)     4795 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/visualize.png
+-rw-r--r--   0 simon      (501) staff       (20)     2142 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/concat.png
+-rw-r--r--   0 simon      (501) staff       (20)     1474 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/boris.png
+-rw-r--r--   0 simon      (501) staff       (20)     4804 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/frames.png
+-rw-r--r--   0 simon      (501) staff       (20)     2425 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/video.png
+-rw-r--r--   0 simon      (501) staff       (20)     2089 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/sample.png
+-rw-r--r--   0 simon      (501) staff       (20)     1471 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/metrics.png
+-rw-r--r--   0 simon      (501) staff       (20)     4555 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/grey.png
+-rw-r--r--   0 simon      (501) staff       (20)      930 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/exit.png
+-rw-r--r--   0 simon      (501) staff       (20)     4751 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/outlier.png
+-rw-r--r--   0 simon      (501) staff       (20)     4392 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/clahe.png
+-rw-r--r--   0 simon      (501) staff       (20)     4637 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/trash.png
+-rw-r--r--   0 simon      (501) staff       (20)     1239 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/about.png
+-rw-r--r--   0 simon      (501) staff       (20)     4666 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/convert.png
+-rw-r--r--   0 simon      (501) staff       (20)    93229 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/SimBA_logo.icns
+-rw-r--r--   0 simon      (501) staff       (20)      991 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/reorganize.png
+-rw-r--r--   0 simon      (501) staff       (20)     4784 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/browse.png
+-rw-r--r--   0 simon      (501) staff       (20)    30707 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/SimBA_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/ethovision.png
+-rw-r--r--   0 simon      (501) staff       (20)     1018 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/icons/close.png
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/dash_simba_base.css
+-rw-r--r--   0 simon      (501) staff       (20)    31812 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.89.8/simba/assets/TheGoldenLab.PNG
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 20:23:19.000000 Simba-UW-tf-dev-1.89.8/Simba_UW_tf_dev.egg-info/
+-rw-r--r--   0 simon      (501) staff       (20)     2797 2024-04-12 20:23:19.000000 Simba-UW-tf-dev-1.89.8/Simba_UW_tf_dev.egg-info/PKG-INFO
+-rw-r--r--   0 simon      (501) staff       (20)    23084 2024-04-12 20:23:19.000000 Simba-UW-tf-dev-1.89.8/Simba_UW_tf_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 simon      (501) staff       (20)       44 2024-04-12 20:23:19.000000 Simba-UW-tf-dev-1.89.8/Simba_UW_tf_dev.egg-info/entry_points.txt
+-rw-r--r--   0 simon      (501) staff       (20)      797 2024-04-12 20:23:19.000000 Simba-UW-tf-dev-1.89.8/Simba_UW_tf_dev.egg-info/requires.txt
+-rw-r--r--   0 simon      (501) staff       (20)        6 2024-04-12 20:23:19.000000 Simba-UW-tf-dev-1.89.8/Simba_UW_tf_dev.egg-info/top_level.txt
+-rw-r--r--   0 simon      (501) staff       (20)        1 2024-04-12 20:23:19.000000 Simba-UW-tf-dev-1.89.8/Simba_UW_tf_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 simon      (501) staff       (20)    35127 2024-02-07 18:56:10.000000 Simba-UW-tf-dev-1.89.8/LICENSE
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-12 20:23:20.000000 Simba-UW-tf-dev-1.89.8/tests/
+-rw-r--r--   0 simon      (501) staff       (20)     4753 2024-04-11 20:40:04.000000 Simba-UW-tf-dev-1.89.8/tests/test_data_processors.py
+-rw-r--r--   0 simon      (501) staff       (20)    13415 2024-03-01 16:43:04.000000 Simba-UW-tf-dev-1.89.8/tests/test_circlular_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)    13399 2024-04-11 20:36:51.000000 Simba-UW-tf-dev-1.89.8/tests/test_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)     5374 2024-04-11 22:48:09.000000 Simba-UW-tf-dev-1.89.8/tests/test_distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    11863 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.89.8/tests/test_train_model_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     6525 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.89.8/tests/test_feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     1739 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.89.8/tests/test_utils_data.py
+-rw-r--r--   0 simon      (501) staff       (20)     8120 2024-03-01 19:06:25.000000 Simba-UW-tf-dev-1.89.8/tests/test_config_reader_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     1070 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.89.8/tests/test_outlier_correctors.py
+-rw-r--r--   0 simon      (501) staff       (20)     4435 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.89.8/tests/test_visualize_directing_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)     1596 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.89.8/tests/test_featurizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     8570 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.89.8/tests/test_video_processors.py
+-rw-r--r--   0 simon      (501) staff       (20)     3554 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.89.8/tests/test_thirdparty_appenders.py
+-rw-r--r--   0 simon      (501) staff       (20)     3021 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.89.8/tests/test_validation_clips.py
+-rw-r--r--   0 simon      (501) staff       (20)     3992 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.89.8/tests/test_roi_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)      318 2024-03-04 20:16:28.000000 Simba-UW-tf-dev-1.89.8/MANIFEST.in
+-rw-r--r--   0 simon      (501) staff       (20)    18403 2024-02-12 00:49:21.000000 Simba-UW-tf-dev-1.89.8/README.md
+-rw-r--r--   0 simon      (501) staff       (20)     1426 2024-04-12 20:23:17.000000 Simba-UW-tf-dev-1.89.8/setup.py
+-rw-r--r--   0 simon      (501) staff       (20)       38 2024-04-12 20:23:20.000000 Simba-UW-tf-dev-1.89.8/setup.cfg
```

### Comparing `Simba-UW-tf-dev-1.89.7/PKG-INFO` & `Simba-UW-tf-dev-1.89.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.89.7
+Version: 1.89.8
 Summary: Toolkit for computer classification of behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/.DS_Store` & `Simba-UW-tf-dev-1.89.8/simba/ui/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/mutual_exclusivity_pop_up.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/mutual_exclusivity_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/csv_2_parquet_pop_up.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/csv_2_parquet_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/quick_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/quick_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/batch_preprocess_pop_up.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/batch_preprocess_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/heatmap_location_pop_up.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/heatmap_location_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/clf_probability_plot_pop_up.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/clf_probability_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/movement_analysis_pop_up.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/movement_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/clf_plot_pop_up.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/clf_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/path_plot_pop_up.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/remove_roi_features_pop_up.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/remove_roi_features_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/targeted_annotation_clips_pop_up.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/targeted_annotation_clips_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/smoothing_interpolation_pop_up.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/smoothing_interpolation_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/roi_size_standardizer_popup.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/roi_size_standardizer_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/roi_analysis_pop_up.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/roi_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/outlier_settings_pop_up.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/outlier_settings_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/gantt_pop_up.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/gantt_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/clf_validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/clf_validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/severity_analysis_pop_up.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/severity_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/fsttc_pop_up.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/fsttc_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/kleinberg_pop_up.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/kleinberg_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/spontaneous_alternation_pop_up.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/spontaneous_alternation_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/pose_reorganizer_pop_up.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/pose_reorganizer_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/animal_directing_other_animals_pop_up.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/animal_directing_other_animals_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/append_roi_features_animals_pop_up.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/append_roi_features_animals_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/clf_by_timebins_pop_up.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/clf_by_timebins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/heatmap_clf_pop_up.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/heatmap_clf_pop_up.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,26 +14,27 @@
 from simba.utils.checks import check_if_filepath_list_is_empty
 from simba.utils.enums import Formats, Keys, Links, Paths
 from simba.utils.read_write import get_file_name_info_in_directory
 
 
 class HeatmapClfPopUp(PopUpMixin, ConfigReader):
     def __init__(self, config_path: str):
-        PopUpMixin.__init__(self, title="CREATE CLASSIFICATION HEATMAP PLOTS")
-        ConfigReader.__init__(self, config_path=config_path)
+
         self.data_path = os.path.join(
             self.project_path, Paths.MACHINE_RESULTS_DIR.value
         )
         self.files_found_dict = get_file_name_info_in_directory(
             directory=self.data_path, file_type=self.file_type
         )
         check_if_filepath_list_is_empty(
             filepaths=list(self.files_found_dict.keys()),
             error_msg="SIMBA ERROR: Zero files found in the project_folder/csv/machine_results directory. ",
         )
+        PopUpMixin.__init__(self, title="CREATE CLASSIFICATION HEATMAP PLOTS")
+        ConfigReader.__init__(self, config_path=config_path)
         max_scales = list(np.linspace(5, 600, 5))
         max_scales.insert(0, "Auto-compute")
 
         self.style_settings_frm = CreateLabelFrameWithIcon(
             parent=self.main_frm,
             header="STYLE SETTINGS",
             icon_name=Keys.DOCUMENTATION.value,
```

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/data_plot_pop_up.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/data_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/roi_features_plot_pop_up.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/roi_features_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/pup_retrieval_pop_up.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/pup_retrieval_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/boolean_conditional_slicer_pup_up.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/boolean_conditional_slicer_pup_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/about_simba_pop_up.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/about_simba_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/roi_tracking_plot_pop_up.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/roi_tracking_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/directing_animal_to_bodypart_plot_pop_up.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/directing_animal_to_bodypart_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/clf_add_remove_print_pop_up.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/clf_add_remove_print_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/video_processing_pop_up.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/video_processing_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/clf_by_roi_pop_up.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/clf_by_roi_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/make_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/make_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/direction_animal_to_bodypart_settings_pop_up.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/direction_animal_to_bodypart_settings_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/archive_files_pop_up.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/archive_files_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/pose_bp_drop_pop_up.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/pose_bp_drop_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/distance_plot_pop_up.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/distance_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/subset_feature_extractor_pop_up.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/subset_feature_extractor_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/video_info_ui.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/video_info_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/user_defined_pose_creator.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/user_defined_pose_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/create_project_ui.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/create_project_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/tkinter_functions.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/tkinter_functions.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/ui/machine_model_settings_ui.py` & `Simba-UW-tf-dev-1.89.8/simba/ui/machine_model_settings_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/labelling/labelling_interface.py` & `Simba-UW-tf-dev-1.89.8/simba/labelling/labelling_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/labelling/targeted_annotations_clips.py` & `Simba-UW-tf-dev-1.89.8/simba/labelling/targeted_annotations_clips.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/labelling/extract_labelled_frames.py` & `Simba-UW-tf-dev-1.89.8/simba/labelling/extract_labelled_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/labelling/labelling_advanced_interface.py` & `Simba-UW-tf-dev-1.89.8/simba/labelling/labelling_advanced_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/labelling/play_annotation_video.py` & `Simba-UW-tf-dev-1.89.8/simba/labelling/play_annotation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/unsupervised/dbcv_calculator.py` & `Simba-UW-tf-dev-1.89.8/simba/unsupervised/dbcv_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/unsupervised/cluster_validation_calculator.py` & `Simba-UW-tf-dev-1.89.8/simba/unsupervised/cluster_validation_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/unsupervised/enums.py` & `Simba-UW-tf-dev-1.89.8/simba/unsupervised/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.89.8/simba/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/unsupervised/cluster_video_visualizer.py` & `Simba-UW-tf-dev-1.89.8/simba/unsupervised/cluster_video_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/unsupervised/pop_ups/cluster_videos_popup.py` & `Simba-UW-tf-dev-1.89.8/simba/unsupervised/pop_ups/cluster_videos_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/unsupervised/pop_ups/transform_cluster_popup.py` & `Simba-UW-tf-dev-1.89.8/simba/unsupervised/pop_ups/transform_cluster_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/unsupervised/pop_ups/embedding_correlations_popup.py` & `Simba-UW-tf-dev-1.89.8/simba/unsupervised/pop_ups/embedding_correlations_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/unsupervised/pop_ups/.DS_Store` & `Simba-UW-tf-dev-1.89.8/simba/unsupervised/pop_ups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/unsupervised/pop_ups/transform_dim_reduction_popup.py` & `Simba-UW-tf-dev-1.89.8/simba/unsupervised/pop_ups/transform_dim_reduction_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/unsupervised/pop_ups/fit_dim_reduction_popup.py` & `Simba-UW-tf-dev-1.89.8/simba/unsupervised/pop_ups/fit_dim_reduction_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/unsupervised/pop_ups/data_extractor_popup.py` & `Simba-UW-tf-dev-1.89.8/simba/unsupervised/pop_ups/data_extractor_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/unsupervised/pop_ups/cluster_validation_pop_up.py` & `Simba-UW-tf-dev-1.89.8/simba/unsupervised/pop_ups/cluster_validation_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/unsupervised/pop_ups/fit_cluster_popup.py` & `Simba-UW-tf-dev-1.89.8/simba/unsupervised/pop_ups/fit_cluster_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/unsupervised/pop_ups/clusterer_comparison_popup.py` & `Simba-UW-tf-dev-1.89.8/simba/unsupervised/pop_ups/clusterer_comparison_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/unsupervised/pop_ups/grid_search_visualizer_popup.py` & `Simba-UW-tf-dev-1.89.8/simba/unsupervised/pop_ups/grid_search_visualizer_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/unsupervised/pop_ups/cluster_xai_popup.py` & `Simba-UW-tf-dev-1.89.8/simba/unsupervised/pop_ups/cluster_xai_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/unsupervised/pop_ups/cluster_frequentist_stats_popup.py` & `Simba-UW-tf-dev-1.89.8/simba/unsupervised/pop_ups/cluster_frequentist_stats_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/unsupervised/pop_ups/print_embedding_info_popup.py` & `Simba-UW-tf-dev-1.89.8/simba/unsupervised/pop_ups/print_embedding_info_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/unsupervised/dataset_creator.py` & `Simba-UW-tf-dev-1.89.8/simba/unsupervised/dataset_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/unsupervised/unsupervised_main.py` & `Simba-UW-tf-dev-1.89.8/simba/unsupervised/unsupervised_main.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/unsupervised/grid_search_visualizers.py` & `Simba-UW-tf-dev-1.89.8/simba/unsupervised/grid_search_visualizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/unsupervised/data_extractor.py` & `Simba-UW-tf-dev-1.89.8/simba/unsupervised/data_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/unsupervised/outlier_detector.py` & `Simba-UW-tf-dev-1.89.8/simba/unsupervised/outlier_detector.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/unsupervised/cluster_frequentist_calculator.py` & `Simba-UW-tf-dev-1.89.8/simba/unsupervised/cluster_frequentist_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/unsupervised/embedding_correlation_calculator.py` & `Simba-UW-tf-dev-1.89.8/simba/unsupervised/embedding_correlation_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/unsupervised/cluster_xai_calculator.py` & `Simba-UW-tf-dev-1.89.8/simba/unsupervised/cluster_xai_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/unsupervised/umap_embedder.py` & `Simba-UW-tf-dev-1.89.8/simba/unsupervised/umap_embedder.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/unsupervised/clusterer_comparison_calculator.py` & `Simba-UW-tf-dev-1.89.8/simba/unsupervised/clusterer_comparison_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/unsupervised/bout_aggregator.py` & `Simba-UW-tf-dev-1.89.8/simba/unsupervised/bout_aggregator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/unsupervised/data_map.yaml` & `Simba-UW-tf-dev-1.89.8/simba/unsupervised/data_map.yaml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/unsupervised/hdbscan_clusterer.py` & `Simba-UW-tf-dev-1.89.8/simba/unsupervised/hdbscan_clusterer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/unsupervised/tsne.py` & `Simba-UW-tf-dev-1.89.8/simba/unsupervised/tsne.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/bounding_box_tools/agg_boundary_stats.py` & `Simba-UW-tf-dev-1.89.8/simba/bounding_box_tools/agg_boundary_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/bounding_box_tools/boundary_menus.py` & `Simba-UW-tf-dev-1.89.8/simba/bounding_box_tools/boundary_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/bounding_box_tools/boundary_statistics.py` & `Simba-UW-tf-dev-1.89.8/simba/bounding_box_tools/boundary_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/bounding_box_tools/find_boundaries.py` & `Simba-UW-tf-dev-1.89.8/simba/bounding_box_tools/find_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/bounding_box_tools/visualize_boundaries.py` & `Simba-UW-tf-dev-1.89.8/simba/bounding_box_tools/visualize_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/.DS_Store` & `Simba-UW-tf-dev-1.89.8/simba/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/feature_extractors/feature_extractor_14bp.py` & `Simba-UW-tf-dev-1.89.8/simba/feature_extractors/feature_extractor_14bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/feature_extractors/feature_extractor_7bp.py` & `Simba-UW-tf-dev-1.89.8/simba/feature_extractors/feature_extractor_7bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/feature_extractors/misc/doctests.py` & `Simba-UW-tf-dev-1.89.8/simba/feature_extractors/misc/doctests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py` & `Simba-UW-tf-dev-1.89.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/feature_extractors/misc/read_in_mp.py` & `Simba-UW-tf-dev-1.89.8/simba/feature_extractors/misc/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/feature_extractors/misc/peaks.py` & `Simba-UW-tf-dev-1.89.8/simba/feature_extractors/misc/peaks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/feature_extractors/misc/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.89.8/simba/feature_extractors/misc/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/feature_extractors/misc/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.89.8/simba/feature_extractors/misc/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/feature_extractors/misc/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.89.8/simba/feature_extractors/misc/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py` & `Simba-UW-tf-dev-1.89.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/feature_extractors/misc/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.89.8/simba/feature_extractors/misc/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/feature_extractors/misc/count_values_in_range.py` & `Simba-UW-tf-dev-1.89.8/simba/feature_extractors/misc/count_values_in_range.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/feature_extractors/misc/graph_creator.py` & `Simba-UW-tf-dev-1.89.8/simba/feature_extractors/misc/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/feature_extractors/misc/termite_rois.csv` & `Simba-UW-tf-dev-1.89.8/simba/feature_extractors/misc/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/feature_extractors/misc/mutual_exclusive.py` & `Simba-UW-tf-dev-1.89.8/simba/feature_extractors/misc/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/feature_extractors/misc/video_color.py` & `Simba-UW-tf-dev-1.89.8/simba/feature_extractors/misc/video_color.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/feature_extractors/misc/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.89.8/simba/feature_extractors/misc/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/feature_extractors/misc/video_rotator.py` & `Simba-UW-tf-dev-1.89.8/simba/feature_extractors/misc/video_rotator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/feature_extractors/misc/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.89.8/simba/feature_extractors/misc/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/feature_extractors/misc/make_splash.py` & `Simba-UW-tf-dev-1.89.8/simba/feature_extractors/misc/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py` & `Simba-UW-tf-dev-1.89.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/feature_extractors/misc/time_stamp_calculator.py` & `Simba-UW-tf-dev-1.89.8/simba/feature_extractors/misc/time_stamp_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/feature_extractors/misc/video_rotator_mp.py` & `Simba-UW-tf-dev-1.89.8/simba/feature_extractors/misc/video_rotator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py` & `Simba-UW-tf-dev-1.89.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/feature_extractors/misc/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.89.8/simba/feature_extractors/misc/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/feature_extractors/feature_extractor_8bps_2_animals.py` & `Simba-UW-tf-dev-1.89.8/simba/feature_extractors/feature_extractor_8bps_2_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/feature_extractors/.DS_Store` & `Simba-UW-tf-dev-1.89.8/simba/feature_extractors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/feature_extractors/perimeter_jit.py` & `Simba-UW-tf-dev-1.89.8/simba/feature_extractors/perimeter_jit.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/feature_extractors/feature_subsets.py` & `Simba-UW-tf-dev-1.89.8/simba/feature_extractors/feature_subsets.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/feature_extractors/feature_extractor_user_defined.py` & `Simba-UW-tf-dev-1.89.8/simba/feature_extractors/feature_extractor_user_defined.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/feature_extractors/feature_extractor_16bp.py` & `Simba-UW-tf-dev-1.89.8/simba/feature_extractors/feature_extractor_16bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/feature_extractors/feature_extractor_9bp.py` & `Simba-UW-tf-dev-1.89.8/simba/feature_extractors/feature_extractor_9bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/feature_extractors/feature_extractor_8bp.py` & `Simba-UW-tf-dev-1.89.8/simba/feature_extractors/feature_extractor_8bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/feature_extractors/feature_extractor_4bp.py` & `Simba-UW-tf-dev-1.89.8/simba/feature_extractors/feature_extractor_4bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/feature_extractors/amber_feature_extractor.py` & `Simba-UW-tf-dev-1.89.8/simba/feature_extractors/amber_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/requirements.txt` & `Simba-UW-tf-dev-1.89.8/simba/requirements.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/mixins/annotator_mixin.py` & `Simba-UW-tf-dev-1.89.8/simba/mixins/annotator_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/mixins/timeseries_features_mixin.py` & `Simba-UW-tf-dev-1.89.8/simba/mixins/timeseries_features_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/mixins/.DS_Store` & `Simba-UW-tf-dev-1.89.8/simba/mixins/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/mixins/pop_up_mixin.py` & `Simba-UW-tf-dev-1.89.8/simba/mixins/pop_up_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/mixins/config_reader.py` & `Simba-UW-tf-dev-1.89.8/simba/mixins/config_reader.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/mixins/circular_statistics.py` & `Simba-UW-tf-dev-1.89.8/simba/mixins/circular_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/mixins/network_mixin.py` & `Simba-UW-tf-dev-1.89.8/simba/mixins/network_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/mixins/pose_importer_mixin.py` & `Simba-UW-tf-dev-1.89.8/simba/mixins/pose_importer_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/mixins/video_processing_mixin.py` & `Simba-UW-tf-dev-1.89.8/simba/mixins/video_processing_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/mixins/feature_extraction_supplement_mixin.py` & `Simba-UW-tf-dev-1.89.8/simba/mixins/feature_extraction_supplement_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/mixins/statistics_mixin.py` & `Simba-UW-tf-dev-1.89.8/simba/mixins/statistics_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.89.8/simba/mixins/feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/mixins/plotting_mixin.py` & `Simba-UW-tf-dev-1.89.8/simba/mixins/plotting_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 __author__ = "Simon Nilsson"
-
 import io
 import itertools
 import os
 import random
 import shutil
 from typing import Any, Dict, List, Optional, Tuple, Union
 
@@ -1231,15 +1230,15 @@
     ):
 
         group, frame_rng = data[0], data[1:]
         start_frm, end_frm, current_frm = frame_rng[0], frame_rng[-1], frame_rng[0]
         video_writer = None
         if video_setting:
             fourcc = cv2.VideoWriter_fourcc(*Formats.MP4_CODEC.value)
-            video_save_path = os.path.join(video_save_dir, "{}.mp4".format(str(group)))
+            video_save_path = os.path.join(video_save_dir, f"{group}.mp4")
             video_writer = cv2.VideoWriter(
                 video_save_path, fourcc, fps, (width, height)
             )
 
         while current_frm < end_frm:
             fig, ax = plt.subplots()
             bout_rows = bouts_df.loc[bouts_df["End_frame"] <= current_frm]
```

### Comparing `Simba-UW-tf-dev-1.89.7/simba/mixins/image_mixin.py` & `Simba-UW-tf-dev-1.89.8/simba/mixins/image_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/mixins/unsupervised_mixin.py` & `Simba-UW-tf-dev-1.89.8/simba/mixins/unsupervised_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/mixins/train_model_mixin.py` & `Simba-UW-tf-dev-1.89.8/simba/mixins/train_model_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/mixins/geometry_mixin.py` & `Simba-UW-tf-dev-1.89.8/simba/mixins/geometry_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/mixins/feature_extraction_circular_mixin.py` & `Simba-UW-tf-dev-1.89.8/simba/mixins/feature_extraction_circular_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/third_party_label_appenders/deepethogram_importer.py` & `Simba-UW-tf-dev-1.89.8/simba/third_party_label_appenders/deepethogram_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/third_party_label_appenders/BORIS_appender.py` & `Simba-UW-tf-dev-1.89.8/simba/third_party_label_appenders/BORIS_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/third_party_label_appenders/observer_importer.py` & `Simba-UW-tf-dev-1.89.8/simba/third_party_label_appenders/observer_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/third_party_label_appenders/.DS_Store` & `Simba-UW-tf-dev-1.89.8/simba/third_party_label_appenders/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/third_party_label_appenders/boris_source_cleaner.py` & `Simba-UW-tf-dev-1.89.8/simba/third_party_label_appenders/boris_source_cleaner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/third_party_label_appenders/tools.py` & `Simba-UW-tf-dev-1.89.8/simba/third_party_label_appenders/tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/third_party_label_appenders/third_party_appender.py` & `Simba-UW-tf-dev-1.89.8/simba/third_party_label_appenders/third_party_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/third_party_label_appenders/ethovision_import.py` & `Simba-UW-tf-dev-1.89.8/simba/third_party_label_appenders/ethovision_import.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/third_party_label_appenders/BENTO_appender.py` & `Simba-UW-tf-dev-1.89.8/simba/third_party_label_appenders/BENTO_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/third_party_label_appenders/solomon_importer.py` & `Simba-UW-tf-dev-1.89.8/simba/third_party_label_appenders/solomon_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/cue_light_tools/cue_light_clf_statistics.py` & `Simba-UW-tf-dev-1.89.8/simba/cue_light_tools/cue_light_clf_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/cue_light_tools/cue_light_analyzer.py` & `Simba-UW-tf-dev-1.89.8/simba/cue_light_tools/cue_light_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/cue_light_tools/cue_light_menues.py` & `Simba-UW-tf-dev-1.89.8/simba/cue_light_tools/cue_light_menues.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/cue_light_tools/cue_light_tools.py` & `Simba-UW-tf-dev-1.89.8/simba/cue_light_tools/cue_light_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/cue_light_tools/cue_light_visualizer.py` & `Simba-UW-tf-dev-1.89.8/simba/cue_light_tools/cue_light_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/cue_light_tools/cue_light_movement_statistics.py` & `Simba-UW-tf-dev-1.89.8/simba/cue_light_tools/cue_light_movement_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/utils/config_creator.py` & `Simba-UW-tf-dev-1.89.8/simba/utils/config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/utils/enums.py` & `Simba-UW-tf-dev-1.89.8/simba/utils/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/utils/custom_feature_extractor.py` & `Simba-UW-tf-dev-1.89.8/simba/utils/custom_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/utils/.DS_Store` & `Simba-UW-tf-dev-1.89.8/simba/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/utils/warnings.py` & `Simba-UW-tf-dev-1.89.8/simba/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/utils/checks.py` & `Simba-UW-tf-dev-1.89.8/simba/utils/checks.py`

 * *Files 1% similar despite different names*

```diff
@@ -300,26 +300,30 @@
             missing_videos.append(video_name)
     if len(missing_videos) > 0:
         raise ParametersFileError(
             msg=f"SimBA could not find {len(missing_videos)} video(s) in the video_info.csv file. Make sure all videos analyzed are represented in the project_folder/logs/video_info.csv file. MISSING VIDEOS: {missing_videos}"
         )
 
 
-def check_if_dir_exists(
-    in_dir: Union[str, os.PathLike], source: Optional[str] = None
-) -> None:
+def check_if_dir_exists(in_dir: Union[str, os.PathLike], source: Optional[str] = None, create_if_not_exist: Optional[bool] = False) -> None:
     """
     Check if a directory path exists.
 
     :param Union[str, os.PathLike] in_dir: Putative directory path.
-    :param str source: String source for interpretable error messaging.
+    :param Optional[str] source: String source for interpretable error messaging.
+    :param Optional[bool] create_if_not_exist: If directory does not exist, then create it. Default False,
     :raise NotDirectoryError: The directory does not exist.
     """
 
     if not os.path.isdir(in_dir):
+        if create_if_not_exist:
+            try:
+                os.makedirs(in_dir)
+            except:
+                pass
         if source is None:
             raise NotDirectoryError(
                 msg=f"{in_dir} is not a valid directory",
                 source=check_if_dir_exists.__name__,
             )
         else:
             raise NotDirectoryError(
```

### Comparing `Simba-UW-tf-dev-1.89.7/simba/utils/read_write.py` & `Simba-UW-tf-dev-1.89.8/simba/utils/read_write.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/utils/lookups.py` & `Simba-UW-tf-dev-1.89.8/simba/utils/lookups.py`

 * *Files 0% similar despite different names*

```diff
@@ -433,15 +433,14 @@
 
 def percent_to_crf_lookup() -> Dict[str, int]:
     """
     Create dictionary that matches human-readable percent values to FFmpeg Constant Rate Factor (CRF)
     values that regulates video quality in CPU codecs. Higher CRF values translates to lower video quality and reduced
     file sizes.
     """
-
     return {
         "10": 37,
         "20": 34,
         "30": 31,
         "40": 28,
         "50": 25,
         "60": 22,
```

### Comparing `Simba-UW-tf-dev-1.89.7/simba/utils/cli/cli_tools.py` & `Simba-UW-tf-dev-1.89.8/simba/utils/cli/cli_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/utils/errors.py` & `Simba-UW-tf-dev-1.89.8/simba/utils/errors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/utils/data.py` & `Simba-UW-tf-dev-1.89.8/simba/utils/data.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/utils/keyboard_listener.py` & `Simba-UW-tf-dev-1.89.8/simba/utils/keyboard_listener.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/utils/printing.py` & `Simba-UW-tf-dev-1.89.8/simba/utils/printing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/SimBA_logo.ico` & `Simba-UW-tf-dev-1.89.8/simba/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/pose_processors/reorganize_keypoint.py` & `Simba-UW-tf-dev-1.89.8/simba/pose_processors/reorganize_keypoint.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/pose_processors/remove_keypoints.py` & `Simba-UW-tf-dev-1.89.8/simba/pose_processors/remove_keypoints.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/pose_processors/pose_reset.py` & `Simba-UW-tf-dev-1.89.8/simba/pose_processors/pose_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/pose_processors/reverse_pose.py` & `Simba-UW-tf-dev-1.89.8/simba/pose_processors/reverse_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/doctests.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/doctests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/fish_feature_extractor_2023_version_3.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/fish_feature_extractor_2023_version_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/dprime.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/dprime.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/linear_fretchet.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/linear_fretchet.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/read_in_mp.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/piotr_120324 3.py.zip` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/piotr_120324 3.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/dunn_index.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/dunn_index.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/hausdorff.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/hausdorff.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/peaks.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/peaks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/colinear_features.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/colinear_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/spontaneous_alternation_calculator.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/spontaneous_alternation_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/horizontal_videos_concat.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/horizontal_videos_concat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/silhouette_score.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/silhouette_score.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/two_fish_feature_extractor_040924.py.zip` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/two_fish_feature_extractor_040924.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/cuda_jit.ipynb` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/cuda_jit.ipynb`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/directed_hausdorff.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/directed_hausdorff.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/shannon_diversity_index.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/shannon_diversity_index.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/sequential_lag_analysis.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/sequential_lag_analysis.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/wilcoxon.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/wilcoxon.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/.DS_Store` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/data.npy` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/data.npy`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/distances.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/distances.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/fish_feature_extractor_2023_version_2.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/fish_feature_extractor_2023_version_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/cohens_kappa.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/cohens_kappa.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/paths.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/paths.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/outliers_tietjen.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/outliers_tietjen.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/train_model.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/train_model.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/amber_tests.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/amber_tests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/line_locate_point.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/line_locate_point.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/multifrm_to_points.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/multifrm_to_points.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/two_fish_feature_extractor_040924.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/two_fish_feature_extractor_040924.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/add_body_part.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/add_body_part.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/grubbs_test.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/grubbs_test.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/slide_circ_mean.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/slide_circ_mean.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/calinski_harabasz.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/calinski_harabasz.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/roi_feature_visualizer_example.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/roi_feature_visualizer_example.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/spontaneuous_alternation_plotter.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/spontaneuous_alternation_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/runs_test.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/runs_test.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/pct_counts_in_top_N.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/pct_counts_in_top_N.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/total_variation_distance.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/total_variation_distance.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/crop_single_polygon.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/crop_single_polygon.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/joint_plotter.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/joint_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/elliptic_envelope.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/elliptic_envelope.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/roi_definition_csvs_to_h5.py.zip` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/roi_definition_csvs_to_h5.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/add_body_part.py.zip` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/add_body_part.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/roi_feature_visualizer_example.py.zip` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/roi_feature_visualizer_example.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/sliding_crosscorrelation.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/sliding_crosscorrelation.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/count_values_in_range.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/count_values_in_range.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/roi_definition_csvs_to_h5.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/roi_definition_csvs_to_h5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/distance_velocity.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/distance_velocity.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/graph_creator.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/line_plot_plotly.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/line_plot_plotly.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/termite_rois.csv` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/unsupervised_lof.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/unsupervised_lof.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/siegel_tukey.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/siegel_tukey.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/berger_parker.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/berger_parker.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/isolation_forest.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/isolation_forest.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/davis_bouldin.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/davis_bouldin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/vertical_video_concatenator.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/vertical_video_concatenator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/batch_video_to_greyscale.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/batch_video_to_greyscale.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/crop_circles_pop_up.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/crop_circles_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/heading.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/heading.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/piotr_120324 2.py.zip` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/piotr_120324 2.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/mutual_exclusive.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/grangercausalitytests.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/grangercausalitytests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/multiframe_is_shape_covered.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/multiframe_is_shape_covered.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/redis.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/redis.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/video_color.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/video_color.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/piotr_120324.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/piotr_120324.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/video_rotator.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/video_rotator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/hartley_fmax.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/hartley_fmax.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/fix_clahe.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/fix_clahe.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/cochran_q.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/cochran_q.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/menhinicks_index.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/menhinicks_index.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/spontanous_alternations.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/spontanous_alternations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/piotr_120324.py.zip` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/piotr_120324.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/velocity_aggregator.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/velocity_aggregator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/make_splash.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/abod.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/abod.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/fish_feature_extractor_2023_version_5.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/fish_feature_extractor_2023_version_5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/simpson_diversity_index.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/simpson_diversity_index.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/piotr_120324 4.py.zip` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/piotr_120324 4.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/geometry_ex.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/geometry_ex.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/time_stamp_calculator.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/time_stamp_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/line_plot.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/line_plot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/video_rotator_mp.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/video_rotator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/unsupervised_outliers.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/unsupervised_outliers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/statistics_ex.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/statistics_ex.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/sliding_displacement.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/sliding_displacement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/wald_wolfowitz.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/wald_wolfowitz.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/sliding_autoc.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/sliding_autoc.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/linestring_path.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/linestring_path.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/cronbach_alpha.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/cronbach_alpha.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/mcnamar.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/mcnamar.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/fish_feature_extractor_2023_version_4.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/fish_feature_extractor_2023_version_4.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/AmberFeatureExtractor.py.zip` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/AmberFeatureExtractor.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/mosaic.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/mosaic.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/amber_featurizer.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/amber_featurizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/margalef_diversification_index.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/margalef_diversification_index.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/biweight_midcorrelation.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/biweight_midcorrelation.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/madmedianrule.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/madmedianrule.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/adjusted_rand_score.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/adjusted_rand_score.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/sandbox/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.89.8/simba/sandbox/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/plotting/directing_animals_to_bodypart_visualizer.py` & `Simba-UW-tf-dev-1.89.8/simba/plotting/directing_animals_to_bodypart_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/plotting/gantt_creator.py` & `Simba-UW-tf-dev-1.89.8/simba/plotting/gantt_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/plotting/tools/tkinter_tools.py` & `Simba-UW-tf-dev-1.89.8/simba/plotting/tools/tkinter_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/plotting/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.89.8/simba/plotting/ROI_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/plotting/.DS_Store` & `Simba-UW-tf-dev-1.89.8/simba/plotting/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/plotting/shap_agg_stats_visualizer.py` & `Simba-UW-tf-dev-1.89.8/simba/plotting/shap_agg_stats_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/plotting/gantt_creator_mp.py` & `Simba-UW-tf-dev-1.89.8/simba/plotting/gantt_creator_mp.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 __author__ = "Simon Nilsson"
 
 import warnings
-
 warnings.simplefilter(action="ignore", category=FutureWarning)
 import functools
+import platform
 import multiprocessing
 import os
-import platform
 import shutil
-from typing import Dict, List
-
-import cv2
+from typing import Dict, List, Union, Optional
 import numpy as np
 
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.plotting_mixin import PlottingMixin
-from simba.utils.checks import check_if_filepath_list_is_empty
+from simba.utils.checks import (check_if_filepath_list_is_empty,
+                                check_file_exist_and_readable,
+                                check_int,
+                                check_if_keys_exist_in_dict,
+                                check_that_column_exist,
+                                check_all_file_names_are_represented_in_video_log)
 from simba.utils.data import detect_bouts
 from simba.utils.enums import Formats
 from simba.utils.errors import NoSpecifiedOutputError
 from simba.utils.lookups import get_named_colors
 from simba.utils.printing import SimbaTimer, stdout_success
-from simba.utils.read_write import (concatenate_videos_in_folder, get_fn_ext,
-                                    read_df)
+from simba.utils.read_write import (concatenate_videos_in_folder, get_fn_ext, read_df, find_core_cnt)
 
+HEIGHT = 'height'
+WIDTH = 'width'
+FONT_ROTATION = 'font rotation'
+FONT_SIZE = 'font size'
+STYLE_KEYS = [HEIGHT, WIDTH, FONT_ROTATION, FONT_SIZE]
 
 class GanttCreatorMultiprocess(ConfigReader, PlottingMixin):
     """
     Multiprocess creation of classifier gantt charts in video and/or image format.
     See meth:`simba.gantt_creator.GanttCreatorSingleProcess` for single-process class.
 
     ..note::
@@ -41,181 +47,105 @@
     :param bool frame_setting: If True, creates individual frames.
     :param bool last_frm_setting: If True, creates single .png image representing entire video.
     :param bool video_setting: If True, creates videos
     :param dict style_attr: Attributes of gannt chart (size, font size, font rotation etc).
     :param List[str] files_found: File paths representing files with machine predictions e.g., ['project_folder/csv/machine_results/My_results.csv']
     :param int cores: Number of cores to use.
 
-    Examples
-    ----------
+    :examples:
     >>> gantt_creator = GanttCreatorMultiprocess(config_path='project_folder/project_config.ini', frame_setting=False, video_setting=True, files_found=['project_folder/csv/machine_results/Together_1.csv'], cores=5, style_attr={'width': 640, 'height': 480, 'font size': 8, 'font rotation': 45}).run()
-
     """
 
-    def __init__(
-        self,
-        config_path: str,
-        frame_setting: bool,
-        video_setting: bool,
-        files_found: List[str],
-        cores: int,
-        style_attr: Dict[str, int],
-        last_frm_setting: bool,
-    ):
-        if platform.system() == "Darwin":
-            multiprocessing.set_start_method("spawn", force=True)
+    def __init__(self,
+                 config_path: Union[str, os.PathLike],
+                 style_attr: Dict[str, int],
+                 files_found: List[Union[str, os.PathLike]],
+                 frame_setting: Optional[bool] = False,
+                 video_setting: Optional[bool] = False,
+                 last_frm_setting: Optional[bool] = True,
+                 cores: Optional[int] = -1):
+
+        check_file_exist_and_readable(file_path=config_path)
+        if (not frame_setting) and (not video_setting) and (not last_frm_setting):
+            raise NoSpecifiedOutputError(msg="SIMBA ERROR: Please select gantt videos, frames, and/or last frame.", source=self.__class__.__name__)
+        check_if_filepath_list_is_empty(filepaths=files_found, error_msg="SIMBA ERROR: Zero files found in the project_folder/csv/machine_results directory. Create classification results before visualizing gantt charts")
+        check_int(name=f"{self.__class__.__name__} core_cnt", value=cores, min_value=-1, max_value=find_core_cnt()[0])
+        if cores == -1: cores = find_core_cnt()[0]
+
 
         ConfigReader.__init__(self, config_path=config_path)
         PlottingMixin.__init__(self)
 
-        (
-            self.frame_setting,
-            self.video_setting,
-            self.files_found,
-            self.style_attr,
-            self.cores,
-            self.last_frm_setting,
-        ) = (
-            frame_setting,
-            video_setting,
-            files_found,
-            style_attr,
-            cores,
-            last_frm_setting,
-        )
-        if (
-            (not self.frame_setting)
-            and (not self.video_setting)
-            and (not self.last_frm_setting)
-        ):
-            raise NoSpecifiedOutputError(
-                msg="SIMBA ERROR: Please select gantt videos, frames, and/or last frame."
-            )
-        check_if_filepath_list_is_empty(
-            filepaths=self.files_found,
-            error_msg="SIMBA ERROR: Zero files found in the project_folder/csv/machine_results directory. Create classification results before visualizing gantt charts",
-        )
+        self.frame_setting, self.video_setting, self.files_found, self.style_attr, self.cores, self.last_frm_setting = frame_setting, video_setting, files_found, style_attr, cores, last_frm_setting
+        if not os.path.exists(self.gantt_plot_dir): os.makedirs(self.gantt_plot_dir)
+        check_if_keys_exist_in_dict(data=style_attr, key=STYLE_KEYS, name=f'{self.__class__.__name__} style_attr')
+        self.y_rotation, self.y_fontsize = (self.style_attr["font rotation"], self.style_attr["font size"])
+        self.out_width, self.out_height = (self.style_attr["width"], self.style_attr["height"])
         self.colours = get_named_colors()[:-1]
         self.colour_tuple_x = list(np.arange(3.5, 203.5, 5))
-        if not os.path.exists(self.gantt_plot_dir):
-            os.makedirs(self.gantt_plot_dir)
-        self.y_rotation, self.y_fontsize = (
-            self.style_attr["font rotation"],
-            self.style_attr["font size"],
-        )
-        self.fourcc = cv2.VideoWriter_fourcc(*Formats.MP4_CODEC.value)
-        self.out_width, self.out_height = (
-            self.style_attr["width"],
-            self.style_attr["height"],
-        )
-        print("Processing {} video(s)...".format(str(len(self.files_found))))
+        if platform.system() == "Darwin":
+            multiprocessing.set_start_method("spawn", force=True)
+        print(f"Processing {len(self.files_found)} video(s)...")
 
     def run(self):
-        """
-        Creates gantt charts. Results are stored in the `project_folder/frames/gantt_plots` directory of SimBA project.
-
-        Returns
-        ----------
-        None
-        """
-
+        check_all_file_names_are_represented_in_video_log(video_info_df=self.video_info_df, data_paths=self.files_found)
         for file_cnt, file_path in enumerate(self.files_found):
-            video_timer = SimbaTimer()
-            video_timer.start_timer()
+            video_timer = SimbaTimer(start=True)
             _, self.video_name, _ = get_fn_ext(file_path)
-            self.data_df = read_df(file_path, self.file_type).reset_index(drop=True)
-            print(
-                "Processing video {}, Frame count: {} (Video {}/{})...".format(
-                    self.video_name,
-                    str(len(self.data_df)),
-                    str(file_cnt + 1),
-                    str(len(self.files_found)),
-                )
-            )
-            self.video_info_settings, _, self.fps = self.read_video_info(
-                video_name=self.video_name
-            )
-            self.bouts_df = detect_bouts(
-                data_df=self.data_df, target_lst=list(self.clf_names), fps=int(self.fps)
-            )
-            self.temp_folder = os.path.join(
-                self.gantt_plot_dir, self.video_name, "temp"
-            )
-            self.save_frame_folder_dir = os.path.join(
-                self.gantt_plot_dir, self.video_name
-            )
+            self.data_df = read_df(file_path, self.file_type)
+            check_that_column_exist(df=self.data_df, column_name=self.clf_names, file_name=file_path)
+            print(f"Processing video {self.video_name}, Frame count: {len(self.data_df)} (Video {(file_cnt + 1)}/{len(self.files_found)})...")
+            self.video_info_settings, _, self.fps = self.read_video_info(video_name=self.video_name)
+            self.bouts_df = detect_bouts(data_df=self.data_df, target_lst=list(self.clf_names), fps=int(self.fps))
+            self.bouts_df.to_csv('/Users/simon/Desktop/envs/simba/simba/simba/sandbox/bouts_df')
+            self.temp_folder = os.path.join(self.gantt_plot_dir, self.video_name, "temp")
+            self.save_frame_folder_dir = os.path.join(self.gantt_plot_dir, self.video_name)
             if self.frame_setting:
                 if os.path.exists(self.save_frame_folder_dir):
                     shutil.rmtree(self.save_frame_folder_dir)
-                if not os.path.exists(self.save_frame_folder_dir):
-                    os.makedirs(self.save_frame_folder_dir)
+                os.makedirs(self.save_frame_folder_dir)
             if self.video_setting:
                 self.video_folder = os.path.join(self.gantt_plot_dir, self.video_name)
                 if os.path.exists(self.temp_folder):
                     shutil.rmtree(self.temp_folder)
                     shutil.rmtree(self.video_folder)
                 os.makedirs(self.temp_folder)
-                self.save_video_path = os.path.join(
-                    self.gantt_plot_dir, self.video_name + ".mp4"
-                )
+                self.save_video_path = os.path.join(self.gantt_plot_dir, f"{self.video_name}.mp4")
 
             if self.last_frm_setting:
-                _ = self.make_gantt_plot(
-                    data_df=self.data_df,
-                    bouts_df=self.bouts_df,
-                    clf_names=self.clf_names,
-                    fps=self.fps,
-                    style_attr=self.style_attr,
-                    video_name=self.video_name,
-                    save_path=os.path.join(
-                        self.gantt_plot_dir, self.video_name + "_final_image.png"
-                    ),
-                )
+                self.make_gantt_plot(data_df=self.data_df,
+                                     bouts_df=self.bouts_df,
+                                     clf_names=self.clf_names,
+                                     fps=self.fps,
+                                     style_attr=self.style_attr,
+                                     video_name=self.video_name,
+                                     save_path=os.path.join(self.gantt_plot_dir,  f"{self.video_name}_final_image.png"))
 
             if self.video_setting or self.frame_setting:
-                frame_array = np.array_split(
-                    list(range(0, len(self.data_df))), self.cores
-                )
+                frame_array = np.array_split(list(range(0, len(self.data_df))), self.cores)
                 frm_per_core = len(frame_array[0])
-                for group_cnt, rng in enumerate(frame_array):
-                    frame_array[group_cnt] = np.insert(rng, 0, group_cnt)
-
-                print(
-                    "Creating gantt, multiprocessing (chunksize: {}, cores: {})...".format(
-                        str(self.multiprocess_chunksize), str(self.cores)
-                    )
-                )
-                with multiprocessing.Pool(
-                    self.cores, maxtasksperchild=self.maxtasksperchild
-                ) as pool:
-                    constants = functools.partial(
-                        self.gantt_creator_mp,
-                        video_setting=self.video_setting,
-                        frame_setting=self.frame_setting,
-                        video_save_dir=self.temp_folder,
-                        frame_folder_dir=self.save_frame_folder_dir,
-                        bouts_df=self.bouts_df,
-                        rotation=self.y_rotation,
-                        clf_names=self.clf_names,
-                        colors=self.colours,
-                        color_tuple=self.colour_tuple_x,
-                        fps=self.fps,
-                        font_size=self.y_fontsize,
-                        width=self.out_width,
-                        height=self.out_height,
-                        video_name=self.video_name,
-                    )
-
-                    for cnt, result in enumerate(
-                        pool.imap(
-                            constants,
-                            frame_array,
-                            chunksize=self.multiprocess_chunksize,
-                        )
-                    ):
+                for group_cnt, rng in enumerate(frame_array): frame_array[group_cnt] = np.insert(rng, 0, group_cnt)
+                print(f"Creating gantt, multiprocessing (chunksize: {(self.multiprocess_chunksize)}, cores: {self.cores})...")
+                with multiprocessing.Pool(self.cores, maxtasksperchild=self.maxtasksperchild) as pool:
+                    constants = functools.partial(self.gantt_creator_mp,
+                                                  video_setting=self.video_setting,
+                                                  frame_setting=self.frame_setting,
+                                                  video_save_dir=self.temp_folder,
+                                                  frame_folder_dir=self.save_frame_folder_dir,
+                                                  bouts_df=self.bouts_df,
+                                                  clf_names=self.clf_names,
+                                                  fps=self.fps,
+                                                  rotation=self.y_rotation,
+                                                  colors=self.colours,
+                                                  color_tuple=self.colour_tuple_x,
+                                                  font_size=self.y_fontsize,
+                                                  width=self.out_width,
+                                                  height=self.out_height,
+                                                  video_name=self.video_name)
+                    for cnt, result in enumerate(pool.imap(constants, frame_array, chunksize=self.multiprocess_chunksize)):
                         print(
                             "Image {}/{}, Video {}/{}...".format(
                                 str(int(frm_per_core * (result + 1))),
                                 str(len(self.data_df)),
                                 str(file_cnt + 1),
                                 str(len(self.files_found)),
                             )
@@ -238,21 +168,21 @@
         self.timer.stop_timer()
         stdout_success(
             msg=f"Gantt visualizations for {len(self.files_found)} videos created in project_folder/frames/output/gantt_plots directory",
             elapsed_time=self.timer.elapsed_time_str,
         )
 
 
-# test = GanttCreatorMultiprocess(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
-#                                 frame_setting=False,
-#                                 video_setting=True,
-#                                 files_found=['/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/csv/targets_inserted/Together_1.csv'],
+# test = GanttCreatorMultiprocess(config_path='/Users/simon/Desktop/envs/simba/troubleshooting/beepboop174/project_folder/project_config.ini',
+#                                 frame_setting=True,
+#                                 video_setting=False,
+#                                 files_found=['/Users/simon/Desktop/envs/simba/troubleshooting/beepboop174/project_folder/csv/machine_results/Trial    10.csv'],
 #                                 cores=5,
 #                                 last_frm_setting=False,
-#                                 style_attr={'width': 640, 'height': 480, 'font size': 12, 'font rotation': 45})
+#                                 style_attr={'width': 640, 'height': 480, 'font size': 10, 'font rotation': 65})
 # test.run()
 
 
 # style_attr = {'width': 640, 'height': 480, 'font size': 12, 'font rotation': 45}
 # test = GanttCreatorMultiprocess(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals/project_folder/project_config.ini',
 #                                  frame_setting=False,
 #                                  video_setting=True,
```

### Comparing `Simba-UW-tf-dev-1.89.7/simba/plotting/heat_mapper_clf_mp.py` & `Simba-UW-tf-dev-1.89.8/simba/plotting/heat_mapper_clf_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/plotting/probability_plot_creator.py` & `Simba-UW-tf-dev-1.89.8/simba/plotting/probability_plot_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/plotting/circular_plotting.py` & `Simba-UW-tf-dev-1.89.8/simba/plotting/circular_plotting.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/plotting/plot_clf_results.py` & `Simba-UW-tf-dev-1.89.8/simba/plotting/plot_clf_results.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/plotting/plot_clf_results_mp.py` & `Simba-UW-tf-dev-1.89.8/simba/plotting/plot_clf_results_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/plotting/ROI_feature_visualizer.py` & `Simba-UW-tf-dev-1.89.8/simba/plotting/ROI_feature_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/plotting/heat_mapper_location.py` & `Simba-UW-tf-dev-1.89.8/simba/plotting/heat_mapper_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/plotting/probability_plot_creator_mp.py` & `Simba-UW-tf-dev-1.89.8/simba/plotting/probability_plot_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/plotting/interactive_probability_grapher.py` & `Simba-UW-tf-dev-1.89.8/simba/plotting/interactive_probability_grapher.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/plotting/plot_pose_in_dir.py` & `Simba-UW-tf-dev-1.89.8/simba/plotting/plot_pose_in_dir.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/plotting/single_run_model_validation_video.py` & `Simba-UW-tf-dev-1.89.8/simba/plotting/single_run_model_validation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/plotting/frame_mergerer_ffmpeg.py` & `Simba-UW-tf-dev-1.89.8/simba/plotting/frame_mergerer_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/plotting/pose_plotter_mp.py` & `Simba-UW-tf-dev-1.89.8/simba/plotting/pose_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/plotting/directing_animals_visualizer_mp.py` & `Simba-UW-tf-dev-1.89.8/simba/plotting/directing_animals_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/plotting/clf_validator.py` & `Simba-UW-tf-dev-1.89.8/simba/plotting/clf_validator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/plotting/path_plotter_mp.py` & `Simba-UW-tf-dev-1.89.8/simba/plotting/path_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/plotting/ROI_feature_visualizer_mp.py` & `Simba-UW-tf-dev-1.89.8/simba/plotting/ROI_feature_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/plotting/data_plotter.py` & `Simba-UW-tf-dev-1.89.8/simba/plotting/data_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/plotting/spontaneous_alternation_plotter.py` & `Simba-UW-tf-dev-1.89.8/simba/plotting/spontaneous_alternation_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/plotting/path_plotter.py` & `Simba-UW-tf-dev-1.89.8/simba/plotting/path_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/plotting/ez_lineplot.py` & `Simba-UW-tf-dev-1.89.8/simba/plotting/ez_lineplot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/plotting/distance_plotter_mp.py` & `Simba-UW-tf-dev-1.89.8/simba/plotting/distance_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/plotting/ROI_plotter.py` & `Simba-UW-tf-dev-1.89.8/simba/plotting/ROI_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/plotting/geometry_plotter.py` & `Simba-UW-tf-dev-1.89.8/simba/plotting/geometry_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/plotting/clf_validator_mp.py` & `Simba-UW-tf-dev-1.89.8/simba/plotting/clf_validator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/plotting/heat_mapper_clf.py` & `Simba-UW-tf-dev-1.89.8/simba/plotting/heat_mapper_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/plotting/distance_plotter.py` & `Simba-UW-tf-dev-1.89.8/simba/plotting/distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/plotting/single_run_model_validation_video_mp.py` & `Simba-UW-tf-dev-1.89.8/simba/plotting/single_run_model_validation_video_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/plotting/directing_animals_visualizer.py` & `Simba-UW-tf-dev-1.89.8/simba/plotting/directing_animals_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/plotting/circular_feature_overlay_plotter.py` & `Simba-UW-tf-dev-1.89.8/simba/plotting/circular_feature_overlay_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/plotting/heat_mapper_location_mp.py` & `Simba-UW-tf-dev-1.89.8/simba/plotting/heat_mapper_location_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/dash_app/SimBA_dash_app.py` & `Simba-UW-tf-dev-1.89.8/simba/dash_app/SimBA_dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/dash_app/run_dash_tkinter.py` & `Simba-UW-tf-dev-1.89.8/simba/dash_app/run_dash_tkinter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/dash_app/dash_app.py` & `Simba-UW-tf-dev-1.89.8/simba/dash_app/dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/data_processors/spontaneous_alternation_calculator.py` & `Simba-UW-tf-dev-1.89.8/simba/data_processors/spontaneous_alternation_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/data_processors/agg_clf_calculator.py` & `Simba-UW-tf-dev-1.89.8/simba/data_processors/agg_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/data_processors/.DS_Store` & `Simba-UW-tf-dev-1.89.8/simba/data_processors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/data_processors/severity_bout_based_calculator.py` & `Simba-UW-tf-dev-1.89.8/simba/data_processors/severity_bout_based_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/data_processors/interpolation_smoothing.py` & `Simba-UW-tf-dev-1.89.8/simba/data_processors/interpolation_smoothing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/data_processors/directing_animal_to_bodypart.py` & `Simba-UW-tf-dev-1.89.8/simba/data_processors/directing_animal_to_bodypart.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/data_processors/timebins_clf_calculator.py` & `Simba-UW-tf-dev-1.89.8/simba/data_processors/timebins_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/data_processors/fsttc_calculator.py` & `Simba-UW-tf-dev-1.89.8/simba/data_processors/fsttc_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/data_processors/boolean_conditional_calculator.py` & `Simba-UW-tf-dev-1.89.8/simba/data_processors/boolean_conditional_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/data_processors/interpolate_pose.py` & `Simba-UW-tf-dev-1.89.8/simba/data_processors/interpolate_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/data_processors/directing_other_animals_calculator.py` & `Simba-UW-tf-dev-1.89.8/simba/data_processors/directing_other_animals_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/data_processors/gibbs_sampler.py` & `Simba-UW-tf-dev-1.89.8/simba/data_processors/gibbs_sampler.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/data_processors/timebins_movement_calculator.py` & `Simba-UW-tf-dev-1.89.8/simba/data_processors/timebins_movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/data_processors/severity_calculator.py` & `Simba-UW-tf-dev-1.89.8/simba/data_processors/severity_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/data_processors/pup_retrieval_calculator.py` & `Simba-UW-tf-dev-1.89.8/simba/data_processors/pup_retrieval_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/data_processors/pybursts_calculator.py` & `Simba-UW-tf-dev-1.89.8/simba/data_processors/pybursts_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/data_processors/severity_frame_based_calculator.py` & `Simba-UW-tf-dev-1.89.8/simba/data_processors/severity_frame_based_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/data_processors/mutual_exclusivity_corrector.py` & `Simba-UW-tf-dev-1.89.8/simba/data_processors/mutual_exclusivity_corrector.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/data_processors/kleinberg_calculator.py` & `Simba-UW-tf-dev-1.89.8/simba/data_processors/kleinberg_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/data_processors/movement_calculator.py` & `Simba-UW-tf-dev-1.89.8/simba/data_processors/movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/model/train_rf.py` & `Simba-UW-tf-dev-1.89.8/simba/model/train_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/model/inference_batch.py` & `Simba-UW-tf-dev-1.89.8/simba/model/inference_batch.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/model/train_multiclass_rf.py` & `Simba-UW-tf-dev-1.89.8/simba/model/train_multiclass_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/model/inference_multiclass_batch.py` & `Simba-UW-tf-dev-1.89.8/simba/model/inference_multiclass_batch.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/model/grid_search_multiclass_rf.py` & `Simba-UW-tf-dev-1.89.8/simba/model/grid_search_multiclass_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/model/grid_search_rf.py` & `Simba-UW-tf-dev-1.89.8/simba/model/grid_search_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/model/inference_validation.py` & `Simba-UW-tf-dev-1.89.8/simba/model/inference_validation.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/model/train_multilabel_rf.py` & `Simba-UW-tf-dev-1.89.8/simba/model/train_multilabel_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/roi_tools/ROI_time_bin_calculator.py` & `Simba-UW-tf-dev-1.89.8/simba/roi_tools/ROI_time_bin_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/roi_tools/ROI_movement_analyzer.py` & `Simba-UW-tf-dev-1.89.8/simba/roi_tools/ROI_movement_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/roi_tools/.DS_Store` & `Simba-UW-tf-dev-1.89.8/simba/roi_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/roi_tools/ROI_define.py` & `Simba-UW-tf-dev-1.89.8/simba/roi_tools/ROI_define.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/roi_tools/ROI_reset.py` & `Simba-UW-tf-dev-1.89.8/simba/roi_tools/ROI_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/roi_tools/ROI_size_standardizer.py` & `Simba-UW-tf-dev-1.89.8/simba/roi_tools/ROI_size_standardizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/roi_tools/ROI_analyzer.py` & `Simba-UW-tf-dev-1.89.8/simba/roi_tools/ROI_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/roi_tools/ROI_feature_analyzer.py` & `Simba-UW-tf-dev-1.89.8/simba/roi_tools/ROI_feature_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/roi_tools/ROI_multiply.py` & `Simba-UW-tf-dev-1.89.8/simba/roi_tools/ROI_multiply.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/roi_tools/ROI_size_calculations.py` & `Simba-UW-tf-dev-1.89.8/simba/roi_tools/ROI_size_calculations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/roi_tools/ROI_zoom.py` & `Simba-UW-tf-dev-1.89.8/simba/roi_tools/ROI_zoom.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/roi_tools/ROI_directing_analyzer.py` & `Simba-UW-tf-dev-1.89.8/simba/roi_tools/ROI_directing_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/roi_tools/ROI_move_shape.py` & `Simba-UW-tf-dev-1.89.8/simba/roi_tools/ROI_move_shape.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/roi_tools/ROI_menus.py` & `Simba-UW-tf-dev-1.89.8/simba/roi_tools/ROI_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/roi_tools/ROI_clf_calculator.py` & `Simba-UW-tf-dev-1.89.8/simba/roi_tools/ROI_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/roi_tools/ROI_image.py` & `Simba-UW-tf-dev-1.89.8/simba/roi_tools/ROI_image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/pose_importers/sleap_csv_importer.py` & `Simba-UW-tf-dev-1.89.8/simba/pose_importers/sleap_csv_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/pose_importers/misc/apt_trk_importer.py` & `Simba-UW-tf-dev-1.89.8/simba/pose_importers/misc/apt_trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/pose_importers/read_DANNCE_mat.py` & `Simba-UW-tf-dev-1.89.8/simba/pose_importers/read_DANNCE_mat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/pose_importers/.DS_Store` & `Simba-UW-tf-dev-1.89.8/simba/pose_importers/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/pose_importers/sleap_h5_importer.py` & `Simba-UW-tf-dev-1.89.8/simba/pose_importers/sleap_h5_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/pose_importers/madlc_importer.py` & `Simba-UW-tf-dev-1.89.8/simba/pose_importers/madlc_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/pose_importers/sleap_slp_importer.py` & `Simba-UW-tf-dev-1.89.8/simba/pose_importers/sleap_slp_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/pose_importers/import_mars.py` & `Simba-UW-tf-dev-1.89.8/simba/pose_importers/import_mars.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/pose_importers/dlc_importer_csv.py` & `Simba-UW-tf-dev-1.89.8/simba/pose_importers/dlc_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/pose_importers/trk_importer.py` & `Simba-UW-tf-dev-1.89.8/simba/pose_importers/trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/pose_configurations/.DS_Store` & `Simba-UW-tf-dev-1.89.8/simba/pose_configurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/pose_configurations/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.89.8/simba/pose_configurations/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/pose_configurations/schematics/8.png` & `Simba-UW-tf-dev-1.89.8/simba/pose_configurations/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/pose_configurations/schematics/9.png` & `Simba-UW-tf-dev-1.89.8/simba/pose_configurations/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/pose_configurations/schematics/12.png` & `Simba-UW-tf-dev-1.89.8/simba/pose_configurations/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/pose_configurations/schematics/13.png` & `Simba-UW-tf-dev-1.89.8/simba/pose_configurations/schematics/13.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/pose_configurations/schematics/11.png` & `Simba-UW-tf-dev-1.89.8/simba/pose_configurations/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/pose_configurations/schematics/10.png` & `Simba-UW-tf-dev-1.89.8/simba/pose_configurations/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/pose_configurations/schematics/4.png` & `Simba-UW-tf-dev-1.89.8/simba/pose_configurations/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/pose_configurations/schematics/5.png` & `Simba-UW-tf-dev-1.89.8/simba/pose_configurations/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/pose_configurations/schematics/7.png` & `Simba-UW-tf-dev-1.89.8/simba/pose_configurations/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/pose_configurations/schematics/6.png` & `Simba-UW-tf-dev-1.89.8/simba/pose_configurations/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/pose_configurations/schematics/2.png` & `Simba-UW-tf-dev-1.89.8/simba/pose_configurations/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/pose_configurations/schematics/3.png` & `Simba-UW-tf-dev-1.89.8/simba/pose_configurations/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/pose_configurations/schematics/1.png` & `Simba-UW-tf-dev-1.89.8/simba/pose_configurations/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/video_processors/video_processing.py` & `Simba-UW-tf-dev-1.89.8/simba/video_processors/video_processing.py`

 * *Files 3% similar despite different names*

```diff
@@ -5899,1176 +5899,1322 @@
 000170a0: 6372 6561 7465 5f62 6c61 6e6b 5f76 6964  create_blank_vid
 000170b0: 656f 2e5f 5f6e 616d 655f 5f7d 2068 6569  eo.__name__} hei
 000170c0: 6768 7422 2c20 7661 6c75 653d 6865 6967  ght", value=heig
 000170d0: 6874 2c20 6d69 6e5f 7661 6c75 653d 3129  ht, min_value=1)
 000170e0: 0a20 2020 2063 6865 636b 5f69 665f 6469  .    check_if_di
 000170f0: 725f 6578 6973 7473 2869 6e5f 6469 723d  r_exists(in_dir=
 00017100: 6f73 2e70 6174 682e 6469 726e 616d 6528  os.path.dirname(
-00017110: 7061 7468 2929 0a20 2020 2074 696d 6572  path)).    timer
-00017120: 203d 2053 696d 6261 5469 6d65 7228 7374   = SimbaTimer(st
-00017130: 6172 743d 5472 7565 290a 2020 2020 6966  art=True).    if
-00017140: 2076 6572 626f 7365 3a0a 2020 2020 2020   verbose:.      
-00017150: 2020 7072 696e 7428 2243 7265 6174 696e    print("Creatin
-00017160: 6720 626c 616e 6b20 7669 6465 6f2e 2e2e  g blank video...
-00017170: 2229 0a20 2020 2069 6620 6770 753a 0a20  ").    if gpu:. 
-00017180: 2020 2020 2020 2063 6d64 203d 2066 2766         cmd = f'f
-00017190: 666d 7065 6720 2d79 202d 7420 7b6c 656e  fmpeg -y -t {len
-000171a0: 6774 687d 202d 6620 6c61 7666 6920 2d69  gth} -f lavfi -i
-000171b0: 2063 6f6c 6f72 3d63 3d7b 636f 6c6f 727d   color=c={color}
-000171c0: 3a73 3d7b 7769 6474 687d 787b 6865 6967  :s={width}x{heig
-000171d0: 6874 7d20 2d63 3a76 2068 3236 345f 6e76  ht} -c:v h264_nv
-000171e0: 656e 6320 2d70 7265 7365 7420 736c 6f77  enc -preset slow
-000171f0: 202d 7475 6e65 2073 7469 6c6c 696d 6167   -tune stillimag
-00017200: 6520 2d70 6978 5f66 6d74 2079 7576 3432  e -pix_fmt yuv42
-00017210: 3070 2022 7b70 6174 687d 2220 2d68 6964  0p "{path}" -hid
-00017220: 655f 6261 6e6e 6572 202d 6c6f 676c 6576  e_banner -loglev
-00017230: 656c 2065 7272 6f72 202d 7927 0a20 2020  el error -y'.   
-00017240: 2065 6c73 653a 0a20 2020 2020 2020 2063   else:.        c
-00017250: 6d64 203d 2066 2766 666d 7065 6720 2d79  md = f'ffmpeg -y
-00017260: 202d 7420 7b6c 656e 6774 687d 202d 6620   -t {length} -f 
-00017270: 6c61 7666 6920 2d69 2063 6f6c 6f72 3d63  lavfi -i color=c
-00017280: 3d7b 636f 6c6f 727d 3a73 3d7b 7769 6474  ={color}:s={widt
-00017290: 687d 787b 6865 6967 6874 7d20 2d63 3a76  h}x{height} -c:v
-000172a0: 206c 6962 7832 3634 202d 7475 6e65 2073   libx264 -tune s
-000172b0: 7469 6c6c 696d 6167 6520 2d70 6978 5f66  tillimage -pix_f
-000172c0: 6d74 2079 7576 3432 3070 2022 7b70 6174  mt yuv420p "{pat
-000172d0: 687d 2220 2d68 6964 655f 6261 6e6e 6572  h}" -hide_banner
-000172e0: 202d 6c6f 676c 6576 656c 2065 7272 6f72   -loglevel error
-000172f0: 202d 7927 0a20 2020 2073 7562 7072 6f63   -y'.    subproc
-00017300: 6573 732e 6361 6c6c 2863 6d64 2c20 7368  ess.call(cmd, sh
-00017310: 656c 6c3d 5472 7565 2c20 7374 646f 7574  ell=True, stdout
-00017320: 3d73 7562 7072 6f63 6573 732e 5049 5045  =subprocess.PIPE
-00017330: 290a 2020 2020 7469 6d65 722e 7374 6f70  ).    timer.stop
-00017340: 5f74 696d 6572 2829 0a20 2020 2069 6620  _timer().    if 
-00017350: 7665 7262 6f73 653a 0a20 2020 2020 2020  verbose:.       
-00017360: 2070 7269 6e74 2866 2242 6c61 6e6b 2076   print(f"Blank v
-00017370: 6964 656f 2063 6f6d 706c 6574 652e 2045  ideo complete. E
-00017380: 6c61 7073 6564 2074 696d 653a 207b 7469  lapsed time: {ti
-00017390: 6d65 722e 656c 6170 7365 645f 7469 6d65  mer.elapsed_time
-000173a0: 5f73 7472 7d73 2e22 290a 0a0a 6465 6620  _str}s.")...def 
-000173b0: 686f 7269 7a6f 6e74 616c 5f76 6964 656f  horizontal_video
-000173c0: 5f63 6f6e 6361 7465 6e61 746f 7228 0a20  _concatenator(. 
-000173d0: 2020 2076 6964 656f 5f70 6174 6873 3a20     video_paths: 
-000173e0: 4c69 7374 5b55 6e69 6f6e 5b73 7472 2c20  List[Union[str, 
-000173f0: 6f73 2e50 6174 684c 696b 655d 5d2c 0a20  os.PathLike]],. 
-00017400: 2020 2073 6176 655f 7061 7468 3a20 556e     save_path: Un
-00017410: 696f 6e5b 7374 722c 206f 732e 5061 7468  ion[str, os.Path
-00017420: 4c69 6b65 5d2c 0a20 2020 2068 6569 6768  Like],.    heigh
-00017430: 745f 7078 3a20 4f70 7469 6f6e 616c 5b55  t_px: Optional[U
-00017440: 6e69 6f6e 5b69 6e74 2c20 7374 725d 5d20  nion[int, str]] 
-00017450: 3d20 4e6f 6e65 2c0a 2020 2020 6865 6967  = None,.    heig
-00017460: 6874 5f69 6478 3a20 4f70 7469 6f6e 616c  ht_idx: Optional
-00017470: 5b55 6e69 6f6e 5b69 6e74 2c20 7374 725d  [Union[int, str]
-00017480: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 6770  ] = None,.    gp
-00017490: 753a 204f 7074 696f 6e61 6c5b 626f 6f6c  u: Optional[bool
-000174a0: 5d20 3d20 4661 6c73 652c 0a20 2020 2076  ] = False,.    v
-000174b0: 6572 626f 7365 3a20 4f70 7469 6f6e 616c  erbose: Optional
-000174c0: 5b62 6f6f 6c5d 203d 2054 7275 652c 0a29  [bool] = True,.)
-000174d0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2222   -> None:.    ""
-000174e0: 220a 2020 2020 436f 6e63 6174 656e 6174  ".    Concatenat
-000174f0: 6573 206d 756c 7469 706c 6520 7669 6465  es multiple vide
-00017500: 6f73 2068 6f72 697a 6f6e 7461 6c6c 792e  os horizontally.
-00017510: 0a0a 2020 2020 2e2e 2069 6d61 6765 3a3a  ..    .. image::
-00017520: 205f 7374 6174 6963 2f69 6d67 2f68 6f72   _static/img/hor
-00017530: 697a 6f6e 7461 6c5f 7669 6465 6f5f 636f  izontal_video_co
-00017540: 6e63 6174 656e 6174 6f72 2e70 6e67 0a20  ncatenator.png. 
-00017550: 2020 2020 2020 3a77 6964 7468 3a20 3330        :width: 30
-00017560: 300a 2020 2020 2020 203a 616c 6967 6e3a  0.       :align:
-00017570: 2063 656e 7465 720a 0a20 2020 203a 7061   center..    :pa
-00017580: 7261 6d20 4c69 7374 5b55 6e69 6f6e 5b73  ram List[Union[s
-00017590: 7472 2c20 6f73 2e50 6174 684c 696b 655d  tr, os.PathLike]
-000175a0: 5d20 7669 6465 6f5f 7061 7468 733a 204c  ] video_paths: L
-000175b0: 6973 7420 6f66 2069 6e70 7574 2076 6964  ist of input vid
-000175c0: 656f 2066 696c 6520 7061 7468 732e 0a20  eo file paths.. 
-000175d0: 2020 203a 7061 7261 6d20 556e 696f 6e5b     :param Union[
-000175e0: 7374 722c 206f 732e 5061 7468 4c69 6b65  str, os.PathLike
-000175f0: 5d20 7361 7665 5f70 6174 683a 2046 696c  ] save_path: Fil
-00017600: 6520 7061 7468 2074 6f20 7361 7665 2074  e path to save t
-00017610: 6865 2063 6f6e 6361 7465 6e61 7465 6420  he concatenated 
-00017620: 7669 6465 6f2e 0a20 2020 203a 7061 7261  video..    :para
-00017630: 6d20 4f70 7469 6f6e 616c 5b69 6e74 5d20  m Optional[int] 
-00017640: 6865 6967 6874 5f70 783a 2048 6569 6768  height_px: Heigh
-00017650: 7420 6f66 2074 6865 206f 7574 7075 7420  t of the output 
-00017660: 7669 6465 6f20 696e 2070 6978 656c 732e  video in pixels.
-00017670: 0a20 2020 203a 7061 7261 6d20 4f70 7469  .    :param Opti
-00017680: 6f6e 616c 5b69 6e74 5d20 6865 6967 6874  onal[int] height
-00017690: 5f69 6478 3a20 496e 6465 7820 6f66 2074  _idx: Index of t
-000176a0: 6865 2076 6964 656f 2074 6f20 7573 6520  he video to use 
-000176b0: 666f 7220 6465 7465 726d 696e 696e 6720  for determining 
-000176c0: 4865 6967 6874 2e0a 2020 2020 3a70 6172  Height..    :par
-000176d0: 616d 204f 7074 696f 6e61 6c5b 626f 6f6c  am Optional[bool
-000176e0: 5d20 6770 753a 2057 6865 7468 6572 2074  ] gpu: Whether t
-000176f0: 6f20 7573 6520 4750 552d 6163 6365 6c65  o use GPU-accele
-00017700: 7261 7465 6420 636f 6465 6320 2864 6566  rated codec (def
-00017710: 6175 6c74 3a20 4661 6c73 6529 2e0a 2020  ault: False)..  
-00017720: 2020 3a70 6172 616d 204f 7074 696f 6e61    :param Optiona
-00017730: 6c5b 626f 6f6c 5d20 7665 7262 6f73 653a  l[bool] verbose:
-00017740: 5768 6574 6865 7220 746f 2070 7269 6e74  Whether to print
-00017750: 2070 726f 6772 6573 7320 6d65 7373 6167   progress messag
-00017760: 6573 2028 6465 6661 756c 743a 2054 7275  es (default: Tru
-00017770: 6529 2e0a 0a20 2020 203a 6578 616d 706c  e)...    :exampl
-00017780: 653a 0a20 2020 203e 3e3e 2076 6964 656f  e:.    >>> video
-00017790: 5f70 6174 6873 203d 205b 2776 6964 656f  _paths = ['video
-000177a0: 312e 6d70 3427 2c20 2776 6964 656f 322e  1.mp4', 'video2.
-000177b0: 6d70 3427 5d0a 2020 2020 3e3e 3e20 7820  mp4'].    >>> x 
-000177c0: 3d20 686f 7269 7a6f 6e74 616c 5f76 6964  = horizontal_vid
-000177d0: 656f 5f63 6f6e 6361 7465 6e61 746f 7228  eo_concatenator(
-000177e0: 7669 6465 6f5f 7061 7468 733d 7669 6465  video_paths=vide
-000177f0: 6f5f 7061 7468 732c 2068 6569 6768 745f  o_paths, height_
-00017800: 7078 3d35 302c 2073 6176 655f 7061 7468  px=50, save_path
-00017810: 3d27 2f55 7365 7273 2f73 696d 6f6e 2f44  ='/Users/simon/D
-00017820: 6573 6b74 6f70 2f65 6e76 732f 7369 6d62  esktop/envs/simb
-00017830: 612f 7472 6f75 626c 6573 686f 6f74 696e  a/troubleshootin
-00017840: 672f 5241 545f 4e4f 522f 7072 6f6a 6563  g/RAT_NOR/projec
-00017850: 745f 666f 6c64 6572 2f76 6964 656f 732f  t_folder/videos/
-00017860: 7465 7374 2f6e 6577 2f30 3831 3032 3032  test/new/0810202
-00017870: 315f 444f 545f 5261 7437 5f38 2832 295f  1_DOT_Rat7_8(2)_
-00017880: 2e6d 7034 272c 2067 7075 3d46 616c 7365  .mp4', gpu=False
-00017890: 290a 2020 2020 2222 220a 2020 2020 6368  ).    """.    ch
-000178a0: 6563 6b5f 6666 6d70 6567 5f61 7661 696c  eck_ffmpeg_avail
-000178b0: 6162 6c65 2829 0a20 2020 2069 6620 6770  able().    if gp
-000178c0: 7520 616e 6420 6e6f 7420 6368 6563 6b5f  u and not check_
-000178d0: 6e76 6964 6561 5f67 7075 5f61 7661 696c  nvidea_gpu_avail
-000178e0: 6162 6c65 2829 3a0a 2020 2020 2020 2020  able():.        
-000178f0: 7261 6973 6520 4646 4d50 4547 436f 6465  raise FFMPEGCode
-00017900: 6347 5055 4572 726f 7228 0a20 2020 2020  cGPUError(.     
-00017910: 2020 2020 2020 206d 7367 3d22 4e56 4944         msg="NVID
-00017920: 4541 2047 5055 206e 6f74 2061 7661 696c  EA GPU not avail
-00017930: 6162 6c65 2028 6173 2065 7661 6c75 6174  able (as evaluat
-00017940: 6564 2062 7920 6e76 6964 6561 2d73 6d69  ed by nvidea-smi
-00017950: 2072 6574 7572 6e69 6e67 204e 6f6e 6529   returning None)
-00017960: 222c 0a20 2020 2020 2020 2020 2020 2073  ",.            s
-00017970: 6f75 7263 653d 686f 7269 7a6f 6e74 616c  ource=horizontal
-00017980: 5f76 6964 656f 5f63 6f6e 6361 7465 6e61  _video_concatena
-00017990: 746f 722e 5f5f 6e61 6d65 5f5f 2c0a 2020  tor.__name__,.  
-000179a0: 2020 2020 2020 290a 2020 2020 7469 6d65        ).    time
-000179b0: 7220 3d20 5369 6d62 6154 696d 6572 2873  r = SimbaTimer(s
-000179c0: 7461 7274 3d54 7275 6529 0a20 2020 2063  tart=True).    c
-000179d0: 6865 636b 5f76 616c 6964 5f6c 7374 280a  heck_valid_lst(.
-000179e0: 2020 2020 2020 2020 6461 7461 3d76 6964          data=vid
-000179f0: 656f 5f70 6174 6873 2c20 736f 7572 6365  eo_paths, source
-00017a00: 3d68 6f72 697a 6f6e 7461 6c5f 7669 6465  =horizontal_vide
-00017a10: 6f5f 636f 6e63 6174 656e 6174 6f72 2e5f  o_concatenator._
-00017a20: 5f6e 616d 655f 5f2c 206d 696e 5f6c 656e  _name__, min_len
-00017a30: 3d32 0a20 2020 2029 0a20 2020 2063 6865  =2.    ).    che
-00017a40: 636b 5f69 665f 6469 725f 6578 6973 7473  ck_if_dir_exists
-00017a50: 280a 2020 2020 2020 2020 696e 5f64 6972  (.        in_dir
-00017a60: 3d6f 732e 7061 7468 2e64 6972 6e61 6d65  =os.path.dirname
-00017a70: 2873 6176 655f 7061 7468 292c 2073 6f75  (save_path), sou
-00017a80: 7263 653d 686f 7269 7a6f 6e74 616c 5f76  rce=horizontal_v
-00017a90: 6964 656f 5f63 6f6e 6361 7465 6e61 746f  ideo_concatenato
-00017aa0: 722e 5f5f 6e61 6d65 5f5f 0a20 2020 2029  r.__name__.    )
-00017ab0: 0a20 2020 2076 6964 656f 5f6d 6574 615f  .    video_meta_
-00017ac0: 6461 7461 203d 205b 0a20 2020 2020 2020  data = [.       
-00017ad0: 2067 6574 5f76 6964 656f 5f6d 6574 615f   get_video_meta_
-00017ae0: 6461 7461 2876 6964 656f 5f70 6174 683d  data(video_path=
-00017af0: 7669 6465 6f5f 7061 7468 2920 666f 7220  video_path) for 
-00017b00: 7669 6465 6f5f 7061 7468 2069 6e20 7669  video_path in vi
-00017b10: 6465 6f5f 7061 7468 730a 2020 2020 5d0a  deo_paths.    ].
-00017b20: 2020 2020 6966 2028 2868 6569 6768 745f      if ((height_
-00017b30: 7078 2069 7320 4e6f 6e65 2920 616e 6420  px is None) and 
-00017b40: 2868 6569 6768 745f 6964 7820 6973 204e  (height_idx is N
-00017b50: 6f6e 6529 2920 6f72 2028 0a20 2020 2020  one)) or (.     
-00017b60: 2020 2028 6865 6967 6874 5f70 7820 6973     (height_px is
-00017b70: 206e 6f74 204e 6f6e 6529 2061 6e64 2028   not None) and (
-00017b80: 6865 6967 6874 5f69 6478 2069 7320 6e6f  height_idx is no
-00017b90: 7420 4e6f 6e65 290a 2020 2020 293a 0a20  t None).    ):. 
-00017ba0: 2020 2020 2020 2072 6169 7365 2049 6e76         raise Inv
-00017bb0: 616c 6964 496e 7075 7445 7272 6f72 280a  alidInputError(.
-00017bc0: 2020 2020 2020 2020 2020 2020 6d73 673d              msg=
-00017bd0: 2250 726f 7669 6465 2061 2068 6569 6768  "Provide a heigh
-00017be0: 745f 7078 204f 5220 6865 6967 6874 5f69  t_px OR height_i
-00017bf0: 6478 222c 0a20 2020 2020 2020 2020 2020  dx",.           
-00017c00: 2073 6f75 7263 653d 686f 7269 7a6f 6e74   source=horizont
-00017c10: 616c 5f76 6964 656f 5f63 6f6e 6361 7465  al_video_concate
-00017c20: 6e61 746f 722e 5f5f 6e61 6d65 5f5f 2c0a  nator.__name__,.
-00017c30: 2020 2020 2020 2020 290a 2020 2020 6966          ).    if
-00017c40: 2068 6569 6768 745f 6964 7820 6973 206e   height_idx is n
-00017c50: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00017c60: 2063 6865 636b 5f69 6e74 280a 2020 2020   check_int(.    
-00017c70: 2020 2020 2020 2020 6e61 6d65 3d66 227b          name=f"{
-00017c80: 686f 7269 7a6f 6e74 616c 5f76 6964 656f  horizontal_video
-00017c90: 5f63 6f6e 6361 7465 6e61 746f 722e 5f5f  _concatenator.__
-00017ca0: 6e61 6d65 5f5f 7d20 6865 6967 6874 222c  name__} height",
-00017cb0: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
-00017cc0: 7565 3d68 6569 6768 745f 6964 782c 0a20  ue=height_idx,. 
-00017cd0: 2020 2020 2020 2020 2020 206d 696e 5f76             min_v
-00017ce0: 616c 7565 3d30 2c0a 2020 2020 2020 2020  alue=0,.        
-00017cf0: 2020 2020 6d61 785f 7661 6c75 653d 6c65      max_value=le
-00017d00: 6e28 7669 6465 6f5f 7061 7468 7329 202d  n(video_paths) -
-00017d10: 2031 2c0a 2020 2020 2020 2020 290a 2020   1,.        ).  
-00017d20: 2020 2020 2020 6865 6967 6874 203d 2069        height = i
-00017d30: 6e74 2876 6964 656f 5f6d 6574 615f 6461  nt(video_meta_da
-00017d40: 7461 5b68 6569 6768 745f 6964 785d 5b22  ta[height_idx]["
-00017d50: 6865 6967 6874 225d 290a 2020 2020 656c  height"]).    el
-00017d60: 7365 3a0a 2020 2020 2020 2020 6368 6563  se:.        chec
-00017d70: 6b5f 696e 7428 0a20 2020 2020 2020 2020  k_int(.         
-00017d80: 2020 206e 616d 653d 6622 7b68 6f72 697a     name=f"{horiz
-00017d90: 6f6e 7461 6c5f 7669 6465 6f5f 636f 6e63  ontal_video_conc
-00017da0: 6174 656e 6174 6f72 2e5f 5f6e 616d 655f  atenator.__name_
-00017db0: 5f7d 2068 6569 6768 7422 2c0a 2020 2020  _} height",.    
-00017dc0: 2020 2020 2020 2020 7661 6c75 653d 6865          value=he
-00017dd0: 6967 6874 5f70 782c 0a20 2020 2020 2020  ight_px,.       
-00017de0: 2020 2020 206d 696e 5f76 616c 7565 3d31       min_value=1
-00017df0: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
-00017e00: 2020 2020 6865 6967 6874 203d 2069 6e74      height = int
-00017e10: 2868 6569 6768 745f 7078 290a 2020 2020  (height_px).    
-00017e20: 7669 6465 6f5f 7061 7468 5f73 7472 203d  video_path_str =
-00017e30: 2022 2022 2e6a 6f69 6e28 5b66 272d 6920   " ".join([f'-i 
-00017e40: 227b 7061 7468 7d22 2720 666f 7220 7061  "{path}"' for pa
-00017e50: 7468 2069 6e20 7669 6465 6f5f 7061 7468  th in video_path
-00017e60: 735d 290a 2020 2020 636f 6465 6320 3d20  s]).    codec = 
-00017e70: 2268 3236 345f 6e76 656e 6322 2069 6620  "h264_nvenc" if 
-00017e80: 6770 7520 656c 7365 2022 6c69 6276 7078  gpu else "libvpx
-00017e90: 2d76 7039 220a 2020 2020 6669 6c74 6572  -vp9".    filter
-00017ea0: 5f63 6f6d 706c 6578 203d 2022 3b22 2e6a  _complex = ";".j
-00017eb0: 6f69 6e28 0a20 2020 2020 2020 205b 6622  oin(.        [f"
-00017ec0: 5b7b 6964 787d 3a76 5d73 6361 6c65 3d2d  [{idx}:v]scale=-
-00017ed0: 313a 7b68 6569 6768 747d 5b76 7b69 6478  1:{height}[v{idx
-00017ee0: 7d5d 2220 666f 7220 6964 7820 696e 2072  }]" for idx in r
-00017ef0: 616e 6765 286c 656e 2876 6964 656f 5f70  ange(len(video_p
-00017f00: 6174 6873 2929 5d0a 2020 2020 290a 2020  aths))].    ).  
-00017f10: 2020 6669 6c74 6572 5f63 6f6d 706c 6578    filter_complex
-00017f20: 202b 3d20 6622 3b7b 2727 2e6a 6f69 6e28   += f";{''.join(
-00017f30: 5b66 275b 767b 6964 787d 5d27 2066 6f72  [f'[v{idx}]' for
-00017f40: 2069 6478 2069 6e20 7261 6e67 6528 6c65   idx in range(le
-00017f50: 6e28 7669 6465 6f5f 7061 7468 7329 295d  n(video_paths))]
-00017f60: 297d 6873 7461 636b 3d69 6e70 7574 733d  )}hstack=inputs=
-00017f70: 7b6c 656e 2876 6964 656f 5f70 6174 6873  {len(video_paths
-00017f80: 297d 5b76 5d22 0a20 2020 2069 6620 7665  )}[v]".    if ve
-00017f90: 7262 6f73 653a 0a20 2020 2020 2020 2070  rbose:.        p
-00017fa0: 7269 6e74 280a 2020 2020 2020 2020 2020  rint(.          
-00017fb0: 2020 6622 436f 6e63 6174 656e 6174 696e    f"Concatenatin
-00017fc0: 6720 7b6c 656e 2876 6964 656f 5f70 6174  g {len(video_pat
-00017fd0: 6873 297d 2076 6964 656f 7320 686f 7269  hs)} videos hori
-00017fe0: 7a6f 6e74 616c 6c79 2077 6974 6820 6120  zontally with a 
-00017ff0: 7b68 6569 6768 747d 2070 6978 656c 2068  {height} pixel h
-00018000: 6569 6768 742e 2e2e 2022 0a20 2020 2020  eight... ".     
-00018010: 2020 2029 0a20 2020 2063 6d64 203d 2066     ).    cmd = f
-00018020: 2766 666d 7065 6720 7b76 6964 656f 5f70  'ffmpeg {video_p
-00018030: 6174 685f 7374 727d 202d 6669 6c74 6572  ath_str} -filter
-00018040: 5f63 6f6d 706c 6578 2022 7b66 696c 7465  _complex "{filte
-00018050: 725f 636f 6d70 6c65 787d 2220 2d6d 6170  r_complex}" -map
-00018060: 2022 5b76 5d22 202d 633a 7620 7b63 6f64   "[v]" -c:v {cod
-00018070: 6563 7d20 2d6c 6f67 6c65 7665 6c20 6572  ec} -loglevel er
-00018080: 726f 7220 2d73 7461 7473 2022 7b73 6176  ror -stats "{sav
-00018090: 655f 7061 7468 7d22 202d 7927 0a20 2020  e_path}" -y'.   
-000180a0: 2073 7562 7072 6f63 6573 732e 6361 6c6c   subprocess.call
-000180b0: 2863 6d64 2c20 7368 656c 6c3d 5472 7565  (cmd, shell=True
-000180c0: 2c20 7374 646f 7574 3d73 7562 7072 6f63  , stdout=subproc
-000180d0: 6573 732e 5049 5045 290a 2020 2020 7469  ess.PIPE).    ti
-000180e0: 6d65 722e 7374 6f70 5f74 696d 6572 2829  mer.stop_timer()
-000180f0: 0a20 2020 2069 6620 7665 7262 6f73 653a  .    if verbose:
-00018100: 0a20 2020 2020 2020 2070 7269 6e74 280a  .        print(.
-00018110: 2020 2020 2020 2020 2020 2020 6622 486f              f"Ho
-00018120: 7269 7a6f 6e74 616c 2063 6f6e 6361 7465  rizontal concate
-00018130: 6e61 7469 6f6e 2063 6f6d 706c 6574 652c  nation complete,
-00018140: 2073 6176 6564 2061 7420 7b73 6176 655f   saved at {save_
-00018150: 7061 7468 7d20 2865 6c61 7073 6564 2074  path} (elapsed t
-00018160: 696d 653a 207b 7469 6d65 722e 656c 6170  ime: {timer.elap
-00018170: 7365 645f 7469 6d65 5f73 7472 7d73 2e29  sed_time_str}s.)
-00018180: 220a 2020 2020 2020 2020 290a 0a0a 6465  ".        )...de
-00018190: 6620 7665 7274 6963 616c 5f76 6964 656f  f vertical_video
-000181a0: 5f63 6f6e 6361 7465 6e61 746f 7228 0a20  _concatenator(. 
-000181b0: 2020 2076 6964 656f 5f70 6174 6873 3a20     video_paths: 
-000181c0: 4c69 7374 5b55 6e69 6f6e 5b73 7472 2c20  List[Union[str, 
-000181d0: 6f73 2e50 6174 684c 696b 655d 5d2c 0a20  os.PathLike]],. 
-000181e0: 2020 2073 6176 655f 7061 7468 3a20 556e     save_path: Un
-000181f0: 696f 6e5b 7374 722c 206f 732e 5061 7468  ion[str, os.Path
-00018200: 4c69 6b65 5d2c 0a20 2020 2077 6964 7468  Like],.    width
-00018210: 5f70 783a 204f 7074 696f 6e61 6c5b 696e  _px: Optional[in
-00018220: 745d 203d 204e 6f6e 652c 0a20 2020 2077  t] = None,.    w
-00018230: 6964 7468 5f69 6478 3a20 4f70 7469 6f6e  idth_idx: Option
-00018240: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 2c0a  al[int] = None,.
-00018250: 2020 2020 6770 753a 204f 7074 696f 6e61      gpu: Optiona
-00018260: 6c5b 626f 6f6c 5d20 3d20 4661 6c73 652c  l[bool] = False,
-00018270: 0a20 2020 2076 6572 626f 7365 3a20 4f70  .    verbose: Op
-00018280: 7469 6f6e 616c 5b62 6f6f 6c5d 203d 2054  tional[bool] = T
-00018290: 7275 652c 0a29 202d 3e20 4e6f 6e65 3a0a  rue,.) -> None:.
-000182a0: 2020 2020 2222 220a 2020 2020 436f 6e63      """.    Conc
-000182b0: 6174 656e 6174 6573 206d 756c 7469 706c  atenates multipl
-000182c0: 6520 7669 6465 6f73 2076 6572 7469 6361  e videos vertica
-000182d0: 6c6c 792e 0a0a 2020 2020 2e2e 2069 6d61  lly...    .. ima
-000182e0: 6765 3a3a 205f 7374 6174 6963 2f69 6d67  ge:: _static/img
-000182f0: 2f76 6572 7469 6361 6c5f 7669 6465 6f5f  /vertical_video_
-00018300: 636f 6e63 6174 656e 6174 6f72 2e70 6e67  concatenator.png
-00018310: 0a20 2020 2020 2020 3a77 6964 7468 3a20  .       :width: 
-00018320: 3330 300a 2020 2020 2020 203a 616c 6967  300.       :alig
-00018330: 6e3a 2063 656e 7465 720a 0a20 2020 203a  n: center..    :
-00018340: 7061 7261 6d20 4c69 7374 5b55 6e69 6f6e  param List[Union
-00018350: 5b73 7472 2c20 6f73 2e50 6174 684c 696b  [str, os.PathLik
-00018360: 655d 5d20 7669 6465 6f5f 7061 7468 733a  e]] video_paths:
-00018370: 204c 6973 7420 6f66 2069 6e70 7574 2076   List of input v
-00018380: 6964 656f 2066 696c 6520 7061 7468 732e  ideo file paths.
-00018390: 0a20 2020 203a 7061 7261 6d20 556e 696f  .    :param Unio
-000183a0: 6e5b 7374 722c 206f 732e 5061 7468 4c69  n[str, os.PathLi
-000183b0: 6b65 5d20 7361 7665 5f70 6174 683a 2046  ke] save_path: F
-000183c0: 696c 6520 7061 7468 2074 6f20 7361 7665  ile path to save
-000183d0: 2074 6865 2063 6f6e 6361 7465 6e61 7465   the concatenate
-000183e0: 6420 7669 6465 6f2e 0a20 2020 203a 7061  d video..    :pa
-000183f0: 7261 6d20 4f70 7469 6f6e 616c 5b69 6e74  ram Optional[int
-00018400: 5d20 7769 6474 685f 7078 3a20 5769 6474  ] width_px: Widt
-00018410: 6820 6f66 2074 6865 206f 7574 7075 7420  h of the output 
-00018420: 7669 6465 6f20 696e 2070 6978 656c 732e  video in pixels.
-00018430: 0a20 2020 203a 7061 7261 6d20 4f70 7469  .    :param Opti
-00018440: 6f6e 616c 5b69 6e74 5d20 7769 6474 685f  onal[int] width_
-00018450: 6964 783a 2049 6e64 6578 206f 6620 7468  idx: Index of th
-00018460: 6520 7669 6465 6f20 746f 2075 7365 2066  e video to use f
-00018470: 6f72 2064 6574 6572 6d69 6e69 6e67 2077  or determining w
-00018480: 6964 7468 2e0a 2020 2020 3a70 6172 616d  idth..    :param
-00018490: 204f 7074 696f 6e61 6c5b 626f 6f6c 5d20   Optional[bool] 
-000184a0: 6770 753a 2057 6865 7468 6572 2074 6f20  gpu: Whether to 
-000184b0: 7573 6520 4750 552d 6163 6365 6c65 7261  use GPU-accelera
-000184c0: 7465 6420 636f 6465 6320 2864 6566 6175  ted codec (defau
-000184d0: 6c74 3a20 4661 6c73 6529 2e0a 2020 2020  lt: False)..    
-000184e0: 3a70 6172 616d 204f 7074 696f 6e61 6c5b  :param Optional[
-000184f0: 626f 6f6c 5d20 7665 7262 6f73 653a 5768  bool] verbose:Wh
-00018500: 6574 6865 7220 746f 2070 7269 6e74 2070  ether to print p
-00018510: 726f 6772 6573 7320 6d65 7373 6167 6573  rogress messages
-00018520: 2028 6465 6661 756c 743a 2054 7275 6529   (default: True)
-00018530: 2e0a 2020 2020 3a72 6169 7365 7320 4646  ..    :raises FF
-00018540: 4d50 4547 436f 6465 6347 5055 4572 726f  MPEGCodecGPUErro
-00018550: 723a 2049 6620 4750 5520 6973 2072 6571  r: If GPU is req
-00018560: 7565 7374 6564 2062 7574 206e 6f74 2061  uested but not a
-00018570: 7661 696c 6162 6c65 2e0a 2020 2020 3a72  vailable..    :r
-00018580: 6169 7365 7320 496e 7661 6c69 6449 6e70  aises InvalidInp
-00018590: 7574 4572 726f 723a 2049 6620 626f 7468  utError: If both
-000185a0: 206f 7220 6e65 6974 6865 7220 7769 6474   or neither widt
-000185b0: 685f 7078 2061 6e64 2077 6964 7468 5f69  h_px and width_i
-000185c0: 6478 2061 7265 2070 726f 7669 6465 642e  dx are provided.
-000185d0: 0a0a 2020 2020 3a65 7861 6d70 6c65 3a0a  ..    :example:.
-000185e0: 2020 2020 3e3e 3e20 7669 6465 6f5f 7061      >>> video_pa
-000185f0: 7468 7320 3d20 5b27 2f55 7365 7273 2f73  ths = ['/Users/s
-00018600: 696d 6f6e 2f44 6573 6b74 6f70 2f65 6e76  imon/Desktop/env
-00018610: 732f 7369 6d62 612f 7472 6f75 626c 6573  s/simba/troubles
-00018620: 686f 6f74 696e 672f 5241 545f 4e4f 522f  hooting/RAT_NOR/
-00018630: 7072 6f6a 6563 745f 666f 6c64 6572 2f76  project_folder/v
-00018640: 6964 656f 732f 7465 7374 2f30 3831 3032  ideos/test/08102
-00018650: 3032 315f 444f 545f 5261 7437 5f38 2832  021_DOT_Rat7_8(2
-00018660: 292e 6d70 3427 2c0a 2020 2020 3e3e 3e20  ).mp4',.    >>> 
-00018670: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00018680: 2f55 7365 7273 2f73 696d 6f6e 2f44 6573  /Users/simon/Des
-00018690: 6b74 6f70 2f65 6e76 732f 7369 6d62 612f  ktop/envs/simba/
-000186a0: 7472 6f75 626c 6573 686f 6f74 696e 672f  troubleshooting/
-000186b0: 5241 545f 4e4f 522f 7072 6f6a 6563 745f  RAT_NOR/project_
-000186c0: 666f 6c64 6572 2f76 6964 656f 732f 7465  folder/videos/te
-000186d0: 7374 2f30 3831 3032 3032 315f 444f 545f  st/08102021_DOT_
-000186e0: 5261 7431 315f 3132 2e6d 7034 272c 0a20  Rat11_12.mp4',. 
-000186f0: 2020 203e 3e3e 2020 2020 2020 2020 2020     >>>          
-00018700: 2020 2020 2020 272f 5573 6572 732f 7369        '/Users/si
-00018710: 6d6f 6e2f 4465 736b 746f 702f 656e 7673  mon/Desktop/envs
-00018720: 2f73 696d 6261 2f74 726f 7562 6c65 7368  /simba/troublesh
-00018730: 6f6f 7469 6e67 2f52 4154 5f4e 4f52 2f70  ooting/RAT_NOR/p
-00018740: 726f 6a65 6374 5f66 6f6c 6465 722f 7669  roject_folder/vi
-00018750: 6465 6f73 2f74 6573 742f 3038 3130 3230  deos/test/081020
-00018760: 3231 5f44 4f54 5f52 6174 3131 5f31 325f  21_DOT_Rat11_12_
-00018770: 312e 6d70 3427 5d0a 2020 2020 3e3e 3e20  1.mp4'].    >>> 
-00018780: 5f20 3d20 7665 7274 6963 616c 5f76 6964  _ = vertical_vid
-00018790: 656f 5f63 6f6e 6361 7465 6e61 746f 7228  eo_concatenator(
-000187a0: 7669 6465 6f5f 7061 7468 733d 7669 6465  video_paths=vide
-000187b0: 6f5f 7061 7468 732c 2077 6964 7468 5f69  o_paths, width_i
-000187c0: 6478 3d31 2c20 7361 7665 5f70 6174 683d  dx=1, save_path=
-000187d0: 272f 5573 6572 732f 7369 6d6f 6e2f 4465  '/Users/simon/De
-000187e0: 736b 746f 702f 656e 7673 2f73 696d 6261  sktop/envs/simba
-000187f0: 2f74 726f 7562 6c65 7368 6f6f 7469 6e67  /troubleshooting
-00018800: 2f52 4154 5f4e 4f52 2f70 726f 6a65 6374  /RAT_NOR/project
-00018810: 5f66 6f6c 6465 722f 7669 6465 6f73 2f74  _folder/videos/t
-00018820: 6573 742f 6e65 772f 3038 3130 3230 3231  est/new/08102021
-00018830: 5f44 4f54 5f52 6174 375f 3828 3229 5f2e  _DOT_Rat7_8(2)_.
-00018840: 6d70 3427 2c20 6770 753d 4661 6c73 6529  mp4', gpu=False)
-00018850: 0a20 2020 2022 2222 0a0a 2020 2020 6368  .    """..    ch
-00018860: 6563 6b5f 6666 6d70 6567 5f61 7661 696c  eck_ffmpeg_avail
-00018870: 6162 6c65 2829 0a20 2020 2069 6620 6770  able().    if gp
-00018880: 7520 616e 6420 6e6f 7420 6368 6563 6b5f  u and not check_
-00018890: 6e76 6964 6561 5f67 7075 5f61 7661 696c  nvidea_gpu_avail
-000188a0: 6162 6c65 2829 3a0a 2020 2020 2020 2020  able():.        
-000188b0: 7261 6973 6520 4646 4d50 4547 436f 6465  raise FFMPEGCode
-000188c0: 6347 5055 4572 726f 7228 0a20 2020 2020  cGPUError(.     
-000188d0: 2020 2020 2020 206d 7367 3d22 4e56 4944         msg="NVID
-000188e0: 4941 2047 5055 206e 6f74 2061 7661 696c  IA GPU not avail
-000188f0: 6162 6c65 222c 2073 6f75 7263 653d 7665  able", source=ve
-00018900: 7274 6963 616c 5f76 6964 656f 5f63 6f6e  rtical_video_con
-00018910: 6361 7465 6e61 746f 722e 5f5f 6e61 6d65  catenator.__name
-00018920: 5f5f 0a20 2020 2020 2020 2029 0a20 2020  __.        ).   
-00018930: 2076 6964 656f 5f6d 6574 615f 6461 7461   video_meta_data
-00018940: 203d 205b 0a20 2020 2020 2020 2067 6574   = [.        get
-00018950: 5f76 6964 656f 5f6d 6574 615f 6461 7461  _video_meta_data
-00018960: 2876 6964 656f 5f70 6174 683d 7669 6465  (video_path=vide
-00018970: 6f5f 7061 7468 2920 666f 7220 7669 6465  o_path) for vide
-00018980: 6f5f 7061 7468 2069 6e20 7669 6465 6f5f  o_path in video_
-00018990: 7061 7468 730a 2020 2020 5d0a 2020 2020  paths.    ].    
-000189a0: 7469 6d65 7220 3d20 5369 6d62 6154 696d  timer = SimbaTim
-000189b0: 6572 2873 7461 7274 3d54 7275 6529 0a20  er(start=True). 
-000189c0: 2020 2063 6865 636b 5f76 616c 6964 5f6c     check_valid_l
-000189d0: 7374 280a 2020 2020 2020 2020 6461 7461  st(.        data
-000189e0: 3d76 6964 656f 5f70 6174 6873 2c20 736f  =video_paths, so
-000189f0: 7572 6365 3d76 6572 7469 6361 6c5f 7669  urce=vertical_vi
-00018a00: 6465 6f5f 636f 6e63 6174 656e 6174 6f72  deo_concatenator
-00018a10: 2e5f 5f6e 616d 655f 5f2c 206d 696e 5f6c  .__name__, min_l
-00018a20: 656e 3d32 0a20 2020 2029 0a20 2020 2063  en=2.    ).    c
-00018a30: 6865 636b 5f69 665f 6469 725f 6578 6973  heck_if_dir_exis
-00018a40: 7473 280a 2020 2020 2020 2020 696e 5f64  ts(.        in_d
-00018a50: 6972 3d6f 732e 7061 7468 2e64 6972 6e61  ir=os.path.dirna
-00018a60: 6d65 2873 6176 655f 7061 7468 292c 2073  me(save_path), s
-00018a70: 6f75 7263 653d 7665 7274 6963 616c 5f76  ource=vertical_v
-00018a80: 6964 656f 5f63 6f6e 6361 7465 6e61 746f  ideo_concatenato
-00018a90: 722e 5f5f 6e61 6d65 5f5f 0a20 2020 2029  r.__name__.    )
-00018aa0: 0a20 2020 2069 6620 2828 7769 6474 685f  .    if ((width_
-00018ab0: 7078 2069 7320 4e6f 6e65 2920 616e 6420  px is None) and 
-00018ac0: 2877 6964 7468 5f69 6478 2069 7320 4e6f  (width_idx is No
-00018ad0: 6e65 2929 206f 7220 280a 2020 2020 2020  ne)) or (.      
-00018ae0: 2020 2877 6964 7468 5f70 7820 6973 206e    (width_px is n
-00018af0: 6f74 204e 6f6e 6529 2061 6e64 2028 7769  ot None) and (wi
-00018b00: 6474 685f 6964 7820 6973 206e 6f74 204e  dth_idx is not N
-00018b10: 6f6e 6529 0a20 2020 2029 3a0a 2020 2020  one).    ):.    
-00018b20: 2020 2020 7261 6973 6520 496e 7661 6c69      raise Invali
-00018b30: 6449 6e70 7574 4572 726f 7228 0a20 2020  dInputError(.   
-00018b40: 2020 2020 2020 2020 206d 7367 3d22 5072           msg="Pr
-00018b50: 6f76 6964 6520 6120 7769 6474 685f 7078  ovide a width_px
-00018b60: 204f 5220 7769 6474 685f 6964 7822 2c0a   OR width_idx",.
-00018b70: 2020 2020 2020 2020 2020 2020 736f 7572              sour
-00018b80: 6365 3d76 6572 7469 6361 6c5f 7669 6465  ce=vertical_vide
-00018b90: 6f5f 636f 6e63 6174 656e 6174 6f72 2e5f  o_concatenator._
-00018ba0: 5f6e 616d 655f 5f2c 0a20 2020 2020 2020  _name__,.       
-00018bb0: 2029 0a20 2020 2069 6620 7769 6474 685f   ).    if width_
-00018bc0: 6964 7820 6973 206e 6f74 204e 6f6e 653a  idx is not None:
-00018bd0: 0a20 2020 2020 2020 2063 6865 636b 5f69  .        check_i
-00018be0: 6e74 280a 2020 2020 2020 2020 2020 2020  nt(.            
-00018bf0: 6e61 6d65 3d66 227b 7665 7274 6963 616c  name=f"{vertical
-00018c00: 5f76 6964 656f 5f63 6f6e 6361 7465 6e61  _video_concatena
-00018c10: 746f 722e 5f5f 6e61 6d65 5f5f 7d20 7769  tor.__name__} wi
-00018c20: 6474 6820 696e 6465 7822 2c0a 2020 2020  dth index",.    
-00018c30: 2020 2020 2020 2020 7661 6c75 653d 7769          value=wi
-00018c40: 6474 685f 6964 782c 0a20 2020 2020 2020  dth_idx,.       
-00018c50: 2020 2020 206d 696e 5f76 616c 7565 3d30       min_value=0
-00018c60: 2c0a 2020 2020 2020 2020 2020 2020 6d61  ,.            ma
-00018c70: 785f 7661 6c75 653d 6c65 6e28 7669 6465  x_value=len(vide
-00018c80: 6f5f 7061 7468 7329 202d 2031 2c0a 2020  o_paths) - 1,.  
-00018c90: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00018ca0: 7769 6474 6820 3d20 696e 7428 7669 6465  width = int(vide
-00018cb0: 6f5f 6d65 7461 5f64 6174 615b 7769 6474  o_meta_data[widt
-00018cc0: 685f 6964 785d 5b22 7769 6474 6822 5d29  h_idx]["width"])
-00018cd0: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
-00018ce0: 2020 2063 6865 636b 5f69 6e74 280a 2020     check_int(.  
-00018cf0: 2020 2020 2020 2020 2020 6e61 6d65 3d66            name=f
-00018d00: 227b 7665 7274 6963 616c 5f76 6964 656f  "{vertical_video
-00018d10: 5f63 6f6e 6361 7465 6e61 746f 722e 5f5f  _concatenator.__
-00018d20: 6e61 6d65 5f5f 7d20 7769 6474 6822 2c0a  name__} width",.
-00018d30: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
-00018d40: 653d 7769 6474 685f 7078 2c0a 2020 2020  e=width_px,.    
-00018d50: 2020 2020 2020 2020 6d69 6e5f 7661 6c75          min_valu
-00018d60: 653d 312c 0a20 2020 2020 2020 2029 0a20  e=1,.        ). 
-00018d70: 2020 2020 2020 2077 6964 7468 203d 2069         width = i
-00018d80: 6e74 2877 6964 7468 5f70 7829 0a20 2020  nt(width_px).   
-00018d90: 2076 6964 656f 5f70 6174 685f 7374 7220   video_path_str 
-00018da0: 3d20 2220 222e 6a6f 696e 285b 6627 2d69  = " ".join([f'-i
-00018db0: 2022 7b70 6174 687d 2227 2066 6f72 2070   "{path}"' for p
-00018dc0: 6174 6820 696e 2076 6964 656f 5f70 6174  ath in video_pat
-00018dd0: 6873 5d29 0a20 2020 2063 6f64 6563 203d  hs]).    codec =
-00018de0: 2022 6832 3634 5f6e 7665 6e63 2220 6966   "h264_nvenc" if
-00018df0: 2067 7075 2065 6c73 6520 226c 6962 7670   gpu else "libvp
-00018e00: 782d 7670 3922 0a20 2020 2066 696c 7465  x-vp9".    filte
-00018e10: 725f 636f 6d70 6c65 7820 3d20 223b 222e  r_complex = ";".
-00018e20: 6a6f 696e 280a 2020 2020 2020 2020 5b66  join(.        [f
-00018e30: 225b 7b69 6478 7d3a 765d 7363 616c 653d  "[{idx}:v]scale=
-00018e40: 7b77 6964 7468 7d3a 2d31 5b76 7b69 6478  {width}:-1[v{idx
-00018e50: 7d5d 2220 666f 7220 6964 7820 696e 2072  }]" for idx in r
-00018e60: 616e 6765 286c 656e 2876 6964 656f 5f70  ange(len(video_p
-00018e70: 6174 6873 2929 5d0a 2020 2020 290a 2020  aths))].    ).  
-00018e80: 2020 6669 6c74 6572 5f63 6f6d 706c 6578    filter_complex
-00018e90: 202b 3d20 6622 3b7b 2727 2e6a 6f69 6e28   += f";{''.join(
-00018ea0: 5b66 275b 767b 6964 787d 5d27 2066 6f72  [f'[v{idx}]' for
-00018eb0: 2069 6478 2069 6e20 7261 6e67 6528 6c65   idx in range(le
-00018ec0: 6e28 7669 6465 6f5f 7061 7468 7329 295d  n(video_paths))]
-00018ed0: 297d 220a 2020 2020 6669 6c74 6572 5f63  )}".    filter_c
-00018ee0: 6f6d 706c 6578 202b 3d20 6622 7673 7461  omplex += f"vsta
-00018ef0: 636b 3d69 6e70 7574 733d 7b6c 656e 2876  ck=inputs={len(v
-00018f00: 6964 656f 5f70 6174 6873 297d 5b76 5d22  ideo_paths)}[v]"
-00018f10: 0a20 2020 2069 6620 7665 7262 6f73 653a  .    if verbose:
-00018f20: 0a20 2020 2020 2020 2070 7269 6e74 280a  .        print(.
-00018f30: 2020 2020 2020 2020 2020 2020 6622 436f              f"Co
-00018f40: 6e63 6174 656e 6174 696e 6720 7b6c 656e  ncatenating {len
-00018f50: 2876 6964 656f 5f70 6174 6873 297d 2076  (video_paths)} v
-00018f60: 6964 656f 7320 7665 7274 6963 616c 6c79  ideos vertically
-00018f70: 2077 6974 6820 6120 7b77 6964 7468 7d20   with a {width} 
-00018f80: 7069 7865 6c20 7769 6474 682e 2e2e 220a  pixel width...".
-00018f90: 2020 2020 2020 2020 290a 2020 2020 636d          ).    cm
-00018fa0: 6420 3d20 6627 6666 6d70 6567 207b 7669  d = f'ffmpeg {vi
-00018fb0: 6465 6f5f 7061 7468 5f73 7472 7d20 2d66  deo_path_str} -f
-00018fc0: 696c 7465 725f 636f 6d70 6c65 7820 227b  ilter_complex "{
-00018fd0: 6669 6c74 6572 5f63 6f6d 706c 6578 7d22  filter_complex}"
-00018fe0: 202d 6d61 7020 225b 765d 2220 2d63 3a76   -map "[v]" -c:v
-00018ff0: 207b 636f 6465 637d 202d 6c6f 676c 6576   {codec} -loglev
-00019000: 656c 2065 7272 6f72 202d 7374 6174 7320  el error -stats 
-00019010: 227b 7361 7665 5f70 6174 687d 2220 2d79  "{save_path}" -y
-00019020: 270a 2020 2020 7375 6270 726f 6365 7373  '.    subprocess
-00019030: 2e63 616c 6c28 636d 642c 2073 6865 6c6c  .call(cmd, shell
-00019040: 3d54 7275 652c 2073 7464 6f75 743d 7375  =True, stdout=su
-00019050: 6270 726f 6365 7373 2e50 4950 4529 0a20  bprocess.PIPE). 
-00019060: 2020 2074 696d 6572 2e73 746f 705f 7469     timer.stop_ti
-00019070: 6d65 7228 290a 2020 2020 6966 2076 6572  mer().    if ver
-00019080: 626f 7365 3a0a 2020 2020 2020 2020 7072  bose:.        pr
-00019090: 696e 7428 0a20 2020 2020 2020 2020 2020  int(.           
-000190a0: 2066 2256 6572 7469 6361 6c20 636f 6e63   f"Vertical conc
-000190b0: 6174 656e 6174 696f 6e20 636f 6d70 6c65  atenation comple
-000190c0: 7465 2e20 5361 7665 6420 6174 207b 7361  te. Saved at {sa
-000190d0: 7665 5f70 6174 687d 2028 456c 6170 7365  ve_path} (Elapse
-000190e0: 6420 7469 6d65 3a20 7b74 696d 6572 2e65  d time: {timer.e
-000190f0: 6c61 7073 6564 5f74 696d 655f 7374 727d  lapsed_time_str}
-00019100: 732e 2922 0a20 2020 2020 2020 2029 0a0a  s.)".        )..
-00019110: 0a64 6566 206d 6f73 6169 635f 636f 6e63  .def mosaic_conc
-00019120: 6174 656e 6174 6f72 280a 2020 2020 7669  atenator(.    vi
-00019130: 6465 6f5f 7061 7468 733a 204c 6973 745b  deo_paths: List[
-00019140: 556e 696f 6e5b 7374 722c 206f 732e 5061  Union[str, os.Pa
-00019150: 7468 4c69 6b65 5d5d 2c0a 2020 2020 7361  thLike]],.    sa
-00019160: 7665 5f70 6174 683a 2055 6e69 6f6e 5b73  ve_path: Union[s
-00019170: 7472 2c20 6f73 2e50 6174 684c 696b 655d  tr, os.PathLike]
-00019180: 2c0a 2020 2020 7769 6474 685f 6964 783a  ,.    width_idx:
-00019190: 204f 7074 696f 6e61 6c5b 556e 696f 6e5b   Optional[Union[
-000191a0: 696e 742c 2073 7472 5d5d 203d 204e 6f6e  int, str]] = Non
-000191b0: 652c 0a20 2020 2077 6964 7468 5f70 783a  e,.    width_px:
-000191c0: 204f 7074 696f 6e61 6c5b 556e 696f 6e5b   Optional[Union[
-000191d0: 696e 742c 2073 7472 5d5d 203d 204e 6f6e  int, str]] = Non
-000191e0: 652c 0a20 2020 2068 6569 6768 745f 6964  e,.    height_id
-000191f0: 783a 204f 7074 696f 6e61 6c5b 556e 696f  x: Optional[Unio
-00019200: 6e5b 696e 742c 2073 7472 5d5d 203d 204e  n[int, str]] = N
-00019210: 6f6e 652c 0a20 2020 2068 6569 6768 745f  one,.    height_
-00019220: 7078 3a20 4f70 7469 6f6e 616c 5b55 6e69  px: Optional[Uni
-00019230: 6f6e 5b69 6e74 2c20 7374 725d 5d20 3d20  on[int, str]] = 
-00019240: 4e6f 6e65 2c0a 2020 2020 6770 753a 204f  None,.    gpu: O
-00019250: 7074 696f 6e61 6c5b 626f 6f6c 5d20 3d20  ptional[bool] = 
-00019260: 4661 6c73 652c 0a20 2020 2076 6572 626f  False,.    verbo
-00019270: 7365 3a20 4f70 7469 6f6e 616c 5b62 6f6f  se: Optional[boo
-00019280: 6c5d 203d 2054 7275 652c 0a20 2020 2075  l] = True,.    u
-00019290: 6e65 7665 6e5f 6669 6c6c 5f63 6f6c 6f72  neven_fill_color
-000192a0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
-000192b0: 3d20 2262 6c61 636b 222c 0a29 202d 3e20  = "black",.) -> 
-000192c0: 4e6f 6e65 3a0a 2020 2020 2222 220a 2020  None:.    """.  
-000192d0: 2020 436f 6e63 6174 656e 6174 6573 206d    Concatenates m
-000192e0: 756c 7469 706c 6520 7669 6465 6f73 2069  ultiple videos i
-000192f0: 6e74 6f20 6120 6d6f 7361 6963 206c 6179  nto a mosaic lay
-00019300: 6f75 742e 0a0a 2020 2020 2e2e 2069 6d61  out...    .. ima
-00019310: 6765 3a3a 205f 7374 6174 6963 2f69 6d67  ge:: _static/img
-00019320: 2f6d 6f73 6169 635f 636f 6e63 6174 656e  /mosaic_concaten
-00019330: 6174 6f72 2e70 6e67 0a20 2020 2020 2020  ator.png.       
-00019340: 3a77 6964 7468 3a20 3630 300a 2020 2020  :width: 600.    
-00019350: 2020 203a 616c 6967 6e3a 2063 656e 7465     :align: cente
-00019360: 720a 0a20 2020 202e 2e20 6e6f 7465 3a3a  r..    .. note::
-00019370: 0a20 2020 2020 2020 6966 2061 6e20 756e  .       if an un
-00019380: 6576 656e 206e 756d 6265 7220 6f66 2076  even number of v
-00019390: 6964 656f 732c 2074 6865 206c 6173 7420  ideos, the last 
-000193a0: 696e 6465 7820 7769 6c6c 2062 6520 6669  index will be fi
-000193b0: 6c6c 6564 2062 7920 6060 756e 6576 656e  lled by ``uneven
-000193c0: 5f66 696c 6c5f 636f 6c6f 7260 602e 0a0a  _fill_color``...
-000193d0: 2020 2020 3a70 6172 616d 204c 6973 745b      :param List[
-000193e0: 556e 696f 6e5b 7374 722c 206f 732e 5061  Union[str, os.Pa
-000193f0: 7468 4c69 6b65 5d5d 2076 6964 656f 5f70  thLike]] video_p
-00019400: 6174 6873 3a20 4c69 7374 206f 6620 696e  aths: List of in
-00019410: 7075 7420 7669 6465 6f20 6669 6c65 2070  put video file p
-00019420: 6174 6873 2e0a 2020 2020 3a70 6172 616d  aths..    :param
-00019430: 2055 6e69 6f6e 5b73 7472 2c20 6f73 2e50   Union[str, os.P
-00019440: 6174 684c 696b 655d 2073 6176 655f 7061  athLike] save_pa
-00019450: 7468 3a20 4669 6c65 2070 6174 6820 746f  th: File path to
-00019460: 2073 6176 6520 7468 6520 636f 6e63 6174   save the concat
-00019470: 656e 6174 6564 2076 6964 656f 2e0a 2020  enated video..  
-00019480: 2020 3a70 6172 616d 204f 7074 696f 6e61    :param Optiona
-00019490: 6c5b 696e 745d 2077 6964 7468 5f70 783a  l[int] width_px:
-000194a0: 2057 6964 7468 206f 6620 7468 6520 6f75   Width of the ou
-000194b0: 7470 7574 2076 6964 656f 2069 6e20 7069  tput video in pi
-000194c0: 7865 6c73 2e0a 2020 2020 3a70 6172 616d  xels..    :param
-000194d0: 204f 7074 696f 6e61 6c5b 696e 745d 2077   Optional[int] w
-000194e0: 6964 7468 5f69 6478 3a20 496e 6465 7820  idth_idx: Index 
-000194f0: 6f66 2074 6865 2076 6964 656f 2074 6f20  of the video to 
-00019500: 7573 6520 666f 7220 6465 7465 726d 696e  use for determin
-00019510: 696e 6720 7769 6474 682e 0a20 2020 203a  ing width..    :
-00019520: 7061 7261 6d20 4f70 7469 6f6e 616c 5b69  param Optional[i
-00019530: 6e74 5d20 6865 6967 6874 5f70 783a 2048  nt] height_px: H
-00019540: 6569 6768 7420 6f66 2074 6865 206f 7574  eight of the out
-00019550: 7075 7420 7669 6465 6f20 7061 6e65 6c73  put video panels
-00019560: 2069 6e20 7069 7865 6c73 2e0a 2020 2020   in pixels..    
-00019570: 3a70 6172 616d 204f 7074 696f 6e61 6c5b  :param Optional[
-00019580: 696e 745d 2068 6569 6768 745f 6964 783a  int] height_idx:
-00019590: 2048 6569 6768 7420 6f66 2074 6865 2076   Height of the v
-000195a0: 6964 656f 2074 6f20 7573 6520 666f 7220  ideo to use for 
-000195b0: 6465 7465 726d 696e 696e 6720 7769 6474  determining widt
-000195c0: 682e 0a20 2020 203a 7061 7261 6d20 4f70  h..    :param Op
-000195d0: 7469 6f6e 616c 5b62 6f6f 6c5d 2067 7075  tional[bool] gpu
-000195e0: 3a20 5768 6574 6865 7220 746f 2075 7365  : Whether to use
-000195f0: 2047 5055 2d61 6363 656c 6572 6174 6564   GPU-accelerated
-00019600: 2063 6f64 6563 2028 6465 6661 756c 743a   codec (default:
-00019610: 2046 616c 7365 292e 0a20 2020 203a 7061   False)..    :pa
-00019620: 7261 6d20 4f70 7469 6f6e 616c 5b62 6f6f  ram Optional[boo
-00019630: 6c5d 2076 6572 626f 7365 3a20 5768 6574  l] verbose: Whet
-00019640: 6865 7220 746f 2070 7269 6e74 2070 726f  her to print pro
-00019650: 6772 6573 7320 6d65 7373 6167 6573 2028  gress messages (
-00019660: 6465 6661 756c 743a 2054 7275 6529 2e0a  default: True)..
-00019670: 0a20 2020 203a 6578 616d 706c 653a 0a20  .    :example:. 
-00019680: 2020 203e 3e3e 2076 6964 656f 5f70 6174     >>> video_pat
-00019690: 6873 203d 205b 272f 5573 6572 732f 7369  hs = ['/Users/si
-000196a0: 6d6f 6e2f 4465 736b 746f 702f 656e 7673  mon/Desktop/envs
-000196b0: 2f73 696d 6261 2f74 726f 7562 6c65 7368  /simba/troublesh
-000196c0: 6f6f 7469 6e67 2f52 4154 5f4e 4f52 2f70  ooting/RAT_NOR/p
-000196d0: 726f 6a65 6374 5f66 6f6c 6465 722f 7669  roject_folder/vi
-000196e0: 6465 6f73 2f74 6573 742f 3038 3130 3230  deos/test/081020
-000196f0: 3231 5f44 4f54 5f52 6174 375f 3828 3229  21_DOT_Rat7_8(2)
-00019700: 2e6d 7034 272c 2027 2f55 7365 7273 2f73  .mp4', '/Users/s
-00019710: 696d 6f6e 2f44 6573 6b74 6f70 2f65 6e76  imon/Desktop/env
-00019720: 732f 7369 6d62 612f 7472 6f75 626c 6573  s/simba/troubles
-00019730: 686f 6f74 696e 672f 5241 545f 4e4f 522f  hooting/RAT_NOR/
-00019740: 7072 6f6a 6563 745f 666f 6c64 6572 2f76  project_folder/v
-00019750: 6964 656f 732f 7465 7374 2f30 3831 3032  ideos/test/08102
-00019760: 3032 315f 444f 545f 5261 7431 315f 3132  021_DOT_Rat11_12
-00019770: 2e6d 7034 272c 2027 2f55 7365 7273 2f73  .mp4', '/Users/s
-00019780: 696d 6f6e 2f44 6573 6b74 6f70 2f65 6e76  imon/Desktop/env
-00019790: 732f 7369 6d62 612f 7472 6f75 626c 6573  s/simba/troubles
-000197a0: 686f 6f74 696e 672f 5241 545f 4e4f 522f  hooting/RAT_NOR/
-000197b0: 7072 6f6a 6563 745f 666f 6c64 6572 2f76  project_folder/v
-000197c0: 6964 656f 732f 7465 7374 2f6e 6577 2f32  ideos/test/new/2
-000197d0: 3032 322d 3036 2d32 315f 4e4f 425f 494f  022-06-21_NOB_IO
-000197e0: 545f 3233 2e6d 7034 275d 0a20 2020 203e  T_23.mp4'].    >
-000197f0: 3e3e 2073 6176 655f 7061 7468 203d 2027  >> save_path = '
-00019800: 2f55 7365 7273 2f73 696d 6f6e 2f44 6573  /Users/simon/Des
-00019810: 6b74 6f70 2f65 6e76 732f 7369 6d62 612f  ktop/envs/simba/
-00019820: 7472 6f75 626c 6573 686f 6f74 696e 672f  troubleshooting/
-00019830: 5241 545f 4e4f 522f 7072 6f6a 6563 745f  RAT_NOR/project_
-00019840: 666f 6c64 6572 2f76 6964 656f 732f 7465  folder/videos/te
-00019850: 7374 2f6e 6577 2f62 6c61 6e6b 5f74 6573  st/new/blank_tes
-00019860: 742e 6d70 3427 0a20 2020 203e 3e3e 206d  t.mp4'.    >>> m
-00019870: 6f73 6169 635f 636f 6e63 6174 656e 6174  osaic_concatenat
-00019880: 6f72 2876 6964 656f 5f70 6174 6873 3d76  or(video_paths=v
-00019890: 6964 656f 5f70 6174 6873 2c20 7361 7665  ideo_paths, save
-000198a0: 5f70 6174 683d 7361 7665 5f70 6174 682c  _path=save_path,
-000198b0: 2077 6964 7468 5f69 6478 3d31 2c20 6865   width_idx=1, he
-000198c0: 6967 6874 5f69 6478 3d31 2c20 6770 753d  ight_idx=1, gpu=
-000198d0: 4661 6c73 6529 0a20 2020 2022 2222 0a0a  False).    """..
-000198e0: 2020 2020 6368 6563 6b5f 6666 6d70 6567      check_ffmpeg
-000198f0: 5f61 7661 696c 6162 6c65 2829 0a20 2020  _available().   
-00019900: 2069 6620 6770 7520 616e 6420 6e6f 7420   if gpu and not 
-00019910: 6368 6563 6b5f 6e76 6964 6561 5f67 7075  check_nvidea_gpu
-00019920: 5f61 7661 696c 6162 6c65 2829 3a0a 2020  _available():.  
-00019930: 2020 2020 2020 7261 6973 6520 4646 4d50        raise FFMP
-00019940: 4547 436f 6465 6347 5055 4572 726f 7228  EGCodecGPUError(
-00019950: 0a20 2020 2020 2020 2020 2020 206d 7367  .            msg
-00019960: 3d22 4e56 4944 4941 2047 5055 206e 6f74  ="NVIDIA GPU not
-00019970: 2061 7661 696c 6162 6c65 222c 2073 6f75   available", sou
-00019980: 7263 653d 6d6f 7361 6963 5f63 6f6e 6361  rce=mosaic_conca
-00019990: 7465 6e61 746f 722e 5f5f 6e61 6d65 5f5f  tenator.__name__
-000199a0: 0a20 2020 2020 2020 2029 0a20 2020 2074  .        ).    t
-000199b0: 696d 6572 203d 2053 696d 6261 5469 6d65  imer = SimbaTime
-000199c0: 7228 7374 6172 743d 5472 7565 290a 2020  r(start=True).  
-000199d0: 2020 6474 203d 2064 6174 6574 696d 652e    dt = datetime.
-000199e0: 6e6f 7728 292e 7374 7266 7469 6d65 2822  now().strftime("
-000199f0: 2559 256d 2564 2548 254d 2553 2229 0a20  %Y%m%d%H%M%S"). 
-00019a00: 2020 2063 6865 636b 5f76 616c 6964 5f6c     check_valid_l
-00019a10: 7374 280a 2020 2020 2020 2020 6461 7461  st(.        data
-00019a20: 3d76 6964 656f 5f70 6174 6873 2c0a 2020  =video_paths,.  
-00019a30: 2020 2020 2020 736f 7572 6365 3d66 227b        source=f"{
-00019a40: 6d6f 7361 6963 5f63 6f6e 6361 7465 6e61  mosaic_concatena
-00019a50: 746f 722e 5f5f 6e61 6d65 5f5f 7d20 7669  tor.__name__} vi
-00019a60: 6465 6f5f 7061 7468 7322 2c0a 2020 2020  deo_paths",.    
-00019a70: 2020 2020 6d69 6e5f 6c65 6e3d 332c 0a20      min_len=3,. 
-00019a80: 2020 2029 0a20 2020 2076 6964 656f 5f6d     ).    video_m
-00019a90: 6574 615f 6461 7461 203d 205b 0a20 2020  eta_data = [.   
-00019aa0: 2020 2020 2067 6574 5f76 6964 656f 5f6d       get_video_m
-00019ab0: 6574 615f 6461 7461 2876 6964 656f 5f70  eta_data(video_p
-00019ac0: 6174 683d 7669 6465 6f5f 7061 7468 2920  ath=video_path) 
-00019ad0: 666f 7220 7669 6465 6f5f 7061 7468 2069  for video_path i
-00019ae0: 6e20 7669 6465 6f5f 7061 7468 730a 2020  n video_paths.  
-00019af0: 2020 5d0a 2020 2020 6d61 785f 7669 6465    ].    max_vide
-00019b00: 6f5f 6c65 6e67 7468 203d 206d 6178 285b  o_length = max([
-00019b10: 785b 2276 6964 656f 5f6c 656e 6774 685f  x["video_length_
-00019b20: 7322 5d20 666f 7220 7820 696e 2076 6964  s"] for x in vid
-00019b30: 656f 5f6d 6574 615f 6461 7461 5d29 0a20  eo_meta_data]). 
-00019b40: 2020 2069 6620 2828 7769 6474 685f 7078     if ((width_px
-00019b50: 2069 7320 4e6f 6e65 2920 616e 6420 2877   is None) and (w
-00019b60: 6964 7468 5f69 6478 2069 7320 4e6f 6e65  idth_idx is None
-00019b70: 2929 206f 7220 280a 2020 2020 2020 2020  )) or (.        
-00019b80: 2877 6964 7468 5f70 7820 6973 206e 6f74  (width_px is not
-00019b90: 204e 6f6e 6529 2061 6e64 2028 7769 6474   None) and (widt
-00019ba0: 685f 6964 7820 6973 206e 6f74 204e 6f6e  h_idx is not Non
-00019bb0: 6529 0a20 2020 2029 3a0a 2020 2020 2020  e).    ):.      
-00019bc0: 2020 7261 6973 6520 496e 7661 6c69 6449    raise InvalidI
-00019bd0: 6e70 7574 4572 726f 7228 0a20 2020 2020  nputError(.     
-00019be0: 2020 2020 2020 206d 7367 3d22 5072 6f76         msg="Prov
-00019bf0: 6964 6520 6120 7769 6474 685f 7078 204f  ide a width_px O
-00019c00: 5220 7769 6474 685f 6964 7822 2c20 736f  R width_idx", so
-00019c10: 7572 6365 3d6d 6f73 6169 635f 636f 6e63  urce=mosaic_conc
-00019c20: 6174 656e 6174 6f72 2e5f 5f6e 616d 655f  atenator.__name_
-00019c30: 5f0a 2020 2020 2020 2020 290a 2020 2020  _.        ).    
-00019c40: 6966 2028 2868 6569 6768 745f 7078 2069  if ((height_px i
-00019c50: 7320 4e6f 6e65 2920 616e 6420 2868 6569  s None) and (hei
-00019c60: 6768 745f 6964 7820 6973 204e 6f6e 6529  ght_idx is None)
-00019c70: 2920 6f72 2028 0a20 2020 2020 2020 2028  ) or (.        (
-00019c80: 6865 6967 6874 5f70 7820 6973 206e 6f74  height_px is not
-00019c90: 204e 6f6e 6529 2061 6e64 2028 6865 6967   None) and (heig
-00019ca0: 6874 5f69 6478 2069 7320 6e6f 7420 4e6f  ht_idx is not No
-00019cb0: 6e65 290a 2020 2020 293a 0a20 2020 2020  ne).    ):.     
-00019cc0: 2020 2072 6169 7365 2049 6e76 616c 6964     raise Invalid
-00019cd0: 496e 7075 7445 7272 6f72 280a 2020 2020  InputError(.    
-00019ce0: 2020 2020 2020 2020 6d73 673d 2250 726f          msg="Pro
-00019cf0: 7669 6465 2061 2068 6569 6768 745f 7078  vide a height_px
-00019d00: 204f 5220 6865 6967 6874 5f69 6478 222c   OR height_idx",
-00019d10: 2073 6f75 7263 653d 6d6f 7361 6963 5f63   source=mosaic_c
-00019d20: 6f6e 6361 7465 6e61 746f 722e 5f5f 6e61  oncatenator.__na
-00019d30: 6d65 5f5f 0a20 2020 2020 2020 2029 0a20  me__.        ). 
-00019d40: 2020 2069 6620 7769 6474 685f 6964 7820     if width_idx 
-00019d50: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00019d60: 2020 2020 2063 6865 636b 5f69 6e74 280a       check_int(.
-00019d70: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
-00019d80: 3d66 227b 7665 7274 6963 616c 5f76 6964  =f"{vertical_vid
-00019d90: 656f 5f63 6f6e 6361 7465 6e61 746f 722e  eo_concatenator.
-00019da0: 5f5f 6e61 6d65 5f5f 7d20 7769 6474 6820  __name__} width 
-00019db0: 696e 6465 7822 2c0a 2020 2020 2020 2020  index",.        
-00019dc0: 2020 2020 7661 6c75 653d 7769 6474 685f      value=width_
-00019dd0: 6964 782c 0a20 2020 2020 2020 2020 2020  idx,.           
-00019de0: 206d 696e 5f76 616c 7565 3d31 2c0a 2020   min_value=1,.  
-00019df0: 2020 2020 2020 2020 2020 6d61 785f 7661            max_va
-00019e00: 6c75 653d 6c65 6e28 7669 6465 6f5f 7061  lue=len(video_pa
-00019e10: 7468 7329 202d 2031 2c0a 2020 2020 2020  ths) - 1,.      
-00019e20: 2020 290a 2020 2020 2020 2020 7769 6474    ).        widt
-00019e30: 6820 3d20 696e 7428 7669 6465 6f5f 6d65  h = int(video_me
-00019e40: 7461 5f64 6174 615b 7769 6474 685f 6964  ta_data[width_id
-00019e50: 785d 5b22 7769 6474 6822 5d29 0a20 2020  x]["width"]).   
-00019e60: 2065 6c73 653a 0a20 2020 2020 2020 2077   else:.        w
-00019e70: 6964 7468 203d 2077 6964 7468 5f70 780a  idth = width_px.
-00019e80: 2020 2020 6966 2068 6569 6768 745f 6964      if height_id
-00019e90: 7820 6973 206e 6f74 204e 6f6e 653a 0a20  x is not None:. 
-00019ea0: 2020 2020 2020 2063 6865 636b 5f69 6e74         check_int
-00019eb0: 280a 2020 2020 2020 2020 2020 2020 6e61  (.            na
-00019ec0: 6d65 3d66 227b 7665 7274 6963 616c 5f76  me=f"{vertical_v
-00019ed0: 6964 656f 5f63 6f6e 6361 7465 6e61 746f  ideo_concatenato
-00019ee0: 722e 5f5f 6e61 6d65 5f5f 7d20 6865 6967  r.__name__} heig
-00019ef0: 6874 2069 6e64 6578 222c 0a20 2020 2020  ht index",.     
-00019f00: 2020 2020 2020 2076 616c 7565 3d77 6964         value=wid
-00019f10: 7468 5f69 6478 2c0a 2020 2020 2020 2020  th_idx,.        
-00019f20: 2020 2020 6d69 6e5f 7661 6c75 653d 312c      min_value=1,
-00019f30: 0a20 2020 2020 2020 2020 2020 206d 6178  .            max
-00019f40: 5f76 616c 7565 3d6c 656e 2876 6964 656f  _value=len(video
-00019f50: 5f70 6174 6873 2920 2d20 312c 0a20 2020  _paths) - 1,.   
-00019f60: 2020 2020 2029 0a20 2020 2020 2020 2068       ).        h
-00019f70: 6569 6768 7420 3d20 696e 7428 7669 6465  eight = int(vide
-00019f80: 6f5f 6d65 7461 5f64 6174 615b 7769 6474  o_meta_data[widt
-00019f90: 685f 6964 785d 5b22 6865 6967 6874 225d  h_idx]["height"]
-00019fa0: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
-00019fb0: 2020 2020 6865 6967 6874 203d 2068 6569      height = hei
-00019fc0: 6768 745f 7078 0a20 2020 2069 6620 7665  ght_px.    if ve
-00019fd0: 7262 6f73 653a 0a20 2020 2020 2020 2070  rbose:.        p
-00019fe0: 7269 6e74 2866 2243 7265 6174 696e 6720  rint(f"Creating 
-00019ff0: 6d6f 7361 6963 2076 6964 656f 202e 2e2e  mosaic video ...
-0001a000: 2229 0a20 2020 2074 656d 705f 6469 7220  ").    temp_dir 
-0001a010: 3d20 6f73 2e70 6174 682e 6a6f 696e 286f  = os.path.join(o
-0001a020: 732e 7061 7468 2e64 6972 6e61 6d65 2876  s.path.dirname(v
-0001a030: 6964 656f 5f70 6174 6873 5b30 5d29 2c20  ideo_paths[0]), 
-0001a040: 6622 7465 6d70 5f7b 6474 7d22 290a 2020  f"temp_{dt}").  
-0001a050: 2020 6f73 2e6d 616b 6564 6972 7328 7465    os.makedirs(te
-0001a060: 6d70 5f64 6972 290a 2020 2020 6966 206e  mp_dir).    if n
-0001a070: 6f74 2028 6c65 6e28 7669 6465 6f5f 7061  ot (len(video_pa
-0001a080: 7468 7329 2025 2032 2920 3d3d 2030 3a0a  ths) % 2) == 0:.
-0001a090: 2020 2020 2020 2020 626c 616e 6b5f 7061          blank_pa
-0001a0a0: 7468 203d 206f 732e 7061 7468 2e6a 6f69  th = os.path.joi
-0001a0b0: 6e28 7465 6d70 5f64 6972 2c20 6622 7b64  n(temp_dir, f"{d
-0001a0c0: 747d 2e6d 7034 2229 0a20 2020 2020 2020  t}.mp4").       
-0001a0d0: 2063 7265 6174 655f 626c 616e 6b5f 7669   create_blank_vi
-0001a0e0: 6465 6f28 0a20 2020 2020 2020 2020 2020  deo(.           
-0001a0f0: 2070 6174 683d 626c 616e 6b5f 7061 7468   path=blank_path
-0001a100: 2c0a 2020 2020 2020 2020 2020 2020 6c65  ,.            le
-0001a110: 6e67 7468 3d6d 6178 5f76 6964 656f 5f6c  ngth=max_video_l
-0001a120: 656e 6774 682c 0a20 2020 2020 2020 2020  ength,.         
-0001a130: 2020 2077 6964 7468 3d77 6964 7468 2c0a     width=width,.
-0001a140: 2020 2020 2020 2020 2020 2020 6865 6967              heig
-0001a150: 6874 3d68 6569 6768 742c 0a20 2020 2020  ht=height,.     
-0001a160: 2020 2020 2020 2067 7075 3d67 7075 2c0a         gpu=gpu,.
-0001a170: 2020 2020 2020 2020 2020 2020 7665 7262              verb
-0001a180: 6f73 653d 7665 7262 6f73 652c 0a20 2020  ose=verbose,.   
-0001a190: 2020 2020 2020 2020 2063 6f6c 6f72 3d75           color=u
-0001a1a0: 6e65 7665 6e5f 6669 6c6c 5f63 6f6c 6f72  neven_fill_color
-0001a1b0: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
-0001a1c0: 2020 2020 7669 6465 6f5f 7061 7468 732e      video_paths.
-0001a1d0: 6170 7065 6e64 2862 6c61 6e6b 5f70 6174  append(blank_pat
-0001a1e0: 6829 0a20 2020 2075 7070 6572 5f76 6964  h).    upper_vid
-0001a1f0: 656f 732c 206c 6f77 6572 5f76 6964 656f  eos, lower_video
-0001a200: 7320 3d20 280a 2020 2020 2020 2020 7669  s = (.        vi
-0001a210: 6465 6f5f 7061 7468 735b 3a20 6c65 6e28  deo_paths[: len(
-0001a220: 7669 6465 6f5f 7061 7468 7329 202f 2f20  video_paths) // 
-0001a230: 325d 2c0a 2020 2020 2020 2020 7669 6465  2],.        vide
-0001a240: 6f5f 7061 7468 735b 6c65 6e28 7669 6465  o_paths[len(vide
-0001a250: 6f5f 7061 7468 7329 202f 2f20 3220 3a5d  o_paths) // 2 :]
-0001a260: 2c0a 2020 2020 290a 2020 2020 6966 2076  ,.    ).    if v
-0001a270: 6572 626f 7365 3a0a 2020 2020 2020 2020  erbose:.        
-0001a280: 7072 696e 7428 2243 7265 6174 696e 6720  print("Creating 
-0001a290: 7570 7065 7220 6d6f 7361 6963 2e2e 2e20  upper mosaic... 
-0001a2a0: 2853 7465 7020 312f 3329 2229 0a20 2020  (Step 1/3)").   
-0001a2b0: 2069 6620 6c65 6e28 7570 7065 725f 7669   if len(upper_vi
-0001a2c0: 6465 6f73 2920 3e20 313a 0a20 2020 2020  deos) > 1:.     
-0001a2d0: 2020 2075 7070 6572 5f70 6174 6820 3d20     upper_path = 
-0001a2e0: 6f73 2e70 6174 682e 6a6f 696e 2874 656d  os.path.join(tem
-0001a2f0: 705f 6469 722c 2022 7570 7065 722e 6d70  p_dir, "upper.mp
-0001a300: 3422 290a 2020 2020 2020 2020 686f 7269  4").        hori
-0001a310: 7a6f 6e74 616c 5f76 6964 656f 5f63 6f6e  zontal_video_con
-0001a320: 6361 7465 6e61 746f 7228 0a20 2020 2020  catenator(.     
-0001a330: 2020 2020 2020 2076 6964 656f 5f70 6174         video_pat
-0001a340: 6873 3d75 7070 6572 5f76 6964 656f 732c  hs=upper_videos,
-0001a350: 0a20 2020 2020 2020 2020 2020 2073 6176  .            sav
-0001a360: 655f 7061 7468 3d75 7070 6572 5f70 6174  e_path=upper_pat
-0001a370: 682c 0a20 2020 2020 2020 2020 2020 2067  h,.            g
-0001a380: 7075 3d67 7075 2c0a 2020 2020 2020 2020  pu=gpu,.        
-0001a390: 2020 2020 6865 6967 6874 5f70 783d 6865      height_px=he
-0001a3a0: 6967 6874 2c0a 2020 2020 2020 2020 2020  ight,.          
-0001a3b0: 2020 7665 7262 6f73 653d 7665 7262 6f73    verbose=verbos
-0001a3c0: 652c 0a20 2020 2020 2020 2029 0a20 2020  e,.        ).   
-0001a3d0: 2065 6c73 653a 0a20 2020 2020 2020 2075   else:.        u
-0001a3e0: 7070 6572 5f70 6174 6820 3d20 7570 7065  pper_path = uppe
-0001a3f0: 725f 7669 6465 6f73 5b30 5d0a 2020 2020  r_videos[0].    
-0001a400: 6966 2076 6572 626f 7365 3a0a 2020 2020  if verbose:.    
-0001a410: 2020 2020 7072 696e 7428 2243 7265 6174      print("Creat
-0001a420: 696e 6720 6c6f 7765 7220 6d6f 7361 6963  ing lower mosaic
-0001a430: 2e2e 2e20 2853 7465 7020 322f 3329 2229  ... (Step 2/3)")
-0001a440: 0a20 2020 2069 6620 6c65 6e28 6c6f 7765  .    if len(lowe
-0001a450: 725f 7669 6465 6f73 2920 3e20 313a 0a20  r_videos) > 1:. 
-0001a460: 2020 2020 2020 206c 6f77 6572 5f70 6174         lower_pat
-0001a470: 6820 3d20 6f73 2e70 6174 682e 6a6f 696e  h = os.path.join
-0001a480: 2874 656d 705f 6469 722c 2022 6c6f 7765  (temp_dir, "lowe
-0001a490: 722e 6d70 3422 290a 2020 2020 2020 2020  r.mp4").        
-0001a4a0: 686f 7269 7a6f 6e74 616c 5f76 6964 656f  horizontal_video
-0001a4b0: 5f63 6f6e 6361 7465 6e61 746f 7228 0a20  _concatenator(. 
-0001a4c0: 2020 2020 2020 2020 2020 2076 6964 656f             video
-0001a4d0: 5f70 6174 6873 3d6c 6f77 6572 5f76 6964  _paths=lower_vid
-0001a4e0: 656f 732c 0a20 2020 2020 2020 2020 2020  eos,.           
-0001a4f0: 2073 6176 655f 7061 7468 3d6c 6f77 6572   save_path=lower
-0001a500: 5f70 6174 682c 0a20 2020 2020 2020 2020  _path,.         
-0001a510: 2020 2067 7075 3d67 7075 2c0a 2020 2020     gpu=gpu,.    
-0001a520: 2020 2020 2020 2020 6865 6967 6874 5f70          height_p
-0001a530: 783d 6865 6967 6874 2c0a 2020 2020 2020  x=height,.      
-0001a540: 2020 2020 2020 7665 7262 6f73 653d 7665        verbose=ve
-0001a550: 7262 6f73 652c 0a20 2020 2020 2020 2029  rbose,.        )
-0001a560: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
-0001a570: 2020 206c 6f77 6572 5f70 6174 6820 3d20     lower_path = 
-0001a580: 6c6f 7765 725f 7669 6465 6f73 5b30 5d0a  lower_videos[0].
-0001a590: 2020 2020 7061 6e65 6c73 5f6d 6574 6120      panels_meta 
-0001a5a0: 3d20 5b0a 2020 2020 2020 2020 6765 745f  = [.        get_
-0001a5b0: 7669 6465 6f5f 6d65 7461 5f64 6174 6128  video_meta_data(
-0001a5c0: 7669 6465 6f5f 7061 7468 3d76 6964 656f  video_path=video
-0001a5d0: 5f70 6174 6829 0a20 2020 2020 2020 2066  _path).        f
-0001a5e0: 6f72 2076 6964 656f 5f70 6174 6820 696e  or video_path in
-0001a5f0: 205b 6c6f 7765 725f 7061 7468 2c20 7570   [lower_path, up
-0001a600: 7065 725f 7061 7468 5d0a 2020 2020 5d0a  per_path].    ].
-0001a610: 2020 2020 6966 2076 6572 626f 7365 3a0a      if verbose:.
-0001a620: 2020 2020 2020 2020 7072 696e 7428 224a          print("J
-0001a630: 6f69 6e69 6e67 2075 7070 6572 2061 6e64  oining upper and
-0001a640: 206c 6f77 6572 206d 6f73 6169 632e 2e2e   lower mosaic...
-0001a650: 2028 5374 6570 2032 2f33 2922 290a 2020   (Step 2/3)").  
-0001a660: 2020 7665 7274 6963 616c 5f76 6964 656f    vertical_video
-0001a670: 5f63 6f6e 6361 7465 6e61 746f 7228 0a20  _concatenator(. 
-0001a680: 2020 2020 2020 2076 6964 656f 5f70 6174         video_pat
-0001a690: 6873 3d5b 7570 7065 725f 7061 7468 2c20  hs=[upper_path, 
-0001a6a0: 6c6f 7765 725f 7061 7468 5d2c 0a20 2020  lower_path],.   
-0001a6b0: 2020 2020 2073 6176 655f 7061 7468 3d73       save_path=s
-0001a6c0: 6176 655f 7061 7468 2c0a 2020 2020 2020  ave_path,.      
-0001a6d0: 2020 7665 7262 6f73 653d 7665 7262 6f73    verbose=verbos
-0001a6e0: 652c 0a20 2020 2020 2020 2067 7075 3d67  e,.        gpu=g
-0001a6f0: 7075 2c0a 2020 2020 2020 2020 7769 6474  pu,.        widt
-0001a700: 685f 7078 3d6d 6178 285b 785b 2277 6964  h_px=max([x["wid
-0001a710: 7468 225d 2066 6f72 2078 2069 6e20 7061  th"] for x in pa
-0001a720: 6e65 6c73 5f6d 6574 615d 292c 0a20 2020  nels_meta]),.   
-0001a730: 2029 0a20 2020 2074 696d 6572 2e73 746f   ).    timer.sto
-0001a740: 705f 7469 6d65 7228 290a 2020 2020 7368  p_timer().    sh
-0001a750: 7574 696c 2e72 6d74 7265 6528 7465 6d70  util.rmtree(temp
-0001a760: 5f64 6972 290a 2020 2020 6966 2076 6572  _dir).    if ver
-0001a770: 626f 7365 3a0a 2020 2020 2020 2020 7072  bose:.        pr
-0001a780: 696e 7428 0a20 2020 2020 2020 2020 2020  int(.           
-0001a790: 2066 224d 6f73 6169 6320 636f 6e63 6174   f"Mosaic concat
-0001a7a0: 656e 6174 696f 6e20 636f 6d70 6c65 7465  enation complete
-0001a7b0: 2e20 5361 7665 6420 6174 207b 7361 7665  . Saved at {save
-0001a7c0: 5f70 6174 687d 2028 456c 6170 7365 6420  _path} (Elapsed 
-0001a7d0: 7469 6d65 3a20 7b74 696d 6572 2e65 6c61  time: {timer.ela
-0001a7e0: 7073 6564 5f74 696d 655f 7374 727d 732e  psed_time_str}s.
-0001a7f0: 2922 0a20 2020 2020 2020 2029 0a0a 0a64  )".        )...d
-0001a800: 6566 206d 6978 6564 5f6d 6f73 6169 635f  ef mixed_mosaic_
-0001a810: 636f 6e63 6174 656e 6174 6f72 280a 2020  concatenator(.  
-0001a820: 2020 7669 6465 6f5f 7061 7468 733a 204c    video_paths: L
-0001a830: 6973 745b 556e 696f 6e5b 7374 722c 206f  ist[Union[str, o
-0001a840: 732e 5061 7468 4c69 6b65 5d5d 2c0a 2020  s.PathLike]],.  
-0001a850: 2020 7361 7665 5f70 6174 683a 2055 6e69    save_path: Uni
-0001a860: 6f6e 5b73 7472 2c20 6f73 2e50 6174 684c  on[str, os.PathL
-0001a870: 696b 655d 2c0a 2020 2020 6770 753a 204f  ike],.    gpu: O
-0001a880: 7074 696f 6e61 6c5b 626f 6f6c 5d20 3d20  ptional[bool] = 
-0001a890: 4661 6c73 652c 0a20 2020 2076 6572 626f  False,.    verbo
-0001a8a0: 7365 3a20 4f70 7469 6f6e 616c 5b62 6f6f  se: Optional[boo
-0001a8b0: 6c5d 203d 2054 7275 652c 0a20 2020 2075  l] = True,.    u
-0001a8c0: 6e65 7665 6e5f 6669 6c6c 5f63 6f6c 6f72  neven_fill_color
-0001a8d0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
-0001a8e0: 3d20 2262 6c61 636b 222c 0a29 202d 3e20  = "black",.) -> 
-0001a8f0: 4e6f 6e65 3a0a 2020 2020 2222 220a 2020  None:.    """.  
-0001a900: 2020 4372 6561 7465 2061 206d 6978 6564    Create a mixed
-0001a910: 206d 6f73 6169 6320 7669 6465 6f20 6279   mosaic video by
-0001a920: 2063 6f6e 6361 7465 6e61 7469 6e67 206d   concatenating m
-0001a930: 756c 7469 706c 6520 696e 7075 7420 7669  ultiple input vi
-0001a940: 6465 6f73 2069 6e20 6120 6d6f 7361 6963  deos in a mosaic
-0001a950: 206c 6179 6f75 7420 6f66 2076 6172 696f   layout of vario
-0001a960: 7573 2073 697a 6573 2e0a 0a20 2020 202e  us sizes...    .
-0001a970: 2e20 696d 6167 653a 3a20 5f73 7461 7469  . image:: _stati
-0001a980: 632f 696d 672f 6d69 7865 645f 6d6f 7361  c/img/mixed_mosa
-0001a990: 6963 5f63 6f6e 6361 7465 6e61 746f 722e  ic_concatenator.
-0001a9a0: 706e 670a 2020 2020 2020 203a 7769 6474  png.       :widt
-0001a9b0: 683a 2036 3030 0a20 2020 2020 2020 3a61  h: 600.       :a
-0001a9c0: 6c69 676e 3a20 6365 6e74 6572 0a0a 2020  lign: center..  
-0001a9d0: 2020 2e2e 206e 6f74 653a 3a0a 2020 2020    .. note::.    
-0001a9e0: 2020 2054 6865 2072 6573 6f6c 7574 696f     The resolutio
-0001a9f0: 6e20 6f66 2074 6865 206f 7574 7075 7420  n of the output 
-0001aa00: 7669 6465 6f20 6973 2064 6574 6572 6d69  video is determi
-0001aa10: 6e65 6420 6279 2074 6865 2072 6573 6f6c  ned by the resol
-0001aa20: 7574 696f 6e20 6f66 2074 6865 2076 6964  ution of the vid
-0001aa30: 656f 2070 6174 6820 6174 2074 6865 2066  eo path at the f
-0001aa40: 6972 7374 2069 6e64 6578 2e0a 0a20 2020  irst index...   
-0001aa50: 2020 2020 4966 2061 6e20 756e 6576 656e      If an uneven
-0001aa60: 206e 756d 6265 7220 6f66 2072 6967 6874   number of right
-0001aa70: 2d70 616e 656c 2076 6964 656f 7320 2820  -panel videos ( 
-0001aa80: 6966 206e 6f74 2028 6c65 6e28 7669 6465  if not (len(vide
-0001aa90: 6f5f 7061 7468 7329 2d31 2920 2520 3229  o_paths)-1) % 2)
-0001aaa0: 203d 3d20 3029 2c20 7468 656e 2074 6865   == 0), then the
-0001aab0: 206c 6173 7420 696e 6465 7820 7769 6c6c   last index will
-0001aac0: 2062 6520 6669 6c6c 6564 2062 7920 6060   be filled by ``
-0001aad0: 756e 6576 656e 5f66 696c 6c5f 636f 6c6f  uneven_fill_colo
-0001aae0: 7260 602e 0a0a 2020 2020 3a70 6172 616d  r``...    :param
-0001aaf0: 204c 6973 745b 556e 696f 6e5b 7374 722c   List[Union[str,
-0001ab00: 206f 732e 5061 7468 4c69 6b65 5d5d 2076   os.PathLike]] v
-0001ab10: 6964 656f 5f70 6174 6873 3a20 4c69 7374  ideo_paths: List
-0001ab20: 206f 6620 696e 7075 7420 7669 6465 6f20   of input video 
-0001ab30: 6669 6c65 2070 6174 6873 2e0a 2020 2020  file paths..    
-0001ab40: 3a70 6172 616d 2055 6e69 6f6e 5b73 7472  :param Union[str
-0001ab50: 2c20 6f73 2e50 6174 684c 696b 655d 2073  , os.PathLike] s
-0001ab60: 6176 655f 7061 7468 3a20 4669 6c65 2070  ave_path: File p
-0001ab70: 6174 6820 746f 2073 6176 6520 7468 6520  ath to save the 
-0001ab80: 636f 6e63 6174 656e 6174 6564 2076 6964  concatenated vid
-0001ab90: 656f 2e0a 2020 2020 3a70 6172 616d 204f  eo..    :param O
-0001aba0: 7074 696f 6e61 6c5b 626f 6f6c 5d20 6770  ptional[bool] gp
-0001abb0: 753a 2057 6865 7468 6572 2074 6f20 7573  u: Whether to us
-0001abc0: 6520 4750 552d 6163 6365 6c65 7261 7465  e GPU-accelerate
-0001abd0: 6420 636f 6465 6320 2864 6566 6175 6c74  d codec (default
-0001abe0: 3a20 4661 6c73 6529 2e0a 2020 2020 3a70  : False)..    :p
-0001abf0: 6172 616d 204f 7074 696f 6e61 6c5b 626f  aram Optional[bo
-0001ac00: 6f6c 5d20 7665 7262 6f73 653a 2057 6865  ol] verbose: Whe
-0001ac10: 7468 6572 2074 6f20 7072 696e 7420 7072  ther to print pr
-0001ac20: 6f67 7265 7373 206d 6573 7361 6765 7320  ogress messages 
-0001ac30: 2864 6566 6175 6c74 3a20 5472 7565 292e  (default: True).
-0001ac40: 0a0a 2020 2020 3a65 7861 6d70 6c65 3a0a  ..    :example:.
-0001ac50: 2020 2020 3e3e 3e20 7669 6465 6f5f 7061      >>> video_pa
-0001ac60: 7468 7320 3d20 5b27 7669 6465 6f31 2e6d  ths = ['video1.m
-0001ac70: 7034 272c 2027 7669 6465 6f32 2e6d 7034  p4', 'video2.mp4
-0001ac80: 272c 2027 7669 6465 6f33 2e6d 7034 275d  ', 'video3.mp4']
-0001ac90: 0a20 2020 203e 3e3e 2073 6176 655f 7061  .    >>> save_pa
-0001aca0: 7468 203d 2027 2f55 7365 7273 2f73 696d  th = '/Users/sim
-0001acb0: 6f6e 2f44 6573 6b74 6f70 2f65 6e76 732f  on/Desktop/envs/
-0001acc0: 7369 6d62 612f 7472 6f75 626c 6573 686f  simba/troublesho
-0001acd0: 6f74 696e 672f 5241 545f 4e4f 522f 7072  oting/RAT_NOR/pr
-0001ace0: 6f6a 6563 745f 666f 6c64 6572 2f76 6964  oject_folder/vid
-0001acf0: 656f 732f 7465 7374 2f6e 6577 2f62 6c61  eos/test/new/bla
-0001ad00: 6e6b 5f74 6573 742e 6d70 3427 0a20 2020  nk_test.mp4'.   
-0001ad10: 203e 3e3e 206d 6978 6564 5f6d 6f73 6169   >>> mixed_mosai
-0001ad20: 635f 636f 6e63 6174 656e 6174 6f72 2876  c_concatenator(v
-0001ad30: 6964 656f 5f70 6174 6873 3d76 6964 656f  ideo_paths=video
-0001ad40: 5f70 6174 6873 2c20 7361 7665 5f70 6174  _paths, save_pat
-0001ad50: 683d 7361 7665 5f70 6174 682c 2067 7075  h=save_path, gpu
-0001ad60: 3d46 616c 7365 2c20 7665 7262 6f73 653d  =False, verbose=
-0001ad70: 5472 7565 290a 2020 2020 2222 220a 0a20  True).    """.. 
-0001ad80: 2020 2063 6865 636b 5f66 666d 7065 675f     check_ffmpeg_
-0001ad90: 6176 6169 6c61 626c 6528 290a 2020 2020  available().    
-0001ada0: 6966 2067 7075 2061 6e64 206e 6f74 2063  if gpu and not c
-0001adb0: 6865 636b 5f6e 7669 6465 615f 6770 755f  heck_nvidea_gpu_
-0001adc0: 6176 6169 6c61 626c 6528 293a 0a20 2020  available():.   
-0001add0: 2020 2020 2072 6169 7365 2046 464d 5045       raise FFMPE
-0001ade0: 4743 6f64 6563 4750 5545 7272 6f72 280a  GCodecGPUError(.
-0001adf0: 2020 2020 2020 2020 2020 2020 6d73 673d              msg=
-0001ae00: 224e 5649 4449 4120 4750 5520 6e6f 7420  "NVIDIA GPU not 
-0001ae10: 6176 6169 6c61 626c 6522 2c20 736f 7572  available", sour
-0001ae20: 6365 3d6d 6978 6564 5f6d 6f73 6169 635f  ce=mixed_mosaic_
-0001ae30: 636f 6e63 6174 656e 6174 6f72 2e5f 5f6e  concatenator.__n
-0001ae40: 616d 655f 5f0a 2020 2020 2020 2020 290a  ame__.        ).
-0001ae50: 2020 2020 7469 6d65 7220 3d20 5369 6d62      timer = Simb
-0001ae60: 6154 696d 6572 2873 7461 7274 3d54 7275  aTimer(start=Tru
-0001ae70: 6529 0a20 2020 2063 6865 636b 5f76 616c  e).    check_val
-0001ae80: 6964 5f6c 7374 280a 2020 2020 2020 2020  id_lst(.        
-0001ae90: 6461 7461 3d76 6964 656f 5f70 6174 6873  data=video_paths
-0001aea0: 2c20 736f 7572 6365 3d6d 6978 6564 5f6d  , source=mixed_m
-0001aeb0: 6f73 6169 635f 636f 6e63 6174 656e 6174  osaic_concatenat
-0001aec0: 6f72 2e5f 5f6e 616d 655f 5f2c 206d 696e  or.__name__, min
-0001aed0: 5f6c 656e 3d32 0a20 2020 2029 0a20 2020  _len=2.    ).   
-0001aee0: 2064 7420 3d20 6461 7465 7469 6d65 2e6e   dt = datetime.n
-0001aef0: 6f77 2829 2e73 7472 6674 696d 6528 2225  ow().strftime("%
-0001af00: 5925 6d25 6425 4825 4d25 5322 290a 2020  Y%m%d%H%M%S").  
-0001af10: 2020 7669 6465 6f5f 6d65 7461 5f64 6174    video_meta_dat
-0001af20: 6120 3d20 5b0a 2020 2020 2020 2020 6765  a = [.        ge
-0001af30: 745f 7669 6465 6f5f 6d65 7461 5f64 6174  t_video_meta_dat
-0001af40: 6128 7669 6465 6f5f 7061 7468 3d76 6964  a(video_path=vid
-0001af50: 656f 5f70 6174 6829 2066 6f72 2076 6964  eo_path) for vid
-0001af60: 656f 5f70 6174 6820 696e 2076 6964 656f  eo_path in video
-0001af70: 5f70 6174 6873 0a20 2020 205d 0a20 2020  _paths.    ].   
-0001af80: 206d 6178 5f76 6964 656f 5f6c 656e 6774   max_video_lengt
-0001af90: 6820 3d20 6d61 7828 5b78 5b22 7669 6465  h = max([x["vide
-0001afa0: 6f5f 6c65 6e67 7468 5f73 225d 2066 6f72  o_length_s"] for
-0001afb0: 2078 2069 6e20 7669 6465 6f5f 6d65 7461   x in video_meta
-0001afc0: 5f64 6174 615d 290a 2020 2020 6368 6563  _data]).    chec
-0001afd0: 6b5f 6966 5f64 6972 5f65 7869 7374 7328  k_if_dir_exists(
-0001afe0: 0a20 2020 2020 2020 2069 6e5f 6469 723d  .        in_dir=
-0001aff0: 6f73 2e70 6174 682e 6469 726e 616d 6528  os.path.dirname(
-0001b000: 7361 7665 5f70 6174 6829 2c20 736f 7572  save_path), sour
-0001b010: 6365 3d6d 6978 6564 5f6d 6f73 6169 635f  ce=mixed_mosaic_
-0001b020: 636f 6e63 6174 656e 6174 6f72 2e5f 5f6e  concatenator.__n
-0001b030: 616d 655f 5f0a 2020 2020 290a 2020 2020  ame__.    ).    
-0001b040: 6c61 7267 655f 6d6f 7361 6963 5f70 6174  large_mosaic_pat
-0001b050: 682c 2076 6964 656f 5f70 6174 6873 203d  h, video_paths =
-0001b060: 2076 6964 656f 5f70 6174 6873 5b30 5d2c   video_paths[0],
-0001b070: 2076 6964 656f 5f70 6174 6873 5b31 3a5d   video_paths[1:]
-0001b080: 0a20 2020 206d 6f73 6169 635f 6865 6967  .    mosaic_heig
-0001b090: 6874 203d 2069 6e74 2876 6964 656f 5f6d  ht = int(video_m
-0001b0a0: 6574 615f 6461 7461 5b30 5d5b 2268 6569  eta_data[0]["hei
-0001b0b0: 6768 7422 5d20 2f20 3229 0a20 2020 2069  ght"] / 2).    i
-0001b0c0: 6620 7665 7262 6f73 653a 0a20 2020 2020  f verbose:.     
-0001b0d0: 2020 2070 7269 6e74 2822 4372 6561 7469     print("Creati
-0001b0e0: 6e67 206d 6978 6564 206d 6f73 6169 6320  ng mixed mosaic 
-0001b0f0: 7669 6465 6f2e 2e2e 2022 290a 2020 2020  video... ").    
-0001b100: 7465 6d70 5f64 6972 203d 206f 732e 7061  temp_dir = os.pa
-0001b110: 7468 2e6a 6f69 6e28 6f73 2e70 6174 682e  th.join(os.path.
-0001b120: 6469 726e 616d 6528 7669 6465 6f5f 7061  dirname(video_pa
-0001b130: 7468 735b 305d 292c 2066 2274 656d 705f  ths[0]), f"temp_
-0001b140: 7b64 747d 2229 0a20 2020 206f 732e 6d61  {dt}").    os.ma
-0001b150: 6b65 6469 7273 2874 656d 705f 6469 7229  kedirs(temp_dir)
-0001b160: 0a20 2020 2069 6620 6e6f 7420 286c 656e  .    if not (len
-0001b170: 2876 6964 656f 5f70 6174 6873 2920 2520  (video_paths) % 
-0001b180: 3229 203d 3d20 303a 0a20 2020 2020 2020  2) == 0:.       
-0001b190: 2062 6c61 6e6b 5f70 6174 6820 3d20 6f73   blank_path = os
-0001b1a0: 2e70 6174 682e 6a6f 696e 2874 656d 705f  .path.join(temp_
-0001b1b0: 6469 722c 2066 227b 6474 7d2e 6d70 3422  dir, f"{dt}.mp4"
-0001b1c0: 290a 2020 2020 2020 2020 6372 6561 7465  ).        create
-0001b1d0: 5f62 6c61 6e6b 5f76 6964 656f 280a 2020  _blank_video(.  
-0001b1e0: 2020 2020 2020 2020 2020 7061 7468 3d62            path=b
-0001b1f0: 6c61 6e6b 5f70 6174 682c 0a20 2020 2020  lank_path,.     
-0001b200: 2020 2020 2020 206c 656e 6774 683d 6d61         length=ma
-0001b210: 785f 7669 6465 6f5f 6c65 6e67 7468 2c0a  x_video_length,.
-0001b220: 2020 2020 2020 2020 2020 2020 7769 6474              widt
-0001b230: 683d 7669 6465 6f5f 6d65 7461 5f64 6174  h=video_meta_dat
-0001b240: 615b 2d31 5d5b 2277 6964 7468 225d 2c0a  a[-1]["width"],.
-0001b250: 2020 2020 2020 2020 2020 2020 6865 6967              heig
-0001b260: 6874 3d6d 6f73 6169 635f 6865 6967 6874  ht=mosaic_height
-0001b270: 2c0a 2020 2020 2020 2020 2020 2020 6770  ,.            gp
-0001b280: 753d 6770 752c 0a20 2020 2020 2020 2020  u=gpu,.         
-0001b290: 2020 2076 6572 626f 7365 3d54 7275 652c     verbose=True,
-0001b2a0: 0a20 2020 2020 2020 2020 2020 2063 6f6c  .            col
-0001b2b0: 6f72 3d75 6e65 7665 6e5f 6669 6c6c 5f63  or=uneven_fill_c
-0001b2c0: 6f6c 6f72 2c0a 2020 2020 2020 2020 290a  olor,.        ).
-0001b2d0: 2020 2020 2020 2020 7669 6465 6f5f 7061          video_pa
-0001b2e0: 7468 732e 6170 7065 6e64 2862 6c61 6e6b  ths.append(blank
-0001b2f0: 5f70 6174 6829 0a20 2020 2075 7070 6572  _path).    upper
-0001b300: 5f76 6964 656f 732c 206c 6f77 6572 5f76  _videos, lower_v
-0001b310: 6964 656f 7320 3d20 280a 2020 2020 2020  ideos = (.      
-0001b320: 2020 7669 6465 6f5f 7061 7468 735b 3a20    video_paths[: 
-0001b330: 6c65 6e28 7669 6465 6f5f 7061 7468 7329  len(video_paths)
-0001b340: 202f 2f20 325d 2c0a 2020 2020 2020 2020   // 2],.        
-0001b350: 7669 6465 6f5f 7061 7468 735b 6c65 6e28  video_paths[len(
-0001b360: 7669 6465 6f5f 7061 7468 7329 202f 2f20  video_paths) // 
-0001b370: 3220 3a5d 2c0a 2020 2020 290a 2020 2020  2 :],.    ).    
-0001b380: 6966 2076 6572 626f 7365 3a0a 2020 2020  if verbose:.    
-0001b390: 2020 2020 7072 696e 7428 2243 7265 6174      print("Creat
-0001b3a0: 696e 6720 7570 7065 7220 7269 6768 7420  ing upper right 
-0001b3b0: 6d6f 7361 6963 202e 2e2e 2028 5374 6570  mosaic ... (Step
-0001b3c0: 2031 2f34 2922 290a 2020 2020 6966 206c   1/4)").    if l
-0001b3d0: 656e 2875 7070 6572 5f76 6964 656f 7329  en(upper_videos)
-0001b3e0: 203e 2031 3a0a 2020 2020 2020 2020 7570   > 1:.        up
-0001b3f0: 7065 725f 7061 7468 203d 206f 732e 7061  per_path = os.pa
-0001b400: 7468 2e6a 6f69 6e28 7465 6d70 5f64 6972  th.join(temp_dir
-0001b410: 2c20 2275 7070 6572 2e6d 7034 2229 0a20  , "upper.mp4"). 
-0001b420: 2020 2020 2020 2068 6f72 697a 6f6e 7461         horizonta
-0001b430: 6c5f 7669 6465 6f5f 636f 6e63 6174 656e  l_video_concaten
-0001b440: 6174 6f72 280a 2020 2020 2020 2020 2020  ator(.          
-0001b450: 2020 7669 6465 6f5f 7061 7468 733d 7570    video_paths=up
-0001b460: 7065 725f 7669 6465 6f73 2c0a 2020 2020  per_videos,.    
-0001b470: 2020 2020 2020 2020 7361 7665 5f70 6174          save_pat
-0001b480: 683d 7570 7065 725f 7061 7468 2c0a 2020  h=upper_path,.  
-0001b490: 2020 2020 2020 2020 2020 6770 753d 6770            gpu=gp
-0001b4a0: 752c 0a20 2020 2020 2020 2020 2020 2068  u,.            h
-0001b4b0: 6569 6768 745f 7078 3d6d 6f73 6169 635f  eight_px=mosaic_
-0001b4c0: 6865 6967 6874 2c0a 2020 2020 2020 2020  height,.        
-0001b4d0: 2020 2020 7665 7262 6f73 653d 7665 7262      verbose=verb
-0001b4e0: 6f73 652c 0a20 2020 2020 2020 2029 0a20  ose,.        ). 
-0001b4f0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0001b500: 2075 7070 6572 5f70 6174 6820 3d20 7570   upper_path = up
-0001b510: 7065 725f 7669 6465 6f73 5b30 5d0a 2020  per_videos[0].  
-0001b520: 2020 6966 2076 6572 626f 7365 3a0a 2020    if verbose:.  
-0001b530: 2020 2020 2020 7072 696e 7428 2243 7265        print("Cre
-0001b540: 6174 696e 6720 6c6f 7765 7220 7269 6768  ating lower righ
-0001b550: 7420 6d6f 7361 6963 202e 2e2e 2028 5374  t mosaic ... (St
-0001b560: 6570 2032 2f34 2922 290a 2020 2020 6966  ep 2/4)").    if
-0001b570: 206c 656e 286c 6f77 6572 5f76 6964 656f   len(lower_video
-0001b580: 7329 203e 2031 3a0a 2020 2020 2020 2020  s) > 1:.        
-0001b590: 6c6f 7765 725f 7061 7468 203d 206f 732e  lower_path = os.
-0001b5a0: 7061 7468 2e6a 6f69 6e28 7465 6d70 5f64  path.join(temp_d
-0001b5b0: 6972 2c20 226c 6f77 6572 2e6d 7034 2229  ir, "lower.mp4")
-0001b5c0: 0a20 2020 2020 2020 2068 6f72 697a 6f6e  .        horizon
-0001b5d0: 7461 6c5f 7669 6465 6f5f 636f 6e63 6174  tal_video_concat
-0001b5e0: 656e 6174 6f72 280a 2020 2020 2020 2020  enator(.        
-0001b5f0: 2020 2020 7669 6465 6f5f 7061 7468 733d      video_paths=
-0001b600: 6c6f 7765 725f 7669 6465 6f73 2c20 7361  lower_videos, sa
-0001b610: 7665 5f70 6174 683d 6c6f 7765 725f 7061  ve_path=lower_pa
-0001b620: 7468 2c20 6770 753d 6770 752c 2076 6572  th, gpu=gpu, ver
-0001b630: 626f 7365 3d76 6572 626f 7365 0a20 2020  bose=verbose.   
-0001b640: 2020 2020 2029 0a20 2020 2065 6c73 653a       ).    else:
-0001b650: 0a20 2020 2020 2020 206c 6f77 6572 5f70  .        lower_p
-0001b660: 6174 6820 3d20 6c6f 7765 725f 7669 6465  ath = lower_vide
-0001b670: 6f73 5b30 5d0a 2020 2020 7061 6e65 6c73  os[0].    panels
-0001b680: 5f6d 6574 6120 3d20 5b0a 2020 2020 2020  _meta = [.      
-0001b690: 2020 6765 745f 7669 6465 6f5f 6d65 7461    get_video_meta
-0001b6a0: 5f64 6174 6128 7669 6465 6f5f 7061 7468  _data(video_path
-0001b6b0: 3d76 6964 656f 5f70 6174 6829 0a20 2020  =video_path).   
-0001b6c0: 2020 2020 2066 6f72 2076 6964 656f 5f70       for video_p
-0001b6d0: 6174 6820 696e 205b 6c6f 7765 725f 7061  ath in [lower_pa
-0001b6e0: 7468 2c20 7570 7065 725f 7061 7468 5d0a  th, upper_path].
-0001b6f0: 2020 2020 5d0a 2020 2020 6d6f 7361 6963      ].    mosaic
-0001b700: 5f70 6174 6820 3d20 6f73 2e70 6174 682e  _path = os.path.
-0001b710: 6a6f 696e 2874 656d 705f 6469 722c 2022  join(temp_dir, "
-0001b720: 6d6f 7361 6963 2e6d 7034 2229 0a20 2020  mosaic.mp4").   
-0001b730: 2069 6620 7665 7262 6f73 653a 0a20 2020   if verbose:.   
-0001b740: 2020 2020 2070 7269 6e74 2822 4a6f 696e       print("Join
-0001b750: 696e 6720 7570 7065 7220 616e 6420 6c6f  ing upper and lo
-0001b760: 7765 7220 7269 6768 7420 6d6f 7361 6963  wer right mosaic
-0001b770: 2e2e 2e20 2853 7465 7020 332f 3429 2229  ... (Step 3/4)")
-0001b780: 0a20 2020 2076 6572 7469 6361 6c5f 7669  .    vertical_vi
-0001b790: 6465 6f5f 636f 6e63 6174 656e 6174 6f72  deo_concatenator
-0001b7a0: 280a 2020 2020 2020 2020 7669 6465 6f5f  (.        video_
-0001b7b0: 7061 7468 733d 5b75 7070 6572 5f70 6174  paths=[upper_pat
-0001b7c0: 682c 206c 6f77 6572 5f70 6174 685d 2c0a  h, lower_path],.
-0001b7d0: 2020 2020 2020 2020 7769 6474 685f 7078          width_px
-0001b7e0: 3d6d 696e 285b 785b 2277 6964 7468 225d  =min([x["width"]
-0001b7f0: 2066 6f72 2078 2069 6e20 7061 6e65 6c73   for x in panels
-0001b800: 5f6d 6574 615d 292c 0a20 2020 2020 2020  _meta]),.       
-0001b810: 2073 6176 655f 7061 7468 3d6d 6f73 6169   save_path=mosai
-0001b820: 635f 7061 7468 2c0a 2020 2020 2020 2020  c_path,.        
-0001b830: 6770 753d 6770 752c 0a20 2020 2020 2020  gpu=gpu,.       
-0001b840: 2076 6572 626f 7365 3d76 6572 626f 7365   verbose=verbose
-0001b850: 2c0a 2020 2020 290a 2020 2020 6966 2076  ,.    ).    if v
-0001b860: 6572 626f 7365 3a0a 2020 2020 2020 2020  erbose:.        
-0001b870: 7072 696e 7428 224a 6f69 6e69 6e67 206c  print("Joining l
-0001b880: 6566 7420 616e 6420 7269 6768 7420 6d6f  eft and right mo
-0001b890: 7361 6963 2e2e 2e20 2853 7465 7020 342f  saic... (Step 4/
-0001b8a0: 3429 2229 0a20 2020 2068 6f72 697a 6f6e  4)").    horizon
-0001b8b0: 7461 6c5f 7669 6465 6f5f 636f 6e63 6174  tal_video_concat
-0001b8c0: 656e 6174 6f72 280a 2020 2020 2020 2020  enator(.        
-0001b8d0: 7669 6465 6f5f 7061 7468 733d 5b6c 6172  video_paths=[lar
-0001b8e0: 6765 5f6d 6f73 6169 635f 7061 7468 2c20  ge_mosaic_path, 
-0001b8f0: 6d6f 7361 6963 5f70 6174 685d 2c0a 2020  mosaic_path],.  
-0001b900: 2020 2020 2020 6865 6967 6874 5f69 6478        height_idx
-0001b910: 3d30 2c0a 2020 2020 2020 2020 7361 7665  =0,.        save
-0001b920: 5f70 6174 683d 7361 7665 5f70 6174 682c  _path=save_path,
-0001b930: 0a20 2020 2020 2020 2067 7075 3d67 7075  .        gpu=gpu
-0001b940: 2c0a 2020 2020 290a 2020 2020 7469 6d65  ,.    ).    time
-0001b950: 722e 7374 6f70 5f74 696d 6572 2829 0a20  r.stop_timer(). 
-0001b960: 2020 2073 6875 7469 6c2e 726d 7472 6565     shutil.rmtree
-0001b970: 2874 656d 705f 6469 7229 0a20 2020 2069  (temp_dir).    i
-0001b980: 6620 7665 7262 6f73 653a 0a20 2020 2020  f verbose:.     
-0001b990: 2020 2070 7269 6e74 280a 2020 2020 2020     print(.      
-0001b9a0: 2020 2020 2020 6622 4d69 7865 6420 6d6f        f"Mixed mo
-0001b9b0: 7361 6963 2063 6f6e 6361 7465 6e61 7469  saic concatenati
-0001b9c0: 6f6e 2063 6f6d 706c 6574 652e 2053 6176  on complete. Sav
-0001b9d0: 6564 2061 7420 7b73 6176 655f 7061 7468  ed at {save_path
-0001b9e0: 7d20 2845 6c61 7073 6564 2074 696d 653a  } (Elapsed time:
-0001b9f0: 207b 7469 6d65 722e 656c 6170 7365 645f   {timer.elapsed_
-0001ba00: 7469 6d65 5f73 7472 7d73 2e29 220a 2020  time_str}s.)".  
-0001ba10: 2020 2020 2020 290a                            ).
+00017110: 7061 7468 292c 2073 6f75 7263 653d 6372  path), source=cr
+00017120: 6561 7465 5f62 6c61 6e6b 5f76 6964 656f  eate_blank_video
+00017130: 2e5f 5f6e 616d 655f 5f2c 2063 7265 6174  .__name__, creat
+00017140: 655f 6966 5f6e 6f74 5f65 7869 7374 3d54  e_if_not_exist=T
+00017150: 7275 6529 0a20 2020 2074 696d 6572 203d  rue).    timer =
+00017160: 2053 696d 6261 5469 6d65 7228 7374 6172   SimbaTimer(star
+00017170: 743d 5472 7565 290a 2020 2020 6966 2076  t=True).    if v
+00017180: 6572 626f 7365 3a0a 2020 2020 2020 2020  erbose:.        
+00017190: 7072 696e 7428 2243 7265 6174 696e 6720  print("Creating 
+000171a0: 626c 616e 6b20 7669 6465 6f2e 2e2e 2229  blank video...")
+000171b0: 0a20 2020 2069 6620 6770 753a 0a20 2020  .    if gpu:.   
+000171c0: 2020 2020 2063 6d64 203d 2066 2766 666d       cmd = f'ffm
+000171d0: 7065 6720 2d79 202d 7420 7b6c 656e 6774  peg -y -t {lengt
+000171e0: 687d 202d 6620 6c61 7666 6920 2d69 2063  h} -f lavfi -i c
+000171f0: 6f6c 6f72 3d63 3d7b 636f 6c6f 727d 3a73  olor=c={color}:s
+00017200: 3d7b 7769 6474 687d 787b 6865 6967 6874  ={width}x{height
+00017210: 7d20 2d63 3a76 2068 3236 345f 6e76 656e  } -c:v h264_nven
+00017220: 6320 2d70 7265 7365 7420 736c 6f77 202d  c -preset slow -
+00017230: 7475 6e65 2073 7469 6c6c 696d 6167 6520  tune stillimage 
+00017240: 2d70 6978 5f66 6d74 2079 7576 3432 3070  -pix_fmt yuv420p
+00017250: 2022 7b70 6174 687d 2220 2d68 6964 655f   "{path}" -hide_
+00017260: 6261 6e6e 6572 202d 6c6f 676c 6576 656c  banner -loglevel
+00017270: 2065 7272 6f72 202d 7927 0a20 2020 2065   error -y'.    e
+00017280: 6c73 653a 0a20 2020 2020 2020 2063 6d64  lse:.        cmd
+00017290: 203d 2066 2766 666d 7065 6720 2d79 202d   = f'ffmpeg -y -
+000172a0: 7420 7b6c 656e 6774 687d 202d 6620 6c61  t {length} -f la
+000172b0: 7666 6920 2d69 2063 6f6c 6f72 3d63 3d7b  vfi -i color=c={
+000172c0: 636f 6c6f 727d 3a73 3d7b 7769 6474 687d  color}:s={width}
+000172d0: 787b 6865 6967 6874 7d20 2d63 3a76 206c  x{height} -c:v l
+000172e0: 6962 7832 3634 202d 7475 6e65 2073 7469  ibx264 -tune sti
+000172f0: 6c6c 696d 6167 6520 2d70 6978 5f66 6d74  llimage -pix_fmt
+00017300: 2079 7576 3432 3070 2022 7b70 6174 687d   yuv420p "{path}
+00017310: 2220 2d68 6964 655f 6261 6e6e 6572 202d  " -hide_banner -
+00017320: 6c6f 676c 6576 656c 2065 7272 6f72 202d  loglevel error -
+00017330: 7927 0a20 2020 2073 7562 7072 6f63 6573  y'.    subproces
+00017340: 732e 6361 6c6c 2863 6d64 2c20 7368 656c  s.call(cmd, shel
+00017350: 6c3d 5472 7565 2c20 7374 646f 7574 3d73  l=True, stdout=s
+00017360: 7562 7072 6f63 6573 732e 5049 5045 290a  ubprocess.PIPE).
+00017370: 2020 2020 7469 6d65 722e 7374 6f70 5f74      timer.stop_t
+00017380: 696d 6572 2829 0a20 2020 2069 6620 7665  imer().    if ve
+00017390: 7262 6f73 653a 0a20 2020 2020 2020 2070  rbose:.        p
+000173a0: 7269 6e74 2866 2242 6c61 6e6b 2076 6964  rint(f"Blank vid
+000173b0: 656f 2063 6f6d 706c 6574 652e 2053 6176  eo complete. Sav
+000173c0: 6564 2061 7420 7b70 6174 687d 2e20 456c  ed at {path}. El
+000173d0: 6170 7365 6420 7469 6d65 3a20 7b74 696d  apsed time: {tim
+000173e0: 6572 2e65 6c61 7073 6564 5f74 696d 655f  er.elapsed_time_
+000173f0: 7374 727d 732e 2229 0a0a 0a64 6566 2068  str}s.")...def h
+00017400: 6f72 697a 6f6e 7461 6c5f 7669 6465 6f5f  orizontal_video_
+00017410: 636f 6e63 6174 656e 6174 6f72 280a 2020  concatenator(.  
+00017420: 2020 7669 6465 6f5f 7061 7468 733a 204c    video_paths: L
+00017430: 6973 745b 556e 696f 6e5b 7374 722c 206f  ist[Union[str, o
+00017440: 732e 5061 7468 4c69 6b65 5d5d 2c0a 2020  s.PathLike]],.  
+00017450: 2020 7361 7665 5f70 6174 683a 2055 6e69    save_path: Uni
+00017460: 6f6e 5b73 7472 2c20 6f73 2e50 6174 684c  on[str, os.PathL
+00017470: 696b 655d 2c0a 2020 2020 6865 6967 6874  ike],.    height
+00017480: 5f70 783a 204f 7074 696f 6e61 6c5b 556e  _px: Optional[Un
+00017490: 696f 6e5b 696e 742c 2073 7472 5d5d 203d  ion[int, str]] =
+000174a0: 204e 6f6e 652c 0a20 2020 2068 6569 6768   None,.    heigh
+000174b0: 745f 6964 783a 204f 7074 696f 6e61 6c5b  t_idx: Optional[
+000174c0: 556e 696f 6e5b 696e 742c 2073 7472 5d5d  Union[int, str]]
+000174d0: 203d 204e 6f6e 652c 0a20 2020 2067 7075   = None,.    gpu
+000174e0: 3a20 4f70 7469 6f6e 616c 5b62 6f6f 6c5d  : Optional[bool]
+000174f0: 203d 2046 616c 7365 2c0a 2020 2020 7665   = False,.    ve
+00017500: 7262 6f73 653a 204f 7074 696f 6e61 6c5b  rbose: Optional[
+00017510: 626f 6f6c 5d20 3d20 5472 7565 2c0a 2920  bool] = True,.) 
+00017520: 2d3e 204e 6f6e 653a 0a20 2020 2022 2222  -> None:.    """
+00017530: 0a20 2020 2043 6f6e 6361 7465 6e61 7465  .    Concatenate
+00017540: 7320 6d75 6c74 6970 6c65 2076 6964 656f  s multiple video
+00017550: 7320 686f 7269 7a6f 6e74 616c 6c79 2e0a  s horizontally..
+00017560: 0a20 2020 202e 2e20 696d 6167 653a 3a20  .    .. image:: 
+00017570: 5f73 7461 7469 632f 696d 672f 686f 7269  _static/img/hori
+00017580: 7a6f 6e74 616c 5f76 6964 656f 5f63 6f6e  zontal_video_con
+00017590: 6361 7465 6e61 746f 722e 706e 670a 2020  catenator.png.  
+000175a0: 2020 2020 203a 7769 6474 683a 2033 3030       :width: 300
+000175b0: 0a20 2020 2020 2020 3a61 6c69 676e 3a20  .       :align: 
+000175c0: 6365 6e74 6572 0a0a 2020 2020 3a70 6172  center..    :par
+000175d0: 616d 204c 6973 745b 556e 696f 6e5b 7374  am List[Union[st
+000175e0: 722c 206f 732e 5061 7468 4c69 6b65 5d5d  r, os.PathLike]]
+000175f0: 2076 6964 656f 5f70 6174 6873 3a20 4c69   video_paths: Li
+00017600: 7374 206f 6620 696e 7075 7420 7669 6465  st of input vide
+00017610: 6f20 6669 6c65 2070 6174 6873 2e0a 2020  o file paths..  
+00017620: 2020 3a70 6172 616d 2055 6e69 6f6e 5b73    :param Union[s
+00017630: 7472 2c20 6f73 2e50 6174 684c 696b 655d  tr, os.PathLike]
+00017640: 2073 6176 655f 7061 7468 3a20 4669 6c65   save_path: File
+00017650: 2070 6174 6820 746f 2073 6176 6520 7468   path to save th
+00017660: 6520 636f 6e63 6174 656e 6174 6564 2076  e concatenated v
+00017670: 6964 656f 2e0a 2020 2020 3a70 6172 616d  ideo..    :param
+00017680: 204f 7074 696f 6e61 6c5b 696e 745d 2068   Optional[int] h
+00017690: 6569 6768 745f 7078 3a20 4865 6967 6874  eight_px: Height
+000176a0: 206f 6620 7468 6520 6f75 7470 7574 2076   of the output v
+000176b0: 6964 656f 2069 6e20 7069 7865 6c73 2e0a  ideo in pixels..
+000176c0: 2020 2020 3a70 6172 616d 204f 7074 696f      :param Optio
+000176d0: 6e61 6c5b 696e 745d 2068 6569 6768 745f  nal[int] height_
+000176e0: 6964 783a 2049 6e64 6578 206f 6620 7468  idx: Index of th
+000176f0: 6520 7669 6465 6f20 746f 2075 7365 2066  e video to use f
+00017700: 6f72 2064 6574 6572 6d69 6e69 6e67 2048  or determining H
+00017710: 6569 6768 742e 0a20 2020 203a 7061 7261  eight..    :para
+00017720: 6d20 4f70 7469 6f6e 616c 5b62 6f6f 6c5d  m Optional[bool]
+00017730: 2067 7075 3a20 5768 6574 6865 7220 746f   gpu: Whether to
+00017740: 2075 7365 2047 5055 2d61 6363 656c 6572   use GPU-acceler
+00017750: 6174 6564 2063 6f64 6563 2028 6465 6661  ated codec (defa
+00017760: 756c 743a 2046 616c 7365 292e 0a20 2020  ult: False)..   
+00017770: 203a 7061 7261 6d20 4f70 7469 6f6e 616c   :param Optional
+00017780: 5b62 6f6f 6c5d 2076 6572 626f 7365 3a57  [bool] verbose:W
+00017790: 6865 7468 6572 2074 6f20 7072 696e 7420  hether to print 
+000177a0: 7072 6f67 7265 7373 206d 6573 7361 6765  progress message
+000177b0: 7320 2864 6566 6175 6c74 3a20 5472 7565  s (default: True
+000177c0: 292e 0a0a 2020 2020 3a65 7861 6d70 6c65  )...    :example
+000177d0: 3a0a 2020 2020 3e3e 3e20 7669 6465 6f5f  :.    >>> video_
+000177e0: 7061 7468 7320 3d20 5b27 7669 6465 6f31  paths = ['video1
+000177f0: 2e6d 7034 272c 2027 7669 6465 6f32 2e6d  .mp4', 'video2.m
+00017800: 7034 275d 0a20 2020 203e 3e3e 2078 203d  p4'].    >>> x =
+00017810: 2068 6f72 697a 6f6e 7461 6c5f 7669 6465   horizontal_vide
+00017820: 6f5f 636f 6e63 6174 656e 6174 6f72 2876  o_concatenator(v
+00017830: 6964 656f 5f70 6174 6873 3d76 6964 656f  ideo_paths=video
+00017840: 5f70 6174 6873 2c20 6865 6967 6874 5f70  _paths, height_p
+00017850: 783d 3530 2c20 7361 7665 5f70 6174 683d  x=50, save_path=
+00017860: 272f 5573 6572 732f 7369 6d6f 6e2f 4465  '/Users/simon/De
+00017870: 736b 746f 702f 656e 7673 2f73 696d 6261  sktop/envs/simba
+00017880: 2f74 726f 7562 6c65 7368 6f6f 7469 6e67  /troubleshooting
+00017890: 2f52 4154 5f4e 4f52 2f70 726f 6a65 6374  /RAT_NOR/project
+000178a0: 5f66 6f6c 6465 722f 7669 6465 6f73 2f74  _folder/videos/t
+000178b0: 6573 742f 6e65 772f 3038 3130 3230 3231  est/new/08102021
+000178c0: 5f44 4f54 5f52 6174 375f 3828 3229 5f2e  _DOT_Rat7_8(2)_.
+000178d0: 6d70 3427 2c20 6770 753d 4661 6c73 6529  mp4', gpu=False)
+000178e0: 0a20 2020 2022 2222 0a20 2020 2063 6865  .    """.    che
+000178f0: 636b 5f66 666d 7065 675f 6176 6169 6c61  ck_ffmpeg_availa
+00017900: 626c 6528 290a 2020 2020 6966 2067 7075  ble().    if gpu
+00017910: 2061 6e64 206e 6f74 2063 6865 636b 5f6e   and not check_n
+00017920: 7669 6465 615f 6770 755f 6176 6169 6c61  videa_gpu_availa
+00017930: 626c 6528 293a 0a20 2020 2020 2020 2072  ble():.        r
+00017940: 6169 7365 2046 464d 5045 4743 6f64 6563  aise FFMPEGCodec
+00017950: 4750 5545 7272 6f72 280a 2020 2020 2020  GPUError(.      
+00017960: 2020 2020 2020 6d73 673d 224e 5649 4445        msg="NVIDE
+00017970: 4120 4750 5520 6e6f 7420 6176 6169 6c61  A GPU not availa
+00017980: 626c 6520 2861 7320 6576 616c 7561 7465  ble (as evaluate
+00017990: 6420 6279 206e 7669 6465 612d 736d 6920  d by nvidea-smi 
+000179a0: 7265 7475 726e 696e 6720 4e6f 6e65 2922  returning None)"
+000179b0: 2c0a 2020 2020 2020 2020 2020 2020 736f  ,.            so
+000179c0: 7572 6365 3d68 6f72 697a 6f6e 7461 6c5f  urce=horizontal_
+000179d0: 7669 6465 6f5f 636f 6e63 6174 656e 6174  video_concatenat
+000179e0: 6f72 2e5f 5f6e 616d 655f 5f2c 0a20 2020  or.__name__,.   
+000179f0: 2020 2020 2029 0a20 2020 2074 696d 6572       ).    timer
+00017a00: 203d 2053 696d 6261 5469 6d65 7228 7374   = SimbaTimer(st
+00017a10: 6172 743d 5472 7565 290a 2020 2020 6368  art=True).    ch
+00017a20: 6563 6b5f 7661 6c69 645f 6c73 7428 0a20  eck_valid_lst(. 
+00017a30: 2020 2020 2020 2064 6174 613d 7669 6465         data=vide
+00017a40: 6f5f 7061 7468 732c 2073 6f75 7263 653d  o_paths, source=
+00017a50: 686f 7269 7a6f 6e74 616c 5f76 6964 656f  horizontal_video
+00017a60: 5f63 6f6e 6361 7465 6e61 746f 722e 5f5f  _concatenator.__
+00017a70: 6e61 6d65 5f5f 2c20 6d69 6e5f 6c65 6e3d  name__, min_len=
+00017a80: 320a 2020 2020 290a 2020 2020 6368 6563  2.    ).    chec
+00017a90: 6b5f 6966 5f64 6972 5f65 7869 7374 7328  k_if_dir_exists(
+00017aa0: 0a20 2020 2020 2020 2069 6e5f 6469 723d  .        in_dir=
+00017ab0: 6f73 2e70 6174 682e 6469 726e 616d 6528  os.path.dirname(
+00017ac0: 7361 7665 5f70 6174 6829 2c20 736f 7572  save_path), sour
+00017ad0: 6365 3d68 6f72 697a 6f6e 7461 6c5f 7669  ce=horizontal_vi
+00017ae0: 6465 6f5f 636f 6e63 6174 656e 6174 6f72  deo_concatenator
+00017af0: 2e5f 5f6e 616d 655f 5f0a 2020 2020 290a  .__name__.    ).
+00017b00: 2020 2020 7669 6465 6f5f 6d65 7461 5f64      video_meta_d
+00017b10: 6174 6120 3d20 5b0a 2020 2020 2020 2020  ata = [.        
+00017b20: 6765 745f 7669 6465 6f5f 6d65 7461 5f64  get_video_meta_d
+00017b30: 6174 6128 7669 6465 6f5f 7061 7468 3d76  ata(video_path=v
+00017b40: 6964 656f 5f70 6174 6829 2066 6f72 2076  ideo_path) for v
+00017b50: 6964 656f 5f70 6174 6820 696e 2076 6964  ideo_path in vid
+00017b60: 656f 5f70 6174 6873 0a20 2020 205d 0a20  eo_paths.    ]. 
+00017b70: 2020 2069 6620 2828 6865 6967 6874 5f70     if ((height_p
+00017b80: 7820 6973 204e 6f6e 6529 2061 6e64 2028  x is None) and (
+00017b90: 6865 6967 6874 5f69 6478 2069 7320 4e6f  height_idx is No
+00017ba0: 6e65 2929 206f 7220 280a 2020 2020 2020  ne)) or (.      
+00017bb0: 2020 2868 6569 6768 745f 7078 2069 7320    (height_px is 
+00017bc0: 6e6f 7420 4e6f 6e65 2920 616e 6420 2868  not None) and (h
+00017bd0: 6569 6768 745f 6964 7820 6973 206e 6f74  eight_idx is not
+00017be0: 204e 6f6e 6529 0a20 2020 2029 3a0a 2020   None).    ):.  
+00017bf0: 2020 2020 2020 7261 6973 6520 496e 7661        raise Inva
+00017c00: 6c69 6449 6e70 7574 4572 726f 7228 0a20  lidInputError(. 
+00017c10: 2020 2020 2020 2020 2020 206d 7367 3d22             msg="
+00017c20: 5072 6f76 6964 6520 6120 6865 6967 6874  Provide a height
+00017c30: 5f70 7820 4f52 2068 6569 6768 745f 6964  _px OR height_id
+00017c40: 7822 2c0a 2020 2020 2020 2020 2020 2020  x",.            
+00017c50: 736f 7572 6365 3d68 6f72 697a 6f6e 7461  source=horizonta
+00017c60: 6c5f 7669 6465 6f5f 636f 6e63 6174 656e  l_video_concaten
+00017c70: 6174 6f72 2e5f 5f6e 616d 655f 5f2c 0a20  ator.__name__,. 
+00017c80: 2020 2020 2020 2029 0a20 2020 2069 6620         ).    if 
+00017c90: 6865 6967 6874 5f69 6478 2069 7320 6e6f  height_idx is no
+00017ca0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00017cb0: 6368 6563 6b5f 696e 7428 0a20 2020 2020  check_int(.     
+00017cc0: 2020 2020 2020 206e 616d 653d 6622 7b68         name=f"{h
+00017cd0: 6f72 697a 6f6e 7461 6c5f 7669 6465 6f5f  orizontal_video_
+00017ce0: 636f 6e63 6174 656e 6174 6f72 2e5f 5f6e  concatenator.__n
+00017cf0: 616d 655f 5f7d 2068 6569 6768 7422 2c0a  ame__} height",.
+00017d00: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
+00017d10: 653d 6865 6967 6874 5f69 6478 2c0a 2020  e=height_idx,.  
+00017d20: 2020 2020 2020 2020 2020 6d69 6e5f 7661            min_va
+00017d30: 6c75 653d 302c 0a20 2020 2020 2020 2020  lue=0,.         
+00017d40: 2020 206d 6178 5f76 616c 7565 3d6c 656e     max_value=len
+00017d50: 2876 6964 656f 5f70 6174 6873 2920 2d20  (video_paths) - 
+00017d60: 312c 0a20 2020 2020 2020 2029 0a20 2020  1,.        ).   
+00017d70: 2020 2020 2068 6569 6768 7420 3d20 696e       height = in
+00017d80: 7428 7669 6465 6f5f 6d65 7461 5f64 6174  t(video_meta_dat
+00017d90: 615b 6865 6967 6874 5f69 6478 5d5b 2268  a[height_idx]["h
+00017da0: 6569 6768 7422 5d29 0a20 2020 2065 6c73  eight"]).    els
+00017db0: 653a 0a20 2020 2020 2020 2063 6865 636b  e:.        check
+00017dc0: 5f69 6e74 280a 2020 2020 2020 2020 2020  _int(.          
+00017dd0: 2020 6e61 6d65 3d66 227b 686f 7269 7a6f    name=f"{horizo
+00017de0: 6e74 616c 5f76 6964 656f 5f63 6f6e 6361  ntal_video_conca
+00017df0: 7465 6e61 746f 722e 5f5f 6e61 6d65 5f5f  tenator.__name__
+00017e00: 7d20 6865 6967 6874 222c 0a20 2020 2020  } height",.     
+00017e10: 2020 2020 2020 2076 616c 7565 3d68 6569         value=hei
+00017e20: 6768 745f 7078 2c0a 2020 2020 2020 2020  ght_px,.        
+00017e30: 2020 2020 6d69 6e5f 7661 6c75 653d 312c      min_value=1,
+00017e40: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+00017e50: 2020 2068 6569 6768 7420 3d20 696e 7428     height = int(
+00017e60: 6865 6967 6874 5f70 7829 0a20 2020 2076  height_px).    v
+00017e70: 6964 656f 5f70 6174 685f 7374 7220 3d20  ideo_path_str = 
+00017e80: 2220 222e 6a6f 696e 285b 6627 2d69 2022  " ".join([f'-i "
+00017e90: 7b70 6174 687d 2227 2066 6f72 2070 6174  {path}"' for pat
+00017ea0: 6820 696e 2076 6964 656f 5f70 6174 6873  h in video_paths
+00017eb0: 5d29 0a20 2020 2063 6f64 6563 203d 2022  ]).    codec = "
+00017ec0: 6832 3634 5f6e 7665 6e63 2220 6966 2067  h264_nvenc" if g
+00017ed0: 7075 2065 6c73 6520 226c 6962 7670 782d  pu else "libvpx-
+00017ee0: 7670 3922 0a20 2020 2066 696c 7465 725f  vp9".    filter_
+00017ef0: 636f 6d70 6c65 7820 3d20 223b 222e 6a6f  complex = ";".jo
+00017f00: 696e 280a 2020 2020 2020 2020 5b66 225b  in(.        [f"[
+00017f10: 7b69 6478 7d3a 765d 7363 616c 653d 2d31  {idx}:v]scale=-1
+00017f20: 3a7b 6865 6967 6874 7d5b 767b 6964 787d  :{height}[v{idx}
+00017f30: 5d22 2066 6f72 2069 6478 2069 6e20 7261  ]" for idx in ra
+00017f40: 6e67 6528 6c65 6e28 7669 6465 6f5f 7061  nge(len(video_pa
+00017f50: 7468 7329 295d 0a20 2020 2029 0a20 2020  ths))].    ).   
+00017f60: 2066 696c 7465 725f 636f 6d70 6c65 7820   filter_complex 
+00017f70: 2b3d 2066 223b 7b27 272e 6a6f 696e 285b  += f";{''.join([
+00017f80: 6627 5b76 7b69 6478 7d5d 2720 666f 7220  f'[v{idx}]' for 
+00017f90: 6964 7820 696e 2072 616e 6765 286c 656e  idx in range(len
+00017fa0: 2876 6964 656f 5f70 6174 6873 2929 5d29  (video_paths))])
+00017fb0: 7d68 7374 6163 6b3d 696e 7075 7473 3d7b  }hstack=inputs={
+00017fc0: 6c65 6e28 7669 6465 6f5f 7061 7468 7329  len(video_paths)
+00017fd0: 7d5b 765d 220a 2020 2020 6966 2076 6572  }[v]".    if ver
+00017fe0: 626f 7365 3a0a 2020 2020 2020 2020 7072  bose:.        pr
+00017ff0: 696e 7428 0a20 2020 2020 2020 2020 2020  int(.           
+00018000: 2066 2243 6f6e 6361 7465 6e61 7469 6e67   f"Concatenating
+00018010: 207b 6c65 6e28 7669 6465 6f5f 7061 7468   {len(video_path
+00018020: 7329 7d20 7669 6465 6f73 2068 6f72 697a  s)} videos horiz
+00018030: 6f6e 7461 6c6c 7920 7769 7468 2061 207b  ontally with a {
+00018040: 6865 6967 6874 7d20 7069 7865 6c20 6865  height} pixel he
+00018050: 6967 6874 2e2e 2e20 220a 2020 2020 2020  ight... ".      
+00018060: 2020 290a 2020 2020 636d 6420 3d20 6627    ).    cmd = f'
+00018070: 6666 6d70 6567 207b 7669 6465 6f5f 7061  ffmpeg {video_pa
+00018080: 7468 5f73 7472 7d20 2d66 696c 7465 725f  th_str} -filter_
+00018090: 636f 6d70 6c65 7820 227b 6669 6c74 6572  complex "{filter
+000180a0: 5f63 6f6d 706c 6578 7d22 202d 6d61 7020  _complex}" -map 
+000180b0: 225b 765d 2220 2d63 3a76 207b 636f 6465  "[v]" -c:v {code
+000180c0: 637d 202d 6c6f 676c 6576 656c 2065 7272  c} -loglevel err
+000180d0: 6f72 202d 7374 6174 7320 227b 7361 7665  or -stats "{save
+000180e0: 5f70 6174 687d 2220 2d79 270a 2020 2020  _path}" -y'.    
+000180f0: 7375 6270 726f 6365 7373 2e63 616c 6c28  subprocess.call(
+00018100: 636d 642c 2073 6865 6c6c 3d54 7275 652c  cmd, shell=True,
+00018110: 2073 7464 6f75 743d 7375 6270 726f 6365   stdout=subproce
+00018120: 7373 2e50 4950 4529 0a20 2020 2074 696d  ss.PIPE).    tim
+00018130: 6572 2e73 746f 705f 7469 6d65 7228 290a  er.stop_timer().
+00018140: 2020 2020 6966 2076 6572 626f 7365 3a0a      if verbose:.
+00018150: 2020 2020 2020 2020 7072 696e 7428 0a20          print(. 
+00018160: 2020 2020 2020 2020 2020 2066 2248 6f72             f"Hor
+00018170: 697a 6f6e 7461 6c20 636f 6e63 6174 656e  izontal concaten
+00018180: 6174 696f 6e20 636f 6d70 6c65 7465 2c20  ation complete, 
+00018190: 7361 7665 6420 6174 207b 7361 7665 5f70  saved at {save_p
+000181a0: 6174 687d 2028 656c 6170 7365 6420 7469  ath} (elapsed ti
+000181b0: 6d65 3a20 7b74 696d 6572 2e65 6c61 7073  me: {timer.elaps
+000181c0: 6564 5f74 696d 655f 7374 727d 732e 2922  ed_time_str}s.)"
+000181d0: 0a20 2020 2020 2020 2029 0a0a 0a64 6566  .        )...def
+000181e0: 2076 6572 7469 6361 6c5f 7669 6465 6f5f   vertical_video_
+000181f0: 636f 6e63 6174 656e 6174 6f72 280a 2020  concatenator(.  
+00018200: 2020 7669 6465 6f5f 7061 7468 733a 204c    video_paths: L
+00018210: 6973 745b 556e 696f 6e5b 7374 722c 206f  ist[Union[str, o
+00018220: 732e 5061 7468 4c69 6b65 5d5d 2c0a 2020  s.PathLike]],.  
+00018230: 2020 7361 7665 5f70 6174 683a 2055 6e69    save_path: Uni
+00018240: 6f6e 5b73 7472 2c20 6f73 2e50 6174 684c  on[str, os.PathL
+00018250: 696b 655d 2c0a 2020 2020 7769 6474 685f  ike],.    width_
+00018260: 7078 3a20 4f70 7469 6f6e 616c 5b69 6e74  px: Optional[int
+00018270: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 7769  ] = None,.    wi
+00018280: 6474 685f 6964 783a 204f 7074 696f 6e61  dth_idx: Optiona
+00018290: 6c5b 696e 745d 203d 204e 6f6e 652c 0a20  l[int] = None,. 
+000182a0: 2020 2067 7075 3a20 4f70 7469 6f6e 616c     gpu: Optional
+000182b0: 5b62 6f6f 6c5d 203d 2046 616c 7365 2c0a  [bool] = False,.
+000182c0: 2020 2020 7665 7262 6f73 653a 204f 7074      verbose: Opt
+000182d0: 696f 6e61 6c5b 626f 6f6c 5d20 3d20 5472  ional[bool] = Tr
+000182e0: 7565 2c0a 2920 2d3e 204e 6f6e 653a 0a20  ue,.) -> None:. 
+000182f0: 2020 2022 2222 0a20 2020 2043 6f6e 6361     """.    Conca
+00018300: 7465 6e61 7465 7320 6d75 6c74 6970 6c65  tenates multiple
+00018310: 2076 6964 656f 7320 7665 7274 6963 616c   videos vertical
+00018320: 6c79 2e0a 0a20 2020 202e 2e20 696d 6167  ly...    .. imag
+00018330: 653a 3a20 5f73 7461 7469 632f 696d 672f  e:: _static/img/
+00018340: 7665 7274 6963 616c 5f76 6964 656f 5f63  vertical_video_c
+00018350: 6f6e 6361 7465 6e61 746f 722e 706e 670a  oncatenator.png.
+00018360: 2020 2020 2020 203a 7769 6474 683a 2033         :width: 3
+00018370: 3030 0a20 2020 2020 2020 3a61 6c69 676e  00.       :align
+00018380: 3a20 6365 6e74 6572 0a0a 2020 2020 3a70  : center..    :p
+00018390: 6172 616d 204c 6973 745b 556e 696f 6e5b  aram List[Union[
+000183a0: 7374 722c 206f 732e 5061 7468 4c69 6b65  str, os.PathLike
+000183b0: 5d5d 2076 6964 656f 5f70 6174 6873 3a20  ]] video_paths: 
+000183c0: 4c69 7374 206f 6620 696e 7075 7420 7669  List of input vi
+000183d0: 6465 6f20 6669 6c65 2070 6174 6873 2e0a  deo file paths..
+000183e0: 2020 2020 3a70 6172 616d 2055 6e69 6f6e      :param Union
+000183f0: 5b73 7472 2c20 6f73 2e50 6174 684c 696b  [str, os.PathLik
+00018400: 655d 2073 6176 655f 7061 7468 3a20 4669  e] save_path: Fi
+00018410: 6c65 2070 6174 6820 746f 2073 6176 6520  le path to save 
+00018420: 7468 6520 636f 6e63 6174 656e 6174 6564  the concatenated
+00018430: 2076 6964 656f 2e0a 2020 2020 3a70 6172   video..    :par
+00018440: 616d 204f 7074 696f 6e61 6c5b 696e 745d  am Optional[int]
+00018450: 2077 6964 7468 5f70 783a 2057 6964 7468   width_px: Width
+00018460: 206f 6620 7468 6520 6f75 7470 7574 2076   of the output v
+00018470: 6964 656f 2069 6e20 7069 7865 6c73 2e0a  ideo in pixels..
+00018480: 2020 2020 3a70 6172 616d 204f 7074 696f      :param Optio
+00018490: 6e61 6c5b 696e 745d 2077 6964 7468 5f69  nal[int] width_i
+000184a0: 6478 3a20 496e 6465 7820 6f66 2074 6865  dx: Index of the
+000184b0: 2076 6964 656f 2074 6f20 7573 6520 666f   video to use fo
+000184c0: 7220 6465 7465 726d 696e 696e 6720 7769  r determining wi
+000184d0: 6474 682e 0a20 2020 203a 7061 7261 6d20  dth..    :param 
+000184e0: 4f70 7469 6f6e 616c 5b62 6f6f 6c5d 2067  Optional[bool] g
+000184f0: 7075 3a20 5768 6574 6865 7220 746f 2075  pu: Whether to u
+00018500: 7365 2047 5055 2d61 6363 656c 6572 6174  se GPU-accelerat
+00018510: 6564 2063 6f64 6563 2028 6465 6661 756c  ed codec (defaul
+00018520: 743a 2046 616c 7365 292e 0a20 2020 203a  t: False)..    :
+00018530: 7061 7261 6d20 4f70 7469 6f6e 616c 5b62  param Optional[b
+00018540: 6f6f 6c5d 2076 6572 626f 7365 3a57 6865  ool] verbose:Whe
+00018550: 7468 6572 2074 6f20 7072 696e 7420 7072  ther to print pr
+00018560: 6f67 7265 7373 206d 6573 7361 6765 7320  ogress messages 
+00018570: 2864 6566 6175 6c74 3a20 5472 7565 292e  (default: True).
+00018580: 0a20 2020 203a 7261 6973 6573 2046 464d  .    :raises FFM
+00018590: 5045 4743 6f64 6563 4750 5545 7272 6f72  PEGCodecGPUError
+000185a0: 3a20 4966 2047 5055 2069 7320 7265 7175  : If GPU is requ
+000185b0: 6573 7465 6420 6275 7420 6e6f 7420 6176  ested but not av
+000185c0: 6169 6c61 626c 652e 0a20 2020 203a 7261  ailable..    :ra
+000185d0: 6973 6573 2049 6e76 616c 6964 496e 7075  ises InvalidInpu
+000185e0: 7445 7272 6f72 3a20 4966 2062 6f74 6820  tError: If both 
+000185f0: 6f72 206e 6569 7468 6572 2077 6964 7468  or neither width
+00018600: 5f70 7820 616e 6420 7769 6474 685f 6964  _px and width_id
+00018610: 7820 6172 6520 7072 6f76 6964 6564 2e0a  x are provided..
+00018620: 0a20 2020 203a 6578 616d 706c 653a 0a20  .    :example:. 
+00018630: 2020 203e 3e3e 2076 6964 656f 5f70 6174     >>> video_pat
+00018640: 6873 203d 205b 272f 5573 6572 732f 7369  hs = ['/Users/si
+00018650: 6d6f 6e2f 4465 736b 746f 702f 656e 7673  mon/Desktop/envs
+00018660: 2f73 696d 6261 2f74 726f 7562 6c65 7368  /simba/troublesh
+00018670: 6f6f 7469 6e67 2f52 4154 5f4e 4f52 2f70  ooting/RAT_NOR/p
+00018680: 726f 6a65 6374 5f66 6f6c 6465 722f 7669  roject_folder/vi
+00018690: 6465 6f73 2f74 6573 742f 3038 3130 3230  deos/test/081020
+000186a0: 3231 5f44 4f54 5f52 6174 375f 3828 3229  21_DOT_Rat7_8(2)
+000186b0: 2e6d 7034 272c 0a20 2020 203e 3e3e 2020  .mp4',.    >>>  
+000186c0: 2020 2020 2020 2020 2020 2020 2020 272f                '/
+000186d0: 5573 6572 732f 7369 6d6f 6e2f 4465 736b  Users/simon/Desk
+000186e0: 746f 702f 656e 7673 2f73 696d 6261 2f74  top/envs/simba/t
+000186f0: 726f 7562 6c65 7368 6f6f 7469 6e67 2f52  roubleshooting/R
+00018700: 4154 5f4e 4f52 2f70 726f 6a65 6374 5f66  AT_NOR/project_f
+00018710: 6f6c 6465 722f 7669 6465 6f73 2f74 6573  older/videos/tes
+00018720: 742f 3038 3130 3230 3231 5f44 4f54 5f52  t/08102021_DOT_R
+00018730: 6174 3131 5f31 322e 6d70 3427 2c0a 2020  at11_12.mp4',.  
+00018740: 2020 3e3e 3e20 2020 2020 2020 2020 2020    >>>           
+00018750: 2020 2020 2027 2f55 7365 7273 2f73 696d       '/Users/sim
+00018760: 6f6e 2f44 6573 6b74 6f70 2f65 6e76 732f  on/Desktop/envs/
+00018770: 7369 6d62 612f 7472 6f75 626c 6573 686f  simba/troublesho
+00018780: 6f74 696e 672f 5241 545f 4e4f 522f 7072  oting/RAT_NOR/pr
+00018790: 6f6a 6563 745f 666f 6c64 6572 2f76 6964  oject_folder/vid
+000187a0: 656f 732f 7465 7374 2f30 3831 3032 3032  eos/test/0810202
+000187b0: 315f 444f 545f 5261 7431 315f 3132 5f31  1_DOT_Rat11_12_1
+000187c0: 2e6d 7034 275d 0a20 2020 203e 3e3e 205f  .mp4'].    >>> _
+000187d0: 203d 2076 6572 7469 6361 6c5f 7669 6465   = vertical_vide
+000187e0: 6f5f 636f 6e63 6174 656e 6174 6f72 2876  o_concatenator(v
+000187f0: 6964 656f 5f70 6174 6873 3d76 6964 656f  ideo_paths=video
+00018800: 5f70 6174 6873 2c20 7769 6474 685f 6964  _paths, width_id
+00018810: 783d 312c 2073 6176 655f 7061 7468 3d27  x=1, save_path='
+00018820: 2f55 7365 7273 2f73 696d 6f6e 2f44 6573  /Users/simon/Des
+00018830: 6b74 6f70 2f65 6e76 732f 7369 6d62 612f  ktop/envs/simba/
+00018840: 7472 6f75 626c 6573 686f 6f74 696e 672f  troubleshooting/
+00018850: 5241 545f 4e4f 522f 7072 6f6a 6563 745f  RAT_NOR/project_
+00018860: 666f 6c64 6572 2f76 6964 656f 732f 7465  folder/videos/te
+00018870: 7374 2f6e 6577 2f30 3831 3032 3032 315f  st/new/08102021_
+00018880: 444f 545f 5261 7437 5f38 2832 295f 2e6d  DOT_Rat7_8(2)_.m
+00018890: 7034 272c 2067 7075 3d46 616c 7365 290a  p4', gpu=False).
+000188a0: 2020 2020 2222 220a 0a20 2020 2063 6865      """..    che
+000188b0: 636b 5f66 666d 7065 675f 6176 6169 6c61  ck_ffmpeg_availa
+000188c0: 626c 6528 290a 2020 2020 6966 2067 7075  ble().    if gpu
+000188d0: 2061 6e64 206e 6f74 2063 6865 636b 5f6e   and not check_n
+000188e0: 7669 6465 615f 6770 755f 6176 6169 6c61  videa_gpu_availa
+000188f0: 626c 6528 293a 0a20 2020 2020 2020 2072  ble():.        r
+00018900: 6169 7365 2046 464d 5045 4743 6f64 6563  aise FFMPEGCodec
+00018910: 4750 5545 7272 6f72 280a 2020 2020 2020  GPUError(.      
+00018920: 2020 2020 2020 6d73 673d 224e 5649 4449        msg="NVIDI
+00018930: 4120 4750 5520 6e6f 7420 6176 6169 6c61  A GPU not availa
+00018940: 626c 6522 2c20 736f 7572 6365 3d76 6572  ble", source=ver
+00018950: 7469 6361 6c5f 7669 6465 6f5f 636f 6e63  tical_video_conc
+00018960: 6174 656e 6174 6f72 2e5f 5f6e 616d 655f  atenator.__name_
+00018970: 5f0a 2020 2020 2020 2020 290a 2020 2020  _.        ).    
+00018980: 7669 6465 6f5f 6d65 7461 5f64 6174 6120  video_meta_data 
+00018990: 3d20 5b0a 2020 2020 2020 2020 6765 745f  = [.        get_
+000189a0: 7669 6465 6f5f 6d65 7461 5f64 6174 6128  video_meta_data(
+000189b0: 7669 6465 6f5f 7061 7468 3d76 6964 656f  video_path=video
+000189c0: 5f70 6174 6829 2066 6f72 2076 6964 656f  _path) for video
+000189d0: 5f70 6174 6820 696e 2076 6964 656f 5f70  _path in video_p
+000189e0: 6174 6873 0a20 2020 205d 0a20 2020 2074  aths.    ].    t
+000189f0: 696d 6572 203d 2053 696d 6261 5469 6d65  imer = SimbaTime
+00018a00: 7228 7374 6172 743d 5472 7565 290a 2020  r(start=True).  
+00018a10: 2020 6368 6563 6b5f 7661 6c69 645f 6c73    check_valid_ls
+00018a20: 7428 0a20 2020 2020 2020 2064 6174 613d  t(.        data=
+00018a30: 7669 6465 6f5f 7061 7468 732c 2073 6f75  video_paths, sou
+00018a40: 7263 653d 7665 7274 6963 616c 5f76 6964  rce=vertical_vid
+00018a50: 656f 5f63 6f6e 6361 7465 6e61 746f 722e  eo_concatenator.
+00018a60: 5f5f 6e61 6d65 5f5f 2c20 6d69 6e5f 6c65  __name__, min_le
+00018a70: 6e3d 320a 2020 2020 290a 2020 2020 6368  n=2.    ).    ch
+00018a80: 6563 6b5f 6966 5f64 6972 5f65 7869 7374  eck_if_dir_exist
+00018a90: 7328 0a20 2020 2020 2020 2069 6e5f 6469  s(.        in_di
+00018aa0: 723d 6f73 2e70 6174 682e 6469 726e 616d  r=os.path.dirnam
+00018ab0: 6528 7361 7665 5f70 6174 6829 2c20 736f  e(save_path), so
+00018ac0: 7572 6365 3d76 6572 7469 6361 6c5f 7669  urce=vertical_vi
+00018ad0: 6465 6f5f 636f 6e63 6174 656e 6174 6f72  deo_concatenator
+00018ae0: 2e5f 5f6e 616d 655f 5f0a 2020 2020 290a  .__name__.    ).
+00018af0: 2020 2020 6966 2028 2877 6964 7468 5f70      if ((width_p
+00018b00: 7820 6973 204e 6f6e 6529 2061 6e64 2028  x is None) and (
+00018b10: 7769 6474 685f 6964 7820 6973 204e 6f6e  width_idx is Non
+00018b20: 6529 2920 6f72 2028 0a20 2020 2020 2020  e)) or (.       
+00018b30: 2028 7769 6474 685f 7078 2069 7320 6e6f   (width_px is no
+00018b40: 7420 4e6f 6e65 2920 616e 6420 2877 6964  t None) and (wid
+00018b50: 7468 5f69 6478 2069 7320 6e6f 7420 4e6f  th_idx is not No
+00018b60: 6e65 290a 2020 2020 293a 0a20 2020 2020  ne).    ):.     
+00018b70: 2020 2072 6169 7365 2049 6e76 616c 6964     raise Invalid
+00018b80: 496e 7075 7445 7272 6f72 280a 2020 2020  InputError(.    
+00018b90: 2020 2020 2020 2020 6d73 673d 2250 726f          msg="Pro
+00018ba0: 7669 6465 2061 2077 6964 7468 5f70 7820  vide a width_px 
+00018bb0: 4f52 2077 6964 7468 5f69 6478 222c 0a20  OR width_idx",. 
+00018bc0: 2020 2020 2020 2020 2020 2073 6f75 7263             sourc
+00018bd0: 653d 7665 7274 6963 616c 5f76 6964 656f  e=vertical_video
+00018be0: 5f63 6f6e 6361 7465 6e61 746f 722e 5f5f  _concatenator.__
+00018bf0: 6e61 6d65 5f5f 2c0a 2020 2020 2020 2020  name__,.        
+00018c00: 290a 2020 2020 6966 2077 6964 7468 5f69  ).    if width_i
+00018c10: 6478 2069 7320 6e6f 7420 4e6f 6e65 3a0a  dx is not None:.
+00018c20: 2020 2020 2020 2020 6368 6563 6b5f 696e          check_in
+00018c30: 7428 0a20 2020 2020 2020 2020 2020 206e  t(.            n
+00018c40: 616d 653d 6622 7b76 6572 7469 6361 6c5f  ame=f"{vertical_
+00018c50: 7669 6465 6f5f 636f 6e63 6174 656e 6174  video_concatenat
+00018c60: 6f72 2e5f 5f6e 616d 655f 5f7d 2077 6964  or.__name__} wid
+00018c70: 7468 2069 6e64 6578 222c 0a20 2020 2020  th index",.     
+00018c80: 2020 2020 2020 2076 616c 7565 3d77 6964         value=wid
+00018c90: 7468 5f69 6478 2c0a 2020 2020 2020 2020  th_idx,.        
+00018ca0: 2020 2020 6d69 6e5f 7661 6c75 653d 302c      min_value=0,
+00018cb0: 0a20 2020 2020 2020 2020 2020 206d 6178  .            max
+00018cc0: 5f76 616c 7565 3d6c 656e 2876 6964 656f  _value=len(video
+00018cd0: 5f70 6174 6873 2920 2d20 312c 0a20 2020  _paths) - 1,.   
+00018ce0: 2020 2020 2029 0a20 2020 2020 2020 2077       ).        w
+00018cf0: 6964 7468 203d 2069 6e74 2876 6964 656f  idth = int(video
+00018d00: 5f6d 6574 615f 6461 7461 5b77 6964 7468  _meta_data[width
+00018d10: 5f69 6478 5d5b 2277 6964 7468 225d 290a  _idx]["width"]).
+00018d20: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00018d30: 2020 6368 6563 6b5f 696e 7428 0a20 2020    check_int(.   
+00018d40: 2020 2020 2020 2020 206e 616d 653d 6622           name=f"
+00018d50: 7b76 6572 7469 6361 6c5f 7669 6465 6f5f  {vertical_video_
+00018d60: 636f 6e63 6174 656e 6174 6f72 2e5f 5f6e  concatenator.__n
+00018d70: 616d 655f 5f7d 2077 6964 7468 222c 0a20  ame__} width",. 
+00018d80: 2020 2020 2020 2020 2020 2076 616c 7565             value
+00018d90: 3d77 6964 7468 5f70 782c 0a20 2020 2020  =width_px,.     
+00018da0: 2020 2020 2020 206d 696e 5f76 616c 7565         min_value
+00018db0: 3d31 2c0a 2020 2020 2020 2020 290a 2020  =1,.        ).  
+00018dc0: 2020 2020 2020 7769 6474 6820 3d20 696e        width = in
+00018dd0: 7428 7769 6474 685f 7078 290a 2020 2020  t(width_px).    
+00018de0: 7669 6465 6f5f 7061 7468 5f73 7472 203d  video_path_str =
+00018df0: 2022 2022 2e6a 6f69 6e28 5b66 272d 6920   " ".join([f'-i 
+00018e00: 227b 7061 7468 7d22 2720 666f 7220 7061  "{path}"' for pa
+00018e10: 7468 2069 6e20 7669 6465 6f5f 7061 7468  th in video_path
+00018e20: 735d 290a 2020 2020 636f 6465 6320 3d20  s]).    codec = 
+00018e30: 2268 3236 345f 6e76 656e 6322 2069 6620  "h264_nvenc" if 
+00018e40: 6770 7520 656c 7365 2022 6c69 6276 7078  gpu else "libvpx
+00018e50: 2d76 7039 220a 2020 2020 6669 6c74 6572  -vp9".    filter
+00018e60: 5f63 6f6d 706c 6578 203d 2022 3b22 2e6a  _complex = ";".j
+00018e70: 6f69 6e28 0a20 2020 2020 2020 205b 6622  oin(.        [f"
+00018e80: 5b7b 6964 787d 3a76 5d73 6361 6c65 3d7b  [{idx}:v]scale={
+00018e90: 7769 6474 687d 3a2d 315b 767b 6964 787d  width}:-1[v{idx}
+00018ea0: 5d22 2066 6f72 2069 6478 2069 6e20 7261  ]" for idx in ra
+00018eb0: 6e67 6528 6c65 6e28 7669 6465 6f5f 7061  nge(len(video_pa
+00018ec0: 7468 7329 295d 0a20 2020 2029 0a20 2020  ths))].    ).   
+00018ed0: 2066 696c 7465 725f 636f 6d70 6c65 7820   filter_complex 
+00018ee0: 2b3d 2066 223b 7b27 272e 6a6f 696e 285b  += f";{''.join([
+00018ef0: 6627 5b76 7b69 6478 7d5d 2720 666f 7220  f'[v{idx}]' for 
+00018f00: 6964 7820 696e 2072 616e 6765 286c 656e  idx in range(len
+00018f10: 2876 6964 656f 5f70 6174 6873 2929 5d29  (video_paths))])
+00018f20: 7d22 0a20 2020 2066 696c 7465 725f 636f  }".    filter_co
+00018f30: 6d70 6c65 7820 2b3d 2066 2276 7374 6163  mplex += f"vstac
+00018f40: 6b3d 696e 7075 7473 3d7b 6c65 6e28 7669  k=inputs={len(vi
+00018f50: 6465 6f5f 7061 7468 7329 7d5b 765d 220a  deo_paths)}[v]".
+00018f60: 2020 2020 6966 2076 6572 626f 7365 3a0a      if verbose:.
+00018f70: 2020 2020 2020 2020 7072 696e 7428 0a20          print(. 
+00018f80: 2020 2020 2020 2020 2020 2066 2243 6f6e             f"Con
+00018f90: 6361 7465 6e61 7469 6e67 207b 6c65 6e28  catenating {len(
+00018fa0: 7669 6465 6f5f 7061 7468 7329 7d20 7669  video_paths)} vi
+00018fb0: 6465 6f73 2076 6572 7469 6361 6c6c 7920  deos vertically 
+00018fc0: 7769 7468 2061 207b 7769 6474 687d 2070  with a {width} p
+00018fd0: 6978 656c 2077 6964 7468 2e2e 2e22 0a20  ixel width...". 
+00018fe0: 2020 2020 2020 2029 0a20 2020 2063 6d64         ).    cmd
+00018ff0: 203d 2066 2766 666d 7065 6720 7b76 6964   = f'ffmpeg {vid
+00019000: 656f 5f70 6174 685f 7374 727d 202d 6669  eo_path_str} -fi
+00019010: 6c74 6572 5f63 6f6d 706c 6578 2022 7b66  lter_complex "{f
+00019020: 696c 7465 725f 636f 6d70 6c65 787d 2220  ilter_complex}" 
+00019030: 2d6d 6170 2022 5b76 5d22 202d 633a 7620  -map "[v]" -c:v 
+00019040: 7b63 6f64 6563 7d20 2d6c 6f67 6c65 7665  {codec} -logleve
+00019050: 6c20 6572 726f 7220 2d73 7461 7473 2022  l error -stats "
+00019060: 7b73 6176 655f 7061 7468 7d22 202d 7927  {save_path}" -y'
+00019070: 0a20 2020 2073 7562 7072 6f63 6573 732e  .    subprocess.
+00019080: 6361 6c6c 2863 6d64 2c20 7368 656c 6c3d  call(cmd, shell=
+00019090: 5472 7565 2c20 7374 646f 7574 3d73 7562  True, stdout=sub
+000190a0: 7072 6f63 6573 732e 5049 5045 290a 2020  process.PIPE).  
+000190b0: 2020 7469 6d65 722e 7374 6f70 5f74 696d    timer.stop_tim
+000190c0: 6572 2829 0a20 2020 2069 6620 7665 7262  er().    if verb
+000190d0: 6f73 653a 0a20 2020 2020 2020 2070 7269  ose:.        pri
+000190e0: 6e74 280a 2020 2020 2020 2020 2020 2020  nt(.            
+000190f0: 6622 5665 7274 6963 616c 2063 6f6e 6361  f"Vertical conca
+00019100: 7465 6e61 7469 6f6e 2063 6f6d 706c 6574  tenation complet
+00019110: 652e 2053 6176 6564 2061 7420 7b73 6176  e. Saved at {sav
+00019120: 655f 7061 7468 7d20 2845 6c61 7073 6564  e_path} (Elapsed
+00019130: 2074 696d 653a 207b 7469 6d65 722e 656c   time: {timer.el
+00019140: 6170 7365 645f 7469 6d65 5f73 7472 7d73  apsed_time_str}s
+00019150: 2e29 220a 2020 2020 2020 2020 290a 0a0a  .)".        )...
+00019160: 6465 6620 6d6f 7361 6963 5f63 6f6e 6361  def mosaic_conca
+00019170: 7465 6e61 746f 7228 0a20 2020 2076 6964  tenator(.    vid
+00019180: 656f 5f70 6174 6873 3a20 4c69 7374 5b55  eo_paths: List[U
+00019190: 6e69 6f6e 5b73 7472 2c20 6f73 2e50 6174  nion[str, os.Pat
+000191a0: 684c 696b 655d 5d2c 0a20 2020 2073 6176  hLike]],.    sav
+000191b0: 655f 7061 7468 3a20 556e 696f 6e5b 7374  e_path: Union[st
+000191c0: 722c 206f 732e 5061 7468 4c69 6b65 5d2c  r, os.PathLike],
+000191d0: 0a20 2020 2077 6964 7468 5f69 6478 3a20  .    width_idx: 
+000191e0: 4f70 7469 6f6e 616c 5b55 6e69 6f6e 5b69  Optional[Union[i
+000191f0: 6e74 2c20 7374 725d 5d20 3d20 4e6f 6e65  nt, str]] = None
+00019200: 2c0a 2020 2020 7769 6474 685f 7078 3a20  ,.    width_px: 
+00019210: 4f70 7469 6f6e 616c 5b55 6e69 6f6e 5b69  Optional[Union[i
+00019220: 6e74 2c20 7374 725d 5d20 3d20 4e6f 6e65  nt, str]] = None
+00019230: 2c0a 2020 2020 6865 6967 6874 5f69 6478  ,.    height_idx
+00019240: 3a20 4f70 7469 6f6e 616c 5b55 6e69 6f6e  : Optional[Union
+00019250: 5b69 6e74 2c20 7374 725d 5d20 3d20 4e6f  [int, str]] = No
+00019260: 6e65 2c0a 2020 2020 6865 6967 6874 5f70  ne,.    height_p
+00019270: 783a 204f 7074 696f 6e61 6c5b 556e 696f  x: Optional[Unio
+00019280: 6e5b 696e 742c 2073 7472 5d5d 203d 204e  n[int, str]] = N
+00019290: 6f6e 652c 0a20 2020 2067 7075 3a20 4f70  one,.    gpu: Op
+000192a0: 7469 6f6e 616c 5b62 6f6f 6c5d 203d 2046  tional[bool] = F
+000192b0: 616c 7365 2c0a 2020 2020 7665 7262 6f73  alse,.    verbos
+000192c0: 653a 204f 7074 696f 6e61 6c5b 626f 6f6c  e: Optional[bool
+000192d0: 5d20 3d20 5472 7565 2c0a 2020 2020 756e  ] = True,.    un
+000192e0: 6576 656e 5f66 696c 6c5f 636f 6c6f 723a  even_fill_color:
+000192f0: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+00019300: 2022 626c 6163 6b22 2c0a 2920 2d3e 204e   "black",.) -> N
+00019310: 6f6e 653a 0a20 2020 2022 2222 0a20 2020  one:.    """.   
+00019320: 2043 6f6e 6361 7465 6e61 7465 7320 6d75   Concatenates mu
+00019330: 6c74 6970 6c65 2076 6964 656f 7320 696e  ltiple videos in
+00019340: 746f 2061 206d 6f73 6169 6320 6c61 796f  to a mosaic layo
+00019350: 7574 2e0a 0a20 2020 202e 2e20 696d 6167  ut...    .. imag
+00019360: 653a 3a20 5f73 7461 7469 632f 696d 672f  e:: _static/img/
+00019370: 6d6f 7361 6963 5f63 6f6e 6361 7465 6e61  mosaic_concatena
+00019380: 746f 722e 706e 670a 2020 2020 2020 203a  tor.png.       :
+00019390: 7769 6474 683a 2036 3030 0a20 2020 2020  width: 600.     
+000193a0: 2020 3a61 6c69 676e 3a20 6365 6e74 6572    :align: center
+000193b0: 0a0a 2020 2020 2e2e 206e 6f74 653a 3a0a  ..    .. note::.
+000193c0: 2020 2020 2020 2069 6620 616e 2075 6e65         if an une
+000193d0: 7665 6e20 6e75 6d62 6572 206f 6620 7669  ven number of vi
+000193e0: 6465 6f73 2c20 7468 6520 6c61 7374 2069  deos, the last i
+000193f0: 6e64 6578 2077 696c 6c20 6265 2066 696c  ndex will be fil
+00019400: 6c65 6420 6279 2060 6075 6e65 7665 6e5f  led by ``uneven_
+00019410: 6669 6c6c 5f63 6f6c 6f72 6060 2e0a 0a20  fill_color``... 
+00019420: 2020 203a 7061 7261 6d20 4c69 7374 5b55     :param List[U
+00019430: 6e69 6f6e 5b73 7472 2c20 6f73 2e50 6174  nion[str, os.Pat
+00019440: 684c 696b 655d 5d20 7669 6465 6f5f 7061  hLike]] video_pa
+00019450: 7468 733a 204c 6973 7420 6f66 2069 6e70  ths: List of inp
+00019460: 7574 2076 6964 656f 2066 696c 6520 7061  ut video file pa
+00019470: 7468 732e 0a20 2020 203a 7061 7261 6d20  ths..    :param 
+00019480: 556e 696f 6e5b 7374 722c 206f 732e 5061  Union[str, os.Pa
+00019490: 7468 4c69 6b65 5d20 7361 7665 5f70 6174  thLike] save_pat
+000194a0: 683a 2046 696c 6520 7061 7468 2074 6f20  h: File path to 
+000194b0: 7361 7665 2074 6865 2063 6f6e 6361 7465  save the concate
+000194c0: 6e61 7465 6420 7669 6465 6f2e 0a20 2020  nated video..   
+000194d0: 203a 7061 7261 6d20 4f70 7469 6f6e 616c   :param Optional
+000194e0: 5b69 6e74 5d20 7769 6474 685f 7078 3a20  [int] width_px: 
+000194f0: 5769 6474 6820 6f66 2074 6865 206f 7574  Width of the out
+00019500: 7075 7420 7669 6465 6f20 696e 2070 6978  put video in pix
+00019510: 656c 732e 0a20 2020 203a 7061 7261 6d20  els..    :param 
+00019520: 4f70 7469 6f6e 616c 5b69 6e74 5d20 7769  Optional[int] wi
+00019530: 6474 685f 6964 783a 2049 6e64 6578 206f  dth_idx: Index o
+00019540: 6620 7468 6520 7669 6465 6f20 746f 2075  f the video to u
+00019550: 7365 2066 6f72 2064 6574 6572 6d69 6e69  se for determini
+00019560: 6e67 2077 6964 7468 2e0a 2020 2020 3a70  ng width..    :p
+00019570: 6172 616d 204f 7074 696f 6e61 6c5b 696e  aram Optional[in
+00019580: 745d 2068 6569 6768 745f 7078 3a20 4865  t] height_px: He
+00019590: 6967 6874 206f 6620 7468 6520 6f75 7470  ight of the outp
+000195a0: 7574 2076 6964 656f 2070 616e 656c 7320  ut video panels 
+000195b0: 696e 2070 6978 656c 732e 0a20 2020 203a  in pixels..    :
+000195c0: 7061 7261 6d20 4f70 7469 6f6e 616c 5b69  param Optional[i
+000195d0: 6e74 5d20 6865 6967 6874 5f69 6478 3a20  nt] height_idx: 
+000195e0: 4865 6967 6874 206f 6620 7468 6520 7669  Height of the vi
+000195f0: 6465 6f20 746f 2075 7365 2066 6f72 2064  deo to use for d
+00019600: 6574 6572 6d69 6e69 6e67 2077 6964 7468  etermining width
+00019610: 2e0a 2020 2020 3a70 6172 616d 204f 7074  ..    :param Opt
+00019620: 696f 6e61 6c5b 626f 6f6c 5d20 6770 753a  ional[bool] gpu:
+00019630: 2057 6865 7468 6572 2074 6f20 7573 6520   Whether to use 
+00019640: 4750 552d 6163 6365 6c65 7261 7465 6420  GPU-accelerated 
+00019650: 636f 6465 6320 2864 6566 6175 6c74 3a20  codec (default: 
+00019660: 4661 6c73 6529 2e0a 2020 2020 3a70 6172  False)..    :par
+00019670: 616d 204f 7074 696f 6e61 6c5b 626f 6f6c  am Optional[bool
+00019680: 5d20 7665 7262 6f73 653a 2057 6865 7468  ] verbose: Wheth
+00019690: 6572 2074 6f20 7072 696e 7420 7072 6f67  er to print prog
+000196a0: 7265 7373 206d 6573 7361 6765 7320 2864  ress messages (d
+000196b0: 6566 6175 6c74 3a20 5472 7565 292e 0a0a  efault: True)...
+000196c0: 2020 2020 3a65 7861 6d70 6c65 3a0a 2020      :example:.  
+000196d0: 2020 3e3e 3e20 7669 6465 6f5f 7061 7468    >>> video_path
+000196e0: 7320 3d20 5b27 2f55 7365 7273 2f73 696d  s = ['/Users/sim
+000196f0: 6f6e 2f44 6573 6b74 6f70 2f65 6e76 732f  on/Desktop/envs/
+00019700: 7369 6d62 612f 7472 6f75 626c 6573 686f  simba/troublesho
+00019710: 6f74 696e 672f 5241 545f 4e4f 522f 7072  oting/RAT_NOR/pr
+00019720: 6f6a 6563 745f 666f 6c64 6572 2f76 6964  oject_folder/vid
+00019730: 656f 732f 7465 7374 2f30 3831 3032 3032  eos/test/0810202
+00019740: 315f 444f 545f 5261 7437 5f38 2832 292e  1_DOT_Rat7_8(2).
+00019750: 6d70 3427 2c20 272f 5573 6572 732f 7369  mp4', '/Users/si
+00019760: 6d6f 6e2f 4465 736b 746f 702f 656e 7673  mon/Desktop/envs
+00019770: 2f73 696d 6261 2f74 726f 7562 6c65 7368  /simba/troublesh
+00019780: 6f6f 7469 6e67 2f52 4154 5f4e 4f52 2f70  ooting/RAT_NOR/p
+00019790: 726f 6a65 6374 5f66 6f6c 6465 722f 7669  roject_folder/vi
+000197a0: 6465 6f73 2f74 6573 742f 3038 3130 3230  deos/test/081020
+000197b0: 3231 5f44 4f54 5f52 6174 3131 5f31 322e  21_DOT_Rat11_12.
+000197c0: 6d70 3427 2c20 272f 5573 6572 732f 7369  mp4', '/Users/si
+000197d0: 6d6f 6e2f 4465 736b 746f 702f 656e 7673  mon/Desktop/envs
+000197e0: 2f73 696d 6261 2f74 726f 7562 6c65 7368  /simba/troublesh
+000197f0: 6f6f 7469 6e67 2f52 4154 5f4e 4f52 2f70  ooting/RAT_NOR/p
+00019800: 726f 6a65 6374 5f66 6f6c 6465 722f 7669  roject_folder/vi
+00019810: 6465 6f73 2f74 6573 742f 6e65 772f 3230  deos/test/new/20
+00019820: 3232 2d30 362d 3231 5f4e 4f42 5f49 4f54  22-06-21_NOB_IOT
+00019830: 5f32 332e 6d70 3427 5d0a 2020 2020 3e3e  _23.mp4'].    >>
+00019840: 3e20 7361 7665 5f70 6174 6820 3d20 272f  > save_path = '/
+00019850: 5573 6572 732f 7369 6d6f 6e2f 4465 736b  Users/simon/Desk
+00019860: 746f 702f 656e 7673 2f73 696d 6261 2f74  top/envs/simba/t
+00019870: 726f 7562 6c65 7368 6f6f 7469 6e67 2f52  roubleshooting/R
+00019880: 4154 5f4e 4f52 2f70 726f 6a65 6374 5f66  AT_NOR/project_f
+00019890: 6f6c 6465 722f 7669 6465 6f73 2f74 6573  older/videos/tes
+000198a0: 742f 6e65 772f 626c 616e 6b5f 7465 7374  t/new/blank_test
+000198b0: 2e6d 7034 270a 2020 2020 3e3e 3e20 6d6f  .mp4'.    >>> mo
+000198c0: 7361 6963 5f63 6f6e 6361 7465 6e61 746f  saic_concatenato
+000198d0: 7228 7669 6465 6f5f 7061 7468 733d 7669  r(video_paths=vi
+000198e0: 6465 6f5f 7061 7468 732c 2073 6176 655f  deo_paths, save_
+000198f0: 7061 7468 3d73 6176 655f 7061 7468 2c20  path=save_path, 
+00019900: 7769 6474 685f 6964 783d 312c 2068 6569  width_idx=1, hei
+00019910: 6768 745f 6964 783d 312c 2067 7075 3d46  ght_idx=1, gpu=F
+00019920: 616c 7365 290a 2020 2020 2222 220a 0a20  alse).    """.. 
+00019930: 2020 2063 6865 636b 5f66 666d 7065 675f     check_ffmpeg_
+00019940: 6176 6169 6c61 626c 6528 290a 2020 2020  available().    
+00019950: 6966 2067 7075 2061 6e64 206e 6f74 2063  if gpu and not c
+00019960: 6865 636b 5f6e 7669 6465 615f 6770 755f  heck_nvidea_gpu_
+00019970: 6176 6169 6c61 626c 6528 293a 0a20 2020  available():.   
+00019980: 2020 2020 2072 6169 7365 2046 464d 5045       raise FFMPE
+00019990: 4743 6f64 6563 4750 5545 7272 6f72 280a  GCodecGPUError(.
+000199a0: 2020 2020 2020 2020 2020 2020 6d73 673d              msg=
+000199b0: 224e 5649 4449 4120 4750 5520 6e6f 7420  "NVIDIA GPU not 
+000199c0: 6176 6169 6c61 626c 6522 2c20 736f 7572  available", sour
+000199d0: 6365 3d6d 6f73 6169 635f 636f 6e63 6174  ce=mosaic_concat
+000199e0: 656e 6174 6f72 2e5f 5f6e 616d 655f 5f0a  enator.__name__.
+000199f0: 2020 2020 2020 2020 290a 2020 2020 7469          ).    ti
+00019a00: 6d65 7220 3d20 5369 6d62 6154 696d 6572  mer = SimbaTimer
+00019a10: 2873 7461 7274 3d54 7275 6529 0a20 2020  (start=True).   
+00019a20: 2064 7420 3d20 6461 7465 7469 6d65 2e6e   dt = datetime.n
+00019a30: 6f77 2829 2e73 7472 6674 696d 6528 2225  ow().strftime("%
+00019a40: 5925 6d25 6425 4825 4d25 5322 290a 2020  Y%m%d%H%M%S").  
+00019a50: 2020 6368 6563 6b5f 7661 6c69 645f 6c73    check_valid_ls
+00019a60: 7428 0a20 2020 2020 2020 2064 6174 613d  t(.        data=
+00019a70: 7669 6465 6f5f 7061 7468 732c 0a20 2020  video_paths,.   
+00019a80: 2020 2020 2073 6f75 7263 653d 6622 7b6d       source=f"{m
+00019a90: 6f73 6169 635f 636f 6e63 6174 656e 6174  osaic_concatenat
+00019aa0: 6f72 2e5f 5f6e 616d 655f 5f7d 2076 6964  or.__name__} vid
+00019ab0: 656f 5f70 6174 6873 222c 0a20 2020 2020  eo_paths",.     
+00019ac0: 2020 206d 696e 5f6c 656e 3d33 2c0a 2020     min_len=3,.  
+00019ad0: 2020 290a 2020 2020 7669 6465 6f5f 6d65    ).    video_me
+00019ae0: 7461 5f64 6174 6120 3d20 5b0a 2020 2020  ta_data = [.    
+00019af0: 2020 2020 6765 745f 7669 6465 6f5f 6d65      get_video_me
+00019b00: 7461 5f64 6174 6128 7669 6465 6f5f 7061  ta_data(video_pa
+00019b10: 7468 3d76 6964 656f 5f70 6174 6829 2066  th=video_path) f
+00019b20: 6f72 2076 6964 656f 5f70 6174 6820 696e  or video_path in
+00019b30: 2076 6964 656f 5f70 6174 6873 0a20 2020   video_paths.   
+00019b40: 205d 0a20 2020 206d 6178 5f76 6964 656f   ].    max_video
+00019b50: 5f6c 656e 6774 6820 3d20 6d61 7828 5b78  _length = max([x
+00019b60: 5b22 7669 6465 6f5f 6c65 6e67 7468 5f73  ["video_length_s
+00019b70: 225d 2066 6f72 2078 2069 6e20 7669 6465  "] for x in vide
+00019b80: 6f5f 6d65 7461 5f64 6174 615d 290a 2020  o_meta_data]).  
+00019b90: 2020 6966 2028 2877 6964 7468 5f70 7820    if ((width_px 
+00019ba0: 6973 204e 6f6e 6529 2061 6e64 2028 7769  is None) and (wi
+00019bb0: 6474 685f 6964 7820 6973 204e 6f6e 6529  dth_idx is None)
+00019bc0: 2920 6f72 2028 0a20 2020 2020 2020 2028  ) or (.        (
+00019bd0: 7769 6474 685f 7078 2069 7320 6e6f 7420  width_px is not 
+00019be0: 4e6f 6e65 2920 616e 6420 2877 6964 7468  None) and (width
+00019bf0: 5f69 6478 2069 7320 6e6f 7420 4e6f 6e65  _idx is not None
+00019c00: 290a 2020 2020 293a 0a20 2020 2020 2020  ).    ):.       
+00019c10: 2072 6169 7365 2049 6e76 616c 6964 496e   raise InvalidIn
+00019c20: 7075 7445 7272 6f72 280a 2020 2020 2020  putError(.      
+00019c30: 2020 2020 2020 6d73 673d 2250 726f 7669        msg="Provi
+00019c40: 6465 2061 2077 6964 7468 5f70 7820 4f52  de a width_px OR
+00019c50: 2077 6964 7468 5f69 6478 222c 2073 6f75   width_idx", sou
+00019c60: 7263 653d 6d6f 7361 6963 5f63 6f6e 6361  rce=mosaic_conca
+00019c70: 7465 6e61 746f 722e 5f5f 6e61 6d65 5f5f  tenator.__name__
+00019c80: 0a20 2020 2020 2020 2029 0a20 2020 2069  .        ).    i
+00019c90: 6620 2828 6865 6967 6874 5f70 7820 6973  f ((height_px is
+00019ca0: 204e 6f6e 6529 2061 6e64 2028 6865 6967   None) and (heig
+00019cb0: 6874 5f69 6478 2069 7320 4e6f 6e65 2929  ht_idx is None))
+00019cc0: 206f 7220 280a 2020 2020 2020 2020 2868   or (.        (h
+00019cd0: 6569 6768 745f 7078 2069 7320 6e6f 7420  eight_px is not 
+00019ce0: 4e6f 6e65 2920 616e 6420 2868 6569 6768  None) and (heigh
+00019cf0: 745f 6964 7820 6973 206e 6f74 204e 6f6e  t_idx is not Non
+00019d00: 6529 0a20 2020 2029 3a0a 2020 2020 2020  e).    ):.      
+00019d10: 2020 7261 6973 6520 496e 7661 6c69 6449    raise InvalidI
+00019d20: 6e70 7574 4572 726f 7228 0a20 2020 2020  nputError(.     
+00019d30: 2020 2020 2020 206d 7367 3d22 5072 6f76         msg="Prov
+00019d40: 6964 6520 6120 6865 6967 6874 5f70 7820  ide a height_px 
+00019d50: 4f52 2068 6569 6768 745f 6964 7822 2c20  OR height_idx", 
+00019d60: 736f 7572 6365 3d6d 6f73 6169 635f 636f  source=mosaic_co
+00019d70: 6e63 6174 656e 6174 6f72 2e5f 5f6e 616d  ncatenator.__nam
+00019d80: 655f 5f0a 2020 2020 2020 2020 290a 2020  e__.        ).  
+00019d90: 2020 6966 2077 6964 7468 5f69 6478 2069    if width_idx i
+00019da0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00019db0: 2020 2020 6368 6563 6b5f 696e 7428 0a20      check_int(. 
+00019dc0: 2020 2020 2020 2020 2020 206e 616d 653d             name=
+00019dd0: 6622 7b76 6572 7469 6361 6c5f 7669 6465  f"{vertical_vide
+00019de0: 6f5f 636f 6e63 6174 656e 6174 6f72 2e5f  o_concatenator._
+00019df0: 5f6e 616d 655f 5f7d 2077 6964 7468 2069  _name__} width i
+00019e00: 6e64 6578 222c 0a20 2020 2020 2020 2020  ndex",.         
+00019e10: 2020 2076 616c 7565 3d77 6964 7468 5f69     value=width_i
+00019e20: 6478 2c0a 2020 2020 2020 2020 2020 2020  dx,.            
+00019e30: 6d69 6e5f 7661 6c75 653d 312c 0a20 2020  min_value=1,.   
+00019e40: 2020 2020 2020 2020 206d 6178 5f76 616c           max_val
+00019e50: 7565 3d6c 656e 2876 6964 656f 5f70 6174  ue=len(video_pat
+00019e60: 6873 2920 2d20 312c 0a20 2020 2020 2020  hs) - 1,.       
+00019e70: 2029 0a20 2020 2020 2020 2077 6964 7468   ).        width
+00019e80: 203d 2069 6e74 2876 6964 656f 5f6d 6574   = int(video_met
+00019e90: 615f 6461 7461 5b77 6964 7468 5f69 6478  a_data[width_idx
+00019ea0: 5d5b 2277 6964 7468 225d 290a 2020 2020  ]["width"]).    
+00019eb0: 656c 7365 3a0a 2020 2020 2020 2020 7769  else:.        wi
+00019ec0: 6474 6820 3d20 7769 6474 685f 7078 0a20  dth = width_px. 
+00019ed0: 2020 2069 6620 6865 6967 6874 5f69 6478     if height_idx
+00019ee0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00019ef0: 2020 2020 2020 6368 6563 6b5f 696e 7428        check_int(
+00019f00: 0a20 2020 2020 2020 2020 2020 206e 616d  .            nam
+00019f10: 653d 6622 7b76 6572 7469 6361 6c5f 7669  e=f"{vertical_vi
+00019f20: 6465 6f5f 636f 6e63 6174 656e 6174 6f72  deo_concatenator
+00019f30: 2e5f 5f6e 616d 655f 5f7d 2068 6569 6768  .__name__} heigh
+00019f40: 7420 696e 6465 7822 2c0a 2020 2020 2020  t index",.      
+00019f50: 2020 2020 2020 7661 6c75 653d 7769 6474        value=widt
+00019f60: 685f 6964 782c 0a20 2020 2020 2020 2020  h_idx,.         
+00019f70: 2020 206d 696e 5f76 616c 7565 3d31 2c0a     min_value=1,.
+00019f80: 2020 2020 2020 2020 2020 2020 6d61 785f              max_
+00019f90: 7661 6c75 653d 6c65 6e28 7669 6465 6f5f  value=len(video_
+00019fa0: 7061 7468 7329 202d 2031 2c0a 2020 2020  paths) - 1,.    
+00019fb0: 2020 2020 290a 2020 2020 2020 2020 6865      ).        he
+00019fc0: 6967 6874 203d 2069 6e74 2876 6964 656f  ight = int(video
+00019fd0: 5f6d 6574 615f 6461 7461 5b77 6964 7468  _meta_data[width
+00019fe0: 5f69 6478 5d5b 2268 6569 6768 7422 5d29  _idx]["height"])
+00019ff0: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+0001a000: 2020 2068 6569 6768 7420 3d20 6865 6967     height = heig
+0001a010: 6874 5f70 780a 2020 2020 6966 2076 6572  ht_px.    if ver
+0001a020: 626f 7365 3a0a 2020 2020 2020 2020 7072  bose:.        pr
+0001a030: 696e 7428 6622 4372 6561 7469 6e67 206d  int(f"Creating m
+0001a040: 6f73 6169 6320 7669 6465 6f20 2e2e 2e22  osaic video ..."
+0001a050: 290a 2020 2020 7465 6d70 5f64 6972 203d  ).    temp_dir =
+0001a060: 206f 732e 7061 7468 2e6a 6f69 6e28 6f73   os.path.join(os
+0001a070: 2e70 6174 682e 6469 726e 616d 6528 7669  .path.dirname(vi
+0001a080: 6465 6f5f 7061 7468 735b 305d 292c 2066  deo_paths[0]), f
+0001a090: 2274 656d 705f 7b64 747d 2229 0a20 2020  "temp_{dt}").   
+0001a0a0: 206f 732e 6d61 6b65 6469 7273 2874 656d   os.makedirs(tem
+0001a0b0: 705f 6469 7229 0a20 2020 2069 6620 6e6f  p_dir).    if no
+0001a0c0: 7420 286c 656e 2876 6964 656f 5f70 6174  t (len(video_pat
+0001a0d0: 6873 2920 2520 3229 203d 3d20 303a 0a20  hs) % 2) == 0:. 
+0001a0e0: 2020 2020 2020 2062 6c61 6e6b 5f70 6174         blank_pat
+0001a0f0: 6820 3d20 6f73 2e70 6174 682e 6a6f 696e  h = os.path.join
+0001a100: 2874 656d 705f 6469 722c 2066 227b 6474  (temp_dir, f"{dt
+0001a110: 7d2e 6d70 3422 290a 2020 2020 2020 2020  }.mp4").        
+0001a120: 6372 6561 7465 5f62 6c61 6e6b 5f76 6964  create_blank_vid
+0001a130: 656f 280a 2020 2020 2020 2020 2020 2020  eo(.            
+0001a140: 7061 7468 3d62 6c61 6e6b 5f70 6174 682c  path=blank_path,
+0001a150: 0a20 2020 2020 2020 2020 2020 206c 656e  .            len
+0001a160: 6774 683d 6d61 785f 7669 6465 6f5f 6c65  gth=max_video_le
+0001a170: 6e67 7468 2c0a 2020 2020 2020 2020 2020  ngth,.          
+0001a180: 2020 7769 6474 683d 7769 6474 682c 0a20    width=width,. 
+0001a190: 2020 2020 2020 2020 2020 2068 6569 6768             heigh
+0001a1a0: 743d 6865 6967 6874 2c0a 2020 2020 2020  t=height,.      
+0001a1b0: 2020 2020 2020 6770 753d 6770 752c 0a20        gpu=gpu,. 
+0001a1c0: 2020 2020 2020 2020 2020 2076 6572 626f             verbo
+0001a1d0: 7365 3d76 6572 626f 7365 2c0a 2020 2020  se=verbose,.    
+0001a1e0: 2020 2020 2020 2020 636f 6c6f 723d 756e          color=un
+0001a1f0: 6576 656e 5f66 696c 6c5f 636f 6c6f 722c  even_fill_color,
+0001a200: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+0001a210: 2020 2076 6964 656f 5f70 6174 6873 2e61     video_paths.a
+0001a220: 7070 656e 6428 626c 616e 6b5f 7061 7468  ppend(blank_path
+0001a230: 290a 2020 2020 7570 7065 725f 7669 6465  ).    upper_vide
+0001a240: 6f73 2c20 6c6f 7765 725f 7669 6465 6f73  os, lower_videos
+0001a250: 203d 2028 0a20 2020 2020 2020 2076 6964   = (.        vid
+0001a260: 656f 5f70 6174 6873 5b3a 206c 656e 2876  eo_paths[: len(v
+0001a270: 6964 656f 5f70 6174 6873 2920 2f2f 2032  ideo_paths) // 2
+0001a280: 5d2c 0a20 2020 2020 2020 2076 6964 656f  ],.        video
+0001a290: 5f70 6174 6873 5b6c 656e 2876 6964 656f  _paths[len(video
+0001a2a0: 5f70 6174 6873 2920 2f2f 2032 203a 5d2c  _paths) // 2 :],
+0001a2b0: 0a20 2020 2029 0a20 2020 2069 6620 7665  .    ).    if ve
+0001a2c0: 7262 6f73 653a 0a20 2020 2020 2020 2070  rbose:.        p
+0001a2d0: 7269 6e74 2822 4372 6561 7469 6e67 2075  rint("Creating u
+0001a2e0: 7070 6572 206d 6f73 6169 632e 2e2e 2028  pper mosaic... (
+0001a2f0: 5374 6570 2031 2f33 2922 290a 2020 2020  Step 1/3)").    
+0001a300: 6966 206c 656e 2875 7070 6572 5f76 6964  if len(upper_vid
+0001a310: 656f 7329 203e 2031 3a0a 2020 2020 2020  eos) > 1:.      
+0001a320: 2020 7570 7065 725f 7061 7468 203d 206f    upper_path = o
+0001a330: 732e 7061 7468 2e6a 6f69 6e28 7465 6d70  s.path.join(temp
+0001a340: 5f64 6972 2c20 2275 7070 6572 2e6d 7034  _dir, "upper.mp4
+0001a350: 2229 0a20 2020 2020 2020 2068 6f72 697a  ").        horiz
+0001a360: 6f6e 7461 6c5f 7669 6465 6f5f 636f 6e63  ontal_video_conc
+0001a370: 6174 656e 6174 6f72 280a 2020 2020 2020  atenator(.      
+0001a380: 2020 2020 2020 7669 6465 6f5f 7061 7468        video_path
+0001a390: 733d 7570 7065 725f 7669 6465 6f73 2c0a  s=upper_videos,.
+0001a3a0: 2020 2020 2020 2020 2020 2020 7361 7665              save
+0001a3b0: 5f70 6174 683d 7570 7065 725f 7061 7468  _path=upper_path
+0001a3c0: 2c0a 2020 2020 2020 2020 2020 2020 6770  ,.            gp
+0001a3d0: 753d 6770 752c 0a20 2020 2020 2020 2020  u=gpu,.         
+0001a3e0: 2020 2068 6569 6768 745f 7078 3d68 6569     height_px=hei
+0001a3f0: 6768 742c 0a20 2020 2020 2020 2020 2020  ght,.           
+0001a400: 2076 6572 626f 7365 3d76 6572 626f 7365   verbose=verbose
+0001a410: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
+0001a420: 656c 7365 3a0a 2020 2020 2020 2020 7570  else:.        up
+0001a430: 7065 725f 7061 7468 203d 2075 7070 6572  per_path = upper
+0001a440: 5f76 6964 656f 735b 305d 0a20 2020 2069  _videos[0].    i
+0001a450: 6620 7665 7262 6f73 653a 0a20 2020 2020  f verbose:.     
+0001a460: 2020 2070 7269 6e74 2822 4372 6561 7469     print("Creati
+0001a470: 6e67 206c 6f77 6572 206d 6f73 6169 632e  ng lower mosaic.
+0001a480: 2e2e 2028 5374 6570 2032 2f33 2922 290a  .. (Step 2/3)").
+0001a490: 2020 2020 6966 206c 656e 286c 6f77 6572      if len(lower
+0001a4a0: 5f76 6964 656f 7329 203e 2031 3a0a 2020  _videos) > 1:.  
+0001a4b0: 2020 2020 2020 6c6f 7765 725f 7061 7468        lower_path
+0001a4c0: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
+0001a4d0: 7465 6d70 5f64 6972 2c20 226c 6f77 6572  temp_dir, "lower
+0001a4e0: 2e6d 7034 2229 0a20 2020 2020 2020 2068  .mp4").        h
+0001a4f0: 6f72 697a 6f6e 7461 6c5f 7669 6465 6f5f  orizontal_video_
+0001a500: 636f 6e63 6174 656e 6174 6f72 280a 2020  concatenator(.  
+0001a510: 2020 2020 2020 2020 2020 7669 6465 6f5f            video_
+0001a520: 7061 7468 733d 6c6f 7765 725f 7669 6465  paths=lower_vide
+0001a530: 6f73 2c0a 2020 2020 2020 2020 2020 2020  os,.            
+0001a540: 7361 7665 5f70 6174 683d 6c6f 7765 725f  save_path=lower_
+0001a550: 7061 7468 2c0a 2020 2020 2020 2020 2020  path,.          
+0001a560: 2020 6770 753d 6770 752c 0a20 2020 2020    gpu=gpu,.     
+0001a570: 2020 2020 2020 2068 6569 6768 745f 7078         height_px
+0001a580: 3d68 6569 6768 742c 0a20 2020 2020 2020  =height,.       
+0001a590: 2020 2020 2076 6572 626f 7365 3d76 6572       verbose=ver
+0001a5a0: 626f 7365 2c0a 2020 2020 2020 2020 290a  bose,.        ).
+0001a5b0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0001a5c0: 2020 6c6f 7765 725f 7061 7468 203d 206c    lower_path = l
+0001a5d0: 6f77 6572 5f76 6964 656f 735b 305d 0a20  ower_videos[0]. 
+0001a5e0: 2020 2070 616e 656c 735f 6d65 7461 203d     panels_meta =
+0001a5f0: 205b 0a20 2020 2020 2020 2067 6574 5f76   [.        get_v
+0001a600: 6964 656f 5f6d 6574 615f 6461 7461 2876  ideo_meta_data(v
+0001a610: 6964 656f 5f70 6174 683d 7669 6465 6f5f  ideo_path=video_
+0001a620: 7061 7468 290a 2020 2020 2020 2020 666f  path).        fo
+0001a630: 7220 7669 6465 6f5f 7061 7468 2069 6e20  r video_path in 
+0001a640: 5b6c 6f77 6572 5f70 6174 682c 2075 7070  [lower_path, upp
+0001a650: 6572 5f70 6174 685d 0a20 2020 205d 0a20  er_path].    ]. 
+0001a660: 2020 2069 6620 7665 7262 6f73 653a 0a20     if verbose:. 
+0001a670: 2020 2020 2020 2070 7269 6e74 2822 4a6f         print("Jo
+0001a680: 696e 696e 6720 7570 7065 7220 616e 6420  ining upper and 
+0001a690: 6c6f 7765 7220 6d6f 7361 6963 2e2e 2e20  lower mosaic... 
+0001a6a0: 2853 7465 7020 322f 3329 2229 0a20 2020  (Step 2/3)").   
+0001a6b0: 2076 6572 7469 6361 6c5f 7669 6465 6f5f   vertical_video_
+0001a6c0: 636f 6e63 6174 656e 6174 6f72 280a 2020  concatenator(.  
+0001a6d0: 2020 2020 2020 7669 6465 6f5f 7061 7468        video_path
+0001a6e0: 733d 5b75 7070 6572 5f70 6174 682c 206c  s=[upper_path, l
+0001a6f0: 6f77 6572 5f70 6174 685d 2c0a 2020 2020  ower_path],.    
+0001a700: 2020 2020 7361 7665 5f70 6174 683d 7361      save_path=sa
+0001a710: 7665 5f70 6174 682c 0a20 2020 2020 2020  ve_path,.       
+0001a720: 2076 6572 626f 7365 3d76 6572 626f 7365   verbose=verbose
+0001a730: 2c0a 2020 2020 2020 2020 6770 753d 6770  ,.        gpu=gp
+0001a740: 752c 0a20 2020 2020 2020 2077 6964 7468  u,.        width
+0001a750: 5f70 783d 6d61 7828 5b78 5b22 7769 6474  _px=max([x["widt
+0001a760: 6822 5d20 666f 7220 7820 696e 2070 616e  h"] for x in pan
+0001a770: 656c 735f 6d65 7461 5d29 2c0a 2020 2020  els_meta]),.    
+0001a780: 290a 2020 2020 7469 6d65 722e 7374 6f70  ).    timer.stop
+0001a790: 5f74 696d 6572 2829 0a20 2020 2073 6875  _timer().    shu
+0001a7a0: 7469 6c2e 726d 7472 6565 2874 656d 705f  til.rmtree(temp_
+0001a7b0: 6469 7229 0a20 2020 2069 6620 7665 7262  dir).    if verb
+0001a7c0: 6f73 653a 0a20 2020 2020 2020 2070 7269  ose:.        pri
+0001a7d0: 6e74 280a 2020 2020 2020 2020 2020 2020  nt(.            
+0001a7e0: 6622 4d6f 7361 6963 2063 6f6e 6361 7465  f"Mosaic concate
+0001a7f0: 6e61 7469 6f6e 2063 6f6d 706c 6574 652e  nation complete.
+0001a800: 2053 6176 6564 2061 7420 7b73 6176 655f   Saved at {save_
+0001a810: 7061 7468 7d20 2845 6c61 7073 6564 2074  path} (Elapsed t
+0001a820: 696d 653a 207b 7469 6d65 722e 656c 6170  ime: {timer.elap
+0001a830: 7365 645f 7469 6d65 5f73 7472 7d73 2e29  sed_time_str}s.)
+0001a840: 220a 2020 2020 2020 2020 290a 0a0a 6465  ".        )...de
+0001a850: 6620 6d69 7865 645f 6d6f 7361 6963 5f63  f mixed_mosaic_c
+0001a860: 6f6e 6361 7465 6e61 746f 7228 0a20 2020  oncatenator(.   
+0001a870: 2076 6964 656f 5f70 6174 6873 3a20 4c69   video_paths: Li
+0001a880: 7374 5b55 6e69 6f6e 5b73 7472 2c20 6f73  st[Union[str, os
+0001a890: 2e50 6174 684c 696b 655d 5d2c 0a20 2020  .PathLike]],.   
+0001a8a0: 2073 6176 655f 7061 7468 3a20 556e 696f   save_path: Unio
+0001a8b0: 6e5b 7374 722c 206f 732e 5061 7468 4c69  n[str, os.PathLi
+0001a8c0: 6b65 5d2c 0a20 2020 2067 7075 3a20 4f70  ke],.    gpu: Op
+0001a8d0: 7469 6f6e 616c 5b62 6f6f 6c5d 203d 2046  tional[bool] = F
+0001a8e0: 616c 7365 2c0a 2020 2020 7665 7262 6f73  alse,.    verbos
+0001a8f0: 653a 204f 7074 696f 6e61 6c5b 626f 6f6c  e: Optional[bool
+0001a900: 5d20 3d20 5472 7565 2c0a 2020 2020 756e  ] = True,.    un
+0001a910: 6576 656e 5f66 696c 6c5f 636f 6c6f 723a  even_fill_color:
+0001a920: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+0001a930: 2022 626c 6163 6b22 2c0a 2920 2d3e 204e   "black",.) -> N
+0001a940: 6f6e 653a 0a20 2020 2022 2222 0a20 2020  one:.    """.   
+0001a950: 2043 7265 6174 6520 6120 6d69 7865 6420   Create a mixed 
+0001a960: 6d6f 7361 6963 2076 6964 656f 2062 7920  mosaic video by 
+0001a970: 636f 6e63 6174 656e 6174 696e 6720 6d75  concatenating mu
+0001a980: 6c74 6970 6c65 2069 6e70 7574 2076 6964  ltiple input vid
+0001a990: 656f 7320 696e 2061 206d 6f73 6169 6320  eos in a mosaic 
+0001a9a0: 6c61 796f 7574 206f 6620 7661 7269 6f75  layout of variou
+0001a9b0: 7320 7369 7a65 732e 0a0a 2020 2020 2e2e  s sizes...    ..
+0001a9c0: 2069 6d61 6765 3a3a 205f 7374 6174 6963   image:: _static
+0001a9d0: 2f69 6d67 2f6d 6978 6564 5f6d 6f73 6169  /img/mixed_mosai
+0001a9e0: 635f 636f 6e63 6174 656e 6174 6f72 2e70  c_concatenator.p
+0001a9f0: 6e67 0a20 2020 2020 2020 3a77 6964 7468  ng.       :width
+0001aa00: 3a20 3630 300a 2020 2020 2020 203a 616c  : 600.       :al
+0001aa10: 6967 6e3a 2063 656e 7465 720a 0a20 2020  ign: center..   
+0001aa20: 202e 2e20 6e6f 7465 3a3a 0a20 2020 2020   .. note::.     
+0001aa30: 2020 5468 6520 7265 736f 6c75 7469 6f6e    The resolution
+0001aa40: 206f 6620 7468 6520 6f75 7470 7574 2076   of the output v
+0001aa50: 6964 656f 2069 7320 6465 7465 726d 696e  ideo is determin
+0001aa60: 6564 2062 7920 7468 6520 7265 736f 6c75  ed by the resolu
+0001aa70: 7469 6f6e 206f 6620 7468 6520 7669 6465  tion of the vide
+0001aa80: 6f20 7061 7468 2061 7420 7468 6520 6669  o path at the fi
+0001aa90: 7273 7420 696e 6465 782e 0a0a 2020 2020  rst index...    
+0001aaa0: 2020 2049 6620 616e 2075 6e65 7665 6e20     If an uneven 
+0001aab0: 6e75 6d62 6572 206f 6620 7269 6768 742d  number of right-
+0001aac0: 7061 6e65 6c20 7669 6465 6f73 2028 2069  panel videos ( i
+0001aad0: 6620 6e6f 7420 286c 656e 2876 6964 656f  f not (len(video
+0001aae0: 5f70 6174 6873 292d 3129 2025 2032 2920  _paths)-1) % 2) 
+0001aaf0: 3d3d 2030 292c 2074 6865 6e20 7468 6520  == 0), then the 
+0001ab00: 6c61 7374 2069 6e64 6578 2077 696c 6c20  last index will 
+0001ab10: 6265 2066 696c 6c65 6420 6279 2060 6075  be filled by ``u
+0001ab20: 6e65 7665 6e5f 6669 6c6c 5f63 6f6c 6f72  neven_fill_color
+0001ab30: 6060 2e0a 0a20 2020 203a 7061 7261 6d20  ``...    :param 
+0001ab40: 4c69 7374 5b55 6e69 6f6e 5b73 7472 2c20  List[Union[str, 
+0001ab50: 6f73 2e50 6174 684c 696b 655d 5d20 7669  os.PathLike]] vi
+0001ab60: 6465 6f5f 7061 7468 733a 204c 6973 7420  deo_paths: List 
+0001ab70: 6f66 2069 6e70 7574 2076 6964 656f 2066  of input video f
+0001ab80: 696c 6520 7061 7468 732e 0a20 2020 203a  ile paths..    :
+0001ab90: 7061 7261 6d20 556e 696f 6e5b 7374 722c  param Union[str,
+0001aba0: 206f 732e 5061 7468 4c69 6b65 5d20 7361   os.PathLike] sa
+0001abb0: 7665 5f70 6174 683a 2046 696c 6520 7061  ve_path: File pa
+0001abc0: 7468 2074 6f20 7361 7665 2074 6865 2063  th to save the c
+0001abd0: 6f6e 6361 7465 6e61 7465 6420 7669 6465  oncatenated vide
+0001abe0: 6f2e 0a20 2020 203a 7061 7261 6d20 4f70  o..    :param Op
+0001abf0: 7469 6f6e 616c 5b62 6f6f 6c5d 2067 7075  tional[bool] gpu
+0001ac00: 3a20 5768 6574 6865 7220 746f 2075 7365  : Whether to use
+0001ac10: 2047 5055 2d61 6363 656c 6572 6174 6564   GPU-accelerated
+0001ac20: 2063 6f64 6563 2028 6465 6661 756c 743a   codec (default:
+0001ac30: 2046 616c 7365 292e 0a20 2020 203a 7061   False)..    :pa
+0001ac40: 7261 6d20 4f70 7469 6f6e 616c 5b62 6f6f  ram Optional[boo
+0001ac50: 6c5d 2076 6572 626f 7365 3a20 5768 6574  l] verbose: Whet
+0001ac60: 6865 7220 746f 2070 7269 6e74 2070 726f  her to print pro
+0001ac70: 6772 6573 7320 6d65 7373 6167 6573 2028  gress messages (
+0001ac80: 6465 6661 756c 743a 2054 7275 6529 2e0a  default: True)..
+0001ac90: 0a20 2020 203a 6578 616d 706c 653a 0a20  .    :example:. 
+0001aca0: 2020 203e 3e3e 2076 6964 656f 5f70 6174     >>> video_pat
+0001acb0: 6873 203d 205b 2776 6964 656f 312e 6d70  hs = ['video1.mp
+0001acc0: 3427 2c20 2776 6964 656f 322e 6d70 3427  4', 'video2.mp4'
+0001acd0: 2c20 2776 6964 656f 332e 6d70 3427 5d0a  , 'video3.mp4'].
+0001ace0: 2020 2020 3e3e 3e20 7361 7665 5f70 6174      >>> save_pat
+0001acf0: 6820 3d20 272f 5573 6572 732f 7369 6d6f  h = '/Users/simo
+0001ad00: 6e2f 4465 736b 746f 702f 656e 7673 2f73  n/Desktop/envs/s
+0001ad10: 696d 6261 2f74 726f 7562 6c65 7368 6f6f  imba/troubleshoo
+0001ad20: 7469 6e67 2f52 4154 5f4e 4f52 2f70 726f  ting/RAT_NOR/pro
+0001ad30: 6a65 6374 5f66 6f6c 6465 722f 7669 6465  ject_folder/vide
+0001ad40: 6f73 2f74 6573 742f 6e65 772f 626c 616e  os/test/new/blan
+0001ad50: 6b5f 7465 7374 2e6d 7034 270a 2020 2020  k_test.mp4'.    
+0001ad60: 3e3e 3e20 6d69 7865 645f 6d6f 7361 6963  >>> mixed_mosaic
+0001ad70: 5f63 6f6e 6361 7465 6e61 746f 7228 7669  _concatenator(vi
+0001ad80: 6465 6f5f 7061 7468 733d 7669 6465 6f5f  deo_paths=video_
+0001ad90: 7061 7468 732c 2073 6176 655f 7061 7468  paths, save_path
+0001ada0: 3d73 6176 655f 7061 7468 2c20 6770 753d  =save_path, gpu=
+0001adb0: 4661 6c73 652c 2076 6572 626f 7365 3d54  False, verbose=T
+0001adc0: 7275 6529 0a20 2020 2022 2222 0a0a 2020  rue).    """..  
+0001add0: 2020 6368 6563 6b5f 6666 6d70 6567 5f61    check_ffmpeg_a
+0001ade0: 7661 696c 6162 6c65 2829 0a20 2020 2069  vailable().    i
+0001adf0: 6620 6770 7520 616e 6420 6e6f 7420 6368  f gpu and not ch
+0001ae00: 6563 6b5f 6e76 6964 6561 5f67 7075 5f61  eck_nvidea_gpu_a
+0001ae10: 7661 696c 6162 6c65 2829 3a0a 2020 2020  vailable():.    
+0001ae20: 2020 2020 7261 6973 6520 4646 4d50 4547      raise FFMPEG
+0001ae30: 436f 6465 6347 5055 4572 726f 7228 6d73  CodecGPUError(ms
+0001ae40: 673d 224e 5649 4449 4120 4750 5520 6e6f  g="NVIDIA GPU no
+0001ae50: 7420 6176 6169 6c61 626c 6522 2c20 736f  t available", so
+0001ae60: 7572 6365 3d6d 6978 6564 5f6d 6f73 6169  urce=mixed_mosai
+0001ae70: 635f 636f 6e63 6174 656e 6174 6f72 2e5f  c_concatenator._
+0001ae80: 5f6e 616d 655f 5f29 0a20 2020 2074 696d  _name__).    tim
+0001ae90: 6572 203d 2053 696d 6261 5469 6d65 7228  er = SimbaTimer(
+0001aea0: 7374 6172 743d 5472 7565 290a 2020 2020  start=True).    
+0001aeb0: 6368 6563 6b5f 7661 6c69 645f 6c73 7428  check_valid_lst(
+0001aec0: 6461 7461 3d76 6964 656f 5f70 6174 6873  data=video_paths
+0001aed0: 2c20 736f 7572 6365 3d6d 6978 6564 5f6d  , source=mixed_m
+0001aee0: 6f73 6169 635f 636f 6e63 6174 656e 6174  osaic_concatenat
+0001aef0: 6f72 2e5f 5f6e 616d 655f 5f2c 206d 696e  or.__name__, min
+0001af00: 5f6c 656e 3d32 290a 2020 2020 6474 203d  _len=2).    dt =
+0001af10: 2064 6174 6574 696d 652e 6e6f 7728 292e   datetime.now().
+0001af20: 7374 7266 7469 6d65 2822 2559 256d 2564  strftime("%Y%m%d
+0001af30: 2548 254d 2553 2229 0a20 2020 2076 6964  %H%M%S").    vid
+0001af40: 656f 5f6d 6574 615f 6461 7461 203d 205b  eo_meta_data = [
+0001af50: 6765 745f 7669 6465 6f5f 6d65 7461 5f64  get_video_meta_d
+0001af60: 6174 6128 7669 6465 6f5f 7061 7468 3d76  ata(video_path=v
+0001af70: 6964 656f 5f70 6174 6829 2066 6f72 2076  ideo_path) for v
+0001af80: 6964 656f 5f70 6174 6820 696e 2076 6964  ideo_path in vid
+0001af90: 656f 5f70 6174 6873 5d0a 2020 2020 6d61  eo_paths].    ma
+0001afa0: 785f 7669 6465 6f5f 6c65 6e67 7468 203d  x_video_length =
+0001afb0: 206d 6178 285b 785b 2276 6964 656f 5f6c   max([x["video_l
+0001afc0: 656e 6774 685f 7322 5d20 666f 7220 7820  ength_s"] for x 
+0001afd0: 696e 2076 6964 656f 5f6d 6574 615f 6461  in video_meta_da
+0001afe0: 7461 5d29 0a20 2020 2063 6865 636b 5f69  ta]).    check_i
+0001aff0: 665f 6469 725f 6578 6973 7473 280a 2020  f_dir_exists(.  
+0001b000: 2020 2020 2020 696e 5f64 6972 3d6f 732e        in_dir=os.
+0001b010: 7061 7468 2e64 6972 6e61 6d65 2873 6176  path.dirname(sav
+0001b020: 655f 7061 7468 292c 2073 6f75 7263 653d  e_path), source=
+0001b030: 6d69 7865 645f 6d6f 7361 6963 5f63 6f6e  mixed_mosaic_con
+0001b040: 6361 7465 6e61 746f 722e 5f5f 6e61 6d65  catenator.__name
+0001b050: 5f5f 0a20 2020 2029 0a20 2020 206c 6172  __.    ).    lar
+0001b060: 6765 5f6d 6f73 6169 635f 7061 7468 2c20  ge_mosaic_path, 
+0001b070: 7669 6465 6f5f 7061 7468 7320 3d20 7669  video_paths = vi
+0001b080: 6465 6f5f 7061 7468 735b 305d 2c20 7669  deo_paths[0], vi
+0001b090: 6465 6f5f 7061 7468 735b 313a 5d0a 2020  deo_paths[1:].  
+0001b0a0: 2020 6d6f 7361 6963 5f68 6569 6768 7420    mosaic_height 
+0001b0b0: 3d20 696e 7428 7669 6465 6f5f 6d65 7461  = int(video_meta
+0001b0c0: 5f64 6174 615b 305d 5b22 6865 6967 6874  _data[0]["height
+0001b0d0: 225d 202f 2032 290a 2020 2020 6966 2076  "] / 2).    if v
+0001b0e0: 6572 626f 7365 3a0a 2020 2020 2020 2020  erbose:.        
+0001b0f0: 7072 696e 7428 2243 7265 6174 696e 6720  print("Creating 
+0001b100: 6d69 7865 6420 6d6f 7361 6963 2076 6964  mixed mosaic vid
+0001b110: 656f 2e2e 2e20 2229 0a20 2020 2074 656d  eo... ").    tem
+0001b120: 705f 6469 7220 3d20 6f73 2e70 6174 682e  p_dir = os.path.
+0001b130: 6a6f 696e 286f 732e 7061 7468 2e64 6972  join(os.path.dir
+0001b140: 6e61 6d65 286c 6172 6765 5f6d 6f73 6169  name(large_mosai
+0001b150: 635f 7061 7468 292c 2066 2274 656d 705f  c_path), f"temp_
+0001b160: 7b64 747d 2229 0a20 2020 206f 732e 6d61  {dt}").    os.ma
+0001b170: 6b65 6469 7273 2874 656d 705f 6469 7229  kedirs(temp_dir)
+0001b180: 0a20 2020 2069 6620 6e6f 7420 286c 656e  .    if not (len
+0001b190: 2876 6964 656f 5f70 6174 6873 2920 2520  (video_paths) % 
+0001b1a0: 3229 203d 3d20 303a 0a20 2020 2020 2020  2) == 0:.       
+0001b1b0: 2062 6c61 6e6b 5f70 6174 6820 3d20 6f73   blank_path = os
+0001b1c0: 2e70 6174 682e 6a6f 696e 2874 656d 705f  .path.join(temp_
+0001b1d0: 6469 722c 2066 227b 6474 7d2e 6d70 3422  dir, f"{dt}.mp4"
+0001b1e0: 290a 2020 2020 2020 2020 6372 6561 7465  ).        create
+0001b1f0: 5f62 6c61 6e6b 5f76 6964 656f 280a 2020  _blank_video(.  
+0001b200: 2020 2020 2020 2020 2020 7061 7468 3d62            path=b
+0001b210: 6c61 6e6b 5f70 6174 682c 0a20 2020 2020  lank_path,.     
+0001b220: 2020 2020 2020 206c 656e 6774 683d 6d61         length=ma
+0001b230: 785f 7669 6465 6f5f 6c65 6e67 7468 2c0a  x_video_length,.
+0001b240: 2020 2020 2020 2020 2020 2020 7769 6474              widt
+0001b250: 683d 6765 745f 7669 6465 6f5f 6d65 7461  h=get_video_meta
+0001b260: 5f64 6174 6128 7669 6465 6f5f 7061 7468  _data(video_path
+0001b270: 3d76 6964 656f 5f70 6174 6873 5b2d 315d  =video_paths[-1]
+0001b280: 295b 2277 6964 7468 225d 2c0a 2020 2020  )["width"],.    
+0001b290: 2020 2020 2020 2020 6865 6967 6874 3d67          height=g
+0001b2a0: 6574 5f76 6964 656f 5f6d 6574 615f 6461  et_video_meta_da
+0001b2b0: 7461 2876 6964 656f 5f70 6174 683d 7669  ta(video_path=vi
+0001b2c0: 6465 6f5f 7061 7468 735b 2d31 5d29 5b22  deo_paths[-1])["
+0001b2d0: 6865 6967 6874 225d 2c0a 2020 2020 2020  height"],.      
+0001b2e0: 2020 2020 2020 6770 753d 6770 752c 0a20        gpu=gpu,. 
+0001b2f0: 2020 2020 2020 2020 2020 2076 6572 626f             verbo
+0001b300: 7365 3d54 7275 652c 0a20 2020 2020 2020  se=True,.       
+0001b310: 2020 2020 2063 6f6c 6f72 3d75 6e65 7665       color=uneve
+0001b320: 6e5f 6669 6c6c 5f63 6f6c 6f72 2c0a 2020  n_fill_color,.  
+0001b330: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0001b340: 7669 6465 6f5f 7061 7468 732e 6170 7065  video_paths.appe
+0001b350: 6e64 2862 6c61 6e6b 5f70 6174 6829 0a20  nd(blank_path). 
+0001b360: 2020 2075 7070 6572 5f76 6964 656f 732c     upper_videos,
+0001b370: 206c 6f77 6572 5f76 6964 656f 7320 3d20   lower_videos = 
+0001b380: 2876 6964 656f 5f70 6174 6873 5b3a 206c  (video_paths[: l
+0001b390: 656e 2876 6964 656f 5f70 6174 6873 2920  en(video_paths) 
+0001b3a0: 2f2f 2032 5d2c 2076 6964 656f 5f70 6174  // 2], video_pat
+0001b3b0: 6873 5b6c 656e 2876 6964 656f 5f70 6174  hs[len(video_pat
+0001b3c0: 6873 2920 2f2f 2032 203a 5d29 0a20 2020  hs) // 2 :]).   
+0001b3d0: 2069 6620 7665 7262 6f73 653a 0a20 2020   if verbose:.   
+0001b3e0: 2020 2020 2070 7269 6e74 2822 4372 6561       print("Crea
+0001b3f0: 7469 6e67 2075 7070 6572 2072 6967 6874  ting upper right
+0001b400: 206d 6f73 6169 6320 2e2e 2e20 2853 7465   mosaic ... (Ste
+0001b410: 7020 312f 3429 2229 0a20 2020 2069 6620  p 1/4)").    if 
+0001b420: 6c65 6e28 7570 7065 725f 7669 6465 6f73  len(upper_videos
+0001b430: 2920 3e20 313a 0a20 2020 2020 2020 2075  ) > 1:.        u
+0001b440: 7070 6572 5f70 6174 6820 3d20 6f73 2e70  pper_path = os.p
+0001b450: 6174 682e 6a6f 696e 2874 656d 705f 6469  ath.join(temp_di
+0001b460: 722c 2022 7570 7065 722e 6d70 3422 290a  r, "upper.mp4").
+0001b470: 2020 2020 2020 2020 686f 7269 7a6f 6e74          horizont
+0001b480: 616c 5f76 6964 656f 5f63 6f6e 6361 7465  al_video_concate
+0001b490: 6e61 746f 7228 0a20 2020 2020 2020 2020  nator(.         
+0001b4a0: 2020 2076 6964 656f 5f70 6174 6873 3d75     video_paths=u
+0001b4b0: 7070 6572 5f76 6964 656f 732c 0a20 2020  pper_videos,.   
+0001b4c0: 2020 2020 2020 2020 2073 6176 655f 7061           save_pa
+0001b4d0: 7468 3d75 7070 6572 5f70 6174 682c 0a20  th=upper_path,. 
+0001b4e0: 2020 2020 2020 2020 2020 2067 7075 3d67             gpu=g
+0001b4f0: 7075 2c0a 2020 2020 2020 2020 2020 2020  pu,.            
+0001b500: 6865 6967 6874 5f70 783d 6d6f 7361 6963  height_px=mosaic
+0001b510: 5f68 6569 6768 742c 0a20 2020 2020 2020  _height,.       
+0001b520: 2020 2020 2076 6572 626f 7365 3d76 6572       verbose=ver
+0001b530: 626f 7365 2c0a 2020 2020 2020 2020 290a  bose,.        ).
+0001b540: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0001b550: 2020 7570 7065 725f 7061 7468 203d 2075    upper_path = u
+0001b560: 7070 6572 5f76 6964 656f 735b 305d 0a20  pper_videos[0]. 
+0001b570: 2020 2069 6620 7665 7262 6f73 653a 0a20     if verbose:. 
+0001b580: 2020 2020 2020 2070 7269 6e74 2822 4372         print("Cr
+0001b590: 6561 7469 6e67 206c 6f77 6572 2072 6967  eating lower rig
+0001b5a0: 6874 206d 6f73 6169 6320 2e2e 2e20 2853  ht mosaic ... (S
+0001b5b0: 7465 7020 322f 3429 2229 0a20 2020 2069  tep 2/4)").    i
+0001b5c0: 6620 6c65 6e28 6c6f 7765 725f 7669 6465  f len(lower_vide
+0001b5d0: 6f73 2920 3e20 313a 0a20 2020 2020 2020  os) > 1:.       
+0001b5e0: 206c 6f77 6572 5f70 6174 6820 3d20 6f73   lower_path = os
+0001b5f0: 2e70 6174 682e 6a6f 696e 2874 656d 705f  .path.join(temp_
+0001b600: 6469 722c 2022 6c6f 7765 722e 6d70 3422  dir, "lower.mp4"
+0001b610: 290a 2020 2020 2020 2020 686f 7269 7a6f  ).        horizo
+0001b620: 6e74 616c 5f76 6964 656f 5f63 6f6e 6361  ntal_video_conca
+0001b630: 7465 6e61 746f 7228 7669 6465 6f5f 7061  tenator(video_pa
+0001b640: 7468 733d 6c6f 7765 725f 7669 6465 6f73  ths=lower_videos
+0001b650: 2c20 7361 7665 5f70 6174 683d 6c6f 7765  , save_path=lowe
+0001b660: 725f 7061 7468 2c20 6770 753d 6770 752c  r_path, gpu=gpu,
+0001b670: 2076 6572 626f 7365 3d76 6572 626f 7365   verbose=verbose
+0001b680: 2c20 6865 6967 6874 5f70 783d 6d6f 7361  , height_px=mosa
+0001b690: 6963 5f68 6569 6768 7429 0a20 2020 2065  ic_height).    e
+0001b6a0: 6c73 653a 0a20 2020 2020 2020 206c 6f77  lse:.        low
+0001b6b0: 6572 5f70 6174 6820 3d20 6c6f 7765 725f  er_path = lower_
+0001b6c0: 7669 6465 6f73 5b30 5d0a 2020 2020 7061  videos[0].    pa
+0001b6d0: 6e65 6c73 5f6d 6574 6120 3d20 5b0a 2020  nels_meta = [.  
+0001b6e0: 2020 2020 2020 6765 745f 7669 6465 6f5f        get_video_
+0001b6f0: 6d65 7461 5f64 6174 6128 7669 6465 6f5f  meta_data(video_
+0001b700: 7061 7468 3d76 6964 656f 5f70 6174 6829  path=video_path)
+0001b710: 0a20 2020 2020 2020 2066 6f72 2076 6964  .        for vid
+0001b720: 656f 5f70 6174 6820 696e 205b 6c6f 7765  eo_path in [lowe
+0001b730: 725f 7061 7468 2c20 7570 7065 725f 7061  r_path, upper_pa
+0001b740: 7468 5d0a 2020 2020 5d0a 2020 2020 6d6f  th].    ].    mo
+0001b750: 7361 6963 5f70 6174 6820 3d20 6f73 2e70  saic_path = os.p
+0001b760: 6174 682e 6a6f 696e 2874 656d 705f 6469  ath.join(temp_di
+0001b770: 722c 2022 6d6f 7361 6963 2e6d 7034 2229  r, "mosaic.mp4")
+0001b780: 0a20 2020 2069 6620 7665 7262 6f73 653a  .    if verbose:
+0001b790: 0a20 2020 2020 2020 2070 7269 6e74 2822  .        print("
+0001b7a0: 4a6f 696e 696e 6720 7570 7065 7220 616e  Joining upper an
+0001b7b0: 6420 6c6f 7765 7220 7269 6768 7420 6d6f  d lower right mo
+0001b7c0: 7361 6963 2e2e 2e20 2853 7465 7020 332f  saic... (Step 3/
+0001b7d0: 3429 2229 0a20 2020 2076 6572 7469 6361  4)").    vertica
+0001b7e0: 6c5f 7669 6465 6f5f 636f 6e63 6174 656e  l_video_concaten
+0001b7f0: 6174 6f72 280a 2020 2020 2020 2020 7669  ator(.        vi
+0001b800: 6465 6f5f 7061 7468 733d 5b75 7070 6572  deo_paths=[upper
+0001b810: 5f70 6174 682c 206c 6f77 6572 5f70 6174  _path, lower_pat
+0001b820: 685d 2c0a 2020 2020 2020 2020 7769 6474  h],.        widt
+0001b830: 685f 7078 3d6d 6178 285b 785b 2277 6964  h_px=max([x["wid
+0001b840: 7468 225d 2066 6f72 2078 2069 6e20 7061  th"] for x in pa
+0001b850: 6e65 6c73 5f6d 6574 615d 292c 0a20 2020  nels_meta]),.   
+0001b860: 2020 2020 2073 6176 655f 7061 7468 3d6d       save_path=m
+0001b870: 6f73 6169 635f 7061 7468 2c0a 2020 2020  osaic_path,.    
+0001b880: 2020 2020 6770 753d 6770 752c 0a20 2020      gpu=gpu,.   
+0001b890: 2020 2020 2076 6572 626f 7365 3d76 6572       verbose=ver
+0001b8a0: 626f 7365 2c0a 2020 2020 290a 2020 2020  bose,.    ).    
+0001b8b0: 6966 2076 6572 626f 7365 3a0a 2020 2020  if verbose:.    
+0001b8c0: 2020 2020 7072 696e 7428 224a 6f69 6e69      print("Joini
+0001b8d0: 6e67 206c 6566 7420 616e 6420 7269 6768  ng left and righ
+0001b8e0: 7420 6d6f 7361 6963 2e2e 2e20 2853 7465  t mosaic... (Ste
+0001b8f0: 7020 342f 3429 2229 0a20 2020 2068 6f72  p 4/4)").    hor
+0001b900: 697a 6f6e 7461 6c5f 7669 6465 6f5f 636f  izontal_video_co
+0001b910: 6e63 6174 656e 6174 6f72 280a 2020 2020  ncatenator(.    
+0001b920: 2020 2020 7669 6465 6f5f 7061 7468 733d      video_paths=
+0001b930: 5b6c 6172 6765 5f6d 6f73 6169 635f 7061  [large_mosaic_pa
+0001b940: 7468 2c20 6d6f 7361 6963 5f70 6174 685d  th, mosaic_path]
+0001b950: 2c0a 2020 2020 2020 2020 6865 6967 6874  ,.        height
+0001b960: 5f69 6478 3d30 2c0a 2020 2020 2020 2020  _idx=0,.        
+0001b970: 7361 7665 5f70 6174 683d 7361 7665 5f70  save_path=save_p
+0001b980: 6174 682c 0a20 2020 2020 2020 2067 7075  ath,.        gpu
+0001b990: 3d67 7075 2c0a 2020 2020 290a 2020 2020  =gpu,.    ).    
+0001b9a0: 7469 6d65 722e 7374 6f70 5f74 696d 6572  timer.stop_timer
+0001b9b0: 2829 0a20 2020 2023 7368 7574 696c 2e72  ().    #shutil.r
+0001b9c0: 6d74 7265 6528 7465 6d70 5f64 6972 290a  mtree(temp_dir).
+0001b9d0: 2020 2020 6966 2076 6572 626f 7365 3a0a      if verbose:.
+0001b9e0: 2020 2020 2020 2020 7072 696e 7428 0a20          print(. 
+0001b9f0: 2020 2020 2020 2020 2020 2066 224d 6978             f"Mix
+0001ba00: 6564 206d 6f73 6169 6320 636f 6e63 6174  ed mosaic concat
+0001ba10: 656e 6174 696f 6e20 636f 6d70 6c65 7465  enation complete
+0001ba20: 2e20 5361 7665 6420 6174 207b 7361 7665  . Saved at {save
+0001ba30: 5f70 6174 687d 2028 456c 6170 7365 6420  _path} (Elapsed 
+0001ba40: 7469 6d65 3a20 7b74 696d 6572 2e65 6c61  time: {timer.ela
+0001ba50: 7073 6564 5f74 696d 655f 7374 727d 732e  psed_time_str}s.
+0001ba60: 2922 0a20 2020 2020 2020 2029 0a0a 0a23  )".        )...#
+0001ba70: 2076 6964 656f 5f70 6174 6873 203d 205b   video_paths = [
+0001ba80: 272f 5573 6572 732f 7369 6d6f 6e2f 4465  '/Users/simon/De
+0001ba90: 736b 746f 702f 656e 7673 2f73 696d 6261  sktop/envs/simba
+0001baa0: 2f74 726f 7562 6c65 7368 6f6f 7469 6e67  /troubleshooting
+0001bab0: 2f62 6565 7062 6f6f 7031 3734 2f70 726f  /beepboop174/pro
+0001bac0: 6a65 6374 5f66 6f6c 6465 722f 6d65 7267  ject_folder/merg
+0001bad0: 652f 5472 6961 6c20 2020 2031 305f 636c  e/Trial    10_cl
+0001bae0: 6970 7065 645f 6761 6e74 742e 6d70 3427  ipped_gantt.mp4'
+0001baf0: 2c0a 2320 2020 2020 2020 2020 2020 2020  ,.#             
+0001bb00: 2020 2027 2f55 7365 7273 2f73 696d 6f6e     '/Users/simon
+0001bb10: 2f44 6573 6b74 6f70 2f65 6e76 732f 7369  /Desktop/envs/si
+0001bb20: 6d62 612f 7472 6f75 626c 6573 686f 6f74  mba/troubleshoot
+0001bb30: 696e 672f 6265 6570 626f 6f70 3137 342f  ing/beepboop174/
+0001bb40: 7072 6f6a 6563 745f 666f 6c64 6572 2f6d  project_folder/m
+0001bb50: 6572 6765 2f54 7269 616c 2020 2020 3130  erge/Trial    10
+0001bb60: 5f63 6c69 7070 6564 2e6d 7034 272c 0a23  _clipped.mp4',.#
+0001bb70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bb80: 272f 5573 6572 732f 7369 6d6f 6e2f 4465  '/Users/simon/De
+0001bb90: 736b 746f 702f 656e 7673 2f73 696d 6261  sktop/envs/simba
+0001bba0: 2f74 726f 7562 6c65 7368 6f6f 7469 6e67  /troubleshooting
+0001bbb0: 2f62 6565 7062 6f6f 7031 3734 2f70 726f  /beepboop174/pro
+0001bbc0: 6a65 6374 5f66 6f6c 6465 722f 6d65 7267  ject_folder/merg
+0001bbd0: 652f 5472 6961 6c20 2020 2031 305f 636c  e/Trial    10_cl
+0001bbe0: 6970 7065 645f 6c69 6e65 2e6d 7034 272c  ipped_line.mp4',
+0001bbf0: 0a23 2020 2020 2020 2020 2020 2020 2020  .#              
+0001bc00: 2020 272f 5573 6572 732f 7369 6d6f 6e2f    '/Users/simon/
+0001bc10: 4465 736b 746f 702f 656e 7673 2f73 696d  Desktop/envs/sim
+0001bc20: 6261 2f74 726f 7562 6c65 7368 6f6f 7469  ba/troubleshooti
+0001bc30: 6e67 2f62 6565 7062 6f6f 7031 3734 2f70  ng/beepboop174/p
+0001bc40: 726f 6a65 6374 5f66 6f6c 6465 722f 6d65  roject_folder/me
+0001bc50: 7267 652f 5472 6961 6c20 2020 2020 335f  rge/Trial     3_
+0001bc60: 636c 6970 7065 642e 6d70 3427 5d0a 230a  clipped.mp4'].#.
+0001bc70: 2320 7669 6465 6f5f 7061 7468 7320 3d20  # video_paths = 
+0001bc80: 5b27 2f55 7365 7273 2f73 696d 6f6e 2f44  ['/Users/simon/D
+0001bc90: 6573 6b74 6f70 2f65 6e76 732f 7369 6d62  esktop/envs/simb
+0001bca0: 612f 7472 6f75 626c 6573 686f 6f74 696e  a/troubleshootin
+0001bcb0: 672f 6265 6570 626f 6f70 3137 342f 7072  g/beepboop174/pr
+0001bcc0: 6f6a 6563 745f 666f 6c64 6572 2f76 6964  oject_folder/vid
+0001bcd0: 656f 732f 5472 6961 6c20 2020 2031 302e  eos/Trial    10.
+0001bce0: 6d70 3427 2c0a 2320 2020 2020 2020 2020  mp4',.#         
+0001bcf0: 2020 2020 2020 2027 2f55 7365 7273 2f73         '/Users/s
+0001bd00: 696d 6f6e 2f44 6573 6b74 6f70 2f65 6e76  imon/Desktop/env
+0001bd10: 732f 7369 6d62 612f 7472 6f75 626c 6573  s/simba/troubles
+0001bd20: 686f 6f74 696e 672f 6265 6570 626f 6f70  hooting/beepboop
+0001bd30: 3137 342f 7072 6f6a 6563 745f 666f 6c64  174/project_fold
+0001bd40: 6572 2f6d 6572 6765 2f54 7269 616c 2020  er/merge/Trial  
+0001bd50: 2020 3130 5f63 6c69 7070 6564 5f67 616e    10_clipped_gan
+0001bd60: 7474 2e6d 7034 272c 0a23 2020 2020 2020  tt.mp4',.#      
+0001bd70: 2020 2020 2020 2020 2020 272f 5573 6572            '/User
+0001bd80: 732f 7369 6d6f 6e2f 4465 736b 746f 702f  s/simon/Desktop/
+0001bd90: 656e 7673 2f73 696d 6261 2f74 726f 7562  envs/simba/troub
+0001bda0: 6c65 7368 6f6f 7469 6e67 2f62 6565 7062  leshooting/beepb
+0001bdb0: 6f6f 7031 3734 2f70 726f 6a65 6374 5f66  oop174/project_f
+0001bdc0: 6f6c 6465 722f 6d65 7267 652f 5472 6961  older/merge/Tria
+0001bdd0: 6c20 2020 2031 305f 636c 6970 7065 645f  l    10_clipped_
+0001bde0: 6c69 6e65 2e6d 7034 272c 0a23 2020 2020  line.mp4',.#    
+0001bdf0: 2020 2020 2020 2020 2020 2020 272f 5573              '/Us
+0001be00: 6572 732f 7369 6d6f 6e2f 4465 736b 746f  ers/simon/Deskto
+0001be10: 702f 656e 7673 2f73 696d 6261 2f74 726f  p/envs/simba/tro
+0001be20: 7562 6c65 7368 6f6f 7469 6e67 2f62 6565  ubleshooting/bee
+0001be30: 7062 6f6f 7031 3734 2f70 726f 6a65 6374  pboop174/project
+0001be40: 5f66 6f6c 6465 722f 6d65 7267 652f 5472  _folder/merge/Tr
+0001be50: 6961 6c20 2020 2020 335f 636c 6970 7065  ial     3_clippe
+0001be60: 642e 6d70 3427 5d0a 230a 2320 7361 7665  d.mp4'].#.# save
+0001be70: 5f70 6174 6820 3d20 272f 5573 6572 732f  _path = '/Users/
+0001be80: 7369 6d6f 6e2f 4465 736b 746f 702f 656e  simon/Desktop/en
+0001be90: 7673 2f73 696d 6261 2f74 726f 7562 6c65  vs/simba/trouble
+0001bea0: 7368 6f6f 7469 6e67 2f62 6565 7062 6f6f  shooting/beepboo
+0001beb0: 7031 3734 2f70 726f 6a65 6374 5f66 6f6c  p174/project_fol
+0001bec0: 6465 722f 6d65 7267 652f 6f75 742e 6d70  der/merge/out.mp
+0001bed0: 3427 0a0a 230a 2320 7669 6465 6f5f 7061  4'..#.# video_pa
+0001bee0: 7468 7320 3d20 5b27 2f55 7365 7273 2f73  ths = ['/Users/s
+0001bef0: 696d 6f6e 2f44 6573 6b74 6f70 2f65 6e76  imon/Desktop/env
+0001bf00: 732f 7369 6d62 612f 7472 6f75 626c 6573  s/simba/troubles
+0001bf10: 686f 6f74 696e 672f 6265 6570 626f 6f70  hooting/beepboop
+0001bf20: 3137 342f 7072 6f6a 6563 745f 666f 6c64  174/project_fold
+0001bf30: 6572 2f66 7261 6d65 732f 6f75 7470 7574  er/frames/output
+0001bf40: 2f67 616e 7474 5f70 6c6f 7473 2f54 7269  /gantt_plots/Tri
+0001bf50: 616c 2020 2020 3130 2e6d 7034 272c 0a23  al    10.mp4',.#
+0001bf60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bf70: 272f 5573 6572 732f 7369 6d6f 6e2f 4465  '/Users/simon/De
+0001bf80: 736b 746f 702f 656e 7673 2f73 696d 6261  sktop/envs/simba
+0001bf90: 2f74 726f 7562 6c65 7368 6f6f 7469 6e67  /troubleshooting
+0001bfa0: 2f62 6565 7062 6f6f 7031 3734 2f70 726f  /beepboop174/pro
+0001bfb0: 6a65 6374 5f66 6f6c 6465 722f 7669 6465  ject_folder/vide
+0001bfc0: 6f73 2f54 7269 616c 2020 2020 3130 2e6d  os/Trial    10.m
+0001bfd0: 7034 272c 0a23 2020 2020 2020 2020 2020  p4',.#          
+0001bfe0: 2020 2020 2020 272f 5573 6572 732f 7369        '/Users/si
+0001bff0: 6d6f 6e2f 4465 736b 746f 702f 656e 7673  mon/Desktop/envs
+0001c000: 2f73 696d 6261 2f74 726f 7562 6c65 7368  /simba/troublesh
+0001c010: 6f6f 7469 6e67 2f62 6565 7062 6f6f 7031  ooting/beepboop1
+0001c020: 3734 2f70 726f 6a65 6374 5f66 6f6c 6465  74/project_folde
+0001c030: 722f 6672 616d 6573 2f6f 7574 7075 742f  r/frames/output/
+0001c040: 6c69 6e65 5f70 6c6f 742f 5472 6961 6c20  line_plot/Trial 
+0001c050: 2020 2031 302e 6d70 3427 2c0a 2320 2020     10.mp4',.#   
+0001c060: 2020 2020 2020 2020 2020 2020 2027 2f55               '/U
+0001c070: 7365 7273 2f73 696d 6f6e 2f44 6573 6b74  sers/simon/Deskt
+0001c080: 6f70 2f65 6e76 732f 7369 6d62 612f 7472  op/envs/simba/tr
+0001c090: 6f75 626c 6573 686f 6f74 696e 672f 6265  oubleshooting/be
+0001c0a0: 6570 626f 6f70 3137 342f 7072 6f6a 6563  epboop174/projec
+0001c0b0: 745f 666f 6c64 6572 2f66 7261 6d65 732f  t_folder/frames/
+0001c0c0: 6f75 7470 7574 2f6c 696e 655f 706c 6f74  output/line_plot
+0001c0d0: 2f54 7269 616c 2020 2020 2033 2e6d 7034  /Trial     3.mp4
+0001c0e0: 275d 0a23 2073 6176 655f 7061 7468 203d  '].# save_path =
+0001c0f0: 2027 2f55 7365 7273 2f73 696d 6f6e 2f44   '/Users/simon/D
+0001c100: 6573 6b74 6f70 2f65 6e76 732f 7369 6d62  esktop/envs/simb
+0001c110: 612f 7472 6f75 626c 6573 686f 6f74 696e  a/troubleshootin
+0001c120: 672f 5241 545f 4e4f 522f 7072 6f6a 6563  g/RAT_NOR/projec
+0001c130: 745f 666f 6c64 6572 2f76 6964 656f 732f  t_folder/videos/
+0001c140: 7465 7374 2f6e 6577 2f62 6c61 6e6b 5f74  test/new/blank_t
+0001c150: 6573 742e 6d70 3427 0a0a 2320 7669 6465  est.mp4'..# vide
+0001c160: 6f5f 7061 7468 7320 3d20 5b27 2f55 7365  o_paths = ['/Use
+0001c170: 7273 2f73 696d 6f6e 2f44 6573 6b74 6f70  rs/simon/Desktop
+0001c180: 2f65 6e76 732f 7369 6d62 612f 7472 6f75  /envs/simba/trou
+0001c190: 626c 6573 686f 6f74 696e 672f 6265 6570  bleshooting/beep
+0001c1a0: 626f 6f70 3137 342f 7072 6f6a 6563 745f  boop174/project_
+0001c1b0: 666f 6c64 6572 2f76 6964 656f 732f 5472  folder/videos/Tr
+0001c1c0: 6961 6c20 2020 2031 302e 6d70 3427 2c0a  ial    10.mp4',.
+0001c1d0: 2320 2020 2020 2020 2020 2020 2020 2020  #               
+0001c1e0: 2027 2f55 7365 7273 2f73 696d 6f6e 2f44   '/Users/simon/D
+0001c1f0: 6573 6b74 6f70 2f65 6e76 732f 7369 6d62  esktop/envs/simb
+0001c200: 612f 7472 6f75 626c 6573 686f 6f74 696e  a/troubleshootin
+0001c210: 672f 6265 6570 626f 6f70 3137 342f 7072  g/beepboop174/pr
+0001c220: 6f6a 6563 745f 666f 6c64 6572 2f66 7261  oject_folder/fra
+0001c230: 6d65 732f 6f75 7470 7574 2f6c 696e 655f  mes/output/line_
+0001c240: 706c 6f74 2f54 7269 616c 2020 2020 3130  plot/Trial    10
+0001c250: 2e6d 7034 272c 0a23 2020 2020 2020 2020  .mp4',.#        
+0001c260: 2020 2020 2020 2020 272f 5573 6572 732f          '/Users/
+0001c270: 7369 6d6f 6e2f 4465 736b 746f 702f 656e  simon/Desktop/en
+0001c280: 7673 2f73 696d 6261 2f74 726f 7562 6c65  vs/simba/trouble
+0001c290: 7368 6f6f 7469 6e67 2f62 6565 7062 6f6f  shooting/beepboo
+0001c2a0: 7031 3734 2f70 726f 6a65 6374 5f66 6f6c  p174/project_fol
+0001c2b0: 6465 722f 6672 616d 6573 2f6f 7574 7075  der/frames/outpu
+0001c2c0: 742f 6c69 6e65 5f70 6c6f 742f 5472 6961  t/line_plot/Tria
+0001c2d0: 6c20 2020 2020 332e 6d70 3427 5d0a 0a23  l     3.mp4']..#
+0001c2e0: 6d69 7865 645f 6d6f 7361 6963 5f63 6f6e  mixed_mosaic_con
+0001c2f0: 6361 7465 6e61 746f 7228 7669 6465 6f5f  catenator(video_
+0001c300: 7061 7468 733d 7669 6465 6f5f 7061 7468  paths=video_path
+0001c310: 732c 2073 6176 655f 7061 7468 3d73 6176  s, save_path=sav
+0001c320: 655f 7061 7468 2c20 6770 753d 4661 6c73  e_path, gpu=Fals
+0001c330: 652c 2076 6572 626f 7365 3d54 7275 6529  e, verbose=True)
```

### Comparing `Simba-UW-tf-dev-1.89.7/simba/video_processors/.DS_Store` & `Simba-UW-tf-dev-1.89.8/simba/video_processors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/video_processors/roi_selector_circle.py` & `Simba-UW-tf-dev-1.89.8/simba/video_processors/roi_selector_circle.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/video_processors/px_to_mm.py` & `Simba-UW-tf-dev-1.89.8/simba/video_processors/px_to_mm.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/video_processors/batch_process_menus.py` & `Simba-UW-tf-dev-1.89.8/simba/video_processors/batch_process_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/video_processors/multi_cropper.py` & `Simba-UW-tf-dev-1.89.8/simba/video_processors/multi_cropper.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/video_processors/extract_frames.py` & `Simba-UW-tf-dev-1.89.8/simba/video_processors/extract_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/video_processors/roi_selector.py` & `Simba-UW-tf-dev-1.89.8/simba/video_processors/roi_selector.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/video_processors/calculate_px_dist.py` & `Simba-UW-tf-dev-1.89.8/simba/video_processors/calculate_px_dist.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/video_processors/roi_selector_polygon.py` & `Simba-UW-tf-dev-1.89.8/simba/video_processors/roi_selector_polygon.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/video_processors/extract_seqframes.py` & `Simba-UW-tf-dev-1.89.8/simba/video_processors/extract_seqframes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/video_processors/batch_process_create_ffmpeg_commands.py` & `Simba-UW-tf-dev-1.89.8/simba/video_processors/batch_process_create_ffmpeg_commands.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/outlier_tools/outlier_corrector_movement.py` & `Simba-UW-tf-dev-1.89.8/simba/outlier_tools/outlier_corrector_movement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/outlier_tools/outlier_corrector_location_advanced.py` & `Simba-UW-tf-dev-1.89.8/simba/outlier_tools/outlier_corrector_location_advanced.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/outlier_tools/outlier_corrector_movement_advanced.py` & `Simba-UW-tf-dev-1.89.8/simba/outlier_tools/outlier_corrector_movement_advanced.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/outlier_tools/outlier_corrector_location.py` & `Simba-UW-tf-dev-1.89.8/simba/outlier_tools/outlier_corrector_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/outlier_tools/skip_outlier_correction.py` & `Simba-UW-tf-dev-1.89.8/simba/outlier_tools/skip_outlier_correction.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/SimBA.py` & `Simba-UW-tf-dev-1.89.8/simba/SimBA.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/unsupervised/model_names.parquet` & `Simba-UW-tf-dev-1.89.8/simba/assets/unsupervised/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/unsupervised/features.csv` & `Simba-UW-tf-dev-1.89.8/simba/assets/unsupervised/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/shap/down_arrow.jpg` & `Simba-UW-tf-dev-1.89.8/simba/assets/shap/down_arrow.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/shap/intruder_shape.jpg` & `Simba-UW-tf-dev-1.89.8/simba/assets/shap/intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/shap/feature_categories/shap_feature_categories.csv` & `Simba-UW-tf-dev-1.89.8/simba/assets/shap/feature_categories/shap_feature_categories.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/shap/resident_shape.jpg` & `Simba-UW-tf-dev-1.89.8/simba/assets/shap/resident_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/shap/resident_intruder_shape.jpg` & `Simba-UW-tf-dev-1.89.8/simba/assets/shap/resident_intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/shap/animal_distances.jpg` & `Simba-UW-tf-dev-1.89.8/simba/assets/shap/animal_distances.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/shap/baseline_scale.jpg` & `Simba-UW-tf-dev-1.89.8/simba/assets/shap/baseline_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/shap/ubuntu.regular.ttf` & `Simba-UW-tf-dev-1.89.8/simba/assets/shap/ubuntu.regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/shap/side_scale.jpg` & `Simba-UW-tf-dev-1.89.8/simba/assets/shap/side_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/shap/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.89.8/simba/assets/shap/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/shap/side_scale_5.jpg` & `Simba-UW-tf-dev-1.89.8/simba/assets/shap/side_scale_5.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/shap/intruder_movement.jpg` & `Simba-UW-tf-dev-1.89.8/simba/assets/shap/intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/shap/resident_movement.jpg` & `Simba-UW-tf-dev-1.89.8/simba/assets/shap/resident_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/shap/color_bar.jpg` & `Simba-UW-tf-dev-1.89.8/simba/assets/shap/color_bar.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/shap/resident_intruder_movement.jpg` & `Simba-UW-tf-dev-1.89.8/simba/assets/shap/resident_intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/.DS_Store` & `Simba-UW-tf-dev-1.89.8/simba/assets/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/lookups/model_names.parquet` & `Simba-UW-tf-dev-1.89.8/simba/assets/lookups/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/lookups/feature_extraction_headers.csv` & `Simba-UW-tf-dev-1.89.8/simba/assets/lookups/feature_extraction_headers.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/lookups/critical_values_05.pickle` & `Simba-UW-tf-dev-1.89.8/simba/assets/lookups/critical_values_05.pickle`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/lookups/features.csv` & `Simba-UW-tf-dev-1.89.8/simba/assets/lookups/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/lookups/unsupervised_example_x.csv` & `Simba-UW-tf-dev-1.89.8/simba/assets/lookups/unsupervised_example_x.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/stl/operant_tray.stl` & `Simba-UW-tf-dev-1.89.8/simba/assets/stl/operant_tray.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/stl/operant_lever.stl` & `Simba-UW-tf-dev-1.89.8/simba/assets/stl/operant_lever.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/stl/operant_walls.stl` & `Simba-UW-tf-dev-1.89.8/simba/assets/stl/operant_walls.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/stl/grid_floor.stl` & `Simba-UW-tf-dev-1.89.8/simba/assets/stl/grid_floor.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/img/splash_2024.mp4` & `Simba-UW-tf-dev-1.89.8/simba/assets/img/splash_2024.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/img/bg_2024.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/img/bg_2024.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/img/about_me.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/img/about_me.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/img/splash.mp4` & `Simba-UW-tf-dev-1.89.8/simba/assets/img/splash.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/img/bg_2.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/img/bg_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/img/splash.pptx` & `Simba-UW-tf-dev-1.89.8/simba/assets/img/splash.pptx`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/img/bg.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/img/bg.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.89.8/simba/assets/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/factory.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/factory.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/cluster.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/cluster.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/load.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/load.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/gif.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/gif.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/pose.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/pose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/features.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/features.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/.DS_Store` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/settings.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/settings.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/stopwatch.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/stopwatch.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/link.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/link.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/dash_simba.css` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/dash_simba.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/documentation.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/documentation.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/fps.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/fps.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/dimensionality_reduction.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/dimensionality_reduction.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/roi.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/roi.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/simba_logo_2.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/simba_logo_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/superimpose.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/superimpose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/label.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/label.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/change.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/change.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/readthedocs_logo.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/readthedocs_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/crop.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/crop.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/rotate.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/rotate.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/circle.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/circle.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/path.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/path.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/polygon.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/polygon.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/clip.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/clip.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/restart.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/restart.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/calipher.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/calipher.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/add_on.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/add_on.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/create.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/create.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/SimBA_logo.ico` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/print.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/print.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/clf.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/clf.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/concat_icons/mosaic.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/concat_icons/mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/concat_icons/vertical.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/concat_icons/vertical.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/concat_icons/horizontal.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/concat_icons/horizontal.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/concat_icons/mixed_mosaic.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/concat_icons/mixed_mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/merge.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/merge.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/clean.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/clean.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/clf_2.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/clf_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/visualize.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/visualize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/concat.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/concat.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/boris.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/boris.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/frames.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/frames.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/video.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/video.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/sample.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/sample.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/metrics.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/metrics.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/grey.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/grey.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/exit.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/exit.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/outlier.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/outlier.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/clahe.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/clahe.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/trash.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/trash.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/about.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/about.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/convert.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/convert.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/SimBA_logo.icns` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/SimBA_logo.icns`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/reorganize.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/reorganize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/browse.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/browse.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/SimBA_logo.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/SimBA_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/ethovision.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/ethovision.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/icons/close.png` & `Simba-UW-tf-dev-1.89.8/simba/assets/icons/close.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/dash_simba_base.css` & `Simba-UW-tf-dev-1.89.8/simba/assets/dash_simba_base.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/simba/assets/TheGoldenLab.PNG` & `Simba-UW-tf-dev-1.89.8/simba/assets/TheGoldenLab.PNG`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/Simba_UW_tf_dev.egg-info/PKG-INFO` & `Simba-UW-tf-dev-1.89.8/Simba_UW_tf_dev.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.89.7
+Version: 1.89.8
 Summary: Toolkit for computer classification of behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.89.7/Simba_UW_tf_dev.egg-info/SOURCES.txt` & `Simba-UW-tf-dev-1.89.8/Simba_UW_tf_dev.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -339,14 +339,15 @@
 simba/sandbox/add_probability_cnt_features.py
 simba/sandbox/adjusted_rand_score.py
 simba/sandbox/amber_featurizer.py
 simba/sandbox/amber_tests.py
 simba/sandbox/batch_video_to_greyscale.py
 simba/sandbox/berger_parker.py
 simba/sandbox/biweight_midcorrelation.py
+simba/sandbox/bouts_df
 simba/sandbox/calc_N_degree_direction_switches.py
 simba/sandbox/calinski_harabasz.py
 simba/sandbox/cochran_q.py
 simba/sandbox/cohens_kappa.py
 simba/sandbox/colinear_features.py
 simba/sandbox/convex_hull_3_scratch_3.py
 simba/sandbox/convex_hull_scratch_1.py
@@ -403,14 +404,15 @@
 simba/sandbox/pct_counts_in_top_N.py
 simba/sandbox/peaks.py
 simba/sandbox/piotr_120324 2.py.zip
 simba/sandbox/piotr_120324 3.py.zip
 simba/sandbox/piotr_120324 4.py.zip
 simba/sandbox/piotr_120324.py
 simba/sandbox/piotr_120324.py.zip
+simba/sandbox/plotly_gantt.py
 simba/sandbox/read_in_mp.py
 simba/sandbox/redis.py
 simba/sandbox/roi_definition_csvs_to_h5.py
 simba/sandbox/roi_definition_csvs_to_h5.py.zip
 simba/sandbox/roi_feature_visualizer_example.py
 simba/sandbox/roi_feature_visualizer_example.py.zip
 simba/sandbox/runs_test.py
```

### Comparing `Simba-UW-tf-dev-1.89.7/Simba_UW_tf_dev.egg-info/requires.txt` & `Simba-UW-tf-dev-1.89.8/Simba_UW_tf_dev.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/LICENSE` & `Simba-UW-tf-dev-1.89.8/LICENSE`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/tests/test_data_processors.py` & `Simba-UW-tf-dev-1.89.8/tests/test_data_processors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/tests/test_circlular_stats.py` & `Simba-UW-tf-dev-1.89.8/tests/test_circlular_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/tests/test_stats.py` & `Simba-UW-tf-dev-1.89.8/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/tests/test_distance_plotter.py` & `Simba-UW-tf-dev-1.89.8/tests/test_distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/tests/test_train_model_mixin.py` & `Simba-UW-tf-dev-1.89.8/tests/test_train_model_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/tests/test_feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.89.8/tests/test_feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/tests/test_utils_data.py` & `Simba-UW-tf-dev-1.89.8/tests/test_utils_data.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/tests/test_config_reader_mixin.py` & `Simba-UW-tf-dev-1.89.8/tests/test_config_reader_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/tests/test_outlier_correctors.py` & `Simba-UW-tf-dev-1.89.8/tests/test_outlier_correctors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/tests/test_visualize_directing_animals.py` & `Simba-UW-tf-dev-1.89.8/tests/test_visualize_directing_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/tests/test_featurizers.py` & `Simba-UW-tf-dev-1.89.8/tests/test_featurizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/tests/test_video_processors.py` & `Simba-UW-tf-dev-1.89.8/tests/test_video_processors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/tests/test_thirdparty_appenders.py` & `Simba-UW-tf-dev-1.89.8/tests/test_thirdparty_appenders.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/tests/test_validation_clips.py` & `Simba-UW-tf-dev-1.89.8/tests/test_validation_clips.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/tests/test_roi_tools.py` & `Simba-UW-tf-dev-1.89.8/tests/test_roi_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/README.md` & `Simba-UW-tf-dev-1.89.8/README.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.89.7/setup.py` & `Simba-UW-tf-dev-1.89.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 
 exclusion_patterns = ["pose_configurations_archive"]
 
 setuptools.setup(
     name="Simba-UW-tf-dev",
-    version="1.89.7",
+    version="1.89.8",
     author="Simon Nilsson, Jia Jie Choong, Sophia Hwang",
     author_email="sronilsson@gmail.com",
     description="Toolkit for computer classification of behaviors in experimental animals",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/sgoldenlab/simba",
     install_requires=requirements,
```

