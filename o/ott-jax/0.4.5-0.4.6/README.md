# Comparing `tmp/ott-jax-0.4.5.tar.gz` & `tmp/ott_jax-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ott-jax-0.4.5.tar", last modified: Tue Jan  2 13:42:46 2024, max compression
+gzip compressed data, was "ott_jax-0.4.6.tar", last modified: Fri Apr 12 16:54:44 2024, max compression
```

## Comparing `ott-jax-0.4.5.tar` & `ott_jax-0.4.6.tar`

### file list

```diff
@@ -1,119 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 13:42:46.416027 ott-jax-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-01-02 13:41:50.000000 ott-jax-0.4.5/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-01-02 13:41:50.000000 ott-jax-0.4.5/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-01-02 13:41:50.000000 ott-jax-0.4.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-01-02 13:41:50.000000 ott-jax-0.4.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-01-02 13:41:50.000000 ott-jax-0.4.5/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-01-02 13:41:50.000000 ott-jax-0.4.5/CITATION.bib
--rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-01-02 13:41:50.000000 ott-jax-0.4.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-01-02 13:41:50.000000 ott-jax-0.4.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-02 13:41:50.000000 ott-jax-0.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-01-02 13:41:50.000000 ott-jax-0.4.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    20840 2024-01-02 13:42:46.416027 ott-jax-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5069 2024-01-02 13:41:50.000000 ott-jax-0.4.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-01-02 13:41:51.000000 ott-jax-0.4.5/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)     8696 2024-01-02 13:41:51.000000 ott-jax-0.4.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-02 13:42:46.416027 ott-jax-0.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-01-02 13:41:51.000000 ott-jax-0.4.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 13:42:46.392027 ott-jax-0.4.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 13:42:46.396027 ott-jax-0.4.5/src/ott/
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 13:42:46.400027 ott-jax-0.4.5/src/ott/geometry/
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37689 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/geometry/costs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/geometry/distrib_costs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/geometry/epsilon_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8601 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/geometry/geodesic.py
--rw-r--r--   0 runner    (1001) docker     (127)    32431 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/geometry/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     8935 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/geometry/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    15339 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/geometry/grid.py
--rw-r--r--   0 runner    (1001) docker     (127)    16682 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/geometry/low_rank.py
--rw-r--r--   0 runner    (1001) docker     (127)    26509 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/geometry/pointcloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     7035 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/geometry/segment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 13:42:46.400027 ott-jax-0.4.5/src/ott/initializers/
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/initializers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 13:42:46.400027 ott-jax-0.4.5/src/ott/initializers/linear/
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/initializers/linear/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12739 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/initializers/linear/initializers.py
--rw-r--r--   0 runner    (1001) docker     (127)    18858 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/initializers/linear/initializers_lr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 13:42:46.400027 ott-jax-0.4.5/src/ott/initializers/quadratic/
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/initializers/quadratic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6599 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/initializers/quadratic/initializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 13:42:46.400027 ott-jax-0.4.5/src/ott/math/
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8395 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/math/fixed_point_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)    10936 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/math/matrix_square_root.py
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/math/unbalanced_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9904 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/math/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 13:42:46.400027 ott-jax-0.4.5/src/ott/neural/
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/neural/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7892 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/neural/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/neural/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)    13616 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/neural/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 13:42:46.400027 ott-jax-0.4.5/src/ott/neural/solvers/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/neural/solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/neural/solvers/conjugate.py
--rw-r--r--   0 runner    (1001) docker     (127)     9944 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/neural/solvers/map_estimator.py
--rw-r--r--   0 runner    (1001) docker     (127)    24937 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/neural/solvers/neuraldual.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 13:42:46.404027 ott-jax-0.4.5/src/ott/problems/
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/problems/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 13:42:46.404027 ott-jax-0.4.5/src/ott/problems/linear/
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/problems/linear/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6892 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/problems/linear/barycenter_problem.py
--rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/problems/linear/linear_problem.py
--rw-r--r--   0 runner    (1001) docker     (127)    14243 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/problems/linear/potentials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 13:42:46.404027 ott-jax-0.4.5/src/ott/problems/quadratic/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/problems/quadratic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11128 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/problems/quadratic/gw_barycenter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/problems/quadratic/quadratic_costs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18895 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/problems/quadratic/quadratic_problem.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 13:42:46.404027 ott-jax-0.4.5/src/ott/solvers/
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/solvers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 13:42:46.408027 ott-jax-0.4.5/src/ott/solvers/linear/
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/solvers/linear/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/solvers/linear/_solve.py
--rw-r--r--   0 runner    (1001) docker     (127)     6365 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/solvers/linear/acceleration.py
--rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/solvers/linear/continuous_barycenter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8466 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/solvers/linear/discrete_barycenter.py
--rw-r--r--   0 runner    (1001) docker     (127)    13701 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/solvers/linear/implicit_differentiation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/solvers/linear/lineax_implicit.py
--rw-r--r--   0 runner    (1001) docker     (127)    11102 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/solvers/linear/lr_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    51278 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/solvers/linear/sinkhorn.py
--rw-r--r--   0 runner    (1001) docker     (127)    26711 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/solvers/linear/sinkhorn_lr.py
--rw-r--r--   0 runner    (1001) docker     (127)    13348 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/solvers/linear/univariate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 13:42:46.408027 ott-jax-0.4.5/src/ott/solvers/quadratic/
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/solvers/quadratic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/solvers/quadratic/_solve.py
--rw-r--r--   0 runner    (1001) docker     (127)    14165 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/solvers/quadratic/gromov_wasserstein.py
--rw-r--r--   0 runner    (1001) docker     (127)    29286 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/solvers/quadratic/gromov_wasserstein_lr.py
--rw-r--r--   0 runner    (1001) docker     (127)    11797 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/solvers/quadratic/gw_barycenter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/solvers/quadratic/lower_bound.py
--rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/solvers/was_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 13:42:46.408027 ott-jax-0.4.5/src/ott/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 13:42:46.412027 ott-jax-0.4.5/src/ott/tools/gaussian_mixture/
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/tools/gaussian_mixture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9108 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/tools/gaussian_mixture/fit_gmm.py
--rw-r--r--   0 runner    (1001) docker     (127)    12063 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/tools/gaussian_mixture/fit_gmm_pair.py
--rw-r--r--   0 runner    (1001) docker     (127)     6429 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/tools/gaussian_mixture/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)    10670 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/tools/gaussian_mixture/gaussian_mixture.py
--rw-r--r--   0 runner    (1001) docker     (127)     7669 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/tools/gaussian_mixture/gaussian_mixture_pair.py
--rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/tools/gaussian_mixture/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/tools/gaussian_mixture/probabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/tools/gaussian_mixture/scale_tril.py
--rw-r--r--   0 runner    (1001) docker     (127)    13649 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/tools/k_means.py
--rw-r--r--   0 runner    (1001) docker     (127)     8275 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/tools/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/tools/segment_sinkhorn.py
--rw-r--r--   0 runner    (1001) docker     (127)    14315 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/tools/sinkhorn_divergence.py
--rw-r--r--   0 runner    (1001) docker     (127)    28718 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/tools/soft_sort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-01-02 13:41:51.000000 ott-jax-0.4.5/src/ott/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 13:42:46.412027 ott-jax-0.4.5/src/ott_jax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20840 2024-01-02 13:42:46.000000 ott-jax-0.4.5/src/ott_jax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-01-02 13:42:46.000000 ott-jax-0.4.5/src/ott_jax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-02 13:42:46.000000 ott-jax-0.4.5/src/ott_jax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-01-02 13:42:46.000000 ott-jax-0.4.5/src/ott_jax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-01-02 13:42:46.000000 ott-jax-0.4.5/src/ott_jax.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:54:44.965899 ott_jax-0.4.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-12 16:53:44.000000 ott_jax-0.4.6/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-12 16:53:44.000000 ott_jax-0.4.6/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-04-12 16:53:44.000000 ott_jax-0.4.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-12 16:53:44.000000 ott_jax-0.4.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-12 16:53:44.000000 ott_jax-0.4.6/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-12 16:53:44.000000 ott_jax-0.4.6/CITATION.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-04-12 16:53:44.000000 ott_jax-0.4.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-04-12 16:53:44.000000 ott_jax-0.4.6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-12 16:53:44.000000 ott_jax-0.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-12 16:53:44.000000 ott_jax-0.4.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    20889 2024-04-12 16:54:44.961899 ott_jax-0.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5069 2024-04-12 16:53:44.000000 ott_jax-0.4.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-12 16:53:44.000000 ott_jax-0.4.6/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     8745 2024-04-12 16:53:44.000000 ott_jax-0.4.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 16:54:44.965899 ott_jax-0.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-12 16:53:44.000000 ott_jax-0.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:54:44.937899 ott_jax-0.4.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:54:44.941899 ott_jax-0.4.6/src/ott/
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:54:44.941899 ott_jax-0.4.6/src/ott/geometry/
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39175 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/geometry/costs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/geometry/distrib_costs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/geometry/epsilon_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9515 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/geometry/geodesic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32264 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/geometry/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8940 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/geometry/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15340 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/geometry/grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16603 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/geometry/low_rank.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25989 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/geometry/pointcloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7035 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/geometry/segment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:54:44.941899 ott_jax-0.4.6/src/ott/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/initializers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:54:44.941899 ott_jax-0.4.6/src/ott/initializers/linear/
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/initializers/linear/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12735 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/initializers/linear/initializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18864 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/initializers/linear/initializers_lr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:54:44.945900 ott_jax-0.4.6/src/ott/initializers/neural/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/initializers/neural/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7352 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/initializers/neural/meta_initializer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:54:44.945900 ott_jax-0.4.6/src/ott/initializers/quadratic/
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/initializers/quadratic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/initializers/quadratic/initializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:54:44.945900 ott_jax-0.4.6/src/ott/math/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8395 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/math/fixed_point_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10835 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/math/matrix_square_root.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/math/unbalanced_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9905 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/math/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:54:44.945900 ott_jax-0.4.6/src/ott/neural/
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/neural/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/neural/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:54:44.945900 ott_jax-0.4.6/src/ott/neural/methods/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/neural/methods/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:54:44.945900 ott_jax-0.4.6/src/ott/neural/methods/flows/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/neural/methods/flows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/neural/methods/flows/dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11628 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/neural/methods/flows/genot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6161 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/neural/methods/flows/otfm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15456 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/neural/methods/monge_gap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20922 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/neural/methods/neuraldual.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:54:44.949900 ott_jax-0.4.6/src/ott/neural/networks/
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/neural/networks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5694 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/neural/networks/icnn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:54:44.949900 ott_jax-0.4.6/src/ott/neural/networks/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/neural/networks/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/neural/networks/layers/conjugate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7872 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/neural/networks/layers/posdef.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/neural/networks/layers/time_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5987 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/neural/networks/potentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/neural/networks/velocity_field.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:54:44.949900 ott_jax-0.4.6/src/ott/problems/
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/problems/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:54:44.949900 ott_jax-0.4.6/src/ott/problems/linear/
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/problems/linear/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6892 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/problems/linear/barycenter_problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/problems/linear/linear_problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14539 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/problems/linear/potentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:54:44.949900 ott_jax-0.4.6/src/ott/problems/quadratic/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/problems/quadratic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11131 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/problems/quadratic/gw_barycenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/problems/quadratic/quadratic_costs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18234 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/problems/quadratic/quadratic_problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:54:44.949900 ott_jax-0.4.6/src/ott/solvers/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/solvers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:54:44.953899 ott_jax-0.4.6/src/ott/solvers/linear/
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/solvers/linear/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/solvers/linear/_solve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6385 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/solvers/linear/acceleration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7633 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/solvers/linear/continuous_barycenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8466 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/solvers/linear/discrete_barycenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13701 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/solvers/linear/implicit_differentiation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/solvers/linear/lineax_implicit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11102 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/solvers/linear/lr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51055 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/solvers/linear/sinkhorn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26677 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/solvers/linear/sinkhorn_lr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13348 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/solvers/linear/univariate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:54:44.953899 ott_jax-0.4.6/src/ott/solvers/quadratic/
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/solvers/quadratic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/solvers/quadratic/_solve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14125 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/solvers/quadratic/gromov_wasserstein.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29609 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/solvers/quadratic/gromov_wasserstein_lr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11797 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/solvers/quadratic/gw_barycenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/solvers/quadratic/lower_bound.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5381 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/solvers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/solvers/was_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:54:44.957899 ott_jax-0.4.6/src/ott/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:54:44.957899 ott_jax-0.4.6/src/ott/tools/gaussian_mixture/
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/tools/gaussian_mixture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9079 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/tools/gaussian_mixture/fit_gmm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12063 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/tools/gaussian_mixture/fit_gmm_pair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6313 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/tools/gaussian_mixture/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10576 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/tools/gaussian_mixture/gaussian_mixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7670 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/tools/gaussian_mixture/gaussian_mixture_pair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/tools/gaussian_mixture/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/tools/gaussian_mixture/probabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6712 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/tools/gaussian_mixture/scale_tril.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13658 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/tools/k_means.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8275 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/tools/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5982 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/tools/segment_sinkhorn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14339 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/tools/sinkhorn_divergence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28726 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/tools/soft_sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6572 2024-04-12 16:53:44.000000 ott_jax-0.4.6/src/ott/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:54:44.961899 ott_jax-0.4.6/src/ott_jax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20889 2024-04-12 16:54:44.000000 ott_jax-0.4.6/src/ott_jax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-04-12 16:54:44.000000 ott_jax-0.4.6/src/ott_jax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 16:54:44.000000 ott_jax-0.4.6/src/ott_jax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-12 16:54:44.000000 ott_jax-0.4.6/src/ott_jax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-12 16:54:44.000000 ott_jax-0.4.6/src/ott_jax.egg-info/top_level.txt
```

### Comparing `ott-jax-0.4.5/.gitignore` & `ott_jax-0.4.6/.gitignore`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.5/.pre-commit-config.yaml` & `ott_jax-0.4.6/.pre-commit-config.yaml`

 * *Files 27% similar despite different names*

```diff
@@ -2,52 +2,56 @@
 default_language_version:
   python: python3
 default_stages:
 - commit
 - push
 minimum_pre_commit_version: 3.0.0
 repos:
-- repo: https://github.com/google/yapf
-  rev: v0.40.0
-  hooks:
-  - id: yapf
-    additional_dependencies: [toml]
-- repo: https://github.com/nbQA-dev/nbQA
-  rev: 1.7.0
-  hooks:
-  - id: nbqa-pyupgrade
-    args: [--py38-plus]
-  - id: nbqa-black
-  - id: nbqa-isort
-- repo: https://github.com/macisamuele/language-formatters-pre-commit-hooks
-  rev: v2.10.0
-  hooks:
-  - id: pretty-format-yaml
-    args: [--autofix, --indent, '2']
 - repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v4.4.0
+  rev: v4.5.0
   hooks:
   - id: detect-private-key
   - id: check-ast
   - id: check-toml
   - id: end-of-file-fixer
   - id: mixed-line-ending
     args: [--fix=lf]
   - id: file-contents-sorter
     files: docs/spelling/.*\.txt
   - id: trailing-whitespace
   - id: check-case-conflict
 - repo: https://github.com/charliermarsh/ruff-pre-commit
-  # Ruff version.
-  rev: v0.0.285
+  rev: v0.2.1
   hooks:
   - id: ruff
     args: [--fix, --exit-non-zero-on-fix]
+- repo: https://github.com/pycqa/isort
+  rev: 5.13.2
+  hooks:
+  - id: isort
+    name: isort
+- repo: https://github.com/google/yapf
+  rev: v0.40.2
+  hooks:
+  - id: yapf
+    additional_dependencies: [toml]
+- repo: https://github.com/nbQA-dev/nbQA
+  rev: 1.7.1
+  hooks:
+  - id: nbqa-pyupgrade
+    args: [--py38-plus]
+  - id: nbqa-black
+  - id: nbqa-isort
+- repo: https://github.com/macisamuele/language-formatters-pre-commit-hooks
+  rev: v2.12.0
+  hooks:
+  - id: pretty-format-yaml
+    args: [--autofix, --indent, '2']
 - repo: https://github.com/rstcheck/rstcheck
-  rev: v6.1.2
+  rev: v6.2.0
   hooks:
   - id: rstcheck
     additional_dependencies: [tomli]
     args: [--config=pyproject.toml]
 - repo: https://github.com/PyCQA/doc8
   rev: v1.1.1
   hooks:
```

### Comparing `ott-jax-0.4.5/CODE_OF_CONDUCT.md` & `ott_jax-0.4.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.5/CONTRIBUTING.md` & `ott_jax-0.4.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.5/LICENSE` & `ott_jax-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.5/PKG-INFO` & `ott_jax-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ott-jax
-Version: 0.4.5
+Version: 0.4.6
 Summary: Optimal Transport Tools in JAX.
 Author-email: OTT team <optimal.transport.tools@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -232,14 +232,15 @@
 Requires-Dist: jax>=0.4.0
 Requires-Dist: jaxopt>=0.8
 Requires-Dist: lineax>=0.0.1; python_version >= "3.9"
 Requires-Dist: numpy>=1.20.0
 Provides-Extra: neural
 Requires-Dist: flax>=0.6.6; extra == "neural"
 Requires-Dist: optax>=0.1.1; extra == "neural"
+Requires-Dist: diffrax>=0.4.1; extra == "neural"
 Provides-Extra: dev
 Requires-Dist: pre-commit>=2.16.0; extra == "dev"
 Requires-Dist: tox>=4; extra == "dev"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-xdist; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
```

### Comparing `ott-jax-0.4.5/README.md` & `ott_jax-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.5/pyproject.toml` & `ott_jax-0.4.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 "Issue Tracker" = "https://github.com/ott-jax/ott/issues"
 Changelog = "https://github.com/ott-jax/ott/releases"
 
 [project.optional-dependencies]
 neural = [
     "flax>=0.6.6",
     "optax>=0.1.1",
+    "diffrax>=0.4.1",
 ]
 dev = [
     "pre-commit>=2.16.0",
     "tox>=4",
 ]
 test = [
     "pytest",
@@ -98,33 +99,39 @@
 [tool.black]
 line-length = 80
 target-version = ["py38"]
 include = '\.ipynb$'
 
 [tool.isort]
 profile = "black"
+line_length = 80
 include_trailing_comma = true
 multi_line_output = 3
-sections = ["FUTURE", "STDLIB", "THIRDPARTY", "NUMERIC", "PLOTTING", "FIRSTPARTY", "LOCALFOLDER"]
-# also contains what we import in notebooks
-known_numeric = ["numpy", "scipy", "jax", "flax", "optax", "jaxopt", "torch", "ot", "torchvision", "pandas", "sklearn"]
+sections = ["FUTURE", "STDLIB", "THIRDPARTY", "TEST", "NUMERIC", "NEURAL", "PLOTTING", "FIRSTPARTY", "LOCALFOLDER"]
+# also contains what we import in notebooks/tests
+known_neural = ["flax", "optax", "diffrax", "orbax"]
+known_numeric = ["numpy", "scipy", "jax", "flax", "optax", "jaxopt", "ot", "torch", "torchvision", "pandas", "sklearn", "tslearn"]
+known_test = ["_pytest", "pytest"]
 known_plotting = ["IPython", "matplotlib", "mpl_toolkits", "seaborn"]
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = '-m "not notebook"'
 testpaths = [
     "tests",
 ]
 markers = [
     "cpu: Mark tests as CPU only.",
     "fast: Mark tests as fast.",
 ]
 filterwarnings = [
+    "ignore:\\n*.*scipy.sparse array",
     "ignore:jax.random.KeyArray is deprecated:DeprecationWarning",
+    "ignore:.*jax.config:DeprecationWarning",
+    "ignore:jax.core.Shape is deprecated:DeprecationWarning:chex",
 ]
 
 [tool.coverage.run]
 branch = true
 source = ["src/"]
 omit = [
     "*/__init__.py",
@@ -175,121 +182,123 @@
 [tool.doc8]
 max_line_length = 80
 # Parser "myst_parser.sphinx_" not found. No module named 'myst_parser'.
 ignore_path = ["docs/**/_autosummary", "docs/contributing.rst"]
 
 [tool.tox]
 legacy_tox_ini = """
-    [tox]
-    min_version = 4.0
-    env_list = lint-code,py{3.8,3.9,3.10,3.11,3.12},py3.9-jax-default
-    skip_missing_interpreters = true
-
-    [testenv]
-    extras =
-        test
-        # https://github.com/google/flax/issues/3329
-        py{3.9,3.10,3.11,3.12},py3.9-jax-default: neural
-    pass_env = CUDA_*,PYTEST_*,CI
-    commands_pre =
-        gpu: python -I -m pip install "jax[cuda]" -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
-        jax-latest: python -I -m pip install 'git+https://github.com/google/jax@main'
-    commands =
-        python -m pytest {tty:--color=yes} {posargs: \
-            --cov={env_site_packages_dir}{/}ott --cov-config={tox_root}{/}pyproject.toml \
-            --no-cov-on-fail --cov-report=xml --cov-report=term-missing:skip-covered}
-
-    [testenv:lint-code]
-    description = Lint the code.
-    deps = pre-commit>=2.16.0
-    skip_install = true
-    commands =
-        pre-commit run --all-files --show-diff-on-failure
-
-    [testenv:lint-docs]
-    description = Lint the documentation.
-    deps =
-    extras = docs,neural
-    ignore_errors = true
-    allowlist_externals = make
-    pass_env = PYENCHANT_LIBRARY_PATH
-    set_env = SPHINXOPTS = -W -q --keep-going
-    changedir = {tox_root}{/}docs
-    commands =
-        make linkcheck {posargs}
-        make spelling {posargs}
-
-    [testenv:build-docs]
-    description = Build the documentation.
-    use_develop = true
-    deps =
-    extras = docs,neural
-    allowlist_externals = make
-    changedir = {tox_root}{/}docs
-    commands =
-        make html {posargs}
-    commands_post =
-        python -c 'import pathlib; print("Documentation is under:", pathlib.Path("{tox_root}") / "docs" / "_build" / "html" / "index.html")'
-
-    [testenv:clean-docs]
-    description = Remove the documentation.
-    deps =
-    skip_install = true
-    changedir = {tox_root}{/}docs
-    allowlist_externals = make
-    commands =
-        make clean
-
-    [testenv:build-package]
-    description = Build the package.
-    deps =
-        build
-        twine
-    commands =
-        python -m build --sdist --wheel --outdir {tox_root}{/}dist{/} {posargs:}
-        twine check {tox_root}{/}dist{/}*
-    commands_post =
-        python -c 'import pathlib; print(f"Package is under:", pathlib.Path("{tox_root}") / "dist")'
-
-    [testenv:format-references]
-    description = Format references.bib.
-    skip_install = true
-    allowlist_externals = biber
-    commands = biber --tool --output_file={tox_root}{/}docs{/}references.bib --nolog \
-        --output_align --output_indent=2 --output_fieldcase=lower \
-        --output_legacy_dates --output-field-replace=journaltitle:journal,thesis:phdthesis,institution:school \
-        {tox_root}{/}docs{/}references.bib
+[tox]
+min_version = 4.0
+env_list = lint-code,py{3.8,3.9,3.10,3.11,3.12},py3.9-jax-default
+skip_missing_interpreters = true
+
+[testenv]
+extras =
+    test
+    # https://github.com/google/flax/issues/3329
+    py{3.9,3.10,3.11,3.12},py3.9-jax-default: neural
+pass_env = CUDA_*,PYTEST_*,CI
+commands_pre =
+    gpu: python -I -m pip install "jax[cuda]" -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
+    jax-latest: python -I -m pip install 'git+https://github.com/google/jax@main'
+commands =
+    python -m pytest {tty:--color=yes} {posargs: \
+      --cov={env_site_packages_dir}{/}ott --cov-config={tox_root}{/}pyproject.toml \
+      --no-cov-on-fail --cov-report=xml --cov-report=term-missing:skip-covered}
+
+[testenv:lint-code]
+description = Lint the code.
+deps = pre-commit>=2.16.0
+skip_install = true
+commands =
+    pre-commit run --all-files --show-diff-on-failure
+
+[testenv:lint-docs]
+description = Lint the documentation.
+deps =
+extras = docs,neural
+ignore_errors = true
+allowlist_externals = make
+pass_env = PYENCHANT_LIBRARY_PATH
+set_env = SPHINXOPTS = -W -q --keep-going
+changedir = {tox_root}{/}docs
+commands =
+    make linkcheck {posargs}
+    make spelling {posargs}
+
+[testenv:build-docs]
+description = Build the documentation.
+use_develop = true
+deps =
+extras = docs,neural
+allowlist_externals = make
+changedir = {tox_root}{/}docs
+commands =
+    make html {posargs}
+commands_post =
+    python -c 'import pathlib; print("Documentation is under:", pathlib.Path("{tox_root}") / "docs" / "_build" / "html" / "index.html")'
+
+[testenv:clean-docs]
+description = Remove the documentation.
+deps =
+skip_install = true
+changedir = {tox_root}{/}docs
+allowlist_externals = make
+commands =
+    make clean
+
+[testenv:build-package]
+description = Build the package.
+deps =
+    build
+    twine
+commands =
+    python -m build --sdist --wheel --outdir {tox_root}{/}dist{/} {posargs:}
+    twine check {tox_root}{/}dist{/}*
+commands_post =
+    python -c 'import pathlib; print(f"Package is under:", pathlib.Path("{tox_root}") / "dist")'
+
+[testenv:format-references]
+description = Format references.bib.
+skip_install = true
+allowlist_externals = biber
+commands = biber --tool --output_file={tox_root}{/}docs{/}references.bib --nolog \
+    --output_align --output_indent=2 --output_fieldcase=lower \
+    --output_legacy_dates --output-field-replace=journaltitle:journal,thesis:phdthesis,institution:school \
+    {tox_root}{/}docs{/}references.bib
 """
 
 [tool.ruff]
 exclude = [
     ".git",
     "__pycache__",
     "build",
     "docs/_build",
     "dist"
 ]
+line-length = 80
+target-version = "py38"
+
+[tool.ruff.lint]
 ignore = [
     # Do not assign a lambda expression, use a def -> lambda expression assignments are convenient
     "E731",
     # allow I, O, l as variable names -> I is the identity matrix, i, j, k, l is reasonable indexing notation
     "E741",
     # Missing docstring in public package
     "D104",
     # Missing docstring in public module
     "D100",
     # Missing docstring in __init__
     "D107",
     # Missing docstring in magic method
     "D105",
 ]
-line-length = 80
 select = [
     "D", # flake8-docstrings
-    "I", # isort
     "E", # pycodestyle
     "F", # pyflakes
     "W", # pycodestyle
     "Q", # flake8-quotes
     "SIM", # flake8-simplify
     "TID",  # flake-8-tidy-imports
     "NPY",  # NumPy-specific rules
@@ -298,24 +307,24 @@
     "UP", # pyupgrade
     "C4", # flake8-comprehensions
     "BLE", # flake8-blind-except
     "T20",  # flake8-print
     "RET", # flake8-raise
 ]
 unfixable = ["B", "UP", "C4", "BLE", "T20", "RET"]
-target-version = "py38"
-[tool.ruff.per-file-ignores]
+
+[tool.ruff.lint.per-file-ignores]
 # TODO(michalk8): PO004 - remove `self.initialize`
 "tests/*" = ["D", "PT004", "E402"]
 "*/__init__.py" = ["F401"]
 "docs/*" = ["D"]
 "src/ott/types.py" = ["D102"]
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 convention = "google"
-[tool.ruff.pyupgrade]
+[tool.ruff.lint.pyupgrade]
 # Preserve types, even if a file imports `from __future__ import annotations`.
 keep-runtime-typing = true
-[tool.ruff.flake8-tidy-imports]
+[tool.ruff.lint.flake8-tidy-imports]
 # Disallow all relative imports.
 ban-relative-imports = "parents"
-[tool.ruff.flake8-quotes]
+[tool.ruff.lint.flake8-quotes]
 inline-quotes = "double"
```

### Comparing `ott-jax-0.4.5/setup.py` & `ott_jax-0.4.6/setup.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.5/src/ott/__init__.py` & `ott_jax-0.4.6/src/ott/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,13 +21,12 @@
     problems,
     solvers,
     tools,
     utils,
 )
 
 with contextlib.suppress(ImportError):
-  # TODO(michalk8): add warning that neural module is not imported
   from . import neural
 
 from ._version import __version__
 
 del contextlib
```

### Comparing `ott-jax-0.4.5/src/ott/_version.py` & `ott_jax-0.4.6/src/ott/_version.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.5/src/ott/datasets.py` & `ott_jax-0.4.6/src/ott/datasets.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,25 +47,25 @@
       - ``circle`` - two-dimensional Gaussians arranged on a circle,
       - ``square_five`` - two-dimensional Gaussians on a square with
         one Gaussian in the center, and
       - ``square_four`` - two-dimensional Gaussians in the corners of a
         rectangle
 
     batch_size: batch size of the samples
-    init_rng: initial PRNG key
+    rng: initial PRNG key
     scale: scale of the Gaussian means
     std: the standard deviation of the individual Gaussian samples
   """
   name: Name_t
   batch_size: int
-  init_rng: jax.Array
+  rng: jax.Array
   scale: float = 5.0
   std: float = 0.5
 
-  def __post_init__(self):
+  def __post_init__(self) -> None:
     gaussian_centers = {
         "simple":
             np.array([[0, 0]]),
         "circle":
             np.array([
                 (1, 0),
                 (-1, 0),
@@ -92,15 +92,15 @@
 
     Returns:
       A generator of samples from the Gaussian mixture.
     """
     return self._create_sample_generators()
 
   def _create_sample_generators(self) -> Iterator[jnp.array]:
-    rng = self.init_rng
+    rng = self.rng
     while True:
       rng1, rng2, rng = jax.random.split(rng, 3)
       means = jax.random.choice(rng1, self.centers, (self.batch_size,))
       normal_samples = jax.random.normal(rng2, (self.batch_size, 2))
       samples = self.scale * means + (self.std ** 2) * normal_samples
       yield samples
 
@@ -124,31 +124,23 @@
   Returns:
     The dataset and dimension of the data.
   """
   rng = utils.default_prng_key(rng)
   rng1, rng2, rng3, rng4 = jax.random.split(rng, 4)
   train_dataset = Dataset(
       source_iter=iter(
-          GaussianMixture(
-              name_source, batch_size=train_batch_size, init_rng=rng1
-          )
+          GaussianMixture(name_source, batch_size=train_batch_size, rng=rng1)
       ),
       target_iter=iter(
-          GaussianMixture(
-              name_target, batch_size=train_batch_size, init_rng=rng2
-          )
+          GaussianMixture(name_target, batch_size=train_batch_size, rng=rng2)
       )
   )
   valid_dataset = Dataset(
       source_iter=iter(
-          GaussianMixture(
-              name_source, batch_size=valid_batch_size, init_rng=rng3
-          )
+          GaussianMixture(name_source, batch_size=valid_batch_size, rng=rng3)
       ),
       target_iter=iter(
-          GaussianMixture(
-              name_target, batch_size=valid_batch_size, init_rng=rng4
-          )
+          GaussianMixture(name_target, batch_size=valid_batch_size, rng=rng4)
       )
   )
   dim_data = 2
   return train_dataset, valid_dataset, dim_data
```

### Comparing `ott-jax-0.4.5/src/ott/geometry/__init__.py` & `ott_jax-0.4.6/src/ott/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.5/src/ott/geometry/costs.py` & `ott_jax-0.4.6/src/ott/geometry/costs.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,14 +134,35 @@
       y: Array of shape ``[m, ...]``.
 
     Returns:
       Array of shape ``[n, m]`` of cost evaluations.
     """
     return jax.vmap(lambda x_: jax.vmap(lambda y_: self.pairwise(x_, y_))(y))(x)
 
+  def twist_operator(
+      self, vec: jnp.ndarray, dual_vec: jnp.ndarray, variable: bool
+  ) -> jnp.ndarray:
+    r"""Twist inverse operator of the cost function.
+
+    Given a cost function :math:`c`, the twist operator returns
+    :math:`\nabla_{1}c(x, \cdot)^{-1}(z)` if ``variable`` is ``0``,
+    and :math:`\nabla_{2}c(\cdot, y)^{-1}(z)` if ``variable`` is ``1``, for
+    :math:`x=y` equal to ``vec`` and :math:`z` equal to ``dual_vec``.
+
+    Args:
+      vec: ``[p,]`` point at which the twist inverse operator is evaluated.
+      dual_vec: ``[q,]`` point to invert by the operator.
+      variable: apply twist inverse operator on first (i.e. value set to ``0``
+        or equivalently ``False``) or second (``1`` or ``True``) variable.
+
+    Returns:
+      A vector.
+    """
+    raise NotImplementedError("Twist operator is not implemented.")
+
   def tree_flatten(self):  # noqa: D102
     return (), None
 
   @classmethod
   def tree_unflatten(cls, aux_data, children):  # noqa: D102
     del aux_data
     return cls(*children)
@@ -178,14 +199,22 @@
     """Legendre transform of :func:`h` when it is convex."""
     raise NotImplementedError("Legendre transform of `h` is not implemented.")
 
   def pairwise(self, x: jnp.ndarray, y: jnp.ndarray) -> float:
     """Compute cost as evaluation of :func:`h` on :math:`x-y`."""
     return self.h(x - y)
 
+  def twist_operator(
+      self, vec: jnp.ndarray, dual_vec: jnp.ndarray, variable: bool
+  ) -> jnp.ndarray:
+    # Note: when `h` is pair, i.e. h(z) = h(-z), the expressions below coincide
+    if variable:
+      return vec + jax.grad(self.h_legendre)(-dual_vec)
+    return vec - jax.grad(self.h_legendre)(dual_vec)
+
 
 @jax.tree_util.register_pytree_node_class
 class SqPNorm(TICost):
   r"""Squared p-norm of the difference of two vectors.
 
   Uses custom implementation of `norm` to avoid `NaN` values when
   differentiating the norm of `x-x`.
@@ -238,14 +267,19 @@
   def h(self, z: jnp.ndarray) -> float:  # noqa: D102
     return mu.norm(z, self.p) ** self.p / self.p
 
   def h_legendre(self, z: jnp.ndarray) -> float:  # noqa: D102
     # not defined for `p=1`
     return mu.norm(z, self.q) ** self.q / self.q
 
+  def barycenter(self, weights: jnp.ndarray,
+                 xs: jnp.ndarray) -> Tuple[jnp.ndarray, Any]:
+    """Output barycenter of vectors."""
+    return jnp.average(xs, weights=weights, axis=0), None
+
   def tree_flatten(self):  # noqa: D102
     return (), (self.p,)
 
   @classmethod
   def tree_unflatten(cls, aux_data, children):  # noqa: D102
     del children
     return cls(*aux_data)
@@ -280,15 +314,15 @@
 
   def norm(self, x: jnp.ndarray) -> Union[float, jnp.ndarray]:
     """Compute squared Euclidean norm for vector."""
     return jnp.sum(x ** 2, axis=-1)
 
   def pairwise(self, x: jnp.ndarray, y: jnp.ndarray) -> float:
     """Compute minus twice the dot-product between vectors."""
-    return -2. * jnp.vdot(x, y)
+    return -2.0 * jnp.vdot(x, y)
 
   def h(self, z: jnp.ndarray) -> float:  # noqa: D102
     return jnp.sum(z ** 2)
 
   def h_legendre(self, z: jnp.ndarray) -> float:  # noqa: D102
     return 0.25 * jnp.sum(z ** 2)
 
@@ -495,15 +529,15 @@
     return z - tau * self.prox_reg(z / tau, 1.0 / tau)
 
   def h(self, z: jnp.ndarray) -> float:  # noqa: D102
     out = 0.5 * jnp.sum(z ** 2)
     return out + self.scaling_reg * self.reg(z)
 
   def h_legendre(self, z: jnp.ndarray) -> float:  # noqa: D102
-    q = jax.lax.stop_gradient(self.prox_reg(z))
+    q = self.prox_reg(jax.lax.stop_gradient(z))
     return jnp.sum(q * z) - self.h(q)
 
   def h_transform(self, f: Callable[[jnp.ndarray], float],
                   **kwargs: Any) -> Callable[[jnp.ndarray], float]:
     r"""Compute the h-transform of a concave function.
 
     Return a callable :math:`f_h` defined as:
@@ -548,14 +582,19 @@
       pg = jaxopt.ProximalGradient(fun=minus_f, prox=prox, **kwargs)
       pg_run = pg.run(x, self.scaling_reg, x=x)
       pg_sol = jax.lax.stop_gradient(pg_run.params)
       return self.h(pg_sol) + minus_f(pg_sol, x)
 
     return f_h
 
+  def barycenter(self, weights: jnp.ndarray,
+                 xs: jnp.ndarray) -> Tuple[jnp.ndarray, Any]:
+    """Output barycenter of vectors."""
+    return jnp.average(xs, weights=weights, axis=0), None
+
   def tree_flatten(self):  # noqa: D102
     return (self.scaling_reg, self.matrix), {"orthogonal": self.orthogonal}
 
   @classmethod
   def tree_unflatten(cls, aux_data, children):  # noqa: D102
     return cls(*children, **aux_data)
 
@@ -802,15 +841,14 @@
       to monitor convergence.
     """
     sqrtm_kw = {} if sqrtm_kw is None else sqrtm_kw
     # Pop values or set defaults for fixed-point loop.
     min_iterations = kwargs.pop("min_iterations", 1)
     max_iterations = kwargs.pop("max_iterations", 100)
     inner_iterations = kwargs.pop("inner_iterations", 5)
-    dtype = covs.dtype
 
     @functools.partial(jax.vmap, in_axes=[None, 0, 0])
     def scale_covariances(
         cov_sqrt: jnp.ndarray, cov: jnp.ndarray, weight: jnp.ndarray
     ) -> jnp.ndarray:
       """Rescale covariance in barycenter step."""
       return weight * matrix_square_root.sqrtm_only((cov_sqrt @ cov) @ cov_sqrt,
@@ -834,18 +872,15 @@
       next_cov = (cov_inv_sqrt @ scaled_cov) @ cov_inv_sqrt
       diff = jnp.sum((next_cov - cov) ** 2) / jnp.prod(jnp.array(cov.shape))
       diffs = diffs.at[iteration // inner_iterations].set(diff)
       return next_cov, diffs
 
     def init_state() -> Tuple[jnp.ndarray, float]:
       cov_init = jnp.eye(self._dimension)
-      diffs = -jnp.ones(
-          (np.ceil(max_iterations / inner_iterations).astype(int),),
-          dtype=dtype
-      )
+      diffs = -jnp.ones(math.ceil(max_iterations / inner_iterations))
       return cov_init, diffs
 
     cov, diffs = fixed_point_loop.fixpoint_iter(
         cond_fn=cond_fn,
         body_fn=body_fn,
         min_iterations=min_iterations,
         max_iterations=max_iterations,
@@ -986,15 +1021,15 @@
     mass_x, mass_y = x[0], y[0]
     mean_x, cov_x = x_to_means_and_covs(x[1:], self._dimension)
     mean_y, cov_y = x_to_means_and_covs(y[1:], self._dimension)
 
     diff_means = mean_x - mean_y
 
     # Identity matrix of suitable size
-    iden = jnp.eye(self._dimension, dtype=x.dtype)
+    iden = jnp.eye(self._dimension)
 
     # Creates matrices needed in the computation
     tilde_a = 0.5 * gam * (iden - lam * jnp.linalg.inv(cov_x + lam * iden))
     tilde_b = 0.5 * gam * (iden - lam * jnp.linalg.inv(cov_y + lam * iden))
 
     tilde_a_b = jnp.matmul(tilde_a, tilde_b)
     c_mat = matrix_square_root.sqrtm(
```

### Comparing `ott-jax-0.4.5/src/ott/geometry/distrib_costs.py` & `ott_jax-0.4.6/src/ott/geometry/distrib_costs.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.5/src/ott/geometry/epsilon_scheduler.py` & `ott_jax-0.4.6/src/ott/geometry/epsilon_scheduler.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.5/src/ott/geometry/geodesic.py` & `ott_jax-0.4.6/src/ott/geometry/geodesic.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,29 +7,30 @@
 #   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from typing import Any, Dict, Optional, Sequence, Tuple
+from typing import Any, Dict, Optional, Sequence, Tuple, Union
 
 import jax
 import jax.experimental.sparse as jesp
 import jax.numpy as jnp
 import numpy as np
 from scipy.special import ive
 
 from ott import utils
 from ott.geometry import geometry
 from ott.math import utils as mu
-from ott.types import Array_g
 
 __all__ = ["Geodesic"]
 
+Array_g = Union[jnp.ndarray, jesp.BCOO]
+
 
 @jax.tree_util.register_pytree_node_class
 class Geodesic(geometry.Geometry):
   r"""Graph distance approximation using heat kernel :cite:`huguet:2023`.
 
   .. note::
     This constructor is not meant to be called by the user,
@@ -52,15 +53,15 @@
       self,
       scaled_laplacian: Array_g,
       eigval: jnp.ndarray,
       chebyshev_coeffs: jnp.ndarray,
       t: float = 1e-3,
       **kwargs: Any
   ):
-    super().__init__(epsilon=1., **kwargs)
+    super().__init__(epsilon=1.0, **kwargs)
     self.scaled_laplacian = scaled_laplacian
     self.eigval = eigval
     self.chebyshev_coeffs = chebyshev_coeffs
     self.t = t
 
   @classmethod
   def from_graph(
@@ -100,23 +101,20 @@
     """
     assert G.shape[0] == G.shape[1], G.shape
     rng = utils.default_prng_key(rng)
 
     if directed:
       G = G + G.T
     if t is None:
-      t = (jnp.sum(G) / jnp.sum(G > 0.0)) ** 2.0
+      t = (jnp.sum(G) / jnp.sum(G > 0.0)) ** 2
 
-    degree = jnp.sum(G, axis=1)
-    laplacian = jnp.diag(degree) - G
-    if normalize:
-      inv_sqrt_deg = jnp.diag(
-          jnp.where(degree > 0.0, 1.0 / jnp.sqrt(degree), 0.0)
-      )
-      laplacian = inv_sqrt_deg @ laplacian @ inv_sqrt_deg
+    if isinstance(G, jesp.BCOO):
+      laplacian = compute_sparse_laplacian(G, normalize)
+    else:
+      laplacian = compute_dense_laplacian(G, normalize)
 
     if eigval is None:
       eigval = compute_largest_eigenvalue(laplacian, rng)
 
     scaled_laplacian, eigval = jax.lax.cond((eigval > 2.0), lambda l:
                                             (2.0 * l / eigval, 2.0), lambda l:
                                             (l, eigval), laplacian)
@@ -216,14 +214,47 @@
   @classmethod
   def tree_unflatten(  # noqa: D102
       cls, aux_data: Dict[str, Any], children: Sequence[Any]
   ) -> "Geodesic":
     return cls(*children, **aux_data)
 
 
+def normalize_laplacian(laplacian: Array_g, degree: jnp.ndarray) -> Array_g:
+  inv_sqrt_deg = jnp.where(degree > 0.0, 1.0 / jnp.sqrt(degree), 0.0)
+  return inv_sqrt_deg[:, None] * laplacian * inv_sqrt_deg[None, :]
+
+
+def compute_dense_laplacian(
+    G: jnp.ndarray, normalize: bool = False
+) -> jnp.ndarray:
+  degree = jnp.sum(G, axis=1)
+  laplacian = jnp.diag(degree) - G
+  if normalize:
+    laplacian = normalize_laplacian(laplacian, degree)
+  return laplacian
+
+
+def compute_sparse_laplacian(
+    G: jesp.BCOO, normalize: bool = False
+) -> jesp.BCOO:
+  n, _ = G.shape
+  # making sure allocated indices has same dtype
+  # on different devices int32 vs int64 can cause issues
+  indices_dtype = G.indices.dtype
+  data_degree, ixs = G.sum(1).todense(), jnp.arange(n, dtype=indices_dtype)
+  degree = jesp.BCOO(
+      (data_degree, jnp.c_[ixs, ixs]),
+      shape=(n, n),
+  )
+  laplacian = degree - G
+  if normalize:
+    laplacian = normalize_laplacian(laplacian, data_degree)
+  return laplacian
+
+
 def compute_largest_eigenvalue(
     laplacian_matrix: jnp.ndarray,
     rng: jax.Array,
 ) -> float:
   # Compute the largest eigenvalue of the Laplacian matrix.
   n = laplacian_matrix.shape[0]
   # Generate random initial directions for eigenvalue computation
@@ -238,15 +269,15 @@
       lapl_vector_product,
       initial_dirs,
   )
   return eigvals[0]
 
 
 def expm_multiply(
-    L: jnp.ndarray, X: jnp.ndarray, coeff: jnp.ndarray, eigval: float
+    L: Array_g, X: jnp.ndarray, coeff: jnp.ndarray, eigval: float
 ) -> jnp.ndarray:
 
   def body(carry, c):
     T0, T1, Y = carry
     T2 = (2.0 / eigval) * L @ T1 - 2.0 * T1 - T0
     Y = Y + c * T2
     return (T1, T2, Y), None
```

### Comparing `ott-jax-0.4.5/src/ott/geometry/geometry.py` & `ott_jax-0.4.6/src/ott/geometry/geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,14 @@
     relative_epsilon: when `False`, the parameter ``epsilon`` specifies the
       value of the entropic regularization parameter. When `True`, ``epsilon``
       refers to a fraction of the :attr:`mean_cost_matrix`, which is computed
       adaptively from data.
     scale_cost: option to rescale the cost matrix. Implemented scalings are
       'median', 'mean' and 'max_cost'. Alternatively, a float factor can be
       given to rescale the cost such that ``cost_matrix /= scale_cost``.
-      If `True`, use 'mean'.
     src_mask: Mask specifying valid rows when computing some statistics of
       :attr:`cost_matrix`, see :attr:`src_mask`.
     tgt_mask: Mask specifying valid columns when computing some statistics of
       :attr:`cost_matrix`, see :attr:`tgt_mask`.
 
   Note:
     When defining a :class:`~ott.geometry.geometry.Geometry` through a
@@ -79,29 +78,29 @@
 
   def __init__(
       self,
       cost_matrix: Optional[jnp.ndarray] = None,
       kernel_matrix: Optional[jnp.ndarray] = None,
       epsilon: Optional[Union[float, epsilon_scheduler.Epsilon]] = None,
       relative_epsilon: Optional[bool] = None,
-      scale_cost: Union[bool, int, float, Literal["mean", "max_cost",
-                                                  "median"]] = 1.0,
+      scale_cost: Union[int, float, Literal["mean", "max_cost",
+                                            "median"]] = 1.0,
       src_mask: Optional[jnp.ndarray] = None,
       tgt_mask: Optional[jnp.ndarray] = None,
   ):
     self._cost_matrix = cost_matrix
     self._kernel_matrix = kernel_matrix
 
     # needed for `copy_epsilon`, because of the `isinstance` check
     self._epsilon_init = epsilon if isinstance(
         epsilon, epsilon_scheduler.Epsilon
     ) else epsilon_scheduler.Epsilon(epsilon)
     self._relative_epsilon = relative_epsilon
 
-    self._scale_cost = "mean" if scale_cost is True else scale_cost
+    self._scale_cost = scale_cost
 
     self._src_mask = src_mask
     self._tgt_mask = tgt_mask
 
   @property
   def cost_rank(self) -> Optional[int]:
     """Output rank of cost matrix, if any was provided."""
@@ -208,19 +207,19 @@
       return 1.0 / jnp.nanmax(self._cost_matrix)
     if self._scale_cost == "mean":
       return 1.0 / jnp.nanmean(self._cost_matrix)
     if self._scale_cost == "median":
       return 1.0 / jnp.nanmedian(self._cost_matrix)
     raise ValueError(f"Scaling {self._scale_cost} not implemented.")
 
-  def set_scale_cost(self, scale_cost: Union[bool, float, str]) -> "Geometry":
+  def set_scale_cost(self, scale_cost: Union[float, str]) -> "Geometry":
     """Modify how to rescale of the :attr:`cost_matrix`."""
     # case when `geom` doesn't have `scale_cost` or doesn't need to be modified
     # `False` retains the original scale
-    if scale_cost is False or scale_cost == self._scale_cost:
+    if scale_cost == self._scale_cost:
       return self
     children, aux_data = self.tree_flatten()
     aux_data["scale_cost"] = scale_cost
     return type(self).tree_unflatten(aux_data, children)
 
   def copy_epsilon(self, other: "Geometry") -> "Geometry":
     """Copy the epsilon parameters from another geometry."""
@@ -622,15 +621,15 @@
     )
 
   def to_LRCGeometry(
       self,
       rank: int = 0,
       tol: float = 1e-2,
       rng: Optional[jax.Array] = None,
-      scale: float = 1.
+      scale: float = 1.0
   ) -> "low_rank.LRCGeometry":
     r"""Factorize the cost matrix using either SVD (full) or :cite:`indyk:19`.
 
     When `rank=min(n,m)` or `0` (by default), use :func:`jax.numpy.linalg.svd`.
 
     For other values, use the routine in sublinear time :cite:`indyk:19`.
     Uses the implementation of :cite:`scetbon:21`, algorithm 4.
@@ -669,16 +668,16 @@
       rng = utils.default_prng_key(rng)
       rng1, rng2, rng3, rng4, rng5 = jax.random.split(rng, 5)
       n_subset = min(int(rank / tol), n, m)
 
       i_star = jax.random.randint(rng1, shape=(), minval=0, maxval=n)
       j_star = jax.random.randint(rng2, shape=(), minval=0, maxval=m)
 
-      ci_star = self.subset(i_star, None).cost_matrix.ravel() ** 2  # (m,)
-      cj_star = self.subset(None, j_star).cost_matrix.ravel() ** 2  # (n,)
+      ci_star = self.subset([i_star], None).cost_matrix.ravel() ** 2  # (m,)
+      cj_star = self.subset(None, [j_star]).cost_matrix.ravel() ** 2  # (n,)
 
       p_row = cj_star + ci_star[j_star] + jnp.mean(ci_star)  # (n,)
       p_row /= jnp.sum(p_row)
       row_ixs = jax.random.choice(rng3, n, shape=(n_subset,), p=p_row)
       # (n_subset, m)
       s = self.subset(row_ixs, None).cost_matrix
       s /= jnp.sqrt(n_subset * p_row[row_ixs][:, None])
@@ -693,15 +692,15 @@
       U, _, V = jsp.linalg.svd(w)
       U = U[:, :rank]  # (n_subset, rank)
       U = (s.T @ U) / jnp.linalg.norm(w.T @ U, axis=0)  # (m, rank)
 
       _, d, v = jnp.linalg.svd(U.T @ U)  # (k,), (k, k)
       v = v.T / jnp.sqrt(d)[None, :]
 
-      inv_scale = (1. / jnp.sqrt(n_subset))
+      inv_scale = (1.0 / jnp.sqrt(n_subset))
       col_ixs = jax.random.choice(rng5, m, shape=(n_subset,))  # (n_subset,)
 
       # (n, n_subset)
       A_trans = self.subset(None, col_ixs).cost_matrix * inv_scale
       B = (U[col_ixs, :] @ v * inv_scale)  # (n_subset, k)
       M = jnp.linalg.inv(B.T @ B)  # (k, k)
       V = jnp.linalg.multi_dot([A_trans, B, M.T, v.T])  # (n, k)
@@ -736,32 +735,32 @@
         arr: Optional[jnp.ndarray],
         src_ixs: Optional[jnp.ndarray],
         tgt_ixs: Optional[jnp.ndarray],
     ) -> Optional[jnp.ndarray]:
       if arr is None:
         return None
       if src_ixs is not None:
-        arr = arr[jnp.atleast_1d(src_ixs)]
+        arr = arr[src_ixs, ...]
       if tgt_ixs is not None:
-        arr = arr[:, jnp.atleast_1d(tgt_ixs)]
+        arr = arr[:, tgt_ixs]
       return arr  # noqa: RET504
 
     return self._mask_subset_helper(
         src_ixs,
         tgt_ixs,
         fn=subset_fn,
         propagate_mask=True,
         **kwargs,
     )
 
   def mask(
       self,
       src_mask: Optional[jnp.ndarray],
       tgt_mask: Optional[jnp.ndarray],
-      mask_value: float = 0.,
+      mask_value: float = 0.0,
   ) -> "Geometry":
     """Mask rows or columns of a geometry.
 
     The mask is used only when computing some statistics of the
     :attr:`cost_matrix`.
 
         - :attr:`mean_cost_matrix`
@@ -851,15 +850,15 @@
   @property
   def dtype(self) -> jnp.dtype:
     """The data type."""
     return (
         self._kernel_matrix if self._cost_matrix is None else self._cost_matrix
     ).dtype
 
-  def _masked_geom(self, mask_value: float = 0.) -> "Geometry":
+  def _masked_geom(self, mask_value: float = 0.0) -> "Geometry":
     """Mask geometry based on :attr:`src_mask` and :attr:`tgt_mask`."""
     src_mask, tgt_mask = self.src_mask, self.tgt_mask
     if src_mask is None and tgt_mask is None:
       return self
     return self.mask(src_mask, tgt_mask, mask_value=mask_value)
 
   @property
@@ -873,20 +872,19 @@
   def _m_normed_ones(self) -> jnp.ndarray:
     """Normalized array of shape ``[num_b,]``."""
     mask = self.tgt_mask
     arr = jnp.ones(self.shape[1]) if mask is None else mask
     return arr / jnp.sum(arr)
 
   @staticmethod
-  def _normalize_mask(mask: Optional[Union[int, jnp.ndarray]],
+  def _normalize_mask(mask: Optional[jnp.ndarray],
                       size: int) -> Optional[jnp.ndarray]:
     """Convert array of indices to a boolean mask."""
     if mask is None:
       return None
-    mask = jnp.atleast_1d(mask)
     if not jnp.issubdtype(mask, (bool, jnp.bool_)):
       mask = jnp.isin(jnp.arange(size), mask)
     assert mask.shape == (size,)
     return mask
 
   def tree_flatten(self):  # noqa: D102
     return (
```

### Comparing `ott-jax-0.4.5/src/ott/geometry/graph.py` & `ott_jax-0.4.6/src/ott/geometry/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
       t: float = 1e-3,
       n_steps: int = 100,
       numerical_scheme: Literal["backward_euler",
                                 "crank_nicolson"] = "backward_euler",
       tol: float = -1.0,
       **kwargs: Any
   ):
-    super().__init__(epsilon=1., **kwargs)
+    super().__init__(epsilon=1.0, **kwargs)
     self.laplacian = laplacian
     self.t = t
     self.n_steps = n_steps
     self.numerical_scheme = numerical_scheme
     self.tol = tol
 
   @classmethod
@@ -103,15 +103,15 @@
     if normalize:
       inv_sqrt_deg = jnp.diag(
           jnp.where(degree > 0.0, 1.0 / jnp.sqrt(degree), 0.0)
       )
       laplacian = inv_sqrt_deg @ laplacian @ inv_sqrt_deg
 
     if t is None:
-      t = (jnp.sum(G) / jnp.sum(G > 0.)) ** 2
+      t = (jnp.sum(G) / jnp.sum(G > 0.0)) ** 2
 
     return cls(laplacian, t=t, **kwargs)
 
   def apply_kernel(
       self,
       scaling: jnp.ndarray,
       eps: Optional[float] = None,
@@ -158,15 +158,15 @@
         b = b - scaled_lap @ b
       return b, jsp.linalg.solve_triangular(L, b, lower=True)
 
     # eps we cannot use since it would require a re-solve
     # axis we can ignore since the matrix is symmetric
     del eps, axis
 
-    force_scan = self.tol < 0.
+    force_scan = self.tol < 0.0
     fixpoint_fn = (
         fixed_point_loop.fixpoint_iter
         if force_scan else fixed_point_loop.fixpoint_iter_backprop
     )
 
     state = (jnp.full_like(scaling, jnp.nan), scaling)
     L = jsp.linalg.cholesky(self._M, lower=True)
@@ -200,17 +200,17 @@
   def cost_matrix(self) -> jnp.ndarray:  # noqa: D102
     return -self.t * mu.safe_log(self.kernel_matrix)
 
   @property
   def _scale(self) -> float:
     """Constant used to scale the Laplacian."""
     if self.numerical_scheme == "backward_euler":
-      return self.t / (4. * self.n_steps)
+      return self.t / (4.0 * self.n_steps)
     if self.numerical_scheme == "crank_nicolson":
-      return self.t / (2. * self.n_steps)
+      return self.t / (2.0 * self.n_steps)
     raise NotImplementedError(
         f"Numerical scheme `{self.numerical_scheme}` is not implemented."
     )
 
   @property
   def _scaled_laplacian(self) -> jnp.ndarray:
     """Laplacian scaled by a constant, depending on the numerical scheme."""
```

### Comparing `ott-jax-0.4.5/src/ott/geometry/grid.py` & `ott_jax-0.4.6/src/ott/geometry/grid.py`

 * *Files 0% similar despite different names*

```diff
@@ -316,15 +316,15 @@
     """Not implemented."""
     raise NotImplementedError("Subsetting is not implemented for grids.")
 
   def mask(
       self,
       src_mask: Optional[jnp.ndarray],
       tgt_mask: Optional[jnp.ndarray],
-      mask_value: float = 0.,
+      mask_value: float = 0.0,
   ) -> NoReturn:
     """Not implemented."""
     raise NotImplementedError("Masking is not implemented for grids.")
 
   @classmethod
   def prepare_divergences(
       cls,
```

### Comparing `ott-jax-0.4.5/src/ott/geometry/low_rank.py` & `ott_jax-0.4.6/src/ott/geometry/low_rank.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,40 +38,40 @@
     cost_1: Array of shape ``[num_a, r]``.
     cost_2: Array of shape ``[num_b, r]``.
     bias: constant added to entire cost matrix.
     scale: Value used to rescale the factors of the low-rank geometry.
     scale_cost: option to rescale the cost matrix. Implemented scalings are
       'max_bound', 'mean' and 'max_cost'. Alternatively, a float
       factor can be given to rescale the cost such that
-      ``cost_matrix /= scale_cost``. If `True`, use 'mean'.
+      ``cost_matrix /= scale_cost``.
     batch_size: optional size of the batch to compute online (without
       instantiating the matrix) the scale factor ``scale_cost`` of the
       :attr:`cost_matrix` when ``scale_cost = 'max_cost'``. If `None`, the batch
       size is set to `1024` or to the largest number of samples between
       :attr:`cost_1` and :attr:`cost_2` if smaller than `1024`.
     kwargs: keyword arguments for :class:`~ott.geometry.geometry.Geometry`.
   """
 
   def __init__(
       self,
       cost_1: jnp.ndarray,
       cost_2: jnp.ndarray,
       bias: float = 0.0,
       scale_factor: float = 1.0,
-      scale_cost: Union[bool, int, float, Literal["mean", "max_bound",
-                                                  "max_cost"]] = 1.0,
+      scale_cost: Union[int, float, Literal["mean", "max_bound",
+                                            "max_cost"]] = 1.0,
       batch_size: Optional[int] = None,
       **kwargs: Any,
   ):
     super().__init__(**kwargs)
     self._cost_1 = cost_1
     self._cost_2 = cost_2
     self._bias = bias
     self._scale_factor = scale_factor
-    self._scale_cost = "mean" if scale_cost is True else scale_cost
+    self._scale_cost = scale_cost
     self.batch_size = batch_size
 
   @property
   def cost_1(self) -> jnp.ndarray:
     """First factor of the :attr:`cost_matrix`."""
     scale_factor = jnp.sqrt(self._scale_factor * self.inv_scale_cost)
     return scale_factor * self._cost_1
@@ -247,25 +247,25 @@
       **kwargs: Any
   ) -> "LRCGeometry":
 
     def subset_fn(
         arr: Optional[jnp.ndarray],
         ixs: Optional[jnp.ndarray],
     ) -> jnp.ndarray:
-      return arr if arr is None or ixs is None else arr[jnp.atleast_1d(ixs)]
+      return arr if arr is None or ixs is None else arr[ixs, ...]
 
     return self._mask_subset_helper(
         src_ixs, tgt_ixs, fn=subset_fn, propagate_mask=True, **kwargs
     )
 
   def mask(  # noqa: D102
       self,
       src_mask: Optional[jnp.ndarray],
       tgt_mask: Optional[jnp.ndarray],
-      mask_value: float = 0.,
+      mask_value: float = 0.0,
   ) -> "LRCGeometry":
 
     def mask_fn(
         arr: Optional[jnp.ndarray],
         mask: Optional[jnp.ndarray],
     ) -> Optional[jnp.ndarray]:
       if arr is None or mask is None:
```

### Comparing `ott-jax-0.4.5/src/ott/geometry/pointcloud.py` & `ott_jax-0.4.6/src/ott/geometry/pointcloud.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,51 +46,50 @@
      recomputed at each call of the :meth:`apply_lse_kernel` step,
      ``batch_size`` lines at a time, used on a vector and discarded.
      The online computation is particularly useful for big point clouds
      whose cost matrix does not fit in memory.
     scale_cost: option to rescale the cost matrix. Implemented scalings are
       'median', 'mean', 'max_cost', 'max_norm' and 'max_bound'.
       Alternatively, a float factor can be given to rescale the cost such
-      that ``cost_matrix /= scale_cost``. If `True`, use 'mean'.
+      that ``cost_matrix /= scale_cost``.
     kwargs: keyword arguments for :class:`~ott.geometry.geometry.Geometry`.
   """
 
   def __init__(
       self,
       x: jnp.ndarray,
       y: Optional[jnp.ndarray] = None,
       cost_fn: Optional[costs.CostFn] = None,
       batch_size: Optional[int] = None,
-      scale_cost: Union[bool, int, float,
-                        Literal["mean", "max_norm", "max_bound", "max_cost",
-                                "median"]] = 1.0,
+      scale_cost: Union[int, float, Literal["mean", "max_norm", "max_bound",
+                                            "max_cost", "median"]] = 1.0,
       **kwargs: Any
   ):
     super().__init__(**kwargs)
     self.x = x
     self.y = self.x if y is None else y
 
     self.cost_fn = costs.SqEuclidean() if cost_fn is None else cost_fn
     self._axis_norm = 0 if callable(self.cost_fn.norm) else None
     if batch_size is not None:
       assert batch_size > 0, f"`batch_size={batch_size}` must be positive."
     self._batch_size = batch_size
-    self._scale_cost = "mean" if scale_cost is True else scale_cost
+    self._scale_cost = scale_cost
 
   @property
   def _norm_x(self) -> Union[float, jnp.ndarray]:
     if self._axis_norm == 0:
       return self.cost_fn.norm(self.x)
-    return 0.
+    return 0.0
 
   @property
   def _norm_y(self) -> Union[float, jnp.ndarray]:
     if self._axis_norm == 0:
       return self.cost_fn.norm(self.y)
-    return 0.
+    return 0.0
 
   @property
   def can_LRC(self):  # noqa: D102
     return self.is_squared_euclidean and self._check_LRC_dim
 
   @property
   def _check_LRC_dim(self):
@@ -130,15 +129,14 @@
     return isinstance(self.cost_fn, costs.SqEuclidean)
 
   @property
   def is_online(self) -> bool:
     """Whether the cost/kernel is computed on-the-fly."""
     return self.batch_size is not None
 
-  # TODO(michalk8): when refactoring, consider PC as a subclass of LR?
   @property
   def cost_rank(self) -> int:  # noqa: D102
     return self.x.shape[1]
 
   @property
   def inv_scale_cost(self) -> float:  # noqa: D102
     if isinstance(self._scale_cost, (int, float, jax.Array)):
@@ -196,85 +194,73 @@
       eps: float,
       vec: Optional[jnp.ndarray] = None,
       axis: int = 0
   ) -> jnp.ndarray:
 
     def body0(carry, i: int):
       f, g, eps, vec = carry
-      y = jax.lax.dynamic_slice(
-          self.y, (i * self.batch_size, 0), (self.batch_size, self.y.shape[1])
+      y, g_ = self._leading_slice(self.y, i), self._leading_slice(g, i)
+      norm_y = self._norm_y if self._axis_norm is None else self._leading_slice(
+          self._norm_y, i
       )
-      g_ = jax.lax.dynamic_slice(g, (i * self.batch_size,), (self.batch_size,))
-      if self._axis_norm is None:
-        norm_y = self._norm_y
-      else:
-        norm_y = jax.lax.dynamic_slice(
-            self._norm_y, (i * self.batch_size,), (self.batch_size,)
-        )
       h_res, h_sgn = app(
-          self.x, y, self._norm_x, norm_y, f, g_, eps, vec, self.cost_fn,
+          self.x, y, self._norm_x, norm_y, f, g_, eps, vec, cost_fn,
           self.inv_scale_cost
       )
       return carry, (h_res, h_sgn)
 
     def body1(carry, i: int):
       f, g, eps, vec = carry
-      x = jax.lax.dynamic_slice(
-          self.x, (i * self.batch_size, 0), (self.batch_size, self.x.shape[1])
+      x, f_ = self._leading_slice(self.x, i), self._leading_slice(f, i)
+      norm_x = self._norm_x if self._axis_norm is None else self._leading_slice(
+          self._norm_x, i
       )
-      f_ = jax.lax.dynamic_slice(f, (i * self.batch_size,), (self.batch_size,))
-      if self._axis_norm is None:
-        norm_x = self._norm_x
-      else:
-        norm_x = jax.lax.dynamic_slice(
-            self._norm_x, (i * self.batch_size,), (self.batch_size,)
-        )
       h_res, h_sgn = app(
-          self.y, x, self._norm_y, norm_x, g, f_, eps, vec, self.cost_fn,
+          self.y, x, self._norm_y, norm_x, g, f_, eps, vec, cost_fn,
           self.inv_scale_cost
       )
       return carry, (h_res, h_sgn)
 
-    def finalize(i: int):
+    def rest(i: int):
       if axis == 0:
         norm_y = self._norm_y if self._axis_norm is None else self._norm_y[i:]
         return app(
             self.x, self.y[i:], self._norm_x, norm_y, f, g[i:], eps, vec,
-            self.cost_fn, self.inv_scale_cost
+            cost_fn, self.inv_scale_cost
         )
       norm_x = self._norm_x if self._axis_norm is None else self._norm_x[i:]
       return app(
-          self.y, self.x[i:], self._norm_y, norm_x, g, f[i:], eps, vec,
-          self.cost_fn, self.inv_scale_cost
+          self.y, self.x[i:], self._norm_y, norm_x, g, f[i:], eps, vec, cost_fn,
+          self.inv_scale_cost
       )
 
     if not self.is_online:
       return super().apply_lse_kernel(f, g, eps, vec, axis)
 
     app = jax.vmap(
         _apply_lse_kernel_xy,
         in_axes=[
             None, 0, None, self._axis_norm, None, 0, None, None, None, None
         ]
     )
 
     if axis == 0:
-      fun = body0
+      fun, cost_fn = body0, self.cost_fn.pairwise
       v, n = g, self._y_nsplit
     elif axis == 1:
-      fun = body1
+      fun, cost_fn = body1, lambda y, x: self.cost_fn.pairwise(x, y)
       v, n = f, self._x_nsplit
     else:
       raise ValueError(axis)
 
     _, (h_res, h_sign) = jax.lax.scan(
         fun, init=(f, g, eps, vec), xs=jnp.arange(n)
     )
     h_res, h_sign = jnp.concatenate(h_res), jnp.concatenate(h_sign)
-    h_res_rest, h_sign_rest = finalize(n * self.batch_size)
+    h_res_rest, h_sign_rest = rest(n * self.batch_size)
     h_res = jnp.concatenate([h_res, h_res_rest])
     h_sign = jnp.concatenate([h_sign, h_sign_rest])
 
     return eps * h_res - jnp.where(jnp.isfinite(v), v, 0), h_sign
 
   def apply_kernel(  # noqa: D102
       self,
@@ -284,64 +270,55 @@
   ) -> jnp.ndarray:
     if eps is None:
       eps = self.epsilon
 
     if not self.is_online:
       return super().apply_kernel(scaling, eps, axis)
 
+    # TODO(michalk8): batch this properly
     app = jax.vmap(
         _apply_kernel_xy,
         in_axes=[None, 0, None, self._axis_norm, None, None, None, None]
     )
     if axis == 0:
       return app(
           self.x, self.y, self._norm_x, self._norm_y, scaling, eps,
-          self.cost_fn, self.inv_scale_cost
+          self.cost_fn.pairwise, self.inv_scale_cost
       )
+    # for non-symmetric costs
+    cost_fn = lambda y, x: self.cost_fn.pairwise(x, y)
     return app(
-        self.y, self.x, self._norm_y, self._norm_x, scaling, eps, self.cost_fn,
+        self.y, self.x, self._norm_y, self._norm_x, scaling, eps, cost_fn,
         self.inv_scale_cost
     )
 
   def transport_from_potentials(  # noqa: D102
       self, f: jnp.ndarray, g: jnp.ndarray
   ) -> jnp.ndarray:
     if not self.is_online:
       return super().transport_from_potentials(f, g)
-    transport = jax.vmap(
-        _transport_from_potentials_xy,
-        in_axes=[None, 0, None, self._axis_norm, None, 0, None, None, None]
-    )
+    in_axes = [None, 0, None, self._axis_norm, None, 0, None, None, None]
+    transport = jax.vmap(_transport_from_potentials_xy, in_axes=in_axes)
+    cost_fn = lambda y, x: self.cost_fn.pairwise(x, y)
     return transport(
-        self.y, self.x, self._norm_y, self._norm_x, g, f, self.epsilon,
-        self.cost_fn, self.inv_scale_cost
+        self.y, self.x, self._norm_y, self._norm_x, g, f, self.epsilon, cost_fn,
+        self.inv_scale_cost
     )
 
   def transport_from_scalings(  # noqa: D102
       self, u: jnp.ndarray, v: jnp.ndarray
   ) -> jnp.ndarray:
     if not self.is_online:
       return super().transport_from_scalings(u, v)
-    transport = jax.vmap(
-        _transport_from_scalings_xy,
-        in_axes=[
-            None,
-            0,
-            None,
-            self._axis_norm,
-            None,
-            0,
-            None,
-            None,
-            None,
-        ]
-    )
+    in_axes = [None, 0, None, self._axis_norm, None, 0, None, None, None]
+    transport = jax.vmap(_transport_from_scalings_xy, in_axes=in_axes)
+    cost_fn = lambda y, x: self.cost_fn.pairwise(x, y)
     return transport(
-        self.y, self.x, self._norm_y, self._norm_x, v, u, self.epsilon,
-        self.cost_fn, self.inv_scale_cost
+        self.y, self.x, self._norm_y, self._norm_x, v, u, self.epsilon, cost_fn,
+        self.inv_scale_cost
     )
 
   def apply_cost(
       self,
       arr: jnp.ndarray,
       axis: int = 0,
       fn: Optional[Callable[[jnp.ndarray], jnp.ndarray]] = None,
@@ -378,28 +355,30 @@
   def _apply_cost(
       self, arr: jnp.ndarray, axis: int = 0, fn=None
   ) -> jnp.ndarray:
     """See :meth:`apply_cost`."""
     if not self.is_online:
       return super().apply_cost(arr, axis, fn)
 
+    # TODO(michalk8): batch this properly
     app = jax.vmap(
         _apply_cost_xy,
         in_axes=[None, 0, None, self._axis_norm, None, None, None, None]
     )
     if arr.ndim == 1:
       arr = arr.reshape(-1, 1)
 
     if axis == 0:
       return app(
-          self.x, self.y, self._norm_x, self._norm_y, arr, self.cost_fn,
-          self.inv_scale_cost, fn
+          self.x, self.y, self._norm_x, self._norm_y, arr,
+          self.cost_fn.pairwise, self.inv_scale_cost, fn
       )
+    cost_fn = lambda y, x: self.cost_fn.pairwise(x, y)
     return app(
-        self.y, self.x, self._norm_y, self._norm_x, arr, self.cost_fn,
+        self.y, self.x, self._norm_y, self._norm_x, arr, cost_fn,
         self.inv_scale_cost, fn
     )
 
   def vec_apply_cost(
       self,
       arr: jnp.ndarray,
       axis: int = 0,
@@ -448,49 +427,39 @@
       summary: can be 'mean' or 'max_cost'.
 
     Returns:
       summary statistics
     """
     scale_cost = 1.0
 
-    def body0(carry, i: int):
-      vec, = carry
+    def body0(vec: jnp.ndarray, i: int):
       y = self._leading_slice(self.y, i)
-      if self._axis_norm is None:
-        norm_y = self._norm_y
-      else:
-        norm_y = self._leading_slice(self._norm_y, i)
-      h_res = app(
-          self.x, y, self._norm_x, norm_y, vec, self.cost_fn, scale_cost
+      norm_y = self._norm_y if self._axis_norm is None else self._leading_slice(
+          self._norm_y, i
       )
-      return carry, h_res
+      h_res = app(self.x, y, self._norm_x, norm_y, vec, cost_fn, scale_cost)
+      return vec, h_res
 
-    def body1(carry, i: int):
-      vec, = carry
+    def body1(vec: jnp.ndarray, i: int):
       x = self._leading_slice(self.x, i)
-      if self._axis_norm is None:
-        norm_x = self._norm_x
-      else:
-        norm_x = self._leading_slice(self._norm_x, i)
-      h_res = app(
-          self.y, x, self._norm_y, norm_x, vec, self.cost_fn, scale_cost
+      norm_x = self._norm_x if self._axis_norm is None else self._leading_slice(
+          self._norm_x, i
       )
-      return carry, h_res
+      h_res = app(self.y, x, self._norm_y, norm_x, vec, cost_fn, scale_cost)
+      return vec, h_res
 
-    def finalize(i: int):
+    def rest(i: int) -> jnp.ndarray:
       if batch_for_y:
         norm_y = self._norm_y if self._axis_norm is None else self._norm_y[i:]
         return app(
-            self.x, self.y[i:], self._norm_x, norm_y, vec, self.cost_fn,
-            scale_cost
+            self.x, self.y[i:], self._norm_x, norm_y, vec, cost_fn, scale_cost
         )
       norm_x = self._norm_x if self._axis_norm is None else self._norm_x[i:]
       return app(
-          self.y, self.x[i:], self._norm_y, norm_x, vec, self.cost_fn,
-          scale_cost
+          self.y, self.x[i:], self._norm_y, norm_x, vec, cost_fn, scale_cost
       )
 
     if summary == "mean":
       fn = _apply_cost_xy
     elif summary == "max_cost":
       fn = _apply_max_xy
     else:
@@ -499,31 +468,30 @@
       )
     app = jax.vmap(
         fn, in_axes=[None, 0, None, self._axis_norm, None, None, None]
     )
 
     batch_for_y = self.shape[0] < self.shape[1]
     if batch_for_y:
-      fun = body0
+      fun, cost_fn = body0, self.cost_fn.pairwise
       n = self._y_nsplit
       vec, other = self._n_normed_ones, self._m_normed_ones
     else:
-      fun = body1
+      fun, cost_fn = body1, lambda y, x: self.cost_fn.pairwise(x, y)
       n = self._x_nsplit
       vec, other = self._m_normed_ones, self._n_normed_ones
 
-    _, val = jax.lax.scan(fun, init=(vec,), xs=jnp.arange(n))
+    _, val = jax.lax.scan(fun, init=vec, xs=jnp.arange(n))
     val = jnp.concatenate(val).squeeze()
-    val_rest = finalize(n * self.batch_size)
+    val_rest = rest(n * self.batch_size)
     val_res = jnp.concatenate([val, val_rest])
 
     if summary == "mean":
       return jnp.sum(val_res * other)
     if summary == "max_cost":
-      # TODO(michalk8): explain why scaling is not needed
       return jnp.max(val_res)
     raise ValueError(
         f"Scaling method {summary} does not exist for online mode."
     )
 
   def barycenter(self, weights: jnp.ndarray) -> jnp.ndarray:
     """Compute barycenter of points in self.x using weights."""
@@ -579,15 +547,15 @@
 
   def _cosine_to_sqeucl(self) -> "PointCloud":
     assert isinstance(self.cost_fn, costs.Cosine), type(self.cost_fn)
     (x, y, *args, _), aux_data = self.tree_flatten()
     x = x / jnp.linalg.norm(x, axis=-1, keepdims=True)
     y = y / jnp.linalg.norm(y, axis=-1, keepdims=True)
     # TODO(michalk8): find a better way
-    aux_data["scale_cost"] = 2. / self.inv_scale_cost
+    aux_data["scale_cost"] = 2.0 / self.inv_scale_cost
     cost_fn = costs.SqEuclidean()
     return type(self).tree_unflatten(aux_data, [x, y] + args + [cost_fn])
 
   def to_LRCGeometry(
       self,
       scale: float = 1.0,
       **kwargs: Any,
@@ -608,17 +576,14 @@
       Otherwise, returns the re-scaled low-rank geometry.
     """
     if self.is_squared_euclidean:
       if self._check_LRC_dim:
         return self._sqeucl_to_lr(scale)
       # we don't update the `scale_factor` because in GW, the linear cost
       # is first materialized and then scaled by `fused_penalty` afterwards
-
-      # TODO(michalk8): in the future, consider defining point cloud as a
-      # subclass of LRCGeometry
       return self
     return super().to_LRCGeometry(scale=scale, **kwargs)
 
   def _sqeucl_to_lr(self, scale: float = 1.0) -> low_rank.LRCGeometry:
     assert self.is_squared_euclidean, "Geometry must be squared Euclidean."
     n, m = self.shape
     nx = jnp.sum(self.x ** 2, axis=1, keepdims=True)
@@ -644,25 +609,25 @@
       **kwargs: Any
   ) -> "PointCloud":
 
     def subset_fn(
         arr: Optional[jnp.ndarray],
         ixs: Optional[jnp.ndarray],
     ) -> jnp.ndarray:
-      return arr if arr is None or ixs is None else arr[jnp.atleast_1d(ixs)]
+      return arr if arr is None or ixs is None else arr[ixs, ...]
 
     return self._mask_subset_helper(
         src_ixs, tgt_ixs, fn=subset_fn, propagate_mask=True, **kwargs
     )
 
   def mask(  # noqa: D102
       self,
       src_mask: Optional[jnp.ndarray],
       tgt_mask: Optional[jnp.ndarray],
-      mask_value: float = 0.,
+      mask_value: float = 0.0,
   ) -> "PointCloud":
 
     def mask_fn(
         arr: Optional[jnp.ndarray],
         mask: Optional[jnp.ndarray],
     ) -> Optional[jnp.ndarray]:
       if arr is None or mask is None:
@@ -732,34 +697,32 @@
   c = _cost(x, y, norm_x, norm_y, cost_fn, scale_cost)
   return mu.logsumexp((f + g - c) / eps, b=vec, return_sign=True, axis=-1)
 
 
 def _transport_from_potentials_xy(
     x, y, norm_x, norm_y, f, g, eps, cost_fn, scale_cost
 ):
-  return jnp.exp(
-      (f + g - _cost(x, y, norm_x, norm_y, cost_fn, scale_cost)) / eps
-  )
+  c = _cost(x, y, norm_x, norm_y, cost_fn, scale_cost)
+  return jnp.exp((f + g - c) / eps)
 
 
 def _apply_kernel_xy(x, y, norm_x, norm_y, vec, eps, cost_fn, scale_cost):
   c = _cost(x, y, norm_x, norm_y, cost_fn, scale_cost)
   return jnp.dot(jnp.exp(-c / eps), vec)
 
 
 def _transport_from_scalings_xy(
     x, y, norm_x, norm_y, u, v, eps, cost_fn, scale_cost
 ):
-  return jnp.exp(
-      -_cost(x, y, norm_x, norm_y, cost_fn, scale_cost) * scale_cost / eps
-  ) * u * v
+  c = _cost(x, y, norm_x, norm_y, cost_fn, scale_cost)
+  return jnp.exp(-c * scale_cost / eps) * u * v
 
 
 def _cost(x, y, norm_x, norm_y, cost_fn, scale_cost):
-  one_line_pairwise = jax.vmap(cost_fn.pairwise, in_axes=[0, None])
+  one_line_pairwise = jax.vmap(cost_fn, in_axes=[0, None])
   cost = norm_x + norm_y + one_line_pairwise(x, y)
   return cost * scale_cost
 
 
 def _apply_cost_xy(x, y, norm_x, norm_y, vec, cost_fn, scale_cost, fn=None):
   """Apply [num_b, num_a] fn(cost) matrix (or transpose) to vector.
```

### Comparing `ott-jax-0.4.5/src/ott/geometry/segment.py` & `ott_jax-0.4.6/src/ott/geometry/segment.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.5/src/ott/initializers/__init__.py` & `ott_jax-0.4.6/src/ott/problems/__init__.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.5/src/ott/initializers/linear/__init__.py` & `ott_jax-0.4.6/src/ott/initializers/linear/__init__.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.5/src/ott/initializers/linear/initializers.py` & `ott_jax-0.4.6/src/ott/initializers/linear/initializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,16 +101,16 @@
         n,
     ), f"Expected `f_u` to have shape `{n,}`, found `{a.shape}`."
     assert b.shape == (
         m,
     ), f"Expected `g_v` to have shape `{m,}`, found `{b.shape}`."
 
     # cancel dual variables for zero weights
-    a = jnp.where(ot_prob.a > 0., a, -jnp.inf if lse_mode else 0.)
-    b = jnp.where(ot_prob.b > 0., b, -jnp.inf if lse_mode else 0.)
+    a = jnp.where(ot_prob.a > 0.0, a, -jnp.inf if lse_mode else 0.0)
+    b = jnp.where(ot_prob.b > 0.0, b, -jnp.inf if lse_mode else 0.0)
 
     return a, b
 
   def tree_flatten(self) -> Tuple[Sequence[Any], Dict[str, Any]]:  # noqa: D102
     return [], {}
 
   @classmethod
@@ -335,18 +335,18 @@
     rng_x, rng_y = jax.random.split(rng, 2)
 
     x, y = ot_prob.geom.x, ot_prob.geom.y
     a, b = ot_prob.a, ot_prob.b
 
     # subsample
     sub_x = jax.random.choice(
-        key=rng_x, a=x, shape=(self.subsample_n_x,), replace=True, p=a, axis=0
+        rng_x, a=x, shape=(self.subsample_n_x,), replace=True, p=a, axis=0
     )
     sub_y = jax.random.choice(
-        key=rng_y, a=y, shape=(self.subsample_n_y,), replace=True, p=b, axis=0
+        rng_y, a=y, shape=(self.subsample_n_y,), replace=True, p=b, axis=0
     )
 
     # create subsampled point cloud geometry
     sub_geom = pointcloud.PointCloud(
         sub_x,
         sub_y,
         epsilon=ot_prob.geom.epsilon,
```

### Comparing `ott-jax-0.4.5/src/ott/initializers/linear/initializers_lr.py` & `ott_jax-0.4.6/src/ott/initializers/linear/initializers_lr.py`

 * *Files 0% similar despite different names*

```diff
@@ -258,15 +258,15 @@
   def init_g(  # noqa: D102
       self,
       ot_prob: Problem_t,
       rng: jax.Array,
       **kwargs: Any,
   ) -> jnp.ndarray:
     del kwargs
-    init_g = jnp.abs(jax.random.uniform(rng, (self.rank,))) + 1.
+    init_g = jnp.abs(jax.random.uniform(rng, (self.rank,))) + 1.0
     return init_g / jnp.sum(init_g)
 
 
 @jax.tree_util.register_pytree_node_class
 class Rank2Initializer(LRInitializer):
   """Low-rank Sinkhorn factorization using rank-2 factors :cite:`scetbon:21`.
 
@@ -296,15 +296,15 @@
     g2 = (init_g - lambda_1 * g1) / (1.0 - lambda_1)
 
     x = jnp.arange(1, n + 1)
     x /= x.astype(float).sum()
     y = (marginal - lambda_1 * x) / (1.0 - lambda_1)
 
     return ((lambda_1 * x[:, None] @ g1.reshape(1, -1)) +
-            ((1 - lambda_1) * y[:, None] @ g2.reshape(1, -1)))
+            ((1.0 - lambda_1) * y[:, None] @ g2.reshape(1, -1)))
 
   def init_q(  # noqa: D102
       self,
       ot_prob: Problem_t,
       rng: jax.Array,
       *,
       init_g: jnp.ndarray,
@@ -473,15 +473,15 @@
     sinkhorn_kwargs: Keyword arguments for
       :class:`~ott.solvers.linear.sinkhorn.Sinkhorn`.
   """
 
   def __init__(
       self,
       rank: int,
-      gamma: float = 10.,
+      gamma: float = 10.0,
       min_iterations: int = 0,
       max_iterations: int = 100,
       inner_iterations: int = 10,
       threshold: float = 1e-6,
       sinkhorn_kwargs: Optional[Mapping[str, Any]] = None,
   ):
     super().__init__(
@@ -519,15 +519,15 @@
   ) -> jnp.ndarray:
     from ott.problems.linear import linear_problem
     from ott.problems.quadratic import quadratic_problem
     from ott.solvers.linear import sinkhorn
 
     def init_fn() -> GeneralizedKMeansInitializer.State:
       n = geom.shape[0]
-      factor = jnp.abs(jax.random.normal(rng, (n, self.rank))) + 1.  # (n, r)
+      factor = jnp.abs(jax.random.normal(rng, (n, self.rank))) + 1.0  # (n, r)
       factor *= consts.marginal[:, None] / jnp.sum(
           factor, axis=1, keepdims=True
       )
 
       return self.State(
           factor,
           criterions=-jnp.ones(outer_iterations),
@@ -582,15 +582,15 @@
 
       grad = consts.geom.apply_cost(state.factor, axis=1)  # (n, r)
       grad = grad + consts.geom.apply_cost(state.factor, axis=0)  # (n, r)
       grad = grad / consts.g
 
       norm = jnp.max(jnp.abs(grad)) ** 2
       gamma = consts.gamma / norm
-      eps = 1. / gamma
+      eps = 1.0 / gamma
 
       cost = grad - eps * mu.safe_log(state.factor)  # (n, r)
       cost = geometry.Geometry(
           cost_matrix=cost,
           epsilon=eps,
       )
       problem = linear_problem.LinearProblem(
```

### Comparing `ott-jax-0.4.5/src/ott/initializers/quadratic/__init__.py` & `ott_jax-0.4.6/src/ott/initializers/quadratic/__init__.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.5/src/ott/initializers/quadratic/initializers.py` & `ott_jax-0.4.6/src/ott/initializers/quadratic/initializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,17 +170,15 @@
     if quad_prob.is_balanced:
       cost_matrix = marginal_cost.cost_matrix - tmp
     else:
       # initialize epsilon for Unbalanced GW according to Sejourne et. al (2021)
       init_transport = jnp.outer(quad_prob.a, quad_prob.b)
       marginal_1, marginal_2 = init_transport.sum(1), init_transport.sum(0)
 
-      epsilon = quadratic_problem.update_epsilon_unbalanced(
-          epsilon=epsilon, transport_mass=marginal_1.sum()
-      )
+      epsilon *= marginal_1.sum()
       unbalanced_correction = quad_prob.cost_unbalanced_correction(
           init_transport, marginal_1, marginal_2, epsilon=epsilon
       )
       cost_matrix = marginal_cost.cost_matrix - tmp + unbalanced_correction
 
     cost_matrix += quad_prob.fused_penalty * quad_prob._fused_cost_matrix
     return geometry.Geometry(
```

### Comparing `ott-jax-0.4.5/src/ott/math/__init__.py` & `ott_jax-0.4.6/src/ott/solvers/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,13 +7,8 @@
 #   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from . import (
-    fixed_point_loop,
-    matrix_square_root,
-    unbalanced_functions,
-    utils,
-)
+from . import linear, quadratic, utils, was_solver
```

### Comparing `ott-jax-0.4.5/src/ott/math/fixed_point_loop.py` & `ott_jax-0.4.6/src/ott/math/fixed_point_loop.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.5/src/ott/math/matrix_square_root.py` & `ott_jax-0.4.6/src/ott/math/matrix_square_root.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import functools
+import math
 from typing import Tuple
 
 import jax
 import jax.numpy as jnp
-import numpy as np
 
 from ott.math import fixed_point_loop
 
 __all__ = ["sqrtm", "sqrtm_only", "inv_sqrtm_only"]
 
 
 @functools.partial(jax.custom_vjp, nondiff_argnums=(1, 2, 3, 4, 5))
@@ -83,32 +83,30 @@
     """
     x, _ = const
     errors, y, z = state
     w = 0.5 * jnp.matmul(z, y)
     y = 1.5 * y - jnp.matmul(y, w)
     z = 1.5 * z - jnp.matmul(w, z)
 
-    err = jnp.where(compute_error, new_err(x, norm_x, y), np.inf)
+    err = jnp.where(compute_error, new_err(x, norm_x, y), jnp.inf)
 
     errors = errors.at[iteration // inner_iterations].set(err)
 
     return errors, y, z
 
   def new_err(x, norm_x, y):
     res = x - norm_x * jnp.matmul(y, y)
     norm_fn = functools.partial(jnp.linalg.norm, axis=(-2, -1))
     return jnp.max(norm_fn(res) / norm_fn(x))
 
-  dtype = x.dtype
   y = x / norm_x
-  z = jnp.eye(dimension, dtype=dtype)
+  z = jnp.eye(dimension)
   if jnp.ndim(x) > 2:
     z = jnp.tile(z, list(x.shape[:-2]) + [1, 1])
-  errors = -jnp.ones((np.ceil(max_iterations / inner_iterations).astype(int),),
-                     dtype=dtype)
+  errors = -jnp.ones(math.ceil(max_iterations / inner_iterations))
   state = (errors, y, z)
   const = (x, threshold)
   errors, y, z = fixed_point_loop.fixpoint_iter_backprop(
       cond_fn, body_fn, min_iterations, max_iterations, inner_iterations, const,
       state
   )
   sqrt_x = jnp.sqrt(norm_x) * y
@@ -135,15 +133,15 @@
   r, u = jax.lax.linalg.schur(a + 0j)
   s, v = jax.lax.linalg.schur(b + 0j)
   d = jnp.matmul(
       jnp.conjugate(jnp.swapaxes(u, axis1=-2, axis2=-1)), jnp.matmul(c, v)
   )
   # The solution in the transformed space will in general be complex, too.
   y = jnp.zeros(a.shape[:-2] + (m, n)) + 0j
-  idx = jnp.arange(m, dtype=jnp.int32)
+  idx = jnp.arange(m)
   for j in range(n):
     lhs = r.at[..., idx, idx].add(-s[..., j:j + 1, j])
     rhs = d[..., j] + jnp.matmul(y[..., :j], s[..., :j, j:j + 1])[..., 0]
     y = y.at[..., j].set(jax.scipy.linalg.solve_triangular(lhs, rhs))
 
   x = jnp.matmul(
       u, jnp.matmul(y, jnp.conjugate(jnp.swapaxes(v, axis1=-2, axis2=-1)))
```

### Comparing `ott-jax-0.4.5/src/ott/math/unbalanced_functions.py` & `ott_jax-0.4.6/src/ott/math/unbalanced_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,20 +71,20 @@
     epsilon: regularization
     derivative: Callable
 
   Returns:
     a vector of the same size as c or h.
   """
   if tau == 1.0:
-    return 0.
+    return 0.0
 
   r = rho(epsilon, tau)
   # here no minus sign because we are taking derivative w.r.t -h
   return jnp.where(
       c > 0,
       c * second_derivative_phi_star(-h, r) *
       derivative(c * derivative_phi_star(-h, r)), 0.0
   )
 
 
 def rho(epsilon: float, tau: float) -> float:  # noqa: D103
-  return (epsilon * tau) / (1. - tau)
+  return (epsilon * tau) / (1.0 - tau)
```

### Comparing `ott-jax-0.4.5/src/ott/math/utils.py` & `ott_jax-0.4.6/src/ott/math/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 def safe_log(  # noqa: D103
     x: jnp.ndarray,
     *,
     eps: Optional[float] = None
 ) -> jnp.ndarray:
   if eps is None:
     eps = jnp.finfo(x.dtype).tiny
-  return jnp.where(x > 0., jnp.log(x), jnp.log(eps))
+  return jnp.where(x > 0.0, jnp.log(x), jnp.log(eps))
 
 
 @functools.partial(jax.custom_jvp, nondiff_argnums=[1, 2, 3])
 @functools.partial(jax.jit, static_argnames=("ord", "axis", "keepdims"))
 def norm(
     x: jnp.ndarray,
     ord: Union[int, str, None] = None,
```

### Comparing `ott-jax-0.4.5/src/ott/neural/__init__.py` & `ott_jax-0.4.6/src/ott/neural/methods/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 #   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from . import layers, losses, models, solvers
+from . import monge_gap, neuraldual
```

### Comparing `ott-jax-0.4.5/src/ott/neural/layers.py` & `ott_jax-0.4.6/src/ott/neural/networks/layers/posdef.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,24 +11,24 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Any, Callable, Optional, Tuple
 
 import jax
 import jax.numpy as jnp
+
 from flax import linen as nn
 
 __all__ = ["PositiveDense", "PosDefPotentials"]
 
 PRNGKey = jax.Array
 Shape = Tuple[int, ...]
 Dtype = Any
 Array = jnp.ndarray
 
-# wrap to silence docs linter
 DEFAULT_KERNEL_INIT = lambda *a, **k: nn.initializers.lecun_normal()(*a, **k)
 DEFAULT_BIAS_INIT = nn.initializers.zeros
 DEFAULT_RECTIFIER = nn.activation.relu
 
 
 class PositiveDense(nn.Module):
   """A linear transformation using a matrix with all entries non-negative.
@@ -74,15 +74,16 @@
     if self.use_bias:
       x = x + self.param("bias", self.bias_init, (self.dim_hidden,))
 
     return x
 
 
 class PosDefPotentials(nn.Module):
-  r""":math:`\frac{1}{2} x^T (A_i A_i^T + \text{Diag}(d_i)) x + b_i^T x^2 + c_i` potentials.
+  r""":math:`\frac{1}{2} x^T (A_i A_i^T + \text{Diag}(d_i)) x + b_i^T x^2 + c_i`
+    potentials.
 
   This class implements a layer that takes (batched) ``d``-dimensional vectors
   ``x`` in, to output a ``num_potentials``-dimensional vector. Each of the
   entries in that output is a positive definite quadratic form evaluated at
   ``x``; each of these quadratic terms is parameterized as a low-rank plus
   diagonal matrix. The low-rank term is parameterized as :math:`A_i A_i^T`,
   where each of these matrices is of size ``(rank, d)``. Taken together,
@@ -106,15 +107,15 @@
     kernel_diag_init: Initializer for the diagonals :math:`d_i`.
       The default is :func:`~flax.linen.initializers.ones`.
     kernel_linear_init: Initializer for the linear layers :math:`b_i`.
       The default is :func:`~flax.linen.initializers.lecun_normal`.
     bias_init: Initializer for the bias. The default is
       :func:`~flax.linen.initializers.zeros`.
     precision: Numerical precision of the computation.
-  """  # noqa: E501
+  """  # noqa: D205,E501
 
   num_potentials: int
   rank: int = 0
   rectifier_fn: Callable[[Array], Array] = DEFAULT_RECTIFIER
   use_linear: bool = True
   use_bias: bool = True
   kernel_lr_init: Callable[[PRNGKey, Shape, Dtype], Array] = DEFAULT_KERNEL_INIT
```

### Comparing `ott-jax-0.4.5/src/ott/neural/models.py` & `ott_jax-0.4.6/src/ott/problems/linear/potentials.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,387 +7,426 @@
 #   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import functools
-from typing import Any, Callable, Dict, Optional, Sequence, Tuple, Union
+from typing import Any, Callable, Dict, Literal, Optional, Sequence, Tuple
 
 import jax
 import jax.numpy as jnp
-import optax
-from flax import linen as nn
-from flax.core import frozen_dict
-from flax.training import train_state
-
-from ott import utils
-from ott.geometry import geometry
-from ott.initializers.linear import initializers as lin_init
-from ott.neural import layers
-from ott.neural.solvers import neuraldual
-from ott.problems.linear import linear_problem
-
-__all__ = ["ICNN", "MLP", "MetaInitializer"]
-
-# wrap to silence docs linter
-DEFAULT_KERNEL_INIT = lambda *a, **k: nn.initializers.normal()(*a, **k)
-DEFAULT_RECTIFIER = nn.activation.relu
-DEFAULT_ACTIVATION = nn.activation.relu
+import jax.scipy as jsp
+import jax.tree_util as jtu
+import numpy as np
 
+from ott.geometry import costs
+from ott.problems.linear import linear_problem
 
-class ICNN(neuraldual.BaseW2NeuralDual):
-  """Input convex neural network (ICNN).
+try:
+  import matplotlib as mpl
+  import matplotlib.pyplot as plt
+except ImportError:
+  mpl = plt = None
+
+__all__ = ["DualPotentials", "EntropicPotentials"]
+Potential_t = Callable[[jnp.ndarray], float]
+
+
+@jtu.register_pytree_node_class
+class DualPotentials:
+  r"""The Kantorovich dual potential functions :math:`f` and :math:`g`.
 
-  Implementation of input convex neural networks as introduced in
-  :cite:`amos:17` with initialization schemes proposed by :cite:`bunne:22`.
+  :math:`f` and :math:`g` are a pair of functions, candidates for the dual
+  OT Kantorovich problem, supposedly optimal for a given pair of measures.
 
   Args:
-    dim_data: data dimensionality.
-    dim_hidden: sequence specifying size of hidden dimensions. The
-      output dimension of the last layer is 1 by default.
-    ranks: ranks of the matrices :math:`A_i` used as low-rank factors
-      for the quadratic potentials. If a sequence is passed, it must contain
-      ``len(dim_hidden) + 2`` elements, where the last 2 elements correspond
-      to the ranks of the final layer with dimension 1 and the potentials,
-      respectively.
-    init_fn: Initializer for the kernel weight matrices.
-      The default is :func:`~flax.linen.initializers.normal`.
-    act_fn: choice of activation function used in network architecture,
-      needs to be convex. The default is :func:`~flax.linen.activation.relu`.
-    pos_weights: Enforce positive weights with a projection.
-      If :obj:`False`, the positive weights should be enforced with clipping
-      or regularization in the loss.
-    rectifier_fn: function to ensure the non negativity of the weights.
-      The default is :func:`~flax.linen.activation.relu`.
-    gaussian_map_samples: Tuple of source and target points, used to initialize
-      the ICNN to mimic the linear Bures map that morphs the (Gaussian
-      approximation) of the input measure to that of the target measure. If
-      :obj:`None`, the identity initialization is used, and ICNN mimics half the
-      squared Euclidean norm.
+    f: The first dual potential function.
+    g: The second dual potential function.
+    cost_fn: The cost function used to solve the OT problem.
+    corr: Whether the duals solve the problem in distance form, or correlation
+      form (as used for instance for ICNNs, see, e.g., top right of p.3 in
+      :cite:`makkuva:20`)
   """
 
-  dim_data: int
-  dim_hidden: Sequence[int]
-  ranks: Union[int, Tuple[int, ...]] = 1
-  init_fn: Callable[[jax.Array, Tuple[int, ...], Any],
-                    jnp.ndarray] = DEFAULT_KERNEL_INIT
-  act_fn: Callable[[jnp.ndarray], jnp.ndarray] = DEFAULT_ACTIVATION
-  pos_weights: bool = False
-  rectifier_fn: Callable[[jnp.ndarray], jnp.ndarray] = DEFAULT_RECTIFIER
-  gaussian_map_samples: Optional[Tuple[jnp.ndarray, jnp.ndarray]] = None
-
-  def setup(self) -> None:  # noqa: D102
-    dim_hidden = list(self.dim_hidden) + [1]
-    *ranks, pos_def_rank = self._normalize_ranks()
-
-    # final layer computes average, still with normalized rescaling
-    self.w_zs = [self._get_wz(dim) for dim in dim_hidden[1:]]
-    # subsequent layers re-injected into convex functions
-    self.w_xs = [
-        self._get_wx(dim, rank) for dim, rank in zip(dim_hidden, ranks)
-    ]
-    self.pos_def_potentials = self._get_pos_def_potentials(pos_def_rank)
-
-  @nn.compact
-  def __call__(self, x: jnp.ndarray) -> float:  # noqa: D102
-    w_x, *w_xs = self.w_xs
-    assert len(self.w_zs) == len(w_xs), (len(self.w_zs), len(w_xs))
-
-    z = self.act_fn(w_x(x))
-    for w_z, w_x in zip(self.w_zs, w_xs):
-      z = self.act_fn(w_z(z) + w_x(x))
-    z = z + self.pos_def_potentials(x)
-
-    return z.squeeze()
-
-  def _get_wz(self, dim: int) -> nn.Module:
-    if self.pos_weights:
-      return layers.PositiveDense(
-          dim,
-          kernel_init=self.init_fn,
-          use_bias=False,
-          rectifier_fn=self.rectifier_fn,
-      )
+  def __init__(
+      self,
+      f: Potential_t,
+      g: Potential_t,
+      *,
+      cost_fn: costs.CostFn,
+      corr: bool = False
+  ):
+    self._f = f
+    self._g = g
+    assert (
+        not corr or type(cost_fn) == costs.SqEuclidean
+    ), "Duals in `corr` form can only be used with a squared-Euclidean cost."
+    self.cost_fn = cost_fn
+    self._corr = corr
+
+  def transport(self, vec: jnp.ndarray, forward: bool = True) -> jnp.ndarray:
+    r"""Transport ``vec`` according to Gangbo-McCann Brenier :cite:`brenier:91`.
+
+    Uses Proposition 1.15 from :cite:`santambrogio:15` to compute an OT map when
+    applying the inverse gradient of cost.
+
+    When the cost is a general cost, the operator uses the
+    :meth:`~ott.geometry.costs.CostFn.twist_operator` associated of the
+    corresponding :class:`~ott.geometry.costs.CostFn`.
+
+    When the cost is a translation invariant :class:`~ott.geometry.costs.TICost`
+    cost, :math:`c(x,y)=h(x-y)`, and the twist operator translates to the
+    application of the convex conjugate of :math:`h` to the
+    gradient of the dual potentials, namely
+    :math:`x- (\nabla h^*)\circ \nabla f(x)` for the forward map,
+    where :math:`h^*` is the Legendre transform of :math:`h`. For instance,
+    in the case :math:`h(\cdot) = \|\cdot\|^2, \nabla h(\cdot) = 2 \cdot\,`,
+    one has :math:`h^*(\cdot) = \|.\|^2 / 4`, and therefore
+    :math:`\nabla h^*(\cdot) = 0.5 \cdot\,`.
+
+    Note:
+      When the dual potentials are solved in correlation form, and marked
+      accordingly by setting ``corr`` to ``True``, the maps are
+      :math:`\nabla g` for forward, :math:`\nabla f` for backward map. This can
+      only make sense when using the squared-Euclidean
+      :class:`~ott.geometry.costs.SqEuclidean` cost.
 
-    return nn.Dense(
-        dim,
-        kernel_init=self.init_fn,
-        use_bias=False,
-    )
+    Args:
+      vec: Points to transport, array of shape ``[n, d]``.
+      forward: Whether to transport the points from source to the target
+        distribution or vice-versa.
 
-  def _get_wx(self, dim: int, rank: int) -> nn.Module:
-    return layers.PosDefPotentials(
-        rank=rank,
-        num_potentials=dim,
-        use_linear=True,
-        use_bias=True,
-        kernel_diag_init=nn.initializers.zeros,
-        kernel_lr_init=self.init_fn,
-        kernel_linear_init=self.init_fn,
-        bias_init=nn.initializers.zeros,
-    )
+    Returns:
+      The transported points.
+    """
+    from ott.geometry import costs
 
-  def _get_pos_def_potentials(self, rank: int) -> layers.PosDefPotentials:
-    kwargs = {
-        "num_potentials": 1,
-        "use_linear": True,
-        "use_bias": True,
-        "bias_init": nn.initializers.zeros
-    }
+    vec = jnp.atleast_2d(vec)
 
-    if self.gaussian_map_samples is None:
-      return layers.PosDefPotentials(
-          rank=rank,
-          kernel_diag_init=nn.initializers.ones,
-          kernel_lr_init=nn.initializers.zeros,
-          kernel_linear_init=nn.initializers.zeros,
-          **kwargs,
-      )
+    if self._corr and isinstance(self.cost_fn, costs.SqEuclidean):
+      return self._grad_f(vec) if forward else self._grad_g(vec)
+    twist_op = jax.vmap(self.cost_fn.twist_operator, in_axes=[0, 0, None])
+    if forward:
+      return twist_op(vec, self._grad_f(vec), False)
+    return twist_op(vec, self._grad_g(vec), True)
+
+  def distance(self, src: jnp.ndarray, tgt: jnp.ndarray) -> float:
+    r"""Evaluate Wasserstein distance between samples using dual potentials.
+
+    This uses direct estimation of potentials against measures when dual
+    functions are provided in usual form. This expression is valid for any
+    cost function.
+
+    When potentials are given in correlation form, as specified by the flag
+    ``corr``, the dual potentials solve the dual problem corresponding to the
+    minimization of the primal OT problem where the ground cost is
+    :math:`-2\langle x,y\rangle`. To recover the (squared) 2-Wasserstein
+    distance, terms are re-arranged and contributions from squared norms are
+    taken into account.
 
-    source, target = self.gaussian_map_samples
-    return layers.PosDefPotentials.init_from_samples(
-        source,
-        target,
-        rank=self.dim_data,
-        kernel_diag_init=nn.initializers.zeros,
-        **kwargs,
-    )
+    Args:
+      src: Samples from the source distribution, array of shape ``[n, d]``.
+      tgt: Samples from the target distribution, array of shape ``[m, d]``.
 
-  def _normalize_ranks(self) -> Tuple[int, ...]:
-    # +2 for the newly added layer with 1 + the final potentials
-    n_ranks = len(self.dim_hidden) + 2
-    if isinstance(self.ranks, int):
-      return (self.ranks,) * n_ranks
+    Returns:
+      Wasserstein distance using specified cost function.
+    """
+    src, tgt = jnp.atleast_2d(src), jnp.atleast_2d(tgt)
+    f = jax.vmap(self.f)
+    g = jax.vmap(self.g)
+    out = jnp.mean(f(src)) + jnp.mean(g(tgt))
+    if self._corr:
+      out = -2.0 * out + jnp.mean(jnp.sum(src ** 2, axis=-1))
+      out += jnp.mean(jnp.sum(tgt ** 2, axis=-1))
+    return out
 
-    assert len(self.ranks) == n_ranks, (len(self.ranks), n_ranks)
-    return tuple(self.ranks)
+  @property
+  def f(self) -> Potential_t:
+    """The first dual potential function."""
+    return self._f
 
   @property
-  def is_potential(self) -> bool:  # noqa: D102
-    return True
+  def g(self) -> Potential_t:
+    """The second dual potential function."""
+    return self._g
 
+  @property
+  def _grad_f(self) -> Callable[[jnp.ndarray], jnp.ndarray]:
+    """Vectorized gradient of the potential function :attr:`f`."""
+    return jax.vmap(jax.grad(self.f, argnums=0))
 
-class MLP(neuraldual.BaseW2NeuralDual):
-  """A generic, not-convex MLP.
+  @property
+  def _grad_g(self) -> Callable[[jnp.ndarray], jnp.ndarray]:
+    """Vectorized gradient of the potential function :attr:`g`."""
+    return jax.vmap(jax.grad(self.g, argnums=0))
 
-  Args:
-    dim_hidden: sequence specifying size of hidden dimensions. The output
-      dimension of the last layer is automatically set to 1 if
-      :attr:`is_potential` is ``True``, or the dimension of the input otherwise
-    is_potential: Model the potential if ``True``, otherwise
-      model the gradient of the potential
-    act_fn: Activation function
-  """
+  def tree_flatten(self) -> Tuple[Sequence[Any], Dict[str, Any]]:  # noqa: D102
+    return [], {
+        "f": self._f,
+        "g": self._g,
+        "cost_fn": self.cost_fn,
+        "corr": self._corr
+    }
 
-  dim_hidden: Sequence[int]
-  is_potential: bool = True
-  act_fn: Callable[[jnp.ndarray], jnp.ndarray] = nn.leaky_relu
-
-  @nn.compact
-  def __call__(self, x: jnp.ndarray) -> jnp.ndarray:  # noqa: D102
-    squeeze = x.ndim == 1
-    if squeeze:
-      x = jnp.expand_dims(x, 0)
-    assert x.ndim == 2, x.ndim
-    n_input = x.shape[-1]
-
-    z = x
-    for n_hidden in self.dim_hidden:
-      Wx = nn.Dense(n_hidden, use_bias=True)
-      z = self.act_fn(Wx(z))
-
-    if self.is_potential:
-      Wx = nn.Dense(1, use_bias=True)
-      z = Wx(z).squeeze(-1)
+  @classmethod
+  def tree_unflatten(  # noqa: D102
+      cls, aux_data: Dict[str, Any], children: Sequence[Any]
+  ) -> "DualPotentials":
+    return cls(*children, **aux_data)
 
-      quad_term = 0.5 * jax.vmap(jnp.dot)(x, x)
-      z += quad_term
-    else:
-      Wx = nn.Dense(n_input, use_bias=True)
-      z = x + Wx(z)
+  def plot_ot_map(
+      self,
+      source: jnp.ndarray,
+      target: jnp.ndarray,
+      samples: Optional[jnp.ndarray] = None,
+      forward: bool = True,
+      ax: Optional["plt.Axes"] = None,
+      scatter_kwargs: Optional[Dict[str, Any]] = None,
+      legend_kwargs: Optional[Dict[str, Any]] = None,
+  ) -> Tuple["plt.Figure", "plt.Axes"]:
+    """Plot data and learned optimal transport map.
 
-    return z.squeeze(0) if squeeze else z
+    Args:
+      source: samples from the source measure
+      target: samples from the target measure
+      samples: extra samples to transport, either ``source`` (if ``forward``) or
+        ``target`` (if not ``forward``) by default.
+      forward: use the forward map from the potentials if ``True``,
+        otherwise use the inverse map.
+      ax: axis to add the plot to
+      scatter_kwargs: additional kwargs passed into
+        :meth:`~matplotlib.axes.Axes.scatter`
+      legend_kwargs: additional kwargs passed into
+        :meth:`~matplotlib.axes.Axes.legend`
 
+    Returns:
+      Figure and axes.
+    """
+    if mpl is None:
+      raise RuntimeError("Please install `matplotlib` first.")
 
-@jax.tree_util.register_pytree_node_class
-class MetaInitializer(lin_init.DefaultInitializer):
-  """Meta OT Initializer with a fixed geometry :cite:`amos:22`.
+    if scatter_kwargs is None:
+      scatter_kwargs = {"alpha": 0.5}
+    if legend_kwargs is None:
+      legend_kwargs = {
+          "ncol": 3,
+          "loc": "upper center",
+          "bbox_to_anchor": (0.5, -0.05),
+          "edgecolor": "k"
+      }
+
+    if ax is None:
+      fig = plt.figure(facecolor="white")
+      ax = fig.add_subplot(111)
+    else:
+      fig = ax.get_figure()
 
-  This initializer consists of a predictive model that outputs the
-  :math:`f` duals to solve the entropy-regularized OT problem given
-  input probability weights ``a`` and ``b``, and a given (assumed to be
-  fixed) geometry ``geom``.
+    # plot the source and target samples
+    if forward:
+      label_transport = r"$\nabla f(source)$"
+      source_color, target_color = "#1A254B", "#A7BED3"
+    else:
+      label_transport = r"$\nabla g(target)$"
+      source_color, target_color = "#A7BED3", "#1A254B"
 
-  The model's parameters are learned using a training set of OT
-  instances (multiple pairs of probability weights), that assume the
-  **same** geometry ``geom`` is used throughout, both for training and
-  evaluation.
+    ax.scatter(
+        source[:, 0],
+        source[:, 1],
+        color=source_color,
+        label="source",
+        **scatter_kwargs,
+    )
+    ax.scatter(
+        target[:, 0],
+        target[:, 1],
+        color=target_color,
+        label="target",
+        **scatter_kwargs,
+    )
 
-  Args:
-    geom: The fixed geometry of the problem instances.
-    meta_model: The model to predict the potential :math:`f` from the measures.
-    opt: The optimizer to update the parameters. If :obj:`None`, use
-      :func:`optax.adam` with :math:`0.001` learning rate.
-    rng: The PRNG key to use for initializing the model.
-    state: The training state of the model to start from.
-
-  Examples:
-    The following code shows a simple
-    example of using ``update`` to train the model, where
-    ``a`` and ``b`` are the weights of the measures and
-    ``geom`` is the fixed geometry.
-
-    .. code-block:: python
-
-      meta_initializer = init_lib.MetaInitializer(geom)
-      while training():
-        a, b = sample_batch()
-        loss, init_f, meta_initializer.state = meta_initializer.update(
-          meta_initializer.state, a=a, b=b
-        )
-  """
+    # plot the transported samples
+    samples = (source if forward else target) if samples is None else samples
+    transported_samples = self.transport(samples, forward=forward)
+    ax.scatter(
+        transported_samples[:, 0],
+        transported_samples[:, 1],
+        color="#F2545B",
+        label=label_transport,
+        **scatter_kwargs,
+    )
 
-  def __init__(
-      self,
-      geom: geometry.Geometry,
-      meta_model: nn.Module,
-      opt: Optional[optax.GradientTransformation
-                   ] = optax.adam(learning_rate=1e-3),  # noqa: B008
-      rng: Optional[jax.Array] = None,
-      state: Optional[train_state.TrainState] = None,
-  ):
-    self.geom = geom
-    self.opt = opt
-    self.rng = utils.default_prng_key(rng)
-
-    na, nb = geom.shape
-    self.meta_model = meta_model
-
-    if state is None:
-      # Initialize the model's training state.
-      placeholder = jnp.concatenate([jnp.zeros(na), jnp.zeros(nb)], axis=-1)
-      params = self.meta_model.init(self.rng, placeholder)["params"]
-      self.state = train_state.TrainState.create(
-          apply_fn=self.meta_model.apply, params=params, tx=opt
+    for i in range(samples.shape[0]):
+      ax.arrow(
+          samples[i, 0],
+          samples[i, 1],
+          transported_samples[i, 0] - samples[i, 0],
+          transported_samples[i, 1] - samples[i, 1],
+          color=[0.5, 0.5, 1],
+          alpha=0.3,
       )
-    else:
-      self.state = state
 
-    self.update_impl = self._get_update_fn()
+    ax.legend(**legend_kwargs)
+    return fig, ax
 
-  def update(
-      self, state: train_state.TrainState, a: jnp.ndarray, b: jnp.ndarray
-  ) -> Tuple[jnp.ndarray, jnp.ndarray, train_state.TrainState]:
-    r"""Update the meta model with the dual objective.
-
-    The goal is for the model to match the optimal duals, i.e.,
-    :math:`\hat f_\theta \approx f^\star`.
-    This can be done by training the predictions of :math:`\hat f_\theta`
-    to optimize the dual objective, which :math:`f^\star` also optimizes for.
-    The overall learning setup can thus be written as:
-
-    .. math::
-      \min_\theta\; {\mathbb E}_{(\alpha,\beta)\sim{\mathcal{D}}}\;
-      J(\hat f_\theta(a, b); \alpha, \beta),
-
-    where :math:`a,b` are the probabilities of the measures :math:`\alpha,\beta`
-    ,:math:`\mathcal{D}` is a meta distribution of optimal transport problems,
-
-    .. math::
-      -J(f; \alpha, \beta, c) := \langle f, a\rangle + \langle g, b \rangle -
-      \varepsilon\left\langle \exp\{f/\varepsilon\}, K\exp\{g/\varepsilon\}
-      \right\rangle
-
-    is the entropic dual objective,
-    and :math:`K_{i,j} := -C_{i,j}/\varepsilon` is the *Gibbs kernel*.
+  def plot_potential(
+      self,
+      forward: bool = True,
+      quantile: float = 0.05,
+      kantorovich: bool = True,
+      ax: Optional["mpl.axes.Axes"] = None,
+      x_bounds: Tuple[float, float] = (-6, 6),
+      y_bounds: Tuple[float, float] = (-6, 6),
+      num_grid: int = 50,
+      contourf_kwargs: Optional[Dict[str, Any]] = None,
+  ) -> Tuple["mpl.figure.Figure", "mpl.axes.Axes"]:
+    r"""Plot the potential.
 
     Args:
-      state: Optimizer state of the meta model.
-      a: Probabilities of the :math:`\alpha` measure's atoms.
-      b: Probabilities of the :math:`\beta` measure's atoms.
+      forward: use the forward map from the potentials
+        if ``True``, otherwise use the inverse map
+      quantile: quantile to filter the potentials with
+      kantorovich: whether to plot the Kantorovich potential
+      ax: axis to add the plot to
+      x_bounds: x-axis bounds of the plot
+        :math:`(x_{\text{min}}, x_{\text{max}})`
+      y_bounds: y-axis bounds of the plot
+        :math:`(y_{\text{min}}, y_{\text{max}})`
+      num_grid: number of points to discretize the domain into a grid
+        along each dimension
+      contourf_kwargs: additional kwargs passed into
+        :meth:`~matplotlib.axes.Axes.contourf`
 
     Returns:
-      The training loss, :math:`f`, and updated state.
+      Figure and axes.
     """
-    return self.update_impl(state, a, b)
+    if contourf_kwargs is None:
+      contourf_kwargs = {}
 
-  def init_dual_a(  # noqa: D102
-      self,
-      ot_prob: "linear_problem.LinearProblem",
-      lse_mode: bool,
-      rng: Optional[jax.Array] = None,
-  ) -> jnp.ndarray:
-    del rng
-    # Detect if the problem is batched.
-    assert ot_prob.a.ndim in (1, 2)
-    assert ot_prob.b.ndim in (1, 2)
-    vmap_a_val = 0 if ot_prob.a.ndim == 2 else None
-    vmap_b_val = 0 if ot_prob.b.ndim == 2 else None
-
-    if vmap_a_val is not None or vmap_b_val is not None:
-      compute_f_maybe_batch = jax.vmap(
-          self._compute_f, in_axes=(vmap_a_val, vmap_b_val, None)
-      )
+    ax_specified = ax is not None
+    if not ax_specified:
+      fig, ax = plt.subplots(figsize=(6, 6), facecolor="white")
     else:
-      compute_f_maybe_batch = self._compute_f
+      fig = ax.get_figure()
 
-    init_f = compute_f_maybe_batch(ot_prob.a, ot_prob.b, self.state.params)
-    return init_f if lse_mode else ot_prob.geom.scaling_from_potential(init_f)
+    x1 = jnp.linspace(*x_bounds, num=num_grid)
+    x2 = jnp.linspace(*y_bounds, num=num_grid)
+    X1, X2 = jnp.meshgrid(x1, x2)
+    X12flat = jnp.hstack((X1.reshape(-1, 1), X2.reshape(-1, 1)))
+    Zflat = jax.vmap(self.f if forward else self.g)(X12flat)
+    if kantorovich:
+      Zflat = 0.5 * (jnp.linalg.norm(X12flat, axis=-1) ** 2) - Zflat
+    Zflat = np.asarray(Zflat)
+    vmin, vmax = np.quantile(Zflat, [quantile, 1.0 - quantile])
+    Zflat = Zflat.clip(vmin, vmax)
+    Z = Zflat.reshape(X1.shape)
+
+    CS = ax.contourf(X1, X2, Z, cmap="Blues", **contourf_kwargs)
+    ax.set_xlim(*x_bounds)
+    ax.set_ylim(*y_bounds)
+    fig.colorbar(CS, ax=ax)
+    if not ax_specified:
+      fig.tight_layout()
+    ax.set_title(r"$f$" if forward else r"$g$")
+    return fig, ax
+
+
+@jtu.register_pytree_node_class
+class EntropicPotentials(DualPotentials):
+  """Dual potential functions from finite samples :cite:`pooladian:21`.
 
-  def _get_update_fn(self):
-    """Return the implementation (and jitted) update function."""
-    from ott.problems.linear import linear_problem
-    from ott.solvers.linear import sinkhorn
-
-    def dual_obj_loss_single(params, a, b):
-      f_pred = self._compute_f(a, b, params)
-      g_pred = self.geom.update_potential(
-          f_pred, jnp.zeros_like(b), jnp.log(b), 0, axis=0
-      )
-      g_pred = jnp.where(jnp.isfinite(g_pred), g_pred, 0.0)
+  Args:
+    f_xy: The first dual potential vector of shape ``[n,]``.
+    g_xy: The second dual potential vector of shape ``[m,]``.
+    prob: Linear problem with :class:`~ott.geometry.pointcloud.PointCloud`
+      geometry that was used to compute the dual potentials using, e.g.,
+      :class:`~ott.solvers.linear.sinkhorn.Sinkhorn`.
+    f_xx: The first dual potential vector of shape ``[n,]`` used for debiasing
+      :cite:`pooladian:22`.
+    g_yy: The second dual potential vector of shape ``[m,]`` used for debiasing.
+  """
 
-      ot_prob = linear_problem.LinearProblem(geom=self.geom, a=a, b=b)
-      dual_obj = sinkhorn.compute_kl_reg_cost(
-          f_pred, g_pred, ot_prob, lse_mode=True
-      )
-      loss = -dual_obj
-      return loss, f_pred
+  def __init__(
+      self,
+      f_xy: jnp.ndarray,
+      g_xy: jnp.ndarray,
+      prob: linear_problem.LinearProblem,
+      f_xx: Optional[jnp.ndarray] = None,
+      g_yy: Optional[jnp.ndarray] = None,
+  ):
+    # we pass directly the arrays and override the properties
+    # since only the properties need to be callable
+    super().__init__(f_xy, g_xy, cost_fn=prob.geom.cost_fn, corr=False)
+    self._prob = prob
+    self._f_xx = f_xx
+    self._g_yy = g_yy
 
-    def loss_batch(params, a, b):
-      loss_fn = functools.partial(dual_obj_loss_single, params=params)
-      loss, f_pred = jax.vmap(loss_fn)(a=a, b=b)
-      return jnp.mean(loss), f_pred
-
-    @jax.jit
-    def update(state, a, b):
-      a = jnp.atleast_2d(a)
-      b = jnp.atleast_2d(b)
-      grad_fn = jax.value_and_grad(loss_batch, has_aux=True)
-      (loss, init_f), grads = grad_fn(state.params, a, b)
-      return loss, init_f, state.apply_gradients(grads=grads)
-
-    return update
-
-  def _compute_f(
-      self, a: jnp.ndarray, b: jnp.ndarray,
-      params: frozen_dict.FrozenDict[str, jnp.ndarray]
-  ) -> jnp.ndarray:
-    r"""Predict the optimal :math:`f` potential.
+  @property
+  def f(self) -> Potential_t:  # noqa: D102
+    return self._potential_fn(kind="f")
 
-    Args:
-      a: Probabilities of the :math:`\alpha` measure's atoms.
-      b: Probabilities of the :math:`\beta` measure's atoms.
-      params: The parameters of the Meta model.
+  @property
+  def g(self) -> Potential_t:  # noqa: D102
+    return self._potential_fn(kind="g")
 
-    Returns:
-      The :math:`f` potential.
-    """
-    return self.meta_model.apply({"params": params},
-                                 jnp.concatenate([a, b], axis=-1))
+  def _potential_fn(self, *, kind: Literal["f", "g"]) -> Potential_t:
+    from ott.geometry import pointcloud
+
+    def callback(
+        x: jnp.ndarray,
+        *,
+        potential: jnp.ndarray,
+        y: jnp.ndarray,
+        weights: jnp.ndarray,
+        epsilon: float,
+    ) -> float:
+      x = jnp.atleast_2d(x)
+      assert x.shape[-1] == y.shape[-1], (x.shape, y.shape)
+      geom = pointcloud.PointCloud(x, y, cost_fn=self.cost_fn)
+      cost = geom.cost_matrix
+      z = (potential - cost) / epsilon
+      lse = -epsilon * jsp.special.logsumexp(z, b=weights, axis=-1)
+      return jnp.squeeze(lse)
+
+    assert isinstance(
+        self._prob.geom, pointcloud.PointCloud
+    ), f"Expected point cloud geometry, found `{type(self._prob.geom)}`."
+    x, y = self._prob.geom.x, self._prob.geom.y
+    a, b = self._prob.a, self._prob.b
+
+    if kind == "f":
+      # When seeking to evaluate 1st potential function,
+      # the 2nd set of potential values and support should be used,
+      # see proof of Prop. 2 in https://arxiv.org/pdf/2109.12004.pdf
+      potential, arr, weights = self._g, y, b
+    else:
+      potential, arr, weights = self._f, x, a
+
+    potential_xy = jax.tree_util.Partial(
+        callback,
+        potential=potential,
+        y=arr,
+        weights=weights,
+        epsilon=self.epsilon,
+    )
+    if not self.is_debiased:
+      return potential_xy
+
+    ep = EntropicPotentials(self._f_xx, self._g_yy, prob=self._prob)
+    # switch the order because for `kind='f'` we require `f/x/a` in `other`
+    # which is accessed when `kind='g'`
+    potential_other = ep._potential_fn(kind="g" if kind == "f" else "f")
+
+    return lambda x: (potential_xy(x) - potential_other(x))
+
+  @property
+  def is_debiased(self) -> bool:
+    """Whether the entropic map is debiased."""
+    return self._f_xx is not None and self._g_yy is not None
+
+  @property
+  def epsilon(self) -> float:
+    """Entropy regularizer."""
+    return self._prob.geom.epsilon
 
   def tree_flatten(self) -> Tuple[Sequence[Any], Dict[str, Any]]:  # noqa: D102
-    return [self.geom, self.meta_model, self.opt], {
-        "rng": self.rng,
-        "state": self.state
-    }
+    return [self._f, self._g, self._prob, self._f_xx, self._g_yy], {}
```

### Comparing `ott-jax-0.4.5/src/ott/neural/solvers/__init__.py` & `ott_jax-0.4.6/src/ott/neural/networks/layers/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 #   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from . import conjugate, map_estimator, neuraldual
+from . import conjugate, posdef, time_encoder
```

### Comparing `ott-jax-0.4.5/src/ott/neural/solvers/conjugate.py` & `ott_jax-0.4.6/src/ott/neural/networks/layers/conjugate.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.5/src/ott/neural/solvers/neuraldual.py` & `ott_jax-0.4.6/src/ott/neural/methods/neuraldual.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,174 +7,53 @@
 #   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import abc
 import warnings
 from typing import (
-    Any,
     Callable,
     Dict,
     Iterator,
     List,
     Literal,
     Optional,
     Tuple,
     Union,
 )
 
 import jax
 import jax.numpy as jnp
+
 import optax
-from flax import linen as nn
-from flax import struct
-from flax.core import frozen_dict
-from flax.training import train_state
 
 from ott import utils
 from ott.geometry import costs
-from ott.neural import models
-from ott.neural.solvers import conjugate
-from ott.problems.linear import potentials
+from ott.neural.networks import icnn, potentials
+from ott.neural.networks.layers import conjugate
+from ott.problems.linear import potentials as dual_potentials
 
-__all__ = ["W2NeuralTrainState", "BaseW2NeuralDual", "W2NeuralDual"]
+__all__ = ["W2NeuralDual"]
 
 Train_t = Dict[Literal["train_logs", "valid_logs"], Dict[str, List[float]]]
-Callback_t = Callable[[int, potentials.DualPotentials], None]
-
-PotentialValueFn_t = Callable[[jnp.ndarray], jnp.ndarray]
-PotentialGradientFn_t = Callable[[jnp.ndarray], jnp.ndarray]
-
-
-class W2NeuralTrainState(train_state.TrainState):
-  """Adds information about the model's value and gradient to the state.
-
-  This extends :class:`~flax.training.train_state.TrainState` to include
-  the potential methods from the
-  :class:`~ott.neural.solvers.neuraldual.BaseW2NeuralDual` used during training.
-
-  Args:
-    potential_value_fn: the potential's value function
-    potential_gradient_fn: the potential's gradient function
-  """
-  potential_value_fn: Callable[
-      [frozen_dict.FrozenDict[str, jnp.ndarray], Optional[PotentialValueFn_t]],
-      PotentialValueFn_t] = struct.field(pytree_node=False)
-  potential_gradient_fn: Callable[[frozen_dict.FrozenDict[str, jnp.ndarray]],
-                                  PotentialGradientFn_t] = struct.field(
-                                      pytree_node=False
-                                  )
-
-
-class BaseW2NeuralDual(abc.ABC, nn.Module):
-  """Base class for the neural solver models."""
-
-  @property
-  @abc.abstractmethod
-  def is_potential(self) -> bool:
-    """Indicates if the module implements a potential value or a vector field.
-
-    Returns:
-      ``True`` if the module defines a potential, ``False`` if it defines a
-       vector field.
-    """
-
-  def potential_value_fn(
-      self,
-      params: frozen_dict.FrozenDict[str, jnp.ndarray],
-      other_potential_value_fn: Optional[PotentialValueFn_t] = None,
-  ) -> PotentialValueFn_t:
-    r"""Return a function giving the value of the potential.
-
-    Applies the module if :attr:`is_potential` is ``True``, otherwise
-    constructs the value of the potential from the gradient with
-
-    .. math::
-
-      g(y) = -f(\nabla_y g(y)) + y^T \nabla_y g(y)
-
-    where :math:`\nabla_y g(y)` is detached for the envelope theorem
-    :cite:`danskin:67,bertsekas:71`
-    to give the appropriate first derivatives of this construction.
-
-    Args:
-      params: parameters of the module
-      other_potential_value_fn: function giving the value of the other
-        potential. Only needed when :attr:`is_potential` is ``False``.
-
-    Returns:
-      A function that can be evaluated to obtain a potential value, or a linear
-      interpolation of a potential.
-    """
-    if self.is_potential:
-      return lambda x: self.apply({"params": params}, x)
-
-    assert other_potential_value_fn is not None, \
-      "The value of the gradient-based potential depends " \
-      "on the value of the other potential."
-
-    def value_fn(x: jnp.ndarray) -> jnp.ndarray:
-      squeeze = x.ndim == 1
-      if squeeze:
-        x = jnp.expand_dims(x, 0)
-      grad_g_x = jax.lax.stop_gradient(self.apply({"params": params}, x))
-      value = -other_potential_value_fn(grad_g_x) + \
-              jax.vmap(jnp.dot)(grad_g_x, x)
-      return value.squeeze(0) if squeeze else value
-
-    return value_fn
-
-  def potential_gradient_fn(
-      self,
-      params: frozen_dict.FrozenDict[str, jnp.ndarray],
-  ) -> PotentialGradientFn_t:
-    """Return a function returning a vector or the gradient of the potential.
-
-    Args:
-      params: parameters of the module
-
-    Returns:
-      A function that can be evaluated to obtain the potential's gradient
-    """
-    if self.is_potential:
-      return jax.vmap(jax.grad(self.potential_value_fn(params)))
-    return lambda x: self.apply({"params": params}, x)
-
-  def create_train_state(
-      self,
-      rng: jax.Array,
-      optimizer: optax.OptState,
-      input: Union[int, Tuple[int, ...]],
-      **kwargs: Any,
-  ) -> W2NeuralTrainState:
-    """Create initial training state."""
-    params = self.init(rng, jnp.ones(input))["params"]
-
-    return W2NeuralTrainState.create(
-        apply_fn=self.apply,
-        params=params,
-        tx=optimizer,
-        potential_value_fn=self.potential_value_fn,
-        potential_gradient_fn=self.potential_gradient_fn,
-        **kwargs,
-    )
+Callback_t = Callable[[int, dual_potentials.DualPotentials], None]
 
 
 class W2NeuralDual:
   r"""Solver for the Wasserstein-2 Kantorovich dual between Euclidean spaces.
 
   Learn the Wasserstein-2 optimal transport between two measures
   :math:`\alpha` and :math:`\beta` in :math:`n`-dimensional Euclidean space,
   denoted source and target, respectively. This is achieved by parameterizing
   a Kantorovich potential :math:`f_\theta: \mathbb{R}^n\rightarrow\mathbb{R}`
   associated with the :math:`\alpha` measure with an
-  :class:`~ott.neural.models.ICNN` or :class:`~ott.neural.models.MLP`, where
+  :class:`~ott.neural.networks.icnn.ICNN` or a
+  :class:`~ott.neural.networks.potentials.PotentialMLP`, where
   :math:`\nabla f` transports source to target cells. This potential is learned
   by optimizing the dual form associated with the negative inner product cost
 
   .. math::
 
     \text{argsup}_{\theta}\; -\mathbb{E}_{x\sim\alpha}[f_\theta(x)] -
     \mathbb{E}_{y\sim\beta}[f^\star_\theta(y)],
@@ -182,27 +61,27 @@
   where :math:`f^\star(y) := -\inf_{x\in\mathbb{R}^n} f(x)-\langle x, y\rangle`
   is the convex conjugate.
   :math:`\nabla f^\star` transports from the target
   to source cells and provides the inverse optimal
   transport map from :math:`\beta` to :math:`\alpha`.
   This solver estimates the conjugate :math:`f^\star`
   with a neural approximation :math:`g` that is fine-tuned
-  with :class:`~ott.neural.solvers.conjugate.FenchelConjugateSolver`,
+  with :class:`~ott.neural.networks.layers.conjugate.FenchelConjugateSolver`,
   which is a combination further described in :cite:`amos:23`.
 
-  The :class:`~ott.neural.solvers.neuraldual.BaseW2NeuralDual` potentials for
+  The :class:`~ott.neural.networks.potentials.BasePotential` potentials for
   ``neural_f`` and ``neural_g`` can
 
   1. both provide the values of the potentials :math:`f` and :math:`g`, or
   2. one of them can provide the gradient mapping e.g., :math:`\nabla f`
      or :math:`\nabla g` where the potential's value can be obtained
      via the Fenchel conjugate as discussed in :cite:`amos:23`.
 
   The potential's value or gradient mapping is specified via
-  :attr:`~ott.neural.solvers.neuraldual.BaseW2NeuralDual.is_potential`.
+  :attr:`~ott.neural.networks.potentials.BasePotential.is_potential`.
 
   Args:
     dim_data: input dimensionality of data required for network init
     neural_f: network architecture for potential :math:`f`.
     neural_g: network architecture for the conjugate potential
       :math:`g\approx f^\star`
     optimizer_f: optimizer function for potential :math:`f`
@@ -224,16 +103,16 @@
       `'regression'` :cite:`amos:23`.
     parallel_updates: Update :math:`f` and :math:`g` at the same time
   """
 
   def __init__(
       self,
       dim_data: int,
-      neural_f: Optional[BaseW2NeuralDual] = None,
-      neural_g: Optional[BaseW2NeuralDual] = None,
+      neural_f: Optional[potentials.BasePotential] = None,
+      neural_g: Optional[potentials.BasePotential] = None,
       optimizer_f: Optional[optax.OptState] = None,
       optimizer_g: Optional[optax.OptState] = None,
       num_train_iters: int = 20000,
       num_inner_iters: int = 1,
       back_and_forth: Optional[bool] = None,
       valid_freq: int = 1000,
       log_freq: int = 1000,
@@ -262,17 +141,17 @@
     if optimizer_f is None:
       optimizer_f = optax.adam(learning_rate=0.0001, b1=0.5, b2=0.9, eps=1e-8)
     if optimizer_g is None:
       optimizer_g = optax.adam(learning_rate=0.0001, b1=0.5, b2=0.9, eps=1e-8)
 
     # set default neural architectures
     if neural_f is None:
-      neural_f = models.ICNN(dim_data=dim_data, dim_hidden=[64, 64, 64, 64])
+      neural_f = icnn.ICNN(dim_data=dim_data, dim_hidden=[64, 64, 64, 64])
     if neural_g is None:
-      neural_g = models.ICNN(dim_data=dim_data, dim_hidden=[64, 64, 64, 64])
+      neural_g = icnn.ICNN(dim_data=dim_data, dim_hidden=[64, 64, 64, 64])
     self.neural_f = neural_f
     self.neural_g = neural_g
 
     # set optimizer and networks
     self.setup(
         utils.default_prng_key(rng),
         neural_f,
@@ -281,37 +160,37 @@
         optimizer_f,
         optimizer_g,
     )
 
   def setup(
       self,
       rng: jax.Array,
-      neural_f: BaseW2NeuralDual,
-      neural_g: BaseW2NeuralDual,
+      neural_f: potentials.BasePotential,
+      neural_g: potentials.BasePotential,
       dim_data: int,
       optimizer_f: optax.OptState,
       optimizer_g: optax.OptState,
   ) -> None:
     """Setup all components required to train the network."""
     # split random number generator
     rng, rng_f, rng_g = jax.random.split(rng, 3)
 
     # check setting of network architectures
     warn_str = f"Setting of ICNN and the positive weights setting of the " \
         f"`W2NeuralDual` are not consistent. Proceeding with " \
         f"the `W2NeuralDual` setting, with positive weights " \
         f"being {self.pos_weights}."
     if isinstance(
-        neural_f, models.ICNN
+        neural_f, icnn.ICNN
     ) and neural_f.pos_weights is not self.pos_weights:
       warnings.warn(warn_str, stacklevel=2)
       neural_f.pos_weights = self.pos_weights
 
     if isinstance(
-        neural_g, models.ICNN
+        neural_g, icnn.ICNN
     ) and neural_g.pos_weights is not self.pos_weights:
       warnings.warn(warn_str, stacklevel=2)
       neural_g.pos_weights = self.pos_weights
 
     self.state_f = neural_f.create_train_state(
         rng_f,
         optimizer_f,
@@ -321,15 +200,15 @@
         rng_g,
         optimizer_g,
         (1, dim_data),
     )
 
     # default to using back_and_forth with the non-convex models
     if self.back_and_forth is None:
-      self.back_and_forth = isinstance(neural_f, models.MLP)
+      self.back_and_forth = isinstance(neural_f, potentials.PotentialMLP)
 
     if self.num_inner_iters == 1 and self.parallel_updates:
       self.train_step_parallel = self.get_step_fn(
           train=True, to_optimize="both"
       )
       self.valid_step_parallel = self.get_step_fn(
           train=False, to_optimize="both"
@@ -355,16 +234,16 @@
   def __call__(  # noqa: D102
       self,
       trainloader_source: Iterator[jnp.ndarray],
       trainloader_target: Iterator[jnp.ndarray],
       validloader_source: Iterator[jnp.ndarray],
       validloader_target: Iterator[jnp.ndarray],
       callback: Optional[Callback_t] = None,
-  ) -> Union[potentials.DualPotentials, Tuple[potentials.DualPotentials,
-                                              Train_t]]:
+  ) -> Union[dual_potentials.DualPotentials,
+             Tuple[dual_potentials.DualPotentials, Train_t]]:
     logs = self.train_fn(
         trainloader_source,
         trainloader_target,
         validloader_source,
         validloader_target,
         callback=callback,
     )
@@ -585,15 +464,15 @@
         # the potentials reversed with the back_and_forth.
         loss += self.beta * self._penalize_weights_icnn(params_f) + \
             self.beta * self._penalize_weights_icnn(params_g)
 
       # compute Wasserstein-2 distance
       C = jnp.mean(jnp.sum(source ** 2, axis=-1)) + \
           jnp.mean(jnp.sum(target ** 2, axis=-1))
-      W2_dist = C - 2. * (f_source.mean() + f_star_target.mean())
+      W2_dist = C - 2.0 * (f_source.mean() + f_star_target.mean())
 
       return loss, (dual_loss, amor_loss, W2_dist)
 
     @jax.jit
     def step_fn(state_f, state_g, batch):
       """Step function of either training or validation."""
       grad_fn = jax.value_and_grad(loss_fn, argnums=[0, 1], has_aux=True)
@@ -639,15 +518,15 @@
         return loss_g, W2_dist
       raise ValueError("Optimization target has been misspecified.")
 
     return step_fn
 
   def to_dual_potentials(
       self, finetune_g: bool = True
-  ) -> potentials.DualPotentials:
+  ) -> dual_potentials.DualPotentials:
     r"""Return the Kantorovich dual potentials from the trained potentials.
 
     Args:
       finetune_g: Run the conjugate solver to fine-tune the prediction.
 
     Returns:
       A dual potential object
@@ -660,15 +539,15 @@
     def g_value_finetuned(y: jnp.ndarray) -> jnp.ndarray:
       x_hat = jax.grad(g_value_prediction)(y)
       grad_g_y = jax.lax.stop_gradient(
           self.conjugate_solver.solve(f_value, y, x_init=x_hat).grad
       )
       return -f_value(grad_g_y) + jnp.dot(grad_g_y, y)
 
-    return potentials.DualPotentials(
+    return dual_potentials.DualPotentials(
         f=f_value,
         g=g_value_prediction if not finetune_g or self.conjugate_solver is None
         else g_value_finetuned,
         cost_fn=costs.SqEuclidean(),
         corr=True
     )
```

### Comparing `ott-jax-0.4.5/src/ott/problems/__init__.py` & `ott_jax-0.4.6/src/ott/neural/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 #   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from . import linear, quadratic
+from . import datasets, methods, networks
```

### Comparing `ott-jax-0.4.5/src/ott/problems/linear/__init__.py` & `ott_jax-0.4.6/src/ott/problems/linear/__init__.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.5/src/ott/problems/linear/barycenter_problem.py` & `ott_jax-0.4.6/src/ott/problems/linear/barycenter_problem.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.5/src/ott/problems/linear/linear_problem.py` & `ott_jax-0.4.6/src/ott/problems/linear/linear_problem.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.5/src/ott/problems/quadratic/__init__.py` & `ott_jax-0.4.6/src/ott/problems/quadratic/__init__.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.5/src/ott/problems/quadratic/gw_barycenter.py` & `ott_jax-0.4.6/src/ott/problems/quadratic/gw_barycenter.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
     @functools.partial(jax.vmap, in_axes=[0, 0, 0, None])
     def project(
         y: jnp.ndarray,
         b: jnp.ndarray,
         transport: jnp.ndarray,
         fn: Optional[quadratic_costs.Loss],
     ) -> jnp.ndarray:
-      geom = self._create_y_geometry(y, mask=b > 0.)
+      geom = self._create_y_geometry(y, mask=b > 0.0)
       fn, lin = (None, True) if fn is None else (fn.func, fn.is_linear)
 
       tmp = geom.apply_cost(
           transport.T,
           axis=0,
           fn=fn,
           is_linear=lin,
@@ -236,16 +236,16 @@
       self,
       state: "GWBarycenterState",  # noqa: F821
       y: jnp.ndarray,
       b: jnp.ndarray,
       f: Optional[jnp.ndarray] = None
   ) -> quadratic_problem.QuadraticProblem:
     # TODO(michalk8): in future, mask in the problem for convenience?
-    bary_mask = state.a > 0.
-    y_mask = b > 0.
+    bary_mask = state.a > 0.0
+    y_mask = b > 0.0
 
     geom_xx = self._create_bary_geometry(state.cost, mask=bary_mask)
     geom_yy = self._create_y_geometry(y, mask=y_mask)
     if self.is_fused:
       assert f is not None
       assert state.x.shape[1] == f.shape[1]
       geom_xy = self._create_fused_geometry(
```

### Comparing `ott-jax-0.4.5/src/ott/problems/quadratic/quadratic_costs.py` & `ott_jax-0.4.6/src/ott/problems/quadratic/quadratic_costs.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.5/src/ott/problems/quadratic/quadratic_problem.py` & `ott_jax-0.4.6/src/ott/problems/quadratic/quadratic_problem.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from typing import TYPE_CHECKING, Literal, Optional, Tuple, Union
 
 import jax
 import jax.numpy as jnp
 import jax.scipy as jsp
 
 from ott import utils
-from ott.geometry import epsilon_scheduler, geometry, low_rank, pointcloud
+from ott.geometry import geometry, low_rank, pointcloud
 from ott.problems.linear import linear_problem
 from ott.problems.quadratic import quadratic_costs
 from ott.types import Transport
 
 if TYPE_CHECKING:
   from ott.solvers.linear import sinkhorn_lr
 
@@ -47,23 +47,18 @@
     geom_xx: Ground geometry of the first space.
     geom_yy: Ground geometry of the second space.
     geom_xy: Geometry defining the linear penalty term for
       fused Gromov-Wasserstein :cite:`vayer:19`. If :obj:`None`, the problem
       reduces to a plain Gromov-Wasserstein problem :cite:`peyre:16`.
     fused_penalty: Multiplier of the linear term in fused Gromov-Wasserstein,
       i.e. ``problem = purely quadratic + fused_penalty * linear problem``.
-    scale_cost: option to rescale the cost matrices:
-
-      - if :obj:`True`, use the default for each geometry.
-      - if :obj:`False`, keep the original scaling in geometries.
-      - if :class:`str`, use a specific method available in
-        :class:`~ott.geometry.geometry.Geometry` or
-        :class:`~ott.geometry.pointcloud.PointCloud`.
-      - if :obj:`None`, do not scale the cost matrices.
-
+    scale_cost: How to rescale the cost matrices. If a :class:`str`,
+      use specific options available in :class:`~ott.geometry.geometry.Geometry`
+      or :class:`~ott.geometry.pointcloud.PointCloud`. If :obj:`None`, keep
+      the original scaling.
     a: The first marginal. If :obj:`None`, it will be uniform.
     b: The second marginal. If :obj:`None`, it will be uniform.
     loss: Gromov-Wasserstein loss function, see
       :class:`~ott.problems.quadratic.quadratic_costs.GWLoss` for more
       information.
     tau_a: If :math:`< 1.0`, defines how much unbalanced the problem is on
       the first marginal.
@@ -86,29 +81,33 @@
 
   def __init__(
       self,
       geom_xx: geometry.Geometry,
       geom_yy: geometry.Geometry,
       geom_xy: Optional[geometry.Geometry] = None,
       fused_penalty: float = 1.0,
-      scale_cost: Optional[Union[bool, float, str]] = False,
+      scale_cost: Optional[Union[float, str]] = None,
       a: Optional[jnp.ndarray] = None,
       b: Optional[jnp.ndarray] = None,
       loss: Union[Literal["sqeucl", "kl"], quadratic_costs.GWLoss] = "sqeucl",
       tau_a: float = 1.0,
       tau_b: float = 1.0,
       gw_unbalanced_correction: bool = True,
       ranks: Union[int, Tuple[int, ...]] = -1,
       tolerances: Union[float, Tuple[float, ...]] = 1e-2,
   ):
-    self._geom_xx = geom_xx.set_scale_cost(scale_cost)
-    self._geom_yy = geom_yy.set_scale_cost(scale_cost)
-    self._geom_xy = (
-        None if geom_xy is None else geom_xy.set_scale_cost(scale_cost)
-    )
+    if scale_cost is not None:
+      geom_xx = geom_xx.set_scale_cost(scale_cost)
+      geom_yy = geom_yy.set_scale_cost(scale_cost)
+      if geom_xy is not None:
+        geom_xy = geom_xy.set_scale_cost(scale_cost)
+
+    self._geom_xx = geom_xx
+    self._geom_yy = geom_yy
+    self._geom_xy = geom_xy
     self.fused_penalty = fused_penalty
     self.scale_cost = scale_cost
     self._a = a
     self._b = b
     self.tau_a = tau_a
     self.tau_b = tau_b
     self.gw_unbalanced_correction = gw_unbalanced_correction
@@ -168,15 +167,15 @@
     return low_rank.LRCGeometry(cost_1=x_term, cost_2=y_term)
 
   def cost_unbalanced_correction(
       self,
       transport_matrix: jnp.ndarray,
       marginal_1: jnp.ndarray,
       marginal_2: jnp.ndarray,
-      epsilon: epsilon_scheduler.Epsilon,
+      epsilon: float,
   ) -> float:
     r"""Calculate cost term from the quadratic divergence when unbalanced.
 
     In the unbalanced setting (``tau_a < 1.0 or tau_b < 1.0``), the
     introduction of a quadratic divergence :cite:`sejourne:21` adds a term
     to the GW local cost.
 
@@ -201,21 +200,20 @@
       epsilon: entropy regularizer.
 
     Returns:
       The cost term.
     """
 
     def regularizer(tau: float) -> float:
-      return eps * tau / (1.0 - tau)
+      return epsilon * tau / (1.0 - tau)
 
-    eps = epsilon._target_init
     marginal_1loga = jsp.special.xlogy(marginal_1, self.a).sum()
     marginal_2logb = jsp.special.xlogy(marginal_2, self.b).sum()
 
-    cost = eps * jsp.special.xlogy(transport_matrix, transport_matrix).sum()
+    cost = epsilon * jsp.special.xlogy(transport_matrix, transport_matrix).sum()
     if self.tau_a != 1.0:
       cost += regularizer(
           self.tau_a
       ) * (-jsp.special.entr(marginal_1).sum() - marginal_1loga)
     if self.tau_b != 1.0:
       cost += regularizer(
           self.tau_b
@@ -266,15 +264,15 @@
           cost_matrix=cost_matrix, relative_epsilon=relative_epsilon
       )
     return geom  # noqa: RET504
 
   def update_linearization(
       self,
       transport: Transport,
-      epsilon: Optional[Union[epsilon_scheduler.Epsilon, float]] = None,
+      epsilon: Optional[float] = None,
       old_transport_mass: float = 1.0,
       relative_epsilon: Optional[bool] = None,
   ) -> linear_problem.LinearProblem:
     """Update linearization of GW problem by updating cost matrix.
 
     If the problem is balanced (``tau_a = 1.0 and tau_b = 1.0``), the equation
     follows eq. 6, p. 1 of :cite:`peyre:16`.
@@ -307,34 +305,32 @@
     marginal_1 = transport.marginal(axis=1) * rescale_factor
     marginal_2 = transport.marginal(axis=0) * rescale_factor
     marginal_cost = self.marginal_dependent_cost(marginal_1, marginal_2)
 
     transport_matrix = transport.matrix * rescale_factor
 
     if not self.is_balanced:
-      # Rescales transport for Unbalanced GW according to Sejourne et al. (2021)
-      transport_mass = jax.lax.stop_gradient(marginal_1.sum())
-      epsilon = update_epsilon_unbalanced(epsilon, transport_mass)
+      epsilon *= jax.lax.stop_gradient(marginal_1.sum())
       unbalanced_correction = self.cost_unbalanced_correction(
-          transport_matrix, marginal_1, marginal_2, epsilon
+          transport_matrix, marginal_1, marginal_2, epsilon=epsilon
       )
 
     h1, h2 = self.quad_loss
     geom_xx, geom_yy = self.geom_xx, self.geom_yy
 
     tmp = apply_cost(geom_xx, transport_matrix, axis=1, fn=h1)
     tmp = apply_cost(geom_yy, tmp.T, axis=1, fn=h2).T
 
     cost_matrix = marginal_cost.cost_matrix - tmp + unbalanced_correction
     cost_matrix += self.fused_penalty * rescale_factor * self._fused_cost_matrix
 
     geom = geometry.Geometry(
         cost_matrix=cost_matrix,
         epsilon=epsilon,
-        relative_epsilon=relative_epsilon
+        relative_epsilon=relative_epsilon,
     )
 
     return linear_problem.LinearProblem(
         geom, self.a, self.b, tau_a=self.tau_a, tau_b=self.tau_b
     )
 
   def update_lr_linearization(
@@ -497,20 +493,12 @@
 
   @classmethod
   def tree_unflatten(cls, aux_data, children):  # noqa: D102
     geoms, (a, b) = children[:3], children[3:]
     return cls(*geoms, a=a, b=b, **aux_data)
 
 
-def update_epsilon_unbalanced(  # noqa: D103
-    epsilon: Union[float, epsilon_scheduler.Epsilon], transport_mass: float
-) -> epsilon_scheduler.Epsilon:
-  if not isinstance(epsilon, epsilon_scheduler.Epsilon):
-    epsilon = epsilon_scheduler.Epsilon(epsilon, scale_epsilon=1.0)
-  return epsilon.set(scale_epsilon=epsilon._scale_epsilon * transport_mass)
-
-
 def apply_cost(  # noqa: D103
     geom: geometry.Geometry, arr: jnp.ndarray, *, axis: int,
     fn: quadratic_costs.Loss
 ) -> jnp.ndarray:
   return geom.apply_cost(arr, axis=axis, fn=fn.func, is_linear=fn.is_linear)
```

### Comparing `ott-jax-0.4.5/src/ott/solvers/__init__.py` & `ott_jax-0.4.6/src/ott/solvers/quadratic/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,8 +7,14 @@
 #   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from . import linear, quadratic, was_solver
+from . import (
+    gromov_wasserstein,
+    gromov_wasserstein_lr,
+    gw_barycenter,
+    lower_bound,
+)
+from ._solve import solve
```

### Comparing `ott-jax-0.4.5/src/ott/solvers/linear/__init__.py` & `ott_jax-0.4.6/src/ott/solvers/linear/__init__.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.5/src/ott/solvers/linear/_solve.py` & `ott_jax-0.4.6/src/ott/solvers/linear/_solve.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.5/src/ott/solvers/linear/acceleration.py` & `ott_jax-0.4.6/src/ott/solvers/linear/acceleration.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     )
 
     # If update was triggered, ensure a scaling is returned, since the result
     # from the extrapolation was outputted in potential form.
     fu = jnp.where(
         trigger_update, fu if lse_mode else geom.scaling_from_potential(fu), fu
     )
-    return state.set(fu=fu, old_fus=old_fus)
+    return state.set(potentials=(fu, state.gv), old_fus=old_fus)
 
   def init_maps(
       self, pb, state: "sinkhorn.SinkhornState"
   ) -> "sinkhorn.SinkhornState":
     """Initialize log matrix used in Anderson acceleration with *NaN* values."""
     fus = jnp.ones((pb.geom.shape[0], self.memory)) * jnp.nan
     return state.set(old_fus=fus, old_mapped_fus=fus)
```

### Comparing `ott-jax-0.4.5/src/ott/solvers/linear/continuous_barycenter.py` & `ott_jax-0.4.6/src/ott/solvers/linear/continuous_barycenter.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,16 +73,16 @@
         a: Optional[jnp.ndarray], x: jnp.ndarray, b: jnp.ndarray, y: jnp.ndarray
     ):
       out = linear_ot_solver(
           linear_problem.LinearProblem(
               pointcloud.PointCloud(
                   x,
                   y,
-                  src_mask=a > 0.,
-                  tgt_mask=b > 0.,
+                  src_mask=a > 0.0,
+                  tgt_mask=b > 0.0,
                   cost_fn=bar_prob.cost_fn,
                   epsilon=bar_prob.epsilon
               ), a, b
           )
       )
       return (
           out.reg_ot_cost, out.converged, out.matrix,
```

### Comparing `ott-jax-0.4.5/src/ott/solvers/linear/discrete_barycenter.py` & `ott_jax-0.4.6/src/ott/solvers/linear/discrete_barycenter.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.5/src/ott/solvers/linear/implicit_differentiation.py` & `ott_jax-0.4.6/src/ott/solvers/linear/implicit_differentiation.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.5/src/ott/solvers/linear/lineax_implicit.py` & `ott_jax-0.4.6/src/ott/solvers/linear/lineax_implicit.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,19 +10,20 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Any, Callable, Optional, TypeVar
 
 import equinox as eqx
+import lineax as lx
+from jaxtyping import Array, Float, PyTree
+
 import jax
 import jax.numpy as jnp
 import jax.tree_util as jtu
-import lineax as lx
-from jaxtyping import Array, Float, PyTree
 
 _T = TypeVar("_T")
 _FlatPyTree = tuple[list[_T], jtu.PyTreeDef]
 
 __all__ = ["CustomTransposeLinearOperator", "solve_lineax"]
```

### Comparing `ott-jax-0.4.5/src/ott/solvers/linear/lr_utils.py` & `ott_jax-0.4.6/src/ott/solvers/linear/lr_utils.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.5/src/ott/solvers/linear/sinkhorn.py` & `ott_jax-0.4.6/src/ott/solvers/linear/sinkhorn.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,57 +8,51 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import (
-    TYPE_CHECKING,
     Any,
     Callable,
     Literal,
     Mapping,
     NamedTuple,
     Optional,
     Sequence,
     Tuple,
     Union,
 )
 
 import jax
-import jax.experimental
 import jax.numpy as jnp
 import jax.scipy as jsp
 import numpy as np
 
 from ott import utils
 from ott.geometry import geometry
 from ott.initializers.linear import initializers as init_lib
 from ott.math import fixed_point_loop
 from ott.math import unbalanced_functions as uf
 from ott.math import utils as mu
 from ott.problems.linear import linear_problem, potentials
 from ott.solvers.linear import acceleration
 from ott.solvers.linear import implicit_differentiation as implicit_lib
 
-if TYPE_CHECKING:
-  from ott.solvers.linear.sinkhorn_lr import LRSinkhornOutput
-
-__all__ = ["Sinkhorn", "SinkhornOutput", "solve"]
+__all__ = ["Sinkhorn", "SinkhornOutput"]
 
 ProgressCallbackFn_t = Callable[
     [Tuple[np.ndarray, np.ndarray, np.ndarray, "SinkhornState"]], None]
 
 
 class SinkhornState(NamedTuple):
   """Holds the state variables used to solve OT with Sinkhorn."""
 
+  potentials: Tuple[jnp.ndarray, ...]
   errors: Optional[jnp.ndarray] = None
-  fu: Optional[jnp.ndarray] = None
-  gv: Optional[jnp.ndarray] = None
   old_fus: Optional[jnp.ndarray] = None
   old_mapped_fus: Optional[jnp.ndarray] = None
 
   def set(self, **kwargs: Any) -> "SinkhornState":
     """Return a copy of self, with potential overwrites."""
     return self._replace(**kwargs)
 
@@ -109,31 +103,41 @@
 
     Returns:
       The centered potentials.
     """
     if ot_prob.is_balanced:
       # center the potentials for numerical stability
       is_finite = jnp.isfinite(f)
-      shift = jnp.sum(jnp.where(is_finite, f, 0.)) / jnp.sum(is_finite)
+      shift = jnp.sum(jnp.where(is_finite, f, 0.0)) / jnp.sum(is_finite)
       return f - shift, g + shift
 
-    if ot_prob.tau_a == 1. or ot_prob.tau_b == 1.:
+    if ot_prob.tau_a == 1.0 or ot_prob.tau_b == 1.0:
       # re-centering wasn't done during the lse-step, ignore
       return f, g
 
     rho_a = uf.rho(ot_prob.epsilon, ot_prob.tau_a)
     rho_b = uf.rho(ot_prob.epsilon, ot_prob.tau_b)
     tau = rho_a * rho_b / (rho_a + rho_b)
 
     shift = tau * (
         mu.logsumexp(-f / rho_a, b=ot_prob.a) -
         mu.logsumexp(-g / rho_b, b=ot_prob.b)
     )
     return f + shift, g - shift
 
+  @property
+  def fu(self) -> jnp.ndarray:
+    """The first dual potential or scaling."""
+    return self.potentials[0]
+
+  @property
+  def gv(self) -> jnp.ndarray:
+    """The second dual potential or scaling."""
+    return self.potentials[1]
+
 
 def solution_error(
     f_u: jnp.ndarray,
     g_v: jnp.ndarray,
     ot_prob: linear_problem.LinearProblem,
     *,
     norm_error: Sequence[int],
@@ -316,16 +320,15 @@
       algorithm.
     converged: whether the output corresponds to a solution whose error is
       below the convergence threshold.
     inner_iterations: number of iterations that were run between two
       computations of errors.
   """
 
-  f: Optional[jnp.ndarray] = None
-  g: Optional[jnp.ndarray] = None
+  potentials: Tuple[jnp.ndarray, ...]
   errors: Optional[jnp.ndarray] = None
   reg_ot_cost: Optional[float] = None
   ot_prob: Optional[linear_problem.LinearProblem] = None
   threshold: Optional[jnp.ndarray] = None
   converged: Optional[bool] = None
   inner_iterations: Optional[int] = None
 
@@ -485,14 +488,24 @@
         self.geom.epsilon * jnp.sum(jax.scipy.special.entr(self.matrix))
     )
 
   def to_dual_potentials(self) -> potentials.EntropicPotentials:
     """Return the entropic map estimator."""
     return potentials.EntropicPotentials(self.f, self.g, self.ot_prob)
 
+  @property
+  def f(self) -> jnp.ndarray:
+    """The first dual potential."""
+    return self.potentials[0]
+
+  @property
+  def g(self) -> jnp.ndarray:
+    """The second dual potential."""
+    return self.potentials[1]
+
 
 @jax.tree_util.register_pytree_node_class
 class Sinkhorn:
   r"""Sinkhorn solver.
 
   The Sinkhorn algorithm is a fixed point iteration that solves a regularized
   optimal transport (reg-OT) problem between two measures.
@@ -872,25 +885,25 @@
     def k(tau_i: float, tau_j: float) -> float:
       num = -tau_j * (tau_a - 1) * (tau_b - 1) * (tau_i - 1)
       denom = (tau_j - 1) * (tau_a * (tau_b - 1) + tau_b * (tau_a - 1))
       return num / denom
 
     def xi(tau_i: float, tau_j: float) -> float:
       k_ij = k(tau_i, tau_j)
-      return k_ij / (1. - k_ij)
+      return k_ij / (1.0 - k_ij)
 
     def smin(
         potential: jnp.ndarray, marginal: jnp.ndarray, tau: float
     ) -> float:
       rho = uf.rho(ot_prob.epsilon, tau)
       return -rho * mu.logsumexp(-potential / rho, b=marginal)
 
     # only for an unbalanced problems with `tau_{a,b} < 1`
     recenter = (
-        self.recenter_potentials and ot_prob.tau_a < 1. and ot_prob.tau_b < 1.
+        self.recenter_potentials and ot_prob.tau_a < 1.0 and ot_prob.tau_b < 1.0
     )
     w = self.momentum.weight(state, iteration)
     tau_a, tau_b = ot_prob.tau_a, ot_prob.tau_b
     old_fu, old_gv = state.fu, state.gv
 
     if recenter:
       k11, k22 = k(tau_a, tau_a), k(tau_b, tau_b)
@@ -913,15 +926,15 @@
         old_fu, old_gv, jnp.log(ot_prob.a), iteration, axis=1
     )
     if recenter:
       new_fu -= k11 * smin(old_gv, ot_prob.b, tau_b)
       new_fu += xi12 * smin(new_fu, ot_prob.a, tau_a)
     fu = self.momentum(w, old_fu, new_fu, self.lse_mode)
 
-    return state.set(fu=fu, gv=gv)
+    return state.set(potentials=(fu, gv))
 
   def kernel_step(
       self, ot_prob: linear_problem.LinearProblem, state: SinkhornState,
       iteration: int
   ) -> SinkhornState:
     """Sinkhorn multiplicative update."""
     w = self.momentum.weight(state, iteration)
@@ -933,15 +946,15 @@
     new_fu = ot_prob.geom.update_scaling(
         old_gv if self.parallel_dual_updates else gv,
         ot_prob.a,
         iteration,
         axis=1
     ) ** ot_prob.tau_a
     fu = self.momentum(w, state.fu, new_fu, self.lse_mode)
-    return state.set(fu=fu, gv=gv)
+    return state.set(potentials=(fu, gv))
 
   def one_iteration(
       self, ot_prob: linear_problem.LinearProblem, state: SinkhornState,
       iteration: int, compute_error: bool
   ) -> SinkhornState:
     """Carries out one Sinkhorn iteration.
 
@@ -990,16 +1003,16 @@
         state,
         ot_prob,
     )
     errors = state.errors.at[iteration // self.inner_iterations, :].set(err)
     state = state.set(errors=errors)
 
     if self.progress_fn is not None:
-      jax.experimental.io_callback(
-          self.progress_fn, None,
+      jax.debug.callback(
+          self.progress_fn,
           (iteration, self.inner_iterations, self.max_iterations, state)
       )
     return state
 
   def _converged(self, state: SinkhornState, iteration: int) -> bool:
     err = state.errors[iteration // self.inner_iterations - 1, 0]
     return jnp.logical_and(iteration > 0, err < self.threshold)
@@ -1025,18 +1038,16 @@
     return np.ceil(self.max_iterations / self.inner_iterations).astype(int)
 
   def init_state(
       self, ot_prob: linear_problem.LinearProblem, init: Tuple[jnp.ndarray,
                                                                jnp.ndarray]
   ) -> SinkhornState:
     """Return the initial state of the loop."""
-    fu, gv = init
-    errors = -jnp.ones((self.outer_iterations, len(self.norm_error)),
-                       dtype=fu.dtype)
-    state = SinkhornState(errors=errors, fu=fu, gv=gv)
+    errors = -jnp.ones((self.outer_iterations, len(self.norm_error)))
+    state = SinkhornState(init, errors=errors)
     return self.anderson.init_maps(ot_prob, state) if self.anderson else state
 
   def output_from_state(
       self, ot_prob: linear_problem.LinearProblem, state: SinkhornState
   ) -> SinkhornOutput:
     """Create an output from a loop state.
 
@@ -1082,22 +1093,19 @@
     # position) is lower than the threshold.
 
     converged = jnp.logical_and(
         jnp.logical_not(jnp.any(jnp.isnan(state.errors))), state.errors[-1]
         < self.threshold
     )[0]
 
-    return SinkhornOutput(
-        f=f,
-        g=g,
-        errors=state.errors[:, 0],
-        threshold=jnp.array(self.threshold),
-        converged=converged,
-        inner_iterations=self.inner_iterations
-    )
+    return SinkhornOutput((f, g),
+                          errors=state.errors[:, 0],
+                          threshold=jnp.array(self.threshold),
+                          converged=converged,
+                          inner_iterations=self.inner_iterations)
 
   @property
   def norm_error(self) -> Tuple[int, ...]:
     """Powers used to compute the p-norm between marginal/target."""
     # To change momentum adaptively, one needs errors in ||.||_1 norm.
     # In that case, we add this exponent to the list of errors to compute,
     # notably if that was not the error requested by the user.
@@ -1188,49 +1196,32 @@
 ) -> Tuple[SinkhornOutput, Tuple[jnp.ndarray, jnp.ndarray,
                                  linear_problem.LinearProblem, Sinkhorn]]:
   """Run forward pass of the Sinkhorn algorithm storing side information."""
   state = iterations(ot_prob, solver, init)
   return state, (state.f, state.g, ot_prob, solver)
 
 
-def _iterations_implicit_bwd(res, gr):
+def _iterations_implicit_bwd(res, gr: SinkhornOutput):
   """Run Sinkhorn in backward mode, using implicit differentiation.
 
   Args:
     res: residual data sent from fwd pass, used for computations below. In this
       case consists in the output itself, as well as inputs against which we
       wish to differentiate.
     gr: gradients w.r.t outputs of fwd pass, here w.r.t size f, g, errors. Note
       that differentiability w.r.t. errors is not handled, and only f, g is
       considered.
 
   Returns:
     a tuple of gradients: PyTree for geom, one jnp.ndarray for each of a and b.
   """
   f, g, ot_prob, solver = res
-  gr = gr[:2]
-  return (
-      *solver.implicit_diff.gradient(ot_prob, f, g, solver.lse_mode, gr), None,
-      None
+  out = solver.implicit_diff.gradient(
+      ot_prob, f, g, solver.lse_mode, gr.potentials
   )
+  return *out, None, None
 
 
 # sets threshold, norm_errors, geom, a and b to be differentiable, as those are
 # non-static. Only differentiability w.r.t. geom, a and b will be used.
 _iterations_implicit = jax.custom_vjp(iterations)
 _iterations_implicit.defvjp(_iterations_taped, _iterations_implicit_bwd)
-
-
-@utils.deprecate(alt="Please use `ott.solvers.linear.solve()` instead.")
-def solve(*args: Any,
-          **kwargs: Any) -> Union[SinkhornOutput, "LRSinkhornOutput"]:
-  """Solve linear regularized OT problem using Sinkhorn iterations.
-
-  Args:
-    args: Position arguments for :func:`ott.solvers.linear.solve`.
-    kwargs: Keyword arguments for :func:`ott.solvers.linear.solve`.
-
-  Returns:
-    The Sinkhorn output.
-  """
-  from ott.solvers.linear import solve
-  return solve(*args, **kwargs)
```

### Comparing `ott-jax-0.4.5/src/ott/solvers/linear/sinkhorn_lr.py` & `ott_jax-0.4.6/src/ott/solvers/linear/sinkhorn_lr.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,14 @@
     NamedTuple,
     Optional,
     Tuple,
     Union,
 )
 
 import jax
-import jax.experimental
 import jax.numpy as jnp
 import jax.scipy as jsp
 import numpy as np
 
 from ott.geometry import geometry
 from ott.initializers.linear import initializers_lr
 from ott.math import fixed_point_loop
@@ -259,15 +258,15 @@
   @property
   def transport_mass(self) -> float:
     """Sum of transport matrix."""
     return self.marginal(0).sum()
 
   @property
   def _inv_g(self) -> jnp.ndarray:
-    return 1. / self.g
+    return 1.0 / self.g
 
 
 @jax.tree_util.register_pytree_node_class
 class LRSinkhorn(sinkhorn.Sinkhorn):
   r"""Low-Rank Sinkhorn solver for linear reg-OT problems.
 
   The algorithm is described in :cite:`scetbon:21` and the implementation
@@ -303,15 +302,15 @@
     kwargs: Keyword arguments for
       :class:`~ott.solvers.linear.sinkhorn.Sinkhorn`.
   """
 
   def __init__(
       self,
       rank: int,
-      gamma: float = 10.,
+      gamma: float = 10.0,
       gamma_rescale: bool = True,
       epsilon: float = 0.0,
       initializer: Union[Literal["random", "rank2", "k-means",
                                  "generalized-k-means"],
                          initializers_lr.LRInitializer] = "random",
       lse_mode: bool = True,
       inner_iterations: int = 10,
@@ -473,17 +472,17 @@
       h_old = h
 
       # Update couplings
       g_q = _softm(f1, g1_old, c_q, axis=0)
       g_r = _softm(f2, g2_old, c_r, axis=0)
 
       # Second Projection
-      h = (1. / 3.) * (h_old + w_gp + w_q + w_r)
-      h += g_q / (3. * gamma)
-      h += g_r / (3. * gamma)
+      h = (1.0 / 3.0) * (h_old + w_gp + w_q + w_r)
+      h += g_q / (3.0 * gamma)
+      h += g_r / (3.0 * gamma)
       g1 = h + g1_old - g_q / gamma
       g2 = h + g2_old - g_r / gamma
 
       w_q = w_q + g1_old - g1
       w_r = w_r + g2_old - g2
       w_gp = h_old + w_gp - h
 
@@ -699,16 +698,16 @@
     state = state.set(
         costs=state.costs.at[it].set(cost),
         errors=state.errors.at[it].set(error),
         crossed_threshold=crossed_threshold,
     )
 
     if self.progress_fn is not None:
-      jax.experimental.io_callback(
-          self.progress_fn, None,
+      jax.debug.callback(
+          self.progress_fn,
           (iteration, self.inner_iterations, self.max_iterations, state)
       )
 
     return state
 
   @property
   def norm_error(self) -> Tuple[int]:  # noqa: D102
```

### Comparing `ott-jax-0.4.5/src/ott/solvers/linear/univariate.py` & `ott_jax-0.4.6/src/ott/solvers/linear/univariate.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.5/src/ott/solvers/quadratic/__init__.py` & `ott_jax-0.4.6/src/ott/tools/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,13 +8,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from . import (
-    gromov_wasserstein,
-    gromov_wasserstein_lr,
-    gw_barycenter,
-    lower_bound,
+    gaussian_mixture,
+    k_means,
+    plot,
+    segment_sinkhorn,
+    sinkhorn_divergence,
+    soft_sort,
 )
-from ._solve import solve
```

### Comparing `ott-jax-0.4.5/src/ott/solvers/quadratic/_solve.py` & `ott_jax-0.4.6/src/ott/solvers/quadratic/_solve.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.5/src/ott/solvers/quadratic/gromov_wasserstein.py` & `ott_jax-0.4.6/src/ott/solvers/quadratic/gromov_wasserstein.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,14 @@
     Optional,
     Sequence,
     Tuple,
     Union,
 )
 
 import jax
-import jax.experimental
 import jax.numpy as jnp
 import numpy as np
 
 from ott import utils
 from ott.geometry import geometry
 from ott.initializers.quadratic import initializers as quad_initializers
 from ott.math import fixed_point_loop
@@ -401,16 +400,16 @@
     new_state = state.update(
         iteration, out, linear_pb, solver.store_inner_errors, old_transport_mass
     )
 
     # Inner iterations is currently fixed to 1.
     inner_iterations = 1
     if solver.progress_fn is not None:
-      jax.experimental.io_callback(
-          solver.progress_fn, None,
+      jax.debug.callback(
+          solver.progress_fn,
           (iteration, inner_iterations, solver.max_iterations, state)
       )
 
     return new_state
 
   state = fixed_point_loop.fixpoint_iter(
       cond_fn=cond_fn,
```

### Comparing `ott-jax-0.4.5/src/ott/solvers/quadratic/gromov_wasserstein_lr.py` & `ott_jax-0.4.6/src/ott/solvers/quadratic/gromov_wasserstein_lr.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,14 @@
     NamedTuple,
     Optional,
     Tuple,
     Union,
 )
 
 import jax
-import jax.experimental
 import jax.numpy as jnp
 import jax.scipy as jsp
 import numpy as np
 
 from ott import utils
 from ott.geometry import geometry, low_rank
 from ott.initializers.linear import initializers_lr
@@ -274,14 +273,17 @@
       described in :cite:`scetbon:22b`.
     epsilon: Entropic regularization added on top of low-rank problem.
     initializer: How to initialize the :math:`Q`, :math:`R` and :math:`g`
       factors.
     lse_mode: Whether to run computations in LSE or kernel mode.
     inner_iterations: Number of inner iterations used by the algorithm before
       re-evaluating progress.
+    min_iterations: The minimum number of low-rank Sinkhorn iterations carried
+      out before the error is computed and monitored.
+    max_iterations: The maximum number of low-rank Sinkhorn iterations.
     use_danskin: Use Danskin theorem to evaluate gradient of objective w.r.t.
       input parameters. Only `True` handled at this moment.
     implicit_diff: Whether to use implicit differentiation. Currently, only
       ``implicit_diff = False`` is implemented.
     progress_fn: callback function which gets called during the GW
       iterations, so the user can display the error at each iteration,
       e.g., using a progress bar. See :func:`~ott.utils.default_progress_fn`
@@ -301,26 +303,30 @@
       gamma: float = 10.0,
       gamma_rescale: bool = True,
       epsilon: float = 0.0,
       initializer: Union[Literal["random", "rank2", "k-means",
                                  "generalized-k-means"],
                          initializers_lr.LRInitializer] = "random",
       lse_mode: bool = True,
-      inner_iterations: int = 10,
       use_danskin: bool = True,
       implicit_diff: bool = False,
+      inner_iterations: int = 2_000,
+      min_iterations: int = 10_000,
+      max_iterations: int = 100_000,
       kwargs_dys: Optional[Mapping[str, Any]] = None,
       kwargs_init: Optional[Mapping[str, Any]] = None,
       progress_fn: Optional[ProgressCallbackFn_t] = None,
       **kwargs: Any,
   ):
     assert not implicit_diff, "Implicit diff. not yet implemented."
     super().__init__(
         lse_mode=lse_mode,
         inner_iterations=inner_iterations,
+        min_iterations=min_iterations,
+        max_iterations=max_iterations,
         use_danskin=use_danskin,
         implicit_diff=implicit_diff,
         **kwargs
     )
     self.rank = rank
     self.gamma = gamma
     self.gamma_rescale = gamma_rescale
@@ -493,17 +499,17 @@
       h_old = h
 
       # Update couplings
       g_q = _softm(f1, g1_old, c_q, axis=0)
       g_r = _softm(f2, g2_old, c_r, axis=0)
 
       # Second Projection
-      h = (1. / 3.) * (h_old + w_gp + w_q + w_r)
-      h += g_q / (3. * gamma)
-      h += g_r / (3. * gamma)
+      h = (1.0 / 3.0) * (h_old + w_gp + w_q + w_r)
+      h += g_q / (3.0 * gamma)
+      h += g_r / (3.0 * gamma)
       g1 = h + g1_old - g_q / gamma
       g2 = h + g2_old - g_r / gamma
 
       w_q = w_q + g1_old - g1
       w_r = w_r + g2_old - g2
       w_gp = h_old + w_gp - h
 
@@ -723,16 +729,16 @@
     state = state.set(
         costs=state.costs.at[it].set(cost),
         errors=state.errors.at[it].set(error),
         crossed_threshold=crossed_threshold,
     )
 
     if self.progress_fn is not None:
-      jax.experimental.io_callback(
-          self.progress_fn, None,
+      jax.debug.callback(
+          self.progress_fn,
           (iteration, self.inner_iterations, self.max_iterations, state)
       )
 
     return state
 
   @property
   def norm_error(self) -> Tuple[int]:  # noqa: D102
```

### Comparing `ott-jax-0.4.5/src/ott/solvers/quadratic/gw_barycenter.py` & `ott_jax-0.4.6/src/ott/solvers/quadratic/gw_barycenter.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.5/src/ott/solvers/quadratic/lower_bound.py` & `ott_jax-0.4.6/src/ott/solvers/quadratic/lower_bound.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,88 +9,50 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import TYPE_CHECKING, Any, Optional
 
-import jax
-import jax.tree_util as jtu
-
 from ott.geometry import pointcloud
 from ott.problems.quadratic import quadratic_problem
 from ott.solvers import linear
 from ott.solvers.linear import sinkhorn
 
 if TYPE_CHECKING:
   from ott.geometry import distrib_costs
 
-__all__ = ["LowerBoundSolver"]
-
+__all__ = ["third_lower_bound"]
 
-@jtu.register_pytree_node_class
-class LowerBoundSolver:
-  """Lower bound OT solver.
 
-  Computes the third lower bound distance from :cite:`memoli:11`, def. 6.3.
+def third_lower_bound(
+    prob: quadratic_problem.QuadraticProblem,
+    distrib_cost: Optional["distrib_costs.UnivariateWasserstein"] = None,
+    epsilon: Optional[float] = None,
+    **kwargs: Any,
+) -> sinkhorn.SinkhornOutput:
+  """Computes the third lower bound distance from :cite:`memoli:11`, def. 6.3.
 
   Args:
-    epsilon: Entropy regularization for the resulting linear problem.
-    distrib_cost: Univariate Wasserstein cost, used to compare two point clouds
-      in different spaces, where each point is seen as its distribution of costs
-      to other points in its point cloud.
+    prob: Quadratic OT problem.
+    distrib_cost: Univariate Wasserstein cost used to compare two point clouds
+      in different spaces. Each point is seen as its distribution of costs
+      to other points in its respective point cloud.
+    epsilon: Entropy regularization.
+    kwargs: Keyword arguments for :func:`~ott.solvers.linear.solve`.
+
+  Returns:
+    An approximation of the GW coupling that can be used to initialize
+    the solution of the quadratic OT problem.
   """
+  from ott.geometry import distrib_costs
+
+  if distrib_cost is None:
+    distrib_cost = distrib_costs.UnivariateWasserstein()
+
+  dists_xx = prob.geom_xx.cost_matrix
+  dists_yy = prob.geom_yy.cost_matrix
+  geom_xy = pointcloud.PointCloud(
+      dists_xx, dists_yy, cost_fn=distrib_cost, epsilon=epsilon
+  )
 
-  def __init__(
-      self,
-      epsilon: Optional[float] = None,
-      distrib_cost: Optional["distrib_costs.UnivariateWasserstein"] = None,
-  ):
-    from ott.geometry import distrib_costs
-
-    self.epsilon = epsilon
-    self.distrib_cost = (
-        distrib_costs.UnivariateWasserstein()
-        if distrib_cost is None else distrib_cost
-    )
-
-  def __call__(
-      self,
-      prob: quadratic_problem.QuadraticProblem,
-      epsilon: Optional[float] = None,
-      rng: Optional[jax.Array] = None,
-      **kwargs: Any
-  ) -> sinkhorn.SinkhornOutput:
-    """Compute a lower-bound for the GW problem using a simple linearization.
-
-    This solver handles a quadratic problem by computing a proxy ``[n, m]``
-    cost-matrix, injecting it into a linear OT solver to output a first an OT
-    matrix that can be used either to linearize/initialize the resolution
-    ot the GW problem, or more simply as a simple GW solution.
-
-    Args:
-      prob: Quadratic OT problem.
-      epsilon: Entropic regularization passed on to solve the linearization of
-        the quadratic problem using 1D costs.
-      rng: Random key, possibly used when computing 1D costs when using
-        subsampling.
-      kwargs: Keyword arguments for :func:`~ott.solvers.linear.solve`.
-
-    Returns:
-      A linear OT output, an approximation of the OT coupling obtained using
-      the lower bound provided by :cite:`memoli:11`.
-    """
-    dists_xx = prob.geom_xx.cost_matrix
-    dists_yy = prob.geom_yy.cost_matrix
-
-    geom_xy = pointcloud.PointCloud(
-        dists_xx, dists_yy, cost_fn=self.distrib_cost, epsilon=self.epsilon
-    )
-    return linear.solve(geom_xy, **kwargs)
-
-  def tree_flatten(self):  # noqa: D102
-    return (self.epsilon, self.distrib_cost), None
-
-  @classmethod
-  def tree_unflatten(cls, aux_data, children):  # noqa: D102
-    del aux_data
-    return cls(*children)
+  return linear.solve(geom_xy, **kwargs)
```

### Comparing `ott-jax-0.4.5/src/ott/solvers/was_solver.py` & `ott_jax-0.4.6/src/ott/solvers/was_solver.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.5/src/ott/tools/__init__.py` & `ott_jax-0.4.6/src/ott/neural/methods/flows/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,8 @@
 #   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from . import (
-    gaussian_mixture,
-    k_means,
-    plot,
-    segment_sinkhorn,
-    sinkhorn_divergence,
-    soft_sort,
-)
+from . import dynamics, genot, otfm
```

### Comparing `ott-jax-0.4.5/src/ott/tools/gaussian_mixture/__init__.py` & `ott_jax-0.4.6/src/ott/tools/gaussian_mixture/__init__.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.5/src/ott/tools/gaussian_mixture/fit_gmm.py` & `ott_jax-0.4.6/src/ott/tools/gaussian_mixture/fit_gmm.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
     jit: if True, compile functions
     verbose: if True, print the loss at each step
 
   Returns:
     A GMM with updated parameters.
   """
   if point_weights is None:
-    point_weights = jnp.ones(points.shape[:-1], dtype=points.dtype)
+    point_weights = jnp.ones(points.shape[:-1])
   loss_fn = log_prob_loss
   get_q_fn = get_q
   e_step_fn = get_assignment_probs
   m_step_fn = gaussian_mixture.GaussianMixture.from_points_and_assignment_probs
   if jit:
     loss_fn = jax.jit(loss_fn)
     get_q_fn = jax.jit(get_q_fn)
@@ -184,15 +184,15 @@
 # See https://en.wikipedia.org/wiki/K-means%2B%2B for details
 
 
 def _get_dist_sq(points: jnp.ndarray, loc: jnp.ndarray) -> jnp.ndarray:
   """Get the squared distance from each point to each loc."""
 
   def _dist_sq_one_loc(points: jnp.ndarray, loc: jnp.ndarray) -> jnp.ndarray:
-    return jnp.sum((points - loc[None]) ** 2., axis=-1)
+    return jnp.sum((points - loc[None]) ** 2, axis=-1)
 
   dist_sq_fn = jax.vmap(_dist_sq_one_loc, in_axes=(None, 0), out_axes=1)
   return dist_sq_fn(points, loc)
 
 
 def _get_locs(
     rng: jax.Array, points: jnp.ndarray, n_components: int
@@ -207,25 +207,25 @@
   Returns:
     (n_components, n_dimensions) array of means.
   """
   points = points.copy()
   n_points = points.shape[0]
   weights = jnp.ones(n_points) / n_points
   rng, subrng = jax.random.split(rng)
-  index = jax.random.choice(key=subrng, a=points.shape[0], p=weights)
+  index = jax.random.choice(subrng, a=points.shape[0], p=weights)
   loc = points[index]
   points = jnp.concatenate([points[:index], points[index + 1:]], axis=0)
 
   locs = loc[None]
   for _ in range(n_components - 1):
     dist_sq = _get_dist_sq(points, locs)
     min_dist_sq = jnp.min(dist_sq, axis=-1)
     weights = min_dist_sq / jnp.sum(min_dist_sq)
     rng, subrng = jax.random.split(rng)
-    index = jax.random.choice(key=subrng, a=points.shape[0], p=weights)
+    index = jax.random.choice(subrng, a=points.shape[0], p=weights)
     loc = points[index]
     points = jnp.concatenate([points[:index], points[index + 1:]], axis=0)
     locs = jnp.concatenate([locs, loc[None]], axis=0)
   return locs
 
 
 def from_kmeans_plusplus(
```

### Comparing `ott-jax-0.4.5/src/ott/tools/gaussian_mixture/fit_gmm_pair.py` & `ott_jax-0.4.6/src/ott/tools/gaussian_mixture/fit_gmm_pair.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.5/src/ott/tools/gaussian_mixture/gaussian.py` & `ott_jax-0.4.6/src/ott/tools/gaussian_mixture/gaussian.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import jax
 import jax.numpy as jnp
 
 from ott.tools.gaussian_mixture import scale_tril
 
 __all__ = ["Gaussian"]
 
-LOG2PI = math.log(2. * math.pi)
+LOG2PI = math.log(2.0 * math.pi)
 
 
 @jax.tree_util.register_pytree_node_class
 class Gaussian:
   """Normal distribution."""
 
   def __init__(self, loc: jnp.ndarray, scale: scale_tril.ScaleTriL):
@@ -64,36 +64,32 @@
   def from_random(
       cls,
       rng: jax.Array,
       n_dimensions: int,
       stdev_mean: float = 0.1,
       stdev_cov: float = 0.1,
       ridge: Union[float, jnp.ndarray] = 0,
-      dtype: Optional[jnp.dtype] = None
   ) -> "Gaussian":
     """Construct a random Gaussian.
 
     Args:
       rng: jax.random key
       n_dimensions: desired covariance dimensions
       stdev_mean: standard deviation of location and log eigenvalues
         (means for both are 0)
       stdev_cov: standard deviated of the covariance
       ridge: Offset for means.
-      dtype: data type
 
     Returns:
       A random Gaussian.
     """
     rng, subrng0, subrng1 = jax.random.split(rng, num=3)
-    loc = jax.random.normal(
-        key=subrng0, shape=(n_dimensions,), dtype=dtype
-    ) * stdev_mean + ridge
+    loc = jax.random.normal(subrng0, shape=(n_dimensions,)) * stdev_mean + ridge
     scale = scale_tril.ScaleTriL.from_random(
-        rng=subrng1, n_dimensions=n_dimensions, stdev=stdev_cov, dtype=dtype
+        subrng1, n_dimensions=n_dimensions, stdev=stdev_cov
     )
     return cls(loc=loc, scale=scale)
 
   @classmethod
   def from_mean_and_cov(cls, mean: jnp.ndarray, cov: jnp.ndarray) -> "Gaussian":
     """Construct a Gaussian from a mean and covariance."""
     scale = scale_tril.ScaleTriL.from_covariance(cov)
@@ -131,20 +127,20 @@
       x: jnp.ndarray,  # (?, d)
   ) -> jnp.ndarray:  # (?, d)
     """Log probability for a Gaussian with a diagonal covariance."""
     d = x.shape[-1]
     z = self.to_z(x)
     log_det = self.scale.log_det_covariance()
     return (
-        -0.5 * (d * LOG2PI + log_det[None] + jnp.sum(z ** 2., axis=-1))
+        -0.5 * (d * LOG2PI + log_det[None] + jnp.sum(z ** 2, axis=-1))
     )  # (?, k)
 
   def sample(self, rng: jax.Array, size: int) -> jnp.ndarray:
     """Generate samples from the distribution."""
-    std_samples_t = jax.random.normal(key=rng, shape=(self.n_dimensions, size))
+    std_samples_t = jax.random.normal(rng, shape=(self.n_dimensions, size))
     return self.loc[None] + (
         jnp.swapaxes(
             jnp.matmul(self.scale.cholesky(), std_samples_t),
             axis1=-2,
             axis2=-1
         )
     )
@@ -159,15 +155,15 @@
 
     Args:
       other: other Gaussian
 
     Returns:
       The :math:`W_2^2` distance between self and other
     """
-    delta_mean = jnp.sum((self.loc - other.loc) ** 2., axis=-1)
+    delta_mean = jnp.sum((self.loc - other.loc) ** 2, axis=-1)
     delta_sigma = self.scale.w2_dist(other.scale)
     return delta_mean + delta_sigma
 
   def f_potential(self, dest: "Gaussian", points: jnp.ndarray) -> jnp.ndarray:
     """Optimal potential for W2 distance between Gaussians. Evaluated on points.
 
     Args:
```

### Comparing `ott-jax-0.4.5/src/ott/tools/gaussian_mixture/gaussian_mixture.py` & `ott_jax-0.4.6/src/ott/tools/gaussian_mixture/gaussian_mixture.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from typing import List, Optional, Tuple, Union
+from typing import List, Tuple, Union
 
 import jax
 import jax.numpy as jnp
 
 from ott.tools.gaussian_mixture import (
     gaussian,
     linalg,
@@ -81,35 +81,35 @@
       rng: jax.Array,
       n_components: int,
       n_dimensions: int,
       stdev_mean: float = 0.1,
       stdev_cov: float = 0.1,
       stdev_weights: float = 0.1,
       ridge: Union[float, jnp.array] = 0,
-      dtype: Optional[jnp.dtype] = None
   ) -> "GaussianMixture":
     """Construct a random GMM."""
     loc = []
     scale_params = []
     for _ in range(n_components):
       rng, subrng = jax.random.split(rng)
       component = gaussian.Gaussian.from_random(
-          rng=subrng,
+          subrng,
           n_dimensions=n_dimensions,
           stdev_mean=stdev_mean,
           stdev_cov=stdev_cov,
           ridge=ridge,
-          dtype=dtype
       )
       loc.append(component.loc)
       scale_params.append(component.scale.params)
     loc = jnp.stack(loc, axis=0)
     scale_params = jnp.stack(scale_params, axis=0)
     weight_ob = probabilities.Probabilities.from_random(
-        rng=subrng, n_dimensions=n_components, stdev=stdev_weights, dtype=dtype
+        subrng,
+        n_dimensions=n_components,
+        stdev=stdev_weights,
     )
     return cls(
         loc=loc, scale_params=scale_params, component_weight_ob=weight_ob
     )
 
   @classmethod
   def from_mean_cov_component_weights(
@@ -219,17 +219,15 @@
     """List of all GMM components."""
     return [self.get_component(i) for i in range(self.n_components)]
 
   def sample(self, rng: jax.Array, size: int) -> jnp.ndarray:
     """Generate samples from the distribution."""
     subrng0, subrng1 = jax.random.split(rng)
     component = self.component_weight_ob.sample(rng=subrng0, size=size)
-    std_samples = jax.random.normal(
-        key=subrng1, shape=(size, self.n_dimensions)
-    )
+    std_samples = jax.random.normal(subrng1, shape=(size, self.n_dimensions))
 
     def _transform_single_component(k, scale, loc):
 
       def _transform_single_value(single_component, single_x):
         return jax.lax.cond(
             single_component == k,
             lambda x: jnp.matmul(scale, x[:, None])[:, 0] + loc, jnp.zeros_like,
```

### Comparing `ott-jax-0.4.5/src/ott/tools/gaussian_mixture/gaussian_mixture_pair.py` & `ott_jax-0.4.6/src/ott/tools/gaussian_mixture/gaussian_mixture_pair.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,16 +47,16 @@
   to compute the divergence between GMMs.
   """
 
   def __init__(
       self,
       gmm0: gaussian_mixture.GaussianMixture,
       gmm1: gaussian_mixture.GaussianMixture,
-      epsilon: float = 1.e-2,
-      tau: float = 1.,
+      epsilon: float = 1e-2,
+      tau: float = 1.0,
       lock_gmm1: bool = False,
   ):
     """Constructor.
 
     When fitting a pair of coupled GMMs with *no* reweighting of components
     using the algorithm in :cite:`delon:20`, set tau = 1. The coupling between
     components will be determined via the balanced Sinkhorn algorithm.
@@ -100,15 +100,15 @@
 
   @property
   def tau(self):  # noqa: D102
     return self._tau
 
   @property
   def rho(self):  # noqa: D102
-    return self.epsilon * self.tau / (1. - self.tau)
+    return self.epsilon * self.tau / (1.0 - self.tau)
 
   @property
   def lock_gmm1(self):  # noqa: D102
     return self._lock_gmm1
 
   def get_bures_geometry(self) -> pointcloud.PointCloud:
     """Get a Bures Geometry for the two GMMs."""
```

### Comparing `ott-jax-0.4.5/src/ott/tools/gaussian_mixture/linalg.py` & `ott_jax-0.4.6/src/ott/tools/gaussian_mixture/linalg.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from typing import Callable, Iterable, List, Optional, Tuple
+from typing import Callable, Iterable, List, Tuple
 
 import jax
 import jax.numpy as jnp
 
 
 def get_mean_and_var(
     points: jnp.ndarray,  # (n, d)
@@ -27,15 +27,15 @@
       # matmul((1, n), (n, d)) -> (1, d)
       jnp.matmul(weights, points) / weights_sum
   )
   # center points
   centered = points - mean[None, :]  # (n, d) - (1, d)
   var = (
       # matmul((1, n), (n, d)) -> (1, d)
-      jnp.matmul(weights, centered ** 2.) / weights_sum
+      jnp.matmul(weights, centered ** 2) / weights_sum
   )
   return mean, var
 
 
 def get_mean_and_cov(
     points: jnp.ndarray,  # (n, d)
     weights: jnp.ndarray,  # (n,)
@@ -67,15 +67,15 @@
     size: size of lower triangular matrices. x should have shape
       (..., size(size+1)/2), and the final matrices should have shape
       (..., size, size).
 
   Returns:
     Lower triangular matrices.
   """
-  m = jnp.zeros(tuple(list(x.shape[:-1]) + [size, size]), dtype=x.dtype)
+  m = jnp.zeros(x.shape[:-1] + (size, size))
   tril = jnp.tril_indices(size)
   return m.at[..., tril[0], tril[1]].set(x)
 
 
 def tril_to_flat(m: jnp.ndarray) -> jnp.ndarray:
   """Flatten lower triangular matrices.
 
@@ -92,15 +92,15 @@
 
 def apply_to_diag(
     m: jnp.ndarray, fn: Callable[[jnp.ndarray], jnp.ndarray]
 ) -> jnp.ndarray:
   """Apply a function to the diagonal of a matrix."""
   size = m.shape[-1]
   diag = jnp.diagonal(m, axis1=-2, axis2=-1)
-  ind = jnp.arange(size, dtype=jnp.int32)
+  ind = jnp.arange(size)
   return m.at[..., ind, ind].set(fn(diag))
 
 
 def matrix_powers(
     m: jnp.ndarray,
     powers: Iterable[float],
 ) -> List[jnp.ndarray]:
@@ -127,14 +127,12 @@
     m^{-1} x
   """
   return jnp.transpose(
       jax.scipy.linalg.solve_triangular(m, jnp.transpose(x), lower=lower)
   )
 
 
-def get_random_orthogonal(
-    rng: jax.Array, dim: int, dtype: Optional[jnp.dtype] = None
-) -> jnp.ndarray:
+def get_random_orthogonal(rng: jax.Array, dim: int) -> jnp.ndarray:
   """Get a random orthogonal matrix with the specified dimension."""
-  m = jax.random.normal(key=rng, shape=[dim, dim], dtype=dtype)
+  m = jax.random.normal(rng, shape=[dim, dim])
   q, _ = jnp.linalg.qr(m)
   return q
```

### Comparing `ott-jax-0.4.5/src/ott/tools/gaussian_mixture/probabilities.py` & `ott_jax-0.4.6/src/ott/tools/gaussian_mixture/probabilities.py`

 * *Files 18% similar despite different names*

```diff
@@ -34,21 +34,17 @@
 
   @classmethod
   def from_random(
       cls,
       rng: jax.Array,
       n_dimensions: int,
       stdev: Optional[float] = 0.1,
-      dtype: Optional[jnp.dtype] = None
   ) -> "Probabilities":
     """Construct a random Probabilities."""
-    return cls(
-        params=jax.random
-        .normal(key=rng, shape=(n_dimensions - 1,), dtype=dtype) * stdev
-    )
+    return cls(params=jax.random.normal(rng, shape=(n_dimensions - 1,)) * stdev)
 
   @classmethod
   def from_probs(cls, probs: jnp.ndarray) -> "Probabilities":
     """Construct Probabilities from a vector of probabilities."""
     log_probs = jnp.log(probs)
     log_probs_normalized, norm = log_probs[:-1], log_probs[-1]
     log_probs_normalized -= norm
@@ -60,30 +56,28 @@
 
   @property
   def dtype(self):  # noqa: D102
     return self._params.dtype
 
   def unnormalized_log_probs(self) -> jnp.ndarray:
     """Get the unnormalized log probabilities."""
-    return jnp.concatenate([self._params,
-                            jnp.zeros((1,), dtype=self.dtype)],
-                           axis=-1)
+    return jnp.concatenate([self._params, jnp.zeros((1,))], axis=-1)
 
   def log_probs(self) -> jnp.ndarray:
     """Get the log probabilities."""
     return jax.nn.log_softmax(self.unnormalized_log_probs())
 
   def probs(self) -> jnp.ndarray:
     """Get the probabilities."""
     return jax.nn.softmax(self.unnormalized_log_probs())
 
   def sample(self, rng: jax.Array, size: int) -> jnp.ndarray:
     """Sample from the distribution."""
     return jax.random.categorical(
-        key=rng, logits=self.unnormalized_log_probs(), shape=(size,)
+        rng, logits=self.unnormalized_log_probs(), shape=(size,)
     )
 
   def tree_flatten(self):  # noqa: D102
     children = (self.params,)
     aux_data = {}
     return children, aux_data
```

### Comparing `ott-jax-0.4.5/src/ott/tools/gaussian_mixture/scale_tril.py` & `ott_jax-0.4.6/src/ott/tools/gaussian_mixture/scale_tril.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,35 +43,31 @@
 
   @classmethod
   def from_random(
       cls,
       rng: jax.Array,
       n_dimensions: int,
       stdev: Optional[float] = 0.1,
-      dtype: jnp.dtype = jnp.float32,
   ) -> "ScaleTriL":
     """Construct a random ScaleTriL.
 
     Args:
       rng: pseudo-random number generator key
       n_dimensions: number of dimensions
       stdev: desired standard deviation (around 0) for the log eigenvalues
-      dtype: data type for the covariance matrix
 
     Returns:
       A ScaleTriL.
     """
     # generate a random orthogonal matrix
     rng, subrng = jax.random.split(rng)
-    q = linalg.get_random_orthogonal(rng=subrng, dim=n_dimensions, dtype=dtype)
+    q = linalg.get_random_orthogonal(subrng, dim=n_dimensions)
 
     # generate random eigenvalues
-    eigs = stdev * jnp.exp(
-        jax.random.normal(key=rng, shape=(n_dimensions,), dtype=dtype)
-    )
+    eigs = stdev * jnp.exp(jax.random.normal(rng, shape=(n_dimensions,)))
 
     # random positive definite matrix
     sigma = q * jnp.expand_dims(eigs, -2) @ q.T
 
     # cholesky factorization
     chol = jnp.linalg.cholesky(sigma)
     # flatten
@@ -123,15 +119,15 @@
   def covariance_sqrt(self) -> jnp.ndarray:
     """Get the square root of the covariance matrix."""
     return linalg.matrix_powers(self.covariance(), (0.5,))[0]
 
   def log_det_covariance(self) -> jnp.ndarray:
     """Get the log of the determinant of the covariance matrix."""
     diag = jnp.diagonal(self.cholesky(), axis1=-2, axis2=-1)
-    return 2. * jnp.sum(jnp.log(diag), axis=-1)
+    return 2.0 * jnp.sum(jnp.log(diag), axis=-1)
 
   def centered_to_z(self, x_centered: jnp.ndarray) -> jnp.ndarray:
     """Map centered points to standardized centered points (i.e. cov(z) = I)."""
     return linalg.invmatvectril(m=self.cholesky(), x=x_centered, lower=True)
 
   def z_to_centered(self, z: jnp.ndarray) -> jnp.ndarray:
     """Scale standardized points to points with the specified covariance."""
```

### Comparing `ott-jax-0.4.5/src/ott/tools/k_means.py` & `ott_jax-0.4.6/src/ott/tools/k_means.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,15 @@
     n_local_trials: Optional[int] = None,
 ) -> jnp.ndarray:
 
   def init_fn(geom: pointcloud.PointCloud, rng: jax.Array) -> KPPState:
     rng, next_rng = jax.random.split(rng, 2)
     ix = jax.random.choice(rng, jnp.arange(geom.shape[0]), shape=())
     centroids = jnp.full((k, geom.cost_rank), jnp.inf).at[0].set(geom.x[ix])
-    dists = geom.subset(ix, None).cost_matrix[0]
+    dists = geom.subset([ix], None).cost_matrix[0]
     return KPPState(rng=next_rng, centroids=centroids, centroid_dists=dists)
 
   def body_fn(
       iteration: int, const: Tuple[pointcloud.PointCloud, jnp.ndarray],
       state: KPPState, compute_error: bool
   ) -> KPPState:
     del compute_error
@@ -177,15 +177,15 @@
 @functools.partial(jax.vmap, in_axes=[None, 0, 0, 0], out_axes=0)
 def _reallocate_centroids(
     const: KMeansConst,
     ix: jnp.ndarray,
     centroid: jnp.ndarray,
     weight: jnp.ndarray,
 ) -> Tuple[jnp.ndarray, jnp.ndarray]:
-  is_empty = weight <= 0.
+  is_empty = weight <= 0.0
   new_centroid = (1 - is_empty) * centroid + is_empty * const.x[ix]  # (ndim,)
   centroid_to_remove = is_empty * const.weighted_x[ix]  # (ndim,)
   weight_to_remove = is_empty * const.weights[ix]  # (1,)
   return new_centroid, jnp.concatenate([centroid_to_remove, weight_to_remove])
 
 
 def _update_assignment(
@@ -215,15 +215,15 @@
   centroids, to_remove = _reallocate_centroids(const, far_ixs, centroids, ws)
   to_remove = jax.ops.segment_sum(
       to_remove, assignment[far_ixs], num_segments=k
   )
   centroids -= to_remove[:, :-1]
   ws -= to_remove[:, -1:]
 
-  return centroids * jnp.where(ws > 0., 1. / ws, 1.)
+  return centroids * jnp.where(ws > 0.0, 1.0 / ws, 1.0)
 
 
 @functools.partial(jax.vmap, in_axes=[0] + [None] * 9)
 def _k_means(
     rng: jax.Array,
     geom: pointcloud.PointCloud,
     k: int,
@@ -262,17 +262,17 @@
     # .../jax/_src/dtypes.py:370:
     # .0 = <set_iterator object at 0x7f4d002a1dc0>
     # >   CUB = set.intersection(*(UB[n] for n in N))
     # E   jax._src.traceback_util.UnfilteredStackTrace:
     #   KeyError: dtype([('float0', 'V')])
     # E   The stack trace below excludes JAX-internal frames.
     # E   The preceding is the original exception that occurred, unmodified.
-    prev_assignment = jnp.full((n,), -2.)
-    assignment = jnp.full((n,), -1.)
-    errors = jnp.full((max_iterations,), -1.)
+    prev_assignment = jnp.full((n,), -2.0)
+    assignment = jnp.full((n,), -1.0)
+    errors = jnp.full((max_iterations,), -1.0)
 
     return KMeansState(
         centroids=centroids,
         prev_assignment=prev_assignment,
         assignment=assignment,
         center_shift=jnp.inf,
         errors=errors,
```

### Comparing `ott-jax-0.4.5/src/ott/tools/plot.py` & `ott_jax-0.4.6/src/ott/tools/plot.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.5/src/ott/tools/segment_sinkhorn.py` & `ott_jax-0.4.6/src/ott/tools/segment_sinkhorn.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,16 +105,16 @@
 
   def eval_fn(
       padded_x: jnp.ndarray,
       padded_y: jnp.ndarray,
       padded_weight_x: jnp.ndarray,
       padded_weight_y: jnp.ndarray,
   ) -> float:
-    mask_x = padded_weight_x > 0.
-    mask_y = padded_weight_y > 0.
+    mask_x = padded_weight_x > 0.0
+    mask_y = padded_weight_y > 0.0
 
     geom = pointcloud.PointCloud(
         padded_x,
         padded_y,
         cost_fn=cost_fn,
         src_mask=mask_x,
         tgt_mask=mask_y,
```

### Comparing `ott-jax-0.4.5/src/ott/tools/sinkhorn_divergence.py` & `ott_jax-0.4.6/src/ott/tools/sinkhorn_divergence.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,14 +189,15 @@
 
   out_xy = linear.solve(geometry_xy, a, b, **kwargs)
   out_xx = linear.solve(geometry_xx, a, a, **kwargs_symmetric)
   if geometry_yy is None:
     # Create dummy output, corresponds to scenario where static_b is True.
     # This choice ensures that `converged`` of this dummy output is True.
     out_yy = sinkhorn.SinkhornOutput(
+        (None, None),
         errors=jnp.array([-jnp.inf]),
         reg_ot_cost=0.0,
         threshold=0.0,
         inner_iterations=0,
     )
   else:
     out_yy = linear.solve(geometry_yy, b, b, **kwargs_symmetric)
@@ -314,16 +315,16 @@
 
   def eval_fn(
       padded_x: jnp.ndarray,
       padded_y: jnp.ndarray,
       padded_weight_x: jnp.ndarray,
       padded_weight_y: jnp.ndarray,
   ) -> float:
-    mask_x = padded_weight_x > 0.
-    mask_y = padded_weight_y > 0.
+    mask_x = padded_weight_x > 0.0
+    mask_y = padded_weight_y > 0.0
     return sinkhorn_divergence(
         pointcloud.PointCloud,
         padded_x,
         padded_y,
         a=padded_weight_x,
         b=padded_weight_y,
         sinkhorn_kwargs=sinkhorn_kwargs,
```

### Comparing `ott-jax-0.4.5/src/ott/tools/soft_sort.py` & `ott_jax-0.4.6/src/ott/tools/soft_sort.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,15 +125,15 @@
   """Apply the soft sort operator on a one dimensional array."""
   num_points = inputs.shape[0]
   a = jnp.ones((num_points,)) / num_points
   if 0 < topk < num_points:
     start_index = 1
     b = jnp.concatenate([
         jnp.array([(num_points - topk) / num_points]),
-        jnp.ones(topk, dtype=inputs.dtype) / num_points
+        jnp.ones(topk) / num_points
     ])
   else:
     # Use the "sorting" initializer if default uniform weights of same size.
     if num_targets is None or num_targets == num_points:
       num_targets = num_points
       # use sorting initializer in this case.
       kwargs.setdefault("initializer", "sorting")
@@ -365,15 +365,16 @@
   .. code-block:: python
 
     x_quantiles = jax.numpy.quantile(x, q=jnp.array([0.2, 0.8]))
 
   Args:
    inputs: an Array of any shape.
    q: values of the quantile level to be computed, e.g. [0.5] for median.
-     These values should all lie in :math:`[0,1]`.
+     These values should all lie within the segment :math:`]0,1[`, excluding
+     boundary values :math:`0` and :math:`1`.
    axis: the axis on which to apply the operator.
    weight: the weight assigned to each quantile target value in the OT problem.
      This weight should be small, typically of the order of ``1/n``, where ``n``
      is the size of ``x``. Note: Since the size of ``q`` times ``weight``
      must be strictly smaller than ``1``, in order to leave enough mass to set
      other target values in the transport problem, the algorithm might ensure
      this by setting, when needed, a lower value.
@@ -410,15 +411,15 @@
         jnp.array([1.0 / num_quantiles]), filler_weights
     ])
     if weight is None:
       # Populate with other options.
       safe_weight = jnp.concatenate([
           safe_weight,
           jnp.array(
-              [.02]
+              [0.02]
           ),  # reasonable mass per quantile for a small number of points
           jnp.array(
               [1.5 / num_points]
           ),  # this means each quantile would be ~ assigned 1.5 points.
       ])
     else:
       safe_weight = jnp.concatenate([safe_weight, jnp.atleast_1d(weight)])
@@ -454,15 +455,15 @@
 
   return apply_on_axis(_quantile, inputs, axis, q, weight, **kwargs)
 
 
 def multivariate_cdf_quantile_maps(
     inputs: jnp.ndarray,
     target_sampler: Optional[Callable[[jax.Array, Tuple[int, int]],
-                                      jnp.ndarray]] = None,
+                                      jax.Array]] = None,
     rng: Optional[jax.Array] = None,
     num_target_samples: Optional[int] = None,
     cost_fn: Optional[costs.CostFn] = None,
     epsilon: Optional[float] = None,
     input_weights: Optional[jnp.ndarray] = None,
     target_weights: Optional[jnp.ndarray] = None,
     **kwargs: Any
@@ -631,20 +632,20 @@
       are passed on to parameterize the
       :class:`~ott.solvers.linear.sinkhorn.Sinkhorn` solver.
 
   Returns:
     An Array of size [batch | topk, dim].
   """
   num_points = criterion.shape[0]
-  weights = jnp.ones(num_points, dtype=criterion.dtype) / num_points
+  weights = jnp.ones(num_points) / num_points
   if 0 < topk < num_points:
     start_index = 1
     target_weights = jnp.concatenate([
         jnp.array([(num_points - topk) / num_points]),
-        jnp.ones(topk, dtype=inputs.dtype) / num_points
+        jnp.ones(topk) / num_points
     ])
   else:
     start_index = 0
     target_weights = jnp.ones((num_points,)) / num_points
   ot = transport_for_sort(criterion, weights, target_weights, **kwargs)
   # Applies the topk on each of the dimensions of the inputs.
   sort_fn = jax.vmap(
```

### Comparing `ott-jax-0.4.5/src/ott/types.py` & `ott_jax-0.4.6/src/ott/types.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,26 +7,22 @@
 #   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from typing import Protocol, Union
+from typing import Protocol
 
-import jax.experimental.sparse as jesp
 import jax.numpy as jnp
 
-__all__ = ["Transport", "Array_g"]
+__all__ = ["Transport"]
 
 # TODO(michalk8): introduce additional types here
 
-# Either a dense or sparse array.
-Array_g = Union[jnp.ndarray, jesp.BCOO]
-
 
 class Transport(Protocol):
   """Interface for the solution of a transport problem.
 
   Classes implementing those function do not have to inherit from it, the
   class can however be used in type hints to support duck typing.
   """
```

### Comparing `ott-jax-0.4.5/src/ott/utils.py` & `ott_jax-0.4.6/src/ott/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 Status_t = Tuple[np.ndarray, np.ndarray, np.ndarray, NamedTuple]
 IOCallback_t = Callable[[Status_t], None]
 
 
 def register_pytree_node(cls: type) -> type:
   """Register dataclasses as pytree_nodes."""
   cls = dataclasses.dataclass()(cls)
-  flatten = lambda obj: jax.tree_flatten(dataclasses.asdict(obj))
+  flatten = lambda obj: jax.tree_util.tree_flatten(dataclasses.asdict(obj))
   unflatten = lambda d, children: cls(**d.unflatten(children))
   jax.tree_util.register_pytree_node(cls, flatten, unflatten)
   return cls
 
 
 def deprecate(  # noqa: D103
     *,
```

### Comparing `ott-jax-0.4.5/src/ott_jax.egg-info/PKG-INFO` & `ott_jax-0.4.6/src/ott_jax.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ott-jax
-Version: 0.4.5
+Version: 0.4.6
 Summary: Optimal Transport Tools in JAX.
 Author-email: OTT team <optimal.transport.tools@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -232,14 +232,15 @@
 Requires-Dist: jax>=0.4.0
 Requires-Dist: jaxopt>=0.8
 Requires-Dist: lineax>=0.0.1; python_version >= "3.9"
 Requires-Dist: numpy>=1.20.0
 Provides-Extra: neural
 Requires-Dist: flax>=0.6.6; extra == "neural"
 Requires-Dist: optax>=0.1.1; extra == "neural"
+Requires-Dist: diffrax>=0.4.1; extra == "neural"
 Provides-Extra: dev
 Requires-Dist: pre-commit>=2.16.0; extra == "dev"
 Requires-Dist: tox>=4; extra == "dev"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-xdist; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
```

### Comparing `ott-jax-0.4.5/src/ott_jax.egg-info/requires.txt` & `ott_jax-0.4.6/src/ott_jax.egg-info/requires.txt`

 * *Files 23% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 sphinxcontrib-bibtex>=2.5.0
 sphinxcontrib-spelling>=7.7.0
 myst-nb>=0.17.1
 
 [neural]
 flax>=0.6.6
 optax>=0.1.1
+diffrax>=0.4.1
 
 [test]
 pytest
 pytest-xdist
 pytest-cov
 pytest-memray
 coverage[toml]
```

