# Comparing `tmp/spine_segmentation-0.1.4.tar.gz` & `tmp/spine_segmentation-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spine_segmentation-0.1.4.tar", max compression
+gzip compressed data, was "spine_segmentation-0.1.5.tar", max compression
```

## Comparing `spine_segmentation-0.1.4.tar` & `spine_segmentation-0.1.5.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0     1211 2024-04-11 11:32:29.446351 spine_segmentation-0.1.4/README.md
--rw-r--r--   0        0        0     2382 2024-04-11 16:08:12.315294 spine_segmentation-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      122 2024-04-11 12:53:48.914194 spine_segmentation-0.1.4/spine_segmentation/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 12:31:20.207512 spine_segmentation-0.1.4/spine_segmentation/annotators/__init__.py
--rw-r--r--   0        0        0    16308 2024-04-11 12:53:48.934194 spine_segmentation-0.1.4/spine_segmentation/annotators/annotator_base.py
--rw-r--r--   0        0        0     8225 2024-04-11 12:53:48.814193 spine_segmentation-0.1.4/spine_segmentation/annotators/vector_annotator.py
--rw-r--r--   0        0        0     2190 2024-04-11 12:53:48.766192 spine_segmentation-0.1.4/spine_segmentation/cli/cli.py
--rw-r--r--   0        0        0    12072 2024-04-10 12:31:20.207512 spine_segmentation-0.1.4/spine_segmentation/dataloader/statistics.py
--rw-r--r--   0        0        0        0 2024-04-10 12:31:20.207512 spine_segmentation-0.1.4/spine_segmentation/datasets/__init__.py
--rw-r--r--   0        0        0     2868 2024-04-10 12:31:20.207512 spine_segmentation-0.1.4/spine_segmentation/datasets/augmentation.py
--rw-r--r--   0        0        0     4312 2024-04-11 12:53:48.806193 spine_segmentation-0.1.4/spine_segmentation/datasets/feature_dataset.py
--rw-r--r--   0        0        0     6696 2024-04-11 15:53:29.418496 spine_segmentation-0.1.4/spine_segmentation/datasets/metadata_prediction_dataset.py
--rw-r--r--   0        0        0     6372 2024-04-11 15:53:29.430496 spine_segmentation-0.1.4/spine_segmentation/datasets/patch_segmentation_dataset.py
--rw-r--r--   0        0        0     1360 2024-04-11 15:53:29.410496 spine_segmentation-0.1.4/spine_segmentation/datasets/path_helper.py
--rw-r--r--   0        0        0    14744 2024-04-11 15:47:48.534212 spine_segmentation-0.1.4/spine_segmentation/datasets/sample.py
--rw-r--r--   0        0        0    14989 2024-04-11 15:53:29.422496 spine_segmentation-0.1.4/spine_segmentation/datasets/segmentation_dataset.py
--rw-r--r--   0        0        0     2037 2024-04-11 12:53:48.782192 spine_segmentation-0.1.4/spine_segmentation/datasets/vector_table_graphs_dataset.py
--rw-r--r--   0        0        0     2581 2024-04-11 12:53:48.890194 spine_segmentation-0.1.4/spine_segmentation/evaluate/analyze_edge_cases.py
--rw-r--r--   0        0        0     2520 2024-04-11 12:53:48.798193 spine_segmentation-0.1.4/spine_segmentation/evaluate/analyze_index_list.py
--rw-r--r--   0        0        0     1659 2024-04-11 12:53:48.854193 spine_segmentation-0.1.4/spine_segmentation/evaluate/classic_ml.py
--rw-r--r--   0        0        0     1108 2024-04-10 12:31:20.207512 spine_segmentation-0.1.4/spine_segmentation/evaluate/eval_created_stats.py
--rw-r--r--   0        0        0    15527 2024-04-11 15:52:07.339228 spine_segmentation-0.1.4/spine_segmentation/evaluate/eval_instance_seg_model.py
--rw-r--r--   0        0        0     8215 2024-04-11 12:53:48.746192 spine_segmentation-0.1.4/spine_segmentation/evaluate/eval_splitting.py
--rw-r--r--   0        0        0     6109 2024-04-11 15:52:07.363228 spine_segmentation-0.1.4/spine_segmentation/evaluate/load_model.py
--rw-r--r--   0        0        0     4885 2024-04-11 12:53:48.882194 spine_segmentation-0.1.4/spine_segmentation/evaluate/metadata.py
--rw-r--r--   0        0        0     1627 2024-04-11 12:53:48.894194 spine_segmentation-0.1.4/spine_segmentation/evaluate/volume_size_in_gt.py
--rw-r--r--   0        0        0    15726 2024-04-11 15:52:07.351228 spine_segmentation-0.1.4/spine_segmentation/inference/instance_segmentation.py
--rw-r--r--   0        0        0     6761 2024-04-11 12:53:48.846193 spine_segmentation-0.1.4/spine_segmentation/inference/onnx_model.py
--rw-r--r--   0        0        0     7515 2024-04-11 12:53:48.906194 spine_segmentation-0.1.4/spine_segmentation/instance_separation/instance_separation.py
--rw-r--r--   0        0        0      304 2024-04-10 12:31:20.207512 spine_segmentation-0.1.4/spine_segmentation/losses/diffis1.py
--rw-r--r--   0        0        0     2080 2024-04-11 15:40:00.222464 spine_segmentation-0.1.4/spine_segmentation/model_downloader/model_downloader.py
--rw-r--r--   0        0        0      712 2024-04-11 12:53:48.850193 spine_segmentation-0.1.4/spine_segmentation/plotting/bmi.py
--rw-r--r--   0        0        0     8132 2024-04-11 12:53:48.778192 spine_segmentation-0.1.4/spine_segmentation/plotting/classification_correlation.py
--rw-r--r--   0        0        0     2566 2024-04-11 12:53:48.886194 spine_segmentation-0.1.4/spine_segmentation/plotting/patient_metadata.py
--rw-r--r--   0        0        0    10404 2024-04-11 12:53:48.826193 spine_segmentation-0.1.4/spine_segmentation/plotting/plot_slice.py
--rw-r--r--   0        0        0     1795 2024-04-11 12:53:48.938195 spine_segmentation-0.1.4/spine_segmentation/plotting/plot_statistics.py
--rw-r--r--   0        0        0     5823 2024-04-11 12:53:48.834193 spine_segmentation-0.1.4/spine_segmentation/plotting/read_npz_eval_per_roi_accuracy.py
--rw-r--r--   0        0        0     5767 2024-04-11 12:53:48.786192 spine_segmentation-0.1.4/spine_segmentation/plotting/show_plane_splitting_3d.py
--rw-r--r--   0        0        0      266 2024-04-11 12:53:48.858193 spine_segmentation-0.1.4/spine_segmentation/plotting/ydata_profile_report.py
--rw-r--r--   0        0        0      930 2024-04-11 15:55:12.773382 spine_segmentation-0.1.4/spine_segmentation/resources/paths.py
--rw-r--r--   0        0        0      933 2024-04-11 12:53:48.842193 spine_segmentation-0.1.4/spine_segmentation/resources/preloaded.py
--rw-r--r--   0        0        0       63 2024-04-11 09:34:14.336647 spine_segmentation-0.1.4/spine_segmentation/run.py
--rw-r--r--   0        0        0     4575 2024-04-10 12:31:20.207512 spine_segmentation-0.1.4/spine_segmentation/scripts/format_results.py
--rw-r--r--   0        0        0     4546 2024-04-11 12:53:48.866193 spine_segmentation-0.1.4/spine_segmentation/scripts/split_train_val_test.py
--rw-r--r--   0        0        0      210 2024-04-10 12:31:20.207512 spine_segmentation-0.1.4/spine_segmentation/scripts/test_patient_ids.txt
--rw-r--r--   0        0        0      112 2024-04-10 18:52:49.798849 spine_segmentation-0.1.4/spine_segmentation/spine_types/disc.py
--rw-r--r--   0        0        0     1033 2024-04-10 12:31:20.207512 spine_segmentation-0.1.4/spine_segmentation/spine_types/labels.py
--rw-r--r--   0        0        0      219 2024-04-10 12:31:20.207512 spine_segmentation-0.1.4/spine_segmentation/spine_types/line_segment.py
--rw-r--r--   0        0        0     2409 2024-04-10 12:31:20.207512 spine_segmentation-0.1.4/spine_segmentation/spine_types/plane.py
--rw-r--r--   0        0        0       67 2024-04-10 12:31:20.207512 spine_segmentation-0.1.4/spine_segmentation/spine_types/roi.py
--rw-r--r--   0        0        0      246 2024-04-10 12:31:20.207512 spine_segmentation-0.1.4/spine_segmentation/spine_types/spine.py
--rw-r--r--   0        0        0      116 2024-04-10 18:52:49.974852 spine_segmentation-0.1.4/spine_segmentation/spine_types/vertebra.py
--rw-r--r--   0        0        0     1190 2024-04-11 12:53:48.874194 spine_segmentation-0.1.4/spine_segmentation/trainer/learning_rate_finder.py
--rw-r--r--   0        0        0        0 2024-04-10 12:31:20.207512 spine_segmentation-0.1.4/spine_segmentation/utils/__init__.py
--rw-r--r--   0        0        0      685 2024-04-10 12:31:20.207512 spine_segmentation-0.1.4/spine_segmentation/utils/fix_validations_step_bar.py
--rw-r--r--   0        0        0      218 2024-04-10 12:31:20.207512 spine_segmentation-0.1.4/spine_segmentation/utils/globals.py
--rw-r--r--   0        0        0      552 2024-04-10 12:31:20.207512 spine_segmentation-0.1.4/spine_segmentation/utils/log_dir.py
--rw-r--r--   0        0        0      690 2024-04-10 12:31:20.207512 spine_segmentation-0.1.4/spine_segmentation/utils/profiling.py
--rw-r--r--   0        0        0      930 2024-04-10 12:31:20.207512 spine_segmentation-0.1.4/spine_segmentation/utils/proxy_class.py
--rw-r--r--   0        0        0        0 2024-04-10 12:31:20.207512 spine_segmentation-0.1.4/spine_segmentation/visualisation/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 12:31:20.207512 spine_segmentation-0.1.4/spine_segmentation/visualisation/blender/__init__.py
--rw-r--r--   0        0        0    11971 2024-04-10 12:31:20.207512 spine_segmentation-0.1.4/spine_segmentation/visualisation/blender/blender_script.py
--rw-r--r--   0        0        0     9179 2024-04-11 12:53:48.830193 spine_segmentation-0.1.4/spine_segmentation/visualisation/blender/gen_obj.py
--rw-r--r--   0        0        0     8158 2024-04-11 12:53:48.822193 spine_segmentation-0.1.4/spine_segmentation/visualisation/blender/open_in_blender.py
--rw-r--r--   0        0        0    12036 2024-04-10 12:31:20.207512 spine_segmentation-0.1.4/spine_segmentation/visualisation/color.py
--rw-r--r--   0        0        0     1705 2024-04-11 12:53:48.794192 spine_segmentation-0.1.4/spine_segmentation/visualisation/color_palettes.py
--rw-r--r--   0        0        0     2602 1970-01-01 00:00:00.000000 spine_segmentation-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-04-11 11:32:29.446351 spine_segmentation-0.1.5/README.md
+-rw-r--r--   0        0        0     2382 2024-04-12 12:46:50.936963 spine_segmentation-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      122 2024-04-11 12:53:48.914194 spine_segmentation-0.1.5/spine_segmentation/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 12:31:20.207512 spine_segmentation-0.1.5/spine_segmentation/annotators/__init__.py
+-rw-r--r--   0        0        0    16308 2024-04-11 12:53:48.934194 spine_segmentation-0.1.5/spine_segmentation/annotators/annotator_base.py
+-rw-r--r--   0        0        0     8225 2024-04-11 12:53:48.814193 spine_segmentation-0.1.5/spine_segmentation/annotators/vector_annotator.py
+-rw-r--r--   0        0        0     2190 2024-04-11 12:53:48.766192 spine_segmentation-0.1.5/spine_segmentation/cli/cli.py
+-rw-r--r--   0        0        0    12072 2024-04-10 12:31:20.207512 spine_segmentation-0.1.5/spine_segmentation/dataloader/statistics.py
+-rw-r--r--   0        0        0        0 2024-04-10 12:31:20.207512 spine_segmentation-0.1.5/spine_segmentation/datasets/__init__.py
+-rw-r--r--   0        0        0     2868 2024-04-10 12:31:20.207512 spine_segmentation-0.1.5/spine_segmentation/datasets/augmentation.py
+-rw-r--r--   0        0        0     4312 2024-04-11 12:53:48.806193 spine_segmentation-0.1.5/spine_segmentation/datasets/feature_dataset.py
+-rw-r--r--   0        0        0     6696 2024-04-11 15:53:29.418496 spine_segmentation-0.1.5/spine_segmentation/datasets/metadata_prediction_dataset.py
+-rw-r--r--   0        0        0     6372 2024-04-11 15:53:29.430496 spine_segmentation-0.1.5/spine_segmentation/datasets/patch_segmentation_dataset.py
+-rw-r--r--   0        0        0     1360 2024-04-11 15:53:29.410496 spine_segmentation-0.1.5/spine_segmentation/datasets/path_helper.py
+-rw-r--r--   0        0        0    14744 2024-04-11 15:47:48.534212 spine_segmentation-0.1.5/spine_segmentation/datasets/sample.py
+-rw-r--r--   0        0        0    14989 2024-04-11 15:53:29.422496 spine_segmentation-0.1.5/spine_segmentation/datasets/segmentation_dataset.py
+-rw-r--r--   0        0        0     2037 2024-04-11 12:53:48.782192 spine_segmentation-0.1.5/spine_segmentation/datasets/vector_table_graphs_dataset.py
+-rw-r--r--   0        0        0     2581 2024-04-11 12:53:48.890194 spine_segmentation-0.1.5/spine_segmentation/evaluate/analyze_edge_cases.py
+-rw-r--r--   0        0        0     2520 2024-04-11 12:53:48.798193 spine_segmentation-0.1.5/spine_segmentation/evaluate/analyze_index_list.py
+-rw-r--r--   0        0        0     1659 2024-04-11 12:53:48.854193 spine_segmentation-0.1.5/spine_segmentation/evaluate/classic_ml.py
+-rw-r--r--   0        0        0     1108 2024-04-10 12:31:20.207512 spine_segmentation-0.1.5/spine_segmentation/evaluate/eval_created_stats.py
+-rw-r--r--   0        0        0    15527 2024-04-11 15:52:07.339228 spine_segmentation-0.1.5/spine_segmentation/evaluate/eval_instance_seg_model.py
+-rw-r--r--   0        0        0     8215 2024-04-11 12:53:48.746192 spine_segmentation-0.1.5/spine_segmentation/evaluate/eval_splitting.py
+-rw-r--r--   0        0        0     6109 2024-04-11 15:52:07.363228 spine_segmentation-0.1.5/spine_segmentation/evaluate/load_model.py
+-rw-r--r--   0        0        0     4885 2024-04-11 12:53:48.882194 spine_segmentation-0.1.5/spine_segmentation/evaluate/metadata.py
+-rw-r--r--   0        0        0     1627 2024-04-11 12:53:48.894194 spine_segmentation-0.1.5/spine_segmentation/evaluate/volume_size_in_gt.py
+-rw-r--r--   0        0        0    10268 2024-04-12 12:46:46.364931 spine_segmentation-0.1.5/spine_segmentation/inference/instance_segmentation.py
+-rw-r--r--   0        0        0     6761 2024-04-11 12:53:48.846193 spine_segmentation-0.1.5/spine_segmentation/inference/onnx_model.py
+-rw-r--r--   0        0        0     7515 2024-04-11 12:53:48.906194 spine_segmentation-0.1.5/spine_segmentation/instance_separation/instance_separation.py
+-rw-r--r--   0        0        0      304 2024-04-10 12:31:20.207512 spine_segmentation-0.1.5/spine_segmentation/losses/diffis1.py
+-rw-r--r--   0        0        0     2080 2024-04-11 15:40:00.222464 spine_segmentation-0.1.5/spine_segmentation/model_downloader/model_downloader.py
+-rw-r--r--   0        0        0      712 2024-04-11 12:53:48.850193 spine_segmentation-0.1.5/spine_segmentation/plotting/bmi.py
+-rw-r--r--   0        0        0     8132 2024-04-11 12:53:48.778192 spine_segmentation-0.1.5/spine_segmentation/plotting/classification_correlation.py
+-rw-r--r--   0        0        0     2566 2024-04-11 12:53:48.886194 spine_segmentation-0.1.5/spine_segmentation/plotting/patient_metadata.py
+-rw-r--r--   0        0        0    10404 2024-04-11 12:53:48.826193 spine_segmentation-0.1.5/spine_segmentation/plotting/plot_slice.py
+-rw-r--r--   0        0        0     1795 2024-04-11 12:53:48.938195 spine_segmentation-0.1.5/spine_segmentation/plotting/plot_statistics.py
+-rw-r--r--   0        0        0     5823 2024-04-11 12:53:48.834193 spine_segmentation-0.1.5/spine_segmentation/plotting/read_npz_eval_per_roi_accuracy.py
+-rw-r--r--   0        0        0     5767 2024-04-11 12:53:48.786192 spine_segmentation-0.1.5/spine_segmentation/plotting/show_plane_splitting_3d.py
+-rw-r--r--   0        0        0      266 2024-04-11 12:53:48.858193 spine_segmentation-0.1.5/spine_segmentation/plotting/ydata_profile_report.py
+-rw-r--r--   0        0        0      930 2024-04-11 15:55:12.773382 spine_segmentation-0.1.5/spine_segmentation/resources/paths.py
+-rw-r--r--   0        0        0      933 2024-04-11 12:53:48.842193 spine_segmentation-0.1.5/spine_segmentation/resources/preloaded.py
+-rw-r--r--   0        0        0       63 2024-04-11 09:34:14.336647 spine_segmentation-0.1.5/spine_segmentation/run.py
+-rw-r--r--   0        0        0     4575 2024-04-10 12:31:20.207512 spine_segmentation-0.1.5/spine_segmentation/scripts/format_results.py
+-rw-r--r--   0        0        0     4546 2024-04-11 12:53:48.866193 spine_segmentation-0.1.5/spine_segmentation/scripts/split_train_val_test.py
+-rw-r--r--   0        0        0      210 2024-04-10 12:31:20.207512 spine_segmentation-0.1.5/spine_segmentation/scripts/test_patient_ids.txt
+-rw-r--r--   0        0        0      112 2024-04-10 18:52:49.798849 spine_segmentation-0.1.5/spine_segmentation/spine_types/disc.py
+-rw-r--r--   0        0        0     1033 2024-04-10 12:31:20.207512 spine_segmentation-0.1.5/spine_segmentation/spine_types/labels.py
+-rw-r--r--   0        0        0      219 2024-04-10 12:31:20.207512 spine_segmentation-0.1.5/spine_segmentation/spine_types/line_segment.py
+-rw-r--r--   0        0        0     2409 2024-04-10 12:31:20.207512 spine_segmentation-0.1.5/spine_segmentation/spine_types/plane.py
+-rw-r--r--   0        0        0       67 2024-04-10 12:31:20.207512 spine_segmentation-0.1.5/spine_segmentation/spine_types/roi.py
+-rw-r--r--   0        0        0      246 2024-04-10 12:31:20.207512 spine_segmentation-0.1.5/spine_segmentation/spine_types/spine.py
+-rw-r--r--   0        0        0      116 2024-04-10 18:52:49.974852 spine_segmentation-0.1.5/spine_segmentation/spine_types/vertebra.py
+-rw-r--r--   0        0        0     1190 2024-04-11 12:53:48.874194 spine_segmentation-0.1.5/spine_segmentation/trainer/learning_rate_finder.py
+-rw-r--r--   0        0        0        0 2024-04-10 12:31:20.207512 spine_segmentation-0.1.5/spine_segmentation/utils/__init__.py
+-rw-r--r--   0        0        0      685 2024-04-10 12:31:20.207512 spine_segmentation-0.1.5/spine_segmentation/utils/fix_validations_step_bar.py
+-rw-r--r--   0        0        0      218 2024-04-10 12:31:20.207512 spine_segmentation-0.1.5/spine_segmentation/utils/globals.py
+-rw-r--r--   0        0        0      552 2024-04-10 12:31:20.207512 spine_segmentation-0.1.5/spine_segmentation/utils/log_dir.py
+-rw-r--r--   0        0        0      690 2024-04-10 12:31:20.207512 spine_segmentation-0.1.5/spine_segmentation/utils/profiling.py
+-rw-r--r--   0        0        0      930 2024-04-10 12:31:20.207512 spine_segmentation-0.1.5/spine_segmentation/utils/proxy_class.py
+-rw-r--r--   0        0        0        0 2024-04-10 12:31:20.207512 spine_segmentation-0.1.5/spine_segmentation/visualisation/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 12:31:20.207512 spine_segmentation-0.1.5/spine_segmentation/visualisation/blender/__init__.py
+-rw-r--r--   0        0        0    11971 2024-04-10 12:31:20.207512 spine_segmentation-0.1.5/spine_segmentation/visualisation/blender/blender_script.py
+-rw-r--r--   0        0        0     9179 2024-04-11 12:53:48.830193 spine_segmentation-0.1.5/spine_segmentation/visualisation/blender/gen_obj.py
+-rw-r--r--   0        0        0     8158 2024-04-11 12:53:48.822193 spine_segmentation-0.1.5/spine_segmentation/visualisation/blender/open_in_blender.py
+-rw-r--r--   0        0        0    12036 2024-04-10 12:31:20.207512 spine_segmentation-0.1.5/spine_segmentation/visualisation/color.py
+-rw-r--r--   0        0        0     1705 2024-04-11 12:53:48.794192 spine_segmentation-0.1.5/spine_segmentation/visualisation/color_palettes.py
+-rw-r--r--   0        0        0     2602 1970-01-01 00:00:00.000000 spine_segmentation-0.1.5/PKG-INFO
```

### Comparing `spine_segmentation-0.1.4/README.md` & `spine_segmentation-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.4/pyproject.toml` & `spine_segmentation-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spine-segmentation"
-version = "0.1.4"
+version = "0.1.5"
 description = "Anatomical labeling of the spine in small field-of-view MRI scans"
 authors = [
     "Brutenis Gliwa <brutenis@gmail.com>",
 ]
 readme = "README.md"
 
 classifiers = [
```

### Comparing `spine_segmentation-0.1.4/spine_segmentation/annotators/annotator_base.py` & `spine_segmentation-0.1.5/spine_segmentation/annotators/annotator_base.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.4/spine_segmentation/annotators/vector_annotator.py` & `spine_segmentation-0.1.5/spine_segmentation/annotators/vector_annotator.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.4/spine_segmentation/cli/cli.py` & `spine_segmentation-0.1.5/spine_segmentation/cli/cli.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.4/spine_segmentation/dataloader/statistics.py` & `spine_segmentation-0.1.5/spine_segmentation/dataloader/statistics.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.4/spine_segmentation/datasets/augmentation.py` & `spine_segmentation-0.1.5/spine_segmentation/datasets/augmentation.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.4/spine_segmentation/datasets/feature_dataset.py` & `spine_segmentation-0.1.5/spine_segmentation/datasets/feature_dataset.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.4/spine_segmentation/datasets/metadata_prediction_dataset.py` & `spine_segmentation-0.1.5/spine_segmentation/datasets/metadata_prediction_dataset.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.4/spine_segmentation/datasets/patch_segmentation_dataset.py` & `spine_segmentation-0.1.5/spine_segmentation/datasets/patch_segmentation_dataset.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.4/spine_segmentation/datasets/path_helper.py` & `spine_segmentation-0.1.5/spine_segmentation/datasets/path_helper.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.4/spine_segmentation/datasets/sample.py` & `spine_segmentation-0.1.5/spine_segmentation/datasets/sample.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.4/spine_segmentation/datasets/segmentation_dataset.py` & `spine_segmentation-0.1.5/spine_segmentation/datasets/segmentation_dataset.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.4/spine_segmentation/datasets/vector_table_graphs_dataset.py` & `spine_segmentation-0.1.5/spine_segmentation/datasets/vector_table_graphs_dataset.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.4/spine_segmentation/evaluate/analyze_edge_cases.py` & `spine_segmentation-0.1.5/spine_segmentation/evaluate/analyze_edge_cases.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.4/spine_segmentation/evaluate/analyze_index_list.py` & `spine_segmentation-0.1.5/spine_segmentation/evaluate/analyze_index_list.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.4/spine_segmentation/evaluate/classic_ml.py` & `spine_segmentation-0.1.5/spine_segmentation/evaluate/classic_ml.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.4/spine_segmentation/evaluate/eval_created_stats.py` & `spine_segmentation-0.1.5/spine_segmentation/evaluate/eval_created_stats.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.4/spine_segmentation/evaluate/eval_instance_seg_model.py` & `spine_segmentation-0.1.5/spine_segmentation/evaluate/eval_instance_seg_model.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.4/spine_segmentation/evaluate/eval_splitting.py` & `spine_segmentation-0.1.5/spine_segmentation/evaluate/eval_splitting.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.4/spine_segmentation/evaluate/load_model.py` & `spine_segmentation-0.1.5/spine_segmentation/evaluate/load_model.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.4/spine_segmentation/evaluate/metadata.py` & `spine_segmentation-0.1.5/spine_segmentation/evaluate/metadata.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.4/spine_segmentation/evaluate/volume_size_in_gt.py` & `spine_segmentation-0.1.5/spine_segmentation/evaluate/volume_size_in_gt.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.4/spine_segmentation/inference/instance_segmentation.py` & `spine_segmentation-0.1.5/spine_segmentation/inference/instance_segmentation.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-import random
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Literal, Union, Dict
 
+from loguru import logger
 
 from spine_segmentation.inference.onnx_model import ONNXInferenceModel
 from spine_segmentation.instance_separation.instance_separation import (
     get_planes_from_rois,
     mask_rare_rois,
     separate_rois_with_labels,
     separate_segmented_rois_by_planes,
 )
-from spine_segmentation.resources.paths import TRAIN_SPLIT_CSV_PATH, VAL_SPLIT_CSV_PATH
-from spine_segmentation.resources.other_paths import RAW_NAKO_DATASET_PATH
 from spine_segmentation.spine_types.labels import get_labels_for_n_classes
 from spine_segmentation.utils.log_dir import get_next_log_dir
 from spine_segmentation.visualisation.blender.open_in_blender import open_in_blender
 
 import numpy as np
 
 
@@ -79,31 +77,24 @@
 
 # def find_best_matching(vertebra_instances, vertebra_segmentation):
 
 
 def post_process_instances(vertebra_instances, segmentation, plot_dir=None):
     vertebra_instances = vertebra_instances.copy()
     vertebra = segmentation == 1
-    # from matplotlib import pyplot as plt
 
-    # plt.imshow(vertebra_instances[8])
-    # plt.imshow(instance_mask[8])
-    # plt.imshow(vertebra[8])
-    # plt.imshow(split_segmentation[8])
-    # plt.show()
     vertebra_instances[~vertebra] = 0
     split_segmentation, _ = separate_rois_with_labels(segmentation)
     split_vertebra_segmentation = split_segmentation.copy()
     split_vertebra_segmentation[~vertebra] = 0
     split_vertebra_segmentation[vertebra] -= np.unique(split_vertebra_segmentation)[1] - 1
     add2 = vertebra * 2
     print(split_vertebra_segmentation.shape, np.unique(split_vertebra_segmentation))
     add2_only_s1 = (split_vertebra_segmentation == split_vertebra_segmentation.max()) * 2
 
-    # best_i = 0
     best_vertebra_instances = split_vertebra_segmentation
     best_mse = 1e9
 
     plots = [(vertebra_instances, "Inst", np.zeros_like(vertebra_instances))]
 
     for ith, add_for_s1 in enumerate([0, add2_only_s1, add2_only_s1 * 2]):
         for i in range(26):
@@ -178,152 +169,14 @@
     for stat in stats:
         if stat:
             correct_sum += stat["correct"]
             correct_no_edges_sum += stat["correct_no_edges"]
     print(f"{correct_sum=} / {len(stats)}, {correct_no_edges_sum=} / {len(stats)}")
 
 
-def plot_every_val_dataset(directory=None, device=3, model_height=896, cropped_height=None, cropped_V=None):
-    import torch
-    from spine_segmentation.datasets.sample import SampleIterator, get_random_crop_slice
-    from spine_segmentation.plotting.plot_slice import get_stats, plot_npz, single_plot
-    from spine_segmentation.datasets.segmentation_dataset import SegmentationDataModule
-    from spine_segmentation.datasets.path_helper import expand_path_to_data_dirs
-
-    if directory is None:
-        directory = get_next_log_dir()
-    directory = Path(directory)
-
-    if cropped_V is not None:
-        assert 1 <= cropped_V <= 49
-
-    if cropped_height is not None:
-        assert 50 <= cropped_V
-
-    sample_iterator = SampleIterator(
-        expand_path_to_data_dirs(RAW_NAKO_DATASET_PATH), add_adjacent_slices=True, skip_first_percent=0.9505
-    )
-
-    # index_list_path = (
-    #     Path.home() / "devel/src/git/spine_annotator/cache/onnx_inference/2023-09-12_Seg_Unet_mitb5/index_list.npz"
-    # )
-    # val_dataloader = get_dataloader("val", index_list_path, bs=1)
-
-    val_dataloader = SegmentationDataModule(
-        [TRAIN_SPLIT_CSV_PATH, VAL_SPLIT_CSV_PATH],
-        add_adjacent_slices=True,
-        batch_size=16,
-        # crop_height_to_px=416,
-        target_shape=(18, 320, 896),
-    ).val_dataloader()
-
-    stats = []
-
-    gt = None
-    # cropped_height = 50
-    random.seed(0)
-    # for i, (image, _, sample, path) in enumerate(sample_iterator):
-    # for i, (image, *_) in enumerate(sample_iterator):
-    for i, (image, gt) in enumerate(val_dataloader):
-        # if i >= 100:
-        # break
-
-        if isinstance(image, torch.Tensor):
-            image = image.cpu().detach().numpy()
-
-        if gt is None:
-            gt_npz = onnx_seg_inference.inference(image)
-        else:
-            gt_instances, id_to_label = separate_rois_with_labels(gt.numpy()[:, 0, :, :])
-            gt_npz = {"instances": gt_instances, "id_to_label": id_to_label}
-
-        gt_npz["instances"][gt_npz["instances"] == gt_npz["instances"].max()] = 49
-
-        print(gt_npz["instances"].shape)
-
-        orig_gt_nonzero = np.nonzero(np.any(gt_npz["instances"], axis=(0, 1)))[0]
-        gt_start_at = orig_gt_nonzero[0]
-        gt_end_at = orig_gt_nonzero[-1]
-        print(f"{gt_start_at=} {gt_end_at=}")
-        how_many_crops = 10
-        if cropped_height == model_height == 896:
-            how_many_crops = 1
-            gt_end_at = gt_start_at = 0
-
-        # for start_at in np.linspace(gt_start_at, gt_end_at - cropped_height, how_many_crops):
-        for start_at_class in range(1, 49 - cropped_V + 2, 2):  # +2 so that 49 is inclusive
-            end_at_class = start_at_class + cropped_V - 1
-            try:
-                print(f"\n\n============ Processing sample {i}: {start_at_class}-{end_at_class} =============\n")
-                print(gt_npz["instances"].shape)
-                relevant_classes = np.any(
-                    (gt_npz["instances"] >= start_at_class) & (gt_npz["instances"] <= end_at_class), axis=(0, 1)
-                )
-                print(f"{relevant_classes.shape=}")
-                nonzero_relevant_classes = np.nonzero(relevant_classes)[0]
-                start_at = nonzero_relevant_classes[0]
-                end_at = nonzero_relevant_classes[-1]
-                cropped_height = end_at - start_at
-                print(f"{start_at=} {end_at=} {cropped_height=}")
-
-                image = np.array(image)
-                print(image.shape)
-
-                crop_slice = get_random_crop_slice(cropped_height, image.shape[3], start_at=round(start_at))
-
-                curr_dir = directory / f"sample_{i:03}_{crop_slice.start:03}-{crop_slice.stop:03}"
-                curr_dir.mkdir(parents=True, exist_ok=True)
-
-                # ==================
-                # Create ground truth segmentation
-                # ==================
-
-                cropped_instance_gt = gt_npz["instances"][:, None, :, crop_slice].copy(order="C")
-
-                # ==================
-                # Create cropped input image for segmentation model (which will be used as input for instance segmentation)
-                # ==================
-
-                cropped_seg_input = image[:, :, :, crop_slice].copy(order="C")
-                new_npz = instance_segmentation_for_image(
-                    crop_slice,
-                    cropped_height,
-                    cropped_instance_gt,
-                    cropped_seg_input,
-                    curr_dir,
-                    directory,
-                    gt_npz,
-                    image,
-                    model_height,
-                    onnx_inst_inference,
-                    onnx_seg_inference,
-                    stats,
-                )
-                stats.append(get_stats(new_npz["instances_post_processed"], new_npz["gt_instances"]))
-                np.savez_compressed(directory / "stats.npz", stats=stats)
-                open_npz_in_blender(new_npz)
-                plot_npz(new_npz, curr_dir / "plot.png", slices=range(7, 10), stats=stats[-1])
-                print_stats_summary(stats)
-                # if i > 50:
-                #    break
-                # exit(0)
-            except KeyboardInterrupt:
-                raise
-            except:
-                print(f"Error processing sample {i}")
-                stats.append({})
-                import traceback
-
-                traceback.print_exc()
-                continue
-
-    # open_npz_and_plot_rois(new_npz, curr_dir / "plot.png")
-    # open_npz_in_blender_separate_rois(npz, curr_dir / "render.png")
-
-
 @dataclass
 class SegmentationResult:
     semantic_segmentation: np.ndarray
     instance_segmentation: np.ndarray
     id_to_label: Dict[int, str]
 
 
@@ -331,61 +184,61 @@
 
 DeviceType = Union[Literal["CPU", "GPU"], int]
 
 
 class SegmentationInference:
 
     def __init__(self, segmentation_device: DeviceType = "CPU", instance_segmentation_device: DeviceType = "CPU"):
-        self.model_height = MODEL_HEIGHT
-        self.onnx_seg_inference = ONNXInferenceModel.get_best_segmentation_model(device=segmentation_device)
-        self.onnx_inst_inference = ONNXInferenceModel.get_best_instance_segmentation_model(
+        self._model_height = MODEL_HEIGHT
+        self._onnx_seg_inference = ONNXInferenceModel.get_best_segmentation_model(device=segmentation_device)
+        self._onnx_inst_inference = ONNXInferenceModel.get_best_instance_segmentation_model(
             device=instance_segmentation_device
         )
 
     def segment(
         self,
-        input_image,
-        curr_dir=None,
+        mri_3d_numpy_image: np.ndarray,
+        *,
+        batch_size: int,
+        cache_dir: Union[Literal["auto"], None, Path, str] = "auto",
     ):
-        padding_to_896 = ((0, 0), (0, 0), (0, 0), (0, input_image.shape[3] - MODEL_HEIGHT))
-        cropped_padded_seg_input = np.pad(input_image, padding_to_896, mode="constant")
-        seg_npz = self.onnx_seg_inference.inference(cropped_padded_seg_input)
+        if len(mri_3d_numpy_image.shape) < 3:
+            logger.error(
+                f"mri_3d_numpy_image must be 3 dimensional. Got {mri_3d_numpy_image.shape}. If you "
+                f"wish to segment only a 2D slice, consider repeating the slice three times in the "
+                f"first dimension, resulting in this shape: {(3, *mri_3d_numpy_image.shape)}:"
+                "\n\n\tnp.tile(input_image, (3, 1, 1))\n"
+            )
+            exit(1)
+        if len(mri_3d_numpy_image.shape) > 3:
+            logger.error(f"mri_3d_numpy_image must be 3 dimensional. Got {mri_3d_numpy_image.shape}. "
+                         f"Consider dropping the batch-dimension and just using the 3D mri image as entire input.")
+
+        padding_to_896 = ((0, 0), (0, 0), (0, 0), (0, mri_3d_numpy_image.shape[3] - MODEL_HEIGHT))
+        cropped_padded_seg_input = np.pad(mri_3d_numpy_image, padding_to_896, mode="constant")
+        seg_npz = self._onnx_seg_inference.inference(cropped_padded_seg_input)
         inst_seg_input = seg_npz["segmentation"][:, None, :, :]
         cropped_inst_seg_input = inst_seg_input[:, :, :, :MODEL_HEIGHT]
         padding_to_416 = ((0, 0), (0, 0), (0, 0), (0, MODEL_HEIGHT - MODEL_HEIGHT))
         cropped_input_image_with_gt = np.concatenate(
             [
-                np.pad(input_image[:, 1:2, :, :], padding_to_416, mode="constant"),
+                np.pad(mri_3d_numpy_image[:, 1:2, :, :], padding_to_416, mode="constant"),
                 (cropped_inst_seg_input == 1),
                 (cropped_inst_seg_input == 2),
             ],
             axis=1,
         )
         cropped_input_image_with_gt = cropped_input_image_with_gt.astype(np.float32)
-        cropped_input_image_without_gt = np.pad(input_image[:, :, :, :], padding_to_416, mode="constant").astype(
+        cropped_input_image_without_gt = np.pad(mri_3d_numpy_image[:, :, :, :], padding_to_416, mode="constant").astype(
             np.float32
         )
 
-        new_npz = self.onnx_inst_inference.inference(cropped_input_image_without_gt)
+        new_npz = self._onnx_inst_inference.inference(cropped_input_image_without_gt)
         new_npz["instances"] = new_npz["instances"] * 2 - (new_npz["instances"] != 0)
         # new_npz["id_to_label"] = gt_npz["id_to_label"]
         # new_npz["gt_id_to_label"] = gt_npz["id_to_label"]
         new_npz["instances_post_processed"] = post_process_instances(
-            new_npz["instances"], cropped_inst_seg_input[:, 0, :, :], plot_dir=curr_dir
+            new_npz["instances"], cropped_inst_seg_input[:, 0, :, :], plot_dir=cache_dir
         )
         new_npz["cropped_segmentation"] = cropped_inst_seg_input[:, 0, :, :]
         id_to_labels = get_labels_for_n_classes(49)
         return SegmentationResult(inst_seg_input, new_npz["instances_post_processed"], id_to_labels)
-
-
-def main():
-    # Get first argument as int
-    import sys
-
-    slice_height = int(sys.argv[1]) if len(sys.argv) > 1 else 49
-    gpu = int(sys.argv[2]) if len(sys.argv) > 2 else "CPU"
-    # plot_every_val_dataset(cropped_height=slice_height, device=gpu)
-    plot_every_val_dataset(cropped_V=slice_height, device=gpu)
-
-
-if __name__ == "__main__":
-    main()
```

### Comparing `spine_segmentation-0.1.4/spine_segmentation/inference/onnx_model.py` & `spine_segmentation-0.1.5/spine_segmentation/inference/onnx_model.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.4/spine_segmentation/instance_separation/instance_separation.py` & `spine_segmentation-0.1.5/spine_segmentation/instance_separation/instance_separation.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.4/spine_segmentation/model_downloader/model_downloader.py` & `spine_segmentation-0.1.5/spine_segmentation/model_downloader/model_downloader.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.4/spine_segmentation/plotting/bmi.py` & `spine_segmentation-0.1.5/spine_segmentation/plotting/bmi.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.4/spine_segmentation/plotting/classification_correlation.py` & `spine_segmentation-0.1.5/spine_segmentation/plotting/classification_correlation.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.4/spine_segmentation/plotting/patient_metadata.py` & `spine_segmentation-0.1.5/spine_segmentation/plotting/patient_metadata.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.4/spine_segmentation/plotting/plot_slice.py` & `spine_segmentation-0.1.5/spine_segmentation/plotting/plot_slice.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.4/spine_segmentation/plotting/plot_statistics.py` & `spine_segmentation-0.1.5/spine_segmentation/plotting/plot_statistics.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.4/spine_segmentation/plotting/read_npz_eval_per_roi_accuracy.py` & `spine_segmentation-0.1.5/spine_segmentation/plotting/read_npz_eval_per_roi_accuracy.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.4/spine_segmentation/plotting/show_plane_splitting_3d.py` & `spine_segmentation-0.1.5/spine_segmentation/plotting/show_plane_splitting_3d.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.4/spine_segmentation/resources/paths.py` & `spine_segmentation-0.1.5/spine_segmentation/resources/paths.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.4/spine_segmentation/resources/preloaded.py` & `spine_segmentation-0.1.5/spine_segmentation/resources/preloaded.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.4/spine_segmentation/scripts/format_results.py` & `spine_segmentation-0.1.5/spine_segmentation/scripts/format_results.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.4/spine_segmentation/scripts/split_train_val_test.py` & `spine_segmentation-0.1.5/spine_segmentation/scripts/split_train_val_test.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.4/spine_segmentation/spine_types/labels.py` & `spine_segmentation-0.1.5/spine_segmentation/spine_types/labels.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.4/spine_segmentation/spine_types/plane.py` & `spine_segmentation-0.1.5/spine_segmentation/spine_types/plane.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.4/spine_segmentation/trainer/learning_rate_finder.py` & `spine_segmentation-0.1.5/spine_segmentation/trainer/learning_rate_finder.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.4/spine_segmentation/utils/fix_validations_step_bar.py` & `spine_segmentation-0.1.5/spine_segmentation/utils/fix_validations_step_bar.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.4/spine_segmentation/utils/log_dir.py` & `spine_segmentation-0.1.5/spine_segmentation/utils/log_dir.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.4/spine_segmentation/utils/profiling.py` & `spine_segmentation-0.1.5/spine_segmentation/utils/profiling.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.4/spine_segmentation/utils/proxy_class.py` & `spine_segmentation-0.1.5/spine_segmentation/utils/proxy_class.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.4/spine_segmentation/visualisation/blender/blender_script.py` & `spine_segmentation-0.1.5/spine_segmentation/visualisation/blender/blender_script.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.4/spine_segmentation/visualisation/blender/gen_obj.py` & `spine_segmentation-0.1.5/spine_segmentation/visualisation/blender/gen_obj.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.4/spine_segmentation/visualisation/blender/open_in_blender.py` & `spine_segmentation-0.1.5/spine_segmentation/visualisation/blender/open_in_blender.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.4/spine_segmentation/visualisation/color.py` & `spine_segmentation-0.1.5/spine_segmentation/visualisation/color.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.4/spine_segmentation/visualisation/color_palettes.py` & `spine_segmentation-0.1.5/spine_segmentation/visualisation/color_palettes.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.4/PKG-INFO` & `spine_segmentation-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spine-segmentation
-Version: 0.1.4
+Version: 0.1.5
 Summary: Anatomical labeling of the spine in small field-of-view MRI scans
 Author: Brutenis Gliwa
 Author-email: brutenis@gmail.com
 Requires-Python: >=3.8.1,<3.13.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

