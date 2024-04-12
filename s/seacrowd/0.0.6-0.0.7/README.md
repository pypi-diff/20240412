# Comparing `tmp/seacrowd-0.0.6.tar.gz` & `tmp/seacrowd-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seacrowd-0.0.6.tar", last modified: Fri Apr 12 07:28:54 2024, max compression
+gzip compressed data, was "seacrowd-0.0.7.tar", last modified: Fri Apr 12 07:52:57 2024, max compression
```

## Comparing `seacrowd-0.0.6.tar` & `seacrowd-0.0.7.tar`

### file list

```diff
@@ -1,982 +1,982 @@
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:54.583225 seacrowd-0.0.6/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    11357 2024-04-04 06:00:44.000000 seacrowd-0.0.6/LICENSE
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1071 2024-04-12 07:28:54.579359 seacrowd-0.0.6/PKG-INFO
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5757 2024-04-04 06:00:44.000000 seacrowd-0.0.6/README.md
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:46.732901 seacrowd-0.0.6/seacrowd/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      251 2024-04-12 07:21:36.000000 seacrowd-0.0.6/seacrowd/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    40451 2024-04-11 08:39:41.000000 seacrowd-0.0.6/seacrowd/config_helper.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:46.848049 seacrowd-0.0.6/seacrowd/sea_datasets/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/__init__.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:46.868089 seacrowd-0.0.6/seacrowd/sea_datasets/abui_wordnet/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/abui_wordnet/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5277 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/abui_wordnet/abui_wordnet.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:46.887959 seacrowd-0.0.6/seacrowd/sea_datasets/alt_burmese_treebank/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/alt_burmese_treebank/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5692 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/alt_burmese_treebank/alt_burmese_treebank.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:46.909020 seacrowd-0.0.6/seacrowd/sea_datasets/alt_burmese_treebank/utils/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/alt_burmese_treebank/utils/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     2661 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/alt_burmese_treebank/utils/alt_burmese_treebank_utils.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:46.931600 seacrowd-0.0.6/seacrowd/sea_datasets/ara_close/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/ara_close/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8227 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/ara_close/ara_close.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:46.957167 seacrowd-0.0.6/seacrowd/sea_datasets/asr_sindodusc/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/asr_sindodusc/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7231 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/asr_sindodusc/asr_sindodusc.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:46.978836 seacrowd-0.0.6/seacrowd/sea_datasets/asr_smaldusc/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/asr_smaldusc/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7305 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/asr_smaldusc/asr_smaldusc.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.009337 seacrowd-0.0.6/seacrowd/sea_datasets/asr_stidusc/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/asr_stidusc/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6979 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/asr_stidusc/asr_stidusc.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.036352 seacrowd-0.0.6/seacrowd/sea_datasets/audio_keyword_spotting/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/audio_keyword_spotting/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7860 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/audio_keyword_spotting/audio_keyword_spotting.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.064027 seacrowd-0.0.6/seacrowd/sea_datasets/aya_dataset/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/aya_dataset/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7482 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/aya_dataset/aya_dataset.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.084109 seacrowd-0.0.6/seacrowd/sea_datasets/barasa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/barasa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7224 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/barasa/barasa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.109275 seacrowd-0.0.6/seacrowd/sea_datasets/beaye_lexicon/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/beaye_lexicon/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4357 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/beaye_lexicon/beaye_lexicon.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.130968 seacrowd-0.0.6/seacrowd/sea_datasets/belebele/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/belebele/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8610 2024-04-11 08:39:41.000000 seacrowd-0.0.6/seacrowd/sea_datasets/belebele/belebele.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.153641 seacrowd-0.0.6/seacrowd/sea_datasets/bible_en_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/bible_en_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6790 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/bible_en_id/bible_en_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.174766 seacrowd-0.0.6/seacrowd/sea_datasets/bible_jv_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/bible_jv_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6856 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/bible_jv_id/bible_jv_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.197212 seacrowd-0.0.6/seacrowd/sea_datasets/bible_su_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/bible_su_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6632 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/bible_su_id/bible_su_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.235098 seacrowd-0.0.6/seacrowd/sea_datasets/bioner_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/bioner_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6108 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/bioner_id/bioner_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.258688 seacrowd-0.0.6/seacrowd/sea_datasets/bloom_captioning/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/bloom_captioning/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8518 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/bloom_captioning/bloom_captioning.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.288029 seacrowd-0.0.6/seacrowd/sea_datasets/bloom_lm/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/bloom_lm/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8430 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/bloom_lm/bloom_lm.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.335590 seacrowd-0.0.6/seacrowd/sea_datasets/bloom_speech/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/bloom_speech/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6922 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/bloom_speech/bloom_speech.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.361637 seacrowd-0.0.6/seacrowd/sea_datasets/bloom_vist/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/bloom_vist/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9674 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/bloom_vist/bloom_vist.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.381018 seacrowd-0.0.6/seacrowd/sea_datasets/burapha_th/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/burapha_th/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6995 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/burapha_th/burapha_th.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.419602 seacrowd-0.0.6/seacrowd/sea_datasets/burmese_romanize/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/burmese_romanize/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4420 2024-04-11 08:39:41.000000 seacrowd-0.0.6/seacrowd/sea_datasets/burmese_romanize/burmese_romanize.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.450411 seacrowd-0.0.6/seacrowd/sea_datasets/casa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/casa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5635 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/casa/casa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.473904 seacrowd-0.0.6/seacrowd/sea_datasets/cc100/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/cc100/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10941 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/cc100/cc100.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.495134 seacrowd-0.0.6/seacrowd/sea_datasets/cc_aligned_doc/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/cc_aligned_doc/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6230 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/cc_aligned_doc/cc_aligned_doc.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.529630 seacrowd-0.0.6/seacrowd/sea_datasets/cc_aligned_sent/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/cc_aligned_sent/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6256 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/cc_aligned_sent/cc_aligned_sent.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.554037 seacrowd-0.0.6/seacrowd/sea_datasets/cebuaner/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/cebuaner/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7783 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/cebuaner/cebuaner.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.574548 seacrowd-0.0.6/seacrowd/sea_datasets/coco_35l/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/coco_35l/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9830 2024-04-11 08:39:41.000000 seacrowd-0.0.6/seacrowd/sea_datasets/coco_35l/coco_35l.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.608979 seacrowd-0.0.6/seacrowd/sea_datasets/cod/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/cod/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6239 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/cod/cod.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.629113 seacrowd-0.0.6/seacrowd/sea_datasets/code_mixed_jv_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/code_mixed_jv_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8760 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/code_mixed_jv_id/code_mixed_jv_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.647789 seacrowd-0.0.6/seacrowd/sea_datasets/codeswitch_reddit/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/codeswitch_reddit/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9015 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/codeswitch_reddit/codeswitch_reddit.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.670309 seacrowd-0.0.6/seacrowd/sea_datasets/commonvoice_120/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/commonvoice_120/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9438 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/commonvoice_120/commonvoice_120.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.689763 seacrowd-0.0.6/seacrowd/sea_datasets/copal/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/copal/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5868 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/copal/copal.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.712355 seacrowd-0.0.6/seacrowd/sea_datasets/covost2/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/covost2/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10329 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/covost2/covost2.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.760118 seacrowd-0.0.6/seacrowd/sea_datasets/creole_rc/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/creole_rc/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9448 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/creole_rc/creole_rc.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.780285 seacrowd-0.0.6/seacrowd/sea_datasets/crosssum/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/crosssum/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5467 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/crosssum/crosssum.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.804116 seacrowd-0.0.6/seacrowd/sea_datasets/cub_bahasa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/cub_bahasa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    14495 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/cub_bahasa/cub_bahasa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.824936 seacrowd-0.0.6/seacrowd/sea_datasets/culturax/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/culturax/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6383 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/culturax/culturax.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.849359 seacrowd-0.0.6/seacrowd/sea_datasets/cvss/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/cvss/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    11054 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/cvss/cvss.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.869445 seacrowd-0.0.6/seacrowd/sea_datasets/dengue_filipino/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/dengue_filipino/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4777 2024-04-11 08:39:41.000000 seacrowd-0.0.6/seacrowd/sea_datasets/dengue_filipino/dengue_filipino.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.889299 seacrowd-0.0.6/seacrowd/sea_datasets/emot/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/emot/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5522 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/emot/emot.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.909140 seacrowd-0.0.6/seacrowd/sea_datasets/emotcmt/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/emotcmt/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4484 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/emotcmt/emotcmt.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.927021 seacrowd-0.0.6/seacrowd/sea_datasets/emotes_3k/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/emotes_3k/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9257 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/emotes_3k/emotes_3k.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.947002 seacrowd-0.0.6/seacrowd/sea_datasets/emotion_id_opinion/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/emotion_id_opinion/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7315 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/emotion_id_opinion/emotion_id_opinion.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.968816 seacrowd-0.0.6/seacrowd/sea_datasets/etos/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/etos/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7041 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/etos/etos.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.988780 seacrowd-0.0.6/seacrowd/sea_datasets/facqa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/facqa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5788 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/facqa/facqa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.010272 seacrowd-0.0.6/seacrowd/sea_datasets/facqa/utils/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/facqa/utils/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      815 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/facqa/utils/facqa_utils.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.037824 seacrowd-0.0.6/seacrowd/sea_datasets/fakenews_ph/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/fakenews_ph/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4936 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/fakenews_ph/fakenews_ph.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.057662 seacrowd-0.0.6/seacrowd/sea_datasets/filipino_gay_lang/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/filipino_gay_lang/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4808 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/filipino_gay_lang/filipino_gay_lang.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.077081 seacrowd-0.0.6/seacrowd/sea_datasets/filipino_hatespeech_tiktok/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/filipino_hatespeech_tiktok/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4697 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/filipino_hatespeech_tiktok/filipino_hatespeech_tiktok.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.102456 seacrowd-0.0.6/seacrowd/sea_datasets/filipino_slang_norm/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/filipino_slang_norm/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4967 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/filipino_slang_norm/filipino_slang_norm.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.123926 seacrowd-0.0.6/seacrowd/sea_datasets/filipino_words_aoa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/filipino_words_aoa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4965 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/filipino_words_aoa/filipino_words_aoa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.144609 seacrowd-0.0.6/seacrowd/sea_datasets/filwordnet/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/filwordnet/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4819 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/filwordnet/filwordnet.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.184920 seacrowd-0.0.6/seacrowd/sea_datasets/fleurs/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/fleurs/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    13248 2024-04-11 09:11:07.000000 seacrowd-0.0.6/seacrowd/sea_datasets/fleurs/fleurs.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      785 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/fleurs/lang_config.json
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.225488 seacrowd-0.0.6/seacrowd/sea_datasets/flores200/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/flores200/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    13920 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/flores200/flores200.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.249544 seacrowd-0.0.6/seacrowd/sea_datasets/fsl_105/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/fsl_105/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6753 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/fsl_105/fsl_105.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.281406 seacrowd-0.0.6/seacrowd/sea_datasets/gatitos/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/gatitos/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6624 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/gatitos/gatitos.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.307190 seacrowd-0.0.6/seacrowd/sea_datasets/gklmip_newsclass/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/gklmip_newsclass/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6024 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/gklmip_newsclass/gklmip_newsclass.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.334563 seacrowd-0.0.6/seacrowd/sea_datasets/gklmip_sentiment/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/gklmip_sentiment/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5007 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/gklmip_sentiment/gklmip_sentiment.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.369817 seacrowd-0.0.6/seacrowd/sea_datasets/globalwoz/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/globalwoz/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10031 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/globalwoz/globalwoz.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.399450 seacrowd-0.0.6/seacrowd/sea_datasets/glotstorybook/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/glotstorybook/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5878 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/glotstorybook/glotstorybook.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.428794 seacrowd-0.0.6/seacrowd/sea_datasets/hoasa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/hoasa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6301 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/hoasa/hoasa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.468492 seacrowd-0.0.6/seacrowd/sea_datasets/iapp_squad/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/iapp_squad/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5420 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/iapp_squad/iapp_squad.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.500634 seacrowd-0.0.6/seacrowd/sea_datasets/iatf/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/iatf/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5801 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/iatf/iatf.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.527877 seacrowd-0.0.6/seacrowd/sea_datasets/icon/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/icon/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8351 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/icon/icon.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.560614 seacrowd-0.0.6/seacrowd/sea_datasets/id_abusive/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_abusive/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6540 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_abusive/id_abusive.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.592468 seacrowd-0.0.6/seacrowd/sea_datasets/id_abusive_news_comment/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_abusive_news_comment/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4293 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_abusive_news_comment/id_abusive_news_comment.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.616104 seacrowd-0.0.6/seacrowd/sea_datasets/id_am2ico/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_am2ico/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7430 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_am2ico/id_am2ico.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.659734 seacrowd-0.0.6/seacrowd/sea_datasets/id_clickbait/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_clickbait/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5770 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_clickbait/id_clickbait.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.682230 seacrowd-0.0.6/seacrowd/sea_datasets/id_coreference_resolution/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_coreference_resolution/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7576 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_coreference_resolution/id_coreference_resolution.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.721906 seacrowd-0.0.6/seacrowd/sea_datasets/id_frog_story/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_frog_story/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4524 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_frog_story/id_frog_story.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.748382 seacrowd-0.0.6/seacrowd/sea_datasets/id_google_play_review/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_google_play_review/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6144 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_google_play_review/id_google_play_review.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.776868 seacrowd-0.0.6/seacrowd/sea_datasets/id_hatespeech/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_hatespeech/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4450 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_hatespeech/id_hatespeech.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.809546 seacrowd-0.0.6/seacrowd/sea_datasets/id_hoax_news/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_hoax_news/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4555 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_hoax_news/id_hoax_news.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.841938 seacrowd-0.0.6/seacrowd/sea_datasets/id_hsd_nofaaulia/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_hsd_nofaaulia/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7252 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_hsd_nofaaulia/id_hsd_nofaaulia.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.863161 seacrowd-0.0.6/seacrowd/sea_datasets/id_msvd/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_msvd/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5051 2024-04-11 08:39:41.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_msvd/id_msvd.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.882911 seacrowd-0.0.6/seacrowd/sea_datasets/id_multilabel_hs/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_multilabel_hs/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6021 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_multilabel_hs/id_multilabel_hs.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.904554 seacrowd-0.0.6/seacrowd/sea_datasets/id_panl_bppt/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_panl_bppt/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5616 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_panl_bppt/id_panl_bppt.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.923158 seacrowd-0.0.6/seacrowd/sea_datasets/id_qqp/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_qqp/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4686 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_qqp/id_qqp.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.944203 seacrowd-0.0.6/seacrowd/sea_datasets/id_sent_emo_mobile_apps/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_sent_emo_mobile_apps/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5395 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_sent_emo_mobile_apps/id_sent_emo_mobile_apps.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.961114 seacrowd-0.0.6/seacrowd/sea_datasets/id_sentiment_analysis/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_sentiment_analysis/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5538 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_sentiment_analysis/id_sentiment_analysis.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.981440 seacrowd-0.0.6/seacrowd/sea_datasets/id_short_answer_grading/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_short_answer_grading/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9107 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_short_answer_grading/id_short_answer_grading.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.998930 seacrowd-0.0.6/seacrowd/sea_datasets/id_short_answer_grading/utils/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_short_answer_grading/utils/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1826 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_short_answer_grading/utils/id_short_answer_grading_utils.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.019605 seacrowd-0.0.6/seacrowd/sea_datasets/id_stance/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_stance/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5114 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_stance/id_stance.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.039297 seacrowd-0.0.6/seacrowd/sea_datasets/id_sts/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_sts/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4308 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_sts/id_sts.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.073196 seacrowd-0.0.6/seacrowd/sea_datasets/id_vaccines_tweets/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_vaccines_tweets/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4329 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_vaccines_tweets/id_vaccines_tweets.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.099644 seacrowd-0.0.6/seacrowd/sea_datasets/id_wiki_parallel/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_wiki_parallel/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6697 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_wiki_parallel/id_wiki_parallel.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.122231 seacrowd-0.0.6/seacrowd/sea_datasets/id_wsd/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_wsd/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6404 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_wsd/id_wsd.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.149399 seacrowd-0.0.6/seacrowd/sea_datasets/identic/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/identic/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    13357 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/identic/identic.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.170225 seacrowd-0.0.6/seacrowd/sea_datasets/identifikasi_bahasa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/identifikasi_bahasa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5177 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/identifikasi_bahasa/identifikasi_bahasa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.190050 seacrowd-0.0.6/seacrowd/sea_datasets/idk_mrc/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/idk_mrc/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9530 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/idk_mrc/idk_mrc.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.217169 seacrowd-0.0.6/seacrowd/sea_datasets/idn_tagged_corpus_csui/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/idn_tagged_corpus_csui/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6193 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/idn_tagged_corpus_csui/idn_tagged_corpus_csui.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.244659 seacrowd-0.0.6/seacrowd/sea_datasets/ijelid/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/ijelid/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5403 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/ijelid/ijelid.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.273919 seacrowd-0.0.6/seacrowd/sea_datasets/imdb_jv/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/imdb_jv/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4894 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/imdb_jv/imdb_jv.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.293300 seacrowd-0.0.6/seacrowd/sea_datasets/indo4b/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indo4b/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7236 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indo4b/indo4b.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.314059 seacrowd-0.0.6/seacrowd/sea_datasets/indo4b_plus/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indo4b_plus/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7417 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indo4b_plus/indo4b_plus.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.337684 seacrowd-0.0.6/seacrowd/sea_datasets/indo_general_mt_en_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indo_general_mt_en_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6442 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indo_general_mt_en_id/indo_general_mt_en_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.359122 seacrowd-0.0.6/seacrowd/sea_datasets/indo_law/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indo_law/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5445 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indo_law/indo_law.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.382674 seacrowd-0.0.6/seacrowd/sea_datasets/indo_puisi/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indo_puisi/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4018 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indo_puisi/indo_puisi.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.418853 seacrowd-0.0.6/seacrowd/sea_datasets/indo_religious_mt_en_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indo_religious_mt_en_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8507 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indo_religious_mt_en_id/indo_religious_mt_en_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.440682 seacrowd-0.0.6/seacrowd/sea_datasets/indo_story_cloze/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indo_story_cloze/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6563 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indo_story_cloze/indo_story_cloze.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.464337 seacrowd-0.0.6/seacrowd/sea_datasets/indocamrest/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indocamrest/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6670 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indocamrest/indocamrest.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.487101 seacrowd-0.0.6/seacrowd/sea_datasets/indocollex/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indocollex/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6949 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indocollex/indocollex.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.512342 seacrowd-0.0.6/seacrowd/sea_datasets/indocoref/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indocoref/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    11610 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indocoref/indocoref.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.564345 seacrowd-0.0.6/seacrowd/sea_datasets/indocoref/utils/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indocoref/utils/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9072 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indocoref/utils/feature_utils.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     2091 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indocoref/utils/file_utils.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4307 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indocoref/utils/text_preprocess.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.588729 seacrowd-0.0.6/seacrowd/sea_datasets/indolem_ner_ugm/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indolem_ner_ugm/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6402 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indolem_ner_ugm/indolem_ner_ugm.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.609922 seacrowd-0.0.6/seacrowd/sea_datasets/indolem_nerui/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indolem_nerui/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8192 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indolem_nerui/indolem_nerui.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.630316 seacrowd-0.0.6/seacrowd/sea_datasets/indolem_ntp/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indolem_ntp/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5885 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indolem_ntp/indolem_ntp.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.652099 seacrowd-0.0.6/seacrowd/sea_datasets/indolem_sentiment/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indolem_sentiment/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    12679 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indolem_sentiment/indolem_sentiment.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.671427 seacrowd-0.0.6/seacrowd/sea_datasets/indolem_tweet_ordering/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indolem_tweet_ordering/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    12454 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indolem_tweet_ordering/indolem_tweet_ordering.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.691835 seacrowd-0.0.6/seacrowd/sea_datasets/indolem_ud_id_gsd/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indolem_ud_id_gsd/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8462 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indolem_ud_id_gsd/indolem_ud_id_gsd.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.712359 seacrowd-0.0.6/seacrowd/sea_datasets/indolem_ud_id_pud/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indolem_ud_id_pud/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8825 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indolem_ud_id_pud/indolem_ud_id_pud.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.731063 seacrowd-0.0.6/seacrowd/sea_datasets/indoler/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indoler/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9100 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indoler/indoler.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.749482 seacrowd-0.0.6/seacrowd/sea_datasets/indommlu/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indommlu/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10934 2024-04-11 08:39:41.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indommlu/indommlu.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.769543 seacrowd-0.0.6/seacrowd/sea_datasets/indoner_tourism/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indoner_tourism/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8394 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indoner_tourism/indoner_tourism.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.787605 seacrowd-0.0.6/seacrowd/sea_datasets/indonesia_chinese_mtrobusteval/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indonesia_chinese_mtrobusteval/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5250 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indonesia_chinese_mtrobusteval/indonesia_chinese_mtrobusteval.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.810219 seacrowd-0.0.6/seacrowd/sea_datasets/indonesian_madurese_bible_translation/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indonesian_madurese_bible_translation/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7932 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indonesian_madurese_bible_translation/indonesian_madurese_bible_translation.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.829474 seacrowd-0.0.6/seacrowd/sea_datasets/indonesian_news_dataset/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indonesian_news_dataset/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4581 2024-04-11 08:39:41.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indonesian_news_dataset/indonesian_news_dataset.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.848476 seacrowd-0.0.6/seacrowd/sea_datasets/indonesiannmt/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indonesiannmt/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9148 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indonesiannmt/indonesiannmt.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.868241 seacrowd-0.0.6/seacrowd/sea_datasets/indonglish/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indonglish/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8339 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indonglish/indonglish.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.887867 seacrowd-0.0.6/seacrowd/sea_datasets/indonli/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indonli/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8050 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indonli/indonli.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.907031 seacrowd-0.0.6/seacrowd/sea_datasets/indonlu_nergrit/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indonlu_nergrit/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5677 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indonlu_nergrit/indonlu_nergrit.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.925615 seacrowd-0.0.6/seacrowd/sea_datasets/indoqa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indoqa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5422 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indoqa/indoqa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.944445 seacrowd-0.0.6/seacrowd/sea_datasets/indosmd/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indosmd/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    13550 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indosmd/indosmd.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.961796 seacrowd-0.0.6/seacrowd/sea_datasets/indosum/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indosum/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6872 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indosum/indosum.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.984010 seacrowd-0.0.6/seacrowd/sea_datasets/indotacos/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indotacos/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5477 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indotacos/indotacos.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.002761 seacrowd-0.0.6/seacrowd/sea_datasets/indowiki/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indowiki/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7684 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indowiki/indowiki.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.021235 seacrowd-0.0.6/seacrowd/sea_datasets/indqner/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        1 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indqner/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6614 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indqner/indqner.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.036397 seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_digit_cdsr/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_digit_cdsr/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9856 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_digit_cdsr/indspeech_digit_cdsr.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.055601 seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_news_ethnicsr/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_news_ethnicsr/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8440 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_news_ethnicsr/indspeech_news_ethnicsr.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.077458 seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_news_lvcsr/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_news_lvcsr/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9432 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_news_lvcsr/indspeech_news_lvcsr.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.097760 seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_news_tts/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_news_tts/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8857 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_news_tts/indspeech_news_tts.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.116918 seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_newstra_ethnicsr/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_newstra_ethnicsr/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    11615 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_newstra_ethnicsr/indspeech_newstra_ethnicsr.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.136618 seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_teldialog_lvcsr/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_teldialog_lvcsr/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9932 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_teldialog_lvcsr/indspeech_teldialog_lvcsr.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.156815 seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_teldialog_svcsr/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_teldialog_svcsr/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9818 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_teldialog_svcsr/indspeech_teldialog_svcsr.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.180791 seacrowd-0.0.6/seacrowd/sea_datasets/inset_lexicon/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/inset_lexicon/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4829 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/inset_lexicon/inset_lexicon.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.203285 seacrowd-0.0.6/seacrowd/sea_datasets/jadi_ide/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/jadi_ide/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4404 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/jadi_ide/jadi_ide.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.224124 seacrowd-0.0.6/seacrowd/sea_datasets/jv_id_asr/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/jv_id_asr/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6236 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/jv_id_asr/jv_id_asr.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.246083 seacrowd-0.0.6/seacrowd/sea_datasets/jv_id_tts/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/jv_id_tts/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7628 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/jv_id_tts/jv_id_tts.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.265532 seacrowd-0.0.6/seacrowd/sea_datasets/kamus_alay/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/kamus_alay/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5286 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/kamus_alay/kamus_alay.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.284753 seacrowd-0.0.6/seacrowd/sea_datasets/karonese_sentiment/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/karonese_sentiment/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4533 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/karonese_sentiment/karonese_sentiment.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.306271 seacrowd-0.0.6/seacrowd/sea_datasets/kawat/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/kawat/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5933 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/kawat/kawat.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.332834 seacrowd-0.0.6/seacrowd/sea_datasets/kde4/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/kde4/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    14408 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/kde4/kde4.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.352141 seacrowd-0.0.6/seacrowd/sea_datasets/keps/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/keps/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5066 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/keps/keps.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.377063 seacrowd-0.0.6/seacrowd/sea_datasets/kheng_info/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/kheng_info/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3687 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/kheng_info/kheng_info.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.398409 seacrowd-0.0.6/seacrowd/sea_datasets/khmer_alt_pos/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/khmer_alt_pos/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7442 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/khmer_alt_pos/khmer_alt_pos.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.425789 seacrowd-0.0.6/seacrowd/sea_datasets/khpos/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/khpos/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8756 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/khpos/khpos.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.450333 seacrowd-0.0.6/seacrowd/sea_datasets/kopi_cc/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/kopi_cc/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10035 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/kopi_cc/kopi_cc.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.472020 seacrowd-0.0.6/seacrowd/sea_datasets/kopi_cc_news/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/kopi_cc_news/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5088 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/kopi_cc_news/kopi_cc_news.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.491281 seacrowd-0.0.6/seacrowd/sea_datasets/kopi_nllb/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/kopi_nllb/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5956 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/kopi_nllb/kopi_nllb.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.510706 seacrowd-0.0.6/seacrowd/sea_datasets/korpus_nusantara/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/korpus_nusantara/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8476 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/korpus_nusantara/korpus_nusantara.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.529386 seacrowd-0.0.6/seacrowd/sea_datasets/lazada_review_filipino/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/lazada_review_filipino/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4913 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/lazada_review_filipino/lazada_review_filipino.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.548696 seacrowd-0.0.6/seacrowd/sea_datasets/librivox_indonesia/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/librivox_indonesia/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8736 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/librivox_indonesia/librivox_indonesia.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.568334 seacrowd-0.0.6/seacrowd/sea_datasets/limesoda/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/limesoda/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6775 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/limesoda/limesoda.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.590361 seacrowd-0.0.6/seacrowd/sea_datasets/liputan6/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/liputan6/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7512 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/liputan6/liputan6.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.610947 seacrowd-0.0.6/seacrowd/sea_datasets/local_id_abusive/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/local_id_abusive/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7530 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/local_id_abusive/local_id_abusive.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.631210 seacrowd-0.0.6/seacrowd/sea_datasets/lr_sum/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/lr_sum/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6160 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/lr_sum/lr_sum.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.659269 seacrowd-0.0.6/seacrowd/sea_datasets/m3exam/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/m3exam/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    14637 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/m3exam/m3exam.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.685192 seacrowd-0.0.6/seacrowd/sea_datasets/mabl/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/mabl/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8609 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/mabl/mabl.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.705454 seacrowd-0.0.6/seacrowd/sea_datasets/malaysia_tweets/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/malaysia_tweets/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6432 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/malaysia_tweets/malaysia_tweets.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.728278 seacrowd-0.0.6/seacrowd/sea_datasets/malindo_morph/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/malindo_morph/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4617 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/malindo_morph/malindo_morph.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.746300 seacrowd-0.0.6/seacrowd/sea_datasets/malindo_parallel/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/malindo_parallel/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6494 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/malindo_parallel/malindo_parallel.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.771053 seacrowd-0.0.6/seacrowd/sea_datasets/massive/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/massive/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    18420 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/massive/massive.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.792771 seacrowd-0.0.6/seacrowd/sea_datasets/mc4_indo/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/mc4_indo/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5510 2024-04-11 08:39:41.000000 seacrowd-0.0.6/seacrowd/sea_datasets/mc4_indo/mc4_indo.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.811734 seacrowd-0.0.6/seacrowd/sea_datasets/melayu_brunei/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/melayu_brunei/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10682 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/melayu_brunei/melayu_brunei.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.832739 seacrowd-0.0.6/seacrowd/sea_datasets/melayu_sabah/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/melayu_sabah/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5561 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/melayu_sabah/melayu_sabah.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.851137 seacrowd-0.0.6/seacrowd/sea_datasets/melayu_sarawak/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/melayu_sarawak/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6559 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/melayu_sarawak/melayu_sarawak.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.869954 seacrowd-0.0.6/seacrowd/sea_datasets/melayu_standard_lisan/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/melayu_standard_lisan/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7594 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/melayu_standard_lisan/melayu_standard_lisan.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.887035 seacrowd-0.0.6/seacrowd/sea_datasets/memolon/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/memolon/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5589 2024-04-11 08:39:41.000000 seacrowd-0.0.6/seacrowd/sea_datasets/memolon/memolon.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.907814 seacrowd-0.0.6/seacrowd/sea_datasets/minangnlp_mt/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/minangnlp_mt/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6874 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/minangnlp_mt/minangnlp_mt.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.927611 seacrowd-0.0.6/seacrowd/sea_datasets/miracl/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/miracl/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    13119 2024-04-11 08:39:41.000000 seacrowd-0.0.6/seacrowd/sea_datasets/miracl/miracl.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.948262 seacrowd-0.0.6/seacrowd/sea_datasets/mkqa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/mkqa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8345 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/mkqa/mkqa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.971349 seacrowd-0.0.6/seacrowd/sea_datasets/mlqa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        1 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/mlqa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9825 2024-04-11 08:39:41.000000 seacrowd-0.0.6/seacrowd/sea_datasets/mlqa/mlqa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.994086 seacrowd-0.0.6/seacrowd/sea_datasets/mozilla_pontoon/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/mozilla_pontoon/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6211 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/mozilla_pontoon/mozilla_pontoon.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.024238 seacrowd-0.0.6/seacrowd/sea_datasets/mswc/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/mswc/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8048 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/mswc/mswc.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.054345 seacrowd-0.0.6/seacrowd/sea_datasets/mtop_intent_classification/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/mtop_intent_classification/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     2654 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/mtop_intent_classification/labels.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5662 2024-04-11 08:39:41.000000 seacrowd-0.0.6/seacrowd/sea_datasets/mtop_intent_classification/mtop_intent_classification.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.075330 seacrowd-0.0.6/seacrowd/sea_datasets/multilexnorm/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/multilexnorm/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6223 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/multilexnorm/multilexnorm.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.096930 seacrowd-0.0.6/seacrowd/sea_datasets/my_paraphrase/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/my_paraphrase/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8124 2024-04-11 08:39:41.000000 seacrowd-0.0.6/seacrowd/sea_datasets/my_paraphrase/my_paraphrase.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.119908 seacrowd-0.0.6/seacrowd/sea_datasets/myanmar_rakhine_parallel/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/myanmar_rakhine_parallel/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7223 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/myanmar_rakhine_parallel/myanmar_rakhine_parallel.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.142628 seacrowd-0.0.6/seacrowd/sea_datasets/mypos/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/mypos/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5116 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/mypos/mypos.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.162927 seacrowd-0.0.6/seacrowd/sea_datasets/mysentence/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/mysentence/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7612 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/mysentence/mysentence.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.182927 seacrowd-0.0.6/seacrowd/sea_datasets/myxnli/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/myxnli/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5096 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/myxnli/myxnli.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.201681 seacrowd-0.0.6/seacrowd/sea_datasets/nergrit/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/nergrit/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6322 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/nergrit/nergrit.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.220345 seacrowd-0.0.6/seacrowd/sea_datasets/nerp/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/nerp/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4852 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/nerp/nerp.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.240939 seacrowd-0.0.6/seacrowd/sea_datasets/netifier/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/netifier/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4838 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/netifier/netifier.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.262756 seacrowd-0.0.6/seacrowd/sea_datasets/news_en_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/news_en_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5003 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/news_en_id/news_en_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.283584 seacrowd-0.0.6/seacrowd/sea_datasets/newsph/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/newsph/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3810 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/newsph/newsph.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.302819 seacrowd-0.0.6/seacrowd/sea_datasets/nllb_seed/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/nllb_seed/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    15208 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/nllb_seed/nllb_seed.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.319712 seacrowd-0.0.6/seacrowd/sea_datasets/ntrex_128/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/ntrex_128/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10971 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/ntrex_128/ntrex_128.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.355007 seacrowd-0.0.6/seacrowd/sea_datasets/nusaparagraph_emot/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/nusaparagraph_emot/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8785 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/nusaparagraph_emot/nusaparagraph_emot.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.377840 seacrowd-0.0.6/seacrowd/sea_datasets/nusaparagraph_rhetoric/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/nusaparagraph_rhetoric/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8792 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/nusaparagraph_rhetoric/nusaparagraph_rhetoric.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.397230 seacrowd-0.0.6/seacrowd/sea_datasets/nusaparagraph_topic/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/nusaparagraph_topic/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8845 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/nusaparagraph_topic/nusaparagraph_topic.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.416960 seacrowd-0.0.6/seacrowd/sea_datasets/nusatranslation_emot/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/nusatranslation_emot/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8233 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/nusatranslation_emot/nusatranslation_emot.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.438103 seacrowd-0.0.6/seacrowd/sea_datasets/nusatranslation_mt/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/nusatranslation_mt/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9156 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/nusatranslation_mt/nusatranslation_mt.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.465473 seacrowd-0.0.6/seacrowd/sea_datasets/nusatranslation_senti/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/nusatranslation_senti/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8285 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/nusatranslation_senti/nusatranslation_senti.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.485183 seacrowd-0.0.6/seacrowd/sea_datasets/nusax_mt/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/nusax_mt/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7578 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/nusax_mt/nusax_mt.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.506795 seacrowd-0.0.6/seacrowd/sea_datasets/nusax_senti/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/nusax_senti/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7250 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/nusax_senti/nusax_senti.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.526569 seacrowd-0.0.6/seacrowd/sea_datasets/oil/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/oil/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5477 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/oil/oil.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.547104 seacrowd-0.0.6/seacrowd/sea_datasets/ojw/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/ojw/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5110 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/ojw/ojw.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.565774 seacrowd-0.0.6/seacrowd/sea_datasets/openlid/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/openlid/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7915 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/openlid/openlid.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.585778 seacrowd-0.0.6/seacrowd/sea_datasets/openslr/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/openslr/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10343 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/openslr/openslr.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.613775 seacrowd-0.0.6/seacrowd/sea_datasets/orchid_pos/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/orchid_pos/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9625 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/orchid_pos/orchid_pos.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.633731 seacrowd-0.0.6/seacrowd/sea_datasets/oscar_2201/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/oscar_2201/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    16270 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/oscar_2201/oscar_2201.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.655182 seacrowd-0.0.6/seacrowd/sea_datasets/palito/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/palito/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5930 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/palito/palito.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.674421 seacrowd-0.0.6/seacrowd/sea_datasets/paracotta_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/paracotta_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4768 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/paracotta_id/paracotta_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.693919 seacrowd-0.0.6/seacrowd/sea_datasets/parallel_id_nyo/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/parallel_id_nyo/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5471 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/parallel_id_nyo/parallel_id_nyo.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.710989 seacrowd-0.0.6/seacrowd/sea_datasets/parallel_su_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/parallel_su_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4782 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/parallel_su_id/parallel_su_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.734097 seacrowd-0.0.6/seacrowd/sea_datasets/ph_fake_news_corpus/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/ph_fake_news_corpus/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4339 2024-04-11 08:39:41.000000 seacrowd-0.0.6/seacrowd/sea_datasets/ph_fake_news_corpus/ph_fake_news_corpus.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.756381 seacrowd-0.0.6/seacrowd/sea_datasets/pho_ner_covid/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/pho_ner_covid/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6866 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/pho_ner_covid/pho_ner_covid.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.774104 seacrowd-0.0.6/seacrowd/sea_datasets/phomt/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/phomt/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5141 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/phomt/phomt.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.793708 seacrowd-0.0.6/seacrowd/sea_datasets/phost/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/phost/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9498 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/phost/phost.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.814098 seacrowd-0.0.6/seacrowd/sea_datasets/posp/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/posp/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5990 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/posp/posp.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.833201 seacrowd-0.0.6/seacrowd/sea_datasets/postag_su/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/postag_su/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8033 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/postag_su/postag_su.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.854553 seacrowd-0.0.6/seacrowd/sea_datasets/prdect_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/prdect_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7572 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/prdect_id/prdect_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.884638 seacrowd-0.0.6/seacrowd/sea_datasets/qasina/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/qasina/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6424 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/qasina/qasina.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.903931 seacrowd-0.0.6/seacrowd/sea_datasets/roots_vi_ted/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/roots_vi_ted/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5065 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/roots_vi_ted/roots_vi_ted.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.925362 seacrowd-0.0.6/seacrowd/sea_datasets/sampiran/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/sampiran/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5024 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/sampiran/sampiran.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.954764 seacrowd-0.0.6/seacrowd/sea_datasets/sap_wat/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/sap_wat/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7077 2024-04-11 08:39:41.000000 seacrowd-0.0.6/seacrowd/sea_datasets/sap_wat/sap_wat.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.977381 seacrowd-0.0.6/seacrowd/sea_datasets/sarawak_malay/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/sarawak_malay/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7381 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/sarawak_malay/sarawak_malay.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.995690 seacrowd-0.0.6/seacrowd/sea_datasets/scb_mt_en_th/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/scb_mt_en_th/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7071 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/scb_mt_en_th/scb_mt_en_th.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.020982 seacrowd-0.0.6/seacrowd/sea_datasets/sea_bench/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/sea_bench/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7206 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/sea_bench/sea_bench.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.045137 seacrowd-0.0.6/seacrowd/sea_datasets/sea_madlad/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/sea_madlad/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10051 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/sea_madlad/sea_madlad.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.080157 seacrowd-0.0.6/seacrowd/sea_datasets/sea_wiki/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/sea_wiki/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1829 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/sea_wiki/lang_config.json
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9350 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/sea_wiki/sea_wiki.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.100232 seacrowd-0.0.6/seacrowd/sea_datasets/seaeval/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/seaeval/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9350 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/seaeval/seaeval.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.120085 seacrowd-0.0.6/seacrowd/sea_datasets/seahorse/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/seahorse/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6884 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/seahorse/seahorse.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.139474 seacrowd-0.0.6/seacrowd/sea_datasets/sentiment_nathasa_review/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/sentiment_nathasa_review/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6002 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/sentiment_nathasa_review/sentiment_nathasa_review.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.158288 seacrowd-0.0.6/seacrowd/sea_datasets/shopee_reviews_tagalog/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/shopee_reviews_tagalog/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4597 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/shopee_reviews_tagalog/shopee_reviews_tagalog.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.175538 seacrowd-0.0.6/seacrowd/sea_datasets/singgalang/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/singgalang/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5430 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/singgalang/singgalang.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.194957 seacrowd-0.0.6/seacrowd/sea_datasets/smsa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/smsa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5575 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/smsa/smsa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.214265 seacrowd-0.0.6/seacrowd/sea_datasets/snli_indo/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/snli_indo/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6244 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/snli_indo/snli_indo.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.235054 seacrowd-0.0.6/seacrowd/sea_datasets/spamid_pair/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/spamid_pair/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5524 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/spamid_pair/spamid_pair.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.254263 seacrowd-0.0.6/seacrowd/sea_datasets/squad_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/squad_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5315 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/squad_id/squad_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.271852 seacrowd-0.0.6/seacrowd/sea_datasets/stb_ext/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/stb_ext/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9273 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/stb_ext/stb_ext.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.290865 seacrowd-0.0.6/seacrowd/sea_datasets/stif_indonesia/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/stif_indonesia/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5135 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/stif_indonesia/stif_indonesia.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.312547 seacrowd-0.0.6/seacrowd/sea_datasets/struct_amb_ind/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/struct_amb_ind/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7724 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/struct_amb_ind/struct_amb_ind.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.334159 seacrowd-0.0.6/seacrowd/sea_datasets/su_emot/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/su_emot/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4567 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/su_emot/su_emot.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.353250 seacrowd-0.0.6/seacrowd/sea_datasets/su_id_asr/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/su_id_asr/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5601 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/su_id_asr/su_id_asr.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.369887 seacrowd-0.0.6/seacrowd/sea_datasets/su_id_tts/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/su_id_tts/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7636 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/su_id_tts/su_id_tts.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.391168 seacrowd-0.0.6/seacrowd/sea_datasets/talpco/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/talpco/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6870 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/talpco/talpco.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.410038 seacrowd-0.0.6/seacrowd/sea_datasets/tatabahasa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/tatabahasa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5411 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/tatabahasa/tatabahasa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.430492 seacrowd-0.0.6/seacrowd/sea_datasets/tatoeba/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/tatoeba/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7636 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/tatoeba/tatoeba.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.451051 seacrowd-0.0.6/seacrowd/sea_datasets/tcope/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/tcope/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6693 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/tcope/tcope.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.471554 seacrowd-0.0.6/seacrowd/sea_datasets/ted_en_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/ted_en_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7105 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/ted_en_id/ted_en_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.491820 seacrowd-0.0.6/seacrowd/sea_datasets/term_a/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/term_a/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5358 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/term_a/term_a.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.512615 seacrowd-0.0.6/seacrowd/sea_datasets/tgl_profanity/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/tgl_profanity/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4351 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/tgl_profanity/tgl_profanity.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.530491 seacrowd-0.0.6/seacrowd/sea_datasets/tha_lao_embassy_parcor/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/tha_lao_embassy_parcor/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4436 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/tha_lao_embassy_parcor/tha_lao_embassy_parcor.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.550752 seacrowd-0.0.6/seacrowd/sea_datasets/thai_alpaca/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/thai_alpaca/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3943 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/thai_alpaca/thai_alpaca.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.569334 seacrowd-0.0.6/seacrowd/sea_datasets/thai_constitution/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/thai_constitution/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10954 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/thai_constitution/thai_constitution.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.590187 seacrowd-0.0.6/seacrowd/sea_datasets/thai_databricks_dolly/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/thai_databricks_dolly/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4388 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/thai_databricks_dolly/thai_databricks_dolly.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.610185 seacrowd-0.0.6/seacrowd/sea_datasets/thai_depression/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/thai_depression/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5739 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/thai_depression/thai_depression.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.629439 seacrowd-0.0.6/seacrowd/sea_datasets/thai_gpteacher/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/thai_gpteacher/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3960 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/thai_gpteacher/thai_gpteacher.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.649549 seacrowd-0.0.6/seacrowd/sea_datasets/thai_hh_rlhf/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/thai_hh_rlhf/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5077 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/thai_hh_rlhf/thai_hh_rlhf.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.668593 seacrowd-0.0.6/seacrowd/sea_datasets/thai_sum/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/thai_sum/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5683 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/thai_sum/thai_sum.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.693104 seacrowd-0.0.6/seacrowd/sea_datasets/thai_toxicity_tweet/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/thai_toxicity_tweet/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4555 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/thai_toxicity_tweet/thai_toxicity_tweet.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.712448 seacrowd-0.0.6/seacrowd/sea_datasets/tico_19/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/tico_19/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    12192 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/tico_19/tico_19.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.730671 seacrowd-0.0.6/seacrowd/sea_datasets/titml_idn/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/titml_idn/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5900 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/titml_idn/titml_idn.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.749801 seacrowd-0.0.6/seacrowd/sea_datasets/tlunified_ner/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/tlunified_ner/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5800 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/tlunified_ner/tlunified_ner.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.771364 seacrowd-0.0.6/seacrowd/sea_datasets/toxicity_200/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/toxicity_200/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5975 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/toxicity_200/toxicity_200.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.790921 seacrowd-0.0.6/seacrowd/sea_datasets/tydiqa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/tydiqa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    23881 2024-04-11 08:39:41.000000 seacrowd-0.0.6/seacrowd/sea_datasets/tydiqa/tydiqa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.813641 seacrowd-0.0.6/seacrowd/sea_datasets/typhoon_yolanda_tweets/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        1 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/typhoon_yolanda_tweets/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5165 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/typhoon_yolanda_tweets/typhoon_yolanda_tweets.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.835234 seacrowd-0.0.6/seacrowd/sea_datasets/ucla_phonetic/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/ucla_phonetic/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6531 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/ucla_phonetic/ucla_phonetic.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.867533 seacrowd-0.0.6/seacrowd/sea_datasets/ud_id_csui/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/ud_id_csui/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9185 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/ud_id_csui/ud_id_csui.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.896691 seacrowd-0.0.6/seacrowd/sea_datasets/ud_jv_csui/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/ud_jv_csui/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10052 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/ud_jv_csui/ud_jv_csui.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.919987 seacrowd-0.0.6/seacrowd/sea_datasets/udhr/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/udhr/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6030 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/udhr/udhr.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.936703 seacrowd-0.0.6/seacrowd/sea_datasets/udhr_lid/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/udhr_lid/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5190 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/udhr_lid/udhr_lid.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.964902 seacrowd-0.0.6/seacrowd/sea_datasets/uit_vicov19qa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/uit_vicov19qa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7244 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/uit_vicov19qa/uit_vicov19qa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.993713 seacrowd-0.0.6/seacrowd/sea_datasets/uit_victsd/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/uit_victsd/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5311 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/uit_victsd/uit_victsd.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.022732 seacrowd-0.0.6/seacrowd/sea_datasets/uit_vihsd/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/uit_vihsd/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5721 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/uit_vihsd/uit_vihsd.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.059473 seacrowd-0.0.6/seacrowd/sea_datasets/uit_viic/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/uit_viic/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6572 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/uit_viic/uit_viic.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.091222 seacrowd-0.0.6/seacrowd/sea_datasets/uit_viocd/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/uit_viocd/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4819 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/uit_viocd/uit_viocd.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.116615 seacrowd-0.0.6/seacrowd/sea_datasets/uit_vion/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/uit_vion/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5939 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/uit_vion/uit_vion.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.158425 seacrowd-0.0.6/seacrowd/sea_datasets/uit_visd4sa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/uit_visd4sa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7034 2024-04-11 08:39:41.000000 seacrowd-0.0.6/seacrowd/sea_datasets/uit_visd4sa/uit_visd4sa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.187888 seacrowd-0.0.6/seacrowd/sea_datasets/uit_vsfc/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/uit_vsfc/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8715 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/uit_vsfc/uit_vsfc.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.210728 seacrowd-0.0.6/seacrowd/sea_datasets/uit_vsmec/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/uit_vsmec/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4802 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/uit_vsmec/uit_vsmec.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.244139 seacrowd-0.0.6/seacrowd/sea_datasets/unimorph/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/unimorph/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    15492 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/unimorph/unimorph.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.268184 seacrowd-0.0.6/seacrowd/sea_datasets/unimorph_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/unimorph_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7445 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/unimorph_id/unimorph_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.300159 seacrowd-0.0.6/seacrowd/sea_datasets/vi_pubmed/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/vi_pubmed/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    15136 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/vi_pubmed/vi_pubmed.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.355915 seacrowd-0.0.6/seacrowd/sea_datasets/vihealthqa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/vihealthqa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5587 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/vihealthqa/vihealthqa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.381141 seacrowd-0.0.6/seacrowd/sea_datasets/visobert/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/visobert/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6265 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/visobert/visobert.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.409133 seacrowd-0.0.6/seacrowd/sea_datasets/vispamreviews/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/vispamreviews/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7245 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/vispamreviews/vispamreviews.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.445508 seacrowd-0.0.6/seacrowd/sea_datasets/vistec_tp_th_21/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/vistec_tp_th_21/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6739 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/vistec_tp_th_21/vistec_tp_th_21.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.471518 seacrowd-0.0.6/seacrowd/sea_datasets/vitext2sql/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/vitext2sql/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6893 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/vitext2sql/vitext2sql.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.498382 seacrowd-0.0.6/seacrowd/sea_datasets/vivos/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/vivos/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7832 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/vivos/vivos.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.524840 seacrowd-0.0.6/seacrowd/sea_datasets/vivqa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/vivqa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9080 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/vivqa/vivqa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.544552 seacrowd-0.0.6/seacrowd/sea_datasets/vlsp2016_ner/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/vlsp2016_ner/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5857 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/vlsp2016_ner/vlsp2016_ner.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.570179 seacrowd-0.0.6/seacrowd/sea_datasets/vlsp2016_sa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/vlsp2016_sa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7134 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/vlsp2016_sa/vlsp2016_sa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.618434 seacrowd-0.0.6/seacrowd/sea_datasets/vndt/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/vndt/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     2232 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/vndt/utils.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7852 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/vndt/vndt.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.637585 seacrowd-0.0.6/seacrowd/sea_datasets/voxlingua/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/voxlingua/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7980 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/voxlingua/voxlingua.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.661093 seacrowd-0.0.6/seacrowd/sea_datasets/weathub/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/weathub/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7521 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/weathub/weathub.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.681222 seacrowd-0.0.6/seacrowd/sea_datasets/wikiann/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/wikiann/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8643 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/wikiann/wikiann.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.700781 seacrowd-0.0.6/seacrowd/sea_datasets/wikilingua/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/wikilingua/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4984 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/wikilingua/wikilingua.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.720214 seacrowd-0.0.6/seacrowd/sea_datasets/wikimatrix/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/wikimatrix/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8585 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/wikimatrix/wikimatrix.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.749112 seacrowd-0.0.6/seacrowd/sea_datasets/wikitext_tl_39/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/wikitext_tl_39/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3663 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/wikitext_tl_39/wikitext_tl_39.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.780130 seacrowd-0.0.6/seacrowd/sea_datasets/wili_2018/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/wili_2018/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6699 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/wili_2018/wili_2018.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.799674 seacrowd-0.0.6/seacrowd/sea_datasets/wisesight_thai_sentiment/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/wisesight_thai_sentiment/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7027 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/wisesight_thai_sentiment/wisesight_thai_sentiment.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.827694 seacrowd-0.0.6/seacrowd/sea_datasets/wit/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/wit/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    12057 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/wit/wit.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.850932 seacrowd-0.0.6/seacrowd/sea_datasets/wongnai_reviews/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/wongnai_reviews/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4106 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/wongnai_reviews/wongnai_reviews.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.868850 seacrowd-0.0.6/seacrowd/sea_datasets/wrete/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/wrete/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6113 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/wrete/wrete.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.885963 seacrowd-0.0.6/seacrowd/sea_datasets/x_fact/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/x_fact/__init__.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.905417 seacrowd-0.0.6/seacrowd/sea_datasets/x_fact/utils/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/x_fact/utils/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      473 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/x_fact/utils/x_fact_utils.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5900 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/x_fact/x_fact.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.935194 seacrowd-0.0.6/seacrowd/sea_datasets/xcopa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/xcopa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7024 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/xcopa/xcopa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.961232 seacrowd-0.0.6/seacrowd/sea_datasets/xl_jailbreak/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/xl_jailbreak/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6317 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/xl_jailbreak/xl_jailbreak.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.978210 seacrowd-0.0.6/seacrowd/sea_datasets/xl_sum/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/xl_sum/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6903 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/xl_sum/xl_sum.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.995494 seacrowd-0.0.6/seacrowd/sea_datasets/xm3600/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/xm3600/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8233 2024-04-11 08:39:41.000000 seacrowd-0.0.6/seacrowd/sea_datasets/xm3600/xm3600.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:54.043503 seacrowd-0.0.6/seacrowd/sea_datasets/xnli/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/xnli/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8333 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/xnli/xnli.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:54.085793 seacrowd-0.0.6/seacrowd/sea_datasets/xpersona_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/xpersona_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6550 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/xpersona_id/xpersona_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:54.106224 seacrowd-0.0.6/seacrowd/sea_datasets/xquad/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/xquad/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4819 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/xquad/xquad.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:54.146233 seacrowd-0.0.6/seacrowd/sea_datasets/xsid/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/sea_datasets/xsid/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9510 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/sea_datasets/xsid/xsid.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:54.166886 seacrowd-0.0.6/seacrowd/sea_datasets/xstorycloze/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/sea_datasets/xstorycloze/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6794 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/sea_datasets/xstorycloze/xstorycloze.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:54.188320 seacrowd-0.0.6/seacrowd/sea_datasets/yunshan_cup_2020/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/sea_datasets/yunshan_cup_2020/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5828 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/sea_datasets/yunshan_cup_2020/yunshan_cup_2020.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:54.245136 seacrowd-0.0.6/seacrowd/utils/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/utils/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5493 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/utils/common_parser.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      284 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/utils/configs.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    12786 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/utils/constants.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:54.490913 seacrowd-0.0.6/seacrowd/utils/schemas/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1485 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/utils/schemas/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      506 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/utils/schemas/image_text.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1101 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/utils/schemas/imqa.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     2283 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/utils/schemas/kb.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      626 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/utils/schemas/pairs.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      371 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/utils/schemas/pairs_multilabel.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1007 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/utils/schemas/qa.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      206 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/utils/schemas/self_supervised_pretraining.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      525 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/utils/schemas/seq_label.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      618 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/utils/schemas/speech.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      606 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/utils/schemas/speech_multilabel.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      454 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/utils/schemas/speech_text.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      796 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/utils/schemas/speech_to_speech.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      311 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/utils/schemas/text.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      331 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/utils/schemas/text_multilabel.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      444 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/utils/schemas/text_to_text.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3046 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/utils/schemas/tod.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3068 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/utils/schemas/tree.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      810 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/utils/schemas/video.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:54.560764 seacrowd-0.0.6/seacrowd.egg-info/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1071 2024-04-12 07:28:43.000000 seacrowd-0.0.6/seacrowd.egg-info/PKG-INFO
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    31371 2024-04-12 07:28:44.000000 seacrowd-0.0.6/seacrowd.egg-info/SOURCES.txt
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        1 2024-04-12 07:28:43.000000 seacrowd-0.0.6/seacrowd.egg-info/dependency_links.txt
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      409 2024-04-12 07:28:43.000000 seacrowd-0.0.6/seacrowd.egg-info/requires.txt
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)       15 2024-04-12 07:28:43.000000 seacrowd-0.0.6/seacrowd.egg-info/top_level.txt
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      703 2024-04-12 07:28:54.593051 seacrowd-0.0.6/setup.cfg
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)       68 2024-04-12 07:28:29.000000 seacrowd-0.0.6/setup.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:54.541365 seacrowd-0.0.6/tests/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:52.000000 seacrowd-0.0.6/tests/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    23314 2024-04-04 06:00:52.000000 seacrowd-0.0.6/tests/test_seacrowd.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    20714 2024-04-04 06:00:52.000000 seacrowd-0.0.6/tests/test_seacrowd_source_only.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:57.229260 seacrowd-0.0.7/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    11357 2024-04-04 06:00:44.000000 seacrowd-0.0.7/LICENSE
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1071 2024-04-12 07:52:57.225948 seacrowd-0.0.7/PKG-INFO
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5757 2024-04-04 06:00:44.000000 seacrowd-0.0.7/README.md
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:49.866057 seacrowd-0.0.7/seacrowd/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      251 2024-04-12 07:52:40.000000 seacrowd-0.0.7/seacrowd/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    40451 2024-04-11 08:39:41.000000 seacrowd-0.0.7/seacrowd/config_helper.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:49.940039 seacrowd-0.0.7/seacrowd/sea_datasets/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/__init__.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:49.955731 seacrowd-0.0.7/seacrowd/sea_datasets/abui_wordnet/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/abui_wordnet/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5277 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/abui_wordnet/abui_wordnet.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:49.973441 seacrowd-0.0.7/seacrowd/sea_datasets/alt_burmese_treebank/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/alt_burmese_treebank/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5692 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/alt_burmese_treebank/alt_burmese_treebank.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:49.992809 seacrowd-0.0.7/seacrowd/sea_datasets/alt_burmese_treebank/utils/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/alt_burmese_treebank/utils/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     2661 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/alt_burmese_treebank/utils/alt_burmese_treebank_utils.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:50.016681 seacrowd-0.0.7/seacrowd/sea_datasets/ara_close/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/ara_close/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8227 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/ara_close/ara_close.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:50.034899 seacrowd-0.0.7/seacrowd/sea_datasets/asr_sindodusc/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/asr_sindodusc/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7231 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/asr_sindodusc/asr_sindodusc.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:50.058040 seacrowd-0.0.7/seacrowd/sea_datasets/asr_smaldusc/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/asr_smaldusc/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7305 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/asr_smaldusc/asr_smaldusc.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:50.077296 seacrowd-0.0.7/seacrowd/sea_datasets/asr_stidusc/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/asr_stidusc/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6979 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/asr_stidusc/asr_stidusc.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:50.093819 seacrowd-0.0.7/seacrowd/sea_datasets/audio_keyword_spotting/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/audio_keyword_spotting/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7860 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/audio_keyword_spotting/audio_keyword_spotting.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:50.112904 seacrowd-0.0.7/seacrowd/sea_datasets/aya_dataset/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/aya_dataset/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7482 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/aya_dataset/aya_dataset.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:50.131642 seacrowd-0.0.7/seacrowd/sea_datasets/barasa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/barasa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7224 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/barasa/barasa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:50.157139 seacrowd-0.0.7/seacrowd/sea_datasets/beaye_lexicon/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/beaye_lexicon/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4357 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/beaye_lexicon/beaye_lexicon.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:50.177525 seacrowd-0.0.7/seacrowd/sea_datasets/belebele/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/belebele/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8610 2024-04-11 08:39:41.000000 seacrowd-0.0.7/seacrowd/sea_datasets/belebele/belebele.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:50.196589 seacrowd-0.0.7/seacrowd/sea_datasets/bible_en_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/bible_en_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6790 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/bible_en_id/bible_en_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:50.216491 seacrowd-0.0.7/seacrowd/sea_datasets/bible_jv_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/bible_jv_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6856 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/bible_jv_id/bible_jv_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:50.236173 seacrowd-0.0.7/seacrowd/sea_datasets/bible_su_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/bible_su_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6632 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/bible_su_id/bible_su_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:50.255079 seacrowd-0.0.7/seacrowd/sea_datasets/bioner_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/bioner_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6108 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/bioner_id/bioner_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:50.274134 seacrowd-0.0.7/seacrowd/sea_datasets/bloom_captioning/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/bloom_captioning/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8518 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/bloom_captioning/bloom_captioning.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:50.293646 seacrowd-0.0.7/seacrowd/sea_datasets/bloom_lm/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/bloom_lm/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8430 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/bloom_lm/bloom_lm.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:50.314247 seacrowd-0.0.7/seacrowd/sea_datasets/bloom_speech/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/bloom_speech/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6922 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/bloom_speech/bloom_speech.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:50.332097 seacrowd-0.0.7/seacrowd/sea_datasets/bloom_vist/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/bloom_vist/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9674 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/bloom_vist/bloom_vist.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:50.353269 seacrowd-0.0.7/seacrowd/sea_datasets/burapha_th/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/burapha_th/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6995 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/burapha_th/burapha_th.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:50.371327 seacrowd-0.0.7/seacrowd/sea_datasets/burmese_romanize/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/burmese_romanize/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4420 2024-04-11 08:39:41.000000 seacrowd-0.0.7/seacrowd/sea_datasets/burmese_romanize/burmese_romanize.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:50.393146 seacrowd-0.0.7/seacrowd/sea_datasets/casa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/casa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5635 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/casa/casa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:50.407407 seacrowd-0.0.7/seacrowd/sea_datasets/cc100/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/cc100/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10941 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/cc100/cc100.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:50.424719 seacrowd-0.0.7/seacrowd/sea_datasets/cc_aligned_doc/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/cc_aligned_doc/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6230 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/cc_aligned_doc/cc_aligned_doc.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:50.442417 seacrowd-0.0.7/seacrowd/sea_datasets/cc_aligned_sent/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/cc_aligned_sent/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6256 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/cc_aligned_sent/cc_aligned_sent.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:50.461124 seacrowd-0.0.7/seacrowd/sea_datasets/cebuaner/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/cebuaner/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7783 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/cebuaner/cebuaner.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:50.480247 seacrowd-0.0.7/seacrowd/sea_datasets/coco_35l/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/coco_35l/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9830 2024-04-11 08:39:41.000000 seacrowd-0.0.7/seacrowd/sea_datasets/coco_35l/coco_35l.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:50.503722 seacrowd-0.0.7/seacrowd/sea_datasets/cod/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/cod/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6239 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/cod/cod.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:50.526021 seacrowd-0.0.7/seacrowd/sea_datasets/code_mixed_jv_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/code_mixed_jv_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8760 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/code_mixed_jv_id/code_mixed_jv_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:50.544876 seacrowd-0.0.7/seacrowd/sea_datasets/codeswitch_reddit/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/codeswitch_reddit/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9015 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/codeswitch_reddit/codeswitch_reddit.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:50.596519 seacrowd-0.0.7/seacrowd/sea_datasets/commonvoice_120/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/commonvoice_120/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9438 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/commonvoice_120/commonvoice_120.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:50.617754 seacrowd-0.0.7/seacrowd/sea_datasets/copal/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/copal/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5868 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/copal/copal.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:50.641028 seacrowd-0.0.7/seacrowd/sea_datasets/covost2/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/covost2/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10329 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/covost2/covost2.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:50.659331 seacrowd-0.0.7/seacrowd/sea_datasets/creole_rc/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.7/seacrowd/sea_datasets/creole_rc/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9448 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/creole_rc/creole_rc.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:50.677372 seacrowd-0.0.7/seacrowd/sea_datasets/crosssum/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/crosssum/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5467 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/crosssum/crosssum.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:50.699874 seacrowd-0.0.7/seacrowd/sea_datasets/cub_bahasa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/cub_bahasa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    14495 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/cub_bahasa/cub_bahasa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:50.724771 seacrowd-0.0.7/seacrowd/sea_datasets/culturax/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/culturax/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6383 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/culturax/culturax.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:50.752061 seacrowd-0.0.7/seacrowd/sea_datasets/cvss/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/cvss/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    11054 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/cvss/cvss.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:50.779681 seacrowd-0.0.7/seacrowd/sea_datasets/dengue_filipino/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/dengue_filipino/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4777 2024-04-11 08:39:41.000000 seacrowd-0.0.7/seacrowd/sea_datasets/dengue_filipino/dengue_filipino.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:50.798678 seacrowd-0.0.7/seacrowd/sea_datasets/emot/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/emot/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5522 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/emot/emot.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:50.816913 seacrowd-0.0.7/seacrowd/sea_datasets/emotcmt/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/emotcmt/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4484 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/emotcmt/emotcmt.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:50.834674 seacrowd-0.0.7/seacrowd/sea_datasets/emotes_3k/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/emotes_3k/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9257 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/emotes_3k/emotes_3k.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:50.852768 seacrowd-0.0.7/seacrowd/sea_datasets/emotion_id_opinion/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/emotion_id_opinion/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7315 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/emotion_id_opinion/emotion_id_opinion.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:50.871784 seacrowd-0.0.7/seacrowd/sea_datasets/etos/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/etos/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7041 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/etos/etos.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:50.895965 seacrowd-0.0.7/seacrowd/sea_datasets/facqa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/facqa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5788 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/facqa/facqa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:50.918806 seacrowd-0.0.7/seacrowd/sea_datasets/facqa/utils/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/facqa/utils/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      815 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/facqa/utils/facqa_utils.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:50.936941 seacrowd-0.0.7/seacrowd/sea_datasets/fakenews_ph/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/fakenews_ph/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4936 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/fakenews_ph/fakenews_ph.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:50.954584 seacrowd-0.0.7/seacrowd/sea_datasets/filipino_gay_lang/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/filipino_gay_lang/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4808 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/filipino_gay_lang/filipino_gay_lang.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:50.974155 seacrowd-0.0.7/seacrowd/sea_datasets/filipino_hatespeech_tiktok/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/filipino_hatespeech_tiktok/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4697 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/filipino_hatespeech_tiktok/filipino_hatespeech_tiktok.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:50.991564 seacrowd-0.0.7/seacrowd/sea_datasets/filipino_slang_norm/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/filipino_slang_norm/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4967 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/filipino_slang_norm/filipino_slang_norm.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:51.008214 seacrowd-0.0.7/seacrowd/sea_datasets/filipino_words_aoa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/filipino_words_aoa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4965 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/filipino_words_aoa/filipino_words_aoa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:51.032177 seacrowd-0.0.7/seacrowd/sea_datasets/filwordnet/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/filwordnet/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4819 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/filwordnet/filwordnet.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:51.057258 seacrowd-0.0.7/seacrowd/sea_datasets/fleurs/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/fleurs/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    13115 2024-04-12 07:50:18.000000 seacrowd-0.0.7/seacrowd/sea_datasets/fleurs/fleurs.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      800 2024-04-12 07:46:55.000000 seacrowd-0.0.7/seacrowd/sea_datasets/fleurs/lang_config.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:51.072550 seacrowd-0.0.7/seacrowd/sea_datasets/flores200/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/flores200/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    13920 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/flores200/flores200.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:51.089601 seacrowd-0.0.7/seacrowd/sea_datasets/fsl_105/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/fsl_105/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6753 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/fsl_105/fsl_105.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:51.107089 seacrowd-0.0.7/seacrowd/sea_datasets/gatitos/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/gatitos/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6624 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/gatitos/gatitos.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:51.124683 seacrowd-0.0.7/seacrowd/sea_datasets/gklmip_newsclass/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/gklmip_newsclass/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6024 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/gklmip_newsclass/gklmip_newsclass.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:51.143279 seacrowd-0.0.7/seacrowd/sea_datasets/gklmip_sentiment/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/gklmip_sentiment/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5007 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/gklmip_sentiment/gklmip_sentiment.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:51.161953 seacrowd-0.0.7/seacrowd/sea_datasets/globalwoz/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/globalwoz/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10031 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/globalwoz/globalwoz.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:51.182351 seacrowd-0.0.7/seacrowd/sea_datasets/glotstorybook/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/glotstorybook/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5878 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/glotstorybook/glotstorybook.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:51.200422 seacrowd-0.0.7/seacrowd/sea_datasets/hoasa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/hoasa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6301 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/hoasa/hoasa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:51.219009 seacrowd-0.0.7/seacrowd/sea_datasets/iapp_squad/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/iapp_squad/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5420 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/iapp_squad/iapp_squad.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:51.236534 seacrowd-0.0.7/seacrowd/sea_datasets/iatf/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/iatf/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5801 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/iatf/iatf.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:51.255149 seacrowd-0.0.7/seacrowd/sea_datasets/icon/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/icon/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8351 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/icon/icon.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:51.274929 seacrowd-0.0.7/seacrowd/sea_datasets/id_abusive/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/id_abusive/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6540 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/id_abusive/id_abusive.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:51.299845 seacrowd-0.0.7/seacrowd/sea_datasets/id_abusive_news_comment/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/id_abusive_news_comment/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4293 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/id_abusive_news_comment/id_abusive_news_comment.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:51.321220 seacrowd-0.0.7/seacrowd/sea_datasets/id_am2ico/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/id_am2ico/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7430 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/id_am2ico/id_am2ico.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:51.344428 seacrowd-0.0.7/seacrowd/sea_datasets/id_clickbait/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/id_clickbait/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5770 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/id_clickbait/id_clickbait.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:51.361111 seacrowd-0.0.7/seacrowd/sea_datasets/id_coreference_resolution/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/id_coreference_resolution/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7576 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/id_coreference_resolution/id_coreference_resolution.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:51.378479 seacrowd-0.0.7/seacrowd/sea_datasets/id_frog_story/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/id_frog_story/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4524 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/id_frog_story/id_frog_story.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:51.396222 seacrowd-0.0.7/seacrowd/sea_datasets/id_google_play_review/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/id_google_play_review/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6144 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/id_google_play_review/id_google_play_review.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:51.414622 seacrowd-0.0.7/seacrowd/sea_datasets/id_hatespeech/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/id_hatespeech/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4450 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/id_hatespeech/id_hatespeech.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:51.438731 seacrowd-0.0.7/seacrowd/sea_datasets/id_hoax_news/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/id_hoax_news/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4555 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/id_hoax_news/id_hoax_news.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:51.456815 seacrowd-0.0.7/seacrowd/sea_datasets/id_hsd_nofaaulia/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/id_hsd_nofaaulia/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7252 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/id_hsd_nofaaulia/id_hsd_nofaaulia.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:51.476053 seacrowd-0.0.7/seacrowd/sea_datasets/id_msvd/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/id_msvd/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5051 2024-04-11 08:39:41.000000 seacrowd-0.0.7/seacrowd/sea_datasets/id_msvd/id_msvd.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:51.494158 seacrowd-0.0.7/seacrowd/sea_datasets/id_multilabel_hs/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/id_multilabel_hs/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6021 2024-04-04 06:00:46.000000 seacrowd-0.0.7/seacrowd/sea_datasets/id_multilabel_hs/id_multilabel_hs.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:51.512002 seacrowd-0.0.7/seacrowd/sea_datasets/id_panl_bppt/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/id_panl_bppt/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5616 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/id_panl_bppt/id_panl_bppt.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:51.530427 seacrowd-0.0.7/seacrowd/sea_datasets/id_qqp/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/id_qqp/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4686 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/id_qqp/id_qqp.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:51.546885 seacrowd-0.0.7/seacrowd/sea_datasets/id_sent_emo_mobile_apps/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/id_sent_emo_mobile_apps/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5395 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/id_sent_emo_mobile_apps/id_sent_emo_mobile_apps.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:51.566011 seacrowd-0.0.7/seacrowd/sea_datasets/id_sentiment_analysis/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/id_sentiment_analysis/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5538 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/id_sentiment_analysis/id_sentiment_analysis.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:51.585798 seacrowd-0.0.7/seacrowd/sea_datasets/id_short_answer_grading/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/id_short_answer_grading/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9107 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/id_short_answer_grading/id_short_answer_grading.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:51.603239 seacrowd-0.0.7/seacrowd/sea_datasets/id_short_answer_grading/utils/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/id_short_answer_grading/utils/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1826 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/id_short_answer_grading/utils/id_short_answer_grading_utils.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:51.621704 seacrowd-0.0.7/seacrowd/sea_datasets/id_stance/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/id_stance/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5114 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/id_stance/id_stance.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:51.644498 seacrowd-0.0.7/seacrowd/sea_datasets/id_sts/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/id_sts/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4308 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/id_sts/id_sts.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:51.667106 seacrowd-0.0.7/seacrowd/sea_datasets/id_vaccines_tweets/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/id_vaccines_tweets/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4329 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/id_vaccines_tweets/id_vaccines_tweets.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:51.682331 seacrowd-0.0.7/seacrowd/sea_datasets/id_wiki_parallel/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/id_wiki_parallel/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6697 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/id_wiki_parallel/id_wiki_parallel.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:51.699547 seacrowd-0.0.7/seacrowd/sea_datasets/id_wsd/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/id_wsd/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6404 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/id_wsd/id_wsd.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:51.717961 seacrowd-0.0.7/seacrowd/sea_datasets/identic/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/identic/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    13357 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/identic/identic.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:51.738515 seacrowd-0.0.7/seacrowd/sea_datasets/identifikasi_bahasa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/identifikasi_bahasa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5177 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/identifikasi_bahasa/identifikasi_bahasa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:51.756099 seacrowd-0.0.7/seacrowd/sea_datasets/idk_mrc/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/idk_mrc/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9530 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/idk_mrc/idk_mrc.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:51.779686 seacrowd-0.0.7/seacrowd/sea_datasets/idn_tagged_corpus_csui/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/idn_tagged_corpus_csui/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6193 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/idn_tagged_corpus_csui/idn_tagged_corpus_csui.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:51.799405 seacrowd-0.0.7/seacrowd/sea_datasets/ijelid/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/ijelid/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5403 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/ijelid/ijelid.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:51.817334 seacrowd-0.0.7/seacrowd/sea_datasets/imdb_jv/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/imdb_jv/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4894 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/imdb_jv/imdb_jv.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:51.835718 seacrowd-0.0.7/seacrowd/sea_datasets/indo4b/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indo4b/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7236 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indo4b/indo4b.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:51.854256 seacrowd-0.0.7/seacrowd/sea_datasets/indo4b_plus/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indo4b_plus/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7417 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indo4b_plus/indo4b_plus.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:51.874281 seacrowd-0.0.7/seacrowd/sea_datasets/indo_general_mt_en_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indo_general_mt_en_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6442 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indo_general_mt_en_id/indo_general_mt_en_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:51.894088 seacrowd-0.0.7/seacrowd/sea_datasets/indo_law/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indo_law/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5445 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indo_law/indo_law.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:51.911689 seacrowd-0.0.7/seacrowd/sea_datasets/indo_puisi/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indo_puisi/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4018 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indo_puisi/indo_puisi.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:51.936436 seacrowd-0.0.7/seacrowd/sea_datasets/indo_religious_mt_en_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indo_religious_mt_en_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8507 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indo_religious_mt_en_id/indo_religious_mt_en_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:51.954483 seacrowd-0.0.7/seacrowd/sea_datasets/indo_story_cloze/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indo_story_cloze/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6563 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indo_story_cloze/indo_story_cloze.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:51.970957 seacrowd-0.0.7/seacrowd/sea_datasets/indocamrest/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indocamrest/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6670 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indocamrest/indocamrest.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:51.986694 seacrowd-0.0.7/seacrowd/sea_datasets/indocollex/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indocollex/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6949 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indocollex/indocollex.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:52.005327 seacrowd-0.0.7/seacrowd/sea_datasets/indocoref/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indocoref/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    11610 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indocoref/indocoref.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:52.046602 seacrowd-0.0.7/seacrowd/sea_datasets/indocoref/utils/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indocoref/utils/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9072 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indocoref/utils/feature_utils.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     2091 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indocoref/utils/file_utils.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4307 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indocoref/utils/text_preprocess.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:52.065398 seacrowd-0.0.7/seacrowd/sea_datasets/indolem_ner_ugm/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indolem_ner_ugm/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6402 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indolem_ner_ugm/indolem_ner_ugm.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:52.085895 seacrowd-0.0.7/seacrowd/sea_datasets/indolem_nerui/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indolem_nerui/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8192 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indolem_nerui/indolem_nerui.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:52.104362 seacrowd-0.0.7/seacrowd/sea_datasets/indolem_ntp/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indolem_ntp/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5885 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indolem_ntp/indolem_ntp.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:52.121571 seacrowd-0.0.7/seacrowd/sea_datasets/indolem_sentiment/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indolem_sentiment/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    12679 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indolem_sentiment/indolem_sentiment.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:52.141845 seacrowd-0.0.7/seacrowd/sea_datasets/indolem_tweet_ordering/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indolem_tweet_ordering/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    12454 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indolem_tweet_ordering/indolem_tweet_ordering.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:52.160828 seacrowd-0.0.7/seacrowd/sea_datasets/indolem_ud_id_gsd/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indolem_ud_id_gsd/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8462 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indolem_ud_id_gsd/indolem_ud_id_gsd.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:52.180661 seacrowd-0.0.7/seacrowd/sea_datasets/indolem_ud_id_pud/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indolem_ud_id_pud/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8825 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indolem_ud_id_pud/indolem_ud_id_pud.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:52.199089 seacrowd-0.0.7/seacrowd/sea_datasets/indoler/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indoler/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9100 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indoler/indoler.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:52.218866 seacrowd-0.0.7/seacrowd/sea_datasets/indommlu/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indommlu/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10934 2024-04-11 08:39:41.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indommlu/indommlu.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:52.236608 seacrowd-0.0.7/seacrowd/sea_datasets/indoner_tourism/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indoner_tourism/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8394 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indoner_tourism/indoner_tourism.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:52.255081 seacrowd-0.0.7/seacrowd/sea_datasets/indonesia_chinese_mtrobusteval/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indonesia_chinese_mtrobusteval/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5250 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indonesia_chinese_mtrobusteval/indonesia_chinese_mtrobusteval.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:52.270427 seacrowd-0.0.7/seacrowd/sea_datasets/indonesian_madurese_bible_translation/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indonesian_madurese_bible_translation/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7932 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indonesian_madurese_bible_translation/indonesian_madurese_bible_translation.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:52.286471 seacrowd-0.0.7/seacrowd/sea_datasets/indonesian_news_dataset/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indonesian_news_dataset/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4581 2024-04-11 08:39:41.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indonesian_news_dataset/indonesian_news_dataset.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:52.308839 seacrowd-0.0.7/seacrowd/sea_datasets/indonesiannmt/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indonesiannmt/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9148 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indonesiannmt/indonesiannmt.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:52.335582 seacrowd-0.0.7/seacrowd/sea_datasets/indonglish/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indonglish/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8339 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indonglish/indonglish.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:52.354767 seacrowd-0.0.7/seacrowd/sea_datasets/indonli/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indonli/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8050 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indonli/indonli.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:52.372179 seacrowd-0.0.7/seacrowd/sea_datasets/indonlu_nergrit/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indonlu_nergrit/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5677 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indonlu_nergrit/indonlu_nergrit.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:52.391134 seacrowd-0.0.7/seacrowd/sea_datasets/indoqa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indoqa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5422 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indoqa/indoqa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:52.409685 seacrowd-0.0.7/seacrowd/sea_datasets/indosmd/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indosmd/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    13550 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indosmd/indosmd.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:52.431681 seacrowd-0.0.7/seacrowd/sea_datasets/indosum/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indosum/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6872 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indosum/indosum.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:52.449025 seacrowd-0.0.7/seacrowd/sea_datasets/indotacos/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indotacos/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5477 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indotacos/indotacos.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:52.466277 seacrowd-0.0.7/seacrowd/sea_datasets/indowiki/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indowiki/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7684 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indowiki/indowiki.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:52.488860 seacrowd-0.0.7/seacrowd/sea_datasets/indqner/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        1 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indqner/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6614 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indqner/indqner.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:52.511755 seacrowd-0.0.7/seacrowd/sea_datasets/indspeech_digit_cdsr/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indspeech_digit_cdsr/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9856 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indspeech_digit_cdsr/indspeech_digit_cdsr.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:52.530965 seacrowd-0.0.7/seacrowd/sea_datasets/indspeech_news_ethnicsr/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indspeech_news_ethnicsr/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8440 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indspeech_news_ethnicsr/indspeech_news_ethnicsr.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:52.548919 seacrowd-0.0.7/seacrowd/sea_datasets/indspeech_news_lvcsr/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indspeech_news_lvcsr/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9432 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indspeech_news_lvcsr/indspeech_news_lvcsr.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:52.566630 seacrowd-0.0.7/seacrowd/sea_datasets/indspeech_news_tts/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indspeech_news_tts/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8857 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indspeech_news_tts/indspeech_news_tts.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:52.584370 seacrowd-0.0.7/seacrowd/sea_datasets/indspeech_newstra_ethnicsr/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indspeech_newstra_ethnicsr/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    11615 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indspeech_newstra_ethnicsr/indspeech_newstra_ethnicsr.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:52.602897 seacrowd-0.0.7/seacrowd/sea_datasets/indspeech_teldialog_lvcsr/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indspeech_teldialog_lvcsr/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9932 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indspeech_teldialog_lvcsr/indspeech_teldialog_lvcsr.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:52.628613 seacrowd-0.0.7/seacrowd/sea_datasets/indspeech_teldialog_svcsr/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indspeech_teldialog_svcsr/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9818 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/indspeech_teldialog_svcsr/indspeech_teldialog_svcsr.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:52.646739 seacrowd-0.0.7/seacrowd/sea_datasets/inset_lexicon/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/inset_lexicon/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4829 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/inset_lexicon/inset_lexicon.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:52.664616 seacrowd-0.0.7/seacrowd/sea_datasets/jadi_ide/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/jadi_ide/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4404 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/jadi_ide/jadi_ide.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:52.682367 seacrowd-0.0.7/seacrowd/sea_datasets/jv_id_asr/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/jv_id_asr/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6236 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/jv_id_asr/jv_id_asr.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:52.702490 seacrowd-0.0.7/seacrowd/sea_datasets/jv_id_tts/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/jv_id_tts/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7628 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/jv_id_tts/jv_id_tts.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:52.721430 seacrowd-0.0.7/seacrowd/sea_datasets/kamus_alay/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/kamus_alay/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5286 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/kamus_alay/kamus_alay.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:52.738881 seacrowd-0.0.7/seacrowd/sea_datasets/karonese_sentiment/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/karonese_sentiment/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4533 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/karonese_sentiment/karonese_sentiment.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:52.766751 seacrowd-0.0.7/seacrowd/sea_datasets/kawat/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/kawat/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5933 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/kawat/kawat.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:52.784527 seacrowd-0.0.7/seacrowd/sea_datasets/kde4/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/kde4/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    14408 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/kde4/kde4.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:52.802329 seacrowd-0.0.7/seacrowd/sea_datasets/keps/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/keps/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5066 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/keps/keps.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:52.826717 seacrowd-0.0.7/seacrowd/sea_datasets/kheng_info/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/kheng_info/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3687 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/kheng_info/kheng_info.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:52.845449 seacrowd-0.0.7/seacrowd/sea_datasets/khmer_alt_pos/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/khmer_alt_pos/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7442 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/khmer_alt_pos/khmer_alt_pos.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:52.875411 seacrowd-0.0.7/seacrowd/sea_datasets/khpos/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/khpos/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8756 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/khpos/khpos.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:52.912846 seacrowd-0.0.7/seacrowd/sea_datasets/kopi_cc/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/kopi_cc/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10035 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/kopi_cc/kopi_cc.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:52.936560 seacrowd-0.0.7/seacrowd/sea_datasets/kopi_cc_news/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/kopi_cc_news/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5088 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/kopi_cc_news/kopi_cc_news.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:52.953380 seacrowd-0.0.7/seacrowd/sea_datasets/kopi_nllb/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/kopi_nllb/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5956 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/kopi_nllb/kopi_nllb.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:52.970789 seacrowd-0.0.7/seacrowd/sea_datasets/korpus_nusantara/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/korpus_nusantara/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8476 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/korpus_nusantara/korpus_nusantara.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:52.990947 seacrowd-0.0.7/seacrowd/sea_datasets/lazada_review_filipino/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/lazada_review_filipino/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4913 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/lazada_review_filipino/lazada_review_filipino.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:53.013474 seacrowd-0.0.7/seacrowd/sea_datasets/librivox_indonesia/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/librivox_indonesia/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8736 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/librivox_indonesia/librivox_indonesia.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:53.033867 seacrowd-0.0.7/seacrowd/sea_datasets/limesoda/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/limesoda/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6775 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/limesoda/limesoda.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:53.054534 seacrowd-0.0.7/seacrowd/sea_datasets/liputan6/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/liputan6/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7512 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/liputan6/liputan6.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:53.081307 seacrowd-0.0.7/seacrowd/sea_datasets/local_id_abusive/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/local_id_abusive/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7530 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/local_id_abusive/local_id_abusive.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:53.105780 seacrowd-0.0.7/seacrowd/sea_datasets/lr_sum/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/lr_sum/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6160 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/lr_sum/lr_sum.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:53.145825 seacrowd-0.0.7/seacrowd/sea_datasets/m3exam/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/m3exam/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    14637 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/m3exam/m3exam.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:53.184143 seacrowd-0.0.7/seacrowd/sea_datasets/mabl/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/mabl/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8609 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/mabl/mabl.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:53.207697 seacrowd-0.0.7/seacrowd/sea_datasets/malaysia_tweets/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/malaysia_tweets/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6432 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/malaysia_tweets/malaysia_tweets.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:53.239789 seacrowd-0.0.7/seacrowd/sea_datasets/malindo_morph/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/malindo_morph/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4617 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/malindo_morph/malindo_morph.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:53.273342 seacrowd-0.0.7/seacrowd/sea_datasets/malindo_parallel/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/malindo_parallel/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6494 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/malindo_parallel/malindo_parallel.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:53.304225 seacrowd-0.0.7/seacrowd/sea_datasets/massive/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/massive/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    18420 2024-04-04 06:00:48.000000 seacrowd-0.0.7/seacrowd/sea_datasets/massive/massive.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:53.325557 seacrowd-0.0.7/seacrowd/sea_datasets/mc4_indo/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/mc4_indo/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5510 2024-04-11 08:39:41.000000 seacrowd-0.0.7/seacrowd/sea_datasets/mc4_indo/mc4_indo.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:53.349086 seacrowd-0.0.7/seacrowd/sea_datasets/melayu_brunei/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/melayu_brunei/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10682 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/melayu_brunei/melayu_brunei.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:53.372804 seacrowd-0.0.7/seacrowd/sea_datasets/melayu_sabah/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/melayu_sabah/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5561 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/melayu_sabah/melayu_sabah.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:53.390445 seacrowd-0.0.7/seacrowd/sea_datasets/melayu_sarawak/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/melayu_sarawak/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6559 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/melayu_sarawak/melayu_sarawak.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:53.421123 seacrowd-0.0.7/seacrowd/sea_datasets/melayu_standard_lisan/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/melayu_standard_lisan/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7594 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/melayu_standard_lisan/melayu_standard_lisan.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:53.444988 seacrowd-0.0.7/seacrowd/sea_datasets/memolon/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/memolon/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5589 2024-04-11 08:39:41.000000 seacrowd-0.0.7/seacrowd/sea_datasets/memolon/memolon.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:53.469685 seacrowd-0.0.7/seacrowd/sea_datasets/minangnlp_mt/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/minangnlp_mt/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6874 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/minangnlp_mt/minangnlp_mt.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:53.490651 seacrowd-0.0.7/seacrowd/sea_datasets/miracl/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/miracl/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    13119 2024-04-11 08:39:41.000000 seacrowd-0.0.7/seacrowd/sea_datasets/miracl/miracl.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:53.511348 seacrowd-0.0.7/seacrowd/sea_datasets/mkqa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/mkqa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8345 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/mkqa/mkqa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:53.562178 seacrowd-0.0.7/seacrowd/sea_datasets/mlqa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        1 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/mlqa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9825 2024-04-11 08:39:41.000000 seacrowd-0.0.7/seacrowd/sea_datasets/mlqa/mlqa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:53.597807 seacrowd-0.0.7/seacrowd/sea_datasets/mozilla_pontoon/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/mozilla_pontoon/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6211 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/mozilla_pontoon/mozilla_pontoon.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:53.624264 seacrowd-0.0.7/seacrowd/sea_datasets/mswc/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/mswc/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8048 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/mswc/mswc.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:53.664264 seacrowd-0.0.7/seacrowd/sea_datasets/mtop_intent_classification/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/mtop_intent_classification/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     2654 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/mtop_intent_classification/labels.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5662 2024-04-11 08:39:41.000000 seacrowd-0.0.7/seacrowd/sea_datasets/mtop_intent_classification/mtop_intent_classification.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:53.685180 seacrowd-0.0.7/seacrowd/sea_datasets/multilexnorm/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/multilexnorm/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6223 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/multilexnorm/multilexnorm.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:53.703298 seacrowd-0.0.7/seacrowd/sea_datasets/my_paraphrase/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/my_paraphrase/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8124 2024-04-11 08:39:41.000000 seacrowd-0.0.7/seacrowd/sea_datasets/my_paraphrase/my_paraphrase.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:53.719945 seacrowd-0.0.7/seacrowd/sea_datasets/myanmar_rakhine_parallel/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/myanmar_rakhine_parallel/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7223 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/myanmar_rakhine_parallel/myanmar_rakhine_parallel.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:53.738599 seacrowd-0.0.7/seacrowd/sea_datasets/mypos/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/mypos/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5116 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/mypos/mypos.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:53.767549 seacrowd-0.0.7/seacrowd/sea_datasets/mysentence/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/mysentence/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7612 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/mysentence/mysentence.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:53.783631 seacrowd-0.0.7/seacrowd/sea_datasets/myxnli/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/myxnli/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5096 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/myxnli/myxnli.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:53.801382 seacrowd-0.0.7/seacrowd/sea_datasets/nergrit/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/nergrit/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6322 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/nergrit/nergrit.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:53.834437 seacrowd-0.0.7/seacrowd/sea_datasets/nerp/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/nerp/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4852 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/nerp/nerp.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:53.860091 seacrowd-0.0.7/seacrowd/sea_datasets/netifier/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/netifier/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4838 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/netifier/netifier.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:53.879059 seacrowd-0.0.7/seacrowd/sea_datasets/news_en_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/news_en_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5003 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/news_en_id/news_en_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:53.897631 seacrowd-0.0.7/seacrowd/sea_datasets/newsph/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/newsph/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3810 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/newsph/newsph.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:53.919094 seacrowd-0.0.7/seacrowd/sea_datasets/nllb_seed/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/nllb_seed/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    15208 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/nllb_seed/nllb_seed.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:53.952178 seacrowd-0.0.7/seacrowd/sea_datasets/ntrex_128/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/ntrex_128/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10971 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/ntrex_128/ntrex_128.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:53.981422 seacrowd-0.0.7/seacrowd/sea_datasets/nusaparagraph_emot/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/nusaparagraph_emot/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8785 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/nusaparagraph_emot/nusaparagraph_emot.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:54.009690 seacrowd-0.0.7/seacrowd/sea_datasets/nusaparagraph_rhetoric/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/nusaparagraph_rhetoric/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8792 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/nusaparagraph_rhetoric/nusaparagraph_rhetoric.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:54.043187 seacrowd-0.0.7/seacrowd/sea_datasets/nusaparagraph_topic/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/nusaparagraph_topic/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8845 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/nusaparagraph_topic/nusaparagraph_topic.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:54.069766 seacrowd-0.0.7/seacrowd/sea_datasets/nusatranslation_emot/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/nusatranslation_emot/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8233 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/nusatranslation_emot/nusatranslation_emot.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:54.095998 seacrowd-0.0.7/seacrowd/sea_datasets/nusatranslation_mt/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/nusatranslation_mt/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9156 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/nusatranslation_mt/nusatranslation_mt.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:54.114422 seacrowd-0.0.7/seacrowd/sea_datasets/nusatranslation_senti/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/nusatranslation_senti/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8285 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/nusatranslation_senti/nusatranslation_senti.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:54.142522 seacrowd-0.0.7/seacrowd/sea_datasets/nusax_mt/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/nusax_mt/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7578 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/nusax_mt/nusax_mt.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:54.174433 seacrowd-0.0.7/seacrowd/sea_datasets/nusax_senti/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/nusax_senti/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7250 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/nusax_senti/nusax_senti.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:54.193338 seacrowd-0.0.7/seacrowd/sea_datasets/oil/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/oil/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5477 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/oil/oil.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:54.220823 seacrowd-0.0.7/seacrowd/sea_datasets/ojw/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/ojw/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5110 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/ojw/ojw.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:54.247135 seacrowd-0.0.7/seacrowd/sea_datasets/openlid/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/openlid/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7915 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/openlid/openlid.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:54.265611 seacrowd-0.0.7/seacrowd/sea_datasets/openslr/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/openslr/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10343 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/openslr/openslr.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:54.285833 seacrowd-0.0.7/seacrowd/sea_datasets/orchid_pos/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/orchid_pos/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9625 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/orchid_pos/orchid_pos.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:54.306414 seacrowd-0.0.7/seacrowd/sea_datasets/oscar_2201/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/oscar_2201/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    16270 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/oscar_2201/oscar_2201.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:54.328131 seacrowd-0.0.7/seacrowd/sea_datasets/palito/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/palito/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5930 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/palito/palito.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:54.346236 seacrowd-0.0.7/seacrowd/sea_datasets/paracotta_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/paracotta_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4768 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/paracotta_id/paracotta_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:54.363246 seacrowd-0.0.7/seacrowd/sea_datasets/parallel_id_nyo/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/parallel_id_nyo/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5471 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/parallel_id_nyo/parallel_id_nyo.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:54.382563 seacrowd-0.0.7/seacrowd/sea_datasets/parallel_su_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/parallel_su_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4782 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/parallel_su_id/parallel_su_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:54.399908 seacrowd-0.0.7/seacrowd/sea_datasets/ph_fake_news_corpus/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/ph_fake_news_corpus/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4339 2024-04-11 08:39:41.000000 seacrowd-0.0.7/seacrowd/sea_datasets/ph_fake_news_corpus/ph_fake_news_corpus.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:54.423696 seacrowd-0.0.7/seacrowd/sea_datasets/pho_ner_covid/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/pho_ner_covid/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6866 2024-04-04 06:00:49.000000 seacrowd-0.0.7/seacrowd/sea_datasets/pho_ner_covid/pho_ner_covid.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:54.466461 seacrowd-0.0.7/seacrowd/sea_datasets/phomt/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/phomt/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5141 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/phomt/phomt.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:54.483347 seacrowd-0.0.7/seacrowd/sea_datasets/phost/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/phost/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9498 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/phost/phost.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:54.499168 seacrowd-0.0.7/seacrowd/sea_datasets/posp/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/posp/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5990 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/posp/posp.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:54.532146 seacrowd-0.0.7/seacrowd/sea_datasets/postag_su/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/postag_su/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8033 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/postag_su/postag_su.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:54.553560 seacrowd-0.0.7/seacrowd/sea_datasets/prdect_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/prdect_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7572 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/prdect_id/prdect_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:54.573285 seacrowd-0.0.7/seacrowd/sea_datasets/qasina/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/qasina/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6424 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/qasina/qasina.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:54.591740 seacrowd-0.0.7/seacrowd/sea_datasets/roots_vi_ted/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/roots_vi_ted/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5065 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/roots_vi_ted/roots_vi_ted.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:54.613725 seacrowd-0.0.7/seacrowd/sea_datasets/sampiran/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/sampiran/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5024 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/sampiran/sampiran.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:54.634255 seacrowd-0.0.7/seacrowd/sea_datasets/sap_wat/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/sap_wat/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7077 2024-04-11 08:39:41.000000 seacrowd-0.0.7/seacrowd/sea_datasets/sap_wat/sap_wat.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:54.662865 seacrowd-0.0.7/seacrowd/sea_datasets/sarawak_malay/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/sarawak_malay/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7381 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/sarawak_malay/sarawak_malay.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:54.686669 seacrowd-0.0.7/seacrowd/sea_datasets/scb_mt_en_th/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/scb_mt_en_th/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7071 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/scb_mt_en_th/scb_mt_en_th.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:54.715669 seacrowd-0.0.7/seacrowd/sea_datasets/sea_bench/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/sea_bench/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7206 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/sea_bench/sea_bench.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:54.746353 seacrowd-0.0.7/seacrowd/sea_datasets/sea_madlad/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/sea_madlad/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10051 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/sea_madlad/sea_madlad.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:54.781338 seacrowd-0.0.7/seacrowd/sea_datasets/sea_wiki/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/sea_wiki/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1844 2024-04-12 07:50:53.000000 seacrowd-0.0.7/seacrowd/sea_datasets/sea_wiki/lang_config.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9272 2024-04-12 07:52:13.000000 seacrowd-0.0.7/seacrowd/sea_datasets/sea_wiki/sea_wiki.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:54.798986 seacrowd-0.0.7/seacrowd/sea_datasets/seaeval/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/seaeval/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9350 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/seaeval/seaeval.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:54.822638 seacrowd-0.0.7/seacrowd/sea_datasets/seahorse/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/seahorse/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6884 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/seahorse/seahorse.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:54.851938 seacrowd-0.0.7/seacrowd/sea_datasets/sentiment_nathasa_review/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/sentiment_nathasa_review/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6002 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/sentiment_nathasa_review/sentiment_nathasa_review.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:54.872635 seacrowd-0.0.7/seacrowd/sea_datasets/shopee_reviews_tagalog/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/shopee_reviews_tagalog/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4597 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/shopee_reviews_tagalog/shopee_reviews_tagalog.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:54.893543 seacrowd-0.0.7/seacrowd/sea_datasets/singgalang/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/singgalang/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5430 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/singgalang/singgalang.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:54.935872 seacrowd-0.0.7/seacrowd/sea_datasets/smsa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/smsa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5575 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/smsa/smsa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:54.955777 seacrowd-0.0.7/seacrowd/sea_datasets/snli_indo/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/snli_indo/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6244 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/snli_indo/snli_indo.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:54.977931 seacrowd-0.0.7/seacrowd/sea_datasets/spamid_pair/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/spamid_pair/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5524 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/spamid_pair/spamid_pair.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:54.996973 seacrowd-0.0.7/seacrowd/sea_datasets/squad_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/squad_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5315 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/squad_id/squad_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:55.027928 seacrowd-0.0.7/seacrowd/sea_datasets/stb_ext/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/stb_ext/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9273 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/stb_ext/stb_ext.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:55.046142 seacrowd-0.0.7/seacrowd/sea_datasets/stif_indonesia/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/stif_indonesia/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5135 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/stif_indonesia/stif_indonesia.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:55.065302 seacrowd-0.0.7/seacrowd/sea_datasets/struct_amb_ind/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/struct_amb_ind/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7724 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/struct_amb_ind/struct_amb_ind.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:55.082462 seacrowd-0.0.7/seacrowd/sea_datasets/su_emot/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/su_emot/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4567 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/su_emot/su_emot.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:55.100371 seacrowd-0.0.7/seacrowd/sea_datasets/su_id_asr/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/su_id_asr/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5601 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/su_id_asr/su_id_asr.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:55.117761 seacrowd-0.0.7/seacrowd/sea_datasets/su_id_tts/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/su_id_tts/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7636 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/su_id_tts/su_id_tts.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:55.142170 seacrowd-0.0.7/seacrowd/sea_datasets/talpco/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/talpco/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6870 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/talpco/talpco.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:55.167865 seacrowd-0.0.7/seacrowd/sea_datasets/tatabahasa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/tatabahasa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5411 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/tatabahasa/tatabahasa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:55.186079 seacrowd-0.0.7/seacrowd/sea_datasets/tatoeba/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/tatoeba/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7636 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/tatoeba/tatoeba.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:55.204479 seacrowd-0.0.7/seacrowd/sea_datasets/tcope/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/tcope/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6693 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/tcope/tcope.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:55.231257 seacrowd-0.0.7/seacrowd/sea_datasets/ted_en_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/ted_en_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7105 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/ted_en_id/ted_en_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:55.266511 seacrowd-0.0.7/seacrowd/sea_datasets/term_a/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/term_a/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5358 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/term_a/term_a.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:55.285191 seacrowd-0.0.7/seacrowd/sea_datasets/tgl_profanity/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/tgl_profanity/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4351 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/tgl_profanity/tgl_profanity.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:55.311239 seacrowd-0.0.7/seacrowd/sea_datasets/tha_lao_embassy_parcor/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/tha_lao_embassy_parcor/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4436 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/tha_lao_embassy_parcor/tha_lao_embassy_parcor.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:55.339482 seacrowd-0.0.7/seacrowd/sea_datasets/thai_alpaca/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/thai_alpaca/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3943 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/thai_alpaca/thai_alpaca.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:55.360484 seacrowd-0.0.7/seacrowd/sea_datasets/thai_constitution/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/thai_constitution/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10954 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/thai_constitution/thai_constitution.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:55.377994 seacrowd-0.0.7/seacrowd/sea_datasets/thai_databricks_dolly/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/thai_databricks_dolly/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4388 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/thai_databricks_dolly/thai_databricks_dolly.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:55.397239 seacrowd-0.0.7/seacrowd/sea_datasets/thai_depression/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/thai_depression/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5739 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/thai_depression/thai_depression.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:55.441330 seacrowd-0.0.7/seacrowd/sea_datasets/thai_gpteacher/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/thai_gpteacher/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3960 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/thai_gpteacher/thai_gpteacher.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:55.459253 seacrowd-0.0.7/seacrowd/sea_datasets/thai_hh_rlhf/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/thai_hh_rlhf/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5077 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/thai_hh_rlhf/thai_hh_rlhf.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:55.478815 seacrowd-0.0.7/seacrowd/sea_datasets/thai_sum/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/thai_sum/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5683 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/thai_sum/thai_sum.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:55.508410 seacrowd-0.0.7/seacrowd/sea_datasets/thai_toxicity_tweet/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/thai_toxicity_tweet/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4555 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/thai_toxicity_tweet/thai_toxicity_tweet.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:55.528756 seacrowd-0.0.7/seacrowd/sea_datasets/tico_19/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/tico_19/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    12192 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/tico_19/tico_19.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:55.551835 seacrowd-0.0.7/seacrowd/sea_datasets/titml_idn/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/titml_idn/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5900 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/titml_idn/titml_idn.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:55.571701 seacrowd-0.0.7/seacrowd/sea_datasets/tlunified_ner/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.7/seacrowd/sea_datasets/tlunified_ner/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5800 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/tlunified_ner/tlunified_ner.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:55.590230 seacrowd-0.0.7/seacrowd/sea_datasets/toxicity_200/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/toxicity_200/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5975 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/toxicity_200/toxicity_200.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:55.610142 seacrowd-0.0.7/seacrowd/sea_datasets/tydiqa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/tydiqa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    23881 2024-04-11 08:39:41.000000 seacrowd-0.0.7/seacrowd/sea_datasets/tydiqa/tydiqa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:55.652463 seacrowd-0.0.7/seacrowd/sea_datasets/typhoon_yolanda_tweets/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        1 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/typhoon_yolanda_tweets/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5165 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/typhoon_yolanda_tweets/typhoon_yolanda_tweets.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:55.673501 seacrowd-0.0.7/seacrowd/sea_datasets/ucla_phonetic/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/ucla_phonetic/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6531 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/ucla_phonetic/ucla_phonetic.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:55.692723 seacrowd-0.0.7/seacrowd/sea_datasets/ud_id_csui/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/ud_id_csui/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9185 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/ud_id_csui/ud_id_csui.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:55.715296 seacrowd-0.0.7/seacrowd/sea_datasets/ud_jv_csui/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/ud_jv_csui/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10052 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/ud_jv_csui/ud_jv_csui.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:55.744427 seacrowd-0.0.7/seacrowd/sea_datasets/udhr/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/udhr/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6030 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/udhr/udhr.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:55.766323 seacrowd-0.0.7/seacrowd/sea_datasets/udhr_lid/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/udhr_lid/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5190 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/udhr_lid/udhr_lid.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:55.784732 seacrowd-0.0.7/seacrowd/sea_datasets/uit_vicov19qa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/uit_vicov19qa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7244 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/uit_vicov19qa/uit_vicov19qa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:55.802572 seacrowd-0.0.7/seacrowd/sea_datasets/uit_victsd/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/uit_victsd/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5311 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/uit_victsd/uit_victsd.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:55.841362 seacrowd-0.0.7/seacrowd/sea_datasets/uit_vihsd/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/uit_vihsd/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5721 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/uit_vihsd/uit_vihsd.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:55.860585 seacrowd-0.0.7/seacrowd/sea_datasets/uit_viic/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/uit_viic/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6572 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/uit_viic/uit_viic.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:55.884987 seacrowd-0.0.7/seacrowd/sea_datasets/uit_viocd/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/uit_viocd/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4819 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/uit_viocd/uit_viocd.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:55.913365 seacrowd-0.0.7/seacrowd/sea_datasets/uit_vion/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/uit_vion/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5939 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/uit_vion/uit_vion.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:55.951865 seacrowd-0.0.7/seacrowd/sea_datasets/uit_visd4sa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/uit_visd4sa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7034 2024-04-11 08:39:41.000000 seacrowd-0.0.7/seacrowd/sea_datasets/uit_visd4sa/uit_visd4sa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:55.970684 seacrowd-0.0.7/seacrowd/sea_datasets/uit_vsfc/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/uit_vsfc/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8715 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/uit_vsfc/uit_vsfc.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:55.987447 seacrowd-0.0.7/seacrowd/sea_datasets/uit_vsmec/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/uit_vsmec/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4802 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/uit_vsmec/uit_vsmec.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:56.013305 seacrowd-0.0.7/seacrowd/sea_datasets/unimorph/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/unimorph/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    15492 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/unimorph/unimorph.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:56.053969 seacrowd-0.0.7/seacrowd/sea_datasets/unimorph_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/unimorph_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7445 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/unimorph_id/unimorph_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:56.077862 seacrowd-0.0.7/seacrowd/sea_datasets/vi_pubmed/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/vi_pubmed/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    15136 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/vi_pubmed/vi_pubmed.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:56.096478 seacrowd-0.0.7/seacrowd/sea_datasets/vihealthqa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/vihealthqa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5587 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/vihealthqa/vihealthqa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:56.123643 seacrowd-0.0.7/seacrowd/sea_datasets/visobert/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/visobert/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6265 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/visobert/visobert.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:56.139355 seacrowd-0.0.7/seacrowd/sea_datasets/vispamreviews/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/vispamreviews/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7245 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/vispamreviews/vispamreviews.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:56.162921 seacrowd-0.0.7/seacrowd/sea_datasets/vistec_tp_th_21/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/vistec_tp_th_21/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6739 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/vistec_tp_th_21/vistec_tp_th_21.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:56.182101 seacrowd-0.0.7/seacrowd/sea_datasets/vitext2sql/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/vitext2sql/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6893 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/vitext2sql/vitext2sql.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:56.209326 seacrowd-0.0.7/seacrowd/sea_datasets/vivos/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/vivos/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7832 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/vivos/vivos.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:56.236140 seacrowd-0.0.7/seacrowd/sea_datasets/vivqa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/vivqa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9080 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/vivqa/vivqa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:56.254902 seacrowd-0.0.7/seacrowd/sea_datasets/vlsp2016_ner/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/vlsp2016_ner/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5857 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/vlsp2016_ner/vlsp2016_ner.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:56.273465 seacrowd-0.0.7/seacrowd/sea_datasets/vlsp2016_sa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/vlsp2016_sa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7134 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/vlsp2016_sa/vlsp2016_sa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:56.316379 seacrowd-0.0.7/seacrowd/sea_datasets/vndt/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/vndt/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     2232 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/vndt/utils.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7852 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/vndt/vndt.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:56.343952 seacrowd-0.0.7/seacrowd/sea_datasets/voxlingua/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/voxlingua/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7980 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/voxlingua/voxlingua.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:56.365208 seacrowd-0.0.7/seacrowd/sea_datasets/weathub/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/weathub/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7521 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/weathub/weathub.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:56.383498 seacrowd-0.0.7/seacrowd/sea_datasets/wikiann/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/wikiann/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8643 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/wikiann/wikiann.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:56.405413 seacrowd-0.0.7/seacrowd/sea_datasets/wikilingua/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/wikilingua/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4984 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/wikilingua/wikilingua.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:56.435191 seacrowd-0.0.7/seacrowd/sea_datasets/wikimatrix/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/wikimatrix/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8585 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/wikimatrix/wikimatrix.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:56.459698 seacrowd-0.0.7/seacrowd/sea_datasets/wikitext_tl_39/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/wikitext_tl_39/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3663 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/wikitext_tl_39/wikitext_tl_39.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:56.474955 seacrowd-0.0.7/seacrowd/sea_datasets/wili_2018/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/wili_2018/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6699 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/wili_2018/wili_2018.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:56.492182 seacrowd-0.0.7/seacrowd/sea_datasets/wisesight_thai_sentiment/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/wisesight_thai_sentiment/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7027 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/wisesight_thai_sentiment/wisesight_thai_sentiment.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:56.510595 seacrowd-0.0.7/seacrowd/sea_datasets/wit/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/wit/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    12057 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/wit/wit.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:56.542319 seacrowd-0.0.7/seacrowd/sea_datasets/wongnai_reviews/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/wongnai_reviews/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4106 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/wongnai_reviews/wongnai_reviews.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:56.571360 seacrowd-0.0.7/seacrowd/sea_datasets/wrete/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/wrete/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6113 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/wrete/wrete.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:56.598157 seacrowd-0.0.7/seacrowd/sea_datasets/x_fact/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/x_fact/__init__.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:56.622400 seacrowd-0.0.7/seacrowd/sea_datasets/x_fact/utils/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/x_fact/utils/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      473 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/x_fact/utils/x_fact_utils.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5900 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/x_fact/x_fact.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:56.644353 seacrowd-0.0.7/seacrowd/sea_datasets/xcopa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/xcopa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7024 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/xcopa/xcopa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:56.666822 seacrowd-0.0.7/seacrowd/sea_datasets/xl_jailbreak/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/xl_jailbreak/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6317 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/xl_jailbreak/xl_jailbreak.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:56.684629 seacrowd-0.0.7/seacrowd/sea_datasets/xl_sum/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/xl_sum/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6903 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/xl_sum/xl_sum.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:56.716884 seacrowd-0.0.7/seacrowd/sea_datasets/xm3600/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/xm3600/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8233 2024-04-11 08:39:41.000000 seacrowd-0.0.7/seacrowd/sea_datasets/xm3600/xm3600.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:56.734171 seacrowd-0.0.7/seacrowd/sea_datasets/xnli/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/xnli/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8333 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/xnli/xnli.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:56.760838 seacrowd-0.0.7/seacrowd/sea_datasets/xpersona_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/xpersona_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6550 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/xpersona_id/xpersona_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:56.791565 seacrowd-0.0.7/seacrowd/sea_datasets/xquad/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/xquad/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4819 2024-04-04 06:00:51.000000 seacrowd-0.0.7/seacrowd/sea_datasets/xquad/xquad.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:56.817274 seacrowd-0.0.7/seacrowd/sea_datasets/xsid/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:52.000000 seacrowd-0.0.7/seacrowd/sea_datasets/xsid/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9510 2024-04-04 06:00:52.000000 seacrowd-0.0.7/seacrowd/sea_datasets/xsid/xsid.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:56.837890 seacrowd-0.0.7/seacrowd/sea_datasets/xstorycloze/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:52.000000 seacrowd-0.0.7/seacrowd/sea_datasets/xstorycloze/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6794 2024-04-04 06:00:52.000000 seacrowd-0.0.7/seacrowd/sea_datasets/xstorycloze/xstorycloze.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:56.855592 seacrowd-0.0.7/seacrowd/sea_datasets/yunshan_cup_2020/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:52.000000 seacrowd-0.0.7/seacrowd/sea_datasets/yunshan_cup_2020/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5828 2024-04-04 06:00:52.000000 seacrowd-0.0.7/seacrowd/sea_datasets/yunshan_cup_2020/yunshan_cup_2020.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:56.906286 seacrowd-0.0.7/seacrowd/utils/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:52.000000 seacrowd-0.0.7/seacrowd/utils/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5493 2024-04-04 06:00:52.000000 seacrowd-0.0.7/seacrowd/utils/common_parser.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      284 2024-04-04 06:00:52.000000 seacrowd-0.0.7/seacrowd/utils/configs.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    12786 2024-04-04 06:00:52.000000 seacrowd-0.0.7/seacrowd/utils/constants.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:57.161607 seacrowd-0.0.7/seacrowd/utils/schemas/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1485 2024-04-04 06:00:52.000000 seacrowd-0.0.7/seacrowd/utils/schemas/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      506 2024-04-04 06:00:52.000000 seacrowd-0.0.7/seacrowd/utils/schemas/image_text.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1101 2024-04-04 06:00:52.000000 seacrowd-0.0.7/seacrowd/utils/schemas/imqa.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     2283 2024-04-04 06:00:52.000000 seacrowd-0.0.7/seacrowd/utils/schemas/kb.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      626 2024-04-04 06:00:52.000000 seacrowd-0.0.7/seacrowd/utils/schemas/pairs.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      371 2024-04-04 06:00:52.000000 seacrowd-0.0.7/seacrowd/utils/schemas/pairs_multilabel.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1007 2024-04-04 06:00:52.000000 seacrowd-0.0.7/seacrowd/utils/schemas/qa.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      206 2024-04-04 06:00:52.000000 seacrowd-0.0.7/seacrowd/utils/schemas/self_supervised_pretraining.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      525 2024-04-04 06:00:52.000000 seacrowd-0.0.7/seacrowd/utils/schemas/seq_label.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      618 2024-04-04 06:00:52.000000 seacrowd-0.0.7/seacrowd/utils/schemas/speech.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      606 2024-04-04 06:00:52.000000 seacrowd-0.0.7/seacrowd/utils/schemas/speech_multilabel.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      454 2024-04-04 06:00:52.000000 seacrowd-0.0.7/seacrowd/utils/schemas/speech_text.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      796 2024-04-04 06:00:52.000000 seacrowd-0.0.7/seacrowd/utils/schemas/speech_to_speech.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      311 2024-04-04 06:00:52.000000 seacrowd-0.0.7/seacrowd/utils/schemas/text.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      331 2024-04-04 06:00:52.000000 seacrowd-0.0.7/seacrowd/utils/schemas/text_multilabel.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      444 2024-04-04 06:00:52.000000 seacrowd-0.0.7/seacrowd/utils/schemas/text_to_text.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3046 2024-04-04 06:00:52.000000 seacrowd-0.0.7/seacrowd/utils/schemas/tod.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3068 2024-04-04 06:00:52.000000 seacrowd-0.0.7/seacrowd/utils/schemas/tree.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      810 2024-04-04 06:00:52.000000 seacrowd-0.0.7/seacrowd/utils/schemas/video.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:57.211539 seacrowd-0.0.7/seacrowd.egg-info/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1071 2024-04-12 07:52:47.000000 seacrowd-0.0.7/seacrowd.egg-info/PKG-INFO
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    31367 2024-04-12 07:52:48.000000 seacrowd-0.0.7/seacrowd.egg-info/SOURCES.txt
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        1 2024-04-12 07:52:47.000000 seacrowd-0.0.7/seacrowd.egg-info/dependency_links.txt
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      409 2024-04-12 07:52:47.000000 seacrowd-0.0.7/seacrowd.egg-info/requires.txt
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)       15 2024-04-12 07:52:47.000000 seacrowd-0.0.7/seacrowd.egg-info/top_level.txt
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      703 2024-04-12 07:52:57.242250 seacrowd-0.0.7/setup.cfg
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)       68 2024-04-12 07:28:29.000000 seacrowd-0.0.7/setup.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:52:57.191608 seacrowd-0.0.7/tests/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:52.000000 seacrowd-0.0.7/tests/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    23314 2024-04-04 06:00:52.000000 seacrowd-0.0.7/tests/test_seacrowd.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    20714 2024-04-04 06:00:52.000000 seacrowd-0.0.7/tests/test_seacrowd_source_only.py
```

### Comparing `seacrowd-0.0.6/LICENSE` & `seacrowd-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/PKG-INFO` & `seacrowd-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seacrowd
-Version: 0.0.6
+Version: 0.0.7
 Requires-Python: >=3.7
 License-File: LICENSE
 Requires-Dist: loguru>=0.5.3
 Requires-Dist: bioc>=1.3.7
 Requires-Dist: pandas>=1.3.3
 Requires-Dist: numpy>=1.20
 Requires-Dist: datasets>=2.2.0
```

### Comparing `seacrowd-0.0.6/README.md` & `seacrowd-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/config_helper.py` & `seacrowd-0.0.7/seacrowd/config_helper.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/abui_wordnet/abui_wordnet.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/abui_wordnet/abui_wordnet.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/alt_burmese_treebank/alt_burmese_treebank.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/alt_burmese_treebank/alt_burmese_treebank.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/alt_burmese_treebank/utils/alt_burmese_treebank_utils.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/alt_burmese_treebank/utils/alt_burmese_treebank_utils.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/ara_close/ara_close.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/ara_close/ara_close.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/asr_sindodusc/asr_sindodusc.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/asr_sindodusc/asr_sindodusc.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/asr_smaldusc/asr_smaldusc.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/asr_smaldusc/asr_smaldusc.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/asr_stidusc/asr_stidusc.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/asr_stidusc/asr_stidusc.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/audio_keyword_spotting/audio_keyword_spotting.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/audio_keyword_spotting/audio_keyword_spotting.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/aya_dataset/aya_dataset.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/aya_dataset/aya_dataset.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/barasa/barasa.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/barasa/barasa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/beaye_lexicon/beaye_lexicon.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/beaye_lexicon/beaye_lexicon.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/belebele/belebele.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/belebele/belebele.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/bible_en_id/bible_en_id.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/bible_en_id/bible_en_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/bible_jv_id/bible_jv_id.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/bible_jv_id/bible_jv_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/bible_su_id/bible_su_id.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/bible_su_id/bible_su_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/bioner_id/bioner_id.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/bioner_id/bioner_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/bloom_captioning/bloom_captioning.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/bloom_captioning/bloom_captioning.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/bloom_lm/bloom_lm.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/bloom_lm/bloom_lm.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/bloom_speech/bloom_speech.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/bloom_speech/bloom_speech.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/bloom_vist/bloom_vist.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/bloom_vist/bloom_vist.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/burapha_th/burapha_th.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/burapha_th/burapha_th.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/burmese_romanize/burmese_romanize.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/burmese_romanize/burmese_romanize.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/casa/casa.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/casa/casa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/cc100/cc100.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/cc100/cc100.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/cc_aligned_doc/cc_aligned_doc.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/cc_aligned_doc/cc_aligned_doc.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/cc_aligned_sent/cc_aligned_sent.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/cc_aligned_sent/cc_aligned_sent.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/cebuaner/cebuaner.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/cebuaner/cebuaner.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/coco_35l/coco_35l.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/coco_35l/coco_35l.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/cod/cod.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/cod/cod.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/code_mixed_jv_id/code_mixed_jv_id.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/code_mixed_jv_id/code_mixed_jv_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/codeswitch_reddit/codeswitch_reddit.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/codeswitch_reddit/codeswitch_reddit.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/commonvoice_120/commonvoice_120.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/commonvoice_120/commonvoice_120.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/copal/copal.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/copal/copal.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/covost2/covost2.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/covost2/covost2.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/creole_rc/creole_rc.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/creole_rc/creole_rc.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/crosssum/crosssum.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/crosssum/crosssum.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/cub_bahasa/cub_bahasa.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/cub_bahasa/cub_bahasa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/culturax/culturax.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/culturax/culturax.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/cvss/cvss.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/cvss/cvss.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/dengue_filipino/dengue_filipino.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/dengue_filipino/dengue_filipino.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/emot/emot.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/emot/emot.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/emotcmt/emotcmt.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/emotcmt/emotcmt.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/emotes_3k/emotes_3k.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/emotes_3k/emotes_3k.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/emotion_id_opinion/emotion_id_opinion.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/emotion_id_opinion/emotion_id_opinion.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/etos/etos.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/etos/etos.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/facqa/facqa.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/facqa/facqa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/facqa/utils/facqa_utils.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/facqa/utils/facqa_utils.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/fakenews_ph/fakenews_ph.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/fakenews_ph/fakenews_ph.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/filipino_gay_lang/filipino_gay_lang.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/filipino_gay_lang/filipino_gay_lang.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/filipino_hatespeech_tiktok/filipino_hatespeech_tiktok.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/filipino_hatespeech_tiktok/filipino_hatespeech_tiktok.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/filipino_slang_norm/filipino_slang_norm.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/filipino_slang_norm/filipino_slang_norm.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/filipino_words_aoa/filipino_words_aoa.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/filipino_words_aoa/filipino_words_aoa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/filwordnet/filwordnet.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/filwordnet/filwordnet.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/fleurs/fleurs.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/fleurs/fleurs.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 """
 
 import json
 from itertools import product
 from typing import Dict, List, Tuple
 
 import datasets
-import pathlib
+
 from datasets import load_dataset
 from datasets.download.download_manager import DownloadManager
 
+from seacrowd.sea_datasets.fleurs.lang_config import _LANG_CONFIG
 from seacrowd.utils import schemas
 from seacrowd.utils.configs import SEACrowdConfig
 from seacrowd.utils.constants import TASK_TO_SCHEMA, Licenses, Tasks
 
 _CITATION = """
 @inproceedings{conneau22_interspeech,
   author={Alexis Conneau and Ankur Bapna and Yu Zhang and Min Ma and Patrick {von Platen} and Anton Lozhkov and Colin Cherry
@@ -34,17 +35,14 @@
 _LOCAL = False
 
 # since this fleurs source already subsets SEA langs, the names on lang group id is hard-coded
 _LANG_GROUP_ID = ["south_east_asian_sea"]
 
 _DATASETNAME = "fleurs"
 
-path_to_here = pathlib.Path(__file__).parent.absolute()
-with open(DownloadManager().download_and_extract(f"{path_to_here}/lang_config.json"), "r") as f:
-    _LANG_CONFIG = json.load(f)
 _LANGUAGES = list(_LANG_CONFIG.keys())
 
 _DESCRIPTION = """\
     Fleurs dataset is a part of XTREME-S benchmark to evaluate universal cross-lingual speech representations in many languages.
     Fleurs is used for two tasks: automatic speech recognition and speech classification.
     Fleurs covers 10 language native to Southeast Asian and other 3 major languages
     mostly spoken in few of Southeast Asia countries (Mandarin Chinese, Portuguese, and Tamil).
```

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/fleurs/lang_config.json` & `seacrowd-0.0.7/seacrowd/sea_datasets/fleurs/lang_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-00000000: 7b0a 2020 226d 7961 223a 207b 0a20 2020  {.  "mya": {.   
-00000010: 2022 666c 6575 7273 5f6c 616e 675f 636f   "fleurs_lang_co
-00000020: 6465 223a 2022 6d79 222c 0a20 2020 2022  de": "my",.    "
-00000030: 666c 6575 7273 5f63 6f75 6e74 7279 5f63  fleurs_country_c
-00000040: 6f64 6522 3a20 226d 6d22 0a20 207d 2c0a  ode": "mm".  },.
-00000050: 2020 2263 6562 223a 207b 0a20 2020 2022    "ceb": {.    "
-00000060: 666c 6575 7273 5f6c 616e 675f 636f 6465  fleurs_lang_code
-00000070: 223a 2022 6365 6222 2c0a 2020 2020 2266  ": "ceb",.    "f
-00000080: 6c65 7572 735f 636f 756e 7472 795f 636f  leurs_country_co
-00000090: 6465 223a 2022 7068 220a 2020 7d2c 0a20  de": "ph".  },. 
-000000a0: 2022 6669 6c22 3a20 7b0a 2020 2020 2266   "fil": {.    "f
-000000b0: 6c65 7572 735f 6c61 6e67 5f63 6f64 6522  leurs_lang_code"
-000000c0: 3a20 2266 696c 222c 0a20 2020 2022 666c  : "fil",.    "fl
-000000d0: 6575 7273 5f63 6f75 6e74 7279 5f63 6f64  eurs_country_cod
-000000e0: 6522 3a20 2270 6822 0a20 207d 2c0a 2020  e": "ph".  },.  
-000000f0: 2269 6e64 223a 207b 0a20 2020 2022 666c  "ind": {.    "fl
-00000100: 6575 7273 5f6c 616e 675f 636f 6465 223a  eurs_lang_code":
-00000110: 2022 6964 222c 0a20 2020 2022 666c 6575   "id",.    "fleu
-00000120: 7273 5f63 6f75 6e74 7279 5f63 6f64 6522  rs_country_code"
-00000130: 3a20 2269 6422 0a20 207d 2c0a 2020 226a  : "id".  },.  "j
-00000140: 6176 223a 207b 0a20 2020 2022 666c 6575  av": {.    "fleu
-00000150: 7273 5f6c 616e 675f 636f 6465 223a 2022  rs_lang_code": "
-00000160: 6a76 222c 0a20 2020 2022 666c 6575 7273  jv",.    "fleurs
-00000170: 5f63 6f75 6e74 7279 5f63 6f64 6522 3a20  _country_code": 
-00000180: 2269 6422 0a20 207d 2c0a 2020 226b 686d  "id".  },.  "khm
-00000190: 223a 207b 0a20 2020 2022 666c 6575 7273  ": {.    "fleurs
-000001a0: 5f6c 616e 675f 636f 6465 223a 2022 6b6d  _lang_code": "km
-000001b0: 222c 0a20 2020 2022 666c 6575 7273 5f63  ",.    "fleurs_c
-000001c0: 6f75 6e74 7279 5f63 6f64 6522 3a20 226b  ountry_code": "k
-000001d0: 6822 0a20 207d 2c0a 2020 226c 616f 223a  h".  },.  "lao":
-000001e0: 207b 0a20 2020 2022 666c 6575 7273 5f6c   {.    "fleurs_l
-000001f0: 616e 675f 636f 6465 223a 2022 6c6f 222c  ang_code": "lo",
-00000200: 0a20 2020 2022 666c 6575 7273 5f63 6f75  .    "fleurs_cou
-00000210: 6e74 7279 5f63 6f64 6522 3a20 226c 6122  ntry_code": "la"
-00000220: 0a20 207d 2c0a 2020 227a 6c6d 223a 207b  .  },.  "zlm": {
-00000230: 0a20 2020 2022 666c 6575 7273 5f6c 616e  .    "fleurs_lan
-00000240: 675f 636f 6465 223a 2022 6d73 222c 0a20  g_code": "ms",. 
-00000250: 2020 2022 666c 6575 7273 5f63 6f75 6e74     "fleurs_count
-00000260: 7279 5f63 6f64 6522 3a20 226d 7922 0a20  ry_code": "my". 
-00000270: 207d 2c0a 2020 2274 6861 223a 207b 0a20   },.  "tha": {. 
-00000280: 2020 2022 666c 6575 7273 5f6c 616e 675f     "fleurs_lang_
-00000290: 636f 6465 223a 2022 7468 222c 0a20 2020  code": "th",.   
-000002a0: 2022 666c 6575 7273 5f63 6f75 6e74 7279   "fleurs_country
-000002b0: 5f63 6f64 6522 3a20 2274 6822 0a20 207d  _code": "th".  }
-000002c0: 2c0a 2020 2276 6965 223a 207b 0a20 2020  ,.  "vie": {.   
-000002d0: 2022 666c 6575 7273 5f6c 616e 675f 636f   "fleurs_lang_co
-000002e0: 6465 223a 2022 7669 222c 0a20 2020 2022  de": "vi",.    "
-000002f0: 666c 6575 7273 5f63 6f75 6e74 7279 5f63  fleurs_country_c
-00000300: 6f64 6522 3a20 2276 6e22 0a20 207d 0a7d  ode": "vn".  }.}
-00000310: 0a                                       .
+00000000: 5f4c 414e 475f 434f 4e46 4947 203d 207b  _LANG_CONFIG = {
+00000010: 0a20 2022 6d79 6122 3a20 7b0a 2020 2020  .  "mya": {.    
+00000020: 2266 6c65 7572 735f 6c61 6e67 5f63 6f64  "fleurs_lang_cod
+00000030: 6522 3a20 226d 7922 2c0a 2020 2020 2266  e": "my",.    "f
+00000040: 6c65 7572 735f 636f 756e 7472 795f 636f  leurs_country_co
+00000050: 6465 223a 2022 6d6d 220a 2020 7d2c 0a20  de": "mm".  },. 
+00000060: 2022 6365 6222 3a20 7b0a 2020 2020 2266   "ceb": {.    "f
+00000070: 6c65 7572 735f 6c61 6e67 5f63 6f64 6522  leurs_lang_code"
+00000080: 3a20 2263 6562 222c 0a20 2020 2022 666c  : "ceb",.    "fl
+00000090: 6575 7273 5f63 6f75 6e74 7279 5f63 6f64  eurs_country_cod
+000000a0: 6522 3a20 2270 6822 0a20 207d 2c0a 2020  e": "ph".  },.  
+000000b0: 2266 696c 223a 207b 0a20 2020 2022 666c  "fil": {.    "fl
+000000c0: 6575 7273 5f6c 616e 675f 636f 6465 223a  eurs_lang_code":
+000000d0: 2022 6669 6c22 2c0a 2020 2020 2266 6c65   "fil",.    "fle
+000000e0: 7572 735f 636f 756e 7472 795f 636f 6465  urs_country_code
+000000f0: 223a 2022 7068 220a 2020 7d2c 0a20 2022  ": "ph".  },.  "
+00000100: 696e 6422 3a20 7b0a 2020 2020 2266 6c65  ind": {.    "fle
+00000110: 7572 735f 6c61 6e67 5f63 6f64 6522 3a20  urs_lang_code": 
+00000120: 2269 6422 2c0a 2020 2020 2266 6c65 7572  "id",.    "fleur
+00000130: 735f 636f 756e 7472 795f 636f 6465 223a  s_country_code":
+00000140: 2022 6964 220a 2020 7d2c 0a20 2022 6a61   "id".  },.  "ja
+00000150: 7622 3a20 7b0a 2020 2020 2266 6c65 7572  v": {.    "fleur
+00000160: 735f 6c61 6e67 5f63 6f64 6522 3a20 226a  s_lang_code": "j
+00000170: 7622 2c0a 2020 2020 2266 6c65 7572 735f  v",.    "fleurs_
+00000180: 636f 756e 7472 795f 636f 6465 223a 2022  country_code": "
+00000190: 6964 220a 2020 7d2c 0a20 2022 6b68 6d22  id".  },.  "khm"
+000001a0: 3a20 7b0a 2020 2020 2266 6c65 7572 735f  : {.    "fleurs_
+000001b0: 6c61 6e67 5f63 6f64 6522 3a20 226b 6d22  lang_code": "km"
+000001c0: 2c0a 2020 2020 2266 6c65 7572 735f 636f  ,.    "fleurs_co
+000001d0: 756e 7472 795f 636f 6465 223a 2022 6b68  untry_code": "kh
+000001e0: 220a 2020 7d2c 0a20 2022 6c61 6f22 3a20  ".  },.  "lao": 
+000001f0: 7b0a 2020 2020 2266 6c65 7572 735f 6c61  {.    "fleurs_la
+00000200: 6e67 5f63 6f64 6522 3a20 226c 6f22 2c0a  ng_code": "lo",.
+00000210: 2020 2020 2266 6c65 7572 735f 636f 756e      "fleurs_coun
+00000220: 7472 795f 636f 6465 223a 2022 6c61 220a  try_code": "la".
+00000230: 2020 7d2c 0a20 2022 7a6c 6d22 3a20 7b0a    },.  "zlm": {.
+00000240: 2020 2020 2266 6c65 7572 735f 6c61 6e67      "fleurs_lang
+00000250: 5f63 6f64 6522 3a20 226d 7322 2c0a 2020  _code": "ms",.  
+00000260: 2020 2266 6c65 7572 735f 636f 756e 7472    "fleurs_countr
+00000270: 795f 636f 6465 223a 2022 6d79 220a 2020  y_code": "my".  
+00000280: 7d2c 0a20 2022 7468 6122 3a20 7b0a 2020  },.  "tha": {.  
+00000290: 2020 2266 6c65 7572 735f 6c61 6e67 5f63    "fleurs_lang_c
+000002a0: 6f64 6522 3a20 2274 6822 2c0a 2020 2020  ode": "th",.    
+000002b0: 2266 6c65 7572 735f 636f 756e 7472 795f  "fleurs_country_
+000002c0: 636f 6465 223a 2022 7468 220a 2020 7d2c  code": "th".  },
+000002d0: 0a20 2022 7669 6522 3a20 7b0a 2020 2020  .  "vie": {.    
+000002e0: 2266 6c65 7572 735f 6c61 6e67 5f63 6f64  "fleurs_lang_cod
+000002f0: 6522 3a20 2276 6922 2c0a 2020 2020 2266  e": "vi",.    "f
+00000300: 6c65 7572 735f 636f 756e 7472 795f 636f  leurs_country_co
+00000310: 6465 223a 2022 766e 220a 2020 7d0a 7d0a  de": "vn".  }.}.
```

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/flores200/flores200.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/flores200/flores200.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/fsl_105/fsl_105.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/fsl_105/fsl_105.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/gatitos/gatitos.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/gatitos/gatitos.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/gklmip_newsclass/gklmip_newsclass.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/gklmip_newsclass/gklmip_newsclass.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/gklmip_sentiment/gklmip_sentiment.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/gklmip_sentiment/gklmip_sentiment.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/globalwoz/globalwoz.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/globalwoz/globalwoz.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/glotstorybook/glotstorybook.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/glotstorybook/glotstorybook.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/hoasa/hoasa.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/hoasa/hoasa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/iapp_squad/iapp_squad.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/iapp_squad/iapp_squad.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/iatf/iatf.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/iatf/iatf.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/icon/icon.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/icon/icon.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/id_abusive/id_abusive.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/id_abusive/id_abusive.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/id_abusive_news_comment/id_abusive_news_comment.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/id_abusive_news_comment/id_abusive_news_comment.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/id_am2ico/id_am2ico.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/id_am2ico/id_am2ico.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/id_clickbait/id_clickbait.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/id_clickbait/id_clickbait.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/id_coreference_resolution/id_coreference_resolution.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/id_coreference_resolution/id_coreference_resolution.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/id_frog_story/id_frog_story.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/id_frog_story/id_frog_story.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/id_google_play_review/id_google_play_review.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/id_google_play_review/id_google_play_review.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/id_hatespeech/id_hatespeech.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/id_hatespeech/id_hatespeech.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/id_hoax_news/id_hoax_news.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/id_hoax_news/id_hoax_news.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/id_hsd_nofaaulia/id_hsd_nofaaulia.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/id_hsd_nofaaulia/id_hsd_nofaaulia.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/id_msvd/id_msvd.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/id_msvd/id_msvd.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/id_multilabel_hs/id_multilabel_hs.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/id_multilabel_hs/id_multilabel_hs.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/id_panl_bppt/id_panl_bppt.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/id_panl_bppt/id_panl_bppt.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/id_qqp/id_qqp.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/id_qqp/id_qqp.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/id_sent_emo_mobile_apps/id_sent_emo_mobile_apps.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/id_sent_emo_mobile_apps/id_sent_emo_mobile_apps.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/id_sentiment_analysis/id_sentiment_analysis.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/id_sentiment_analysis/id_sentiment_analysis.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/id_short_answer_grading/id_short_answer_grading.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/id_short_answer_grading/id_short_answer_grading.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/id_short_answer_grading/utils/id_short_answer_grading_utils.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/id_short_answer_grading/utils/id_short_answer_grading_utils.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/id_stance/id_stance.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/id_stance/id_stance.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/id_sts/id_sts.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/id_sts/id_sts.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/id_vaccines_tweets/id_vaccines_tweets.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/id_vaccines_tweets/id_vaccines_tweets.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/id_wiki_parallel/id_wiki_parallel.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/id_wiki_parallel/id_wiki_parallel.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/id_wsd/id_wsd.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/id_wsd/id_wsd.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/identic/identic.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/identic/identic.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/identifikasi_bahasa/identifikasi_bahasa.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/identifikasi_bahasa/identifikasi_bahasa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/idk_mrc/idk_mrc.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/idk_mrc/idk_mrc.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/idn_tagged_corpus_csui/idn_tagged_corpus_csui.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/idn_tagged_corpus_csui/idn_tagged_corpus_csui.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/ijelid/ijelid.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/ijelid/ijelid.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/imdb_jv/imdb_jv.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/imdb_jv/imdb_jv.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/indo4b/indo4b.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/indo4b/indo4b.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/indo4b_plus/indo4b_plus.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/indo4b_plus/indo4b_plus.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/indo_general_mt_en_id/indo_general_mt_en_id.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/indo_general_mt_en_id/indo_general_mt_en_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/indo_law/indo_law.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/indo_law/indo_law.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/indo_puisi/indo_puisi.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/indo_puisi/indo_puisi.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/indo_religious_mt_en_id/indo_religious_mt_en_id.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/indo_religious_mt_en_id/indo_religious_mt_en_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/indo_story_cloze/indo_story_cloze.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/indo_story_cloze/indo_story_cloze.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/indocamrest/indocamrest.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/indocamrest/indocamrest.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/indocollex/indocollex.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/indocollex/indocollex.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/indocoref/indocoref.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/indocoref/indocoref.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/indocoref/utils/feature_utils.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/indocoref/utils/feature_utils.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/indocoref/utils/file_utils.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/indocoref/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/indocoref/utils/text_preprocess.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/indocoref/utils/text_preprocess.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/indolem_ner_ugm/indolem_ner_ugm.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/indolem_ner_ugm/indolem_ner_ugm.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/indolem_nerui/indolem_nerui.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/indolem_nerui/indolem_nerui.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/indolem_ntp/indolem_ntp.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/indolem_ntp/indolem_ntp.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/indolem_sentiment/indolem_sentiment.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/indolem_sentiment/indolem_sentiment.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/indolem_tweet_ordering/indolem_tweet_ordering.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/indolem_tweet_ordering/indolem_tweet_ordering.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/indolem_ud_id_gsd/indolem_ud_id_gsd.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/indolem_ud_id_gsd/indolem_ud_id_gsd.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/indolem_ud_id_pud/indolem_ud_id_pud.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/indolem_ud_id_pud/indolem_ud_id_pud.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/indoler/indoler.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/indoler/indoler.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/indommlu/indommlu.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/indommlu/indommlu.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/indoner_tourism/indoner_tourism.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/indoner_tourism/indoner_tourism.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/indonesia_chinese_mtrobusteval/indonesia_chinese_mtrobusteval.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/indonesia_chinese_mtrobusteval/indonesia_chinese_mtrobusteval.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/indonesian_madurese_bible_translation/indonesian_madurese_bible_translation.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/indonesian_madurese_bible_translation/indonesian_madurese_bible_translation.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/indonesian_news_dataset/indonesian_news_dataset.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/indonesian_news_dataset/indonesian_news_dataset.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/indonesiannmt/indonesiannmt.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/indonesiannmt/indonesiannmt.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/indonglish/indonglish.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/indonglish/indonglish.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/indonli/indonli.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/indonli/indonli.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/indonlu_nergrit/indonlu_nergrit.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/indonlu_nergrit/indonlu_nergrit.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/indoqa/indoqa.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/indoqa/indoqa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/indosmd/indosmd.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/indosmd/indosmd.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/indosum/indosum.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/indosum/indosum.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/indotacos/indotacos.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/indotacos/indotacos.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/indowiki/indowiki.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/indowiki/indowiki.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/indqner/indqner.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/indqner/indqner.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_digit_cdsr/indspeech_digit_cdsr.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/indspeech_digit_cdsr/indspeech_digit_cdsr.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_news_ethnicsr/indspeech_news_ethnicsr.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/indspeech_news_ethnicsr/indspeech_news_ethnicsr.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_news_lvcsr/indspeech_news_lvcsr.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/indspeech_news_lvcsr/indspeech_news_lvcsr.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_news_tts/indspeech_news_tts.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/indspeech_news_tts/indspeech_news_tts.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_newstra_ethnicsr/indspeech_newstra_ethnicsr.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/indspeech_newstra_ethnicsr/indspeech_newstra_ethnicsr.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_teldialog_lvcsr/indspeech_teldialog_lvcsr.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/indspeech_teldialog_lvcsr/indspeech_teldialog_lvcsr.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_teldialog_svcsr/indspeech_teldialog_svcsr.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/indspeech_teldialog_svcsr/indspeech_teldialog_svcsr.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/inset_lexicon/inset_lexicon.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/inset_lexicon/inset_lexicon.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/jadi_ide/jadi_ide.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/jadi_ide/jadi_ide.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/jv_id_asr/jv_id_asr.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/jv_id_asr/jv_id_asr.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/jv_id_tts/jv_id_tts.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/jv_id_tts/jv_id_tts.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/kamus_alay/kamus_alay.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/kamus_alay/kamus_alay.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/karonese_sentiment/karonese_sentiment.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/karonese_sentiment/karonese_sentiment.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/kawat/kawat.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/kawat/kawat.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/kde4/kde4.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/kde4/kde4.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/keps/keps.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/keps/keps.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/kheng_info/kheng_info.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/kheng_info/kheng_info.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/khmer_alt_pos/khmer_alt_pos.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/khmer_alt_pos/khmer_alt_pos.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/khpos/khpos.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/khpos/khpos.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/kopi_cc/kopi_cc.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/kopi_cc/kopi_cc.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/kopi_cc_news/kopi_cc_news.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/kopi_cc_news/kopi_cc_news.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/kopi_nllb/kopi_nllb.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/kopi_nllb/kopi_nllb.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/korpus_nusantara/korpus_nusantara.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/korpus_nusantara/korpus_nusantara.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/lazada_review_filipino/lazada_review_filipino.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/lazada_review_filipino/lazada_review_filipino.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/librivox_indonesia/librivox_indonesia.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/librivox_indonesia/librivox_indonesia.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/limesoda/limesoda.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/limesoda/limesoda.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/liputan6/liputan6.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/liputan6/liputan6.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/local_id_abusive/local_id_abusive.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/local_id_abusive/local_id_abusive.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/lr_sum/lr_sum.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/lr_sum/lr_sum.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/m3exam/m3exam.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/m3exam/m3exam.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/mabl/mabl.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/mabl/mabl.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/malaysia_tweets/malaysia_tweets.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/malaysia_tweets/malaysia_tweets.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/malindo_morph/malindo_morph.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/malindo_morph/malindo_morph.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/malindo_parallel/malindo_parallel.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/malindo_parallel/malindo_parallel.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/massive/massive.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/massive/massive.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/mc4_indo/mc4_indo.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/mc4_indo/mc4_indo.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/melayu_brunei/melayu_brunei.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/melayu_brunei/melayu_brunei.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/melayu_sabah/melayu_sabah.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/melayu_sabah/melayu_sabah.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/melayu_sarawak/melayu_sarawak.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/melayu_sarawak/melayu_sarawak.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/melayu_standard_lisan/melayu_standard_lisan.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/melayu_standard_lisan/melayu_standard_lisan.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/memolon/memolon.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/memolon/memolon.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/minangnlp_mt/minangnlp_mt.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/minangnlp_mt/minangnlp_mt.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/miracl/miracl.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/miracl/miracl.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/mkqa/mkqa.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/mkqa/mkqa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/mlqa/mlqa.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/mlqa/mlqa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/mozilla_pontoon/mozilla_pontoon.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/mozilla_pontoon/mozilla_pontoon.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/mswc/mswc.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/mswc/mswc.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/mtop_intent_classification/labels.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/mtop_intent_classification/labels.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/mtop_intent_classification/mtop_intent_classification.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/mtop_intent_classification/mtop_intent_classification.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/multilexnorm/multilexnorm.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/multilexnorm/multilexnorm.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/my_paraphrase/my_paraphrase.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/my_paraphrase/my_paraphrase.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/myanmar_rakhine_parallel/myanmar_rakhine_parallel.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/myanmar_rakhine_parallel/myanmar_rakhine_parallel.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/mypos/mypos.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/mypos/mypos.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/mysentence/mysentence.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/mysentence/mysentence.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/myxnli/myxnli.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/myxnli/myxnli.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/nergrit/nergrit.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/nergrit/nergrit.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/nerp/nerp.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/nerp/nerp.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/netifier/netifier.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/netifier/netifier.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/news_en_id/news_en_id.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/news_en_id/news_en_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/newsph/newsph.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/newsph/newsph.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/nllb_seed/nllb_seed.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/nllb_seed/nllb_seed.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/ntrex_128/ntrex_128.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/ntrex_128/ntrex_128.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/nusaparagraph_emot/nusaparagraph_emot.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/nusaparagraph_emot/nusaparagraph_emot.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/nusaparagraph_rhetoric/nusaparagraph_rhetoric.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/nusaparagraph_rhetoric/nusaparagraph_rhetoric.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/nusaparagraph_topic/nusaparagraph_topic.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/nusaparagraph_topic/nusaparagraph_topic.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/nusatranslation_emot/nusatranslation_emot.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/nusatranslation_emot/nusatranslation_emot.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/nusatranslation_mt/nusatranslation_mt.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/nusatranslation_mt/nusatranslation_mt.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/nusatranslation_senti/nusatranslation_senti.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/nusatranslation_senti/nusatranslation_senti.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/nusax_mt/nusax_mt.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/nusax_mt/nusax_mt.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/nusax_senti/nusax_senti.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/nusax_senti/nusax_senti.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/oil/oil.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/oil/oil.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/ojw/ojw.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/ojw/ojw.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/openlid/openlid.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/openlid/openlid.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/openslr/openslr.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/openslr/openslr.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/orchid_pos/orchid_pos.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/orchid_pos/orchid_pos.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/oscar_2201/oscar_2201.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/oscar_2201/oscar_2201.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/palito/palito.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/palito/palito.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/paracotta_id/paracotta_id.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/paracotta_id/paracotta_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/parallel_id_nyo/parallel_id_nyo.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/parallel_id_nyo/parallel_id_nyo.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/parallel_su_id/parallel_su_id.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/parallel_su_id/parallel_su_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/ph_fake_news_corpus/ph_fake_news_corpus.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/ph_fake_news_corpus/ph_fake_news_corpus.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/pho_ner_covid/pho_ner_covid.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/pho_ner_covid/pho_ner_covid.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/phomt/phomt.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/phomt/phomt.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/phost/phost.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/phost/phost.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/posp/posp.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/posp/posp.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/postag_su/postag_su.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/postag_su/postag_su.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/prdect_id/prdect_id.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/prdect_id/prdect_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/qasina/qasina.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/qasina/qasina.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/roots_vi_ted/roots_vi_ted.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/roots_vi_ted/roots_vi_ted.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/sampiran/sampiran.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/sampiran/sampiran.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/sap_wat/sap_wat.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/sap_wat/sap_wat.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/sarawak_malay/sarawak_malay.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/sarawak_malay/sarawak_malay.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/scb_mt_en_th/scb_mt_en_th.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/scb_mt_en_th/scb_mt_en_th.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/sea_bench/sea_bench.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/sea_bench/sea_bench.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/sea_madlad/sea_madlad.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/sea_madlad/sea_madlad.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/sea_wiki/lang_config.json` & `seacrowd-0.0.7/seacrowd/sea_datasets/sea_wiki/lang_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,115 +1,116 @@
-00000000: 7b0a 2020 2261 6365 223a 207b 0a20 2020  {.  "ace": {.   
-00000010: 2022 6e61 6d65 223a 2022 4163 6568 6e65   "name": "Acehne
-00000020: 7365 222c 0a20 2020 2022 736f 7572 6365  se",.    "source
-00000030: 5f73 7562 7365 7422 3a20 2261 6365 220a  _subset": "ace".
-00000040: 2020 7d2c 0a20 2022 6261 6e22 3a20 7b0a    },.  "ban": {.
-00000050: 2020 2020 226e 616d 6522 3a20 2242 616c      "name": "Bal
-00000060: 696e 6573 6522 2c0a 2020 2020 2273 6f75  inese",.    "sou
-00000070: 7263 655f 7375 6273 6574 223a 2022 6261  rce_subset": "ba
-00000080: 6e22 0a20 207d 2c0a 2020 2262 636c 223a  n".  },.  "bcl":
-00000090: 207b 0a20 2020 2022 6e61 6d65 223a 2022   {.    "name": "
-000000a0: 4365 6e74 7261 6c20 4269 636f 6c61 6e6f  Central Bicolano
-000000b0: 222c 0a20 2020 2022 736f 7572 6365 5f73  ",.    "source_s
-000000c0: 7562 7365 7422 3a20 2262 636c 220a 2020  ubset": "bcl".  
-000000d0: 7d2c 0a20 2022 626a 6e22 3a20 7b0a 2020  },.  "bjn": {.  
-000000e0: 2020 226e 616d 6522 3a20 2242 616e 6a61    "name": "Banja
-000000f0: 7265 7365 222c 0a20 2020 2022 736f 7572  rese",.    "sour
-00000100: 6365 5f73 7562 7365 7422 3a20 2262 6a6e  ce_subset": "bjn
-00000110: 220a 2020 7d2c 0a20 2022 6275 6722 3a20  ".  },.  "bug": 
-00000120: 7b0a 2020 2020 226e 616d 6522 3a20 2242  {.    "name": "B
-00000130: 7567 696e 6573 6522 2c0a 2020 2020 2273  uginese",.    "s
-00000140: 6f75 7263 655f 7375 6273 6574 223a 2022  ource_subset": "
-00000150: 6275 6722 0a20 207d 2c0a 2020 2263 626b  bug".  },.  "cbk
-00000160: 223a 207b 0a20 2020 2022 6e61 6d65 223a  ": {.    "name":
-00000170: 2022 4368 6176 6163 616e 6f22 2c0a 2020   "Chavacano",.  
-00000180: 2020 2273 6f75 7263 655f 7375 6273 6574    "source_subset
-00000190: 223a 2022 6362 6b2d 7a61 6d22 0a20 207d  ": "cbk-zam".  }
-000001a0: 2c0a 2020 2267 6f72 223a 207b 0a20 2020  ,.  "gor": {.   
-000001b0: 2022 6e61 6d65 223a 2022 476f 726f 6e74   "name": "Goront
-000001c0: 616c 6f22 2c0a 2020 2020 2273 6f75 7263  alo",.    "sourc
-000001d0: 655f 7375 6273 6574 223a 2022 676f 7222  e_subset": "gor"
-000001e0: 0a20 207d 2c0a 2020 2269 6c6f 223a 207b  .  },.  "ilo": {
-000001f0: 0a20 2020 2022 6e61 6d65 223a 2022 496c  .    "name": "Il
-00000200: 6f6b 616e 6f22 2c0a 2020 2020 2273 6f75  okano",.    "sou
-00000210: 7263 655f 7375 6273 6574 223a 2022 696c  rce_subset": "il
-00000220: 6f22 0a20 207d 2c0a 2020 2269 6e64 223a  o".  },.  "ind":
-00000230: 207b 0a20 2020 2022 6e61 6d65 223a 2022   {.    "name": "
-00000240: 496e 646f 6e65 7369 616e 222c 0a20 2020  Indonesian",.   
-00000250: 2022 736f 7572 6365 5f73 7562 7365 7422   "source_subset"
-00000260: 3a20 2269 6422 0a20 207d 2c0a 2020 226a  : "id".  },.  "j
-00000270: 6176 223a 207b 0a20 2020 2022 6e61 6d65  av": {.    "name
-00000280: 223a 2022 4a61 7661 6e65 7365 222c 0a20  ": "Javanese",. 
-00000290: 2020 2022 736f 7572 6365 5f73 7562 7365     "source_subse
-000002a0: 7422 3a20 226a 7622 0a20 207d 2c0a 2020  t": "jv".  },.  
-000002b0: 226b 686d 223a 207b 0a20 2020 2022 6e61  "khm": {.    "na
-000002c0: 6d65 223a 2022 4b68 6d65 7222 2c0a 2020  me": "Khmer",.  
-000002d0: 2020 2273 6f75 7263 655f 7375 6273 6574    "source_subset
-000002e0: 223a 2022 6b6d 220a 2020 7d2c 0a20 2022  ": "km".  },.  "
-000002f0: 6c61 6f22 3a20 7b0a 2020 2020 226e 616d  lao": {.    "nam
-00000300: 6522 3a20 224c 616f 222c 0a20 2020 2022  e": "Lao",.    "
-00000310: 736f 7572 6365 5f73 7562 7365 7422 3a20  source_subset": 
-00000320: 226c 6f22 0a20 207d 2c0a 2020 226d 6164  "lo".  },.  "mad
-00000330: 223a 207b 0a20 2020 2022 6e61 6d65 223a  ": {.    "name":
-00000340: 2022 4d61 6475 7265 7365 222c 0a20 2020   "Madurese",.   
-00000350: 2022 736f 7572 6365 5f73 7562 7365 7422   "source_subset"
-00000360: 3a20 226d 6164 220a 2020 7d2c 0a20 2022  : "mad".  },.  "
-00000370: 6d61 705f 626d 7322 3a20 7b0a 2020 2020  map_bms": {.    
-00000380: 226e 616d 6522 3a20 2242 616e 7975 6d61  "name": "Banyuma
-00000390: 7361 6e20 2844 6961 6c65 6374 206f 6620  san (Dialect of 
-000003a0: 4a61 7661 6e65 7365 2922 2c0a 2020 2020  Javanese)",.    
-000003b0: 2273 6f75 7263 655f 7375 6273 6574 223a  "source_subset":
-000003c0: 2022 6d61 702d 626d 7322 0a20 207d 2c0a   "map-bms".  },.
-000003d0: 2020 226d 696e 223a 207b 0a20 2020 2022    "min": {.    "
-000003e0: 6e61 6d65 223a 2022 4d69 6e61 6e67 6b61  name": "Minangka
-000003f0: 6261 7522 2c0a 2020 2020 2273 6f75 7263  bau",.    "sourc
-00000400: 655f 7375 6273 6574 223a 2022 6d69 6e22  e_subset": "min"
-00000410: 0a20 207d 2c0a 2020 226d 6e77 223a 207b  .  },.  "mnw": {
-00000420: 0a20 2020 2022 6e61 6d65 223a 2022 4d6f  .    "name": "Mo
-00000430: 6e22 2c0a 2020 2020 2273 6f75 7263 655f  n",.    "source_
-00000440: 7375 6273 6574 223a 2022 6d69 6e22 0a20  subset": "min". 
-00000450: 207d 2c0a 2020 226d 7961 223a 207b 0a20   },.  "mya": {. 
-00000460: 2020 2022 6e61 6d65 223a 2022 4275 726d     "name": "Burm
-00000470: 6573 6522 2c0a 2020 2020 2273 6f75 7263  ese",.    "sourc
-00000480: 655f 7375 6273 6574 223a 2022 6d79 220a  e_subset": "my".
-00000490: 2020 7d2c 0a20 2022 6e69 6122 3a20 7b0a    },.  "nia": {.
-000004a0: 2020 2020 226e 616d 6522 3a20 224e 6961      "name": "Nia
-000004b0: 7322 2c0a 2020 2020 2273 6f75 7263 655f  s",.    "source_
-000004c0: 7375 6273 6574 223a 2022 6e69 6122 0a20  subset": "nia". 
-000004d0: 207d 2c0a 2020 2270 6167 223a 207b 0a20   },.  "pag": {. 
-000004e0: 2020 2022 6e61 6d65 223a 2022 5061 6e67     "name": "Pang
-000004f0: 6173 696e 616e 222c 0a20 2020 2022 736f  asinan",.    "so
-00000500: 7572 6365 5f73 7562 7365 7422 3a20 2270  urce_subset": "p
-00000510: 6167 220a 2020 7d2c 0a20 2022 7061 6d22  ag".  },.  "pam"
-00000520: 3a20 7b0a 2020 2020 226e 616d 6522 3a20  : {.    "name": 
-00000530: 224b 6170 616d 7061 6e67 616e 222c 0a20  "Kapampangan",. 
-00000540: 2020 2022 736f 7572 6365 5f73 7562 7365     "source_subse
-00000550: 7422 3a20 2270 616d 220a 2020 7d2c 0a20  t": "pam".  },. 
-00000560: 2022 7368 6e22 3a20 7b0a 2020 2020 226e   "shn": {.    "n
-00000570: 616d 6522 3a20 2253 6861 6e22 2c0a 2020  ame": "Shan",.  
-00000580: 2020 2273 6f75 7263 655f 7375 6273 6574    "source_subset
-00000590: 223a 2022 7368 6e22 0a20 207d 2c0a 2020  ": "shn".  },.  
-000005a0: 2273 756e 223a 207b 0a20 2020 2022 6e61  "sun": {.    "na
-000005b0: 6d65 223a 2022 5375 6e64 616e 6573 6522  me": "Sundanese"
-000005c0: 2c0a 2020 2020 2273 6f75 7263 655f 7375  ,.    "source_su
-000005d0: 6273 6574 223a 2022 7375 220a 2020 7d2c  bset": "su".  },
-000005e0: 0a20 2022 7465 7422 3a20 7b0a 2020 2020  .  "tet": {.    
-000005f0: 226e 616d 6522 3a20 2254 6574 756d 222c  "name": "Tetum",
-00000600: 0a20 2020 2022 736f 7572 6365 5f73 7562  .    "source_sub
-00000610: 7365 7422 3a20 2274 6574 220a 2020 7d2c  set": "tet".  },
-00000620: 0a20 2022 7467 6c22 3a20 7b0a 2020 2020  .  "tgl": {.    
-00000630: 226e 616d 6522 3a20 2254 6167 616c 6f67  "name": "Tagalog
-00000640: 222c 0a20 2020 2022 736f 7572 6365 5f73  ",.    "source_s
-00000650: 7562 7365 7422 3a20 2274 6c22 0a20 207d  ubset": "tl".  }
-00000660: 2c0a 2020 2274 6861 223a 207b 0a20 2020  ,.  "tha": {.   
-00000670: 2022 6e61 6d65 223a 2022 5468 6169 222c   "name": "Thai",
-00000680: 0a20 2020 2022 736f 7572 6365 5f73 7562  .    "source_sub
-00000690: 7365 7422 3a20 2274 6822 0a20 207d 2c0a  set": "th".  },.
-000006a0: 2020 2276 6965 223a 207b 0a20 2020 2022    "vie": {.    "
-000006b0: 6e61 6d65 223a 2022 5669 6574 6e61 6d65  name": "Vietname
-000006c0: 7365 222c 0a20 2020 2022 736f 7572 6365  se",.    "source
-000006d0: 5f73 7562 7365 7422 3a20 2276 6922 0a20  _subset": "vi". 
-000006e0: 207d 2c0a 2020 2277 6172 223a 207b 0a20   },.  "war": {. 
-000006f0: 2020 2022 6e61 6d65 223a 2022 5761 7261     "name": "Wara
-00000700: 7922 2c0a 2020 2020 2273 6f75 7263 655f  y",.    "source_
-00000710: 7375 6273 6574 223a 2022 7761 7222 0a20  subset": "war". 
-00000720: 207d 0a7d 0a                              }.}.
+00000000: 5f4c 414e 475f 434f 4e46 4947 203d 207b  _LANG_CONFIG = {
+00000010: 0a20 2022 6163 6522 3a20 7b0a 2020 2020  .  "ace": {.    
+00000020: 226e 616d 6522 3a20 2241 6365 686e 6573  "name": "Acehnes
+00000030: 6522 2c0a 2020 2020 2273 6f75 7263 655f  e",.    "source_
+00000040: 7375 6273 6574 223a 2022 6163 6522 0a20  subset": "ace". 
+00000050: 207d 2c0a 2020 2262 616e 223a 207b 0a20   },.  "ban": {. 
+00000060: 2020 2022 6e61 6d65 223a 2022 4261 6c69     "name": "Bali
+00000070: 6e65 7365 222c 0a20 2020 2022 736f 7572  nese",.    "sour
+00000080: 6365 5f73 7562 7365 7422 3a20 2262 616e  ce_subset": "ban
+00000090: 220a 2020 7d2c 0a20 2022 6263 6c22 3a20  ".  },.  "bcl": 
+000000a0: 7b0a 2020 2020 226e 616d 6522 3a20 2243  {.    "name": "C
+000000b0: 656e 7472 616c 2042 6963 6f6c 616e 6f22  entral Bicolano"
+000000c0: 2c0a 2020 2020 2273 6f75 7263 655f 7375  ,.    "source_su
+000000d0: 6273 6574 223a 2022 6263 6c22 0a20 207d  bset": "bcl".  }
+000000e0: 2c0a 2020 2262 6a6e 223a 207b 0a20 2020  ,.  "bjn": {.   
+000000f0: 2022 6e61 6d65 223a 2022 4261 6e6a 6172   "name": "Banjar
+00000100: 6573 6522 2c0a 2020 2020 2273 6f75 7263  ese",.    "sourc
+00000110: 655f 7375 6273 6574 223a 2022 626a 6e22  e_subset": "bjn"
+00000120: 0a20 207d 2c0a 2020 2262 7567 223a 207b  .  },.  "bug": {
+00000130: 0a20 2020 2022 6e61 6d65 223a 2022 4275  .    "name": "Bu
+00000140: 6769 6e65 7365 222c 0a20 2020 2022 736f  ginese",.    "so
+00000150: 7572 6365 5f73 7562 7365 7422 3a20 2262  urce_subset": "b
+00000160: 7567 220a 2020 7d2c 0a20 2022 6362 6b22  ug".  },.  "cbk"
+00000170: 3a20 7b0a 2020 2020 226e 616d 6522 3a20  : {.    "name": 
+00000180: 2243 6861 7661 6361 6e6f 222c 0a20 2020  "Chavacano",.   
+00000190: 2022 736f 7572 6365 5f73 7562 7365 7422   "source_subset"
+000001a0: 3a20 2263 626b 2d7a 616d 220a 2020 7d2c  : "cbk-zam".  },
+000001b0: 0a20 2022 676f 7222 3a20 7b0a 2020 2020  .  "gor": {.    
+000001c0: 226e 616d 6522 3a20 2247 6f72 6f6e 7461  "name": "Goronta
+000001d0: 6c6f 222c 0a20 2020 2022 736f 7572 6365  lo",.    "source
+000001e0: 5f73 7562 7365 7422 3a20 2267 6f72 220a  _subset": "gor".
+000001f0: 2020 7d2c 0a20 2022 696c 6f22 3a20 7b0a    },.  "ilo": {.
+00000200: 2020 2020 226e 616d 6522 3a20 2249 6c6f      "name": "Ilo
+00000210: 6b61 6e6f 222c 0a20 2020 2022 736f 7572  kano",.    "sour
+00000220: 6365 5f73 7562 7365 7422 3a20 2269 6c6f  ce_subset": "ilo
+00000230: 220a 2020 7d2c 0a20 2022 696e 6422 3a20  ".  },.  "ind": 
+00000240: 7b0a 2020 2020 226e 616d 6522 3a20 2249  {.    "name": "I
+00000250: 6e64 6f6e 6573 6961 6e22 2c0a 2020 2020  ndonesian",.    
+00000260: 2273 6f75 7263 655f 7375 6273 6574 223a  "source_subset":
+00000270: 2022 6964 220a 2020 7d2c 0a20 2022 6a61   "id".  },.  "ja
+00000280: 7622 3a20 7b0a 2020 2020 226e 616d 6522  v": {.    "name"
+00000290: 3a20 224a 6176 616e 6573 6522 2c0a 2020  : "Javanese",.  
+000002a0: 2020 2273 6f75 7263 655f 7375 6273 6574    "source_subset
+000002b0: 223a 2022 6a76 220a 2020 7d2c 0a20 2022  ": "jv".  },.  "
+000002c0: 6b68 6d22 3a20 7b0a 2020 2020 226e 616d  khm": {.    "nam
+000002d0: 6522 3a20 224b 686d 6572 222c 0a20 2020  e": "Khmer",.   
+000002e0: 2022 736f 7572 6365 5f73 7562 7365 7422   "source_subset"
+000002f0: 3a20 226b 6d22 0a20 207d 2c0a 2020 226c  : "km".  },.  "l
+00000300: 616f 223a 207b 0a20 2020 2022 6e61 6d65  ao": {.    "name
+00000310: 223a 2022 4c61 6f22 2c0a 2020 2020 2273  ": "Lao",.    "s
+00000320: 6f75 7263 655f 7375 6273 6574 223a 2022  ource_subset": "
+00000330: 6c6f 220a 2020 7d2c 0a20 2022 6d61 6422  lo".  },.  "mad"
+00000340: 3a20 7b0a 2020 2020 226e 616d 6522 3a20  : {.    "name": 
+00000350: 224d 6164 7572 6573 6522 2c0a 2020 2020  "Madurese",.    
+00000360: 2273 6f75 7263 655f 7375 6273 6574 223a  "source_subset":
+00000370: 2022 6d61 6422 0a20 207d 2c0a 2020 226d   "mad".  },.  "m
+00000380: 6170 5f62 6d73 223a 207b 0a20 2020 2022  ap_bms": {.    "
+00000390: 6e61 6d65 223a 2022 4261 6e79 756d 6173  name": "Banyumas
+000003a0: 616e 2028 4469 616c 6563 7420 6f66 204a  an (Dialect of J
+000003b0: 6176 616e 6573 6529 222c 0a20 2020 2022  avanese)",.    "
+000003c0: 736f 7572 6365 5f73 7562 7365 7422 3a20  source_subset": 
+000003d0: 226d 6170 2d62 6d73 220a 2020 7d2c 0a20  "map-bms".  },. 
+000003e0: 2022 6d69 6e22 3a20 7b0a 2020 2020 226e   "min": {.    "n
+000003f0: 616d 6522 3a20 224d 696e 616e 676b 6162  ame": "Minangkab
+00000400: 6175 222c 0a20 2020 2022 736f 7572 6365  au",.    "source
+00000410: 5f73 7562 7365 7422 3a20 226d 696e 220a  _subset": "min".
+00000420: 2020 7d2c 0a20 2022 6d6e 7722 3a20 7b0a    },.  "mnw": {.
+00000430: 2020 2020 226e 616d 6522 3a20 224d 6f6e      "name": "Mon
+00000440: 222c 0a20 2020 2022 736f 7572 6365 5f73  ",.    "source_s
+00000450: 7562 7365 7422 3a20 226d 696e 220a 2020  ubset": "min".  
+00000460: 7d2c 0a20 2022 6d79 6122 3a20 7b0a 2020  },.  "mya": {.  
+00000470: 2020 226e 616d 6522 3a20 2242 7572 6d65    "name": "Burme
+00000480: 7365 222c 0a20 2020 2022 736f 7572 6365  se",.    "source
+00000490: 5f73 7562 7365 7422 3a20 226d 7922 0a20  _subset": "my". 
+000004a0: 207d 2c0a 2020 226e 6961 223a 207b 0a20   },.  "nia": {. 
+000004b0: 2020 2022 6e61 6d65 223a 2022 4e69 6173     "name": "Nias
+000004c0: 222c 0a20 2020 2022 736f 7572 6365 5f73  ",.    "source_s
+000004d0: 7562 7365 7422 3a20 226e 6961 220a 2020  ubset": "nia".  
+000004e0: 7d2c 0a20 2022 7061 6722 3a20 7b0a 2020  },.  "pag": {.  
+000004f0: 2020 226e 616d 6522 3a20 2250 616e 6761    "name": "Panga
+00000500: 7369 6e61 6e22 2c0a 2020 2020 2273 6f75  sinan",.    "sou
+00000510: 7263 655f 7375 6273 6574 223a 2022 7061  rce_subset": "pa
+00000520: 6722 0a20 207d 2c0a 2020 2270 616d 223a  g".  },.  "pam":
+00000530: 207b 0a20 2020 2022 6e61 6d65 223a 2022   {.    "name": "
+00000540: 4b61 7061 6d70 616e 6761 6e22 2c0a 2020  Kapampangan",.  
+00000550: 2020 2273 6f75 7263 655f 7375 6273 6574    "source_subset
+00000560: 223a 2022 7061 6d22 0a20 207d 2c0a 2020  ": "pam".  },.  
+00000570: 2273 686e 223a 207b 0a20 2020 2022 6e61  "shn": {.    "na
+00000580: 6d65 223a 2022 5368 616e 222c 0a20 2020  me": "Shan",.   
+00000590: 2022 736f 7572 6365 5f73 7562 7365 7422   "source_subset"
+000005a0: 3a20 2273 686e 220a 2020 7d2c 0a20 2022  : "shn".  },.  "
+000005b0: 7375 6e22 3a20 7b0a 2020 2020 226e 616d  sun": {.    "nam
+000005c0: 6522 3a20 2253 756e 6461 6e65 7365 222c  e": "Sundanese",
+000005d0: 0a20 2020 2022 736f 7572 6365 5f73 7562  .    "source_sub
+000005e0: 7365 7422 3a20 2273 7522 0a20 207d 2c0a  set": "su".  },.
+000005f0: 2020 2274 6574 223a 207b 0a20 2020 2022    "tet": {.    "
+00000600: 6e61 6d65 223a 2022 5465 7475 6d22 2c0a  name": "Tetum",.
+00000610: 2020 2020 2273 6f75 7263 655f 7375 6273      "source_subs
+00000620: 6574 223a 2022 7465 7422 0a20 207d 2c0a  et": "tet".  },.
+00000630: 2020 2274 676c 223a 207b 0a20 2020 2022    "tgl": {.    "
+00000640: 6e61 6d65 223a 2022 5461 6761 6c6f 6722  name": "Tagalog"
+00000650: 2c0a 2020 2020 2273 6f75 7263 655f 7375  ,.    "source_su
+00000660: 6273 6574 223a 2022 746c 220a 2020 7d2c  bset": "tl".  },
+00000670: 0a20 2022 7468 6122 3a20 7b0a 2020 2020  .  "tha": {.    
+00000680: 226e 616d 6522 3a20 2254 6861 6922 2c0a  "name": "Thai",.
+00000690: 2020 2020 2273 6f75 7263 655f 7375 6273      "source_subs
+000006a0: 6574 223a 2022 7468 220a 2020 7d2c 0a20  et": "th".  },. 
+000006b0: 2022 7669 6522 3a20 7b0a 2020 2020 226e   "vie": {.    "n
+000006c0: 616d 6522 3a20 2256 6965 746e 616d 6573  ame": "Vietnames
+000006d0: 6522 2c0a 2020 2020 2273 6f75 7263 655f  e",.    "source_
+000006e0: 7375 6273 6574 223a 2022 7669 220a 2020  subset": "vi".  
+000006f0: 7d2c 0a20 2022 7761 7222 3a20 7b0a 2020  },.  "war": {.  
+00000700: 2020 226e 616d 6522 3a20 2257 6172 6179    "name": "Waray
+00000710: 222c 0a20 2020 2022 736f 7572 6365 5f73  ",.    "source_s
+00000720: 7562 7365 7422 3a20 2277 6172 220a 2020  ubset": "war".  
+00000730: 7d0a 7d0a                                }.}.
```

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/sea_wiki/sea_wiki.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/sea_wiki/sea_wiki.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from itertools import product
 from typing import Dict, List, Tuple
 
 import datasets
 from datasets import load_dataset
 from datasets.download.download_manager import DownloadManager
 
+from seacrowd.sea_datasets.sea_wiki.lang_config import _LANG_CONFIG
 from seacrowd.utils import schemas
 from seacrowd.utils.configs import SEACrowdConfig
 from seacrowd.utils.constants import Licenses, Tasks
 
 _CITATION = """
 @ONLINE{wikidump,
     author = "Wikimedia Foundation",
@@ -25,18 +26,14 @@
 @ONLINE{wikipedia-hf,
     title  = "Huggingface SEA Wikipedia Dataset",
     url    = "https://huggingface.co/datasets/sabilmakbar/sea_wiki"}
 """
 
 logger = datasets.logging.get_logger(__name__)
 
-
-with open(DownloadManager().download_and_extract("seacrowd/sea_datasets/sea_wiki/lang_config.json"), "r") as f:
-    _LANG_CONFIG = json.load(f)
-
 _LOCAL = False
 _LANGUAGES = list(_LANG_CONFIG.keys())
 
 _DATASETNAME = "sea_wiki"
 _DESCRIPTION = """\
     SEA Lang & Local Langs Wikipedia Archives, dumped from WIkipedia HF and processed by boilerplate removal.
     This dataset consists of URL of referred Wikipedia Article, its Title, and its Text Data (Article Contents).
```

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/seaeval/seaeval.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/seaeval/seaeval.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/seahorse/seahorse.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/seahorse/seahorse.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/sentiment_nathasa_review/sentiment_nathasa_review.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/sentiment_nathasa_review/sentiment_nathasa_review.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/shopee_reviews_tagalog/shopee_reviews_tagalog.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/shopee_reviews_tagalog/shopee_reviews_tagalog.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/singgalang/singgalang.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/singgalang/singgalang.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/smsa/smsa.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/smsa/smsa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/snli_indo/snli_indo.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/snli_indo/snli_indo.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/spamid_pair/spamid_pair.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/spamid_pair/spamid_pair.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/squad_id/squad_id.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/squad_id/squad_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/stb_ext/stb_ext.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/stb_ext/stb_ext.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/stif_indonesia/stif_indonesia.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/stif_indonesia/stif_indonesia.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/struct_amb_ind/struct_amb_ind.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/struct_amb_ind/struct_amb_ind.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/su_emot/su_emot.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/su_emot/su_emot.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/su_id_asr/su_id_asr.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/su_id_asr/su_id_asr.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/su_id_tts/su_id_tts.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/su_id_tts/su_id_tts.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/talpco/talpco.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/talpco/talpco.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/tatabahasa/tatabahasa.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/tatabahasa/tatabahasa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/tatoeba/tatoeba.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/tatoeba/tatoeba.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/tcope/tcope.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/tcope/tcope.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/ted_en_id/ted_en_id.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/ted_en_id/ted_en_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/term_a/term_a.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/term_a/term_a.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/tgl_profanity/tgl_profanity.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/tgl_profanity/tgl_profanity.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/tha_lao_embassy_parcor/tha_lao_embassy_parcor.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/tha_lao_embassy_parcor/tha_lao_embassy_parcor.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/thai_alpaca/thai_alpaca.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/thai_alpaca/thai_alpaca.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/thai_constitution/thai_constitution.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/thai_constitution/thai_constitution.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/thai_databricks_dolly/thai_databricks_dolly.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/thai_databricks_dolly/thai_databricks_dolly.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/thai_depression/thai_depression.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/thai_depression/thai_depression.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/thai_gpteacher/thai_gpteacher.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/thai_gpteacher/thai_gpteacher.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/thai_hh_rlhf/thai_hh_rlhf.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/thai_hh_rlhf/thai_hh_rlhf.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/thai_sum/thai_sum.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/thai_sum/thai_sum.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/thai_toxicity_tweet/thai_toxicity_tweet.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/thai_toxicity_tweet/thai_toxicity_tweet.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/tico_19/tico_19.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/tico_19/tico_19.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/titml_idn/titml_idn.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/titml_idn/titml_idn.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/tlunified_ner/tlunified_ner.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/tlunified_ner/tlunified_ner.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/toxicity_200/toxicity_200.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/toxicity_200/toxicity_200.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/tydiqa/tydiqa.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/tydiqa/tydiqa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/typhoon_yolanda_tweets/typhoon_yolanda_tweets.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/typhoon_yolanda_tweets/typhoon_yolanda_tweets.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/ucla_phonetic/ucla_phonetic.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/ucla_phonetic/ucla_phonetic.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/ud_id_csui/ud_id_csui.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/ud_id_csui/ud_id_csui.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/ud_jv_csui/ud_jv_csui.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/ud_jv_csui/ud_jv_csui.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/udhr/udhr.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/udhr/udhr.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/udhr_lid/udhr_lid.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/udhr_lid/udhr_lid.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/uit_vicov19qa/uit_vicov19qa.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/uit_vicov19qa/uit_vicov19qa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/uit_victsd/uit_victsd.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/uit_victsd/uit_victsd.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/uit_vihsd/uit_vihsd.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/uit_vihsd/uit_vihsd.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/uit_viic/uit_viic.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/uit_viic/uit_viic.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/uit_viocd/uit_viocd.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/uit_viocd/uit_viocd.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/uit_vion/uit_vion.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/uit_vion/uit_vion.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/uit_visd4sa/uit_visd4sa.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/uit_visd4sa/uit_visd4sa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/uit_vsfc/uit_vsfc.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/uit_vsfc/uit_vsfc.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/uit_vsmec/uit_vsmec.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/uit_vsmec/uit_vsmec.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/unimorph/unimorph.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/unimorph/unimorph.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/unimorph_id/unimorph_id.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/unimorph_id/unimorph_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/vi_pubmed/vi_pubmed.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/vi_pubmed/vi_pubmed.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/vihealthqa/vihealthqa.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/vihealthqa/vihealthqa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/visobert/visobert.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/visobert/visobert.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/vispamreviews/vispamreviews.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/vispamreviews/vispamreviews.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/vistec_tp_th_21/vistec_tp_th_21.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/vistec_tp_th_21/vistec_tp_th_21.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/vitext2sql/vitext2sql.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/vitext2sql/vitext2sql.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/vivos/vivos.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/vivos/vivos.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/vivqa/vivqa.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/vivqa/vivqa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/vlsp2016_ner/vlsp2016_ner.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/vlsp2016_ner/vlsp2016_ner.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/vlsp2016_sa/vlsp2016_sa.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/vlsp2016_sa/vlsp2016_sa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/vndt/utils.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/vndt/utils.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/vndt/vndt.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/vndt/vndt.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/voxlingua/voxlingua.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/voxlingua/voxlingua.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/weathub/weathub.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/weathub/weathub.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/wikiann/wikiann.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/wikiann/wikiann.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/wikilingua/wikilingua.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/wikilingua/wikilingua.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/wikimatrix/wikimatrix.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/wikimatrix/wikimatrix.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/wikitext_tl_39/wikitext_tl_39.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/wikitext_tl_39/wikitext_tl_39.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/wili_2018/wili_2018.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/wili_2018/wili_2018.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/wisesight_thai_sentiment/wisesight_thai_sentiment.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/wisesight_thai_sentiment/wisesight_thai_sentiment.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/wit/wit.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/wit/wit.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/wongnai_reviews/wongnai_reviews.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/wongnai_reviews/wongnai_reviews.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/wrete/wrete.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/wrete/wrete.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/x_fact/x_fact.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/x_fact/x_fact.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/xcopa/xcopa.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/xcopa/xcopa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/xl_jailbreak/xl_jailbreak.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/xl_jailbreak/xl_jailbreak.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/xl_sum/xl_sum.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/xl_sum/xl_sum.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/xm3600/xm3600.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/xm3600/xm3600.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/xnli/xnli.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/xnli/xnli.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/xpersona_id/xpersona_id.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/xpersona_id/xpersona_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/xquad/xquad.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/xquad/xquad.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/xsid/xsid.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/xsid/xsid.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/xstorycloze/xstorycloze.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/xstorycloze/xstorycloze.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/sea_datasets/yunshan_cup_2020/yunshan_cup_2020.py` & `seacrowd-0.0.7/seacrowd/sea_datasets/yunshan_cup_2020/yunshan_cup_2020.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/utils/common_parser.py` & `seacrowd-0.0.7/seacrowd/utils/common_parser.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/utils/constants.py` & `seacrowd-0.0.7/seacrowd/utils/constants.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/utils/schemas/__init__.py` & `seacrowd-0.0.7/seacrowd/utils/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/utils/schemas/imqa.py` & `seacrowd-0.0.7/seacrowd/utils/schemas/imqa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/utils/schemas/kb.py` & `seacrowd-0.0.7/seacrowd/utils/schemas/kb.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/utils/schemas/pairs.py` & `seacrowd-0.0.7/seacrowd/utils/schemas/pairs.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/utils/schemas/qa.py` & `seacrowd-0.0.7/seacrowd/utils/schemas/qa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/utils/schemas/seq_label.py` & `seacrowd-0.0.7/seacrowd/utils/schemas/seq_label.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/utils/schemas/speech.py` & `seacrowd-0.0.7/seacrowd/utils/schemas/speech.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/utils/schemas/speech_multilabel.py` & `seacrowd-0.0.7/seacrowd/utils/schemas/speech_multilabel.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/utils/schemas/speech_to_speech.py` & `seacrowd-0.0.7/seacrowd/utils/schemas/speech_to_speech.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/utils/schemas/tod.py` & `seacrowd-0.0.7/seacrowd/utils/schemas/tod.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/utils/schemas/tree.py` & `seacrowd-0.0.7/seacrowd/utils/schemas/tree.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd/utils/schemas/video.py` & `seacrowd-0.0.7/seacrowd/utils/schemas/video.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/seacrowd.egg-info/PKG-INFO` & `seacrowd-0.0.7/seacrowd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seacrowd
-Version: 0.0.6
+Version: 0.0.7
 Requires-Python: >=3.7
 License-File: LICENSE
 Requires-Dist: loguru>=0.5.3
 Requires-Dist: bioc>=1.3.7
 Requires-Dist: pandas>=1.3.3
 Requires-Dist: numpy>=1.20
 Requires-Dist: datasets>=2.2.0
```

### Comparing `seacrowd-0.0.6/seacrowd.egg-info/SOURCES.txt` & `seacrowd-0.0.7/seacrowd.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
 seacrowd/sea_datasets/filipino_slang_norm/filipino_slang_norm.py
 seacrowd/sea_datasets/filipino_words_aoa/__init__.py
 seacrowd/sea_datasets/filipino_words_aoa/filipino_words_aoa.py
 seacrowd/sea_datasets/filwordnet/__init__.py
 seacrowd/sea_datasets/filwordnet/filwordnet.py
 seacrowd/sea_datasets/fleurs/__init__.py
 seacrowd/sea_datasets/fleurs/fleurs.py
-seacrowd/sea_datasets/fleurs/lang_config.json
+seacrowd/sea_datasets/fleurs/lang_config.py
 seacrowd/sea_datasets/flores200/__init__.py
 seacrowd/sea_datasets/flores200/flores200.py
 seacrowd/sea_datasets/fsl_105/__init__.py
 seacrowd/sea_datasets/fsl_105/fsl_105.py
 seacrowd/sea_datasets/gatitos/__init__.py
 seacrowd/sea_datasets/gatitos/gatitos.py
 seacrowd/sea_datasets/gklmip_newsclass/__init__.py
@@ -455,15 +455,15 @@
 seacrowd/sea_datasets/scb_mt_en_th/__init__.py
 seacrowd/sea_datasets/scb_mt_en_th/scb_mt_en_th.py
 seacrowd/sea_datasets/sea_bench/__init__.py
 seacrowd/sea_datasets/sea_bench/sea_bench.py
 seacrowd/sea_datasets/sea_madlad/__init__.py
 seacrowd/sea_datasets/sea_madlad/sea_madlad.py
 seacrowd/sea_datasets/sea_wiki/__init__.py
-seacrowd/sea_datasets/sea_wiki/lang_config.json
+seacrowd/sea_datasets/sea_wiki/lang_config.py
 seacrowd/sea_datasets/sea_wiki/sea_wiki.py
 seacrowd/sea_datasets/seaeval/__init__.py
 seacrowd/sea_datasets/seaeval/seaeval.py
 seacrowd/sea_datasets/seahorse/__init__.py
 seacrowd/sea_datasets/seahorse/seahorse.py
 seacrowd/sea_datasets/sentiment_nathasa_review/__init__.py
 seacrowd/sea_datasets/sentiment_nathasa_review/sentiment_nathasa_review.py
```

### Comparing `seacrowd-0.0.6/setup.cfg` & `seacrowd-0.0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/tests/test_seacrowd.py` & `seacrowd-0.0.7/tests/test_seacrowd.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.6/tests/test_seacrowd_source_only.py` & `seacrowd-0.0.7/tests/test_seacrowd_source_only.py`

 * *Files identical despite different names*

