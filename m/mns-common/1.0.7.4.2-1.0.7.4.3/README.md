# Comparing `tmp/mns_common-1.0.7.4.2.tar.gz` & `tmp/mns_common-1.0.7.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mns_common-1.0.7.4.2.tar", last modified: Tue Apr  2 12:27:39 2024, max compression
+gzip compressed data, was "mns_common-1.0.7.4.3.tar", last modified: Fri Apr 12 04:35:56 2024, max compression
```

## Comparing `mns_common-1.0.7.4.2.tar` & `mns_common-1.0.7.4.3.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 12:27:39.522348 mns_common-1.0.7.4.2/
--rw-rw-rw-   0        0        0       61 2024-04-02 12:27:39.522348 mns_common-1.0.7.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     1354 2023-12-14 15:25:31.000000 mns_common-1.0.7.4.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 12:27:39.483197 mns_common-1.0.7.4.2/mns_common/
--rw-rw-rw-   0        0        0      163 2024-01-10 10:52:31.000000 mns_common-1.0.7.4.2/mns_common/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:27:39.485192 mns_common-1.0.7.4.2/mns_common/api/
--rw-rw-rw-   0        0        0      163 2023-12-15 04:00:46.000000 mns_common-1.0.7.4.2/mns_common/api/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:27:39.488184 mns_common-1.0.7.4.2/mns_common/api/akshare/
--rw-rw-rw-   0        0        0      165 2023-12-15 04:25:30.000000 mns_common-1.0.7.4.2/mns_common/api/akshare/__init__.py
--rw-rw-rw-   0        0        0     5057 2023-12-22 09:50:37.000000 mns_common-1.0.7.4.2/mns_common/api/akshare/k_line_api.py
--rw-rw-rw-   0        0        0     5999 2024-01-05 08:16:46.000000 mns_common-1.0.7.4.2/mns_common/api/akshare/stock_bid_ask_api.py
--rw-rw-rw-   0        0        0     2245 2023-12-16 12:13:22.000000 mns_common-1.0.7.4.2/mns_common/api/akshare/stock_dt_pool.py
--rw-rw-rw-   0        0        0     2038 2023-12-16 13:25:10.000000 mns_common-1.0.7.4.2/mns_common/api/akshare/stock_zb_pool.py
--rw-rw-rw-   0        0        0     1929 2023-12-16 12:13:22.000000 mns_common-1.0.7.4.2/mns_common/api/akshare/stock_zt_pool_api.py
--rw-rw-rw-   0        0        0     4108 2023-12-16 12:13:22.000000 mns_common-1.0.7.4.2/mns_common/api/akshare/yjyg_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:27:39.491185 mns_common-1.0.7.4.2/mns_common/api/em/
--rw-rw-rw-   0        0        0      163 2023-12-15 04:08:44.000000 mns_common-1.0.7.4.2/mns_common/api/em/__init__.py
--rw-rw-rw-   0        0        0     8251 2023-12-18 12:33:18.000000 mns_common-1.0.7.4.2/mns_common/api/em/east_money_stock_api.py
--rw-rw-rw-   0        0        0     5504 2023-12-22 09:50:37.000000 mns_common-1.0.7.4.2/mns_common/api/em/east_money_stock_gdfx_free_top_10_api.py
--rw-rw-rw-   0        0        0    12619 2023-12-18 12:33:18.000000 mns_common-1.0.7.4.2/mns_common/api/em/east_money_stock_v2_api.py
--rw-rw-rw-   0        0        0     8285 2023-12-22 09:50:37.000000 mns_common-1.0.7.4.2/mns_common/api/em/em_concept_index_api.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:27:39.491185 mns_common-1.0.7.4.2/mns_common/api/kpl/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.7.4.2/mns_common/api/kpl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:27:39.492176 mns_common-1.0.7.4.2/mns_common/api/kpl/common/
--rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.7.4.2/mns_common/api/kpl/common/__init__.py
--rw-rw-rw-   0        0        0     6447 2024-01-16 11:07:48.000000 mns_common-1.0.7.4.2/mns_common/api/kpl/common/kpl_common_api.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:27:39.493173 mns_common-1.0.7.4.2/mns_common/api/kpl/concept/
--rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.7.4.2/mns_common/api/kpl/concept/__init__.py
--rw-rw-rw-   0        0        0      607 2023-12-16 12:13:22.000000 mns_common-1.0.7.4.2/mns_common/api/kpl/concept/kpl_concept_api.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:27:39.494170 mns_common-1.0.7.4.2/mns_common/api/kpl/constant/
--rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.0.7.4.2/mns_common/api/kpl/constant/__init__.py
--rw-rw-rw-   0        0        0      669 2023-12-22 09:50:37.000000 mns_common-1.0.7.4.2/mns_common/api/kpl/constant/kpl_constant.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:27:39.495168 mns_common-1.0.7.4.2/mns_common/api/kpl/industry/
--rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.7.4.2/mns_common/api/kpl/industry/__init__.py
--rw-rw-rw-   0        0        0      565 2023-12-16 12:13:22.000000 mns_common-1.0.7.4.2/mns_common/api/kpl/industry/kpl_industry_api.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:27:39.496165 mns_common-1.0.7.4.2/mns_common/api/kpl/selection/
--rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.0.7.4.2/mns_common/api/kpl/selection/__init__.py
--rw-rw-rw-   0        0        0     1777 2024-01-11 08:08:46.000000 mns_common-1.0.7.4.2/mns_common/api/kpl/selection/kpl_selection_plate_api.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:27:39.498160 mns_common-1.0.7.4.2/mns_common/api/kpl/symbol/
--rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.7.4.2/mns_common/api/kpl/symbol/__init__.py
--rw-rw-rw-   0        0        0     4792 2024-03-22 08:55:03.000000 mns_common-1.0.7.4.2/mns_common/api/kpl/symbol/kpl_real_time_quotes_api.py
--rw-rw-rw-   0        0        0     1625 2024-03-22 08:56:47.000000 mns_common-1.0.7.4.2/mns_common/api/kpl/symbol/kpl_symbol_common_field_constant.py
--rw-rw-rw-   0        0        0     4208 2023-12-16 12:13:22.000000 mns_common-1.0.7.4.2/mns_common/api/kpl/symbol/symbol_his_quotes_api.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:27:39.499157 mns_common-1.0.7.4.2/mns_common/api/msg/
--rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.0.7.4.2/mns_common/api/msg/__init__.py
--rw-rw-rw-   0        0        0     1421 2024-02-03 04:57:25.000000 mns_common-1.0.7.4.2/mns_common/api/msg/push_msg_api.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:27:39.501177 mns_common-1.0.7.4.2/mns_common/api/ths/
--rw-rw-rw-   0        0        0      163 2023-12-15 03:59:01.000000 mns_common-1.0.7.4.2/mns_common/api/ths/__init__.py
--rw-rw-rw-   0        0        0     3614 2023-12-22 09:50:37.000000 mns_common-1.0.7.4.2/mns_common/api/ths/ths_big_deal_api.py
--rw-rw-rw-   0        0        0    39926 2024-01-12 12:47:02.000000 mns_common-1.0.7.4.2/mns_common/api/ths/ths_stock_api.py
--rw-rw-rw-   0        0        0     6784 2024-01-12 12:47:02.000000 mns_common-1.0.7.4.2/mns_common/api/ths/ths_stock_zt_pool_api.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:27:39.501965 mns_common-1.0.7.4.2/mns_common/component/
--rw-rw-rw-   0        0        0      163 2023-12-15 04:38:42.000000 mns_common-1.0.7.4.2/mns_common/component/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:27:39.503955 mns_common-1.0.7.4.2/mns_common/component/classify/
--rw-rw-rw-   0        0        0      163 2024-01-09 08:35:24.000000 mns_common-1.0.7.4.2/mns_common/component/classify/__init__.py
--rw-rw-rw-   0        0        0      522 2024-01-09 09:22:06.000000 mns_common-1.0.7.4.2/mns_common/component/classify/classify_constant.py
--rw-rw-rw-   0        0        0     3880 2024-01-09 08:35:24.000000 mns_common-1.0.7.4.2/mns_common/component/classify/symbol_classify_api.py
--rw-rw-rw-   0        0        0     4790 2024-01-13 08:29:24.000000 mns_common-1.0.7.4.2/mns_common/component/common_service_fun_api.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:27:39.504952 mns_common-1.0.7.4.2/mns_common/component/company/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.7.4.2/mns_common/component/company/__init__.py
--rw-rw-rw-   0        0        0     6987 2023-12-17 11:37:16.000000 mns_common-1.0.7.4.2/mns_common/component/company/company_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:27:39.505949 mns_common-1.0.7.4.2/mns_common/component/concept/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.7.4.2/mns_common/component/concept/__init__.py
--rw-rw-rw-   0        0        0     1096 2024-04-02 12:18:51.000000 mns_common-1.0.7.4.2/mns_common/component/concept/kpl_concept_common_service_api.py
--rw-rw-rw-   0        0        0     8532 2024-04-02 12:11:42.000000 mns_common-1.0.7.4.2/mns_common/component/concept/ths_concept_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:27:39.506946 mns_common-1.0.7.4.2/mns_common/component/data/
--rw-rw-rw-   0        0        0      163 2023-12-17 11:33:58.000000 mns_common-1.0.7.4.2/mns_common/component/data/__init__.py
--rw-rw-rw-   0        0        0     4757 2023-12-17 11:40:38.000000 mns_common-1.0.7.4.2/mns_common/component/data/data_init_api.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:27:39.507944 mns_common-1.0.7.4.2/mns_common/component/industry/
--rw-rw-rw-   0        0        0      163 2024-01-13 08:34:39.000000 mns_common-1.0.7.4.2/mns_common/component/industry/__init__.py
--rw-rw-rw-   0        0        0     3252 2024-01-13 08:57:34.000000 mns_common-1.0.7.4.2/mns_common/component/industry/ths_industry_index_api.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:27:39.507944 mns_common-1.0.7.4.2/mns_common/component/k_line/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.7.4.2/mns_common/component/k_line/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:27:39.508942 mns_common-1.0.7.4.2/mns_common/component/k_line/clean/
--rw-rw-rw-   0        0        0      163 2024-01-09 09:22:06.000000 mns_common-1.0.7.4.2/mns_common/component/k_line/clean/__init__.py
--rw-rw-rw-   0        0        0      248 2024-01-09 09:22:06.000000 mns_common-1.0.7.4.2/mns_common/component/k_line/clean/k_line_param.py
--rw-rw-rw-   0        0        0    12593 2024-01-09 10:28:47.000000 mns_common-1.0.7.4.2/mns_common/component/k_line/clean/sh_small_normal_zt_k_line_check_api.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:27:39.509939 mns_common-1.0.7.4.2/mns_common/component/k_line/common/
--rw-rw-rw-   0        0        0      163 2023-12-22 09:41:45.000000 mns_common-1.0.7.4.2/mns_common/component/k_line/common/__init__.py
--rw-rw-rw-   0        0        0     4449 2023-12-29 04:25:17.000000 mns_common-1.0.7.4.2/mns_common/component/k_line/common/k_line_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:27:39.511864 mns_common-1.0.7.4.2/mns_common/component/k_line/patterns/
--rw-rw-rw-   0        0        0      163 2023-12-22 07:50:10.000000 mns_common-1.0.7.4.2/mns_common/component/k_line/patterns/__init__.py
--rw-rw-rw-   0        0        0     1809 2023-12-22 08:25:35.000000 mns_common-1.0.7.4.2/mns_common/component/k_line/patterns/k_line_patterns_service_api.py
--rw-rw-rw-   0        0        0      509 2023-12-22 09:49:23.000000 mns_common-1.0.7.4.2/mns_common/component/k_line/patterns/pattern_Enum.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:27:39.512845 mns_common-1.0.7.4.2/mns_common/component/real_time/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.7.4.2/mns_common/component/real_time/__init__.py
--rw-rw-rw-   0        0        0     1378 2023-12-16 12:13:22.000000 mns_common-1.0.7.4.2/mns_common/component/real_time/real_time_common_service_api.py
--rw-rw-rw-   0        0        0     1034 2024-01-05 08:29:27.000000 mns_common-1.0.7.4.2/mns_common/component/real_time/real_time_symbol_bid_service_api.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:27:39.513843 mns_common-1.0.7.4.2/mns_common/component/trade_date/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.7.4.2/mns_common/component/trade_date/__init__.py
--rw-rw-rw-   0        0        0     2776 2023-12-28 13:35:59.000000 mns_common-1.0.7.4.2/mns_common/component/trade_date/trade_date_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:27:39.514840 mns_common-1.0.7.4.2/mns_common/component/zt/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.7.4.2/mns_common/component/zt/__init__.py
--rw-rw-rw-   0        0        0     7794 2024-01-13 09:14:41.000000 mns_common-1.0.7.4.2/mns_common/component/zt/zt_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:27:39.517359 mns_common-1.0.7.4.2/mns_common/constant/
--rw-rw-rw-   0        0        0      163 2023-12-17 08:25:43.000000 mns_common-1.0.7.4.2/mns_common/constant/__init__.py
--rw-rw-rw-   0        0        0     1186 2024-01-26 03:46:17.000000 mns_common-1.0.7.4.2/mns_common/constant/db_name_constant.py
--rw-rw-rw-   0        0        0     4507 2024-01-25 14:21:07.000000 mns_common-1.0.7.4.2/mns_common/constant/kpl_selection_no_choose_constant.py
--rw-rw-rw-   0        0        0    12240 2024-03-11 15:08:57.000000 mns_common-1.0.7.4.2/mns_common/constant/ths_concept_no_choose_constant.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:27:39.518356 mns_common-1.0.7.4.2/mns_common/db/
--rw-rw-rw-   0        0        0    10824 2023-12-27 08:37:01.000000 mns_common-1.0.7.4.2/mns_common/db/MongodbUtil.py
--rw-rw-rw-   0        0        0      163 2023-12-15 04:08:44.000000 mns_common-1.0.7.4.2/mns_common/db/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:27:39.521357 mns_common-1.0.7.4.2/mns_common/utils/
--rw-rw-rw-   0        0        0      163 2023-12-15 04:00:46.000000 mns_common-1.0.7.4.2/mns_common/utils/__init__.py
--rw-rw-rw-   0        0        0      352 2023-12-15 04:16:28.000000 mns_common-1.0.7.4.2/mns_common/utils/async_fun.py
--rw-rw-rw-   0        0        0     1316 2023-12-22 08:25:35.000000 mns_common-1.0.7.4.2/mns_common/utils/data_frame_util.py
--rw-rw-rw-   0        0        0     7379 2023-12-21 03:38:02.000000 mns_common-1.0.7.4.2/mns_common/utils/date_handle_util.py
--rw-rw-rw-   0        0        0      451 2023-12-15 04:16:28.000000 mns_common-1.0.7.4.2/mns_common/utils/ip_util.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:27:39.521357 mns_common-1.0.7.4.2/mns_common.egg-info/
--rw-rw-rw-   0        0        0       61 2024-04-02 12:27:39.000000 mns_common-1.0.7.4.2/mns_common.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3516 2024-04-02 12:27:39.000000 mns_common-1.0.7.4.2/mns_common.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 12:27:39.000000 mns_common-1.0.7.4.2/mns_common.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-02 12:27:39.000000 mns_common-1.0.7.4.2/mns_common.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-02 12:27:39.522348 mns_common-1.0.7.4.2/setup.cfg
--rw-rw-rw-   0        0        0      466 2024-04-02 12:09:35.000000 mns_common-1.0.7.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 04:35:56.561658 mns_common-1.0.7.4.3/
+-rw-rw-rw-   0        0        0       61 2024-04-12 04:35:56.560660 mns_common-1.0.7.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1354 2023-12-14 15:25:31.000000 mns_common-1.0.7.4.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-12 04:35:56.521793 mns_common-1.0.7.4.3/mns_common/
+-rw-rw-rw-   0        0        0      163 2024-01-10 10:52:31.000000 mns_common-1.0.7.4.3/mns_common/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 04:35:56.524786 mns_common-1.0.7.4.3/mns_common/api/
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:00:46.000000 mns_common-1.0.7.4.3/mns_common/api/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 04:35:56.527777 mns_common-1.0.7.4.3/mns_common/api/akshare/
+-rw-rw-rw-   0        0        0      165 2023-12-15 04:25:30.000000 mns_common-1.0.7.4.3/mns_common/api/akshare/__init__.py
+-rw-rw-rw-   0        0        0     5057 2023-12-22 09:50:37.000000 mns_common-1.0.7.4.3/mns_common/api/akshare/k_line_api.py
+-rw-rw-rw-   0        0        0     5999 2024-01-05 08:16:46.000000 mns_common-1.0.7.4.3/mns_common/api/akshare/stock_bid_ask_api.py
+-rw-rw-rw-   0        0        0     2245 2023-12-16 12:13:22.000000 mns_common-1.0.7.4.3/mns_common/api/akshare/stock_dt_pool.py
+-rw-rw-rw-   0        0        0     2038 2023-12-16 13:25:10.000000 mns_common-1.0.7.4.3/mns_common/api/akshare/stock_zb_pool.py
+-rw-rw-rw-   0        0        0     1929 2023-12-16 12:13:22.000000 mns_common-1.0.7.4.3/mns_common/api/akshare/stock_zt_pool_api.py
+-rw-rw-rw-   0        0        0     4108 2023-12-16 12:13:22.000000 mns_common-1.0.7.4.3/mns_common/api/akshare/yjyg_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-04-12 04:35:56.530769 mns_common-1.0.7.4.3/mns_common/api/em/
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:08:44.000000 mns_common-1.0.7.4.3/mns_common/api/em/__init__.py
+-rw-rw-rw-   0        0        0     8251 2023-12-18 12:33:18.000000 mns_common-1.0.7.4.3/mns_common/api/em/east_money_stock_api.py
+-rw-rw-rw-   0        0        0     5504 2023-12-22 09:50:37.000000 mns_common-1.0.7.4.3/mns_common/api/em/east_money_stock_gdfx_free_top_10_api.py
+-rw-rw-rw-   0        0        0    12619 2023-12-18 12:33:18.000000 mns_common-1.0.7.4.3/mns_common/api/em/east_money_stock_v2_api.py
+-rw-rw-rw-   0        0        0     8285 2023-12-22 09:50:37.000000 mns_common-1.0.7.4.3/mns_common/api/em/em_concept_index_api.py
+drwxrwxrwx   0        0        0        0 2024-04-12 04:35:56.530769 mns_common-1.0.7.4.3/mns_common/api/kpl/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.7.4.3/mns_common/api/kpl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 04:35:56.531767 mns_common-1.0.7.4.3/mns_common/api/kpl/common/
+-rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.7.4.3/mns_common/api/kpl/common/__init__.py
+-rw-rw-rw-   0        0        0     6447 2024-01-16 11:07:48.000000 mns_common-1.0.7.4.3/mns_common/api/kpl/common/kpl_common_api.py
+drwxrwxrwx   0        0        0        0 2024-04-12 04:35:56.532764 mns_common-1.0.7.4.3/mns_common/api/kpl/concept/
+-rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.7.4.3/mns_common/api/kpl/concept/__init__.py
+-rw-rw-rw-   0        0        0      607 2023-12-16 12:13:22.000000 mns_common-1.0.7.4.3/mns_common/api/kpl/concept/kpl_concept_api.py
+drwxrwxrwx   0        0        0        0 2024-04-12 04:35:56.533764 mns_common-1.0.7.4.3/mns_common/api/kpl/constant/
+-rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.0.7.4.3/mns_common/api/kpl/constant/__init__.py
+-rw-rw-rw-   0        0        0      669 2023-12-22 09:50:37.000000 mns_common-1.0.7.4.3/mns_common/api/kpl/constant/kpl_constant.py
+drwxrwxrwx   0        0        0        0 2024-04-12 04:35:56.534730 mns_common-1.0.7.4.3/mns_common/api/kpl/industry/
+-rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.7.4.3/mns_common/api/kpl/industry/__init__.py
+-rw-rw-rw-   0        0        0      565 2023-12-16 12:13:22.000000 mns_common-1.0.7.4.3/mns_common/api/kpl/industry/kpl_industry_api.py
+drwxrwxrwx   0        0        0        0 2024-04-12 04:35:56.535727 mns_common-1.0.7.4.3/mns_common/api/kpl/selection/
+-rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.0.7.4.3/mns_common/api/kpl/selection/__init__.py
+-rw-rw-rw-   0        0        0     1777 2024-01-11 08:08:46.000000 mns_common-1.0.7.4.3/mns_common/api/kpl/selection/kpl_selection_plate_api.py
+drwxrwxrwx   0        0        0        0 2024-04-12 04:35:56.537722 mns_common-1.0.7.4.3/mns_common/api/kpl/symbol/
+-rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.7.4.3/mns_common/api/kpl/symbol/__init__.py
+-rw-rw-rw-   0        0        0     4792 2024-03-22 08:55:03.000000 mns_common-1.0.7.4.3/mns_common/api/kpl/symbol/kpl_real_time_quotes_api.py
+-rw-rw-rw-   0        0        0     1625 2024-03-22 08:56:47.000000 mns_common-1.0.7.4.3/mns_common/api/kpl/symbol/kpl_symbol_common_field_constant.py
+-rw-rw-rw-   0        0        0     4208 2023-12-16 12:13:22.000000 mns_common-1.0.7.4.3/mns_common/api/kpl/symbol/symbol_his_quotes_api.py
+drwxrwxrwx   0        0        0        0 2024-04-12 04:35:56.538719 mns_common-1.0.7.4.3/mns_common/api/msg/
+-rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.0.7.4.3/mns_common/api/msg/__init__.py
+-rw-rw-rw-   0        0        0     1421 2024-02-03 04:57:25.000000 mns_common-1.0.7.4.3/mns_common/api/msg/push_msg_api.py
+drwxrwxrwx   0        0        0        0 2024-04-12 04:35:56.540743 mns_common-1.0.7.4.3/mns_common/api/ths/
+-rw-rw-rw-   0        0        0      163 2023-12-15 03:59:01.000000 mns_common-1.0.7.4.3/mns_common/api/ths/__init__.py
+-rw-rw-rw-   0        0        0     3614 2023-12-22 09:50:37.000000 mns_common-1.0.7.4.3/mns_common/api/ths/ths_big_deal_api.py
+-rw-rw-rw-   0        0        0    39935 2024-04-12 00:08:48.000000 mns_common-1.0.7.4.3/mns_common/api/ths/ths_stock_api.py
+-rw-rw-rw-   0        0        0     6784 2024-01-12 12:47:02.000000 mns_common-1.0.7.4.3/mns_common/api/ths/ths_stock_zt_pool_api.py
+drwxrwxrwx   0        0        0        0 2024-04-12 04:35:56.541742 mns_common-1.0.7.4.3/mns_common/component/
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:38:42.000000 mns_common-1.0.7.4.3/mns_common/component/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 04:35:56.542745 mns_common-1.0.7.4.3/mns_common/component/classify/
+-rw-rw-rw-   0        0        0      163 2024-01-09 08:35:24.000000 mns_common-1.0.7.4.3/mns_common/component/classify/__init__.py
+-rw-rw-rw-   0        0        0      522 2024-01-09 09:22:06.000000 mns_common-1.0.7.4.3/mns_common/component/classify/classify_constant.py
+-rw-rw-rw-   0        0        0     3880 2024-01-09 08:35:24.000000 mns_common-1.0.7.4.3/mns_common/component/classify/symbol_classify_api.py
+-rw-rw-rw-   0        0        0     4790 2024-01-13 08:29:24.000000 mns_common-1.0.7.4.3/mns_common/component/common_service_fun_api.py
+drwxrwxrwx   0        0        0        0 2024-04-12 04:35:56.543735 mns_common-1.0.7.4.3/mns_common/component/company/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.7.4.3/mns_common/component/company/__init__.py
+-rw-rw-rw-   0        0        0     6987 2023-12-17 11:37:16.000000 mns_common-1.0.7.4.3/mns_common/component/company/company_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-04-12 04:35:56.545737 mns_common-1.0.7.4.3/mns_common/component/concept/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.7.4.3/mns_common/component/concept/__init__.py
+-rw-rw-rw-   0        0        0     1096 2024-04-02 12:18:51.000000 mns_common-1.0.7.4.3/mns_common/component/concept/kpl_concept_common_service_api.py
+-rw-rw-rw-   0        0        0     9929 2024-04-12 04:35:23.000000 mns_common-1.0.7.4.3/mns_common/component/concept/ths_concept_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-04-12 04:35:56.545737 mns_common-1.0.7.4.3/mns_common/component/data/
+-rw-rw-rw-   0        0        0      163 2023-12-17 11:33:58.000000 mns_common-1.0.7.4.3/mns_common/component/data/__init__.py
+-rw-rw-rw-   0        0        0     4757 2023-12-17 11:40:38.000000 mns_common-1.0.7.4.3/mns_common/component/data/data_init_api.py
+drwxrwxrwx   0        0        0        0 2024-04-12 04:35:56.546729 mns_common-1.0.7.4.3/mns_common/component/industry/
+-rw-rw-rw-   0        0        0      163 2024-01-13 08:34:39.000000 mns_common-1.0.7.4.3/mns_common/component/industry/__init__.py
+-rw-rw-rw-   0        0        0     3252 2024-01-13 08:57:34.000000 mns_common-1.0.7.4.3/mns_common/component/industry/ths_industry_index_api.py
+drwxrwxrwx   0        0        0        0 2024-04-12 04:35:56.547697 mns_common-1.0.7.4.3/mns_common/component/k_line/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.7.4.3/mns_common/component/k_line/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 04:35:56.548722 mns_common-1.0.7.4.3/mns_common/component/k_line/clean/
+-rw-rw-rw-   0        0        0      163 2024-01-09 09:22:06.000000 mns_common-1.0.7.4.3/mns_common/component/k_line/clean/__init__.py
+-rw-rw-rw-   0        0        0      248 2024-01-09 09:22:06.000000 mns_common-1.0.7.4.3/mns_common/component/k_line/clean/k_line_param.py
+-rw-rw-rw-   0        0        0    12593 2024-01-09 10:28:47.000000 mns_common-1.0.7.4.3/mns_common/component/k_line/clean/sh_small_normal_zt_k_line_check_api.py
+drwxrwxrwx   0        0        0        0 2024-04-12 04:35:56.549719 mns_common-1.0.7.4.3/mns_common/component/k_line/common/
+-rw-rw-rw-   0        0        0      163 2023-12-22 09:41:45.000000 mns_common-1.0.7.4.3/mns_common/component/k_line/common/__init__.py
+-rw-rw-rw-   0        0        0     4449 2023-12-29 04:25:17.000000 mns_common-1.0.7.4.3/mns_common/component/k_line/common/k_line_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-04-12 04:35:56.551685 mns_common-1.0.7.4.3/mns_common/component/k_line/patterns/
+-rw-rw-rw-   0        0        0      163 2023-12-22 07:50:10.000000 mns_common-1.0.7.4.3/mns_common/component/k_line/patterns/__init__.py
+-rw-rw-rw-   0        0        0     1809 2023-12-22 08:25:35.000000 mns_common-1.0.7.4.3/mns_common/component/k_line/patterns/k_line_patterns_service_api.py
+-rw-rw-rw-   0        0        0      509 2023-12-22 09:49:23.000000 mns_common-1.0.7.4.3/mns_common/component/k_line/patterns/pattern_Enum.py
+drwxrwxrwx   0        0        0        0 2024-04-12 04:35:56.552682 mns_common-1.0.7.4.3/mns_common/component/real_time/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.7.4.3/mns_common/component/real_time/__init__.py
+-rw-rw-rw-   0        0        0     1378 2023-12-16 12:13:22.000000 mns_common-1.0.7.4.3/mns_common/component/real_time/real_time_common_service_api.py
+-rw-rw-rw-   0        0        0     1034 2024-01-05 08:29:27.000000 mns_common-1.0.7.4.3/mns_common/component/real_time/real_time_symbol_bid_service_api.py
+drwxrwxrwx   0        0        0        0 2024-04-12 04:35:56.553679 mns_common-1.0.7.4.3/mns_common/component/trade_date/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.7.4.3/mns_common/component/trade_date/__init__.py
+-rw-rw-rw-   0        0        0     2776 2023-12-28 13:35:59.000000 mns_common-1.0.7.4.3/mns_common/component/trade_date/trade_date_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-04-12 04:35:56.554676 mns_common-1.0.7.4.3/mns_common/component/zt/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.7.4.3/mns_common/component/zt/__init__.py
+-rw-rw-rw-   0        0        0     7794 2024-01-13 09:14:41.000000 mns_common-1.0.7.4.3/mns_common/component/zt/zt_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-04-12 04:35:56.556672 mns_common-1.0.7.4.3/mns_common/constant/
+-rw-rw-rw-   0        0        0      163 2023-12-17 08:25:43.000000 mns_common-1.0.7.4.3/mns_common/constant/__init__.py
+-rw-rw-rw-   0        0        0     1186 2024-01-26 03:46:17.000000 mns_common-1.0.7.4.3/mns_common/constant/db_name_constant.py
+-rw-rw-rw-   0        0        0     4507 2024-01-25 14:21:07.000000 mns_common-1.0.7.4.3/mns_common/constant/kpl_selection_no_choose_constant.py
+-rw-rw-rw-   0        0        0    12240 2024-03-11 15:08:57.000000 mns_common-1.0.7.4.3/mns_common/constant/ths_concept_no_choose_constant.py
+drwxrwxrwx   0        0        0        0 2024-04-12 04:35:56.557669 mns_common-1.0.7.4.3/mns_common/db/
+-rw-rw-rw-   0        0        0    10824 2023-12-27 08:37:01.000000 mns_common-1.0.7.4.3/mns_common/db/MongodbUtil.py
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:08:44.000000 mns_common-1.0.7.4.3/mns_common/db/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 04:35:56.559663 mns_common-1.0.7.4.3/mns_common/utils/
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:00:46.000000 mns_common-1.0.7.4.3/mns_common/utils/__init__.py
+-rw-rw-rw-   0        0        0      352 2023-12-15 04:16:28.000000 mns_common-1.0.7.4.3/mns_common/utils/async_fun.py
+-rw-rw-rw-   0        0        0     1316 2023-12-22 08:25:35.000000 mns_common-1.0.7.4.3/mns_common/utils/data_frame_util.py
+-rw-rw-rw-   0        0        0     7379 2023-12-21 03:38:02.000000 mns_common-1.0.7.4.3/mns_common/utils/date_handle_util.py
+-rw-rw-rw-   0        0        0      451 2023-12-15 04:16:28.000000 mns_common-1.0.7.4.3/mns_common/utils/ip_util.py
+drwxrwxrwx   0        0        0        0 2024-04-12 04:35:56.560660 mns_common-1.0.7.4.3/mns_common.egg-info/
+-rw-rw-rw-   0        0        0       61 2024-04-12 04:35:56.000000 mns_common-1.0.7.4.3/mns_common.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3516 2024-04-12 04:35:56.000000 mns_common-1.0.7.4.3/mns_common.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 04:35:56.000000 mns_common-1.0.7.4.3/mns_common.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-12 04:35:56.000000 mns_common-1.0.7.4.3/mns_common.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-12 04:35:56.561658 mns_common-1.0.7.4.3/setup.cfg
+-rw-rw-rw-   0        0        0      466 2024-04-12 04:35:23.000000 mns_common-1.0.7.4.3/setup.py
```

### Comparing `mns_common-1.0.7.4.2/README.md` & `mns_common-1.0.7.4.3/README.md`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.4.2/mns_common/api/akshare/k_line_api.py` & `mns_common-1.0.7.4.3/mns_common/api/akshare/k_line_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.4.2/mns_common/api/akshare/stock_bid_ask_api.py` & `mns_common-1.0.7.4.3/mns_common/api/akshare/stock_bid_ask_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.4.2/mns_common/api/akshare/stock_dt_pool.py` & `mns_common-1.0.7.4.3/mns_common/api/akshare/stock_dt_pool.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.4.2/mns_common/api/akshare/stock_zb_pool.py` & `mns_common-1.0.7.4.3/mns_common/api/akshare/stock_zb_pool.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.4.2/mns_common/api/akshare/stock_zt_pool_api.py` & `mns_common-1.0.7.4.3/mns_common/api/akshare/stock_zt_pool_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.4.2/mns_common/api/akshare/yjyg_sync_api.py` & `mns_common-1.0.7.4.3/mns_common/api/akshare/yjyg_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.4.2/mns_common/api/em/east_money_stock_api.py` & `mns_common-1.0.7.4.3/mns_common/api/em/east_money_stock_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.4.2/mns_common/api/em/east_money_stock_gdfx_free_top_10_api.py` & `mns_common-1.0.7.4.3/mns_common/api/em/east_money_stock_gdfx_free_top_10_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.4.2/mns_common/api/em/east_money_stock_v2_api.py` & `mns_common-1.0.7.4.3/mns_common/api/em/east_money_stock_v2_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.4.2/mns_common/api/em/em_concept_index_api.py` & `mns_common-1.0.7.4.3/mns_common/api/em/em_concept_index_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.4.2/mns_common/api/kpl/common/kpl_common_api.py` & `mns_common-1.0.7.4.3/mns_common/api/kpl/common/kpl_common_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.4.2/mns_common/api/kpl/concept/kpl_concept_api.py` & `mns_common-1.0.7.4.3/mns_common/api/kpl/concept/kpl_concept_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.4.2/mns_common/api/kpl/constant/kpl_constant.py` & `mns_common-1.0.7.4.3/mns_common/api/kpl/constant/kpl_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.4.2/mns_common/api/kpl/industry/kpl_industry_api.py` & `mns_common-1.0.7.4.3/mns_common/api/kpl/industry/kpl_industry_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.4.2/mns_common/api/kpl/selection/kpl_selection_plate_api.py` & `mns_common-1.0.7.4.3/mns_common/api/kpl/selection/kpl_selection_plate_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.4.2/mns_common/api/kpl/symbol/kpl_real_time_quotes_api.py` & `mns_common-1.0.7.4.3/mns_common/api/kpl/symbol/kpl_real_time_quotes_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.4.2/mns_common/api/kpl/symbol/kpl_symbol_common_field_constant.py` & `mns_common-1.0.7.4.3/mns_common/api/kpl/symbol/kpl_symbol_common_field_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.4.2/mns_common/api/kpl/symbol/symbol_his_quotes_api.py` & `mns_common-1.0.7.4.3/mns_common/api/kpl/symbol/symbol_his_quotes_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.4.2/mns_common/api/msg/push_msg_api.py` & `mns_common-1.0.7.4.3/mns_common/api/msg/push_msg_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.4.2/mns_common/api/ths/ths_big_deal_api.py` & `mns_common-1.0.7.4.3/mns_common/api/ths/ths_big_deal_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.4.2/mns_common/api/ths/ths_stock_api.py` & `mns_common-1.0.7.4.3/mns_common/api/ths/ths_stock_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -834,15 +834,15 @@
                           "detail",
                           "market_code",
                           "concept_code"]
     return concept_df
 
 
 if __name__ == '__main__':
-    df = ths_stock_concept('885598')
+    df = get_symbol_add_new_concept('600128')
     print(df)
     # while True:
     #     concept_test()
     # company_info = get_concept_name('881121')
     # print(company_info)
     # new_concept_symbol_list = ths_stock_concept('881121')
     # print(new_concept_symbol_list)
```

### Comparing `mns_common-1.0.7.4.2/mns_common/api/ths/ths_stock_zt_pool_api.py` & `mns_common-1.0.7.4.3/mns_common/api/ths/ths_stock_zt_pool_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.4.2/mns_common/component/classify/classify_constant.py` & `mns_common-1.0.7.4.3/mns_common/component/classify/classify_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.4.2/mns_common/component/classify/symbol_classify_api.py` & `mns_common-1.0.7.4.3/mns_common/component/classify/symbol_classify_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.4.2/mns_common/component/common_service_fun_api.py` & `mns_common-1.0.7.4.3/mns_common/component/common_service_fun_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.4.2/mns_common/component/company/company_common_service_api.py` & `mns_common-1.0.7.4.3/mns_common/component/company/company_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.4.2/mns_common/component/concept/kpl_concept_common_service_api.py` & `mns_common-1.0.7.4.3/mns_common/component/concept/kpl_concept_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.4.2/mns_common/component/concept/ths_concept_common_service_api.py` & `mns_common-1.0.7.4.3/mns_common/component/concept/ths_concept_common_service_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,74 +13,103 @@
 import pandas as pd
 from io import StringIO
 from functools import lru_cache
 
 
 # 同花顺概念操作类
 
-# 获取单个股票所有概念数据
+
+# 获取所有同花顺概念代码
 @lru_cache(maxsize=None)
-def get_all_ths_concept(symbol):
-    effective_ths_concept_list = get_choose_effective_ths_concept()
-    effective_ths_concept_ids = list(effective_ths_concept_list['symbol'])
-    query = {'symbol': symbol, '$and': [{'concept_code': {'$in': effective_ths_concept_ids}},
-                                        {'concept_name': {"$ne": None}}]}
-    return mongodb_util.find_query_data('ths_stock_concept_detail', query)
+def get_all_ths_concept():
+    query = {}
+    ths_concept_list = mongodb_util.find_query_data('ths_concept_list', query)
+    return ths_concept_list
 
 
 # 获取有效同花顺概念代码
 @lru_cache(maxsize=None)
-def get_choose_effective_ths_concept():
+def get_all_ths_effective_concept():
     query = {}
     ths_concept_list = mongodb_util.find_query_data('ths_concept_list', query)
     # 选择有效的概念
     ths_concept_list_effective = ths_concept_list.loc[ths_concept_list['valid']]
     return ths_concept_list_effective
 
 
+# 获取单个股票所有有效概念数据
+@lru_cache(maxsize=None)
+def get_one_symbol_effective_ths_concept(symbol):
+    ths_concept_list = get_all_ths_concept()
+    # 选择有效的概念
+    ths_concept_list_effective = ths_concept_list.loc[ths_concept_list['valid']]
+    effective_ths_concept_ids = list(ths_concept_list_effective['symbol'])
+    query = {'symbol': symbol, '$and': [{'concept_code': {'$in': effective_ths_concept_ids}},
+                                        {'concept_name': {"$ne": None}}]}
+    return mongodb_util.find_query_data('ths_stock_concept_detail', query)
+
+
+# 获取单个股票所有有效概念数据
+@lru_cache(maxsize=None)
+def get_one_symbol_ths_concept(symbol):
+    ths_concept_list = get_all_ths_concept()
+    # 选择有效的概念
+    ths_concept_list_effective = ths_concept_list.loc[ths_concept_list['valid']]
+    effective_ths_concept_ids = list(ths_concept_list_effective['symbol'])
+    query = {'symbol': symbol, '$and': [{'concept_code': {'$in': effective_ths_concept_ids}},
+                                        {'concept_name': {"$ne": None}}]}
+    return mongodb_util.find_query_data('ths_stock_concept_detail', query)
+
+
 # 设置同花顺最新概念
 def set_ths_concept(symbol, df):
-    ths_stock_concept_detail = get_all_ths_concept(symbol)
+    ths_stock_concept_detail = get_one_symbol_ths_concept(symbol)
     df['ths_concept_name'] = "未有"
     df['ths_concept_code'] = 0
     df['ths_concept_sync_day'] = "1989-07-29"
 
     df['ths_concept_list_info'] = "-"
 
     if ths_stock_concept_detail.shape[0] == 0:
         return df
 
     ths_stock_concept_detail = ths_stock_concept_detail.sort_values(by=['concept_code'], ascending=False)
-    ths_stock_concept_detail_last_one = ths_stock_concept_detail.iloc[0:1]
-    if ths_stock_concept_detail_last_one['concept_name'] is None:
-        df['ths_concept_name'] = "未有"
-    else:
-        df['ths_concept_name'] = list(ths_stock_concept_detail_last_one['concept_name'])[0]
-
-    if ths_stock_concept_detail_last_one['concept_code'] is None:
-        df['concept_code'] = 0
-    else:
-        df['ths_concept_code'] = list(ths_stock_concept_detail_last_one['concept_code'])[0]
-
-    df['ths_concept_sync_day'] = list(ths_stock_concept_detail_last_one['str_day'])[0]
-
     ths_stock_concept_detail.dropna(subset=['concept_name'], axis=0, inplace=True)
     ths_stock_concept_detail.dropna(subset=['concept_code'], axis=0, inplace=True)
 
     if data_frame_util.is_not_empty(ths_stock_concept_detail):
         ths_stock_concept_detail = ths_stock_concept_detail[[
             'concept_code',
             'concept_name',
             'str_day',
             'str_now_time',
             'concept_create_day']]
         # 去除空格
         ths_stock_concept_detail['concept_name'] = ths_stock_concept_detail['concept_name'].str.replace(' ', '')
         df.loc[:, 'ths_concept_list_info'] = ths_stock_concept_detail.to_string(index=False)
 
+    ths_effective_concept_list = get_all_ths_effective_concept()
+    ths_effective_concept_code_list = list(ths_effective_concept_list['symbol'])
+
+    ths_stock_concept_detail_effective = ths_stock_concept_detail.loc[
+        ths_stock_concept_detail['concept_code'].isin(ths_effective_concept_code_list)]
+
+    # 最新概念设置
+    ths_stock_concept_detail_last_one = ths_stock_concept_detail_effective.iloc[0:1]
+    if ths_stock_concept_detail_last_one['concept_name'] is None:
+        df['ths_concept_name'] = "未有"
+    else:
+        df['ths_concept_name'] = list(ths_stock_concept_detail_last_one['concept_name'])[0]
+    if ths_stock_concept_detail_last_one['concept_code'] is None:
+        df['concept_code'] = 0
+    else:
+        df['ths_concept_code'] = list(ths_stock_concept_detail_last_one['concept_code'])[0]
+
+    df['ths_concept_sync_day'] = list(ths_stock_concept_detail_last_one['str_day'])[0]
+
     return df
 
 
 def set_last_ths_concept(symbol, stock_em_zt_pool_df_data, str_day):
     query = {'concept_name': {'$ne': ""}, 'symbol': symbol, "str_day": {"$lte": str_day}}
     ths_stock_concept_detail = mongodb_util.descend_query(query, 'ths_stock_concept_detail', 'concept_code', 1)
     stock_em_zt_pool_df_data.loc[stock_em_zt_pool_df_data['symbol'] == symbol, ['ths_concept_name']] = "未有"
@@ -179,27 +208,29 @@
         'plate_name_list',
         'most_relative_name',
         'index_class'
     ]]
 
 
 def clear_ths_concept_cache():
-    get_choose_effective_ths_concept.cache_clear()
     get_all_ths_concept.cache_clear()
-    get_concept_by_code.cache_clear()
+    get_all_ths_effective_concept.cache_clear()
+    get_one_symbol_effective_ths_concept.cache_clear()
+    get_one_symbol_ths_concept.cache_clear()
 
 
 def clear_effective_ths_concept_cache():
-    get_choose_effective_ths_concept.cache_clear()
+    get_all_ths_effective_concept.cache_clear()
+    get_one_symbol_effective_ths_concept.cache_clear()
 
 
 def get_choose_effective_ths_concept_no_cache():
     query = {'valid': True}
     ths_concept_list_effective = mongodb_util.find_query_data('ths_concept_list', query)
     return ths_concept_list_effective
 
 
 if __name__ == '__main__':
-    df = get_all_ths_concept('300085')
+    df_ths = get_all_ths_concept('300085')
     while True:
         get_choose_effective_ths_concept_no_cache()
         print(1)
```

### Comparing `mns_common-1.0.7.4.2/mns_common/component/data/data_init_api.py` & `mns_common-1.0.7.4.3/mns_common/component/data/data_init_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.4.2/mns_common/component/industry/ths_industry_index_api.py` & `mns_common-1.0.7.4.3/mns_common/component/industry/ths_industry_index_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.4.2/mns_common/component/k_line/clean/sh_small_normal_zt_k_line_check_api.py` & `mns_common-1.0.7.4.3/mns_common/component/k_line/clean/sh_small_normal_zt_k_line_check_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.4.2/mns_common/component/k_line/common/k_line_common_service_api.py` & `mns_common-1.0.7.4.3/mns_common/component/k_line/common/k_line_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.4.2/mns_common/component/k_line/patterns/k_line_patterns_service_api.py` & `mns_common-1.0.7.4.3/mns_common/component/k_line/patterns/k_line_patterns_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.4.2/mns_common/component/real_time/real_time_common_service_api.py` & `mns_common-1.0.7.4.3/mns_common/component/real_time/real_time_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.4.2/mns_common/component/real_time/real_time_symbol_bid_service_api.py` & `mns_common-1.0.7.4.3/mns_common/component/real_time/real_time_symbol_bid_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.4.2/mns_common/component/trade_date/trade_date_common_service_api.py` & `mns_common-1.0.7.4.3/mns_common/component/trade_date/trade_date_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.4.2/mns_common/component/zt/zt_common_service_api.py` & `mns_common-1.0.7.4.3/mns_common/component/zt/zt_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.4.2/mns_common/constant/db_name_constant.py` & `mns_common-1.0.7.4.3/mns_common/constant/db_name_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.4.2/mns_common/constant/kpl_selection_no_choose_constant.py` & `mns_common-1.0.7.4.3/mns_common/constant/kpl_selection_no_choose_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.4.2/mns_common/constant/ths_concept_no_choose_constant.py` & `mns_common-1.0.7.4.3/mns_common/constant/ths_concept_no_choose_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.4.2/mns_common/db/MongodbUtil.py` & `mns_common-1.0.7.4.3/mns_common/db/MongodbUtil.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.4.2/mns_common/utils/data_frame_util.py` & `mns_common-1.0.7.4.3/mns_common/utils/data_frame_util.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.4.2/mns_common/utils/date_handle_util.py` & `mns_common-1.0.7.4.3/mns_common/utils/date_handle_util.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.4.2/mns_common.egg-info/SOURCES.txt` & `mns_common-1.0.7.4.3/mns_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

