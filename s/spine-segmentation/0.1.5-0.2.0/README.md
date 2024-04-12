# Comparing `tmp/spine_segmentation-0.1.5.tar.gz` & `tmp/spine_segmentation-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spine_segmentation-0.1.5.tar", max compression
+gzip compressed data, was "spine_segmentation-0.2.0.tar", max compression
```

## Comparing `spine_segmentation-0.1.5.tar` & `spine_segmentation-0.2.0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0     1211 2024-04-11 11:32:29.446351 spine_segmentation-0.1.5/README.md
--rw-r--r--   0        0        0     2382 2024-04-12 12:46:50.936963 spine_segmentation-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      122 2024-04-11 12:53:48.914194 spine_segmentation-0.1.5/spine_segmentation/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 12:31:20.207512 spine_segmentation-0.1.5/spine_segmentation/annotators/__init__.py
--rw-r--r--   0        0        0    16308 2024-04-11 12:53:48.934194 spine_segmentation-0.1.5/spine_segmentation/annotators/annotator_base.py
--rw-r--r--   0        0        0     8225 2024-04-11 12:53:48.814193 spine_segmentation-0.1.5/spine_segmentation/annotators/vector_annotator.py
--rw-r--r--   0        0        0     2190 2024-04-11 12:53:48.766192 spine_segmentation-0.1.5/spine_segmentation/cli/cli.py
--rw-r--r--   0        0        0    12072 2024-04-10 12:31:20.207512 spine_segmentation-0.1.5/spine_segmentation/dataloader/statistics.py
--rw-r--r--   0        0        0        0 2024-04-10 12:31:20.207512 spine_segmentation-0.1.5/spine_segmentation/datasets/__init__.py
--rw-r--r--   0        0        0     2868 2024-04-10 12:31:20.207512 spine_segmentation-0.1.5/spine_segmentation/datasets/augmentation.py
--rw-r--r--   0        0        0     4312 2024-04-11 12:53:48.806193 spine_segmentation-0.1.5/spine_segmentation/datasets/feature_dataset.py
--rw-r--r--   0        0        0     6696 2024-04-11 15:53:29.418496 spine_segmentation-0.1.5/spine_segmentation/datasets/metadata_prediction_dataset.py
--rw-r--r--   0        0        0     6372 2024-04-11 15:53:29.430496 spine_segmentation-0.1.5/spine_segmentation/datasets/patch_segmentation_dataset.py
--rw-r--r--   0        0        0     1360 2024-04-11 15:53:29.410496 spine_segmentation-0.1.5/spine_segmentation/datasets/path_helper.py
--rw-r--r--   0        0        0    14744 2024-04-11 15:47:48.534212 spine_segmentation-0.1.5/spine_segmentation/datasets/sample.py
--rw-r--r--   0        0        0    14989 2024-04-11 15:53:29.422496 spine_segmentation-0.1.5/spine_segmentation/datasets/segmentation_dataset.py
--rw-r--r--   0        0        0     2037 2024-04-11 12:53:48.782192 spine_segmentation-0.1.5/spine_segmentation/datasets/vector_table_graphs_dataset.py
--rw-r--r--   0        0        0     2581 2024-04-11 12:53:48.890194 spine_segmentation-0.1.5/spine_segmentation/evaluate/analyze_edge_cases.py
--rw-r--r--   0        0        0     2520 2024-04-11 12:53:48.798193 spine_segmentation-0.1.5/spine_segmentation/evaluate/analyze_index_list.py
--rw-r--r--   0        0        0     1659 2024-04-11 12:53:48.854193 spine_segmentation-0.1.5/spine_segmentation/evaluate/classic_ml.py
--rw-r--r--   0        0        0     1108 2024-04-10 12:31:20.207512 spine_segmentation-0.1.5/spine_segmentation/evaluate/eval_created_stats.py
--rw-r--r--   0        0        0    15527 2024-04-11 15:52:07.339228 spine_segmentation-0.1.5/spine_segmentation/evaluate/eval_instance_seg_model.py
--rw-r--r--   0        0        0     8215 2024-04-11 12:53:48.746192 spine_segmentation-0.1.5/spine_segmentation/evaluate/eval_splitting.py
--rw-r--r--   0        0        0     6109 2024-04-11 15:52:07.363228 spine_segmentation-0.1.5/spine_segmentation/evaluate/load_model.py
--rw-r--r--   0        0        0     4885 2024-04-11 12:53:48.882194 spine_segmentation-0.1.5/spine_segmentation/evaluate/metadata.py
--rw-r--r--   0        0        0     1627 2024-04-11 12:53:48.894194 spine_segmentation-0.1.5/spine_segmentation/evaluate/volume_size_in_gt.py
--rw-r--r--   0        0        0    10268 2024-04-12 12:46:46.364931 spine_segmentation-0.1.5/spine_segmentation/inference/instance_segmentation.py
--rw-r--r--   0        0        0     6761 2024-04-11 12:53:48.846193 spine_segmentation-0.1.5/spine_segmentation/inference/onnx_model.py
--rw-r--r--   0        0        0     7515 2024-04-11 12:53:48.906194 spine_segmentation-0.1.5/spine_segmentation/instance_separation/instance_separation.py
--rw-r--r--   0        0        0      304 2024-04-10 12:31:20.207512 spine_segmentation-0.1.5/spine_segmentation/losses/diffis1.py
--rw-r--r--   0        0        0     2080 2024-04-11 15:40:00.222464 spine_segmentation-0.1.5/spine_segmentation/model_downloader/model_downloader.py
--rw-r--r--   0        0        0      712 2024-04-11 12:53:48.850193 spine_segmentation-0.1.5/spine_segmentation/plotting/bmi.py
--rw-r--r--   0        0        0     8132 2024-04-11 12:53:48.778192 spine_segmentation-0.1.5/spine_segmentation/plotting/classification_correlation.py
--rw-r--r--   0        0        0     2566 2024-04-11 12:53:48.886194 spine_segmentation-0.1.5/spine_segmentation/plotting/patient_metadata.py
--rw-r--r--   0        0        0    10404 2024-04-11 12:53:48.826193 spine_segmentation-0.1.5/spine_segmentation/plotting/plot_slice.py
--rw-r--r--   0        0        0     1795 2024-04-11 12:53:48.938195 spine_segmentation-0.1.5/spine_segmentation/plotting/plot_statistics.py
--rw-r--r--   0        0        0     5823 2024-04-11 12:53:48.834193 spine_segmentation-0.1.5/spine_segmentation/plotting/read_npz_eval_per_roi_accuracy.py
--rw-r--r--   0        0        0     5767 2024-04-11 12:53:48.786192 spine_segmentation-0.1.5/spine_segmentation/plotting/show_plane_splitting_3d.py
--rw-r--r--   0        0        0      266 2024-04-11 12:53:48.858193 spine_segmentation-0.1.5/spine_segmentation/plotting/ydata_profile_report.py
--rw-r--r--   0        0        0      930 2024-04-11 15:55:12.773382 spine_segmentation-0.1.5/spine_segmentation/resources/paths.py
--rw-r--r--   0        0        0      933 2024-04-11 12:53:48.842193 spine_segmentation-0.1.5/spine_segmentation/resources/preloaded.py
--rw-r--r--   0        0        0       63 2024-04-11 09:34:14.336647 spine_segmentation-0.1.5/spine_segmentation/run.py
--rw-r--r--   0        0        0     4575 2024-04-10 12:31:20.207512 spine_segmentation-0.1.5/spine_segmentation/scripts/format_results.py
--rw-r--r--   0        0        0     4546 2024-04-11 12:53:48.866193 spine_segmentation-0.1.5/spine_segmentation/scripts/split_train_val_test.py
--rw-r--r--   0        0        0      210 2024-04-10 12:31:20.207512 spine_segmentation-0.1.5/spine_segmentation/scripts/test_patient_ids.txt
--rw-r--r--   0        0        0      112 2024-04-10 18:52:49.798849 spine_segmentation-0.1.5/spine_segmentation/spine_types/disc.py
--rw-r--r--   0        0        0     1033 2024-04-10 12:31:20.207512 spine_segmentation-0.1.5/spine_segmentation/spine_types/labels.py
--rw-r--r--   0        0        0      219 2024-04-10 12:31:20.207512 spine_segmentation-0.1.5/spine_segmentation/spine_types/line_segment.py
--rw-r--r--   0        0        0     2409 2024-04-10 12:31:20.207512 spine_segmentation-0.1.5/spine_segmentation/spine_types/plane.py
--rw-r--r--   0        0        0       67 2024-04-10 12:31:20.207512 spine_segmentation-0.1.5/spine_segmentation/spine_types/roi.py
--rw-r--r--   0        0        0      246 2024-04-10 12:31:20.207512 spine_segmentation-0.1.5/spine_segmentation/spine_types/spine.py
--rw-r--r--   0        0        0      116 2024-04-10 18:52:49.974852 spine_segmentation-0.1.5/spine_segmentation/spine_types/vertebra.py
--rw-r--r--   0        0        0     1190 2024-04-11 12:53:48.874194 spine_segmentation-0.1.5/spine_segmentation/trainer/learning_rate_finder.py
--rw-r--r--   0        0        0        0 2024-04-10 12:31:20.207512 spine_segmentation-0.1.5/spine_segmentation/utils/__init__.py
--rw-r--r--   0        0        0      685 2024-04-10 12:31:20.207512 spine_segmentation-0.1.5/spine_segmentation/utils/fix_validations_step_bar.py
--rw-r--r--   0        0        0      218 2024-04-10 12:31:20.207512 spine_segmentation-0.1.5/spine_segmentation/utils/globals.py
--rw-r--r--   0        0        0      552 2024-04-10 12:31:20.207512 spine_segmentation-0.1.5/spine_segmentation/utils/log_dir.py
--rw-r--r--   0        0        0      690 2024-04-10 12:31:20.207512 spine_segmentation-0.1.5/spine_segmentation/utils/profiling.py
--rw-r--r--   0        0        0      930 2024-04-10 12:31:20.207512 spine_segmentation-0.1.5/spine_segmentation/utils/proxy_class.py
--rw-r--r--   0        0        0        0 2024-04-10 12:31:20.207512 spine_segmentation-0.1.5/spine_segmentation/visualisation/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 12:31:20.207512 spine_segmentation-0.1.5/spine_segmentation/visualisation/blender/__init__.py
--rw-r--r--   0        0        0    11971 2024-04-10 12:31:20.207512 spine_segmentation-0.1.5/spine_segmentation/visualisation/blender/blender_script.py
--rw-r--r--   0        0        0     9179 2024-04-11 12:53:48.830193 spine_segmentation-0.1.5/spine_segmentation/visualisation/blender/gen_obj.py
--rw-r--r--   0        0        0     8158 2024-04-11 12:53:48.822193 spine_segmentation-0.1.5/spine_segmentation/visualisation/blender/open_in_blender.py
--rw-r--r--   0        0        0    12036 2024-04-10 12:31:20.207512 spine_segmentation-0.1.5/spine_segmentation/visualisation/color.py
--rw-r--r--   0        0        0     1705 2024-04-11 12:53:48.794192 spine_segmentation-0.1.5/spine_segmentation/visualisation/color_palettes.py
--rw-r--r--   0        0        0     2602 1970-01-01 00:00:00.000000 spine_segmentation-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-04-11 11:32:29.446351 spine_segmentation-0.2.0/README.md
+-rw-r--r--   0        0        0     2382 2024-04-12 17:14:05.652289 spine_segmentation-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      122 2024-04-11 12:53:48.914194 spine_segmentation-0.2.0/spine_segmentation/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 12:31:20.207512 spine_segmentation-0.2.0/spine_segmentation/annotators/__init__.py
+-rw-r--r--   0        0        0    16308 2024-04-11 12:53:48.934194 spine_segmentation-0.2.0/spine_segmentation/annotators/annotator_base.py
+-rw-r--r--   0        0        0     8225 2024-04-11 12:53:48.814193 spine_segmentation-0.2.0/spine_segmentation/annotators/vector_annotator.py
+-rw-r--r--   0        0        0     2190 2024-04-11 12:53:48.766192 spine_segmentation-0.2.0/spine_segmentation/cli/cli.py
+-rw-r--r--   0        0        0    12072 2024-04-10 12:31:20.207512 spine_segmentation-0.2.0/spine_segmentation/dataloader/statistics.py
+-rw-r--r--   0        0        0        0 2024-04-10 12:31:20.207512 spine_segmentation-0.2.0/spine_segmentation/datasets/__init__.py
+-rw-r--r--   0        0        0     2868 2024-04-10 12:31:20.207512 spine_segmentation-0.2.0/spine_segmentation/datasets/augmentation.py
+-rw-r--r--   0        0        0     4312 2024-04-11 12:53:48.806193 spine_segmentation-0.2.0/spine_segmentation/datasets/feature_dataset.py
+-rw-r--r--   0        0        0     6696 2024-04-11 15:53:29.418496 spine_segmentation-0.2.0/spine_segmentation/datasets/metadata_prediction_dataset.py
+-rw-r--r--   0        0        0     6372 2024-04-11 15:53:29.430496 spine_segmentation-0.2.0/spine_segmentation/datasets/patch_segmentation_dataset.py
+-rw-r--r--   0        0        0     1360 2024-04-11 15:53:29.410496 spine_segmentation-0.2.0/spine_segmentation/datasets/path_helper.py
+-rw-r--r--   0        0        0    14744 2024-04-11 15:47:48.534212 spine_segmentation-0.2.0/spine_segmentation/datasets/sample.py
+-rw-r--r--   0        0        0    14989 2024-04-11 15:53:29.422496 spine_segmentation-0.2.0/spine_segmentation/datasets/segmentation_dataset.py
+-rw-r--r--   0        0        0     2037 2024-04-11 12:53:48.782192 spine_segmentation-0.2.0/spine_segmentation/datasets/vector_table_graphs_dataset.py
+-rw-r--r--   0        0        0     2581 2024-04-11 12:53:48.890194 spine_segmentation-0.2.0/spine_segmentation/evaluate/analyze_edge_cases.py
+-rw-r--r--   0        0        0     2520 2024-04-11 12:53:48.798193 spine_segmentation-0.2.0/spine_segmentation/evaluate/analyze_index_list.py
+-rw-r--r--   0        0        0     1659 2024-04-11 12:53:48.854193 spine_segmentation-0.2.0/spine_segmentation/evaluate/classic_ml.py
+-rw-r--r--   0        0        0     1108 2024-04-10 12:31:20.207512 spine_segmentation-0.2.0/spine_segmentation/evaluate/eval_created_stats.py
+-rw-r--r--   0        0        0    15527 2024-04-11 15:52:07.339228 spine_segmentation-0.2.0/spine_segmentation/evaluate/eval_instance_seg_model.py
+-rw-r--r--   0        0        0     8215 2024-04-11 12:53:48.746192 spine_segmentation-0.2.0/spine_segmentation/evaluate/eval_splitting.py
+-rw-r--r--   0        0        0     6109 2024-04-11 15:52:07.363228 spine_segmentation-0.2.0/spine_segmentation/evaluate/load_model.py
+-rw-r--r--   0        0        0     4885 2024-04-11 12:53:48.882194 spine_segmentation-0.2.0/spine_segmentation/evaluate/metadata.py
+-rw-r--r--   0        0        0     1627 2024-04-11 12:53:48.894194 spine_segmentation-0.2.0/spine_segmentation/evaluate/volume_size_in_gt.py
+-rw-r--r--   0        0        0     9412 2024-04-12 17:12:56.059085 spine_segmentation-0.2.0/spine_segmentation/inference/instance_segmentation.py
+-rw-r--r--   0        0        0     6761 2024-04-11 12:53:48.846193 spine_segmentation-0.2.0/spine_segmentation/inference/onnx_model.py
+-rw-r--r--   0        0        0     7515 2024-04-11 12:53:48.906194 spine_segmentation-0.2.0/spine_segmentation/instance_separation/instance_separation.py
+-rw-r--r--   0        0        0      304 2024-04-10 12:31:20.207512 spine_segmentation-0.2.0/spine_segmentation/losses/diffis1.py
+-rw-r--r--   0        0        0     2080 2024-04-11 15:40:00.222464 spine_segmentation-0.2.0/spine_segmentation/model_downloader/model_downloader.py
+-rw-r--r--   0        0        0      712 2024-04-11 12:53:48.850193 spine_segmentation-0.2.0/spine_segmentation/plotting/bmi.py
+-rw-r--r--   0        0        0     8132 2024-04-11 12:53:48.778192 spine_segmentation-0.2.0/spine_segmentation/plotting/classification_correlation.py
+-rw-r--r--   0        0        0     2566 2024-04-11 12:53:48.886194 spine_segmentation-0.2.0/spine_segmentation/plotting/patient_metadata.py
+-rw-r--r--   0        0        0    10404 2024-04-11 12:53:48.826193 spine_segmentation-0.2.0/spine_segmentation/plotting/plot_slice.py
+-rw-r--r--   0        0        0     1795 2024-04-11 12:53:48.938195 spine_segmentation-0.2.0/spine_segmentation/plotting/plot_statistics.py
+-rw-r--r--   0        0        0     5823 2024-04-11 12:53:48.834193 spine_segmentation-0.2.0/spine_segmentation/plotting/read_npz_eval_per_roi_accuracy.py
+-rw-r--r--   0        0        0     5767 2024-04-11 12:53:48.786192 spine_segmentation-0.2.0/spine_segmentation/plotting/show_plane_splitting_3d.py
+-rw-r--r--   0        0        0      266 2024-04-11 12:53:48.858193 spine_segmentation-0.2.0/spine_segmentation/plotting/ydata_profile_report.py
+-rw-r--r--   0        0        0      930 2024-04-11 15:55:12.773382 spine_segmentation-0.2.0/spine_segmentation/resources/paths.py
+-rw-r--r--   0        0        0      933 2024-04-11 12:53:48.842193 spine_segmentation-0.2.0/spine_segmentation/resources/preloaded.py
+-rw-r--r--   0        0        0       63 2024-04-11 09:34:14.336647 spine_segmentation-0.2.0/spine_segmentation/run.py
+-rw-r--r--   0        0        0     4575 2024-04-10 12:31:20.207512 spine_segmentation-0.2.0/spine_segmentation/scripts/format_results.py
+-rw-r--r--   0        0        0     4546 2024-04-11 12:53:48.866193 spine_segmentation-0.2.0/spine_segmentation/scripts/split_train_val_test.py
+-rw-r--r--   0        0        0      210 2024-04-10 12:31:20.207512 spine_segmentation-0.2.0/spine_segmentation/scripts/test_patient_ids.txt
+-rw-r--r--   0        0        0      112 2024-04-10 18:52:49.798849 spine_segmentation-0.2.0/spine_segmentation/spine_types/disc.py
+-rw-r--r--   0        0        0     1033 2024-04-10 12:31:20.207512 spine_segmentation-0.2.0/spine_segmentation/spine_types/labels.py
+-rw-r--r--   0        0        0      219 2024-04-10 12:31:20.207512 spine_segmentation-0.2.0/spine_segmentation/spine_types/line_segment.py
+-rw-r--r--   0        0        0     2409 2024-04-10 12:31:20.207512 spine_segmentation-0.2.0/spine_segmentation/spine_types/plane.py
+-rw-r--r--   0        0        0       67 2024-04-10 12:31:20.207512 spine_segmentation-0.2.0/spine_segmentation/spine_types/roi.py
+-rw-r--r--   0        0        0      246 2024-04-10 12:31:20.207512 spine_segmentation-0.2.0/spine_segmentation/spine_types/spine.py
+-rw-r--r--   0        0        0      116 2024-04-10 18:52:49.974852 spine_segmentation-0.2.0/spine_segmentation/spine_types/vertebra.py
+-rw-r--r--   0        0        0     1190 2024-04-11 12:53:48.874194 spine_segmentation-0.2.0/spine_segmentation/trainer/learning_rate_finder.py
+-rw-r--r--   0        0        0        0 2024-04-10 12:31:20.207512 spine_segmentation-0.2.0/spine_segmentation/utils/__init__.py
+-rw-r--r--   0        0        0      685 2024-04-10 12:31:20.207512 spine_segmentation-0.2.0/spine_segmentation/utils/fix_validations_step_bar.py
+-rw-r--r--   0        0        0      218 2024-04-10 12:31:20.207512 spine_segmentation-0.2.0/spine_segmentation/utils/globals.py
+-rw-r--r--   0        0        0      552 2024-04-10 12:31:20.207512 spine_segmentation-0.2.0/spine_segmentation/utils/log_dir.py
+-rw-r--r--   0        0        0      690 2024-04-10 12:31:20.207512 spine_segmentation-0.2.0/spine_segmentation/utils/profiling.py
+-rw-r--r--   0        0        0      930 2024-04-10 12:31:20.207512 spine_segmentation-0.2.0/spine_segmentation/utils/proxy_class.py
+-rw-r--r--   0        0        0        0 2024-04-10 12:31:20.207512 spine_segmentation-0.2.0/spine_segmentation/visualisation/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 12:31:20.207512 spine_segmentation-0.2.0/spine_segmentation/visualisation/blender/__init__.py
+-rw-r--r--   0        0        0    11971 2024-04-10 12:31:20.207512 spine_segmentation-0.2.0/spine_segmentation/visualisation/blender/blender_script.py
+-rw-r--r--   0        0        0     9179 2024-04-11 12:53:48.830193 spine_segmentation-0.2.0/spine_segmentation/visualisation/blender/gen_obj.py
+-rw-r--r--   0        0        0     8158 2024-04-11 12:53:48.822193 spine_segmentation-0.2.0/spine_segmentation/visualisation/blender/open_in_blender.py
+-rw-r--r--   0        0        0    12036 2024-04-10 12:31:20.207512 spine_segmentation-0.2.0/spine_segmentation/visualisation/color.py
+-rw-r--r--   0        0        0     1705 2024-04-11 12:53:48.794192 spine_segmentation-0.2.0/spine_segmentation/visualisation/color_palettes.py
+-rw-r--r--   0        0        0     2602 1970-01-01 00:00:00.000000 spine_segmentation-0.2.0/PKG-INFO
```

### Comparing `spine_segmentation-0.1.5/README.md` & `spine_segmentation-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.5/pyproject.toml` & `spine_segmentation-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spine-segmentation"
-version = "0.1.5"
+version = "0.2.0"
 description = "Anatomical labeling of the spine in small field-of-view MRI scans"
 authors = [
     "Brutenis Gliwa <brutenis@gmail.com>",
 ]
 readme = "README.md"
 
 classifiers = [
```

### Comparing `spine_segmentation-0.1.5/spine_segmentation/annotators/annotator_base.py` & `spine_segmentation-0.2.0/spine_segmentation/annotators/annotator_base.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.5/spine_segmentation/annotators/vector_annotator.py` & `spine_segmentation-0.2.0/spine_segmentation/annotators/vector_annotator.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.5/spine_segmentation/cli/cli.py` & `spine_segmentation-0.2.0/spine_segmentation/cli/cli.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.5/spine_segmentation/dataloader/statistics.py` & `spine_segmentation-0.2.0/spine_segmentation/dataloader/statistics.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.5/spine_segmentation/datasets/augmentation.py` & `spine_segmentation-0.2.0/spine_segmentation/datasets/augmentation.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.5/spine_segmentation/datasets/feature_dataset.py` & `spine_segmentation-0.2.0/spine_segmentation/datasets/feature_dataset.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.5/spine_segmentation/datasets/metadata_prediction_dataset.py` & `spine_segmentation-0.2.0/spine_segmentation/datasets/metadata_prediction_dataset.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.5/spine_segmentation/datasets/patch_segmentation_dataset.py` & `spine_segmentation-0.2.0/spine_segmentation/datasets/patch_segmentation_dataset.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.5/spine_segmentation/datasets/path_helper.py` & `spine_segmentation-0.2.0/spine_segmentation/datasets/path_helper.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.5/spine_segmentation/datasets/sample.py` & `spine_segmentation-0.2.0/spine_segmentation/datasets/sample.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.5/spine_segmentation/datasets/segmentation_dataset.py` & `spine_segmentation-0.2.0/spine_segmentation/datasets/segmentation_dataset.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.5/spine_segmentation/datasets/vector_table_graphs_dataset.py` & `spine_segmentation-0.2.0/spine_segmentation/datasets/vector_table_graphs_dataset.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.5/spine_segmentation/evaluate/analyze_edge_cases.py` & `spine_segmentation-0.2.0/spine_segmentation/evaluate/analyze_edge_cases.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.5/spine_segmentation/evaluate/analyze_index_list.py` & `spine_segmentation-0.2.0/spine_segmentation/evaluate/analyze_index_list.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.5/spine_segmentation/evaluate/classic_ml.py` & `spine_segmentation-0.2.0/spine_segmentation/evaluate/classic_ml.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.5/spine_segmentation/evaluate/eval_created_stats.py` & `spine_segmentation-0.2.0/spine_segmentation/evaluate/eval_created_stats.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.5/spine_segmentation/evaluate/eval_instance_seg_model.py` & `spine_segmentation-0.2.0/spine_segmentation/evaluate/eval_instance_seg_model.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.5/spine_segmentation/evaluate/eval_splitting.py` & `spine_segmentation-0.2.0/spine_segmentation/evaluate/eval_splitting.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.5/spine_segmentation/evaluate/load_model.py` & `spine_segmentation-0.2.0/spine_segmentation/evaluate/load_model.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.5/spine_segmentation/evaluate/metadata.py` & `spine_segmentation-0.2.0/spine_segmentation/evaluate/metadata.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.5/spine_segmentation/evaluate/volume_size_in_gt.py` & `spine_segmentation-0.2.0/spine_segmentation/evaluate/volume_size_in_gt.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.5/spine_segmentation/inference/instance_segmentation.py` & `spine_segmentation-0.2.0/spine_segmentation/inference/instance_segmentation.py`

 * *Files 13% similar despite different names*

```diff
@@ -114,51 +114,18 @@
             #     np.unique(curr_vertebra_instances),
             #     list(zip(*np.unique(vertebra_instances, return_counts=True))),
             # )
             if mse < best_mse:
                 best_mse = mse
                 best_vertebra_instances = curr_vertebra_instances
 
-    if plot_dir is not None:
-        import matplotlib.pyplot as plt
-
-        # fig, axes = plt.subplots(4, (len(plots) + 3) // 4)
-        fig, axes = plt.subplots(2, len(plots))
-        fig.tight_layout(pad=0)
-
-        from spine_segmentation.visualisation.color_palettes import get_alternating_palette
-
-        id_to_labels = dict(zip(range(1, 50), get_labels_for_n_classes(49)))
-        directory = get_next_log_dir()
-        for i, (instances, title, error_map) in enumerate(plots):
-            alternating = get_alternating_palette()
-            ax = axes[0, i]
-            single_plot(ax, alternating, None, instances[8, :, ::-1].T, id_to_labels, title, font_scale=0.4)
-            ax = axes[1, i]
-            single_plot(ax, alternating, error_map[8, :, ::-1].T != 0, None, id_to_labels, None, font_scale=0.4)
-
-        plt.savefig(plot_dir / f"mse_comparison.png", dpi=600)
-        plt.close()
-    # fig.close()
-
-    # np.unique(split_vertebra_segmentation + add2 * 100)
-    # plt.imshow((vertebra_instances - (split_vertebra_segmentation + add2 * i))[10])
-    # plt.imshow((split_vertebra_segmentation)[10])
-    # plt.show()
 
     # vertebra_instances = split_vertebra_segmentation + add2 * best_i
     vertebra_instances = best_vertebra_instances
 
-    # print(f"{np.unique(split_segmentation)=}")
-    # for i in np.unique(split_segmentation)[1:]:
-    #     instance_mask = split_segmentation == i
-    #     instance = vertebra_instances[instance_mask]
-    #     most_common = np.bincount(instance).argmax()
-    #     vertebra_instances[instance_mask] = most_common
-
     planes = get_planes_from_rois(vertebra_instances)
     # vertebrae = separate_segmented_rois(arr3d == 1)
     disc_instances = separate_segmented_rois_by_planes((segmentation == 2).astype(int), planes, use_plane_index=True)
     disc_instances[vertebra_instances != 0] = 0
 
     instances = vertebra_instances + disc_instances
     return mask_rare_rois(instances, 50)
@@ -181,14 +148,28 @@
 
 
 MODEL_HEIGHT = 896
 
 DeviceType = Union[Literal["CPU", "GPU"], int]
 
 
+def _add_channel_to_3d_mri(mri3d: np.ndarray):
+    """Given a shape (20, 320, 896), convert it to (20, 3, 320, 896), where in the RGB channel adjacent slices are encoded"""
+    first = np.roll(mri3d, axis=0, shift=1)
+    first[0, :, :] = first[1, :, :]
+
+    last = np.roll(mri3d, axis=0, shift=-1)
+    last[-1, :, :] = last[-2, :, :]
+
+    result = np.stack([first, mri3d, last], axis=1)
+    new_shape = (mri3d.shape[0], 3, mri3d.shape[1], mri3d.shape[2])
+    assert new_shape == result.shape
+    return result
+
+
 class SegmentationInference:
 
     def __init__(self, segmentation_device: DeviceType = "CPU", instance_segmentation_device: DeviceType = "CPU"):
         self._model_height = MODEL_HEIGHT
         self._onnx_seg_inference = ONNXInferenceModel.get_best_segmentation_model(device=segmentation_device)
         self._onnx_inst_inference = ONNXInferenceModel.get_best_instance_segmentation_model(
             device=instance_segmentation_device
@@ -209,30 +190,32 @@
                 "\n\n\tnp.tile(input_image, (3, 1, 1))\n"
             )
             exit(1)
         if len(mri_3d_numpy_image.shape) > 3:
             logger.error(f"mri_3d_numpy_image must be 3 dimensional. Got {mri_3d_numpy_image.shape}. "
                          f"Consider dropping the batch-dimension and just using the 3D mri image as entire input.")
 
-        padding_to_896 = ((0, 0), (0, 0), (0, 0), (0, mri_3d_numpy_image.shape[3] - MODEL_HEIGHT))
-        cropped_padded_seg_input = np.pad(mri_3d_numpy_image, padding_to_896, mode="constant")
+        mri_4d_with_channels = _add_channel_to_3d_mri(mri_3d_numpy_image)
+
+        padding_to_896 = ((0, 0), (0, 0), (0, 0), (0, mri_4d_with_channels.shape[3] - MODEL_HEIGHT))
+        cropped_padded_seg_input = np.pad(mri_4d_with_channels, padding_to_896, mode="constant")
         seg_npz = self._onnx_seg_inference.inference(cropped_padded_seg_input)
         inst_seg_input = seg_npz["segmentation"][:, None, :, :]
         cropped_inst_seg_input = inst_seg_input[:, :, :, :MODEL_HEIGHT]
         padding_to_416 = ((0, 0), (0, 0), (0, 0), (0, MODEL_HEIGHT - MODEL_HEIGHT))
         cropped_input_image_with_gt = np.concatenate(
             [
-                np.pad(mri_3d_numpy_image[:, 1:2, :, :], padding_to_416, mode="constant"),
+                np.pad(mri_4d_with_channels[:, 1:2, :, :], padding_to_416, mode="constant"),
                 (cropped_inst_seg_input == 1),
                 (cropped_inst_seg_input == 2),
             ],
             axis=1,
         )
         cropped_input_image_with_gt = cropped_input_image_with_gt.astype(np.float32)
-        cropped_input_image_without_gt = np.pad(mri_3d_numpy_image[:, :, :, :], padding_to_416, mode="constant").astype(
+        cropped_input_image_without_gt = np.pad(mri_4d_with_channels[:, :, :, :], padding_to_416, mode="constant").astype(
             np.float32
         )
 
         new_npz = self._onnx_inst_inference.inference(cropped_input_image_without_gt)
         new_npz["instances"] = new_npz["instances"] * 2 - (new_npz["instances"] != 0)
         # new_npz["id_to_label"] = gt_npz["id_to_label"]
         # new_npz["gt_id_to_label"] = gt_npz["id_to_label"]
```

### Comparing `spine_segmentation-0.1.5/spine_segmentation/inference/onnx_model.py` & `spine_segmentation-0.2.0/spine_segmentation/inference/onnx_model.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.5/spine_segmentation/instance_separation/instance_separation.py` & `spine_segmentation-0.2.0/spine_segmentation/instance_separation/instance_separation.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.5/spine_segmentation/model_downloader/model_downloader.py` & `spine_segmentation-0.2.0/spine_segmentation/model_downloader/model_downloader.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.5/spine_segmentation/plotting/bmi.py` & `spine_segmentation-0.2.0/spine_segmentation/plotting/bmi.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.5/spine_segmentation/plotting/classification_correlation.py` & `spine_segmentation-0.2.0/spine_segmentation/plotting/classification_correlation.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.5/spine_segmentation/plotting/patient_metadata.py` & `spine_segmentation-0.2.0/spine_segmentation/plotting/patient_metadata.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.5/spine_segmentation/plotting/plot_slice.py` & `spine_segmentation-0.2.0/spine_segmentation/plotting/plot_slice.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.5/spine_segmentation/plotting/plot_statistics.py` & `spine_segmentation-0.2.0/spine_segmentation/plotting/plot_statistics.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.5/spine_segmentation/plotting/read_npz_eval_per_roi_accuracy.py` & `spine_segmentation-0.2.0/spine_segmentation/plotting/read_npz_eval_per_roi_accuracy.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.5/spine_segmentation/plotting/show_plane_splitting_3d.py` & `spine_segmentation-0.2.0/spine_segmentation/plotting/show_plane_splitting_3d.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.5/spine_segmentation/resources/paths.py` & `spine_segmentation-0.2.0/spine_segmentation/resources/paths.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.5/spine_segmentation/resources/preloaded.py` & `spine_segmentation-0.2.0/spine_segmentation/resources/preloaded.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.5/spine_segmentation/scripts/format_results.py` & `spine_segmentation-0.2.0/spine_segmentation/scripts/format_results.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.5/spine_segmentation/scripts/split_train_val_test.py` & `spine_segmentation-0.2.0/spine_segmentation/scripts/split_train_val_test.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.5/spine_segmentation/spine_types/labels.py` & `spine_segmentation-0.2.0/spine_segmentation/spine_types/labels.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.5/spine_segmentation/spine_types/plane.py` & `spine_segmentation-0.2.0/spine_segmentation/spine_types/plane.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.5/spine_segmentation/trainer/learning_rate_finder.py` & `spine_segmentation-0.2.0/spine_segmentation/trainer/learning_rate_finder.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.5/spine_segmentation/utils/fix_validations_step_bar.py` & `spine_segmentation-0.2.0/spine_segmentation/utils/fix_validations_step_bar.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.5/spine_segmentation/utils/log_dir.py` & `spine_segmentation-0.2.0/spine_segmentation/utils/log_dir.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.5/spine_segmentation/utils/profiling.py` & `spine_segmentation-0.2.0/spine_segmentation/utils/profiling.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.5/spine_segmentation/utils/proxy_class.py` & `spine_segmentation-0.2.0/spine_segmentation/utils/proxy_class.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.5/spine_segmentation/visualisation/blender/blender_script.py` & `spine_segmentation-0.2.0/spine_segmentation/visualisation/blender/blender_script.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.5/spine_segmentation/visualisation/blender/gen_obj.py` & `spine_segmentation-0.2.0/spine_segmentation/visualisation/blender/gen_obj.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.5/spine_segmentation/visualisation/blender/open_in_blender.py` & `spine_segmentation-0.2.0/spine_segmentation/visualisation/blender/open_in_blender.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.5/spine_segmentation/visualisation/color.py` & `spine_segmentation-0.2.0/spine_segmentation/visualisation/color.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.5/spine_segmentation/visualisation/color_palettes.py` & `spine_segmentation-0.2.0/spine_segmentation/visualisation/color_palettes.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.5/PKG-INFO` & `spine_segmentation-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spine-segmentation
-Version: 0.1.5
+Version: 0.2.0
 Summary: Anatomical labeling of the spine in small field-of-view MRI scans
 Author: Brutenis Gliwa
 Author-email: brutenis@gmail.com
 Requires-Python: >=3.8.1,<3.13.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

