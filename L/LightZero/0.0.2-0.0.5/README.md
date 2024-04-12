# Comparing `tmp/LightZero-0.0.2.tar.gz` & `tmp/LightZero-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LightZero-0.0.2.tar", last modified: Sun Nov 19 12:18:05 2023, max compression
+gzip compressed data, was "LightZero-0.0.5.tar", last modified: Fri Apr 12 05:04:43 2024, max compression
```

## Comparing `LightZero-0.0.2.tar` & `LightZero-0.0.5.tar`

### file list

```diff
@@ -1,353 +1,448 @@
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.350638 LightZero-0.0.2/
--rw-r--r--   0 puyuan     (501) 453037844    11357 2023-04-14 09:11:22.000000 LightZero-0.0.2/LICENSE
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.320451 LightZero-0.0.2/LightZero.egg-info/
--rw-r--r--   0 puyuan     (501) 453037844     1004 2023-11-19 12:18:05.000000 LightZero-0.0.2/LightZero.egg-info/PKG-INFO
--rw-r--r--   0 puyuan     (501) 453037844    13229 2023-11-19 12:18:05.000000 LightZero-0.0.2/LightZero.egg-info/SOURCES.txt
--rw-r--r--   0 puyuan     (501) 453037844        1 2023-11-19 12:18:05.000000 LightZero-0.0.2/LightZero.egg-info/dependency_links.txt
--rw-r--r--   0 puyuan     (501) 453037844      715 2023-11-19 12:18:05.000000 LightZero-0.0.2/LightZero.egg-info/requires.txt
--rw-r--r--   0 puyuan     (501) 453037844       10 2023-11-19 12:18:05.000000 LightZero-0.0.2/LightZero.egg-info/top_level.txt
--rw-r--r--   0 puyuan     (501) 453037844     1004 2023-11-19 12:18:05.350539 LightZero-0.0.2/PKG-INFO
--rw-r--r--   0 puyuan     (501) 453037844    34672 2023-10-31 13:23:33.000000 LightZero-0.0.2/README.md
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.320573 LightZero-0.0.2/lzero/
--rw-r--r--   0 puyuan     (501) 453037844       52 2023-05-24 10:01:45.000000 LightZero-0.0.2/lzero/__init__.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.320859 LightZero-0.0.2/lzero/config/
--rw-r--r--   0 puyuan     (501) 453037844        0 2023-05-24 10:01:45.000000 LightZero-0.0.2/lzero/config/__init__.py
--rw-r--r--   0 puyuan     (501) 453037844      490 2023-10-10 08:13:33.000000 LightZero-0.0.2/lzero/config/meta.py
--rw-r--r--   0 puyuan     (501) 453037844      542 2023-10-10 08:13:33.000000 LightZero-0.0.2/lzero/config/utils.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.321870 LightZero-0.0.2/lzero/entry/
--rw-r--r--   0 puyuan     (501) 453037844      366 2023-11-09 09:09:19.000000 LightZero-0.0.2/lzero/entry/__init__.py
--rw-r--r--   0 puyuan     (501) 453037844     4051 2023-11-15 04:39:38.000000 LightZero-0.0.2/lzero/entry/eval_alphazero.py
--rw-r--r--   0 puyuan     (501) 453037844     4512 2023-10-10 08:13:33.000000 LightZero-0.0.2/lzero/entry/eval_muzero.py
--rw-r--r--   0 puyuan     (501) 453037844     5004 2023-05-24 10:01:45.000000 LightZero-0.0.2/lzero/entry/eval_muzero_with_gym_env.py
--rw-r--r--   0 puyuan     (501) 453037844     6324 2023-08-22 03:29:23.000000 LightZero-0.0.2/lzero/entry/train_alphazero.py
--rw-r--r--   0 puyuan     (501) 453037844     9066 2023-11-02 15:34:58.000000 LightZero-0.0.2/lzero/entry/train_muzero.py
--rw-r--r--   0 puyuan     (501) 453037844     7816 2023-10-13 09:55:49.000000 LightZero-0.0.2/lzero/entry/train_muzero_with_gym_env.py
--rw-r--r--   0 puyuan     (501) 453037844    10008 2023-10-30 04:54:58.000000 LightZero-0.0.2/lzero/entry/train_muzero_with_reward_model.py
--rw-r--r--   0 puyuan     (501) 453037844     3150 2023-10-31 13:06:51.000000 LightZero-0.0.2/lzero/entry/utils.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.322073 LightZero-0.0.2/lzero/envs/
--rw-r--r--   0 puyuan     (501) 453037844        0 2023-05-24 10:01:45.000000 LightZero-0.0.2/lzero/envs/__init__.py
--rw-r--r--   0 puyuan     (501) 453037844     1118 2023-05-24 10:01:45.000000 LightZero-0.0.2/lzero/envs/get_wrapped_env.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.322371 LightZero-0.0.2/lzero/envs/tests/
--rw-r--r--   0 puyuan     (501) 453037844        0 2023-05-24 10:01:45.000000 LightZero-0.0.2/lzero/envs/tests/__init__.py
--rw-r--r--   0 puyuan     (501) 453037844      901 2023-05-24 10:01:45.000000 LightZero-0.0.2/lzero/envs/tests/test_ding_env_wrapper.py
--rw-r--r--   0 puyuan     (501) 453037844     4598 2023-05-24 10:01:45.000000 LightZero-0.0.2/lzero/envs/tests/test_lightzero_env_wrapper.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.322700 LightZero-0.0.2/lzero/envs/wrappers/
--rw-r--r--   0 puyuan     (501) 453037844       86 2023-05-24 10:01:45.000000 LightZero-0.0.2/lzero/envs/wrappers/__init__.py
--rw-r--r--   0 puyuan     (501) 453037844     3675 2023-05-24 10:01:45.000000 LightZero-0.0.2/lzero/envs/wrappers/action_discretization_env_wrapper.py
--rw-r--r--   0 puyuan     (501) 453037844     4527 2023-10-10 08:13:33.000000 LightZero-0.0.2/lzero/envs/wrappers/lightzero_env_wrapper.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.322970 LightZero-0.0.2/lzero/mcts/
--rw-r--r--   0 puyuan     (501) 453037844       91 2023-05-24 10:01:45.000000 LightZero-0.0.2/lzero/mcts/__init__.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.324069 LightZero-0.0.2/lzero/mcts/buffer/
--rw-r--r--   0 puyuan     (501) 453037844      322 2023-10-10 08:13:33.000000 LightZero-0.0.2/lzero/mcts/buffer/__init__.py
--rw-r--r--   0 puyuan     (501) 453037844    18046 2023-11-13 12:09:06.000000 LightZero-0.0.2/lzero/mcts/buffer/game_buffer.py
--rw-r--r--   0 puyuan     (501) 453037844    24104 2023-09-03 11:51:06.000000 LightZero-0.0.2/lzero/mcts/buffer/game_buffer_efficientzero.py
--rw-r--r--   0 puyuan     (501) 453037844     5783 2023-08-02 09:19:21.000000 LightZero-0.0.2/lzero/mcts/buffer/game_buffer_gumbel_muzero.py
--rw-r--r--   0 puyuan     (501) 453037844    36096 2023-10-13 09:55:49.000000 LightZero-0.0.2/lzero/mcts/buffer/game_buffer_muzero.py
--rw-r--r--   0 puyuan     (501) 453037844    30989 2023-10-18 03:06:33.000000 LightZero-0.0.2/lzero/mcts/buffer/game_buffer_sampled_efficientzero.py
--rw-r--r--   0 puyuan     (501) 453037844     8096 2023-10-10 08:13:33.000000 LightZero-0.0.2/lzero/mcts/buffer/game_buffer_stochastic_muzero.py
--rw-r--r--   0 puyuan     (501) 453037844    15509 2023-11-13 12:09:06.000000 LightZero-0.0.2/lzero/mcts/buffer/game_segment.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.324193 LightZero-0.0.2/lzero/mcts/ctree/
--rw-r--r--   0 puyuan     (501) 453037844        0 2023-04-14 09:11:22.000000 LightZero-0.0.2/lzero/mcts/ctree/__init__.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.324404 LightZero-0.0.2/lzero/mcts/ctree/common_lib/
--rw-r--r--   0 puyuan     (501) 453037844     1661 2023-05-24 10:01:45.000000 LightZero-0.0.2/lzero/mcts/ctree/common_lib/cminimax.cpp
--rw-r--r--   0 puyuan     (501) 453037844      785 2023-05-24 10:01:45.000000 LightZero-0.0.2/lzero/mcts/ctree/common_lib/cminimax.h
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.324530 LightZero-0.0.2/lzero/mcts/ctree/ctree_efficientzero/
--rw-r--r--   0 puyuan     (501) 453037844        0 2023-04-14 09:11:22.000000 LightZero-0.0.2/lzero/mcts/ctree/ctree_efficientzero/__init__.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.324758 LightZero-0.0.2/lzero/mcts/ctree/ctree_efficientzero/lib/
--rw-r--r--   0 puyuan     (501) 453037844    26811 2023-08-02 09:19:21.000000 LightZero-0.0.2/lzero/mcts/ctree/ctree_efficientzero/lib/cnode.cpp
--rw-r--r--   0 puyuan     (501) 453037844     3973 2023-08-02 09:19:21.000000 LightZero-0.0.2/lzero/mcts/ctree/ctree_efficientzero/lib/cnode.h
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.324878 LightZero-0.0.2/lzero/mcts/ctree/ctree_gumbel_muzero/
--rw-r--r--   0 puyuan     (501) 453037844        0 2023-08-02 09:19:21.000000 LightZero-0.0.2/lzero/mcts/ctree/ctree_gumbel_muzero/__init__.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.325090 LightZero-0.0.2/lzero/mcts/ctree/ctree_gumbel_muzero/lib/
--rw-r--r--   0 puyuan     (501) 453037844    41503 2023-08-02 09:19:21.000000 LightZero-0.0.2/lzero/mcts/ctree/ctree_gumbel_muzero/lib/cnode.cpp
--rw-r--r--   0 puyuan     (501) 453037844     5537 2023-08-02 09:19:21.000000 LightZero-0.0.2/lzero/mcts/ctree/ctree_gumbel_muzero/lib/cnode.h
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.325190 LightZero-0.0.2/lzero/mcts/ctree/ctree_muzero/
--rw-r--r--   0 puyuan     (501) 453037844        0 2023-04-14 09:11:22.000000 LightZero-0.0.2/lzero/mcts/ctree/ctree_muzero/__init__.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.325386 LightZero-0.0.2/lzero/mcts/ctree/ctree_muzero/lib/
--rw-r--r--   0 puyuan     (501) 453037844    24132 2023-08-02 09:19:21.000000 LightZero-0.0.2/lzero/mcts/ctree/ctree_muzero/lib/cnode.cpp
--rw-r--r--   0 puyuan     (501) 453037844     3782 2023-08-02 09:19:21.000000 LightZero-0.0.2/lzero/mcts/ctree/ctree_muzero/lib/cnode.h
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.325478 LightZero-0.0.2/lzero/mcts/ctree/ctree_sampled_efficientzero/
--rw-r--r--   0 puyuan     (501) 453037844        0 2023-04-14 09:11:22.000000 LightZero-0.0.2/lzero/mcts/ctree/ctree_sampled_efficientzero/__init__.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.325682 LightZero-0.0.2/lzero/mcts/ctree/ctree_sampled_efficientzero/lib/
--rw-r--r--   0 puyuan     (501) 453037844    46245 2023-11-19 12:18:03.000000 LightZero-0.0.2/lzero/mcts/ctree/ctree_sampled_efficientzero/lib/cnode.cpp
--rw-r--r--   0 puyuan     (501) 453037844     4955 2023-10-13 09:55:49.000000 LightZero-0.0.2/lzero/mcts/ctree/ctree_sampled_efficientzero/lib/cnode.h
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.325784 LightZero-0.0.2/lzero/mcts/ctree/ctree_stochastic_muzero/
--rw-r--r--   0 puyuan     (501) 453037844        0 2023-10-10 08:13:33.000000 LightZero-0.0.2/lzero/mcts/ctree/ctree_stochastic_muzero/__init__.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.326000 LightZero-0.0.2/lzero/mcts/ctree/ctree_stochastic_muzero/lib/
--rw-r--r--   0 puyuan     (501) 453037844    26898 2023-10-10 08:13:33.000000 LightZero-0.0.2/lzero/mcts/ctree/ctree_stochastic_muzero/lib/cnode.cpp
--rw-r--r--   0 puyuan     (501) 453037844     4089 2023-10-10 08:13:33.000000 LightZero-0.0.2/lzero/mcts/ctree/ctree_stochastic_muzero/lib/cnode.h
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.326991 LightZero-0.0.2/lzero/mcts/ptree/
--rw-r--r--   0 puyuan     (501) 453037844       23 2023-05-24 10:01:45.000000 LightZero-0.0.2/lzero/mcts/ptree/__init__.py
--rw-r--r--   0 puyuan     (501) 453037844     1216 2023-05-24 10:01:45.000000 LightZero-0.0.2/lzero/mcts/ptree/minimax.py
--rw-r--r--   0 puyuan     (501) 453037844    22124 2023-10-30 04:54:58.000000 LightZero-0.0.2/lzero/mcts/ptree/ptree_az.py
--rw-r--r--   0 puyuan     (501) 453037844    24634 2023-11-15 04:39:38.000000 LightZero-0.0.2/lzero/mcts/ptree/ptree_az_sampled.py
--rw-r--r--   0 puyuan     (501) 453037844    23610 2023-08-02 09:19:21.000000 LightZero-0.0.2/lzero/mcts/ptree/ptree_ez.py
--rw-r--r--   0 puyuan     (501) 453037844    22992 2023-10-26 17:49:52.000000 LightZero-0.0.2/lzero/mcts/ptree/ptree_mz.py
--rw-r--r--   0 puyuan     (501) 453037844    34700 2023-11-15 04:39:38.000000 LightZero-0.0.2/lzero/mcts/ptree/ptree_sez.py
--rw-r--r--   0 puyuan     (501) 453037844    25032 2023-10-10 08:13:33.000000 LightZero-0.0.2/lzero/mcts/ptree/ptree_stochastic_mz.py
--rw-r--r--   0 puyuan     (501) 453037844      599 2023-04-14 09:11:22.000000 LightZero-0.0.2/lzero/mcts/ptree/test_sez_sample.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.328125 LightZero-0.0.2/lzero/mcts/tests/
--rw-r--r--   0 puyuan     (501) 453037844        0 2023-10-10 08:13:33.000000 LightZero-0.0.2/lzero/mcts/tests/__init__.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.328405 LightZero-0.0.2/lzero/mcts/tests/config/
--rw-r--r--   0 puyuan     (501) 453037844        0 2023-10-10 08:13:33.000000 LightZero-0.0.2/lzero/mcts/tests/config/__init__.py
--rw-r--r--   0 puyuan     (501) 453037844     3569 2023-10-10 08:13:33.000000 LightZero-0.0.2/lzero/mcts/tests/config/atari_efficientzero_config_for_test.py
--rw-r--r--   0 puyuan     (501) 453037844     3228 2023-10-10 08:13:33.000000 LightZero-0.0.2/lzero/mcts/tests/config/tictactoe_muzero_bot_mode_config_for_test.py
--rw-r--r--   0 puyuan     (501) 453037844     4804 2023-10-31 13:06:51.000000 LightZero-0.0.2/lzero/mcts/tests/cprofile_mcts_ptree.py
--rw-r--r--   0 puyuan     (501) 453037844    14991 2023-10-31 13:06:51.000000 LightZero-0.0.2/lzero/mcts/tests/eval_tree_speed.py
--rw-r--r--   0 puyuan     (501) 453037844     2767 2023-05-24 10:01:45.000000 LightZero-0.0.2/lzero/mcts/tests/test_game_buffer.py
--rw-r--r--   0 puyuan     (501) 453037844     6008 2023-10-10 08:13:33.000000 LightZero-0.0.2/lzero/mcts/tests/test_game_segment.py
--rw-r--r--   0 puyuan     (501) 453037844      340 2023-05-24 10:01:45.000000 LightZero-0.0.2/lzero/mcts/tests/test_image_transform.py
--rw-r--r--   0 puyuan     (501) 453037844    14808 2023-10-31 13:06:51.000000 LightZero-0.0.2/lzero/mcts/tests/test_mcts_ctree.py
--rw-r--r--   0 puyuan     (501) 453037844    11715 2023-10-30 07:53:41.000000 LightZero-0.0.2/lzero/mcts/tests/test_mcts_ptree.py
--rw-r--r--   0 puyuan     (501) 453037844     5048 2023-10-30 08:11:12.000000 LightZero-0.0.2/lzero/mcts/tests/test_mcts_sampled_ctree.py
--rw-r--r--   0 puyuan     (501) 453037844     1016 2023-05-24 10:01:45.000000 LightZero-0.0.2/lzero/mcts/tests/test_utils.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.329152 LightZero-0.0.2/lzero/mcts/tree_search/
--rw-r--r--   0 puyuan     (501) 453037844      397 2023-10-13 09:55:49.000000 LightZero-0.0.2/lzero/mcts/tree_search/__init__.py
--rw-r--r--   0 puyuan     (501) 453037844    26627 2023-11-09 09:09:19.000000 LightZero-0.0.2/lzero/mcts/tree_search/mcts_ctree.py
--rw-r--r--   0 puyuan     (501) 453037844    11601 2023-10-13 09:55:49.000000 LightZero-0.0.2/lzero/mcts/tree_search/mcts_ctree_sampled.py
--rw-r--r--   0 puyuan     (501) 453037844    12786 2023-10-10 08:13:33.000000 LightZero-0.0.2/lzero/mcts/tree_search/mcts_ctree_stochastic.py
--rw-r--r--   0 puyuan     (501) 453037844    18633 2023-08-02 09:19:21.000000 LightZero-0.0.2/lzero/mcts/tree_search/mcts_ptree.py
--rw-r--r--   0 puyuan     (501) 453037844    11526 2023-10-13 09:55:49.000000 LightZero-0.0.2/lzero/mcts/tree_search/mcts_ptree_sampled.py
--rw-r--r--   0 puyuan     (501) 453037844    12633 2023-10-10 08:13:33.000000 LightZero-0.0.2/lzero/mcts/tree_search/mcts_ptree_stochastic.py
--rw-r--r--   0 puyuan     (501) 453037844     6877 2023-10-18 03:06:33.000000 LightZero-0.0.2/lzero/mcts/utils.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.330650 LightZero-0.0.2/lzero/model/
--rw-r--r--   0 puyuan     (501) 453037844       68 2023-05-24 10:01:45.000000 LightZero-0.0.2/lzero/model/__init__.py
--rw-r--r--   0 puyuan     (501) 453037844    17173 2023-11-15 04:39:38.000000 LightZero-0.0.2/lzero/model/alphazero_model.py
--rw-r--r--   0 puyuan     (501) 453037844    22145 2023-10-13 09:55:49.000000 LightZero-0.0.2/lzero/model/common.py
--rw-r--r--   0 puyuan     (501) 453037844    32400 2023-08-02 09:19:21.000000 LightZero-0.0.2/lzero/model/efficientzero_model.py
--rw-r--r--   0 puyuan     (501) 453037844    26915 2023-09-03 11:51:06.000000 LightZero-0.0.2/lzero/model/efficientzero_model_mlp.py
--rw-r--r--   0 puyuan     (501) 453037844     4173 2023-05-24 10:01:46.000000 LightZero-0.0.2/lzero/model/image_transform.py
--rw-r--r--   0 puyuan     (501) 453037844    28672 2023-10-13 09:55:49.000000 LightZero-0.0.2/lzero/model/muzero_model.py
--rw-r--r--   0 puyuan     (501) 453037844    24178 2023-10-13 09:55:49.000000 LightZero-0.0.2/lzero/model/muzero_model_mlp.py
--rw-r--r--   0 puyuan     (501) 453037844    36681 2023-10-13 09:55:49.000000 LightZero-0.0.2/lzero/model/sampled_efficientzero_model.py
--rw-r--r--   0 puyuan     (501) 453037844    29432 2023-08-02 09:19:21.000000 LightZero-0.0.2/lzero/model/sampled_efficientzero_model_mlp.py
--rw-r--r--   0 puyuan     (501) 453037844    41962 2023-10-10 08:13:34.000000 LightZero-0.0.2/lzero/model/stochastic_muzero_model.py
--rw-r--r--   0 puyuan     (501) 453037844    19412 2023-10-10 08:13:34.000000 LightZero-0.0.2/lzero/model/stochastic_muzero_model_mlp.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.331430 LightZero-0.0.2/lzero/model/tests/
--rw-r--r--   0 puyuan     (501) 453037844        0 2023-04-14 09:11:22.000000 LightZero-0.0.2/lzero/model/tests/__init__.py
--rw-r--r--   0 puyuan     (501) 453037844     4554 2023-11-15 04:39:38.000000 LightZero-0.0.2/lzero/model/tests/test_alphazero_model.py
--rw-r--r--   0 puyuan     (501) 453037844      957 2023-04-14 09:11:22.000000 LightZero-0.0.2/lzero/model/tests/test_common.py
--rw-r--r--   0 puyuan     (501) 453037844     6687 2023-08-02 09:19:21.000000 LightZero-0.0.2/lzero/model/tests/test_efficientzero_model.py
--rw-r--r--   0 puyuan     (501) 453037844     5754 2023-08-02 09:19:21.000000 LightZero-0.0.2/lzero/model/tests/test_muzero_model.py
--rw-r--r--   0 puyuan     (501) 453037844     6897 2023-08-02 09:19:21.000000 LightZero-0.0.2/lzero/model/tests/test_sampled_efficientzero_model.py
--rw-r--r--   0 puyuan     (501) 453037844     2241 2023-10-10 08:13:34.000000 LightZero-0.0.2/lzero/model/tests/test_stochastic_muzero_model.py
--rw-r--r--   0 puyuan     (501) 453037844     2775 2023-08-22 03:29:23.000000 LightZero-0.0.2/lzero/model/utils.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.332736 LightZero-0.0.2/lzero/policy/
--rw-r--r--   0 puyuan     (501) 453037844       54 2023-05-21 12:25:43.000000 LightZero-0.0.2/lzero/policy/__init__.py
--rw-r--r--   0 puyuan     (501) 453037844    18301 2023-11-15 04:39:38.000000 LightZero-0.0.2/lzero/policy/alphazero.py
--rw-r--r--   0 puyuan     (501) 453037844    41639 2023-10-31 13:06:51.000000 LightZero-0.0.2/lzero/policy/efficientzero.py
--rw-r--r--   0 puyuan     (501) 453037844    40343 2023-11-13 12:09:06.000000 LightZero-0.0.2/lzero/policy/gumbel_muzero.py
--rw-r--r--   0 puyuan     (501) 453037844    40977 2023-11-13 12:09:06.000000 LightZero-0.0.2/lzero/policy/muzero.py
--rw-r--r--   0 puyuan     (501) 453037844    14651 2023-10-31 13:06:51.000000 LightZero-0.0.2/lzero/policy/random_policy.py
--rw-r--r--   0 puyuan     (501) 453037844    28564 2023-11-15 04:39:38.000000 LightZero-0.0.2/lzero/policy/sampled_alphazero.py
--rw-r--r--   0 puyuan     (501) 453037844    62265 2023-10-31 13:06:51.000000 LightZero-0.0.2/lzero/policy/sampled_efficientzero.py
--rw-r--r--   0 puyuan     (501) 453037844     5375 2023-10-10 08:30:27.000000 LightZero-0.0.2/lzero/policy/scaling_transform.py
--rw-r--r--   0 puyuan     (501) 453037844    43299 2023-10-31 13:06:51.000000 LightZero-0.0.2/lzero/policy/stochastic_muzero.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.333140 LightZero-0.0.2/lzero/policy/tests/
--rw-r--r--   0 puyuan     (501) 453037844        0 2023-04-14 09:11:22.000000 LightZero-0.0.2/lzero/policy/tests/__init__.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.333411 LightZero-0.0.2/lzero/policy/tests/config/
--rw-r--r--   0 puyuan     (501) 453037844        0 2023-10-10 08:13:34.000000 LightZero-0.0.2/lzero/policy/tests/config/__init__.py
--rw-r--r--   0 puyuan     (501) 453037844     3364 2023-10-10 08:13:34.000000 LightZero-0.0.2/lzero/policy/tests/config/atari_muzero_config_for_test.py
--rw-r--r--   0 puyuan     (501) 453037844     2593 2023-10-10 08:13:34.000000 LightZero-0.0.2/lzero/policy/tests/config/cartpole_muzero_config_for_test.py
--rw-r--r--   0 puyuan     (501) 453037844     3057 2023-10-10 08:13:34.000000 LightZero-0.0.2/lzero/policy/tests/test_get_target_obs_index_in_step_k.py
--rw-r--r--   0 puyuan     (501) 453037844      561 2023-05-24 10:01:46.000000 LightZero-0.0.2/lzero/policy/tests/test_scaling_transform.py
--rw-r--r--   0 puyuan     (501) 453037844     7116 2023-10-18 03:06:33.000000 LightZero-0.0.2/lzero/policy/tests/test_utils.py
--rw-r--r--   0 puyuan     (501) 453037844    24390 2023-11-15 04:39:38.000000 LightZero-0.0.2/lzero/policy/utils.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.334010 LightZero-0.0.2/lzero/worker/
--rw-r--r--   0 puyuan     (501) 453037844      195 2023-10-13 09:55:49.000000 LightZero-0.0.2/lzero/worker/__init__.py
--rw-r--r--   0 puyuan     (501) 453037844    17052 2023-10-30 04:54:58.000000 LightZero-0.0.2/lzero/worker/alphazero_collector.py
--rw-r--r--   0 puyuan     (501) 453037844    13252 2023-10-30 04:54:58.000000 LightZero-0.0.2/lzero/worker/alphazero_evaluator.py
--rw-r--r--   0 puyuan     (501) 453037844    37480 2023-10-31 13:06:51.000000 LightZero-0.0.2/lzero/worker/muzero_collector.py
--rw-r--r--   0 puyuan     (501) 453037844    22758 2023-11-02 15:34:40.000000 LightZero-0.0.2/lzero/worker/muzero_evaluator.py
--rw-r--r--   0 puyuan     (501) 453037844     1329 2023-08-22 03:29:23.000000 LightZero-0.0.2/pyproject.toml
--rw-r--r--   0 puyuan     (501) 453037844       38 2023-11-19 12:18:05.350689 LightZero-0.0.2/setup.cfg
--rw-r--r--   0 puyuan     (501) 453037844     4676 2023-10-10 08:13:34.000000 LightZero-0.0.2/setup.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.334122 LightZero-0.0.2/zoo/
--rw-r--r--   0 puyuan     (501) 453037844        0 2023-04-14 09:11:22.000000 LightZero-0.0.2/zoo/__init__.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.334202 LightZero-0.0.2/zoo/atari/
--rw-r--r--   0 puyuan     (501) 453037844        0 2023-04-14 09:11:22.000000 LightZero-0.0.2/zoo/atari/__init__.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.335036 LightZero-0.0.2/zoo/atari/config/
--rw-r--r--   0 puyuan     (501) 453037844        0 2023-04-14 09:11:22.000000 LightZero-0.0.2/zoo/atari/config/__init__.py
--rw-r--r--   0 puyuan     (501) 453037844     3583 2023-10-22 10:11:59.000000 LightZero-0.0.2/zoo/atari/config/atari_efficientzero_config.py
--rw-r--r--   0 puyuan     (501) 453037844     4820 2023-10-10 08:13:34.000000 LightZero-0.0.2/zoo/atari/config/atari_efficientzero_multigpu_ddp_config.py
--rw-r--r--   0 puyuan     (501) 453037844     3351 2023-10-10 08:13:34.000000 LightZero-0.0.2/zoo/atari/config/atari_gumbel_muzero_config.py
--rw-r--r--   0 puyuan     (501) 453037844     3659 2023-11-06 10:43:13.000000 LightZero-0.0.2/zoo/atari/config/atari_muzero_config.py
--rw-r--r--   0 puyuan     (501) 453037844     4288 2023-10-10 08:13:34.000000 LightZero-0.0.2/zoo/atari/config/atari_muzero_multigpu_ddp_config.py
--rw-r--r--   0 puyuan     (501) 453037844     3456 2023-10-17 09:17:07.000000 LightZero-0.0.2/zoo/atari/config/atari_sampled_efficientzero_config.py
--rw-r--r--   0 puyuan     (501) 453037844     3722 2023-10-10 08:13:34.000000 LightZero-0.0.2/zoo/atari/config/atari_stochastic_muzero_config.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.335236 LightZero-0.0.2/zoo/atari/entry/
--rw-r--r--   0 puyuan     (501) 453037844        0 2023-10-10 08:13:34.000000 LightZero-0.0.2/zoo/atari/entry/__init__.py
--rw-r--r--   0 puyuan     (501) 453037844     2226 2023-10-10 08:13:34.000000 LightZero-0.0.2/zoo/atari/entry/atari_eval.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.335569 LightZero-0.0.2/zoo/atari/envs/
--rw-r--r--   0 puyuan     (501) 453037844       46 2023-04-14 09:11:22.000000 LightZero-0.0.2/zoo/atari/envs/__init__.py
--rw-r--r--   0 puyuan     (501) 453037844     5926 2023-05-24 10:01:46.000000 LightZero-0.0.2/zoo/atari/envs/atari_lightzero_env.py
--rw-r--r--   0 puyuan     (501) 453037844     7836 2023-10-10 08:02:56.000000 LightZero-0.0.2/zoo/atari/envs/atari_wrappers.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.336038 LightZero-0.0.2/zoo/board_games/
--rw-r--r--   0 puyuan     (501) 453037844        0 2023-04-14 09:11:22.000000 LightZero-0.0.2/zoo/board_games/__init__.py
--rw-r--r--   0 puyuan     (501) 453037844     9171 2023-10-30 04:54:58.000000 LightZero-0.0.2/zoo/board_games/alphabeta_pruning_bot.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.336595 LightZero-0.0.2/zoo/board_games/classic_search_algorithm/
--rw-r--r--   0 puyuan     (501) 453037844        0 2023-04-14 09:11:22.000000 LightZero-0.0.2/zoo/board_games/classic_search_algorithm/__init__.py
--rw-r--r--   0 puyuan     (501) 453037844     1839 2023-04-14 09:11:22.000000 LightZero-0.0.2/zoo/board_games/classic_search_algorithm/alphabeta_pruning.py
--rw-r--r--   0 puyuan     (501) 453037844     2304 2023-04-14 09:11:22.000000 LightZero-0.0.2/zoo/board_games/classic_search_algorithm/alphabeta_pruning_return_best_subtree.py
--rw-r--r--   0 puyuan     (501) 453037844      759 2023-04-14 09:11:22.000000 LightZero-0.0.2/zoo/board_games/classic_search_algorithm/minimax_v0.py
--rw-r--r--   0 puyuan     (501) 453037844     1426 2023-04-14 09:11:22.000000 LightZero-0.0.2/zoo/board_games/classic_search_algorithm/minimax_v1.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.336733 LightZero-0.0.2/zoo/board_games/go/
--rw-r--r--   0 puyuan     (501) 453037844        0 2023-04-14 09:11:22.000000 LightZero-0.0.2/zoo/board_games/go/__init__.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.336962 LightZero-0.0.2/zoo/board_games/go/config/
--rw-r--r--   0 puyuan     (501) 453037844        0 2023-05-24 10:01:46.000000 LightZero-0.0.2/zoo/board_games/go/config/__init__.py
--rw-r--r--   0 puyuan     (501) 453037844        8 2023-08-22 03:29:23.000000 LightZero-0.0.2/zoo/board_games/go/config/go_alphazero_sp-mode_config.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.337320 LightZero-0.0.2/zoo/board_games/go/envs/
--rw-r--r--   0 puyuan     (501) 453037844        0 2023-08-22 03:29:23.000000 LightZero-0.0.2/zoo/board_games/go/envs/__init__.py
--rw-r--r--   0 puyuan     (501) 453037844    12612 2023-08-22 03:29:23.000000 LightZero-0.0.2/zoo/board_games/go/envs/go_env.py
--rw-r--r--   0 puyuan     (501) 453037844     1302 2023-08-22 03:29:23.000000 LightZero-0.0.2/zoo/board_games/go/envs/test_go_env.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.337455 LightZero-0.0.2/zoo/board_games/gomoku/
--rw-r--r--   0 puyuan     (501) 453037844        0 2023-04-14 09:11:22.000000 LightZero-0.0.2/zoo/board_games/gomoku/__init__.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.338466 LightZero-0.0.2/zoo/board_games/gomoku/config/
--rw-r--r--   0 puyuan     (501) 453037844        0 2023-05-24 10:01:46.000000 LightZero-0.0.2/zoo/board_games/gomoku/config/__init__.py
--rw-r--r--   0 puyuan     (501) 453037844     4070 2023-11-15 04:40:19.000000 LightZero-0.0.2/zoo/board_games/gomoku/config/gomoku_alphazero_bot_mode_config.py
--rw-r--r--   0 puyuan     (501) 453037844     3978 2023-10-30 04:54:58.000000 LightZero-0.0.2/zoo/board_games/gomoku/config/gomoku_alphazero_sp_mode_config.py
--rw-r--r--   0 puyuan     (501) 453037844     3366 2023-11-13 12:09:06.000000 LightZero-0.0.2/zoo/board_games/gomoku/config/gomoku_gumbel_muzero_bot_mode_config.py
--rw-r--r--   0 puyuan     (501) 453037844     3251 2023-10-10 08:13:34.000000 LightZero-0.0.2/zoo/board_games/gomoku/config/gomoku_muzero_bot_mode_config.py
--rw-r--r--   0 puyuan     (501) 453037844     3305 2023-08-22 03:29:23.000000 LightZero-0.0.2/zoo/board_games/gomoku/config/gomoku_muzero_sp_mode_config.py
--rw-r--r--   0 puyuan     (501) 453037844     4483 2023-11-15 04:39:38.000000 LightZero-0.0.2/zoo/board_games/gomoku/config/gomoku_sampled_alphazero_bot_mode_config.py
--rw-r--r--   0 puyuan     (501) 453037844     4471 2023-11-15 04:39:38.000000 LightZero-0.0.2/zoo/board_games/gomoku/config/gomoku_sampled_alphazero_sp_mode_config.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.339068 LightZero-0.0.2/zoo/board_games/gomoku/entry/
--rw-r--r--   0 puyuan     (501) 453037844        0 2023-10-10 08:13:34.000000 LightZero-0.0.2/zoo/board_games/gomoku/entry/__init__.py
--rw-r--r--   0 puyuan     (501) 453037844     1975 2023-11-15 04:39:38.000000 LightZero-0.0.2/zoo/board_games/gomoku/entry/gomoku_alphazero_eval.py
--rw-r--r--   0 puyuan     (501) 453037844     2047 2023-10-10 08:13:34.000000 LightZero-0.0.2/zoo/board_games/gomoku/entry/gomoku_gumbel_muzero_eval.py
--rw-r--r--   0 puyuan     (501) 453037844     1911 2023-10-10 08:13:34.000000 LightZero-0.0.2/zoo/board_games/gomoku/entry/gomoku_muzero_eval.py
--rw-r--r--   0 puyuan     (501) 453037844     2095 2023-11-15 04:39:38.000000 LightZero-0.0.2/zoo/board_games/gomoku/entry/gomoku_sampled_alphazero_eval.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.340537 LightZero-0.0.2/zoo/board_games/gomoku/envs/
--rw-r--r--   0 puyuan     (501) 453037844        0 2023-08-22 03:29:23.000000 LightZero-0.0.2/zoo/board_games/gomoku/envs/__init__.py
--rw-r--r--   0 puyuan     (501) 453037844    32723 2023-11-15 04:39:38.000000 LightZero-0.0.2/zoo/board_games/gomoku/envs/gomoku_env.py
--rw-r--r--   0 puyuan     (501) 453037844     8458 2023-11-15 04:39:38.000000 LightZero-0.0.2/zoo/board_games/gomoku/envs/gomoku_human_vs_bot_UI.py
--rw-r--r--   0 puyuan     (501) 453037844    16828 2023-11-15 04:39:38.000000 LightZero-0.0.2/zoo/board_games/gomoku/envs/gomoku_rule_bot_v0.py
--rw-r--r--   0 puyuan     (501) 453037844    15588 2023-11-15 04:39:38.000000 LightZero-0.0.2/zoo/board_games/gomoku/envs/gomoku_rule_bot_v1.py
--rw-r--r--   0 puyuan     (501) 453037844     4747 2023-11-13 12:15:56.000000 LightZero-0.0.2/zoo/board_games/gomoku/envs/test_gomoku_alphabeta_pruning_bot.py
--rw-r--r--   0 puyuan     (501) 453037844     3440 2023-11-15 04:39:38.000000 LightZero-0.0.2/zoo/board_games/gomoku/envs/test_gomoku_env.py
--rw-r--r--   0 puyuan     (501) 453037844     6487 2023-11-13 12:15:56.000000 LightZero-0.0.2/zoo/board_games/gomoku/envs/test_gomoku_mcts_bot.py
--rw-r--r--   0 puyuan     (501) 453037844     4725 2023-11-15 04:39:38.000000 LightZero-0.0.2/zoo/board_games/gomoku/envs/test_gomoku_rule_bot_v0.py
--rw-r--r--   0 puyuan     (501) 453037844     1898 2023-11-13 12:15:56.000000 LightZero-0.0.2/zoo/board_games/gomoku/envs/test_gomoku_rule_bot_v1.py
--rw-r--r--   0 puyuan     (501) 453037844     1260 2023-08-22 03:29:23.000000 LightZero-0.0.2/zoo/board_games/gomoku/envs/utils.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.341291 LightZero-0.0.2/zoo/board_games/gomoku/test/
--rw-r--r--   0 puyuan     (501) 453037844        0 2023-08-02 09:19:22.000000 LightZero-0.0.2/zoo/board_games/gomoku/test/__init__.py
--rw-r--r--   0 puyuan     (501) 453037844     4968 2023-08-02 09:19:22.000000 LightZero-0.0.2/zoo/board_games/gomoku/test/eval_get_done_winner.py
--rw-r--r--   0 puyuan     (501) 453037844     5110 2023-08-02 09:19:22.000000 LightZero-0.0.2/zoo/board_games/gomoku/test/eval_legal_actions.py
--rw-r--r--   0 puyuan     (501) 453037844     2663 2023-08-02 09:19:22.000000 LightZero-0.0.2/zoo/board_games/gomoku/test/test_get_done_winner_cython.py
--rw-r--r--   0 puyuan     (501) 453037844     2552 2023-11-13 12:15:56.000000 LightZero-0.0.2/zoo/board_games/gomoku/test/test_gomoku_env_legal_actions.py
--rw-r--r--   0 puyuan     (501) 453037844     1797 2023-08-02 09:19:22.000000 LightZero-0.0.2/zoo/board_games/gomoku/test/test_legal_actions_cython.py
--rw-r--r--   0 puyuan     (501) 453037844    18368 2023-10-30 04:54:58.000000 LightZero-0.0.2/zoo/board_games/mcts_bot.py
--rw-r--r--   0 puyuan     (501) 453037844    21648 2023-11-13 12:15:56.000000 LightZero-0.0.2/zoo/board_games/test_speed_win-rate_between_bots.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.341414 LightZero-0.0.2/zoo/board_games/tictactoe/
--rw-r--r--   0 puyuan     (501) 453037844        0 2023-04-14 09:11:22.000000 LightZero-0.0.2/zoo/board_games/tictactoe/__init__.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.342346 LightZero-0.0.2/zoo/board_games/tictactoe/config/
--rw-r--r--   0 puyuan     (501) 453037844        0 2023-08-22 03:29:23.000000 LightZero-0.0.2/zoo/board_games/tictactoe/config/__init__.py
--rw-r--r--   0 puyuan     (501) 453037844     3499 2023-11-15 04:39:38.000000 LightZero-0.0.2/zoo/board_games/tictactoe/config/tictactoe_alphazero_bot_mode_config.py
--rw-r--r--   0 puyuan     (501) 453037844     3966 2023-10-30 04:54:58.000000 LightZero-0.0.2/zoo/board_games/tictactoe/config/tictactoe_alphazero_bot_mode_multigpu_ddp_config.py
--rw-r--r--   0 puyuan     (501) 453037844     3364 2023-10-30 04:54:58.000000 LightZero-0.0.2/zoo/board_games/tictactoe/config/tictactoe_alphazero_sp_mode_config.py
--rw-r--r--   0 puyuan     (501) 453037844     3947 2023-10-30 04:54:58.000000 LightZero-0.0.2/zoo/board_games/tictactoe/config/tictactoe_alphazero_sp_mode_multigpu_ddp_config.py
--rw-r--r--   0 puyuan     (501) 453037844     3052 2023-11-13 12:09:06.000000 LightZero-0.0.2/zoo/board_games/tictactoe/config/tictactoe_gumbel_muzero_bot_mode_config.py
--rw-r--r--   0 puyuan     (501) 453037844     2965 2023-10-13 09:55:49.000000 LightZero-0.0.2/zoo/board_games/tictactoe/config/tictactoe_muzero_bot_mode_config.py
--rw-r--r--   0 puyuan     (501) 453037844     2932 2023-10-10 08:13:34.000000 LightZero-0.0.2/zoo/board_games/tictactoe/config/tictactoe_muzero_sp_mode_config.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.342646 LightZero-0.0.2/zoo/board_games/tictactoe/entry/
--rw-r--r--   0 puyuan     (501) 453037844        0 2023-10-10 08:13:34.000000 LightZero-0.0.2/zoo/board_games/tictactoe/entry/__init__.py
--rw-r--r--   0 puyuan     (501) 453037844     1926 2023-10-10 08:13:34.000000 LightZero-0.0.2/zoo/board_games/tictactoe/entry/tictactoe_alphazero_eval.py
--rw-r--r--   0 puyuan     (501) 453037844     1918 2023-10-10 08:13:34.000000 LightZero-0.0.2/zoo/board_games/tictactoe/entry/tictactoe_muzero_eval.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.343268 LightZero-0.0.2/zoo/board_games/tictactoe/envs/
--rw-r--r--   0 puyuan     (501) 453037844        0 2023-04-14 09:11:22.000000 LightZero-0.0.2/zoo/board_games/tictactoe/envs/__init__.py
--rw-r--r--   0 puyuan     (501) 453037844     4105 2023-05-24 10:01:46.000000 LightZero-0.0.2/zoo/board_games/tictactoe/envs/test_tictactoe_alphabeta_prunning_bot.py
--rw-r--r--   0 puyuan     (501) 453037844     3096 2023-08-02 09:19:22.000000 LightZero-0.0.2/zoo/board_games/tictactoe/envs/test_tictactoe_env.py
--rw-r--r--   0 puyuan     (501) 453037844     6229 2023-04-14 09:11:22.000000 LightZero-0.0.2/zoo/board_games/tictactoe/envs/test_tictactoe_mcts_bot.py
--rw-r--r--   0 puyuan     (501) 453037844     1203 2023-05-24 10:01:46.000000 LightZero-0.0.2/zoo/board_games/tictactoe/envs/test_tictactoe_rule_bot_v0.py
--rw-r--r--   0 puyuan     (501) 453037844    24101 2023-10-30 04:54:58.000000 LightZero-0.0.2/zoo/board_games/tictactoe/envs/tictactoe_env.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.343414 LightZero-0.0.2/zoo/box2d/
--rw-r--r--   0 puyuan     (501) 453037844        0 2023-04-14 09:11:22.000000 LightZero-0.0.2/zoo/box2d/__init__.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.343511 LightZero-0.0.2/zoo/box2d/bipedalwalker/
--rw-r--r--   0 puyuan     (501) 453037844        0 2023-05-24 10:01:46.000000 LightZero-0.0.2/zoo/box2d/bipedalwalker/__init__.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.344047 LightZero-0.0.2/zoo/box2d/bipedalwalker/config/
--rw-r--r--   0 puyuan     (501) 453037844        0 2023-05-24 10:01:46.000000 LightZero-0.0.2/zoo/box2d/bipedalwalker/config/__init__.py
--rw-r--r--   0 puyuan     (501) 453037844     4203 2023-10-10 08:32:30.000000 LightZero-0.0.2/zoo/box2d/bipedalwalker/config/bipedalwalker_cont_disc_efficientzero_config.py
--rw-r--r--   0 puyuan     (501) 453037844     4313 2023-10-10 08:32:30.000000 LightZero-0.0.2/zoo/box2d/bipedalwalker/config/bipedalwalker_cont_disc_sampled_efficientzero_config.py
--rw-r--r--   0 puyuan     (501) 453037844     4262 2023-10-13 09:55:49.000000 LightZero-0.0.2/zoo/box2d/bipedalwalker/config/bipedalwalker_cont_sampled_efficientzero_config.py
--rw-r--r--   0 puyuan     (501) 453037844     4768 2023-08-21 13:43:50.000000 LightZero-0.0.2/zoo/box2d/bipedalwalker/config/tmp.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.344223 LightZero-0.0.2/zoo/box2d/bipedalwalker/entry/
--rw-r--r--   0 puyuan     (501) 453037844        0 2023-10-10 08:13:34.000000 LightZero-0.0.2/zoo/box2d/bipedalwalker/entry/__init__.py
--rw-r--r--   0 puyuan     (501) 453037844     1621 2023-10-10 08:13:34.000000 LightZero-0.0.2/zoo/box2d/bipedalwalker/entry/bipedalwalker_eval.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.344529 LightZero-0.0.2/zoo/box2d/bipedalwalker/envs/
--rw-r--r--   0 puyuan     (501) 453037844        0 2023-05-24 10:01:46.000000 LightZero-0.0.2/zoo/box2d/bipedalwalker/envs/__init__.py
--rw-r--r--   0 puyuan     (501) 453037844     7935 2023-10-10 08:13:34.000000 LightZero-0.0.2/zoo/box2d/bipedalwalker/envs/bipedalwalker_cont_disc_env.py
--rw-r--r--   0 puyuan     (501) 453037844     6647 2023-10-13 09:55:49.000000 LightZero-0.0.2/zoo/box2d/bipedalwalker/envs/bipedalwalker_env.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.344648 LightZero-0.0.2/zoo/box2d/lunarlander/
--rw-r--r--   0 puyuan     (501) 453037844        0 2023-04-14 09:11:22.000000 LightZero-0.0.2/zoo/box2d/lunarlander/__init__.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.345556 LightZero-0.0.2/zoo/box2d/lunarlander/config/
--rw-r--r--   0 puyuan     (501) 453037844        0 2023-04-14 09:11:22.000000 LightZero-0.0.2/zoo/box2d/lunarlander/config/__init__.py
--rw-r--r--   0 puyuan     (501) 453037844     3996 2023-10-10 08:32:30.000000 LightZero-0.0.2/zoo/box2d/lunarlander/config/lunarlander_cont_disc_efficientzero_config.py
--rw-r--r--   0 puyuan     (501) 453037844     4010 2023-10-10 08:32:30.000000 LightZero-0.0.2/zoo/box2d/lunarlander/config/lunarlander_cont_disc_sampled_efficientzero_config.py
--rw-r--r--   0 puyuan     (501) 453037844     4053 2023-10-31 13:06:51.000000 LightZero-0.0.2/zoo/box2d/lunarlander/config/lunarlander_cont_sampled_efficientzero_config.py
--rw-r--r--   0 puyuan     (501) 453037844     3435 2023-10-10 08:32:30.000000 LightZero-0.0.2/zoo/box2d/lunarlander/config/lunarlander_disc_efficientzero_config.py
--rw-r--r--   0 puyuan     (501) 453037844     3633 2023-11-13 12:09:06.000000 LightZero-0.0.2/zoo/box2d/lunarlander/config/lunarlander_disc_gumbel_muzero_config.py
--rw-r--r--   0 puyuan     (501) 453037844     3662 2023-10-13 09:55:49.000000 LightZero-0.0.2/zoo/box2d/lunarlander/config/lunarlander_disc_muzero_config.py
--rw-r--r--   0 puyuan     (501) 453037844     3765 2023-10-10 08:13:34.000000 LightZero-0.0.2/zoo/box2d/lunarlander/config/lunarlander_disc_stochastic_muzero_config.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.345771 LightZero-0.0.2/zoo/box2d/lunarlander/entry/
--rw-r--r--   0 puyuan     (501) 453037844        0 2023-10-10 08:13:34.000000 LightZero-0.0.2/zoo/box2d/lunarlander/entry/__init__.py
--rw-r--r--   0 puyuan     (501) 453037844     1602 2023-10-10 08:13:34.000000 LightZero-0.0.2/zoo/box2d/lunarlander/entry/lunarlander_eval.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.346219 LightZero-0.0.2/zoo/box2d/lunarlander/envs/
--rwxr-xr-x   0 puyuan     (501) 453037844       44 2023-04-14 09:11:22.000000 LightZero-0.0.2/zoo/box2d/lunarlander/envs/__init__.py
--rwxr-xr-x   0 puyuan     (501) 453037844     8243 2023-05-24 10:01:46.000000 LightZero-0.0.2/zoo/box2d/lunarlander/envs/lunarlander_cont_disc_env.py
--rwxr-xr-x   0 puyuan     (501) 453037844     6905 2023-05-24 10:01:46.000000 LightZero-0.0.2/zoo/box2d/lunarlander/envs/lunarlander_env.py
--rwxr-xr-x   0 puyuan     (501) 453037844     1429 2023-05-24 10:01:46.000000 LightZero-0.0.2/zoo/box2d/lunarlander/envs/test_lunarlander_env.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.346323 LightZero-0.0.2/zoo/classic_control/
--rw-r--r--   0 puyuan     (501) 453037844        0 2023-04-14 09:11:22.000000 LightZero-0.0.2/zoo/classic_control/__init__.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.346417 LightZero-0.0.2/zoo/classic_control/cartpole/
--rw-r--r--   0 puyuan     (501) 453037844        0 2023-08-02 09:19:22.000000 LightZero-0.0.2/zoo/classic_control/cartpole/__init__.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.347158 LightZero-0.0.2/zoo/classic_control/cartpole/config/
--rw-r--r--   0 puyuan     (501) 453037844        0 2023-05-24 10:01:46.000000 LightZero-0.0.2/zoo/classic_control/cartpole/config/__init__.py
--rw-r--r--   0 puyuan     (501) 453037844     3306 2023-10-10 08:13:34.000000 LightZero-0.0.2/zoo/classic_control/cartpole/config/cartpole_efficientzero_config.py
--rw-r--r--   0 puyuan     (501) 453037844     3462 2023-11-13 12:09:06.000000 LightZero-0.0.2/zoo/classic_control/cartpole/config/cartpole_gumbel_muzero_config.py
--rw-r--r--   0 puyuan     (501) 453037844     3347 2023-10-10 08:13:34.000000 LightZero-0.0.2/zoo/classic_control/cartpole/config/cartpole_muzero_config.py
--rw-r--r--   0 puyuan     (501) 453037844     3693 2023-10-07 04:09:16.000000 LightZero-0.0.2/zoo/classic_control/cartpole/config/cartpole_muzero_config_ckpt.py
--rw-r--r--   0 puyuan     (501) 453037844     3558 2023-10-13 09:55:49.000000 LightZero-0.0.2/zoo/classic_control/cartpole/config/cartpole_sampled_efficientzero_config.py
--rw-r--r--   0 puyuan     (501) 453037844     2865 2023-10-10 08:13:34.000000 LightZero-0.0.2/zoo/classic_control/cartpole/config/cartpole_stochastic_muzero_config.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.347366 LightZero-0.0.2/zoo/classic_control/cartpole/entry/
--rw-r--r--   0 puyuan     (501) 453037844        0 2023-10-10 08:13:34.000000 LightZero-0.0.2/zoo/classic_control/cartpole/entry/__init__.py
--rw-r--r--   0 puyuan     (501) 453037844     1485 2023-10-10 08:13:34.000000 LightZero-0.0.2/zoo/classic_control/cartpole/entry/cartpole_eval.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.347579 LightZero-0.0.2/zoo/classic_control/cartpole/envs/
--rw-r--r--   0 puyuan     (501) 453037844        0 2023-05-24 10:01:46.000000 LightZero-0.0.2/zoo/classic_control/cartpole/envs/__init__.py
--rw-r--r--   0 puyuan     (501) 453037844     3889 2023-05-24 10:01:46.000000 LightZero-0.0.2/zoo/classic_control/cartpole/envs/cartpole_lightzero_env.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.347696 LightZero-0.0.2/zoo/classic_control/pendulum/
--rw-r--r--   0 puyuan     (501) 453037844        0 2023-04-14 09:11:22.000000 LightZero-0.0.2/zoo/classic_control/pendulum/__init__.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.348328 LightZero-0.0.2/zoo/classic_control/pendulum/config/
--rw-r--r--   0 puyuan     (501) 453037844        0 2023-04-14 09:11:22.000000 LightZero-0.0.2/zoo/classic_control/pendulum/config/__init__.py
--rw-r--r--   0 puyuan     (501) 453037844     3299 2023-10-10 08:13:34.000000 LightZero-0.0.2/zoo/classic_control/pendulum/config/pendulum_cont_disc_efficientzero_config.py
--rw-r--r--   0 puyuan     (501) 453037844     3644 2023-11-13 12:09:06.000000 LightZero-0.0.2/zoo/classic_control/pendulum/config/pendulum_cont_disc_gumbel_muzero_config.py
--rw-r--r--   0 puyuan     (501) 453037844     3528 2023-10-10 08:13:34.000000 LightZero-0.0.2/zoo/classic_control/pendulum/config/pendulum_cont_disc_muzero_config.py
--rw-r--r--   0 puyuan     (501) 453037844     3516 2023-10-10 08:13:34.000000 LightZero-0.0.2/zoo/classic_control/pendulum/config/pendulum_cont_disc_sampled_efficientzero_config.py
--rw-r--r--   0 puyuan     (501) 453037844     3823 2023-08-22 03:29:23.000000 LightZero-0.0.2/zoo/classic_control/pendulum/config/pendulum_cont_sampled_efficientzero_config.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.348512 LightZero-0.0.2/zoo/classic_control/pendulum/entry/
--rw-r--r--   0 puyuan     (501) 453037844        0 2023-10-10 08:13:34.000000 LightZero-0.0.2/zoo/classic_control/pendulum/entry/__init__.py
--rw-r--r--   0 puyuan     (501) 453037844     1621 2023-10-10 08:13:34.000000 LightZero-0.0.2/zoo/classic_control/pendulum/entry/pendulum_eval.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.348733 LightZero-0.0.2/zoo/classic_control/pendulum/envs/
--rw-r--r--   0 puyuan     (501) 453037844        0 2023-04-14 09:11:22.000000 LightZero-0.0.2/zoo/classic_control/pendulum/envs/__init__.py
--rw-r--r--   0 puyuan     (501) 453037844     5470 2023-05-24 10:01:46.000000 LightZero-0.0.2/zoo/classic_control/pendulum/envs/pendulum_lightzero_env.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.348836 LightZero-0.0.2/zoo/game_2048/
--rw-r--r--   0 puyuan     (501) 453037844        0 2023-10-10 08:13:34.000000 LightZero-0.0.2/zoo/game_2048/__init__.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.349150 LightZero-0.0.2/zoo/game_2048/entry/
--rw-r--r--   0 puyuan     (501) 453037844     1963 2023-10-10 08:13:34.000000 LightZero-0.0.2/zoo/game_2048/entry/2048_bot_eval.py
--rw-r--r--   0 puyuan     (501) 453037844     2316 2023-10-10 08:13:34.000000 LightZero-0.0.2/zoo/game_2048/entry/2048_eval.py
--rw-r--r--   0 puyuan     (501) 453037844        0 2023-10-10 08:13:34.000000 LightZero-0.0.2/zoo/game_2048/entry/__init__.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.349579 LightZero-0.0.2/zoo/game_2048/envs/
--rw-r--r--   0 puyuan     (501) 453037844        0 2023-10-10 08:13:34.000000 LightZero-0.0.2/zoo/game_2048/envs/__init__.py
--rw-r--r--   0 puyuan     (501) 453037844     5468 2023-10-10 08:13:34.000000 LightZero-0.0.2/zoo/game_2048/envs/expectimax_search_based_bot.py
--rw-r--r--   0 puyuan     (501) 453037844    37246 2023-10-10 08:13:34.000000 LightZero-0.0.2/zoo/game_2048/envs/game_2048_env.py
--rw-r--r--   0 puyuan     (501) 453037844     7276 2023-10-10 08:13:34.000000 LightZero-0.0.2/zoo/game_2048/envs/test_game_2048_env.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.349681 LightZero-0.0.2/zoo/minigrid/
--rw-r--r--   0 puyuan     (501) 453037844        0 2023-10-30 04:54:58.000000 LightZero-0.0.2/zoo/minigrid/__init__.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.350167 LightZero-0.0.2/zoo/minigrid/config/
--rw-r--r--   0 puyuan     (501) 453037844        0 2023-10-30 04:54:58.000000 LightZero-0.0.2/zoo/minigrid/config/__init__.py
--rw-r--r--   0 puyuan     (501) 453037844     4464 2023-10-30 04:54:58.000000 LightZero-0.0.2/zoo/minigrid/config/minigrd_sampled_efficientzero_config.py
--rw-r--r--   0 puyuan     (501) 453037844     3605 2023-10-30 04:54:58.000000 LightZero-0.0.2/zoo/minigrid/config/minigrid_efficientzero_config.py
--rw-r--r--   0 puyuan     (501) 453037844     3825 2023-10-30 04:54:58.000000 LightZero-0.0.2/zoo/minigrid/config/minigrid_muzero_config.py
--rw-r--r--   0 puyuan     (501) 453037844     5510 2023-10-30 04:54:58.000000 LightZero-0.0.2/zoo/minigrid/config/minigrid_muzero_rnd_config.py
-drwxr-xr-x   0 puyuan     (501) 453037844        0 2023-11-19 12:18:05.350371 LightZero-0.0.2/zoo/minigrid/entry/
--rw-r--r--   0 puyuan     (501) 453037844        0 2023-10-30 04:54:58.000000 LightZero-0.0.2/zoo/minigrid/entry/__init__.py
--rw-r--r--   0 puyuan     (501) 453037844     1505 2023-10-30 04:54:58.000000 LightZero-0.0.2/zoo/minigrid/entry/minigrid_eval.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:43.037816 LightZero-0.0.5/
+-rw-r--r--   0 puyuan     (501) 453037844    11357 2023-04-14 09:11:22.000000 LightZero-0.0.5/LICENSE
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:43.035267 LightZero-0.0.5/LightZero.egg-info/
+-rw-r--r--   0 puyuan     (501) 453037844     3014 2024-04-12 05:04:42.000000 LightZero-0.0.5/LightZero.egg-info/PKG-INFO
+-rw-r--r--   0 puyuan     (501) 453037844    17114 2024-04-12 05:04:42.000000 LightZero-0.0.5/LightZero.egg-info/SOURCES.txt
+-rw-r--r--   0 puyuan     (501) 453037844        1 2024-04-12 05:04:42.000000 LightZero-0.0.5/LightZero.egg-info/dependency_links.txt
+-rw-r--r--   0 puyuan     (501) 453037844      728 2024-04-12 05:04:42.000000 LightZero-0.0.5/LightZero.egg-info/requires.txt
+-rw-r--r--   0 puyuan     (501) 453037844       10 2024-04-12 05:04:42.000000 LightZero-0.0.5/LightZero.egg-info/top_level.txt
+-rw-r--r--   0 puyuan     (501) 453037844     3014 2024-04-12 05:04:43.037595 LightZero-0.0.5/PKG-INFO
+-rw-r--r--   0 puyuan     (501) 453037844    40651 2024-04-12 04:43:12.000000 LightZero-0.0.5/README.md
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:42.937344 LightZero-0.0.5/lzero/
+-rw-r--r--   0 puyuan     (501) 453037844       52 2023-05-24 10:01:45.000000 LightZero-0.0.5/lzero/__init__.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:42.938917 LightZero-0.0.5/lzero/agent/
+-rw-r--r--   0 puyuan     (501) 453037844      275 2024-02-21 06:58:36.000000 LightZero-0.0.5/lzero/agent/__init__.py
+-rw-r--r--   0 puyuan     (501) 453037844    16988 2024-02-21 06:58:36.000000 LightZero-0.0.5/lzero/agent/alphazero.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:42.939067 LightZero-0.0.5/lzero/agent/config/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-12-07 08:13:35.000000 LightZero-0.0.5/lzero/agent/config/__init__.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:42.939576 LightZero-0.0.5/lzero/agent/config/alphazero/
+-rw-r--r--   0 puyuan     (501) 453037844      341 2024-02-21 06:58:36.000000 LightZero-0.0.5/lzero/agent/config/alphazero/__init__.py
+-rw-r--r--   0 puyuan     (501) 453037844     3757 2024-02-21 06:58:36.000000 LightZero-0.0.5/lzero/agent/config/alphazero/gomoku_play_with_bot.py
+-rw-r--r--   0 puyuan     (501) 453037844     3625 2024-02-21 06:58:36.000000 LightZero-0.0.5/lzero/agent/config/alphazero/tictactoe_play_with_bot.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:42.941217 LightZero-0.0.5/lzero/agent/config/efficientzero/
+-rw-r--r--   0 puyuan     (501) 453037844      794 2024-02-21 06:58:36.000000 LightZero-0.0.5/lzero/agent/config/efficientzero/__init__.py
+-rw-r--r--   0 puyuan     (501) 453037844     3076 2024-02-21 06:58:36.000000 LightZero-0.0.5/lzero/agent/config/efficientzero/gym_breakoutnoframeskip_v4.py
+-rw-r--r--   0 puyuan     (501) 453037844     2549 2024-02-21 06:58:36.000000 LightZero-0.0.5/lzero/agent/config/efficientzero/gym_cartpole_v0.py
+-rw-r--r--   0 puyuan     (501) 453037844     2631 2024-02-21 06:58:36.000000 LightZero-0.0.5/lzero/agent/config/efficientzero/gym_lunarlander_v2.py
+-rw-r--r--   0 puyuan     (501) 453037844     2985 2024-02-21 06:58:36.000000 LightZero-0.0.5/lzero/agent/config/efficientzero/gym_mspacmannoframeskip_v4.py
+-rw-r--r--   0 puyuan     (501) 453037844     2507 2024-02-21 06:58:36.000000 LightZero-0.0.5/lzero/agent/config/efficientzero/gym_pendulum_v1.py
+-rw-r--r--   0 puyuan     (501) 453037844     2977 2024-02-21 06:58:36.000000 LightZero-0.0.5/lzero/agent/config/efficientzero/gym_pongnoframeskip_v4.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:42.942146 LightZero-0.0.5/lzero/agent/config/gumbel_muzero/
+-rw-r--r--   0 puyuan     (501) 453037844      441 2024-02-21 06:58:36.000000 LightZero-0.0.5/lzero/agent/config/gumbel_muzero/__init__.py
+-rw-r--r--   0 puyuan     (501) 453037844     3383 2024-02-21 06:58:36.000000 LightZero-0.0.5/lzero/agent/config/gumbel_muzero/gomoku_play_with_bot.py
+-rw-r--r--   0 puyuan     (501) 453037844     2736 2024-02-21 06:58:36.000000 LightZero-0.0.5/lzero/agent/config/gumbel_muzero/gym_cartpole_v0.py
+-rw-r--r--   0 puyuan     (501) 453037844     3042 2024-02-21 06:58:36.000000 LightZero-0.0.5/lzero/agent/config/gumbel_muzero/tictactoe_play_with_bot.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:42.944714 LightZero-0.0.5/lzero/agent/config/muzero/
+-rw-r--r--   0 puyuan     (501) 453037844     1031 2024-02-21 06:58:36.000000 LightZero-0.0.5/lzero/agent/config/muzero/__init__.py
+-rw-r--r--   0 puyuan     (501) 453037844     3321 2024-02-21 06:58:36.000000 LightZero-0.0.5/lzero/agent/config/muzero/gomoku_play_with_bot.py
+-rw-r--r--   0 puyuan     (501) 453037844     3226 2024-02-21 06:58:36.000000 LightZero-0.0.5/lzero/agent/config/muzero/gym_breakoutnoframeskip_v4.py
+-rw-r--r--   0 puyuan     (501) 453037844     2672 2023-12-07 08:13:35.000000 LightZero-0.0.5/lzero/agent/config/muzero/gym_cartpole_v0.py
+-rw-r--r--   0 puyuan     (501) 453037844     2907 2024-02-21 06:58:36.000000 LightZero-0.0.5/lzero/agent/config/muzero/gym_lunarlander_v2.py
+-rw-r--r--   0 puyuan     (501) 453037844     3134 2024-02-21 06:58:36.000000 LightZero-0.0.5/lzero/agent/config/muzero/gym_mspacmannoframeskip_v4.py
+-rw-r--r--   0 puyuan     (501) 453037844     2619 2024-02-21 06:58:36.000000 LightZero-0.0.5/lzero/agent/config/muzero/gym_pendulum_v1.py
+-rw-r--r--   0 puyuan     (501) 453037844     3126 2024-02-21 06:58:36.000000 LightZero-0.0.5/lzero/agent/config/muzero/gym_pongnoframeskip_v4.py
+-rw-r--r--   0 puyuan     (501) 453037844     3013 2024-02-21 06:58:36.000000 LightZero-0.0.5/lzero/agent/config/muzero/tictactoe_play_with_bot.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:42.945278 LightZero-0.0.5/lzero/agent/config/sampled_alphazero/
+-rw-r--r--   0 puyuan     (501) 453037844      341 2024-02-21 06:58:36.000000 LightZero-0.0.5/lzero/agent/config/sampled_alphazero/__init__.py
+-rw-r--r--   0 puyuan     (501) 453037844     4134 2024-02-21 06:58:36.000000 LightZero-0.0.5/lzero/agent/config/sampled_alphazero/gomoku_play_with_bot.py
+-rw-r--r--   0 puyuan     (501) 453037844     3763 2024-02-21 06:58:36.000000 LightZero-0.0.5/lzero/agent/config/sampled_alphazero/tictactoe_play_with_bot.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:42.946632 LightZero-0.0.5/lzero/agent/config/sampled_efficientzero/
+-rw-r--r--   0 puyuan     (501) 453037844      824 2024-02-21 06:58:36.000000 LightZero-0.0.5/lzero/agent/config/sampled_efficientzero/__init__.py
+-rw-r--r--   0 puyuan     (501) 453037844     2763 2024-02-21 06:58:36.000000 LightZero-0.0.5/lzero/agent/config/sampled_efficientzero/gym_breakoutnoframeskip_v4.py
+-rw-r--r--   0 puyuan     (501) 453037844     2743 2024-02-21 06:58:36.000000 LightZero-0.0.5/lzero/agent/config/sampled_efficientzero/gym_cartpole_v0.py
+-rw-r--r--   0 puyuan     (501) 453037844     3068 2024-02-21 06:58:36.000000 LightZero-0.0.5/lzero/agent/config/sampled_efficientzero/gym_lunarlandercontinuous_v2.py
+-rw-r--r--   0 puyuan     (501) 453037844     2763 2024-02-21 06:58:36.000000 LightZero-0.0.5/lzero/agent/config/sampled_efficientzero/gym_mspacmannoframeskip_v4.py
+-rw-r--r--   0 puyuan     (501) 453037844     2878 2024-02-21 06:58:36.000000 LightZero-0.0.5/lzero/agent/config/sampled_efficientzero/gym_pendulum_v1.py
+-rw-r--r--   0 puyuan     (501) 453037844     2755 2024-02-21 06:58:36.000000 LightZero-0.0.5/lzero/agent/config/sampled_efficientzero/gym_pongnoframeskip_v4.py
+-rw-r--r--   0 puyuan     (501) 453037844    19658 2024-02-21 06:58:36.000000 LightZero-0.0.5/lzero/agent/efficientzero.py
+-rw-r--r--   0 puyuan     (501) 453037844    19604 2024-02-21 06:58:36.000000 LightZero-0.0.5/lzero/agent/gumbel_muzero.py
+-rw-r--r--   0 puyuan     (501) 453037844    19511 2024-02-21 06:58:36.000000 LightZero-0.0.5/lzero/agent/muzero.py
+-rw-r--r--   0 puyuan     (501) 453037844    17031 2024-02-21 06:58:36.000000 LightZero-0.0.5/lzero/agent/sampled_alphazero.py
+-rw-r--r--   0 puyuan     (501) 453037844    19810 2024-02-21 06:58:36.000000 LightZero-0.0.5/lzero/agent/sampled_efficientzero.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:42.947203 LightZero-0.0.5/lzero/config/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-05-24 10:01:45.000000 LightZero-0.0.5/lzero/config/__init__.py
+-rw-r--r--   0 puyuan     (501) 453037844      490 2023-12-07 08:13:50.000000 LightZero-0.0.5/lzero/config/meta.py
+-rw-r--r--   0 puyuan     (501) 453037844      542 2023-10-10 08:13:33.000000 LightZero-0.0.5/lzero/config/utils.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:42.949827 LightZero-0.0.5/lzero/entry/
+-rw-r--r--   0 puyuan     (501) 453037844      366 2024-03-30 09:59:19.000000 LightZero-0.0.5/lzero/entry/__init__.py
+-rw-r--r--   0 puyuan     (501) 453037844     4049 2024-02-21 06:58:36.000000 LightZero-0.0.5/lzero/entry/eval_alphazero.py
+-rw-r--r--   0 puyuan     (501) 453037844     4512 2024-03-30 09:59:19.000000 LightZero-0.0.5/lzero/entry/eval_muzero.py
+-rw-r--r--   0 puyuan     (501) 453037844     4998 2024-02-21 06:58:36.000000 LightZero-0.0.5/lzero/entry/eval_muzero_with_gym_env.py
+-rw-r--r--   0 puyuan     (501) 453037844     6324 2024-04-10 09:15:39.000000 LightZero-0.0.5/lzero/entry/train_alphazero.py
+-rw-r--r--   0 puyuan     (501) 453037844    10604 2024-03-30 09:59:19.000000 LightZero-0.0.5/lzero/entry/train_muzero.py
+-rw-r--r--   0 puyuan     (501) 453037844     7810 2024-02-21 06:58:36.000000 LightZero-0.0.5/lzero/entry/train_muzero_with_gym_env.py
+-rw-r--r--   0 puyuan     (501) 453037844    10008 2023-11-27 13:16:04.000000 LightZero-0.0.5/lzero/entry/train_muzero_with_reward_model.py
+-rw-r--r--   0 puyuan     (501) 453037844     3318 2024-03-30 09:59:19.000000 LightZero-0.0.5/lzero/entry/utils.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:42.950331 LightZero-0.0.5/lzero/envs/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-05-24 10:01:45.000000 LightZero-0.0.5/lzero/envs/__init__.py
+-rw-r--r--   0 puyuan     (501) 453037844     1110 2024-02-21 06:58:36.000000 LightZero-0.0.5/lzero/envs/get_wrapped_env.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:42.950950 LightZero-0.0.5/lzero/envs/tests/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-05-24 10:01:45.000000 LightZero-0.0.5/lzero/envs/tests/__init__.py
+-rw-r--r--   0 puyuan     (501) 453037844      917 2023-12-07 08:13:35.000000 LightZero-0.0.5/lzero/envs/tests/test_ding_env_wrapper.py
+-rw-r--r--   0 puyuan     (501) 453037844     4582 2024-02-21 06:58:36.000000 LightZero-0.0.5/lzero/envs/tests/test_lightzero_env_wrapper.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:42.951650 LightZero-0.0.5/lzero/envs/wrappers/
+-rw-r--r--   0 puyuan     (501) 453037844       86 2023-05-24 10:01:45.000000 LightZero-0.0.5/lzero/envs/wrappers/__init__.py
+-rw-r--r--   0 puyuan     (501) 453037844     3671 2024-02-21 06:58:36.000000 LightZero-0.0.5/lzero/envs/wrappers/action_discretization_env_wrapper.py
+-rw-r--r--   0 puyuan     (501) 453037844     4523 2024-02-21 06:58:36.000000 LightZero-0.0.5/lzero/envs/wrappers/lightzero_env_wrapper.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:42.952163 LightZero-0.0.5/lzero/mcts/
+-rw-r--r--   0 puyuan     (501) 453037844       91 2023-05-24 10:01:45.000000 LightZero-0.0.5/lzero/mcts/__init__.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:42.955186 LightZero-0.0.5/lzero/mcts/buffer/
+-rw-r--r--   0 puyuan     (501) 453037844      322 2024-03-30 09:59:19.000000 LightZero-0.0.5/lzero/mcts/buffer/__init__.py
+-rw-r--r--   0 puyuan     (501) 453037844    18135 2024-03-30 09:59:19.000000 LightZero-0.0.5/lzero/mcts/buffer/game_buffer.py
+-rw-r--r--   0 puyuan     (501) 453037844    25797 2024-03-13 12:25:48.000000 LightZero-0.0.5/lzero/mcts/buffer/game_buffer_efficientzero.py
+-rw-r--r--   0 puyuan     (501) 453037844     5867 2024-01-07 11:33:44.000000 LightZero-0.0.5/lzero/mcts/buffer/game_buffer_gumbel_muzero.py
+-rw-r--r--   0 puyuan     (501) 453037844    37742 2024-03-30 09:59:19.000000 LightZero-0.0.5/lzero/mcts/buffer/game_buffer_muzero.py
+-rw-r--r--   0 puyuan     (501) 453037844    32688 2024-03-13 12:25:48.000000 LightZero-0.0.5/lzero/mcts/buffer/game_buffer_sampled_efficientzero.py
+-rw-r--r--   0 puyuan     (501) 453037844     8182 2023-12-07 08:13:35.000000 LightZero-0.0.5/lzero/mcts/buffer/game_buffer_stochastic_muzero.py
+-rw-r--r--   0 puyuan     (501) 453037844    15478 2024-03-30 09:59:19.000000 LightZero-0.0.5/lzero/mcts/buffer/game_segment.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:42.955485 LightZero-0.0.5/lzero/mcts/ctree/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-04-14 09:11:22.000000 LightZero-0.0.5/lzero/mcts/ctree/__init__.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:42.955800 LightZero-0.0.5/lzero/mcts/ctree/common_lib/
+-rw-r--r--   0 puyuan     (501) 453037844     1661 2023-05-24 10:01:45.000000 LightZero-0.0.5/lzero/mcts/ctree/common_lib/cminimax.cpp
+-rw-r--r--   0 puyuan     (501) 453037844      785 2023-05-24 10:01:45.000000 LightZero-0.0.5/lzero/mcts/ctree/common_lib/cminimax.h
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:42.956025 LightZero-0.0.5/lzero/mcts/ctree/ctree_efficientzero/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-04-14 09:11:22.000000 LightZero-0.0.5/lzero/mcts/ctree/ctree_efficientzero/__init__.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:42.956520 LightZero-0.0.5/lzero/mcts/ctree/ctree_efficientzero/lib/
+-rw-r--r--   0 puyuan     (501) 453037844    26754 2024-03-13 12:25:48.000000 LightZero-0.0.5/lzero/mcts/ctree/ctree_efficientzero/lib/cnode.cpp
+-rw-r--r--   0 puyuan     (501) 453037844     3973 2023-08-02 09:19:21.000000 LightZero-0.0.5/lzero/mcts/ctree/ctree_efficientzero/lib/cnode.h
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:42.956764 LightZero-0.0.5/lzero/mcts/ctree/ctree_gumbel_muzero/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-08-02 09:19:21.000000 LightZero-0.0.5/lzero/mcts/ctree/ctree_gumbel_muzero/__init__.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:42.957860 LightZero-0.0.5/lzero/mcts/ctree/ctree_gumbel_muzero/lib/
+-rw-r--r--   0 puyuan     (501) 453037844    41503 2024-02-21 06:58:36.000000 LightZero-0.0.5/lzero/mcts/ctree/ctree_gumbel_muzero/lib/cnode.cpp
+-rw-r--r--   0 puyuan     (501) 453037844     5537 2023-08-02 09:19:21.000000 LightZero-0.0.5/lzero/mcts/ctree/ctree_gumbel_muzero/lib/cnode.h
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:42.958365 LightZero-0.0.5/lzero/mcts/ctree/ctree_muzero/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-04-14 09:11:22.000000 LightZero-0.0.5/lzero/mcts/ctree/ctree_muzero/__init__.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:42.958992 LightZero-0.0.5/lzero/mcts/ctree/ctree_muzero/lib/
+-rw-r--r--   0 puyuan     (501) 453037844    22180 2024-03-13 12:25:48.000000 LightZero-0.0.5/lzero/mcts/ctree/ctree_muzero/lib/cnode.cpp
+-rw-r--r--   0 puyuan     (501) 453037844     3782 2023-11-27 13:16:04.000000 LightZero-0.0.5/lzero/mcts/ctree/ctree_muzero/lib/cnode.h
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:42.959239 LightZero-0.0.5/lzero/mcts/ctree/ctree_sampled_efficientzero/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-04-14 09:11:22.000000 LightZero-0.0.5/lzero/mcts/ctree/ctree_sampled_efficientzero/__init__.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:42.959543 LightZero-0.0.5/lzero/mcts/ctree/ctree_sampled_efficientzero/lib/
+-rw-r--r--   0 puyuan     (501) 453037844    46208 2024-02-21 06:58:36.000000 LightZero-0.0.5/lzero/mcts/ctree/ctree_sampled_efficientzero/lib/cnode.cpp
+-rw-r--r--   0 puyuan     (501) 453037844     4955 2023-10-13 09:55:49.000000 LightZero-0.0.5/lzero/mcts/ctree/ctree_sampled_efficientzero/lib/cnode.h
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:42.959834 LightZero-0.0.5/lzero/mcts/ctree/ctree_stochastic_muzero/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-10-10 08:13:33.000000 LightZero-0.0.5/lzero/mcts/ctree/ctree_stochastic_muzero/__init__.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:42.960283 LightZero-0.0.5/lzero/mcts/ctree/ctree_stochastic_muzero/lib/
+-rw-r--r--   0 puyuan     (501) 453037844    26958 2024-02-21 06:58:36.000000 LightZero-0.0.5/lzero/mcts/ctree/ctree_stochastic_muzero/lib/cnode.cpp
+-rw-r--r--   0 puyuan     (501) 453037844     4089 2023-10-10 08:13:33.000000 LightZero-0.0.5/lzero/mcts/ctree/ctree_stochastic_muzero/lib/cnode.h
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:42.966912 LightZero-0.0.5/lzero/mcts/ptree/
+-rw-r--r--   0 puyuan     (501) 453037844       23 2023-05-24 10:01:45.000000 LightZero-0.0.5/lzero/mcts/ptree/__init__.py
+-rw-r--r--   0 puyuan     (501) 453037844     2900 2024-02-21 06:58:36.000000 LightZero-0.0.5/lzero/mcts/ptree/minimax.py
+-rw-r--r--   0 puyuan     (501) 453037844    22393 2024-04-10 04:50:28.000000 LightZero-0.0.5/lzero/mcts/ptree/ptree_az.py
+-rw-r--r--   0 puyuan     (501) 453037844    24894 2024-01-07 11:33:44.000000 LightZero-0.0.5/lzero/mcts/ptree/ptree_az_sampled.py
+-rw-r--r--   0 puyuan     (501) 453037844    26924 2024-03-13 12:25:48.000000 LightZero-0.0.5/lzero/mcts/ptree/ptree_ez.py
+-rw-r--r--   0 puyuan     (501) 453037844    25044 2024-02-21 06:58:36.000000 LightZero-0.0.5/lzero/mcts/ptree/ptree_mz.py
+-rw-r--r--   0 puyuan     (501) 453037844    38894 2024-02-21 06:58:36.000000 LightZero-0.0.5/lzero/mcts/ptree/ptree_sez.py
+-rw-r--r--   0 puyuan     (501) 453037844    27108 2024-02-21 06:58:36.000000 LightZero-0.0.5/lzero/mcts/ptree/ptree_stochastic_mz.py
+-rw-r--r--   0 puyuan     (501) 453037844      599 2023-04-14 09:11:22.000000 LightZero-0.0.5/lzero/mcts/ptree/test_sez_sample.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:42.972427 LightZero-0.0.5/lzero/mcts/tests/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-10-10 08:13:33.000000 LightZero-0.0.5/lzero/mcts/tests/__init__.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:42.973223 LightZero-0.0.5/lzero/mcts/tests/config/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-10-10 08:13:33.000000 LightZero-0.0.5/lzero/mcts/tests/config/__init__.py
+-rw-r--r--   0 puyuan     (501) 453037844     3564 2024-03-13 12:25:48.000000 LightZero-0.0.5/lzero/mcts/tests/config/atari_efficientzero_config_for_test.py
+-rw-r--r--   0 puyuan     (501) 453037844     3552 2024-03-30 09:59:19.000000 LightZero-0.0.5/lzero/mcts/tests/config/tictactoe_muzero_bot_mode_config_for_test.py
+-rw-r--r--   0 puyuan     (501) 453037844     4804 2023-11-27 13:16:04.000000 LightZero-0.0.5/lzero/mcts/tests/cprofile_mcts_ptree.py
+-rw-r--r--   0 puyuan     (501) 453037844    14991 2023-11-27 13:16:04.000000 LightZero-0.0.5/lzero/mcts/tests/eval_tree_speed.py
+-rw-r--r--   0 puyuan     (501) 453037844     2809 2023-12-07 08:13:35.000000 LightZero-0.0.5/lzero/mcts/tests/test_game_buffer.py
+-rw-r--r--   0 puyuan     (501) 453037844     6861 2024-03-30 09:59:19.000000 LightZero-0.0.5/lzero/mcts/tests/test_game_segment.py
+-rw-r--r--   0 puyuan     (501) 453037844      340 2023-05-24 10:01:45.000000 LightZero-0.0.5/lzero/mcts/tests/test_image_transform.py
+-rw-r--r--   0 puyuan     (501) 453037844    14840 2024-03-13 12:25:48.000000 LightZero-0.0.5/lzero/mcts/tests/test_mcts_ctree.py
+-rw-r--r--   0 puyuan     (501) 453037844    11751 2024-03-13 12:25:48.000000 LightZero-0.0.5/lzero/mcts/tests/test_mcts_ptree.py
+-rw-r--r--   0 puyuan     (501) 453037844     5088 2024-03-13 12:25:48.000000 LightZero-0.0.5/lzero/mcts/tests/test_mcts_sampled_ctree.py
+-rw-r--r--   0 puyuan     (501) 453037844     5509 2024-03-30 09:59:19.000000 LightZero-0.0.5/lzero/mcts/tests/test_muzero_game_buffer.py
+-rw-r--r--   0 puyuan     (501) 453037844     4036 2024-02-21 14:08:19.000000 LightZero-0.0.5/lzero/mcts/tests/test_muzero_game_buffer_local_tmp.py
+-rw-r--r--   0 puyuan     (501) 453037844     5088 2024-02-23 08:30:27.000000 LightZero-0.0.5/lzero/mcts/tests/test_muzero_game_buffer_script_tmp.py
+-rw-r--r--   0 puyuan     (501) 453037844     1016 2023-05-24 10:01:45.000000 LightZero-0.0.5/lzero/mcts/tests/test_utils.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:42.975417 LightZero-0.0.5/lzero/mcts/tree_search/
+-rw-r--r--   0 puyuan     (501) 453037844      397 2023-10-13 09:55:49.000000 LightZero-0.0.5/lzero/mcts/tree_search/__init__.py
+-rw-r--r--   0 puyuan     (501) 453037844    31259 2024-03-30 09:59:19.000000 LightZero-0.0.5/lzero/mcts/tree_search/mcts_ctree.py
+-rw-r--r--   0 puyuan     (501) 453037844    13035 2024-03-13 12:25:48.000000 LightZero-0.0.5/lzero/mcts/tree_search/mcts_ctree_sampled.py
+-rw-r--r--   0 puyuan     (501) 453037844    14333 2024-03-13 12:25:48.000000 LightZero-0.0.5/lzero/mcts/tree_search/mcts_ctree_stochastic.py
+-rw-r--r--   0 puyuan     (501) 453037844    21744 2024-03-13 12:25:48.000000 LightZero-0.0.5/lzero/mcts/tree_search/mcts_ptree.py
+-rw-r--r--   0 puyuan     (501) 453037844    12875 2024-03-13 12:25:48.000000 LightZero-0.0.5/lzero/mcts/tree_search/mcts_ptree_sampled.py
+-rw-r--r--   0 puyuan     (501) 453037844    14208 2024-03-13 12:25:48.000000 LightZero-0.0.5/lzero/mcts/tree_search/mcts_ptree_stochastic.py
+-rw-r--r--   0 puyuan     (501) 453037844     6302 2024-03-13 12:25:48.000000 LightZero-0.0.5/lzero/mcts/utils.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:42.981745 LightZero-0.0.5/lzero/model/
+-rw-r--r--   0 puyuan     (501) 453037844       68 2023-05-24 10:01:45.000000 LightZero-0.0.5/lzero/model/__init__.py
+-rw-r--r--   0 puyuan     (501) 453037844    17173 2023-12-02 15:34:44.000000 LightZero-0.0.5/lzero/model/alphazero_model.py
+-rw-r--r--   0 puyuan     (501) 453037844    21950 2024-03-30 09:59:19.000000 LightZero-0.0.5/lzero/model/common.py
+-rw-r--r--   0 puyuan     (501) 453037844    32014 2024-03-30 09:59:19.000000 LightZero-0.0.5/lzero/model/efficientzero_model.py
+-rw-r--r--   0 puyuan     (501) 453037844    26915 2023-11-27 06:56:20.000000 LightZero-0.0.5/lzero/model/efficientzero_model_mlp.py
+-rw-r--r--   0 puyuan     (501) 453037844     4173 2023-05-24 10:01:46.000000 LightZero-0.0.5/lzero/model/image_transform.py
+-rw-r--r--   0 puyuan     (501) 453037844    28672 2024-03-30 09:59:19.000000 LightZero-0.0.5/lzero/model/muzero_model.py
+-rw-r--r--   0 puyuan     (501) 453037844    24178 2023-11-27 06:56:20.000000 LightZero-0.0.5/lzero/model/muzero_model_mlp.py
+-rw-r--r--   0 puyuan     (501) 453037844    36999 2023-12-22 06:44:47.000000 LightZero-0.0.5/lzero/model/sampled_efficientzero_model.py
+-rw-r--r--   0 puyuan     (501) 453037844    29429 2023-12-22 06:41:44.000000 LightZero-0.0.5/lzero/model/sampled_efficientzero_model_mlp.py
+-rw-r--r--   0 puyuan     (501) 453037844    41962 2023-10-10 08:13:34.000000 LightZero-0.0.5/lzero/model/stochastic_muzero_model.py
+-rw-r--r--   0 puyuan     (501) 453037844    19412 2023-10-10 08:13:34.000000 LightZero-0.0.5/lzero/model/stochastic_muzero_model_mlp.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:42.982950 LightZero-0.0.5/lzero/model/tests/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-04-14 09:11:22.000000 LightZero-0.0.5/lzero/model/tests/__init__.py
+-rw-r--r--   0 puyuan     (501) 453037844     4554 2023-12-02 15:34:44.000000 LightZero-0.0.5/lzero/model/tests/test_alphazero_model.py
+-rw-r--r--   0 puyuan     (501) 453037844      957 2023-04-14 09:11:22.000000 LightZero-0.0.5/lzero/model/tests/test_common.py
+-rw-r--r--   0 puyuan     (501) 453037844     6687 2023-08-02 09:19:21.000000 LightZero-0.0.5/lzero/model/tests/test_efficientzero_model.py
+-rw-r--r--   0 puyuan     (501) 453037844     5754 2023-08-02 09:19:21.000000 LightZero-0.0.5/lzero/model/tests/test_muzero_model.py
+-rw-r--r--   0 puyuan     (501) 453037844     6897 2023-08-02 09:19:21.000000 LightZero-0.0.5/lzero/model/tests/test_sampled_efficientzero_model.py
+-rw-r--r--   0 puyuan     (501) 453037844     2241 2023-10-10 08:13:34.000000 LightZero-0.0.5/lzero/model/tests/test_stochastic_muzero_model.py
+-rw-r--r--   0 puyuan     (501) 453037844     2775 2023-08-22 03:29:23.000000 LightZero-0.0.5/lzero/model/utils.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:42.987970 LightZero-0.0.5/lzero/policy/
+-rw-r--r--   0 puyuan     (501) 453037844       54 2023-05-21 12:25:43.000000 LightZero-0.0.5/lzero/policy/__init__.py
+-rw-r--r--   0 puyuan     (501) 453037844    20395 2024-04-10 14:22:05.000000 LightZero-0.0.5/lzero/policy/alphazero.py
+-rw-r--r--   0 puyuan     (501) 453037844    42205 2024-03-30 09:59:19.000000 LightZero-0.0.5/lzero/policy/efficientzero.py
+-rw-r--r--   0 puyuan     (501) 453037844    22475 2024-04-10 14:22:05.000000 LightZero-0.0.5/lzero/policy/gumbel_alphazero.py
+-rw-r--r--   0 puyuan     (501) 453037844    41313 2024-03-13 12:25:48.000000 LightZero-0.0.5/lzero/policy/gumbel_muzero.py
+-rw-r--r--   0 puyuan     (501) 453037844    41450 2024-03-30 10:11:50.000000 LightZero-0.0.5/lzero/policy/muzero.py
+-rw-r--r--   0 puyuan     (501) 453037844    14651 2023-11-27 13:16:04.000000 LightZero-0.0.5/lzero/policy/random_policy.py
+-rw-r--r--   0 puyuan     (501) 453037844    28574 2024-03-13 12:25:48.000000 LightZero-0.0.5/lzero/policy/sampled_alphazero.py
+-rw-r--r--   0 puyuan     (501) 453037844    62661 2024-03-13 12:25:48.000000 LightZero-0.0.5/lzero/policy/sampled_efficientzero.py
+-rw-r--r--   0 puyuan     (501) 453037844     5375 2023-10-10 08:30:27.000000 LightZero-0.0.5/lzero/policy/scaling_transform.py
+-rw-r--r--   0 puyuan     (501) 453037844    43537 2024-03-13 12:25:48.000000 LightZero-0.0.5/lzero/policy/stochastic_muzero.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:42.989032 LightZero-0.0.5/lzero/policy/tests/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-04-14 09:11:22.000000 LightZero-0.0.5/lzero/policy/tests/__init__.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:42.989577 LightZero-0.0.5/lzero/policy/tests/config/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-10-10 08:13:34.000000 LightZero-0.0.5/lzero/policy/tests/config/__init__.py
+-rw-r--r--   0 puyuan     (501) 453037844     3347 2024-03-01 10:49:45.000000 LightZero-0.0.5/lzero/policy/tests/config/atari_muzero_config_for_test.py
+-rw-r--r--   0 puyuan     (501) 453037844     2591 2024-02-21 06:58:36.000000 LightZero-0.0.5/lzero/policy/tests/config/cartpole_muzero_config_for_test.py
+-rw-r--r--   0 puyuan     (501) 453037844     3057 2023-10-10 08:13:34.000000 LightZero-0.0.5/lzero/policy/tests/test_get_target_obs_index_in_step_k.py
+-rw-r--r--   0 puyuan     (501) 453037844      561 2023-05-24 10:01:46.000000 LightZero-0.0.5/lzero/policy/tests/test_scaling_transform.py
+-rw-r--r--   0 puyuan     (501) 453037844     7116 2023-11-27 13:16:04.000000 LightZero-0.0.5/lzero/policy/tests/test_utils.py
+-rw-r--r--   0 puyuan     (501) 453037844    27329 2024-03-30 09:59:19.000000 LightZero-0.0.5/lzero/policy/utils.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:42.991733 LightZero-0.0.5/lzero/worker/
+-rw-r--r--   0 puyuan     (501) 453037844      195 2023-11-27 13:16:04.000000 LightZero-0.0.5/lzero/worker/__init__.py
+-rw-r--r--   0 puyuan     (501) 453037844    17147 2024-04-10 08:10:55.000000 LightZero-0.0.5/lzero/worker/alphazero_collector.py
+-rw-r--r--   0 puyuan     (501) 453037844    13380 2024-02-21 06:58:36.000000 LightZero-0.0.5/lzero/worker/alphazero_evaluator.py
+-rw-r--r--   0 puyuan     (501) 453037844    38389 2024-03-30 10:17:56.000000 LightZero-0.0.5/lzero/worker/muzero_collector.py
+-rw-r--r--   0 puyuan     (501) 453037844    23209 2024-03-30 10:10:14.000000 LightZero-0.0.5/lzero/worker/muzero_evaluator.py
+-rw-r--r--   0 puyuan     (501) 453037844      870 2024-03-07 08:08:19.000000 LightZero-0.0.5/lzero/worker/tmp.py
+-rw-r--r--   0 puyuan     (501) 453037844     1329 2023-08-22 03:29:23.000000 LightZero-0.0.5/pyproject.toml
+-rw-r--r--   0 puyuan     (501) 453037844       38 2024-04-12 05:04:43.037858 LightZero-0.0.5/setup.cfg
+-rw-r--r--   0 puyuan     (501) 453037844     4010 2024-04-12 04:59:56.000000 LightZero-0.0.5/setup.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:42.991985 LightZero-0.0.5/zoo/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-04-14 09:11:22.000000 LightZero-0.0.5/zoo/__init__.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:42.992071 LightZero-0.0.5/zoo/atari/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-04-14 09:11:22.000000 LightZero-0.0.5/zoo/atari/__init__.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:42.994948 LightZero-0.0.5/zoo/atari/config/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-04-14 09:11:22.000000 LightZero-0.0.5/zoo/atari/config/__init__.py
+-rw-r--r--   0 puyuan     (501) 453037844     3565 2024-02-21 06:58:36.000000 LightZero-0.0.5/zoo/atari/config/atari_efficientzero_config.py
+-rw-r--r--   0 puyuan     (501) 453037844     3778 2024-03-07 08:58:23.000000 LightZero-0.0.5/zoo/atari/config/atari_efficientzero_config_tmp.py
+-rw-r--r--   0 puyuan     (501) 453037844     4795 2024-03-30 09:59:19.000000 LightZero-0.0.5/zoo/atari/config/atari_efficientzero_multigpu_ddp_config.py
+-rw-r--r--   0 puyuan     (501) 453037844     3333 2024-02-21 06:58:36.000000 LightZero-0.0.5/zoo/atari/config/atari_gumbel_muzero_config.py
+-rw-r--r--   0 puyuan     (501) 453037844     3667 2024-03-30 09:59:19.000000 LightZero-0.0.5/zoo/atari/config/atari_muzero_config.py
+-rw-r--r--   0 puyuan     (501) 453037844     3747 2024-03-06 09:31:38.000000 LightZero-0.0.5/zoo/atari/config/atari_muzero_config_tmp.py
+-rw-r--r--   0 puyuan     (501) 453037844     4265 2024-03-30 09:59:19.000000 LightZero-0.0.5/zoo/atari/config/atari_muzero_multigpu_ddp_config.py
+-rw-r--r--   0 puyuan     (501) 453037844     3438 2024-02-21 06:58:36.000000 LightZero-0.0.5/zoo/atari/config/atari_sampled_efficientzero_config.py
+-rw-r--r--   0 puyuan     (501) 453037844     3704 2024-02-21 06:58:36.000000 LightZero-0.0.5/zoo/atari/config/atari_stochastic_muzero_config.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:42.995294 LightZero-0.0.5/zoo/atari/entry/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-10-10 08:13:34.000000 LightZero-0.0.5/zoo/atari/entry/__init__.py
+-rw-r--r--   0 puyuan     (501) 453037844     4107 2023-12-26 05:44:59.000000 LightZero-0.0.5/zoo/atari/entry/atari_eval.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:42.996182 LightZero-0.0.5/zoo/atari/envs/
+-rw-r--r--   0 puyuan     (501) 453037844       46 2023-04-14 09:11:22.000000 LightZero-0.0.5/zoo/atari/envs/__init__.py
+-rw-r--r--   0 puyuan     (501) 453037844     9695 2024-03-30 09:59:19.000000 LightZero-0.0.5/zoo/atari/envs/atari_lightzero_env.py
+-rw-r--r--   0 puyuan     (501) 453037844    10831 2024-03-30 09:59:19.000000 LightZero-0.0.5/zoo/atari/envs/atari_wrappers.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:42.997290 LightZero-0.0.5/zoo/board_games/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-04-14 09:11:22.000000 LightZero-0.0.5/zoo/board_games/__init__.py
+-rw-r--r--   0 puyuan     (501) 453037844     9173 2024-03-30 09:59:19.000000 LightZero-0.0.5/zoo/board_games/alphabeta_pruning_bot.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:42.998977 LightZero-0.0.5/zoo/board_games/classic_search_algorithm/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-04-14 09:11:22.000000 LightZero-0.0.5/zoo/board_games/classic_search_algorithm/__init__.py
+-rw-r--r--   0 puyuan     (501) 453037844     1839 2023-04-14 09:11:22.000000 LightZero-0.0.5/zoo/board_games/classic_search_algorithm/alphabeta_pruning.py
+-rw-r--r--   0 puyuan     (501) 453037844     2304 2023-04-14 09:11:22.000000 LightZero-0.0.5/zoo/board_games/classic_search_algorithm/alphabeta_pruning_return_best_subtree.py
+-rw-r--r--   0 puyuan     (501) 453037844      759 2023-04-14 09:11:22.000000 LightZero-0.0.5/zoo/board_games/classic_search_algorithm/minimax_v0.py
+-rw-r--r--   0 puyuan     (501) 453037844     1426 2023-04-14 09:11:22.000000 LightZero-0.0.5/zoo/board_games/classic_search_algorithm/minimax_v1.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:42.999115 LightZero-0.0.5/zoo/board_games/go/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-04-14 09:11:22.000000 LightZero-0.0.5/zoo/board_games/go/__init__.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:42.999278 LightZero-0.0.5/zoo/board_games/go/config/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-05-24 10:01:46.000000 LightZero-0.0.5/zoo/board_games/go/config/__init__.py
+-rw-r--r--   0 puyuan     (501) 453037844        8 2023-08-22 03:29:23.000000 LightZero-0.0.5/zoo/board_games/go/config/go_alphazero_sp-mode_config.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:42.999959 LightZero-0.0.5/zoo/board_games/go/envs/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-08-22 03:29:23.000000 LightZero-0.0.5/zoo/board_games/go/envs/__init__.py
+-rw-r--r--   0 puyuan     (501) 453037844    12618 2023-12-05 15:14:38.000000 LightZero-0.0.5/zoo/board_games/go/envs/go_env.py
+-rw-r--r--   0 puyuan     (501) 453037844     1302 2023-08-22 03:29:23.000000 LightZero-0.0.5/zoo/board_games/go/envs/test_go_env.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:43.000178 LightZero-0.0.5/zoo/board_games/gomoku/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-04-14 09:11:22.000000 LightZero-0.0.5/zoo/board_games/gomoku/__init__.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:43.002889 LightZero-0.0.5/zoo/board_games/gomoku/config/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-05-24 10:01:46.000000 LightZero-0.0.5/zoo/board_games/gomoku/config/__init__.py
+-rw-r--r--   0 puyuan     (501) 453037844     4085 2024-04-10 14:22:05.000000 LightZero-0.0.5/zoo/board_games/gomoku/config/gomoku_alphazero_bot_mode_config.py
+-rw-r--r--   0 puyuan     (501) 453037844     4086 2024-02-21 06:58:36.000000 LightZero-0.0.5/zoo/board_games/gomoku/config/gomoku_alphazero_sp_mode_config.py
+-rw-r--r--   0 puyuan     (501) 453037844     4272 2024-04-10 14:22:05.000000 LightZero-0.0.5/zoo/board_games/gomoku/config/gomoku_gumbel_alphazero_bot_mode_config.py
+-rw-r--r--   0 puyuan     (501) 453037844     3409 2024-01-29 10:01:00.000000 LightZero-0.0.5/zoo/board_games/gomoku/config/gomoku_gumbel_muzero_bot_mode_config.py
+-rw-r--r--   0 puyuan     (501) 453037844     3293 2024-01-29 10:01:00.000000 LightZero-0.0.5/zoo/board_games/gomoku/config/gomoku_muzero_bot_mode_config.py
+-rw-r--r--   0 puyuan     (501) 453037844     3348 2024-01-29 10:01:00.000000 LightZero-0.0.5/zoo/board_games/gomoku/config/gomoku_muzero_sp_mode_config.py
+-rw-r--r--   0 puyuan     (501) 453037844     4515 2024-02-21 06:58:36.000000 LightZero-0.0.5/zoo/board_games/gomoku/config/gomoku_sampled_alphazero_bot_mode_config.py
+-rw-r--r--   0 puyuan     (501) 453037844     4503 2024-02-21 06:58:36.000000 LightZero-0.0.5/zoo/board_games/gomoku/config/gomoku_sampled_alphazero_sp_mode_config.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:43.003962 LightZero-0.0.5/zoo/board_games/gomoku/entry/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-10-10 08:13:34.000000 LightZero-0.0.5/zoo/board_games/gomoku/entry/__init__.py
+-rw-r--r--   0 puyuan     (501) 453037844     2892 2023-12-02 15:39:07.000000 LightZero-0.0.5/zoo/board_games/gomoku/entry/gomoku_alphazero_eval.py
+-rw-r--r--   0 puyuan     (501) 453037844     2047 2023-10-10 08:13:34.000000 LightZero-0.0.5/zoo/board_games/gomoku/entry/gomoku_gumbel_muzero_eval.py
+-rw-r--r--   0 puyuan     (501) 453037844     1911 2023-12-04 10:36:50.000000 LightZero-0.0.5/zoo/board_games/gomoku/entry/gomoku_muzero_eval.py
+-rw-r--r--   0 puyuan     (501) 453037844     2095 2023-12-02 15:34:44.000000 LightZero-0.0.5/zoo/board_games/gomoku/entry/gomoku_sampled_alphazero_eval.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:43.008846 LightZero-0.0.5/zoo/board_games/gomoku/envs/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-08-22 03:29:23.000000 LightZero-0.0.5/zoo/board_games/gomoku/envs/__init__.py
+-rw-r--r--   0 puyuan     (501) 453037844    36356 2024-02-21 06:58:36.000000 LightZero-0.0.5/zoo/board_games/gomoku/envs/gomoku_env.py
+-rw-r--r--   0 puyuan     (501) 453037844     8458 2023-12-02 15:34:44.000000 LightZero-0.0.5/zoo/board_games/gomoku/envs/gomoku_human_vs_bot_UI.py
+-rw-r--r--   0 puyuan     (501) 453037844    16828 2023-12-02 15:34:44.000000 LightZero-0.0.5/zoo/board_games/gomoku/envs/gomoku_rule_bot_v0.py
+-rw-r--r--   0 puyuan     (501) 453037844    15588 2024-01-29 10:01:00.000000 LightZero-0.0.5/zoo/board_games/gomoku/envs/gomoku_rule_bot_v1.py
+-rw-r--r--   0 puyuan     (501) 453037844     4747 2023-11-13 12:15:56.000000 LightZero-0.0.5/zoo/board_games/gomoku/envs/test_gomoku_alphabeta_pruning_bot.py
+-rw-r--r--   0 puyuan     (501) 453037844     3440 2024-01-29 10:01:00.000000 LightZero-0.0.5/zoo/board_games/gomoku/envs/test_gomoku_env.py
+-rw-r--r--   0 puyuan     (501) 453037844     6488 2024-03-30 09:59:19.000000 LightZero-0.0.5/zoo/board_games/gomoku/envs/test_gomoku_mcts_bot.py
+-rw-r--r--   0 puyuan     (501) 453037844     4725 2023-12-02 15:34:44.000000 LightZero-0.0.5/zoo/board_games/gomoku/envs/test_gomoku_rule_bot_v0.py
+-rw-r--r--   0 puyuan     (501) 453037844     1898 2024-01-29 10:01:00.000000 LightZero-0.0.5/zoo/board_games/gomoku/envs/test_gomoku_rule_bot_v1.py
+-rw-r--r--   0 puyuan     (501) 453037844     1260 2023-08-22 03:29:23.000000 LightZero-0.0.5/zoo/board_games/gomoku/envs/utils.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:43.009992 LightZero-0.0.5/zoo/board_games/gomoku/test/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-08-02 09:19:22.000000 LightZero-0.0.5/zoo/board_games/gomoku/test/__init__.py
+-rw-r--r--   0 puyuan     (501) 453037844     4968 2023-08-02 09:19:22.000000 LightZero-0.0.5/zoo/board_games/gomoku/test/eval_get_done_winner.py
+-rw-r--r--   0 puyuan     (501) 453037844     5110 2023-08-02 09:19:22.000000 LightZero-0.0.5/zoo/board_games/gomoku/test/eval_legal_actions.py
+-rw-r--r--   0 puyuan     (501) 453037844     2663 2023-08-02 09:19:22.000000 LightZero-0.0.5/zoo/board_games/gomoku/test/test_get_done_winner_cython.py
+-rw-r--r--   0 puyuan     (501) 453037844     2755 2024-02-21 06:58:36.000000 LightZero-0.0.5/zoo/board_games/gomoku/test/test_gomoku_env_legal_actions.py
+-rw-r--r--   0 puyuan     (501) 453037844     1797 2023-08-02 09:19:22.000000 LightZero-0.0.5/zoo/board_games/gomoku/test/test_legal_actions_cython.py
+-rw-r--r--   0 puyuan     (501) 453037844    18368 2023-11-27 13:16:04.000000 LightZero-0.0.5/zoo/board_games/mcts_bot.py
+-rw-r--r--   0 puyuan     (501) 453037844    21650 2024-03-30 09:59:19.000000 LightZero-0.0.5/zoo/board_games/test_speed_win-rate_between_bots.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:43.010144 LightZero-0.0.5/zoo/board_games/tictactoe/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-04-14 09:11:22.000000 LightZero-0.0.5/zoo/board_games/tictactoe/__init__.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:43.012982 LightZero-0.0.5/zoo/board_games/tictactoe/config/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-08-22 03:29:23.000000 LightZero-0.0.5/zoo/board_games/tictactoe/config/__init__.py
+-rw-r--r--   0 puyuan     (501) 453037844     3572 2024-02-21 06:58:36.000000 LightZero-0.0.5/zoo/board_games/tictactoe/config/tictactoe_alphazero_bot_mode_config.py
+-rw-r--r--   0 puyuan     (501) 453037844     3964 2024-02-21 06:58:36.000000 LightZero-0.0.5/zoo/board_games/tictactoe/config/tictactoe_alphazero_bot_mode_multigpu_ddp_config.py
+-rw-r--r--   0 puyuan     (501) 453037844     3515 2024-02-21 06:58:36.000000 LightZero-0.0.5/zoo/board_games/tictactoe/config/tictactoe_alphazero_sp_mode_config.py
+-rw-r--r--   0 puyuan     (501) 453037844     3945 2024-02-21 06:58:36.000000 LightZero-0.0.5/zoo/board_games/tictactoe/config/tictactoe_alphazero_sp_mode_multigpu_ddp_config.py
+-rw-r--r--   0 puyuan     (501) 453037844     3194 2024-04-10 04:54:19.000000 LightZero-0.0.5/zoo/board_games/tictactoe/config/tictactoe_efficientzero_bot_mode_config.py
+-rw-r--r--   0 puyuan     (501) 453037844     3162 2024-04-10 04:54:19.000000 LightZero-0.0.5/zoo/board_games/tictactoe/config/tictactoe_efficientzero_sp_mode_config.py
+-rw-r--r--   0 puyuan     (501) 453037844     3095 2023-12-07 08:13:35.000000 LightZero-0.0.5/zoo/board_games/tictactoe/config/tictactoe_gumbel_muzero_bot_mode_config.py
+-rw-r--r--   0 puyuan     (501) 453037844     3008 2024-03-12 04:08:23.000000 LightZero-0.0.5/zoo/board_games/tictactoe/config/tictactoe_muzero_bot_mode_config.py
+-rw-r--r--   0 puyuan     (501) 453037844     2975 2023-12-07 08:13:35.000000 LightZero-0.0.5/zoo/board_games/tictactoe/config/tictactoe_muzero_sp_mode_config.py
+-rw-r--r--   0 puyuan     (501) 453037844     3818 2024-02-21 06:58:36.000000 LightZero-0.0.5/zoo/board_games/tictactoe/config/tictactoe_sampled_alphazero_bot_mode_config.py
+-rw-r--r--   0 puyuan     (501) 453037844     3761 2024-02-21 06:58:36.000000 LightZero-0.0.5/zoo/board_games/tictactoe/config/tictactoe_sampled_alphazero_sp_mode_config.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:43.013335 LightZero-0.0.5/zoo/board_games/tictactoe/entry/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-10-10 08:13:34.000000 LightZero-0.0.5/zoo/board_games/tictactoe/entry/__init__.py
+-rw-r--r--   0 puyuan     (501) 453037844     2806 2024-02-21 06:58:36.000000 LightZero-0.0.5/zoo/board_games/tictactoe/entry/tictactoe_alphazero_eval.py
+-rw-r--r--   0 puyuan     (501) 453037844     2753 2024-02-21 06:58:36.000000 LightZero-0.0.5/zoo/board_games/tictactoe/entry/tictactoe_muzero_eval.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:43.014538 LightZero-0.0.5/zoo/board_games/tictactoe/envs/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-04-14 09:11:22.000000 LightZero-0.0.5/zoo/board_games/tictactoe/envs/__init__.py
+-rw-r--r--   0 puyuan     (501) 453037844     4105 2023-05-24 10:01:46.000000 LightZero-0.0.5/zoo/board_games/tictactoe/envs/test_tictactoe_alphabeta_prunning_bot.py
+-rw-r--r--   0 puyuan     (501) 453037844     3327 2024-03-13 12:25:48.000000 LightZero-0.0.5/zoo/board_games/tictactoe/envs/test_tictactoe_env.py
+-rw-r--r--   0 puyuan     (501) 453037844     6229 2023-04-14 09:11:22.000000 LightZero-0.0.5/zoo/board_games/tictactoe/envs/test_tictactoe_mcts_bot.py
+-rw-r--r--   0 puyuan     (501) 453037844     1204 2024-03-30 09:59:19.000000 LightZero-0.0.5/zoo/board_games/tictactoe/envs/test_tictactoe_rule_bot_v0.py
+-rw-r--r--   0 puyuan     (501) 453037844    32758 2024-03-13 12:25:48.000000 LightZero-0.0.5/zoo/board_games/tictactoe/envs/tictactoe_env.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:43.014945 LightZero-0.0.5/zoo/box2d/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-04-14 09:11:22.000000 LightZero-0.0.5/zoo/box2d/__init__.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:43.015037 LightZero-0.0.5/zoo/box2d/bipedalwalker/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-05-24 10:01:46.000000 LightZero-0.0.5/zoo/box2d/bipedalwalker/__init__.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:43.015946 LightZero-0.0.5/zoo/box2d/bipedalwalker/config/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-05-24 10:01:46.000000 LightZero-0.0.5/zoo/box2d/bipedalwalker/config/__init__.py
+-rw-r--r--   0 puyuan     (501) 453037844     4201 2024-02-21 06:58:36.000000 LightZero-0.0.5/zoo/box2d/bipedalwalker/config/bipedalwalker_cont_disc_efficientzero_config.py
+-rw-r--r--   0 puyuan     (501) 453037844     4311 2024-02-21 06:58:36.000000 LightZero-0.0.5/zoo/box2d/bipedalwalker/config/bipedalwalker_cont_disc_sampled_efficientzero_config.py
+-rw-r--r--   0 puyuan     (501) 453037844     4260 2024-02-21 06:58:36.000000 LightZero-0.0.5/zoo/box2d/bipedalwalker/config/bipedalwalker_cont_sampled_efficientzero_config.py
+-rw-r--r--   0 puyuan     (501) 453037844     4768 2023-08-21 13:43:50.000000 LightZero-0.0.5/zoo/box2d/bipedalwalker/config/tmp.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:43.016267 LightZero-0.0.5/zoo/box2d/bipedalwalker/entry/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-10-10 08:13:34.000000 LightZero-0.0.5/zoo/box2d/bipedalwalker/entry/__init__.py
+-rw-r--r--   0 puyuan     (501) 453037844     4019 2023-12-05 15:14:38.000000 LightZero-0.0.5/zoo/box2d/bipedalwalker/entry/bipedalwalker_eval.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:43.016771 LightZero-0.0.5/zoo/box2d/bipedalwalker/envs/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-05-24 10:01:46.000000 LightZero-0.0.5/zoo/box2d/bipedalwalker/envs/__init__.py
+-rw-r--r--   0 puyuan     (501) 453037844     7794 2024-02-21 06:58:36.000000 LightZero-0.0.5/zoo/box2d/bipedalwalker/envs/bipedalwalker_cont_disc_env.py
+-rw-r--r--   0 puyuan     (501) 453037844     8932 2024-02-21 06:58:36.000000 LightZero-0.0.5/zoo/box2d/bipedalwalker/envs/bipedalwalker_env.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:43.017186 LightZero-0.0.5/zoo/box2d/lunarlander/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-04-14 09:11:22.000000 LightZero-0.0.5/zoo/box2d/lunarlander/__init__.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:43.018336 LightZero-0.0.5/zoo/box2d/lunarlander/config/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-04-14 09:11:22.000000 LightZero-0.0.5/zoo/box2d/lunarlander/config/__init__.py
+-rw-r--r--   0 puyuan     (501) 453037844     3994 2024-02-21 06:58:36.000000 LightZero-0.0.5/zoo/box2d/lunarlander/config/lunarlander_cont_disc_efficientzero_config.py
+-rw-r--r--   0 puyuan     (501) 453037844     4008 2024-02-21 06:58:36.000000 LightZero-0.0.5/zoo/box2d/lunarlander/config/lunarlander_cont_disc_sampled_efficientzero_config.py
+-rw-r--r--   0 puyuan     (501) 453037844     4050 2024-02-21 06:58:36.000000 LightZero-0.0.5/zoo/box2d/lunarlander/config/lunarlander_cont_sampled_efficientzero_config.py
+-rw-r--r--   0 puyuan     (501) 453037844     3433 2024-02-21 06:58:36.000000 LightZero-0.0.5/zoo/box2d/lunarlander/config/lunarlander_disc_efficientzero_config.py
+-rw-r--r--   0 puyuan     (501) 453037844     3829 2024-02-21 06:58:36.000000 LightZero-0.0.5/zoo/box2d/lunarlander/config/lunarlander_disc_gumbel_muzero_config.py
+-rw-r--r--   0 puyuan     (501) 453037844     3660 2024-02-21 06:58:36.000000 LightZero-0.0.5/zoo/box2d/lunarlander/config/lunarlander_disc_muzero_config.py
+-rw-r--r--   0 puyuan     (501) 453037844     3763 2024-02-21 06:58:36.000000 LightZero-0.0.5/zoo/box2d/lunarlander/config/lunarlander_disc_stochastic_muzero_config.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:43.018547 LightZero-0.0.5/zoo/box2d/lunarlander/entry/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-10-10 08:13:34.000000 LightZero-0.0.5/zoo/box2d/lunarlander/entry/__init__.py
+-rw-r--r--   0 puyuan     (501) 453037844     3985 2023-12-02 15:39:07.000000 LightZero-0.0.5/zoo/box2d/lunarlander/entry/lunarlander_eval.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:43.019656 LightZero-0.0.5/zoo/box2d/lunarlander/envs/
+-rwxr-xr-x   0 puyuan     (501) 453037844       44 2023-04-14 09:11:22.000000 LightZero-0.0.5/zoo/box2d/lunarlander/envs/__init__.py
+-rwxr-xr-x   0 puyuan     (501) 453037844     8084 2024-02-21 06:58:36.000000 LightZero-0.0.5/zoo/box2d/lunarlander/envs/lunarlander_cont_disc_env.py
+-rwxr-xr-x   0 puyuan     (501) 453037844     9138 2024-02-21 06:58:36.000000 LightZero-0.0.5/zoo/box2d/lunarlander/envs/lunarlander_env.py
+-rwxr-xr-x   0 puyuan     (501) 453037844     1643 2024-02-21 06:58:36.000000 LightZero-0.0.5/zoo/box2d/lunarlander/envs/test_lunarlander_env.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:43.019801 LightZero-0.0.5/zoo/classic_control/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-04-14 09:11:22.000000 LightZero-0.0.5/zoo/classic_control/__init__.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:43.019887 LightZero-0.0.5/zoo/classic_control/cartpole/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-08-02 09:19:22.000000 LightZero-0.0.5/zoo/classic_control/cartpole/__init__.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:43.021247 LightZero-0.0.5/zoo/classic_control/cartpole/config/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-05-24 10:01:46.000000 LightZero-0.0.5/zoo/classic_control/cartpole/config/__init__.py
+-rw-r--r--   0 puyuan     (501) 453037844     3304 2024-02-21 06:58:36.000000 LightZero-0.0.5/zoo/classic_control/cartpole/config/cartpole_efficientzero_config.py
+-rw-r--r--   0 puyuan     (501) 453037844     3460 2024-02-21 06:58:36.000000 LightZero-0.0.5/zoo/classic_control/cartpole/config/cartpole_gumbel_muzero_config.py
+-rw-r--r--   0 puyuan     (501) 453037844     3388 2024-03-30 09:59:19.000000 LightZero-0.0.5/zoo/classic_control/cartpole/config/cartpole_muzero_config.py
+-rw-r--r--   0 puyuan     (501) 453037844     3695 2024-02-23 09:31:32.000000 LightZero-0.0.5/zoo/classic_control/cartpole/config/cartpole_muzero_config_ckpt_tmp.py
+-rw-r--r--   0 puyuan     (501) 453037844     3556 2024-02-21 06:58:36.000000 LightZero-0.0.5/zoo/classic_control/cartpole/config/cartpole_sampled_efficientzero_config.py
+-rw-r--r--   0 puyuan     (501) 453037844     2863 2024-02-21 06:58:36.000000 LightZero-0.0.5/zoo/classic_control/cartpole/config/cartpole_stochastic_muzero_config.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:43.021512 LightZero-0.0.5/zoo/classic_control/cartpole/entry/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-10-10 08:13:34.000000 LightZero-0.0.5/zoo/classic_control/cartpole/entry/__init__.py
+-rw-r--r--   0 puyuan     (501) 453037844     2623 2023-12-02 15:39:07.000000 LightZero-0.0.5/zoo/classic_control/cartpole/entry/cartpole_eval.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:43.021854 LightZero-0.0.5/zoo/classic_control/cartpole/envs/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-05-24 10:01:46.000000 LightZero-0.0.5/zoo/classic_control/cartpole/envs/__init__.py
+-rw-r--r--   0 puyuan     (501) 453037844     7553 2024-03-30 09:59:19.000000 LightZero-0.0.5/zoo/classic_control/cartpole/envs/cartpole_lightzero_env.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:43.022229 LightZero-0.0.5/zoo/classic_control/mountain_car/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2024-03-30 09:59:19.000000 LightZero-0.0.5/zoo/classic_control/mountain_car/__init__.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:43.022460 LightZero-0.0.5/zoo/classic_control/mountain_car/entry/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2024-03-30 09:59:19.000000 LightZero-0.0.5/zoo/classic_control/mountain_car/entry/__init__.py
+-rw-r--r--   0 puyuan     (501) 453037844     2740 2024-03-30 09:59:19.000000 LightZero-0.0.5/zoo/classic_control/mountain_car/entry/mountain_car_eval.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:43.023891 LightZero-0.0.5/zoo/classic_control/mountain_car/envs/
+-rw-r--r--   0 puyuan     (501) 453037844       49 2024-03-30 09:59:19.000000 LightZero-0.0.5/zoo/classic_control/mountain_car/envs/__init__.py
+-rw-r--r--   0 puyuan     (501) 453037844     4952 2024-03-30 09:59:19.000000 LightZero-0.0.5/zoo/classic_control/mountain_car/envs/mtcar_lightzero_env.py
+-rw-r--r--   0 puyuan     (501) 453037844     1409 2024-03-30 09:59:19.000000 LightZero-0.0.5/zoo/classic_control/mountain_car/envs/test_mtcar_env.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:43.024136 LightZero-0.0.5/zoo/classic_control/pendulum/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-04-14 09:11:22.000000 LightZero-0.0.5/zoo/classic_control/pendulum/__init__.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:43.025447 LightZero-0.0.5/zoo/classic_control/pendulum/config/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-04-14 09:11:22.000000 LightZero-0.0.5/zoo/classic_control/pendulum/config/__init__.py
+-rw-r--r--   0 puyuan     (501) 453037844     3297 2024-02-21 06:58:36.000000 LightZero-0.0.5/zoo/classic_control/pendulum/config/pendulum_cont_disc_efficientzero_config.py
+-rw-r--r--   0 puyuan     (501) 453037844     3642 2024-02-21 06:58:36.000000 LightZero-0.0.5/zoo/classic_control/pendulum/config/pendulum_cont_disc_gumbel_muzero_config.py
+-rw-r--r--   0 puyuan     (501) 453037844     3526 2024-02-21 06:58:36.000000 LightZero-0.0.5/zoo/classic_control/pendulum/config/pendulum_cont_disc_muzero_config.py
+-rw-r--r--   0 puyuan     (501) 453037844     3514 2024-02-21 06:58:36.000000 LightZero-0.0.5/zoo/classic_control/pendulum/config/pendulum_cont_disc_sampled_efficientzero_config.py
+-rw-r--r--   0 puyuan     (501) 453037844     3647 2024-02-21 06:58:36.000000 LightZero-0.0.5/zoo/classic_control/pendulum/config/pendulum_cont_disc_stochastic_muzero_config.py
+-rw-r--r--   0 puyuan     (501) 453037844     3821 2024-02-21 06:58:36.000000 LightZero-0.0.5/zoo/classic_control/pendulum/config/pendulum_cont_sampled_efficientzero_config.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:43.025680 LightZero-0.0.5/zoo/classic_control/pendulum/entry/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-10-10 08:13:34.000000 LightZero-0.0.5/zoo/classic_control/pendulum/entry/__init__.py
+-rw-r--r--   0 puyuan     (501) 453037844     2723 2023-12-26 05:44:59.000000 LightZero-0.0.5/zoo/classic_control/pendulum/entry/pendulum_eval.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:43.026145 LightZero-0.0.5/zoo/classic_control/pendulum/envs/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-04-14 09:11:22.000000 LightZero-0.0.5/zoo/classic_control/pendulum/envs/__init__.py
+-rw-r--r--   0 puyuan     (501) 453037844     7509 2023-12-26 05:44:59.000000 LightZero-0.0.5/zoo/classic_control/pendulum/envs/pendulum_lightzero_env.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:43.026572 LightZero-0.0.5/zoo/game_2048/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-10-10 08:13:34.000000 LightZero-0.0.5/zoo/game_2048/__init__.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:43.027121 LightZero-0.0.5/zoo/game_2048/entry/
+-rw-r--r--   0 puyuan     (501) 453037844     1962 2024-03-30 09:59:19.000000 LightZero-0.0.5/zoo/game_2048/entry/2048_bot_eval.py
+-rw-r--r--   0 puyuan     (501) 453037844     2977 2023-12-02 15:39:07.000000 LightZero-0.0.5/zoo/game_2048/entry/2048_eval.py
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-10-10 08:13:34.000000 LightZero-0.0.5/zoo/game_2048/entry/__init__.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:43.028502 LightZero-0.0.5/zoo/game_2048/envs/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-10-10 08:13:34.000000 LightZero-0.0.5/zoo/game_2048/envs/__init__.py
+-rw-r--r--   0 puyuan     (501) 453037844     5468 2023-10-10 08:13:34.000000 LightZero-0.0.5/zoo/game_2048/envs/expectimax_search_based_bot.py
+-rw-r--r--   0 puyuan     (501) 453037844    37378 2024-03-30 09:59:19.000000 LightZero-0.0.5/zoo/game_2048/envs/game_2048_env.py
+-rw-r--r--   0 puyuan     (501) 453037844     7275 2024-03-30 09:59:19.000000 LightZero-0.0.5/zoo/game_2048/envs/test_game_2048_env.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:43.028790 LightZero-0.0.5/zoo/memory/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2024-03-19 16:45:24.000000 LightZero-0.0.5/zoo/memory/__init__.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:43.029729 LightZero-0.0.5/zoo/memory/config/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2024-03-19 16:45:24.000000 LightZero-0.0.5/zoo/memory/config/__init__.py
+-rw-r--r--   0 puyuan     (501) 453037844     3620 2024-03-30 09:59:19.000000 LightZero-0.0.5/zoo/memory/config/memory_efficientzero_config.py
+-rw-r--r--   0 puyuan     (501) 453037844     3955 2024-03-30 09:59:19.000000 LightZero-0.0.5/zoo/memory/config/memory_muzero_config.py
+-rw-r--r--   0 puyuan     (501) 453037844     5529 2024-03-30 09:59:19.000000 LightZero-0.0.5/zoo/memory/config/memory_muzero_rnd_config.py
+-rw-r--r--   0 puyuan     (501) 453037844     4457 2024-03-30 09:59:19.000000 LightZero-0.0.5/zoo/memory/config/memory_sampled_efficientzero_config.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:43.030088 LightZero-0.0.5/zoo/memory/entry/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2024-03-19 16:45:24.000000 LightZero-0.0.5/zoo/memory/entry/__init__.py
+-rw-r--r--   0 puyuan     (501) 453037844     3879 2024-03-30 09:59:19.000000 LightZero-0.0.5/zoo/memory/entry/memory_eval.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:43.031073 LightZero-0.0.5/zoo/memory/envs/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2024-03-19 16:45:24.000000 LightZero-0.0.5/zoo/memory/envs/__init__.py
+-rw-r--r--   0 puyuan     (501) 453037844    12286 2024-03-30 09:59:19.000000 LightZero-0.0.5/zoo/memory/envs/memory_lightzero_env.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:43.033043 LightZero-0.0.5/zoo/memory/envs/pycolab_tvt/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2024-03-19 16:45:24.000000 LightZero-0.0.5/zoo/memory/envs/pycolab_tvt/__init__.py
+-rw-r--r--   0 puyuan     (501) 453037844    10798 2024-04-12 04:33:30.000000 LightZero-0.0.5/zoo/memory/envs/pycolab_tvt/common.py
+-rw-r--r--   0 puyuan     (501) 453037844     1326 2024-03-19 16:45:24.000000 LightZero-0.0.5/zoo/memory/envs/pycolab_tvt/game.py
+-rw-r--r--   0 puyuan     (501) 453037844     2019 2024-04-12 04:33:30.000000 LightZero-0.0.5/zoo/memory/envs/pycolab_tvt/human_player.py
+-rw-r--r--   0 puyuan     (501) 453037844     8057 2024-03-30 09:59:19.000000 LightZero-0.0.5/zoo/memory/envs/pycolab_tvt/key_to_door.py
+-rw-r--r--   0 puyuan     (501) 453037844     4488 2024-03-19 16:45:24.000000 LightZero-0.0.5/zoo/memory/envs/pycolab_tvt/objects.py
+-rw-r--r--   0 puyuan     (501) 453037844     6340 2024-04-12 04:33:30.000000 LightZero-0.0.5/zoo/memory/envs/pycolab_tvt/visual_match.py
+-rw-r--r--   0 puyuan     (501) 453037844     5152 2024-04-12 04:33:30.000000 LightZero-0.0.5/zoo/memory/envs/test_memory_lightzero_env.py
+-rw-r--r--   0 puyuan     (501) 453037844     3421 2024-03-30 09:59:19.000000 LightZero-0.0.5/zoo/memory/envs/test_render.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:43.033352 LightZero-0.0.5/zoo/minigrid/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-11-27 13:16:04.000000 LightZero-0.0.5/zoo/minigrid/__init__.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:43.034368 LightZero-0.0.5/zoo/minigrid/config/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-11-27 13:16:04.000000 LightZero-0.0.5/zoo/minigrid/config/__init__.py
+-rw-r--r--   0 puyuan     (501) 453037844     4456 2024-02-21 06:58:36.000000 LightZero-0.0.5/zoo/minigrid/config/minigrd_sampled_efficientzero_config.py
+-rw-r--r--   0 puyuan     (501) 453037844     3597 2024-02-21 06:58:36.000000 LightZero-0.0.5/zoo/minigrid/config/minigrid_efficientzero_config.py
+-rw-r--r--   0 puyuan     (501) 453037844     3817 2024-02-21 06:58:36.000000 LightZero-0.0.5/zoo/minigrid/config/minigrid_muzero_config.py
+-rw-r--r--   0 puyuan     (501) 453037844     5502 2024-02-21 06:58:36.000000 LightZero-0.0.5/zoo/minigrid/config/minigrid_muzero_rnd_config.py
+drwxr-xr-x   0 puyuan     (501) 453037844        0 2024-04-12 05:04:43.034876 LightZero-0.0.5/zoo/minigrid/entry/
+-rw-r--r--   0 puyuan     (501) 453037844        0 2023-11-27 13:16:04.000000 LightZero-0.0.5/zoo/minigrid/entry/__init__.py
+-rw-r--r--   0 puyuan     (501) 453037844     3883 2023-12-05 15:14:38.000000 LightZero-0.0.5/zoo/minigrid/entry/minigrid_eval.py
```

### Comparing `LightZero-0.0.2/LICENSE` & `LightZero-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/LightZero.egg-info/SOURCES.txt` & `LightZero-0.0.5/LightZero.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,55 @@
 /Users/puyuan/code/LightZero/zoo/board_games/tictactoe/envs/legal_actions_cython.cpp
 LightZero.egg-info/PKG-INFO
 LightZero.egg-info/SOURCES.txt
 LightZero.egg-info/dependency_links.txt
 LightZero.egg-info/requires.txt
 LightZero.egg-info/top_level.txt
 lzero/__init__.py
+lzero/agent/__init__.py
+lzero/agent/alphazero.py
+lzero/agent/efficientzero.py
+lzero/agent/gumbel_muzero.py
+lzero/agent/muzero.py
+lzero/agent/sampled_alphazero.py
+lzero/agent/sampled_efficientzero.py
+lzero/agent/config/__init__.py
+lzero/agent/config/alphazero/__init__.py
+lzero/agent/config/alphazero/gomoku_play_with_bot.py
+lzero/agent/config/alphazero/tictactoe_play_with_bot.py
+lzero/agent/config/efficientzero/__init__.py
+lzero/agent/config/efficientzero/gym_breakoutnoframeskip_v4.py
+lzero/agent/config/efficientzero/gym_cartpole_v0.py
+lzero/agent/config/efficientzero/gym_lunarlander_v2.py
+lzero/agent/config/efficientzero/gym_mspacmannoframeskip_v4.py
+lzero/agent/config/efficientzero/gym_pendulum_v1.py
+lzero/agent/config/efficientzero/gym_pongnoframeskip_v4.py
+lzero/agent/config/gumbel_muzero/__init__.py
+lzero/agent/config/gumbel_muzero/gomoku_play_with_bot.py
+lzero/agent/config/gumbel_muzero/gym_cartpole_v0.py
+lzero/agent/config/gumbel_muzero/tictactoe_play_with_bot.py
+lzero/agent/config/muzero/__init__.py
+lzero/agent/config/muzero/gomoku_play_with_bot.py
+lzero/agent/config/muzero/gym_breakoutnoframeskip_v4.py
+lzero/agent/config/muzero/gym_cartpole_v0.py
+lzero/agent/config/muzero/gym_lunarlander_v2.py
+lzero/agent/config/muzero/gym_mspacmannoframeskip_v4.py
+lzero/agent/config/muzero/gym_pendulum_v1.py
+lzero/agent/config/muzero/gym_pongnoframeskip_v4.py
+lzero/agent/config/muzero/tictactoe_play_with_bot.py
+lzero/agent/config/sampled_alphazero/__init__.py
+lzero/agent/config/sampled_alphazero/gomoku_play_with_bot.py
+lzero/agent/config/sampled_alphazero/tictactoe_play_with_bot.py
+lzero/agent/config/sampled_efficientzero/__init__.py
+lzero/agent/config/sampled_efficientzero/gym_breakoutnoframeskip_v4.py
+lzero/agent/config/sampled_efficientzero/gym_cartpole_v0.py
+lzero/agent/config/sampled_efficientzero/gym_lunarlandercontinuous_v2.py
+lzero/agent/config/sampled_efficientzero/gym_mspacmannoframeskip_v4.py
+lzero/agent/config/sampled_efficientzero/gym_pendulum_v1.py
+lzero/agent/config/sampled_efficientzero/gym_pongnoframeskip_v4.py
 lzero/config/__init__.py
 lzero/config/meta.py
 lzero/config/utils.py
 lzero/entry/__init__.py
 lzero/entry/eval_alphazero.py
 lzero/entry/eval_muzero.py
 lzero/entry/eval_muzero_with_gym_env.py
@@ -80,14 +121,17 @@
 lzero/mcts/tests/eval_tree_speed.py
 lzero/mcts/tests/test_game_buffer.py
 lzero/mcts/tests/test_game_segment.py
 lzero/mcts/tests/test_image_transform.py
 lzero/mcts/tests/test_mcts_ctree.py
 lzero/mcts/tests/test_mcts_ptree.py
 lzero/mcts/tests/test_mcts_sampled_ctree.py
+lzero/mcts/tests/test_muzero_game_buffer.py
+lzero/mcts/tests/test_muzero_game_buffer_local_tmp.py
+lzero/mcts/tests/test_muzero_game_buffer_script_tmp.py
 lzero/mcts/tests/test_utils.py
 lzero/mcts/tests/config/__init__.py
 lzero/mcts/tests/config/atari_efficientzero_config_for_test.py
 lzero/mcts/tests/config/tictactoe_muzero_bot_mode_config_for_test.py
 lzero/mcts/tree_search/__init__.py
 lzero/mcts/tree_search/mcts_ctree.py
 lzero/mcts/tree_search/mcts_ctree_sampled.py
@@ -114,14 +158,15 @@
 lzero/model/tests/test_efficientzero_model.py
 lzero/model/tests/test_muzero_model.py
 lzero/model/tests/test_sampled_efficientzero_model.py
 lzero/model/tests/test_stochastic_muzero_model.py
 lzero/policy/__init__.py
 lzero/policy/alphazero.py
 lzero/policy/efficientzero.py
+lzero/policy/gumbel_alphazero.py
 lzero/policy/gumbel_muzero.py
 lzero/policy/muzero.py
 lzero/policy/random_policy.py
 lzero/policy/sampled_alphazero.py
 lzero/policy/sampled_efficientzero.py
 lzero/policy/scaling_transform.py
 lzero/policy/stochastic_muzero.py
@@ -134,21 +179,24 @@
 lzero/policy/tests/config/atari_muzero_config_for_test.py
 lzero/policy/tests/config/cartpole_muzero_config_for_test.py
 lzero/worker/__init__.py
 lzero/worker/alphazero_collector.py
 lzero/worker/alphazero_evaluator.py
 lzero/worker/muzero_collector.py
 lzero/worker/muzero_evaluator.py
+lzero/worker/tmp.py
 zoo/__init__.py
 zoo/atari/__init__.py
 zoo/atari/config/__init__.py
 zoo/atari/config/atari_efficientzero_config.py
+zoo/atari/config/atari_efficientzero_config_tmp.py
 zoo/atari/config/atari_efficientzero_multigpu_ddp_config.py
 zoo/atari/config/atari_gumbel_muzero_config.py
 zoo/atari/config/atari_muzero_config.py
+zoo/atari/config/atari_muzero_config_tmp.py
 zoo/atari/config/atari_muzero_multigpu_ddp_config.py
 zoo/atari/config/atari_sampled_efficientzero_config.py
 zoo/atari/config/atari_stochastic_muzero_config.py
 zoo/atari/entry/__init__.py
 zoo/atari/entry/atari_eval.py
 zoo/atari/envs/__init__.py
 zoo/atari/envs/atari_lightzero_env.py
@@ -168,14 +216,15 @@
 zoo/board_games/go/envs/__init__.py
 zoo/board_games/go/envs/go_env.py
 zoo/board_games/go/envs/test_go_env.py
 zoo/board_games/gomoku/__init__.py
 zoo/board_games/gomoku/config/__init__.py
 zoo/board_games/gomoku/config/gomoku_alphazero_bot_mode_config.py
 zoo/board_games/gomoku/config/gomoku_alphazero_sp_mode_config.py
+zoo/board_games/gomoku/config/gomoku_gumbel_alphazero_bot_mode_config.py
 zoo/board_games/gomoku/config/gomoku_gumbel_muzero_bot_mode_config.py
 zoo/board_games/gomoku/config/gomoku_muzero_bot_mode_config.py
 zoo/board_games/gomoku/config/gomoku_muzero_sp_mode_config.py
 zoo/board_games/gomoku/config/gomoku_sampled_alphazero_bot_mode_config.py
 zoo/board_games/gomoku/config/gomoku_sampled_alphazero_sp_mode_config.py
 zoo/board_games/gomoku/entry/__init__.py
 zoo/board_games/gomoku/entry/gomoku_alphazero_eval.py
@@ -201,17 +250,21 @@
 zoo/board_games/gomoku/test/test_legal_actions_cython.py
 zoo/board_games/tictactoe/__init__.py
 zoo/board_games/tictactoe/config/__init__.py
 zoo/board_games/tictactoe/config/tictactoe_alphazero_bot_mode_config.py
 zoo/board_games/tictactoe/config/tictactoe_alphazero_bot_mode_multigpu_ddp_config.py
 zoo/board_games/tictactoe/config/tictactoe_alphazero_sp_mode_config.py
 zoo/board_games/tictactoe/config/tictactoe_alphazero_sp_mode_multigpu_ddp_config.py
+zoo/board_games/tictactoe/config/tictactoe_efficientzero_bot_mode_config.py
+zoo/board_games/tictactoe/config/tictactoe_efficientzero_sp_mode_config.py
 zoo/board_games/tictactoe/config/tictactoe_gumbel_muzero_bot_mode_config.py
 zoo/board_games/tictactoe/config/tictactoe_muzero_bot_mode_config.py
 zoo/board_games/tictactoe/config/tictactoe_muzero_sp_mode_config.py
+zoo/board_games/tictactoe/config/tictactoe_sampled_alphazero_bot_mode_config.py
+zoo/board_games/tictactoe/config/tictactoe_sampled_alphazero_sp_mode_config.py
 zoo/board_games/tictactoe/entry/__init__.py
 zoo/board_games/tictactoe/entry/tictactoe_alphazero_eval.py
 zoo/board_games/tictactoe/entry/tictactoe_muzero_eval.py
 zoo/board_games/tictactoe/envs/__init__.py
 zoo/board_games/tictactoe/envs/test_tictactoe_alphabeta_prunning_bot.py
 zoo/board_games/tictactoe/envs/test_tictactoe_env.py
 zoo/board_games/tictactoe/envs/test_tictactoe_mcts_bot.py
@@ -246,40 +299,66 @@
 zoo/box2d/lunarlander/envs/test_lunarlander_env.py
 zoo/classic_control/__init__.py
 zoo/classic_control/cartpole/__init__.py
 zoo/classic_control/cartpole/config/__init__.py
 zoo/classic_control/cartpole/config/cartpole_efficientzero_config.py
 zoo/classic_control/cartpole/config/cartpole_gumbel_muzero_config.py
 zoo/classic_control/cartpole/config/cartpole_muzero_config.py
-zoo/classic_control/cartpole/config/cartpole_muzero_config_ckpt.py
+zoo/classic_control/cartpole/config/cartpole_muzero_config_ckpt_tmp.py
 zoo/classic_control/cartpole/config/cartpole_sampled_efficientzero_config.py
 zoo/classic_control/cartpole/config/cartpole_stochastic_muzero_config.py
 zoo/classic_control/cartpole/entry/__init__.py
 zoo/classic_control/cartpole/entry/cartpole_eval.py
 zoo/classic_control/cartpole/envs/__init__.py
 zoo/classic_control/cartpole/envs/cartpole_lightzero_env.py
+zoo/classic_control/mountain_car/__init__.py
+zoo/classic_control/mountain_car/entry/__init__.py
+zoo/classic_control/mountain_car/entry/mountain_car_eval.py
+zoo/classic_control/mountain_car/envs/__init__.py
+zoo/classic_control/mountain_car/envs/mtcar_lightzero_env.py
+zoo/classic_control/mountain_car/envs/test_mtcar_env.py
 zoo/classic_control/pendulum/__init__.py
 zoo/classic_control/pendulum/config/__init__.py
 zoo/classic_control/pendulum/config/pendulum_cont_disc_efficientzero_config.py
 zoo/classic_control/pendulum/config/pendulum_cont_disc_gumbel_muzero_config.py
 zoo/classic_control/pendulum/config/pendulum_cont_disc_muzero_config.py
 zoo/classic_control/pendulum/config/pendulum_cont_disc_sampled_efficientzero_config.py
+zoo/classic_control/pendulum/config/pendulum_cont_disc_stochastic_muzero_config.py
 zoo/classic_control/pendulum/config/pendulum_cont_sampled_efficientzero_config.py
 zoo/classic_control/pendulum/entry/__init__.py
 zoo/classic_control/pendulum/entry/pendulum_eval.py
 zoo/classic_control/pendulum/envs/__init__.py
 zoo/classic_control/pendulum/envs/pendulum_lightzero_env.py
 zoo/game_2048/__init__.py
 zoo/game_2048/entry/2048_bot_eval.py
 zoo/game_2048/entry/2048_eval.py
 zoo/game_2048/entry/__init__.py
 zoo/game_2048/envs/__init__.py
 zoo/game_2048/envs/expectimax_search_based_bot.py
 zoo/game_2048/envs/game_2048_env.py
 zoo/game_2048/envs/test_game_2048_env.py
+zoo/memory/__init__.py
+zoo/memory/config/__init__.py
+zoo/memory/config/memory_efficientzero_config.py
+zoo/memory/config/memory_muzero_config.py
+zoo/memory/config/memory_muzero_rnd_config.py
+zoo/memory/config/memory_sampled_efficientzero_config.py
+zoo/memory/entry/__init__.py
+zoo/memory/entry/memory_eval.py
+zoo/memory/envs/__init__.py
+zoo/memory/envs/memory_lightzero_env.py
+zoo/memory/envs/test_memory_lightzero_env.py
+zoo/memory/envs/test_render.py
+zoo/memory/envs/pycolab_tvt/__init__.py
+zoo/memory/envs/pycolab_tvt/common.py
+zoo/memory/envs/pycolab_tvt/game.py
+zoo/memory/envs/pycolab_tvt/human_player.py
+zoo/memory/envs/pycolab_tvt/key_to_door.py
+zoo/memory/envs/pycolab_tvt/objects.py
+zoo/memory/envs/pycolab_tvt/visual_match.py
 zoo/minigrid/__init__.py
 zoo/minigrid/config/__init__.py
 zoo/minigrid/config/minigrd_sampled_efficientzero_config.py
 zoo/minigrid/config/minigrid_efficientzero_config.py
 zoo/minigrid/config/minigrid_muzero_config.py
 zoo/minigrid/config/minigrid_muzero_rnd_config.py
 zoo/minigrid/entry/__init__.py
```

### Comparing `LightZero-0.0.2/LightZero.egg-info/requires.txt` & `LightZero-0.0.5/LightZero.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,16 @@
-DI-engine[common_env]>=0.4.7
-gym[accept-rom-license]==0.25.1
+DI-engine>=0.4.7
+gymnasium[atari]
+moviepy
 numpy>=1.22.4
 pympler
+bsuite
+minigrid
+moviepy
+pycolab
 
 [build]
 cython>=0.29
 build>=0.7.0
 auditwheel>=4
 numpy>=1.22.4
```

### Comparing `LightZero-0.0.2/README.md` & `LightZero-0.0.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -23,17 +23,18 @@
 [![GitHub forks](https://img.shields.io/github/forks/opendilab/LightZero)](https://github.com/opendilab/LightZero/network)
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/opendilab/LightZero)
 [![GitHub issues](https://img.shields.io/github/issues/opendilab/LightZero)](https://github.com/opendilab/LightZero/issues)
 [![GitHub pulls](https://img.shields.io/github/issues-pr/opendilab/LightZero)](https://github.com/opendilab/LightZero/pulls)
 [![Contributors](https://img.shields.io/github/contributors/opendilab/LightZero)](https://github.com/opendilab/LightZero/graphs/contributors)
 [![GitHub license](https://img.shields.io/github/license/opendilab/LightZero)](https://github.com/opendilab/LightZero/blob/master/LICENSE)
 
-Updated on 2023.09.21 LightZero-v0.0.2
+Updated on 2024.04.12 LightZero-v0.0.5
 
-> LightZero is a lightweight, efficient, and easy-to-understand open-source algorithm toolkit that combines Monte Carlo Tree Search (MCTS) and Deep Reinforcement Learning (RL). 
+> LightZero is a lightweight, efficient, and easy-to-understand open-source algorithm toolkit that combines Monte Carlo Tree Search (MCTS) and Deep Reinforcement Learning (RL).
+> For any questions about LightZero, you can consult the RAG-based Q&A assistant: [ZeroPal](https://huggingface.co/spaces/OpenDILabCommunity/ZeroPal)gst.
 
 English | [简体中文(Simplified Chinese)](https://github.com/opendilab/LightZero/blob/main/README.zh.md) | [Paper](https://arxiv.org/pdf/2310.08348.pdf)
 
 ## Background
 
 The integration of Monte Carlo Tree Search and Deep Reinforcement Learning,
 exemplified by AlphaZero and MuZero,
@@ -117,28 +118,30 @@
 - [Stochastic MuZero](https://openreview.net/pdf?id=X6D9bAHhBQ1)
 - [EfficientZero](https://arxiv.org/abs/2111.00210)
 - [Gumbel MuZero](https://openreview.net/pdf?id=bERaNdoegnO&)
 
 The environments and algorithms currently supported by LightZero are shown in the table below:
 
 | Env./Algo.    | AlphaZero | MuZero | EfficientZero | Sampled EfficientZero | Gumbel MuZero | Stochastic MuZero | 
-|---------------| --------- | ------ |-------------| ------------------ | ---------- |----------------|
-| TicTacToe     | ✔       | ✔      | 🔒           | 🔒                | ✔          | 🔒             |
-| Gomoku        | ✔       | ✔      | 🔒          | 🔒               | ✔          | 🔒             |
-| Connect4      | ✔       | ✔      | 🔒          | 🔒               | 🔒           | 🔒             |
-| 2048          | ✔       | ✔      | 🔒            | 🔒                | 🔒           | ✔              |
-| Chess         | 🔒       | 🔒     | 🔒          | 🔒               | 🔒         | 🔒             |
-| Go            | 🔒       | 🔒     | 🔒          | 🔒               | 🔒         | 🔒             |
-| CartPole      | ---       | ✔      | ✔           | ✔                | ✔          | ✔              |
-| Pendulum      | ---       | ✔      | ✔           | ✔                | ✔          | 🔒             |
-| LunarLander   | ---       | ✔      | ✔           | ✔                | ✔          | ✔              |
-| BipedalWalker | ---       | ✔      | ✔           | ✔                | ✔          | 🔒              |
-| Atari         | ---       | ✔      | ✔           | ✔                | ✔          | ✔              |
-| MuJoCo        | ---       | ✔     | ✔          | ✔                | 🔒         | 🔒               |
-| MiniGrid      | ---       | 🔒     | 🔒          | 🔒               | 🔒         | 🔒             |
+|---------------| -------- | ------ |-------------| ------------------ | ---------- |----------------|
+| TicTacToe     | ✔      | ✔      | 🔒           | 🔒                | ✔          | 🔒             |
+| Gomoku        | ✔      | ✔      | 🔒          | 🔒               | ✔          | 🔒             |
+| Connect4      | ✔      | ✔      | 🔒          | 🔒               | 🔒           | 🔒             |
+| 2048          | ---       | ✔      | 🔒            | 🔒                | 🔒           | ✔              |
+| Chess         | 🔒      | 🔒     | 🔒          | 🔒               | 🔒         | 🔒             |
+| Go            | 🔒      | 🔒     | 🔒          | 🔒               | 🔒         | 🔒             |
+| CartPole      | ---      | ✔      | ✔           | ✔                | ✔          | ✔              |
+| Pendulum      | ---      | ✔      | ✔           | ✔                | ✔          | ✔              |
+| LunarLander   | ---      | ✔      | ✔           | ✔                | ✔          | ✔              |
+| BipedalWalker | ---      | ✔      | ✔           | ✔                | ✔          | 🔒              |
+| Atari         | ---      | ✔      | ✔           | ✔                | ✔          | ✔              |
+| MuJoCo        | ---      | ✔     | ✔          | ✔                | 🔒         | 🔒               |
+| MiniGrid      | ---      | ✔     | ✔          | ✔               | 🔒         | 🔒             |
+| Bsuite        | ---      | ✔     | ✔          | ✔               | 🔒         | 🔒             |
+| Memory        | ---      | ✔     | ✔          | ✔               | 🔒         | 🔒             |
 
 <sup>(1): "✔" means that the corresponding item is finished and well-tested.</sup>
 
 <sup>(2): "🔒" means that the corresponding item is in the waiting-list (Work In Progress).</sup>
 
 <sup>(3): "---" means that this algorithm doesn't support this environment.</sup>
 
@@ -202,14 +205,23 @@
 Train a MuZero agent to play [TicTacToe](https://en.wikipedia.org/wiki/Tic-tac-toe):
 
 ```bash
 cd LightZero
 python3 -u zoo/board_games/tictactoe/config/tictactoe_muzero_bot_mode_config.py
 ```
 
+## Customization Documentation
+
+For those looking to tailor environments and algorithms, we offer comprehensive guides:
+
+- **Environments:** [Customize Environments](https://github.com/opendilab/LightZero/blob/main/docs/source/tutorials/envs/customize_envs.md)
+- **Algorithms:** [Customize Algorithms](https://github.com/opendilab/LightZero/blob/main/docs/source/tutorials/algos/customize_algos.md)
+
+Should you have any questions, feel free to contact us for support.
+
 ## Benchmark
 
 <details open><summary>Click to collapse</summary>
 
 - Below are the benchmark results of [AlphaZero](https://github.com/opendilab/LightZero/blob/main/lzero/policy/alphazero.py) and [MuZero](https://github.com/opendilab/LightZero/blob/main/lzero/policy/muzero.py) on three board games: [TicTacToe](https://github.com/opendilab/LightZero/blob/main/zoo/board_games/tictactoe/envs/tictactoe_env.py), [Connect4](https://github.com/opendilab/LightZero/blob/main/zoo/board_games/connect4/envs/connect4_env.py), [Gomoku](https://github.com/opendilab/LightZero/blob/main/zoo/board_games/gomoku/envs/gomoku_env.py).
 <p align="center">
   <img src="assets/benchmark/main/tictactoe_bot-mode_main.png" alt="tictactoe_bot-mode_main" width="30%" height="auto" style="margin: 0 1%;">
@@ -307,52 +319,61 @@
 
 #### LightZero Implemented series
 
 - [2018 _Science_ AlphaZero: A general reinforcement learning algorithm that masters chess, shogi, and Go through self-play](https://www.science.org/doi/10.1126/science.aar6404)
 - [2019 MuZero: Mastering Atari, Go, Chess and Shogi by Planning with a Learned Model](https://arxiv.org/abs/1911.08265)
 - [2021 EfficientZero: Mastering Atari Games with Limited Data](https://arxiv.org/abs/2111.00210)
 - [2021 Sampled MuZero: Learning and Planning in Complex Action Spaces](https://arxiv.org/abs/2104.06303)
-
-[comment]: <> (- [2022 Gumbel MuZero: Policy Improoveemenet by Planning with Gumbel]&#40;https://openreview.net/pdf?id=bERaNdoegnO&#41;)
+- [2022 Stochastic MuZero: Planning in Stochastic Environments with A Learned Model](https://openreview.net/pdf?id=X6D9bAHhBQ1)
+- [2022 Gumbel MuZero: Policy Improvement by Planning with Gumbel](https://openreview.net/pdf?id=bERaNdoegnO&)
 
 #### AlphaGo series
-
 - [2015 _Nature_ AlphaGo Mastering the game of Go with deep neural networks and tree search](https://www.nature.com/articles/nature16961)
 - [2017 _Nature_ AlphaGo Zero Mastering the game of Go without human knowledge](https://www.nature.com/articles/nature24270)
 - [2019 ELF OpenGo: An Analysis and Open Reimplementation of AlphaZero](https://arxiv.org/abs/1902.04522) 
   - [Code](https://github.com/pytorch/ELF)
+- [2023 Student of Games: A unified learning algorithm for both perfect and imperfect information games](https://www.science.org/doi/10.1126/sciadv.adg3256)
+
 #### MuZero series
 - [2022 Online and Offline Reinforcement Learning by Planning with a Learned Model](https://arxiv.org/abs/2104.06294)
 - [2021 Vector Quantized Models for Planning](https://arxiv.org/abs/2106.04615)
-- [2022 Stochastic MuZero: Planning in Stochastic Environments with A Learned Model](https://openreview.net/pdf?id=X6D9bAHhBQ1)
 - [2021 Muesli: Combining Improvements in Policy Optimization. ](https://arxiv.org/abs/2104.06159)
 #### MCTS Analysis
 - [2020 Monte-Carlo Tree Search as Regularized Policy Optimization](https://arxiv.org/abs/2007.12509)
 - [2021 Self-Consistent Models and Values](https://arxiv.org/abs/2110.12840)
 - [2022 Adversarial Policies Beat Professional-Level Go AIs](https://arxiv.org/abs/2211.00241)
 - [2022 _PNAS_ Acquisition of Chess Knowledge in AlphaZero.](https://arxiv.org/abs/2111.09259)
 
 #### MCTS Application
+- [2023 Symbolic Physics Learner: Discovering governing equations via Monte Carlo tree search](https://openreview.net/pdf?id=ZTK3SefE8_Z)
 - [2022 _Nature_ Discovering faster matrix multiplication algorithms with reinforcement learning](https://www.nature.com/articles/s41586-022-05172-4) 
   - [Code](https://github.com/deepmind/alphatensor)
 - [2022 MuZero with Self-competition for Rate Control in VP9 Video Compression](https://arxiv.org/abs/2202.06626)
 - [2021 DouZero: Mastering DouDizhu with Self-Play Deep Reinforcement Learning](https://arxiv.org/abs/2106.06135)
 - [2019 Combining Planning and Deep Reinforcement Learning in Tactical Decision Making for Autonomous Driving](https://arxiv.org/pdf/1905.02680.pdf)
 
 </details>
 
 ### Other Papers
 
 <details><summary>Click to expand</summary>
 
 #### ICML
+- [Scalable Safe Policy Improvement via Monte Carlo Tree Search](https://openreview.net/pdf?id=tevbBSzSfK) 2023
+  - Alberto Castellini, Federico Bianchi, Edoardo Zorzi, Thiago D. Simão, Alessandro Farinelli, Matthijs T. J. Spaan
+  - Key: safe policy improvement online using a MCTS based strategy, Safe Policy Improvement with Baseline Bootstrapping
+  - ExpEnv: Gridworld and SysAdmin
 - [Efficient Learning for AlphaZero via Path Consistency](https://proceedings.mlr.press/v162/zhao22h/zhao22h.pdf) 2022
   - Dengwei Zhao, Shikui Tu, Lei Xu
   - Key: limited amount of self-plays,  path consistency (PC) optimality
   - ExpEnv: Go, Othello, Gomoku
+- [Visualizing MuZero Models](https://arxiv.org/abs/2102.12924) 2021
+  - Joery A. de Vries, Ken S. Voskuil, Thomas M. Moerland, Aske Plaat
+  - Key: visualizing the value equivalent dynamics model, action trajectories diverge, two regularization techniques
+  - ExpEnv: CartPole and MountainCar.
 - [Convex Regularization in Monte-Carlo Tree Search](https://arxiv.org/pdf/2007.00391.pdf) 2021
   - Tuan Dam, Carlo D'Eramo, Jan Peters, Joni Pajarinen
   - Key: entropy-regularization backup operators, regret analysis, Tsallis etropy, 
   - ExpEnv: synthetic tree, Atari
 - [Information Particle Filter Tree: An Online Algorithm for POMDPs with Belief-Based Rewards on Continuous Domains](http://proceedings.mlr.press/v119/fischer20a/fischer20a.pdf) 2020
   - Johannes Fischer, Ömer Sahin Tas
   - Key: Continuous POMDP, Particle Filter Tree, information-based reward shaping, Information Gathering.
@@ -360,14 +381,34 @@
   - [Code](https://github.com/johannes-fischer/icml2020_ipft)
 - [Retro*: Learning Retrosynthetic Planning with Neural Guided A* Search](http://proceedings.mlr.press/v119/chen20k/chen20k.pdf) 2020
   - Binghong Chen, Chengtao Li, Hanjun Dai, Le Song 
   - Key: chemical retrosynthetic planning, neural-based A*-like algorithm, ANDOR tree
   - ExpEnv: USPTO datasets
   - [Code](https://github.com/binghong-ml/retro_star)
 #### ICLR
+- [The Update Equivalence Framework for Decision-Time Planning](https://openreview.net/forum?id=JXGph215fL) 2024
+  - Samuel Sokota, Gabriele Farina, David J Wu, Hengyuan Hu, Kevin A. Wang, J Zico Kolter, Noam Brown
+  - Key: imperfect-information games, search, decision-time planning, update equivalence
+  - ExpEnv: Hanabi, 3x3 Abrupt Dark Hex and Phantom Tic-Tac-Toe
+- [Efficient Multi-agent Reinforcement Learning by Planning](https://openreview.net/forum?id=CpnKq3UJwp) 2024
+  - Qihan Liu, Jianing Ye, Xiaoteng Ma, Jun Yang, Bin Liang, Chongjie Zhang
+  - Key: multi-agent reinforcement learning, planning, multi-agent MCTS
+  - ExpEnv: SMAC, LunarLander, MuJoCo, and Google Research Football
+- [Become a Proficient Player with Limited Data through Watching Pure Videos](https://openreview.net/pdf?id=Sy-o2N0hF4f) 2023
+  - Weirui Ye, Yunsheng Zhang, Pieter Abbeel, Yang Gao
+  - Key: pre-training from action-free videos, forward-inverse cycle consistency (FICC) objective based on vector quantization, pre-training phase, fine-tuning phase.
+  - ExpEnv: Atari
+- [Policy-Based Self-Competition for Planning Problems](https://arxiv.org/abs/2306.04403) 2023
+  - Jonathan Pirnay, Quirin Göttl, Jakob Burger, Dominik Gerhard Grimm
+  - Key: self-competition, find strong trajectories by planning against possible strategies of its past self.
+  - ExpEnv: Traveling Salesman Problem and the Job-Shop Scheduling Problem.
+- [Explaining Temporal Graph Models through an Explorer-Navigator Framework](https://openreview.net/pdf?id=BR_ZhvcYbGJ) 2023
+  - Wenwen Xia, Mincai Lai, Caihua Shan, Yao Zhang, Xinnan Dai, Xiang Li, Dongsheng Li
+  - Key: Temporal GNN Explainer, an explorer to find the event subsets with MCTS, a navigator that learns the correlations between events and helps reduce the search space.
+  - ExpEnv: Wikipedia and Reddit, Synthetic datasets
 - [SpeedyZero: Mastering Atari with Limited Data and Time](https://openreview.net/pdf?id=Mg5CLXZgvLJ) 2023
   - Yixuan Mei, Jiaxuan Gao, Weirui Ye, Shaohuai Liu, Yang Gao, Yi Wu
   - Key: distributed RL system, Priority Refresh, Clipped LARS
   - ExpEnv: Atari
 - [Efficient Offline Policy Optimization with a Learned Model](https://openreview.net/pdf?id=Yt-yM-JbYFO) 2023
   - Zichen Liu, Siyi Li, Wee Sun Lee, Shuicheng YAN, Zhongwen Xu
   - Key: Regularized One-Step Model-based algorithm for Offline-RL
@@ -375,85 +416,113 @@
   - [Code](https://github.com/sail-sg/rosmo/tree/main)
 - [Enabling Arbitrary Translation Objectives with Adaptive Tree Search](https://arxiv.org/pdf/2202.11444.pdf) 2022
   - Wang Ling, Wojciech Stokowiec, Domenic Donato, Chris Dyer, Lei Yu, Laurent Sartran, Austin Matthews
   - Key: adaptive tree search, translation models, autoregressive models, 
   - ExpEnv: Chinese–English and Pashto–English tasks from WMT2020, German–English from WMT2014
 - [What's Wrong with Deep Learning in Tree Search for Combinatorial Optimization](https://arxiv.org/abs/2201.10494) 2022
   - Maximili1an Böther, Otto Kißig, Martin Taraz, Sarel Cohen, Karen Seidel, Tobias Friedrich
-  - Key: Combinatorial optimization, open-source benchmark suite for the NP-hard MAXIMUM INDEPENDENT SET problem, an in-depth analysis of the popular guided tree search algorithm,  compare the tree search implementations to other solvers
+  - Key: combinatorial optimization, open-source benchmark suite for the NP-hard maximum independent set problem, an in-depth analysis of the popular guided tree search algorithm, compare the tree search implementations to other solvers
   - ExpEnv: NP-hard MAXIMUM INDEPENDENT SET.
   - [Code](https://github.com/maxiboether/mis-benchmark-framework)
 - [Monte-Carlo Planning and Learning with Language Action Value Estimates](https://openreview.net/pdf?id=7_G8JySGecm) 2021
   - Youngsoo Jang, Seokin Seo, Jongmin Lee, Kee-Eung Kim
-  - Key: Monte-Carlo tree search with language-driven exploration, locally optimistic language value estimates,
+  - Key: Monte-Carlo tree search with language-driven exploration, locally optimistic language value estimates.
   - ExpEnv: Interactive Fiction (IF) games
 - [Practical Massively Parallel Monte-Carlo Tree Search Applied to Molecular Design](https://arxiv.org/abs/2006.10504) 2021
   - Xiufeng Yang, Tanuj Kr Aasawat, Kazuki Yoshizoe
   - Key: massively parallel Monte-Carlo Tree Search, molecular design, Hash-driven parallel search, 
   - ExpEnv:  octanol-water partition coefficient (logP) penalized by the synthetic accessibility (SA) and large Ring Penalty score.
 - [Watch the Unobserved: A Simple Approach to Parallelizing Monte Carlo Tree Search](https://arxiv.org/pdf/1810.11755.pdf) 2020
   - Anji Liu, Jianshu Chen, Mingze Yu, Yu Zhai, Xuewen Zhou, Ji Liu
-  - Key: parallel Monte-Carlo Tree Search, partition the tree into sub-trees efficiently, compare the observation ratio of each processor
+  - Key: parallel Monte-Carlo Tree Search, partition the tree into sub-trees efficiently, compare the observation ratio of each processor.
   - ExpEnv: speedup and performance comparison on JOY-CITY game, average episode return on atari game
   - [Code](https://github.com/liuanji/WU-UCT)
 - [Learning to Plan in High Dimensions via Neural Exploration-Exploitation Trees](https://openreview.net/pdf?id=rJgJDAVKvB) 2020
-  - Binghong Chen,  Bo Dai, Qinjie Lin, Guo Ye, Han Liu, Le Song
+  - Binghong Chen, Bo Dai, Qinjie Lin, Guo Ye, Han Liu, Le Song
   - Key: meta path planning algorithm, exploits a novel neural architecture which can learn promising search directions from problem structures.
   - ExpEnv: a 2d workspace with a 2 DoF (degrees of freedom) point robot, a 3 DoF stick robot and a 5 DoF snake robot
 #### NeurIPS
+- [LightZero: A Unified Benchmark for Monte Carlo Tree Search in General Sequential Decision Scenarios](https://openreview.net/pdf?id=oIUXpBnyjv) 2023
+  - Yazhe Niu, Yuan Pu, Zhenjie Yang, Xueyan Li, Tong Zhou, Jiyuan Ren, Shuai Hu, Hongsheng Li, Yu Liu
+  - Key: the first unified benchmark for deploying MCTS/MuZero in general sequential decision scenarios.
+  - ExpEnv: ClassicControl, Box2D, Atari, MuJoCo, GoBigger, MiniGrid, TicTacToe, ConnectFour, Gomoku, 2048, etc.
+- [Large Language Models as Commonsense Knowledge for Large-Scale Task Planning](https://openreview.net/pdf?id=Wjp1AYB8lH) 2023
+  - Zirui Zhao, Wee Sun Lee, David Hsu
+  - Key: world model (LLM) and the LLM-induced policy can be combined in MCTS, to scale up task planning.
+  - ExpEnv: multiplication, travel planning, object rearrangement
+- [Monte Carlo Tree Search with Boltzmann Exploration](https://openreview.net/pdf?id=NG4DaApavi) 2023
+  - Michael Painter, Mohamed Baioumy, Nick Hawes, Bruno Lacerda
+  - Key: Boltzmann exploration with MCTS, optimal actions for the maximum entropy objective do not necessarily correspond to optimal actions for the original objective, two improved algorithms.
+  - ExpEnv: the Frozen Lake environment, the Sailing Problem, Go
+- [Generalized Weighted Path Consistency for Mastering Atari Games](https://openreview.net/pdf?id=vHRLS8HhK1) 2023
+  - Dengwei Zhao, Shikui Tu, Lei Xu
+  - Key: Generalized Weighted Path Consistency, A weighting mechanism.
+  - ExpEnv: Atari
+- [Accelerating Monte Carlo Tree Search with Probability Tree State Abstraction](https://openreview.net/pdf?id=0zeLTZAqaJ) 2023
+  - Yangqing Fu, Ming Sun, Buqing Nie, Yue Gao
+  - Key: probability tree state abstraction, transitivity and aggregation error bound
+  - ExpEnv: Atari, CartPole, LunarLander, Gomoku
+- [Spending Thinking Time Wisely: Accelerating MCTS with Virtual Expansions](https://openreview.net/pdf?id=B_LdLljS842) 2022
+  - Weirui Ye, Pieter Abbeel, Yang Gao
+  - Key: trade off computation versus performancem, virtual expansions, spend thinking time adaptively.
+  - ExpEnv: Atari, 9x9 Go
 - [Planning for Sample Efficient Imitation Learning](https://openreview.net/forum?id=BkN5UoAqF7) 2022
   - Zhao-Heng Yin, Weirui Ye, Qifeng Chen, Yang Gao
-  - Key: Behavioral Cloning，Adversarial Imitation Learning (AIL)，MCTS-based RL，
+  - Key: Behavioral Cloning，Adversarial Imitation Learning (AIL)，MCTS-based RL.
   - ExpEnv:  DeepMind Control Suite
   - [Code](https://github.com/zhaohengyin/EfficientImitate)
 - [Evaluation Beyond Task Performance: Analyzing Concepts in AlphaZero in Hex](https://openreview.net/pdf?id=dwKwB2Cd-Km) 2022 
   - Charles Lovering, Jessica Zosa Forde, George Konidaris, Ellie Pavlick, Michael L. Littman
   - Key: AlphaZero’s internal representations, model probing and behavioral tests, how these concepts are captured in the network.
   - ExpEnv: Hex
 - [Are AlphaZero-like Agents Robust to Adversarial Perturbations?](https://openreview.net/pdf?id=yZ_JlZaOCzv) 2022
   - Li-Cheng Lan, Huan Zhang, Ti-Rong Wu, Meng-Yu Tsai, I-Chen Wu, 4 Cho-Jui Hsieh
-  - Key:  adversarial states, first adversarial attack on Go AIs
+  - Key: adversarial states, first adversarial attack on Go AIs.
   - ExpEnv: Go
 - [Monte Carlo Tree Descent for Black-Box Optimization](https://openreview.net/pdf?id=FzdmrTUyZ4g) 2022
   - Yaoguang Zhai, Sicun Gao
   - Key: Black-Box Optimization, how to further integrate samplebased descent for faster optimization. 
   - ExpEnv: synthetic functions for nonlinear optimization, reinforcement learning problems in MuJoCo locomotion environments, and optimization problems in Neural Architecture Search (NAS).
 - [Monte Carlo Tree Search based Variable Selection for High Dimensional Bayesian Optimization](https://openreview.net/pdf?id=SUzPos_pUC) 2022
   - Lei Song∗ , Ke Xue∗ , Xiaobin Huang, Chao Qian
   - Key:  a low-dimensional subspace via MCTS, optimizes in the subspace with any Bayesian optimization algorithm.
   - ExpEnv: NAS-bench problems and MuJoCo locomotion
 - [Monte Carlo Tree Search With Iteratively Refining State Abstractions](https://proceedings.neurips.cc/paper/2021/file/9b0ead00a217ea2c12e06a72eec4923f-Paper.pdf) 2021
   - Samuel Sokota, Caleb Ho, Zaheen Ahmad, J. Zico Kolter
-  - Key: stochastic environments, Progressive widening, abstraction refining,
+  - Key: stochastic environments, Progressive widening, abstraction refining
   - ExpEnv:  Blackjack, Trap, five by five Go.
 - [Deep Synoptic Monte Carlo Planning in Reconnaissance Blind Chess](https://proceedings.neurips.cc/paper/2021/file/215a71a12769b056c3c32e7299f1c5ed-Paper.pdf) 2021
   - Gregory Clark
   - Key: imperfect information, belief state with an unweighted particle filter, a novel stochastic abstraction of information states.
   - ExpEnv:  reconnaissance blind chess
 - [POLY-HOOT: Monte-Carlo Planning in Continuous Space MDPs with Non-Asymptotic Analysis](https://proceedings.neurips.cc/paper/2020/file/30de24287a6d8f07b37c716ad51623a7-Paper.pdf) 2020
   - Weichao Mao, Kaiqing Zhang, Qiaomin Xie, Tamer Ba¸sar
-  - Key: continuous state-action spaces, Hierarchical Optimistic Optimization,
+  - Key: continuous state-action spaces, Hierarchical Optimistic Optimization.
   - ExpEnv: CartPole, Inverted Pendulum, Swing-up, and LunarLander.
 - [Learning Search Space Partition for Black-box Optimization using Monte Carlo Tree Search](https://proceedings.neurips.cc/paper/2020/file/e2ce14e81dba66dbff9cbc35ecfdb704-Paper.pdf) 2020
   - Linnan Wang, Rodrigo Fonseca, Yuandong Tian
   - Key: learns the partition of the search space using a few samples, a nonlinear decision boundary and learns a local model to pick good candidates.
   - ExpEnv: MuJoCo locomotion tasks, Small-scale Benchmarks, 
 - [Mix and Match: An Optimistic Tree-Search Approach for Learning Models from Mixture Distributions](https://arxiv.org/abs/1907.10154) 2020
   - Matthew Faw, Rajat Sen, Karthikeyan Shanmugam, Constantine Caramanis, Sanjay Shakkottai
   - Key: covariate shift problem, Mix&Match combines stochastic gradient descent (SGD) with optimistic tree search and model re-use (evolving partially trained models with samples from different mixture distributions)
   - [Code](https://github.com/matthewfaw/mixnmatch)
 
 #### Other Conference or Journal
+- [Learning to Stop: Dynamic Simulation Monte-Carlo Tree Search](https://arxiv.org/pdf/2012.07910.pdf) AAAI 2021.
 - [On Monte Carlo Tree Search and Reinforcement Learning](https://www.jair.org/index.php/jair/article/download/11099/26289/20632) Journal of Artificial Intelligence Research 2017.
 - [Sample-Efficient Neural Architecture Search by Learning Actions for Monte Carlo Tree Search](https://arxiv.org/pdf/1906.06832) IEEE Transactions on Pattern Analysis and Machine Intelligence 2022.
 </details>
 
 
 ## Feedback and Contribution
+
 - [File an issue](https://github.com/opendilab/LightZero/issues/new/choose) on Github
+- Open or participate in our [discussion forum](https://github.com/opendilab/LightZero/discussions)
+- Discuss on LightZero [discord server](https://discord.gg/qZTQTycu)
 - Contact our email (opendilab@pjlab.org.cn)
 
 - We appreciate all the feedback and contributions to improve LightZero, both algorithms and system designs. 
 
 [comment]: <> (- Contributes to our future plan [Roadmap]&#40;https://github.com/opendilab/LightZero/projects&#41;)
 
 [comment]: <> (And `CONTRIBUTING.md` offers some necessary information.)
```

### Comparing `LightZero-0.0.2/lzero/config/utils.py` & `LightZero-0.0.5/lzero/config/utils.py`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/lzero/entry/eval_alphazero.py` & `LightZero-0.0.5/lzero/entry/eval_alphazero.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,14 +83,14 @@
             returns.append(episode_info['eval_episode_return'])
 
         returns = np.array(returns)
 
         if print_seed_details:
             print("=" * 20)
             print(f'In seed {seed}, returns: {returns}')
-            if cfg.policy.simulation_env_name in ['tictactoe', 'connect4', 'gomoku', 'chess']:
+            if cfg.policy.simulation_env_id in ['tictactoe', 'connect4', 'gomoku', 'chess']:
                 print(
                     f'win rate: {len(np.where(returns == 1.)[0]) / num_episodes_each_seed}, draw rate: {len(np.where(returns == 0.)[0]) / num_episodes_each_seed}, lose rate: {len(np.where(returns == -1.)[0]) / num_episodes_each_seed}'
                 )
             print("=" * 20)
 
         return returns.mean(), returns
```

### Comparing `LightZero-0.0.2/lzero/entry/eval_muzero.py` & `LightZero-0.0.5/lzero/entry/eval_muzero.py`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/lzero/entry/eval_muzero_with_gym_env.py` & `LightZero-0.0.5/lzero/entry/eval_muzero_with_gym_env.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         model_path: Optional[str] = None,
         num_episodes_each_seed: int = 1,
         print_seed_details: int = False,
 ) -> 'Policy':  # noqa
     """
     Overview:
         The eval entry for MCTS+RL algorithms, including MuZero, EfficientZero, Sampled EfficientZero.
-        We create a gym environment using env_name parameter, and then convert it to the format
+        We create a gym environment using env_id parameter, and then convert it to the format
         required by LightZero using LightZeroEnvWrapper class.
         Please refer to the get_wrappered_env method for more details.
     Arguments:
         - input_cfg (:obj:`Tuple[dict, dict]`): Config in dict type.
             ``Tuple[dict, dict]`` type means [user_config, create_cfg].
         - seed (:obj:`int`): Random seed.
         - model (:obj:`Optional[torch.nn.Module]`): Instance of torch.nn.Module.
@@ -51,18 +51,18 @@
 
     cfg = compile_config(cfg, seed=seed, env=None, auto=True, create_cfg=create_cfg, save_cfg=True)
 
     # Create main components: env, policy
     collector_env_cfg = DingEnvWrapper.create_collector_env_cfg(cfg.env)
     evaluator_env_cfg = DingEnvWrapper.create_evaluator_env_cfg(cfg.env)
     collector_env = BaseEnvManager(
-        [get_wrappered_env(c, cfg.env.env_name) for c in collector_env_cfg], cfg=BaseEnvManager.default_config()
+        [get_wrappered_env(c, cfg.env.env_id) for c in collector_env_cfg], cfg=BaseEnvManager.default_config()
     )
     evaluator_env = BaseEnvManager(
-        [get_wrappered_env(c, cfg.env.env_name) for c in evaluator_env_cfg], cfg=BaseEnvManager.default_config()
+        [get_wrappered_env(c, cfg.env.env_id) for c in evaluator_env_cfg], cfg=BaseEnvManager.default_config()
     )
     collector_env.seed(cfg.seed)
     evaluator_env.seed(cfg.seed, dynamic_seed=False)
     set_pkg_seed(cfg.seed, use_cuda=cfg.policy.cuda)
 
     policy = create_policy(cfg.policy, model=model, enable_field=['learn', 'collect', 'eval'])
```

### Comparing `LightZero-0.0.2/lzero/entry/train_alphazero.py` & `LightZero-0.0.5/lzero/entry/train_alphazero.py`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/lzero/entry/train_muzero.py` & `LightZero-0.0.5/lzero/entry/train_muzero.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         - max_env_step (:obj:`Optional[int]`): Maximum collected environment interaction steps.
     Returns:
         - policy (:obj:`Policy`): Converged policy.
     """
 
     cfg, create_cfg = input_cfg
     assert create_cfg.policy.type in ['efficientzero', 'muzero', 'sampled_efficientzero', 'gumbel_muzero', 'stochastic_muzero'], \
-        "train_muzero entry now only support the following algo.: 'efficientzero', 'muzero', 'sampled_efficientzero', 'gumbel_muzero'"
+        "train_muzero entry now only support the following algo.: 'efficientzero', 'muzero', 'sampled_efficientzero', 'gumbel_muzero', 'stochastic_muzero'"
 
     if create_cfg.policy.type == 'muzero':
         from lzero.mcts import MuZeroGameBuffer as GameBuffer
     elif create_cfg.policy.type == 'efficientzero':
         from lzero.mcts import EfficientZeroGameBuffer as GameBuffer
     elif create_cfg.policy.type == 'sampled_efficientzero':
         from lzero.mcts import SampledEfficientZeroGameBuffer as GameBuffer
@@ -73,14 +73,17 @@
     collector_env = create_env_manager(cfg.env.manager, [partial(env_fn, cfg=c) for c in collector_env_cfg])
     evaluator_env = create_env_manager(cfg.env.manager, [partial(env_fn, cfg=c) for c in evaluator_env_cfg])
 
     collector_env.seed(cfg.seed)
     evaluator_env.seed(cfg.seed, dynamic_seed=False)
     set_pkg_seed(cfg.seed, use_cuda=cfg.policy.cuda)
 
+    if cfg.policy.eval_offline:
+        cfg.policy.learn.learner.hook.save_ckpt_after_iter = cfg.policy.eval_freq
+
     policy = create_policy(cfg.policy, model=model, enable_field=['learn', 'collect', 'eval'])
 
     # load pretrained model
     if model_path is not None:
         policy.learn_mode.load_state_dict(torch.load(model_path, map_location=cfg.policy.device))
 
     # Create worker components: learner, collector, evaluator, replay buffer, commander.
@@ -113,23 +116,29 @@
     )
 
     # ==============================================================
     # Main loop
     # ==============================================================
     # Learner's before_run hook.
     learner.call_hook('before_run')
-    
+
     if cfg.policy.update_per_collect is not None:
         update_per_collect = cfg.policy.update_per_collect
 
     # The purpose of collecting random data before training:
     # Exploration: Collecting random data helps the agent explore the environment and avoid getting stuck in a suboptimal policy prematurely.
     # Comparison: By observing the agent's performance during random action-taking, we can establish a baseline to evaluate the effectiveness of reinforcement learning algorithms.
     if cfg.policy.random_collect_episode_num > 0:
         random_collect(cfg.policy, policy, LightZeroRandomPolicy, collector, collector_env, replay_buffer)
+    if cfg.policy.eval_offline:
+        eval_train_iter_list = []
+        eval_train_envstep_list = []
+
+    # Evaluate the random agent
+    stop, reward = evaluator.eval(learner.save_checkpoint, learner.train_iter, collector.envstep)
 
     while True:
         log_buffer_memory_usage(learner.train_iter, replay_buffer, tb_logger)
         collect_kwargs = {}
         # set temperature for visit count distributions according to the train_iter,
         # please refer to Appendix D in MuZero paper for details.
         collect_kwargs['temperature'] = visit_count_temperature(
@@ -148,17 +157,21 @@
             )
             collect_kwargs['epsilon'] = epsilon_greedy_fn(collector.envstep)
         else:
             collect_kwargs['epsilon'] = 0.0
 
         # Evaluate policy performance.
         if evaluator.should_eval(learner.train_iter):
-            stop, reward = evaluator.eval(learner.save_checkpoint, learner.train_iter, collector.envstep)
-            if stop:
-                break
+            if cfg.policy.eval_offline:
+                eval_train_iter_list.append(learner.train_iter)
+                eval_train_envstep_list.append(collector.envstep)
+            else:
+                stop, reward = evaluator.eval(learner.save_checkpoint, learner.train_iter, collector.envstep)
+                if stop:
+                    break
 
         # Collect data by default config n_sample/n_episode.
         new_data = collector.collect(train_iter=learner.train_iter, policy_kwargs=collect_kwargs)
         if cfg.policy.update_per_collect is None:
             # update_per_collect is None, then update_per_collect is set to the number of collected transitions multiplied by the model_update_ratio.
             collected_transitions_num = sum([len(game_segment) for game_segment in new_data[0]])
             update_per_collect = int(collected_transitions_num * cfg.policy.model_update_ratio)
@@ -184,12 +197,25 @@
             # The core train steps for MCTS+RL algorithms.
             log_vars = learner.train(train_data, collector.envstep)
 
             if cfg.policy.use_priority:
                 replay_buffer.update_priority(train_data, log_vars[0]['value_priority_orig'])
 
         if collector.envstep >= max_env_step or learner.train_iter >= max_train_iter:
+            if cfg.policy.eval_offline:
+                logging.info(f'eval offline beginning...')
+                ckpt_dirname = './{}/ckpt'.format(learner.exp_name)
+                # Evaluate the performance of the pretrained model.
+                for train_iter, collector_envstep in zip(eval_train_iter_list, eval_train_envstep_list):
+                    ckpt_name = 'iteration_{}.pth.tar'.format(train_iter)
+                    ckpt_path = os.path.join(ckpt_dirname, ckpt_name)
+                    # load the ckpt of pretrained model
+                    policy.learn_mode.load_state_dict(torch.load(ckpt_path, map_location=cfg.policy.device))
+                    stop, reward = evaluator.eval(learner.save_checkpoint, train_iter, collector_envstep)
+                    logging.info(
+                        f'eval offline at train_iter: {train_iter}, collector_envstep: {collector_envstep}, reward: {reward}')
+                logging.info(f'eval offline finished!')
             break
 
     # Learner's after_run hook.
     learner.call_hook('after_run')
     return policy
```

### Comparing `LightZero-0.0.2/lzero/entry/train_muzero_with_gym_env.py` & `LightZero-0.0.5/lzero/entry/train_muzero_with_gym_env.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         model_path: Optional[str] = None,
         max_train_iter: Optional[int] = int(1e10),
         max_env_step: Optional[int] = int(1e10),
 ) -> 'Policy':  # noqa
     """
     Overview:
         The train entry for MCTS+RL algorithms, including MuZero, EfficientZero, Sampled EfficientZero.
-        We create a gym environment using env_name parameter, and then convert it to the format required by LightZero using LightZeroEnvWrapper class.
+        We create a gym environment using env_id parameter, and then convert it to the format required by LightZero using LightZeroEnvWrapper class.
         Please refer to the get_wrappered_env method for more details.
     Arguments:
         - input_cfg (:obj:`Tuple[dict, dict]`): Config in dict type.
             ``Tuple[dict, dict]`` type means [user_config, create_cfg].
         - seed (:obj:`int`): Random seed.
         - model (:obj:`Optional[torch.nn.Module]`): Instance of torch.nn.Module.
         - model_path (:obj:`Optional[str]`): The pretrained model path, which should
@@ -61,18 +61,18 @@
 
     cfg = compile_config(cfg, seed=seed, env=None, auto=True, create_cfg=create_cfg, save_cfg=True)
 
     # Create main components: env, policy
     collector_env_cfg = DingEnvWrapper.create_collector_env_cfg(cfg.env)
     evaluator_env_cfg = DingEnvWrapper.create_evaluator_env_cfg(cfg.env)
     collector_env = BaseEnvManager(
-        [get_wrappered_env(c, cfg.env.env_name) for c in collector_env_cfg], cfg=BaseEnvManager.default_config()
+        [get_wrappered_env(c, cfg.env.env_id) for c in collector_env_cfg], cfg=BaseEnvManager.default_config()
     )
     evaluator_env = BaseEnvManager(
-        [get_wrappered_env(c, cfg.env.env_name) for c in evaluator_env_cfg], cfg=BaseEnvManager.default_config()
+        [get_wrappered_env(c, cfg.env.env_id) for c in evaluator_env_cfg], cfg=BaseEnvManager.default_config()
     )
     collector_env.seed(cfg.seed)
     evaluator_env.seed(cfg.seed, dynamic_seed=False)
     set_pkg_seed(cfg.seed, use_cuda=cfg.policy.cuda)
 
     policy = create_policy(cfg.policy, model=model, enable_field=['learn', 'collect', 'eval'])
```

### Comparing `LightZero-0.0.2/lzero/entry/train_muzero_with_reward_model.py` & `LightZero-0.0.5/lzero/entry/train_muzero_with_reward_model.py`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/lzero/entry/utils.py` & `LightZero-0.0.5/lzero/entry/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,31 +45,33 @@
     Overview:
         Log the memory usage of the buffer and the current process to TensorBoard.
     Arguments:
         - train_iter (:obj:`int`): The current training iteration.
         - buffer (:obj:`GameBuffer`): The game buffer.
         - writer (:obj:`SummaryWriter`): The TensorBoard writer.
     """
-    writer.add_scalar('Buffer/num_of_all_collected_episodes', buffer.num_of_collected_episodes, train_iter)
-    writer.add_scalar('Buffer/num_of_game_segments', len(buffer.game_segment_buffer), train_iter)
-    writer.add_scalar('Buffer/num_of_transitions', len(buffer.game_segment_game_pos_look_up), train_iter)
+    # "writer is None" means we are in a slave process in the DDP setup.
+    if writer is not None:
+        writer.add_scalar('Buffer/num_of_all_collected_episodes', buffer.num_of_collected_episodes, train_iter)
+        writer.add_scalar('Buffer/num_of_game_segments', len(buffer.game_segment_buffer), train_iter)
+        writer.add_scalar('Buffer/num_of_transitions', len(buffer.game_segment_game_pos_look_up), train_iter)
 
-    game_segment_buffer = buffer.game_segment_buffer
+        game_segment_buffer = buffer.game_segment_buffer
 
-    # Calculate the amount of memory occupied by self.game_segment_buffer (in bytes).
-    buffer_memory_usage = asizeof(game_segment_buffer)
+        # Calculate the amount of memory occupied by self.game_segment_buffer (in bytes).
+        buffer_memory_usage = asizeof(game_segment_buffer)
 
-    # Convert buffer_memory_usage to megabytes (MB).
-    buffer_memory_usage_mb = buffer_memory_usage / (1024 * 1024)
+        # Convert buffer_memory_usage to megabytes (MB).
+        buffer_memory_usage_mb = buffer_memory_usage / (1024 * 1024)
 
-    # Record the memory usage of self.game_segment_buffer to TensorBoard.
-    writer.add_scalar('Buffer/memory_usage/game_segment_buffer', buffer_memory_usage_mb, train_iter)
+        # Record the memory usage of self.game_segment_buffer to TensorBoard.
+        writer.add_scalar('Buffer/memory_usage/game_segment_buffer', buffer_memory_usage_mb, train_iter)
 
-    # Get the amount of memory currently used by the process (in bytes).
-    process = psutil.Process(os.getpid())
-    process_memory_usage = process.memory_info().rss
+        # Get the amount of memory currently used by the process (in bytes).
+        process = psutil.Process(os.getpid())
+        process_memory_usage = process.memory_info().rss
 
-    # Convert process_memory_usage to megabytes (MB).
-    process_memory_usage_mb = process_memory_usage / (1024 * 1024)
+        # Convert process_memory_usage to megabytes (MB).
+        process_memory_usage_mb = process_memory_usage / (1024 * 1024)
 
-    # Record the memory usage of the process to TensorBoard.
-    writer.add_scalar('Buffer/memory_usage/process', process_memory_usage_mb, train_iter)
+        # Record the memory usage of the process to TensorBoard.
+        writer.add_scalar('Buffer/memory_usage/process', process_memory_usage_mb, train_iter)
```

### Comparing `LightZero-0.0.2/lzero/envs/get_wrapped_env.py` & `LightZero-0.0.5/lzero/envs/get_wrapped_env.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import gym
 from easydict import EasyDict
 
 from ding.envs import DingEnvWrapper
 from lzero.envs.wrappers import ActionDiscretizationEnvWrapper, LightZeroEnvWrapper
 
 
-def get_wrappered_env(wrapper_cfg: EasyDict, env_name: str):
+def get_wrappered_env(wrapper_cfg: EasyDict, env_id: str):
     """
     Overview:
         Returns a new environment with one or more wrappers applied to it.
     Arguments:
         - wrapper_cfg (:obj:`EasyDict`): A dictionary containing configuration settings for the wrappers.
-       -  env_name (:obj:`str`): The name of the environment to create.
+       -  env_id (:obj:`str`): The name of the environment to create.
     Returns:
         A callable that creates the wrapped environment.
     """
     if wrapper_cfg.manually_discretization:
         return lambda: DingEnvWrapper(
-            gym.make(env_name),
+            gym.make(env_id),
             cfg={
                 'env_wrapper': [
                     lambda env: ActionDiscretizationEnvWrapper(env, wrapper_cfg), lambda env:
                     LightZeroEnvWrapper(env, wrapper_cfg)
                 ]
             }
         )
     else:
         return lambda: DingEnvWrapper(
-            gym.make(env_name), cfg={'env_wrapper': [lambda env: LightZeroEnvWrapper(env, wrapper_cfg)]}
+            gym.make(env_id), cfg={'env_wrapper': [lambda env: LightZeroEnvWrapper(env, wrapper_cfg)]}
         )
```

### Comparing `LightZero-0.0.2/lzero/envs/tests/test_ding_env_wrapper.py` & `LightZero-0.0.5/lzero/envs/tests/test_ding_env_wrapper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from easydict import EasyDict
 import pytest
-import gym
+import gymnasium as gym
 import numpy as np
 
 from ding.envs import DingEnvWrapper
 
 
 @pytest.mark.unittest
 class TestDingEnvWrapper:
@@ -22,10 +22,10 @@
         l1 = ding_env.create_collector_env_cfg(cfg)
         assert isinstance(l1, list)
         l1 = ding_env.create_evaluator_env_cfg(cfg)
         assert isinstance(l1, list)
 
         obs = ding_env.reset()
 
-        assert isinstance(obs, np.ndarray)
+        assert isinstance(obs[0], np.ndarray)
         action = ding_env.random_action()
         print('random_action: {}, action_space: {}'.format(action.shape, ding_env.action_space))
```

### Comparing `LightZero-0.0.2/lzero/envs/tests/test_lightzero_env_wrapper.py` & `LightZero-0.0.5/lzero/envs/tests/test_lightzero_env_wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 
 @pytest.mark.unittest
 class TestLightZeroEnvWrapper:
 
     def test_continuous_pendulum(self):
         env_cfg = EasyDict(
             dict(
-                env_name='Pendulum-v1',
+                env_id='Pendulum-v1',
                 manually_discretization=False,
                 continuous=True,
                 each_dim_disc_size=None,
                 is_train=True,
             )
         )
 
         lightzero_env = DingEnvWrapper(
-            gym.make(env_cfg.env_name), cfg={'env_wrapper': [
+            gym.make(env_cfg.env_id), cfg={'env_wrapper': [
                 lambda env: LightZeroEnvWrapper(env, env_cfg),
             ]}
         )
 
         obs = lightzero_env.reset()
         print("obs: ", obs)
 
@@ -39,24 +39,24 @@
         action = lightzero_env.random_action()
 
         print('random_action: {}, action_space: {}'.format(action.shape, lightzero_env.action_space))
 
     def test_discretization_pendulum(self):
         env_cfg = EasyDict(
             dict(
-                env_name='Pendulum-v1',
+                env_id='Pendulum-v1',
                 manually_discretization=True,
                 continuous=False,
                 each_dim_disc_size=11,
                 is_train=True,
             )
         )
 
         lightzero_env = DingEnvWrapper(
-            gym.make(env_cfg.env_name),
+            gym.make(env_cfg.env_id),
             cfg={
                 'env_wrapper': [
                     lambda env: ActionDiscretizationEnvWrapper(env, env_cfg),
                     lambda env: LightZeroEnvWrapper(env, env_cfg),
                 ]
             }
         )
@@ -73,24 +73,24 @@
         action = lightzero_env.random_action()
 
         print('random_action: {}, action_space: {}'.format(action.shape, lightzero_env.action_space))
 
     def test_continuous_bipedalwalker(self):
         env_cfg = EasyDict(
             dict(
-                env_name='BipedalWalker-v3',
+                env_id='BipedalWalker-v3',
                 manually_discretization=False,
                 continuous=True,
                 each_dim_disc_size=4,
                 is_train=True,
             )
         )
 
         lightzero_env = DingEnvWrapper(
-            gym.make(env_cfg.env_name), cfg={'env_wrapper': [
+            gym.make(env_cfg.env_id), cfg={'env_wrapper': [
                 lambda env: LightZeroEnvWrapper(env, env_cfg),
             ]}
         )
 
         obs = lightzero_env.reset()
         print("obs: ", obs)
 
@@ -103,24 +103,24 @@
         action = lightzero_env.random_action()
 
         print('random_action: {}, action_space: {}'.format(action.shape, lightzero_env.action_space))
 
     def test_discretization_bipedalwalker(self):
         env_cfg = EasyDict(
             dict(
-                env_name='BipedalWalker-v3',
+                env_id='BipedalWalker-v3',
                 manually_discretization=True,
                 continuous=False,
                 each_dim_disc_size=4,
                 is_train=True,
             )
         )
 
         lightzero_env = DingEnvWrapper(
-            gym.make(env_cfg.env_name),
+            gym.make(env_cfg.env_id),
             cfg={
                 'env_wrapper': [
                     lambda env: ActionDiscretizationEnvWrapper(env, env_cfg),
                     lambda env: LightZeroEnvWrapper(env, env_cfg),
                 ]
             }
         )
```

### Comparing `LightZero-0.0.2/lzero/envs/wrappers/action_discretization_env_wrapper.py` & `LightZero-0.0.5/lzero/envs/wrappers/action_discretization_env_wrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         Arguments:
             - env (:obj:`gym.Env`): the environment to wrap.
         """
         super().__init__(env)
         assert 'is_train' in cfg, '`is_train` flag must set in the config of env'
         self.is_train = cfg.is_train
         self.cfg = cfg
-        self.env_name = cfg.env_name
+        self.env_id = cfg.env_id
         self.continuous = cfg.continuous
 
     def reset(self, **kwargs):
         """
         Overview:
             Resets the state of the environment and reset properties.
         Arguments:
```

### Comparing `LightZero-0.0.2/lzero/envs/wrappers/lightzero_env_wrapper.py` & `LightZero-0.0.5/lzero/envs/wrappers/lightzero_env_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         Arguments:
             - env (:obj:`gym.Env`): the environment to wrap.
         """
         super().__init__(env)
         assert 'is_train' in cfg, '`is_train` flag must set in the config of env'
         self.is_train = cfg.is_train
         self.cfg = cfg
-        self.env_name = cfg.env_name
+        self.env_id = cfg.env_id
         self.continuous = cfg.continuous
 
     def reset(self, **kwargs):
         """
         Overview:
             Resets the state of the environment and reset properties.
         Arguments:
```

### Comparing `LightZero-0.0.2/lzero/mcts/buffer/game_buffer.py` & `LightZero-0.0.5/lzero/mcts/buffer/game_buffer.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         reanalyze_ratio=0.3,
         # (bool) Whether to consider outdated experiences for reanalyzing. If True, we first sort the data in the minibatch by the time it was produced
         # and only reanalyze the oldest ``reanalyze_ratio`` fraction.
         reanalyze_outdated=True,
         # (bool) Whether to use the root value in the reanalyzing part. Please refer to EfficientZero paper for details.
         use_root_value=False,
         # (int) The number of samples required for mini inference.
-        mini_infer_size=256,
+        mini_infer_size=10240,
     )
 
     def __init__(self, cfg: dict):
         super().__init__()
         """
         Overview:
             Use the default configuration mechanism. If a user passes in a cfg with a key that matches an existing key
@@ -49,14 +49,16 @@
             the default configuration will be used.
         """
         default_config = self.default_config()
         default_config.update(cfg)
         self._cfg = default_config
         self._cfg = cfg
         assert self._cfg.env_type in ['not_board_games', 'board_games']
+        assert self._cfg.action_type in ['fixed_action_space', 'varied_action_space']
+
         self.replay_buffer_size = self._cfg.replay_buffer_size
         self.batch_size = self._cfg.batch_size
         self._alpha = self._cfg.priority_prob_alpha
         self._beta = self._cfg.priority_prob_beta
 
         self.game_segment_buffer = []
         self.game_pos_priorities = []
```

### Comparing `LightZero-0.0.2/lzero/mcts/buffer/game_buffer_efficientzero.py` & `LightZero-0.0.5/lzero/mcts/buffer/game_buffer_efficientzero.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,15 @@
             in the default configuration, the user-provided value will override the default configuration. Otherwise,
             the default configuration will be used.
         """
         default_config = self.default_config()
         default_config.update(cfg)
         self._cfg = default_config
         assert self._cfg.env_type in ['not_board_games', 'board_games']
+        assert self._cfg.action_type in ['fixed_action_space', 'varied_action_space']
         self.replay_buffer_size = self._cfg.replay_buffer_size
         self.batch_size = self._cfg.batch_size
         self._alpha = self._cfg.priority_prob_alpha
         self._beta = self._cfg.priority_prob_beta
 
         self.game_segment_buffer = []
         self.game_pos_priorities = []
@@ -230,21 +231,27 @@
                 noises = [
                     np.random.dirichlet([self._cfg.root_dirichlet_alpha] * self._cfg.model.action_space_size
                                         ).astype(np.float32).tolist() for _ in range(transition_batch_size)
                 ]
                 if self._cfg.mcts_ctree:
                     # cpp mcts_tree
                     roots = MCTSCtree.roots(transition_batch_size, legal_actions)
-                    roots.prepare(self._cfg.root_noise_weight, noises, value_prefix_pool, policy_logits_pool, to_play)
+                    if self._cfg.reanalyze_noise:
+                        roots.prepare(self._cfg.root_noise_weight, noises, value_prefix_pool, policy_logits_pool, to_play)
+                    else:
+                        roots.prepare_no_noise(value_prefix_pool, policy_logits_pool, to_play)
                     # do MCTS for a new policy with the recent target model
                     MCTSCtree(self._cfg).search(roots, model, latent_state_roots, reward_hidden_state_roots, to_play)
                 else:
                     # python mcts_tree
                     roots = MCTSPtree.roots(transition_batch_size, legal_actions)
-                    roots.prepare(self._cfg.root_noise_weight, noises, value_prefix_pool, policy_logits_pool, to_play)
+                    if self._cfg.reanalyze_noise:
+                        roots.prepare(self._cfg.root_noise_weight, noises, value_prefix_pool, policy_logits_pool, to_play)
+                    else:
+                        roots.prepare_no_noise(value_prefix_pool, policy_logits_pool, to_play)
                     # do MCTS for a new policy with the recent target model
                     MCTSPtree(self._cfg).search(
                         roots, model, latent_state_roots, reward_hidden_state_roots, to_play=to_play
                     )
                 roots_values = roots.get_values()
                 value_list = np.array(roots_values)
             else:
@@ -321,15 +328,15 @@
         Returns:
             - batch_target_policies_re
         """
         if policy_re_context is None:
             return []
         batch_target_policies_re = []
 
-        policy_obs_list, policy_mask, pos_in_game_segment_list, batch_index_list, child_visits, game_segment_lens, action_mask_segment, \
+        policy_obs_list, policy_mask, pos_in_game_segment_list, batch_index_list, child_visits, root_values, game_segment_lens, action_mask_segment, \
         to_play_segment = policy_re_context  # noqa
         # transition_batch_size = game_segment_batch_size * (self._cfg.num_unroll_steps + 1)
         transition_batch_size = len(policy_obs_list)
         game_segment_batch_size = len(pos_in_game_segment_list)
         to_play, action_mask = self._preprocess_to_play_and_action_mask(
             game_segment_batch_size, to_play_segment, action_mask_segment, pos_in_game_segment_list
         )
@@ -364,68 +371,85 @@
                 network_output.append(m_output)
 
             _, value_prefix_pool, policy_logits_pool, latent_state_roots, reward_hidden_state_roots = concat_output(
                 network_output, data_type='efficientzero'
             )
             value_prefix_pool = value_prefix_pool.squeeze().tolist()
             policy_logits_pool = policy_logits_pool.tolist()
+            # noises are not necessary for reanalyze
             noises = [
                 np.random.dirichlet([self._cfg.root_dirichlet_alpha] * self._cfg.model.action_space_size
                                     ).astype(np.float32).tolist() for _ in range(transition_batch_size)
             ]
             if self._cfg.mcts_ctree:
                 # cpp mcts_tree
                 roots = MCTSCtree.roots(transition_batch_size, legal_actions)
-                roots.prepare(self._cfg.root_noise_weight, noises, value_prefix_pool, policy_logits_pool, to_play)
+                if self._cfg.reanalyze_noise:
+                    roots.prepare(self._cfg.root_noise_weight, noises, value_prefix_pool, policy_logits_pool, to_play)
+                else:
+                    roots.prepare_no_noise(value_prefix_pool, policy_logits_pool, to_play)
                 # do MCTS for a new policy with the recent target model
                 MCTSCtree(self._cfg).search(roots, model, latent_state_roots, reward_hidden_state_roots, to_play)
             else:
                 # python mcts_tree
                 roots = MCTSPtree.roots(transition_batch_size, legal_actions)
-                roots.prepare(self._cfg.root_noise_weight, noises, value_prefix_pool, policy_logits_pool, to_play)
+                if self._cfg.reanalyze_noise:
+                    roots.prepare(self._cfg.root_noise_weight, noises, value_prefix_pool, policy_logits_pool, to_play)
+                else:
+                    roots.prepare_no_noise(value_prefix_pool, policy_logits_pool, to_play)
                 # do MCTS for a new policy with the recent target model
                 MCTSPtree(self._cfg).search(
                     roots, model, latent_state_roots, reward_hidden_state_roots, to_play=to_play
                 )
 
             roots_legal_actions_list = legal_actions
             roots_distributions = roots.get_distributions()
+            roots_values = roots.get_values()
             policy_index = 0
-            for state_index, game_index in zip(pos_in_game_segment_list, batch_index_list):
+            for state_index, child_visit, root_value in zip(pos_in_game_segment_list, child_visits, root_values):
                 target_policies = []
                 for current_index in range(state_index, state_index + self._cfg.num_unroll_steps + 1):
                     distributions = roots_distributions[policy_index]
+                    searched_value = roots_values[policy_index]
+
                     if policy_mask[policy_index] == 0:
-                        # NOTE: the invalid padding target policy, O is to make sure the correspoding cross_entropy_loss=0
+                        # NOTE: the invalid padding target policy, O is to make sure the corresponding cross_entropy_loss=0
                         target_policies.append([0 for _ in range(self._cfg.model.action_space_size)])
                     else:
                         if distributions is None:
                             # if at some obs, the legal_action is None, add the fake target_policy
                             target_policies.append(
                                 list(np.ones(self._cfg.model.action_space_size) / self._cfg.model.action_space_size)
                             )
                         else:
+                            # Update the data in game segment:
+                            # after the reanalyze search, new target policies and root values are obtained
+                            # the target policies and root values are stored in the gamesegment, specifically, ``child_visit_segment`` and ``root_value_segment``
+                            # we replace the data at the corresponding location with the latest search results to keep the most up-to-date targets
+                            sim_num = sum(distributions)
+                            child_visit[current_index] = [visit_count/sim_num for visit_count in distributions]
+                            root_value[current_index] = searched_value
                             if self._cfg.mcts_ctree:
                                 # cpp mcts_tree
-                                if self._cfg.env_type == 'not_board_games':
+                                if self._cfg.action_type == 'fixed_action_space':
                                     sum_visits = sum(distributions)
                                     policy = [visit_count / sum_visits for visit_count in distributions]
                                     target_policies.append(policy)
                                 else:
                                     # for two_player board games
                                     policy_tmp = [0 for _ in range(self._cfg.model.action_space_size)]
                                     # to make sure target_policies have the same dimension
                                     sum_visits = sum(distributions)
                                     policy = [visit_count / sum_visits for visit_count in distributions]
                                     for index, legal_action in enumerate(roots_legal_actions_list[policy_index]):
                                         policy_tmp[legal_action] = policy[index]
                                     target_policies.append(policy_tmp)
                             else:
                                 # python mcts_tree
-                                if self._cfg.env_type == 'not_board_games':
+                                if self._cfg.action_type == 'fixed_action_space':
                                     sum_visits = sum(distributions)
                                     policy = [visit_count / sum_visits for visit_count in distributions]
                                     target_policies.append(policy)
                                 else:
                                     # for two_player board games
                                     policy_tmp = [0 for _ in range(self._cfg.model.action_space_size)]
                                     # to make sure target_policies have the same dimension
```

### Comparing `LightZero-0.0.2/lzero/mcts/buffer/game_buffer_gumbel_muzero.py` & `LightZero-0.0.5/lzero/mcts/buffer/game_buffer_gumbel_muzero.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-from typing import Any, List, Tuple, Union, TYPE_CHECKING, Optional
+from typing import Any, Tuple
 
 import numpy as np
 from ding.utils import BUFFER_REGISTRY
 
-from lzero.mcts.utils import prepare_observation
 from lzero.mcts.buffer import MuZeroGameBuffer
+from lzero.mcts.utils import prepare_observation
+
 
 @BUFFER_REGISTRY.register('game_buffer_gumbel_muzero')
 class GumbelMuZeroGameBuffer(MuZeroGameBuffer):
     """
     Overview:
         The specific game buffer for Gumbel MuZero policy.
     """
@@ -40,50 +41,53 @@
         obs_list, action_list, improved_policy_list, mask_list = [], [], [], []
         # prepare the inputs of a batch
         for i in range(batch_size):
             game = game_segment_list[i]
             pos_in_game_segment = pos_in_game_segment_list[i]
 
             actions_tmp = game.action_segment[pos_in_game_segment:pos_in_game_segment +
-                                              self._cfg.num_unroll_steps].tolist()
-            
-            _improved_policy = game.improved_policy_probs[pos_in_game_segment:pos_in_game_segment + self._cfg.num_unroll_steps]
+                                                                  self._cfg.num_unroll_steps].tolist()
+
+            _improved_policy = game.improved_policy_probs[
+                               pos_in_game_segment:pos_in_game_segment + self._cfg.num_unroll_steps]
             if not isinstance(_improved_policy, list):
                 _improved_policy = _improved_policy.tolist()
 
             # add mask for invalid actions (out of trajectory)
             mask_tmp = [1. for i in range(len(actions_tmp))]
-            mask_tmp += [0. for _ in range(self._cfg.num_unroll_steps+1 - len(mask_tmp))]
+            mask_tmp += [0. for _ in range(self._cfg.num_unroll_steps + 1 - len(mask_tmp))]
 
             # pad random action
             actions_tmp += [
                 np.random.randint(0, game.action_space_size)
                 for _ in range(self._cfg.num_unroll_steps - len(actions_tmp))
             ]
 
-            # pad improved policy with with a value such that the sum of the values is equal to 1
-            _improved_policy.extend(np.random.dirichlet(np.ones(game.action_space_size),size=self._cfg.num_unroll_steps + 1 - len(_improved_policy)))
+            # pad improved policy with a value such that the sum of the values is equal to 1
+            _improved_policy.extend(np.random.dirichlet(np.ones(game.action_space_size),
+                                                        size=self._cfg.num_unroll_steps + 1 - len(_improved_policy)))
 
             # obtain the input observations
             # pad if length of obs in game_segment is less than stack+num_unroll_steps
-            # e.g. stack+num_unroll_steps  4+5
+            # e.g. stack+num_unroll_steps = 4+5
             obs_list.append(
                 game_segment_list[i].get_unroll_obs(
                     pos_in_game_segment_list[i], num_unroll_steps=self._cfg.num_unroll_steps, padding=True
                 )
             )
             action_list.append(actions_tmp)
             improved_policy_list.append(_improved_policy)
             mask_list.append(mask_tmp)
 
         # formalize the input observations
         obs_list = prepare_observation(obs_list, self._cfg.model.model_type)
 
         # formalize the inputs of a batch
-        current_batch = [obs_list, action_list, improved_policy_list, mask_list, batch_index_list, weights_list, make_time_list]
+        current_batch = [obs_list, action_list, improved_policy_list, mask_list, batch_index_list, weights_list,
+                         make_time_list]
         for i in range(len(current_batch)):
             current_batch[i] = np.asarray(current_batch[i])
 
         total_transitions = self.get_num_of_transitions()
 
         # obtain the context of value targets
         reward_value_context = self._prepare_reward_value_context(
@@ -112,8 +116,8 @@
                 batch_index_list[reanalyze_num:], game_segment_list[reanalyze_num:],
                 pos_in_game_segment_list[reanalyze_num:]
             )
         else:
             policy_non_re_context = None
 
         context = reward_value_context, policy_re_context, policy_non_re_context, current_batch
-        return context
+        return context
```

### Comparing `LightZero-0.0.2/lzero/mcts/buffer/game_buffer_muzero.py` & `LightZero-0.0.5/lzero/mcts/buffer/game_buffer_muzero.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
             in the default configuration, the user-provided value will override the default configuration. Otherwise,
             the default configuration will be used.
         """
         default_config = self.default_config()
         default_config.update(cfg)
         self._cfg = default_config
         assert self._cfg.env_type in ['not_board_games', 'board_games']
+        assert self._cfg.action_type in ['fixed_action_space', 'varied_action_space']
         self.replay_buffer_size = self._cfg.replay_buffer_size
         self.batch_size = self._cfg.batch_size
         self._alpha = self._cfg.priority_prob_alpha
         self._beta = self._cfg.priority_prob_beta
 
         self.keep_ratio = 1
         self.model_update_interval = 10
@@ -299,26 +300,27 @@
         zero_obs = game_segment_list[0].zero_obs()
         with torch.no_grad():
             # for policy
             policy_obs_list = []
             policy_mask = []
             # 0 -> Invalid target policy for padding outside of game segments,
             # 1 -> Previous target policy for game segments.
-            rewards, child_visits, game_segment_lens = [], [], []
+            rewards, child_visits, game_segment_lens, root_values = [], [], [], []
             # for board games
             action_mask_segment, to_play_segment = [], []
             for game_segment, state_index in zip(game_segment_list, pos_in_game_segment_list):
                 game_segment_len = len(game_segment)
                 game_segment_lens.append(game_segment_len)
                 rewards.append(game_segment.reward_segment)
                 # for board games
                 action_mask_segment.append(game_segment.action_mask_segment)
                 to_play_segment.append(game_segment.to_play_segment)
 
                 child_visits.append(game_segment.child_visit_segment)
+                root_values.append(game_segment.root_value_segment)
                 # prepare the corresponding observations
                 game_obs = game_segment.get_unroll_obs(state_index, self._cfg.num_unroll_steps)
                 for current_index in range(state_index, state_index + self._cfg.num_unroll_steps + 1):
 
                     if current_index < game_segment_len:
                         policy_mask.append(1)
                         beg_index = current_index - state_index
@@ -326,15 +328,15 @@
                         obs = game_obs[beg_index:end_index]
                     else:
                         policy_mask.append(0)
                         obs = zero_obs
                     policy_obs_list.append(obs)
 
         policy_re_context = [
-            policy_obs_list, policy_mask, pos_in_game_segment_list, batch_index_list, child_visits, game_segment_lens,
+            policy_obs_list, policy_mask, pos_in_game_segment_list, batch_index_list, child_visits, root_values, game_segment_lens,
             action_mask_segment, to_play_segment
         ]
         return policy_re_context
 
     def _compute_target_reward_value(self, reward_value_context: List[Any], model: Any) -> Tuple[Any, Any]:
         """
         Overview:
@@ -373,15 +375,15 @@
             # split a full batch into slices of mini_infer_size: to save the GPU memory for more GPU actors
             slices = int(np.ceil(transition_batch_size / self._cfg.mini_infer_size))
             network_output = []
             for i in range(slices):
                 beg_index = self._cfg.mini_infer_size * i
                 end_index = self._cfg.mini_infer_size * (i + 1)
 
-                m_obs = torch.from_numpy(value_obs_list[beg_index:end_index]).to(self._cfg.device).float()
+                m_obs = torch.from_numpy(value_obs_list[beg_index:end_index]).to(self._cfg.device)
 
                 # calculate the target value
                 m_output = model.initial_inference(m_obs)
 
                 if not model.training:
                     # if not in training, obtain the scalars of the value/reward
                     [m_output.latent_state, m_output.value, m_output.policy_logits] = to_detach_cpu_numpy(
@@ -392,35 +394,41 @@
                         ]
                     )
 
                 network_output.append(m_output)
 
             # concat the output slices after model inference
             if self._cfg.use_root_value:
-                # use the root values from MCTS, as in EfficiientZero
+                # use the root values from MCTS, as in EfficientZero
                 # the root values have limited improvement but require much more GPU actors;
                 _, reward_pool, policy_logits_pool, latent_state_roots = concat_output(
                     network_output, data_type='muzero'
                 )
                 reward_pool = reward_pool.squeeze().tolist()
                 policy_logits_pool = policy_logits_pool.tolist()
                 noises = [
                     np.random.dirichlet([self._cfg.root_dirichlet_alpha] * int(sum(action_mask[j]))
                                         ).astype(np.float32).tolist() for j in range(transition_batch_size)
                 ]
                 if self._cfg.mcts_ctree:
                     # cpp mcts_tree
                     roots = MCTSCtree.roots(transition_batch_size, legal_actions)
-                    roots.prepare(self._cfg.root_noise_weight, noises, reward_pool, policy_logits_pool, to_play)
+                    if self._cfg.reanalyze_noise:
+                        roots.prepare(self._cfg.root_noise_weight, noises, reward_pool, policy_logits_pool, to_play)
+                    else:
+                        roots.prepare_no_noise(reward_pool, policy_logits_pool, to_play)
                     # do MCTS for a new policy with the recent target model
                     MCTSCtree(self._cfg).search(roots, model, latent_state_roots, to_play)
                 else:
                     # python mcts_tree
                     roots = MCTSPtree.roots(transition_batch_size, legal_actions)
-                    roots.prepare(self._cfg.root_noise_weight, noises, reward_pool, policy_logits_pool, to_play)
+                    if self._cfg.reanalyze_noise:
+                        roots.prepare(self._cfg.root_noise_weight, noises, reward_pool, policy_logits_pool, to_play)
+                    else:
+                        roots.prepare_no_noise(reward_pool, policy_logits_pool, to_play)
                     # do MCTS for a new policy with the recent target model
                     MCTSPtree(self._cfg).search(roots, model, latent_state_roots, to_play)
 
                 roots_values = roots.get_values()
                 value_list = np.array(roots_values)
             else:
                 # use the predicted values
@@ -467,16 +475,14 @@
 
                     if current_index < game_segment_len_non_re:
                         target_values.append(value_list[value_index])
                         target_rewards.append(reward_list[current_index])
                     else:
                         target_values.append(0)
                         target_rewards.append(0.0)
-                        # TODO: check
-                        # target_rewards.append(reward)
                     value_index += 1
 
                 batch_rewards.append(target_rewards)
                 batch_target_values.append(target_values)
 
         batch_rewards = np.asarray(batch_rewards, dtype=object)
         batch_target_values = np.asarray(batch_target_values, dtype=object)
@@ -492,16 +498,16 @@
             - batch_target_policies_re
         """
         if policy_re_context is None:
             return []
         batch_target_policies_re = []
 
         # for board games
-        policy_obs_list, policy_mask, pos_in_game_segment_list, batch_index_list, child_visits, game_segment_lens, action_mask_segment, \
-        to_play_segment = policy_re_context  # noqa
+        policy_obs_list, policy_mask, pos_in_game_segment_list, batch_index_list, child_visits, root_values, game_segment_lens, action_mask_segment, \
+        to_play_segment = policy_re_context
         # transition_batch_size = game_segment_batch_size * (self._cfg.num_unroll_steps + 1)
         transition_batch_size = len(policy_obs_list)
         game_segment_batch_size = len(pos_in_game_segment_list)
 
         to_play, action_mask = self._preprocess_to_play_and_action_mask(
             game_segment_batch_size, to_play_segment, action_mask_segment, pos_in_game_segment_list
         )
@@ -522,15 +528,15 @@
             policy_obs_list = prepare_observation(policy_obs_list, self._cfg.model.model_type)
             # split a full batch into slices of mini_infer_size: to save the GPU memory for more GPU actors
             slices = int(np.ceil(transition_batch_size / self._cfg.mini_infer_size))
             network_output = []
             for i in range(slices):
                 beg_index = self._cfg.mini_infer_size * i
                 end_index = self._cfg.mini_infer_size * (i + 1)
-                m_obs = torch.from_numpy(policy_obs_list[beg_index:end_index]).to(self._cfg.device).float()
+                m_obs = torch.from_numpy(policy_obs_list[beg_index:end_index]).to(self._cfg.device)
                 m_output = model.initial_inference(m_obs)
                 if not model.training:
                     # if not in training, obtain the scalars of the value/reward
                     [m_output.latent_state, m_output.value, m_output.policy_logits] = to_detach_cpu_numpy(
                         [
                             m_output.latent_state,
                             inverse_scalar_transform(m_output.value, self._cfg.model.support_scale),
@@ -539,51 +545,67 @@
                     )
 
                 network_output.append(m_output)
 
             _, reward_pool, policy_logits_pool, latent_state_roots = concat_output(network_output, data_type='muzero')
             reward_pool = reward_pool.squeeze().tolist()
             policy_logits_pool = policy_logits_pool.tolist()
+            # noises are not necessary for reanalyze
             noises = [
                 np.random.dirichlet([self._cfg.root_dirichlet_alpha] * self._cfg.model.action_space_size
                                     ).astype(np.float32).tolist() for _ in range(transition_batch_size)
             ]
             if self._cfg.mcts_ctree:
                 # cpp mcts_tree
                 roots = MCTSCtree.roots(transition_batch_size, legal_actions)
-                roots.prepare(self._cfg.root_noise_weight, noises, reward_pool, policy_logits_pool, to_play)
+                if self._cfg.reanalyze_noise:
+                    roots.prepare(self._cfg.root_noise_weight, noises, reward_pool, policy_logits_pool, to_play)
+                else:
+                    roots.prepare_no_noise(reward_pool, policy_logits_pool, to_play)
                 # do MCTS for a new policy with the recent target model
                 MCTSCtree(self._cfg).search(roots, model, latent_state_roots, to_play)
             else:
                 # python mcts_tree
                 roots = MCTSPtree.roots(transition_batch_size, legal_actions)
-                roots.prepare(self._cfg.root_noise_weight, noises, reward_pool, policy_logits_pool, to_play)
+                if self._cfg.reanalyze_noise:
+                    roots.prepare(self._cfg.root_noise_weight, noises, reward_pool, policy_logits_pool, to_play)
+                else:
+                    roots.prepare_no_noise(reward_pool, policy_logits_pool, to_play)
                 # do MCTS for a new policy with the recent target model
                 MCTSPtree(self._cfg).search(roots, model, latent_state_roots, to_play)
 
             roots_legal_actions_list = legal_actions
             roots_distributions = roots.get_distributions()
+            roots_values = roots.get_values()
             policy_index = 0
-            for state_index, game_index in zip(pos_in_game_segment_list, batch_index_list):
+            for state_index, child_visit, root_value in zip(pos_in_game_segment_list, child_visits, root_values):
                 target_policies = []
 
                 for current_index in range(state_index, state_index + self._cfg.num_unroll_steps + 1):
                     distributions = roots_distributions[policy_index]
+                    searched_value = roots_values[policy_index]
 
                     if policy_mask[policy_index] == 0:
                         # NOTE: the invalid padding target policy, O is to make sure the corresponding cross_entropy_loss=0
                         target_policies.append([0 for _ in range(self._cfg.model.action_space_size)])
                     else:
                         if distributions is None:
                             # if at some obs, the legal_action is None, add the fake target_policy
                             target_policies.append(
                                 list(np.ones(self._cfg.model.action_space_size) / self._cfg.model.action_space_size)
                             )
                         else:
-                            if self._cfg.env_type == 'not_board_games':
+                            # Update the data in game segment:
+                            # after the reanalyze search, new target policies and root values are obtained
+                            # the target policies and root values are stored in the gamesegment, specifically, ``child_visit_segment`` and ``root_value_segment``
+                            # we replace the data at the corresponding location with the latest search results to keep the most up-to-date targets
+                            sim_num = sum(distributions)
+                            child_visit[current_index] = [visit_count/sim_num for visit_count in distributions]
+                            root_value[current_index] = searched_value
+                            if self._cfg.action_type == 'fixed_action_space':
                                 # for atari/classic_control/box2d environments that only have one player.
                                 sum_visits = sum(distributions)
                                 policy = [visit_count / sum_visits for visit_count in distributions]
                                 target_policies.append(policy)
                             else:
                                 # for board games that have two players and legal_actions is dy
                                 policy_tmp = [0 for _ in range(self._cfg.model.action_space_size)]
@@ -653,15 +675,15 @@
                 target_policies = []
 
                 for current_index in range(state_index, state_index + self._cfg.num_unroll_steps + 1):
                     if current_index < game_segment_len:
                         policy_mask.append(1)
                         # NOTE: child_visit is already a distribution
                         distributions = child_visit[current_index]
-                        if self._cfg.env_type == 'not_board_games':
+                        if self._cfg.action_type == 'fixed_action_space':
                             # for atari/classic_control/box2d environments that only have one player.
                             target_policies.append(distributions)
                         else:
                             # for board games that have two players.
                             policy_tmp = [0 for _ in range(policy_shape)]
                             for index, legal_action in enumerate(legal_actions[policy_index]):
                                 # only the action in ``legal_action`` the policy logits is nonzero
```

### Comparing `LightZero-0.0.2/lzero/mcts/buffer/game_buffer_sampled_efficientzero.py` & `LightZero-0.0.5/lzero/mcts/buffer/game_buffer_sampled_efficientzero.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
             in the default configuration, the user-provided value will override the default configuration. Otherwise,
             the default configuration will be used.
         """
         default_config = self.default_config()
         default_config.update(cfg)
         self._cfg = default_config
         assert self._cfg.env_type in ['not_board_games', 'board_games']
+        assert self._cfg.action_type in ['fixed_action_space', 'varied_action_space']
         self.replay_buffer_size = self._cfg.replay_buffer_size
         self.batch_size = self._cfg.batch_size
         self._alpha = self._cfg.priority_prob_alpha
         self._beta = self._cfg.priority_prob_beta
 
         self.game_segment_buffer = []
         self.game_pos_priorities = []
@@ -319,25 +320,30 @@
                 if self._cfg.mcts_ctree:
                     # cpp mcts_tree
                     # prepare the root nodes for MCTS
                     roots = MCTSCtree.roots(
                         transition_batch_size, legal_actions, self._cfg.model.action_space_size,
                         self._cfg.model.num_of_sampled_actions, self._cfg.model.continuous_action_space
                     )
-
-                    roots.prepare(self._cfg.root_noise_weight, noises, value_prefix_pool, policy_logits_pool, to_play)
+                    if self._cfg.reanalyze_noise:
+                        roots.prepare(self._cfg.root_noise_weight, noises, value_prefix_pool, policy_logits_pool, to_play)
+                    else:
+                        roots.prepare_no_noise(value_prefix_pool, policy_logits_pool, to_play)
                     # do MCTS for a new policy with the recent target model
                     MCTSCtree(self._cfg).search(roots, model, latent_state_roots, reward_hidden_state_roots, to_play)
                 else:
                     # python mcts_tree
                     roots = MCTSPtree.roots(
                         transition_batch_size, legal_actions, self._cfg.model.action_space_size,
                         self._cfg.model.num_of_sampled_actions, self._cfg.model.continuous_action_space
                     )
-                    roots.prepare(self._cfg.root_noise_weight, noises, value_prefix_pool, policy_logits_pool, to_play)
+                    if self._cfg.reanalyze_noise:
+                        roots.prepare(self._cfg.root_noise_weight, noises, value_prefix_pool, policy_logits_pool, to_play)
+                    else:
+                        roots.prepare_no_noise(value_prefix_pool, policy_logits_pool, to_play)
                     # do MCTS for a new policy with the recent target model
                     MCTSPtree.roots(self._cfg
                                     ).search(roots, model, latent_state_roots, reward_hidden_state_roots, to_play)
 
                 roots_values = roots.get_values()
                 value_list = np.array(roots_values)
             else:
@@ -421,15 +427,15 @@
         Returns:
             - batch_target_policies_re
         """
         if policy_re_context is None:
             return []
         batch_target_policies_re = []
 
-        policy_obs_list, policy_mask, pos_in_game_segment_list, batch_index_list, child_visits, game_segment_lens, action_mask_segment, \
+        policy_obs_list, policy_mask, pos_in_game_segment_list, batch_index_list, child_visits, root_values, game_segment_lens, action_mask_segment, \
         to_play_segment = policy_re_context  # noqa
         # transition_batch_size = game_segment_batch_size * (self._cfg.num_unroll_steps + 1)
         transition_batch_size = len(policy_obs_list)
         game_segment_batch_size = len(pos_in_game_segment_list)
 
         to_play, action_mask = self._preprocess_to_play_and_action_mask(
             game_segment_batch_size, to_play_segment, action_mask_segment, pos_in_game_segment_list
@@ -477,74 +483,90 @@
 
             _, value_prefix_pool, policy_logits_pool, latent_state_roots, reward_hidden_state_roots = concat_output(
                 network_output, data_type='efficientzero'
             )
 
             value_prefix_pool = value_prefix_pool.squeeze().tolist()
             policy_logits_pool = policy_logits_pool.tolist()
+            # noises are not necessary for reanalyze
             noises = [
                 np.random.dirichlet([self._cfg.root_dirichlet_alpha] * self._cfg.model.num_of_sampled_actions
                                     ).astype(np.float32).tolist() for _ in range(transition_batch_size)
             ]
             if self._cfg.mcts_ctree:
                 # ==============================================================
                 # sampled related core code
                 # ==============================================================
                 # cpp mcts_tree
                 roots = MCTSCtree.roots(
                     transition_batch_size, legal_actions, self._cfg.model.action_space_size,
                     self._cfg.model.num_of_sampled_actions, self._cfg.model.continuous_action_space
                 )
-                roots.prepare(self._cfg.root_noise_weight, noises, value_prefix_pool, policy_logits_pool, to_play)
+                if self._cfg.reanalyze_noise:
+                    roots.prepare(self._cfg.root_noise_weight, noises, value_prefix_pool, policy_logits_pool, to_play)
+                else:
+                    roots.prepare_no_noise(value_prefix_pool, policy_logits_pool, to_play)
                 # do MCTS for a new policy with the recent target model
                 MCTSCtree(self._cfg).search(roots, model, latent_state_roots, reward_hidden_state_roots, to_play)
             else:
                 # python mcts_tree
                 roots = MCTSPtree.roots(
                     transition_batch_size, legal_actions, self._cfg.model.action_space_size,
                     self._cfg.model.num_of_sampled_actions, self._cfg.model.continuous_action_space
                 )
-                roots.prepare(self._cfg.root_noise_weight, noises, value_prefix_pool, policy_logits_pool, to_play)
+                if self._cfg.reanalyze_noise:
+                    roots.prepare(self._cfg.root_noise_weight, noises, value_prefix_pool, policy_logits_pool, to_play)
+                else:
+                    roots.prepare_no_noise(value_prefix_pool, policy_logits_pool, to_play)
                 # do MCTS for a new policy with the recent target model
                 MCTSPtree.roots(self._cfg).search(roots, model, latent_state_roots, reward_hidden_state_roots, to_play)
 
             roots_legal_actions_list = legal_actions
             roots_distributions = roots.get_distributions()
+            roots_values = roots.get_values()
 
             # ==============================================================
             # fix reanalyze in sez
             # ==============================================================
             roots_sampled_actions = roots.get_sampled_actions()
             try:
                 root_sampled_actions = np.array([action.value for action in roots_sampled_actions])
             except Exception:
                 root_sampled_actions = np.array([action for action in roots_sampled_actions])
-
+            
             policy_index = 0
-            for state_index, game_idx in zip(pos_in_game_segment_list, batch_index_list):
+            for state_index, child_visit, root_value in zip(pos_in_game_segment_list, child_visits, root_values):
                 target_policies = []
                 for current_index in range(state_index, state_index + self._cfg.num_unroll_steps + 1):
                     distributions = roots_distributions[policy_index]
+                    searched_value = roots_values[policy_index]
                     # ==============================================================
                     # sampled related core code
                     # ==============================================================
                     if policy_mask[policy_index] == 0:
-                        # NOTE: the invalid padding target policy, O is to make sure the correspoding cross_entropy_loss=0
+                        # NOTE: the invalid padding target policy, O is to make sure the corresponding cross_entropy_loss=0
                         target_policies.append([0 for _ in range(self._cfg.model.num_of_sampled_actions)])
                     else:
                         if distributions is None:
                             # if at some obs, the legal_action is None, then add the fake target_policy
                             target_policies.append(
                                 list(
                                     np.ones(self._cfg.model.num_of_sampled_actions) /
                                     self._cfg.model.num_of_sampled_actions
                                 )
                             )
                         else:
-                            if self._cfg.env_type == 'not_board_games':
+                            # Update the data in game segment:
+                            # after the reanalyze search, new target policies and root values are obtained
+                            # the target policies and root values are stored in the gamesegment, specifically, ``child_visit_segment`` and ``root_value_segment``
+                            # we replace the data at the corresponding location with the latest search results to keep the most up-to-date targets
+                            sim_num = sum(distributions)
+                            child_visit[current_index] = [visit_count/sim_num for visit_count in distributions]
+                            root_value[current_index] = searched_value
+                            if self._cfg.action_type == 'fixed_action_space':
                                 sum_visits = sum(distributions)
                                 policy = [visit_count / sum_visits for visit_count in distributions]
                                 target_policies.append(policy)
                             else:
                                 # for two_player board games
                                 policy_tmp = [0 for _ in range(self._cfg.model.num_of_sampled_actions)]
                                 # to make sure target_policies have the same dimension
```

### Comparing `LightZero-0.0.2/lzero/mcts/buffer/game_buffer_stochastic_muzero.py` & `LightZero-0.0.5/lzero/mcts/buffer/game_buffer_stochastic_muzero.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
             in the default configuration, the user-provided value will override the default configuration. Otherwise,
             the default configuration will be used.
         """
         default_config = self.default_config()
         default_config.update(cfg)
         self._cfg = default_config
         assert self._cfg.env_type in ['not_board_games', 'board_games']
+        assert self._cfg.action_type in ['fixed_action_space', 'varied_action_space']
         self.replay_buffer_size = self._cfg.replay_buffer_size
         self.batch_size = self._cfg.batch_size
         self._alpha = self._cfg.priority_prob_alpha
         self._beta = self._cfg.priority_prob_beta
 
         self.keep_ratio = 1
         self.model_update_interval = 10
```

### Comparing `LightZero-0.0.2/lzero/mcts/buffer/game_segment.py` & `LightZero-0.0.5/lzero/mcts/buffer/game_segment.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,17 +53,15 @@
         self.use_ture_chance_label_in_chance_encoder = config.use_ture_chance_label_in_chance_encoder
 
         if isinstance(config.model.observation_shape, int) or len(config.model.observation_shape) == 1:
             # for vector obs input, e.g. classical control and box2d environments
             self.zero_obs_shape = config.model.observation_shape
         elif len(config.model.observation_shape) == 3:
             # image obs input, e.g. atari environments
-            self.zero_obs_shape = (
-                config.model.observation_shape[-2], config.model.observation_shape[-1], config.model.image_channel
-            )
+            self.zero_obs_shape = (config.model.image_channel, config.model.observation_shape[-2], config.model.observation_shape[-1])
 
         self.obs_segment = []
         self.action_segment = []
         self.reward_segment = []
 
         self.child_visit_segment = []
         self.root_value_segment = []
@@ -78,15 +76,14 @@
         self.improved_policy_probs = []
 
         if self.sampled_algo:
             self.root_sampled_actions = []
         if self.use_ture_chance_label_in_chance_encoder:
             self.chance_segment = []
 
-
     def get_unroll_obs(self, timestep: int, num_unroll_steps: int = 0, padding: bool = False) -> np.ndarray:
         """
         Overview:
             Get an observation of the correct format: o[t, t + stack frames + num_unroll_steps].
         Arguments:
             - timestep (int): The time step.
             - num_unroll_steps (int): The extra length of the observation frames.
```

### Comparing `LightZero-0.0.2/lzero/mcts/ctree/common_lib/cminimax.cpp` & `LightZero-0.0.5/lzero/mcts/ctree/common_lib/cminimax.cpp`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/lzero/mcts/ctree/common_lib/cminimax.h` & `LightZero-0.0.5/lzero/mcts/ctree/common_lib/cminimax.h`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/lzero/mcts/ctree/ctree_efficientzero/lib/cnode.cpp` & `LightZero-0.0.5/lzero/mcts/ctree/ctree_efficientzero/lib/cnode.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -207,19 +207,14 @@
         else
         {
             mean_q = (parent_q + total_unsigned_q) / (total_visits + 1);
         }
         return mean_q;
     }
 
-    void CNode::print_out()
-    {
-        return;
-    }
-
     int CNode::expanded()
     {
         /*
         Overview:
             Return whether the current node is expanded.
         */
         return this->children.size() > 0;
@@ -244,15 +239,15 @@
     }
 
     std::vector<int> CNode::get_trajectory()
     {
         /*
         Overview:
             Find the current best trajectory starts from the current node.
-        Outputs:
+        Returns:
             - traj: a vector of node index, which is the current best trajectory from this node.
         */
         std::vector<int> traj;
 
         CNode *node = this;
         int best_action = node->best_action;
         while (best_action >= 0)
@@ -266,15 +261,15 @@
     }
 
     std::vector<int> CNode::get_children_distribution()
     {
         /*
         Overview:
             Get the distribution of child nodes in the format of visit_count.
-        Outputs:
+        Returns:
             - distribution: a vector of distribution of child nodes in the format of visit count (i.e. [1,3,0,2,5]).
         */
         std::vector<int> distribution;
         if (this->expanded())
         {
             for (auto a : this->legal_actions)
             {
@@ -374,15 +369,15 @@
     }
 
     std::vector<std::vector<int> > CRoots::get_trajectories()
     {
         /*
         Overview:
             Find the current best trajectory starts from each root.
-        Outputs:
+        Returns:
             - traj: a vector of node index, which is the current best trajectory from each root.
         */
         std::vector<std::vector<int> > trajs;
         trajs.reserve(this->root_num);
 
         for (int i = 0; i < this->root_num; ++i)
         {
@@ -392,15 +387,15 @@
     }
 
     std::vector<std::vector<int> > CRoots::get_distributions()
     {
         /*
         Overview:
             Get the children distribution of each root.
-        Outputs:
+        Returns:
             - distribution: a vector of distribution of child nodes in the format of visit count (i.e. [1,3,0,2,5]).
         */
         std::vector<std::vector<int> > distributions;
         distributions.reserve(this->root_num);
 
         for (int i = 0; i < this->root_num; ++i)
         {
@@ -614,15 +609,15 @@
             - root: the roots to select the child node.
             - min_max_stats: a tool used to min-max normalize the score.
             - pb_c_base: constants c2 in muzero.
             - pb_c_init: constants c1 in muzero.
             - disount_factor: the discount factor of reward.
             - mean_q: the mean q value of the parent node.
             - players: the number of players.
-        Outputs:
+        Returns:
             - action: the action to select.
         */
         float max_score = FLOAT_MIN;
         const float epsilon = 0.000001;
         std::vector<int> max_index_lst;
         for (auto a : root->legal_actions)
         {
@@ -663,15 +658,15 @@
             - is_reset: whether the value prefix needs to be reset.
             - total_children_visit_counts: the total visit counts of the child nodes of the parent node.
             - parent_value_prefix: the value prefix of parent node.
             - pb_c_base: constants c2 in muzero.
             - pb_c_init: constants c1 in muzero.
             - disount_factor: the discount factor of reward.
             - players: the number of players.
-        Outputs:
+        Returns:
             - ucb_value: the ucb score of the child.
         */
         float pb_c = 0.0, prior_score = 0.0, value_score = 0.0;
         pb_c = log((total_children_visit_counts + pb_c_base + 1) / pb_c_base) + pb_c_init;
         pb_c *= (sqrt(total_children_visit_counts) / (child->visit_count + 1));
 
         prior_score = pb_c * child->prior;
```

### Comparing `LightZero-0.0.2/lzero/mcts/ctree/ctree_efficientzero/lib/cnode.h` & `LightZero-0.0.5/lzero/mcts/ctree/ctree_efficientzero/lib/cnode.h`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/lzero/mcts/ctree/ctree_gumbel_muzero/lib/cnode.cpp` & `LightZero-0.0.5/lzero/mcts/ctree/ctree_gumbel_muzero/lib/cnode.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -261,15 +261,15 @@
     }
 
     std::vector<int> CNode::get_trajectory()
     {
         /*
         Overview:
             Find the current best trajectory starts from the current node.
-        Outputs:
+        Returns:
             - traj: a vector of node index, which is the current best trajectory from this node.
         */
         std::vector<int> traj;
 
         CNode *node = this;
         int best_action = node->best_action;
         while (best_action >= 0)
@@ -283,15 +283,15 @@
     }
 
     std::vector<int> CNode::get_children_distribution()
     {
         /*
         Overview:
             Get the distribution of child nodes in the format of visit_count.
-        Outputs:
+        Returns:
             - distribution: a vector of distribution of child nodes in the format of visit count (i.e. [1,3,0,2,5]).
         */
         std::vector<int> distribution;
         if (this->expanded())
         {
             for (auto a : this->legal_actions)
             {
@@ -307,15 +307,15 @@
     //*********************************************************
 
     std::vector<float> CNode::get_children_value(float discount_factor, int action_space_size)
     {
         /*
         Overview:
             Get the completed value of child nodes.
-        Outputs:
+        Returns:
             - discount_factor: the discount_factor of reward.
             - action_space_size: the size of action space.
         */
         float infymin = -std::numeric_limits<float>::infinity();
         std::vector<int> child_visit_count;
         std::vector<float> child_prior;
         for(auto a: this->legal_actions){
@@ -464,15 +464,15 @@
     }
 
     std::vector<std::vector<int> > CRoots::get_trajectories()
     {
         /*
         Overview:
             Find the current best trajectory starts from each root.
-        Outputs:
+        Returns:
             - traj: a vector of node index, which is the current best trajectory from each root.
         */
         std::vector<std::vector<int> > trajs;
         trajs.reserve(this->root_num);
 
         for (int i = 0; i < this->root_num; ++i)
         {
@@ -482,15 +482,15 @@
     }
 
     std::vector<std::vector<int> > CRoots::get_distributions()
     {
         /*
         Overview:
             Get the children distribution of each root.
-        Outputs:
+        Returns:
             - distribution: a vector of distribution of child nodes in the format of visit count (i.e. [1,3,0,2,5]).
         */
         std::vector<std::vector<int> > distributions;
         distributions.reserve(this->root_num);
 
         for (int i = 0; i < this->root_num; ++i)
         {
@@ -660,15 +660,15 @@
             - root: the roots to select the child node.
             - min_max_stats: a tool used to min-max normalize the score.
             - pb_c_base: constants c2 in muzero.
             - pb_c_init: constants c1 in muzero.
             - disount_factor: the discount factor of reward.
             - mean_q: the mean q value of the parent node.
             - players: the number of players.
-        Outputs:
+        Returns:
             - action: the action to select.
         */
         float max_score = FLOAT_MIN;
         const float epsilon = 0.000001;
         std::vector<int> max_index_lst;
         for(auto a: root->legal_actions){
 
@@ -704,15 +704,15 @@
         Overview:
             Select the child node of the roots in gumbel muzero.
         Arguments:
             - root: the roots to select the child node.
             - disount_factor: the discount factor of reward.
             - num_simulations: the upper limit number of simulations.
             - max_num_considered_actions: the maximum number of considered actions.
-        Outputs:
+        Returns:
             - action: the action to select.
         */
         std::vector<int> child_visit_count;
         std::vector<float> child_prior;
         for(auto a: root->legal_actions){
             CNode* child = root->get_child(a);
             child_visit_count.push_back(child->visit_count);
@@ -748,15 +748,15 @@
     {
         /*
         Overview:
             Select the child node of the interior node in gumbel muzero.
         Arguments:
             - root: the roots to select the child node.
             - disount_factor: the discount factor of reward.
-        Outputs:
+        Returns:
             - action: the action to select.
         */
         std::vector<int> child_visit_count;
         std::vector<float> child_prior;
         for(auto a: root->legal_actions){
             CNode* child = root->get_child(a);
             child_visit_count.push_back(child->visit_count);
@@ -799,15 +799,15 @@
             - min_max_stats: a tool used to min-max normalize the score.
             - mean_q: the mean q value of the parent node.
             - total_children_visit_counts: the total visit counts of the child nodes of the parent node.
             - pb_c_base: constants c2 in muzero.
             - pb_c_init: constants c1 in muzero.
             - disount_factor: the discount factor of reward.
             - players: the number of players.
-        Outputs:
+        Returns:
             - ucb_value: the ucb score of the child.
         */
         float pb_c = 0.0, prior_score = 0.0, value_score = 0.0;
         pb_c = log((total_children_visit_counts + pb_c_base + 1) / pb_c_base) + pb_c_init;
         pb_c *= (sqrt(total_children_visit_counts) / (child->visit_count + 1));
 
         prior_score = pb_c * child->prior;
@@ -938,15 +938,15 @@
         Overview:
             Compute the mixed Q value.
         Arguments:
             - raw_value: the approximated value of the current node from the value network.
             - q_value: the q value of the current node.
             - child_visit: the visit counts of the child nodes.
             - child_prior: the prior of the child nodes.
-        Outputs:
+        Returns:
             - mixed Q value.
         */
         float visit_count_sum = 0.0;
         float probs_sum = 0.0;
         float weighted_q_sum = 0.0;
         float min_num = -10e7;
 
@@ -998,15 +998,15 @@
             - child_visit: the visit counts of the child nodes.
             - child_prior: the prior of the child nodes.
             - discount_factor: the discount factor of reward.
             - maxvisit_init: the init of the maximization of visit counts.
             - value_cale: the scale of value.
             - rescale_values: whether to rescale the values.
             - epsilon: the lower limit of gap in max-min normalization
-        Outputs:
+        Returns:
             - completed Q value.
         */
         assert (child_visit.size() == child_prior.size());
         std::vector<float> qvalues;
         std::vector<float> child_prior_tmp;
 
         child_prior_tmp.assign(child_prior.begin(), child_prior.end());
@@ -1043,15 +1043,15 @@
     {
         /*
         Overview:
             Calculate the considered visit sequence.
         Arguments:
             - max_num_considered_actions: the maximum number of considered actions.
             - num_simulations: the upper limit number of simulations.
-        Outputs:
+        Returns:
             - the considered visit sequence.
         */
         std::vector<int> visit_seq;
         if(max_num_considered_actions <= 1){
             for (int i=0;i < num_simulations;i++)
                 visit_seq.push_back(i);
             return visit_seq;
@@ -1080,15 +1080,15 @@
     {
         /*
         Overview:
             Calculate the table of considered visits.
         Arguments:
             - max_num_considered_actions: the maximum number of considered actions.
             - num_simulations: the upper limit number of simulations.
-        Outputs:
+        Returns:
             - the table of considered visits.
         */
         std::vector<std::vector<int> > table;
         for (int m=0;m < max_num_considered_actions+1;m++){
             table.push_back(get_sequence_of_considered_visits(m, num_simulations));
         }
         return table;
@@ -1101,15 +1101,15 @@
             Calculate the score of nodes to be considered according to the considered visit.
         Arguments:
             - considered_visit: the visit counts of node to be considered.
             - gumbel: the gumbel vector.
             - logits: the logits vector of child nodes.
             - normalized_qvalues: the normalized Q values of child nodes.
             - visit_counts: the visit counts of child nodes.
-        Outputs:
+        Returns:
             - the score of nodes to be considered.
         */
         float low_logit = -1e9;
         float max_logit = *max_element(logits.begin(), logits.end());
         for (unsigned int i=0;i < logits.size();i++){
             logits[i] -= max_logit;
         }
@@ -1135,15 +1135,15 @@
         /*
         Overview:
             Generate gumbel vectors.
         Arguments:
             - gumbel_scale: the scale of gumbel.
             - gumbel_rng: the seed to generate gumbel.
             - shape: the shape of gumbel vectors to be generated
-        Outputs:
+        Returns:
             - gumbel vectors.
         */
         std::mt19937 gen(static_cast<unsigned int>(gumbel_rng));
         std::extreme_value_distribution<float> d(0, 1);
 
         std::vector<float> gumbel;
         for (int i = 0;i < shape;i++)
```

### Comparing `LightZero-0.0.2/lzero/mcts/ctree/ctree_gumbel_muzero/lib/cnode.h` & `LightZero-0.0.5/lzero/mcts/ctree/ctree_gumbel_muzero/lib/cnode.h`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/lzero/mcts/ctree/ctree_muzero/lib/cnode.cpp` & `LightZero-0.0.5/lzero/mcts/ctree/ctree_muzero/lib/cnode.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -235,15 +235,15 @@
     }
 
     std::vector<int> CNode::get_trajectory()
     {
         /*
         Overview:
             Find the current best trajectory starts from the current node.
-        Outputs:
+        Returns:
             - traj: a vector of node index, which is the current best trajectory from this node.
         */
         std::vector<int> traj;
 
         CNode *node = this;
         int best_action = node->best_action;
         while (best_action >= 0)
@@ -257,15 +257,15 @@
     }
 
     std::vector<int> CNode::get_children_distribution()
     {
         /*
         Overview:
             Get the distribution of child nodes in the format of visit_count.
-        Outputs:
+        Returns:
             - distribution: a vector of distribution of child nodes in the format of visit count (i.e. [1,3,0,2,5]).
         */
         std::vector<int> distribution;
         if (this->expanded())
         {
             for (auto a : this->legal_actions)
             {
@@ -367,15 +367,15 @@
     }
 
     std::vector<std::vector<int> > CRoots::get_trajectories()
     {
         /*
         Overview:
             Find the current best trajectory starts from each root.
-        Outputs:
+        Returns:
             - traj: a vector of node index, which is the current best trajectory from each root.
         */
         std::vector<std::vector<int> > trajs;
         trajs.reserve(this->root_num);
 
         for (int i = 0; i < this->root_num; ++i)
         {
@@ -385,15 +385,15 @@
     }
 
     std::vector<std::vector<int> > CRoots::get_distributions()
     {
         /*
         Overview:
             Get the children distribution of each root.
-        Outputs:
+        Returns:
             - distribution: a vector of distribution of child nodes in the format of visit count (i.e. [1,3,0,2,5]).
         */
         std::vector<std::vector<int> > distributions;
         distributions.reserve(this->root_num);
 
         for (int i = 0; i < this->root_num; ++i)
         {
@@ -412,63 +412,14 @@
         for (int i = 0; i < this->root_num; ++i)
         {
             values.push_back(this->roots[i].value());
         }
         return values;
     }
 
-    //*********************************************************
-    //
-    void update_tree_q(CNode *root, tools::CMinMaxStats &min_max_stats, float discount_factor, int players)
-    {
-        /*
-        Overview:
-            Update the q value of the root and its child nodes.
-        Arguments:
-            - root: the root that update q value from.
-            - min_max_stats: a tool used to min-max normalize the q value.
-            - discount_factor: the discount factor of reward.
-            - players: the number of players.
-        */
-        std::stack<CNode *> node_stack;
-        node_stack.push(root);
-        while (node_stack.size() > 0)
-        {
-            CNode *node = node_stack.top();
-            node_stack.pop();
-
-            if (node != root)
-            {
-                //                # NOTE: in self-play-mode, value_prefix is not calculated according to the perspective of current player of node,
-                //                # but treated as 1 player, just for obtaining the true reward in the perspective of current player of node.
-                //                # true_reward = node.value_prefix - (- parent_value_prefix)
-                //                float true_reward = node->value_prefix - node->parent_value_prefix;
-                float true_reward = node->reward;
-
-                float qsa;
-                if (players == 1)
-                    qsa = true_reward + discount_factor * node->value();
-                else if (players == 2)
-                    // TODO(pu):
-                    qsa = true_reward + discount_factor * (-1) * node->value();
-
-                min_max_stats.update(qsa);
-            }
-
-            for (auto a : node->legal_actions)
-            {
-                CNode *child = node->get_child(a);
-                if (child->expanded())
-                {
-                    node_stack.push(child);
-                }
-            }
-        }
-    }
-
     void cbackpropagate(std::vector<CNode *> &search_path, tools::CMinMaxStats &min_max_stats, int to_play, float value, float discount_factor)
     {
         /*
         Overview:
             Update the value sum and visit count of nodes along the search path.
         Arguments:
             - search_path: a vector of nodes on the search path.
@@ -522,32 +473,32 @@
                     bootstrap_value = -true_reward + discount_factor * bootstrap_value;
                 else
                     bootstrap_value = true_reward + discount_factor * bootstrap_value;
             }
         }
     }
 
-    void cbatch_backpropagate(int current_latent_state_index, float discount_factor, const std::vector<float> &value_prefixs, const std::vector<float> &values, const std::vector<std::vector<float> > &policies, tools::CMinMaxStatsList *min_max_stats_lst, CSearchResults &results, std::vector<int> &to_play_batch)
+    void cbatch_backpropagate(int current_latent_state_index, float discount_factor, const std::vector<float> &rewards, const std::vector<float> &values, const std::vector<std::vector<float> > &policies, tools::CMinMaxStatsList *min_max_stats_lst, CSearchResults &results, std::vector<int> &to_play_batch)
     {
         /*
         Overview:
             Expand the nodes along the search path and update the infos.
         Arguments:
             - current_latent_state_index: The index of latent state of the leaf node in the search path.
             - discount_factor: the discount factor of reward.
-            - value_prefixs: the value prefixs of nodes along the search path.
+            - rewards: the rewards of nodes along the search path.
             - values: the values to propagate along the search path.
             - policies: the policy logits of nodes along the search path.
             - min_max_stats: a tool used to min-max normalize the q value.
             - results: the search results.
             - to_play_batch: the batch of which player is playing on this node.
         */
         for (int i = 0; i < results.num; ++i)
         {
-            results.nodes[i]->expand(to_play_batch[i], current_latent_state_index, i, value_prefixs[i], policies[i]);
+            results.nodes[i]->expand(to_play_batch[i], current_latent_state_index, i, rewards[i], policies[i]);
             cbackpropagate(results.search_paths[i], min_max_stats_lst->stats_lst[i], to_play_batch[i], values[i], discount_factor);
         }
     }
 
     int cselect_child(CNode *root, tools::CMinMaxStats &min_max_stats, int pb_c_base, float pb_c_init, float discount_factor, float mean_q, int players)
     {
         /*
@@ -557,15 +508,15 @@
             - root: the roots to select the child node.
             - min_max_stats: a tool used to min-max normalize the score.
             - pb_c_base: constants c2 in muzero.
             - pb_c_init: constants c1 in muzero.
             - disount_factor: the discount factor of reward.
             - mean_q: the mean q value of the parent node.
             - players: the number of players.
-        Outputs:
+        Returns:
             - action: the action to select.
         */
         float max_score = FLOAT_MIN;
         const float epsilon = 0.000001;
         std::vector<int> max_index_lst;
         for (auto a : root->legal_actions)
         {
@@ -605,15 +556,15 @@
             - min_max_stats: a tool used to min-max normalize the score.
             - mean_q: the mean q value of the parent node.
             - total_children_visit_counts: the total visit counts of the child nodes of the parent node.
             - pb_c_base: constants c2 in muzero.
             - pb_c_init: constants c1 in muzero.
             - disount_factor: the discount factor of reward.
             - players: the number of players.
-        Outputs:
+        Returns:
             - ucb_value: the ucb score of the child.
         */
         float pb_c = 0.0, prior_score = 0.0, value_score = 0.0;
         pb_c = log((total_children_visit_counts + pb_c_base + 1) / pb_c_base) + pb_c_init;
         pb_c *= (sqrt(total_children_visit_counts) / (child->visit_count + 1));
 
         prior_score = pb_c * child->prior;
```

### Comparing `LightZero-0.0.2/lzero/mcts/ctree/ctree_muzero/lib/cnode.h` & `LightZero-0.0.5/lzero/mcts/ctree/ctree_muzero/lib/cnode.h`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/lzero/mcts/ctree/ctree_sampled_efficientzero/lib/cnode.cpp` & `LightZero-0.0.5/lzero/mcts/ctree/ctree_sampled_efficientzero/lib/cnode.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         }
         return hash;
     }
     size_t CAction::get_combined_hash(void)
     {
         /*
         Overview:
-            get the final combined hash value from the hash values of each dimension of the multi-dimensional action.
+            Get the final combined hash value from the hash values of each dimension of the multi-dimensional action.
         */
         std::vector<size_t> hash = this->get_hash();
         size_t combined_hash = hash[0];
 
         if (hash.size() >= 1)
         {
             for (int i = 1; i < hash.size(); ++i)
@@ -376,20 +376,22 @@
                 disturbed_probs.push_back(std::pow(uniform_distribution(generator), 1. / prob));
             }
 
             // Sort from large to small according to the probability value after the disturbance:
             // After sorting, the first vector is the index, and the second vector is the probability value after perturbation sorted from large to small.
             for (size_t iter = 0; iter < disturbed_probs.size(); iter++)
             {
-//                #ifdef __APPLE__
-//                    disc_action_with_probs.__emplace_back(std::make_pair(iter, disturbed_probs[iter]));
-//                #else
-//                    disc_action_with_probs.emplace_back(std::make_pair(iter, disturbed_probs[iter]));
-//                #endif
-                 disc_action_with_probs.emplace_back(std::make_pair(iter, disturbed_probs[iter]));
+
+            #ifdef __GNUC__
+                // Use push_back for GCC
+                disc_action_with_probs.push_back(std::make_pair(iter, disturbed_probs[iter]));
+            #else
+                // Use emplace_back for other compilers
+                disc_action_with_probs.emplace_back(std::make_pair(iter, disturbed_probs[iter]));
+            #endif
             }
 
             std::sort(disc_action_with_probs.begin(), disc_action_with_probs.end(), cmp);
 
             // take the fist ``num_of_sampled_actions`` actions
             for (int k = 0; k < num_of_sampled_actions; ++k)
             {
@@ -552,15 +554,15 @@
     }
 
     std::vector<std::vector<float> > CNode::get_trajectory()
     {
         /*
         Overview:
             Find the current best trajectory starts from the current node.
-        Outputs:
+        Returns:
             - traj: a vector of node index, which is the current best trajectory from this node.
         */
         std::vector<CAction> traj;
 
         CNode *node = this;
         CAction best_action = node->best_action;
         while (best_action.is_root_action != 1)
@@ -579,15 +581,15 @@
     }
 
     std::vector<int> CNode::get_children_distribution()
     {
         /*
         Overview:
             Get the distribution of child nodes in the format of visit_count.
-        Outputs:
+        Returns:
             - distribution: a vector of distribution of child nodes in the format of visit count (i.e. [1,3,0,2,5]).
         */
         std::vector<int> distribution;
         if (this->expanded())
         {
             for (auto a : this->legal_actions)
             {
@@ -718,15 +720,15 @@
     }
 
     std::vector<std::vector<std::vector<float> > > CRoots::get_trajectories()
     {
         /*
         Overview:
             Find the current best trajectory starts from each root.
-        Outputs:
+        Returns:
             - traj: a vector of node index, which is the current best trajectory from each root.
         */
         std::vector<std::vector<std::vector<float> > > trajs;
         trajs.reserve(this->root_num);
 
         for (int i = 0; i < this->root_num; ++i)
         {
@@ -736,15 +738,15 @@
     }
 
     std::vector<std::vector<int> > CRoots::get_distributions()
     {
         /*
         Overview:
             Get the children distribution of each root.
-        Outputs:
+        Returns:
             - distribution: a vector of distribution of child nodes in the format of visit count (i.e. [1,3,0,2,5]).
         */
         std::vector<std::vector<int> > distributions;
         distributions.reserve(this->root_num);
 
         for (int i = 0; i < this->root_num; ++i)
         {
@@ -755,15 +757,15 @@
 
     // sampled related core code
     std::vector<std::vector<std::vector<float> > > CRoots::get_sampled_actions()
     {
         /*
         Overview:
             Get the sampled_actions of each root.
-        Outputs:
+        Returns:
             - python_sampled_actions: a vector of sampled_actions for each root, e.g. the size of original action space is 6, the K=3, 
             python_sampled_actions = [[1,3,0], [2,4,0], [5,4,1]].
         */
         std::vector<std::vector<CAction> > sampled_actions;
         std::vector<std::vector<std::vector<float> > > python_sampled_actions;
 
         //  sampled_actions.reserve(this->root_num);
@@ -978,15 +980,15 @@
             - min_max_stats: a tool used to min-max normalize the score.
             - pb_c_base: constants c2 in muzero.
             - pb_c_init: constants c1 in muzero.
             - disount_factor: the discount factor of reward.
             - mean_q: the mean q value of the parent node.
             - players: the number of players.
             - continuous_action_space: whether the action space is continous in current env.
-        Outputs:
+        Returns:
             - action: the action to select.
         */
         // sampled related core code
         // TODO(pu): Progressive widening (See https://hal.archives-ouvertes.fr/hal-00542673v2/document)
         float max_score = FLOAT_MIN;
         const float epsilon = 0.000001;
         std::vector<CAction> max_index_lst;
@@ -1034,15 +1036,15 @@
             - total_children_visit_counts: the total visit counts of the child nodes of the parent node.
             - parent_value_prefix: the value prefix of parent node.
             - pb_c_base: constants c2 in muzero.
             - pb_c_init: constants c1 in muzero.
             - disount_factor: the discount factor of reward.
             - players: the number of players.
             - continuous_action_space: whether the action space is continous in current env.
-        Outputs:
+        Returns:
             - ucb_value: the ucb score of the child.
         */
         float pb_c = 0.0, prior_score = 0.0, value_score = 0.0;
         pb_c = log((total_children_visit_counts + pb_c_base + 1) / pb_c_base) + pb_c_init;
         pb_c *= (sqrt(total_children_visit_counts) / (child->visit_count + 1));
 
         // prior_score = pb_c * child->prior;
```

### Comparing `LightZero-0.0.2/lzero/mcts/ctree/ctree_sampled_efficientzero/lib/cnode.h` & `LightZero-0.0.5/lzero/mcts/ctree/ctree_sampled_efficientzero/lib/cnode.h`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/lzero/mcts/ctree/ctree_stochastic_muzero/lib/cnode.cpp` & `LightZero-0.0.5/lzero/mcts/ctree/ctree_stochastic_muzero/lib/cnode.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,15 @@
     {
         /*
         Overview:
             Initialization of CNode with prior value and legal actions.
         Arguments:
             - prior: the prior value of this node.
             - legal_actions: a vector of legal actions of this node.
+            - is_chance: Whether the node is a chance node.
         */
         this->prior = prior;
         this->legal_actions = legal_actions;
 
         this->visit_count = 0;
         this->value_sum = 0;
         this->best_action = -1;
@@ -260,15 +261,15 @@
     }
 
     std::vector<int> CNode::get_trajectory()
     {
         /*
         Overview:
             Find the current best trajectory starts from the current node.
-        Outputs:
+        Returns:
             - traj: a vector of node index, which is the current best trajectory from this node.
         */
         std::vector<int> traj;
 
         CNode *node = this;
         int best_action = node->best_action;
         while (best_action >= 0)
@@ -282,15 +283,15 @@
     }
 
     std::vector<int> CNode::get_children_distribution()
     {
         /*
         Overview:
             Get the distribution of child nodes in the format of visit_count.
-        Outputs:
+        Returns:
             - distribution: a vector of distribution of child nodes in the format of visit count (i.e. [1,3,0,2,5]).
         */
         std::vector<int> distribution;
         if (this->expanded())
         {
             for (auto a : this->legal_actions)
             {
@@ -394,15 +395,15 @@
     }
 
     std::vector<std::vector<int> > CRoots::get_trajectories()
     {
         /*
         Overview:
             Find the current best trajectory starts from each root.
-        Outputs:
+        Returns:
             - traj: a vector of node index, which is the current best trajectory from each root.
         */
         std::vector<std::vector<int> > trajs;
         trajs.reserve(this->root_num);
 
         for (int i = 0; i < this->root_num; ++i)
         {
@@ -412,15 +413,15 @@
     }
 
     std::vector<std::vector<int> > CRoots::get_distributions()
     {
         /*
         Overview:
             Get the children distribution of each root.
-        Outputs:
+        Returns:
             - distribution: a vector of distribution of child nodes in the format of visit count (i.e. [1,3,0,2,5]).
         */
         std::vector<std::vector<int> > distributions;
         distributions.reserve(this->root_num);
 
         for (int i = 0; i < this->root_num; ++i)
         {
@@ -599,15 +600,15 @@
             - root: the roots to select the child node.
             - min_max_stats: a tool used to min-max normalize the score.
             - pb_c_base: constants c2 in muzero.
             - pb_c_init: constants c1 in muzero.
             - disount_factor: the discount factor of reward.
             - mean_q: the mean q value of the parent node.
             - players: the number of players.
-        Outputs:
+        Returns:
             - action: the action to select.
         */
         if (root->is_chance) {
                 // std::cout << "root->is_chance: True " << std::endl;
 
                 // If the node is a chance node, we sample from the prior outcome distribution.
                 std::vector<int> outcomes;
@@ -671,15 +672,15 @@
             - min_max_stats: a tool used to min-max normalize the score.
             - mean_q: the mean q value of the parent node.
             - total_children_visit_counts: the total visit counts of the child nodes of the parent node.
             - pb_c_base: constants c2 in muzero.
             - pb_c_init: constants c1 in muzero.
             - disount_factor: the discount factor of reward.
             - players: the number of players.
-        Outputs:
+        Returns:
             - ucb_value: the ucb score of the child.
         */
         float pb_c = 0.0, prior_score = 0.0, value_score = 0.0;
         pb_c = log((total_children_visit_counts + pb_c_base + 1) / pb_c_base) + pb_c_init;
         pb_c *= (sqrt(total_children_visit_counts) / (child->visit_count + 1));
 
         prior_score = pb_c * child->prior;
```

### Comparing `LightZero-0.0.2/lzero/mcts/ctree/ctree_stochastic_muzero/lib/cnode.h` & `LightZero-0.0.5/lzero/mcts/ctree/ctree_stochastic_muzero/lib/cnode.h`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/lzero/mcts/ptree/ptree_az.py` & `LightZero-0.0.5/lzero/mcts/ptree/ptree_az.py`

 * *Files 5% similar despite different names*

```diff
@@ -71,47 +71,47 @@
             - value (:obj:`Float`): The value of the node.
         """
         # Updates the number of times this node has been visited.
         self._visit_count += 1
         # Updates the sum of the values of all child nodes of this node.
         self._value_sum += value
 
-    def update_recursive(self, leaf_value: float, mcts_mode: str) -> None:
+    def update_recursive(self, leaf_value: float, battle_mode_in_simulation_env: str) -> None:
         """
         Overview:
             Update node information recursively.
             The same game state has opposite values in the eyes of two players playing against each other. 
             The value of a node is evaluated from the perspective of the player corresponding to its parent node. 
             In ``self_play_mode``, because the player corresponding to a node changes every step during the backpropagation process, the value needs to be negated once. 
             In ``play_with_bot_mode``, since all nodes correspond to the same player, the value does not need to be negated.
 
         Arguments:
             - leaf_value (:obj:`Float`): The value of the node.
-            - mcts_mode (:obj:`str`): The mode of MCTS, can be 'self_play_mode' or 'play_with_bot_mode'.
+            - battle_mode_in_simulation_env (:obj:`str`): The mode of MCTS, can be 'self_play_mode' or 'play_with_bot_mode'.
         """
         # Update the node information recursively based on the MCTS mode.
-        if mcts_mode == 'self_play_mode':
+        if battle_mode_in_simulation_env == 'self_play_mode':
             # Update the current node's information.
             self.update(leaf_value)
             # If the current node is the root node, return.
             if self.is_root():
                 return
             # Update the parent node's information recursively. When propagating the value back to the parent node,
             # the value needs to be negated once because the perspective of evaluation has changed.
-            self._parent.update_recursive(-leaf_value, mcts_mode)
-        if mcts_mode == 'play_with_bot_mode':
+            self._parent.update_recursive(-leaf_value, battle_mode_in_simulation_env)
+        if battle_mode_in_simulation_env == 'play_with_bot_mode':
             # Update the current node's information.
             self.update(leaf_value)
             # If the current node is the root node, return.
             if self.is_root():
                 return
             # Update the parent node's information recursively. In ``play_with_bot_mode``, since the nodes' values
             # are always evaluated from the perspective of the agent player, there is no need to negate the value
             # during value propagation.
-            self._parent.update_recursive(leaf_value, mcts_mode)
+            self._parent.update_recursive(leaf_value, battle_mode_in_simulation_env)
 
     def is_leaf(self) -> bool:
         """
         Overview:
             Check if the current node is a leaf node or not.
         Returns:
             - output (:obj:`Bool`): If self._children is empty, it means that the node has not 
@@ -238,15 +238,15 @@
                 init_state=state_config_for_simulate_env_reset.init_state,
             )
             # Set the battle mode adopted by the environment during the MCTS process.
             # In ``self_play_mode``, when the environment calls the step function once, it will play one move based on the incoming action.
             # In ``play_with_bot_mode``, when the step function is called, it will play one move based on the incoming action,
             # and then it will play another move based on the action generated by the built-in bot in the environment, which means two moves in total.
             # Therefore, in the MCTS process, except for the terminal nodes, the player corresponding to each node is the same player as the root node.
-            self.simulate_env.battle_mode = self.simulate_env.mcts_mode
+            self.simulate_env.battle_mode = self.simulate_env.battle_mode_in_simulation_env
             self.simulate_env.render_mode = None
             # Run the simulation from the root to a leaf node and update the node values along the way.
             self._simulate(root, self.simulate_env, policy_forward_fn)
 
         # Get the visit count for each possible action at the root node.
         action_visits = []
         for action in range(self.simulate_env.action_space.n):
@@ -258,15 +258,15 @@
         # Unpack the tuples in action_visits list into two separate tuples: actions and visits.
         actions, visits = zip(*action_visits)
 
         # Calculate the action probabilities based on the visit counts and temperature.
         # When the visit count of a node is 0, then the corresponding action probability will be 0 in order to prevent the selection of illegal actions.
         visits_t = torch.as_tensor(visits, dtype=torch.float32)
         visits_t = torch.pow(visits_t, 1/temperature)
-        action_probs= (visits_t / visits_t.sum()).numpy()
+        action_probs = (visits_t / visits_t.sum()).numpy()
 
         # action_probs = nn.functional.softmax(1.0 / temperature * np.log(torch.as_tensor(visits) + 1e-10), dim=0).numpy()
 
         # Choose the next action to take based on the action probabilities.
         if sample:
             action = np.random.choice(actions, p=action_probs)
         else:
@@ -302,46 +302,46 @@
         if not done:
             # The leaf_value here is obtained from the neural network. The perspective of this value is from the
             # player corresponding to the game state input to the neural network. For example, if the current_player
             # of the current node is player 1, the value output by the network represents the goodness of the current
             # game state from the perspective of player 1.
             leaf_value = self._expand_leaf_node(node, simulate_env, policy_forward_fn)
         else:
-            if simulate_env.mcts_mode == 'self_play_mode':
+            if simulate_env.battle_mode_in_simulation_env == 'self_play_mode':
                 # In a tie game, the value corresponding to a terminal node is 0.
                 if winner == -1:
                     leaf_value = 0
                 else:
                     # To maintain consistency with the perspective of the neural network, the value of a terminal
                     # node is also calculated from the perspective of the current_player of the terminal node,
                     # which is convenient for subsequent updates.
                     leaf_value = 1 if simulate_env.current_player == winner else -1
 
-            if simulate_env.mcts_mode == 'play_with_bot_mode':
+            if simulate_env.battle_mode_in_simulation_env == 'play_with_bot_mode':
                 # in ``play_with_bot_mode``, the leaf_value should be transformed to the perspective of player 1.
                 if winner == -1:
                     leaf_value = 0
                 elif winner == 1:
                     leaf_value = 1
                 elif winner == 2:
                     leaf_value = -1
 
         # Update value and visit count of nodes in this traversal.
-        if simulate_env.mcts_mode == 'play_with_bot_mode':
-            node.update_recursive(leaf_value, simulate_env.mcts_mode)
-        elif simulate_env.mcts_mode == 'self_play_mode':
+        if simulate_env.battle_mode_in_simulation_env == 'play_with_bot_mode':
+            node.update_recursive(leaf_value, simulate_env.battle_mode_in_simulation_env)
+        elif simulate_env.battle_mode_in_simulation_env == 'self_play_mode':
             # NOTE: e.g.
             #       to_play: 1  ---------->  2  ---------->  1  ----------> 2
             #         state: s1 ---------->  s2 ---------->  s3 ----------> s4
             #                                     action    node
             #                                            leaf_value
             # leaf_value is calculated from the perspective of player 1, leaf_value = value_func(s3),
             # but node.value should be the value of E[q(s2, action)], i.e. calculated from the perspective of player 2.
             # thus we add the negative when call update_recursive().
-            node.update_recursive(-leaf_value, simulate_env.mcts_mode)
+            node.update_recursive(-leaf_value, simulate_env.battle_mode_in_simulation_env)
 
     def _select_child(self, node: Node, simulate_env: Type[BaseEnv]) -> Tuple[Union[int, float], Node]:
         """
         Overview:
             Select the child with the highest UCB score.
         Arguments:
             - node (:obj:`Class Node`): Current node.
@@ -398,15 +398,15 @@
         return leaf_value
 
     def _ucb_score(self, parent: Node, child: Node) -> float:
         """
         Overview:
             Compute UCB score. The score for a node is based on its value, plus an exploration bonus based on the prior.
             For more details, please refer to this paper: http://gauss.ececs.uc.edu/Workshops/isaim2010/papers/rosin.pdf
-            UCB = Q(s,a) + P(s,a) \cdot \frac{N(\text{parent})}{1+N(\text{child})} \cdot \left(c_1 + \log\left(\frac{N(\text{parent})+c_2+1}{c_2}\right)\right)
+            UCB = Q(s,a) + P(s,a) \cdot \frac{ \sqrt{N(\text{parent})}}{1+N(\text{child})} \cdot \left(c_1 + \log\left(\frac{N(\text{parent})+c_2+1}{c_2}\right)\right)
             - Q(s,a): value of a child node.
             - P(s,a): The prior of a child node.
             - N(parent): The number of the visiting of the parent node.
             - N(child): The number of the visiting of the child node.
             - c_1: a parameter given by self._pb_c_init to control the influence of the prior P(s,a) relative to the value Q(s,a).
             - c_2: a parameter given by self._pb_c_base to control the influence of the prior P(s,a) relative to the value Q(s,a).
         Arguments:
```

### Comparing `LightZero-0.0.2/lzero/mcts/ptree/ptree_az_sampled.py` & `LightZero-0.0.5/lzero/mcts/ptree/ptree_az_sampled.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,47 +72,47 @@
             - value (:obj:`Float`): The value of the node.
         """
         # Updates the number of times this node has been visited.
         self._visit_count += 1
         # Updates the sum of the values of all child nodes of this node.
         self._value_sum += value
 
-    def update_recursive(self, leaf_value: float, mcts_mode: str) -> None:
+    def update_recursive(self, leaf_value: float, battle_mode_in_simulation_env: str) -> None:
         """
         Overview:
             Update node information recursively.
             The same game state has opposite values in the eyes of two players playing against each other.
             The value of a node is evaluated from the perspective of the player corresponding to its parent node.
             In ``self_play_mode``, because the player corresponding to a node changes every step during the backpropagation process, the value needs to be negated once.
             In ``play_with_bot_mode``, since all nodes correspond to the same player, the value does not need to be negated.
 
         Arguments:
             - leaf_value (:obj:`Float`): The value of the node.
-            - mcts_mode (:obj:`str`): The mode of MCTS, can be 'self_play_mode' or 'play_with_bot_mode'.
+            - battle_mode_in_simulation_env (:obj:`str`): The mode of MCTS, can be 'self_play_mode' or 'play_with_bot_mode'.
         """
         # Update the node information recursively based on the MCTS mode.
-        if mcts_mode == 'self_play_mode':
+        if battle_mode_in_simulation_env == 'self_play_mode':
             # Update the current node's information.
             self.update(leaf_value)
             # If the current node is the root node, return.
             if self.is_root():
                 return
             # Update the parent node's information recursively. When propagating the value back to the parent node,
             # the value needs to be negated once because the perspective of evaluation has changed.
-            self._parent.update_recursive(-leaf_value, mcts_mode)
-        if mcts_mode == 'play_with_bot_mode':
+            self._parent.update_recursive(-leaf_value, battle_mode_in_simulation_env)
+        if battle_mode_in_simulation_env == 'play_with_bot_mode':
             # Update the current node's information.
             self.update(leaf_value)
             # If the current node is the root node, return.
             if self.is_root():
                 return
             # Update the parent node's information recursively. In ``play_with_bot_mode``, since the nodes' values
             # are always evaluated from the perspective of the agent player, there is no need to negate the value
             # during value propagation.
-            self._parent.update_recursive(leaf_value, mcts_mode)
+            self._parent.update_recursive(leaf_value, battle_mode_in_simulation_env)
 
     def is_leaf(self) -> bool:
         """
         Overview:
             Check if the current node is a leaf node or not.
         Returns:
             - output (:obj:`Bool`): If self._children is empty, it means that the node has not
@@ -238,15 +238,15 @@
             self._add_exploration_noise(self.root)
 
         for n in range(self._num_simulations):
             self.simulate_env.reset(
                 start_player_index=state_config_for_env_reset.start_player_index,
                 init_state=state_config_for_env_reset.init_state,
             )
-            self.simulate_env.battle_mode = self.simulate_env.mcts_mode
+            self.simulate_env.battle_mode = self.simulate_env.battle_mode_in_simulation_env
             self._simulate(self.root, self.simulate_env, policy_value_func)
 
         # sampled related code
         # Get the visit count for each possible action at the root node.
         action_visits = []
         for action in range(self.simulate_env.action_space.n):
             # Create an Action object for the current action
@@ -317,46 +317,46 @@
             # The leaf_value here is obtained from the neural network. The perspective of this value is from the
             # player corresponding to the game state input to the neural network. For example, if the current_player
             # of the current node is player 1, the value output by the network represents the goodness of the current
             # game state from the perspective of player 1.
             leaf_value = self._expand_leaf_node(node, simulate_env, policy_value_func)
 
         else:
-            if simulate_env.mcts_mode == 'self_play_mode':
+            if simulate_env.battle_mode_in_simulation_env == 'self_play_mode':
                 # In a tie game, the value corresponding to a terminal node is 0.
                 if winner == -1:
                     leaf_value = 0
                 else:
                     # To maintain consistency with the perspective of the neural network, the value of a terminal
                     # node is also calculated from the perspective of the current_player of the terminal node,
                     # which is convenient for subsequent updates.
                     leaf_value = 1 if simulate_env.current_player == winner else -1
 
-            if simulate_env.mcts_mode == 'play_with_bot_mode':
+            if simulate_env.battle_mode_in_simulation_env == 'play_with_bot_mode':
                 # in ``play_with_bot_mode``, the leaf_value should be transformed to the perspective of player 1.
                 if winner == -1:
                     leaf_value = 0
                 elif winner == 1:
                     leaf_value = 1
                 elif winner == 2:
                     leaf_value = -1
 
         # Update value and visit count of nodes in this traversal.
-        if simulate_env.mcts_mode == 'play_with_bot_mode':
-            node.update_recursive(leaf_value, simulate_env.mcts_mode)
-        elif simulate_env.mcts_mode == 'self_play_mode':
+        if simulate_env.battle_mode_in_simulation_env == 'play_with_bot_mode':
+            node.update_recursive(leaf_value, simulate_env.battle_mode_in_simulation_env)
+        elif simulate_env.battle_mode_in_simulation_env == 'self_play_mode':
             # NOTE: e.g.
             #       to_play: 1  ---------->  2  ---------->  1  ----------> 2
             #         state: s1 ---------->  s2 ---------->  s3 ----------> s4
             #                                     action    node
             #                                            leaf_value
             # leaf_value is calculated from the perspective of player 1, leaf_value = value_func(s3),
             # but node.value should be the value of E[q(s2, action)], i.e. calculated from the perspective of player 2.
             # thus we add the negative when call update_recursive().
-            node.update_recursive(-leaf_value, simulate_env.mcts_mode)
+            node.update_recursive(-leaf_value, simulate_env.battle_mode_in_simulation_env)
 
     def _select_child(self, node: Node, simulate_env: Type[BaseEnv]) -> Tuple[Union[int, float], Node]:
         """
         Overview:
             Select the child with the highest UCB score.
         Arguments:
             - node (:obj:`Class Node`): Current node.
```

### Comparing `LightZero-0.0.2/lzero/mcts/ptree/ptree_ez.py` & `LightZero-0.0.5/lzero/mcts/ptree/ptree_stochastic_mz.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,76 +1,104 @@
 """
-The Node, Roots class and related core functions for EfficientZero.
+The Node, Roots class and related core functions for Stochastic MuZero.
 """
 import math
 import random
-from typing import List, Any, Tuple, Union
+from typing import List, Dict, Any, Tuple, Union
 
 import numpy as np
 import torch
 
 from .minimax import MinMaxStats
 
 
 class Node:
     """
-     Overview:
-         the node base class for EfficientZero.
-     """
+    Overview:
+        The Node class for  Stochastic MuZero. The basic functions of the node are implemented.
+    Interfaces:
+        ``__init__``, ``expand``, ``add_exploration_noise``, ``compute_mean_q``, ``get_trajectory``, \
+        ``get_children_distribution``, ``get_child``, ``expanded``, ``value``.
+    """
 
-    def __init__(self, prior: float, legal_actions: List = None, action_space_size: int = 9) -> None:
+    def __init__(self, prior: float, legal_actions: List = None, action_space_size: int = 9, is_chance: bool = False, chance_space_size: int = 2) -> None:
+        """
+        Overview:
+            Initializes a Node instance.
+        Arguments:
+            - prior (:obj:`float`): The prior probability of the node.
+            - legal_actions (:obj:`List`, optional): The list of legal actions of the node. Defaults to None.
+            - action_space_size (:obj:`int`, optional): The size of the action space. Defaults to 9.
+            - is_chance (:obj:`bool`) Whether the node is a chance node.
+        """
         self.prior = prior
         self.legal_actions = legal_actions
         self.action_space_size = action_space_size
 
-        self.is_reset = 0
         self.visit_count = 0
         self.value_sum = 0
         self.best_action = -1
-        self.to_play = -1  # default -1 means play_with_bot_mode
+        self.to_play = 0  # default 0 means play_with_bot_mode
+        self.reward = 0
         self.value_prefix = 0.0
         self.children = {}
         self.children_index = []
-        self.simulation_index = 0
-        self.batch_index = 0
+        self.latent_state_index_in_search_path = 0
+        self.latent_state_index_in_batch = 0
         self.parent_value_prefix = 0  # only used in update_tree_q method
 
+        self.is_chance = is_chance
+        self.chance_space_size = chance_space_size
+
     def expand(
-            self, to_play: int, simulation_index: int, batch_index: int, value_prefix: float, policy_logits: List[float]
+            self, to_play: int, latent_state_index_in_search_path: int, latent_state_index_in_batch: int, reward: float,
+            policy_logits: List[float], child_is_chance: bool = True
     ) -> None:
         """
         Overview:
             Expand the child nodes of the current node.
         Arguments:
-            - to_play (:obj:`Class int`): which player to play the game in the current node.
-            - simulation_index (:obj:`Class int`): the x/first index of hidden state vector of the current node, i.e. the search depth.
-            - batch_index (:obj:`Class int`): the y/second index of hidden state vector of the current node, i.e. the index of batch root node, its maximum is ``batch_size``/``env_num``.
-            - value_prefix: (:obj:`Class float`): the value prefix of the current node.
-            - policy_logits: (:obj:`Class List`): the policy logit of the child nodes.
+            - to_play (:obj:`int`): which player to play the game in the current node.
+            - latent_state_index_in_search_path (:obj:`int`): the x/first index of latent state vector of the current node, i.e. the search depth.
+            - latent_state_index_in_batch (:obj:`int`): the y/second index of latent state vector of the current node, i.e. the index of batch root node, its maximum is ``batch_size``/``env_num``.
+            - reward: (:obj:`float`): the value prefix of the current node.
+            - policy_logits: (:obj:`List`): the policy logit of the child nodes.
         """
         self.to_play = to_play
-        if self.legal_actions is None:
-            self.legal_actions = np.arange(len(policy_logits))
+        self.reward = reward
 
-        self.simulation_index = simulation_index
-        self.batch_index = batch_index
-        self.value_prefix = value_prefix
-
-        policy_values = torch.softmax(torch.tensor([policy_logits[a] for a in self.legal_actions]), dim=0).tolist()
-        policy = {a: policy_values[i] for i, a in enumerate(self.legal_actions)}
-        for action, p in policy.items():
-            self.children[action] = Node(p, action_space_size=self.action_space_size)
+        if self.is_chance is True:
+            child_is_chance = False
+            self.reward = 0.0
+
+            if self.legal_actions is None:
+                self.legal_actions = np.arange(self.chance_space_size)
+            self.latent_state_index_in_search_path = latent_state_index_in_search_path
+            self.latent_state_index_in_batch = latent_state_index_in_batch
+            policy_values = torch.softmax(torch.tensor([policy_logits[a] for a in self.legal_actions]), dim=0).tolist()
+            policy = {legal_action: policy_values[index] for index, legal_action in enumerate(self.legal_actions)}
+            for action, prior in policy.items():
+                self.children[action] = Node(prior, is_chance=child_is_chance)
+        else:
+            child_is_chance = True
+            self.legal_actions = np.arange(len(policy_logits))
+            self.latent_state_index_in_search_path = latent_state_index_in_search_path
+            self.latent_state_index_in_batch = latent_state_index_in_batch
+            policy_values = torch.softmax(torch.tensor([policy_logits[a] for a in self.legal_actions]), dim=0).tolist()
+            policy = {legal_action: policy_values[index] for index, legal_action in enumerate(self.legal_actions)}
+            for action, prior in policy.items():
+                self.children[action] = Node(prior, is_chance=child_is_chance)
 
     def add_exploration_noise(self, exploration_fraction: float, noises: List[float]) -> None:
         """
         Overview:
-            Add a noise to the prior of the child nodes.
+            Add exploration noise to the priors.
         Arguments:
-            - exploration_fraction: the fraction to add noise.
-            - noises (:obj: list): the vector of noises added to each child node. length is len(self.legal_actions)
+            - exploration_fraction (:obj:`float`): The fraction of exploration noise to be added.
+            - noises (:obj:`List[float]`): The list of noises to be added to the priors.
         """
         for i, a in enumerate(self.legal_actions):
             """
             i in index, a is action, e.g. self.legal_actions = [0,1,2,4,6,8], i=[0,1,2,3,4,5], a=[0,1,2,4,6,8]
             """
             try:
                 noise = noises[i]
@@ -79,507 +107,536 @@
             child = self.get_child(a)
             prior = child.prior
             child.prior = prior * (1 - exploration_fraction) + noise * exploration_fraction
 
     def compute_mean_q(self, is_root: bool, parent_q: float, discount_factor: float) -> float:
         """
         Overview:
-            Compute the mean q value of the current node.
+            Compute the mean of the action values of all legal actions.
         Arguments:
-            - is_root (:obj:`bool`): whether the current node is a root node.
-            - parent_q (:obj:`float`): the q value of the parent node.
-            - discount_factor (:obj:`float`): the discount_factor of reward.
+            - is_root (:obj:`bool`): Whether the current node is a root node.
+            - parent_q (:obj:`float`): The q value of the parent node.
+            - discount_factor (:obj:`float`): The discount factor of the reward.
+        Returns:
+            - mean_q (:obj:`float`): The mean of the action values.
         """
         total_unsigned_q = 0.0
         total_visits = 0
-        parent_value_prefix = self.value_prefix
         for a in self.legal_actions:
             child = self.get_child(a)
             if child.visit_count > 0:
-                true_reward = child.value_prefix - parent_value_prefix
-                if self.is_reset == 1:
-                    # TODO(pu)
-                    true_reward = child.value_prefix
+                true_reward = child.reward
                 # TODO(pu): only one step bootstrap?
                 q_of_s_a = true_reward + discount_factor * child.value
                 total_unsigned_q += q_of_s_a
                 total_visits += 1
         if is_root and total_visits > 0:
             mean_q = total_unsigned_q / total_visits
         else:
             # if is not root node,
             # TODO(pu): why parent_q?
             mean_q = (parent_q + total_unsigned_q) / (total_visits + 1)
         return mean_q
 
-    def print_out(self) -> None:
-        pass
-
     def get_trajectory(self) -> List[Union[int, float]]:
         """
         Overview:
-            Find the current best trajectory starts from the current node.
-        Outputs:
-            - traj: a vector of node index, which is the current best trajectory from this node.
+            Find the current best trajectory starting from the current node.
+        Returns:
+            - traj (:obj:`List[Union[int, float]]`): A vector of node indices representing the current best trajectory.
         """
         # TODO(pu): best action
         traj = []
         node = self
         best_action = node.best_action
         while best_action >= 0:
             traj.append(best_action)
 
             node = node.get_child(best_action)
             best_action = node.best_action
         return traj
 
     def get_children_distribution(self) -> List[Union[int, float]]:
+        """
+        Overview:
+            Get the distribution of visit counts among the child nodes.
+        Returns:
+            - distribution (:obj:`List[Union[int, float]]` or :obj:`None`): The distribution of visit counts among the children nodes. \
+              If the legal_actions list is empty, returns None.
+        """
         if self.legal_actions == []:
             return None
         distribution = {a: 0 for a in self.legal_actions}
         if self.expanded:
             for a in self.legal_actions:
                 child = self.get_child(a)
                 distribution[a] = child.visit_count
             # only take the visit counts
             distribution = [v for k, v in distribution.items()]
         return distribution
 
     def get_child(self, action: Union[int, float]) -> "Node":
         """
         Overview:
-            get children node according to the input action.
+            Get the child node according to the input action.
+        Arguments:
+            - action (:obj:`Union[int, float]`): The action for which the child node is to be retrieved.
+        Returns:
+            - child (:obj:`Node`): The child node corresponding to the input action.
         """
         if not isinstance(action, np.int64):
             action = int(action)
         return self.children[action]
 
     @property
     def expanded(self) -> bool:
+        """
+        Overview:
+            Check if the node has been expanded.
+        Returns:
+            - expanded (:obj:`bool`): True if the node has been expanded, False otherwise.
+        """
         return len(self.children) > 0
 
     @property
     def value(self) -> float:
         """
         Overview:
-            Return the estimated value of the current root node.
+            Return the estimated value of the current node.
+        Returns:
+            - value (:obj:`float`): The estimated value of the current node.
         """
         if self.visit_count == 0:
             return 0
         else:
             return self.value_sum / self.visit_count
 
 
 class Roots:
+    """
+    Overview:
+        The class to process a batch of roots(Node instances) at the same time.
+    Interfaces:
+        ``__init__``, ``prepare``,  ``prepare_no_noise``, ``clear``, ``get_trajectories``, \
+        ``get_distributions``, ``get_values``
+    """
 
     def __init__(self, root_num: int, legal_actions_list: List) -> None:
+        """
+        Overview:
+            Initializes an instance of the Roots class with the specified number of roots and legal actions.
+        Arguments:
+            - root_num (:obj:`int`): The number of roots.
+            - legal_actions_list(:obj:`List`): A list of the legal actions for each root.
+        """
         self.num = root_num
         self.root_num = root_num
         self.legal_actions_list = legal_actions_list  # list of list
 
         self.roots = []
         for i in range(self.root_num):
             if isinstance(legal_actions_list, list):
-                self.action_space_size = len(legal_actions_list[i])
-
-                self.roots.append(Node(0, legal_actions_list[i], action_space_size=self.action_space_size))
+                self.roots.append(Node(0, legal_actions_list[i]))
             else:
                 # if legal_actions_list is int
-                self.action_space_size = legal_actions_list
-
-                self.roots.append(Node(0, np.arange(legal_actions_list), action_space_size=self.action_space_size))
+                self.roots.append(Node(0, np.arange(legal_actions_list)))
 
     def prepare(
             self,
             root_noise_weight: float,
             noises: List[float],
-            value_prefixs: List[float],
+            rewards: List[float],
             policies: List[List[float]],
             to_play: int = -1
     ) -> None:
         """
         Overview:
-            Expand the roots and add noises.
+            Expand the roots and add noises for exploration.
         Arguments:
-            - root_noise_weight: the exploration fraction of roots
-            - noises: the vector of noise add to the roots.
-            - value_prefixs: the vector of value prefixs of each root.
-            - policies: the vector of policy logits of each root.
-            - to_play_batch: the vector of the player side of each root.
+            - root_noise_weight (:obj:`float`): the exploration fraction of roots
+            - noises (:obj:`List[float]`): the vector of noise add to the roots.
+            - rewards (:obj:`List[float]`): the vector of rewards of each root.
+            - policies (:obj:`List[List[float]]`): the vector of policy logits of each root.
+            - to_play(:obj:`List`): The vector of the player side of each root.
         """
         for i in range(self.root_num):
-
-            if to_play in [-1, None]:
-                self.roots[i].expand(-1, 0, i, value_prefixs[i], policies[i])
-            elif to_play is [None]:
-                print('debug')
+            #  to_play: int, latent_state_index_in_search_path: int, latent_state_index_in_batch: int,
+            if to_play is None:
+                # TODO(pu): why latent_state_index_in_search_path=0, latent_state_index_in_batch=i?
+                self.roots[i].expand(-1, 0, i, rewards[i], policies[i])
             else:
-                self.roots[i].expand(to_play[i], 0, i, value_prefixs[i], policies[i])
+                self.roots[i].expand(to_play[i], 0, i, rewards[i], policies[i])
 
             self.roots[i].add_exploration_noise(root_noise_weight, noises[i])
             self.roots[i].visit_count += 1
 
-    def prepare_no_noise(self, value_prefixs: List[float], policies: List[List[float]], to_play: int = -1) -> None:
+    def prepare_no_noise(self, rewards: List[float], policies: List[List[float]], to_play: int = -1) -> None:
         """
         Overview:
             Expand the roots without noise.
         Arguments:
-            - value_prefixs: the vector of value prefixs of each root.
-            - policies: the vector of policy logits of each root.
-            - to_play_batch: the vector of the player side of each root.
+            - rewards (:obj:`List[float]`): the vector of rewards of each root.
+            - policies (:obj:`List[List[float]]`): the vector of policy logits of each root.
+            - to_play(:obj:`List`): The vector of the player side of each root.
         """
         for i in range(self.root_num):
-            if to_play in [-1, None]:
-                self.roots[i].expand(-1, 0, i, value_prefixs[i], policies[i])
+            if to_play is None:
+                self.roots[i].expand(-1, 0, i, rewards[i], policies[i])
             else:
-                self.roots[i].expand(to_play[i], 0, i, value_prefixs[i], policies[i])
+                self.roots[i].expand(to_play[i], 0, i, rewards[i], policies[i])
 
             self.roots[i].visit_count += 1
 
     def clear(self) -> None:
+        """
+        Overview:
+            Clear all the roots in the list.
+        """
         self.roots.clear()
 
     def get_trajectories(self) -> List[List[Union[int, float]]]:
         """
         Overview:
             Find the current best trajectory starts from each root.
-        Outputs:
-            - traj: a vector of node index, which is the current best trajectory from each root.
+        Returns:
+            - traj (:obj:`List[List[Union[int, float]]]`): a vector of node index, which is the current best trajectory from each root.
         """
         trajs = []
         for i in range(self.root_num):
             trajs.append(self.roots[i].get_trajectory())
         return trajs
 
     def get_distributions(self) -> List[List[Union[int, float]]]:
         """
         Overview:
-            Get the children distribution of each root.
-        Outputs:
-            - distribution: a vector of distribution of child nodes in the format of visit count (i.e. [1,3,0,2,5]).
+            Get the visit count distribution of child nodes for each root.
+        Returns:
+            - distribution (:obj:`List[List[Union[int, float]]]`): a vector of distribution of child nodes in the format of visit count (i.e. [1,3,0,2,5]).
         """
         distributions = []
         for i in range(self.root_num):
             distributions.append(self.roots[i].get_children_distribution())
 
         return distributions
 
     def get_values(self) -> List[float]:
         """
         Overview:
-            Return the estimated value of each root.
+            Get the estimated value of each root.
+        Returns:
+            - values (:obj:`List[float]`): The estimated value of each root.
         """
         values = []
         for i in range(self.root_num):
             values.append(self.roots[i].value)
         return values
 
 
 class SearchResults:
+    """
+    Overview:
+        The class to record the results of the simulations for the batch of roots.
+    Interfaces:
+        ``__init__``.
+    """
 
     def __init__(self, num: int) -> None:
+        """
+        Overview:
+            Initiaizes the attributes to be recorded.
+        Arguments:
+            -num (:obj:`int`): The number of search results(equal to ``batch_size``).
+        """
         self.num = num
         self.nodes = []
         self.search_paths = []
         self.latent_state_index_in_search_path = []
         self.latent_state_index_in_batch = []
         self.last_actions = []
         self.search_lens = []
 
-
 def select_child(
-        root: Node, min_max_stats: MinMaxStats, pb_c_base: float, pb_c_int: float, discount_factor: float,
+        node: Node, min_max_stats: MinMaxStats, pb_c_base: float, pb_c_int: float, discount_factor: float,
         mean_q: float, players: int
 ) -> Union[int, float]:
     """
     Overview:
         Select the child node of the roots according to ucb scores.
     Arguments:
-        - root: the roots to select the child node.
-        - min_max_stats (:obj:`Class MinMaxStats`):  a tool used to min-max normalize the score.
-        - pb_c_base (:obj:`Class Float`): constant c1 used in pUCT rule, typically 1.25.
-        - pb_c_int (:obj:`Class Float`): constant c2 used in pUCT rule, typically 19652.
-        - discount_factor (:obj:`Class Float`): The discount factor used in calculating bootstrapped value, if env is board_games, we set discount_factor=1.
-        - mean_q (:obj:`Class Float`): the mean q value of the parent node.
-        - players (:obj:`Class Int`): the number of players. one/in self-play-mode board games.
+        - node(:obj:`Node`): The root to select the child node.
+        - min_max_stats (:obj:`MinMaxStats`):  A tool used to min-max normalize the score.
+        - pb_c_base (:obj:`float`): Constant c1 used in pUCT rule, typically 1.25.
+        - pb_c_int (:obj:`float`): Constant c2 used in pUCT rule, typically 19652.
+        - discount_factor (:obj:`float`): The discount factor used in calculating bootstrapped value, if env is board_games, we set discount_factor=1.
+        - mean_q (:obj:`float`): The mean q value of the parent node.
+        - players (:obj:`int`): The number of players. In two-player games such as board games, the value need to be negatived when backpropating.
     Returns:
         - action (:obj:`Union[int, float]`): Choose the action with the highest ucb score.
     """
+
+    if node.is_chance:
+        # print("root->is_chance: True ")
+
+        # If the node is chance node, we sample from the prior outcome distribution.
+        outcomes, probs = zip(*[(o, n.prior) for o, n in node.children.items()])
+        outcome = np.random.choice(outcomes, p=probs)
+        # print(outcome, probs)
+        return outcome
+
+    # print("root->is_chance: False ")
+    # If the node is decision node, we select the action with the highest ucb score.
     max_score = -np.inf
     epsilon = 0.000001
     max_index_lst = []
-    for a in root.legal_actions:
-        child = root.get_child(a)
+    for a in node.legal_actions:
+        child = node.get_child(a)
         temp_score = compute_ucb_score(
-            child, min_max_stats, mean_q, root.is_reset, root.visit_count, root.value_prefix, pb_c_base, pb_c_int,
-            discount_factor, players
+            child, min_max_stats, mean_q, node.visit_count, pb_c_base, pb_c_int, discount_factor, players
         )
         if max_score < temp_score:
             max_score = temp_score
             max_index_lst.clear()
             max_index_lst.append(a)
         elif temp_score >= max_score - epsilon:
-            # NOTE: if the difference is less than  epsilon = 0.000001, we random choice action from  max_index_lst
+            # TODO(pu): if the difference is less than epsilon = 0.000001, we random choice action from  max_index_lst
             max_index_lst.append(a)
 
     action = 0
     if len(max_index_lst) > 0:
         action = random.choice(max_index_lst)
     return action
 
 
 def compute_ucb_score(
         child: Node,
         min_max_stats: MinMaxStats,
         parent_mean_q: float,
-        is_reset: int,
         total_children_visit_counts: float,
-        parent_value_prefix: float,
         pb_c_base: float,
         pb_c_init: float,
         discount_factor: float,
         players: int = 1,
 ) -> float:
     """
     Overview:
         Compute the ucb score of the child.
-        Arguments:
-            - child: the child node to compute ucb score.
-            - min_max_stats: a tool used to min-max normalize the score.
-            - parent_mean_q: the mean q value of the parent node.
-            - is_reset: whether the value prefix needs to be reset.
-            - total_children_visit_counts: the total visit counts of the child nodes of the parent node.
-            - parent_value_prefix: the value prefix of parent node.
-            - pb_c_base: constants c2 in muzero.
-            - pb_c_init: constants c1 in muzero.
-            - disount_factor: the discount factor of reward.
-            - players: the number of players.
-        Outputs:
-            - ucb_value: the ucb score of the child.
+    Arguments:
+        - child (:obj:`Node`): the child node to compute ucb score.
+        - min_max_stats (:obj:`MinMaxStats`): a tool used to min-max normalize the score.
+        - parent_mean_q (:obj:`float`): the mean q value of the parent node.
+        - total_children_visit_counts (:obj:`float`): the total visit counts of the child nodes of the parent node.
+        - pb_c_base (:obj:`float`): constants c2 in muzero.
+        - pb_c_init (:obj:`float`): constants c1 in muzero.
+        - disount_factor (:obj:`float`): the discount factor of reward.
+        - players (:obj:`int`): the number of players.
+    Returns:
+        - ucb_value (:obj:`float`): the ucb score of the child.
     """
+    # Compute the prior score.
     pb_c = math.log((total_children_visit_counts + pb_c_base + 1) / pb_c_base) + pb_c_init
     pb_c *= (math.sqrt(total_children_visit_counts) / (child.visit_count + 1))
-
     prior_score = pb_c * child.prior
+
+    # Compute the value score.
     if child.visit_count == 0:
         value_score = parent_mean_q
     else:
-        true_reward = child.value_prefix - parent_value_prefix
-        if is_reset == 1:
-            true_reward = child.value_prefix
+        true_reward = child.reward
         if players == 1:
             value_score = true_reward + discount_factor * child.value
         elif players == 2:
             value_score = true_reward + discount_factor * (-child.value)
 
+    # Normalize the value score.
     value_score = min_max_stats.normalize(value_score)
     if value_score < 0:
         value_score = 0
     if value_score > 1:
         value_score = 1
+    
     ucb_score = prior_score + value_score
 
     return ucb_score
 
 
 def batch_traverse(
         roots: Any,
         pb_c_base: float,
         pb_c_init: float,
         discount_factor: float,
         min_max_stats_lst: List[MinMaxStats],
         results: SearchResults,
         virtual_to_play: List,
-) -> Tuple[List[None], List[None], List[None], Union[list, int]]:
+) -> Tuple[Any, Any]:
+
     """
     Overview:
-        traverse, also called expansion. process a batch roots parallely.
+        traverse, also called expansion. Process a batch roots at once.
     Arguments:
-        - roots (:obj:`Any`): a batch of root nodes to be expanded.
-        - pb_c_base (:obj:`float`): constant c1 used in pUCT rule, typically 1.25.
-        - pb_c_init (:obj:`float`): constant c2 used in pUCT rule, typically 19652.
+        - roots (:obj:`Any`): A batch of root nodes to be expanded.
+        - pb_c_base (:obj:`float`): Constant c1 used in pUCT rule, typically 1.25.
+        - pb_c_init (:obj:`float`): Constant c2 used in pUCT rule, typically 19652.
         - discount_factor (:obj:`float`): The discount factor used in calculating bootstrapped value, if env is board_games, we set discount_factor=1.
-        - virtual_to_play (:obj:`list`): the to_play list used in self_play collecting and training in board games,
+        - results (:obj:`SearchResults`): An instance to record the simulation results for all the roots in the batch.
+        - virtual_to_play (:obj:`list`): The to_play list used in self_play collecting and training in board games,
             `virtual` is to emphasize that actions are performed on an imaginary hidden state.
     Returns:
-        - latent_state_index_in_search_path (:obj:`list`): the list of x/first index of hidden state vector of the searched node, i.e. the search depth.
-        - latent_state_index_in_batch (:obj:`list`): the list of y/second index of hidden state vector of the searched node, i.e. the index of batch root node, its maximum is ``batch_size``/``env_num``.
-        - last_actions (:obj:`list`): the action performed by the previous node.
-        - virtual_to_play (:obj:`list`): the to_play list used in self_play collecting and trainin gin board games,
+        - latent_state_index_in_search_path (:obj:`list`): The list of x/first index of hidden state vector of the searched node, i.e. the search depth.
+        - latent_state_index_in_batch (:obj:`list`): The list of y/second index of hidden state vector of the searched node, i.e. the index of batch root node, its maximum is ``batch_size``/``env_num``.
+        - last_actions (:obj:`list`): The action performed by the previous node.
+        - virtual_to_play (:obj:`list`): The to_play list used in self_play collecting and trainin gin board games,
             `virtual` is to emphasize that actions are performed on an imaginary hidden state.
     """
     parent_q = 0.0
-    results.search_lens = [None for _ in range(results.num)]
-    results.last_actions = [None for _ in range(results.num)]
-    results.nodes = [None for _ in range(results.num)]
-    results.latent_state_index_in_search_path = [None for _ in range(results.num)]
-    results.latent_state_index_in_batch = [None for _ in range(results.num)]
-    results.search_paths = {i: [] for i in range(results.num)}
+    results.search_lens = [None for i in range(results.num)]
+    results.last_actions = [None for i in range(results.num)]
 
-    if isinstance(virtual_to_play, int):
-        if virtual_to_play in [1, 2]:
-            players = 2
-        elif virtual_to_play in [-1, None]:
-            players = 1
-    elif isinstance(virtual_to_play, list):
-        if virtual_to_play[0] in [1, 2]:
-            players = 2
-        elif virtual_to_play[0] in [-1, None]:
-            players = 1
+    results.nodes = [None for i in range(results.num)]
+    results.latent_state_index_in_search_path = [None for i in range(results.num)]
+    results.latent_state_index_in_batch = [None for i in range(results.num)]
+    if virtual_to_play in [1, 2] or virtual_to_play[0] in [1, 2]:
+        players = 2
+    elif virtual_to_play in [-1, None] or virtual_to_play[0] in [-1, None]:
+        players = 1
 
+    results.search_paths = {i: [] for i in range(results.num)}
     for i in range(results.num):
         node = roots.roots[i]
         is_root = 1
         search_len = 0
         results.search_paths[i].append(node)
+
         """
         MCTS stage 1: Selection
-            Each simulation starts from the internal root state s0, and finishes when the simulation reaches a leaf node s_l. 
-            The leaf node is the node that is currently not expanded.
+            Each simulation starts from the internal root state s0, and finishes when the simulation reaches a leaf node s_l.
         """
+        # the leaf node is not expanded
         while node.expanded:
-
             mean_q = node.compute_mean_q(is_root, parent_q, discount_factor)
             is_root = 0
             parent_q = mean_q
 
             # select action according to the pUCT rule.
             action = select_child(
                 node, min_max_stats_lst.stats_lst[i], pb_c_base, pb_c_init, discount_factor, mean_q, players
             )
             if players == 2:
                 # Players play turn by turn
                 if virtual_to_play[i] == 1:
                     virtual_to_play[i] = 2
                 else:
                     virtual_to_play[i] = 1
-            node.best_action = action
 
+            node.best_action = action
             # move to child node according to selected action.
             node = node.get_child(action)
+
             last_action = action
+
             results.search_paths[i].append(node)
             search_len += 1
 
             # note this return the parent node of the current searched node
             parent = results.search_paths[i][len(results.search_paths[i]) - 1 - 1]
-
-            results.latent_state_index_in_search_path[i] = parent.simulation_index
-            results.latent_state_index_in_batch[i] = parent.batch_index
+            results.latent_state_index_in_search_path[i] = parent.latent_state_index_in_search_path
+            results.latent_state_index_in_batch[i] = parent.latent_state_index_in_batch
             results.last_actions[i] = last_action
             results.search_lens[i] = search_len
             # while we break out the while loop, results.nodes[i] save the leaf node.
             results.nodes[i] = node
 
-    return results.latent_state_index_in_search_path, results.latent_state_index_in_batch, results.last_actions, virtual_to_play
+    # print(f'env {i} one simulation done!')
+    return results, virtual_to_play
 
 
 def backpropagate(
         search_path: List[Node], min_max_stats: MinMaxStats, to_play: int, value: float, discount_factor: float
 ) -> None:
     """
     Overview:
         Update the value sum and visit count of nodes along the search path.
     Arguments:
-        - search_path: a vector of nodes on the search path.
-        - min_max_stats: a tool used to min-max normalize the q value.
-        - to_play: which player to play the game in the current node.
-        - value: the value to propagate along the search path.
-        - discount_factor: the discount factor of reward.
+        - search_path (:obj:`List[Node]`): a vector of nodes on the search path.
+        - min_max_stats (:obj:`MinMaxStats`): a tool used to min-max normalize the q value.
+        - to_play (:obj:`int`): which player to play the game in the current node.
+        - value (:obj:`float`): the value to propagate along the search path.
+        - discount_factor (:obj:`float`): the discount factor of reward.
     """
-    assert to_play is None or to_play in [-1, 1, 2], f'to_play is {to_play}!'
+    assert to_play is None or to_play in [-1, 1, 2], to_play
     if to_play is None or to_play == -1:
-        # for play-with-bot-mode
+        # for play-with-bot mode
         bootstrap_value = value
         path_len = len(search_path)
         for i in range(path_len - 1, -1, -1):
             node = search_path[i]
             node.value_sum += bootstrap_value
             node.visit_count += 1
-
-            parent_value_prefix = 0.0
-            is_reset = 0
-            if i >= 1:
-                parent = search_path[i - 1]
-                parent_value_prefix = parent.value_prefix
-                is_reset = parent.is_reset
-
-            true_reward = node.value_prefix - parent_value_prefix
+            true_reward = node.reward
             min_max_stats.update(true_reward + discount_factor * node.value)
-            if is_reset == 1:
-                true_reward = node.value_prefix
             bootstrap_value = true_reward + discount_factor * bootstrap_value
     else:
         # for self-play-mode
         bootstrap_value = value
         path_len = len(search_path)
         for i in range(path_len - 1, -1, -1):
             node = search_path[i]
-
+            # to_play related
             node.value_sum += bootstrap_value if node.to_play == to_play else -bootstrap_value
 
             node.visit_count += 1
-            parent_value_prefix = 0.0
-            is_reset = 0
-            if i >= 1:
-                parent = search_path[i - 1]
-                parent_value_prefix = parent.value_prefix
-                is_reset = parent.is_reset
-
-            # NOTE: in self-play-mode, value_prefix is not calculated according to the perspective of current player of node.
-            # TODO: true_reward = node.value_prefix - (- parent_value_prefix)
-            true_reward = node.value_prefix - parent_value_prefix
 
-            if is_reset == 1:
-                true_reward = node.value_prefix
+            # NOTE: in self-play-mode,
+            # we should calculate the true_reward according to the perspective of current player of node
+            # true_reward = node.value_prefix - (- parent_value_prefix)
+            true_reward = node.reward
 
+            # min_max_stats.update(true_reward + discount_factor * node.value)
             min_max_stats.update(true_reward + discount_factor * -node.value)
 
+            # TODO(pu): to_play related
             # true_reward is in the perspective of current player of node
-            bootstrap_value = (
-                -true_reward if node.to_play == to_play else true_reward
-            ) + discount_factor * bootstrap_value
+            bootstrap_value = (-true_reward if node.to_play == to_play else true_reward) + discount_factor * bootstrap_value
 
 
 def batch_backpropagate(
-        simulation_index: int,
+        latent_state_index_in_search_path: int,
         discount_factor: float,
-        value_prefixs: List,
+        value_prefixs: List[float],
         values: List[float],
         policies: List[float],
         min_max_stats_lst: List[MinMaxStats],
         results: SearchResults,
-        is_reset_list: List,
         to_play: list = None,
+        is_chance_list: list = None,
+        leaf_idx_list: list = None,
 ) -> None:
     """
     Overview:
-        Backpropagation along the search path to update the attributes.
+        Update the value sum and visit count of nodes along the search paths for each root in the batch.
     Arguments:
-        - simulation_index (:obj:`Class Int`): The index of latent state of the leaf node in the search path.
-        - discount_factor (:obj:`Class Float`): The discount factor used in calculating bootstrapped value, if env is board_games, we set discount_factor=1.
-        - value_prefixs (:obj:`Class List`): the value prefixs of nodes along the search path.
-        - values (:obj:`Class List`):  the values to propagate along the search path.
-        - policies (:obj:`Class List`): the policy logits of nodes along the search path.
-        - min_max_stats_lst (:obj:`Class List[MinMaxStats]`):  a tool used to min-max normalize the q value.
-        - results (:obj:`Class List`): the search results.
-        - is_reset_list (:obj:`Class List`): the vector of is_reset nodes along the search path, where is_reset represents for whether the parent value prefix needs to be reset.
-        - to_play (:obj:`Class List`):  the batch of which player is playing on this node.
-    """
-    for i in range(results.num):
+        - latent_state_index_in_search_path (:obj:`int`): the index of latent state vector.
+        - discount_factor (:obj:`float`): discount_factor factor used i calculating bootstrapped value,
+            if env is board_games, we set discount_factor=1.
+        - value_prefixs (:obj:`List`): the value prefixs of nodes along the search path.
+        - values (:obj:`List`):  the values to propagate along the search path.
+        - policies (:obj:`List`): the policy logits of nodes along the search path.
+        - min_max_stats_lst (:obj:`List[MinMaxStats]`):  a tool used to min-max normalize the q value.
+        - results (:obj:`List`): the search results.
+        - to_play (:obj:`List`):  the batch of which player is playing on this node.
+    """
+    if leaf_idx_list is None:
+        leaf_idx_list = list(range(results.num))
+    for leaf_order, i in enumerate(leaf_idx_list):
         # ****** expand the leaf node ******
-        if to_play in [-1, None]:
-            # set to_play=-1, because in self-play-mode to_play = {1,2}
-            results.nodes[i].expand(-1, simulation_index, i, value_prefixs[i], policies[i])
+        if to_play is None:
+            # set to_play=-1, because two_player mode to_play = {1,2}
+            results.nodes[i].expand(-1, latent_state_index_in_search_path, i, value_prefixs[leaf_order], policies[leaf_order], is_chance_list[i])
         else:
-            results.nodes[i].expand(to_play[i], simulation_index, i, value_prefixs[i], policies[i])
-
-        # reset
-        results.nodes[i].is_reset = is_reset_list[i]
+            results.nodes[i].expand(to_play[i], latent_state_index_in_search_path, i, value_prefixs[leaf_order], policies[leaf_order], is_chance_list[i])
 
         # ****** backpropagate ******
-        if to_play in [-1, None]:
-            backpropagate(results.search_paths[i], min_max_stats_lst.stats_lst[i], -1, values[i], discount_factor)
+        if to_play is None:
+            backpropagate(results.search_paths[i], min_max_stats_lst.stats_lst[i], 0, values[leaf_order], discount_factor)
         else:
             backpropagate(
-                results.search_paths[i], min_max_stats_lst.stats_lst[i], to_play[i], values[i], discount_factor
+                results.search_paths[i], min_max_stats_lst.stats_lst[i], to_play[i], values[leaf_order], discount_factor
             )
```

### Comparing `LightZero-0.0.2/lzero/mcts/ptree/ptree_mz.py` & `LightZero-0.0.5/lzero/mcts/ptree/ptree_mz.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,44 +9,54 @@
 import torch
 
 from .minimax import MinMaxStats
 
 
 class Node:
     """
-     Overview:
-        The base class of Node for MuZero.
-     """
+    Overview:
+        The Node class for MuZero. The basic functions of the node are implemented.
+    Interfaces:
+        ``__init__``, ``expand``, ``add_exploration_noise``, ``compute_mean_q``, ``get_trajectory``, \
+        ``get_children_distribution``, ``get_child``, ``expanded``, ``value``.
+    """
     def __init__(self, prior: float, legal_actions: List = None, action_space_size: int = 9) -> None:
+        """
+        Overview:
+            Initializes a Node instance.
+        Arguments:
+            - prior (:obj:`float`): The prior probability of the node.
+            - legal_actions (:obj:`List`, optional): The list of legal actions of the node. Defaults to None.
+            - action_space_size (:obj:`int`, optional): The size of the action space. Defaults to 9.
+        """
         self.prior = prior
         self.legal_actions = legal_actions
         self.action_space_size = action_space_size
         self.visit_count = 0
         self.value_sum = 0
         self.best_action = -1
         self.to_play = -1  # default -1 means play_with_bot_mode
         self.reward = 0
         self.value_prefix = 0.0
         self.children = {}
         self.children_index = []
         self.simulation_index = 0
         self.batch_index = 0
-        self.parent_value_prefix = 0  # only used in update_tree_q method
 
     def expand(self, to_play: int, simulation_index: int, batch_index: int, reward: float,
                policy_logits: List[float]) -> None:
         """
         Overview:
             Expand the child nodes of the current node.
         Arguments:
-            - to_play (:obj:`Class int`): which player to play the game in the current node.
-            - simulation_index (:obj:`Class int`): the x/first index of hidden state vector of the current node, i.e. the search depth.
-            - batch_index (:obj:`Class int`): the y/second index of hidden state vector of the current node, i.e. the index of batch root node, its maximum is ``batch_size``/``env_num``.
-            - value_prefix: (:obj:`Class float`): the value prefix of the current node.
-            - policy_logits: (:obj:`Class List`): the policy logit of the child nodes.
+            - to_play (:obj:`int`): The player to play the game in the current node.
+            - simulation_index (:obj:`int`): The x/first index of the hidden state vector of the current node, i.e., the search depth.
+            - batch_index (:obj:`int`): The y/second index of the hidden state vector of the current node, i.e., the index of the batch root node, its maximum is `batch_size`/`env_num`.
+            - reward (:obj:`float`): The reward associated with the current node.
+            - policy_logits (:obj:`List[float]`): The policy logits providing the priors for the child nodes.
         """
         self.to_play = to_play
         if self.legal_actions is None:
             self.legal_actions = np.arange(len(policy_logits))
 
         self.simulation_index = simulation_index
         self.batch_index = batch_index
@@ -56,40 +66,44 @@
         policy = {a: policy_values[i] for i, a in enumerate(self.legal_actions)}
         for action, prior in policy.items():
             self.children[action] = Node(prior)
 
     def add_exploration_noise(self, exploration_fraction: float, noises: List[float]) -> None:
         """
         Overview:
-            add exploration noise to priors
+            Add exploration noise to the priors.
         Arguments:
-            - noises (:obj: list): length is len(self.legal_actions)
+            - exploration_fraction (:obj:`float`): The fraction of exploration noise to be added.
+            - noises (:obj:`List[float]`): The list of noises to be added to the priors.
         """
         for i, a in enumerate(self.legal_actions):
             """
             i in index, a is action, e.g. self.legal_actions = [0,1,2,4,6,8], i=[0,1,2,3,4,5], a=[0,1,2,4,6,8]
             """
             noise = noises[i]
             child = self.get_child(a)
             prior = child.prior
             child.prior = prior * (1 - exploration_fraction) + noise * exploration_fraction
 
-    def compute_mean_q(self, is_root: int, parent_q: float, discount_factor: float) -> float:
+    def compute_mean_q(self, is_root: bool, parent_q: float, discount_factor: float) -> float:
         """
         Overview:
-            Compute the mean q value of the current node.
+            Compute the mean of the action values of all legal actions.
         Arguments:
-            - is_root (:obj:`int`): whether the current node is a root node.
-            - parent_q (:obj:`float`): the q value of the parent node.
-            - discount_factor (:obj:`float`): the discount_factor of reward.
+            - is_root (:obj:`bool`): Whether the current node is a root node.
+            - parent_q (:obj:`float`): The q value of the parent node.
+            - discount_factor (:obj:`float`): The discount factor of the reward.
+        Returns:
+            - mean_q (:obj:`float`): The mean of the action values.
         """
         total_unsigned_q = 0.0
         total_visits = 0
         for a in self.legal_actions:
             child = self.get_child(a)
+            # Only count the child nodes which have been visited.
             if child.visit_count > 0:
                 true_reward = child.reward
                 # TODO(pu): why only one step bootstrap?
                 q_of_s_a = true_reward + discount_factor * child.value
                 total_unsigned_q += q_of_s_a
                 total_visits += 1
         if is_root and total_visits > 0:
@@ -98,67 +112,100 @@
             # TODO(pu): why parent_q?
             mean_q = (parent_q + total_unsigned_q) / (total_visits + 1)
         return mean_q
 
     def get_trajectory(self) -> List[Union[int, float]]:
         """
         Overview:
-            Find the current best trajectory starts from the current node.
-        Outputs:
-            - traj: a vector of node index, which is the current best trajectory from this node.
+            Find the current best trajectory starting from the current node.
+        Returns:
+            - traj (:obj:`List[Union[int, float]]`): A vector of node indices representing the current best trajectory.
         """
         traj = []
         node = self
         best_action = node.best_action
         while best_action >= 0:
             traj.append(best_action)
             node = node.get_child(best_action)
             best_action = node.best_action
         return traj
 
     def get_children_distribution(self) -> List[Union[int, float]]:
+        """
+        Overview:
+            Get the distribution of visit counts among the child nodes.
+        Returns:
+            - distribution (:obj:`List[Union[int, float]]` or :obj:`None`): The distribution of visit counts among the children nodes. \
+              If the legal_actions list is empty, returns None.
+        """
         if self.legal_actions == []:
             return None
         distribution = {a: 0 for a in self.legal_actions}
         if self.expanded:
             for a in self.legal_actions:
                 child = self.get_child(a)
                 distribution[a] = child.visit_count
             # only take the visit counts
             distribution = [v for k, v in distribution.items()]
         return distribution
 
     def get_child(self, action: Union[int, float]) -> "Node":
         """
         Overview:
-            get children node according to the input action.
+            Get the child node according to the input action.
+        Arguments:
+            - action (:obj:`Union[int, float]`): The action for which the child node is to be retrieved.
+        Returns:
+            - child (:obj:`Node`): The child node corresponding to the input action.
         """
         if not isinstance(action, np.int64):
             action = int(action)
         return self.children[action]
 
     @property
     def expanded(self) -> bool:
+        """
+        Overview:
+            Check if the node has been expanded.
+        Returns:
+            - expanded (:obj:`bool`): True if the node has been expanded, False otherwise.
+        """
         return len(self.children) > 0
 
     @property
     def value(self) -> float:
         """
         Overview:
-            Return the estimated value of the current root node.
+            Return the estimated value of the current node.
+        Returns:
+            - value (:obj:`float`): The estimated value of the current node.
         """
         if self.visit_count == 0:
             return 0
         else:
             return self.value_sum / self.visit_count
 
 
 class Roots:
+    """
+    Overview:
+        The class to process a batch of roots(Node instances) at the same time.
+    Interfaces:
+        ``__init__``, ``prepare``,  ``prepare_no_noise``, ``clear``, ``get_trajectories``, \
+        ``get_distributions``, ``get_values``
+    """
 
     def __init__(self, root_num: int, legal_actions_list: List) -> None:
+        """
+        Overview:
+            Initializes an instance of the Roots class with the specified number of roots and legal actions.
+        Arguments:
+            - root_num (:obj:`int`): The number of roots.
+            - legal_actions_list(:obj:`List`): A list of the legal actions for each root.
+        """
         self.num = root_num
         self.root_num = root_num
         self.legal_actions_list = legal_actions_list  # list of list
 
         self.roots = []
         for i in range(self.root_num):
             if isinstance(legal_actions_list, list):
@@ -172,22 +219,21 @@
             noises: List[float],
             rewards: List[float],
             policies: List[List[float]],
             to_play: int = -1
     ) -> None:
         """
         Overview:
-            Expand the roots and add noises.
+            Expand the roots and add noises for exploration.
         Arguments:
-            - root_noise_weight: the exploration fraction of roots
-            - noises: the vector of noise add to the roots.
-            - rewards: the vector of rewards of each root.
-            - policies: the vector of policy logits of each root.
-            - to_play_batch: the vector of the player side of each root.
-
+            - root_noise_weight (:obj:`float`): the exploration fraction of roots
+            - noises (:obj:`List[float]`): the vector of noise add to the roots.
+            - rewards (:obj:`List[float]`): the vector of rewards of each root.
+            - policies (:obj:`List[List[float]]`): the vector of policy logits of each root.
+            - to_play(:obj:`List`): The vector of the player side of each root.
         """
         for i in range(self.root_num):
             if to_play is None:
                 self.roots[i].expand(-1, 0, i, rewards[i], policies[i])
             else:
                 self.roots[i].expand(to_play[i], 0, i, rewards[i], policies[i])
 
@@ -195,124 +241,110 @@
             self.roots[i].visit_count += 1
 
     def prepare_no_noise(self, rewards: List[float], policies: List[List[float]], to_play: int = -1) -> None:
         """
         Overview:
             Expand the roots without noise.
         Arguments:
-            - rewards: the vector of rewards of each root.
-            - policies: the vector of policy logits of each root.
-            - to_play_batch: the vector of the player side of each root.
+            - rewards (:obj:`List[float]`): the vector of rewards of each root.
+            - policies (:obj:`List[List[float]]`): the vector of policy logits of each root.
+            - to_play(:obj:`List`): The vector of the player side of each root.
         """
         for i in range(self.root_num):
             if to_play is None:
                 self.roots[i].expand(-1, 0, i, rewards[i], policies[i])
             else:
                 self.roots[i].expand(to_play[i], 0, i, rewards[i], policies[i])
 
             self.roots[i].visit_count += 1
 
     def clear(self) -> None:
+        """
+        Overview:
+            Clear all the roots in the list.
+        """
         self.roots.clear()
 
     def get_trajectories(self) -> List[List[Union[int, float]]]:
         """
         Overview:
             Find the current best trajectory starts from each root.
-        Outputs:
-            - traj: a vector of node index, which is the current best trajectory from each root.
+        Returns:
+            - traj (:obj:`List[List[Union[int, float]]]`): a vector of node index, which is the current best trajectory from each root.
         """
         trajs = []
         for i in range(self.root_num):
             trajs.append(self.roots[i].get_trajectory())
         return trajs
 
     def get_distributions(self) -> List[List[Union[int, float]]]:
         """
         Overview:
-            Get the children distribution of each root.
-        Outputs:
-            - distribution: a vector of distribution of child nodes in the format of visit count (i.e. [1,3,0,2,5]).
+            Get the visit count distribution of child nodes for each root.
+        Returns:
+            - distribution (:obj:`List[List[Union[int, float]]]`): a vector of distribution of child nodes in the format of visit count (i.e. [1,3,0,2,5]).
         """
         distributions = []
         for i in range(self.root_num):
             distributions.append(self.roots[i].get_children_distribution())
 
         return distributions
 
-    def get_values(self) -> float:
+    def get_values(self) -> List[float]:
         """
         Overview:
-            Return the estimated value of each root.
+            Get the estimated value of each root.
+        Returns:
+            - values (:obj:`List[float]`): The estimated value of each root.
         """
         values = []
         for i in range(self.root_num):
             values.append(self.roots[i].value)
         return values
 
 
 class SearchResults:
+    """
+    Overview:
+        The class to record the results of the simulations for the batch of roots.
+    Interfaces:
+        ``__init__``.
+    """
 
     def __init__(self, num: int) -> None:
+        """
+        Overview:
+            Initiaizes the attributes to be recorded.
+        Arguments:
+            -num (:obj:`int`): The number of search results(equal to ``batch_size``).
+        """
         self.num = num
         self.nodes = []
         self.search_paths = []
         self.latent_state_index_in_search_path = []
         self.latent_state_index_in_batch = []
         self.last_actions = []
         self.search_lens = []
 
 
-def update_tree_q(root: Node, min_max_stats: MinMaxStats, discount_factor: float, players: int = 1) -> None:
-    """
-    Overview:
-        Update the value sum and visit count of nodes along the search path.
-    Arguments:
-        - search_path: a vector of nodes on the search path.
-        - min_max_stats: a tool used to min-max normalize the q value.
-        - to_play: which player to play the game in the current node.
-        - value: the value to propagate along the search path.
-        - discount_factor: the discount factor of reward.
-    """
-    node_stack = []
-    node_stack.append(root)
-    while len(node_stack) > 0:
-        node = node_stack[-1]
-        node_stack.pop()
-
-        if node != root:
-            true_reward = node.reward
-            if players == 1:
-                q_of_s_a = true_reward + discount_factor * node.value
-            elif players == 2:
-                q_of_s_a = true_reward + discount_factor * (-node.value)
-
-            min_max_stats.update(q_of_s_a)
-
-        for a in node.legal_actions:
-            child = node.get_child(a)
-            if child.expanded:
-                node_stack.append(child)
-
-
 def select_child(
         root: Node, min_max_stats: MinMaxStats, pb_c_base: float, pb_c_int: float, discount_factor: float,
         mean_q: float, players: int
 ) -> Union[int, float]:
     """
     Overview:
         Select the child node of the roots according to ucb scores.
     Arguments:
-        - root: the roots to select the child node.
-        - min_max_stats (:obj:`Class MinMaxStats`):  a tool used to min-max normalize the score.
-        - pb_c_base (:obj:`Class Float`): constant c1 used in pUCT rule, typically 1.25.
-        - pb_c_int (:obj:`Class Float`): constant c2 used in pUCT rule, typically 19652.
-        - discount_factor (:obj:`Class Float`): The discount factor used in calculating bootstrapped value, if env is board_games, we set discount_factor=1.
-        - mean_q (:obj:`Class Float`): the mean q value of the parent node.
-        - players (:obj:`Class Int`): the number of players. one/in self-play-mode board games.
+        - root(:obj:`Node`): The root to select the child node.
+        - min_max_stats (:obj:`MinMaxStats`):  A tool used to min-max normalize the score.
+        - pb_c_base (:obj:`float`): Constant c1 used in pUCT rule, typically 1.25.
+        - pb_c_int (:obj:`float`): Constant c2 used in pUCT rule, typically 19652.
+        - discount_factor (:obj:`float`): The discount factor used in calculating bootstrapped value, if env is board_games, we set discount_factor=1.
+        - mean_q (:obj:`float`): The mean q value of the parent node.
+        - players (:obj:`int`): The number of players. In two-player games such as board games, the value need to be negatived when backpropating.
     Returns:
         - action (:obj:`Union[int, float]`): Choose the action with the highest ucb score.
     """
     max_score = -np.inf
     epsilon = 0.000001
     max_index_lst = []
     for a in root.legal_actions:
@@ -343,77 +375,78 @@
         pb_c_init: float,
         discount_factor: float,
         players: int = 1,
 ) -> float:
     """
     Overview:
         Compute the ucb score of the child.
-        Arguments:
-            - child: the child node to compute ucb score.
-            - min_max_stats: a tool used to min-max normalize the score.
-            - parent_mean_q: the mean q value of the parent node.
-            - is_reset: whether the value prefix needs to be reset.
-            - total_children_visit_counts: the total visit counts of the child nodes of the parent node.
-            - parent_value_prefix: the value prefix of parent node.
-            - pb_c_base: constants c2 in muzero.
-            - pb_c_init: constants c1 in muzero.
-            - disount_factor: the discount factor of reward.
-            - players: the number of players.
-            - continuous_action_space: whether the action space is continuous in current env.
-        Outputs:
-            - ucb_value: the ucb score of the child.
+    Arguments:
+        - child (:obj:`Node`): the child node to compute ucb score.
+        - min_max_stats (:obj:`MinMaxStats`): a tool used to min-max normalize the score.
+        - parent_mean_q (:obj:`float`): the mean q value of the parent node.
+        - total_children_visit_counts (:obj:`float`): the total visit counts of the child nodes of the parent node.
+        - pb_c_base (:obj:`float`): constants c2 in muzero.
+        - pb_c_init (:obj:`float`): constants c1 in muzero.
+        - disount_factor (:obj:`float`): the discount factor of reward.
+        - players (:obj:`int`): the number of players.
+    Returns:
+        - ucb_value (:obj:`float`): the ucb score of the child.
     """
+    # Compute the prior score.
     pb_c = math.log((total_children_visit_counts + pb_c_base + 1) / pb_c_base) + pb_c_init
     pb_c *= (math.sqrt(total_children_visit_counts) / (child.visit_count + 1))
-
     prior_score = pb_c * child.prior
+
+    # Compute the value score.
     if child.visit_count == 0:
         value_score = parent_mean_q
     else:
         true_reward = child.reward
         if players == 1:
             value_score = true_reward + discount_factor * child.value
         elif players == 2:
             value_score = true_reward + discount_factor * (-child.value)
 
+    # Normalize the value score.
     value_score = min_max_stats.normalize(value_score)
     if value_score < 0:
         value_score = 0
     if value_score > 1:
         value_score = 1
+    
     ucb_score = prior_score + value_score
 
     return ucb_score
 
 
 def batch_traverse(
         roots: Any,
         pb_c_base: float,
         pb_c_init: float,
         discount_factor: float,
         min_max_stats_lst: List[MinMaxStats],
         results: SearchResults,
         virtual_to_play: List,
-) -> Tuple[List[None], List[None], List[None], list]:
+) -> Tuple[List[None], List[None], List[None], Union[list, int]]:
     """
     Overview:
-        traverse, also called expansion. process a batch roots parallelly.
+        traverse, also called expansion. Process a batch roots at once.
     Arguments:
-        - roots (:obj:`Any`): a batch of root nodes to be expanded.
-        - pb_c_base (:obj:`float`): constant c1 used in pUCT rule, typically 1.25.
-        - pb_c_init (:obj:`float`): constant c2 used in pUCT rule, typically 19652.
+        - roots (:obj:`Any`): A batch of root nodes to be expanded.
+        - pb_c_base (:obj:`float`): Constant c1 used in pUCT rule, typically 1.25.
+        - pb_c_init (:obj:`float`): Constant c2 used in pUCT rule, typically 19652.
         - discount_factor (:obj:`float`): The discount factor used in calculating bootstrapped value, if env is board_games, we set discount_factor=1.
-        - virtual_to_play (:obj:`list`): the to_play list used in self_play collecting and training in board games,
+        - results (:obj:`SearchResults`): An instance to record the simulation results for all the roots in the batch.
+        - virtual_to_play (:obj:`list`): The to_play list used in self_play collecting and training in board games,
             `virtual` is to emphasize that actions are performed on an imaginary hidden state.
-        - continuous_action_space: whether the action space is continuous in current env.
     Returns:
-        - latent_state_index_in_search_path (:obj:`list`): the list of x/first index of hidden state vector of the searched node, i.e. the search depth.
-        - latent_state_index_in_batch (:obj:`list`): the list of y/second index of hidden state vector of the searched node, i.e. the index of batch root node, its maximum is ``batch_size``/``env_num``.
-        - last_actions (:obj:`list`): the action performed by the previous node.
-        - virtual_to_play (:obj:`list`): the to_play list used in self_play collecting and trainin gin board games,
+        - latent_state_index_in_search_path (:obj:`list`): The list of x/first index of hidden state vector of the searched node, i.e. the search depth.
+        - latent_state_index_in_batch (:obj:`list`): The list of y/second index of hidden state vector of the searched node, i.e. the index of batch root node, its maximum is ``batch_size``/``env_num``.
+        - last_actions (:obj:`list`): The action performed by the previous node.
+        - virtual_to_play (:obj:`list`): The to_play list used in self_play collecting and trainin gin board games,
             `virtual` is to emphasize that actions are performed on an imaginary hidden state.
     """
     parent_q = 0.0
     results.search_lens = [None for _ in range(results.num)]
     results.last_actions = [None for _ in range(results.num)]
 
     results.nodes = [None for _ in range(results.num)]
@@ -477,19 +510,19 @@
 def backpropagate(
         search_path: List[Node], min_max_stats: MinMaxStats, to_play: int, value: float, discount_factor: float
 ) -> None:
     """
     Overview:
         Update the value sum and visit count of nodes along the search path.
     Arguments:
-        - search_path: a vector of nodes on the search path.
-        - min_max_stats: a tool used to min-max normalize the q value.
-        - to_play: which player to play the game in the current node.
-        - value: the value to propagate along the search path.
-        - discount_factor: the discount factor of reward.
+        - search_path (:obj:`List[Node]`): a vector of nodes on the search path.
+        - min_max_stats (:obj:`MinMaxStats`): a tool used to min-max normalize the q value.
+        - to_play (:obj:`int`): which player to play the game in the current node.
+        - value (:obj:`float`): the value to propagate along the search path.
+        - discount_factor (:obj:`float`): the discount factor of reward.
     """
     assert to_play is None or to_play in [-1, 1, 2], to_play
     if to_play is None or to_play == -1:
         # for play-with-bot-mode
         bootstrap_value = value
         path_len = len(search_path)
         for i in range(path_len - 1, -1, -1):
@@ -536,24 +569,24 @@
         policies: List[float],
         min_max_stats_lst: List[MinMaxStats],
         results: SearchResults,
         to_play: list = None
 ) -> None:
     """
     Overview:
-        Backpropagation along the search path to update the attributes.
+        Update the value sum and visit count of nodes along the search paths for each root in the batch.
     Arguments:
-        - simulation_index (:obj:`Class Int`): The index of latent state of the leaf node in the search path.
-        - discount_factor (:obj:`Class Float`): The discount factor used in calculating bootstrapped value, if env is board_games, we set discount_factor=1.
-        - value_prefixs (:obj:`Class List`): the value prefixs of nodes along the search path.
-        - values (:obj:`Class List`):  the values to propagate along the search path.
-        - policies (:obj:`Class List`): the policy logits of nodes along the search path.
-        - min_max_stats_lst (:obj:`Class List[MinMaxStats]`):  a tool used to min-max normalize the q value.
-        - results (:obj:`Class List`): the search results.
-        - to_play (:obj:`Class List`): the batch of which player is playing on this node.
+        - simulation_index (:obj:`int`): The index of latent state of the leaf node in the search path.
+        - discount_factor (:obj:`float`): The discount factor used in calculating bootstrapped value, if env is board_games, we set discount_factor=1.
+        - value_prefixs (:obj:`List`): the value prefixs of nodes along the search path.
+        - values (:obj:`List`):  the values to propagate along the search path.
+        - policies (:obj:`List`): the policy logits of nodes along the search path.
+        - min_max_stats_lst (:obj:`List[MinMaxStats]`):  a tool used to min-max normalize the q value.
+        - results (:obj:`List`): the search results.
+        - to_play (:obj:`List`): the batch of which player is playing on this node.
     """
     for i in range(results.num):
         # ****** expand the leaf node ******
         if to_play is None:
             # set to_play=-1, because in self-play-mode to_play = {1,2}
             results.nodes[i].expand(-1, simulation_index, i, value_prefixs[i], policies[i])
         else:
```

### Comparing `LightZero-0.0.2/lzero/mcts/ptree/ptree_sez.py` & `LightZero-0.0.5/lzero/mcts/ptree/ptree_sez.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,26 +10,39 @@
 from torch.distributions import Normal, Independent
 
 from .minimax import MinMaxStats
 
 
 class Node:
     """
-     Overview:
-         the node base class for Sampled EfficientZero.
-     """
+    Overview:
+        The Node class for  Sampled EfficientZero. The basic functions of the node are implemented.
+    Interfaces:
+        ``__init__``, ``expand``, ``add_exploration_noise``, ``compute_mean_q``, ``get_trajectory``, \
+        ``get_children_distribution``, ``get_child``, ``expanded``, ``value``.
+    """
 
     def __init__(
             self,
             prior: Union[list, float],
             legal_actions: List = None,
             action_space_size: int = 9,
             num_of_sampled_actions: int = 20,
             continuous_action_space: bool = False,
     ) -> None:
+        """
+        Overview:
+            Initializes a Node instance.
+        Arguments:
+            - prior (:obj:`float`): The prior probability of the node.
+            - legal_actions (:obj:`List`, optional): The list of legal actions of the node. Defaults to None.
+            - action_space_size (:obj:`int`, optional): The size of the action space. Defaults to 9.
+            - num_of_sampled_actions (:obj:`int`): The number of sampled actions, i.e. K in the Sampled MuZero paper.
+            - continuous_action_space (:obj:'bool'): Whether the action space is continous in current env.
+        """
         self.prior = prior
         self.mu = None
         self.sigma = None
         self.legal_actions = legal_actions
         self.action_space_size = action_space_size
         self.num_of_sampled_actions = num_of_sampled_actions
         self.continuous_action_space = continuous_action_space
@@ -48,19 +61,19 @@
     def expand(
             self, to_play: int, simulation_index: int, batch_index: int, value_prefix: float, policy_logits: List[float]
     ) -> None:
         """
         Overview:
             Expand the child nodes of the current node.
         Arguments:
-            - to_play (:obj:`Class int`): which player to play the game in the current node.
-            - simulation_index (:obj:`Class int`): the x/first index of hidden state vector of the current node, i.e. the search depth.
-            - batch_index (:obj:`Class int`): the y/second index of hidden state vector of the current node, i.e. the index of batch root node, its maximum is ``batch_size``/``env_num``.
-            - value_prefix: (:obj:`Class float`): the value prefix of the current node.
-            - policy_logits: (:obj:`Class List`): the policy logit of the child nodes.
+            - to_play (:obj:`int`): The player to play the game in the current node.
+            - simulation_index (:obj:`int`): The x/first index of the hidden state vector of the current node, i.e., the search depth.
+            - batch_index (:obj:`int`): The y/second index of the hidden state vector of the current node, i.e., the index of the batch root node, its maximum is `batch_size`/`env_num`.
+            - value_prefix: (:obj:`float`): the value prefix of the current node.
+            - policy_logits (:obj:`List[float]`): The policy logits providing the priors for the child nodes.
         """
         """
         to varify ctree_efficientzero:
             import numpy as np
             import torch
             from torch.distributions import Normal, Independent
             mu= torch.tensor([0.1,0.1])
@@ -150,18 +163,18 @@
             else:
                 # probs is prob
                 policy_logits[i] = policy_logits[i] * (1 - exploration_fraction) + noises[i] * exploration_fraction
 
     def add_exploration_noise(self, exploration_fraction: float, noises: List[float]) -> None:
         """
         Overview:
-            Add a noise to the prior of the child nodes.
+            Add exploration noise to the priors of the child nodes..
         Arguments:
-            - exploration_fraction: the fraction to add noise.
-            - noises (:obj: list): the vector of noises added to each child node. length is len(self.legal_actions)
+            - exploration_fraction (:obj:`float`): The fraction of exploration noise to be added.
+            - noises (:obj:`List[float]`): The list of noises to be added to the priors. Length is ``len(self.legal_actions)``.
         """
         # ==============================================================
         # sampled related core code
         # ==============================================================
         actions = list(self.children.keys())
         for a, n in zip(actions, noises):
             if self.continuous_action_space:
@@ -172,19 +185,21 @@
             else:
                 # prior is prob
                 self.children[a].prior = self.children[a].prior * (1 - exploration_fraction) + n * exploration_fraction
 
     def compute_mean_q(self, is_root: int, parent_q: float, discount_factor: float) -> float:
         """
         Overview:
-            Compute the mean q value of the current node.
+            Compute the mean of the action values of all legal actions.
         Arguments:
-            - is_root (:obj:`int`): whether the current node is a root node.
-            - parent_q (:obj:`float`): the q value of the parent node.
-            - discount_factor (:obj:`float`): the discount_factor of reward.
+            - is_root (:obj:`bool`): Whether the current node is a root node.
+            - parent_q (:obj:`float`): The q value of the parent node.
+            - discount_factor (:obj:`float`): The discount factor of the reward.
+        Returns:
+            - mean_q (:obj:`float`): The mean of the action values.
         """
         total_unsigned_q = 0.0
         total_visits = 0
         parent_value_prefix = self.value_prefix
         for a in self.legal_actions:
             child = self.get_child(a)
             if child.visit_count > 0:
@@ -205,28 +220,35 @@
 
     def print_out(self) -> None:
         pass
 
     def get_trajectory(self) -> List[Union[int, float]]:
         """
         Overview:
-            Find the current best trajectory starts from the current node.
-        Outputs:
-            - traj: a vector of node index, which is the current best trajectory from this node.
+            Find the current best trajectory starting from the current node.
+        Returns:
+            - traj (:obj:`List[Union[int, float]]`): A vector of node indices representing the current best trajectory.
         """
         traj = []
         node = self
         best_action = node.best_action
         while best_action >= 0:
             traj.append(best_action)
             node = node.get_child(best_action)
             best_action = node.best_action
         return traj
 
     def get_children_distribution(self) -> List[Union[int, float]]:
+        """
+        Overview:
+            Get the distribution of visit counts among the child nodes.
+        Returns:
+            - distribution (:obj:`List[Union[int, float]]` or :obj:`None`): The distribution of visit counts among the children nodes. \
+              If the legal_actions list is empty, returns None.
+        """
         if self.legal_actions == []:
             return None
         # distribution = {a: 0 for a in self.legal_actions}
         distribution = {}
         if self.expanded:
             for a in self.legal_actions:
                 child = self.get_child(a)
@@ -234,48 +256,76 @@
             # only take the visit counts
             distribution = [v for k, v in distribution.items()]
         return distribution
 
     def get_child(self, action: Union[int, float]) -> "Node":
         """
         Overview:
-            get children node according to the input action.
+            Get the child node according to the input action.
+        Arguments:
+            - action (:obj:`Union[int, float]`): The action for which the child node is to be retrieved.
+        Returns:
+            - child (:obj:`Node`): The child node corresponding to the input action.
         """
         if isinstance(action, Action):
             return self.children[action]
         if not isinstance(action, np.int64):
             action = int(action)
         return self.children[action]
 
     @property
     def expanded(self) -> bool:
+        """
+        Overview:
+            Check if the node has been expanded.
+        Returns:
+            - expanded (:obj:`bool`): True if the node has been expanded, False otherwise.
+        """
         return len(self.children) > 0
 
     @property
     def value(self) -> float:
         """
         Overview:
-            Return the estimated value of the current root node.
+            Return the estimated value of the current node.
+        Returns:
+            - value (:obj:`float`): The estimated value of the current node.
         """
         if self.visit_count == 0:
             return 0
         else:
             return self.value_sum / self.visit_count
 
 
 class Roots:
-
+    """
+    Overview:
+        The class to process a batch of roots(Node instances) at the same time.
+    Interfaces:
+        ``__init__``, ``prepare``,  ``prepare_no_noise``, ``clear``, ``get_trajectories``, \
+        ``get_distributions``, ``get_values``
+    """
     def __init__(
             self,
             root_num: int,
             legal_actions_list: List,
             action_space_size: int = 9,
             num_of_sampled_actions: int = 20,
             continuous_action_space: bool = False,
     ) -> None:
+        """
+        Overview:
+            Initializes an instance of the Roots class with the specified number of roots and legal actions.
+        Arguments:
+            - root_num (:obj:`int`): The number of roots.
+            - legal_actions_list(:obj:`List`): A list of the legal actions for each root.
+            - action_space_size (:obj:'int'): the size of action space of the current env.
+            - num_of_sampled_actions (:obj:'int'): The number of sampled actions, i.e. K in the Sampled MuZero paper.
+            - continuous_action_space (:obj:'bool'): whether the action space is continous in current env.
+        """
         self.num = root_num
         self.root_num = root_num
         self.legal_actions_list = legal_actions_list  # list of list
         self.num_of_sampled_actions = num_of_sampled_actions
         self.continuous_action_space = continuous_action_space
 
         self.roots = []
@@ -324,21 +374,21 @@
             noises: List[float],
             value_prefixs: List[float],
             policies: List[List[float]],
             to_play: int = -1
     ) -> None:
         """
         Overview:
-            Expand the roots and add noises.
+            Expand the roots and add noises for exploration.
         Arguments:
-            - root_noise_weight: the exploration fraction of roots
-            - noises: the vector of noise add to the roots.
-            - value_prefixs: the vector of value prefixs of each root.
-            - policies: the vector of policy logits of each root.
-            - to_play_batch: the vector of the player side of each root.
+            - root_noise_weight (:obj:`float`): the exploration fraction of roots
+            - noises (:obj:`List[float]`): the vector of noise add to the roots.
+            - value_prefixs (:obj:`List[float]`): the vector of rewards of each root.
+            - policies (:obj:`List[List[float]]`): the vector of policy logits of each root.
+            - to_play(:obj:`List`): The vector of the player side of each root.
         """
         for i in range(self.root_num):
 
             if to_play is None:
                 self.roots[i].expand(-1, 0, i, value_prefixs[i], policies[i])
             else:
                 self.roots[i].expand(to_play[i], 0, i, value_prefixs[i], policies[i])
@@ -347,86 +397,104 @@
             self.roots[i].visit_count += 1
 
     def prepare_no_noise(self, value_prefixs: List[float], policies: List[List[float]], to_play: int = -1) -> None:
         """
         Overview:
             Expand the roots without noise.
         Arguments:
-            - value_prefixs: the vector of value prefixs of each root.
-            - policies: the vector of policy logits of each root.
-            - to_play_batch: the vector of the player side of each root.
+            - value_prefixs (:obj:`List[float]`): the vector of value prefixs of each root.
+            - policies (:obj:`List[List[float]]`): the vector of policy logits of each root.
+            - to_play(:obj:`List`): The vector of the player side of each root.
         """
         for i in range(self.root_num):
             if to_play is None:
                 self.roots[i].expand(-1, 0, i, value_prefixs[i], policies[i])
             else:
                 self.roots[i].expand(to_play[i], 0, i, value_prefixs[i], policies[i])
 
             self.roots[i].visit_count += 1
 
     def clear(self) -> None:
+        """
+        Overview:
+            Clear all the roots in the list.
+        """
         self.roots.clear()
 
     def get_trajectories(self) -> List[List[Union[int, float]]]:
         """
         Overview:
             Find the current best trajectory starts from each root.
-        Outputs:
-            - traj: a vector of node index, which is the current best trajectory from each root.
+        Returns:
+            - traj (:obj:`List[List[Union[int, float]]]`): a vector of node index, which is the current best trajectory from each root.
         """
         trajs = []
         for i in range(self.root_num):
             trajs.append(self.roots[i].get_trajectory())
         return trajs
 
     def get_distributions(self) -> List[List[Union[int, float]]]:
         """
         Overview:
-            Get the children distribution of each root.
-        Outputs:
-            - distribution: a vector of distribution of child nodes in the format of visit count (i.e. [1,3,0,2,5]).
+            Get the visit count distribution of child nodes for each root.
+        Returns:
+            - distribution (:obj:`List[List[Union[int, float]]]`): a vector of distribution of child nodes in the format of visit count (i.e. [1,3,0,2,5]).
         """
         distributions = []
         for i in range(self.root_num):
             distributions.append(self.roots[i].get_children_distribution())
 
         return distributions
 
     # ==============================================================
     # sampled related core code
     # ==============================================================
     def get_sampled_actions(self) -> List[List[Union[int, float]]]:
         """
         Overview:
             Get the sampled_actions of each root.
-        Outputs:
-            - python_sampled_actions: a vector of sampled_actions for each root, e.g. the size of original action space is 6, the K=3,
-            python_sampled_actions = [[1,3,0], [2,4,0], [5,4,1]].
+        Returns:
+            - sampled_actions (:obj:`List[List[Union[int, float]]]`): a vector of sampled_actions for each root, \
+                e.g. the size of original action space is 6, K=3, sampled_actions = [[1,3,0], [2,4,0], [5,4,1]].
         """
         # TODO(pu): root_sampled_actions bug in discere action space?
         sampled_actions = []
         for i in range(self.root_num):
             sampled_actions.append(self.roots[i].legal_actions)
 
         return sampled_actions
 
     def get_values(self) -> float:
         """
         Overview:
-            Return the estimated value of each root.
+            Get the estimated value of each root.
+        Returns:
+            - values (:obj:`List[float]`): The estimated value of each root.
         """
         values = []
         for i in range(self.root_num):
             values.append(self.roots[i].value)
         return values
 
 
 class SearchResults:
+    """
+    Overview:
+        The class to record the results of the simulations for the batch of roots.
+    Interfaces:
+        ``__init__``.
+    """
 
-    def __init__(self, num: int):
+    def __init__(self, num: int) -> None:
+        """
+        Overview:
+            Initiaizes the attributes to be recorded.
+        Arguments:
+            -num (:obj:`int`): The number of search results(equal to ``batch_size``).
+        """
         self.num = num
         self.nodes = []
         self.search_paths = []
         self.latent_state_index_in_search_path = []
         self.latent_state_index_in_batch = []
         self.last_actions = []
         self.search_lens = []
@@ -442,22 +510,22 @@
         players: int,
         continuous_action_space: bool = False,
 ) -> Union[int, float]:
     """
     Overview:
         Select the child node of the roots according to ucb scores.
     Arguments:
-        - root: the roots to select the child node.
-        - min_max_stats (:obj:`Class MinMaxStats`):  a tool used to min-max normalize the score.
-        - pb_c_base (:obj:`Class Float`): constant c1 used in pUCT rule, typically 1.25.
-        - pb_c_int (:obj:`Class Float`): constant c2 used in pUCT rule, typically 19652.
-        - discount_factor (:obj:`Class Float`): The discount factor used in calculating bootstrapped value, if env is board_games, we set discount_factor=1.
-        - mean_q (:obj:`Class Float`): the mean q value of the parent node.
-        - players (:obj:`Class Float`): the number of players. one/in self-play-mode board games.
-        - continuous_action_space: whether the action space is continous in current env.
+        - root(:obj:`Node`): The root to select the child node.
+        - min_max_stats (:obj:`MinMaxStats`):  A tool used to min-max normalize the score.
+        - pb_c_base (:obj:`float`): Constant c1 used in pUCT rule, typically 1.25.
+        - pb_c_int (:obj:`float`): Constant c2 used in pUCT rule, typically 19652.
+        - discount_factor (:obj:`float`): The discount factor used in calculating bootstrapped value, if env is board_games, we set discount_factor=1.
+        - mean_q (:obj:`float`): The mean q value of the parent node.
+        - players (:obj:`int`): The number of players. In two-player games such as board games, the value need to be negatived when backpropating.
+        - continuous_action_space (:obj: `bool`): Whether the action space is continous in current env.
     Returns:
         - action (:obj:`Union[int, float]`): Choose the action with the highest ucb score.
     """
     # ==============================================================
     # sampled related core code
     # ==============================================================
     # TODO(pu): Progressive widening (See https://hal.archives-ouvertes.fr/hal-00542673v2/document)
@@ -500,28 +568,28 @@
         discount_factor: float,
         players: int = 1,
         continuous_action_space: bool = False,
 ) -> float:
     """
     Overview:
         Compute the ucb score of the child.
-        Arguments:
-            - child: the child node to compute ucb score.
-            - min_max_stats: a tool used to min-max normalize the score.
-            - parent_mean_q: the mean q value of the parent node.
-            - is_reset: whether the value prefix needs to be reset.
-            - total_children_visit_counts: the total visit counts of the child nodes of the parent node.
-            - parent_value_prefix: the value prefix of parent node.
-            - pb_c_base: constants c2 in muzero.
-            - pb_c_init: constants c1 in muzero.
-            - disount_factor: the discount factor of reward.
-            - players: the number of players.
-            - continuous_action_space: whether the action space is continous in current env.
-        Outputs:
-            - ucb_value: the ucb score of the child.
+    Arguments:
+        - child (:obj:`Node`): the child node to compute ucb score.
+        - min_max_stats (:obj:`MinMaxStats`): a tool used to min-max normalize the score.
+        - parent_mean_q (:obj:`float`): the mean q value of the parent node.
+        - is_reset (:obj:`float`): whether the value prefix needs to be reset.
+        - total_children_visit_counts (:obj:`float`): the total visit counts of the child nodes of the parent node.
+        - parent_value_prefix(:obj:`float`): The value prefix of parent node.
+        - pb_c_base (:obj:`float`): constants c2 in muzero.
+        - pb_c_init (:obj:`float`): constants c1 in muzero.
+        - disount_factor (:obj:`float`): the discount factor of reward.
+        - players (:obj:`int`): the number of players.
+        - continuous_action_space (:obj: `bool`): Whether the action space is continous in current env.
+    Returns:
+        - ucb_value (:obj:`float`): the ucb score of the child.
     """
     assert total_children_visit_counts == parent.visit_count
     pb_c = math.log((total_children_visit_counts + pb_c_base + 1) / pb_c_base) + pb_c_init
     pb_c *= (math.sqrt(total_children_visit_counts) / (child.visit_count + 1))
 
     # ==============================================================
     # sampled related core code
@@ -553,50 +621,53 @@
         if is_reset == 1:
             true_reward = child.value_prefix
         if players == 1:
             value_score = true_reward + discount_factor * child.value
         elif players == 2:
             value_score = true_reward + discount_factor * (-child.value)
 
+    # Normalize the value score.
     value_score = min_max_stats.normalize(value_score)
     if value_score < 0:
         value_score = 0
     if value_score > 1:
         value_score = 1
+    
     ucb_score = prior_score + value_score
 
     return ucb_score
 
 
 def batch_traverse(
         roots: Any,
         pb_c_base: float,
         pb_c_init: float,
         discount_factor: float,
-        min_max_stats_lst,
+        min_max_stats_lst: List[MinMaxStats],
         results: SearchResults,
         virtual_to_play: List,
         continuous_action_space: bool = False,
 ) -> Tuple[List[int], List[int], List[Union[int, float]], List]:
     """
     Overview:
-        traverse, also called expansion. process a batch roots parallely.
+        traverse, also called expansion. Process a batch roots at once.
     Arguments:
-        - roots (:obj:`Any`): a batch of root nodes to be expanded.
-        - pb_c_base (:obj:`float`): constant c1 used in pUCT rule, typically 1.25.
-        - pb_c_init (:obj:`float`): constant c2 used in pUCT rule, typically 19652.
+        - roots (:obj:`Any`): A batch of root nodes to be expanded.
+        - pb_c_base (:obj:`float`): Constant c1 used in pUCT rule, typically 1.25.
+        - pb_c_init (:obj:`float`): Constant c2 used in pUCT rule, typically 19652.
         - discount_factor (:obj:`float`): The discount factor used in calculating bootstrapped value, if env is board_games, we set discount_factor=1.
-        - virtual_to_play (:obj:`list`): the to_play list used in self_play collecting and training in board games,
+        - results (:obj:`SearchResults`): An instance to record the simulation results for all the roots in the batch.
+        - virtual_to_play (:obj:`list`): The to_play list used in self_play collecting and training in board games,
             `virtual` is to emphasize that actions are performed on an imaginary hidden state.
         - continuous_action_space: whether the action space is continous in current env.
     Returns:
-        - latent_state_index_in_search_path (:obj:`list`): the list of x/first index of hidden state vector of the searched node, i.e. the search depth.
-        - latent_state_index_in_batch (:obj:`list`): the list of y/second index of hidden state vector of the searched node, i.e. the index of batch root node, its maximum is ``batch_size``/``env_num``.
-        - last_actions (:obj:`list`): the action performed by the previous node.
-        - virtual_to_play (:obj:`list`): the to_play list used in self_play collecting and trainin gin board games,
+        - latent_state_index_in_search_path (:obj:`list`): The list of x/first index of hidden state vector of the searched node, i.e. the search depth.
+        - latent_state_index_in_batch (:obj:`list`): The list of y/second index of hidden state vector of the searched node, i.e. the index of batch root node, its maximum is ``batch_size``/``env_num``.
+        - last_actions (:obj:`list`): The action performed by the previous node.
+        - virtual_to_play (:obj:`list`): The to_play list used in self_play collecting and trainin gin board games,
             `virtual` is to emphasize that actions are performed on an imaginary hidden state.
     """
     parent_q = 0.0
     results.search_lens = [None for _ in range(results.num)]
     results.last_actions = [None for _ in range(results.num)]
 
     results.nodes = [None for _ in range(results.num)]
@@ -662,21 +733,21 @@
 def backpropagate(
         search_path: List[Node], min_max_stats: MinMaxStats, to_play: int, value: float, discount_factor: float
 ) -> None:
     """
     Overview:
         Update the value sum and visit count of nodes along the search path.
     Arguments:
-        - search_path: a vector of nodes on the search path.
-        - min_max_stats: a tool used to min-max normalize the q value.
-        - to_play: which player to play the game in the current node.
-        - value: the value to propagate along the search path.
-        - discount_factor: the discount factor of reward.
+        - search_path (:obj:`List[Node]`): a vector of nodes on the search path.
+        - min_max_stats (:obj:`MinMaxStats`): a tool used to min-max normalize the q value.
+        - to_play (:obj:`int`): which player to play the game in the current node.
+        - value (:obj:`float`): the value to propagate along the search path.
+        - discount_factor (:obj:`float`): the discount factor of reward.
     """
-    assert to_play is None or to_play in [-1, 1, 2], to_play
+    assert to_play is None or to_play in [-1, 1, 2], f'to_play is {to_play}!'
     if to_play is None or to_play == -1:
         # for play-with-bot-mode
         bootstrap_value = value
         path_len = len(search_path)
         for i in range(path_len - 1, -1, -1):
             node = search_path[i]
             node.value_sum += bootstrap_value
@@ -734,29 +805,29 @@
         discount_factor: float,
         value_prefixs: List,
         values: List[float],
         policies: List[float],
         min_max_stats_lst: List[MinMaxStats],
         results: SearchResults,
         is_reset_list: List,
-        to_play: list = None
+        to_play: list = None,
 ) -> None:
     """
     Overview:
-        Backpropagation along the search path to update the attributes.
+        Update the value sum and visit count of nodes along the search paths for each root in the batch.
     Arguments:
-        - simulation_index (:obj:`Class Int`): The index of latent state of the leaf node in the search path.
-        - discount_factor (:obj:`Class Float`): The discount factor used in calculating bootstrapped value, if env is board_games, we set discount_factor=1.
-        - value_prefixs (:obj:`Class List`): the value prefixs of nodes along the search path.
-        - values (:obj:`Class List`):  the values to propagate along the search path.
-        - policies (:obj:`Class List`): the policy logits of nodes along the search path.
-        - min_max_stats_lst (:obj:`Class List[MinMaxStats]`):  a tool used to min-max normalize the q value.
-        - results (:obj:`Class List`): the search results.
-        - is_reset_list (:obj:`Class List`): the vector of is_reset nodes along the search path, where is_reset represents for whether the parent value prefix needs to be reset.
-        - to_play (:obj:`Class List`):  the batch of which player is playing on this node.
+        - simulation_index (:obj:`int`): The index of latent state of the leaf node in the search path.
+        - discount_factor (:obj:`float`): The discount factor used in calculating bootstrapped value, if env is board_games, we set discount_factor=1.
+        - value_prefixs (:obj:`List`): the value prefixs of nodes along the search path.
+        - values (:obj:`List`):  the values to propagate along the search path.
+        - policies (:obj:`List`): the policy logits of nodes along the search path.
+        - min_max_stats_lst (:obj:`List[MinMaxStats]`):  a tool used to min-max normalize the q value.
+        - results (:obj:`List`): the search results.
+        - is_reset_list (:obj:`List`): the vector of is_reset nodes along the search path, where is_reset represents for whether the parent value prefix needs to be reset.
+        - to_play (:obj:`List`): the batch of which player is playing on this node.
     """
     for i in range(results.num):
         # ****** expand the leaf node ******
         if to_play is None:
             # we set to_play=-1, because in self-play-mode of board_games to_play = {1, 2}.
             results.nodes[i].expand(-1, simulation_index, i, value_prefixs[i], policies[i])
         else:
@@ -775,78 +846,71 @@
 
 
 from typing import Union
 import numpy as np
 
 class Action:
     """
-    Class that represents an action of a game.
-
-    Attributes:
-        value (Union[int, np.ndarray]): The value of the action. Can be either an integer or a numpy array.
+    Overview:
+        Class that represents an action of the game.
     """
-
     def __init__(self, value: Union[int, np.ndarray]) -> None:
         """
-        Initializes the Action with the given value.
-
-        Args:
-            value (Union[int, np.ndarray]): The value of the action.
+        Overview:
+            Initializes the Action with the given value.
+        Arguments:
+            - value (:obj:`Union[int, np.ndarray]`): The value of the action. Can be either an integer or a numpy array.
         """
         self.value = value
 
     def __hash__(self) -> int:
         """
-        Returns a hash of the Action's value.
-
-        If the value is a numpy array, it is flattened to a tuple and then hashed.
-        If the value is a single integer, it is hashed directly.
-
+        Overview:
+            Returns a hash of the Action's value. \
+            If the value is a numpy array, it is flattened to a tuple and then hashed. \
+            If the value is a single integer, it is hashed directly. 
         Returns:
-            int: The hash of the Action's value.
+            hash (:obj:`int`): The hash of the Action's value.
         """
         if isinstance(self.value, np.ndarray):
             if self.value.ndim == 0:
                 return hash(self.value.item())
             else:
                 return hash(tuple(self.value.flatten()))
         else:
             return hash(self.value)
 
     def __eq__(self, other: "Action") -> bool:
         """
-        Determines if this Action is equal to another Action.
-
-        If both values are numpy arrays, they are compared element-wise.
-        Otherwise, they are compared directly.
-
-        Args:
-            other (Action): The Action to compare with.
-
+        Overview:
+            Determines if this Action is equal to another Action. \
+            If both values are numpy arrays, they are compared element-wise. \
+            Otherwise, they are compared directly.
+        Arguments:
+            - other (:obj:`Action`): The Action to compare with.
         Returns:
-            bool: True if the two Actions are equal, False otherwise.
+            - bool (:obj:`bool`): True if the two Actions are equal, False otherwise.
         """
         if isinstance(self.value, np.ndarray) and isinstance(other.value, np.ndarray):
             return np.array_equal(self.value, other.value)
         else:
             return self.value == other.value
 
     def __gt__(self, other: "Action") -> bool:
         """
-        Determines if this Action's value is greater than another Action's value.
-
-        Args:
-            other (Action): The Action to compare with.
-
+        Overview:
+            Determines if this Action's value is greater than another Action's value.
+        Arguments:
+            - other (:obj:`Action`): The Action to compare with.
         Returns:
-            bool: True if this Action's value is greater, False otherwise.
+            - bool (:obj:`bool`): True if the two Actions are equal, False otherwise.
         """
         return self.value > other.value
 
     def __repr__(self) -> str:
         """
-        Returns a string representation of this Action.
-
+        Overview:
+            Returns a string representation of this Action.
         Returns:
-            str: A string representation of the Action's value.
+            - str (:obj:`str`): A string representation of the Action's value.
         """
         return str(self.value)
```

### Comparing `LightZero-0.0.2/lzero/mcts/ptree/ptree_stochastic_mz.py` & `LightZero-0.0.5/lzero/mcts/ptree/ptree_ez.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,609 +1,652 @@
 """
-The Node, Roots class and related core functions for Stochastic MuZero.
+The Node, Roots class and related core functions for EfficientZero.
 """
 import math
 import random
-from typing import List, Dict, Any, Tuple, Union
+from typing import List, Any, Tuple, Union
 
 import numpy as np
 import torch
 
 from .minimax import MinMaxStats
 
 
 class Node:
     """
-     Overview:
-         the node base class for Stochastic MuZero.
-     Arguments:
-     """
+    Overview:
+        The Node class for EfficientZero. The basic functions of the node are implemented.
+    Interfaces:
+        ``__init__``, ``expand``, ``add_exploration_noise``, ``compute_mean_q``, ``get_trajectory``, \
+        ``get_children_distribution``, ``get_child``, ``expanded``, ``value``.
+    """
 
-    def __init__(self, prior: float, legal_actions: List = None, action_space_size: int = 9, is_chance: bool = False, chance_space_size: int = 2) -> None:
+    def __init__(self, prior: float, legal_actions: List = None, action_space_size: int = 9) -> None:
+        """
+        Overview:
+            Initializes a Node instance.
+        Arguments:
+            - prior (:obj:`float`): The prior probability of the node.
+            - legal_actions (:obj:`List`, optional): The list of legal actions of the node. Defaults to None.
+            - action_space_size (:obj:`int`, optional): The size of the action space. Defaults to 9.
+        """
         self.prior = prior
         self.legal_actions = legal_actions
         self.action_space_size = action_space_size
 
+        self.is_reset = 0
         self.visit_count = 0
         self.value_sum = 0
         self.best_action = -1
-        self.to_play = 0  # default 0 means play_with_bot_mode
-        self.reward = 0
+        self.to_play = -1  # default -1 means play_with_bot_mode
         self.value_prefix = 0.0
         self.children = {}
         self.children_index = []
-        self.latent_state_index_in_search_path = 0
-        self.latent_state_index_in_batch = 0
-        self.parent_value_prefix = 0  # only used in update_tree_q method
-
-        self.is_chance = is_chance
-        self.chance_space_size = chance_space_size
+        self.simulation_index = 0
+        self.batch_index = 0
 
     def expand(
-            self, to_play: int, latent_state_index_in_search_path: int, latent_state_index_in_batch: int, reward: float,
-            policy_logits: List[float], child_is_chance: bool = True
+            self, to_play: int, simulation_index: int, batch_index: int, value_prefix: float, policy_logits: List[float]
     ) -> None:
         """
         Overview:
             Expand the child nodes of the current node.
         Arguments:
-            - to_play (:obj:`Class int`): which player to play the game in the current node.
-            - latent_state_index_in_search_path (:obj:`Class int`): the x/first index of latent state vector of the current node, i.e. the search depth.
-            - latent_state_index_in_batch (:obj:`Class int`): the y/second index of latent state vector of the current node, i.e. the index of batch root node, its maximum is ``batch_size``/``env_num``.
-            - value_prefix: (:obj:`Class float`): the value prefix of the current node.
-            - policy_logits: (:obj:`Class List`): the policy logit of the child nodes.
+            - to_play (:obj:`int`): The player to play the game in the current node.
+            - simulation_index (:obj:`int`): The x/first index of the hidden state vector of the current node, i.e., the search depth.
+            - batch_index (:obj:`int`): The y/second index of the hidden state vector of the current node, i.e., the index of the batch root node, its maximum is `batch_size`/`env_num`.
+            - value_prefix: (:obj:`float`): the value prefix of the current node.
+            - policy_logits (:obj:`List[float]`): The policy logits providing the priors for the child nodes.
         """
         self.to_play = to_play
-        self.reward = reward
-
-        if self.is_chance is True:
-            child_is_chance = False
-            self.reward = 0.0
-
-            if self.legal_actions is None:
-                self.legal_actions = np.arange(self.chance_space_size)
-            self.latent_state_index_in_search_path = latent_state_index_in_search_path
-            self.latent_state_index_in_batch = latent_state_index_in_batch
-            policy_values = torch.softmax(torch.tensor([policy_logits[a] for a in self.legal_actions]), dim=0).tolist()
-            policy = {legal_action: policy_values[index] for index, legal_action in enumerate(self.legal_actions)}
-            for action, prior in policy.items():
-                self.children[action] = Node(prior, is_chance=child_is_chance)
-        else:
-            child_is_chance = True
+        if self.legal_actions is None:
             self.legal_actions = np.arange(len(policy_logits))
-            self.latent_state_index_in_search_path = latent_state_index_in_search_path
-            self.latent_state_index_in_batch = latent_state_index_in_batch
-            policy_values = torch.softmax(torch.tensor([policy_logits[a] for a in self.legal_actions]), dim=0).tolist()
-            policy = {legal_action: policy_values[index] for index, legal_action in enumerate(self.legal_actions)}
-            for action, prior in policy.items():
-                self.children[action] = Node(prior, is_chance=child_is_chance)
+
+        self.simulation_index = simulation_index
+        self.batch_index = batch_index
+        self.value_prefix = value_prefix
+
+        policy_values = torch.softmax(torch.tensor([policy_logits[a] for a in self.legal_actions]), dim=0).tolist()
+        policy = {a: policy_values[i] for i, a in enumerate(self.legal_actions)}
+        for action, p in policy.items():
+            self.children[action] = Node(p, action_space_size=self.action_space_size)
 
     def add_exploration_noise(self, exploration_fraction: float, noises: List[float]) -> None:
         """
         Overview:
-            add exploration noise to priors
+            Add exploration noise to the priors of the child nodes..
         Arguments:
-            - noises (:obj: list): length is len(self.legal_actions)
+            - exploration_fraction (:obj:`float`): The fraction of exploration noise to be added.
+            - noises (:obj:`List[float]`): The list of noises to be added to the priors.
         """
         for i, a in enumerate(self.legal_actions):
             """
             i in index, a is action, e.g. self.legal_actions = [0,1,2,4,6,8], i=[0,1,2,3,4,5], a=[0,1,2,4,6,8]
             """
             try:
                 noise = noises[i]
             except Exception as error:
                 print(error)
             child = self.get_child(a)
             prior = child.prior
             child.prior = prior * (1 - exploration_fraction) + noise * exploration_fraction
 
-    def compute_mean_q(self, is_root: int, parent_q: float, discount_factor: float) -> float:
+    def compute_mean_q(self, is_root: bool, parent_q: float, discount_factor: float) -> float:
         """
         Overview:
-            Compute the mean q value of the current node.
+            Compute the mean of the action values of all legal actions.
         Arguments:
-            - is_root (:obj:`int`): whether the current node is a root node.
-            - parent_q (:obj:`float`): the q value of the parent node.
-            - discount_factor (:obj:`float`): the discount_factor of reward.
+            - is_root (:obj:`bool`): Whether the current node is a root node.
+            - parent_q (:obj:`float`): The q value of the parent node.
+            - discount_factor (:obj:`float`): The discount factor of the reward.
+        Returns:
+            - mean_q (:obj:`float`): The mean of the action values.
         """
         total_unsigned_q = 0.0
         total_visits = 0
+        parent_value_prefix = self.value_prefix
         for a in self.legal_actions:
             child = self.get_child(a)
             if child.visit_count > 0:
-                true_reward = child.reward
+                true_reward = child.value_prefix - parent_value_prefix
+                if self.is_reset == 1:
+                    # TODO(pu)
+                    true_reward = child.value_prefix
                 # TODO(pu): only one step bootstrap?
                 q_of_s_a = true_reward + discount_factor * child.value
                 total_unsigned_q += q_of_s_a
                 total_visits += 1
         if is_root and total_visits > 0:
             mean_q = total_unsigned_q / total_visits
         else:
             # if is not root node,
             # TODO(pu): why parent_q?
             mean_q = (parent_q + total_unsigned_q) / (total_visits + 1)
         return mean_q
 
+    def print_out(self) -> None:
+        pass
+
     def get_trajectory(self) -> List[Union[int, float]]:
         """
         Overview:
-            Find the current best trajectory starts from the current node.
-        Outputs:
-            - traj: a vector of node index, which is the current best trajectory from this node.
+            Find the current best trajectory starting from the current node.
+        Returns:
+            - traj (:obj:`List[Union[int, float]]`): A vector of node indices representing the current best trajectory.
         """
         # TODO(pu): best action
         traj = []
         node = self
         best_action = node.best_action
         while best_action >= 0:
             traj.append(best_action)
 
             node = node.get_child(best_action)
             best_action = node.best_action
         return traj
 
     def get_children_distribution(self) -> List[Union[int, float]]:
+        """
+        Overview:
+            Get the distribution of visit counts among the child nodes.
+        Returns:
+            - distribution (:obj:`List[Union[int, float]]` or :obj:`None`): The distribution of visit counts among the children nodes. \
+              If the legal_actions list is empty, returns None.
+        """
         if self.legal_actions == []:
             return None
         distribution = {a: 0 for a in self.legal_actions}
         if self.expanded:
             for a in self.legal_actions:
                 child = self.get_child(a)
                 distribution[a] = child.visit_count
             # only take the visit counts
             distribution = [v for k, v in distribution.items()]
         return distribution
 
     def get_child(self, action: Union[int, float]) -> "Node":
         """
         Overview:
-            get children node according to the input action.
+            Get the child node according to the input action.
+        Arguments:
+            - action (:obj:`Union[int, float]`): The action for which the child node is to be retrieved.
+        Returns:
+            - child (:obj:`Node`): The child node corresponding to the input action.
         """
         if not isinstance(action, np.int64):
             action = int(action)
         return self.children[action]
 
     @property
     def expanded(self) -> bool:
+        """
+        Overview:
+            Check if the node has been expanded.
+        Returns:
+            - expanded (:obj:`bool`): True if the node has been expanded, False otherwise.
+        """
         return len(self.children) > 0
 
     @property
     def value(self) -> float:
         """
         Overview:
-            Return the estimated value of the current root node.
+            Return the estimated value of the current node.
+        Returns:
+            - value (:obj:`float`): The estimated value of the current node.
         """
         if self.visit_count == 0:
             return 0
         else:
             return self.value_sum / self.visit_count
 
 
 class Roots:
+    """
+    Overview:
+        The class to process a batch of roots(Node instances) at the same time.
+    Interfaces:
+        ``__init__``, ``prepare``,  ``prepare_no_noise``, ``clear``, ``get_trajectories``, \
+        ``get_distributions``, ``get_values``
+    """
 
     def __init__(self, root_num: int, legal_actions_list: List) -> None:
+        """
+        Overview:
+            Initializes an instance of the Roots class with the specified number of roots and legal actions.
+        Arguments:
+            - root_num (:obj:`int`): The number of roots.
+            - legal_actions_list(:obj:`List`): A list of the legal actions for each root.
+        """
         self.num = root_num
         self.root_num = root_num
         self.legal_actions_list = legal_actions_list  # list of list
 
         self.roots = []
         for i in range(self.root_num):
             if isinstance(legal_actions_list, list):
-                self.roots.append(Node(0, legal_actions_list[i]))
+                self.action_space_size = len(legal_actions_list[i])
+
+                self.roots.append(Node(0, legal_actions_list[i], action_space_size=self.action_space_size))
             else:
                 # if legal_actions_list is int
-                self.roots.append(Node(0, np.arange(legal_actions_list)))
+                self.action_space_size = legal_actions_list
+
+                self.roots.append(Node(0, np.arange(legal_actions_list), action_space_size=self.action_space_size))
 
     def prepare(
             self,
             root_noise_weight: float,
             noises: List[float],
-            rewards: List[float],
+            value_prefixs: List[float],
             policies: List[List[float]],
             to_play: int = -1
     ) -> None:
         """
         Overview:
-            Expand the roots and add noises.
+            Expand the roots and add noises for exploration.
         Arguments:
-            - root_noise_weight: the exploration fraction of roots
-            - noises: the vector of noise add to the roots.
-            - rewards: the vector of rewards of each root.
-            - policies: the vector of policy logits of each root.
-            - to_play_batch: the vector of the player side of each root.
+            - root_noise_weight (:obj:`float`): the exploration fraction of roots
+            - noises (:obj:`List[float]`): the vector of noise add to the roots.
+            - value_prefixs (:obj:`List[float]`): the vector of rewards of each root.
+            - policies (:obj:`List[List[float]]`): the vector of policy logits of each root.
+            - to_play(:obj:`List`): The vector of the player side of each root.
         """
         for i in range(self.root_num):
-            #  to_play: int, latent_state_index_in_search_path: int, latent_state_index_in_batch: int,
-            if to_play is None:
-                # TODO(pu): why latent_state_index_in_search_path=0, latent_state_index_in_batch=i?
-                self.roots[i].expand(-1, 0, i, rewards[i], policies[i])
+
+            if to_play in [-1, None]:
+                self.roots[i].expand(-1, 0, i, value_prefixs[i], policies[i])
             else:
-                self.roots[i].expand(to_play[i], 0, i, rewards[i], policies[i])
+                self.roots[i].expand(to_play[i], 0, i, value_prefixs[i], policies[i])
 
             self.roots[i].add_exploration_noise(root_noise_weight, noises[i])
             self.roots[i].visit_count += 1
 
-    def prepare_no_noise(self, rewards: List[float], policies: List[List[float]], to_play: int = -1) -> None:
+    def prepare_no_noise(self, value_prefixs: List[float], policies: List[List[float]], to_play: int = -1) -> None:
         """
         Overview:
             Expand the roots without noise.
         Arguments:
-            - rewards: the vector of rewards of each root.
-            - policies: the vector of policy logits of each root.
-            - to_play_batch: the vector of the player side of each root.
+            - value_prefixs (:obj:`List[float]`): the vector of value prefixs of each root.
+            - policies (:obj:`List[List[float]]`): the vector of policy logits of each root.
+            - to_play(:obj:`List`): The vector of the player side of each root.
         """
         for i in range(self.root_num):
-            if to_play is None:
-                self.roots[i].expand(-1, 0, i, rewards[i], policies[i])
+            if to_play in [-1, None]:
+                self.roots[i].expand(-1, 0, i, value_prefixs[i], policies[i])
             else:
-                self.roots[i].expand(to_play[i], 0, i, rewards[i], policies[i])
+                self.roots[i].expand(to_play[i], 0, i, value_prefixs[i], policies[i])
 
             self.roots[i].visit_count += 1
 
     def clear(self) -> None:
+        """
+        Overview:
+            Clear all the roots in the list.
+        """
         self.roots.clear()
 
     def get_trajectories(self) -> List[List[Union[int, float]]]:
         """
         Overview:
             Find the current best trajectory starts from each root.
-        Outputs:
-            - traj: a vector of node index, which is the current best trajectory from each root.
+        Returns:
+            - traj (:obj:`List[List[Union[int, float]]]`): a vector of node index, which is the current best trajectory from each root.
         """
         trajs = []
         for i in range(self.root_num):
             trajs.append(self.roots[i].get_trajectory())
         return trajs
 
     def get_distributions(self) -> List[List[Union[int, float]]]:
         """
         Overview:
-            Get the children distribution of each root.
-        Outputs:
-            - distribution: a vector of distribution of child nodes in the format of visit count (i.e. [1,3,0,2,5]).
+            Get the visit count distribution of child nodes for each root.
+        Returns:
+            - distribution (:obj:`List[List[Union[int, float]]]`): a vector of distribution of child nodes in the format of visit count (i.e. [1,3,0,2,5]).
         """
         distributions = []
         for i in range(self.root_num):
             distributions.append(self.roots[i].get_children_distribution())
 
         return distributions
 
-    def get_values(self) -> float:
+    def get_values(self) -> List[float]:
         """
         Overview:
-            Return the estimated value of each root.
+            Get the estimated value of each root.
+        Returns:
+            - values (:obj:`List[float]`): The estimated value of each root.
         """
         values = []
         for i in range(self.root_num):
             values.append(self.roots[i].value)
         return values
 
 
 class SearchResults:
+    """
+    Overview:
+        The class to record the results of the simulations for the batch of roots.
+    Interfaces:
+        ``__init__``.
+    """
 
     def __init__(self, num: int) -> None:
+        """
+        Overview:
+            Initiaizes the attributes to be recorded.
+        Arguments:
+            -num (:obj:`int`): The number of search results(equal to ``batch_size``).
+        """
         self.num = num
         self.nodes = []
         self.search_paths = []
         self.latent_state_index_in_search_path = []
         self.latent_state_index_in_batch = []
         self.last_actions = []
         self.search_lens = []
 
 
-def update_tree_q(root: Node, min_max_stats: MinMaxStats, discount_factor: float, players: int = 1) -> None:
-    """
-    Overview:
-        Update the value sum and visit count of nodes along the search path.
-    Arguments:
-        - search_path: a vector of nodes on the search path.
-        - min_max_stats: a tool used to min-max normalize the q value.
-        - to_play: which player to play the game in the current node.
-        - value: the value to propagate along the search path.
-        - discount_factor: the discount factor of reward.
-    """
-    node_stack = []
-    node_stack.append(root)
-    while len(node_stack) > 0:
-        node = node_stack[-1]
-        node_stack.pop()
-
-        if node != root:
-            true_reward = node.reward
-            if players == 1:
-                q_of_s_a = true_reward + discount_factor * node.value
-            elif players == 2:
-                q_of_s_a = true_reward + discount_factor * (-node.value)
-
-            min_max_stats.update(q_of_s_a)
-
-        for a in node.legal_actions:
-            child = node.get_child(a)
-            if child.expanded:
-                node_stack.append(child)
-
-
 def select_child(
-        node: Node, min_max_stats: MinMaxStats, pb_c_base: float, pb_c_int: float, discount_factor: float,
+        root: Node, min_max_stats: MinMaxStats, pb_c_base: float, pb_c_int: float, discount_factor: float,
         mean_q: float, players: int
 ) -> Union[int, float]:
     """
     Overview:
         Select the child node of the roots according to ucb scores.
     Arguments:
-        - node: the node to select the child node.
-        - min_max_stats (:obj:`Class MinMaxStats`):  a tool used to min-max normalize the score.
-        - pb_c_base (:obj:`Class Float`): constant c1 used in pUCT rule, typically 1.25.
-        - pb_c_int (:obj:`Class Float`): constant c2 used in pUCT rule, typically 19652.
-        - discount_factor (:obj:`Class Float`): discount_factor factor used i calculating bootstrapped value, if env is board_games, we set discount_factor=1.
-        - mean_q (:obj:`Class Float`): the mean q value of the parent node.
-        - players (:obj:`Class Int`): the number of players. one/two_player mode board games.
+        - root(:obj:`Node`): The root to select the child node.
+        - min_max_stats (:obj:`MinMaxStats`):  A tool used to min-max normalize the score.
+        - pb_c_base (:obj:`float`): Constant c1 used in pUCT rule, typically 1.25.
+        - pb_c_int (:obj:`float`): Constant c2 used in pUCT rule, typically 19652.
+        - discount_factor (:obj:`float`): The discount factor used in calculating bootstrapped value, if env is board_games, we set discount_factor=1.
+        - mean_q (:obj:`float`): The mean q value of the parent node.
+        - players (:obj:`int`): The number of players. In two-player games such as board games, the value need to be negatived when backpropating.
     Returns:
         - action (:obj:`Union[int, float]`): Choose the action with the highest ucb score.
     """
-
-    if node.is_chance:
-        # print("root->is_chance: True ")
-
-        # If the node is chance node, we sample from the prior outcome distribution.
-        outcomes, probs = zip(*[(o, n.prior) for o, n in node.children.items()])
-        outcome = np.random.choice(outcomes, p=probs)
-        # print(outcome, probs)
-        return outcome
-
-    # print("root->is_chance: False ")
-    # If the node is decision node, we select the action with the highest ucb score.
     max_score = -np.inf
     epsilon = 0.000001
     max_index_lst = []
-    for a in node.legal_actions:
-        child = node.get_child(a)
+    for a in root.legal_actions:
+        child = root.get_child(a)
         temp_score = compute_ucb_score(
-            child, min_max_stats, mean_q, node.visit_count, pb_c_base, pb_c_int, discount_factor, players
+            child, min_max_stats, mean_q, root.is_reset, root.visit_count, root.value_prefix, pb_c_base, pb_c_int,
+            discount_factor, players
         )
         if max_score < temp_score:
             max_score = temp_score
             max_index_lst.clear()
             max_index_lst.append(a)
         elif temp_score >= max_score - epsilon:
-            # TODO(pu): if the difference is less than epsilon = 0.000001, we random choice action from  max_index_lst
+            # NOTE: if the difference is less than  epsilon = 0.000001, we random choice action from  max_index_lst
             max_index_lst.append(a)
 
     action = 0
     if len(max_index_lst) > 0:
         action = random.choice(max_index_lst)
     return action
 
 
 def compute_ucb_score(
         child: Node,
         min_max_stats: MinMaxStats,
         parent_mean_q: float,
+        is_reset: int,
         total_children_visit_counts: float,
+        parent_value_prefix: float,
         pb_c_base: float,
         pb_c_init: float,
         discount_factor: float,
         players: int = 1,
 ) -> float:
     """
     Overview:
         Compute the ucb score of the child.
-        Arguments:
-            - child: the child node to compute ucb score.
-            - min_max_stats: a tool used to min-max normalize the score.
-            - parent_mean_q: the mean q value of the parent node.
-            - is_reset: whether the value prefix needs to be reset.
-            - total_children_visit_counts: the total visit counts of the child nodes of the parent node.
-            - parent_value_prefix: the value prefix of parent node.
-            - pb_c_base: constants c2 in muzero.
-            - pb_c_init: constants c1 in muzero.
-            - disount_factor: the discount factor of reward.
-            - players: the number of players.
-            - continuous_action_space: whether the action space is continous in current env.
-        Outputs:
-            - ucb_value: the ucb score of the child.
+    Arguments:
+        - child (:obj:`Node`): the child node to compute ucb score.
+        - min_max_stats (:obj:`MinMaxStats`): a tool used to min-max normalize the score.
+        - parent_mean_q (:obj:`float`): the mean q value of the parent node.
+        - is_reset (:obj:`float`): whether the value prefix needs to be reset.
+        - total_children_visit_counts (:obj:`float`): the total visit counts of the child nodes of the parent node.
+        - parent_value_prefix(:obj:`float`): The value prefix of parent node.
+        - pb_c_base (:obj:`float`): constants c2 in muzero.
+        - pb_c_init (:obj:`float`): constants c1 in muzero.
+        - disount_factor (:obj:`float`): the discount factor of reward.
+        - players (:obj:`int`): the number of players.
+    Returns:
+        - ucb_value (:obj:`float`): the ucb score of the child.
     """
+    # Compute the prior score.
     pb_c = math.log((total_children_visit_counts + pb_c_base + 1) / pb_c_base) + pb_c_init
     pb_c *= (math.sqrt(total_children_visit_counts) / (child.visit_count + 1))
 
     prior_score = pb_c * child.prior
+
+    # Compute the value score.
     if child.visit_count == 0:
         value_score = parent_mean_q
     else:
-        true_reward = child.reward
+        true_reward = child.value_prefix - parent_value_prefix
+        if is_reset == 1:
+            true_reward = child.value_prefix
         if players == 1:
             value_score = true_reward + discount_factor * child.value
         elif players == 2:
             value_score = true_reward + discount_factor * (-child.value)
 
+    # Normalize the value score.
     value_score = min_max_stats.normalize(value_score)
     if value_score < 0:
         value_score = 0
     if value_score > 1:
         value_score = 1
+    
     ucb_score = prior_score + value_score
 
     return ucb_score
 
 
 def batch_traverse(
         roots: Any,
         pb_c_base: float,
         pb_c_init: float,
         discount_factor: float,
         min_max_stats_lst: List[MinMaxStats],
         results: SearchResults,
-        virtual_to_play: List,
-) -> Tuple[Any, Any]:
-
+        virtual_to_play: Union[list, int],
+) -> Tuple[List[None], List[None], List[None], Union[list, int]]:
     """
     Overview:
-        traverse, also called selection. process a batch roots parallely.
+        traverse, also called expansion. Process a batch roots at once.
     Arguments:
-        - roots (:obj:`Any`): a batch of root nodes to be expanded.
-        - pb_c_base (:obj:`float`): constant c1 used in pUCT rule, typically 1.25.
-        - pb_c_init (:obj:`float`): constant c2 used in pUCT rule, typically 19652.
-        - discount_factor (:obj:`float`): discount_factor factor used i calculating bootstrapped value, if env is board_games, we set discount_factor=1.
-        - virtual_to_play (:obj:`list`): the to_play list used in self_play collecting and training in board games,
+        - roots (:obj:`Any`): A batch of root nodes to be expanded.
+        - pb_c_base (:obj:`float`): Constant c1 used in pUCT rule, typically 1.25.
+        - pb_c_init (:obj:`float`): Constant c2 used in pUCT rule, typically 19652.
+        - discount_factor (:obj:`float`): The discount factor used in calculating bootstrapped value, if env is board_games, we set discount_factor=1.
+        - results (:obj:`SearchResults`): An instance to record the simulation results for all the roots in the batch.
+        - virtual_to_play (:obj:`Union[list, int]`): The to_play list used in self_play collecting and training in board games,
             `virtual` is to emphasize that actions are performed on an imaginary hidden state.
-        - continuous_action_space: whether the action space is continous in current env.
     Returns:
-        - latent_state_index_in_search_path (:obj:`list`): the list of x/first index of latent state vector of the searched node, i.e. the search depth.
-        - latent_state_index_in_batch (:obj:`list`): the list of y/second index of latent state vector of the searched node, i.e. the index of batch root node, its maximum is ``batch_size``/``env_num``.
-        - last_actions (:obj:`list`): the action performed by the previous node.
-        - virtual_to_play (:obj:`list`): the to_play list used in self_play collecting and trainin gin board games,
+        - latent_state_index_in_search_path (:obj:`list`): The list of x/first index of hidden state vector of the searched node, i.e. the search depth.
+        - latent_state_index_in_batch (:obj:`list`): The list of y/second index of hidden state vector of the searched node, i.e. the index of batch root node, its maximum is ``batch_size``/``env_num``.
+        - last_actions (:obj:`list`): The action performed by the previous node.
+        - virtual_to_play (:obj:`Union[list, int]`): The to_play list used in self_play collecting and trainin gin board games,
             `virtual` is to emphasize that actions are performed on an imaginary hidden state.
     """
     parent_q = 0.0
-    results.search_lens = [None for i in range(results.num)]
-    results.last_actions = [None for i in range(results.num)]
+    results.search_lens = [None for _ in range(results.num)]
+    results.last_actions = [None for _ in range(results.num)]
+    results.nodes = [None for _ in range(results.num)]
+    results.latent_state_index_in_search_path = [None for _ in range(results.num)]
+    results.latent_state_index_in_batch = [None for _ in range(results.num)]
+    results.search_paths = {i: [] for i in range(results.num)}
 
-    results.nodes = [None for i in range(results.num)]
-    results.latent_state_index_in_search_path = [None for i in range(results.num)]
-    results.latent_state_index_in_batch = [None for i in range(results.num)]
-    if virtual_to_play in [1, 2] or virtual_to_play[0] in [1, 2]:
-        players = 2
-    elif virtual_to_play in [-1, None] or virtual_to_play[0] in [-1, None]:
-        players = 1
+    if isinstance(virtual_to_play, int):
+        if virtual_to_play in [1, 2]:
+            players = 2
+        elif virtual_to_play in [-1, None]:
+            players = 1
+    elif isinstance(virtual_to_play, list):
+        if virtual_to_play[0] in [1, 2]:
+            players = 2
+        elif virtual_to_play[0] in [-1, None]:
+            players = 1
 
-    results.search_paths = {i: [] for i in range(results.num)}
     for i in range(results.num):
         node = roots.roots[i]
         is_root = 1
         search_len = 0
         results.search_paths[i].append(node)
-
         """
         MCTS stage 1: Selection
-            Each simulation starts from the internal root state s0, and finishes when the simulation reaches a leaf node s_l.
+            Each simulation starts from the internal root state s0, and finishes when the simulation reaches a leaf node s_l. 
+            The leaf node is the node that is currently not expanded.
         """
-        # the leaf node is not expanded
         while node.expanded:
+
             mean_q = node.compute_mean_q(is_root, parent_q, discount_factor)
             is_root = 0
             parent_q = mean_q
 
             # select action according to the pUCT rule.
             action = select_child(
                 node, min_max_stats_lst.stats_lst[i], pb_c_base, pb_c_init, discount_factor, mean_q, players
             )
             if players == 2:
                 # Players play turn by turn
                 if virtual_to_play[i] == 1:
                     virtual_to_play[i] = 2
                 else:
                     virtual_to_play[i] = 1
-
             node.best_action = action
+
             # move to child node according to selected action.
             node = node.get_child(action)
-
             last_action = action
-
             results.search_paths[i].append(node)
             search_len += 1
 
             # note this return the parent node of the current searched node
             parent = results.search_paths[i][len(results.search_paths[i]) - 1 - 1]
-            results.latent_state_index_in_search_path[i] = parent.latent_state_index_in_search_path
-            results.latent_state_index_in_batch[i] = parent.latent_state_index_in_batch
+
+            results.latent_state_index_in_search_path[i] = parent.simulation_index
+            results.latent_state_index_in_batch[i] = parent.batch_index
             results.last_actions[i] = last_action
             results.search_lens[i] = search_len
             # while we break out the while loop, results.nodes[i] save the leaf node.
             results.nodes[i] = node
 
-    # print(f'env {i} one simulation done!')
-    return results, virtual_to_play
+    return results.latent_state_index_in_search_path, results.latent_state_index_in_batch, results.last_actions, virtual_to_play
 
 
 def backpropagate(
         search_path: List[Node], min_max_stats: MinMaxStats, to_play: int, value: float, discount_factor: float
 ) -> None:
     """
     Overview:
         Update the value sum and visit count of nodes along the search path.
     Arguments:
-        - search_path: a vector of nodes on the search path.
-        - min_max_stats: a tool used to min-max normalize the q value.
-        - to_play: which player to play the game in the current node.
-        - value: the value to propagate along the search path.
-        - discount_factor: the discount factor of reward.
+        - search_path (:obj:`List[Node]`): a vector of nodes on the search path.
+        - min_max_stats (:obj:`MinMaxStats`): a tool used to min-max normalize the q value.
+        - to_play (:obj:`int`): which player to play the game in the current node.
+        - value (:obj:`float`): the value to propagate along the search path.
+        - discount_factor (:obj:`float`): the discount factor of reward.
     """
-    assert to_play is None or to_play in [-1, 1, 2]
+    assert to_play is None or to_play in [-1, 1, 2], f'to_play is {to_play}!'
     if to_play is None or to_play == -1:
-        # for play-with-bot mode
+        # for play-with-bot-mode
         bootstrap_value = value
         path_len = len(search_path)
         for i in range(path_len - 1, -1, -1):
             node = search_path[i]
             node.value_sum += bootstrap_value
             node.visit_count += 1
-            true_reward = node.reward
+
+            parent_value_prefix = 0.0
+            is_reset = 0
+            if i >= 1:
+                parent = search_path[i - 1]
+                parent_value_prefix = parent.value_prefix
+                is_reset = parent.is_reset
+
+            true_reward = node.value_prefix - parent_value_prefix
             min_max_stats.update(true_reward + discount_factor * node.value)
+            if is_reset == 1:
+                true_reward = node.value_prefix
             bootstrap_value = true_reward + discount_factor * bootstrap_value
     else:
         # for self-play-mode
         bootstrap_value = value
         path_len = len(search_path)
         for i in range(path_len - 1, -1, -1):
             node = search_path[i]
-            # to_play related
+
             node.value_sum += bootstrap_value if node.to_play == to_play else -bootstrap_value
 
             node.visit_count += 1
+            parent_value_prefix = 0.0
+            is_reset = 0
+            if i >= 1:
+                parent = search_path[i - 1]
+                parent_value_prefix = parent.value_prefix
+                is_reset = parent.is_reset
+
+            # NOTE: in self-play-mode, value_prefix is not calculated according to the perspective of current player of node.
+            # TODO: true_reward = node.value_prefix - (- parent_value_prefix)
+            true_reward = node.value_prefix - parent_value_prefix
 
-            # NOTE: in self-play-mode,
-            # we should calculate the true_reward according to the perspective of current player of node
-            # true_reward = node.value_prefix - (- parent_value_prefix)
-            true_reward = node.reward
+            if is_reset == 1:
+                true_reward = node.value_prefix
 
-            # min_max_stats.update(true_reward + discount_factor * node.value)
             min_max_stats.update(true_reward + discount_factor * -node.value)
 
-            # TODO(pu): to_play related
             # true_reward is in the perspective of current player of node
-            bootstrap_value = (-true_reward if node.to_play == to_play else true_reward) + discount_factor * bootstrap_value
+            bootstrap_value = (
+                -true_reward if node.to_play == to_play else true_reward
+            ) + discount_factor * bootstrap_value
 
 
 def batch_backpropagate(
-        latent_state_index_in_search_path: int,
+        simulation_index: int,
         discount_factor: float,
-        value_prefixs: List[float],
+        value_prefixs: List,
         values: List[float],
         policies: List[float],
         min_max_stats_lst: List[MinMaxStats],
         results: SearchResults,
+        is_reset_list: List,
         to_play: list = None,
-        is_chance_list: list = None,
-        leaf_idx_list: list = None,
 ) -> None:
     """
     Overview:
-        Backpropagation along the search path to update the attributes.
+        Update the value sum and visit count of nodes along the search paths for each root in the batch.
     Arguments:
-        - latent_state_index_in_search_path (:obj:`Class Int`): the index of latent state vector.
-        - discount_factor (:obj:`Class Float`): discount_factor factor used i calculating bootstrapped value,
-            if env is board_games, we set discount_factor=1.
-        - value_prefixs (:obj:`Class List`): the value prefixs of nodes along the search path.
-        - values (:obj:`Class List`):  the values to propagate along the search path.
-        - policies (:obj:`Class List`): the policy logits of nodes along the search path.
-        - min_max_stats_lst (:obj:`Class List[MinMaxStats]`):  a tool used to min-max normalize the q value.
-        - results (:obj:`Class List`): the search results.
-        - to_play (:obj:`Class List`):  the batch of which player is playing on this node.
-    """
-    if leaf_idx_list is None:
-        leaf_idx_list = list(range(results.num))
-    for leaf_order, i in enumerate(leaf_idx_list):
+        - simulation_index (:obj:`int`): The index of latent state of the leaf node in the search path.
+        - discount_factor (:obj:`float`): The discount factor used in calculating bootstrapped value, if env is board_games, we set discount_factor=1.
+        - value_prefixs (:obj:`List`): the value prefixs of nodes along the search path.
+        - values (:obj:`List`):  the values to propagate along the search path.
+        - policies (:obj:`List`): the policy logits of nodes along the search path.
+        - min_max_stats_lst (:obj:`List[MinMaxStats]`):  a tool used to min-max normalize the q value.
+        - results (:obj:`List`): the search results.
+        - is_reset_list (:obj:`List`): the vector of is_reset nodes along the search path, where is_reset represents for whether the parent value prefix needs to be reset.
+        - to_play (:obj:`List`): the batch of which player is playing on this node.
+    """
+    for i in range(results.num):
         # ****** expand the leaf node ******
-        if to_play is None:
-            # set to_play=-1, because two_player mode to_play = {1,2}
-            results.nodes[i].expand(-1, latent_state_index_in_search_path, i, value_prefixs[leaf_order], policies[leaf_order], is_chance_list[i])
+        if to_play in [-1, None]:
+            # set to_play=-1, because in self-play-mode to_play = {1,2}
+            results.nodes[i].expand(-1, simulation_index, i, value_prefixs[i], policies[i])
         else:
-            results.nodes[i].expand(to_play[i], latent_state_index_in_search_path, i, value_prefixs[leaf_order], policies[leaf_order], is_chance_list[i])
+            results.nodes[i].expand(to_play[i], simulation_index, i, value_prefixs[i], policies[i])
+
+        # reset
+        results.nodes[i].is_reset = is_reset_list[i]
 
         # ****** backpropagate ******
-        if to_play is None:
-            backpropagate(results.search_paths[i], min_max_stats_lst.stats_lst[i], 0, values[leaf_order], discount_factor)
+        if to_play in [-1, None]:
+            backpropagate(results.search_paths[i], min_max_stats_lst.stats_lst[i], -1, values[i], discount_factor)
         else:
             backpropagate(
-                results.search_paths[i], min_max_stats_lst.stats_lst[i], to_play[i], values[leaf_order], discount_factor
+                results.search_paths[i], min_max_stats_lst.stats_lst[i], to_play[i], values[i], discount_factor
             )
```

### Comparing `LightZero-0.0.2/lzero/mcts/ptree/test_sez_sample.py` & `LightZero-0.0.5/lzero/mcts/ptree/test_sez_sample.py`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/lzero/mcts/tests/config/atari_efficientzero_config_for_test.py` & `LightZero-0.0.5/lzero/mcts/tests/config/atari_efficientzero_config_for_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from easydict import EasyDict
 
-env_name = 'PongNoFrameskip-v4'
+env_id = 'PongNoFrameskip-v4'
 action_space_size = 6
 
 # ==============================================================
 # begin of the most frequently changed config specified by the user
 # ==============================================================
 collector_env_num = 8
 n_episode = 8
@@ -17,27 +17,27 @@
 # ==============================================================
 # end of the most frequently changed config specified by the user
 # ==============================================================
 
 atari_efficientzero_config = dict(
     exp_name='data_ez_ctree/efficientzero_seed0',
     env=dict(
-        env_name=env_name,
+        env_id=env_id,
         obs_shape=(4, 96, 96),
         collector_env_num=collector_env_num,
         evaluator_env_num=evaluator_env_num,
         n_evaluator_episode=evaluator_env_num,
         manager=dict(shared_memory=False, ),
         env_type='Atari',
         max_episode_steps=int(1.08e5),
         gray_scale=True,
         frame_skip=4,
         episode_life=True,
         clip_rewards=True,
-        channel_last=True,
+        channel_last=False,
         render_mode_human=False,
         scale=True,
         warp_frame=True,
         save_video=False,
         transform2string=False,
         game_wrapper=True,
         stop_value=int(1e6),
```

### Comparing `LightZero-0.0.2/lzero/mcts/tests/config/tictactoe_muzero_bot_mode_config_for_test.py` & `LightZero-0.0.5/zoo/board_games/tictactoe/config/tictactoe_muzero_sp_mode_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,83 +2,70 @@
 
 # ==============================================================
 # begin of the most frequently changed config specified by the user
 # ==============================================================
 collector_env_num = 8
 n_episode = 8
 evaluator_env_num = 5
-num_simulations = 5
-update_per_collect = 10
-batch_size = 4
-max_env_step = int(2e6)
+num_simulations = 25
+update_per_collect = 50
+batch_size = 256
+max_env_step = int(2e5)
 reanalyze_ratio = 0.
 # ==============================================================
 # end of the most frequently changed config specified by the user
 # ==============================================================
 
 tictactoe_muzero_config = dict(
-    exp_name='data_mz_ctree/tictactoe_muzero_bot_mode_seed0',
+    exp_name=
+    f'data_mz_ctree/tictactoe_muzero_sp-mode_ns{num_simulations}_upc{update_per_collect}_rr{reanalyze_ratio}_seed0',
     env=dict(
-        battle_mode='play_with_bot_mode',
+        battle_mode='self_play_mode',
         collector_env_num=collector_env_num,
         evaluator_env_num=evaluator_env_num,
         n_evaluator_episode=evaluator_env_num,
         manager=dict(shared_memory=False, ),
-        env_name="TicTacToe",
-        mcts_mode='self_play_mode',  # only used in AlphaZero
-        bot_action_type='v0',  # {'v0', 'alpha_beta_pruning'}
-        agent_vs_human=False,
-        prob_random_agent=0,
-        prob_expert_agent=0,
-        channel_last=True,
-        scale=True,
-        stop_value=1,
     ),
     policy=dict(
-        sampled_algo=False,
-        gumbel_algo=False,
         model=dict(
             observation_shape=(3, 3, 3),
             action_space_size=9,
             image_channel=3,
-            # We use the small size model for tictactoe
+            # We use the small size model for tictactoe.
             num_res_blocks=1,
             num_channels=16,
-            frame_stack_num=1,
-            model_type='conv',
+            fc_reward_layers=[8],
+            fc_value_layers=[8],
+            fc_policy_layers=[8],
             support_scale=10,
             reward_support_size=21,
             value_support_size=21,
-            categorical_distribution=True,
         ),
         cuda=True,
         env_type='board_games',
-        transform2string=False,
-        gray_scale=False,
+        action_type='varied_action_space',
+        game_segment_length=9,
         update_per_collect=update_per_collect,
         batch_size=batch_size,
         optim_type='Adam',
         lr_piecewise_constant_decay=False,
-        learning_rate=0.003,  # lr for Adam optimizer
+        learning_rate=0.003,
         grad_clip_value=0.5,
-        manual_temperature_decay=True,
         num_simulations=num_simulations,
         reanalyze_ratio=reanalyze_ratio,
-        game_segment_length=5,
         # NOTE：In board_games, we set large td_steps to make sure the value target is the final outcome.
         td_steps=9,
         num_unroll_steps=3,
+        # NOTE：In board_games, we set discount_factor=1.
         discount_factor=1,
         n_episode=n_episode,
         eval_freq=int(2e3),
-        replay_buffer_size=int(3e3),
+        replay_buffer_size=int(1e4),
         collector_env_num=collector_env_num,
         evaluator_env_num=evaluator_env_num,
-        lstm_horizon_len=5,
-        use_ture_chance_label_in_chance_encoder=False,
     ),
 )
 tictactoe_muzero_config = EasyDict(tictactoe_muzero_config)
 main_config = tictactoe_muzero_config
 
 tictactoe_muzero_create_config = dict(
     env=dict(
@@ -89,7 +76,11 @@
     policy=dict(
         type='muzero',
         import_names=['lzero.policy.muzero'],
     ),
 )
 tictactoe_muzero_create_config = EasyDict(tictactoe_muzero_create_config)
 create_config = tictactoe_muzero_create_config
+
+if __name__ == "__main__":
+    from lzero.entry import train_muzero
+    train_muzero([main_config, create_config], seed=0, max_env_step=max_env_step)
```

### Comparing `LightZero-0.0.2/lzero/mcts/tests/cprofile_mcts_ptree.py` & `LightZero-0.0.5/lzero/mcts/tests/cprofile_mcts_ptree.py`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/lzero/mcts/tests/eval_tree_speed.py` & `LightZero-0.0.5/lzero/mcts/tests/eval_tree_speed.py`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/lzero/mcts/tests/test_game_buffer.py` & `LightZero-0.0.5/lzero/mcts/tests/test_game_buffer.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
         batch_size=10,
         transition_num=20,
         priority_prob_alpha=0.6,
         priority_prob_beta=0.4,
         replay_buffer_size=10000,
         env_type='not_board_games',
         use_priority=True,
+        action_type='fixed_action_space',
     )
 )
 
 
 @pytest.mark.unittest
 def test_push():
     buffer = EfficientZeroGameBuffer(config)
```

### Comparing `LightZero-0.0.2/lzero/mcts/tests/test_game_segment.py` & `LightZero-0.0.5/lzero/mcts/tests/test_game_segment.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,42 +2,56 @@
 import pytest
 import torch
 
 from lzero.mcts.buffer.game_segment import GameSegment
 from lzero.mcts.utils import prepare_observation
 from lzero.policy import select_action
 
-# args = ['EfficientZero', 'MuZero']
-args = ["MuZero"]
+args = ["MuZero"]  # ['EfficientZero', 'MuZero']
 
 
 @pytest.mark.unittest
 @pytest.mark.parametrize('test_algo', args)
 def test_game_segment(test_algo):
     # import different modules according to ``test_algo``
     if test_algo == 'EfficientZero':
         from lzero.mcts.tree_search.mcts_ctree import EfficientZeroMCTSCtree as MCTSCtree
         from lzero.model.efficientzero_model import EfficientZeroModel as Model
         from lzero.mcts.tests.config.atari_efficientzero_config_for_test import atari_efficientzero_config as config
-        from zoo.atari.envs.atari_lightzero_env import AtariLightZeroEnv
-        envs = [AtariLightZeroEnv(config.env) for _ in range(config.env.evaluator_env_num)]
+        from zoo.atari.envs.atari_lightzero_env import AtariEnvLightZero
+        envs = [AtariEnvLightZero(config.env) for _ in range(config.env.evaluator_env_num)]
 
     elif test_algo == 'MuZero':
         from lzero.mcts.tree_search.mcts_ctree import MuZeroMCTSCtree as MCTSCtree
         from lzero.model.muzero_model import MuZeroModel as Model
         from lzero.mcts.tests.config.tictactoe_muzero_bot_mode_config_for_test import tictactoe_muzero_config as config
         from zoo.board_games.tictactoe.envs.tictactoe_env import TicTacToeEnv
         envs = [TicTacToeEnv(config.env) for _ in range(config.env.evaluator_env_num)]
 
     # create model
     model = Model(**config.policy.model)
     if config.policy.cuda and torch.cuda.is_available():
         config.policy.device = 'cuda'
     else:
         config.policy.device = 'cpu'
+
+    # load pretrained model
+    if config.policy.model_path is not None:
+        # Load the state dictionary from the specified file path
+        state_dict = torch.load(config.policy.model_path, map_location=config.policy.device)
+        # Create a new state dictionary that contains only the matching keys
+        model_state_dict = model.state_dict()
+        matched_state_dict = {k: v for k, v in state_dict['model'].items() if k in model_state_dict}
+        # Load the matched state dictionary into the model
+        model.load_state_dict(matched_state_dict, strict=False)
+        # Print a message indicating the number of loaded parameters
+        num_loaded_params = len(matched_state_dict)
+        num_model_params = len(model_state_dict)
+        print(f"Loaded {num_loaded_params} out of {num_model_params} parameters from the state dictionary.")
+
     model.to(config.policy.device)
     model.eval()
 
     with torch.no_grad():
         # initializations
         init_observations = [env.reset() for env in envs]
         dones = np.array([False for _ in range(config.env.evaluator_env_num)])
@@ -69,15 +83,15 @@
             if test_algo == 'EfficientZero':
                 reward_hidden_state_roots = network_output.reward_hidden_state
                 value_prefix_pool = network_output.value_prefix
                 reward_hidden_state_roots = (
                     reward_hidden_state_roots[0].detach().cpu().numpy(),
                     reward_hidden_state_roots[1].detach().cpu().numpy()
                 )
-                # for atari env, all actions is legal_action
+                # for atari env, all actions are legal_action
                 legal_actions_list = [
                     [i for i in range(config.policy.model.action_space_size)]
                     for _ in range(config.env.evaluator_env_num)
                 ]
             elif test_algo == 'MuZero':
                 reward_pool = network_output.reward
                 # for board games, we use the all actions is legal_action
@@ -100,15 +114,15 @@
                 MCTSCtree(config.policy).search(roots, model, latent_state_roots, to_play)
 
             roots_distributions = roots.get_distributions()
             roots_values = roots.get_values()
 
             for i in range(config.env.evaluator_env_num):
                 distributions, value, env = roots_distributions[i], roots_values[i], envs[i]
-                # ``deterministic=True``  indicates that we select the argmax action instead of sampling.
+                # ``deterministic=True`` indicates that we select the argmax action instead of sampling.
                 action, _ = select_action(distributions, temperature=1, deterministic=True)
                 # ==============================================================
                 # the core initial_inference.
                 # ==============================================================
                 obs, reward, done, info = env.step(action)
                 obs = obs['observation']
```

### Comparing `LightZero-0.0.2/lzero/mcts/tests/test_mcts_ctree.py` & `LightZero-0.0.5/lzero/mcts/tests/test_mcts_ctree.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,14 +88,15 @@
     device='cpu',
     value_delta_max=0.01,
     model=dict(
         action_space_size=9,
         support_scale=300,
         categorical_distribution=True,
     ),
+    env_type='not_board_games',
 )
 
 batch_size = env_nums = policy_config.batch_size
 action_space_size = policy_config.model.action_space_size
 
 model = MuZeroModelFake(action_num=9)
 stack_obs = torch.zeros(size=(batch_size, 8), dtype=torch.float)
```

### Comparing `LightZero-0.0.2/lzero/mcts/tests/test_mcts_ptree.py` & `LightZero-0.0.5/lzero/mcts/tests/test_mcts_ptree.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,15 @@
         device='cpu',
         value_delta_max=0.01,
         model=dict(
             action_space_size=9,
             categorical_distribution=True,
             support_scale=300,
         ),
+        env_type='not_board_games',
     )
 )
 
 batch_size = env_nums = policy_config.batch_size
 action_space_size = policy_config.model.action_space_size
 
 model = MuZeroModelFake(action_num=9)
```

### Comparing `LightZero-0.0.2/lzero/mcts/tests/test_mcts_sampled_ctree.py` & `LightZero-0.0.5/lzero/mcts/tests/test_mcts_sampled_ctree.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,15 @@
             value_delta_max=0,
             model=dict(
                 continuous_action_space=True,
                 support_scale=300,
                 action_space_size=2,
                 categorical_distribution=True,
             ),
+            env_type='not_board_games',
         )
     )
 
     batch_size = env_nums = policy_config.batch_size
     model = MuZeroModelFake(action_num=policy_config.model.action_space_size * 2)
     stack_obs = torch.zeros(
         size=(
```

### Comparing `LightZero-0.0.2/lzero/mcts/tests/test_utils.py` & `LightZero-0.0.5/lzero/mcts/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/lzero/mcts/tree_search/mcts_ctree.py` & `LightZero-0.0.5/lzero/mcts/tree_search/mcts_ptree.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 import copy
 from typing import TYPE_CHECKING, List, Any, Union
 
 import numpy as np
 import torch
 from easydict import EasyDict
 
-from lzero.mcts.ctree.ctree_efficientzero import ez_tree as tree_efficientzero
-from lzero.mcts.ctree.ctree_muzero import mz_tree as tree_muzero
-from lzero.mcts.ctree.ctree_gumbel_muzero import gmz_tree as tree_gumbel_muzero
+import lzero.mcts.ptree.ptree_ez as tree_efficientzero
+import lzero.mcts.ptree.ptree_mz as tree_muzero
+from lzero.mcts.ptree import MinMaxStatsList
 from lzero.policy import InverseScalarTransform, to_detach_cpu_numpy
 
 if TYPE_CHECKING:
-    from lzero.mcts.ctree.ctree_efficientzero import ez_tree as ez_ctree
-    from lzero.mcts.ctree.ctree_muzero import mz_tree as mz_ctree
-    from lzero.mcts.ctree.ctree_gumbel_muzero import gmz_tree as gmz_ctree
+    import lzero.mcts.ptree.ptree_ez as ez_ptree
+    import lzero.mcts.ptree.ptree_mz as mz_ptree
 
-# ==============================================================
-# EfficientZero
-# ==============================================================
 
-
-class EfficientZeroMCTSCtree(object):
+class MuZeroMCTSPtree(object):
     """
     Overview:
-        MCTSCtree for EfficientZero. The core ``batch_traverse`` and ``batch_backpropagate`` function is implemented in C++.
+        The Python implementation of MCTS (batch format) for MuZero.  \
+        It completes the ``roots``and ``search`` methods by calling functions in module ``ptree_mz``, \
+        which are implemented in Python.
     Interfaces:
-        __init__, roots, search
-        
+        ``__init__``, ``roots``, ``search``
+
+    ..note::
+        The benefit of searching for a batch of nodes at the same time is that \
+        it can be parallelized during model inference, thus saving time.
     """
 
+    # the default_config for MuZeroMCTSPtree.
     config = dict(
         # (float) The alpha value used in the Dirichlet distribution for exploration at the root node of the search tree.
         root_dirichlet_alpha=0.3,
         # (float) The noise weight at the root node of the search tree.
         root_noise_weight=0.25,
         # (int) The base constant used in the PUCT formula for balancing exploration and exploitation during tree search.
         pb_c_base=19652,
@@ -40,178 +41,178 @@
         pb_c_init=1.25,
         # (float) The maximum change in value allowed during the backup step of the search tree update.
         value_delta_max=0.01,
     )
 
     @classmethod
     def default_config(cls: type) -> EasyDict:
+        """
+        Overview:
+            A class method that returns a default configuration in the form of an EasyDict object.
+        Returns:
+            - cfg (:obj:`EasyDict`): The dict of the default configuration.
+        """
+        # Create a deep copy of the `config` attribute of the class.
         cfg = EasyDict(copy.deepcopy(cls.config))
+        # Add a new attribute `cfg_type` to the `cfg` object.
         cfg.cfg_type = cls.__name__ + 'Dict'
         return cfg
 
     def __init__(self, cfg: EasyDict = None) -> None:
         """
         Overview:
-            Use the default configuration mechanism. If a user passes in a cfg with a key that matches an existing key
-            in the default configuration, the user-provided value will override the default configuration. Otherwise,
+            Use the default configuration mechanism. If a user passes in a cfg with a key that matches an existing key \
+            in the default configuration, the user-provided value will override the default configuration. Otherwise, \
             the default configuration will be used.
+        Arguments:
+            - cfg (:obj:`EasyDict`): The configuration passed in by the user.
         """
+        # Get the default configuration.
         default_config = self.default_config()
+        # Update the default configuration with the values provided by the user in ``cfg``.
         default_config.update(cfg)
         self._cfg = default_config
         self.inverse_scalar_transform_handle = InverseScalarTransform(
             self._cfg.model.support_scale, self._cfg.device, self._cfg.model.categorical_distribution
         )
 
     @classmethod
-    def roots(cls: int, active_collect_env_num: int, legal_actions: List[Any]) -> "ez_ctree.Roots":
+    def roots(cls: int, root_num: int, legal_actions: List[Any]) -> "mz_ptree.Roots":
         """
         Overview:
-            The initialization of CRoots with root num and legal action lists.
+            Initializes a batch of roots to search parallelly later.
         Arguments:
-            - root_num (:obj:'int'): the number of the current root.
-            - legal_action_list (:obj:'List'): the vector of the legal action of this root.
+            - root_num (:obj:`int`): the number of the roots in a batch.
+            - legal_action_list (:obj:`List[Any]`): the vector of the legal actions for the roots.
+
+        ..note::
+            The initialization is achieved by the ``Roots`` class from the ``ptree_mz`` module.
         """
-        from lzero.mcts.ctree.ctree_efficientzero import ez_tree as ctree
-        return ctree.Roots(active_collect_env_num, legal_actions)
+        return tree_muzero.Roots(root_num, legal_actions)
 
     def search(
-            self, roots: Any, model: torch.nn.Module, latent_state_roots: List[Any],
-            reward_hidden_state_roots: List[Any], to_play_batch: Union[int, List[Any]]
+            self,
+            roots: Any,
+            model: torch.nn.Module,
+            latent_state_roots: List[Any],
+            to_play_batch: Union[int, List[Any]] = -1
     ) -> None:
         """
         Overview:
-            Do MCTS for the roots (a batch of root nodes in parallel). Parallel in model inference.
-            Use the cpp ctree.
+            Do MCTS for a batch of roots. Parallel in model inference. \
+            Use Python to implement the tree search.
         Arguments:
-            - roots (:obj:`Any`): a batch of expanded root nodes
-            - latent_state_roots (:obj:`list`): the hidden states of the roots
-            - reward_hidden_state_roots (:obj:`list`): the value prefix hidden states in LSTM of the roots
-            - to_play_batch (:obj:`list`): the to_play_batch list used in self-play-mode board games
+            - roots (:obj:`Any`): a batch of expanded root nodes.
+            - latent_state_roots (:obj:`list`): the hidden states of the roots.
+            - model (:obj:`torch.nn.Module`): The model used for inference.
+            - to_play_batch (:obj:`list`): the to_play_batch list used in in self-play-mode board games.
+
+        .. note::
+            The core functions ``batch_traverse`` and ``batch_backpropagate`` are implemented in Python.
         """
         with torch.no_grad():
             model.eval()
 
             # preparation some constant
             batch_size = roots.num
             pb_c_base, pb_c_init, discount_factor = self._cfg.pb_c_base, self._cfg.pb_c_init, self._cfg.discount_factor
 
             # the data storage of latent states: storing the latent state of all the nodes in one search.
             latent_state_batch_in_search_path = [latent_state_roots]
-            # the data storage of value prefix hidden states in LSTM
-            reward_hidden_state_c_batch = [reward_hidden_state_roots[0]]
-            reward_hidden_state_h_batch = [reward_hidden_state_roots[1]]
 
             # minimax value storage
-            min_max_stats_lst = tree_efficientzero.MinMaxStatsList(batch_size)
-            min_max_stats_lst.set_delta(self._cfg.value_delta_max)
+            min_max_stats_lst = MinMaxStatsList(batch_size)
 
             for simulation_index in range(self._cfg.num_simulations):
                 # In each simulation, we expanded a new node, so in one search, we have ``num_simulations`` num of nodes at most.
 
                 latent_states = []
-                hidden_states_c_reward = []
-                hidden_states_h_reward = []
-
                 # prepare a result wrapper to transport results between python and c++ parts
-                results = tree_efficientzero.ResultsWrapper(num=batch_size)
+                results = tree_muzero.SearchResults(num=batch_size)
 
-                # latent_state_index_in_search_path: the first index of leaf node states in latent_state_batch_in_search_path, i.e. is current_latent_state_index in one the search.
-                # latent_state_index_in_batch: the second index of leaf node states in latent_state_batch_in_search_path, i.e. the index in the batch, whose maximum is ``batch_size``.
+                # latent_state_index_in_search_path: The first index of the latent state corresponding to the leaf node in latent_state_batch_in_search_path, that is, the search depth.
+                # latent_state_index_in_batch: The second index of the latent state corresponding to the leaf node in latent_state_batch_in_search_path, i.e. the index in the batch, whose maximum is ``batch_size``.
                 # e.g. the latent state of the leaf node in (x, y) is latent_state_batch_in_search_path[x, y], where x is current_latent_state_index, y is batch_index.
-                # The index of value prefix hidden state of the leaf node is in the same manner.
                 """
                 MCTS stage 1: Selection
                     Each simulation starts from the internal root state s0, and finishes when the simulation reaches a leaf node s_l.
                 """
-                latent_state_index_in_search_path, latent_state_index_in_batch, last_actions, virtual_to_play_batch = tree_efficientzero.batch_traverse(
-                    roots, pb_c_base, pb_c_init, discount_factor, min_max_stats_lst, results,
-                    copy.deepcopy(to_play_batch)
-                )
-                # obtain the search horizon for leaf nodes
-                search_lens = results.get_search_len()
+                if self._cfg.env_type == 'not_board_games':
+                    latent_state_index_in_search_path, latent_state_index_in_batch, last_actions, virtual_to_play_batch = tree_muzero.batch_traverse(
+                        roots, pb_c_base, pb_c_init, discount_factor, min_max_stats_lst, results, to_play_batch
+                    )
+                else:
+                    # the ``to_play_batch`` is only used in board games, here we need to deepcopy it to avoid changing the original data.
+                    latent_state_index_in_search_path, latent_state_index_in_batch, last_actions, virtual_to_play_batch = tree_muzero.batch_traverse(
+                        roots, pb_c_base, pb_c_init, discount_factor, min_max_stats_lst, results,
+                        copy.deepcopy(to_play_batch)
+                    )
 
                 # obtain the latent state for leaf node
                 for ix, iy in zip(latent_state_index_in_search_path, latent_state_index_in_batch):
                     latent_states.append(latent_state_batch_in_search_path[ix][iy])
-                    hidden_states_c_reward.append(reward_hidden_state_c_batch[ix][0][iy])
-                    hidden_states_h_reward.append(reward_hidden_state_h_batch[ix][0][iy])
-
-                latent_states = torch.from_numpy(np.asarray(latent_states)).to(self._cfg.device).float()
-                hidden_states_c_reward = torch.from_numpy(np.asarray(hidden_states_c_reward)).to(self._cfg.device
-                                                                                                 ).unsqueeze(0)
-                hidden_states_h_reward = torch.from_numpy(np.asarray(hidden_states_h_reward)).to(self._cfg.device
-                                                                                                 ).unsqueeze(0)
-                # .long() is only for discrete action
+                latent_states = torch.from_numpy(np.asarray(latent_states)).to(self._cfg.device)
+                # only for discrete action
                 last_actions = torch.from_numpy(np.asarray(last_actions)).to(self._cfg.device).long()
                 """
                 MCTS stage 2: Expansion
                     At the final time-step l of the simulation, the next_latent_state and reward/value_prefix are computed by the dynamics function.
                     Then we calculate the policy_logits and value for the leaf node (next_latent_state) by the prediction function. (aka. evaluation)
                 MCTS stage 3: Backup
                     At the end of the simulation, the statistics along the trajectory are updated.
                 """
-                network_output = model.recurrent_inference(
-                    latent_states, (hidden_states_c_reward, hidden_states_h_reward), last_actions
-                )
-
-                network_output.latent_state = to_detach_cpu_numpy(network_output.latent_state)
-                network_output.policy_logits = to_detach_cpu_numpy(network_output.policy_logits)
-                network_output.value = to_detach_cpu_numpy(self.inverse_scalar_transform_handle(network_output.value))
-                network_output.value_prefix = to_detach_cpu_numpy(self.inverse_scalar_transform_handle(network_output.value_prefix))
+                network_output = model.recurrent_inference(latent_states, last_actions)
 
-                network_output.reward_hidden_state = (
-                    network_output.reward_hidden_state[0].detach().cpu().numpy(),
-                    network_output.reward_hidden_state[1].detach().cpu().numpy()
-                )
+                if not model.training:
+                    # if not in training, obtain the scalars of the value/reward
+                    [
+                        network_output.latent_state, network_output.policy_logits, network_output.value,
+                        network_output.reward
+                    ] = to_detach_cpu_numpy(
+                        [
+                            network_output.latent_state,
+                            network_output.policy_logits,
+                            self.inverse_scalar_transform_handle(network_output.value),
+                            self.inverse_scalar_transform_handle(network_output.reward),
+                        ]
+                    )
 
                 latent_state_batch_in_search_path.append(network_output.latent_state)
                 # tolist() is to be compatible with cpp datatype.
-                value_prefix_batch = network_output.value_prefix.reshape(-1).tolist()
                 value_batch = network_output.value.reshape(-1).tolist()
+                reward_batch = network_output.reward.reshape(-1).tolist()
                 policy_logits_batch = network_output.policy_logits.tolist()
 
-                reward_latent_state_batch = network_output.reward_hidden_state
-                # reset the hidden states in LSTM every ``lstm_horizon_len`` steps in one search.
-                # which enable the model only need to predict the value prefix in a range (e.g.: [s0,...,s5])
-                assert self._cfg.lstm_horizon_len > 0
-                reset_idx = (np.array(search_lens) % self._cfg.lstm_horizon_len == 0)
-                assert len(reset_idx) == batch_size
-                reward_latent_state_batch[0][:, reset_idx, :] = 0
-                reward_latent_state_batch[1][:, reset_idx, :] = 0
-                is_reset_list = reset_idx.astype(np.int32).tolist()
-                reward_hidden_state_c_batch.append(reward_latent_state_batch[0])
-                reward_hidden_state_h_batch.append(reward_latent_state_batch[1])
-
                 # In ``batch_backpropagate()``, we first expand the leaf node using ``the policy_logits`` and
                 # ``reward`` predicted by the model, then perform backpropagation along the search path to update the
                 # statistics.
 
                 # NOTE: simulation_index + 1 is very important, which is the depth of the current leaf node.
                 current_latent_state_index = simulation_index + 1
-                tree_efficientzero.batch_backpropagate(
-                    current_latent_state_index, discount_factor, value_prefix_batch, value_batch, policy_logits_batch,
-                    min_max_stats_lst, results, is_reset_list, virtual_to_play_batch
+                tree_muzero.batch_backpropagate(
+                    current_latent_state_index, discount_factor, reward_batch, value_batch, policy_logits_batch,
+                    min_max_stats_lst, results, virtual_to_play_batch
                 )
 
 
-# ==============================================================
-# MuZero
-# ==============================================================
-
-
-class MuZeroMCTSCtree(object):
+class EfficientZeroMCTSPtree(object):
     """
     Overview:
-        MCTSCtree for MuZero. The core ``batch_traverse`` and ``batch_backpropagate`` function is implemented in C++.
-
+        The Python implementation of MCTS (batch format) for EfficientZero.  \
+        It completes the ``roots``and ``search`` methods by calling functions in module ``ptree_ez``, \
+        which are implemented in Python.
     Interfaces:
-        __init__, roots, search
+        ``__init__``, ``roots``, ``search``
+    
+    ..note::
+        The benefit of searching for a batch of nodes at the same time is that \
+        it can be parallelized during model inference, thus saving time.
     """
 
+    # the default_config for EfficientZeroMCTSPtree.
     config = dict(
         # (float) The alpha value used in the Dirichlet distribution for exploration at the root node of the search tree.
         root_dirichlet_alpha=0.3,
         # (float) The noise weight at the root node of the search tree.
         root_noise_weight=0.25,
         # (int) The base constant used in the PUCT formula for balancing exploration and exploitation during tree search.
         pb_c_base=19652,
@@ -219,260 +220,188 @@
         pb_c_init=1.25,
         # (float) The maximum change in value allowed during the backup step of the search tree update.
         value_delta_max=0.01,
     )
 
     @classmethod
     def default_config(cls: type) -> EasyDict:
+        """
+        Overview:
+            A class method that returns a default configuration in the form of an EasyDict object.
+        Returns:
+            - cfg (:obj:`EasyDict`): The dict of the default configuration.
+        """
+        # Create a deep copy of the `config` attribute of the class.
         cfg = EasyDict(copy.deepcopy(cls.config))
+        # Add a new attribute `cfg_type` to the `cfg` object.
         cfg.cfg_type = cls.__name__ + 'Dict'
         return cfg
 
     def __init__(self, cfg: EasyDict = None) -> None:
         """
         Overview:
             Use the default configuration mechanism. If a user passes in a cfg with a key that matches an existing key
             in the default configuration, the user-provided value will override the default configuration. Otherwise,
             the default configuration will be used.
+        Arguments:
+            - cfg (:obj:`EasyDict`): The configuration passed in by the user.
         """
+        # Get the default configuration.
         default_config = self.default_config()
+        # Update the default configuration with the values provided by the user in ``cfg``.
         default_config.update(cfg)
         self._cfg = default_config
         self.inverse_scalar_transform_handle = InverseScalarTransform(
             self._cfg.model.support_scale, self._cfg.device, self._cfg.model.categorical_distribution
         )
 
     @classmethod
-    def roots(cls: int, active_collect_env_num: int, legal_actions: List[Any]) -> "mz_ctree":
+    def roots(cls: int, root_num: int, legal_actions: List[Any]) -> "ez_ptree.Roots":
         """
         Overview:
-            The initialization of CRoots with root num and legal action lists.
+            Initializes a batch of roots to search parallelly later.
         Arguments:
-            - root_num (:obj:`int`): the number of the current root.
-            - legal_action_list (:obj:`list`): the vector of the legal action of this root.
+            - root_num (:obj:`int`): the number of the roots in a batch.
+            - legal_action_list (:obj:`List[Any]`): the vector of the legal actions for the roots.
+        
+        ..note::
+            The initialization is achieved by the ``Roots`` class from the ``ptree_ez`` module.
         """
-        from lzero.mcts.ctree.ctree_muzero import mz_tree as ctree
-        return ctree.Roots(active_collect_env_num, legal_actions)
+        return tree_efficientzero.Roots(root_num, legal_actions)
 
     def search(
-            self, roots: Any, model: torch.nn.Module, latent_state_roots: List[Any], to_play_batch: Union[int,
-                                                                                                          List[Any]]
+            self,
+            roots: Any,
+            model: torch.nn.Module,
+            latent_state_roots: List[Any],
+            reward_hidden_state_roots: List[Any],
+            to_play_batch: Union[int, List[Any]] = -1
     ) -> None:
         """
         Overview:
-            Do MCTS for the roots (a batch of root nodes in parallel). Parallel in model inference.
-            Use the cpp ctree.
+            Do MCTS for a batch of roots. Parallel in model inference. \
+            Use Python to implement the tree search.
         Arguments:
-            - roots (:obj:`Any`): a batch of expanded root nodes
-            - latent_state_roots (:obj:`list`): the hidden states of the roots
-            - to_play_batch (:obj:`list`): the to_play_batch list used in in self-play-mode board games
+            - roots (:obj:`Any`): a batch of expanded root nodes.
+            - latent_state_roots (:obj:`list`): the hidden states of the roots.
+            - reward_hidden_state_roots (:obj:`list`): the value prefix hidden states in LSTM of the roots.
+            - model (:obj:`torch.nn.Module`): The model used for inference.
+            - to_play_batch (:obj:`list`): the to_play_batch list used in in self-play-mode board games.
+        
+        .. note::
+            The core functions ``batch_traverse`` and ``batch_backpropagate`` are implemented in Python.
         """
         with torch.no_grad():
             model.eval()
 
             # preparation some constant
             batch_size = roots.num
             pb_c_base, pb_c_init, discount_factor = self._cfg.pb_c_base, self._cfg.pb_c_init, self._cfg.discount_factor
-            # the data storage of latent states: storing the latent state of all the nodes in the search.
+
+            # the data storage of latent states: storing the latent state of all the nodes in one search.
             latent_state_batch_in_search_path = [latent_state_roots]
 
+            # the data storage of value prefix hidden states in LSTM
+            reward_hidden_state_c_batch = [reward_hidden_state_roots[0]]
+            reward_hidden_state_h_batch = [reward_hidden_state_roots[1]]
+
             # minimax value storage
-            min_max_stats_lst = tree_muzero.MinMaxStatsList(batch_size)
-            min_max_stats_lst.set_delta(self._cfg.value_delta_max)
+            min_max_stats_lst = MinMaxStatsList(batch_size)
 
             for simulation_index in range(self._cfg.num_simulations):
                 # In each simulation, we expanded a new node, so in one search, we have ``num_simulations`` num of nodes at most.
 
                 latent_states = []
+                hidden_states_c_reward = []
+                hidden_states_h_reward = []
 
                 # prepare a result wrapper to transport results between python and c++ parts
-                results = tree_muzero.ResultsWrapper(num=batch_size)
+                results = tree_efficientzero.SearchResults(num=batch_size)
 
                 # latent_state_index_in_search_path: the first index of leaf node states in latent_state_batch_in_search_path, i.e. is current_latent_state_index in one the search.
                 # latent_state_index_in_batch: the second index of leaf node states in latent_state_batch_in_search_path, i.e. the index in the batch, whose maximum is ``batch_size``.
                 # e.g. the latent state of the leaf node in (x, y) is latent_state_batch_in_search_path[x, y], where x is current_latent_state_index, y is batch_index.
                 # The index of value prefix hidden state of the leaf node are in the same manner.
                 """
                 MCTS stage 1: Selection
                     Each simulation starts from the internal root state s0, and finishes when the simulation reaches a leaf node s_l.
                 """
-                latent_state_index_in_search_path, latent_state_index_in_batch, last_actions, virtual_to_play_batch = tree_muzero.batch_traverse(
-                    roots, pb_c_base, pb_c_init, discount_factor, min_max_stats_lst, results,
-                    copy.deepcopy(to_play_batch)
-                )
+                if self._cfg.env_type == 'not_board_games':
+                    latent_state_index_in_search_path, latent_state_index_in_batch, last_actions, virtual_to_play_batch = tree_efficientzero.batch_traverse(
+                        roots, pb_c_base, pb_c_init, discount_factor, min_max_stats_lst, results, to_play_batch
+                    )
+                else:
+                    latent_state_index_in_search_path, latent_state_index_in_batch, last_actions, virtual_to_play_batch = tree_efficientzero.batch_traverse(
+                        roots, pb_c_base, pb_c_init, discount_factor, min_max_stats_lst, results, copy.deepcopy(to_play_batch)
+                    )
+                # obtain the search horizon for leaf nodes
+                search_lens = results.search_lens
 
                 # obtain the latent state for leaf node
                 for ix, iy in zip(latent_state_index_in_search_path, latent_state_index_in_batch):
                     latent_states.append(latent_state_batch_in_search_path[ix][iy])
+                    hidden_states_c_reward.append(reward_hidden_state_c_batch[ix][0][iy])
+                    hidden_states_h_reward.append(reward_hidden_state_h_batch[ix][0][iy])
 
-                latent_states = torch.from_numpy(np.asarray(latent_states)).to(self._cfg.device).float()
+                latent_states = torch.from_numpy(np.asarray(latent_states)).to(self._cfg.device)
+                hidden_states_c_reward = torch.from_numpy(np.asarray(hidden_states_c_reward)).to(self._cfg.device
+                                                                                                 ).unsqueeze(0)
+                hidden_states_h_reward = torch.from_numpy(np.asarray(hidden_states_h_reward)).to(self._cfg.device
+                                                                                                 ).unsqueeze(0)
                 # .long() is only for discrete action
                 last_actions = torch.from_numpy(np.asarray(last_actions)).to(self._cfg.device).long()
                 """
                 MCTS stage 2: Expansion
                     At the final time-step l of the simulation, the next_latent_state and reward/value_prefix are computed by the dynamics function.
                     Then we calculate the policy_logits and value for the leaf node (next_latent_state) by the prediction function. (aka. evaluation)
                 MCTS stage 3: Backup
                     At the end of the simulation, the statistics along the trajectory are updated.
                 """
-                network_output = model.recurrent_inference(latent_states, last_actions)
-
-                network_output.latent_state = to_detach_cpu_numpy(network_output.latent_state)
-                network_output.policy_logits = to_detach_cpu_numpy(network_output.policy_logits)
-                network_output.value = to_detach_cpu_numpy(self.inverse_scalar_transform_handle(network_output.value))
-                network_output.reward = to_detach_cpu_numpy(self.inverse_scalar_transform_handle(network_output.reward))
-
-                latent_state_batch_in_search_path.append(network_output.latent_state)
-                # tolist() is to be compatible with cpp datatype.
-                reward_batch = network_output.reward.reshape(-1).tolist()
-                value_batch = network_output.value.reshape(-1).tolist()
-                policy_logits_batch = network_output.policy_logits.tolist()
-
-                # In ``batch_backpropagate()``, we first expand the leaf node using ``the policy_logits`` and
-                # ``reward`` predicted by the model, then perform backpropagation along the search path to update the
-                # statistics.
-
-                # NOTE: simulation_index + 1 is very important, which is the depth of the current leaf node.
-                current_latent_state_index = simulation_index + 1
-                tree_muzero.batch_backpropagate(
-                    current_latent_state_index, discount_factor, reward_batch, value_batch, policy_logits_batch,
-                    min_max_stats_lst, results, virtual_to_play_batch
+                network_output = model.recurrent_inference(
+                    latent_states, (hidden_states_c_reward, hidden_states_h_reward), last_actions
                 )
 
-class GumbelMuZeroMCTSCtree(object):
-    """
-    Overview:
-        MCTSCtree for Gumbel MuZero. The core ``batch_traverse`` and ``batch_backpropagate`` function is implemented in C++.
-    Interfaces:
-        __init__, roots, search
-        
-    """
-    config = dict(
-        # (int) The max limitation of simluation times during the simulation.
-        num_simulations=50,
-        # (float) The alpha value used in the Dirichlet distribution for exploration at the root node of the search tree.
-        root_dirichlet_alpha=0.3,
-        # (float) The noise weight at the root node of the search tree.
-        root_noise_weight=0.25,
-        # (float) The maximum change in value allowed during the backup step of the search tree update.
-        value_delta_max=0.01,
-    )
-
-    @classmethod
-    def default_config(cls: type) -> EasyDict:
-        cfg = EasyDict(copy.deepcopy(cls.config))
-        cfg.cfg_type = cls.__name__ + 'Dict'
-        return cfg
-
-    def __init__(self, cfg: EasyDict = None) -> None:
-        """
-        Overview:
-            Use the default configuration mechanism. If a user passes in a cfg with a key that matches an existing key
-            in the default configuration, the user-provided value will override the default configuration. Otherwise,
-            the default configuration will be used.
-        """
-        default_config = self.default_config()
-        default_config.update(cfg)
-        self._cfg = default_config
-        self.inverse_scalar_transform_handle = InverseScalarTransform(
-            self._cfg.model.support_scale, self._cfg.device, self._cfg.model.categorical_distribution
-        )
-    
-    @classmethod
-    def roots(cls: int, active_collect_env_num: int, legal_actions: List[Any]) -> "gmz_ctree":
-        """
-        Overview:
-            The initialization of CRoots with root num and legal action lists.
-        Arguments:
-            - root_num (:obj:`int`): the number of the current root.
-            - legal_action_list (:obj:`list`): the vector of the legal action of this root.
-        """
-        from lzero.mcts.ctree.ctree_gumbel_muzero import gmz_tree as ctree
-        return ctree.Roots(active_collect_env_num, legal_actions)
-
-    def search(self, roots: Any, model: torch.nn.Module, latent_state_roots: List[Any], to_play_batch: Union[int,
-                                                                                                          List[Any]]
-    ) -> None:
-        """
-        Overview:
-            Do MCTS for the roots (a batch of root nodes in parallel). Parallel in model inference.
-            Use the cpp tree.
-        Arguments:
-            - roots (:obj:`Any`): a batch of expanded root nodes
-            - latent_state_roots (:obj:`list`): the hidden states of the roots
-            - to_play_batch (:obj:`list`): the to_play_batch list used in two_player mode board games
-        """
-        with torch.no_grad():
-            model.eval()
-
-            # preparation some constant
-            batch_size = roots.num
-            device = self._cfg.device
-            discount_factor = self._cfg.discount_factor
-            # the data storage of hidden states: storing the states of all the tree nodes
-            latent_state_batch_in_search_path = [latent_state_roots]
-
-            # minimax value storage
-            min_max_stats_lst = tree_gumbel_muzero.MinMaxStatsList(batch_size)
-            min_max_stats_lst.set_delta(self._cfg.value_delta_max)
-
-            for simulation_index in range(self._cfg.num_simulations):
-                # In each simulation, we expanded a new node, so in one search, we have ``num_simulations`` num of nodes at most.
-
-                latent_states = []
-
-                # prepare a result wrapper to transport results between python and c++ parts
-                results = tree_gumbel_muzero.ResultsWrapper(num=batch_size)
-
-                # traverse to select actions for each root
-                # hidden_state_index_x_lst: the first index of leaf node states in hidden_state_pool
-                # hidden_state_index_y_lst: the second index of leaf node states in hidden_state_pool
-                # the hidden state of the leaf node is hidden_state_pool[x, y]; value prefix states are the same
-                """
-                MCTS stage 1: Selection
-                    Each simulation starts from the internal root state s0, and finishes when the simulation reaches a leaf node s_l.
-                    In gumbel muzero, the action at the root node is selected using the Sequential Halving algorithm, while the action 
-                    at the interier node is selected based on the completion of the action values.
-                """
-                latent_state_index_in_search_path, latent_state_index_in_batch, last_actions, virtual_to_play_batch = tree_gumbel_muzero.batch_traverse(
-                    roots, self._cfg.num_simulations, self._cfg.max_num_considered_actions, discount_factor, results, copy.deepcopy(to_play_batch)
+                [
+                    network_output.latent_state, network_output.policy_logits, network_output.value,
+                    network_output.value_prefix
+                ] = to_detach_cpu_numpy(
+                    [
+                        network_output.latent_state,
+                        network_output.policy_logits,
+                        self.inverse_scalar_transform_handle(network_output.value),
+                        self.inverse_scalar_transform_handle(network_output.value_prefix),
+                    ]
+                )
+                network_output.reward_hidden_state = (
+                    network_output.reward_hidden_state[0].detach().cpu().numpy(),
+                    network_output.reward_hidden_state[1].detach().cpu().numpy()
                 )
-
-                # obtain the states for leaf nodes
-                for ix, iy in zip(latent_state_index_in_search_path, latent_state_index_in_batch):
-                    latent_states.append(latent_state_batch_in_search_path[ix][iy])
-
-                latent_states = torch.from_numpy(np.asarray(latent_states)).to(device).float()
-                # .long() is only for discrete action
-                last_actions = torch.from_numpy(np.asarray(last_actions)).to(device).unsqueeze(1).long()
-                """
-                MCTS stage 2: Expansion
-                    At the final time-step l of the simulation, the next_latent_state and reward/value_prefix are computed by the dynamics function.
-                    Then we calculate the policy_logits and value for the leaf node (next_latent_state) by the prediction function. (aka. evaluation)
-                MCTS stage 3: Backup
-                    At the end of the simulation, the statistics along the trajectory are updated.
-                """
-                network_output = model.recurrent_inference(latent_states, last_actions)
-
-                network_output.latent_state = to_detach_cpu_numpy(network_output.latent_state)
-                network_output.policy_logits = to_detach_cpu_numpy(network_output.policy_logits)
-                network_output.value = to_detach_cpu_numpy(self.inverse_scalar_transform_handle(network_output.value))
-                network_output.reward = to_detach_cpu_numpy(self.inverse_scalar_transform_handle(network_output.reward))
 
                 latent_state_batch_in_search_path.append(network_output.latent_state)
+                reward_latent_state_batch = network_output.reward_hidden_state
                 # tolist() is to be compatible with cpp datatype.
-                reward_batch = network_output.reward.reshape(-1).tolist()
                 value_batch = network_output.value.reshape(-1).tolist()
+                value_prefix_batch = network_output.value_prefix.reshape(-1).tolist()
                 policy_logits_batch = network_output.policy_logits.tolist()
 
+                # reset the hidden states in LSTM every ``lstm_horizon_len`` steps in one search.
+                # which enable the model only need to predict the value prefix in a range (e.g.: [s0,...,s5]).
+                assert self._cfg.lstm_horizon_len > 0
+                reset_idx = (np.array(search_lens) % self._cfg.lstm_horizon_len == 0)
+                reward_latent_state_batch[0][:, reset_idx, :] = 0
+                reward_latent_state_batch[1][:, reset_idx, :] = 0
+                is_reset_list = reset_idx.astype(np.int32).tolist()
+                reward_hidden_state_c_batch.append(reward_latent_state_batch[0])
+                reward_hidden_state_h_batch.append(reward_latent_state_batch[1])
+
                 # In ``batch_backpropagate()``, we first expand the leaf node using ``the policy_logits`` and
                 # ``reward`` predicted by the model, then perform backpropagation along the search path to update the
                 # statistics.
 
                 # NOTE: simulation_index + 1 is very important, which is the depth of the current leaf node.
                 current_latent_state_index = simulation_index + 1
-
-                # backpropagation along the search path to update the attributes
-                tree_gumbel_muzero.batch_back_propagate(
-                    current_latent_state_index, discount_factor, reward_batch, value_batch, policy_logits_batch,
-                    min_max_stats_lst, results, virtual_to_play_batch
+                tree_efficientzero.batch_backpropagate(
+                    current_latent_state_index, discount_factor, value_prefix_batch, value_batch, policy_logits_batch,
+                    min_max_stats_lst, results, is_reset_list, virtual_to_play_batch
                 )
+
+
```

### Comparing `LightZero-0.0.2/lzero/mcts/tree_search/mcts_ctree_sampled.py` & `LightZero-0.0.5/lzero/mcts/tree_search/mcts_ptree_sampled.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 import copy
 from typing import TYPE_CHECKING, List, Any, Union
 
 import numpy as np
 import torch
 from easydict import EasyDict
 
-from lzero.mcts.ctree.ctree_sampled_efficientzero import ezs_tree as tree_efficientzero
+from lzero.mcts.ptree import MinMaxStatsList
 from lzero.policy import InverseScalarTransform, to_detach_cpu_numpy
 
 if TYPE_CHECKING:
-    from lzero.mcts.ctree.ctree_sampled_efficientzero import ezs_tree as ezs_ctree
+    import lzero.mcts.ptree.ptree_sez as ptree
 
-# ==============================================================
-# Sampled EfficientZero
-# ==============================================================
 
+import lzero.mcts.ptree.ptree_sez as tree_sez
 
-class SampledEfficientZeroMCTSCtree(object):
+
+class SampledEfficientZeroMCTSPtree(object):
     """
     Overview:
-        MCTSCtree for Sampled EfficientZero. The core ``batch_traverse`` and ``batch_backpropagate`` function is implemented in C++.
+        The Python implementation of MCTS (batch format) for Sampled EfficientZero.  \
+        It completes the ``roots``and ``search`` methods by calling functions in module ``ptree_sez``, \
+        which are implemented in Python.
     Interfaces:
-        __init__, roots, search
+        ``__init__``, ``roots``, ``search``
+    
+    ..note::
+        The benefit of searching for a batch of nodes at the same time is that \
+        it can be parallelized during model inference, thus saving time.
     """
 
-    # the default_config for SampledEfficientZeroMCTSCtree.
+    # the default_config for SampledEfficientZeroMCTSPtree.
     config = dict(
         # (float) The alpha value used in the Dirichlet distribution for exploration at the root node of the search tree.
         root_dirichlet_alpha=0.3,
         # (float) The noise weight at the root node of the search tree.
         root_noise_weight=0.25,
         # (int) The base constant used in the PUCT formula for balancing exploration and exploitation during tree search.
         pb_c_base=19652,
@@ -36,126 +41,153 @@
         pb_c_init=1.25,
         # (float) The maximum change in value allowed during the backup step of the search tree update.
         value_delta_max=0.01,
     )
 
     @classmethod
     def default_config(cls: type) -> EasyDict:
+        """
+        Overview:
+            A class method that returns a default configuration in the form of an EasyDict object.
+        Returns:
+            - cfg (:obj:`EasyDict`): The dict of the default configuration.
+        """
+        # Create a deep copy of the `config` attribute of the class.
         cfg = EasyDict(copy.deepcopy(cls.config))
+        # Add a new attribute `cfg_type` to the `cfg` object.
         cfg.cfg_type = cls.__name__ + 'Dict'
         return cfg
 
     def __init__(self, cfg: EasyDict = None) -> None:
         """
         Overview:
             Use the default configuration mechanism. If a user passes in a cfg with a key that matches an existing key
             in the default configuration, the user-provided value will override the default configuration. Otherwise,
             the default configuration will be used.
+        Arguments:
+            - cfg (:obj:`EasyDict`): The configuration passed in by the user.
         """
+        # Get the default configuration.
         default_config = self.default_config()
+        # Update the default configuration with the values provided by the user in ``cfg``.
         default_config.update(cfg)
         self._cfg = default_config
         self.inverse_scalar_transform_handle = InverseScalarTransform(
             self._cfg.model.support_scale, self._cfg.device, self._cfg.model.categorical_distribution
         )
 
     @classmethod
     def roots(
             cls: int, root_num: int, legal_action_lis: List[Any], action_space_size: int, num_of_sampled_actions: int,
             continuous_action_space: bool
-    ) -> "ezs_ctree.Roots":
+    ) -> "ptree.Roots":
         """
         Overview:
-            Initialization of CNode with root_num, legal_actions_list, action_space_size, num_of_sampled_actions, continuous_action_space.
+            Initializes a batch of roots to search parallelly later.
         Arguments:
-            - root_num (:obj:'int'): the number of the current root.
-            - legal_action_list (:obj:'List'): the vector of the legal action of this root.
+            - root_num (:obj:`int`): the number of the roots in a batch.
+            - legal_action_list (:obj:`List[Any]`): the vector of the legal actions for the roots.
             - action_space_size (:obj:'int'): the size of action space of the current env.
-            - num_of_sampled_actions (:obj:'int'): the number of sampled actions, i.e. K in the Sampled MuZero papers.
+            - num_of_sampled_actions (:obj:'int'): The number of sampled actions, i.e. K in the Sampled MuZero paper.
             - continuous_action_space (:obj:'bool'): whether the action space is continous in current env.
+        
+        ..note::
+            The initialization is achieved by the ``Roots`` class from the ``ptree_sez`` module.
         """
-        from lzero.mcts.ctree.ctree_sampled_efficientzero import ezs_tree as ctree
-        return ctree.Roots(
+        return tree_sez.Roots(
             root_num, legal_action_lis, action_space_size, num_of_sampled_actions, continuous_action_space
         )
 
     def search(
-            self, roots: Any, model: torch.nn.Module, latent_state_roots: List[Any],
-            reward_hidden_state_roots: List[Any], to_play_batch: Union[int, List[Any]]
+            self,
+            roots: Any,
+            model: torch.nn.Module,
+            latent_state_roots: List[Any],
+            reward_hidden_state_roots: List[Any],
+            to_play_batch: Union[int, List[Any]] = -1
     ) -> None:
         """
         Overview:
-            Do MCTS for the roots (a batch of root nodes in parallel). Parallel in model inference.
-             Use the cpp ctree.
+            Do MCTS for a batch of roots. Parallel in model inference. \
+            Use Python to implement the tree search.
         Arguments:
-            - roots (:obj:`Any`): a batch of expanded root nodes
-            - model (:obj:`torch.nn.Module`): Instance of torch.nn.Module.
-            - latent_state_roots (:obj:`list`): the hidden states of the roots
-            - reward_hidden_state_roots (:obj:`list`): the value prefix hidden states in LSTM of the roots
-            - to_play_batch (:obj:`list`): the to_play_batch list used in in self-play-mode board games
+            - roots (:obj:`Any`): a batch of expanded root nodes.
+            - model (:obj:`torch.nn.Module`): The model used for inference.
+            - latent_state_roots (:obj:`list`): the hidden states of the roots.
+            - reward_hidden_state_roots (:obj:`list`): the value prefix hidden states in LSTM of the roots.
+            - to_play_batch (:obj:`list`): the to_play_batch list used in in self-play-mode board games.
+        
+        .. note::
+            The core functions ``batch_traverse`` and ``batch_backpropagate`` are implemented in Python.
         """
         with torch.no_grad():
             model.eval()
 
             # preparation some constant
             batch_size = roots.num
-            device = self._cfg.device
             pb_c_base, pb_c_init, discount_factor = self._cfg.pb_c_base, self._cfg.pb_c_init, self._cfg.discount_factor
 
             # the data storage of latent states: storing the latent state of all the nodes in one search.
             latent_state_batch_in_search_path = [latent_state_roots]
             # the data storage of value prefix hidden states in LSTM
-            reward_hidden_state_c_pool = [reward_hidden_state_roots[0]]
-            reward_hidden_state_h_pool = [reward_hidden_state_roots[1]]
+            reward_hidden_state_c_batch = [reward_hidden_state_roots[0]]
+            reward_hidden_state_h_batch = [reward_hidden_state_roots[1]]
 
             # minimax value storage
-            min_max_stats_lst = tree_efficientzero.MinMaxStatsList(batch_size)
-            min_max_stats_lst.set_delta(self._cfg.value_delta_max)
+            min_max_stats_lst = MinMaxStatsList(batch_size)
 
             for simulation_index in range(self._cfg.num_simulations):
                 # In each simulation, we expanded a new node, so in one search, we have ``num_simulations`` num of nodes at most.
 
                 latent_states = []
                 hidden_states_c_reward = []
                 hidden_states_h_reward = []
 
                 # prepare a result wrapper to transport results between python and c++ parts
-                results = tree_efficientzero.ResultsWrapper(num=batch_size)
+                results = tree_sez.SearchResults(num=batch_size)
 
                 # latent_state_index_in_search_path: the first index of leaf node states in latent_state_batch_in_search_path, i.e. is current_latent_state_index in one the search.
                 # latent_state_index_in_batch: the second index of leaf node states in latent_state_batch_in_search_path, i.e. the index in the batch, whose maximum is ``batch_size``.
                 # e.g. the latent state of the leaf node in (x, y) is latent_state_batch_in_search_path[x, y], where x is current_latent_state_index, y is batch_index.
                 # The index of value prefix hidden state of the leaf node are in the same manner.
                 """
                 MCTS stage 1: Selection
                     Each simulation starts from the internal root state s0, and finishes when the simulation reaches a leaf node s_l.
                 """
-                latent_state_index_in_search_path, latent_state_index_in_batch, last_actions, virtual_to_play_batch = tree_efficientzero.batch_traverse(
-                    roots, pb_c_base, pb_c_init, discount_factor, min_max_stats_lst, results,
-                    copy.deepcopy(to_play_batch), self._cfg.model.continuous_action_space
-                )
-
+                if self._cfg.env_type == 'not_board_games':
+                    latent_state_index_in_search_path, latent_state_index_in_batch, last_actions, virtual_to_play_batch = tree_sez.batch_traverse(
+                        roots, pb_c_base, pb_c_init, discount_factor, min_max_stats_lst, results, to_play_batch,
+                        self._cfg.model.continuous_action_space
+                    )
+                else:
+                    # the ``to_play_batch`` is only used in board games, here we need to deepcopy it to avoid changing the original data.
+                    latent_state_index_in_search_path, latent_state_index_in_batch, last_actions, virtual_to_play_batch = tree_sez.batch_traverse(
+                        roots, pb_c_base, pb_c_init, discount_factor, min_max_stats_lst, results, copy.deepcopy(to_play_batch),
+                        self._cfg.model.continuous_action_space
+                    )
                 # obtain the search horizon for leaf nodes
-                search_lens = results.get_search_len()
+                search_lens = results.search_lens
+
                 # obtain the latent state for leaf node
                 for ix, iy in zip(latent_state_index_in_search_path, latent_state_index_in_batch):
                     latent_states.append(latent_state_batch_in_search_path[ix][iy])
-                    hidden_states_c_reward.append(reward_hidden_state_c_pool[ix][0][iy])
-                    hidden_states_h_reward.append(reward_hidden_state_h_pool[ix][0][iy])
-                latent_states = torch.from_numpy(np.asarray(latent_states)).to(device).float()
-                hidden_states_c_reward = torch.from_numpy(np.asarray(hidden_states_c_reward)).to(device).unsqueeze(0)
-                hidden_states_h_reward = torch.from_numpy(np.asarray(hidden_states_h_reward)).to(device).unsqueeze(0)
+                    hidden_states_c_reward.append(reward_hidden_state_c_batch[ix][0][iy])
+                    hidden_states_h_reward.append(reward_hidden_state_h_batch[ix][0][iy])
+
+                latent_states = torch.from_numpy(np.asarray(latent_states)).to(self._cfg.device)
+                hidden_states_c_reward = torch.from_numpy(np.asarray(hidden_states_c_reward)).to(self._cfg.device).unsqueeze(0)
+                hidden_states_h_reward = torch.from_numpy(np.asarray(hidden_states_h_reward)).to(self._cfg.device).unsqueeze(0)
 
                 if self._cfg.model.continuous_action_space is True:
                     # continuous action
-                    last_actions = torch.from_numpy(np.asarray(last_actions)).to(device).float()
-
+                    last_actions = torch.from_numpy(np.asarray(last_actions)).to(self._cfg.device)
                 else:
                     # discrete action
-                    last_actions = torch.from_numpy(np.asarray(last_actions)).to(device).long()
+                    last_actions = torch.from_numpy(np.asarray(last_actions)).to(self._cfg.device).long()
+
                 """
                 MCTS stage 2: Expansion
                     At the final time-step l of the simulation, the next_latent_state and reward/value_prefix are computed by the dynamics function.
                     Then we calculate the policy_logits and value for the leaf node (next_latent_state) by the prediction function. (aka. evaluation)
                 MCTS stage 3: Backup
                     At the end of the simulation, the statistics along the trajectory are updated.
                 """
@@ -174,35 +206,35 @@
                         self.inverse_scalar_transform_handle(network_output.value_prefix),
                     ]
                 )
                 network_output.reward_hidden_state = (
                     network_output.reward_hidden_state[0].detach().cpu().numpy(),
                     network_output.reward_hidden_state[1].detach().cpu().numpy()
                 )
+
                 latent_state_batch_in_search_path.append(network_output.latent_state)
-                # tolist() is to be compatible with cpp datatype.
-                value_prefix_pool = network_output.value_prefix.reshape(-1).tolist()
-                value_pool = network_output.value.reshape(-1).tolist()
-                policy_logits_pool = network_output.policy_logits.tolist()
                 reward_latent_state_batch = network_output.reward_hidden_state
+                # tolist() is to be compatible with cpp datatype.
+                value_batch = network_output.value.reshape(-1).tolist()
+                value_prefix_batch = network_output.value_prefix.reshape(-1).tolist()
+                policy_logits_batch = network_output.policy_logits.tolist()
 
                 # reset the hidden states in LSTM every ``lstm_horizon_len`` steps in one search.
                 # which enable the model only need to predict the value prefix in a range (e.g.: [s0,...,s5]).
                 assert self._cfg.lstm_horizon_len > 0
                 reset_idx = (np.array(search_lens) % self._cfg.lstm_horizon_len == 0)
-                assert len(reset_idx) == batch_size
                 reward_latent_state_batch[0][:, reset_idx, :] = 0
                 reward_latent_state_batch[1][:, reset_idx, :] = 0
                 is_reset_list = reset_idx.astype(np.int32).tolist()
-                reward_hidden_state_c_pool.append(reward_latent_state_batch[0])
-                reward_hidden_state_h_pool.append(reward_latent_state_batch[1])
+                reward_hidden_state_c_batch.append(reward_latent_state_batch[0])
+                reward_hidden_state_h_batch.append(reward_latent_state_batch[1])
 
                 # In ``batch_backpropagate()``, we first expand the leaf node using ``the policy_logits`` and
                 # ``reward`` predicted by the model, then perform backpropagation along the search path to update the
                 # statistics.
 
                 # NOTE: simulation_index + 1 is very important, which is the depth of the current leaf node.
                 current_latent_state_index = simulation_index + 1
-                tree_efficientzero.batch_backpropagate(
-                    current_latent_state_index, discount_factor, value_prefix_pool, value_pool, policy_logits_pool,
+                tree_sez.batch_backpropagate(
+                    current_latent_state_index, discount_factor, value_prefix_batch, value_batch, policy_logits_batch,
                     min_max_stats_lst, results, is_reset_list, virtual_to_play_batch
                 )
```

### Comparing `LightZero-0.0.2/lzero/mcts/tree_search/mcts_ctree_stochastic.py` & `LightZero-0.0.5/lzero/mcts/tree_search/mcts_ctree_stochastic.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 import torch
 from easydict import EasyDict
 
 from lzero.policy import InverseScalarTransform
 from lzero.mcts.ctree.ctree_stochastic_muzero import stochastic_mz_tree
 
 
-# ==============================================================
-# Stochastic MuZero
-# ==============================================================
-
-
 class StochasticMuZeroMCTSCtree(object):
     """
     Overview:
-        MCTSCtree for Stochastic MuZero. The core ``batch_traverse`` and ``batch_backpropagate`` function is implemented in C++.
-
+        The C++ implementation of MCTS (batch format) for Stochastic MuZero.  \
+        It completes the ``roots``and ``search`` methods by calling functions in module ``ctree_stochastic_muzero``, \
+        which are implemented in C++.
     Interfaces:
-        __init__, roots, search
+        ``__init__``, ``roots``, ``search``
+    
+    ..note::
+        The benefit of searching for a batch of nodes at the same time is that \
+        it can be parallelized during model inference, thus saving time.
     """
 
     config = dict(
         # (float) The alpha value used in the Dirichlet distribution for exploration at the root node of the search tree.
         root_dirichlet_alpha=0.3,
         # (float) The noise weight at the root node of the search tree.
         root_noise_weight=0.25,
@@ -34,57 +34,75 @@
         pb_c_init=1.25,
         # (float) The maximum change in value allowed during the backup step of the search tree update.
         value_delta_max=0.01,
     )
 
     @classmethod
     def default_config(cls: type) -> EasyDict:
+        """
+        Overview:
+            A class method that returns a default configuration in the form of an EasyDict object.
+        Returns:
+            - cfg (:obj:`EasyDict`): The dict of the default configuration.
+        """
+        # Create a deep copy of the `config` attribute of the class.
         cfg = EasyDict(copy.deepcopy(cls.config))
+        # Add a new attribute `cfg_type` to the `cfg` object.
         cfg.cfg_type = cls.__name__ + 'Dict'
         return cfg
 
     def __init__(self, cfg: EasyDict = None) -> None:
         """
         Overview:
             Use the default configuration mechanism. If a user passes in a cfg with a key that matches an existing key
             in the default configuration, the user-provided value will override the default configuration. Otherwise,
             the default configuration will be used.
+        Arguments:
+            - cfg (:obj:`EasyDict`): The configuration passed in by the user.
         """
+        # Get the default configuration.
         default_config = self.default_config()
+        # Update the default configuration with the values provided by the user in ``cfg``.
         default_config.update(cfg)
         self._cfg = default_config
         self.inverse_scalar_transform_handle = InverseScalarTransform(
             self._cfg.model.support_scale, self._cfg.device, self._cfg.model.categorical_distribution
         )
 
     @classmethod
     def roots(cls: int, active_collect_env_num: int, legal_actions: List[Any],
               chance_space_size: int = 2) -> "stochastic_mz_tree.Roots":
         """
         Overview:
-            The initialization of CRoots with root num and legal action lists.
+            Initializes a batch of roots to search parallelly later.
         Arguments:
-            - root_num (:obj:`int`): the number of the current root.
-            - legal_action_list (:obj:`list`): the vector of the legal action of this root.
+            - root_num (:obj:`int`): the number of the roots in a batch.
+            - legal_action_list (:obj:`List[Any]`): the vector of the legal actions for the roots.
+        
+        ..note::
+            The initialization is achieved by the ``Roots`` class from the ``ctree_stochastic_muzero`` module.
         """
-        from lzero.mcts.ctree.ctree_stochastic_muzero import stochastic_mz_tree as ctree
-        return ctree.Roots(active_collect_env_num, legal_actions, chance_space_size)
+        return stochastic_mz_tree.Roots(active_collect_env_num, legal_actions, chance_space_size)
 
     def search(
             self, roots: Any, model: torch.nn.Module, latent_state_roots: List[Any], to_play_batch: Union[int,
             List[Any]]
     ) -> None:
         """
         Overview:
-            Do MCTS for the roots (a batch of root nodes in parallel). Parallel in model inference.
-             Use the cpp ctree.
+            Do MCTS for a batch of roots. Parallel in model inference. \
+            Use C++ to implement the tree search.
         Arguments:
-            - roots (:obj:`Any`): a batch of expanded root nodes
-            - latent_state_roots (:obj:`list`): the hidden states of the roots
-            - to_play_batch (:obj:`list`): the to_play_batch list used in in self-play-mode board games
+            - roots (:obj:`Any`): a batch of expanded root nodes.
+            - latent_state_roots (:obj:`list`): the hidden states of the roots.
+            - model (:obj:`torch.nn.Module`): The model used for inference.
+            - to_play (:obj:`list`): the to_play list used in in self-play-mode board games.
+        
+        .. note::
+            The core functions ``batch_traverse`` and ``batch_backpropagate`` are implemented in C++.
         """
         with torch.no_grad():
             model.eval()
 
             # preparation some constant
             batch_size = roots.num
             pb_c_base, pb_c_init, discount_factor = self._cfg.pb_c_base, self._cfg.pb_c_init, self._cfg.discount_factor
@@ -107,24 +125,31 @@
                 # latent_state_index_in_batch: the second index of leaf node states in latent_state_batch_in_search_path, i.e. the index in the batch, whose maximum is ``batch_size``.
                 # e.g. the latent state of the leaf node in (x, y) is latent_state_batch_in_search_path[x, y], where x is current_latent_state_index, y is batch_index.
                 # The index of value prefix hidden state of the leaf node are in the same manner.
                 """
                 MCTS stage 1: Selection
                     Each simulation starts from the internal root state s0, and finishes when the simulation reaches a leaf node s_l.
                 """
-                leaf_node_is_chance, latent_state_index_in_search_path, latent_state_index_in_batch, last_actions, virtual_to_play_batch = stochastic_mz_tree.batch_traverse(
-                    roots, pb_c_base, pb_c_init, discount_factor, min_max_stats_lst, results,
-                    copy.deepcopy(to_play_batch)
-                )
+                if self._cfg.env_type == 'not_board_games':
+                    leaf_node_is_chance, latent_state_index_in_search_path, latent_state_index_in_batch, last_actions, virtual_to_play_batch = stochastic_mz_tree.batch_traverse(
+                        roots, pb_c_base, pb_c_init, discount_factor, min_max_stats_lst, results,
+                        to_play_batch
+                    )
+                else:
+                    # the ``to_play_batch`` is only used in board games, here we need to deepcopy it to avoid changing the original data.
+                    leaf_node_is_chance, latent_state_index_in_search_path, latent_state_index_in_batch, last_actions, virtual_to_play_batch = stochastic_mz_tree.batch_traverse(
+                        roots, pb_c_base, pb_c_init, discount_factor, min_max_stats_lst, results,
+                        copy.deepcopy(to_play_batch)
+                    )
 
                 # obtain the latent state for leaf node
                 for ix, iy in zip(latent_state_index_in_search_path, latent_state_index_in_batch):
                     latent_states.append(latent_state_batch_in_search_path[ix][iy])
 
-                latent_states = torch.from_numpy(np.asarray(latent_states)).to(self._cfg.device).float()
+                latent_states = torch.from_numpy(np.asarray(latent_states)).to(self._cfg.device)
                 # .long() is only for discrete action
                 last_actions = torch.from_numpy(np.asarray(last_actions)).to(self._cfg.device).long()
                 """
                 MCTS stage 2: Expansion
                     At the final time-step l of the simulation, the next_latent_state and reward/value_prefix are computed by the dynamics function.
                     Then we calculate the policy_logits and value for the leaf node (next_latent_state) by the prediction function. (aka. evaluation)
                 MCTS stage 3: Backup
```

### Comparing `LightZero-0.0.2/lzero/mcts/tree_search/mcts_ptree.py` & `LightZero-0.0.5/lzero/mcts/tree_search/mcts_ptree_stochastic.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,37 @@
+import copy
 from typing import TYPE_CHECKING, List, Any, Union
-from easydict import EasyDict
 
-import copy
 import numpy as np
 import torch
+from easydict import EasyDict
 
+import lzero.mcts.ptree.ptree_stochastic_mz as tree_stochastic_muzero
 from lzero.mcts.ptree import MinMaxStatsList
-from lzero.policy import InverseScalarTransform, to_detach_cpu_numpy
-import lzero.mcts.ptree.ptree_mz as tree_muzero
+from lzero.policy import InverseScalarTransform
 
 if TYPE_CHECKING:
-    import lzero.mcts.ptree.ptree_ez as ez_ptree
-    import lzero.mcts.ptree.ptree_mz as mz_ptree
+    import lzero.mcts.ptree.ptree_stochastic_mz as stochastic_mz_ptree
 
-# ==============================================================
-# EfficientZero
-# ==============================================================
-import lzero.mcts.ptree.ptree_ez as tree
 
-
-class EfficientZeroMCTSPtree(object):
+class StochasticMuZeroMCTSPtree(object):
     """
     Overview:
-        MCTSPtree for EfficientZero. The core ``batch_traverse`` and ``batch_backpropagate`` function is implemented in python.
+        The Python implementation of MCTS (batch format) for Stochastic MuZero.  \
+        It completes the ``roots``and ``search`` methods by calling functions in module ``ptree_stochastic_mz``, \
+        which are implemented in Python.
     Interfaces:
-        __init__, roots, search
+        ``__init__``, ``roots``, ``search``
+
+    ..note::
+        The benefit of searching for a batch of nodes at the same time is that \
+        it can be parallelized during model inference, thus saving time.
     """
 
-    # the default_config for EfficientZeroMCTSPtree.
+    # the default_config for MuZeroMCTSPtree.
     config = dict(
         # (float) The alpha value used in the Dirichlet distribution for exploration at the root node of the search tree.
         root_dirichlet_alpha=0.3,
         # (float) The noise weight at the root node of the search tree.
         root_noise_weight=0.25,
         # (int) The base constant used in the PUCT formula for balancing exploration and exploitation during tree search.
         pb_c_base=19652,
@@ -39,316 +39,216 @@
         pb_c_init=1.25,
         # (float) The maximum change in value allowed during the backup step of the search tree update.
         value_delta_max=0.01,
     )
 
     @classmethod
     def default_config(cls: type) -> EasyDict:
-        cfg = EasyDict(copy.deepcopy(cls.config))
-        cfg.cfg_type = cls.__name__ + 'Dict'
-        return cfg
-
-    def __init__(self, cfg: EasyDict = None) -> None:
         """
         Overview:
-            Use the default configuration mechanism. If a user passes in a cfg with a key that matches an existing key
-            in the default configuration, the user-provided value will override the default configuration. Otherwise,
-            the default configuration will be used.
-        """
-        default_config = self.default_config()
-        default_config.update(cfg)
-        self._cfg = default_config
-        self.inverse_scalar_transform_handle = InverseScalarTransform(
-            self._cfg.model.support_scale, self._cfg.device, self._cfg.model.categorical_distribution
-        )
-
-    @classmethod
-    def roots(cls: int, root_num: int, legal_actions: List[Any]) -> "ez_ptree.Roots":
-        """
-        Overview:
-            The initialization of CRoots with root num and legal action lists.
-        Arguments:
-            - root_num: the number of the current root.
-            - legal_action_list: the vector of the legal action of this root.
+            A class method that returns a default configuration in the form of an EasyDict object.
+        Returns:
+            - cfg (:obj:`EasyDict`): The dict of the default configuration.
         """
-        import lzero.mcts.ptree.ptree_ez as ptree
-        return ptree.Roots(root_num, legal_actions)
-
-    def search(
-            self,
-            roots: Any,
-            model: torch.nn.Module,
-            latent_state_roots: List[Any],
-            reward_hidden_state_roots: List[Any],
-            to_play: Union[int, List[Any]] = -1
-    ) -> None:
-        """
-        Overview:
-            Do MCTS for the roots (a batch of root nodes in parallel). Parallel in model inference.
-            Use the python ctree.
-        Arguments:
-            - roots (:obj:`Any`): a batch of expanded root nodes
-            - latent_state_roots (:obj:`list`): the hidden states of the roots
-            - reward_hidden_state_roots (:obj:`list`): the value prefix hidden states in LSTM of the roots
-            - to_play (:obj:`list`): the to_play list used in in self-play-mode board games
-        """
-        with torch.no_grad():
-            model.eval()
-
-            # preparation some constant
-            batch_size = roots.num
-            pb_c_base, pb_c_init, discount_factor = self._cfg.pb_c_base, self._cfg.pb_c_init, self._cfg.discount_factor
-
-            # the data storage of latent states: storing the latent state of all the nodes in one search.
-            latent_state_batch_in_search_path = [latent_state_roots]
-
-            # the data storage of value prefix hidden states in LSTM
-            reward_hidden_state_c_batch = [reward_hidden_state_roots[0]]
-            reward_hidden_state_h_batch = [reward_hidden_state_roots[1]]
-
-            # minimax value storage
-            min_max_stats_lst = MinMaxStatsList(batch_size)
-
-            for simulation_index in range(self._cfg.num_simulations):
-                # In each simulation, we expanded a new node, so in one search, we have ``num_simulations`` num of nodes at most.
-
-                latent_states = []
-                hidden_states_c_reward = []
-                hidden_states_h_reward = []
-
-                # prepare a result wrapper to transport results between python and c++ parts
-                results = tree.SearchResults(num=batch_size)
-
-                # latent_state_index_in_search_path: the first index of leaf node states in latent_state_batch_in_search_path, i.e. is current_latent_state_index in one the search.
-                # latent_state_index_in_batch: the second index of leaf node states in latent_state_batch_in_search_path, i.e. the index in the batch, whose maximum is ``batch_size``.
-                # e.g. the latent state of the leaf node in (x, y) is latent_state_batch_in_search_path[x, y], where x is current_latent_state_index, y is batch_index.
-                # The index of value prefix hidden state of the leaf node are in the same manner.
-                """
-                MCTS stage 1: Selection
-                    Each simulation starts from the internal root state s0, and finishes when the simulation reaches a leaf node s_l.
-                """
-                latent_state_index_in_search_path, latent_state_index_in_batch, last_actions, virtual_to_play = tree.batch_traverse(
-                    roots, pb_c_base, pb_c_init, discount_factor, min_max_stats_lst, results, copy.deepcopy(to_play)
-                )
-                # obtain the search horizon for leaf nodes
-                search_lens = results.search_lens
-
-                # obtain the latent state for leaf node
-                for ix, iy in zip(latent_state_index_in_search_path, latent_state_index_in_batch):
-                    latent_states.append(latent_state_batch_in_search_path[ix][iy])
-                    hidden_states_c_reward.append(reward_hidden_state_c_batch[ix][0][iy])
-                    hidden_states_h_reward.append(reward_hidden_state_h_batch[ix][0][iy])
-
-                latent_states = torch.from_numpy(np.asarray(latent_states)).to(self._cfg.device).float()
-                hidden_states_c_reward = torch.from_numpy(np.asarray(hidden_states_c_reward)).to(self._cfg.device
-                                                                                                 ).unsqueeze(0)
-                hidden_states_h_reward = torch.from_numpy(np.asarray(hidden_states_h_reward)).to(self._cfg.device
-                                                                                                 ).unsqueeze(0)
-                # .long() is only for discrete action
-                last_actions = torch.from_numpy(np.asarray(last_actions)).to(self._cfg.device).long()
-                """
-                MCTS stage 2: Expansion
-                    At the final time-step l of the simulation, the next_latent_state and reward/value_prefix are computed by the dynamics function.
-                    Then we calculate the policy_logits and value for the leaf node (next_latent_state) by the prediction function. (aka. evaluation)
-                MCTS stage 3: Backup
-                    At the end of the simulation, the statistics along the trajectory are updated.
-                """
-                network_output = model.recurrent_inference(
-                    latent_states, (hidden_states_c_reward, hidden_states_h_reward), last_actions
-                )
-
-                [
-                    network_output.latent_state, network_output.policy_logits, network_output.value,
-                    network_output.value_prefix
-                ] = to_detach_cpu_numpy(
-                    [
-                        network_output.latent_state,
-                        network_output.policy_logits,
-                        self.inverse_scalar_transform_handle(network_output.value),
-                        self.inverse_scalar_transform_handle(network_output.value_prefix),
-                    ]
-                )
-                network_output.reward_hidden_state = (
-                    network_output.reward_hidden_state[0].detach().cpu().numpy(),
-                    network_output.reward_hidden_state[1].detach().cpu().numpy()
-                )
-
-                latent_state_batch_in_search_path.append(network_output.latent_state)
-                reward_latent_state_batch = network_output.reward_hidden_state
-                # tolist() is to be compatible with cpp datatype.
-                value_batch = network_output.value.reshape(-1).tolist()
-                value_prefix_batch = network_output.value_prefix.reshape(-1).tolist()
-                policy_logits_batch = network_output.policy_logits.tolist()
-
-                # reset the hidden states in LSTM every ``lstm_horizon_len`` steps in one search.
-                # which enable the model only need to predict the value prefix in a range (e.g.: [s0,...,s5]).
-                assert self._cfg.lstm_horizon_len > 0
-                reset_idx = (np.array(search_lens) % self._cfg.lstm_horizon_len == 0)
-                reward_latent_state_batch[0][:, reset_idx, :] = 0
-                reward_latent_state_batch[1][:, reset_idx, :] = 0
-                is_reset_list = reset_idx.astype(np.int32).tolist()
-                reward_hidden_state_c_batch.append(reward_latent_state_batch[0])
-                reward_hidden_state_h_batch.append(reward_latent_state_batch[1])
-
-                # In ``batch_backpropagate()``, we first expand the leaf node using ``the policy_logits`` and
-                # ``reward`` predicted by the model, then perform backpropagation along the search path to update the
-                # statistics.
-
-                # NOTE: simulation_index + 1 is very important, which is the depth of the current leaf node.
-                current_latent_state_index = simulation_index + 1
-                tree.batch_backpropagate(
-                    current_latent_state_index, discount_factor, value_prefix_batch, value_batch, policy_logits_batch,
-                    min_max_stats_lst, results, is_reset_list, virtual_to_play
-                )
-
-
-# ==============================================================
-# MuZero
-# ==============================================================
-
-
-class MuZeroMCTSPtree(object):
-    """
-    Overview:
-        MCTSPtree for MuZero. The core ``batch_traverse`` and ``batch_backpropagate`` function is implemented in python.
-    Interfaces:
-        __init__, roots, search
-    """
-
-    # the default_config for MuZeroMCTSPtree.
-    config = dict(
-        # (float) The alpha value used in the Dirichlet distribution for exploration at the root node of the search tree.
-        root_dirichlet_alpha=0.3,
-        # (float) The noise weight at the root node of the search tree.
-        root_noise_weight=0.25,
-        # (int) The base constant used in the PUCT formula for balancing exploration and exploitation during tree search.
-        pb_c_base=19652,
-        # (float) The initialization constant used in the PUCT formula for balancing exploration and exploitation during tree search.
-        pb_c_init=1.25,
-        # (float) The maximum change in value allowed during the backup step of the search tree update.
-        value_delta_max=0.01,
-    )
-
-    @classmethod
-    def default_config(cls: type) -> EasyDict:
+        # Create a deep copy of the `config` attribute of the class.
         cfg = EasyDict(copy.deepcopy(cls.config))
+        # Add a new attribute `cfg_type` to the `cfg` object.
         cfg.cfg_type = cls.__name__ + 'Dict'
         return cfg
 
     def __init__(self, cfg: EasyDict = None) -> None:
         """
         Overview:
             Use the default configuration mechanism. If a user passes in a cfg with a key that matches an existing key
             in the default configuration, the user-provided value will override the default configuration. Otherwise,
             the default configuration will be used.
+        Arguments:
+            - cfg (:obj:`EasyDict`): The configuration passed in by the user.
         """
+        # Get the default configuration.
         default_config = self.default_config()
+        # Update the default configuration with the values provided by the user in ``cfg``.
         default_config.update(cfg)
         self._cfg = default_config
         self.inverse_scalar_transform_handle = InverseScalarTransform(
             self._cfg.model.support_scale, self._cfg.device, self._cfg.model.categorical_distribution
         )
 
     @classmethod
-    def roots(cls: int, root_num: int, legal_actions: List[Any]) -> "mz_ptree.Roots":
+    def roots(cls: int, root_num: int, legal_actions: List[Any]) -> "stochastic_mz_ptree.Roots":
         """
         Overview:
-            The initialization of CRoots with root num and legal action lists.
+            Initializes a batch of roots to search parallelly later.
         Arguments:
-            - root_num: the number of the current root.
-            - legal_action_list: the vector of the legal action of this root.
+            - root_num (:obj:`int`): the number of the roots in a batch.
+            - legal_action_list (:obj:`List[Any]`): the vector of the legal actions for the roots.
+        
+        ..note::
+            The initialization is achieved by the ``Roots`` class from the ``ptree_stochastic_mz`` module.
         """
-        import lzero.mcts.ptree.ptree_mz as ptree
-        return ptree.Roots(root_num, legal_actions)
+        return tree_stochastic_muzero.Roots(root_num, legal_actions)
 
     def search(
             self,
             roots: Any,
             model: torch.nn.Module,
             latent_state_roots: List[Any],
-            to_play: Union[int, List[Any]] = -1
+            to_play_batch: Union[int, List[Any]] = -1
     ) -> None:
         """
         Overview:
-            Do MCTS for the roots (a batch of root nodes in parallel). Parallel in model inference.
-            Use the python ctree.
+            Do MCTS for a batch of roots. Parallel in model inference. \
+            Use Python to implement the tree search.
         Arguments:
-            - roots (:obj:`Any`): a batch of expanded root nodes
-            - latent_state_roots (:obj:`list`): the hidden states of the roots
-            - to_play (:obj:`list`): the to_play list used in in self-play-mode board games
+            - roots (:obj:`Any`): a batch of expanded root nodes.
+            - latent_state_roots (:obj:`list`): the hidden states of the roots.
+            - model (:obj:`torch.nn.Module`): The model used for inference.
+            - to_play_batch (:obj:`list`): the to_play_batch list used in in self-play-mode board games.
+        
+        .. note::
+            The core functions ``batch_traverse`` and ``batch_backpropagate`` are implemented in Python.
         """
         with torch.no_grad():
             model.eval()
 
-            # preparation some constant
-            batch_size = roots.num
+            # preparation
+            num = roots.num
+            device = self._cfg.device
             pb_c_base, pb_c_init, discount_factor = self._cfg.pb_c_base, self._cfg.pb_c_init, self._cfg.discount_factor
-
-            # the data storage of latent states: storing the latent state of all the nodes in one search.
+            # the data storage of hidden states: storing the hidden states of all the ctree root nodes
+            # latent_state_roots.shape  (2, 12, 3, 3)
             latent_state_batch_in_search_path = [latent_state_roots]
 
+            # the index of each layer in the ctree
+            current_latent_state_index = 0
             # minimax value storage
-            min_max_stats_lst = MinMaxStatsList(batch_size)
+            min_max_stats_lst = MinMaxStatsList(num)
 
             for simulation_index in range(self._cfg.num_simulations):
                 # In each simulation, we expanded a new node, so in one search, we have ``num_simulations`` num of nodes at most.
 
                 latent_states = []
+
                 # prepare a result wrapper to transport results between python and c++ parts
-                results = tree_muzero.SearchResults(num=batch_size)
+                results = tree_stochastic_muzero.SearchResults(num=num)
 
                 # latent_state_index_in_search_path: The first index of the latent state corresponding to the leaf node in latent_state_batch_in_search_path, that is, the search depth.
                 # latent_state_index_in_batch: The second index of the latent state corresponding to the leaf node in latent_state_batch_in_search_path, i.e. the index in the batch, whose maximum is ``batch_size``.
                 # e.g. the latent state of the leaf node in (x, y) is latent_state_batch_in_search_path[x, y], where x is current_latent_state_index, y is batch_index.
                 """
                 MCTS stage 1: Selection
                     Each simulation starts from the internal root state s0, and finishes when the simulation reaches a leaf node s_l.
                 """
-                latent_state_index_in_search_path, latent_state_index_in_batch, last_actions, virtual_to_play = tree_muzero.batch_traverse(
-                    roots, pb_c_base, pb_c_init, discount_factor, min_max_stats_lst, results, copy.deepcopy(to_play)
-                )
+                # leaf_nodes, latent_state_index_in_search_path, latent_state_index_in_batch, last_actions, virtual_to_play_batch = tree_stochastic_muzero.batch_traverse(
+                #     roots, pb_c_base, pb_c_init, discount_factor, min_max_stats_lst, results, copy.deepcopy(to_play_batch)
+                # )
+                if self._cfg.env_type == 'not_board_games':
+                    results, virtual_to_play_batch = tree_stochastic_muzero.batch_traverse(
+                        roots, pb_c_base, pb_c_init, discount_factor, min_max_stats_lst, results, to_play_batch
+                    )
+                else:
+                    # the ``to_play_batch`` is only used in board games, here we need to deepcopy it to avoid changing the original data.
+                    results, virtual_to_play_batch = tree_stochastic_muzero.batch_traverse(
+                        roots, pb_c_base, pb_c_init, discount_factor, min_max_stats_lst, results, copy.deepcopy(to_play_batch)
+                    )
+
+                leaf_nodes, latent_state_index_in_search_path, latent_state_index_in_batch, last_actions = results.nodes, results.latent_state_index_in_search_path, results.latent_state_index_in_batch, results.last_actions
 
-                # obtain the latent state for leaf node
+                # obtain the states for leaf nodes
                 for ix, iy in zip(latent_state_index_in_search_path, latent_state_index_in_batch):
-                    latent_states.append(latent_state_batch_in_search_path[ix][iy])
-                latent_states = torch.from_numpy(np.asarray(latent_states)).to(self._cfg.device).float()
+                    latent_states.append(
+                        latent_state_batch_in_search_path[ix][
+                            iy])  # latent_state_batch_in_search_path[ix][iy] shape e.g. (64,4,4)
+
+                latent_states = torch.from_numpy(np.asarray(latent_states)).to(device)
                 # only for discrete action
-                last_actions = torch.from_numpy(np.asarray(last_actions)).to(self._cfg.device).long()
+                last_actions = torch.from_numpy(np.asarray(last_actions)).to(device).long()
                 """
                 MCTS stage 2: Expansion
-                    At the final time-step l of the simulation, the next_latent_state and reward/value_prefix are computed by the dynamics function.
-                    Then we calculate the policy_logits and value for the leaf node (next_latent_state) by the prediction function. (aka. evaluation)
+                   At the final time-step l of the simulation, the next_latent_state and reward/value_prefix are computed by the dynamics function.
+                   Then we calculate the policy_logits and value for the leaf node (next_latent_state) by the prediction function. (aka. evaluation)
                 MCTS stage 3: Backup
-                    At the end of the simulation, the statistics along the trajectory are updated.
+                   At the end of the simulation, the statistics along the trajectory are updated.
                 """
-                network_output = model.recurrent_inference(latent_states, last_actions)
+                
+                # network_output = model.recurrent_inference(latent_states, last_actions)
+                num = len(leaf_nodes)
+                latent_state_batch = [None] * num
+                value_batch = [None] * num
+                reward_batch = [None] * num
+                policy_logits_batch = [None] * num
+                child_is_chance_batch = [None] * num
+                chance_nodes = []
+                decision_nodes = []
+                for i, node in enumerate(leaf_nodes):
+                    if node.is_chance:
+                        chance_nodes.append(i)
+                    else:
+                        decision_nodes.append(i)
+
+                def process_nodes(node_indices, is_chance):
+                    # Return early if node_indices is empty
+                    if not node_indices:
+                        return
+                    # Slice and stack latent_states and last_actions based on node_indices
+                    latent_states_stack = torch.stack([latent_states[i] for i in node_indices], dim=0)
+                    last_actions_stack = torch.stack([last_actions[i] for i in node_indices], dim=0)
+
+                    # Pass the stacked batch through the recurrent_inference function
+                    network_output_batch = model.recurrent_inference(latent_states_stack,
+                                                                     last_actions_stack,
+                                                                     afterstate=not is_chance)
+
+                    # Split the batch output into separate nodes
+                    latent_state_splits = torch.split(network_output_batch.latent_state, 1, dim=0)
+                    value_splits = torch.split(network_output_batch.value, 1, dim=0)
+                    reward_splits = torch.split(network_output_batch.reward, 1, dim=0)
+                    policy_logits_splits = torch.split(network_output_batch.policy_logits, 1, dim=0)
+
+                    for i, (latent_state, value, reward, policy_logits) in zip(node_indices,
+                                                                               zip(latent_state_splits, value_splits,
+                                                                                   reward_splits,
+                                                                                   policy_logits_splits)):
+                        if not model.training:
+                            value = self.inverse_scalar_transform_handle(value).detach().cpu().numpy()
+                            reward = self.inverse_scalar_transform_handle(reward).detach().cpu().numpy()
+                            latent_state = latent_state.detach().cpu().numpy()
+                            policy_logits = policy_logits.detach().cpu().numpy()
+
+                        latent_state_batch[i] = latent_state
+                        value_batch[i] = value.reshape(-1).tolist()
+                        reward_batch[i] = reward.reshape(-1).tolist()
+                        policy_logits_batch[i] = policy_logits.tolist()
+                        child_is_chance_batch[i] = is_chance
+
+                process_nodes(chance_nodes, True)
+                process_nodes(decision_nodes, False)
+
+                value_batch_chance = [value_batch[leaf_idx] for leaf_idx in chance_nodes]
+                value_batch_decision = [value_batch[leaf_idx] for leaf_idx in decision_nodes]
+                reward_batch_chance = [reward_batch[leaf_idx] for leaf_idx in chance_nodes]
+                reward_batch_decision = [reward_batch[leaf_idx] for leaf_idx in decision_nodes]
+                policy_logits_batch_chance = [policy_logits_batch[leaf_idx] for leaf_idx in chance_nodes]
+                policy_logits_batch_decision = [policy_logits_batch[leaf_idx] for leaf_idx in decision_nodes]
 
-                if not model.training:
-                    # if not in training, obtain the scalars of the value/reward
-                    [
-                        network_output.latent_state, network_output.policy_logits, network_output.value,
-                        network_output.reward
-                    ] = to_detach_cpu_numpy(
-                        [
-                            network_output.latent_state,
-                            network_output.policy_logits,
-                            self.inverse_scalar_transform_handle(network_output.value),
-                            self.inverse_scalar_transform_handle(network_output.reward),
-                        ]
-                    )
-
-                latent_state_batch_in_search_path.append(network_output.latent_state)
-                # tolist() is to be compatible with cpp datatype.
-                value_batch = network_output.value.reshape(-1).tolist()
-                reward_batch = network_output.reward.reshape(-1).tolist()
-                policy_logits_batch = network_output.policy_logits.tolist()
-
-                # In ``batch_backpropagate()``, we first expand the leaf node using ``the policy_logits`` and
-                # ``reward`` predicted by the model, then perform backpropagation along the search path to update the
-                # statistics.
-
-                # NOTE: simulation_index + 1 is very important, which is the depth of the current leaf node.
+                latent_state_batch = np.concatenate(latent_state_batch, axis=0)
+                latent_state_batch_in_search_path.append(latent_state_batch)
                 current_latent_state_index = simulation_index + 1
-                tree_muzero.batch_backpropagate(
-                    current_latent_state_index, discount_factor, reward_batch, value_batch, policy_logits_batch,
-                    min_max_stats_lst, results, virtual_to_play
-                )
+
+                if len(chance_nodes) > 0:
+                    value_batch_chance = np.concatenate(value_batch_chance, axis=0)
+                    reward_batch_chance = np.concatenate(reward_batch_chance, axis=0)
+                    policy_logits_batch_chance = np.concatenate(policy_logits_batch_chance, axis=0)
+                    tree_stochastic_muzero.batch_backpropagate(
+                        current_latent_state_index, discount_factor, reward_batch_chance, value_batch_chance,
+                        policy_logits_batch_chance,
+                        min_max_stats_lst, results, virtual_to_play_batch, child_is_chance_batch, chance_nodes
+                    )
+                if len(decision_nodes) > 0:
+                    value_batch_decision = np.concatenate(value_batch_decision, axis=0)
+                    reward_batch_decision = np.concatenate(reward_batch_decision, axis=0)
+                    policy_logits_batch_decision = np.concatenate(policy_logits_batch_decision, axis=0)
+                    tree_stochastic_muzero.batch_backpropagate(
+                        current_latent_state_index, discount_factor, reward_batch_decision, value_batch_decision,
+                        policy_logits_batch_decision,
+                        min_max_stats_lst, results, virtual_to_play_batch, child_is_chance_batch, decision_nodes
+                    )
```

### Comparing `LightZero-0.0.2/lzero/mcts/utils.py` & `LightZero-0.0.5/lzero/mcts/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -76,60 +76,50 @@
                 }
             )
     return extend_data
 
 
 def prepare_observation(observation_list, model_type='conv'):
     """
-    Overview:
-        Prepare the observations to satisfy the input format of model.
-        if model_type='conv':
-            [B, S, W, H, C] -> [B, S x C, W, H]
-            where B is batch size, S is stack num, W is width, H is height, and C is the number of channels
-        if model_type='mlp':
-            [B, S, O] -> [B, S x O]
-            where B is batch size, S is stack num, O is obs shape.
+    Prepare the observations to satisfy the input format of the model.
+
+    For model_type='conv':
+        [B, S, C, W, H] -> [B, S x C, W, H]
+        where B is batch size, S is stack num, W is width, H is height, and C is the number of channels.
+
+    For model_type='mlp':
+        [B, S, O] -> [B, S x O]
+        where B is batch size, S is stack num, O is obs shape.
+
     Arguments:
-        - observation_list (:obj:`List`): list of observations.
-        - model_type (:obj:`str`): type of the model. (default is 'conv')
+        - observation_list (List): list of observations.
+        - model_type (str): type of the model. (default is 'conv')
+
+    Returns:
+        - np.ndarray: Reshaped array of observations.
     """
-    assert model_type in ['conv', 'mlp']
+    assert model_type in ['conv', 'mlp'], "model_type must be either 'conv' or 'mlp'"
     observation_array = np.array(observation_list)
+    batch_size = observation_array.shape[0]
 
     if model_type == 'conv':
-        # for 3-dimensional image obs
-        if len(observation_array.shape) == 3:
-            # for vector obs input, e.g. classical control and box2d environments
-            # to be compatible with LightZero model/policy,
-            # observation_array: [B, S, O], where O is original obs shape
-            # [B, S, O] -> [B, S, O, 1]
-            observation_array = observation_array.reshape(
-                observation_array.shape[0], observation_array.shape[1], observation_array.shape[2], 1
-            )
-
-        elif len(observation_array.shape) == 5:
-            # image obs input, e.g. atari environments
-            # observation_array: [B, S, W, H, C]
-
-            # 1, 4, 8, 1, 1 -> 1, 4, 1, 8, 1
-            #   [B, S, W, H, C] -> [B, S, C, W, H]
-            observation_array = np.transpose(observation_array, (0, 1, 4, 2, 3))
-
-            shape = observation_array.shape
-            # 1, 4, 1, 8, 1 -> 1, 4*1, 8, 1
-            #  [B, S, C, W, H] -> [B, S*C, W, H]
-            observation_array = observation_array.reshape((shape[0], -1, shape[-2], shape[-1]))
+        if observation_array.ndim == 3:
+            # Add a channel dimension if it's missing
+            observation_array = observation_array[..., np.newaxis]
+        elif observation_array.ndim == 5:
+            # Reshape to [B, S*C, W, H]
+            _, stack_num, channels, width, height = observation_array.shape
+            observation_array = observation_array.reshape(batch_size, stack_num * channels, width, height)
 
     elif model_type == 'mlp':
-        # for 1-dimensional vector obs
-        # observation_array: [B, S, O], where O is original obs shape
-        # [B, S, O] -> [B, S*O]
-        # print(observation_array.shape)
-        observation_array = observation_array.reshape(observation_array.shape[0], -1)
-        # print(observation_array.shape)
+        if observation_array.ndim == 3:
+            # Flatten the last two dimensions
+            observation_array = observation_array.reshape(batch_size, -1)
+        else:
+            raise ValueError("For 'mlp' model_type, the observation must have 3 dimensions [B, S, O]")
 
     return observation_array
 
 
 def obtain_tree_topology(root, to_play=-1):
     node_stack = []
     edge_topology_list = []
```

### Comparing `LightZero-0.0.2/lzero/model/alphazero_model.py` & `LightZero-0.0.5/lzero/model/alphazero_model.py`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/lzero/model/common.py` & `LightZero-0.0.5/lzero/model/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,22 +76,14 @@
                     activation=activation,
                     norm_type='BN',
                     res_type='basic',
                     bias=False
                 ) for _ in range(1)
             ]
         )
-        self.conv2 = nn.Conv2d(
-            out_channels // 2,
-            out_channels,
-            kernel_size=3,
-            stride=2,
-            padding=1,
-            bias=False,
-        )
         self.downsample_block = ResBlock(
             in_channels=out_channels // 2,
             out_channels=out_channels,
             activation=activation,
             norm_type='BN',
             res_type='downsample',
             bias=False
```

### Comparing `LightZero-0.0.2/lzero/model/efficientzero_model.py` & `LightZero-0.0.5/lzero/model/efficientzero_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -492,25 +492,14 @@
                     activation=self.activation,
                     norm_type='BN',
                     res_type='basic',
                     bias=False
                 ) for _ in range(num_res_blocks)
             ]
         )
-        self.reward_resblocks = nn.ModuleList(
-            [
-                ResBlock(
-                    in_channels=num_channels - self.action_encoding_dim,
-                    activation=self.activation,
-                    norm_type='BN',
-                    res_type='basic',
-                    bias=False
-                ) for _ in range(num_res_blocks)
-            ]
-        )
 
         self.conv1x1_reward = nn.Conv2d(num_channels - self.action_encoding_dim, reward_head_channels, 1)
         
         if norm_type == 'BN':
             self.norm_reward = nn.BatchNorm2d(reward_head_channels)
         elif norm_type == 'LN':
             if downsample:
```

### Comparing `LightZero-0.0.2/lzero/model/efficientzero_model_mlp.py` & `LightZero-0.0.5/lzero/model/efficientzero_model_mlp.py`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/lzero/model/image_transform.py` & `LightZero-0.0.5/lzero/model/image_transform.py`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/lzero/model/muzero_model.py` & `LightZero-0.0.5/lzero/model/muzero_model.py`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/lzero/model/muzero_model_mlp.py` & `LightZero-0.0.5/lzero/model/muzero_model_mlp.py`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/lzero/model/sampled_efficientzero_model.py` & `LightZero-0.0.5/lzero/model/sampled_efficientzero_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,14 +178,15 @@
             num_res_blocks,
             num_channels + self.action_encoding_dim,
             reward_head_channels,
             fc_reward_layers,
             self.reward_support_size,
             flatten_output_size_for_reward_head,
             downsample,
+            lstm_hidden_size=self.lstm_hidden_size,
             last_linear_layer_init_zero=self.last_linear_layer_init_zero,
             activation=activation,
             norm_type=norm_type
         )
 
         self.prediction_network = PredictionNetwork(
             observation_shape,
@@ -392,30 +393,34 @@
                 # The final action_encoding shape is (batch_size, 1, latent_state[2], latent_state[3]), e.g. (8, 1, 4, 1).
                 if len(action.shape) == 2:
                     # (batch_size, action_dim=1) -> (batch_size, 1, 1, 1)
                     # e.g.,  torch.Size([8, 1]) ->  torch.Size([8, 1, 1, 1])
                     action = action.unsqueeze(-1).unsqueeze(-1)
                 elif len(action.shape) == 1:
                     # (batch_size,) -> (batch_size, 1, 1, 1)
-                    # e.g.,  -> torch.Size([8, 1, 1, 1])
+                    # e.g., torch.Size([8])  -> torch.Size([8, 1, 1, 1])
                     action = action.unsqueeze(-1).unsqueeze(-1).unsqueeze(-1)
 
                 action_encoding = action.expand(
                     latent_state.shape[0], 1, latent_state.shape[2], latent_state.shape[3]
                 ) / self.action_space_size
         else:
             # continuous action space
-            if len(action.shape) == 2:
-                # (batch_size, action_dim) -> (batch_size, action_dim, 1, 1)
-                # e.g.,  torch.Size([8, 2]) ->  torch.Size([8, 2, 1, 1])
-                action = action.unsqueeze(-1).unsqueeze(-1)
-            elif len(action.shape) == 1:
+            if len(action.shape) == 1:
                 # (batch_size,) -> (batch_size, action_dim=1, 1, 1)
-                # e.g.,  -> torch.Size([8, 2, 1, 1])
+                # e.g., torch.Size([8]) -> torch.Size([8, 1, 1, 1])
                 action = action.unsqueeze(-1).unsqueeze(-1).unsqueeze(-1)
+            elif len(action.shape) == 2:
+                # (batch_size, action_dim) -> (batch_size, action_dim, 1, 1)
+                # e.g., torch.Size([8, 2]) ->  torch.Size([8, 2, 1, 1])
+                action = action.unsqueeze(-1).unsqueeze(-1)
+            elif len(action.shape) == 3:
+                # (batch_size, action_dim, 1) -> (batch_size, action_dim)
+                # e.g., torch.Size([8, 2, 1]) ->  torch.Size([8, 2, 1, 1])
+                action = action.unsqueeze(-1)
 
             action_encoding_tmp = action
             action_encoding = action_encoding_tmp.expand(
                 latent_state.shape[0], self.action_space_size, latent_state.shape[2], latent_state.shape[3]
             )
 
         action_encoding = action_encoding.to(latent_state.device).float()
```

### Comparing `LightZero-0.0.2/lzero/model/sampled_efficientzero_model_mlp.py` & `LightZero-0.0.5/lzero/model/sampled_efficientzero_model_mlp.py`

 * *Files 1% similar despite different names*

```diff
@@ -321,25 +321,25 @@
                 action = action.long()
                 action_one_hot.scatter_(1, action, 1)
                 action_encoding = action_one_hot
             elif self.discrete_action_encoding_type == 'not_one_hot':
                 action_encoding = action / self.action_space_size
                 if len(action_encoding.shape) == 1:
                     # (batch_size, ) -> (batch_size, 1)
-                    # e.g.,  torch.Size([8]) ->  torch.Size([8, 1])
+                    # e.g., torch.Size([8]) ->  torch.Size([8, 1])
                     action_encoding = action_encoding.unsqueeze(-1)
         else:
             # continuous action space
             if len(action.shape) == 1:
                 # (batch_size, ) -> (batch_size, 1)
-                # e.g.,  torch.Size([8]) ->  torch.Size([8, 1])
+                # e.g., torch.Size([8]) ->  torch.Size([8, 1])
                 action = action.unsqueeze(-1)
             elif len(action.shape) == 3:
                 # (batch_size, action_dim, 1) -> (batch_size,  action_dim)
-                # e.g.,  torch.Size([8, 2, 1]) ->  torch.Size([8, 2])
+                # e.g., torch.Size([8, 2, 1]) ->  torch.Size([8, 2])
                 action = action.squeeze(-1)
 
             action_encoding = action
 
         action_encoding = action_encoding.to(latent_state.device).float()
         # state_action_encoding shape: (batch_size, latent_state[1] + action_dim]) or
         # (batch_size, latent_state[1] + action_space_size]) depending on the discrete_action_encoding_type.
```

### Comparing `LightZero-0.0.2/lzero/model/stochastic_muzero_model.py` & `LightZero-0.0.5/lzero/model/stochastic_muzero_model.py`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/lzero/model/stochastic_muzero_model_mlp.py` & `LightZero-0.0.5/lzero/model/stochastic_muzero_model_mlp.py`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/lzero/model/tests/test_alphazero_model.py` & `LightZero-0.0.5/lzero/model/tests/test_alphazero_model.py`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/lzero/model/tests/test_common.py` & `LightZero-0.0.5/lzero/model/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/lzero/model/tests/test_efficientzero_model.py` & `LightZero-0.0.5/lzero/model/tests/test_efficientzero_model.py`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/lzero/model/tests/test_muzero_model.py` & `LightZero-0.0.5/lzero/model/tests/test_muzero_model.py`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/lzero/model/tests/test_sampled_efficientzero_model.py` & `LightZero-0.0.5/lzero/model/tests/test_sampled_efficientzero_model.py`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/lzero/model/tests/test_stochastic_muzero_model.py` & `LightZero-0.0.5/lzero/model/tests/test_stochastic_muzero_model.py`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/lzero/model/utils.py` & `LightZero-0.0.5/lzero/model/utils.py`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/lzero/policy/alphazero.py` & `LightZero-0.0.5/lzero/policy/alphazero.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,14 +32,19 @@
             # (tuple) The stacked obs shape.
             observation_shape=(3, 6, 6),
             # (int) The number of res blocks in AlphaZero model.
             num_res_blocks=1,
             # (int) The number of channels of hidden states in AlphaZero model.
             num_channels=32,
         ),
+        # (bool) Whether to enable the sampled-based algorithm (e.g. Sampled EfficientZero)
+        # this variable is used in ``collector``.
+        sampled_algo=False,
+        # (bool) Whether to enable the gumbel-based algorithm (e.g. Gumbel Muzero)
+        gumbel_algo=False,
         # (bool) Whether to use multi-gpu training.
         multi_gpu=False,
         # (bool) Whether to use cuda for network.
         cuda=False,
         # (int) How many updates(iterations) to train after collector's one collection.
         # Bigger "update_per_collect" means bigger off-policy.
         # collect data -> update policy-> collect data -> ...
@@ -159,24 +164,24 @@
         reward = inputs['reward']
 
         state_batch = state_batch.to(device=self._device, dtype=torch.float)
         mcts_probs = mcts_probs.to(device=self._device, dtype=torch.float)
         reward = reward.to(device=self._device, dtype=torch.float)
 
         action_probs, values = self._learn_model.compute_policy_value(state_batch)
-        log_probs = torch.log(action_probs)
+        policy_log_probs = torch.log(action_probs)
 
         # calculate policy entropy, for monitoring only
-        entropy = torch.mean(-torch.sum(action_probs * log_probs, 1))
+        entropy = torch.mean(-torch.sum(action_probs * policy_log_probs, 1))
         entropy_loss = -entropy
 
         # ============
         # policy loss
         # ============
-        policy_loss = -torch.mean(torch.sum(mcts_probs * log_probs, 1))
+        policy_loss = -torch.mean(torch.sum(mcts_probs * policy_log_probs, 1))
 
         # ============
         # value loss
         # ============
         value_loss = F.mse_loss(values.view(-1), reward)
 
         total_loss = self._value_weight * value_loss + policy_loss + self._entropy_weight * entropy_loss
@@ -199,27 +204,27 @@
         return {
             'cur_lr': self._optimizer.param_groups[0]['lr'],
             'total_loss': total_loss.item(),
             'policy_loss': policy_loss.item(),
             'value_loss': value_loss.item(),
             'entropy_loss': entropy_loss.item(),
             'total_grad_norm_before_clip': total_grad_norm_before_clip.item(),
-            'collect_mcts_temperature': self._collect_mcts_temperature,
+            'collect_mcts_temperature': self.collect_mcts_temperature,
         }
 
     def _init_collect(self) -> None:
         """
         Overview:
             Collect mode init method. Called by ``self.__init__``. Initialize the collect model and MCTS utils.
         """
         self._get_simulation_env()
         self._collect_model = self._model
         if self._cfg.mcts_ctree:
             import sys
-            sys.path.append('./LightZero/lzero/mcts/ctree/ctree_alphazero/build')
+            sys.path.append('/Users/your_user_name/code/LightZero/lzero/mcts/ctree/ctree_alphazero/build')
             import mcts_alphazero
             self._collect_mcts = mcts_alphazero.MCTS(self._cfg.mcts.max_moves, self._cfg.mcts.num_simulations,
                                                      self._cfg.mcts.pb_c_base,
                                                      self._cfg.mcts.pb_c_init, self._cfg.mcts.root_dirichlet_alpha,
                                                      self._cfg.mcts.root_noise_weight, self.simulate_env)
         else:
             if self._cfg.sampled_algo:
@@ -239,44 +244,46 @@
             - obs (:obj:`Dict`): The dict of obs, the key is env_id and the value is the \
                 corresponding obs in this timestep.
             - temperature (:obj:`float`): The temperature for MCTS search.
         Returns:
             - output (:obj:`Dict[str, torch.Tensor]`): The dict of output, the key is env_id and the value is the \
                 the corresponding policy output in this timestep, including action, probs and so on.
         """
-        self._collect_mcts_temperature = temperature
+        self.collect_mcts_temperature = temperature
         ready_env_id = list(obs.keys())
         init_state = {env_id: obs[env_id]['board'] for env_id in ready_env_id}
+        # If 'katago_game_state' is in the observation of the given environment ID, it's value is used.
+        # If it's not present (which will raise a KeyError), None is used instead.
+        # This approach is taken to maintain compatibility with the handling of 'katago' related parts of 'alphazero_mcts_ctree' in Go.
+        katago_game_state = {env_id: obs[env_id].get('katago_game_state', None) for env_id in ready_env_id}
         start_player_index = {env_id: obs[env_id]['current_player_index'] for env_id in ready_env_id}
         output = {}
         self._policy_model = self._collect_model
         for env_id in ready_env_id:
             state_config_for_simulation_env_reset = EasyDict(dict(start_player_index=start_player_index[env_id],
-                                                                  init_state=init_state[env_id], ))
-            action, mcts_probs = self._collect_mcts.get_next_action(
-                state_config_for_simulation_env_reset,
-                policy_forward_fn=self._policy_value_fn,
-                temperature=self._collect_mcts_temperature,
-                sample=True
-            )
+                                                                  init_state=init_state[env_id],
+                                                                  katago_policy_init=False,
+                                                                  katago_game_state=katago_game_state[env_id]))
+            action, mcts_probs = self._collect_mcts.get_next_action(state_config_for_simulation_env_reset, self._policy_value_fn, self.collect_mcts_temperature, True)
+
             output[env_id] = {
                 'action': action,
                 'probs': mcts_probs,
             }
         return output
 
     def _init_eval(self) -> None:
         """
         Overview:
             Evaluate mode init method. Called by ``self.__init__``. Initialize the eval model and MCTS utils.
         """
         self._get_simulation_env()
         if self._cfg.mcts_ctree:
             import sys
-            sys.path.append('./LightZero/lzero/mcts/ctree/ctree_alphazero/build')
+            sys.path.append('/Users/your_user_name/code/LightZero/lzero/mcts/ctree/ctree_alphazero/build')
             import mcts_alphazero
             # TODO(pu): how to set proper num_simulations for evaluation
             self._eval_mcts = mcts_alphazero.MCTS(self._cfg.mcts.max_moves,
                                                   min(800, self._cfg.mcts.num_simulations * 4),
                                                   self._cfg.mcts.pb_c_base,
                                                   self._cfg.mcts.pb_c_init, self._cfg.mcts.root_dirichlet_alpha,
                                                   self._cfg.mcts.root_noise_weight, self.simulate_env)
@@ -301,52 +308,66 @@
                 corresponding obs in this timestep.
         Returns:
             - output (:obj:`Dict[str, torch.Tensor]`): The dict of output, the key is env_id and the value is the \
                 the corresponding policy output in this timestep, including action, probs and so on.
         """
         ready_env_id = list(obs.keys())
         init_state = {env_id: obs[env_id]['board'] for env_id in ready_env_id}
+        # If 'katago_game_state' is in the observation of the given environment ID, it's value is used.
+        # If it's not present (which will raise a KeyError), None is used instead.
+        # This approach is taken to maintain compatibility with the handling of 'katago' related parts of 'alphazero_mcts_ctree' in Go.
+        katago_game_state = {env_id: obs[env_id].get('katago_game_state', None) for env_id in ready_env_id}
         start_player_index = {env_id: obs[env_id]['current_player_index'] for env_id in ready_env_id}
         output = {}
         self._policy_model = self._eval_model
         for env_id in ready_env_id:
             state_config_for_simulation_env_reset = EasyDict(dict(start_player_index=start_player_index[env_id],
-                                                                  init_state=init_state[env_id], ))
+                                                                  init_state=init_state[env_id],
+                                                                  katago_policy_init=False,
+                                                                  katago_game_state=katago_game_state[env_id]))
             action, mcts_probs = self._eval_mcts.get_next_action(
-                state_config_for_simulation_env_reset, policy_forward_fn=self._policy_value_fn, temperature=1.0,
-                sample=False
+                state_config_for_simulation_env_reset, self._policy_value_fn, 1.0, False
             )
             output[env_id] = {
                 'action': action,
                 'probs': mcts_probs,
             }
         return output
 
     def _get_simulation_env(self):
-        if self._cfg.simulation_env_name == 'tictactoe':
+        if self._cfg.simulation_env_id == 'tictactoe':
             from zoo.board_games.tictactoe.envs.tictactoe_env import TicTacToeEnv
             if self._cfg.simulation_env_config_type == 'play_with_bot':
                 from zoo.board_games.tictactoe.config.tictactoe_alphazero_bot_mode_config import \
                     tictactoe_alphazero_config
             elif self._cfg.simulation_env_config_type == 'self_play':
                 from zoo.board_games.tictactoe.config.tictactoe_alphazero_sp_mode_config import \
                     tictactoe_alphazero_config
             else:
                 raise NotImplementedError
             self.simulate_env = TicTacToeEnv(tictactoe_alphazero_config.env)
 
-        elif self._cfg.simulation_env_name == 'gomoku':
+        elif self._cfg.simulation_env_id == 'gomoku':
             from zoo.board_games.gomoku.envs.gomoku_env import GomokuEnv
             if self._cfg.simulation_env_config_type == 'play_with_bot':
                 from zoo.board_games.gomoku.config.gomoku_alphazero_bot_mode_config import gomoku_alphazero_config
             elif self._cfg.simulation_env_config_type == 'self_play':
                 from zoo.board_games.gomoku.config.gomoku_alphazero_sp_mode_config import gomoku_alphazero_config
             else:
                 raise NotImplementedError
             self.simulate_env = GomokuEnv(gomoku_alphazero_config.env)
+        elif self._cfg.simulation_env_id == 'connect4':
+            from zoo.board_games.connect4.envs.connect4_env import Connect4Env
+            if self._cfg.simulation_env_config_type == 'play_with_bot':
+                from zoo.board_games.connect4.config.connect4_alphazero_bot_mode_config import connect4_alphazero_config
+            elif self._cfg.simulation_env_config_type == 'self_play':
+                from zoo.board_games.connect4.config.connect4_alphazero_sp_mode_config import connect4_alphazero_config
+            else:
+                raise NotImplementedError
+            self.simulate_env = Connect4Env(connect4_alphazero_config.env)
         else:
             raise NotImplementedError
 
     @torch.no_grad()
     def _policy_value_fn(self, env: 'Env') -> Tuple[Dict[int, np.ndarray], float]:  # noqa
         legal_actions = env.legal_actions
         current_state, current_state_scale = env.current_state()
```

### Comparing `LightZero-0.0.2/lzero/policy/efficientzero.py` & `LightZero-0.0.5/lzero/policy/efficientzero.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,20 +73,27 @@
         cuda=True,
         # (int) The number of environments used in collecting data.
         collector_env_num=8,
         # (int) The number of environments used in evaluating policy.
         evaluator_env_num=3,
         # (str) The type of environment. The options are ['not_board_games', 'board_games'].
         env_type='not_board_games',
+        # (str) The type of action space. Options are ['fixed_action_space', 'varied_action_space'].
+        action_type='fixed_action_space',
         # (str) The type of battle mode. The options are ['play_with_bot_mode', 'self_play_mode'].
         battle_mode='play_with_bot_mode',
         # (bool) Whether to monitor extra statistics in tensorboard.
         monitor_extra_statistics=True,
         # (int) The transition number of one ``GameSegment``.
         game_segment_length=200,
+        # (bool): Indicates whether to perform an offline evaluation of the checkpoint (ckpt).
+        # If set to True, the checkpoint will be evaluated after the training process is complete.
+        # IMPORTANT: Setting eval_offline to True requires configuring the saving of checkpoints to align with the evaluation frequency.
+        # This is done by setting the parameter learn.learner.hook.save_ckpt_after_iter to the same value as eval_freq in the train_muzero.py automatically.
+        eval_offline=False,
 
         # ****** observation ******
         # (bool) Whether to transform image to string to save memory.
         transform2string=False,
         # (bool) Whether to use gray scale image.
         gray_scale=False,
         # (bool) Whether to use data augmentation.
@@ -153,14 +160,16 @@
         # i.e. temperature: 1 -> 0.5 -> 0.25
         manual_temperature_decay=False,
         # (float) The fixed temperature value for MCTS action selection, which is used to control the exploration.
         # The larger the value, the more exploration. This value is only used when manual_temperature_decay=False.
         fixed_temperature_value=0.25,
         # (bool) Whether to use the true chance in MCTS in some environments with stochastic dynamics, such as 2048.
         use_ture_chance_label_in_chance_encoder=False,
+        # (bool) Whether to add noise to roots during reanalyze process.
+        reanalyze_noise=False,
 
         # ****** Priority ******
         # (bool) Whether to use priority when sampling training data from the buffer.
         use_priority=True,
         # (float) The degree of prioritization to use. A value of 0 means no prioritization,
         # while a value of 1 means full prioritization.
         priority_prob_alpha=0.6,
@@ -330,26 +339,23 @@
         # transform the scaled value or its categorical representation to its original value,
         # i.e. h^(-1)(.) function in paper https://arxiv.org/pdf/1805.11593.pdf.
         original_value = self.inverse_scalar_transform_handle(value)
 
         # Note: The following lines are just for debugging.
         predicted_value_prefixs = []
         if self._cfg.monitor_extra_statistics:
-            latent_state_list = latent_state.detach().cpu().numpy()
             predicted_values, predicted_policies = original_value.detach().cpu(), torch.softmax(
                 policy_logits, dim=1
             ).detach().cpu()
 
         # calculate the new priorities for each transition.
-        value_priority = L1Loss(reduction='none')(original_value.squeeze(-1), target_value[:, 0])
-        value_priority = value_priority.data.cpu().numpy() + 1e-6
+        value_priority = L1Loss(reduction='none')(original_value.squeeze(-1), target_value[:, 0]) + 1e-6
 
         prob = torch.softmax(policy_logits, dim=-1)
-        dist = Categorical(prob)
-        policy_entropy = dist.entropy().mean()
+        policy_entropy = -(prob * prob.log()).sum(-1).mean()
 
         # ==============================================================
         # calculate policy and value loss for the first step.
         # ==============================================================
         policy_loss = cross_entropy_loss(policy_logits, target_policy[:, 0])
 
         # Here we take the init hypothetical step k=0.
@@ -358,19 +364,18 @@
         # ******* NOTE: target_policy_entropy is only for debug.  ******
         non_masked_indices = torch.nonzero(mask_batch[:, 0]).squeeze(-1)
         # Check if there are any unmasked rows
         if len(non_masked_indices) > 0:
             target_normalized_visit_count_masked = torch.index_select(
                 target_normalized_visit_count_init_step, 0, non_masked_indices
             )
-            target_dist = Categorical(target_normalized_visit_count_masked)
-            target_policy_entropy = target_dist.entropy().mean()
+            target_policy_entropy = -((target_normalized_visit_count_masked+1e-6) * (target_normalized_visit_count_masked+1e-6).log()).sum(-1).mean()
         else:
-            # Set target_policy_entropy to 0 if all rows are masked
-            target_policy_entropy = 0
+            # Set target_policy_entropy to log(|A|) if all rows are masked
+            target_policy_entropy = torch.log(torch.tensor(target_normalized_visit_count_init_step.shape[-1]))
 
         value_loss = cross_entropy_loss(value, target_value_categorical[:, 0])
 
         value_prefix_loss = torch.zeros(self._cfg.batch_size, device=self._cfg.device)
         consistency_loss = torch.zeros(self._cfg.batch_size, device=self._cfg.device)
 
         # ==============================================================
@@ -415,51 +420,48 @@
             # calculate policy loss for the next ``num_unroll_steps`` unroll steps.
             # NOTE: the +=.
             # ==============================================================
             policy_loss += cross_entropy_loss(policy_logits, target_policy[:, step_k + 1])
 
             # Here we take the hypothetical step k = step_k + 1
             prob = torch.softmax(policy_logits, dim=-1)
-            dist = Categorical(prob)
-            policy_entropy += dist.entropy().mean()
+            policy_entropy += -(prob * prob.log()).sum(-1).mean()
+
             target_normalized_visit_count = target_policy[:, step_k + 1]
 
             # ******* NOTE: target_policy_entropy is only for debug.  ******
             non_masked_indices = torch.nonzero(mask_batch[:, step_k + 1]).squeeze(-1)
             # Check if there are any unmasked rows
             if len(non_masked_indices) > 0:
                 target_normalized_visit_count_masked = torch.index_select(
                     target_normalized_visit_count, 0, non_masked_indices
                 )
-                target_dist = Categorical(target_normalized_visit_count_masked)
-                target_policy_entropy += target_dist.entropy().mean()
+                target_policy_entropy += -((target_normalized_visit_count_masked+1e-6) * (target_normalized_visit_count_masked+1e-6).log()).sum(-1).mean()
             else:
-                # Set target_policy_entropy to 0 if all rows are masked
-                target_policy_entropy += 0
+                # Set target_policy_entropy to log(|A|) if all rows are masked
+                target_policy_entropy += torch.log(torch.tensor(target_normalized_visit_count.shape[-1]))
 
             value_loss += cross_entropy_loss(value, target_value_categorical[:, step_k + 1])
             value_prefix_loss += cross_entropy_loss(value_prefix, target_value_prefix_categorical[:, step_k])
 
             # reset hidden states every ``lstm_horizon_len`` unroll steps.
             if (step_k + 1) % self._cfg.lstm_horizon_len == 0:
                 reward_hidden_state = (
                     torch.zeros(1, self._cfg.batch_size, self._cfg.model.lstm_hidden_size).to(self._cfg.device),
                     torch.zeros(1, self._cfg.batch_size, self._cfg.model.lstm_hidden_size).to(self._cfg.device)
                 )
 
             if self._cfg.monitor_extra_statistics:
                 original_value_prefixs = self.inverse_scalar_transform_handle(value_prefix)
                 original_value_prefixs_cpu = original_value_prefixs.detach().cpu()
-
                 predicted_values = torch.cat(
                     (predicted_values, self.inverse_scalar_transform_handle(value).detach().cpu())
                 )
                 predicted_value_prefixs.append(original_value_prefixs_cpu)
                 predicted_policies = torch.cat((predicted_policies, torch.softmax(policy_logits, dim=1).detach().cpu()))
-                latent_state_list = np.concatenate((latent_state_list, latent_state.detach().cpu().numpy()))
 
         # ==============================================================
         # the core learn model update step.
         # ==============================================================
         # weighted loss with masks (some invalid states which are out of trajectory.)
         loss = (
             self._cfg.ssl_loss_weight * consistency_loss + self._cfg.policy_loss_weight * policy_loss +
@@ -497,27 +499,26 @@
             'total_loss': loss.mean().item(),
             'policy_loss': policy_loss.mean().item(),
             'policy_entropy': policy_entropy.item() / (self._cfg.num_unroll_steps + 1),
             'target_policy_entropy': target_policy_entropy.item() / (self._cfg.num_unroll_steps + 1),
             'value_prefix_loss': value_prefix_loss.mean().item(),
             'value_loss': value_loss.mean().item(),
             'consistency_loss': consistency_loss.mean().item() / self._cfg.num_unroll_steps,
-
+            'target_value_prefix': target_value_prefix.mean().item(),
+            'target_value': target_value.mean().item(),
+            'transformed_target_value_prefix': transformed_target_value_prefix.mean().item(),
+            'transformed_target_value': transformed_target_value.mean().item(),
+            'predicted_value_prefixs': predicted_value_prefixs.mean().item(),
+            'predicted_values': predicted_values.mean().item(),
+            'total_grad_norm_before_clip': total_grad_norm_before_clip.item(),
             # ==============================================================
             # priority related
             # ==============================================================
             'value_priority': value_priority.mean().item(),
-            'value_priority_orig': value_priority,
-            'target_value_prefix': target_value_prefix.detach().cpu().numpy().mean().item(),
-            'target_value': target_value.detach().cpu().numpy().mean().item(),
-            'transformed_target_value_prefix': transformed_target_value_prefix.detach().cpu().numpy().mean().item(),
-            'transformed_target_value': transformed_target_value.detach().cpu().numpy().mean().item(),
-            'predicted_value_prefixs': predicted_value_prefixs.detach().cpu().numpy().mean().item(),
-            'predicted_values': predicted_values.detach().cpu().numpy().mean().item(),
-            'total_grad_norm_before_clip': total_grad_norm_before_clip.item()
+            'value_priority_orig': value_priority,  # torch.tensor compatible with ddp settings
         }
 
     def _init_collect(self) -> None:
         """
          Overview:
              Collect mode init method. Called by ``self.__init__``. Initialize the collect model and MCTS utils.
          """
@@ -532,15 +533,15 @@
     def _forward_collect(
         self,
         data: torch.Tensor,
         action_mask: list = None,
         temperature: float = 1,
         to_play: List = [-1],
         epsilon: float = 0.25,
-        ready_env_id = None
+        ready_env_id: np.array = None
     ):
         """
         Overview:
             The forward function for collecting data in collect mode. Use model to execute MCTS search.
             Choosing the action through sampling during the collect mode.
         Arguments:
             - data (:obj:`torch.Tensor`): The input data, i.e. the observation.
```

### Comparing `LightZero-0.0.2/lzero/policy/gumbel_muzero.py` & `LightZero-0.0.5/lzero/policy/gumbel_muzero.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,15 +54,15 @@
             # (bool) whether to learn bias in the last linear layer in value and policy head.
             bias=True,
             # (str) The type of action encoding. Options are ['one_hot', 'not_one_hot']. Default to 'one_hot'.
             discrete_action_encoding_type='one_hot',
             # (bool) whether to use res connection in dynamics.
             res_connection_in_dynamics=True,
             # (str) The type of normalization in MuZero model. Options are ['BN', 'LN']. Default to 'LN'.
-            norm_type='BN', 
+            norm_type='BN',
         ),
         # ****** common ******
         # (bool) Whether to use multi-gpu training.
         multi_gpu=False,
         # (bool) Whether to enable the sampled-based algorithm (e.g. Sampled EfficientZero)
         # this variable is used in ``collector``.
         sampled_algo=False,
@@ -74,20 +74,27 @@
         cuda=True,
         # (int) The number of environments used in collecting data.
         collector_env_num=8,
         # (int) The number of environments used in evaluating policy.
         evaluator_env_num=3,
         # (str) The type of environment. Options is ['not_board_games', 'board_games'].
         env_type='not_board_games',
+        # (str) The type of action space. Options are ['fixed_action_space', 'varied_action_space'].
+        action_type='fixed_action_space',
         # (str) The type of battle mode. Options is ['play_with_bot_mode', 'self_play_mode'].
         battle_mode='play_with_bot_mode',
         # (bool) Whether to monitor extra statistics in tensorboard.
         monitor_extra_statistics=True,
         # (int) The transition number of one ``GameSegment``.
         game_segment_length=200,
+        # (bool): Indicates whether to perform an offline evaluation of the checkpoint (ckpt).
+        # If set to True, the checkpoint will be evaluated after the training process is complete.
+        # IMPORTANT: Setting eval_offline to True requires configuring the saving of checkpoints to align with the evaluation frequency.
+        # This is done by setting the parameter learn.learner.hook.save_ckpt_after_iter to the same value as eval_freq in the train_muzero.py automatically.
+        eval_offline=False,
 
         # ****** observation ******
         # (bool) Whether to transform image to string to save memory.
         transform2string=False,
         # (bool) Whether to use gray scale image.
         gray_scale=False,
         # (bool) Whether to use data augmentation.
@@ -150,14 +157,16 @@
         # (bool) Whether to use manually decayed temperature.
         manual_temperature_decay=False,
         # (int) The number of final training iterations to control temperature, which is only used for manually decay.
         threshold_training_steps_for_final_temperature=int(1e5),
         # (float) The fixed temperature value for MCTS action selection, which is used to control the exploration.
         # The larger the value, the more exploration. This value is only used when manual_temperature_decay=False.
         fixed_temperature_value=0.25,
+        # (bool) Whether to add noise to roots during reanalyze process.
+        reanalyze_noise=False,
 
         # ****** Priority ******
         # (bool) Whether to use priority when sampling training data from the buffer.
         use_priority=True,
         # (float) The degree of prioritization to use. A value of 0 means no prioritization,
         # while a value of 1 means full prioritization.
         priority_prob_alpha=0.6,
@@ -224,15 +233,16 @@
                 weight_decay=self._cfg.weight_decay,
             )
         elif self._cfg.optim_type == 'Adam':
             self._optimizer = optim.Adam(
                 self._model.parameters(), lr=self._cfg.learning_rate, weight_decay=self._cfg.weight_decay
             )
         elif self._cfg.optim_type == 'AdamW':
-            self._optimizer = configure_optimizers(model=self._model, weight_decay=self._cfg.weight_decay, learning_rate=self._cfg.learning_rate, device_type=self._cfg.device)
+            self._optimizer = configure_optimizers(model=self._model, weight_decay=self._cfg.weight_decay,
+                                                   learning_rate=self._cfg.learning_rate, device_type=self._cfg.device)
 
         if self._cfg.lr_piecewise_constant_decay:
             from torch.optim.lr_scheduler import LambdaLR
             max_step = self._cfg.threshold_training_steps_for_final_lr
             # NOTE: the 1, 0.1, 0.01 is the decay rate, not the lr.
             lr_lambda = lambda step: 1 if step < max_step * 0.5 else (0.1 if step < max_step else 0.01)  # noqa
             self.lr_scheduler = LambdaLR(self._optimizer, lr_lambda=lr_lambda)
@@ -315,24 +325,23 @@
 
         # ==============================================================
         # the core initial_inference in Gumbel MuZero policy.
         # ==============================================================
         network_output = self._learn_model.initial_inference(obs_batch)
 
         # value_prefix shape: (batch_size, 10), the ``value_prefix`` at the first step is zero padding.
-        hidden_state, reward, value, policy_logits = mz_network_output_unpack(network_output)
+        latent_state, reward, value, policy_logits = mz_network_output_unpack(network_output)
 
         # transform the scaled value or its categorical representation to its original value,
         # i.e. h^(-1)(.) function in paper https://arxiv.org/pdf/1805.11593.pdf.
         original_value = self.inverse_scalar_transform_handle(value)
 
         # Note: The following lines are just for debugging.
         predicted_rewards = []
         if self._cfg.monitor_extra_statistics:
-            hidden_state_list = hidden_state.detach().cpu().numpy()
             predicted_values, predicted_policies = original_value.detach().cpu(), torch.softmax(
                 policy_logits, dim=1
             ).detach().cpu()
 
         # calculate the new priorities for each transition.
         value_priority = L1Loss(reduction='none')(original_value.squeeze(-1), target_value[:, 0])
         value_priority = value_priority.data.cpu().numpy() + 1e-6
@@ -340,88 +349,91 @@
         # ==============================================================
         # calculate policy and value loss for the first step.
         # ==============================================================
         # ==============================================================
         # The core difference between GumbelMuZero and MuZero
         # ==============================================================
         # In Gumbel MuZero, the policy loss is defined as the KL loss between current policy and improved policy calculated in MCTS.
-        policy_loss = self.kl_loss(torch.log(torch.softmax(policy_logits, dim=1)), torch.from_numpy(improved_policy_batch[:, 0]).to(self._cfg.device).detach().float())
-        policy_loss = policy_loss.mean(dim=-1)*mask_batch[:,0]
+        policy_loss = self.kl_loss(torch.log(torch.softmax(policy_logits, dim=1)),
+                                   torch.from_numpy(improved_policy_batch[:, 0]).to(self._cfg.device).detach().float())
+        policy_loss = policy_loss.mean(dim=-1) * mask_batch[:, 0]
         # Output the entropy for experimental observation.
-        entropy_loss = -torch.sum(torch.softmax(policy_logits, dim=1) * torch.log(torch.softmax(policy_logits, dim=1)), dim=-1)
+
+        prob = torch.softmax(policy_logits, dim=-1)
+        policy_entropy = -(prob * prob.log()).sum(-1)
 
         value_loss = cross_entropy_loss(value, target_value_categorical[:, 0])
 
         reward_loss = torch.zeros(self._cfg.batch_size, device=self._cfg.device)
         consistency_loss = torch.zeros(self._cfg.batch_size, device=self._cfg.device)
 
         # ==============================================================
         # the core recurrent_inference in Gumbel MuZero policy.
         # ==============================================================
         for step_k in range(self._cfg.num_unroll_steps):
-            # unroll with the dynamics function: predict the next ``hidden_state``, ``reward``,
-            # given current ``hidden_state`` and ``action``.
+            # unroll with the dynamics function: predict the next ``latent_state``, ``reward``,
+            # given current ``latent_state`` and ``action``.
             # And then predict policy_logits and value with the prediction function.
-            network_output = self._learn_model.recurrent_inference(hidden_state, action_batch[:, step_k])
-            hidden_state, reward, value, policy_logits = mz_network_output_unpack(network_output)
+            network_output = self._learn_model.recurrent_inference(latent_state, action_batch[:, step_k])
+            latent_state, reward, value, policy_logits = mz_network_output_unpack(network_output)
 
             # transform the scaled value or its categorical representation to its original value,
             # i.e. h^(-1)(.) function in paper https://arxiv.org/pdf/1805.11593.pdf.
             original_value = self.inverse_scalar_transform_handle(value)
 
             if self._cfg.model.self_supervised_learning_loss:
                 # ==============================================================
                 # calculate consistency loss for the next ``num_unroll_steps`` unroll steps.
                 # ==============================================================
                 if self._cfg.ssl_loss_weight > 0:
                     # obtain the oracle latent states from representation function.
                     beg_index, end_index = self._get_target_obs_index_in_step_k(step_k)
                     network_output = self._learn_model.initial_inference(obs_target_batch[:, beg_index:end_index])
 
-                    hidden_state = to_tensor(hidden_state)
+                    latent_state = to_tensor(latent_state)
                     representation_state = to_tensor(network_output.latent_state)
 
                     # NOTE: no grad for the representation_state branch
-                    dynamic_proj = self._learn_model.project(hidden_state, with_grad=True)
+                    dynamic_proj = self._learn_model.project(latent_state, with_grad=True)
                     observation_proj = self._learn_model.project(representation_state, with_grad=False)
                     temp_loss = negative_cosine_similarity(dynamic_proj, observation_proj) * mask_batch[:, step_k]
                     consistency_loss += temp_loss
 
             # NOTE: the target policy, target_value_categorical, target_reward_categorical is calculated in
             # game buffer now.
             # ==============================================================
             # calculate policy loss for the next ``num_unroll_steps`` unroll steps.
             # NOTE: the +=.
             # ==============================================================
-            policy_loss += self.kl_loss(torch.log(torch.softmax(policy_logits, dim=1)),torch.from_numpy(improved_policy_batch[:, step_k + 1]).to(self._cfg.device).detach().float()).mean(dim=-1) * mask_batch[:,step_k+1]
+            policy_loss += self.kl_loss(torch.log(torch.softmax(policy_logits, dim=1)),
+                                        torch.from_numpy(improved_policy_batch[:, step_k + 1]).to(
+                                            self._cfg.device).detach().float()).mean(dim=-1) * mask_batch[:, step_k + 1]
             value_loss += cross_entropy_loss(value, target_value_categorical[:, step_k + 1])
             reward_loss += cross_entropy_loss(reward, target_reward_categorical[:, step_k])
-            entropy_loss += -torch.sum(torch.softmax(policy_logits, dim=1) * torch.log(torch.softmax(policy_logits, dim=1)), dim=-1)
 
-            # Follow MuZero, set half gradient
-            # hidden_state.register_hook(lambda grad: grad * 0.5)
+            prob = torch.softmax(policy_logits, dim=-1)
+            policy_entropy += (prob * prob.log()).sum(-1)
 
             if self._cfg.monitor_extra_statistics:
                 original_rewards = self.inverse_scalar_transform_handle(reward)
                 original_rewards_cpu = original_rewards.detach().cpu()
 
                 predicted_values = torch.cat(
                     (predicted_values, self.inverse_scalar_transform_handle(value).detach().cpu())
                 )
                 predicted_rewards.append(original_rewards_cpu)
                 predicted_policies = torch.cat((predicted_policies, torch.softmax(policy_logits, dim=1).detach().cpu()))
-                hidden_state_list = np.concatenate((hidden_state_list, hidden_state.detach().cpu().numpy()))
 
         # ==============================================================
         # the core learn model update step.
         # ==============================================================
         # weighted loss with masks (some invalid states which are out of trajectory.)
         loss = (
-            self._cfg.ssl_loss_weight * consistency_loss + self._cfg.policy_loss_weight * policy_loss +
-            self._cfg.value_loss_weight * value_loss + self._cfg.reward_loss_weight * reward_loss
+                self._cfg.ssl_loss_weight * consistency_loss + self._cfg.policy_loss_weight * policy_loss +
+                self._cfg.value_loss_weight * value_loss + self._cfg.reward_loss_weight * reward_loss
         )
         weighted_total_loss = (weights * loss).mean()
 
         gradient_scale = 1 / self._cfg.num_unroll_steps
         weighted_total_loss.register_hook(lambda grad: grad * gradient_scale)
         self._optimizer.zero_grad()
         weighted_total_loss.backward()
@@ -448,15 +460,15 @@
             'cur_lr': self._optimizer.param_groups[0]['lr'],
             'weighted_total_loss': weighted_total_loss.item(),
             'total_loss': loss.mean().item(),
             'policy_loss': policy_loss.mean().item(),
             'reward_loss': reward_loss.mean().item(),
             'value_loss': value_loss.mean().item(),
             'consistency_loss': consistency_loss.mean().item() / self._cfg.num_unroll_steps,
-            'entropy_loss': entropy_loss.mean().item(),
+            'policy_entropy': policy_entropy.mean().item(),
 
             # ==============================================================
             # priority related
             # ==============================================================
             'value_priority_orig': value_priority,
             'value_priority': value_priority.mean().item(),
             'target_reward': target_reward.detach().cpu().numpy().mean().item(),
@@ -541,42 +553,46 @@
 
             roots.prepare(self._cfg.root_noise_weight, noises, reward_roots, list(pred_values), policy_logits, to_play)
             self._mcts_collect.search(roots, self._collect_model, latent_state_roots, to_play)
 
             # list of list, shape: ``{list: batch_size} -> {list: action_space_size}``
             roots_visit_count_distributions = roots.get_distributions()
             roots_values = roots.get_values()  # shape: {list: batch_size}
-            roots_completed_values = roots.get_children_values(self._cfg.discount_factor, self._cfg.model.action_space_size)
+            roots_completed_values = roots.get_children_values(self._cfg.discount_factor,
+                                                               self._cfg.model.action_space_size)
 
             # ==============================================================
             # The core difference between GumbelMuZero and MuZero
             # ==============================================================
             # Gumbel MuZero selects the action according to the improved policy
-            roots_improved_policy_probs = roots.get_policies(self._cfg.discount_factor, self._cfg.model.action_space_size) # new policy constructed with completed Q in gumbel muzero
+            roots_improved_policy_probs = roots.get_policies(self._cfg.discount_factor,
+                                                             self._cfg.model.action_space_size)  # new policy constructed with completed Q in gumbel muzero
             roots_improved_policy_probs = np.array(roots_improved_policy_probs)
 
             data_id = [i for i in range(active_collect_env_num)]
             output = {i: None for i in data_id}
 
             if ready_env_id is None:
                 ready_env_id = np.arange(active_collect_env_num)
 
             for i, env_id in enumerate(ready_env_id):
-                distributions, value, improved_policy_probs = roots_visit_count_distributions[i], roots_values[i], roots_improved_policy_probs[i]
+                distributions, value, improved_policy_probs = roots_visit_count_distributions[i], roots_values[i], \
+                roots_improved_policy_probs[i]
 
                 roots_completed_value = roots_completed_values[i]
                 # NOTE: Only legal actions possess visit counts, so the ``action_index_in_legal_action_set`` represents
                 # the index within the legal action set, rather than the index in the entire action set.
                 action_index_in_legal_action_set, visit_count_distribution_entropy = select_action(
                     distributions, temperature=self._collect_mcts_temperature, deterministic=False
                 )
                 # NOTE: Convert the ``action_index_in_legal_action_set`` to the corresponding ``action`` in the
                 # entire action set.
                 valid_value = np.where(action_mask[i] == 1.0, improved_policy_probs, 0.0)
                 action = np.argmax([v for v in valid_value])
+                roots_completed_value = np.where(action_mask[i] == 1.0, roots_completed_value, 0.0)
 
                 output[env_id] = {
                     'action': action,
                     'visit_count_distributions': distributions,
                     'visit_count_distribution_entropy': visit_count_distribution_entropy,
                     'searched_value': value,
                     'roots_completed_value': roots_completed_value,
@@ -594,15 +610,16 @@
         """
         self._eval_model = self._model
         if self._cfg.mcts_ctree:
             self._mcts_eval = MCTSCtree(self._cfg)
         else:
             self._mcts_eval = MCTSPtree(self._cfg)
 
-    def _forward_eval(self, data: torch.Tensor, action_mask: list, to_play: int = -1, ready_env_id: np.array = None,) -> Dict:
+    def _forward_eval(self, data: torch.Tensor, action_mask: list, to_play: int = -1,
+                      ready_env_id: np.array = None, ) -> Dict:
         """
         Overview:
             The forward function for evaluating the current policy in eval mode. Use model to execute MCTS search.
             Choosing the action with the highest value (argmax) rather than sampling during the eval mode.
         Arguments:
             - data (:obj:`torch.Tensor`): The input data, i.e. the observation.
             - action_mask (:obj:`list`): The action mask, i.e. the action that cannot be selected.
@@ -647,25 +664,27 @@
             roots_visit_count_distributions = roots.get_distributions()
             roots_values = roots.get_values()  # shape: {list: batch_size}
 
             # ==============================================================
             # The core difference between GumbelMuZero and MuZero
             # ==============================================================
             # Gumbel MuZero selects the action according to the improved policy
-            roots_improved_policy_probs = roots.get_policies(self._cfg.discount_factor, self._cfg.model.action_space_size) # new policy constructed with completed Q in gumbel muzero
+            roots_improved_policy_probs = roots.get_policies(self._cfg.discount_factor,
+                                                             self._cfg.model.action_space_size)  # new policy constructed with completed Q in gumbel muzero
             roots_improved_policy_probs = np.array(roots_improved_policy_probs)
 
             data_id = [i for i in range(active_eval_env_num)]
             output = {i: None for i in data_id}
 
             if ready_env_id is None:
                 ready_env_id = np.arange(active_eval_env_num)
 
             for i, env_id in enumerate(ready_env_id):
-                distributions, value, improved_policy_probs = roots_visit_count_distributions[i], roots_values[i], roots_improved_policy_probs[i]
+                distributions, value, improved_policy_probs = roots_visit_count_distributions[i], roots_values[i], \
+                roots_improved_policy_probs[i]
                 # NOTE: Only legal actions possess visit counts, so the ``action_index_in_legal_action_set`` represents
                 # the index within the legal action set, rather than the index in the entire action set.
                 #  Setting deterministic=True implies choosing the action with the highest value (argmax) rather than
                 # sampling during the evaluation phase.
                 action_index_in_legal_action_set, visit_count_distribution_entropy = select_action(
                     distributions, temperature=1, deterministic=True
                 )
@@ -698,15 +717,15 @@
             'cur_lr',
             'weighted_total_loss',
             'total_loss',
             'policy_loss',
             'reward_loss',
             'value_loss',
             'consistency_loss',
-            'entropy_loss',
+            'policy_entropy',
             'value_priority',
             'target_reward',
             'target_value',
             'predicted_rewards',
             'predicted_values',
             'transformed_target_reward',
             'transformed_target_value',
```

### Comparing `LightZero-0.0.2/lzero/policy/muzero.py` & `LightZero-0.0.5/lzero/policy/muzero.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import numpy as np
 import torch
 import torch.optim as optim
 from ding.model import model_wrap
 from ding.policy.base_policy import Policy
 from ding.torch_utils import to_tensor
 from ding.utils import POLICY_REGISTRY
-from torch.distributions import Categorical
 from torch.nn import L1Loss
 
 from lzero.mcts import MuZeroMCTSCtree as MCTSCtree
 from lzero.mcts import MuZeroMCTSPtree as MCTSPtree
 from lzero.model import ImageTransforms
 from lzero.policy import scalar_transform, InverseScalarTransform, cross_entropy_loss, phi_transform, \
     DiscreteSupport, to_torch_float_tensor, mz_network_output_unpack, select_action, negative_cosine_similarity, \
@@ -35,14 +34,15 @@
             continuous_action_space=False,
             # (tuple) The stacked obs shape.
             # observation_shape=(1, 96, 96),  # if frame_stack_num=1
             observation_shape=(4, 96, 96),  # if frame_stack_num=4
             # (bool) Whether to use the self-supervised learning loss.
             self_supervised_learning_loss=False,
             # (bool) Whether to use discrete support to represent categorical distribution for value/reward/value_prefix.
+            # reference: http://proceedings.mlr.press/v80/imani18a/imani18a.pdf, https://arxiv.org/abs/2403.03950
             categorical_distribution=True,
             # (int) The image channel in image observation.
             image_channel=1,
             # (int) The number of frames to stack together.
             frame_stack_num=1,
             # (int) The number of res blocks in MuZero model.
             num_res_blocks=1,
@@ -76,20 +76,27 @@
         cuda=True,
         # (int) The number of environments used in collecting data.
         collector_env_num=8,
         # (int) The number of environments used in evaluating policy.
         evaluator_env_num=3,
         # (str) The type of environment. Options are ['not_board_games', 'board_games'].
         env_type='not_board_games',
+        # (str) The type of action space. Options are ['fixed_action_space', 'varied_action_space'].
+        action_type='fixed_action_space',
         # (str) The type of battle mode. Options are ['play_with_bot_mode', 'self_play_mode'].
         battle_mode='play_with_bot_mode',
         # (bool) Whether to monitor extra statistics in tensorboard.
         monitor_extra_statistics=True,
         # (int) The transition number of one ``GameSegment``.
         game_segment_length=200,
+        # (bool): Indicates whether to perform an offline evaluation of the checkpoint (ckpt).
+        # If set to True, the checkpoint will be evaluated after the training process is complete.
+        # IMPORTANT: Setting eval_offline to True requires configuring the saving of checkpoints to align with the evaluation frequency.
+        # This is done by setting the parameter learn.learner.hook.save_ckpt_after_iter to the same value as eval_freq in the train_muzero.py automatically.
+        eval_offline=False,
 
         # ****** observation ******
         # (bool) Whether to transform image to string to save memory.
         transform2string=False,
         # (bool) Whether to use gray scale image.
         gray_scale=False,
         # (bool) Whether to use data augmentation.
@@ -157,14 +164,16 @@
         # (int) The number of final training iterations to control temperature, which is only used for manually decay.
         threshold_training_steps_for_final_temperature=int(1e5),
         # (float) The fixed temperature value for MCTS action selection, which is used to control the exploration.
         # The larger the value, the more exploration. This value is only used when manual_temperature_decay=False.
         fixed_temperature_value=0.25,
         # (bool) Whether to use the true chance in MCTS in some environments with stochastic dynamics, such as 2048.
         use_ture_chance_label_in_chance_encoder=False,
+        # (bool) Whether to add noise to roots during reanalyze process.
+        reanalyze_noise=False,
 
         # ****** Priority ******
         # (bool) Whether to use priority when sampling training data from the buffer.
         use_priority=True,
         # (float) The degree of prioritization to use. A value of 0 means no prioritization,
         # while a value of 1 means full prioritization.
         priority_prob_alpha=0.6,
@@ -346,33 +355,30 @@
         # transform the scaled value or its categorical representation to its original value,
         # i.e. h^(-1)(.) function in paper https://arxiv.org/pdf/1805.11593.pdf.
         original_value = self.inverse_scalar_transform_handle(value)
 
         # Note: The following lines are just for debugging.
         predicted_rewards = []
         if self._cfg.monitor_extra_statistics:
-            latent_state_list = latent_state.detach().cpu().numpy()
             predicted_values, predicted_policies = original_value.detach().cpu(), torch.softmax(
                 policy_logits, dim=1
             ).detach().cpu()
 
         # calculate the new priorities for each transition.
-        value_priority = L1Loss(reduction='none')(original_value.squeeze(-1), target_value[:, 0])
-        value_priority = value_priority.data.cpu().numpy() + 1e-6
+        value_priority = L1Loss(reduction='none')(original_value.squeeze(-1), target_value[:, 0]) + 1e-6
 
         # ==============================================================
         # calculate policy and value loss for the first step.
         # ==============================================================
         policy_loss = cross_entropy_loss(policy_logits, target_policy[:, 0])
         value_loss = cross_entropy_loss(value, target_value_categorical[:, 0])
 
         prob = torch.softmax(policy_logits, dim=-1)
-        dist = Categorical(prob)
-        policy_entropy_loss = -dist.entropy()
-
+        entropy = -(prob * prob.log()).sum(-1)
+        policy_entropy_loss = -entropy
 
         reward_loss = torch.zeros(self._cfg.batch_size, device=self._cfg.device)
         consistency_loss = torch.zeros(self._cfg.batch_size, device=self._cfg.device)
 
         # ==============================================================
         # the core recurrent_inference in MuZero policy.
         # ==============================================================
@@ -410,33 +416,29 @@
             # ==============================================================
             # calculate policy loss for the next ``num_unroll_steps`` unroll steps.
             # NOTE: the +=.
             # ==============================================================
             policy_loss += cross_entropy_loss(policy_logits, target_policy[:, step_k + 1])
 
             prob = torch.softmax(policy_logits, dim=-1)
-            dist = Categorical(prob)
-            policy_entropy_loss += -dist.entropy()
+            entropy = -(prob * prob.log()).sum(-1)
+            policy_entropy_loss += -entropy
 
             value_loss += cross_entropy_loss(value, target_value_categorical[:, step_k + 1])
             reward_loss += cross_entropy_loss(reward, target_reward_categorical[:, step_k])
 
-            # Follow MuZero, set half gradient
-            # latent_state.register_hook(lambda grad: grad * 0.5)
-
             if self._cfg.monitor_extra_statistics:
                 original_rewards = self.inverse_scalar_transform_handle(reward)
                 original_rewards_cpu = original_rewards.detach().cpu()
 
                 predicted_values = torch.cat(
                     (predicted_values, self.inverse_scalar_transform_handle(value).detach().cpu())
                 )
                 predicted_rewards.append(original_rewards_cpu)
                 predicted_policies = torch.cat((predicted_policies, torch.softmax(policy_logits, dim=1).detach().cpu()))
-                latent_state_list = np.concatenate((latent_state_list, latent_state.detach().cpu().numpy()))
 
         # ==============================================================
         # the core learn model update step.
         # ==============================================================
         # weighted loss with masks (some invalid states which are out of trajectory.)
         loss = (
                 self._cfg.ssl_loss_weight * consistency_loss + self._cfg.policy_loss_weight * policy_loss +
@@ -447,17 +449,16 @@
 
         gradient_scale = 1 / self._cfg.num_unroll_steps
         weighted_total_loss.register_hook(lambda grad: grad * gradient_scale)
         self._optimizer.zero_grad()
         weighted_total_loss.backward()
         if self._cfg.multi_gpu:
             self.sync_gradients(self._learn_model)
-        total_grad_norm_before_clip = torch.nn.utils.clip_grad_norm_(
-            self._learn_model.parameters(), self._cfg.grad_clip_value
-        )
+        total_grad_norm_before_clip = torch.nn.utils.clip_grad_norm_(self._learn_model.parameters(),
+                                                                     self._cfg.grad_clip_value)
         self._optimizer.step()
         if self._cfg.lr_piecewise_constant_decay:
             self.lr_scheduler.step()
 
         # ==============================================================
         # the core target model update step.
         # ==============================================================
@@ -476,27 +477,26 @@
             'weighted_total_loss': weighted_total_loss.item(),
             'total_loss': loss.mean().item(),
             'policy_loss': policy_loss.mean().item(),
             'policy_entropy': - policy_entropy_loss.mean().item() / (self._cfg.num_unroll_steps + 1),
             'reward_loss': reward_loss.mean().item(),
             'value_loss': value_loss.mean().item(),
             'consistency_loss': consistency_loss.mean().item() / self._cfg.num_unroll_steps,
-
+            'target_reward': target_reward.mean().item(),
+            'target_value': target_value.mean().item(),
+            'transformed_target_reward': transformed_target_reward.mean().item(),
+            'transformed_target_value': transformed_target_value.mean().item(),
+            'predicted_rewards': predicted_rewards.mean().item(),
+            'predicted_values': predicted_values.mean().item(),
+            'total_grad_norm_before_clip': total_grad_norm_before_clip.item(),
             # ==============================================================
             # priority related
             # ==============================================================
-            'value_priority_orig': value_priority,
             'value_priority': value_priority.mean().item(),
-            'target_reward': target_reward.detach().cpu().numpy().mean().item(),
-            'target_value': target_value.detach().cpu().numpy().mean().item(),
-            'transformed_target_reward': transformed_target_reward.detach().cpu().numpy().mean().item(),
-            'transformed_target_value': transformed_target_value.detach().cpu().numpy().mean().item(),
-            'predicted_rewards': predicted_rewards.detach().cpu().numpy().mean().item(),
-            'predicted_values': predicted_values.detach().cpu().numpy().mean().item(),
-            'total_grad_norm_before_clip': total_grad_norm_before_clip.item()
+            'value_priority_orig': value_priority,  # torch.tensor compatible with ddp settings
         }
 
     def _init_collect(self) -> None:
         """
         Overview:
             Collect mode init method. Called by ``self.__init__``. Initialize the collect model and MCTS utils.
         """
@@ -642,15 +642,16 @@
             beg_index = self._cfg.model.image_channel * step
             end_index = self._cfg.model.image_channel * (step + self._cfg.model.frame_stack_num)
         elif self._cfg.model.model_type == 'mlp':
             beg_index = self._cfg.model.observation_shape * step
             end_index = self._cfg.model.observation_shape * (step + self._cfg.model.frame_stack_num)
         return beg_index, end_index
 
-    def _forward_eval(self, data: torch.Tensor, action_mask: list, to_play: int = -1, ready_env_id: np.array = None,) -> Dict:
+    def _forward_eval(self, data: torch.Tensor, action_mask: list, to_play: int = -1,
+                      ready_env_id: np.array = None, ) -> Dict:
         """
         Overview:
             The forward function for evaluating the current policy in eval mode. Use model to execute MCTS search.
             Choosing the action with the highest value (argmax) rather than sampling during the eval mode.
         Arguments:
             - data (:obj:`torch.Tensor`): The input data, i.e. the observation.
             - action_mask (:obj:`list`): The action mask, i.e. the action that cannot be selected.
```

### Comparing `LightZero-0.0.2/lzero/policy/random_policy.py` & `LightZero-0.0.5/lzero/policy/random_policy.py`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/lzero/policy/sampled_alphazero.py` & `LightZero-0.0.5/lzero/policy/sampled_alphazero.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,32 +194,31 @@
         if len(root_sampled_actions.shape) == 1:
             print(f"root_sampled_actions.shape: {root_sampled_actions.shape}")
         state_batch = state_batch.to(device=self._device, dtype=torch.float)
         mcts_visit_count_probs = mcts_visit_count_probs.to(device=self._device, dtype=torch.float)
         reward = reward.to(device=self._device, dtype=torch.float)
 
         policy_probs, values = self._learn_model.compute_policy_value(state_batch)
-        policy_log_probs = torch.log(policy_probs)
 
         # calculate policy entropy, for monitoring only
-        entropy = compute_entropy(policy_probs)
-        entropy_loss = -entropy
+        policy_entropy = -(policy_probs * policy_probs.log()).sum(-1).mean()
+        policy_entropy_loss = -policy_entropy
 
         # ==============================================================
         # policy loss
         # ==============================================================
         policy_loss = self._calculate_policy_loss_disc(policy_probs, mcts_visit_count_probs, root_sampled_actions,
                                                        valid_action_length)
 
         # ==============================================================
         # value loss
         # ==============================================================
         value_loss = F.mse_loss(values.view(-1), reward)
 
-        total_loss = self._value_weight * value_loss + policy_loss + self._entropy_weight * entropy_loss
+        total_loss = self._value_weight * value_loss + policy_loss + self._entropy_weight * policy_entropy_loss
         self._optimizer.zero_grad()
         total_loss.backward()
 
         total_grad_norm_before_clip = torch.nn.utils.clip_grad_norm_(
             list(self._model.parameters()),
             max_norm=self._cfg.grad_clip_value,
         )
@@ -231,15 +230,15 @@
         # after update
         # =============
         return {
             'cur_lr': self._optimizer.param_groups[0]['lr'],
             'total_loss': total_loss.item(),
             'policy_loss': policy_loss.item(),
             'value_loss': value_loss.item(),
-            'entropy_loss': entropy_loss.item(),
+            'policy_entropy_loss': policy_entropy_loss.item(),
             'total_grad_norm_before_clip': total_grad_norm_before_clip.item(),
             'collect_mcts_temperature': self.collect_mcts_temperature,
         }
 
     def _calculate_policy_loss_disc(
             self, policy_probs: torch.Tensor, target_policy: torch.Tensor,
             target_sampled_actions: torch.Tensor, valid_action_lengths: torch.Tensor
@@ -456,18 +455,18 @@
             output[env_id] = {
                 'action': action,
                 'probs': mcts_visit_count_probs,
             }
         return output
 
     def _get_simulation_env(self):
-        assert self._cfg.simulation_env_name in ['tictactoe', 'gomoku', 'go'], self._cfg.simulation_env_name
+        assert self._cfg.simulation_env_id in ['tictactoe', 'gomoku', 'go'], self._cfg.simulation_env_id
         assert self._cfg.simulation_env_config_type in ['play_with_bot', 'self_play', 'league',
                                                         'sampled_play_with_bot'], self._cfg.simulation_env_config_type
-        if self._cfg.simulation_env_name == 'tictactoe':
+        if self._cfg.simulation_env_id == 'tictactoe':
             from zoo.board_games.tictactoe.envs.tictactoe_env import TicTacToeEnv
             if self._cfg.simulation_env_config_type == 'play_with_bot':
                 from zoo.board_games.tictactoe.config.tictactoe_alphazero_bot_mode_config import \
                     tictactoe_alphazero_config
             elif self._cfg.simulation_env_config_type == 'self_play':
                 from zoo.board_games.tictactoe.config.tictactoe_alphazero_sp_mode_config import \
                     tictactoe_alphazero_config
@@ -476,28 +475,28 @@
                     tictactoe_alphazero_config
             elif self._cfg.simulation_env_config_type == 'sampled_play_with_bot':
                 from zoo.board_games.tictactoe.config.tictactoe_sampled_alphazero_bot_mode_config import \
                     tictactoe_sampled_alphazero_config as tictactoe_alphazero_config
 
             self.simulate_env = TicTacToeEnv(tictactoe_alphazero_config.env)
 
-        elif self._cfg.simulation_env_name == 'gomoku':
+        elif self._cfg.simulation_env_id == 'gomoku':
             from zoo.board_games.gomoku.envs.gomoku_env import GomokuEnv
             if self._cfg.simulation_env_config_type == 'play_with_bot':
                 from zoo.board_games.gomoku.config.gomoku_alphazero_bot_mode_config import gomoku_alphazero_config
             elif self._cfg.simulation_env_config_type == 'self_play':
                 from zoo.board_games.gomoku.config.gomoku_alphazero_sp_mode_config import gomoku_alphazero_config
             elif self._cfg.simulation_env_config_type == 'league':
                 from zoo.board_games.gomoku.config.gomoku_alphazero_league_config import gomoku_alphazero_config
             elif self._cfg.simulation_env_config_type == 'sampled_play_with_bot':
                 from zoo.board_games.gomoku.config.gomoku_sampled_alphazero_bot_mode_config import \
                     gomoku_sampled_alphazero_config as gomoku_alphazero_config
 
             self.simulate_env = GomokuEnv(gomoku_alphazero_config.env)
-        elif self._cfg.simulation_env_name == 'go':
+        elif self._cfg.simulation_env_id == 'go':
             from zoo.board_games.go.envs.go_env import GoEnv
             if self._cfg.simulation_env_config_type == 'play_with_bot':
                 from zoo.board_games.go.config.go_alphazero_bot_mode_config import go_alphazero_config
             elif self._cfg.simulation_env_config_type == 'self_play':
                 from zoo.board_games.go.config.go_alphazero_sp_mode_config import go_alphazero_config
             elif self._cfg.simulation_env_config_type == 'league':
                 from zoo.board_games.go.config.go_alphazero_league_config import go_alphazero_config
@@ -534,15 +533,15 @@
     def _monitor_vars_learn(self) -> List[str]:
         """
         Overview:
             Register the variables to be monitored in learn mode. The registered variables will be logged in
             tensorboard according to the return value ``_forward_learn``.
         """
         return super()._monitor_vars_learn() + [
-            'cur_lr', 'total_loss', 'policy_loss', 'value_loss', 'entropy_loss', 'total_grad_norm_before_clip',
+            'cur_lr', 'total_loss', 'policy_loss', 'value_loss', 'policy_entropy_loss', 'total_grad_norm_before_clip',
             'collect_mcts_temperature'
         ]
 
     def _process_transition(self, obs: Dict, model_output: Dict[str, torch.Tensor], timestep: namedtuple) -> Dict:
         """
         Overview:
             Generate the dict type transition (one timestep) data from policy learning.
```

### Comparing `LightZero-0.0.2/lzero/policy/sampled_efficientzero.py` & `LightZero-0.0.5/lzero/policy/sampled_efficientzero.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,20 +80,27 @@
         cuda=True,
         # (int) The number of environments used in collecting data.
         collector_env_num=8,
         # (int) The number of environments used in evaluating policy.
         evaluator_env_num=3,
         # (str) The type of environment. The options are ['not_board_games', 'board_games'].
         env_type='not_board_games',
+        # (str) The type of action space. Options are ['fixed_action_space', 'varied_action_space'].
+        action_type='fixed_action_space',
         # (str) The type of battle mode. The options are ['play_with_bot_mode', 'self_play_mode'].
         battle_mode='play_with_bot_mode',
         # (bool) Whether to monitor extra statistics in tensorboard.
         monitor_extra_statistics=True,
         # (int) The transition number of one ``GameSegment``.
         game_segment_length=200,
+        # (bool): Indicates whether to perform an offline evaluation of the checkpoint (ckpt).
+        # If set to True, the checkpoint will be evaluated after the training process is complete.
+        # IMPORTANT: Setting eval_offline to True requires configuring the saving of checkpoints to align with the evaluation frequency.
+        # This is done by setting the parameter learn.learner.hook.save_ckpt_after_iter to the same value as eval_freq in the train_muzero.py automatically.
+        eval_offline=False,
 
         # ****** observation ******
         # (bool) Whether to transform image to string to save memory.
         transform2string=False,
         # (bool) Whether to use gray scale image.
         gray_scale=False,
         # (bool) Whether to use data augmentation.
@@ -168,14 +175,16 @@
         # i.e. temperature: 1 -> 0.5 -> 0.25
         manual_temperature_decay=False,
         # (float) The fixed temperature value for MCTS action selection, which is used to control the exploration.
         # The larger the value, the more exploration. This value is only used when manual_temperature_decay=False.
         fixed_temperature_value=0.25,
         # (bool) Whether to use the true chance in MCTS in some environments with stochastic dynamics, such as 2048.
         use_ture_chance_label_in_chance_encoder=False,
+        # (bool) Whether to add noise to roots during reanalyze process.
+        reanalyze_noise=False,
 
         # ****** Priority ******
         # (bool) Whether to use priority when sampling training data from the buffer.
         use_priority=True,
         # (float) The degree of prioritization to use. A value of 0 means no prioritization,
         # while a value of 1 means full prioritization.
         priority_prob_alpha=0.6,
@@ -326,27 +335,27 @@
         if self._cfg.use_augmentation:
             obs_batch = self.image_transforms.transform(obs_batch)
             if self._cfg.model.self_supervised_learning_loss:
                 obs_target_batch = self.image_transforms.transform(obs_target_batch)
 
         # shape: (batch_size, num_unroll_steps, action_dim)
         # NOTE: .float(), in continuous action space.
-        action_batch = torch.from_numpy(action_batch).to(self._cfg.device).float().unsqueeze(-1)
+        action_batch = torch.from_numpy(action_batch).to(self._cfg.device).float()
         data_list = [
             mask_batch,
             target_value_prefix.astype('float32'),
             target_value.astype('float32'), target_policy, weights
         ]
         [mask_batch, target_value_prefix, target_value, target_policy,
          weights] = to_torch_float_tensor(data_list, self._cfg.device)
         # ==============================================================
         # sampled related core code
         # ==============================================================
-        # shape: (batch_size, num_unroll_steps+1, num_of_sampled_actions, action_dim, 1), e.g. (4, 6, 5, 1, 1)
-        child_sampled_actions_batch = torch.from_numpy(child_sampled_actions_batch).to(self._cfg.device).unsqueeze(-1)
+        # shape: (batch_size, num_unroll_steps+1, num_of_sampled_actions, action_dim), e.g. (4, 6, 5, 1)
+        child_sampled_actions_batch = torch.from_numpy(child_sampled_actions_batch).to(self._cfg.device)
 
         target_value_prefix = target_value_prefix.view(self._cfg.batch_size, -1)
         target_value = target_value.view(self._cfg.batch_size, -1)
 
         assert obs_batch.size(0) == self._cfg.batch_size == target_value_prefix.size(0)
 
         # ``scalar_transform`` to transform the original value to the scaled value,
@@ -368,15 +377,14 @@
         # transform the scaled value or its categorical representation to its original value,
         # i.e. h^(-1)(.) function in paper https://arxiv.org/pdf/1805.11593.pdf.
         original_value = self.inverse_scalar_transform_handle(value)
 
         # Note: The following lines are just for logging.
         predicted_value_prefixs = []
         if self._cfg.monitor_extra_statistics:
-            latent_state_list = latent_state.detach().cpu().numpy()
             predicted_values, predicted_policies = original_value.detach().cpu(), torch.softmax(
                 policy_logits, dim=1
             ).detach().cpu()
 
         # calculate the new priorities for each transition.
         value_priority = L1Loss(reduction='none')(original_value.squeeze(-1), target_value[:, 0])
         value_priority = value_priority.data.cpu().numpy() + 1e-6
@@ -414,18 +422,14 @@
             network_output = self._learn_model.recurrent_inference(
                 latent_state, reward_hidden_state, action_batch[:, step_k]
             )
             latent_state, value_prefix, reward_hidden_state, value, policy_logits = ez_network_output_unpack(
                 network_output
             )
 
-            # transform the scaled value or its categorical representation to its original value,
-            # i.e. h^(-1)(.) function in paper https://arxiv.org/pdf/1805.11593.pdf.
-            original_value = self.inverse_scalar_transform_handle(value)
-
             if self._cfg.model.self_supervised_learning_loss:
                 # ==============================================================
                 # calculate consistency loss for the next ``num_unroll_steps`` unroll steps.
                 # ==============================================================
                 if self._cfg.ssl_loss_weight > 0:
                     # obtain the oracle latent states from representation function.
                     beg_index, end_index = self._get_target_obs_index_in_step_k(step_k)
@@ -484,15 +488,14 @@
                 original_value_prefixs_cpu = original_value_prefixs.detach().cpu()
 
                 predicted_values = torch.cat(
                     (predicted_values, self.inverse_scalar_transform_handle(value).detach().cpu())
                 )
                 predicted_value_prefixs.append(original_value_prefixs_cpu)
                 predicted_policies = torch.cat((predicted_policies, torch.softmax(policy_logits, dim=1).detach().cpu()))
-                latent_state_list = np.concatenate((latent_state_list, latent_state.detach().cpu().numpy()))
 
         # ==============================================================
         # the core learn model update step.
         # ==============================================================
         # weighted loss with masks (some invalid states which are out of trajectory.)
         loss = (
                 self._cfg.ssl_loss_weight * consistency_loss + self._cfg.policy_loss_weight * policy_loss +
@@ -619,17 +622,17 @@
             )
             target_dist = Categorical(target_normalized_visit_count_masked)
             target_policy_entropy = target_dist.entropy().mean()
         else:
             # Set target_policy_entropy to 0 if all rows are masked
             target_policy_entropy = 0
 
-        # shape: (batch_size, num_unroll_steps, num_of_sampled_actions, action_dim, 1) -> (batch_size,
-        # num_of_sampled_actions, action_dim) e.g. (4, 6, 20, 2, 1) ->  (4, 20, 2)
-        target_sampled_actions = child_sampled_actions_batch[:, unroll_step].squeeze(-1)
+        # shape: (batch_size, num_unroll_steps, num_of_sampled_actions, action_dim) -> (batch_size,
+        # num_of_sampled_actions, action_dim) e.g. (4, 6, 20, 2) ->  (4, 20, 2)
+        target_sampled_actions = child_sampled_actions_batch[:, unroll_step]
 
         policy_entropy = dist.entropy().mean()
         policy_entropy_loss = -dist.entropy()
 
         # Project the sampled-based improved policy back onto the space of representable policies. calculate KL
         # loss (batch_size, num_of_sampled_actions) -> (4,20) target_normalized_visit_count is
         # categorical distribution, the range of target_log_prob_sampled_actions is (-inf, 0), add 1e-6 for
@@ -644,17 +647,17 @@
             # way 1:
             # log_prob = dist.log_prob(target_sampled_actions[:, k, :])
 
             # way 2: SAC-like
             y = 1 - target_sampled_actions[:, k, :].pow(2)
 
             # NOTE: for numerical stability.
-            target_sampled_actions_clamped = torch.clamp(
-                target_sampled_actions[:, k, :], torch.tensor(-1 + 1e-6), torch.tensor(1 - 1e-6)
-            )
+            min_val = torch.tensor(-1 + 1e-6).to(target_sampled_actions.device)
+            max_val = torch.tensor(1 - 1e-6).to(target_sampled_actions.device)
+            target_sampled_actions_clamped = torch.clamp(target_sampled_actions[:, k, :], min_val, max_val)
             target_sampled_actions_before_tanh = torch.arctanh(target_sampled_actions_clamped)
 
             # keep dimension for loss computation (usually for action space is 1 env. e.g. pendulum)
             log_prob = dist.log_prob(target_sampled_actions_before_tanh).unsqueeze(-1)
             log_prob = log_prob - torch.log(y + 1e-6).sum(-1, keepdim=True)
             log_prob = log_prob.squeeze(-1)
 
@@ -705,33 +708,34 @@
             - policy_loss (:obj:`torch.Tensor`): The policy loss tensor.
             - policy_entropy (:obj:`torch.Tensor`): The policy entropy tensor.
             - policy_entropy_loss (:obj:`torch.Tensor`): The policy entropy loss tensor.
             - target_policy_entropy (:obj:`torch.Tensor`): The target policy entropy tensor.
             - target_sampled_actions (:obj:`torch.Tensor`): The target sampled actions tensor.
         """
         prob = torch.softmax(policy_logits, dim=-1)
-        dist = Categorical(prob)
 
         # take the init hypothetical step k=unroll_step
         target_normalized_visit_count = target_policy[:, unroll_step]
 
         # Note: The target_policy_entropy is just for debugging.
         target_normalized_visit_count_masked = torch.index_select(
             target_normalized_visit_count, 0,
             torch.nonzero(mask_batch[:, unroll_step]).squeeze(-1)
         )
-        target_dist = Categorical(target_normalized_visit_count_masked)
-        target_policy_entropy = target_dist.entropy().mean()
 
-        # shape: (batch_size, num_unroll_steps, num_of_sampled_actions, action_dim, 1) -> (batch_size,
-        # num_of_sampled_actions, action_dim) e.g. (4, 6, 20, 2, 1) ->  (4, 20, 2)
-        target_sampled_actions = child_sampled_actions_batch[:, unroll_step].squeeze(-1)
+        target_policy_entropy = -((target_normalized_visit_count_masked + 1e-6) * (
+                    target_normalized_visit_count_masked + 1e-6).log()).sum(-1).mean()
 
-        policy_entropy = dist.entropy().mean()
-        policy_entropy_loss = -dist.entropy()
+        # shape: (batch_size, num_unroll_steps, num_of_sampled_actions, action_dim) -> (batch_size,
+        # num_of_sampled_actions, action_dim) e.g. (4, 6, 20, 2) ->  (4, 20, 2)
+        target_sampled_actions = child_sampled_actions_batch[:, unroll_step]
+
+        entropy = -(prob * prob.log()).sum(-1)
+        policy_entropy = entropy.mean()
+        policy_entropy_loss = -entropy
 
         # Project the sampled-based improved policy back onto the space of representable policies. calculate KL
         # loss (batch_size, num_of_sampled_actions) -> (4,20) target_normalized_visit_count is
         # categorical distribution, the range of target_log_prob_sampled_actions is (-inf, 0), add 1e-6 for
         # numerical stability.
         target_log_prob_sampled_actions = torch.log(target_normalized_visit_count + 1e-6)
```

### Comparing `LightZero-0.0.2/lzero/policy/scaling_transform.py` & `LightZero-0.0.5/lzero/policy/scaling_transform.py`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/lzero/policy/stochastic_muzero.py` & `LightZero-0.0.5/lzero/policy/stochastic_muzero.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,22 +67,29 @@
         cuda=True,
         # (int) The number of environments used in collecting data.
         collector_env_num=8,
         # (int) The number of environments used in evaluating policy.
         evaluator_env_num=3,
         # (str) The type of environment. Options is ['not_board_games', 'board_games'].
         env_type='not_board_games',
+        # (str) The type of action space. Options are ['fixed_action_space', 'varied_action_space'].
+        action_type='fixed_action_space',
         # (str) The type of battle mode. Options is ['play_with_bot_mode', 'self_play_mode'].
         battle_mode='play_with_bot_mode',
         # (bool) Whether to monitor extra statistics in tensorboard.
         monitor_extra_statistics=True,
         # (bool) Whether to analyze the chance distribution.
         analyze_chance_distribution=False,
         # (int) The transition number of one ``GameSegment``.
         game_segment_length=200,
+        # (bool): Indicates whether to perform an offline evaluation of the checkpoint (ckpt).
+        # If set to True, the checkpoint will be evaluated after the training process is complete.
+        # IMPORTANT: Setting eval_offline to True requires configuring the saving of checkpoints to align with the evaluation frequency.
+        # This is done by setting the parameter learn.learner.hook.save_ckpt_after_iter to the same value as eval_freq in the train_muzero.py automatically.
+        eval_offline=False,
 
         # ****** observation ******
         # (bool) Whether to transform image to string to save memory.
         transform2string=False,
         # (bool) Whether to use gray scale image.
         gray_scale=False,
         # (bool) Whether to use data augmentation.
@@ -151,14 +158,16 @@
         # (int) The number of final training iterations to control temperature, which is only used for manually decay.
         threshold_training_steps_for_final_temperature=int(1e5),
         # (float) The fixed temperature value for MCTS action selection, which is used to control the exploration.
         # The larger the value, the more exploration. This value is only used when manual_temperature_decay=False.
         fixed_temperature_value=0.25,
         # (bool) Whether to use the true chance in MCTS. If False, use the predicted chance.
         use_ture_chance_label_in_chance_encoder=False,
+        # (bool) Whether to add noise to roots during reanalyze process.
+        reanalyze_noise=False,
 
         # ****** Priority ******
         # (bool) Whether to use priority when sampling training data from the buffer.
         use_priority=True,
         # (bool) Whether to use the maximum priority for new collecting data.
         use_max_priority_for_new_data=True,
         # (float) The degree of prioritization to use. A value of 0 means no prioritization,
@@ -336,15 +345,14 @@
         # transform the scaled value or its categorical representation to its original value,
         # i.e. h^(-1)(.) function in paper https://arxiv.org/pdf/1805.11593.pdf.
         original_value = self.inverse_scalar_transform_handle(value)
 
         # Note: The following lines are just for debugging.
         predicted_rewards = []
         if self._cfg.monitor_extra_statistics:
-            latent_state_list = latent_state.detach().cpu().numpy()
             predicted_values, predicted_policies = original_value.detach().cpu(), torch.softmax(
                 policy_logits, dim=1
             ).detach().cpu()
 
         # calculate the new priorities for each transition.
         value_priority = L1Loss(reduction='none')(original_value.squeeze(-1), target_value[:, 0])
         value_priority = value_priority.data.cpu().numpy() + 1e-6
@@ -463,15 +471,14 @@
                 original_rewards_cpu = original_rewards.detach().cpu()
 
                 predicted_values = torch.cat(
                     (predicted_values, self.inverse_scalar_transform_handle(value).detach().cpu())
                 )
                 predicted_rewards.append(original_rewards_cpu)
                 predicted_policies = torch.cat((predicted_policies, torch.softmax(policy_logits, dim=1).detach().cpu()))
-                latent_state_list = np.concatenate((latent_state_list, latent_state.detach().cpu().numpy()))
 
         # ==============================================================
         # the core learn model update step.
         # ==============================================================
         # weighted loss with masks (some invalid states which are out of trajectory.)
         loss = (
             self._cfg.ssl_loss_weight * consistency_loss + self._cfg.policy_loss_weight * policy_loss +
@@ -511,53 +518,50 @@
         )
         if self._cfg.monitor_extra_statistics:
             predicted_rewards = torch.stack(predicted_rewards).transpose(1, 0).squeeze(-1)
             predicted_rewards = predicted_rewards.reshape(-1).unsqueeze(-1)
 
             td_data = (
                 value_priority,
-                target_reward.detach().cpu().numpy(),
-                target_value.detach().cpu().numpy(),
-                transformed_target_reward.detach().cpu().numpy(),
-                transformed_target_value.detach().cpu().numpy(),
-                target_reward_categorical.detach().cpu().numpy(),
-                target_value_categorical.detach().cpu().numpy(),
-                predicted_rewards.detach().cpu().numpy(),
-                predicted_values.detach().cpu().numpy(),
-                target_policy.detach().cpu().numpy(),
-                predicted_policies.detach().cpu().numpy(),
-                latent_state_list,
+                target_reward,
+                target_value,
+                transformed_target_reward,
+                transformed_target_value,
+                target_reward_categorical,
+                target_value_categorical,
+                predicted_rewards,
+                predicted_values,
+                target_policy,
+                predicted_policies,
             )
 
         return {
             'collect_mcts_temperature': self._collect_mcts_temperature,
             'cur_lr': self._optimizer.param_groups[0]['lr'],
             'weighted_total_loss': loss_info[0],
             'total_loss': loss_info[1],
             'policy_loss': loss_info[2],
             'reward_loss': loss_info[3],
             'value_loss': loss_info[4],
             'consistency_loss': loss_info[5] / self._cfg.num_unroll_steps,
             'afterstate_policy_loss': loss_info[6],
             'afterstate_value_loss': loss_info[7],
             'commitment_loss': loss_info[8],
-
+            'target_reward': td_data[1].mean().item(),
+            'target_value': td_data[2].mean().item(),
+            'transformed_target_reward': td_data[3].mean().item(),
+            'transformed_target_value': td_data[4].mean().item(),
+            'predicted_rewards': td_data[7].mean().item(),
+            'predicted_values': td_data[8].mean().item(),
+            'total_grad_norm_before_clip': total_grad_norm_before_clip,
             # ==============================================================
             # priority related
             # ==============================================================
             'value_priority_orig': value_priority,
-            'value_priority': td_data[0].flatten().mean().item(),
-            
-            'target_reward': td_data[1].flatten().mean().item(),
-            'target_value': td_data[2].flatten().mean().item(),
-            'transformed_target_reward': td_data[3].flatten().mean().item(),
-            'transformed_target_value': td_data[4].flatten().mean().item(),
-            'predicted_rewards': td_data[7].flatten().mean().item(),
-            'predicted_values': td_data[8].flatten().mean().item(),
-            'total_grad_norm_before_clip': total_grad_norm_before_clip
+            'value_priority': td_data[0].mean().item(),
         }
 
     def _init_collect(self) -> None:
         """
         Overview:
             Collect mode init method. Called by ``self.__init__``. Initialize the collect model and MCTS utils.
         """
```

### Comparing `LightZero-0.0.2/lzero/policy/tests/config/atari_muzero_config_for_test.py` & `LightZero-0.0.5/lzero/policy/tests/config/atari_muzero_config_for_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 from easydict import EasyDict
 
-env_name = 'PongNoFrameskip-v4'
+env_id = 'PongNoFrameskip-v4'
 
-if env_name == 'PongNoFrameskip-v4':
+if env_id == 'PongNoFrameskip-v4':
     action_space_size = 6
-elif env_name == 'QbertNoFrameskip-v4':
+elif env_id == 'QbertNoFrameskip-v4':
     action_space_size = 6
-elif env_name == 'MsPacmanNoFrameskip-v4':
+elif env_id == 'MsPacmanNoFrameskip-v4':
     action_space_size = 9
-elif env_name == 'SpaceInvadersNoFrameskip-v4':
+elif env_id == 'SpaceInvadersNoFrameskip-v4':
     action_space_size = 6
-elif env_name == 'BreakoutNoFrameskip-v4':
+elif env_id == 'BreakoutNoFrameskip-v4':
     action_space_size = 4
 
 # ==============================================================
 # begin of the most frequently changed config specified by the user
 # ==============================================================
 collector_env_num = 8
 n_episode = 8
 evaluator_env_num = 3
 num_simulations = 50
 update_per_collect = 1000
 batch_size = 256
 max_env_step = int(1e6)
-reanalyze_ratio = 0.
+reanalyze_ratio = 0.1
 eps_greedy_exploration_in_collect = False
 # ==============================================================
 # end of the most frequently changed config specified by the user
 # ==============================================================
 
 atari_muzero_config = dict(
     exp_name=
-    f'data_mz_ctree/{env_name[:-14]}_muzero_ns{num_simulations}_upc{update_per_collect}_rr{reanalyze_ratio}_seed0',
+    f'data_mz_ctree/{env_id[:-14]}_muzero_ns{num_simulations}_upc{update_per_collect}_rr{reanalyze_ratio}_seed0',
     env=dict(
         stop_value=int(1e6),
-        env_name=env_name,
+        env_id=env_id,
         obs_shape=(4, 96, 96),
         collector_env_num=collector_env_num,
         evaluator_env_num=evaluator_env_num,
         n_evaluator_episode=evaluator_env_num,
         manager=dict(shared_memory=False, ),
     ),
     policy=dict(
```

### Comparing `LightZero-0.0.2/lzero/policy/tests/config/cartpole_muzero_config_for_test.py` & `LightZero-0.0.5/lzero/policy/tests/config/cartpole_muzero_config_for_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # ==============================================================
 # end of the most frequently changed config specified by the user
 # ==============================================================
 
 cartpole_muzero_config = dict(
     exp_name=f'data_mz_ctree/cartpole_muzero_ns{num_simulations}_upc{update_per_collect}_rr{reanalyze_ratio}_seed0',
     env=dict(
-        env_name='CartPole-v0',
+        env_id='CartPole-v0',
         continuous=False,
         manually_discretization=False,
         collector_env_num=collector_env_num,
         evaluator_env_num=evaluator_env_num,
         n_evaluator_episode=evaluator_env_num,
         manager=dict(shared_memory=False, ),
     ),
```

### Comparing `LightZero-0.0.2/lzero/policy/tests/test_get_target_obs_index_in_step_k.py` & `LightZero-0.0.5/lzero/policy/tests/test_get_target_obs_index_in_step_k.py`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/lzero/policy/tests/test_scaling_transform.py` & `LightZero-0.0.5/lzero/policy/tests/test_scaling_transform.py`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/lzero/policy/tests/test_utils.py` & `LightZero-0.0.5/lzero/policy/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/lzero/policy/utils.py` & `LightZero-0.0.5/lzero/policy/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -286,14 +286,60 @@
 
     return optimizer
 
 
 def prepare_obs(obs_batch_ori: np.ndarray, cfg: EasyDict) -> Tuple[torch.Tensor, torch.Tensor]:
     """
     Overview:
+        Prepare the observations for the model by converting the original batch of observations
+        to a PyTorch tensor, and then slicing it to create the batches used for the initial inference
+        and for calculating the consistency loss if required.
+
+    Arguments:
+        - obs_batch_ori (:obj:`np.ndarray`): The original observations in a batch style.
+        - cfg (:obj:`EasyDict`): The configuration dictionary containing model settings.
+
+    Returns:
+        - obs_batch (:obj:`torch.Tensor`): The tensor containing the observations for the initial inference.
+        - obs_target_batch (:obj:`torch.Tensor`): The tensor containing the observations for calculating
+                                                   the consistency loss, if applicable.
+    """
+    # Convert the numpy array of original observations to a PyTorch tensor and transfer it to the specified device.
+    # Also, ensure the tensor is of the correct floating-point type for the model.
+    # obs_batch_ori = torch.from_numpy(obs_batch_ori).to(cfg.device).float()
+    obs_batch_ori = torch.from_numpy(obs_batch_ori).to(cfg.device)
+
+    # Calculate the dimension size to slice based on the model configuration.
+    # For convolutional models ('conv'), use the number of frames to stack times the number of channels.
+    # For multi-layer perceptron models ('mlp'), use the number of frames to stack times the size of the observation space.
+    stack_dim = cfg.model.frame_stack_num * (
+        cfg.model.image_channel if cfg.model.model_type == 'conv' else cfg.model.observation_shape)
+
+    # Slice the original observation tensor to obtain the batch for the initial inference.
+    obs_batch = obs_batch_ori[:, :stack_dim]
+
+    # Initialize the target batch for consistency loss as `None`. It will only be set if consistency loss calculation is enabled.
+    obs_target_batch = None
+    # If the model configuration specifies the use of self-supervised learning loss, prepare the target batch for the consistency loss.
+    if cfg.model.self_supervised_learning_loss:
+        # Determine the starting dimension to exclude based on the model type.
+        # For 'conv', exclude the first 'image_channel' dimensions.
+        # For 'mlp', exclude the first 'observation_shape' dimensions.
+        exclude_dim = cfg.model.image_channel if cfg.model.model_type == 'conv' else cfg.model.observation_shape
+
+        # Slice the original observation tensor to obtain the batch for consistency loss calculation.
+        obs_target_batch = obs_batch_ori[:, exclude_dim:]
+
+    # Return the prepared batches: one for the initial inference and one for the consistency loss calculation (if applicable).
+    return obs_batch, obs_target_batch
+
+
+def prepare_obs_bkp(obs_batch_ori: np.ndarray, cfg: EasyDict) -> Tuple[torch.Tensor, torch.Tensor]:
+    """
+    Overview:
         Prepare the observations for the model, including:
         1. convert the obs to torch tensor
         2. stack the obs
         3. calculate the consistency loss
     Arguments:
         - obs_batch_ori (:obj:`np.ndarray`): the original observations in a batch style
         - cfg (:obj:`EasyDict`): the config dict
@@ -302,27 +348,28 @@
         - obs_target_batch (:obj:`torch.Tensor`): the stacked observations for calculating consistency loss
     """
     obs_target_batch = None
     if cfg.model.model_type == 'conv':
         # for 3-dimensional image obs
         """
         ``obs_batch_ori`` is the original observations in a batch style, shape is:
-        (batch_size, stack_num+num_unroll_steps, W, H, C) -> (batch_size, (stack_num+num_unroll_steps)*C, W, H )
+        (batch_size, stack_num+num_unroll_steps, C, W, H) -> (batch_size, (stack_num+num_unroll_steps)*C, W, H )
 
         e.g. in pong: stack_num=4, num_unroll_steps=5
-        (4, 9, 96, 96, 3) -> (4, 9*3, 96, 96) = (4, 27, 96, 96)
+        (4, (4+5), 3, 96, 96) -> (4, 9, 3, 96, 96) -> (4, 9*3, 96, 96) = (4, 27, 96, 96)
 
         the second dim of ``obs_batch_ori``:
         timestep t:     1,   2,   3,  4,    5,   6,   7,   8,     9
         channel_num:    3    3    3   3     3    3    3    3      3
                        ---, ---, ---, ---,  ---, ---, ---, ---,   ---
         """
-        obs_batch_ori = torch.from_numpy(obs_batch_ori).to(cfg.device).float()
+        # obs_batch_ori = torch.from_numpy(obs_batch_ori).to(cfg.device).float()
+        obs_batch_ori = torch.from_numpy(obs_batch_ori).to(cfg.device)
         # ``obs_batch`` is used in ``initial_inference()``, which is the first stacked obs at timestep t in
-        # ``obs_batch_ori``. shape is (4, 4*3, 96, 96) = (4, 12, 96, 96)
+        # ``obs_batch_ori``. shape is (4, (4+5)*1, 96, 96) = (4, 9, 96, 96)
         obs_batch = obs_batch_ori[:, 0:cfg.model.frame_stack_num * cfg.model.image_channel, :, :]
 
         if cfg.model.self_supervised_learning_loss:
             # ``obs_target_batch`` is only used for calculate consistency loss, which take the all obs other than
             # timestep t1, and is only performed in the last 8 timesteps in the second dim in ``obs_batch_ori``.
             obs_target_batch = obs_batch_ori[:, cfg.model.image_channel:, :, :]
     elif cfg.model.model_type == 'mlp':
```

### Comparing `LightZero-0.0.2/lzero/worker/alphazero_collector.py` & `LightZero-0.0.5/lzero/worker/alphazero_collector.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from collections import namedtuple
-from typing import Optional, Any, List, Dict
+from typing import Optional, Any, List
 
 import numpy as np
 from ding.envs import BaseEnvManager
 from ding.torch_utils import to_ndarray
-from ding.utils import build_logger, EasyTimer, SERIAL_COLLECTOR_REGISTRY, one_time_warning, get_rank, get_world_size, \
-    broadcast_object_list, allreduce_data
+from ding.utils import build_logger, EasyTimer, SERIAL_COLLECTOR_REGISTRY, get_rank, get_world_size, \
+    allreduce_data
 from ding.worker.collector.base_serial_collector import ISerialCollector, CachePool, TrajBuffer, INF, \
     to_tensor_transitions
 
 
 @SERIAL_COLLECTOR_REGISTRY.register('episode_alphazero')
 class AlphaZeroCollector(ISerialCollector):
     """
     Overview:
-        AlphaZero collector (n_episode).
+        AlphaZero collector for collecting episodes of experience during self-play or playing against an opponent.
+        This collector is specifically designed for the AlphaZero algorithm.
     Interfaces:
-        __init__, reset, reset_env, reset_policy, collect, close
+        ``__init__``, ``reset``, ``reset_env``, ``reset_policy``, ``collect``, ``close``
     Property:
         envstep
     """
 
     # TO be compatible with ISerialCollector
     config = dict()
 
@@ -31,26 +32,25 @@
             policy: namedtuple = None,
             tb_logger: 'SummaryWriter' = None,  # noqa
             exp_name: Optional[str] = 'default_experiment',
             instance_name: Optional[str] = 'collector',
             env_config=None,
     ) -> None:
         """
-            Overview:
-                Init the AlphaZero collector according to input arguments.
-            Arguments:
-                - collect_print_freq (:obj:`int`): collect_print_frequency in terms of training_steps.
-                - env (:obj:`BaseEnvManager`): The env for the collection, the BaseEnvManager object or \
-                    its derivatives are supported.
-                - policy (:obj:`Policy`): The policy to be collected.
-                - tb_logger (:obj:`SummaryWriter`): Logger, defaultly set as 'SummaryWriter' for model summary.
-                - instance_name (:obj:`Optional[str]`): Name of this instance.
-                - exp_name (:obj:`str`): Experiment name, which is used to indicate output directory.
-                - env_config: Config of environment
-            """
+        Overview:
+            Initialize the AlphaZero collector with the provided environment, policy, and configurations.
+        Arguments:
+            - collect_print_freq (:obj:`int`): Frequency of printing collection statistics (in training steps).
+            - env (:obj:`Optional[BaseEnvManager]`): Environment manager for managing multiple environments.
+            - policy (:obj:`Optional[namedtuple]`): Policy used for making decisions during collection.
+            - tb_logger (:obj:`Optional[SummaryWriter]`): TensorBoard logger for logging statistics.
+            - exp_name (:obj:`str`): Name of the experiment for logging purposes.
+            - instance_name (:obj:`str`): Unique identifier for this collector instance.
+            - env_config (:obj:`Optional[dict]`): Configuration for the environment.
+        """
         self._exp_name = exp_name
         self._instance_name = instance_name
         self._collect_print_freq = collect_print_freq
         self._timer = EasyTimer()
         self._end_flag = False
         self._env_config = env_config
 
@@ -75,37 +75,36 @@
             self._tb_logger = None
 
         self.reset(policy, env)
 
     def reset_env(self, _env: Optional[BaseEnvManager] = None) -> None:
         """
         Overview:
-            Reset the environment.
+            Reset or replace the environment in the collector.
             If _env is None, reset the old environment.
             If _env is not None, replace the old environment in the collector with the new passed \
                 in environment and launch.
         Arguments:
-            - env (:obj:`Optional[BaseEnvManager]`): instance of the subclass of vectorized \
-                env_manager(BaseEnvManager)
+            - _env (:obj:`Optional[BaseEnvManager]`): New environment to replace the existing one, if provided.
         """
         if _env is not None:
             self._env = _env
             self._env.launch()
             self._env_num = self._env.env_num
         else:
             self._env.reset()
 
     def reset_policy(self, _policy: Optional[namedtuple] = None) -> None:
         """
         Overview:
-            Reset the policy.
+            Reset or replace the policy in the collector.
             If _policy is None, reset the old policy.
             If _policy is not None, replace the old policy in the collector with the new passed in policy.
         Arguments:
-            - policy (:obj:`Optional[namedtuple]`): the api namedtuple of collect_mode policy
+            - _policy (:obj:`Optional[namedtuple]`): New policy to replace the existing one, if provided.
         """
         assert hasattr(self, '_env'), "please set env first"
         if _policy is not None:
             self._policy = _policy
             self._default_n_episode = _policy.get_attribute('cfg').get('n_episode', None)
             self._on_policy = _policy.get_attribute('cfg').on_policy
             self._traj_len = INF
@@ -115,24 +114,23 @@
                 )
             )
         self._policy.reset()
 
     def reset(self, _policy: Optional[namedtuple] = None, _env: Optional[BaseEnvManager] = None) -> None:
         """
         Overview:
-            Reset the environment and policy.
+            Reset the environment and policy within the collector.
             If _env is None, reset the old environment.
             If _env is not None, replace the old environment in the collector with the new passed \
                 in environment and launch.
             If _policy is None, reset the old policy.
             If _policy is not None, replace the old policy in the collector with the new passed in policy.
         Arguments:
-            - policy (:obj:`Optional[namedtuple]`): the api namedtuple of collect_mode policy
-            - env (:obj:`Optional[BaseEnvManager]`): instance of the subclass of vectorized \
-                env_manager(BaseEnvManager)
+            - _policy (:obj:`Optional[namedtuple]`): New policy to replace the existing one, if provided.
+            - _env (:obj:`Optional[BaseEnvManager]`): New environment to replace the existing one, if provided.
         """
         if _env is not None:
             self.reset_env(_env)
         if _policy is not None:
             self.reset_policy(_policy)
 
         self._obs_pool = CachePool('obs', self._env_num, deepcopy=False)
@@ -147,30 +145,31 @@
         self._total_duration = 0
         self._last_train_iter = 0
         self._end_flag = False
 
     def _reset_stat(self, env_id: int) -> None:
         """
         Overview:
-            Reset the collector's state. Including reset the traj_buffer, obs_pool, policy_output_pool\
-                and env_info. Reset these states according to env_id. You can refer to base_serial_collector\
-                to get more messages.
+            Reset the statistics for a specific environment.
+            Including reset the traj_buffer, obs_pool, policy_output_pool and env_info.
+            Reset these states according to env_id.
+            You can refer to base_serial_collector to get more messages.
         Arguments:
             - env_id (:obj:`int`): the id where we need to reset the collector's state
         """
         self._traj_buffer[env_id].clear()
         self._obs_pool.reset(env_id)
         self._policy_output_pool.reset(env_id)
         self._env_info[env_id] = {'time': 0., 'step': 0}
 
     def close(self) -> None:
         """
         Overview:
-            Close the collector. If end_flag is False, close the environment, flush the tb_logger\
-                and close the tb_logger.
+            Close the collector. If end_flag is False, close the environment, flush the tb_logger
+            and close the tb_logger.
         """
         if self._end_flag:
             return
         self._end_flag = True
         self._env.close()
         if self._tb_logger:
             self._tb_logger.flush()
@@ -178,21 +177,21 @@
 
     def collect(self,
                 n_episode: Optional[int] = None,
                 train_iter: int = 0,
                 policy_kwargs: Optional[dict] = None) -> List[Any]:
         """
         Overview:
-            Collect `n_episode` data with policy_kwargs, which is already trained `train_iter` iterations
+            Collect experience data for a specified number of episodes using the current policy.
         Arguments:
-            - n_episode (:obj:`int`): the number of collecting data episode
-            - train_iter (:obj:`int`): the number of training iteration
-            - policy_kwargs (:obj:`dict`): the keyword args for policy forward
+            - n_episode (:obj:`Optional[int]`): Number of episodes to collect. Defaults to a pre-set value if None.
+            - train_iter (:obj:`int`): Current training iteration.
+            - policy_kwargs (:obj:`Optional[dict]`): Additional keyword arguments for the policy.
         Returns:
-            - return_data (:obj:`List`): A list containing collected episodes.
+            - return_data (:obj:`List[Any]`): A list of collected experience episodes.
         """
         if n_episode is None:
             if self._default_n_episode is None:
                 raise RuntimeError("Please specify collect n_episode")
             else:
                 n_episode = self._default_n_episode
         assert n_episode >= self._env_num, "Please make sure n_episode >= env_num{}/{}".format(n_episode, self._env_num)
@@ -256,15 +255,14 @@
                         transitions = self.reward_shaping(transitions, timestep.info['eval_episode_return'])
 
                         return_data.append(transitions)
                         self._traj_buffer[env_id].clear()
 
                 self._env_info[env_id]['time'] += self._timer.value + interaction_duration
                 if timestep.done:
-                    self._total_episode_count += 1
                     # the eval_episode_return is calculated from Player 1's perspective
                     reward = timestep.info['eval_episode_return']
                     info = {
                         'reward': reward,  # only means player1 reward
                         'time': self._env_info[env_id]['time'],
                         'step': self._env_info[env_id]['step'],
                     }
@@ -291,49 +289,46 @@
         self._output_log(train_iter)
         return return_data
 
     @property
     def envstep(self) -> int:
         """
         Overview:
-            Print the total envstep count.
-        Return:
-            - envstep (:obj:`int`): the total envstep count
+            Get the total number of environment steps taken by the collector.
+        Returns:
+            - envstep (:obj:`int`): Total count of environment steps.
         """
         return self._total_envstep_count
 
     def close(self) -> None:
         """
         Overview:
-            Close the collector. If end_flag is False, close the environment, flush the tb_logger\
-                and close the tb_logger.
+            Close the collector and clean up resources such as environment and logger.
         """
         if self._end_flag:
             return
         self._end_flag = True
         self._env.close()
         if self._tb_logger:
             self._tb_logger.flush()
             self._tb_logger.close()
 
     def __del__(self) -> None:
         """
         Overview:
-            Execute the close command and close the collector. __del__ is automatically called to \
-                destroy the collector instance when the collector finishes its work
+            Destructor method that is called when the collector object is being destroyed.
         """
         self.close()
 
     def _output_log(self, train_iter: int) -> None:
         """
         Overview:
-            Print the output log information. You can refer to Docs/Best Practice/How to understand\
-             training generated folders/Serial mode/log/collector for more details.
+            Output logging information for the current collection phase.
         Arguments:
-            - train_iter (:obj:`int`): the number of training iteration.
+            - train_iter (:obj:`int`): Current training iteration for logging purposes.
         """
         if self._rank != 0:
             return
         if (train_iter - self._last_train_iter) >= self._collect_print_freq and len(self._episode_info) > 0:
             self._last_train_iter = train_iter
             episode_count = len(self._episode_info)
             envstep_count = sum([d['step'] for d in self._episode_info])
@@ -364,17 +359,17 @@
                 if k in ['total_envstep_count']:
                     continue
                 self._tb_logger.add_scalar('{}_step/'.format(self._instance_name) + k, v, self._total_envstep_count)
 
     def reward_shaping(self, transitions, eval_episode_return):
         """
         Overview:
-            Shape the reward according to the player.
+            Shape the rewards in the collected transitions based on the outcome of the episode.
         Return:
-            - transitions: data transitions.
+            - transitions (:obj:`List[dict]`): List of data transitions.
         """
         reward = transitions[-1]['reward']
         to_play = transitions[-1]['obs']['to_play']
         for t in transitions:
             if t['obs']['to_play'] == -1:
                 # play_with_bot_mode
                 # the eval_episode_return is calculated from Player 1's perspective
```

### Comparing `LightZero-0.0.2/lzero/worker/alphazero_evaluator.py` & `LightZero-0.0.5/lzero/worker/alphazero_evaluator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from collections import namedtuple
 from typing import Optional, Callable, Tuple
-import torch
+
 import numpy as np
+import torch
 from ding.envs import BaseEnv
 from ding.envs import BaseEnvManager
 from ding.torch_utils import to_tensor, to_item
-
 from ding.utils import build_logger, EasyTimer, SERIAL_EVALUATOR_REGISTRY
 from ding.utils import get_world_size, get_rank, broadcast_object_list
 from ding.worker.collector.base_serial_evaluator import ISerialEvaluator, VectorEvalMonitor
 
 
 @SERIAL_EVALUATOR_REGISTRY.register('alphazero')
 class AlphaZeroEvaluator(ISerialEvaluator):
     """
     Overview:
-        AlphaZero Evaluator.
+        AlphaZero Evaluator class which handles the evaluation of the trained policy.
     Interfaces:
-        __init__, reset, reset_policy, reset_env, close, should_eval, eval
+        ``__init__``, ``reset``, ``reset_policy``, ``reset_env``, ``close``, ``should_eval``, ``eval``
     Property:
         env, policy
     """
 
     def __init__(
             self,
             eval_freq: int = 1000,
@@ -32,25 +32,25 @@
             tb_logger: 'SummaryWriter' = None,  # noqa
             exp_name: Optional[str] = 'default_experiment',
             instance_name: Optional[str] = 'evaluator',
             env_config=None,
     ) -> None:
         """
         Overview:
-            Init the AlphaZero evaluator according to input arguments.
+            Initialize the AlphaZero evaluator with the given parameters.
         Arguments:
-            - eval_freq (:obj:`int`): evaluation frequency in terms of training steps.
-            - n_evaluator_episode (:obj:`int`): the number of episodes to eval in total.
-            - env (:obj:`BaseEnvManager`): The env for the collection, the BaseEnvManager object or \
-                its derivatives are supported.
-            - policy (:obj:`Policy`): The policy to be collected.
-            - tb_logger (:obj:`SummaryWriter`): Logger, defaultly set as 'SummaryWriter' for model summary.
-            - exp_name (:obj:`str`): Experiment name, which is used to indicate output directory.
-            - instance_name (:obj:`Optional[str]`): Name of this instance.
-            - env_config: Config of environment
+            - eval_freq (:obj:`int`): Evaluation frequency in terms of training steps.
+            - n_evaluator_episode (:obj:`int`): Number of episodes for each evaluation.
+            - stop_value (:obj:`float`): Reward threshold to stop training if surpassed.
+            - env (:obj:`Optional[BaseEnvManager]`): Environment manager for managing multiple environments.
+            - policy (:obj:`Optional[namedtuple]`): Policy to be evaluated.
+            - tb_logger (:obj:`Optional[SummaryWriter]`): TensorBoard logger for logging statistics.
+            - exp_name (:obj:`str`): Name of the experiment for logging purposes.
+            - instance_name (:obj:`str`): Unique identifier for this evaluator instance.
+            - env_config (:obj:`Optional[dict]`): Configuration for the environment.
         """
         self._eval_freq = eval_freq
         self._exp_name = exp_name
         self._instance_name = instance_name
         self._end_flag = False
         self._env_config = env_config
 
@@ -74,96 +74,92 @@
         self._timer = EasyTimer()
         self._default_n_episode = n_evaluator_episode
         self._stop_value = stop_value
 
     def reset_env(self, _env: Optional[BaseEnvManager] = None) -> None:
         """
         Overview:
-            Reset evaluator's environment. In some case, we need evaluator use the same policy in different \
-                environments. We can use reset_env to reset the environment.
+            Reset or replace the environment in the evaluator.
             If _env is None, reset the old environment.
             If _env is not None, replace the old environment in the evaluator with the \
                 new passed in environment and launch.
         Arguments:
-            - env (:obj:`Optional[BaseEnvManager]`): instance of the subclass of vectorized \
-                env_manager(BaseEnvManager)
+            - _env (:obj:`Optional[BaseEnvManager]`): New environment to replace the existing one, if provided.
         """
         if _env is not None:
             self._env = _env
             self._env.launch()
             self._env_num = self._env.env_num
         else:
             self._env.reset()
 
     def reset_policy(self, _policy: Optional[namedtuple] = None) -> None:
         """
         Overview:
-            Reset evaluator's policy. In some case, we need evaluator work in this same environment but use\
-                different policy. We can use reset_policy to reset the policy.
+            Reset or replace the policy in the evaluator.
             If _policy is None, reset the old policy.
             If _policy is not None, replace the old policy in the evaluator with the new passed in policy.
         Arguments:
             - policy (:obj:`Optional[namedtuple]`): the api namedtuple of eval_mode policy
         """
         assert hasattr(self, '_env'), "please set env first"
         if _policy is not None:
             self._policy = _policy
         self._policy.reset()
 
     def reset(self, _policy: Optional[namedtuple] = None, _env: Optional[BaseEnvManager] = None) -> None:
         """
         Overview:
-            Reset evaluator's policy and environment. Use new policy and environment to collect data.
+            Reset the environment and policy within the evaluator.
             If _env is None, reset the old environment.
             If _env is not None, replace the old environment in the evaluator with the new passed in \
                 environment and launch.
             If _policy is None, reset the old policy.
             If _policy is not None, replace the old policy in the evaluator with the new passed in policy.
         Arguments:
-            - policy (:obj:`Optional[namedtuple]`): the api namedtuple of eval_mode policy
-            - env (:obj:`Optional[BaseEnvManager]`): instance of the subclass of vectorized \
-                env_manager(BaseEnvManager)
+            - _policy (:obj:`Optional[namedtuple]`): New policy to replace the existing one, if provided.
+            - _env (:obj:`Optional[BaseEnvManager]`): New environment to replace the existing one, if provided.
         """
         if _env is not None:
             self.reset_env(_env)
         if _policy is not None:
             self.reset_policy(_policy)
         self._max_eval_reward = float("-inf")
         self._last_eval_iter = -1
         self._end_flag = False
 
     def close(self) -> None:
         """
         Overview:
-            Close the evaluator. If end_flag is False, close the environment, flush the tb_logger\
-                and close the tb_logger.
+            Close the evaluator and clean up resources such as environment and logger.
+            If end_flag is False, close the environment, flush the tb_logger and close the tb_logger.
         """
         if self._end_flag:
             return
         self._end_flag = True
         self._env.close()
         if self._tb_logger:
             self._tb_logger.flush()
             self._tb_logger.close()
 
     def __del__(self) -> None:
         """
         Overview:
-            Execute the close command and close the evaluator. __del__ is automatically called \
-                to destroy the evaluator instance when the evaluator finishes its work
+            Destructor method that is called when the evaluator object is being destroyed.
+             __del__ is automatically called to destroy the evaluator instance when the evaluator finishes its work.
         """
         self.close()
 
     def should_eval(self, train_iter: int) -> bool:
         """
         Overview:
-            Determine whether you need to start the evaluation mode, if the number of training has reached\
-                the maximum number of times to start the evaluator, return True
-        Arguments:
-            - train_iter (:obj:`int`): Current training iteration.
+            Check if it is time to evaluate the policy based on the training iteration count.
+            If the amount of training has reached the maximum number of times to start the evaluator, return True.
+        Returns:
+            - (:obj:`bool`): Flag indicating whether evaluation should be performed.
         """
         if train_iter == self._last_eval_iter:
             return False
         if (train_iter - self._last_eval_iter) < self._eval_freq and train_iter != 0:
             return False
         self._last_eval_iter = train_iter
         return True
@@ -174,25 +170,26 @@
             train_iter: int = -1,
             envstep: int = -1,
             n_episode: Optional[int] = None,
             force_render: bool = False,
     ) -> Tuple[bool, dict]:
         """
         Overview:
-            Evaluate policy and store the best policy based on whether it reaches the highest historical reward.
+            Execute the evaluation of the policy and determine if the stopping condition has been met.
         Arguments:
-            - save_ckpt_fn (:obj:`Callable`): Saving ckpt function, which will be triggered by getting the best reward.
-            - train_iter (:obj:`int`): Current training iteration.
-            - envstep (:obj:`int`): Current env interaction step.
-            - n_episode (:obj:`int`): Number of evaluation episodes.
+            - save_ckpt_fn (:obj:`Optional[Callable]`): Callback function to save a checkpoint.
+            - train_iter (:obj:`int`): Current number of training iterations completed.
+            - envstep (:obj:`int`): Current number of environment steps completed.
+            - n_episode (:obj:`Optional[int]`): Number of episodes to evaluate. Defaults to preset if None.
+            - force_render (:obj:`bool`): Force rendering of the environment, if applicable.
         Returns:
-            - stop_flag (:obj:`bool`): Whether this training program can be ended.
-            - return_info (:obj:`dict`): Current evaluation return information.
+            - stop_flag (:obj:`bool`): Whether the training process should stop based on evaluation results.
+            - return_info (:obj:`dict`): Information about the evaluation results.
         """
-        # evaluator only work on rank0
+        # the evaluator only works on rank0
         stop_flag, return_info = False, []
         if get_rank() == 0:
             if n_episode is None:
                 n_episode = self._default_n_episode
             assert n_episode is not None, "please indicate eval n_episode"
             envstep_count = 0
             eval_monitor = VectorEvalMonitor(self._env.env_num, n_episode)
```

### Comparing `LightZero-0.0.2/lzero/worker/muzero_collector.py` & `LightZero-0.0.5/lzero/worker/muzero_collector.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,32 +2,34 @@
 from collections import deque, namedtuple
 from typing import Optional, Any, List
 
 import numpy as np
 import torch
 from ding.envs import BaseEnvManager
 from ding.torch_utils import to_ndarray
-from ding.utils import build_logger, EasyTimer, SERIAL_COLLECTOR_REGISTRY, one_time_warning, get_rank, get_world_size, \
-    broadcast_object_list, allreduce_data
+from ding.utils import build_logger, EasyTimer, SERIAL_COLLECTOR_REGISTRY, get_rank, get_world_size, \
+    allreduce_data
 from ding.worker.collector.base_serial_collector import ISerialCollector
 from torch.nn import L1Loss
 
 from lzero.mcts.buffer.game_segment import GameSegment
 from lzero.mcts.utils import prepare_observation
 
 
 @SERIAL_COLLECTOR_REGISTRY.register('episode_muzero')
 class MuZeroCollector(ISerialCollector):
     """
     Overview:
         The Collector for MCTS+RL algorithms, including MuZero, EfficientZero, Sampled EfficientZero, Gumbel MuZero.
+        It manages the data collection process for training these algorithms using a serial mechanism.
     Interfaces:
-        __init__, reset, reset_env, reset_policy, _reset_stat, envstep, __del__, _compute_priorities, pad_and_save_last_trajectory, collect, _output_log, close
-    Property:
-        envstep
+        ``__init__``, ``reset``, ``reset_env``, ``reset_policy``, ``_reset_stat``, ``envstep``, ``__del__``, ``_compute_priorities``,
+        ``pad_and_save_last_trajectory``, ``collect``, ``_output_log``, ``close``
+    Properties:
+        ``envstep``
     """
 
     # TO be compatible with ISerialCollector
     config = dict()
 
     def __init__(
             self,
@@ -37,23 +39,23 @@
             tb_logger: 'SummaryWriter' = None,  # noqa
             exp_name: Optional[str] = 'default_experiment',
             instance_name: Optional[str] = 'collector',
             policy_config: 'policy_config' = None,  # noqa
     ) -> None:
         """
         Overview:
-            Init the collector according to input arguments.
+            Initialize the MuZeroCollector with the given parameters.
         Arguments:
-            - collect_print_freq (:obj:`int`): collect_print_frequency in terms of training_steps.
-            - env (:obj:`BaseEnvManager`): the subclass of vectorized env_manager(BaseEnvManager)
-            - policy (:obj:`namedtuple`): the api namedtuple of collect_mode policy
-            - tb_logger (:obj:`SummaryWriter`): tensorboard handle
-            - instance_name (:obj:`Optional[str]`): Name of this instance.
-            - exp_name (:obj:`str`): Experiment name, which is used to indicate output directory.
-            - policy_config: Config of game.
+            - collect_print_freq (:obj:`int`): Frequency (in training steps) at which to print collection information.
+            - env (:obj:`Optional[BaseEnvManager]`): Instance of the subclass of vectorized environment manager.
+            - policy (:obj:`Optional[namedtuple]`): namedtuple of the collection mode policy API.
+            - tb_logger (:obj:`Optional[SummaryWriter]`): TensorBoard logger instance.
+            - exp_name (:obj:`str`): Name of the experiment, used for logging and saving purposes.
+            - instance_name (:obj:`str`): Unique identifier for this collector instance.
+            - policy_config (:obj:`Optional[policy_config]`): Configuration object for the policy.
         """
         self._exp_name = exp_name
         self._instance_name = instance_name
         self._collect_print_freq = collect_print_freq
         self._timer = EasyTimer()
         self._end_flag = False
 
@@ -80,33 +82,32 @@
         self.policy_config = policy_config
 
         self.reset(policy, env)
 
     def reset_env(self, _env: Optional[BaseEnvManager] = None) -> None:
         """
         Overview:
-            Reset the environment.
+            Reset or replace the environment managed by this collector.
             If _env is None, reset the old environment.
             If _env is not None, replace the old environment in the collector with the new passed \
                 in environment and launch.
         Arguments:
-            - env (:obj:`Optional[BaseEnvManager]`): instance of the subclass of vectorized \
-                env_manager(BaseEnvManager)
+            - env (:obj:`Optional[BaseEnvManager]`): New environment to manage, if provided.
         """
         if _env is not None:
             self._env = _env
             self._env.launch()
             self._env_num = self._env.env_num
         else:
             self._env.reset()
 
     def reset_policy(self, _policy: Optional[namedtuple] = None) -> None:
         """
         Overview:
-            Reset the policy.
+            Reset or replace the policy used by this collector.
             If _policy is None, reset the old policy.
             If _policy is not None, replace the old policy in the collector with the new passed in policy.
         Arguments:
             - policy (:obj:`Optional[namedtuple]`): the api namedtuple of collect_mode policy
         """
         assert hasattr(self, '_env'), "please set env first"
         if _policy is not None:
@@ -116,15 +117,15 @@
                 'Set default n_episode mode(n_episode({}), env_num({}))'.format(self._default_n_episode, self._env_num)
             )
         self._policy.reset()
 
     def reset(self, _policy: Optional[namedtuple] = None, _env: Optional[BaseEnvManager] = None) -> None:
         """
         Overview:
-            Reset the environment and policy.
+            Reset the collector with the given policy and/or environment.
             If _env is None, reset the old environment.
             If _env is not None, replace the old environment in the collector with the new passed \
                 in environment and launch.
             If _policy is None, reset the old policy.
             If _policy is not None, replace the old policy in the collector with the new passed in policy.
         Arguments:
             - policy (:obj:`Optional[namedtuple]`): the api namedtuple of collect_mode policy
@@ -148,65 +149,67 @@
         # A game_segment_pool implementation based on the deque structure.
         self.game_segment_pool = deque(maxlen=int(1e6))
         self.unroll_plus_td_steps = self.policy_config.num_unroll_steps + self.policy_config.td_steps
 
     def _reset_stat(self, env_id: int) -> None:
         """
         Overview:
-            Reset the collector's state. Including reset the traj_buffer, obs_pool, policy_output_pool\
-                and env_info. Reset these states according to env_id. You can refer to base_serial_collector\
-                to get more messages.
+            Reset the collector's state. Including reset the traj_buffer, obs_pool, policy_output_pool \
+            and env_info. Reset these states according to env_id. You can refer to base_serial_collector\
+            to get more messages.
         Arguments:
             - env_id (:obj:`int`): the id where we need to reset the collector's state
         """
         self._env_info[env_id] = {'time': 0., 'step': 0}
 
     @property
     def envstep(self) -> int:
         """
         Overview:
-            Print the total envstep count.
-        Return:
-            - envstep (:obj:`int`): the total envstep count
+            Get the total number of environment steps collected.
+        Returns:
+            - envstep (:obj:`int`): Total number of environment steps collected.
         """
         return self._total_envstep_count
 
     def close(self) -> None:
         """
         Overview:
-            Close the collector. If end_flag is False, close the environment, flush the tb_logger\
-                and close the tb_logger.
+            Close the collector. If end_flag is False, close the environment, flush the tb_logger \
+            and close the tb_logger.
         """
         if self._end_flag:
             return
         self._end_flag = True
         self._env.close()
         if self._tb_logger:
             self._tb_logger.flush()
             self._tb_logger.close()
 
     def __del__(self) -> None:
         """
         Overview:
             Execute the close command and close the collector. __del__ is automatically called to \
-                destroy the collector instance when the collector finishes its work
+            destroy the collector instance when the collector finishes its work
         """
         self.close()
 
     # ==============================================================
     # MCTS+RL related core code
     # ==============================================================
-    def _compute_priorities(self, i, pred_values_lst, search_values_lst):
+    def _compute_priorities(self, i: int, pred_values_lst: List[float], search_values_lst: List[float]) -> np.ndarray:
         """
         Overview:
-            obtain the priorities at index i.
+            Compute the priorities for transitions based on prediction and search value discrepancies.
         Arguments:
-            - i: index.
-            - pred_values_lst: The list of value being predicted.
-            - search_values_lst: The list of value obtained through search.
+            - i (:obj:`int`): Index of the values in the list to compute the priority for.
+            - pred_values_lst (:obj:`List[float]`): List of predicted values.
+            - search_values_lst (:obj:`List[float]`): List of search values obtained from MCTS.
+        Returns:
+            - priorities (:obj:`np.ndarray`): Array of computed priorities.
         """
         if self.policy_config.use_priority:
             # Calculate priorities. The priorities are the L1 losses between the predicted
             # values and the search values. We use 'none' as the reduction parameter, which
             # means the loss is calculated for each element individually, instead of being summed or averaged. 
             # A small constant (1e-6) is added to the results to avoid zero priorities. This
             # is done because zero priorities could potentially cause issues in some scenarios.
@@ -218,30 +221,35 @@
                                   search_values).detach().cpu().numpy() + 1e-6
         else:
             # priorities is None -> use the max priority for all newly collected data
             priorities = None
 
         return priorities
 
-    def pad_and_save_last_trajectory(self, i, last_game_segments, last_game_priorities, game_segments, done) -> None:
+    def pad_and_save_last_trajectory(self, i: int, last_game_segments: List[GameSegment],
+                                     last_game_priorities: List[np.ndarray],
+                                     game_segments: List[GameSegment], done: np.ndarray) -> None:
         """
         Overview:
-            put the last game segment into the pool if the current game is finished
+            Save the game segment to the pool if the current game is finished, padding it if necessary.
         Arguments:
-            - last_game_segments (:obj:`list`): list of the last game segments
-            - last_game_priorities (:obj:`list`): list of the last game priorities
-            - game_segments (:obj:`list`): list of the current game segments
+            - i (:obj:`int`): Index of the current game segment.
+            - last_game_segments (:obj:`List[GameSegment]`): List of the last game segments to be padded and saved.
+            - last_game_priorities (:obj:`List[np.ndarray]`): List of priorities of the last game segments.
+            - game_segments (:obj:`List[GameSegment]`): List of the current game segments.
+            - done (:obj:`np.ndarray`): Array indicating whether each game is done.
         Note:
             (last_game_segments[i].obs_segment[-4:][j] == game_segments[i].obs_segment[:4][j]).all() is True
         """
         # pad over last segment trajectory
         beg_index = self.policy_config.model.frame_stack_num
         end_index = beg_index + self.policy_config.num_unroll_steps
 
-        # the start <frame_stack_num> obs is init zero obs, so we take the [<frame_stack_num> : <frame_stack_num>+<num_unroll_steps>] obs as the pad obs
+        # the start <frame_stack_num> obs is init zero obs, so we take the
+        # [<frame_stack_num> : <frame_stack_num>+<num_unroll_steps>] obs as the pad obs
         # e.g. the start 4 obs is init zero obs, the num_unroll_steps is 5, so we take the [4:9] obs as the pad obs
         pad_obs_lst = game_segments[i].obs_segment[beg_index:end_index]
         pad_child_visits_lst = game_segments[i].child_visit_segment[:self.policy_config.num_unroll_steps]
         # EfficientZero original repo bug:
         # pad_child_visits_lst = game_segments[i].child_visit_segment[beg_index:end_index]
 
         beg_index = 0
@@ -258,18 +266,20 @@
         pad_root_values_lst = game_segments[i].root_value_segment[beg_index:end_index]
 
         if self.policy_config.gumbel_algo:
             pad_improved_policy_prob = game_segments[i].improved_policy_probs[beg_index:end_index]
 
         # pad over and save
         if self.policy_config.gumbel_algo:
-            last_game_segments[i].pad_over(pad_obs_lst, pad_reward_lst, pad_root_values_lst, pad_child_visits_lst, next_segment_improved_policy = pad_improved_policy_prob)
+            last_game_segments[i].pad_over(pad_obs_lst, pad_reward_lst, pad_root_values_lst, pad_child_visits_lst,
+                                           next_segment_improved_policy=pad_improved_policy_prob)
         else:
             if self.policy_config.use_ture_chance_label_in_chance_encoder:
-                last_game_segments[i].pad_over(pad_obs_lst, pad_reward_lst, pad_root_values_lst, pad_child_visits_lst, next_chances = chance_lst)
+                last_game_segments[i].pad_over(pad_obs_lst, pad_reward_lst, pad_root_values_lst, pad_child_visits_lst,
+                                               next_chances=chance_lst)
             else:
                 last_game_segments[i].pad_over(pad_obs_lst, pad_reward_lst, pad_root_values_lst, pad_child_visits_lst)
         """
         Note:
             game_segment element shape:
             obs: game_segment_length + stack + num_unroll_steps, 20+4 +5
             rew: game_segment_length + stack + num_unroll_steps + td_steps -1  20 +5+3-1
@@ -293,21 +303,21 @@
 
     def collect(self,
                 n_episode: Optional[int] = None,
                 train_iter: int = 0,
                 policy_kwargs: Optional[dict] = None) -> List[Any]:
         """
         Overview:
-            Collect `n_episode` data with policy_kwargs, which is already trained `train_iter` iterations.
+            Collect `n_episode` episodes of data with policy_kwargs, trained for `train_iter` iterations.
         Arguments:
-            - n_episode (:obj:`int`): the number of collecting data episode.
-            - train_iter (:obj:`int`): the number of training iteration.
-            - policy_kwargs (:obj:`dict`): the keyword args for policy forward.
+            - n_episode (:obj:`Optional[int]`): Number of episodes to collect.
+            - train_iter (:obj:`int`): Number of training iterations completed so far.
+            - policy_kwargs (:obj:`Optional[dict]`): Additional keyword arguments for the policy.
         Returns:
-            - return_data (:obj:`List`): A list containing collected game_segments
+            - return_data (:obj:`List[Any]`): Collected data in the form of a list.
         """
         if n_episode is None:
             if self._default_n_episode is None:
                 raise RuntimeError("Please specify collect n_episode")
             else:
                 n_episode = self._default_n_episode
         assert n_episode >= self._env_num, "Please make sure n_episode >= env_num{}/{}".format(n_episode, self._env_num)
@@ -321,15 +331,15 @@
         env_nums = self._env_num
 
         # initializations
         init_obs = self._env.ready_obs
 
         retry_waiting_time = 0.001
         while len(init_obs.keys()) != self._env_num:
-            # In order to be compatible with subprocess env_manager, in which sometimes self._env_num is not equal to
+            # To be compatible with subprocess env_manager, in which sometimes self._env_num is not equal to
             # len(self._env.ready_obs), especially in tictactoe env.
             self._logger.info('The current init_obs.keys() is {}'.format(init_obs.keys()))
             self._logger.info('Before sleeping, the _env_states is {}'.format(self._env._env_states))
             time.sleep(retry_waiting_time)
             self._logger.info('=' * 10 + 'Wait for all environments (subprocess) to finish resetting.' + '=' * 10)
             self._logger.info(
                 'After sleeping {}s, the current _env_states is {}'.format(retry_waiting_time, self._env._env_states)
@@ -396,18 +406,19 @@
                 action_mask = [action_mask_dict[env_id] for env_id in ready_env_id]
                 to_play = [to_play_dict[env_id] for env_id in ready_env_id]
                 if self.policy_config.use_ture_chance_label_in_chance_encoder:
                     chance_dict = {env_id: chance_dict[env_id] for env_id in ready_env_id}
                     chance = [chance_dict[env_id] for env_id in ready_env_id]
 
                 stack_obs = to_ndarray(stack_obs)
-
+                # return stack_obs shape: [B, S*C, W, H] e.g. [8, 4*1, 96, 96]
                 stack_obs = prepare_observation(stack_obs, self.policy_config.model.model_type)
 
-                stack_obs = torch.from_numpy(stack_obs).to(self.policy_config.device).float()
+                # stack_obs = torch.from_numpy(stack_obs).to(self.policy_config.device).float()
+                stack_obs = torch.from_numpy(stack_obs).to(self.policy_config.device)
 
                 # ==============================================================
                 # policy forward
                 # ==============================================================
                 policy_output = self._policy.forward(stack_obs, action_mask, temperature, to_play, epsilon)
 
                 actions_no_env_id = {k: v['action'] for k, v in policy_output.items()}
@@ -460,32 +471,33 @@
 
             interaction_duration = self._timer.value / len(timesteps)
 
             for env_id, timestep in timesteps.items():
                 with self._timer:
                     if timestep.info.get('abnormal', False):
                         # If there is an abnormal timestep, reset all the related variables(including this env).
-                        # suppose there is no reset param, just reset this env
+                        # suppose there is no reset param, reset this env
                         self._env.reset({env_id: None})
                         self._policy.reset([env_id])
                         self._reset_stat(env_id)
                         self._logger.info('Env{} returns a abnormal step, its info is {}'.format(env_id, timestep.info))
                         continue
                     obs, reward, done, info = timestep.obs, timestep.reward, timestep.done, timestep.info
 
                     if self.policy_config.sampled_algo:
                         game_segments[env_id].store_search_stats(
                             distributions_dict[env_id], value_dict[env_id], root_sampled_actions_dict[env_id]
                         )
                     elif self.policy_config.gumbel_algo:
-                        game_segments[env_id].store_search_stats(distributions_dict[env_id], value_dict[env_id], improved_policy = improved_policy_dict[env_id])
+                        game_segments[env_id].store_search_stats(distributions_dict[env_id], value_dict[env_id],
+                                                                 improved_policy=improved_policy_dict[env_id])
                     else:
                         game_segments[env_id].store_search_stats(distributions_dict[env_id], value_dict[env_id])
                     # append a transition tuple, including a_t, o_{t+1}, r_{t}, action_mask_{t}, to_play_{t}
-                    # in ``game_segments[env_id].init``, we have append o_{t} in ``self.obs_segment``
+                    # in ``game_segments[env_id].init``, we have appended o_{t} in ``self.obs_segment``
                     if self.policy_config.use_ture_chance_label_in_chance_encoder:
                         game_segments[env_id].append(
                             actions[env_id], to_ndarray(obs['observation']), reward, action_mask_dict[env_id],
                             to_play_dict[env_id], chance_dict[env_id]
                         )
                     else:
                         game_segments[env_id].append(
@@ -554,15 +566,14 @@
                         game_segments[env_id].reset(observation_window_stack[env_id])
 
                     self._env_info[env_id]['step'] += 1
                     collected_step += 1
 
                 self._env_info[env_id]['time'] += self._timer.value + interaction_duration
                 if timestep.done:
-                    self._total_episode_count += 1
                     reward = timestep.info['eval_episode_return']
                     info = {
                         'reward': reward,
                         'time': self._env_info[env_id]['time'],
                         'step': self._env_info[env_id]['step'],
                         'visit_entropy': visit_entropies_lst[env_id] / eps_steps_lst[env_id],
                     }
@@ -661,19 +672,14 @@
                     {
                         'priorities': self.game_segment_pool[i][1],
                         'done': self.game_segment_pool[i][2],
                         'unroll_plus_td_steps': self.unroll_plus_td_steps
                     } for i in range(len(self.game_segment_pool))
                 ]
                 self.game_segment_pool.clear()
-                # for i in range(len(self.game_segment_pool)):
-                #     print(self.game_segment_pool[i][0].obs_segment.__len__())
-                #     print(self.game_segment_pool[i][0].reward_segment)
-                # for i in range(len(return_data[0])):
-                #     print(return_data[0][i].reward_segment)
                 break
 
         collected_duration = sum([d['time'] for d in self._episode_info])
         # reduce data when enables DDP
         if self._world_size > 1:
             collected_step = allreduce_data(collected_step, 'sum')
             collected_episode = allreduce_data(collected_episode, 'sum')
@@ -685,18 +691,17 @@
         # log
         self._output_log(train_iter)
         return return_data
 
     def _output_log(self, train_iter: int) -> None:
         """
         Overview:
-            Print the output log information. You can refer to Docs/Best Practice/How to understand\
-             training generated folders/Serial mode/log/collector for more details.
+            Log the collector's data and output the log information.
         Arguments:
-            - train_iter (:obj:`int`): the number of training iteration.
+            - train_iter (:obj:`int`): Current training iteration number for logging context.
         """
         if self._rank != 0:
             return
         if (train_iter - self._last_train_iter) >= self._collect_print_freq and len(self._episode_info) > 0:
             self._last_train_iter = train_iter
             episode_count = len(self._episode_info)
             envstep_count = sum([d['step'] for d in self._episode_info])
```

### Comparing `LightZero-0.0.2/lzero/worker/muzero_evaluator.py` & `LightZero-0.0.5/lzero/worker/muzero_evaluator.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import copy
 import time
 from collections import namedtuple
-from typing import Optional, Callable, Tuple
+from typing import Optional, Callable, Tuple, Dict, Any
 
 import numpy as np
 import torch
 from ding.envs import BaseEnvManager
 from ding.torch_utils import to_ndarray, to_item, to_tensor
 from ding.utils import build_logger, EasyTimer
 from ding.utils import get_world_size, get_rank, broadcast_object_list
@@ -15,29 +15,29 @@
 from lzero.mcts.buffer.game_segment import GameSegment
 from lzero.mcts.utils import prepare_observation
 
 
 class MuZeroEvaluator(ISerialEvaluator):
     """
     Overview:
-        The Evaluator for MCTS+RL algorithms, including MuZero, EfficientZero, Sampled EfficientZero.
+        The Evaluator class for MCTS+RL algorithms, such as MuZero, EfficientZero, and Sampled EfficientZero.
     Interfaces:
         __init__, reset, reset_policy, reset_env, close, should_eval, eval
-    Property:
+    Properties:
         env, policy
     """
 
     @classmethod
     def default_config(cls: type) -> EasyDict:
         """
         Overview:
-            Get evaluator's default config. We merge evaluator's default config with other default configs\
-                and user's config to get the final config.
-        Return:
-            cfg (:obj:`EasyDict`): evaluator's default config
+            Retrieve the default configuration for the evaluator by merging evaluator-specific defaults with other
+            defaults and any user-provided configuration.
+        Returns:
+            - cfg (:obj:`EasyDict`): The default configuration for the evaluator.
         """
         cfg = EasyDict(copy.deepcopy(cls.config))
         cfg.cfg_type = cls.__name__ + 'Dict'
         return cfg
 
     config = dict(
         # Evaluate every "eval_freq" training iterations.
@@ -54,25 +54,25 @@
             tb_logger: 'SummaryWriter' = None,  # noqa
             exp_name: Optional[str] = 'default_experiment',
             instance_name: Optional[str] = 'evaluator',
             policy_config: 'policy_config' = None,  # noqa
     ) -> None:
         """
         Overview:
-            Init method. Load config and use ``self._cfg`` setting to build common serial evaluator components,
-            e.g. logger helper, timer.
+            Initialize the evaluator with configuration settings for various components such as logger helper and timer.
         Arguments:
-            - eval_freq (:obj:`int`): evaluation frequency in terms of training steps.
-            - n_evaluator_episode (:obj:`int`): the number of episodes to eval in total.
-            - env (:obj:`BaseEnvManager`): the subclass of vectorized env_manager(BaseEnvManager)
-            - policy (:obj:`namedtuple`): the api namedtuple of collect_mode policy
-            - tb_logger (:obj:`SummaryWriter`): tensorboard handle
-            - exp_name (:obj:`str`): Experiment name, which is used to indicate output directory.
-            - instance_name (:obj:`Optional[str]`): Name of this instance.
-            - policy_config: Config of game.
+            - eval_freq (:obj:`int`): Evaluation frequency in terms of training steps.
+            - n_evaluator_episode (:obj:`int`): Number of episodes to evaluate in total.
+            - stop_value (:obj:`float`): A reward threshold above which the training is considered converged.
+            - env (:obj:`Optional[BaseEnvManager]`): An optional instance of a subclass of BaseEnvManager.
+            - policy (:obj:`Optional[namedtuple]`): An optional API namedtuple defining the policy for evaluation.
+            - tb_logger (:obj:`Optional[SummaryWriter]`): Optional TensorBoard logger instance.
+            - exp_name (:obj:`str`): Name of the experiment, used to determine output directory.
+            - instance_name (:obj:`str`): Name of this evaluator instance.
+            - policy_config (:obj:`Optional[dict]`): Optional configuration for the game policy.
         """
         self._eval_freq = eval_freq
         self._exp_name = exp_name
         self._instance_name = instance_name
 
         # Logger (Monitor will be initialized in policy setter)
         # Only rank == 0 learner needs monitor and tb_logger, others only need text_logger to display terminal output.
@@ -99,72 +99,66 @@
         # MCTS+RL related core code
         # ==============================================================
         self.policy_config = policy_config
 
     def reset_env(self, _env: Optional[BaseEnvManager] = None) -> None:
         """
         Overview:
-            Reset evaluator's environment. In some case, we need evaluator use the same policy in different \
-                environments. We can use reset_env to reset the environment.
-            If _env is None, reset the old environment.
-            If _env is not None, replace the old environment in the evaluator with the \
-                new passed in environment and launch.
+            Reset the environment for the evaluator, optionally replacing it with a new environment.
+            If _env is None, reset the old environment. If _env is not None, replace the old environment
+            in the evaluator with the new passed in environment and launch.
         Arguments:
-            - env (:obj:`Optional[BaseEnvManager]`): instance of the subclass of vectorized \
-                env_manager(BaseEnvManager)
+            - _env (:obj:`Optional[BaseEnvManager]`): An optional new environment instance to replace the existing one.
         """
         if _env is not None:
             self._env = _env
             self._env.launch()
             self._env_num = self._env.env_num
         else:
             self._env.reset()
 
     def reset_policy(self, _policy: Optional[namedtuple] = None) -> None:
         """
         Overview:
-            Reset evaluator's policy. In some case, we need evaluator work in this same environment but use\
-                different policy. We can use reset_policy to reset the policy.
+            Reset the policy for the evaluator, optionally replacing it with a new policy.
             If _policy is None, reset the old policy.
             If _policy is not None, replace the old policy in the evaluator with the new passed in policy.
         Arguments:
-            - policy (:obj:`Optional[namedtuple]`): the api namedtuple of eval_mode policy
+            - _policy (:obj:`Optional[namedtuple]`): An optional new policy namedtuple to replace the existing one.
         """
         assert hasattr(self, '_env'), "please set env first"
         if _policy is not None:
             self._policy = _policy
         self._policy.reset()
 
     def reset(self, _policy: Optional[namedtuple] = None, _env: Optional[BaseEnvManager] = None) -> None:
         """
         Overview:
-            Reset evaluator's policy and environment. Use new policy and environment to collect data.
+            Reset both the policy and environment for the evaluator, optionally replacing them.
             If _env is None, reset the old environment.
             If _env is not None, replace the old environment in the evaluator with the new passed in \
                 environment and launch.
             If _policy is None, reset the old policy.
             If _policy is not None, replace the old policy in the evaluator with the new passed in policy.
         Arguments:
-            - policy (:obj:`Optional[namedtuple]`): the api namedtuple of eval_mode policy
-            - env (:obj:`Optional[BaseEnvManager]`): instance of the subclass of vectorized \
-                env_manager(BaseEnvManager)
+            - _policy (:obj:`Optional[namedtuple]`): An optional new policy namedtuple to replace the existing one.
+            - _env (:obj:`Optional[BaseEnvManager]`): An optional new environment instance to replace the existing one.
         """
         if _env is not None:
             self.reset_env(_env)
         if _policy is not None:
             self.reset_policy(_policy)
         self._max_episode_return = float("-inf")
         self._last_eval_iter = 0
         self._end_flag = False
 
     def close(self) -> None:
         """
         Overview:
-            Close the evaluator. If end_flag is False, close the environment, flush the tb_logger\
-                and close the tb_logger.
+            Close the evaluator, the environment, flush and close the TensorBoard logger if applicable.
         """
         if self._end_flag:
             return
         self._end_flag = True
         self._env.close()
         if self._tb_logger:
             self._tb_logger.flush()
@@ -177,46 +171,49 @@
                 to destroy the evaluator instance when the evaluator finishes its work
         """
         self.close()
 
     def should_eval(self, train_iter: int) -> bool:
         """
         Overview:
-            Determine whether you need to start the evaluation mode, if the number of training has reached\
-                the maximum number of times to start the evaluator, return True
+            Determine whether to initiate evaluation based on the training iteration count and evaluation frequency.
         Arguments:
-            - train_iter (:obj:`int`): Current training iteration.
+            - train_iter (:obj:`int`): The current count of training iterations.
+        Returns:
+            - (:obj:`bool`): `True` if evaluation should be initiated, otherwise `False`.
         """
         if train_iter == self._last_eval_iter:
             return False
         if (train_iter - self._last_eval_iter) < self._eval_freq and train_iter != 0:
             return False
         self._last_eval_iter = train_iter
         return True
 
     def eval(
             self,
             save_ckpt_fn: Callable = None,
             train_iter: int = -1,
             envstep: int = -1,
             n_episode: Optional[int] = None,
+            return_trajectory: bool = False,
     ) -> Tuple[bool, float]:
         """
         Overview:
-            Evaluate policy and store the best policy based on whether it reaches the highest historical reward.
+            Evaluate the current policy, storing the best policy if it achieves the highest historical reward.
         Arguments:
-            - save_ckpt_fn (:obj:`Callable`): Saving ckpt function, which will be triggered by getting the best reward.
-            - train_iter (:obj:`int`): Current training iteration.
-            - envstep (:obj:`int`): Current env interaction step.
-            - n_episode (:obj:`int`): Number of evaluation episodes.
+            - save_ckpt_fn (:obj:`Optional[Callable]`): Optional function to save a checkpoint when a new best reward is achieved.
+            - train_iter (:obj:`int`): The current training iteration count.
+            - envstep (:obj:`int`): The current environment step count.
+            - n_episode (:obj:`Optional[int]`): Optional number of evaluation episodes; defaults to the evaluator's setting.
+            - return_trajectory (:obj:`bool`): Return the evaluated trajectory `game_segments` in `episode_info` if True.
         Returns:
-            - stop_flag (:obj:`bool`): Whether this training program can be ended.
-            - episode_info (:obj:`Dict[str, List]`): Current evaluation episode information.
+            - stop_flag (:obj:`bool`): Indicates whether the training can be stopped based on the stop value.
+            - episode_info (:obj:`Dict[str, Any]`): A dictionary containing information about the evaluation episodes.
         """
-        # evaluator only work on rank0
+        # the evaluator only works on rank0
         episode_info = None
         stop_flag = False
         if get_rank() == 0:
             if n_episode is None:
                 n_episode = self._default_n_episode
             assert n_episode is not None, "please indicate eval n_episode"
             envstep_count = 0
@@ -227,15 +224,15 @@
             self._policy.reset()
 
             # initializations
             init_obs = self._env.ready_obs
 
             retry_waiting_time = 0.001
             while len(init_obs.keys()) != self._env_num:
-                # In order to be compatible with subprocess env_manager, in which sometimes self._env_num is not equal to
+                # To be compatible with subprocess env_manager, in which sometimes self._env_num is not equal to
                 # len(self._env.ready_obs), especially in tictactoe env.
                 self._logger.info('The current init_obs.keys() is {}'.format(init_obs.keys()))
                 self._logger.info('Before sleeping, the _env_states is {}'.format(self._env._env_states))
                 time.sleep(retry_waiting_time)
                 self._logger.info('=' * 10 + 'Wait for all environments (subprocess) to finish resetting.' + '=' * 10)
                 self._logger.info(
                     'After sleeping {}s, the current _env_states is {}'.format(retry_waiting_time,
@@ -451,8 +448,10 @@
 
         if get_world_size() > 1:
             objects = [stop_flag, episode_info]
             broadcast_object_list(objects, src=0)
             stop_flag, episode_info = objects
 
         episode_info = to_item(episode_info)
+        if return_trajectory:
+            episode_info['trajectory'] = game_segments
         return stop_flag, episode_info
```

### Comparing `LightZero-0.0.2/pyproject.toml` & `LightZero-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/setup.py` & `LightZero-0.0.5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,37 +11,23 @@
 # limitations under the License.
 import os
 import re
 from distutils.core import setup
 
 import numpy as np
 from setuptools import find_packages, Extension
-# from setuptools.command.build_ext import build_ext
 from Cython.Build import cythonize  # this line should be after 'from setuptools import find_packages'
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 
 def _load_req(file: str):
     with open(file, 'r', encoding='utf-8') as f:
         return [line.strip() for line in f.readlines() if line.strip()]
 
-
-# class custom_build_ext(build_ext):
-#     def build_extensions(self):
-#         # Override the compiler executables. Importantly, this
-#         # removes the "default" compiler flags that would
-#         # otherwise get passed on to the compiler, i.e.,
-#         # distutils.sysconfig.get_var("CFLAGS").
-#         self.compiler.set_executable("compiler_so", "g++")
-#         self.compiler.set_executable("compiler_cxx", "g++")
-#         self.compiler.set_executable("linker_so", "g++")
-#         build_ext.build_extensions(self)
-
-
 requirements = _load_req('requirements.txt')
 
 _REQ_PATTERN = re.compile('^requirements-([a-zA-Z0-9_]+)\\.txt$')
 group_requirements = {
     item.group(1): _load_req(item.group(0))
     for item in [_REQ_PATTERN.fullmatch(reqpath) for reqpath in os.listdir()] if item
 }
@@ -81,17 +67,16 @@
     return extensions
 
 
 _LINETRACE = not not os.environ.get('LINETRACE', None)
 
 setup(
     name='LightZero',
-    version='0.0.2',
+    version='0.0.5',
     description='A lightweight and efficient MCTS/AlphaZero/MuZero algorithm toolkits.',
-    # long_description=readme,
     long_description_content_type='text/markdown',
     author='opendilab',
     author_email='opendilab@pjlab.org.cn',
     url='https://github.com/opendilab/LightZero',
     license='Apache License, Version 2.0',
     keywords='Reinforcement Learning, MCTS, MuZero',
     packages=[
@@ -111,15 +96,14 @@
     ext_modules=cythonize(
         find_cython_extensions(),
         language_level=3,
         compiler_directives=dict(
             linetrace=_LINETRACE,
         ),
     ),
-    # cmdclass={"build_ext": custom_build_ext},
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         "Intended Audience :: Science/Research",
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: POSIX :: Linux',
         # 'Operating System :: Microsoft :: Windows',
         'Operating System :: MacOS :: MacOS X',
```

### Comparing `LightZero-0.0.2/zoo/atari/config/atari_efficientzero_config.py` & `LightZero-0.0.5/zoo/atari/config/atari_efficientzero_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from easydict import EasyDict
 
 # options={'PongNoFrameskip-v4', 'QbertNoFrameskip-v4', 'MsPacmanNoFrameskip-v4', 'SpaceInvadersNoFrameskip-v4', 'BreakoutNoFrameskip-v4', ...}
-env_name = 'PongNoFrameskip-v4'
+env_id = 'PongNoFrameskip-v4'
 
-if env_name == 'PongNoFrameskip-v4':
+if env_id == 'PongNoFrameskip-v4':
     action_space_size = 6
-elif env_name == 'QbertNoFrameskip-v4':
+elif env_id == 'QbertNoFrameskip-v4':
     action_space_size = 6
-elif env_name == 'MsPacmanNoFrameskip-v4':
+elif env_id == 'MsPacmanNoFrameskip-v4':
     action_space_size = 9
-elif env_name == 'SpaceInvadersNoFrameskip-v4':
+elif env_id == 'SpaceInvadersNoFrameskip-v4':
     action_space_size = 6
-elif env_name == 'BreakoutNoFrameskip-v4':
+elif env_id == 'BreakoutNoFrameskip-v4':
     action_space_size = 4
 
 # ==============================================================
 # begin of the most frequently changed config specified by the user
 # ==============================================================
 collector_env_num = 8
 n_episode = 8
@@ -29,17 +29,17 @@
 eps_greedy_exploration_in_collect = False
 # ==============================================================
 # end of the most frequently changed config specified by the user
 # ==============================================================
 
 atari_efficientzero_config = dict(
     exp_name=
-    f'data_ez_ctree/{env_name[:-14]}_efficientzero_ns{num_simulations}_upc{update_per_collect}_rr{reanalyze_ratio}_seed0',
+    f'data_ez_ctree/{env_id[:-14]}_efficientzero_ns{num_simulations}_upc{update_per_collect}_rr{reanalyze_ratio}_seed0',
     env=dict(
-        env_name=env_name,
+        env_id=env_id,
         obs_shape=(4, 96, 96),
         collector_env_num=collector_env_num,
         evaluator_env_num=evaluator_env_num,
         n_evaluator_episode=evaluator_env_num,
         manager=dict(shared_memory=False, ),
     ),
     policy=dict(
```

### Comparing `LightZero-0.0.2/zoo/atari/config/atari_efficientzero_multigpu_ddp_config.py` & `LightZero-0.0.5/zoo/atari/config/atari_efficientzero_multigpu_ddp_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from easydict import EasyDict
 
 # options={'PongNoFrameskip-v4', 'QbertNoFrameskip-v4', 'MsPacmanNoFrameskip-v4', 'SpaceInvadersNoFrameskip-v4', 'BreakoutNoFrameskip-v4', ...}
-env_name = 'PongNoFrameskip-v4'
+env_id = 'PongNoFrameskip-v4'
 
-if env_name == 'PongNoFrameskip-v4':
+if env_id == 'PongNoFrameskip-v4':
     action_space_size = 6
-elif env_name == 'QbertNoFrameskip-v4':
+elif env_id == 'QbertNoFrameskip-v4':
     action_space_size = 6
-elif env_name == 'MsPacmanNoFrameskip-v4':
+elif env_id == 'MsPacmanNoFrameskip-v4':
     action_space_size = 9
-elif env_name == 'SpaceInvadersNoFrameskip-v4':
+elif env_id == 'SpaceInvadersNoFrameskip-v4':
     action_space_size = 6
-elif env_name == 'BreakoutNoFrameskip-v4':
+elif env_id == 'BreakoutNoFrameskip-v4':
     action_space_size = 4
 
 # ==============================================================
 # begin of the most frequently changed config specified by the user
 # ==============================================================
 gpu_num = 2
 collector_env_num = 8
@@ -37,18 +37,17 @@
 # batch_size = 4
 # max_env_step = int(1e6)
 # ==============================================================
 # end of the most frequently changed config specified by the user
 # ==============================================================
 
 atari_efficientzero_config = dict(
-    exp_name=
-    f'data_ez_ctree/{env_name[:-14]}_efficientzero_ns{num_simulations}_upc{update_per_collect}_rr{reanalyze_ratio}_ddp_{gpu_num}gpu_seed0',
+    exp_name=f'data_ez_ctree/{env_id[:-14]}_efficientzero_ns{num_simulations}_upc{update_per_collect}_rr{reanalyze_ratio}_ddp_{gpu_num}gpu_seed0',
     env=dict(
-        env_name=env_name,
+        env_id=env_id,
         obs_shape=(4, 96, 96),
         collector_env_num=collector_env_num,
         evaluator_env_num=evaluator_env_num,
         n_evaluator_episode=evaluator_env_num,
         manager=dict(shared_memory=False, ),
     ),
     policy=dict(
@@ -121,10 +120,10 @@
     from lzero.config.utils import lz_to_ddp_config
 
     seed_list = [0, 1, 2]  # list of seeds you want to use for training
     for seed in seed_list:
         with DDPContext():
             # Each iteration uses a different seed for training
             # Change exp_name according to current seed
-            main_config.exp_name = f'data_ez_ctree/{env_name[:-14]}_efficientzero_ns{num_simulations}_upc{update_per_collect}_rr{reanalyze_ratio}_ddp_{gpu_num}gpu_seed{seed}'
+            main_config.exp_name = f'data_ez_ctree/{env_id[:-14]}_efficientzero_ns{num_simulations}_upc{update_per_collect}_rr{reanalyze_ratio}_ddp_{gpu_num}gpu_seed{seed}'
             main_config = lz_to_ddp_config(main_config)
             train_muzero([main_config, create_config], seed=seed, max_env_step=max_env_step)
```

### Comparing `LightZero-0.0.2/zoo/atari/config/atari_gumbel_muzero_config.py` & `LightZero-0.0.5/zoo/atari/config/atari_gumbel_muzero_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from easydict import EasyDict
 
 # options={'PongNoFrameskip-v4', 'QbertNoFrameskip-v4', 'MsPacmanNoFrameskip-v4', 'SpaceInvadersNoFrameskip-v4', 'BreakoutNoFrameskip-v4', ...}
-env_name = 'PongNoFrameskip-v4'
+env_id = 'PongNoFrameskip-v4'
 
-if env_name == 'PongNoFrameskip-v4':
+if env_id == 'PongNoFrameskip-v4':
     action_space_size = 6
-elif env_name == 'QbertNoFrameskip-v4':
+elif env_id == 'QbertNoFrameskip-v4':
     action_space_size = 6
-elif env_name == 'MsPacmanNoFrameskip-v4':
+elif env_id == 'MsPacmanNoFrameskip-v4':
     action_space_size = 9
-elif env_name == 'SpaceInvadersNoFrameskip-v4':
+elif env_id == 'SpaceInvadersNoFrameskip-v4':
     action_space_size = 6
-elif env_name == 'BreakoutNoFrameskip-v4':
+elif env_id == 'BreakoutNoFrameskip-v4':
     action_space_size = 4
 
 # ==============================================================
 # begin of the most frequently changed config specified by the user
 # ==============================================================
 collector_env_num = 8
 n_episode = 8
@@ -27,18 +27,18 @@
 reanalyze_ratio = 0.
 # ==============================================================
 # end of the most frequently changed config specified by the user
 # ==============================================================
 
 atari_gumbel_muzero_config = dict(
     exp_name=
-    f'data_mz_ctree/{env_name[:-14]}_gumbel_muzero_ns{num_simulations}_upc{update_per_collect}_rr{reanalyze_ratio}_seed0',
+    f'data_mz_ctree/{env_id[:-14]}_gumbel_muzero_ns{num_simulations}_upc{update_per_collect}_rr{reanalyze_ratio}_seed0',
     env=dict(
         stop_value=int(1e6),
-        env_name=env_name,
+        env_id=env_id,
         obs_shape=(4, 96, 96),
         collector_env_num=collector_env_num,
         evaluator_env_num=evaluator_env_num,
         n_evaluator_episode=evaluator_env_num,
         manager=dict(shared_memory=False, ),
     ),
     policy=dict(
```

### Comparing `LightZero-0.0.2/zoo/atari/config/atari_muzero_config.py` & `LightZero-0.0.5/zoo/atari/config/atari_muzero_config_tmp.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,50 +1,54 @@
 from easydict import EasyDict
 
 # options={'PongNoFrameskip-v4', 'QbertNoFrameskip-v4', 'MsPacmanNoFrameskip-v4', 'SpaceInvadersNoFrameskip-v4', 'BreakoutNoFrameskip-v4', ...}
-env_name = 'PongNoFrameskip-v4'
+env_id = 'PongNoFrameskip-v4'
 
-if env_name == 'PongNoFrameskip-v4':
+if env_id == 'PongNoFrameskip-v4':
     action_space_size = 6
-elif env_name == 'QbertNoFrameskip-v4':
+elif env_id == 'QbertNoFrameskip-v4':
     action_space_size = 6
-elif env_name == 'MsPacmanNoFrameskip-v4':
+elif env_id == 'MsPacmanNoFrameskip-v4':
     action_space_size = 9
-elif env_name == 'SpaceInvadersNoFrameskip-v4':
+elif env_id == 'SpaceInvadersNoFrameskip-v4':
     action_space_size = 6
-elif env_name == 'BreakoutNoFrameskip-v4':
+elif env_id == 'BreakoutNoFrameskip-v4':
     action_space_size = 4
 
 # ==============================================================
 # begin of the most frequently changed config specified by the user
 # ==============================================================
 collector_env_num = 8
 n_episode = 8
 evaluator_env_num = 3
-num_simulations = 50
+# num_simulations = 50
+num_simulations = 5
+
 update_per_collect = 1000
 batch_size = 256
 max_env_step = int(1e6)
-reanalyze_ratio = 0.
+reanalyze_ratio = 1.
 eps_greedy_exploration_in_collect = False
 # ==============================================================
 # end of the most frequently changed config specified by the user
 # ==============================================================
 
 atari_muzero_config = dict(
     exp_name=
-    f'data_mz_ctree/{env_name[:-14]}_muzero_ns{num_simulations}_upc{update_per_collect}_rr{reanalyze_ratio}_seed0',
+    f'data_mz_ctree/{env_id[:-14]}_muzero_ns{num_simulations}_upc{update_per_collect}_rr{reanalyze_ratio}_seed0',
     env=dict(
         stop_value=int(1e6),
-        env_name=env_name,
+        env_id=env_id,
         obs_shape=(4, 96, 96),
         collector_env_num=collector_env_num,
         evaluator_env_num=evaluator_env_num,
         n_evaluator_episode=evaluator_env_num,
         manager=dict(shared_memory=False, ),
+        collect_max_episode_steps=int(50),
+        eval_max_episode_steps=int(50),
     ),
     policy=dict(
         model=dict(
             observation_shape=(4, 96, 96),
             frame_stack_num=4,
             action_space_size=action_space_size,
             downsample=True,
```

### Comparing `LightZero-0.0.2/zoo/atari/config/atari_muzero_multigpu_ddp_config.py` & `LightZero-0.0.5/zoo/atari/config/atari_muzero_multigpu_ddp_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from easydict import EasyDict
 
 # options={'PongNoFrameskip-v4', 'QbertNoFrameskip-v4', 'MsPacmanNoFrameskip-v4', 'SpaceInvadersNoFrameskip-v4', 'BreakoutNoFrameskip-v4', ...}
-env_name = 'PongNoFrameskip-v4'
+env_id = 'PongNoFrameskip-v4'
 
-if env_name == 'PongNoFrameskip-v4':
+if env_id == 'PongNoFrameskip-v4':
     action_space_size = 6
-elif env_name == 'QbertNoFrameskip-v4':
+elif env_id == 'QbertNoFrameskip-v4':
     action_space_size = 6
-elif env_name == 'MsPacmanNoFrameskip-v4':
+elif env_id == 'MsPacmanNoFrameskip-v4':
     action_space_size = 9
-elif env_name == 'SpaceInvadersNoFrameskip-v4':
+elif env_id == 'SpaceInvadersNoFrameskip-v4':
     action_space_size = 6
-elif env_name == 'BreakoutNoFrameskip-v4':
+elif env_id == 'BreakoutNoFrameskip-v4':
     action_space_size = 4
 
 # ==============================================================
 # begin of the most frequently changed config specified by the user
 # ==============================================================
 gpu_num = 2
 collector_env_num = 8
@@ -28,19 +28,18 @@
 reanalyze_ratio = 0.
 eps_greedy_exploration_in_collect = False
 # ==============================================================
 # end of the most frequently changed config specified by the user
 # ==============================================================
 
 atari_muzero_config = dict(
-    exp_name=
-    f'data_mz_ctree/{env_name[:-14]}_muzero_ns{num_simulations}_upc{update_per_collect}_rr{reanalyze_ratio}_ddp_{gpu_num}gpu_seed0',
+    exp_name=f'data_mz_ctree/{env_id[:-14]}_muzero_ns{num_simulations}_upc{update_per_collect}_rr{reanalyze_ratio}_ddp_{gpu_num}gpu_seed0',
     env=dict(
         stop_value=int(1e6),
-        env_name=env_name,
+        env_id=env_id,
         obs_shape=(4, 96, 96),
         collector_env_num=collector_env_num,
         evaluator_env_num=evaluator_env_num,
         n_evaluator_episode=evaluator_env_num,
         manager=dict(shared_memory=False, ),
     ),
     policy=dict(
```

### Comparing `LightZero-0.0.2/zoo/atari/config/atari_sampled_efficientzero_config.py` & `LightZero-0.0.5/zoo/atari/config/atari_sampled_efficientzero_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from easydict import EasyDict
 
 # options={'PongNoFrameskip-v4', 'QbertNoFrameskip-v4', 'MsPacmanNoFrameskip-v4', 'SpaceInvadersNoFrameskip-v4', 'BreakoutNoFrameskip-v4', ...}
-env_name = 'PongNoFrameskip-v4'
+env_id = 'PongNoFrameskip-v4'
 
-if env_name == 'PongNoFrameskip-v4':
+if env_id == 'PongNoFrameskip-v4':
     action_space_size = 6
-elif env_name == 'QbertNoFrameskip-v4':
+elif env_id == 'QbertNoFrameskip-v4':
     action_space_size = 6
-elif env_name == 'MsPacmanNoFrameskip-v4':
+elif env_id == 'MsPacmanNoFrameskip-v4':
     action_space_size = 9
-elif env_name == 'SpaceInvadersNoFrameskip-v4':
+elif env_id == 'SpaceInvadersNoFrameskip-v4':
     action_space_size = 6
-elif env_name == 'BreakoutNoFrameskip-v4':
+elif env_id == 'BreakoutNoFrameskip-v4':
     action_space_size = 4
 
 # ==============================================================
 # begin of the most frequently changed config specified by the user
 # ==============================================================
 continuous_action_space = False
 K = 5  # num_of_sampled_actions
@@ -29,17 +29,17 @@
 reanalyze_ratio = 0.
 # ==============================================================
 # end of the most frequently changed config specified by the user
 # ==============================================================
 
 atari_sampled_efficientzero_config = dict(
     exp_name=
-    f'data_sez_ctree/{env_name[:-14]}_sampled_efficientzero_k{K}_ns{num_simulations}_upc{update_per_collect}_rr{reanalyze_ratio}_seed0',
+    f'data_sez_ctree/{env_id[:-14]}_sampled_efficientzero_k{K}_ns{num_simulations}_upc{update_per_collect}_rr{reanalyze_ratio}_seed0',
     env=dict(
-        env_name=env_name,
+        env_id=env_id,
         obs_shape=(4, 96, 96),
         collector_env_num=collector_env_num,
         evaluator_env_num=evaluator_env_num,
         n_evaluator_episode=evaluator_env_num,
         manager=dict(shared_memory=False, ),
     ),
     policy=dict(
```

### Comparing `LightZero-0.0.2/zoo/atari/config/atari_stochastic_muzero_config.py` & `LightZero-0.0.5/zoo/atari/config/atari_stochastic_muzero_config.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from easydict import EasyDict
 
 # options={'PongNoFrameskip-v4', 'QbertNoFrameskip-v4', 'MsPacmanNoFrameskip-v4', 'SpaceInvadersNoFrameskip-v4', 'BreakoutNoFrameskip-v4', ...}
-env_name = 'PongNoFrameskip-v4'
+env_id = 'PongNoFrameskip-v4'
 
-if env_name == 'PongNoFrameskip-v4':
+if env_id == 'PongNoFrameskip-v4':
     action_space_size = 6
-elif env_name == 'QbertNoFrameskip-v4':
+elif env_id == 'QbertNoFrameskip-v4':
     action_space_size = 6
-elif env_name == 'MsPacmanNoFrameskip-v4':
+elif env_id == 'MsPacmanNoFrameskip-v4':
     action_space_size = 9
-elif env_name == 'SpaceInvadersNoFrameskip-v4':
+elif env_id == 'SpaceInvadersNoFrameskip-v4':
     action_space_size = 6
-elif env_name == 'BreakoutNoFrameskip-v4':
+elif env_id == 'BreakoutNoFrameskip-v4':
     action_space_size = 4
 
 # ==============================================================
 # begin of the most frequently changed config specified by the user
 # ==============================================================
 # collector_env_num = 8
 # n_episode = 8
@@ -39,18 +39,18 @@
 chance_space_size = 4
 # ==============================================================
 # end of the most frequently changed config specified by the user
 # ==============================================================
 
 atari_stochastic_muzero_config = dict(
     exp_name=
-    f'data_stochastic_mz_ctree/{env_name[:-14]}_stochastic_muzero_ns{num_simulations}_upc{update_per_collect}_rr{reanalyze_ratio}_chance{chance_space_size}_seed0',
+    f'data_stochastic_mz_ctree/{env_id[:-14]}_stochastic_muzero_ns{num_simulations}_upc{update_per_collect}_rr{reanalyze_ratio}_chance{chance_space_size}_seed0',
     env=dict(
         stop_value=int(1e6),
-        env_name=env_name,
+        env_id=env_id,
         obs_shape=(4, 96, 96),
         collector_env_num=collector_env_num,
         evaluator_env_num=evaluator_env_num,
         n_evaluator_episode=evaluator_env_num,
         manager=dict(shared_memory=False, ),
     ),
     policy=dict(
```

### Comparing `LightZero-0.0.2/zoo/atari/entry/atari_eval.py` & `LightZero-0.0.5/zoo/game_2048/entry/2048_eval.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,50 @@
 # According to the model you want to evaluate, import the corresponding config.
-from lzero.entry import eval_muzero
 import numpy as np
 
+from lzero.entry import eval_muzero
+from zoo.game_2048.config.muzero_2048_config import main_config, create_config
+from zoo.game_2048.config.stochastic_muzero_2048_config import main_config, create_config
+
 if __name__ == "__main__":
-    """ 
-    model_path (:obj:`Optional[str]`): The pretrained model path, which should
-    point to the ckpt file of the pretrained model, and an absolute path is recommended.
-    In LightZero, the path is usually something like ``exp_name/ckpt/ckpt_best.pth.tar``.
     """
-    # Take the config of sampled efficientzero as an example
-    from zoo.atari.config.atari_sampled_efficientzero_config import main_config, create_config
+    Entry point for the evaluation of the muzero or stochastic_muzero model on the 2048 environment. 
+
+    Variables:
+        - model_path (:obj:`Optional[str]`): The pretrained model path, which should point to the ckpt file of the 
+        pretrained model. An absolute path is recommended. In LightZero, the path is usually something like 
+        ``exp_name/ckpt/ckpt_best.pth.tar``.
+        - returns_mean_seeds (:obj:`List[float]`): List to store the mean returns for each seed.
+        - returns_seeds (:obj:`List[float]`): List to store the returns for each seed.
+        - seeds (:obj:`List[int]`): List of seeds for the environment.
+        - num_episodes_each_seed (:obj:`int`): Number of episodes to run for each seed.
+        - total_test_episodes (:obj:`int`): Total number of test episodes, computed as the product of the number of 
+        seeds and the number of episodes per seed.
+    """
 
-    model_path = "/path/ckpt/ckpt_best.pth.tar"
+    # model_path = './ckpt/ckpt_best.pth.tar'
+    model_path = None
 
     returns_mean_seeds = []
     returns_seeds = []
     seeds = [0]
     num_episodes_each_seed = 1
+
+    # main_config.env.render_mode = 'image_realtime_mode'
+    main_config.env.render_mode = 'image_savefile_mode'
+    main_config.env.replay_path = './video'
+    main_config.env.replay_format = 'gif'
+    main_config.env.replay_name_suffix = 'muzero_ns100_s0'
+    # main_config.env.replay_name_suffix = 'stochastic_muzero_ns100_s0'
+
+    main_config.env.max_episode_steps = int(1e9)  # Adjust according to different environments
     total_test_episodes = num_episodes_each_seed * len(seeds)
     create_config.env_manager.type = 'base'  # Visualization requires the 'type' to be set as base
-    main_config.env.evaluator_env_num = 1  # Visualization requires the 'env_num' to be set as 1
+    main_config.env.evaluator_env_num = 1   # Visualization requires the 'env_num' to be set as 1
     main_config.env.n_evaluator_episode = total_test_episodes
-    main_config.env.render_mode_human = True  # Whether to enable real-time rendering
-    main_config.env.save_video = True  # Whether to save the video, if save the video render_mode_human must to be True
-    main_config.env.save_path = '../config/'
-    main_config.env.eval_max_episode_steps = int(1e3)  # Adjust according to different environments
-
     for seed in seeds:
         returns_mean, returns = eval_muzero(
             [main_config, create_config],
             seed=seed,
             num_episodes_each_seed=num_episodes_each_seed,
             print_seed_details=False,
             model_path=model_path
```

### Comparing `LightZero-0.0.2/zoo/atari/envs/atari_wrappers.py` & `LightZero-0.0.5/zoo/atari/envs/atari_wrappers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,24 @@
-# Borrow a lot from openai baselines:
-# https://github.com/openai/baselines/blob/master/baselines/common/atari_wrappers.py
+# Adapted from openai baselines: https://github.com/openai/baselines/blob/master/baselines/common/atari_wrappers.py
+from datetime import datetime
+from typing import Optional
 
 import cv2
+import gymnasium 
 import gym
 import numpy as np
 from ding.envs import NoopResetWrapper, MaxAndSkipWrapper, EpisodicLifeWrapper, FireResetWrapper, WarpFrameWrapper, \
     ScaledFloatFrameWrapper, \
     ClipRewardWrapper, FrameStackWrapper
 from ding.utils.compression_helper import jpeg_data_compressor
-from gym.wrappers import RecordVideo
+from easydict import EasyDict
+from gymnasium.wrappers import RecordVideo
 
 
+# only for reference now
 def wrap_deepmind(env_id, episode_life=True, clip_rewards=True, frame_stack=4, scale=True, warp_frame=True):
     """Configure environment for DeepMind-style Atari. The observation is
     channel-first: (c, h, w) instead of (h, w, c).
 
     :param str env_id: the atari environment id.
     :param bool episode_life: wrap the episode life wrapper.
     :param bool clip_rewards: wrap the reward clipping wrapper.
@@ -38,14 +42,15 @@
     if clip_rewards:
         env = ClipRewardWrapper(env)
     if frame_stack:
         env = FrameStackWrapper(env, frame_stack)
     return env
 
 
+# only for reference now
 def wrap_deepmind_mr(env_id, episode_life=True, clip_rewards=True, frame_stack=4, scale=True, warp_frame=True):
     """Configure environment for DeepMind-style Atari. The observation is
     channel-first: (c, h, w) instead of (h, w, c).
 
     :param str env_id: the atari environment id.
     :param bool episode_life: wrap the episode life wrapper.
     :param bool clip_rewards: wrap the reward clipping wrapper.
@@ -69,63 +74,74 @@
     if clip_rewards:
         env = ClipRewardWrapper(env)
     if frame_stack:
         env = FrameStackWrapper(env, frame_stack)
     return env
 
 
-def wrap_lightzero(config, episode_life, clip_rewards):
+def wrap_lightzero(config: EasyDict, episode_life: bool, clip_rewards: bool) -> gym.Env:
     """
     Overview:
         Configure environment for MuZero-style Atari. The observation is
         channel-first: (c, h, w) instead of (h, w, c).
     Arguments:
-        - config (:obj:`Dict`): Dict containing configuration.
-        - wrap_frame (:obj:`bool`):
-        - save_video (:obj:`bool`):
-        - save_path (:obj:`bool`):
+        - config (:obj:`Dict`): Dict containing configuration parameters for the environment.
+        - episode_life (:obj:`bool`): If True, the agent starts with a set number of lives and loses them during the game.
+        - clip_rewards (:obj:`bool`): If True, the rewards are clipped to a certain range.
     Return:
-        - the wrapped atari environment.
+        - env (:obj:`gym.Env`): The wrapped Atari environment with the given configurations.
     """
     if config.render_mode_human:
-        env = gym.make(config.env_name, render_mode='human')
+        env = gymnasium.make(config.env_id, render_mode='human')
     else:
-        env = gym.make(config.env_name)
+        env = gymnasium.make(config.env_id, render_mode='rgb_array')
     assert 'NoFrameskip' in env.spec.id
+    if hasattr(config, 'save_replay') and config.save_replay \
+            and hasattr(config, 'replay_path') and config.replay_path is not None:
+        timestamp = datetime.now().strftime("%Y%m%d%H%M%S")
+        video_name = f'{env.spec.id}-video-{timestamp}'
+        env = RecordVideo(
+            env,
+            video_folder=config.replay_path,
+            episode_trigger=lambda episode_id: True,
+            name_prefix=video_name
+        )
+    env = GymnasiumToGymWrapper(env)
     env = NoopResetWrapper(env, noop_max=30)
     env = MaxAndSkipWrapper(env, skip=config.frame_skip)
     if episode_life:
         env = EpisodicLifeWrapper(env)
     env = TimeLimit(env, max_episode_steps=config.max_episode_steps)
     if config.warp_frame:
         # we must set WarpFrame before ScaledFloatFrameWrapper
         env = WarpFrame(env, width=config.obs_shape[1], height=config.obs_shape[2], grayscale=config.gray_scale)
     if config.scale:
         env = ScaledFloatFrameWrapper(env)
     if clip_rewards:
         env = ClipRewardWrapper(env)
-    if config.save_video:
-        import random, string
-        env = RecordVideo(
-            env,
-            video_folder=config.save_path,
-            episode_trigger=lambda episode_id: True,
-            name_prefix='rl-video-{}'.format(''.join(random.choice(string.ascii_lowercase) for i in range(5))),
-        )
 
     env = JpegWrapper(env, transform2string=config.transform2string)
     if config.game_wrapper:
         env = GameWrapper(env)
 
     return env
 
 
 class TimeLimit(gym.Wrapper):
+    """
+    Overview:
+        A wrapper that limits the maximum number of steps in an episode.
+    """
 
-    def __init__(self, env, max_episode_steps=None):
+    def __init__(self, env: gym.Env, max_episode_steps: Optional[int] = None):
+        """
+        Arguments:
+            - env (:obj:`gym.Env`): The environment to wrap.
+            - max_episode_steps (:obj:`Optional[int]`): Maximum number of steps per episode. If None, no limit is applied.
+        """
         super(TimeLimit, self).__init__(env)
         self._max_episode_steps = max_episode_steps
         self._elapsed_steps = 0
 
     def step(self, ac):
         observation, reward, done, info = self.env.step(ac)
         self._elapsed_steps += 1
@@ -136,20 +152,28 @@
 
     def reset(self, **kwargs):
         self._elapsed_steps = 0
         return self.env.reset(**kwargs)
 
 
 class WarpFrame(gym.ObservationWrapper):
+    """
+    Overview:
+        A wrapper that warps frames to 84x84 as done in the Nature paper and later work.
+    """
 
-    def __init__(self, env, width=84, height=84, grayscale=True, dict_space_key=None):
+    def __init__(self, env: gym.Env, width: int = 84, height: int = 84, grayscale: bool = True,
+                 dict_space_key: Optional[str] = None):
         """
-        Warp frames to 84x84 as done in the Nature paper and later work.
-        If the environment uses dictionary observations, `dict_space_key` can be specified which indicates which
-        observation should be warped.
+        Arguments:
+            - env (:obj:`gym.Env`): The environment to wrap.
+            - width (:obj:`int`): The width to which the frames are resized.
+            - height (:obj:`int`): The height to which the frames are resized.
+            - grayscale (:obj:`bool`): If True, convert frames to grayscale.
+            - dict_space_key (:obj:`Optional[str]`): If specified, indicates which observation should be warped.
         """
         super().__init__(env)
         self._width = width
         self._height = height
         self._grayscale = grayscale
         self._key = dict_space_key
         if self._grayscale:
@@ -188,18 +212,24 @@
         else:
             obs = obs.copy()
             obs[self._key] = frame
         return obs
 
 
 class JpegWrapper(gym.Wrapper):
+    """
+    Overview:
+        A wrapper that converts the observation into a string to save memory.
+    """
 
-    def __init__(self, env, transform2string=True):
+    def __init__(self, env: gym.Env, transform2string: bool = True):
         """
-        Overview: convert the observation into string to save memory
+        Arguments:
+            - env (:obj:`gym.Env`): The environment to wrap.
+            - transform2string (:obj:`bool`): If True, transform the observations to string.
         """
         super().__init__(env)
         self.transform2string = transform2string
 
     def step(self, action):
         observation, reward, done, info = self.env.step(action)
 
@@ -214,16 +244,66 @@
         if self.transform2string:
             observation = jpeg_data_compressor(observation)
 
         return observation
 
 
 class GameWrapper(gym.Wrapper):
+    """
+    Overview:
+        A wrapper to adapt the environment to the game interface.
+    """
 
-    def __init__(self, env):
+    def __init__(self, env: gym.Env):
         """
-        Overview: warp env to adapt the game interface
+        Arguments:
+            - env (:obj:`gym.Env`): The environment to wrap.
         """
         super().__init__(env)
 
     def legal_actions(self):
         return [_ for _ in range(self.env.action_space.n)]
+
+class GymnasiumToGymWrapper(gym.Wrapper):
+    """
+    Overview:
+        A wrapper class that adapts a Gymnasium environment to the Gym interface.
+    Interface:
+        ``__init__``, ``reset``, ``seed``
+    Properties:
+        - _seed (:obj:`int` or None): The seed value for the environment.
+    """
+
+    def __init__(self, env):
+        """
+        Overview:
+            Initializes the GymnasiumToGymWrapper.
+        Arguments:
+            - env (:obj:`gymnasium.Env`): The Gymnasium environment to be wrapped.
+        """
+
+        assert isinstance(env, gymnasium.Env), type(env)
+        super().__init__(env)
+        self._seed = None
+
+    def seed(self, seed):
+        """
+        Overview:
+            Sets the seed value for the environment.
+        Arguments:
+            - seed (:obj:`int`): The seed value to use for random number generation.
+        """
+        self._seed = seed
+
+    def reset(self):
+        """
+        Overview:
+            Resets the environment and returns the initial observation.
+        Returns:
+            - observation (:obj:`Any`): The initial observation of the environment.
+        """
+        if self._seed is not None:
+            obs, _ = self.env.reset(seed=self._seed)
+            return obs
+        else:
+            obs, _ = self.env.reset()
+            return obs
```

### Comparing `LightZero-0.0.2/zoo/board_games/alphabeta_pruning_bot.py` & `LightZero-0.0.5/zoo/board_games/alphabeta_pruning_bot.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,15 +157,15 @@
     from zoo.board_games.tictactoe.envs.tictactoe_env import TicTacToeEnv
     cfg = dict(
         prob_random_agent=0,
         prob_expert_agent=0,
         battle_mode='self_play_mode',
         agent_vs_human=False,
         bot_action_type='alpha_beta_pruning',  # {'v0', 'alpha_beta_pruning'}
-        channel_last=True,
+        channel_last=False,
         scale=True,
     )
     env = TicTacToeEnv(EasyDict(cfg))
     player_0 = AlphaBetaPruningBot(TicTacToeEnv, cfg, 'player 1')  # player_index = 0, player = 1
     player_1 = AlphaBetaPruningBot(TicTacToeEnv, cfg, 'player 2')  # player_index = 1, player = 2
 
     ### test from the init empty board ###
@@ -212,15 +212,15 @@
     from zoo.board_games.gomoku.envs.gomoku_env import GomokuEnv
     cfg = dict(
         board_size=5,
         prob_random_agent=0,
         prob_expert_agent=0,
         battle_mode='self_play_mode',
         scale=True,
-        channel_last=True,
+        channel_last=False,
         agent_vs_human=False,
         bot_action_type='alpha_beta_pruning',  # {'v0', 'alpha_beta_pruning'}
         prob_random_action_in_bot=0.,
         check_action_to_connect4_in_bot_v0=False,
     )
     env = GomokuEnv(EasyDict(cfg))
     player_0 = AlphaBetaPruningBot(GomokuEnv, cfg, 'player 1')  # player_index = 0, player = 1
```

### Comparing `LightZero-0.0.2/zoo/board_games/classic_search_algorithm/alphabeta_pruning.py` & `LightZero-0.0.5/zoo/board_games/classic_search_algorithm/alphabeta_pruning.py`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/zoo/board_games/classic_search_algorithm/alphabeta_pruning_return_best_subtree.py` & `LightZero-0.0.5/zoo/board_games/classic_search_algorithm/alphabeta_pruning_return_best_subtree.py`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/zoo/board_games/classic_search_algorithm/minimax_v0.py` & `LightZero-0.0.5/zoo/board_games/classic_search_algorithm/minimax_v0.py`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/zoo/board_games/classic_search_algorithm/minimax_v1.py` & `LightZero-0.0.5/zoo/board_games/classic_search_algorithm/minimax_v1.py`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/zoo/board_games/go/envs/go_env.py` & `LightZero-0.0.5/zoo/board_games/go/envs/go_env.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 import sys
 
 import numpy as np
 import pygame
 from ding.envs import BaseEnv, BaseEnvTimestep
 from ding.utils import ENV_REGISTRY
-from gym import spaces
+from gymnasium import spaces
 from pettingzoo.classic.go import coords, go
 from pettingzoo.utils.agent_selector import agent_selector
 
 
 def get_image(path):
     from os import path as os_path
```

### Comparing `LightZero-0.0.2/zoo/board_games/go/envs/test_go_env.py` & `LightZero-0.0.5/zoo/board_games/go/envs/test_go_env.py`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/zoo/board_games/gomoku/config/gomoku_alphazero_bot_mode_config.py` & `LightZero-0.0.5/zoo/board_games/gomoku/config/gomoku_alphazero_sp_mode_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 from easydict import EasyDict
 
 # ==============================================================
 # begin of the most frequently changed config specified by the user
 # ==============================================================
 board_size = 6  # default_size is 15
-collector_env_num = 8
-n_episode = 8
-evaluator_env_num = 3
+collector_env_num = 32
+n_episode = 32
+evaluator_env_num = 5
 num_simulations = 50
 update_per_collect = 50
 batch_size = 256
 max_env_step = int(5e5)
 prob_random_action_in_bot = 0.5
 mcts_ctree = True
 # ==============================================================
 # end of the most frequently changed config specified by the user
 # ==============================================================
 gomoku_alphazero_config = dict(
     exp_name=
-    f'data_az_ptree/gomoku_alphazero_bot-mode_rand{prob_random_action_in_bot}_ns{num_simulations}_upc{update_per_collect}_seed0',
+    f'data_az_ctree/gomoku_alphazero_sp-mode_rand{prob_random_action_in_bot}_ns{num_simulations}_upc{update_per_collect}_seed0',
     env=dict(
         board_size=board_size,
-        battle_mode='play_with_bot_mode',
+        battle_mode='self_play_mode',
         bot_action_type='v1',
         prob_random_action_in_bot=prob_random_action_in_bot,
         channel_last=False,
         collector_env_num=collector_env_num,
         evaluator_env_num=evaluator_env_num,
         n_evaluator_episode=evaluator_env_num,
         manager=dict(shared_memory=False, ),
         # ==============================================================
         # for the creation of simulation env
         agent_vs_human=False,
         prob_random_agent=0,
         prob_expert_agent=0,
         scale=True,
-        check_action_to_connect4_in_bot_v0=False,
-        mcts_ctree=mcts_ctree,
         screen_scaling=9,
         render_mode=None,
+        replay_path=None,
+        alphazero_mcts_ctree=mcts_ctree,
         # ==============================================================
     ),
     policy=dict(
         mcts_ctree=mcts_ctree,
         # ==============================================================
         # for the creation of simulation env
-        simulation_env_name='gomoku',
-        simulation_env_config_type='play_with_bot',
+        simulation_env_id='gomoku',
+        simulation_env_config_type='self_play',
         # ==============================================================
         torch_compile=False,
         tensor_float_32=False,
         model=dict(
             observation_shape=(3, board_size, board_size),
             action_space_size=int(1 * board_size * board_size),
             num_res_blocks=1,
@@ -59,14 +59,15 @@
         cuda=True,
         board_size=board_size,
         update_per_collect=update_per_collect,
         batch_size=batch_size,
         optim_type='Adam',
         lr_piecewise_constant_decay=False,
         learning_rate=0.003,
+        manual_temperature_decay=True,
         grad_clip_value=0.5,
         value_weight=1.0,
         entropy_weight=0.0,
         n_episode=n_episode,
         eval_freq=int(2e3),
         mcts=dict(num_simulations=num_simulations),
         collector_env_num=collector_env_num,
```

### Comparing `LightZero-0.0.2/zoo/board_games/gomoku/config/gomoku_alphazero_sp_mode_config.py` & `LightZero-0.0.5/zoo/board_games/gomoku/config/gomoku_gumbel_alphazero_bot_mode_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,48 +4,57 @@
 # begin of the most frequently changed config specified by the user
 # ==============================================================
 board_size = 6  # default_size is 15
 collector_env_num = 32
 n_episode = 32
 evaluator_env_num = 5
 num_simulations = 50
-update_per_collect = 50
+update_per_collect = 100
 batch_size = 256
 max_env_step = int(5e5)
 prob_random_action_in_bot = 0.5
+mcts_ctree = True
+
 # ==============================================================
 # end of the most frequently changed config specified by the user
 # ==============================================================
-gomoku_alphazero_config = dict(
-    exp_name=
-    f'data_az_ptree/gomoku_alphazero_sp-mode_rand{prob_random_action_in_bot}_ns{num_simulations}_upc{update_per_collect}_seed0',
+gomoku_gumbel_alphazero_config = dict(
+    exp_name=f'data_gaz_ctree/gomoku_gumbel_alphazero_bot-mode_rand{prob_random_action_in_bot}_ns{num_simulations}_upc{update_per_collect}_seed0',
     env=dict(
+        stop_value=2,
         board_size=board_size,
-        battle_mode='self_play_mode',
-        bot_action_type='v0',
+        battle_mode='play_with_bot_mode',
+        bot_action_type='v1',
         prob_random_action_in_bot=prob_random_action_in_bot,
-        channel_last=False,  # NOTE
+        channel_last=False,
         collector_env_num=collector_env_num,
         evaluator_env_num=evaluator_env_num,
         n_evaluator_episode=evaluator_env_num,
         manager=dict(shared_memory=False, ),
         # ==============================================================
         # for the creation of simulation env
         agent_vs_human=False,
         prob_random_agent=0,
         prob_expert_agent=0,
         scale=True,
-        check_action_to_connect4_in_bot_v0=False,
+        screen_scaling=9,
+        render_mode=None,
+        replay_path=None,
+        alphazero_mcts_ctree=mcts_ctree,
         # ==============================================================
     ),
     policy=dict(
+        mcts_ctree=mcts_ctree,
+        env_type='board_games',
+        action_type='varied_action_space',
         # ==============================================================
         # for the creation of simulation env
-        simulation_env_name='gomoku',
-        simulation_env_config_type='self_play',
+        simulation_env_id='gomoku',
+        simulation_env_config_type='play_with_bot',
+        alphazero_mcts_ctree=mcts_ctree,
         # ==============================================================
         torch_compile=False,
         tensor_float_32=False,
         model=dict(
             observation_shape=(3, board_size, board_size),
             action_space_size=int(1 * board_size * board_size),
             num_res_blocks=1,
@@ -54,41 +63,41 @@
         cuda=True,
         board_size=board_size,
         update_per_collect=update_per_collect,
         batch_size=batch_size,
         optim_type='Adam',
         lr_piecewise_constant_decay=False,
         learning_rate=0.003,
-        manual_temperature_decay=True,
         grad_clip_value=0.5,
         value_weight=1.0,
         entropy_weight=0.0,
         n_episode=n_episode,
         eval_freq=int(2e3),
         mcts=dict(num_simulations=num_simulations),
         collector_env_num=collector_env_num,
         evaluator_env_num=evaluator_env_num,
     ),
 )
 
-gomoku_alphazero_config = EasyDict(gomoku_alphazero_config)
-main_config = gomoku_alphazero_config
+gomoku_gumbel_alphazero_config = EasyDict(gomoku_gumbel_alphazero_config)
+main_config = gomoku_gumbel_alphazero_config
 
 gomoku_alphazero_create_config = dict(
     env=dict(
         type='gomoku',
         import_names=['zoo.board_games.gomoku.envs.gomoku_env'],
     ),
     env_manager=dict(type='subprocess'),
     policy=dict(
-        type='alphazero',
-        import_names=['lzero.policy.alphazero'],
+        type='gumbel_alphazero',
+        import_names=['lzero.policy.gumbel_alphazero'],
     ),
     collector=dict(
         type='episode_alphazero',
+        get_train_sample=False,
         import_names=['lzero.worker.alphazero_collector'],
     ),
     evaluator=dict(
         type='alphazero',
         import_names=['lzero.worker.alphazero_evaluator'],
     )
 )
@@ -102,8 +111,8 @@
         # The flag below controls whether to allow TF32 on matmul. This flag defaults to False
         # in PyTorch 1.12 and later.
         torch.backends.cuda.matmul.allow_tf32 = True
         # The flag below controls whether to allow TF32 on cuDNN. This flag defaults to True.
         torch.backends.cudnn.allow_tf32 = True
 
     from lzero.entry import train_alphazero
-    train_alphazero([main_config, create_config], seed=0, max_env_step=max_env_step)
+    train_alphazero([main_config, create_config], seed=0, max_env_step=max_env_step)
```

### Comparing `LightZero-0.0.2/zoo/board_games/gomoku/config/gomoku_gumbel_muzero_bot_mode_config.py` & `LightZero-0.0.5/zoo/board_games/gomoku/config/gomoku_gumbel_muzero_bot_mode_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
             num_channels=32,
             support_scale=10,
             reward_support_size=21,
             value_support_size=21,
         ),
         cuda=True,
         env_type='board_games',
+        action_type='varied_action_space',
         game_segment_length=int(board_size * board_size / 2),  # for battle_mode='play_with_bot_mode'
         update_per_collect=update_per_collect,
         batch_size=batch_size,
         optim_type='Adam',
         lr_piecewise_constant_decay=False,
         learning_rate=0.003,
         grad_clip_value=0.5,
```

### Comparing `LightZero-0.0.2/zoo/board_games/gomoku/config/gomoku_muzero_bot_mode_config.py` & `LightZero-0.0.5/zoo/board_games/gomoku/config/gomoku_muzero_bot_mode_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,15 @@
             num_channels=32,
             support_scale=10,
             reward_support_size=21,
             value_support_size=21,
         ),
         cuda=True,
         env_type='board_games',
+        action_type='varied_action_space',
         game_segment_length=int(board_size * board_size / 2),  # for battle_mode='play_with_bot_mode'
         update_per_collect=update_per_collect,
         batch_size=batch_size,
         optim_type='Adam',
         lr_piecewise_constant_decay=False,
         learning_rate=0.003,
         grad_clip_value=0.5,
@@ -81,9 +82,8 @@
     ),
 )
 gomoku_muzero_create_config = EasyDict(gomoku_muzero_create_config)
 create_config = gomoku_muzero_create_config
 
 if __name__ == "__main__":
     from lzero.entry import train_muzero
-
     train_muzero([main_config, create_config], seed=0, max_env_step=max_env_step)
```

### Comparing `LightZero-0.0.2/zoo/board_games/gomoku/config/gomoku_muzero_sp_mode_config.py` & `LightZero-0.0.5/zoo/board_games/gomoku/config/gomoku_muzero_sp_mode_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
             num_channels=32,
             support_scale=10,
             reward_support_size=21,
             value_support_size=21,
         ),
         cuda=True,
         env_type='board_games',
+        action_type='varied_action_space',
         game_segment_length=int(board_size * board_size),  # for battle_mode='self_play_mode'
         update_per_collect=update_per_collect,
         batch_size=batch_size,
         optim_type='Adam',
         lr_piecewise_constant_decay=False,
         learning_rate=0.003,
         grad_clip_value=0.5,
```

### Comparing `LightZero-0.0.2/zoo/board_games/gomoku/config/gomoku_sampled_alphazero_bot_mode_config.py` & `LightZero-0.0.5/zoo/board_games/gomoku/config/gomoku_sampled_alphazero_bot_mode_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,24 +38,25 @@
         # ==============================================================
         # for the creation of simulation env
         agent_vs_human=False,
         prob_random_agent=0,
         prob_expert_agent=0,
         scale=True,
         check_action_to_connect4_in_bot_v0=False,
-        simulation_env_name="gomoku",
-        # ==============================================================
-        mcts_ctree=mcts_ctree,
+        simulation_env_id="gomoku",
         screen_scaling=9,
         render_mode=None,
+        replay_path=None,
+        alphazero_mcts_ctree=mcts_ctree,
+        # ==============================================================
     ),
     policy=dict(
         # ==============================================================
         # for the creation of simulation env
-        simulation_env_name='gomoku',
+        simulation_env_id='gomoku',
         simulation_env_config_type='sampled_play_with_bot',
         # ==============================================================
         torch_compile=False,
         tensor_float_32=False,
         model=dict(
             observation_shape=(3, board_size, board_size),
             action_space_size=int(1 * board_size * board_size),
```

### Comparing `LightZero-0.0.2/zoo/board_games/gomoku/config/gomoku_sampled_alphazero_sp_mode_config.py` & `LightZero-0.0.5/zoo/board_games/gomoku/config/gomoku_sampled_alphazero_sp_mode_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,24 +34,25 @@
         # ==============================================================
         # for the creation of simulation env
         agent_vs_human=False,
         prob_random_agent=0,
         prob_expert_agent=0,
         scale=True,
         check_action_to_connect4_in_bot_v0=False,
-        simulation_env_name="gomoku",
-        # ==============================================================
-        mcts_ctree=mcts_ctree,
+        simulation_env_id="gomoku",
         screen_scaling=9,
         render_mode=None,
+        replay_path=None,
+        alphazero_mcts_ctree=mcts_ctree,
+        # ==============================================================
     ),
     policy=dict(
         # ==============================================================
         # for the creation of simulation env
-        simulation_env_name='gomoku',
+        simulation_env_id='gomoku',
         simulation_env_config_type='sampled_self_play',
         # ==============================================================
         torch_compile=False,
         tensor_float_32=False,
         model=dict(
             observation_shape=(3, board_size, board_size),
             action_space_size=int(1 * board_size * board_size),
```

### Comparing `LightZero-0.0.2/zoo/board_games/gomoku/entry/gomoku_alphazero_eval.py` & `LightZero-0.0.5/zoo/board_games/gomoku/entry/gomoku_muzero_eval.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,30 @@
-from zoo.board_games.gomoku.config.gomoku_alphazero_bot_mode_config import main_config, create_config
-from lzero.entry import eval_alphazero
+from zoo.board_games.gomoku.config.gomoku_muzero_bot_mode_config import main_config, create_config
+from lzero.entry import eval_muzero
 import numpy as np
 
 if __name__ == '__main__':
     """ 
     model_path (:obj:`Optional[str]`): The pretrained model path, which should
     point to the ckpt file of the pretrained model, and an absolute path is recommended.
     In LightZero, the path is usually something like ``exp_name/ckpt/ckpt_best.pth.tar``.
     """
     model_path = './ckpt/ckpt_best.pth.tar'
     seeds = [0]
     num_episodes_each_seed = 5
     # If True, you can play with the agent.
-    main_config.env.agent_vs_human = True
-    main_config.env.render_mode = 'image_realtime_mode'
+    main_config.env.agent_vs_human = False
     create_config.env_manager.type = 'base'
     main_config.env.evaluator_env_num = 1
     main_config.env.n_evaluator_episode = 1
     total_test_episodes = num_episodes_each_seed * len(seeds)
     returns_mean_seeds = []
     returns_seeds = []
     for seed in seeds:
-        returns_mean, returns = eval_alphazero(
+        returns_mean, returns = eval_muzero(
             [main_config, create_config],
             seed=seed,
             num_episodes_each_seed=num_episodes_each_seed,
             print_seed_details=True,
             model_path=model_path
         )
         returns_mean_seeds.append(returns_mean)
```

### Comparing `LightZero-0.0.2/zoo/board_games/gomoku/entry/gomoku_gumbel_muzero_eval.py` & `LightZero-0.0.5/zoo/board_games/gomoku/entry/gomoku_gumbel_muzero_eval.py`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/zoo/board_games/gomoku/entry/gomoku_muzero_eval.py` & `LightZero-0.0.5/zoo/board_games/gomoku/entry/gomoku_sampled_alphazero_eval.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,34 @@
-from zoo.board_games.gomoku.config.gomoku_muzero_bot_mode_config import main_config, create_config
-from lzero.entry import eval_muzero
+from zoo.board_games.gomoku.config.gomoku_sampled_alphazero_bot_mode_config import main_config, create_config
+from lzero.entry import eval_alphazero
 import numpy as np
 
 if __name__ == '__main__':
     """ 
     model_path (:obj:`Optional[str]`): The pretrained model path, which should
     point to the ckpt file of the pretrained model, and an absolute path is recommended.
     In LightZero, the path is usually something like ``exp_name/ckpt/ckpt_best.pth.tar``.
     """
-    model_path = './ckpt/ckpt_best.pth.tar'
+    # model_path = './ckpt/ckpt_best.pth.tar'
+    model_path = None
     seeds = [0]
-    num_episodes_each_seed = 5
+    num_episodes_each_seed = 1
     # If True, you can play with the agent.
-    main_config.env.agent_vs_human = False
+    main_config.env.agent_vs_human = True
+    main_config.env.battle_mode = 'eval_mode'
+    main_config.env.render_mode = 'image_realtime_mode'
     create_config.env_manager.type = 'base'
+    main_config.env.collector_env_num = 1
     main_config.env.evaluator_env_num = 1
     main_config.env.n_evaluator_episode = 1
     total_test_episodes = num_episodes_each_seed * len(seeds)
     returns_mean_seeds = []
     returns_seeds = []
     for seed in seeds:
-        returns_mean, returns = eval_muzero(
+        returns_mean, returns = eval_alphazero(
             [main_config, create_config],
             seed=seed,
             num_episodes_each_seed=num_episodes_each_seed,
             print_seed_details=True,
             model_path=model_path
         )
         returns_mean_seeds.append(returns_mean)
```

### Comparing `LightZero-0.0.2/zoo/board_games/gomoku/entry/gomoku_sampled_alphazero_eval.py` & `LightZero-0.0.5/zoo/classic_control/cartpole/entry/cartpole_eval.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,55 @@
-from zoo.board_games.gomoku.config.gomoku_sampled_alphazero_bot_mode_config import main_config, create_config
-from lzero.entry import eval_alphazero
+from zoo.classic_control.cartpole.config.cartpole_muzero_config import main_config, create_config
+from lzero.entry import eval_muzero
 import numpy as np
 
-if __name__ == '__main__':
-    """ 
-    model_path (:obj:`Optional[str]`): The pretrained model path, which should
-    point to the ckpt file of the pretrained model, and an absolute path is recommended.
-    In LightZero, the path is usually something like ``exp_name/ckpt/ckpt_best.pth.tar``.
+if __name__ == "__main__":
     """
-    # model_path = './ckpt/ckpt_best.pth.tar'
+    Entry point for the evaluation of the MuZero model on the CartPole environment. 
+
+    Variables:
+        - model_path (:obj:`Optional[str]`): The pretrained model path, which should point to the ckpt file of the 
+        pretrained model. An absolute path is recommended. In LightZero, the path is usually something like 
+        ``exp_name/ckpt/ckpt_best.pth.tar``.
+        - returns_mean_seeds (:obj:`List[float]`): List to store the mean returns for each seed.
+        - returns_seeds (:obj:`List[float]`): List to store the returns for each seed.
+        - seeds (:obj:`List[int]`): List of seeds for the environment.
+        - num_episodes_each_seed (:obj:`int`): Number of episodes to run for each seed.
+        - total_test_episodes (:obj:`int`): Total number of test episodes, computed as the product of the number of 
+        seeds and the number of episodes per seed.
+    """
+    # model_path = "./ckpt/ckpt_best.pth.tar"
     model_path = None
-    seeds = [0]
-    num_episodes_each_seed = 1
-    # If True, you can play with the agent.
-    main_config.env.agent_vs_human = True
-    main_config.env.battle_mode = 'eval_mode'
-    main_config.env.render_mode = 'image_realtime_mode'
-    create_config.env_manager.type = 'base'
-    main_config.env.collector_env_num = 1
-    main_config.env.evaluator_env_num = 1
-    main_config.env.n_evaluator_episode = 1
-    total_test_episodes = num_episodes_each_seed * len(seeds)
     returns_mean_seeds = []
     returns_seeds = []
+    seeds = [0]
+    num_episodes_each_seed = 2
+    total_test_episodes = num_episodes_each_seed * len(seeds)
+    create_config.env_manager.type = 'base'  # Visualization requires the 'type' to be set as base
+    main_config.env.evaluator_env_num = 1  # Visualization requires the 'env_num' to be set as 1
+    main_config.env.n_evaluator_episode = total_test_episodes
+    main_config.env.replay_path = './video'
+
     for seed in seeds:
-        returns_mean, returns = eval_alphazero(
+        """
+        - returns_mean (:obj:`float`): The mean return of the evaluation.
+        - returns (:obj:`List[float]`): The returns of the evaluation.
+        """
+        returns_mean, returns = eval_muzero(
             [main_config, create_config],
             seed=seed,
             num_episodes_each_seed=num_episodes_each_seed,
-            print_seed_details=True,
+            print_seed_details=False,
             model_path=model_path
         )
         returns_mean_seeds.append(returns_mean)
         returns_seeds.append(returns)
 
     returns_mean_seeds = np.array(returns_mean_seeds)
     returns_seeds = np.array(returns_seeds)
 
+    # Print evaluation results
     print("=" * 20)
-    print(f'We eval total {len(seeds)} seeds. In each seed, we eval {num_episodes_each_seed} episodes.')
-    print(f'In seeds {seeds}, returns_mean_seeds is {returns_mean_seeds}, returns is {returns_seeds}')
-    print('In all seeds, reward_mean:', returns_mean_seeds.mean(), end='. ')
-    print(
-        f'win rate: {len(np.where(returns_seeds == 1.)[0]) / total_test_episodes}, draw rate: {len(np.where(returns_seeds == 0.)[0]) / total_test_episodes}, lose rate: {len(np.where(returns_seeds == -1.)[0]) / total_test_episodes}'
-    )
-    print("=" * 20)
+    print(f"We evaluated a total of {len(seeds)} seeds. For each seed, we evaluated {num_episodes_each_seed} episode(s).")
+    print(f"For seeds {seeds}, the mean returns are {returns_mean_seeds}, and the returns are {returns_seeds}.")
+    print("Across all seeds, the mean reward is:", returns_mean_seeds.mean())
+    print("=" * 20)
```

### Comparing `LightZero-0.0.2/zoo/board_games/gomoku/envs/gomoku_env.py` & `LightZero-0.0.5/zoo/board_games/gomoku/envs/gomoku_env.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import copy
 import os
 import sys
+from datetime import datetime
 from functools import lru_cache
 from typing import List, Any
 
-import gym
+import gymnasium as gym
 import imageio
+import matplotlib
+matplotlib.use('Agg') 
 import matplotlib.patches as patches
 import matplotlib.pyplot as plt
 import numpy as np
 import pygame
 from ding.envs import BaseEnv, BaseEnvTimestep
 from ding.utils import ENV_REGISTRY
 from ditk import logging
@@ -38,44 +41,56 @@
     # Convert NumPy array to memory view.
     board_view = board_array.view(dtype=np.int32).reshape(board_array.shape)
     return get_done_winner_cython(board_size, board_view)
 
 
 @ENV_REGISTRY.register('gomoku')
 class GomokuEnv(BaseEnv):
+    """
+    Overview:
+        A Gomoku environment that inherits from the BaseEnv. This environment can be used for training and
+        evaluating AI players for the game of Gomoku.
+
+    .. note::
+        For the latest macOS, you should set context='spawn' or 'forkserver' in ding/envs/env_manager/subprocess_env_manager.py
+        to be able to use subprocess env_manager.
+    """
+
     config = dict(
         # (str) The name of the environment registered in the environment registry.
-        env_name="Gomoku",
+        env_id="Gomoku",
         # (int) The size of the board.
         board_size=6,
         # (str) The mode of the environment when take a step.
         battle_mode='self_play_mode',
         # (str) The mode of the environment when doing the MCTS.
-        mcts_mode='self_play_mode',  # only used in AlphaZero
+        battle_mode_in_simulation_env='self_play_mode',  # only used in AlphaZero
         # (str) The render mode. Options are 'None', 'state_realtime_mode', 'image_realtime_mode' or 'image_savefile_mode'.
         # If None, then the game will not be rendered.
         render_mode=None,
+        # (str or None) The directory in which to save the replay file. If None, the file is saved in the current directory.
+        replay_path=None,
         # (float) The scale of the render screen.
         screen_scaling=9,
         # (bool) Whether to use the 'channel last' format for the observation space. If False, 'channel first' format is used.
         channel_last=False,
         # (bool) Whether to scale the observation.
         scale=True,
         # (bool) Whether to let human to play with the agent when evaluating. If False, then use the bot to evaluate the agent.
         agent_vs_human=False,
         # (str) The type of the bot of the environment.
         bot_action_type='v1',  # {'v0', 'v1', 'alpha_beta_pruning'}, 'v1' is faster and stronger than 'v0' now.
         # (float) The probability that a random agent is used instead of the learning agent.
         prob_random_agent=0,
         # (float) The probability that a random action will be taken when calling the bot.
         prob_random_action_in_bot=0.,
-        # (bool) Whether to check the action to connect 4 in the bot v0.
-        check_action_to_connect4_in_bot_v0=False,
         # (float) The stop value when training the agent. If the evalue return reach the stop value, then the training will stop.
         stop_value=2,
+        # (bool) Whether to use the MCTS ctree in AlphaZero. If True, then the AlphaZero MCTS ctree will be used.
+        alphazero_mcts_ctree=False,
     )
 
     @classmethod
     def default_config(cls: type) -> EasyDict:
         cfg = EasyDict(copy.deepcopy(cls.config))
         cfg.cfg_type = cls.__name__ + 'Dict'
         return cfg
@@ -106,60 +121,83 @@
 
     def __init__(self, cfg: dict = None):
         self.cfg = cfg
         self.battle_mode = cfg.battle_mode
         # The mode of interaction between the agent and the environment.
         assert self.battle_mode in ['self_play_mode', 'play_with_bot_mode', 'eval_mode']
         # The mode of MCTS is only used in AlphaZero.
-        self.mcts_mode = 'self_play_mode'
+        self.battle_mode_in_simulation_env = 'self_play_mode'
 
         self.board_size = cfg.board_size
         self.prob_random_agent = cfg.prob_random_agent
         self.prob_random_action_in_bot = cfg.prob_random_action_in_bot
         self.channel_last = cfg.channel_last
         self.scale = cfg.scale
-        self.check_action_to_connect4_in_bot_v0 = cfg.check_action_to_connect4_in_bot_v0
         self.agent_vs_human = cfg.agent_vs_human
         self.bot_action_type = cfg.bot_action_type
 
         # Set the parameters about replay render.
         self.screen_scaling = cfg.screen_scaling
         # options = {None, 'state_realtime_mode', 'image_realtime_mode', 'image_savefile_mode'}
         self.render_mode = cfg.render_mode
-        self.replay_name_suffix = "test"
-        self.replay_path = None
-        self.replay_format = 'gif'  # 'mp4' #
+        assert self.render_mode in [None, 'state_realtime_mode', 'image_realtime_mode', 'image_savefile_mode']
+        self.replay_name_suffix = "" if hasattr(cfg, 'replay_name_suffix') is False else cfg.replay_name_suffix
+        self.replay_path = cfg.replay_path
+        self.replay_format = 'gif' if hasattr(cfg, 'replay_format') is False else cfg.replay_format
+        assert self.replay_format in ['gif', 'mp4']
         self.screen = None
         self.frames = []
 
         self.players = [1, 2]
         self._current_player = 1
         self.board_markers = [str(i + 1) for i in range(self.board_size)]
         self.total_num_actions = self.board_size * self.board_size
         self.gomoku_rule_bot_v1 = GomokuRuleBotV1()
         self._env = self
 
         if self.bot_action_type == 'alpha_beta_pruning':
             self.alpha_beta_pruning_player = AlphaBetaPruningBot(self, cfg, 'alpha_beta_pruning_player')
         elif self.bot_action_type == 'v0':
             self.rule_bot = GomokuRuleBotV0(self, self._current_player)
+        self.alphazero_mcts_ctree = cfg.alphazero_mcts_ctree
+        if not self.alphazero_mcts_ctree:
+            # plt is not work in mcts_ctree mode
+            self.fig, self.ax = plt.subplots(figsize=(self.board_size, self.board_size))
+            plt.ion()
+        self._save_replay_count = 0
 
-        self.fig, self.ax = plt.subplots(figsize=(self.board_size, self.board_size))
-        plt.ion()
+    def reset(self, start_player_index=0, init_state=None, katago_policy_init=False, katago_game_state=None):
+        """
+        Overview:
+            This method resets the environment and optionally starts with a custom state specified by 'init_state'.
+        Arguments:
+            - start_player_index (:obj:`int`, optional): Specifies the starting player. The players are [1,2] and
+                their corresponding indices are [0,1]. Defaults to 0.
+            - init_state (:obj:`Any`, optional): The custom starting state. If provided, the game starts from this state.
+                Defaults to None.
+            - katago_policy_init (:obj:`bool`, optional): This parameter is used to maintain compatibility with the
+                handling of 'katago' related parts in 'alphazero_mcts_ctree' in Go. Defaults to False.
+            - katago_game_state (:obj:`Any`, optional): This parameter is similar to 'katago_policy_init' and is used to
+                maintain compatibility with 'katago' in 'alphazero_mcts_ctree'. Defaults to None.
+        """
+        if self.alphazero_mcts_ctree and init_state is not None:
+            # Convert byte string to np.ndarray
+            init_state = np.frombuffer(init_state, dtype=np.int32)
 
-    def reset(self, start_player_index=0, init_state=None):
         self._observation_space = gym.spaces.Box(
             low=0, high=2, shape=(self.board_size, self.board_size, 3), dtype=np.int32
         )
         self._action_space = gym.spaces.Discrete(self.board_size ** 2)
         self._reward_space = gym.spaces.Box(low=0, high=1, shape=(1,), dtype=np.float32)
         self.start_player_index = start_player_index
         self._current_player = self.players[self.start_player_index]
         if init_state is not None:
             self.board = np.array(copy.deepcopy(init_state), dtype="int32")
+            if self.alphazero_mcts_ctree:
+                self.board = self.board.reshape((self.board_size, self.board_size))
         else:
             self.board = np.zeros((self.board_size, self.board_size), dtype="int32")
         action_mask = np.zeros(self.total_num_actions, 'int8')
         action_mask[self.legal_actions] = 1
         if self.battle_mode == 'play_with_bot_mode' or self.battle_mode == 'eval_mode':
             # In ``play_with_bot_mode`` and ``eval_mode``, we need to set the "to_play" parameter in the "obs" dict to -1,
             # because we don't take into account the alternation between players.
@@ -235,16 +273,18 @@
             # And the to_play is used in MCTS.
             timestep.obs['to_play'] = -1
             return timestep
 
         elif self.battle_mode == 'eval_mode':
             # player 1 battle with expert player 2
 
+            self._env.render(self.render_mode)
             # player 1's turn
             timestep_player1 = self._player_step(action)
+            self._env.render(self.render_mode)
             if self.agent_vs_human:
                 print('player 1 (agent): ' + self.action_to_string(action))  # Note: visualize
                 self.render(mode="image_realtime_mode")
 
             if timestep_player1.done:
                 # in eval_mode, we set to_play as None/-1, because we don't consider the alternation between players
                 timestep_player1.obs['to_play'] = -1
@@ -254,14 +294,15 @@
             if self.agent_vs_human:
                 bot_action = self.human_to_action()
             else:
                 bot_action = self.bot_action()
                 # bot_action = self.random_action()
 
             timestep_player2 = self._player_step(bot_action)
+            self._env.render(self.render_mode)
             if self.agent_vs_human:
                 print('player 2 (human): ' + self.action_to_string(bot_action))  # Note: visualize
                 self.render(mode="image_realtime_mode")
 
             # the eval_episode_return is calculated from Player 1's perspective
             timestep_player2.info['eval_episode_return'] = -timestep_player2.reward
             timestep_player2 = timestep_player2._replace(reward=-timestep_player2.reward)
@@ -291,23 +332,23 @@
         reward = np.array(float(winner == self.current_player)).astype(np.float32)
         info = {'next player to play': self.to_play}
         """
         NOTE: here exchange the player
         """
         self.current_player = self.to_play
 
-        # Render the new step.
-        # The following code is used to save the rendered images in both
-        # collect/eval step and the simulated mcts step.
+        # The following code will save the rendered images in both env step in collect/eval phase and the env step in
+        # simulated mcts.
         # if self.render_mode is not None:
         #     self.render(self.render_mode)
 
         if done:
             info['eval_episode_return'] = reward
-            if self.render_mode == 'image_savefile_mode':
+            self._env.render(self.render_mode)
+            if self.render_mode == 'image_savefile_mode' and self.replay_path is not None:
                 self.save_render_output(replay_name_suffix=self.replay_name_suffix, replay_path=self.replay_path,
                                         format=self.replay_format)
 
         action_mask = np.zeros(self.total_num_actions, 'int8')
         action_mask[self.legal_actions] = 1
         obs = {
             'observation': self.current_state()[1],
@@ -375,16 +416,14 @@
         action_list = self.legal_actions
         return np.random.choice(action_list)
 
     def bot_action(self):
         if np.random.rand() < self.prob_random_action_in_bot:
             return self.random_action()
         else:
-            # if self.bot_action_type == 'v0':
-            # return self.rule_bot_v0()
             if self.bot_action_type == 'v0':
                 return self.rule_bot.get_rule_bot_action(self.board, self._current_player)
             elif self.bot_action_type == 'v1':
                 return self.rule_bot_v1()
             elif self.bot_action_type == 'alpha_beta_pruning':
                 return self.bot_action_alpha_beta_pruning()
 
@@ -554,20 +593,22 @@
         Overview:
             The render method is used to draw the current state of the game. The rendering mode can be
             set according to the needs of the user.
         Arguments:
             - mode (str): Rendering mode, options are "state_realtime_mode", "image_realtime_mode",
               and "image_savefile_mode".
         """
+        if mode is None:
+            return
         # Print the state of the board directly
         if mode == "state_realtime_mode":
             print(np.array(self.board).reshape(self.board_size, self.board_size))
             return
         # Render the game as an image
-        elif mode == "image_realtime_mode" or mode == "image_savefile_mode":
+        elif mode == "image_realtime_mode" or (mode == "image_savefile_mode" and self.replay_path is not None):
             self.draw_board()
             # Draw the pieces on the board
             for x in range(self.board_size):
                 for y in range(self.board_size):
                     if self.board[x][y] == 1:  # Black piece
                         circle = patches.Circle((y + 1, x + 1), 0.4, edgecolor='black',
                                                 facecolor='black', zorder=3)
@@ -583,15 +624,22 @@
                 plt.draw()
                 plt.pause(0.1)
             # In savefile mode, save the current frame to the frames list
             elif mode == "image_savefile_mode":
                 # Save the current frame to the frames list.
                 self.fig.canvas.draw()
                 image = np.frombuffer(self.fig.canvas.tostring_rgb(), dtype='uint8')
-                image = image.reshape(self.fig.canvas.get_width_height()[::-1] + (3,))
+
+                # Get the width and height of the figure
+                width, height = self.fig.get_size_inches() * self.fig.get_dpi()
+                width = int(width)
+                height = int(height)
+                image = image.reshape(height, width, 3)
+
+                # image = image.reshape(self.fig.canvas.get_width_height()[::-1] + (3,))
                 self.frames.append(image)
 
     def close(self):
         """
         Overview:
             This method is used to display the final game board to the user and turn off interactive
             mode in matplotlib.
@@ -677,27 +725,45 @@
         Overview:
             Save the rendered frames as an output file.
         Arguments:
             - replay_name_suffix (:obj:`str`): The suffix to be added to the replay filename.
             - replay_path (:obj:`str`): The path to save the replay file. If None, the default filename will be used.
             - format (:obj:`str`): The format of the output file. Options are 'gif' or 'mp4'.
         """
+        timestamp = datetime.now().strftime("%Y%m%d%H%M%S")
+        
         # At the end of the episode, save the frames.
-        if replay_path is None:
-            filename = f'game_gomoku_{self.board_size}_{replay_name_suffix}.{format}'
+        if replay_name_suffix == '':
+            if replay_path is None:
+                filename = f'gomoku_{self.board_size}_{os.getpid()}_{timestamp}.{format}'
+            else:
+                if not os.path.exists(replay_path):
+                    os.makedirs(replay_path)
+                filename = os.path.join(
+                    replay_path,
+                    f'gomoku_{self.board_size}_{os.getpid()}_{timestamp}.{format}'
+                )
         else:
-            filename = f'{replay_path}.{format}'
+            if replay_path is None:
+                filename = f'gomoku_{self.board_size}_{replay_name_suffix}.{format}'
+            else:
+                if not os.path.exists(replay_path):
+                    os.makedirs(replay_path)
+                filename = replay_path+f'/gomoku_{self.board_size}_{replay_name_suffix}.{format}'
+
+        self._save_replay_count += 1
 
         if format == 'gif':
             # Save frames as a GIF with a duration of 0.1 seconds per frame.
             # imageio.mimsave(filename, self.frames, 'GIF', duration=0.1)
             imageio.mimsave(filename, self.frames, 'GIF', fps=30, subrectangles=True)
         elif format == 'mp4':
             # Save frames as an MP4 video with a frame rate of 30 frames per second.
-            imageio.mimsave(filename, self.frames, fps=30, codec='mpeg4')
+            # imageio.mimsave(filename, self.frames, fps=30, codec='mpeg4')
+            imageio.mimwrite(filename, self.frames, fps=30)
 
         else:
             raise ValueError("Unsupported format: {}".format(format))
         logging.info("Saved output to {}".format(filename))
         self.frames = []
 
     def render_naive(self, mode="human"):
@@ -758,14 +824,12 @@
         return "LightZero Gomoku Env"
 
     def close(self) -> None:
         pass
 
     def get_image(self, path: str) -> Any:
         from os import path as os_path
-        import pygame
-
         cwd = os_path.dirname(__file__)
         image = pygame.image.load(cwd + "/" + path)
         sfc = pygame.Surface(image.get_size(), flags=pygame.SRCALPHA)
         sfc.blit(image, (0, 0))
         return sfc
```

### Comparing `LightZero-0.0.2/zoo/board_games/gomoku/envs/gomoku_human_vs_bot_UI.py` & `LightZero-0.0.5/zoo/board_games/gomoku/envs/gomoku_human_vs_bot_UI.py`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/zoo/board_games/gomoku/envs/gomoku_rule_bot_v0.py` & `LightZero-0.0.5/zoo/board_games/gomoku/envs/gomoku_rule_bot_v0.py`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/zoo/board_games/gomoku/envs/gomoku_rule_bot_v1.py` & `LightZero-0.0.5/zoo/board_games/gomoku/envs/gomoku_rule_bot_v1.py`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/zoo/board_games/gomoku/envs/test_gomoku_alphabeta_pruning_bot.py` & `LightZero-0.0.5/zoo/board_games/gomoku/envs/test_gomoku_alphabeta_pruning_bot.py`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/zoo/board_games/gomoku/envs/test_gomoku_env.py` & `LightZero-0.0.5/zoo/board_games/gomoku/envs/test_gomoku_env.py`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/zoo/board_games/gomoku/envs/test_gomoku_mcts_bot.py` & `LightZero-0.0.5/zoo/board_games/gomoku/envs/test_gomoku_mcts_bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 cfg = dict(
     board_size=5,
     prob_random_agent=0,
     prob_expert_agent=0,
     battle_mode='self_play_mode',
     scale=True,
-    channel_last=True,
+    channel_last=False,
     agent_vs_human=False,
     bot_action_type='alpha_beta_pruning',  # {'v0', 'alpha_beta_pruning'}
     prob_random_action_in_bot=0.,
     check_action_to_connect4_in_bot_v0=False,
 )
```

### Comparing `LightZero-0.0.2/zoo/board_games/gomoku/envs/test_gomoku_rule_bot_v0.py` & `LightZero-0.0.5/zoo/board_games/gomoku/envs/test_gomoku_rule_bot_v0.py`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/zoo/board_games/gomoku/envs/test_gomoku_rule_bot_v1.py` & `LightZero-0.0.5/zoo/board_games/gomoku/envs/test_gomoku_rule_bot_v1.py`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/zoo/board_games/gomoku/envs/utils.py` & `LightZero-0.0.5/zoo/board_games/gomoku/envs/utils.py`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/zoo/board_games/gomoku/test/eval_get_done_winner.py` & `LightZero-0.0.5/zoo/board_games/gomoku/test/eval_get_done_winner.py`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/zoo/board_games/gomoku/test/eval_legal_actions.py` & `LightZero-0.0.5/zoo/board_games/gomoku/test/eval_legal_actions.py`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/zoo/board_games/gomoku/test/test_get_done_winner_cython.py` & `LightZero-0.0.5/zoo/board_games/gomoku/test/test_get_done_winner_cython.py`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/zoo/board_games/gomoku/test/test_gomoku_env_legal_actions.py` & `LightZero-0.0.5/zoo/board_games/gomoku/test/test_gomoku_env_legal_actions.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,20 @@
             prob_random_agent=0,
             channel_last=False,
             scale=True,
             agent_vs_human=False,
             bot_action_type='v0',
             prob_random_action_in_bot=0.,
             check_action_to_connect4_in_bot_v0=False,
+            prob_expert_agent=0,
+            simulation_env_id="gomoku",
+            screen_scaling=9,
+            render_mode=None,
+            replay_path=None,
+            alphazero_mcts_ctree=False,
         )
         env = GomokuEnv(cfg)
         obs = env.reset()
         print('init board state: ')
         env.render()
         gomoku_env_legal_actions_cython = 0
         gomoku_env_legal_actions_cython_lru = 0
```

### Comparing `LightZero-0.0.2/zoo/board_games/gomoku/test/test_legal_actions_cython.py` & `LightZero-0.0.5/zoo/board_games/gomoku/test/test_legal_actions_cython.py`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/zoo/board_games/mcts_bot.py` & `LightZero-0.0.5/zoo/board_games/mcts_bot.py`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/zoo/board_games/test_speed_win-rate_between_bots.py` & `LightZero-0.0.5/zoo/board_games/test_speed_win-rate_between_bots.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 cfg_tictactoe = dict(
     battle_mode='self_play_mode',
     agent_vs_human=False,
     bot_action_type='v0',  # {'v0', 'alpha_beta_pruning'}
     prob_random_agent=0,
     prob_expert_agent=0,
-    channel_last=True,
+    channel_last=False,
     scale=True,
     prob_random_action_in_bot=0.,
 )
 
 
 def test_tictactoe_mcts_bot_vs_rule_bot_v0_bot(num_simulations=50):
     """
@@ -427,15 +427,15 @@
 
 cfg_gomoku = dict(
     board_size=5,
     battle_mode='self_play_mode',
     bot_action_type='v0',  # {'v0', 'alpha_beta_pruning'}
     agent_vs_human=False,
     prob_random_agent=0,
-    channel_last=True,
+    channel_last=False,
     scale=True,
     prob_random_action_in_bot=0.,
     check_action_to_connect4_in_bot_v0=False,
 )
 
 
 def test_gomoku_mcts_bot_vs_rule_bot_v0_bot(num_simulations=50):
```

### Comparing `LightZero-0.0.2/zoo/board_games/tictactoe/config/tictactoe_alphazero_bot_mode_config.py` & `LightZero-0.0.5/zoo/board_games/tictactoe/config/tictactoe_alphazero_bot_mode_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,46 +6,49 @@
 collector_env_num = 8
 n_episode = 8
 evaluator_env_num = 5
 num_simulations = 25
 update_per_collect = 50
 batch_size = 256
 max_env_step = int(2e5)
-mcts_ctree = True
+mcts_ctree = False
+
 # ==============================================================
 # end of the most frequently changed config specified by the user
 # ==============================================================
 
 tictactoe_alphazero_config = dict(
     exp_name=f'data_az_ptree/tictactoe_alphazero_bot-mode_ns{num_simulations}_upc{update_per_collect}_seed0',
     env=dict(
         board_size=3,
         battle_mode='play_with_bot_mode',
         bot_action_type='v0',  # {'v0', 'alpha_beta_pruning'}
-        channel_last=False,  # NOTE
+        channel_last=False,
         collector_env_num=collector_env_num,
         evaluator_env_num=evaluator_env_num,
         n_evaluator_episode=evaluator_env_num,
         manager=dict(shared_memory=False, ),
         # ==============================================================
         # for the creation of simulation env
         agent_vs_human=False,
         prob_random_agent=0,
         prob_expert_agent=0,
         scale=True,
-        mcts_ctree=mcts_ctree,
+        alphazero_mcts_ctree=mcts_ctree,
+        save_replay_gif=False,
+        replay_path_gif='./replay_gif',
         # ==============================================================
     ),
     policy=dict(
+        mcts_ctree=mcts_ctree,
         # ==============================================================
         # for the creation of simulation env
-        simulation_env_name='tictactoe',
+        simulation_env_id='tictactoe',
         simulation_env_config_type='play_with_bot',
         # ==============================================================
-        mcts_ctree=mcts_ctree,
         model=dict(
             observation_shape=(3, 3, 3),
             action_space_size=int(1 * 3 * 3),
             # We use the small size model for tictactoe.
             num_res_blocks=1,
             num_channels=16,
             fc_value_layers=[8],
```

### Comparing `LightZero-0.0.2/zoo/board_games/tictactoe/config/tictactoe_alphazero_bot_mode_multigpu_ddp_config.py` & `LightZero-0.0.5/zoo/board_games/tictactoe/config/tictactoe_alphazero_bot_mode_multigpu_ddp_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         prob_expert_agent=0,
         scale=True,
         # ==============================================================
     ),
     policy=dict(
         # ==============================================================
         # for the creation of simulation env
-        simulation_env_name='tictactoe',
+        simulation_env_id='tictactoe',
         simulation_env_config_type='play_with_bot',
         # ==============================================================
         model=dict(
             observation_shape=(3, 3, 3),
             action_space_size=int(1 * 3 * 3),
             # We use the small size model for tictactoe.
             num_res_blocks=1,
```

### Comparing `LightZero-0.0.2/zoo/board_games/tictactoe/config/tictactoe_alphazero_sp_mode_config.py` & `LightZero-0.0.5/zoo/board_games/tictactoe/config/tictactoe_alphazero_sp_mode_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,40 +6,45 @@
 collector_env_num = 8
 n_episode = 8
 evaluator_env_num = 5
 num_simulations = 25
 update_per_collect = 50
 batch_size = 256
 max_env_step = int(2e5)
+mcts_ctree = True
 # ==============================================================
 # end of the most frequently changed config specified by the user
 # ==============================================================
 tictactoe_alphazero_config = dict(
-    exp_name='data_az_ptree/tictactoe_sp-mode_alphazero_seed0',
+    exp_name='data_az_ctree/tictactoe_sp-mode_alphazero_seed0',
     env=dict(
         board_size=3,
         battle_mode='self_play_mode',
         bot_action_type='v0',  # {'v0', 'alpha_beta_pruning'}
-        channel_last=False,  # NOTE
+        channel_last=False,
         collector_env_num=collector_env_num,
         evaluator_env_num=evaluator_env_num,
         n_evaluator_episode=evaluator_env_num,
         manager=dict(shared_memory=False, ),
         # ==============================================================
         # for the creation of simulation env
         agent_vs_human=False,
         prob_random_agent=0,
         prob_expert_agent=0,
         scale=True,
+        alphazero_mcts_ctree=mcts_ctree,
+        save_replay_gif=False,
+        replay_path_gif='./replay_gif',
         # ==============================================================
     ),
     policy=dict(
+        mcts_ctree=mcts_ctree,
         # ==============================================================
         # for the creation of simulation env
-        simulation_env_name='tictactoe',
+        simulation_env_id='tictactoe',
         simulation_env_config_type='self_play',
         # ==============================================================
         model=dict(
             observation_shape=(3, 3, 3),
             action_space_size=int(1 * 3 * 3),
             # We use the small size model for tictactoe.
             num_res_blocks=1,
```

### Comparing `LightZero-0.0.2/zoo/board_games/tictactoe/config/tictactoe_alphazero_sp_mode_multigpu_ddp_config.py` & `LightZero-0.0.5/zoo/board_games/tictactoe/config/tictactoe_alphazero_sp_mode_multigpu_ddp_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         prob_expert_agent=0,
         scale=True,
         # ==============================================================
     ),
     policy=dict(
         # ==============================================================
         # for the creation of simulation env
-        simulation_env_name='tictactoe',
+        simulation_env_id='tictactoe',
         simulation_env_config_type='self_play',
         # ==============================================================
         model=dict(
             observation_shape=(3, 3, 3),
             action_space_size=int(1 * 3 * 3),
             # We use the small size model for tictactoe.
             num_res_blocks=1,
```

### Comparing `LightZero-0.0.2/zoo/board_games/tictactoe/config/tictactoe_gumbel_muzero_bot_mode_config.py` & `LightZero-0.0.5/zoo/board_games/tictactoe/config/tictactoe_gumbel_muzero_bot_mode_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,14 +38,15 @@
             fc_policy_layers=[8],
             support_scale=10,
             reward_support_size=21,
             value_support_size=21,
         ),
         cuda=True,
         env_type='board_games',
+        action_type='varied_action_space',
         game_segment_length=5,
         update_per_collect=update_per_collect,
         batch_size=batch_size,
         optim_type='Adam',
         lr_piecewise_constant_decay=False,
         learning_rate=0.003,
         grad_clip_value=0.5,
```

### Comparing `LightZero-0.0.2/zoo/board_games/tictactoe/config/tictactoe_muzero_bot_mode_config.py` & `LightZero-0.0.5/zoo/board_games/tictactoe/config/tictactoe_muzero_bot_mode_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,15 @@
             support_scale=10,
             reward_support_size=21,
             value_support_size=21,
             norm_type='BN', 
         ),
         cuda=True,
         env_type='board_games',
+        action_type='varied_action_space',
         game_segment_length=5,
         update_per_collect=update_per_collect,
         batch_size=batch_size,
         optim_type='Adam',
         lr_piecewise_constant_decay=False,
         learning_rate=0.003,
         grad_clip_value=0.5,
```

### Comparing `LightZero-0.0.2/zoo/board_games/tictactoe/config/tictactoe_muzero_sp_mode_config.py` & `LightZero-0.0.5/lzero/agent/config/muzero/tictactoe_play_with_bot.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,75 +11,76 @@
 batch_size = 256
 max_env_step = int(2e5)
 reanalyze_ratio = 0.
 # ==============================================================
 # end of the most frequently changed config specified by the user
 # ==============================================================
 
-tictactoe_muzero_config = dict(
-    exp_name=
-    f'data_mz_ctree/tictactoe_muzero_sp-mode_ns{num_simulations}_upc{update_per_collect}_rr{reanalyze_ratio}_seed0',
-    env=dict(
-        battle_mode='self_play_mode',
-        collector_env_num=collector_env_num,
-        evaluator_env_num=evaluator_env_num,
-        n_evaluator_episode=evaluator_env_num,
-        manager=dict(shared_memory=False, ),
-    ),
-    policy=dict(
-        model=dict(
-            observation_shape=(3, 3, 3),
-            action_space_size=9,
-            image_channel=3,
-            # We use the small size model for tictactoe.
-            num_res_blocks=1,
-            num_channels=16,
-            fc_reward_layers=[8],
-            fc_value_layers=[8],
-            fc_policy_layers=[8],
-            support_scale=10,
-            reward_support_size=21,
-            value_support_size=21,
+cfg = dict(
+    main_config=dict(
+        exp_name='TicTacToe-play-with-bot-MuZero',
+        seed=0,
+        env=dict(
+            env_id='TicTacToe-play-with-bot',
+            battle_mode='play_with_bot_mode',
+            collector_env_num=collector_env_num,
+            evaluator_env_num=evaluator_env_num,
+            n_evaluator_episode=evaluator_env_num,
+            manager=dict(shared_memory=False, ),
+        ),
+        policy=dict(
+            model=dict(
+                observation_shape=(3, 3, 3),
+                action_space_size=9,
+                image_channel=3,
+                # We use the small size model for tictactoe.
+                num_res_blocks=1,
+                num_channels=16,
+                fc_reward_layers=[8],
+                fc_value_layers=[8],
+                fc_policy_layers=[8],
+                support_scale=10,
+                reward_support_size=21,
+                value_support_size=21,
+                norm_type='BN', 
+            ),
+            cuda=True,
+            env_type='board_games',
+            action_type='varied_action_space',
+            game_segment_length=5,
+            update_per_collect=update_per_collect,
+            batch_size=batch_size,
+            optim_type='Adam',
+            lr_piecewise_constant_decay=False,
+            learning_rate=0.003,
+            grad_clip_value=0.5,
+            num_simulations=num_simulations,
+            reanalyze_ratio=reanalyze_ratio,
+            # NOTE：In board_games, we set large td_steps to make sure the value target is the final outcome.
+            td_steps=9,
+            num_unroll_steps=3,
+            # NOTE：In board_games, we set discount_factor=1.
+            discount_factor=1,
+            n_episode=n_episode,
+            eval_freq=int(2e3),
+            replay_buffer_size=int(1e4),
+            collector_env_num=collector_env_num,
+            evaluator_env_num=evaluator_env_num,
+        ),
+        wandb_logger=dict(
+            gradient_logger=False, video_logger=False, plot_logger=False, action_logger=False, return_logger=False
         ),
-        cuda=True,
-        env_type='board_games',
-        game_segment_length=9,
-        update_per_collect=update_per_collect,
-        batch_size=batch_size,
-        optim_type='Adam',
-        lr_piecewise_constant_decay=False,
-        learning_rate=0.003,
-        grad_clip_value=0.5,
-        num_simulations=num_simulations,
-        reanalyze_ratio=reanalyze_ratio,
-        # NOTE：In board_games, we set large td_steps to make sure the value target is the final outcome.
-        td_steps=9,
-        num_unroll_steps=3,
-        # NOTE：In board_games, we set discount_factor=1.
-        discount_factor=1,
-        n_episode=n_episode,
-        eval_freq=int(2e3),
-        replay_buffer_size=int(1e4),
-        collector_env_num=collector_env_num,
-        evaluator_env_num=evaluator_env_num,
-    ),
-)
-tictactoe_muzero_config = EasyDict(tictactoe_muzero_config)
-main_config = tictactoe_muzero_config
-
-tictactoe_muzero_create_config = dict(
-    env=dict(
-        type='tictactoe',
-        import_names=['zoo.board_games.tictactoe.envs.tictactoe_env'],
-    ),
-    env_manager=dict(type='subprocess'),
-    policy=dict(
-        type='muzero',
-        import_names=['lzero.policy.muzero'],
     ),
+    create_config = dict(
+        env=dict(
+            type='tictactoe',
+            import_names=['zoo.board_games.tictactoe.envs.tictactoe_env'],
+        ),
+        env_manager=dict(type='subprocess'),
+        policy=dict(
+            type='muzero',
+            import_names=['lzero.policy.muzero'],
+        ),
+    )
 )
-tictactoe_muzero_create_config = EasyDict(tictactoe_muzero_create_config)
-create_config = tictactoe_muzero_create_config
 
-if __name__ == "__main__":
-    from lzero.entry import train_muzero
-    train_muzero([main_config, create_config], seed=0, max_env_step=max_env_step)
+cfg = EasyDict(cfg)
```

### Comparing `LightZero-0.0.2/zoo/board_games/tictactoe/entry/tictactoe_alphazero_eval.py` & `LightZero-0.0.5/zoo/board_games/tictactoe/entry/tictactoe_muzero_eval.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,60 @@
-from zoo.board_games.tictactoe.config.tictactoe_alphazero_bot_mode_config import main_config, create_config
-from lzero.entry import eval_alphazero
+from zoo.board_games.tictactoe.config.tictactoe_muzero_bot_mode_config import main_config, create_config
+from lzero.entry import eval_muzero
 import numpy as np
 
-if __name__ == '__main__':
-    """ 
-    model_path (:obj:`Optional[str]`): The pretrained model path, which should
-    point to the ckpt file of the pretrained model, and an absolute path is recommended.
-    In LightZero, the path is usually something like ``exp_name/ckpt/ckpt_best.pth.tar``.
+if __name__ == "__main__":
     """
-    model_path = './ckpt/ckpt_best.pth.tar'
+    Entry point for the evaluation of the MuZero model on the TicTacToe environment. 
+
+    Variables:
+        - model_path (:obj:`Optional[str]`): The pretrained model path, which should point to the ckpt file of the 
+        pretrained model. An absolute path is recommended. In LightZero, the path is usually something like 
+        ``exp_name/ckpt/ckpt_best.pth.tar``.
+        - returns_mean_seeds (:obj:`List[float]`): List to store the mean returns for each seed.
+        - returns_seeds (:obj:`List[float]`): List to store the returns for each seed.
+        - seeds (:obj:`List[int]`): List of seeds for the environment.
+        - num_episodes_each_seed (:obj:`int`): Number of episodes to run for each seed.
+        - total_test_episodes (:obj:`int`): Total number of test episodes, computed as the product of the number of 
+        seeds and the number of episodes per seed.
+    """
+
+    # model_path = "./ckpt/ckpt_best.pth.tar"
+    model_path = None
+
     seeds = [0]
-    num_episodes_each_seed = 5
+    num_episodes_each_seed = 1
     # If True, you can play with the agent.
     main_config.env.agent_vs_human = False
     create_config.env_manager.type = 'base'
     main_config.env.evaluator_env_num = 1
     main_config.env.n_evaluator_episode = 1
     total_test_episodes = num_episodes_each_seed * len(seeds)
+
+    # Enable saving of replay as a gif, specify the path to save the replay gif
+    main_config.env.replay_path = './video'
+
     returns_mean_seeds = []
     returns_seeds = []
     for seed in seeds:
-        returns_mean, returns = eval_alphazero(
+        returns_mean, returns = eval_muzero(
             [main_config, create_config],
             seed=seed,
             num_episodes_each_seed=num_episodes_each_seed,
             print_seed_details=True,
             model_path=model_path
         )
         returns_mean_seeds.append(returns_mean)
         returns_seeds.append(returns)
 
     returns_mean_seeds = np.array(returns_mean_seeds)
     returns_seeds = np.array(returns_seeds)
 
+    # Print evaluation results
     print("=" * 20)
-    print(f'We eval total {len(seeds)} seeds. In each seed, we eval {num_episodes_each_seed} episodes.')
-    print(f'In seeds {seeds}, returns_mean_seeds is {returns_mean_seeds}, returns is {returns_seeds}')
-    print('In all seeds, reward_mean:', returns_mean_seeds.mean(), end='. ')
+    print(f"We evaluated a total of {len(seeds)} seeds. For each seed, we evaluated {num_episodes_each_seed} episode(s).")
+    print(f"For seeds {seeds}, the mean returns are {returns_mean_seeds}, and the returns are {returns_seeds}.")
+    print("Across all seeds, the mean reward is:", returns_mean_seeds.mean())
     print(
         f'win rate: {len(np.where(returns_seeds == 1.)[0]) / total_test_episodes}, draw rate: {len(np.where(returns_seeds == 0.)[0]) / total_test_episodes}, lose rate: {len(np.where(returns_seeds == -1.)[0]) / total_test_episodes}'
     )
     print("=" * 20)
```

### Comparing `LightZero-0.0.2/zoo/board_games/tictactoe/entry/tictactoe_muzero_eval.py` & `LightZero-0.0.5/zoo/board_games/gomoku/entry/gomoku_alphazero_eval.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,61 @@
-from zoo.board_games.tictactoe.config.tictactoe_muzero_bot_mode_config import main_config, create_config
-from lzero.entry import eval_muzero
+from zoo.board_games.gomoku.config.gomoku_alphazero_bot_mode_config import main_config, create_config
+from lzero.entry import eval_alphazero
 import numpy as np
 
-if __name__ == "__main__":
-    """ 
-    model_path (:obj:`Optional[str]`): The pretrained model path, which should
-    point to the ckpt file of the pretrained model, and an absolute path is recommended.
-    In LightZero, the path is usually something like ``exp_name/ckpt/ckpt_best.pth.tar``.
+if __name__ == '__main__':
     """
+    Entry point for the evaluation of the AlphaZero model on the Gomoku environment. 
+
+    Variables:
+        - model_path (:obj:`Optional[str]`): The pretrained model path, which should point to the ckpt file of the 
+        pretrained model. An absolute path is recommended. In LightZero, the path is usually something like 
+        ``exp_name/ckpt/ckpt_best.pth.tar``.
+        - returns_mean_seeds (:obj:`List[float]`): List to store the mean returns for each seed.
+        - returns_seeds (:obj:`List[float]`): List to store the returns for each seed.
+        - seeds (:obj:`List[int]`): List of seeds for the environment.
+        - num_episodes_each_seed (:obj:`int`): Number of episodes to run for each seed.
+        - total_test_episodes (:obj:`int`): Total number of test episodes, computed as the product of the number of 
+        seeds and the number of episodes per seed.
+    """
+    # model_path = './ckpt/ckpt_best.pth.tar'
+    model_path = None
 
-    model_path = "./ckpt/ckpt_best.pth.tar"
     seeds = [0]
-    num_episodes_each_seed = 5
+    num_episodes_each_seed = 1
     # If True, you can play with the agent.
+    # main_config.env.agent_vs_human = True
     main_config.env.agent_vs_human = False
+    # main_config.env.render_mode = 'image_realtime_mode'
+    main_config.env.render_mode = 'image_savefile_mode'
+    main_config.env.replay_path = './video'
+
     create_config.env_manager.type = 'base'
+    main_config.env.alphazero_mcts_ctree = False
+    main_config.policy.mcts_ctree = False
     main_config.env.evaluator_env_num = 1
     main_config.env.n_evaluator_episode = 1
     total_test_episodes = num_episodes_each_seed * len(seeds)
     returns_mean_seeds = []
     returns_seeds = []
     for seed in seeds:
-        returns_mean, returns = eval_muzero(
+        returns_mean, returns = eval_alphazero(
             [main_config, create_config],
             seed=seed,
             num_episodes_each_seed=num_episodes_each_seed,
             print_seed_details=True,
             model_path=model_path
         )
         returns_mean_seeds.append(returns_mean)
         returns_seeds.append(returns)
 
     returns_mean_seeds = np.array(returns_mean_seeds)
     returns_seeds = np.array(returns_seeds)
 
     print("=" * 20)
-    print(f'We eval total {len(seeds)} seeds. In each seed, we eval {num_episodes_each_seed} episodes.')
-    print(f'In seeds {seeds}, returns_mean_seeds is {returns_mean_seeds}, returns is {returns_seeds}')
-    print('In all seeds, reward_mean:', returns_mean_seeds.mean(), end='. ')
+    print(f"We evaluated a total of {len(seeds)} seeds. For each seed, we evaluated {num_episodes_each_seed} episode(s).")
+    print(f"For seeds {seeds}, the mean returns are {returns_mean_seeds}, and the returns are {returns_seeds}.")
+    print("Across all seeds, the mean reward is:", returns_mean_seeds.mean())
     print(
         f'win rate: {len(np.where(returns_seeds == 1.)[0]) / total_test_episodes}, draw rate: {len(np.where(returns_seeds == 0.)[0]) / total_test_episodes}, lose rate: {len(np.where(returns_seeds == -1.)[0]) / total_test_episodes}'
     )
     print("=" * 20)
```

### Comparing `LightZero-0.0.2/zoo/board_games/tictactoe/envs/test_tictactoe_alphabeta_prunning_bot.py` & `LightZero-0.0.5/zoo/board_games/tictactoe/envs/test_tictactoe_alphabeta_prunning_bot.py`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/zoo/board_games/tictactoe/envs/test_tictactoe_env.py` & `LightZero-0.0.5/zoo/board_games/tictactoe/envs/test_tictactoe_env.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,20 +5,22 @@
 
 @pytest.mark.envtest
 class TestTicTacToeEnv:
 
     def test_self_play_mode(self):
         cfg = EasyDict(
             battle_mode='self_play_mode',
-            channel_last=True,
+            channel_last=False,
             scale=True,
             agent_vs_human=False,
             prob_random_agent=0,
             prob_expert_agent=0,
-            bot_action_type='v0'
+            bot_action_type='v0',
+            # alphazero_mcts_ctree (bool): If True, the Monte Carlo Tree Search from AlphaZero is used.
+            alphazero_mcts_ctree=False,
         )
         env = TicTacToeEnv(cfg)
         env.reset()
         print('init board state: ')
         env.render()
         while True:
             """player 1"""
@@ -52,22 +54,22 @@
                 else:
                     print('draw')
                 break
 
     def test_play_with_bot_mode(self):
         cfg = EasyDict(
             battle_mode='play_with_bot_mode',
-            channel_last=True,
+            channel_last=False,
             scale=True,
-            # channel_last=False,
-            # scale=False,
             agent_vs_human=False,
             prob_random_agent=0,
             prob_expert_agent=0,
-            bot_action_type='v0'
+            bot_action_type='v0',
+            # alphazero_mcts_ctree (bool): If True, the Monte Carlo Tree Search from AlphaZero is used.
+            alphazero_mcts_ctree=False,
         )
         env = TicTacToeEnv(cfg)
         env.reset()
         print('init board state: ')
         env.render()
         while True:
             """player 1"""
```

### Comparing `LightZero-0.0.2/zoo/board_games/tictactoe/envs/test_tictactoe_mcts_bot.py` & `LightZero-0.0.5/zoo/board_games/tictactoe/envs/test_tictactoe_mcts_bot.py`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/zoo/board_games/tictactoe/envs/test_tictactoe_rule_bot_v0.py` & `LightZero-0.0.5/zoo/board_games/tictactoe/envs/test_tictactoe_rule_bot_v0.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 from easydict import EasyDict
 import pytest
 
 from zoo.board_games.tictactoe.envs.tictactoe_env import TicTacToeEnv
 
 cfg = EasyDict(
-    channel_last=True,
+    channel_last=False,
     scale=False,
     prob_random_agent=0,
     prob_expert_agent=0,
     battle_mode='play_with_bot_mode',
     agent_vs_human=False,
     bot_action_type='v0',  # {'v0',  'alpha_beta_pruning'}
 )
```

### Comparing `LightZero-0.0.2/zoo/board_games/tictactoe/envs/tictactoe_env.py` & `LightZero-0.0.5/zoo/board_games/tictactoe/envs/tictactoe_env.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 import copy
+import os
 import sys
+from datetime import datetime
 from functools import lru_cache
 from typing import List
 
-import gym
+import gymnasium as gym
+import matplotlib.pyplot as plt
 import numpy as np
 from ding.envs.env.base_env import BaseEnv, BaseEnvTimestep
 from ding.utils.registry_factory import ENV_REGISTRY
 from ditk import logging
 from easydict import EasyDict
+from zoo.board_games.tictactoe.envs.get_done_winner_cython import get_done_winner_cython
+from zoo.board_games.tictactoe.envs.legal_actions_cython import legal_actions_cython
 
 from zoo.board_games.alphabeta_pruning_bot import AlphaBetaPruningBot
-from zoo.board_games.tictactoe.envs.legal_actions_cython import legal_actions_cython
-from zoo.board_games.tictactoe.envs.get_done_winner_cython import get_done_winner_cython
 
 
 @lru_cache(maxsize=512)
 def _legal_actions_func_lru(board_tuple):
     # Convert tuple to NumPy array.
     board_array = np.array(board_tuple, dtype=np.int32)
     # Convert NumPy array to memory view.
@@ -31,25 +34,40 @@
     # Convert NumPy array to memory view.
     board_view = board_array.view(dtype=np.int32).reshape(board_array.shape)
     return get_done_winner_cython(board_view)
 
 
 @ENV_REGISTRY.register('tictactoe')
 class TicTacToeEnv(BaseEnv):
+
     config = dict(
-        env_name="TicTacToe",
+        # env_id (str): The name of the environment.
+        env_id="TicTacToe",
+        # battle_mode (str): The mode of the battle. Choices are 'self_play_mode' or 'alpha_beta_pruning'.
         battle_mode='self_play_mode',
-        mcts_mode='self_play_mode',  # only used in AlphaZero
-        bot_action_type='v0',  # {'v0', 'alpha_beta_pruning'}
+        # battle_mode_in_simulation_env (str): The mode of Monte Carlo Tree Search. This is only used in AlphaZero.
+        battle_mode_in_simulation_env='self_play_mode',
+        # bot_action_type (str): The type of action the bot should take. Choices are 'v0' or 'alpha_beta_pruning'.
+        bot_action_type='v0',
+        # replay_path (str): The folder path where replay video saved, if None, will not save replay video.
+        replay_path=None,
+        # agent_vs_human (bool): If True, the agent will play against a human.
         agent_vs_human=False,
+        # prob_random_agent (int): The probability of the random agent.
         prob_random_agent=0,
+        # prob_expert_agent (int): The probability of the expert agent.
         prob_expert_agent=0,
-        channel_last=True,
+        # channel_last (bool): If True, the channel will be the last dimension.
+        channel_last=False,
+        # scale (bool): If True, the pixel values will be scaled.
         scale=True,
+        # stop_value (int): The value to stop the game.
         stop_value=1,
+        # alphazero_mcts_ctree (bool): If True, the Monte Carlo Tree Search from AlphaZero is used.
+        alphazero_mcts_ctree=False,
     )
 
     @classmethod
     def default_config(cls: type) -> EasyDict:
         cfg = EasyDict(copy.deepcopy(cls.config))
         cfg.cfg_type = cls.__name__ + 'Dict'
         return cfg
@@ -58,28 +76,31 @@
         self.cfg = cfg
         self.channel_last = cfg.channel_last
         self.scale = cfg.scale
         self.battle_mode = cfg.battle_mode
         # The mode of interaction between the agent and the environment.
         assert self.battle_mode in ['self_play_mode', 'play_with_bot_mode', 'eval_mode']
         # The mode of MCTS is only used in AlphaZero.
-        self.mcts_mode = 'self_play_mode'
+        self.battle_mode_in_simulation_env = 'self_play_mode'
         self.board_size = 3
         self.players = [1, 2]
         self.total_num_actions = 9
         self.prob_random_agent = cfg.prob_random_agent
         self.prob_expert_agent = cfg.prob_expert_agent
         assert (self.prob_random_agent >= 0 and self.prob_expert_agent == 0) or (
                 self.prob_random_agent == 0 and self.prob_expert_agent >= 0), \
             f'self.prob_random_agent:{self.prob_random_agent}, self.prob_expert_agent:{self.prob_expert_agent}'
         self._env = self
         self.agent_vs_human = cfg.agent_vs_human
         self.bot_action_type = cfg.bot_action_type
         if 'alpha_beta_pruning' in self.bot_action_type:
             self.alpha_beta_pruning_player = AlphaBetaPruningBot(self, cfg, 'alpha_beta_pruning_player')
+        self.alphazero_mcts_ctree = cfg.alphazero_mcts_ctree
+        self._replay_path = cfg.replay_path if hasattr(cfg, "replay_path") and cfg.replay_path is not None else None
+        self._save_replay_count = 0
 
     @property
     def legal_actions(self):
         # Convert NumPy arrays to nested tuples to make them hashable.
         return _legal_actions_func_lru(tuple(map(tuple, self.board)))
 
     # only for evaluation speed
@@ -90,39 +111,61 @@
     # only for evaluation speed
     @property
     def legal_actions_cython_lru(self):
         # Convert NumPy arrays to nested tuples to make them hashable.
         return _legal_actions_func_lru(tuple(map(tuple, self.board)))
 
     def get_done_winner(self):
+        """
+        Overview:
+             Check if the game is over and who the winner is. Return 'done' and 'winner'.
+        Returns:
+            - outputs (:obj:`Tuple`): Tuple containing 'done' and 'winner',
+                - if player 1 win,     'done' = True, 'winner' = 1
+                - if player 2 win,     'done' = True, 'winner' = 2
+                - if draw,             'done' = True, 'winner' = -1
+                - if game is not over, 'done' = False, 'winner' = -1
+        """
         # Convert NumPy arrays to nested tuples to make them hashable.
         return _get_done_winner_func_lru(tuple(map(tuple, self.board)))
 
-    def reset(self, start_player_index=0, init_state=None):
+    def reset(self, start_player_index=0, init_state=None, katago_policy_init=False, katago_game_state=None):
         """
         Overview:
-            Env reset and custom state start by init_state
+            This method resets the environment and optionally starts with a custom state specified by 'init_state'.
         Arguments:
-            start_player_index: players = [1,2], player_index = [0,1]
-            init_state: custom start state.
-        """
+            - start_player_index (:obj:`int`, optional): Specifies the starting player. The players are [1,2] and
+                their corresponding indices are [0,1]. Defaults to 0.
+            - init_state (:obj:`Any`, optional): The custom starting state. If provided, the game starts from this state.
+                Defaults to None.
+            - katago_policy_init (:obj:`bool`, optional): This parameter is used to maintain compatibility with the
+                handling of 'katago' related parts in 'alphazero_mcts_ctree' in Go. Defaults to False.
+            - katago_game_state (:obj:`Any`, optional): This parameter is similar to 'katago_policy_init' and is used to
+                maintain compatibility with 'katago' in 'alphazero_mcts_ctree'. Defaults to None.
+        """
+        if self.alphazero_mcts_ctree and init_state is not None:
+            # Convert byte string to np.ndarray
+            init_state = np.frombuffer(init_state, dtype=np.int32)
+
         if self.scale:
             self._observation_space = gym.spaces.Box(
                 low=0, high=1, shape=(self.board_size, self.board_size, 3), dtype=np.float32
             )
         else:
             self._observation_space = gym.spaces.Box(
                 low=0, high=2, shape=(self.board_size, self.board_size, 3), dtype=np.uint8
             )
         self._action_space = gym.spaces.Discrete(self.board_size ** 2)
         self._reward_space = gym.spaces.Box(low=0, high=1, shape=(1,), dtype=np.float32)
         self.start_player_index = start_player_index
         self._current_player = self.players[self.start_player_index]
         if init_state is not None:
             self.board = np.array(copy.deepcopy(init_state), dtype="int32")
+            if self.alphazero_mcts_ctree:
+                self.board = self.board.reshape((self.board_size, self.board_size))
         else:
             self.board = np.zeros((self.board_size, self.board_size), dtype="int32")
 
         action_mask = np.zeros(self.total_num_actions, 'int8')
         action_mask[self.legal_actions] = 1
 
         if self.battle_mode == 'play_with_bot_mode' or self.battle_mode == 'eval_mode':
@@ -142,14 +185,17 @@
             obs = {
                 'observation': self.current_state()[1],
                 'action_mask': action_mask,
                 'board': copy.deepcopy(self.board),
                 'current_player_index': self.start_player_index,
                 'to_play': self.current_player
             }
+        if self._replay_path is not None:
+            self._frames = []
+
         return obs
 
     def reset_v2(self, start_player_index=0, init_state=None):
         """
         Overview:
             only used in alpha-beta pruning bot.
         """
@@ -168,15 +214,16 @@
             elif self.prob_expert_agent > 0:
                 if np.random.rand() < self.prob_expert_agent:
                     action = self.bot_action()
 
             timestep = self._player_step(action)
             if timestep.done:
                 # The eval_episode_return is calculated from Player 1's perspective。
-                timestep.info['eval_episode_return'] = -timestep.reward if timestep.obs['to_play'] == 1 else timestep.reward
+                timestep.info['eval_episode_return'] = -timestep.reward if timestep.obs[
+                                                                               'to_play'] == 1 else timestep.reward
             return timestep
         elif self.battle_mode == 'play_with_bot_mode':
             # player 1 battle with expert player 2
 
             # player 1's turn
             timestep_player1 = self._player_step(action)
             # self.env.render()
@@ -200,41 +247,74 @@
             timestep.obs['to_play'] = -1
 
             return timestep
         elif self.battle_mode == 'eval_mode':
             # player 1 battle with expert player 2
 
             # player 1's turn
+            if self._replay_path is not None:
+                self._frames.append(self._env.render(mode='rgb_array'))
             timestep_player1 = self._player_step(action)
             # self.env.render()
             if timestep_player1.done:
                 # NOTE: in eval_mode, we must set to_play as -1, because we don't consider the alternation between players.
                 # And the to_play is used in MCTS.
                 timestep_player1.obs['to_play'] = -1
+
+                if self._replay_path is not None:
+                    if not os.path.exists(self._replay_path):
+                        os.makedirs(self._replay_path)
+                    timestamp = datetime.now().strftime("%Y%m%d%H%M%S")
+                    path = os.path.join(
+                        self._replay_path,
+                        'tictactoe_{}_{}_{}.mp4'.format(os.getpid(), timestamp, self._save_replay_count)
+                    )
+                    self.display_frames_as_mp4(self._frames, path)
+                    print(f'replay {path} saved!')
+                    self._save_replay_count += 1
+
                 return timestep_player1
 
             # player 2's turn
             if self.agent_vs_human:
                 bot_action = self.human_to_action()
             else:
                 bot_action = self.bot_action()
             # print('player 2 (computer player): ' + self.action_to_string(bot_action))
+            if self._replay_path is not None:
+                self._frames.append(self._env.render(mode='rgb_array'))
             timestep_player2 = self._player_step(bot_action)
+            if self._replay_path is not None:
+                self._frames.append(self._env.render(mode='rgb_array'))
             # the eval_episode_return is calculated from Player 1's perspective
             timestep_player2.info['eval_episode_return'] = -timestep_player2.reward
             timestep_player2 = timestep_player2._replace(reward=-timestep_player2.reward)
 
             timestep = timestep_player2
             # NOTE: in eval_mode, we must set to_play as -1, because we don't consider the alternation between players.
             # And the to_play is used in MCTS.
             timestep.obs['to_play'] = -1
 
+            if timestep_player2.done:
+                if self._replay_path is not None:
+                    if not os.path.exists(self._replay_path):
+                        os.makedirs(self._replay_path)
+                    timestamp = datetime.now().strftime("%Y%m%d%H%M%S")
+                    path = os.path.join(
+                        self._replay_path,
+                        'tictactoe_{}_{}_{}.mp4'.format(os.getpid(), timestamp, self._save_replay_count)
+                    )
+                    self.display_frames_as_mp4(self._frames, path)
+                    print(f'replay {path} saved!')
+                    self._save_replay_count += 1
+
             return timestep
 
     def _player_step(self, action):
+
         if action in self.legal_actions:
             row, col = self.action_to_coord(action)
             self.board[row, col] = self.current_player
         else:
             logging.warning(
                 f"You input illegal action: {action}, the legal_actions are {self.legal_actions}. "
                 f"Now we randomly choice a action from self.legal_actions."
@@ -243,24 +323,23 @@
             row, col = self.action_to_coord(action)
             self.board[row, col] = self.current_player
 
         # Check whether the game is ended or not and give the winner
         done, winner = self.get_done_winner()
 
         reward = np.array(float(winner == self.current_player)).astype(np.float32)
-        info = {'next player to play': self.to_play}
+        info = {'next player to play': self.next_player}
         """
         NOTE: here exchange the player
         """
-        self.current_player = self.to_play
+        self.current_player = self.next_player
 
         if done:
             info['eval_episode_return'] = reward
             # print('tictactoe one episode done: ', info)
-
         action_mask = np.zeros(self.total_num_actions, 'int8')
         action_mask[self.legal_actions] = 1
         obs = {
             'observation': self.current_state()[1],
             'action_mask': action_mask,
             'board': copy.deepcopy(self.board),
             'current_player_index': self.players.index(self.current_player),
@@ -273,19 +352,19 @@
         Overview:
             obtain the state from the view of current player.
             self.board is nd-array, 0 indicates that no stones is placed here,
             1 indicates that player 1's stone is placed here, 2 indicates player 2's stone is placed here
         Returns:
             - current_state (:obj:`array`):
                 the 0 dim means which positions is occupied by self.current_player,
-                the 1 dim indicates which positions are occupied by self.to_play,
+                the 1 dim indicates which positions are occupied by self.next_player,
                 the 2 dim indicates which player is the to_play player, 1 means player 1, 2 means player 2
         """
         board_curr_player = np.where(self.board == self.current_player, 1, 0)
-        board_opponent_player = np.where(self.board == self.to_play, 1, 0)
+        board_opponent_player = np.where(self.board == self.next_player, 1, 0)
         board_to_play = np.full((self.board_size, self.board_size), self.current_player)
         raw_obs = np.array([board_curr_player, board_opponent_player, board_to_play], dtype=np.float32)
         if self.scale:
             scale_obs = copy.deepcopy(raw_obs / 2)
         else:
             scale_obs = copy.deepcopy(raw_obs)
         if self.channel_last:
@@ -409,21 +488,22 @@
     @property
     def current_player(self):
         return self._current_player
 
     @property
     def current_player_index(self):
         """
-        current_player_index = 0, current_player = 1
-        current_player_index = 1, current_player = 2
+        Overview:
+            current_player_index = 0, current_player = 1
+            current_player_index = 1, current_player = 2
         """
         return 0 if self._current_player == 1 else 1
 
     @property
-    def to_play(self):
+    def next_player(self):
         return self.players[0] if self.current_player == self.players[1] else self.players[1]
 
     @property
     def current_player_to_compute_bot_action(self):
         """
         Overview: to compute expert action easily.
         """
@@ -530,25 +610,114 @@
         row, col = self.action_to_coord(action)
         self.board[row, col] = self.current_player
         new_legal_actions = copy.deepcopy(self.legal_actions)
         new_board = copy.deepcopy(self.board)
 
         return new_board, new_legal_actions
 
+    def render(self, mode="human"):
+        """
+        Render the game state, either as a string (mode='human') or as an RGB image (mode='rgb_array').
+
+        Arguments:
+            - mode (:obj:`str`): The mode to render with. Valid modes are:
+                - 'human': render to the current display or terminal and
+                - 'rgb_array': Return an numpy.ndarray with shape (x, y, 3),
+                  representing RGB values for an image of the board
+        Returns:
+            if mode is:
+            - 'human': returns None
+            - 'rgb_array': return a numpy array representing the rendered image.
+        Raises:
+            ValueError: If the provided mode is unknown.
+        """
+        if mode == 'human':
+            print(self.board)
+        elif mode == 'rgb_array':
+            dpi = 80
+            fig, ax = plt.subplots(figsize=(6, 6), dpi=dpi)
+
+            # """Piece is in the cross point of row and col"""
+            # # Draw a black background, white grid
+            # ax.imshow(np.zeros((self.board_size, self.board_size, 3)), origin='lower')
+            # ax.grid(color='white', linewidth=2)
+            #
+            # # Draw the 'X' and 'O' symbols for each player
+            # for i in range(self.board_size):
+            #     for j in range(self.board_size):
+            #         if self.board[i, j] == 1:  # Player 1
+            #             ax.text(j, i, 'X', ha='center', va='center', color='white', fontsize=24)
+            #         elif self.board[i, j] == 2:  # Player 2
+            #             ax.text(j, i, 'O', ha='center', va='center', color='white', fontsize=24)
+
+            # # Setup the axes
+            # ax.set_xticks(np.arange(self.board_size))
+            # ax.set_yticks(np.arange(self.board_size))
+
+            """Piece is in the center point of grid"""
+            # Draw a peachpuff background, black grid
+            ax.imshow(np.ones((self.board_size, self.board_size, 3)) * np.array([255, 218, 185]) / 255, origin='lower')
+            ax.grid(color='black', linewidth=2)
+
+            # Draw the 'X' and 'O' symbols for each player
+            for i in range(self.board_size):
+                for j in range(self.board_size):
+                    if self.board[i, j] == 1:  # Player 1
+                        ax.text(j, i, 'X', ha='center', va='center', color='black', fontsize=24)
+                    elif self.board[i, j] == 2:  # Player 2
+                        ax.text(j, i, 'O', ha='center', va='center', color='white', fontsize=24)
+
+            # Setup the axes
+            ax.set_xticks(np.arange(0.5, self.board_size, 1))
+            ax.set_yticks(np.arange(0.5, self.board_size, 1))
+
+            ax.set_xticklabels([])
+            ax.set_yticklabels([])
+            ax.xaxis.set_ticks_position('none')
+            ax.yaxis.set_ticks_position('none')
+
+            # Set the title of the game
+            plt.title('TicTacToe: ' + ('Black Turn' if self.current_player == 1 else 'White Turn'))
+
+            fig.canvas.draw()
+
+            # Get the width and height of the figure
+            width, height = fig.get_size_inches() * fig.get_dpi()
+            width = int(width)
+            height = int(height)
+
+            # Use the width and height values to reshape the numpy array
+            img = np.frombuffer(fig.canvas.tostring_rgb(), dtype='uint8')
+            img = img.reshape(height, width, 3)
+
+            plt.close(fig)
+
+            return img
+        else:
+            raise ValueError(f"Unknown mode '{mode}', it should be either 'human' or 'rgb_array'.")
+
+    @staticmethod
+    def display_frames_as_gif(frames: list, path: str) -> None:
+        import imageio
+        imageio.mimsave(path, frames, fps=20)
+
+    @staticmethod
+    def display_frames_as_mp4(frames: list, path: str, fps=5) -> None:
+        assert path.endswith('.mp4'), f'path must end with .mp4, but got {path}'
+        import imageio
+        imageio.mimwrite(path, frames, fps=fps)
+
     def clone(self):
         return copy.deepcopy(self)
 
     def seed(self, seed: int, dynamic_seed: bool = True) -> None:
         self._seed = seed
         self._dynamic_seed = dynamic_seed
         np.random.seed(self._seed)
 
-    def render(self, mode="human"):
-        print(self.board)
-
     @property
     def observation_space(self) -> gym.spaces.Space:
         return self._observation_space
 
     @property
     def action_space(self) -> gym.spaces.Space:
         return self._action_space
```

### Comparing `LightZero-0.0.2/zoo/box2d/bipedalwalker/config/bipedalwalker_cont_disc_efficientzero_config.py` & `LightZero-0.0.5/zoo/box2d/bipedalwalker/config/bipedalwalker_cont_disc_efficientzero_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # ==============================================================
 
 bipedalwalker_cont_disc_efficientzero_config = dict(
     exp_name=
     f'data_sez_ctree/bipedalwalker_cont_disc_efficientzero_ns{num_simulations}_upc{update_per_collect}-mur{model_update_ratio}_rr{reanalyze_ratio}_seed0',
     env=dict(
         stop_value=int(1e6),
-        env_name='BipedalWalker-v3',
+        env_id='BipedalWalker-v3',
         env_type='normal',
         manually_discretization=True,
         continuous=False,
         each_dim_disc_size=each_dim_disc_size,
         collector_env_num=collector_env_num,
         evaluator_env_num=evaluator_env_num,
         n_evaluator_episode=evaluator_env_num,
```

### Comparing `LightZero-0.0.2/zoo/box2d/bipedalwalker/config/bipedalwalker_cont_disc_sampled_efficientzero_config.py` & `LightZero-0.0.5/zoo/box2d/bipedalwalker/config/bipedalwalker_cont_disc_sampled_efficientzero_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 # ==============================================================
 
 bipedalwalker_cont_disc_sampled_efficientzero_config = dict(
     exp_name=
     f'data_sez_ctree/bipedalwalker_cont_disc_sampled_efficientzero_k{K}_ns{num_simulations}_upc{update_per_collect}-mur{model_update_ratio}_rr{reanalyze_ratio}_seed0',
     env=dict(
         stop_value=int(1e6),
-        env_name='BipedalWalker-v3',
+        env_id='BipedalWalker-v3',
         env_type='normal',
         continuous=True,
         manually_discretization=True,
         each_dim_disc_size=each_dim_disc_size,
         collector_env_num=collector_env_num,
         evaluator_env_num=evaluator_env_num,
         n_evaluator_episode=evaluator_env_num,
```

### Comparing `LightZero-0.0.2/zoo/box2d/bipedalwalker/config/bipedalwalker_cont_sampled_efficientzero_config.py` & `LightZero-0.0.5/zoo/box2d/bipedalwalker/config/bipedalwalker_cont_sampled_efficientzero_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # end of the most frequently changed config specified by the user
 # ==============================================================
 
 bipedalwalker_cont_sampled_efficientzero_config = dict(
     exp_name=
     f'data_sez_ctree/bipedalwalker_cont_sampled_efficientzero_k{K}_ns{num_simulations}_upc{update_per_collect}-mur{model_update_ratio}_rr{reanalyze_ratio}_seed0',
     env=dict(
-        env_name='BipedalWalker-v3',
+        env_id='BipedalWalker-v3',
         env_type='normal',
         continuous=True,
         manually_discretization=False,
         collector_env_num=collector_env_num,
         evaluator_env_num=evaluator_env_num,
         n_evaluator_episode=evaluator_env_num,
         manager=dict(shared_memory=False, ),
```

### Comparing `LightZero-0.0.2/zoo/box2d/bipedalwalker/config/tmp.py` & `LightZero-0.0.5/zoo/box2d/bipedalwalker/config/tmp.py`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/zoo/box2d/bipedalwalker/envs/bipedalwalker_cont_disc_env.py` & `LightZero-0.0.5/zoo/classic_control/cartpole/envs/cartpole_lightzero_env.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,206 +1,184 @@
 import copy
-import os
-from itertools import product
-from typing import List, Optional
+from datetime import datetime
+from typing import Union, Optional, Dict
 
-import gym
+import gymnasium as gym
 import numpy as np
 from ding.envs import BaseEnv, BaseEnvTimestep
-from ding.envs.common.common_function import affine_transform
+from ding.envs import ObsPlusPrevActRewWrapper
 from ding.torch_utils import to_ndarray
 from ding.utils import ENV_REGISTRY
 from easydict import EasyDict
 
 
-@ENV_REGISTRY.register('bipedalwalker_cont_disc')
-class BipedalWalkerDiscEnv(BaseEnv):
+@ENV_REGISTRY.register('cartpole_lightzero')
+class CartPoleEnv(BaseEnv):
     """
-        Overview:
-            The modified BipedalWalker environment with manually discretized action space. For each dimension, equally dividing the
-            original continuous action into ``each_dim_disc_size`` bins and using their Cartesian product to obtain
-            handcrafted discrete actions.
+    LightZero version of the classic CartPole environment. This class includes methods for resetting, closing, and
+    stepping through the environment, as well as seeding for reproducibility, saving replay videos, and generating random
+    actions. It also includes properties for accessing the observation space, action space, and reward space of the
+    environment.
     """
 
+    config = dict(
+        # env_id (str): The name of the environment.
+        env_id="CartPole-v0",
+        # replay_path (str): The path to save the replay video. If None, the replay will not be saved.
+        # Only effective when env_manager.type is 'base'.
+        replay_path=None,
+    )
+
     @classmethod
     def default_config(cls: type) -> EasyDict:
         cfg = EasyDict(copy.deepcopy(cls.config))
         cfg.cfg_type = cls.__name__ + 'Dict'
         return cfg
 
-    config = dict(
-        save_replay_gif=False,
-        replay_path_gif=None,
-        replay_path=None,
-        act_scale=True,
-        rew_clip=True,
-        delay_reward_step=0,
-        prob_random_agent=0.,
-        collect_max_episode_steps=int(1.08e5),
-        eval_max_episode_steps=int(1.08e5),
-        each_dim_disc_size=4,
-    )
-
-    def __init__(self, cfg: dict) -> None:
+    def __init__(self, cfg: dict = {}) -> None:
+        """
+        Initialize the environment with a configuration dictionary. Sets up spaces for observations, actions, and rewards.
+        """
         self._cfg = cfg
         self._init_flag = False
-        self._act_scale = cfg.act_scale
-        self._rew_clip = cfg.rew_clip
+        self._continuous = False
         self._replay_path = cfg.replay_path
-        self._replay_path_gif = cfg.replay_path_gif
-        self._save_replay_gif = cfg.save_replay_gif
-        self._save_replay_count = 0
+        self._observation_space = gym.spaces.Box(
+            low=np.array([-4.8, float("-inf"), -0.42, float("-inf")]),
+            high=np.array([4.8, float("inf"), 0.42, float("inf")]),
+            shape=(4,),
+            dtype=np.float32
+        )
+        self._action_space = gym.spaces.Discrete(2)
+        self._action_space.seed(0)  # default seed
+        self._reward_space = gym.spaces.Box(low=0.0, high=1.0, shape=(1,), dtype=np.float32)
 
-    def reset(self) -> np.ndarray:
+    def reset(self) -> Dict[str, np.ndarray]:
         """
-        Overview:
-             During the reset phase, the original environment will be created,
-             and at the same time, the action space will be discretized into "each_dim_disc_size" bins.
-        Returns:
-            - info_dict (:obj:`Dict[str, Any]`): Including observation, action_mask, and to_play label.
+        Reset the environment. If it hasn't been initialized yet, this method also handles that. It also handles seeding
+        if necessary. Returns the first observation.
         """
         if not self._init_flag:
-            self._env = gym.make('BipedalWalker-v3', hardcore=True)
-            self._observation_space = self._env.observation_space
-            self._action_space = self._env.action_space
-            self._reward_space = gym.spaces.Box(
-                low=self._env.reward_range[0], high=self._env.reward_range[1], shape=(1, ), dtype=np.float32
-            )
+            self._env = gym.make('CartPole-v0', render_mode="rgb_array")
+            if self._replay_path is not None:
+                timestamp = datetime.now().strftime("%Y%m%d%H%M%S")
+                video_name = f'{self._env.spec.id}-video-{timestamp}'
+                self._env = gym.wrappers.RecordVideo(
+                    self._env,
+                    video_folder=self._replay_path,
+                    episode_trigger=lambda episode_id: True,
+                    name_prefix=video_name
+                )
+            if hasattr(self._cfg, 'obs_plus_prev_action_reward') and self._cfg.obs_plus_prev_action_reward:
+                self._env = ObsPlusPrevActRewWrapper(self._env)
             self._init_flag = True
         if hasattr(self, '_seed') and hasattr(self, '_dynamic_seed') and self._dynamic_seed:
             np_seed = 100 * np.random.randint(1, 1000)
-            self._env.seed(self._seed + np_seed)
+            self._seed = self._seed + np_seed
+            self._action_space.seed(self._seed)
+            obs, _ = self._env.reset(seed=self._seed)
         elif hasattr(self, '_seed'):
-            self._env.seed(self._seed)
-        if self._replay_path is not None:
-            self._env = gym.wrappers.RecordVideo(
-                self._env,
-                video_folder=self._replay_path,
-                episode_trigger=lambda episode_id: True,
-                name_prefix='rl-video-{}'.format(id(self))
-            )
-        obs = self._env.reset()
-        obs = to_ndarray(obs).astype(np.float32)
+            self._action_space.seed(self._seed)
+            obs, _ = self._env.reset(seed=self._seed)
+        else:
+            obs, _ = self._env.reset()
+        self._observation_space = self._env.observation_space
         self._eval_episode_return = 0
-        if self._save_replay_gif:
-            self._frames = []
-        # disc_to_cont: transform discrete action index to original continuous action
-        self._raw_action_space = self._env.action_space
-        self.m = self._raw_action_space.shape[0]
-        self.n = self._cfg.each_dim_disc_size
-        self.K = self.n ** self.m
-        self.disc_to_cont = list(product(*[list(range(self.n)) for _ in range(self.m)]))
-        # the modified discrete action space
-        self._action_space = gym.spaces.Discrete(self.K)
+        obs = to_ndarray(obs)
 
-        action_mask = np.ones(self.K, 'int8')
+        action_mask = np.ones(self.action_space.n, 'int8')
         obs = {'observation': obs, 'action_mask': action_mask, 'to_play': -1}
-        return obs
 
-    def close(self) -> None:
-        if self._init_flag:
-            self._env.close()
-        self._init_flag = False
-
-    def render(self) -> None:
-        self._env.render()
-
-    def seed(self, seed: int, dynamic_seed: bool = True) -> None:
-        self._seed = seed
-        self._dynamic_seed = dynamic_seed
-        np.random.seed(self._seed)
+        return obs
 
-    def step(self, action: np.ndarray) -> BaseEnvTimestep:
+    def step(self, action: Union[int, np.ndarray]) -> BaseEnvTimestep:
         """
         Overview:
-             During the step phase, the environment first converts the discrete action into a continuous action,
-             and then passes it into the original environment.
+            Perform a step in the environment using the provided action, and return the next state of the environment.
+            The next state is encapsulated in a BaseEnvTimestep object, which includes the new observation, reward,
+            done flag, and info dictionary.
         Arguments:
-            - action (:obj:`np.ndarray`): Discrete action
+            - action (:obj:`Union[int, np.ndarray]`): The action to be performed in the environment. If the action is
+              a 1-dimensional numpy array, it is squeezed to a 0-dimension array.
         Returns:
-            - BaseEnvTimestep (:obj:`tuple`): Including observation, reward, done, and info.
+            - timestep (:obj:`BaseEnvTimestep`): An object containing the new observation, reward, done flag,
+              and info dictionary.
+        .. note::
+            - The cumulative reward (`_eval_episode_return`) is updated with the reward obtained in this step.
+            - If the episode ends (done is True), the total reward for the episode is stored in the info dictionary
+              under the key 'eval_episode_return'.
+            - An action mask is created with ones, which represents the availability of each action in the action space.
+            - Observations are returned in a dictionary format containing 'observation', 'action_mask', and 'to_play'.
         """
-        # disc_to_cont: transform discrete action index to original continuous action
-        action = [-1 + 2 / self.n * k for k in self.disc_to_cont[int(action)]]
-        action = to_ndarray(action)
-        if action.shape == (1, ):
-            action = action.squeeze()
-        if self._act_scale:
-            action = affine_transform(action, min_val=self._raw_action_space.low, max_val=self._raw_action_space.high)
-        if self._save_replay_gif:
-            self._frames.append(self._env.render(mode='rgb_array'))
-        obs, rew, done, info = self._env.step(action)
+        if isinstance(action, np.ndarray) and action.shape == (1,):
+            action = action.squeeze()  # 0-dim array
+
+        obs, rew, terminated, truncated, info = self._env.step(action)
+        done = terminated or truncated
 
-        action_mask = None
-        obs = {'observation': obs, 'action_mask': action_mask, 'to_play': -1}
         self._eval_episode_return += rew
-        if self._rew_clip:
-            rew = max(-10, rew)
-        rew = np.float32(rew)
         if done:
             info['eval_episode_return'] = self._eval_episode_return
-            if self._save_replay_gif:
-                if not os.path.exists(self._replay_path_gif):
-                    os.makedirs(self._replay_path_gif)
-                path = os.path.join(
-                    self._replay_path_gif,
-                    '{}_episode_{}_seed{}.gif'.format(self._env_id, self._save_replay_count, self._seed)
-                )
-                self.display_frames_as_gif(self._frames, path)
-                print(f'save episode {self._save_replay_count} in {self._replay_path_gif}!')
-                self._save_replay_count += 1
-        obs = to_ndarray(obs)
-        rew = to_ndarray([rew])
+
+        action_mask = np.ones(self.action_space.n, 'int8')
+        obs = {'observation': obs, 'action_mask': action_mask, 'to_play': -1}
+
         return BaseEnvTimestep(obs, rew, done, info)
 
-    @property
-    def legal_actions(self):
-        return np.arange(self._action_space.n)
+    def close(self) -> None:
+        """
+        Close the environment, and set the initialization flag to False.
+        """
+        if self._init_flag:
+            self._env.close()
+        self._init_flag = False
+
+    def seed(self, seed: int, dynamic_seed: bool = True) -> None:
+        """
+        Set the seed for the environment's random number generator. Can handle both static and dynamic seeding.
+        """
+        self._seed = seed
+        self._dynamic_seed = dynamic_seed
+        np.random.seed(self._seed)
 
     def enable_save_replay(self, replay_path: Optional[str] = None) -> None:
+        """
+        Enable the saving of replay videos. If no replay path is given, a default is used.
+        """
         if replay_path is None:
             replay_path = './video'
         self._replay_path = replay_path
-        self._save_replay_gif = True
-        self._save_replay_count = 0
-
-    @staticmethod
-    def display_frames_as_gif(frames: list, path: str) -> None:
-        import imageio
-        imageio.mimsave(path, frames, fps=20)
 
     def random_action(self) -> np.ndarray:
+        """
+         Generate a random action using the action space's sample method. Returns a numpy array containing the action.
+         """
         random_action = self.action_space.sample()
-        if isinstance(random_action, np.ndarray):
-            pass
-        elif isinstance(random_action, int):
-            random_action = to_ndarray([random_action], dtype=np.int64)
+        random_action = to_ndarray([random_action], dtype=np.int64)
         return random_action
 
     @property
     def observation_space(self) -> gym.spaces.Space:
+        """
+        Property to access the observation space of the environment.
+        """
         return self._observation_space
 
     @property
     def action_space(self) -> gym.spaces.Space:
+        """
+        Property to access the action space of the environment.
+        """
         return self._action_space
 
     @property
     def reward_space(self) -> gym.spaces.Space:
+        """
+        Property to access the reward space of the environment.
+        """
         return self._reward_space
 
     def __repr__(self) -> str:
-        return "DI-engine BipedalWalker Env"
-
-    @staticmethod
-    def create_collector_env_cfg(cfg: dict) -> List[dict]:
-        collector_env_num = cfg.pop('collector_env_num')
-        cfg = copy.deepcopy(cfg)
-        cfg.max_episode_steps = cfg.collect_max_episode_steps
-        return [cfg for _ in range(collector_env_num)]
-
-    @staticmethod
-    def create_evaluator_env_cfg(cfg: dict) -> List[dict]:
-        evaluator_env_num = cfg.pop('evaluator_env_num')
-        cfg = copy.deepcopy(cfg)
-        cfg.max_episode_steps = cfg.eval_max_episode_steps
-        return [cfg for _ in range(evaluator_env_num)]
+        """
+        String representation of the environment.
+        """
+        return "LightZero CartPole Env"
```

### Comparing `LightZero-0.0.2/zoo/box2d/lunarlander/config/lunarlander_cont_disc_efficientzero_config.py` & `LightZero-0.0.5/zoo/box2d/lunarlander/config/lunarlander_cont_disc_efficientzero_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 NOTE: the lunarlander_cont_disc in file name means we use the lunarlander continuous env ('LunarLanderContinuous-v2')
-with manually discretitze action space. That is to say, the final action space is discrete.
+with manually discretized action space. That is to say, the final action space is discrete.
 """
 from easydict import EasyDict
 
 # ==============================================================
 # begin of the most frequently changed config specified by the user
 # ==============================================================
 collector_env_num = 8
@@ -20,15 +20,15 @@
 # end of the most frequently changed config specified by the user
 # ==============================================================
 
 lunarlander_cont_disc_efficientzero_config = dict(
     exp_name=
     f'data_ez_ctree/lunarlander_cont_disc_efficientzero_ns{num_simulations}_upc{update_per_collect}_rr{reanalyze_ratio}_seed0',
     env=dict(
-        env_name='LunarLanderContinuous-v2',
+        env_id='LunarLanderContinuous-v2',
         continuous=False,
         manually_discretization=True,
         each_dim_disc_size=each_dim_disc_size,
         collector_env_num=collector_env_num,
         evaluator_env_num=evaluator_env_num,
         n_evaluator_episode=evaluator_env_num,
         manager=dict(shared_memory=False, ),
@@ -61,15 +61,15 @@
         evaluator_env_num=evaluator_env_num,
     ),
 )
 lunarlander_cont_disc_efficientzero_config = EasyDict(lunarlander_cont_disc_efficientzero_config)
 main_config = lunarlander_cont_disc_efficientzero_config
 
 lunarlander_cont_disc_efficientzero_create_config = dict(
-    # NOTE: here we use the lunarlander env with manually discretitze action space.
+    # NOTE: here we use the lunarlander env with manually discretized action space.
     env=dict(
         type='lunarlander_cont_disc',
         import_names=['zoo.box2d.lunarlander.envs.lunarlander_cont_disc_env'],
     ),
     env_manager=dict(type='subprocess'),
     policy=dict(
         type='efficientzero',
```

### Comparing `LightZero-0.0.2/zoo/box2d/lunarlander/config/lunarlander_cont_disc_sampled_efficientzero_config.py` & `LightZero-0.0.5/zoo/box2d/lunarlander/config/lunarlander_cont_disc_sampled_efficientzero_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # end of the most frequently changed config specified by the user
 # ==============================================================
 
 lunarlander_cont_disc_sampled_efficientzero_config = dict(
     exp_name=
     f'data_sez_ctree/lunarlander_cont_disc_sampled_efficientzero_k{K}_ns{num_simulations}_upc{update_per_collect}_rr{reanalyze_ratio}_seed0',
     env=dict(
-        env_name='LunarLanderContinuous-v2',
+        env_id='LunarLanderContinuous-v2',
         continuous=False,
         manually_discretization=True,
         each_dim_disc_size=each_dim_disc_size,
         collector_env_num=collector_env_num,
         evaluator_env_num=evaluator_env_num,
         n_evaluator_episode=evaluator_env_num,
         manager=dict(shared_memory=False, ),
@@ -63,15 +63,15 @@
         evaluator_env_num=evaluator_env_num,
     ),
 )
 lunarlander_cont_disc_sampled_efficientzero_config = EasyDict(lunarlander_cont_disc_sampled_efficientzero_config)
 main_config = lunarlander_cont_disc_sampled_efficientzero_config
 
 lunarlander_cont_disc_sampled_efficientzero_create_config = dict(
-    # NOTE: here we use the lunarlander env with manually discretitze action space.
+    # NOTE: here we use the lunarlander env with manually discretized action space.
     env=dict(
         type='lunarlander_cont_disc',
         import_names=['zoo.box2d.lunarlander.envs.lunarlander_cont_disc_env'],
     ),
     env_manager=dict(type='subprocess'),
     policy=dict(
         type='sampled_efficientzero',
```

### Comparing `LightZero-0.0.2/zoo/box2d/lunarlander/config/lunarlander_cont_sampled_efficientzero_config.py` & `LightZero-0.0.5/zoo/box2d/lunarlander/config/lunarlander_cont_sampled_efficientzero_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # end of the most frequently changed config specified by the user
 # ==============================================================
 
 lunarlander_cont_sampled_efficientzero_config = dict(
     exp_name=
     f'data_sez_ctree/lunarlander_cont_sampled_efficientzero_k{K}_ns{num_simulations}_upc{update_per_collect}_rr{reanalyze_ratio}_seed0',
     env=dict(
-        env_name='LunarLanderContinuous-v2',
+        env_id='LunarLanderContinuous-v2',
         continuous=True,
         manually_discretization=False,
         collector_env_num=collector_env_num,
         evaluator_env_num=evaluator_env_num,
         n_evaluator_episode=evaluator_env_num,
         manager=dict(shared_memory=False, ),
     ),
@@ -33,15 +33,15 @@
         mcts_ctree=True,
         model=dict(
             observation_shape=8,
             action_space_size=2,
             continuous_action_space=continuous_action_space,
             num_of_sampled_actions=K,
             sigma_type='conditioned',
-            model_type='mlp', 
+            model_type='mlp',
             lstm_hidden_size=256,
             latent_state_dim=256,
             res_connection_in_dynamics=True,
             norm_type='BN', 
         ),
         cuda=True,
         env_type='not_board_games',
```

### Comparing `LightZero-0.0.2/zoo/box2d/lunarlander/config/lunarlander_disc_efficientzero_config.py` & `LightZero-0.0.5/zoo/box2d/lunarlander/config/lunarlander_disc_efficientzero_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # end of the most frequently changed config specified by the user
 # ==============================================================
 
 lunarlander_disc_efficientzero_config = dict(
     exp_name=
     f'data_ez_ctree/lunarlander_disc_efficientzero_ns{num_simulations}_upc{update_per_collect}_rr{reanalyze_ratio}_seed0',
     env=dict(
-        env_name='LunarLander-v2',
+        env_id='LunarLander-v2',
         continuous=False,
         manually_discretization=False,
         collector_env_num=collector_env_num,
         evaluator_env_num=evaluator_env_num,
         n_evaluator_episode=evaluator_env_num,
         manager=dict(shared_memory=False, ),
     ),
```

### Comparing `LightZero-0.0.2/zoo/box2d/lunarlander/config/lunarlander_disc_gumbel_muzero_config.py` & `LightZero-0.0.5/zoo/box2d/lunarlander/config/lunarlander_disc_gumbel_muzero_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # ==============================================================
 # end of the most frequently changed config specified by the user
 # ==============================================================
 
 lunarlander_gumbel_muzero_config = dict(
     exp_name=f'data_mz_ctree/lunarlander_gumbel_muzero_ns{num_simulations}_upc{update_per_collect}_rr{reanalyze_ratio}_seed0',
     env=dict(
-        env_name='LunarLander-v2',
+        env_id='LunarLander-v2',
         continuous=False,
         manually_discretization=False,
         collector_env_num=collector_env_num,
         evaluator_env_num=evaluator_env_num,
         n_evaluator_episode=evaluator_env_num,
         manager=dict(shared_memory=False, ),
     ),
@@ -36,14 +36,16 @@
             self_supervised_learning_loss=True,  # NOTE: default is False.
             discrete_action_encoding_type='one_hot',
             res_connection_in_dynamics=True,
             norm_type='BN', 
         ),
         cuda=True,
         env_type='not_board_games',
+        # TODO: test the performance of varied_action_space.
+        action_type='varied_action_space',
         game_segment_length=200,
         update_per_collect=update_per_collect,
         batch_size=batch_size,
         optim_type='Adam',
         max_num_considered_actions=4,
         lr_piecewise_constant_decay=False,
         learning_rate=0.003,
@@ -62,15 +64,17 @@
 main_config = lunarlander_gumbel_muzero_config
 
 lunarlander_gumbel_muzero_create_config = dict(
     env=dict(
         type='lunarlander',
         import_names=['zoo.box2d.lunarlander.envs.lunarlander_env'],
     ),
-    env_manager=dict(type='subprocess'),
+    # TODO: test the performance of varied_action_space.
+    # env_manager=dict(type='subprocess'),
+    env_manager=dict(type='base'),
     policy=dict(
         type='gumbel_muzero',
         import_names=['lzero.policy.gumbel_muzero'],
     ),
 )
 lunarlander_gumbel_muzero_create_config = EasyDict(lunarlander_gumbel_muzero_create_config)
 create_config = lunarlander_gumbel_muzero_create_config
```

### Comparing `LightZero-0.0.2/zoo/box2d/lunarlander/config/lunarlander_disc_muzero_config.py` & `LightZero-0.0.5/zoo/box2d/lunarlander/config/lunarlander_disc_muzero_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # ==============================================================
 # end of the most frequently changed config specified by the user
 # ==============================================================
 
 lunarlander_muzero_config = dict(
     exp_name=f'data_mz_ctree/lunarlander_muzero_ns{num_simulations}_upc{update_per_collect}_rr{reanalyze_ratio}_seed0',
     env=dict(
-        env_name='LunarLander-v2',
+        env_id='LunarLander-v2',
         continuous=False,
         manually_discretization=False,
         collector_env_num=collector_env_num,
         evaluator_env_num=evaluator_env_num,
         n_evaluator_episode=evaluator_env_num,
         manager=dict(shared_memory=False, ),
     ),
```

### Comparing `LightZero-0.0.2/zoo/box2d/lunarlander/config/lunarlander_disc_stochastic_muzero_config.py` & `LightZero-0.0.5/zoo/box2d/lunarlander/config/lunarlander_disc_stochastic_muzero_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # ==============================================================
 # end of the most frequently changed config specified by the user
 # ==============================================================
 
 lunarlander_muzero_config = dict(
     exp_name=f'data_stochastic_mz_ctree/lunarlander_stochastic_muzero_ns{num_simulations}_upc{update_per_collect}_rr{reanalyze_ratio}_seed0',
     env=dict(
-        env_name='LunarLander-v2',
+        env_id='LunarLander-v2',
         continuous=False,
         manually_discretization=False,
         collector_env_num=collector_env_num,
         evaluator_env_num=evaluator_env_num,
         n_evaluator_episode=evaluator_env_num,
         manager=dict(shared_memory=False, ),
     ),
```

### Comparing `LightZero-0.0.2/zoo/box2d/lunarlander/envs/lunarlander_cont_disc_env.py` & `LightZero-0.0.5/zoo/box2d/lunarlander/envs/lunarlander_cont_disc_env.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,96 +1,123 @@
-from typing import Any, List, Union, Optional
-import gym
+import copy
 import os
+from datetime import datetime
+from itertools import product
+
+import gymnasium as gym
 import numpy as np
-from ding.envs import BaseEnv, BaseEnvTimestep
-from ding.torch_utils import to_ndarray, to_list
-from ding.utils import ENV_REGISTRY
-from ding.envs.common import affine_transform
-from ding.envs import ObsPlusPrevActRewWrapper
 from itertools import product
+from ding.envs import BaseEnvTimestep
+from ding.envs import ObsPlusPrevActRewWrapper
+from ding.envs.common import affine_transform
+from ding.torch_utils import to_ndarray
+from ding.utils import ENV_REGISTRY
 from easydict import EasyDict
-import copy
+
+from zoo.box2d.lunarlander.envs.lunarlander_env import LunarLanderEnv
 
 
 @ENV_REGISTRY.register('lunarlander_cont_disc')
-class LunarLanderDiscEnv(BaseEnv):
+class LunarLanderDiscEnv(LunarLanderEnv):
     """
-        Overview:
-            The modified LunarLander environment with manually discretized action space. For each dimension, equally dividing the
-            original continuous action into ``each_dim_disc_size`` bins and using their Cartesian product to obtain
-            handcrafted discrete actions.
+    Overview:
+        The modified LunarLander environment with manually discretized action space. For each dimension, it equally divides the
+        original continuous action into ``each_dim_disc_size`` bins and uses their Cartesian product to obtain
+        handcrafted discrete actions.
     """
 
     @classmethod
     def default_config(cls: type) -> EasyDict:
+        """
+        Overview:
+            Get the default configuration of the LunarLander environment.
+        Returns:
+            - cfg (:obj:`EasyDict`): Default configuration dictionary.
+        """
         cfg = EasyDict(copy.deepcopy(cls.config))
         cfg.cfg_type = cls.__name__ + 'Dict'
         return cfg
 
     config = dict(
+        # (str) The gym environment name.
+        env_id="LunarLander-v2",
+        # (int) The number of bins for each dimension of the action space.
+        each_dim_disc_size=4,
+        # (bool) If True, save the replay as a gif file.
         save_replay_gif=False,
+        # (str or None) The path to save the replay gif. If None, the replay gif will not be saved.
         replay_path_gif=None,
+        # (str or None) The path to save the replay. If None, the replay will not be saved.
         replay_path=None,
-        use_act_scale=False,
-        delay_reward_step=0,
-        prob_random_agent=0.,
+        # (bool) If True, the action will be scaled.
+        act_scale=True,
+        # (int) The maximum number of steps for each episode during collection.
         collect_max_episode_steps=int(1.08e5),
+        # (int) The maximum number of steps for each episode during evaluation.
         eval_max_episode_steps=int(1.08e5),
-        each_dim_disc_size=4,
     )
 
     def __init__(self, cfg: dict) -> None:
+        """
+        Overview:
+            Initialize the LunarLander environment with the given config dictionary.
+        Arguments:
+            - cfg (:obj:`dict`): Configuration dictionary.
+        """
         self._cfg = cfg
         self._init_flag = False
-        # env_name: LunarLander-v2, LunarLanderContinuous-v2
-        self._env_name = cfg.env_name
+        # env_id: LunarLander-v2, LunarLanderContinuous-v2
+        self._env_id = cfg.env_id
         self._replay_path = cfg.replay_path
         self._replay_path_gif = cfg.replay_path_gif
         self._save_replay_gif = cfg.save_replay_gif
         self._save_replay_count = 0
-        if 'Continuous' in self._env_name:
-            self._act_scale = cfg.use_act_scale  # act_scale only works in continuous env
+        if 'Continuous' in self._env_id:
+            self._act_scale = cfg.act_scale  # act_scale only works in continuous env
         else:
             self._act_scale = False
 
     def reset(self) -> np.ndarray:
         """
         Overview:
-             During the reset phase, the original environment will be created,
-             and at the same time, the action space will be discretized into "each_dim_disc_size" bins.
+            Reset the environment. During the reset phase, the original environment will be created,
+            and at the same time, the action space will be discretized into "each_dim_disc_size" bins.
         Returns:
             - info_dict (:obj:`Dict[str, Any]`): Including observation, action_mask, and to_play label.
         """
         if not self._init_flag:
-            self._env = gym.make(self._cfg.env_name)
+            self._env = gym.make(self._cfg.env_id, render_mode="rgb_array")
             if self._replay_path is not None:
+                timestamp = datetime.now().strftime("%Y%m%d%H%M%S")
+                video_name = f'{self._env.spec.id}-video-{timestamp}'
                 self._env = gym.wrappers.RecordVideo(
                     self._env,
                     video_folder=self._replay_path,
                     episode_trigger=lambda episode_id: True,
-                    name_prefix='rl-video-{}'.format(id(self))
+                    name_prefix=video_name
                 )
             if hasattr(self._cfg, 'obs_plus_prev_action_reward') and self._cfg.obs_plus_prev_action_reward:
                 self._env = ObsPlusPrevActRewWrapper(self._env)
             self._observation_space = self._env.observation_space
 
             self._reward_space = gym.spaces.Box(
                 low=self._env.reward_range[0], high=self._env.reward_range[1], shape=(1, ), dtype=np.float32
             )
             self._reward_space = gym.spaces.Box(
                 low=self._env.reward_range[0], high=self._env.reward_range[1], shape=(1, ), dtype=np.float32
             )
             self._init_flag = True
         if hasattr(self, '_seed') and hasattr(self, '_dynamic_seed') and self._dynamic_seed:
             np_seed = 100 * np.random.randint(1, 1000)
-            self._env.seed(self._seed + np_seed)
+            self._seed = self._seed + np_seed
+            obs, _ = self._env.reset(seed=self._seed)  # using the reset method of Gymnasium env
         elif hasattr(self, '_seed'):
-            self._env.seed(self._seed)
-        obs = self._env.reset()
+            obs, _ = self._env.reset(seed=self._seed)
+        else:
+            obs, _ = self._env.reset()
         obs = to_ndarray(obs)
         self._eval_episode_return = 0
         if self._save_replay_gif:
             self._frames = []
         # disc_to_cont: transform discrete action index to original continuous action
         self._raw_action_space = self._env.action_space
         self.m = self._raw_action_space.shape[0]
@@ -100,110 +127,57 @@
         # the modified discrete action space
         self._action_space = gym.spaces.Discrete(self.K)
 
         action_mask = np.ones(self.K, 'int8')
         obs = {'observation': obs, 'action_mask': action_mask, 'to_play': -1}
         return obs
 
-    def close(self) -> None:
-        if self._init_flag:
-            self._env.close()
-        self._init_flag = False
-
-    def render(self) -> None:
-        self._env.render()
-
-    def seed(self, seed: int, dynamic_seed: bool = True) -> None:
-        self._seed = seed
-        self._dynamic_seed = dynamic_seed
-        np.random.seed(self._seed)
-
     def step(self, action: np.ndarray) -> BaseEnvTimestep:
         """
         Overview:
-             During the step phase, the environment first converts the discrete action into a continuous action,
-             and then passes it into the original environment.
+            Take an action in the environment. During the step phase, the environment first converts the discrete action into a continuous action,
+            and then passes it into the original environment.
         Arguments:
-            - action (:obj:`np.ndarray`): Discrete action
+            - action (:obj:`np.ndarray`): Discrete action to be taken in the environment.
         Returns:
-            - BaseEnvTimestep (:obj:`tuple`): Including observation, reward, done, and info.
+            - BaseEnvTimestep (:obj:`BaseEnvTimestep`): A tuple containing observation, reward, done, and info.
         """
         action = [-1 + 2 / self.n * k for k in self.disc_to_cont[int(action)]]
         action = to_ndarray(action)
         if action.shape == (1, ):
             action = action.item()  # 0-dim array
         if self._act_scale:
             action = affine_transform(action, min_val=-1, max_val=1)
         if self._save_replay_gif:
-            self._frames.append(self._env.render(mode='rgb_array'))
-        obs, rew, done, info = self._env.step(action)
+            self._frames.append(self._env.render())
+        obs, rew, terminated, truncated, info = self._env.step(action)
+        done = terminated or truncated
 
         action_mask = np.ones(self._action_space.n, 'int8')
         obs = {'observation': obs, 'action_mask': action_mask, 'to_play': -1}
         self._eval_episode_return += rew
         if done:
             info['eval_episode_return'] = self._eval_episode_return
             if self._save_replay_gif:
-                print(self._replay_path)
-                if not os.path.exists(self._replay_path):
-                    os.makedirs(self._replay_path)
+                if not os.path.exists(self._replay_path_gif):
+                    os.makedirs(self._replay_path_gif)
+                timestamp = datetime.now().strftime("%Y%m%d%H%M%S")
                 path = os.path.join(
-                    self._replay_path, '{}_episode_{}.gif'.format(self._env_name, self._save_replay_count)
+                    self._replay_path_gif,
+                    '{}_episode_{}_seed{}_{}.gif'.format(self._env_id, self._save_replay_count, self._seed, timestamp)
                 )
                 self.display_frames_as_gif(self._frames, path)
+                print(f'save episode {self._save_replay_count} in {self._replay_path_gif}!')
                 self._save_replay_count += 1
         obs = to_ndarray(obs)
-        rew = to_ndarray([rew]).astype(np.float32)  # wrapped to be transferred to a array with shape (1,)
+        rew = to_ndarray([rew]).astype(np.float32)  # wrapped to be transferred to an array with shape (1,)
         return BaseEnvTimestep(obs, rew, done, info)
 
-    @property
-    def legal_actions(self):
-        return np.arange(self._action_space.n)
-
-    def enable_save_replay(self, replay_path: Optional[str] = None) -> None:
-        if replay_path is None:
-            replay_path = './video'
-        self._replay_path = replay_path
-        self._save_replay_gif = True
-        self._save_replay_count = 0
-
-    @staticmethod
-    def display_frames_as_gif(frames: list, path: str) -> None:
-        import imageio
-        imageio.mimsave(path, frames, fps=20)
-
-    def random_action(self) -> np.ndarray:
-        random_action = self.action_space.sample()
-        if isinstance(random_action, np.ndarray):
-            pass
-        elif isinstance(random_action, int):
-            random_action = to_ndarray([random_action], dtype=np.int64)
-        return random_action
-
-    @property
-    def observation_space(self) -> gym.spaces.Space:
-        return self._observation_space
-
-    @property
-    def action_space(self) -> gym.spaces.Space:
-        return self._action_space
-
-    @property
-    def reward_space(self) -> gym.spaces.Space:
-        return self._reward_space
-
     def __repr__(self) -> str:
-        return "DI-engine LunarLander Env"
+        """
+        Overview:
+            Represent the environment instance as a string.
+        Returns:
+            - repr_str (:obj:`str`): Representation string of the environment instance.
+        """
+        return "LightZero LunarLander Env (with manually discretized action space)"
 
-    @staticmethod
-    def create_collector_env_cfg(cfg: dict) -> List[dict]:
-        collector_env_num = cfg.pop('collector_env_num')
-        cfg = copy.deepcopy(cfg)
-        cfg.max_episode_steps = cfg.collect_max_episode_steps
-        return [cfg for _ in range(collector_env_num)]
-
-    @staticmethod
-    def create_evaluator_env_cfg(cfg: dict) -> List[dict]:
-        evaluator_env_num = cfg.pop('evaluator_env_num')
-        cfg = copy.deepcopy(cfg)
-        cfg.max_episode_steps = cfg.eval_max_episode_steps
-        return [cfg for _ in range(evaluator_env_num)]
```

### Comparing `LightZero-0.0.2/zoo/classic_control/cartpole/config/cartpole_efficientzero_config.py` & `LightZero-0.0.5/zoo/classic_control/cartpole/config/cartpole_efficientzero_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # end of the most frequently changed config specified by the user
 # ==============================================================
 
 cartpole_efficientzero_config = dict(
     exp_name=
     f'data_ez_ctree/cartpole_efficientzero_ns{num_simulations}_upc{update_per_collect}_rr{reanalyze_ratio}_seed0',
     env=dict(
-        env_name='CartPole-v0',
+        env_id='CartPole-v0',
         continuous=False,
         manually_discretization=False,
         collector_env_num=collector_env_num,
         evaluator_env_num=evaluator_env_num,
         n_evaluator_episode=evaluator_env_num,
         manager=dict(shared_memory=False, ),
     ),
```

### Comparing `LightZero-0.0.2/zoo/classic_control/cartpole/config/cartpole_gumbel_muzero_config.py` & `LightZero-0.0.5/zoo/classic_control/cartpole/config/cartpole_gumbel_muzero_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # ==============================================================
 # end of the most frequently changed config specified by the user
 # ==============================================================
 
 cartpole_gumbel_muzero_config = dict(
     exp_name=f'data_mz_ctree/cartpole_gumbel_muzero_ns{num_simulations}_upc{update_per_collect}_rr{reanalyze_ratio}_seed0',
     env=dict(
-        env_name='CartPole-v0',
+        env_id='CartPole-v0',
         continuous=False,
         manually_discretization=False,
         collector_env_num=collector_env_num,
         evaluator_env_num=evaluator_env_num,
         n_evaluator_episode=evaluator_env_num,
         manager=dict(shared_memory=False, ),
     ),
```

### Comparing `LightZero-0.0.2/zoo/classic_control/cartpole/config/cartpole_muzero_config.py` & `LightZero-0.0.5/zoo/classic_control/cartpole/config/cartpole_muzero_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # ==============================================================
 # end of the most frequently changed config specified by the user
 # ==============================================================
 
 cartpole_muzero_config = dict(
     exp_name=f'data_mz_ctree/cartpole_muzero_ns{num_simulations}_upc{update_per_collect}_rr{reanalyze_ratio}_seed0',
     env=dict(
-        env_name='CartPole-v0',
+        env_id='CartPole-v0',
         continuous=False,
         manually_discretization=False,
         collector_env_num=collector_env_num,
         evaluator_env_num=evaluator_env_num,
         n_evaluator_episode=evaluator_env_num,
         manager=dict(shared_memory=False, ),
     ),
@@ -35,14 +35,15 @@
             latent_state_dim=128,
             self_supervised_learning_loss=True,  # NOTE: default is False.
             discrete_action_encoding_type='one_hot',
             norm_type='BN', 
         ),
         cuda=True,
         env_type='not_board_games',
+        action_type='varied_action_space',
         game_segment_length=50,
         update_per_collect=update_per_collect,
         batch_size=batch_size,
         optim_type='Adam',
         lr_piecewise_constant_decay=False,
         learning_rate=0.003,
         ssl_loss_weight=2,  # NOTE: default is 0.
```

### Comparing `LightZero-0.0.2/zoo/classic_control/cartpole/config/cartpole_muzero_config_ckpt.py` & `LightZero-0.0.5/zoo/classic_control/cartpole/config/cartpole_muzero_config_ckpt_tmp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 from easydict import EasyDict
 
 # ==============================================================
 # begin of the most frequently changed config specified by the user
 # ==============================================================
-collector_env_num = 8
-n_episode = 8
-evaluator_env_num = 3
+# collector_env_num = 8
+# n_episode = 8
+# evaluator_env_num = 3
+
+collector_env_num = 2
+n_episode = 2
+evaluator_env_num = 2
+
 num_simulations = 25
 update_per_collect = 100
 batch_size = 256
-max_env_step = int(1e5)
+max_env_step = int(500)
 reanalyze_ratio = 0
 # ==============================================================
 # end of the most frequently changed config specified by the user
 # ==============================================================
 
 cartpole_muzero_config = dict(
     exp_name=f'data_mz_ctree/cartpole_muzero_ns{num_simulations}_upc{update_per_collect}_rr{reanalyze_ratio}_seed0',
@@ -23,25 +28,14 @@
         manually_discretization=False,
         collector_env_num=collector_env_num,
         evaluator_env_num=evaluator_env_num,
         n_evaluator_episode=evaluator_env_num,
         manager=dict(shared_memory=False, ),
     ),
     policy=dict(
-        learn=dict(
-            learner=dict(
-                hook=dict(
-                    # load_ckpt_before_run='',
-                    log_show_after_iter=100,
-                    save_ckpt_after_iter=2,
-                    save_ckpt_after_run=True,
-                ),
-                # cfg_type='BaseLearnerDict',
-            ),
-        ),
         model=dict(
             observation_shape=4,
             action_space_size=2,
             model_type='mlp', 
             lstm_hidden_size=128,
             latent_state_dim=128,
             self_supervised_learning_loss=True,  # NOTE: default is False.
@@ -56,15 +50,25 @@
         optim_type='Adam',
         lr_piecewise_constant_decay=False,
         learning_rate=0.003,
         ssl_loss_weight=2,  # NOTE: default is 0.
         num_simulations=num_simulations,
         reanalyze_ratio=reanalyze_ratio,
         n_episode=n_episode,
-        eval_freq=int(2e2),
+        eval_freq=int(1e2),
+        eval_offline=True,
+        learn=dict(
+            learner=dict(
+                hook=dict(
+                    log_show_after_iter=100,
+                    save_ckpt_after_iter=100,
+                    save_ckpt_after_run=True,
+                ),
+            ),
+        ),
         replay_buffer_size=int(1e6),  # the size/capacity of replay_buffer, in the terms of transitions.
         collector_env_num=collector_env_num,
         evaluator_env_num=evaluator_env_num,
     ),
 )
 
 cartpole_muzero_config = EasyDict(cartpole_muzero_config)
```

### Comparing `LightZero-0.0.2/zoo/classic_control/cartpole/config/cartpole_sampled_efficientzero_config.py` & `LightZero-0.0.5/zoo/classic_control/cartpole/config/cartpole_sampled_efficientzero_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # end of the most frequently changed config specified by the user
 # ==============================================================
 
 cartpole_sampled_efficientzero_config = dict(
     exp_name=
     f'data_sez_ctree/cartpole_sampled_efficientzero_ns{num_simulations}_upc{update_per_collect}_rr{reanalyze_ratio}_seed0',
     env=dict(
-        env_name='CartPole-v0',
+        env_id='CartPole-v0',
         continuous=False,
         manually_discretization=False,
         collector_env_num=collector_env_num,
         evaluator_env_num=evaluator_env_num,
         n_evaluator_episode=evaluator_env_num,
         manager=dict(shared_memory=False, ),
     ),
```

### Comparing `LightZero-0.0.2/zoo/classic_control/cartpole/config/cartpole_stochastic_muzero_config.py` & `LightZero-0.0.5/zoo/classic_control/cartpole/config/cartpole_stochastic_muzero_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # ==============================================================
 # end of the most frequently changed config specified by the user
 # ==============================================================
 
 cartpole_stochastic_muzero_config = dict(
     exp_name=f'data_stochastic_mz_ctree/cartpole_stochastic_muzero_ns{num_simulations}_upc{update_per_collect}_rr{reanalyze_ratio}_seed0',
     env=dict(
-        env_name='CartPole-v0',
+        env_id='CartPole-v0',
         continuous=False,
         manually_discretization=False,
         collector_env_num=collector_env_num,
         evaluator_env_num=evaluator_env_num,
         n_evaluator_episode=evaluator_env_num,
         manager=dict(shared_memory=False, ),
     ),
```

### Comparing `LightZero-0.0.2/zoo/classic_control/pendulum/config/pendulum_cont_disc_efficientzero_config.py` & `LightZero-0.0.5/zoo/classic_control/pendulum/config/pendulum_cont_disc_efficientzero_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # end of the most frequently changed config specified by the user
 # ==============================================================
 
 pendulum_disc_efficientzero_config = dict(
     exp_name=
     f'data_ez_ctree/pendulum_disc_efficientzero_ns{num_simulations}_upc{update_per_collect}_rr{reanalyze_ratio}_seed0',
     env=dict(
-        env_name='Pendulum-v1',
+        env_id='Pendulum-v1',
         continuous=False,
         manually_discretization=True,
         each_dim_disc_size=11,
         collector_env_num=collector_env_num,
         evaluator_env_num=evaluator_env_num,
         n_evaluator_episode=evaluator_env_num,
         manager=dict(shared_memory=False, ),
```

### Comparing `LightZero-0.0.2/zoo/classic_control/pendulum/config/pendulum_cont_disc_gumbel_muzero_config.py` & `LightZero-0.0.5/zoo/classic_control/pendulum/config/pendulum_cont_disc_gumbel_muzero_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 NOTE: the pendulum_cont_disc in file name means we use the Pendulum-v1 continuous env
-with manually discretitze action space. That is to say, the final action space is discrete.
+with manually discretized action space. That is to say, the final action space is discrete.
 """
 from easydict import EasyDict
 
 # ==============================================================
 # begin of the most frequently changed config specified by the user
 # ==============================================================
 collector_env_num = 8
@@ -18,15 +18,15 @@
 # ==============================================================
 # end of the most frequently changed config specified by the user
 # ==============================================================
 
 pendulum_disc_gumbel_muzero_config = dict(
     exp_name=f'data_mz_ctree/pendulum_disc_gumbel_muzero_ns{num_simulations}_upc{update_per_collect}_rr{reanalyze_ratio}_seed0',
     env=dict(
-        env_name='Pendulum-v1',
+        env_id='Pendulum-v1',
         continuous=False,
         manually_discretization=True,
         each_dim_disc_size=11,
         collector_env_num=collector_env_num,
         evaluator_env_num=evaluator_env_num,
         n_evaluator_episode=evaluator_env_num,
         manager=dict(shared_memory=False, ),
```

### Comparing `LightZero-0.0.2/zoo/classic_control/pendulum/config/pendulum_cont_disc_muzero_config.py` & `LightZero-0.0.5/zoo/classic_control/pendulum/config/pendulum_cont_disc_muzero_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 NOTE: the pendulum_cont_disc in file name means we use the Pendulum-v1 continuous env
-with manually discretitze action space. That is to say, the final action space is discrete.
+with manually discretized action space. That is to say, the final action space is discrete.
 """
 from easydict import EasyDict
 
 # ==============================================================
 # begin of the most frequently changed config specified by the user
 # ==============================================================
 collector_env_num = 8
@@ -18,15 +18,15 @@
 # ==============================================================
 # end of the most frequently changed config specified by the user
 # ==============================================================
 
 pendulum_disc_muzero_config = dict(
     exp_name=f'data_ez_ctree/pendulum_disc_muzero_ns{num_simulations}_upc{update_per_collect}_rr{reanalyze_ratio}_seed0',
     env=dict(
-        env_name='Pendulum-v1',
+        env_id='Pendulum-v1',
         continuous=False,
         manually_discretization=True,
         each_dim_disc_size=11,
         collector_env_num=collector_env_num,
         evaluator_env_num=evaluator_env_num,
         n_evaluator_episode=evaluator_env_num,
         manager=dict(shared_memory=False, ),
```

### Comparing `LightZero-0.0.2/zoo/classic_control/pendulum/config/pendulum_cont_disc_sampled_efficientzero_config.py` & `LightZero-0.0.5/zoo/classic_control/pendulum/config/pendulum_cont_disc_sampled_efficientzero_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # end of the most frequently changed config specified by the user
 # ==============================================================
 
 pendulum_sampled_efficientzero_config = dict(
     exp_name=
     f'data_sez_ctree/pendulum_disc_sampled_efficientzero_k{K}_ns{num_simulations}_upc{update_per_collect}_rr{reanalyze_ratio}_seed0',
     env=dict(
-        env_name='Pendulum-v1',
+        env_id='Pendulum-v1',
         continuous=False,
         manually_discretization=True,
         each_dim_disc_size=11,
         collector_env_num=collector_env_num,
         evaluator_env_num=evaluator_env_num,
         n_evaluator_episode=evaluator_env_num,
         manager=dict(shared_memory=False, ),
```

### Comparing `LightZero-0.0.2/zoo/classic_control/pendulum/config/pendulum_cont_sampled_efficientzero_config.py` & `LightZero-0.0.5/zoo/classic_control/pendulum/config/pendulum_cont_sampled_efficientzero_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # end of the most frequently changed config specified by the user
 # ==============================================================
 
 pendulum_sampled_efficientzero_config = dict(
     exp_name=
     f'data_sez_ctree/pendulum_sampled_efficientzero_k{K}_ns{num_simulations}_upc{update_per_collect}_rr{reanalyze_ratio}_seed0',
     env=dict(
-        env_name='Pendulum-v1',
+        env_id='Pendulum-v1',
         continuous=True,
         manually_discretization=False,
         collector_env_num=collector_env_num,
         evaluator_env_num=evaluator_env_num,
         n_evaluator_episode=evaluator_env_num,
         manager=dict(shared_memory=False, ),
     ),
```

### Comparing `LightZero-0.0.2/zoo/classic_control/pendulum/entry/pendulum_eval.py` & `LightZero-0.0.5/zoo/classic_control/mountain_car/entry/mountain_car_eval.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,38 +1,56 @@
-# According to the model you want to evaluate, import the corresponding config.
-from zoo.classic_control.pendulum.config.pendulum_cont_sampled_efficientzero_config import main_config, create_config
+from zoo.classic_control.mountain_car.config.mtcar_muzero_config import main_config, create_config
 from lzero.entry import eval_muzero
 import numpy as np
 
 if __name__ == "__main__":
-    """ 
-    model_path (:obj:`Optional[str]`): The pretrained model path, which should
-    point to the ckpt file of the pretrained model, and an absolute path is recommended.
-    In LightZero, the path is usually something like ``exp_name/ckpt/ckpt_best.pth.tar``.
     """
-    model_path = "./ckpt/ckpt_best.pth.tar"
-    seeds = [0]
-    num_episodes_each_seed = 5
-    main_config.env.evaluator_env_num = 1
-    main_config.env.n_evaluator_episode = 1
-    total_test_episodes = num_episodes_each_seed * len(seeds)
+    Entry point for the evaluation of the MuZero model on the CartPole environment. 
+
+    Variables:
+        - model_path (:obj:`Optional[str]`): The pretrained model path, which should point to the ckpt file of the 
+        pretrained model. An absolute path is recommended. In LightZero, the path is usually something like 
+        ``exp_name/ckpt/ckpt_best.pth.tar``.
+        - returns_mean_seeds (:obj:`List[float]`): List to store the mean returns for each seed.
+        - returns_seeds (:obj:`List[float]`): List to store the returns for each seed.
+        - seeds (:obj:`List[int]`): List of seeds for the environment.
+        - num_episodes_each_seed (:obj:`int`): Number of episodes to run for each seed.
+        - total_test_episodes (:obj:`int`): Total number of test episodes, computed as the product of the number of 
+        seeds and the number of episodes per seed.
+    """
+    # model_path = "./ckpt/ckpt_best.pth.tar"
+    model_path = None
     returns_mean_seeds = []
     returns_seeds = []
+    seeds = [0]
+    num_episodes_each_seed = 2
+    total_test_episodes = num_episodes_each_seed * len(seeds)
+    create_config.env_manager.type = 'base'  # Visualization requires the 'type' to be set as base
+    main_config.env.evaluator_env_num = 1  # Visualization requires the 'env_num' to be set as 1
+    main_config.env.n_evaluator_episode = total_test_episodes
+    main_config.env.replay_path = './video'
+    main_config.exp_name = f'lz_result/eval/muzero_eval_ls{main_config.policy.model.latent_state_dim}'
+
     for seed in seeds:
-        returns_mean, returns = eval_muzero(
+        """
+        - returns_mean (:obj:`float`): The mean return of the evaluation.
+        - returns (:obj:`List[float]`): The returns of the evaluation.
+        """
+        returns_mean, returns, trajectorys = eval_muzero(
             [main_config, create_config],
             seed=seed,
             num_episodes_each_seed=num_episodes_each_seed,
             print_seed_details=False,
             model_path=model_path
         )
         returns_mean_seeds.append(returns_mean)
         returns_seeds.append(returns)
 
     returns_mean_seeds = np.array(returns_mean_seeds)
     returns_seeds = np.array(returns_seeds)
 
+    # Print evaluation results
     print("=" * 20)
-    print(f'We eval total {len(seeds)} seeds. In each seed, we eval {num_episodes_each_seed} episodes.')
-    print(f'In seeds {seeds}, returns_mean_seeds is {returns_mean_seeds}, returns is {returns_seeds}')
-    print('In all seeds, reward_mean:', returns_mean_seeds.mean())
-    print("=" * 20)
+    print(f"We evaluated a total of {len(seeds)} seeds. For each seed, we evaluated {num_episodes_each_seed} episode(s).")
+    print(f"For seeds {seeds}, the mean returns are {returns_mean_seeds}, and the returns are {returns_seeds}.")
+    print("Across all seeds, the mean reward is:", returns_mean_seeds.mean())
+    print("=" * 20)
```

### Comparing `LightZero-0.0.2/zoo/game_2048/entry/2048_bot_eval.py` & `LightZero-0.0.5/zoo/game_2048/entry/2048_bot_eval.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 from rich import print
 
 from zoo.game_2048.envs.expectimax_search_based_bot import expectimax_search
 from zoo.game_2048.envs.game_2048_env import Game2048Env
 
 # Define game configuration
 config = EasyDict(dict(
-    env_name="game_2048",
+    env_id="game_2048",
     # (str) The render mode. Options are 'None', 'state_realtime_mode', 'image_realtime_mode' or 'image_savefile_mode'.
     # If None, then the game will not be rendered.
     render_mode='image_realtime_mode',
     replay_format='gif',
     replay_name_suffix='bot',
     replay_path=None,
     act_scale=True,
-    channel_last=True,
+    channel_last=False,
     obs_type='raw_board',  # options=['raw_board', 'raw_encoded_board', 'dict_encoded_board']
     reward_type='raw',  # options=['raw', 'merged_tiles_plus_log_max_tile_num']
     reward_normalize=False,
     reward_norm_scale=100,
     max_tile=int(2 ** 16),
     delay_reward_step=0,
     prob_random_agent=0.,
```

### Comparing `LightZero-0.0.2/zoo/game_2048/entry/2048_eval.py` & `LightZero-0.0.5/zoo/board_games/tictactoe/entry/tictactoe_alphazero_eval.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,60 @@
-# According to the model you want to evaluate, import the corresponding config.
+from zoo.board_games.tictactoe.config.tictactoe_alphazero_bot_mode_config import main_config, create_config
+from lzero.entry import eval_alphazero
 import numpy as np
 
-from lzero.entry import eval_muzero
-from zoo.game_2048.config.muzero_2048_config import main_config, create_config
-from zoo.game_2048.config.stochastic_muzero_2048_config import main_config, create_config
-
-if __name__ == "__main__":
-    """ 
-    model_path (:obj:`Optional[str]`): The pretrained model path, which should
-    point to the ckpt file of the pretrained model, and an absolute path is recommended.
-    In LightZero, the path is usually something like ``exp_name/ckpt/ckpt_best.pth.tar``.
+if __name__ == '__main__':
     """
+    Entry point for the evaluation of the AlphaZero model on the TicTacToe environment. 
 
-    model_path = "./ckpt/ckpt_best.pth.tar"
-
-    returns_mean_seeds = []
-    returns_seeds = []
+    Variables:
+        - model_path (:obj:`Optional[str]`): The pretrained model path, which should point to the ckpt file of the 
+        pretrained model. An absolute path is recommended. In LightZero, the path is usually something like 
+        ``exp_name/ckpt/ckpt_best.pth.tar``.
+        - returns_mean_seeds (:obj:`List[float]`): List to store the mean returns for each seed.
+        - returns_seeds (:obj:`List[float]`): List to store the returns for each seed.
+        - seeds (:obj:`List[int]`): List of seeds for the environment.
+        - num_episodes_each_seed (:obj:`int`): Number of episodes to run for each seed.
+        - total_test_episodes (:obj:`int`): Total number of test episodes, computed as the product of the number of 
+        seeds and the number of episodes per seed.
+    """
+    # model_path = './ckpt/ckpt_best.pth.tar'
+    model_path = None
     seeds = [0]
     num_episodes_each_seed = 1
-    total_test_episodes = num_episodes_each_seed * len(seeds)
-    create_config.env_manager.type = 'base'  # Visualization requires the 'type' to be set as base
-    main_config.env.evaluator_env_num = 1   # Visualization requires the 'env_num' to be set as 1
-    main_config.env.n_evaluator_episode = total_test_episodes
-    main_config.env.save_replay = True  # Whether to save the replay, if save the video render_mode_human must to be True
-    main_config.env.replay_format = 'gif'
-    main_config.env.replay_name_suffix = 'muzero_ns100_s0'
-    # main_config.env.replay_name_suffix = 'stochastic_muzero_ns100_s0'
 
-    main_config.env.replay_path = None
-    main_config.env.max_episode_steps = int(1e9)  # Adjust according to different environments
+    # Enable saving of replay as a gif, specify the path to save the replay gif
+    main_config.env.replay_path = './video'
 
+    main_config.policy.mcts_ctree = False
+    # If True, you can play with the agent.
+    main_config.env.agent_vs_human = False
+    create_config.env_manager.type = 'base'
+    main_config.env.evaluator_env_num = 1
+    main_config.env.n_evaluator_episode = 1
+    total_test_episodes = num_episodes_each_seed * len(seeds)
+
+    returns_mean_seeds = []
+    returns_seeds = []
     for seed in seeds:
-        returns_mean, returns = eval_muzero(
+        returns_mean, returns = eval_alphazero(
             [main_config, create_config],
             seed=seed,
             num_episodes_each_seed=num_episodes_each_seed,
-            print_seed_details=False,
+            print_seed_details=True,
             model_path=model_path
         )
-        print(returns_mean, returns)
         returns_mean_seeds.append(returns_mean)
         returns_seeds.append(returns)
 
     returns_mean_seeds = np.array(returns_mean_seeds)
     returns_seeds = np.array(returns_seeds)
 
+    # Print evaluation results
     print("=" * 20)
-    print(f'We eval total {len(seeds)} seeds. In each seed, we eval {num_episodes_each_seed} episodes.')
-    print(f'In seeds {seeds}, returns_mean_seeds is {returns_mean_seeds}, returns is {returns_seeds}')
-    print('In all seeds, reward_mean:', returns_mean_seeds.mean())
+    print(f"We evaluated a total of {len(seeds)} seeds. For each seed, we evaluated {num_episodes_each_seed} episode(s).")
+    print(f"For seeds {seeds}, the mean returns are {returns_mean_seeds}, and the returns are {returns_seeds}.")
+    print("Across all seeds, the mean reward is:", returns_mean_seeds.mean())
+    print(
+        f'win rate: {len(np.where(returns_seeds == 1.)[0]) / total_test_episodes}, draw rate: {len(np.where(returns_seeds == 0.)[0]) / total_test_episodes}, lose rate: {len(np.where(returns_seeds == -1.)[0]) / total_test_episodes}'
+    )
     print("=" * 20)
```

### Comparing `LightZero-0.0.2/zoo/game_2048/envs/expectimax_search_based_bot.py` & `LightZero-0.0.5/zoo/game_2048/envs/expectimax_search_based_bot.py`

 * *Files identical despite different names*

### Comparing `LightZero-0.0.2/zoo/game_2048/envs/game_2048_env.py` & `LightZero-0.0.5/zoo/game_2048/envs/game_2048_env.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import copy
 import logging
+import os
 import sys
 from typing import List
 
-import gym
+import gymnasium as gym
 import imageio
 import matplotlib.font_manager as fm
 import matplotlib.pyplot as plt
 import numpy as np
 from PIL import Image, ImageDraw, ImageFont
 from ding.envs import BaseEnvTimestep
 from ding.torch_utils import to_ndarray
 from ding.utils import ENV_REGISTRY
 from easydict import EasyDict
-from gym import spaces
-from gym.utils import seeding
+from gymnasium import spaces
+from gymnasium.utils import seeding
 
 
 @ENV_REGISTRY.register('game_2048')
 class Game2048Env(gym.Env):
     """
     Overview:
         The Game2048Env is a gym environment implementation of the 2048 game. The goal of the game is to slide numbered tiles
@@ -84,29 +85,29 @@
             With 'image_savefile_mode', the game is rendered as an RGB image but not displayed in real-time. Instead, the image is saved to a designated file.
             Please note that the default rendering mode is set to None.
       """
 
     # The default_config for game 2048 env.
     config = dict(
         # (str) The name of the environment registered in the environment registry.
-        env_name="game_2048",
+        env_id="game_2048",
         # (str) The render mode. Options are 'None', 'state_realtime_mode', 'image_realtime_mode' or 'image_savefile_mode'.
         # If None, then the game will not be rendered.
         render_mode=None,
         # (str) The format in which to save the replay. 'gif' is a popular choice.
         replay_format='gif',
         # (str) A suffix for the replay file name to distinguish it from other files.
         replay_name_suffix='eval',
         # (str or None) The directory in which to save the replay file. If None, the file is saved in the current directory.
         replay_path=None,
         # (bool) Whether to scale the actions. If True, actions are divided by the action space size.
         act_scale=True,
         # (bool) Whether to use the 'channel last' format for the observation space.
         # If False, 'channel first' format is used.
-        channel_last=True,
+        channel_last=False,
         # (str) The type of observation to use. Options are 'raw_board', 'raw_encoded_board', and 'dict_encoded_board'.
         obs_type='dict_encoded_board',
         # (bool) Whether to normalize rewards. If True, rewards are divided by the maximum possible reward.
         reward_normalize=False,
         # (float) The factor to scale rewards by when reward normalization is used.
         reward_norm_scale=100,
         # (str) The type of reward to use. 'raw' means the raw game score. 'merged_tiles_plus_log_max_tile_num' is an alternative.
@@ -138,19 +139,19 @@
         cfg = EasyDict(copy.deepcopy(cls.config))
         cfg.cfg_type = cls.__name__ + 'Dict'
         return cfg
 
     def __init__(self, cfg: dict) -> None:
         self._cfg = cfg
         self._init_flag = False
-        self._env_name = cfg.env_name
+        self._env_id = cfg.env_id
         self.replay_format = cfg.replay_format
         self.replay_name_suffix = cfg.replay_name_suffix
         self.replay_path = cfg.replay_path
-        self.render_mode = cfg.render_mode 
+        self.render_mode = cfg.render_mode
 
         self.channel_last = cfg.channel_last
         self.obs_type = cfg.obs_type
         self.reward_type = cfg.reward_type
         self.reward_normalize = cfg.reward_normalize
         self.reward_norm_scale = cfg.reward_norm_scale
         assert self.reward_type in ['raw', 'merged_tiles_plus_log_max_tile_num']
@@ -351,16 +352,16 @@
         if self.render_mode is not None:
             self.render(self.render_mode)
 
         # If the game has ended, save additional information and the replay if necessary
         if done:
             info['eval_episode_return'] = self._final_eval_reward
             if self.render_mode == 'image_savefile_mode':
-                    self.save_render_output(replay_name_suffix=self.replay_name_suffix, replay_path=self.replay_path,
-                                            format=self.replay_format)
+                self.save_render_output(replay_name_suffix=self.replay_name_suffix, replay_path=self.replay_path,
+                                        format=self.replay_format)
 
         return BaseEnvTimestep(observation, reward, done, info)
 
     def move(self, direction, trial=False):
         """
         Overview:
             Perform one move in the game. The game board can be shifted in one of four directions: up (0), right (1), down (2), or left (3).
@@ -709,17 +710,19 @@
             text_x_size, text_y_size = bbox[2] - bbox[0], bbox[3] - bbox[1]
             draw.text((x * grid_size + (grid_size - text_x_size) // 2,
                        y * grid_size + (grid_size - text_y_size) // 2), str(o), font=fnt, fill=white)
 
     def save_render_output(self, replay_name_suffix: str = '', replay_path=None, format='gif'):
         # At the end of the episode, save the frames to a gif or mp4 file
         if replay_path is None:
-            filename = f'game_2048_{replay_name_suffix}.{format}'
+            filename = f'2048_{replay_name_suffix}.{format}'
         else:
-            filename = f'{replay_path}.{format}'
+            if not os.path.exists(replay_path):
+                os.makedirs(replay_path)
+            filename = replay_path + f'/2048_{replay_name_suffix}.{format}'
 
         if format == 'gif':
             imageio.mimsave(filename, self.frames, 'GIF')
         elif format == 'mp4':
             imageio.mimsave(filename, self.frames, fps=30, codec='mpeg4')
 
         else:
```

### Comparing `LightZero-0.0.2/zoo/game_2048/envs/test_game_2048_env.py` & `LightZero-0.0.5/zoo/game_2048/envs/test_game_2048_env.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 
 
 @pytest.mark.unittest
 class TestGame2048():
     def setup(self) -> None:
         # Configuration for the Game2048 environment
         cfg = EasyDict(dict(
-            env_name="game_2048",
+            env_id="game_2048",
             # (str) The render mode. Options are 'None', 'state_realtime_mode', 'image_realtime_mode' or 'image_savefile_mode'.  If None, then the game will not be rendered.
             render_mode=None,
             replay_format='gif',
             replay_name_suffix='eval',
             replay_path=None,
             act_scale=True,
-            channel_last=True,
+            channel_last=False,
             # (str) The type of observation to use. Options are 'raw_board', 'raw_encoded_board', and 'dict_encoded_board'.
             obs_type='raw_encoded_board',
             reward_type='raw',  # options=['raw', 'merged_tiles_plus_log_max_tile_num']
             reward_normalize=False,
             reward_norm_scale=100,
             max_tile=int(2 ** 16),  # 2**11=2048, 2**16=65536
             delay_reward_step=0,
```

### Comparing `LightZero-0.0.2/zoo/minigrid/config/minigrd_sampled_efficientzero_config.py` & `LightZero-0.0.5/zoo/minigrid/config/minigrd_sampled_efficientzero_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from easydict import EasyDict
 
 # The typical MiniGrid env id: {'MiniGrid-Empty-8x8-v0', 'MiniGrid-FourRooms-v0', 'MiniGrid-DoorKey-8x8-v0','MiniGrid-DoorKey-16x16-v0'},
 # please refer to https://github.com/Farama-Foundation/MiniGrid for details.
-env_name = 'MiniGrid-Empty-8x8-v0'
+env_id = 'MiniGrid-Empty-8x8-v0'
 max_env_step = int(1e6)
 # ==============================================================
 # begin of the most frequently changed config specified by the user
 # ==============================================================
 seed = 0
 
 collector_env_num = 8
@@ -25,17 +25,17 @@
 threshold_training_steps_for_final_temperature = int(5e5)
 eps_greedy_exploration_in_collect = False
 # ==============================================================
 # end of the most frequently changed config specified by the user
 # ==============================================================
 
 minigrid_sampled_efficientzero_config = dict(
-    exp_name=f'data_sez_ctree/{env_name}_sampled_efficientzero_ns{num_simulations}_upc{update_per_collect}_rr{reanalyze_ratio}_seed{seed}',
+    exp_name=f'data_sez_ctree/{env_id}_sampled_efficientzero_ns{num_simulations}_upc{update_per_collect}_rr{reanalyze_ratio}_seed{seed}',
     env=dict(
-        env_name=env_name,
+        env_id=env_id,
         continuous=False,
         manually_discretization=False,
         collector_env_num=collector_env_num,
         evaluator_env_num=evaluator_env_num,
         n_evaluator_episode=evaluator_env_num,
         manager=dict(shared_memory=False, ),
     ),
```

### Comparing `LightZero-0.0.2/zoo/minigrid/config/minigrid_efficientzero_config.py` & `LightZero-0.0.5/zoo/minigrid/config/minigrid_efficientzero_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from easydict import EasyDict
 
 # The typical MiniGrid env id: {'MiniGrid-Empty-8x8-v0', 'MiniGrid-FourRooms-v0', 'MiniGrid-DoorKey-8x8-v0','MiniGrid-DoorKey-16x16-v0'},
 # please refer to https://github.com/Farama-Foundation/MiniGrid for details.
-env_name = 'MiniGrid-Empty-8x8-v0'
+env_id = 'MiniGrid-Empty-8x8-v0'
 max_env_step = int(1e6)
 
 # ==============================================================
 # begin of the most frequently changed config specified by the user
 # ==============================================================
 seed = 0
 collector_env_num = 8
@@ -21,18 +21,18 @@
 threshold_training_steps_for_final_temperature = int(5e5)
 eps_greedy_exploration_in_collect = False
 # ==============================================================
 # end of the most frequently changed config specified by the user
 # ==============================================================
 
 minigrid_efficientzero_config = dict(
-    exp_name=f'data_ez_ctree/{env_name}_efficientzero_ns{num_simulations}_upc{update_per_collect}_rr{reanalyze_ratio}_seed{seed}',
+    exp_name=f'data_ez_ctree/{env_id}_efficientzero_ns{num_simulations}_upc{update_per_collect}_rr{reanalyze_ratio}_seed{seed}',
     env=dict(
         stop_value=int(1e6),
-        env_name=env_name,
+        env_id=env_id,
         continuous=False,
         manually_discretization=False,
         collector_env_num=collector_env_num,
         evaluator_env_num=evaluator_env_num,
         n_evaluator_episode=evaluator_env_num,
         manager=dict(shared_memory=False, ),
     ),
```

### Comparing `LightZero-0.0.2/zoo/minigrid/config/minigrid_muzero_config.py` & `LightZero-0.0.5/zoo/minigrid/config/minigrid_muzero_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from easydict import EasyDict
 
 # The typical MiniGrid env id: {'MiniGrid-Empty-8x8-v0', 'MiniGrid-FourRooms-v0', 'MiniGrid-DoorKey-8x8-v0','MiniGrid-DoorKey-16x16-v0'},
 # please refer to https://github.com/Farama-Foundation/MiniGrid for details.
-env_name = 'MiniGrid-Empty-8x8-v0'
+env_id = 'MiniGrid-Empty-8x8-v0'
 max_env_step = int(1e6)
 
 # ==============================================================
 # begin of the most frequently changed config specified by the user
 # ==============================================================
 seed = 0
 collector_env_num = 8
@@ -21,19 +21,19 @@
 threshold_training_steps_for_final_temperature = int(5e5)
 eps_greedy_exploration_in_collect = False
 # ==============================================================
 # end of the most frequently changed config specified by the user
 # ==============================================================
 
 minigrid_muzero_config = dict(
-    exp_name=f'data_mz_ctree/{env_name}_muzero_ns{num_simulations}_upc{update_per_collect}_rr{reanalyze_ratio}_'
+    exp_name=f'data_mz_ctree/{env_id}_muzero_ns{num_simulations}_upc{update_per_collect}_rr{reanalyze_ratio}_'
              f'collect-eps-{eps_greedy_exploration_in_collect}_temp-final-steps-{threshold_training_steps_for_final_temperature}_pelw{policy_entropy_loss_weight}_seed{seed}',
     env=dict(
         stop_value=int(1e6),
-        env_name=env_name,
+        env_id=env_id,
         continuous=False,
         manually_discretization=False,
         collector_env_num=collector_env_num,
         evaluator_env_num=evaluator_env_num,
         n_evaluator_episode=evaluator_env_num,
         manager=dict(shared_memory=False, ),
     ),
```

### Comparing `LightZero-0.0.2/zoo/minigrid/config/minigrid_muzero_rnd_config.py` & `LightZero-0.0.5/zoo/minigrid/config/minigrid_muzero_rnd_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from easydict import EasyDict
 
 # The typical MiniGrid env id: {'MiniGrid-Empty-8x8-v0', 'MiniGrid-FourRooms-v0', 'MiniGrid-DoorKey-8x8-v0','MiniGrid-DoorKey-16x16-v0'},
 # please refer to https://github.com/Farama-Foundation/MiniGrid for details.
-env_name = 'MiniGrid-Empty-8x8-v0'
+env_id = 'MiniGrid-Empty-8x8-v0'
 max_env_step = int(1e6)
 
 # ==============================================================
 # begin of the most frequently changed config specified by the user
 # ==============================================================
 seed = 0
 collector_env_num = 8
@@ -26,20 +26,20 @@
 target_model_for_intrinsic_reward_update_type = 'assign'  # 'assign' or 'momentum'
 
 # ==============================================================
 # end of the most frequently changed config specified by the user
 # ==============================================================
 
 minigrid_muzero_rnd_config = dict(
-    exp_name=f'data_mz_rnd_ctree/{env_name}_muzero-rnd_ns{num_simulations}_upc{update_per_collect}_rr{reanalyze_ratio}'
+    exp_name=f'data_mz_rnd_ctree/{env_id}_muzero-rnd_ns{num_simulations}_upc{update_per_collect}_rr{reanalyze_ratio}'
              f'_collect-eps-{eps_greedy_exploration_in_collect}_temp-final-steps-{threshold_training_steps_for_final_temperature}_pelw{policy_entropy_loss_weight}'
              f'_rnd-rew-{input_type}-{target_model_for_intrinsic_reward_update_type}_seed{seed}',
     env=dict(
         stop_value=int(1e6),
-        env_name=env_name,
+        env_id=env_id,
         continuous=False,
         manually_discretization=False,
         collector_env_num=collector_env_num,
         evaluator_env_num=evaluator_env_num,
         n_evaluator_episode=evaluator_env_num,
         manager=dict(shared_memory=False, ),
     ),
```

