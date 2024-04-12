# Comparing `tmp/monai_deploy_app_sdk-0.6.0-py3-none-any.whl.zip` & `tmp/monai_deploy_app_sdk-1.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,64 +1,66 @@
-Zip file size: 125094 bytes, number of entries: 62
--rw-rw-r--  2.0 unx      832 b- defN 23-Sep-01 02:22 monai/deploy/__init__.py
--rw-rw-r--  2.0 unx      497 b- defN 23-Sep-01 03:57 monai/deploy/_version.py
--rw-rw-r--  2.0 unx      496 b- defN 23-Sep-01 01:59 monai/deploy/_version_local.py
--rw-rw-r--  2.0 unx     1359 b- defN 23-Sep-01 01:59 monai/deploy/exceptions.py
--rw-rw-r--  2.0 unx      665 b- defN 23-Sep-01 01:59 monai/deploy/logging.json
--rw-rw-r--  2.0 unx      323 b- defN 23-Sep-01 02:22 monai/deploy/conditions/__init__.py
--rw-rw-r--  2.0 unx     1592 b- defN 23-Sep-01 02:22 monai/deploy/core/__init__.py
--rw-rw-r--  2.0 unx     3380 b- defN 23-Sep-01 02:22 monai/deploy/core/app_context.py
--rw-rw-r--  2.0 unx     3684 b- defN 23-Sep-01 02:22 monai/deploy/core/arg_parser.py
--rw-rw-r--  2.0 unx      741 b- defN 23-Sep-01 02:22 monai/deploy/core/io_type.py
--rw-rw-r--  2.0 unx     1472 b- defN 23-Sep-01 02:22 monai/deploy/core/runtime_env.py
--rw-rw-r--  2.0 unx      790 b- defN 23-Sep-01 01:59 monai/deploy/core/datastores/__init__.py
--rw-rw-r--  2.0 unx     2062 b- defN 23-Sep-01 01:59 monai/deploy/core/datastores/datastore.py
--rw-rw-r--  2.0 unx     1522 b- defN 23-Sep-01 01:59 monai/deploy/core/datastores/factory.py
--rw-rw-r--  2.0 unx     1258 b- defN 23-Sep-01 01:59 monai/deploy/core/datastores/memory.py
--rw-rw-r--  2.0 unx     1068 b- defN 23-Sep-01 01:59 monai/deploy/core/domain/__init__.py
--rw-rw-r--  2.0 unx     2901 b- defN 23-Sep-01 01:59 monai/deploy/core/domain/datapath.py
--rw-rw-r--  2.0 unx     8530 b- defN 23-Sep-01 01:59 monai/deploy/core/domain/dicom_series.py
--rw-rw-r--  2.0 unx     5605 b- defN 23-Sep-01 01:59 monai/deploy/core/domain/dicom_series_selection.py
--rw-rw-r--  2.0 unx     1963 b- defN 23-Sep-01 01:59 monai/deploy/core/domain/dicom_sop_instance.py
--rw-rw-r--  2.0 unx     3611 b- defN 23-Sep-01 01:59 monai/deploy/core/domain/dicom_study.py
--rw-rw-r--  2.0 unx     1057 b- defN 23-Sep-01 01:59 monai/deploy/core/domain/domain.py
--rw-rw-r--  2.0 unx     1863 b- defN 23-Sep-01 01:59 monai/deploy/core/domain/image.py
--rw-rw-r--  2.0 unx      950 b- defN 23-Sep-01 01:59 monai/deploy/core/models/__init__.py
--rw-rw-r--  2.0 unx     2248 b- defN 23-Sep-01 01:59 monai/deploy/core/models/factory.py
--rw-rw-r--  2.0 unx     7865 b- defN 23-Sep-01 01:59 monai/deploy/core/models/model.py
--rw-rw-r--  2.0 unx     3398 b- defN 23-Sep-01 01:59 monai/deploy/core/models/named_model.py
--rw-rw-r--  2.0 unx     4472 b- defN 23-Sep-01 01:59 monai/deploy/core/models/torch_model.py
--rw-rw-r--  2.0 unx     4650 b- defN 23-Sep-01 01:59 monai/deploy/core/models/triton_model.py
--rw-rw-r--  2.0 unx       33 b- defN 23-Sep-01 02:22 monai/deploy/executors/__init__.py
--rw-rw-r--  2.0 unx       30 b- defN 23-Sep-01 02:22 monai/deploy/graphs/__init__.py
--rw-rw-r--  2.0 unx      110 b- defN 23-Sep-01 02:22 monai/deploy/logger/__init__.py
--rw-rw-r--  2.0 unx     2378 b- defN 23-Sep-01 02:22 monai/deploy/operators/__init__.py
--rw-rw-r--  2.0 unx     6178 b- defN 23-Sep-01 02:22 monai/deploy/operators/clara_viz_operator.py
--rw-rw-r--  2.0 unx    16371 b- defN 23-Sep-01 02:22 monai/deploy/operators/dicom_data_loader_operator.py
--rw-rw-r--  2.0 unx    13996 b- defN 23-Sep-01 02:22 monai/deploy/operators/dicom_encapsulated_pdf_writer_operator.py
--rw-rw-r--  2.0 unx    21642 b- defN 23-Sep-01 02:22 monai/deploy/operators/dicom_seg_writer_operator.py
--rw-rw-r--  2.0 unx    16536 b- defN 23-Sep-01 02:22 monai/deploy/operators/dicom_series_selector_operator.py
--rw-rw-r--  2.0 unx    17354 b- defN 23-Sep-01 02:22 monai/deploy/operators/dicom_series_to_volume_operator.py
--rw-rw-r--  2.0 unx    14428 b- defN 23-Sep-01 02:22 monai/deploy/operators/dicom_text_sr_writer_operator.py
--rw-rw-r--  2.0 unx    12722 b- defN 23-Sep-01 01:59 monai/deploy/operators/dicom_utils.py
--rw-rw-r--  2.0 unx     2918 b- defN 23-Sep-01 02:22 monai/deploy/operators/inference_operator.py
--rw-rw-r--  2.0 unx    40183 b- defN 23-Sep-01 02:22 monai/deploy/operators/monai_bundle_inference_operator.py
--rw-rw-r--  2.0 unx    24697 b- defN 23-Sep-01 02:22 monai/deploy/operators/monai_seg_inference_operator.py
--rw-rw-r--  2.0 unx     3898 b- defN 23-Sep-01 02:22 monai/deploy/operators/nii_data_loader_operator.py
--rw-rw-r--  2.0 unx     4664 b- defN 23-Sep-01 02:22 monai/deploy/operators/png_converter_operator.py
--rw-rw-r--  2.0 unx    23242 b- defN 23-Sep-01 02:22 monai/deploy/operators/publisher_operator.py
--rw-rw-r--  2.0 unx    18115 b- defN 23-Sep-01 02:22 monai/deploy/operators/stl_conversion_operator.py
--rw-rw-r--  2.0 unx       33 b- defN 23-Sep-01 02:22 monai/deploy/resources/__init__.py
--rw-rw-r--  2.0 unx        0 b- defN 23-Sep-01 01:59 monai/deploy/utils/__init__.py
--rw-rw-r--  2.0 unx     2897 b- defN 23-Sep-01 01:59 monai/deploy/utils/argparse_types.py
--rw-rw-r--  2.0 unx     1140 b- defN 23-Sep-01 01:59 monai/deploy/utils/deviceutil.py
--rw-rw-r--  2.0 unx     1838 b- defN 23-Sep-01 01:59 monai/deploy/utils/fileutil.py
--rw-rw-r--  2.0 unx    17078 b- defN 23-Sep-01 02:22 monai/deploy/utils/importutil.py
--rw-rw-r--  2.0 unx     4142 b- defN 23-Sep-01 01:59 monai/deploy/utils/sizeutil.py
--rw-rw-r--  2.0 unx     2597 b- defN 23-Sep-01 01:59 monai/deploy/utils/spinner.py
--rw-rw-r--  2.0 unx     4514 b- defN 23-Sep-01 02:22 monai/deploy/utils/version.py
--rw-rw-r--  2.0 unx    11357 b- defN 23-Sep-01 03:57 monai_deploy_app_sdk-0.6.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx     6797 b- defN 23-Sep-01 03:57 monai_deploy_app_sdk-0.6.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Sep-01 03:57 monai_deploy_app_sdk-0.6.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx        6 b- defN 23-Sep-01 03:57 monai_deploy_app_sdk-0.6.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     5878 b- defN 23-Sep-01 03:57 monai_deploy_app_sdk-0.6.0.dist-info/RECORD
-62 files, 368718 bytes uncompressed, 115544 bytes compressed:  68.7%
+Zip file size: 132371 bytes, number of entries: 64
+-rw-rw-r--  2.0 unx      832 b- defN 24-Mar-28 01:46 monai/deploy/__init__.py
+-rw-rw-r--  2.0 unx      497 b- defN 24-Apr-11 21:37 monai/deploy/_version.py
+-rw-rw-r--  2.0 unx      496 b- defN 24-Mar-28 00:46 monai/deploy/_version_1.0.py
+-rw-rw-r--  2.0 unx     1359 b- defN 23-Sep-01 03:58 monai/deploy/exceptions.py
+-rw-r--r--  2.0 unx      665 b- defN 23-Sep-01 03:58 monai/deploy/logging.json
+-rw-r--r--  2.0 unx        0 b- defN 22-Aug-30 23:50 monai/deploy/py.typed
+-rw-rw-r--  2.0 unx      324 b- defN 24-Apr-10 00:08 monai/deploy/conditions/__init__.py
+-rw-rw-r--  2.0 unx     1592 b- defN 23-Sep-01 03:58 monai/deploy/core/__init__.py
+-rw-rw-r--  2.0 unx     3380 b- defN 23-Sep-01 03:58 monai/deploy/core/app_context.py
+-rw-rw-r--  2.0 unx     3684 b- defN 23-Sep-01 03:58 monai/deploy/core/arg_parser.py
+-rw-rw-r--  2.0 unx      741 b- defN 23-Sep-01 03:58 monai/deploy/core/io_type.py
+-rw-rw-r--  2.0 unx     1472 b- defN 23-Sep-01 03:58 monai/deploy/core/runtime_env.py
+-rw-rw-r--  2.0 unx      790 b- defN 23-Sep-01 03:58 monai/deploy/core/datastores/__init__.py
+-rw-rw-r--  2.0 unx     2062 b- defN 23-Sep-01 03:58 monai/deploy/core/datastores/datastore.py
+-rw-rw-r--  2.0 unx     1522 b- defN 23-Sep-01 03:58 monai/deploy/core/datastores/factory.py
+-rw-rw-r--  2.0 unx     1258 b- defN 23-Sep-01 03:58 monai/deploy/core/datastores/memory.py
+-rw-rw-r--  2.0 unx     1068 b- defN 23-Sep-01 03:58 monai/deploy/core/domain/__init__.py
+-rw-rw-r--  2.0 unx     2901 b- defN 23-Sep-01 03:58 monai/deploy/core/domain/datapath.py
+-rw-rw-r--  2.0 unx     8530 b- defN 23-Sep-01 03:58 monai/deploy/core/domain/dicom_series.py
+-rw-rw-r--  2.0 unx     5605 b- defN 23-Sep-01 03:58 monai/deploy/core/domain/dicom_series_selection.py
+-rw-rw-r--  2.0 unx     1963 b- defN 23-Sep-01 03:58 monai/deploy/core/domain/dicom_sop_instance.py
+-rw-rw-r--  2.0 unx     3611 b- defN 23-Sep-01 03:58 monai/deploy/core/domain/dicom_study.py
+-rw-rw-r--  2.0 unx     1057 b- defN 23-Sep-01 03:58 monai/deploy/core/domain/domain.py
+-rw-rw-r--  2.0 unx     1863 b- defN 23-Sep-01 03:58 monai/deploy/core/domain/image.py
+-rw-rw-r--  2.0 unx      950 b- defN 23-Sep-01 03:58 monai/deploy/core/models/__init__.py
+-rw-rw-r--  2.0 unx     2248 b- defN 23-Sep-01 03:58 monai/deploy/core/models/factory.py
+-rw-rw-r--  2.0 unx     7865 b- defN 23-Sep-01 03:58 monai/deploy/core/models/model.py
+-rw-rw-r--  2.0 unx     3398 b- defN 23-Sep-01 03:58 monai/deploy/core/models/named_model.py
+-rw-rw-r--  2.0 unx     4472 b- defN 23-Sep-01 03:58 monai/deploy/core/models/torch_model.py
+-rw-rw-r--  2.0 unx     4650 b- defN 23-Sep-01 03:58 monai/deploy/core/models/triton_model.py
+-rw-rw-r--  2.0 unx       33 b- defN 23-Sep-01 03:58 monai/deploy/executors/__init__.py
+-rw-rw-r--  2.0 unx       30 b- defN 23-Sep-01 03:58 monai/deploy/graphs/__init__.py
+-rw-rw-r--  2.0 unx      110 b- defN 23-Sep-01 03:58 monai/deploy/logger/__init__.py
+-rw-rw-r--  2.0 unx     2378 b- defN 23-Sep-01 03:58 monai/deploy/operators/__init__.py
+-rw-rw-r--  2.0 unx     6178 b- defN 23-Sep-01 03:58 monai/deploy/operators/clara_viz_operator.py
+-rw-rw-r--  2.0 unx    16371 b- defN 23-Sep-01 03:58 monai/deploy/operators/dicom_data_loader_operator.py
+-rw-rw-r--  2.0 unx    13996 b- defN 23-Sep-01 03:58 monai/deploy/operators/dicom_encapsulated_pdf_writer_operator.py
+-rw-rw-r--  2.0 unx    22005 b- defN 23-Nov-20 02:56 monai/deploy/operators/dicom_seg_writer_operator.py
+-rw-rw-r--  2.0 unx    21940 b- defN 23-Nov-16 22:03 monai/deploy/operators/dicom_seg_writer_operator_all_frames.py
+-rw-rw-r--  2.0 unx    16536 b- defN 23-Sep-01 03:58 monai/deploy/operators/dicom_series_selector_operator.py
+-rw-rw-r--  2.0 unx    17354 b- defN 23-Sep-01 03:58 monai/deploy/operators/dicom_series_to_volume_operator.py
+-rw-rw-r--  2.0 unx    14428 b- defN 23-Sep-01 03:58 monai/deploy/operators/dicom_text_sr_writer_operator.py
+-rw-rw-r--  2.0 unx    12722 b- defN 23-Sep-01 03:58 monai/deploy/operators/dicom_utils.py
+-rw-rw-r--  2.0 unx     2918 b- defN 23-Sep-01 03:58 monai/deploy/operators/inference_operator.py
+-rw-rw-r--  2.0 unx    40183 b- defN 23-Sep-01 03:58 monai/deploy/operators/monai_bundle_inference_operator.py
+-rw-rw-r--  2.0 unx    24697 b- defN 23-Sep-01 03:58 monai/deploy/operators/monai_seg_inference_operator.py
+-rw-rw-r--  2.0 unx     3898 b- defN 23-Sep-01 03:58 monai/deploy/operators/nii_data_loader_operator.py
+-rw-rw-r--  2.0 unx     4664 b- defN 23-Sep-01 03:58 monai/deploy/operators/png_converter_operator.py
+-rw-rw-r--  2.0 unx    23242 b- defN 24-Mar-19 23:14 monai/deploy/operators/publisher_operator.py
+-rw-rw-r--  2.0 unx    18115 b- defN 23-Dec-06 04:38 monai/deploy/operators/stl_conversion_operator.py
+-rw-rw-r--  2.0 unx       33 b- defN 23-Sep-01 03:58 monai/deploy/resources/__init__.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Sep-01 03:58 monai/deploy/utils/__init__.py
+-rw-rw-r--  2.0 unx     2897 b- defN 23-Sep-01 03:58 monai/deploy/utils/argparse_types.py
+-rw-rw-r--  2.0 unx     1140 b- defN 23-Sep-01 03:58 monai/deploy/utils/deviceutil.py
+-rw-rw-r--  2.0 unx     1838 b- defN 23-Sep-01 03:58 monai/deploy/utils/fileutil.py
+-rw-rw-r--  2.0 unx    17078 b- defN 23-Sep-01 03:58 monai/deploy/utils/importutil.py
+-rw-rw-r--  2.0 unx     4142 b- defN 23-Sep-01 03:58 monai/deploy/utils/sizeutil.py
+-rw-rw-r--  2.0 unx     2597 b- defN 23-Sep-01 03:58 monai/deploy/utils/spinner.py
+-rw-rw-r--  2.0 unx     4514 b- defN 23-Sep-01 03:58 monai/deploy/utils/version.py
+-rw-r--r--  2.0 unx    11357 b- defN 24-Apr-11 21:37 monai_deploy_app_sdk-1.0.0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     7611 b- defN 24-Apr-11 21:37 monai_deploy_app_sdk-1.0.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-11 21:37 monai_deploy_app_sdk-1.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 24-Apr-11 21:37 monai_deploy_app_sdk-1.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     6071 b- defN 24-Apr-11 21:37 monai_deploy_app_sdk-1.0.0.dist-info/RECORD
+64 files, 392029 bytes uncompressed, 122507 bytes compressed:  68.8%
```

## zipnote {}

```diff
@@ -1,22 +1,25 @@
 Filename: monai/deploy/__init__.py
 Comment: 
 
 Filename: monai/deploy/_version.py
 Comment: 
 
-Filename: monai/deploy/_version_local.py
+Filename: monai/deploy/_version_1.0.py
 Comment: 
 
 Filename: monai/deploy/exceptions.py
 Comment: 
 
 Filename: monai/deploy/logging.json
 Comment: 
 
+Filename: monai/deploy/py.typed
+Comment: 
+
 Filename: monai/deploy/conditions/__init__.py
 Comment: 
 
 Filename: monai/deploy/core/__init__.py
 Comment: 
 
 Filename: monai/deploy/core/app_context.py
@@ -105,14 +108,17 @@
 
 Filename: monai/deploy/operators/dicom_encapsulated_pdf_writer_operator.py
 Comment: 
 
 Filename: monai/deploy/operators/dicom_seg_writer_operator.py
 Comment: 
 
+Filename: monai/deploy/operators/dicom_seg_writer_operator_all_frames.py
+Comment: 
+
 Filename: monai/deploy/operators/dicom_series_selector_operator.py
 Comment: 
 
 Filename: monai/deploy/operators/dicom_series_to_volume_operator.py
 Comment: 
 
 Filename: monai/deploy/operators/dicom_text_sr_writer_operator.py
@@ -165,23 +171,23 @@
 
 Filename: monai/deploy/utils/spinner.py
 Comment: 
 
 Filename: monai/deploy/utils/version.py
 Comment: 
 
-Filename: monai_deploy_app_sdk-0.6.0.dist-info/LICENSE
+Filename: monai_deploy_app_sdk-1.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: monai_deploy_app_sdk-0.6.0.dist-info/METADATA
+Filename: monai_deploy_app_sdk-1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: monai_deploy_app_sdk-0.6.0.dist-info/WHEEL
+Filename: monai_deploy_app_sdk-1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: monai_deploy_app_sdk-0.6.0.dist-info/top_level.txt
+Filename: monai_deploy_app_sdk-1.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: monai_deploy_app_sdk-0.6.0.dist-info/RECORD
+Filename: monai_deploy_app_sdk-1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## monai/deploy/_version.py

```diff
@@ -4,18 +4,18 @@
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
 {
- "date": "2023-08-31T20:56:55-0700",
+ "date": "2024-04-11T14:37:33-0700",
  "dirty": false,
  "error": null,
- "full-revisionid": "d5244a595f708a34f69d34944133d24e268425a6",
- "version": "0.6.0"
+ "full-revisionid": "24762f85bbf4874cfd0a46a3ad4471a2bbb9cbd9",
+ "version": "1.0.0"
 }
 '''  # END VERSION_JSON
 
 
 def get_versions():
     return json.loads(version_json)
```

## monai/deploy/conditions/__init__.py

```diff
@@ -4,10 +4,11 @@
 
     BooleanCondition
     CountCondition
     DownstreamMessageAffordableCondition
     MessageAvailableCondition
     PeriodicCondition
 """
+
 # Need to import explicit ones to quiet mypy complaints
 from holoscan.conditions import *
 from holoscan.conditions import CountCondition
```

## monai/deploy/operators/dicom_seg_writer_operator.py

```diff
@@ -180,14 +180,15 @@
     def __init__(
         self,
         fragment: Fragment,
         *args,
         segment_descriptions: List[SegmentDescription],
         output_folder: Path,
         custom_tags: Optional[Dict[str, str]] = None,
+        omit_empty_frames: bool = True,
         **kwargs,
     ):
         """Instantiates the DICOM Seg Writer instance with optional list of segment label strings.
 
         Each unique, non-zero integer value in the segmentation image represents a segment that must be
         described by an item of the segment descriptions list with the corresponding segment number.
         Items in the list must be arranged starting at segment number 1 and increasing by 1.
@@ -201,20 +202,24 @@
 
         Args:
             fragment (Fragment): An instance of the Application class which is derived from Fragment.
             segment_descriptions: List[SegmentDescription]
                 Object encapsulating the description of each segment present in the segmentation.
             output_folder: Folder for file output, overridden by named input on compute.
                            Defaults to current working dir's child folder, output.
-            custom_tags: OptonalDict[str, str], optional
+            custom_tags: Optonal[Dict[str, str]], optional
                 Dictionary for setting custom DICOM tags using Keywords and str values only
+            omit_empty_frames: bool, optional
+                Whether to omit frames that contain no segmented pixels from the output segmentation.
+                Defaults to True, same as the underlying lib API.
         """
 
         self._seg_descs = [sd.to_segment_description(n) for n, sd in enumerate(segment_descriptions, 1)]
         self._custom_tags = custom_tags
+        self._omit_empty_frames = omit_empty_frames
         self.output_folder = output_folder if output_folder else DICOMSegmentationWriterOperator.DEFAULT_OUTPUT_FOLDER
 
         self.input_name_seg = "seg_image"
         self.input_name_series = "study_selected_series_list"
         self.input_name_output_folder = "output_folder"
 
         super().__init__(fragment, *args, **kwargs)
@@ -319,14 +324,15 @@
             series_number=random_with_n_digits(4),
             sop_instance_uid=seg_sop_instance_uid,
             instance_number=1,
             manufacturer="The MONAI Consortium",
             manufacturer_model_name="MONAI Deploy App SDK",
             software_versions=version_str,
             device_serial_number="0000",
+            omit_empty_frames=self._omit_empty_frames,
         )
 
         # Adding a few tags that are not in the Dataset
         # Also try to set the custom tags that are of string type
         dt_now = datetime.datetime.now()
         seg.SeriesDate = dt_now.strftime("%Y%m%d")
         seg.SeriesTime = dt_now.strftime("%H%M%S")
```

## Comparing `monai_deploy_app_sdk-0.6.0.dist-info/LICENSE` & `monai_deploy_app_sdk-1.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `monai_deploy_app_sdk-0.6.0.dist-info/METADATA` & `monai_deploy_app_sdk-1.0.0.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: monai-deploy-app-sdk
-Version: 0.6.0
+Version: 1.0.0
 Summary: A framework and associated tools to design, verify and analyze performance of MONAI apps
 Home-page: https://monai.io/
 Author: MONAI Consortium
 Author-email: monai.contact@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.monai.io/projects/monai-deploy-app-sdk/en/stable/
 Project-URL: Bug Tracker, https://github.com/Project-MONAI/monai-deploy-app-sdk/issues
 Project-URL: Source Code, https://github.com/Project-MONAI/monai-deploy-app-sdk
 Platform: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8
 License-File: LICENSE
 Requires-Dist: numpy >=1.21.6
-Requires-Dist: holoscan ~=0.6.0
+Requires-Dist: holoscan ~=1.0
 Requires-Dist: colorama >=0.4.1
 Requires-Dist: typeguard >=3.0.0
 Provides-Extra: all
 Requires-Dist: cucim ~=21.06 ; extra == 'all'
 Provides-Extra: cucim
 Requires-Dist: cucim ~=21.06 ; extra == 'cucim'
 
@@ -42,37 +42,43 @@
 - Out-of-the-box support for in-proc PyTorch based inference
 - Easy incorporation of MONAI based pre and post transformations in the inference application
 - Package inference application with a single command into a portable MONAI Application Package
 - Locally run and debug your inference application using App Runner
 
 ## User Guide
 
-User guide is available at [docs.monai.io](https://docs.monai.io/projects/monai-deploy-app-sdk/en/latest/).
+User guide is available at [docs.monai.io](https://docs.monai.io/projects/monai-deploy-app-sdk/en/stable/).
 
 ## Installation
 
 To install [the current release](https://pypi.org/project/monai-deploy-app-sdk/), you can simply run:
 
 ```bash
 pip install monai-deploy-app-sdk  # '--pre' to install a pre-release version.
 ```
 
+Please also note the following system requirements:
+- Ubuntu 22.04 on X86-64 is required, as this is the only X86 platform that the underlying Holoscan SDK has been tested to support as of now.
+- [CUDA 12](https://developer.nvidia.com/cuda-12-0-0-download-archive) is required along with a supported NVIDIA GPU with at least 8GB of video RAM. If AI inference is not used in the example application and a GPU is not installed, at least [CUDA 12 runtime](https://pypi.org/project/nvidia-cuda-runtime-cu12/) is required, as this is one of the requirements of Holoscan SDK, in addition, the `LIB_LIBRARY_PATH` must be set to include the installed shared library, e.g. in a Python 3.8 env, ```export LD_LIBRARY_PATH=`pwd`/.venv/lib/python3.8/site-packages/nvidia/cuda_runtime/lib:$LD_LIBRARY_PATH```
+
+
+
 ## Getting Started
 
-Getting started guide is available at [here](https://docs.monai.io/projects/monai-deploy-app-sdk/en/latest/getting_started/index.html).
+Getting started guide is available at [here](https://docs.monai.io/projects/monai-deploy-app-sdk/en/stable/getting_started/index.html).
 
 ```bash
 pip install monai-deploy-app-sdk  # '--pre' to install a pre-release version.
 
 # Clone monai-deploy-app-sdk repository for accessing examples.
 git clone https://github.com/Project-MONAI/monai-deploy-app-sdk.git
 cd monai-deploy-app-sdk
 
 # Install necessary dependencies for simple_imaging_app
-pip install scikit-image
+pip install matplotlib Pillow scikit-image
 
 # Execute the app locally
 python examples/apps/simple_imaging_app/app.py -i examples/apps/simple_imaging_app/brain_mr_input.jpg -o output
 
 # Package app (creating MAP Docker image), using `-l DEBUG` option to see progress.
 monai-deploy package examples/apps/simple_imaging_app -c simple_imaging_app/app.yaml -t simple_app:latest --platform x64-workstation -l DEBUG
```

## Comparing `monai_deploy_app_sdk-0.6.0.dist-info/RECORD` & `monai_deploy_app_sdk-1.0.0.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 monai/deploy/__init__.py,sha256=DXLIYcUMLcOsT6XIjDWqmGdpzaUPe-qj8PxVYSMMl1E,832
-monai/deploy/_version.py,sha256=cC6_OaM93-3Vqo506VpLd_q9cimyIUy4_v2RDqK5emc,497
-monai/deploy/_version_local.py,sha256=munT4eLvF4rCneNJmmFhb8Ynr3mTKamoUSqj8LF7rxg,496
+monai/deploy/_version.py,sha256=N_auHepqoE2sx9B5nEcyFC-9iO4wSuFxfnpr5PIHyjQ,497
+monai/deploy/_version_1.0.py,sha256=yHsRFOvx_TjaPIv2EGhrg2XtE6WExFTqUlWqbqD0Npg,496
 monai/deploy/exceptions.py,sha256=8o4Xym6WQktL2FRiei7D06Jr9zlrNu91aIHc4bWNCdw,1359
 monai/deploy/logging.json,sha256=50nU8-uOWnPkw9JHXySMscMOFdB-W0rELBRPmDfw04g,665
-monai/deploy/conditions/__init__.py,sha256=cKi33rJ_bIQszkBXG077HBtjgmyKqg2axgCygVlpZx8,323
+monai/deploy/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+monai/deploy/conditions/__init__.py,sha256=50y80pXBcTJqS3nplAKIuF3qr12G1AniQluDJZE3Bi0,324
 monai/deploy/core/__init__.py,sha256=aa2nAaqRA7goOdoPIJISgP1dmfNnWChFookU4TZYF30,1592
 monai/deploy/core/app_context.py,sha256=I-FmQO4SSWmWm3MPou9qZUVGUrYYiOf0oqsurhk4DzI,3380
 monai/deploy/core/arg_parser.py,sha256=BPO3NqI9CdpdWJxEb5X8J4aR30YkavjlMe4XP3knmAI,3684
 monai/deploy/core/io_type.py,sha256=5vsdd73EDOVQKL6_0nm2M0vbNNVcSgj00GMjVNRHPyA,741
 monai/deploy/core/runtime_env.py,sha256=I0qeZr6MLASJ7y9cKmM_tV7v74Lu3OuvqsWg8eYhmb8,1472
 monai/deploy/core/datastores/__init__.py,sha256=fbbUSdRYdKLnyppa5mCw020Mbot4mACm8S7B6G4Ilf8,790
 monai/deploy/core/datastores/datastore.py,sha256=R06esFD-adxN9oBwXXoG1Z1FZfcSJStSkEV8gyx_U5I,2062
@@ -30,15 +31,16 @@
 monai/deploy/executors/__init__.py,sha256=jF9ZoW2aUeLjnnS5-VS8GtiHKJE7fl8SM-SKf7dxxtM,33
 monai/deploy/graphs/__init__.py,sha256=rgFo8AvtKZCsA2_NWNDQ5cHWtg7sQ1PS2j4DmYIAw8w,30
 monai/deploy/logger/__init__.py,sha256=lShzexwc5OqkxSaR7r7iL6CubSwsfkmEUW7E350N_Ww,110
 monai/deploy/operators/__init__.py,sha256=fIEeFBRPwVLkuV7vfnK-1xpx4RWno6G23OZhvnYMams,2378
 monai/deploy/operators/clara_viz_operator.py,sha256=8yrl78CfAN8qLlqhQCG4NQguuYHTpX8C2upPVcVDPJQ,6178
 monai/deploy/operators/dicom_data_loader_operator.py,sha256=Fz0Wdh1zc3FYjmgUZiftfCkXT7juMsUxz2chg4G4xFQ,16371
 monai/deploy/operators/dicom_encapsulated_pdf_writer_operator.py,sha256=gAB4b_ONCwqMDJKdBCUIOSrhALtucMcWwDH1GIOjGn4,13996
-monai/deploy/operators/dicom_seg_writer_operator.py,sha256=tgk1dR9zE7JWrYaON08Yv31cnvTjM8YdYKaHa9f56Mk,21642
+monai/deploy/operators/dicom_seg_writer_operator.py,sha256=TL4Zd9JkVFi21OxD1yrk7FHcRPl2RrqxEQnEvtchZVY,22005
+monai/deploy/operators/dicom_seg_writer_operator_all_frames.py,sha256=lrbI861Hf3DjYj5EDFTft-Bm7dWnBA8AdjeGpBj9hO4,21940
 monai/deploy/operators/dicom_series_selector_operator.py,sha256=vwWwhThak1XITXgFYWeWV_CZmMQLudkP13CeTPEWGf8,16536
 monai/deploy/operators/dicom_series_to_volume_operator.py,sha256=Rv0UVNLD234FtBFIxTTq2pgffTvK8uNpllwwZ8vcoLw,17354
 monai/deploy/operators/dicom_text_sr_writer_operator.py,sha256=99pMWBuO2xbWGFiEUcsN-dM96jrZEJZsOiVQvymeVtY,14428
 monai/deploy/operators/dicom_utils.py,sha256=gX2kQ7Ug-gYG0mMYJ_qth9m1_snvEomxaocYDC0-cvQ,12722
 monai/deploy/operators/inference_operator.py,sha256=Fgd8bnSzXGVN_4xHwf7vMltFT986YJ0jjaqmzTum4RQ,2918
 monai/deploy/operators/monai_bundle_inference_operator.py,sha256=bxT1ZFMn1SG4PCr02oKXKYs8bLzPoXOoQmEK7cpl_Ps,40183
 monai/deploy/operators/monai_seg_inference_operator.py,sha256=aHSSoP-cu_LOx8zwByd2hYYBW3h0xtsNJJUtirS-mBI,24697
@@ -51,12 +53,12 @@
 monai/deploy/utils/argparse_types.py,sha256=zCg8E61qQA8IRBmX708TMFNyAiMnZBw3aoRvXeFafls,2897
 monai/deploy/utils/deviceutil.py,sha256=hXmkMaKuHxrmpoKuc4tExr7BB7zOQIqnPLncznZzkuk,1140
 monai/deploy/utils/fileutil.py,sha256=9ep1glfCrCm-h85x5j_TKVs9KwxYTWrOtr_JV4Kb3Z0,1838
 monai/deploy/utils/importutil.py,sha256=5LKIac9aLAZZPPlSwokFu8YbB5jxhOow1fKjVOdZTSY,17078
 monai/deploy/utils/sizeutil.py,sha256=yej-GxO3NlguVhyy8WjcZB-Ard49eubtxAi90z0v5UE,4142
 monai/deploy/utils/spinner.py,sha256=PpqAE2CfBXEw1qEWUP9woW-vw28L4Tyn5AUeWsbnXwc,2597
 monai/deploy/utils/version.py,sha256=mSZ95TI2YV8Grxc7fUO-LISGK_GB6pe_tWF9Q-Ezdoc,4514
-monai_deploy_app_sdk-0.6.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-monai_deploy_app_sdk-0.6.0.dist-info/METADATA,sha256=POroo531Y0kCrsZUx09o8JWvbWGg0kHwDh9Sphg_0A8,6797
-monai_deploy_app_sdk-0.6.0.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-monai_deploy_app_sdk-0.6.0.dist-info/top_level.txt,sha256=UaNwRzLGORdus41Ip446s3bBfViLkdkDsXDo34J2P44,6
-monai_deploy_app_sdk-0.6.0.dist-info/RECORD,,
+monai_deploy_app_sdk-1.0.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+monai_deploy_app_sdk-1.0.0.dist-info/METADATA,sha256=NI1kZ_V2l4qT3Mc1XXruB0wfsL23F8BTvpMiFROyl2s,7611
+monai_deploy_app_sdk-1.0.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+monai_deploy_app_sdk-1.0.0.dist-info/top_level.txt,sha256=UaNwRzLGORdus41Ip446s3bBfViLkdkDsXDo34J2P44,6
+monai_deploy_app_sdk-1.0.0.dist-info/RECORD,,
```

