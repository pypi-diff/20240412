# Comparing `tmp/curated-tokenizers-0.9.2.tar.gz` & `tmp/curated-tokenizers-2.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curated-tokenizers-0.9.2.tar", last modified: Wed Feb  7 09:22:39 2024, max compression
+gzip compressed data, was "curated-tokenizers-2.0.0.dev0.tar", last modified: Fri Apr 12 12:15:39 2024, max compression
```

## Comparing `curated-tokenizers-0.9.2.tar` & `curated-tokenizers-2.0.0.dev0.tar`

### file list

```diff
@@ -1,236 +1,239 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-07 09:22:39.915222 curated-tokenizers-0.9.2/
--rw-r--r--   0 vsts      (1001) docker     (127)     2642 2024-02-07 09:22:13.000000 curated-tokenizers-0.9.2/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)     1960 2024-02-07 09:22:39.915222 curated-tokenizers-0.9.2/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      939 2024-02-07 09:22:13.000000 curated-tokenizers-0.9.2/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-07 09:22:39.879221 curated-tokenizers-0.9.2/curated_tokenizers/
--rw-r--r--   0 vsts      (1001) docker     (127)      120 2024-02-07 09:22:13.000000 curated-tokenizers-0.9.2/curated_tokenizers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      334 2024-02-07 09:22:13.000000 curated-tokenizers-0.9.2/curated_tokenizers/_bbpe.pxd
--rw-r--r--   0 vsts      (1001) docker     (127)     6847 2024-02-07 09:22:13.000000 curated-tokenizers-0.9.2/curated_tokenizers/_bbpe.pyx
--rw-r--r--   0 vsts      (1001) docker     (127)     2150 2024-02-07 09:22:13.000000 curated-tokenizers-0.9.2/curated_tokenizers/_spp.pxd
--rw-r--r--   0 vsts      (1001) docker     (127)     8321 2024-02-07 09:22:13.000000 curated-tokenizers-0.9.2/curated_tokenizers/_spp.pyx
--rw-r--r--   0 vsts      (1001) docker     (127)     1025 2024-02-07 09:22:13.000000 curated-tokenizers-0.9.2/curated_tokenizers/_util.py
--rw-r--r--   0 vsts      (1001) docker     (127)      655 2024-02-07 09:22:13.000000 curated-tokenizers-0.9.2/curated_tokenizers/_wordpiece.pxd
--rw-r--r--   0 vsts      (1001) docker     (127)     5250 2024-02-07 09:22:13.000000 curated-tokenizers-0.9.2/curated_tokenizers/_wordpiece.pyx
--rw-r--r--   0 vsts      (1001) docker     (127)      156 2024-02-07 09:22:13.000000 curated-tokenizers-0.9.2/curated_tokenizers/config.h
--rw-r--r--   0 vsts      (1001) docker     (127)     2126 2024-02-07 09:22:13.000000 curated-tokenizers-0.9.2/curated_tokenizers/merges.cc
--rw-r--r--   0 vsts      (1001) docker     (127)     1190 2024-02-07 09:22:13.000000 curated-tokenizers-0.9.2/curated_tokenizers/merges.hh
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-07 09:22:13.000000 curated-tokenizers-0.9.2/curated_tokenizers/py.typed
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-07 09:22:39.879221 curated-tokenizers-0.9.2/curated_tokenizers/tests/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-07 09:22:13.000000 curated-tokenizers-0.9.2/curated_tokenizers/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)       19 2024-02-07 09:22:13.000000 curated-tokenizers-0.9.2/curated_tokenizers/tests/incorrect-merges.txt
--rw-r--r--   0 vsts      (1001) docker     (127)     6291 2024-02-07 09:22:13.000000 curated-tokenizers-0.9.2/curated_tokenizers/tests/robbert-merges-1000.txt
--rw-r--r--   0 vsts      (1001) docker     (127)    16815 2024-02-07 09:22:13.000000 curated-tokenizers-0.9.2/curated_tokenizers/tests/robbert-vocab-1000.json
--rw-r--r--   0 vsts      (1001) docker     (127)     3103 2024-02-07 09:22:13.000000 curated-tokenizers-0.9.2/curated_tokenizers/tests/test_bbpe_processor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4448 2024-02-07 09:22:13.000000 curated-tokenizers-0.9.2/curated_tokenizers/tests/test_sp.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2479 2024-02-07 09:22:13.000000 curated-tokenizers-0.9.2/curated_tokenizers/tests/test_word_piece_processor.py
--rw-r--r--   0 vsts      (1001) docker     (127)       31 2024-02-07 09:22:13.000000 curated-tokenizers-0.9.2/curated_tokenizers/tests/toy-word-pieces.txt
--rw-r--r--   0 vsts      (1001) docker     (127)   253270 2024-02-07 09:22:13.000000 curated-tokenizers-0.9.2/curated_tokenizers/tests/toy.model
--rw-r--r--   0 vsts      (1001) docker     (127)      157 2024-02-07 09:22:13.000000 curated-tokenizers-0.9.2/curated_tokenizers/types.py
--rw-r--r--   0 vsts      (1001) docker     (127)      333 2024-02-07 09:22:13.000000 curated-tokenizers-0.9.2/curated_tokenizers/util.hh
--rw-r--r--   0 vsts      (1001) docker     (127)     1083 2024-02-07 09:22:13.000000 curated-tokenizers-0.9.2/curated_tokenizers/wordpiece.cc
--rw-r--r--   0 vsts      (1001) docker     (127)     1011 2024-02-07 09:22:13.000000 curated-tokenizers-0.9.2/curated_tokenizers/wordpiece.hh
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-07 09:22:39.915222 curated-tokenizers-0.9.2/curated_tokenizers.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     1960 2024-02-07 09:22:39.000000 curated-tokenizers-0.9.2/curated_tokenizers.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)    10515 2024-02-07 09:22:39.000000 curated-tokenizers-0.9.2/curated_tokenizers.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-02-07 09:22:39.000000 curated-tokenizers-0.9.2/curated_tokenizers.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       12 2024-02-07 09:22:39.000000 curated-tokenizers-0.9.2/curated_tokenizers.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       19 2024-02-07 09:22:39.000000 curated-tokenizers-0.9.2/curated_tokenizers.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-02-07 09:22:39.000000 curated-tokenizers-0.9.2/curated_tokenizers.egg-info/zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)      107 2024-02-07 09:22:13.000000 curated-tokenizers-0.9.2/pyproject.toml
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-07 09:22:39.875221 curated-tokenizers-0.9.2/sentencepiece/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-07 09:22:39.899221 curated-tokenizers-0.9.2/sentencepiece/src/
--rw-r--r--   0 vsts      (1001) docker     (127)     6596 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/bpe_model.cc
--rw-r--r--   0 vsts      (1001) docker     (127)     1748 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/bpe_model.h
--rw-r--r--   0 vsts      (1001) docker     (127)     9294 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/bpe_model_test.cc
--rw-r--r--   0 vsts      (1001) docker     (127)    11226 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/bpe_model_trainer.cc
--rw-r--r--   0 vsts      (1001) docker     (127)     4521 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/bpe_model_trainer.h
--rw-r--r--   0 vsts      (1001) docker     (127)     4850 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/bpe_model_trainer_test.cc
--rw-r--r--   0 vsts      (1001) docker     (127)    18686 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/builder.cc
--rw-r--r--   0 vsts      (1001) docker     (127)     5203 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/builder.h
--rw-r--r--   0 vsts      (1001) docker     (127)     7354 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/builder_test.cc
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-07 09:22:39.899221 curated-tokenizers-0.9.2/sentencepiece/src/builtin_pb/
--rw-r--r--   0 vsts      (1001) docker     (127)    35154 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/builtin_pb/sentencepiece.pb.cc
--rw-r--r--   0 vsts      (1001) docker     (127)    40648 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/builtin_pb/sentencepiece.pb.h
--rw-r--r--   0 vsts      (1001) docker     (127)   136631 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/builtin_pb/sentencepiece_model.pb.cc
--rw-r--r--   0 vsts      (1001) docker     (127)   200094 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/builtin_pb/sentencepiece_model.pb.h
--rw-r--r--   0 vsts      (1001) docker     (127)     1304 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/char_model.cc
--rw-r--r--   0 vsts      (1001) docker     (127)     1061 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/char_model.h
--rw-r--r--   0 vsts      (1001) docker     (127)     3525 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/char_model_test.cc
--rw-r--r--   0 vsts      (1001) docker     (127)     1782 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/char_model_trainer.cc
--rw-r--r--   0 vsts      (1001) docker     (127)     1265 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/char_model_trainer.h
--rw-r--r--   0 vsts      (1001) docker     (127)     2506 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/char_model_trainer_test.cc
--rw-r--r--   0 vsts      (1001) docker     (127)     5168 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/common.h
--rw-r--r--   0 vsts      (1001) docker     (127)     5936 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/compile_charsmap_main.cc
--rw-r--r--   0 vsts      (1001) docker     (127)     4103 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/error.cc
--rw-r--r--   0 vsts      (1001) docker     (127)     3563 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/filesystem.cc
--rw-r--r--   0 vsts      (1001) docker     (127)     1852 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/filesystem.h
--rw-r--r--   0 vsts      (1001) docker     (127)     1577 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/filesystem_test.cc
--rw-r--r--   0 vsts      (1001) docker     (127)     2605 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/freelist.h
--rw-r--r--   0 vsts      (1001) docker     (127)     1280 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/freelist_test.cc
--rw-r--r--   0 vsts      (1001) docker     (127)     1770 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/init.h
--rw-r--r--   0 vsts      (1001) docker     (127)     5359 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/init_test.cc
--rw-r--r--   0 vsts      (1001) docker     (127)     1644 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/model_factory.cc
--rw-r--r--   0 vsts      (1001) docker     (127)      972 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/model_factory.h
--rw-r--r--   0 vsts      (1001) docker     (127)     1743 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/model_factory_test.cc
--rw-r--r--   0 vsts      (1001) docker     (127)     6609 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/model_interface.cc
--rw-r--r--   0 vsts      (1001) docker     (127)     8751 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/model_interface.h
--rw-r--r--   0 vsts      (1001) docker     (127)    15351 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/model_interface_test.cc
--rw-r--r--   0 vsts      (1001) docker     (127)  7198605 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/normalization_rule.h
--rw-r--r--   0 vsts      (1001) docker     (127)    11583 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/normalizer.cc
--rw-r--r--   0 vsts      (1001) docker     (127)     5817 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/normalizer.h
--rw-r--r--   0 vsts      (1001) docker     (127)    16156 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/normalizer_test.cc
--rw-r--r--   0 vsts      (1001) docker     (127)     2132 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/pretokenizer_for_training.cc
--rw-r--r--   0 vsts      (1001) docker     (127)     2152 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/pretokenizer_for_training.h
--rw-r--r--   0 vsts      (1001) docker     (127)     2892 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/pretokenizer_for_training_test.cc
--rw-r--r--   0 vsts      (1001) docker     (127)    37639 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/sentencepiece_processor.cc
--rw-r--r--   0 vsts      (1001) docker     (127)    27254 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/sentencepiece_processor.h
--rw-r--r--   0 vsts      (1001) docker     (127)    54189 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/sentencepiece_processor_test.cc
--rw-r--r--   0 vsts      (1001) docker     (127)     9966 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/sentencepiece_trainer.cc
--rw-r--r--   0 vsts      (1001) docker     (127)     6523 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/sentencepiece_trainer.h
--rw-r--r--   0 vsts      (1001) docker     (127)    13402 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/sentencepiece_trainer_test.cc
--rw-r--r--   0 vsts      (1001) docker     (127)    10925 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/spec_parser.h
--rw-r--r--   0 vsts      (1001) docker     (127)     4037 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/spm_decode_main.cc
--rw-r--r--   0 vsts      (1001) docker     (127)     6597 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/spm_encode_main.cc
--rw-r--r--   0 vsts      (1001) docker     (127)     2083 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/spm_export_vocab_main.cc
--rw-r--r--   0 vsts      (1001) docker     (127)     4214 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/spm_normalize_main.cc
--rw-r--r--   0 vsts      (1001) docker     (127)    13036 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/spm_train_main.cc
--rw-r--r--   0 vsts      (1001) docker     (127)     1077 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/test_main.cc
--rw-r--r--   0 vsts      (1001) docker     (127)     1899 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/testharness.cc
--rw-r--r--   0 vsts      (1001) docker     (127)     8718 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/testharness.h
--rw-r--r--   0 vsts      (1001) docker     (127)     2103 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/trainer_factory.cc
--rw-r--r--   0 vsts      (1001) docker     (127)     1104 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/trainer_factory.h
--rw-r--r--   0 vsts      (1001) docker     (127)     1656 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/trainer_factory_test.cc
--rw-r--r--   0 vsts      (1001) docker     (127)    28978 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/trainer_interface.cc
--rw-r--r--   0 vsts      (1001) docker     (127)     5727 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/trainer_interface.h
--rw-r--r--   0 vsts      (1001) docker     (127)    20727 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/trainer_interface_test.cc
--rw-r--r--   0 vsts      (1001) docker     (127)     1239 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/unicode_script.cc
--rw-r--r--   0 vsts      (1001) docker     (127)     2817 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/unicode_script.h
--rw-r--r--   0 vsts      (1001) docker     (127)   106446 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/unicode_script_map.h
--rw-r--r--   0 vsts      (1001) docker     (127)     1525 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/unicode_script_test.cc
--rw-r--r--   0 vsts      (1001) docker     (127)    34126 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/unigram_model.cc
--rw-r--r--   0 vsts      (1001) docker     (127)     7324 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/unigram_model.h
--rw-r--r--   0 vsts      (1001) docker     (127)    32283 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/unigram_model_test.cc
--rw-r--r--   0 vsts      (1001) docker     (127)    22266 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/unigram_model_trainer.cc
--rw-r--r--   0 vsts      (1001) docker     (127)     4053 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/unigram_model_trainer.h
--rw-r--r--   0 vsts      (1001) docker     (127)     6752 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/unigram_model_trainer_test.cc
--rw-r--r--   0 vsts      (1001) docker     (127)     7393 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/util.cc
--rw-r--r--   0 vsts      (1001) docker     (127)    10907 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/util.h
--rw-r--r--   0 vsts      (1001) docker     (127)    12866 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/util_test.cc
--rw-r--r--   0 vsts      (1001) docker     (127)     1124 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/word_model.cc
--rw-r--r--   0 vsts      (1001) docker     (127)     1045 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/word_model.h
--rw-r--r--   0 vsts      (1001) docker     (127)     2639 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/word_model_test.cc
--rw-r--r--   0 vsts      (1001) docker     (127)     2101 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/word_model_trainer.cc
--rw-r--r--   0 vsts      (1001) docker     (127)     1372 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/word_model_trainer.h
--rw-r--r--   0 vsts      (1001) docker     (127)     2464 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/src/word_model_trainer_test.cc
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-07 09:22:39.875221 curated-tokenizers-0.9.2/sentencepiece/third_party/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-07 09:22:39.875221 curated-tokenizers-0.9.2/sentencepiece/third_party/absl/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-07 09:22:39.899221 curated-tokenizers-0.9.2/sentencepiece/third_party/absl/container/
--rw-r--r--   0 vsts      (1001) docker     (127)     1001 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/absl/container/flat_hash_map.h
--rw-r--r--   0 vsts      (1001) docker     (127)      966 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/absl/container/flat_hash_set.h
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-07 09:22:39.903221 curated-tokenizers-0.9.2/sentencepiece/third_party/absl/flags/
--rw-r--r--   0 vsts      (1001) docker     (127)     5857 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/absl/flags/flag.cc
--rw-r--r--   0 vsts      (1001) docker     (127)     1745 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/absl/flags/flag.h
--rw-r--r--   0 vsts      (1001) docker     (127)      799 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/absl/flags/parse.h
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-07 09:22:39.903221 curated-tokenizers-0.9.2/sentencepiece/third_party/absl/memory/
--rw-r--r--   0 vsts      (1001) docker     (127)     2592 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/absl/memory/memory.h
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-07 09:22:39.903221 curated-tokenizers-0.9.2/sentencepiece/third_party/absl/random/
--rw-r--r--   0 vsts      (1001) docker     (127)      959 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/absl/random/distributions.h
--rw-r--r--   0 vsts      (1001) docker     (127)      926 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/absl/random/random.h
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-07 09:22:39.903221 curated-tokenizers-0.9.2/sentencepiece/third_party/absl/strings/
--rw-r--r--   0 vsts      (1001) docker     (127)     1309 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/absl/strings/ascii.h
--rw-r--r--   0 vsts      (1001) docker     (127)     1308 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/absl/strings/match.h
--rw-r--r--   0 vsts      (1001) docker     (127)     1012 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/absl/strings/numbers.h
--rw-r--r--   0 vsts      (1001) docker     (127)     1447 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/absl/strings/str_cat.h
--rw-r--r--   0 vsts      (1001) docker     (127)     1088 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/absl/strings/str_format.h
--rw-r--r--   0 vsts      (1001) docker     (127)     2413 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/absl/strings/str_join.h
--rw-r--r--   0 vsts      (1001) docker     (127)     2127 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/absl/strings/str_replace.h
--rw-r--r--   0 vsts      (1001) docker     (127)     2669 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/absl/strings/str_split.h
--rw-r--r--   0 vsts      (1001) docker     (127)     2106 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/absl/strings/string_view.h
--rw-r--r--   0 vsts      (1001) docker     (127)      991 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/absl/strings/strip.h
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-07 09:22:39.903221 curated-tokenizers-0.9.2/sentencepiece/third_party/darts_clone/
--rw-r--r--   0 vsts      (1001) docker     (127)    51750 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/darts_clone/darts.h
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-07 09:22:39.907221 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/
--rw-r--r--   0 vsts      (1001) docker     (127)    15726 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/arena.cc
--rw-r--r--   0 vsts      (1001) docker     (127)     8985 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/arenastring.cc
--rw-r--r--   0 vsts      (1001) docker     (127)     5975 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/bytestream.cc
--rw-r--r--   0 vsts      (1001) docker     (127)    30847 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/coded_stream.cc
--rw-r--r--   0 vsts      (1001) docker     (127)    10999 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/common.cc
--rw-r--r--   0 vsts      (1001) docker     (127)    82338 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/extension_set.cc
--rw-r--r--   0 vsts      (1001) docker     (127)     3573 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/generated_enum_util.cc
--rw-r--r--   0 vsts      (1001) docker     (127)     4441 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/generated_message_table_driven_lite.cc
--rw-r--r--   0 vsts      (1001) docker     (127)    30000 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/generated_message_util.cc
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-07 09:22:39.875221 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-07 09:22:39.911221 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/
--rw-r--r--   0 vsts      (1001) docker     (127)     6215 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/any.h
--rw-r--r--   0 vsts      (1001) docker     (127)    29756 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/arena.h
--rw-r--r--   0 vsts      (1001) docker     (127)    18092 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/arena_impl.h
--rw-r--r--   0 vsts      (1001) docker     (127)    15918 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/arenastring.h
--rw-r--r--   0 vsts      (1001) docker     (127)    96637 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/descriptor.h
--rw-r--r--   0 vsts      (1001) docker     (127)    78585 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set.h
--rw-r--r--   0 vsts      (1001) docker     (127)    12437 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set_inl.h
--rw-r--r--   0 vsts      (1001) docker     (127)     3993 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_reflection.h
--rw-r--r--   0 vsts      (1001) docker     (127)     3266 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_util.h
--rw-r--r--   0 vsts      (1001) docker     (127)    12532 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven.h
--rw-r--r--   0 vsts      (1001) docker     (127)    31313 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven_lite.h
--rw-r--r--   0 vsts      (1001) docker     (127)    10023 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_util.h
--rw-r--r--   0 vsts      (1001) docker     (127)     3542 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/has_bits.h
--rw-r--r--   0 vsts      (1001) docker     (127)     7024 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/implicit_weak_message.h
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-07 09:22:39.911221 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/io/
--rw-r--r--   0 vsts      (1001) docker     (127)    69376 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/io/coded_stream.h
--rw-r--r--   0 vsts      (1001) docker     (127)     5384 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/io/io_win32.h
--rw-r--r--   0 vsts      (1001) docker     (127)    10258 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream.h
--rw-r--r--   0 vsts      (1001) docker     (127)    12750 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl.h
--rw-r--r--   0 vsts      (1001) docker     (127)    16950 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl_lite.h
--rw-r--r--   0 vsts      (1001) docker     (127)    48107 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/map.h
--rw-r--r--   0 vsts      (1001) docker     (127)    24921 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/map_entry_lite.h
--rw-r--r--   0 vsts      (1001) docker     (127)     7104 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/map_field_lite.h
--rw-r--r--   0 vsts      (1001) docker     (127)    31973 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/map_type_handler.h
--rw-r--r--   0 vsts      (1001) docker     (127)    27172 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/message_lite.h
--rw-r--r--   0 vsts      (1001) docker     (127)     8270 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/metadata_lite.h
--rw-r--r--   0 vsts      (1001) docker     (127)    32754 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/parse_context.h
--rw-r--r--   0 vsts      (1001) docker     (127)     2050 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/port.h
--rw-r--r--   0 vsts      (1001) docker     (127)    20834 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/port_def.inc
--rw-r--r--   0 vsts      (1001) docker     (127)     4209 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/port_undef.inc
--rw-r--r--   0 vsts      (1001) docker     (127)   101600 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/repeated_field.h
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-07 09:22:39.915222 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/
--rw-r--r--   0 vsts      (1001) docker     (127)    11769 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/bytestream.h
--rw-r--r--   0 vsts      (1001) docker     (127)    17098 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/callback.h
--rw-r--r--   0 vsts      (1001) docker     (127)     5733 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/casts.h
--rw-r--r--   0 vsts      (1001) docker     (127)     7283 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/common.h
--rw-r--r--   0 vsts      (1001) docker     (127)     3911 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/hash.h
--rw-r--r--   0 vsts      (1001) docker     (127)    11971 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/int128.h
--rw-r--r--   0 vsts      (1001) docker     (127)     8915 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/logging.h
--rw-r--r--   0 vsts      (1001) docker     (127)     4903 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/macros.h
--rw-r--r--   0 vsts      (1001) docker     (127)    31213 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/map_util.h
--rw-r--r--   0 vsts      (1001) docker     (127)     6157 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/mutex.h
--rw-r--r--   0 vsts      (1001) docker     (127)     2184 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/once.h
--rw-r--r--   0 vsts      (1001) docker     (127)     5108 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/platform_macros.h
--rw-r--r--   0 vsts      (1001) docker     (127)    12765 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/port.h
--rw-r--r--   0 vsts      (1001) docker     (127)     3949 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/status.h
--rw-r--r--   0 vsts      (1001) docker     (127)     8558 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/statusor.h
--rw-r--r--   0 vsts      (1001) docker     (127)     3293 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stl_util.h
--rw-r--r--   0 vsts      (1001) docker     (127)    17861 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringpiece.h
--rw-r--r--   0 vsts      (1001) docker     (127)     3615 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringprintf.h
--rw-r--r--   0 vsts      (1001) docker     (127)    39629 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/strutil.h
--rw-r--r--   0 vsts      (1001) docker     (127)     3356 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/time.h
--rw-r--r--   0 vsts      (1001) docker     (127)    14401 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/unknown_field_set.h
--rw-r--r--   0 vsts      (1001) docker     (127)    83648 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/wire_format_lite.h
--rw-r--r--   0 vsts      (1001) docker     (127)     2756 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/implicit_weak_message.cc
--rw-r--r--   0 vsts      (1001) docker     (127)     6587 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/int128.cc
--rw-r--r--   0 vsts      (1001) docker     (127)    13526 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/io_win32.cc
--rw-r--r--   0 vsts      (1001) docker     (127)    20751 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/message_lite.cc
--rw-r--r--   0 vsts      (1001) docker     (127)    20703 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/parse_context.cc
--rw-r--r--   0 vsts      (1001) docker     (127)     5500 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/repeated_field.cc
--rw-r--r--   0 vsts      (1001) docker     (127)     4197 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/status.cc
--rw-r--r--   0 vsts      (1001) docker     (127)     2096 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/statusor.cc
--rw-r--r--   0 vsts      (1001) docker     (127)     9193 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/stringpiece.cc
--rw-r--r--   0 vsts      (1001) docker     (127)     6283 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/stringprintf.cc
--rw-r--r--   0 vsts      (1001) docker     (127)    26415 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/structurally_valid.cc
--rw-r--r--   0 vsts      (1001) docker     (127)    88575 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/strutil.cc
--rw-r--r--   0 vsts      (1001) docker     (127)    10168 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/time.cc
--rw-r--r--   0 vsts      (1001) docker     (127)    27892 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/wire_format_lite.cc
--rw-r--r--   0 vsts      (1001) docker     (127)     2392 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/zero_copy_stream.cc
--rw-r--r--   0 vsts      (1001) docker     (127)    11345 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl.cc
--rw-r--r--   0 vsts      (1001) docker     (127)    13255 2024-02-07 09:22:18.000000 curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl_lite.cc
--rw-r--r--   0 vsts      (1001) docker     (127)     1238 2024-02-07 09:22:39.915222 curated-tokenizers-0.9.2/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (127)     5144 2024-02-07 09:22:13.000000 curated-tokenizers-0.9.2/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 12:15:39.259081 curated-tokenizers-2.0.0.dev0/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2642 2024-04-12 12:15:25.000000 curated-tokenizers-2.0.0.dev0/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)     1915 2024-04-12 12:15:39.259081 curated-tokenizers-2.0.0.dev0/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      939 2024-04-12 12:15:25.000000 curated-tokenizers-2.0.0.dev0/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 12:15:39.223080 curated-tokenizers-2.0.0.dev0/curated_tokenizers/
+-rw-r--r--   0 vsts      (1001) docker     (127)      120 2024-04-12 12:15:25.000000 curated-tokenizers-2.0.0.dev0/curated_tokenizers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      347 2024-04-12 12:15:25.000000 curated-tokenizers-2.0.0.dev0/curated_tokenizers/_bbpe.pxd
+-rw-r--r--   0 vsts      (1001) docker     (127)     7537 2024-04-12 12:15:25.000000 curated-tokenizers-2.0.0.dev0/curated_tokenizers/_bbpe.pyx
+-rw-r--r--   0 vsts      (1001) docker     (127)     2150 2024-04-12 12:15:25.000000 curated-tokenizers-2.0.0.dev0/curated_tokenizers/_spp.pxd
+-rw-r--r--   0 vsts      (1001) docker     (127)     8321 2024-04-12 12:15:25.000000 curated-tokenizers-2.0.0.dev0/curated_tokenizers/_spp.pyx
+-rw-r--r--   0 vsts      (1001) docker     (127)     1025 2024-04-12 12:15:25.000000 curated-tokenizers-2.0.0.dev0/curated_tokenizers/_util.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      655 2024-04-12 12:15:25.000000 curated-tokenizers-2.0.0.dev0/curated_tokenizers/_wordpiece.pxd
+-rw-r--r--   0 vsts      (1001) docker     (127)     5250 2024-04-12 12:15:25.000000 curated-tokenizers-2.0.0.dev0/curated_tokenizers/_wordpiece.pyx
+-rw-r--r--   0 vsts      (1001) docker     (127)      156 2024-04-12 12:15:25.000000 curated-tokenizers-2.0.0.dev0/curated_tokenizers/config.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     2145 2024-04-12 12:15:25.000000 curated-tokenizers-2.0.0.dev0/curated_tokenizers/merges.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)     1287 2024-04-12 12:15:25.000000 curated-tokenizers-2.0.0.dev0/curated_tokenizers/merges.hh
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 12:15:25.000000 curated-tokenizers-2.0.0.dev0/curated_tokenizers/py.typed
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 12:15:39.227080 curated-tokenizers-2.0.0.dev0/curated_tokenizers/tests/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 12:15:25.000000 curated-tokenizers-2.0.0.dev0/curated_tokenizers/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      159 2024-04-12 12:15:25.000000 curated-tokenizers-2.0.0.dev0/curated_tokenizers/tests/compat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1114 2024-04-12 12:15:25.000000 curated-tokenizers-2.0.0.dev0/curated_tokenizers/tests/conftest.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       19 2024-04-12 12:15:25.000000 curated-tokenizers-2.0.0.dev0/curated_tokenizers/tests/incorrect-merges.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)     6291 2024-04-12 12:15:25.000000 curated-tokenizers-2.0.0.dev0/curated_tokenizers/tests/robbert-merges-1000.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)    16815 2024-04-12 12:15:25.000000 curated-tokenizers-2.0.0.dev0/curated_tokenizers/tests/robbert-vocab-1000.json
+-rw-r--r--   0 vsts      (1001) docker     (127)     3858 2024-04-12 12:15:25.000000 curated-tokenizers-2.0.0.dev0/curated_tokenizers/tests/test_bbpe_processor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4448 2024-04-12 12:15:25.000000 curated-tokenizers-2.0.0.dev0/curated_tokenizers/tests/test_sp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2479 2024-04-12 12:15:25.000000 curated-tokenizers-2.0.0.dev0/curated_tokenizers/tests/test_word_piece_processor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       31 2024-04-12 12:15:25.000000 curated-tokenizers-2.0.0.dev0/curated_tokenizers/tests/toy-word-pieces.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)   253270 2024-04-12 12:15:25.000000 curated-tokenizers-2.0.0.dev0/curated_tokenizers/tests/toy.model
+-rw-r--r--   0 vsts      (1001) docker     (127)    69708 2024-04-12 12:15:25.000000 curated-tokenizers-2.0.0.dev0/curated_tokenizers/tests/troonrede.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      157 2024-04-12 12:15:25.000000 curated-tokenizers-2.0.0.dev0/curated_tokenizers/types.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      333 2024-04-12 12:15:25.000000 curated-tokenizers-2.0.0.dev0/curated_tokenizers/util.hh
+-rw-r--r--   0 vsts      (1001) docker     (127)     1083 2024-04-12 12:15:25.000000 curated-tokenizers-2.0.0.dev0/curated_tokenizers/wordpiece.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)     1011 2024-04-12 12:15:25.000000 curated-tokenizers-2.0.0.dev0/curated_tokenizers/wordpiece.hh
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 12:15:39.259081 curated-tokenizers-2.0.0.dev0/curated_tokenizers.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1915 2024-04-12 12:15:39.000000 curated-tokenizers-2.0.0.dev0/curated_tokenizers.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)    10626 2024-04-12 12:15:39.000000 curated-tokenizers-2.0.0.dev0/curated_tokenizers.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-12 12:15:39.000000 curated-tokenizers-2.0.0.dev0/curated_tokenizers.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       12 2024-04-12 12:15:39.000000 curated-tokenizers-2.0.0.dev0/curated_tokenizers.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       19 2024-04-12 12:15:39.000000 curated-tokenizers-2.0.0.dev0/curated_tokenizers.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-12 12:15:38.000000 curated-tokenizers-2.0.0.dev0/curated_tokenizers.egg-info/zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)      107 2024-04-12 12:15:25.000000 curated-tokenizers-2.0.0.dev0/pyproject.toml
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 12:15:39.219080 curated-tokenizers-2.0.0.dev0/sentencepiece/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 12:15:39.243081 curated-tokenizers-2.0.0.dev0/sentencepiece/src/
+-rw-r--r--   0 vsts      (1001) docker     (127)     6596 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/bpe_model.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)     1748 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/bpe_model.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     9294 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/bpe_model_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)    11226 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/bpe_model_trainer.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)     4521 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/bpe_model_trainer.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     4850 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/bpe_model_trainer_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)    18686 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/builder.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)     5203 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/builder.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     7354 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/builder_test.cc
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 12:15:39.243081 curated-tokenizers-2.0.0.dev0/sentencepiece/src/builtin_pb/
+-rw-r--r--   0 vsts      (1001) docker     (127)    35154 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/builtin_pb/sentencepiece.pb.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)    40648 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/builtin_pb/sentencepiece.pb.h
+-rw-r--r--   0 vsts      (1001) docker     (127)   136631 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/builtin_pb/sentencepiece_model.pb.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)   200094 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/builtin_pb/sentencepiece_model.pb.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     1304 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/char_model.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)     1061 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/char_model.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     3525 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/char_model_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)     1782 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/char_model_trainer.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)     1265 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/char_model_trainer.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     2506 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/char_model_trainer_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)     5168 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/common.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     5936 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/compile_charsmap_main.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)     4103 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/error.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)     3563 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/filesystem.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)     1852 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/filesystem.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     1577 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/filesystem_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)     2605 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/freelist.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     1280 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/freelist_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)     1770 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/init.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     5359 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/init_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)     1644 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/model_factory.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)      972 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/model_factory.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     1743 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/model_factory_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)     6609 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/model_interface.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)     8751 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/model_interface.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    15351 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/model_interface_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)  7198605 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/normalization_rule.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    11583 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/normalizer.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)     5817 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/normalizer.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    16156 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/normalizer_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)     2132 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/pretokenizer_for_training.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)     2152 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/pretokenizer_for_training.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     2892 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/pretokenizer_for_training_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)    37639 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/sentencepiece_processor.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)    27254 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/sentencepiece_processor.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    54189 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/sentencepiece_processor_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)     9966 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/sentencepiece_trainer.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)     6523 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/sentencepiece_trainer.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    13402 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/sentencepiece_trainer_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)    10925 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/spec_parser.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     4037 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/spm_decode_main.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)     6597 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/spm_encode_main.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)     2083 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/spm_export_vocab_main.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)     4214 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/spm_normalize_main.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)    13036 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/spm_train_main.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)     1077 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/test_main.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)     1899 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/testharness.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)     8718 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/testharness.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     2103 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/trainer_factory.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)     1104 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/trainer_factory.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     1656 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/trainer_factory_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)    28978 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/trainer_interface.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)     5727 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/trainer_interface.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    20727 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/trainer_interface_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)     1239 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/unicode_script.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)     2817 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/unicode_script.h
+-rw-r--r--   0 vsts      (1001) docker     (127)   106446 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/unicode_script_map.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     1525 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/unicode_script_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)    34126 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/unigram_model.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)     7324 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/unigram_model.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    32283 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/unigram_model_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)    22266 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/unigram_model_trainer.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)     4053 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/unigram_model_trainer.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     6752 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/unigram_model_trainer_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)     7393 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/util.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)    10907 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/util.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    12866 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/util_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)     1124 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/word_model.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)     1045 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/word_model.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     2639 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/word_model_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)     2101 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/word_model_trainer.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)     1372 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/word_model_trainer.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     2464 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/src/word_model_trainer_test.cc
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 12:15:39.219080 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 12:15:39.219080 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/absl/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 12:15:39.243081 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/absl/container/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1001 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/absl/container/flat_hash_map.h
+-rw-r--r--   0 vsts      (1001) docker     (127)      966 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/absl/container/flat_hash_set.h
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 12:15:39.243081 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/absl/flags/
+-rw-r--r--   0 vsts      (1001) docker     (127)     5857 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/absl/flags/flag.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)     1745 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/absl/flags/flag.h
+-rw-r--r--   0 vsts      (1001) docker     (127)      799 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/absl/flags/parse.h
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 12:15:39.243081 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/absl/memory/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2592 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/absl/memory/memory.h
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 12:15:39.243081 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/absl/random/
+-rw-r--r--   0 vsts      (1001) docker     (127)      959 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/absl/random/distributions.h
+-rw-r--r--   0 vsts      (1001) docker     (127)      926 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/absl/random/random.h
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 12:15:39.247081 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/absl/strings/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1309 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/absl/strings/ascii.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     1308 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/absl/strings/match.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     1012 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/absl/strings/numbers.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     1447 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/absl/strings/str_cat.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     1088 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/absl/strings/str_format.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     2413 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/absl/strings/str_join.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     2127 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/absl/strings/str_replace.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     2669 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/absl/strings/str_split.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     2106 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/absl/strings/string_view.h
+-rw-r--r--   0 vsts      (1001) docker     (127)      991 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/absl/strings/strip.h
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 12:15:39.247081 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/darts_clone/
+-rw-r--r--   0 vsts      (1001) docker     (127)    51750 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/darts_clone/darts.h
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 12:15:39.251081 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/
+-rw-r--r--   0 vsts      (1001) docker     (127)    15726 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/arena.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)     8985 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/arenastring.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)     5975 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/bytestream.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)    30847 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/coded_stream.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)    10999 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/common.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)    82338 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/extension_set.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)     3573 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/generated_enum_util.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)     4441 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/generated_message_table_driven_lite.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)    30000 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/generated_message_util.cc
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 12:15:39.219080 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 12:15:39.255081 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/
+-rw-r--r--   0 vsts      (1001) docker     (127)     6215 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/any.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    29756 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/arena.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    18092 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/arena_impl.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    15918 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/arenastring.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    96637 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/descriptor.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    78585 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    12437 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set_inl.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     3993 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_reflection.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     3266 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_util.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    12532 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    31313 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven_lite.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    10023 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_util.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     3542 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/has_bits.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     7024 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/implicit_weak_message.h
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 12:15:39.255081 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/io/
+-rw-r--r--   0 vsts      (1001) docker     (127)    69376 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/io/coded_stream.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     5384 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/io/io_win32.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    10258 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    12750 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    16950 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl_lite.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    48107 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/map.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    24921 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/map_entry_lite.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     7104 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/map_field_lite.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    31973 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/map_type_handler.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    27172 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/message_lite.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     8270 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/metadata_lite.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    32754 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/parse_context.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     2050 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/port.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    20834 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/port_def.inc
+-rw-r--r--   0 vsts      (1001) docker     (127)     4209 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/port_undef.inc
+-rw-r--r--   0 vsts      (1001) docker     (127)   101600 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/repeated_field.h
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 12:15:39.259081 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/
+-rw-r--r--   0 vsts      (1001) docker     (127)    11769 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/bytestream.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    17098 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/callback.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     5733 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/casts.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     7283 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/common.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     3911 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/hash.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    11971 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/int128.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     8915 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/logging.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     4903 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/macros.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    31213 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/map_util.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     6157 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/mutex.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     2184 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/once.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     5108 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/platform_macros.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    12765 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/port.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     3949 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/status.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     8558 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/statusor.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     3293 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stl_util.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    17861 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringpiece.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     3615 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringprintf.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    39629 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/strutil.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     3356 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/time.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    14401 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/unknown_field_set.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    83648 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/wire_format_lite.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     2756 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/implicit_weak_message.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)     6587 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/int128.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)    13526 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/io_win32.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)    20751 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/message_lite.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)    20703 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/parse_context.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)     5500 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/repeated_field.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)     4197 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/status.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)     2096 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/statusor.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)     9193 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/stringpiece.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)     6283 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/stringprintf.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)    26415 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/structurally_valid.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)    88575 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/strutil.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)    10168 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/time.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)    27892 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/wire_format_lite.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)     2392 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/zero_copy_stream.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)    11345 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)    13255 2024-04-12 12:15:29.000000 curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl_lite.cc
+-rw-r--r--   0 vsts      (1001) docker     (127)     1204 2024-04-12 12:15:39.259081 curated-tokenizers-2.0.0.dev0/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     5138 2024-04-12 12:15:25.000000 curated-tokenizers-2.0.0.dev0/setup.py
```

### Comparing `curated-tokenizers-0.9.2/LICENSE` & `curated-tokenizers-2.0.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/PKG-INFO` & `curated-tokenizers-2.0.0.dev0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: curated-tokenizers
-Version: 0.9.2
+Version: 2.0.0.dev0
 Summary: Lightweight piece tokenization library
 Home-page: https://github.com/explosion/curated-tokenizers
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: regex>=2022
 
 # 🥢 Curated Tokenizers
 
 This Python library provides word-/sentencepiece tokenizers. The following
```

### Comparing `curated-tokenizers-0.9.2/README.md` & `curated-tokenizers-2.0.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/curated_tokenizers/_bbpe.pyx` & `curated-tokenizers-2.0.0.dev0/curated_tokenizers/_bbpe.pyx`

 * *Files 6% similar despite different names*

```diff
@@ -47,34 +47,40 @@
     cs = bs[:]
     n = 0
     for b in range(2**8):
         if b not in bs:
             bs.append(b)
             cs.append(2**8 + n)
             n += 1
-    cs = [chr(n).encode("utf-8") for n in cs]
+    cs = [chr(n) for n in cs]
     return dict(zip(bs, cs))
 
 cdef class ByteBPEProcessor:
     cdef shared_ptr[Merges] _merges
     cdef dict _byte_decoder
     cdef dict _byte_encoder
     cdef object _split_pattern
     cdef dict _piece_to_id
     cdef dict _id_to_piece
 
     def __init__(self, vocab: Dict[str, int], merges: List[Tuple[str, str]]):
         self._byte_encoder = bytes_to_unicode()
-        self._byte_decoder = {v.decode("utf-8"): k for k, v in self._byte_encoder.items()}
+        self._byte_decoder = {v: k for k, v in self._byte_encoder.items()}
         self._split_pattern = regex.compile(SPLIT_PATTERN)
         self._piece_to_id = vocab
         self._id_to_piece = {v: k for k, v in vocab.items()}
-        cdef vector[pair[string, string]] c_merges
+        cdef vector[Merge] c_merges
+        cdef Merge merge
         for p1, p2 in merges:
-            c_merges.push_back(pair[string, string](p1.encode('utf-8'), p2.encode('utf-8')))
+            merge.merge = pair[int, int](vocab[p1], vocab[p2])
+            try:
+                merge.merged_id = vocab[p1 + p2]
+            except KeyError:
+                raise ValueError(f"Merge of '{p1}' and '{p2}' not in vocabulary")
+            c_merges.push_back(merge)
         self._merges = make_shared[Merges](c_merges)
 
     def __copy__(self):
         return ByteBPEProcessor(vocab=self.vocab, merges=self.merges)
 
     def __deepcopy__(self, memo):
         # We don't need a deepcopy of the vocab and merges dicts as their
@@ -132,50 +138,67 @@
     def encode_as_ids(self, text: str) -> List[int]:
         """
         Split a text into pieces, returning piece identifiers.
 
             text: The text to split.
             RETURNS: Piece identifiers.
         """
-        pieces = self.encode_as_pieces(text)
-        return self._pieces_to_ids(pieces)
+        ids = []
+        for token in regex.findall(self._split_pattern, text):
+            ids.extend(self._encode_token_as_ids(token))
+        return ids
 
     def encode_as_pieces(self, text: str) -> List[str]:
         """
         Split a text into pieces, returning piece pieces.
 
             text: The text to split.
             RETURNS: Piece pieces.
         """
-        pieces = []
-        for token in regex.findall(self._split_pattern, text):
-            token_bytes = [self._byte_encoder[b] for b in token.encode("utf-8")]
-            merged = deref(self._merges).apply_merges(token_bytes)
-            pieces.extend(merge.decode("utf-8") for merge in merged)
-        return pieces
+        ids = self.encode_as_ids(text)
+        return self._ids_to_pieces(ids)
+
+    @lru_cache(maxsize=8192)
+    def _encode_token_as_ids(self, token: str) -> List[str]:
+            try:
+                byte_ids = [self._piece_to_id[self._byte_encoder[b]] for b in token.encode("utf-8")]
+            except KeyError as e:
+                raise ValueError(f"Vocabulary does not contain byte '{e.args[0]}'")
+            return deref(self._merges).apply_merges(byte_ids)
+
 
     @property
     def merges(self) -> List[Tuple[str, str]]:
         """Get all merges."""
-        merges_bytes = deref(self._merges).merges()
-        return [(m1.decode('utf-8'), m2.decode('utf-8')) for m1, m2 in merges_bytes]
+        merges_ids = deref(self._merges).merges()
+        return [(self._id_to_piece[m1], self._id_to_piece[m2]) for m1, m2 in merges_ids]
 
     def piece_to_id(self, piece: str) -> Optional[int]:
         """Get the identifier for a piece."""
         return self._piece_to_id.get(piece)
 
     def id_to_piece(self, piece_id: int) -> Optional[str]:
         """Get the piece for an identifier."""
         return self._id_to_piece.get(piece_id)
 
     @property
     def vocab(self) -> Dict[str, int]:
         """Get a copy of the vocabulary."""
         return dict(self._piece_to_id)
 
+    def _ids_to_pieces(self, ids):
+        pieces = []
+        for piece_id in ids:
+            piece = self._id_to_piece.get(piece_id)
+            if piece is None:
+                raise ValueError(f"Piece identifier is not in vocabulary: {piece_id}")
+            pieces.append(piece)
+
+        return pieces
+
     def _pieces_to_ids(self, pieces):
         piece_ids = []
         for piece in pieces:
             piece_id = self._piece_to_id.get(piece)
             if piece_id is None:
                 raise ValueError(f"Piece is not in vocabulary: {piece}")
             piece_ids.append(piece_id)
```

### Comparing `curated-tokenizers-0.9.2/curated_tokenizers/_spp.pxd` & `curated-tokenizers-2.0.0.dev0/curated_tokenizers/_spp.pxd`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/curated_tokenizers/_spp.pyx` & `curated-tokenizers-2.0.0.dev0/curated_tokenizers/_spp.pyx`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/curated_tokenizers/_util.py` & `curated-tokenizers-2.0.0.dev0/curated_tokenizers/_util.py`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/curated_tokenizers/_wordpiece.pxd` & `curated-tokenizers-2.0.0.dev0/curated_tokenizers/_wordpiece.pxd`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/curated_tokenizers/_wordpiece.pyx` & `curated-tokenizers-2.0.0.dev0/curated_tokenizers/_wordpiece.pyx`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/curated_tokenizers/merges.cc` & `curated-tokenizers-2.0.0.dev0/curated_tokenizers/merges.cc`

 * *Files 20% similar despite different names*

```diff
@@ -1,75 +1,80 @@
-#include <string>
+#include <cstddef>
 #include <unordered_map>
 #include <utility>
 #include <vector>
 
 #include "merges.hh"
 
-Merges::Merges(std::vector<string_pair> const &merges) {
+Merges::Merges(std::vector<Merge> const &merges) {
     for (size_t i = 0; i < merges.size(); i++) {
-        _merges[merges[i]] = i;
+        MergeValue value;
+        value.rank = static_cast<int>(i);
+        value.merged_id = merges[i].merged_id;
+        _merges[merges[i].merge] = value;
     }
 }
 
-std::vector<std::string> Merges::apply_merges(std::vector<std::string> pieces) const {
+std::vector<int> Merges::apply_merges(std::vector<int> ids) const {
     // This function could be optimized more, e.g.:
     //
     // * Use an LRU cache for frequent inputs.
     // * Keep a priority queue of merges rather than reconstucting
     //   a pair list each iteration.
     //
     // But let's see if performance is actually an issue in practice.
 
-    while (pieces.size() != 1) {
-        auto best_pair = find_best_pair(pieces);
-        if (best_pair.first.empty() && best_pair.second.empty()) {
+    while (ids.size() != 1) {
+        auto iter = find_best_pair(ids);
+        if (iter == _merges.end()) {
             break;
         }
 
-        std::vector<std::string> new_pieces;
-        for (size_t i = 0; i < pieces.size();) {
-            if (i < pieces.size() - 1 && pieces[i] == best_pair.first && pieces[i+1] == best_pair.second) {
+        auto best_pair = iter->first;
+
+        std::vector<int> new_ids;
+        for (size_t i = 0; i < ids.size();) {
+            if (i < ids.size() - 1 && ids[i] == best_pair.first && ids[i+1] == best_pair.second) {
                 // Merge
-                new_pieces.emplace_back(pieces[i] + pieces[i + 1]);
+                new_ids.emplace_back(iter->second.merged_id);
                 i += 2;
             } else {
                 // Copy
-                new_pieces.emplace_back(pieces[i]);
+                new_ids.emplace_back(ids[i]);
                 ++i;
             }
 
         }
 
-        pieces = new_pieces;
+        ids = new_ids;
     }
     
-    return pieces;
+    return ids;
 }
 
-string_pair Merges::find_best_pair(std::vector<std::string> const &pieces) const {
-    string_pair best_pair;
+MergesMap::const_iterator Merges::find_best_pair(std::vector<int> const &ids) const {
+    auto best_iter = _merges.end();
     size_t best_rank = _merges.size();
-    for (size_t i = 0; i < pieces.size() - 1; ++i) {
-        auto cur_pair = std::make_pair(pieces[i], pieces[i + 1]);
+    for (size_t i = 0; i < ids.size() - 1; ++i) {
+        auto cur_pair = std::make_pair(ids[i], ids[i + 1]);
         auto iter = _merges.find(cur_pair);
         if (iter == _merges.end()) {
             continue;
         }
 
-        if (iter->second < best_rank) {
-            best_pair = cur_pair;
-            best_rank = iter->second;
+        if (iter->second.rank < best_rank) {
+            best_iter = iter;
+            best_rank = iter->second.rank;
         }
     }
 
-    return best_pair;
+    return best_iter;
 }
 
-std::vector<std::pair<std::string, std::string>> Merges::merges() const {
-    std::vector<std::pair<std::string, std::string>> merges(_merges.size());
+std::vector<merge_pair> Merges::merges() const {
+    std::vector<merge_pair> merges(_merges.size());
     for (auto const &merge: _merges) {
-        merges[merge.second] = merge.first;
+        merges[merge.second.rank] = merge.first;
     }
 
     return merges;
 }
```

### Comparing `curated-tokenizers-0.9.2/curated_tokenizers/tests/robbert-merges-1000.txt` & `curated-tokenizers-2.0.0.dev0/curated_tokenizers/tests/robbert-merges-1000.txt`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/curated_tokenizers/tests/robbert-vocab-1000.json` & `curated-tokenizers-2.0.0.dev0/curated_tokenizers/tests/robbert-vocab-1000.json`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/curated_tokenizers/tests/test_bbpe_processor.py` & `curated-tokenizers-2.0.0.dev0/curated_tokenizers/tests/test_word_piece_processor.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,125 +1,91 @@
-import json
 from pathlib import Path
 from pickle import dumps, loads
 
 import pytest
 
-from curated_tokenizers import ByteBPEProcessor
+from curated_tokenizers import WordPieceProcessor
+
+EXAMPLE_TOKENS = [
+    "voor",
+    "voorman",
+    "coördinatie",
+    "voorkomen",
+]
+
+EXAMPLE_ENCODINGS = [
+    ([0], ["voor"]),
+    ([0, -1], ["voor", None]),
+    ([2, 1], ["coördina", "##tie"]),
+    ([0, 3, 4], ["voor", "##kom", "##en"]),
+]
+
+EXAMPLE_DECODINGS = [
+    "voor",
+    "",  # Will raise an error.
+    "coördinatie",
+    "voorkomen",
+]
+
+TOKEN_PIECES = ["voor", "##tie", "coördina", "##kom", "##en"]
 
 
 @pytest.fixture(scope="module")
 def test_dir(request):
     return Path(request.fspath).parent
 
 
 @pytest.fixture
-def vocab_path(test_dir):
-    return test_dir / "robbert-vocab-1000.json"
+def toy_processor_from_file(test_dir):
+    return WordPieceProcessor.from_file(str(test_dir / "toy-word-pieces.txt"))
 
 
 @pytest.fixture
-def merges_path(test_dir):
-    return test_dir / "robbert-merges-1000.txt"
+def toy_processor():
+    return WordPieceProcessor(TOKEN_PIECES)
 
 
-@pytest.fixture
-def toy_processor(vocab_path, merges_path):
-    return ByteBPEProcessor.load_from_files(
-        vocab=vocab_path,
-        merges=merges_path,
-    )
-
-
-EXAMPLE_TEXT = " Wij bezoeken alle provinciën."
-EXAMPLE_PIECES = [
-    "ĠWij",
-    "Ġbez",
-    "oeken",
-    "Ġalle",
-    "Ġpro",
-    "v",
-    "in",
-    "c",
-    "iÃ«n",
-    ".",
-]
+def test_word_piece_processor_small_encode(toy_processor):
+    for token, output in zip(EXAMPLE_TOKENS, EXAMPLE_ENCODINGS):
+        y = toy_processor.encode(token)
+        assert y == output
+
+
+def test_word_piece_processor_small_decode(toy_processor):
+    for encoding, result in zip(EXAMPLE_ENCODINGS, EXAMPLE_DECODINGS):
+        if -1 in encoding[0]:
+            with pytest.raises(ValueError):
+                toy_processor.decode(encoding[0])
+        else:
+            assert toy_processor.decode(encoding[0]) == result
+
+
+def test_to_list(toy_processor):
+    assert toy_processor.to_list() == TOKEN_PIECES
+
+
+def test_from_file(toy_processor_from_file):
+    assert toy_processor_from_file.to_list() == TOKEN_PIECES
+
+
+def test_get_initial_and_id_to_piece(toy_processor):
+    assert toy_processor.get_initial("voor") == 0
+    assert toy_processor.get_initial("tie") is None
+    assert toy_processor.get_initial("##tie") is None
 
-EXAMPLE_PIECE_IDS = [280, 3377, 7095, 92, 1951, 253, 194, 311, 3698, 4]
+    assert toy_processor.id_to_piece(2) == ("coördina", True)
+    assert toy_processor.id_to_piece(1) == ("tie", False)
+    assert toy_processor.id_to_piece(999) is None
 
 
-def test_empty_processor():
-    bbpe = ByteBPEProcessor({}, [])
-    # An empty processor never merges, only recodes bytes.
-    assert bbpe.encode_as_pieces("they'll visit Köln") == [
-        "t",
-        "h",
-        "e",
-        "y",
-        "'",
-        "l",
-        "l",
-        "Ġ",
-        "v",
-        "i",
-        "s",
-        "i",
-        "t",
-        "Ġ",
-        "K",
-        "Ã",
-        "¶",
-        "l",
-        "n",
-    ]
-
-
-def test_can_decode(toy_processor):
-    assert toy_processor.decode_from_ids(EXAMPLE_PIECE_IDS) == EXAMPLE_TEXT
-
-
-def test_can_encode(toy_processor):
-    assert toy_processor.encode(EXAMPLE_TEXT) == (EXAMPLE_PIECE_IDS, EXAMPLE_PIECES)
-
-
-def test_can_encode_as_ids(toy_processor):
-    assert toy_processor.encode_as_ids(EXAMPLE_TEXT) == EXAMPLE_PIECE_IDS
-
-
-def test_can_encode_as_pieces(toy_processor):
-    assert toy_processor.encode_as_pieces(EXAMPLE_TEXT) == EXAMPLE_PIECES
-
-
-def test_rejects_incorrect_merges(test_dir):
-    with pytest.raises(ValueError, match=r"Merge must consist of 2 items"):
-        ByteBPEProcessor.load_from_files(
-            vocab=test_dir / "robbert-vocab-1000.json",
-            merges=test_dir / "incorrect-merges.txt",
-        )
-
-
-def test_id_to_piece_and_piece_to_id(toy_processor):
-    assert toy_processor.piece_to_id("woord") == 4083
-    assert toy_processor.piece_to_id("Ġwebsite") == 258
-    assert toy_processor.piece_to_id("kglw") is None
-
-    assert toy_processor.id_to_piece(207) == "ĠNederland"
-    assert toy_processor.id_to_piece(113) == "Ġdoen"
-    assert toy_processor.id_to_piece(99999) is None
-
-
-def test_can_load_from_file_object(vocab_path, merges_path):
-    with open(vocab_path, encoding="utf-8") as vocab:
-        with open(merges_path, encoding="utf-8") as merges:
-            toy_processor = ByteBPEProcessor.load_from_files(
-                vocab=vocab,
-                merges=merges,
-            )
-    assert toy_processor.encode(EXAMPLE_TEXT) == (EXAMPLE_PIECE_IDS, EXAMPLE_PIECES)
+def test_piece_id_valid(toy_processor):
+    assert toy_processor.is_valid_piece_id(-1) == False
+    assert toy_processor.is_valid_piece_id(0) == True
+    assert toy_processor.is_valid_piece_id(len(TOKEN_PIECES)) == False
+    assert toy_processor.is_valid_piece_id(len(TOKEN_PIECES) - 1) == True
 
 
 def test_pickle(toy_processor):
     serialized = dumps(toy_processor)
     deserialized = loads(serialized)
-    assert isinstance(deserialized, ByteBPEProcessor)
-    assert deserialized.vocab == toy_processor.vocab
-    assert deserialized.merges == toy_processor.merges
+    assert isinstance(deserialized, WordPieceProcessor)
+    assert deserialized.to_list() == toy_processor.to_list()
```

### Comparing `curated-tokenizers-0.9.2/curated_tokenizers/tests/test_sp.py` & `curated-tokenizers-2.0.0.dev0/curated_tokenizers/tests/test_sp.py`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/curated_tokenizers/tests/toy.model` & `curated-tokenizers-2.0.0.dev0/curated_tokenizers/tests/toy.model`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/curated_tokenizers/wordpiece.cc` & `curated-tokenizers-2.0.0.dev0/curated_tokenizers/wordpiece.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/curated_tokenizers/wordpiece.hh` & `curated-tokenizers-2.0.0.dev0/curated_tokenizers/wordpiece.hh`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/curated_tokenizers.egg-info/PKG-INFO` & `curated-tokenizers-2.0.0.dev0/curated_tokenizers.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: curated-tokenizers
-Version: 0.9.2
+Version: 2.0.0.dev0
 Summary: Lightweight piece tokenization library
 Home-page: https://github.com/explosion/curated-tokenizers
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: regex>=2022
 
 # 🥢 Curated Tokenizers
 
 This Python library provides word-/sentencepiece tokenizers. The following
```

### Comparing `curated-tokenizers-0.9.2/curated_tokenizers.egg-info/SOURCES.txt` & `curated-tokenizers-2.0.0.dev0/curated_tokenizers.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -22,22 +22,25 @@
 curated_tokenizers.egg-info/PKG-INFO
 curated_tokenizers.egg-info/SOURCES.txt
 curated_tokenizers.egg-info/dependency_links.txt
 curated_tokenizers.egg-info/requires.txt
 curated_tokenizers.egg-info/top_level.txt
 curated_tokenizers.egg-info/zip-safe
 curated_tokenizers/tests/__init__.py
+curated_tokenizers/tests/compat.py
+curated_tokenizers/tests/conftest.py
 curated_tokenizers/tests/incorrect-merges.txt
 curated_tokenizers/tests/robbert-merges-1000.txt
 curated_tokenizers/tests/robbert-vocab-1000.json
 curated_tokenizers/tests/test_bbpe_processor.py
 curated_tokenizers/tests/test_sp.py
 curated_tokenizers/tests/test_word_piece_processor.py
 curated_tokenizers/tests/toy-word-pieces.txt
 curated_tokenizers/tests/toy.model
+curated_tokenizers/tests/troonrede.txt
 sentencepiece/src/bpe_model.cc
 sentencepiece/src/bpe_model.h
 sentencepiece/src/bpe_model_test.cc
 sentencepiece/src/bpe_model_trainer.cc
 sentencepiece/src/bpe_model_trainer.h
 sentencepiece/src/bpe_model_trainer_test.cc
 sentencepiece/src/builder.cc
```

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/bpe_model.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/bpe_model.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/bpe_model.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/bpe_model.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/bpe_model_test.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/bpe_model_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/bpe_model_trainer.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/bpe_model_trainer.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/bpe_model_trainer.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/bpe_model_trainer.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/bpe_model_trainer_test.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/bpe_model_trainer_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/builder.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/builder.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/builder.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/builder.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/builder_test.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/builder_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/builtin_pb/sentencepiece.pb.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/builtin_pb/sentencepiece.pb.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/builtin_pb/sentencepiece.pb.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/builtin_pb/sentencepiece.pb.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/builtin_pb/sentencepiece_model.pb.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/builtin_pb/sentencepiece_model.pb.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/builtin_pb/sentencepiece_model.pb.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/builtin_pb/sentencepiece_model.pb.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/char_model.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/char_model.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/char_model.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/char_model.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/char_model_test.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/char_model_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/char_model_trainer.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/char_model_trainer.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/char_model_trainer.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/char_model_trainer.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/char_model_trainer_test.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/char_model_trainer_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/common.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/common.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/compile_charsmap_main.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/compile_charsmap_main.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/error.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/error.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/filesystem.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/filesystem.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/filesystem.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/filesystem.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/filesystem_test.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/filesystem_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/freelist.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/freelist.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/freelist_test.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/freelist_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/init.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/init.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/init_test.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/init_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/model_factory.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/model_factory.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/model_factory.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/model_factory.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/model_factory_test.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/model_factory_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/model_interface.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/model_interface.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/model_interface.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/model_interface.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/model_interface_test.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/model_interface_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/normalization_rule.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/normalization_rule.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/normalizer.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/normalizer.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/normalizer.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/normalizer.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/normalizer_test.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/normalizer_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/pretokenizer_for_training.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/pretokenizer_for_training.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/pretokenizer_for_training.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/pretokenizer_for_training.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/pretokenizer_for_training_test.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/pretokenizer_for_training_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/sentencepiece_processor.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/sentencepiece_processor.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/sentencepiece_processor.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/sentencepiece_processor.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/sentencepiece_processor_test.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/sentencepiece_processor_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/sentencepiece_trainer.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/sentencepiece_trainer.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/sentencepiece_trainer.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/sentencepiece_trainer.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/sentencepiece_trainer_test.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/sentencepiece_trainer_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/spec_parser.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/spec_parser.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/spm_decode_main.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/spm_decode_main.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/spm_encode_main.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/spm_encode_main.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/spm_export_vocab_main.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/spm_export_vocab_main.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/spm_normalize_main.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/spm_normalize_main.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/spm_train_main.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/spm_train_main.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/test_main.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/test_main.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/testharness.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/testharness.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/testharness.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/testharness.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/trainer_factory.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/trainer_factory.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/trainer_factory.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/trainer_factory.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/trainer_factory_test.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/trainer_factory_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/trainer_interface.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/trainer_interface.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/trainer_interface.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/trainer_interface.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/trainer_interface_test.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/trainer_interface_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/unicode_script.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/unicode_script.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/unicode_script.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/unicode_script.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/unicode_script_map.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/unicode_script_map.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/unicode_script_test.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/unicode_script_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/unigram_model.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/unigram_model.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/unigram_model.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/unigram_model.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/unigram_model_test.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/unigram_model_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/unigram_model_trainer.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/unigram_model_trainer.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/unigram_model_trainer.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/unigram_model_trainer.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/unigram_model_trainer_test.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/unigram_model_trainer_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/util.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/util.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/util.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/util.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/util_test.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/util_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/word_model.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/word_model.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/word_model.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/word_model.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/word_model_test.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/word_model_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/word_model_trainer.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/word_model_trainer.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/word_model_trainer.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/word_model_trainer.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/src/word_model_trainer_test.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/src/word_model_trainer_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/absl/container/flat_hash_map.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/absl/container/flat_hash_map.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/absl/container/flat_hash_set.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/absl/container/flat_hash_set.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/absl/flags/flag.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/absl/flags/flag.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/absl/flags/flag.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/absl/flags/flag.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/absl/flags/parse.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/absl/flags/parse.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/absl/memory/memory.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/absl/memory/memory.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/absl/random/distributions.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/absl/random/distributions.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/absl/random/random.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/absl/random/random.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/absl/strings/ascii.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/absl/strings/ascii.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/absl/strings/match.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/absl/strings/match.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/absl/strings/numbers.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/absl/strings/numbers.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/absl/strings/str_cat.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/absl/strings/str_cat.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/absl/strings/str_format.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/absl/strings/str_format.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/absl/strings/str_join.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/absl/strings/str_join.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/absl/strings/str_replace.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/absl/strings/str_replace.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/absl/strings/str_split.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/absl/strings/str_split.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/absl/strings/string_view.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/absl/strings/string_view.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/absl/strings/strip.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/absl/strings/strip.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/darts_clone/darts.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/darts_clone/darts.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/arena.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/arena.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/arenastring.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/arenastring.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/bytestream.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/bytestream.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/coded_stream.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/coded_stream.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/common.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/common.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/extension_set.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/extension_set.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/generated_enum_util.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/generated_enum_util.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/generated_message_table_driven_lite.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/generated_message_table_driven_lite.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/generated_message_util.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/generated_message_util.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/any.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/any.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/arena.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/arena.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/arena_impl.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/arena_impl.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/arenastring.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/arenastring.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/descriptor.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/descriptor.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set_inl.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set_inl.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_reflection.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_reflection.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_util.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_util.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven_lite.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven_lite.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_util.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_util.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/has_bits.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/has_bits.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/implicit_weak_message.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/implicit_weak_message.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/io/coded_stream.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/io/coded_stream.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/io/io_win32.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/io/io_win32.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl_lite.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl_lite.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/map.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/map.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/map_entry_lite.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/map_entry_lite.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/map_field_lite.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/map_field_lite.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/map_type_handler.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/map_type_handler.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/message_lite.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/message_lite.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/metadata_lite.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/metadata_lite.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/parse_context.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/parse_context.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/port.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/port.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/port_def.inc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/port_def.inc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/port_undef.inc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/port_undef.inc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/repeated_field.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/repeated_field.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/bytestream.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/bytestream.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/callback.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/callback.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/casts.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/casts.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/common.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/common.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/hash.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/hash.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/int128.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/int128.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/logging.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/logging.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/macros.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/macros.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/map_util.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/map_util.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/mutex.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/mutex.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/once.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/once.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/platform_macros.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/platform_macros.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/port.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/port.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/status.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/status.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/statusor.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/statusor.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stl_util.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stl_util.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringpiece.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringpiece.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringprintf.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringprintf.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/strutil.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/strutil.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/time.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/time.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/unknown_field_set.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/unknown_field_set.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/google/protobuf/wire_format_lite.h` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/wire_format_lite.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/implicit_weak_message.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/implicit_weak_message.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/int128.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/int128.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/io_win32.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/io_win32.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/message_lite.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/message_lite.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/parse_context.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/parse_context.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/repeated_field.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/repeated_field.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/status.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/status.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/statusor.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/statusor.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/stringpiece.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/stringpiece.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/stringprintf.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/stringprintf.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/structurally_valid.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/structurally_valid.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/strutil.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/strutil.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/time.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/time.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/wire_format_lite.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/wire_format_lite.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/zero_copy_stream.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/zero_copy_stream.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl_lite.cc` & `curated-tokenizers-2.0.0.dev0/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl_lite.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.9.2/setup.cfg` & `curated-tokenizers-2.0.0.dev0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 description = Lightweight piece tokenization library
-version = 0.9.2
+version = 2.0.0.dev0
 url = https://github.com/explosion/curated-tokenizers
 author = Explosion
 author_email = contact@explosion.ai
 license = MIT
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
@@ -12,25 +12,24 @@
 	Environment :: Console
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: MIT License
 	Operating System :: MacOS :: MacOS X
 	Programming Language :: Cython
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3.12
 	Topic :: Scientific/Engineering
 
 [options]
 zip_safe = true
 include_package_data = true
-python_requires = >=3.8
+python_requires = >=3.9
 install_requires = 
 	regex >= 2022
 
 [bdist_wheel]
 universal = false
 
 [sdist]
```

### Comparing `curated-tokenizers-0.9.2/setup.py` & `curated-tokenizers-2.0.0.dev0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,17 +12,15 @@
 Options.docstrings = True
 
 
 def prefix_path(prefix, files):
     return list(map(lambda f: f"{prefix}/{f}", files))
 
 
-ABSL_SRC = prefix_path(
-    "sentencepiece/third_party/absl", ["flags/flag.cc"]
-)
+ABSL_SRC = prefix_path("sentencepiece/third_party/absl", ["flags/flag.cc"])
 
 PROTOBUF_LIGHT_SRC = prefix_path(
     "sentencepiece/third_party/protobuf-lite",
     [
         "arena.cc",
         "arenastring.cc",
         "bytestream.cc",
```

