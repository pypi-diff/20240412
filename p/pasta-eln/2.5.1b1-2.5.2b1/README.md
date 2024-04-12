# Comparing `tmp/pasta_eln-2.5.1b1.tar.gz` & `tmp/pasta_eln-2.5.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pasta_eln-2.5.1b1.tar", last modified: Fri Apr  5 09:17:15 2024, max compression
+gzip compressed data, was "pasta_eln-2.5.2b1.tar", last modified: Fri Apr 12 11:11:17 2024, max compression
```

## Comparing `pasta_eln-2.5.1b1.tar` & `pasta_eln-2.5.2b1.tar`

### file list

```diff
@@ -1,179 +1,179 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:17:15.634384 pasta_eln-2.5.1b1/
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-05 09:17:15.634384 pasta_eln-2.5.1b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4952 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/README_PYPI.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:17:15.598384 pasta_eln-2.5.1b1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     7518 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:17:15.602384 pasta_eln-2.5.1b1/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:17:15.610384 pasta_eln-2.5.1b1/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)  2003429 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/docs/source/_static/Data_Hierarchy_Editor_Manual.odp
--rw-r--r--   0 runner    (1001) docker     (127)  1695262 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/docs/source/_static/Data_Hierarchy_Editor_Manual.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/docs/source/_static/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   225801 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/docs/source/_static/data_hierarchy_editor.png
--rw-r--r--   0 runner    (1001) docker     (127)   985134 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/docs/source/_static/metadata_group_combobox.png
--rw-r--r--   0 runner    (1001) docker     (127)    11481 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/docs/source/_static/pasta_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   100504 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/docs/source/_static/pyside.png
--rw-r--r--   0 runner    (1001) docker     (127)   846253 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/docs/source/_static/types_combo_box.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:17:15.598384 pasta_eln-2.5.1b1/docs/source/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:17:15.610384 pasta_eln-2.5.1b1/docs/source/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/docs/source/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/docs/source/data_hierarchy_configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/docs/source/dodonts.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9683 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/docs/source/extractors.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/docs/source/faqs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/docs/source/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11238 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/docs/source/motivation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/docs/source/userstory.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:17:15.614384 pasta_eln-2.5.1b1/pasta_eln/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:17:15.614384 pasta_eln-2.5.1b1/pasta_eln/Extractors/
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/Extractors/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/Extractors/extractor_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/Extractors/extractor_jpeg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/Extractors/extractor_jpg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/Extractors/extractor_json.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/Extractors/extractor_md.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/Extractors/extractor_png.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/Extractors/extractor_py.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:17:15.618384 pasta_eln-2.5.1b1/pasta_eln/GUI/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/_contextMenu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/body.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/configAuthors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/configGUI.py
--rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/configSetupLinux.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7874 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/configSetupWindows.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:17:15.622384 pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/attachments_tableview_data_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/create_type_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/create_type_dialog_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/create_type_dialog_base.ui
--rw-r--r--   0 runner    (1001) docker     (127)    23214 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/data_hierarchy_editor_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)    21471 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/data_hierarchy_editor_dialog_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    21656 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/data_hierarchy_editor_dialog_base.ui
--rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/delete_column_delegate.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/document_null_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/generic_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/iri_column_delegate.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/key_not_found_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/lookup_iri_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/mandatory_column_delegate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/metadata_tableview_data_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/reorder_column_delegate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7616 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/tableview_data_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/terminology_lookup_config.json
--rw-r--r--   0 runner    (1001) docker     (127)     7251 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/terminology_lookup_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     6836 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/terminology_lookup_dialog_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5381 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/terminology_lookup_dialog_base.ui
--rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/terminology_lookup_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    19014 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/utility_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:17:15.626384 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/completed_upload_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/completed_upload_task.ui
--rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/completed_uploads.py
--rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/completed_uploads_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/completed_uploads_base.ui
--rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/config_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/config_dialog_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8740 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/config_dialog_base.ui
--rw-r--r--   0 runner    (1001) docker     (127)     7415 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/controlled_vocab_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/dialog_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)    10081 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/edit_metadata_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     5920 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/edit_metadata_dialog_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4917 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/edit_metadata_dialog_base.ui
--rw-r--r--   0 runner    (1001) docker     (127)    10695 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/main_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     9688 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/main_dialog_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9608 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/main_dialog_base.ui
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/primitive_compound_controlled_frame_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/primitive_compound_controlled_frame_base.ui
--rw-r--r--   0 runner    (1001) docker     (127)    21062 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/primitive_compound_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/project_item_frame_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/project_item_frame_base.ui
--rw-r--r--   0 runner    (1001) docker     (127)     6550 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/upload_config_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     6087 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/upload_config_dialog_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/upload_config_dialog_base.ui
--rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/upload_widget_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/upload_widget_base.ui
--rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/details.py
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/docTypes.py
--rw-r--r--   0 runner    (1001) docker     (127)    29145 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/form.py
--rw-r--r--   0 runner    (1001) docker     (127)    18963 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    11340 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/projectGroup.py
--rw-r--r--   0 runner    (1001) docker     (127)    10059 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/projectLeafRenderer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8566 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/projectTreeView.py
--rw-r--r--   0 runner    (1001) docker     (127)     9559 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/sidebar.py
--rw-r--r--   0 runner    (1001) docker     (127)    19456 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/tableHeader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:17:15.598384 pasta_eln-2.5.1b1/pasta_eln/Resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:17:15.626384 pasta_eln-2.5.1b1/pasta_eln/Resources/ExampleMeasurements/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/Resources/ExampleMeasurements/simple.csv
--rw-r--r--   0 runner    (1001) docker     (127)     9450 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/Resources/ExampleMeasurements/simple.png
--rw-r--r--   0 runner    (1001) docker     (127)     8417 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/Resources/ExampleMeasurements/story.odt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:17:15.626384 pasta_eln-2.5.1b1/pasta_eln/Resources/Icons/
--rw-r--r--   0 runner    (1001) docker     (127)     5694 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/Resources/Icons/favicon64.ico
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/Resources/Icons/favicon64.png
--rw-r--r--   0 runner    (1001) docker     (127)    20226 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/Resources/Icons/ols.png
--rw-r--r--   0 runner    (1001) docker     (127)    17206 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/Resources/Icons/tib.png
--rw-r--r--   0 runner    (1001) docker     (127)     8673 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/Resources/Icons/wikidata.png
--rw-r--r--   0 runner    (1001) docker     (127)    17310 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/Resources/Icons/wikipedia.png
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35774 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/backend.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14107 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    43862 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/database.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:17:15.630384 pasta_eln-2.5.1b1/pasta_eln/dataverse/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/dataverse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12850 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/dataverse/base_database_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/dataverse/base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    31059 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/dataverse/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/dataverse/config_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     7487 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/dataverse/config_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/dataverse/data_upload_task.py
--rw-r--r--   0 runner    (1001) docker     (127)    11705 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/dataverse/database_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/dataverse/database_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    49819 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/dataverse/dataset-create-new-all-default-fields.json
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/dataverse/generic_task_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/dataverse/incorrect_parameter_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     8623 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/dataverse/project_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/dataverse/task_thread_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)    10671 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/dataverse/upload_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6157 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/dataverse/upload_queue_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/dataverse/upload_status_values.py
--rw-r--r--   0 runner    (1001) docker     (127)    21590 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/dataverse/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    29213 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/fixedStringsJson.py
--rw-r--r--   0 runner    (1001) docker     (127)    11775 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/guiCommunicate.py
--rw-r--r--   0 runner    (1001) docker     (127)    13007 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/guiStyle.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8622 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/handleDictionaries.py
--rw-r--r--   0 runner    (1001) docker     (127)    23440 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/inputOutput.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22498 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/installationTools.py
--rw-r--r--   0 runner    (1001) docker     (127)    10811 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/miscTools.py
--rw-r--r--   0 runner    (1001) docker     (127)     5789 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/mixin_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/printer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    23450 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/serverActions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:17:15.630384 pasta_eln-2.5.1b1/pasta_eln/webclient/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/webclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6567 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/webclient/http_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:17:15.630384 pasta_eln-2.5.1b1/pasta_eln.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-05 09:17:15.000000 pasta_eln-2.5.1b1/pasta_eln.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6120 2024-04-05 09:17:15.000000 pasta_eln-2.5.1b1/pasta_eln.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 09:17:15.000000 pasta_eln-2.5.1b1/pasta_eln.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-05 09:17:15.000000 pasta_eln-2.5.1b1/pasta_eln.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-05 09:17:15.000000 pasta_eln-2.5.1b1/pasta_eln.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-05 09:17:15.000000 pasta_eln-2.5.1b1/pasta_eln.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-04-05 09:17:15.634384 pasta_eln-2.5.1b1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      170 2024-04-05 09:17:15.000000 pasta_eln-2.5.1b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:17:15.630384 pasta_eln-2.5.1b1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7792 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/tests/test_01_3Projects.py
--rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/tests/test_02_3Projects_ExportImport.py
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/tests/test_50_importOthers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7794 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/tests/test_99_3Projects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:17.854858 pasta_eln-2.5.2b1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-12 11:11:17.854858 pasta_eln-2.5.2b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/README_PYPI.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:17.814859 pasta_eln-2.5.2b1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7518 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:17.814859 pasta_eln-2.5.2b1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:17.822858 pasta_eln-2.5.2b1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)  2003429 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/docs/source/_static/Data_Hierarchy_Editor_Manual.odp
+-rw-r--r--   0 runner    (1001) docker     (127)  1695262 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/docs/source/_static/Data_Hierarchy_Editor_Manual.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/docs/source/_static/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   225801 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/docs/source/_static/data_hierarchy_editor.png
+-rw-r--r--   0 runner    (1001) docker     (127)   985134 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/docs/source/_static/metadata_group_combobox.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11481 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/docs/source/_static/pasta_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   100504 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/docs/source/_static/pyside.png
+-rw-r--r--   0 runner    (1001) docker     (127)   846253 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/docs/source/_static/types_combo_box.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:17.810858 pasta_eln-2.5.2b1/docs/source/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:17.826858 pasta_eln-2.5.2b1/docs/source/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/docs/source/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/docs/source/data_hierarchy_configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/docs/source/dodonts.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9683 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/docs/source/extractors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/docs/source/faqs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/docs/source/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11238 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/docs/source/motivation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/docs/source/userstory.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:17.826858 pasta_eln-2.5.2b1/pasta_eln/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:17.830858 pasta_eln-2.5.2b1/pasta_eln/Extractors/
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/Extractors/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/Extractors/extractor_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/Extractors/extractor_jpeg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/Extractors/extractor_jpg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/Extractors/extractor_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/Extractors/extractor_md.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/Extractors/extractor_png.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/Extractors/extractor_py.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:17.834858 pasta_eln-2.5.2b1/pasta_eln/GUI/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/_contextMenu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/body.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/configAuthors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/configGUI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/configSetupLinux.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7874 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/configSetupWindows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:17.838858 pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/attachments_tableview_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/create_type_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/create_type_dialog_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/create_type_dialog_base.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    23214 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/data_hierarchy_editor_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21471 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/data_hierarchy_editor_dialog_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21656 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/data_hierarchy_editor_dialog_base.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/delete_column_delegate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/document_null_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/generic_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/iri_column_delegate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/key_not_found_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/lookup_iri_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/mandatory_column_delegate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/metadata_tableview_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/reorder_column_delegate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7616 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/tableview_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/terminology_lookup_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7251 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/terminology_lookup_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6836 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/terminology_lookup_dialog_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5381 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/terminology_lookup_dialog_base.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/terminology_lookup_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19014 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/utility_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:17.846858 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/completed_upload_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/completed_upload_task.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/completed_uploads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/completed_uploads_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/completed_uploads_base.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/config_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/config_dialog_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8740 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/config_dialog_base.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     7415 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/controlled_vocab_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/dialog_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10081 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/edit_metadata_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5920 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/edit_metadata_dialog_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4917 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/edit_metadata_dialog_base.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    10695 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/main_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9688 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/main_dialog_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9608 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/main_dialog_base.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/primitive_compound_controlled_frame_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/primitive_compound_controlled_frame_base.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    21062 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/primitive_compound_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/project_item_frame_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/project_item_frame_base.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     6550 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/upload_config_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6087 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/upload_config_dialog_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/upload_config_dialog_base.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/upload_widget_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/upload_widget_base.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/docTypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30148 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/form.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18969 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11340 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/projectGroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10059 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/projectLeafRenderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10503 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/projectTreeView.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9559 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/sidebar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19456 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/GUI/tableHeader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:17.810858 pasta_eln-2.5.2b1/pasta_eln/Resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:17.846858 pasta_eln-2.5.2b1/pasta_eln/Resources/ExampleMeasurements/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/Resources/ExampleMeasurements/simple.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     9450 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/Resources/ExampleMeasurements/simple.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8417 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/Resources/ExampleMeasurements/story.odt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:17.846858 pasta_eln-2.5.2b1/pasta_eln/Resources/Icons/
+-rw-r--r--   0 runner    (1001) docker     (127)     5694 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/Resources/Icons/favicon64.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/Resources/Icons/favicon64.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20226 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/Resources/Icons/ols.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17206 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/Resources/Icons/tib.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8673 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/Resources/Icons/wikidata.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17310 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/Resources/Icons/wikipedia.png
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35762 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/backend.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14107 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43862 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/database.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:17.850858 pasta_eln-2.5.2b1/pasta_eln/dataverse/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/dataverse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12850 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/dataverse/base_database_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/dataverse/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31059 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/dataverse/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/dataverse/config_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7487 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/dataverse/config_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/dataverse/data_upload_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11705 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/dataverse/database_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/dataverse/database_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49819 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/dataverse/dataset-create-new-all-default-fields.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/dataverse/generic_task_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/dataverse/incorrect_parameter_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8623 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/dataverse/project_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/dataverse/task_thread_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10671 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/dataverse/upload_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6157 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/dataverse/upload_queue_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/dataverse/upload_status_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21590 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/dataverse/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29212 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/fixedStringsJson.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11124 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/guiCommunicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13065 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/guiStyle.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8622 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/handleDictionaries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23440 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/inputOutput.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22498 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/installationTools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10811 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/miscTools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5789 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/mixin_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/printer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23596 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/serverActions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:17.850858 pasta_eln-2.5.2b1/pasta_eln/webclient/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/webclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6567 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pasta_eln/webclient/http_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:17.850858 pasta_eln-2.5.2b1/pasta_eln.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-12 11:11:17.000000 pasta_eln-2.5.2b1/pasta_eln.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6120 2024-04-12 11:11:17.000000 pasta_eln-2.5.2b1/pasta_eln.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 11:11:17.000000 pasta_eln-2.5.2b1/pasta_eln.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-12 11:11:17.000000 pasta_eln-2.5.2b1/pasta_eln.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-12 11:11:17.000000 pasta_eln-2.5.2b1/pasta_eln.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-12 11:11:17.000000 pasta_eln-2.5.2b1/pasta_eln.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-04-12 11:11:17.854858 pasta_eln-2.5.2b1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      170 2024-04-12 11:11:17.000000 pasta_eln-2.5.2b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:17.850858 pasta_eln-2.5.2b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7792 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/tests/test_01_3Projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/tests/test_02_3Projects_ExportImport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/tests/test_50_importOthers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7794 2024-04-12 11:11:13.000000 pasta_eln-2.5.2b1/tests/test_99_3Projects.py
```

### Comparing `pasta_eln-2.5.1b1/LICENSE` & `pasta_eln-2.5.2b1/LICENSE`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/PKG-INFO` & `pasta_eln-2.5.2b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pasta_eln
-Version: 2.5.1b1
+Version: 2.5.2b1
 Summary: The favorite ELN for experimental scientists
 Home-page: https://pasta-eln.github.io/
 Author: The PASTA-ELN Team and Steffen Brinckmann
 Author-email: sbrinckm@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pasta_eln-2.5.1b1/README.md` & `pasta_eln-2.5.2b1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -134,11 +134,18 @@
       from cProfile import Profile
       from pstats import SortKey, Stats
       with Profile() as profile:
 
 End...
       (Stats(profile).strip_dirs().sort_stats(SortKey.CUMULATIVE).print_stats()) #end cProfile
 
+#### Debugging on a conventional install: linux
+- 'sudo apt install python3-pudb' (not pip install)
+- create small 'temp.py' into any folder, with this content
+  from pasta_eln.gui import startMain
+  startMain()
+- start with 'pudb3 temp.py'
+
 
 #### General notes
 - Find qt-awesome icons: qta-browser
 - print works great in frondend and backend
```

### Comparing `pasta_eln-2.5.1b1/README_PYPI.md` & `pasta_eln-2.5.2b1/README_PYPI.md`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/docs/Makefile` & `pasta_eln-2.5.2b1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/docs/README.md` & `pasta_eln-2.5.2b1/docs/README.md`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/docs/source/_static/Data_Hierarchy_Editor_Manual.odp` & `pasta_eln-2.5.2b1/docs/source/_static/Data_Hierarchy_Editor_Manual.odp`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/docs/source/_static/Data_Hierarchy_Editor_Manual.pdf` & `pasta_eln-2.5.2b1/docs/source/_static/Data_Hierarchy_Editor_Manual.pdf`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/docs/source/_static/data_hierarchy_editor.png` & `pasta_eln-2.5.2b1/docs/source/_static/data_hierarchy_editor.png`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/docs/source/_static/metadata_group_combobox.png` & `pasta_eln-2.5.2b1/docs/source/_static/metadata_group_combobox.png`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/docs/source/_static/pasta_logo.svg` & `pasta_eln-2.5.2b1/docs/source/_static/pasta_logo.svg`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/docs/source/_static/pyside.png` & `pasta_eln-2.5.2b1/docs/source/_static/pyside.png`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/docs/source/_static/types_combo_box.png` & `pasta_eln-2.5.2b1/docs/source/_static/types_combo_box.png`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/docs/source/conf.py` & `pasta_eln-2.5.2b1/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 project = u'PASTA-ELN'
 copyright = u'2022-{}, PASTA-ELN team'.format(datetime.datetime.now().year)
 author = u'PASTA-ELN team'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
-version = "2.5.0"
+version = "2.5.1"
 release = version
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
```

### Comparing `pasta_eln-2.5.1b1/docs/source/data_hierarchy_configuration.rst` & `pasta_eln-2.5.2b1/docs/source/data_hierarchy_configuration.rst`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/docs/source/dodonts.rst` & `pasta_eln-2.5.2b1/docs/source/dodonts.rst`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/docs/source/extractors.rst` & `pasta_eln-2.5.2b1/docs/source/extractors.rst`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/docs/source/faqs.rst` & `pasta_eln-2.5.2b1/docs/source/faqs.rst`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/docs/source/index.rst` & `pasta_eln-2.5.2b1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/docs/source/install.rst` & `pasta_eln-2.5.2b1/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/docs/source/motivation.rst` & `pasta_eln-2.5.2b1/docs/source/motivation.rst`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/docs/source/userstory.rst` & `pasta_eln-2.5.2b1/docs/source/userstory.rst`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/Extractors/extractor_csv.py` & `pasta_eln-2.5.2b1/pasta_eln/Extractors/extractor_csv.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/Extractors/extractor_jpeg.py` & `pasta_eln-2.5.2b1/pasta_eln/Extractors/extractor_jpeg.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/Extractors/extractor_jpg.py` & `pasta_eln-2.5.2b1/pasta_eln/Extractors/extractor_jpg.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/Extractors/extractor_json.py` & `pasta_eln-2.5.2b1/pasta_eln/Extractors/extractor_json.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/Extractors/extractor_md.py` & `pasta_eln-2.5.2b1/pasta_eln/Extractors/extractor_md.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/Extractors/extractor_png.py` & `pasta_eln-2.5.2b1/pasta_eln/Extractors/extractor_png.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/Extractors/extractor_py.py` & `pasta_eln-2.5.2b1/pasta_eln/Extractors/extractor_py.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/_contextMenu.py` & `pasta_eln-2.5.2b1/pasta_eln/GUI/_contextMenu.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/body.py` & `pasta_eln-2.5.2b1/pasta_eln/GUI/body.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/config.py` & `pasta_eln-2.5.2b1/pasta_eln/GUI/config.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/configAuthors.py` & `pasta_eln-2.5.2b1/pasta_eln/GUI/configAuthors.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/configGUI.py` & `pasta_eln-2.5.2b1/pasta_eln/GUI/configGUI.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/configSetupLinux.py` & `pasta_eln-2.5.2b1/pasta_eln/GUI/configSetupLinux.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/configSetupWindows.py` & `pasta_eln-2.5.2b1/pasta_eln/GUI/configSetupWindows.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/attachments_tableview_data_model.py` & `pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/attachments_tableview_data_model.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/constants.py` & `pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/constants.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/create_type_dialog.py` & `pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/create_type_dialog.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/create_type_dialog_base.py` & `pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/create_type_dialog_base.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/create_type_dialog_base.ui` & `pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/create_type_dialog_base.ui`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/data_hierarchy_editor_dialog.py` & `pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/data_hierarchy_editor_dialog.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/data_hierarchy_editor_dialog_base.py` & `pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/data_hierarchy_editor_dialog_base.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/data_hierarchy_editor_dialog_base.ui` & `pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/data_hierarchy_editor_dialog_base.ui`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/delete_column_delegate.py` & `pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/delete_column_delegate.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/document_null_exception.py` & `pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/document_null_exception.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/generic_exception.py` & `pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/generic_exception.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/iri_column_delegate.py` & `pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/iri_column_delegate.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/key_not_found_exception.py` & `pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/key_not_found_exception.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/lookup_iri_action.py` & `pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/lookup_iri_action.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/mandatory_column_delegate.py` & `pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/mandatory_column_delegate.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/metadata_tableview_data_model.py` & `pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/metadata_tableview_data_model.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/reorder_column_delegate.py` & `pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/reorder_column_delegate.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/tableview_data_model.py` & `pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/tableview_data_model.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/terminology_lookup_config.json` & `pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/terminology_lookup_config.json`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/terminology_lookup_dialog.py` & `pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/terminology_lookup_dialog.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/terminology_lookup_dialog_base.py` & `pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/terminology_lookup_dialog_base.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/terminology_lookup_dialog_base.ui` & `pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/terminology_lookup_dialog_base.ui`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/terminology_lookup_service.py` & `pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/terminology_lookup_service.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/utility_functions.py` & `pasta_eln-2.5.2b1/pasta_eln/GUI/data_hierarchy/utility_functions.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/completed_upload_task.py` & `pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/completed_upload_task.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/completed_upload_task.ui` & `pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/completed_upload_task.ui`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/completed_uploads.py` & `pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/completed_uploads.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/completed_uploads_base.py` & `pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/completed_uploads_base.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/completed_uploads_base.ui` & `pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/completed_uploads_base.ui`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/config_dialog.py` & `pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/config_dialog.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/config_dialog_base.py` & `pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/config_dialog_base.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/config_dialog_base.ui` & `pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/config_dialog_base.ui`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/controlled_vocab_frame.py` & `pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/controlled_vocab_frame.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/dialog_extension.py` & `pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/dialog_extension.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/edit_metadata_dialog.py` & `pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/edit_metadata_dialog.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/edit_metadata_dialog_base.py` & `pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/edit_metadata_dialog_base.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/edit_metadata_dialog_base.ui` & `pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/edit_metadata_dialog_base.ui`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/main_dialog.py` & `pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/main_dialog.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/main_dialog_base.py` & `pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/main_dialog_base.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/main_dialog_base.ui` & `pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/main_dialog_base.ui`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/primitive_compound_controlled_frame_base.py` & `pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/primitive_compound_controlled_frame_base.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/primitive_compound_controlled_frame_base.ui` & `pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/primitive_compound_controlled_frame_base.ui`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/primitive_compound_frame.py` & `pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/primitive_compound_frame.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/project_item_frame_base.py` & `pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/project_item_frame_base.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/project_item_frame_base.ui` & `pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/project_item_frame_base.ui`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/upload_config_dialog.py` & `pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/upload_config_dialog.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/upload_config_dialog_base.py` & `pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/upload_config_dialog_base.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/upload_config_dialog_base.ui` & `pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/upload_config_dialog_base.ui`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/upload_widget_base.py` & `pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/upload_widget_base.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/upload_widget_base.ui` & `pasta_eln-2.5.2b1/pasta_eln/GUI/dataverse/upload_widget_base.ui`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/details.py` & `pasta_eln-2.5.2b1/pasta_eln/GUI/details.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/docTypes.py` & `pasta_eln-2.5.2b1/pasta_eln/GUI/docTypes.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/form.py` & `pasta_eln-2.5.2b1/pasta_eln/GUI/form.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     self.flagNewDoc = True
     if '_id' in self.doc or '_ids' in self.doc:
       self.flagNewDoc = False
     if self.flagNewDoc:
       self.setWindowTitle('Create new entry')
       self.doc['-name'] = ''
     else:
-      self.setWindowTitle('Edit content')
+      self.setWindowTitle('Edit information')
     self.skipKeys = ['image','metaVendor','metaUser','shasum']
     self.skipKeys0= ['_','-', '#']
     self.allHidden = False
 
     # GUI elements
     mainL = QVBoxLayout(self)
     splitter = QSplitter(Qt.Horizontal)
@@ -156,15 +156,15 @@
         elif (key[0] in self.skipKeys0) or key in self.skipKeys:  #skip non desired ones
           continue
         elif isinstance(value, list):   #list of items, qrCodes in sample
           if len(value)>0 and isinstance(value[0], str):
             setattr(self, f'key_{key}', QLineEdit(' '.join(value)))
             formL.addRow(QLabel(key.capitalize()), getattr(self, f'key_{key}'))
           else:
-            logging.info('Cannot display value of key=%s: %s. Write unknown content for docID=%s',
+            logging.info('Cannot display value of key=%s: %s. Write unknown value for docID=%s',
                          key, str(value), self.doc['_id'])
         elif isinstance(value, str):    #string
           dataHierarchyItem = [i for group in dataHierarchyNode for i in dataHierarchyNode[group] if i['name']==key]
           if len(dataHierarchyItem)==1 and 'list' in dataHierarchyItem[0]:       #choice dropdown
             setattr(self, f'key_{key}', QComboBox())
             if isinstance(dataHierarchyItem[0]['list'], list):            #dataHierarchy-defined choices
               getattr(self, f'key_{key}').addItems(dataHierarchyItem[0]['list'])
@@ -226,41 +226,59 @@
     TextButton('Cancel',           self, [Command.FORM_CANCEL],   buttonLineL, 'Discard changes')
     if self.flagNewDoc: #new dataset
       TextButton('Save && Next', self, [Command.FORM_SAVE_NEXT], buttonLineL, 'Save this and handle next')
     # autosave
     if (Path.home()/'.pastaELN.temp').is_file():
       with open(Path.home()/'.pastaELN.temp', 'r', encoding='utf-8') as fTemp:
         content = json.loads(fTemp.read())
-        for key in self.doc.keys():
-          if key[0] in self.skipKeys0 or key in self.skipKeys or key not in content:
-            continue
-          if key in ['comment','content']:
-            getattr(self, f'textEdit_{key}').setPlainText(content[key])
-          elif isinstance(getattr(self, f'key_{key}'), QLineEdit):
-            getattr(self, f'key_{key}').setText(content[key])
-          # skip QCombobox items since cannot be sure that next from has them and they are easy to recreate
+        if self.doc.get('_id', '') in content:
+          ret = QMessageBox.information(self, 'Information', 'There is an unsaved information from a '+
+                  'prematurely closed form. Do you want to restore it?\nIf you decline, the unsaved information'+
+                  'will be removed',
+                  QMessageBox.StandardButton.No | QMessageBox.StandardButton.Yes,      # type: ignore[operator]
+                  QMessageBox.StandardButton.Yes)
+          if ret==QMessageBox.StandardButton.Yes:
+            subContent = content[self.doc.get('_id', '')]
+            for key in subContent.keys():
+              if key in ('comment', 'content'):
+                getattr(self, f'textEdit_{key}').setPlainText(subContent[key])
+              elif key in ('-tags'):
+                self.doc[key] = subContent[key]
+                self.updateTagsBar()
+              elif isinstance(getattr(self, f'key_{key}'), QLineEdit):
+                getattr(self, f'key_{key}').setText(subContent[key])
+              # skip QCombobox items since cannot be sure that next from has them and they are easy to recreate
+          del content[self.doc.get('_id', '')]
+      with open(Path.home()/'.pastaELN.temp', 'w', encoding='utf-8') as fTemp:
+        fTemp.write(json.dumps(content))
     self.checkThreadTimer = QTimer(self)
     self.checkThreadTimer.setInterval(1*60*1000) #1 min
     self.checkThreadTimer.timeout.connect(self.autosave)
     self.checkThreadTimer.start()
 
 
   def autosave(self) -> None:
     """ Autosave comment to file """
     if self.comm.backend.configuration['GUI']['autosave'] == 'No':
       return
-    content = {'-name': getattr(self, 'key_-name').text().strip()}
-    for key in self.doc.keys():
+    subContent = {'-name':getattr(self, 'key_-name').text().strip(), '-tags':self.doc['-tags']}
+    for key in self.allKeys:
       if key in ['comment','content']:
-        content[key] = getattr(self, f'textEdit_{key}').toPlainText().strip()
+        subContent[key] = getattr(self, f'textEdit_{key}').toPlainText().strip()
       elif key[0] in self.skipKeys0 or key in self.skipKeys or not hasattr(self, f'key_{key}'):
         continue
       elif isinstance(getattr(self, f'key_{key}'), QLineEdit):
-        content[key] = getattr(self, f'key_{key}').text().strip()
+        subContent[key] = getattr(self, f'key_{key}').text().strip()
       # skip QCombobox items since cannot be sure that next from has them and they are easy to recreate
+    if (Path.home()/'.pastaELN.temp').is_file():
+      with open(Path.home()/'.pastaELN.temp', 'r', encoding='utf-8') as fTemp:
+        content = json.loads(fTemp.read())
+    else:
+      content = {}
+    content[self.doc.get('_id', '')] = subContent
     with open(Path.home()/'.pastaELN.temp', 'w', encoding='utf-8') as fTemp:
       fTemp.write(json.dumps(content))
     return
 
 
   def execute(self, command:list[Any]) -> None:
     """
@@ -325,24 +343,23 @@
           self.formsL[idx].itemAt(unknownWidget[1]).widget().hide()
         if command[1]=='comment' and len(unknownWidget)==5:
           self.formsL[idx].itemAt(unknownWidget[2]).widget().hide()
           self.formsL[idx].itemAt(unknownWidget[3]).widget().hide()
       self.allHidden = not self.allHidden
     elif command[0] is Command.FORM_CANCEL:
       if self.comm.backend.configuration['GUI']['autosave'] == 'Yes':
-        ret = QMessageBox.critical(self, 'Warning', 'You will loose all new data. Do you want to save it '+\
-                                   'for next time?',
-                                   QMessageBox.StandardButton.No | QMessageBox.StandardButton.Yes,  # type: ignore[operator]
-                                   QMessageBox.StandardButton.No)
+        ret = QMessageBox.critical(self, 'Warning', 'You will lose the entered information. Do you want to '+
+          'save everything to a temporary location?',
+          QMessageBox.StandardButton.Cancel | QMessageBox.StandardButton.No | QMessageBox.StandardButton.Yes,  # type: ignore[operator]
+          QMessageBox.StandardButton.No)
+        if ret==QMessageBox.StandardButton.Cancel:
+          return
         if ret==QMessageBox.StandardButton.Yes:
           self.autosave()
-        else:
-          self.checkThreadTimer.stop()
-          if (Path.home()/'.pastaELN.temp').is_file():
-            (Path.home()/'.pastaELN.temp').unlink()
+      self.checkThreadTimer.stop()
       self.reject()
     elif command[0] in (Command.FORM_SAVE, Command.FORM_SAVE_NEXT):
       # create the data that has to be saved
       self.checkThreadTimer.stop()
       if (Path.home()/'.pastaELN.temp').is_file():
         (Path.home()/'.pastaELN.temp').unlink()
       if hasattr(self, 'key_-name'):
```

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/project.py` & `pasta_eln-2.5.2b1/pasta_eln/GUI/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -251,15 +251,15 @@
         for line in children:
           self.comm.backend.db.remove(line['id'])
         #update sidebar, show projects
         self.comm.changeSidebar.emit('redraw')
         self.comm.changeTable.emit('x0','')
     elif command[0] is Command.SCAN:
       self.comm.backend.scanProject(self.comm.progressBar, self.projID, self.docProj['-branch'][0]['path'])
-      self.comm.changeSidebar.emit('redraw')
+      self.comm.changeProject.emit(self.projID,'')
       showMessage(self, 'Information','Scanning finished')
     elif command[0] is Command.SHOW_PROJ_DETAILS:
       self.docProj['-gui'][0] = not self.docProj['-gui'][0]
       self.comm.backend.db.setGUI(self.projID, self.docProj['-gui'])
       if self.infoWSA is not None and self.infoWSA.isHidden():
         self.infoWSA.show()
         self.actHideDetail.setText('Hide project details')
```

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/projectGroup.py` & `pasta_eln-2.5.2b1/pasta_eln/GUI/projectGroup.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/projectLeafRenderer.py` & `pasta_eln-2.5.2b1/pasta_eln/GUI/projectLeafRenderer.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/projectTreeView.py` & `pasta_eln-2.5.2b1/pasta_eln/GUI/projectTreeView.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 """ Custom tree view on data model """
 import subprocess, os, platform, logging, shutil
 from enum import Enum
 from pathlib import Path
 from typing import Any
-from PySide6.QtWidgets import QWidget, QTreeView, QAbstractItemView, QMenu, QMessageBox # pylint: disable=no-name-in-module
-from PySide6.QtGui import QStandardItemModel, QStandardItem  # pylint: disable=no-name-in-module
+from PySide6.QtWidgets import QWidget, QTreeView, QMenu, QMessageBox # pylint: disable=no-name-in-module
+from PySide6.QtGui import QStandardItemModel, QStandardItem, QMouseEvent # pylint: disable=no-name-in-module
 from PySide6.QtCore import QPoint, Qt  # pylint: disable=no-name-in-module
 from .projectLeafRenderer import ProjectLeafRenderer
 from ..guiStyle import Action, showMessage
 from ..guiCommunicate import Communicate
 
 class TreeView(QTreeView):
   """ Custom tree view on data model """
   def __init__(self, parent:QWidget, comm:Communicate, model:QStandardItemModel):
     super().__init__(parent)
     self.comm = comm
     self.setModel(model)
     self.setHeaderHidden(True)
     self.setStyleSheet('QTreeView::branch {border-image: none;}')
-    self.setExpandsOnDoubleClick(False)
     self.setIndentation(40)
     self.renderer = ProjectLeafRenderer(self.comm)
     self.setItemDelegate(self.renderer)
-    self.setDragDropMode(QAbstractItemView.InternalMove)
+    self.setExpandsOnDoubleClick(False)
+    self.setAcceptDrops(True)
+    self.setDropIndicatorShown(True)
+    self.setDefaultDropAction(Qt.MoveAction)
+    self.setDragDropMode(QTreeView.InternalMove)
     self.doubleClicked.connect(self.tree2Clicked)
 
 
   def contextMenuEvent(self, p:QPoint) -> None:
     """
     create context menu
 
@@ -127,17 +130,15 @@
       gui[0] = not gui[0]
       item.setData({ **item.data(), **{'gui':gui}})
       self.comm.backend.db.setGUI(docID, gui)
     elif command[0] is Command.HIDE:
       logging.debug('hide stack %s',str(hierStack))
       self.comm.backend.db.hideShow(hierStack)
       # self.comm.changeProject.emit('','') #refresh project
-      # after hide, not immediately hidden but on next refresh
-      # TODO Comment out for now to keep consistent with hide via context menu directly or form (which does
-      # not know it is a project )
+      # after hide, do not hide immediately but wait on next refresh
     elif command[0] is Command.OPEN_EXTERNAL or command[0] is Command.OPEN_FILEBROWSER:
       # depending if non-folder / folder; address different item in hierstack
       docID = hierStack[-2] \
         if command[0] is Command.OPEN_FILEBROWSER and hierStack[-1][0]!='x' \
         else hierStack[-1]
       doc   = self.comm.backend.db.getDoc(docID)
       if doc['-branch'][0]['path'] is None:
@@ -167,14 +168,69 @@
     docNew = self.comm.backend.db.getDoc(docID)
     item.setText(docNew['-name'])
     item.setData(item.data() | {"docType":docNew['-type'], "gui":docNew['-gui']})
     item.emitDataChanged()  #force redraw (resizing and repainting) of this item only
     return
 
 
+  def dragEnterEvent(self, event:QMouseEvent) -> None:
+    """
+    Override default: what happens if you drag an item
+
+    Args:
+      event (QMouseEvent): event
+    """
+    event.acceptProposedAction()
+    return
+
+
+  def dropEvent(self, event:QMouseEvent) -> None:
+    """
+    Override default: what happens at end of drag&drop
+
+    Args:
+      event (QMouseEvent): event
+    """
+    if event.mimeData().hasUrls():
+      item = self.model().itemFromIndex(self.indexAt(event.pos()))
+      if item.data()['docType'][0][0]!='x':
+        showMessage(self, 'Error', 'You cannot drop files on non folders.')
+        return
+      # create a list of all files
+      files, folders = [], []
+      for url in event.mimeData().urls():
+        path = url.toLocalFile()
+        if Path(path).is_file():
+          files.append(path)
+        else:
+          files +=   list(Path(path).rglob("*"))
+          folders += [x[0] for x in os.walk(path)]
+      docID = item.data()['hierStack'].split('/')[-1]
+      doc = self.comm.backend.db.getDoc(docID)
+      targetFolder = Path(self.comm.backend.cwd/doc['-branch'][0]['path'])
+      commonBase   = os.path.commonpath(folders+[str(i) for i in files])
+      # create folders and copy files
+      for folder in folders:
+        (targetFolder/(Path(folder).relative_to(commonBase))).mkdir(parents=True, exist_ok=True)
+      for fileStr in files:
+        file = Path(fileStr)
+        if file.is_file():
+          shutil.copy(file, targetFolder/(file.relative_to(commonBase)))
+      # scan
+      self.comm.backend.scanProject(self.comm.progressBar, docID, str(targetFolder) )
+      self.comm.changeProject.emit(item.data()['hierStack'].split('/')[0],'')
+      showMessage(self, 'Information','Drag & drop is finished')
+      event.ignore()
+    elif 'application/x-qstandarditemmodeldatalist' in event.mimeData().formats():
+      super().dropEvent(event)
+    else:
+      logging.error('Drop unknown data: %s', event.mimeData().formats())
+    return
+
+
 class Command(Enum):
   """ Commands used in this file """
   ADD_CHILD        = 1
   ADD_SIBLING      = 2
   DELETE           = 3
   SHOW_DETAILS   = 4
   HIDE             = 5
```

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/sidebar.py` & `pasta_eln-2.5.2b1/pasta_eln/GUI/sidebar.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/table.py` & `pasta_eln-2.5.2b1/pasta_eln/GUI/table.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/GUI/tableHeader.py` & `pasta_eln-2.5.2b1/pasta_eln/GUI/tableHeader.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/Resources/ExampleMeasurements/simple.png` & `pasta_eln-2.5.2b1/pasta_eln/Resources/ExampleMeasurements/simple.png`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/Resources/ExampleMeasurements/story.odt` & `pasta_eln-2.5.2b1/pasta_eln/Resources/ExampleMeasurements/story.odt`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/Resources/Icons/favicon64.ico` & `pasta_eln-2.5.2b1/pasta_eln/Resources/Icons/favicon64.ico`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/Resources/Icons/favicon64.png` & `pasta_eln-2.5.2b1/pasta_eln/Resources/Icons/favicon64.png`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/Resources/Icons/ols.png` & `pasta_eln-2.5.2b1/pasta_eln/Resources/Icons/ols.png`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/Resources/Icons/tib.png` & `pasta_eln-2.5.2b1/pasta_eln/Resources/Icons/tib.png`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/Resources/Icons/wikidata.png` & `pasta_eln-2.5.2b1/pasta_eln/Resources/Icons/wikidata.png`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/Resources/Icons/wikipedia.png` & `pasta_eln-2.5.2b1/pasta_eln/Resources/Icons/wikipedia.png`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/backend.py` & `pasta_eln-2.5.2b1/pasta_eln/backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -503,15 +503,15 @@
             if isinstance(doc[meta][item], tuple):
               doc[meta][item] = list(doc[meta][item])
             try:
               _ = json.dumps(doc[meta][item])
             except:
               doc[meta][item] = str(doc[meta][item])
               print('**Warning -> stringified  ',meta, item)
-        if doc['-type'][0] in [doc['recipe'].split('/')[0], '-']:
+        if doc['recipe'].startswith(doc['-type'][0]):
           doc['-type']     = doc['recipe'].split('/')
         else:
           #user has strange wish: trust him/her
           logging.info('user has strange wish: trust him/her: '+'/'.join(doc['-type'])+'  '+doc['recipe'])
         del doc['recipe']
         if 'fileExtension' not in doc['metaVendor']:
           doc['metaVendor']['fileExtension'] = extension.lower()
```

### Comparing `pasta_eln-2.5.1b1/pasta_eln/cli.py` & `pasta_eln-2.5.2b1/pasta_eln/cli.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/database.py` & `pasta_eln-2.5.2b1/pasta_eln/database.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/dataverse/base_database_api.py` & `pasta_eln-2.5.2b1/pasta_eln/dataverse/base_database_api.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/dataverse/base_model.py` & `pasta_eln-2.5.2b1/pasta_eln/dataverse/base_model.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/dataverse/client.py` & `pasta_eln-2.5.2b1/pasta_eln/dataverse/client.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/dataverse/config_error.py` & `pasta_eln-2.5.2b1/pasta_eln/dataverse/config_error.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/dataverse/config_model.py` & `pasta_eln-2.5.2b1/pasta_eln/dataverse/config_model.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/dataverse/data_upload_task.py` & `pasta_eln-2.5.2b1/pasta_eln/dataverse/data_upload_task.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/dataverse/database_api.py` & `pasta_eln-2.5.2b1/pasta_eln/dataverse/database_api.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/dataverse/database_error.py` & `pasta_eln-2.5.2b1/pasta_eln/dataverse/database_error.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/dataverse/dataset-create-new-all-default-fields.json` & `pasta_eln-2.5.2b1/pasta_eln/dataverse/dataset-create-new-all-default-fields.json`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/dataverse/generic_task_object.py` & `pasta_eln-2.5.2b1/pasta_eln/dataverse/generic_task_object.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/dataverse/incorrect_parameter_error.py` & `pasta_eln-2.5.2b1/pasta_eln/dataverse/incorrect_parameter_error.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/dataverse/project_model.py` & `pasta_eln-2.5.2b1/pasta_eln/dataverse/project_model.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/dataverse/task_thread_extension.py` & `pasta_eln-2.5.2b1/pasta_eln/dataverse/task_thread_extension.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/dataverse/upload_model.py` & `pasta_eln-2.5.2b1/pasta_eln/dataverse/upload_model.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/dataverse/upload_queue_manager.py` & `pasta_eln-2.5.2b1/pasta_eln/dataverse/upload_queue_manager.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/dataverse/upload_status_values.py` & `pasta_eln-2.5.2b1/pasta_eln/dataverse/upload_status_values.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/dataverse/utils.py` & `pasta_eln-2.5.2b1/pasta_eln/dataverse/utils.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/fixedStringsJson.py` & `pasta_eln-2.5.2b1/pasta_eln/fixedStringsJson.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
   "general": {
     "theme": ["Theme",
               "light_blue",
               ["dark_amber", "dark_blue", "dark_cyan", "dark_lightgreen", "dark_pink", "dark_purple", "dark_red", \
                "dark_teal", "dark_yellow", "light_amber", "light_blue", "light_cyan", "light_lightgreen", \
                "light_pink", "light_purple", "light_red", "light_teal", "light_yellow", "none"]],
     "loggingLevel":  ["Logging level (more->less)", "INFO", ["DEBUG", "INFO", "WARNING", "ERROR"]],
-    "autosave":      ["Autosave entries in form", "Yes", ["Yes", "No"]],
+    "autosave":      ["Autosave entries in form", "No", ["Yes", "No"]],
     "showProjectBtn":["Show project button on top-left", "Yes", ["Yes", "No"]]
   },
   "dimensions": {
     "sidebarWidth": ["Sidebar width", 280, [220, 280, 340]],
     "maxTableColumnWidth": ["Maximum column width in tables", 400, [300, 400, 500, 600]],
     "imageSizeDetails": ["Image size in details view and form", 600, [300, 400, 500, 600]],
     "imageWidthProject": ["Image width in project view", 300, [200, 250, 300, 350, 400]],
```

### Comparing `pasta_eln-2.5.1b1/pasta_eln/gui.py` & `pasta_eln-2.5.2b1/pasta_eln/gui.py`

 * *Files 3% similar despite different names*

```diff
@@ -100,24 +100,14 @@
     # if hasattr(self.comm.backend, 'configuration'):
     #   sidebarScroll.setFixedWidth(self.comm.backend.configuration['GUI']['sidebarWidth']+10)
     # mainLayout.addWidget(sidebarScroll)
     mainLayout.addWidget(self.sidebar)
     mainLayout.addWidget(body)
     self.comm.changeTable.emit('x0', '')
 
-    #check if temporary save exist: warn user
-    if (Path.home()/'.pastaELN.temp').is_file():
-      ret = QMessageBox.information(self, 'Information', 'There is data from a prematurely closed form. '+
-              'Do you want to use it? \n\n- If you choose yes, please reopen that form and content will' +
-              'be reloaded.\n\n- If you choose no, this temporary data will be removed now.',
-              QMessageBox.StandardButton.No | QMessageBox.StandardButton.Yes,      # type: ignore[operator]
-              QMessageBox.StandardButton.Yes)
-      if ret==QMessageBox.StandardButton.No:
-        (Path.home()/'.pastaELN.temp').unlink()
-
 
   @Slot(str)
   def formDoc(self, doc: dict[str, Any]) -> None:
     """
     What happens when new/edit dialog is shown
 
     Args:
```

### Comparing `pasta_eln-2.5.1b1/pasta_eln/guiCommunicate.py` & `pasta_eln-2.5.2b1/pasta_eln/guiCommunicate.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/guiStyle.py` & `pasta_eln-2.5.2b1/pasta_eln/guiStyle.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,16 @@
       style (str): css style
       hide (bool): hidden or shown initially
     """
     super().__init__()
     self.setText(label)
     self.setCheckable(checkable)
     self.setChecked(checkable)
+    self.setAutoDefault(False)
+    self.setDefault(False)
     self.clicked.connect(lambda: widget.execute(command))
     if tooltip:
       self.setToolTip(tooltip)
     if style:
       self.setStyleSheet(style)
     else:
       primaryColor   = getColor(widget.comm.backend, 'primary')
```

### Comparing `pasta_eln-2.5.1b1/pasta_eln/handleDictionaries.py` & `pasta_eln-2.5.2b1/pasta_eln/handleDictionaries.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/inputOutput.py` & `pasta_eln-2.5.2b1/pasta_eln/inputOutput.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/installationTools.py` & `pasta_eln-2.5.2b1/pasta_eln/installationTools.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/miscTools.py` & `pasta_eln-2.5.2b1/pasta_eln/miscTools.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/mixin_cli.py` & `pasta_eln-2.5.2b1/pasta_eln/mixin_cli.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/printer.py` & `pasta_eln-2.5.2b1/pasta_eln/printer.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/serverActions.py` & `pasta_eln-2.5.2b1/pasta_eln/serverActions.py`

 * *Files 0% similar despite different names*

```diff
@@ -450,14 +450,17 @@
   with ZipFile(fileName, 'r', compression=ZIP_DEFLATED) as zipFile:
     files = zipFile.namelist()
     #first run through: create documents and design documents
     for fileI in files:
       fileParts = fileI.split('/')[1:]
       if fileParts==['pastaELN.json']: #do not recreate file, it is only there for manual recovery
         continue
+      if len(fileParts)!=2 or fileParts[-1]=='':
+        print(f"**ERROR: Cannot process file {fileI}: does not have 1+2 parts")
+        continue
       database = fileParts[0]
       docID = fileParts[1]
       if docID.endswith('_attach'):
         continue #Do in second loop
       #test if database is exists: create otherwise
       resp = requests.get(f'http://{location}:5984/{database}/_all_docs', headers=headers, auth=authUser, timeout=10)
       if resp.status_code != 200 and resp.json()['reason']=='Database does not exist.':
```

### Comparing `pasta_eln-2.5.1b1/pasta_eln/utils.py` & `pasta_eln-2.5.2b1/pasta_eln/utils.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln/webclient/http_client.py` & `pasta_eln-2.5.2b1/pasta_eln/webclient/http_client.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/pasta_eln.egg-info/PKG-INFO` & `pasta_eln-2.5.2b1/pasta_eln.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pasta_eln
-Version: 2.5.1b1
+Version: 2.5.2b1
 Summary: The favorite ELN for experimental scientists
 Home-page: https://pasta-eln.github.io/
 Author: The PASTA-ELN Team and Steffen Brinckmann
 Author-email: sbrinckm@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pasta_eln-2.5.1b1/pasta_eln.egg-info/SOURCES.txt` & `pasta_eln-2.5.2b1/pasta_eln.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/setup.cfg` & `pasta_eln-2.5.2b1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/tests/test_01_3Projects.py` & `pasta_eln-2.5.2b1/tests/test_01_3Projects.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/tests/test_02_3Projects_ExportImport.py` & `pasta_eln-2.5.2b1/tests/test_02_3Projects_ExportImport.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/tests/test_50_importOthers.py` & `pasta_eln-2.5.2b1/tests/test_50_importOthers.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.1b1/tests/test_99_3Projects.py` & `pasta_eln-2.5.2b1/tests/test_99_3Projects.py`

 * *Files identical despite different names*

