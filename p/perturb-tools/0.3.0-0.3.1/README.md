# Comparing `tmp/perturb-tools-0.3.0.tar.gz` & `tmp/perturb_tools-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perturb-tools-0.3.0.tar", last modified: Sun Nov 26 00:55:56 2023, max compression
+gzip compressed data, was "perturb_tools-0.3.1.tar", last modified: Fri Apr 12 18:42:03 2024, max compression
```

## Comparing `perturb-tools-0.3.0.tar` & `perturb_tools-0.3.1.tar`

### file list

```diff
@@ -1,134 +1,90 @@
-drwxrwx---   0 jr1025   (5074632) pinello  (10066)        0 2023-11-26 00:55:56.518941 perturb-tools-0.3.0/
-drwxrwx---   0 jr1025   (5074632) pinello  (10066)        0 2023-11-26 00:55:55.428025 perturb-tools-0.3.0/.github/
-drwxrwx---   0 jr1025   (5074632) pinello  (10066)        0 2023-11-26 00:55:55.556014 perturb-tools-0.3.0/.github/workflows/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      856 2021-11-08 18:28:06.000000 perturb-tools-0.3.0/.github/workflows/pypi_release.yml
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1799 2021-11-08 18:28:06.000000 perturb-tools-0.3.0/.gitignore
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1072 2021-11-08 18:28:06.000000 perturb-tools-0.3.0/LICENSE
--rw-r--r--   0 jr1025   (5074632) pinello  (10066)     3770 2023-11-26 00:55:56.508501 perturb-tools-0.3.0/PKG-INFO
--rw-r--r--   0 jr1025   (5074632) pinello  (10066)     2706 2023-08-21 19:42:09.000000 perturb-tools-0.3.0/README.md
-drwxrwx---   0 jr1025   (5074632) pinello  (10066)        0 2023-11-26 00:55:55.433774 perturb-tools-0.3.0/docs/
-drwxrwx---   0 jr1025   (5074632) pinello  (10066)        0 2023-11-26 00:55:55.572917 perturb-tools-0.3.0/docs/images/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     7007 2021-11-08 18:28:06.000000 perturb-tools-0.3.0/docs/images/perturb_tools_logo.svg
--rw-rw----   0 jr1025   (5074632) pinello  (10066)   185680 2021-11-08 18:28:06.000000 perturb-tools-0.3.0/docs/images/screendata.svg
-drwxrwx---   0 jr1025   (5074632) pinello  (10066)        0 2023-11-26 00:55:55.619771 perturb-tools-0.3.0/perturb_tools/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     6148 2022-07-11 22:11:21.000000 perturb-tools-0.3.0/perturb_tools/.DS_Store
--rw-r--r--   0 jr1025   (5074632) pinello  (10066)      416 2023-08-21 19:42:09.000000 perturb-tools-0.3.0/perturb_tools/__init__.py
-drwxrwx---   0 jr1025   (5074632) pinello  (10066)        0 2023-11-26 00:55:55.678474 perturb-tools-0.3.0/perturb_tools/_arithmetic/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      103 2022-07-11 22:11:21.000000 perturb-tools-0.3.0/perturb_tools/_arithmetic/__init__.py
-drwxrwx---   0 jr1025   (5074632) pinello  (10066)        0 2023-11-26 00:55:55.710985 perturb-tools-0.3.0/perturb_tools/_arithmetic/_funcs/
-drwxrwx---   0 jr1025   (5074632) pinello  (10066)        0 2023-11-26 00:55:55.733329 perturb-tools-0.3.0/perturb_tools/_arithmetic/_funcs/_LogFoldChange/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     4164 2022-07-11 22:11:21.000000 perturb-tools-0.3.0/perturb_tools/_arithmetic/_funcs/_LogFoldChange/_LogFoldChange_Module.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)        0 2022-07-12 20:47:57.000000 perturb-tools-0.3.0/perturb_tools/_arithmetic/_funcs/_LogFoldChange/__init__.py
--rw-r--r--   0 jr1025   (5074632) pinello  (10066)     1806 2023-08-21 19:42:09.000000 perturb-tools-0.3.0/perturb_tools/_arithmetic/_funcs/_LogFoldChange/_calculate_log_fold_change.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     2189 2022-07-11 22:11:21.000000 perturb-tools-0.3.0/perturb_tools/_arithmetic/_funcs/_SequenceManipulation.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)        0 2022-07-12 20:47:25.000000 perturb-tools-0.3.0/perturb_tools/_arithmetic/_funcs/__init__.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      192 2022-07-11 22:11:21.000000 perturb-tools-0.3.0/perturb_tools/_arithmetic/_funcs/_log_fold_change.py
-drwxrwx---   0 jr1025   (5074632) pinello  (10066)        0 2023-11-26 00:55:55.742499 perturb-tools-0.3.0/perturb_tools/_experimental_design/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      504 2022-07-12 20:50:08.000000 perturb-tools-0.3.0/perturb_tools/_experimental_design/__init__.py
-drwxrwx---   0 jr1025   (5074632) pinello  (10066)        0 2023-11-26 00:55:55.751478 perturb-tools-0.3.0/perturb_tools/_experimental_design/_coding/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)        0 2022-07-12 20:50:30.000000 perturb-tools-0.3.0/perturb_tools/_experimental_design/_coding/__init__.py
-drwxrwx---   0 jr1025   (5074632) pinello  (10066)        0 2023-11-26 00:55:55.771668 perturb-tools-0.3.0/perturb_tools/_experimental_design/_coding/_funcs/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)        0 2022-07-12 20:50:25.000000 perturb-tools-0.3.0/perturb_tools/_experimental_design/_coding/_funcs/__init__.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1128 2022-07-12 05:46:12.000000 perturb-tools-0.3.0/perturb_tools/_experimental_design/_coding/_funcs/_plot_CDS.py
-drwxrwx---   0 jr1025   (5074632) pinello  (10066)        0 2023-11-26 00:55:55.781932 perturb-tools-0.3.0/perturb_tools/_experimental_design/_funcs/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)        0 2022-07-12 21:07:41.000000 perturb-tools-0.3.0/perturb_tools/_experimental_design/_funcs/__init__.py
-drwxrwx---   0 jr1025   (5074632) pinello  (10066)        0 2023-11-26 00:55:55.929014 perturb-tools-0.3.0/perturb_tools/_experimental_design/_general/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      229 2022-07-11 22:11:22.000000 perturb-tools-0.3.0/perturb_tools/_experimental_design/_general/_GTF_Module.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     3536 2022-07-11 22:11:22.000000 perturb-tools-0.3.0/perturb_tools/_experimental_design/_general/_TargetModule.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)        0 2022-07-12 21:07:26.000000 perturb-tools-0.3.0/perturb_tools/_experimental_design/_general/__init__.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      304 2022-07-11 22:11:22.000000 perturb-tools-0.3.0/perturb_tools/_experimental_design/_general/_add_region_labels.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     2125 2022-07-11 22:11:22.000000 perturb-tools-0.3.0/perturb_tools/_experimental_design/_general/_add_sgRNA_context.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      777 2022-07-11 22:11:22.000000 perturb-tools-0.3.0/perturb_tools/_experimental_design/_general/_annotate_guide_biochemistry.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     2096 2022-07-11 22:11:22.000000 perturb-tools-0.3.0/perturb_tools/_experimental_design/_general/_annotate_protospacer.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      870 2022-07-11 22:11:22.000000 perturb-tools-0.3.0/perturb_tools/_experimental_design/_general/_get_chromosome_sequence.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      768 2022-07-11 22:11:22.000000 perturb-tools-0.3.0/perturb_tools/_experimental_design/_general/_get_screen_target_features.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     6031 2022-07-11 22:11:22.000000 perturb-tools-0.3.0/perturb_tools/_experimental_design/_general/_identify_overlapping_fragments.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     4535 2022-07-11 22:11:22.000000 perturb-tools-0.3.0/perturb_tools/_experimental_design/_general/_make_guide_library_df.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     5407 2022-07-11 22:11:22.000000 perturb-tools-0.3.0/perturb_tools/_experimental_design/_general/_query_region_for_PAM.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1444 2022-07-11 22:11:22.000000 perturb-tools-0.3.0/perturb_tools/_experimental_design/_general/_scan_for_BsmbI.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      157 2022-07-11 22:11:22.000000 perturb-tools-0.3.0/perturb_tools/_experimental_design/_general/_widen_regions.py
-drwxrwx---   0 jr1025   (5074632) pinello  (10066)        0 2023-11-26 00:55:55.937754 perturb-tools-0.3.0/perturb_tools/_external_tools/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      213 2022-07-11 22:11:22.000000 perturb-tools-0.3.0/perturb_tools/_external_tools/__init__.py
-drwxrwx---   0 jr1025   (5074632) pinello  (10066)        0 2023-11-26 00:55:55.983468 perturb-tools-0.3.0/perturb_tools/_framework/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      593 2022-07-12 05:52:01.000000 perturb-tools-0.3.0/perturb_tools/_framework/README.md
--rw-r--r--   0 jr1025   (5074632) pinello  (10066)    15308 2023-11-25 20:50:54.000000 perturb-tools-0.3.0/perturb_tools/_framework/_ScreenModule.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)        1 2022-07-12 05:52:01.000000 perturb-tools-0.3.0/perturb_tools/_framework/__init__.py
-drwxrwx---   0 jr1025   (5074632) pinello  (10066)        0 2023-11-26 00:55:56.043803 perturb-tools-0.3.0/perturb_tools/_framework/_supporting_functions/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)        1 2022-07-12 19:59:13.000000 perturb-tools-0.3.0/perturb_tools/_framework/_supporting_functions/__init__.py
-drwxrwx---   0 jr1025   (5074632) pinello  (10066)        0 2023-11-26 00:55:56.052801 perturb-tools-0.3.0/perturb_tools/_framework/_supporting_functions/_data_reading/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)        0 2022-07-12 20:46:24.000000 perturb-tools-0.3.0/perturb_tools/_framework/_supporting_functions/_data_reading/__init__.py
-drwxrwx---   0 jr1025   (5074632) pinello  (10066)        0 2023-11-26 00:55:56.066712 perturb-tools-0.3.0/perturb_tools/_framework/_supporting_functions/_guides/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1972 2022-07-12 05:52:01.000000 perturb-tools-0.3.0/perturb_tools/_framework/_supporting_functions/_guides/_GuideAnnotationModule.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)        0 2022-07-12 20:45:35.000000 perturb-tools-0.3.0/perturb_tools/_framework/_supporting_functions/_guides/__init__.py
-drwxrwx---   0 jr1025   (5074632) pinello  (10066)        0 2023-11-26 00:55:56.133460 perturb-tools-0.3.0/perturb_tools/_framework/_supporting_functions/_guides/_supporting_functions/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)        0 2022-07-12 20:45:58.000000 perturb-tools-0.3.0/perturb_tools/_framework/_supporting_functions/_guides/_supporting_functions/__init__.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1546 2021-11-12 01:11:10.000000 perturb-tools-0.3.0/perturb_tools/_framework/_supporting_functions/_guides/_supporting_functions/_add_context_sequence_to_gene_dict.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1066 2021-11-12 01:11:10.000000 perturb-tools-0.3.0/perturb_tools/_framework/_supporting_functions/_guides/_supporting_functions/_add_guide_target_metadata.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     2136 2022-07-12 05:45:47.000000 perturb-tools-0.3.0/perturb_tools/_framework/_supporting_functions/_guides/_supporting_functions/_annotate_guide_position.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      233 2021-11-12 01:11:10.000000 perturb-tools-0.3.0/perturb_tools/_framework/_supporting_functions/_guides/_supporting_functions/_annotate_protospacer.py
--rw-r--r--   0 jr1025   (5074632) pinello  (10066)      353 2022-07-12 05:45:04.000000 perturb-tools-0.3.0/perturb_tools/_framework/_supporting_functions/_guides/_supporting_functions/_create_gene_dict.py
--rw-r--r--   0 jr1025   (5074632) pinello  (10066)     1083 2023-08-21 19:42:09.000000 perturb-tools-0.3.0/perturb_tools/_framework/_supporting_functions/_print_screen_object.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     3216 2021-11-08 18:28:06.000000 perturb-tools-0.3.0/perturb_tools/_framework/_supporting_functions/_read_write_poolQ.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)    56688 2022-07-12 05:52:01.000000 perturb-tools-0.3.0/perturb_tools/_framework/anndata_demo.ipynb
--rw-r--r--   0 jr1025   (5074632) pinello  (10066)    68228 2023-08-21 19:42:09.000000 perturb-tools-0.3.0/perturb_tools/_framework/screen_demo.ipynb
-drwxrwx---   0 jr1025   (5074632) pinello  (10066)        0 2023-11-26 00:55:56.152084 perturb-tools-0.3.0/perturb_tools/_normalization/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)       16 2021-11-08 18:28:06.000000 perturb-tools-0.3.0/perturb_tools/_normalization/README.md
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      100 2021-11-08 18:28:06.000000 perturb-tools-0.3.0/perturb_tools/_normalization/__init__.py
-drwxrwx---   0 jr1025   (5074632) pinello  (10066)        0 2023-11-26 00:55:56.165400 perturb-tools-0.3.0/perturb_tools/_normalization/_funcs/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)        0 2022-07-12 20:50:49.000000 perturb-tools-0.3.0/perturb_tools/_normalization/_funcs/__init__.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      598 2023-11-01 19:55:37.000000 perturb-tools-0.3.0/perturb_tools/_normalization/_funcs/_read_count_norm.py
-drwxrwx---   0 jr1025   (5074632) pinello  (10066)        0 2023-11-26 00:55:56.179539 perturb-tools-0.3.0/perturb_tools/_plotting/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     6148 2022-07-11 22:11:22.000000 perturb-tools-0.3.0/perturb_tools/_plotting/.DS_Store
--rw-r--r--   0 jr1025   (5074632) pinello  (10066)      335 2023-08-21 19:42:09.000000 perturb-tools-0.3.0/perturb_tools/_plotting/__init__.py
-drwxrwx---   0 jr1025   (5074632) pinello  (10066)        0 2023-11-26 00:55:56.248462 perturb-tools-0.3.0/perturb_tools/_plotting/_funcs/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)        0 2022-07-12 20:51:02.000000 perturb-tools-0.3.0/perturb_tools/_plotting/_funcs/__init__.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      725 2021-11-12 01:11:10.000000 perturb-tools-0.3.0/perturb_tools/_plotting/_funcs/_get_default_matplotlib_figure_width_height.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1655 2021-11-12 01:11:10.000000 perturb-tools-0.3.0/perturb_tools/_plotting/_funcs/_plot_correlation_heatmap.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1182 2022-07-11 22:11:22.000000 perturb-tools-0.3.0/perturb_tools/_plotting/_funcs/_plot_gene_exon.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     2473 2022-07-11 22:11:22.000000 perturb-tools-0.3.0/perturb_tools/_plotting/_funcs/_plot_guide_enrichment.py
--rw-r--r--   0 jr1025   (5074632) pinello  (10066)     1854 2023-08-21 19:42:09.000000 perturb-tools-0.3.0/perturb_tools/_plotting/_funcs/_plot_rep_consistency.py
--rw-r--r--   0 jr1025   (5074632) pinello  (10066)     1612 2023-08-21 19:42:09.000000 perturb-tools-0.3.0/perturb_tools/_plotting/_funcs/_plot_stats.py
--rw-r--r--   0 jr1025   (5074632) pinello  (10066)      265 2023-08-21 19:42:09.000000 perturb-tools-0.3.0/perturb_tools/_plotting/_funcs/_set_matplotlib_rc_params.py
-drwxrwx---   0 jr1025   (5074632) pinello  (10066)        0 2023-11-26 00:55:56.274281 perturb-tools-0.3.0/perturb_tools/_qc/
--rw-r--r--   0 jr1025   (5074632) pinello  (10066)       19 2023-08-21 19:42:09.000000 perturb-tools-0.3.0/perturb_tools/_qc/__init__.py
--rw-r--r--   0 jr1025   (5074632) pinello  (10066)     7497 2023-11-25 04:36:33.000000 perturb-tools-0.3.0/perturb_tools/_qc/qc.py
-drwxrwx---   0 jr1025   (5074632) pinello  (10066)        0 2023-11-26 00:55:56.290657 perturb-tools-0.3.0/perturb_tools/_readwrite/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)       48 2021-11-12 01:11:10.000000 perturb-tools-0.3.0/perturb_tools/_readwrite/README.md
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      316 2022-09-21 06:50:56.000000 perturb-tools-0.3.0/perturb_tools/_readwrite/__init__.py
-drwxrwx---   0 jr1025   (5074632) pinello  (10066)        0 2023-11-26 00:55:56.357243 perturb-tools-0.3.0/perturb_tools/_readwrite/_funcs/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)        1 2022-07-12 05:52:01.000000 perturb-tools-0.3.0/perturb_tools/_readwrite/_funcs/__init__.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      578 2021-11-12 01:11:10.000000 perturb-tools-0.3.0/perturb_tools/_readwrite/_funcs/_check_fix_file_extension.py
--rw-r--r--   0 jr1025   (5074632) pinello  (10066)    10406 2023-08-21 19:42:09.000000 perturb-tools-0.3.0/perturb_tools/_readwrite/_funcs/_read_screen_from_PoolQ.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     3201 2023-10-23 18:23:32.000000 perturb-tools-0.3.0/perturb_tools/_readwrite/_funcs/_read_screen_from_csvs.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1487 2022-07-11 22:11:22.000000 perturb-tools-0.3.0/perturb_tools/_readwrite/_funcs/_write_experiment_report_to_excel.py
--rw-r--r--   0 jr1025   (5074632) pinello  (10066)     1260 2023-08-21 19:42:09.000000 perturb-tools-0.3.0/perturb_tools/_readwrite/_funcs/_write_screen_to_csv.py
--rw-r--r--   0 jr1025   (5074632) pinello  (10066)     3182 2023-08-21 19:42:09.000000 perturb-tools-0.3.0/perturb_tools/_readwrite/_funcs/_write_screen_to_excel.py
-drwxrwx---   0 jr1025   (5074632) pinello  (10066)        0 2023-11-26 00:55:56.367673 perturb-tools-0.3.0/perturb_tools/_tools/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)        0 2022-07-12 20:51:40.000000 perturb-tools-0.3.0/perturb_tools/_tools/__init__.py
-drwxrwx---   0 jr1025   (5074632) pinello  (10066)        0 2023-11-26 00:55:56.390074 perturb-tools-0.3.0/perturb_tools/_utilities/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     6148 2022-07-11 22:11:22.000000 perturb-tools-0.3.0/perturb_tools/_utilities/.DS_Store
--rw-rw----   0 jr1025   (5074632) pinello  (10066)       21 2022-07-11 22:11:22.000000 perturb-tools-0.3.0/perturb_tools/_utilities/README.md
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      228 2022-07-11 22:11:22.000000 perturb-tools-0.3.0/perturb_tools/_utilities/__init__.py
-drwxrwx---   0 jr1025   (5074632) pinello  (10066)        0 2023-11-26 00:55:56.482455 perturb-tools-0.3.0/perturb_tools/_utilities/_funcs/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      909 2022-07-11 22:11:22.000000 perturb-tools-0.3.0/perturb_tools/_utilities/_funcs/_FileHandler.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     2148 2022-07-11 22:11:22.000000 perturb-tools-0.3.0/perturb_tools/_utilities/_funcs/_SequenceManipulation.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)        0 2022-07-12 20:51:50.000000 perturb-tools-0.3.0/perturb_tools/_utilities/_funcs/__init__.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      590 2022-07-11 22:11:22.000000 perturb-tools-0.3.0/perturb_tools/_utilities/_funcs/_fetch_chromosome_sequence.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1240 2022-07-12 05:52:01.000000 perturb-tools-0.3.0/perturb_tools/_utilities/_funcs/_flexible_mkdir.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1113 2022-07-11 22:11:22.000000 perturb-tools-0.3.0/perturb_tools/_utilities/_funcs/_get_chromosome_sequence.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1019 2022-07-11 22:11:22.000000 perturb-tools-0.3.0/perturb_tools/_utilities/_funcs/_get_gene_exons.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1410 2022-07-11 22:11:22.000000 perturb-tools-0.3.0/perturb_tools/_utilities/_funcs/_glob_dict.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      220 2022-07-11 22:11:22.000000 perturb-tools-0.3.0/perturb_tools/_utilities/_funcs/_scan_sequence_for_motif.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      341 2022-07-11 22:11:22.000000 perturb-tools-0.3.0/perturb_tools/_utilities/_funcs/_update_dict.py
--rw-r--r--   0 jr1025   (5074632) pinello  (10066)    75471 2023-08-21 19:42:09.000000 perturb-tools-0.3.0/perturb_tools/screen_demo.ipynb
-drwxrwx---   0 jr1025   (5074632) pinello  (10066)        0 2023-11-26 00:55:55.671520 perturb-tools-0.3.0/perturb_tools.egg-info/
--rw-r--r--   0 jr1025   (5074632) pinello  (10066)     3770 2023-11-26 00:55:54.000000 perturb-tools-0.3.0/perturb_tools.egg-info/PKG-INFO
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     5247 2023-11-26 00:55:55.000000 perturb-tools-0.3.0/perturb_tools.egg-info/SOURCES.txt
--rw-rw----   0 jr1025   (5074632) pinello  (10066)        1 2023-11-26 00:55:55.000000 perturb-tools-0.3.0/perturb_tools.egg-info/dependency_links.txt
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      118 2023-11-26 00:55:55.000000 perturb-tools-0.3.0/perturb_tools.egg-info/requires.txt
--rw-rw----   0 jr1025   (5074632) pinello  (10066)       14 2023-11-26 00:55:55.000000 perturb-tools-0.3.0/perturb_tools.egg-info/top_level.txt
--rw-rw----   0 jr1025   (5074632) pinello  (10066)        9 2021-11-12 05:53:34.000000 perturb-tools-0.3.0/requirements.txt
--rw-rw----   0 jr1025   (5074632) pinello  (10066)       38 2023-11-26 00:55:56.522041 perturb-tools-0.3.0/setup.cfg
--rw-r--r--   0 jr1025   (5074632) pinello  (10066)     1761 2023-11-25 02:51:13.000000 perturb-tools-0.3.0/setup.py
-drwxrwx---   0 jr1025   (5074632) pinello  (10066)        0 2023-11-26 00:55:56.498013 perturb-tools-0.3.0/tests/
--rw-r--r--   0 jr1025   (5074632) pinello  (10066)     1449 2023-08-21 19:42:09.000000 perturb-tools-0.3.0/tests/test_screen.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:42:03.985123 perturb_tools-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-12 18:42:03.985123 perturb_tools-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:42:03.973122 perturb_tools-0.3.1/perturb_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:42:03.973122 perturb_tools-0.3.1/perturb_tools/_arithmetic/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/_arithmetic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:42:03.977122 perturb_tools-0.3.1/perturb_tools/_arithmetic/_funcs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:42:03.977122 perturb_tools-0.3.1/perturb_tools/_arithmetic/_funcs/_LogFoldChange/
+-rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/_arithmetic/_funcs/_LogFoldChange/_LogFoldChange_Module.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/_arithmetic/_funcs/_LogFoldChange/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/_arithmetic/_funcs/_LogFoldChange/_calculate_log_fold_change.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/_arithmetic/_funcs/_SequenceManipulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/_arithmetic/_funcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/_arithmetic/_funcs/_log_fold_change.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:42:03.977122 perturb_tools-0.3.1/perturb_tools/_experimental_design/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/_experimental_design/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:42:03.977122 perturb_tools-0.3.1/perturb_tools/_experimental_design/_coding/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/_experimental_design/_coding/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:42:03.977122 perturb_tools-0.3.1/perturb_tools/_experimental_design/_coding/_funcs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/_experimental_design/_coding/_funcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/_experimental_design/_coding/_funcs/_plot_CDS.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:42:03.977122 perturb_tools-0.3.1/perturb_tools/_experimental_design/_funcs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/_experimental_design/_funcs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:42:03.977122 perturb_tools-0.3.1/perturb_tools/_experimental_design/_general/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/_experimental_design/_general/_GTF_Module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/_experimental_design/_general/_TargetModule.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/_experimental_design/_general/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/_experimental_design/_general/_add_region_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/_experimental_design/_general/_add_sgRNA_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/_experimental_design/_general/_annotate_guide_biochemistry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/_experimental_design/_general/_annotate_protospacer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/_experimental_design/_general/_get_chromosome_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/_experimental_design/_general/_get_screen_target_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6031 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/_experimental_design/_general/_identify_overlapping_fragments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/_experimental_design/_general/_make_guide_library_df.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5407 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/_experimental_design/_general/_query_region_for_PAM.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/_experimental_design/_general/_scan_for_BsmbI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/_experimental_design/_general/_widen_regions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:42:03.981123 perturb_tools-0.3.1/perturb_tools/_external_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/_external_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:42:03.981123 perturb_tools-0.3.1/perturb_tools/_framework/
+-rw-r--r--   0 runner    (1001) docker     (127)    13372 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/_framework/_ScreenModule.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/_framework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:42:03.981123 perturb_tools-0.3.1/perturb_tools/_framework/_supporting_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/_framework/_supporting_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/_framework/_supporting_functions/_print_screen_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/_framework/_supporting_functions/_read_write_poolQ.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:42:03.981123 perturb_tools-0.3.1/perturb_tools/_normalization/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/_normalization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:42:03.981123 perturb_tools-0.3.1/perturb_tools/_plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/_plotting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:42:03.981123 perturb_tools-0.3.1/perturb_tools/_qc/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/_qc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7258 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/_qc/qc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:42:03.981123 perturb_tools-0.3.1/perturb_tools/_readwrite/
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/_readwrite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:42:03.981123 perturb_tools-0.3.1/perturb_tools/_readwrite/_funcs/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/_readwrite/_funcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/_readwrite/_funcs/_check_fix_file_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10406 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/_readwrite/_funcs/_read_screen_from_PoolQ.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/_readwrite/_funcs/_write_experiment_report_to_excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/_readwrite/_funcs/_write_screen_to_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/_readwrite/_funcs/_write_screen_to_excel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:42:03.981123 perturb_tools-0.3.1/perturb_tools/_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:42:03.981123 perturb_tools-0.3.1/perturb_tools/_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/_utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:42:03.985123 perturb_tools-0.3.1/perturb_tools/_utilities/_funcs/
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/_utilities/_funcs/_FileHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/_utilities/_funcs/_SequenceManipulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/_utilities/_funcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/_utilities/_funcs/_fetch_chromosome_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/_utilities/_funcs/_flexible_mkdir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/_utilities/_funcs/_get_chromosome_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/_utilities/_funcs/_get_gene_exons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/_utilities/_funcs/_glob_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/_utilities/_funcs/_scan_sequence_for_motif.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/perturb_tools/_utilities/_funcs/_update_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:42:03.985123 perturb_tools-0.3.1/perturb_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-12 18:42:03.000000 perturb_tools-0.3.1/perturb_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-04-12 18:42:03.000000 perturb_tools-0.3.1/perturb_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 18:42:03.000000 perturb_tools-0.3.1/perturb_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-12 18:42:03.000000 perturb_tools-0.3.1/perturb_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-12 18:42:03.000000 perturb_tools-0.3.1/perturb_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 18:42:03.985123 perturb_tools-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:42:03.985123 perturb_tools-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-12 18:41:56.000000 perturb_tools-0.3.1/tests/test_screen.py
```

### Comparing `perturb-tools-0.3.0/LICENSE` & `perturb_tools-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `perturb-tools-0.3.0/PKG-INFO` & `perturb_tools-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perturb-tools
-Version: 0.3.0
+Version: 0.3.1
 Summary: perturb-tools - Analysis Framework for Pooled CRISPR Genome Editing Screens.
 Home-page: https://github.com/pinellolab/perturb-tools
 Author: ['Michael E. Vinyard - Harvard University - Massachussetts General Hospital - Broad Institute of MIT and Harvard', 'Jayoung K. Ryu - Harvard University - Massachussetts General Hospital - Broad Institute of MIT and Harvard']
 Author-email: mvinyard@broadinstitute.org, jayoung_ryu@g.harvard.edu
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `perturb-tools-0.3.0/README.md` & `perturb_tools-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `perturb-tools-0.3.0/perturb_tools/_arithmetic/_funcs/_LogFoldChange/_LogFoldChange_Module.py` & `perturb_tools-0.3.1/perturb_tools/_arithmetic/_funcs/_LogFoldChange/_LogFoldChange_Module.py`

 * *Files identical despite different names*

### Comparing `perturb-tools-0.3.0/perturb_tools/_arithmetic/_funcs/_LogFoldChange/_calculate_log_fold_change.py` & `perturb_tools-0.3.1/perturb_tools/_arithmetic/_funcs/_LogFoldChange/_calculate_log_fold_change.py`

 * *Files identical despite different names*

### Comparing `perturb-tools-0.3.0/perturb_tools/_arithmetic/_funcs/_SequenceManipulation.py` & `perturb_tools-0.3.1/perturb_tools/_arithmetic/_funcs/_SequenceManipulation.py`

 * *Files identical despite different names*

### Comparing `perturb-tools-0.3.0/perturb_tools/_experimental_design/_coding/_funcs/_plot_CDS.py` & `perturb_tools-0.3.1/perturb_tools/_experimental_design/_coding/_funcs/_plot_CDS.py`

 * *Files identical despite different names*

### Comparing `perturb-tools-0.3.0/perturb_tools/_experimental_design/_general/_TargetModule.py` & `perturb_tools-0.3.1/perturb_tools/_experimental_design/_general/_TargetModule.py`

 * *Files identical despite different names*

### Comparing `perturb-tools-0.3.0/perturb_tools/_experimental_design/_general/_add_sgRNA_context.py` & `perturb_tools-0.3.1/perturb_tools/_experimental_design/_general/_add_sgRNA_context.py`

 * *Files identical despite different names*

### Comparing `perturb-tools-0.3.0/perturb_tools/_experimental_design/_general/_annotate_guide_biochemistry.py` & `perturb_tools-0.3.1/perturb_tools/_experimental_design/_general/_annotate_guide_biochemistry.py`

 * *Files identical despite different names*

### Comparing `perturb-tools-0.3.0/perturb_tools/_experimental_design/_general/_annotate_protospacer.py` & `perturb_tools-0.3.1/perturb_tools/_experimental_design/_general/_annotate_protospacer.py`

 * *Files identical despite different names*

### Comparing `perturb-tools-0.3.0/perturb_tools/_experimental_design/_general/_get_chromosome_sequence.py` & `perturb_tools-0.3.1/perturb_tools/_experimental_design/_general/_get_chromosome_sequence.py`

 * *Files identical despite different names*

### Comparing `perturb-tools-0.3.0/perturb_tools/_experimental_design/_general/_get_screen_target_features.py` & `perturb_tools-0.3.1/perturb_tools/_experimental_design/_general/_get_screen_target_features.py`

 * *Files identical despite different names*

### Comparing `perturb-tools-0.3.0/perturb_tools/_experimental_design/_general/_identify_overlapping_fragments.py` & `perturb_tools-0.3.1/perturb_tools/_experimental_design/_general/_identify_overlapping_fragments.py`

 * *Files identical despite different names*

### Comparing `perturb-tools-0.3.0/perturb_tools/_experimental_design/_general/_make_guide_library_df.py` & `perturb_tools-0.3.1/perturb_tools/_experimental_design/_general/_make_guide_library_df.py`

 * *Files identical despite different names*

### Comparing `perturb-tools-0.3.0/perturb_tools/_experimental_design/_general/_query_region_for_PAM.py` & `perturb_tools-0.3.1/perturb_tools/_experimental_design/_general/_query_region_for_PAM.py`

 * *Files identical despite different names*

### Comparing `perturb-tools-0.3.0/perturb_tools/_experimental_design/_general/_scan_for_BsmbI.py` & `perturb_tools-0.3.1/perturb_tools/_experimental_design/_general/_scan_for_BsmbI.py`

 * *Files identical despite different names*

### Comparing `perturb-tools-0.3.0/perturb_tools/_framework/_ScreenModule.py` & `perturb_tools-0.3.1/perturb_tools/_framework/_ScreenModule.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # _ScreenModule.py
 __module_name__ = "_ScreenModule.py"
 __author__ = ", ".join(["Michael E. Vinyard", "Jayoung Kim Ryu"])
 __email__ = ", ".join(["vinyard@g.harvard.edu", "jayoung_ryu@g.harvard.edu"])
 
 import warnings
-from typing import Union, List
+from typing import Union
 
 import anndata as ad
 import numpy as np
 import pandas as pd
 from anndata import AnnData
 
 from .._arithmetic._funcs._log_fold_change import _log_fold_change
@@ -19,15 +19,15 @@
 from .._utilities._funcs._update_dict import _update_dict
 from ._supporting_functions._guides._GuideAnnotationModule import _annotate_sgRNAs
 from ._supporting_functions._print_screen_object import _print_screen_object
 
 
 class _Screen(AnnData):
     def __init__(self, X=None, guides=None, samples=None, *args, **kwargs):
-        super().__init__(X=X, dtype=X.dtype, obs=guides, var=samples, *args, **kwargs)
+        super().__init__(X=X, obs=guides, var=samples, *args, **kwargs)
 
     @classmethod
     def from_adata(cls, adata: ad.AnnData):
         return cls(
             (adata.X),
             guides=(adata.obs),
             samples=(adata.var),
@@ -98,14 +98,15 @@
             )
 
         _print_screen_object(self)
 
     def annotate_guides(
         self, genes, chrom, start, stop, annotations, DirectPairDict, ref_seq_path
     ):
+
         """
         Annotate sgRNA table.
 
         """
         self.guides = _annotate_sgRNAs(
             self.guides,
             genes,
@@ -132,14 +133,15 @@
         sample1,
         sample2,
         lognorm_counts_key="lognorm_counts",
         name=False,
         out_guides_suffix="lfc",
         return_result=False,
     ):
+
         """
         General module to calculate LFC across experimental conditions.
         """
         if "lognorm" not in lognorm_counts_key:
             warnings.warn(
                 "The layer specified must be log-normalized values using screen.log_norm()."
             )
@@ -183,92 +185,52 @@
                 self.guides[name] = dlfc
 
     def log_fold_change_reps(
         self,
         cond1,
         cond2,
         lognorm_counts_key="lognorm_counts",
-        rep_col: Union[str, List[str]] = "replicate",
+        rep_col="replicate",
         compare_col="sort",
         out_guides_suffix="lfc",
         keep_result=False,
-        ignore_missing=False,
     ):
-        """Get gRNA abundance LFC across conditions for each replicate.
-        ignore_missing: If True, does not raise Error when one of the conditions is missing for a replicate.
-        """
-        if isinstance(rep_col, str) and rep_col not in self.samples.columns:
+
+        if rep_col not in self.samples.columns:
             raise ValueError(f"{rep_col} not in samples features")
-        elif isinstance(rep_col, list):
-            for rc in rep_col:
-                if rc not in self.samples.columns:
-                    raise ValueError(f"{rc} not in samples features")
         if compare_col not in self.samples.columns:
             raise ValueError(f"{compare_col} not in samples features")
-        if (
-            cond1 not in self.samples[compare_col].tolist()
-            or cond2 not in self.samples[compare_col].tolist()
-        ):
-            raise ValueError(
-                f"{cond1} or {cond2} not in sample conditions {self.samples[compare_col]}"
-            )
 
         lfcs = []
+        for rep in self.samples[rep_col].unique():
+            cond1_idx = np.where(
+                (self.samples[rep_col] == rep) & (self.samples[compare_col] == cond1)
+            )[0]
+            cond2_idx = np.where(
+                (self.samples[rep_col] == rep) & (self.samples[compare_col] == cond2)
+            )[0]
 
-        if isinstance(rep_col, str):
-            lfc_rep_cols = self.samples[rep_col].unique().tolist()
-            unique_reps = self.samples[rep_col].unique()
-        else:
-            unique_reps = [
-                list(t)
-                for t in self.samples[rep_col].drop_duplicates().to_records(index=False)
-            ]
-            lfc_rep_cols = [
-                ".".join(list(map(str, rep_list))) for rep_list in unique_reps
-            ]
-        for rep in unique_reps:
-            if isinstance(rep_col, str):
-                cond1_idx = np.where(
-                    (self.samples[rep_col] == rep)
-                    & (self.samples[compare_col] == cond1)
-                )[0]
-                cond2_idx = np.where(
-                    (self.samples[rep_col] == rep)
-                    & (self.samples[compare_col] == cond2)
-                )[0]
-            elif isinstance(rep_col, list):
-                cond1_idx = np.where(
-                    (self.samples[rep_col] == rep).all(axis=1)
-                    & (self.samples[compare_col] == cond1)
-                )[0]
-                cond2_idx = np.where(
-                    (self.samples[rep_col] == rep).all(axis=1)
-                    & (self.samples[compare_col] == cond2)
-                )[0]
             if len(cond1_idx) != 1 or len(cond2_idx) != 1:
-                if not ignore_missing:
-                    raise ValueError(
-                        f"Conditions are not unique for each replicates ({rep_col} == {rep}) to be aggregated:\n{cond1}:{self.samples[cond1_idx]} or {cond2}:{self.samples[cond2_idx]}\n {self.samples}"
-                    )
-                else:
-                    lfc_rep_cols.pop(rep)
-                    continue
+                raise ValueError(
+                    "Conditions are not unique for each replicates to be aggregated."
+                )
 
             lfcs.append(
                 self.log_fold_change(
                     self.samples.index[cond1_idx].tolist()[0],
                     self.samples.index[cond2_idx].tolist()[0],
                     lognorm_counts_key=lognorm_counts_key,
                     return_result=True,
                 )
             )
 
         lfcs_array = np.concatenate(lfcs, axis=1)
         lfcs_df_columns = [
-            f"{s}.{cond1}_{cond2}.{out_guides_suffix}" for s in lfc_rep_cols
+            f"{s}.{cond1}_{cond2}.{out_guides_suffix}"
+            for s in self.samples[rep_col].unique()
         ]
         lfcs_df = pd.DataFrame(
             lfcs_array, index=self.guides.index, columns=lfcs_df_columns
         )
 
         if keep_result:
             self.guides[lfcs_df_columns] = lfcs_df
@@ -284,14 +246,15 @@
         compare_col="sort",
         out_guides_suffix="lfc",
         agg_fn="median",
         name=None,
         return_result=False,
         keep_per_replicate=False,
     ):
+
         lfcs_df = self.log_fold_change_reps(
             cond1,
             cond2,
             lognorm_counts_key=lognorm_counts_key,
             rep_col=agg_col,
             compare_col=compare_col,
             out_guides_suffix=out_guides_suffix,
@@ -357,14 +320,15 @@
             workbook_path,
             index,
             silent,
             include_uns,
         )
 
     def to_csv(self, out_path="CRISPR_screen"):
+
         """
 
         Write .csv files for each part of the screen. will eventually be replaced by something more native to AnnData.
 
         """
 
         _write_screen_to_csv(self, out_path)
```

### Comparing `perturb-tools-0.3.0/perturb_tools/_framework/_supporting_functions/_print_screen_object.py` & `perturb_tools-0.3.1/perturb_tools/_framework/_supporting_functions/_print_screen_object.py`

 * *Files identical despite different names*

### Comparing `perturb-tools-0.3.0/perturb_tools/_framework/_supporting_functions/_read_write_poolQ.py` & `perturb_tools-0.3.1/perturb_tools/_framework/_supporting_functions/_read_write_poolQ.py`

 * *Files identical despite different names*

### Comparing `perturb-tools-0.3.0/perturb_tools/_qc/qc.py` & `perturb_tools-0.3.1/perturb_tools/_qc/qc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy as np
 import numpy.ma as ma
+import scipy.stats
 import pandas as pd
 import matplotlib.pyplot as plt
 import seaborn as sns
 
 linestyles = ["solid", "dotted", "dashed", "dashdot"]
 
 
@@ -45,15 +46,15 @@
             f"Failed to calculate {method} correlation. Check if your matrix is constant or have no valid values."
         )
         return
     screen.varm[f"{prefix}corr_X"] = c
 
     # screen.samples[f"{prefix}mean_corr_X"] = screen.varm[f"{prefix}corr_X"].mean(0)
 
-    screen.samples[f"{prefix}median_corr_X"] = np.nanmedian(
+    screen.samples[f"{prefix}median_corr_X"] = np.median(
         screen.varm[f"{prefix}corr_X"], axis=0
     )
 
 
 def set_sample_correlation(screen, method="Pearson"):
     set_sample_correlation_guides(screen, screen.guides.index, prefix="", method=method)
 
@@ -100,25 +101,18 @@
     screen_subset = screen[guide_idx, :]
     lfcs = screen_subset.log_fold_change_reps(
         cond1=cond1, cond2=cond2, rep_col=rep_col, **kwargs
     )
     screen.uns["lfc"] = lfcs
     screen.uns["lfc_corr"] = corr_func_dict[method](lfcs)
     for i, col in enumerate(lfcs.columns):
-        rep = col.split(f".{cond1}_{cond2}", 1)[0]
-        if "." in rep:
-            rep = rep.split(".")
-        if isinstance(rep_col, str):
-            rep_idx = screen.samples[rep_col].astype(str) == rep
-        else:
-            rep_idx = (screen.samples[rep_col] == rep).all(axis=1)
+        rep = col.split(".")[0]
         screen.samples.loc[
-            rep_idx,
-            f"median_lfc_corr.{cond1}_{cond2}",
-        ] = np.nanmedian(np.delete(screen.uns["lfc_corr"][i, :], i))
+            screen.samples[rep_col] == rep, f"median_lfc_corr.{cond1}_{cond2}"
+        ] = np.nanmedian(screen.uns["lfc_corr"][i, :])
     fig, ax = plt.subplots(figsize=figsize)
     sns.heatmap(
         screen.uns["lfc_corr"],
         ax=ax,
         annot=True,
         xticklabels=lfcs.columns.map(lambda s: s.split(".")[0]),
         yticklabels=lfcs.columns.map(lambda s: s.split(".")[0]),
@@ -189,29 +183,30 @@
 ):
     """Obtain outlier guides.
     For each experimental condition in `samples`, find outlier guides that shows extreme counts compared to guides.
     Outlier guides are defined as those With MAD criteria (z>`mad_z_thres`) and has absolute RPM of `abs_RPM_thres`.
     """
 
     if "X_RPM" not in screen.layers:
-        screen.layers["X_RPM"] = (screen.X / screen.X.sum(axis=0) * 10e6).copy()
+        screen.layers["X_RPM"] = screen.X / screen.X.sum(axis=0) * 10e6
     aberr_dict = {}
 
     for cond in screen.samples[condit_col].unique():
         adata = screen[:, screen.samples[condit_col] == cond]
         median_p = np.nanmedian(adata.layers["X_RPM"].copy(), axis=1)
         aberr_guide_df_condit = []
+        aberr_idx_list = []
         for i, sample in enumerate(adata.samples.index):
             outlier_idx = np.where(
                 (adata.layers["X_RPM"][:, i] > median_p * mad_z_thres)
                 & (adata.layers["X_RPM"][:, i] > abs_RPM_thres)
             )[0]
             outlier_guides = adata.guides.iloc[outlier_idx, :].copy()
             outlier_guides["sample"] = adata.samples.index[i]
-            outlier_guides["RPM"] = adata.layers["X_RPM"].copy()[outlier_idx, i]
+            outlier_guides["RPM"] = adata.layers["X_RPM"][outlier_idx, i]
             aberr_guide_df_condit.append(outlier_guides[["sample", "RPM"]])
         aberr_dict[cond] = aberr_guide_df_condit
     aberr_guide_dfs = []
     for df in aberr_dict.values():
         aberr_guide_dfs.extend(df)
     if len(aberr_guide_dfs) == 0:
         return pd.DataFrame({"name": [], "sample": [], "RPM": []})
```

### Comparing `perturb-tools-0.3.0/perturb_tools/_readwrite/_funcs/_check_fix_file_extension.py` & `perturb_tools-0.3.1/perturb_tools/_readwrite/_funcs/_check_fix_file_extension.py`

 * *Files identical despite different names*

### Comparing `perturb-tools-0.3.0/perturb_tools/_readwrite/_funcs/_read_screen_from_PoolQ.py` & `perturb_tools-0.3.1/perturb_tools/_readwrite/_funcs/_read_screen_from_PoolQ.py`

 * *Files identical despite different names*

### Comparing `perturb-tools-0.3.0/perturb_tools/_readwrite/_funcs/_write_experiment_report_to_excel.py` & `perturb_tools-0.3.1/perturb_tools/_readwrite/_funcs/_write_experiment_report_to_excel.py`

 * *Files identical despite different names*

### Comparing `perturb-tools-0.3.0/perturb_tools/_readwrite/_funcs/_write_screen_to_csv.py` & `perturb_tools-0.3.1/perturb_tools/_readwrite/_funcs/_write_screen_to_csv.py`

 * *Files identical despite different names*

### Comparing `perturb-tools-0.3.0/perturb_tools/_readwrite/_funcs/_write_screen_to_excel.py` & `perturb_tools-0.3.1/perturb_tools/_readwrite/_funcs/_write_screen_to_excel.py`

 * *Files identical despite different names*

### Comparing `perturb-tools-0.3.0/perturb_tools/_utilities/_funcs/_FileHandler.py` & `perturb_tools-0.3.1/perturb_tools/_utilities/_funcs/_FileHandler.py`

 * *Files identical despite different names*

### Comparing `perturb-tools-0.3.0/perturb_tools/_utilities/_funcs/_SequenceManipulation.py` & `perturb_tools-0.3.1/perturb_tools/_utilities/_funcs/_SequenceManipulation.py`

 * *Files identical despite different names*

### Comparing `perturb-tools-0.3.0/perturb_tools/_utilities/_funcs/_fetch_chromosome_sequence.py` & `perturb_tools-0.3.1/perturb_tools/_utilities/_funcs/_fetch_chromosome_sequence.py`

 * *Files identical despite different names*

### Comparing `perturb-tools-0.3.0/perturb_tools/_utilities/_funcs/_flexible_mkdir.py` & `perturb_tools-0.3.1/perturb_tools/_utilities/_funcs/_flexible_mkdir.py`

 * *Files identical despite different names*

### Comparing `perturb-tools-0.3.0/perturb_tools/_utilities/_funcs/_get_chromosome_sequence.py` & `perturb_tools-0.3.1/perturb_tools/_utilities/_funcs/_get_chromosome_sequence.py`

 * *Files identical despite different names*

### Comparing `perturb-tools-0.3.0/perturb_tools/_utilities/_funcs/_get_gene_exons.py` & `perturb_tools-0.3.1/perturb_tools/_utilities/_funcs/_get_gene_exons.py`

 * *Files identical despite different names*

### Comparing `perturb-tools-0.3.0/perturb_tools/_utilities/_funcs/_glob_dict.py` & `perturb_tools-0.3.1/perturb_tools/_utilities/_funcs/_glob_dict.py`

 * *Files identical despite different names*

### Comparing `perturb-tools-0.3.0/perturb_tools.egg-info/PKG-INFO` & `perturb_tools-0.3.1/perturb_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perturb-tools
-Version: 0.3.0
+Version: 0.3.1
 Summary: perturb-tools - Analysis Framework for Pooled CRISPR Genome Editing Screens.
 Home-page: https://github.com/pinellolab/perturb-tools
 Author: ['Michael E. Vinyard - Harvard University - Massachussetts General Hospital - Broad Institute of MIT and Harvard', 'Jayoung K. Ryu - Harvard University - Massachussetts General Hospital - Broad Institute of MIT and Harvard']
 Author-email: mvinyard@broadinstitute.org, jayoung_ryu@g.harvard.edu
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `perturb-tools-0.3.0/setup.py` & `perturb_tools-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import re
 import os
 import sys
 
 
 setup(
     name="perturb-tools",
-    version="0.3.0",
+    version="0.3.1",
     python_requires=">3.7.0",
     author=[
         "Michael E. Vinyard - Harvard University - Massachussetts General Hospital - Broad Institute of MIT and Harvard",
         "Jayoung K. Ryu - Harvard University - Massachussetts General Hospital - Broad Institute of MIT and Harvard",
     ],
     author_email="mvinyard@broadinstitute.org, jayoung_ryu@g.harvard.edu",
     url="https://github.com/pinellolab/perturb-tools",
```

### Comparing `perturb-tools-0.3.0/tests/test_screen.py` & `perturb_tools-0.3.1/tests/test_screen.py`

 * *Files identical despite different names*

