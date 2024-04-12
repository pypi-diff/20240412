# Comparing `tmp/utopya-1.3.0b1.tar.gz` & `tmp/utopya-1.3.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utopya-1.3.0b1.tar", last modified: Mon Jan 22 22:01:31 2024, max compression
+gzip compressed data, was "utopya-1.3.0b3.tar", last modified: Fri Apr 12 21:20:31 2024, max compression
```

## Comparing `utopya-1.3.0b1.tar` & `utopya-1.3.0b3.tar`

### file list

```diff
@@ -1,129 +1,131 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 22:01:31.276199 utopya-1.3.0b1/
--rw-rw-rw-   0 root         (0) root         (0)    11765 2024-01-22 22:01:17.000000 utopya-1.3.0b1/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)    35149 2024-01-22 22:01:17.000000 utopya-1.3.0b1/COPYING
--rw-rw-rw-   0 root         (0) root         (0)     7633 2024-01-22 22:01:17.000000 utopya-1.3.0b1/COPYING.LESSER
--rw-r--r--   0 root         (0) root         (0)     3160 2024-01-22 22:01:31.276199 utopya-1.3.0b1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5594 2024-01-22 22:01:17.000000 utopya-1.3.0b1/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1734 2024-01-22 22:01:17.000000 utopya-1.3.0b1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-01-22 22:01:31.276199 utopya-1.3.0b1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     5880 2024-01-22 22:01:17.000000 utopya-1.3.0b1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 22:01:31.254200 utopya-1.3.0b1/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 22:01:31.257200 utopya-1.3.0b1/tests/_gen_figures/
--rw-rw-rw-   0 root         (0) root         (0)      560 2024-01-22 22:01:17.000000 utopya-1.3.0b1/tests/_gen_figures/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       50 2024-01-22 22:01:17.000000 utopya-1.3.0b1/tests/_gen_figures/_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     5271 2024-01-22 22:01:17.000000 utopya-1.3.0b1/tests/_gen_figures/test_plots.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 22:01:31.258200 utopya-1.3.0b1/tests/backend/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-22 22:01:17.000000 utopya-1.3.0b1/tests/backend/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8239 2024-01-22 22:01:17.000000 utopya-1.3.0b1/tests/backend/test_benchmark.py
--rw-rw-rw-   0 root         (0) root         (0)    12007 2024-01-22 22:01:17.000000 utopya-1.3.0b1/tests/backend/test_model.py
--rw-rw-rw-   0 root         (0) root         (0)     2898 2024-01-22 22:01:17.000000 utopya-1.3.0b1/tests/backend/test_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 22:01:31.260200 utopya-1.3.0b1/tests/cli/
--rw-rw-rw-   0 root         (0) root         (0)      193 2024-01-22 22:01:17.000000 utopya-1.3.0b1/tests/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2844 2024-01-22 22:01:17.000000 utopya-1.3.0b1/tests/cli/test__shell_complete.py
--rw-rw-rw-   0 root         (0) root         (0)     2810 2024-01-22 22:01:17.000000 utopya-1.3.0b1/tests/cli/test__to_migrate.py
--rw-rw-rw-   0 root         (0) root         (0)      914 2024-01-22 22:01:17.000000 utopya-1.3.0b1/tests/cli/test_batch.py
--rw-rw-rw-   0 root         (0) root         (0)     4804 2024-01-22 22:01:17.000000 utopya-1.3.0b1/tests/cli/test_config.py
--rw-rw-rw-   0 root         (0) root         (0)    15337 2024-01-22 22:01:17.000000 utopya-1.3.0b1/tests/cli/test_models.py
--rw-rw-rw-   0 root         (0) root         (0)     6940 2024-01-22 22:01:17.000000 utopya-1.3.0b1/tests/cli/test_projects.py
--rw-rw-rw-   0 root         (0) root         (0)     2169 2024-01-22 22:01:17.000000 utopya-1.3.0b1/tests/cli/test_run_and_eval.py
--rw-rw-rw-   0 root         (0) root         (0)     2477 2024-01-22 22:01:17.000000 utopya-1.3.0b1/tests/cli/test_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 22:01:31.261200 utopya-1.3.0b1/tests/eval/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-22 22:01:17.000000 utopya-1.3.0b1/tests/eval/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9145 2024-01-22 22:01:17.000000 utopya-1.3.0b1/tests/eval/test_containers.py
--rw-rw-rw-   0 root         (0) root         (0)     6607 2024-01-22 22:01:17.000000 utopya-1.3.0b1/tests/eval/test_datamanager.py
--rw-rw-rw-   0 root         (0) root         (0)     2975 2024-01-22 22:01:17.000000 utopya-1.3.0b1/tests/eval/test_groups.py
--rw-rw-rw-   0 root         (0) root         (0)     6444 2024-01-22 22:01:17.000000 utopya-1.3.0b1/tests/eval/test_plot_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    45377 2024-01-22 22:01:17.000000 utopya-1.3.0b1/tests/eval/test_plotting.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 22:01:31.265200 utopya-1.3.0b1/utopya/
--rw-rw-rw-   0 root         (0) root         (0)     3257 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3340 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya/_cluster.py
--rw-rw-rw-   0 root         (0) root         (0)      704 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya/_import_tools.py
--rw-rw-rw-   0 root         (0) root         (0)      249 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya/_signal.py
--rw-rw-rw-   0 root         (0) root         (0)      169 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya/_yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 22:01:31.266200 utopya-1.3.0b1/utopya/_yaml_registry/
--rw-rw-rw-   0 root         (0) root         (0)      135 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya/_yaml_registry/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9532 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya/_yaml_registry/entry.py
--rw-rw-rw-   0 root         (0) root         (0)    10253 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya/_yaml_registry/registry.py
--rw-rw-rw-   0 root         (0) root         (0)    18565 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya/batch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 22:01:31.267200 utopya-1.3.0b1/utopya/cfg/
--rw-rw-rw-   0 root         (0) root         (0)    21639 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya/cfg/base_cfg.yml
--rw-rw-rw-   0 root         (0) root         (0)    13221 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya/cfg/base_plots.yml
--rw-rw-rw-   0 root         (0) root         (0)     8757 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya/cfg/btm_cfg.yml
--rw-rw-rw-   0 root         (0) root         (0)      339 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya/cfg/user_cfg_header.yml
--rw-rw-rw-   0 root         (0) root         (0)     2939 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya/cfg.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 22:01:31.268200 utopya-1.3.0b1/utopya/eval/
--rw-rw-rw-   0 root         (0) root         (0)      480 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya/eval/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6936 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya/eval/_plot_func_resolver.py
--rw-rw-rw-   0 root         (0) root         (0)    16706 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya/eval/containers.py
--rw-rw-rw-   0 root         (0) root         (0)     1311 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya/eval/data_ops.py
--rw-rw-rw-   0 root         (0) root         (0)     3079 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya/eval/datamanager.py
--rw-rw-rw-   0 root         (0) root         (0)     2507 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya/eval/groups.py
--rw-rw-rw-   0 root         (0) root         (0)     1623 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya/eval/plotcreators.py
--rw-rw-rw-   0 root         (0) root         (0)      853 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya/eval/plothelper.py
--rw-rw-rw-   0 root         (0) root         (0)     9048 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya/eval/plotmanager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 22:01:31.271200 utopya-1.3.0b1/utopya/eval/plots/
--rw-rw-rw-   0 root         (0) root         (0)      445 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya/eval/plots/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7502 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya/eval/plots/_attractor.py
--rw-rw-rw-   0 root         (0) root         (0)    72723 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya/eval/plots/_graph.py
--rw-rw-rw-   0 root         (0) root         (0)     1789 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya/eval/plots/_mpl.py
--rw-rw-rw-   0 root         (0) root         (0)    12091 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya/eval/plots/_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    58799 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya/eval/plots/abm.py
--rw-rw-rw-   0 root         (0) root         (0)    25571 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya/eval/plots/attractor.py
--rw-rw-rw-   0 root         (0) root         (0)    53660 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya/eval/plots/ca.py
--rw-rw-rw-   0 root         (0) root         (0)     6924 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya/eval/plots/distributions.py
--rw-rw-rw-   0 root         (0) root         (0)    26857 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya/eval/plots/graph.py
--rw-rw-rw-   0 root         (0) root         (0)     9451 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya/eval/plots/snsplot.py
--rw-rw-rw-   0 root         (0) root         (0)     3193 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya/eval/plots/time_series.py
--rw-rw-rw-   0 root         (0) root         (0)     2265 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya/eval/transform.py
--rw-rw-rw-   0 root         (0) root         (0)     3623 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    23144 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 22:01:31.272200 utopya-1.3.0b1/utopya/model_registry/
--rw-rw-rw-   0 root         (0) root         (0)      659 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya/model_registry/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3494 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya/model_registry/_registration.py
--rw-rw-rw-   0 root         (0) root         (0)    16777 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya/model_registry/entry.py
--rw-rw-rw-   0 root         (0) root         (0)    15927 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya/model_registry/info_bundle.py
--rw-rw-rw-   0 root         (0) root         (0)    11936 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya/model_registry/registry.py
--rw-rw-rw-   0 root         (0) root         (0)     3635 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya/model_registry/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    71586 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya/multiverse.py
--rw-rw-rw-   0 root         (0) root         (0)    19695 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya/parameter.py
--rw-rw-rw-   0 root         (0) root         (0)      674 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya/plotting.py
--rw-rw-rw-   0 root         (0) root         (0)    12297 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya/project_registry.py
--rw-rw-rw-   0 root         (0) root         (0)    54018 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya/reporter.py
--rw-rw-rw-   0 root         (0) root         (0)    13652 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya/stop_conditions.py
--rw-rw-rw-   0 root         (0) root         (0)    52862 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya/task.py
--rw-rw-rw-   0 root         (0) root         (0)     1835 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya/testtools.py
--rw-rw-rw-   0 root         (0) root         (0)     9031 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya/tools.py
--rw-rw-rw-   0 root         (0) root         (0)    42058 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya/workermanager.py
--rw-rw-rw-   0 root         (0) root         (0)     1598 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya/yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 22:01:31.266200 utopya-1.3.0b1/utopya.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3160 2024-01-22 22:01:31.000000 utopya-1.3.0b1/utopya.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2775 2024-01-22 22:01:31.000000 utopya-1.3.0b1/utopya.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-22 22:01:31.000000 utopya-1.3.0b1/utopya.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       74 2024-01-22 22:01:31.000000 utopya-1.3.0b1/utopya.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      511 2024-01-22 22:01:31.000000 utopya-1.3.0b1/utopya.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       39 2024-01-22 22:01:31.000000 utopya-1.3.0b1/utopya.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 22:01:31.273200 utopya-1.3.0b1/utopya_backend/
--rw-rw-rw-   0 root         (0) root         (0)      460 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya_backend/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17633 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya_backend/benchmark.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 22:01:31.273200 utopya-1.3.0b1/utopya_backend/io/
--rw-rw-rw-   0 root         (0) root         (0)       63 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya_backend/io/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1504 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya_backend/logging.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 22:01:31.273200 utopya-1.3.0b1/utopya_backend/model/
--rw-rw-rw-   0 root         (0) root         (0)      512 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya_backend/model/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    21214 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya_backend/model/base.py
--rw-rw-rw-   0 root         (0) root         (0)     8082 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya_backend/model/step.py
--rw-rw-rw-   0 root         (0) root         (0)     1619 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya_backend/signal.py
--rw-rw-rw-   0 root         (0) root         (0)     5411 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya_backend/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 22:01:31.275200 utopya-1.3.0b1/utopya_cli/
--rw-rw-rw-   0 root         (0) root         (0)       66 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya_cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18051 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya_cli/_copy_model.py
--rw-rw-rw-   0 root         (0) root         (0)     9861 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya_cli/_shared.py
--rw-rw-rw-   0 root         (0) root         (0)    15555 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya_cli/_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1644 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya_cli/batch.py
--rw-rw-rw-   0 root         (0) root         (0)     1382 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya_cli/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     5722 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya_cli/config.py
--rw-rw-rw-   0 root         (0) root         (0)    17744 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya_cli/eval.py
--rw-rw-rw-   0 root         (0) root         (0)    24141 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya_cli/models.py
--rw-rw-rw-   0 root         (0) root         (0)     7872 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya_cli/projects.py
--rw-rw-rw-   0 root         (0) root         (0)     7108 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya_cli/run.py
--rw-rw-rw-   0 root         (0) root         (0)     2627 2024-01-22 22:01:17.000000 utopya-1.3.0b1/utopya_cli/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:20:31.584468 utopya-1.3.0b3/
+-rw-rw-rw-   0 root         (0) root         (0)    12038 2024-04-12 21:20:19.000000 utopya-1.3.0b3/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)    35149 2024-04-12 21:20:19.000000 utopya-1.3.0b3/COPYING
+-rw-rw-rw-   0 root         (0) root         (0)     7633 2024-04-12 21:20:19.000000 utopya-1.3.0b3/COPYING.LESSER
+-rw-r--r--   0 root         (0) root         (0)     3160 2024-04-12 21:20:31.583468 utopya-1.3.0b3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5594 2024-04-12 21:20:19.000000 utopya-1.3.0b3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1734 2024-04-12 21:20:19.000000 utopya-1.3.0b3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-12 21:20:31.584468 utopya-1.3.0b3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     5876 2024-04-12 21:20:19.000000 utopya-1.3.0b3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:20:31.562469 utopya-1.3.0b3/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:20:31.566469 utopya-1.3.0b3/tests/_gen_figures/
+-rw-rw-rw-   0 root         (0) root         (0)      560 2024-04-12 21:20:19.000000 utopya-1.3.0b3/tests/_gen_figures/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       50 2024-04-12 21:20:19.000000 utopya-1.3.0b3/tests/_gen_figures/_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     5271 2024-04-12 21:20:19.000000 utopya-1.3.0b3/tests/_gen_figures/test_plots.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:20:31.566469 utopya-1.3.0b3/tests/backend/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 21:20:19.000000 utopya-1.3.0b3/tests/backend/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8239 2024-04-12 21:20:19.000000 utopya-1.3.0b3/tests/backend/test_benchmark.py
+-rw-rw-rw-   0 root         (0) root         (0)    12007 2024-04-12 21:20:19.000000 utopya-1.3.0b3/tests/backend/test_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2898 2024-04-12 21:20:19.000000 utopya-1.3.0b3/tests/backend/test_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:20:31.568469 utopya-1.3.0b3/tests/cli/
+-rw-rw-rw-   0 root         (0) root         (0)      193 2024-04-12 21:20:19.000000 utopya-1.3.0b3/tests/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2844 2024-04-12 21:20:19.000000 utopya-1.3.0b3/tests/cli/test__shell_complete.py
+-rw-rw-rw-   0 root         (0) root         (0)     2810 2024-04-12 21:20:19.000000 utopya-1.3.0b3/tests/cli/test__to_migrate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1094 2024-04-12 21:20:19.000000 utopya-1.3.0b3/tests/cli/test_batch.py
+-rw-rw-rw-   0 root         (0) root         (0)     4804 2024-04-12 21:20:19.000000 utopya-1.3.0b3/tests/cli/test_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    15337 2024-04-12 21:20:19.000000 utopya-1.3.0b3/tests/cli/test_models.py
+-rw-rw-rw-   0 root         (0) root         (0)     6940 2024-04-12 21:20:19.000000 utopya-1.3.0b3/tests/cli/test_projects.py
+-rw-rw-rw-   0 root         (0) root         (0)     6343 2024-04-12 21:20:19.000000 utopya-1.3.0b3/tests/cli/test_run_and_eval.py
+-rw-rw-rw-   0 root         (0) root         (0)     2478 2024-04-12 21:20:19.000000 utopya-1.3.0b3/tests/cli/test_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:20:31.569469 utopya-1.3.0b3/tests/eval/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 21:20:19.000000 utopya-1.3.0b3/tests/eval/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9145 2024-04-12 21:20:19.000000 utopya-1.3.0b3/tests/eval/test_containers.py
+-rw-rw-rw-   0 root         (0) root         (0)     6607 2024-04-12 21:20:19.000000 utopya-1.3.0b3/tests/eval/test_datamanager.py
+-rw-rw-rw-   0 root         (0) root         (0)     2975 2024-04-12 21:20:19.000000 utopya-1.3.0b3/tests/eval/test_groups.py
+-rw-rw-rw-   0 root         (0) root         (0)     6444 2024-04-12 21:20:19.000000 utopya-1.3.0b3/tests/eval/test_plot_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    45377 2024-04-12 21:20:19.000000 utopya-1.3.0b3/tests/eval/test_plotting.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:20:31.572469 utopya-1.3.0b3/utopya/
+-rw-rw-rw-   0 root         (0) root         (0)     2149 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3388 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/_cluster.py
+-rw-rw-rw-   0 root         (0) root         (0)      704 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/_import_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     1234 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/_logging.py
+-rw-rw-rw-   0 root         (0) root         (0)      249 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/_signal.py
+-rw-rw-rw-   0 root         (0) root         (0)      169 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/_yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:20:31.574469 utopya-1.3.0b3/utopya/_yaml_registry/
+-rw-rw-rw-   0 root         (0) root         (0)      135 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/_yaml_registry/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9532 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/_yaml_registry/entry.py
+-rw-rw-rw-   0 root         (0) root         (0)    10253 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/_yaml_registry/registry.py
+-rw-rw-rw-   0 root         (0) root         (0)    18565 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/batch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:20:31.575469 utopya-1.3.0b3/utopya/cfg/
+-rw-rw-rw-   0 root         (0) root         (0)    22003 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/cfg/base_cfg.yml
+-rw-rw-rw-   0 root         (0) root         (0)    13221 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/cfg/base_plots.yml
+-rw-rw-rw-   0 root         (0) root         (0)     8757 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/cfg/btm_cfg.yml
+-rw-rw-rw-   0 root         (0) root         (0)      339 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/cfg/user_cfg_header.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2939 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/cfg.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:20:31.576469 utopya-1.3.0b3/utopya/eval/
+-rw-rw-rw-   0 root         (0) root         (0)      480 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/eval/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6936 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/eval/_plot_func_resolver.py
+-rw-rw-rw-   0 root         (0) root         (0)    16706 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/eval/containers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1311 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/eval/data_ops.py
+-rw-rw-rw-   0 root         (0) root         (0)     3079 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/eval/datamanager.py
+-rw-rw-rw-   0 root         (0) root         (0)     2507 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/eval/groups.py
+-rw-rw-rw-   0 root         (0) root         (0)     1623 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/eval/plotcreators.py
+-rw-rw-rw-   0 root         (0) root         (0)      853 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/eval/plothelper.py
+-rw-rw-rw-   0 root         (0) root         (0)     9048 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/eval/plotmanager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:20:31.578468 utopya-1.3.0b3/utopya/eval/plots/
+-rw-rw-rw-   0 root         (0) root         (0)      445 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/eval/plots/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7502 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/eval/plots/_attractor.py
+-rw-rw-rw-   0 root         (0) root         (0)    72723 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/eval/plots/_graph.py
+-rw-rw-rw-   0 root         (0) root         (0)     1789 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/eval/plots/_mpl.py
+-rw-rw-rw-   0 root         (0) root         (0)    12091 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/eval/plots/_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    58831 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/eval/plots/abm.py
+-rw-rw-rw-   0 root         (0) root         (0)    25571 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/eval/plots/attractor.py
+-rw-rw-rw-   0 root         (0) root         (0)    53660 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/eval/plots/ca.py
+-rw-rw-rw-   0 root         (0) root         (0)     6924 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/eval/plots/distributions.py
+-rw-rw-rw-   0 root         (0) root         (0)    26857 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/eval/plots/graph.py
+-rw-rw-rw-   0 root         (0) root         (0)     9451 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/eval/plots/snsplot.py
+-rw-rw-rw-   0 root         (0) root         (0)     3193 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/eval/plots/time_series.py
+-rw-rw-rw-   0 root         (0) root         (0)     2265 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/eval/transform.py
+-rw-rw-rw-   0 root         (0) root         (0)     3623 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    23681 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:20:31.579468 utopya-1.3.0b3/utopya/model_registry/
+-rw-rw-rw-   0 root         (0) root         (0)      660 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/model_registry/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3494 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/model_registry/_registration.py
+-rw-rw-rw-   0 root         (0) root         (0)    16777 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/model_registry/entry.py
+-rw-rw-rw-   0 root         (0) root         (0)    15928 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/model_registry/info_bundle.py
+-rw-rw-rw-   0 root         (0) root         (0)    11936 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/model_registry/registry.py
+-rw-rw-rw-   0 root         (0) root         (0)     3635 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/model_registry/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    86054 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/multiverse.py
+-rw-rw-rw-   0 root         (0) root         (0)    19695 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/parameter.py
+-rw-rw-rw-   0 root         (0) root         (0)      675 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/plotting.py
+-rw-rw-rw-   0 root         (0) root         (0)    12297 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/project_registry.py
+-rw-rw-rw-   0 root         (0) root         (0)    54030 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/reporter.py
+-rw-rw-rw-   0 root         (0) root         (0)    13652 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/stop_conditions.py
+-rw-rw-rw-   0 root         (0) root         (0)    55886 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/task.py
+-rw-rw-rw-   0 root         (0) root         (0)     1835 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/testtools.py
+-rw-rw-rw-   0 root         (0) root         (0)     9031 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/tools.py
+-rw-rw-rw-   0 root         (0) root         (0)    42072 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/workermanager.py
+-rw-rw-rw-   0 root         (0) root         (0)     1598 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya/yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:20:31.573469 utopya-1.3.0b3/utopya.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3160 2024-04-12 21:20:31.000000 utopya-1.3.0b3/utopya.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2821 2024-04-12 21:20:31.000000 utopya-1.3.0b3/utopya.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 21:20:31.000000 utopya-1.3.0b3/utopya.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       74 2024-04-12 21:20:31.000000 utopya-1.3.0b3/utopya.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      507 2024-04-12 21:20:31.000000 utopya-1.3.0b3/utopya.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2024-04-12 21:20:31.000000 utopya-1.3.0b3/utopya.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:20:31.580469 utopya-1.3.0b3/utopya_backend/
+-rw-rw-rw-   0 root         (0) root         (0)      460 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya_backend/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17633 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya_backend/benchmark.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:20:31.580469 utopya-1.3.0b3/utopya_backend/io/
+-rw-rw-rw-   0 root         (0) root         (0)       63 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya_backend/io/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1504 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya_backend/logging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:20:31.581468 utopya-1.3.0b3/utopya_backend/model/
+-rw-rw-rw-   0 root         (0) root         (0)      512 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya_backend/model/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    21215 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya_backend/model/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     8082 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya_backend/model/step.py
+-rw-rw-rw-   0 root         (0) root         (0)     1619 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya_backend/signal.py
+-rw-rw-rw-   0 root         (0) root         (0)     5411 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya_backend/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:20:31.583468 utopya-1.3.0b3/utopya_cli/
+-rw-rw-rw-   0 root         (0) root         (0)       66 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya_cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18051 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya_cli/_copy_model.py
+-rw-rw-rw-   0 root         (0) root         (0)    10332 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya_cli/_shared.py
+-rw-rw-rw-   0 root         (0) root         (0)    16323 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya_cli/_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1644 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya_cli/batch.py
+-rw-rw-rw-   0 root         (0) root         (0)     1459 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya_cli/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     5722 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya_cli/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    17744 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya_cli/eval.py
+-rw-rw-rw-   0 root         (0) root         (0)    24141 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya_cli/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     7872 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya_cli/projects.py
+-rw-rw-rw-   0 root         (0) root         (0)     7382 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya_cli/run.py
+-rw-rw-rw-   0 root         (0) root         (0)     3334 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya_cli/run_existing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2627 2024-04-12 21:20:19.000000 utopya-1.3.0b3/utopya_cli/test.py
```

### Comparing `utopya-1.3.0b1/CHANGELOG.md` & `utopya-1.3.0b3/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,22 @@
 
 `utopya` aims to adhere to [semantic versioning](https://semver.org/).
 
 ## v1.3.0 *(Work in progress)*
 ### Features and enhancements
 - !71 allows setting permissions on a simulation's subdirectories.
   Also sets the `eval` directory permissions such that other users of the same group can evaluate simulations without requiring manual permission changes.
+- !74 implements `utopya run-existing`, an *experimental* feature that allows finishing or re-running a previously-created simulation run.
 
 ### Removals and deprecations
 - !72 removes the deprecated CA `ca.state` plot and the `draw_cbar` and `limits` arguments of the `.plot.ca`.
 
+### Internal
+- !76 moves the logging-related adjustments (e.g. colored log messages) to their own private module, `utopya._logging`.
+
 
 ## v1.2.13
 - !70 adds `utopia` as a console script, giving access to the `utopya` CLI.
 
 ## v1.2.12
 - !68 lets the `xr.DataArray` underlying `XarrayDC` inherit attributes from the container instance (don't know why that wasn't configured to be the case before).
 - !67 fixes a regression in the Read-The-Docs configuration.
```

### Comparing `utopya-1.3.0b1/COPYING` & `utopya-1.3.0b3/COPYING`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/COPYING.LESSER` & `utopya-1.3.0b3/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/PKG-INFO` & `utopya-1.3.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utopya
-Version: 1.3.0b1
+Version: 1.3.0b3
 Summary: A simulation management and evaluation framework
 Home-page: https://gitlab.com/utopia-project/utopya
 Author: utopya developers
 Author-email: Yunus Sevinchan <yunus.sevinchan@hu-berlin.de>
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `utopya-1.3.0b1/README.md` & `utopya-1.3.0b3/README.md`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/pyproject.toml` & `utopya-1.3.0b3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/setup.py` & `utopya-1.3.0b3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,17 @@
     "coloredlogs",
     "colorama",
     "click",
     "pydantic >= 2.0",
     "python-git-info",
     #
     # first-party packages
-    "yayaml>=0.1.1",
-    "paramspace>=2.6.1",
-    "dantro>=0.19.2",
+    "yayaml>=0.2",
+    "paramspace>=2.7",
+    "dantro>=0.19.5",
 ]
 # NOTE When adding a new dependency, make sure to denote it in the isort
 #      configuration, see pyproject.toml.
 
 # Dependencies for running tests and general development of utopya
 TEST_DEPS = [
     "pytest",
```

### Comparing `utopya-1.3.0b1/tests/_gen_figures/__init__.py` & `utopya-1.3.0b3/tests/_gen_figures/__init__.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/tests/_gen_figures/test_plots.py` & `utopya-1.3.0b3/tests/_gen_figures/test_plots.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/tests/backend/test_benchmark.py` & `utopya-1.3.0b3/tests/backend/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/tests/backend/test_model.py` & `utopya-1.3.0b3/tests/backend/test_model.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/tests/backend/test_tools.py` & `utopya-1.3.0b3/tests/backend/test_tools.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/tests/cli/test__shell_complete.py` & `utopya-1.3.0b3/tests/cli/test__shell_complete.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/tests/cli/test__to_migrate.py` & `utopya-1.3.0b3/tests/cli/test__to_migrate.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/tests/cli/test_batch.py` & `utopya-1.3.0b3/tests/cli/test_batch.py`

 * *Files 21% similar despite different names*

```diff
@@ -26,12 +26,18 @@
 
 # -----------------------------------------------------------------------------
 
 
 @skip_if_on_macOS
 def test_batch(with_test_models):  # FIXME creates test artifacts in output dir
     """Tests the `utopya batch` subcommand"""
+    # Make sure the ExtendedModel has already run
+    model = utopya.Model(name="ExtendedModel")
+    mv = model.create_mv()
+    mv.run()
+
+    # Now actually perform the batch eval
     res = invoke_cli(("batch", "-d", "-s", "--note", "some_note", BATCH_FILE))
     print(res.output)
 
     assert res.exit_code == 0
     assert "time_series/mean_state" in res.output
```

### Comparing `utopya-1.3.0b1/tests/cli/test_config.py` & `utopya-1.3.0b3/tests/cli/test_config.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/tests/cli/test_models.py` & `utopya-1.3.0b3/tests/cli/test_models.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/tests/cli/test_projects.py` & `utopya-1.3.0b3/tests/cli/test_projects.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/tests/cli/test_test.py` & `utopya-1.3.0b3/tests/cli/test_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import pytest
 
 from .._fixtures import *
 from . import invoke_cli
 
 # -----------------------------------------------------------------------------
 
+
 # FIXME for whatever strange reason, this creates side effects in
 #       eval/test_plotting.py::test_preloading
 #       Removing "model_plots" from sys.modules here does not resolve it.
 @pytest.mark.order("last")
 def test_test(with_test_models):
     """Tests `utopya test`"""
     # No tests available for dummy model
```

### Comparing `utopya-1.3.0b1/tests/eval/test_containers.py` & `utopya-1.3.0b3/tests/eval/test_containers.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/tests/eval/test_datamanager.py` & `utopya-1.3.0b3/tests/eval/test_datamanager.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/tests/eval/test_groups.py` & `utopya-1.3.0b3/tests/eval/test_groups.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/tests/eval/test_plot_utils.py` & `utopya-1.3.0b3/tests/eval/test_plot_utils.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/tests/eval/test_plotting.py` & `utopya-1.3.0b3/tests/eval/test_plotting.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/utopya/_cluster.py` & `utopya-1.3.0b3/utopya/_cluster.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,17 +47,19 @@
             # Get the string width
             digits = len(segments[0][0])
 
             # In segments, lists longer than 1 are intervals, the
             # others are node numbers of a single node.
             # Expand intervals
             segments = [
-                [int(seg[0])]
-                if len(seg) == 1
-                else list(range(int(seg[0]), int(seg[1]) + 1))
+                (
+                    [int(seg[0])]
+                    if len(seg) == 1
+                    else list(range(int(seg[0]), int(seg[1]) + 1))
+                )
                 for seg in segments
             ]
 
             # Combine to list of individual node numbers
             node_nos = []
             for seg in segments:
                 node_nos += seg
```

### Comparing `utopya-1.3.0b1/utopya/_import_tools.py` & `utopya-1.3.0b3/utopya/_import_tools.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/utopya/_yaml_registry/entry.py` & `utopya-1.3.0b3/utopya/_yaml_registry/entry.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/utopya/_yaml_registry/registry.py` & `utopya-1.3.0b3/utopya/_yaml_registry/registry.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/utopya/batch.py` & `utopya-1.3.0b3/utopya/batch.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/utopya/cfg/base_cfg.yml` & `utopya-1.3.0b3/utopya/cfg/base_cfg.yml`

 * *Files 2% similar despite different names*

```diff
@@ -149,14 +149,15 @@
         file:
           path: _sweep_info.txt
           skip_if_empty: true
         log:
           lvl: 18
           skip_if_empty: true
       fstr: "Sweeping over the following parameter space:\n\n{sweep_info:}"
+      only_for_sweep: true
 
   # Can define a default format to use
   # default_format: ~
 
 
 # Worker Manager ..............................................................
 # Initialization arguments for the WorkerManager
@@ -240,14 +241,21 @@
   # See docs for how to set these up:
   #   https://docs.utopia-project.org/html/usage/run/stop-conditions.html
 
 
 # The defaults for the worker_kwargs
 # These are passed to the setup function of each WorkerTask before spawning
 worker_kwargs:
+  # Whether the task should be performed at all.
+  # If false, this will call each universes' setup function, writing respective
+  # config files, but not actually carry out universe simulations. This is used
+  # in combination with the DistributedMultiverse, which can then carry out the
+  # actual universe runs.
+  perform_task: true
+
   # Whether to save the streams of each Universe to a log file
   save_streams: true
   # This file is saved only after the WorkerTask has finished in order to
   # reduce I/O operations on files
 
   # Whether to forward the streams to stdout
   forward_streams: in_single_run
```

### Comparing `utopya-1.3.0b1/utopya/cfg/base_plots.yml` & `utopya-1.3.0b3/utopya/cfg/base_plots.yml`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/utopya/cfg/btm_cfg.yml` & `utopya-1.3.0b3/utopya/cfg/btm_cfg.yml`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/utopya/cfg.py` & `utopya-1.3.0b3/utopya/cfg.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/utopya/eval/_plot_func_resolver.py` & `utopya-1.3.0b3/utopya/eval/_plot_func_resolver.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/utopya/eval/containers.py` & `utopya-1.3.0b3/utopya/eval/containers.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/utopya/eval/data_ops.py` & `utopya-1.3.0b3/utopya/eval/data_ops.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/utopya/eval/datamanager.py` & `utopya-1.3.0b3/utopya/eval/datamanager.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/utopya/eval/groups.py` & `utopya-1.3.0b3/utopya/eval/groups.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/utopya/eval/plotcreators.py` & `utopya-1.3.0b3/utopya/eval/plotcreators.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/utopya/eval/plothelper.py` & `utopya-1.3.0b3/utopya/eval/plothelper.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/utopya/eval/plotmanager.py` & `utopya-1.3.0b3/utopya/eval/plotmanager.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/utopya/eval/plots/_attractor.py` & `utopya-1.3.0b3/utopya/eval/plots/_attractor.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/utopya/eval/plots/_graph.py` & `utopya-1.3.0b3/utopya/eval/plots/_graph.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/utopya/eval/plots/_mpl.py` & `utopya-1.3.0b3/utopya/eval/plots/_mpl.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/utopya/eval/plots/_utils.py` & `utopya-1.3.0b3/utopya/eval/plots/_utils.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/utopya/eval/plots/abm.py` & `utopya-1.3.0b3/utopya/eval/plots/abm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1422,17 +1422,19 @@
         ax=hlpr.ax, layers=layers, **parse_domain_kwargs(domain)
     )
 
     # Inform about the plot ...
     log.remark("  Data variables:         %s", ", ".join(to_plot))
     log.remark(
         "  Frames dimension(s):    %s",
-        shared_frames_dim
-        if shared_frames_dim
-        else ", ".join(f"{f}" for f in frame_dims),
+        (
+            shared_frames_dim
+            if shared_frames_dim
+            else ", ".join(f"{f}" for f in frame_dims)
+        ),
     )
     log.remark(
         "  Number of frames:       %s",
         num_frames if num_frames > 1 else "(snapshot)",
     )
     log.remark(
         "  Domain area:            %.4g  (aspect: %.3g)", domain_area, _aspect
```

### Comparing `utopya-1.3.0b1/utopya/eval/plots/attractor.py` & `utopya-1.3.0b3/utopya/eval/plots/attractor.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/utopya/eval/plots/ca.py` & `utopya-1.3.0b3/utopya/eval/plots/ca.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/utopya/eval/plots/distributions.py` & `utopya-1.3.0b3/utopya/eval/plots/distributions.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/utopya/eval/plots/graph.py` & `utopya-1.3.0b3/utopya/eval/plots/graph.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/utopya/eval/plots/snsplot.py` & `utopya-1.3.0b3/utopya/eval/plots/snsplot.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/utopya/eval/plots/time_series.py` & `utopya-1.3.0b3/utopya/eval/plots/time_series.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/utopya/eval/transform.py` & `utopya-1.3.0b3/utopya/eval/transform.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/utopya/exceptions.py` & `utopya-1.3.0b3/utopya/exceptions.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/utopya/model.py` & `utopya-1.3.0b3/utopya/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from dantro.tools import adjusted_log_levels as _adjusted_log_levels
 from dantro.tools import make_columns as _make_columns
 
 from .cfg import load_from_cfg_dir
 from .eval import DataManager
 from .model_registry import ModelInfoBundle, get_info_bundle, load_model_cfg
-from .multiverse import FrozenMultiverse, Multiverse
+from .multiverse import DistributedMultiverse, FrozenMultiverse, Multiverse
 
 log = logging.getLogger(__name__)
 
 # -----------------------------------------------------------------------------
 
 
 class Model:
@@ -316,14 +316,29 @@
                 :py:meth:`utopya.multiverse.FrozenMultiverse.__init__`
         """
         mv = FrozenMultiverse(model_name=self.name, **fmv_kwargs)
         self._store_mv(mv)
 
         return mv
 
+    def create_distributed_mv(self, **dmv_kwargs) -> DistributedMultiverse:
+        """Create a :py:class:`utopya.multiverse.FrozenMultiverse`, coupling it
+        to a run directory.
+
+        Use this method if you want to load an *existing* simulation run.
+
+        Args:
+            **fmv_kwargs: Passed on to
+                :py:meth:`utopya.multiverse.FrozenMultiverse.__init__`
+        """
+        mv = DistributedMultiverse(model_name=self.name, **dmv_kwargs)
+        self._store_mv(mv)
+
+        return mv
+
     def create_run_load(
         self,
         *,
         from_cfg: str = None,
         run_cfg_path: str = None,
         from_cfg_set: str = None,
         use_tmpdir: bool = None,
```

### Comparing `utopya-1.3.0b1/utopya/model_registry/__init__.py` & `utopya-1.3.0b3/utopya/model_registry/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """This submodule implements a registry of Utopia models, which is used to
 provide the required model information to the frontend and use it throughout.
 """
+
 from ..exceptions import BundleExistsError, ModelRegistryError
 from .entry import ModelRegistryEntry
 
 # Make names of class definitions available
 from .info_bundle import ModelInfoBundle
 
 # Import the registry class only as "private"; should only be instantiated once
```

### Comparing `utopya-1.3.0b1/utopya/model_registry/_registration.py` & `utopya-1.3.0b3/utopya/model_registry/_registration.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/utopya/model_registry/entry.py` & `utopya-1.3.0b3/utopya/model_registry/entry.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/utopya/model_registry/info_bundle.py` & `utopya-1.3.0b3/utopya/model_registry/info_bundle.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Implements the ModelInfoBundle class, which holds a single bundle of
 information about a model.
 """
+
 import copy
 import logging
 import os
 import time
 from typing import Optional, Sequence, Tuple, Union
 
 from ..exceptions import MissingProjectError
```

### Comparing `utopya-1.3.0b1/utopya/model_registry/registry.py` & `utopya-1.3.0b3/utopya/model_registry/registry.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/utopya/model_registry/utils.py` & `utopya-1.3.0b3/utopya/model_registry/utils.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/utopya/multiverse.py` & `utopya-1.3.0b3/utopya/multiverse.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Implementation of the :py:class:`~utopya.multiverse.Multiverse` class which
 sits at the heart of utopya and supplies the main user interface for the
 frontend. It allows to run a simulation and then evaluate it.
 """
+
 import copy
 import itertools
 import logging
 import os
 import re
 import time
 import warnings
@@ -20,14 +21,15 @@
 from ._cluster import parse_node_list
 from .cfg import get_cfg_path as _get_cfg_path
 from .eval import DataManager, PlotManager
 from .model_registry import ModelInfoBundle, get_info_bundle, load_model_cfg
 from .parameter import ValidationError
 from .project_registry import PROJECTS
 from .reporter import WorkerManagerReporter
+from .task import NoWorkTask, WorkerTask
 from .tools import parse_num_steps, pformat, recursive_update
 from .workermanager import WorkerManager
 from .yaml import load_yml, write_yml
 
 log = logging.getLogger(__name__)
 
 # -----------------------------------------------------------------------------
@@ -305,15 +307,15 @@
     def pm(self) -> PlotManager:
         """The Multiverse's PlotManager."""
         return self._pm
 
     # Public methods ..........................................................
 
     def run(self, *, sweep: bool = None):
-        """Starts a Utopia simulation run.
+        """Starts a simulation run.
 
         Specifically, this method adds simulation tasks to the associated
         WorkerManager, locks its task list, and then invokes the
         :py:meth:`~utopya.workermanager.WorkerManager.start_working` method
         which performs all the simulation tasks.
 
         If cluster mode is enabled, this will split up the parameter space into
@@ -748,14 +750,112 @@
             log.debug(
                 "Setting permissions on %s directory to %s ...",
                 dirname,
                 oct(mode),
             )
             os.chmod(self.dirs[dirname], mode)
 
+    def _get_run_dir(self, *, out_dir: str, run_dir: str, **__):
+        """Helper function to find the run directory from arguments given
+        to :py:meth:`~utopya.multiverse.Multiverse.__init__`.
+        This is not actually used in :py:class:`~utopya.multiverse.Multiverse`
+        but in :py:class:`~utopya.multiverse.FrozenMultiverse` and
+        :py:class:`~utopya.multiverse.DistributedMultiverse`.
+
+        Args:
+            out_dir (str): The output directory
+            run_dir (str): The run directory to use
+            ``**__``: ignored
+
+        Raises:
+            IOError: No directory found to use as run directory
+            TypeError: When run_dir was not a string
+        """
+        PATTERN = r"\d{6}-\d{6}_?.*"
+
+        # Create model directory path (where the to-be-loaded data is expected)
+        out_dir = os.path.expanduser(str(out_dir))
+        model_dir = os.path.join(out_dir, self.model_name)
+
+        if not os.path.isdir(model_dir):
+            # Just create it, there's no harm in that ...
+            os.makedirs(model_dir)
+
+        # Distinguish different types of values for the run_dir argument
+        if run_dir is None:
+            log.info("Trying to identify the most recent run directory ...")
+
+            # Create list of _directories_ matching timestamp pattern
+            dirs = [
+                d
+                for d in sorted(os.listdir(model_dir))
+                if os.path.isdir(os.path.join(model_dir, d))
+                and re.match(PATTERN, os.path.basename(d))
+            ]
+
+            if not dirs:
+                raise FileNotFoundError(
+                    "Could not find a run directory to load for evaluation "
+                    f"of model '{self.model_name}'!\n"
+                    f"Model output directory:  {model_dir}\n\n"
+                    "Did you perform a simulation yet? If you are using this "
+                    "model only for evaluation, place your data in a new "
+                    "subdirectory in that folder (using timestamp as name)."
+                )
+
+            # Use the latest to choose the run directory
+            run_dir = os.path.join(model_dir, dirs[-1])
+
+        elif isinstance(run_dir, str):
+            run_dir = os.path.expanduser(run_dir)
+
+            # Distinguish absolute and relative paths and those starting with
+            # a timestamp-like pattern, which can be looked up from the model
+            # directory.
+            if os.path.isabs(run_dir):
+                log.debug("Received absolute run_dir, using that one.")
+
+            elif re.match(PATTERN, run_dir):
+                # Looks like a relative path within the model directory
+                log.info(
+                    "Received timestamp '%s' for run_dir; trying to find "
+                    "one within the model output directory ...",
+                    run_dir,
+                )
+                run_dir = os.path.join(model_dir, run_dir)
+
+            else:
+                # Is not an absolute path and not a timestamp; thus a path
+                # relative to the current working directory
+                run_dir = os.path.join(os.getcwd(), run_dir)
+
+        else:
+            raise TypeError(
+                "Argument run_dir needs to be None, an absolute "
+                "path, or a path relative to the model output "
+                f"directory, but it was: {run_dir}"
+            )
+
+        # Check if the directory exists
+        if not os.path.isdir(run_dir):
+            raise OSError(f"No run directory found at '{run_dir}'!")
+
+        # Store the path and associate the subdirectories
+        self.dirs["run"] = run_dir
+
+        for subdir in ("config", "eval", "data"):
+            subdir_path = os.path.join(run_dir, subdir)
+            if not os.path.exists(subdir_path):
+                raise FileNotFoundError(
+                    "Missing '%s' subdirectory in `run_dir` %s!",
+                    subdir,
+                    run_dir,
+                )
+            self.dirs[subdir] = subdir_path
+
     def _setup_pm(self, **update_kwargs) -> PlotManager:
         """Helper function to setup a PlotManager instance"""
         pm_kwargs = copy.deepcopy(self.meta_cfg["plot_manager"])
 
         if update_kwargs:
             pm_kwargs = recursive_update(pm_kwargs, update_kwargs)
 
@@ -1038,15 +1138,15 @@
             - ``config/{filename}_info.yml``: the passed ``pspace`` object's
                 info dictionary containing relevant metadata (and the
                 additionally passed ``info_kwargs``)
 
         .. note::
 
             This method is separated from the regular backup method
-            :py:meth:`._perform_backup` because the
+            :py:meth:`Multiverse._perform_backup` because the
             parameter space that is *used* during a simulation run may be a
             lower-dimensional version of the one the Multiverse was
             initialized with.
             To that end, :py:meth:`.run` will invoke this backup function
             again once the relevant information is fully determined. This is
             important because it is needed to communicate the correct
             information about the sweep to objects downstream in the pipeline
@@ -1197,14 +1297,151 @@
         # node_index: the offset in the modulo operation
         resolved["node_index"] = node_list.index(resolved["node_name"])
 
         # Return the resolved values
         log.debug("Resolved cluster parameters:\n%s", pformat(resolved))
         return resolved
 
+    def _setup_universe(
+        self,
+        *,
+        worker_kwargs: dict,
+        model_name: str,
+        model_executable: str,
+        uni_cfg: dict,
+        uni_basename: str,
+    ) -> dict:
+        """Setup function for individual universes.
+
+        This is called before the worker process starts working on the
+        universe.
+
+        Args:
+            worker_kwargs (dict): the current status of the worker_kwargs
+                dictionary; is always passed to a task setup function
+            model_name (str): The name of the model
+            model_executable (str): path to the binary to execute
+            uni_cfg (dict): the configuration to create a yml file from
+                which is then needed by the model
+            uni_basename (str): Basename of the universe to use for folder
+                creation, i.e.: zero-padded universe number, e.g. uni0042
+
+        Returns:
+            dict: kwargs for the process to be run when task is grabbed by
+                Worker.
+        """
+        # Generate paths
+        uni_dir = os.path.join(self.dirs["data"], uni_basename)
+        uni_cfg_path = os.path.join(uni_dir, "config.yml")
+
+        # Create universe directory path using the basename
+        self._setup_universe_dir(uni_dir, uni_basename=uni_basename)
+        uni_cfg = self._setup_universe_config(
+            uni_cfg=uni_cfg, uni_dir=uni_dir, uni_cfg_path=uni_cfg_path
+        )
+        wk = self._setup_universe_worker_kwargs(
+            model_executable=model_executable,
+            uni_dir=uni_dir,
+            uni_cfg_path=uni_cfg_path,
+            uni_cfg=uni_cfg,
+            **worker_kwargs,
+        )
+        return wk
+
+    def _setup_universe_dir(self, uni_dir: str, *, uni_basename: str) -> None:
+        """Determines the universe directory and, if needed, creates it.
+
+        This is invoked from :py:meth:`~._setup_universe` and is carried out
+        directly before work on that universe starts.
+
+        Args:
+            uni_basename (str): The basename of the universe to create the run
+                directory for.
+        """
+        os.mkdir(uni_dir)
+        log.debug("Created universe directory:\n  %s", uni_dir)
+
+    def _setup_universe_config(
+        self,
+        *,
+        uni_cfg: dict,
+        uni_dir: str,
+        uni_cfg_path: str,
+    ) -> dict:
+        """Sets up the universe configuration and writes it to a file.
+
+        This is invoked from :py:meth:`~._setup_universe` and is carried out
+        directly before work on that universe starts.
+
+        Args:
+            uni_cfg (dict): The given universe configuration
+            uni_dir (str): The universe directory, added to the configuration
+            uni_cfg_path (str): Where to store the uni configuration at
+
+        Returns:
+            dict: The (potentially updated) universe configuration
+        """
+        # Store output directory and determine a path to the output hdf5 file
+        uni_cfg["output_dir"] = uni_dir
+        uni_cfg["output_path"] = os.path.join(uni_dir, "data.h5")
+
+        # Parse the potentially string-valued number of steps values, and
+        # other step-like arguments. Raises an error if they are negative.
+        uni_cfg["num_steps"] = parse_num_steps(uni_cfg["num_steps"])
+        uni_cfg["write_every"] = parse_num_steps(uni_cfg["write_every"])
+        uni_cfg["write_start"] = parse_num_steps(uni_cfg["write_start"])
+
+        # Write the universe config to file
+        write_yml(uni_cfg, path=uni_cfg_path)
+
+        return uni_cfg
+
+    def _setup_universe_worker_kwargs(
+        self,
+        *,
+        model_executable: str,
+        uni_cfg_path: str,
+        uni_cfg: dict,
+        uni_dir: str,
+        save_streams: bool = False,
+        **worker_kwargs,
+    ) -> dict:
+        """Assembles worker kwargs for a specific universe.
+
+        This is invoked from :py:meth:`~._setup_universe` and is carried out
+        directly before work on that universe starts.
+
+        Returns:
+            dict: the combined worker kwargs, including ``args`` for running
+                the model executable.
+        """
+        # Build args tuple for task assignment; only need to pass the path
+        # to the configuration file
+        args = (model_executable, uni_cfg_path)
+
+        # Assemble the worker_kwargs dict
+        wk = dict(
+            args=args,
+            read_stdout=True,
+            stdout_parser="yaml_dict",
+            save_streams=save_streams,
+            **worker_kwargs,
+        )
+
+        # Determine where to save the streams to, if enabled
+        if save_streams:
+            wk["save_streams_to"] = os.path.join(uni_dir, "{name:}.log")
+
+        return wk
+
+    def _get_TaskCls(self, *, perform_task: bool = True, **_) -> type:
+        if perform_task:
+            return WorkerTask
+        return NoWorkTask
+
     def _add_sim_task(
         self, *, uni_id_str: str, uni_cfg: dict, is_sweep: bool
     ) -> None:
         """Helper function that handles task assignment to the WorkerManager.
 
         This function creates a WorkerTask that will perform the following
         actions **once it is grabbed and worked at**:
@@ -1223,85 +1460,14 @@
             is_sweep (bool): Flag is needed to distinguish between sweeps
                 and single simulations. With this information, the forwarding
                 of a simulation's output stream can be controlled.
 
         Raises:
             RuntimeError: If adding the simulation task failed
         """
-
-        def setup_universe(
-            *,
-            worker_kwargs: dict,
-            model_name: str,
-            model_executable: str,
-            uni_cfg: dict,
-            uni_basename: str,
-        ) -> dict:
-            """The callable that will setup everything needed for a universe.
-
-            This is called before the worker process starts working on the
-            universe.
-
-            Args:
-                worker_kwargs (dict): the current status of the worker_kwargs
-                    dictionary; is always passed to a task setup function
-                model_name (str): The name of the model
-                model_executable (str): path to the binary to execute
-                uni_cfg (dict): the configuration to create a yml file from
-                    which is then needed by the model
-                uni_basename (str): Basename of the universe to use for folder
-                    creation, i.e.: zero-padded universe number, e.g. uni0042
-
-            Returns:
-                dict: kwargs for the process to be run when task is grabbed by
-                    Worker.
-            """
-            # Create universe directory path using the basename
-            uni_dir = os.path.join(self.dirs["data"], uni_basename)
-
-            # Now create the folder
-            os.mkdir(uni_dir)
-            log.debug("Created universe directory:\n  %s", uni_dir)
-
-            # Store it in the configuration
-            uni_cfg["output_dir"] = uni_dir
-
-            # Generate a path to the output hdf5 file and add it to the dict
-            output_path = os.path.join(uni_dir, "data.h5")
-            uni_cfg["output_path"] = output_path
-
-            # Parse the potentially string-valued number of steps values, and
-            # other step-like arguments. Raises an error if they are negative.
-            uni_cfg["num_steps"] = parse_num_steps(uni_cfg["num_steps"])
-            uni_cfg["write_every"] = parse_num_steps(uni_cfg["write_every"])
-            uni_cfg["write_start"] = parse_num_steps(uni_cfg["write_start"])
-
-            # write essential part of config to file:
-            uni_cfg_path = os.path.join(uni_dir, "config.yml")
-            write_yml(uni_cfg, path=uni_cfg_path)
-
-            # Build args tuple for task assignment; only need to pass the path
-            # to the configuration file ...
-            args = (model_executable, uni_cfg_path)
-
-            # Generate a new worker_kwargs dict, carrying over the given ones
-            wk = dict(
-                args=args,
-                read_stdout=True,
-                stdout_parser="yaml_dict",
-                **(worker_kwargs if worker_kwargs else {}),
-            )
-
-            # Determine whether to save the streams (True by default)
-            if wk.get("save_streams", True):
-                # Generate a path and store in the worker kwargs
-                wk["save_streams_to"] = os.path.join(uni_dir, "{name:}.log")
-
-            return wk
-
         # Generate the universe basename, which will be used for the folder
         # and the task name
         uni_basename = f"uni{uni_id_str}"
 
         # Create the dict that will be passed as arguments to setup_universe
         setup_kwargs = dict(
             model_name=self.model_name,
@@ -1315,27 +1481,29 @@
 
         if wk and wk.get("forward_streams") == "in_single_run":
             # Reverse the flag to determine whether to forward streams
             wk["forward_streams"] = not is_sweep
             wk["forward_kwargs"] = dict(forward_raw=True)
 
         # Try to add a task to the worker manager
+        TaskCls = self._get_TaskCls(**wk)
         try:
             self.wm.add_task(
+                TaskCls=TaskCls,
                 name=uni_basename,
                 priority=None,
-                setup_func=setup_universe,
+                setup_func=self._setup_universe,
                 setup_kwargs=setup_kwargs,
                 worker_kwargs=wk,
             )
 
         except RuntimeError as err:
             # Task list was locked, probably because there already was a run
             raise RuntimeError(
-                "Could not add simulation task for universe '{uni_basename}'! "
+                f"Could not add simulation task for universe '{uni_basename}'! "
                 "Did you already perform a run with this Multiverse?"
             ) from err
 
         log.debug("Added simulation task: %s.", uni_basename)
 
     def _add_sim_tasks(self, *, sweep: bool = None) -> int:
         """Adds the simulation tasks needed for a single run or for a sweep.
@@ -1674,15 +1842,15 @@
             # _Additional_ arguments to pass to DataManager.__init__ below
             timestamp = rcps["timestamp"]
             dm_cluster_kwargs = dict(
                 out_dir_kwargs=dict(timestamp=timestamp, exist_ok=True)
             )
 
         # Generate the path to the run directory that is to be loaded
-        self._create_run_dir(**self.meta_cfg["paths"], run_dir=run_dir)
+        self._get_run_dir(**self.meta_cfg["paths"], run_dir=run_dir)
         log.note("Run directory:\n  %s", self.dirs["run"])
 
         # Create a data manager
         self._dm = DataManager(
             self.dirs["run"],
             name=f"{self.model_name}_data",
             **self.meta_cfg["data_manager"],
@@ -1691,101 +1859,335 @@
         log.progress("Initialized DataManager.")
 
         # Instantiate the PlotManager via the helper method
         self._pm = self._setup_pm()
 
         log.progress("Initialized FrozenMultiverse.\n")
 
-    def _create_run_dir(self, *, out_dir: str, run_dir: str, **__):
-        """Helper function to find the run directory from arguments given
-        to :py:meth:`~utopya.multiverse.Multiverse.__init__`.
+    def _create_run_dir(self, *_, **__):
+        """Overload of parent method, for safety: we should not create a new
+        run directory."""
+        raise AttributeError(
+            f"`_create_run_dir` method should not be called from {type(self)}"
+        )
 
-        Overwrites the method from the parent Multiverse class, because the
-        FrozenMultiverse does not require setting up a *new* run directory but
-        should instead identify the existing one and create an appropriate
-        output directory.
+
+# -----------------------------------------------------------------------------
+# -----------------------------------------------------------------------------
+
+
+class DistributedMultiverse(FrozenMultiverse):
+    """A distributed Multiverse is like a Multiverse, but initialized from an
+    existing meta-configuration.
+
+    It re-creates the WorkerManager attributes from that configuration and
+    is not allowed to change the meta-configuration that was loaded.
+    """
+
+    def __init__(
+        self,
+        *,
+        run_dir: str,
+        model_name: str = None,
+        info_bundle: ModelInfoBundle = None,
+    ):
+        """Initializes a DistributedMultiverse from a model name and the name
+        of an existing run directory.
 
         Args:
-            out_dir (str): The output directory
-            run_dir (str): The run directory to use
-            ``**__``: ignored
+            run_dir (str, optional): The run directory to load. Can be a path
+                relative to the current working directory, an absolute path,
+                or the timestamp of the run directory. If not given, will use
+                the most recent timestamp.
+            model_name (str): The name of the model to load. From this, the
+                model output directory is determined and the run_dir will be
+                seen as relative to that directory.
+            info_bundle (ModelInfoBundle, optional): The model information
+                bundle that includes information about the binary path etc.
+                If not given, will attempt to read it from the model registry.
+        """
+        # First things first: get the info bundle
+        if info_bundle is None:
+            info_bundle = get_info_bundle(
+                model_name=model_name, info_bundle=info_bundle
+            )
+        self._info_bundle = info_bundle
 
-        Raises:
-            IOError: No directory found to use as run directory
-            TypeError: When run_dir was not a string
+        log.progress(
+            "Initializing DistributedMultiverse for '%s' model ...",
+            self.model_name,
+        )
+
+        # Initialize property-managed attributes
+        self._dirs = dict()
+        self._model_executable = None
+        self._tmpdir = None
+
+        self._clear_existing_output = False
+
+        # Generate the path to the run directory that is to be loaded
+        # TODO Extract out dir from available infos
+        self._get_run_dir(out_dir=None, run_dir=run_dir)
+        log.note("Run directory:\n  %s", self.dirs["run"])
+
+        # Load the meta config
+        meta_cfg_path = os.path.join(run_dir, "config", "meta_cfg.yml")
+        if not os.path.isfile(meta_cfg_path):
+            raise ValueError(
+                "No meta config found in run dir {} at {}!",
+                run_dir,
+                meta_cfg_path,
+            )
+
+        log.debug("Loading from meta config at %s ...", meta_cfg_path)
+
+        # Only keep selected entries from the meta configuration. The rest is
+        # not needed and is deleted in order to not confuse the user with
+        # potentially varying versions of the meta config.
+        mcfg = load_yml(meta_cfg_path)
+        self._meta_cfg = {
+            k: v
+            for k, v in mcfg.items()
+            if k
+            not in (
+                "data_manager",
+                "plot_manager",
+                "cluster_mode",
+                "cluster_params",
+            )
+        }
+        self._meta_cfg["cluster_mode"] = False
+        log.info("Restored meta-configuration.")
+
+        log.remark("  Debug level:  %d", self.debug_level)
+        self._apply_debug_level()
+
+        # Prepare the executable
+        self._prepare_executable(**self.meta_cfg["executable_control"])
+
+        self._wm = WorkerManager(**self.meta_cfg["worker_manager"])
+        self._reporter = WorkerManagerReporter(
+            self.wm,
+            mv=self,
+            report_dir=self.dirs["run"],
+            **self.meta_cfg["reporter"],
+        )
+
+        log.progress("Initialized DistributedMultiverse.\n")
+
+    def run_selection(
+        self,
+        *,
+        uni_id_strs: List[str],
+        num_workers=None,
+        clear_existing_output: bool = False,
+    ):
+        """Starts a simulation run for specified universes.
+
+        Specifically, this method adds simulation tasks to the associated
+        WorkerManager, locks its task list, and then invokes the
+        :py:meth:`~utopya.workermanager.WorkerManager.start_working` method
+        which performs all the simulation tasks.
+
+        .. note::
+
+            As this method locks the task list of the
+            :py:class:`~utopya.workermanager.WorkerManager`, no further tasks
+            can be added henceforth. This means, that each Multiverse instance
+            can only perform a single simulation run.
+
+        Args:
+            uni_id_strs(List[str]): The list of universe ID strings to run,
+                e.g. '00154'. Note that leading zeros are required.
+            num_workers (int, optional): Specify the number of workers
+                to use, overwriting the setting from the meta-configuration.
+            clear_existing_output (bool, optional): Whether to remove
+                existing files from the universe outpout directories.
+                Only the configuration file will not be deleted.
         """
-        PATTERN = r"\d{6}-\d{6}_?.*"
+        log.info(
+            "Preparing for simulation run of %d universe(s) (%s) ...",
+            len(uni_id_strs),
+            uni_id_strs,
+        )
 
-        # Create model directory path (where the to-be-loaded data is expected)
-        out_dir = os.path.expanduser(str(out_dir))
-        model_dir = os.path.join(out_dir, self.model_name)
+        # Store parameter, used during universe dir setup
+        self._clear_existing_output = clear_existing_output
 
-        if not os.path.isdir(model_dir):
-            # Just create it, there's no harm in that ...
-            os.makedirs(model_dir)
+        # Generate all possible parameter space combinations
+        pspace = self.meta_cfg["parameter_space"]
+        psp_iter = pspace.iterator(with_info="state_no_str")
 
-        # Distinguish different types of values for the run_dir argument
-        if run_dir is None:
-            log.info("Trying to identify the most recent run directory ...")
+        uni_cfgs = dict()
+        for uni_cfg, uni_id_str in psp_iter:
+            uni_cfgs[uni_id_str] = uni_cfg
+
+        # Now, add the respective tasks, if the selection matches
+        is_sweep = len(uni_id_strs) > 1
+        for i, uni_id_str in enumerate(uni_id_strs):
+            if uni_id_str.startswith("uni"):
+                uni_id_str = uni_id_str[3:]
+
+            uni_cfg = uni_cfgs.get(uni_id_str, None)
+            if uni_cfg is None:
+                raise ValueError(f"No universe '{uni_id_str}' found!")
+
+            self._add_sim_task(
+                uni_id_str=uni_id_str,
+                uni_cfg=uni_cfg,
+                is_sweep=is_sweep,
+            )
 
-            # Create list of _directories_ matching timestamp pattern
-            dirs = [
-                d
-                for d in sorted(os.listdir(model_dir))
-                if os.path.isdir(os.path.join(model_dir, d))
-                and re.match(PATTERN, os.path.basename(d))
-            ]
+        self.wm.tasks.lock()
+        if num_workers is not None:
+            self.wm.num_workers = num_workers
 
-            if not dirs:
-                raise FileNotFoundError(
-                    "Could not find a run directory to load for evaluation "
-                    f"of model '{self.model_name}'!\n"
-                    f"Model output directory:  {model_dir}\n\n"
-                    "Did you perform a simulation yet? If you are using this "
-                    "model only for evaluation, place your data in a new "
-                    "subdirectory in that folder (using timestamp as name)."
-                )
+        # Tell the WorkerManager to start working (is a blocking call)
+        self.wm.start_working(**self.meta_cfg["run_kwargs"])
 
-            # Use the latest to choose the run directory
-            run_dir = os.path.join(model_dir, dirs[-1])
+        # Done! :)
+        log.success("Finished simulation run. Wohoo. :)\n")
 
-        elif isinstance(run_dir, str):
-            run_dir = os.path.expanduser(run_dir)
+    def run(
+        self,
+        *,
+        num_workers=None,
+        clear_existing_output: bool = False,
+        skip_existing_output: bool = False,
+    ):
+        """Starts a simulation run for all universes.
 
-            # Distinguish absolute and relative paths and those starting with
-            # a timestamp-like pattern, which can be looked up from the model
-            # directory.
-            if os.path.isabs(run_dir):
-                log.debug("Received absolute run_dir, using that one.")
+        Overload of parent method that allows for universes to be skipped if
+        output already exists from a previous run.
 
-            elif re.match(PATTERN, run_dir):
-                # Looks like a relative path within the model directory
-                log.info(
-                    "Received timestamp '%s' for run_dir; trying to find "
-                    "one within the model output directory ...",
-                    run_dir,
-                )
-                run_dir = os.path.join(model_dir, run_dir)
+        Args:
+            num_workers (int, optional): Specify the number of workers
+                available.
+            clear_existing_output (bool, optional): Whether to remove
+                files in the output directory of the universes other than the
+                configuration file.
+            skip_existing_output (bool, optional): Whether to skip
+                universes if output already exists.
+        """
+        ALLOWED_FILES = ("config.yml",)  # make sure these are sorted
+
+        log.info("Preparing for repeated simulation run ...")
+
+        # Store parameter, used during universe dir setup
+        self._clear_existing_output = clear_existing_output
+
+        # Generate all possible parameter space combinations
+        pspace = self.meta_cfg["parameter_space"]
+        psp_iter = pspace.iterator(with_info="state_no_str")
+
+        # Gather uni configs
+        # TODO Rework this: skip-existing decision should be taken later!
+        uni_cfgs = dict()
+        for uni_cfg, uni_id_str in psp_iter:
+            if skip_existing_output:
+                output_exists = False
+                uni_basename = f"uni{uni_id_str}"
+                uni_dir = os.path.join(self.dirs["data"], uni_basename)
+
+                # Check existence of path and its content
+                if os.path.isdir(uni_dir):
+                    for file in os.listdir(uni_dir):
+                        if file not in ALLOWED_FILES:
+                            output_exists = True
+                            break
+
+                # only add uni to tasks if no output exists
+                if not output_exists:
+                    uni_cfgs[uni_id_str] = uni_cfg
 
             else:
-                # Is not an absolute path and not a timestamp; thus a path
-                # relative to the current working directory
-                run_dir = os.path.join(os.getcwd(), run_dir)
+                uni_cfgs[uni_id_str] = uni_cfg
 
-        else:
-            raise TypeError(
-                "Argument run_dir needs to be None, an absolute "
-                "path, or a path relative to the model output "
-                f"directory, but it was: {run_dir}"
+        log.info("  Found %d universe(s) to work on.", len(uni_cfgs))
+
+        # Now, add the respective tasks, if the selection matches
+        is_sweep = len(uni_cfgs) > 1
+        for uni_id_str, uni_cfg in uni_cfgs.items():
+            self._add_sim_task(
+                uni_id_str=uni_id_str,
+                uni_cfg=uni_cfg,
+                is_sweep=is_sweep,
             )
 
-        # Check if the directory exists
-        if not os.path.isdir(run_dir):
-            raise OSError(f"No run directory found at '{run_dir}'!")
+        self.wm.tasks.lock()
+        if num_workers is not None:
+            self.wm.num_workers = num_workers
 
-        # Store the path and associate the subdirectories
-        self.dirs["run"] = run_dir
+        # Tell the WorkerManager to start working (is a blocking call)
+        self.wm.start_working(**self.meta_cfg["run_kwargs"])
 
-        for subdir in ("config", "eval", "data"):
-            subdir_path = os.path.join(run_dir, subdir)
-            self.dirs[subdir] = subdir_path
-            # TODO Consider checking if it exists?
+        # Done! :)
+        log.success("Finished simulation run. Wohoo. :)\n")
+
+    def _prepare_executable(self, *args, **kwargs) -> None:
+        if self.meta_cfg["backups"]["backup_executable"]:
+            execpath = os.path.join(
+                self.dirs["run"], "backup", self.model_name
+            )
+            if not os.path.isfile(execpath):
+                raise FileNotFoundError(f"No executable found at {execpath}!")
+            log.remark("Restored executable at:\n  %s", execpath)
+
+            self._model_executable = execpath
+
+        return super()._prepare_executable(*args, **kwargs)
+
+    def _perform_pspace_backup(*args, **kwargs):
+        log.debug(
+            "  Skipping parameter space backup (was already read from backup)."
+        )
+
+    # .. Overloads for universe setup .........................................
+
+    def _get_TaskCls(self, **_) -> type:
+        return WorkerTask
+
+    def _setup_universe_dir(self, uni_dir: str, *, uni_basename: str):
+        """Overload of parent method that allows for universe directories to
+        already exist."""
+        ALLOWED_FILES = ("config.yml",)  # make sure these are sorted
+
+        if not os.path.isdir(uni_dir):
+            # Easy, set up from scratch:
+            super()._setup_universe_dir(
+                uni_dir=uni_dir, uni_basename=uni_basename
+            )
+            return
+
+        # else: already exists.
+        # Allow to remove existing output from the directory
+        if self._clear_existing_output and len(os.listdir(uni_dir)) > 1:
+            for file in os.listdir(uni_dir):
+                if file in ALLOWED_FILES:
+                    continue
+                os.remove(os.path.join(uni_dir, file))
+
+        # Check that the universe directory is empty
+        existing_files = os.listdir(uni_dir)
+        if existing_files and sorted(existing_files) != list(ALLOWED_FILES):
+            raise RuntimeError(
+                f"Output directory of universe '{uni_basename}' contains "
+                f"files other than ({', '.join(ALLOWED_FILES)}). "
+                "Did you already perform a run on this universe? "
+                f"Found the following files:  {', '.join(existing_files)}"
+            )
+
+    def _setup_universe_config(self, *, uni_cfg_path: str, **kwargs) -> dict:
+        """Overload of parent method that checks if a universe config already
+        exists and, if so, loads that one instead of storing a new one.
+        """
+        if os.path.isfile(uni_cfg_path):
+            # Can restore it
+            log.debug("Restoring universe config from:\n  %s.", uni_cfg_path)
+            uni_cfg = load_yml(uni_cfg_path)
+        else:
+            # Need to create it
+            uni_cfg = super()._setup_universe_config(
+                uni_cfg_path=uni_cfg_path, **kwargs
+            )
+
+        return uni_cfg
```

### Comparing `utopya-1.3.0b1/utopya/parameter.py` & `utopya-1.3.0b3/utopya/parameter.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/utopya/plotting.py` & `utopya-1.3.0b3/utopya/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """**DEPRECATED** module that provides backwards-compatibility for the old
 utopya module structure.
 
 .. deprecated:: 1.0.0
 
     This module will be removed soon, please use :py:mod:`utopya.eval` instead.
 """
+
 import warnings
 
 from .eval import MultiverseGroup, PlotManager, UniverseGroup
 from .eval.plotcreators import MultiversePlotCreator, UniversePlotCreator
 from .eval.plothelper import PlotHelper
 from .eval.plots import is_plot_func
 from .eval.transform import register_operation
```

### Comparing `utopya-1.3.0b1/utopya/project_registry.py` & `utopya-1.3.0b3/utopya/project_registry.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/utopya/reporter.py` & `utopya-1.3.0b3/utopya/reporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -262,15 +262,15 @@
                 the ``**kwargs`` to the writer function.
             min_report_intv (float, optional): The minimum report interval (in
                 seconds) for this report format
             rf_kwargs (dict, optional): Further kwargs to ReportFormat.__init__
             **parser_kwargs: The kwargs to the parser function
 
         Raises:
-            ValueError: A report format with this `name` already exists
+            ValueError: A report format with this ``name`` already exists
         """
         if name in self.report_formats:
             raise ValueError(
                 f"A report format with the name '{name}' already exists."
             )
 
         # Get the parser and writer function
@@ -659,25 +659,25 @@
                 "because it is needed by the WorkerManager."
             )
 
             self.add_report_format(
                 "after_work", parser="progress_bar", write_to="stdout_noreturn"
             )
 
-        # Store the WorkerManager and associate it with this reporter
-        self._wm = wm
-        wm.reporter = self
-        log.debug("Associated reporter with WorkerManager.")
-
         # Other attributes
         self.mv = mv
         self.runtimes = []
         self.exit_codes = Counter()
         self._eta_info = dict()
 
+        # Store the WorkerManager and associate it with this reporter
+        self._wm = wm
+        wm.reporter = self
+        log.debug("Associated reporter with WorkerManager.")
+
         log.debug("WorkerManagerReporter initialised.")
 
     @property
     def wm(self) -> "utopya.workermanager.WorkerManager":
         """Returns the associated
         :py:class:`~utopya.workermanager.WorkerManager`
         """
@@ -1359,15 +1359,17 @@
                             v=format_time(rt, ms_precision=1),
                             w=max_name_len,
                         )
                     ]
 
         return " \n".join(parts)
 
-    def _parse_pspace_info(self, *, fstr: str, report_no: int = None) -> str:
+    def _parse_pspace_info(
+        self, *, fstr: str, only_for_sweep: bool = True, report_no: int = None
+    ) -> str:
         """Provides information about the parameter space.
 
         Extracts the ``parameter_space`` from the associated Multiverse's meta
         configuration and provides information on that.
 
         If there are multiple tasks specified, it is assumed that a sweep is or
         was being carried out and an information string is retrieved from the
@@ -1391,20 +1393,18 @@
                 "Cannot parse ParamSpace information."
             )
 
         pspace = self.mv.meta_cfg["parameter_space"]
         if not isinstance(pspace, psp.ParamSpace):
             raise TypeError(f"Expected a ParamSpace object, got:\n\n{pspace}")
 
-        if len(self.wm.tasks) <= 1:
+        if only_for_sweep and len(self.wm.tasks) <= 1:
             return ""
 
-        return fstr.format(
-            num_tasks=len(self.wm.tasks), sweep_info=pspace.get_info_str()
-        )
+        return fstr.format(sweep_info=pspace.get_info_str())
 
     # Writer methods ..........................................................
 
     def _write_to_file(
         self,
         *args,
         path: str = "_report.txt",
```

### Comparing `utopya-1.3.0b1/utopya/stop_conditions.py` & `utopya-1.3.0b3/utopya/stop_conditions.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/utopya/task.py` & `utopya-1.3.0b3/utopya/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -1093,14 +1093,109 @@
             "Task %s: worker finished with status %s.",
             self.name,
             self.worker_status,
         )
 
 
 # -----------------------------------------------------------------------------
+
+
+class NoWorkTask(WorkerTask):
+    """A WorkerTask specialization that does not spawn the worker.
+
+    It is mostly equivalent to :py:class:`~utopya.task.WorkerTask` but adjusts
+    the private methods that take care of spawning the actual process and
+    skips the actual work.
+    """
+
+    @property
+    def worker(self) -> subprocess.Popen:
+        """The associated worker process object or None, if not yet created."""
+        return self._worker
+
+    @worker.setter
+    def worker(self, proc: subprocess.Popen):
+        """Set the associated worker process of this task."""
+        if proc is not None:
+            raise RuntimeError("NoWorkTask does not accept an active worker!")
+
+    @property
+    def worker_pid(self) -> int:
+        """The process ID of the associated worker process"""
+        raise RuntimeError("NoWorkTask does not have an active worker!")
+
+    @property
+    def worker_status(self) -> Union[int, None]:
+        """The worker processe's current status or False, if there is no
+        worker spawned yet.
+
+        Note that the worker is inactive after it was spawned.
+
+        Returns:
+            Union[int, None]: Current worker status. False, if there was no
+                worker associated yet.
+        """
+        if self._worker_status is None:
+            return False
+
+        return self._worker_status
+
+    @property
+    def outstream_objs(self) -> list:
+        """Returns the list of objects parsed from the 'out' stream"""
+        if not self.streams:
+            return []
+        return self.streams["out"]["log_parsed"]
+
+    def spawn_worker(self) -> None:
+        """Spawn a void process.
+
+        Returns:
+            None
+
+        Raises:
+            RuntimeError: If a worker was already spawned for this task.
+        """
+        if self._worker_status is not None:
+            raise RuntimeError("Can only spawn one worker per task!")
+
+        # If a setup function is available, call it with the given kwargs
+        if self.setup_func:
+            log.debug("Calling a setup function ...")
+            worker_kwargs = self.setup_func(
+                worker_kwargs=self.worker_kwargs, **self.setup_kwargs
+            )
+        else:
+            log.debug("No setup function given; using given `worker_kwargs`")
+            worker_kwargs = self.worker_kwargs
+
+        self.profiling["create_time"] = time.time()
+        log.debug("This is a NoWorkTask: Skipping to work on task.")
+        self._worker_status = 0
+        self._finished()
+
+        return None
+
+    def _setup_stream_reader(
+        self,
+        stream_name: str,
+        **_,
+    ):
+        raise RuntimeError("NoWorkTasks cannot have a stream!")
+
+    def signal_worker(self, signal: str) -> tuple:
+        """Overwrites signal_worker from WorkerTask
+
+        Raises:
+            RuntimeError: It is not possible to signal a NoWorkTask.
+        """
+        raise RuntimeError("Cannot signal to a terminated worker!")
+
+
+# -----------------------------------------------------------------------------
 # ... working with the multiprocessing module
 
 
 def _target_wrapper(target, streams: dict, *args, **kwargs):
     """A wrapper around the multiprocessing.Process target function which
     takes care of stream handling.
     """
```

### Comparing `utopya-1.3.0b1/utopya/testtools.py` & `utopya-1.3.0b3/utopya/testtools.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/utopya/tools.py` & `utopya-1.3.0b3/utopya/tools.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/utopya/workermanager.py` & `utopya-1.3.0b3/utopya/workermanager.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import logging
 import os
 import queue
 import sys
 import time
 import warnings
 from datetime import datetime as dt
-from typing import Callable, Dict, List, Sequence, Set, Union
+from typing import Callable, Dict, List, Optional, Sequence, Set, Union
 
 from .exceptions import *
 from .reporter import WorkerManagerReporter
 from .stop_conditions import SIG_STOPCOND, StopCondition
 from .task import SIGMAP, TaskList, WorkerTask
 from .tools import format_time
 
@@ -55,14 +55,15 @@
     allows for other threads that have access to the WorkerManager to add an
     exception and let it be handled in the main thread.
     """
     rf_spec: dict = None
     """The report format specifications that are used throughout the
     WorkerManager. These are invoked at different points of the operation:
 
+    - ``before_working``
     - ``while_working``
     - ``after_work``
     - ``after_abort``
     - ``task_spawn``
     - ``task_finished``
     """
 
@@ -108,15 +109,16 @@
             QueueCls (type, optional): Which class to use for the queue.
                 Defaults to the FiFo :py:class:`queue.Queue`.
             reporter (WorkerManagerReporter, optional): The reporter associated
                 with this WorkerManager, reporting on the progress.
             rf_spec (Dict[str, Union[str, List[str]]], optional): The names of
                 report formats that should be invoked at different points of
                 the WorkerManager's operation.
-                Possible keys: ``before_working``, ``while_working``,
+                Possible keys:
+                ``before_working``, ``while_working``,
                 ``after_work``, ``after_abort``, ``task_spawn``,
                 ``task_finished``. All other keys are ignored.
 
                 The values of the dict can be either strings or lists of
                 strings, where the strings always refer to report formats
                 registered with the WorkerManagerReporter. This argument
                 updates the default report format specifications.
@@ -531,15 +533,14 @@
 
         log.debug("Task %s (uid: %s) added.", task.name, task.uid)
         return task
 
     def start_working(
         self,
         *,
-        detach: bool = False,
         timeout: float = None,
         stop_conditions: Sequence[StopCondition] = None,
         post_poll_func: Callable = None,
     ) -> None:
         """Upon call, all enqueued tasks will be worked on sequentially.
 
         Args:
@@ -553,89 +554,56 @@
             stop_conditions (Sequence[StopCondition], optional): During the
                 run these StopCondition objects will be checked
             post_poll_func (Callable, optional): If given, this is called after
                 all workers have been polled. It can be used to perform custom
                 actions during a the polling loop.
 
         Raises:
-            NotImplementedError: if ``detach`` was set
             ValueError: For invalid (i.e., negative) timeout value
             WorkerManagerTotalTimeout: Upon a total timeout
         """
-        if detach:
-            raise NotImplementedError(
-                "It is currently not possible to detach the WorkerManager "
-                "from the main thread."
-            )
-
         self._invoke_report("before_working")
 
         log.progress("Preparing to work ...")
 
-        # Determine timeout arguments
-        if timeout:
-            if timeout <= 0:
-                raise ValueError(
-                    f"Invalid value for argument `timeout`: {timeout} -- "
-                    "needs to be positive."
-                )
-
-            # Already calculate the time after which a timeout would be reached
-            self.times["timeout"] = time.time() + timeout
-
-        # Set the variable needed for checking; if above condition was not
-        # fulfilled, this will be None
-        timeout_time = self.times["timeout"]
-
         # Set some variables needed during the run
         poll_no = 0
         self.times["start_working"] = dt.now()
 
-        # Prepare stop conditions, creating objects if needed
-        if stop_conditions:
-            stop_conditions = [
-                sc if isinstance(sc, StopCondition) else StopCondition(**sc)
-                for sc in stop_conditions
-            ]
-
-        # Inform about timeout and stop conditions
-        if timeout:
-            _to_fstr = "%X" if timeout < 60 * 60 * 12 else "%X, %d.%m.%y"
-            _to_at = dt.fromtimestamp(timeout_time).strftime(_to_fstr)
-        log.note(
-            "  Timeout:         %s",
-            "None" if not timeout else f"{_to_at} (in {format_time(timeout)})",
-        )
-        log.note(
-            "  Stop conditions: %s",
-            "None"
-            if not stop_conditions
-            else ", ".join([sc.name for sc in stop_conditions]),
-        )
-
-        log.hilight("Starting to work ...")
-
-        # Keep track of the stop condition objects
-        if stop_conditions:
-            self._stop_conditions.update(set(stop_conditions))
+        # Prepare timeout and stop conditions
+        timeout_time = self._parse_timeout_args(timeout=timeout)
+        stop_conditions = self._parse_stop_conditions(stop_conditions)
 
         # Start with the polling loop
         # Basically all working time will be spent in there ...
+        log.hilight("Starting to work ...")
+
         try:
             while self.active_tasks or self.task_queue.qsize() > 0:
                 # Check total timeout
                 if timeout_time is not None and time.time() > timeout_time:
                     raise WorkerManagerTotalTimeout()
 
                 # Check if there was another reason for exiting
                 self._handle_pending_exceptions()
 
                 # Assign tasks to free workers
                 self._assign_tasks(self.num_free_workers)
 
+                # Poll the workers. (Will also remove no longer active workers)
+                self._poll_workers()
+
+                # Call the post-poll function
+                if post_poll_func is not None:
+                    log.debug(
+                        "Calling post_poll_func %s ...",
+                        post_poll_func.__name__,
+                    )
+                    post_poll_func()
+
                 # Do stream-related actions for each task
                 for task in self.active_tasks:
                     # Read the streams and forward them (if the tasks were
                     # configured to do so)
                     task.read_streams(
                         forward_directly=True,
                         max_num_reads=self.lines_per_poll,
@@ -651,25 +619,14 @@
                     # were fulfilled and store them.
                     fulfilled = self._check_stop_conds(stop_conditions)
                     self.stopped_tasks += fulfilled
 
                     # Now signal those workers such that they terminate.
                     self._signal_workers(fulfilled, signal=SIG_STOPCOND)
 
-                # Poll the workers. (Will also remove no longer active workers)
-                self._poll_workers()
-
-                # Call the post-poll function
-                if post_poll_func is not None:
-                    log.debug(
-                        "Calling post_poll_func %s ...",
-                        post_poll_func.__name__,
-                    )
-                    post_poll_func()
-
                 # Invoke periodic callback for all tasks
                 if (
                     self._periodic_callback
                     and poll_no % self._periodic_callback == 0
                 ):
                     self._invoke_periodic_callbacks()
 
@@ -687,85 +644,15 @@
             # Finished working
             # Handle any remaining pending exceptions
             self._handle_pending_exceptions()
 
         except (KeyboardInterrupt, WorkerManagerTotalTimeout) as exc:
             # Got interrupted or a total timeout.
             # Interrupt the workers, giving them some time to shut down ...
-
-            # Suppress reporter to use CR; then inform via log messages
-            if self.reporter:
-                self.reporter.suppress_cr = True
-
-            log.warning("Received %s.", type(exc).__name__)
-
-            # Extract parameters from config
-            # Which signal to send to workers
-            signal = self.interrupt_params.get("send_signal", "SIGINT")
-
-            # The grace period within which the tasks have to shut down
-            grace_period = self.interrupt_params.get("grace_period", 5.0)
-
-            # Send the signal
-            log.info(
-                "Sending signal %s to %d active task(s) ...",
-                signal,
-                len(self.active_tasks),
-            )
-            self._signal_workers(self.active_tasks, signal=signal)
-
-            # Continuously poll them for a certain grace period in order to
-            # find out if they have shut down.
-            log.warning(
-                "Allowing %s for %d task(s) to shut down ... "
-                "(Ctrl + C to kill them now.)",
-                format_time(grace_period, ms_precision=1),
-                len(self.active_tasks),
-            )
-            grace_period_start = time.time()
-
-            try:
-                while True:
-                    self._poll_workers()
-
-                    # Check whether to leave the loop
-                    if not self.active_tasks:
-                        break
-                    elif time.time() > grace_period_start + grace_period:
-                        raise KeyboardInterrupt
-
-                    # Need to continue. Delay polling ...
-                    time.sleep(self.poll_delay)
-
-            except KeyboardInterrupt:
-                log.critical(
-                    "Killing workers of %d tasks now ...",
-                    len(self.active_tasks),
-                )
-                self._signal_workers(self.active_tasks, signal="SIGKILL")
-
-                # Wait briefly (killing shouldn't take long), then poll
-                # one last time to update all task's status.
-                time.sleep(0.5)
-                self._poll_workers()
-
-            # Store end time and invoke a report
-            self.times["end_working"] = dt.now()
-            self._invoke_report("after_abort", force=True)
-
-            log.hilight("Work session ended.")
-
-            if type(exc) is KeyboardInterrupt and self.interrupt_params.get(
-                "exit", True
-            ):
-                # Exit with appropriate exit code (128 + abs(signum))
-                log.warning("Exiting after KeyboardInterrupt ...")
-                sys.exit(128 + abs(SIGMAP[signal]))
-
-            # Otherwise, just return control to the calling scope
+            self._handle_KeyboardInterrupt_or_TotalTimeout(exc)
 
         except WorkerManagerError as err:
             # Some error not related to the non-zero exit code occurred.
             # Gracefully terminate remaining tasks before re-raising the
             # exception
 
             # Suppress reporter to use CR; then inform via log messages
@@ -808,23 +695,72 @@
             return
 
         # Check whether to suppress this rf_spec
         if self._suppress_rf_specs and rf_spec_name in self._suppress_rf_specs:
             # Do not report this one
             return
 
-        # Resolve the spec name
+        # Resolve the spec name and invoke the reports
         rfs = self.rf_spec[rf_spec_name]
-
         if not isinstance(rfs, list):
             rfs = [rfs]
 
         for rf in rfs:
             self.reporter.report(rf, *args, **kwargs)
 
+    def _parse_timeout_args(
+        self, *, timeout: Optional[float]
+    ) -> Optional[float]:
+        """Parses timeout-related arguments"""
+        # Determine timeout arguments
+        if not timeout:
+            log.note("  Timeout:         None")
+            return None
+
+        if timeout <= 0:
+            raise ValueError(
+                f"Invalid value for argument `timeout`: {timeout} -- "
+                "needs to be positive."
+            )
+
+        # Calculate the time after which a timeout would be reached
+        timeout_time = time.time() + timeout
+        self.times["timeout"] = timeout_time
+
+        # Inform about timeout
+        _to_fstr = "%X" if timeout < 60 * 60 * 12 else "%X, %d.%m.%y"
+        _to_at = dt.fromtimestamp(timeout_time).strftime(_to_fstr)
+        log.note(
+            "  Timeout:         %s", f"{_to_at} (in {format_time(timeout)})"
+        )
+
+        return self.times["timeout"]
+
+    def _parse_stop_conditions(
+        self, stop_conditions: Optional[list]
+    ) -> Optional[List[StopCondition]]:
+        """Prepare stop conditions, creating the corresponding objects if
+        needed."""
+        if not stop_conditions:
+            log.note("  Stop conditions: None")
+            return
+
+        stop_conditions = [
+            sc if isinstance(sc, StopCondition) else StopCondition(**sc)
+            for sc in stop_conditions
+        ]
+        self._stop_conditions.update(set(stop_conditions))
+
+        log.note(
+            "  Stop conditions: %s",
+            ", ".join([sc.name for sc in stop_conditions]),
+        )
+
+        return stop_conditions
+
     def _grab_task(self) -> WorkerTask:
         """Will initiate that a task is gotten from the queue and that it
         spawns its worker process.
 
         Returns:
             WorkerTask: The WorkerTask grabbed from the queue.
 
@@ -1089,7 +1025,79 @@
 
             # By raising here, the except block in start_working will be
             # invoked and terminate workers before calling sys.exit
             raise exc
 
         # The pending_exceptions list is now empty
         log.debug("Handled all pending exceptions.")
+
+    def _handle_KeyboardInterrupt_or_TotalTimeout(self, exc: Exception):
+        # Suppress reporter to use CR; then inform via log messages
+        if self.reporter:
+            self.reporter.suppress_cr = True
+
+        log.warning("Received %s.", type(exc).__name__)
+
+        # Extract parameters from config
+        # Which signal to send to workers
+        signal = self.interrupt_params.get("send_signal", "SIGINT")
+
+        # The grace period within which the tasks have to shut down
+        grace_period = self.interrupt_params.get("grace_period", 5.0)
+
+        # Send the signal
+        log.info(
+            "Sending signal %s to %d active task(s) ...",
+            signal,
+            len(self.active_tasks),
+        )
+        self._signal_workers(self.active_tasks, signal=signal)
+
+        # Continuously poll them for a certain grace period in order to
+        # find out if they have shut down.
+        log.warning(
+            "Allowing %s for %d task(s) to shut down ... "
+            "(Ctrl + C to kill them now.)",
+            format_time(grace_period, ms_precision=1),
+            len(self.active_tasks),
+        )
+        grace_period_start = time.time()
+
+        try:
+            while True:
+                self._poll_workers()
+
+                # Check whether to leave the loop
+                if not self.active_tasks:
+                    break
+                elif time.time() > grace_period_start + grace_period:
+                    raise KeyboardInterrupt
+
+                # Need to continue. Delay polling ...
+                time.sleep(self.poll_delay)
+
+        except KeyboardInterrupt:
+            log.critical(
+                "Killing workers of %d tasks now ...",
+                len(self.active_tasks),
+            )
+            self._signal_workers(self.active_tasks, signal="SIGKILL")
+
+            # Wait briefly (killing shouldn't take long), then poll
+            # one last time to update all task's status.
+            time.sleep(0.5)
+            self._poll_workers()
+
+        # Store end time and invoke a report
+        self.times["end_working"] = dt.now()
+        self._invoke_report("after_abort", force=True)
+
+        log.hilight("Work session ended.")
+
+        exit = self.interrupt_params.get("exit", True)
+        if type(exc) is KeyboardInterrupt and exit:
+            # Exit with appropriate exit code (128 + abs(signum))
+            log.warning("Exiting after KeyboardInterrupt ...")
+            sys.exit(128 + abs(SIGMAP[signal]))
+
+        # Otherwise, just return control to the calling scope
+        return
```

### Comparing `utopya-1.3.0b1/utopya/yaml.py` & `utopya-1.3.0b3/utopya/yaml.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/utopya.egg-info/PKG-INFO` & `utopya-1.3.0b3/utopya.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utopya
-Version: 1.3.0b1
+Version: 1.3.0b3
 Summary: A simulation management and evaluation framework
 Home-page: https://gitlab.com/utopia-project/utopya
 Author: utopya developers
 Author-email: Yunus Sevinchan <yunus.sevinchan@hu-berlin.de>
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `utopya-1.3.0b1/utopya.egg-info/SOURCES.txt` & `utopya-1.3.0b3/utopya.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 tests/eval/test_datamanager.py
 tests/eval/test_groups.py
 tests/eval/test_plot_utils.py
 tests/eval/test_plotting.py
 utopya/__init__.py
 utopya/_cluster.py
 utopya/_import_tools.py
+utopya/_logging.py
 utopya/_signal.py
 utopya/_yaml.py
 utopya/batch.py
 utopya/cfg.py
 utopya/exceptions.py
 utopya/model.py
 utopya/multiverse.py
@@ -103,8 +104,9 @@
 utopya_cli/batch.py
 utopya_cli/cli.py
 utopya_cli/config.py
 utopya_cli/eval.py
 utopya_cli/models.py
 utopya_cli/projects.py
 utopya_cli/run.py
+utopya_cli/run_existing.py
 utopya_cli/test.py
```

### Comparing `utopya-1.3.0b1/utopya_backend/benchmark.py` & `utopya-1.3.0b3/utopya_backend/benchmark.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/utopya_backend/logging.py` & `utopya-1.3.0b3/utopya_backend/logging.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/utopya_backend/model/__init__.py` & `utopya-1.3.0b3/utopya_backend/model/__init__.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/utopya_backend/model/base.py` & `utopya-1.3.0b3/utopya_backend/model/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -421,14 +421,15 @@
 
         if t > self._last_emit + self._monitor_emit_interval:
             return True
         return False
 
     def _emit_monitor(self):
         """Actually emits the monitoring information using :py:func:`print`."""
+
         # TODO Consider using YAML for creating the monitor string
         def parse_val(v) -> str:
             if isinstance(v, float):
                 return f"{v:6g}"
             return repr(v)
 
         progress = str(self.compute_progress())
```

### Comparing `utopya-1.3.0b1/utopya_backend/model/step.py` & `utopya-1.3.0b3/utopya_backend/model/step.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/utopya_backend/signal.py` & `utopya-1.3.0b3/utopya_backend/signal.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/utopya_backend/tools.py` & `utopya-1.3.0b3/utopya_backend/tools.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/utopya_cli/_copy_model.py` & `utopya-1.3.0b3/utopya_cli/_copy_model.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/utopya_cli/_shared.py` & `utopya-1.3.0b3/utopya_cli/_shared.py`

 * *Files 9% similar despite different names*

```diff
@@ -233,14 +233,28 @@
     click.option(
         "--cluster-mode",
         flag_value=True,
         default=None,
         help="Enables cluster mode.",
     ),
 )
+OPTIONS["num_workers"] = (
+    click.option(
+        "-W",
+        "--num-workers",
+        default=None,
+        type=click.IntRange(min=-os.cpu_count() + 1, max=+os.cpu_count()),
+        help=(
+            "Shortcut for meta-config entry ``worker_manager.num_workers``, "
+            "which sets the number of worker processes. "
+            "Can be an integer; if negative, will deduce the number from the "
+            "number of available CPUs."
+        ),
+    ),
+)
 
 # -- Data loading options
 OPTIONS["load"] = (
     click.option(
         "-P",
         "--load-parallel",
         flag_value=True,
```

### Comparing `utopya-1.3.0b1/utopya_cli/_utils.py` & `utopya-1.3.0b3/utopya_cli/_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -446,14 +446,33 @@
         if args.run_mode is not None:
             add_item(
                 args.run_mode == "sweep",
                 add_to=update_dict,
                 key_path=("perform_sweep",),
             )
 
+        if args.worker_perform_task is not None:
+            add_item(
+                args.worker_perform_task,
+                add_to=update_dict,
+                key_path=("worker_kwargs", "perform_task"),
+            )
+            if (
+                not args.worker_perform_task
+                and args.perform_eval is not None
+                and args.perform_eval
+            ):
+                raise ValueError("Cannot perform eval after --no-work.")
+            if not args.worker_perform_task and args.perform_eval is None:
+                raise NotImplementedError(
+                    "Please explicityly specify "
+                    "'--no-eval' option together with '--no-work'. Sorry for "
+                    "the inconvenience."
+                )
+
         if args.set_model_params:
             # TODO More elegant solution?
             if not update_dict.get("parameter_space"):
                 update_dict["parameter_space"] = dict()
 
             if not update_dict["parameter_space"].get(args.model_name):
                 update_dict["parameter_space"][args.model_name] = dict()
```

### Comparing `utopya-1.3.0b1/utopya_cli/batch.py` & `utopya-1.3.0b3/utopya_cli/batch.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/utopya_cli/cli.py` & `utopya-1.3.0b3/utopya_cli/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 
 from .batch import batch
 from .config import config
 from .eval import evaluate
 from .models import models
 from .projects import projects
 from .run import run
+from .run_existing import run_existing as __run_existing
 from .test import run_test as test
 
 SUBCOMMANDS = [
     run,
+    __run_existing,
     evaluate,
     test,
     batch,
     config,
     models,
     projects,
 ]
```

### Comparing `utopya-1.3.0b1/utopya_cli/config.py` & `utopya-1.3.0b3/utopya_cli/config.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/utopya_cli/eval.py` & `utopya-1.3.0b3/utopya_cli/eval.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/utopya_cli/models.py` & `utopya-1.3.0b3/utopya_cli/models.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/utopya_cli/projects.py` & `utopya-1.3.0b3/utopya_cli/projects.py`

 * *Files identical despite different names*

### Comparing `utopya-1.3.0b1/utopya_cli/run.py` & `utopya-1.3.0b3/utopya_cli/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,24 @@
     type=click.Choice(("single", "sweep")),
     help=(
         "Forces a single simulation or a sweep. If not given, will use the "
         "value specified in the meta configuration."
     ),
 )
 @click.option(
+    "--no-work",
+    "worker_perform_task",
+    default=True,
+    is_flag=True,
+    help=(
+        "Whether to call WorkerTask or NoWorkTask. NoWorkerTask only creates "
+        "configurations, but does not spawn a worker. No-work implies no-eval."
+    ),
+)
+@click.option(
     "--note",
     default=None,
     type=str,
     help=(
         "A suffix that is appended to the name of the run output directory; "
         "this can be useful to give a name to a certain simulation run."
     ),
```

### Comparing `utopya-1.3.0b1/utopya_cli/test.py` & `utopya-1.3.0b3/utopya_cli/test.py`

 * *Files identical despite different names*

