# Comparing `tmp/liana-1.0.5.tar.gz` & `tmp/liana-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liana-1.0.5.tar", max compression
+gzip compressed data, was "liana-1.1.0.tar", max compression
```

## Comparing `liana-1.0.5.tar` & `liana-1.1.0.tar`

### file list

```diff
@@ -1,93 +1,96 @@
--rw-r--r--   0        0        0    35149 2022-09-22 13:22:13.706956 liana-1.0.5/LICENSE
--rw-r--r--   0        0        0     2667 2024-03-05 14:34:47.030454 liana-1.0.5/README.md
--rw-r--r--   0        0        0      411 2024-02-25 13:50:51.564250 liana-1.0.5/liana/__init__.py
--rw-r--r--   0        0        0     2108 2024-02-25 13:50:51.564250 liana-1.0.5/liana/_constants.py
--rw-r--r--   0        0        0     8670 2024-01-02 14:41:49.557050 liana-1.0.5/liana/_docs.py
--rw-r--r--   0        0        0      984 2023-10-11 06:41:18.553363 liana-1.0.5/liana/_logging.py
--rw-r--r--   0        0        0     1976 2024-02-25 13:50:51.564250 liana-1.0.5/liana/method/__init__.py
--rw-r--r--   0        0        0       96 2024-01-02 14:41:52.277014 liana-1.0.5/liana/method/_pipe_utils/__init__.py
--rw-r--r--   0        0        0     5158 2023-11-06 12:56:19.933679 liana-1.0.5/liana/method/_pipe_utils/_aggregate.py
--rw-r--r--   0        0        0     1619 2024-02-25 13:50:51.564250 liana-1.0.5/liana/method/_pipe_utils/_common.py
--rw-r--r--   0        0        0     4478 2024-01-02 14:41:49.557050 liana-1.0.5/liana/method/_pipe_utils/_get_mean_perms.py
--rw-r--r--   0        0        0     9152 2024-01-02 14:41:49.557050 liana-1.0.5/liana/method/_pipe_utils/_pre.py
--rw-r--r--   0        0        0       60 2023-11-06 12:56:19.937679 liana-1.0.5/liana/method/fun/__init__.py
--rw-r--r--   0        0        0     9210 2024-02-25 13:50:51.568250 liana-1.0.5/liana/method/fun/_causalnet.py
--rw-r--r--   0        0        0     9782 2024-01-04 07:36:04.092801 liana-1.0.5/liana/method/sc/_Method.py
--rw-r--r--   0        0        0      336 2024-02-25 13:50:51.568250 liana-1.0.5/liana/method/sc/__init__.py
--rw-r--r--   0        0        0     1915 2024-01-02 14:41:49.557050 liana-1.0.5/liana/method/sc/_cellchat.py
--rw-r--r--   0        0        0     1897 2024-01-02 14:41:49.557050 liana-1.0.5/liana/method/sc/_cellphonedb.py
--rw-r--r--   0        0        0     1638 2023-11-06 12:56:19.937679 liana-1.0.5/liana/method/sc/_connectome.py
--rw-r--r--   0        0        0     1558 2023-12-05 07:31:15.866959 liana-1.0.5/liana/method/sc/_geometric_mean.py
--rw-r--r--   0        0        0    19466 2024-02-25 13:50:51.568250 liana-1.0.5/liana/method/sc/_liana_pipe.py
--rw-r--r--   0        0        0     1181 2023-11-07 09:15:10.387722 liana-1.0.5/liana/method/sc/_logfc.py
--rw-r--r--   0        0        0     1376 2024-02-25 13:50:51.568250 liana-1.0.5/liana/method/sc/_natmi.py
--rw-r--r--   0        0        0     6864 2024-01-02 14:41:49.557050 liana-1.0.5/liana/method/sc/_rank_aggregate.py
--rw-r--r--   0        0        0     1059 2024-02-25 13:50:51.568250 liana-1.0.5/liana/method/sc/_scseqcomm.py
--rw-r--r--   0        0        0     1499 2023-09-24 13:38:26.386870 liana-1.0.5/liana/method/sc/_singlecellsignalr.py
--rw-r--r--   0        0        0    16160 2024-01-02 14:41:49.557050 liana-1.0.5/liana/method/sp/_Misty.py
--rw-r--r--   0        0        0    12184 2024-02-25 13:50:51.568250 liana-1.0.5/liana/method/sp/_SpatialBivariate.py
--rw-r--r--   0        0        0      141 2023-11-07 09:15:10.387722 liana-1.0.5/liana/method/sp/__init__.py
--rw-r--r--   0        0        0     7298 2024-01-02 08:34:17.346248 liana-1.0.5/liana/method/sp/_bivariate_funs.py
--rw-r--r--   0        0        0     3221 2024-02-25 13:50:51.568250 liana-1.0.5/liana/method/sp/_lr_bivar.py
--rw-r--r--   0        0        0    10823 2023-11-15 09:29:11.500596 liana-1.0.5/liana/method/sp/_misty_constructs.py
--rw-r--r--   0        0        0    13432 2024-02-25 13:50:51.568250 liana-1.0.5/liana/method/sp/_spatial_pipe.py
--rw-r--r--   0        0        0      267 2024-02-25 13:50:51.568250 liana-1.0.5/liana/multi/__init__.py
--rw-r--r--   0        0        0     4032 2024-02-25 13:50:51.568250 liana-1.0.5/liana/multi/_nmf.py
--rw-r--r--   0        0        0     6941 2024-02-25 13:50:51.568250 liana-1.0.5/liana/multi/df_to_lr.py
--rw-r--r--   0        0        0    14203 2024-02-25 13:50:51.568250 liana-1.0.5/liana/multi/to_mudata.py
--rw-r--r--   0        0        0     4286 2024-02-25 13:50:51.568250 liana-1.0.5/liana/multi/to_tensor_c2c.py
--rw-r--r--   0        0        0      196 2023-11-06 12:56:19.941680 liana-1.0.5/liana/plotting/__init__.py
--rw-r--r--   0        0        0     4026 2024-01-11 12:36:30.484599 liana-1.0.5/liana/plotting/_common.py
--rw-r--r--   0        0        0     1760 2023-11-07 09:15:10.391722 liana-1.0.5/liana/plotting/_connectivity_plot.py
--rw-r--r--   0        0        0     7243 2024-01-02 14:41:49.561050 liana-1.0.5/liana/plotting/_dotplot.py
--rw-r--r--   0        0        0     7170 2024-02-25 13:50:51.572250 liana-1.0.5/liana/plotting/_misty_plots.py
--rw-r--r--   0        0        0     4667 2024-02-25 13:50:51.572250 liana-1.0.5/liana/plotting/_tileplot.py
--rw-r--r--   0        0        0      303 2024-02-25 13:50:51.572250 liana-1.0.5/liana/resource/__init__.py
--rw-r--r--   0        0        0     4760 2024-02-25 13:50:51.572250 liana-1.0.5/liana/resource/_reassemble_complexes.py
--rw-r--r--   0        0        0     5542 2024-02-25 13:50:51.572250 liana-1.0.5/liana/resource/_resource_utils.py
--rw-r--r--   0        0        0     7732 2024-02-25 13:50:51.572250 liana-1.0.5/liana/resource/get_metalinks.py
--rwxr-xr-x   0        0        0  2004583 2024-01-03 12:47:37.202135 liana-1.0.5/liana/resource/omni_resource.csv
--rw-r--r--   0        0        0     2929 2024-02-25 13:50:51.572250 liana-1.0.5/liana/resource/select_resource.py
--rw-r--r--   0        0        0      301 2023-10-31 12:22:28.754376 liana-1.0.5/liana/testing/__init__.py
--rw-r--r--   0        0        0     1420 2024-02-25 13:50:51.572250 liana-1.0.5/liana/testing/_sample_anndata.py
--rw-r--r--   0        0        0      584 2023-11-06 12:56:19.941680 liana-1.0.5/liana/testing/_sample_dea.py
--rw-r--r--   0        0        0     1207 2023-11-06 12:56:19.941680 liana-1.0.5/liana/testing/_sample_lrs.py
--rw-r--r--   0        0        0      926 2023-11-06 12:56:19.941680 liana-1.0.5/liana/testing/_sample_misty.py
--rw-r--r--   0        0        0     1726 2023-11-06 12:56:19.945680 liana-1.0.5/liana/testing/datasets.py
--rw-r--r--   0        0        0        0 2022-10-10 17:40:32.066002 liana-1.0.5/liana/tests/__init__.py
--rwxr-xr-x   0        0        0   188646 2024-02-25 13:50:51.576250 liana-1.0.5/liana/tests/data/aggregate_rank_rest.csv
--rwxr-xr-x   0        0        0   360667 2024-02-25 13:50:51.576250 liana-1.0.5/liana/tests/data/all_defaults.csv
--rwxr-xr-x   0        0        0  1240013 2024-02-25 13:50:51.588250 liana-1.0.5/liana/tests/data/not_defaults.csv
--rwxr-xr-x   0        0        0   627053 2023-10-13 08:35:25.822208 liana-1.0.5/liana/tests/data/synthetic.h5ad
--rw-r--r--   0        0        0        0 2024-02-21 15:25:52.489019 liana-1.0.5/liana/tests/disease
--rw-r--r--   0        0        0     4256 2024-02-25 13:50:51.592250 liana-1.0.5/liana/tests/test_bivar.py
--rw-r--r--   0        0        0     2333 2023-10-13 08:35:25.822208 liana-1.0.5/liana/tests/test_bivariate_funs.py
--rw-r--r--   0        0        0     1979 2024-02-06 08:51:19.104460 liana-1.0.5/liana/tests/test_causalnet.py
--rw-r--r--   0        0        0     1550 2023-11-06 12:56:19.945680 liana-1.0.5/liana/tests/test_converters.py
--rw-r--r--   0        0        0     1151 2024-02-25 13:50:51.592250 liana-1.0.5/liana/tests/test_generate_lr.py
--rw-r--r--   0        0        0     2866 2024-01-02 14:41:49.581049 liana-1.0.5/liana/tests/test_get_mean_perms.py
--rw-r--r--   0        0        0     2023 2024-01-02 14:41:49.581049 liana-1.0.5/liana/tests/test_interpolate.py
--rw-r--r--   0        0        0     4637 2024-02-25 13:50:51.592250 liana-1.0.5/liana/tests/test_liana_pipe.py
--rw-r--r--   0        0        0     2212 2024-02-25 13:50:51.592250 liana-1.0.5/liana/tests/test_lr_bivar.py
--rw-r--r--   0        0        0     1312 2024-02-25 13:50:51.592250 liana-1.0.5/liana/tests/test_metalinksdb.py
--rw-r--r--   0        0        0     5375 2024-02-25 13:50:51.596249 liana-1.0.5/liana/tests/test_misty.py
--rw-r--r--   0        0        0     1681 2024-01-02 14:41:49.581049 liana-1.0.5/liana/tests/test_misty_plots.py
--rw-r--r--   0        0        0     5973 2023-11-07 09:15:10.391722 liana-1.0.5/liana/tests/test_multi.py
--rw-r--r--   0        0        0     1754 2024-01-02 14:41:49.581049 liana-1.0.5/liana/tests/test_multi_dea.py
--rw-r--r--   0        0        0     1277 2024-02-25 13:50:51.596249 liana-1.0.5/liana/tests/test_multi_nmf.py
--rw-r--r--   0        0        0     2577 2024-01-02 14:41:49.581049 liana-1.0.5/liana/tests/test_plotting.py
--rw-r--r--   0        0        0     2061 2023-10-13 06:13:31.232542 liana-1.0.5/liana/tests/test_pre.py
--rw-r--r--   0        0        0     3202 2024-02-25 13:50:51.596249 liana-1.0.5/liana/tests/test_rank_aggregate.py
--rw-r--r--   0        0        0     8301 2024-02-25 13:50:51.596249 liana-1.0.5/liana/tests/test_sc_methods.py
--rw-r--r--   0        0        0     2359 2024-02-25 13:50:51.596249 liana-1.0.5/liana/tests/test_select_resource.py
--rw-r--r--   0        0        0     4643 2024-02-25 13:50:51.596249 liana-1.0.5/liana/tests/test_spatial_utils.py
--rw-r--r--   0        0        0      417 2024-01-02 14:41:49.581049 liana-1.0.5/liana/utils/__init__.py
--rw-r--r--   0        0        0     3611 2023-11-07 09:15:10.391722 liana-1.0.5/liana/utils/_getters.py
--rw-r--r--   0        0        0     2221 2024-01-02 14:41:49.581049 liana-1.0.5/liana/utils/interpolate_adata.py
--rw-r--r--   0        0        0     2258 2024-01-10 09:10:17.424395 liana-1.0.5/liana/utils/mdata_to_anndata.py
--rw-r--r--   0        0        0     1477 2024-01-10 09:10:12.848404 liana-1.0.5/liana/utils/obsm_to_adata.py
--rw-r--r--   0        0        0     2086 2023-11-06 12:56:19.949680 liana-1.0.5/liana/utils/query_bandwidth.py
--rw-r--r--   0        0        0     5619 2024-02-25 13:50:51.596249 liana-1.0.5/liana/utils/spatial_neighbors.py
--rw-r--r--   0        0        0     1341 2023-11-06 12:56:19.949680 liana-1.0.5/liana/utils/transform.py
--rw-r--r--   0        0        0     1987 2024-02-25 13:50:51.600249 liana-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     4677 1970-01-01 00:00:00.000000 liana-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-09-22 13:22:13.706956 liana-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2667 2024-03-25 09:18:41.388773 liana-1.1.0/README.md
+-rw-r--r--   0        0        0      411 2024-04-12 09:05:15.061801 liana-1.1.0/liana/__init__.py
+-rw-r--r--   0        0        0     2108 2024-02-25 13:50:51.564250 liana-1.1.0/liana/_constants.py
+-rw-r--r--   0        0        0     9200 2024-04-12 09:05:15.061801 liana-1.1.0/liana/_docs.py
+-rw-r--r--   0        0        0      984 2024-04-05 08:51:49.271659 liana-1.1.0/liana/_logging.py
+-rw-r--r--   0        0        0     1969 2024-04-12 09:05:15.061801 liana-1.1.0/liana/method/__init__.py
+-rw-r--r--   0        0        0       96 2024-01-02 14:41:52.277014 liana-1.1.0/liana/method/_pipe_utils/__init__.py
+-rw-r--r--   0        0        0     5158 2023-11-06 12:56:19.933679 liana-1.1.0/liana/method/_pipe_utils/_aggregate.py
+-rw-r--r--   0        0        0     1619 2024-04-12 09:05:15.061801 liana-1.1.0/liana/method/_pipe_utils/_common.py
+-rw-r--r--   0        0        0     4478 2024-01-02 14:41:49.557050 liana-1.1.0/liana/method/_pipe_utils/_get_mean_perms.py
+-rw-r--r--   0        0        0     9190 2024-04-12 09:05:15.061801 liana-1.1.0/liana/method/_pipe_utils/_pre.py
+-rw-r--r--   0        0        0       60 2023-11-06 12:56:19.937679 liana-1.1.0/liana/method/fun/__init__.py
+-rw-r--r--   0        0        0    10524 2024-04-12 09:05:15.065801 liana-1.1.0/liana/method/fun/_causalnet.py
+-rw-r--r--   0        0        0     9782 2024-01-04 07:36:04.092801 liana-1.1.0/liana/method/sc/_Method.py
+-rw-r--r--   0        0        0      336 2024-02-25 13:50:51.568250 liana-1.1.0/liana/method/sc/__init__.py
+-rw-r--r--   0        0        0     1915 2024-01-02 14:41:49.557050 liana-1.1.0/liana/method/sc/_cellchat.py
+-rw-r--r--   0        0        0     1897 2024-01-02 14:41:49.557050 liana-1.1.0/liana/method/sc/_cellphonedb.py
+-rw-r--r--   0        0        0     1638 2023-11-06 12:56:19.937679 liana-1.1.0/liana/method/sc/_connectome.py
+-rw-r--r--   0        0        0     1558 2023-12-05 07:31:15.866959 liana-1.1.0/liana/method/sc/_geometric_mean.py
+-rw-r--r--   0        0        0    19466 2024-02-25 13:50:51.568250 liana-1.1.0/liana/method/sc/_liana_pipe.py
+-rw-r--r--   0        0        0     1181 2023-11-07 09:15:10.387722 liana-1.1.0/liana/method/sc/_logfc.py
+-rw-r--r--   0        0        0     1376 2024-02-25 13:50:51.568250 liana-1.1.0/liana/method/sc/_natmi.py
+-rw-r--r--   0        0        0     6864 2024-01-02 14:41:49.557050 liana-1.1.0/liana/method/sc/_rank_aggregate.py
+-rw-r--r--   0        0        0     1059 2024-02-25 13:50:51.568250 liana-1.1.0/liana/method/sc/_scseqcomm.py
+-rw-r--r--   0        0        0     1499 2023-09-24 13:38:26.386870 liana-1.1.0/liana/method/sc/_singlecellsignalr.py
+-rw-r--r--   0        0        0      284 2024-04-12 09:05:15.065801 liana-1.1.0/liana/method/sp/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 09:05:15.065801 liana-1.1.0/liana/method/sp/_bivariate/__init__.py
+-rw-r--r--   0        0        0     4698 2024-04-12 09:05:15.065801 liana-1.1.0/liana/method/sp/_bivariate/_global_functions.py
+-rw-r--r--   0        0        0    12256 2024-04-12 09:05:15.065801 liana-1.1.0/liana/method/sp/_bivariate/_local_functions.py
+-rw-r--r--   0        0        0    15729 2024-04-12 09:05:15.065801 liana-1.1.0/liana/method/sp/_bivariate/_spatial_bivariate.py
+-rw-r--r--   0        0        0    15023 2024-04-12 09:05:15.065801 liana-1.1.0/liana/method/sp/_misty/_Misty.py
+-rw-r--r--   0        0        0        0 2024-04-12 09:05:15.065801 liana-1.1.0/liana/method/sp/_misty/__init__.py
+-rw-r--r--   0        0        0    10823 2024-04-12 09:05:15.065801 liana-1.1.0/liana/method/sp/_misty/_misty_constructs.py
+-rw-r--r--   0        0        0     3621 2024-04-12 09:05:15.065801 liana-1.1.0/liana/method/sp/_misty/_single_view_models.py
+-rw-r--r--   0        0        0     1682 2024-04-12 09:05:15.065801 liana-1.1.0/liana/method/sp/_utils.py
+-rw-r--r--   0        0        0      267 2024-02-25 13:50:51.568250 liana-1.1.0/liana/multi/__init__.py
+-rw-r--r--   0        0        0     4034 2024-04-12 09:05:15.065801 liana-1.1.0/liana/multi/_nmf.py
+-rw-r--r--   0        0        0     7140 2024-04-12 09:05:15.065801 liana-1.1.0/liana/multi/df_to_lr.py
+-rw-r--r--   0        0        0    14204 2024-04-12 09:05:15.065801 liana-1.1.0/liana/multi/to_mudata.py
+-rw-r--r--   0        0        0     4286 2024-02-25 13:50:51.568250 liana-1.1.0/liana/multi/to_tensor_c2c.py
+-rw-r--r--   0        0        0      196 2023-11-06 12:56:19.941680 liana-1.1.0/liana/plotting/__init__.py
+-rw-r--r--   0        0        0     4026 2024-01-11 12:36:30.484599 liana-1.1.0/liana/plotting/_common.py
+-rw-r--r--   0        0        0     1760 2023-11-07 09:15:10.391722 liana-1.1.0/liana/plotting/_connectivity_plot.py
+-rw-r--r--   0        0        0     7243 2024-01-02 14:41:49.561050 liana-1.1.0/liana/plotting/_dotplot.py
+-rw-r--r--   0        0        0     7170 2024-02-25 13:50:51.572250 liana-1.1.0/liana/plotting/_misty_plots.py
+-rw-r--r--   0        0        0     4667 2024-02-25 13:50:51.572250 liana-1.1.0/liana/plotting/_tileplot.py
+-rw-r--r--   0        0        0      303 2024-04-09 07:27:00.642648 liana-1.1.0/liana/resource/__init__.py
+-rw-r--r--   0        0        0     4760 2024-02-25 13:50:51.572250 liana-1.1.0/liana/resource/_reassemble_complexes.py
+-rw-r--r--   0        0        0     5542 2024-02-25 13:50:51.572250 liana-1.1.0/liana/resource/_resource_utils.py
+-rw-r--r--   0        0        0     7732 2024-04-09 07:25:45.471128 liana-1.1.0/liana/resource/get_metalinks.py
+-rwxr-xr-x   0        0        0  2004583 2024-01-03 12:47:37.202135 liana-1.1.0/liana/resource/omni_resource.csv
+-rw-r--r--   0        0        0     2929 2024-02-25 13:50:51.572250 liana-1.1.0/liana/resource/select_resource.py
+-rw-r--r--   0        0        0      301 2023-10-31 12:22:28.754376 liana-1.1.0/liana/testing/__init__.py
+-rw-r--r--   0        0        0     2783 2024-04-12 09:05:15.081801 liana-1.1.0/liana/testing/_sample_anndata.py
+-rw-r--r--   0        0        0      584 2023-11-06 12:56:19.941680 liana-1.1.0/liana/testing/_sample_dea.py
+-rw-r--r--   0        0        0     1206 2024-04-12 09:05:15.081801 liana-1.1.0/liana/testing/_sample_lrs.py
+-rw-r--r--   0        0        0      926 2023-11-06 12:56:19.941680 liana-1.1.0/liana/testing/_sample_misty.py
+-rw-r--r--   0        0        0      380 2024-04-12 09:05:15.081801 liana-1.1.0/liana/testing/_sample_resource.py
+-rw-r--r--   0        0        0     1726 2023-11-06 12:56:19.945680 liana-1.1.0/liana/testing/datasets.py
+-rw-r--r--   0        0        0        0 2022-10-10 17:40:32.066002 liana-1.1.0/liana/tests/__init__.py
+-rwxr-xr-x   0        0        0   188646 2024-02-25 13:50:51.576250 liana-1.1.0/liana/tests/data/aggregate_rank_rest.csv
+-rwxr-xr-x   0        0        0   360667 2024-02-25 13:50:51.576250 liana-1.1.0/liana/tests/data/all_defaults.csv
+-rwxr-xr-x   0        0        0  1240013 2024-02-25 13:50:51.588250 liana-1.1.0/liana/tests/data/not_defaults.csv
+-rwxr-xr-x   0        0        0   627053 2023-10-13 08:35:25.822208 liana-1.1.0/liana/tests/data/synthetic.h5ad
+-rw-r--r--   0        0        0 16830464 2024-04-12 09:08:03.093124 liana-1.1.0/liana/tests/metalinksdb.db
+-rw-r--r--   0        0        0     9308 2024-04-12 09:05:15.081801 liana-1.1.0/liana/tests/test_bivar.py
+-rw-r--r--   0        0        0     2344 2024-04-12 09:05:15.081801 liana-1.1.0/liana/tests/test_bivariate_funs.py
+-rw-r--r--   0        0        0     2008 2024-04-12 09:05:15.081801 liana-1.1.0/liana/tests/test_causalnet.py
+-rw-r--r--   0        0        0     1550 2023-11-06 12:56:19.945680 liana-1.1.0/liana/tests/test_converters.py
+-rw-r--r--   0        0        0     1151 2024-02-25 13:50:51.592250 liana-1.1.0/liana/tests/test_generate_lr.py
+-rw-r--r--   0        0        0     2866 2024-01-02 14:41:49.581049 liana-1.1.0/liana/tests/test_get_mean_perms.py
+-rw-r--r--   0        0        0     2023 2024-01-02 14:41:49.581049 liana-1.1.0/liana/tests/test_interpolate.py
+-rw-r--r--   0        0        0     4637 2024-02-25 13:50:51.592250 liana-1.1.0/liana/tests/test_liana_pipe.py
+-rw-r--r--   0        0        0     1312 2024-02-25 13:50:51.592250 liana-1.1.0/liana/tests/test_metalinksdb.py
+-rw-r--r--   0        0        0     6851 2024-04-12 09:05:15.081801 liana-1.1.0/liana/tests/test_misty.py
+-rw-r--r--   0        0        0     1681 2024-01-02 14:41:49.581049 liana-1.1.0/liana/tests/test_misty_plots.py
+-rw-r--r--   0        0        0     5973 2023-11-07 09:15:10.391722 liana-1.1.0/liana/tests/test_multi.py
+-rw-r--r--   0        0        0     1754 2024-04-12 07:53:29.775783 liana-1.1.0/liana/tests/test_multi_dea.py
+-rw-r--r--   0        0        0     1277 2024-02-25 13:50:51.596249 liana-1.1.0/liana/tests/test_multi_nmf.py
+-rw-r--r--   0        0        0     2577 2024-01-02 14:41:49.581049 liana-1.1.0/liana/tests/test_plotting.py
+-rw-r--r--   0        0        0     2061 2023-10-13 06:13:31.232542 liana-1.1.0/liana/tests/test_pre.py
+-rw-r--r--   0        0        0     3202 2024-02-25 13:50:51.596249 liana-1.1.0/liana/tests/test_rank_aggregate.py
+-rw-r--r--   0        0        0     8301 2024-02-25 13:50:51.596249 liana-1.1.0/liana/tests/test_sc_methods.py
+-rw-r--r--   0        0        0     2359 2024-02-25 13:50:51.596249 liana-1.1.0/liana/tests/test_select_resource.py
+-rw-r--r--   0        0        0     4527 2024-04-12 09:05:15.081801 liana-1.1.0/liana/tests/test_spatial_utils.py
+-rw-r--r--   0        0        0      417 2024-01-02 14:41:49.581049 liana-1.1.0/liana/utils/__init__.py
+-rw-r--r--   0        0        0     3611 2023-11-07 09:15:10.391722 liana-1.1.0/liana/utils/_getters.py
+-rw-r--r--   0        0        0     2221 2024-01-02 14:41:49.581049 liana-1.1.0/liana/utils/interpolate_adata.py
+-rw-r--r--   0        0        0     2258 2024-01-10 09:10:17.424395 liana-1.1.0/liana/utils/mdata_to_anndata.py
+-rw-r--r--   0        0        0     1477 2024-01-10 09:10:12.848404 liana-1.1.0/liana/utils/obsm_to_adata.py
+-rw-r--r--   0        0        0     2174 2024-04-12 09:05:15.081801 liana-1.1.0/liana/utils/query_bandwidth.py
+-rw-r--r--   0        0        0     5619 2024-02-25 13:50:51.596249 liana-1.1.0/liana/utils/spatial_neighbors.py
+-rw-r--r--   0        0        0     1341 2023-11-06 12:56:19.949680 liana-1.1.0/liana/utils/transform.py
+-rw-r--r--   0        0        0     2070 2024-04-12 09:05:15.089801 liana-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4728 1970-01-01 00:00:00.000000 liana-1.1.0/PKG-INFO
```

### Comparing `liana-1.0.5/LICENSE` & `liana-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/README.md` & `liana-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/liana/_constants.py` & `liana-1.1.0/liana/_constants.py`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/liana/_docs.py` & `liana-1.1.0/liana/_docs.py`

 * *Files 6% similar despite different names*

```diff
@@ -161,17 +161,21 @@
 spatial_key
     Key in `adata.obsm` that contains the spatial coordinates. Default is `'spatial'`."""
 
 _connectivity_key = """\
 connectivity_key
     Key in `adata.obsp` that contains the spatial connectivity matrix. Default is `'spatial_connectivity'`. """
 
-_function_name = """\
-function_name
-    Name of the function to use for the analysis."""
+_local_name = """\
+local_name
+    Name of the local function to use for the analysis. Passing `None` will return only the Global scores."""
+
+_global_name = """\
+global_name
+    Name or names (list) of the global function(s) to use for the analysis. Passing `None` will not calculate any global scores"""
 
 _positive_only = """\
 positive_only
     Whether to mask non-positive interactions."""
 
 _add_categories = """\
 add_categories
@@ -181,14 +185,22 @@
 x_mod
     Name of the modality to use for the x-axis."""
 
 _y_mod = """\
 y_mod
     Name of the modality to use for the y-axis."""
 
+_x_name = """\
+x_name
+    Name of the x-variable. If passing a `resource` dataframe, this should match the first column."""
+
+_y_name = """\
+y_name
+    Name of the y-variable. If passing a `resource` dataframe, this should match the second column."""
+
 _mask_negatives = """\
 mask_negatives
     Whether to mask negative-negative (low-low) or uncategorized interactions."""
 
 
 # Plot docstrings
 _liana_res = """\
@@ -309,19 +321,22 @@
     ligand_key=_ligand_key,
     receptor_key=_receptor_key,
     score_key=_score_key,
     uns_key=_uns_key,
     inverse_fun=_inverse_fun,
     spatial_key=_spatial_key,
     connectivity_key=_connectivity_key,
-    function_name=_function_name,
+    local_name=_local_name,
+    global_name=_global_name,
     positive_only=_positive_only,
     add_categories=_add_categories,
     x_mod=_x_mod,
     y_mod=_y_mod,
+    x_name=_x_name,
+    y_name=_y_name,
     mask_negatives=_mask_negatives,
     colour=_colour,
     size=_size,
     source_labels=_source_labels,
     target_labels=_target_labels,
     top_n=_top_n,
     orderby=_orderby,
```

### Comparing `liana-1.0.5/liana/_logging.py` & `liana-1.1.0/liana/_logging.py`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/liana/method/__init__.py` & `liana-1.1.0/liana/method/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 
 from liana.method.sc._Method import Method, MethodMeta, _show_methods
 from liana.method.sc._rank_aggregate import AggregateClass, _rank_aggregate_meta as aggregate_meta
 from liana.method.sc import cellphonedb, connectome, logfc, natmi, singlecellsignalr, geometric_mean, cellchat, scseqcomm
 
-from liana.method.sp import bivar, lr_bivar, genericMistyData, lrMistyData, MistyData
+from liana.method.sp import bivariate, genericMistyData, lrMistyData, MistyData
 from liana.method.fun._causalnet import find_causalnet, build_prior_network
 from liana._constants import DefaultValues as V
 
 # callable consensus instance
 _methods = [cellphonedb, connectome, logfc, natmi, singlecellsignalr]
 rank_aggregate = AggregateClass(aggregate_meta, methods=_methods)
 
@@ -31,15 +31,15 @@
 
 def process_scores(liana_res, score_key, inverse_fun=V.inverse_fun):
 
     df = liana_res.copy()
     scores = get_method_scores()
 
     if not np.isin(score_key, list(scores.keys())).any():
-        raise ValueError(f"Score column {score_key} not found in liana's method scores. ")
+        raise ValueError(f"Score column {score_key} not found in liana's method scores.")
 
     # reverse if ascending order
     ascending_order = scores[score_key]
     if(ascending_order):
         df[score_key] = inverse_fun(df[score_key])
 
     return df
```

### Comparing `liana-1.0.5/liana/method/_pipe_utils/_aggregate.py` & `liana-1.1.0/liana/method/_pipe_utils/_aggregate.py`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/liana/method/_pipe_utils/_common.py` & `liana-1.1.0/liana/method/_pipe_utils/_common.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -43,11 +43,11 @@
 
 def _get_groupby_subset(groupby_pairs):
     if groupby_pairs is not V.groupby_pairs:
         if not (P.source in groupby_pairs.columns) | (P.target in groupby_pairs.columns):
             raise AssertionError(f"{P.source} and {P.target} must be in groupby_pairs")
         groupby_subset = union1d(groupby_pairs[P.source].unique(),
                                  groupby_pairs[P.target].unique())
+
     else:
         groupby_subset = None
-
     return groupby_subset
```

### Comparing `liana-1.0.5/liana/method/_pipe_utils/_get_mean_perms.py` & `liana-1.1.0/liana/method/_pipe_utils/_get_mean_perms.py`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/liana/method/_pipe_utils/_pre.py` & `liana-1.1.0/liana/method/_pipe_utils/_pre.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,15 @@
 def prep_check_adata(adata: AnnData,
                      groupby: (str | None),
                      min_cells: (int | None),
                      groupby_subset: (np.array | None) = None,
                      use_raw: Optional[bool] = False,
                      layer: Optional[str] = None,
                      obsm = None,
+                     uns = None,
                      complex_sep='_',
                      verbose: Optional[bool] = False) -> AnnData:
     """
     Check if the anndata object is in the correct format and preprocess
 
     Parameters
     ----------
@@ -109,14 +110,15 @@
         obsm = {k: v for k, v in obsm.items() if not isinstance(v, AnnData)}
 
     adata = sc.AnnData(X=X,
                        obs=adata.obs.copy(),
                        dtype="float32",
                        var=var,
                        obsp=adata.obsp.copy(),
+                       uns=uns,
                        obsm=obsm
                        ).copy()
     adata.var_names_make_unique()
 
     # Check for empty features
     msk_features = np.sum(adata.X, axis=0).A1 == 0
     n_empty_features = np.sum(msk_features)
@@ -158,22 +160,18 @@
             adata = adata[msk]
             _logg("The following cell identities were excluded: {0}".format(", ".join(lowly_abundant_idents)),
                  level='warn', verbose=verbose)
 
     check_vars(adata.var_names,
                complex_sep=complex_sep,
                verbose=verbose)
-
     # Re-order adata vars alphabetically
     adata = adata[:, np.sort(adata.var_names)]
-
     return adata
 
-
-# format variable names
 def check_vars(var_names, complex_sep, verbose=False) -> list:
     """
     Raise a warning if `complex_sep` is part of any variable name.
     """
     var_issues = []
     if complex_sep is not None:
         for name in var_names:
```

### Comparing `liana-1.0.5/liana/method/fun/_causalnet.py` & `liana-1.1.0/liana/method/fun/_causalnet.py`

 * *Files 9% similar despite different names*

```diff
@@ -93,15 +93,16 @@
         node_cutoff=0.1,
         min_penalty=0.01,
         max_penalty=1.0,
         missing_penalty=10,
         edge_penalty=0.01,
         solver=None,
         seed=1337,
-        max_seconds=None,
+        max_runs=1,
+        stable_runs=5,
         verbose=True,
         **kwargs
         ):
     """
     Find the causal network that best explains the input/output node scores.
 
     Parameters
@@ -130,16 +131,20 @@
     edge_penalty : float
         The penalty to assign to edges. Default: 0.01
     solver : str, optional
         The solver to use. If None, the default solver will be used. Default: None
         It will default to the solver included in SCIPY, if no other solver is available.
     seed : int, optional
         The seed to use for the random number generator. Default: 1337
-    max_seconds : int, optional
-        The maximum number of seconds to run the solver. Default: None
+    max_runs : int, optional
+        The maximum number of runs to perform. Consider increasing this value if the solver does not converge.
+        In each run, the noise added to the edge and node penalties is perturbed slightly (iterating over the seed).
+        By default, only 1 run is performed.
+    stable_runs : int, optional
+        The number of consecutive stable solutions requires to interrupt the iteration over max_runs. Only used if max_runs is not == 1. Default: 5
     verbose : bool, optional
         Whether to print progress information. Default: True
     **kwargs : dict, optional
         Additional arguments to pass to the solver.
     """
 
     cn = _check_if_installed("corneto")
@@ -165,53 +170,81 @@
         node_penalties = {}
     else:
         node_penalties = _weights_to_penalties(node_weights,
                                                cutoff=node_cutoff,
                                                max_penalty=max_penalty,
                                                min_penalty=min_penalty)
 
-    # assign 0 penalties to input/output nodes, missing_penalty to missing nodes
-    # add a small amount of noise to the penalties to ensure reproducible solutions
-    rng = np.random.default_rng(seed=seed)
-    c_node_penalties = {k: node_penalties.get(k, missing_penalty) + rng.uniform(min_penalty/20, min_penalty/10)
-                        if k not in measured_nodes else 0.0 for k in prior_graph.vertices}
-
-    _logg("Building CORNETO problem...", verbose=verbose)
-    P, G = cn.methods.carnival._extended_carnival_problem(
-        prior_graph,
-        input_node_scores,
-        output_node_scores,
-        node_penalties=c_node_penalties,
-        edge_penalty=edge_penalty
-    )
-
-    # E is the variable with 1 if edge activates or inhibits, 0 otherwise
-    E = P.symbols['reaction_sends_activation_c0'] + P.symbols['reaction_sends_inhibition_c0']
-    W = rng.uniform(edge_penalty/20, edge_penalty/10, size=E.shape)
-    P.add_objectives(W.T @ E)
-
-    _logg(f"Solving with {solver}...", verbose=verbose)
-    if (solver=='scipy') and verbose:
-        kwargs.update(scipy_options=dict(disp='true'))
-    P.solve(
-        solver=solver,
-        max_seconds=max_seconds,
-        verbosity=int(verbose),
-        **kwargs)
-
-    _logg("Done.", verbose=verbose)
-
-    obj_names = ["Loss (unfitted inputs/output)", "Edge penalty error", "Node penalty error"]
-    _logg("Solution summary:", verbose=verbose)
-    for s, o in zip(obj_names, P.objectives):
-        _logg(f" - {s}: {o.value}", verbose=verbose)
-    rows, cols = cn.methods.carnival.export_results(P, G, input_node_scores, output_node_scores)
-    df = pd.DataFrame(rows, columns=cols)
+    run_count = 0 # total runs
+    stable_count = 0 # stable solutions in a row
+    df_all = None # df with all solutions
+
+    while run_count < max_runs:
+        current_seed = seed + run_count
+        if run_count > 0:
+            _logg(f"Run {run_count} with seed {current_seed}", verbose=verbose)
+
+        # assign 0 penalties to input/output nodes, missing_penalty to missing nodes
+        # add a small amount of noise to the penalties to ensure reproducible solutions
+        rng = np.random.default_rng(seed=current_seed)
+        c_node_penalties = {k: node_penalties.get(k, missing_penalty) + rng.uniform(min_penalty/20, min_penalty/10)
+                            if k not in measured_nodes else 0.0 for k in prior_graph.vertices}
+
+        _logg("Building CORNETO problem...", verbose=verbose)
+        P, G = cn.methods.carnival._extended_carnival_problem(
+            prior_graph,
+            input_node_scores,
+            output_node_scores,
+            node_penalties=c_node_penalties,
+            edge_penalty=edge_penalty
+        )
+
+        # E is the variable with 1 if edge activates or inhibits, 0 otherwise
+        E = P.symbols['reaction_sends_activation_c0'] + P.symbols['reaction_sends_inhibition_c0']
+        W = rng.uniform(edge_penalty / 20, edge_penalty / 10, size=E.shape)
+        P.add_objectives(W.T @ E)
+
+        _logg(f"Solving with {solver}...", verbose=verbose)
+        if (solver=='scipy') and verbose:
+            kwargs.update(scipy_options=dict(disp='true'))
+
+        P.solve(
+            solver=solver,
+            verbosity=int(verbose),
+            **kwargs)
+
+        obj_names = ["Loss (unfitted inputs/output)", "Edge penalty error", "Node penalty error"]
+        _logg("Solution summary:", verbose=verbose)
+        for s, o in zip(obj_names, P.objectives):
+            _logg(f" - {s}: {o.value}", verbose=verbose)
+
+        rows, cols = cn.methods.carnival.export_results(P, G, input_node_scores, output_node_scores)
+        df = pd.DataFrame(rows, columns=cols)
+
+        # Check if all rows from df are contained in df_all
+        if df_all is None:
+            df_all = df
+            continue
+        else:
+            set_df = set(tuple(row) for row in df.values)
+            set_df_all = set(tuple(row) for row in df_all.values)
+
+            if set_df.issubset(set_df_all):
+                stable_count += 1
+            else:
+                stable_count = 0
 
-    return df, P
+            df_all = pd.concat([df_all, df]).drop_duplicates()
+
+        if stable_count >= stable_runs:
+            break
+
+        run_count += 1
+
+    return df_all, P
 
 
 def _weights_to_penalties(props,
                           cutoff,
                           min_penalty,
                           max_penalty):
     if any(p < 0 or p > 1 for p in props.values()):
```

### Comparing `liana-1.0.5/liana/method/sc/_Method.py` & `liana-1.1.0/liana/method/sc/_Method.py`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/liana/method/sc/_cellchat.py` & `liana-1.1.0/liana/method/sc/_cellchat.py`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/liana/method/sc/_cellphonedb.py` & `liana-1.1.0/liana/method/sc/_cellphonedb.py`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/liana/method/sc/_connectome.py` & `liana-1.1.0/liana/method/sc/_connectome.py`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/liana/method/sc/_geometric_mean.py` & `liana-1.1.0/liana/method/sc/_geometric_mean.py`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/liana/method/sc/_liana_pipe.py` & `liana-1.1.0/liana/method/sc/_liana_pipe.py`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/liana/method/sc/_logfc.py` & `liana-1.1.0/liana/method/sc/_logfc.py`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/liana/method/sc/_natmi.py` & `liana-1.1.0/liana/method/sc/_natmi.py`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/liana/method/sc/_rank_aggregate.py` & `liana-1.1.0/liana/method/sc/_rank_aggregate.py`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/liana/method/sc/_scseqcomm.py` & `liana-1.1.0/liana/method/sc/_scseqcomm.py`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/liana/method/sc/_singlecellsignalr.py` & `liana-1.1.0/liana/method/sc/_singlecellsignalr.py`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/liana/method/sp/_Misty.py` & `liana-1.1.0/liana/method/sp/_misty/_Misty.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,50 @@
 from __future__ import annotations
 
 import numpy as np
 import pandas as pd
-from liana._logging import _logg
 from tqdm import tqdm
 
-from scipy.sparse import isspmatrix_csr, csr_matrix
-import statsmodels.api as sm
 from mudata import MuData
-from sklearn.ensemble import RandomForestRegressor
 from sklearn.linear_model import LinearRegression, RidgeCV
-from sklearn.model_selection import KFold, cross_val_predict
+from sklearn.model_selection import KFold
+
+from liana.method.sp._misty._single_view_models import SingleViewModel
 
 from liana._docs import d
 from liana._constants import Keys as K, DefaultValues as V
+from liana._logging import _logg
 
 
 class MistyData(MuData):
     """MistyData Class used to construct multi-view objects"""
     @d.dedent
     def __init__(self,
                  data:(dict | MuData),
-                 obs:(pd.DataFrame | None)= None,
-                 spatial_key:str=K.spatial_key, # NOTE: change to spatial_connectivities?
-                 enforce_obs=True,
+                 obs:(pd.DataFrame | None)=None,
+                 spatial_key: str=K.spatial_key,
+                 enforce_obs:bool=True,
                  **kwargs):
         """
         Construct a MistyData object from a dictionary of views (anndatas).
 
         Parameters
         ----------
         data : `dict`
-            Dictionary of views (anndatas) or an mdata object.
-            Requires an intra-view called "intra".
+            Dictionary of views (anndatas) or a MuData object. Note that only the .X attribute is used.
+            An intra-view called "intra" is required.
         obs : `pd.DataFrame`
             DataFrame of observations. If None, the obs of the intra-view is used.
         %(spatial_key)s
+        enforce_obs : `bool`, optional (default: True)
+            If True, the number of observations in each extra-view must match the intra-view.
+            Then the connectivities are stored in the .obsp attribute, while the weighted matrix is stored in .layers['weighted'].
+
+            If False, the connectivities are stored in the .obsm attribute, while the weighted matrix is transposed and stored in .varm['weighted'].
+
         **kwargs
             Keyword arguments passed to the MuData Super class
         """
         if isinstance(data, MuData):
             data = data.mod
 
         super().__init__(data, **kwargs)
@@ -50,87 +55,94 @@
         self.obs = obs if obs is not None else self.mod['intra'].obs
 
     def _check_views(self):
         assert isinstance(self, MuData), "views must be a MuData object"
         assert "intra" in self.view_names, "views must contain an intra view"
 
         for view in self.view_names:
-            if not isspmatrix_csr(self.mod[view].X):
-                _logg(f"view {view} is not a csr_matrix. Converting to csr_matrix", verbose=True, level='warn')
-                self.mod[view].X = csr_matrix(self.mod[view].X)
             if view=="intra":
                 continue
             if self.enforce_obs:
                 if f"{self.spatial_key}_connectivities" not in self.mod[view].obsp.keys():
                     raise ValueError(f"view {view} does not contain `{self.spatial_key}_connectivities` key in .obsp")
                 if self.mod[view].shape[0] != self.mod['intra'].shape[0]:
                     raise ValueError(f"view {view} has {self.mod[view].shape[0]} observations, " + \
                                     f"but the intra-view has {self.mod['intra'].shape[0]} observations")
             else:
                 if f"{self.spatial_key}_connectivities" not in self.mod[view].obsm.keys():
                     raise ValueError(f"view {view} does not contain `{self.spatial_key}_connectivities` key in .obsm")
 
-    def _get_conn(self, view_name):
+            self._set_weighted_matrix(view)
+
+    def _set_weighted_matrix(self, view_name):
+        if self.enforce_obs:
+            weights = self.mod[view_name].obsp[f"{self.spatial_key}_connectivities"]
+            self.mod[view_name].layers['weighted'] = weights @ self.mod[view_name].X
+        else:
+            weights = self.mod[view_name].obsm[f"{self.spatial_key}_connectivities"].T
+            self.mod[view_name].varm['weighted'] = (weights @ self.mod[view_name].X).T
+
+    def get_weighted_matrix(self, view_name, predictors=None):
+        if predictors is None:
+            predictors = self.mod[view_name].var_names
+
         if self.enforce_obs:
-            return self.mod[view_name].obsp[f"{self.spatial_key}_connectivities"]
+            return self.mod[view_name][:, predictors].layers['weighted']
         else:
-            return self.mod[view_name].obsm[f"{self.spatial_key}_connectivities"].T
+            return self.mod[view_name][:, predictors].varm['weighted'].T
+
 
     @d.dedent
     def __call__(self,
-                 model: str = 'rf',
+                 model: SingleViewModel,
                  bypass_intra: bool = False,
                  predict_self: bool = False,
-                 k_cv: int = 10,
-                 alphas = [0.1, 1, 10],
                  maskby = None,
-                 n_jobs = -1,
+                 k_cv: int = 10,
+                 alphas = np.array([0.1, 1, 10]),
                  seed: int = V.seed,
                  inplace: bool = V.inplace,
                  verbose: bool = V.verbose,
                  **kwargs
                  ):
         """
         A Multi-view Learning for dissecting Spatial Transcriptomics data (MISTy) model.
 
         Parameters
         ----------
-        n_estimators : `int`, optional (default: 100)
-            Number of trees in the random forest models used to model single views
         model : `str`, optional (default: 'rf')
-            Model used to model the single views. Default is 'rf'.
-            Can be either 'rf' (random forest) or 'linear' (linear regression).
-        predict_self : `bool`, optional (default: False)
-            Whether to predict self-interactions. These are determined purely by the feature names.
+            Single-view model of class SingleViewModel. Default options are RandomForestModel, LinearModel, and RobustLinearModel
+            available via ``liana.method.sp._misty._single_view_models``.
         bypass_intra : `bool`, optional (default: False)
             Whether to bypass modeling the intraview via leave-one-feature-out (LOFO).
             In other words, whether to bypass modelling each target by LOFO within the same spots.
+        predict_self : `bool`, optional (default: False)
+            Whether to predict self-interactions. These are determined purely by the feature names.
         maskby : `str`, optional (default: None)
             Column in the .obs attribute used to group or mask observations in the intra-view
             If None, all cells are considered as one group.
         k_cv : `int`, optional (default: 10)
             Number of folds for cross-validation used in the multi-view model,
             and single-view models if model is 'linear'.
         alphas : `list`, optional (default: [0.1, 1, 10])
             List of alpha values used to choose from, that control the strength of the ridge regression,
             used for the multi-view part of the model. Only used if there are more than 2 views being modeled (including intra).
-        n_jobs : `int`, optional (default: -1)
-            Number of cores used to construct random forest models
         %(seed)s
         %(inplace)s
         %(verbose)s
         **kwargs : `dict`
-            Keyword arguments passed to the Regressors. Note that n_jobs & random_state are already set.
+            Keyword arguments passed to the Regressors. Note that random_state is already set via ``seed``.
 
         Returns
         -------
         If inplace is True, the results are written to the `.uns` attribute of the object.
         Otherwise two DataFrames are returned, one for target metrics and one for importances.
 
         """
+        model = model(seed, **kwargs)
         view_str = list(self.view_names)
         obs_masks = _create_obs_masks(self.mod['intra'], maskby)
 
         if bypass_intra:
             view_str.remove('intra')
         intra = self.mod['intra']
 
@@ -144,28 +156,26 @@
                 importance_dict = {}
                 if verbose:
                     d = f"Now learning: {target}" + \
                         (f" masked by {intra_group}" if intra_group is not None else "")
                     progress_bar.set_description(d)
 
                 predictors_nonself, insert_index = _get_nonself(target, intra_features)
-                y = intra[msk, target].X.toarray().reshape(-1)
+                y = intra[msk, target].X.toarray().flatten()
                 X = intra[msk, predictors_nonself].X.toarray()
 
                 if not bypass_intra:
+                    model.fit(y=y,
+                              X=X,
+                              predictors=predictors_nonself,
+                              k_cv=k_cv,
+                              )
                     predictions_intra, importance_dict["intra"] = \
-                        _single_view_model(y,
-                                           X,
-                                           predictors_nonself,
-                                           model=model,
-                                           k_cv=k_cv,
-                                           seed=seed,
-                                           n_jobs=n_jobs,
-                                           **kwargs
-                                           )
+                        model.predictions, model.importances
+
                     if insert_index is not None and predict_self:
                         # add self-interactions as nan
                         importance_dict["intra"][target] = np.nan
 
                 # store the predictions for each view to construct predictor matrix for meta model
                 predictions_list = []
 
@@ -175,29 +185,24 @@
                 # model the juxta and paraview (if applicable)
                 for view_name in [v for v in view_str if v != "intra"]:
                     extra = self.mod[view_name]
 
                     extra_features = extra.var_names.to_list()
                     _predictors, _ =  _get_nonself(target, extra_features) if not predict_self else (extra_features, None)
 
-                    # NOTE: we multiply before masking
-                    weights = self._get_conn(view_name)
-                    X = weights @ extra[:, _predictors].X.toarray()
+                    X = self.get_weighted_matrix(view_name, _predictors).toarray()
                     X = X[msk, :]
-
+                    model.fit(y=y,
+                              X=X,
+                              predictors=_predictors,
+                              k_cv=k_cv,
+                              )
                     predictions_extra, importance_dict[view_name] = \
-                        _single_view_model(y,
-                                           X,
-                                           _predictors,
-                                           model=model,
-                                           k_cv=k_cv,
-                                           seed=seed,
-                                           n_jobs=n_jobs,
-                                           **kwargs
-                                           )
+                        model.predictions, model.importances
+
                     predictions_list.append(predictions_extra)
 
                 target_metrics = _multi_model(y,
                                               np.column_stack(predictions_list),
                                               intra_group,
                                               bypass_intra,
                                               view_str,
@@ -263,44 +268,14 @@
     # drop intra and extra group columns if they are all None
     importances = importances.dropna(axis=1, how='all')
     importances = importances.dropna(axis=0)
 
     return target_metrics, importances
 
 
-def _single_view_model(y, X, predictors, model, k_cv, seed, n_jobs, **kwargs):
-    if model=='rf':
-        model = RandomForestRegressor(oob_score=True,
-                                      n_jobs=n_jobs,
-                                      random_state=seed,
-                                      **kwargs,
-                                      )
-        model = model.fit(y=y, X=X)
-        predictions = model.oob_prediction_
-        importances = model.feature_importances_
-
-    elif model=='linear':
-        model = LinearRegression(n_jobs=1, **kwargs)
-        predictions = cross_val_predict(model,
-                                        X, y,
-                                        cv=KFold(n_splits=k_cv,
-                                                 random_state = seed,
-                                                 shuffle=True),
-                                        n_jobs=n_jobs
-                                        )
-        importances = sm.OLS(y, X).fit().tvalues
-
-    else:
-        raise ValueError(f"model {model} is not supported")
-
-    importances = dict(zip(predictors, importances))
-
-    return predictions, importances
-
-
 def _multi_model(y, predictions, intra_group, bypass_intra, view_str, target, k_cv, alphas, seed):
     n_views = len(view_str)
 
     if (predictions.shape[0] < k_cv) or (y.var() == 0.0):
         if predictions.shape[0] < k_cv:
             warning_message = (f"Number of samples is less than k_cv, {target} metrics set to NaN")
         else:
@@ -358,14 +333,15 @@
         predictors_subset = predictors.copy()
         predictors_subset.pop(insert_idx)
     else:
         predictors_subset = predictors
         insert_idx = None
     return predictors_subset, insert_idx
 
+
 def _create_obs_masks(intra, maskby):
     obs_masks = {}
     # if maskby is a column of only boleans take it as is
     if maskby is None:
         obs_masks[None] = np.ones(intra.shape[0], dtype=bool)
     elif intra.obs[maskby].dtype == bool:
         obs_masks[None] = intra.obs[maskby]
```

### Comparing `liana-1.0.5/liana/method/sp/_SpatialBivariate.py` & `liana-1.1.0/liana/method/sp/_bivariate/_spatial_bivariate.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,301 +1,382 @@
 from __future__ import annotations
+from typing import Union, Optional
 
 import numpy as np
 import pandas as pd
 from scipy.sparse import csr_matrix, isspmatrix_csr
 from anndata import AnnData
 from mudata import MuData
 
 from liana.method._pipe_utils._common import _get_props
-from liana.method.sp._spatial_pipe import (
-    _categorize,
-    _rename_means,
-    _run_scores_pipeline,
-    _add_complexes_to_var
-    )
 from liana.utils.mdata_to_anndata import mdata_to_anndata
 from liana.resource.select_resource import _handle_resource
 from liana.method._pipe_utils import prep_check_adata, assert_covered
-from liana.method.sp._bivariate_funs import _handle_functions, _bivariate_functions
+
+from liana.method.sp._utils import _add_complexes_to_var, _zscore
+from liana.method.sp._bivariate._global_functions import GlobalFunction
+from liana.method.sp._bivariate._local_functions import LocalFunction
 
 from liana._logging import _logg
 from liana._docs import d
 from liana._constants import Keys as K, DefaultValues as V
 
 
 class SpatialBivariate():
     """ A class for bivariate local spatial metrics. """
-    def __init__(self, x_name='x', y_name='y'):
+    def __init__(self, x_name: str = 'x', y_name: str = 'y'):
         self.x_name = x_name
         self.y_name = y_name
 
-    def _handle_return(self, data, stats, local_scores, x_added, inplace=False):
-        if not inplace:
-            return stats, local_scores
-
-        if isinstance(data, MuData):
-            data.mod[x_added] = local_scores
-        else:
-            data.obsm[x_added] = local_scores
-
-
-    def _handle_connectivity(self, adata, connectivity_key):
-        if connectivity_key not in adata.obsp.keys():
-            raise ValueError(f'No connectivity matrix founds in mdata.obsp[{connectivity_key}]')
-        connectivity = adata.obsp[connectivity_key]
-
-        if not isspmatrix_csr(connectivity):
-            connectivity = csr_matrix(connectivity, dtype=np.float32)
-
-        return connectivity
-
-    def _connectivity_to_weight(self, connectivity, local_fun):
-        if not isspmatrix_csr(connectivity) or (connectivity.dtype != np.float32):
-            connectivity = csr_matrix(connectivity, dtype=np.float32)
-
-        if local_fun.__name__ == "_local_morans":
-            norm_factor = connectivity.shape[0] / connectivity.sum()
-            connectivity = norm_factor * connectivity
-
-        if (connectivity.shape[0] < 5000) | local_fun.__name__.__contains__("masked"):
-                return connectivity.A
-        else:
-            return connectivity
-
-
     @d.dedent
     def __call__(self,
                  mdata: (MuData | AnnData),
-                 x_mod: str,
-                 y_mod: str,
-                 function_name: str = 'cosine',
-                 interactions: (None | list) = None,
-                 resource: (None | pd.DataFrame) = None,
-                 resource_name: (None | str) = None,
-                 connectivity_key:str = K.connectivity_key,
-                 mod_added: str = "local_scores",
+                 local_name: (str | None) = 'cosine',
+                 global_name: (None | str | list) = None,
+                 resource_name: str = None,
+                 resource: Optional[pd.DataFrame] = V.resource,
+                 interactions: list = V.interactions,
+                 connectivity_key: str = K.connectivity_key,
                  mask_negatives: bool = False,
                  add_categories: bool = False,
                  n_perms: int = None,
-                 seed:int = V.seed,
-                 nz_threshold:float = 0, # NOTE: do I rename this?
-                 x_use_raw: bool = V.use_raw,
-                 x_layer: (None | str) = V.layer,
-                 x_transform: (bool | callable) = False,
-                 y_use_raw: bool = V.use_raw,
-                 y_layer: (None | str) = V.layer,
-                 y_transform: (bool | callable) = False,
-                 complex_sep: (None | str) = None,
-                 xy_sep:str = V.lr_sep,
+                 seed: int = V.seed,
+                 nz_prop: float = 0.05,
                  remove_self_interactions: bool = True,
-                 inplace:bool = V.inplace,
-                 verbose:bool = V.verbose,
-                 ):
+                 complex_sep: (None | str) = "_",
+                 xy_sep: str = V.lr_sep,
+                 inplace: bool = V.inplace,
+                 key_added: str = "local_scores",
+                 verbose: bool = V.verbose,
+                 **kwargs
+                 ) -> Union[AnnData, pd.DataFrame] | None:
         """
         A method for bivariate local spatial metrics.
 
         Parameters
         ----------
 
         %(mdata)s
-        %(x_mod)s
-        %(y_mod)s
-        %(function_name)s
+        %(local_name)s
+        %(global_name)s
         %(interactions)s
         %(resource)s
         %(resource_name)s
         %(connectivity_key)s
-        mod_added: str
-            Key in `mdata.mod` where the local scores are stored.
         %(mask_negatives)s
         %(add_categories)s
         %(n_perms)s
         %(seed)s
-        nz_threshold: float
-            Minimum proportion of cells expressing the ligand and receptor.
-        x_use_raw: bool
-            Whether to use the raw counts for the x-mod.
-        x_layer: str
-            Layer to use for x-mod.
-        x_transform: bool
-            Function to transform the x-mod.
-        y_use_raw: bool
-            Whether to use the raw counts for y-mod.
-        y_layer: str
-            Layer to use for y-mod.
-        y_transform: bool
-            Function to transform the y-mod.
+        nz_prop: float
+            Minimum proportion of non-zero values for each features. For example, if working with gene expression data,
+            this would be the proportion of cells expressing a gene. Both features must have a proportion greater than
+            `nz_prop` to be considered in the analysis.
         complex_sep: str
             Separator to use for complex names.
         xy_sep: str
             Separator to use for interaction names.
         remove_self_interactions: bool
             Whether to remove self-interactions. `True` by default.
         %(inplace)s
+        key_added: str
+            Key in `mdata.mod` (if MuData) or `adata.obsm` (if AnnData) where the local scores will be stored.
         %(verbose)s
 
+        **kwargs : dict, optional
+            Additional keyword arguments:
+            - For AnnData:
+                %(x_name)s By default: 'ligand'.
+                %(y_name)s By default: 'receptor'.
+
+            - For MuData:
+                %(x_mod)s
+                %(y_mod)s
+                %(x_name)s By default: 'x'.
+                %(y_name)s By default: 'y'.
+                x_use_raw: bool
+                    Whether to use the raw counts for the x-mod.
+                y_use_raw: bool
+                    Whether to use the raw counts for y-mod.
+                x_layer: str
+                    Layer to use for x-mod.
+                y_layer: str
+                    Layer to use for y-mod.
+                x_transform: bool
+                    Function to transform the x-mod.
+                y_transform: bool
+                    Function to transform the y-mod.
+
         Returns
         -------
         If `inplace` is `True`, the results are added to `mdata` and `None` is returned.
-        Note that `obsm`, `varm`, `obsp` and `varp` are copied to the output `AnnData` object.
-        When an MuData object is passed, `obsm`, `varm`, `obsp` and `varp` are copied to `.mod`.
-        When `mdata` is an AnnData object, `obsm`, `varm`, `obsp` and `varp` are copied to `.obsm`.
+        Note that `var`, `obs`, `obsm`, `uns` and `obsp` attributes are copied to the output object.
+        When `mdata` is an `AnnData` object, the results are stored in `mdata.obsm[key_added]`
+        When `mdata` is an `MuData` object, the results are stored in `mdata.mod[key_added]`
+
         `AnnData` objects in `obsm` will not be copied to the output object.
 
         If `inplace` is `False`, the results are returned.
 
         """
 
         if n_perms is not None:
             if not isinstance(n_perms, int) or n_perms < 0:
                 raise ValueError("n_perms must be None, 0 for analytical or > 0 for permutation")
-        if (n_perms == 0) and (function_name != "morans"):
+        if (n_perms == 0) and ((local_name != "morans") or (global_name=='morans')):
             raise ValueError("An analytical solution is currently available only for Moran's R")
+        if global_name is not None:
+            if isinstance(global_name, str):
+                global_name = [global_name]
+
+            global_funs = GlobalFunction.instances.keys()
+            for g_fun in global_funs:
+                if g_fun not in global_funs:
+                    raise ValueError(f"Invalid global function: {g_fun}. Must be in {global_funs}")
 
-        local_fun = _handle_functions(function_name)
-
-        resource = _handle_resource(interactions=interactions,
-                                    resource=resource,
-                                    resource_name=resource_name,
-                                    x_name=self.x_name,
-                                    y_name=self.y_name,
-                                    verbose=verbose)
+        if local_name is not None:
+            local_fun = LocalFunction._get_instance(name=local_name)
 
         if isinstance(mdata, MuData):
-            adata = mdata_to_anndata(mdata,
-                                     x_mod=x_mod,
-                                     y_mod=y_mod,
-                                     x_use_raw=x_use_raw,
-                                     x_layer=x_layer,
-                                     y_use_raw=y_use_raw,
-                                     y_layer=y_layer,
-                                     x_transform=x_transform,
-                                     y_transform=y_transform,
-                                     verbose=verbose,
-                                     )
-            use_raw = False
-            layer = None
+            adata = self._process_mudata(mdata, complex_sep, verbose=verbose, **kwargs)
         elif isinstance(mdata, AnnData):
-            adata = mdata
-            use_raw = x_use_raw
-            layer = x_layer
+            adata = self._process_anndata(mdata, complex_sep, verbose=verbose, **kwargs)
         else:
             raise ValueError("Invalid type, `adata/mdata` must be an AnnData/MuData object")
 
-        _uns = adata.uns
-        adata = prep_check_adata(adata=adata,
-                                 use_raw=use_raw,
-                                 layer=layer,
-                                 verbose=verbose,
-                                 obsm = adata.obsm.copy(),
-                                 groupby=None,
-                                 min_cells=None,
-                                 complex_sep=complex_sep,
-                                )
-
-
-        connectivity = self._handle_connectivity(adata=adata, connectivity_key=connectivity_key)
-        weight = self._connectivity_to_weight(connectivity=connectivity, local_fun=local_fun)
+        resource = _handle_resource(interactions=interactions,
+                                    resource=resource,
+                                    resource_name=resource_name,
+                                    x_name=self.x_name,
+                                    y_name=self.y_name,
+                                    verbose=verbose
+                                    )
+        weight = self._handle_connectivity(adata=adata, connectivity_key=connectivity_key)
 
         if complex_sep is not None:
             adata = _add_complexes_to_var(adata,
                                           np.union1d(resource[self.x_name].astype(str),
                                                      resource[self.y_name].astype(str)
                                                      ),
                                           complex_sep=complex_sep
                                           )
 
         # filter_resource
         resource = resource[(np.isin(resource[self.x_name], adata.var_names)) &
                             (np.isin(resource[self.y_name], adata.var_names))]
 
-        # NOTE: Should I just get rid of remove_self_interactions?
         self_interactions = resource[self.x_name] == resource[self.y_name]
         if self_interactions.any() & remove_self_interactions:
             _logg(f"Removing {self_interactions.sum()} self-interactions", verbose=verbose)
             resource = resource[~self_interactions]
 
         # get entities
         entities = np.union1d(np.unique(resource[self.x_name]),
                                 np.unique(resource[self.y_name]))
-        # Check overlap between resource and adata TODO check if this works
         assert_covered(entities, adata.var_names, verbose=verbose)
 
         # Filter to only include the relevant features
         adata = adata[:, np.intersect1d(entities, adata.var.index)]
 
         xy_stats = pd.DataFrame({'means': adata.X.mean(axis=0).A.flatten(),
                                  'props': _get_props(adata.X)},
                                 index=adata.var_names
                                 ).reset_index().rename(columns={'index': 'gene'})
         # join global stats to LRs from resource
-        xy_stats = resource.merge(_rename_means(xy_stats, entity=self.x_name)).merge(
-            _rename_means(xy_stats, entity=self.y_name))
+        xy_stats = resource.merge(self._rename_means(xy_stats, entity=self.x_name)).merge(
+                                    self._rename_means(xy_stats, entity=self.y_name))
 
-        # TODO: nz_threshold to nz_prop? For consistency with other methods
         # filter according to props
-        xy_stats = xy_stats[(xy_stats[f'{self.x_name}_props'] >= nz_threshold) &
-                            (xy_stats[f'{self.y_name}_props'] >= nz_threshold)]
+        xy_stats = xy_stats[(xy_stats[f'{self.x_name}_props'] >= nz_prop) &
+                            (xy_stats[f'{self.y_name}_props'] >= nz_prop)]
         # create interaction column
         xy_stats['interaction'] = xy_stats[self.x_name] + xy_sep + xy_stats[self.y_name]
 
-        x_mat = adata[:, xy_stats[self.x_name]].X.T
-        y_mat = adata[:, xy_stats[self.y_name]].X.T
+        x_mat = adata[:, xy_stats[self.x_name]].X
+        y_mat = adata[:, xy_stats[self.y_name]].X
+
+        if global_name is not None:
+            for gname in global_name:
+                global_fun = GlobalFunction.instances[gname]
+                global_fun(xy_stats,
+                           x_mat=x_mat,
+                           y_mat=y_mat,
+                           weight=weight,
+                           seed=seed,
+                           n_perms=n_perms,
+                           mask_negatives=mask_negatives,
+                           verbose=verbose,
+                           )
 
-        # reorder columns, NOTE: why?
-        xy_stats = xy_stats.reindex(columns=sorted(xy_stats.columns))
+        if local_name is None:
+            return xy_stats
 
+        # Calculate local scores
         if add_categories or mask_negatives:
-            local_cats = _categorize(x_mat=x_mat,
-                                     y_mat=y_mat,
-                                     weight=weight,
-                                     )
+            local_cats = self._categorize(x_mat=x_mat,
+                                          y_mat=y_mat,
+                                          weight=weight,
+                                          )
         else:
             local_cats = None
 
         # get local scores
-        xy_stats, local_scores, local_pvals = \
-            _run_scores_pipeline(xy_stats=xy_stats,
-                                 x_mat=x_mat,
-                                 y_mat=y_mat,
-                                 local_fun=local_fun,
-                                 weight=weight,
-                                 seed=seed,
-                                 n_perms=n_perms,
-                                 mask_negatives=mask_negatives,
-                                 verbose=verbose,
-                                 )
+        local_scores, local_pvals = \
+            local_fun(x_mat=x_mat,
+                      y_mat=y_mat,
+                      weight=weight,
+                      seed=seed,
+                      n_perms=n_perms,
+                      mask_negatives=mask_negatives,
+                      verbose=verbose,
+                      )
+
+        xy_stats.loc[:, ['mean', 'std']] = \
+            np.vstack(
+                [np.mean(local_scores, axis=0),
+                 np.std(local_scores, axis=0)]
+                ).T
 
         if mask_negatives:
             local_scores = np.where(local_cats!=1, 0, local_scores)
             if local_pvals is not None:
                 local_pvals = np.where(local_cats!=1, 1, local_pvals)
 
-        local_scores = AnnData(csr_matrix(local_scores.T),
+        local_scores = AnnData(csr_matrix(local_scores),
                                obs=adata.obs,
                                var=xy_stats.set_index('interaction'),
-                               uns=_uns,
+                               uns=adata.uns,
                                obsm=adata.obsm,
+                               obsp=adata.obsp,
                                )
 
         if add_categories:
-            local_scores.layers['cats'] = csr_matrix(local_cats.T)
+            local_scores.layers['cats'] = csr_matrix(local_cats)
         if local_pvals is not None:
-            local_scores.layers['pvals'] = csr_matrix(local_pvals.T)
+            local_scores.layers['pvals'] = csr_matrix(local_pvals)
+
+        return self._handle_return(mdata, xy_stats, local_scores, key_added, inplace)
+
+    def _process_anndata(self,
+                         adata,
+                         complex_sep,
+                         verbose,
+                         **kwargs):
+        expected_params = {'x_name', 'y_name', 'use_raw', 'layer'}
+        self.validate_kwargs(expected_params=expected_params, **kwargs)
+
+        self.x_name = kwargs.get('x_name', 'ligand')
+        self.y_name = kwargs.get('y_name', 'receptor')
+
+        return prep_check_adata(adata=adata,
+                                use_raw=kwargs.get('use_raw', V.use_raw),
+                                layer=kwargs.get('layer', V.layer),
+                                verbose=verbose,
+                                obsm=adata.obsm.copy(),
+                                uns=adata.uns.copy(),
+                                groupby=None,
+                                min_cells=None,
+                                complex_sep=complex_sep,
+                                )
+
+    def _process_mudata(self,
+                        mdata,
+                        complex_sep,
+                        verbose,
+                        **kwargs):
+        expected_params = {'x_name', 'y_name',
+                           'x_mod', 'y_mod',
+                           'x_use_raw', 'x_layer',
+                           'y_use_raw', 'y_layer',
+                           'x_transform', 'y_transform'}
+        self.validate_kwargs(expected_params=expected_params, **kwargs)
+
+        self.x_name = kwargs.get('x_name', self.x_name)
+        self.y_name = kwargs.get('y_name', self.y_name)
+
+        x_mod = kwargs.get('x_mod')
+        y_mod = kwargs.get('y_mod')
+
+        if x_mod is None or y_mod is None:
+            raise ValueError("MuData processing requires 'x_mod' and 'y_mod' parameters.")
+
+        adata = mdata_to_anndata(mdata,
+                                 x_mod=x_mod,
+                                 y_mod=y_mod,
+                                 x_use_raw=kwargs.get('x_use_raw', V.use_raw),
+                                 x_layer=kwargs.get('x_layer', V.layer),
+                                 y_use_raw=kwargs.get('y_use_raw', V.use_raw),
+                                 y_layer=kwargs.get('y_layer', V.layer),
+                                 x_transform=kwargs.get('x_transform', False),
+                                 y_transform=kwargs.get('y_transform', False),
+                                 verbose=verbose
+                                 )
+
+        return prep_check_adata(adata=adata,
+                                use_raw=False,
+                                layer=None,
+                                verbose=verbose,
+                                obsm = adata.obsm.copy(),
+                                uns=adata.uns.copy(),
+                                groupby=None,
+                                min_cells=None,
+                                complex_sep=complex_sep, # NOTE
+                                )
+
+
+    def validate_kwargs(self, expected_params, **kwargs):
+        unexpected_kwargs = set(kwargs) - expected_params
+        if unexpected_kwargs:
+            raise ValueError(f"Unexpected keyword arguments: {unexpected_kwargs}")
+
+
+    def _rename_means(self, lr_stats, entity):
+        df = lr_stats.copy()
+        df.columns = df.columns.map(lambda x: entity + '_' + str(x) if x != 'gene' else 'gene')
+        return df.rename(columns={'gene': entity})
 
-        return self._handle_return(mdata, xy_stats, local_scores, mod_added, inplace)
+    def _handle_return(self, data, stats, local_scores, key_added, inplace=False):
+        if not inplace:
+            return stats, local_scores
+
+        if isinstance(data, MuData):
+            data.mod[key_added] = local_scores
+        else:
+            data.obsm[key_added] = local_scores
+
+    def _handle_connectivity(self, adata, connectivity_key):
+        if connectivity_key not in adata.obsp.keys():
+            raise ValueError(f'No connectivity matrix founds in mdata.obsp[{connectivity_key}]')
+        connectivity = adata.obsp[connectivity_key]
+
+        if not isspmatrix_csr(connectivity) or (connectivity.dtype != np.float32):
+            connectivity = csr_matrix(connectivity, dtype=np.float32)
+
+        return connectivity
+
+    def _encode_cats(self, a, weight):
+        if np.all(a >= 0):
+            a = _zscore(a)
+        a = weight @ a
+        a = np.where(a > 0, 1, np.where(a < 0, -1, np.nan))
+        return a
+
+    def _categorize(self, x_mat, y_mat, weight):
+        x_cats = self._encode_cats(x_mat.A, weight)
+        y_cats = self._encode_cats(y_mat.A, weight)
+        cats = x_cats + y_cats
+        cats = np.where(cats == 2, 1, np.where(cats == 0, -1, 0))
+
+        return cats
 
     def show_functions(self):
         """
         Print information about all bivariate local metrics.
         """
-        funs = dict()
-        for function in _bivariate_functions:
+        funs = LocalFunction.instances.copy()
+        for function in funs.values():
             funs[function.name] = {
                 "metadata":function.metadata,
                 "reference":function.reference,
                 }
-
         return pd.DataFrame(funs).T.reset_index().rename(columns={"index":"name"})
 
-bivar = SpatialBivariate()
+bivariate = SpatialBivariate()
```

### Comparing `liana-1.0.5/liana/method/sp/_misty_constructs.py` & `liana-1.1.0/liana/method/sp/_misty/_misty_constructs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import numpy as np
 import pandas as pd
 from anndata import AnnData
 
 from types import ModuleType
 from liana.method._pipe_utils._common import _get_props
 
-from liana.method.sp._Misty import MistyData
+from liana.method.sp._misty._Misty import MistyData
 
 from liana.utils.spatial_neighbors import spatial_neighbors
 from liana.method._pipe_utils._pre import _choose_mtx_rep
 
 from liana.resource import select_resource
 from liana.method._pipe_utils import prep_check_adata
-from liana.method.sp._spatial_pipe import _add_complexes_to_var
+from liana.method.sp._utils import _add_complexes_to_var
 from liana._logging import _check_if_installed
 
 def _make_view(adata, nz_threshold=0.1, add_obs=False, use_raw=False,
                layer=None, connecitivity=None, spatial_key=None, verbose=False):
 
     X = _choose_mtx_rep(adata=adata, use_raw=use_raw, layer=layer, verbose=verbose)
```

### Comparing `liana-1.0.5/liana/multi/_nmf.py` & `liana-1.1.0/liana/multi/_nmf.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 @d.dedent
 def nmf(adata: AnnData=None,
         df: pd.DataFrame=None,
         n_components: (int or None)=None,
         k_range: range = range(1, 11),
         use_raw: bool=False,
         layer: (str or None)=None,
-        inplace:bool=True,
-        verbose:bool=False,
+        inplace: bool=True,
+        verbose: bool=False,
         **kwargs):
     """
     Fits NMF to an AnnData object.
 
     Parameters
     ----------
     %(adata)s
```

### Comparing `liana-1.0.5/liana/multi/df_to_lr.py` & `liana-1.1.0/liana/multi/df_to_lr.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,14 +64,16 @@
 
     """
     _check_groupby(adata=adata, groupby=groupby, verbose=verbose)
     if (groupby not in adata.obs.columns) or (groupby not in dea_df.columns):
         raise ValueError('groupby must match a column in both adata.obs and dea_df')
     if not np.any(adata.var_names.isin(dea_df.index)):
         raise ValueError('index of dea_df must match adata.var_names')
+    if len(np.intersect1d(adata.obs[groupby].unique(), dea_df[groupby].unique())) == 0:
+        raise AssertionError("`groupby` intersect between `dea_df` and `adata` is 0. Please check `groupby`.")
 
     resource = _handle_resource(interactions=interactions,
                                 resource=resource,
                                 resource_name=resource_name,
                                 verbose=verbose)
 
     stat_names = ['expr', 'props'] + stat_keys
```

### Comparing `liana-1.0.5/liana/multi/to_mudata.py` & `liana-1.1.0/liana/multi/to_mudata.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
 
     return mdata
 
 @d.dedent
 def lrs_to_views(adata: AnnData,
                  score_key: (str or None) = None,
                  inverse_fun: callable = V.inverse_fun,
-                 obs_keys: (list or None) =None,
+                 obs_keys: (list or None) = None,
                  lr_prop: float = 0.5,
                  lr_fill: np.nan = np.nan,
                  lrs_per_view:int = 20,
                  lrs_per_sample:int = 10,
                  samples_per_view: int = 3,
                  min_variance:int = 0,
                  lr_sep: str = V.lr_sep,
```

### Comparing `liana-1.0.5/liana/multi/to_tensor_c2c.py` & `liana-1.1.0/liana/multi/to_tensor_c2c.py`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/liana/plotting/_common.py` & `liana-1.1.0/liana/plotting/_common.py`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/liana/plotting/_connectivity_plot.py` & `liana-1.1.0/liana/plotting/_connectivity_plot.py`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/liana/plotting/_dotplot.py` & `liana-1.1.0/liana/plotting/_dotplot.py`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/liana/plotting/_misty_plots.py` & `liana-1.1.0/liana/plotting/_misty_plots.py`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/liana/plotting/_tileplot.py` & `liana-1.1.0/liana/plotting/_tileplot.py`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/liana/resource/_reassemble_complexes.py` & `liana-1.1.0/liana/resource/_reassemble_complexes.py`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/liana/resource/_resource_utils.py` & `liana-1.1.0/liana/resource/_resource_utils.py`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/liana/resource/get_metalinks.py` & `liana-1.1.0/liana/resource/get_metalinks.py`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/liana/resource/omni_resource.csv` & `liana-1.1.0/liana/resource/omni_resource.csv`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/liana/resource/select_resource.py` & `liana-1.1.0/liana/resource/select_resource.py`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/liana/testing/_sample_dea.py` & `liana-1.1.0/liana/testing/_sample_dea.py`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/liana/testing/_sample_lrs.py` & `liana-1.1.0/liana/testing/_sample_lrs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import numpy as np
 import pandas as pd
 import string
 
-
 # Function to generate a liana_res sample/example
 def sample_lrs(by_sample=False):
     """Create sample method output for testing metrics in this task."""
     row_num = 200
     rng = np.random.default_rng(seed=1)
 
     label_vector = list(string.ascii_uppercase[0:10])
```

### Comparing `liana-1.0.5/liana/testing/_sample_misty.py` & `liana-1.1.0/liana/testing/_sample_misty.py`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/liana/testing/datasets.py` & `liana-1.1.0/liana/testing/datasets.py`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/liana/tests/data/aggregate_rank_rest.csv` & `liana-1.1.0/liana/tests/data/aggregate_rank_rest.csv`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/liana/tests/data/all_defaults.csv` & `liana-1.1.0/liana/tests/data/all_defaults.csv`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/liana/tests/data/not_defaults.csv` & `liana-1.1.0/liana/tests/data/not_defaults.csv`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/liana/tests/data/synthetic.h5ad` & `liana-1.1.0/liana/tests/data/synthetic.h5ad`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/liana/tests/test_bivariate_funs.py` & `liana-1.1.0/liana/tests/test_bivariate_funs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 import numpy as np
 
-from liana.method.sp._bivariate_funs import _vectorized_pearson, _vectorized_spearman, \
+from liana.method.sp._bivariate._local_functions import _vectorized_pearson, _vectorized_spearman, \
     _vectorized_cosine, _vectorized_jaccard, _masked_spearman, _local_morans, _product, \
     _norm_product
 
 from scipy.sparse import csr_matrix
 
 
 rng = np.random.default_rng(seed=0)
 
 x_mat = rng.normal(size=(20, 5)).astype(np.float32)
 y_mat = rng.normal(size=(20, 5)).astype(np.float32)
 weight = csr_matrix(rng.uniform(size=(20, 20)).astype(np.float32))
 
-
 def _assert_bivariate(function, desired, x_mat, y_mat, weight):
     actual = function(x_mat, y_mat, weight)
-    assert actual.shape == (5, 20)
-    np.testing.assert_almost_equal(actual[:, 0], desired, decimal=5)
+    assert actual.shape == (20, 5)
+    np.testing.assert_almost_equal(actual[0, :], desired, decimal=5)
 
 
 def test_pc_vectorized():
     pc_vec_truth = np.array([0.25005114, 0.04262733, -0.00130362, 0.2903336, -0.1236529])
     _assert_bivariate(_vectorized_pearson, pc_vec_truth, x_mat, y_mat, weight)
```

### Comparing `liana-1.0.5/liana/tests/test_causalnet.py` & `liana-1.1.0/liana/tests/test_causalnet.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,21 +23,22 @@
     prior_graph = build_prior_network(input_pkn, input_scores, output_scores, verbose=False)
     df_res, problem = find_causalnet(prior_graph,
                                      input_scores,
                                      output_scores,
                                      node_weights=node_weights,
                                      verbose=False,
                                      solver='scipy',
-                                     seed=1337
+                                     seed=1337,
+                                     max_runs=20,
+                                     stable_runs=10,
                                      )
 
     assert problem.weights == [1.0, 0.01, 1.0, 1.0]
-    assert df_res['source_pred_val'].values.sum() == 5
-    assert df_res['target_pred_val'].values.sum() == 8
-    assert df_res[df_res['source_type']=='input']['source'].values[0] == 'I2'
+    assert df_res['source_pred_val'].values.sum() == 8.0
+    assert df_res['target_pred_val'].values.sum() == 11
     assert (df_res[df_res['target_type']=='output']['target'].isin(['M1', 'M2'])).all()
 
 
 
 def test_causalnet_noweights():
     prior_graph = build_prior_network(input_pkn, input_scores, output_scores, verbose=False)
     df_res, problem = find_causalnet(prior_graph,
```

### Comparing `liana-1.0.5/liana/tests/test_converters.py` & `liana-1.1.0/liana/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/liana/tests/test_generate_lr.py` & `liana-1.1.0/liana/tests/test_generate_lr.py`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/liana/tests/test_get_mean_perms.py` & `liana-1.1.0/liana/tests/test_get_mean_perms.py`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/liana/tests/test_interpolate.py` & `liana-1.1.0/liana/tests/test_interpolate.py`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/liana/tests/test_liana_pipe.py` & `liana-1.1.0/liana/tests/test_liana_pipe.py`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/liana/tests/test_metalinksdb.py` & `liana-1.1.0/liana/tests/test_metalinksdb.py`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/liana/tests/test_misty.py` & `liana-1.1.0/liana/tests/test_misty.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,50 @@
 import os
 import pathlib
 import numpy as np
 import scanpy as sc
-from liana.method.sp._misty_constructs import lrMistyData, genericMistyData
+from liana.method.sp._misty._misty_constructs import lrMistyData, genericMistyData
+from liana.method.sp._misty._single_view_models import RandomForestModel, LinearModel, RobustLinearModel
 from liana.testing._sample_anndata import generate_toy_spatial
 from liana.method import MistyData
 
 test_path = pathlib.Path(__file__).parent
 
 adata = sc.read_h5ad(os.path.join(test_path, "data" , "synthetic.h5ad"))
 adata = sc.pp.subsample(adata, n_obs=100, copy=True)
 
 
 def test_misty_para():
-    misty = genericMistyData(adata, bandwidth=10,
-                             cutoff=0, add_juxta=False,
-                             set_diag=False, seed=133)
-    misty(bypass_intra=False, seed=42, n_estimators=11)
+    misty = genericMistyData(adata,
+                             bandwidth=10,
+                             cutoff=0,
+                             add_juxta=False,
+                             set_diag=False,
+                             seed=133
+                             )
+    misty(model=RandomForestModel, bypass_intra=False, seed=42, n_estimators=11)
     assert np.isin(list(misty.uns.keys()), ['target_metrics', 'interactions']).all()
     target_metrics = misty.uns['target_metrics']
     assert np.sum(target_metrics[['intra', 'para']].values, axis=1).sum() == 11.0
     assert target_metrics.shape == (11, 6)
 
     interactions = misty.uns['interactions']
     assert interactions.shape == (220, 4)
     assert interactions[interactions['target']=='ECM']['importances'].sum().round(8) == 2.0
 
 
 def test_misty_bypass():
-    misty = genericMistyData(adata, bandwidth=10, add_juxta=True, set_diag=True,
-                             cutoff=0, coord_type="generic", delaunay=True)
-    misty(alphas=1, bypass_intra=True, seed=42, n_estimators=11)
+    misty = genericMistyData(adata,
+                             bandwidth=10,
+                             add_juxta=True,
+                             set_diag=True,
+                             cutoff=0,
+                             coord_type="generic",
+                             delaunay=True)
+    misty(model=RandomForestModel, alphas=1, bypass_intra=True, seed=42, n_estimators=11)
     assert np.isin(['juxta', 'para'], misty.uns['target_metrics'].columns).all()
     assert ~np.isin(['intra'], misty.uns['target_metrics'].columns).all()
     assert misty.uns['target_metrics'].shape == (11, 6)
     np.testing.assert_almost_equal(misty.uns['target_metrics']['multi_R2'].sum(), 0, decimal=5)
 
     interactions = misty.uns['interactions']
     assert interactions.shape == (220, 4)
@@ -49,15 +59,16 @@
                              bandwidth=20,
                              add_juxta=True,
                              set_diag=False,
                              cutoff=0,
                              coord_type="generic",
                              delaunay=True
                              )
-    misty(alphas=1,
+    misty(model=RandomForestModel,
+          alphas=1,
           bypass_intra=False,
           seed=42,
           predict_self=True,
           maskby='cell_type',
           n_estimators=11)
 
     assert misty.uns['target_metrics'].shape==(22, 8)
@@ -77,57 +88,76 @@
 
 
 def test_lr_misty():
     adata = generate_toy_spatial()
     misty = lrMistyData(adata, bandwidth=10, set_diag=True, cutoff=0)
     assert misty.shape == (700, 42)
 
-    misty(n_estimators=10, bypass_intra=True)
+    misty(model=RandomForestModel, n_estimators=10, bypass_intra=True)
     assert misty.uns['target_metrics'].shape == (16, 5)
 
     interactions = misty.uns['interactions']
     assert interactions.shape == (415, 4)
     cmplxs = interactions[interactions['target'].str.contains('_')]['target'].unique()
     assert np.isin(['CD8A_CD8B', 'CD74_CXCR4'], cmplxs).all()
 
 
 def test_linear_misty():
     misty = genericMistyData(adata, bandwidth=10, set_diag=False, cutoff=0)
     assert misty.shape == (100, 33)
 
-    misty(model='linear')
+    misty(model=LinearModel)
     assert misty.uns['target_metrics'].shape == (11, 7)
 
     assert misty.uns['interactions'].shape == (330, 4)
     actual = misty.uns['interactions']['importances'].values.mean()
-    np.testing.assert_almost_equal(actual, 0.6683044, decimal=2)
+    np.testing.assert_almost_equal(actual, 0.4941761900911731, decimal=3)
 
 
 def test_misty_mask():
     misty = genericMistyData(adata, bandwidth=10, set_diag=False, cutoff=0)
     misty = MistyData(misty)
     assert misty.shape == (100, 33)
 
     misty.mod['intra'].obs['mask'] = misty.mod['intra'].obs=='A'
-    misty(model='linear', maskby='mask')
+    misty(model=LinearModel, maskby='mask')
 
     assert misty.uns['target_metrics'].shape == (11, 7)
     np.testing.assert_almost_equal(misty.uns['target_metrics']['multi_R2'].mean(), 0.4203699749106394, decimal=3)
     np.testing.assert_almost_equal(misty.uns['target_metrics']['intra_R2'].mean(), 0.4248588250759459, decimal=3)
 
     assert misty.uns['interactions'].shape == (330, 4)
-    np.testing.assert_almost_equal(misty.uns['interactions']['importances'].sum(), 184, decimal=0)
+    np.testing.assert_almost_equal(misty.uns['interactions']['importances'].sum(), 141.05332654128952, decimal=0)
 
 
-def test_misty_multivew():
+def test_misty_custom():
     adata = generate_toy_spatial()
     # keep first 10 vars
     xdata = adata[:, :10].copy()
     xdata.var.index = 'x' + xdata.var.index
 
     ydata = adata[:, -10:].copy()
     ydata.var.index = 'y' + ydata.var.index
     intra = adata[:, 25:30].copy()
     misty = MistyData({'intra': intra, 'xdata': xdata, 'ydata': ydata}, verbose=True)
-    misty(model='linear')
+    misty(model=RobustLinearModel, k_cv=25, seed=420)
 
     misty.uns['interactions'].shape == (120, 4)
+    np.testing.assert_almost_equal(misty.uns['interactions']['importances'].max(), 7.427809495362697, decimal=3)
+    np.testing.assert_almost_equal(misty.uns['interactions']['importances'].min(), -2.8430222384873396, decimal=3)
+    # the data is random
+    np.testing.assert_almost_equal(misty.uns['target_metrics']['multi_R2'].mean(), 0, decimal=3)
+
+
+def test_misty_nonaligned():
+    adata = generate_toy_spatial()
+
+    intra = adata[:, :10].copy()
+    intra.var.index = 'x' + intra.var.index
+    para = adata[:int(adata.n_obs*0.9), -10:].copy()
+    para.var.index = 'y' + para.var.index
+    # Generate connectivities with shape (para.n_obs, intra.n_obs)
+    para.obsm['spatial_connectivities'] = np.ones((para.n_obs, intra.n_obs))
+    misty = MistyData({'intra': intra, 'ydata': para},
+                      enforce_obs=False, # NOTE: This is the key parameter
+                      verbose=True)
+    misty(model=LinearModel, k_cv=3)
```

### Comparing `liana-1.0.5/liana/tests/test_misty_plots.py` & `liana-1.1.0/liana/tests/test_misty_plots.py`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/liana/tests/test_multi.py` & `liana-1.1.0/liana/tests/test_multi.py`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/liana/tests/test_multi_dea.py` & `liana-1.1.0/liana/tests/test_multi_dea.py`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/liana/tests/test_multi_nmf.py` & `liana-1.1.0/liana/tests/test_multi_nmf.py`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/liana/tests/test_plotting.py` & `liana-1.1.0/liana/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/liana/tests/test_pre.py` & `liana-1.1.0/liana/tests/test_pre.py`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/liana/tests/test_rank_aggregate.py` & `liana-1.1.0/liana/tests/test_rank_aggregate.py`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/liana/tests/test_sc_methods.py` & `liana-1.1.0/liana/tests/test_sc_methods.py`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/liana/tests/test_select_resource.py` & `liana-1.1.0/liana/tests/test_select_resource.py`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/liana/tests/test_spatial_utils.py` & `liana-1.1.0/liana/tests/test_spatial_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 from  scipy.sparse import csr_matrix
 
-from liana.method.sp._spatial_pipe import _global_zscore_pvals, _global_permutation_pvals, _local_permutation_pvals, _local_zscore_pvals
-from liana.method.sp._bivariate_funs import _local_morans
+from liana.method.sp._bivariate._global_functions import _global_r
+from liana.method.sp._bivariate._local_functions import LocalFunction
 from liana.utils.spatial_neighbors import spatial_neighbors
 
 from liana.testing._sample_anndata import generate_toy_spatial
 
 adata = generate_toy_spatial()
 
 def test_get_spatial_connectivities():
@@ -54,61 +54,56 @@
 
 x_mat = rng.normal(size=(10, 10))
 y_mat = rng.normal(size=(10, 10))
 n_perms = 100
 mask_negatives = True
 
 
-def test_global_permutation_pvals():
-    global_truth = rng.normal(size=(10))
-
-    pvals = _global_permutation_pvals(x_mat=x_mat,
-                                      y_mat=y_mat,
-                                      global_r=global_truth,
-                                      seed=seed,
-                                      n_perms=n_perms,
-                                      mask_negatives=mask_negatives,
-                                      weight = weight,
-                                      verbose=False
-                                      )
-    assert pvals.shape == (10, )
-    assert pvals.sum().round(3)==5.16
-
-
-
+local_morans = LocalFunction._get_instance('morans')
 def test_local_permutation_pvals():
     local_truth = rng.normal(size=(10, 10))
     mask_negatives = True
 
-    pvals = _local_permutation_pvals(x_mat = x_mat,
-                                     y_mat = y_mat,
-                                     local_truth = local_truth,
-                                     local_fun = _local_morans,
-                                     weight = weight,
-                                     n_perms = n_perms,
-                                     seed = seed,
-                                     mask_negatives=mask_negatives,
-                                     verbose=False
-                                     )
+    pvals = local_morans._permutation_pvals(x_mat = x_mat,
+                                            y_mat = y_mat,
+                                            local_truth = local_truth,
+                                            weight = weight,
+                                            n_perms = n_perms,
+                                            seed = seed,
+                                            mask_negatives=mask_negatives,
+                                            verbose=False
+                                            )
     assert pvals.shape == (10, 10)
 
 
-def test_global_zscore_pvals():
-    global_truth = rng.normal(size=(10))
-    pvals = _global_zscore_pvals(global_r=global_truth,
-                                 weight=weight,
-                                 mask_negatives=mask_negatives
-    )
-    assert pvals.shape == (10, )
-
-
 def test_local_zscore_pvals():
     local_truth = rng.normal(size=(10, 10))
-    pvals = _local_zscore_pvals(x_mat=x_mat, y_mat=y_mat, weight=weight,
-                                local_truth=local_truth, mask_negatives=mask_negatives)
-    actual = _local_zscore_pvals(x_mat=x_mat, y_mat=y_mat,
-                                 weight=weight, local_truth=local_truth,
-                                 mask_negatives=mask_negatives).mean(axis=0)[0:3]
-    np.testing.assert_almost_equal(actual, np.array([0.51388, 0.48678, 0.49618]), decimal=5)
+    actual = local_morans._zscore_pvals(x_mat=x_mat, y_mat=y_mat,
+                                        weight=weight, local_truth=local_truth,
+                                        mask_negatives=mask_negatives)
+    np.testing.assert_almost_equal(actual.mean(axis=0)[0:3], np.array([0.51747, 0.47383, 0.49125]), decimal=5)
+    assert actual.shape == (10, 10)
 
 
-    assert pvals.shape == (10, 10)
+
+def test_global_zscore_pvals():
+    global_stat = rng.normal(size=(10))
+    pvals = _global_r._zscore_pvals(global_stat=global_stat,
+                                    weight=weight,
+                                    mask_negatives=mask_negatives
+    )
+    assert pvals.shape == (10,)
+
+
+def test_global_permutation_pvals():
+    global_stat = rng.normal(size=(10))
+    pvals = _global_r._permutation_pvals(x_mat=x_mat,
+                                         y_mat=y_mat,
+                                         global_stat=global_stat,
+                                         seed=seed,
+                                         n_perms=n_perms,
+                                         mask_negatives=mask_negatives,
+                                         weight=weight,
+                                         verbose=False
+                                      )
+    assert pvals.shape == (10, )
+    assert pvals.sum().round(3)==4.97
```

### Comparing `liana-1.0.5/liana/utils/_getters.py` & `liana-1.1.0/liana/utils/_getters.py`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/liana/utils/interpolate_adata.py` & `liana-1.1.0/liana/utils/interpolate_adata.py`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/liana/utils/mdata_to_anndata.py` & `liana-1.1.0/liana/utils/mdata_to_anndata.py`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/liana/utils/obsm_to_adata.py` & `liana-1.1.0/liana/utils/obsm_to_adata.py`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/liana/utils/query_bandwidth.py` & `liana-1.1.0/liana/utils/query_bandwidth.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 from sklearn.neighbors import BallTree
-from plotnine import ggplot, aes, geom_line, geom_point, theme_bw, xlab, ylab
+from plotnine import ggplot, aes, geom_line, geom_point, theme_bw, xlab, ylab, scale_y_continuous
 from pandas import DataFrame
 
 def query_bandwidth(coordinates: np.ndarray,
                     start: int = 0,
                     end: int = 500,
                     interval_n:int = 50,
                     reference: np.ndarray = None
@@ -51,13 +51,14 @@
         # calculate the average number of neighbors
         avg_nn = np.mean(num_neighbors)
         df.loc[n, 'neighbours'] = avg_nn
 
     p = (ggplot(df, aes(x='bandwith', y='neighbours')) +
          geom_line() +
          geom_point() +
+         scale_y_continuous(breaks=range(start, end, interval_n)) +
          theme_bw(base_size=16) +
          xlab("Bandwidth") +
          ylab("Number of Neighbors")
          )
 
     return p, df
```

### Comparing `liana-1.0.5/liana/utils/spatial_neighbors.py` & `liana-1.1.0/liana/utils/spatial_neighbors.py`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/liana/utils/transform.py` & `liana-1.1.0/liana/utils/transform.py`

 * *Files identical despite different names*

### Comparing `liana-1.0.5/pyproject.toml` & `liana-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "liana"
-version = "1.0.5"
+version = "1.1.0"
 description = "LIANA+: a one-stop-shop framework for cell-cell communication"
 authors = ["Daniel Dimitrov <daniel.dimitrov@uni-heidelberg.de>"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Topic :: Software Development :: Build Tools",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Scientific/Engineering :: Bio-Informatics",
@@ -30,14 +30,15 @@
 omnipath = {version = ">=1.0.6", optional = true}
 decoupler = {version = ">=1.4.0", optional = true}
 pydeseq2 = {version = ">=0.3.5", optional = true}
 squidpy = {version = "*", optional = true}
 cell2cell = {version = "*", optional = true}
 muon = {version = "*", optional = true}
 mofax = {version = "*", optional = true}
+mofapy2 = {version = ">=0.7.0", optional = true}
 corneto = {version = "0.9.1-alpha.4", optional = true}
 cvxpy = {version = "^1.2.1", optional = true}
 cylp = {version = "^0.91.5", optional = true}
 pre-commit = {version = ">=3.0.0", optional = true}
 requests = {version = "^2.25.1", optional = true}
 docrep = ">=0.3.1"
 
@@ -48,15 +49,16 @@
 sphinx = "^4.0"
 nbsphinx = "^0.8"
 sphinx_automodapi = "^0.14"
 ipython = "^7.0"
 ipykernel = "^6.0"
 pandoc = "^1.0"
 numpydoc = "^1.1"
+bumpversion = "^0.6.0"
 
 [tool.poetry.extras]
 common = ["decoupler", "omnipath", "requests"]
-full = ["decoupler", "omnipath", "pydeseq2", "squidpy", "cell2cell", "muon", "mofax", "corneto", "cvxpy", "cylp", "requests"]
+full = ["decoupler", "omnipath", "pydeseq2", "squidpy", "cell2cell", "muon", "mofax", "mofapy2", "corneto", "cvxpy", "cylp", "requests"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `liana-1.0.5/PKG-INFO` & `liana-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liana
-Version: 1.0.5
+Version: 1.1.0
 Summary: LIANA+: a one-stop-shop framework for cell-cell communication
 Home-page: https://liana-py.readthedocs.io
 License: GPLv3
 Author: Daniel Dimitrov
 Author-email: daniel.dimitrov@uni-heidelberg.de
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 3 - Alpha
@@ -26,14 +26,15 @@
 Requires-Dist: anndata (>=0.7.4)
 Requires-Dist: cell2cell ; extra == "full"
 Requires-Dist: corneto (==0.9.1-alpha.4) ; extra == "full"
 Requires-Dist: cvxpy (>=1.2.1,<2.0.0) ; extra == "full"
 Requires-Dist: cylp (>=0.91.5,<0.92.0) ; extra == "full"
 Requires-Dist: decoupler (>=1.4.0) ; extra == "common" or extra == "full"
 Requires-Dist: docrep (>=0.3.1)
+Requires-Dist: mofapy2 (>=0.7.0) ; extra == "full"
 Requires-Dist: mofax ; extra == "full"
 Requires-Dist: mudata
 Requires-Dist: muon ; extra == "full"
 Requires-Dist: numba (>=0.54.0)
 Requires-Dist: omnipath (>=1.0.6) ; extra == "common" or extra == "full"
 Requires-Dist: plotnine (>=0.10.0)
 Requires-Dist: pre-commit (>=3.0.0)
```

