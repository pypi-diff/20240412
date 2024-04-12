# Comparing `tmp/DESlib-0.3.6.tar.gz` & `tmp/DESlib-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/DESlib-0.3.6.tar", last modified: Tue Apr  9 22:34:51 2024, max compression
+gzip compressed data, was "DESlib-0.3.7.tar", last modified: Fri Apr 12 01:14:23 2024, max compression
```

## Comparing `DESlib-0.3.6.tar` & `DESlib-0.3.7.tar`

### file list

```diff
@@ -1,182 +1,182 @@
-drwxr-xr-x   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        0 2024-04-09 22:34:51.768548 DESlib-0.3.6/
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     3469 2021-03-27 00:32:40.000000 DESlib-0.3.6/CONTRIBUTING.md
-drwxr-xr-x   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        0 2024-04-09 22:34:51.733036 DESlib-0.3.6/DESlib.egg-info/
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)    14426 2024-04-09 22:34:51.000000 DESlib-0.3.6/DESlib.egg-info/PKG-INFO
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     4524 2024-04-09 22:34:51.000000 DESlib-0.3.6/DESlib.egg-info/SOURCES.txt
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        1 2024-04-09 22:34:51.000000 DESlib-0.3.6/DESlib.egg-info/dependency_links.txt
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)       48 2024-04-09 22:34:51.000000 DESlib-0.3.6/DESlib.egg-info/requires.txt
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        7 2024-04-09 22:34:51.000000 DESlib-0.3.6/DESlib.egg-info/top_level.txt
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     1476 2021-03-27 00:32:40.000000 DESlib-0.3.6/LICENSE.txt
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      207 2021-03-27 00:32:40.000000 DESlib-0.3.6/MANIFEST.in
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)    14426 2024-04-09 22:34:51.768365 DESlib-0.3.6/PKG-INFO
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)    11733 2021-03-27 00:32:40.000000 DESlib-0.3.6/README.rst
-drwxr-xr-x   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        0 2024-04-09 22:34:51.733372 DESlib-0.3.6/deslib/
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      704 2024-04-09 21:56:21.000000 DESlib-0.3.6/deslib/__init__.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)    28533 2024-04-09 21:55:14.000000 DESlib-0.3.6/deslib/base.py
-drwxr-xr-x   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        0 2024-04-09 22:34:51.735550 DESlib-0.3.6/deslib/dcs/
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      463 2021-03-27 00:32:40.000000 DESlib-0.3.6/deslib/dcs/__init__.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)    11054 2022-05-25 04:21:28.000000 DESlib-0.3.6/deslib/dcs/a_posteriori.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     9017 2022-05-25 04:21:28.000000 DESlib-0.3.6/deslib/dcs/a_priori.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)    12386 2024-04-09 21:55:14.000000 DESlib-0.3.6/deslib/dcs/base.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     8422 2022-05-25 04:21:28.000000 DESlib-0.3.6/deslib/dcs/lca.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)    10359 2022-05-25 04:21:28.000000 DESlib-0.3.6/deslib/dcs/mcb.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     9352 2022-05-25 04:21:28.000000 DESlib-0.3.6/deslib/dcs/mla.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     7136 2022-05-25 04:21:28.000000 DESlib-0.3.6/deslib/dcs/ola.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     7802 2022-05-25 04:21:28.000000 DESlib-0.3.6/deslib/dcs/rank.py
-drwxr-xr-x   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        0 2024-04-09 22:34:51.738712 DESlib-0.3.6/deslib/des/
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     1051 2021-03-27 00:32:40.000000 DESlib-0.3.6/deslib/des/__init__.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)    10416 2022-05-25 04:21:28.000000 DESlib-0.3.6/deslib/des/base.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)    17305 2024-04-09 21:55:14.000000 DESlib-0.3.6/deslib/des/des_clustering.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)    17511 2022-05-25 04:30:11.000000 DESlib-0.3.6/deslib/des/des_knn.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)    13483 2024-04-09 21:55:14.000000 DESlib-0.3.6/deslib/des/des_mi.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     7776 2022-05-25 05:13:52.000000 DESlib-0.3.6/deslib/des/des_p.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)    11615 2024-04-09 21:55:14.000000 DESlib-0.3.6/deslib/des/knop.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     9974 2024-04-09 21:55:14.000000 DESlib-0.3.6/deslib/des/knora_e.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     7682 2024-04-09 21:55:14.000000 DESlib-0.3.6/deslib/des/knora_u.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)    23075 2024-04-09 21:55:14.000000 DESlib-0.3.6/deslib/des/meta_des.py
-drwxr-xr-x   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        0 2024-04-09 22:34:51.740478 DESlib-0.3.6/deslib/des/probabilistic/
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      362 2021-03-27 00:32:40.000000 DESlib-0.3.6/deslib/des/probabilistic/__init__.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     7287 2022-05-25 04:21:28.000000 DESlib-0.3.6/deslib/des/probabilistic/base.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     6473 2022-05-25 04:32:34.000000 DESlib-0.3.6/deslib/des/probabilistic/deskl.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     6478 2022-05-25 04:38:46.000000 DESlib-0.3.6/deslib/des/probabilistic/exponential.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     5704 2022-05-25 04:35:37.000000 DESlib-0.3.6/deslib/des/probabilistic/logarithmic.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     5902 2022-05-25 04:37:36.000000 DESlib-0.3.6/deslib/des/probabilistic/minimum_difference.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     5730 2022-05-25 04:38:04.000000 DESlib-0.3.6/deslib/des/probabilistic/rrc.py
-drwxr-xr-x   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        0 2024-04-09 22:34:51.743061 DESlib-0.3.6/deslib/static/
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      428 2021-03-27 00:32:40.000000 DESlib-0.3.6/deslib/static/__init__.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     5080 2022-06-06 05:38:53.000000 DESlib-0.3.6/deslib/static/base.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     5928 2024-04-09 21:55:14.000000 DESlib-0.3.6/deslib/static/oracle.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     6261 2024-04-09 21:55:14.000000 DESlib-0.3.6/deslib/static/single_best.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     7488 2024-04-09 21:55:14.000000 DESlib-0.3.6/deslib/static/stacked.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     7389 2024-04-09 21:55:14.000000 DESlib-0.3.6/deslib/static/static_selection.py
-drwxr-xr-x   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        0 2024-04-09 22:34:51.745702 DESlib-0.3.6/deslib/tests/
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)       24 2021-03-27 00:32:40.000000 DESlib-0.3.6/deslib/tests/__init__.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     6803 2022-05-25 04:21:28.000000 DESlib-0.3.6/deslib/tests/conftest.py
-drwxr-xr-x   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        0 2024-04-09 22:34:51.748707 DESlib-0.3.6/deslib/tests/dcs/
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        0 2021-03-27 00:32:40.000000 DESlib-0.3.6/deslib/tests/dcs/__init__.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     5773 2022-05-25 04:21:28.000000 DESlib-0.3.6/deslib/tests/dcs/test_a_posteriori.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     3497 2022-05-25 04:21:28.000000 DESlib-0.3.6/deslib/tests/dcs/test_a_priori.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)    10024 2022-05-25 04:21:28.000000 DESlib-0.3.6/deslib/tests/dcs/test_base.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     2558 2022-05-25 04:21:28.000000 DESlib-0.3.6/deslib/tests/dcs/test_lca.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     3822 2022-05-25 04:21:28.000000 DESlib-0.3.6/deslib/tests/dcs/test_mcb.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     4250 2022-05-25 04:21:28.000000 DESlib-0.3.6/deslib/tests/dcs/test_mla.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     1215 2022-05-25 04:21:28.000000 DESlib-0.3.6/deslib/tests/dcs/test_ola.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     1099 2022-05-25 04:21:28.000000 DESlib-0.3.6/deslib/tests/dcs/test_rank.py
-drwxr-xr-x   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        0 2024-04-09 22:34:51.751765 DESlib-0.3.6/deslib/tests/des/
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        0 2021-03-27 00:32:40.000000 DESlib-0.3.6/deslib/tests/des/__init__.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     9310 2022-05-25 04:21:28.000000 DESlib-0.3.6/deslib/tests/des/test_base.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     8713 2022-05-25 04:21:28.000000 DESlib-0.3.6/deslib/tests/des/test_des_clustering.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)    10425 2022-05-25 04:21:28.000000 DESlib-0.3.6/deslib/tests/des/test_des_knn.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     5035 2022-05-25 04:21:28.000000 DESlib-0.3.6/deslib/tests/des/test_des_mi.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     2597 2022-05-25 04:21:28.000000 DESlib-0.3.6/deslib/tests/des/test_desp.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     2650 2021-03-29 03:42:00.000000 DESlib-0.3.6/deslib/tests/des/test_knop.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     2394 2022-05-25 04:21:28.000000 DESlib-0.3.6/deslib/tests/des/test_knorae.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     1587 2022-05-25 04:21:28.000000 DESlib-0.3.6/deslib/tests/des/test_knorau.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     9161 2022-05-25 04:21:28.000000 DESlib-0.3.6/deslib/tests/des/test_meta_des.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)    11213 2022-05-25 04:21:28.000000 DESlib-0.3.6/deslib/tests/des/test_probabilistic.py
-drwxr-xr-x   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        0 2024-04-09 22:34:51.753667 DESlib-0.3.6/deslib/tests/static/
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        0 2021-03-27 00:32:40.000000 DESlib-0.3.6/deslib/tests/static/__init__.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     2131 2024-04-09 21:55:14.000000 DESlib-0.3.6/deslib/tests/static/test_oracle.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     3544 2024-04-09 21:55:14.000000 DESlib-0.3.6/deslib/tests/static/test_single_best.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     3172 2024-04-09 21:55:14.000000 DESlib-0.3.6/deslib/tests/static/test_stacked.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     4534 2024-04-09 21:55:14.000000 DESlib-0.3.6/deslib/tests/static/test_static_selection.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)    11190 2022-05-25 04:21:28.000000 DESlib-0.3.6/deslib/tests/test_base.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)    21327 2024-04-09 21:55:14.000000 DESlib-0.3.6/deslib/tests/test_des_integration.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     3389 2021-03-27 00:32:40.000000 DESlib-0.3.6/deslib/tests/test_des_integration_multiclass.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     3335 2022-06-06 06:15:34.000000 DESlib-0.3.6/deslib/tests/test_integration_DFP_IH.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     8021 2024-04-09 21:55:14.000000 DESlib-0.3.6/deslib/tests/test_integration_dfp.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     6839 2024-04-09 21:55:14.000000 DESlib-0.3.6/deslib/tests/test_metric.py
-drwxr-xr-x   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        0 2024-04-09 22:34:51.756141 DESlib-0.3.6/deslib/tests/util/
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        0 2021-03-27 00:32:40.000000 DESlib-0.3.6/deslib/tests/util/__init__.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     5205 2021-03-27 00:32:40.000000 DESlib-0.3.6/deslib/tests/util/test_aggregation.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     1656 2021-03-27 00:32:40.000000 DESlib-0.3.6/deslib/tests/util/test_datasets.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     6205 2021-03-27 00:32:40.000000 DESlib-0.3.6/deslib/tests/util/test_diversity.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     4140 2024-04-09 21:55:14.000000 DESlib-0.3.6/deslib/tests/util/test_diversity_batch.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      852 2021-10-06 23:58:31.000000 DESlib-0.3.6/deslib/tests/util/test_faiss.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     2372 2021-03-27 00:32:40.000000 DESlib-0.3.6/deslib/tests/util/test_fire.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     1491 2021-03-29 03:42:00.000000 DESlib-0.3.6/deslib/tests/util/test_instance_hardness.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     2834 2021-03-27 00:32:40.000000 DESlib-0.3.6/deslib/tests/util/test_knne.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     5450 2021-03-29 03:42:00.000000 DESlib-0.3.6/deslib/tests/util/test_prob_functions.py
-drwxr-xr-x   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        0 2024-04-09 22:34:51.758313 DESlib-0.3.6/deslib/util/
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     1032 2021-03-27 00:32:40.000000 DESlib-0.3.6/deslib/util/__init__.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)    15221 2024-04-09 21:55:14.000000 DESlib-0.3.6/deslib/util/aggregation.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     9532 2021-03-27 00:32:40.000000 DESlib-0.3.6/deslib/util/datasets.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     4337 2021-03-27 00:32:40.000000 DESlib-0.3.6/deslib/util/dfp.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)    10449 2021-03-27 00:32:40.000000 DESlib-0.3.6/deslib/util/diversity.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)    11638 2024-04-09 21:55:14.000000 DESlib-0.3.6/deslib/util/diversity_batch.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     6774 2021-10-06 23:58:35.000000 DESlib-0.3.6/deslib/util/faiss_knn_wrapper.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     3096 2022-05-25 04:21:28.000000 DESlib-0.3.6/deslib/util/instance_hardness.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     9014 2021-10-06 23:58:35.000000 DESlib-0.3.6/deslib/util/knne.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     9614 2024-04-09 21:55:14.000000 DESlib-0.3.6/deslib/util/prob_functions.py
-drwxr-xr-x   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        0 2024-04-09 22:34:51.759510 DESlib-0.3.6/docs/
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     7409 2021-03-27 00:32:40.000000 DESlib-0.3.6/docs/Makefile
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     2105 2021-03-27 00:32:40.000000 DESlib-0.3.6/docs/api.rst
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)    10869 2021-03-27 00:32:40.000000 DESlib-0.3.6/docs/conf.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     4971 2021-03-27 00:32:40.000000 DESlib-0.3.6/docs/index.rst
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     7244 2021-03-27 00:32:40.000000 DESlib-0.3.6/docs/make.bat
-drwxr-xr-x   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        0 2024-04-09 22:34:51.730612 DESlib-0.3.6/docs/modules/
-drwxr-xr-x   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        0 2024-04-09 22:34:51.760520 DESlib-0.3.6/docs/modules/dcs/
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      173 2021-03-27 00:32:40.000000 DESlib-0.3.6/docs/modules/dcs/a_posteriori.rst
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      159 2021-03-27 00:32:40.000000 DESlib-0.3.6/docs/modules/dcs/a_priori.rst
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      184 2021-03-27 00:32:40.000000 DESlib-0.3.6/docs/modules/dcs/lca.rst
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      202 2021-03-27 00:32:40.000000 DESlib-0.3.6/docs/modules/dcs/mcb.rst
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      190 2021-03-27 00:32:40.000000 DESlib-0.3.6/docs/modules/dcs/mla.rst
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      189 2021-03-27 00:32:40.000000 DESlib-0.3.6/docs/modules/dcs/ola.rst
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      163 2021-03-27 00:32:40.000000 DESlib-0.3.6/docs/modules/dcs/rank.rst
-drwxr-xr-x   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        0 2024-04-09 22:34:51.762539 DESlib-0.3.6/docs/modules/des/
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      181 2021-03-27 00:32:40.000000 DESlib-0.3.6/docs/modules/des/des_clustering.rst
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      227 2021-03-27 00:32:40.000000 DESlib-0.3.6/docs/modules/des/des_p.rst
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      204 2021-03-27 00:32:40.000000 DESlib-0.3.6/docs/modules/des/deskl.rst
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      204 2021-03-27 00:32:40.000000 DESlib-0.3.6/docs/modules/des/desmi.rst
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      160 2021-03-27 00:32:40.000000 DESlib-0.3.6/docs/modules/des/ds_knn.rst
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      199 2021-03-27 00:32:40.000000 DESlib-0.3.6/docs/modules/des/exponential.rst
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      209 2021-03-27 00:32:40.000000 DESlib-0.3.6/docs/modules/des/knop.rst
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      213 2021-03-27 00:32:40.000000 DESlib-0.3.6/docs/modules/des/knora_e.rst
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      203 2021-03-27 00:32:40.000000 DESlib-0.3.6/docs/modules/des/knora_u.rst
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      198 2021-03-27 00:32:40.000000 DESlib-0.3.6/docs/modules/des/logarithmic.rst
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      168 2021-03-27 00:32:40.000000 DESlib-0.3.6/docs/modules/des/meta_des.rst
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      218 2021-03-27 00:32:40.000000 DESlib-0.3.6/docs/modules/des/minimum_difference.rst
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      205 2021-03-27 00:32:40.000000 DESlib-0.3.6/docs/modules/des/probabilistic.rst
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      234 2021-03-27 00:32:40.000000 DESlib-0.3.6/docs/modules/des/rrc.rst
-drwxr-xr-x   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        0 2024-04-09 22:34:51.763113 DESlib-0.3.6/docs/modules/static/
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)       98 2021-03-27 00:32:40.000000 DESlib-0.3.6/docs/modules/static/oracle.rst
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      147 2021-03-27 00:32:40.000000 DESlib-0.3.6/docs/modules/static/single_best.rst
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      160 2021-03-27 00:32:40.000000 DESlib-0.3.6/docs/modules/static/stacked.rst
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      163 2021-03-27 00:32:40.000000 DESlib-0.3.6/docs/modules/static/static_selection.rst
-drwxr-xr-x   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        0 2024-04-09 22:34:51.764420 DESlib-0.3.6/docs/modules/util/
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      231 2021-03-27 00:32:40.000000 DESlib-0.3.6/docs/modules/util/aggregation.rst
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      276 2021-03-27 00:32:40.000000 DESlib-0.3.6/docs/modules/util/datasets.rst
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)       80 2021-03-27 00:32:40.000000 DESlib-0.3.6/docs/modules/util/dfp.rst
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      360 2021-03-27 00:32:40.000000 DESlib-0.3.6/docs/modules/util/diversity.rst
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      165 2021-03-27 00:32:40.000000 DESlib-0.3.6/docs/modules/util/faiss_knn_wrapper.rst
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      182 2021-03-27 00:32:40.000000 DESlib-0.3.6/docs/modules/util/instance_hardness.rst
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      135 2021-03-27 00:32:40.000000 DESlib-0.3.6/docs/modules/util/knne.rst
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      285 2021-03-27 00:32:40.000000 DESlib-0.3.6/docs/modules/util/prob_functions.rst
-drwxr-xr-x   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        0 2024-04-09 22:34:51.765146 DESlib-0.3.6/docs/news/
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     1153 2021-03-27 00:32:40.000000 DESlib-0.3.6/docs/news/v0.1.rst
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      920 2021-03-27 00:32:40.000000 DESlib-0.3.6/docs/news/v0.2.rst
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     1622 2021-03-29 03:42:00.000000 DESlib-0.3.6/docs/news/v0.3.5.rst
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     2501 2021-03-27 00:32:40.000000 DESlib-0.3.6/docs/news/v0.3.rst
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      228 2021-03-27 00:32:40.000000 DESlib-0.3.6/docs/news.rst
-drwxr-xr-x   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        0 2024-04-09 22:34:51.765859 DESlib-0.3.6/docs/user_guide/
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     4093 2021-03-27 00:32:40.000000 DESlib-0.3.6/docs/user_guide/development.rst
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      803 2021-03-27 00:32:40.000000 DESlib-0.3.6/docs/user_guide/installation.rst
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      737 2021-03-27 00:32:40.000000 DESlib-0.3.6/docs/user_guide/known_issues.rst
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     3204 2021-03-27 00:32:40.000000 DESlib-0.3.6/docs/user_guide/packaging.rst
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)    11982 2021-03-27 00:32:40.000000 DESlib-0.3.6/docs/user_guide/tutorial.rst
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      435 2021-03-27 00:32:40.000000 DESlib-0.3.6/docs/user_guide.rst
-drwxr-xr-x   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        0 2024-04-09 22:34:51.768046 DESlib-0.3.6/examples/
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     5431 2021-03-29 03:42:00.000000 DESlib-0.3.6/examples/example_calibrating_classifiers.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     4920 2022-05-25 04:21:28.000000 DESlib-0.3.6/examples/example_heterogeneous.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     6411 2021-03-27 00:32:40.000000 DESlib-0.3.6/examples/plot_comparing_dynamic_static.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     4959 2021-03-27 00:32:40.000000 DESlib-0.3.6/examples/plot_example_DFP.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     8338 2021-03-27 00:32:40.000000 DESlib-0.3.6/examples/plot_example_P2.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     3250 2021-03-29 03:42:00.000000 DESlib-0.3.6/examples/plot_influence_k_value.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     4708 2022-05-25 04:21:28.000000 DESlib-0.3.6/examples/plot_random_forest.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     4349 2022-05-25 04:21:28.000000 DESlib-0.3.6/examples/plot_using_instance_hardness.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     5904 2021-03-27 00:32:40.000000 DESlib-0.3.6/examples/plot_xor_example.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     1787 2021-03-27 00:32:40.000000 DESlib-0.3.6/examples/simple_example.py
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      148 2024-04-09 21:55:14.000000 DESlib-0.3.6/requirements-dev.txt
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)       46 2022-06-07 03:49:32.000000 DESlib-0.3.6/requirements.txt
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)       38 2024-04-09 22:34:51.768602 DESlib-0.3.6/setup.cfg
--rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     1407 2024-04-09 21:57:57.000000 DESlib-0.3.6/setup.py
+drwxr-xr-x   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        0 2024-04-12 01:14:23.710571 DESlib-0.3.7/
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     3469 2021-03-27 00:32:40.000000 DESlib-0.3.7/CONTRIBUTING.md
+drwxr-xr-x   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        0 2024-04-12 01:14:23.665852 DESlib-0.3.7/DESlib.egg-info/
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)    13351 2024-04-12 01:14:23.000000 DESlib-0.3.7/DESlib.egg-info/PKG-INFO
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     4524 2024-04-12 01:14:23.000000 DESlib-0.3.7/DESlib.egg-info/SOURCES.txt
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        1 2024-04-12 01:14:23.000000 DESlib-0.3.7/DESlib.egg-info/dependency_links.txt
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)       47 2024-04-12 01:14:23.000000 DESlib-0.3.7/DESlib.egg-info/requires.txt
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        7 2024-04-12 01:14:23.000000 DESlib-0.3.7/DESlib.egg-info/top_level.txt
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     1476 2021-03-27 00:32:40.000000 DESlib-0.3.7/LICENSE.txt
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      207 2021-03-27 00:32:40.000000 DESlib-0.3.7/MANIFEST.in
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)    13351 2024-04-12 01:14:23.709909 DESlib-0.3.7/PKG-INFO
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)    12142 2024-04-12 00:52:16.000000 DESlib-0.3.7/README.rst
+drwxr-xr-x   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        0 2024-04-12 01:14:23.666433 DESlib-0.3.7/deslib/
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      704 2024-04-12 01:09:26.000000 DESlib-0.3.7/deslib/__init__.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)    28533 2024-04-11 05:36:17.000000 DESlib-0.3.7/deslib/base.py
+drwxr-xr-x   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        0 2024-04-12 01:14:23.670765 DESlib-0.3.7/deslib/dcs/
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      463 2021-03-27 00:32:40.000000 DESlib-0.3.7/deslib/dcs/__init__.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)    11054 2022-05-25 04:21:28.000000 DESlib-0.3.7/deslib/dcs/a_posteriori.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     9017 2022-05-25 04:21:28.000000 DESlib-0.3.7/deslib/dcs/a_priori.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)    12386 2024-04-09 21:55:14.000000 DESlib-0.3.7/deslib/dcs/base.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     8422 2022-05-25 04:21:28.000000 DESlib-0.3.7/deslib/dcs/lca.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)    10359 2022-05-25 04:21:28.000000 DESlib-0.3.7/deslib/dcs/mcb.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     9352 2022-05-25 04:21:28.000000 DESlib-0.3.7/deslib/dcs/mla.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     7136 2022-05-25 04:21:28.000000 DESlib-0.3.7/deslib/dcs/ola.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     7802 2022-05-25 04:21:28.000000 DESlib-0.3.7/deslib/dcs/rank.py
+drwxr-xr-x   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        0 2024-04-12 01:14:23.675641 DESlib-0.3.7/deslib/des/
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     1051 2021-03-27 00:32:40.000000 DESlib-0.3.7/deslib/des/__init__.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)    10416 2022-05-25 04:21:28.000000 DESlib-0.3.7/deslib/des/base.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)    17305 2024-04-09 21:55:14.000000 DESlib-0.3.7/deslib/des/des_clustering.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)    17511 2022-05-25 04:30:11.000000 DESlib-0.3.7/deslib/des/des_knn.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)    13483 2024-04-09 21:55:14.000000 DESlib-0.3.7/deslib/des/des_mi.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     7776 2022-05-25 05:13:52.000000 DESlib-0.3.7/deslib/des/des_p.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)    11615 2024-04-09 21:55:14.000000 DESlib-0.3.7/deslib/des/knop.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     9974 2024-04-09 21:55:14.000000 DESlib-0.3.7/deslib/des/knora_e.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     7682 2024-04-09 21:55:14.000000 DESlib-0.3.7/deslib/des/knora_u.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)    23083 2024-04-12 00:52:16.000000 DESlib-0.3.7/deslib/des/meta_des.py
+drwxr-xr-x   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        0 2024-04-12 01:14:23.678306 DESlib-0.3.7/deslib/des/probabilistic/
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      362 2021-03-27 00:32:40.000000 DESlib-0.3.7/deslib/des/probabilistic/__init__.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     7287 2022-05-25 04:21:28.000000 DESlib-0.3.7/deslib/des/probabilistic/base.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     6473 2022-05-25 04:32:34.000000 DESlib-0.3.7/deslib/des/probabilistic/deskl.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     6478 2022-05-25 04:38:46.000000 DESlib-0.3.7/deslib/des/probabilistic/exponential.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     5704 2022-05-25 04:35:37.000000 DESlib-0.3.7/deslib/des/probabilistic/logarithmic.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     5902 2022-05-25 04:37:36.000000 DESlib-0.3.7/deslib/des/probabilistic/minimum_difference.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     5730 2022-05-25 04:38:04.000000 DESlib-0.3.7/deslib/des/probabilistic/rrc.py
+drwxr-xr-x   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        0 2024-04-12 01:14:23.680872 DESlib-0.3.7/deslib/static/
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      428 2021-03-27 00:32:40.000000 DESlib-0.3.7/deslib/static/__init__.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     5080 2022-06-06 05:38:53.000000 DESlib-0.3.7/deslib/static/base.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     5928 2024-04-09 21:55:14.000000 DESlib-0.3.7/deslib/static/oracle.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     6261 2024-04-09 21:55:14.000000 DESlib-0.3.7/deslib/static/single_best.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     7488 2024-04-09 21:55:14.000000 DESlib-0.3.7/deslib/static/stacked.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     7389 2024-04-09 21:55:14.000000 DESlib-0.3.7/deslib/static/static_selection.py
+drwxr-xr-x   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        0 2024-04-12 01:14:23.684461 DESlib-0.3.7/deslib/tests/
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)       24 2021-03-27 00:32:40.000000 DESlib-0.3.7/deslib/tests/__init__.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     6803 2022-05-25 04:21:28.000000 DESlib-0.3.7/deslib/tests/conftest.py
+drwxr-xr-x   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        0 2024-04-12 01:14:23.687825 DESlib-0.3.7/deslib/tests/dcs/
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        0 2021-03-27 00:32:40.000000 DESlib-0.3.7/deslib/tests/dcs/__init__.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     5773 2022-05-25 04:21:28.000000 DESlib-0.3.7/deslib/tests/dcs/test_a_posteriori.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     3497 2022-05-25 04:21:28.000000 DESlib-0.3.7/deslib/tests/dcs/test_a_priori.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)    10024 2022-05-25 04:21:28.000000 DESlib-0.3.7/deslib/tests/dcs/test_base.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     2558 2022-05-25 04:21:28.000000 DESlib-0.3.7/deslib/tests/dcs/test_lca.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     3822 2022-05-25 04:21:28.000000 DESlib-0.3.7/deslib/tests/dcs/test_mcb.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     4250 2022-05-25 04:21:28.000000 DESlib-0.3.7/deslib/tests/dcs/test_mla.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     1215 2022-05-25 04:21:28.000000 DESlib-0.3.7/deslib/tests/dcs/test_ola.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     1099 2022-05-25 04:21:28.000000 DESlib-0.3.7/deslib/tests/dcs/test_rank.py
+drwxr-xr-x   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        0 2024-04-12 01:14:23.690867 DESlib-0.3.7/deslib/tests/des/
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        0 2021-03-27 00:32:40.000000 DESlib-0.3.7/deslib/tests/des/__init__.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     9310 2022-05-25 04:21:28.000000 DESlib-0.3.7/deslib/tests/des/test_base.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     8713 2022-05-25 04:21:28.000000 DESlib-0.3.7/deslib/tests/des/test_des_clustering.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)    10425 2022-05-25 04:21:28.000000 DESlib-0.3.7/deslib/tests/des/test_des_knn.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     5035 2022-05-25 04:21:28.000000 DESlib-0.3.7/deslib/tests/des/test_des_mi.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     2597 2022-05-25 04:21:28.000000 DESlib-0.3.7/deslib/tests/des/test_desp.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     2650 2021-03-29 03:42:00.000000 DESlib-0.3.7/deslib/tests/des/test_knop.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     2394 2022-05-25 04:21:28.000000 DESlib-0.3.7/deslib/tests/des/test_knorae.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     1587 2022-05-25 04:21:28.000000 DESlib-0.3.7/deslib/tests/des/test_knorau.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     9165 2024-04-12 00:52:16.000000 DESlib-0.3.7/deslib/tests/des/test_meta_des.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)    11213 2022-05-25 04:21:28.000000 DESlib-0.3.7/deslib/tests/des/test_probabilistic.py
+drwxr-xr-x   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        0 2024-04-12 01:14:23.692180 DESlib-0.3.7/deslib/tests/static/
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        0 2021-03-27 00:32:40.000000 DESlib-0.3.7/deslib/tests/static/__init__.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     2131 2024-04-09 21:55:14.000000 DESlib-0.3.7/deslib/tests/static/test_oracle.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     3544 2024-04-09 21:55:14.000000 DESlib-0.3.7/deslib/tests/static/test_single_best.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     3172 2024-04-09 21:55:14.000000 DESlib-0.3.7/deslib/tests/static/test_stacked.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     4534 2024-04-09 21:55:14.000000 DESlib-0.3.7/deslib/tests/static/test_static_selection.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)    11190 2022-05-25 04:21:28.000000 DESlib-0.3.7/deslib/tests/test_base.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)    21249 2024-04-12 00:52:16.000000 DESlib-0.3.7/deslib/tests/test_des_integration.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     3389 2021-03-27 00:32:40.000000 DESlib-0.3.7/deslib/tests/test_des_integration_multiclass.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     2929 2024-04-12 00:52:16.000000 DESlib-0.3.7/deslib/tests/test_integration_DFP_IH.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     8021 2024-04-09 21:55:14.000000 DESlib-0.3.7/deslib/tests/test_integration_dfp.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     6839 2024-04-09 21:55:14.000000 DESlib-0.3.7/deslib/tests/test_metric.py
+drwxr-xr-x   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        0 2024-04-12 01:14:23.696275 DESlib-0.3.7/deslib/tests/util/
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        0 2021-03-27 00:32:40.000000 DESlib-0.3.7/deslib/tests/util/__init__.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     5205 2021-03-27 00:32:40.000000 DESlib-0.3.7/deslib/tests/util/test_aggregation.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     1656 2021-03-27 00:32:40.000000 DESlib-0.3.7/deslib/tests/util/test_datasets.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     6205 2021-03-27 00:32:40.000000 DESlib-0.3.7/deslib/tests/util/test_diversity.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     4140 2024-04-09 21:55:14.000000 DESlib-0.3.7/deslib/tests/util/test_diversity_batch.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      852 2021-10-06 23:58:31.000000 DESlib-0.3.7/deslib/tests/util/test_faiss.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     2372 2021-03-27 00:32:40.000000 DESlib-0.3.7/deslib/tests/util/test_fire.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     1491 2021-03-29 03:42:00.000000 DESlib-0.3.7/deslib/tests/util/test_instance_hardness.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     2834 2021-03-27 00:32:40.000000 DESlib-0.3.7/deslib/tests/util/test_knne.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     5450 2021-03-29 03:42:00.000000 DESlib-0.3.7/deslib/tests/util/test_prob_functions.py
+drwxr-xr-x   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        0 2024-04-12 01:14:23.698924 DESlib-0.3.7/deslib/util/
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     1032 2021-03-27 00:32:40.000000 DESlib-0.3.7/deslib/util/__init__.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)    15221 2024-04-09 21:55:14.000000 DESlib-0.3.7/deslib/util/aggregation.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     9532 2021-03-27 00:32:40.000000 DESlib-0.3.7/deslib/util/datasets.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     4337 2021-03-27 00:32:40.000000 DESlib-0.3.7/deslib/util/dfp.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)    10449 2021-03-27 00:32:40.000000 DESlib-0.3.7/deslib/util/diversity.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)    11638 2024-04-09 21:55:14.000000 DESlib-0.3.7/deslib/util/diversity_batch.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     6774 2021-10-06 23:58:35.000000 DESlib-0.3.7/deslib/util/faiss_knn_wrapper.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     3096 2022-05-25 04:21:28.000000 DESlib-0.3.7/deslib/util/instance_hardness.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     9014 2021-10-06 23:58:35.000000 DESlib-0.3.7/deslib/util/knne.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     9614 2024-04-09 21:55:14.000000 DESlib-0.3.7/deslib/util/prob_functions.py
+drwxr-xr-x   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        0 2024-04-12 01:14:23.700556 DESlib-0.3.7/docs/
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     7409 2021-03-27 00:32:40.000000 DESlib-0.3.7/docs/Makefile
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     2105 2021-03-27 00:32:40.000000 DESlib-0.3.7/docs/api.rst
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)    10869 2021-03-27 00:32:40.000000 DESlib-0.3.7/docs/conf.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     4971 2021-03-27 00:32:40.000000 DESlib-0.3.7/docs/index.rst
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     7244 2021-03-27 00:32:40.000000 DESlib-0.3.7/docs/make.bat
+drwxr-xr-x   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        0 2024-04-12 01:14:23.662784 DESlib-0.3.7/docs/modules/
+drwxr-xr-x   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        0 2024-04-12 01:14:23.701614 DESlib-0.3.7/docs/modules/dcs/
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      173 2021-03-27 00:32:40.000000 DESlib-0.3.7/docs/modules/dcs/a_posteriori.rst
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      159 2021-03-27 00:32:40.000000 DESlib-0.3.7/docs/modules/dcs/a_priori.rst
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      184 2021-03-27 00:32:40.000000 DESlib-0.3.7/docs/modules/dcs/lca.rst
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      202 2021-03-27 00:32:40.000000 DESlib-0.3.7/docs/modules/dcs/mcb.rst
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      190 2021-03-27 00:32:40.000000 DESlib-0.3.7/docs/modules/dcs/mla.rst
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      189 2021-03-27 00:32:40.000000 DESlib-0.3.7/docs/modules/dcs/ola.rst
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      163 2021-03-27 00:32:40.000000 DESlib-0.3.7/docs/modules/dcs/rank.rst
+drwxr-xr-x   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        0 2024-04-12 01:14:23.703694 DESlib-0.3.7/docs/modules/des/
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      181 2021-03-27 00:32:40.000000 DESlib-0.3.7/docs/modules/des/des_clustering.rst
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      227 2021-03-27 00:32:40.000000 DESlib-0.3.7/docs/modules/des/des_p.rst
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      204 2021-03-27 00:32:40.000000 DESlib-0.3.7/docs/modules/des/deskl.rst
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      204 2021-03-27 00:32:40.000000 DESlib-0.3.7/docs/modules/des/desmi.rst
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      160 2021-03-27 00:32:40.000000 DESlib-0.3.7/docs/modules/des/ds_knn.rst
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      199 2021-03-27 00:32:40.000000 DESlib-0.3.7/docs/modules/des/exponential.rst
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      209 2021-03-27 00:32:40.000000 DESlib-0.3.7/docs/modules/des/knop.rst
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      213 2021-03-27 00:32:40.000000 DESlib-0.3.7/docs/modules/des/knora_e.rst
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      203 2021-03-27 00:32:40.000000 DESlib-0.3.7/docs/modules/des/knora_u.rst
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      198 2021-03-27 00:32:40.000000 DESlib-0.3.7/docs/modules/des/logarithmic.rst
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      168 2021-03-27 00:32:40.000000 DESlib-0.3.7/docs/modules/des/meta_des.rst
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      218 2021-03-27 00:32:40.000000 DESlib-0.3.7/docs/modules/des/minimum_difference.rst
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      205 2021-03-27 00:32:40.000000 DESlib-0.3.7/docs/modules/des/probabilistic.rst
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      234 2021-03-27 00:32:40.000000 DESlib-0.3.7/docs/modules/des/rrc.rst
+drwxr-xr-x   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        0 2024-04-12 01:14:23.704330 DESlib-0.3.7/docs/modules/static/
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)       98 2021-03-27 00:32:40.000000 DESlib-0.3.7/docs/modules/static/oracle.rst
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      147 2021-03-27 00:32:40.000000 DESlib-0.3.7/docs/modules/static/single_best.rst
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      160 2021-03-27 00:32:40.000000 DESlib-0.3.7/docs/modules/static/stacked.rst
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      163 2021-03-27 00:32:40.000000 DESlib-0.3.7/docs/modules/static/static_selection.rst
+drwxr-xr-x   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        0 2024-04-12 01:14:23.705553 DESlib-0.3.7/docs/modules/util/
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      231 2021-03-27 00:32:40.000000 DESlib-0.3.7/docs/modules/util/aggregation.rst
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      276 2021-03-27 00:32:40.000000 DESlib-0.3.7/docs/modules/util/datasets.rst
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)       80 2021-03-27 00:32:40.000000 DESlib-0.3.7/docs/modules/util/dfp.rst
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      360 2021-03-27 00:32:40.000000 DESlib-0.3.7/docs/modules/util/diversity.rst
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      165 2021-03-27 00:32:40.000000 DESlib-0.3.7/docs/modules/util/faiss_knn_wrapper.rst
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      182 2021-03-27 00:32:40.000000 DESlib-0.3.7/docs/modules/util/instance_hardness.rst
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      135 2021-03-27 00:32:40.000000 DESlib-0.3.7/docs/modules/util/knne.rst
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      285 2021-03-27 00:32:40.000000 DESlib-0.3.7/docs/modules/util/prob_functions.rst
+drwxr-xr-x   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        0 2024-04-12 01:14:23.706189 DESlib-0.3.7/docs/news/
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     1153 2021-03-27 00:32:40.000000 DESlib-0.3.7/docs/news/v0.1.rst
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      920 2021-03-27 00:32:40.000000 DESlib-0.3.7/docs/news/v0.2.rst
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     1622 2021-03-29 03:42:00.000000 DESlib-0.3.7/docs/news/v0.3.5.rst
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     2501 2021-03-27 00:32:40.000000 DESlib-0.3.7/docs/news/v0.3.rst
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      228 2021-03-27 00:32:40.000000 DESlib-0.3.7/docs/news.rst
+drwxr-xr-x   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        0 2024-04-12 01:14:23.706947 DESlib-0.3.7/docs/user_guide/
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     4093 2021-03-27 00:32:40.000000 DESlib-0.3.7/docs/user_guide/development.rst
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      803 2021-03-27 00:32:40.000000 DESlib-0.3.7/docs/user_guide/installation.rst
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      737 2021-03-27 00:32:40.000000 DESlib-0.3.7/docs/user_guide/known_issues.rst
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     3204 2021-03-27 00:32:40.000000 DESlib-0.3.7/docs/user_guide/packaging.rst
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)    11982 2021-03-27 00:32:40.000000 DESlib-0.3.7/docs/user_guide/tutorial.rst
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      435 2021-03-27 00:32:40.000000 DESlib-0.3.7/docs/user_guide.rst
+drwxr-xr-x   0 rafaelmenelauoliveiraecruz   (501) staff       (20)        0 2024-04-12 01:14:23.709520 DESlib-0.3.7/examples/
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     5431 2021-03-29 03:42:00.000000 DESlib-0.3.7/examples/example_calibrating_classifiers.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     4920 2022-05-25 04:21:28.000000 DESlib-0.3.7/examples/example_heterogeneous.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     6411 2021-03-27 00:32:40.000000 DESlib-0.3.7/examples/plot_comparing_dynamic_static.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     4959 2021-03-27 00:32:40.000000 DESlib-0.3.7/examples/plot_example_DFP.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     8338 2021-03-27 00:32:40.000000 DESlib-0.3.7/examples/plot_example_P2.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     3250 2021-03-29 03:42:00.000000 DESlib-0.3.7/examples/plot_influence_k_value.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     4708 2022-05-25 04:21:28.000000 DESlib-0.3.7/examples/plot_random_forest.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     4349 2022-05-25 04:21:28.000000 DESlib-0.3.7/examples/plot_using_instance_hardness.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     5904 2021-03-27 00:32:40.000000 DESlib-0.3.7/examples/plot_xor_example.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     1787 2021-03-27 00:32:40.000000 DESlib-0.3.7/examples/simple_example.py
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)      148 2024-04-12 00:52:16.000000 DESlib-0.3.7/requirements-dev.txt
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)       47 2024-04-12 00:52:16.000000 DESlib-0.3.7/requirements.txt
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)       38 2024-04-12 01:14:23.710621 DESlib-0.3.7/setup.cfg
+-rw-r--r--   0 rafaelmenelauoliveiraecruz   (501) staff       (20)     1664 2024-04-12 01:09:26.000000 DESlib-0.3.7/setup.py
```

### Comparing `DESlib-0.3.6/CONTRIBUTING.md` & `DESlib-0.3.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/DESlib.egg-info/PKG-INFO` & `DESlib-0.3.7/DESlib.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,250 +1,272 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: DESlib
-Version: 0.3.6
+Version: 0.3.7
 Summary: Implementation of Dynamic Ensemble Selection methods
 Home-page: https://github.com/Menelau/DESlib
 Author: Rafael M. O. Cruz
 Author-email: rafaelmenelau@gmail.com
 Maintainer: Rafael M. O. Cruz, L. G. Hafemann
 Maintainer-email: rafaelmenelau@gmail.com
 License: BSD 3-clause "New" or "Revised License"
-Description: .. image:: https://readthedocs.org/projects/deslib/badge/?version=latest
-            :target: http://deslib.readthedocs.io/en/latest/?badge=latest
-            :alt: Documentation Status
-        
-        .. image:: https://circleci.com/gh/scikit-learn-contrib/DESlib.svg?style=shield
-            :target: https://circleci.com/gh/scikit-learn-contrib/DESlib
-        
-        .. image:: https://travis-ci.org/scikit-learn-contrib/DESlib.svg?branch=master
-            :target: https://travis-ci.org/scikit-learn-contrib/DESlib
-        
-        .. image:: https://codecov.io/gh/scikit-learn-contrib/DESlib/branch/master/graph/badge.svg
-            :target: https://codecov.io/gh/scikit-learn-contrib/DESlib
-            
-        .. image:: https://api.codacy.com/project/badge/Grade/59500eecc5524c59b9eb2284b43ae3e6
-           :alt: Codacy Badge
-           :target: https://app.codacy.com/app/Menelau/DESlib?
-        
-        .. image:: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg
-            :target: https://opensource.org/licenses/BSD-3-Clause
-        
-        .. image:: https://badges.gitter.im/DESlib/gitter.png
-            :target: https://gitter.im/deslib/Lobby
-        
-        DESlib
-        ========
-        
-        DESlib is an easy-to-use ensemble learning library focused on the implementation of the state-of-the-art techniques for dynamic classifier and ensemble selection.
-        The library is is based on scikit-learn_, using the same method signatures: **fit**, **predict**, **predict_proba** and **score**.
-        All dynamic selection techniques were implemented according to the definitions from [1]_.
-        
-        Dynamic Selection:
-        -------------------
-        
-        Dynamic Selection (DS) refers to techniques in which the base classifiers are selected
-        dynamically at test time, according to each new sample to be classified. Only the most competent, or an ensemble of the most competent classifiers is selected to predict
-        the label of a specific test sample. The rationale for these techniques is that not every classifier in
-        the pool is an expert in classifying all unknown samples, but rather each base classifier is an expert in
-        a different local region of the feature space.
-        
-        DS is one of the most promising MCS approaches (Multiple Classifier Systems) due to an increasing number of empirical studies
-        reporting superior performance over static combination methods. Such techniques
-        have achieved better classification performance especially when dealing with small-sized and imbalanced datasets.
-        
-        Installation:
-        -------------
-        
-        The package can be installed using pip:
-        
-        Stable version:
-        
-        .. code-block:: bash
-        
-            pip install deslib
-        
-        Latest version (under development):
-        
-        .. code-block:: bash
-        
-            pip install git+https://github.com/scikit-learn-contrib/DESlib
-        
-        
-        Dependencies:
-        -------------
-        
-        DESlib is tested to work with Python 3.5, 3.6 and 3.7. The dependency requirements are:
-        
-        * scipy(>=1.4.0)
-        * numpy(>=1.17.0)
-        * scikit-learn(>=0.20.0)
-        
-        These dependencies are automatically installed using the pip commands above.
-        
-        Examples:
-        ---------
-        
-        Here we show an example using the KNORA-E method with random forest as a pool of classifiers:
-        
-        .. code-block:: python
-        
-            from deslib.des.knora_e import KNORAE
-        
-            # Train a pool of 10 classifiers
-            pool_classifiers = RandomForestClassifier(n_estimators=10)
-            pool_classifiers.fit(X_train, y_train)
-        
-            # Initialize the DES model
-            knorae = KNORAE(pool_classifiers)
-        
-            # Preprocess the Dynamic Selection dataset (DSEL)
-            knorae.fit(X_dsel, y_dsel)
-        
-            # Predict new examples:
-            knorae.predict(X_test)
-        
-        The library accepts any list of classifiers (compatible with scikit-learn) as input, including a list containing different classifier models (heterogeneous ensembles).
-        More examples on how to use the API can be found in the documentation_ and in the Examples directory.
-        
-        Organization:
-        -------------
-        
-        The library is divided into four modules:
-        
-        1. deslib.des: Implementation of DES techniques (Dynamic Ensemble Selection).
-        2. deslib.dcs: Implementation of DCS techniques (Dynamic Classifier Selection).
-        3. deslib.static: Implementation of baseline ensemble methods.
-        4. deslib.util: A collection of aggregation functions and diversity measures for ensemble of classifiers.
-        
-        * DES techniques currently available are:
-            1. META-DES [7]_ [8]_ [15]_
-            2. K-Nearest-Oracle-Eliminate (KNORA-E) [3]_
-            3. K-Nearest-Oracle-Union (KNORA-U) [3]_
-            4. Dynamic Ensemble Selection-Performance(DES-P) [12]_
-            5. K-Nearest-Output Profiles (KNOP) [9]_
-            6. Randomized Reference Classifier (DES-RRC) [10]_
-            7. DES Kullback-Leibler Divergence (DES-KL) [12]_
-            8. DES-Exponential [21]_
-            9. DES-Logarithmic [11]_
-            10. DES-Minimum Difference [21]_
-            11. DES-Clustering [16]_
-            12. DES-KNN [16]_
-            13. DES Multiclass Imbalance (DES-MI) [24]_
-        
-        * DCS techniques currently available are:
-            1. Modified Classifier Rank (Rank) [19]_
-            2. Overall Local Accuracy (OLA) [4]_
-            3. Local Class Accuracy (LCA) [4]_
-            4. Modified Local Accuracy (MLA) [23]_
-            5. Multiple Classifier Behaviour (MCB) [5]_
-            6. A Priori Selection (A Priori) [6]_
-            7. A Posteriori Selection (A Posteriori) [6]_
-        
-        * Baseline methods:
-            1. Oracle [20]_
-            2. Single Best [2]_
-            3. Static Selection [2]_
-            4. Stacked Classifier [25]_
-        
-        Variations of each DES techniques are also provided by the library (e.g., different versions of the META-DES framework).
-        
-        The following techniques are also available for all methods:
-         * For DES techniques, the combination of the selected classifiers can be done as Dynamic Selection (majority voting), Dynamic Weighting  (weighted majority voting) or a Hybrid (selection + weighting).
-         * For all DS techniques, Dynamic Frienemy Pruning (DFP) [13]_ can be used.
-         * For all DS techniques, Instance Hardness (IH) can be used to classify easy samples with a KNN and hard samples using the DS technique. More details on IH and Dynamic Selection can be found in [14]_.
-        
-        As an optional requirement, the fast KNN implementation from FAISS_ can be used to speed-up the computation of the region of competence.
-        
-        Citation
-        ---------
-        
-        If you use DESLib in a scientific paper, please consider citing the following paper:
-        
-        Rafael M. O. Cruz, Luiz G. Hafemann, Robert Sabourin and George D. C. Cavalcanti `DESlib: A Dynamic ensemble selection library in Python. <https://arxiv.org/abs/1802.04967>`_ arXiv preprint arXiv:1802.04967 (2018).
-        
-        .. code-block:: text
-        
-            @article{JMLR:v21:18-144,
-                author  = {Rafael M. O. Cruz and Luiz G. Hafemann and Robert Sabourin and George D. C. Cavalcanti},
-                title   = {DESlib: A Dynamic ensemble selection library in Python},
-                journal = {Journal of Machine Learning Research},
-                year    = {2020},
-                volume  = {21},
-                number  = {8},
-                pages   = {1-5},
-                url     = {http://jmlr.org/papers/v21/18-144.html}
-            }
-        
-        References:
-        -----------
-        
-        .. [1] : R. M. O. Cruz, R. Sabourin, and G. D. Cavalcanti, “Dynamic classifier selection: Recent advances and perspectives,” Information Fusion, vol. 41, pp. 195 – 216, 2018.
-        
-        .. [2] : A. S. Britto, R. Sabourin, L. E. S. de Oliveira, Dynamic selection of classifiers - A comprehensive review, Pattern Recognition 47 (11) (2014) 3665–3680.
-        
-        .. [3] : A. H. R. Ko, R. Sabourin, u. S. Britto, Jr., From dynamic classifier selection to dynamic ensemble selection, Pattern Recognition 41 (2008) 1735–1748.
-        
-        .. [4] : K. Woods, W. P. Kegelmeyer, Jr., K. Bowyer, Combination of multiple classifiers using local accuracy estimates, IEEE Transactions on Pattern Analysis Machine Intelligence 19 (1997) 405–410.
-        
-        .. [5] : G. Giacinto, F. Roli, Dynamic classifier selection based on multiple classifier behaviour, Pattern Recognition 34 (2001) 1879–1881.
-        
-        .. [6] : L. Didaci, G. Giacinto, F. Roli, G. L. Marcialis, A study on the performances of dynamic classifier selection based on local accuracy estimation, Pattern Recognition 38 (11) (2005) 2188–2191.
-        
-        .. [7] : R. M. O. Cruz, R. Sabourin, G. D. C. Cavalcanti, T. I. Ren, META-DES: A dynamic ensemble selection framework using meta-learning, Pattern Recognition 48 (5) (2015) 1925–1935.
-        
-        .. [8] : Cruz, R.M., Sabourin, R. and Cavalcanti, G.D., 2015, July. META-DES. H: a dynamic ensemble selection technique using meta-learning and a dynamic weighting approach. In Neural Networks (IJCNN), 2015 International Joint Conference on (pp. 1-8)
-        
-        .. [9] : P. R. Cavalin, R. Sabourin, C. Y. Suen, Dynamic selection approaches for multiple classifier systems, Neural Computing and Applications 22 (3-4) (2013) 673–688.
-        
-        .. [10] : T.Woloszynski, M. Kurzynski, A probabilistic model of classifier competence for dynamic ensemble selection, Pattern Recognition 44 (2011) 2656–2668.
-        
-        .. [11] : T.Woloszynski, M. Kurzynski, A measure of competence based on randomized reference classifier for dynamic ensemble selection, in: International Conference on Pattern Recognition (ICPR), 2010, pp. 4194–4197.
-        
-        .. [12] : T. Woloszynski, M. Kurzynski, P. Podsiadlo, G. W. Stachowiak, A measure of competence based on random classification for dynamic ensemble selection, Information Fusion 13 (3) (2012) 207–213.
-        
-        .. [13] : Oliveira, D.V.R., Cavalcanti, G.D.C. and Sabourin, R., Online Pruning of Base Classifiers for Dynamic Ensemble Selection, Pattern Recognition, vol. 72, December 2017, pp 44-58.
-        
-        .. [14] : Cruz RM, Zakane HH, Sabourin R, Cavalcanti GD. Dynamic Ensemble Selection VS K-NN: why and when Dynamic Selection obtains higher classification performance?.
-        
-        .. [15] : R. M. O. Cruz, R. Sabourin, G. D. C. Cavalcanti, META-DES.Oracle: Meta-learning and feature selection for dynamic ensemble selection, Information Fusion 38 (2017) 84–103.Nov 30;38:84-103.
-        
-        .. [16] : R. G. F. Soares, A. Santana, A. M. P. Canuto, M. C. P. de Souto, Using accuracy and diversity to select classifiers to build ensembles, Proceedings of the International Joint Conference on Neural Networks (2006) 1310–1316.
-        
-        .. [17] : L. I. Kuncheva, Combining Pattern Classifiers: Methods and Algorithms, Wiley-Interscience, 2004.
-        
-        .. [18] : Shipp, Catherine A., and Ludmila I. Kuncheva. "Relationships between combination methods and measures of diversity in combining classifiers." Information fusion 3.2 (2002): 135-148.
-        
-        .. [19] : M. Sabourin, A. Mitiche, D. Thomas, G. Nagy, Classifier combination for handprinted digit recognition, International Conference on Document Analysis and Recognition (1993) 163–166.
-        
-        .. [20] : L. I. Kuncheva, A theoretical study on six classifier fusion strategies, IEEE Transactions on Pattern Analysis and Machine Intelligence 24 (2) (2002) 281–286.
-        
-        .. [21] : B. Antosik, M. Kurzynski, New measures of classifier competence – heuristics and application to the design of multiple classifier systems., in: Computer recognition systems 4., 2011, pp. 197–206.
-        
-        .. [22] : Smith, Michael R., Tony Martinez, and Christophe Giraud-Carrier. "An instance level analysis of data complexity." Machine learning 95.2 (2014), pp 225-256.
-        
-        .. [23] : P. C. Smits, Multiple classifier systems for supervised remote sensing image classification based on dynamic classifier selection, IEEE Transactions on Geoscience and Remote Sensing 40 (4) (2002) 801–813.
-        
-        .. [24] : García, S., Zhang, Z.L., Altalhi, A., Alshomrani, S. and Herrera, F., "Dynamic ensemble selection for multi-class imbalanced datasets." Information Sciences 445 (2018): 22-37.
-        
-        .. [25] : Wolpert, David H. "Stacked generalization." Neural networks 5, no. 2 (1992): 241-259.
-        
-        .. _scikit-learn: http://scikit-learn.org/stable/
-        
-        .. _numpy: http://www.numpy.org/
-        
-        .. _scipy: https://www.scipy.org/
-        
-        .. _documentation: https://deslib.readthedocs.io
-        
-        .. _FAISS: https://github.com/facebookresearch/faiss
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3
+License-File: LICENSE.txt
+Requires-Dist: scikit-learn>=1.0.2
+Requires-Dist: numpy>=1.17.0
+Requires-Dist: scipy>=1.4.0
+
+.. -*- mode: rst -*-
+
+.. _scikit-learn-contrib: https://github.com/scikit-learn-contrib
+
+|Docs|_ |CircleCI|_ |BSD|_ |PyPi|_ |PythonVersion|_ |Downloads|_ |Wheel|_ |Black|_
+
+.. |Docs| image:: https://readthedocs.org/projects/deslib/badge/?version=latest
+..    _Docs: http://deslib.readthedocs.io/en/latest/?badge=latest
+
+.. |CircleCI| image:: https://circleci.com/gh/scikit-learn-contrib/DESlib.svg?style=shield
+..    _CircleCI: https://circleci.com/gh/scikit-learn-contrib/DESlib
+
+.. |BSD| image:: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg
+..    _BSD: https://opensource.org/licenses/BSD-3-Clause
+
+.. |PyPi| image:: https://badge.fury.io/py/DESlib.svg
+..    _PyPi: https://pypi.org/project/DESlib/
+
+.. |PythonVersion| image:: https://img.shields.io/pypi/pyversions/deslib.svg
+..   _PythonVersion: https://pypi.org/project/DESlib/
+
+.. |Downloads| image:: https://img.shields.io/pypi/dm/deslib.svg
+..   _Downloads: https://pypistats.org/packages/deslib
+
+.. |Wheel| image:: https://img.shields.io/pypi/wheel/deslib.svg
+..   _Wheel: https://img.shields.io/pypi/wheel/deslib.svg
+
+.. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+.. _Black: :target: https://github.com/psf/black
+
+
+.. |PythonMinVersion| replace:: 3.7
+.. |NumPyMinVersion| replace:: 1.17.3
+.. |SciPyMinVersion| replace:: 1.5.0
+.. |ScikitLearnMinVersion| replace:: 1.0.2
+
+DESlib
+========
+
+DESlib is an easy-to-use ensemble learning library focused on the implementation of the state-of-the-art techniques for dynamic classifier and ensemble selection.
+The library is is based on scikit-learn_, using the same method signatures: **fit**, **predict**, **predict_proba** and **score**.
+All dynamic selection techniques were implemented according to the definitions from [1]_.
+
+Dynamic Selection:
+-------------------
+
+Dynamic Selection (DS) refers to techniques in which the base classifiers are selected
+dynamically at test time, according to each new sample to be classified. Only the most competent, or an ensemble of the most competent classifiers is selected to predict
+the label of a specific test sample. The rationale for these techniques is that not every classifier in
+the pool is an expert in classifying all unknown samples, but rather each base classifier is an expert in
+a different local region of the feature space.
+
+DS is one of the most promising MCS approaches (Multiple Classifier Systems) due to an increasing number of empirical studies
+reporting superior performance over static combination methods. Such techniques
+have achieved better classification performance especially when dealing with small-sized and imbalanced datasets.
+
+Installation:
+-------------
+
+The package can be installed using pip:
+
+Stable version:
+
+.. code-block:: bash
+
+    pip install deslib
+
+Latest version (under development):
+
+.. code-block:: bash
+
+    pip install git+https://github.com/scikit-learn-contrib/DESlib
+
+
+Dependencies:
+-------------
+
+The dependency requirements are:
+
+- Python (>= |PythonMinVersion|)
+- NumPy (>= |NumPyMinVersion|)
+- SciPy (>= |SciPyMinVersion|)
+- Scikit-learn (>= |ScikitLearnMinVersion|)
+
+These dependencies are automatically installed using the pip commands above.
+
+Examples:
+---------
+
+Here we show an example using the KNORA-E method with random forest as a pool of classifiers:
+
+.. code-block:: python
+
+    from deslib.des.knora_e import KNORAE
+
+    # Train a pool of 10 classifiers
+    pool_classifiers = RandomForestClassifier(n_estimators=10)
+    pool_classifiers.fit(X_train, y_train)
+
+    # Initialize the DES model
+    knorae = KNORAE(pool_classifiers)
+
+    # Preprocess the Dynamic Selection dataset (DSEL)
+    knorae.fit(X_dsel, y_dsel)
+
+    # Predict new examples:
+    knorae.predict(X_test)
+
+The library accepts any list of classifiers (compatible with scikit-learn) as input, including a list containing different classifier models (heterogeneous ensembles).
+More examples on how to use the API can be found in the documentation_ and in the Examples directory.
+
+Organization:
+-------------
+
+The library is divided into four modules:
+
+1. deslib.des: Implementation of DES techniques (Dynamic Ensemble Selection).
+2. deslib.dcs: Implementation of DCS techniques (Dynamic Classifier Selection).
+3. deslib.static: Implementation of baseline ensemble methods.
+4. deslib.util: A collection of aggregation functions and diversity measures for ensemble of classifiers.
+
+* DES techniques currently available are:
+    1. META-DES [7]_ [8]_ [15]_
+    2. K-Nearest-Oracle-Eliminate (KNORA-E) [3]_
+    3. K-Nearest-Oracle-Union (KNORA-U) [3]_
+    4. Dynamic Ensemble Selection-Performance(DES-P) [12]_
+    5. K-Nearest-Output Profiles (KNOP) [9]_
+    6. Randomized Reference Classifier (DES-RRC) [10]_
+    7. DES Kullback-Leibler Divergence (DES-KL) [12]_
+    8. DES-Exponential [21]_
+    9. DES-Logarithmic [11]_
+    10. DES-Minimum Difference [21]_
+    11. DES-Clustering [16]_
+    12. DES-KNN [16]_
+    13. DES Multiclass Imbalance (DES-MI) [24]_
+
+* DCS techniques currently available are:
+    1. Modified Classifier Rank (Rank) [19]_
+    2. Overall Local Accuracy (OLA) [4]_
+    3. Local Class Accuracy (LCA) [4]_
+    4. Modified Local Accuracy (MLA) [23]_
+    5. Multiple Classifier Behaviour (MCB) [5]_
+    6. A Priori Selection (A Priori) [6]_
+    7. A Posteriori Selection (A Posteriori) [6]_
+
+* Baseline methods:
+    1. Oracle [20]_
+    2. Single Best [2]_
+    3. Static Selection [2]_
+    4. Stacked Classifier [25]_
+
+Variations of each DES techniques are also provided by the library (e.g., different versions of the META-DES framework).
+
+The following techniques are also available for all methods:
+ * For DES techniques, the combination of the selected classifiers can be done as Dynamic Selection (majority voting), Dynamic Weighting  (weighted majority voting) or a Hybrid (selection + weighting).
+ * For all DS techniques, Dynamic Frienemy Pruning (DFP) [13]_ can be used.
+ * For all DS techniques, Instance Hardness (IH) can be used to classify easy samples with a KNN and hard samples using the DS technique. More details on IH and Dynamic Selection can be found in [14]_.
+
+As an optional requirement, the fast KNN implementation from FAISS_ can be used to speed-up the computation of the region of competence on GPU.
+
+Citation
+---------
+
+If you use DESLib in a scientific paper, please consider citing the following paper:
+
+Rafael M. O. Cruz, Luiz G. Hafemann, Robert Sabourin and George D. C. Cavalcanti `DESlib: A Dynamic ensemble selection library in Python. <https://arxiv.org/abs/1802.04967>`_ arXiv preprint arXiv:1802.04967 (2018).
+
+.. code-block:: text
+
+    @article{JMLR:v21:18-144,
+        author  = {Rafael M. O. Cruz and Luiz G. Hafemann and Robert Sabourin and George D. C. Cavalcanti},
+        title   = {DESlib: A Dynamic ensemble selection library in Python},
+        journal = {Journal of Machine Learning Research},
+        year    = {2020},
+        volume  = {21},
+        number  = {8},
+        pages   = {1-5},
+        url     = {http://jmlr.org/papers/v21/18-144.html}
+    }
+
+References:
+-----------
+
+.. [1] : R. M. O. Cruz, R. Sabourin, and G. D. Cavalcanti, “Dynamic classifier selection: Recent advances and perspectives,” Information Fusion, vol. 41, pp. 195 – 216, 2018.
+
+.. [2] : A. S. Britto, R. Sabourin, L. E. S. de Oliveira, Dynamic selection of classifiers - A comprehensive review, Pattern Recognition 47 (11) (2014) 3665–3680.
+
+.. [3] : A. H. R. Ko, R. Sabourin, u. S. Britto, Jr., From dynamic classifier selection to dynamic ensemble selection, Pattern Recognition 41 (2008) 1735–1748.
+
+.. [4] : K. Woods, W. P. Kegelmeyer, Jr., K. Bowyer, Combination of multiple classifiers using local accuracy estimates, IEEE Transactions on Pattern Analysis Machine Intelligence 19 (1997) 405–410.
+
+.. [5] : G. Giacinto, F. Roli, Dynamic classifier selection based on multiple classifier behaviour, Pattern Recognition 34 (2001) 1879–1881.
+
+.. [6] : L. Didaci, G. Giacinto, F. Roli, G. L. Marcialis, A study on the performances of dynamic classifier selection based on local accuracy estimation, Pattern Recognition 38 (11) (2005) 2188–2191.
+
+.. [7] : R. M. O. Cruz, R. Sabourin, G. D. C. Cavalcanti, T. I. Ren, META-DES: A dynamic ensemble selection framework using meta-learning, Pattern Recognition 48 (5) (2015) 1925–1935.
+
+.. [8] : Cruz, R.M., Sabourin, R. and Cavalcanti, G.D., 2015, July. META-DES. H: a dynamic ensemble selection technique using meta-learning and a dynamic weighting approach. In Neural Networks (IJCNN), 2015 International Joint Conference on (pp. 1-8)
+
+.. [9] : P. R. Cavalin, R. Sabourin, C. Y. Suen, Dynamic selection approaches for multiple classifier systems, Neural Computing and Applications 22 (3-4) (2013) 673–688.
+
+.. [10] : T.Woloszynski, M. Kurzynski, A probabilistic model of classifier competence for dynamic ensemble selection, Pattern Recognition 44 (2011) 2656–2668.
+
+.. [11] : T.Woloszynski, M. Kurzynski, A measure of competence based on randomized reference classifier for dynamic ensemble selection, in: International Conference on Pattern Recognition (ICPR), 2010, pp. 4194–4197.
+
+.. [12] : T. Woloszynski, M. Kurzynski, P. Podsiadlo, G. W. Stachowiak, A measure of competence based on random classification for dynamic ensemble selection, Information Fusion 13 (3) (2012) 207–213.
+
+.. [13] : Oliveira, D.V.R., Cavalcanti, G.D.C. and Sabourin, R., Online Pruning of Base Classifiers for Dynamic Ensemble Selection, Pattern Recognition, vol. 72, December 2017, pp 44-58.
+
+.. [14] : Cruz RM, Zakane HH, Sabourin R, Cavalcanti GD. Dynamic Ensemble Selection VS K-NN: why and when Dynamic Selection obtains higher classification performance?.
+
+.. [15] : R. M. O. Cruz, R. Sabourin, G. D. C. Cavalcanti, META-DES.Oracle: Meta-learning and feature selection for dynamic ensemble selection, Information Fusion 38 (2017) 84–103.Nov 30;38:84-103.
+
+.. [16] : R. G. F. Soares, A. Santana, A. M. P. Canuto, M. C. P. de Souto, Using accuracy and diversity to select classifiers to build ensembles, Proceedings of the International Joint Conference on Neural Networks (2006) 1310–1316.
+
+.. [17] : L. I. Kuncheva, Combining Pattern Classifiers: Methods and Algorithms, Wiley-Interscience, 2004.
+
+.. [18] : Shipp, Catherine A., and Ludmila I. Kuncheva. "Relationships between combination methods and measures of diversity in combining classifiers." Information fusion 3.2 (2002): 135-148.
+
+.. [19] : M. Sabourin, A. Mitiche, D. Thomas, G. Nagy, Classifier combination for handprinted digit recognition, International Conference on Document Analysis and Recognition (1993) 163–166.
+
+.. [20] : L. I. Kuncheva, A theoretical study on six classifier fusion strategies, IEEE Transactions on Pattern Analysis and Machine Intelligence 24 (2) (2002) 281–286.
+
+.. [21] : B. Antosik, M. Kurzynski, New measures of classifier competence – heuristics and application to the design of multiple classifier systems., in: Computer recognition systems 4., 2011, pp. 197–206.
+
+.. [22] : Smith, Michael R., Tony Martinez, and Christophe Giraud-Carrier. "An instance level analysis of data complexity." Machine learning 95.2 (2014), pp 225-256.
+
+.. [23] : P. C. Smits, Multiple classifier systems for supervised remote sensing image classification based on dynamic classifier selection, IEEE Transactions on Geoscience and Remote Sensing 40 (4) (2002) 801–813.
+
+.. [24] : García, S., Zhang, Z.L., Altalhi, A., Alshomrani, S. and Herrera, F., "Dynamic ensemble selection for multi-class imbalanced datasets." Information Sciences 445 (2018): 22-37.
+
+.. [25] : Wolpert, David H. "Stacked generalization." Neural networks 5, no. 2 (1992): 241-259.
+
+.. _scikit-learn: http://scikit-learn.org/stable/
+
+.. _numpy: http://www.numpy.org/
+
+.. _scipy: https://www.scipy.org/
+
+.. _documentation: https://deslib.readthedocs.io
+
+.. _FAISS: https://github.com/facebookresearch/faiss
```

### Comparing `DESlib-0.3.6/DESlib.egg-info/SOURCES.txt` & `DESlib-0.3.7/DESlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/LICENSE.txt` & `DESlib-0.3.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/PKG-INFO` & `DESlib-0.3.7/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,250 +1,272 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: DESlib
-Version: 0.3.6
+Version: 0.3.7
 Summary: Implementation of Dynamic Ensemble Selection methods
 Home-page: https://github.com/Menelau/DESlib
 Author: Rafael M. O. Cruz
 Author-email: rafaelmenelau@gmail.com
 Maintainer: Rafael M. O. Cruz, L. G. Hafemann
 Maintainer-email: rafaelmenelau@gmail.com
 License: BSD 3-clause "New" or "Revised License"
-Description: .. image:: https://readthedocs.org/projects/deslib/badge/?version=latest
-            :target: http://deslib.readthedocs.io/en/latest/?badge=latest
-            :alt: Documentation Status
-        
-        .. image:: https://circleci.com/gh/scikit-learn-contrib/DESlib.svg?style=shield
-            :target: https://circleci.com/gh/scikit-learn-contrib/DESlib
-        
-        .. image:: https://travis-ci.org/scikit-learn-contrib/DESlib.svg?branch=master
-            :target: https://travis-ci.org/scikit-learn-contrib/DESlib
-        
-        .. image:: https://codecov.io/gh/scikit-learn-contrib/DESlib/branch/master/graph/badge.svg
-            :target: https://codecov.io/gh/scikit-learn-contrib/DESlib
-            
-        .. image:: https://api.codacy.com/project/badge/Grade/59500eecc5524c59b9eb2284b43ae3e6
-           :alt: Codacy Badge
-           :target: https://app.codacy.com/app/Menelau/DESlib?
-        
-        .. image:: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg
-            :target: https://opensource.org/licenses/BSD-3-Clause
-        
-        .. image:: https://badges.gitter.im/DESlib/gitter.png
-            :target: https://gitter.im/deslib/Lobby
-        
-        DESlib
-        ========
-        
-        DESlib is an easy-to-use ensemble learning library focused on the implementation of the state-of-the-art techniques for dynamic classifier and ensemble selection.
-        The library is is based on scikit-learn_, using the same method signatures: **fit**, **predict**, **predict_proba** and **score**.
-        All dynamic selection techniques were implemented according to the definitions from [1]_.
-        
-        Dynamic Selection:
-        -------------------
-        
-        Dynamic Selection (DS) refers to techniques in which the base classifiers are selected
-        dynamically at test time, according to each new sample to be classified. Only the most competent, or an ensemble of the most competent classifiers is selected to predict
-        the label of a specific test sample. The rationale for these techniques is that not every classifier in
-        the pool is an expert in classifying all unknown samples, but rather each base classifier is an expert in
-        a different local region of the feature space.
-        
-        DS is one of the most promising MCS approaches (Multiple Classifier Systems) due to an increasing number of empirical studies
-        reporting superior performance over static combination methods. Such techniques
-        have achieved better classification performance especially when dealing with small-sized and imbalanced datasets.
-        
-        Installation:
-        -------------
-        
-        The package can be installed using pip:
-        
-        Stable version:
-        
-        .. code-block:: bash
-        
-            pip install deslib
-        
-        Latest version (under development):
-        
-        .. code-block:: bash
-        
-            pip install git+https://github.com/scikit-learn-contrib/DESlib
-        
-        
-        Dependencies:
-        -------------
-        
-        DESlib is tested to work with Python 3.5, 3.6 and 3.7. The dependency requirements are:
-        
-        * scipy(>=1.4.0)
-        * numpy(>=1.17.0)
-        * scikit-learn(>=0.20.0)
-        
-        These dependencies are automatically installed using the pip commands above.
-        
-        Examples:
-        ---------
-        
-        Here we show an example using the KNORA-E method with random forest as a pool of classifiers:
-        
-        .. code-block:: python
-        
-            from deslib.des.knora_e import KNORAE
-        
-            # Train a pool of 10 classifiers
-            pool_classifiers = RandomForestClassifier(n_estimators=10)
-            pool_classifiers.fit(X_train, y_train)
-        
-            # Initialize the DES model
-            knorae = KNORAE(pool_classifiers)
-        
-            # Preprocess the Dynamic Selection dataset (DSEL)
-            knorae.fit(X_dsel, y_dsel)
-        
-            # Predict new examples:
-            knorae.predict(X_test)
-        
-        The library accepts any list of classifiers (compatible with scikit-learn) as input, including a list containing different classifier models (heterogeneous ensembles).
-        More examples on how to use the API can be found in the documentation_ and in the Examples directory.
-        
-        Organization:
-        -------------
-        
-        The library is divided into four modules:
-        
-        1. deslib.des: Implementation of DES techniques (Dynamic Ensemble Selection).
-        2. deslib.dcs: Implementation of DCS techniques (Dynamic Classifier Selection).
-        3. deslib.static: Implementation of baseline ensemble methods.
-        4. deslib.util: A collection of aggregation functions and diversity measures for ensemble of classifiers.
-        
-        * DES techniques currently available are:
-            1. META-DES [7]_ [8]_ [15]_
-            2. K-Nearest-Oracle-Eliminate (KNORA-E) [3]_
-            3. K-Nearest-Oracle-Union (KNORA-U) [3]_
-            4. Dynamic Ensemble Selection-Performance(DES-P) [12]_
-            5. K-Nearest-Output Profiles (KNOP) [9]_
-            6. Randomized Reference Classifier (DES-RRC) [10]_
-            7. DES Kullback-Leibler Divergence (DES-KL) [12]_
-            8. DES-Exponential [21]_
-            9. DES-Logarithmic [11]_
-            10. DES-Minimum Difference [21]_
-            11. DES-Clustering [16]_
-            12. DES-KNN [16]_
-            13. DES Multiclass Imbalance (DES-MI) [24]_
-        
-        * DCS techniques currently available are:
-            1. Modified Classifier Rank (Rank) [19]_
-            2. Overall Local Accuracy (OLA) [4]_
-            3. Local Class Accuracy (LCA) [4]_
-            4. Modified Local Accuracy (MLA) [23]_
-            5. Multiple Classifier Behaviour (MCB) [5]_
-            6. A Priori Selection (A Priori) [6]_
-            7. A Posteriori Selection (A Posteriori) [6]_
-        
-        * Baseline methods:
-            1. Oracle [20]_
-            2. Single Best [2]_
-            3. Static Selection [2]_
-            4. Stacked Classifier [25]_
-        
-        Variations of each DES techniques are also provided by the library (e.g., different versions of the META-DES framework).
-        
-        The following techniques are also available for all methods:
-         * For DES techniques, the combination of the selected classifiers can be done as Dynamic Selection (majority voting), Dynamic Weighting  (weighted majority voting) or a Hybrid (selection + weighting).
-         * For all DS techniques, Dynamic Frienemy Pruning (DFP) [13]_ can be used.
-         * For all DS techniques, Instance Hardness (IH) can be used to classify easy samples with a KNN and hard samples using the DS technique. More details on IH and Dynamic Selection can be found in [14]_.
-        
-        As an optional requirement, the fast KNN implementation from FAISS_ can be used to speed-up the computation of the region of competence.
-        
-        Citation
-        ---------
-        
-        If you use DESLib in a scientific paper, please consider citing the following paper:
-        
-        Rafael M. O. Cruz, Luiz G. Hafemann, Robert Sabourin and George D. C. Cavalcanti `DESlib: A Dynamic ensemble selection library in Python. <https://arxiv.org/abs/1802.04967>`_ arXiv preprint arXiv:1802.04967 (2018).
-        
-        .. code-block:: text
-        
-            @article{JMLR:v21:18-144,
-                author  = {Rafael M. O. Cruz and Luiz G. Hafemann and Robert Sabourin and George D. C. Cavalcanti},
-                title   = {DESlib: A Dynamic ensemble selection library in Python},
-                journal = {Journal of Machine Learning Research},
-                year    = {2020},
-                volume  = {21},
-                number  = {8},
-                pages   = {1-5},
-                url     = {http://jmlr.org/papers/v21/18-144.html}
-            }
-        
-        References:
-        -----------
-        
-        .. [1] : R. M. O. Cruz, R. Sabourin, and G. D. Cavalcanti, “Dynamic classifier selection: Recent advances and perspectives,” Information Fusion, vol. 41, pp. 195 – 216, 2018.
-        
-        .. [2] : A. S. Britto, R. Sabourin, L. E. S. de Oliveira, Dynamic selection of classifiers - A comprehensive review, Pattern Recognition 47 (11) (2014) 3665–3680.
-        
-        .. [3] : A. H. R. Ko, R. Sabourin, u. S. Britto, Jr., From dynamic classifier selection to dynamic ensemble selection, Pattern Recognition 41 (2008) 1735–1748.
-        
-        .. [4] : K. Woods, W. P. Kegelmeyer, Jr., K. Bowyer, Combination of multiple classifiers using local accuracy estimates, IEEE Transactions on Pattern Analysis Machine Intelligence 19 (1997) 405–410.
-        
-        .. [5] : G. Giacinto, F. Roli, Dynamic classifier selection based on multiple classifier behaviour, Pattern Recognition 34 (2001) 1879–1881.
-        
-        .. [6] : L. Didaci, G. Giacinto, F. Roli, G. L. Marcialis, A study on the performances of dynamic classifier selection based on local accuracy estimation, Pattern Recognition 38 (11) (2005) 2188–2191.
-        
-        .. [7] : R. M. O. Cruz, R. Sabourin, G. D. C. Cavalcanti, T. I. Ren, META-DES: A dynamic ensemble selection framework using meta-learning, Pattern Recognition 48 (5) (2015) 1925–1935.
-        
-        .. [8] : Cruz, R.M., Sabourin, R. and Cavalcanti, G.D., 2015, July. META-DES. H: a dynamic ensemble selection technique using meta-learning and a dynamic weighting approach. In Neural Networks (IJCNN), 2015 International Joint Conference on (pp. 1-8)
-        
-        .. [9] : P. R. Cavalin, R. Sabourin, C. Y. Suen, Dynamic selection approaches for multiple classifier systems, Neural Computing and Applications 22 (3-4) (2013) 673–688.
-        
-        .. [10] : T.Woloszynski, M. Kurzynski, A probabilistic model of classifier competence for dynamic ensemble selection, Pattern Recognition 44 (2011) 2656–2668.
-        
-        .. [11] : T.Woloszynski, M. Kurzynski, A measure of competence based on randomized reference classifier for dynamic ensemble selection, in: International Conference on Pattern Recognition (ICPR), 2010, pp. 4194–4197.
-        
-        .. [12] : T. Woloszynski, M. Kurzynski, P. Podsiadlo, G. W. Stachowiak, A measure of competence based on random classification for dynamic ensemble selection, Information Fusion 13 (3) (2012) 207–213.
-        
-        .. [13] : Oliveira, D.V.R., Cavalcanti, G.D.C. and Sabourin, R., Online Pruning of Base Classifiers for Dynamic Ensemble Selection, Pattern Recognition, vol. 72, December 2017, pp 44-58.
-        
-        .. [14] : Cruz RM, Zakane HH, Sabourin R, Cavalcanti GD. Dynamic Ensemble Selection VS K-NN: why and when Dynamic Selection obtains higher classification performance?.
-        
-        .. [15] : R. M. O. Cruz, R. Sabourin, G. D. C. Cavalcanti, META-DES.Oracle: Meta-learning and feature selection for dynamic ensemble selection, Information Fusion 38 (2017) 84–103.Nov 30;38:84-103.
-        
-        .. [16] : R. G. F. Soares, A. Santana, A. M. P. Canuto, M. C. P. de Souto, Using accuracy and diversity to select classifiers to build ensembles, Proceedings of the International Joint Conference on Neural Networks (2006) 1310–1316.
-        
-        .. [17] : L. I. Kuncheva, Combining Pattern Classifiers: Methods and Algorithms, Wiley-Interscience, 2004.
-        
-        .. [18] : Shipp, Catherine A., and Ludmila I. Kuncheva. "Relationships between combination methods and measures of diversity in combining classifiers." Information fusion 3.2 (2002): 135-148.
-        
-        .. [19] : M. Sabourin, A. Mitiche, D. Thomas, G. Nagy, Classifier combination for handprinted digit recognition, International Conference on Document Analysis and Recognition (1993) 163–166.
-        
-        .. [20] : L. I. Kuncheva, A theoretical study on six classifier fusion strategies, IEEE Transactions on Pattern Analysis and Machine Intelligence 24 (2) (2002) 281–286.
-        
-        .. [21] : B. Antosik, M. Kurzynski, New measures of classifier competence – heuristics and application to the design of multiple classifier systems., in: Computer recognition systems 4., 2011, pp. 197–206.
-        
-        .. [22] : Smith, Michael R., Tony Martinez, and Christophe Giraud-Carrier. "An instance level analysis of data complexity." Machine learning 95.2 (2014), pp 225-256.
-        
-        .. [23] : P. C. Smits, Multiple classifier systems for supervised remote sensing image classification based on dynamic classifier selection, IEEE Transactions on Geoscience and Remote Sensing 40 (4) (2002) 801–813.
-        
-        .. [24] : García, S., Zhang, Z.L., Altalhi, A., Alshomrani, S. and Herrera, F., "Dynamic ensemble selection for multi-class imbalanced datasets." Information Sciences 445 (2018): 22-37.
-        
-        .. [25] : Wolpert, David H. "Stacked generalization." Neural networks 5, no. 2 (1992): 241-259.
-        
-        .. _scikit-learn: http://scikit-learn.org/stable/
-        
-        .. _numpy: http://www.numpy.org/
-        
-        .. _scipy: https://www.scipy.org/
-        
-        .. _documentation: https://deslib.readthedocs.io
-        
-        .. _FAISS: https://github.com/facebookresearch/faiss
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3
+License-File: LICENSE.txt
+Requires-Dist: scikit-learn>=1.0.2
+Requires-Dist: numpy>=1.17.0
+Requires-Dist: scipy>=1.4.0
+
+.. -*- mode: rst -*-
+
+.. _scikit-learn-contrib: https://github.com/scikit-learn-contrib
+
+|Docs|_ |CircleCI|_ |BSD|_ |PyPi|_ |PythonVersion|_ |Downloads|_ |Wheel|_ |Black|_
+
+.. |Docs| image:: https://readthedocs.org/projects/deslib/badge/?version=latest
+..    _Docs: http://deslib.readthedocs.io/en/latest/?badge=latest
+
+.. |CircleCI| image:: https://circleci.com/gh/scikit-learn-contrib/DESlib.svg?style=shield
+..    _CircleCI: https://circleci.com/gh/scikit-learn-contrib/DESlib
+
+.. |BSD| image:: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg
+..    _BSD: https://opensource.org/licenses/BSD-3-Clause
+
+.. |PyPi| image:: https://badge.fury.io/py/DESlib.svg
+..    _PyPi: https://pypi.org/project/DESlib/
+
+.. |PythonVersion| image:: https://img.shields.io/pypi/pyversions/deslib.svg
+..   _PythonVersion: https://pypi.org/project/DESlib/
+
+.. |Downloads| image:: https://img.shields.io/pypi/dm/deslib.svg
+..   _Downloads: https://pypistats.org/packages/deslib
+
+.. |Wheel| image:: https://img.shields.io/pypi/wheel/deslib.svg
+..   _Wheel: https://img.shields.io/pypi/wheel/deslib.svg
+
+.. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+.. _Black: :target: https://github.com/psf/black
+
+
+.. |PythonMinVersion| replace:: 3.7
+.. |NumPyMinVersion| replace:: 1.17.3
+.. |SciPyMinVersion| replace:: 1.5.0
+.. |ScikitLearnMinVersion| replace:: 1.0.2
+
+DESlib
+========
+
+DESlib is an easy-to-use ensemble learning library focused on the implementation of the state-of-the-art techniques for dynamic classifier and ensemble selection.
+The library is is based on scikit-learn_, using the same method signatures: **fit**, **predict**, **predict_proba** and **score**.
+All dynamic selection techniques were implemented according to the definitions from [1]_.
+
+Dynamic Selection:
+-------------------
+
+Dynamic Selection (DS) refers to techniques in which the base classifiers are selected
+dynamically at test time, according to each new sample to be classified. Only the most competent, or an ensemble of the most competent classifiers is selected to predict
+the label of a specific test sample. The rationale for these techniques is that not every classifier in
+the pool is an expert in classifying all unknown samples, but rather each base classifier is an expert in
+a different local region of the feature space.
+
+DS is one of the most promising MCS approaches (Multiple Classifier Systems) due to an increasing number of empirical studies
+reporting superior performance over static combination methods. Such techniques
+have achieved better classification performance especially when dealing with small-sized and imbalanced datasets.
+
+Installation:
+-------------
+
+The package can be installed using pip:
+
+Stable version:
+
+.. code-block:: bash
+
+    pip install deslib
+
+Latest version (under development):
+
+.. code-block:: bash
+
+    pip install git+https://github.com/scikit-learn-contrib/DESlib
+
+
+Dependencies:
+-------------
+
+The dependency requirements are:
+
+- Python (>= |PythonMinVersion|)
+- NumPy (>= |NumPyMinVersion|)
+- SciPy (>= |SciPyMinVersion|)
+- Scikit-learn (>= |ScikitLearnMinVersion|)
+
+These dependencies are automatically installed using the pip commands above.
+
+Examples:
+---------
+
+Here we show an example using the KNORA-E method with random forest as a pool of classifiers:
+
+.. code-block:: python
+
+    from deslib.des.knora_e import KNORAE
+
+    # Train a pool of 10 classifiers
+    pool_classifiers = RandomForestClassifier(n_estimators=10)
+    pool_classifiers.fit(X_train, y_train)
+
+    # Initialize the DES model
+    knorae = KNORAE(pool_classifiers)
+
+    # Preprocess the Dynamic Selection dataset (DSEL)
+    knorae.fit(X_dsel, y_dsel)
+
+    # Predict new examples:
+    knorae.predict(X_test)
+
+The library accepts any list of classifiers (compatible with scikit-learn) as input, including a list containing different classifier models (heterogeneous ensembles).
+More examples on how to use the API can be found in the documentation_ and in the Examples directory.
+
+Organization:
+-------------
+
+The library is divided into four modules:
+
+1. deslib.des: Implementation of DES techniques (Dynamic Ensemble Selection).
+2. deslib.dcs: Implementation of DCS techniques (Dynamic Classifier Selection).
+3. deslib.static: Implementation of baseline ensemble methods.
+4. deslib.util: A collection of aggregation functions and diversity measures for ensemble of classifiers.
+
+* DES techniques currently available are:
+    1. META-DES [7]_ [8]_ [15]_
+    2. K-Nearest-Oracle-Eliminate (KNORA-E) [3]_
+    3. K-Nearest-Oracle-Union (KNORA-U) [3]_
+    4. Dynamic Ensemble Selection-Performance(DES-P) [12]_
+    5. K-Nearest-Output Profiles (KNOP) [9]_
+    6. Randomized Reference Classifier (DES-RRC) [10]_
+    7. DES Kullback-Leibler Divergence (DES-KL) [12]_
+    8. DES-Exponential [21]_
+    9. DES-Logarithmic [11]_
+    10. DES-Minimum Difference [21]_
+    11. DES-Clustering [16]_
+    12. DES-KNN [16]_
+    13. DES Multiclass Imbalance (DES-MI) [24]_
+
+* DCS techniques currently available are:
+    1. Modified Classifier Rank (Rank) [19]_
+    2. Overall Local Accuracy (OLA) [4]_
+    3. Local Class Accuracy (LCA) [4]_
+    4. Modified Local Accuracy (MLA) [23]_
+    5. Multiple Classifier Behaviour (MCB) [5]_
+    6. A Priori Selection (A Priori) [6]_
+    7. A Posteriori Selection (A Posteriori) [6]_
+
+* Baseline methods:
+    1. Oracle [20]_
+    2. Single Best [2]_
+    3. Static Selection [2]_
+    4. Stacked Classifier [25]_
+
+Variations of each DES techniques are also provided by the library (e.g., different versions of the META-DES framework).
+
+The following techniques are also available for all methods:
+ * For DES techniques, the combination of the selected classifiers can be done as Dynamic Selection (majority voting), Dynamic Weighting  (weighted majority voting) or a Hybrid (selection + weighting).
+ * For all DS techniques, Dynamic Frienemy Pruning (DFP) [13]_ can be used.
+ * For all DS techniques, Instance Hardness (IH) can be used to classify easy samples with a KNN and hard samples using the DS technique. More details on IH and Dynamic Selection can be found in [14]_.
+
+As an optional requirement, the fast KNN implementation from FAISS_ can be used to speed-up the computation of the region of competence on GPU.
+
+Citation
+---------
+
+If you use DESLib in a scientific paper, please consider citing the following paper:
+
+Rafael M. O. Cruz, Luiz G. Hafemann, Robert Sabourin and George D. C. Cavalcanti `DESlib: A Dynamic ensemble selection library in Python. <https://arxiv.org/abs/1802.04967>`_ arXiv preprint arXiv:1802.04967 (2018).
+
+.. code-block:: text
+
+    @article{JMLR:v21:18-144,
+        author  = {Rafael M. O. Cruz and Luiz G. Hafemann and Robert Sabourin and George D. C. Cavalcanti},
+        title   = {DESlib: A Dynamic ensemble selection library in Python},
+        journal = {Journal of Machine Learning Research},
+        year    = {2020},
+        volume  = {21},
+        number  = {8},
+        pages   = {1-5},
+        url     = {http://jmlr.org/papers/v21/18-144.html}
+    }
+
+References:
+-----------
+
+.. [1] : R. M. O. Cruz, R. Sabourin, and G. D. Cavalcanti, “Dynamic classifier selection: Recent advances and perspectives,” Information Fusion, vol. 41, pp. 195 – 216, 2018.
+
+.. [2] : A. S. Britto, R. Sabourin, L. E. S. de Oliveira, Dynamic selection of classifiers - A comprehensive review, Pattern Recognition 47 (11) (2014) 3665–3680.
+
+.. [3] : A. H. R. Ko, R. Sabourin, u. S. Britto, Jr., From dynamic classifier selection to dynamic ensemble selection, Pattern Recognition 41 (2008) 1735–1748.
+
+.. [4] : K. Woods, W. P. Kegelmeyer, Jr., K. Bowyer, Combination of multiple classifiers using local accuracy estimates, IEEE Transactions on Pattern Analysis Machine Intelligence 19 (1997) 405–410.
+
+.. [5] : G. Giacinto, F. Roli, Dynamic classifier selection based on multiple classifier behaviour, Pattern Recognition 34 (2001) 1879–1881.
+
+.. [6] : L. Didaci, G. Giacinto, F. Roli, G. L. Marcialis, A study on the performances of dynamic classifier selection based on local accuracy estimation, Pattern Recognition 38 (11) (2005) 2188–2191.
+
+.. [7] : R. M. O. Cruz, R. Sabourin, G. D. C. Cavalcanti, T. I. Ren, META-DES: A dynamic ensemble selection framework using meta-learning, Pattern Recognition 48 (5) (2015) 1925–1935.
+
+.. [8] : Cruz, R.M., Sabourin, R. and Cavalcanti, G.D., 2015, July. META-DES. H: a dynamic ensemble selection technique using meta-learning and a dynamic weighting approach. In Neural Networks (IJCNN), 2015 International Joint Conference on (pp. 1-8)
+
+.. [9] : P. R. Cavalin, R. Sabourin, C. Y. Suen, Dynamic selection approaches for multiple classifier systems, Neural Computing and Applications 22 (3-4) (2013) 673–688.
+
+.. [10] : T.Woloszynski, M. Kurzynski, A probabilistic model of classifier competence for dynamic ensemble selection, Pattern Recognition 44 (2011) 2656–2668.
+
+.. [11] : T.Woloszynski, M. Kurzynski, A measure of competence based on randomized reference classifier for dynamic ensemble selection, in: International Conference on Pattern Recognition (ICPR), 2010, pp. 4194–4197.
+
+.. [12] : T. Woloszynski, M. Kurzynski, P. Podsiadlo, G. W. Stachowiak, A measure of competence based on random classification for dynamic ensemble selection, Information Fusion 13 (3) (2012) 207–213.
+
+.. [13] : Oliveira, D.V.R., Cavalcanti, G.D.C. and Sabourin, R., Online Pruning of Base Classifiers for Dynamic Ensemble Selection, Pattern Recognition, vol. 72, December 2017, pp 44-58.
+
+.. [14] : Cruz RM, Zakane HH, Sabourin R, Cavalcanti GD. Dynamic Ensemble Selection VS K-NN: why and when Dynamic Selection obtains higher classification performance?.
+
+.. [15] : R. M. O. Cruz, R. Sabourin, G. D. C. Cavalcanti, META-DES.Oracle: Meta-learning and feature selection for dynamic ensemble selection, Information Fusion 38 (2017) 84–103.Nov 30;38:84-103.
+
+.. [16] : R. G. F. Soares, A. Santana, A. M. P. Canuto, M. C. P. de Souto, Using accuracy and diversity to select classifiers to build ensembles, Proceedings of the International Joint Conference on Neural Networks (2006) 1310–1316.
+
+.. [17] : L. I. Kuncheva, Combining Pattern Classifiers: Methods and Algorithms, Wiley-Interscience, 2004.
+
+.. [18] : Shipp, Catherine A., and Ludmila I. Kuncheva. "Relationships between combination methods and measures of diversity in combining classifiers." Information fusion 3.2 (2002): 135-148.
+
+.. [19] : M. Sabourin, A. Mitiche, D. Thomas, G. Nagy, Classifier combination for handprinted digit recognition, International Conference on Document Analysis and Recognition (1993) 163–166.
+
+.. [20] : L. I. Kuncheva, A theoretical study on six classifier fusion strategies, IEEE Transactions on Pattern Analysis and Machine Intelligence 24 (2) (2002) 281–286.
+
+.. [21] : B. Antosik, M. Kurzynski, New measures of classifier competence – heuristics and application to the design of multiple classifier systems., in: Computer recognition systems 4., 2011, pp. 197–206.
+
+.. [22] : Smith, Michael R., Tony Martinez, and Christophe Giraud-Carrier. "An instance level analysis of data complexity." Machine learning 95.2 (2014), pp 225-256.
+
+.. [23] : P. C. Smits, Multiple classifier systems for supervised remote sensing image classification based on dynamic classifier selection, IEEE Transactions on Geoscience and Remote Sensing 40 (4) (2002) 801–813.
+
+.. [24] : García, S., Zhang, Z.L., Altalhi, A., Alshomrani, S. and Herrera, F., "Dynamic ensemble selection for multi-class imbalanced datasets." Information Sciences 445 (2018): 22-37.
+
+.. [25] : Wolpert, David H. "Stacked generalization." Neural networks 5, no. 2 (1992): 241-259.
+
+.. _scikit-learn: http://scikit-learn.org/stable/
+
+.. _numpy: http://www.numpy.org/
+
+.. _scipy: https://www.scipy.org/
+
+.. _documentation: https://deslib.readthedocs.io
+
+.. _FAISS: https://github.com/facebookresearch/faiss
```

### Comparing `DESlib-0.3.6/README.rst` & `DESlib-0.3.7/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,42 @@
-.. image:: https://readthedocs.org/projects/deslib/badge/?version=latest
-    :target: http://deslib.readthedocs.io/en/latest/?badge=latest
-    :alt: Documentation Status
-
-.. image:: https://circleci.com/gh/scikit-learn-contrib/DESlib.svg?style=shield
-    :target: https://circleci.com/gh/scikit-learn-contrib/DESlib
-
-.. image:: https://travis-ci.org/scikit-learn-contrib/DESlib.svg?branch=master
-    :target: https://travis-ci.org/scikit-learn-contrib/DESlib
-
-.. image:: https://codecov.io/gh/scikit-learn-contrib/DESlib/branch/master/graph/badge.svg
-    :target: https://codecov.io/gh/scikit-learn-contrib/DESlib
-    
-.. image:: https://api.codacy.com/project/badge/Grade/59500eecc5524c59b9eb2284b43ae3e6
-   :alt: Codacy Badge
-   :target: https://app.codacy.com/app/Menelau/DESlib?
+.. -*- mode: rst -*-
 
-.. image:: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg
-    :target: https://opensource.org/licenses/BSD-3-Clause
+.. _scikit-learn-contrib: https://github.com/scikit-learn-contrib
 
-.. image:: https://badges.gitter.im/DESlib/gitter.png
-    :target: https://gitter.im/deslib/Lobby
+|Docs|_ |CircleCI|_ |BSD|_ |PyPi|_ |PythonVersion|_ |Downloads|_ |Wheel|_ |Black|_
+
+.. |Docs| image:: https://readthedocs.org/projects/deslib/badge/?version=latest
+..    _Docs: http://deslib.readthedocs.io/en/latest/?badge=latest
+
+.. |CircleCI| image:: https://circleci.com/gh/scikit-learn-contrib/DESlib.svg?style=shield
+..    _CircleCI: https://circleci.com/gh/scikit-learn-contrib/DESlib
+
+.. |BSD| image:: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg
+..    _BSD: https://opensource.org/licenses/BSD-3-Clause
+
+.. |PyPi| image:: https://badge.fury.io/py/DESlib.svg
+..    _PyPi: https://pypi.org/project/DESlib/
+
+.. |PythonVersion| image:: https://img.shields.io/pypi/pyversions/deslib.svg
+..   _PythonVersion: https://pypi.org/project/DESlib/
+
+.. |Downloads| image:: https://img.shields.io/pypi/dm/deslib.svg
+..   _Downloads: https://pypistats.org/packages/deslib
+
+.. |Wheel| image:: https://img.shields.io/pypi/wheel/deslib.svg
+..   _Wheel: https://img.shields.io/pypi/wheel/deslib.svg
+
+.. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+.. _Black: :target: https://github.com/psf/black
+
+
+.. |PythonMinVersion| replace:: 3.7
+.. |NumPyMinVersion| replace:: 1.17.3
+.. |SciPyMinVersion| replace:: 1.5.0
+.. |ScikitLearnMinVersion| replace:: 1.0.2
 
 DESlib
 ========
 
 DESlib is an easy-to-use ensemble learning library focused on the implementation of the state-of-the-art techniques for dynamic classifier and ensemble selection.
 The library is is based on scikit-learn_, using the same method signatures: **fit**, **predict**, **predict_proba** and **score**.
 All dynamic selection techniques were implemented according to the definitions from [1]_.
@@ -58,19 +71,20 @@
 
     pip install git+https://github.com/scikit-learn-contrib/DESlib
 
 
 Dependencies:
 -------------
 
-DESlib is tested to work with Python 3.5, 3.6 and 3.7. The dependency requirements are:
+The dependency requirements are:
 
-* scipy(>=1.4.0)
-* numpy(>=1.17.0)
-* scikit-learn(>=0.20.0)
+- Python (>= |PythonMinVersion|)
+- NumPy (>= |NumPyMinVersion|)
+- SciPy (>= |SciPyMinVersion|)
+- Scikit-learn (>= |ScikitLearnMinVersion|)
 
 These dependencies are automatically installed using the pip commands above.
 
 Examples:
 ---------
 
 Here we show an example using the KNORA-E method with random forest as a pool of classifiers:
@@ -138,15 +152,15 @@
 Variations of each DES techniques are also provided by the library (e.g., different versions of the META-DES framework).
 
 The following techniques are also available for all methods:
  * For DES techniques, the combination of the selected classifiers can be done as Dynamic Selection (majority voting), Dynamic Weighting  (weighted majority voting) or a Hybrid (selection + weighting).
  * For all DS techniques, Dynamic Frienemy Pruning (DFP) [13]_ can be used.
  * For all DS techniques, Instance Hardness (IH) can be used to classify easy samples with a KNN and hard samples using the DS technique. More details on IH and Dynamic Selection can be found in [14]_.
 
-As an optional requirement, the fast KNN implementation from FAISS_ can be used to speed-up the computation of the region of competence.
+As an optional requirement, the fast KNN implementation from FAISS_ can be used to speed-up the computation of the region of competence on GPU.
 
 Citation
 ---------
 
 If you use DESLib in a scientific paper, please consider citing the following paper:
 
 Rafael M. O. Cruz, Luiz G. Hafemann, Robert Sabourin and George D. C. Cavalcanti `DESlib: A Dynamic ensemble selection library in Python. <https://arxiv.org/abs/1802.04967>`_ arXiv preprint arXiv:1802.04967 (2018).
```

### Comparing `DESlib-0.3.6/deslib/__init__.py` & `DESlib-0.3.7/deslib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,8 +19,8 @@
     A collection of aggregation functions and diversity measures for ensemble
     of classifiers.
 """
 
 # list of all modules available in the library
 __all__ = ['des', 'dcs', 'static', 'util', 'tests']
 
-__version__ = '0.3.6'
+__version__ = '0.3.7'
```

### Comparing `DESlib-0.3.6/deslib/base.py` & `DESlib-0.3.7/deslib/base.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/dcs/a_posteriori.py` & `DESlib-0.3.7/deslib/dcs/a_posteriori.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/dcs/a_priori.py` & `DESlib-0.3.7/deslib/dcs/a_priori.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/dcs/base.py` & `DESlib-0.3.7/deslib/dcs/base.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/dcs/lca.py` & `DESlib-0.3.7/deslib/dcs/lca.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/dcs/mcb.py` & `DESlib-0.3.7/deslib/dcs/mcb.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/dcs/mla.py` & `DESlib-0.3.7/deslib/dcs/mla.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/dcs/ola.py` & `DESlib-0.3.7/deslib/dcs/ola.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/dcs/rank.py` & `DESlib-0.3.7/deslib/dcs/rank.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/des/__init__.py` & `DESlib-0.3.7/deslib/des/__init__.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/des/base.py` & `DESlib-0.3.7/deslib/des/base.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/des/des_clustering.py` & `DESlib-0.3.7/deslib/des/des_clustering.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/des/des_knn.py` & `DESlib-0.3.7/deslib/des/des_knn.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/des/des_mi.py` & `DESlib-0.3.7/deslib/des/des_mi.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/des/des_p.py` & `DESlib-0.3.7/deslib/des/des_p.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/des/knop.py` & `DESlib-0.3.7/deslib/des/knop.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/des/knora_e.py` & `DESlib-0.3.7/deslib/des/knora_e.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/des/knora_u.py` & `DESlib-0.3.7/deslib/des/knora_u.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/des/meta_des.py` & `DESlib-0.3.7/deslib/des/meta_des.py`

 * *Files 1% similar despite different names*

```diff
@@ -545,16 +545,16 @@
 
             raise ValueError(
                 "The meta-classifier should output probability estimates")
 
         if self.Kp is not None:
             if not isinstance(self.Kp, int):
                 raise TypeError("parameter Kp should be an integer.")
-            if self.Kp <= 1:
-                raise ValueError("parameter Kp must be higher than 1."
+            if self.Kp <= 0:
+                raise ValueError("parameter Kp must be equal orhigher than 1."
                                  "input Kp is {} .".format(self.Kp))
         else:
             raise ValueError("Parameter Kp is 'None'.")
 
         super()._validate_parameters()
 
     def _check_Kp_samples(self):
```

### Comparing `DESlib-0.3.6/deslib/des/probabilistic/base.py` & `DESlib-0.3.7/deslib/des/probabilistic/base.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/des/probabilistic/deskl.py` & `DESlib-0.3.7/deslib/des/probabilistic/deskl.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/des/probabilistic/exponential.py` & `DESlib-0.3.7/deslib/des/probabilistic/exponential.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/des/probabilistic/logarithmic.py` & `DESlib-0.3.7/deslib/des/probabilistic/logarithmic.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/des/probabilistic/minimum_difference.py` & `DESlib-0.3.7/deslib/des/probabilistic/minimum_difference.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/des/probabilistic/rrc.py` & `DESlib-0.3.7/deslib/des/probabilistic/rrc.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/static/base.py` & `DESlib-0.3.7/deslib/static/base.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/static/oracle.py` & `DESlib-0.3.7/deslib/static/oracle.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/static/single_best.py` & `DESlib-0.3.7/deslib/static/single_best.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/static/stacked.py` & `DESlib-0.3.7/deslib/static/stacked.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/static/static_selection.py` & `DESlib-0.3.7/deslib/static/static_selection.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/tests/conftest.py` & `DESlib-0.3.7/deslib/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/tests/dcs/test_a_posteriori.py` & `DESlib-0.3.7/deslib/tests/dcs/test_a_posteriori.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/tests/dcs/test_a_priori.py` & `DESlib-0.3.7/deslib/tests/dcs/test_a_priori.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/tests/dcs/test_base.py` & `DESlib-0.3.7/deslib/tests/dcs/test_base.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/tests/dcs/test_lca.py` & `DESlib-0.3.7/deslib/tests/dcs/test_lca.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/tests/dcs/test_mcb.py` & `DESlib-0.3.7/deslib/tests/dcs/test_mcb.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/tests/dcs/test_mla.py` & `DESlib-0.3.7/deslib/tests/dcs/test_mla.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/tests/dcs/test_ola.py` & `DESlib-0.3.7/deslib/tests/dcs/test_ola.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/tests/dcs/test_rank.py` & `DESlib-0.3.7/deslib/tests/dcs/test_rank.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/tests/des/test_base.py` & `DESlib-0.3.7/deslib/tests/des/test_base.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/tests/des/test_des_clustering.py` & `DESlib-0.3.7/deslib/tests/des/test_des_clustering.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/tests/des/test_des_knn.py` & `DESlib-0.3.7/deslib/tests/des/test_des_knn.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/tests/des/test_des_mi.py` & `DESlib-0.3.7/deslib/tests/des/test_des_mi.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/tests/des/test_desp.py` & `DESlib-0.3.7/deslib/tests/des/test_desp.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/tests/des/test_knop.py` & `DESlib-0.3.7/deslib/tests/des/test_knop.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/tests/des/test_knorae.py` & `DESlib-0.3.7/deslib/tests/des/test_knorae.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/tests/des/test_knorau.py` & `DESlib-0.3.7/deslib/tests/des/test_knorau.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/tests/des/test_meta_des.py` & `DESlib-0.3.7/deslib/tests/des/test_meta_des.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from sklearn.utils.estimator_checks import check_estimator
 from sklearn.utils.validation import check_is_fitted
 
 from deslib.des.meta_des import METADES
 
 
 def test_check_estimator():
-    check_estimator(METADES())
+    check_estimator(METADES(Kp=1))
 
 
 # ---------------------- Testing Hyper-parameters -----------------------
 @pytest.mark.parametrize('model,', [SVC(), Perceptron()])
 def test_meta_classifier_not_predict_proba(create_pool_classifiers, model):
     X = np.random.rand(10, 2)
     y = np.ones(10)
```

### Comparing `DESlib-0.3.6/deslib/tests/des/test_probabilistic.py` & `DESlib-0.3.7/deslib/tests/des/test_probabilistic.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/tests/static/test_oracle.py` & `DESlib-0.3.7/deslib/tests/static/test_oracle.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/tests/static/test_single_best.py` & `DESlib-0.3.7/deslib/tests/static/test_single_best.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/tests/static/test_stacked.py` & `DESlib-0.3.7/deslib/tests/static/test_stacked.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/tests/static/test_static_selection.py` & `DESlib-0.3.7/deslib/tests/static/test_static_selection.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/tests/test_base.py` & `DESlib-0.3.7/deslib/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/tests/test_des_integration.py` & `DESlib-0.3.7/deslib/tests/test_des_integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,15 +202,15 @@
 
 def test_apriori():
     pool_classifiers, X_dsel, y_dsel, X_test, y_test = setup_classifiers()
     rng = np.random.RandomState(123456)
 
     apriori = APriori(pool_classifiers, random_state=rng)
     apriori.fit(X_dsel, y_dsel)
-    assert np.isclose(apriori.score(X_test, y_test), 0.973404255319149)
+    assert np.isclose(apriori.score(X_test, y_test), 0.9680851063829787)
 
 
 @pytest.mark.parametrize('knn_methods', knn_methods)
 def test_rank(knn_methods):
     pool_classifiers, X_dsel, y_dsel, X_test, y_test = setup_classifiers()
 
     rank = Rank(pool_classifiers, knn_classifier=knn_methods)
@@ -220,15 +220,15 @@
 
 def test_aposteriori():
     pool_classifiers, X_dsel, y_dsel, X_test, y_test = setup_classifiers()
     rng = np.random.RandomState(123456)
 
     a_posteriori = APosteriori(pool_classifiers, random_state=rng)
     a_posteriori.fit(X_dsel, y_dsel)
-    assert np.isclose(a_posteriori.score(X_test, y_test), 0.973404255319149)
+    assert np.isclose(a_posteriori.score(X_test, y_test), 0.9787234042553191)
 
 
 @pytest.mark.parametrize('knn_methods, voting',
                          itertools.product(knn_methods, voting))
 def test_meta(knn_methods, voting):
     pool_classifiers, X_dsel, y_dsel, X_test, y_test = setup_classifiers()
 
@@ -329,90 +329,87 @@
     pool_classifiers, X_dsel, y_dsel, X_test, y_test = setup_classifiers()
 
     kne = KNORAE(pool_classifiers, knn_classifier=knn_methods, voting='soft')
     kne.fit(X_dsel, y_dsel)
     probas = kne.predict_proba(X_test)
     expected = np.load(
         'deslib/tests/expected_values/kne_proba_integration.npy')
-    assert np.allclose(probas, expected)
+    assert np.allclose(probas, expected, atol=0.01)
 
 
 @pytest.mark.parametrize('knn_methods', knn_methods)
 def test_desp_proba(knn_methods):
     pool_classifiers, X_dsel, y_dsel, X_test, y_test = setup_classifiers()
     desp = DESP(pool_classifiers, knn_classifier=knn_methods, voting='soft')
     desp.fit(X_dsel, y_dsel)
     probas = desp.predict_proba(X_test)
     expected = np.load(
         'deslib/tests/expected_values/desp_proba_integration.npy')
-    assert np.allclose(probas, expected)
+    assert np.allclose(probas, expected, atol=0.01)
 
 
 @pytest.mark.parametrize('knn_methods', knn_methods)
 def test_ola_proba(knn_methods):
     pool_classifiers, X_dsel, y_dsel, X_test, y_test = setup_classifiers()
 
     ola = OLA(pool_classifiers, knn_classifier=knn_methods)
     ola.fit(X_dsel, y_dsel)
     probas = ola.predict_proba(X_test)
     expected = np.load(
         'deslib/tests/expected_values/ola_proba_integration.npy')
-    assert np.allclose(probas, expected)
+    assert np.allclose(probas, expected, atol=0.01)
 
 
 @pytest.mark.parametrize('knn_methods', knn_methods)
 def test_mcb_proba(knn_methods):
     pool_classifiers, X_dsel, y_dsel, X_test, y_test = setup_classifiers()
     rng = np.random.RandomState(123456)
 
     mcb = MCB(pool_classifiers, random_state=rng, knn_classifier=knn_methods)
 
     mcb.fit(X_dsel, y_dsel)
-    probas = mcb.predict_proba(X_test)
-    expected = np.load(
-        'deslib/tests/expected_values/mcb_proba_integration.npy')
+    probas = mcb.predict_proba(X_test).argmax(axis=1)
+    expected = mcb.predict(X_test)
     assert np.allclose(probas, expected)
 
 
 @pytest.mark.parametrize('knn_methods', knn_methods)
 def test_desknn_proba(knn_methods):
     pool_classifiers, X_dsel, y_dsel, X_test, y_test = setup_classifiers()
 
     desknn = DESKNN(pool_classifiers, knn_classifier=knn_methods,
                     voting='soft')
     desknn.fit(X_dsel, y_dsel)
-    probas = desknn.predict_proba(X_test)
-    expected = np.load(
-        'deslib/tests/expected_values/desknn_proba_integration.npy')
+    probas = desknn.predict_proba(X_test).argmax(axis=1)
+    expected = desknn.predict(X_test)
     assert np.allclose(probas, expected)
 
 
 def test_des_clustering_proba():
     pool_classifiers, X_dsel, y_dsel, X_test, y_test = setup_classifiers()
     rng = np.random.RandomState(123456)
     cluster = KMeans(n_clusters=5, random_state=rng)
     des_clustering = DESClustering(pool_classifiers, clustering=cluster,
                                    voting='soft')
     des_clustering.fit(X_dsel, y_dsel)
-    probas = des_clustering.predict_proba(X_test)
-    expected = np.load(
-        'deslib/tests/expected_values/des_clustering_proba_integration.npy')
+    probas = des_clustering.predict_proba(X_test).argmax(axis=1)
+    expected = des_clustering.predict(X_test)
     assert np.allclose(probas, expected)
 
 
 @pytest.mark.parametrize('knn_methods', knn_methods)
 def test_knop_proba(knn_methods):
     pool_classifiers, X_dsel, y_dsel, X_test, y_test = setup_classifiers()
 
     knop = KNOP(pool_classifiers, knn_classifier=knn_methods, voting='soft')
     knop.fit(X_dsel, y_dsel)
     probas = knop.predict_proba(X_test)
     expected = np.load(
         'deslib/tests/expected_values/knop_proba_integration.npy')
-    assert np.allclose(probas, expected)
+    assert np.allclose(probas, expected, atol=0.01)
 
 
 def test_meta_no_pool_of_classifiers():
     rng = np.random.RandomState(123456)
     data = load_breast_cancer()
     X = data.data
     y = data.target
@@ -508,30 +505,30 @@
     pool = BaggingClassifier(LogisticRegression(),
                              max_features=0.5,
                              random_state=rng).fit(X_train, y_train)
 
     static = StaticSelection(pool)
     static.fit(X_dsel, y_dsel)
     assert np.isclose(static.score(X_test, y_test),
-                      0.9840425531914894)
+                      0.9787234042553191)
 
 
 def test_static_selection_subspaces_proba():
     rng = np.random.RandomState(123456)
     X_dsel, X_test, X_train, y_dsel, y_test, y_train = load_dataset(
         None, rng)
     pool = BaggingClassifier(LogisticRegression(),
                              max_features=0.5,
                              random_state=rng).fit(X_train, y_train)
 
     static = StaticSelection(pool)
     static.fit(X_dsel, y_dsel)
-    y_pred = static.predict_proba(X_test).argmax(axis=1)
-    assert np.isclose(accuracy_score(y_pred, y_test),
-                      0.9840425531914894)
+    y_pred_proba = static.predict_proba(X_test).argmax(axis=1)
+    y_pred = static.predict(X_test)
+    assert np.isclose(y_pred, y_pred_proba).all()
 
 
 def test_stacked_subspaces():
     rng = np.random.RandomState(123456)
     X_dsel, X_test, X_train, y_dsel, y_test, y_train = load_dataset(
         None, rng)
     pool = BaggingClassifier(LogisticRegression(),
```

### Comparing `DESlib-0.3.6/deslib/tests/test_des_integration_multiclass.py` & `DESlib-0.3.7/deslib/tests/test_des_integration_multiclass.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/tests/test_integration_DFP_IH.py` & `DESlib-0.3.7/deslib/tests/test_integration_DFP_IH.py`

 * *Files 7% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 
 def test_knorau():
     pool_classifiers, X_dsel, y_dsel, X_test, y_test = setup_classifiers()
 
     knorau = KNORAU(pool_classifiers, DFP=True, with_IH=True, IH_rate=0.1)
     knorau.fit(X_dsel, y_dsel)
-    assert np.isclose(knorau.score(X_test, y_test), 0.896969696969697)
+    assert np.isclose(knorau.score(X_test, y_test), 0.9)
 
 
 def test_desp():
     pool_classifiers, X_dsel, y_dsel, X_test, y_test = setup_classifiers()
 
     desp = DESP(pool_classifiers, DFP=True, with_IH=True, IH_rate=0.1)
     desp.fit(X_dsel, y_dsel)
@@ -71,18 +71,8 @@
 def test_mcb():
     pool_classifiers, X_dsel, y_dsel, X_test, y_test = setup_classifiers()
     rng = np.random.RandomState(123456)
 
     mcb = MCB(pool_classifiers, random_state=rng, DFP=True, with_IH=True,
               IH_rate=0.1)
     mcb.fit(X_dsel, y_dsel)
-    assert np.isclose(mcb.score(X_test, y_test), 0.9030303030303031)
-
-
-def test_aposteriori():
-    pool_classifiers, X_dsel, y_dsel, X_test, y_test = setup_classifiers()
-    rng = np.random.RandomState(123456)
-
-    a_posteriori = APosteriori(pool_classifiers, random_state=rng, DFP=True,
-                               with_IH=True, IH_rate=0.1)
-    a_posteriori.fit(X_dsel, y_dsel)
-    assert np.isclose(a_posteriori.score(X_test, y_test), 0.8333333333333334)
+    assert np.isclose(mcb.score(X_test, y_test), 0.8878787878787879)
```

### Comparing `DESlib-0.3.6/deslib/tests/test_integration_dfp.py` & `DESlib-0.3.7/deslib/tests/test_integration_dfp.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/tests/test_metric.py` & `DESlib-0.3.7/deslib/tests/test_metric.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/tests/util/test_aggregation.py` & `DESlib-0.3.7/deslib/tests/util/test_aggregation.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/tests/util/test_datasets.py` & `DESlib-0.3.7/deslib/tests/util/test_datasets.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/tests/util/test_diversity.py` & `DESlib-0.3.7/deslib/tests/util/test_diversity.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/tests/util/test_diversity_batch.py` & `DESlib-0.3.7/deslib/tests/util/test_diversity_batch.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/tests/util/test_faiss.py` & `DESlib-0.3.7/deslib/tests/util/test_faiss.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/tests/util/test_fire.py` & `DESlib-0.3.7/deslib/tests/util/test_fire.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/tests/util/test_instance_hardness.py` & `DESlib-0.3.7/deslib/tests/util/test_instance_hardness.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/tests/util/test_knne.py` & `DESlib-0.3.7/deslib/tests/util/test_knne.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/tests/util/test_prob_functions.py` & `DESlib-0.3.7/deslib/tests/util/test_prob_functions.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/util/__init__.py` & `DESlib-0.3.7/deslib/util/__init__.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/util/aggregation.py` & `DESlib-0.3.7/deslib/util/aggregation.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/util/datasets.py` & `DESlib-0.3.7/deslib/util/datasets.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/util/dfp.py` & `DESlib-0.3.7/deslib/util/dfp.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/util/diversity.py` & `DESlib-0.3.7/deslib/util/diversity.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/util/diversity_batch.py` & `DESlib-0.3.7/deslib/util/diversity_batch.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/util/faiss_knn_wrapper.py` & `DESlib-0.3.7/deslib/util/faiss_knn_wrapper.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/util/instance_hardness.py` & `DESlib-0.3.7/deslib/util/instance_hardness.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/util/knne.py` & `DESlib-0.3.7/deslib/util/knne.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/deslib/util/prob_functions.py` & `DESlib-0.3.7/deslib/util/prob_functions.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/docs/Makefile` & `DESlib-0.3.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/docs/api.rst` & `DESlib-0.3.7/docs/api.rst`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/docs/conf.py` & `DESlib-0.3.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/docs/index.rst` & `DESlib-0.3.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/docs/make.bat` & `DESlib-0.3.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/docs/news/v0.1.rst` & `DESlib-0.3.7/docs/news/v0.1.rst`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/docs/news/v0.2.rst` & `DESlib-0.3.7/docs/news/v0.2.rst`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/docs/news/v0.3.5.rst` & `DESlib-0.3.7/docs/news/v0.3.5.rst`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/docs/news/v0.3.rst` & `DESlib-0.3.7/docs/news/v0.3.rst`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/docs/user_guide/development.rst` & `DESlib-0.3.7/docs/user_guide/development.rst`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/docs/user_guide/installation.rst` & `DESlib-0.3.7/docs/user_guide/installation.rst`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/docs/user_guide/known_issues.rst` & `DESlib-0.3.7/docs/user_guide/known_issues.rst`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/docs/user_guide/packaging.rst` & `DESlib-0.3.7/docs/user_guide/packaging.rst`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/docs/user_guide/tutorial.rst` & `DESlib-0.3.7/docs/user_guide/tutorial.rst`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/examples/example_calibrating_classifiers.py` & `DESlib-0.3.7/examples/example_calibrating_classifiers.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/examples/example_heterogeneous.py` & `DESlib-0.3.7/examples/example_heterogeneous.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/examples/plot_comparing_dynamic_static.py` & `DESlib-0.3.7/examples/plot_comparing_dynamic_static.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/examples/plot_example_DFP.py` & `DESlib-0.3.7/examples/plot_example_DFP.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/examples/plot_example_P2.py` & `DESlib-0.3.7/examples/plot_example_P2.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/examples/plot_influence_k_value.py` & `DESlib-0.3.7/examples/plot_influence_k_value.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/examples/plot_random_forest.py` & `DESlib-0.3.7/examples/plot_random_forest.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/examples/plot_using_instance_hardness.py` & `DESlib-0.3.7/examples/plot_using_instance_hardness.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/examples/plot_xor_example.py` & `DESlib-0.3.7/examples/plot_xor_example.py`

 * *Files identical despite different names*

### Comparing `DESlib-0.3.6/examples/simple_example.py` & `DESlib-0.3.7/examples/simple_example.py`

 * *Files identical despite different names*

