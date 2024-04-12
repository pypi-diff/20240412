# Comparing `tmp/upsies-2024.3.9.tar.gz` & `tmp/upsies-2024.4.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upsies-2024.3.9.tar", last modified: Sat Mar  9 18:30:37 2024, max compression
+gzip compressed data, was "upsies-2024.4.12.tar", last modified: Fri Apr 12 10:16:30 2024, max compression
```

## Comparing `upsies-2024.3.9.tar` & `upsies-2024.4.12.tar`

### file list

```diff
@@ -1,283 +1,283 @@
-drwx------   0 ich       (1000) ich       (1000)        0 2024-03-09 18:30:37.496133 upsies-2024.3.9/
--rw-------   0 ich       (1000) ich       (1000)    35149 2024-01-26 16:22:51.000000 upsies-2024.3.9/LICENSE
--rw-r--r--   0 ich       (1000) ich       (1000)     3780 2024-03-09 18:30:37.492133 upsies-2024.3.9/PKG-INFO
--rw-------   0 ich       (1000) ich       (1000)     1915 2024-01-26 16:44:19.000000 upsies-2024.3.9/README.rst
-drwx------   0 ich       (1000) ich       (1000)        0 2024-03-09 18:30:37.440132 upsies-2024.3.9/docs/
-drwx------   0 ich       (1000) ich       (1000)        0 2024-03-09 18:30:37.440132 upsies-2024.3.9/docs/_ext/
--rw-------   0 ich       (1000) ich       (1000)     2805 2024-01-26 16:22:51.000000 upsies-2024.3.9/docs/_ext/cli_reference.py
--rw-------   0 ich       (1000) ich       (1000)      789 2024-01-26 16:22:51.000000 upsies-2024.3.9/docs/conf.py
--rw-------   0 ich       (1000) ich       (1000)     2325 2024-02-24 18:36:30.000000 upsies-2024.3.9/pyproject.toml
--rw-------   0 ich       (1000) ich       (1000)       38 2024-03-09 18:30:37.496133 upsies-2024.3.9/setup.cfg
-drwx------   0 ich       (1000) ich       (1000)        0 2024-03-09 18:30:37.440132 upsies-2024.3.9/tests/
--rw-------   0 ich       (1000) ich       (1000)      974 2024-01-26 16:22:51.000000 upsies-2024.3.9/tests/conftest.py
--rw-------   0 ich       (1000) ich       (1000)     3756 2024-03-06 10:16:46.000000 upsies-2024.3.9/tests/errors_test.py
-drwx------   0 ich       (1000) ich       (1000)        0 2024-03-09 18:30:37.444131 upsies-2024.3.9/tests/jobs_test/
--rw-------   0 ich       (1000) ich       (1000)     3036 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/jobs_test/add_torrent_job_test.py
--rw-------   0 ich       (1000) ich       (1000)    18319 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/jobs_test/choice_job_test.py
--rw-------   0 ich       (1000) ich       (1000)     4833 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/jobs_test/copy_torrent_job_test.py
--rw-------   0 ich       (1000) ich       (1000)    18719 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/jobs_test/create_torrent_job_test.py
--rw-------   0 ich       (1000) ich       (1000)     4032 2024-02-22 11:14:53.000000 upsies-2024.3.9/tests/jobs_test/custom_job_test.py
--rw-------   0 ich       (1000) ich       (1000)    11267 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/jobs_test/imghost_job_test.py
--rw-------   0 ich       (1000) ich       (1000)    48835 2024-03-06 10:16:46.000000 upsies-2024.3.9/tests/jobs_test/job_base_test.py
--rw-------   0 ich       (1000) ich       (1000)    31750 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/jobs_test/mediainfo_job_test.py
--rw-------   0 ich       (1000) ich       (1000)    30823 2024-03-08 10:45:34.000000 upsies-2024.3.9/tests/jobs_test/poster_job_test.py
--rw-------   0 ich       (1000) ich       (1000)     4022 2024-02-18 11:31:43.000000 upsies-2024.3.9/tests/jobs_test/queue_job_base_test.py
--rw-------   0 ich       (1000) ich       (1000)    19752 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/jobs_test/scene_check_job_test.py
--rw-------   0 ich       (1000) ich       (1000)     3206 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/jobs_test/scene_search_job_test.py
--rw-------   0 ich       (1000) ich       (1000)    47144 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/jobs_test/screenshots_job_test.py
--rw-------   0 ich       (1000) ich       (1000)    13841 2024-02-13 10:51:19.000000 upsies-2024.3.9/tests/jobs_test/set_job_test.py
--rw-------   0 ich       (1000) ich       (1000)    14526 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/jobs_test/submit_job_test.py
--rw-------   0 ich       (1000) ich       (1000)    14526 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/jobs_test/text_field_job_test.py
--rw-------   0 ich       (1000) ich       (1000)    24151 2024-02-24 18:36:30.000000 upsies-2024.3.9/tests/jobs_test/webdb_search_job_test.py
-drwx------   0 ich       (1000) ich       (1000)        0 2024-03-09 18:30:37.444131 upsies-2024.3.9/tests/trackers_test/
-drwx------   0 ich       (1000) ich       (1000)        0 2024-03-09 18:30:37.444131 upsies-2024.3.9/tests/trackers_test/ant/
--rw-------   0 ich       (1000) ich       (1000)     1899 2024-03-09 18:29:18.000000 upsies-2024.3.9/tests/trackers_test/ant/ant_tracker_config_test.py
--rw-------   0 ich       (1000) ich       (1000)     6014 2024-02-27 14:09:57.000000 upsies-2024.3.9/tests/trackers_test/ant/ant_tracker_jobs_test.py
--rw-------   0 ich       (1000) ich       (1000)     8004 2024-03-09 18:29:18.000000 upsies-2024.3.9/tests/trackers_test/ant/ant_tracker_test.py
-drwx------   0 ich       (1000) ich       (1000)        0 2024-03-09 18:30:37.444131 upsies-2024.3.9/tests/trackers_test/base/
--rw-------   0 ich       (1000) ich       (1000)     5708 2024-02-07 12:59:33.000000 upsies-2024.3.9/tests/trackers_test/base/tracker_base_exclude_test.py
--rw-------   0 ich       (1000) ich       (1000)     5603 2024-02-13 10:51:19.000000 upsies-2024.3.9/tests/trackers_test/base/tracker_base_howto_test.py
--rw-------   0 ich       (1000) ich       (1000)     6308 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/trackers_test/base/tracker_base_test.py
--rw-------   0 ich       (1000) ich       (1000)     6223 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/trackers_test/base/tracker_config_base_test.py
--rw-------   0 ich       (1000) ich       (1000)    74842 2024-03-09 18:29:18.000000 upsies-2024.3.9/tests/trackers_test/base/tracker_jobs_base_test.py
-drwx------   0 ich       (1000) ich       (1000)        0 2024-03-09 18:30:37.444131 upsies-2024.3.9/tests/trackers_test/bhd/
--rw-------   0 ich       (1000) ich       (1000)     6461 2024-02-03 14:55:23.000000 upsies-2024.3.9/tests/trackers_test/bhd/bhd_tracker_config_test.py
--rw-------   0 ich       (1000) ich       (1000)    28862 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/trackers_test/bhd/bhd_tracker_jobs_test.py
--rw-------   0 ich       (1000) ich       (1000)    11369 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/trackers_test/bhd/bhd_tracker_test.py
--rw-------   0 ich       (1000) ich       (1000)     1496 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/trackers_test/conftest.py
-drwx------   0 ich       (1000) ich       (1000)        0 2024-03-09 18:30:37.444131 upsies-2024.3.9/tests/trackers_test/mtv/
--rw-------   0 ich       (1000) ich       (1000)     4916 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/trackers_test/mtv/mtv_tracker_config_test.py
--rw-------   0 ich       (1000) ich       (1000)    32342 2024-02-07 12:59:33.000000 upsies-2024.3.9/tests/trackers_test/mtv/mtv_tracker_jobs_test.py
--rw-------   0 ich       (1000) ich       (1000)    32629 2024-02-23 16:54:56.000000 upsies-2024.3.9/tests/trackers_test/mtv/mtv_tracker_test.py
-drwx------   0 ich       (1000) ich       (1000)        0 2024-03-09 18:30:37.444131 upsies-2024.3.9/tests/trackers_test/nbl/
--rw-------   0 ich       (1000) ich       (1000)     1577 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/trackers_test/nbl/nbl_tracker_config_test.py
--rw-------   0 ich       (1000) ich       (1000)     4216 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/trackers_test/nbl/nbl_tracker_jobs_test.py
--rw-------   0 ich       (1000) ich       (1000)     6119 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/trackers_test/nbl/nbl_tracker_test.py
-drwx------   0 ich       (1000) ich       (1000)        0 2024-03-09 18:30:37.448132 upsies-2024.3.9/tests/trackers_test/ptp/
--rw-------   0 ich       (1000) ich       (1000)     2475 2024-03-06 10:16:46.000000 upsies-2024.3.9/tests/trackers_test/ptp/ptp_metadata_test.py
--rw-------   0 ich       (1000) ich       (1000)     5863 2024-02-16 17:01:10.000000 upsies-2024.3.9/tests/trackers_test/ptp/ptp_tracker_config_test.py
--rw-------   0 ich       (1000) ich       (1000)   101119 2024-03-09 18:29:18.000000 upsies-2024.3.9/tests/trackers_test/ptp/ptp_tracker_jobs_test.py
--rw-------   0 ich       (1000) ich       (1000)    40879 2024-03-08 10:45:34.000000 upsies-2024.3.9/tests/trackers_test/ptp/ptp_tracker_test.py
--rw-------   0 ich       (1000) ich       (1000)     1916 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/trackers_test/trackers_test.py
-drwx------   0 ich       (1000) ich       (1000)        0 2024-03-09 18:30:37.448132 upsies-2024.3.9/tests/trackers_test/uhd/
--rw-------   0 ich       (1000) ich       (1000)     5630 2024-02-20 15:06:57.000000 upsies-2024.3.9/tests/trackers_test/uhd/uhd_tracker_config_test.py
--rw-------   0 ich       (1000) ich       (1000)    58690 2024-03-08 16:04:07.000000 upsies-2024.3.9/tests/trackers_test/uhd/uhd_tracker_jobs_test.py
--rw-------   0 ich       (1000) ich       (1000)    22951 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/trackers_test/uhd/uhd_tracker_test.py
-drwx------   0 ich       (1000) ich       (1000)        0 2024-03-09 18:30:37.448132 upsies-2024.3.9/tests/uis_test/
--rw-------   0 ich       (1000) ich       (1000)     3696 2024-03-06 10:16:46.000000 upsies-2024.3.9/tests/uis_test/prompts_test.py
-drwx------   0 ich       (1000) ich       (1000)        0 2024-03-09 18:30:37.448132 upsies-2024.3.9/tests/uis_test/tui_test/
--rw-------   0 ich       (1000) ich       (1000)    22688 2024-03-06 10:16:46.000000 upsies-2024.3.9/tests/uis_test/tui_test/tui_test.py
--rw-------   0 ich       (1000) ich       (1000)     1425 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/uis_test/tui_test/tui_utils_test.py
--rw-------   0 ich       (1000) ich       (1000)     4101 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/uis_test/tui_test/tui_widgets_test.py
-drwx------   0 ich       (1000) ich       (1000)        0 2024-03-09 18:30:37.452132 upsies-2024.3.9/tests/utils_test/
--rw-------   0 ich       (1000) ich       (1000)    10214 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/utils_test/argtypes_test.py
--rw-------   0 ich       (1000) ich       (1000)     9397 2024-01-28 13:35:49.000000 upsies-2024.3.9/tests/utils_test/btclient_test.py
--rw-------   0 ich       (1000) ich       (1000)    36600 2024-02-13 10:51:19.000000 upsies-2024.3.9/tests/utils_test/configfiles_test.py
--rw-------   0 ich       (1000) ich       (1000)     1266 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/utils_test/country_test.py
--rw-------   0 ich       (1000) ich       (1000)     9149 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/utils_test/daemon_test.py
--rw-------   0 ich       (1000) ich       (1000)    32645 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/utils_test/fs_test.py
--rw-------   0 ich       (1000) ich       (1000)     3848 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/utils_test/html_test.py
-drwx------   0 ich       (1000) ich       (1000)        0 2024-03-09 18:30:37.452132 upsies-2024.3.9/tests/utils_test/http_test/
--rw-------   0 ich       (1000) ich       (1000)     1474 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/utils_test/http_test/conftest.py
--rw-------   0 ich       (1000) ich       (1000)    56267 2024-03-06 10:16:46.000000 upsies-2024.3.9/tests/utils_test/http_test/http_test.py
--rw-------   0 ich       (1000) ich       (1000)     1233 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/utils_test/http_test/http_tls_test.py
--rw-------   0 ich       (1000) ich       (1000)     2348 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/utils_test/image_optimize_test.py
--rw-------   0 ich       (1000) ich       (1000)     9198 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/utils_test/image_resize_test.py
--rw-------   0 ich       (1000) ich       (1000)    10428 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/utils_test/image_screenshot_test.py
--rw-------   0 ich       (1000) ich       (1000)      425 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/utils_test/image_test.py
-drwx------   0 ich       (1000) ich       (1000)        0 2024-03-09 18:30:37.456132 upsies-2024.3.9/tests/utils_test/imghosts_test/
--rw-------   0 ich       (1000) ich       (1000)     3390 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/utils_test/imghosts_test/freeimage_test.py
--rw-------   0 ich       (1000) ich       (1000)     3690 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/utils_test/imghosts_test/imgbb_test.py
--rw-------   0 ich       (1000) ich       (1000)     1932 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/utils_test/imghosts_test/imgbox_test.py
--rw-------   0 ich       (1000) ich       (1000)    15660 2024-01-30 15:17:59.000000 upsies-2024.3.9/tests/utils_test/imghosts_test/imghost_base_test.py
--rw-------   0 ich       (1000) ich       (1000)     3055 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/utils_test/imghosts_test/imghost_common_test.py
--rw-------   0 ich       (1000) ich       (1000)     2791 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/utils_test/imghosts_test/imghost_test.py
--rw-------   0 ich       (1000) ich       (1000)     7105 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/utils_test/imghosts_test/ptpimg_test.py
-drwx------   0 ich       (1000) ich       (1000)        0 2024-03-09 18:30:37.456132 upsies-2024.3.9/tests/utils_test/predbs_test/
--rw-------   0 ich       (1000) ich       (1000)     1116 2024-01-30 15:17:59.000000 upsies-2024.3.9/tests/utils_test/predbs_test/conftest.py
--rw-------   0 ich       (1000) ich       (1000)     6369 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/utils_test/predbs_test/corruptnet_test.py
--rw-------   0 ich       (1000) ich       (1000)     5723 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/utils_test/predbs_test/predbclub_test.py
--rw-------   0 ich       (1000) ich       (1000)     6719 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/utils_test/predbs_test/predbde_test.py
--rw-------   0 ich       (1000) ich       (1000)     5710 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/utils_test/predbs_test/predbovh_test.py
--rw-------   0 ich       (1000) ich       (1000)     8255 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/utils_test/predbs_test/predbs_base_test.py
--rw-------   0 ich       (1000) ich       (1000)     8539 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/utils_test/predbs_test/predbs_common_test.py
--rw-------   0 ich       (1000) ich       (1000)    49558 2024-01-30 15:17:59.000000 upsies-2024.3.9/tests/utils_test/predbs_test/predbs_integration_test.py
--rw-------   0 ich       (1000) ich       (1000)    22846 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/utils_test/predbs_test/predbs_multi_test.py
--rw-------   0 ich       (1000) ich       (1000)     1900 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/utils_test/predbs_test/predbs_test.py
--rw-------   0 ich       (1000) ich       (1000)    22438 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/utils_test/predbs_test/srrdb_test.py
--rw-------   0 ich       (1000) ich       (1000)     9604 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/utils_test/release_episodes_test.py
--rw-------   0 ich       (1000) ich       (1000)    31672 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/utils_test/release_info_test.py
--rw-------   0 ich       (1000) ich       (1000)    64416 2024-02-08 15:57:50.000000 upsies-2024.3.9/tests/utils_test/release_name_test.py
--rw-------   0 ich       (1000) ich       (1000)     5791 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/utils_test/signal_test.py
--rw-------   0 ich       (1000) ich       (1000)    10913 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/utils_test/string_test.py
--rw-------   0 ich       (1000) ich       (1000)     2695 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/utils_test/subproc_test.py
--rw-------   0 ich       (1000) ich       (1000)    10675 2024-02-16 17:01:10.000000 upsies-2024.3.9/tests/utils_test/subtitle_test.py
--rw-------   0 ich       (1000) ich       (1000)     3156 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/utils_test/timestamp_test.py
--rw-------   0 ich       (1000) ich       (1000)    30564 2024-02-08 15:57:50.000000 upsies-2024.3.9/tests/utils_test/torrent_test.py
--rw-------   0 ich       (1000) ich       (1000)    22669 2024-02-13 10:51:19.000000 upsies-2024.3.9/tests/utils_test/types_test.py
--rw-------   0 ich       (1000) ich       (1000)     5089 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/utils_test/update_test.py
--rw-------   0 ich       (1000) ich       (1000)    14246 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/utils_test/utils_test.py
--rw-------   0 ich       (1000) ich       (1000)    78592 2024-02-16 17:01:10.000000 upsies-2024.3.9/tests/utils_test/video_test.py
-drwx------   0 ich       (1000) ich       (1000)        0 2024-03-09 18:30:37.456132 upsies-2024.3.9/tests/utils_test/webdbs_test/
--rw-------   0 ich       (1000) ich       (1000)     1423 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/utils_test/webdbs_test/conftest.py
--rw-------   0 ich       (1000) ich       (1000)    32060 2024-02-24 18:36:30.000000 upsies-2024.3.9/tests/utils_test/webdbs_test/imdb_test.py
--rw-------   0 ich       (1000) ich       (1000)    20676 2024-02-27 15:39:02.000000 upsies-2024.3.9/tests/utils_test/webdbs_test/tmdb_test.py
--rw-------   0 ich       (1000) ich       (1000)    25024 2024-01-28 13:35:49.000000 upsies-2024.3.9/tests/utils_test/webdbs_test/tvmaze_test.py
--rw-------   0 ich       (1000) ich       (1000)     6285 2024-02-24 18:36:30.000000 upsies-2024.3.9/tests/utils_test/webdbs_test/webdbs_base_test.py
--rw-------   0 ich       (1000) ich       (1000)    19557 2024-02-24 18:36:30.000000 upsies-2024.3.9/tests/utils_test/webdbs_test/webdbs_common_test.py
--rw-------   0 ich       (1000) ich       (1000)     1903 2024-01-26 16:22:52.000000 upsies-2024.3.9/tests/utils_test/webdbs_test/webdbs_test.py
-drwx------   0 ich       (1000) ich       (1000)        0 2024-03-09 18:30:37.460132 upsies-2024.3.9/upsies/
--rw-------   0 ich       (1000) ich       (1000)     1194 2024-03-09 18:29:18.000000 upsies-2024.3.9/upsies/__init__.py
--rw-------   0 ich       (1000) ich       (1000)       73 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/__main__.py
--rw-------   0 ich       (1000) ich       (1000)     1457 2024-02-13 10:51:19.000000 upsies-2024.3.9/upsies/constants.py
--rw-------   0 ich       (1000) ich       (1000)     2059 2024-02-09 13:32:20.000000 upsies-2024.3.9/upsies/defaults.py
--rw-------   0 ich       (1000) ich       (1000)     6839 2024-03-06 10:16:46.000000 upsies-2024.3.9/upsies/errors.py
-drwx------   0 ich       (1000) ich       (1000)        0 2024-03-09 18:30:37.460132 upsies-2024.3.9/upsies/jobs/
--rw-------   0 ich       (1000) ich       (1000)      215 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/jobs/__init__.py
--rw-------   0 ich       (1000) ich       (1000)    37386 2024-03-06 10:16:46.000000 upsies-2024.3.9/upsies/jobs/base.py
--rw-------   0 ich       (1000) ich       (1000)     2089 2024-02-22 11:14:53.000000 upsies-2024.3.9/upsies/jobs/custom.py
--rw-------   0 ich       (1000) ich       (1000)    22518 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/jobs/dialog.py
--rw-------   0 ich       (1000) ich       (1000)     4996 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/jobs/imghost.py
--rw-------   0 ich       (1000) ich       (1000)     5303 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/jobs/mediainfo.py
--rw-------   0 ich       (1000) ich       (1000)    10199 2024-03-08 10:45:34.000000 upsies-2024.3.9/upsies/jobs/poster.py
--rw-------   0 ich       (1000) ich       (1000)     9155 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/jobs/scene.py
--rw-------   0 ich       (1000) ich       (1000)    19869 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/jobs/screenshots.py
--rw-------   0 ich       (1000) ich       (1000)     3682 2024-02-13 10:51:19.000000 upsies-2024.3.9/upsies/jobs/set.py
--rw-------   0 ich       (1000) ich       (1000)     7836 2024-02-23 10:15:44.000000 upsies-2024.3.9/upsies/jobs/submit.py
--rw-------   0 ich       (1000) ich       (1000)    12771 2024-02-07 13:47:38.000000 upsies-2024.3.9/upsies/jobs/torrent.py
--rw-------   0 ich       (1000) ich       (1000)    13470 2024-02-24 18:36:30.000000 upsies-2024.3.9/upsies/jobs/webdb.py
-drwx------   0 ich       (1000) ich       (1000)        0 2024-03-09 18:30:37.460132 upsies-2024.3.9/upsies/trackers/
--rw-------   0 ich       (1000) ich       (1000)     1385 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/trackers/__init__.py
-drwx------   0 ich       (1000) ich       (1000)        0 2024-03-09 18:30:37.464132 upsies-2024.3.9/upsies/trackers/ant/
--rw-------   0 ich       (1000) ich       (1000)      119 2024-02-27 14:09:57.000000 upsies-2024.3.9/upsies/trackers/ant/__init__.py
--rw-------   0 ich       (1000) ich       (1000)      852 2024-03-09 18:29:18.000000 upsies-2024.3.9/upsies/trackers/ant/config.py
--rw-------   0 ich       (1000) ich       (1000)     2866 2024-02-27 14:09:57.000000 upsies-2024.3.9/upsies/trackers/ant/jobs.py
--rw-------   0 ich       (1000) ich       (1000)     4899 2024-03-09 18:29:18.000000 upsies-2024.3.9/upsies/trackers/ant/tracker.py
-drwx------   0 ich       (1000) ich       (1000)        0 2024-03-09 18:30:37.464132 upsies-2024.3.9/upsies/trackers/base/
--rw-------   0 ich       (1000) ich       (1000)      149 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/trackers/base/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     5889 2024-02-13 10:51:19.000000 upsies-2024.3.9/upsies/trackers/base/_howto.py
--rw-------   0 ich       (1000) ich       (1000)     3101 2024-02-09 13:47:32.000000 upsies-2024.3.9/upsies/trackers/base/config.py
--rw-------   0 ich       (1000) ich       (1000)     1191 2024-02-03 17:36:34.000000 upsies-2024.3.9/upsies/trackers/base/exclude.py
--rw-------   0 ich       (1000) ich       (1000)    38592 2024-03-09 18:29:18.000000 upsies-2024.3.9/upsies/trackers/base/jobs.py
--rw-------   0 ich       (1000) ich       (1000)     6748 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/trackers/base/tracker.py
-drwx------   0 ich       (1000) ich       (1000)        0 2024-03-09 18:30:37.464132 upsies-2024.3.9/upsies/trackers/bhd/
--rw-------   0 ich       (1000) ich       (1000)      119 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/trackers/bhd/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     4392 2024-02-09 13:47:42.000000 upsies-2024.3.9/upsies/trackers/bhd/config.py
--rw-------   0 ich       (1000) ich       (1000)    16191 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/trackers/bhd/jobs.py
--rw-------   0 ich       (1000) ich       (1000)     6269 2024-02-27 09:48:09.000000 upsies-2024.3.9/upsies/trackers/bhd/tracker.py
--rw-------   0 ich       (1000) ich       (1000)     9636 2024-02-22 15:05:39.000000 upsies-2024.3.9/upsies/trackers/dummy.py
-drwx------   0 ich       (1000) ich       (1000)        0 2024-03-09 18:30:37.464132 upsies-2024.3.9/upsies/trackers/mtv/
--rw-------   0 ich       (1000) ich       (1000)      119 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/trackers/mtv/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     2976 2024-02-03 10:17:51.000000 upsies-2024.3.9/upsies/trackers/mtv/config.py
--rw-------   0 ich       (1000) ich       (1000)    10358 2024-01-31 10:06:16.000000 upsies-2024.3.9/upsies/trackers/mtv/jobs.py
--rw-------   0 ich       (1000) ich       (1000)    14458 2024-02-23 16:54:56.000000 upsies-2024.3.9/upsies/trackers/mtv/tracker.py
-drwx------   0 ich       (1000) ich       (1000)        0 2024-03-09 18:30:37.468132 upsies-2024.3.9/upsies/trackers/nbl/
--rw-------   0 ich       (1000) ich       (1000)      119 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/trackers/nbl/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     1059 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/trackers/nbl/config.py
--rw-------   0 ich       (1000) ich       (1000)     1801 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/trackers/nbl/jobs.py
--rw-------   0 ich       (1000) ich       (1000)     3879 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/trackers/nbl/tracker.py
-drwx------   0 ich       (1000) ich       (1000)        0 2024-03-09 18:30:37.468132 upsies-2024.3.9/upsies/trackers/ptp/
--rw-------   0 ich       (1000) ich       (1000)      119 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/trackers/ptp/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     3693 2024-02-19 15:24:34.000000 upsies-2024.3.9/upsies/trackers/ptp/config.py
--rw-------   0 ich       (1000) ich       (1000)    43313 2024-03-09 18:29:18.000000 upsies-2024.3.9/upsies/trackers/ptp/jobs.py
--rw-------   0 ich       (1000) ich       (1000)     4545 2024-03-06 10:16:46.000000 upsies-2024.3.9/upsies/trackers/ptp/metadata.py
--rw-------   0 ich       (1000) ich       (1000)    19392 2024-03-09 18:29:18.000000 upsies-2024.3.9/upsies/trackers/ptp/tracker.py
-drwx------   0 ich       (1000) ich       (1000)        0 2024-03-09 18:30:37.468132 upsies-2024.3.9/upsies/trackers/uhd/
--rw-------   0 ich       (1000) ich       (1000)      119 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/trackers/uhd/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     3125 2024-02-20 15:06:57.000000 upsies-2024.3.9/upsies/trackers/uhd/config.py
--rw-------   0 ich       (1000) ich       (1000)    26926 2024-03-08 14:50:46.000000 upsies-2024.3.9/upsies/trackers/uhd/jobs.py
--rw-------   0 ich       (1000) ich       (1000)     8695 2024-02-20 11:12:54.000000 upsies-2024.3.9/upsies/trackers/uhd/tracker.py
-drwx------   0 ich       (1000) ich       (1000)        0 2024-03-09 18:30:37.468132 upsies-2024.3.9/upsies/uis/
--rw-------   0 ich       (1000) ich       (1000)      163 2024-02-20 15:50:34.000000 upsies-2024.3.9/upsies/uis/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     3560 2024-03-06 10:16:46.000000 upsies-2024.3.9/upsies/uis/prompts.py
-drwx------   0 ich       (1000) ich       (1000)        0 2024-03-09 18:30:37.472132 upsies-2024.3.9/upsies/uis/tui/
--rw-------   0 ich       (1000) ich       (1000)       55 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/uis/tui/__init__.py
-drwx------   0 ich       (1000) ich       (1000)        0 2024-03-09 18:30:37.472132 upsies-2024.3.9/upsies/uis/tui/commands/
--rw-------   0 ich       (1000) ich       (1000)     1319 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/uis/tui/commands/__init__.py
--rw-------   0 ich       (1000) ich       (1000)    15248 2024-02-09 13:33:18.000000 upsies-2024.3.9/upsies/uis/tui/commands/base.py
--rw-------   0 ich       (1000) ich       (1000)     2279 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/uis/tui/commands/mediainfo.py
--rw-------   0 ich       (1000) ich       (1000)     3979 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/uis/tui/commands/poster.py
--rw-------   0 ich       (1000) ich       (1000)     2530 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/uis/tui/commands/release_name.py
--rw-------   0 ich       (1000) ich       (1000)     2710 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/uis/tui/commands/scene.py
--rw-------   0 ich       (1000) ich       (1000)     4710 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/uis/tui/commands/screenshots.py
--rw-------   0 ich       (1000) ich       (1000)     6117 2024-02-22 11:14:53.000000 upsies-2024.3.9/upsies/uis/tui/commands/set.py
--rw-------   0 ich       (1000) ich       (1000)     8661 2024-02-07 13:44:15.000000 upsies-2024.3.9/upsies/uis/tui/commands/submit.py
--rw-------   0 ich       (1000) ich       (1000)    10345 2024-02-12 13:49:50.000000 upsies-2024.3.9/upsies/uis/tui/commands/torrent.py
--rw-------   0 ich       (1000) ich       (1000)     2091 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/uis/tui/commands/upload_images.py
--rw-------   0 ich       (1000) ich       (1000)     1799 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/uis/tui/commands/webdb.py
--rw-------   0 ich       (1000) ich       (1000)     2943 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/uis/tui/headless.py
-drwx------   0 ich       (1000) ich       (1000)        0 2024-03-09 18:30:37.476132 upsies-2024.3.9/upsies/uis/tui/jobwidgets/
--rw-------   0 ich       (1000) ich       (1000)      947 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/uis/tui/jobwidgets/__init__.py
--rw-------   0 ich       (1000) ich       (1000)    10706 2024-03-08 13:58:19.000000 upsies-2024.3.9/upsies/uis/tui/jobwidgets/base.py
--rw-------   0 ich       (1000) ich       (1000)      281 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/uis/tui/jobwidgets/config.py
--rw-------   0 ich       (1000) ich       (1000)     1156 2024-03-06 10:16:46.000000 upsies-2024.3.9/upsies/uis/tui/jobwidgets/custom.py
--rw-------   0 ich       (1000) ich       (1000)     3257 2024-02-29 13:37:30.000000 upsies-2024.3.9/upsies/uis/tui/jobwidgets/dialog.py
--rw-------   0 ich       (1000) ich       (1000)      796 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/uis/tui/jobwidgets/imghost.py
--rw-------   0 ich       (1000) ich       (1000)      234 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/uis/tui/jobwidgets/mediainfo.py
--rw-------   0 ich       (1000) ich       (1000)     1259 2024-02-20 15:50:34.000000 upsies-2024.3.9/upsies/uis/tui/jobwidgets/poster.py
--rw-------   0 ich       (1000) ich       (1000)     4718 2024-03-06 10:16:46.000000 upsies-2024.3.9/upsies/uis/tui/jobwidgets/scene.py
--rw-------   0 ich       (1000) ich       (1000)     1737 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/uis/tui/jobwidgets/screenshots.py
--rw-------   0 ich       (1000) ich       (1000)      715 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/uis/tui/jobwidgets/submit.py
--rw-------   0 ich       (1000) ich       (1000)     9132 2024-02-07 17:06:55.000000 upsies-2024.3.9/upsies/uis/tui/jobwidgets/torrent.py
--rw-------   0 ich       (1000) ich       (1000)    13859 2024-02-26 09:50:52.000000 upsies-2024.3.9/upsies/uis/tui/jobwidgets/webdb.py
--rw-------   0 ich       (1000) ich       (1000)     3009 2024-02-02 11:42:37.000000 upsies-2024.3.9/upsies/uis/tui/main.py
--rw-------   0 ich       (1000) ich       (1000)     1402 2024-03-06 10:16:46.000000 upsies-2024.3.9/upsies/uis/tui/style.py
--rw-------   0 ich       (1000) ich       (1000)    12653 2024-03-06 10:16:46.000000 upsies-2024.3.9/upsies/uis/tui/tui.py
--rw-------   0 ich       (1000) ich       (1000)      626 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/uis/tui/utils.py
--rw-------   0 ich       (1000) ich       (1000)    17036 2024-03-06 10:16:46.000000 upsies-2024.3.9/upsies/uis/tui/widgets.py
-drwx------   0 ich       (1000) ich       (1000)        0 2024-03-09 18:30:37.484133 upsies-2024.3.9/upsies/utils/
--rw-------   0 ich       (1000) ich       (1000)    12361 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/utils/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     5777 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/utils/argtypes.py
--rw-------   0 ich       (1000) ich       (1000)      302 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/utils/browser.py
--rw-------   0 ich       (1000) ich       (1000)     5593 2024-02-03 17:36:34.000000 upsies-2024.3.9/upsies/utils/btclient.py
--rw-------   0 ich       (1000) ich       (1000)    15785 2024-02-13 10:51:19.000000 upsies-2024.3.9/upsies/utils/configfiles.py
--rw-------   0 ich       (1000) ich       (1000)     1825 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/utils/country.py
--rw-------   0 ich       (1000) ich       (1000)     7457 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/utils/daemon.py
--rw-------   0 ich       (1000) ich       (1000)    18714 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/utils/fs.py
--rw-------   0 ich       (1000) ich       (1000)     2749 2024-02-23 11:29:01.000000 upsies-2024.3.9/upsies/utils/html.py
--rw-------   0 ich       (1000) ich       (1000)    24349 2024-03-06 10:16:46.000000 upsies-2024.3.9/upsies/utils/http.py
--rw-------   0 ich       (1000) ich       (1000)    10618 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/utils/image.py
-drwx------   0 ich       (1000) ich       (1000)        0 2024-03-09 18:30:37.488133 upsies-2024.3.9/upsies/utils/imghosts/
--rw-------   0 ich       (1000) ich       (1000)     1391 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/utils/imghosts/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     6802 2024-01-30 15:17:59.000000 upsies-2024.3.9/upsies/utils/imghosts/base.py
--rw-------   0 ich       (1000) ich       (1000)     1147 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/utils/imghosts/common.py
--rw-------   0 ich       (1000) ich       (1000)      932 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/utils/imghosts/dummy.py
--rw-------   0 ich       (1000) ich       (1000)     1997 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/utils/imghosts/freeimage.py
--rw-------   0 ich       (1000) ich       (1000)     2459 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/utils/imghosts/imgbb.py
--rw-------   0 ich       (1000) ich       (1000)      912 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/utils/imghosts/imgbox.py
--rw-------   0 ich       (1000) ich       (1000)     3332 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/utils/imghosts/ptpimg.py
-drwx------   0 ich       (1000) ich       (1000)        0 2024-03-09 18:30:37.492133 upsies-2024.3.9/upsies/utils/predbs/
--rw-------   0 ich       (1000) ich       (1000)     1364 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/utils/predbs/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     9619 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/utils/predbs/base.py
--rw-------   0 ich       (1000) ich       (1000)     4128 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/utils/predbs/common.py
--rw-------   0 ich       (1000) ich       (1000)     2278 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/utils/predbs/corruptnet.py
--rw-------   0 ich       (1000) ich       (1000)    20881 2024-01-30 14:38:02.000000 upsies-2024.3.9/upsies/utils/predbs/multi.py
--rw-------   0 ich       (1000) ich       (1000)     2176 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/utils/predbs/predbclub.py
--rw-------   0 ich       (1000) ich       (1000)     2414 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/utils/predbs/predbde.py
--rw-------   0 ich       (1000) ich       (1000)     2169 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/utils/predbs/predbovh.py
--rw-------   0 ich       (1000) ich       (1000)     5425 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/utils/predbs/query.py
--rw-------   0 ich       (1000) ich       (1000)     6654 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/utils/predbs/srrdb.py
--rw-------   0 ich       (1000) ich       (1000)    56269 2024-03-03 11:09:35.000000 upsies-2024.3.9/upsies/utils/release.py
--rw-------   0 ich       (1000) ich       (1000)     4366 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/utils/signal.py
--rw-------   0 ich       (1000) ich       (1000)     5154 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/utils/string.py
--rw-------   0 ich       (1000) ich       (1000)     1908 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/utils/subproc.py
--rw-------   0 ich       (1000) ich       (1000)     8297 2024-02-16 17:01:10.000000 upsies-2024.3.9/upsies/utils/subtitle.py
--rw-------   0 ich       (1000) ich       (1000)     2034 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/utils/timestamp.py
--rw-------   0 ich       (1000) ich       (1000)    19817 2024-03-09 18:29:18.000000 upsies-2024.3.9/upsies/utils/torrent.py
--rw-------   0 ich       (1000) ich       (1000)    16509 2024-02-13 10:51:19.000000 upsies-2024.3.9/upsies/utils/types.py
--rw-------   0 ich       (1000) ich       (1000)     2927 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/utils/update.py
--rw-------   0 ich       (1000) ich       (1000)    37644 2024-02-16 17:01:10.000000 upsies-2024.3.9/upsies/utils/video.py
-drwx------   0 ich       (1000) ich       (1000)        0 2024-03-09 18:30:37.492133 upsies-2024.3.9/upsies/utils/webdbs/
--rw-------   0 ich       (1000) ich       (1000)     1140 2024-01-26 16:22:52.000000 upsies-2024.3.9/upsies/utils/webdbs/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     9725 2024-02-24 18:36:30.000000 upsies-2024.3.9/upsies/utils/webdbs/base.py
--rw-------   0 ich       (1000) ich       (1000)    12698 2024-02-24 18:36:30.000000 upsies-2024.3.9/upsies/utils/webdbs/common.py
--rw-------   0 ich       (1000) ich       (1000)    13721 2024-02-24 18:36:30.000000 upsies-2024.3.9/upsies/utils/webdbs/imdb.py
--rw-------   0 ich       (1000) ich       (1000)    12748 2024-02-27 15:39:02.000000 upsies-2024.3.9/upsies/utils/webdbs/tmdb.py
--rw-------   0 ich       (1000) ich       (1000)     9826 2024-02-24 18:36:30.000000 upsies-2024.3.9/upsies/utils/webdbs/tvmaze.py
-drwx------   0 ich       (1000) ich       (1000)        0 2024-03-09 18:30:37.492133 upsies-2024.3.9/upsies.egg-info/
--rw-r--r--   0 ich       (1000) ich       (1000)     3780 2024-03-09 18:30:37.000000 upsies-2024.3.9/upsies.egg-info/PKG-INFO
--rw-------   0 ich       (1000) ich       (1000)     8176 2024-03-09 18:30:37.000000 upsies-2024.3.9/upsies.egg-info/SOURCES.txt
--rw-------   0 ich       (1000) ich       (1000)        1 2024-03-09 18:30:37.000000 upsies-2024.3.9/upsies.egg-info/dependency_links.txt
--rw-------   0 ich       (1000) ich       (1000)       47 2024-03-09 18:30:37.000000 upsies-2024.3.9/upsies.egg-info/entry_points.txt
--rw-------   0 ich       (1000) ich       (1000)      388 2024-03-09 18:30:37.000000 upsies-2024.3.9/upsies.egg-info/requires.txt
--rw-------   0 ich       (1000) ich       (1000)       74 2024-03-09 18:30:37.000000 upsies-2024.3.9/upsies.egg-info/top_level.txt
+drwx------   0 ich       (1000) ich       (1000)        0 2024-04-12 10:16:30.604498 upsies-2024.4.12/
+-rw-------   0 ich       (1000) ich       (1000)    35149 2024-01-26 16:22:51.000000 upsies-2024.4.12/LICENSE
+-rw-r--r--   0 ich       (1000) ich       (1000)     4106 2024-04-12 10:16:30.604498 upsies-2024.4.12/PKG-INFO
+-rw-------   0 ich       (1000) ich       (1000)     2240 2024-04-11 13:54:29.000000 upsies-2024.4.12/README.rst
+drwx------   0 ich       (1000) ich       (1000)        0 2024-04-12 10:16:30.564497 upsies-2024.4.12/docs/
+drwx------   0 ich       (1000) ich       (1000)        0 2024-04-12 10:16:30.564497 upsies-2024.4.12/docs/_ext/
+-rw-------   0 ich       (1000) ich       (1000)     2805 2024-01-26 16:22:51.000000 upsies-2024.4.12/docs/_ext/cli_reference.py
+-rw-------   0 ich       (1000) ich       (1000)      789 2024-01-26 16:22:51.000000 upsies-2024.4.12/docs/conf.py
+-rw-------   0 ich       (1000) ich       (1000)     2325 2024-02-24 18:36:30.000000 upsies-2024.4.12/pyproject.toml
+-rw-------   0 ich       (1000) ich       (1000)       38 2024-04-12 10:16:30.604498 upsies-2024.4.12/setup.cfg
+drwx------   0 ich       (1000) ich       (1000)        0 2024-04-12 10:16:30.564497 upsies-2024.4.12/tests/
+-rw-------   0 ich       (1000) ich       (1000)      974 2024-01-26 16:22:51.000000 upsies-2024.4.12/tests/conftest.py
+-rw-------   0 ich       (1000) ich       (1000)     3756 2024-03-06 10:16:46.000000 upsies-2024.4.12/tests/errors_test.py
+drwx------   0 ich       (1000) ich       (1000)        0 2024-04-12 10:16:30.568497 upsies-2024.4.12/tests/jobs_test/
+-rw-------   0 ich       (1000) ich       (1000)     3036 2024-01-26 16:22:52.000000 upsies-2024.4.12/tests/jobs_test/add_torrent_job_test.py
+-rw-------   0 ich       (1000) ich       (1000)    18319 2024-01-26 16:22:52.000000 upsies-2024.4.12/tests/jobs_test/choice_job_test.py
+-rw-------   0 ich       (1000) ich       (1000)     4833 2024-01-26 16:22:52.000000 upsies-2024.4.12/tests/jobs_test/copy_torrent_job_test.py
+-rw-------   0 ich       (1000) ich       (1000)    18716 2024-04-07 12:42:40.000000 upsies-2024.4.12/tests/jobs_test/create_torrent_job_test.py
+-rw-------   0 ich       (1000) ich       (1000)     4032 2024-02-22 11:14:53.000000 upsies-2024.4.12/tests/jobs_test/custom_job_test.py
+-rw-------   0 ich       (1000) ich       (1000)    11267 2024-01-26 16:22:52.000000 upsies-2024.4.12/tests/jobs_test/imghost_job_test.py
+-rw-------   0 ich       (1000) ich       (1000)    48835 2024-03-06 10:16:46.000000 upsies-2024.4.12/tests/jobs_test/job_base_test.py
+-rw-------   0 ich       (1000) ich       (1000)    31750 2024-01-26 16:22:52.000000 upsies-2024.4.12/tests/jobs_test/mediainfo_job_test.py
+-rw-------   0 ich       (1000) ich       (1000)    31145 2024-03-11 17:27:17.000000 upsies-2024.4.12/tests/jobs_test/poster_job_test.py
+-rw-------   0 ich       (1000) ich       (1000)     4022 2024-02-18 11:31:43.000000 upsies-2024.4.12/tests/jobs_test/queue_job_base_test.py
+-rw-------   0 ich       (1000) ich       (1000)    19752 2024-01-26 16:22:52.000000 upsies-2024.4.12/tests/jobs_test/scene_check_job_test.py
+-rw-------   0 ich       (1000) ich       (1000)     3206 2024-01-26 16:22:52.000000 upsies-2024.4.12/tests/jobs_test/scene_search_job_test.py
+-rw-------   0 ich       (1000) ich       (1000)    49216 2024-03-16 17:48:37.000000 upsies-2024.4.12/tests/jobs_test/screenshots_job_test.py
+-rw-------   0 ich       (1000) ich       (1000)    13841 2024-02-13 10:51:19.000000 upsies-2024.4.12/tests/jobs_test/set_job_test.py
+-rw-------   0 ich       (1000) ich       (1000)    14564 2024-04-07 12:42:40.000000 upsies-2024.4.12/tests/jobs_test/submit_job_test.py
+-rw-------   0 ich       (1000) ich       (1000)    14526 2024-01-26 16:22:52.000000 upsies-2024.4.12/tests/jobs_test/text_field_job_test.py
+-rw-------   0 ich       (1000) ich       (1000)    25998 2024-04-10 14:04:50.000000 upsies-2024.4.12/tests/jobs_test/webdb_search_job_test.py
+drwx------   0 ich       (1000) ich       (1000)        0 2024-04-12 10:16:30.568497 upsies-2024.4.12/tests/trackers_test/
+drwx------   0 ich       (1000) ich       (1000)        0 2024-04-12 10:16:30.568497 upsies-2024.4.12/tests/trackers_test/ant/
+-rw-------   0 ich       (1000) ich       (1000)     2468 2024-04-07 12:42:40.000000 upsies-2024.4.12/tests/trackers_test/ant/ant_tracker_config_test.py
+-rw-------   0 ich       (1000) ich       (1000)     7715 2024-03-21 15:33:14.000000 upsies-2024.4.12/tests/trackers_test/ant/ant_tracker_jobs_test.py
+-rw-------   0 ich       (1000) ich       (1000)     8101 2024-04-07 12:42:40.000000 upsies-2024.4.12/tests/trackers_test/ant/ant_tracker_test.py
+drwx------   0 ich       (1000) ich       (1000)        0 2024-04-12 10:16:30.568497 upsies-2024.4.12/tests/trackers_test/base/
+-rw-------   0 ich       (1000) ich       (1000)     5708 2024-02-07 12:59:33.000000 upsies-2024.4.12/tests/trackers_test/base/tracker_base_exclude_test.py
+-rw-------   0 ich       (1000) ich       (1000)     5602 2024-03-11 17:27:17.000000 upsies-2024.4.12/tests/trackers_test/base/tracker_base_howto_test.py
+-rw-------   0 ich       (1000) ich       (1000)     6356 2024-04-07 12:42:40.000000 upsies-2024.4.12/tests/trackers_test/base/tracker_base_test.py
+-rw-------   0 ich       (1000) ich       (1000)     5554 2024-04-07 12:42:40.000000 upsies-2024.4.12/tests/trackers_test/base/tracker_config_base_test.py
+-rw-------   0 ich       (1000) ich       (1000)    75925 2024-04-07 12:42:40.000000 upsies-2024.4.12/tests/trackers_test/base/tracker_jobs_base_test.py
+drwx------   0 ich       (1000) ich       (1000)        0 2024-04-12 10:16:30.568497 upsies-2024.4.12/tests/trackers_test/bhd/
+-rw-------   0 ich       (1000) ich       (1000)     6665 2024-04-07 12:42:40.000000 upsies-2024.4.12/tests/trackers_test/bhd/bhd_tracker_config_test.py
+-rw-------   0 ich       (1000) ich       (1000)    28862 2024-01-26 16:22:52.000000 upsies-2024.4.12/tests/trackers_test/bhd/bhd_tracker_jobs_test.py
+-rw-------   0 ich       (1000) ich       (1000)    11466 2024-04-07 12:42:40.000000 upsies-2024.4.12/tests/trackers_test/bhd/bhd_tracker_test.py
+-rw-------   0 ich       (1000) ich       (1000)     1496 2024-01-26 16:22:52.000000 upsies-2024.4.12/tests/trackers_test/conftest.py
+drwx------   0 ich       (1000) ich       (1000)        0 2024-04-12 10:16:30.568497 upsies-2024.4.12/tests/trackers_test/mtv/
+-rw-------   0 ich       (1000) ich       (1000)     5120 2024-04-07 12:42:40.000000 upsies-2024.4.12/tests/trackers_test/mtv/mtv_tracker_config_test.py
+-rw-------   0 ich       (1000) ich       (1000)    32342 2024-02-07 12:59:33.000000 upsies-2024.4.12/tests/trackers_test/mtv/mtv_tracker_jobs_test.py
+-rw-------   0 ich       (1000) ich       (1000)    32726 2024-04-07 12:42:40.000000 upsies-2024.4.12/tests/trackers_test/mtv/mtv_tracker_test.py
+drwx------   0 ich       (1000) ich       (1000)        0 2024-04-12 10:16:30.572497 upsies-2024.4.12/tests/trackers_test/nbl/
+-rw-------   0 ich       (1000) ich       (1000)     1453 2024-04-07 12:42:40.000000 upsies-2024.4.12/tests/trackers_test/nbl/nbl_tracker_config_test.py
+-rw-------   0 ich       (1000) ich       (1000)     4216 2024-01-26 16:22:52.000000 upsies-2024.4.12/tests/trackers_test/nbl/nbl_tracker_jobs_test.py
+-rw-------   0 ich       (1000) ich       (1000)     6220 2024-04-07 12:42:40.000000 upsies-2024.4.12/tests/trackers_test/nbl/nbl_tracker_test.py
+drwx------   0 ich       (1000) ich       (1000)        0 2024-04-12 10:16:30.572497 upsies-2024.4.12/tests/trackers_test/ptp/
+-rw-------   0 ich       (1000) ich       (1000)     4438 2024-04-07 12:42:40.000000 upsies-2024.4.12/tests/trackers_test/ptp/ptp_metadata_test.py
+-rw-------   0 ich       (1000) ich       (1000)     7508 2024-04-10 14:04:50.000000 upsies-2024.4.12/tests/trackers_test/ptp/ptp_tracker_config_test.py
+-rw-------   0 ich       (1000) ich       (1000)   104001 2024-04-10 14:04:50.000000 upsies-2024.4.12/tests/trackers_test/ptp/ptp_tracker_jobs_test.py
+-rw-------   0 ich       (1000) ich       (1000)    41147 2024-04-07 12:42:40.000000 upsies-2024.4.12/tests/trackers_test/ptp/ptp_tracker_test.py
+-rw-------   0 ich       (1000) ich       (1000)     1916 2024-01-26 16:22:52.000000 upsies-2024.4.12/tests/trackers_test/trackers_test.py
+drwx------   0 ich       (1000) ich       (1000)        0 2024-04-12 10:16:30.572497 upsies-2024.4.12/tests/trackers_test/uhd/
+-rw-------   0 ich       (1000) ich       (1000)     5525 2024-04-07 12:42:40.000000 upsies-2024.4.12/tests/trackers_test/uhd/uhd_tracker_config_test.py
+-rw-------   0 ich       (1000) ich       (1000)    58946 2024-03-21 15:33:14.000000 upsies-2024.4.12/tests/trackers_test/uhd/uhd_tracker_jobs_test.py
+-rw-------   0 ich       (1000) ich       (1000)    21820 2024-04-10 14:04:50.000000 upsies-2024.4.12/tests/trackers_test/uhd/uhd_tracker_test.py
+drwx------   0 ich       (1000) ich       (1000)        0 2024-04-12 10:16:30.572497 upsies-2024.4.12/tests/uis_test/
+-rw-------   0 ich       (1000) ich       (1000)     3696 2024-03-06 10:16:46.000000 upsies-2024.4.12/tests/uis_test/prompts_test.py
+drwx------   0 ich       (1000) ich       (1000)        0 2024-04-12 10:16:30.572497 upsies-2024.4.12/tests/uis_test/tui_test/
+-rw-------   0 ich       (1000) ich       (1000)    22688 2024-03-06 10:16:46.000000 upsies-2024.4.12/tests/uis_test/tui_test/tui_test.py
+-rw-------   0 ich       (1000) ich       (1000)     1425 2024-01-26 16:22:52.000000 upsies-2024.4.12/tests/uis_test/tui_test/tui_utils_test.py
+-rw-------   0 ich       (1000) ich       (1000)     4101 2024-01-26 16:22:52.000000 upsies-2024.4.12/tests/uis_test/tui_test/tui_widgets_test.py
+drwx------   0 ich       (1000) ich       (1000)        0 2024-04-12 10:16:30.576497 upsies-2024.4.12/tests/utils_test/
+-rw-------   0 ich       (1000) ich       (1000)    10214 2024-01-26 16:22:52.000000 upsies-2024.4.12/tests/utils_test/argtypes_test.py
+-rw-------   0 ich       (1000) ich       (1000)     9397 2024-01-28 13:35:49.000000 upsies-2024.4.12/tests/utils_test/btclient_test.py
+-rw-------   0 ich       (1000) ich       (1000)    38522 2024-03-21 15:33:14.000000 upsies-2024.4.12/tests/utils_test/configfiles_test.py
+-rw-------   0 ich       (1000) ich       (1000)     1266 2024-01-26 16:22:52.000000 upsies-2024.4.12/tests/utils_test/country_test.py
+-rw-------   0 ich       (1000) ich       (1000)     9149 2024-01-26 16:22:52.000000 upsies-2024.4.12/tests/utils_test/daemon_test.py
+-rw-------   0 ich       (1000) ich       (1000)    32645 2024-01-26 16:22:52.000000 upsies-2024.4.12/tests/utils_test/fs_test.py
+-rw-------   0 ich       (1000) ich       (1000)     3848 2024-01-26 16:22:52.000000 upsies-2024.4.12/tests/utils_test/html_test.py
+drwx------   0 ich       (1000) ich       (1000)        0 2024-04-12 10:16:30.576497 upsies-2024.4.12/tests/utils_test/http_test/
+-rw-------   0 ich       (1000) ich       (1000)     1474 2024-01-26 16:22:52.000000 upsies-2024.4.12/tests/utils_test/http_test/conftest.py
+-rw-------   0 ich       (1000) ich       (1000)    59029 2024-04-12 10:12:23.000000 upsies-2024.4.12/tests/utils_test/http_test/http_test.py
+-rw-------   0 ich       (1000) ich       (1000)     1233 2024-01-26 16:22:52.000000 upsies-2024.4.12/tests/utils_test/http_test/http_tls_test.py
+-rw-------   0 ich       (1000) ich       (1000)     2348 2024-01-26 16:22:52.000000 upsies-2024.4.12/tests/utils_test/image_optimize_test.py
+-rw-------   0 ich       (1000) ich       (1000)     9198 2024-01-26 16:22:52.000000 upsies-2024.4.12/tests/utils_test/image_resize_test.py
+-rw-------   0 ich       (1000) ich       (1000)    10485 2024-04-04 09:35:14.000000 upsies-2024.4.12/tests/utils_test/image_screenshot_test.py
+-rw-------   0 ich       (1000) ich       (1000)      425 2024-01-26 16:22:52.000000 upsies-2024.4.12/tests/utils_test/image_test.py
+drwx------   0 ich       (1000) ich       (1000)        0 2024-04-12 10:16:30.580498 upsies-2024.4.12/tests/utils_test/imghosts_test/
+-rw-------   0 ich       (1000) ich       (1000)     3390 2024-01-26 16:22:52.000000 upsies-2024.4.12/tests/utils_test/imghosts_test/freeimage_test.py
+-rw-------   0 ich       (1000) ich       (1000)     3690 2024-01-26 16:22:52.000000 upsies-2024.4.12/tests/utils_test/imghosts_test/imgbb_test.py
+-rw-------   0 ich       (1000) ich       (1000)     1932 2024-01-26 16:22:52.000000 upsies-2024.4.12/tests/utils_test/imghosts_test/imgbox_test.py
+-rw-------   0 ich       (1000) ich       (1000)    15660 2024-01-30 15:17:59.000000 upsies-2024.4.12/tests/utils_test/imghosts_test/imghost_base_test.py
+-rw-------   0 ich       (1000) ich       (1000)     3055 2024-01-26 16:22:52.000000 upsies-2024.4.12/tests/utils_test/imghosts_test/imghost_common_test.py
+-rw-------   0 ich       (1000) ich       (1000)     2791 2024-01-26 16:22:52.000000 upsies-2024.4.12/tests/utils_test/imghosts_test/imghost_test.py
+-rw-------   0 ich       (1000) ich       (1000)     7105 2024-01-26 16:22:52.000000 upsies-2024.4.12/tests/utils_test/imghosts_test/ptpimg_test.py
+drwx------   0 ich       (1000) ich       (1000)        0 2024-04-12 10:16:30.580498 upsies-2024.4.12/tests/utils_test/predbs_test/
+-rw-------   0 ich       (1000) ich       (1000)     1116 2024-01-30 15:17:59.000000 upsies-2024.4.12/tests/utils_test/predbs_test/conftest.py
+-rw-------   0 ich       (1000) ich       (1000)     6369 2024-01-26 16:22:52.000000 upsies-2024.4.12/tests/utils_test/predbs_test/corruptnet_test.py
+-rw-------   0 ich       (1000) ich       (1000)     5723 2024-01-26 16:22:52.000000 upsies-2024.4.12/tests/utils_test/predbs_test/predbclub_test.py
+-rw-------   0 ich       (1000) ich       (1000)     6719 2024-01-26 16:22:52.000000 upsies-2024.4.12/tests/utils_test/predbs_test/predbde_test.py
+-rw-------   0 ich       (1000) ich       (1000)     5710 2024-01-26 16:22:52.000000 upsies-2024.4.12/tests/utils_test/predbs_test/predbovh_test.py
+-rw-------   0 ich       (1000) ich       (1000)     8255 2024-01-26 16:22:52.000000 upsies-2024.4.12/tests/utils_test/predbs_test/predbs_base_test.py
+-rw-------   0 ich       (1000) ich       (1000)     8539 2024-04-11 13:58:04.000000 upsies-2024.4.12/tests/utils_test/predbs_test/predbs_common_test.py
+-rw-------   0 ich       (1000) ich       (1000)    49558 2024-01-30 15:17:59.000000 upsies-2024.4.12/tests/utils_test/predbs_test/predbs_integration_test.py
+-rw-------   0 ich       (1000) ich       (1000)    22846 2024-01-26 16:22:52.000000 upsies-2024.4.12/tests/utils_test/predbs_test/predbs_multi_test.py
+-rw-------   0 ich       (1000) ich       (1000)     1900 2024-01-26 16:22:52.000000 upsies-2024.4.12/tests/utils_test/predbs_test/predbs_test.py
+-rw-------   0 ich       (1000) ich       (1000)    22438 2024-01-26 16:22:52.000000 upsies-2024.4.12/tests/utils_test/predbs_test/srrdb_test.py
+-rw-------   0 ich       (1000) ich       (1000)     9604 2024-01-26 16:22:52.000000 upsies-2024.4.12/tests/utils_test/release_episodes_test.py
+-rw-------   0 ich       (1000) ich       (1000)    31672 2024-01-26 16:22:52.000000 upsies-2024.4.12/tests/utils_test/release_info_test.py
+-rw-------   0 ich       (1000) ich       (1000)    65135 2024-03-22 11:06:28.000000 upsies-2024.4.12/tests/utils_test/release_name_test.py
+-rw-------   0 ich       (1000) ich       (1000)     5791 2024-01-26 16:22:52.000000 upsies-2024.4.12/tests/utils_test/signal_test.py
+-rw-------   0 ich       (1000) ich       (1000)    10913 2024-01-26 16:22:52.000000 upsies-2024.4.12/tests/utils_test/string_test.py
+-rw-------   0 ich       (1000) ich       (1000)     2695 2024-01-26 16:22:52.000000 upsies-2024.4.12/tests/utils_test/subproc_test.py
+-rw-------   0 ich       (1000) ich       (1000)    10675 2024-02-16 17:01:10.000000 upsies-2024.4.12/tests/utils_test/subtitle_test.py
+-rw-------   0 ich       (1000) ich       (1000)     3156 2024-01-26 16:22:52.000000 upsies-2024.4.12/tests/utils_test/timestamp_test.py
+-rw-------   0 ich       (1000) ich       (1000)    30564 2024-02-08 15:57:50.000000 upsies-2024.4.12/tests/utils_test/torrent_test.py
+-rw-------   0 ich       (1000) ich       (1000)    22669 2024-02-13 10:51:19.000000 upsies-2024.4.12/tests/utils_test/types_test.py
+-rw-------   0 ich       (1000) ich       (1000)     5089 2024-01-26 16:22:52.000000 upsies-2024.4.12/tests/utils_test/update_test.py
+-rw-------   0 ich       (1000) ich       (1000)    17308 2024-03-12 15:18:06.000000 upsies-2024.4.12/tests/utils_test/utils_test.py
+-rw-------   0 ich       (1000) ich       (1000)    78592 2024-02-16 17:01:10.000000 upsies-2024.4.12/tests/utils_test/video_test.py
+drwx------   0 ich       (1000) ich       (1000)        0 2024-04-12 10:16:30.580498 upsies-2024.4.12/tests/utils_test/webdbs_test/
+-rw-------   0 ich       (1000) ich       (1000)     1423 2024-01-26 16:22:52.000000 upsies-2024.4.12/tests/utils_test/webdbs_test/conftest.py
+-rw-------   0 ich       (1000) ich       (1000)    32060 2024-02-24 18:36:30.000000 upsies-2024.4.12/tests/utils_test/webdbs_test/imdb_test.py
+-rw-------   0 ich       (1000) ich       (1000)    21744 2024-04-10 14:04:50.000000 upsies-2024.4.12/tests/utils_test/webdbs_test/tmdb_test.py
+-rw-------   0 ich       (1000) ich       (1000)    25024 2024-01-28 13:35:49.000000 upsies-2024.4.12/tests/utils_test/webdbs_test/tvmaze_test.py
+-rw-------   0 ich       (1000) ich       (1000)     6285 2024-02-24 18:36:30.000000 upsies-2024.4.12/tests/utils_test/webdbs_test/webdbs_base_test.py
+-rw-------   0 ich       (1000) ich       (1000)    20577 2024-04-10 14:04:50.000000 upsies-2024.4.12/tests/utils_test/webdbs_test/webdbs_common_test.py
+-rw-------   0 ich       (1000) ich       (1000)     1903 2024-01-26 16:22:52.000000 upsies-2024.4.12/tests/utils_test/webdbs_test/webdbs_test.py
+drwx------   0 ich       (1000) ich       (1000)        0 2024-04-12 10:16:30.584498 upsies-2024.4.12/upsies/
+-rw-------   0 ich       (1000) ich       (1000)     1194 2024-04-12 10:15:54.000000 upsies-2024.4.12/upsies/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)       73 2024-01-26 16:22:52.000000 upsies-2024.4.12/upsies/__main__.py
+-rw-------   0 ich       (1000) ich       (1000)     1527 2024-04-10 14:04:50.000000 upsies-2024.4.12/upsies/constants.py
+-rw-------   0 ich       (1000) ich       (1000)     2293 2024-04-09 08:10:30.000000 upsies-2024.4.12/upsies/defaults.py
+-rw-------   0 ich       (1000) ich       (1000)     6839 2024-03-06 10:16:46.000000 upsies-2024.4.12/upsies/errors.py
+drwx------   0 ich       (1000) ich       (1000)        0 2024-04-12 10:16:30.584498 upsies-2024.4.12/upsies/jobs/
+-rw-------   0 ich       (1000) ich       (1000)      215 2024-01-26 16:22:52.000000 upsies-2024.4.12/upsies/jobs/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)    37386 2024-03-06 10:16:46.000000 upsies-2024.4.12/upsies/jobs/base.py
+-rw-------   0 ich       (1000) ich       (1000)     2089 2024-02-22 11:14:53.000000 upsies-2024.4.12/upsies/jobs/custom.py
+-rw-------   0 ich       (1000) ich       (1000)    22530 2024-04-05 16:43:28.000000 upsies-2024.4.12/upsies/jobs/dialog.py
+-rw-------   0 ich       (1000) ich       (1000)     4996 2024-01-26 16:22:52.000000 upsies-2024.4.12/upsies/jobs/imghost.py
+-rw-------   0 ich       (1000) ich       (1000)     5303 2024-01-26 16:22:52.000000 upsies-2024.4.12/upsies/jobs/mediainfo.py
+-rw-------   0 ich       (1000) ich       (1000)    10222 2024-04-05 09:24:25.000000 upsies-2024.4.12/upsies/jobs/poster.py
+-rw-------   0 ich       (1000) ich       (1000)     9155 2024-03-14 10:33:57.000000 upsies-2024.4.12/upsies/jobs/scene.py
+-rw-------   0 ich       (1000) ich       (1000)    20453 2024-03-16 17:48:37.000000 upsies-2024.4.12/upsies/jobs/screenshots.py
+-rw-------   0 ich       (1000) ich       (1000)     3682 2024-02-13 10:51:19.000000 upsies-2024.4.12/upsies/jobs/set.py
+-rw-------   0 ich       (1000) ich       (1000)     7836 2024-04-08 11:12:16.000000 upsies-2024.4.12/upsies/jobs/submit.py
+-rw-------   0 ich       (1000) ich       (1000)    12774 2024-04-07 12:42:40.000000 upsies-2024.4.12/upsies/jobs/torrent.py
+-rw-------   0 ich       (1000) ich       (1000)    14641 2024-04-10 14:04:50.000000 upsies-2024.4.12/upsies/jobs/webdb.py
+drwx------   0 ich       (1000) ich       (1000)        0 2024-04-12 10:16:30.584498 upsies-2024.4.12/upsies/trackers/
+-rw-------   0 ich       (1000) ich       (1000)     1385 2024-01-26 16:22:52.000000 upsies-2024.4.12/upsies/trackers/__init__.py
+drwx------   0 ich       (1000) ich       (1000)        0 2024-04-12 10:16:30.584498 upsies-2024.4.12/upsies/trackers/ant/
+-rw-------   0 ich       (1000) ich       (1000)      119 2024-02-27 14:09:57.000000 upsies-2024.4.12/upsies/trackers/ant/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     1354 2024-04-07 12:42:40.000000 upsies-2024.4.12/upsies/trackers/ant/config.py
+-rw-------   0 ich       (1000) ich       (1000)     3600 2024-03-21 15:33:14.000000 upsies-2024.4.12/upsies/trackers/ant/jobs.py
+-rw-------   0 ich       (1000) ich       (1000)     4932 2024-04-07 12:42:40.000000 upsies-2024.4.12/upsies/trackers/ant/tracker.py
+drwx------   0 ich       (1000) ich       (1000)        0 2024-04-12 10:16:30.588498 upsies-2024.4.12/upsies/trackers/base/
+-rw-------   0 ich       (1000) ich       (1000)      149 2024-01-26 16:22:52.000000 upsies-2024.4.12/upsies/trackers/base/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     5888 2024-03-11 17:27:17.000000 upsies-2024.4.12/upsies/trackers/base/_howto.py
+-rw-------   0 ich       (1000) ich       (1000)     2940 2024-04-07 12:42:40.000000 upsies-2024.4.12/upsies/trackers/base/config.py
+-rw-------   0 ich       (1000) ich       (1000)     1191 2024-02-03 17:36:34.000000 upsies-2024.4.12/upsies/trackers/base/exclude.py
+-rw-------   0 ich       (1000) ich       (1000)    39139 2024-04-10 14:04:50.000000 upsies-2024.4.12/upsies/trackers/base/jobs.py
+-rw-------   0 ich       (1000) ich       (1000)     6972 2024-04-07 12:42:40.000000 upsies-2024.4.12/upsies/trackers/base/tracker.py
+drwx------   0 ich       (1000) ich       (1000)        0 2024-04-12 10:16:30.588498 upsies-2024.4.12/upsies/trackers/bhd/
+-rw-------   0 ich       (1000) ich       (1000)      119 2024-01-26 16:22:52.000000 upsies-2024.4.12/upsies/trackers/bhd/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     4714 2024-04-07 12:42:40.000000 upsies-2024.4.12/upsies/trackers/bhd/config.py
+-rw-------   0 ich       (1000) ich       (1000)    16191 2024-03-14 17:24:18.000000 upsies-2024.4.12/upsies/trackers/bhd/jobs.py
+-rw-------   0 ich       (1000) ich       (1000)     6302 2024-04-07 12:42:40.000000 upsies-2024.4.12/upsies/trackers/bhd/tracker.py
+-rw-------   0 ich       (1000) ich       (1000)     9725 2024-04-07 12:42:40.000000 upsies-2024.4.12/upsies/trackers/dummy.py
+drwx------   0 ich       (1000) ich       (1000)        0 2024-04-12 10:16:30.588498 upsies-2024.4.12/upsies/trackers/mtv/
+-rw-------   0 ich       (1000) ich       (1000)      119 2024-01-26 16:22:52.000000 upsies-2024.4.12/upsies/trackers/mtv/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     3298 2024-04-07 12:42:40.000000 upsies-2024.4.12/upsies/trackers/mtv/config.py
+-rw-------   0 ich       (1000) ich       (1000)    10358 2024-01-31 10:06:16.000000 upsies-2024.4.12/upsies/trackers/mtv/jobs.py
+-rw-------   0 ich       (1000) ich       (1000)    14491 2024-04-07 12:42:40.000000 upsies-2024.4.12/upsies/trackers/mtv/tracker.py
+drwx------   0 ich       (1000) ich       (1000)        0 2024-04-12 10:16:30.588498 upsies-2024.4.12/upsies/trackers/nbl/
+-rw-------   0 ich       (1000) ich       (1000)      119 2024-01-26 16:22:52.000000 upsies-2024.4.12/upsies/trackers/nbl/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     1034 2024-04-07 12:42:40.000000 upsies-2024.4.12/upsies/trackers/nbl/config.py
+-rw-------   0 ich       (1000) ich       (1000)     1801 2024-01-26 16:22:52.000000 upsies-2024.4.12/upsies/trackers/nbl/jobs.py
+-rw-------   0 ich       (1000) ich       (1000)     3912 2024-04-07 12:42:40.000000 upsies-2024.4.12/upsies/trackers/nbl/tracker.py
+drwx------   0 ich       (1000) ich       (1000)        0 2024-04-12 10:16:30.588498 upsies-2024.4.12/upsies/trackers/ptp/
+-rw-------   0 ich       (1000) ich       (1000)      119 2024-01-26 16:22:52.000000 upsies-2024.4.12/upsies/trackers/ptp/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     4898 2024-04-10 14:04:50.000000 upsies-2024.4.12/upsies/trackers/ptp/config.py
+-rw-------   0 ich       (1000) ich       (1000)    43959 2024-04-10 14:04:50.000000 upsies-2024.4.12/upsies/trackers/ptp/jobs.py
+-rw-------   0 ich       (1000) ich       (1000)     5386 2024-04-07 12:42:40.000000 upsies-2024.4.12/upsies/trackers/ptp/metadata.py
+-rw-------   0 ich       (1000) ich       (1000)    19532 2024-04-07 12:42:40.000000 upsies-2024.4.12/upsies/trackers/ptp/tracker.py
+drwx------   0 ich       (1000) ich       (1000)        0 2024-04-12 10:16:30.588498 upsies-2024.4.12/upsies/trackers/uhd/
+-rw-------   0 ich       (1000) ich       (1000)      119 2024-01-26 16:22:52.000000 upsies-2024.4.12/upsies/trackers/uhd/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     3281 2024-04-07 12:42:40.000000 upsies-2024.4.12/upsies/trackers/uhd/config.py
+-rw-------   0 ich       (1000) ich       (1000)    27037 2024-03-21 15:33:14.000000 upsies-2024.4.12/upsies/trackers/uhd/jobs.py
+-rw-------   0 ich       (1000) ich       (1000)     9291 2024-04-10 14:04:50.000000 upsies-2024.4.12/upsies/trackers/uhd/tracker.py
+drwx------   0 ich       (1000) ich       (1000)        0 2024-04-12 10:16:30.592498 upsies-2024.4.12/upsies/uis/
+-rw-------   0 ich       (1000) ich       (1000)      163 2024-02-20 15:50:34.000000 upsies-2024.4.12/upsies/uis/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     3560 2024-03-06 10:16:46.000000 upsies-2024.4.12/upsies/uis/prompts.py
+drwx------   0 ich       (1000) ich       (1000)        0 2024-04-12 10:16:30.592498 upsies-2024.4.12/upsies/uis/tui/
+-rw-------   0 ich       (1000) ich       (1000)       55 2024-01-26 16:22:52.000000 upsies-2024.4.12/upsies/uis/tui/__init__.py
+drwx------   0 ich       (1000) ich       (1000)        0 2024-04-12 10:16:30.592498 upsies-2024.4.12/upsies/uis/tui/commands/
+-rw-------   0 ich       (1000) ich       (1000)     1319 2024-01-26 16:22:52.000000 upsies-2024.4.12/upsies/uis/tui/commands/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)    15248 2024-03-18 15:05:12.000000 upsies-2024.4.12/upsies/uis/tui/commands/base.py
+-rw-------   0 ich       (1000) ich       (1000)     2279 2024-01-26 16:22:52.000000 upsies-2024.4.12/upsies/uis/tui/commands/mediainfo.py
+-rw-------   0 ich       (1000) ich       (1000)     4047 2024-04-08 16:39:10.000000 upsies-2024.4.12/upsies/uis/tui/commands/poster.py
+-rw-------   0 ich       (1000) ich       (1000)     2598 2024-04-08 16:39:06.000000 upsies-2024.4.12/upsies/uis/tui/commands/release_name.py
+-rw-------   0 ich       (1000) ich       (1000)     2710 2024-01-26 16:22:52.000000 upsies-2024.4.12/upsies/uis/tui/commands/scene.py
+-rw-------   0 ich       (1000) ich       (1000)     4710 2024-01-26 16:22:52.000000 upsies-2024.4.12/upsies/uis/tui/commands/screenshots.py
+-rw-------   0 ich       (1000) ich       (1000)     6117 2024-02-22 11:14:53.000000 upsies-2024.4.12/upsies/uis/tui/commands/set.py
+-rw-------   0 ich       (1000) ich       (1000)     8729 2024-04-08 16:39:02.000000 upsies-2024.4.12/upsies/uis/tui/commands/submit.py
+-rw-------   0 ich       (1000) ich       (1000)    10345 2024-02-12 13:49:50.000000 upsies-2024.4.12/upsies/uis/tui/commands/torrent.py
+-rw-------   0 ich       (1000) ich       (1000)     2091 2024-01-26 16:22:52.000000 upsies-2024.4.12/upsies/uis/tui/commands/upload_images.py
+-rw-------   0 ich       (1000) ich       (1000)     2038 2024-04-10 14:04:50.000000 upsies-2024.4.12/upsies/uis/tui/commands/webdb.py
+-rw-------   0 ich       (1000) ich       (1000)     2943 2024-01-26 16:22:52.000000 upsies-2024.4.12/upsies/uis/tui/headless.py
+drwx------   0 ich       (1000) ich       (1000)        0 2024-04-12 10:16:30.596498 upsies-2024.4.12/upsies/uis/tui/jobwidgets/
+-rw-------   0 ich       (1000) ich       (1000)      947 2024-01-26 16:22:52.000000 upsies-2024.4.12/upsies/uis/tui/jobwidgets/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)    10706 2024-03-08 13:58:19.000000 upsies-2024.4.12/upsies/uis/tui/jobwidgets/base.py
+-rw-------   0 ich       (1000) ich       (1000)      281 2024-01-26 16:22:52.000000 upsies-2024.4.12/upsies/uis/tui/jobwidgets/config.py
+-rw-------   0 ich       (1000) ich       (1000)     1156 2024-03-06 10:16:46.000000 upsies-2024.4.12/upsies/uis/tui/jobwidgets/custom.py
+-rw-------   0 ich       (1000) ich       (1000)     3257 2024-02-29 13:37:30.000000 upsies-2024.4.12/upsies/uis/tui/jobwidgets/dialog.py
+-rw-------   0 ich       (1000) ich       (1000)      796 2024-01-26 16:22:52.000000 upsies-2024.4.12/upsies/uis/tui/jobwidgets/imghost.py
+-rw-------   0 ich       (1000) ich       (1000)      234 2024-01-26 16:22:52.000000 upsies-2024.4.12/upsies/uis/tui/jobwidgets/mediainfo.py
+-rw-------   0 ich       (1000) ich       (1000)     1259 2024-02-20 15:50:34.000000 upsies-2024.4.12/upsies/uis/tui/jobwidgets/poster.py
+-rw-------   0 ich       (1000) ich       (1000)     4767 2024-04-07 12:42:40.000000 upsies-2024.4.12/upsies/uis/tui/jobwidgets/scene.py
+-rw-------   0 ich       (1000) ich       (1000)     1737 2024-01-26 16:22:52.000000 upsies-2024.4.12/upsies/uis/tui/jobwidgets/screenshots.py
+-rw-------   0 ich       (1000) ich       (1000)      715 2024-01-26 16:22:52.000000 upsies-2024.4.12/upsies/uis/tui/jobwidgets/submit.py
+-rw-------   0 ich       (1000) ich       (1000)     9132 2024-02-07 17:06:55.000000 upsies-2024.4.12/upsies/uis/tui/jobwidgets/torrent.py
+-rw-------   0 ich       (1000) ich       (1000)    13859 2024-02-26 09:50:52.000000 upsies-2024.4.12/upsies/uis/tui/jobwidgets/webdb.py
+-rw-------   0 ich       (1000) ich       (1000)     3009 2024-02-02 11:42:37.000000 upsies-2024.4.12/upsies/uis/tui/main.py
+-rw-------   0 ich       (1000) ich       (1000)     1402 2024-03-06 10:16:46.000000 upsies-2024.4.12/upsies/uis/tui/style.py
+-rw-------   0 ich       (1000) ich       (1000)    12653 2024-03-18 17:08:33.000000 upsies-2024.4.12/upsies/uis/tui/tui.py
+-rw-------   0 ich       (1000) ich       (1000)      626 2024-01-26 16:22:52.000000 upsies-2024.4.12/upsies/uis/tui/utils.py
+-rw-------   0 ich       (1000) ich       (1000)    17036 2024-03-06 10:16:46.000000 upsies-2024.4.12/upsies/uis/tui/widgets.py
+drwx------   0 ich       (1000) ich       (1000)        0 2024-04-12 10:16:30.600498 upsies-2024.4.12/upsies/utils/
+-rw-------   0 ich       (1000) ich       (1000)    13689 2024-03-12 15:18:06.000000 upsies-2024.4.12/upsies/utils/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     5982 2024-04-07 12:42:40.000000 upsies-2024.4.12/upsies/utils/argtypes.py
+-rw-------   0 ich       (1000) ich       (1000)      302 2024-01-26 16:22:52.000000 upsies-2024.4.12/upsies/utils/browser.py
+-rw-------   0 ich       (1000) ich       (1000)     5593 2024-03-17 12:11:58.000000 upsies-2024.4.12/upsies/utils/btclient.py
+-rw-------   0 ich       (1000) ich       (1000)    15585 2024-03-21 15:33:14.000000 upsies-2024.4.12/upsies/utils/configfiles.py
+-rw-------   0 ich       (1000) ich       (1000)     1825 2024-01-26 16:22:52.000000 upsies-2024.4.12/upsies/utils/country.py
+-rw-------   0 ich       (1000) ich       (1000)     7457 2024-01-26 16:22:52.000000 upsies-2024.4.12/upsies/utils/daemon.py
+-rw-------   0 ich       (1000) ich       (1000)    18714 2024-01-26 16:22:52.000000 upsies-2024.4.12/upsies/utils/fs.py
+-rw-------   0 ich       (1000) ich       (1000)     2749 2024-02-23 11:29:01.000000 upsies-2024.4.12/upsies/utils/html.py
+-rw-------   0 ich       (1000) ich       (1000)    24581 2024-04-12 10:12:23.000000 upsies-2024.4.12/upsies/utils/http.py
+-rw-------   0 ich       (1000) ich       (1000)    10667 2024-04-04 09:35:14.000000 upsies-2024.4.12/upsies/utils/image.py
+drwx------   0 ich       (1000) ich       (1000)        0 2024-04-12 10:16:30.600498 upsies-2024.4.12/upsies/utils/imghosts/
+-rw-------   0 ich       (1000) ich       (1000)     1391 2024-01-26 16:22:52.000000 upsies-2024.4.12/upsies/utils/imghosts/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     6802 2024-01-30 15:17:59.000000 upsies-2024.4.12/upsies/utils/imghosts/base.py
+-rw-------   0 ich       (1000) ich       (1000)     1147 2024-01-26 16:22:52.000000 upsies-2024.4.12/upsies/utils/imghosts/common.py
+-rw-------   0 ich       (1000) ich       (1000)      932 2024-01-26 16:22:52.000000 upsies-2024.4.12/upsies/utils/imghosts/dummy.py
+-rw-------   0 ich       (1000) ich       (1000)     1997 2024-01-26 16:22:52.000000 upsies-2024.4.12/upsies/utils/imghosts/freeimage.py
+-rw-------   0 ich       (1000) ich       (1000)     2459 2024-01-26 16:22:52.000000 upsies-2024.4.12/upsies/utils/imghosts/imgbb.py
+-rw-------   0 ich       (1000) ich       (1000)      912 2024-01-26 16:22:52.000000 upsies-2024.4.12/upsies/utils/imghosts/imgbox.py
+-rw-------   0 ich       (1000) ich       (1000)     3332 2024-01-26 16:22:52.000000 upsies-2024.4.12/upsies/utils/imghosts/ptpimg.py
+drwx------   0 ich       (1000) ich       (1000)        0 2024-04-12 10:16:30.600498 upsies-2024.4.12/upsies/utils/predbs/
+-rw-------   0 ich       (1000) ich       (1000)     1364 2024-01-26 16:22:52.000000 upsies-2024.4.12/upsies/utils/predbs/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     9619 2024-01-26 16:22:52.000000 upsies-2024.4.12/upsies/utils/predbs/base.py
+-rw-------   0 ich       (1000) ich       (1000)     4128 2024-04-11 13:58:01.000000 upsies-2024.4.12/upsies/utils/predbs/common.py
+-rw-------   0 ich       (1000) ich       (1000)     2278 2024-01-26 16:22:52.000000 upsies-2024.4.12/upsies/utils/predbs/corruptnet.py
+-rw-------   0 ich       (1000) ich       (1000)    20881 2024-01-30 14:38:02.000000 upsies-2024.4.12/upsies/utils/predbs/multi.py
+-rw-------   0 ich       (1000) ich       (1000)     2176 2024-01-26 16:22:52.000000 upsies-2024.4.12/upsies/utils/predbs/predbclub.py
+-rw-------   0 ich       (1000) ich       (1000)     2414 2024-01-26 16:22:52.000000 upsies-2024.4.12/upsies/utils/predbs/predbde.py
+-rw-------   0 ich       (1000) ich       (1000)     2169 2024-01-26 16:22:52.000000 upsies-2024.4.12/upsies/utils/predbs/predbovh.py
+-rw-------   0 ich       (1000) ich       (1000)     5425 2024-01-26 16:22:52.000000 upsies-2024.4.12/upsies/utils/predbs/query.py
+-rw-------   0 ich       (1000) ich       (1000)     6654 2024-01-26 16:22:52.000000 upsies-2024.4.12/upsies/utils/predbs/srrdb.py
+-rw-------   0 ich       (1000) ich       (1000)    56587 2024-03-22 11:06:28.000000 upsies-2024.4.12/upsies/utils/release.py
+-rw-------   0 ich       (1000) ich       (1000)     4366 2024-01-26 16:22:52.000000 upsies-2024.4.12/upsies/utils/signal.py
+-rw-------   0 ich       (1000) ich       (1000)     5154 2024-01-26 16:22:52.000000 upsies-2024.4.12/upsies/utils/string.py
+-rw-------   0 ich       (1000) ich       (1000)     1908 2024-01-26 16:22:52.000000 upsies-2024.4.12/upsies/utils/subproc.py
+-rw-------   0 ich       (1000) ich       (1000)     8297 2024-02-16 17:01:10.000000 upsies-2024.4.12/upsies/utils/subtitle.py
+-rw-------   0 ich       (1000) ich       (1000)     2034 2024-01-26 16:22:52.000000 upsies-2024.4.12/upsies/utils/timestamp.py
+-rw-------   0 ich       (1000) ich       (1000)    19817 2024-03-09 18:29:18.000000 upsies-2024.4.12/upsies/utils/torrent.py
+-rw-------   0 ich       (1000) ich       (1000)    16509 2024-02-13 10:51:19.000000 upsies-2024.4.12/upsies/utils/types.py
+-rw-------   0 ich       (1000) ich       (1000)     2927 2024-03-09 19:05:41.000000 upsies-2024.4.12/upsies/utils/update.py
+-rw-------   0 ich       (1000) ich       (1000)    37644 2024-04-10 13:57:11.000000 upsies-2024.4.12/upsies/utils/video.py
+drwx------   0 ich       (1000) ich       (1000)        0 2024-04-12 10:16:30.600498 upsies-2024.4.12/upsies/utils/webdbs/
+-rw-------   0 ich       (1000) ich       (1000)     1140 2024-01-26 16:22:52.000000 upsies-2024.4.12/upsies/utils/webdbs/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     9725 2024-02-24 18:36:30.000000 upsies-2024.4.12/upsies/utils/webdbs/base.py
+-rw-------   0 ich       (1000) ich       (1000)    13792 2024-04-10 14:04:50.000000 upsies-2024.4.12/upsies/utils/webdbs/common.py
+-rw-------   0 ich       (1000) ich       (1000)    13721 2024-04-12 09:26:32.000000 upsies-2024.4.12/upsies/utils/webdbs/imdb.py
+-rw-------   0 ich       (1000) ich       (1000)    12882 2024-04-10 14:04:50.000000 upsies-2024.4.12/upsies/utils/webdbs/tmdb.py
+-rw-------   0 ich       (1000) ich       (1000)     9826 2024-02-24 18:36:30.000000 upsies-2024.4.12/upsies/utils/webdbs/tvmaze.py
+drwx------   0 ich       (1000) ich       (1000)        0 2024-04-12 10:16:30.600498 upsies-2024.4.12/upsies.egg-info/
+-rw-r--r--   0 ich       (1000) ich       (1000)     4106 2024-04-12 10:16:30.000000 upsies-2024.4.12/upsies.egg-info/PKG-INFO
+-rw-------   0 ich       (1000) ich       (1000)     8176 2024-04-12 10:16:30.000000 upsies-2024.4.12/upsies.egg-info/SOURCES.txt
+-rw-------   0 ich       (1000) ich       (1000)        1 2024-04-12 10:16:30.000000 upsies-2024.4.12/upsies.egg-info/dependency_links.txt
+-rw-------   0 ich       (1000) ich       (1000)       47 2024-04-12 10:16:30.000000 upsies-2024.4.12/upsies.egg-info/entry_points.txt
+-rw-------   0 ich       (1000) ich       (1000)      388 2024-04-12 10:16:30.000000 upsies-2024.4.12/upsies.egg-info/requires.txt
+-rw-------   0 ich       (1000) ich       (1000)       64 2024-04-12 10:16:30.000000 upsies-2024.4.12/upsies.egg-info/top_level.txt
```

### Comparing `upsies-2024.3.9/LICENSE` & `upsies-2024.4.12/LICENSE`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/PKG-INFO` & `upsies-2024.4.12/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upsies
-Version: 2024.3.9
+Version: 2024.4.12
 Summary: Media metadata aggregator
 Author-email: plotski <plotski@example.org>
 License: GPL-3.0-or-later
 Project-URL: Repository, https://codeberg.org/plotski/upsies
 Project-URL: Documentation, https://upsies.readthedocs.io
 Project-URL: Bug Tracker, https://codeberg.org/plotski/upsies/issues
 Project-URL: Changelog, https://codeberg.org/plotski/upsies/raw/branch/master/NEWS
@@ -88,7 +88,24 @@
 * Do everything simultaneously
 
 ``upsies`` is developed on `Codeberg <https://codeberg.org/plotski/upsies>`_.
 
 The latest release is available on `PyPI <https://pypi.org/project/upsies>`_.
 
 Documentation is hosted on `Read the Docs <https://upsies.readthedocs.io/en/stable/>`_.
+
+Supported Trackers
+------------------
+
+* ANT
+* BHD
+* MTV
+* NBL
+* PTP
+* UHD
+
+Contact
+-------
+
+To report an issue or ask for a feature, please post in the upsies thread in the
+relevant tracker's forum. If you don't want to wait days for a response, you can
+leave a ping `here <https://codeberg.org/plotski/upsies/issues/9>`_.
```

### Comparing `upsies-2024.3.9/README.rst` & `upsies-2024.4.12/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -39,7 +39,24 @@
 * Do everything simultaneously
 
 ``upsies`` is developed on `Codeberg <https://codeberg.org/plotski/upsies>`_.
 
 The latest release is available on `PyPI <https://pypi.org/project/upsies>`_.
 
 Documentation is hosted on `Read the Docs <https://upsies.readthedocs.io/en/stable/>`_.
+
+Supported Trackers
+------------------
+
+* ANT
+* BHD
+* MTV
+* NBL
+* PTP
+* UHD
+
+Contact
+-------
+
+To report an issue or ask for a feature, please post in the upsies thread in the
+relevant tracker's forum. If you don't want to wait days for a response, you can
+leave a ping `here <https://codeberg.org/plotski/upsies/issues/9>`_.
```

### Comparing `upsies-2024.3.9/docs/_ext/cli_reference.py` & `upsies-2024.4.12/docs/_ext/cli_reference.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/docs/conf.py` & `upsies-2024.4.12/docs/conf.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/pyproject.toml` & `upsies-2024.4.12/pyproject.toml`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/conftest.py` & `upsies-2024.4.12/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/errors_test.py` & `upsies-2024.4.12/tests/errors_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/jobs_test/add_torrent_job_test.py` & `upsies-2024.4.12/tests/jobs_test/add_torrent_job_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/jobs_test/choice_job_test.py` & `upsies-2024.4.12/tests/jobs_test/choice_job_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/jobs_test/copy_torrent_job_test.py` & `upsies-2024.4.12/tests/jobs_test/copy_torrent_job_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/jobs_test/create_torrent_job_test.py` & `upsies-2024.4.12/tests/jobs_test/create_torrent_job_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 
 
 @pytest.fixture
 def tracker():
     tracker = Mock()
     tracker.configure_mock(
         name='AsdF',
+        torrent_source_field='ASDF',
         options={
-            'source': 'AsdF',
             'randomize_infohash': 'maybe randomize infohash',
             'exclude': ('a', 'b'),
         },
         login=AsyncMock(),
         get_announce_url=AsyncMock(),
         logout=AsyncMock(),
         calculate_piece_size_=Mock(name='calculate_piece_size'),
@@ -185,18 +185,18 @@
     job._start_torrent_process(announce_url)
     assert DaemonProcess_mock.call_args_list == [call(
         name=job.name,
         target=_torrent_process,
         kwargs={
             'content_path': 'path/to/foo',
             'announce': announce_url,
-            'source': job._tracker.options['source'],
+            'source': job._tracker.torrent_source_field,
             'torrent_path': os.path.join(
                 job.home_directory,
-                f'foo.{job._tracker.options["source"].lower()}.torrent',
+                f'foo.{job._tracker.name.lower()}.torrent',
             ),
             'exclude': job._exclude_files,
             'use_cache': not job.ignore_cache,
             'reuse_torrent_path': job._reuse_torrent_path,
             'randomize_infohash': job._tracker.options['randomize_infohash'],
             'piece_size_calculator': job._tracker.calculate_piece_size,
             'piece_size_min_max_calculator': job._tracker.calculate_piece_size_min_max,
```

### Comparing `upsies-2024.3.9/tests/jobs_test/custom_job_test.py` & `upsies-2024.4.12/tests/jobs_test/custom_job_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/jobs_test/imghost_job_test.py` & `upsies-2024.4.12/tests/jobs_test/imghost_job_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/jobs_test/job_base_test.py` & `upsies-2024.4.12/tests/jobs_test/job_base_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/jobs_test/mediainfo_job_test.py` & `upsies-2024.4.12/tests/jobs_test/mediainfo_job_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/jobs_test/poster_job_test.py` & `upsies-2024.4.12/tests/jobs_test/poster_job_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import hashlib
 import os
 import re
-from unittest.mock import AsyncMock, Mock, PropertyMock, call
+from unittest.mock import AsyncMock, Mock, PropertyMock, call, patch
 
 import pytest
 
 from upsies import errors
 from upsies.jobs.poster import PosterJob
 
 
@@ -316,118 +316,123 @@
             await job._obtain()
     else:
         return_value = await job._obtain()
         assert return_value == exp_result
     assert mocks.mock_calls == exp_mock_calls
 
 
-class MockPrompt:
-    _instances = {}
-
-    def __new__(cls, result):
-        if result in cls._instances:
-            return cls._instances[result]
-        else:
-            cls._instances[result] = self = super().__new__(cls)
-        return self
-
-    def __init__(self, result):
-        self.result = result
-        self.wait = AsyncMock()
+class UserInput(str):
+    """Awaitable `str` to mock `add_prompt` return value"""
+    def __await__(self):
+        async def await_():
+            return self
+        return await_().__await__()
 
     def __repr__(self):
-        return f'MockPrompt({self.result!r})'
+        return f'UserInput({str(self)!r})'
 
 @pytest.mark.parametrize(
-    argnames='prompts, responses, exp_return_value, exp_mock_calls',
+    argnames='inputs, responses, exp_return_value, exp_mock_calls',
     argvalues=(
         pytest.param(
-            (
-                MockPrompt(''),
-                MockPrompt('no/such/file.jpg'),
-                MockPrompt('existing_poster.jpg'),
-            ),
+            [
+                UserInput(''),
+                UserInput('no/such/file.jpg'),
+                UserInput('path/to/existing/directory'),
+                UserInput('existing_poster.jpg'),
+            ],
             (
             ),
             {'poster': 'existing_poster.jpg'},
             [
                 call.emit('info', 'Please enter a poster file or URL.'),
-                call.TextPrompt(),
-                call.add_prompt(MockPrompt('')),
-                call.prompt1_wait(),
+                call.TextPrompt(text=''),
+                call.add_prompt('<TextPrompt instance 1>'),
                 call.warn('Poster file or URL is required.'),
 
-                call.TextPrompt(),
-                call.add_prompt(MockPrompt('no/such/file.jpg')),
-                call.prompt2_wait(),
+                call.TextPrompt(text=UserInput('')),
+                call.add_prompt('<TextPrompt instance 2>'),
                 call.warn('Poster file does not exist: no/such/file.jpg'),
 
-                call.TextPrompt(),
-                call.add_prompt(MockPrompt('existing_poster.jpg')),
-                call.prompt3_wait(),
+                call.TextPrompt(text=UserInput('no/such/file.jpg')),
+                call.add_prompt('<TextPrompt instance 3>'),
+                call.warn('Poster is not a file: path/to/existing/directory'),
+
+                call.TextPrompt(text=UserInput('path/to/existing/directory')),
+                call.add_prompt('<TextPrompt instance 4>'),
 
                 call.clear_warnings(),
             ],
             id='File',
         ),
         pytest.param(
-            (
-                MockPrompt(''),
-                MockPrompt('http://foo.local/poster1.jpg'),
-                MockPrompt('http://bar.local/poster2.jpg'),
-            ),
+            [
+                UserInput(''),
+                UserInput('http://foo.local/poster1.jpg'),
+                UserInput('http://bar.local/poster2.jpg'),
+            ],
             (
                 errors.RequestError('No server response'),
                 '<ignored poster data>',
             ),
             {'poster': 'http://bar.local/poster2.jpg'},
             [
                 call.emit('info', 'Please enter a poster file or URL.'),
-                call.TextPrompt(),
-                call.add_prompt(MockPrompt('')),
-                call.prompt1_wait(),
+                call.TextPrompt(text=''),
+                call.add_prompt('<TextPrompt instance 1>'),
                 call.warn('Poster file or URL is required.'),
 
-                call.TextPrompt(),
-                call.add_prompt(MockPrompt('http://foo.local/poster1.jpg')),
-                call.prompt2_wait(),
-                call.http_get('http://foo.local/poster1.jpg', cache=True),
+                call.TextPrompt(text=UserInput('')),
+                call.add_prompt('<TextPrompt instance 2>'),
+                call.http_get(UserInput('http://foo.local/poster1.jpg'), cache=True),
                 call.warn('Failed to download poster: No server response'),
 
-                call.TextPrompt(),
-                call.add_prompt(MockPrompt('http://bar.local/poster2.jpg')),
-                call.prompt3_wait(),
-                call.http_get('http://bar.local/poster2.jpg', cache=True),
+                call.TextPrompt(text=UserInput('http://foo.local/poster1.jpg')),
+                call.add_prompt('<TextPrompt instance 3>'),
+                call.http_get(UserInput('http://bar.local/poster2.jpg'), cache=True),
 
                 call.clear_warnings(),
             ],
             id='URL',
         ),
     ),
     ids=lambda v: repr(v),
 )
 @pytest.mark.asyncio
-async def test__obtain_via_prompt(prompts, responses, exp_return_value, exp_mock_calls, job, mocker, tmp_path):
+async def test__obtain_via_prompt(inputs, responses, exp_return_value, exp_mock_calls, job, mocker, tmp_path):
     existing_poster_file = tmp_path / 'existing_poster.jpg'
     existing_poster_file.write_bytes(b'poster data')
+
     orig_cwd = os.getcwd()
     os.chdir(tmp_path)
     try:
-
         mocks = Mock()
-        mocks.attach_mock(mocker.patch('upsies.uis.prompts.TextPrompt', side_effect=prompts), 'TextPrompt')
-        for i, prompt in enumerate(prompts, start=1):
-            mocks.attach_mock(prompt.wait, f'prompt{i}_wait')
+
+        def TextPrompt(*args, i=[0], **kwargs):
+            i[0] += 1
+            return f'<TextPrompt instance {i[0]}>'
+
+        mocks.attach_mock(mocker.patch('upsies.uis.prompts.TextPrompt', side_effect=TextPrompt), 'TextPrompt')
+
         mocks.attach_mock(mocker.patch('upsies.utils.http.get', side_effect=responses), 'http_get')
-        mocks.attach_mock(mocker.patch.object(job, 'add_prompt'), 'add_prompt')
+        mocks.attach_mock(mocker.patch.object(job, 'add_prompt', side_effect=inputs), 'add_prompt')
         mocks.attach_mock(mocker.patch.object(job.signal, 'emit'), 'emit')
         mocks.attach_mock(mocker.patch.object(job, 'warn'), 'warn')
         mocks.attach_mock(mocker.patch.object(job, 'clear_warnings'), 'clear_warnings')
 
-        return_value = await job._obtain_via_prompt()
+        def path_exists(path):
+            return 'existing' in path
+
+        def path_isfile(path):
+            return 'directory' not in path
+
+        with patch('os.path.exists', path_exists):
+            with patch('os.path.isfile', path_isfile):
+                return_value = await job._obtain_via_prompt()
+
         assert return_value == exp_return_value
         assert mocks.mock_calls == exp_mock_calls
     finally:
         os.chdir(orig_cwd)
 
 
 @pytest.mark.parametrize(
```

### Comparing `upsies-2024.3.9/tests/jobs_test/queue_job_base_test.py` & `upsies-2024.4.12/tests/jobs_test/queue_job_base_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/jobs_test/scene_check_job_test.py` & `upsies-2024.4.12/tests/jobs_test/scene_check_job_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/jobs_test/scene_search_job_test.py` & `upsies-2024.4.12/tests/jobs_test/scene_search_job_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/jobs_test/screenshots_job_test.py` & `upsies-2024.4.12/tests/jobs_test/screenshots_job_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -519,14 +519,45 @@
             args['output_queue'],
             content_path=args['content_path'],
             exclude_files=args['exclude_files'],
         ),
         call.output_queue_put((MsgType.error, 'No videos found')),
     ]
 
+def test__screenshots_process__mapping_timestamps_fails(screenshots_process_mocks):
+    args, mocks = screenshots_process_mocks
+    mocks._get_video_files.return_value = ['foo.mkv']
+    mocks._map_timestamps.side_effect = errors.ContentError('Video duration is too short: -1s')
+
+    return_value = screenshots._screenshots_process(
+        args['output_queue'], args['input_queue'],
+        content_path=args['content_path'],
+        exclude_files=args['exclude_files'],
+        timestamps=args['timestamps'],
+        count=args['count'],
+        from_all_videos=args['from_all_videos'],
+        output_dir=args['output_dir'],
+        overwrite=args['overwrite'],
+    )
+    assert return_value is None
+
+    assert mocks.mock_calls == [
+        call._get_video_files(
+            args['output_queue'],
+            content_path=args['content_path'],
+            exclude_files=args['exclude_files'],
+        ),
+        call._map_timestamps(
+            video_files=['foo.mkv'],
+            timestamps=args['timestamps'],
+            count=args['count'],
+        ),
+        call.output_queue_put((MsgType.error, 'Video duration is too short: -1s')),
+    ]
+
 @pytest.mark.parametrize('termination_indicated', (False, True), ids=['not terminated', 'terminated'])
 @pytest.mark.parametrize('from_all_videos', (False, True), ids=['from_first_video', 'from_all_videos'])
 def test__screenshots_process(from_all_videos, termination_indicated, screenshots_process_mocks):
     args, mocks = screenshots_process_mocks
     args['from_all_videos'] = from_all_videos
     mocks._get_video_files.return_value = ('foo.mkv', 'bar.mp4', 'baz.web')
     mocks._map_timestamps.return_value = {
@@ -872,59 +903,73 @@
             count=count,
         )
         for video_file in video_files
     ]
 
 
 @pytest.mark.parametrize(
-    argnames='duration, count, timestamps, exp_timestamps',
+    argnames='duration, count, timestamps, exp_result',
     argvalues=(
-        # Invalid duration
-        (-1, 0, [], []),
-        (0, 0, [], []),
-        (1, 0, [], []),
-        (59, 0, [], []),
-        (70, 0, [], ['0:00:30', '0:00:45']),
-        # Default
-        (300, 0, [], ['0:02:25', '0:03:37']),
-        # Specific count
-        (300, 1, [], ['0:02:25']),
-        (300, 2, [], ['0:02:25', '0:03:37']),
-        (300, 3, [], ['0:01:12', '0:02:25', '0:03:37']),
-        (300, 4, [], ['0:01:12', '0:02:25', '0:03:37', '0:04:13']),
-        # Specific timestamps
+        # Duration too short
+        (-1, 0, [], errors.ContentError('Video duration is too short: -1s')),
+        (0, 0, [], errors.ContentError('Video duration is too short: 0s')),
+        # Invalid custom timestamp
+        (60, 0, [20, 'foo', '0:00:30'], errors.ContentError("Invalid timestamp: 'foo'")),
+        # Very short duration
+        (1, 0, [], ['0:00:00']),
+        (9, 0, [], ['0:00:04', '0:00:06']),
+        (9, 3, [], ['0:00:02', '0:00:04', '0:00:06']),
+        (9, 12, [], ['0:00:01', '0:00:02', '0:00:03', '0:00:04', '0:00:05', '0:00:06', '0:00:07', '0:00:08']),
+        (60, 0, [], ['0:00:30', '0:00:45']),
+        (60, 3, [], ['0:00:15', '0:00:30', '0:00:45']),
+        (60, 6, [], ['0:00:15', '0:00:22', '0:00:30', '0:00:37', '0:00:45', '0:00:52']),
+        # Normal duration with specific count
+        (300, 1, [], ['0:02:30']),
+        (300, 2, [], ['0:02:30', '0:03:45']),
+        (300, 3, [], ['0:01:15', '0:02:30', '0:03:45']),
+        (300, 4, [], ['0:01:15', '0:02:30', '0:03:45', '0:04:22']),
+        # Normal duration with specific timestamps
         (300, 0, [60], ['0:01:00']),
         (300, 0, [60, 60], ['0:01:00']),
         (300, 0, [60, '180'], ['0:01:00', '0:03:00']),
         (300, 0, [60, '180', '0:181'], ['0:01:00', '0:03:00', '0:03:01']),
-        (300, 0, [60, '180', '002:01:181'], ['0:01:00', '0:03:00', '0:04:50']),
+        (300, 0, [60, '180', '002:01:181'], ['0:01:00', '0:03:00', '0:05:00']),
         (86400, 0, [60, '180', '002:01:181'], ['0:01:00', '0:03:00', '2:04:01']),
-        # Specific timestamps and specific count
-        (300, 3, [0], ['0:00:00', '0:02:25', '0:03:37']),
-        (300, 3, [300], ['0:02:25', '0:03:37', '0:04:50']),
-        (300, 3, [0, 301], ['0:00:00', '0:02:25', '0:04:50']),
+        # Normal duration with specific timestamps and specific count
+        (300, 3, [0], ['0:00:00', '0:02:30', '0:03:45']),
+        (300, 3, [300], ['0:02:30', '0:03:45', '0:05:00']),
+        (300, 3, [0, 301], ['0:00:00', '0:02:30', '0:05:00']),
         (300, 1, [60], ['0:01:00']),
-        (300, 2, [60], ['0:01:00', '0:02:55']),
-        (300, 3, [60], ['0:01:00', '0:02:55', '0:03:52']),
-        (300, 3, [60, 180], ['0:01:00', '0:02:00', '0:03:00']),
+        (300, 2, [60], ['0:01:00', '0:03:00']),
+        (300, 3, [60], ['0:01:00', '0:02:00', '0:03:00']),
+        (300, 3, [60, 180], ['0:01:00', '0:03:00', '0:04:00']),
         # Timestamps are returned sorted
         (300, 3, [60, 180, 120, 90], ['0:01:00', '0:01:30', '0:02:00', '0:03:00']),
         # Timestamps are deduplicated
-        (300, 4, [60, '0:60', 90, '1:00'], ['0:01:00', '0:01:30', '0:03:10', '0:04:00']),
+        (300, 4, [60, '0:60', 90, '1:00'], ['0:01:00', '0:01:30', '0:03:14', '0:04:07']),
     ),
     ids=lambda v: repr(v),
 )
-def test__validate_timestamps(duration, count, timestamps, exp_timestamps, mocker):
+def test__validate_timestamps(duration, count, timestamps, exp_result, mocker):
     duration_mock = mocker.patch('upsies.utils.video.duration', return_value=duration)
-    return_value = screenshots._validate_timestamps(
-        video_file='foo.mkv',
-        timestamps=timestamps,
-        count=count,
-    )
-    assert return_value == exp_timestamps
+
+    if isinstance(exp_result, Exception):
+        with pytest.raises(type(exp_result), match=rf'^{re.escape(str(exp_result))}$'):
+            screenshots._validate_timestamps(
+                video_file='foo.mkv',
+                timestamps=timestamps,
+                count=count,
+            )
+    else:
+        return_value = screenshots._validate_timestamps(
+            video_file='foo.mkv',
+            timestamps=timestamps,
+            count=count,
+        )
+        assert return_value == exp_result
     assert duration_mock.call_args_list == [call('foo.mkv')]
 
 
 @pytest.mark.parametrize(
     argnames='get_nowait, exp_exception',
     argvalues=(
         (
```

### Comparing `upsies-2024.3.9/tests/jobs_test/set_job_test.py` & `upsies-2024.4.12/tests/jobs_test/set_job_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/jobs_test/submit_job_test.py` & `upsies-2024.4.12/tests/jobs_test/submit_job_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
 
 @pytest.fixture
 def tracker():
     class TestTracker(TrackerBase):
         name = 'test'
         label = 'TeST'
+        torrent_source_field = 'TEST'
         TrackerConfig = 'tracker config class'
         TrackerJobs = 'tracker jobs class'
         login = AsyncMock()
         logout = AsyncMock()
         _login = AsyncMock()
         _logout = AsyncMock()
         is_logged_in = PropertyMock()
```

### Comparing `upsies-2024.3.9/tests/jobs_test/text_field_job_test.py` & `upsies-2024.4.12/tests/jobs_test/text_field_job_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/jobs_test/webdb_search_job_test.py` & `upsies-2024.4.12/tests/jobs_test/webdb_search_job_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -79,14 +79,30 @@
 )
 def test_WebDbSearchJob_no_id_ok(value, exp_value, job):
     assert job.no_id_ok is False
     job.no_id_ok = value
     assert job.no_id_ok is exp_value
 
 
+@pytest.mark.parametrize(
+    argnames='value, exp_value',
+    argvalues=(
+        (True, True),
+        (False, False),
+        (None, False),
+        (1, True),
+    ),
+)
+def test_WebDbSearchJob_show_poster(value, exp_value, job):
+    assert job.show_poster is True
+    job.show_poster = value
+    assert job.show_poster is exp_value
+    assert job._get_show_poster() is exp_value
+
+
 def test_WebDbSearchJob_is_searching(job, mocker):
     mocker.patch.object(job, '_is_searching', object())
     assert job.is_searching is job._is_searching
 
 
 @pytest.mark.parametrize(
     argnames='query, exp_from_any_called',
@@ -236,30 +252,49 @@
         call('summary'),
         call('title_original'),
         call('title_english'),
         call('genres'),
         call('directors'),
         call('cast'),
         call('countries'),
-        call('poster'),
+        call('poster', condition=job._get_show_poster),
     ]
 
 
-def test_WebDbSearchJob__make_update_info_func(job, mocker):
+@pytest.mark.parametrize(
+    argnames='condition, exp_info_updated',
+    argvalues=(
+        (None, True),
+        (Mock(return_value=True), True),
+        (Mock(return_value=False), False),
+    ),
+)
+def test_WebDbSearchJob__make_update_info_func(condition, exp_info_updated, job, mocker):
     mocker.patch.object(job, '_update_info_value')
-    func = job._make_update_info_func('my key')
+    if condition is None:
+        func = job._make_update_info_func('my key')
+    else:
+        func = job._make_update_info_func('my key', condition=condition)
+
     func('value 1')
-    assert job._update_info_value.call_args_list == [
-        call('my key', 'value 1'),
-    ]
+    if exp_info_updated:
+        assert job._update_info_value.call_args_list == [
+            call('my key', 'value 1'),
+        ]
+    else:
+        assert job._update_info_value.call_args_list == []
+
     func('value 2')
-    assert job._update_info_value.call_args_list == [
-        call('my key', 'value 1'),
-        call('my key', 'value 2'),
-    ]
+    if exp_info_updated:
+        assert job._update_info_value.call_args_list == [
+            call('my key', 'value 1'),
+            call('my key', 'value 2'),
+        ]
+    else:
+        assert job._update_info_value.call_args_list == []
 
 
 def test_WebDbSearchJob__update_info_value(job):
     mocks = Mock()
     job.signal.register('info_updating', mocks.info_updating)
     job.signal.register('info_updated', mocks.info_updated)
 
@@ -298,50 +333,69 @@
 
     assert mocks.mock_calls == [
         call.search(job.query),
         call.finalization(),
     ]
 
 
-@pytest.mark.parametrize('results', ((), ('foo', 'bar', 'baz')), ids=('results found', 'no results found'))
+@pytest.mark.parametrize('results', ((), ('foo',), ('foo', 'bar', 'baz')), ids=('no results', 'one result', 'multiple results'))
+@pytest.mark.parametrize('feeling_lucky', (False, True), ids=('feeling lucky', 'not feeling lucky'))
 @pytest.mark.asyncio
-async def test_WebDbSearchJob__search_calls_search_and__run_info_callbacks(results, job, mocker):
+async def test_WebDbSearchJob__search_calls_search_and__run_info_callbacks(results, feeling_lucky, job, mocker):
     mocks = Mock()
     mocks.attach_mock(mocker.patch.object(job, '_set_state'), '_set_state')
     mocks.attach_mock(mocker.patch.object(job._db, 'search', return_value=results), 'search')
     mocks.attach_mock(mocker.patch.object(job, '_run_info_callbacks'), '_run_info_callbacks')
+    mocks.attach_mock(mocker.patch.object(job, 'result_selected'), 'result_selected')
     mocks.attach_mock(mocker.patch.object(job, 'warn'), 'warn')
 
-    await job._search('mock query')
+    query = Mock(feeling_lucky=feeling_lucky)
 
-    assert mocks.mock_calls == [
+    await job._search(query)
+
+    exp_mock_calls = [
         call._set_state(is_searching=True, results=()),
-        call.search('mock query'),
+        call.search(query),
         call._set_state(is_searching=False, results=results),
-        call._run_info_callbacks(results[0] if results else None),
-        call._set_state(is_searching=False),
     ]
 
+    if len(results) == 1 and feeling_lucky:
+        exp_mock_calls.append(call.result_selected(results[0]))
+    elif results:
+        exp_mock_calls.append(call._run_info_callbacks(results[0]))
+    else:
+        exp_mock_calls.append(call._run_info_callbacks(None)),
+    exp_mock_calls.append(call._set_state(is_searching=False))
+    for a, b in zip(mocks.mock_calls, exp_mock_calls):
+        print(a, b)
+    assert mocks.mock_calls == exp_mock_calls
+
 
 @pytest.mark.asyncio
 async def test_WebDbSearchJob__search_catches_exception_from_search(job, mocker):
     mocks = Mock()
     mocks.attach_mock(mocker.patch.object(job, '_set_state'), '_set_state')
     mocks.attach_mock(mocker.patch.object(job._db, 'search', side_effect=errors.RequestError('network error')), 'search')
     mocks.attach_mock(mocker.patch.object(job, '_run_info_callbacks'), '_run_info_callbacks')
+    mocks.attach_mock(mocker.patch.object(job, 'result_selected'), 'result_selected')
     mocks.attach_mock(mocker.patch.object(job, 'warn'), 'warn')
 
     await job._search('mock query')
 
-    assert mocks.mock_calls == [
+    mocks.attach_mock(mocker.patch.object(job, 'result_selected'), 'result_selected')
+
+    exp_mock_calls = [
         call._set_state(is_searching=True, results=()),
         call.search('mock query'),
         call.warn(errors.RequestError('network error')),
         call._set_state(is_searching=False),
     ]
+    for a, b in zip(mocks.mock_calls, exp_mock_calls):
+        print(a, b)
+    assert mocks.mock_calls == exp_mock_calls
 
 
 @pytest.mark.parametrize(
     argnames='kwargs, exp_attrs, exp_emit_calls',
     argvalues=(
         ({}, {}, []),
         (
```

### Comparing `upsies-2024.3.9/tests/trackers_test/ant/ant_tracker_config_test.py` & `upsies-2024.4.12/tests/trackers_test/ant/ant_tracker_config_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 
 
 def test_AntTrackerConfig_defaults(tracker_config):
     assert set(tracker_config) == {
         'base_url',
         'apikey',
         'announce_url',
-        'source',
         'exclude',
+        'anonymous',
 
         # Inherited from TrackerConfigBase
         'add_to',
         'copy_to',
         'randomize_infohash',
     }
 
@@ -41,28 +41,42 @@
 def test_AntTrackerConfig_defaults_announce_url(tracker_config):
     assert tracker_config['announce_url'] == ''
     assert tracker_config['announce_url'].description == (
         'Your personal announce URL.'
     )
 
 
-def test_AntTrackerConfig_defaults_source(tracker_config):
-    assert tracker_config['source'] == 'ANT'
-
-
 def test_AntTrackerConfig_defaults_exclude(tracker_config):
     assert tracker_config['exclude'] == (
         utils.types.RegEx(base.exclude.checksums),
         utils.types.RegEx(base.exclude.images),
         utils.types.RegEx(base.exclude.nfo),
         utils.types.RegEx(base.exclude.samples),
     )
 
 
+def test_AntTrackerConfig_defaults_anonymous(tracker_config):
+    assert isinstance(tracker_config['anonymous'], utils.types.Bool)
+    assert not tracker_config['anonymous']
+    assert tracker_config['anonymous'] == 'no'
+    assert tracker_config['anonymous'].description == (
+        'Whether your username is displayed on your uploads.'
+    )
+
+
 def test_AntTrackerConfig_arguments(tracker_config):
     exp_argument_definitions = {
-        'submit': set(
-        ),
+        'submit': {
+            ('--anonymous', '--an'),
+        },
     }
     assert set(tracker_config.argument_definitions) == set(exp_argument_definitions)
     for command in exp_argument_definitions:
         assert set(tracker_config.argument_definitions[command]) == exp_argument_definitions[command]
+
+
+def test_AntTrackerConfig_argument_definitions_submit_anonymous(tracker_config):
+    assert tracker_config.argument_definitions['submit'][('--anonymous', '--an')] == {
+        'help': 'Hide your username for this submission',
+        'action': 'store_true',
+        'default': None,
+    }
```

### Comparing `upsies-2024.3.9/tests/trackers_test/ant/ant_tracker_jobs_test.py` & `upsies-2024.4.12/tests/trackers_test/ant/ant_tracker_jobs_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -135,39 +135,85 @@
     mocker.patch('upsies.utils.video.hdr_formats', return_value=attrs.get('hdr_formats', ()))
     mocker.patch('upsies.utils.video.has_commentary', return_value=attrs.get('has_commentary', False))
 
     return_value = await ant_tracker_jobs.autodetect_flags('job_')
     assert return_value == exp_flags
 
 
-async def test_post_data(ant_tracker_jobs, mocker):
+@pytest.mark.parametrize('anonymous, exp_anonymous_post_data', (
+    (None, {'anonymous': None}),
+    (False, {'anonymous': None}),
+    (True, {'anonymous': '1'}),
+))
+@pytest.mark.parametrize('is_scene, exp_is_scene_post_data', (
+    (False, {'censored': None}),
+    (True, {'censored': '1'}),
+))
+async def test_post_data(
+        anonymous, exp_anonymous_post_data,
+        is_scene, exp_is_scene_post_data,
+        ant_tracker_jobs, mocker,
+):
     mocker.patch.object(type(ant_tracker_jobs), 'tmdb_job', PropertyMock())
     mocker.patch.object(type(ant_tracker_jobs), 'mediainfo_job', PropertyMock())
     mocker.patch.object(type(ant_tracker_jobs), 'flags_job', PropertyMock())
+    mocker.patch.object(type(ant_tracker_jobs), 'scene_check_job', PropertyMock())
+    mocker.patch.object(type(ant_tracker_jobs), '_post_data_release_group', PropertyMock(return_value={
+        'release_group': 'info',
+    }))
     mocker.patch.object(ant_tracker_jobs, '_tracker', Mock(
         apikey='d34db33f',
     ))
     mocker.patch.object(ant_tracker_jobs, 'get_job_output', side_effect=(
         'movie/123456',
         '[mediainfo]',
         ('Uncut', 'Commentary'),
     ))
+    mocker.patch.object(ant_tracker_jobs, 'get_job_attribute', side_effect=(
+        is_scene,
+    ))
+    options = {}
+    if anonymous is not None:
+        options['anonymous'] = anonymous
+    mocker.patch.object(type(ant_tracker_jobs), 'options', PropertyMock(return_value=options))
 
-    assert ant_tracker_jobs.post_data == {
+    exp_post_data = {
         'api_key': 'd34db33f',
         'action': 'upload',
         'tmdbid': '123456',
         'mediainfo': '[mediainfo]',
         'flags[]': ('Uncut', 'Commentary'),
+        'release_group': 'info',
     }
+    exp_post_data.update(exp_is_scene_post_data)
+    exp_post_data.update(exp_anonymous_post_data)
+
+    assert ant_tracker_jobs.post_data == exp_post_data
     assert ant_tracker_jobs.get_job_output.call_args_list == [
         call(ant_tracker_jobs.tmdb_job, slice=0),
         call(ant_tracker_jobs.mediainfo_job, slice=0),
         call(ant_tracker_jobs.flags_job),
     ]
+    assert ant_tracker_jobs.get_job_attribute.call_args_list == [
+        call(ant_tracker_jobs.scene_check_job, 'is_scene_release'),
+    ]
+
+
+@pytest.mark.parametrize(
+    argnames='group, exp_return_value',
+    argvalues=(
+        ('NOGROUP', {'noreleasegroup': 'on'}),
+        ('ASDF', {'releasegroup': 'ASDF'}),
+    ),
+    ids=lambda v: repr(v),
+)
+async def test__post_data_release_group(group, exp_return_value, ant_tracker_jobs, mocker):
+    mocker.patch.object(type(ant_tracker_jobs), 'release_name', PropertyMock(return_value=Mock(group=group)))
+
+    assert ant_tracker_jobs._post_data_release_group == exp_return_value
 
 
 async def test_post_files(ant_tracker_jobs, mocker):
     mocker.patch.object(type(ant_tracker_jobs), 'torrent_filepath', PropertyMock(
         return_value='path/to/torrent',
     ))
```

### Comparing `upsies-2024.3.9/tests/trackers_test/ant/ant_tracker_test.py` & `upsies-2024.4.12/tests/trackers_test/ant/ant_tracker_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,18 @@
     assert AntTracker.name == 'ant'
 
 
 def test_label_attribute():
     assert AntTracker.label == 'ANT'
 
 
+def test_torrent_source_field_attribute():
+    assert AntTracker.torrent_source_field == 'ANT'
+
+
 def test_TrackerConfig_attribute():
     assert AntTracker.TrackerConfig is AntTrackerConfig
 
 
 def test_TrackerJobs_attribute():
     assert AntTracker.TrackerJobs is AntTrackerJobs
```

### Comparing `upsies-2024.3.9/tests/trackers_test/base/tracker_base_exclude_test.py` & `upsies-2024.4.12/tests/trackers_test/base/tracker_base_exclude_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/trackers_test/base/tracker_base_howto_test.py` & `upsies-2024.4.12/tests/trackers_test/base/tracker_base_howto_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         'N. How To Read This Howto\n'
         '\n'
         '   C.1 Words in ALL_CAPS_AND_WITH_UNDERSCORES are placeholders.\n'
         '   CC.2 Everything after "$" is a terminal command.\n'
         '\n'
         'NN. Configuration Defaults (Optional)\n'
         '\n'
-        '    If you prefer, you can write all default values at once and then edit \n'
+        '    If you prefer, you can write all default values at once and then edit\n'
         '    them in your favorite $EDITOR.\n'
         '\n'
         f'    $ {__project_name__} set --dump\n'
         f'    $ $EDITOR ~/.conf/trackers.ini\n'
         f'    $ $EDITOR ~/.conf/imghosts.ini\n'
         f'    $ $EDITOR ~/.conf/clients.ini\n'
         f'    $ $EDITOR ~/.conf/config.ini'
```

### Comparing `upsies-2024.3.9/tests/trackers_test/base/tracker_base_test.py` & `upsies-2024.4.12/tests/trackers_test/base/tracker_base_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from upsies.trackers import base
 
 
 def make_MockTracker(**kwargs):
     class MockTracker(base.TrackerBase):
         name = 'asdf'
         label = 'AsdF'
+        torrent_source_field = '->!!!ASDF!!!<-'
         TrackerJobs = PropertyMock()
         TrackerConfig = PropertyMock()
         _login = AsyncMock()
         _logout = AsyncMock()
         get_announce_url = AsyncMock()
         upload = AsyncMock()
```

### Comparing `upsies-2024.3.9/tests/trackers_test/base/tracker_config_base_test.py` & `upsies-2024.4.12/tests/trackers_test/base/tracker_config_base_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -58,33 +58,14 @@
     assert isinstance(config['ratio'], float)
     assert isinstance(config['my_list'], list)
 
 
 @pytest.mark.parametrize(
     argnames='defaults, userconfig, exp_value',
     argvalues=(
-        ({}, {}, ''),
-        ({'source': 'FOO'}, {}, 'FOO'),
-        ({'source': 'FOO'}, {'source': ''}, ''),
-        ({'source': 'FOO'}, {'source': 'BAR'}, 'BAR'),
-    ),
-    ids=lambda v: repr(v),
-)
-def test_source_value(defaults, userconfig, exp_value, make_tracker_config):
-    config = make_tracker_config(defaults=defaults, userconfig=userconfig)
-    assert config['source'] == exp_value
-
-def test_source_description(make_tracker_config):
-    config = make_tracker_config()
-    assert config['source'].description == 'Value of the "source" field in generated torrents.'
-
-
-@pytest.mark.parametrize(
-    argnames='defaults, userconfig, exp_value',
-    argvalues=(
         ({}, {}, False),
         ({'randomize_infohash': 'yes'}, {}, True),
         ({'randomize_infohash': 'false'}, {}, False),
         ({'randomize_infohash': 'true'}, {'randomize_infohash': 'false'}, False),
         ({'randomize_infohash': 'no'}, {'randomize_infohash': 'true'}, True),
     ),
     ids=lambda v: repr(v),
```

### Comparing `upsies-2024.3.9/tests/trackers_test/base/tracker_jobs_base_test.py` & `upsies-2024.4.12/tests/trackers_test/base/tracker_jobs_base_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
             'content_path': '',
             'tracker': tracker,
             'reuse_torrent_path': '',
             'btclient': Mock(),
             'torrent_destination': '',
             'image_hosts': (Mock(),),
             'screenshots_optimization': 'my optimization level',
+            'show_poster': 'maybe show poster',
             'common_job_args': {},
         }
         return TestTrackerJobs(**{**default_kwargs, **kwargs})
 
     return make_TestTrackerJobs
 
 
@@ -62,22 +63,39 @@
         assert getattr(tracker_jobs, k) is v
 
 
 @pytest.mark.parametrize(
     argnames='common_job_args, overload, exp_return_value',
     argvalues=(
         (
-            {'home_directory': 'initial/path', 'ignore_cache': 'mock bool'},
-            {'home_directory': 'overloaded/path'},
-            {'home_directory': 'overloaded/path', 'ignore_cache': 'mock bool'},
+            {'home_directory': 'default/home', 'cache_directory': 'default/cache', 'ignore_cache': False},
+            {'home_directory': 'overloaded/home'},
+            {'home_directory': 'overloaded/home', 'cache_directory': 'default/cache', 'ignore_cache': False},
         ),
         (
-            {'home_directory': 'initial/path', 'ignore_cache': 'mock bool'},
-            {'additional_value': 'something'},
-            {'home_directory': 'initial/path', 'ignore_cache': 'mock bool', 'additional_value': 'something'},
+            {'home_directory': 'default/home', 'cache_directory': 'default/cache', 'ignore_cache': False},
+            {'cache_directory': 'overloaded/cache'},
+            {'home_directory': 'default/home', 'cache_directory': 'overloaded/cache', 'ignore_cache': False},
+        ),
+        # `ignore_cache=False` can only be overloaded if `ignore_cache=True` was
+        # not set globally.
+        (
+            {'home_directory': 'default/home', 'cache_directory': 'default/cache', 'ignore_cache': False},
+            {'ignore_cache': True},
+            {'home_directory': 'default/home', 'cache_directory': 'default/cache', 'ignore_cache': True},
+        ),
+        (
+            {'home_directory': 'default/home', 'cache_directory': 'default/cache', 'ignore_cache': True},
+            {'ignore_cache': False},
+            {'home_directory': 'default/home', 'cache_directory': 'default/cache', 'ignore_cache': True},
+        ),
+        (
+            {'home_directory': 'default/home', 'cache_directory': 'default/cache', 'ignore_cache': True},
+            {'ignore_cache': True},
+            {'home_directory': 'default/home', 'cache_directory': 'default/cache', 'ignore_cache': True},
         ),
     ),
     ids=lambda v: repr(v),
 )
 def test_common_job_args(common_job_args, overload, exp_return_value, make_TestTrackerJobs):
     tracker_jobs = make_TestTrackerJobs(common_job_args=common_job_args)
     return_value = tracker_jobs.common_job_args(**overload)
@@ -320,27 +338,27 @@
 def test_create_torrent_job(make_TestTrackerJobs, mocker):
     CreateTorrentJob_mock = mocker.patch('upsies.jobs.torrent.CreateTorrentJob')
     tracker_jobs = make_TestTrackerJobs(
         content_path='path/to/content',
         reuse_torrent_path='path/to/existing.torrent',
         tracker='mock tracker',
         exclude_files=('a', 'b', 'c'),
-        common_job_args={'home_directory': 'path/to/home', 'ignore_cache': 'mock bool'},
+        common_job_args={'home_directory': 'path/to/home', 'ignore_cache': False},
     )
     mocker.patch.object(tracker_jobs, 'make_precondition')
     assert tracker_jobs.create_torrent_job is CreateTorrentJob_mock.return_value
     assert CreateTorrentJob_mock.call_args_list == [
         call(
             content_path='path/to/content',
             reuse_torrent_path='path/to/existing.torrent',
             tracker='mock tracker',
             exclude_files=('a', 'b', 'c'),
             precondition=tracker_jobs.make_precondition.return_value,
             home_directory='path/to/home',
-            ignore_cache='mock bool',
+            ignore_cache=False,
         ),
     ]
     assert tracker_jobs.make_precondition.call_args_list == [call('create_torrent_job')]
 
 def test_create_torrent_job_is_singleton(make_TestTrackerJobs, mocker):
     mocker.patch('upsies.jobs.torrent.CreateTorrentJob', side_effect=(Mock(), Mock()))
     tracker_jobs = make_TestTrackerJobs()
@@ -354,15 +372,15 @@
         (None, Mock(), True),
         (Mock(), None, True),
     ),
 )
 def test_add_torrent_job(btclient, create_torrent_job, exp_add_torrent_job_is_None, make_TestTrackerJobs, mocker):
     AddTorrentJob_mock = mocker.patch('upsies.jobs.torrent.AddTorrentJob')
     tracker_jobs = make_TestTrackerJobs(
-        common_job_args={'home_directory': 'path/to/home', 'ignore_cache': 'mock bool'},
+        common_job_args={'home_directory': 'path/to/home', 'ignore_cache': False},
         btclient=btclient,
     )
     mocker.patch.object(type(tracker_jobs), 'create_torrent_job', PropertyMock(return_value=create_torrent_job))
     mocker.patch.object(tracker_jobs, 'make_precondition')
     if exp_add_torrent_job_is_None:
         assert tracker_jobs.add_torrent_job is None
         assert AddTorrentJob_mock.call_args_list == []
@@ -371,15 +389,15 @@
         assert tracker_jobs.add_torrent_job is AddTorrentJob_mock.return_value
         assert AddTorrentJob_mock.call_args_list == [
             call(
                 autostart=False,
                 btclient=btclient,
                 precondition=tracker_jobs.make_precondition.return_value,
                 home_directory='path/to/home',
-                ignore_cache='mock bool',
+                ignore_cache=False,
             ),
         ]
         assert tracker_jobs.create_torrent_job.signal.register.call_args_list == [
             call('output', tracker_jobs.add_torrent_job.enqueue),
             call('finished', tracker_jobs.finalize_add_torrent_job),
         ]
         assert tracker_jobs.make_precondition.call_args_list == [call('add_torrent_job')]
@@ -410,15 +428,15 @@
 )
 def test_copy_torrent_job(
         torrent_destination, create_torrent_job, exp_copy_torrent_job_is_None,
         make_TestTrackerJobs, mocker,
 ):
     CopyTorrentJob_mock = mocker.patch('upsies.jobs.torrent.CopyTorrentJob')
     tracker_jobs = make_TestTrackerJobs(
-        common_job_args={'home_directory': 'path/to/home', 'ignore_cache': 'mock bool'},
+        common_job_args={'home_directory': 'path/to/home', 'ignore_cache': False},
         torrent_destination=torrent_destination,
     )
     mocker.patch.object(type(tracker_jobs), 'create_torrent_job', PropertyMock(return_value=create_torrent_job))
     mocker.patch.object(tracker_jobs, 'make_precondition')
     if exp_copy_torrent_job_is_None:
         assert tracker_jobs.copy_torrent_job is None
         assert CopyTorrentJob_mock.call_args_list == []
@@ -427,15 +445,15 @@
         assert tracker_jobs.copy_torrent_job is CopyTorrentJob_mock.return_value
         assert CopyTorrentJob_mock.call_args_list == [
             call(
                 autostart=False,
                 destination=torrent_destination,
                 precondition=tracker_jobs.make_precondition.return_value,
                 home_directory='path/to/home',
-                ignore_cache='mock bool',
+                ignore_cache=False,
             ),
         ]
         assert tracker_jobs.create_torrent_job.signal.register.call_args_list == [
             call('output', tracker_jobs.copy_torrent_job.enqueue),
             call('finished', tracker_jobs.finalize_copy_torrent_job),
         ]
         assert tracker_jobs.make_precondition.call_args_list == [call('copy_torrent_job')]
@@ -494,15 +512,15 @@
     ]
 
 
 def test_release_name_job(make_TestTrackerJobs, mocker):
     TextFieldJob_mock = mocker.patch('upsies.jobs.dialog.TextFieldJob')
     tracker_jobs = make_TestTrackerJobs(
         content_path='path/to/content',
-        common_job_args={'home_directory': 'path/to/home', 'ignore_cache': 'mock bool'},
+        common_job_args={'home_directory': 'path/to/home', 'ignore_cache': False},
     )
 
     mocker.patch.object(type(tracker_jobs), 'release_name', PropertyMock())
     mocker.patch.object(tracker_jobs, 'get_job_name')
     mocker.patch.object(tracker_jobs, 'make_precondition')
 
     release_name_job = tracker_jobs.release_name_job
@@ -513,15 +531,15 @@
             label='Release Name',
             callbacks={
                 'output': tracker_jobs.release_name.set_release_info,
             },
             precondition=tracker_jobs.make_precondition.return_value,
             validator=tracker_jobs.validate_release_name,
             home_directory='path/to/home',
-            ignore_cache='mock bool',
+            ignore_cache=False,
         ),
     ]
     assert tracker_jobs.make_precondition.call_args_list == [call('release_name_job')]
 
 def test_release_name_job_is_singleton(make_TestTrackerJobs, mocker):
     mocker.patch('upsies.jobs.dialog.TextFieldJob', side_effect=(Mock(), Mock()))
     tracker_jobs = make_TestTrackerJobs()
@@ -571,30 +589,31 @@
     ]
     assert tracker_jobs.release_name.fetch_info.call_args_list == [call(webdb=webdb, webdb_id='tt123456')]
 
 
 def test_imdb_job(make_TestTrackerJobs, mocker):
     tracker_jobs = make_TestTrackerJobs(
         content_path='path/to/content',
-        common_job_args={'home_directory': 'path/to/home', 'ignore_cache': 'mock bool'},
+        common_job_args={'home_directory': 'path/to/home', 'ignore_cache': False},
     )
     WebDbSearchJob_mock = mocker.patch('upsies.jobs.webdb.WebDbSearchJob')
     mocker.patch.object(tracker_jobs, 'make_precondition')
     imdb_job = tracker_jobs.imdb_job
     assert imdb_job is WebDbSearchJob_mock.return_value
     assert WebDbSearchJob_mock.call_args_list == [
         call(
             query='path/to/content',
             db=tracker_jobs.imdb,
+            show_poster=tracker_jobs._show_poster,
             callbacks={
                 'output': tracker_jobs._handle_imdb_id,
             },
             precondition=tracker_jobs.make_precondition.return_value,
             home_directory='path/to/home',
-            ignore_cache='mock bool',
+            ignore_cache=False,
         ),
     ]
     assert tracker_jobs.make_precondition.call_args_list == [call('imdb_job')]
 
 def test_imdb_job_is_singleton(make_TestTrackerJobs, mocker):
     mocker.patch('upsies.jobs.webdb.WebDbSearchJob', side_effect=(Mock(), Mock()))
     tracker_jobs = make_TestTrackerJobs()
@@ -627,28 +646,29 @@
 
 
 def test_tmdb_job(make_TestTrackerJobs, mocker):
     WebDbSearchJob_mock = mocker.patch('upsies.jobs.webdb.WebDbSearchJob')
     webdb_mock = mocker.patch('upsies.utils.webdbs.webdb')
     tracker_jobs = make_TestTrackerJobs(
         content_path='path/to/content',
-        common_job_args={'home_directory': 'path/to/home', 'ignore_cache': 'mock bool'},
+        common_job_args={'home_directory': 'path/to/home', 'ignore_cache': False},
     )
     mocker.patch.object(tracker_jobs, 'make_precondition')
     assert tracker_jobs.tmdb_job is WebDbSearchJob_mock.return_value
     assert WebDbSearchJob_mock.call_args_list == [
         call(
             query='path/to/content',
             db=webdb_mock.return_value,
+            show_poster=tracker_jobs._show_poster,
             callbacks={
                 'output': tracker_jobs._handle_tmdb_id,
             },
             precondition=tracker_jobs.make_precondition.return_value,
             home_directory='path/to/home',
-            ignore_cache='mock bool',
+            ignore_cache=False,
         ),
     ]
     assert webdb_mock.call_args_list == [call('tmdb')]
     assert tracker_jobs.make_precondition.call_args_list == [call('tmdb_job')]
 
 
 def test_tmdb_job_is_singleton(make_TestTrackerJobs, mocker):
@@ -683,28 +703,29 @@
 
 
 def test_tvmaze_job(make_TestTrackerJobs, mocker):
     WebDbSearchJob_mock = mocker.patch('upsies.jobs.webdb.WebDbSearchJob')
     webdb_mock = mocker.patch('upsies.utils.webdbs.webdb')
     tracker_jobs = make_TestTrackerJobs(
         content_path='path/to/content',
-        common_job_args={'home_directory': 'path/to/home', 'ignore_cache': 'mock bool'},
+        common_job_args={'home_directory': 'path/to/home', 'ignore_cache': False},
     )
     mocker.patch.object(tracker_jobs, 'make_precondition')
     assert tracker_jobs.tvmaze_job is WebDbSearchJob_mock.return_value
     assert WebDbSearchJob_mock.call_args_list == [
         call(
             query='path/to/content',
             db=webdb_mock.return_value,
+            show_poster=tracker_jobs._show_poster,
             callbacks={
                 'output': tracker_jobs._handle_tvmaze_id,
             },
             precondition=tracker_jobs.make_precondition.return_value,
             home_directory='path/to/home',
-            ignore_cache='mock bool',
+            ignore_cache=False,
         ),
     ]
     assert webdb_mock.call_args_list == [call('tvmaze')]
     assert tracker_jobs.make_precondition.call_args_list == [call('tvmaze_job')]
 
 def test_tvmaze_job_is_singleton(make_TestTrackerJobs, mocker):
     mocker.patch('upsies.jobs.webdb.WebDbSearchJob', side_effect=(Mock(), Mock()))
@@ -816,15 +837,15 @@
     ]
 
 
 def test_screenshots_job(make_TestTrackerJobs, mocker):
     ScreenshotsJob_mock = mocker.patch('upsies.jobs.screenshots.ScreenshotsJob')
     tracker_jobs = make_TestTrackerJobs(
         content_path='path/to/content',
-        common_job_args={'home_directory': 'path/to/home', 'ignore_cache': 'mock bool'},
+        common_job_args={'home_directory': 'path/to/home', 'ignore_cache': False},
     )
     mocker.patch.object(tracker_jobs, 'make_precondition')
     mocker.patch.object(type(tracker_jobs), 'screenshots_count', PropertyMock())
     mocker.patch.object(type(tracker_jobs), 'screenshots_from_all_videos', PropertyMock())
     mocker.patch.object(type(tracker_jobs), 'create_torrent_job', PropertyMock())
     assert tracker_jobs.screenshots_job is ScreenshotsJob_mock.return_value
     assert ScreenshotsJob_mock.call_args_list == [
@@ -832,15 +853,15 @@
             content_path='path/to/content',
             exclude_files=tracker_jobs.exclude_files,
             count=tracker_jobs.screenshots_count,
             from_all_videos=tracker_jobs.screenshots_from_all_videos,
             optimize=tracker_jobs._screenshots_optimization,
             precondition=tracker_jobs.make_precondition.return_value,
             home_directory='path/to/home',
-            ignore_cache='mock bool',
+            ignore_cache=False,
         ),
     ]
     assert tracker_jobs.make_precondition.call_args_list == [call('screenshots_job')]
 
 def test_screenshots_job_is_singleton(make_TestTrackerJobs, mocker):
     mocker.patch('upsies.jobs.screenshots.ScreenshotsJob', side_effect=(Mock(), Mock()))
     tracker_jobs = make_TestTrackerJobs()
@@ -877,29 +898,29 @@
         make_TestTrackerJobs, mocker,
 ):
     ImageHostJob_mock = mocker.patch('upsies.jobs.imghost.ImageHostJob')
     mocker.patch('upsies.jobs.screenshots.ScreenshotsJob')
     tracker_jobs = make_TestTrackerJobs(
         image_hosts=image_hosts,
         content_path='path/to/content',
-        common_job_args={'home_directory': 'path/to/home', 'ignore_cache': 'mock bool'},
+        common_job_args={'home_directory': 'path/to/home', 'ignore_cache': False},
     )
     mocker.patch.object(type(tracker_jobs), 'screenshots_job', PropertyMock(return_value=screenshots_job))
     mocker.patch.object(tracker_jobs, 'make_precondition')
     if exp_upload_screenshots_job_is_None:
         assert tracker_jobs.upload_screenshots_job is None
         assert ImageHostJob_mock.call_args_list == []
         assert tracker_jobs.make_precondition.call_args_list == []
     else:
         assert tracker_jobs.upload_screenshots_job is ImageHostJob_mock.return_value
         assert ImageHostJob_mock.call_args_list == [call(
             imghosts=image_hosts,
             precondition=tracker_jobs.make_precondition.return_value,
             home_directory='path/to/home',
-            ignore_cache='mock bool',
+            ignore_cache=False,
         )]
         # ScreenshotsJob also registers a callback for "timestamps"
         assert tracker_jobs.screenshots_job.signal.register.call_args_list == [
             call('screenshots_total', tracker_jobs.upload_screenshots_job.set_images_total),
             call('output', tracker_jobs.upload_screenshots_job.enqueue),
             call('finished', tracker_jobs.finalize_upload_screenshots_job),
         ]
@@ -911,23 +932,23 @@
     tracker_jobs = make_TestTrackerJobs()
     assert tracker_jobs.upload_screenshots_job is tracker_jobs.upload_screenshots_job
 
 
 def test_poster_job(make_TestTrackerJobs, mocker):
     PosterJob_mock = mocker.patch('upsies.jobs.poster.PosterJob')
     tracker_jobs = make_TestTrackerJobs(
-        common_job_args={'home_directory': 'path/to/home', 'ignore_cache': 'mock bool'},
+        common_job_args={'home_directory': 'path/to/home', 'ignore_cache': False},
     )
     mocker.patch.object(tracker_jobs, 'make_poster_job_precondition')
     assert tracker_jobs.poster_job is PosterJob_mock.return_value
     assert PosterJob_mock.call_args_list == [
         call(
             precondition=tracker_jobs.make_poster_job_precondition.return_value,
             home_directory='path/to/home',
-            ignore_cache='mock bool',
+            ignore_cache=False,
             getter=tracker_jobs.get_poster,
             width=tracker_jobs.poster_max_width,
             height=tracker_jobs.poster_max_height,
             write_to=None,
             imghosts=tracker_jobs.image_hosts,
         ),
     ]
@@ -1305,15 +1326,15 @@
     assert tracker_jobs.upload_screenshots_job.close.call_args_list == [call()]
 
 
 def test_mediainfo_job(make_TestTrackerJobs, mocker):
     MediainfoJob_mock = mocker.patch('upsies.jobs.mediainfo.MediainfoJob')
     tracker_jobs = make_TestTrackerJobs(
         content_path='path/to/content',
-        common_job_args={'home_directory': 'path/to/home', 'ignore_cache': 'mock bool'},
+        common_job_args={'home_directory': 'path/to/home', 'ignore_cache': False},
     )
     mocker.patch.object(type(tracker_jobs), 'mediainfo_from_all_videos', PropertyMock(
         return_value='maybe from_all_videos?',
     )),
     mocker.patch.object(type(tracker_jobs), 'exclude_files', PropertyMock(
         return_value='exclude these files!',
     )),
@@ -1322,15 +1343,15 @@
     assert MediainfoJob_mock.call_args_list == [
         call(
             content_path='path/to/content',
             from_all_videos='maybe from_all_videos?',
             exclude_files='exclude these files!',
             precondition=tracker_jobs.make_precondition.return_value,
             home_directory='path/to/home',
-            ignore_cache='mock bool',
+            ignore_cache=False,
         ),
     ]
     assert tracker_jobs.make_precondition.call_args_list == [call('mediainfo_job')]
 
 def test_mediainfo_job_is_singleton(make_TestTrackerJobs, mocker):
     mocker.patch('upsies.jobs.mediainfo.MediainfoJob', side_effect=(Mock(), Mock()))
     tracker_jobs = make_TestTrackerJobs()
```

### Comparing `upsies-2024.3.9/tests/trackers_test/bhd/bhd_tracker_config_test.py` & `upsies-2024.4.12/tests/trackers_test/bhd/bhd_tracker_config_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 def test_BhdTrackerConfig_defaults(tracker_config):
     assert set(tracker_config) == {
         'upload_url',
         'announce_url',
         'announce_passkey',
         'apikey',
-        'source',
         'randomize_infohash',
         'anonymous',
         'draft',
         'image_host',
         'screenshots',
         'exclude',
 
@@ -55,18 +54,14 @@
     assert tracker_config['apikey'] == ''
     assert tracker_config['apikey'].description == (
         'Your personal private API key.\n'
         'Get it from the website: My Security -> API key'
     )
 
 
-def test_BhdTrackerConfig_defaults_source(tracker_config):
-    assert tracker_config['source'] == 'BHD'
-
-
 def test_BhdTrackerConfig_defaults_anonymous(tracker_config):
     assert isinstance(tracker_config['anonymous'], utils.types.Bool)
     assert not tracker_config['anonymous']
     assert tracker_config['anonymous'] == 'no'
     assert tracker_config['anonymous'].description == (
         'Whether your username is displayed on your uploads.'
     )
@@ -112,28 +107,37 @@
         utils.types.RegEx(base.exclude.subtitles),
     )
 
 
 def test_BhdTrackerConfig_arguments(tracker_config):
     exp_argument_definitions = {
         'submit': {
+            ('--anonymous', '--an'),
             ('--custom-edition', '--ce'),
             ('--draft', '--dr'),
             ('--personal-rip', '--pr'),
             ('--screenshots', '--ss'),
             ('--special', '--sp'),
             ('--only-description', '--od'),
             ('--only-title', '--ot'),
         },
     }
     assert set(tracker_config.argument_definitions) == set(exp_argument_definitions)
     for command in exp_argument_definitions:
         assert set(tracker_config.argument_definitions[command]) == exp_argument_definitions[command]
 
 
+def test_BhdTrackerConfig_argument_definitions_submit_anonymous(tracker_config):
+    assert tracker_config.argument_definitions['submit'][('--anonymous', '--an')] == {
+        'help': 'Hide your username for this submission',
+        'action': 'store_true',
+        'default': None,
+    }
+
+
 def test_BhdTrackerConfig_argument_definitions_submit_custom_edition(tracker_config):
     assert tracker_config.argument_definitions['submit'][('--custom-edition', '--ce')] == {
         'help': 'Non-standard edition, e.g. "Final Cut"',
         'default': '',
     }
```

### Comparing `upsies-2024.3.9/tests/trackers_test/bhd/bhd_tracker_jobs_test.py` & `upsies-2024.4.12/tests/trackers_test/bhd/bhd_tracker_jobs_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/trackers_test/bhd/bhd_tracker_test.py` & `upsies-2024.4.12/tests/trackers_test/bhd/bhd_tracker_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,18 @@
     assert BhdTracker.name == 'bhd'
 
 
 def test_label_attribute():
     assert BhdTracker.label == 'BHD'
 
 
+def test_torrent_source_field_attribute():
+    assert BhdTracker.torrent_source_field == 'BHD'
+
+
 def test_TrackerConfig_attribute():
     assert BhdTracker.TrackerConfig is BhdTrackerConfig
 
 
 def test_TrackerJobs_attribute():
     assert BhdTracker.TrackerJobs is BhdTrackerJobs
```

### Comparing `upsies-2024.3.9/tests/trackers_test/conftest.py` & `upsies-2024.4.12/tests/trackers_test/conftest.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/trackers_test/mtv/mtv_tracker_config_test.py` & `upsies-2024.4.12/tests/trackers_test/mtv/mtv_tracker_config_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 def test_MtvTrackerConfig_defaults(tracker_config):
     assert set(tracker_config) == {
         'base_url',
         'username',
         'password',
         'announce_url',
-        'source',
         'randomize_infohash',
         'image_host',
         'screenshots',
         'exclude',
         'anonymous',
 
         # Inherited from TrackerConfigBase
@@ -46,18 +45,14 @@
 def test_MtvTrackerConfig_defaults_announce_url(tracker_config):
     assert tracker_config['announce_url'] == ''
     assert tracker_config['announce_url'].description == (
         'Your personal announce URL. Automatically fetched from the website if not set.'
     )
 
 
-def test_MtvTrackerConfig_defaults_source(tracker_config):
-    assert tracker_config['source'] == 'MTV'
-
-
 def test_MtvTrackerConfig_defaults_image_host(tracker_config, assert_config_list_of_choice):
     exp_options = ('dummy', 'imgbox', 'ptpimg')
     assert_config_list_of_choice(
         items=tracker_config['image_host'],
         exp_items=('imgbox',),
         exp_options=exp_options,
         exp_description=(
@@ -97,25 +92,34 @@
         'Whether your username is displayed on your uploads.'
     )
 
 
 def test_MtvTrackerConfig_arguments(tracker_config):
     exp_argument_definitions = {
         'submit': {
+            ('--anonymous', '--an'),
             ('--screenshots', '--ss'),
             ('--only-description', '--od'),
             ('--only-title', '--ot'),
             ('--ignore-dupes', '--id'),
         },
     }
     assert set(tracker_config.argument_definitions) == set(exp_argument_definitions)
     for command in exp_argument_definitions:
         assert set(tracker_config.argument_definitions[command]) == exp_argument_definitions[command]
 
 
+def test_MtvTrackerConfig_argument_definitions_submit_anonymous(tracker_config):
+    assert tracker_config.argument_definitions['submit'][('--anonymous', '--an')] == {
+        'help': 'Hide your username for this submission',
+        'action': 'store_true',
+        'default': None,
+    }
+
+
 def test_MtvTrackerConfig_argument_definitions_submit_screenshots(tracker_config):
     assert tracker_config.argument_definitions['submit'][('--screenshots', '--ss')] == {
         'help': ('How many screenshots to make '
                  f'(min={tracker_config["screenshots"].min}, '
                  f'max={tracker_config["screenshots"].max})'),
         'type': utils.argtypes.number_of_screenshots(
             min=tracker_config['screenshots'].min,
```

### Comparing `upsies-2024.3.9/tests/trackers_test/mtv/mtv_tracker_jobs_test.py` & `upsies-2024.4.12/tests/trackers_test/mtv/mtv_tracker_jobs_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/trackers_test/mtv/mtv_tracker_test.py` & `upsies-2024.4.12/tests/trackers_test/mtv/mtv_tracker_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,18 @@
     assert MtvTracker.name == 'mtv'
 
 
 def test_label_attribute():
     assert MtvTracker.label == 'MTV'
 
 
+def test_torrent_source_field_attribute():
+    assert MtvTracker.torrent_source_field == 'MTV'
+
+
 def test_TrackerConfig_attribute():
     assert MtvTracker.TrackerConfig is MtvTrackerConfig
 
 
 def test_TrackerJobs_attribute():
     assert MtvTracker.TrackerJobs is MtvTrackerJobs
```

### Comparing `upsies-2024.3.9/tests/trackers_test/nbl/nbl_tracker_config_test.py` & `upsies-2024.4.12/tests/trackers_test/nbl/nbl_tracker_config_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 
 
 def test_NblTrackerConfig_defaults(tracker_config):
     assert set(tracker_config) == {
         'upload_url',
         'announce_url',
         'apikey',
-        'source',
         'randomize_infohash',
         'exclude',
 
         # Inherited from TrackerConfigBase
         'add_to',
         'copy_to',
     }
@@ -41,17 +40,13 @@
     assert tracker_config['announce_url'] == ''
     assert tracker_config['announce_url'].description == (
         'The complete announce URL with your private passkey.\n'
         'Get it from the website: Shows -> Upload -> Your personal announce URL'
     )
 
 
-def test_NblTrackerConfig_defaults_source(tracker_config):
-    assert tracker_config['source'] == 'NBL'
-
-
 def test_NblTrackerConfig_defaults_exclude(tracker_config):
     assert tracker_config['exclude'] == ()
 
 
 def test_NblTrackerConfig_argument_definitions(tracker_config):
     assert tracker_config.argument_definitions == {}
```

### Comparing `upsies-2024.3.9/tests/trackers_test/nbl/nbl_tracker_jobs_test.py` & `upsies-2024.4.12/tests/trackers_test/nbl/nbl_tracker_jobs_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/trackers_test/nbl/nbl_tracker_test.py` & `upsies-2024.4.12/tests/trackers_test/nbl/nbl_tracker_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,18 @@
     assert nbl.NblTracker.name == 'nbl'
 
 
 def test_label_attribute():
     assert nbl.NblTracker.label == 'NBL'
 
 
+def test_torrent_source_field_attribute():
+    assert nbl.NblTracker.torrent_source_field == 'NBL'
+
+
 @pytest.mark.asyncio
 async def test_login(mocker):
     tracker = nbl.NblTracker()
     await tracker._login()
 
 
 @pytest.mark.asyncio
```

### Comparing `upsies-2024.3.9/tests/trackers_test/ptp/ptp_tracker_jobs_test.py` & `upsies-2024.4.12/tests/trackers_test/ptp/ptp_tracker_jobs_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,61 +120,72 @@
     mock_job_attributes(ptp_tracker_jobs)
     mocker.patch.object(type(ptp_tracker_jobs), 'options', PropertyMock(return_value={}))
     mocker.patch.object(ptp_tracker_jobs, 'get_job_and_dependencies')
     assert ptp_tracker_jobs.isolated_jobs == ()
     assert ptp_tracker_jobs.get_job_and_dependencies.call_args_list == []
 
 
-def test_type_job(ptp_tracker_jobs, mocker):
+@pytest.mark.parametrize(
+    argnames='options, exp_autofinish, exp_ignore_cache',
+    argvalues=(
+        ({}, False, False),
+        ({'type': ''}, False, False),
+        ({'type': None}, False, False),
+        ({'type': 'Movie'}, True, True),
+        ({'type': 'Short'}, True, True),
+    ),
+    ids=lambda v: repr(v),
+)
+def test_type_job(options, exp_autofinish, exp_ignore_cache, ptp_tracker_jobs, mocker):
     ChoiceJob_mock = mocker.patch('upsies.jobs.dialog.ChoiceJob')
     mocker.patch.object(ptp_tracker_jobs, 'get_job_name')
     mocker.patch.object(ptp_tracker_jobs, 'make_precondition')
     mocker.patch.object(ptp_tracker_jobs, 'common_job_args', return_value={'common_job_arg': 'common job argument'})
+    mocker.patch.object(type(ptp_tracker_jobs), 'options', PropertyMock(return_value=options))
 
     assert ptp_tracker_jobs.type_job is ChoiceJob_mock.return_value
     assert ChoiceJob_mock.call_args_list == [call(
         name=ptp_tracker_jobs.get_job_name.return_value,
         label='Type',
         precondition=ptp_tracker_jobs.make_precondition.return_value,
         autodetect=ptp_tracker_jobs.autodetect_type,
-        options=(
-            ('Feature Film', 'Feature Film'),
-            ('Short Film', 'Short Film'),
-            ('Miniseries', 'Miniseries'),
-            ('Stand-up Comedy', 'Stand-up Comedy'),
-            ('Live Performance', 'Live Performance'),
-            ('Movie Collection', 'Movie Collection'),
-        ),
+        options=ptp.metadata.types,
+        autofinish=exp_autofinish,
         callbacks={
             'finished': ptp_tracker_jobs.update_imdb_query,
         },
         common_job_arg='common job argument',
     )]
     assert ptp_tracker_jobs.get_job_name.call_args_list == [call('type')]
     assert ptp_tracker_jobs.make_precondition.call_args_list == [call('type_job')]
-    assert ptp_tracker_jobs.common_job_args.call_args_list == [call()]
+    assert ptp_tracker_jobs.common_job_args.call_args_list == [call(ignore_cache=exp_ignore_cache)]
 
 
 @pytest.mark.parametrize(
-    argnames='release_type, main_video_duration, exp_return_value, exp_duration_calls',
+    argnames='options, release_type, main_video_duration, exp_return_value, exp_duration_calls',
     argvalues=(
-        (utils.release.ReleaseType.season, 123, 'Miniseries', False),
-        (utils.release.ReleaseType.movie, 45 * 60, 'Short Film', True),
-        (utils.release.ReleaseType.movie, (45 * 60) + 1, None, True),
+        ({'type': 'movie'}, None, 0, 'Feature Film', False),
+        ({'type': 'short'}, None, 0, 'Short Film', False),
+        ({'type': 'series'}, None, 0, 'Miniseries', False),
+        ({'type': 'live'}, None, 0, 'Live Performance', False),
+        ({}, utils.release.ReleaseType.season, 123, 'Miniseries', False),
+        ({}, utils.release.ReleaseType.movie, 45 * 60, 'Short Film', True),
+        ({}, utils.release.ReleaseType.movie, (45 * 60) + 1, None, True),
     ),
     ids=lambda v: str(v),
 )
 def test_autodetect_type(
-        release_type, main_video_duration,
+        options, release_type, main_video_duration,
         exp_return_value, exp_duration_calls,
         ptp_tracker_jobs, mocker,
 ):
     mocker.patch.object(type(ptp_tracker_jobs), 'release_name', PropertyMock(return_value=Mock(
         type=release_type,
     )))
+    mocker.patch.object(type(ptp_tracker_jobs), 'options', PropertyMock(return_value=options))
 
     mocks = Mock()
     mocks.attach_mock(
         mocker.patch('upsies.utils.video.find_videos', return_value=iter(
             ('Foo.S01E01.mkv', 'Foo.S01E02.mkv', 'Foo.S01E03.mkv', 'Foo.sample.mkv'),
         )),
         'find_videos',
@@ -199,17 +210,38 @@
             call.filter_main_videos(('Foo.S01E01.mkv', 'Foo.S01E02.mkv', 'Foo.S01E03.mkv', 'Foo.sample.mkv')),
             call.duration('Foo.S01E01.mkv'),
         ]
     else:
         assert mocks.mock_calls == []
 
 
-def test_imdb_job(ptp_tracker_jobs, mocker):
-    mocker.patch('upsies.jobs.webdb.WebDbSearchJob')
-    assert ptp_tracker_jobs.imdb_job.no_id_ok is True
+@pytest.mark.parametrize(
+    argnames='options, exp_imdb_job_attributes, exp_query_attributes',
+    argvalues=(
+        (
+            {},
+            {'no_id_ok': True},
+            {'id': None, 'feeling_lucky': False},
+        ),
+        (
+            {'imdb': 'tt0123456'},
+            {'no_id_ok': True},
+            {'id': 'tt0123456', 'feeling_lucky': True},
+        ),
+    ),
+    ids=lambda v: repr(v),
+)
+def test_imdb_job(options, exp_imdb_job_attributes, exp_query_attributes, ptp_tracker_jobs, mocker):
+    mocker.patch.object(type(ptp_tracker_jobs), 'options', PropertyMock(return_value=options))
+
+    for name, exp_value in exp_imdb_job_attributes.items():
+        assert getattr(ptp_tracker_jobs.imdb_job, name) == exp_value
+
+    for name, exp_value in exp_query_attributes.items():
+        assert getattr(ptp_tracker_jobs.imdb_job.query, name) == exp_value
 
 
 @pytest.mark.parametrize(
     argnames='type_job_output, exp_query_type',
     argvalues=(
         ([], '<original query type>'),
         (['Feature Film'], utils.release.ReleaseType.movie),
@@ -869,44 +901,48 @@
         ptp_tracker_jobs.ptp_group_id_job,
         ptp_tracker_jobs.imdb_job,
     )]
     assert ptp_tracker_jobs.common_job_args.call_args_list == [call()]
 
 
 @pytest.mark.parametrize(
-    argnames='imdb_job, exp_exception',
+    argnames='imdb_job, metadata, exp_result',
     argvalues=(
-        (Mock(is_finished=False), AssertionError),
-        (Mock(is_finished=True, output=['123']), None),
+        (Mock(is_finished=False), {}, AssertionError),
+        (Mock(is_finished=True), {'title': 'The PTP Title'}, 'The PTP Title'),
+        (Mock(is_finished=True), {'title': ''}, None),
     ),
     ids=lambda v: str(v),
 )
 @pytest.mark.asyncio
-async def test_fetch_title(imdb_job, exp_exception, ptp_tracker_jobs, mocker):
+async def test_fetch_title(imdb_job, metadata, exp_result, ptp_tracker_jobs, mocker):
     mocker.patch.object(type(ptp_tracker_jobs), 'imdb_job', PropertyMock(return_value=imdb_job))
+    mocker.patch.object(type(ptp_tracker_jobs), 'imdb_id', PropertyMock(return_value='tt123456'))
     mocker.patch.object(type(ptp_tracker_jobs), 'title_job', PropertyMock())
     mocker.patch.object(type(ptp_tracker_jobs), 'release_name', PropertyMock(return_value=Mock(
         title='The Release Name Title',
     )))
 
     async def get_movie_metadata(*args, **kwargs):
         assert ptp_tracker_jobs.title_job.text == 'The Release Name Title'
-        return {'title': 'The PTP Title'}
+        return metadata
 
     mocker.patch.object(ptp_tracker_jobs.tracker, 'get_movie_metadata', AsyncMock(
         side_effect=get_movie_metadata,
     ))
 
-    if exp_exception:
-        with pytest.raises(exp_exception) as exception_info:
+    if isinstance(exp_result, type) and issubclass(exp_result, Exception):
+        with pytest.raises(exp_result):
+            await ptp_tracker_jobs.fetch_title()
+    elif isinstance(exp_result, Exception):
+        with pytest.raises(type(exp_result), match=rf'^{re.escape(str(exp_result))}$'):
             await ptp_tracker_jobs.fetch_title()
-        assert exception_info.value.args[0] is ptp_tracker_jobs.imdb_job
     else:
         return_value = await ptp_tracker_jobs.fetch_title()
-        assert return_value == 'The PTP Title'
+        assert return_value == exp_result
         assert ptp_tracker_jobs.tracker.get_movie_metadata.call_args_list == [
             call(ptp_tracker_jobs.imdb_id),
         ]
 
 
 @pytest.mark.parametrize(
     argnames='text, exp_title',
@@ -974,44 +1010,50 @@
         ptp_tracker_jobs.ptp_group_id_job,
         ptp_tracker_jobs.imdb_job,
     )]
     assert ptp_tracker_jobs.common_job_args.call_args_list == [call()]
 
 
 @pytest.mark.parametrize(
-    argnames='imdb_job, exp_exception',
+    argnames='imdb_job, metadata, exp_result',
     argvalues=(
-        (Mock(is_finished=False), AssertionError),
-        (Mock(is_finished=True, output=['2012']), None),
+        (Mock(is_finished=False), {}, AssertionError),
+        (Mock(is_finished=True), {'year': '2013'}, '2013'),
+        (Mock(is_finished=True), {'year': ''}, None),
     ),
     ids=lambda v: str(v),
 )
 @pytest.mark.asyncio
-async def test_fetch_year(imdb_job, exp_exception, ptp_tracker_jobs, mocker):
+async def test_fetch_year(imdb_job, metadata, exp_result, ptp_tracker_jobs, mocker):
     mocker.patch.object(type(ptp_tracker_jobs), 'imdb_job', PropertyMock(return_value=imdb_job))
+    mocker.patch.object(type(ptp_tracker_jobs), 'imdb_id', PropertyMock(return_value='tt123456'))
     mocker.patch.object(type(ptp_tracker_jobs), 'year_job', PropertyMock())
     mocker.patch.object(type(ptp_tracker_jobs), 'release_name', PropertyMock(return_value=Mock(
         year='2012',
     )))
 
     async def get_movie_metadata(*args, **kwargs):
         assert ptp_tracker_jobs.year_job.text == '2012'
-        return {'year': '2021'}
+        return metadata
 
     mocker.patch.object(ptp_tracker_jobs.tracker, 'get_movie_metadata', AsyncMock(
         side_effect=get_movie_metadata,
     ))
 
-    if exp_exception:
-        with pytest.raises(exp_exception) as exception_info:
+    if isinstance(exp_result, type) and issubclass(exp_result, Exception):
+        with pytest.raises(exp_result):
             await ptp_tracker_jobs.fetch_year()
-        assert exception_info.value.args[0] is ptp_tracker_jobs.imdb_job
+
+    elif isinstance(exp_result, Exception):
+        with pytest.raises(type(exp_result), match=rf'^{re.escape(str(exp_result))}$'):
+            await ptp_tracker_jobs.fetch_year()
+
     else:
         return_value = await ptp_tracker_jobs.fetch_year()
-        assert return_value == '2021'
+        assert return_value == exp_result
         assert ptp_tracker_jobs.tracker.get_movie_metadata.call_args_list == [
             call(ptp_tracker_jobs.imdb_id),
         ]
 
 
 @pytest.mark.parametrize(
     argnames='text, exp_year',
@@ -1440,15 +1482,16 @@
 
 
 @pytest.mark.parametrize(
     argnames='text, exp_exception',
     argvalues=(
         ('horror,awesome,drama', ValueError('Tag is not valid: awesome')),
         ('horror,drama', None),
-        ('', None),
+        ('', ValueError('You must provide at least one tag.')),
+        (', '.join(ptp.metadata.tags), ValueError('You provided too many tags.')),
     ),
     ids=lambda v: str(v),
 )
 @pytest.mark.asyncio
 async def test_validate_tags(text, exp_exception, ptp_tracker_jobs):
     if exp_exception:
         with pytest.raises(type(exp_exception), match=rf'^{re.escape(str(exp_exception))}$'):
@@ -2077,79 +2120,93 @@
         call.TextPrompt(
             question='Wat?',
         ),
         call.add_prompt(mocks.TextPrompt.return_value),
     ]
 
 
-def test_source_job(ptp_tracker_jobs, mocker):
+@pytest.mark.parametrize(
+    argnames='options, exp_ignore_cache',
+    argvalues=(
+        ({}, False),
+        ({'source': ''}, False),
+        ({'source': None}, False),
+        ({'source': 'WEB-ray'}, True),
+    ),
+    ids=lambda v: repr(v),
+)
+def test_source_job(options, exp_ignore_cache, ptp_tracker_jobs, mocker):
     TextFieldJob_mock = mocker.patch('upsies.jobs.dialog.TextFieldJob')
     mocker.patch.object(ptp_tracker_jobs, 'get_job_name')
     mocker.patch.object(ptp_tracker_jobs, 'make_precondition')
     mocker.patch.object(ptp_tracker_jobs, 'common_job_args', return_value={'common_job_arg': 'common job argument'})
+    mocker.patch.object(type(ptp_tracker_jobs), 'options', PropertyMock(return_value=options))
 
     assert ptp_tracker_jobs.source_job is TextFieldJob_mock.return_value
     assert TextFieldJob_mock.call_args_list == [call(
         name=ptp_tracker_jobs.get_job_name.return_value,
         label='Source',
         precondition=ptp_tracker_jobs.make_precondition.return_value,
         text=ptp_tracker_jobs.autodetect_source,
         normalizer=ptp_tracker_jobs.normalize_source,
         validator=ptp_tracker_jobs.validate_source,
         finish_on_success=True,
         common_job_arg='common job argument',
     )]
     assert ptp_tracker_jobs.get_job_name.call_args_list == [call('source')]
     assert ptp_tracker_jobs.make_precondition.call_args_list == [call('source_job')]
-    assert ptp_tracker_jobs.common_job_args.call_args_list == [call()]
+    assert ptp_tracker_jobs.common_job_args.call_args_list == [call(ignore_cache=exp_ignore_cache)]
 
 
 @pytest.mark.parametrize(
-    argnames='release_name_source, exp_source, exp_source_job_text',
+    argnames='options, release_name_source, exp_source, exp_source_job_text',
     argvalues=(
-        ('BluRay', 'Blu-ray', None),
-        ('DVD', 'DVD', None),
-        ('DVDRip', 'DVD', None),
-        ('WEB', 'WEB', None),
-        ('WEB-DL', 'WEB', None),
-        ('WEBDL', 'WEB', None),
-        ('WEBRip', 'WEB', None),
-        ('HD-DVD', 'HD-DVD', None),
-        ('HDDVD', 'HD-DVD', None),
-        ('HD-TV', 'HDTV', None),
-        ('HDTV', 'HDTV', None),
-        ('TV', 'TV', None),
-        ('VHS', 'VHS', None),
-        ('VHSRip', 'VHS', None),
-        ('YerMom', None, 'YerMom'),
+        ({}, 'BluRay', 'Blu-ray', None),
+        ({'source': 'dvd'}, 'Blu-ray', 'DVD', None),
+        ({'source': ''}, 'DVDrip', 'DVD', None),
+        ({'source': 'WEB'}, 'DVDRip', 'WEB', None),
+        ({}, 'WEB-DL', 'WEB', None),
+        ({'source': 'WEBDL'}, 'DVD', 'WEB', None),
+        ({'source': None}, 'WEBRip', 'WEB', None),
+        ({'source': 'Hd-Dvd'}, None, 'HD-DVD', None),
+        ({'source': ''}, 'HDDVD', 'HD-DVD', None),
+        ({'source': ''}, 'HD-TV', 'HDTV', None),
+        ({'source': 'HDtv'}, 'Blu-ray', 'HDTV', None),
+        ({}, 'TV', 'TV', None),
+        ({'source': 'VHS'}, 'WEB', 'VHS', None),
+        ({}, 'VHSRip', 'VHS', None),
+        ({}, 'YerMom', None, 'YerMom'),
+        ({'source': 'MeMom'}, 'YerMom', None, 'MeMom'),
     ),
     ids=lambda v: str(v),
 )
-def test_autodetect_source(release_name_source, exp_source, exp_source_job_text, ptp_tracker_jobs, mocker):
+def test_autodetect_source(options, release_name_source, exp_source, exp_source_job_text, ptp_tracker_jobs, mocker):
     mocker.patch.object(type(ptp_tracker_jobs), 'release_name', PropertyMock(return_value=Mock(
         source=release_name_source,
     )))
     mocker.patch.object(type(ptp_tracker_jobs), 'source_job', PropertyMock(return_value=Mock(
         text='not set',
     )))
+    mocker.patch.object(type(ptp_tracker_jobs), 'options', PropertyMock(return_value=options))
 
     return_value = ptp_tracker_jobs.autodetect_source()
     assert return_value == exp_source
     if exp_source_job_text is not None:
         assert ptp_tracker_jobs.source_job.text == exp_source_job_text
     else:
         assert ptp_tracker_jobs.source_job.text == 'not set'
 
 
 @pytest.mark.parametrize(
     argnames='text, exp_source',
     argvalues=(
-        ('blu-ray', 'Blu-ray'),
-        ('Blu-ray', 'Blu-ray'),
-        ('BLU-RAY', 'Blu-ray'),
+        ('bluray', 'Blu-ray'),
+        ('BluRay', 'Blu-ray'),
+        ('hd-dvd', 'HD-DVD'),
+        ('hddvd', 'HD-DVD'),
         ('YerMom', 'YerMom'),
     ),
     ids=lambda v: str(v),
 )
 def test_normalize_source(text, exp_source, ptp_tracker_jobs):
     return_value = ptp_tracker_jobs.normalize_source(text)
     assert return_value == exp_source
```

### Comparing `upsies-2024.3.9/tests/trackers_test/ptp/ptp_tracker_test.py` & `upsies-2024.4.12/tests/trackers_test/ptp/ptp_tracker_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,14 +37,18 @@
     assert ptp.PtpTracker.name == 'ptp'
 
 
 def test_label_attribute():
     assert ptp.PtpTracker.label == 'PTP'
 
 
+def test_torrent_source_field_attribute():
+    assert ptp.PtpTracker.torrent_source_field == 'PTP'
+
+
 def test_TrackerConfig_attribute():
     assert ptp.PtpTracker.TrackerConfig is ptp.PtpTrackerConfig
 
 
 def test_TrackerJobs_attribute():
     assert ptp.PtpTracker.TrackerJobs is ptp.PtpTrackerJobs
 
@@ -623,14 +627,22 @@
     assert return_value == exp_return_value
 
 
 @pytest.mark.parametrize(
     argnames='imdb_id, exceptions, response, exp_return_value, exp_mock_calls',
     argvalues=(
         pytest.param(
+            None,
+            {},
+            MockResponse(),
+            None,
+            [],
+            id='No IMDb ID provided',
+        ),
+        pytest.param(
             'tt0123',
             {},
             MockResponse(headers={'location': 'foo.php?id=123456'}),
             '123456',
             [
                 call.login(),
                 call.normalize_imdb_id('tt0123'),
```

### Comparing `upsies-2024.3.9/tests/trackers_test/trackers_test.py` & `upsies-2024.4.12/tests/trackers_test/trackers_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/trackers_test/uhd/uhd_tracker_config_test.py` & `upsies-2024.4.12/tests/trackers_test/uhd/uhd_tracker_config_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 def test_UhdTrackerConfig_defaults(tracker_config):
     assert set(tracker_config) == {
         'base_url',
         'username',
         'password',
         'anonymous',
         'announce_url',
-        'source',
         'image_host',
         'screenshots',
         'exclude',
 
         # Inherited from TrackerConfigBase
         'add_to',
         'copy_to',
@@ -55,18 +54,14 @@
 def test_UhdTrackerConfig_defaults_announce_url(tracker_config):
     assert tracker_config['announce_url'] == ''
     assert tracker_config['announce_url'].description == (
         'Your personal announce URL.'
     )
 
 
-def test_UhdTrackerConfig_defaults_source(tracker_config):
-    assert tracker_config['source'] == '[UHDBits]'
-
-
 def test_UhdTrackerConfig_defaults_image_host(tracker_config, assert_config_list_of_choice):
     exp_options = utils.imghosts.imghost_names()
     assert_config_list_of_choice(
         items=tracker_config['image_host'],
         exp_items=('ptpimg', 'freeimage', 'imgbox'),
         exp_options=exp_options,
         exp_description=(
@@ -115,14 +110,15 @@
         assert set(tracker_config.argument_definitions[command]) == exp_argument_definitions[command]
 
 
 def test_UhdTrackerConfig_argument_definitions_submit_anonymous(tracker_config):
     assert tracker_config.argument_definitions['submit'][('--anonymous', '--an')] == {
         'help': 'Hide your username for this submission',
         'action': 'store_true',
+        'default': None,
     }
 
 
 def test_UhdTrackerConfig_argument_definitions_submit_internal(tracker_config):
     assert tracker_config.argument_definitions['submit'][('--internal', '--in')] == {
         'help': 'Internal encode (use only if you were told to)',
         'action': 'store_true',
```

### Comparing `upsies-2024.3.9/tests/trackers_test/uhd/uhd_tracker_jobs_test.py` & `upsies-2024.4.12/tests/trackers_test/uhd/uhd_tracker_jobs_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -723,14 +723,17 @@
     return_value = await uhd_tracker_jobs.autodetect_source('job_')
     assert return_value is None
 
 
 @pytest.mark.parametrize(
     argnames='source, release, exp_return_value',
     argvalues=(
+        ('Remux', Mock(source='foo BluRay Remux bar'), True),
+        ('Remux', Mock(source='foo DVD Remux bar'), True),
+        ('Remux', Mock(source='foo WEB Remux bar'), True),
         ('Encode', Mock(source='foo BluRay baz'), True),
         ('Encode', Mock(source='foo BluRay baz'), True),
         ('Encode', Mock(source='foo bar baz'), False),
         ('Encode', Mock(source='foo HD-DVD baz'), True),
         ('WEB-DL', Mock(source='foo bar baz'), False),
         ('WEB-DL', Mock(source='foo WEB-DL baz'), True),
         ('WEBRip', Mock(source='foo bar baz'), False),
@@ -925,14 +928,15 @@
 )
 @pytest.mark.asyncio
 async def test_autodetect_tags(
         imdb_id, uhd_info,
         exp_return_value,
         uhd_tracker_jobs, mocker,
 ):
+    mocker.patch.object(type(uhd_tracker_jobs), 'imdb_job', PropertyMock())
     mocker.patch.object(type(uhd_tracker_jobs), 'imdb_id', PropertyMock(return_value=imdb_id))
     mocker.patch.object(uhd_tracker_jobs.tracker, 'get_uhd_info', AsyncMock(return_value=uhd_info))
 
     return_value = await uhd_tracker_jobs.autodetect_tags()
     assert return_value == exp_return_value
     assert uhd_tracker_jobs.tracker.get_uhd_info.call_args_list == [call(uhd_tracker_jobs.imdb_id)]
```

### Comparing `upsies-2024.3.9/tests/trackers_test/uhd/uhd_tracker_test.py` & `upsies-2024.4.12/tests/trackers_test/uhd/uhd_tracker_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import datetime
 import re
 from unittest.mock import AsyncMock, Mock, PropertyMock, call
 
 import bs4
 import pytest
 
 from upsies import __project_name__, errors
@@ -32,14 +31,18 @@
     assert UhdTracker.name == 'uhd'
 
 
 def test_label_attribute():
     assert UhdTracker.label == 'UHD'
 
 
+def test_torrent_source_field_attribute():
+    assert UhdTracker.torrent_source_field == '[UHDBits]'
+
+
 def test_TrackerConfig_attribute():
     assert UhdTracker.TrackerConfig is UhdTrackerConfig
 
 
 def test_TrackerJobs_attribute():
     assert UhdTracker.TrackerJobs is UhdTrackerJobs
 
@@ -346,215 +349,175 @@
     mocks = Mock()
     mocks.attach_mock(mocker.patch.object(tracker, '_get_uhd_info'), '_get_uhd_info')
     mocks.attach_mock(mocker.patch('asyncio.sleep'), 'sleep')
     return mocks
 
 @pytest.mark.asyncio
 async def test_get_uhd_info_with_unknown_imdb_id(mocks_for_get_uhd_info, tracker):
+    tracker.get_uhd_info.clear_cache()
     with pytest.raises(AssertionError, match=r'^IMDb ID is not available yet$'):
         await tracker.get_uhd_info(None)
     assert mocks_for_get_uhd_info.mock_calls == []
 
+@pytest.mark.parametrize('error_type', (int, str), ids=('int', 'str'))
 @pytest.mark.asyncio
-async def test_get_uhd_info_with_readily_available_info(mocks_for_get_uhd_info, tracker):
+async def test_get_uhd_info_with_readily_available_info(error_type, mocks_for_get_uhd_info, tracker):
     imdb_id = 'tt123456'
-    mocks_for_get_uhd_info._get_uhd_info.return_value = {'error': '0', 'the': 'info'}
+    mocks_for_get_uhd_info._get_uhd_info.return_value = {'error': error_type('0'), 'the': 'info'}
 
+    tracker.get_uhd_info.clear_cache()
     return_value = await tracker.get_uhd_info(imdb_id)
-    assert return_value == {'error': '0', 'the': 'info'}
+    assert return_value == {'error': error_type('0'), 'the': 'info'}
     assert mocks_for_get_uhd_info.mock_calls == [
         call._get_uhd_info(imdb_id),
     ]
 
 @pytest.mark.parametrize(
-    argnames='imdb_id, responses, exp_mock_calls',
+    argnames='imdb_id, responses, exp_return_value, exp_mock_calls',
     argvalues=(
         (
             'tt123456',
             (
                 {'error': '1', 'message': 'Fetching'},
                 {'error': '0', 'the': 'info'},
             ),
+            {'error': '0', 'the': 'info'},
             [
                 call._get_uhd_info('tt123456'),
                 call.sleep(6),
                 call._get_uhd_info('tt123456'),
             ],
         ),
         (
             'tt123456',
             (
                 {'error': '1', 'message': 'Fetching'},
                 {'error': '1', 'message': 'Loading'},
-                {'error': '0', 'the': 'info'},
-            ),
-            [
-                call._get_uhd_info('tt123456'),
-                call.sleep(6),
-                call._get_uhd_info('tt123456'),
-                call.sleep(5),
-                call._get_uhd_info('tt123456'),
-            ],
-        ),
-        (
-            'tt123456',
-            (
-                {'error': '1', 'message': 'Fetching'},
-                {'error': '1', 'message': 'Loading'},
                 {'error': '1', 'message': 'Still loading'},
                 {'error': '0', 'the': 'info'},
             ),
+            {'error': '0', 'the': 'info'},
             [
                 call._get_uhd_info('tt123456'),
                 call.sleep(6),
                 call._get_uhd_info('tt123456'),
-                call.sleep(5),
-                call._get_uhd_info('tt123456'),
-                call.sleep(4),
-                call._get_uhd_info('tt123456'),
-            ],
-        ),
-        (
-            'tt123456',
-            (
-                {'error': '1', 'message': 'Fetching'},
-                {'error': '1', 'message': 'Loading'},
-                {'error': '1', 'message': 'Still loading'},
-                {'error': '1', 'message': '...'},
-                {'error': '0', 'the': 'info'},
-            ),
-            [
-                call._get_uhd_info('tt123456'),
-                call.sleep(6),
-                call._get_uhd_info('tt123456'),
-                call.sleep(5),
-                call._get_uhd_info('tt123456'),
-                call.sleep(4),
+                call.sleep(3),
                 call._get_uhd_info('tt123456'),
                 call.sleep(3),
                 call._get_uhd_info('tt123456'),
             ],
         ),
         (
             'tt123456',
             (
                 {'error': '1', 'message': 'Fetching'},
                 {'error': '1', 'message': 'Loading'},
                 {'error': '1', 'message': 'Still loading'},
                 {'error': '1', 'message': '...'},
-                {'error': '1', 'message': '!!!'},
-                {'error': '0', 'the': 'info'},
+                {'error': 'rate limit exceeded', 'status': 'failure'},
             ),
+            {},
             [
                 call._get_uhd_info('tt123456'),
                 call.sleep(6),
                 call._get_uhd_info('tt123456'),
-                call.sleep(5),
-                call._get_uhd_info('tt123456'),
-                call.sleep(4),
+                call.sleep(3),
                 call._get_uhd_info('tt123456'),
                 call.sleep(3),
                 call._get_uhd_info('tt123456'),
                 call.sleep(3),
                 call._get_uhd_info('tt123456'),
             ],
         ),
     ),
     ids=lambda v: repr(v),
 )
+@pytest.mark.parametrize('error_type', (int, str), ids=('int', 'str'))
 @pytest.mark.asyncio
 async def test_get_uhd_info_with_info_getting_fetched_by_server(
-        imdb_id, responses, exp_mock_calls,
+        imdb_id, responses, error_type,
+        exp_return_value, exp_mock_calls,
         mocks_for_get_uhd_info, tracker,
 ):
+    for response in responses:
+        if 'error' in response and str(response['error']).isdecimal():
+            response['error'] = error_type(response['error'])
+    if 'error' in exp_return_value:
+        exp_return_value['error'] = error_type(exp_return_value['error'])
+
     mocks_for_get_uhd_info._get_uhd_info.side_effect = responses
 
+    tracker.get_uhd_info.clear_cache()
     return_value = await tracker.get_uhd_info(imdb_id)
-    assert return_value == responses[-1]
+    assert return_value == exp_return_value
     assert mocks_for_get_uhd_info.mock_calls == exp_mock_calls
 
+@pytest.mark.parametrize('error_type', (int, str), ids=('int', 'str'))
 @pytest.mark.asyncio
-async def test_get_uhd_info_with_server_fetching_too_long(mocks_for_get_uhd_info, tracker):
+async def test_get_uhd_info_with_server_fetching_too_long(error_type, mocks_for_get_uhd_info, tracker):
     imdb_id = 'tt123456'
     mocks_for_get_uhd_info._get_uhd_info.side_effect = (
-        {'error': '1', 'message': 'Fetching'},
-        {'error': '1', 'message': 'Fetching'},
-        {'error': '1', 'message': 'Fetching'},
-        {'error': '1', 'message': 'Fetching'},
-        {'error': '1', 'message': 'Fetching'},
-        {'error': '1', 'message': 'Fetching'},
-        {'error': '1', 'message': 'Fetching'},
-        {'error': '1', 'message': 'Fetching'},
-        {'error': '1', 'message': 'Fetching'},
-        {'error': '1', 'message': 'Fetching'},
-        {'error': '1', 'message': 'Fetching'},
-        {'error': '1', 'message': 'Fetching'},
-    )
+        {'error': error_type('1'), 'message': 'Fetching'},
+    ) * 300
 
+    tracker.get_uhd_info.clear_cache()
     return_value = await tracker.get_uhd_info(imdb_id)
     assert return_value == {}
-    assert mocks_for_get_uhd_info.mock_calls == [
+
+    exp_mock_calls = [
         call._get_uhd_info(imdb_id),
         call.sleep(6),
-        call._get_uhd_info(imdb_id),
-        call.sleep(5),
-        call._get_uhd_info(imdb_id),
-        call.sleep(4),
-        call._get_uhd_info(imdb_id),
-        call.sleep(3),
-        call._get_uhd_info(imdb_id),
-        call.sleep(3),
-        call._get_uhd_info(imdb_id),
-        call.sleep(3),
-        call._get_uhd_info(imdb_id),
-        call.sleep(3),
-        call._get_uhd_info(imdb_id),
-        call.sleep(3),
+    ] + [
         call._get_uhd_info(imdb_id),
         call.sleep(3),
+    ] * 20 * 3 + [
         call._get_uhd_info(imdb_id),
     ]
+    for c, exp_c in zip(mocks_for_get_uhd_info.mock_calls, exp_mock_calls):
+        print(exp_c)
+        print(c)
+        print('---------------------------')
+    assert mocks_for_get_uhd_info.mock_calls == exp_mock_calls
 
+@pytest.mark.parametrize('error_type', (int, str), ids=('int', 'str'))
 @pytest.mark.asyncio
-async def test_get_uhd_info_with_server_request_error(mocks_for_get_uhd_info, tracker):
+async def test_get_uhd_info_with_server_request_error(error_type, mocks_for_get_uhd_info, tracker):
     imdb_id = 'tt123456'
     mocks_for_get_uhd_info._get_uhd_info.side_effect = (
-        {'error': '1', 'message': 'Fetching'},
+        {'error': error_type('1'), 'message': 'Fetching'},
         errors.RequestError('Connection refused'),
     )
 
+    tracker.get_uhd_info.clear_cache()
     return_value = await tracker.get_uhd_info(imdb_id)
     assert return_value == {}
     assert mocks_for_get_uhd_info.mock_calls == [
         call._get_uhd_info(imdb_id),
         call.sleep(6),
         call._get_uhd_info(imdb_id),
     ]
 
 
 @pytest.mark.asyncio
 async def test__get_uhd_info(tracker, mocker):
     imdb_id = 'tt123456'
     mocks = Mock()
     mocks.response.json.return_value = {'the': 'info'}
-    mocks.now.return_value = datetime.datetime(2012, 11, 10, 9, 8, 7, 654321)
-    mocker.patch('datetime.datetime', Mock(now=mocks.now))
     mocks.attach_mock(mocker.patch.object(tracker, '_request', return_value=mocks.response), '_request')
 
+    tracker.get_uhd_info.clear_cache()
     return_value = await tracker._get_uhd_info(imdb_id)
     assert return_value == {'the': 'info'}
     assert mocks.mock_calls == [
-        call.now(datetime.timezone.utc),
         call._request(
             method='GET',
             url=tracker._ajax_url,
             params={
                 'action': 'imdb_fetch',
                 'imdbid': imdb_id,
-                '_': int(mocks.now.return_value.timestamp() * 1000),
             },
         ),
         call.response.json(),
     ]
 
 
 @pytest.fixture
```

### Comparing `upsies-2024.3.9/tests/uis_test/prompts_test.py` & `upsies-2024.4.12/tests/uis_test/prompts_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/uis_test/tui_test/tui_test.py` & `upsies-2024.4.12/tests/uis_test/tui_test/tui_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/uis_test/tui_test/tui_utils_test.py` & `upsies-2024.4.12/tests/uis_test/tui_test/tui_utils_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/uis_test/tui_test/tui_widgets_test.py` & `upsies-2024.4.12/tests/uis_test/tui_test/tui_widgets_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/utils_test/argtypes_test.py` & `upsies-2024.4.12/tests/utils_test/argtypes_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/utils_test/btclient_test.py` & `upsies-2024.4.12/tests/utils_test/btclient_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/utils_test/configfiles_test.py` & `upsies-2024.4.12/tests/utils_test/configfiles_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import configparser
 import os
+import re
 import stat
 from unittest.mock import Mock, call, patch
 
 import pytest
 
 from upsies import errors
 from upsies.utils import configfiles
@@ -73,26 +74,14 @@
     mocker.patch('upsies.utils.configfiles.ConfigFiles._build_types')
     config = configfiles.ConfigFiles(defaults=defaults)
     assert config._cfg == ConfigDict_mock.return_value
     assert ConfigDict_mock.call_args_list == [
         call(defaults, types=config._build_types.return_value),
     ]
 
-def test_ConfigFiles_init_reads_files(mocker):
-    mocker.patch('upsies.utils.configfiles.ConfigFiles.read')
-    config = configfiles.ConfigFiles(
-        defaults={},
-        foo='path/to/foo.ini',
-        bar='path/to/bar.ini',
-    )
-    assert config.read.call_args_list == [
-        call('foo', 'path/to/foo.ini', ignore_missing=False),
-        call('bar', 'path/to/bar.ini', ignore_missing=False),
-    ]
-
 
 def test_ConfigFiles_build_types():
     class Subclass(str):
         pass
 
     d = configfiles.ConfigFiles(defaults={
         'section1': {
@@ -156,23 +145,20 @@
     assert types['section2']['subsection_2']['z'].__name__ == 'SubclassConfigType'
     assert types['section2']['subsection_2']['z'].__qualname__ == 'SubclassConfigType'
     my_assert(types['section2']['subsection_2']['z']('5.3'), '5.3', Subclass)
     my_assert(types['section2']['subsection_2']['z']([5, 3]), '5 3', Subclass)
 
 
 def test_ConfigFiles_files():
-    d = configfiles.ConfigFiles(
-        defaults={},
-        foo='path/to/foo.ini',
-        bar='path/to/bar.ini',
-        ignore_missing=True,
-    )
+    d = configfiles.ConfigFiles(defaults={})
+    d.read('section1', 'path/to/foo.ini', ignore_missing=True)
+    d.read('section2', 'path/to/bar.ini', ignore_missing=True)
     assert d.files == {
-        'foo': 'path/to/foo.ini',
-        'bar': 'path/to/bar.ini',
+        'section1': 'path/to/foo.ini',
+        'section2': 'path/to/bar.ini',
     }
     assert id(d.files) != id(d.files)
 
 
 def test_ConfigFiles_paths():
     d = configfiles.ConfigFiles(defaults={
         'main': {'foo': {'a': 'x'},
@@ -307,14 +293,45 @@
     assert config._set.call_args_list == [
         call('other', 'foo', 'x', 'hello'),
         call('other', 'baz', 'y', 'world'),
     ]
     assert config._files == {'main': file_main, 'other': file_other}
     assert config._defaults == defaults
 
+@pytest.mark.parametrize('ignore_missing', (True, False), ids=lambda v: f'ignore_missing={v!r}')
+def test_ConfigFiles_read_fails_to_update_value(ignore_missing, tmp_path, mocker):
+    defaults = {
+        'main': {'foo': {'a': 'x'},
+                 'bar': {'b': ('x',), 'c': 'x'}},
+        'other': {'foo': {'x': 'asdf'},
+                  'baz': {'y': 'fdsa', 'z': 'qux'}},
+    }
+    file_main = tmp_path / 'file_main.ini'
+    file_main.write_text('[bar]\nc = cee\n\n[foo]\na = z\nno_such_option = ohno\nb = x\n')
+    file_other = tmp_path / 'file_other.ini'
+    file_other.write_text('[foo]\nx = hello\n\n[baz]\ny = world\n')
+
+    def _set(section, subsection_name, option_name, option_value, **kwargs):
+        if option_name == 'no_such_option':
+            raise errors.ConfigError('No such option: no_such_option')
+
+    mocker.patch('upsies.utils.configfiles.ConfigFiles._set', side_effect=_set)
+
+    config = configfiles.ConfigFiles(defaults=defaults)
+
+    with pytest.raises(errors.ConfigError, match=rf'{re.escape(str(file_main))}: No such option: no_such_option$'):
+        config.read('main', file_main, ignore_missing=ignore_missing)
+    assert config._set.call_args_list == [
+        call('main', 'bar', 'c', 'cee'),
+        call('main', 'foo', 'a', 'z'),
+        call('main', 'foo', 'no_such_option', 'ohno'),
+    ]
+    assert config._files == {}
+    assert config._defaults == defaults
+
 
 def test_ConfigFiles_parse_option_outside_of_section():
     with pytest.raises(errors.ConfigError, match=r"^mock/path.ini: Line 1: foo = bar: Option outside of section$"):
         configfiles.ConfigFiles._parse('section1', 'foo = bar\n', 'mock/path.ini')
 
 def test_ConfigFiles_parse_finds_invalid_syntax():
     with pytest.raises(errors.ConfigError, match=r"^mock/path.ini: Line 2: 'foo\\n': Invalid syntax$"):
@@ -525,14 +542,37 @@
         'hey': {
             'you': {'there': ''},
         },
     })
     assert tuple(config) == ('foo', 'hey')
 
 
+def test_ConfigFiles___repr__(tmp_path):
+    config = configfiles.ConfigFiles(defaults={
+        'main': {'foo': {'a': 'x'},
+                 'bar': {'b': ('x',), 'c': 'x'}},
+        'other': {'foo': {'x': 'asdf'},
+                  'baz': {'y': 'fdsa', 'z': 'qux'}},
+    })
+
+    file_main = tmp_path / 'file_main.ini'
+    file_main.write_text('[bar]\nc = cee\n\n[foo]\na = z\n')
+    file_other = tmp_path / 'file_other.ini'
+    file_other.write_text('[foo]\nx = hello\n\n[baz]\ny = world\n')
+
+    config.read('main', file_main)
+    config.read('other', file_other)
+    assert repr(config) == repr({
+        'main': {'foo': {'a': 'z'},
+                 'bar': {'b': ('x',), 'c': 'cee'}},
+        'other': {'foo': {'x': 'hello'},
+                  'baz': {'y': 'world', 'z': 'qux'}},
+    })
+
+
 @pytest.mark.parametrize(
     argnames=('args', 'exp_args'),
     argvalues=(
         ((), ('', '', '')),
         (('foo',), ('foo', '', '')),
         (('foo.bar',), ('foo', 'bar', '')),
         (('foo.bar.baz',), ('foo', 'bar', 'baz')),
@@ -652,23 +692,20 @@
     file1 = tmp_path / 'subdir' / 'subsubdir' / 'file1.ini'
     file2 = tmp_path / 'subdir' / 'subsubdir' / 'file2.ini'
     if files_exist:
         file1.parent.mkdir(parents=True, exist_ok=True)
         file1.write_text('[foo]\nbar = baz\n')
         file2.parent.mkdir(parents=True, exist_ok=True)
         file2.write_text('[foo]\nbar = baz\n')
-    config = configfiles.ConfigFiles(
-        defaults={
-            'File_1': {'foo': {'bar': 'qux'}},
-            'File_2': {'foo': {'bar': 'qux'}},
-        },
-        File_1=file1,
-        File_2=file2,
-        ignore_missing=True,
-    )
+    config = configfiles.ConfigFiles(defaults={
+        'File_1': {'foo': {'bar': 'qux'}},
+        'File_2': {'foo': {'bar': 'qux'}},
+    })
+    config.read('File_1', file1, ignore_missing=True)
+    config.read('File_2', file2, ignore_missing=True)
     config['File_1.foo.bar'] = 'config written'
     config['File_2.foo.bar'] = 'config written'
 
     mocker.patch.object(config, '_as_ini', return_value='<mock config>')
     include_defaults = Mock()
 
     # Make sure umask isn't set so we get expected permissions by default
@@ -714,45 +751,44 @@
         else:
             assert not os.path.exists(f)
 
 @pytest.mark.parametrize(argnames='arg', argvalues=('main', 'main.foo'))
 def test_ConfigFiles_write_extracts_section_from_argument(arg, tmp_path):
     file = tmp_path / 'file1.ini'
     file.write_text('[foo]\nbar = baz\n')
-    config = configfiles.ConfigFiles(
-        defaults={
-            'main': {'foo': {'bar': 'qux'}},
-        },
-        main=file,
-    )
+    config = configfiles.ConfigFiles(defaults={
+        'main': {'foo': {'bar': 'qux'}},
+    })
+    config.read('main', file)
     config['main.foo.bar'] = 'config written'
     config.write(arg)
     assert open(file).read() == '[foo]\nbar = config written\n'
 
 def test_ConfigFiles_write_fails_to_write_file(tmp_path):
     file = tmp_path / 'file1.ini'
     file.write_text('[foo]\nbar = baz\n')
-    config = configfiles.ConfigFiles(
-        defaults={'main': {'foo': {'bar': 'qux'}}},
-        main=file,
-    )
+    config = configfiles.ConfigFiles(defaults={
+        'main': {'foo': {'bar': 'qux'}}
+    })
+    config.read('main', file)
     os.chmod(file, 0o000)
     try:
         with pytest.raises(errors.ConfigError, match=rf'^{file}: Permission denied$'):
             config.write('main')
     finally:
         os.chmod(file, 0o600)
 
 
 def test_ConfigFiles_as_ini():
     config = configfiles.ConfigFiles(
         defaults={'main': {
             'foo': {'a': 'aaa', 'b': [1, 2, 3], 'c': 123},
             'bar': {'b': 'bbb', 'c': [4, 5, 6], 'd': 456},
             'baz': {'c': 'ccc', 'd': [7, 8, 9], 'e': 789},
+            'empty': {},
         }},
     )
     config['main.foo.a'] = 'AAA'
     config['main.bar.c'] = [100, 200, 300]
     config['main.baz.d'] = []
     config['main.baz.e'] = 1000
     assert config._as_ini('main') == (
@@ -762,14 +798,16 @@
         '  200\n'
         '  300\n'
         '\n'
         '[baz]\n'
         'd =\n'
         'e = 1000\n'
         '\n'
+        '[empty]\n'
+        '\n'
         '[foo]\n'
         'a = AAA\n'
     )
     assert config._as_ini('main', include_defaults=True) == (
         '[bar]\n'
         '# b = bbb\n'
         'c =\n'
@@ -779,14 +817,16 @@
         '# d = 456\n'
         '\n'
         '[baz]\n'
         '# c = ccc\n'
         'd =\n'
         'e = 1000\n'
         '\n'
+        '[empty]\n'
+        '\n'
         '[foo]\n'
         'a = AAA\n'
         '# b =\n'
         '#   1\n'
         '#   2\n'
         '#   3\n'
         '# c = 123\n'
```

### Comparing `upsies-2024.3.9/tests/utils_test/country_test.py` & `upsies-2024.4.12/tests/utils_test/country_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/utils_test/daemon_test.py` & `upsies-2024.4.12/tests/utils_test/daemon_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/utils_test/fs_test.py` & `upsies-2024.4.12/tests/utils_test/fs_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/utils_test/html_test.py` & `upsies-2024.4.12/tests/utils_test/html_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/utils_test/http_test/conftest.py` & `upsies-2024.4.12/tests/utils_test/http_test/conftest.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/utils_test/http_test/http_test.py` & `upsies-2024.4.12/tests/utils_test/http_test/http_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1259,59 +1259,139 @@
 def test_get_file_object_returns_fileobj(tmp_path):
     filepath = tmp_path / 'foo'
     filepath.write_bytes(b'hello')
     fileobj = http._get_file_object(filepath)
     assert fileobj.read() == b'hello'
 
 
+@pytest.mark.parametrize(
+    argnames='url, exp_cache_filename',
+    argvalues=(
+        pytest.param(
+            'http://localhost:123/foo',
+            '{method}.http:##localhost:123#foo',
+            id='URL fits into file name',
+        ),
+        pytest.param(
+            'http://localhost:123/foo' + ('o' * 300),
+            '{method}.HTTP:##LOCALHOST:123#FOO' + ('O' * 300),
+            id='URL path is too long',
+        ),
+    ),
+    ids=lambda v: repr(v),
+)
 @pytest.mark.parametrize('method', ('GET', 'POST'))
-def test_cache_file_with_params(method, mocker, tmp_path):
+def test__cache_file_with_no_params_and_no_data(method, url, exp_cache_filename, mocker, tmp_path):
     mocker.patch.object(http, '_get_cache_directory', return_value=str(tmp_path))
 
     def sanitize_filename(filename):
-        return filename.replace('a', '#').replace('A', '#')
+        return filename.replace('/', '#')
 
     mocker.patch('upsies.utils.fs.sanitize_filename', side_effect=sanitize_filename)
 
     def semantic_hash(object):
         return str(object).upper()
 
     mocker.patch('upsies.utils.semantic_hash', side_effect=semantic_hash)
 
-    url = 'http://localhost:123'
-    params = {'foo': 'a b c', 'bar': 12}
-    data = {'this': b'data', 'that': 'text'}
-    exp_cache_file = (
-        str(tmp_path / f'{method.upper()}.')
-        + 'http://loc#lhost:123?foo=#+b+c&b#r=12'
-        + "&this=B'D#T#'&th#t=text"
-    )
-    assert http._cache_file(method, url, params=params, data=data) == exp_cache_file
-
+    exp_cache_file = os.path.join(tmp_path, exp_cache_filename.format(method=method))
+    cache_file = http._cache_file(method, url, params={}, data={})
+    assert cache_file == exp_cache_file
+
+
+@pytest.mark.parametrize(
+    argnames='url, params, data, exp_cache_filename',
+    argvalues=(
+        pytest.param(
+            'http://localhost:123/foo',
+            {'bar': '1 2 3', 'baz': 'abc'},
+            {'mydata': b'hello world'},
+            (
+                '{method}.http:##localhost:123#foo'
+                + '?bar=1+2+3&baz=abc'
+                + '&mydata=' + semantic_hash(b'hello world')
+            ),
+            id='URL, params and data fit into file name',
+        ),
+        pytest.param(
+            'http://localhost:123/foo',
+            {'bar': (1, 2, 3), 'baz': ('abc' * 100)},
+            {
+                'text': 'hello world',
+                'data': b'ello orld'
+            },
+            (
+                '{method}.http:##localhost:123#foo'
+                + '?' + semantic_hash(
+                    {
+                        'bar': (1, 2, 3),
+                        'baz': ('abc' * 100),
+                        'text': 'hello world',
+                        'data': semantic_hash(b'ello orld'),
+                    },
+                )
+            ),
+            id='Params too long',
+        ),
+        pytest.param(
+            'http://localhost:123/foo',
+            {'bar': (1, 2, 3), 'baz': 'abc'},
+            {
+                'text': ', '.join(('hello world' for _ in range(10))),
+                'data': b', '.join((b'ello orld' for _ in range(10))),
+            },
+            (
+                '{method}.http:##localhost:123#foo'
+                + '?' + semantic_hash(
+                    {
+                        'bar': (1, 2, 3),
+                        'baz': 'abc',
+                        'text': ', '.join(('hello world' for _ in range(10))),
+                        'data': semantic_hash(b', '.join((b'ello orld' for _ in range(10)))),
+                    },
+                )
+            ),
+            id='Data too long',
+        ),
+        pytest.param(
+            'http://localhost:123/foo',
+            {'bar': (1, 2, 3), 'baz': ('abc' * 60)},
+            {
+                'text': ', '.join(('hello world' for _ in range(10))),
+                'data': b', '.join((b'ello orld' for _ in range(10))),
+            },
+            (
+                '{method}.http:##localhost:123#foo'
+                + '?' + semantic_hash(
+                    {
+                        'bar': (1, 2, 3),
+                        'baz': ('abc' * 60),
+                        'text': ', '.join(('hello world' for _ in range(10))),
+                        'data': semantic_hash(b', '.join((b'ello orld' for _ in range(10)))),
+                    },
+                )
+            ),
+            id='Params and data too long',
+        ),
+    ),
+    ids=lambda v: repr(v),
+)
 @pytest.mark.parametrize('method', ('GET', 'POST'))
-def test_cache_file_with_very_long_params(method, mocker, tmp_path):
+def test__cache_file_with_params_and_data(url, params, data, exp_cache_filename, method, mocker, tmp_path):
+    mocker.patch.object(http, '_get_cache_directory', return_value=str(tmp_path))
+
     def sanitize_filename(filename):
-        return filename.replace('a', '#')
+        return filename.replace('/', '#')
 
     mocker.patch('upsies.utils.fs.sanitize_filename', side_effect=sanitize_filename)
-    mocker.patch.object(http, '_get_cache_directory', return_value=tmp_path)
-    url = 'http://localhost:123'
-    params = {'foo': 'a b c ' * 100, 'bar': 12}
-    data = {'this': b'data' * 100, 'that': 'text' * 20}
-    exp_params_and_data = {
-        **params,
-        **data,
-        **{'this': semantic_hash(b'data' * 100)},  # Override "this" in `data`
-    }
-    exp_cache_file = (
-        str(tmp_path / f'{method.upper()}.')
-        + 'http://loc#lhost:123?'
-        + semantic_hash(exp_params_and_data)
-    )
-    assert http._cache_file(method, url, params=params, data=data) == exp_cache_file
+
+    exp_cache_file = os.path.join(tmp_path, exp_cache_filename.format(method=method))
+    cache_file = http._cache_file(method, url, params=params, data=data)
+    assert cache_file == exp_cache_file
+
 
 def test_from_cache_with_nonexisting_cache_file():
     assert http._from_cache('/no/such/path') is None
 
 def test_from_cache_with_unreadable_cache_file(tmp_path):
     cache_filepath = tmp_path / 'cache_file'
     cache_filepath.write_text('mock data')
```

### Comparing `upsies-2024.3.9/tests/utils_test/http_test/http_tls_test.py` & `upsies-2024.4.12/tests/utils_test/http_test/http_tls_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/utils_test/image_optimize_test.py` & `upsies-2024.4.12/tests/utils_test/image_optimize_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/utils_test/image_resize_test.py` & `upsies-2024.4.12/tests/utils_test/image_resize_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/utils_test/image_screenshot_test.py` & `upsies-2024.4.12/tests/utils_test/image_screenshot_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,16 @@
         pytest.param(
             'video.mkv', 123, 'foo%.png', 'BT.2020',
             (
                 '-y', '-hide_banner', '-loglevel', 'error',
                 '-ss', '123',
                 '-i', 'ffmpeg_input:video.mkv',
                 '-vf', ':'.join((
-                    'scale=in_h_chr_pos=0',
+                    "scale='max(sar,1)*iw':'max(1/sar,1)*ih'",
+                    'in_h_chr_pos=0',
                     'in_v_chr_pos=0',
                     'in_color_matrix=bt2020',
                     'flags=' + '+'.join(VF_FLAGS),
                 )),
                 '-pix_fmt', 'rgb24', '-vframes', '1',
                 'file:foo%%.png',
             ),
```

### Comparing `upsies-2024.3.9/tests/utils_test/imghosts_test/freeimage_test.py` & `upsies-2024.4.12/tests/utils_test/imghosts_test/freeimage_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/utils_test/imghosts_test/imgbb_test.py` & `upsies-2024.4.12/tests/utils_test/imghosts_test/imgbb_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/utils_test/imghosts_test/imgbox_test.py` & `upsies-2024.4.12/tests/utils_test/imghosts_test/imgbox_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/utils_test/imghosts_test/imghost_base_test.py` & `upsies-2024.4.12/tests/utils_test/imghosts_test/imghost_base_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/utils_test/imghosts_test/imghost_common_test.py` & `upsies-2024.4.12/tests/utils_test/imghosts_test/imghost_common_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/utils_test/imghosts_test/imghost_test.py` & `upsies-2024.4.12/tests/utils_test/imghosts_test/imghost_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/utils_test/imghosts_test/ptpimg_test.py` & `upsies-2024.4.12/tests/utils_test/imghosts_test/ptpimg_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/utils_test/predbs_test/conftest.py` & `upsies-2024.4.12/tests/utils_test/predbs_test/conftest.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/utils_test/predbs_test/corruptnet_test.py` & `upsies-2024.4.12/tests/utils_test/predbs_test/corruptnet_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/utils_test/predbs_test/predbclub_test.py` & `upsies-2024.4.12/tests/utils_test/predbs_test/predbclub_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/utils_test/predbs_test/predbde_test.py` & `upsies-2024.4.12/tests/utils_test/predbs_test/predbde_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/utils_test/predbs_test/predbovh_test.py` & `upsies-2024.4.12/tests/utils_test/predbs_test/predbovh_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/utils_test/predbs_test/predbs_base_test.py` & `upsies-2024.4.12/tests/utils_test/predbs_test/predbs_base_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/utils_test/predbs_test/predbs_common_test.py` & `upsies-2024.4.12/tests/utils_test/predbs_test/predbs_common_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/utils_test/predbs_test/predbs_integration_test.py` & `upsies-2024.4.12/tests/utils_test/predbs_test/predbs_integration_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/utils_test/predbs_test/predbs_multi_test.py` & `upsies-2024.4.12/tests/utils_test/predbs_test/predbs_multi_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/utils_test/predbs_test/predbs_test.py` & `upsies-2024.4.12/tests/utils_test/predbs_test/predbs_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/utils_test/predbs_test/srrdb_test.py` & `upsies-2024.4.12/tests/utils_test/predbs_test/srrdb_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/utils_test/release_episodes_test.py` & `upsies-2024.4.12/tests/utils_test/release_episodes_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/utils_test/release_info_test.py` & `upsies-2024.4.12/tests/utils_test/release_info_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/utils_test/release_name_test.py` & `upsies-2024.4.12/tests/utils_test/release_name_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1099,14 +1099,36 @@
     ReleaseInfo_mock.return_value = {'group': 'ASDF'}
     assert ReleaseName('path/to/something').group == 'ASDF'
     ReleaseInfo_mock.return_value = {'release_group': ''}
     assert ReleaseName('path/to/something').group == 'NOGROUP'
     ReleaseInfo_mock.return_value = {}
     assert ReleaseName('path/to/something').group == 'NOGROUP'
 
+@pytest.mark.parametrize('modifier', (
+    lambda group: group,
+    lambda group: group.lower(),
+    lambda group: group.upper(),
+))
+@pytest.mark.parametrize(
+    argnames='group, exp_group',
+    argvalues=(
+        ('NoGroup', 'NOGROUP'),
+        ('NoGrp', 'NOGROUP'),
+        ('', 'NOGROUP'),
+        (None, 'NOGROUP'),
+    ),
+)
+def test_group_getter_nogroup(modifier, group, exp_group, mocker):
+    ReleaseInfo_mock = mocker.patch('upsies.utils.release.ReleaseInfo', new_callable=lambda: Mock(return_value={}))
+    if group is None:
+        ReleaseInfo_mock.return_value = {}
+    else:
+        ReleaseInfo_mock.return_value = {'group': modifier(group)}
+    assert ReleaseName('path/to/something').group == exp_group
+
 @patch('upsies.utils.release.ReleaseInfo', new_callable=lambda: Mock(return_value={}))
 def test_group_setter(ReleaseInfo_mock):
     rn = ReleaseName('path/to/something')
     assert rn.group == 'NOGROUP'
     rn.group = 'ASDF'
     assert rn.group == 'ASDF'
     rn.group = ''
@@ -1528,15 +1550,15 @@
         (ReleaseType.episode, True),
     ),
 )
 @pytest.mark.parametrize(
     argnames='resolution, dvd_encoding, exp_resolution',
     argvalues=(
         ('123p', None, '123p'),
-        ('123p', 'NTSC-PAL', 'NTSC-PAL'),
+        ('123p', 'NTSCPAL', 'NTSCPAL'),
     ),
 )
 @pytest.mark.parametrize(
     argnames='separator_attribute, separator_argument, exp_separator',
     argvalues=(
         (' ', None, ' '),
         (' ', '.', '.'),
@@ -1587,15 +1609,15 @@
         attributes, exp_release_name,
         mocker,
 ):
     rn = ReleaseName('irrelevant/path/to/content')
 
     static_attributes = {
         'episodes': 'S__E__',
-        'source': 'DLRip',
+        'source': 'WEB-DL',
         'video_format': 'VC',
         'group': 'ASDF',
     }
     for name, value in static_attributes.items():
         mocker.patch.object(type(rn), name, PropertyMock(return_value=value))
     for name, value in attributes.items():
         mocker.patch.object(type(rn), name, PropertyMock(return_value=value))
```

### Comparing `upsies-2024.3.9/tests/utils_test/signal_test.py` & `upsies-2024.4.12/tests/utils_test/signal_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/utils_test/string_test.py` & `upsies-2024.4.12/tests/utils_test/string_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/utils_test/subproc_test.py` & `upsies-2024.4.12/tests/utils_test/subproc_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/utils_test/subtitle_test.py` & `upsies-2024.4.12/tests/utils_test/subtitle_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/utils_test/timestamp_test.py` & `upsies-2024.4.12/tests/utils_test/timestamp_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/utils_test/torrent_test.py` & `upsies-2024.4.12/tests/utils_test/torrent_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/utils_test/types_test.py` & `upsies-2024.4.12/tests/utils_test/types_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/utils_test/update_test.py` & `upsies-2024.4.12/tests/utils_test/update_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/utils_test/utils_test.py` & `upsies-2024.4.12/tests/utils_test/utils_test.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+import random
 import re
 from unittest.mock import AsyncMock, Mock, call
 
 import pytest
 
 from upsies import errors, utils
 
@@ -386,7 +387,104 @@
 )
 @pytest.mark.asyncio
 async def test_run_async(args, kwargs):
     function = Mock()
     return_value = await utils.run_async(function, *args, **kwargs)
     assert return_value == function.return_value
     assert function.call_args_list == [call(*args, **kwargs)]
+
+
+async def test_blocking_memoize():
+    calls = []
+
+    @utils.blocking_memoize
+    async def get_this(what, why='iDunno'):
+        calls.append(('get_this', what, why))
+        await asyncio.sleep(random.random() / 10)
+        print('called get_this() with', (what, why))
+        return f'Here you go: {what} (because: {why})'
+
+    @utils.blocking_memoize
+    async def get_that(item, butnot=()):
+        calls.append(('get_that', item, butnot))
+        await asyncio.sleep(random.random() / 10)
+        print('called get_that() with', (item, butnot))
+        return f'There you are: {item} (excluding: {butnot})'
+
+    coros = [
+        get_this('foo'),
+        get_this('foo'),
+        get_this('foo'),
+
+        get_this('bar', why='iWanna'),
+        get_this('bar', why='iWanna'),
+        get_this('bar', why='iWanna'),
+
+        get_this('baz'),
+        get_this('baz'),
+        get_this('baz'),
+
+        get_that('foo'),
+        get_that('foo'),
+        get_that('foo'),
+
+        get_that('bar', butnot=('arf',)),
+        get_that('bar', butnot=('arf',)),
+        get_that('bar', butnot=('arf', 'arf2')),
+
+        get_that('baz'),
+        get_that('baz'),
+        get_that('baz'),
+    ]
+    random.shuffle(coros)
+    results = await asyncio.gather(*coros)
+
+    assert sorted(calls) == sorted((
+        ('get_this', 'foo', 'iDunno'),
+        ('get_this', 'bar', 'iWanna'),
+        ('get_this', 'baz', 'iDunno'),
+        ('get_that', 'foo', ()),
+        ('get_that', 'bar', ('arf',)),
+        ('get_that', 'bar', ('arf', 'arf2')),
+        ('get_that', 'baz', ()),
+    ))
+
+    assert sorted(results) == sorted((
+        'Here you go: foo (because: iDunno)',
+        'Here you go: foo (because: iDunno)',
+        'Here you go: foo (because: iDunno)',
+
+        'Here you go: bar (because: iWanna)',
+        'Here you go: bar (because: iWanna)',
+        'Here you go: bar (because: iWanna)',
+
+        'Here you go: baz (because: iDunno)',
+        'Here you go: baz (because: iDunno)',
+        'Here you go: baz (because: iDunno)',
+
+        'There you are: foo (excluding: ())',
+        'There you are: foo (excluding: ())',
+        'There you are: foo (excluding: ())',
+
+        "There you are: bar (excluding: ('arf',))",
+        "There you are: bar (excluding: ('arf',))",
+        "There you are: bar (excluding: ('arf', 'arf2'))",
+
+        'There you are: baz (excluding: ())',
+        'There you are: baz (excluding: ())',
+        'There you are: baz (excluding: ())',
+    ))
+
+    get_this.clear_cache()
+    assert await get_this('foo') == 'Here you go: foo (because: iDunno)'
+    assert await get_that('foo') == 'There you are: foo (excluding: ())'
+
+    assert sorted(calls) == sorted((
+        ('get_this', 'foo', 'iDunno'),
+        ('get_this', 'bar', 'iWanna'),
+        ('get_this', 'baz', 'iDunno'),
+        ('get_that', 'foo', ()),
+        ('get_that', 'bar', ('arf',)),
+        ('get_that', 'bar', ('arf', 'arf2')),
+        ('get_that', 'baz', ()),
+        ('get_this', 'foo', 'iDunno'),  # <-- New call because cache was cleared.
+    ))
```

### Comparing `upsies-2024.3.9/tests/utils_test/video_test.py` & `upsies-2024.4.12/tests/utils_test/video_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/utils_test/webdbs_test/conftest.py` & `upsies-2024.4.12/tests/utils_test/webdbs_test/conftest.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/utils_test/webdbs_test/imdb_test.py` & `upsies-2024.4.12/tests/utils_test/webdbs_test/imdb_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/utils_test/webdbs_test/tmdb_test.py` & `upsies-2024.4.12/tests/utils_test/webdbs_test/tmdb_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -77,18 +77,18 @@
     for result in results:
         assert isinstance(result, SearchResult)
 
 
 @pytest.mark.parametrize(
     argnames=('query', 'exp_result'),
     argvalues=(
-        (Query('alien', year='1979'), {'title': 'Alien', 'year': '1979'}),
-        (Query('alien', year='1986'), {'title': 'Aliens', 'year': '1986'}),
-        (Query('january', year='2012'), {'title': 'One Day in January', 'year': '2012'}),
-        (Query('january', year='2015'), {'title': 'January Hymn', 'year': '2015'}),
+        (Query('alien', year='1979', type=ReleaseType.movie), {'title': 'Alien', 'year': '1979'}),
+        (Query('alien', year='1986', type=ReleaseType.movie), {'title': 'Aliens', 'year': '1986'}),
+        (Query('january', year='2012', type=ReleaseType.movie), {'title': 'One Day in January', 'year': '2012'}),
+        (Query('january', year='2015', type=ReleaseType.movie), {'title': 'January Hymn', 'year': '2015'}),
     ),
     ids=lambda value: str(value),
 )
 @pytest.mark.asyncio
 async def test_search_for_year(query, exp_result, api, store_response):
     results = await api.search(query)
     results_title_year = [
@@ -97,16 +97,16 @@
     ]
     assert exp_result in results_title_year
 
 
 @pytest.mark.parametrize(
     argnames=('query', 'exp_titles'),
     argvalues=(
-        (Query('Ash vs Evil Dead', type=ReleaseType.series), ('Ash vs Evil Dead',)),
-        (Query('Ash vs Evil Dead', type=ReleaseType.movie), ()),
+        (Query('Lost & Found Music Studios', type=ReleaseType.series), ('Lost & Found Music Studios',)),
+        (Query('Lost & Found Music Studios', type=ReleaseType.movie), ()),
         (Query('Deadwood', type=ReleaseType.movie), ('Deadwood: The Movie',)),
         (Query('Deadwood', type=ReleaseType.series), ('Deadwood',)),
     ),
     ids=lambda value: str(value),
 )
 @pytest.mark.asyncio
 async def test_search_for_type(query, exp_titles, api, store_response):
@@ -118,17 +118,17 @@
     else:
         assert not titles
 
 
 @pytest.mark.parametrize(
     argnames=('query', 'exp_cast'),
     argvalues=(
-        (Query('The Blues Brothers', year=1980), ('Dan Aykroyd', 'John Belushi')),
-        (Query('February', year=2017), ('Ana Sofrenović', 'Aleksandar Đurica', 'Sonja Kolačarić')),
-        (Query('Deadwood', year=2004), ('Timothy Olyphant', 'Ian McShane')),
+        (Query('The Blues Brothers', year=1980, type=ReleaseType.movie), ('Dan Aykroyd', 'John Belushi')),
+        (Query('February', year=2017, type=ReleaseType.movie), ('Ana Sofrenović', 'Aleksandar Đurica', 'Sonja Kolačarić')),
+        (Query('Deadwood', year=2004, type=ReleaseType.series), ('Timothy Olyphant', 'Ian McShane')),
     ),
     ids=lambda value: str(value),
 )
 @pytest.mark.asyncio
 async def test_search_result_cast(query, exp_cast, api, store_response):
     results = await api.search(query)
     result = [r for r in results if r.title == query.title][0]
@@ -144,48 +144,48 @@
         countries = await result.countries()
         assert countries == ()
 
 
 @pytest.mark.parametrize(
     argnames=('query', 'exp_id'),
     argvalues=(
-        (Query('The Blues Brothers', year=1980), 'movie/525'),
-        (Query('February', year=2017), 'movie/700711'),
-        (Query('Deadwood', year=2004), 'tv/1406'),
+        (Query('The Blues Brothers', year=1980, type=ReleaseType.movie), 'movie/525'),
+        (Query('February', year=2017, type=ReleaseType.movie), 'movie/700711'),
+        (Query('Deadwood', year=2004, type=ReleaseType.series), 'tv/1406'),
     ),
     ids=lambda value: str(value),
 )
 @pytest.mark.asyncio
 async def test_search_result_id(query, exp_id, api, store_response):
     results = await api.search(query)
     result = [r for r in results if r.title == query.title][0]
     assert result.id == exp_id
 
 
 @pytest.mark.parametrize(
     argnames=('query', 'exp_directors'),
     argvalues=(
-        (Query('The Blues Brothers', year=1980), ('John Landis',)),
-        (Query('Deadwood', year=2004), ()),
+        (Query('The Blues Brothers', year=1980, type=ReleaseType.movie), ('John Landis',)),
+        (Query('Deadwood', year=2004, type=ReleaseType.series), ()),
     ),
     ids=lambda value: str(value),
 )
 @pytest.mark.asyncio
 async def test_search_result_directors(query, exp_directors, api, store_response):
     results = await api.search(query)
     assert await results[0].directors() == exp_directors
 
 
 @pytest.mark.parametrize(
     argnames=('query', 'exp_genres'),
     argvalues=(
-        (Query('The Blues Brothers', year=1980), ('music', 'comedy', 'action', 'crime')),
-        (Query('February', year=2017), ('drama',)),
-        (Query('Deadwood', year=2004), ('crime', 'western')),
-        (Query('Farang', year=2017), ('drama',)),
+        (Query('The Blues Brothers', year=1980, type=ReleaseType.movie), ('music', 'comedy', 'action', 'crime')),
+        (Query('February', year=2017, type=ReleaseType.movie), ('drama',)),
+        (Query('Deadwood', year=2004, type=ReleaseType.series), ('crime', 'western')),
+        (Query('Farang', year=2017, type=ReleaseType.series), ('drama',)),
     ),
     ids=lambda value: str(value),
 )
 @pytest.mark.asyncio
 async def test_search_result_genres(query, exp_genres, api, store_response):
     results = await api.search(query)
     result = [r for r in results if r.title == query.title][0]
@@ -196,19 +196,19 @@
     else:
         assert not genres
 
 
 @pytest.mark.parametrize(
     argnames=('query', 'exp_summary'),
     argvalues=(
-        (Query('The Blues Brothers', year=1980), 'released from prison'),
-        (Query('February', year='2017'), 'Husband and wife are going to their vacation cottage to overcome marriage crises'),
-        (Query('Deadwood', year=2004), 'woven around actual historic events'),
-        (Query('Lost & Found Music Studios', year=2015), 'singers-songwriters in an elite music program form bonds of friendship'),
-        (Query('January', year=1973), ''),
+        (Query('The Blues Brothers', year=1980, type=ReleaseType.movie), 'released from prison'),
+        (Query('February', year=2017, type=ReleaseType.movie), 'Husband and wife are going to their vacation cottage to overcome marriage crises'),
+        (Query('Deadwood', year=2004, type=ReleaseType.series), 'woven around actual historic events'),
+        (Query('Lost & Found Music Studios', year=2015, type=ReleaseType.series), 'singers-songwriters in an elite music program form bonds of friendship'),
+        (Query('January', year=1973, type=ReleaseType.movie), ''),
     ),
     ids=lambda value: str(value),
 )
 @pytest.mark.asyncio
 async def test_search_result_summary(query, exp_summary, api, store_response):
     results = await api.search(query)
     result = [r for r in results if r.title == query.title][0]
@@ -218,94 +218,95 @@
     else:
         assert summary == ''
 
 
 @pytest.mark.parametrize(
     argnames=('query', 'exp_title'),
     argvalues=(
-        (Query('Blues Brothers', year=1980), 'The Blues Brothers'),
-        (Query('February', year=2017), "The Blackcoat's Daughter"),
+        (Query('Blues Brothers', year=1980, type=ReleaseType.movie), 'The Blues Brothers'),
+        (Query('February', year=2017, type=ReleaseType.movie), "The Blackcoat's Daughter"),
+        (Query('Seytan goz qabaginda', year=1987, type=ReleaseType.movie), 'The Devil under the Windshield'),
     ),
     ids=lambda value: str(value),
 )
 @pytest.mark.asyncio
 async def test_search_result_title(query, exp_title, api, store_response):
     results = await api.search(query)
     titles = [r.title for r in results]
     assert exp_title in titles
 
 
 @pytest.mark.parametrize(
     argnames=('query', 'exp_title_english'),
     argvalues=(
-        (Query('The Blues Brothers', year=1980), ''),
-        (Query('Deadwood', year=2004), ''),
-        (Query('Le dolci signore', year=1968), 'Anyone Can Play'),
+        (Query('The Blues Brothers', year=1980, type=ReleaseType.movie), ''),
+        (Query('Deadwood', year=2004, type=ReleaseType.series), ''),
+        (Query('Le dolci signore', year=1968, type=ReleaseType.movie), 'Anyone Can Play'),
     ),
     ids=lambda value: str(value),
 )
 @pytest.mark.asyncio
 async def test_search_result_title_english(query, exp_title_english, api, store_response):
     results = await api.search(query)
     assert await results[0].title_english() == exp_title_english
 
 
 @pytest.mark.parametrize(
     argnames=('query', 'exp_title_original'),
     argvalues=(
-        (Query('The Blues Brothers', year=1980), 'The Blues Brothers'),
-        (Query('Deadwind', year=2018), 'Karppi'),
-        (Query('Anyone Can Play', year=1968), 'Le dolci signore'),
+        (Query('The Blues Brothers', year=1980, type=ReleaseType.movie), 'The Blues Brothers'),
+        (Query('Deadwind', year=2018, type=ReleaseType.series), 'Karppi'),
+        (Query('Anyone Can Play', year=1968, type=ReleaseType.movie), 'Le dolci signore'),
     ),
     ids=lambda value: str(value),
 )
 @pytest.mark.asyncio
 async def test_search_result_title_original(query, exp_title_original, api, store_response):
     results = await api.search(query)
     assert await results[0].title_original() == exp_title_original
 
 
 @pytest.mark.parametrize(
     argnames=('query', 'exp_type'),
     argvalues=(
-        (Query('The Blues Brothers', year=1980), ReleaseType.movie),
-        (Query('February', year=2017), ReleaseType.movie),
-        (Query('Deadwood', year=2004), ReleaseType.series),
+        (Query('The Blues Brothers', year=1980, type=ReleaseType.movie), ReleaseType.movie),
+        (Query('February', year=2017, type=ReleaseType.movie), ReleaseType.movie),
+        (Query('Deadwood', year=2004, type=ReleaseType.series), ReleaseType.series),
     ),
     ids=lambda value: str(value),
 )
 @pytest.mark.asyncio
 async def test_search_result_type(query, exp_type, api, store_response):
     results = await api.search(query)
     results_dict = {r.title: r for r in results}
     assert results_dict[query.title].type == exp_type
 
 
 @pytest.mark.parametrize(
     argnames=('query', 'exp_url'),
     argvalues=(
-        (Query('The Blues Brothers', year=1980), 'http://themoviedb.org/movie/525'),
-        (Query('February', year=2017), 'http://themoviedb.org/movie/700711'),
-        (Query('Deadwood', year=2004), 'http://themoviedb.org/tv/1406'),
+        (Query('The Blues Brothers', year=1980, type=ReleaseType.movie), 'http://themoviedb.org/movie/525'),
+        (Query('February', year=2017, type=ReleaseType.movie), 'http://themoviedb.org/movie/700711'),
+        (Query('Deadwood', year=2004, type=ReleaseType.series), 'http://themoviedb.org/tv/1406'),
     ),
     ids=lambda value: str(value),
 )
 @pytest.mark.asyncio
 async def test_search_result_url(query, exp_url, api, store_response):
     results = await api.search(query)
     results_urls = [r.url for r in results]
     assert exp_url in results_urls
 
 
 @pytest.mark.parametrize(
     argnames=('query', 'exp_title', 'exp_year'),
     argvalues=(
-        (Query('Blues Brothers', year=1980), 'The Blues Brothers', '1980'),
-        (Query('February', year='2017'), "The Blackcoat's Daughter", '2017'),
-        (Query('Deadwood', year=2004), 'Deadwood', '2004'),
+        (Query('Blues Brothers', year=1980, type=ReleaseType.movie), 'The Blues Brothers', '1980'),
+        (Query('February', year=2017, type=ReleaseType.movie), "The Blackcoat's Daughter", '2017'),
+        (Query('Deadwood', year=2004, type=ReleaseType.series), 'Deadwood', '2004'),
     ),
     ids=lambda value: str(value),
 )
 @pytest.mark.asyncio
 async def test_search_result_year(query, exp_title, exp_year, api, store_response):
     results = await api.search(query)
     results_dict = {r.title: r for r in results}
@@ -383,15 +384,15 @@
             assert person.url == url
 
 
 @pytest.mark.parametrize(
     argnames=('id', 'exp_directors'),
     argvalues=(
         ('movie/125244', (('James Algar', 'http://themoviedb.org/person/5690-james-algar'),)),
-        ('movie/334536', (('Oz Perkins', 'http://themoviedb.org/person/90609-oz-perkins'),)),
+        ('movie/334536', (('Osgood Perkins', 'http://themoviedb.org/person/90609-osgood-perkins'),)),
         ('tv/1406', ()),
         ('tv/74802', ()),
         (None, ()),
     ),
     ids=lambda value: str(value),
 )
 @pytest.mark.asyncio
@@ -484,19 +485,19 @@
         # The Blues Brothers
         ('movie/525', 77.0),
         # The Blackcoat's Daughter
         ('movie/334536', 58.0),
         # Deadwood
         ('tv/1406', 81.0),
         # Karppi
-        ('tv/74802', 68.0),
+        ('tv/74802', 69.0),
         # Lost & Found Music Studios
         ('tv/66260', 82.0),
         # Le dolci signore
-        ('movie/3405', 18.0),
+        ('movie/3405', 39.0),
         (None, None),
     ),
     ids=lambda value: str(value),
 )
 @pytest.mark.asyncio
 async def test_rating(id, exp_rating, api, store_response):
     rating = await api.rating(id)
```

### Comparing `upsies-2024.3.9/tests/utils_test/webdbs_test/tvmaze_test.py` & `upsies-2024.4.12/tests/utils_test/webdbs_test/tvmaze_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/utils_test/webdbs_test/webdbs_base_test.py` & `upsies-2024.4.12/tests/utils_test/webdbs_test/webdbs_base_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/tests/utils_test/webdbs_test/webdbs_common_test.py` & `upsies-2024.4.12/tests/utils_test/webdbs_test/webdbs_common_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -109,14 +109,27 @@
 
     for _ in range(3):
         q.id = 'tt12345'
         assert q.id == 'tt12345'
         assert cb.mock_calls == [call(q), call(q)]
 
 
+def test_Query_feeling_lucky():
+    q = webdbs.Query('The Title', feeling_lucky=1)
+    cb = Mock()
+    q.signal.register('changed', cb)
+    assert q.feeling_lucky is True
+    assert cb.mock_calls == []
+
+    for _ in range(3):
+        q.feeling_lucky = 0
+        assert q.feeling_lucky is False
+        assert cb.mock_calls == [call(q)]
+
+
 @pytest.mark.parametrize('silent', (False, True))
 def test_Query_update(silent):
     q = webdbs.Query('The Title', type=ReleaseType.series)
     cb = Mock()
     q.signal.register('changed', cb)
     assert cb.call_args_list == []
 
@@ -136,14 +149,19 @@
         assert cb.call_args_list == [] if silent else [call(q), call(q), call(q)]
 
     for _ in range(3):
         q.update(webdbs.Query('The Title', id='123', year='2015', type=ReleaseType.episode), silent=silent)
         assert str(q) == 'id:123'
         assert cb.call_args_list == [] if silent else [call(q), call(q), call(q), call(q)]
 
+    for _ in range(3):
+        q.update(webdbs.Query('The Title', feeling_lucky=True), silent=silent)
+        assert str(q) == '!The Title'
+        assert cb.call_args_list == [] if silent else [call(q), call(q), call(q), call(q), call(q)]
+
 
 def test_Query_copy():
     q = webdbs.Query('The Title', year='2010', type=ReleaseType.series, id='1234')
     cb = Mock()
     q.signal.register('changed', cb)
     assert cb.call_args_list == []
 
@@ -178,14 +196,23 @@
     assert q.copy(id='4321') == webdbs.Query(
         title='The Title',
         year='2010',
         type=ReleaseType.series,
         id='4321',
     )
 
+    # Query doesn't change if we're feeling lucky.
+    assert q.copy(feeling_lucky=True) == webdbs.Query(
+        title='The Title',
+        year='2010',
+        type=ReleaseType.series,
+        id='1234',
+        feeling_lucky=False,
+    )
+
     assert cb.call_args_list == []
 
 @pytest.mark.parametrize(
     argnames=('a', 'b'),
     argvalues=(
         (webdbs.Query('The Title'), webdbs.Query('The Title')),
         (webdbs.Query('The Title'), webdbs.Query('the title')),
@@ -236,14 +263,15 @@
 )
 def test_Query_as_string(query, exp_string):
     assert str(query) == exp_string
 
 @pytest.mark.parametrize(
     argnames=('string', 'exp_result'),
     argvalues=(
+        ('', webdbs.Query('')),
         ('The Title', webdbs.Query('The Title')),
         ('The Title type:movie', webdbs.Query('The Title', type=ReleaseType.movie)),
         ('The Title type:season', webdbs.Query('The Title', type=ReleaseType.season)),
         ('The Title type:episode', webdbs.Query('The Title', type=ReleaseType.episode)),
         ('The Title type:series', webdbs.Query('The Title', type=ReleaseType.series)),
         ('The Title type:film', webdbs.Query('The Title', type=ReleaseType.movie)),
         ('The Title type:tv', webdbs.Query('The Title', type=ReleaseType.series)),
@@ -256,14 +284,15 @@
         ('The Title year:123', ValueError('Invalid year: 123')),
         ('The Title year:foo', ValueError('Invalid year: foo')),
         ('The Title type:movie year:2000', webdbs.Query('The Title', type=ReleaseType.movie, year='2000')),
         ('The Title year:2003 type:series', webdbs.Query('The Title', type=ReleaseType.series, year='2003')),
         ('The Title id:foo', webdbs.Query('The Title', id='foo')),
         ('id:foo', webdbs.Query(id='foo')),
         ('id:foo year:2005', webdbs.Query(id='foo', year='2005')),
+        ('!id:foo', webdbs.Query(id='foo', feeling_lucky=True)),
         ('The Title id: type: year:', webdbs.Query('The Title')),
         ('The Title Id:foo Type:bar Year:baz', webdbs.Query('The Title Id:foo Type:bar Year:baz')),
     ),
     ids=lambda v: str(v),
 )
 def test_Query_from_string(string, exp_result):
     if isinstance(exp_result, Exception):
@@ -350,14 +379,16 @@
          "Query(title='The Title', type=ReleaseType.movie)"),
         (webdbs.Query('The Title', year='1999'),
          "Query(title='The Title', year='1999')"),
         (webdbs.Query('The Title', type=ReleaseType.season, year='1999'),
          "Query(title='The Title', year='1999', type=ReleaseType.season)"),
         (webdbs.Query('The Title', type=ReleaseType.season, year='1999', id='123'),
          "Query(title='The Title', year='1999', type=ReleaseType.season, id='123')"),
+        (webdbs.Query(id='123', feeling_lucky=True),
+         "Query(id='123', feeling_lucky=True)"),
     ),
     ids=lambda value: str(value),
 )
 def test_Query_as_repr(query, exp_repr):
     assert repr(query) == exp_repr
```

### Comparing `upsies-2024.3.9/tests/utils_test/webdbs_test/webdbs_test.py` & `upsies-2024.4.12/tests/utils_test/webdbs_test/webdbs_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/__init__.py` & `upsies-2024.4.12/upsies/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __project_name__ = 'upsies'
 __description__ = 'Media metadata aggregator'
 __homepage__ = 'https://upsies.readthedocs.io'
 __changelog__ = 'https://codeberg.org/plotski/upsies/raw/branch/master/NEWS'
-__version__ = '2024.03.09'
+__version__ = '2024.04.12'
 
 
 def application_setup(config):
     """
     This function should be called by the UI ASAP when `config` is available
 
     :param config: :class:`~.configfiles.ConfigFiles` instance
```

### Comparing `upsies-2024.3.9/upsies/constants.py` & `upsies-2024.4.12/upsies/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,27 @@
 
 IMGHOSTS_FILEPATH = os.path.join(CONFIG_DIRECTORYPATH, 'imghosts.ini')
 """Path to image hosting services configuration file"""
 
 CLIENTS_FILEPATH = os.path.join(CONFIG_DIRECTORYPATH, 'clients.ini')
 """Path to BitTorrent clients configuration file"""
 
-VIDEO_FILE_EXTENSIONS = ('mkv', 'mp4', 'avi', 'wmv', 'vob', 'm2ts', 'mts', 'ts')
+VIDEO_FILE_EXTENSIONS = (
+    'avi',
+    'divx',
+    'm2ts',
+    'mkv',
+    'mp4',
+    'mpeg',
+    'mpg',
+    'mts',
+    'ts',
+    'vob',
+    'wmv',
+)
 """Sequence of file extensions to recognize video files"""
 
 GUESSIT_OPTIONS = {
     'expected_title': [
         'The Collector',
         'xXx',
     ],
```

### Comparing `upsies-2024.3.9/upsies/defaults.py` & `upsies-2024.4.12/upsies/defaults.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,21 @@
                     'pieces hashes from file contents.'
                 ),
             ),
         },
         'screenshots': {
             'optimize': utils.configfiles.config_value(
                 value=utils.types.Choice('default', options=utils.image.optimization_levels),
-                description='Whether to optimize screenshot file sizes',
+                description='Whether to optimize screenshot file sizes.',
+            ),
+        },
+        'id': {
+            'show_poster': utils.configfiles.config_value(
+                value=utils.types.Bool('no'),
+                description='Whether to display a poster for easier identification.',
             ),
         },
     },
 
     'trackers': {
         tracker.name: tracker.TrackerConfig()
         for tracker in trackers.trackers()
```

### Comparing `upsies-2024.3.9/upsies/errors.py` & `upsies-2024.4.12/upsies/errors.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/jobs/base.py` & `upsies-2024.4.12/upsies/jobs/base.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/jobs/custom.py` & `upsies-2024.4.12/upsies/jobs/custom.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/jobs/dialog.py` & `upsies-2024.4.12/upsies/jobs/dialog.py`

 * *Files 1% similar despite different names*

```diff
@@ -613,16 +613,17 @@
             raise exception
 
     def send(self, output):
         """
         Validate `output` before actually sending it
 
         Pass `output` to `validator`. If :class:`ValueError` is raised, pass it
-        to :meth:`warn` and do not finish. Otherwise, pass `output` to
-        :meth:`~.base.JobBase.send` and :meth:`~.base.JobBase.finish` this job.
+        to :meth:`warn` and do not finalize. Otherwise, pass `output` to
+        :meth:`~.base.JobBase.send` and :meth:`~.base.JobBase.finalize` this
+        job.
         """
         # Normalize, e.g. remove leading and trailing whitespace.
         output = self._normalizer(output)
 
         # Remove any warning from previously failed validation.
         self.clear_warnings()
```

### Comparing `upsies-2024.3.9/upsies/jobs/imghost.py` & `upsies-2024.4.12/upsies/jobs/imghost.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/jobs/mediainfo.py` & `upsies-2024.4.12/upsies/jobs/mediainfo.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/jobs/poster.py` & `upsies-2024.4.12/upsies/jobs/poster.py`

 * *Files 3% similar despite different names*

```diff
@@ -93,15 +93,14 @@
 
     async def _obtain(self):
         _log.debug('Obtaining poster: %r', self._getter)
         self.signal.emit('obtaining')
         try:
             params_or_poster = await self._getter()
         except errors.RequestError as e:
-            # raise self._ProcessingError(f'Failed to get poster: {e}')
             self.warn(f'Failed to get poster: {e}')
             params_or_poster = None
 
         _log.debug('Obtained poster: %r', params_or_poster)
         if not params_or_poster:
             params = await self._obtain_via_prompt()
 
@@ -113,20 +112,19 @@
 
         self.signal.emit('obtained', params['poster'])
         return params
 
     async def _obtain_via_prompt(self):
         self.info = 'Please enter a poster file or URL.'
         try:
+            poster = ''
             while True:
-                prompt = uis.prompts.TextPrompt()
-                self.add_prompt(prompt)
-                await prompt.wait()
-                poster = os.path.expanduser(prompt.result)
-
+                poster = os.path.expanduser(await self.add_prompt(
+                    uis.prompts.TextPrompt(text=poster)
+                ))
                 if not poster:
                     self.warn('Poster file or URL is required.')
 
                 elif self._url_regex.search(poster):
                     # Download poster just to get an error if it fails. Later
                     # downloads should grab it from cache without pestering the
                     # server.
@@ -136,14 +134,17 @@
                         self.warn(f'Failed to download poster: {e}')
                     else:
                         return {'poster': poster}
 
                 elif not os.path.exists(poster):
                     self.warn(f'Poster file does not exist: {poster}')
 
+                elif not os.path.isfile(poster):
+                    self.warn(f'Poster is not a file: {poster}')
+
                 else:
                     return {'poster': poster}
         finally:
             self.clear_warnings()
 
     async def _resize(self, poster, width, height):
         if width or height:
```

### Comparing `upsies-2024.3.9/upsies/jobs/scene.py` & `upsies-2024.4.12/upsies/jobs/scene.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/jobs/screenshots.py` & `upsies-2024.4.12/upsies/jobs/screenshots.py`

 * *Files 2% similar despite different names*

```diff
@@ -342,35 +342,39 @@
         output_queue.put((daemon.MsgType.error, 'No videos found'))
         return
 
     if not from_all_videos:
         # Only create screenshots from first video
         del video_files[1:]
 
-    timestamps_map = _map_timestamps(
-        video_files=video_files,
-        timestamps=timestamps,
-        count=count,
-    )
-
-    # Herald how many screenshots we are going to make
-    screenshots_total = sum((len(ts) for ts in timestamps_map.values()))
-    output_queue.put((daemon.MsgType.info, {'screenshots_total': screenshots_total}))
-
     try:
-        _screenshot_video_files(
-            output_queue, input_queue,
-            timestamps_map=timestamps_map,
-            output_dir=output_dir,
-            overwrite=overwrite,
+        timestamps_map = _map_timestamps(
+            video_files=video_files,
+            timestamps=timestamps,
+            count=count,
         )
-    except SystemExit:
-        # _maybe_terminate signals termination by raising SystemExit. This
-        # shouldn't cause any issues as long as we actually exit here.
-        pass
+    except errors.ContentError as e:
+        output_queue.put((daemon.MsgType.error, str(e)))
+
+    else:
+        # Herald how many screenshots we are going to make
+        screenshots_total = sum((len(ts) for ts in timestamps_map.values()))
+        output_queue.put((daemon.MsgType.info, {'screenshots_total': screenshots_total}))
+
+        try:
+            _screenshot_video_files(
+                output_queue, input_queue,
+                timestamps_map=timestamps_map,
+                output_dir=output_dir,
+                overwrite=overwrite,
+            )
+        except SystemExit:
+            # _maybe_terminate signals termination by raising SystemExit. This
+            # shouldn't cause any issues as long as we actually exit here.
+            pass
 
 
 def _get_video_files(output_queue, *, content_path, exclude_files):
     # Make list of appropriate video file(s) from `content_path`
     try:
         filtered_files = torrent.filter_files(content_path, exclude=exclude_files)
         return video.filter_main_videos(filtered_files)
@@ -447,21 +451,24 @@
     return timestamps_map
 
 
 def _validate_timestamps(*, video_file, timestamps, count):
     # Validate, normalize, deduplicate and sort timestamps
 
     # Stay clear of the last 10 seconds
-    duration = video.duration(video_file) - 10
-    if duration < 60:
-        return []
+    duration = video.duration(video_file)
+    if duration < 1:
+        raise errors.ContentError(f'Video duration is too short: {duration}s')
 
     timestamps_pretty = set()
     for ts in timestamps:
-        ts = max(0, min(duration, timestamp.parse(ts)))
+        try:
+            ts = max(0, min(duration, timestamp.parse(ts)))
+        except ValueError as e:
+            raise errors.ContentError(e)
         timestamps_pretty.add(timestamp.pretty(ts))
 
     if not timestamps and not count:
         count = DEFAULT_NUMBER_OF_SCREENSHOTS
 
     # Add more timestamps if the user didn't specify enough
     if count > 0 and len(timestamps_pretty) < count:
@@ -474,22 +481,30 @@
         # Include start and end of video
         if 0.0 not in positions:
             positions.insert(0, 0.0)
         if 1.0 not in positions:
             positions.append(1.0)
 
         # Insert timestamps between the two positions with the largest distance
+        looped = 0
         while len(timestamps_pretty) < count:
             pairs = [(a, b) for a, b in zip(positions, positions[1:])]
             max_distance, pos1, pos2 = max((b - a, a, b) for a, b in pairs)
             position = ((pos2 - pos1) / 2) + pos1
             timestamps_pretty.add(timestamp.pretty(duration * position))
             positions.append(position)
             positions.sort()
 
+            # If the duration in seconds is smaller than `count`, avoid
+            # endlessly looping.
+            looped += 1
+            if looped > count:
+                break
+
+    assert timestamps_pretty, timestamps_pretty
     return natsort.natsorted(timestamps_pretty)
 
 
 def _maybe_terminate(*, input_queue):
     try:
         typ, msg = input_queue.get_nowait()
     except queue.Empty:
```

### Comparing `upsies-2024.3.9/upsies/jobs/set.py` & `upsies-2024.4.12/upsies/jobs/set.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/jobs/submit.py` & `upsies-2024.4.12/upsies/jobs/submit.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/jobs/torrent.py` & `upsies-2024.4.12/upsies/jobs/torrent.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
     def _start_torrent_process(self, announce_url):
         self._torrent_process = daemon.DaemonProcess(
             name=self.name,
             target=_torrent_process,
             kwargs={
                 'content_path': self._content_path,
                 'announce': announce_url,
-                'source': self._tracker.options['source'],
+                'source': self._tracker.torrent_source_field,
                 'torrent_path': self._torrent_path,
                 'exclude': self._exclude_files,
                 'use_cache': not self.ignore_cache,
                 'reuse_torrent_path': self._reuse_torrent_path,
                 'randomize_infohash': self._tracker.options['randomize_infohash'],
                 'piece_size_calculator': self._tracker.calculate_piece_size,
                 'piece_size_min_max_calculator': self._tracker.calculate_piece_size_min_max,
```

### Comparing `upsies-2024.3.9/upsies/jobs/webdb.py` & `upsies-2024.4.12/upsies/jobs/webdb.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,14 +43,19 @@
             :class:`~.utils.webdbs.common.SearchResult` object that returns a
             coroutine function. ``value`` is the return value of that coroutine
             function.
 
         ``query_updated``
             Emitted after the :attr:`query` changed. Registered callbacks get
             the new query as a positional argument.
+
+        ``selected``
+            Emitted when :meth:`result_selected` is called. Registered callbacks
+            get a :class:`dict` with the keys ``id``, ``title``, ``type``,
+            ``url`` and ``year``.
     """
 
     @property
     def name(self):
         return f'{self._db.name}-id'
 
     @property
@@ -78,27 +83,41 @@
         return self._no_id_ok
 
     @no_id_ok.setter
     def no_id_ok(self, value):
         self._no_id_ok = bool(value)
 
     @property
+    def show_poster(self):
+        """Whether to display a poster of the focused search result"""
+        return self._show_poster
+
+    @show_poster.setter
+    def show_poster(self, value):
+        self._show_poster = bool(value)
+
+    def _get_show_poster(self):
+        return self._show_poster
+
+    @property
     def is_searching(self):
         """Whether a search request is currently being made"""
         return self._is_searching
 
-    def initialize(self, *, db, query, no_id_ok=False):
+    def initialize(self, *, db, query, no_id_ok=False, show_poster=True):
         """
         Set internal state
 
         :param WebDbApiBase db: Return value of :func:`.utils.webdbs.webdb`
         :param query: Path of the release (doesn't have to exist) or
             :class:`~.webdbs.common.Query` instance
         :param no_id_ok: Whether this job may finish without error if no ID is
             selected
+        :param show_poster: Whether to display a poster of the focused search
+            result
         """
         assert isinstance(db, webdbs.WebDbApiBase), f'Not a WebDbApiBase: {db!r}'
         self._db = db
         if not isinstance(query, webdbs.Query):
             query = webdbs.Query.from_any(query)
         self._query = self._db.sanitize_query(query)
 
@@ -118,34 +137,38 @@
         self._query.signal.register('changed', self.search)
 
         # Hold some information about the selected search result.
         self._selected = {}
         self.signal.register('selected', self._selected.update)
 
         self.no_id_ok = no_id_ok
+        self.show_poster = show_poster
         self._is_searching = False
         self._search_task = None
         self._info_callbacks_task = None
         self._info_callbacks = _InfoCallbacks(
             callbacks={
                 'id': self._make_update_info_func('id'),
                 'summary': self._make_update_info_func('summary'),
                 'title_original': self._make_update_info_func('title_original'),
                 'title_english': self._make_update_info_func('title_english'),
                 'genres': self._make_update_info_func('genres'),
                 'directors': self._make_update_info_func('directors'),
                 'cast': self._make_update_info_func('cast'),
                 'countries': self._make_update_info_func('countries'),
-                'poster': self._make_update_info_func('poster'),
+                'poster': self._make_update_info_func('poster', condition=self._get_show_poster),
             },
             error_callback=self.warn,
         )
 
-    def _make_update_info_func(self, key):
-        return lambda value: self._update_info_value(key, value)
+    def _make_update_info_func(self, key, condition=lambda: True):
+        def update_info_func(value):
+            if condition():
+                self._update_info_value(key, value)
+        return update_info_func
 
     def _update_info_value(self, attr, value):
         if value is Ellipsis:
             # Indicate that we are updating `attr` by not providing a value.
             self.signal.emit('info_updating', attr)
         else:
             self.signal.emit('info_updated', attr, value)
@@ -161,16 +184,24 @@
         self._set_state(is_searching=True, results=())
 
         try:
             # Get new search results
             results = await self._db.search(query)
             self._set_state(is_searching=False, results=results)
 
-            # Get details about the first search result
-            self._run_info_callbacks(results[0] if results else None)
+            if results:
+                if query.feeling_lucky and len(results) == 1:
+                    # Select single search result.
+                    self.result_selected(results[0])
+                else:
+                    # Display details about the first search result.
+                    self._run_info_callbacks(results[0])
+            else:
+                # Unset all details from previously selected search result.
+                self._run_info_callbacks(None)
 
         except errors.RequestError as e:
             self.warn(e)
 
         finally:
             self._set_state(is_searching=False)
```

### Comparing `upsies-2024.3.9/upsies/trackers/__init__.py` & `upsies-2024.4.12/upsies/trackers/__init__.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/trackers/ant/config.py` & `upsies-2024.4.12/upsies/trackers/ant/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,44 @@
 """
 Concrete :class:`~.base.TrackerConfigBase` subclass for ANT
 """
 
 import base64
 
-from ...utils import configfiles
+from ...utils import configfiles, types
 from ..base import TrackerConfigBase, exclude
 
 
 class AntTrackerConfig(TrackerConfigBase):
     defaults = {
         'base_url': base64.b64decode('aHR0cHM6Ly9hbnRoZWxpb24ubWU=').decode('ascii'),
         'apikey': configfiles.config_value(
             value='',
             description='Your person upload API key you created in your profile.',
         ),
         'announce_url': configfiles.config_value(
             value='',
             description='Your personal announce URL.',
         ),
-        'source': 'ANT',
         'exclude': (
             exclude.checksums,
             exclude.images,
             exclude.nfo,
             exclude.samples,
         ),
+        'anonymous': configfiles.config_value(
+            value=types.Bool('no'),
+            description='Whether your username is displayed on your uploads.',
+        ),
     }
 
     argument_definitions = {
         'submit': {
+            ('--anonymous', '--an'): {
+                'help': 'Hide your username for this submission',
+                'action': 'store_true',
+                # This must be `None` so it doesn't override the "anonymous"
+                # value from the config file. See CommandBase.get_options().
+                'default': None,
+            },
         },
     }
```

### Comparing `upsies-2024.3.9/upsies/trackers/ant/jobs.py` & `upsies-2024.4.12/upsies/trackers/ant/jobs.py`

 * *Files 25% similar despite different names*

```diff
@@ -77,22 +77,37 @@
             flags.append('Commentary')
 
         return flags
 
     @property
     def post_data(self):
         return {
-            'api_key': self._tracker.apikey,
-            'action': 'upload',
-            'tmdbid': self.get_job_output(self.tmdb_job, slice=0).replace('movie/', ''),
-            'mediainfo': self.get_job_output(self.mediainfo_job, slice=0),
-            'flags[]': self.get_job_output(self.flags_job),
+            **{
+                'api_key': self._tracker.apikey,
+                'action': 'upload',
+                'tmdbid': self.get_job_output(self.tmdb_job, slice=0).replace('movie/', ''),
+                'mediainfo': self.get_job_output(self.mediainfo_job, slice=0),
+                'flags[]': self.get_job_output(self.flags_job),
+                # Scene release? (I don't know why it's called "censored".)
+                'censored': '1' if self.get_job_attribute(self.scene_check_job, 'is_scene_release') else None,
+                'anonymous': '1' if self.options.get('anonymous') else None,
+            },
+            **self._post_data_release_group,
         }
 
     @property
+    def _post_data_release_group(self):
+        if self.release_name.group != 'NOGROUP':
+            return {'releasegroup': self.release_name.group}
+        else:
+            # Default value of <input type="checkbox"> is "on":
+            # https://developer.mozilla.org/en-US/docs/Web/HTML/Element/Input/checkbox
+            return {'noreleasegroup': 'on'}
+
+    @property
     def post_files(self):
         return {
             'file_input': {
                 'file': self.torrent_filepath,
                 'mimetype': 'application/x-bittorrent',
             },
         }
```

### Comparing `upsies-2024.3.9/upsies/trackers/ant/tracker.py` & `upsies-2024.4.12/upsies/trackers/ant/tracker.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import logging  # isort:skip
 _log = logging.getLogger(__name__)
 
 
 class AntTracker(TrackerBase):
     name = 'ant'
     label = 'ANT'
+    torrent_source_field = 'ANT'
 
     setup_howto_template = (
         '{howto.introduction}\n'
         '\n'
         '{howto.next_section}. API Key\n'
         '\n'
         '   {howto.current_section}.1 On the website, go to USERNAME -> Edit -> Access Settings\n'
```

### Comparing `upsies-2024.3.9/upsies/trackers/base/_howto.py` & `upsies-2024.4.12/upsies/trackers/base/_howto.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
                     '\n'
                     '   {howto.current_section}.1 Words in ALL_CAPS_AND_WITH_UNDERSCORES are placeholders.\n'
                     '   {howto.current_section}.2 Everything after "$" is a terminal command.\n'
                 ),
                 (
                     '{howto.next_section}. Configuration Defaults (Optional)\n'
                     '\n'
-                    '    If you prefer, you can write all default values at once and then edit \n'
+                    '    If you prefer, you can write all default values at once and then edit\n'
                     '    them in your favorite $EDITOR.\n'
                     '\n'
                     '    $ {executable} set --dump\n'
                     '    $ $EDITOR {tildify(constants.TRACKERS_FILEPATH)}\n'
                     '    $ $EDITOR {tildify(constants.IMGHOSTS_FILEPATH)}\n'
                     '    $ $EDITOR {tildify(constants.CLIENTS_FILEPATH)}\n'
                     '    $ $EDITOR {tildify(constants.CONFIG_FILEPATH)}\n'
```

### Comparing `upsies-2024.3.9/upsies/trackers/base/config.py` & `upsies-2024.4.12/upsies/trackers/base/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,18 +13,14 @@
     Dictionary with default values that are defined by the subclass
 
     Some keys defined by this base class always exist.
     """
 
     # Options that are available for all trackers
     _common_defaults = {
-        'source': utils.configfiles.config_value(
-            value='',
-            description='Value of the "source" field in generated torrents.',
-        ),
         'randomize_infohash': utils.configfiles.config_value(
             value=utils.types.Bool('no'),
             description=(
                 'Whether the info hash of generated torrents is randomized '
                 'by including a random number in the metadata.\n'
                 'WARNING: The tracker may choke on the non-standard field '
                 'or remove the random number, forcing you to manually download '
```

### Comparing `upsies-2024.3.9/upsies/trackers/base/exclude.py` & `upsies-2024.4.12/upsies/trackers/base/exclude.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/trackers/base/jobs.py` & `upsies-2024.4.12/upsies/trackers/base/jobs.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,25 +35,27 @@
     For a description of the arguments see the corresponding properties.
     """
 
     def __init__(self, *, content_path, tracker,
                  reuse_torrent_path=None, exclude_files=(),
                  btclient=None, torrent_destination=None,
                  screenshots_optimization=None, image_hosts=None,
+                 show_poster=False,
                  options=None, common_job_args=None):
         self._content_path = content_path
-        self._reuse_torrent_path = reuse_torrent_path
         self._tracker = tracker
-        self._screenshots_optimization = screenshots_optimization
-        self._image_hosts = image_hosts
+        self._reuse_torrent_path = reuse_torrent_path
+        self._exclude_files = exclude_files
         self._btclient = btclient
         self._torrent_destination = torrent_destination
-        self._exclude_files = exclude_files
-        self._common_job_args = common_job_args or {}
+        self._screenshots_optimization = screenshots_optimization
+        self._image_hosts = image_hosts
+        self._show_poster = show_poster
         self._options = options or {}
+        self._common_job_args = common_job_args or {}
         self._signal = utils.signal.Signal('warning', 'error', 'exception')
 
     @property
     def content_path(self):
         """
         Content path to generate metadata for
 
@@ -132,19 +134,27 @@
     def common_job_args(self, **overload):
         """
         Keyword arguments that are passed to all jobs or empty `dict`
 
         :param overload: Keyword arguments add or replace values from the
             initialization argument
         """
-        return {
+        # Combine global defaults with custom values.
+        args = {
             **self._common_job_args,
             **overload,
         }
 
+        # Individual jobs may only set `ignore_cache=False` if
+        # `ignore_cache=True` wasn't set globally, e.g. with --ignore-cache.
+        if self._common_job_args.get('ignore_cache') or overload.get('ignore_cache'):
+            args['ignore_cache'] = True
+
+        return args
+
     @property
     @abc.abstractmethod
     def jobs_before_upload(self):
         """
         Sequence of jobs that need to finish before :meth:`~.TrackerBase.upload` can
         be called
         """
@@ -454,14 +464,15 @@
 
     @functools.cached_property
     def imdb_job(self):
         """:class:`~.jobs.webdb.WebDbSearchJob` instance"""
         return jobs.webdb.WebDbSearchJob(
             query=self.content_path,
             db=self.imdb,
+            show_poster=self._show_poster,
             callbacks={
                 'output': self._handle_imdb_id,
             },
             precondition=self.make_precondition('imdb_job'),
             **self.common_job_args(),
         )
 
@@ -476,14 +487,15 @@
 
     @functools.cached_property
     def tmdb_job(self):
         """:class:`~.jobs.webdb.WebDbSearchJob` instance"""
         return jobs.webdb.WebDbSearchJob(
             query=self.content_path,
             db=self.tmdb,
+            show_poster=self._show_poster,
             callbacks={
                 'output': self._handle_tmdb_id,
             },
             precondition=self.make_precondition('tmdb_job'),
             **self.common_job_args(),
         )
 
@@ -500,14 +512,15 @@
 
     @functools.cached_property
     def tvmaze_job(self):
         """:class:`~.jobs.webdb.WebDbSearchJob` instance"""
         return jobs.webdb.WebDbSearchJob(
             query=self.content_path,
             db=self.tvmaze,
+            show_poster=self._show_poster,
             callbacks={
                 'output': self._handle_tvmaze_id,
             },
             precondition=self.make_precondition('tvmaze_job'),
             **self.common_job_args(),
         )
```

### Comparing `upsies-2024.3.9/upsies/trackers/base/tracker.py` & `upsies-2024.4.12/upsies/trackers/base/tracker.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,14 +42,23 @@
         """Lower-case tracker name abbreviation for internal use"""
 
     @property
     @abc.abstractmethod
     def label(self):
         """User-facing tracker name abbreviation"""
 
+    @property
+    @abc.abstractmethod
+    def torrent_source_field(self):
+        """
+        Torrents for this tracker get a ``source`` field with this value
+
+        This is usually the same as :attr:`label`.
+        """
+
     setup_howto_template = 'Nobody has written a setup howto yet.'
     """
     Step-by-step guide that explains how to make your first upload
 
     .. note:: This MUST be a class attribute and not a property.
 
     The following placeholders can be used in f-string format:
```

### Comparing `upsies-2024.3.9/upsies/trackers/bhd/config.py` & `upsies-2024.4.12/upsies/trackers/bhd/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,15 +33,14 @@
         'apikey': configfiles.config_value(
             value='',
             description=(
                 'Your personal private API key.\n'
                 'Get it from the website: My Security -> API key'
             ),
         ),
-        'source': 'BHD',
         'anonymous': configfiles.config_value(
             value=types.Bool('no'),
             description='Whether your username is displayed on your uploads.',
         ),
         'draft': configfiles.config_value(
             value=types.Bool('no'),
             description=(
@@ -73,14 +72,21 @@
             exclude.samples,
             exclude.subtitles,
         ),
     }
 
     argument_definitions = {
         'submit': {
+            ('--anonymous', '--an'): {
+                'help': 'Hide your username for this submission',
+                'action': 'store_true',
+                # This must be `None` so it doesn't override the "anonymous"
+                # value from the config file. See CommandBase.get_options().
+                'default': None,
+            },
             ('--custom-edition', '--ce'): {
                 'help': 'Non-standard edition, e.g. "Final Cut"',
                 'default': '',
             },
             ('--draft', '--dr'): {
                 'help': 'Upload as draft',
                 'action': 'store_true',
```

### Comparing `upsies-2024.3.9/upsies/trackers/bhd/jobs.py` & `upsies-2024.4.12/upsies/trackers/bhd/jobs.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/trackers/bhd/tracker.py` & `upsies-2024.4.12/upsies/trackers/bhd/tracker.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import logging  # isort:skip
 _log = logging.getLogger(__name__)
 
 
 class BhdTracker(TrackerBase):
     name = 'bhd'
     label = 'BHD'
+    torrent_source_field = 'BHD'
 
     setup_howto_template = (
         '{howto.introduction}\n'
         '\n'
         '{howto.next_section}. Announce Passkey\n'
         '\n'
         '   {howto.current_section}.1 On the website, go to My Settings -> Security -> Passkey\n'
```

### Comparing `upsies-2024.3.9/upsies/trackers/dummy.py` & `upsies-2024.4.12/upsies/trackers/dummy.py`

 * *Files 2% similar despite different names*

```diff
@@ -253,14 +253,18 @@
             )
 
 
 class DummyTracker(base.TrackerBase):
     name = 'dummy'
     label = 'DuMmY'
 
+    @property
+    def torrent_source_field(self):
+        return self.options['source']
+
     setup_howto_template = (
         'This is just a no-op tracker for testing and demonstration.'
     )
 
     TrackerJobs = DummyTrackerJobs
     TrackerConfig = DummyTrackerConfig
```

### Comparing `upsies-2024.3.9/upsies/trackers/mtv/config.py` & `upsies-2024.4.12/upsies/trackers/mtv/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,14 @@
         'base_url': base64.b64decode('aHR0cHM6Ly93d3cubW9yZXRoYW50di5tZQ==').decode('ascii'),
         'username': '',
         'password': '',
         'announce_url': configfiles.config_value(
             value='',
             description='Your personal announce URL. Automatically fetched from the website if not set.',
         ),
-        'source': 'MTV',
         'image_host': configfiles.config_value(
             value=types.ListOf(
                 item_type=MtvImageHost,
                 default=('imgbox',),
                 separator=',',
             ),
             description=(
@@ -54,14 +53,21 @@
             value=types.Bool('no'),
             description='Whether your username is displayed on your uploads.',
         ),
     }
 
     argument_definitions = {
         'submit': {
+            ('--anonymous', '--an'): {
+                'help': 'Hide your username for this submission',
+                'action': 'store_true',
+                # This must be `None` so it doesn't override the "anonymous"
+                # value from the config file. See CommandBase.get_options().
+                'default': None,
+            },
             ('--screenshots', '--ss'): {
                 'help': ('How many screenshots to make '
                          f'(min={defaults["screenshots"].min}, '
                          f'max={defaults["screenshots"].max})'),
                 'type': argtypes.number_of_screenshots(
                     min=defaults['screenshots'].min,
                     max=defaults['screenshots'].max,
```

### Comparing `upsies-2024.3.9/upsies/trackers/mtv/jobs.py` & `upsies-2024.4.12/upsies/trackers/mtv/jobs.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/trackers/mtv/tracker.py` & `upsies-2024.4.12/upsies/trackers/mtv/tracker.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import logging  # isort:skip
 _log = logging.getLogger(__name__)
 
 
 class MtvTracker(TrackerBase):
     name = 'mtv'
     label = 'MTV'
+    torrent_source_field = 'MTV'
 
     setup_howto_template = (
         '{howto.introduction}\n'
         '\n'
         '{howto.next_section}. Login Credentials\n'
         '\n'
         '   {howto.current_section}.1 $ upsies set trackers.{tracker.name}.username USERNAME\n'
```

### Comparing `upsies-2024.3.9/upsies/trackers/nbl/config.py` & `upsies-2024.4.12/upsies/trackers/nbl/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -24,14 +24,13 @@
         'apikey': configfiles.config_value(
             value='',
             description=(
                 'Your personal private API key.\n'
                 'Get it from the website: <USERNAME> -> Settings -> API keys'
             ),
         ),
-        'source': 'NBL',
         'exclude': (),
     }
 
     argument_definitions = {
         # Custom arguments, e.g. "upsies submit nbl --foo bar"
     }
```

### Comparing `upsies-2024.3.9/upsies/trackers/nbl/jobs.py` & `upsies-2024.4.12/upsies/trackers/nbl/jobs.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/trackers/nbl/tracker.py` & `upsies-2024.4.12/upsies/trackers/nbl/tracker.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import logging  # isort:skip
 _log = logging.getLogger(__name__)
 
 
 class NblTracker(base.TrackerBase):
     name = 'nbl'
     label = 'NBL'
+    torrent_source_field = 'NBL'
 
     setup_howto_template = (
         '{howto.introduction}\n'
         '\n'
         '{howto.next_section}. Announce URL\n'
         '\n'
         '   {howto.current_section}.1 On the website, go to Shows -> Upload and copy the ANNOUNCE_URL.\n'
```

### Comparing `upsies-2024.3.9/upsies/trackers/ptp/jobs.py` & `upsies-2024.4.12/upsies/trackers/ptp/jobs.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,29 +74,33 @@
     @functools.cached_property
     def type_job(self):
         return jobs.dialog.ChoiceJob(
             name=self.get_job_name('type'),
             label='Type',
             precondition=self.make_precondition('type_job'),
             autodetect=self.autodetect_type,
-            options=(
-                ('Feature Film', 'Feature Film'),
-                ('Short Film', 'Short Film'),
-                ('Miniseries', 'Miniseries'),
-                ('Stand-up Comedy', 'Stand-up Comedy'),
-                ('Live Performance', 'Live Performance'),
-                ('Movie Collection', 'Movie Collection'),
-            ),
+            options=metadata.types,
+            # If user specified a type, e.g. via CLI, do not make them select it
+            # again in the TUI.
+            autofinish=bool(self.options.get('type')),
             callbacks={
                 'finished': self.update_imdb_query,
             },
-            **self.common_job_args(),
+            # Ignore cached source if CLI option --type is provided.
+            **self.common_job_args(ignore_cache=bool(self.options.get('type'))),
         )
 
     def autodetect_type(self, _):
+        # User explicitly specified type, e.g. via CLI.
+        if self.options.get('type'):
+            for type, regex in metadata.types.items():
+                if regex.search(self.options['type']):
+                    return type
+
+        # Detect miniseries from release name.
         if self.release_name.type == ReleaseType.season:
             return 'Miniseries'
 
         # Short film if runtime 45 min or less (Rule 1.1.1)
         # NOTE: This doesn't work for VIDEO_TS releases. We could sum the
         #       duration of all .VOB files, but they notoriously lie about their
         #       duration. For now, the user can always correct the autodetected
@@ -106,16 +110,18 @@
         ))[0]
         if utils.video.duration(main_video) <= 45 * 60:
             return 'Short Film'
 
     @functools.cached_property
     def imdb_job(self):
         imdb_job = super().imdb_job
-        # Disabled until #7 is fixed.
         imdb_job.no_id_ok = True
+        if self.options.get('imdb'):
+            imdb_job.query.id = self.options['imdb']
+            imdb_job.query.feeling_lucky = True
         return imdb_job
 
     def update_imdb_query(self, type_job_):
         """
         Set :attr:`~.webdbs.common.Query.type` on
         :attr:`~.TrackerJobsBase.imdb_job` to :attr:`~.ReleaseType.movie` or
         :attr:`~.ReleaseType.series` depending on the output of :attr:`type_job`
@@ -455,15 +461,16 @@
         )
 
     async def fetch_title(self):
         assert self.imdb_job.is_finished, self.imdb_job
         # Fill in title from release name until it is loaded from PTP.
         self.title_job.text = self.release_name.title
         metadata = await self.tracker.get_movie_metadata(self.imdb_id)
-        return metadata['title']
+        # Default to `None` to use title from release name.
+        return metadata['title'] or None
 
     def normalize_title(self, text):
         return text.strip()
 
     def validate_title(self, text):
         if not text:
             raise ValueError('Title must not be empty.')
@@ -496,15 +503,16 @@
         )
 
     async def fetch_year(self):
         assert self.imdb_job.is_finished, self.imdb_job
         # Fill in year from release name until it is loaded from PTP.
         self.year_job.text = self.release_name.year
         metadata = await self.tracker.get_movie_metadata(self.imdb_id)
-        return metadata['year']
+        # Default to `None` to use year from release name.
+        return metadata['year'] or None
 
     def normalize_year(self, text):
         return text.strip()
 
     def validate_year(self, text):
         if not text:
             raise ValueError('Year must not be empty.')
@@ -613,18 +621,27 @@
 
     def normalize_tags(self, text):
         tags = [tag.strip() for tag in text.split(',')]
         deduped = sorted(dict.fromkeys(tags))
         return ', '.join(tag for tag in deduped if tag)
 
     def validate_tags(self, text):
+        if not text.strip():
+            raise ValueError('You must provide at least one tag.')
+
+        tags = []
         for tag in text.split(','):
             tag = tag.strip()
             if tag and tag not in metadata.tags:
                 raise ValueError(f'Tag is not valid: {tag}')
+            else:
+                tags.append(tag)
+
+        if len(self.normalize_tags(text)) > 200:
+            raise ValueError('You provided too many tags.')
 
     @functools.cached_property
     def poster_job(self):
         job = super().poster_job
         # Hide poster_job until imdb_job and ptp_group_id_job are done.
         job.prejobs += (
             self.imdb_job,
@@ -829,49 +846,46 @@
             name=self.get_job_name('source'),
             label='Source',
             precondition=self.make_precondition('source_job'),
             text=self.autodetect_source,
             normalizer=self.normalize_source,
             validator=self.validate_source,
             finish_on_success=True,
-            **self.common_job_args(),
+            # Ignore cached source if CLI option --source is provided.
+            **self.common_job_args(ignore_cache=bool(self.options.get('source'))),
         )
 
-    _known_sources = {
-        'Blu-ray': re.compile(r'(?i:blu-?ray)'),  # (UHD) BluRay (Remux)
-        'DVD': re.compile(r'^(?i:dvd)'),  # DVD(Rip|5|9|...)
-        'WEB': re.compile(r'^(?i:web)'),  # WEB(-DL|Rip)
-        'HD-DVD': re.compile(r'^(?i:hd-?dvd)$'),
-        'HDTV': re.compile(r'^(?i:hd-?tv)$'),
-        'TV': re.compile(r'^(?i:tv)'),  # TV(Rip|...)
-        'VHS': re.compile(r'^(?i:vhs)'),  # VHS(Rip|...)
-    }
-
     def autodetect_source(self):
+        if self.options.get('source'):
+            # Get pre-specified source, e.g. from CLI argument.
+            source = self.options['source']
+        else:
+            # Get source from release name.
+            source = self.release_name.source
+
         # Find autodetected source in valid PTP sources
-        source = self.release_name.source
-        for known_source, regex in self._known_sources.items():
+        for known_source, regex in metadata.sources.items():
             if regex.search(source):
                 # Finish the job without prompting the user
                 return known_source
 
         # Let the user fix the autodetected source
         self.source_job.text = source
 
     def normalize_source(self, text):
         text = text.strip()
-        for source in self._known_sources:
-            if source.casefold() == text.casefold():
+        for source, regex in metadata.sources.items():
+            if regex.search(text):
                 return source
         return text
 
     def validate_source(self, text):
         if not text or text == 'UNKNOWN_SOURCE':
             raise ValueError('You must provide a source.')
-        elif text not in self._known_sources:
+        elif text not in metadata.sources:
             raise ValueError(f'Source is not valid: {text}')
 
     @property
     def post_data(self):
         post_data = self._post_data_common
 
         _log.debug('PTP group ID: %r', self.ptp_group_id)
```

### Comparing `upsies-2024.3.9/upsies/trackers/ptp/metadata.py` & `upsies-2024.4.12/upsies/trackers/ptp/metadata.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Hardcoded PTP metadata from upload.php
 """
 
 import enum
+import re
 
 tags = (
     'action',
     'adventure',
     'animation',
     'arthouse',
     'asian',
@@ -38,14 +39,35 @@
     'thriller',
     'video.art',
     'war',
     'western',
 )
 
 
+types = {
+    'Feature Film': re.compile(r'^(?i:(?:feature|).?film|movie)$'),
+    'Short Film': re.compile(r'^(?i:short.?(?:film|))$'),
+    'Miniseries': re.compile(r'^(?i:(?:mini.?|)series|season|tv)$'),
+    'Stand-up Comedy': re.compile(r'^(?i:stand.?up.?comedy|stand.?up|comedy)$'),
+    'Live Performance': re.compile(r'(?i:live.?performance|live|performance)$'),
+    'Movie Collection': re.compile(r'(?i:movie.?collection|collection)$'),
+}
+
+
+sources = {
+    'Blu-ray': re.compile(r'(?i:blu-?ray)'),  # (UHD) BluRay (Remux)
+    'DVD': re.compile(r'^(?i:dvd)'),  # DVD(Rip|5|9|...)
+    'WEB': re.compile(r'^(?i:web)'),  # WEB(-DL|Rip)
+    'HD-DVD': re.compile(r'^(?i:hd-?dvd)$'),
+    'HDTV': re.compile(r'^(?i:hd-?tv)$'),
+    'TV': re.compile(r'^(?i:tv)'),  # TV(Rip|...)
+    'VHS': re.compile(r'^(?i:vhs)'),  # VHS(Rip|...)
+}
+
+
 # NOTE: The order of the dictionaries and their elements are copied from
 #       upload.php. They should be submitted in the same order as listed here.
 editions = {
     'collection.criterion': 'The Criterion Collection',
     'collection.masters': 'Masters of Cinema',
     'collection.warner': 'Warner Archive Collection',
```

### Comparing `upsies-2024.3.9/upsies/trackers/ptp/tracker.py` & `upsies-2024.4.12/upsies/trackers/ptp/tracker.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import logging  # isort:skip
 _log = logging.getLogger(__name__)
 
 
 class PtpTracker(TrackerBase):
     name = 'ptp'
     label = 'PTP'
+    torrent_source_field = 'PTP'
 
     setup_howto_template = (
         '{howto.introduction}\n'
         '\n'
         '{howto.next_section}. Login Credentials\n'
         '\n'
         '   {howto.current_section}.1 $ upsies set trackers.{tracker.name}.username USERNAME\n'
@@ -250,15 +251,15 @@
             files=post_files,
             # Ignore the HTTP redirect (should be 302 Found) so we can get the
             # torrent URL from the "Location" response header
             follow_redirects=False,
         )
 
         # The server needs some time to process the uploaded metadata before the
-        # torrent is registered by the tracker and we can seed it. If don't
+        # torrent is registered by the tracker and we can seed it. If we don't
         # sleep() here, the torrent may be announced before the tracker knows it
         # exists.
         await asyncio.sleep(1)
 
         # # Read previously received response for debugging
         # response_filepath = 'ptp_upload.response.content'
         # response = utils.http.Response(
@@ -317,37 +318,38 @@
 
         Any :class:`~.RequestError` is caught and passed to
         :meth:`.TrackerBase.error`.
 
         :return: PTP group ID or `None` if PTP doesn't have a group for
             `imdb_id`
         """
-        _log.debug('%s: Fetching PTP group ID', imdb_id)
-        try:
-            await self.login()
-            response = await self._request(
-                method='GET',
-                url=self._torrents_url,
-                params={
-                    'imdb': self.normalize_imdb_id(imdb_id),
-                    'json': '1',
-                },
-                cache=True,
-            )
+        if imdb_id:
+            _log.debug('%s: Fetching PTP group ID', imdb_id)
+            try:
+                await self.login()
+                response = await self._request(
+                    method='GET',
+                    url=self._torrents_url,
+                    params={
+                        'imdb': self.normalize_imdb_id(imdb_id),
+                        'json': '1',
+                    },
+                    cache=True,
+                )
 
-        except errors.RequestError as e:
-            self.error(e)
+            except errors.RequestError as e:
+                self.error(e)
 
-        else:
-            match = re.search(r'id=(\d+)', response.headers.get('location', ''))
-            if match:
-                _log.debug('%s: PTP group ID: %s', imdb_id, match.group(1))
-                return match.group(1)
             else:
-                _log.debug('%s: No PTP group ID', imdb_id)
+                match = re.search(r'id=(\d+)', response.headers.get('location', ''))
+                if match:
+                    _log.debug('%s: PTP group ID: %s', imdb_id, match.group(1))
+                    return match.group(1)
+                else:
+                    _log.debug('%s: No PTP group ID', imdb_id)
 
     async def get_movie_metadata(self, imdb_id):
         """
         Get metadata about movie as :class:`dict` from PTP website
 
         :param imdb_id: IMDb ID (e.g. ``tt123456``)
```

### Comparing `upsies-2024.3.9/upsies/trackers/uhd/config.py` & `upsies-2024.4.12/upsies/trackers/uhd/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,14 @@
             value=types.Bool('no'),
             description='Whether your username is displayed on your uploads.',
         ),
         'announce_url': configfiles.config_value(
             value='',
             description='Your personal announce URL.',
         ),
-        'source': '[UHDBits]',
         'image_host': configfiles.config_value(
             value=types.ListOf(
                 item_type=UhdImageHost,
                 default=('ptpimg', 'freeimage', 'imgbox'),
                 separator=',',
             ),
             description=(
@@ -56,14 +55,17 @@
     }
 
     argument_definitions = {
         'submit': {
             ('--anonymous', '--an'): {
                 'help': 'Hide your username for this submission',
                 'action': 'store_true',
+                # This must be `None` so it doesn't override the "anonymous"
+                # value from the config file. See CommandBase.get_options().
+                'default': None,
             },
             ('--internal', '--in'): {
                 'help': 'Internal encode (use only if you were told to)',
                 'action': 'store_true',
             },
             ('--3d',): {
                 'help': 'Mark this as a 3D release',
```

### Comparing `upsies-2024.3.9/upsies/trackers/uhd/jobs.py` & `upsies-2024.4.12/upsies/trackers/uhd/jobs.py`

 * *Files 0% similar despite different names*

```diff
@@ -308,20 +308,22 @@
     async def autodetect_source(self, _):
         for source, is_source in self.source_map.items():
             if is_source(self.release_name):
                 _log.debug('Autodetected source: %r', source)
                 return source
 
     source_map = {
+        'Remux': lambda release: 'Remux' in release.source,
         'Encode': lambda release: any(
             source in release.source
             for source in (
                 'BluRay',
                 'HD-DVD',
-            )),
+            )
+        ),
         'WEB-DL': lambda release: 'WEB-DL' in release.source,
         'WEBRip': lambda release: 'WEBRip' in release.source,
         'HDTV': lambda release: 'HDTV' in release.source,
         # Not sure what "HDRip" is exactly and how to detect it.
         'HDRip': lambda release: 'Rip' in release.source,
     }
 
@@ -410,14 +412,16 @@
             finish_on_success=True,
             normalizer=self.normalize_tags,
             validator=self.validate_tags,
             **self.common_job_args(),
         )
 
     async def autodetect_tags(self):
+        assert self.imdb_job.is_finished
+
         json = await self._tracker.get_uhd_info(self.imdb_id)
         # Tags are comma-separated and may contain entities like "&eacute;". We
         # split them to a list. Keep in mind that the tags may be an empty
         # string, and `"".split(",")` returns `[""]`.
         return utils.html.as_text(json.get('tag', ''))
 
     max_tags_length = 200
```

### Comparing `upsies-2024.3.9/upsies/trackers/uhd/tracker.py` & `upsies-2024.4.12/upsies/trackers/uhd/tracker.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 Concrete :class:`~.base.TrackerBase` subclass for UHD
 """
 
 import asyncio
-import datetime
 import re
 import urllib
 
 from ... import __project_name__, errors, utils
 from ..base import TrackerBase
 from .config import UhdTrackerConfig
 from .jobs import UhdTrackerJobs
@@ -15,14 +14,15 @@
 import logging  # isort:skip
 _log = logging.getLogger(__name__)
 
 
 class UhdTracker(TrackerBase):
     name = 'uhd'
     label = 'UHD'
+    torrent_source_field = '[UHDBits]'
 
     setup_howto_template = (
         '{howto.introduction}\n'
         '\n'
         '{howto.next_section}. Login Credentials\n'
         '\n'
         '   {howto.current_section}.1 $ upsies set trackers.{tracker.name}.username USERNAME\n'
@@ -159,14 +159,15 @@
             announce_url_tag = doc.find('input', value=re.compile(r'^https?://.*/announce\b'))
             if announce_url_tag:
                 return announce_url_tag['value']
             else:
                 cmd = f'{__project_name__} set trackers.{self.name}.announce_url YOUR_URL'
                 raise errors.RequestError(f'Failed to find announce URL - set it manually: {cmd}')
 
+    @utils.blocking_memoize
     async def get_uhd_info(self, imdb_id):
         """
         Get IMDb information from tracker
 
         :param imdb_id: IMDb ID
 
         The return value is a dictionary returned by ajax.php. It may contain
@@ -175,20 +176,32 @@
         assert imdb_id, 'IMDb ID is not available yet'
 
         try:
             # If ajax.php doesn't have the info cached, it responds with
             # {"error": "1"}, in which case, we wait a decreasing number of
             # seconds before trying again. This is more or less what the website
             # JS is doing.
-            for sleep in (6, 5, 4, 3, 3, 3, 3, 3, 3, 0):
+
+            # Example responses:
+            # {"error":1,"message":" Submited to fetcher..."}
+            # {"error":1,"message":" Fetching..."}
+            # {'status': 'failure', 'error': 'rate limit exceeded'}
+
+            # Wait 6 seconds after the first try, then 3 seconds for up to 3
+            # minutes combined. Wait 0 seconds if the last try also fails.
+            for sleep in (6,) + (3,) * 20 * 3 + (0,):
                 uhd_info = await self._get_uhd_info(imdb_id)
-                _log.debug('UHD info: %r', uhd_info)
-                if uhd_info.get('error', '1') == '0':
+                if str(uhd_info.get('error', '1')) == '0':
+                    _log.debug('UHD info: %r', uhd_info)
                     return uhd_info
+                if str(uhd_info.get('error')) not in ('1', '0'):
+                    _log.debug('Failed to get UHD info for %s: %r', imdb_id, uhd_info['error'])
+                    break
                 elif sleep > 0:
+                    _log.debug('Still waiting for UHD info: %r', uhd_info)
                     await asyncio.sleep(sleep)
 
         except errors.RequestError as e:
             _log.debug('Failed to get UHD info for %s: %r', imdb_id, e)
             pass
 
         return {}
@@ -196,15 +209,14 @@
     async def _get_uhd_info(self, imdb_id):
         response = await self._request(
             method='GET',
             url=self._ajax_url,
             params={
                 'action': 'imdb_fetch',
                 'imdbid': imdb_id,
-                '_': int(datetime.datetime.now(datetime.timezone.utc).timestamp() * 1000),
             },
         )
         _log.debug('UHD info for %s: %r', imdb_id, response)
         return response.json()
 
     async def upload(self, tracker_jobs):
         assert self.is_logged_in
```

### Comparing `upsies-2024.3.9/upsies/uis/prompts.py` & `upsies-2024.4.12/upsies/uis/prompts.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/uis/tui/commands/__init__.py` & `upsies-2024.4.12/upsies/uis/tui/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/uis/tui/commands/base.py` & `upsies-2024.4.12/upsies/uis/tui/commands/base.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/uis/tui/commands/mediainfo.py` & `upsies-2024.4.12/upsies/uis/tui/commands/mediainfo.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/uis/tui/commands/poster.py` & `upsies-2024.4.12/upsies/uis/tui/commands/poster.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,15 @@
     def webdb_job(self):
         return jobs.webdb.WebDbSearchJob(
             home_directory=self.cache_directory,
             cache_directory=self.cache_directory,
             ignore_cache=self.args.ignore_cache,
             query=utils.webdbs.Query.from_release(self.release_name),
             db=self.webdb,
+            show_poster=self.config['config']['id']['show_poster'],
         )
 
     @property
     def webdb_id(self):
         if self.webdb_job.is_finished and self.webdb_job.output:
             return self.webdb_job.output[0]
```

### Comparing `upsies-2024.3.9/upsies/uis/tui/commands/release_name.py` & `upsies-2024.4.12/upsies/uis/tui/commands/release_name.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,12 +76,13 @@
         # an ID first. IMDb seems to be best.
         return jobs.webdb.WebDbSearchJob(
             home_directory=self.home_directory,
             cache_directory=self.cache_directory,
             ignore_cache=self.args.ignore_cache,
             query=utils.webdbs.Query.from_path(self.args.RELEASE),
             db=self.imdb,
+            show_poster=self.config['config']['id']['show_poster'],
         )
 
     @functools.cached_property
     def imdb(self):
         return utils.webdbs.webdb('imdb')
```

### Comparing `upsies-2024.3.9/upsies/uis/tui/commands/scene.py` & `upsies-2024.4.12/upsies/uis/tui/commands/scene.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/uis/tui/commands/screenshots.py` & `upsies-2024.4.12/upsies/uis/tui/commands/screenshots.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/uis/tui/commands/set.py` & `upsies-2024.4.12/upsies/uis/tui/commands/set.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/uis/tui/commands/submit.py` & `upsies-2024.4.12/upsies/uis/tui/commands/submit.py`

 * *Files 4% similar despite different names*

```diff
@@ -144,14 +144,15 @@
             options=self.tracker_options,
             content_path=self.args.CONTENT,
             reuse_torrent_path=(
                 tuple(self.args.reuse_torrent)
                 + tuple(self.config['config']['torrent-create']['reuse_torrent_paths'])
             ),
             screenshots_optimization=self.config['config']['screenshots']['optimize'],
+            show_poster=self.config['config']['id']['show_poster'],
             image_hosts=self._get_image_hosts(),
             btclient=self._get_btclient(),
             torrent_destination=self._get_torrent_destination(),
             exclude_files=(
                 tuple(self.config['trackers'][self.tracker.name]['exclude'])
                 + tuple(self.args.exclude_files)
                 + tuple(self.args.exclude_files_regex)
```

### Comparing `upsies-2024.3.9/upsies/uis/tui/commands/torrent.py` & `upsies-2024.4.12/upsies/uis/tui/commands/torrent.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/uis/tui/commands/upload_images.py` & `upsies-2024.4.12/upsies/uis/tui/commands/upload_images.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/uis/tui/commands/webdb.py` & `upsies-2024.4.12/upsies/uis/tui/commands/webdb.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,14 +28,18 @@
 
       - id:ID
         Search for a specific, known ID.
 
     If possible, the ID is also detected in normal text without the "id:ID"
     format. The exact detection is specific to each database, but searching for
     an URL (e.g. https://www.tvmaze.com/shows/1910) should always work.
+
+    If the query starts with "!" and there is only one search result,
+    automatically select it. This is useful when searching for an ID,
+    e.g. "!id:tt0123456".
     """
 
     names = ('id',)
 
     argument_definitions = {
         'DB': {
             'type': utils.argtypes.webdb,
@@ -53,9 +57,10 @@
         return (
             jobs.webdb.WebDbSearchJob(
                 home_directory=self.home_directory,
                 cache_directory=self.cache_directory,
                 ignore_cache=self.args.ignore_cache,
                 query=utils.webdbs.Query.from_path(self.args.RELEASE),
                 db=utils.webdbs.webdb(self.args.DB),
+                show_poster=self.config['config']['id']['show_poster'],
             ),
         )
```

### Comparing `upsies-2024.3.9/upsies/uis/tui/headless.py` & `upsies-2024.4.12/upsies/uis/tui/headless.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/uis/tui/jobwidgets/__init__.py` & `upsies-2024.4.12/upsies/uis/tui/jobwidgets/__init__.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/uis/tui/jobwidgets/base.py` & `upsies-2024.4.12/upsies/uis/tui/jobwidgets/base.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/uis/tui/jobwidgets/custom.py` & `upsies-2024.4.12/upsies/uis/tui/jobwidgets/custom.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/uis/tui/jobwidgets/dialog.py` & `upsies-2024.4.12/upsies/uis/tui/jobwidgets/dialog.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/uis/tui/jobwidgets/imghost.py` & `upsies-2024.4.12/upsies/uis/tui/jobwidgets/imghost.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/uis/tui/jobwidgets/poster.py` & `upsies-2024.4.12/upsies/uis/tui/jobwidgets/poster.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/uis/tui/jobwidgets/scene.py` & `upsies-2024.4.12/upsies/uis/tui/jobwidgets/scene.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,16 +45,17 @@
         self.job.signal.register('ask_is_scene_release', self._ask_is_scene_release)
 
         @self.keybindings_global.add(
             'c-s', 'n',
             filter=Condition(lambda: self._question.text == ''),
         )
         def _(event):
-            self.job.stop_checking()
-            self.job.set_result(SceneCheckResult.false)
+            if not self.job.is_finished:
+                self.job.stop_checking()
+                self.job.set_result(SceneCheckResult.false)
 
     def _ask_release_name(self, release_names):
         _log.debug('Asking for release name: %r', release_names)
 
         self._activity_indicator.active = False
 
         def handle_release_name(choice):
```

### Comparing `upsies-2024.3.9/upsies/uis/tui/jobwidgets/screenshots.py` & `upsies-2024.4.12/upsies/uis/tui/jobwidgets/screenshots.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/uis/tui/jobwidgets/submit.py` & `upsies-2024.4.12/upsies/uis/tui/jobwidgets/submit.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/uis/tui/jobwidgets/torrent.py` & `upsies-2024.4.12/upsies/uis/tui/jobwidgets/torrent.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/uis/tui/jobwidgets/webdb.py` & `upsies-2024.4.12/upsies/uis/tui/jobwidgets/webdb.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/uis/tui/main.py` & `upsies-2024.4.12/upsies/uis/tui/main.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/uis/tui/style.py` & `upsies-2024.4.12/upsies/uis/tui/style.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/uis/tui/tui.py` & `upsies-2024.4.12/upsies/uis/tui/tui.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/uis/tui/utils.py` & `upsies-2024.4.12/upsies/uis/tui/utils.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/uis/tui/widgets.py` & `upsies-2024.4.12/upsies/uis/tui/widgets.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/utils/__init__.py` & `upsies-2024.4.12/upsies/utils/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -410,14 +410,60 @@
     See :meth:`asyncio.BaseEventLoop.run_in_executor`.
     """
     loop = asyncio.get_running_loop()
     wrapped = functools.partial(function, *args, **kwargs)
     return await loop.run_in_executor(None, wrapped)
 
 
+_NOTHING = object()
+
+def blocking_memoize(coro_func):
+    """
+    Asynchronous memoization decorator that blocks concurrent calls with the
+    same arguments
+
+    The first call calls the decorated function while subsequent calls wait
+    until the first call returns and the return value is cached. Subsequent
+    calls then get the return value from the cache.
+
+    Exceptions raised by `coro_func` are also cached and re-raised on subsequent
+    calls.
+
+    The decorated function provides a `clear_cache` method that removes any
+    cached return values.
+    """
+    cache = {}
+    lock = collections.defaultdict(asyncio.Lock)
+
+    @functools.wraps(coro_func)
+    async def wrapper(*args, **kwargs):
+        cache_key = semantic_hash((str(coro_func), args, kwargs))
+        async with lock[cache_key]:
+            result = cache.get(cache_key, _NOTHING)
+
+            if result is _NOTHING:
+                try:
+                    result = await coro_func(*args, **kwargs)
+                except BaseException as e:
+                    result = e
+                cache[cache_key] = result
+
+            if isinstance(result, BaseException):
+                raise result
+            else:
+                return result
+
+    def clear_cache():
+        cache.clear()
+
+    wrapper.clear_cache = clear_cache
+
+    return wrapper
+
+
 # We must import these here to prevent circular imports
 from . import (  # noqa: E402 isort:skip
     argtypes,
     browser,
     btclient,
     configfiles,
     country,
```

### Comparing `upsies-2024.3.9/upsies/utils/argtypes.py` & `upsies-2024.4.12/upsies/utils/argtypes.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,21 @@
 
 import argparse
 import functools
 import os
 
 from . import types
 
+ArgumentTypeError = argparse.ArgumentTypeError
+"""
+Exception that should be raised by any callable that is passed to
+:func:`argparse.ArgumentParser.add_argument` as `type` if it gets an invalid
+value
+"""
+
 
 def comma_separated(argtype):
     """
     Multiple comma-separated values
 
     :param argtype: Any callable that returns a validated object for one of the
         comma-separated values or raises :class:`ValueError`, :class:`TypeError`
```

### Comparing `upsies-2024.3.9/upsies/utils/btclient.py` & `upsies-2024.4.12/upsies/utils/btclient.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/utils/configfiles.py` & `upsies-2024.4.12/upsies/utils/configfiles.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,20 +69,18 @@
 
     :param defaults: Nested directory structure as described above with
         default values
     :param files: Mapping of section names to file paths that are :meth:`read`
         during initialization
     """
 
-    def __init__(self, defaults, ignore_missing=False, **files):
+    def __init__(self, defaults):
         self._defaults = copy.deepcopy(defaults)
         self._cfg = _ConfigDict(self._defaults, types=self._build_types())
         self._files = {}  # Map section names to file paths
-        for section, filepath in files.items():
-            self.read(section, filepath, ignore_missing=ignore_missing)
 
     def _build_types(self):
         def make_config_type(value):
             parent_class = type(value)
 
             def preconvert(v):
                 # Convert non-sequence to sequence if we expect a sequence
@@ -329,20 +327,19 @@
                     else:
                         # Exclude default value
                         continue
                 else:
                     # Non-default value
                     lines_subsection.append(line)
 
-            if lines_subsection:
-                lines.append(f'[{subsection}]')
-                lines.extend(lines_subsection)
+            lines.append(f'[{subsection}]')
+            lines.extend(lines_subsection)
 
-                # Empty line between subsections
-                lines.append('')
+            # Empty line between subsections
+            lines.append('')
 
         return '\n'.join(lines)
 
 
 class _ConfigDict(collections.abc.MutableMapping):
     """
     Dictionary that only accepts certain keys and value types
```

### Comparing `upsies-2024.3.9/upsies/utils/country.py` & `upsies-2024.4.12/upsies/utils/country.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/utils/daemon.py` & `upsies-2024.4.12/upsies/utils/daemon.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/utils/fs.py` & `upsies-2024.4.12/upsies/utils/fs.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/utils/html.py` & `upsies-2024.4.12/upsies/utils/html.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/utils/http.py` & `upsies-2024.4.12/upsies/utils/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -616,41 +616,48 @@
         with open(filepath, 'rb') as f:
             return f.read()
     except OSError:
         pass
 
 
 def _cache_file(method, url, params, data):
+
     def make_filename(method, url, params_and_data_str):
         if params_and_data_str:
             filename = f'{method.upper()}.{url}?{params_and_data_str}'
         else:
             filename = f'{method.upper()}.{url}'
         return filename.replace(' ', '+')
 
     params_and_data = {
         # GET parameters
         **params,
-        # POST parameters
+        # POST parameters with binary data as hashes
         **{
             k: (
+                v
+                if isinstance(v, str) else
                 utils.semantic_hash(v)
-                if isinstance(v, (bytes, bytearray)) else
-                str(v)
             )
             for k, v in data.items()
         },
     }
     if params_and_data:
         params_and_data_str = '&'.join((f'{k}={v}' for k,v in params_and_data.items()))
-        if len(make_filename(method, url, params_and_data_str)) > 250:
-            params_and_data_str = utils.semantic_hash(params_and_data)
     else:
         params_and_data_str = ''
 
+    # If the payload is too long, hash it.
+    if params_and_data and len(make_filename(method, url, params_and_data_str)) > 250:
+        params_and_data_str = utils.semantic_hash(params_and_data)
+
+    # If the file name is still too long, also hash the URL.
+    if len(make_filename(method, url, params_and_data_str)) > 250:
+        url = utils.semantic_hash(url)
+
     return os.path.join(
         _get_cache_directory(),
         utils.fs.sanitize_filename(make_filename(method, url, params_and_data_str)),
     )
 
 
 DEFAULT_USER_AGENT = 'Mozilla/5.0 (X11; Linux) Gecko/20100101 Firefox'
```

### Comparing `upsies-2024.3.9/upsies/utils/image.py` & `upsies-2024.4.12/upsies/utils/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,16 @@
         'full_chroma_inp',
         'accurate_rnd',
         'spline',
     )
 
     if utils.video.is_bt2020(video_file):
         vf = ':'.join((
-            'scale=in_h_chr_pos=0',
+            "scale='max(sar,1)*iw':'max(1/sar,1)*ih'",
+            'in_h_chr_pos=0',
             'in_v_chr_pos=0',
             'in_color_matrix=bt2020',
             'flags=' + '+'.join(vf_flags),
         ))
 
     elif utils.video.is_bt709(video_file):
         vf = ':'.join((
```

### Comparing `upsies-2024.3.9/upsies/utils/imghosts/__init__.py` & `upsies-2024.4.12/upsies/utils/imghosts/__init__.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/utils/imghosts/base.py` & `upsies-2024.4.12/upsies/utils/imghosts/base.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/utils/imghosts/common.py` & `upsies-2024.4.12/upsies/utils/imghosts/common.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/utils/imghosts/dummy.py` & `upsies-2024.4.12/upsies/utils/imghosts/dummy.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/utils/imghosts/freeimage.py` & `upsies-2024.4.12/upsies/utils/imghosts/freeimage.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/utils/imghosts/imgbb.py` & `upsies-2024.4.12/upsies/utils/imghosts/imgbb.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/utils/imghosts/imgbox.py` & `upsies-2024.4.12/upsies/utils/imghosts/imgbox.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/utils/imghosts/ptpimg.py` & `upsies-2024.4.12/upsies/utils/imghosts/ptpimg.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/utils/predbs/__init__.py` & `upsies-2024.4.12/upsies/utils/predbs/__init__.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/utils/predbs/base.py` & `upsies-2024.4.12/upsies/utils/predbs/base.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/utils/predbs/common.py` & `upsies-2024.4.12/upsies/utils/predbs/common.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/utils/predbs/corruptnet.py` & `upsies-2024.4.12/upsies/utils/predbs/corruptnet.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/utils/predbs/multi.py` & `upsies-2024.4.12/upsies/utils/predbs/multi.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/utils/predbs/predbclub.py` & `upsies-2024.4.12/upsies/utils/predbs/predbclub.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/utils/predbs/predbde.py` & `upsies-2024.4.12/upsies/utils/predbs/predbde.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/utils/predbs/predbovh.py` & `upsies-2024.4.12/upsies/utils/predbs/predbovh.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/utils/predbs/query.py` & `upsies-2024.4.12/upsies/utils/predbs/query.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/utils/predbs/srrdb.py` & `upsies-2024.4.12/upsies/utils/predbs/srrdb.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/utils/release.py` & `upsies-2024.4.12/upsies/utils/release.py`

 * *Files 0% similar despite different names*

```diff
@@ -628,16 +628,26 @@
 
     @video_format.setter
     def video_format(self, value):
         self._info['video_codec'] = str(value)
 
     @_translated_property
     def group(self):
-        '''Name of release group or "NOGROUP"'''
-        return self._info.get('group') or 'NOGROUP'
+        """
+        Name of release group or "NOGROUP"
+
+        "NOGRP", and "" are translated to "NOGROUP" case-insensitively.
+        """
+        group = self._info.get('group', '')
+        if self.nogroup_regex.match(group):
+            return 'NOGROUP'
+        else:
+            return group
+
+    nogroup_regex = re.compile(r'^(?i:nogroup|nogrp|)$')
 
     @group.setter
     def group(self, value):
         self._info['group'] = str(value)
 
     @property
     def has_commentary(self):
@@ -894,29 +904,32 @@
             parts.append(self.audio_channels)
 
         if self.hdr_format:
             parts.append(self.hdr_format)
 
         parts.append(self.video_format)
 
-        joined = ' '.join(parts) + f'-{self.group}'
+        joined = ' '.join(parts)
 
         # Separator (usually " " or ".")
         sep = separator if separator is not None else self.separator
         if sep != ' ':
             joined = joined.replace(' ', sep)
 
         if sep == '.':
             # Replace "&" with "and" before "&" gets removed
             joined = re.sub(r'&', 'and', joined)
             # Remove most non-word characters (e.g. ",") with some exceptions
+            # (e.g. "-" is needed for "WEB-DL")
             joined = re.sub(r'[^ \w\.-]', '', joined)
             # Deduplicate "." in case there is a "." at the end of the title
             joined = re.sub(r'\.+', '.', joined)
 
+        joined += f'-{self.group}'
+
         return joined
 
 
 class ReleaseInfo(collections.abc.MutableMapping):
     """
     Parse information from release name or path
```

### Comparing `upsies-2024.3.9/upsies/utils/signal.py` & `upsies-2024.4.12/upsies/utils/signal.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/utils/string.py` & `upsies-2024.4.12/upsies/utils/string.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/utils/subproc.py` & `upsies-2024.4.12/upsies/utils/subproc.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/utils/subtitle.py` & `upsies-2024.4.12/upsies/utils/subtitle.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/utils/timestamp.py` & `upsies-2024.4.12/upsies/utils/timestamp.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/utils/torrent.py` & `upsies-2024.4.12/upsies/utils/torrent.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/utils/types.py` & `upsies-2024.4.12/upsies/utils/types.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/utils/update.py` & `upsies-2024.4.12/upsies/utils/update.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/utils/video.py` & `upsies-2024.4.12/upsies/utils/video.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/utils/webdbs/__init__.py` & `upsies-2024.4.12/upsies/utils/webdbs/__init__.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/utils/webdbs/base.py` & `upsies-2024.4.12/upsies/utils/webdbs/base.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/utils/webdbs/common.py` & `upsies-2024.4.12/upsies/utils/webdbs/common.py`

 * *Files 23% similar despite different names*

```diff
@@ -18,38 +18,44 @@
     Search query for databases like IMDb
 
     :param str title: Name of the movie or TV series
     :param type: :class:`~.types.ReleaseType` enum or one of its value names
     :param year: Year of release
     :type year: str or int
     :param str id: Known ID for a specific DB
+    :param bool feeling_lucky: Whether an only search result should be
+        autoselected
+
+        This can be convenient if `id` is provided.
 
     :raise ValueError: if an invalid argument is passed
     """
 
     @staticmethod
     def _normalize_title(title):
         return ' '.join(title.casefold().strip().split())
 
     _kwarg_defaults = {
         'year': None,
         'type': ReleaseType.unknown,
         'id': None,
+        'feeling_lucky': False,
     }
 
     def __init__(self, title='', **kwargs):
         for k in kwargs:
             if k not in self._kwarg_defaults:
                 raise TypeError(f'Unkown argument: {k!r}')
         self._signal = signal.Signal()
         self._signal.add('changed')
         self.title = title
         self.type = kwargs.get('type', self._kwarg_defaults['type'])
         self.year = kwargs.get('year', self._kwarg_defaults['year'])
         self.id = kwargs.get('id', self._kwarg_defaults['id'])
+        self.feeling_lucky = kwargs.get('feeling_lucky', self._kwarg_defaults['feeling_lucky'])
 
     @property
     def type(self):
         """:class:`~.types.ReleaseType` value"""
         return self._type
 
     @type.setter
@@ -116,25 +122,39 @@
         before = getattr(self, '_id', None)
 
         self._id = str(id) if id else None
 
         if self._id != before:
             self.signal.emit('changed', self)
 
+    @property
+    def feeling_lucky(self):
+        """Whether an only search result should be autoselected"""
+        return self._feeling_lucky
+
+    @feeling_lucky.setter
+    def feeling_lucky(self, feeling_lucky):
+        before = getattr(self, '_feeling_lucky', None)
+
+        self._feeling_lucky = bool(feeling_lucky)
+
+        if self._feeling_lucky != before:
+            self.signal.emit('changed', self)
+
     def update(self, query, silent=False):
         """
         Copy property values from other query
 
         :param query: :class:`Query` instance to copy values from
         :param bool silent: Whether to prevent any :attr:`signal` emissions
         """
         before = str(self)
 
         with self.signal.suspend('changed'):
-            for attr in ('title', 'type', 'year', 'id'):
+            for attr in ('title', 'type', 'year', 'id', 'feeling_lucky'):
                 other_value = getattr(query, attr)
                 setattr(self, attr, other_value)
 
         if not silent and str(self) != before:
             self.signal.emit('changed', self)
 
     def copy(self, **updates):
@@ -144,14 +164,15 @@
         :param updates: Updated attributes
         """
         kwargs = {
             'title': self.title,
             'type': self.type,
             'year': self.year,
             'id': self.id,
+            'feeling_lucky': self.feeling_lucky,
         }
         kwargs.update(updates)
         return type(self)(**kwargs)
 
     _types = {
         ReleaseType.movie: ('movie', 'film'),
         ReleaseType.season: ('season', 'series', 'tv', 'show', 'tvshow'),
@@ -193,25 +214,34 @@
                     elif kw == 'year':
                         return 'year', value
                     elif kw == 'id':
                         return 'id', value
                     raise ValueError(f'Invalid {kw}: {value}')
             return None, None
 
-        # Extract "key:value" pairs (e.g. "year:2015")
+        query = query.strip()
         title = []
         kwargs = {}
+
+        # "I'm feeling lucky" if query starts with "!".
+        if query and query[0] == '!':
+            kwargs['feeling_lucky'] = True
+            query = query[1:]
+
+        # Extract "key:value" pairs (e.g. "year:2015")
         for part in str(query).strip().split():
             kw, value = get_kwarg(part)
             if (kw, value) != (None, None):
                 kwargs[kw] = value
             else:
                 title.append(part)
+
         if title:
             kwargs['title'] = ' '.join(title)
+
         return cls(**kwargs)
 
     @classmethod
     def from_release(cls, info):
         """
         Create instance from :class:`~.release.ReleaseInfo` or
         :class:`~.release.ReleaseName` instance
@@ -275,30 +305,38 @@
                 and self.id == other.id
             )
         else:
             return NotImplemented
 
     def __str__(self):
         if self.id:
-            return f'id:{self.id}'
+            text = f'id:{self.id}'
         else:
             parts = [self.title]
             for attr in ('type', 'year', 'id'):
                 value = getattr(self, attr)
                 if value:
                     parts.append(f'{attr}:{value}')
-            return ' '.join(parts)
+            text = ' '.join(parts)
+
+        if self.feeling_lucky:
+            text = f'!{text}'
+
+        return text
 
     def __repr__(self):
         kwargs = ', '.join(
             f'{k}={v!r}'
-            for k, v in (('title', self.title),
-                         ('year', self.year),
-                         ('type', self.type),
-                         ('id', self.id))
+            for k, v in (
+                ('title', self.title),
+                ('year', self.year),
+                ('type', self.type),
+                ('id', self.id),
+                ('feeling_lucky', self.feeling_lucky),
+            )
             if v
         )
         return f'{type(self).__name__}({kwargs})'
 
 
 class SearchResult:
     """
```

### Comparing `upsies-2024.3.9/upsies/utils/webdbs/imdb.py` & `upsies-2024.4.12/upsies/utils/webdbs/imdb.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies/utils/webdbs/tmdb.py` & `upsies-2024.4.12/upsies/utils/webdbs/tmdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -338,15 +338,17 @@
                 elif tmdb_type == 'tv':
                     return ReleaseType.series
         return ReleaseType.unknown
 
     def _get_title(self, soup):
         header = soup.select('.result > h2')
         if header:
-            return header[0].string
+            # Title tag may contain other information in smaller font or dimmed.
+            title_tag = header[0].contents[0]
+            return html.as_text(title_tag)
         else:
             return ''
 
     def _get_year(self, soup):
         release_date = soup.find(class_='release_date')
         if release_date:
             match = re.search(r'(\d{4})$', release_date.string)
```

### Comparing `upsies-2024.3.9/upsies/utils/webdbs/tvmaze.py` & `upsies-2024.4.12/upsies/utils/webdbs/tvmaze.py`

 * *Files identical despite different names*

### Comparing `upsies-2024.3.9/upsies.egg-info/PKG-INFO` & `upsies-2024.4.12/upsies.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upsies
-Version: 2024.3.9
+Version: 2024.4.12
 Summary: Media metadata aggregator
 Author-email: plotski <plotski@example.org>
 License: GPL-3.0-or-later
 Project-URL: Repository, https://codeberg.org/plotski/upsies
 Project-URL: Documentation, https://upsies.readthedocs.io
 Project-URL: Bug Tracker, https://codeberg.org/plotski/upsies/issues
 Project-URL: Changelog, https://codeberg.org/plotski/upsies/raw/branch/master/NEWS
@@ -88,7 +88,24 @@
 * Do everything simultaneously
 
 ``upsies`` is developed on `Codeberg <https://codeberg.org/plotski/upsies>`_.
 
 The latest release is available on `PyPI <https://pypi.org/project/upsies>`_.
 
 Documentation is hosted on `Read the Docs <https://upsies.readthedocs.io/en/stable/>`_.
+
+Supported Trackers
+------------------
+
+* ANT
+* BHD
+* MTV
+* NBL
+* PTP
+* UHD
+
+Contact
+-------
+
+To report an issue or ask for a feature, please post in the upsies thread in the
+relevant tracker's forum. If you don't want to wait days for a response, you can
+leave a ping `here <https://codeberg.org/plotski/upsies/issues/9>`_.
```

### Comparing `upsies-2024.3.9/upsies.egg-info/SOURCES.txt` & `upsies-2024.4.12/upsies.egg-info/SOURCES.txt`

 * *Files identical despite different names*

