# Comparing `tmp/corl-3.14.13.tar.gz` & `tmp/corl-3.16.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corl-3.14.13.tar", max compression
+gzip compressed data, was "corl-3.16.2.tar", max compression
```

## Comparing `corl-3.14.13.tar` & `corl-3.16.2.tar`

### file list

```diff
@@ -1,384 +1,392 @@
--rw-r--r--   0        0        0      515 2024-03-22 18:03:48.222324 corl-3.14.13/LICENSE.md
--rw-r--r--   0        0        0     4632 2024-03-22 18:03:48.302324 corl-3.14.13/README.md
--rw-r--r--   0        0        0      493 2024-03-22 18:03:48.872324 corl-3.14.13/corl/__init__.py
--rw-r--r--   0        0        0      493 2024-03-22 18:03:49.292322 corl-3.14.13/corl/agents/__init__.py
--rw-r--r--   0        0        0    39201 2024-03-22 18:03:49.322322 corl-3.14.13/corl/agents/base_agent.py
--rw-r--r--   0        0        0        0 2024-03-22 18:03:49.322322 corl-3.14.13/corl/agents/non_trainable/__init__.py
--rw-r--r--   0        0        0      230 2024-03-22 18:03:49.322322 corl-3.14.13/corl/agents/non_trainable/noop.py
--rw-r--r--   0        0        0      863 2024-03-22 18:03:49.322322 corl-3.14.13/corl/agents/non_trainable/random_action.py
--rw-r--r--   0        0        0    16169 2024-03-22 18:03:49.302322 corl-3.14.13/corl/agents/simple_multi_platform_agent.py
--rw-r--r--   0        0        0      515 2024-03-22 18:03:48.732324 corl-3.14.13/corl/config/policy/ppo/default_config.yml
--rw-r--r--   0        0        0      591 2024-03-22 18:03:48.732324 corl-3.14.13/corl/config/policy/random_action.yml
--rw-r--r--   0        0        0     1287 2024-03-22 18:03:48.732324 corl-3.14.13/corl/config/policy/scripted_action.yml
--rw-r--r--   0        0        0     1033 2024-03-22 18:03:48.582324 corl-3.14.13/corl/config/streamlit_app/default_streamlit_config.yml
--rw-r--r--   0        0        0     1022 2024-03-22 18:03:48.572324 corl-3.14.13/corl/config/streamlit_app/docking1d_streamlit_config.yml
--rw-r--r--   0        0        0     1023 2024-03-22 18:03:48.582324 corl-3.14.13/corl/config/streamlit_app/pong_streamlit_config.yml
--rw-r--r--   0        0        0     2457 2024-03-22 18:03:48.712324 corl-3.14.13/corl/config/tasks/docking_1d/agents/docking1d_agent.yml
--rw-r--r--   0        0        0     1225 2024-03-22 18:03:48.732324 corl-3.14.13/corl/config/tasks/docking_1d/environments/docking1d_env.yml
--rw-r--r--   0        0        0      191 2024-03-22 18:03:48.722324 corl-3.14.13/corl/config/tasks/docking_1d/evaluation/alerts/base_alerts.yml
--rw-r--r--   0        0        0     1179 2024-03-22 18:03:48.722324 corl-3.14.13/corl/config/tasks/docking_1d/evaluation/launch/eval_1d_docking.yml
--rw-r--r--   0        0        0      353 2024-03-22 18:03:48.722324 corl-3.14.13/corl/config/tasks/docking_1d/evaluation/launch/metrics_gen_1d_docking.yml
--rw-r--r--   0        0        0      336 2024-03-22 18:03:48.722324 corl-3.14.13/corl/config/tasks/docking_1d/evaluation/launch/pipeline_1d_docking.yml
--rw-r--r--   0        0        0      549 2024-03-22 18:03:48.722324 corl-3.14.13/corl/config/tasks/docking_1d/evaluation/launch/storage_acedt_1d_docking.yml
--rw-r--r--   0        0        0      236 2024-03-22 18:03:48.732324 corl-3.14.13/corl/config/tasks/docking_1d/evaluation/launch/visualize_1d_docking.yml
--rw-r--r--   0        0        0     2071 2024-03-22 18:03:48.722324 corl-3.14.13/corl/config/tasks/docking_1d/evaluation/metrics/1d_docking.yml
--rw-r--r--   0        0        0      179 2024-03-22 18:03:48.722324 corl-3.14.13/corl/config/tasks/docking_1d/evaluation/test_cases_config/docking1d_tests.yml
--rw-r--r--   0        0        0      424 2024-03-22 18:03:48.712324 corl-3.14.13/corl/config/tasks/docking_1d/experiments/docking_1d.yml
--rw-r--r--   0        0        0      135 2024-03-22 18:03:48.712324 corl-3.14.13/corl/config/tasks/docking_1d/platforms/docking1d_platform.yml
--rw-r--r--   0        0        0      954 2024-03-22 18:03:48.702324 corl-3.14.13/corl/config/tasks/docking_1d/ray_config.yml
--rw-r--r--   0        0        0     1162 2024-03-22 18:03:48.702324 corl-3.14.13/corl/config/tasks/docking_1d/rllib_config.yml
--rw-r--r--   0        0        0     2649 2024-03-22 18:03:48.712324 corl-3.14.13/corl/config/tasks/docking_1d/tasks/docking1d_task.yml
--rw-r--r--   0        0        0     1871 2024-03-22 18:03:48.702324 corl-3.14.13/corl/config/tasks/docking_1d/tune_config.yml
--rw-r--r--   0        0        0       73 2024-03-22 18:03:48.662324 corl-3.14.13/corl/config/tasks/gymnasium/agents/baseline_dones.yml
--rw-r--r--   0        0        0       81 2024-03-22 18:03:48.662324 corl-3.14.13/corl/config/tasks/gymnasium/agents/baseline_epp.yml
--rw-r--r--   0        0        0      126 2024-03-22 18:03:48.662324 corl-3.14.13/corl/config/tasks/gymnasium/agents/baseline_rewards.yml
--rw-r--r--   0        0        0     1403 2024-03-22 18:03:48.672324 corl-3.14.13/corl/config/tasks/gymnasium/agents/gymnasium_agent.yml
--rw-r--r--   0        0        0     3739 2024-03-22 18:03:48.672324 corl-3.14.13/corl/config/tasks/gymnasium/agents/gymnasium_agent_dict_wrapper.yml
--rw-r--r--   0        0        0     1438 2024-03-22 18:03:48.672324 corl-3.14.13/corl/config/tasks/gymnasium/agents/gymnasium_agent_noop.yml
--rw-r--r--   0        0        0     1417 2024-03-22 18:03:48.662324 corl-3.14.13/corl/config/tasks/gymnasium/agents/gymnasium_agent_noop_ctrl.yml
--rw-r--r--   0        0        0     1534 2024-03-22 18:03:48.662324 corl-3.14.13/corl/config/tasks/gymnasium/agents/gymnasium_agent_repeated.yml
--rw-r--r--   0        0        0     4183 2024-03-22 18:03:48.662324 corl-3.14.13/corl/config/tasks/gymnasium/agents/gymnasium_agent_wrapper.yml
--rw-r--r--   0        0        0      872 2024-03-22 18:03:48.702324 corl-3.14.13/corl/config/tasks/gymnasium/environments/cartpole_v1.yml
--rw-r--r--   0        0        0     1022 2024-03-22 18:03:48.702324 corl-3.14.13/corl/config/tasks/gymnasium/environments/cartpole_v1_with_time.yml
--rw-r--r--   0        0        0     1000 2024-03-22 18:03:48.702324 corl-3.14.13/corl/config/tasks/gymnasium/environments/pendulum_v1.yml
--rw-r--r--   0        0        0      347 2024-03-22 18:03:48.682324 corl-3.14.13/corl/config/tasks/gymnasium/experiments/cartpole_v1.yml
--rw-r--r--   0        0        0      357 2024-03-22 18:03:48.672324 corl-3.14.13/corl/config/tasks/gymnasium/experiments/cartpole_v1_benchmark.yml
--rw-r--r--   0        0        0      360 2024-03-22 18:03:48.682324 corl-3.14.13/corl/config/tasks/gymnasium/experiments/cartpole_v1_dict_wrapper.yml
--rw-r--r--   0        0        0      586 2024-03-22 18:03:48.672324 corl-3.14.13/corl/config/tasks/gymnasium/experiments/cartpole_v1_noop.yml
--rw-r--r--   0        0        0      604 2024-03-22 18:03:48.682324 corl-3.14.13/corl/config/tasks/gymnasium/experiments/cartpole_v1_noop_ctrl.yml
--rw-r--r--   0        0        0      587 2024-03-22 18:03:48.682324 corl-3.14.13/corl/config/tasks/gymnasium/experiments/cartpole_v1_random.yml
--rw-r--r--   0        0        0      356 2024-03-22 18:03:48.682324 corl-3.14.13/corl/config/tasks/gymnasium/experiments/cartpole_v1_repeated_obs.yml
--rw-r--r--   0        0        0      605 2024-03-22 18:03:48.672324 corl-3.14.13/corl/config/tasks/gymnasium/experiments/cartpole_v1_scripted.yml
--rw-r--r--   0        0        0      371 2024-03-22 18:03:48.682324 corl-3.14.13/corl/config/tasks/gymnasium/experiments/cartpole_v1_with_wrapper.yml
--rw-r--r--   0        0        0      347 2024-03-22 18:03:48.672324 corl-3.14.13/corl/config/tasks/gymnasium/experiments/pendulum_v1.yml
--rw-r--r--   0        0        0      594 2024-03-22 18:03:48.652324 corl-3.14.13/corl/config/tasks/gymnasium/platforms/gymnasium_platform.yml
--rw-r--r--   0        0        0      608 2024-03-22 18:03:48.652324 corl-3.14.13/corl/config/tasks/gymnasium/platforms/gymnasium_platform_inclusive_parts.yml
--rw-r--r--   0        0        0      957 2024-03-22 18:03:48.652324 corl-3.14.13/corl/config/tasks/gymnasium/ray_config.yml
--rw-r--r--   0        0        0      913 2024-03-22 18:03:48.652324 corl-3.14.13/corl/config/tasks/gymnasium/rllib_config.yml
--rw-r--r--   0        0        0     3175 2024-03-22 18:03:48.692324 corl-3.14.13/corl/config/tasks/gymnasium/tasks/cartpole_v1.yml
--rw-r--r--   0        0        0     3183 2024-03-22 18:03:48.692324 corl-3.14.13/corl/config/tasks/gymnasium/tasks/cartpole_v1_benchmark.yml
--rw-r--r--   0        0        0     3184 2024-03-22 18:03:48.692324 corl-3.14.13/corl/config/tasks/gymnasium/tasks/cartpole_v1_with_time.yml
--rw-r--r--   0        0        0     1804 2024-03-22 18:03:48.692324 corl-3.14.13/corl/config/tasks/gymnasium/tasks/pendulum_v1.yml
--rw-r--r--   0        0        0     1876 2024-03-22 18:03:48.652324 corl-3.14.13/corl/config/tasks/gymnasium/tune_config.yml
--rw-r--r--   0        0        0     5812 2024-03-22 18:03:48.602324 corl-3.14.13/corl/config/tasks/pong/agents/commander_paddle_agent.yml
--rw-r--r--   0        0        0      726 2024-03-22 18:03:48.592324 corl-3.14.13/corl/config/tasks/pong/agents/dummy_noop.yml
--rw-r--r--   0        0        0     1689 2024-03-22 18:03:48.602324 corl-3.14.13/corl/config/tasks/pong/agents/paddle_agent-scripted-noop.yml
--rw-r--r--   0        0        0     1706 2024-03-22 18:03:48.612324 corl-3.14.13/corl/config/tasks/pong/agents/paddle_agent-scripted-random_action.yml
--rw-r--r--   0        0        0     1962 2024-03-22 18:03:48.612324 corl-3.14.13/corl/config/tasks/pong/agents/paddle_agent.yml
--rw-r--r--   0        0        0     2422 2024-03-22 18:03:48.602324 corl-3.14.13/corl/config/tasks/pong/agents/paddle_agent_flat_actions.yml
--rw-r--r--   0        0        0      935 2024-03-22 18:03:48.592324 corl-3.14.13/corl/config/tasks/pong/commander_rllib_config.yml
--rw-r--r--   0        0        0     2293 2024-03-22 18:03:48.642324 corl-3.14.13/corl/config/tasks/pong/environments/commander_pong_env.yml
--rw-r--r--   0        0        0     1561 2024-03-22 18:03:48.642324 corl-3.14.13/corl/config/tasks/pong/environments/pong_env.yml
--rw-r--r--   0        0        0     1810 2024-03-22 18:03:48.642324 corl-3.14.13/corl/config/tasks/pong/evaluation/launch/base_pong_evaluate.yml
--rw-r--r--   0        0        0      333 2024-03-22 18:03:48.642324 corl-3.14.13/corl/config/tasks/pong/evaluation/launch/base_pong_inference.yml
--rw-r--r--   0        0        0     1496 2024-03-22 18:03:48.642324 corl-3.14.13/corl/config/tasks/pong/evaluation/launch/commander_pong_evaluate.yml
--rw-r--r--   0        0        0      108 2024-03-22 18:03:48.642324 corl-3.14.13/corl/config/tasks/pong/evaluation/launch/inference.yml
--rw-r--r--   0        0        0      456 2024-03-22 18:03:48.632324 corl-3.14.13/corl/config/tasks/pong/evaluation/test_cases/commander_pong_test_cases.yml
--rw-r--r--   0        0        0      936 2024-03-22 18:03:48.612324 corl-3.14.13/corl/config/tasks/pong/experiments/pong-both_scripted-random_action.yml
--rw-r--r--   0        0        0      705 2024-03-22 18:03:48.622324 corl-3.14.13/corl/config/tasks/pong/experiments/pong-one_scripted-noop.yml
--rw-r--r--   0        0        0      714 2024-03-22 18:03:48.612324 corl-3.14.13/corl/config/tasks/pong/experiments/pong-one_scripted-random_action.yml
--rw-r--r--   0        0        0      692 2024-03-22 18:03:48.622324 corl-3.14.13/corl/config/tasks/pong/experiments/pong.yml
--rw-r--r--   0        0        0      696 2024-03-22 18:03:48.612324 corl-3.14.13/corl/config/tasks/pong/experiments/pong_alt.yml
--rw-r--r--   0        0        0      527 2024-03-22 18:03:48.622324 corl-3.14.13/corl/config/tasks/pong/experiments/pong_commander.yml
--rw-r--r--   0        0        0      694 2024-03-22 18:03:48.622324 corl-3.14.13/corl/config/tasks/pong/experiments/pong_group.yml
--rw-r--r--   0        0        0      580 2024-03-22 18:03:48.612324 corl-3.14.13/corl/config/tasks/pong/experiments/pong_sac.yml
--rw-r--r--   0        0        0       19 2024-03-22 18:03:48.592324 corl-3.14.13/corl/config/tasks/pong/platforms/paddle.yml
--rw-r--r--   0        0        0      143 2024-03-22 18:03:48.642324 corl-3.14.13/corl/config/tasks/pong/policies/heuristic_paddle_policy.yml
--rw-r--r--   0        0        0       23 2024-03-22 18:03:48.652324 corl-3.14.13/corl/config/tasks/pong/policies/no_policy.yml
--rw-r--r--   0        0        0      665 2024-03-22 18:03:48.652324 corl-3.14.13/corl/config/tasks/pong/policies/ppo_config.yml
--rw-r--r--   0        0        0      585 2024-03-22 18:03:48.652324 corl-3.14.13/corl/config/tasks/pong/policies/sac_config.yml
--rw-r--r--   0        0        0      950 2024-03-22 18:03:48.592324 corl-3.14.13/corl/config/tasks/pong/ray_config.yml
--rw-r--r--   0        0        0     1035 2024-03-22 18:03:48.592324 corl-3.14.13/corl/config/tasks/pong/rllib_config.yml
--rw-r--r--   0        0        0     1947 2024-03-22 18:03:48.632324 corl-3.14.13/corl/config/tasks/pong/tasks/pong_commander_task_ppo.yml
--rw-r--r--   0        0        0     2313 2024-03-22 18:03:48.632324 corl-3.14.13/corl/config/tasks/pong/tasks/pong_task_group.yml
--rw-r--r--   0        0        0     2192 2024-03-22 18:03:48.622324 corl-3.14.13/corl/config/tasks/pong/tasks/pong_task_ppo-all_scripted.yml
--rw-r--r--   0        0        0     2323 2024-03-22 18:03:48.632324 corl-3.14.13/corl/config/tasks/pong/tasks/pong_task_ppo.yml
--rw-r--r--   0        0        0     2415 2024-03-22 18:03:48.632324 corl-3.14.13/corl/config/tasks/pong/tasks/pong_task_ppo_alt.yml
--rw-r--r--   0        0        0     2282 2024-03-22 18:03:48.622324 corl-3.14.13/corl/config/tasks/pong/tasks/pong_task_sac.yml
--rw-r--r--   0        0        0     1870 2024-03-22 18:03:48.592324 corl-3.14.13/corl/config/tasks/pong/tune_config_ppo.yml
--rw-r--r--   0        0        0     1870 2024-03-22 18:03:48.592324 corl-3.14.13/corl/config/tasks/pong/tune_config_sac.yml
--rw-r--r--   0        0        0      958 2024-03-22 18:03:48.582324 corl-3.14.13/corl/config/tasks/ray_config.yml
--rw-r--r--   0        0        0     1115 2024-03-22 18:03:48.582324 corl-3.14.13/corl/config/tasks/rllib_config.yml
--rw-r--r--   0        0        0     1875 2024-03-22 18:03:48.582324 corl-3.14.13/corl/config/tasks/tune_config.yml
--rw-r--r--   0        0        0      493 2024-03-22 18:03:49.442322 corl-3.14.13/corl/dones/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 18:03:49.462322 corl-3.14.13/corl/dones/docking_1d/__init__.py
--rw-r--r--   0        0        0     3196 2024-03-22 18:03:49.462322 corl-3.14.13/corl/dones/docking_1d/dones.py
--rw-r--r--   0        0        0     4633 2024-03-22 18:03:49.452322 corl-3.14.13/corl/dones/done_func_base.py
--rw-r--r--   0        0        0     1808 2024-03-22 18:03:49.452322 corl-3.14.13/corl/dones/done_func_dict_wrapper.py
--rw-r--r--   0        0        0     1762 2024-03-22 18:03:49.452322 corl-3.14.13/corl/dones/done_func_multi_wrapper.py
--rw-r--r--   0        0        0     1724 2024-03-22 18:03:49.452322 corl-3.14.13/corl/dones/done_func_wrapper.py
--rw-r--r--   0        0        0     2174 2024-03-22 18:03:49.452322 corl-3.14.13/corl/dones/episode_length_done.py
--rw-r--r--   0        0        0     1059 2024-03-22 18:03:49.462322 corl-3.14.13/corl/dones/gymnasium_done.py
--rw-r--r--   0        0        0        0 2024-03-22 18:03:49.462322 corl-3.14.13/corl/dones/pong/__init__.py
--rw-r--r--   0        0        0     3068 2024-03-22 18:03:49.462322 corl-3.14.13/corl/dones/pong/commander_pong_dones.py
--rw-r--r--   0        0        0     3042 2024-03-22 18:03:49.462322 corl-3.14.13/corl/dones/pong/dones.py
--rw-r--r--   0        0        0     4025 2024-03-22 18:03:49.442322 corl-3.14.13/corl/dones/sensor_bounds_check_done.py
--rw-r--r--   0        0        0      493 2024-03-22 18:03:49.022323 corl-3.14.13/corl/environment/__init__.py
--rw-r--r--   0        0        0     6657 2024-03-22 18:03:49.022323 corl-3.14.13/corl/environment/base_multi_agent_env.py
--rw-r--r--   0        0        0     1507 2024-03-22 18:03:49.022323 corl-3.14.13/corl/environment/custom_env_metrics.py
--rw-r--r--   0        0        0    13050 2024-03-22 18:03:49.062323 corl-3.14.13/corl/environment/default_env_rllib_callbacks.py
--rw-r--r--   0        0        0     8746 2024-03-22 18:03:49.062323 corl-3.14.13/corl/environment/environment_wrappers.py
--rw-r--r--   0        0        0     1268 2024-03-22 18:03:49.062323 corl-3.14.13/corl/environment/episode_artifact_callbacks.py
--rw-r--r--   0        0        0      493 2024-03-22 18:03:49.052323 corl-3.14.13/corl/environment/gym_env.py
--rw-r--r--   0        0        0    67836 2024-03-22 18:03:49.052323 corl-3.14.13/corl/environment/multi_agent_env.py
--rw-r--r--   0        0        0     3407 2024-03-22 18:03:49.022323 corl-3.14.13/corl/environment/pickle_env_state.py
--rw-r--r--   0        0        0      493 2024-03-22 18:03:49.062323 corl-3.14.13/corl/environment/utils/__init__.py
--rw-r--r--   0        0        0     3250 2024-03-22 18:03:49.072323 corl-3.14.13/corl/environment/utils/env_creation.py
--rw-r--r--   0        0        0     2480 2024-03-22 18:03:49.072323 corl-3.14.13/corl/environment/utils/obs_buffer.py
--rw-r--r--   0        0        0     1840 2024-03-22 18:03:49.072323 corl-3.14.13/corl/environment/utils/space_sort.py
--rw-r--r--   0        0        0      841 2024-03-22 18:03:49.592321 corl-3.14.13/corl/episode_parameter_providers/__init__.py
--rw-r--r--   0        0        0     3945 2024-03-22 18:03:49.622321 corl-3.14.13/corl/episode_parameter_providers/base_network_epp.py
--rw-r--r--   0        0        0     5011 2024-03-22 18:03:49.612321 corl-3.14.13/corl/episode_parameter_providers/core.py
--rw-r--r--   0        0        0     2870 2024-03-22 18:03:49.622321 corl-3.14.13/corl/episode_parameter_providers/incremental.py
--rw-r--r--   0        0        0     5438 2024-03-22 18:03:49.602321 corl-3.14.13/corl/episode_parameter_providers/remote.py
--rw-r--r--   0        0        0      944 2024-03-22 18:03:49.622321 corl-3.14.13/corl/episode_parameter_providers/simple.py
--rw-r--r--   0        0        0     4046 2024-03-22 18:03:49.622321 corl-3.14.13/corl/episode_parameter_providers/tabular_parameter_provider.py
--rw-r--r--   0        0        0      511 2024-03-22 18:03:49.662321 corl-3.14.13/corl/evaluation/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 18:03:49.882321 corl-3.14.13/corl/evaluation/connection/__init__.py
--rw-r--r--   0        0        0     1189 2024-03-22 18:03:49.892321 corl-3.14.13/corl/evaluation/connection/base_epp_update.py
--rw-r--r--   0        0        0     1755 2024-03-22 18:03:49.882321 corl-3.14.13/corl/evaluation/connection/base_eval_connection.py
--rw-r--r--   0        0        0     2248 2024-03-22 18:03:49.892321 corl-3.14.13/corl/evaluation/connection/base_rest_connection.py
--rw-r--r--   0        0        0     5298 2024-03-22 18:03:49.882321 corl-3.14.13/corl/evaluation/connection/signal.py
--rw-r--r--   0        0        0      858 2024-03-22 18:03:49.662321 corl-3.14.13/corl/evaluation/default_config_updates.py
--rw-r--r--   0        0        0     3885 2024-03-22 18:03:49.672321 corl-3.14.13/corl/evaluation/episode_artifact.py
--rw-r--r--   0        0        0      560 2024-03-22 18:03:49.662321 corl-3.14.13/corl/evaluation/eval_logger_name.py
--rw-r--r--   0        0        0     1954 2024-03-22 18:03:49.672321 corl-3.14.13/corl/evaluation/evaluation_artifacts.py
--rw-r--r--   0        0        0     1188 2024-03-22 18:03:49.672321 corl-3.14.13/corl/evaluation/evaluation_factory.py
--rw-r--r--   0        0        0     1309 2024-03-22 18:03:49.662321 corl-3.14.13/corl/evaluation/evaluation_outcome.py
--rw-r--r--   0        0        0      537 2024-03-22 18:03:49.892321 corl-3.14.13/corl/evaluation/launchers/__init__.py
--rw-r--r--   0        0        0     3706 2024-03-22 18:03:49.892321 corl-3.14.13/corl/evaluation/launchers/base_eval.py
--rw-r--r--   0        0        0     5762 2024-03-22 18:03:49.922321 corl-3.14.13/corl/evaluation/launchers/evaluate_runner.py
--rw-r--r--   0        0        0     5447 2024-03-22 18:03:49.892321 corl-3.14.13/corl/evaluation/launchers/evaluate_validator.py
--rw-r--r--   0        0        0     6950 2024-03-22 18:03:49.912321 corl-3.14.13/corl/evaluation/launchers/launch_evaluate.py
--rw-r--r--   0        0        0     5581 2024-03-22 18:03:49.912321 corl-3.14.13/corl/evaluation/launchers/launch_generate_metrics.py
--rw-r--r--   0        0        0    10206 2024-03-22 18:03:49.922321 corl-3.14.13/corl/evaluation/launchers/launch_pipeline.py
--rw-r--r--   0        0        0     2191 2024-03-22 18:03:49.902321 corl-3.14.13/corl/evaluation/launchers/launch_storage.py
--rw-r--r--   0        0        0     2502 2024-03-22 18:03:49.902321 corl-3.14.13/corl/evaluation/launchers/launch_visualize.py
--rw-r--r--   0        0        0     2772 2024-03-22 18:03:49.902321 corl-3.14.13/corl/evaluation/launchers/rest_eval_connection.py
--rw-r--r--   0        0        0      549 2024-03-22 18:03:49.862321 corl-3.14.13/corl/evaluation/loader/__init__.py
--rw-r--r--   0        0        0     1047 2024-03-22 18:03:49.872321 corl-3.14.13/corl/evaluation/loader/heuristic.py
--rw-r--r--   0        0        0     5546 2024-03-22 18:03:49.862321 corl-3.14.13/corl/evaluation/loader/i_agent_loader.py
--rw-r--r--   0        0        0     4646 2024-03-22 18:03:49.872321 corl-3.14.13/corl/evaluation/loader/policy_checkpoint.py
--rw-r--r--   0        0        0      493 2024-03-22 18:03:49.682321 corl-3.14.13/corl/evaluation/metrics/__init__.py
--rw-r--r--   0        0        0      493 2024-03-22 18:03:49.722321 corl-3.14.13/corl/evaluation/metrics/aggregators/__init__.py
--rw-r--r--   0        0        0     1933 2024-03-22 18:03:49.732321 corl-3.14.13/corl/evaluation/metrics/aggregators/accumulate.py
--rw-r--r--   0        0        0     2136 2024-03-22 18:03:49.722321 corl-3.14.13/corl/evaluation/metrics/aggregators/average.py
--rw-r--r--   0        0        0     2437 2024-03-22 18:03:49.722321 corl-3.14.13/corl/evaluation/metrics/aggregators/counter.py
--rw-r--r--   0        0        0     1590 2024-03-22 18:03:49.722321 corl-3.14.13/corl/evaluation/metrics/aggregators/criteria_rate.py
--rw-r--r--   0        0        0     2002 2024-03-22 18:03:49.732321 corl-3.14.13/corl/evaluation/metrics/aggregators/sum.py
--rw-r--r--   0        0        0     2867 2024-03-22 18:03:49.682321 corl-3.14.13/corl/evaluation/metrics/alerts.py
--rw-r--r--   0        0        0     2643 2024-03-22 18:03:49.682321 corl-3.14.13/corl/evaluation/metrics/generator.py
--rw-r--r--   0        0        0      493 2024-03-22 18:03:49.732321 corl-3.14.13/corl/evaluation/metrics/generators/__init__.py
--rw-r--r--   0        0        0     2293 2024-03-22 18:03:49.742321 corl-3.14.13/corl/evaluation/metrics/generators/dones.py
--rw-r--r--   0        0        0      493 2024-03-22 18:03:49.742321 corl-3.14.13/corl/evaluation/metrics/generators/meta/__init__.py
--rw-r--r--   0        0        0     1039 2024-03-22 18:03:49.742321 corl-3.14.13/corl/evaluation/metrics/generators/meta/episode_length.py
--rw-r--r--   0        0        0     1029 2024-03-22 18:03:49.742321 corl-3.14.13/corl/evaluation/metrics/generators/meta/runtime.py
--rw-r--r--   0        0        0     3005 2024-03-22 18:03:49.732321 corl-3.14.13/corl/evaluation/metrics/generators/rewards.py
--rw-r--r--   0        0        0     1258 2024-03-22 18:03:49.682321 corl-3.14.13/corl/evaluation/metrics/metric.py
--rw-r--r--   0        0        0    11776 2024-03-22 18:03:49.692321 corl-3.14.13/corl/evaluation/metrics/processors.py
--rw-r--r--   0        0        0     1895 2024-03-22 18:03:49.682321 corl-3.14.13/corl/evaluation/metrics/scenario_alert_generators.py
--rw-r--r--   0        0        0     2917 2024-03-22 18:03:49.702321 corl-3.14.13/corl/evaluation/metrics/scenario_metric_generators.py
--rw-r--r--   0        0        0     1139 2024-03-22 18:03:49.692321 corl-3.14.13/corl/evaluation/metrics/scopes.py
--rw-r--r--   0        0        0      493 2024-03-22 18:03:49.702321 corl-3.14.13/corl/evaluation/metrics/types/__init__.py
--rw-r--r--   0        0        0      493 2024-03-22 18:03:49.702321 corl-3.14.13/corl/evaluation/metrics/types/nonterminals/__init__.py
--rw-r--r--   0        0        0     1473 2024-03-22 18:03:49.702321 corl-3.14.13/corl/evaluation/metrics/types/nonterminals/dict.py
--rw-r--r--   0        0        0     1323 2024-03-22 18:03:49.712321 corl-3.14.13/corl/evaluation/metrics/types/nonterminals/timed_value.py
--rw-r--r--   0        0        0     1505 2024-03-22 18:03:49.702321 corl-3.14.13/corl/evaluation/metrics/types/nonterminals/vector.py
--rw-r--r--   0        0        0      493 2024-03-22 18:03:49.712321 corl-3.14.13/corl/evaluation/metrics/types/terminals/__init__.py
--rw-r--r--   0        0        0     1085 2024-03-22 18:03:49.712321 corl-3.14.13/corl/evaluation/metrics/types/terminals/discrete.py
--rw-r--r--   0        0        0     2341 2024-03-22 18:03:49.722321 corl-3.14.13/corl/evaluation/metrics/types/terminals/rate.py
--rw-r--r--   0        0        0     1961 2024-03-22 18:03:49.712321 corl-3.14.13/corl/evaluation/metrics/types/terminals/real.py
--rw-r--r--   0        0        0     1010 2024-03-22 18:03:49.712321 corl-3.14.13/corl/evaluation/metrics/types/terminals/string.py
--rw-r--r--   0        0        0      873 2024-03-22 18:03:49.712321 corl-3.14.13/corl/evaluation/metrics/types/terminals/void.py
--rw-r--r--   0        0        0      510 2024-03-22 18:03:49.872321 corl-3.14.13/corl/evaluation/recording/__init__.py
--rw-r--r--   0        0        0     7597 2024-03-22 18:03:49.882321 corl-3.14.13/corl/evaluation/recording/folder.py
--rw-r--r--   0        0        0     1620 2024-03-22 18:03:49.872321 corl-3.14.13/corl/evaluation/recording/i_recorder.py
--rw-r--r--   0        0        0      537 2024-03-22 18:03:49.742321 corl-3.14.13/corl/evaluation/runners/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 18:03:49.752321 corl-3.14.13/corl/evaluation/runners/inference/__init__.py
--rw-r--r--   0        0        0     7553 2024-03-22 18:03:49.752321 corl-3.14.13/corl/evaluation/runners/inference/algorithm_runner.py
--rw-r--r--   0        0        0     1719 2024-03-22 18:03:49.762321 corl-3.14.13/corl/evaluation/runners/inference/inference.py
--rw-r--r--   0        0        0     1548 2024-03-22 18:03:49.762321 corl-3.14.13/corl/evaluation/runners/inference/inference_callback.py
--rw-r--r--   0        0        0        0 2024-03-22 18:03:49.762321 corl-3.14.13/corl/evaluation/runners/inference/protocol/__init__.py
--rw-r--r--   0        0        0     1038 2024-03-22 18:03:49.772321 corl-3.14.13/corl/evaluation/runners/inference/protocol/simple_epp_update.py
--rw-r--r--   0        0        0     2759 2024-03-22 18:03:49.762321 corl-3.14.13/corl/evaluation/runners/inference/protocol/simple_network_epp.py
--rw-r--r--   0        0        0     1780 2024-03-22 18:03:49.762321 corl-3.14.13/corl/evaluation/runners/inference/protocol/simple_network_epp_strategy.py
--rw-r--r--   0        0        0    13553 2024-03-22 18:03:49.752321 corl-3.14.13/corl/evaluation/runners/iterate_test_cases.py
--rw-r--r--   0        0        0      582 2024-03-22 18:03:49.772321 corl-3.14.13/corl/evaluation/runners/section_factories/__init__.py
--rw-r--r--   0        0        0      550 2024-03-22 18:03:49.772321 corl-3.14.13/corl/evaluation/runners/section_factories/engine/__init__.py
--rw-r--r--   0        0        0      513 2024-03-22 18:03:49.782321 corl-3.14.13/corl/evaluation/runners/section_factories/engine/rllib/__init__.py
--rw-r--r--   0        0        0    16896 2024-03-22 18:03:49.792321 corl-3.14.13/corl/evaluation/runners/section_factories/engine/rllib/default_evaluation_callbacks.py
--rw-r--r--   0        0        0    10311 2024-03-22 18:03:49.782321 corl-3.14.13/corl/evaluation/runners/section_factories/engine/rllib/episode_artifact_logging_callback.py
--rw-r--r--   0        0        0     3325 2024-03-22 18:03:49.792321 corl-3.14.13/corl/evaluation/runners/section_factories/engine/rllib/eval_config_updates.py
--rw-r--r--   0        0        0     1938 2024-03-22 18:03:49.802321 corl-3.14.13/corl/evaluation/runners/section_factories/engine/rllib/interruptable_callback.py
--rw-r--r--   0        0        0    10279 2024-03-22 18:03:49.802321 corl-3.14.13/corl/evaluation/runners/section_factories/engine/rllib/rllib_trainer.py
--rw-r--r--   0        0        0      493 2024-03-22 18:03:49.802321 corl-3.14.13/corl/evaluation/runners/section_factories/plugins/__init__.py
--rw-r--r--   0        0        0      886 2024-03-22 18:03:49.812321 corl-3.14.13/corl/evaluation/runners/section_factories/plugins/config_updater.py
--rw-r--r--   0        0        0      868 2024-03-22 18:03:49.812321 corl-3.14.13/corl/evaluation/runners/section_factories/plugins/environment_state_extractor.py
--rw-r--r--   0        0        0     1023 2024-03-22 18:03:49.812321 corl-3.14.13/corl/evaluation/runners/section_factories/plugins/platform_serializer.py
--rw-r--r--   0        0        0     1498 2024-03-22 18:03:49.812321 corl-3.14.13/corl/evaluation/runners/section_factories/plugins/plugins.py
--rw-r--r--   0        0        0     4668 2024-03-22 18:03:49.772321 corl-3.14.13/corl/evaluation/runners/section_factories/task.py
--rw-r--r--   0        0        0     1730 2024-03-22 18:03:49.772321 corl-3.14.13/corl/evaluation/runners/section_factories/teams.py
--rw-r--r--   0        0        0      516 2024-03-22 18:03:49.812321 corl-3.14.13/corl/evaluation/runners/section_factories/test_cases/__init__.py
--rw-r--r--   0        0        0     4104 2024-03-22 18:03:49.832321 corl-3.14.13/corl/evaluation/runners/section_factories/test_cases/base_network_strategy.py
--rw-r--r--   0        0        0     7950 2024-03-22 18:03:49.832321 corl-3.14.13/corl/evaluation/runners/section_factories/test_cases/config_parser.py
--rw-r--r--   0        0        0     3985 2024-03-22 18:03:49.822321 corl-3.14.13/corl/evaluation/runners/section_factories/test_cases/default_strategy.py
--rw-r--r--   0        0        0     5720 2024-03-22 18:03:49.822321 corl-3.14.13/corl/evaluation/runners/section_factories/test_cases/pandas.py
--rw-r--r--   0        0        0     5307 2024-03-22 18:03:49.842321 corl-3.14.13/corl/evaluation/runners/section_factories/test_cases/tabular_strategy.py
--rw-r--r--   0        0        0     7005 2024-03-22 18:03:49.822321 corl-3.14.13/corl/evaluation/runners/section_factories/test_cases/test_case_generator.py
--rw-r--r--   0        0        0     4082 2024-03-22 18:03:49.832321 corl-3.14.13/corl/evaluation/runners/section_factories/test_cases/test_case_manager.py
--rw-r--r--   0        0        0     4244 2024-03-22 18:03:49.672321 corl-3.14.13/corl/evaluation/scene_processors.py
--rw-r--r--   0        0        0     6079 2024-03-22 18:03:49.662321 corl-3.14.13/corl/evaluation/serialize_platforms.py
--rw-r--r--   0        0        0      537 2024-03-22 18:03:49.852321 corl-3.14.13/corl/evaluation/util/__init__.py
--rw-r--r--   0        0        0     2265 2024-03-22 18:03:49.862321 corl-3.14.13/corl/evaluation/util/condition.py
--rw-r--r--   0        0        0     1120 2024-03-22 18:03:49.862321 corl-3.14.13/corl/evaluation/util/storage.py
--rw-r--r--   0        0        0      542 2024-03-22 18:03:49.852321 corl-3.14.13/corl/evaluation/visualization/__init__.py
--rw-r--r--   0        0        0     7186 2024-03-22 18:03:49.852321 corl-3.14.13/corl/evaluation/visualization/html_plots.py
--rw-r--r--   0        0        0    10715 2024-03-22 18:03:49.842321 corl-3.14.13/corl/evaluation/visualization/print.py
--rw-r--r--   0        0        0     2028 2024-03-22 18:03:49.852321 corl-3.14.13/corl/evaluation/visualization/visualization.py
--rw-r--r--   0        0        0      493 2024-03-22 18:03:49.552322 corl-3.14.13/corl/experiments/__init__.py
--rw-r--r--   0        0        0     7204 2024-03-22 18:03:49.552322 corl-3.14.13/corl/experiments/base_experiment.py
--rw-r--r--   0        0        0    13149 2024-03-22 18:03:49.562322 corl-3.14.13/corl/experiments/benchmark_experiment.py
--rwxr-xr-x   0        0        0    14583 2024-03-22 18:03:49.582322 corl-3.14.13/corl/experiments/export_setup_experiment.py
--rw-r--r--   0        0        0    25590 2024-03-22 18:03:49.572322 corl-3.14.13/corl/experiments/rllib_experiment.py
--rw-r--r--   0        0        0        0 2024-03-22 18:03:49.582322 corl-3.14.13/corl/experiments/rllib_utils/__init__.py
--rw-r--r--   0        0        0     1917 2024-03-22 18:03:49.582322 corl-3.14.13/corl/experiments/rllib_utils/policy_mapping_functions.py
--rw-r--r--   0        0        0      852 2024-03-22 18:03:49.582322 corl-3.14.13/corl/experiments/rllib_utils/wrappers.py
--rw-r--r--   0        0        0      493 2024-03-22 18:03:49.472322 corl-3.14.13/corl/glues/__init__.py
--rw-r--r--   0        0        0     1560 2024-03-22 18:03:49.482322 corl-3.14.13/corl/glues/base_dict_wrapper.py
--rw-r--r--   0        0        0    15620 2024-03-22 18:03:49.472322 corl-3.14.13/corl/glues/base_glue.py
--rw-r--r--   0        0        0     1519 2024-03-22 18:03:49.482322 corl-3.14.13/corl/glues/base_multi_wrapper.py
--rw-r--r--   0        0        0     1460 2024-03-22 18:03:49.472322 corl-3.14.13/corl/glues/base_wrapper.py
--rw-r--r--   0        0        0      493 2024-03-22 18:03:49.482322 corl-3.14.13/corl/glues/common/__init__.py
--rw-r--r--   0        0        0     4926 2024-03-22 18:03:49.492322 corl-3.14.13/corl/glues/common/controller_glue.py
--rw-r--r--   0        0        0     3410 2024-03-22 18:03:49.512322 corl-3.14.13/corl/glues/common/magnitude.py
--rw-r--r--   0        0        0     2278 2024-03-22 18:03:49.482322 corl-3.14.13/corl/glues/common/observe_part_validity.py
--rw-r--r--   0        0        0     3999 2024-03-22 18:03:49.502322 corl-3.14.13/corl/glues/common/observe_sensor.py
--rw-r--r--   0        0        0     5338 2024-03-22 18:03:49.502322 corl-3.14.13/corl/glues/common/observe_sensor_repeated.py
--rw-r--r--   0        0        0     2825 2024-03-22 18:03:49.492322 corl-3.14.13/corl/glues/common/projected_quantity.py
--rw-r--r--   0        0        0     6176 2024-03-22 18:03:49.502322 corl-3.14.13/corl/glues/common/target_value.py
--rw-r--r--   0        0        0     7410 2024-03-22 18:03:49.482322 corl-3.14.13/corl/glues/common/target_value_difference.py
--rw-r--r--   0        0        0     3204 2024-03-22 18:03:49.492322 corl-3.14.13/corl/glues/common/trig_values.py
--rw-r--r--   0        0        0     2860 2024-03-22 18:03:49.492322 corl-3.14.13/corl/glues/common/unit_vector_glue.py
--rw-r--r--   0        0        0        0 2024-03-22 18:03:49.512322 corl-3.14.13/corl/glues/controller_wrappers/__init__.py
--rw-r--r--   0        0        0     6121 2024-03-22 18:03:49.542322 corl-3.14.13/corl/glues/controller_wrappers/delta_controller.py
--rw-r--r--   0        0        0     8848 2024-03-22 18:03:49.542322 corl-3.14.13/corl/glues/controller_wrappers/obs_relative_delta_controller.py
--rw-r--r--   0        0        0     5442 2024-03-22 18:03:49.542322 corl-3.14.13/corl/glues/controller_wrappers/obs_relative_delta_controller_dict.py
--rw-r--r--   0        0        0      493 2024-03-22 18:03:48.882324 corl-3.14.13/corl/libraries/__init__.py
--rw-r--r--   0        0        0     1814 2024-03-22 18:03:48.902324 corl-3.14.13/corl/libraries/algorithm_helper.py
--rw-r--r--   0        0        0     1142 2024-03-22 18:03:48.932324 corl-3.14.13/corl/libraries/cleanup.py
--rw-r--r--   0        0        0     1067 2024-03-22 18:03:48.992323 corl-3.14.13/corl/libraries/collection_utils.py
--rw-r--r--   0        0        0     5561 2024-03-22 18:03:48.972323 corl-3.14.13/corl/libraries/config_file_watcher.py
--rw-r--r--   0        0        0     1447 2024-03-22 18:03:48.872324 corl-3.14.13/corl/libraries/context.py
--rw-r--r--   0        0        0     1376 2024-03-22 18:03:49.002323 corl-3.14.13/corl/libraries/env_common.py
--rw-r--r--   0        0        0     1601 2024-03-22 18:03:49.002323 corl-3.14.13/corl/libraries/env_func_base.py
--rw-r--r--   0        0        0    42206 2024-03-22 18:03:48.952323 corl-3.14.13/corl/libraries/env_space_util.py
--rw-r--r--   0        0        0    12949 2024-03-22 18:03:48.912324 corl-3.14.13/corl/libraries/environment_dict.py
--rw-r--r--   0        0        0     2102 2024-03-22 18:03:48.992323 corl-3.14.13/corl/libraries/factory.py
--rw-r--r--   0        0        0      856 2024-03-22 18:03:48.902324 corl-3.14.13/corl/libraries/file_path.py
--rw-r--r--   0        0        0    14324 2024-03-22 18:03:48.902324 corl-3.14.13/corl/libraries/functor.py
--rw-r--r--   0        0        0    28644 2024-03-22 18:03:48.982323 corl-3.14.13/corl/libraries/hparam_search_util.py
--rw-r--r--   0        0        0     2655 2024-03-22 18:03:48.982323 corl-3.14.13/corl/libraries/nan_check.py
--rw-r--r--   0        0        0    11752 2024-03-22 18:03:48.882324 corl-3.14.13/corl/libraries/normalization.py
--rw-r--r--   0        0        0     2793 2024-03-22 18:03:48.952323 corl-3.14.13/corl/libraries/observation_extractor.py
--rw-r--r--   0        0        0     2590 2024-03-22 18:03:48.992323 corl-3.14.13/corl/libraries/observation_util.py
--rw-r--r--   0        0        0    22861 2024-03-22 18:03:48.932324 corl-3.14.13/corl/libraries/parameters.py
--rw-r--r--   0        0        0     9275 2024-03-22 18:03:48.882324 corl-3.14.13/corl/libraries/plugin_library.py
--rw-r--r--   0        0        0    19233 2024-03-22 18:03:48.922324 corl-3.14.13/corl/libraries/property.py
--rw-r--r--   0        0        0     4345 2024-03-22 18:03:48.872324 corl-3.14.13/corl/libraries/space_transformations.py
--rw-r--r--   0        0        0     5143 2024-03-22 18:03:48.962323 corl-3.14.13/corl/libraries/state_dict.py
--rw-r--r--   0        0        0    19395 2024-03-22 18:03:48.962323 corl-3.14.13/corl/libraries/units.py
--rw-r--r--   0        0        0     3378 2024-03-22 18:03:48.982323 corl-3.14.13/corl/libraries/utils.py
--rw-r--r--   0        0        0     4248 2024-03-22 18:03:48.992323 corl-3.14.13/corl/libraries/value_function.py
--rw-r--r--   0        0        0      493 2024-03-22 18:03:49.002323 corl-3.14.13/corl/models/__init__.py
--rw-r--r--   0        0        0    22495 2024-03-22 18:03:49.012323 corl-3.14.13/corl/models/frame_stacking.py
--rw-r--r--   0        0        0     7097 2024-03-22 18:03:49.012323 corl-3.14.13/corl/models/torch_frame_stack.py
--rw-r--r--   0        0        0      493 2024-03-22 18:03:49.922321 corl-3.14.13/corl/parsers/__init__.py
--rw-r--r--   0        0        0     1656 2024-03-22 18:03:49.932321 corl-3.14.13/corl/parsers/agent_and_platform.py
--rw-r--r--   0        0        0    18077 2024-03-22 18:03:49.932321 corl-3.14.13/corl/parsers/yaml_loader.py
--rw-r--r--   0        0        0      493 2024-03-22 18:03:49.592321 corl-3.14.13/corl/parts/__init__.py
--rw-r--r--   0        0        0     4097 2024-03-22 18:03:49.592321 corl-3.14.13/corl/parts/comms.py
--rw-r--r--   0        0        0     1903 2024-03-22 18:03:49.592321 corl-3.14.13/corl/parts/memory_store.py
--rw-r--r--   0        0        0      493 2024-03-22 18:03:49.942320 corl-3.14.13/corl/policies/__init__.py
--rw-r--r--   0        0        0      661 2024-03-22 18:03:49.952320 corl-3.14.13/corl/policies/base_policy.py
--rw-r--r--   0        0        0    11505 2024-03-22 18:03:49.942320 corl-3.14.13/corl/policies/custom_policy.py
--rw-r--r--   0        0        0     2013 2024-03-22 18:03:49.942320 corl-3.14.13/corl/policies/random_action.py
--rw-r--r--   0        0        0     6985 2024-03-22 18:03:49.942320 corl-3.14.13/corl/policies/scripted_action.py
--rw-r--r--   0        0        0      493 2024-03-22 18:03:49.622321 corl-3.14.13/corl/rewards/__init__.py
--rw-r--r--   0        0        0     3868 2024-03-22 18:03:49.632321 corl-3.14.13/corl/rewards/base_measurement_operation.py
--rw-r--r--   0        0        0        0 2024-03-22 18:03:49.652321 corl-3.14.13/corl/rewards/docking_1d/__init__.py
--rw-r--r--   0        0        0     3121 2024-03-22 18:03:49.652321 corl-3.14.13/corl/rewards/docking_1d/docking_distance_change_reward.py
--rw-r--r--   0        0        0     4330 2024-03-22 18:03:49.652321 corl-3.14.13/corl/rewards/docking_1d/docking_reward.py
--rw-r--r--   0        0        0     7593 2024-03-22 18:03:49.642321 corl-3.14.13/corl/rewards/episode_done.py
--rw-r--r--   0        0        0     3870 2024-03-22 18:03:49.652321 corl-3.14.13/corl/rewards/exponential_decay_from_target_value.py
--rw-r--r--   0        0        0     1012 2024-03-22 18:03:49.642321 corl-3.14.13/corl/rewards/gymnasium_reward.py
--rw-r--r--   0        0        0     1684 2024-03-22 18:03:49.642321 corl-3.14.13/corl/rewards/multi_measurement_operation.py
--rw-r--r--   0        0        0     2410 2024-03-22 18:03:49.632321 corl-3.14.13/corl/rewards/reward_func_base.py
--rw-r--r--   0        0        0     1834 2024-03-22 18:03:49.632321 corl-3.14.13/corl/rewards/reward_func_dict_wrapper.py
--rw-r--r--   0        0        0     1829 2024-03-22 18:03:49.652321 corl-3.14.13/corl/rewards/reward_func_multi_wrapper.py
--rw-r--r--   0        0        0     1788 2024-03-22 18:03:49.632321 corl-3.14.13/corl/rewards/reward_func_wrapper.py
--rw-r--r--   0        0        0      493 2024-03-22 18:03:49.202323 corl-3.14.13/corl/simulators/__init__.py
--rw-r--r--   0        0        0    12962 2024-03-22 18:03:49.222323 corl-3.14.13/corl/simulators/base_parts.py
--rw-r--r--   0        0        0     5329 2024-03-22 18:03:49.212323 corl-3.14.13/corl/simulators/base_platform.py
--rw-r--r--   0        0        0     1113 2024-03-22 18:03:49.202323 corl-3.14.13/corl/simulators/base_platform_type.py
--rw-r--r--   0        0        0     1240 2024-03-22 18:03:49.202323 corl-3.14.13/corl/simulators/base_properties.py
--rw-r--r--   0        0        0    11254 2024-03-22 18:03:49.212323 corl-3.14.13/corl/simulators/base_simulator.py
--rw-r--r--   0        0        0     1046 2024-03-22 18:03:49.222323 corl-3.14.13/corl/simulators/base_simulator_state.py
--rw-r--r--   0        0        0     4107 2024-03-22 18:03:49.202323 corl-3.14.13/corl/simulators/common_platform_utils.py
--rw-r--r--   0        0        0        0 2024-03-22 18:03:49.272323 corl-3.14.13/corl/simulators/docking_1d/__init__.py
--rw-r--r--   0        0        0      868 2024-03-22 18:03:49.282323 corl-3.14.13/corl/simulators/docking_1d/available_platforms.py
--rw-r--r--   0        0        0     2289 2024-03-22 18:03:49.292322 corl-3.14.13/corl/simulators/docking_1d/controllers.py
--rw-r--r--   0        0        0     9013 2024-03-22 18:03:49.292322 corl-3.14.13/corl/simulators/docking_1d/entities.py
--rw-r--r--   0        0        0     3274 2024-03-22 18:03:49.282323 corl-3.14.13/corl/simulators/docking_1d/platform.py
--rw-r--r--   0        0        0     2173 2024-03-22 18:03:49.282323 corl-3.14.13/corl/simulators/docking_1d/properties.py
--rw-r--r--   0        0        0     2042 2024-03-22 18:03:49.272323 corl-3.14.13/corl/simulators/docking_1d/sensors.py
--rw-r--r--   0        0        0     4288 2024-03-22 18:03:49.282323 corl-3.14.13/corl/simulators/docking_1d/simulator.py
--rw-r--r--   0        0        0      493 2024-03-22 18:03:49.262323 corl-3.14.13/corl/simulators/gymnasium/__init__.py
--rw-r--r--   0        0        0     1298 2024-03-22 18:03:49.272323 corl-3.14.13/corl/simulators/gymnasium/gymnasium_available_platforms.py
--rw-r--r--   0        0        0     3265 2024-03-22 18:03:49.272323 corl-3.14.13/corl/simulators/gymnasium/gymnasium_controllers.py
--rw-r--r--   0        0        0     4102 2024-03-22 18:03:49.272323 corl-3.14.13/corl/simulators/gymnasium/gymnasium_sensors.py
--rw-r--r--   0        0        0    10957 2024-03-22 18:03:49.272323 corl-3.14.13/corl/simulators/gymnasium/gymnasium_simulator.py
--rw-r--r--   0        0        0      493 2024-03-22 18:03:49.232323 corl-3.14.13/corl/simulators/pong/__init__.py
--rw-r--r--   0        0        0     1078 2024-03-22 18:03:49.252323 corl-3.14.13/corl/simulators/pong/available_platforms.py
--rw-r--r--   0        0        0     3443 2024-03-22 18:03:49.252323 corl-3.14.13/corl/simulators/pong/controllers.py
--rw-r--r--   0        0        0     4480 2024-03-22 18:03:49.242323 corl-3.14.13/corl/simulators/pong/heuristic_paddle_policy.py
--rw-r--r--   0        0        0     3041 2024-03-22 18:03:49.222323 corl-3.14.13/corl/simulators/pong/paddle_platform.py
--rw-r--r--   0        0        0     6416 2024-03-22 18:03:49.242323 corl-3.14.13/corl/simulators/pong/play_pickled_episode.py
--rw-r--r--   0        0        0    11241 2024-03-22 18:03:49.232323 corl-3.14.13/corl/simulators/pong/pong.py
--rw-r--r--   0        0        0     8056 2024-03-22 18:03:49.232323 corl-3.14.13/corl/simulators/pong/sensors.py
--rw-r--r--   0        0        0     7608 2024-03-22 18:03:49.242323 corl-3.14.13/corl/simulators/pong/simulator.py
--rw-r--r--   0        0        0      493 2024-03-22 18:03:49.252323 corl-3.14.13/corl/simulators/six_dof/__init__.py
--rw-r--r--   0        0        0     1780 2024-03-22 18:03:49.252323 corl-3.14.13/corl/simulators/six_dof/base_six_dof_controllers.py
--rw-r--r--   0        0        0     3165 2024-03-22 18:03:49.262323 corl-3.14.13/corl/simulators/six_dof/base_six_dof_platform.py
--rw-r--r--   0        0        0    14749 2024-03-22 18:03:49.262323 corl-3.14.13/corl/simulators/six_dof/base_six_dof_properties.py
--rw-r--r--   0        0        0      493 2024-03-22 18:03:49.322322 corl-3.14.13/corl/test_utils/__init__.py
--rw-r--r--   0        0        0     1432 2024-03-22 18:03:49.322322 corl-3.14.13/corl/test_utils/full_training.py
--rw-r--r--   0        0        0      385 2024-03-22 18:03:49.322322 corl-3.14.13/corl/test_utils/testing_ureg_func.py
--rw-r--r--   0        0        0     4867 2024-03-22 18:03:48.872324 corl-3.14.13/corl/train_rl.py
--rw-r--r--   0        0        0        0 2024-03-22 18:03:49.322322 corl-3.14.13/corl/visualization/__init__.py
--rw-r--r--   0        0        0     5213 2024-03-22 18:03:49.352322 corl-3.14.13/corl/visualization/base_animator.py
--rw-r--r--   0        0        0     1951 2024-03-22 18:03:49.352322 corl-3.14.13/corl/visualization/docking_animator.py
--rw-r--r--   0        0        0    31451 2024-03-22 18:03:49.342322 corl-3.14.13/corl/visualization/episode_artifact_to_tables.py
--rw-r--r--   0        0        0        0 2024-03-22 18:03:49.412322 corl-3.14.13/corl/visualization/network_explainability/__init__.py
--rw-r--r--   0        0        0    15435 2024-03-22 18:03:49.442322 corl-3.14.13/corl/visualization/network_explainability/env_policy_transforms.py
--rw-r--r--   0        0        0    32525 2024-03-22 18:03:49.432322 corl-3.14.13/corl/visualization/network_explainability/network_explainability.py
--rw-r--r--   0        0        0     4470 2024-03-22 18:03:49.412322 corl-3.14.13/corl/visualization/network_explainability/network_explainability_plotter.py
--rw-r--r--   0        0        0     3263 2024-03-22 18:03:49.352322 corl-3.14.13/corl/visualization/platform_plotting_deserializer.py
--rw-r--r--   0        0        0    21481 2024-03-22 18:03:49.332322 corl-3.14.13/corl/visualization/plotly_animator.py
--rw-r--r--   0        0        0     2094 2024-03-22 18:03:49.362322 corl-3.14.13/corl/visualization/pong_animator.py
--rw-r--r--   0        0        0        0 2024-03-22 18:03:49.362322 corl-3.14.13/corl/visualization/streamlit_app/__init__.py
--rw-r--r--   0        0        0    10407 2024-03-22 18:03:49.362322 corl-3.14.13/corl/visualization/streamlit_app/default_layout.py
--rw-r--r--   0        0        0    14389 2024-03-22 18:03:49.372322 corl-3.14.13/corl/visualization/streamlit_app/eval_while_train_layout.py
--rw-r--r--   0        0        0     3058 2024-03-22 18:03:49.382322 corl-3.14.13/corl/visualization/streamlit_app/pages/02_evaluation_from_training.py
--rw-r--r--   0        0        0     2642 2024-03-22 18:03:49.382322 corl-3.14.13/corl/visualization/streamlit_app/pages/03_corl_evaluation.py
--rw-r--r--   0        0        0     2401 2024-03-22 18:03:49.392322 corl-3.14.13/corl/visualization/streamlit_app/pages/04_policy_network_viz.py
--rw-r--r--   0        0        0        0 2024-03-22 18:03:49.382322 corl-3.14.13/corl/visualization/streamlit_app/pages/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 18:03:49.392322 corl-3.14.13/corl/visualization/streamlit_app/sections/__init__.py
--rw-r--r--   0        0        0    31764 2024-03-22 18:03:49.402322 corl-3.14.13/corl/visualization/streamlit_app/sections/agent_steps.py
--rw-r--r--   0        0        0     4886 2024-03-22 18:03:49.412322 corl-3.14.13/corl/visualization/streamlit_app/sections/platform_and_agent_dones.py
--rw-r--r--   0        0        0     6058 2024-03-22 18:03:49.412322 corl-3.14.13/corl/visualization/streamlit_app/sections/trajectory_animation.py
--rw-r--r--   0        0        0     6701 2024-03-22 18:03:49.392322 corl-3.14.13/corl/visualization/streamlit_app/sections/units_conversion.py
--rw-r--r--   0        0        0     3010 2024-03-22 18:03:49.372322 corl-3.14.13/corl/visualization/streamlit_app/streamlit_app.py
--rw-r--r--   0        0        0    20456 2024-03-22 18:03:49.382322 corl-3.14.13/corl/visualization/streamlit_app/utils.py
--rw-r--r--   0        0        0     7915 2024-03-22 18:06:52.670912 corl-3.14.13/pyproject.toml
--rw-r--r--   0        0        0      290 2024-03-22 18:03:49.972320 corl-3.14.13/scripts/build.py
--rw-r--r--   0        0        0     6588 1970-01-01 00:00:00.000000 corl-3.14.13/PKG-INFO
+-rw-r--r--   0        0        0      515 2024-04-12 13:43:47.419694 corl-3.16.2/LICENSE.md
+-rw-r--r--   0        0        0     4631 2024-04-12 13:43:47.169695 corl-3.16.2/README.md
+-rw-r--r--   0        0        0      493 2024-04-12 13:43:47.589693 corl-3.16.2/corl/__init__.py
+-rw-r--r--   0        0        0      493 2024-04-12 13:43:48.380219 corl-3.16.2/corl/agents/__init__.py
+-rw-r--r--   0        0        0    39242 2024-04-12 13:43:48.380219 corl-3.16.2/corl/agents/base_agent.py
+-rw-r--r--   0        0        0        0 2024-04-12 13:43:48.390219 corl-3.16.2/corl/agents/non_trainable/__init__.py
+-rw-r--r--   0        0        0      230 2024-04-12 13:43:48.390219 corl-3.16.2/corl/agents/non_trainable/noop.py
+-rw-r--r--   0        0        0      863 2024-04-12 13:43:48.390219 corl-3.16.2/corl/agents/non_trainable/random_action.py
+-rw-r--r--   0        0        0    16210 2024-04-12 13:43:48.390219 corl-3.16.2/corl/agents/simple_multi_platform_agent.py
+-rw-r--r--   0        0        0      511 2024-04-12 13:43:48.490219 corl-3.16.2/corl/config/policy/ppo/default_config.yml
+-rw-r--r--   0        0        0      587 2024-04-12 13:43:48.480219 corl-3.16.2/corl/config/policy/random_action.yml
+-rw-r--r--   0        0        0     1283 2024-04-12 13:43:48.480219 corl-3.16.2/corl/config/policy/scripted_action.yml
+-rw-r--r--   0        0        0     1033 2024-04-12 13:43:48.390219 corl-3.16.2/corl/config/streamlit_app/default_streamlit_config.yml
+-rw-r--r--   0        0        0     1022 2024-04-12 13:43:48.390219 corl-3.16.2/corl/config/streamlit_app/docking1d_streamlit_config.yml
+-rw-r--r--   0        0        0     1023 2024-04-12 13:43:48.390219 corl-3.16.2/corl/config/streamlit_app/pong_streamlit_config.yml
+-rw-r--r--   0        0        0     2457 2024-04-12 13:43:48.410219 corl-3.16.2/corl/config/tasks/docking_1d/agents/docking1d_agent.yml
+-rw-r--r--   0        0        0     1225 2024-04-12 13:43:48.400219 corl-3.16.2/corl/config/tasks/docking_1d/environments/docking1d_env.yml
+-rw-r--r--   0        0        0      191 2024-04-12 13:43:48.410219 corl-3.16.2/corl/config/tasks/docking_1d/evaluation/alerts/base_alerts.yml
+-rw-r--r--   0        0        0     1179 2024-04-12 13:43:48.410219 corl-3.16.2/corl/config/tasks/docking_1d/evaluation/launch/eval_1d_docking.yml
+-rw-r--r--   0        0        0      353 2024-04-12 13:43:48.410219 corl-3.16.2/corl/config/tasks/docking_1d/evaluation/launch/metrics_gen_1d_docking.yml
+-rw-r--r--   0        0        0      336 2024-04-12 13:43:48.410219 corl-3.16.2/corl/config/tasks/docking_1d/evaluation/launch/pipeline_1d_docking.yml
+-rw-r--r--   0        0        0      549 2024-04-12 13:43:48.410219 corl-3.16.2/corl/config/tasks/docking_1d/evaluation/launch/storage_acedt_1d_docking.yml
+-rw-r--r--   0        0        0      236 2024-04-12 13:43:48.410219 corl-3.16.2/corl/config/tasks/docking_1d/evaluation/launch/visualize_1d_docking.yml
+-rw-r--r--   0        0        0     2071 2024-04-12 13:43:48.410219 corl-3.16.2/corl/config/tasks/docking_1d/evaluation/metrics/1d_docking.yml
+-rw-r--r--   0        0        0      179 2024-04-12 13:43:48.410219 corl-3.16.2/corl/config/tasks/docking_1d/evaluation/test_cases_config/docking1d_tests.yml
+-rw-r--r--   0        0        0      424 2024-04-12 13:43:48.400219 corl-3.16.2/corl/config/tasks/docking_1d/experiments/docking_1d.yml
+-rw-r--r--   0        0        0      135 2024-04-12 13:43:48.410219 corl-3.16.2/corl/config/tasks/docking_1d/platforms/docking1d_platform.yml
+-rw-r--r--   0        0        0      954 2024-04-12 13:43:48.400219 corl-3.16.2/corl/config/tasks/docking_1d/ray_config.yml
+-rw-r--r--   0        0        0     1162 2024-04-12 13:43:48.400219 corl-3.16.2/corl/config/tasks/docking_1d/rllib_config.yml
+-rw-r--r--   0        0        0     2649 2024-04-12 13:43:48.400219 corl-3.16.2/corl/config/tasks/docking_1d/tasks/docking1d_task.yml
+-rw-r--r--   0        0        0     1871 2024-04-12 13:43:48.400219 corl-3.16.2/corl/config/tasks/docking_1d/tune_config.yml
+-rw-r--r--   0        0        0       73 2024-04-12 13:43:48.470219 corl-3.16.2/corl/config/tasks/gymnasium/agents/baseline_dones.yml
+-rw-r--r--   0        0        0       81 2024-04-12 13:43:48.480219 corl-3.16.2/corl/config/tasks/gymnasium/agents/baseline_epp.yml
+-rw-r--r--   0        0        0      126 2024-04-12 13:43:48.480219 corl-3.16.2/corl/config/tasks/gymnasium/agents/baseline_rewards.yml
+-rw-r--r--   0        0        0     1399 2024-04-12 13:43:48.480219 corl-3.16.2/corl/config/tasks/gymnasium/agents/gymnasium_agent.yml
+-rw-r--r--   0        0        0     3739 2024-04-12 13:43:48.480219 corl-3.16.2/corl/config/tasks/gymnasium/agents/gymnasium_agent_dict_wrapper.yml
+-rw-r--r--   0        0        0     1434 2024-04-12 13:43:48.480219 corl-3.16.2/corl/config/tasks/gymnasium/agents/gymnasium_agent_noop.yml
+-rw-r--r--   0        0        0     1413 2024-04-12 13:43:48.470219 corl-3.16.2/corl/config/tasks/gymnasium/agents/gymnasium_agent_noop_ctrl.yml
+-rw-r--r--   0        0        0     1530 2024-04-12 13:43:48.480219 corl-3.16.2/corl/config/tasks/gymnasium/agents/gymnasium_agent_repeated.yml
+-rw-r--r--   0        0        0     4179 2024-04-12 13:43:48.480219 corl-3.16.2/corl/config/tasks/gymnasium/agents/gymnasium_agent_wrapper.yml
+-rw-r--r--   0        0        0      868 2024-04-12 13:43:48.470219 corl-3.16.2/corl/config/tasks/gymnasium/environments/cartpole_v1.yml
+-rw-r--r--   0        0        0     1018 2024-04-12 13:43:48.470219 corl-3.16.2/corl/config/tasks/gymnasium/environments/cartpole_v1_with_time.yml
+-rw-r--r--   0        0        0      996 2024-04-12 13:43:48.470219 corl-3.16.2/corl/config/tasks/gymnasium/environments/pendulum_v1.yml
+-rw-r--r--   0        0        0      347 2024-04-12 13:43:48.460219 corl-3.16.2/corl/config/tasks/gymnasium/experiments/cartpole_v1.yml
+-rw-r--r--   0        0        0      357 2024-04-12 13:43:48.460219 corl-3.16.2/corl/config/tasks/gymnasium/experiments/cartpole_v1_benchmark.yml
+-rw-r--r--   0        0        0      360 2024-04-12 13:43:48.460219 corl-3.16.2/corl/config/tasks/gymnasium/experiments/cartpole_v1_dict_wrapper.yml
+-rw-r--r--   0        0        0      586 2024-04-12 13:43:48.460219 corl-3.16.2/corl/config/tasks/gymnasium/experiments/cartpole_v1_noop.yml
+-rw-r--r--   0        0        0      604 2024-04-12 13:43:48.460219 corl-3.16.2/corl/config/tasks/gymnasium/experiments/cartpole_v1_noop_ctrl.yml
+-rw-r--r--   0        0        0      587 2024-04-12 13:43:48.460219 corl-3.16.2/corl/config/tasks/gymnasium/experiments/cartpole_v1_random.yml
+-rw-r--r--   0        0        0      356 2024-04-12 13:43:48.460219 corl-3.16.2/corl/config/tasks/gymnasium/experiments/cartpole_v1_repeated_obs.yml
+-rw-r--r--   0        0        0      605 2024-04-12 13:43:48.460219 corl-3.16.2/corl/config/tasks/gymnasium/experiments/cartpole_v1_scripted.yml
+-rw-r--r--   0        0        0      371 2024-04-12 13:43:48.460219 corl-3.16.2/corl/config/tasks/gymnasium/experiments/cartpole_v1_with_wrapper.yml
+-rw-r--r--   0        0        0      347 2024-04-12 13:43:48.460219 corl-3.16.2/corl/config/tasks/gymnasium/experiments/pendulum_v1.yml
+-rw-r--r--   0        0        0      590 2024-04-12 13:43:48.470219 corl-3.16.2/corl/config/tasks/gymnasium/platforms/gymnasium_platform.yml
+-rw-r--r--   0        0        0      604 2024-04-12 13:43:48.470219 corl-3.16.2/corl/config/tasks/gymnasium/platforms/gymnasium_platform_inclusive_parts.yml
+-rw-r--r--   0        0        0      953 2024-04-12 13:43:48.460219 corl-3.16.2/corl/config/tasks/gymnasium/ray_config.yml
+-rw-r--r--   0        0        0      909 2024-04-12 13:43:48.450219 corl-3.16.2/corl/config/tasks/gymnasium/rllib_config.yml
+-rw-r--r--   0        0        0     3171 2024-04-12 13:43:48.460219 corl-3.16.2/corl/config/tasks/gymnasium/tasks/cartpole_v1.yml
+-rw-r--r--   0        0        0     3179 2024-04-12 13:43:48.470219 corl-3.16.2/corl/config/tasks/gymnasium/tasks/cartpole_v1_benchmark.yml
+-rw-r--r--   0        0        0     3180 2024-04-12 13:43:48.470219 corl-3.16.2/corl/config/tasks/gymnasium/tasks/cartpole_v1_with_time.yml
+-rw-r--r--   0        0        0     1800 2024-04-12 13:43:48.470219 corl-3.16.2/corl/config/tasks/gymnasium/tasks/pendulum_v1.yml
+-rw-r--r--   0        0        0     1872 2024-04-12 13:43:48.460219 corl-3.16.2/corl/config/tasks/gymnasium/tune_config.yml
+-rw-r--r--   0        0        0     5812 2024-04-12 13:43:48.450219 corl-3.16.2/corl/config/tasks/pong/agents/commander_paddle_agent.yml
+-rw-r--r--   0        0        0      726 2024-04-12 13:43:48.450219 corl-3.16.2/corl/config/tasks/pong/agents/dummy_noop.yml
+-rw-r--r--   0        0        0     1689 2024-04-12 13:43:48.450219 corl-3.16.2/corl/config/tasks/pong/agents/paddle_agent-scripted-noop.yml
+-rw-r--r--   0        0        0     1706 2024-04-12 13:43:48.450219 corl-3.16.2/corl/config/tasks/pong/agents/paddle_agent-scripted-random_action.yml
+-rw-r--r--   0        0        0     1962 2024-04-12 13:43:48.450219 corl-3.16.2/corl/config/tasks/pong/agents/paddle_agent.yml
+-rw-r--r--   0        0        0     2422 2024-04-12 13:43:48.450219 corl-3.16.2/corl/config/tasks/pong/agents/paddle_agent_flat_actions.yml
+-rw-r--r--   0        0        0      935 2024-04-12 13:43:48.420219 corl-3.16.2/corl/config/tasks/pong/commander_rllib_config.yml
+-rw-r--r--   0        0        0     2293 2024-04-12 13:43:48.440219 corl-3.16.2/corl/config/tasks/pong/environments/commander_pong_env.yml
+-rw-r--r--   0        0        0     1586 2024-04-12 13:43:48.440219 corl-3.16.2/corl/config/tasks/pong/environments/pong_env.yml
+-rw-r--r--   0        0        0     1810 2024-04-12 13:43:48.440219 corl-3.16.2/corl/config/tasks/pong/evaluation/launch/base_pong_evaluate.yml
+-rw-r--r--   0        0        0      333 2024-04-12 13:43:48.440219 corl-3.16.2/corl/config/tasks/pong/evaluation/launch/base_pong_inference.yml
+-rw-r--r--   0        0        0     1496 2024-04-12 13:43:48.440219 corl-3.16.2/corl/config/tasks/pong/evaluation/launch/commander_pong_evaluate.yml
+-rw-r--r--   0        0        0      108 2024-04-12 13:43:48.440219 corl-3.16.2/corl/config/tasks/pong/evaluation/launch/inference.yml
+-rw-r--r--   0        0        0      456 2024-04-12 13:43:48.450219 corl-3.16.2/corl/config/tasks/pong/evaluation/test_cases/commander_pong_test_cases.yml
+-rw-r--r--   0        0        0      936 2024-04-12 13:43:48.420219 corl-3.16.2/corl/config/tasks/pong/experiments/pong-both_scripted-random_action.yml
+-rw-r--r--   0        0        0      749 2024-04-12 13:43:48.420219 corl-3.16.2/corl/config/tasks/pong/experiments/pong-one_scripted-centralized-critic.yml
+-rw-r--r--   0        0        0      705 2024-04-12 13:43:48.420219 corl-3.16.2/corl/config/tasks/pong/experiments/pong-one_scripted-noop.yml
+-rw-r--r--   0        0        0      714 2024-04-12 13:43:48.420219 corl-3.16.2/corl/config/tasks/pong/experiments/pong-one_scripted-random_action.yml
+-rw-r--r--   0        0        0      706 2024-04-12 13:43:48.420219 corl-3.16.2/corl/config/tasks/pong/experiments/pong.yml
+-rw-r--r--   0        0        0      696 2024-04-12 13:43:48.420219 corl-3.16.2/corl/config/tasks/pong/experiments/pong_alt.yml
+-rw-r--r--   0        0        0      755 2024-04-12 13:43:48.420219 corl-3.16.2/corl/config/tasks/pong/experiments/pong_centralized_critic.yml
+-rw-r--r--   0        0        0      527 2024-04-12 13:43:48.430219 corl-3.16.2/corl/config/tasks/pong/experiments/pong_commander.yml
+-rw-r--r--   0        0        0      694 2024-04-12 13:43:48.430219 corl-3.16.2/corl/config/tasks/pong/experiments/pong_group.yml
+-rw-r--r--   0        0        0      580 2024-04-12 13:43:48.420219 corl-3.16.2/corl/config/tasks/pong/experiments/pong_sac.yml
+-rw-r--r--   0        0        0       19 2024-04-12 13:43:48.450219 corl-3.16.2/corl/config/tasks/pong/platforms/paddle.yml
+-rw-r--r--   0        0        0      143 2024-04-12 13:43:48.440219 corl-3.16.2/corl/config/tasks/pong/policies/heuristic_paddle_policy.yml
+-rw-r--r--   0        0        0       23 2024-04-12 13:43:48.440219 corl-3.16.2/corl/config/tasks/pong/policies/no_policy.yml
+-rw-r--r--   0        0        0      662 2024-04-12 13:43:48.440219 corl-3.16.2/corl/config/tasks/pong/policies/ppo_config.yml
+-rw-r--r--   0        0        0      725 2024-04-12 13:43:48.440219 corl-3.16.2/corl/config/tasks/pong/policies/ppo_config_central_critic.yml
+-rw-r--r--   0        0        0      581 2024-04-12 13:43:48.440219 corl-3.16.2/corl/config/tasks/pong/policies/sac_config.yml
+-rw-r--r--   0        0        0      950 2024-04-12 13:43:48.420219 corl-3.16.2/corl/config/tasks/pong/ray_config.yml
+-rw-r--r--   0        0        0     1035 2024-04-12 13:43:48.410219 corl-3.16.2/corl/config/tasks/pong/rllib_config.yml
+-rw-r--r--   0        0        0     1947 2024-04-12 13:43:48.430219 corl-3.16.2/corl/config/tasks/pong/tasks/pong_commander_task_ppo.yml
+-rw-r--r--   0        0        0     2313 2024-04-12 13:43:48.430219 corl-3.16.2/corl/config/tasks/pong/tasks/pong_task_group.yml
+-rw-r--r--   0        0        0     2192 2024-04-12 13:43:48.440219 corl-3.16.2/corl/config/tasks/pong/tasks/pong_task_ppo-all_scripted.yml
+-rw-r--r--   0        0        0     2329 2024-04-12 13:43:48.430219 corl-3.16.2/corl/config/tasks/pong/tasks/pong_task_ppo.yml
+-rw-r--r--   0        0        0     2415 2024-04-12 13:43:48.430219 corl-3.16.2/corl/config/tasks/pong/tasks/pong_task_ppo_alt.yml
+-rw-r--r--   0        0        0     2157 2024-04-12 13:43:48.430219 corl-3.16.2/corl/config/tasks/pong/tasks/pong_task_ppo_centralized_critic.yml
+-rw-r--r--   0        0        0     2282 2024-04-12 13:43:48.430219 corl-3.16.2/corl/config/tasks/pong/tasks/pong_task_sac.yml
+-rw-r--r--   0        0        0     1870 2024-04-12 13:43:48.410219 corl-3.16.2/corl/config/tasks/pong/tune_config_ppo.yml
+-rw-r--r--   0        0        0     1870 2024-04-12 13:43:48.420219 corl-3.16.2/corl/config/tasks/pong/tune_config_sac.yml
+-rw-r--r--   0        0        0      954 2024-04-12 13:43:48.400219 corl-3.16.2/corl/config/tasks/ray_config.yml
+-rw-r--r--   0        0        0     1111 2024-04-12 13:43:48.400219 corl-3.16.2/corl/config/tasks/rllib_config.yml
+-rw-r--r--   0        0        0     1871 2024-04-12 13:43:48.400219 corl-3.16.2/corl/config/tasks/tune_config.yml
+-rw-r--r--   0        0        0      493 2024-04-12 13:43:47.819692 corl-3.16.2/corl/dones/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 13:43:47.829692 corl-3.16.2/corl/dones/docking_1d/__init__.py
+-rw-r--r--   0        0        0     3196 2024-04-12 13:43:47.829692 corl-3.16.2/corl/dones/docking_1d/dones.py
+-rw-r--r--   0        0        0     4617 2024-04-12 13:43:47.829692 corl-3.16.2/corl/dones/done_func_base.py
+-rw-r--r--   0        0        0     1800 2024-04-12 13:43:47.819692 corl-3.16.2/corl/dones/done_func_dict_wrapper.py
+-rw-r--r--   0        0        0     1754 2024-04-12 13:43:47.819692 corl-3.16.2/corl/dones/done_func_multi_wrapper.py
+-rw-r--r--   0        0        0     1716 2024-04-12 13:43:47.819692 corl-3.16.2/corl/dones/done_func_wrapper.py
+-rw-r--r--   0        0        0     2175 2024-04-12 13:43:47.819692 corl-3.16.2/corl/dones/episode_length_done.py
+-rw-r--r--   0        0        0     1060 2024-04-12 13:43:47.819692 corl-3.16.2/corl/dones/gymnasium_done.py
+-rw-r--r--   0        0        0        0 2024-04-12 13:43:47.829692 corl-3.16.2/corl/dones/pong/__init__.py
+-rw-r--r--   0        0        0     3068 2024-04-12 13:43:47.829692 corl-3.16.2/corl/dones/pong/commander_pong_dones.py
+-rw-r--r--   0        0        0     3042 2024-04-12 13:43:47.829692 corl-3.16.2/corl/dones/pong/dones.py
+-rw-r--r--   0        0        0     4026 2024-04-12 13:43:47.829692 corl-3.16.2/corl/dones/sensor_bounds_check_done.py
+-rw-r--r--   0        0        0      493 2024-04-12 13:43:48.019690 corl-3.16.2/corl/environment/__init__.py
+-rw-r--r--   0        0        0     6778 2024-04-12 13:43:48.059690 corl-3.16.2/corl/environment/base_multi_agent_env.py
+-rw-r--r--   0        0        0    17979 2024-04-12 13:43:48.069690 corl-3.16.2/corl/environment/centralized_critic_environment.py
+-rw-r--r--   0        0        0     1508 2024-04-12 13:43:48.019690 corl-3.16.2/corl/environment/custom_env_metrics.py
+-rw-r--r--   0        0        0    13050 2024-04-12 13:43:48.019690 corl-3.16.2/corl/environment/default_env_rllib_callbacks.py
+-rw-r--r--   0        0        0     8747 2024-04-12 13:43:48.029690 corl-3.16.2/corl/environment/environment_wrappers.py
+-rw-r--r--   0        0        0     1269 2024-04-12 13:43:48.019690 corl-3.16.2/corl/environment/episode_artifact_callbacks.py
+-rw-r--r--   0        0        0      493 2024-04-12 13:43:48.019690 corl-3.16.2/corl/environment/gym_env.py
+-rw-r--r--   0        0        0    67827 2024-04-12 13:43:48.049690 corl-3.16.2/corl/environment/multi_agent_env.py
+-rw-r--r--   0        0        0     3407 2024-04-12 13:43:48.029690 corl-3.16.2/corl/environment/pickle_env_state.py
+-rw-r--r--   0        0        0      493 2024-04-12 13:43:48.069690 corl-3.16.2/corl/environment/utils/__init__.py
+-rw-r--r--   0        0        0     3251 2024-04-12 13:43:48.069690 corl-3.16.2/corl/environment/utils/env_creation.py
+-rw-r--r--   0        0        0     2480 2024-04-12 13:43:48.069690 corl-3.16.2/corl/environment/utils/obs_buffer.py
+-rw-r--r--   0        0        0     1840 2024-04-12 13:43:48.069690 corl-3.16.2/corl/environment/utils/space_sort.py
+-rw-r--r--   0        0        0      842 2024-04-12 13:43:48.259689 corl-3.16.2/corl/episode_parameter_providers/__init__.py
+-rw-r--r--   0        0        0     3938 2024-04-12 13:43:48.269689 corl-3.16.2/corl/episode_parameter_providers/base_network_epp.py
+-rw-r--r--   0        0        0     5012 2024-04-12 13:43:48.259689 corl-3.16.2/corl/episode_parameter_providers/core.py
+-rw-r--r--   0        0        0     2817 2024-04-12 13:43:48.269689 corl-3.16.2/corl/episode_parameter_providers/incremental.py
+-rw-r--r--   0        0        0     5438 2024-04-12 13:43:48.259689 corl-3.16.2/corl/episode_parameter_providers/remote.py
+-rw-r--r--   0        0        0      935 2024-04-12 13:43:48.269689 corl-3.16.2/corl/episode_parameter_providers/simple.py
+-rw-r--r--   0        0        0     4047 2024-04-12 13:43:48.259689 corl-3.16.2/corl/episode_parameter_providers/tabular_parameter_provider.py
+-rw-r--r--   0        0        0      511 2024-04-12 13:43:48.079690 corl-3.16.2/corl/evaluation/__init__.py
+-rw-r--r--   0        0        0    15068 2024-04-12 13:43:48.079690 corl-3.16.2/corl/evaluation/api.py
+-rw-r--r--   0        0        0    17373 2024-04-12 13:43:48.089690 corl-3.16.2/corl/evaluation/api_utils.py
+-rw-r--r--   0        0        0        0 2024-04-12 13:43:48.149690 corl-3.16.2/corl/evaluation/connection/__init__.py
+-rw-r--r--   0        0        0     1182 2024-04-12 13:43:48.149690 corl-3.16.2/corl/evaluation/connection/base_epp_update.py
+-rw-r--r--   0        0        0     1752 2024-04-12 13:43:48.149690 corl-3.16.2/corl/evaluation/connection/base_eval_connection.py
+-rw-r--r--   0        0        0     2249 2024-04-12 13:43:48.149690 corl-3.16.2/corl/evaluation/connection/base_rest_connection.py
+-rw-r--r--   0        0        0     5287 2024-04-12 13:43:48.149690 corl-3.16.2/corl/evaluation/connection/signal.py
+-rw-r--r--   0        0        0      859 2024-04-12 13:43:48.079690 corl-3.16.2/corl/evaluation/default_config_updates.py
+-rw-r--r--   0        0        0     3886 2024-04-12 13:43:48.099690 corl-3.16.2/corl/evaluation/episode_artifact.py
+-rw-r--r--   0        0        0      561 2024-04-12 13:43:48.089690 corl-3.16.2/corl/evaluation/eval_logger_name.py
+-rw-r--r--   0        0        0     1955 2024-04-12 13:43:48.099690 corl-3.16.2/corl/evaluation/evaluation_artifacts.py
+-rw-r--r--   0        0        0     1188 2024-04-12 13:43:48.069690 corl-3.16.2/corl/evaluation/evaluation_factory.py
+-rw-r--r--   0        0        0     1310 2024-04-12 13:43:48.089690 corl-3.16.2/corl/evaluation/evaluation_outcome.py
+-rw-r--r--   0        0        0      537 2024-04-12 13:43:48.239689 corl-3.16.2/corl/evaluation/launchers/__init__.py
+-rw-r--r--   0        0        0     3706 2024-04-12 13:43:48.249689 corl-3.16.2/corl/evaluation/launchers/base_eval.py
+-rw-r--r--   0        0        0     5759 2024-04-12 13:43:48.239689 corl-3.16.2/corl/evaluation/launchers/evaluate_runner.py
+-rw-r--r--   0        0        0     5438 2024-04-12 13:43:48.249689 corl-3.16.2/corl/evaluation/launchers/evaluate_validator.py
+-rw-r--r--   0        0        0     7007 2024-04-12 13:43:48.239689 corl-3.16.2/corl/evaluation/launchers/launch_evaluate.py
+-rw-r--r--   0        0        0     5582 2024-04-12 13:43:48.259689 corl-3.16.2/corl/evaluation/launchers/launch_generate_metrics.py
+-rw-r--r--   0        0        0    10207 2024-04-12 13:43:48.249689 corl-3.16.2/corl/evaluation/launchers/launch_pipeline.py
+-rw-r--r--   0        0        0     2191 2024-04-12 13:43:48.239689 corl-3.16.2/corl/evaluation/launchers/launch_storage.py
+-rw-r--r--   0        0        0     2503 2024-04-12 13:43:48.229689 corl-3.16.2/corl/evaluation/launchers/launch_visualize.py
+-rw-r--r--   0        0        0     2769 2024-04-12 13:43:48.239689 corl-3.16.2/corl/evaluation/launchers/rest_eval_connection.py
+-rw-r--r--   0        0        0      549 2024-04-12 13:43:48.229689 corl-3.16.2/corl/evaluation/loader/__init__.py
+-rw-r--r--   0        0        0     1048 2024-04-12 13:43:48.229689 corl-3.16.2/corl/evaluation/loader/heuristic.py
+-rw-r--r--   0        0        0     5547 2024-04-12 13:43:48.229689 corl-3.16.2/corl/evaluation/loader/i_agent_loader.py
+-rw-r--r--   0        0        0     4647 2024-04-12 13:43:48.229689 corl-3.16.2/corl/evaluation/loader/policy_checkpoint.py
+-rw-r--r--   0        0        0      493 2024-04-12 13:43:48.099690 corl-3.16.2/corl/evaluation/metrics/__init__.py
+-rw-r--r--   0        0        0      493 2024-04-12 13:43:48.119690 corl-3.16.2/corl/evaluation/metrics/aggregators/__init__.py
+-rw-r--r--   0        0        0     1933 2024-04-12 13:43:48.119690 corl-3.16.2/corl/evaluation/metrics/aggregators/accumulate.py
+-rw-r--r--   0        0        0     2137 2024-04-12 13:43:48.119690 corl-3.16.2/corl/evaluation/metrics/aggregators/average.py
+-rw-r--r--   0        0        0     2438 2024-04-12 13:43:48.129690 corl-3.16.2/corl/evaluation/metrics/aggregators/counter.py
+-rw-r--r--   0        0        0     1590 2024-04-12 13:43:48.119690 corl-3.16.2/corl/evaluation/metrics/aggregators/criteria_rate.py
+-rw-r--r--   0        0        0     2003 2024-04-12 13:43:48.129690 corl-3.16.2/corl/evaluation/metrics/aggregators/sum.py
+-rw-r--r--   0        0        0     2867 2024-04-12 13:43:48.099690 corl-3.16.2/corl/evaluation/metrics/alerts.py
+-rw-r--r--   0        0        0     2644 2024-04-12 13:43:48.099690 corl-3.16.2/corl/evaluation/metrics/generator.py
+-rw-r--r--   0        0        0      493 2024-04-12 13:43:48.109690 corl-3.16.2/corl/evaluation/metrics/generators/__init__.py
+-rw-r--r--   0        0        0     2294 2024-04-12 13:43:48.119690 corl-3.16.2/corl/evaluation/metrics/generators/dones.py
+-rw-r--r--   0        0        0      493 2024-04-12 13:43:48.119690 corl-3.16.2/corl/evaluation/metrics/generators/meta/__init__.py
+-rw-r--r--   0        0        0     1040 2024-04-12 13:43:48.119690 corl-3.16.2/corl/evaluation/metrics/generators/meta/episode_length.py
+-rw-r--r--   0        0        0     1030 2024-04-12 13:43:48.119690 corl-3.16.2/corl/evaluation/metrics/generators/meta/runtime.py
+-rw-r--r--   0        0        0     3005 2024-04-12 13:43:48.119690 corl-3.16.2/corl/evaluation/metrics/generators/rewards.py
+-rw-r--r--   0        0        0     1242 2024-04-12 13:43:48.109690 corl-3.16.2/corl/evaluation/metrics/metric.py
+-rw-r--r--   0        0        0    11777 2024-04-12 13:43:48.109690 corl-3.16.2/corl/evaluation/metrics/processors.py
+-rw-r--r--   0        0        0     1896 2024-04-12 13:43:48.109690 corl-3.16.2/corl/evaluation/metrics/scenario_alert_generators.py
+-rw-r--r--   0        0        0     2918 2024-04-12 13:43:48.099690 corl-3.16.2/corl/evaluation/metrics/scenario_metric_generators.py
+-rw-r--r--   0        0        0     1140 2024-04-12 13:43:48.109690 corl-3.16.2/corl/evaluation/metrics/scopes.py
+-rw-r--r--   0        0        0      493 2024-04-12 13:43:48.129690 corl-3.16.2/corl/evaluation/metrics/types/__init__.py
+-rw-r--r--   0        0        0      493 2024-04-12 13:43:48.139690 corl-3.16.2/corl/evaluation/metrics/types/nonterminals/__init__.py
+-rw-r--r--   0        0        0     1474 2024-04-12 13:43:48.129690 corl-3.16.2/corl/evaluation/metrics/types/nonterminals/dict.py
+-rw-r--r--   0        0        0     1324 2024-04-12 13:43:48.139690 corl-3.16.2/corl/evaluation/metrics/types/nonterminals/timed_value.py
+-rw-r--r--   0        0        0     1506 2024-04-12 13:43:48.139690 corl-3.16.2/corl/evaluation/metrics/types/nonterminals/vector.py
+-rw-r--r--   0        0        0      493 2024-04-12 13:43:48.129690 corl-3.16.2/corl/evaluation/metrics/types/terminals/__init__.py
+-rw-r--r--   0        0        0     1086 2024-04-12 13:43:48.129690 corl-3.16.2/corl/evaluation/metrics/types/terminals/discrete.py
+-rw-r--r--   0        0        0     2342 2024-04-12 13:43:48.129690 corl-3.16.2/corl/evaluation/metrics/types/terminals/rate.py
+-rw-r--r--   0        0        0     1962 2024-04-12 13:43:48.129690 corl-3.16.2/corl/evaluation/metrics/types/terminals/real.py
+-rw-r--r--   0        0        0     1011 2024-04-12 13:43:48.129690 corl-3.16.2/corl/evaluation/metrics/types/terminals/string.py
+-rw-r--r--   0        0        0      874 2024-04-12 13:43:48.129690 corl-3.16.2/corl/evaluation/metrics/types/terminals/void.py
+-rw-r--r--   0        0        0      510 2024-04-12 13:43:48.219689 corl-3.16.2/corl/evaluation/recording/__init__.py
+-rw-r--r--   0        0        0     7598 2024-04-12 13:43:48.219689 corl-3.16.2/corl/evaluation/recording/folder.py
+-rw-r--r--   0        0        0     1621 2024-04-12 13:43:48.219689 corl-3.16.2/corl/evaluation/recording/i_recorder.py
+-rw-r--r--   0        0        0      537 2024-04-12 13:43:48.149690 corl-3.16.2/corl/evaluation/runners/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 13:43:48.209689 corl-3.16.2/corl/evaluation/runners/inference/__init__.py
+-rw-r--r--   0        0        0     7560 2024-04-12 13:43:48.209689 corl-3.16.2/corl/evaluation/runners/inference/algorithm_runner.py
+-rw-r--r--   0        0        0     1871 2024-04-12 13:43:48.209689 corl-3.16.2/corl/evaluation/runners/inference/inference.py
+-rw-r--r--   0        0        0     1541 2024-04-12 13:43:48.209689 corl-3.16.2/corl/evaluation/runners/inference/inference_callback.py
+-rw-r--r--   0        0        0        0 2024-04-12 13:43:48.219689 corl-3.16.2/corl/evaluation/runners/inference/protocol/__init__.py
+-rw-r--r--   0        0        0     1039 2024-04-12 13:43:48.219689 corl-3.16.2/corl/evaluation/runners/inference/protocol/simple_epp_update.py
+-rw-r--r--   0        0        0     2760 2024-04-12 13:43:48.219689 corl-3.16.2/corl/evaluation/runners/inference/protocol/simple_network_epp.py
+-rw-r--r--   0        0        0     1781 2024-04-12 13:43:48.219689 corl-3.16.2/corl/evaluation/runners/inference/protocol/simple_network_epp_strategy.py
+-rw-r--r--   0        0        0    13553 2024-04-12 13:43:48.159690 corl-3.16.2/corl/evaluation/runners/iterate_test_cases.py
+-rw-r--r--   0        0        0      582 2024-04-12 13:43:48.159690 corl-3.16.2/corl/evaluation/runners/section_factories/__init__.py
+-rw-r--r--   0        0        0      550 2024-04-12 13:43:48.159690 corl-3.16.2/corl/evaluation/runners/section_factories/engine/__init__.py
+-rw-r--r--   0        0        0      513 2024-04-12 13:43:48.169690 corl-3.16.2/corl/evaluation/runners/section_factories/engine/rllib/__init__.py
+-rw-r--r--   0        0        0    17770 2024-04-12 13:43:48.169690 corl-3.16.2/corl/evaluation/runners/section_factories/engine/rllib/default_evaluation_callbacks.py
+-rw-r--r--   0        0        0    10851 2024-04-12 13:43:48.179690 corl-3.16.2/corl/evaluation/runners/section_factories/engine/rllib/episode_artifact_logging_callback.py
+-rw-r--r--   0        0        0     3326 2024-04-12 13:43:48.179690 corl-3.16.2/corl/evaluation/runners/section_factories/engine/rllib/eval_config_updates.py
+-rw-r--r--   0        0        0     1939 2024-04-12 13:43:48.169690 corl-3.16.2/corl/evaluation/runners/section_factories/engine/rllib/interruptable_callback.py
+-rw-r--r--   0        0        0    10280 2024-04-12 13:43:48.179690 corl-3.16.2/corl/evaluation/runners/section_factories/engine/rllib/rllib_trainer.py
+-rw-r--r--   0        0        0      493 2024-04-12 13:43:48.199689 corl-3.16.2/corl/evaluation/runners/section_factories/plugins/__init__.py
+-rw-r--r--   0        0        0      887 2024-04-12 13:43:48.209689 corl-3.16.2/corl/evaluation/runners/section_factories/plugins/config_updater.py
+-rw-r--r--   0        0        0      868 2024-04-12 13:43:48.209689 corl-3.16.2/corl/evaluation/runners/section_factories/plugins/environment_state_extractor.py
+-rw-r--r--   0        0        0     1023 2024-04-12 13:43:48.209689 corl-3.16.2/corl/evaluation/runners/section_factories/plugins/platform_serializer.py
+-rw-r--r--   0        0        0     1498 2024-04-12 13:43:48.209689 corl-3.16.2/corl/evaluation/runners/section_factories/plugins/plugins.py
+-rw-r--r--   0        0        0     4669 2024-04-12 13:43:48.159690 corl-3.16.2/corl/evaluation/runners/section_factories/task.py
+-rw-r--r--   0        0        0     1731 2024-04-12 13:43:48.159690 corl-3.16.2/corl/evaluation/runners/section_factories/teams.py
+-rw-r--r--   0        0        0      516 2024-04-12 13:43:48.189689 corl-3.16.2/corl/evaluation/runners/section_factories/test_cases/__init__.py
+-rw-r--r--   0        0        0     4105 2024-04-12 13:43:48.199689 corl-3.16.2/corl/evaluation/runners/section_factories/test_cases/base_network_strategy.py
+-rw-r--r--   0        0        0     7951 2024-04-12 13:43:48.189689 corl-3.16.2/corl/evaluation/runners/section_factories/test_cases/config_parser.py
+-rw-r--r--   0        0        0     3984 2024-04-12 13:43:48.199689 corl-3.16.2/corl/evaluation/runners/section_factories/test_cases/default_strategy.py
+-rw-r--r--   0        0        0     5721 2024-04-12 13:43:48.199689 corl-3.16.2/corl/evaluation/runners/section_factories/test_cases/pandas.py
+-rw-r--r--   0        0        0     5306 2024-04-12 13:43:48.189689 corl-3.16.2/corl/evaluation/runners/section_factories/test_cases/tabular_strategy.py
+-rw-r--r--   0        0        0     7006 2024-04-12 13:43:48.189689 corl-3.16.2/corl/evaluation/runners/section_factories/test_cases/test_case_generator.py
+-rw-r--r--   0        0        0     4082 2024-04-12 13:43:48.199689 corl-3.16.2/corl/evaluation/runners/section_factories/test_cases/test_case_manager.py
+-rw-r--r--   0        0        0     4245 2024-04-12 13:43:48.099690 corl-3.16.2/corl/evaluation/scene_processors.py
+-rw-r--r--   0        0        0     6078 2024-04-12 13:43:48.079690 corl-3.16.2/corl/evaluation/serialize_platforms.py
+-rw-r--r--   0        0        0      537 2024-04-12 13:43:48.229689 corl-3.16.2/corl/evaluation/util/__init__.py
+-rw-r--r--   0        0        0     2266 2024-04-12 13:43:48.219689 corl-3.16.2/corl/evaluation/util/condition.py
+-rw-r--r--   0        0        0     1112 2024-04-12 13:43:48.229689 corl-3.16.2/corl/evaluation/util/storage.py
+-rw-r--r--   0        0        0      542 2024-04-12 13:43:48.139690 corl-3.16.2/corl/evaluation/visualization/__init__.py
+-rw-r--r--   0        0        0     7187 2024-04-12 13:43:48.149690 corl-3.16.2/corl/evaluation/visualization/html_plots.py
+-rw-r--r--   0        0        0    10716 2024-04-12 13:43:48.139690 corl-3.16.2/corl/evaluation/visualization/print.py
+-rw-r--r--   0        0        0     2029 2024-04-12 13:43:48.139690 corl-3.16.2/corl/evaluation/visualization/visualization.py
+-rw-r--r--   0        0        0      493 2024-04-12 13:43:47.789692 corl-3.16.2/corl/experiments/__init__.py
+-rw-r--r--   0        0        0     7204 2024-04-12 13:43:47.799692 corl-3.16.2/corl/experiments/base_experiment.py
+-rw-r--r--   0        0        0    13210 2024-04-12 13:43:47.809692 corl-3.16.2/corl/experiments/benchmark_experiment.py
+-rwxr-xr-x   0        0        0    14584 2024-04-12 13:43:47.789692 corl-3.16.2/corl/experiments/export_setup_experiment.py
+-rw-r--r--   0        0        0    25797 2024-04-12 13:43:47.809692 corl-3.16.2/corl/experiments/rllib_experiment.py
+-rw-r--r--   0        0        0        0 2024-04-12 13:43:47.819692 corl-3.16.2/corl/experiments/rllib_utils/__init__.py
+-rw-r--r--   0        0        0     1914 2024-04-12 13:43:47.819692 corl-3.16.2/corl/experiments/rllib_utils/policy_mapping_functions.py
+-rw-r--r--   0        0        0      853 2024-04-12 13:43:47.819692 corl-3.16.2/corl/experiments/rllib_utils/wrappers.py
+-rw-r--r--   0        0        0      493 2024-04-12 13:43:47.839691 corl-3.16.2/corl/glues/__init__.py
+-rw-r--r--   0        0        0     1560 2024-04-12 13:43:47.839691 corl-3.16.2/corl/glues/base_dict_wrapper.py
+-rw-r--r--   0        0        0    15621 2024-04-12 13:43:47.839691 corl-3.16.2/corl/glues/base_glue.py
+-rw-r--r--   0        0        0     1519 2024-04-12 13:43:47.849691 corl-3.16.2/corl/glues/base_multi_wrapper.py
+-rw-r--r--   0        0        0     1460 2024-04-12 13:43:47.839691 corl-3.16.2/corl/glues/base_wrapper.py
+-rw-r--r--   0        0        0      493 2024-04-12 13:43:47.859691 corl-3.16.2/corl/glues/common/__init__.py
+-rw-r--r--   0        0        0     4927 2024-04-12 13:43:47.859691 corl-3.16.2/corl/glues/common/controller_glue.py
+-rw-r--r--   0        0        0     3411 2024-04-12 13:43:47.859691 corl-3.16.2/corl/glues/common/magnitude.py
+-rw-r--r--   0        0        0     2278 2024-04-12 13:43:47.859691 corl-3.16.2/corl/glues/common/observe_part_validity.py
+-rw-r--r--   0        0        0     3999 2024-04-12 13:43:47.869691 corl-3.16.2/corl/glues/common/observe_sensor.py
+-rw-r--r--   0        0        0     5339 2024-04-12 13:43:47.879691 corl-3.16.2/corl/glues/common/observe_sensor_repeated.py
+-rw-r--r--   0        0        0     2826 2024-04-12 13:43:47.869691 corl-3.16.2/corl/glues/common/projected_quantity.py
+-rw-r--r--   0        0        0     6176 2024-04-12 13:43:47.869691 corl-3.16.2/corl/glues/common/target_value.py
+-rw-r--r--   0        0        0     7411 2024-04-12 13:43:47.859691 corl-3.16.2/corl/glues/common/target_value_difference.py
+-rw-r--r--   0        0        0     3205 2024-04-12 13:43:47.869691 corl-3.16.2/corl/glues/common/trig_values.py
+-rw-r--r--   0        0        0     2860 2024-04-12 13:43:47.869691 corl-3.16.2/corl/glues/common/unit_vector_glue.py
+-rw-r--r--   0        0        0        0 2024-04-12 13:43:47.849691 corl-3.16.2/corl/glues/controller_wrappers/__init__.py
+-rw-r--r--   0        0        0     6122 2024-04-12 13:43:47.849691 corl-3.16.2/corl/glues/controller_wrappers/delta_controller.py
+-rw-r--r--   0        0        0     8849 2024-04-12 13:43:47.849691 corl-3.16.2/corl/glues/controller_wrappers/obs_relative_delta_controller.py
+-rw-r--r--   0        0        0     5443 2024-04-12 13:43:47.849691 corl-3.16.2/corl/glues/controller_wrappers/obs_relative_delta_controller_dict.py
+-rw-r--r--   0        0        0      493 2024-04-12 13:43:47.929691 corl-3.16.2/corl/libraries/__init__.py
+-rw-r--r--   0        0        0     1814 2024-04-12 13:43:47.919691 corl-3.16.2/corl/libraries/algorithm_helper.py
+-rw-r--r--   0        0        0     1143 2024-04-12 13:43:47.929691 corl-3.16.2/corl/libraries/cleanup.py
+-rw-r--r--   0        0        0     1067 2024-04-12 13:43:47.959691 corl-3.16.2/corl/libraries/collection_utils.py
+-rw-r--r--   0        0        0     5562 2024-04-12 13:43:47.929691 corl-3.16.2/corl/libraries/config_file_watcher.py
+-rw-r--r--   0        0        0     1448 2024-04-12 13:43:47.959691 corl-3.16.2/corl/libraries/context.py
+-rw-r--r--   0        0        0     1376 2024-04-12 13:43:47.989691 corl-3.16.2/corl/libraries/env_common.py
+-rw-r--r--   0        0        0     1601 2024-04-12 13:43:47.999691 corl-3.16.2/corl/libraries/env_func_base.py
+-rw-r--r--   0        0        0    42207 2024-04-12 13:43:47.919691 corl-3.16.2/corl/libraries/env_space_util.py
+-rw-r--r--   0        0        0    12950 2024-04-12 13:43:47.929691 corl-3.16.2/corl/libraries/environment_dict.py
+-rw-r--r--   0        0        0     2103 2024-04-12 13:43:47.989691 corl-3.16.2/corl/libraries/factory.py
+-rw-r--r--   0        0        0      856 2024-04-12 13:43:47.989691 corl-3.16.2/corl/libraries/file_path.py
+-rw-r--r--   0        0        0    14325 2024-04-12 13:43:47.969691 corl-3.16.2/corl/libraries/functor.py
+-rw-r--r--   0        0        0    28645 2024-04-12 13:43:47.949691 corl-3.16.2/corl/libraries/hparam_search_util.py
+-rw-r--r--   0        0        0     2656 2024-04-12 13:43:47.959691 corl-3.16.2/corl/libraries/nan_check.py
+-rw-r--r--   0        0        0    11753 2024-04-12 13:43:47.969691 corl-3.16.2/corl/libraries/normalization.py
+-rw-r--r--   0        0        0     2794 2024-04-12 13:43:47.989691 corl-3.16.2/corl/libraries/observation_extractor.py
+-rw-r--r--   0        0        0     2591 2024-04-12 13:43:47.899691 corl-3.16.2/corl/libraries/observation_util.py
+-rw-r--r--   0        0        0    22854 2024-04-12 13:43:47.939691 corl-3.16.2/corl/libraries/parameters.py
+-rw-r--r--   0        0        0     9276 2024-04-12 13:43:47.979691 corl-3.16.2/corl/libraries/plugin_library.py
+-rw-r--r--   0        0        0    19234 2024-04-12 13:43:47.999691 corl-3.16.2/corl/libraries/property.py
+-rw-r--r--   0        0        0     4346 2024-04-12 13:43:47.959691 corl-3.16.2/corl/libraries/space_transformations.py
+-rw-r--r--   0        0        0     5144 2024-04-12 13:43:47.919691 corl-3.16.2/corl/libraries/state_dict.py
+-rw-r--r--   0        0        0    19395 2024-04-12 13:43:47.989691 corl-3.16.2/corl/libraries/units.py
+-rw-r--r--   0        0        0     3379 2024-04-12 13:43:47.959691 corl-3.16.2/corl/libraries/utils.py
+-rw-r--r--   0        0        0     4248 2024-04-12 13:43:47.989691 corl-3.16.2/corl/libraries/value_function.py
+-rw-r--r--   0        0        0      493 2024-04-12 13:43:47.779692 corl-3.16.2/corl/models/__init__.py
+-rw-r--r--   0        0        0     3921 2024-04-12 13:43:47.779692 corl-3.16.2/corl/models/centralized_critic_model.py
+-rw-r--r--   0        0        0    22496 2024-04-12 13:43:47.779692 corl-3.16.2/corl/models/frame_stacking.py
+-rw-r--r--   0        0        0     7097 2024-04-12 13:43:47.789692 corl-3.16.2/corl/models/torch_frame_stack.py
+-rw-r--r--   0        0        0      493 2024-04-12 13:43:47.669692 corl-3.16.2/corl/parsers/__init__.py
+-rw-r--r--   0        0        0     1657 2024-04-12 13:43:47.669692 corl-3.16.2/corl/parsers/agent_and_platform.py
+-rw-r--r--   0        0        0    18078 2024-04-12 13:43:47.669692 corl-3.16.2/corl/parsers/yaml_loader.py
+-rw-r--r--   0        0        0      493 2024-04-12 13:43:47.879691 corl-3.16.2/corl/parts/__init__.py
+-rw-r--r--   0        0        0     4097 2024-04-12 13:43:47.879691 corl-3.16.2/corl/parts/comms.py
+-rw-r--r--   0        0        0     1903 2024-04-12 13:43:47.879691 corl-3.16.2/corl/parts/memory_store.py
+-rw-r--r--   0        0        0      493 2024-04-12 13:43:47.999691 corl-3.16.2/corl/policies/__init__.py
+-rw-r--r--   0        0        0      662 2024-04-12 13:43:47.999691 corl-3.16.2/corl/policies/base_policy.py
+-rw-r--r--   0        0        0    11506 2024-04-12 13:43:48.009690 corl-3.16.2/corl/policies/custom_policy.py
+-rw-r--r--   0        0        0     2014 2024-04-12 13:43:47.999691 corl-3.16.2/corl/policies/random_action.py
+-rw-r--r--   0        0        0     6986 2024-04-12 13:43:48.009690 corl-3.16.2/corl/policies/scripted_action.py
+-rw-r--r--   0        0        0      493 2024-04-12 13:43:47.889691 corl-3.16.2/corl/rewards/__init__.py
+-rw-r--r--   0        0        0     3869 2024-04-12 13:43:47.889691 corl-3.16.2/corl/rewards/base_measurement_operation.py
+-rw-r--r--   0        0        0        0 2024-04-12 13:43:47.899691 corl-3.16.2/corl/rewards/docking_1d/__init__.py
+-rw-r--r--   0        0        0     3121 2024-04-12 13:43:47.899691 corl-3.16.2/corl/rewards/docking_1d/docking_distance_change_reward.py
+-rw-r--r--   0        0        0     4330 2024-04-12 13:43:47.899691 corl-3.16.2/corl/rewards/docking_1d/docking_reward.py
+-rw-r--r--   0        0        0     7594 2024-04-12 13:43:47.889691 corl-3.16.2/corl/rewards/episode_done.py
+-rw-r--r--   0        0        0     3870 2024-04-12 13:43:47.879691 corl-3.16.2/corl/rewards/exponential_decay_from_target_value.py
+-rw-r--r--   0        0        0     1013 2024-04-12 13:43:47.889691 corl-3.16.2/corl/rewards/gymnasium_reward.py
+-rw-r--r--   0        0        0     1685 2024-04-12 13:43:47.899691 corl-3.16.2/corl/rewards/multi_measurement_operation.py
+-rw-r--r--   0        0        0     2403 2024-04-12 13:43:47.899691 corl-3.16.2/corl/rewards/reward_func_base.py
+-rw-r--r--   0        0        0     1827 2024-04-12 13:43:47.889691 corl-3.16.2/corl/rewards/reward_func_dict_wrapper.py
+-rw-r--r--   0        0        0     1822 2024-04-12 13:43:47.889691 corl-3.16.2/corl/rewards/reward_func_multi_wrapper.py
+-rw-r--r--   0        0        0     1781 2024-04-12 13:43:47.889691 corl-3.16.2/corl/rewards/reward_func_wrapper.py
+-rw-r--r--   0        0        0      493 2024-04-12 13:43:47.599693 corl-3.16.2/corl/simulators/__init__.py
+-rw-r--r--   0        0        0    12963 2024-04-12 13:43:47.599693 corl-3.16.2/corl/simulators/base_parts.py
+-rw-r--r--   0        0        0     5330 2024-04-12 13:43:47.609693 corl-3.16.2/corl/simulators/base_platform.py
+-rw-r--r--   0        0        0     1113 2024-04-12 13:43:47.609693 corl-3.16.2/corl/simulators/base_platform_type.py
+-rw-r--r--   0        0        0     1241 2024-04-12 13:43:47.599693 corl-3.16.2/corl/simulators/base_properties.py
+-rw-r--r--   0        0        0    11254 2024-04-12 13:43:47.599693 corl-3.16.2/corl/simulators/base_simulator.py
+-rw-r--r--   0        0        0     1045 2024-04-12 13:43:47.609693 corl-3.16.2/corl/simulators/base_simulator_state.py
+-rw-r--r--   0        0        0     4108 2024-04-12 13:43:47.609693 corl-3.16.2/corl/simulators/common_platform_utils.py
+-rw-r--r--   0        0        0        0 2024-04-12 13:43:47.619692 corl-3.16.2/corl/simulators/docking_1d/__init__.py
+-rw-r--r--   0        0        0      868 2024-04-12 13:43:47.619692 corl-3.16.2/corl/simulators/docking_1d/available_platforms.py
+-rw-r--r--   0        0        0     2288 2024-04-12 13:43:47.619692 corl-3.16.2/corl/simulators/docking_1d/controllers.py
+-rw-r--r--   0        0        0     9013 2024-04-12 13:43:47.609693 corl-3.16.2/corl/simulators/docking_1d/entities.py
+-rw-r--r--   0        0        0     3273 2024-04-12 13:43:47.619692 corl-3.16.2/corl/simulators/docking_1d/platform.py
+-rw-r--r--   0        0        0     2173 2024-04-12 13:43:47.619692 corl-3.16.2/corl/simulators/docking_1d/properties.py
+-rw-r--r--   0        0        0     2043 2024-04-12 13:43:47.619692 corl-3.16.2/corl/simulators/docking_1d/sensors.py
+-rw-r--r--   0        0        0     4287 2024-04-12 13:43:47.619692 corl-3.16.2/corl/simulators/docking_1d/simulator.py
+-rw-r--r--   0        0        0      493 2024-04-12 13:43:47.659692 corl-3.16.2/corl/simulators/gymnasium/__init__.py
+-rw-r--r--   0        0        0     1299 2024-04-12 13:43:47.659692 corl-3.16.2/corl/simulators/gymnasium/gymnasium_available_platforms.py
+-rw-r--r--   0        0        0     3265 2024-04-12 13:43:47.659692 corl-3.16.2/corl/simulators/gymnasium/gymnasium_controllers.py
+-rw-r--r--   0        0        0     4103 2024-04-12 13:43:47.659692 corl-3.16.2/corl/simulators/gymnasium/gymnasium_sensors.py
+-rw-r--r--   0        0        0    10958 2024-04-12 13:43:47.669692 corl-3.16.2/corl/simulators/gymnasium/gymnasium_simulator.py
+-rw-r--r--   0        0        0      493 2024-04-12 13:43:47.629692 corl-3.16.2/corl/simulators/pong/__init__.py
+-rw-r--r--   0        0        0     1078 2024-04-12 13:43:47.629692 corl-3.16.2/corl/simulators/pong/available_platforms.py
+-rw-r--r--   0        0        0     3443 2024-04-12 13:43:47.639692 corl-3.16.2/corl/simulators/pong/controllers.py
+-rw-r--r--   0        0        0     4481 2024-04-12 13:43:47.629692 corl-3.16.2/corl/simulators/pong/heuristic_paddle_policy.py
+-rw-r--r--   0        0        0     3041 2024-04-12 13:43:47.649692 corl-3.16.2/corl/simulators/pong/paddle_platform.py
+-rw-r--r--   0        0        0     6416 2024-04-12 13:43:47.639692 corl-3.16.2/corl/simulators/pong/play_pickled_episode.py
+-rw-r--r--   0        0        0    11242 2024-04-12 13:43:47.639692 corl-3.16.2/corl/simulators/pong/pong.py
+-rw-r--r--   0        0        0     8057 2024-04-12 13:43:47.629692 corl-3.16.2/corl/simulators/pong/sensors.py
+-rw-r--r--   0        0        0     7609 2024-04-12 13:43:47.629692 corl-3.16.2/corl/simulators/pong/simulator.py
+-rw-r--r--   0        0        0      493 2024-04-12 13:43:47.649692 corl-3.16.2/corl/simulators/six_dof/__init__.py
+-rw-r--r--   0        0        0     1781 2024-04-12 13:43:47.659692 corl-3.16.2/corl/simulators/six_dof/base_six_dof_controllers.py
+-rw-r--r--   0        0        0     3166 2024-04-12 13:43:47.649692 corl-3.16.2/corl/simulators/six_dof/base_six_dof_platform.py
+-rw-r--r--   0        0        0    14750 2024-04-12 13:43:47.649692 corl-3.16.2/corl/simulators/six_dof/base_six_dof_properties.py
+-rw-r--r--   0        0        0      493 2024-04-12 13:43:48.009690 corl-3.16.2/corl/test_utils/__init__.py
+-rw-r--r--   0        0        0     1432 2024-04-12 13:43:48.009690 corl-3.16.2/corl/test_utils/full_training.py
+-rw-r--r--   0        0        0      385 2024-04-12 13:43:48.009690 corl-3.16.2/corl/test_utils/testing_ureg_func.py
+-rw-r--r--   0        0        0     4868 2024-04-12 13:43:47.589693 corl-3.16.2/corl/train_rl.py
+-rw-r--r--   0        0        0        0 2024-04-12 13:43:47.679692 corl-3.16.2/corl/visualization/__init__.py
+-rw-r--r--   0        0        0     5214 2024-04-12 13:43:47.699692 corl-3.16.2/corl/visualization/base_animator.py
+-rw-r--r--   0        0        0     1951 2024-04-12 13:43:47.699692 corl-3.16.2/corl/visualization/docking_animator.py
+-rw-r--r--   0        0        0    31451 2024-04-12 13:43:47.699692 corl-3.16.2/corl/visualization/episode_artifact_to_tables.py
+-rw-r--r--   0        0        0        0 2024-04-12 13:43:47.749692 corl-3.16.2/corl/visualization/network_explainability/__init__.py
+-rw-r--r--   0        0        0    15341 2024-04-12 13:43:47.769692 corl-3.16.2/corl/visualization/network_explainability/env_policy_transforms.py
+-rw-r--r--   0        0        0    32525 2024-04-12 13:43:47.759692 corl-3.16.2/corl/visualization/network_explainability/network_explainability.py
+-rw-r--r--   0        0        0     4470 2024-04-12 13:43:47.749692 corl-3.16.2/corl/visualization/network_explainability/network_explainability_plotter.py
+-rw-r--r--   0        0        0     3264 2024-04-12 13:43:47.699692 corl-3.16.2/corl/visualization/platform_plotting_deserializer.py
+-rw-r--r--   0        0        0    21482 2024-04-12 13:43:47.679692 corl-3.16.2/corl/visualization/plotly_animator.py
+-rw-r--r--   0        0        0     2094 2024-04-12 13:43:47.679692 corl-3.16.2/corl/visualization/pong_animator.py
+-rw-r--r--   0        0        0        0 2024-04-12 13:43:47.709692 corl-3.16.2/corl/visualization/streamlit_app/__init__.py
+-rw-r--r--   0        0        0    10408 2024-04-12 13:43:47.719692 corl-3.16.2/corl/visualization/streamlit_app/default_layout.py
+-rw-r--r--   0        0        0    14390 2024-04-12 13:43:47.709692 corl-3.16.2/corl/visualization/streamlit_app/eval_while_train_layout.py
+-rw-r--r--   0        0        0     3059 2024-04-12 13:43:47.749692 corl-3.16.2/corl/visualization/streamlit_app/pages/02_evaluation_from_training.py
+-rw-r--r--   0        0        0     2643 2024-04-12 13:43:47.749692 corl-3.16.2/corl/visualization/streamlit_app/pages/03_corl_evaluation.py
+-rw-r--r--   0        0        0     2402 2024-04-12 13:43:47.749692 corl-3.16.2/corl/visualization/streamlit_app/pages/04_policy_network_viz.py
+-rw-r--r--   0        0        0        0 2024-04-12 13:43:47.749692 corl-3.16.2/corl/visualization/streamlit_app/pages/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 13:43:47.739692 corl-3.16.2/corl/visualization/streamlit_app/sections/__init__.py
+-rw-r--r--   0        0        0    31764 2024-04-12 13:43:47.739692 corl-3.16.2/corl/visualization/streamlit_app/sections/agent_steps.py
+-rw-r--r--   0        0        0     4886 2024-04-12 13:43:47.729692 corl-3.16.2/corl/visualization/streamlit_app/sections/platform_and_agent_dones.py
+-rw-r--r--   0        0        0     6058 2024-04-12 13:43:47.749692 corl-3.16.2/corl/visualization/streamlit_app/sections/trajectory_animation.py
+-rw-r--r--   0        0        0     6757 2024-04-12 13:43:47.739692 corl-3.16.2/corl/visualization/streamlit_app/sections/units_conversion.py
+-rw-r--r--   0        0        0     3011 2024-04-12 13:43:47.709692 corl-3.16.2/corl/visualization/streamlit_app/streamlit_app.py
+-rw-r--r--   0        0        0    20457 2024-04-12 13:43:47.719692 corl-3.16.2/corl/visualization/streamlit_app/utils.py
+-rw-r--r--   0        0        0     7961 2024-04-12 13:43:47.169695 corl-3.16.2/pyproject.toml
+-rw-r--r--   0        0        0      296 2024-04-12 13:43:47.579693 corl-3.16.2/scripts/build.py
+-rw-r--r--   0        0        0     6628 1970-01-01 00:00:00.000000 corl-3.16.2/PKG-INFO
```

### Comparing `corl-3.14.13/LICENSE.md` & `corl-3.16.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/README.md` & `corl-3.16.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 
 #### 1.3.3.1. Case Number
 
 |    Date    |     Release Number     | Description      |
 | :--------: | :--------------------: | :--------------: |
 | 2022-05-20 |     AFRL-2022-2455     | Initial release  |
 | 2023-03-02 | APRS-RYZ-2023-01-00006 | Second release   |
-| 2024-21-03 | AFRL-2024-1562         | Thirst release   |
+| 2024-21-03 | AFRL-2024-1562         | Third release   |
 
 #### 1.3.3.2. Designation Indicator
 
 - Controlled by: Air Force Research Laboratory (AFRL)
 - Controlled by: AFRL Autonomy Capability Team (ACT3)
 
 #### 1.3.3.3. Points of Contact
```

### Comparing `corl-3.14.13/corl/agents/base_agent.py` & `corl-3.16.2/corl/agents/base_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 Base Agent Class
 """
+
 from __future__ import annotations
 
 import abc
 import collections
 import copy
 import fractions
 import typing
@@ -675,17 +676,19 @@
 
     @cached_property
     def normalized_observation_space(self) -> gymnasium.spaces.Space:
         """
         Returns agents normalized observation space
         """
         normalized_obs_space = self._create_space(
-            space_getter=lambda glue_obj: glue_obj.normalized_observation_space
-            if glue_obj.config.training_export_behavior == TrainingExportBehavior.INCLUDE
-            else None
+            space_getter=lambda glue_obj: (
+                glue_obj.normalized_observation_space
+                if glue_obj.config.training_export_behavior == TrainingExportBehavior.INCLUDE
+                else None
+            )
         )
 
         self._obs_space_transformation = self.__create_obs_space_transformation(normalized_obs_space)
         if self._obs_space_transformation:
             return self._obs_space_transformation.output_space
         return normalized_obs_space
```

### Comparing `corl-3.14.13/corl/agents/non_trainable/random_action.py` & `corl-3.16.2/corl/agents/non_trainable/random_action.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/agents/simple_multi_platform_agent.py` & `corl-3.16.2/corl/agents/simple_multi_platform_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 SimpleMultiPlatform Agent Class
 """
+
 import collections
 import typing
 from functools import cached_property
 from graphlib import TopologicalSorter
 
 import gymnasium
 from ray.rllib.utils.spaces.repeated import Repeated
@@ -353,17 +354,19 @@
 
     @cached_property
     def normalized_observation_space(self):
         """
         Returns agents normalized observation space
         """
         tmp = self._create_space(
-            space_getter=lambda glue_obj: glue_obj.normalized_observation_space
-            if glue_obj.config.training_export_behavior == TrainingExportBehavior.INCLUDE
-            else None
+            space_getter=lambda glue_obj: (
+                glue_obj.normalized_observation_space
+                if glue_obj.config.training_export_behavior == TrainingExportBehavior.INCLUDE
+                else None
+            )
         )
         tmp = gymnasium.spaces.Dict(
             {platform_name: Repeated(platform_space, max_len=1) for platform_name, platform_space in tmp.spaces.items()}
         )
         if self.config.policy_observation_transformation:
             self._obs_space_transformation = self.config.policy_observation_transformation.transformation(
                 tmp, self.config.policy_observation_transformation.config
```

### Comparing `corl-3.14.13/corl/config/policy/ppo/default_config.yml` & `corl-3.16.2/corl/evaluation/launchers/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# ---------------------------------------------------------------------------
-#
-#
-# Air Force Research Laboratory (AFRL) Autonomous Capabilities Team (ACT3)
-# Reinforcement Learning (RL) Core.
-#
-# This is a US Government Work not subject to copyright protection in the US.
-#
-# The use, dissemination or disclosure of data in this file is subject to
-# limitation or restriction. See accompanying README and LICENSE for details.
-# ---------------------------------------------------------------------------
-config: {}
+"""
+---------------------------------------------------------------------------
+Air Force Research Laboratory (AFRL) Autonomous Capabilities Team (ACT3)
+Reinforcement Learning (RL) Core.
+
+This is a US Government Work not subject to copyright protection in the US.
+
+The use, dissemination or disclosure of data in this file is subject to
+limitation or restriction. See accompanying README and LICENSE for details.
+---------------------------------------------------------------------------
+Collection of methods to perform evaluation
+"""
```

### Comparing `corl-3.14.13/corl/config/policy/random_action.yml` & `corl-3.16.2/corl/config/tasks/pong/policies/sac_config.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # ---------------------------------------------------------------------------
-#
-#
 # Air Force Research Laboratory (AFRL) Autonomous Capabilities Team (ACT3)
 # Reinforcement Learning (RL) Core.
 #
 # This is a US Government Work not subject to copyright protection in the US.
 #
 # The use, dissemination or disclosure of data in this file is subject to
 # limitation or restriction. See accompanying README and LICENSE for details.
 # ---------------------------------------------------------------------------
-{
-  "policy_class": corl.policies.random_action.RandomActionPolicy,
-  "train": False
+config: {
+  "rollout_fragment_length": 1,
+  "batch_mode": "truncate_episodes",
 }
```

### Comparing `corl-3.14.13/corl/config/policy/scripted_action.yml` & `corl-3.16.2/corl/config/policy/scripted_action.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 # ---------------------------------------------------------------------------
-#
-#
 # Air Force Research Laboratory (AFRL) Autonomous Capabilities Team (ACT3)
 # Reinforcement Learning (RL) Core.
 #
 # This is a US Government Work not subject to copyright protection in the US.
 #
 # The use, dissemination or disclosure of data in this file is subject to
 # limitation or restriction. See accompanying README and LICENSE for details.
```

### Comparing `corl-3.14.13/corl/config/streamlit_app/default_streamlit_config.yml` & `corl-3.16.2/corl/config/streamlit_app/default_streamlit_config.yml`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/config/streamlit_app/docking1d_streamlit_config.yml` & `corl-3.16.2/corl/config/streamlit_app/docking1d_streamlit_config.yml`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/config/streamlit_app/pong_streamlit_config.yml` & `corl-3.16.2/corl/config/streamlit_app/pong_streamlit_config.yml`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/config/tasks/docking_1d/agents/docking1d_agent.yml` & `corl-3.16.2/corl/config/tasks/docking_1d/agents/docking1d_agent.yml`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/config/tasks/docking_1d/environments/docking1d_env.yml` & `corl-3.16.2/corl/config/tasks/docking_1d/environments/docking1d_env.yml`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/config/tasks/docking_1d/evaluation/launch/eval_1d_docking.yml` & `corl-3.16.2/corl/config/tasks/docking_1d/evaluation/launch/eval_1d_docking.yml`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/config/tasks/docking_1d/evaluation/launch/storage_acedt_1d_docking.yml` & `corl-3.16.2/corl/config/tasks/docking_1d/evaluation/launch/storage_acedt_1d_docking.yml`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/config/tasks/docking_1d/evaluation/metrics/1d_docking.yml` & `corl-3.16.2/corl/config/tasks/docking_1d/evaluation/metrics/1d_docking.yml`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/config/tasks/docking_1d/ray_config.yml` & `corl-3.16.2/corl/config/tasks/docking_1d/ray_config.yml`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/config/tasks/docking_1d/rllib_config.yml` & `corl-3.16.2/corl/config/tasks/docking_1d/rllib_config.yml`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/config/tasks/docking_1d/tasks/docking1d_task.yml` & `corl-3.16.2/corl/config/tasks/docking_1d/tasks/docking1d_task.yml`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/config/tasks/docking_1d/tune_config.yml` & `corl-3.16.2/corl/config/tasks/docking_1d/tune_config.yml`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/config/tasks/gymnasium/agents/gymnasium_agent.yml` & `corl-3.16.2/corl/config/tasks/gymnasium/agents/gymnasium_agent.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 # ---------------------------------------------------------------------------
-#
-#
 # Air Force Research Laboratory (AFRL) Autonomous Capabilities Team (ACT3)
 # Reinforcement Learning (RL) Core.
 #
 # This is a US Government Work not subject to copyright protection in the US.
 #
 # The use, dissemination or disclosure of data in this file is subject to
 # limitation or restriction. See accompanying README and LICENSE for details.
```

### Comparing `corl-3.14.13/corl/config/tasks/gymnasium/agents/gymnasium_agent_dict_wrapper.yml` & `corl-3.16.2/corl/config/tasks/gymnasium/agents/gymnasium_agent_dict_wrapper.yml`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/config/tasks/gymnasium/agents/gymnasium_agent_noop.yml` & `corl-3.16.2/corl/config/tasks/gymnasium/agents/gymnasium_agent_noop.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 # ---------------------------------------------------------------------------
-#
-#
 # Air Force Research Laboratory (AFRL) Autonomous Capabilities Team (ACT3)
 # Reinforcement Learning (RL) Core.
 #
 # This is a US Government Work not subject to copyright protection in the US.
 #
 # The use, dissemination or disclosure of data in this file is subject to
 # limitation or restriction. See accompanying README and LICENSE for details.
```

### Comparing `corl-3.14.13/corl/config/tasks/gymnasium/agents/gymnasium_agent_noop_ctrl.yml` & `corl-3.16.2/corl/config/tasks/gymnasium/agents/gymnasium_agent_noop_ctrl.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 # ---------------------------------------------------------------------------
-#
-#
 # Air Force Research Laboratory (AFRL) Autonomous Capabilities Team (ACT3)
 # Reinforcement Learning (RL) Core.
 #
 # This is a US Government Work not subject to copyright protection in the US.
 #
 # The use, dissemination or disclosure of data in this file is subject to
 # limitation or restriction. See accompanying README and LICENSE for details.
```

### Comparing `corl-3.14.13/corl/config/tasks/gymnasium/agents/gymnasium_agent_repeated.yml` & `corl-3.16.2/corl/config/tasks/gymnasium/agents/gymnasium_agent_repeated.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 # ---------------------------------------------------------------------------
-#
-#
 # Air Force Research Laboratory (AFRL) Autonomous Capabilities Team (ACT3)
 # Reinforcement Learning (RL) Core.
 #
 # This is a US Government Work not subject to copyright protection in the US.
 #
 # The use, dissemination or disclosure of data in this file is subject to
 # limitation or restriction. See accompanying README and LICENSE for details.
```

### Comparing `corl-3.14.13/corl/config/tasks/gymnasium/agents/gymnasium_agent_wrapper.yml` & `corl-3.16.2/corl/config/tasks/gymnasium/agents/gymnasium_agent_wrapper.yml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 # ---------------------------------------------------------------------------
-#
-#
 # Air Force Research Laboratory (AFRL) Autonomous Capabilities Team (ACT3)
 # Reinforcement Learning (RL) Core.
 #
 # This is a US Government Work not subject to copyright protection in the US.
 #
 # The use, dissemination or disclosure of data in this file is subject to
 # limitation or restriction. See accompanying README and LICENSE for details.
```

### Comparing `corl-3.14.13/corl/config/tasks/gymnasium/environments/cartpole_v1.yml` & `corl-3.16.2/corl/config/tasks/gymnasium/environments/cartpole_v1.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 # ---------------------------------------------------------------------------
-#
-#
 # Air Force Research Laboratory (AFRL) Autonomous Capabilities Team (ACT3)
 # Reinforcement Learning (RL) Core.
 #
 # This is a US Government Work not subject to copyright protection in the US.
 #
 # The use, dissemination or disclosure of data in this file is subject to
 # limitation or restriction. See accompanying README and LICENSE for details.
```

### Comparing `corl-3.14.13/corl/config/tasks/gymnasium/environments/cartpole_v1_with_time.yml` & `corl-3.16.2/corl/config/tasks/gymnasium/environments/cartpole_v1_with_time.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 # ---------------------------------------------------------------------------
-#
-#
 # Air Force Research Laboratory (AFRL) Autonomous Capabilities Team (ACT3)
 # Reinforcement Learning (RL) Core.
 #
 # This is a US Government Work not subject to copyright protection in the US.
 #
 # The use, dissemination or disclosure of data in this file is subject to
 # limitation or restriction. See accompanying README and LICENSE for details.
```

### Comparing `corl-3.14.13/corl/config/tasks/gymnasium/environments/pendulum_v1.yml` & `corl-3.16.2/corl/config/tasks/gymnasium/environments/pendulum_v1.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 # ---------------------------------------------------------------------------
-#
-#
 # Air Force Research Laboratory (AFRL) Autonomous Capabilities Team (ACT3)
 # Reinforcement Learning (RL) Core.
 #
 # This is a US Government Work not subject to copyright protection in the US.
 #
 # The use, dissemination or disclosure of data in this file is subject to
 # limitation or restriction. See accompanying README and LICENSE for details.
```

### Comparing `corl-3.14.13/corl/config/tasks/gymnasium/experiments/cartpole_v1_noop.yml` & `corl-3.16.2/corl/config/tasks/gymnasium/experiments/cartpole_v1_noop.yml`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/config/tasks/gymnasium/experiments/cartpole_v1_noop_ctrl.yml` & `corl-3.16.2/corl/config/tasks/gymnasium/experiments/cartpole_v1_noop_ctrl.yml`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/config/tasks/gymnasium/experiments/cartpole_v1_random.yml` & `corl-3.16.2/corl/config/tasks/gymnasium/experiments/cartpole_v1_random.yml`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/config/tasks/gymnasium/experiments/cartpole_v1_scripted.yml` & `corl-3.16.2/corl/config/tasks/gymnasium/experiments/cartpole_v1_scripted.yml`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/config/tasks/gymnasium/platforms/gymnasium_platform.yml` & `corl-3.16.2/corl/config/tasks/gymnasium/platforms/gymnasium_platform_inclusive_parts.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 # ---------------------------------------------------------------------------
-#
-#
 # Air Force Research Laboratory (AFRL) Autonomous Capabilities Team (ACT3)
 # Reinforcement Learning (RL) Core.
 #
 # This is a US Government Work not subject to copyright protection in the US.
 #
 # The use, dissemination or disclosure of data in this file is subject to
 # limitation or restriction. See accompanying README and LICENSE for details.
 # ---------------------------------------------------------------------------
 {
-  platform_class: "corl.simulators.gymnasium.gymnasium_simulator.GymnasiumPlatform",
+  platform_class: "corl.simulators.gymnasium.gymnasium_simulator.GymnasiumInclusivePartsPlatform",
 }
```

### Comparing `corl-3.14.13/corl/config/tasks/gymnasium/platforms/gymnasium_platform_inclusive_parts.yml` & `corl-3.16.2/corl/evaluation/runners/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-# ---------------------------------------------------------------------------
-#
-#
-# Air Force Research Laboratory (AFRL) Autonomous Capabilities Team (ACT3)
-# Reinforcement Learning (RL) Core.
-#
-# This is a US Government Work not subject to copyright protection in the US.
-#
-# The use, dissemination or disclosure of data in this file is subject to
-# limitation or restriction. See accompanying README and LICENSE for details.
-# ---------------------------------------------------------------------------
-{
-  platform_class: "corl.simulators.gymnasium.gymnasium_simulator.GymnasiumInclusivePartsPlatform",
-}
+"""
+---------------------------------------------------------------------------
+Air Force Research Laboratory (AFRL) Autonomous Capabilities Team (ACT3)
+Reinforcement Learning (RL) Core.
+
+This is a US Government Work not subject to copyright protection in the US.
+
+The use, dissemination or disclosure of data in this file is subject to
+limitation or restriction. See accompanying README and LICENSE for details.
+---------------------------------------------------------------------------
+Collection of methods to perform evaluation
+"""
```

### Comparing `corl-3.14.13/corl/config/tasks/gymnasium/ray_config.yml` & `corl-3.16.2/corl/config/tasks/gymnasium/ray_config.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 # ---------------------------------------------------------------------------
-#
-#
 # Air Force Research Laboratory (AFRL) Autonomous Capabilities Team (ACT3)
 # Reinforcement Learning (RL) Core.
 #
 # This is a US Government Work not subject to copyright protection in the US.
 #
 # The use, dissemination or disclosure of data in this file is subject to
 # limitation or restriction. See accompanying README and LICENSE for details.
```

### Comparing `corl-3.14.13/corl/config/tasks/gymnasium/rllib_config.yml` & `corl-3.16.2/corl/config/tasks/gymnasium/rllib_config.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 # ---------------------------------------------------------------------------
-#
-#
 # Air Force Research Laboratory (AFRL) Autonomous Capabilities Team (ACT3)
 # Reinforcement Learning (RL) Core.
 #
 # This is a US Government Work not subject to copyright protection in the US.
 #
 # The use, dissemination or disclosure of data in this file is subject to
 # limitation or restriction. See accompanying README and LICENSE for details.
```

### Comparing `corl-3.14.13/corl/config/tasks/gymnasium/tasks/cartpole_v1.yml` & `corl-3.16.2/corl/config/tasks/gymnasium/tasks/cartpole_v1_with_time.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 # ---------------------------------------------------------------------------
-#
-#
 # Air Force Research Laboratory (AFRL) Autonomous Capabilities Team (ACT3)
 # Reinforcement Learning (RL) Core.
 #
 # This is a US Government Work not subject to copyright protection in the US.
 #
 # The use, dissemination or disclosure of data in this file is subject to
 # limitation or restriction. See accompanying README and LICENSE for details.
@@ -12,15 +10,15 @@
 
 ####################################################################
 # Override values used by the setup
 ####################################################################
 experiment_class: corl.experiments.rllib_experiment.RllibExperiment
 config:
   rllib_config_updates: &rllib_config_updates
-    # num_workers: 0
+    #num_workers: 0
     # model:
     #   # Custom model built on top of the existing baseline model.
     #   custom_model: "FrameStackingModel"
     #   # Default model config option: currently adds one more layer than
     #   # default for the computing of rates... This is not intended to
     #   # replace the existing
     #   fcnet_hiddens: [256, 256, 256]
@@ -61,10 +59,10 @@
   # Note that items are patched from the update section
   ###################################################################
   rllib_configs:
     default: !merge [!include ../rllib_config.yml, *rllib_config_updates]
     local: !merge [!include ../rllib_config.yml,  *rllib_config_updates]
 
   ray_config: !merge [!include ../ray_config.yml, *ray_config_updates]
-  env_config: !merge [!include ../environments/cartpole_v1.yml, *env_config_updates]
+  env_config: !merge [!include ../environments/cartpole_v1_with_time.yml, *env_config_updates]
   tune_config: !merge [!include ../tune_config.yml, *tune_config_updates]
```

### Comparing `corl-3.14.13/corl/config/tasks/gymnasium/tasks/cartpole_v1_benchmark.yml` & `corl-3.16.2/corl/config/tasks/gymnasium/tasks/cartpole_v1_benchmark.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 # ---------------------------------------------------------------------------
-#
-#
 # Air Force Research Laboratory (AFRL) Autonomous Capabilities Team (ACT3)
 # Reinforcement Learning (RL) Core.
 #
 # This is a US Government Work not subject to copyright protection in the US.
 #
 # The use, dissemination or disclosure of data in this file is subject to
 # limitation or restriction. See accompanying README and LICENSE for details.
```

### Comparing `corl-3.14.13/corl/config/tasks/gymnasium/tasks/cartpole_v1_with_time.yml` & `corl-3.16.2/corl/config/tasks/gymnasium/tasks/cartpole_v1.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 # ---------------------------------------------------------------------------
-#
-#
 # Air Force Research Laboratory (AFRL) Autonomous Capabilities Team (ACT3)
 # Reinforcement Learning (RL) Core.
 #
 # This is a US Government Work not subject to copyright protection in the US.
 #
 # The use, dissemination or disclosure of data in this file is subject to
 # limitation or restriction. See accompanying README and LICENSE for details.
@@ -12,15 +10,15 @@
 
 ####################################################################
 # Override values used by the setup
 ####################################################################
 experiment_class: corl.experiments.rllib_experiment.RllibExperiment
 config:
   rllib_config_updates: &rllib_config_updates
-    #num_workers: 0
+    # num_workers: 0
     # model:
     #   # Custom model built on top of the existing baseline model.
     #   custom_model: "FrameStackingModel"
     #   # Default model config option: currently adds one more layer than
     #   # default for the computing of rates... This is not intended to
     #   # replace the existing
     #   fcnet_hiddens: [256, 256, 256]
@@ -61,10 +59,10 @@
   # Note that items are patched from the update section
   ###################################################################
   rllib_configs:
     default: !merge [!include ../rllib_config.yml, *rllib_config_updates]
     local: !merge [!include ../rllib_config.yml,  *rllib_config_updates]
 
   ray_config: !merge [!include ../ray_config.yml, *ray_config_updates]
-  env_config: !merge [!include ../environments/cartpole_v1_with_time.yml, *env_config_updates]
+  env_config: !merge [!include ../environments/cartpole_v1.yml, *env_config_updates]
   tune_config: !merge [!include ../tune_config.yml, *tune_config_updates]
```

### Comparing `corl-3.14.13/corl/config/tasks/gymnasium/tasks/pendulum_v1.yml` & `corl-3.16.2/corl/config/tasks/gymnasium/tasks/pendulum_v1.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 # ---------------------------------------------------------------------------
-#
-#
 # Air Force Research Laboratory (AFRL) Autonomous Capabilities Team (ACT3)
 # Reinforcement Learning (RL) Core.
 #
 # This is a US Government Work not subject to copyright protection in the US.
 #
 # The use, dissemination or disclosure of data in this file is subject to
 # limitation or restriction. See accompanying README and LICENSE for details.
```

### Comparing `corl-3.14.13/corl/config/tasks/gymnasium/tune_config.yml` & `corl-3.16.2/corl/config/tasks/gymnasium/tune_config.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 # ---------------------------------------------------------------------------
-#
-#
 # Air Force Research Laboratory (AFRL) Autonomous Capabilities Team (ACT3)
 # Reinforcement Learning (RL) Core.
 #
 # This is a US Government Work not subject to copyright protection in the US.
 #
 # The use, dissemination or disclosure of data in this file is subject to
 # limitation or restriction. See accompanying README and LICENSE for details.
```

### Comparing `corl-3.14.13/corl/config/tasks/pong/agents/commander_paddle_agent.yml` & `corl-3.16.2/corl/config/tasks/pong/agents/commander_paddle_agent.yml`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/config/tasks/pong/agents/dummy_noop.yml` & `corl-3.16.2/corl/config/tasks/pong/agents/dummy_noop.yml`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/config/tasks/pong/agents/paddle_agent-scripted-noop.yml` & `corl-3.16.2/corl/config/tasks/pong/agents/paddle_agent-scripted-noop.yml`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/config/tasks/pong/agents/paddle_agent-scripted-random_action.yml` & `corl-3.16.2/corl/config/tasks/pong/agents/paddle_agent-scripted-random_action.yml`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/config/tasks/pong/agents/paddle_agent.yml` & `corl-3.16.2/corl/config/tasks/pong/agents/paddle_agent.yml`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/config/tasks/pong/agents/paddle_agent_flat_actions.yml` & `corl-3.16.2/corl/config/tasks/pong/agents/paddle_agent_flat_actions.yml`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/config/tasks/pong/commander_rllib_config.yml` & `corl-3.16.2/corl/config/tasks/pong/commander_rllib_config.yml`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/config/tasks/pong/environments/commander_pong_env.yml` & `corl-3.16.2/corl/config/tasks/pong/environments/commander_pong_env.yml`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/config/tasks/pong/environments/pong_env.yml` & `corl-3.16.2/corl/config/tasks/pong/environments/pong_env.yml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # This config defines the environment for the training loop. This includes the Simulator entity, type of platform, path
 # to the directory in which components (Sensors, Controllers, and Simulators) are registered with the PluginLibrary.
 {
+  "sanity_check_obs": 1,
   "horizon": 2500,
   "simulator": {
     "type": "PongSimulator",
     "config": {},
   },
   "plugin_paths": ["corl"],
   "episode_parameter_provider": {
```

### Comparing `corl-3.14.13/corl/config/tasks/pong/evaluation/launch/base_pong_evaluate.yml` & `corl-3.16.2/corl/config/tasks/pong/evaluation/launch/base_pong_evaluate.yml`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/config/tasks/pong/evaluation/launch/commander_pong_evaluate.yml` & `corl-3.16.2/corl/config/tasks/pong/evaluation/launch/commander_pong_evaluate.yml`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/config/tasks/pong/experiments/pong-both_scripted-random_action.yml` & `corl-3.16.2/corl/config/tasks/pong/experiments/pong-both_scripted-random_action.yml`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/config/tasks/pong/experiments/pong-one_scripted-noop.yml` & `corl-3.16.2/corl/config/tasks/pong/experiments/pong-one_scripted-noop.yml`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/config/tasks/pong/experiments/pong-one_scripted-random_action.yml` & `corl-3.16.2/corl/config/tasks/pong/experiments/pong-one_scripted-random_action.yml`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/config/tasks/pong/experiments/pong.yml` & `corl-3.16.2/corl/config/tasks/pong/experiments/pong_alt.yml`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333333333333334%*

 * *Differences: {"'config'": "'config/tasks/pong/tasks/pong_task_ppo_alt.yml'"}*

```diff
@@ -13,15 +13,15 @@
             "name": "paddle1_ctrl",
             "platforms": [
                 "paddle1"
             ],
             "policy": "config/tasks/pong/policies/ppo_config.yml"
         }
     ],
-    "config": "config/tasks/pong/tasks/pong_task_ppo.yml",
+    "config": "config/tasks/pong/tasks/pong_task_ppo_alt.yml",
     "platform_config": [
         {
             "config": "config/tasks/pong/platforms/paddle.yml",
             "name": "paddle0"
         },
         {
             "config": "config/tasks/pong/platforms/paddle.yml",
```

### Comparing `corl-3.14.13/corl/config/tasks/pong/experiments/pong_alt.yml` & `corl-3.16.2/corl/config/tasks/pong/experiments/pong_group.yml`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333333333333334%*

 * *Differences: {"'config'": "'config/tasks/pong/tasks/pong_task_group.yml'"}*

```diff
@@ -13,15 +13,15 @@
             "name": "paddle1_ctrl",
             "platforms": [
                 "paddle1"
             ],
             "policy": "config/tasks/pong/policies/ppo_config.yml"
         }
     ],
-    "config": "config/tasks/pong/tasks/pong_task_ppo_alt.yml",
+    "config": "config/tasks/pong/tasks/pong_task_group.yml",
     "platform_config": [
         {
             "config": "config/tasks/pong/platforms/paddle.yml",
             "name": "paddle0"
         },
         {
             "config": "config/tasks/pong/platforms/paddle.yml",
```

### Comparing `corl-3.14.13/corl/config/tasks/pong/experiments/pong_commander.yml` & `corl-3.16.2/corl/config/tasks/pong/experiments/pong_commander.yml`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/config/tasks/pong/experiments/pong_group.yml` & `corl-3.16.2/corl/config/tasks/pong/experiments/pong.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 00000000: 7b0a 2020 2263 6f6e 6669 6722 3a20 2263  {.  "config": "c
 00000010: 6f6e 6669 672f 7461 736b 732f 706f 6e67  onfig/tasks/pong
 00000020: 2f74 6173 6b73 2f70 6f6e 675f 7461 736b  /tasks/pong_task
-00000030: 5f67 726f 7570 2e79 6d6c 222c 0a20 2022  _group.yml",.  "
-00000040: 706c 6174 666f 726d 5f63 6f6e 6669 6722  platform_config"
-00000050: 3a20 5b0a 2020 2020 7b0a 2020 2020 2020  : [.    {.      
-00000060: 226e 616d 6522 3a20 2270 6164 646c 6530  "name": "paddle0
-00000070: 222c 0a20 2020 2020 2022 636f 6e66 6967  ",.      "config
-00000080: 223a 2022 636f 6e66 6967 2f74 6173 6b73  ": "config/tasks
-00000090: 2f70 6f6e 672f 706c 6174 666f 726d 732f  /pong/platforms/
-000000a0: 7061 6464 6c65 2e79 6d6c 220a 2020 2020  paddle.yml".    
-000000b0: 7d2c 0a20 2020 207b 0a20 2020 2020 2022  },.    {.      "
-000000c0: 6e61 6d65 223a 2022 7061 6464 6c65 3122  name": "paddle1"
-000000d0: 2c0a 2020 2020 2020 2263 6f6e 6669 6722  ,.      "config"
-000000e0: 3a20 2263 6f6e 6669 672f 7461 736b 732f  : "config/tasks/
-000000f0: 706f 6e67 2f70 6c61 7466 6f72 6d73 2f70  pong/platforms/p
-00000100: 6164 646c 652e 796d 6c22 0a20 2020 207d  addle.yml".    }
-00000110: 0a20 205d 2c0a 2020 2261 6765 6e74 5f63  .  ],.  "agent_c
-00000120: 6f6e 6669 6722 3a20 5b0a 2020 2020 7b0a  onfig": [.    {.
-00000130: 2020 2020 2020 226e 616d 6522 3a20 2270        "name": "p
-00000140: 6164 646c 6530 5f63 7472 6c22 2c0a 2020  addle0_ctrl",.  
-00000150: 2020 2020 2270 6c61 7466 6f72 6d73 223a      "platforms":
-00000160: 205b 2270 6164 646c 6530 225d 2c0a 2020   ["paddle0"],.  
-00000170: 2020 2020 2263 6f6e 6669 6722 3a20 2263      "config": "c
-00000180: 6f6e 6669 672f 7461 736b 732f 706f 6e67  onfig/tasks/pong
-00000190: 2f61 6765 6e74 732f 7061 6464 6c65 5f61  /agents/paddle_a
-000001a0: 6765 6e74 2e79 6d6c 222c 0a20 2020 2020  gent.yml",.     
-000001b0: 2022 706f 6c69 6379 223a 2022 636f 6e66   "policy": "conf
-000001c0: 6967 2f74 6173 6b73 2f70 6f6e 672f 706f  ig/tasks/pong/po
-000001d0: 6c69 6369 6573 2f70 706f 5f63 6f6e 6669  licies/ppo_confi
-000001e0: 672e 796d 6c22 0a20 2020 207d 2c0a 2020  g.yml".    },.  
-000001f0: 2020 7b0a 2020 2020 2020 226e 616d 6522    {.      "name"
-00000200: 3a20 2270 6164 646c 6531 5f63 7472 6c22  : "paddle1_ctrl"
-00000210: 2c0a 2020 2020 2020 2270 6c61 7466 6f72  ,.      "platfor
+00000030: 5f70 706f 2e79 6d6c 222c 0a20 2022 706c  _ppo.yml",.  "pl
+00000040: 6174 666f 726d 5f63 6f6e 6669 6722 3a0a  atform_config":.
+00000050: 2020 2020 5b0a 2020 2020 2020 7b20 226e      [.      { "n
+00000060: 616d 6522 3a20 2270 6164 646c 6530 222c  ame": "paddle0",
+00000070: 2022 636f 6e66 6967 223a 2022 636f 6e66   "config": "conf
+00000080: 6967 2f74 6173 6b73 2f70 6f6e 672f 706c  ig/tasks/pong/pl
+00000090: 6174 666f 726d 732f 7061 6464 6c65 2e79  atforms/paddle.y
+000000a0: 6d6c 2220 7d2c 0a20 2020 2020 207b 2022  ml" },.      { "
+000000b0: 6e61 6d65 223a 2022 7061 6464 6c65 3122  name": "paddle1"
+000000c0: 2c20 2263 6f6e 6669 6722 3a20 2263 6f6e  , "config": "con
+000000d0: 6669 672f 7461 736b 732f 706f 6e67 2f70  fig/tasks/pong/p
+000000e0: 6c61 7466 6f72 6d73 2f70 6164 646c 652e  latforms/paddle.
+000000f0: 796d 6c22 207d 2c0a 2020 2020 5d2c 0a20  yml" },.    ],. 
+00000100: 2022 6167 656e 745f 636f 6e66 6967 223a   "agent_config":
+00000110: 0a20 2020 205b 0a20 2020 2020 207b 0a20  .    [.      {. 
+00000120: 2020 2020 2020 2022 6e61 6d65 223a 2022         "name": "
+00000130: 7061 6464 6c65 305f 6374 726c 222c 0a20  paddle0_ctrl",. 
+00000140: 2020 2020 2020 2022 706c 6174 666f 726d         "platform
+00000150: 7322 3a20 5b22 7061 6464 6c65 3022 5d2c  s": ["paddle0"],
+00000160: 0a20 2020 2020 2020 2022 636f 6e66 6967  .        "config
+00000170: 223a 2022 636f 6e66 6967 2f74 6173 6b73  ": "config/tasks
+00000180: 2f70 6f6e 672f 6167 656e 7473 2f70 6164  /pong/agents/pad
+00000190: 646c 655f 6167 656e 742e 796d 6c22 2c0a  dle_agent.yml",.
+000001a0: 2020 2020 2020 2020 2270 6f6c 6963 7922          "policy"
+000001b0: 3a20 2263 6f6e 6669 672f 7461 736b 732f  : "config/tasks/
+000001c0: 706f 6e67 2f70 6f6c 6963 6965 732f 7070  pong/policies/pp
+000001d0: 6f5f 636f 6e66 6967 2e79 6d6c 222c 0a20  o_config.yml",. 
+000001e0: 2020 2020 207d 2c0a 2020 2020 2020 7b0a       },.      {.
+000001f0: 2020 2020 2020 2020 226e 616d 6522 3a20          "name": 
+00000200: 2270 6164 646c 6531 5f63 7472 6c22 2c0a  "paddle1_ctrl",.
+00000210: 2020 2020 2020 2020 2270 6c61 7466 6f72          "platfor
 00000220: 6d73 223a 205b 2270 6164 646c 6531 225d  ms": ["paddle1"]
-00000230: 2c0a 2020 2020 2020 2263 6f6e 6669 6722  ,.      "config"
-00000240: 3a20 2263 6f6e 6669 672f 7461 736b 732f  : "config/tasks/
-00000250: 706f 6e67 2f61 6765 6e74 732f 7061 6464  pong/agents/padd
-00000260: 6c65 5f61 6765 6e74 2e79 6d6c 222c 0a20  le_agent.yml",. 
-00000270: 2020 2020 2022 706f 6c69 6379 223a 2022       "policy": "
-00000280: 636f 6e66 6967 2f74 6173 6b73 2f70 6f6e  config/tasks/pon
-00000290: 672f 706f 6c69 6369 6573 2f70 706f 5f63  g/policies/ppo_c
-000002a0: 6f6e 6669 672e 796d 6c22 0a20 2020 207d  onfig.yml".    }
-000002b0: 0a20 205d 0a7d                           .  ].}
+00000230: 2c0a 2020 2020 2020 2020 2263 6f6e 6669  ,.        "confi
+00000240: 6722 3a20 2263 6f6e 6669 672f 7461 736b  g": "config/task
+00000250: 732f 706f 6e67 2f61 6765 6e74 732f 7061  s/pong/agents/pa
+00000260: 6464 6c65 5f61 6765 6e74 2e79 6d6c 222c  ddle_agent.yml",
+00000270: 0a20 2020 2020 2020 2022 706f 6c69 6379  .        "policy
+00000280: 223a 2022 636f 6e66 6967 2f74 6173 6b73  ": "config/tasks
+00000290: 2f70 6f6e 672f 706f 6c69 6369 6573 2f70  /pong/policies/p
+000002a0: 706f 5f63 6f6e 6669 672e 796d 6c22 2c0a  po_config.yml",.
+000002b0: 2020 2020 2020 7d2c 0a20 2020 205d 2c0a        },.    ],.
+000002c0: 7d0a                                     }.
```

### Comparing `corl-3.14.13/corl/config/tasks/pong/experiments/pong_sac.yml` & `corl-3.16.2/corl/config/tasks/pong/experiments/pong_sac.yml`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/config/tasks/pong/policies/ppo_config.yml` & `corl-3.16.2/corl/config/tasks/pong/policies/ppo_config_central_critic.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # ---------------------------------------------------------------------------
-#
-#
 # Air Force Research Laboratory (AFRL) Autonomous Capabilities Team (ACT3)
 # Reinforcement Learning (RL) Core.
 #
 # This is a US Government Work not subject to copyright protection in the US.
 #
 # The use, dissemination or disclosure of data in this file is subject to
 # limitation or restriction. See accompanying README and LICENSE for details.
 # ---------------------------------------------------------------------------
 config: {
   "rollout_fragment_length": 500,
   "train_batch_size": 5000,
   "sgd_minibatch_size": 150,
   "num_sgd_iter": 30,
-  "batch_mode": "complete_episodes"
+  "batch_mode": "complete_episodes",
+  "model": {
+    custom_model: TorchCentralizedCriticModel
+  }
 }
```

### Comparing `corl-3.14.13/corl/config/tasks/pong/policies/sac_config.yml` & `corl-3.16.2/corl/config/tasks/pong/policies/ppo_config.yml`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # ---------------------------------------------------------------------------
-#
-#
 # Air Force Research Laboratory (AFRL) Autonomous Capabilities Team (ACT3)
 # Reinforcement Learning (RL) Core.
 #
 # This is a US Government Work not subject to copyright protection in the US.
 #
 # The use, dissemination or disclosure of data in this file is subject to
 # limitation or restriction. See accompanying README and LICENSE for details.
 # ---------------------------------------------------------------------------
 config: {
-  "rollout_fragment_length": 1,
-  "batch_mode": "truncate_episodes",
+  "rollout_fragment_length": 500,
+  "train_batch_size": 5000,
+  "sgd_minibatch_size": 150,
+  "num_sgd_iter": 30,
+  "batch_mode": "complete_episodes",
 }
```

### Comparing `corl-3.14.13/corl/config/tasks/pong/ray_config.yml` & `corl-3.16.2/corl/config/tasks/pong/ray_config.yml`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/config/tasks/pong/rllib_config.yml` & `corl-3.16.2/corl/config/tasks/pong/rllib_config.yml`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/config/tasks/pong/tasks/pong_commander_task_ppo.yml` & `corl-3.16.2/corl/config/tasks/pong/tasks/pong_commander_task_ppo.yml`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/config/tasks/pong/tasks/pong_task_group.yml` & `corl-3.16.2/corl/config/tasks/pong/tasks/pong_task_group.yml`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/config/tasks/pong/tasks/pong_task_ppo-all_scripted.yml` & `corl-3.16.2/corl/config/tasks/pong/tasks/pong_task_ppo-all_scripted.yml`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/config/tasks/pong/tasks/pong_task_ppo.yml` & `corl-3.16.2/corl/config/tasks/pong/tasks/pong_task_ppo.yml`

 * *Files 8% similar despite different names*

```diff
@@ -12,16 +12,18 @@
 # Override values used by the setup
 ####################################################################
 experiment_class: corl.experiments.rllib_experiment.RllibExperiment
 
 config:
   # Example of PBT
   # hparam_search_class: corl.libraries.hparam_search_util.HparamSearchPPO_PBT
+  
   # Example of ASHB
   # hparam_search_class: corl.libraries.hparam_search_util.HparamSearchPPO_AHBS
+  
   policy_mapping:
     functor: corl.experiments.rllib_utils.policy_mapping_functions.SinglePolicy
     config:
       policy_id: "paddle0_ctrl"
 
   rllib_config_updates: &rllib_config_updates
 
@@ -45,11 +47,11 @@
   rllib_configs:
     default: !merge [!include ../rllib_config.yml, *rllib_config_updates]
     local: !merge [!include ../rllib_config.yml,  *rllib_config_updates]
 
   ray_config: !merge [!include ../ray_config.yml, *ray_config_updates]
   env_config: !merge [!include ../environments/pong_env.yml, *env_config_updates]
   tune_config: !merge [!include ../tune_config_ppo.yml, *tune_config_updates]
+
   extra_callbacks: [
     corl.environment.episode_artifact_callbacks.PongEpisodeArtifactLogger,
     corl.environment.custom_env_metrics.CustomPongMetrics]
-
```

### Comparing `corl-3.14.13/corl/config/tasks/pong/tasks/pong_task_ppo_alt.yml` & `corl-3.16.2/corl/config/tasks/pong/tasks/pong_task_ppo_alt.yml`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/config/tasks/pong/tasks/pong_task_sac.yml` & `corl-3.16.2/corl/config/tasks/pong/tasks/pong_task_sac.yml`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/config/tasks/pong/tune_config_ppo.yml` & `corl-3.16.2/corl/config/tasks/pong/tune_config_ppo.yml`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/config/tasks/pong/tune_config_sac.yml` & `corl-3.16.2/corl/config/tasks/pong/tune_config_sac.yml`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/config/tasks/ray_config.yml` & `corl-3.16.2/corl/config/tasks/ray_config.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 # ---------------------------------------------------------------------------
-#
-#
 # Air Force Research Laboratory (AFRL) Autonomous Capabilities Team (ACT3)
 # Reinforcement Learning (RL) Core.
 #
 # This is a US Government Work not subject to copyright protection in the US.
 #
 # The use, dissemination or disclosure of data in this file is subject to
 # limitation or restriction. See accompanying README and LICENSE for details.
```

### Comparing `corl-3.14.13/corl/config/tasks/rllib_config.yml` & `corl-3.16.2/corl/config/tasks/rllib_config.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 # ---------------------------------------------------------------------------
-#
-#
 # Air Force Research Laboratory (AFRL) Autonomous Capabilities Team (ACT3)
 # Reinforcement Learning (RL) Core.
 #
 # This is a US Government Work not subject to copyright protection in the US.
 #
 # The use, dissemination or disclosure of data in this file is subject to
 # limitation or restriction. See accompanying README and LICENSE for details.
```

### Comparing `corl-3.14.13/corl/config/tasks/tune_config.yml` & `corl-3.16.2/corl/config/tasks/tune_config.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 # ---------------------------------------------------------------------------
-#
-#
 # Air Force Research Laboratory (AFRL) Autonomous Capabilities Team (ACT3)
 # Reinforcement Learning (RL) Core.
 #
 # This is a US Government Work not subject to copyright protection in the US.
 #
 # The use, dissemination or disclosure of data in this file is subject to
 # limitation or restriction. See accompanying README and LICENSE for details.
```

### Comparing `corl-3.14.13/corl/dones/docking_1d/dones.py` & `corl-3.16.2/corl/dones/docking_1d/dones.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/dones/done_func_base.py` & `corl-3.16.2/corl/dones/done_func_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,16 +98,15 @@
         self,
         observation: OrderedDict,
         action: OrderedDict,
         next_observation: OrderedDict,
         next_state: BaseSimulatorState,
         observation_space: gymnasium.Space,
         observation_units: OrderedDict,
-    ) -> bool:
-        ...
+    ) -> bool: ...
 
 
 class SharedDoneFuncBaseValidator(BaseModel):
     """
     name : str
         The name of this done condition
     """
@@ -149,9 +148,8 @@
         action: OrderedDict,
         next_observation: OrderedDict,
         next_state: StateDict,
         observation_space: StateDict,
         observation_units: StateDict,
         local_dones: DoneDict,
         local_done_info: OrderedDict,
-    ) -> DoneDict:
-        ...
+    ) -> DoneDict: ...
```

### Comparing `corl-3.14.13/corl/dones/done_func_dict_wrapper.py` & `corl-3.16.2/corl/dones/done_func_dict_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,9 +49,8 @@
         self,
         observation: OrderedDict,
         action: OrderedDict,
         next_observation: OrderedDict,
         next_state: BaseSimulatorState,
         observation_space: gymnasium.Space,
         observation_units: OrderedDict,
-    ) -> bool:
-        ...
+    ) -> bool: ...
```

### Comparing `corl-3.14.13/corl/dones/done_func_multi_wrapper.py` & `corl-3.16.2/corl/dones/done_func_multi_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,9 +49,8 @@
         self,
         observation: OrderedDict,
         action: OrderedDict,
         next_observation: OrderedDict,
         next_state: BaseSimulatorState,
         observation_space: gymnasium.Space,
         observation_units: OrderedDict,
-    ) -> bool:
-        ...
+    ) -> bool: ...
```

### Comparing `corl-3.14.13/corl/dones/done_func_wrapper.py` & `corl-3.16.2/corl/dones/done_func_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,9 +49,8 @@
         self,
         observation: OrderedDict,
         action: OrderedDict,
         next_observation: OrderedDict,
         next_state: BaseSimulatorState,
         observation_space: gymnasium.Space,
         observation_units: OrderedDict,
-    ) -> bool:
-        ...
+    ) -> bool: ...
```

### Comparing `corl-3.14.13/corl/dones/episode_length_done.py` & `corl-3.16.2/corl/dones/episode_length_done.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 from collections import OrderedDict
 
 import gymnasium
 
 from corl.dones.done_func_base import DoneFuncBase, DoneFuncBaseValidator, DoneStatusCodes
 from corl.libraries.units import Quantity
 from corl.simulators.base_simulator import BaseSimulatorState
```

### Comparing `corl-3.14.13/corl/dones/gymnasium_done.py` & `corl-3.16.2/corl/dones/gymnasium_done.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 Done condition for GymnasiumSimulator
 """
+
 from corl.dones.done_func_base import DoneFuncBase
 
 
 class GymnasiumDone(DoneFuncBase):
     """
     A done functor that simply mirrors the done condition coming from the sim state
     this only works with the GymnasiumSimulator
```

### Comparing `corl-3.14.13/corl/dones/pong/commander_pong_dones.py` & `corl-3.16.2/corl/dones/pong/commander_pong_dones.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/dones/pong/dones.py` & `corl-3.16.2/corl/dones/pong/dones.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/dones/sensor_bounds_check_done.py` & `corl-3.16.2/corl/dones/sensor_bounds_check_done.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 from collections import OrderedDict
 
 import gymnasium
 from pydantic import field_validator
 
 from corl.dones.done_func_base import DoneFuncBase, DoneFuncBaseValidator, DoneStatusCodes
 from corl.libraries.property import BoxProp
```

### Comparing `corl-3.14.13/corl/environment/base_multi_agent_env.py` & `corl-3.16.2/corl/environment/base_multi_agent_env.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 ---------------------------------------------------------------------------
 """
 
 import copy
 import typing
 from collections import OrderedDict
 
+import gymnasium
 import gymnasium.utils.seeding
 from pydantic import BaseModel
 from ray.rllib.env.multi_agent_env import MultiAgentEnv
 
 from corl.agents.base_agent import BaseAgent
 from corl.episode_parameter_providers import EpisodeParameterProvider
 from corl.libraries.env_space_util import EnvSpaceUtil
@@ -56,14 +57,16 @@
         self._reward_info: typing.OrderedDict = OrderedDict()
         self._actions: list[typing.Any] = []
         self._observation: typing.OrderedDict = OrderedDict()
         self._agent_dict: dict[str, BaseAgent] = {}
         self._state: BaseSimulatorState
         self._simulator: BaseSimulator
         self._episode_id: int | None = None
+        self.action_space: gymnasium.spaces.Dict
+        self.observation_space: gymnasium.spaces.Dict
 
     @staticmethod
     def get_validator() -> type[BaseCorlMultiAgentEnvValidator]:
         """Get the validator for this class."""
         return BaseCorlMultiAgentEnvValidator
 
     def post_process_trajectory(self, agent_id, batch, episode, policy):
@@ -161,15 +164,15 @@
         get the current episode parameter provider episode id
 
         Returns
         -------
         int or None
             the episode id
         """
-        return self.episode_id
+        return self._episode_id
 
     @property
     def local_variable_store(self) -> dict[str, typing.Any]:
         """
         get the local variable store
 
         Returns
```

### Comparing `corl-3.14.13/corl/environment/custom_env_metrics.py` & `corl-3.16.2/corl/environment/custom_env_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 Logs extra environment metrics specific to Pong.
 """
+
 from ray.rllib import BaseEnv
 from ray.rllib.algorithms.callbacks import DefaultCallbacks
 from ray.rllib.evaluation.episode_v2 import EpisodeV2
 
 
 class CustomPongMetrics(DefaultCallbacks):
     """Logs the number of ball hits for each paddle"""
```

### Comparing `corl-3.14.13/corl/environment/default_env_rllib_callbacks.py` & `corl-3.16.2/corl/environment/default_env_rllib_callbacks.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/environment/environment_wrappers.py` & `corl-3.16.2/corl/environment/environment_wrappers.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 Extra callbacks that can be for evaluating during training to
 generate episode artifacts.
 """
+
 import typing
 
 from ray.rllib.utils.typing import MultiAgentDict
 
 import corl.experiments.rllib_utils.wrappers as rllib_wrappers
 from corl.agents.base_agent import BaseAgent
 from corl.environment.base_multi_agent_env import BaseCorlMultiAgentEnv
```

### Comparing `corl-3.14.13/corl/environment/episode_artifact_callbacks.py` & `corl-3.16.2/corl/environment/episode_artifact_callbacks.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 Extra callbacks that can be for evaluating during training to
 generate episode artifacts.
 """
+
 from corl.evaluation import serialize_platforms
 from corl.evaluation.runners.section_factories.engine.rllib.episode_artifact_logging_callback import EpisodeArtifactLoggingCallback
 
 
 class PongEpisodeArtifactLogger(EpisodeArtifactLoggingCallback):
     """Logs episode artifacts for each evaluation epoch during training"""
```

### Comparing `corl-3.14.13/corl/environment/multi_agent_env.py` & `corl-3.16.2/corl/environment/multi_agent_env.py`

 * *Files 0% similar despite different names*

```diff
@@ -557,52 +557,53 @@
 
         # create dictionary to hold done history
         self.__setup_state_history()
 
         # Create the observation and action space now that we have the glue
         # action space operations
         self._action_prop = DictProp(
-            spaces=self.__agent_aggregator(agent_list=self._trainable_agent_dict.keys(), agent_function=lambda agent, _: agent.action_prop)
+            spaces=self._agent_aggregator(agent_list=self._trainable_agent_dict.keys(), agent_function=lambda agent, _: agent.action_prop)
         )
         self._raw_action_space = self._action_prop.create_space()
         gymnasium_space_sort(self._raw_action_space)
         self._action_units = self._action_prop.get_units()
         self.action_space = gymnasium.spaces.Dict(
-            self.__agent_aggregator(
+            self._agent_aggregator(
                 agent_list=self._trainable_agent_dict.keys(), agent_function=lambda agent, _: agent.normalized_action_space
             )
         )
         gymnasium_space_sort(self.action_space)
         self.full_action_space = gymnasium.spaces.Dict(
-            self.__agent_aggregator(agent_list=self.agent_dict.keys(), agent_function=lambda agent, _: agent.normalized_action_space)
+            self._agent_aggregator(agent_list=self.agent_dict.keys(), agent_function=lambda agent, _: agent.normalized_action_space)
         )
         gymnasium_space_sort(self.full_action_space)
 
         # obs space operations
         self._observation_prop = DictProp(
-            spaces=self.__agent_aggregator(
+            spaces=self._agent_aggregator(
                 agent_list=self._trainable_agent_dict.keys(), agent_function=lambda agent, _: agent.observation_prop
             )
         )
         self._raw_observation_space = self._observation_prop.create_space()
         self._observation_units = self._observation_prop.get_units()
         self.observation_space = gymnasium.spaces.Dict(
-            self.__agent_aggregator(
+            self._agent_aggregator(
                 agent_list=self._trainable_agent_dict.keys(), agent_function=lambda agent, _: agent.normalized_observation_space
             )
         )
+
         self.full_observation_space = gymnasium.spaces.Dict(
-            self.__agent_aggregator(agent_list=self.agent_dict.keys(), agent_function=lambda agent, _: agent.normalized_observation_space)
+            self._agent_aggregator(agent_list=self.agent_dict.keys(), agent_function=lambda agent, _: agent.normalized_observation_space)
         )
 
         self._set_space_seeds()
 
         # full obs
         self._full_observation_prop = DictProp(
-            spaces=self.__agent_aggregator(agent_list=self.agent_dict.keys(), agent_function=lambda agent, _: agent.observation_prop)
+            spaces=self._agent_aggregator(agent_list=self.agent_dict.keys(), agent_function=lambda agent, _: agent.observation_prop)
         )
         self._full_observation_units = self._full_observation_prop.get_units()
 
         self._shared_done: DoneDict = DoneDict()
         self._done_info: OrderedDict = OrderedDict()
         self._reward_info: OrderedDict = OrderedDict()
 
@@ -1125,15 +1126,15 @@
             try:
                 self._sanity_check(self._raw_observation_space, unit_extracted_obs)
             except ValueError as err:
                 if self.config.save_state_pickle:
                     self._save_state_pickle(err)
 
         return OrderedDict(
-            self.__agent_aggregator(
+            self._agent_aggregator(
                 agent_list=alive_agents,
                 agent_function=lambda agent, agent_id, all_agent_obs: agent.create_training_observations(all_agent_obs[agent_id]),
                 all_agent_obs=unit_extracted_obs,
             )
         )
 
     def __get_observations_from_glues(self, alive_agents: typing.Iterable[str]) -> OrderedDict:
@@ -1271,17 +1272,17 @@
         if observations is None:
             observations = dict()
         for agent_name, agent_class in agents.items():
             agent_class.create_next_action(
                 observations.get(agent_name), rewards.get(agent_name), dones.get(agent_name), info.get(agent_name)
             )
 
-    def __agent_aggregator(self, agent_list, agent_function: typing.Callable, **kwargs) -> dict:
+    def _agent_aggregator(self, agent_list, agent_function: typing.Callable, **kwargs) -> dict:
         """
-        __agent_aggregator calls function on all agents and places the output in the in a dictionary.
+        _agent_aggregator calls function on all agents and places the output in the in a dictionary.
         Dictionary key set to the agent name and values are set to the return value of the method
 
         Parameters
         ----------
         agent_function
             A function that takes an agent: BaseAgent as an argument
         Returns
```

### Comparing `corl-3.14.13/corl/environment/pickle_env_state.py` & `corl-3.16.2/corl/environment/pickle_env_state.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/environment/utils/env_creation.py` & `corl-3.16.2/corl/environment/utils/env_creation.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 import typing
 
 from corl.agents.base_agent import AgentParseInfo, BaseAgent, PlatformParseInfo
 from corl.episode_parameter_providers import EpisodeParameterProvider
 from corl.libraries.plugin_library import PluginLibrary
 from corl.simulators.base_parts import BasePlatformPart
```

### Comparing `corl-3.14.13/corl/environment/utils/obs_buffer.py` & `corl-3.16.2/corl/environment/utils/obs_buffer.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/environment/utils/space_sort.py` & `corl-3.16.2/corl/environment/utils/space_sort.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/episode_parameter_providers/__init__.py` & `corl-3.16.2/corl/episode_parameter_providers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 from corl.episode_parameter_providers.core import (
     EpisodeParameterProvider,
     EpisodeParameterProviderValidator,
     ParameterModel,
     PathLike,
     Randomness,
 )
```

### Comparing `corl-3.14.13/corl/episode_parameter_providers/base_network_epp.py` & `corl-3.16.2/corl/episode_parameter_providers/base_network_epp.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 import copy
 from abc import abstractmethod
 from collections.abc import Mapping
 from dataclasses import dataclass
 from typing import Generic, Literal, TypeVar
 
 from pydantic import validator
@@ -85,16 +86,15 @@
         print(f"BaseNetworkParameterProvider::on_message {id(self)} {epp_update.test_case_index}")
         self.cur_params = self._do_update_params(copy.deepcopy(self.base_params), epp_update.update)
         self._test_case_idx = epp_update.test_case_index
 
     @abstractmethod
     def _do_update_params(
         self, params: Mapping[tuple[str, ...], OverridableParameterWrapper], updates: T
-    ) -> Mapping[tuple[str, ...], OverridableParameterWrapper]:
-        ...
+    ) -> Mapping[tuple[str, ...], OverridableParameterWrapper]: ...
 
     # def __setstate__(self, state):
     #     self.__dict__.update(state)
     #     self.config.registrar.epp_update_signal.register(Slot(self))
 
 
 class TestNetworkedParameterProvider(BaseNetworkParameterProvider):
```

### Comparing `corl-3.14.13/corl/episode_parameter_providers/core.py` & `corl-3.16.2/corl/episode_parameter_providers/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 import abc
 import os
 import typing
 
 from numpy.random import Generator, RandomState
 from pydantic import BaseModel, ConfigDict
```

### Comparing `corl-3.14.13/corl/episode_parameter_providers/incremental.py` & `corl-3.16.2/corl/episode_parameter_providers/incremental.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 This module defines an evaluation specific ParameterProvider, which wraps a given ParameterProvider
 and delegates parameter value generation to it. It increments an internal 'index' attribute up to
 the provided 'num_test_cases' int, to provide an accurate episode_id during evaluation.
 
 Author: John McCarroll
 """
 
-
 from pydantic import ImportString
 
 from corl.episode_parameter_providers import EpisodeParameterProvider, EpisodeParameterProviderValidator, ParameterModel, Randomness
 
 
 class IncrementalWrapperValidator(EpisodeParameterProviderValidator):
     """
@@ -63,9 +62,7 @@
         # get episode_id
         episode_id = self.index if self.index < self.config.num_test_cases else None  # type: ignore
 
         # increment after params collected
         self.index += 1
 
         return params, episode_id, env_epp_ctx
-
-    # TODO: delegate other methods to wrapped EPP?
```

### Comparing `corl-3.14.13/corl/episode_parameter_providers/remote.py` & `corl-3.16.2/corl/episode_parameter_providers/remote.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/episode_parameter_providers/simple.py` & `corl-3.16.2/corl/episode_parameter_providers/simple.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,19 +6,17 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
 
-
 from corl.episode_parameter_providers import EpisodeParameterProvider, ParameterModel, Randomness
 
 
 class SimpleParameterProvider(EpisodeParameterProvider):
     """EpisodeParameterProvider that does nothing but return the default."""
 
-    def reset(self):
-        ...
+    def reset(self): ...
 
     def _do_get_params(self, rng: Randomness, env_epp_ctx: dict | None) -> tuple[ParameterModel, int | None, dict | None]:
         return self.config.parameters, None, env_epp_ctx
```

### Comparing `corl-3.14.13/corl/episode_parameter_providers/tabular_parameter_provider.py` & `corl-3.16.2/corl/episode_parameter_providers/tabular_parameter_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 EpisodeParameterProvider that reads data from a tabular structure.
 """
+
 import copy
 import typing
 
 import pandas as pd
 from pydantic import field_validator, model_validator
 
 from corl.episode_parameter_providers import EpisodeParameterProvider, EpisodeParameterProviderValidator, ParameterModel, Randomness
```

### Comparing `corl-3.14.13/corl/evaluation/connection/base_epp_update.py` & `corl-3.16.2/corl/evaluation/connection/base_epp_update.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 from abc import abstractmethod
 
 from corl.libraries.units import Quantity
 
 
 class BaseEppUpdate:
     @abstractmethod
-    def get_updates(self) -> dict[tuple[str, ...], Quantity | float | str]:
-        ...
+    def get_updates(self) -> dict[tuple[str, ...], Quantity | float | str]: ...
 
 
 def get_updates(updates: BaseEppUpdate, prefix: str | None = None) -> dict[tuple[str, ...], Quantity | float | str]:
     modified_updates: dict[tuple[str, ...], Quantity | float | str] = {}
 
     key: tuple[str, ...]
     value: Quantity | float | str
```

### Comparing `corl-3.14.13/corl/evaluation/connection/base_eval_connection.py` & `corl-3.16.2/corl/evaluation/connection/base_eval_connection.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 import logging
 from abc import abstractmethod
 from typing import Annotated, Generic, TypeVar
 
 from pydantic import BaseModel, BeforeValidator, ConfigDict
 
 from corl.evaluation.connection.signal import Signal
 from corl.evaluation.launchers.base_eval import EvalConfig
 from corl.libraries.factory import Factory
 
 EppUpdateT = TypeVar("EppUpdateT")
 
 
-class BaseEvalConnectionValidator(BaseModel):
-    ...
+class BaseEvalConnectionValidator(BaseModel): ...
 
 
 class BaseEvalConnection(Generic[EppUpdateT]):
     def __init__(self, **kwargs):
         self._config = self.get_validator()(**kwargs)
         self._logger = logging.getLogger(type(self).__name__)
```

### Comparing `corl-3.14.13/corl/evaluation/connection/base_rest_connection.py` & `corl-3.16.2/corl/evaluation/connection/base_rest_connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 import threading
 from typing import TypeVar
 
 import uvicorn
 from fastapi import FastAPI, Request, status
 from fastapi.encoders import jsonable_encoder
 from fastapi.exceptions import RequestValidationError
```

### Comparing `corl-3.14.13/corl/evaluation/connection/signal.py` & `corl-3.16.2/corl/evaluation/connection/signal.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 from abc import abstractmethod
 from collections.abc import Callable
 from typing import Any, Generic, TypeVar, final
 from weakref import CallableProxyType, ReferenceType, proxy, ref
 
 T = TypeVar("T")
 
@@ -61,16 +62,15 @@
 #                     return _TypeChecker(arg_types)
 
 #                 return _TypeChecker((type_,))
 
 #         return _TypeChecker()
 
 
-class SlotExpired(RuntimeError):
-    ...
+class SlotExpired(RuntimeError): ...
 
 
 class BaseSlot(Generic[T]):
     def __init__(self, *args, **kwargs):
         super().__init__()
         self._expired = False
         self._signals: list[ReferenceType[Signal[T]]] = []  # type: ignore
@@ -87,16 +87,15 @@
 
     def on_message(self, data: T) -> Any:
         if self._expired:
             raise SlotExpired
         return self._on_message(data)
 
     @abstractmethod
-    def _on_message(self, data: T) -> Any:
-        ...
+    def _on_message(self, data: T) -> Any: ...
 
     def __setstate__(self, state):
         self.__dict__.update(state)
         for signal_ref in self._signals:
             if (signal := signal_ref()) is not None:
                 signal.register(self)
```

### Comparing `corl-3.14.13/corl/evaluation/default_config_updates.py` & `corl-3.16.2/corl/evaluation/default_config_updates.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 -------------------------------------------------------------------------------
 
 A set of standard config updates that can be used.
 """
+
 from corl.evaluation.runners.section_factories.plugins.config_updater import ConfigUpdate
 
 
 class DoNothingConfigUpdate(ConfigUpdate):
     """
     A config update that does nothing. Used as a placeholder/default when no config update is required.
     """
```

### Comparing `corl-3.14.13/corl/evaluation/episode_artifact.py` & `corl-3.16.2/corl/evaluation/episode_artifact.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 from __future__ import annotations
 
 import dataclasses
 import typing
 from collections import OrderedDict
 from datetime import datetime
```

### Comparing `corl-3.14.13/corl/evaluation/eval_logger_name.py` & `corl-3.16.2/corl/evaluation/runners/section_factories/engine/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,10 +4,9 @@
 Reinforcement Learning (RL) Core.
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
-Constant name for evaluation logger
+Module for engines that execute the the learning network
 """
-EVAL_LOGGER_NAME = "Evaluator"
```

### Comparing `corl-3.14.13/corl/evaluation/evaluation_artifacts.py` & `corl-3.16.2/corl/evaluation/evaluation_artifacts.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 import dataclasses
 
 import jsonargparse
 
 from corl.evaluation.recording.i_recorder import IRecord
```

### Comparing `corl-3.14.13/corl/evaluation/evaluation_factory.py` & `corl-3.16.2/corl/evaluation/evaluation_factory.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/evaluation/evaluation_outcome.py` & `corl-3.16.2/corl/evaluation/evaluation_outcome.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 Contains classes to represent
 """
+
 import dataclasses
 from collections import defaultdict
 from typing import Any
 
 import pandas as pd
 from pydantic import validator
```

### Comparing `corl-3.14.13/corl/evaluation/launchers/__init__.py` & `corl-3.16.2/corl/evaluation/util/__init__.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/evaluation/launchers/base_eval.py` & `corl-3.16.2/corl/evaluation/launchers/base_eval.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/evaluation/launchers/evaluate_runner.py` & `corl-3.16.2/corl/evaluation/launchers/evaluate_runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 import gc
 import logging
 import os
 import tempfile
 import time
 from pathlib import Path
 from threading import Condition, Thread
@@ -67,16 +68,15 @@
     model_config = ConfigDict(arbitrary_types_allowed=True)
 
     run_forever: bool = False
     tmpdir_base: Path | None = None
     connection: BaseEvalConnection | None = None
 
 
-class EppReset:
-    ...
+class EppReset: ...
 
 
 class EvalRunner:
     def __init__(self, **kwargs):
         super().__init__()
         self._config = self.get_validator()(**kwargs)
```

### Comparing `corl-3.14.13/corl/evaluation/launchers/evaluate_validator.py` & `corl-3.16.2/corl/evaluation/launchers/evaluate_validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 import difflib
 import gc
 import pprint
 from functools import partial
 from pathlib import Path
 from typing import Annotated
 from weakref import CallableProxyType, proxy
@@ -115,14 +116,14 @@
 
             self.teams.iterate_on_participant(apply_weights)
             if algorithm.workers is not None:
                 algorithm.workers.sync_weights()
 
             self.algorithm_ = algorithm
 
-        return self.algorithm
+        return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         if self.algorithm_ is not None:
             cleanup_algorithm(self.algorithm_)
             self.algorithm_ = None
             gc.collect()
```

### Comparing `corl-3.14.13/corl/evaluation/launchers/launch_evaluate.py` & `corl-3.16.2/corl/evaluation/launchers/launch_evaluate.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 import logging
 from collections.abc import Sequence
 from pathlib import Path
 from typing import Any, cast
 
 import jsonargparse
 
@@ -129,42 +130,42 @@
 
 
 def load_config(config_file: Path) -> dict[str, Any]:
     """Loads config from file"""
     return cast(dict[str, Any], load_file(config_filename=config_file))
 
 
-def main(instantiated_args: jsonargparse.Namespace, config: dict[str, Any]):
+def main(cfg_path: Path, tmpdir_base: Path, config: dict[str, Any], include_dashboard: bool = False):
     """Main function block to evaluate from a configuration
 
     Parameters:
     ----------
         instantiated_args: jsonargparse.Namespace
             Contains as a Namespace the instantiated objects needed to run evaluation.
     """
     if "experiment" not in config:
         config = {"experiment": config}
 
     connection = ConnectionValidator(**config).connection
 
     with add_context({"connection": connection}):
-        kwargs = {"path": instantiated_args.cfg, "raw_config": config, **config}
+        kwargs = {"path": cfg_path, "raw_config": config, **config}
         eval_schema = EvalConfig(**kwargs)
 
-        with ray_context(local_mode=eval_schema.experiment.engine.rllib.debug_mode, include_dashboard=instantiated_args.include_dashboard):
-            eval_runner = EvalRunner(tmpdir_base=instantiated_args.tmpdir_base, **{**config, "connection": connection})
+        with ray_context(local_mode=eval_schema.experiment.engine.rllib.debug_mode, include_dashboard=include_dashboard):
+            eval_runner = EvalRunner(tmpdir_base=tmpdir_base, **{**config, "connection": connection})
             eval_runner(eval_schema)
             eval_runner.run()
 
 
 def pre_main(alternate_argv: Sequence[str] | None = None):
     """
     calls gets current args and passes them to main
     """
     instantiated, args = get_args(alternate_argv=alternate_argv)
     LoggingSetup(default_path=str(args.log_config), default_level=logging._nameToLevel[args.log_level])  # noqa: SLF001
     cfg = load_config(instantiated.cfg)
-    main(instantiated, cfg)
+    main(instantiated.cfg, instantiated.tmpdir_base, cfg, include_dashboard=instantiated.include_dashboard)
 
 
 if __name__ == "__main__":
     pre_main()
```

### Comparing `corl-3.14.13/corl/evaluation/launchers/launch_generate_metrics.py` & `corl-3.16.2/corl/evaluation/launchers/launch_generate_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 Entry/Launch point to the generate_metrics process/segment of the evaluation framework.
 """
+
 import itertools
 import pathlib
 import typing
 
 import jsonargparse
 import pandas as pd
 import ray.cloudpickle as pickle
```

### Comparing `corl-3.14.13/corl/evaluation/launchers/launch_pipeline.py` & `corl-3.16.2/corl/evaluation/launchers/launch_pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 Entry / Launch point to run the evaluation framework processes, evaluation , generate_metrics , visualize back to back .
 There are also various storage options
 """
+
 from pathlib import Path
 from typing import Any
 
 import jsonargparse
 
 from corl.evaluation.evaluation_artifacts import (
     EvaluationArtifact_EvaluationOutcome,
```

### Comparing `corl-3.14.13/corl/evaluation/launchers/launch_storage.py` & `corl-3.16.2/corl/evaluation/launchers/launch_storage.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/evaluation/launchers/launch_visualize.py` & `corl-3.16.2/corl/evaluation/launchers/launch_visualize.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 Launch process for performing and visualizing an evaluation
 """
+
 import typing
 
 import jsonargparse
 
 from corl.evaluation.evaluation_artifacts import EvaluationArtifact_Metrics, EvaluationArtifact_Visualization
 from corl.evaluation.visualization.visualization import Visualization
```

### Comparing `corl-3.14.13/corl/evaluation/launchers/rest_eval_connection.py` & `corl-3.16.2/corl/evaluation/launchers/rest_eval_connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 from pathlib import Path
 from typing import Annotated
 
 from fastapi import Request, status
 from fastapi.responses import JSONResponse
 from pydantic import BaseModel, BeforeValidator, ValidationError
 
@@ -31,16 +32,15 @@
 
 
 class _ResetSchema(BaseModel):
     path: Path | None = None
     config: Annotated[dict | None, BeforeValidator(build_config)] = None
 
 
-class RestEvalConnectionValidator(RestConnectionValidator, BaseEvalConnectionValidator):
-    ...
+class RestEvalConnectionValidator(RestConnectionValidator, BaseEvalConnectionValidator): ...
 
 
 class RestEvalConnection(BaseRestConnection, BaseEvalConnection[SimpleEppUpdate]):
     def __init__(self, **kwargs):
         external_delay_start = kwargs.get("delay_start", False)
         kwargs["delay_start"] = True
         super().__init__(**kwargs)
```

### Comparing `corl-3.14.13/corl/evaluation/loader/__init__.py` & `corl-3.16.2/corl/evaluation/loader/__init__.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/evaluation/loader/heuristic.py` & `corl-3.16.2/corl/evaluation/loader/heuristic.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 Load an agent from a weight file
 """
+
 import dataclasses
 import logging
 
 from ray.rllib.algorithms import Algorithm
 
 from corl.evaluation.loader.i_agent_loader import IAgentLoader
```

### Comparing `corl-3.14.13/corl/evaluation/loader/i_agent_loader.py` & `corl-3.16.2/corl/evaluation/loader/i_agent_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 Abstract class to load agents
 """
+
 import re
 from abc import abstractmethod
 
 from ray.rllib.algorithms import Algorithm
 from ray.rllib.utils.typing import ModelWeights
```

### Comparing `corl-3.14.13/corl/evaluation/loader/policy_checkpoint.py` & `corl-3.16.2/corl/evaluation/loader/policy_checkpoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 Load and agent from Checkpoint file
 """
+
 import os
 import typing
 from pathlib import Path
 
 from pydantic import BaseModel, ConfigDict, field_validator
 from ray.rllib.algorithms import Algorithm
 from ray.rllib.policy.policy import Policy
```

### Comparing `corl-3.14.13/corl/evaluation/metrics/aggregators/accumulate.py` & `corl-3.16.2/corl/evaluation/metrics/aggregators/accumulate.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/evaluation/metrics/aggregators/average.py` & `corl-3.16.2/corl/evaluation/metrics/aggregators/average.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 import typing
 
 from corl.evaluation.metrics.generator import MetricGeneratorAggregator
 from corl.evaluation.metrics.metric import Metric, NonTerminalMetric
 from corl.evaluation.metrics.types.nonterminals.timed_value import TimedValue
 from corl.evaluation.metrics.types.nonterminals.vector import Vector
 from corl.evaluation.metrics.types.terminals.void import Void
```

### Comparing `corl-3.14.13/corl/evaluation/metrics/aggregators/counter.py` & `corl-3.16.2/corl/evaluation/metrics/aggregators/counter.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 import itertools
 import typing
 from collections import Counter
 
 from corl.evaluation.metrics.generator import MetricGeneratorAggregator
 from corl.evaluation.metrics.metric import Metric
 from corl.evaluation.metrics.types.nonterminals.dict import Dict
```

### Comparing `corl-3.14.13/corl/evaluation/metrics/aggregators/criteria_rate.py` & `corl-3.16.2/corl/evaluation/metrics/aggregators/criteria_rate.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/evaluation/metrics/aggregators/sum.py` & `corl-3.16.2/corl/evaluation/metrics/aggregators/sum.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 import typing
 
 from corl.evaluation.metrics.generator import MetricGeneratorAggregator
 from corl.evaluation.metrics.metric import Metric, NonTerminalMetric
 from corl.evaluation.metrics.types.nonterminals.timed_value import TimedValue
 from corl.evaluation.metrics.types.nonterminals.vector import Vector
 from corl.evaluation.metrics.types.terminals.void import Void
```

### Comparing `corl-3.14.13/corl/evaluation/metrics/alerts.py` & `corl-3.16.2/corl/evaluation/metrics/alerts.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/evaluation/metrics/generator.py` & `corl-3.16.2/corl/evaluation/metrics/generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 Classes that represent a metric generator
 
 A metric generator is a class that generates a metric.
 """
+
 import abc
 import typing
 
 from pydantic import BaseModel, field_validator
 
 from corl.evaluation.episode_artifact import EpisodeArtifact
 from corl.evaluation.metrics.metric import Metric
```

### Comparing `corl-3.14.13/corl/evaluation/metrics/generators/dones.py` & `corl-3.16.2/corl/evaluation/metrics/generators/dones.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 from corl.dones.done_func_base import DoneStatusCodes
 from corl.evaluation.episode_artifact import EpisodeArtifact
 from corl.evaluation.metrics.generator import MetricGeneratorTerminalEventScope
 from corl.evaluation.metrics.metric import Metric
 from corl.evaluation.metrics.types.nonterminals.vector import Vector
 from corl.evaluation.metrics.types.terminals.discrete import Discrete
 from corl.evaluation.metrics.types.terminals.string import String
```

### Comparing `corl-3.14.13/corl/evaluation/metrics/generators/meta/episode_length.py` & `corl-3.16.2/corl/evaluation/metrics/generators/meta/episode_length.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 from corl.evaluation.episode_artifact import EpisodeArtifact
 from corl.evaluation.metrics.generator import MetricGeneratorTerminalEventScope
 from corl.evaluation.metrics.metric import Metric
 from corl.evaluation.metrics.types.terminals.real import Real
 
 
 class EpisodeLength_Steps(MetricGeneratorTerminalEventScope):
```

### Comparing `corl-3.14.13/corl/evaluation/metrics/generators/meta/runtime.py` & `corl-3.16.2/corl/evaluation/metrics/generators/meta/runtime.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 from corl.evaluation.episode_artifact import EpisodeArtifact
 from corl.evaluation.metrics.generator import MetricGeneratorTerminalEventScope
 from corl.evaluation.metrics.metric import Metric
 from corl.evaluation.metrics.types.terminals.real import Real
 
 
 class Runtime(MetricGeneratorTerminalEventScope):
```

### Comparing `corl-3.14.13/corl/evaluation/metrics/generators/rewards.py` & `corl-3.16.2/corl/evaluation/metrics/generators/rewards.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/evaluation/metrics/metric.py` & `corl-3.16.2/corl/evaluation/metrics/metric.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,20 +14,18 @@
 import typing
 
 
 class Metric:
     """Abstract class that any metric is to inherit from"""
 
     @abc.abstractmethod
-    def __add__(self, rhs: typing.Any):
-        ...
+    def __add__(self, rhs: typing.Any): ...
 
     @abc.abstractmethod
-    def __truediv__(self, rhs: typing.Any):
-        ...
+    def __truediv__(self, rhs: typing.Any): ...
 
 
 class TerminalMetric(abc.ABC, Metric):  # Allows for enhanced type checking
     """Abstract class that a terminal metric is to inherit from.
 
     A Terminal metric is one that is not contains pure data.
     Examples: Real, String, etc
```

### Comparing `corl-3.14.13/corl/evaluation/metrics/processors.py` & `corl-3.16.2/corl/evaluation/metrics/processors.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 Contains processors that execute on given data
 """
+
 from __future__ import annotations
 
 import abc
 import typing
 
 from corl.evaluation.episode_artifact import EpisodeArtifact
 from corl.evaluation.metrics.alerts import Alert, AlertGenerator
```

### Comparing `corl-3.14.13/corl/evaluation/metrics/scenario_alert_generators.py` & `corl-3.16.2/corl/evaluation/metrics/scenario_alert_generators.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 from __future__ import annotations
 
 from pydantic import BaseModel
 
 from .alerts import AlertGenerator
```

### Comparing `corl-3.14.13/corl/evaluation/metrics/scenario_metric_generators.py` & `corl-3.16.2/corl/evaluation/metrics/scenario_metric_generators.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 from __future__ import annotations
 
 from pydantic import BaseModel
 
 from corl.evaluation.metrics.generator import MetricGenerator
 from corl.libraries.factory import Factory
 from corl.libraries.functor import Functor
```

### Comparing `corl-3.14.13/corl/evaluation/metrics/scopes.py` & `corl-3.16.2/corl/evaluation/metrics/scopes.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 import enum
 
 
 class Scopes(enum.IntEnum):
     """Scopes which a metric can be computed on"""
 
     EVENT = enum.auto()
```

### Comparing `corl-3.14.13/corl/evaluation/metrics/types/nonterminals/dict.py` & `corl-3.16.2/corl/evaluation/metrics/types/nonterminals/dict.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 import dataclasses
 import typing
 
 from corl.evaluation.metrics.metric import Metric, NonTerminalMetric
 
 
 @dataclasses.dataclass
```

### Comparing `corl-3.14.13/corl/evaluation/metrics/types/nonterminals/timed_value.py` & `corl-3.16.2/corl/evaluation/metrics/types/nonterminals/timed_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 import typing
 
 from pydantic import BaseModel, ConfigDict, field_validator
 
 from corl.evaluation.metrics.metric import Metric, NonTerminalMetric
 from corl.libraries.units import Quantity, corl_get_ureg
```

### Comparing `corl-3.14.13/corl/evaluation/metrics/types/nonterminals/vector.py` & `corl-3.16.2/corl/evaluation/metrics/types/nonterminals/vector.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 import typing
 
 from corl.evaluation.metrics.metric import Metric, NonTerminalMetric
 from corl.evaluation.metrics.types.nonterminals.timed_value import TimedValue
 
 
 class Vector(NonTerminalMetric):
```

### Comparing `corl-3.14.13/corl/evaluation/metrics/types/terminals/discrete.py` & `corl-3.16.2/corl/evaluation/metrics/types/terminals/discrete.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 import dataclasses
 import typing
 
 from corl.evaluation.metrics.metric import TerminalMetric
 
 Enum = typing.TypeVar("Enum")
```

### Comparing `corl-3.14.13/corl/evaluation/metrics/types/terminals/rate.py` & `corl-3.16.2/corl/evaluation/metrics/types/terminals/rate.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 from __future__ import annotations
 
 import dataclasses
 import typing
 
 from corl.evaluation.metrics.metric import TerminalMetric
```

### Comparing `corl-3.14.13/corl/evaluation/metrics/types/terminals/real.py` & `corl-3.16.2/corl/evaluation/metrics/types/terminals/real.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 import dataclasses
 import typing
 
 from corl.evaluation.metrics.metric import TerminalMetric
 from corl.libraries.units import Quantity
```

### Comparing `corl-3.14.13/corl/evaluation/metrics/types/terminals/string.py` & `corl-3.16.2/corl/evaluation/metrics/types/terminals/string.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 import dataclasses
 import typing
 
 from corl.evaluation.metrics.metric import TerminalMetric
 
 
 @dataclasses.dataclass
```

### Comparing `corl-3.14.13/corl/evaluation/metrics/types/terminals/void.py` & `corl-3.16.2/corl/evaluation/metrics/types/terminals/void.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 import typing
 
 from corl.evaluation.metrics.metric import TerminalMetric
 
 
 class Void(TerminalMetric):
     """Terminal Metric to represent a real number"""
```

### Comparing `corl-3.14.13/corl/evaluation/recording/folder.py` & `corl-3.16.2/corl/evaluation/recording/folder.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 Records an evaluation outcome to a folder
 """
+
 import contextlib
 import logging
 import shutil
 from datetime import datetime
 from pathlib import Path
 from shutil import copyfile
```

### Comparing `corl-3.14.13/corl/evaluation/recording/i_recorder.py` & `corl-3.16.2/corl/evaluation/recording/i_recorder.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 Contains abstract interfaces defining how to record an Evaluation outcome
 """
+
 import typing
 from abc import abstractmethod
 from pathlib import Path
 
 from corl.evaluation.evaluation_outcome import EvaluationOutcome
```

### Comparing `corl-3.14.13/corl/evaluation/runners/__init__.py` & `corl-3.16.2/corl/evaluation/visualization/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,9 +4,9 @@
 Reinforcement Learning (RL) Core.
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
-Collection of methods to perform evaluation
+Module containing visualizations for evaluations
 """
```

### Comparing `corl-3.14.13/corl/evaluation/runners/inference/algorithm_runner.py` & `corl-3.16.2/corl/evaluation/runners/inference/algorithm_runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 import gc
 import logging
 import traceback
 import typing
 from collections.abc import Iterator
 from threading import Condition
 from weakref import CallableProxyType
@@ -100,15 +101,15 @@
             gc.collect()
             self._algorithm_cv.notify_all()
 
     @property
     def _runner(self) -> EnvRunnerV2:
         if self.__runner is None:
             multiple_episodes_in_batch = self.algorithm.config.batch_mode != "complete_episodes"
-            rollout_fragment_length = int(self.algorithm.config.rollout_fragment_length)
+            rollout_fragment_length = int(self.algorithm.config.get_rollout_fragment_length())
             self.__runner = EnvRunnerV2(
                 self.local_worker,
                 convert_to_base_env(env=self.local_worker.env),
                 multiple_episodes_in_batch=multiple_episodes_in_batch,
                 callbacks=self.algorithm.callbacks,
                 perf_stats=_PerfStats(),
                 rollout_fragment_length=rollout_fragment_length,
```

### Comparing `corl-3.14.13/corl/evaluation/runners/inference/inference.py` & `corl-3.16.2/corl/evaluation/runners/inference/inference.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,15 +6,18 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
 
+from collections.abc import Iterator
+
 from pydantic import validator
+from ray.rllib.policy.sample_batch import MultiAgentBatch, SampleBatch
 
 from corl.evaluation.launchers.base_eval import BaseEvaluator, BaseEvaluatorValidator, EvalConfig
 
 from .algorithm_runner import AlgorithmRunner
 
 
 class InferenceValidator(BaseEvaluatorValidator):
@@ -45,10 +48,10 @@
 
     def reset(self):
         self._config.algorithm_runner.stop(continue_running=True)
 
     def stop(self):
         self._config.algorithm_runner.stop()
 
-    def __call__(self, config: EvalConfig, **kwargs):
+    def __call__(self, config: EvalConfig, **kwargs) -> Iterator[SampleBatch | MultiAgentBatch]:
         self._config.algorithm_runner.reset(config.experiment.algorithm)
         yield from self._config.algorithm_runner.run()
```

### Comparing `corl-3.14.13/corl/evaluation/runners/inference/inference_callback.py` & `corl-3.16.2/corl/evaluation/runners/inference/inference_callback.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 from abc import abstractmethod
 from collections.abc import Callable
 from typing import Generic, TypeVar
 
 from pydantic import BaseModel
 from ray.rllib.algorithms.algorithm import Algorithm
 from ray.rllib.algorithms.callbacks import DefaultCallbacks
@@ -35,9 +36,8 @@
 
     def on_algorithm_init(self, *, algorithm: Algorithm, **kwargs) -> None:
         super().on_algorithm_init(algorithm=algorithm, kwargs=kwargs)
 
         self.config = self.get_validator()(**dict(algorithm.config).get(f"{type(self).__name__}", {}))
 
     @abstractmethod
-    def process_message(self, message: T):
-        ...
+    def process_message(self, message: T): ...
```

### Comparing `corl-3.14.13/corl/evaluation/runners/inference/protocol/simple_epp_update.py` & `corl-3.16.2/corl/evaluation/runners/inference/protocol/simple_epp_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 from pydantic import BaseModel
 
 from corl.evaluation.connection.base_epp_update import BaseEppUpdate
 from corl.libraries.units import Quantity
 
 
 class SimpleEppUpdate(BaseModel, BaseEppUpdate):
```

### Comparing `corl-3.14.13/corl/evaluation/runners/inference/protocol/simple_network_epp.py` & `corl-3.16.2/corl/evaluation/runners/inference/protocol/simple_network_epp.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 from collections.abc import Mapping
 
 from corl.episode_parameter_providers import EpisodeParameterProviderValidator
 from corl.episode_parameter_providers.base_network_epp import BaseNetworkParameterProvider, NetworkedParameterProviderValidator
 from corl.evaluation.connection.base_epp_update import get_updates
 from corl.evaluation.runners.inference.protocol.simple_epp_update import SimpleEppUpdate
 from corl.libraries.parameters import OverridableParameterWrapper, ParameterValidator
```

### Comparing `corl-3.14.13/corl/evaluation/runners/inference/protocol/simple_network_epp_strategy.py` & `corl-3.16.2/corl/evaluation/runners/inference/protocol/simple_network_epp_strategy.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 from typing import Any
 
 import numpy as np
 import pandas as pd
 
 from corl.evaluation.connection.base_epp_update import get_updates
 from corl.evaluation.runners.inference.protocol.simple_epp_update import SimpleEppUpdate
```

### Comparing `corl-3.14.13/corl/evaluation/runners/iterate_test_cases.py` & `corl-3.16.2/corl/evaluation/runners/iterate_test_cases.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/evaluation/runners/section_factories/__init__.py` & `corl-3.16.2/corl/evaluation/runners/section_factories/__init__.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/evaluation/runners/section_factories/engine/__init__.py` & `corl-3.16.2/corl/evaluation/runners/section_factories/engine/rllib/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,9 +4,9 @@
 Reinforcement Learning (RL) Core.
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
-Module for engines that execute the the learning network
+Rllib Engine Module
 """
```

### Comparing `corl-3.14.13/corl/evaluation/runners/section_factories/engine/rllib/__init__.py` & `corl-3.16.2/corl/evaluation/eval_logger_name.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,9 +4,11 @@
 Reinforcement Learning (RL) Core.
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
-Rllib Engine Module
+Constant name for evaluation logger
 """
+
+EVAL_LOGGER_NAME = "Evaluator"
```

### Comparing `corl-3.14.13/corl/evaluation/runners/section_factories/engine/rllib/default_evaluation_callbacks.py` & `corl-3.16.2/corl/evaluation/runners/section_factories/engine/rllib/default_evaluation_callbacks.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 Callbacks to do logging of episodes
 """
+
 import collections
 import copy
 import typing
 from abc import ABC, abstractmethod
 from datetime import datetime
 
 import flatten_dict
@@ -23,35 +24,74 @@
 from ray.rllib.evaluation.episode_v2 import EpisodeV2
 from ray.rllib.policy import Policy
 from ray.rllib.policy.sample_batch import SampleBatch
 from ray.rllib.utils.typing import AgentID, PolicyID
 
 from corl.environment.base_multi_agent_env import BaseCorlMultiAgentEnv
 from corl.evaluation.episode_artifact import EpisodeArtifact
+from corl.evaluation.runners.section_factories.plugins.platform_serializer import PlatformSerializer
 from corl.simulators.base_simulator import BaseSimulator
 
 
 class DefaultEvaluationCallbacks(DefaultCallbacks, ABC):
     """Callbacks to extract data for evaluation reporting.
 
     This is intended to be used as a subclass of the environment callbacks used by the experiment using cooperative multiple inheritance.
     """
 
     @abstractmethod
-    def platform_serializer(self):
+    def platform_serializer(self) -> PlatformSerializer:
         """
         Function that holds a placeholder for the SerializePlatform object which contains a serialization function.
         The SerializePlatform object is to be instantiated and placed inside this method for future use
         """
 
     @abstractmethod
     def extract_environment_state(self, env_state: dict):
         """Method that extracts any information in the environment state that needs to be saved"""
         return {}
 
+    def extract_step_data(self, env) -> dict[str, dict[str, typing.Any]]:  # noqa: PLR6301
+        """Method that extracts actions and observations for each agent in the environment
+        Returns
+        -------
+        dict[str, dict[str, typing.Any]]
+        dict[AGENT_ID, dict[Union[Literal['action'] | Literal['observation']], Any]]
+        """
+        step_data: dict[str, dict[str, typing.Any]] = {
+            agent_id: {"observation": collections.OrderedDict(), "action": collections.OrderedDict()} for agent_id in env.agent_dict
+        }
+
+        for agent_id, obj_pair in env.observation.items():
+            step_data[agent_id]["observation"] = obj_pair
+
+        if env._actions:  # noqa: SLF001
+            for agent_id, agent_data in env._actions[-1].items():  # noqa: SLF001
+                if isinstance(agent_data, dict):
+                    agent_data = flatten_dict.flatten(agent_data)  # noqa: PLW2901
+                    for part_name, value in agent_data.items():
+                        part_name = ".".join(part_name)  # noqa: PLW2901
+                        if isinstance(value, tuple) and len(value) > 0 and isinstance(value[0], dict):
+                            # handle RTAModule or otherwise wrapped controllers
+                            for elem in value:
+                                for sub_part_name, sub_value in elem.items():
+                                    step_data[agent_id]["action"][f"{part_name}.{sub_part_name}"] = sub_value
+                        else:
+                            step_data[agent_id]["action"][part_name] = value
+                elif isinstance(agent_data, np.ndarray):
+                    step_data[agent_id]["action"] = collections.OrderedDict()
+                    for i, val in enumerate(agent_data):
+                        step_data[agent_id]["action"][f"action_{i!s}"] = np.array([val])
+                else:
+                    raise ValueError("Only action types dict and np.ndarray are supported")
+
+                # step_data[agent_id]['action'] = agent_data    # change from corl2.0 merge
+
+        return step_data
+
     def on_episode_start(
         self,  # noqa: PLR6301
         *,
         worker: RolloutWorker,
         base_env: BaseEnv,
         policies: dict[PolicyID, Policy],
         episode: EpisodeV2,
@@ -104,15 +144,15 @@
         for agent_id, agent in env.agent_dict.items():
             parameter_values[agent_id] = flatten_dict.flatten(agent.local_variable_store, reducer="dot")
         episode.user_data["parameter_values"] = parameter_values
 
         # Cooperative multiple inheritance
         super().on_episode_start(worker=worker, base_env=base_env, policies=policies, episode=episode, **kwargs)
 
-    def on_episode_step(  # noqa: PLR0912, PLR0915
+    def on_episode_step(
         self,
         *,
         worker: RolloutWorker,
         base_env: BaseEnv,
         policies: dict[PolicyID, Policy] | None = None,
         episode: EpisodeV2,
         **kwargs,
@@ -147,42 +187,15 @@
                         continue
                     episode.user_data["dones"][agent_id].update(self._resolve_sequence_values(name, value))
 
         episode_state: dict = copy.deepcopy(env.state.agent_episode_state)
 
         # ######################################
         # # Step data - append on each step
-        step_data: dict[str, dict[str, typing.Any]] = {
-            agent_id: {"observation": collections.OrderedDict(), "action": collections.OrderedDict()} for agent_id in env.agent_dict
-        }
-
-        for agent_id, obj_pair in env.observation.items():
-            step_data[agent_id]["observation"] = obj_pair
-
-        if env._actions:  # noqa: SLF001
-            for agent_id, agent_data in env._actions[-1].items():  # noqa: SLF001
-                if isinstance(agent_data, dict):
-                    agent_data = flatten_dict.flatten(agent_data)  # noqa: PLW2901
-                    for part_name, value in agent_data.items():
-                        part_name = ".".join(part_name)  # noqa: PLW2901
-                        if isinstance(value, tuple) and len(value) > 0 and isinstance(value[0], dict):
-                            # handle RTAModule or otherwise wrapped controllers
-                            for elem in value:
-                                for sub_part_name, sub_value in elem.items():
-                                    step_data[agent_id]["action"][f"{part_name}.{sub_part_name}"] = sub_value
-                        else:
-                            step_data[agent_id]["action"][part_name] = value
-                elif isinstance(agent_data, np.ndarray):
-                    step_data[agent_id]["action"] = collections.OrderedDict()
-                    for i, val in enumerate(agent_data):
-                        step_data[agent_id]["action"][f"action_{i!s}"] = np.array([val])
-                else:
-                    raise ValueError("Only action types dict and np.ndarray are supported")
-
-                # step_data[agent_id]['action'] = agent_data    # change from corl2.0 merge
+        step_data = self.extract_step_data(env)
 
         # ##################################################
         # # Append the episode's step information to our agent_data knowledge
         serialized_platforms = [self.platform_serializer().serialize(item) for item in env.state.sim_platforms.values()]
 
         # # Start our step artifact, the agent map will be filled out next
         step = EpisodeArtifact.Step(agents={}, platforms=serialized_platforms, environment_state=self.extract_environment_state(env.state))
@@ -247,23 +260,32 @@
                 filters=worker.filters[policy_id],
             )
         }
 
         worker_env: BaseCorlMultiAgentEnv | None = worker.env  # type: ignore
         if worker_env is None:
             raise RuntimeError("Worker.env is None, this is a non op")
+
+        if not isinstance(worker_env, BaseCorlMultiAgentEnv):
+            raise RuntimeError("The env not inherit BaseCorlMultiAgentEnv")
+
         if not isinstance(worker_env.simulator, BaseSimulator):
             raise RuntimeError("The simulator attached to the worker does not inherit BaseSimulator")
         frame_rate = worker_env.simulator.frame_rate
 
+        normalized_action_space = worker_env.action_space
+        normalized_observation_space = worker_env.observation_space
+        raw_action_space = getattr(worker_env, "_raw_action_space", worker_env.action_space)
+        raw_observation_space = getattr(worker_env, "_raw_observation_space", worker_env.observation_space)
+
         space_definitions = EpisodeArtifact.SpaceDefinitions(
-            action_space=worker_env._raw_action_space,  # type: ignore # noqa: SLF001
-            normalized_action_space=worker_env.action_space,  # type: ignore
-            observation_space=worker_env._raw_observation_space,  # type: ignore  # noqa: SLF001
-            normalized_observation_space=worker_env.observation_space,  # type: ignore
+            action_space=raw_action_space,
+            normalized_action_space=normalized_action_space,
+            observation_space=raw_observation_space,
+            normalized_observation_space=normalized_observation_space,
         )
 
         # If we have yet to generate the episode artifact for this episode then do it
         if "episode_artifact" not in episode.user_data:
             episode.user_data["episode_artifact"] = np.array(
                 [
                     EpisodeArtifact(
```

### Comparing `corl-3.14.13/corl/evaluation/runners/section_factories/engine/rllib/episode_artifact_logging_callback.py` & `corl-3.16.2/corl/evaluation/runners/section_factories/engine/rllib/episode_artifact_logging_callback.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,24 +10,23 @@
 import os
 import pickle
 from abc import abstractmethod
 from datetime import datetime
 from pathlib import Path
 
 import flatten_dict
-import gymnasium
 import numpy as np
 from ray.rllib import BaseEnv, RolloutWorker
 from ray.rllib.evaluation.episode_v2 import EpisodeV2
 from ray.rllib.models.preprocessors import get_preprocessor
 from ray.rllib.policy import Policy
 from ray.rllib.policy.sample_batch import SampleBatch
 from ray.rllib.utils.typing import AgentID, PolicyID
 
-from corl.environment.multi_agent_env import ACT3MultiAgentEnv
+from corl.environment.base_multi_agent_env import BaseCorlMultiAgentEnv
 from corl.evaluation.episode_artifact import EpisodeArtifact
 from corl.evaluation.runners.section_factories.engine.rllib.default_evaluation_callbacks import DefaultEvaluationCallbacks
 
 EPOCH_ZFILL = 6
 EVAL_CHECKPOINTS_SUBDIR = "eval_checkpoints"
 
 
@@ -158,45 +157,58 @@
             metrics for the episode.
         """
 
         # Don't need to run if we are not evaluating
         if not worker.config.in_evaluation:
             return
 
-        epoch = str(worker.config["training_iteration"]).zfill(EPOCH_ZFILL)
         env = base_env.get_sub_environments()[episode.env_id]
         done_string_list = []
         # Generate the filenames for trajectories
         for platform_name, done_dict in env.done_info.items():
             for done_name, done_state in done_dict.items():
                 if done_state:
                     done_string_list.extend([platform_name[0].upper(), done_name, str(done_state)])
         episode_counter_str = str(self._episode_counter).zfill(8)
         worker_index_str = str(worker.env_context.worker_index).zfill(3)
         done_string = "_".join(done_string_list)
         done_string = f"{episode_counter_str}-{worker_index_str}-{done_string}"
 
-        sub_directory = Path(worker._original_kwargs["log_dir"]) / "trajectories" / f"epoch_{epoch}"  # noqa: SLF001
+        log_artifacts_to_env_output_dir = worker.config.get("log_artifacts_to_env_output_dir", False)
+        if log_artifacts_to_env_output_dir:
+            sub_directory = Path(env.config.output_path)
+        else:
+            epoch = str(worker.config["training_iteration"]).zfill(EPOCH_ZFILL)
+            sub_directory = Path(worker._original_kwargs["log_dir"]) / "trajectories" / f"epoch_{epoch}"  # noqa: SLF001
+
         policy_artifact = {}
         for policy_id in policies:
             policy_artifact.update(
                 {
                     policy_id: EpisodeArtifact.PolicyArtifact(
                         preprocessor=get_preprocessor(env.observation_space)(env.observation_space), filters=worker.filters[policy_id]
                     )
                 }
             )
-        assert isinstance(worker.env, ACT3MultiAgentEnv)
-        assert isinstance(worker.env.action_space, gymnasium.spaces.Dict)
-        assert isinstance(worker.env.observation_space, gymnasium.spaces.Dict)
+
+        if worker.env is None or not isinstance(worker.env, BaseCorlMultiAgentEnv):
+            raise RuntimeError(
+                f"Invalid Environment - Env must not be None and must be of type BaseCorlMultiAgentEnv; got {type(worker.env)}"
+            )
+
+        normalized_action_space = worker.env.action_space
+        normalized_observation_space = worker.env.observation_space
+        raw_action_space = getattr(worker.env, "_raw_action_space", worker.env.action_space)
+        raw_observation_space = getattr(worker.env, "_raw_observation_space", worker.env.observation_space)
+
         space_definitions = EpisodeArtifact.SpaceDefinitions(
-            action_space=worker.env._raw_action_space,  # noqa: SLF001
-            normalized_action_space=worker.env.action_space,
-            observation_space=worker.env._raw_observation_space,  # noqa: SLF001
-            normalized_observation_space=worker.env.observation_space,
+            action_space=raw_action_space,
+            normalized_action_space=normalized_action_space,
+            observation_space=raw_observation_space,
+            normalized_observation_space=normalized_observation_space,
         )
         episode_artifact = EpisodeArtifact(
             test_case=episode.user_data["test_case"],
             env_config=episode.user_data["env_config"],
             artifacts_filenames=episode.user_data["episode_artifacts_filenames"],
             start_time=episode.user_data["start_time"],
             duration_sec=(datetime.now() - episode.user_data["start_time"]).total_seconds(),
```

### Comparing `corl-3.14.13/corl/evaluation/runners/section_factories/engine/rllib/eval_config_updates.py` & `corl-3.16.2/corl/evaluation/runners/section_factories/engine/rllib/eval_config_updates.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 This Module contains logic to update the rllib config appropriately for evaluation purposes.
 """
+
 from pathlib import Path
 
 from pydantic import BaseModel, ConfigDict
 
 from corl.evaluation.runners.section_factories.plugins.config_updater import ConfigUpdate
 from corl.evaluation.runners.section_factories.test_cases.test_case_manager import TestCaseStrategy
```

### Comparing `corl-3.14.13/corl/evaluation/runners/section_factories/engine/rllib/interruptable_callback.py` & `corl-3.16.2/corl/evaluation/runners/section_factories/engine/rllib/interruptable_callback.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 Callbacks to do logging of episodes
 """
+
 from ray.rllib import BaseEnv, RolloutWorker
 from ray.rllib.algorithms.callbacks import DefaultCallbacks
 from ray.rllib.evaluation.episode import Episode
 from ray.rllib.evaluation.episode_v2 import EpisodeV2
 from ray.rllib.policy import Policy
 from ray.rllib.utils.typing import PolicyID
```

### Comparing `corl-3.14.13/corl/evaluation/runners/section_factories/engine/rllib/rllib_trainer.py` & `corl-3.16.2/corl/evaluation/runners/section_factories/engine/rllib/rllib_trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 Configures a rllib trainer to run evaluation
 """
+
 import copy
 import dataclasses
 import logging
 from contextlib import contextmanager
 from pathlib import Path
 from typing import Annotated
```

### Comparing `corl-3.14.13/corl/evaluation/runners/section_factories/plugins/config_updater.py` & `corl-3.16.2/corl/evaluation/runners/section_factories/plugins/config_updater.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 from abc import ABC, abstractmethod
 
 
 class ConfigUpdate(ABC):
     """Abstract class to update a configuration"""
 
     @abstractmethod
```

### Comparing `corl-3.14.13/corl/evaluation/runners/section_factories/plugins/environment_state_extractor.py` & `corl-3.16.2/corl/evaluation/runners/section_factories/plugins/environment_state_extractor.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/evaluation/runners/section_factories/plugins/platform_serializer.py` & `corl-3.16.2/corl/evaluation/runners/section_factories/plugins/platform_serializer.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/evaluation/runners/section_factories/plugins/plugins.py` & `corl-3.16.2/corl/evaluation/runners/section_factories/plugins/plugins.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/evaluation/runners/section_factories/task.py` & `corl-3.16.2/corl/evaluation/runners/section_factories/task.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 Defines a task
 """
+
 import pathlib
 import warnings
 
 from pydantic import BaseModel, ConfigDict, Field, dataclasses, field_validator, model_validator
 
 from corl.environment.default_env_rllib_callbacks import DefaultCallbacks, EnvironmentDefaultCallbacks
 from corl.evaluation.runners.section_factories.teams import Teams
```

### Comparing `corl-3.14.13/corl/evaluation/runners/section_factories/teams.py` & `corl-3.16.2/corl/evaluation/runners/section_factories/teams.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 Configures teams to perform in evaluation
 """
+
 import typing
 from typing import Annotated
 
 from pydantic import BaseModel, BeforeValidator, ConfigDict
 
 import corl.evaluation.loader.i_agent_loader as agent_loader
 from corl.evaluation.evaluation_factory import FactoryLoader
```

### Comparing `corl-3.14.13/corl/evaluation/runners/section_factories/test_cases/__init__.py` & `corl-3.16.2/corl/evaluation/runners/section_factories/test_cases/__init__.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/evaluation/runners/section_factories/test_cases/base_network_strategy.py` & `corl-3.16.2/corl/evaluation/runners/section_factories/test_cases/base_network_strategy.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 import logging
 from abc import abstractmethod
 from typing import Any, TypeVar
 
 import pandas as pd
 from pydantic import field_validator
```

### Comparing `corl-3.14.13/corl/evaluation/runners/section_factories/test_cases/config_parser.py` & `corl-3.16.2/corl/evaluation/runners/section_factories/test_cases/config_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 Parse the evaluation configuration
 """
+
 import copy
 import typing
 from collections import abc
 
 # Lowest level of data read from the configuration file
 LOW_DATA = int | float | str
 LOW_DATA_SEQUENCE = typing.Sequence[LOW_DATA]
```

### Comparing `corl-3.14.13/corl/evaluation/runners/section_factories/test_cases/default_strategy.py` & `corl-3.16.2/corl/evaluation/runners/section_factories/test_cases/default_strategy.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 This module defines the TestCaseStrategy for running evaluation with the default EPPs defined in the task configs.
 
 Author: John McCarroll
 """
 
-
 from corl.evaluation.runners.section_factories.test_cases.test_case_manager import (
     TestCaseIndex,
     TestCaseStrategy,
     TestCaseStrategyValidator,
 )
```

### Comparing `corl-3.14.13/corl/evaluation/runners/section_factories/test_cases/pandas.py` & `corl-3.16.2/corl/evaluation/runners/section_factories/test_cases/pandas.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 Loads pandas test cases
 """
+
 import dataclasses
 import enum
 import logging
 import typing
 
 import jsonargparse
 import pandas as pd
```

### Comparing `corl-3.14.13/corl/evaluation/runners/section_factories/test_cases/tabular_strategy.py` & `corl-3.16.2/corl/evaluation/runners/section_factories/test_cases/tabular_strategy.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 This module defines the TestCaseStrategy for the TabularParameterProvider
 
 Author: John McCarroll
 """
 
-
 import pandas as pd
 from pydantic import BaseModel, ConfigDict
 
 from corl.evaluation.runners.section_factories.test_cases.pandas import Pandas
 from corl.evaluation.runners.section_factories.test_cases.test_case_manager import (
     TestCaseIndex,
     TestCaseStrategy,
```

### Comparing `corl-3.14.13/corl/evaluation/runners/section_factories/test_cases/test_case_generator.py` & `corl-3.16.2/corl/evaluation/runners/section_factories/test_cases/test_case_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 Generate test cases from configuration
 """
+
 import itertools
 import logging
 
 import pandas as pd
 from numpy.random import BitGenerator, Generator
 
 from corl.evaluation.eval_logger_name import EVAL_LOGGER_NAME
```

### Comparing `corl-3.14.13/corl/evaluation/runners/section_factories/test_cases/test_case_manager.py` & `corl-3.16.2/corl/evaluation/runners/section_factories/test_cases/test_case_manager.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/evaluation/scene_processors.py` & `corl-3.16.2/corl/evaluation/scene_processors.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 import dataclasses
 
 from corl.evaluation import metrics
 from corl.evaluation.episode_artifact import EpisodeArtifact
 from corl.evaluation.metrics.processors import Evaluation
 from corl.evaluation.metrics.scenario_alert_generators import ScenarioAlertGenerators
 from corl.evaluation.metrics.scenario_metric_generators import ScenarioMetricGenerators
```

### Comparing `corl-3.14.13/corl/evaluation/serialize_platforms.py` & `corl-3.16.2/corl/evaluation/serialize_platforms.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 This module contains logic to serialize different platforms
 """
 
-
 from corl.evaluation.runners.section_factories.plugins.platform_serializer import PlatformSerializer
 from corl.simulators.docking_1d.properties import PositionProp as Docking1dPos
 from corl.visualization.platform_plotting_deserializer import PlatformDeserializerPlotlyAnimation
 
 
 class serialize_Docking_1d(PlatformSerializer):
     """
```

### Comparing `corl-3.14.13/corl/evaluation/util/__init__.py` & `corl-3.16.2/corl/policies/base_policy.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,9 +4,16 @@
 Reinforcement Learning (RL) Core.
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
-Collection of methods to perform evaluation
 """
+
+from pydantic import BaseModel
+
+
+class BasePolicyValidator(BaseModel):
+    """
+    Base Policy Validator to subclass for Experiments subclassing BaseExperiment
+    """
```

### Comparing `corl-3.14.13/corl/evaluation/util/condition.py` & `corl-3.16.2/corl/evaluation/util/condition.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 import typing
 
 from pydantic import BaseModel, PrivateAttr
 
 from corl.libraries.factory import Factory
```

### Comparing `corl-3.14.13/corl/evaluation/util/storage.py` & `corl-3.16.2/corl/evaluation/util/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,15 @@
 
 
 class Storage(ABC):
     """
     Abstract class that defines an interface by which various kinds of storage can be utilized
     """
 
-    def __init__(self) -> None:
-        ...
+    def __init__(self) -> None: ...
 
     @abstractmethod
     def load_artifacts_location(self, config: dict[str, str]):
         """
         Load information about the locations of various artifacts
         """
```

### Comparing `corl-3.14.13/corl/evaluation/visualization/html_plots.py` & `corl-3.16.2/corl/evaluation/visualization/html_plots.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 Print a visualization to screen
 """
+
 import os
 import pathlib
 import typing
 
 import pandas as pd
 
 # from dash import Dash, dcc, html, Input, Output
```

### Comparing `corl-3.14.13/corl/evaluation/visualization/print.py` & `corl-3.16.2/corl/evaluation/visualization/print.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 Print a visualization to screen
 """
+
 import io
 import os
 
 from tabulate import tabulate
 
 from corl.evaluation import metrics
 from corl.evaluation.metrics.alerts import Alert
```

### Comparing `corl-3.14.13/corl/evaluation/visualization/visualization.py` & `corl-3.16.2/corl/evaluation/visualization/visualization.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 import pathlib
 import pickle
 from abc import abstractmethod
 from pathlib import Path
 
 from corl.evaluation.evaluation_artifacts import EvaluationArtifact_Metrics, EvaluationArtifact_Visualization
 from corl.evaluation.scene_processors import SceneProcessors
```

### Comparing `corl-3.14.13/corl/experiments/base_experiment.py` & `corl-3.16.2/corl/experiments/base_experiment.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/experiments/benchmark_experiment.py` & `corl-3.16.2/corl/experiments/benchmark_experiment.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,33 +6,37 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
+import contextlib
 import os
 import pathlib
 import time
 import typing
 
 import ray
 from pydantic import ConfigDict, ImportString, field_validator
-from pyinstrument import Profiler
 from ray.tune.registry import get_trainable_cls
 
 from corl.environment.default_env_rllib_callbacks import EnvironmentDefaultCallbacks
 from corl.environment.multi_agent_env import ACT3MultiAgentEnv, ACT3MultiAgentEnvValidator
 from corl.episode_parameter_providers import EpisodeParameterProvider
 from corl.episode_parameter_providers.remote import RemoteEpisodeParameterProvider
 from corl.experiments.base_experiment import BaseExperiment, BaseExperimentValidator, ExperimentFileParse
 from corl.libraries.factory import Factory
 from corl.parsers.yaml_loader import apply_patches
 from corl.policies.base_policy import BasePolicyValidator
 
+with contextlib.suppress(Exception):
+    from pyinstrument import Profiler
+
 
 class BenchmarkExperimentValidator(BaseExperimentValidator):
     """
     ray_config: dictionary to be fed into ray init, validated by ray init call
     env_config: environment configuration, validated by environment class
     rllib_configs: a dictionary
     Arguments:
```

### Comparing `corl-3.14.13/corl/experiments/export_setup_experiment.py` & `corl-3.16.2/corl/experiments/export_setup_experiment.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 import json
 import re
 import typing
 from collections import OrderedDict
 
 import flatten_dict
 import pandas as pd
```

### Comparing `corl-3.14.13/corl/experiments/rllib_experiment.py` & `corl-3.16.2/corl/experiments/rllib_experiment.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 import gc
 import importlib
 import logging
 import os
 import pathlib
 import re
 import socket
@@ -27,14 +28,15 @@
 from ray import tune
 from ray.rllib.algorithms.callbacks import DefaultCallbacks, make_multi_callbacks
 from ray.rllib.policy.policy import Policy
 from ray.tune.registry import get_trainable_cls, register_env
 
 import corl.experiments.rllib_utils.wrappers as rllib_wrappers
 from corl.environment.base_multi_agent_env import BaseCorlMultiAgentEnv
+from corl.environment.centralized_critic_environment import CorlCentralizedCriticEnvWrapper
 from corl.environment.default_env_rllib_callbacks import EnvironmentDefaultCallbacks
 from corl.environment.environment_wrappers import GroupedAgentsEnv
 from corl.environment.multi_agent_env import ACT3MultiAgentEnv
 from corl.episode_parameter_providers import EpisodeParameterProvider
 from corl.episode_parameter_providers.remote import RemoteEpisodeParameterProvider
 from corl.experiments.base_experiment import BaseExperiment, BaseExperimentValidator, ExperimentFileParse
 from corl.experiments.rllib_utils.policy_mapping_functions import PolicyIsAgent
@@ -256,14 +258,15 @@
                     Factory(**agent_configs.class_config.config["episode_parameter_provider"]), agent_name
                 )
         tmp_env: ACT3MultiAgentEnv = self.create_environment()
         self.config.env_config["epp_registry"] = tmp_env.config.epp_registry
         policies, train_policies, available_policies = self.create_policies(tmp_env)
 
         self._update_rllib_config(rllib_config, train_policies, policies, args, available_policies)
+
         self._update_tune_config()
 
         self._enable_episode_parameter_provider_checkpointing()
 
         search_class = None
         if self.config.hparam_search_class is not None:
             if self.config.hparam_search_config is not None:
@@ -319,15 +322,14 @@
 
     def _update_rllib_config(self, rllib_config, train_policies, policies, args: ExperimentFileParse, available_policies) -> None:
         """
         Update several rllib config fields
         tmp_ac: agent_classes from temporary environment to get obs/action space, these should be
                 considered read only, and will be destroyed when training begins
         """
-
         rllib_config["multiagent"] = {
             "policies": policies,
             "policy_mapping_fn": self.config.policy_mapping.functor(**self.config.policy_mapping.config),
             "policies_to_train": train_policies,
         }
 
         rllib_config["env"] = self.config.environment
@@ -356,16 +358,18 @@
                             print(f"Checkpoint hash for {agent_name} at {file_path}: {git_hash}")
                         restored = Policy.from_checkpoint(file_path)
                         agent_weight_dict[agent_name] = restored.get_weights()
                     algorithm.set_weights(agent_weight_dict)
                     algorithm.workers.sync_weights()
 
             callback_list.append(WeightLoaderCallback)
+
         if self.config.extra_callbacks:
             callback_list.extend(self.config.extra_callbacks)
+
         rllib_config["callbacks"] = make_multi_callbacks(callback_list)
         rllib_config["env_config"] = self.config.env_config
         now = datetime.now()
         rllib_config["env_config"]["output_date_string"] = f"{now.strftime('%Y%m%d_%H%M%S')}_{socket.gethostname()}"
         rllib_config["create_env_on_driver"] = True
 
         self._add_git_hashes_to_config(rllib_config)
@@ -450,14 +454,15 @@
 
     def get_callbacks(self) -> type[EnvironmentDefaultCallbacks]:  # noqa: PLR6301
         """Get the environment callbacks"""
         return EnvironmentDefaultCallbacks
 
     def _register_envs(self):  # noqa: PLR6301
         register_env("CorlMultiAgentEnv", lambda config: ACT3MultiAgentEnv(config))
+        register_env("CorlCentralizedCriticEnvWrapper", lambda config: CorlCentralizedCriticEnvWrapper(config))
         register_env("CorlGroupedAgentEnv", lambda config: GroupedAgentsEnv(config))
 
     def _select_rllib_config(self, platform: str | None) -> dict[str, typing.Any]:
         """Extract the rllib config for the proper computational platform
 
         Parameters
         ----------
```

### Comparing `corl-3.14.13/corl/experiments/rllib_utils/policy_mapping_functions.py` & `corl-3.16.2/corl/experiments/rllib_utils/policy_mapping_functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 policy mapping functions
 """
+
 from abc import abstractmethod
 
 from pydantic import BaseModel
 
 
-class PolicyMappingValidatorBase(BaseModel):
-    ...
+class PolicyMappingValidatorBase(BaseModel): ...
 
 
 class PolicyMappingBase:
     """Base class for policy mapping implementations"""
 
     def __init__(self, **kwargs) -> None:
         self.config = self.get_validator()(**kwargs)
```

### Comparing `corl-3.14.13/corl/experiments/rllib_utils/wrappers.py` & `corl-3.16.2/corl/experiments/rllib_utils/wrappers.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 from ray.tune.registry import ENV_CREATOR, _global_registry
 
 
 def get_rllib_environment_creator(env_specifier):
     """
     Returns CoRL environment
     """
```

### Comparing `corl-3.14.13/corl/glues/base_dict_wrapper.py` & `corl-3.16.2/corl/glues/base_dict_wrapper.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/glues/base_glue.py` & `corl-3.16.2/corl/glues/base_glue.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 The glue classes are modular in that you can use multiple glue classes per
 agent. This allows stacking a glue to a stick controller glue to get
 a and stick controlled agent. However, some control schemes may not be
 compatible with each other. For example if you try to add a pitch control with
 the stick and a pitch rate controller, the resulting behavior is not
 straightforward and may cause your backend to throw an error.
 """
+
 import abc
 import enum
 import logging
 import typing
 from collections import OrderedDict
 from functools import cached_property
```

### Comparing `corl-3.14.13/corl/glues/base_multi_wrapper.py` & `corl-3.16.2/corl/glues/base_multi_wrapper.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/glues/base_wrapper.py` & `corl-3.16.2/corl/glues/base_wrapper.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/glues/common/controller_glue.py` & `corl-3.16.2/corl/glues/common/controller_glue.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 Controller Glue
 """
+
 import logging
 from collections import OrderedDict
 from functools import cached_property
 
 from corl.glues.base_glue import BaseAgentControllerGlue, BaseAgentPlatformGlueValidator
 from corl.libraries.env_space_util import EnvSpaceUtil
 from corl.libraries.property import DictProp
```

### Comparing `corl-3.14.13/corl/glues/common/magnitude.py` & `corl-3.16.2/corl/glues/common/magnitude.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 
 Wrapper glue which returns the magnitude of its wrapped glue as an observation.
 
 Author: Jamie Cunningham
 """
+
 from collections import OrderedDict
 from functools import cached_property
 
 import numpy as np
 
 from corl.glues.base_wrapper import BaseWrapperGlue, BaseWrapperGlueValidator
 from corl.glues.common.observe_sensor import ObserveSensor
```

### Comparing `corl-3.14.13/corl/glues/common/observe_part_validity.py` & `corl-3.16.2/corl/glues/common/observe_part_validity.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/glues/common/observe_sensor.py` & `corl-3.16.2/corl/glues/common/observe_sensor.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/glues/common/observe_sensor_repeated.py` & `corl-3.16.2/corl/glues/common/observe_sensor_repeated.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 -------------
 ObserveSensorRepeated Glue
 """
+
 import typing
 from collections import OrderedDict
 from functools import cached_property
 
 import gymnasium
 
 from corl.glues.base_glue import BaseAgentPlatformGlue, BaseAgentPlatformGlueValidator
```

### Comparing `corl-3.14.13/corl/glues/common/projected_quantity.py` & `corl-3.16.2/corl/glues/common/projected_quantity.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 Sensors for GymnasiumSimulator
 """
+
 import typing
 from collections import OrderedDict
 from functools import cached_property
 
 import numpy as np
 
 from corl.glues.base_dict_wrapper import BaseDictWrapperGlue
```

### Comparing `corl-3.14.13/corl/glues/common/target_value.py` & `corl-3.16.2/corl/glues/common/target_value.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/glues/common/target_value_difference.py` & `corl-3.16.2/corl/glues/common/target_value_difference.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 import logging
 from collections import OrderedDict
 from functools import cached_property
 
 import numpy as np
 
 from corl.glues.base_dict_wrapper import BaseDictWrapperGlue, BaseDictWrapperGlueValidator
```

### Comparing `corl-3.14.13/corl/glues/common/trig_values.py` & `corl-3.16.2/corl/glues/common/trig_values.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 import math
 from collections import OrderedDict
 from functools import cached_property
 
 import gymnasium
 import numpy as np
```

### Comparing `corl-3.14.13/corl/glues/common/unit_vector_glue.py` & `corl-3.16.2/corl/glues/common/unit_vector_glue.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/glues/controller_wrappers/delta_controller.py` & `corl-3.16.2/corl/glues/controller_wrappers/delta_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 
 AvailablePlatforms
 """
+
 import logging
 import typing
 from collections import OrderedDict
 from functools import cached_property
 
 import numpy as np
 from gymnasium.spaces import Dict
```

### Comparing `corl-3.14.13/corl/glues/controller_wrappers/obs_relative_delta_controller.py` & `corl-3.16.2/corl/glues/controller_wrappers/obs_relative_delta_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 
 AvailablePlatforms
 """
+
 import logging
 import typing
 from collections import OrderedDict
 from functools import cached_property
 
 import numpy as np
 from gymnasium.spaces import Box, Dict
```

### Comparing `corl-3.14.13/corl/glues/controller_wrappers/obs_relative_delta_controller_dict.py` & `corl-3.16.2/corl/glues/controller_wrappers/obs_relative_delta_controller_dict.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 
 AvailablePlatforms
 """
+
 import logging
 import typing
 from collections import OrderedDict
 
 import gymnasium
 import numpy as np
 from pydantic import field_validator
```

### Comparing `corl-3.14.13/corl/libraries/algorithm_helper.py` & `corl-3.16.2/corl/libraries/algorithm_helper.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/libraries/cleanup.py` & `corl-3.16.2/corl/libraries/cleanup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 import typing
 
 
 def cleanup(fn: typing.Callable):
     """Returns an object that will call fn when it goes out of scope"""
 
     class ScopedDestructor:
```

### Comparing `corl-3.14.13/corl/libraries/collection_utils.py` & `corl-3.16.2/corl/libraries/collection_utils.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/libraries/config_file_watcher.py` & `corl-3.16.2/corl/libraries/config_file_watcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 
 Confi File Watcher Module
 """
+
 import logging
 import logging.config
 import os
 import pathlib
 import pprint
 from datetime import datetime
 from logging import FileHandler
```

### Comparing `corl-3.14.13/corl/libraries/context.py` & `corl-3.16.2/corl/libraries/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 from collections.abc import Iterator
 from contextlib import contextmanager
 from contextvars import ContextVar
 from typing import Any
 
 from pydantic import BaseModel
```

### Comparing `corl-3.14.13/corl/libraries/env_common.py` & `corl-3.16.2/corl/libraries/env_common.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/libraries/env_func_base.py` & `corl-3.16.2/corl/libraries/env_func_base.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/libraries/env_space_util.py` & `corl-3.16.2/corl/libraries/env_space_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 ENV Space Util Module
 
 this file is a mypy nightmare due to lots of typing unions and complex types
 do not trust mypy, trust the unit tests
 """
+
 import copy
 import logging
 import typing
 from collections import OrderedDict
 from collections.abc import MutableSequence
 
 import flatten_dict
```

### Comparing `corl-3.14.13/corl/libraries/environment_dict.py` & `corl-3.16.2/corl/libraries/environment_dict.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 Environment Dict Module
 """
+
 import abc
 import copy
 import logging
 import typing
 import warnings
 from collections import OrderedDict
```

### Comparing `corl-3.14.13/corl/libraries/factory.py` & `corl-3.16.2/corl/libraries/factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 from typing import Any
 
 from pydantic import BaseModel, ImportString, ValidationInfo
 
 
 def _construct(type_, info, **kwargs):
     if info and info.context:
```

### Comparing `corl-3.14.13/corl/libraries/file_path.py` & `corl-3.16.2/corl/libraries/file_path.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/libraries/functor.py` & `corl-3.16.2/corl/libraries/functor.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 from collections.abc import Mapping, Sequence
 from collections.abc import Mapping as Mapping_Type
 from typing import Annotated, Any, Literal, Union
 
 from pydantic import BaseModel, BeforeValidator, ConfigDict, Field, ImportString, StringConstraints, field_validator
 
 from corl.libraries.factory import Factory
```

### Comparing `corl-3.14.13/corl/libraries/hparam_search_util.py` & `corl-3.16.2/corl/libraries/hparam_search_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 -------------------------------------------------------------------------------
 """
+
 import abc
 import random
 from functools import partial
 
 from pydantic import BaseModel
 from ray import tune
```

### Comparing `corl-3.14.13/corl/libraries/nan_check.py` & `corl-3.16.2/corl/libraries/nan_check.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 -------------------------------------------------------------------------------
 
 NaN check module
 """
+
 import traceback
 
 import numpy as np
 
 from corl.libraries.units import Quantity
```

### Comparing `corl-3.14.13/corl/libraries/normalization.py` & `corl-3.16.2/corl/libraries/normalization.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 -------------------------------------------------------------------------------
 
 Normalizer
 """
+
 import abc
 import copy
 from collections import OrderedDict
 
 import gymnasium.spaces
 import numpy as np
 from pydantic import BaseModel, field_validator
```

### Comparing `corl-3.14.13/corl/libraries/observation_extractor.py` & `corl-3.16.2/corl/libraries/observation_extractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 -------------------------------------------------------------------------------
 
 Observation Extractor
 """
+
 import typing
 
 
 class ExtractorSet(typing.NamedTuple):
     """Class defining the set of extractors to pull information about a specific observation"""
 
     value: typing.Callable
```

### Comparing `corl-3.14.13/corl/libraries/observation_util.py` & `corl-3.16.2/corl/libraries/observation_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 from collections import OrderedDict
 from collections.abc import Callable
 
 import numpy as np
 
 ObsType = np.ndarray | tuple | dict
```

### Comparing `corl-3.14.13/corl/libraries/parameters.py` & `corl-3.16.2/corl/libraries/parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 -------------------------------------------------------------------------------
 
 Structures that hold parameters and the ability to update them.
 """
+
 import abc
 import typing
 import warnings
 from typing import runtime_checkable
 
 import numpy as np
 from numpy.random import Generator, RandomState
@@ -27,16 +28,15 @@
 Number = StrictInt | float
 Randomness = Generator | RandomState
 OtherVars = typing.Mapping[tuple[str, ...], Quantity]
 
 
 @runtime_checkable
 class _ConstraintCallbackType(Protocol):
-    def __call__(self, old_arg: Number, new_arg: Number) -> Number:
-        ...
+    def __call__(self, old_arg: Number, new_arg: Number) -> Number: ...
 
 
 class ParameterValidator(BaseModel):
     """Validator class for Parameter"""
 
     units: str = "dimensionless"
     update: dict[str, typing.Any] = {}
```

### Comparing `corl-3.14.13/corl/libraries/plugin_library.py` & `corl-3.16.2/corl/libraries/plugin_library.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 -------------------------------------------------------------------------------
 
 PluginLibrary.AddClassToGroup(CLASS, "NAME", {"simulator": INTEGRATION_CLASS, "platform_type": AvailablePlatformTypes.XXXX})
 """
+
 import importlib
 import inspect
 import itertools
 import pkgutil
 import sys
 import typing
 from traceback import print_tb
```

### Comparing `corl-3.14.13/corl/libraries/property.py` & `corl-3.16.2/corl/libraries/property.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 Property Module
 """
+
 import abc
 import typing
 from collections.abc import KeysView
 from typing import TypeAlias
 
 import gymnasium.spaces
 import numpy as np
```

### Comparing `corl-3.14.13/corl/libraries/space_transformations.py` & `corl-3.16.2/corl/libraries/space_transformations.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 ENV Space Util Module
 
 this file is a mypy nightmare due to lots of typing unions and complex types
 do not trust mypy, trust the unit tests
 """
+
 import abc
 from typing import Annotated
 
 import gymnasium
 from pydantic import AfterValidator, BaseModel, ImportString
 
 from corl.libraries.env_space_util import EnvSpaceUtil, convert_gymnasium_space, convert_sample
```

### Comparing `corl-3.14.13/corl/libraries/state_dict.py` & `corl-3.16.2/corl/libraries/state_dict.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 state Dict - Leverage https://github.com/ramazanpolat/StateDict -
 """
+
 import copy
 from collections import OrderedDict
 
 DICT_RESERVED_KEYS = vars(OrderedDict).keys()
 
 
 class StateDict(OrderedDict):
```

### Comparing `corl-3.14.13/corl/libraries/units.py` & `corl-3.16.2/corl/libraries/units.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/libraries/utils.py` & `corl-3.16.2/corl/libraries/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """ non grouped utils
 """
+
 import math
 import typing
 from string import digits
 
 from corl.libraries.units import Quantity, corl_quantity
```

### Comparing `corl-3.14.13/corl/libraries/value_function.py` & `corl-3.16.2/corl/libraries/value_function.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/models/frame_stacking.py` & `corl-3.16.2/corl/models/frame_stacking.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 The following module contains the implementation for the  stacked observation
 """
+
 import gymnasium
 import numpy as np
 from ray.rllib.models import ModelCatalog
 from ray.rllib.models.tf.misc import normc_initializer
 from ray.rllib.models.tf.tf_modelv2 import TFModelV2
 from ray.rllib.models.utils import get_activation_fn
 from ray.rllib.policy.view_requirement import ViewRequirement
```

### Comparing `corl-3.14.13/corl/models/torch_frame_stack.py` & `corl-3.16.2/corl/models/torch_frame_stack.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/parsers/agent_and_platform.py` & `corl-3.16.2/corl/parsers/agent_and_platform.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 from pathlib import Path
 from typing import Annotated, Any
 
 from pydantic import BaseModel, BeforeValidator
 
 from corl.parsers.yaml_loader import load_file
```

### Comparing `corl-3.14.13/corl/parsers/yaml_loader.py` & `corl-3.16.2/corl/parsers/yaml_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 import collections
 import copy
 import json
 import os
 from pathlib import Path
 from typing import IO, Any
 from urllib.parse import unquote, urlparse
```

### Comparing `corl-3.14.13/corl/parts/comms.py` & `corl-3.16.2/corl/parts/comms.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/parts/memory_store.py` & `corl-3.16.2/corl/parts/memory_store.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/policies/custom_policy.py` & `corl-3.16.2/corl/policies/custom_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 Custom Policy
 """
+
 from abc import abstractmethod
 from collections import defaultdict
 
 import flatten_dict
 import gymnasium
 import numpy as np
 from pydantic import ConfigDict, model_validator
```

### Comparing `corl-3.14.13/corl/policies/random_action.py` & `corl-3.16.2/corl/policies/random_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 Module with base implementations for Observations
 """
+
 from collections import defaultdict
 
 import flatten_dict
 import numpy as np
 from ray.rllib.policy import Policy
 from ray.rllib.policy.sample_batch import SampleBatch
```

### Comparing `corl-3.14.13/corl/policies/scripted_action.py` & `corl-3.16.2/corl/policies/scripted_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 Scripted Action Policy
 """
+
 import typing
 
 import flatten_dict
 import numpy as np
 from pydantic import ConfigDict, field_validator, model_validator
 
 from corl.libraries.env_space_util import EnvSpaceUtil
```

### Comparing `corl-3.14.13/corl/rewards/base_measurement_operation.py` & `corl-3.16.2/corl/rewards/base_measurement_operation.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 Module with base implementations for Observations
 """
+
 from __future__ import annotations
 
 import logging
 
 import numpy as np
 from pydantic import BaseModel
```

### Comparing `corl-3.14.13/corl/rewards/docking_1d/docking_distance_change_reward.py` & `corl-3.16.2/corl/rewards/docking_1d/docking_distance_change_reward.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/rewards/docking_1d/docking_reward.py` & `corl-3.16.2/corl/rewards/docking_1d/docking_reward.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/rewards/episode_done.py` & `corl-3.16.2/corl/rewards/episode_done.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 Reward that uses episode state to accumulate reward"""
+
 import abc
 import enum
 import typing
 from collections import OrderedDict
 from functools import partial
 from typing import Annotated
```

### Comparing `corl-3.14.13/corl/rewards/exponential_decay_from_target_value.py` & `corl-3.16.2/corl/rewards/exponential_decay_from_target_value.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/rewards/gymnasium_reward.py` & `corl-3.16.2/corl/rewards/gymnasium_reward.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 Reward for GymnasiumSimulator
 """
+
 from corl.rewards.reward_func_base import RewardFuncBase
 
 
 class GymnasiumReward(RewardFuncBase):
     """
     Reward for GymnasiumSimulator that rewards the reward
     coming from the simulator provided state and reports it
```

### Comparing `corl-3.14.13/corl/rewards/multi_measurement_operation.py` & `corl-3.16.2/corl/rewards/multi_measurement_operation.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 Module with implementation for multiple Observations
 """
+
 import logging
 
 from corl.rewards.base_measurement_operation import ExtractorSet, ObservationExtractorValidator
 from corl.rewards.reward_func_base import RewardFuncBase, RewardFuncBaseValidator
 
 
 class MultiMeasurementOperationValidator(RewardFuncBaseValidator):
```

### Comparing `corl-3.14.13/corl/rewards/reward_func_base.py` & `corl-3.16.2/corl/rewards/reward_func_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 Reward Functor Base Module
 """
+
 import abc
 from collections import OrderedDict
 
 import gymnasium
 from pydantic import BaseModel
 
 from corl.libraries.env_func_base import EnvFuncBase
@@ -50,16 +51,15 @@
         observation: OrderedDict,
         action,
         next_observation: OrderedDict,
         state: BaseSimulatorState,
         next_state: BaseSimulatorState,
         observation_space: gymnasium.Space,
         observation_units: OrderedDict,
-    ) -> float:
-        ...
+    ) -> float: ...
 
     def post_process_trajectory(self, agent_id, state, batch, episode, policy):
         """Allows the user to modify the trajectory of the episode
         in the batch collected during an rllib callback. WARNING: This function is dangerous
         you can completely destroy training using this
         Use it only as a last resort
         """
```

### Comparing `corl-3.14.13/corl/rewards/reward_func_dict_wrapper.py` & `corl-3.16.2/corl/rewards/reward_func_dict_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 import abc
 from collections import OrderedDict
 
 import gymnasium
 from pydantic import ConfigDict
 
 from corl.rewards.reward_func_base import RewardFuncBase, RewardFuncBaseValidator
@@ -49,9 +50,8 @@
         observation: OrderedDict,
         action,
         next_observation: OrderedDict,
         state: BaseSimulatorState,
         next_state: BaseSimulatorState,
         observation_space: gymnasium.Space,
         observation_units: OrderedDict,
-    ) -> float:
-        ...
+    ) -> float: ...
```

### Comparing `corl-3.14.13/corl/rewards/reward_func_multi_wrapper.py` & `corl-3.16.2/corl/rewards/reward_func_multi_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 import abc
 from collections import OrderedDict
 
 import gymnasium
 from pydantic import ConfigDict
 
 from corl.rewards.reward_func_base import RewardFuncBase, RewardFuncBaseValidator
@@ -49,9 +50,8 @@
         observation: OrderedDict,
         action,
         next_observation: OrderedDict,
         state: BaseSimulatorState,
         next_state: BaseSimulatorState,
         observation_space: gymnasium.Space,
         observation_units: OrderedDict,
-    ) -> float:
-        ...
+    ) -> float: ...
```

### Comparing `corl-3.14.13/corl/rewards/reward_func_wrapper.py` & `corl-3.16.2/corl/rewards/reward_func_wrapper.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 import abc
 from collections import OrderedDict
 
 import gymnasium
 from pydantic import ConfigDict
 
 from corl.rewards.reward_func_base import RewardFuncBase, RewardFuncBaseValidator
@@ -49,9 +50,8 @@
         observation: OrderedDict,
         action,
         next_observation: OrderedDict,
         state: BaseSimulatorState,
         next_state: BaseSimulatorState,
         observation_space: gymnasium.Space,
         observation_units: OrderedDict,
-    ) -> float:
-        ...
+    ) -> float: ...
```

### Comparing `corl-3.14.13/corl/simulators/base_parts.py` & `corl-3.16.2/corl/simulators/base_parts.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 the BasePlatform.
 
 To differentiate from the agent properties, base integration nomenclature uses control and
 measurements for the base parts, in contrast to the nomenclature of the agent which is usually
 action and observation. In this sense actions are made up of controls, and observations are
 made up of measurements.
 """
+
 from __future__ import annotations
 
 import abc
 import numbers
 import typing
 import warnings
 from operator import attrgetter
```

### Comparing `corl-3.14.13/corl/simulators/base_platform.py` & `corl-3.16.2/corl/simulators/base_platform.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 Base Platform Abstract Class Object
 """
+
 import abc
 
 from pydantic import BaseModel, ConfigDict
 
 from corl.simulators.base_parts import BaseController, BaseSensor
```

### Comparing `corl-3.14.13/corl/simulators/base_platform_type.py` & `corl-3.16.2/corl/simulators/base_platform_type.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/simulators/base_properties.py` & `corl-3.16.2/corl/simulators/base_properties.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 property definitions for sensors
 """
+
 from typing import Annotated
 
 import numpy as np
 from pydantic import Field, StrictFloat, StrictStr
 
 from corl.libraries.property import BoxProp, DiscreteProp
```

### Comparing `corl-3.14.13/corl/simulators/base_simulator.py` & `corl-3.16.2/corl/simulators/base_simulator.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/simulators/base_simulator_state.py` & `corl-3.16.2/corl/simulators/base_simulator_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
 
-
 from pydantic import BaseModel, Extra
 
 
 class BaseSimulatorState(BaseModel, extra=Extra.forbid):
     """
     Pydantic model containing a BaseClass for the state a simulator should return
     Other simulators may subclass this to return custom information
```

### Comparing `corl-3.14.13/corl/simulators/common_platform_utils.py` & `corl-3.16.2/corl/simulators/common_platform_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 -------------------------------------------------------------------------------
 
 Common Platform Utils Module
 """
+
 import typing
 
 from corl.simulators.base_parts import BaseController, BasePlatformPart, BaseSensor
 from corl.simulators.base_platform import BasePlatform
 from corl.simulators.base_simulator import BaseSimulatorState
```

### Comparing `corl-3.14.13/corl/simulators/docking_1d/available_platforms.py` & `corl-3.16.2/corl/simulators/docking_1d/available_platforms.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/simulators/docking_1d/controllers.py` & `corl-3.16.2/corl/simulators/docking_1d/controllers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """
 This module defines the controller used by the agent to interact with its environment.
 """
 
-
 from corl.libraries.plugin_library import PluginLibrary
 from corl.libraries.units import Quantity
 from corl.simulators.base_parts import BaseController
 from corl.simulators.docking_1d.available_platforms import Docking1dAvailablePlatformType
 from corl.simulators.docking_1d.properties import ThrustProp
 from corl.simulators.docking_1d.simulator import Docking1dSimulator
```

### Comparing `corl-3.14.13/corl/simulators/docking_1d/entities.py` & `corl-3.16.2/corl/simulators/docking_1d/entities.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/simulators/docking_1d/platform.py` & `corl-3.16.2/corl/simulators/docking_1d/platform.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 This module extends corl.simulators.base_platform.BasePlatform to create a simple one dimensional
 docking platform.
 """
 
-
 import numpy as np
 
 from corl.libraries.units import corl_get_ureg
 from corl.simulators.base_platform import BasePlatform, BasePlatformValidator
 from corl.simulators.docking_1d.entities import Deputy1D
```

### Comparing `corl-3.14.13/corl/simulators/docking_1d/properties.py` & `corl-3.16.2/corl/simulators/docking_1d/properties.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/simulators/docking_1d/sensors.py` & `corl-3.16.2/corl/simulators/docking_1d/sensors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 This module contains implementations of Sensors that reside on the Docking1dPlatform.
 """
+
 from corl.libraries.plugin_library import PluginLibrary
 from corl.libraries.units import Quantity, corl_get_ureg
 from corl.simulators.base_parts import BaseSensor
 from corl.simulators.docking_1d.available_platforms import Docking1dAvailablePlatformType
 from corl.simulators.docking_1d.properties import PositionProp, VelocityProp
 from corl.simulators.docking_1d.simulator import Docking1dSimulator
```

### Comparing `corl-3.14.13/corl/simulators/docking_1d/simulator.py` & `corl-3.16.2/corl/simulators/docking_1d/simulator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 This module defines the Docking1dSimulator class which maintains environment objects (platforms and entities)
 and progresses a simulated training episode via the step() method.
 """
 
-
 import numpy as np
 
 from corl.libraries.plugin_library import PluginLibrary
 from corl.simulators.base_simulator import BaseSimulator, BaseSimulatorResetValidator, BaseSimulatorState, BaseSimulatorValidator
 from corl.simulators.docking_1d.entities import Deputy1D
 from corl.simulators.docking_1d.platform import Docking1dPlatform
```

### Comparing `corl-3.14.13/corl/simulators/gymnasium/gymnasium_available_platforms.py` & `corl-3.16.2/corl/simulators/gymnasium/gymnasium_available_platforms.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 Provides AvailablePlatformTypes for the Open ML Gymnasium Simulator
 """
+
 from __future__ import annotations
 
 from corl.libraries.plugin_library import PluginLibrary
 from corl.simulators.base_platform_type import BasePlatformType
 from corl.simulators.gymnasium.gymnasium_simulator import GymnasiumSimulator
```

### Comparing `corl-3.14.13/corl/simulators/gymnasium/gymnasium_controllers.py` & `corl-3.16.2/corl/simulators/gymnasium/gymnasium_controllers.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/simulators/gymnasium/gymnasium_sensors.py` & `corl-3.16.2/corl/simulators/gymnasium/gymnasium_sensors.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 Sensors for GymnasiumSimulator
 """
+
 # mypy really does not like the dynamic properties and dies on them,
 # this file must be excluded from linting
 # mypy: ignore-errors
 
 
 import numpy as np
 from numpy_ringbuffer import RingBuffer
```

### Comparing `corl-3.14.13/corl/simulators/gymnasium/gymnasium_simulator.py` & `corl-3.16.2/corl/simulators/gymnasium/gymnasium_simulator.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 Base Simulator and Platform for Toy OpenAI Environments
 This mainly shows a "how to use example" and provide an setup to unit test with
 """
+
 import typing
 from functools import cached_property
 
 import gymnasium
 from pydantic import BaseModel, ImportString
 
 from corl.libraries.plugin_library import PluginLibrary
```

### Comparing `corl-3.14.13/corl/simulators/pong/available_platforms.py` & `corl-3.16.2/corl/simulators/pong/available_platforms.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/simulators/pong/controllers.py` & `corl-3.16.2/corl/simulators/pong/controllers.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/simulators/pong/heuristic_paddle_policy.py` & `corl-3.16.2/corl/simulators/pong/heuristic_paddle_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 from enum import Enum
 
 from ray.rllib.evaluation.episode_v2 import EpisodeV2
 from ray.rllib.utils.typing import TensorStructType, TensorType
 
 from corl.policies.custom_policy import CustomPolicy, CustomPolicyValidator
```

### Comparing `corl-3.14.13/corl/simulators/pong/paddle_platform.py` & `corl-3.16.2/corl/simulators/pong/paddle_platform.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/simulators/pong/play_pickled_episode.py` & `corl-3.16.2/corl/simulators/pong/play_pickled_episode.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/simulators/pong/pong.py` & `corl-3.16.2/corl/simulators/pong/pong.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 Pong Game
 This class implements pong and is independing of RL based on
 https://github.com/techwithtim/Pong-Python
 """
+
 from enum import Enum
 
 import pygame
 from pydantic import BaseModel, ConfigDict
 
 
 class Colors(Enum):
```

### Comparing `corl-3.14.13/corl/simulators/pong/sensors.py` & `corl-3.16.2/corl/simulators/pong/sensors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 This module contains implementations of Sensors that reside on the Docking1dPlatform.
 """
+
 from typing import Annotated
 
 import numpy as np
 from pydantic import Field, StrictFloat
 
 from corl.libraries.plugin_library import PluginLibrary
 from corl.libraries.property import BoxProp, DiscreteProp
```

### Comparing `corl-3.14.13/corl/simulators/pong/simulator.py` & `corl-3.16.2/corl/simulators/pong/simulator.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 Base Simulator and Platform for Toy Openai Environments
 This mainly shows a "how to use example" and provide an setup to unit test with
 """
+
 import typing
 
 from corl.libraries.plugin_library import PluginLibrary
 from corl.libraries.units import Quantity
 from corl.simulators.base_simulator import (
     AgentConfig,
     BaseSimulator,
```

### Comparing `corl-3.14.13/corl/simulators/six_dof/base_six_dof_controllers.py` & `corl-3.16.2/corl/simulators/six_dof/base_six_dof_controllers.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 Base Integration Controls Module
 """
+
 import abc
 
 from corl.simulators.base_parts import BaseController
 
 
 class BaseRollPitchYawSpeedController(BaseController, abc.ABC):
     """
```

### Comparing `corl-3.14.13/corl/simulators/six_dof/base_six_dof_platform.py` & `corl-3.16.2/corl/simulators/six_dof/base_six_dof_platform.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 Abstraction Class for 6DOF platform types that can provide
 some properties for common usage
 """
+
 import abc
 
 import corl.simulators.six_dof.base_six_dof_properties as six_dof_props
 from corl.libraries.units import Quantity
 from corl.simulators.base_platform import BasePlatform
```

### Comparing `corl-3.14.13/corl/simulators/six_dof/base_six_dof_properties.py` & `corl-3.16.2/corl/simulators/six_dof/base_six_dof_properties.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 property definitions
 """
+
 from typing import Annotated
 
 import numpy as np
 from pydantic import Field, StrictFloat, StrictStr
 
 from corl.libraries.property import BoxProp
```

### Comparing `corl-3.14.13/corl/test_utils/full_training.py` & `corl-3.16.2/corl/test_utils/full_training.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/train_rl.py` & `corl-3.16.2/corl/train_rl.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 import argparse
 import logging
 import pathlib
 import typing
 import warnings
 
 import numpy as np
```

### Comparing `corl-3.14.13/corl/visualization/base_animator.py` & `corl-3.16.2/corl/visualization/base_animator.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 Base animator class for streamlit application.
 """
+
 from abc import ABC, abstractmethod
 from typing import TypeVar
 
 import matplotlib.colors as mcolors
 import numpy as np
 import pandas as pd
 import plotly.graph_objects as go
```

### Comparing `corl-3.14.13/corl/visualization/docking_animator.py` & `corl-3.16.2/corl/visualization/docking_animator.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/visualization/episode_artifact_to_tables.py` & `corl-3.16.2/corl/visualization/episode_artifact_to_tables.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/visualization/network_explainability/env_policy_transforms.py` & `corl-3.16.2/corl/visualization/network_explainability/env_policy_transforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,24 +261,22 @@
             self.get_raw_observations(agent_id=agent_id, episode_artifact=episode_artifact, include_initial_state=include_initial_state)
         )
         policy_artifact: EpisodeArtifact.PolicyArtifact = episode_artifact.policy_artifact[agent_id]
         _agent = self.env.agent_dict[agent_id]
         for idx, obs in enumerate(raw_observations):
             array_obs = self._get_transformed_obs(
                 _agent.create_training_observations(obs),
-                preprocessor=get_preprocessor(self.env.observation_space[agent_id])(self.env.observation_space[agent_id]),  # type: ignore
+                preprocessor=get_preprocessor(self.env.observation_space[agent_id])(self.env.observation_space[agent_id]),
                 policy_filter=policy_artifact.filters,
             )
             batch_obs.append(array_obs)
             if idx == 0:
                 self._get_policy_input_observation_names(
                     input_obs=array_obs,
-                    preprocessor=get_preprocessor(self.env.observation_space[agent_id])(  # type: ignore
-                        self.env.observation_space[agent_id]  # type: ignore
-                    ),
+                    preprocessor=get_preprocessor(self.env.observation_space[agent_id])(self.env.observation_space[agent_id]),
                 )
         view_requirements = self.policies[agent_id].model.view_requirements
         sample_batch_list = []
 
         collector = AgentCollector(view_reqs=view_requirements, max_seq_len=1, is_training=False)
         for idx, one_batch in enumerate(batch_obs):
             # Adds an observation to the buffer, the rest of the inputs are dummy variables
```

### Comparing `corl-3.14.13/corl/visualization/network_explainability/network_explainability.py` & `corl-3.16.2/corl/visualization/network_explainability/network_explainability.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/visualization/network_explainability/network_explainability_plotter.py` & `corl-3.16.2/corl/visualization/network_explainability/network_explainability_plotter.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/visualization/platform_plotting_deserializer.py` & `corl-3.16.2/corl/visualization/platform_plotting_deserializer.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 from abc import ABC, abstractmethod
 
 
 class PlatformDeserializerPlotlyAnimation(ABC):
     """Abstract class to define how to deserialize a platform for plotting"""
 
     @abstractmethod
```

### Comparing `corl-3.14.13/corl/visualization/plotly_animator.py` & `corl-3.16.2/corl/visualization/plotly_animator.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 Trajectory Animation Class
 """
+
 from collections.abc import Callable
 from typing import Any
 
 import numpy as np
 import pandas as pd
 import plotly.graph_objects as go
 import tqdm
```

### Comparing `corl-3.14.13/corl/visualization/pong_animator.py` & `corl-3.16.2/corl/visualization/pong_animator.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/visualization/streamlit_app/default_layout.py` & `corl-3.16.2/corl/visualization/streamlit_app/default_layout.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 Default layout for streamlit application
 """
+
 from collections.abc import Callable
 from pathlib import Path
 
 import plotly.express as px
 import stqdm
 import streamlit as st
 from pydantic import validate_call
```

### Comparing `corl-3.14.13/corl/visualization/streamlit_app/eval_while_train_layout.py` & `corl-3.16.2/corl/visualization/streamlit_app/eval_while_train_layout.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 Layout for visualizing evaluations generated from training.
 """
+
 import pickle
 from collections.abc import Callable
 
 import streamlit as st
 from pydantic import validate_call
 
 from corl.evaluation.recording.folder import FolderRecord
```

### Comparing `corl-3.14.13/corl/visualization/streamlit_app/pages/02_evaluation_from_training.py` & `corl-3.16.2/corl/visualization/streamlit_app/pages/02_evaluation_from_training.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 Evaluation from Training
 """
+
 import streamlit as st
 
 from corl.evaluation.recording.folder import EpisodeArtifactLoggingCallbackLoader
 from corl.visualization.streamlit_app.eval_while_train_layout import StreamlitPageEvaluationWhileTraining
 
 if __name__ == "__main__":
     st.set_page_config(layout="wide")
```

### Comparing `corl-3.14.13/corl/visualization/streamlit_app/pages/03_corl_evaluation.py` & `corl-3.16.2/corl/visualization/streamlit_app/pages/03_corl_evaluation.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 Corl Evaluation
 """
+
 import streamlit as st
 
 from corl.evaluation.recording.folder import FolderRecord
 from corl.visualization.streamlit_app.default_layout import DefaultStreamlitPage
 
 if __name__ == "__main__":
     st.set_page_config(layout="wide")
```

### Comparing `corl-3.14.13/corl/visualization/streamlit_app/pages/04_policy_network_viz.py` & `corl-3.16.2/corl/visualization/streamlit_app/pages/04_policy_network_viz.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 Policy Network Visualization
 """
+
 import streamlit as st
 
 from corl.evaluation.recording.folder import EpisodeArtifactLoggingCallbackLoader, FolderRecord
 from corl.visualization.streamlit_app.default_layout import DefaultStreamlitPage
 from corl.visualization.streamlit_app.eval_while_train_layout import StreamlitPageEvaluationWhileTraining
 
 if __name__ == "__main__":
```

### Comparing `corl-3.14.13/corl/visualization/streamlit_app/sections/agent_steps.py` & `corl-3.16.2/corl/visualization/streamlit_app/sections/agent_steps.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/visualization/streamlit_app/sections/platform_and_agent_dones.py` & `corl-3.16.2/corl/visualization/streamlit_app/sections/platform_and_agent_dones.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/visualization/streamlit_app/sections/trajectory_animation.py` & `corl-3.16.2/corl/visualization/streamlit_app/sections/trajectory_animation.py`

 * *Files identical despite different names*

### Comparing `corl-3.14.13/corl/visualization/streamlit_app/sections/units_conversion.py` & `corl-3.16.2/corl/visualization/streamlit_app/sections/units_conversion.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,19 +135,21 @@
 
         dataframe["_prev_units"] = dataframe["units"].copy()
 
         dataframe["units"] = dataframe.apply(lambda row: new_units_map.get(row["attribute_name"], row["units"]), axis=1)
         for column in ["min", "max"]:
             # Convert the "normalized columns" that have not been normalized when units exist
             dataframe[f"normalized_{column}"] = dataframe.apply(
-                lambda row, column=column: apply_unit_conversion_to_row(row, "normalized_", column)
-                # Only performs conversions when the normalized
-                # and unnormalized columns match and units exist
-                if row["min"] == row["normalized_min"] and row["max"] == row["normalized_max"] and row["_prev_units"]
-                else row[f"normalized_{column}"],
+                lambda row, column=column: (
+                    apply_unit_conversion_to_row(row, "normalized_", column)
+                    # Only performs conversions when the normalized
+                    # and unnormalized columns match and units exist
+                    if row["min"] == row["normalized_min"] and row["max"] == row["normalized_max"] and row["_prev_units"]
+                    else row[f"normalized_{column}"]
+                ),
                 axis=1,
             )
             # Converts the unnormalized columns. NOTE: this must go after the normalized column.
             dataframe[column] = dataframe.apply(
                 lambda row, column=column: apply_unit_conversion_to_row(row, "", column) if row["_prev_units"] else row[column], axis=1
             )
```

### Comparing `corl-3.14.13/corl/visualization/streamlit_app/streamlit_app.py` & `corl-3.16.2/corl/visualization/streamlit_app/streamlit_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 Entrypoint for Streamlit App
 """
+
 import jsonargparse
 import streamlit as st
 
 from corl.parsers.yaml_loader import load_file
 from corl.visualization.streamlit_app.default_layout import DefaultStreamlitPage, Functor
```

### Comparing `corl-3.14.13/corl/visualization/streamlit_app/utils.py` & `corl-3.16.2/corl/visualization/streamlit_app/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 ---------------------------------------------------------------------------
 
 This is a US Government Work not subject to copyright protection in the US.
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 """
+
 import pickle
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
 import streamlit as st
 import yaml
```

### Comparing `corl-3.14.13/pyproject.toml` & `corl-3.16.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "corl"
-version = "3.14.13"
+version = "3.16.2"
 description = "Core ACT3 Reinforcement Learning (RL) Library - Core framework and base implementations of common things such as controllers, glues, observes, sensors, evaluation, and etc"
 authors = [
     "Benjamin K Heiner <benjamin.heiner@us.af.mil>",
     "Brian Stieber <bstieber@toyon.com>",
     "Cameron Long <clong@toyon.com>",
     "Joshua Blackburn <joshua.blackburn@stresearch.com>",
     "Steven Fierro <sfierro@toyon.com>",
@@ -58,14 +58,15 @@
 codetiming = "^1.4.0"
 fastapi = "^0.104.1"
 uvicorn = "^0.24.0.post1"
 tensorflow = "2.15.0"
 # this is required on python 3.11 as it is not properly installed for some reason
 async_timeout = "^4.0.3"
 tensorflow-probability = "^0.23.0"
+jsonlines = "^4.0.0"
 
 [tool.poetry.dev-dependencies]
 pre-commit = "^2.20.0"
 pre-commit-hooks = "^4.3.0"
 types-PyYAML = "5.4.11"
 rope = "0.19.0"
 jupyter-core = "<5.0"
@@ -128,14 +129,15 @@
 termynal = ">=0.11.1"
 markdown_exec = ">=1.7.0"
 anybadge = ">=1.14.0"
 mkdocs-page-pdf = ">=0.1.1"
 # mkdocs-print-site-plugin = ">=2.3.6"
 mike = ">=2.0.0"
 fuzzywuzzy = ">=0.18.0"
+# Levenshtein = ">=0.25.1"
 
 [tool.poetry.group.pipeline.dependencies]
 twine = "^4.0.2"
 coverage-badge = "^1.1.0"
 pylint-gitlab = "^1.2.0"
 
 [build-system]
@@ -256,15 +258,14 @@
 
 [tool.ruff.isort]
 split-on-trailing-comma = false
 
 [tool.ruff.flake8-unused-arguments]
 ignore-variadic-names = true
 
-
 #################
 # mypy sections #
 #################
 # For a list of configurations go to https://mypy.readthedocs.io/en/stable/config_file.html
 [tool.mypy]
 plugins = "pydantic.mypy"
 ignore_missing_imports = true
```

### Comparing `corl-3.14.13/PKG-INFO` & `corl-3.16.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corl
-Version: 3.14.13
+Version: 3.16.2
 Summary: Core ACT3 Reinforcement Learning (RL) Library - Core framework and base implementations of common things such as controllers, glues, observes, sensors, evaluation, and etc
 Home-page: https://github.com/act3-ace/CoRL
 Keywords: Deep,Reinforcement,Learning,CoRL,act3,ACT3
 Author: Benjamin K Heiner
 Author-email: benjamin.heiner@us.af.mil
 Maintainer: Benjamin K Heiner
 Maintainer-email: benjamin.heiner@us.af.mil
@@ -18,14 +18,15 @@
 Requires-Dist: codetiming (>=1.4.0,<2.0.0)
 Requires-Dist: deepmerge (==0.3.0)
 Requires-Dist: fastapi (>=0.104.1,<0.105.0)
 Requires-Dist: flatten-dict (==0.4.1)
 Requires-Dist: gymnasium (==0.28.1)
 Requires-Dist: h5py (>=3.7)
 Requires-Dist: jsonargparse[argcomplete,signatures] (>=4,<5)
+Requires-Dist: jsonlines (>=4.0.0,<5.0.0)
 Requires-Dist: matplotlib (>=3.7.2,<4.0.0)
 Requires-Dist: numpy (>=1.24.0,<2.0.0)
 Requires-Dist: numpy-ringbuffer (>=0.2.2,<0.3.0)
 Requires-Dist: plotly (>=5.14.1,<6.0.0)
 Requires-Dist: pydantic (>=2.5.0,<3.0.0)
 Requires-Dist: pygame (>=2.1.2,<3.0.0)
 Requires-Dist: pygifsicle (>=1.0.7,<2.0.0)
@@ -134,15 +135,15 @@
 
 #### 1.3.3.1. Case Number
 
 |    Date    |     Release Number     | Description      |
 | :--------: | :--------------------: | :--------------: |
 | 2022-05-20 |     AFRL-2022-2455     | Initial release  |
 | 2023-03-02 | APRS-RYZ-2023-01-00006 | Second release   |
-| 2024-21-03 | AFRL-2024-1562         | Thirst release   |
+| 2024-21-03 | AFRL-2024-1562         | Third release   |
 
 #### 1.3.3.2. Designation Indicator
 
 - Controlled by: Air Force Research Laboratory (AFRL)
 - Controlled by: AFRL Autonomy Capability Team (ACT3)
 
 #### 1.3.3.3. Points of Contact
```

