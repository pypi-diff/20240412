# Comparing `tmp/seacrowd-0.0.5.tar.gz` & `tmp/seacrowd-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seacrowd-0.0.5.tar", last modified: Thu Apr 11 09:12:48 2024, max compression
+gzip compressed data, was "seacrowd-0.0.6.tar", last modified: Fri Apr 12 07:28:54 2024, max compression
```

## Comparing `seacrowd-0.0.5.tar` & `seacrowd-0.0.6.tar`

### file list

```diff
@@ -1,980 +1,982 @@
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:48.364587 seacrowd-0.0.5/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    11357 2024-04-04 06:00:44.000000 seacrowd-0.0.5/LICENSE
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1071 2024-04-11 09:12:48.361183 seacrowd-0.0.5/PKG-INFO
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5757 2024-04-04 06:00:44.000000 seacrowd-0.0.5/README.md
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:41.265476 seacrowd-0.0.5/seacrowd/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      251 2024-04-11 09:12:29.000000 seacrowd-0.0.5/seacrowd/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    40451 2024-04-11 08:39:41.000000 seacrowd-0.0.5/seacrowd/config_helper.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:41.323493 seacrowd-0.0.5/seacrowd/sea_datasets/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/__init__.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:41.338290 seacrowd-0.0.5/seacrowd/sea_datasets/abui_wordnet/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/abui_wordnet/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5277 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/abui_wordnet/abui_wordnet.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:41.355470 seacrowd-0.0.5/seacrowd/sea_datasets/alt_burmese_treebank/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/alt_burmese_treebank/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5692 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/alt_burmese_treebank/alt_burmese_treebank.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:41.370467 seacrowd-0.0.5/seacrowd/sea_datasets/alt_burmese_treebank/utils/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/alt_burmese_treebank/utils/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     2661 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/alt_burmese_treebank/utils/alt_burmese_treebank_utils.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:41.387390 seacrowd-0.0.5/seacrowd/sea_datasets/ara_close/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/ara_close/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8227 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/ara_close/ara_close.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:41.408290 seacrowd-0.0.5/seacrowd/sea_datasets/asr_sindodusc/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/asr_sindodusc/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7231 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/asr_sindodusc/asr_sindodusc.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:41.424436 seacrowd-0.0.5/seacrowd/sea_datasets/asr_smaldusc/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/asr_smaldusc/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7305 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/asr_smaldusc/asr_smaldusc.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:41.441900 seacrowd-0.0.5/seacrowd/sea_datasets/asr_stidusc/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/asr_stidusc/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6979 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/asr_stidusc/asr_stidusc.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:41.458838 seacrowd-0.0.5/seacrowd/sea_datasets/audio_keyword_spotting/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/audio_keyword_spotting/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7860 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/audio_keyword_spotting/audio_keyword_spotting.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:41.477965 seacrowd-0.0.5/seacrowd/sea_datasets/aya_dataset/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/aya_dataset/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7482 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/aya_dataset/aya_dataset.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:41.505816 seacrowd-0.0.5/seacrowd/sea_datasets/barasa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/barasa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7224 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/barasa/barasa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:41.527447 seacrowd-0.0.5/seacrowd/sea_datasets/beaye_lexicon/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/beaye_lexicon/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4357 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/beaye_lexicon/beaye_lexicon.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:41.544374 seacrowd-0.0.5/seacrowd/sea_datasets/belebele/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/belebele/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8610 2024-04-11 08:39:41.000000 seacrowd-0.0.5/seacrowd/sea_datasets/belebele/belebele.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:41.560953 seacrowd-0.0.5/seacrowd/sea_datasets/bible_en_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/bible_en_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6790 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/bible_en_id/bible_en_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:41.580094 seacrowd-0.0.5/seacrowd/sea_datasets/bible_jv_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/bible_jv_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6856 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/bible_jv_id/bible_jv_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:41.596192 seacrowd-0.0.5/seacrowd/sea_datasets/bible_su_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/bible_su_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6632 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/bible_su_id/bible_su_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:41.615966 seacrowd-0.0.5/seacrowd/sea_datasets/bioner_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/bioner_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6108 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/bioner_id/bioner_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:41.634170 seacrowd-0.0.5/seacrowd/sea_datasets/bloom_captioning/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/bloom_captioning/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8518 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/bloom_captioning/bloom_captioning.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:41.650056 seacrowd-0.0.5/seacrowd/sea_datasets/bloom_lm/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/bloom_lm/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8430 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/bloom_lm/bloom_lm.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:41.667307 seacrowd-0.0.5/seacrowd/sea_datasets/bloom_speech/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/bloom_speech/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6922 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/bloom_speech/bloom_speech.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:41.682242 seacrowd-0.0.5/seacrowd/sea_datasets/bloom_vist/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/bloom_vist/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9674 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/bloom_vist/bloom_vist.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:41.698780 seacrowd-0.0.5/seacrowd/sea_datasets/burapha_th/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/burapha_th/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6995 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/burapha_th/burapha_th.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:41.715310 seacrowd-0.0.5/seacrowd/sea_datasets/burmese_romanize/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/burmese_romanize/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4420 2024-04-11 08:39:41.000000 seacrowd-0.0.5/seacrowd/sea_datasets/burmese_romanize/burmese_romanize.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:41.731423 seacrowd-0.0.5/seacrowd/sea_datasets/casa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/casa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5635 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/casa/casa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:41.750016 seacrowd-0.0.5/seacrowd/sea_datasets/cc100/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/cc100/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10941 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/cc100/cc100.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:41.774654 seacrowd-0.0.5/seacrowd/sea_datasets/cc_aligned_doc/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/cc_aligned_doc/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6230 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/cc_aligned_doc/cc_aligned_doc.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:41.797919 seacrowd-0.0.5/seacrowd/sea_datasets/cc_aligned_sent/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/cc_aligned_sent/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6256 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/cc_aligned_sent/cc_aligned_sent.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:41.814922 seacrowd-0.0.5/seacrowd/sea_datasets/cebuaner/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/cebuaner/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7783 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/cebuaner/cebuaner.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:41.831611 seacrowd-0.0.5/seacrowd/sea_datasets/coco_35l/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/coco_35l/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9830 2024-04-11 08:39:41.000000 seacrowd-0.0.5/seacrowd/sea_datasets/coco_35l/coco_35l.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:41.849654 seacrowd-0.0.5/seacrowd/sea_datasets/cod/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/cod/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6239 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/cod/cod.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:41.870306 seacrowd-0.0.5/seacrowd/sea_datasets/code_mixed_jv_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/code_mixed_jv_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8760 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/code_mixed_jv_id/code_mixed_jv_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:41.888091 seacrowd-0.0.5/seacrowd/sea_datasets/codeswitch_reddit/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/codeswitch_reddit/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9015 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/codeswitch_reddit/codeswitch_reddit.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:41.904928 seacrowd-0.0.5/seacrowd/sea_datasets/commonvoice_120/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/commonvoice_120/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9438 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/commonvoice_120/commonvoice_120.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:41.922490 seacrowd-0.0.5/seacrowd/sea_datasets/copal/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/copal/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5868 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/copal/copal.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:41.940034 seacrowd-0.0.5/seacrowd/sea_datasets/covost2/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/covost2/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10329 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/covost2/covost2.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:41.965779 seacrowd-0.0.5/seacrowd/sea_datasets/creole_rc/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.5/seacrowd/sea_datasets/creole_rc/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9448 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/creole_rc/creole_rc.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:41.980663 seacrowd-0.0.5/seacrowd/sea_datasets/crosssum/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/crosssum/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5467 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/crosssum/crosssum.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:41.997061 seacrowd-0.0.5/seacrowd/sea_datasets/cub_bahasa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/cub_bahasa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    14495 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/cub_bahasa/cub_bahasa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:42.014395 seacrowd-0.0.5/seacrowd/sea_datasets/culturax/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/culturax/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6383 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/culturax/culturax.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:42.032613 seacrowd-0.0.5/seacrowd/sea_datasets/cvss/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/cvss/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    11054 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/cvss/cvss.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:42.049003 seacrowd-0.0.5/seacrowd/sea_datasets/dengue_filipino/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/dengue_filipino/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4777 2024-04-11 08:39:41.000000 seacrowd-0.0.5/seacrowd/sea_datasets/dengue_filipino/dengue_filipino.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:42.078003 seacrowd-0.0.5/seacrowd/sea_datasets/emot/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/emot/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5522 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/emot/emot.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:42.098997 seacrowd-0.0.5/seacrowd/sea_datasets/emotcmt/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/emotcmt/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4484 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/emotcmt/emotcmt.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:42.114888 seacrowd-0.0.5/seacrowd/sea_datasets/emotes_3k/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/emotes_3k/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9257 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/emotes_3k/emotes_3k.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:42.133190 seacrowd-0.0.5/seacrowd/sea_datasets/emotion_id_opinion/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/emotion_id_opinion/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7315 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/emotion_id_opinion/emotion_id_opinion.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:42.161370 seacrowd-0.0.5/seacrowd/sea_datasets/etos/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/etos/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7041 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/etos/etos.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:42.178740 seacrowd-0.0.5/seacrowd/sea_datasets/facqa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/facqa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5788 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/facqa/facqa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:42.225610 seacrowd-0.0.5/seacrowd/sea_datasets/facqa/utils/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/facqa/utils/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      815 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/facqa/utils/facqa_utils.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:42.244812 seacrowd-0.0.5/seacrowd/sea_datasets/fakenews_ph/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/fakenews_ph/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4936 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/fakenews_ph/fakenews_ph.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:42.259142 seacrowd-0.0.5/seacrowd/sea_datasets/filipino_gay_lang/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/filipino_gay_lang/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4808 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/filipino_gay_lang/filipino_gay_lang.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:42.273398 seacrowd-0.0.5/seacrowd/sea_datasets/filipino_hatespeech_tiktok/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/filipino_hatespeech_tiktok/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4697 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/filipino_hatespeech_tiktok/filipino_hatespeech_tiktok.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:42.288964 seacrowd-0.0.5/seacrowd/sea_datasets/filipino_slang_norm/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/filipino_slang_norm/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4967 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/filipino_slang_norm/filipino_slang_norm.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:42.324870 seacrowd-0.0.5/seacrowd/sea_datasets/filipino_words_aoa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/filipino_words_aoa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4965 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/filipino_words_aoa/filipino_words_aoa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:42.341535 seacrowd-0.0.5/seacrowd/sea_datasets/filwordnet/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/filwordnet/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4819 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/filwordnet/filwordnet.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:42.357593 seacrowd-0.0.5/seacrowd/sea_datasets/fleurs/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/fleurs/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    13248 2024-04-11 09:11:07.000000 seacrowd-0.0.5/seacrowd/sea_datasets/fleurs/fleurs.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:42.376157 seacrowd-0.0.5/seacrowd/sea_datasets/flores200/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/flores200/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    13920 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/flores200/flores200.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:42.394869 seacrowd-0.0.5/seacrowd/sea_datasets/fsl_105/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/fsl_105/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6753 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/fsl_105/fsl_105.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:42.415342 seacrowd-0.0.5/seacrowd/sea_datasets/gatitos/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/gatitos/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6624 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/gatitos/gatitos.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:42.443427 seacrowd-0.0.5/seacrowd/sea_datasets/gklmip_newsclass/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/gklmip_newsclass/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6024 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/gklmip_newsclass/gklmip_newsclass.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:42.461057 seacrowd-0.0.5/seacrowd/sea_datasets/gklmip_sentiment/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/gklmip_sentiment/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5007 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/gklmip_sentiment/gklmip_sentiment.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:42.478224 seacrowd-0.0.5/seacrowd/sea_datasets/globalwoz/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/globalwoz/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10031 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/globalwoz/globalwoz.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:42.500905 seacrowd-0.0.5/seacrowd/sea_datasets/glotstorybook/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/glotstorybook/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5878 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/glotstorybook/glotstorybook.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:42.519581 seacrowd-0.0.5/seacrowd/sea_datasets/hoasa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/hoasa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6301 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/hoasa/hoasa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:42.548647 seacrowd-0.0.5/seacrowd/sea_datasets/iapp_squad/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/iapp_squad/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5420 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/iapp_squad/iapp_squad.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:42.567726 seacrowd-0.0.5/seacrowd/sea_datasets/iatf/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/iatf/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5801 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/iatf/iatf.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:42.582686 seacrowd-0.0.5/seacrowd/sea_datasets/icon/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/icon/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8351 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/icon/icon.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:42.601482 seacrowd-0.0.5/seacrowd/sea_datasets/id_abusive/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/id_abusive/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6540 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/id_abusive/id_abusive.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:42.628103 seacrowd-0.0.5/seacrowd/sea_datasets/id_abusive_news_comment/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/id_abusive_news_comment/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4293 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/id_abusive_news_comment/id_abusive_news_comment.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:42.652060 seacrowd-0.0.5/seacrowd/sea_datasets/id_am2ico/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/id_am2ico/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7430 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/id_am2ico/id_am2ico.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:42.669405 seacrowd-0.0.5/seacrowd/sea_datasets/id_clickbait/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/id_clickbait/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5770 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/id_clickbait/id_clickbait.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:42.686701 seacrowd-0.0.5/seacrowd/sea_datasets/id_coreference_resolution/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/id_coreference_resolution/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7576 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/id_coreference_resolution/id_coreference_resolution.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:42.721719 seacrowd-0.0.5/seacrowd/sea_datasets/id_frog_story/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/id_frog_story/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4524 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/id_frog_story/id_frog_story.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:42.752260 seacrowd-0.0.5/seacrowd/sea_datasets/id_google_play_review/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/id_google_play_review/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6144 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/id_google_play_review/id_google_play_review.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:42.769139 seacrowd-0.0.5/seacrowd/sea_datasets/id_hatespeech/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/id_hatespeech/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4450 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/id_hatespeech/id_hatespeech.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:42.785689 seacrowd-0.0.5/seacrowd/sea_datasets/id_hoax_news/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/id_hoax_news/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4555 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/id_hoax_news/id_hoax_news.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:42.803162 seacrowd-0.0.5/seacrowd/sea_datasets/id_hsd_nofaaulia/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/id_hsd_nofaaulia/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7252 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/id_hsd_nofaaulia/id_hsd_nofaaulia.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:42.847669 seacrowd-0.0.5/seacrowd/sea_datasets/id_msvd/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/id_msvd/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5051 2024-04-11 08:39:41.000000 seacrowd-0.0.5/seacrowd/sea_datasets/id_msvd/id_msvd.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:42.862929 seacrowd-0.0.5/seacrowd/sea_datasets/id_multilabel_hs/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/id_multilabel_hs/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6021 2024-04-04 06:00:46.000000 seacrowd-0.0.5/seacrowd/sea_datasets/id_multilabel_hs/id_multilabel_hs.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:42.878773 seacrowd-0.0.5/seacrowd/sea_datasets/id_panl_bppt/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/id_panl_bppt/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5616 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/id_panl_bppt/id_panl_bppt.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:42.894654 seacrowd-0.0.5/seacrowd/sea_datasets/id_qqp/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/id_qqp/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4686 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/id_qqp/id_qqp.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:42.912088 seacrowd-0.0.5/seacrowd/sea_datasets/id_sent_emo_mobile_apps/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/id_sent_emo_mobile_apps/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5395 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/id_sent_emo_mobile_apps/id_sent_emo_mobile_apps.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:42.936315 seacrowd-0.0.5/seacrowd/sea_datasets/id_sentiment_analysis/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/id_sentiment_analysis/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5538 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/id_sentiment_analysis/id_sentiment_analysis.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:42.956326 seacrowd-0.0.5/seacrowd/sea_datasets/id_short_answer_grading/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/id_short_answer_grading/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9107 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/id_short_answer_grading/id_short_answer_grading.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:42.971169 seacrowd-0.0.5/seacrowd/sea_datasets/id_short_answer_grading/utils/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/id_short_answer_grading/utils/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1826 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/id_short_answer_grading/utils/id_short_answer_grading_utils.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:42.990672 seacrowd-0.0.5/seacrowd/sea_datasets/id_stance/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/id_stance/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5114 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/id_stance/id_stance.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:43.010481 seacrowd-0.0.5/seacrowd/sea_datasets/id_sts/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/id_sts/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4308 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/id_sts/id_sts.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:43.029963 seacrowd-0.0.5/seacrowd/sea_datasets/id_vaccines_tweets/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/id_vaccines_tweets/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4329 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/id_vaccines_tweets/id_vaccines_tweets.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:43.046870 seacrowd-0.0.5/seacrowd/sea_datasets/id_wiki_parallel/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/id_wiki_parallel/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6697 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/id_wiki_parallel/id_wiki_parallel.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:43.064316 seacrowd-0.0.5/seacrowd/sea_datasets/id_wsd/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/id_wsd/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6404 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/id_wsd/id_wsd.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:43.090279 seacrowd-0.0.5/seacrowd/sea_datasets/identic/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/identic/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    13357 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/identic/identic.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:43.124390 seacrowd-0.0.5/seacrowd/sea_datasets/identifikasi_bahasa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/identifikasi_bahasa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5177 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/identifikasi_bahasa/identifikasi_bahasa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:43.153862 seacrowd-0.0.5/seacrowd/sea_datasets/idk_mrc/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/idk_mrc/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9530 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/idk_mrc/idk_mrc.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:43.182420 seacrowd-0.0.5/seacrowd/sea_datasets/idn_tagged_corpus_csui/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/idn_tagged_corpus_csui/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6193 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/idn_tagged_corpus_csui/idn_tagged_corpus_csui.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:43.204978 seacrowd-0.0.5/seacrowd/sea_datasets/ijelid/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/ijelid/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5403 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/ijelid/ijelid.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:43.239978 seacrowd-0.0.5/seacrowd/sea_datasets/imdb_jv/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/imdb_jv/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4894 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/imdb_jv/imdb_jv.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:43.256924 seacrowd-0.0.5/seacrowd/sea_datasets/indo4b/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indo4b/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7236 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indo4b/indo4b.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:43.276222 seacrowd-0.0.5/seacrowd/sea_datasets/indo4b_plus/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indo4b_plus/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7417 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indo4b_plus/indo4b_plus.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:43.291085 seacrowd-0.0.5/seacrowd/sea_datasets/indo_general_mt_en_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indo_general_mt_en_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6442 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indo_general_mt_en_id/indo_general_mt_en_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:43.341524 seacrowd-0.0.5/seacrowd/sea_datasets/indo_law/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indo_law/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5445 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indo_law/indo_law.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:43.371376 seacrowd-0.0.5/seacrowd/sea_datasets/indo_puisi/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indo_puisi/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4018 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indo_puisi/indo_puisi.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:43.391635 seacrowd-0.0.5/seacrowd/sea_datasets/indo_religious_mt_en_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indo_religious_mt_en_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8507 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indo_religious_mt_en_id/indo_religious_mt_en_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:43.444342 seacrowd-0.0.5/seacrowd/sea_datasets/indo_story_cloze/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indo_story_cloze/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6563 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indo_story_cloze/indo_story_cloze.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:43.464943 seacrowd-0.0.5/seacrowd/sea_datasets/indocamrest/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indocamrest/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6670 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indocamrest/indocamrest.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:43.482676 seacrowd-0.0.5/seacrowd/sea_datasets/indocollex/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indocollex/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6949 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indocollex/indocollex.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:43.517596 seacrowd-0.0.5/seacrowd/sea_datasets/indocoref/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indocoref/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    11610 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indocoref/indocoref.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:43.568942 seacrowd-0.0.5/seacrowd/sea_datasets/indocoref/utils/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indocoref/utils/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9072 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indocoref/utils/feature_utils.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     2091 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indocoref/utils/file_utils.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4307 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indocoref/utils/text_preprocess.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:43.591429 seacrowd-0.0.5/seacrowd/sea_datasets/indolem_ner_ugm/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indolem_ner_ugm/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6402 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indolem_ner_ugm/indolem_ner_ugm.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:43.612558 seacrowd-0.0.5/seacrowd/sea_datasets/indolem_nerui/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indolem_nerui/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8192 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indolem_nerui/indolem_nerui.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:43.651489 seacrowd-0.0.5/seacrowd/sea_datasets/indolem_ntp/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indolem_ntp/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5885 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indolem_ntp/indolem_ntp.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:43.679755 seacrowd-0.0.5/seacrowd/sea_datasets/indolem_sentiment/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indolem_sentiment/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    12679 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indolem_sentiment/indolem_sentiment.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:43.697717 seacrowd-0.0.5/seacrowd/sea_datasets/indolem_tweet_ordering/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indolem_tweet_ordering/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    12454 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indolem_tweet_ordering/indolem_tweet_ordering.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:43.732512 seacrowd-0.0.5/seacrowd/sea_datasets/indolem_ud_id_gsd/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indolem_ud_id_gsd/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8462 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indolem_ud_id_gsd/indolem_ud_id_gsd.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:43.745777 seacrowd-0.0.5/seacrowd/sea_datasets/indolem_ud_id_pud/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indolem_ud_id_pud/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8825 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indolem_ud_id_pud/indolem_ud_id_pud.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:43.760677 seacrowd-0.0.5/seacrowd/sea_datasets/indoler/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indoler/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9100 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indoler/indoler.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:43.776903 seacrowd-0.0.5/seacrowd/sea_datasets/indommlu/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indommlu/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10934 2024-04-11 08:39:41.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indommlu/indommlu.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:43.794282 seacrowd-0.0.5/seacrowd/sea_datasets/indoner_tourism/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indoner_tourism/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8394 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indoner_tourism/indoner_tourism.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:43.828949 seacrowd-0.0.5/seacrowd/sea_datasets/indonesia_chinese_mtrobusteval/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indonesia_chinese_mtrobusteval/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5250 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indonesia_chinese_mtrobusteval/indonesia_chinese_mtrobusteval.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:43.855211 seacrowd-0.0.5/seacrowd/sea_datasets/indonesian_madurese_bible_translation/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indonesian_madurese_bible_translation/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7932 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indonesian_madurese_bible_translation/indonesian_madurese_bible_translation.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:43.872404 seacrowd-0.0.5/seacrowd/sea_datasets/indonesian_news_dataset/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indonesian_news_dataset/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4581 2024-04-11 08:39:41.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indonesian_news_dataset/indonesian_news_dataset.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:43.890659 seacrowd-0.0.5/seacrowd/sea_datasets/indonesiannmt/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indonesiannmt/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9148 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indonesiannmt/indonesiannmt.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:43.921271 seacrowd-0.0.5/seacrowd/sea_datasets/indonglish/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indonglish/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8339 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indonglish/indonglish.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:43.953975 seacrowd-0.0.5/seacrowd/sea_datasets/indonli/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indonli/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8050 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indonli/indonli.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:43.970751 seacrowd-0.0.5/seacrowd/sea_datasets/indonlu_nergrit/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indonlu_nergrit/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5677 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indonlu_nergrit/indonlu_nergrit.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:43.987832 seacrowd-0.0.5/seacrowd/sea_datasets/indoqa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indoqa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5422 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indoqa/indoqa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:44.029019 seacrowd-0.0.5/seacrowd/sea_datasets/indosmd/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indosmd/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    13550 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indosmd/indosmd.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:44.046696 seacrowd-0.0.5/seacrowd/sea_datasets/indosum/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indosum/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6872 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indosum/indosum.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:44.065218 seacrowd-0.0.5/seacrowd/sea_datasets/indotacos/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indotacos/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5477 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indotacos/indotacos.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:44.083351 seacrowd-0.0.5/seacrowd/sea_datasets/indowiki/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indowiki/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7684 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indowiki/indowiki.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:44.098935 seacrowd-0.0.5/seacrowd/sea_datasets/indqner/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        1 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indqner/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6614 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indqner/indqner.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:44.133093 seacrowd-0.0.5/seacrowd/sea_datasets/indspeech_digit_cdsr/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indspeech_digit_cdsr/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9856 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indspeech_digit_cdsr/indspeech_digit_cdsr.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:44.150009 seacrowd-0.0.5/seacrowd/sea_datasets/indspeech_news_ethnicsr/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indspeech_news_ethnicsr/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8440 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indspeech_news_ethnicsr/indspeech_news_ethnicsr.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:44.165925 seacrowd-0.0.5/seacrowd/sea_datasets/indspeech_news_lvcsr/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indspeech_news_lvcsr/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9432 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indspeech_news_lvcsr/indspeech_news_lvcsr.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:44.184276 seacrowd-0.0.5/seacrowd/sea_datasets/indspeech_news_tts/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indspeech_news_tts/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8857 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indspeech_news_tts/indspeech_news_tts.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:44.207064 seacrowd-0.0.5/seacrowd/sea_datasets/indspeech_newstra_ethnicsr/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indspeech_newstra_ethnicsr/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    11615 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indspeech_newstra_ethnicsr/indspeech_newstra_ethnicsr.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:44.249962 seacrowd-0.0.5/seacrowd/sea_datasets/indspeech_teldialog_lvcsr/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indspeech_teldialog_lvcsr/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9932 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indspeech_teldialog_lvcsr/indspeech_teldialog_lvcsr.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:44.266885 seacrowd-0.0.5/seacrowd/sea_datasets/indspeech_teldialog_svcsr/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indspeech_teldialog_svcsr/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9818 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/indspeech_teldialog_svcsr/indspeech_teldialog_svcsr.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:44.284245 seacrowd-0.0.5/seacrowd/sea_datasets/inset_lexicon/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/inset_lexicon/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4829 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/inset_lexicon/inset_lexicon.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:44.300371 seacrowd-0.0.5/seacrowd/sea_datasets/jadi_ide/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/jadi_ide/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4404 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/jadi_ide/jadi_ide.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:44.316375 seacrowd-0.0.5/seacrowd/sea_datasets/jv_id_asr/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/jv_id_asr/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6236 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/jv_id_asr/jv_id_asr.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:44.340399 seacrowd-0.0.5/seacrowd/sea_datasets/jv_id_tts/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/jv_id_tts/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7628 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/jv_id_tts/jv_id_tts.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:44.360810 seacrowd-0.0.5/seacrowd/sea_datasets/kamus_alay/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/kamus_alay/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5286 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/kamus_alay/kamus_alay.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:44.376018 seacrowd-0.0.5/seacrowd/sea_datasets/karonese_sentiment/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/karonese_sentiment/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4533 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/karonese_sentiment/karonese_sentiment.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:44.393202 seacrowd-0.0.5/seacrowd/sea_datasets/kawat/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/kawat/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5933 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/kawat/kawat.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:44.438764 seacrowd-0.0.5/seacrowd/sea_datasets/kde4/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/kde4/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    14408 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/kde4/kde4.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:44.457298 seacrowd-0.0.5/seacrowd/sea_datasets/keps/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/keps/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5066 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/keps/keps.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:44.470502 seacrowd-0.0.5/seacrowd/sea_datasets/kheng_info/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/kheng_info/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3687 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/kheng_info/kheng_info.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:44.486605 seacrowd-0.0.5/seacrowd/sea_datasets/khmer_alt_pos/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/khmer_alt_pos/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7442 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/khmer_alt_pos/khmer_alt_pos.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:44.516143 seacrowd-0.0.5/seacrowd/sea_datasets/khpos/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/khpos/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8756 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/khpos/khpos.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:44.534069 seacrowd-0.0.5/seacrowd/sea_datasets/kopi_cc/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/kopi_cc/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10035 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/kopi_cc/kopi_cc.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:44.550724 seacrowd-0.0.5/seacrowd/sea_datasets/kopi_cc_news/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/kopi_cc_news/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5088 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/kopi_cc_news/kopi_cc_news.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:44.568982 seacrowd-0.0.5/seacrowd/sea_datasets/kopi_nllb/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/kopi_nllb/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5956 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/kopi_nllb/kopi_nllb.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:44.585879 seacrowd-0.0.5/seacrowd/sea_datasets/korpus_nusantara/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/korpus_nusantara/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8476 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/korpus_nusantara/korpus_nusantara.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:44.610010 seacrowd-0.0.5/seacrowd/sea_datasets/lazada_review_filipino/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/lazada_review_filipino/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4913 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/lazada_review_filipino/lazada_review_filipino.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:44.626942 seacrowd-0.0.5/seacrowd/sea_datasets/librivox_indonesia/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/librivox_indonesia/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8736 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/librivox_indonesia/librivox_indonesia.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:44.646576 seacrowd-0.0.5/seacrowd/sea_datasets/limesoda/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/limesoda/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6775 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/limesoda/limesoda.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:44.663290 seacrowd-0.0.5/seacrowd/sea_datasets/liputan6/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/liputan6/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7512 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/liputan6/liputan6.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:44.680730 seacrowd-0.0.5/seacrowd/sea_datasets/local_id_abusive/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/local_id_abusive/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7530 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/local_id_abusive/local_id_abusive.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:44.698074 seacrowd-0.0.5/seacrowd/sea_datasets/lr_sum/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/lr_sum/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6160 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/lr_sum/lr_sum.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:44.727550 seacrowd-0.0.5/seacrowd/sea_datasets/m3exam/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/m3exam/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    14637 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/m3exam/m3exam.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:44.754970 seacrowd-0.0.5/seacrowd/sea_datasets/mabl/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/mabl/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8609 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/mabl/mabl.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:44.769477 seacrowd-0.0.5/seacrowd/sea_datasets/malaysia_tweets/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/malaysia_tweets/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6432 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/malaysia_tweets/malaysia_tweets.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:44.785826 seacrowd-0.0.5/seacrowd/sea_datasets/malindo_morph/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/malindo_morph/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4617 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/malindo_morph/malindo_morph.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:44.801122 seacrowd-0.0.5/seacrowd/sea_datasets/malindo_parallel/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/malindo_parallel/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6494 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/malindo_parallel/malindo_parallel.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:44.820613 seacrowd-0.0.5/seacrowd/sea_datasets/massive/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/massive/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    18420 2024-04-04 06:00:48.000000 seacrowd-0.0.5/seacrowd/sea_datasets/massive/massive.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:44.852298 seacrowd-0.0.5/seacrowd/sea_datasets/mc4_indo/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/mc4_indo/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5510 2024-04-11 08:39:41.000000 seacrowd-0.0.5/seacrowd/sea_datasets/mc4_indo/mc4_indo.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:44.868267 seacrowd-0.0.5/seacrowd/sea_datasets/melayu_brunei/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/melayu_brunei/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10682 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/melayu_brunei/melayu_brunei.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:44.885827 seacrowd-0.0.5/seacrowd/sea_datasets/melayu_sabah/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/melayu_sabah/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5561 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/melayu_sabah/melayu_sabah.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:44.915928 seacrowd-0.0.5/seacrowd/sea_datasets/melayu_sarawak/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/melayu_sarawak/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6559 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/melayu_sarawak/melayu_sarawak.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:44.949896 seacrowd-0.0.5/seacrowd/sea_datasets/melayu_standard_lisan/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/melayu_standard_lisan/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7594 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/melayu_standard_lisan/melayu_standard_lisan.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:44.965878 seacrowd-0.0.5/seacrowd/sea_datasets/memolon/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/memolon/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5589 2024-04-11 08:39:41.000000 seacrowd-0.0.5/seacrowd/sea_datasets/memolon/memolon.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:44.981294 seacrowd-0.0.5/seacrowd/sea_datasets/minangnlp_mt/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/minangnlp_mt/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6874 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/minangnlp_mt/minangnlp_mt.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:44.997438 seacrowd-0.0.5/seacrowd/sea_datasets/miracl/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/miracl/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    13119 2024-04-11 08:39:41.000000 seacrowd-0.0.5/seacrowd/sea_datasets/miracl/miracl.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:45.018716 seacrowd-0.0.5/seacrowd/sea_datasets/mkqa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/mkqa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8345 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/mkqa/mkqa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:45.057198 seacrowd-0.0.5/seacrowd/sea_datasets/mlqa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        1 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/mlqa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9825 2024-04-11 08:39:41.000000 seacrowd-0.0.5/seacrowd/sea_datasets/mlqa/mlqa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:45.073896 seacrowd-0.0.5/seacrowd/sea_datasets/mozilla_pontoon/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/mozilla_pontoon/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6211 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/mozilla_pontoon/mozilla_pontoon.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:45.089183 seacrowd-0.0.5/seacrowd/sea_datasets/mswc/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/mswc/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8048 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/mswc/mswc.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:45.122683 seacrowd-0.0.5/seacrowd/sea_datasets/mtop_intent_classification/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/mtop_intent_classification/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     2654 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/mtop_intent_classification/labels.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5662 2024-04-11 08:39:41.000000 seacrowd-0.0.5/seacrowd/sea_datasets/mtop_intent_classification/mtop_intent_classification.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:45.140119 seacrowd-0.0.5/seacrowd/sea_datasets/multilexnorm/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/multilexnorm/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6223 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/multilexnorm/multilexnorm.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:45.168150 seacrowd-0.0.5/seacrowd/sea_datasets/my_paraphrase/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/my_paraphrase/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8124 2024-04-11 08:39:41.000000 seacrowd-0.0.5/seacrowd/sea_datasets/my_paraphrase/my_paraphrase.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:45.184224 seacrowd-0.0.5/seacrowd/sea_datasets/myanmar_rakhine_parallel/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/myanmar_rakhine_parallel/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7223 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/myanmar_rakhine_parallel/myanmar_rakhine_parallel.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:45.223874 seacrowd-0.0.5/seacrowd/sea_datasets/mypos/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/mypos/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5116 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/mypos/mypos.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:45.246495 seacrowd-0.0.5/seacrowd/sea_datasets/mysentence/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/mysentence/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7612 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/mysentence/mysentence.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:45.264791 seacrowd-0.0.5/seacrowd/sea_datasets/myxnli/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/myxnli/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5096 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/myxnli/myxnli.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:45.281372 seacrowd-0.0.5/seacrowd/sea_datasets/nergrit/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/nergrit/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6322 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/nergrit/nergrit.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:45.305779 seacrowd-0.0.5/seacrowd/sea_datasets/nerp/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/nerp/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4852 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/nerp/nerp.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:45.325772 seacrowd-0.0.5/seacrowd/sea_datasets/netifier/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/netifier/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4838 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/netifier/netifier.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:45.355069 seacrowd-0.0.5/seacrowd/sea_datasets/news_en_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/news_en_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5003 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/news_en_id/news_en_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:45.371355 seacrowd-0.0.5/seacrowd/sea_datasets/newsph/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/newsph/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3810 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/newsph/newsph.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:45.388132 seacrowd-0.0.5/seacrowd/sea_datasets/nllb_seed/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/nllb_seed/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    15208 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/nllb_seed/nllb_seed.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:45.411112 seacrowd-0.0.5/seacrowd/sea_datasets/ntrex_128/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/ntrex_128/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10971 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/ntrex_128/ntrex_128.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:45.454171 seacrowd-0.0.5/seacrowd/sea_datasets/nusaparagraph_emot/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/nusaparagraph_emot/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8785 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/nusaparagraph_emot/nusaparagraph_emot.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:45.473713 seacrowd-0.0.5/seacrowd/sea_datasets/nusaparagraph_rhetoric/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/nusaparagraph_rhetoric/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8792 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/nusaparagraph_rhetoric/nusaparagraph_rhetoric.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:45.491301 seacrowd-0.0.5/seacrowd/sea_datasets/nusaparagraph_topic/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/nusaparagraph_topic/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8845 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/nusaparagraph_topic/nusaparagraph_topic.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:45.512762 seacrowd-0.0.5/seacrowd/sea_datasets/nusatranslation_emot/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/nusatranslation_emot/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8233 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/nusatranslation_emot/nusatranslation_emot.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:45.556420 seacrowd-0.0.5/seacrowd/sea_datasets/nusatranslation_mt/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/nusatranslation_mt/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9156 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/nusatranslation_mt/nusatranslation_mt.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:45.573456 seacrowd-0.0.5/seacrowd/sea_datasets/nusatranslation_senti/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/nusatranslation_senti/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8285 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/nusatranslation_senti/nusatranslation_senti.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:45.592540 seacrowd-0.0.5/seacrowd/sea_datasets/nusax_mt/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/nusax_mt/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7578 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/nusax_mt/nusax_mt.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:45.631930 seacrowd-0.0.5/seacrowd/sea_datasets/nusax_senti/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/nusax_senti/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7250 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/nusax_senti/nusax_senti.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:45.654267 seacrowd-0.0.5/seacrowd/sea_datasets/oil/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/oil/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5477 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/oil/oil.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:45.671092 seacrowd-0.0.5/seacrowd/sea_datasets/ojw/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/ojw/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5110 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/ojw/ojw.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:45.688162 seacrowd-0.0.5/seacrowd/sea_datasets/openlid/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/openlid/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7915 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/openlid/openlid.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:45.727396 seacrowd-0.0.5/seacrowd/sea_datasets/openslr/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/openslr/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10343 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/openslr/openslr.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:45.745676 seacrowd-0.0.5/seacrowd/sea_datasets/orchid_pos/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/orchid_pos/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9625 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/orchid_pos/orchid_pos.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:45.762806 seacrowd-0.0.5/seacrowd/sea_datasets/oscar_2201/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/oscar_2201/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    16270 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/oscar_2201/oscar_2201.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:45.779922 seacrowd-0.0.5/seacrowd/sea_datasets/palito/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/palito/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5930 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/palito/palito.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:45.795361 seacrowd-0.0.5/seacrowd/sea_datasets/paracotta_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/paracotta_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4768 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/paracotta_id/paracotta_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:45.820088 seacrowd-0.0.5/seacrowd/sea_datasets/parallel_id_nyo/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/parallel_id_nyo/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5471 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/parallel_id_nyo/parallel_id_nyo.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:45.839763 seacrowd-0.0.5/seacrowd/sea_datasets/parallel_su_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/parallel_su_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4782 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/parallel_su_id/parallel_su_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:45.853240 seacrowd-0.0.5/seacrowd/sea_datasets/ph_fake_news_corpus/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/ph_fake_news_corpus/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4339 2024-04-11 08:39:41.000000 seacrowd-0.0.5/seacrowd/sea_datasets/ph_fake_news_corpus/ph_fake_news_corpus.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:45.870383 seacrowd-0.0.5/seacrowd/sea_datasets/pho_ner_covid/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/pho_ner_covid/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6866 2024-04-04 06:00:49.000000 seacrowd-0.0.5/seacrowd/sea_datasets/pho_ner_covid/pho_ner_covid.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:45.888138 seacrowd-0.0.5/seacrowd/sea_datasets/phomt/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/phomt/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5141 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/phomt/phomt.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:45.904835 seacrowd-0.0.5/seacrowd/sea_datasets/phost/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/phost/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9498 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/phost/phost.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:45.926052 seacrowd-0.0.5/seacrowd/sea_datasets/posp/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/posp/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5990 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/posp/posp.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:45.962830 seacrowd-0.0.5/seacrowd/sea_datasets/postag_su/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/postag_su/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8033 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/postag_su/postag_su.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:45.982170 seacrowd-0.0.5/seacrowd/sea_datasets/prdect_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/prdect_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7572 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/prdect_id/prdect_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:45.999575 seacrowd-0.0.5/seacrowd/sea_datasets/qasina/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/qasina/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6424 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/qasina/qasina.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:46.020064 seacrowd-0.0.5/seacrowd/sea_datasets/roots_vi_ted/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/roots_vi_ted/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5065 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/roots_vi_ted/roots_vi_ted.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:46.045901 seacrowd-0.0.5/seacrowd/sea_datasets/sampiran/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/sampiran/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5024 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/sampiran/sampiran.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:46.062377 seacrowd-0.0.5/seacrowd/sea_datasets/sap_wat/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/sap_wat/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7077 2024-04-11 08:39:41.000000 seacrowd-0.0.5/seacrowd/sea_datasets/sap_wat/sap_wat.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:46.079439 seacrowd-0.0.5/seacrowd/sea_datasets/sarawak_malay/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/sarawak_malay/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7381 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/sarawak_malay/sarawak_malay.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:46.095755 seacrowd-0.0.5/seacrowd/sea_datasets/scb_mt_en_th/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/scb_mt_en_th/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7071 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/scb_mt_en_th/scb_mt_en_th.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:46.116223 seacrowd-0.0.5/seacrowd/sea_datasets/sea_bench/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/sea_bench/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7206 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/sea_bench/sea_bench.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:46.144314 seacrowd-0.0.5/seacrowd/sea_datasets/sea_madlad/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/sea_madlad/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10051 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/sea_madlad/sea_madlad.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:46.162432 seacrowd-0.0.5/seacrowd/sea_datasets/sea_wiki/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/sea_wiki/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9350 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/sea_wiki/sea_wiki.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:46.177016 seacrowd-0.0.5/seacrowd/sea_datasets/seaeval/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/seaeval/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9350 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/seaeval/seaeval.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:46.194166 seacrowd-0.0.5/seacrowd/sea_datasets/seahorse/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/seahorse/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6884 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/seahorse/seahorse.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:46.250221 seacrowd-0.0.5/seacrowd/sea_datasets/sentiment_nathasa_review/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/sentiment_nathasa_review/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6002 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/sentiment_nathasa_review/sentiment_nathasa_review.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:46.267316 seacrowd-0.0.5/seacrowd/sea_datasets/shopee_reviews_tagalog/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/shopee_reviews_tagalog/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4597 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/shopee_reviews_tagalog/shopee_reviews_tagalog.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:46.284961 seacrowd-0.0.5/seacrowd/sea_datasets/singgalang/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/singgalang/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5430 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/singgalang/singgalang.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:46.306958 seacrowd-0.0.5/seacrowd/sea_datasets/smsa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/smsa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5575 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/smsa/smsa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:46.352159 seacrowd-0.0.5/seacrowd/sea_datasets/snli_indo/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/snli_indo/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6244 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/snli_indo/snli_indo.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:46.370181 seacrowd-0.0.5/seacrowd/sea_datasets/spamid_pair/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/spamid_pair/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5524 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/spamid_pair/spamid_pair.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:46.386675 seacrowd-0.0.5/seacrowd/sea_datasets/squad_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/squad_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5315 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/squad_id/squad_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:46.401913 seacrowd-0.0.5/seacrowd/sea_datasets/stb_ext/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/stb_ext/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9273 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/stb_ext/stb_ext.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:46.429701 seacrowd-0.0.5/seacrowd/sea_datasets/stif_indonesia/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/stif_indonesia/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5135 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/stif_indonesia/stif_indonesia.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:46.450059 seacrowd-0.0.5/seacrowd/sea_datasets/struct_amb_ind/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/struct_amb_ind/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7724 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/struct_amb_ind/struct_amb_ind.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:46.467422 seacrowd-0.0.5/seacrowd/sea_datasets/su_emot/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/su_emot/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4567 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/su_emot/su_emot.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:46.485482 seacrowd-0.0.5/seacrowd/sea_datasets/su_id_asr/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/su_id_asr/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5601 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/su_id_asr/su_id_asr.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:46.506649 seacrowd-0.0.5/seacrowd/sea_datasets/su_id_tts/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/su_id_tts/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7636 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/su_id_tts/su_id_tts.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:46.528046 seacrowd-0.0.5/seacrowd/sea_datasets/talpco/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/talpco/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6870 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/talpco/talpco.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:46.545478 seacrowd-0.0.5/seacrowd/sea_datasets/tatabahasa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/tatabahasa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5411 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/tatabahasa/tatabahasa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:46.569596 seacrowd-0.0.5/seacrowd/sea_datasets/tatoeba/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/tatoeba/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7636 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/tatoeba/tatoeba.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:46.588189 seacrowd-0.0.5/seacrowd/sea_datasets/tcope/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/tcope/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6693 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/tcope/tcope.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:46.627938 seacrowd-0.0.5/seacrowd/sea_datasets/ted_en_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/ted_en_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7105 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/ted_en_id/ted_en_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:46.650042 seacrowd-0.0.5/seacrowd/sea_datasets/term_a/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/term_a/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5358 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/term_a/term_a.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:46.666901 seacrowd-0.0.5/seacrowd/sea_datasets/tgl_profanity/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/tgl_profanity/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4351 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/tgl_profanity/tgl_profanity.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:46.684865 seacrowd-0.0.5/seacrowd/sea_datasets/tha_lao_embassy_parcor/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/tha_lao_embassy_parcor/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4436 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/tha_lao_embassy_parcor/tha_lao_embassy_parcor.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:46.701882 seacrowd-0.0.5/seacrowd/sea_datasets/thai_alpaca/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/thai_alpaca/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3943 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/thai_alpaca/thai_alpaca.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:46.719563 seacrowd-0.0.5/seacrowd/sea_datasets/thai_constitution/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/thai_constitution/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10954 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/thai_constitution/thai_constitution.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:46.752632 seacrowd-0.0.5/seacrowd/sea_datasets/thai_databricks_dolly/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/thai_databricks_dolly/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4388 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/thai_databricks_dolly/thai_databricks_dolly.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:46.783672 seacrowd-0.0.5/seacrowd/sea_datasets/thai_depression/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/thai_depression/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5739 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/thai_depression/thai_depression.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:46.802838 seacrowd-0.0.5/seacrowd/sea_datasets/thai_gpteacher/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/thai_gpteacher/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3960 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/thai_gpteacher/thai_gpteacher.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:46.825968 seacrowd-0.0.5/seacrowd/sea_datasets/thai_hh_rlhf/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/thai_hh_rlhf/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5077 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/thai_hh_rlhf/thai_hh_rlhf.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:46.841385 seacrowd-0.0.5/seacrowd/sea_datasets/thai_sum/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/thai_sum/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5683 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/thai_sum/thai_sum.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:46.863083 seacrowd-0.0.5/seacrowd/sea_datasets/thai_toxicity_tweet/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/thai_toxicity_tweet/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4555 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/thai_toxicity_tweet/thai_toxicity_tweet.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:46.878759 seacrowd-0.0.5/seacrowd/sea_datasets/tico_19/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/tico_19/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    12192 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/tico_19/tico_19.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:46.893785 seacrowd-0.0.5/seacrowd/sea_datasets/titml_idn/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/titml_idn/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5900 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/titml_idn/titml_idn.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:46.909595 seacrowd-0.0.5/seacrowd/sea_datasets/tlunified_ner/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.5/seacrowd/sea_datasets/tlunified_ner/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5800 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/tlunified_ner/tlunified_ner.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:46.939201 seacrowd-0.0.5/seacrowd/sea_datasets/toxicity_200/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/toxicity_200/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5975 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/toxicity_200/toxicity_200.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:46.955118 seacrowd-0.0.5/seacrowd/sea_datasets/tydiqa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/tydiqa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    23881 2024-04-11 08:39:41.000000 seacrowd-0.0.5/seacrowd/sea_datasets/tydiqa/tydiqa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:46.974754 seacrowd-0.0.5/seacrowd/sea_datasets/typhoon_yolanda_tweets/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        1 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/typhoon_yolanda_tweets/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5165 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/typhoon_yolanda_tweets/typhoon_yolanda_tweets.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:46.992374 seacrowd-0.0.5/seacrowd/sea_datasets/ucla_phonetic/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/ucla_phonetic/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6531 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/ucla_phonetic/ucla_phonetic.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:47.022111 seacrowd-0.0.5/seacrowd/sea_datasets/ud_id_csui/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/ud_id_csui/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9185 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/ud_id_csui/ud_id_csui.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:47.052562 seacrowd-0.0.5/seacrowd/sea_datasets/ud_jv_csui/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/ud_jv_csui/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10052 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/ud_jv_csui/ud_jv_csui.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:47.073515 seacrowd-0.0.5/seacrowd/sea_datasets/udhr/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/udhr/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6030 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/udhr/udhr.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:47.089357 seacrowd-0.0.5/seacrowd/sea_datasets/udhr_lid/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/udhr_lid/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5190 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/udhr_lid/udhr_lid.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:47.134384 seacrowd-0.0.5/seacrowd/sea_datasets/uit_vicov19qa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/uit_vicov19qa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7244 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/uit_vicov19qa/uit_vicov19qa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:47.149241 seacrowd-0.0.5/seacrowd/sea_datasets/uit_victsd/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/uit_victsd/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5311 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/uit_victsd/uit_victsd.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:47.165473 seacrowd-0.0.5/seacrowd/sea_datasets/uit_vihsd/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/uit_vihsd/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5721 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/uit_vihsd/uit_vihsd.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:47.181172 seacrowd-0.0.5/seacrowd/sea_datasets/uit_viic/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/uit_viic/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6572 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/uit_viic/uit_viic.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:47.198429 seacrowd-0.0.5/seacrowd/sea_datasets/uit_viocd/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/uit_viocd/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4819 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/uit_viocd/uit_viocd.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:47.215127 seacrowd-0.0.5/seacrowd/sea_datasets/uit_vion/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/uit_vion/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5939 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/uit_vion/uit_vion.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:47.240313 seacrowd-0.0.5/seacrowd/sea_datasets/uit_visd4sa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/uit_visd4sa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7034 2024-04-11 08:39:41.000000 seacrowd-0.0.5/seacrowd/sea_datasets/uit_visd4sa/uit_visd4sa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:47.263624 seacrowd-0.0.5/seacrowd/sea_datasets/uit_vsfc/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/uit_vsfc/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8715 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/uit_vsfc/uit_vsfc.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:47.280973 seacrowd-0.0.5/seacrowd/sea_datasets/uit_vsmec/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/uit_vsmec/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4802 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/uit_vsmec/uit_vsmec.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:47.298213 seacrowd-0.0.5/seacrowd/sea_datasets/unimorph/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/unimorph/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    15492 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/unimorph/unimorph.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:47.314717 seacrowd-0.0.5/seacrowd/sea_datasets/unimorph_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/unimorph_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7445 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/unimorph_id/unimorph_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:47.335399 seacrowd-0.0.5/seacrowd/sea_datasets/vi_pubmed/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/vi_pubmed/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    15136 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/vi_pubmed/vi_pubmed.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:47.353185 seacrowd-0.0.5/seacrowd/sea_datasets/vihealthqa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/vihealthqa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5587 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/vihealthqa/vihealthqa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:47.371629 seacrowd-0.0.5/seacrowd/sea_datasets/visobert/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/visobert/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6265 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/visobert/visobert.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:47.390766 seacrowd-0.0.5/seacrowd/sea_datasets/vispamreviews/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/vispamreviews/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7245 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/vispamreviews/vispamreviews.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:47.409263 seacrowd-0.0.5/seacrowd/sea_datasets/vistec_tp_th_21/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/vistec_tp_th_21/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6739 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/vistec_tp_th_21/vistec_tp_th_21.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:47.426397 seacrowd-0.0.5/seacrowd/sea_datasets/vitext2sql/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/vitext2sql/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6893 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/vitext2sql/vitext2sql.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:47.446148 seacrowd-0.0.5/seacrowd/sea_datasets/vivos/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/vivos/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7832 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/vivos/vivos.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:47.466785 seacrowd-0.0.5/seacrowd/sea_datasets/vivqa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/vivqa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9080 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/vivqa/vivqa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:47.486721 seacrowd-0.0.5/seacrowd/sea_datasets/vlsp2016_ner/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/vlsp2016_ner/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5857 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/vlsp2016_ner/vlsp2016_ner.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:47.503050 seacrowd-0.0.5/seacrowd/sea_datasets/vlsp2016_sa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/vlsp2016_sa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7134 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/vlsp2016_sa/vlsp2016_sa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:47.526470 seacrowd-0.0.5/seacrowd/sea_datasets/vndt/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/vndt/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     2232 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/vndt/utils.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7852 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/vndt/vndt.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:47.540344 seacrowd-0.0.5/seacrowd/sea_datasets/voxlingua/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/voxlingua/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7980 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/voxlingua/voxlingua.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:47.557771 seacrowd-0.0.5/seacrowd/sea_datasets/weathub/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/weathub/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7521 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/weathub/weathub.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:47.573022 seacrowd-0.0.5/seacrowd/sea_datasets/wikiann/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/wikiann/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8643 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/wikiann/wikiann.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:47.590144 seacrowd-0.0.5/seacrowd/sea_datasets/wikilingua/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/wikilingua/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4984 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/wikilingua/wikilingua.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:47.607337 seacrowd-0.0.5/seacrowd/sea_datasets/wikimatrix/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/wikimatrix/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8585 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/wikimatrix/wikimatrix.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:47.625696 seacrowd-0.0.5/seacrowd/sea_datasets/wikitext_tl_39/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/wikitext_tl_39/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3663 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/wikitext_tl_39/wikitext_tl_39.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:47.670337 seacrowd-0.0.5/seacrowd/sea_datasets/wili_2018/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/wili_2018/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6699 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/wili_2018/wili_2018.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:47.697109 seacrowd-0.0.5/seacrowd/sea_datasets/wisesight_thai_sentiment/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/wisesight_thai_sentiment/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7027 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/wisesight_thai_sentiment/wisesight_thai_sentiment.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:47.713511 seacrowd-0.0.5/seacrowd/sea_datasets/wit/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/wit/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    12057 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/wit/wit.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:47.729076 seacrowd-0.0.5/seacrowd/sea_datasets/wongnai_reviews/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/wongnai_reviews/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4106 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/wongnai_reviews/wongnai_reviews.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:47.755037 seacrowd-0.0.5/seacrowd/sea_datasets/wrete/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/wrete/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6113 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/wrete/wrete.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:47.768880 seacrowd-0.0.5/seacrowd/sea_datasets/x_fact/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/x_fact/__init__.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:47.784607 seacrowd-0.0.5/seacrowd/sea_datasets/x_fact/utils/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/x_fact/utils/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      473 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/x_fact/utils/x_fact_utils.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5900 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/x_fact/x_fact.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:47.800650 seacrowd-0.0.5/seacrowd/sea_datasets/xcopa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/xcopa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7024 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/xcopa/xcopa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:47.818002 seacrowd-0.0.5/seacrowd/sea_datasets/xl_jailbreak/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/xl_jailbreak/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6317 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/xl_jailbreak/xl_jailbreak.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:47.840762 seacrowd-0.0.5/seacrowd/sea_datasets/xl_sum/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/xl_sum/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6903 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/xl_sum/xl_sum.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:47.856984 seacrowd-0.0.5/seacrowd/sea_datasets/xm3600/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/xm3600/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8233 2024-04-11 08:39:41.000000 seacrowd-0.0.5/seacrowd/sea_datasets/xm3600/xm3600.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:47.873306 seacrowd-0.0.5/seacrowd/sea_datasets/xnli/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/xnli/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8333 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/xnli/xnli.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:47.889909 seacrowd-0.0.5/seacrowd/sea_datasets/xpersona_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/xpersona_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6550 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/xpersona_id/xpersona_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:47.912109 seacrowd-0.0.5/seacrowd/sea_datasets/xquad/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/xquad/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4819 2024-04-04 06:00:51.000000 seacrowd-0.0.5/seacrowd/sea_datasets/xquad/xquad.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:47.934238 seacrowd-0.0.5/seacrowd/sea_datasets/xsid/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:52.000000 seacrowd-0.0.5/seacrowd/sea_datasets/xsid/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9510 2024-04-04 06:00:52.000000 seacrowd-0.0.5/seacrowd/sea_datasets/xsid/xsid.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:47.957131 seacrowd-0.0.5/seacrowd/sea_datasets/xstorycloze/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:52.000000 seacrowd-0.0.5/seacrowd/sea_datasets/xstorycloze/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6794 2024-04-04 06:00:52.000000 seacrowd-0.0.5/seacrowd/sea_datasets/xstorycloze/xstorycloze.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:47.993892 seacrowd-0.0.5/seacrowd/sea_datasets/yunshan_cup_2020/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:52.000000 seacrowd-0.0.5/seacrowd/sea_datasets/yunshan_cup_2020/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5828 2024-04-04 06:00:52.000000 seacrowd-0.0.5/seacrowd/sea_datasets/yunshan_cup_2020/yunshan_cup_2020.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:48.058231 seacrowd-0.0.5/seacrowd/utils/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:52.000000 seacrowd-0.0.5/seacrowd/utils/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5493 2024-04-04 06:00:52.000000 seacrowd-0.0.5/seacrowd/utils/common_parser.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      284 2024-04-04 06:00:52.000000 seacrowd-0.0.5/seacrowd/utils/configs.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    12786 2024-04-04 06:00:52.000000 seacrowd-0.0.5/seacrowd/utils/constants.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:48.288611 seacrowd-0.0.5/seacrowd/utils/schemas/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1485 2024-04-04 06:00:52.000000 seacrowd-0.0.5/seacrowd/utils/schemas/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      506 2024-04-04 06:00:52.000000 seacrowd-0.0.5/seacrowd/utils/schemas/image_text.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1101 2024-04-04 06:00:52.000000 seacrowd-0.0.5/seacrowd/utils/schemas/imqa.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     2283 2024-04-04 06:00:52.000000 seacrowd-0.0.5/seacrowd/utils/schemas/kb.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      626 2024-04-04 06:00:52.000000 seacrowd-0.0.5/seacrowd/utils/schemas/pairs.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      371 2024-04-04 06:00:52.000000 seacrowd-0.0.5/seacrowd/utils/schemas/pairs_multilabel.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1007 2024-04-04 06:00:52.000000 seacrowd-0.0.5/seacrowd/utils/schemas/qa.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      206 2024-04-04 06:00:52.000000 seacrowd-0.0.5/seacrowd/utils/schemas/self_supervised_pretraining.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      525 2024-04-04 06:00:52.000000 seacrowd-0.0.5/seacrowd/utils/schemas/seq_label.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      618 2024-04-04 06:00:52.000000 seacrowd-0.0.5/seacrowd/utils/schemas/speech.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      606 2024-04-04 06:00:52.000000 seacrowd-0.0.5/seacrowd/utils/schemas/speech_multilabel.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      454 2024-04-04 06:00:52.000000 seacrowd-0.0.5/seacrowd/utils/schemas/speech_text.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      796 2024-04-04 06:00:52.000000 seacrowd-0.0.5/seacrowd/utils/schemas/speech_to_speech.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      311 2024-04-04 06:00:52.000000 seacrowd-0.0.5/seacrowd/utils/schemas/text.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      331 2024-04-04 06:00:52.000000 seacrowd-0.0.5/seacrowd/utils/schemas/text_multilabel.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      444 2024-04-04 06:00:52.000000 seacrowd-0.0.5/seacrowd/utils/schemas/text_to_text.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3046 2024-04-04 06:00:52.000000 seacrowd-0.0.5/seacrowd/utils/schemas/tod.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3068 2024-04-04 06:00:52.000000 seacrowd-0.0.5/seacrowd/utils/schemas/tree.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      810 2024-04-04 06:00:52.000000 seacrowd-0.0.5/seacrowd/utils/schemas/video.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:48.345605 seacrowd-0.0.5/seacrowd.egg-info/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1071 2024-04-11 09:12:39.000000 seacrowd-0.0.5/seacrowd.egg-info/PKG-INFO
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    31277 2024-04-11 09:12:40.000000 seacrowd-0.0.5/seacrowd.egg-info/SOURCES.txt
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        1 2024-04-11 09:12:39.000000 seacrowd-0.0.5/seacrowd.egg-info/dependency_links.txt
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      409 2024-04-11 09:12:39.000000 seacrowd-0.0.5/seacrowd.egg-info/requires.txt
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)       15 2024-04-11 09:12:39.000000 seacrowd-0.0.5/seacrowd.egg-info/top_level.txt
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      666 2024-04-11 09:12:48.376515 seacrowd-0.0.5/setup.cfg
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)       68 2024-04-04 06:00:52.000000 seacrowd-0.0.5/setup.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-11 09:12:48.325745 seacrowd-0.0.5/tests/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:52.000000 seacrowd-0.0.5/tests/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    23314 2024-04-04 06:00:52.000000 seacrowd-0.0.5/tests/test_seacrowd.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    20714 2024-04-04 06:00:52.000000 seacrowd-0.0.5/tests/test_seacrowd_source_only.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:54.583225 seacrowd-0.0.6/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    11357 2024-04-04 06:00:44.000000 seacrowd-0.0.6/LICENSE
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1071 2024-04-12 07:28:54.579359 seacrowd-0.0.6/PKG-INFO
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5757 2024-04-04 06:00:44.000000 seacrowd-0.0.6/README.md
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:46.732901 seacrowd-0.0.6/seacrowd/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      251 2024-04-12 07:21:36.000000 seacrowd-0.0.6/seacrowd/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    40451 2024-04-11 08:39:41.000000 seacrowd-0.0.6/seacrowd/config_helper.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:46.848049 seacrowd-0.0.6/seacrowd/sea_datasets/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/__init__.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:46.868089 seacrowd-0.0.6/seacrowd/sea_datasets/abui_wordnet/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/abui_wordnet/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5277 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/abui_wordnet/abui_wordnet.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:46.887959 seacrowd-0.0.6/seacrowd/sea_datasets/alt_burmese_treebank/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/alt_burmese_treebank/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5692 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/alt_burmese_treebank/alt_burmese_treebank.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:46.909020 seacrowd-0.0.6/seacrowd/sea_datasets/alt_burmese_treebank/utils/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/alt_burmese_treebank/utils/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     2661 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/alt_burmese_treebank/utils/alt_burmese_treebank_utils.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:46.931600 seacrowd-0.0.6/seacrowd/sea_datasets/ara_close/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/ara_close/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8227 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/ara_close/ara_close.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:46.957167 seacrowd-0.0.6/seacrowd/sea_datasets/asr_sindodusc/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/asr_sindodusc/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7231 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/asr_sindodusc/asr_sindodusc.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:46.978836 seacrowd-0.0.6/seacrowd/sea_datasets/asr_smaldusc/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/asr_smaldusc/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7305 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/asr_smaldusc/asr_smaldusc.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.009337 seacrowd-0.0.6/seacrowd/sea_datasets/asr_stidusc/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/asr_stidusc/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6979 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/asr_stidusc/asr_stidusc.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.036352 seacrowd-0.0.6/seacrowd/sea_datasets/audio_keyword_spotting/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/audio_keyword_spotting/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7860 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/audio_keyword_spotting/audio_keyword_spotting.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.064027 seacrowd-0.0.6/seacrowd/sea_datasets/aya_dataset/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/aya_dataset/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7482 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/aya_dataset/aya_dataset.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.084109 seacrowd-0.0.6/seacrowd/sea_datasets/barasa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/barasa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7224 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/barasa/barasa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.109275 seacrowd-0.0.6/seacrowd/sea_datasets/beaye_lexicon/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/beaye_lexicon/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4357 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/beaye_lexicon/beaye_lexicon.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.130968 seacrowd-0.0.6/seacrowd/sea_datasets/belebele/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/belebele/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8610 2024-04-11 08:39:41.000000 seacrowd-0.0.6/seacrowd/sea_datasets/belebele/belebele.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.153641 seacrowd-0.0.6/seacrowd/sea_datasets/bible_en_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/bible_en_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6790 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/bible_en_id/bible_en_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.174766 seacrowd-0.0.6/seacrowd/sea_datasets/bible_jv_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/bible_jv_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6856 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/bible_jv_id/bible_jv_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.197212 seacrowd-0.0.6/seacrowd/sea_datasets/bible_su_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/bible_su_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6632 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/bible_su_id/bible_su_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.235098 seacrowd-0.0.6/seacrowd/sea_datasets/bioner_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/bioner_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6108 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/bioner_id/bioner_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.258688 seacrowd-0.0.6/seacrowd/sea_datasets/bloom_captioning/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/bloom_captioning/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8518 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/bloom_captioning/bloom_captioning.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.288029 seacrowd-0.0.6/seacrowd/sea_datasets/bloom_lm/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/bloom_lm/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8430 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/bloom_lm/bloom_lm.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.335590 seacrowd-0.0.6/seacrowd/sea_datasets/bloom_speech/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/bloom_speech/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6922 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/bloom_speech/bloom_speech.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.361637 seacrowd-0.0.6/seacrowd/sea_datasets/bloom_vist/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/bloom_vist/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9674 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/bloom_vist/bloom_vist.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.381018 seacrowd-0.0.6/seacrowd/sea_datasets/burapha_th/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/burapha_th/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6995 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/burapha_th/burapha_th.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.419602 seacrowd-0.0.6/seacrowd/sea_datasets/burmese_romanize/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/burmese_romanize/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4420 2024-04-11 08:39:41.000000 seacrowd-0.0.6/seacrowd/sea_datasets/burmese_romanize/burmese_romanize.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.450411 seacrowd-0.0.6/seacrowd/sea_datasets/casa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/casa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5635 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/casa/casa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.473904 seacrowd-0.0.6/seacrowd/sea_datasets/cc100/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/cc100/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10941 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/cc100/cc100.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.495134 seacrowd-0.0.6/seacrowd/sea_datasets/cc_aligned_doc/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/cc_aligned_doc/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6230 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/cc_aligned_doc/cc_aligned_doc.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.529630 seacrowd-0.0.6/seacrowd/sea_datasets/cc_aligned_sent/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/cc_aligned_sent/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6256 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/cc_aligned_sent/cc_aligned_sent.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.554037 seacrowd-0.0.6/seacrowd/sea_datasets/cebuaner/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/cebuaner/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7783 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/cebuaner/cebuaner.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.574548 seacrowd-0.0.6/seacrowd/sea_datasets/coco_35l/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/coco_35l/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9830 2024-04-11 08:39:41.000000 seacrowd-0.0.6/seacrowd/sea_datasets/coco_35l/coco_35l.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.608979 seacrowd-0.0.6/seacrowd/sea_datasets/cod/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/cod/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6239 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/cod/cod.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.629113 seacrowd-0.0.6/seacrowd/sea_datasets/code_mixed_jv_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/code_mixed_jv_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8760 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/code_mixed_jv_id/code_mixed_jv_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.647789 seacrowd-0.0.6/seacrowd/sea_datasets/codeswitch_reddit/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/codeswitch_reddit/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9015 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/codeswitch_reddit/codeswitch_reddit.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.670309 seacrowd-0.0.6/seacrowd/sea_datasets/commonvoice_120/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/commonvoice_120/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9438 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/commonvoice_120/commonvoice_120.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.689763 seacrowd-0.0.6/seacrowd/sea_datasets/copal/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/copal/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5868 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/copal/copal.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.712355 seacrowd-0.0.6/seacrowd/sea_datasets/covost2/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/covost2/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10329 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/covost2/covost2.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.760118 seacrowd-0.0.6/seacrowd/sea_datasets/creole_rc/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.6/seacrowd/sea_datasets/creole_rc/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9448 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/creole_rc/creole_rc.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.780285 seacrowd-0.0.6/seacrowd/sea_datasets/crosssum/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/crosssum/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5467 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/crosssum/crosssum.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.804116 seacrowd-0.0.6/seacrowd/sea_datasets/cub_bahasa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/cub_bahasa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    14495 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/cub_bahasa/cub_bahasa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.824936 seacrowd-0.0.6/seacrowd/sea_datasets/culturax/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/culturax/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6383 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/culturax/culturax.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.849359 seacrowd-0.0.6/seacrowd/sea_datasets/cvss/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/cvss/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    11054 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/cvss/cvss.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.869445 seacrowd-0.0.6/seacrowd/sea_datasets/dengue_filipino/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/dengue_filipino/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4777 2024-04-11 08:39:41.000000 seacrowd-0.0.6/seacrowd/sea_datasets/dengue_filipino/dengue_filipino.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.889299 seacrowd-0.0.6/seacrowd/sea_datasets/emot/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/emot/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5522 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/emot/emot.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.909140 seacrowd-0.0.6/seacrowd/sea_datasets/emotcmt/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/emotcmt/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4484 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/emotcmt/emotcmt.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.927021 seacrowd-0.0.6/seacrowd/sea_datasets/emotes_3k/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/emotes_3k/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9257 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/emotes_3k/emotes_3k.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.947002 seacrowd-0.0.6/seacrowd/sea_datasets/emotion_id_opinion/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/emotion_id_opinion/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7315 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/emotion_id_opinion/emotion_id_opinion.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.968816 seacrowd-0.0.6/seacrowd/sea_datasets/etos/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/etos/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7041 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/etos/etos.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:47.988780 seacrowd-0.0.6/seacrowd/sea_datasets/facqa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/facqa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5788 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/facqa/facqa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.010272 seacrowd-0.0.6/seacrowd/sea_datasets/facqa/utils/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/facqa/utils/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      815 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/facqa/utils/facqa_utils.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.037824 seacrowd-0.0.6/seacrowd/sea_datasets/fakenews_ph/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/fakenews_ph/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4936 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/fakenews_ph/fakenews_ph.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.057662 seacrowd-0.0.6/seacrowd/sea_datasets/filipino_gay_lang/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/filipino_gay_lang/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4808 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/filipino_gay_lang/filipino_gay_lang.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.077081 seacrowd-0.0.6/seacrowd/sea_datasets/filipino_hatespeech_tiktok/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/filipino_hatespeech_tiktok/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4697 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/filipino_hatespeech_tiktok/filipino_hatespeech_tiktok.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.102456 seacrowd-0.0.6/seacrowd/sea_datasets/filipino_slang_norm/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/filipino_slang_norm/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4967 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/filipino_slang_norm/filipino_slang_norm.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.123926 seacrowd-0.0.6/seacrowd/sea_datasets/filipino_words_aoa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/filipino_words_aoa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4965 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/filipino_words_aoa/filipino_words_aoa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.144609 seacrowd-0.0.6/seacrowd/sea_datasets/filwordnet/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/filwordnet/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4819 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/filwordnet/filwordnet.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.184920 seacrowd-0.0.6/seacrowd/sea_datasets/fleurs/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/fleurs/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    13248 2024-04-11 09:11:07.000000 seacrowd-0.0.6/seacrowd/sea_datasets/fleurs/fleurs.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      785 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/fleurs/lang_config.json
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.225488 seacrowd-0.0.6/seacrowd/sea_datasets/flores200/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/flores200/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    13920 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/flores200/flores200.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.249544 seacrowd-0.0.6/seacrowd/sea_datasets/fsl_105/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/fsl_105/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6753 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/fsl_105/fsl_105.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.281406 seacrowd-0.0.6/seacrowd/sea_datasets/gatitos/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/gatitos/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6624 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/gatitos/gatitos.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.307190 seacrowd-0.0.6/seacrowd/sea_datasets/gklmip_newsclass/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/gklmip_newsclass/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6024 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/gklmip_newsclass/gklmip_newsclass.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.334563 seacrowd-0.0.6/seacrowd/sea_datasets/gklmip_sentiment/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/gklmip_sentiment/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5007 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/gklmip_sentiment/gklmip_sentiment.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.369817 seacrowd-0.0.6/seacrowd/sea_datasets/globalwoz/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/globalwoz/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10031 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/globalwoz/globalwoz.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.399450 seacrowd-0.0.6/seacrowd/sea_datasets/glotstorybook/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/glotstorybook/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5878 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/glotstorybook/glotstorybook.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.428794 seacrowd-0.0.6/seacrowd/sea_datasets/hoasa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/hoasa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6301 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/hoasa/hoasa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.468492 seacrowd-0.0.6/seacrowd/sea_datasets/iapp_squad/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/iapp_squad/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5420 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/iapp_squad/iapp_squad.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.500634 seacrowd-0.0.6/seacrowd/sea_datasets/iatf/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/iatf/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5801 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/iatf/iatf.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.527877 seacrowd-0.0.6/seacrowd/sea_datasets/icon/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/icon/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8351 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/icon/icon.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.560614 seacrowd-0.0.6/seacrowd/sea_datasets/id_abusive/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_abusive/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6540 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_abusive/id_abusive.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.592468 seacrowd-0.0.6/seacrowd/sea_datasets/id_abusive_news_comment/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_abusive_news_comment/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4293 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_abusive_news_comment/id_abusive_news_comment.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.616104 seacrowd-0.0.6/seacrowd/sea_datasets/id_am2ico/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_am2ico/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7430 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_am2ico/id_am2ico.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.659734 seacrowd-0.0.6/seacrowd/sea_datasets/id_clickbait/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_clickbait/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5770 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_clickbait/id_clickbait.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.682230 seacrowd-0.0.6/seacrowd/sea_datasets/id_coreference_resolution/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_coreference_resolution/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7576 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_coreference_resolution/id_coreference_resolution.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.721906 seacrowd-0.0.6/seacrowd/sea_datasets/id_frog_story/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_frog_story/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4524 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_frog_story/id_frog_story.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.748382 seacrowd-0.0.6/seacrowd/sea_datasets/id_google_play_review/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_google_play_review/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6144 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_google_play_review/id_google_play_review.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.776868 seacrowd-0.0.6/seacrowd/sea_datasets/id_hatespeech/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_hatespeech/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4450 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_hatespeech/id_hatespeech.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.809546 seacrowd-0.0.6/seacrowd/sea_datasets/id_hoax_news/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_hoax_news/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4555 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_hoax_news/id_hoax_news.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.841938 seacrowd-0.0.6/seacrowd/sea_datasets/id_hsd_nofaaulia/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_hsd_nofaaulia/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7252 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_hsd_nofaaulia/id_hsd_nofaaulia.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.863161 seacrowd-0.0.6/seacrowd/sea_datasets/id_msvd/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_msvd/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5051 2024-04-11 08:39:41.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_msvd/id_msvd.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.882911 seacrowd-0.0.6/seacrowd/sea_datasets/id_multilabel_hs/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_multilabel_hs/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6021 2024-04-04 06:00:46.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_multilabel_hs/id_multilabel_hs.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.904554 seacrowd-0.0.6/seacrowd/sea_datasets/id_panl_bppt/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_panl_bppt/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5616 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_panl_bppt/id_panl_bppt.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.923158 seacrowd-0.0.6/seacrowd/sea_datasets/id_qqp/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_qqp/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4686 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_qqp/id_qqp.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.944203 seacrowd-0.0.6/seacrowd/sea_datasets/id_sent_emo_mobile_apps/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_sent_emo_mobile_apps/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5395 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_sent_emo_mobile_apps/id_sent_emo_mobile_apps.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.961114 seacrowd-0.0.6/seacrowd/sea_datasets/id_sentiment_analysis/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_sentiment_analysis/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5538 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_sentiment_analysis/id_sentiment_analysis.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.981440 seacrowd-0.0.6/seacrowd/sea_datasets/id_short_answer_grading/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_short_answer_grading/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9107 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_short_answer_grading/id_short_answer_grading.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:48.998930 seacrowd-0.0.6/seacrowd/sea_datasets/id_short_answer_grading/utils/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_short_answer_grading/utils/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1826 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_short_answer_grading/utils/id_short_answer_grading_utils.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.019605 seacrowd-0.0.6/seacrowd/sea_datasets/id_stance/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_stance/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5114 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_stance/id_stance.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.039297 seacrowd-0.0.6/seacrowd/sea_datasets/id_sts/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_sts/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4308 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_sts/id_sts.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.073196 seacrowd-0.0.6/seacrowd/sea_datasets/id_vaccines_tweets/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_vaccines_tweets/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4329 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_vaccines_tweets/id_vaccines_tweets.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.099644 seacrowd-0.0.6/seacrowd/sea_datasets/id_wiki_parallel/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_wiki_parallel/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6697 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_wiki_parallel/id_wiki_parallel.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.122231 seacrowd-0.0.6/seacrowd/sea_datasets/id_wsd/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_wsd/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6404 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/id_wsd/id_wsd.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.149399 seacrowd-0.0.6/seacrowd/sea_datasets/identic/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/identic/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    13357 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/identic/identic.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.170225 seacrowd-0.0.6/seacrowd/sea_datasets/identifikasi_bahasa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/identifikasi_bahasa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5177 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/identifikasi_bahasa/identifikasi_bahasa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.190050 seacrowd-0.0.6/seacrowd/sea_datasets/idk_mrc/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/idk_mrc/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9530 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/idk_mrc/idk_mrc.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.217169 seacrowd-0.0.6/seacrowd/sea_datasets/idn_tagged_corpus_csui/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/idn_tagged_corpus_csui/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6193 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/idn_tagged_corpus_csui/idn_tagged_corpus_csui.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.244659 seacrowd-0.0.6/seacrowd/sea_datasets/ijelid/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/ijelid/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5403 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/ijelid/ijelid.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.273919 seacrowd-0.0.6/seacrowd/sea_datasets/imdb_jv/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/imdb_jv/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4894 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/imdb_jv/imdb_jv.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.293300 seacrowd-0.0.6/seacrowd/sea_datasets/indo4b/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indo4b/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7236 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indo4b/indo4b.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.314059 seacrowd-0.0.6/seacrowd/sea_datasets/indo4b_plus/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indo4b_plus/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7417 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indo4b_plus/indo4b_plus.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.337684 seacrowd-0.0.6/seacrowd/sea_datasets/indo_general_mt_en_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indo_general_mt_en_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6442 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indo_general_mt_en_id/indo_general_mt_en_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.359122 seacrowd-0.0.6/seacrowd/sea_datasets/indo_law/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indo_law/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5445 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indo_law/indo_law.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.382674 seacrowd-0.0.6/seacrowd/sea_datasets/indo_puisi/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indo_puisi/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4018 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indo_puisi/indo_puisi.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.418853 seacrowd-0.0.6/seacrowd/sea_datasets/indo_religious_mt_en_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indo_religious_mt_en_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8507 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indo_religious_mt_en_id/indo_religious_mt_en_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.440682 seacrowd-0.0.6/seacrowd/sea_datasets/indo_story_cloze/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indo_story_cloze/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6563 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indo_story_cloze/indo_story_cloze.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.464337 seacrowd-0.0.6/seacrowd/sea_datasets/indocamrest/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indocamrest/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6670 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indocamrest/indocamrest.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.487101 seacrowd-0.0.6/seacrowd/sea_datasets/indocollex/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indocollex/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6949 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indocollex/indocollex.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.512342 seacrowd-0.0.6/seacrowd/sea_datasets/indocoref/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indocoref/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    11610 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indocoref/indocoref.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.564345 seacrowd-0.0.6/seacrowd/sea_datasets/indocoref/utils/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indocoref/utils/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9072 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indocoref/utils/feature_utils.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     2091 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indocoref/utils/file_utils.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4307 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indocoref/utils/text_preprocess.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.588729 seacrowd-0.0.6/seacrowd/sea_datasets/indolem_ner_ugm/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indolem_ner_ugm/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6402 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indolem_ner_ugm/indolem_ner_ugm.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.609922 seacrowd-0.0.6/seacrowd/sea_datasets/indolem_nerui/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indolem_nerui/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8192 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indolem_nerui/indolem_nerui.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.630316 seacrowd-0.0.6/seacrowd/sea_datasets/indolem_ntp/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indolem_ntp/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5885 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indolem_ntp/indolem_ntp.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.652099 seacrowd-0.0.6/seacrowd/sea_datasets/indolem_sentiment/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indolem_sentiment/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    12679 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indolem_sentiment/indolem_sentiment.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.671427 seacrowd-0.0.6/seacrowd/sea_datasets/indolem_tweet_ordering/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indolem_tweet_ordering/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    12454 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indolem_tweet_ordering/indolem_tweet_ordering.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.691835 seacrowd-0.0.6/seacrowd/sea_datasets/indolem_ud_id_gsd/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indolem_ud_id_gsd/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8462 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indolem_ud_id_gsd/indolem_ud_id_gsd.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.712359 seacrowd-0.0.6/seacrowd/sea_datasets/indolem_ud_id_pud/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indolem_ud_id_pud/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8825 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indolem_ud_id_pud/indolem_ud_id_pud.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.731063 seacrowd-0.0.6/seacrowd/sea_datasets/indoler/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indoler/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9100 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indoler/indoler.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.749482 seacrowd-0.0.6/seacrowd/sea_datasets/indommlu/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indommlu/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10934 2024-04-11 08:39:41.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indommlu/indommlu.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.769543 seacrowd-0.0.6/seacrowd/sea_datasets/indoner_tourism/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indoner_tourism/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8394 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indoner_tourism/indoner_tourism.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.787605 seacrowd-0.0.6/seacrowd/sea_datasets/indonesia_chinese_mtrobusteval/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indonesia_chinese_mtrobusteval/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5250 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indonesia_chinese_mtrobusteval/indonesia_chinese_mtrobusteval.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.810219 seacrowd-0.0.6/seacrowd/sea_datasets/indonesian_madurese_bible_translation/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indonesian_madurese_bible_translation/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7932 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indonesian_madurese_bible_translation/indonesian_madurese_bible_translation.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.829474 seacrowd-0.0.6/seacrowd/sea_datasets/indonesian_news_dataset/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indonesian_news_dataset/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4581 2024-04-11 08:39:41.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indonesian_news_dataset/indonesian_news_dataset.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.848476 seacrowd-0.0.6/seacrowd/sea_datasets/indonesiannmt/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indonesiannmt/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9148 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indonesiannmt/indonesiannmt.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.868241 seacrowd-0.0.6/seacrowd/sea_datasets/indonglish/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indonglish/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8339 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indonglish/indonglish.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.887867 seacrowd-0.0.6/seacrowd/sea_datasets/indonli/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indonli/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8050 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indonli/indonli.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.907031 seacrowd-0.0.6/seacrowd/sea_datasets/indonlu_nergrit/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indonlu_nergrit/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5677 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indonlu_nergrit/indonlu_nergrit.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.925615 seacrowd-0.0.6/seacrowd/sea_datasets/indoqa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indoqa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5422 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indoqa/indoqa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.944445 seacrowd-0.0.6/seacrowd/sea_datasets/indosmd/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indosmd/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    13550 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indosmd/indosmd.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.961796 seacrowd-0.0.6/seacrowd/sea_datasets/indosum/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indosum/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6872 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indosum/indosum.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:49.984010 seacrowd-0.0.6/seacrowd/sea_datasets/indotacos/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indotacos/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5477 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indotacos/indotacos.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.002761 seacrowd-0.0.6/seacrowd/sea_datasets/indowiki/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indowiki/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7684 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indowiki/indowiki.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.021235 seacrowd-0.0.6/seacrowd/sea_datasets/indqner/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        1 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indqner/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6614 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indqner/indqner.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.036397 seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_digit_cdsr/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_digit_cdsr/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9856 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_digit_cdsr/indspeech_digit_cdsr.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.055601 seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_news_ethnicsr/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_news_ethnicsr/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8440 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_news_ethnicsr/indspeech_news_ethnicsr.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.077458 seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_news_lvcsr/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_news_lvcsr/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9432 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_news_lvcsr/indspeech_news_lvcsr.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.097760 seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_news_tts/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_news_tts/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8857 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_news_tts/indspeech_news_tts.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.116918 seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_newstra_ethnicsr/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_newstra_ethnicsr/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    11615 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_newstra_ethnicsr/indspeech_newstra_ethnicsr.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.136618 seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_teldialog_lvcsr/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_teldialog_lvcsr/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9932 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_teldialog_lvcsr/indspeech_teldialog_lvcsr.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.156815 seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_teldialog_svcsr/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_teldialog_svcsr/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9818 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_teldialog_svcsr/indspeech_teldialog_svcsr.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.180791 seacrowd-0.0.6/seacrowd/sea_datasets/inset_lexicon/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/inset_lexicon/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4829 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/inset_lexicon/inset_lexicon.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.203285 seacrowd-0.0.6/seacrowd/sea_datasets/jadi_ide/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/jadi_ide/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4404 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/jadi_ide/jadi_ide.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.224124 seacrowd-0.0.6/seacrowd/sea_datasets/jv_id_asr/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/jv_id_asr/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6236 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/jv_id_asr/jv_id_asr.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.246083 seacrowd-0.0.6/seacrowd/sea_datasets/jv_id_tts/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/jv_id_tts/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7628 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/jv_id_tts/jv_id_tts.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.265532 seacrowd-0.0.6/seacrowd/sea_datasets/kamus_alay/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/kamus_alay/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5286 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/kamus_alay/kamus_alay.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.284753 seacrowd-0.0.6/seacrowd/sea_datasets/karonese_sentiment/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/karonese_sentiment/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4533 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/karonese_sentiment/karonese_sentiment.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.306271 seacrowd-0.0.6/seacrowd/sea_datasets/kawat/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/kawat/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5933 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/kawat/kawat.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.332834 seacrowd-0.0.6/seacrowd/sea_datasets/kde4/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/kde4/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    14408 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/kde4/kde4.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.352141 seacrowd-0.0.6/seacrowd/sea_datasets/keps/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/keps/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5066 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/keps/keps.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.377063 seacrowd-0.0.6/seacrowd/sea_datasets/kheng_info/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/kheng_info/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3687 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/kheng_info/kheng_info.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.398409 seacrowd-0.0.6/seacrowd/sea_datasets/khmer_alt_pos/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/khmer_alt_pos/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7442 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/khmer_alt_pos/khmer_alt_pos.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.425789 seacrowd-0.0.6/seacrowd/sea_datasets/khpos/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/khpos/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8756 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/khpos/khpos.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.450333 seacrowd-0.0.6/seacrowd/sea_datasets/kopi_cc/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/kopi_cc/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10035 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/kopi_cc/kopi_cc.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.472020 seacrowd-0.0.6/seacrowd/sea_datasets/kopi_cc_news/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/kopi_cc_news/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5088 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/kopi_cc_news/kopi_cc_news.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.491281 seacrowd-0.0.6/seacrowd/sea_datasets/kopi_nllb/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/kopi_nllb/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5956 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/kopi_nllb/kopi_nllb.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.510706 seacrowd-0.0.6/seacrowd/sea_datasets/korpus_nusantara/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/korpus_nusantara/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8476 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/korpus_nusantara/korpus_nusantara.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.529386 seacrowd-0.0.6/seacrowd/sea_datasets/lazada_review_filipino/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/lazada_review_filipino/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4913 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/lazada_review_filipino/lazada_review_filipino.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.548696 seacrowd-0.0.6/seacrowd/sea_datasets/librivox_indonesia/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/librivox_indonesia/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8736 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/librivox_indonesia/librivox_indonesia.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.568334 seacrowd-0.0.6/seacrowd/sea_datasets/limesoda/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/limesoda/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6775 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/limesoda/limesoda.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.590361 seacrowd-0.0.6/seacrowd/sea_datasets/liputan6/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/liputan6/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7512 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/liputan6/liputan6.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.610947 seacrowd-0.0.6/seacrowd/sea_datasets/local_id_abusive/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/local_id_abusive/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7530 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/local_id_abusive/local_id_abusive.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.631210 seacrowd-0.0.6/seacrowd/sea_datasets/lr_sum/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/lr_sum/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6160 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/lr_sum/lr_sum.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.659269 seacrowd-0.0.6/seacrowd/sea_datasets/m3exam/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/m3exam/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    14637 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/m3exam/m3exam.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.685192 seacrowd-0.0.6/seacrowd/sea_datasets/mabl/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/mabl/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8609 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/mabl/mabl.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.705454 seacrowd-0.0.6/seacrowd/sea_datasets/malaysia_tweets/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/malaysia_tweets/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6432 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/malaysia_tweets/malaysia_tweets.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.728278 seacrowd-0.0.6/seacrowd/sea_datasets/malindo_morph/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/malindo_morph/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4617 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/malindo_morph/malindo_morph.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.746300 seacrowd-0.0.6/seacrowd/sea_datasets/malindo_parallel/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/malindo_parallel/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6494 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/malindo_parallel/malindo_parallel.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.771053 seacrowd-0.0.6/seacrowd/sea_datasets/massive/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/massive/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    18420 2024-04-04 06:00:48.000000 seacrowd-0.0.6/seacrowd/sea_datasets/massive/massive.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.792771 seacrowd-0.0.6/seacrowd/sea_datasets/mc4_indo/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/mc4_indo/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5510 2024-04-11 08:39:41.000000 seacrowd-0.0.6/seacrowd/sea_datasets/mc4_indo/mc4_indo.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.811734 seacrowd-0.0.6/seacrowd/sea_datasets/melayu_brunei/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/melayu_brunei/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10682 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/melayu_brunei/melayu_brunei.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.832739 seacrowd-0.0.6/seacrowd/sea_datasets/melayu_sabah/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/melayu_sabah/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5561 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/melayu_sabah/melayu_sabah.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.851137 seacrowd-0.0.6/seacrowd/sea_datasets/melayu_sarawak/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/melayu_sarawak/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6559 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/melayu_sarawak/melayu_sarawak.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.869954 seacrowd-0.0.6/seacrowd/sea_datasets/melayu_standard_lisan/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/melayu_standard_lisan/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7594 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/melayu_standard_lisan/melayu_standard_lisan.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.887035 seacrowd-0.0.6/seacrowd/sea_datasets/memolon/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/memolon/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5589 2024-04-11 08:39:41.000000 seacrowd-0.0.6/seacrowd/sea_datasets/memolon/memolon.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.907814 seacrowd-0.0.6/seacrowd/sea_datasets/minangnlp_mt/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/minangnlp_mt/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6874 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/minangnlp_mt/minangnlp_mt.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.927611 seacrowd-0.0.6/seacrowd/sea_datasets/miracl/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/miracl/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    13119 2024-04-11 08:39:41.000000 seacrowd-0.0.6/seacrowd/sea_datasets/miracl/miracl.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.948262 seacrowd-0.0.6/seacrowd/sea_datasets/mkqa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/mkqa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8345 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/mkqa/mkqa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.971349 seacrowd-0.0.6/seacrowd/sea_datasets/mlqa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        1 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/mlqa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9825 2024-04-11 08:39:41.000000 seacrowd-0.0.6/seacrowd/sea_datasets/mlqa/mlqa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:50.994086 seacrowd-0.0.6/seacrowd/sea_datasets/mozilla_pontoon/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/mozilla_pontoon/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6211 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/mozilla_pontoon/mozilla_pontoon.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.024238 seacrowd-0.0.6/seacrowd/sea_datasets/mswc/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/mswc/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8048 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/mswc/mswc.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.054345 seacrowd-0.0.6/seacrowd/sea_datasets/mtop_intent_classification/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/mtop_intent_classification/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     2654 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/mtop_intent_classification/labels.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5662 2024-04-11 08:39:41.000000 seacrowd-0.0.6/seacrowd/sea_datasets/mtop_intent_classification/mtop_intent_classification.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.075330 seacrowd-0.0.6/seacrowd/sea_datasets/multilexnorm/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/multilexnorm/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6223 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/multilexnorm/multilexnorm.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.096930 seacrowd-0.0.6/seacrowd/sea_datasets/my_paraphrase/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/my_paraphrase/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8124 2024-04-11 08:39:41.000000 seacrowd-0.0.6/seacrowd/sea_datasets/my_paraphrase/my_paraphrase.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.119908 seacrowd-0.0.6/seacrowd/sea_datasets/myanmar_rakhine_parallel/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/myanmar_rakhine_parallel/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7223 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/myanmar_rakhine_parallel/myanmar_rakhine_parallel.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.142628 seacrowd-0.0.6/seacrowd/sea_datasets/mypos/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/mypos/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5116 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/mypos/mypos.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.162927 seacrowd-0.0.6/seacrowd/sea_datasets/mysentence/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/mysentence/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7612 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/mysentence/mysentence.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.182927 seacrowd-0.0.6/seacrowd/sea_datasets/myxnli/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/myxnli/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5096 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/myxnli/myxnli.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.201681 seacrowd-0.0.6/seacrowd/sea_datasets/nergrit/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/nergrit/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6322 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/nergrit/nergrit.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.220345 seacrowd-0.0.6/seacrowd/sea_datasets/nerp/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/nerp/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4852 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/nerp/nerp.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.240939 seacrowd-0.0.6/seacrowd/sea_datasets/netifier/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/netifier/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4838 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/netifier/netifier.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.262756 seacrowd-0.0.6/seacrowd/sea_datasets/news_en_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/news_en_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5003 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/news_en_id/news_en_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.283584 seacrowd-0.0.6/seacrowd/sea_datasets/newsph/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/newsph/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3810 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/newsph/newsph.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.302819 seacrowd-0.0.6/seacrowd/sea_datasets/nllb_seed/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/nllb_seed/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    15208 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/nllb_seed/nllb_seed.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.319712 seacrowd-0.0.6/seacrowd/sea_datasets/ntrex_128/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/ntrex_128/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10971 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/ntrex_128/ntrex_128.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.355007 seacrowd-0.0.6/seacrowd/sea_datasets/nusaparagraph_emot/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/nusaparagraph_emot/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8785 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/nusaparagraph_emot/nusaparagraph_emot.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.377840 seacrowd-0.0.6/seacrowd/sea_datasets/nusaparagraph_rhetoric/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/nusaparagraph_rhetoric/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8792 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/nusaparagraph_rhetoric/nusaparagraph_rhetoric.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.397230 seacrowd-0.0.6/seacrowd/sea_datasets/nusaparagraph_topic/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/nusaparagraph_topic/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8845 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/nusaparagraph_topic/nusaparagraph_topic.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.416960 seacrowd-0.0.6/seacrowd/sea_datasets/nusatranslation_emot/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/nusatranslation_emot/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8233 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/nusatranslation_emot/nusatranslation_emot.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.438103 seacrowd-0.0.6/seacrowd/sea_datasets/nusatranslation_mt/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/nusatranslation_mt/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9156 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/nusatranslation_mt/nusatranslation_mt.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.465473 seacrowd-0.0.6/seacrowd/sea_datasets/nusatranslation_senti/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/nusatranslation_senti/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8285 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/nusatranslation_senti/nusatranslation_senti.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.485183 seacrowd-0.0.6/seacrowd/sea_datasets/nusax_mt/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/nusax_mt/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7578 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/nusax_mt/nusax_mt.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.506795 seacrowd-0.0.6/seacrowd/sea_datasets/nusax_senti/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/nusax_senti/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7250 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/nusax_senti/nusax_senti.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.526569 seacrowd-0.0.6/seacrowd/sea_datasets/oil/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/oil/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5477 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/oil/oil.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.547104 seacrowd-0.0.6/seacrowd/sea_datasets/ojw/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/ojw/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5110 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/ojw/ojw.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.565774 seacrowd-0.0.6/seacrowd/sea_datasets/openlid/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/openlid/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7915 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/openlid/openlid.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.585778 seacrowd-0.0.6/seacrowd/sea_datasets/openslr/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/openslr/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10343 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/openslr/openslr.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.613775 seacrowd-0.0.6/seacrowd/sea_datasets/orchid_pos/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/orchid_pos/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9625 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/orchid_pos/orchid_pos.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.633731 seacrowd-0.0.6/seacrowd/sea_datasets/oscar_2201/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/oscar_2201/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    16270 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/oscar_2201/oscar_2201.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.655182 seacrowd-0.0.6/seacrowd/sea_datasets/palito/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/palito/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5930 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/palito/palito.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.674421 seacrowd-0.0.6/seacrowd/sea_datasets/paracotta_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/paracotta_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4768 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/paracotta_id/paracotta_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.693919 seacrowd-0.0.6/seacrowd/sea_datasets/parallel_id_nyo/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/parallel_id_nyo/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5471 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/parallel_id_nyo/parallel_id_nyo.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.710989 seacrowd-0.0.6/seacrowd/sea_datasets/parallel_su_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/parallel_su_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4782 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/parallel_su_id/parallel_su_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.734097 seacrowd-0.0.6/seacrowd/sea_datasets/ph_fake_news_corpus/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/ph_fake_news_corpus/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4339 2024-04-11 08:39:41.000000 seacrowd-0.0.6/seacrowd/sea_datasets/ph_fake_news_corpus/ph_fake_news_corpus.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.756381 seacrowd-0.0.6/seacrowd/sea_datasets/pho_ner_covid/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/pho_ner_covid/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6866 2024-04-04 06:00:49.000000 seacrowd-0.0.6/seacrowd/sea_datasets/pho_ner_covid/pho_ner_covid.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.774104 seacrowd-0.0.6/seacrowd/sea_datasets/phomt/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/phomt/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5141 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/phomt/phomt.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.793708 seacrowd-0.0.6/seacrowd/sea_datasets/phost/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/phost/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9498 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/phost/phost.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.814098 seacrowd-0.0.6/seacrowd/sea_datasets/posp/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/posp/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5990 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/posp/posp.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.833201 seacrowd-0.0.6/seacrowd/sea_datasets/postag_su/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/postag_su/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8033 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/postag_su/postag_su.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.854553 seacrowd-0.0.6/seacrowd/sea_datasets/prdect_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/prdect_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7572 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/prdect_id/prdect_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.884638 seacrowd-0.0.6/seacrowd/sea_datasets/qasina/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/qasina/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6424 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/qasina/qasina.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.903931 seacrowd-0.0.6/seacrowd/sea_datasets/roots_vi_ted/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/roots_vi_ted/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5065 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/roots_vi_ted/roots_vi_ted.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.925362 seacrowd-0.0.6/seacrowd/sea_datasets/sampiran/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/sampiran/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5024 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/sampiran/sampiran.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.954764 seacrowd-0.0.6/seacrowd/sea_datasets/sap_wat/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/sap_wat/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7077 2024-04-11 08:39:41.000000 seacrowd-0.0.6/seacrowd/sea_datasets/sap_wat/sap_wat.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.977381 seacrowd-0.0.6/seacrowd/sea_datasets/sarawak_malay/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/sarawak_malay/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7381 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/sarawak_malay/sarawak_malay.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:51.995690 seacrowd-0.0.6/seacrowd/sea_datasets/scb_mt_en_th/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/scb_mt_en_th/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7071 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/scb_mt_en_th/scb_mt_en_th.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.020982 seacrowd-0.0.6/seacrowd/sea_datasets/sea_bench/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/sea_bench/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7206 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/sea_bench/sea_bench.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.045137 seacrowd-0.0.6/seacrowd/sea_datasets/sea_madlad/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/sea_madlad/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10051 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/sea_madlad/sea_madlad.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.080157 seacrowd-0.0.6/seacrowd/sea_datasets/sea_wiki/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/sea_wiki/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1829 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/sea_wiki/lang_config.json
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9350 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/sea_wiki/sea_wiki.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.100232 seacrowd-0.0.6/seacrowd/sea_datasets/seaeval/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/seaeval/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9350 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/seaeval/seaeval.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.120085 seacrowd-0.0.6/seacrowd/sea_datasets/seahorse/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/seahorse/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6884 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/seahorse/seahorse.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.139474 seacrowd-0.0.6/seacrowd/sea_datasets/sentiment_nathasa_review/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/sentiment_nathasa_review/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6002 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/sentiment_nathasa_review/sentiment_nathasa_review.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.158288 seacrowd-0.0.6/seacrowd/sea_datasets/shopee_reviews_tagalog/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/shopee_reviews_tagalog/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4597 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/shopee_reviews_tagalog/shopee_reviews_tagalog.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.175538 seacrowd-0.0.6/seacrowd/sea_datasets/singgalang/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/singgalang/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5430 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/singgalang/singgalang.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.194957 seacrowd-0.0.6/seacrowd/sea_datasets/smsa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/smsa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5575 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/smsa/smsa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.214265 seacrowd-0.0.6/seacrowd/sea_datasets/snli_indo/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/snli_indo/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6244 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/snli_indo/snli_indo.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.235054 seacrowd-0.0.6/seacrowd/sea_datasets/spamid_pair/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/spamid_pair/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5524 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/spamid_pair/spamid_pair.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.254263 seacrowd-0.0.6/seacrowd/sea_datasets/squad_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/squad_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5315 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/squad_id/squad_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.271852 seacrowd-0.0.6/seacrowd/sea_datasets/stb_ext/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/stb_ext/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9273 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/stb_ext/stb_ext.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.290865 seacrowd-0.0.6/seacrowd/sea_datasets/stif_indonesia/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/stif_indonesia/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5135 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/stif_indonesia/stif_indonesia.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.312547 seacrowd-0.0.6/seacrowd/sea_datasets/struct_amb_ind/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/struct_amb_ind/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7724 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/struct_amb_ind/struct_amb_ind.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.334159 seacrowd-0.0.6/seacrowd/sea_datasets/su_emot/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/su_emot/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4567 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/su_emot/su_emot.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.353250 seacrowd-0.0.6/seacrowd/sea_datasets/su_id_asr/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/su_id_asr/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5601 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/su_id_asr/su_id_asr.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.369887 seacrowd-0.0.6/seacrowd/sea_datasets/su_id_tts/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/su_id_tts/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7636 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/su_id_tts/su_id_tts.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.391168 seacrowd-0.0.6/seacrowd/sea_datasets/talpco/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/talpco/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6870 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/talpco/talpco.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.410038 seacrowd-0.0.6/seacrowd/sea_datasets/tatabahasa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/tatabahasa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5411 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/tatabahasa/tatabahasa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.430492 seacrowd-0.0.6/seacrowd/sea_datasets/tatoeba/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/tatoeba/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7636 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/tatoeba/tatoeba.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.451051 seacrowd-0.0.6/seacrowd/sea_datasets/tcope/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/tcope/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6693 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/tcope/tcope.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.471554 seacrowd-0.0.6/seacrowd/sea_datasets/ted_en_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/ted_en_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7105 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/ted_en_id/ted_en_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.491820 seacrowd-0.0.6/seacrowd/sea_datasets/term_a/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/term_a/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5358 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/term_a/term_a.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.512615 seacrowd-0.0.6/seacrowd/sea_datasets/tgl_profanity/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/tgl_profanity/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4351 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/tgl_profanity/tgl_profanity.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.530491 seacrowd-0.0.6/seacrowd/sea_datasets/tha_lao_embassy_parcor/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/tha_lao_embassy_parcor/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4436 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/tha_lao_embassy_parcor/tha_lao_embassy_parcor.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.550752 seacrowd-0.0.6/seacrowd/sea_datasets/thai_alpaca/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/thai_alpaca/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3943 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/thai_alpaca/thai_alpaca.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.569334 seacrowd-0.0.6/seacrowd/sea_datasets/thai_constitution/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/thai_constitution/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10954 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/thai_constitution/thai_constitution.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.590187 seacrowd-0.0.6/seacrowd/sea_datasets/thai_databricks_dolly/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/thai_databricks_dolly/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4388 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/thai_databricks_dolly/thai_databricks_dolly.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.610185 seacrowd-0.0.6/seacrowd/sea_datasets/thai_depression/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/thai_depression/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5739 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/thai_depression/thai_depression.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.629439 seacrowd-0.0.6/seacrowd/sea_datasets/thai_gpteacher/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/thai_gpteacher/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3960 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/thai_gpteacher/thai_gpteacher.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.649549 seacrowd-0.0.6/seacrowd/sea_datasets/thai_hh_rlhf/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/thai_hh_rlhf/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5077 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/thai_hh_rlhf/thai_hh_rlhf.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.668593 seacrowd-0.0.6/seacrowd/sea_datasets/thai_sum/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/thai_sum/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5683 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/thai_sum/thai_sum.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.693104 seacrowd-0.0.6/seacrowd/sea_datasets/thai_toxicity_tweet/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/thai_toxicity_tweet/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4555 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/thai_toxicity_tweet/thai_toxicity_tweet.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.712448 seacrowd-0.0.6/seacrowd/sea_datasets/tico_19/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/tico_19/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    12192 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/tico_19/tico_19.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.730671 seacrowd-0.0.6/seacrowd/sea_datasets/titml_idn/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/titml_idn/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5900 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/titml_idn/titml_idn.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.749801 seacrowd-0.0.6/seacrowd/sea_datasets/tlunified_ner/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.6/seacrowd/sea_datasets/tlunified_ner/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5800 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/tlunified_ner/tlunified_ner.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.771364 seacrowd-0.0.6/seacrowd/sea_datasets/toxicity_200/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/toxicity_200/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5975 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/toxicity_200/toxicity_200.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.790921 seacrowd-0.0.6/seacrowd/sea_datasets/tydiqa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/tydiqa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    23881 2024-04-11 08:39:41.000000 seacrowd-0.0.6/seacrowd/sea_datasets/tydiqa/tydiqa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.813641 seacrowd-0.0.6/seacrowd/sea_datasets/typhoon_yolanda_tweets/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        1 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/typhoon_yolanda_tweets/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5165 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/typhoon_yolanda_tweets/typhoon_yolanda_tweets.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.835234 seacrowd-0.0.6/seacrowd/sea_datasets/ucla_phonetic/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/ucla_phonetic/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6531 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/ucla_phonetic/ucla_phonetic.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.867533 seacrowd-0.0.6/seacrowd/sea_datasets/ud_id_csui/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/ud_id_csui/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9185 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/ud_id_csui/ud_id_csui.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.896691 seacrowd-0.0.6/seacrowd/sea_datasets/ud_jv_csui/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/ud_jv_csui/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10052 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/ud_jv_csui/ud_jv_csui.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.919987 seacrowd-0.0.6/seacrowd/sea_datasets/udhr/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/udhr/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6030 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/udhr/udhr.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.936703 seacrowd-0.0.6/seacrowd/sea_datasets/udhr_lid/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/udhr_lid/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5190 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/udhr_lid/udhr_lid.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.964902 seacrowd-0.0.6/seacrowd/sea_datasets/uit_vicov19qa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/uit_vicov19qa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7244 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/uit_vicov19qa/uit_vicov19qa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:52.993713 seacrowd-0.0.6/seacrowd/sea_datasets/uit_victsd/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/uit_victsd/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5311 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/uit_victsd/uit_victsd.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.022732 seacrowd-0.0.6/seacrowd/sea_datasets/uit_vihsd/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/uit_vihsd/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5721 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/uit_vihsd/uit_vihsd.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.059473 seacrowd-0.0.6/seacrowd/sea_datasets/uit_viic/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/uit_viic/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6572 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/uit_viic/uit_viic.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.091222 seacrowd-0.0.6/seacrowd/sea_datasets/uit_viocd/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/uit_viocd/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4819 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/uit_viocd/uit_viocd.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.116615 seacrowd-0.0.6/seacrowd/sea_datasets/uit_vion/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/uit_vion/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5939 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/uit_vion/uit_vion.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.158425 seacrowd-0.0.6/seacrowd/sea_datasets/uit_visd4sa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/uit_visd4sa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7034 2024-04-11 08:39:41.000000 seacrowd-0.0.6/seacrowd/sea_datasets/uit_visd4sa/uit_visd4sa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.187888 seacrowd-0.0.6/seacrowd/sea_datasets/uit_vsfc/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/uit_vsfc/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8715 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/uit_vsfc/uit_vsfc.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.210728 seacrowd-0.0.6/seacrowd/sea_datasets/uit_vsmec/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/uit_vsmec/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4802 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/uit_vsmec/uit_vsmec.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.244139 seacrowd-0.0.6/seacrowd/sea_datasets/unimorph/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/unimorph/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    15492 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/unimorph/unimorph.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.268184 seacrowd-0.0.6/seacrowd/sea_datasets/unimorph_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/unimorph_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7445 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/unimorph_id/unimorph_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.300159 seacrowd-0.0.6/seacrowd/sea_datasets/vi_pubmed/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/vi_pubmed/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    15136 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/vi_pubmed/vi_pubmed.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.355915 seacrowd-0.0.6/seacrowd/sea_datasets/vihealthqa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/vihealthqa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5587 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/vihealthqa/vihealthqa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.381141 seacrowd-0.0.6/seacrowd/sea_datasets/visobert/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/visobert/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6265 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/visobert/visobert.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.409133 seacrowd-0.0.6/seacrowd/sea_datasets/vispamreviews/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/vispamreviews/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7245 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/vispamreviews/vispamreviews.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.445508 seacrowd-0.0.6/seacrowd/sea_datasets/vistec_tp_th_21/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/vistec_tp_th_21/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6739 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/vistec_tp_th_21/vistec_tp_th_21.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.471518 seacrowd-0.0.6/seacrowd/sea_datasets/vitext2sql/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/vitext2sql/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6893 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/vitext2sql/vitext2sql.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.498382 seacrowd-0.0.6/seacrowd/sea_datasets/vivos/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/vivos/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7832 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/vivos/vivos.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.524840 seacrowd-0.0.6/seacrowd/sea_datasets/vivqa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/vivqa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9080 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/vivqa/vivqa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.544552 seacrowd-0.0.6/seacrowd/sea_datasets/vlsp2016_ner/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/vlsp2016_ner/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5857 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/vlsp2016_ner/vlsp2016_ner.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.570179 seacrowd-0.0.6/seacrowd/sea_datasets/vlsp2016_sa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/vlsp2016_sa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7134 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/vlsp2016_sa/vlsp2016_sa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.618434 seacrowd-0.0.6/seacrowd/sea_datasets/vndt/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/vndt/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     2232 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/vndt/utils.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7852 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/vndt/vndt.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.637585 seacrowd-0.0.6/seacrowd/sea_datasets/voxlingua/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/voxlingua/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7980 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/voxlingua/voxlingua.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.661093 seacrowd-0.0.6/seacrowd/sea_datasets/weathub/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/weathub/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7521 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/weathub/weathub.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.681222 seacrowd-0.0.6/seacrowd/sea_datasets/wikiann/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/wikiann/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8643 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/wikiann/wikiann.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.700781 seacrowd-0.0.6/seacrowd/sea_datasets/wikilingua/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/wikilingua/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4984 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/wikilingua/wikilingua.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.720214 seacrowd-0.0.6/seacrowd/sea_datasets/wikimatrix/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/wikimatrix/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8585 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/wikimatrix/wikimatrix.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.749112 seacrowd-0.0.6/seacrowd/sea_datasets/wikitext_tl_39/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/wikitext_tl_39/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3663 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/wikitext_tl_39/wikitext_tl_39.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.780130 seacrowd-0.0.6/seacrowd/sea_datasets/wili_2018/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/wili_2018/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6699 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/wili_2018/wili_2018.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.799674 seacrowd-0.0.6/seacrowd/sea_datasets/wisesight_thai_sentiment/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/wisesight_thai_sentiment/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7027 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/wisesight_thai_sentiment/wisesight_thai_sentiment.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.827694 seacrowd-0.0.6/seacrowd/sea_datasets/wit/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/wit/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    12057 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/wit/wit.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.850932 seacrowd-0.0.6/seacrowd/sea_datasets/wongnai_reviews/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/wongnai_reviews/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4106 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/wongnai_reviews/wongnai_reviews.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.868850 seacrowd-0.0.6/seacrowd/sea_datasets/wrete/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/wrete/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6113 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/wrete/wrete.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.885963 seacrowd-0.0.6/seacrowd/sea_datasets/x_fact/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/x_fact/__init__.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.905417 seacrowd-0.0.6/seacrowd/sea_datasets/x_fact/utils/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/x_fact/utils/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      473 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/x_fact/utils/x_fact_utils.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5900 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/x_fact/x_fact.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.935194 seacrowd-0.0.6/seacrowd/sea_datasets/xcopa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/xcopa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7024 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/xcopa/xcopa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.961232 seacrowd-0.0.6/seacrowd/sea_datasets/xl_jailbreak/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/xl_jailbreak/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6317 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/xl_jailbreak/xl_jailbreak.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.978210 seacrowd-0.0.6/seacrowd/sea_datasets/xl_sum/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/xl_sum/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6903 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/xl_sum/xl_sum.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:53.995494 seacrowd-0.0.6/seacrowd/sea_datasets/xm3600/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/xm3600/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8233 2024-04-11 08:39:41.000000 seacrowd-0.0.6/seacrowd/sea_datasets/xm3600/xm3600.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:54.043503 seacrowd-0.0.6/seacrowd/sea_datasets/xnli/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/xnli/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8333 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/xnli/xnli.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:54.085793 seacrowd-0.0.6/seacrowd/sea_datasets/xpersona_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/xpersona_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6550 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/xpersona_id/xpersona_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:54.106224 seacrowd-0.0.6/seacrowd/sea_datasets/xquad/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/xquad/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4819 2024-04-04 06:00:51.000000 seacrowd-0.0.6/seacrowd/sea_datasets/xquad/xquad.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:54.146233 seacrowd-0.0.6/seacrowd/sea_datasets/xsid/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/sea_datasets/xsid/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9510 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/sea_datasets/xsid/xsid.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:54.166886 seacrowd-0.0.6/seacrowd/sea_datasets/xstorycloze/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/sea_datasets/xstorycloze/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6794 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/sea_datasets/xstorycloze/xstorycloze.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:54.188320 seacrowd-0.0.6/seacrowd/sea_datasets/yunshan_cup_2020/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/sea_datasets/yunshan_cup_2020/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5828 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/sea_datasets/yunshan_cup_2020/yunshan_cup_2020.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:54.245136 seacrowd-0.0.6/seacrowd/utils/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/utils/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5493 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/utils/common_parser.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      284 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/utils/configs.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    12786 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/utils/constants.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:54.490913 seacrowd-0.0.6/seacrowd/utils/schemas/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1485 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/utils/schemas/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      506 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/utils/schemas/image_text.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1101 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/utils/schemas/imqa.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     2283 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/utils/schemas/kb.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      626 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/utils/schemas/pairs.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      371 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/utils/schemas/pairs_multilabel.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1007 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/utils/schemas/qa.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      206 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/utils/schemas/self_supervised_pretraining.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      525 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/utils/schemas/seq_label.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      618 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/utils/schemas/speech.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      606 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/utils/schemas/speech_multilabel.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      454 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/utils/schemas/speech_text.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      796 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/utils/schemas/speech_to_speech.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      311 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/utils/schemas/text.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      331 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/utils/schemas/text_multilabel.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      444 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/utils/schemas/text_to_text.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3046 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/utils/schemas/tod.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3068 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/utils/schemas/tree.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      810 2024-04-04 06:00:52.000000 seacrowd-0.0.6/seacrowd/utils/schemas/video.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:54.560764 seacrowd-0.0.6/seacrowd.egg-info/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1071 2024-04-12 07:28:43.000000 seacrowd-0.0.6/seacrowd.egg-info/PKG-INFO
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    31371 2024-04-12 07:28:44.000000 seacrowd-0.0.6/seacrowd.egg-info/SOURCES.txt
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        1 2024-04-12 07:28:43.000000 seacrowd-0.0.6/seacrowd.egg-info/dependency_links.txt
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      409 2024-04-12 07:28:43.000000 seacrowd-0.0.6/seacrowd.egg-info/requires.txt
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)       15 2024-04-12 07:28:43.000000 seacrowd-0.0.6/seacrowd.egg-info/top_level.txt
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      703 2024-04-12 07:28:54.593051 seacrowd-0.0.6/setup.cfg
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)       68 2024-04-12 07:28:29.000000 seacrowd-0.0.6/setup.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:28:54.541365 seacrowd-0.0.6/tests/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:52.000000 seacrowd-0.0.6/tests/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    23314 2024-04-04 06:00:52.000000 seacrowd-0.0.6/tests/test_seacrowd.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    20714 2024-04-04 06:00:52.000000 seacrowd-0.0.6/tests/test_seacrowd_source_only.py
```

### Comparing `seacrowd-0.0.5/LICENSE` & `seacrowd-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/PKG-INFO` & `seacrowd-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seacrowd
-Version: 0.0.5
+Version: 0.0.6
 Requires-Python: >=3.7
 License-File: LICENSE
 Requires-Dist: loguru>=0.5.3
 Requires-Dist: bioc>=1.3.7
 Requires-Dist: pandas>=1.3.3
 Requires-Dist: numpy>=1.20
 Requires-Dist: datasets>=2.2.0
```

### Comparing `seacrowd-0.0.5/README.md` & `seacrowd-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/config_helper.py` & `seacrowd-0.0.6/seacrowd/config_helper.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/abui_wordnet/abui_wordnet.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/abui_wordnet/abui_wordnet.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/alt_burmese_treebank/alt_burmese_treebank.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/alt_burmese_treebank/alt_burmese_treebank.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/alt_burmese_treebank/utils/alt_burmese_treebank_utils.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/alt_burmese_treebank/utils/alt_burmese_treebank_utils.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/ara_close/ara_close.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/ara_close/ara_close.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/asr_sindodusc/asr_sindodusc.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/asr_sindodusc/asr_sindodusc.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/asr_smaldusc/asr_smaldusc.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/asr_smaldusc/asr_smaldusc.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/asr_stidusc/asr_stidusc.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/asr_stidusc/asr_stidusc.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/audio_keyword_spotting/audio_keyword_spotting.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/audio_keyword_spotting/audio_keyword_spotting.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/aya_dataset/aya_dataset.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/aya_dataset/aya_dataset.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/barasa/barasa.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/barasa/barasa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/beaye_lexicon/beaye_lexicon.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/beaye_lexicon/beaye_lexicon.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/belebele/belebele.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/belebele/belebele.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/bible_en_id/bible_en_id.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/bible_en_id/bible_en_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/bible_jv_id/bible_jv_id.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/bible_jv_id/bible_jv_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/bible_su_id/bible_su_id.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/bible_su_id/bible_su_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/bioner_id/bioner_id.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/bioner_id/bioner_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/bloom_captioning/bloom_captioning.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/bloom_captioning/bloom_captioning.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/bloom_lm/bloom_lm.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/bloom_lm/bloom_lm.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/bloom_speech/bloom_speech.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/bloom_speech/bloom_speech.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/bloom_vist/bloom_vist.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/bloom_vist/bloom_vist.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/burapha_th/burapha_th.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/burapha_th/burapha_th.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/burmese_romanize/burmese_romanize.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/burmese_romanize/burmese_romanize.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/casa/casa.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/casa/casa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/cc100/cc100.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/cc100/cc100.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/cc_aligned_doc/cc_aligned_doc.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/cc_aligned_doc/cc_aligned_doc.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/cc_aligned_sent/cc_aligned_sent.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/cc_aligned_sent/cc_aligned_sent.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/cebuaner/cebuaner.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/cebuaner/cebuaner.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/coco_35l/coco_35l.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/coco_35l/coco_35l.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/cod/cod.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/cod/cod.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/code_mixed_jv_id/code_mixed_jv_id.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/code_mixed_jv_id/code_mixed_jv_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/codeswitch_reddit/codeswitch_reddit.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/codeswitch_reddit/codeswitch_reddit.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/commonvoice_120/commonvoice_120.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/commonvoice_120/commonvoice_120.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/copal/copal.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/copal/copal.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/covost2/covost2.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/covost2/covost2.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/creole_rc/creole_rc.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/creole_rc/creole_rc.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/crosssum/crosssum.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/crosssum/crosssum.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/cub_bahasa/cub_bahasa.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/cub_bahasa/cub_bahasa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/culturax/culturax.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/culturax/culturax.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/cvss/cvss.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/cvss/cvss.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/dengue_filipino/dengue_filipino.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/dengue_filipino/dengue_filipino.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/emot/emot.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/emot/emot.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/emotcmt/emotcmt.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/emotcmt/emotcmt.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/emotes_3k/emotes_3k.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/emotes_3k/emotes_3k.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/emotion_id_opinion/emotion_id_opinion.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/emotion_id_opinion/emotion_id_opinion.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/etos/etos.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/etos/etos.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/facqa/facqa.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/facqa/facqa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/facqa/utils/facqa_utils.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/facqa/utils/facqa_utils.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/fakenews_ph/fakenews_ph.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/fakenews_ph/fakenews_ph.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/filipino_gay_lang/filipino_gay_lang.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/filipino_gay_lang/filipino_gay_lang.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/filipino_hatespeech_tiktok/filipino_hatespeech_tiktok.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/filipino_hatespeech_tiktok/filipino_hatespeech_tiktok.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/filipino_slang_norm/filipino_slang_norm.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/filipino_slang_norm/filipino_slang_norm.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/filipino_words_aoa/filipino_words_aoa.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/filipino_words_aoa/filipino_words_aoa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/filwordnet/filwordnet.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/filwordnet/filwordnet.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/fleurs/fleurs.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/fleurs/fleurs.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/flores200/flores200.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/flores200/flores200.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/fsl_105/fsl_105.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/fsl_105/fsl_105.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/gatitos/gatitos.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/gatitos/gatitos.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/gklmip_newsclass/gklmip_newsclass.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/gklmip_newsclass/gklmip_newsclass.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/gklmip_sentiment/gklmip_sentiment.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/gklmip_sentiment/gklmip_sentiment.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/globalwoz/globalwoz.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/globalwoz/globalwoz.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/glotstorybook/glotstorybook.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/glotstorybook/glotstorybook.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/hoasa/hoasa.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/hoasa/hoasa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/iapp_squad/iapp_squad.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/iapp_squad/iapp_squad.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/iatf/iatf.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/iatf/iatf.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/icon/icon.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/icon/icon.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/id_abusive/id_abusive.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/id_abusive/id_abusive.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/id_abusive_news_comment/id_abusive_news_comment.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/id_abusive_news_comment/id_abusive_news_comment.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/id_am2ico/id_am2ico.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/id_am2ico/id_am2ico.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/id_clickbait/id_clickbait.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/id_clickbait/id_clickbait.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/id_coreference_resolution/id_coreference_resolution.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/id_coreference_resolution/id_coreference_resolution.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/id_frog_story/id_frog_story.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/id_frog_story/id_frog_story.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/id_google_play_review/id_google_play_review.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/id_google_play_review/id_google_play_review.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/id_hatespeech/id_hatespeech.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/id_hatespeech/id_hatespeech.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/id_hoax_news/id_hoax_news.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/id_hoax_news/id_hoax_news.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/id_hsd_nofaaulia/id_hsd_nofaaulia.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/id_hsd_nofaaulia/id_hsd_nofaaulia.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/id_msvd/id_msvd.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/id_msvd/id_msvd.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/id_multilabel_hs/id_multilabel_hs.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/id_multilabel_hs/id_multilabel_hs.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/id_panl_bppt/id_panl_bppt.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/id_panl_bppt/id_panl_bppt.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/id_qqp/id_qqp.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/id_qqp/id_qqp.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/id_sent_emo_mobile_apps/id_sent_emo_mobile_apps.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/id_sent_emo_mobile_apps/id_sent_emo_mobile_apps.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/id_sentiment_analysis/id_sentiment_analysis.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/id_sentiment_analysis/id_sentiment_analysis.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/id_short_answer_grading/id_short_answer_grading.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/id_short_answer_grading/id_short_answer_grading.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/id_short_answer_grading/utils/id_short_answer_grading_utils.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/id_short_answer_grading/utils/id_short_answer_grading_utils.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/id_stance/id_stance.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/id_stance/id_stance.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/id_sts/id_sts.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/id_sts/id_sts.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/id_vaccines_tweets/id_vaccines_tweets.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/id_vaccines_tweets/id_vaccines_tweets.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/id_wiki_parallel/id_wiki_parallel.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/id_wiki_parallel/id_wiki_parallel.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/id_wsd/id_wsd.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/id_wsd/id_wsd.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/identic/identic.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/identic/identic.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/identifikasi_bahasa/identifikasi_bahasa.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/identifikasi_bahasa/identifikasi_bahasa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/idk_mrc/idk_mrc.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/idk_mrc/idk_mrc.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/idn_tagged_corpus_csui/idn_tagged_corpus_csui.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/idn_tagged_corpus_csui/idn_tagged_corpus_csui.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/ijelid/ijelid.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/ijelid/ijelid.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/imdb_jv/imdb_jv.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/imdb_jv/imdb_jv.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/indo4b/indo4b.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/indo4b/indo4b.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/indo4b_plus/indo4b_plus.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/indo4b_plus/indo4b_plus.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/indo_general_mt_en_id/indo_general_mt_en_id.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/indo_general_mt_en_id/indo_general_mt_en_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/indo_law/indo_law.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/indo_law/indo_law.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/indo_puisi/indo_puisi.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/indo_puisi/indo_puisi.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/indo_religious_mt_en_id/indo_religious_mt_en_id.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/indo_religious_mt_en_id/indo_religious_mt_en_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/indo_story_cloze/indo_story_cloze.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/indo_story_cloze/indo_story_cloze.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/indocamrest/indocamrest.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/indocamrest/indocamrest.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/indocollex/indocollex.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/indocollex/indocollex.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/indocoref/indocoref.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/indocoref/indocoref.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/indocoref/utils/feature_utils.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/indocoref/utils/feature_utils.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/indocoref/utils/file_utils.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/indocoref/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/indocoref/utils/text_preprocess.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/indocoref/utils/text_preprocess.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/indolem_ner_ugm/indolem_ner_ugm.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/indolem_ner_ugm/indolem_ner_ugm.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/indolem_nerui/indolem_nerui.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/indolem_nerui/indolem_nerui.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/indolem_ntp/indolem_ntp.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/indolem_ntp/indolem_ntp.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/indolem_sentiment/indolem_sentiment.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/indolem_sentiment/indolem_sentiment.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/indolem_tweet_ordering/indolem_tweet_ordering.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/indolem_tweet_ordering/indolem_tweet_ordering.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/indolem_ud_id_gsd/indolem_ud_id_gsd.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/indolem_ud_id_gsd/indolem_ud_id_gsd.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/indolem_ud_id_pud/indolem_ud_id_pud.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/indolem_ud_id_pud/indolem_ud_id_pud.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/indoler/indoler.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/indoler/indoler.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/indommlu/indommlu.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/indommlu/indommlu.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/indoner_tourism/indoner_tourism.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/indoner_tourism/indoner_tourism.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/indonesia_chinese_mtrobusteval/indonesia_chinese_mtrobusteval.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/indonesia_chinese_mtrobusteval/indonesia_chinese_mtrobusteval.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/indonesian_madurese_bible_translation/indonesian_madurese_bible_translation.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/indonesian_madurese_bible_translation/indonesian_madurese_bible_translation.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/indonesian_news_dataset/indonesian_news_dataset.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/indonesian_news_dataset/indonesian_news_dataset.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/indonesiannmt/indonesiannmt.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/indonesiannmt/indonesiannmt.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/indonglish/indonglish.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/indonglish/indonglish.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/indonli/indonli.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/indonli/indonli.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/indonlu_nergrit/indonlu_nergrit.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/indonlu_nergrit/indonlu_nergrit.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/indoqa/indoqa.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/indoqa/indoqa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/indosmd/indosmd.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/indosmd/indosmd.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/indosum/indosum.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/indosum/indosum.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/indotacos/indotacos.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/indotacos/indotacos.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/indowiki/indowiki.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/indowiki/indowiki.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/indqner/indqner.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/indqner/indqner.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/indspeech_digit_cdsr/indspeech_digit_cdsr.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_digit_cdsr/indspeech_digit_cdsr.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/indspeech_news_ethnicsr/indspeech_news_ethnicsr.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_news_ethnicsr/indspeech_news_ethnicsr.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/indspeech_news_lvcsr/indspeech_news_lvcsr.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_news_lvcsr/indspeech_news_lvcsr.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/indspeech_news_tts/indspeech_news_tts.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_news_tts/indspeech_news_tts.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/indspeech_newstra_ethnicsr/indspeech_newstra_ethnicsr.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_newstra_ethnicsr/indspeech_newstra_ethnicsr.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/indspeech_teldialog_lvcsr/indspeech_teldialog_lvcsr.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_teldialog_lvcsr/indspeech_teldialog_lvcsr.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/indspeech_teldialog_svcsr/indspeech_teldialog_svcsr.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/indspeech_teldialog_svcsr/indspeech_teldialog_svcsr.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/inset_lexicon/inset_lexicon.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/inset_lexicon/inset_lexicon.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/jadi_ide/jadi_ide.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/jadi_ide/jadi_ide.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/jv_id_asr/jv_id_asr.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/jv_id_asr/jv_id_asr.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/jv_id_tts/jv_id_tts.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/jv_id_tts/jv_id_tts.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/kamus_alay/kamus_alay.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/kamus_alay/kamus_alay.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/karonese_sentiment/karonese_sentiment.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/karonese_sentiment/karonese_sentiment.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/kawat/kawat.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/kawat/kawat.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/kde4/kde4.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/kde4/kde4.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/keps/keps.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/keps/keps.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/kheng_info/kheng_info.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/kheng_info/kheng_info.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/khmer_alt_pos/khmer_alt_pos.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/khmer_alt_pos/khmer_alt_pos.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/khpos/khpos.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/khpos/khpos.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/kopi_cc/kopi_cc.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/kopi_cc/kopi_cc.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/kopi_cc_news/kopi_cc_news.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/kopi_cc_news/kopi_cc_news.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/kopi_nllb/kopi_nllb.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/kopi_nllb/kopi_nllb.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/korpus_nusantara/korpus_nusantara.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/korpus_nusantara/korpus_nusantara.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/lazada_review_filipino/lazada_review_filipino.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/lazada_review_filipino/lazada_review_filipino.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/librivox_indonesia/librivox_indonesia.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/librivox_indonesia/librivox_indonesia.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/limesoda/limesoda.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/limesoda/limesoda.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/liputan6/liputan6.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/liputan6/liputan6.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/local_id_abusive/local_id_abusive.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/local_id_abusive/local_id_abusive.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/lr_sum/lr_sum.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/lr_sum/lr_sum.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/m3exam/m3exam.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/m3exam/m3exam.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/mabl/mabl.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/mabl/mabl.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/malaysia_tweets/malaysia_tweets.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/malaysia_tweets/malaysia_tweets.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/malindo_morph/malindo_morph.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/malindo_morph/malindo_morph.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/malindo_parallel/malindo_parallel.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/malindo_parallel/malindo_parallel.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/massive/massive.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/massive/massive.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/mc4_indo/mc4_indo.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/mc4_indo/mc4_indo.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/melayu_brunei/melayu_brunei.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/melayu_brunei/melayu_brunei.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/melayu_sabah/melayu_sabah.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/melayu_sabah/melayu_sabah.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/melayu_sarawak/melayu_sarawak.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/melayu_sarawak/melayu_sarawak.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/melayu_standard_lisan/melayu_standard_lisan.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/melayu_standard_lisan/melayu_standard_lisan.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/memolon/memolon.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/memolon/memolon.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/minangnlp_mt/minangnlp_mt.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/minangnlp_mt/minangnlp_mt.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/miracl/miracl.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/miracl/miracl.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/mkqa/mkqa.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/mkqa/mkqa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/mlqa/mlqa.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/mlqa/mlqa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/mozilla_pontoon/mozilla_pontoon.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/mozilla_pontoon/mozilla_pontoon.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/mswc/mswc.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/mswc/mswc.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/mtop_intent_classification/labels.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/mtop_intent_classification/labels.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/mtop_intent_classification/mtop_intent_classification.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/mtop_intent_classification/mtop_intent_classification.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/multilexnorm/multilexnorm.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/multilexnorm/multilexnorm.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/my_paraphrase/my_paraphrase.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/my_paraphrase/my_paraphrase.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/myanmar_rakhine_parallel/myanmar_rakhine_parallel.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/myanmar_rakhine_parallel/myanmar_rakhine_parallel.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/mypos/mypos.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/mypos/mypos.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/mysentence/mysentence.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/mysentence/mysentence.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/myxnli/myxnli.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/myxnli/myxnli.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/nergrit/nergrit.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/nergrit/nergrit.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/nerp/nerp.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/nerp/nerp.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/netifier/netifier.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/netifier/netifier.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/news_en_id/news_en_id.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/news_en_id/news_en_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/newsph/newsph.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/newsph/newsph.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/nllb_seed/nllb_seed.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/nllb_seed/nllb_seed.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/ntrex_128/ntrex_128.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/ntrex_128/ntrex_128.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/nusaparagraph_emot/nusaparagraph_emot.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/nusaparagraph_emot/nusaparagraph_emot.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/nusaparagraph_rhetoric/nusaparagraph_rhetoric.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/nusaparagraph_rhetoric/nusaparagraph_rhetoric.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/nusaparagraph_topic/nusaparagraph_topic.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/nusaparagraph_topic/nusaparagraph_topic.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/nusatranslation_emot/nusatranslation_emot.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/nusatranslation_emot/nusatranslation_emot.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/nusatranslation_mt/nusatranslation_mt.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/nusatranslation_mt/nusatranslation_mt.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/nusatranslation_senti/nusatranslation_senti.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/nusatranslation_senti/nusatranslation_senti.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/nusax_mt/nusax_mt.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/nusax_mt/nusax_mt.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/nusax_senti/nusax_senti.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/nusax_senti/nusax_senti.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/oil/oil.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/oil/oil.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/ojw/ojw.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/ojw/ojw.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/openlid/openlid.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/openlid/openlid.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/openslr/openslr.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/openslr/openslr.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/orchid_pos/orchid_pos.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/orchid_pos/orchid_pos.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/oscar_2201/oscar_2201.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/oscar_2201/oscar_2201.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/palito/palito.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/palito/palito.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/paracotta_id/paracotta_id.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/paracotta_id/paracotta_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/parallel_id_nyo/parallel_id_nyo.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/parallel_id_nyo/parallel_id_nyo.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/parallel_su_id/parallel_su_id.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/parallel_su_id/parallel_su_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/ph_fake_news_corpus/ph_fake_news_corpus.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/ph_fake_news_corpus/ph_fake_news_corpus.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/pho_ner_covid/pho_ner_covid.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/pho_ner_covid/pho_ner_covid.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/phomt/phomt.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/phomt/phomt.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/phost/phost.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/phost/phost.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/posp/posp.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/posp/posp.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/postag_su/postag_su.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/postag_su/postag_su.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/prdect_id/prdect_id.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/prdect_id/prdect_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/qasina/qasina.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/qasina/qasina.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/roots_vi_ted/roots_vi_ted.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/roots_vi_ted/roots_vi_ted.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/sampiran/sampiran.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/sampiran/sampiran.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/sap_wat/sap_wat.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/sap_wat/sap_wat.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/sarawak_malay/sarawak_malay.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/sarawak_malay/sarawak_malay.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/scb_mt_en_th/scb_mt_en_th.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/scb_mt_en_th/scb_mt_en_th.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/sea_bench/sea_bench.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/sea_bench/sea_bench.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/sea_madlad/sea_madlad.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/sea_madlad/sea_madlad.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/sea_wiki/sea_wiki.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/sea_wiki/sea_wiki.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/seaeval/seaeval.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/seaeval/seaeval.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/seahorse/seahorse.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/seahorse/seahorse.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/sentiment_nathasa_review/sentiment_nathasa_review.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/sentiment_nathasa_review/sentiment_nathasa_review.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/shopee_reviews_tagalog/shopee_reviews_tagalog.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/shopee_reviews_tagalog/shopee_reviews_tagalog.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/singgalang/singgalang.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/singgalang/singgalang.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/smsa/smsa.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/smsa/smsa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/snli_indo/snli_indo.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/snli_indo/snli_indo.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/spamid_pair/spamid_pair.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/spamid_pair/spamid_pair.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/squad_id/squad_id.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/squad_id/squad_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/stb_ext/stb_ext.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/stb_ext/stb_ext.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/stif_indonesia/stif_indonesia.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/stif_indonesia/stif_indonesia.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/struct_amb_ind/struct_amb_ind.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/struct_amb_ind/struct_amb_ind.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/su_emot/su_emot.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/su_emot/su_emot.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/su_id_asr/su_id_asr.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/su_id_asr/su_id_asr.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/su_id_tts/su_id_tts.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/su_id_tts/su_id_tts.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/talpco/talpco.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/talpco/talpco.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/tatabahasa/tatabahasa.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/tatabahasa/tatabahasa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/tatoeba/tatoeba.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/tatoeba/tatoeba.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/tcope/tcope.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/tcope/tcope.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/ted_en_id/ted_en_id.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/ted_en_id/ted_en_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/term_a/term_a.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/term_a/term_a.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/tgl_profanity/tgl_profanity.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/tgl_profanity/tgl_profanity.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/tha_lao_embassy_parcor/tha_lao_embassy_parcor.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/tha_lao_embassy_parcor/tha_lao_embassy_parcor.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/thai_alpaca/thai_alpaca.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/thai_alpaca/thai_alpaca.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/thai_constitution/thai_constitution.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/thai_constitution/thai_constitution.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/thai_databricks_dolly/thai_databricks_dolly.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/thai_databricks_dolly/thai_databricks_dolly.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/thai_depression/thai_depression.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/thai_depression/thai_depression.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/thai_gpteacher/thai_gpteacher.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/thai_gpteacher/thai_gpteacher.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/thai_hh_rlhf/thai_hh_rlhf.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/thai_hh_rlhf/thai_hh_rlhf.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/thai_sum/thai_sum.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/thai_sum/thai_sum.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/thai_toxicity_tweet/thai_toxicity_tweet.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/thai_toxicity_tweet/thai_toxicity_tweet.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/tico_19/tico_19.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/tico_19/tico_19.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/titml_idn/titml_idn.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/titml_idn/titml_idn.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/tlunified_ner/tlunified_ner.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/tlunified_ner/tlunified_ner.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/toxicity_200/toxicity_200.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/toxicity_200/toxicity_200.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/tydiqa/tydiqa.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/tydiqa/tydiqa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/typhoon_yolanda_tweets/typhoon_yolanda_tweets.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/typhoon_yolanda_tweets/typhoon_yolanda_tweets.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/ucla_phonetic/ucla_phonetic.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/ucla_phonetic/ucla_phonetic.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/ud_id_csui/ud_id_csui.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/ud_id_csui/ud_id_csui.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/ud_jv_csui/ud_jv_csui.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/ud_jv_csui/ud_jv_csui.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/udhr/udhr.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/udhr/udhr.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/udhr_lid/udhr_lid.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/udhr_lid/udhr_lid.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/uit_vicov19qa/uit_vicov19qa.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/uit_vicov19qa/uit_vicov19qa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/uit_victsd/uit_victsd.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/uit_victsd/uit_victsd.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/uit_vihsd/uit_vihsd.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/uit_vihsd/uit_vihsd.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/uit_viic/uit_viic.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/uit_viic/uit_viic.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/uit_viocd/uit_viocd.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/uit_viocd/uit_viocd.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/uit_vion/uit_vion.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/uit_vion/uit_vion.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/uit_visd4sa/uit_visd4sa.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/uit_visd4sa/uit_visd4sa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/uit_vsfc/uit_vsfc.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/uit_vsfc/uit_vsfc.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/uit_vsmec/uit_vsmec.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/uit_vsmec/uit_vsmec.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/unimorph/unimorph.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/unimorph/unimorph.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/unimorph_id/unimorph_id.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/unimorph_id/unimorph_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/vi_pubmed/vi_pubmed.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/vi_pubmed/vi_pubmed.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/vihealthqa/vihealthqa.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/vihealthqa/vihealthqa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/visobert/visobert.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/visobert/visobert.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/vispamreviews/vispamreviews.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/vispamreviews/vispamreviews.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/vistec_tp_th_21/vistec_tp_th_21.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/vistec_tp_th_21/vistec_tp_th_21.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/vitext2sql/vitext2sql.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/vitext2sql/vitext2sql.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/vivos/vivos.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/vivos/vivos.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/vivqa/vivqa.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/vivqa/vivqa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/vlsp2016_ner/vlsp2016_ner.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/vlsp2016_ner/vlsp2016_ner.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/vlsp2016_sa/vlsp2016_sa.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/vlsp2016_sa/vlsp2016_sa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/vndt/utils.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/vndt/utils.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/vndt/vndt.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/vndt/vndt.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/voxlingua/voxlingua.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/voxlingua/voxlingua.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/weathub/weathub.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/weathub/weathub.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/wikiann/wikiann.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/wikiann/wikiann.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/wikilingua/wikilingua.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/wikilingua/wikilingua.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/wikimatrix/wikimatrix.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/wikimatrix/wikimatrix.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/wikitext_tl_39/wikitext_tl_39.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/wikitext_tl_39/wikitext_tl_39.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/wili_2018/wili_2018.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/wili_2018/wili_2018.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/wisesight_thai_sentiment/wisesight_thai_sentiment.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/wisesight_thai_sentiment/wisesight_thai_sentiment.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/wit/wit.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/wit/wit.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/wongnai_reviews/wongnai_reviews.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/wongnai_reviews/wongnai_reviews.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/wrete/wrete.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/wrete/wrete.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/x_fact/x_fact.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/x_fact/x_fact.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/xcopa/xcopa.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/xcopa/xcopa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/xl_jailbreak/xl_jailbreak.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/xl_jailbreak/xl_jailbreak.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/xl_sum/xl_sum.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/xl_sum/xl_sum.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/xm3600/xm3600.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/xm3600/xm3600.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/xnli/xnli.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/xnli/xnli.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/xpersona_id/xpersona_id.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/xpersona_id/xpersona_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/xquad/xquad.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/xquad/xquad.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/xsid/xsid.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/xsid/xsid.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/xstorycloze/xstorycloze.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/xstorycloze/xstorycloze.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/sea_datasets/yunshan_cup_2020/yunshan_cup_2020.py` & `seacrowd-0.0.6/seacrowd/sea_datasets/yunshan_cup_2020/yunshan_cup_2020.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/utils/common_parser.py` & `seacrowd-0.0.6/seacrowd/utils/common_parser.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/utils/constants.py` & `seacrowd-0.0.6/seacrowd/utils/constants.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/utils/schemas/__init__.py` & `seacrowd-0.0.6/seacrowd/utils/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/utils/schemas/imqa.py` & `seacrowd-0.0.6/seacrowd/utils/schemas/imqa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/utils/schemas/kb.py` & `seacrowd-0.0.6/seacrowd/utils/schemas/kb.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/utils/schemas/pairs.py` & `seacrowd-0.0.6/seacrowd/utils/schemas/pairs.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/utils/schemas/qa.py` & `seacrowd-0.0.6/seacrowd/utils/schemas/qa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/utils/schemas/seq_label.py` & `seacrowd-0.0.6/seacrowd/utils/schemas/seq_label.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/utils/schemas/speech.py` & `seacrowd-0.0.6/seacrowd/utils/schemas/speech.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/utils/schemas/speech_multilabel.py` & `seacrowd-0.0.6/seacrowd/utils/schemas/speech_multilabel.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/utils/schemas/speech_to_speech.py` & `seacrowd-0.0.6/seacrowd/utils/schemas/speech_to_speech.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/utils/schemas/tod.py` & `seacrowd-0.0.6/seacrowd/utils/schemas/tod.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/utils/schemas/tree.py` & `seacrowd-0.0.6/seacrowd/utils/schemas/tree.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd/utils/schemas/video.py` & `seacrowd-0.0.6/seacrowd/utils/schemas/video.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/seacrowd.egg-info/PKG-INFO` & `seacrowd-0.0.6/seacrowd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seacrowd
-Version: 0.0.5
+Version: 0.0.6
 Requires-Python: >=3.7
 License-File: LICENSE
 Requires-Dist: loguru>=0.5.3
 Requires-Dist: bioc>=1.3.7
 Requires-Dist: pandas>=1.3.3
 Requires-Dist: numpy>=1.20
 Requires-Dist: datasets>=2.2.0
```

### Comparing `seacrowd-0.0.5/seacrowd.egg-info/SOURCES.txt` & `seacrowd-0.0.6/seacrowd.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -114,14 +114,15 @@
 seacrowd/sea_datasets/filipino_slang_norm/filipino_slang_norm.py
 seacrowd/sea_datasets/filipino_words_aoa/__init__.py
 seacrowd/sea_datasets/filipino_words_aoa/filipino_words_aoa.py
 seacrowd/sea_datasets/filwordnet/__init__.py
 seacrowd/sea_datasets/filwordnet/filwordnet.py
 seacrowd/sea_datasets/fleurs/__init__.py
 seacrowd/sea_datasets/fleurs/fleurs.py
+seacrowd/sea_datasets/fleurs/lang_config.json
 seacrowd/sea_datasets/flores200/__init__.py
 seacrowd/sea_datasets/flores200/flores200.py
 seacrowd/sea_datasets/fsl_105/__init__.py
 seacrowd/sea_datasets/fsl_105/fsl_105.py
 seacrowd/sea_datasets/gatitos/__init__.py
 seacrowd/sea_datasets/gatitos/gatitos.py
 seacrowd/sea_datasets/gklmip_newsclass/__init__.py
@@ -454,14 +455,15 @@
 seacrowd/sea_datasets/scb_mt_en_th/__init__.py
 seacrowd/sea_datasets/scb_mt_en_th/scb_mt_en_th.py
 seacrowd/sea_datasets/sea_bench/__init__.py
 seacrowd/sea_datasets/sea_bench/sea_bench.py
 seacrowd/sea_datasets/sea_madlad/__init__.py
 seacrowd/sea_datasets/sea_madlad/sea_madlad.py
 seacrowd/sea_datasets/sea_wiki/__init__.py
+seacrowd/sea_datasets/sea_wiki/lang_config.json
 seacrowd/sea_datasets/sea_wiki/sea_wiki.py
 seacrowd/sea_datasets/seaeval/__init__.py
 seacrowd/sea_datasets/seaeval/seaeval.py
 seacrowd/sea_datasets/seahorse/__init__.py
 seacrowd/sea_datasets/seahorse/seahorse.py
 seacrowd/sea_datasets/sentiment_nathasa_review/__init__.py
 seacrowd/sea_datasets/sentiment_nathasa_review/sentiment_nathasa_review.py
```

### Comparing `seacrowd-0.0.5/tests/test_seacrowd.py` & `seacrowd-0.0.6/tests/test_seacrowd.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.5/tests/test_seacrowd_source_only.py` & `seacrowd-0.0.6/tests/test_seacrowd_source_only.py`

 * *Files identical despite different names*

