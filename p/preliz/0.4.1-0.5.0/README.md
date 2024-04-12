# Comparing `tmp/preliz-0.4.1.tar.gz` & `tmp/preliz-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "preliz-0.4.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "preliz-0.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `preliz-0.4.1.tar` & `preliz-0.5.0.tar`

### file list

```diff
@@ -1,66 +1,83 @@
--rw-r--r--   0        0        0     4324 2024-03-20 20:11:58.296345 preliz-0.4.1/README.md
--rw-r--r--   0        0        0      649 2024-03-20 20:11:58.352345 preliz-0.4.1/preliz/__init__.py
--rw-r--r--   0        0        0     1037 2024-03-20 20:11:58.352345 preliz-0.4.1/preliz/distributions/__init__.py
--rw-r--r--   0        0        0     6843 2024-03-20 20:11:58.352345 preliz-0.4.1/preliz/distributions/asymmetric_laplace.py
--rw-r--r--   0        0        0     4937 2024-03-20 20:11:58.352345 preliz-0.4.1/preliz/distributions/bernoulli.py
--rw-r--r--   0        0        0     7833 2024-03-20 20:11:58.352345 preliz-0.4.1/preliz/distributions/beta.py
--rw-r--r--   0        0        0     5191 2024-03-20 20:11:58.352345 preliz-0.4.1/preliz/distributions/binomial.py
--rw-r--r--   0        0        0    70711 2024-03-20 20:11:58.352345 preliz-0.4.1/preliz/distributions/continuous.py
--rw-r--r--   0        0        0    21548 2024-03-20 20:11:58.352345 preliz-0.4.1/preliz/distributions/continuous_multivariate.py
--rw-r--r--   0        0        0    17413 2024-03-20 20:11:58.352345 preliz-0.4.1/preliz/distributions/discrete.py
--rw-r--r--   0        0        0    23827 2024-03-20 20:11:58.352345 preliz-0.4.1/preliz/distributions/distributions.py
--rw-r--r--   0        0        0     6516 2024-03-20 20:11:58.352345 preliz-0.4.1/preliz/distributions/distributions_multivariate.py
--rw-r--r--   0        0        0     4323 2024-03-20 20:11:58.352345 preliz-0.4.1/preliz/distributions/exponential.py
--rw-r--r--   0        0        0     4927 2024-03-20 20:11:58.352345 preliz-0.4.1/preliz/distributions/halfnormal.py
--rw-r--r--   0        0        0     3986 2024-03-20 20:11:58.352345 preliz-0.4.1/preliz/distributions/laplace.py
--rw-r--r--   0        0        0     6028 2024-03-20 20:11:58.352345 preliz-0.4.1/preliz/distributions/negativebinomial.py
--rw-r--r--   0        0        0     4993 2024-03-20 20:11:58.352345 preliz-0.4.1/preliz/distributions/normal.py
--rw-r--r--   0        0        0     4155 2024-03-20 20:11:58.352345 preliz-0.4.1/preliz/distributions/poisson.py
--rw-r--r--   0        0        0     5005 2024-03-20 20:11:58.352345 preliz-0.4.1/preliz/distributions/weibull.py
--rw-r--r--   0        0        0     5683 2024-03-20 20:11:58.352345 preliz-0.4.1/preliz/distributions/zi_binomial.py
--rw-r--r--   0        0        0     7364 2024-03-20 20:11:58.352345 preliz-0.4.1/preliz/distributions/zi_negativebinomial.py
--rw-r--r--   0        0        0     5767 2024-03-20 20:11:58.352345 preliz-0.4.1/preliz/distributions/zi_poisson.py
--rw-r--r--   0        0        0       64 2024-03-20 20:11:58.352345 preliz-0.4.1/preliz/internal/__init__.py
--rw-r--r--   0        0        0     4449 2024-03-20 20:11:58.352345 preliz-0.4.1/preliz/internal/distribution_helper.py
--rw-r--r--   0        0        0    12151 2024-03-20 20:11:58.352345 preliz-0.4.1/preliz/internal/optimization.py
--rw-r--r--   0        0        0     5596 2024-03-20 20:11:58.352345 preliz-0.4.1/preliz/internal/parser.py
--rw-r--r--   0        0        0    18535 2024-03-20 20:11:58.352345 preliz-0.4.1/preliz/internal/plot_helper.py
--rw-r--r--   0        0        0     9785 2024-03-20 20:11:58.352345 preliz-0.4.1/preliz/internal/plot_helper_multivariate.py
--rw-r--r--   0        0        0     2028 2024-03-20 20:11:58.352345 preliz-0.4.1/preliz/internal/predictive_helper.py
--rw-r--r--   0        0        0     4157 2024-03-20 20:11:58.352345 preliz-0.4.1/preliz/internal/special.py
--rw-r--r--   0        0        0     6465 2024-03-20 20:11:58.352345 preliz-0.4.1/preliz/ppls/pymc_io.py
--rw-r--r--   0        0        0      145 2024-03-20 20:11:58.352345 preliz-0.4.1/preliz/predictive/__init__.py
--rw-r--r--   0        0        0    14617 2024-03-20 20:11:58.352345 preliz-0.4.1/preliz/predictive/ppa.py
--rw-r--r--   0        0        0     2251 2024-03-20 20:11:58.352345 preliz-0.4.1/preliz/predictive/ppe.py
--rw-r--r--   0        0        0     2160 2024-03-20 20:11:58.352345 preliz-0.4.1/preliz/predictive/predictive_explorer.py
--rw-r--r--   0        0        0     1946 2024-03-20 20:11:58.352345 preliz-0.4.1/preliz/tests/check_inside_notebook.ipynb
--rw-r--r--   0        0        0     1787 2024-03-20 20:11:58.352345 preliz-0.4.1/preliz/tests/plot_interactive.ipynb
--rw-r--r--   0        0        0   477854 2024-03-20 20:11:58.356345 preliz-0.4.1/preliz/tests/ppa.ipynb
--rw-r--r--   0        0        0     2787 2024-03-20 20:11:58.356345 preliz-0.4.1/preliz/tests/predictive_explorer.ipynb
--rw-r--r--   0        0        0     1439 2024-03-20 20:11:58.356345 preliz-0.4.1/preliz/tests/quartile_int.ipynb
--rw-r--r--   0        0        0     1472 2024-03-20 20:11:58.356345 preliz-0.4.1/preliz/tests/roulette.ipynb
--rw-r--r--   0        0        0      661 2024-03-20 20:11:58.356345 preliz-0.4.1/preliz/tests/test_beta_mode.py
--rw-r--r--   0        0        0      757 2024-03-20 20:11:58.356345 preliz-0.4.1/preliz/tests/test_dirichlet_mode.py
--rw-r--r--   0        0        0     7196 2024-03-20 20:11:58.356345 preliz-0.4.1/preliz/tests/test_distributions.py
--rw-r--r--   0        0        0      346 2024-03-20 20:11:58.356345 preliz-0.4.1/preliz/tests/test_distributions_helper.py
--rw-r--r--   0        0        0      626 2024-03-20 20:11:58.356345 preliz-0.4.1/preliz/tests/test_helper.py
--rw-r--r--   0        0        0      338 2024-03-20 20:11:58.356345 preliz-0.4.1/preliz/tests/test_internals.py
--rw-r--r--   0        0        0     6659 2024-03-20 20:11:58.356345 preliz-0.4.1/preliz/tests/test_maxent.py
--rw-r--r--   0        0        0     2919 2024-03-20 20:11:58.356345 preliz-0.4.1/preliz/tests/test_mle.py
--rw-r--r--   0        0        0     5741 2024-03-20 20:11:58.356345 preliz-0.4.1/preliz/tests/test_plots.py
--rw-r--r--   0        0        0       85 2024-03-20 20:11:58.356345 preliz-0.4.1/preliz/tests/test_ppa.py
--rw-r--r--   0        0        0      117 2024-03-20 20:11:58.356345 preliz-0.4.1/preliz/tests/test_predictive_explorer.py
--rw-r--r--   0        0        0     3489 2024-03-20 20:11:58.356345 preliz-0.4.1/preliz/tests/test_quartile.py
--rw-r--r--   0        0        0      103 2024-03-20 20:11:58.356345 preliz-0.4.1/preliz/tests/test_quartile_int.py
--rw-r--r--   0        0        0      910 2024-03-20 20:11:58.356345 preliz-0.4.1/preliz/tests/test_roulette.py
--rw-r--r--   0        0        0     4462 2024-03-20 20:11:58.356345 preliz-0.4.1/preliz/tests/test_scipy.py
--rw-r--r--   0        0        0      325 2024-03-20 20:11:58.356345 preliz-0.4.1/preliz/unidimensional/__init__.py
--rw-r--r--   0        0        0     2244 2024-03-20 20:11:58.356345 preliz-0.4.1/preliz/unidimensional/beta_mode.py
--rw-r--r--   0        0        0     2341 2024-03-20 20:11:58.356345 preliz-0.4.1/preliz/unidimensional/dirichlet_mode.py
--rw-r--r--   0        0        0     3895 2024-03-20 20:11:58.356345 preliz-0.4.1/preliz/unidimensional/maxent.py
--rw-r--r--   0        0        0     1681 2024-03-20 20:11:58.356345 preliz-0.4.1/preliz/unidimensional/mle.py
--rw-r--r--   0        0        0     3259 2024-03-20 20:11:58.356345 preliz-0.4.1/preliz/unidimensional/quartile.py
--rw-r--r--   0        0        0     6136 2024-03-20 20:11:58.356345 preliz-0.4.1/preliz/unidimensional/quartile_int.py
--rw-r--r--   0        0        0    12994 2024-03-20 20:11:58.356345 preliz-0.4.1/preliz/unidimensional/roulette.py
--rw-r--r--   0        0        0     1402 2024-03-20 20:11:58.356345 preliz-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     5559 1970-01-01 00:00:00.000000 preliz-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     4324 2024-04-12 12:55:33.124757 preliz-0.5.0/README.md
+-rw-r--r--   0        0        0      649 2024-04-12 12:55:33.180757 preliz-0.5.0/preliz/__init__.py
+-rw-r--r--   0        0        0     1154 2024-04-12 12:55:33.180757 preliz-0.5.0/preliz/distributions/__init__.py
+-rw-r--r--   0        0        0     6930 2024-04-12 12:55:33.180757 preliz-0.5.0/preliz/distributions/asymmetric_laplace.py
+-rw-r--r--   0        0        0     5012 2024-04-12 12:55:33.180757 preliz-0.5.0/preliz/distributions/bernoulli.py
+-rw-r--r--   0        0        0     7701 2024-04-12 12:55:33.180757 preliz-0.5.0/preliz/distributions/beta.py
+-rw-r--r--   0        0        0     5242 2024-04-12 12:55:33.180757 preliz-0.5.0/preliz/distributions/binomial.py
+-rw-r--r--   0        0        0     4723 2024-04-12 12:55:33.180757 preliz-0.5.0/preliz/distributions/categorical.py
+-rw-r--r--   0        0        0     7476 2024-04-12 12:55:33.180757 preliz-0.5.0/preliz/distributions/censored.py
+-rw-r--r--   0        0        0    42469 2024-04-12 12:55:33.180757 preliz-0.5.0/preliz/distributions/continuous.py
+-rw-r--r--   0        0        0    21548 2024-04-12 12:55:33.180757 preliz-0.5.0/preliz/distributions/continuous_multivariate.py
+-rw-r--r--   0        0        0    10600 2024-04-12 12:55:33.180757 preliz-0.5.0/preliz/distributions/discrete.py
+-rw-r--r--   0        0        0     5071 2024-04-12 12:55:33.180757 preliz-0.5.0/preliz/distributions/discrete_uniform.py
+-rw-r--r--   0        0        0    26023 2024-04-12 12:55:33.180757 preliz-0.5.0/preliz/distributions/distributions.py
+-rw-r--r--   0        0        0     6516 2024-04-12 12:55:33.180757 preliz-0.5.0/preliz/distributions/distributions_multivariate.py
+-rw-r--r--   0        0        0     4391 2024-04-12 12:55:33.180757 preliz-0.5.0/preliz/distributions/exponential.py
+-rw-r--r--   0        0        0     5866 2024-04-12 12:55:33.180757 preliz-0.5.0/preliz/distributions/gamma.py
+-rw-r--r--   0        0        0     3885 2024-04-12 12:55:33.180757 preliz-0.5.0/preliz/distributions/geometric.py
+-rw-r--r--   0        0        0     4920 2024-04-12 12:55:33.180757 preliz-0.5.0/preliz/distributions/halfnormal.py
+-rw-r--r--   0        0        0     7938 2024-04-12 12:55:33.180757 preliz-0.5.0/preliz/distributions/halfstudentt.py
+-rw-r--r--   0        0        0     6452 2024-04-12 12:55:33.180757 preliz-0.5.0/preliz/distributions/inversegamma.py
+-rw-r--r--   0        0        0     4061 2024-04-12 12:55:33.180757 preliz-0.5.0/preliz/distributions/laplace.py
+-rw-r--r--   0        0        0     6033 2024-04-12 12:55:33.180757 preliz-0.5.0/preliz/distributions/negativebinomial.py
+-rw-r--r--   0        0        0     5092 2024-04-12 12:55:33.180757 preliz-0.5.0/preliz/distributions/normal.py
+-rw-r--r--   0        0        0     4194 2024-04-12 12:55:33.180757 preliz-0.5.0/preliz/distributions/poisson.py
+-rw-r--r--   0        0        0     7610 2024-04-12 12:55:33.180757 preliz-0.5.0/preliz/distributions/studentt.py
+-rw-r--r--   0        0        0     6875 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/distributions/triangular.py
+-rw-r--r--   0        0        0     5668 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/distributions/truncated.py
+-rw-r--r--   0        0        0     4692 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/distributions/uniform.py
+-rw-r--r--   0        0        0     4987 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/distributions/vonmises.py
+-rw-r--r--   0        0        0     5763 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/distributions/wald.py
+-rw-r--r--   0        0        0     5068 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/distributions/weibull.py
+-rw-r--r--   0        0        0     5562 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/distributions/zi_binomial.py
+-rw-r--r--   0        0        0     7223 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/distributions/zi_negativebinomial.py
+-rw-r--r--   0        0        0     5667 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/distributions/zi_poisson.py
+-rw-r--r--   0        0        0       64 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/internal/__init__.py
+-rw-r--r--   0        0        0     4540 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/internal/distribution_helper.py
+-rw-r--r--   0        0        0    13847 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/internal/optimization.py
+-rw-r--r--   0        0        0     5596 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/internal/parser.py
+-rw-r--r--   0        0        0    19567 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/internal/plot_helper.py
+-rw-r--r--   0        0        0     9785 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/internal/plot_helper_multivariate.py
+-rw-r--r--   0        0        0     2028 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/internal/predictive_helper.py
+-rw-r--r--   0        0        0    11407 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/internal/special.py
+-rw-r--r--   0        0        0     6465 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/ppls/pymc_io.py
+-rw-r--r--   0        0        0      145 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/predictive/__init__.py
+-rw-r--r--   0        0        0    14617 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/predictive/ppa.py
+-rw-r--r--   0        0        0     2251 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/predictive/ppe.py
+-rw-r--r--   0        0        0     2160 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/predictive/predictive_explorer.py
+-rw-r--r--   0        0        0     1946 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/tests/check_inside_notebook.ipynb
+-rw-r--r--   0        0        0     1787 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/tests/plot_interactive.ipynb
+-rw-r--r--   0        0        0   477854 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/tests/ppa.ipynb
+-rw-r--r--   0        0        0     2787 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/tests/predictive_explorer.ipynb
+-rw-r--r--   0        0        0     1439 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/tests/quartile_int.ipynb
+-rw-r--r--   0        0        0     1472 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/tests/roulette.ipynb
+-rw-r--r--   0        0        0      661 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/tests/test_beta_mode.py
+-rw-r--r--   0        0        0     1967 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/tests/test_censored.py
+-rw-r--r--   0        0        0      757 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/tests/test_dirichlet_mode.py
+-rw-r--r--   0        0        0     7196 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/tests/test_distributions.py
+-rw-r--r--   0        0        0      346 2024-04-12 12:55:33.188757 preliz-0.5.0/preliz/tests/test_distributions_helper.py
+-rw-r--r--   0        0        0      626 2024-04-12 12:55:33.188757 preliz-0.5.0/preliz/tests/test_helper.py
+-rw-r--r--   0        0        0      338 2024-04-12 12:55:33.188757 preliz-0.5.0/preliz/tests/test_internals.py
+-rw-r--r--   0        0        0     6659 2024-04-12 12:55:33.188757 preliz-0.5.0/preliz/tests/test_maxent.py
+-rw-r--r--   0        0        0     2919 2024-04-12 12:55:33.188757 preliz-0.5.0/preliz/tests/test_mle.py
+-rw-r--r--   0        0        0      894 2024-04-12 12:55:33.188757 preliz-0.5.0/preliz/tests/test_optimization.py
+-rw-r--r--   0        0        0     5964 2024-04-12 12:55:33.188757 preliz-0.5.0/preliz/tests/test_plots.py
+-rw-r--r--   0        0        0       85 2024-04-12 12:55:33.188757 preliz-0.5.0/preliz/tests/test_ppa.py
+-rw-r--r--   0        0        0      117 2024-04-12 12:55:33.188757 preliz-0.5.0/preliz/tests/test_predictive_explorer.py
+-rw-r--r--   0        0        0     3489 2024-04-12 12:55:33.188757 preliz-0.5.0/preliz/tests/test_quartile.py
+-rw-r--r--   0        0        0      103 2024-04-12 12:55:33.188757 preliz-0.5.0/preliz/tests/test_quartile_int.py
+-rw-r--r--   0        0        0      910 2024-04-12 12:55:33.188757 preliz-0.5.0/preliz/tests/test_roulette.py
+-rw-r--r--   0        0        0     7665 2024-04-12 12:55:33.188757 preliz-0.5.0/preliz/tests/test_scipy.py
+-rw-r--r--   0        0        0     1595 2024-04-12 12:55:33.188757 preliz-0.5.0/preliz/tests/test_special.py
+-rw-r--r--   0        0        0     2589 2024-04-12 12:55:33.188757 preliz-0.5.0/preliz/tests/test_truncated.py
+-rw-r--r--   0        0        0      325 2024-04-12 12:55:33.188757 preliz-0.5.0/preliz/unidimensional/__init__.py
+-rw-r--r--   0        0        0     2244 2024-04-12 12:55:33.188757 preliz-0.5.0/preliz/unidimensional/beta_mode.py
+-rw-r--r--   0        0        0     2341 2024-04-12 12:55:33.188757 preliz-0.5.0/preliz/unidimensional/dirichlet_mode.py
+-rw-r--r--   0        0        0     4125 2024-04-12 12:55:33.188757 preliz-0.5.0/preliz/unidimensional/maxent.py
+-rw-r--r--   0        0        0     1654 2024-04-12 12:55:33.188757 preliz-0.5.0/preliz/unidimensional/mle.py
+-rw-r--r--   0        0        0     3259 2024-04-12 12:55:33.188757 preliz-0.5.0/preliz/unidimensional/quartile.py
+-rw-r--r--   0        0        0     6136 2024-04-12 12:55:33.188757 preliz-0.5.0/preliz/unidimensional/quartile_int.py
+-rw-r--r--   0        0        0    12994 2024-04-12 12:55:33.188757 preliz-0.5.0/preliz/unidimensional/roulette.py
+-rw-r--r--   0        0        0     1410 2024-04-12 12:55:33.188757 preliz-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     5568 1970-01-01 00:00:00.000000 preliz-0.5.0/PKG-INFO
```

### Comparing `preliz-0.4.1/README.md` & `preliz-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `preliz-0.4.1/preliz/__init__.py` & `preliz-0.5.0/preliz/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from .distributions import *
 from .predictive import *
 from .unidimensional import *
 
 
 __all__ = ["maxent", "mle", "ppa", "roulette", "quartile"]
 
-__version__ = "0.4.1"
+__version__ = "0.5.0"
 
 _log = logging.getLogger("preliz")
 
 if not logging.root.handlers:
     _log.setLevel(logging.INFO)
     if len(_log.handlers) == 0:
         handler = logging.StreamHandler()
```

### Comparing `preliz-0.4.1/preliz/distributions/__init__.py` & `preliz-0.5.0/preliz/distributions/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from .continuous import *
 from .discrete import *
 from .continuous_multivariate import *
+from .truncated import Truncated
+from .censored import Censored
 
 all_continuous = [
     AsymmetricLaplace,
     Beta,
     BetaScaled,
     Cauchy,
     ChiSquared,
@@ -53,8 +55,10 @@
 all_continuous_multivariate = [Dirichlet, MvNormal]
 
 
 __all__ = (
     [s.__name__ for s in all_continuous]
     + [s.__name__ for s in all_discrete]
     + [s.__name__ for s in all_continuous_multivariate]
+    + [Truncated.__name__]
+    + [Censored.__name__]
 )
```

### Comparing `preliz-0.4.1/preliz/distributions/asymmetric_laplace.py` & `preliz-0.5.0/preliz/distributions/asymmetric_laplace.py`

 * *Files 3% similar despite different names*

```diff
@@ -161,15 +161,15 @@
 
     def skewness(self):
         return 2.0 * (1 - np.power(self.kappa, 6)) / np.power(1 + np.power(self.kappa, 4), 1.5)
 
     def kurtosis(self):
         return 6.0 * (1 + np.power(self.kappa, 8)) / np.power(1 + np.power(self.kappa, 4), 2)
 
-    def rvs(self, size=1, random_state=None):
+    def rvs(self, size=None, random_state=None):
         random_state = np.random.default_rng(random_state)
         random_samples = random_state.uniform(
             -self.kappa, 1 / self.kappa, size  # pylint: disable=invalid-unary-operand-type
         )
         return nb_rvs(random_samples, self.mu, self.b, self.kappa)
 
     def _fit_moments(self, mean, sigma):
@@ -179,64 +179,64 @@
         self._update(1, mu, b)
 
     def _fit_mle(self, sample, **kwargs):
         kappa, mu, b = nb_fit_mle(sample)
         self._update(kappa, mu, b)
 
 
-@nb.vectorize(nopython=True)
+@nb.vectorize(nopython=True, cache=True)
 def nb_cdf(x, mu, b, kappa):
     x = (x - mu) / b
     kap_inv = 1 / kappa
     kap_kapinv = kappa + kap_inv
     if x >= 0:
         return 1 - np.exp(-x * kappa) * (kap_inv / kap_kapinv)
     return np.exp(x * kap_inv) * (kappa / kap_kapinv)
 
 
-@nb.vectorize(nopython=True)
+@nb.vectorize(nopython=True, cache=True)
 def nb_ppf(q, mu, b, kappa):
     kap_inv = 1 / kappa
     kap_kapinv = kappa + kap_inv
     if q >= kappa / kap_kapinv:
         q_ppf = -np.log((1 - q) * kap_kapinv * kappa) * kap_inv
     else:
         q_ppf = np.log(q * kap_kapinv / kappa) * kappa
     return q_ppf * b + mu
 
 
-@nb.vectorize(nopython=True)
+@nb.vectorize(nopython=True, cache=True)
 def nb_logpdf(x, mu, b, kappa):
     x = (x - mu) / b
     kap_inv = 1 / kappa
     if x >= 0:
         ald_x = x * -kappa
     else:
         ald_x = x * kap_inv
     ald_x -= np.log(kappa + kap_inv)
     return ald_x - np.log(b)
 
 
-@nb.njit
+@nb.njit(cache=True)
 def nb_neg_logpdf(x, mu, b, kappa):
     return (-nb_logpdf(x, mu, b, kappa)).sum()
 
 
-@nb.njit
+@nb.njit(cache=True)
 def nb_rvs(random_samples, mu, b, kappa):
     sgn = np.sign(random_samples)
     return mu - (1 / (1 / b * sgn * kappa**sgn)) * np.log(1 - random_samples * sgn * kappa**sgn)
 
 
-@nb.njit
+@nb.njit(cache=True)
 def nb_entropy(b, kappa):
     return 1 + np.log(kappa + 1 / kappa) + np.log(b)
 
 
-@nb.njit
+@nb.njit(cache=True)
 def nb_fit_mle(sample):
     new_mu = np.median(sample)
     new_b = np.mean(np.abs(sample - new_mu))
     new_kappa = np.sum((sample - new_mu) * np.sign(sample - new_mu)) / np.sum(
         np.abs(sample - new_mu)
     )
     return new_kappa, new_mu, new_b
```

### Comparing `preliz-0.4.1/preliz/distributions/bernoulli.py` & `preliz-0.5.0/preliz/distributions/bernoulli.py`

 * *Files 4% similar despite different names*

```diff
@@ -145,65 +145,65 @@
 
     def skewness(self):
         return (self._q - self.p) / self.std()
 
     def kurtosis(self):
         return (1 - 6 * self.p * self._q) / (self.p * self._q)
 
-    def rvs(self, size=1, random_state=None):
+    def rvs(self, size=None, random_state=None):
         random_state = np.random.default_rng(random_state)
         return random_state.binomial(1, self.p, size=size)
 
 
-@nb.vectorize(nopython=True)
+@nb.vectorize(nopython=True, cache=True)
 def nb_cdf(x, p):
     if x < 0:
         return 0
     elif x < 1:
         return 1 - p
     else:
         return 1
 
 
-@nb.vectorize(nopython=True)
+@nb.vectorize(nopython=True, cache=True)
 def nb_ppf(q, p):
     if q < 0:
         return np.nan
     elif q > 1:
         return np.nan
     elif q == 0:
         return -1
     elif q < 1 - p:
         return 0
     else:
         return 1
 
 
-@nb.vectorize(nopython=True)
+@nb.vectorize(nopython=True, cache=True)
 def nb_pdf(x, p):
     if x == 1:
         return p
     elif x == 0:
         return 1 - p
     else:
         return 0.0
 
 
-@nb.njit
+@nb.njit(cache=True)
 def nb_entropy(p):
     q = 1 - p
     return -q * np.log(q) - p * np.log(p)
 
 
-@nb.vectorize(nopython=True)
+@nb.vectorize(nopython=True, cache=True)
 def nb_logpdf(x, p):
     if x == 1:
         return np.log(p)
     elif x == 0:
         return np.log(1 - p)
     else:
         return -np.inf
 
 
-@nb.njit
+@nb.njit(cache=True)
 def nb_neg_logpdf(x, p):
     return -(nb_logpdf(x, p)).sum()
```

### Comparing `preliz-0.4.1/preliz/distributions/beta.py` & `preliz-0.5.0/preliz/distributions/beta.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 # pylint: disable=attribute-defined-outside-init
 # pylint: disable=arguments-differ
 import numba as nb
 import numpy as np
-from scipy.special import betainc, betaincinv  # pylint: disable=no-name-in-module
 
 from .distributions import Continuous
 from ..internal.distribution_helper import eps, any_not_none, all_not_none
 from ..internal.optimization import optimize_ml
-from ..internal.special import betaln, digamma, gammaln, cdf_bounds, ppf_bounds_cont, mean_and_std
+from ..internal.special import (
+    betaln,
+    betainc,
+    betaincinv,
+    digamma,
+    gammaln,
+    cdf_bounds,
+    ppf_bounds_cont,
+    mean_and_std,
+)
 
 
 class Beta(Continuous):
     r"""
     Beta distribution.
 
     The pdf of this distribution is
@@ -36,51 +44,47 @@
     ========  ==============================================================
     Support   :math:`x \in (0, 1)`
     Mean      :math:`\dfrac{\alpha}{\alpha + \beta}`
     Variance  :math:`\dfrac{\alpha \beta}{(\alpha+\beta)^2(\alpha+\beta+1)}`
     ========  ==============================================================
 
     Beta distribution has 3 alternative parameterizations. In terms of alpha and
-    beta, mean and sigma (standard deviation) or mean and kappa (concentration).
+    beta, mean and sigma (standard deviation) or mean and nu (concentration).
 
     The link between the 3 alternatives is given by
 
     .. math::
 
-       \alpha &= \mu \kappa \\
-       \beta  &= (1 - \mu) \kappa
+       \alpha &= \mu \nu \\
+       \beta  &= (1 - \mu) \nu
 
-       \text{where } \kappa = \frac{\mu(1-\mu)}{\sigma^2} - 1
+       \text{where } \nu = \frac{\mu(1-\mu)}{\sigma^2} - 1
 
 
     Parameters
     ----------
     alpha : float
         alpha  > 0
     beta : float
         beta  > 0
     mu : float
         mean (0 < ``mu`` < 1).
     sigma : float
         standard deviation (``sigma`` < sqrt(``mu`` * (1 - ``mu``))).
-    kappa : float
+    nu : float
         concentration > 0
     """
 
-    def __init__(self, alpha=None, beta=None, mu=None, sigma=None, kappa=None):
+    def __init__(self, alpha=None, beta=None, mu=None, sigma=None, nu=None):
         super().__init__()
         self.support = (0, 1)
-        self._parametrization(alpha, beta, mu, sigma, kappa)
+        self._parametrization(alpha, beta, mu, sigma, nu)
 
-    def _parametrization(self, alpha=None, beta=None, mu=None, sigma=None, kappa=None):
-        if (
-            any_not_none(alpha, beta)
-            and any_not_none(mu, sigma, kappa)
-            or all_not_none(sigma, kappa)
-        ):
+    def _parametrization(self, alpha=None, beta=None, mu=None, sigma=None, nu=None):
+        if any_not_none(alpha, beta) and any_not_none(mu, sigma, nu) or all_not_none(sigma, nu):
             raise ValueError(
                 "Incompatible parametrization. Either use alpha and beta, or mu and sigma."
             )
 
         self.param_names = ("alpha", "beta")
         self.params_support = ((eps, np.inf), (eps, np.inf))
 
@@ -88,76 +92,78 @@
             self.mu = mu
             self.sigma = sigma
             self.param_names = ("mu", "sigma")
             self.params_support = ((eps, 1 - eps), (eps, 1 - eps))
             if all_not_none(mu, sigma):
                 alpha, beta = self._from_mu_sigma(mu, sigma)
 
-        if any_not_none(mu, kappa) and sigma is None:
+        if any_not_none(mu, nu) and sigma is None:
             self.mu = mu
-            self.kappa = kappa
-            self.param_names = ("mu", "kappa")
+            self.nu = nu
+            self.param_names = ("mu", "nu")
             self.params_support = ((eps, 1 - eps), (eps, np.inf))
-            if all_not_none(mu, kappa):
-                alpha, beta = self._from_mu_kappa(mu, kappa)
+            if all_not_none(mu, nu):
+                alpha, beta = self._from_mu_nu(mu, nu)
 
         self.alpha = alpha
         self.beta = beta
         if all_not_none(self.alpha, self.beta):
             self._update(self.alpha, self.beta)
 
     def _from_mu_sigma(self, mu, sigma):
-        kappa = mu * (1 - mu) / sigma**2 - 1
-        alpha = mu * kappa
-        beta = (1 - mu) * kappa
+        nu = mu * (1 - mu) / sigma**2 - 1
+        alpha = mu * nu
+        beta = (1 - mu) * nu
         return alpha, beta
 
-    def _from_mu_kappa(self, mu, kappa):
-        alpha = mu * kappa
-        beta = (1 - mu) * kappa
+    def _from_mu_nu(self, mu, nu):
+        alpha = mu * nu
+        beta = (1 - mu) * nu
         return alpha, beta
 
     def _to_mu_sigma(self, alpha, beta):
         alpha_plus_beta = alpha + beta
         mu = alpha / alpha_plus_beta
         sigma = (alpha * beta) ** 0.5 / alpha_plus_beta / (alpha_plus_beta + 1) ** 0.5
         return mu, sigma
 
     def _update(self, alpha, beta):
         self.alpha = np.float64(alpha)
         self.beta = np.float64(beta)
         self.mu, self.sigma = self._to_mu_sigma(self.alpha, self.beta)
-        self.kappa = self.mu * (1 - self.mu) / self.sigma**2 - 1
+        self.nu = self.mu * (1 - self.mu) / self.sigma**2 - 1
 
         if self.param_names[0] == "alpha":
             self.params = (self.alpha, self.beta)
         elif self.param_names[1] == "sigma":
             self.params = (self.mu, self.sigma)
-        elif self.param_names[1] == "kappa":
-            self.params = (self.mu, self.kappa)
+        elif self.param_names[1] == "nu":
+            self.params = (self.mu, self.nu)
 
         self.is_frozen = True
 
     def pdf(self, x):
         """
         Compute the probability density function (PDF) at a given point x.
         """
         x = np.asarray(x)
         return np.exp(nb_logpdf(x, self.alpha, self.beta))
 
     def cdf(self, x):
         """
         Compute the cumulative distribution function (CDF) at a given point x.
         """
+        x = np.asarray(x)
         return nb_cdf(x, self.alpha, self.beta, self.support[0], self.support[1])
 
     def ppf(self, q):
         """
         Compute the percent point function (PPF) at a given probability q.
         """
+        q = np.asarray(q)
         return nb_ppf(q, self.alpha, self.beta, self.support[0], self.support[1])
 
     def logpdf(self, x):
         """
         Compute the log probability density function (log PDF) at a given point x.
         """
         return nb_logpdf(x, self.alpha, self.beta)
@@ -199,15 +205,15 @@
         prod = self.alpha * self.beta
         return (
             6
             * (np.abs(self.alpha - self.beta) ** 2 * (psc + 1) - prod * (psc + 2))
             / (prod * (psc + 2) * (psc + 3))
         )
 
-    def rvs(self, size=1, random_state=None):
+    def rvs(self, size=None, random_state=None):
         random_state = np.random.default_rng(random_state)
         return random_state.beta(self.alpha, self.beta, size)
 
     def _fit_moments(self, mean, sigma):
         alpha, beta = self._from_mu_sigma(mean, sigma)
         alpha = max(0.5, alpha)
         beta = max(0.5, beta)
@@ -215,42 +221,39 @@
 
     def _fit_mle(self, sample):
         mean, std = mean_and_std(sample)
         self._fit_moments(mean, std)
         optimize_ml(self, sample)
 
 
-# @nb.jit
-# betainc not supported by numba
+@nb.njit(cache=True)
 def nb_cdf(x, alpha, beta, lower, upper):
     prob = betainc(alpha, beta, x)
     return cdf_bounds(prob, x, lower, upper)
 
 
-# @nb.jit
-# betaincinv not supported by numba
+@nb.njit(cache=True)
 def nb_ppf(q, alpha, beta, lower, upper):
-    q = np.asarray(q)
     x_val = betaincinv(alpha, beta, q)
     return ppf_bounds_cont(x_val, q, lower, upper)
 
 
-@nb.njit
+@nb.njit(cache=True)
 def nb_entropy(alpha, beta):
     psc = alpha + beta
     return (
         betaln(alpha, beta)
         - (alpha - 1) * digamma(alpha)
         - (beta - 1) * digamma(beta)
         + (psc - 2) * digamma(psc)
     )
 
 
-@nb.njit
+@nb.njit(cache=True)
 def nb_logpdf(x, alpha, beta):
     beta_ = gammaln(alpha) + gammaln(beta) - gammaln(alpha + beta)
     return (alpha - 1) * np.log(x) + (beta - 1) * np.log(1 - x) - beta_
 
 
-@nb.njit
+@nb.njit(cache=True)
 def nb_neg_logpdf(x, alpha, beta):
     return -(nb_logpdf(x, alpha, beta)).sum()
```

### Comparing `preliz-0.4.1/preliz/distributions/binomial.py` & `preliz-0.5.0/preliz/distributions/binomial.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 
     def skewness(self):
         return (self._q - self.p) / self.std()
 
     def kurtosis(self):
         return (1 - 6 * self.p * self._q) / (self.n * self.p * self._q)
 
-    def rvs(self, size=1, random_state=None):
+    def rvs(self, size=None, random_state=None):
         random_state = np.random.default_rng(random_state)
         return random_state.binomial(self.n, self.p, size=size)
 
     def _fit_moments(self, mean, sigma):
         # crude approximation for n and p
         n = mean + sigma * 2
         p = mean / n
@@ -157,35 +157,35 @@
 # @nb.jit
 def nb_ppf(q, n, p, lower, upper):
     q = np.asarray(q)
     x_vals = np.ceil(bdtrik(q, n, p))
     return ppf_bounds_disc(x_vals, q, lower, upper)
 
 
-@nb.njit
+@nb.njit(cache=True)
 def nb_entropy(n, p):
     return 0.5 * np.log(2 * np.pi * np.e * n * p * (1 - p))
 
 
-@nb.njit
+@nb.njit(cache=True)
 def nb_fit_mle(sample):
     # see https://doi.org/10.1016/j.jspi.2004.02.019 for details
     x_bar, x_std = mean_and_std(sample)
     x_max = np.max(sample)
     n = np.ceil(x_max ** (1.5) * x_std / (x_bar**0.5 * (x_max - x_bar) ** 0.5))
     p = x_bar / n
     return n, p
 
 
-@nb.njit
+@nb.njit(cache=True)
 def nb_logpdf(n, y, p):
     return (
         gammaln(n + 1)
         - (gammaln(y + 1) + gammaln(n - y + 1))
         + y * np.log(p)
         + (n - y) * np.log1p(-p)
     )
 
 
-@nb.njit
+@nb.njit(cache=True)
 def nb_neg_logpdf(n, y, p):
     return -(nb_logpdf(n, y, p)).sum()
```

### Comparing `preliz-0.4.1/preliz/distributions/continuous.py` & `preliz-0.5.0/preliz/distributions/continuous.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,40 @@
 # pylint: disable=too-many-lines
 # pylint: disable=too-many-instance-attributes
 # pylint: disable=invalid-name
 # pylint: disable=attribute-defined-outside-init
+# pylint: disable=unused-import
 """
 Continuous probability distributions.
 """
 from copy import copy
 
 import numpy as np
 from scipy import stats
-from scipy.special import gamma as gammaf
 from scipy.special import beta as betaf  # pylint: disable=no-name-in-module
 from scipy.special import logit, expit  # pylint: disable=no-name-in-module
 
 from ..internal.optimization import optimize_ml, optimize_moments, optimize_moments_rice
 from ..internal.distribution_helper import all_not_none, any_not_none
 from .distributions import Continuous
-from .asymmetric_laplace import AsymmetricLaplace  # pylint: disable=unused-import
-from .beta import Beta  # pylint: disable=unused-import
-from .exponential import Exponential  # pylint: disable=unused-import
-from .normal import Normal  # pylint: disable=unused-import
-from .halfnormal import HalfNormal  # pylint: disable=unused-import
-from .laplace import Laplace  # pylint: disable=unused-import
-from .weibull import Weibull  # pylint: disable=unused-import
+from .asymmetric_laplace import AsymmetricLaplace
+from .beta import Beta
+from .exponential import Exponential
+from .gamma import Gamma
+from .inversegamma import InverseGamma
+from .normal import Normal
+from .halfnormal import HalfNormal
+from .halfstudentt import HalfStudentT
+from .laplace import Laplace
+from .studentt import StudentT
+from .triangular import Triangular
+from .uniform import Uniform
+from .vonmises import VonMises
+from .wald import Wald
+from .weibull import Weibull
 
 
 eps = np.finfo(float).eps
 
 
 def from_precision(precision):
     sigma = 1 / precision**0.5
@@ -352,131 +360,14 @@
         self._update(mean, sigma, 1e-4)
 
     def _fit_mle(self, sample, **kwargs):
         K, mu, sigma = self.dist.fit(sample, **kwargs)
         self._update(mu, sigma, K * sigma)
 
 
-class Gamma(Continuous):
-    r"""
-    Gamma distribution.
-
-    Represents the sum of alpha exponentially distributed random variables,
-    each of which has rate beta.
-
-    The pdf of this distribution is
-
-    .. math::
-
-       f(x \mid \alpha, \beta) =
-           \frac{\beta^{\alpha}x^{\alpha-1}e^{-\beta x}}{\Gamma(\alpha)}
-
-    .. plot::
-        :context: close-figs
-
-        import arviz as az
-        from preliz import Gamma
-        az.style.use('arviz-doc')
-        alphas = [1., 3., 7.5]
-        betas = [.5, 1., 1.]
-        for alpha, beta in zip(alphas, betas):
-            Gamma(alpha, beta).plot_pdf()
-
-    ========  ===============================
-    Support   :math:`x \in (0, \infty)`
-    Mean      :math:`\dfrac{\alpha}{\beta}`
-    Variance  :math:`\dfrac{\alpha}{\beta^2}`
-    ========  ===============================
-
-    Gamma distribution has 2 alternative parameterizations. In terms of alpha and
-    beta or mu (mean) and sigma (standard deviation).
-
-    The link between the 2 alternatives is given by
-
-    .. math::
-
-       \alpha &= \frac{\mu^2}{\sigma^2} \\
-       \beta  &= \frac{\mu}{\sigma^2}
-
-    Parameters
-    ----------
-    alpha : float
-        Shape parameter (alpha > 0).
-    beta : float
-        Rate parameter (beta > 0).
-    mu : float
-        Mean (mu > 0).
-    sigma : float
-        Standard deviation (sigma > 0)
-    """
-
-    def __init__(self, alpha=None, beta=None, mu=None, sigma=None):
-        super().__init__()
-        self.dist = copy(stats.gamma)
-        self.support = (0, np.inf)
-        self._parametrization(alpha, beta, mu, sigma)
-
-    def _parametrization(self, alpha=None, beta=None, mu=None, sigma=None):
-        if any_not_none(alpha, beta) and any_not_none(mu, sigma):
-            raise ValueError(
-                "Incompatible parametrization. Either use alpha and beta or mu and sigma."
-            )
-
-        self.param_names = ("alpha", "beta")
-        self.params_support = ((eps, np.inf), (eps, np.inf))
-
-        if any_not_none(mu, sigma):
-            self.mu = mu
-            self.sigma = sigma
-            self.param_names = ("mu", "sigma")
-            if all_not_none(mu, sigma):
-                alpha, beta = self._from_mu_sigma(mu, sigma)
-
-        self.alpha = alpha
-        self.beta = beta
-        if all_not_none(self.alpha, self.beta):
-            self._update(self.alpha, self.beta)
-
-    def _from_mu_sigma(self, mu, sigma):
-        alpha = mu**2 / sigma**2
-        beta = mu / sigma**2
-        return alpha, beta
-
-    def _to_mu_sigma(self, alpha, beta):
-        mu = alpha / beta
-        sigma = alpha**0.5 / beta
-        return mu, sigma
-
-    def _get_frozen(self):
-        frozen = None
-        if all_not_none(self.params):
-            frozen = self.dist(a=self.alpha, scale=1 / self.beta)
-        return frozen
-
-    def _update(self, alpha, beta):
-        self.alpha = np.float64(alpha)
-        self.beta = np.float64(beta)
-        self.mu, self.sigma = self._to_mu_sigma(self.alpha, self.beta)
-
-        if self.param_names[0] == "alpha":
-            self.params = (self.alpha, self.beta)
-        elif self.param_names[1] == "sigma":
-            self.params = (self.mu, self.sigma)
-
-        self._update_rv_frozen()
-
-    def _fit_moments(self, mean, sigma):
-        alpha, beta = self._from_mu_sigma(mean, sigma)
-        self._update(alpha, beta)
-
-    def _fit_mle(self, sample, **kwargs):
-        alpha, _, beta = self.dist.fit(sample, **kwargs)
-        self._update(alpha, 1 / beta)
-
-
 class Gumbel(Continuous):
     r"""
     Gumbel distribution.
 
     The pdf of this distribution is
 
     .. math::
@@ -613,319 +504,14 @@
         self._update(beta)
 
     def _fit_mle(self, sample, **kwargs):
         _, beta = self.dist.fit(sample, **kwargs)
         self._update(beta)
 
 
-class HalfStudentT(Continuous):
-    r"""
-    HalfStudentT Distribution
-
-    The pdf of this distribution is
-
-    .. math::
-
-        f(x \mid \sigma,\nu) =
-            \frac{2\;\Gamma\left(\frac{\nu+1}{2}\right)}
-            {\Gamma\left(\frac{\nu}{2}\right)\sqrt{\nu\pi\sigma^2}}
-            \left(1+\frac{1}{\nu}\frac{x^2}{\sigma^2}\right)^{-\frac{\nu+1}{2}}
-
-    .. plot::
-        :context: close-figs
-
-        import arviz as az
-        from preliz import HalfStudentT
-        az.style.use('arviz-doc')
-        sigmas = [1., 2., 2.]
-        nus = [3, 3., 10.]
-        for sigma, nu in zip(sigmas, nus):
-            HalfStudentT(nu, sigma).plot_pdf(support=(0,10))
-
-    ========  ==========================================
-    Support   :math:`x \in [0, \infty)`
-    Mean      .. math::
-                  2\sigma\sqrt{\frac{\nu}{\pi}}\
-                  \frac{\Gamma\left(\frac{\nu+1}{2}\right)}\
-                  {\Gamma\left(\frac{\nu}{2}\right)(\nu-1)}\, \text{for } \nu > 2
-    Variance  .. math::
-                  \sigma^2\left(\frac{\nu}{\nu - 2}-\
-                  \frac{4\nu}{\pi(\nu-1)^2}\left(\frac{\Gamma\left(\frac{\nu+1}{2}\right)}\
-                  {\Gamma\left(\frac{\nu}{2}\right)}\right)^2\right) \text{for } \nu > 2\, \infty\
-                  \text{for } 1 < \nu \le 2\, \text{otherwise undefined}
-    ========  ==========================================
-
-    HalfStudentT distribution has 2 alternative parameterizations. In terms of nu and
-    sigma (standard deviation as nu increases) or nu lam (precision as nu increases).
-
-    The link between the 2 alternatives is given by
-
-    .. math::
-
-        \lambda = \frac{1}{\sigma^2}
-
-    Parameters
-    ----------
-    nu : float
-        Degrees of freedom, also known as normality parameter (nu > 0).
-    sigma : float
-        Scale parameter (sigma > 0). Converges to the standard deviation as nu
-        increases.
-    lam : float
-        Scale parameter (lam > 0). Converges to the precision as nu increases.
-    """
-
-    def __init__(self, nu=None, sigma=None, lam=None):
-        super().__init__()
-        self.dist = _HalfStudentT
-        self.support = (0, np.inf)
-        self._parametrization(nu, sigma, lam)
-
-    def _parametrization(self, nu=None, sigma=None, lam=None):
-        if all_not_none(sigma, lam):
-            raise ValueError(
-                "Incompatible parametrization. Either use nu and sigma, or nu and lam."
-            )
-
-        self.param_names = ("nu", "sigma")
-        self.params_support = ((eps, np.inf), (eps, np.inf))
-
-        if lam is not None:
-            self.lam = lam
-            sigma = from_precision(lam)
-            self.param_names = ("nu", "lam")
-
-        self.nu = nu
-        self.sigma = sigma
-        if all_not_none(self.nu, self.sigma):
-            self._update(self.nu, self.sigma)
-
-    def _get_frozen(self):
-        frozen = None
-        if all_not_none(self.params):
-            frozen = self.dist(nu=self.nu, sigma=self.sigma)
-        return frozen
-
-    def _update(self, nu, sigma):
-        self.nu = np.float64(nu)
-        self.sigma = np.float64(sigma)
-        self.lam = to_precision(sigma)
-
-        if self.param_names[1] == "sigma":
-            self.params = (self.nu, self.sigma)
-        elif self.param_names[1] == "lam":
-            self.params = (self.nu, self.lam)
-
-        self._update_rv_frozen()
-
-    def _fit_moments(self, mean, sigma):  # pylint: disable=unused-argument
-        # if nu is smaller than 2 the variance is not defined,
-        # so if that happens we use 2.1 as an approximation
-        nu = self.nu
-        if nu is None:
-            nu = 100
-        elif nu <= 2:
-            nu = 2.1
-
-        gamma0 = gammaf((nu + 1) / 2)
-        gamma1 = gammaf(nu / 2)
-        if np.isfinite(gamma0) and np.isfinite(gamma1):
-            sigma = (
-                sigma**2
-                / ((nu / (nu - 2)) - ((4 * nu) / (np.pi * (nu - 1) ** 2)) * (gamma0 / gamma1) ** 2)
-            ) ** 0.5
-        else:
-            # we assume a Gaussian for large nu
-            sigma = sigma / (1 - 2 / np.pi) ** 0.5
-        self._update(nu, sigma)
-
-    def _fit_mle(self, sample, **kwargs):
-        optimize_ml(self, sample)
-
-
-class _HalfStudentT(stats.rv_continuous):
-    def __init__(self, nu=None, sigma=None):
-        super().__init__()
-        self.nu = nu
-        self.sigma = sigma
-        self.dist = stats.t(loc=0, df=self.nu, scale=self.sigma)
-
-    def support(self, *args, **kwd):  # pylint: disable=unused-argument
-        return (0, np.inf)
-
-    def cdf(self, x, *args, **kwds):
-        return np.maximum(0, self.dist.cdf(x, *args, **kwds) * 2 - 1)
-
-    def pdf(self, x, *args, **kwds):
-        return np.where(x < 0, -np.inf, self.dist.pdf(x, *args, **kwds) * 2)
-
-    def logpdf(self, x, *args, **kwds):
-        return np.where(x < 0, -np.inf, self.dist.logpdf(x, *args, **kwds) + np.log(2))
-
-    def ppf(self, q, *args, **kwds):
-        x_vals = np.linspace(0, self.rvs(10000).max(), 1000)
-        idx = np.searchsorted(self.cdf(x_vals[:-1], *args, **kwds), q)
-        return x_vals[idx]
-
-    def _stats(self, *args, **kwds):  # pylint: disable=unused-argument
-        mean = np.nan
-        var = np.nan
-        skew = np.nan
-        kurtosis = np.nan
-
-        if self.nu > 1:
-            gamma0 = gammaf((self.nu + 1) / 2)
-            gamma1 = gammaf(self.nu / 2)
-            if np.isfinite(gamma0) and np.isfinite(gamma1):
-                mean = (
-                    2 * self.sigma * (self.nu / np.pi) ** 0.5 * (gamma0 / (gamma1 * (self.nu - 1)))
-                )
-            else:
-                # assume nu is large enough that the mean of the halfnormal is a good approximation
-                mean = self.sigma * (2 / np.pi) ** 0.5
-        if self.nu > 2:
-            if np.isfinite(gamma0) and np.isfinite(gamma1):
-                var = self.sigma**2 * (
-                    (self.nu / (self.nu - 2))
-                    - ((4 * self.nu) / (np.pi * (self.nu - 1) ** 2)) * (gamma0 / gamma1) ** 2
-                )
-            else:
-                # assume nu is large enough that the std of the halfnormal is a good approximation
-                var = self.sigma**2 * (1 - 2.0 / np.pi)
-
-        return (mean, var, skew, kurtosis)
-
-    def entropy(self):  # pylint: disable=arguments-differ
-        return self.dist.entropy() - np.log(2)
-
-    def rvs(self, size=1, random_state=None):  # pylint: disable=arguments-differ
-        return np.abs(self.dist.rvs(size=size, random_state=random_state))
-
-
-class InverseGamma(Continuous):
-    r"""
-    Inverse gamma distribution, the reciprocal of the gamma distribution.
-
-    The pdf of this distribution is
-
-    .. math::
-
-       f(x \mid \alpha, \beta) =
-           \frac{\beta^{\alpha}}{\Gamma(\alpha)} x^{-\alpha - 1}
-           \exp\left(\frac{-\beta}{x}\right)
-
-    .. plot::
-        :context: close-figs
-
-        import arviz as az
-        from preliz import InverseGamma
-        az.style.use('arviz-doc')
-        alphas = [1., 2., 3.]
-        betas = [1., 1., .5]
-        for alpha, beta in zip(alphas, betas):
-            InverseGamma(alpha, beta).plot_pdf(support=(0, 3))
-
-    ========  ===============================
-    Support   :math:`x \in (0, \infty)`
-    Mean      :math:`\dfrac{\beta}{\alpha-1}` for :math:`\alpha > 1`
-    Variance  :math:`\dfrac{\beta^2}{(\alpha-1)^2(\alpha - 2)}` for :math:`\alpha > 2`
-    ========  ===============================
-
-    Inverse gamma distribution has 2 alternative parameterizations. In terms of alpha and
-    beta or mu (mean) and sigma (standard deviation).
-
-    The link between the 2 alternatives is given by
-
-    .. math::
-
-       \alpha &= \frac{\mu^2}{\sigma^2} + 2 \\
-       \beta  &= \frac{\mu^3}{\sigma^2} + \mu
-
-    Parameters
-    ----------
-    alpha : float
-        Shape parameter (alpha > 0).
-    beta : float
-        Scale parameter (beta > 0).
-    mu : float
-        Mean (mu > 0).
-    sigma : float
-        Standard deviation (sigma > 0)
-    """
-
-    def __init__(self, alpha=None, beta=None, mu=None, sigma=None):
-        super().__init__()
-        self.dist = copy(stats.invgamma)
-        self.support = (0, np.inf)
-        self._parametrization(alpha, beta, mu, sigma)
-
-    def _parametrization(self, alpha=None, beta=None, mu=None, sigma=None):
-        if any_not_none(alpha, beta) and any_not_none(mu, sigma):
-            raise ValueError(
-                "Incompatible parametrization. Either use alpha and beta or mu and sigma."
-            )
-
-        self.param_names = ("alpha", "beta")
-        self.params_support = ((eps, np.inf), (eps, np.inf))
-
-        if any_not_none(mu, sigma):
-            self.mu = mu
-            self.sigma = sigma
-            self.param_names = ("mu", "sigma")
-            if all_not_none(mu, sigma):
-                alpha, beta = self._from_mu_sigma(mu, sigma)
-
-        self.alpha = alpha
-        self.beta = beta
-        if all_not_none(self.alpha, self.beta):
-            self._update(self.alpha, self.beta)
-
-    def _from_mu_sigma(self, mu, sigma):
-        alpha = mu**2 / sigma**2 + 2
-        beta = mu**3 / sigma**2 + mu
-        return alpha, beta
-
-    def _to_mu_sigma(self, alpha, beta):
-        if alpha > 1:
-            mu = beta / (alpha - 1)
-        else:
-            mu = None
-        if alpha > 2:
-            sigma = beta / ((alpha - 1) * (alpha - 2) ** 0.5)
-        else:
-            sigma = None
-        return mu, sigma
-
-    def _get_frozen(self):
-        frozen = None
-        if all_not_none(self.params):
-            frozen = self.dist(a=self.alpha, scale=self.beta)
-        return frozen
-
-    def _update(self, alpha, beta):
-        self.alpha = np.float64(alpha)
-        self.beta = np.float64(beta)
-        self.mu, self.sigma = self._to_mu_sigma(self.alpha, self.beta)
-
-        if self.param_names[0] == "alpha":
-            self.params = (self.alpha, self.beta)
-        elif self.param_names[1] == "sigma":
-            self.params = (self.mu, self.sigma)
-
-        self._update_rv_frozen()
-
-    def _fit_moments(self, mean, sigma):
-        alpha, beta = self._from_mu_sigma(mean, sigma)
-        self._update(alpha, beta)
-
-    def _fit_mle(self, sample, **kwargs):
-        alpha, _, beta = self.dist.fit(sample, **kwargs)
-        self._update(alpha, beta)
-
-
 class Kumaraswamy(Continuous):
     r"""
     Kumaraswamy distribution.
 
     The pdf of this distribution is
 
     .. math::
@@ -1714,226 +1300,14 @@
         self._update(mean, sigma, 0)
 
     def _fit_mle(self, sample, **kwargs):
         alpha, mu, sigma = self.dist.fit(sample, **kwargs)
         self._update(mu, sigma, alpha)
 
 
-class StudentT(Continuous):
-    r"""
-    StudentT's distribution.
-
-    Describes a normal variable whose precision is gamma distributed.
-
-    The pdf of this distribution is
-
-    .. math::
-
-       f(x \mid \nu, \mu, \sigma) =
-           \frac{\Gamma \left(\frac{\nu+1}{2} \right)} {\sqrt{\nu\pi}\
-           \Gamma \left(\frac{\nu}{2} \right)} \left(1+\frac{x^2}{\nu} \right)^{-\frac{\nu+1}{2}}
-
-    .. plot::
-        :context: close-figs
-
-        import arviz as az
-        from preliz import StudentT
-        az.style.use('arviz-doc')
-        nus = [2., 5., 5.]
-        mus = [0., 0.,  -4.]
-        sigmas = [1., 1., 2.]
-        for nu, mu, sigma in zip(nus, mus, sigmas):
-            StudentT(nu, mu, sigma).plot_pdf(support=(-10,6))
-
-    ========  ========================
-    Support   :math:`x \in \mathbb{R}`
-    Mean      :math:`\mu` for :math:`\nu > 1`, otherwise undefined
-    Variance  :math:`\frac{\nu}{\nu-2}` for :math:`\nu > 2`,
-              :math:`\infty` for :math:`1 < \nu \le 2`, otherwise undefined
-    ========  ========================
-
-    StudentT distribution has 2 alternative parameterizations. In terms of nu, mu and
-    sigma (standard deviation as nu increases) or nu, mu and lam (precision as nu increases).
-
-    The link between the 2 alternatives is given by
-
-    .. math::
-
-        \lambda = \frac{1}{\sigma^2}
-
-    Parameters
-    ----------
-    nu : float
-        Degrees of freedom, also known as normality parameter (nu > 0).
-    mu : float
-        Location parameter.
-    sigma : float
-        Scale parameter (sigma > 0). Converges to the standard deviation as nu
-        increases.
-    lam : float
-        Scale parameter (lam > 0). Converges to the precision as nu increases.
-    """
-
-    def __init__(self, nu=None, mu=None, sigma=None, lam=None):
-        super().__init__()
-        self.dist = copy(stats.t)
-        self.support = (-np.inf, np.inf)
-        self.params_support = ((eps, np.inf), (-np.inf, np.inf), (eps, np.inf))
-        self._parametrization(nu, mu, sigma, lam)
-
-    def _parametrization(self, nu=None, mu=None, sigma=None, lam=None):
-        if all_not_none(sigma, lam):
-            raise ValueError(
-                "Incompatible parametrization. Either use nu, mu and sigma, or nu, mu and lam."
-            )
-
-        self.param_names = ("nu", "mu", "sigma")
-        self.params_support = ((eps, np.inf), (-np.inf, np.inf), (eps, np.inf))
-
-        if lam is not None:
-            self.lam = lam
-            sigma = from_precision(lam)
-            self.param_names = ("nu", "mu", "lam")
-
-        self.nu = nu
-        self.mu = mu
-        self.sigma = sigma
-
-        if all_not_none(self.nu, self.mu, self.sigma):
-            self._update(self.nu, self.mu, self.sigma)
-
-    def _get_frozen(self):
-        frozen = None
-        if all_not_none(self.params):
-            frozen = self.dist(self.nu, self.mu, self.sigma)
-        return frozen
-
-    def _update(self, nu, mu, sigma):
-        self.nu = np.float64(nu)
-        self.mu = np.float64(mu)
-        self.sigma = np.float64(sigma)
-        self.lam = to_precision(sigma)
-
-        if self.param_names[2] == "sigma":
-            self.params = (self.nu, self.mu, self.sigma)
-        elif self.param_names[2] == "lam":
-            self.params = (self.nu, self.mu, self.lam)
-
-        self._update_rv_frozen()
-
-    def _fit_moments(self, mean, sigma):
-        # if nu is smaller than 2 the variance is not defined,
-        # so if that happens we use 2.1 as an approximation
-        nu = self.nu
-        if nu is None:
-            nu = 100
-        elif nu <= 2:
-            nu = 2.1
-        else:
-            sigma = sigma / (nu / (nu - 2)) ** 0.5
-
-        self._update(nu, mean, sigma)
-
-    def _fit_mle(self, sample, **kwargs):
-        nu, mu, sigma = self.dist.fit(sample, **kwargs)
-        self._update(nu, mu, sigma)
-
-
-class Triangular(Continuous):
-    r"""
-    Triangular distribution
-
-    The pdf of this distribution is
-
-    .. math::
-
-       \begin{cases}
-         0 & \text{for } x < a, \\
-         \frac{2(x-a)}{(b-a)(c-a)} & \text{for } a \le x < c, \\[4pt]
-         \frac{2}{b-a}             & \text{for } x = c, \\[4pt]
-         \frac{2(b-x)}{(b-a)(b-c)} & \text{for } c < x \le b, \\[4pt]
-         0 & \text{for } b < x.
-        \end{cases}
-
-    .. plot::
-        :context: close-figs
-
-        import arviz as az
-        from preliz import Triangular
-        az.style.use('arviz-doc')
-        lowers = [0., -1, 2]
-        cs = [2., 0., 6.5]
-        uppers = [4., 1, 8]
-        for lower, c, upper in zip(lowers, cs, uppers):
-            scale = upper - lower
-            c_ = (c - lower) / scale
-            Triangular(lower, c, upper).plot_pdf()
-
-    ========  ============================================================================
-    Support   :math:`x \in [lower, upper]`
-    Mean      :math:`\dfrac{lower + upper + c}{3}`
-    Variance  :math:`\dfrac{upper^2 + lower^2 +c^2 - lower*upper - lower*c - upper*c}{18}`
-    ========  ============================================================================
-
-    Parameters
-    ----------
-    lower : float
-        Lower limit.
-    c : float
-        Mode.
-    upper : float
-        Upper limit.
-    """
-
-    def __init__(self, lower=None, c=None, upper=None):
-        super().__init__()
-        self.dist = copy(stats.triang)
-        self.support = (-np.inf, np.inf)
-        self._parametrization(lower, c, upper)
-
-    def _parametrization(self, lower=None, c=None, upper=None):
-        self.lower = lower
-        self.c = c
-        self.upper = upper
-        self.params = (self.lower, self.c, self.upper)
-        self.param_names = ("lower", "c", "upper")
-        self.params_support = ((-np.inf, np.inf), (-np.inf, np.inf), (-np.inf, np.inf))
-        if all_not_none(lower, c, upper):
-            self._update(lower, c, upper)
-
-    def _get_frozen(self):
-        frozen = None
-        if all_not_none(self.params):
-            scale = self.upper - self.lower
-            c_ = (self.c - self.lower) / scale
-            frozen = self.dist(c=c_, loc=self.lower, scale=scale)
-        return frozen
-
-    def _update(self, lower, c, upper):
-        self.lower = np.float64(lower)
-        self.c = np.float64(c)
-        self.upper = np.float64(upper)
-        self.support = (self.lower, self.upper)
-        self.params = (self.lower, self.c, self.upper)
-        self._update_rv_frozen()
-
-    def _fit_moments(self, mean, sigma):
-        # Assume symmetry
-        lower = mean - 6**0.5 * sigma
-        upper = mean + 6**0.5 * sigma
-        c = mean
-        self._update(lower, c, upper)
-
-    def _fit_mle(self, sample, **kwargs):
-        c_, lower, scale = self.dist.fit(sample, **kwargs)
-        upper = scale + lower
-        c = c_ * scale + lower
-        self._update(lower, c, upper)
-
-
 class TruncatedNormal(Continuous):
     r"""
     TruncatedNormal distribution.
 
     The pdf of this distribution is
 
     .. math::
@@ -2042,284 +1416,7 @@
 
         if np.isfinite(beta):
             b_pdf = beta * norm.pdf(beta)
         else:
             b_pdf = 0
 
         return np.log(4.132731354122493 * zed * self.sigma) + (a_pdf - b_pdf) / (2 * zed)
-
-
-class Uniform(Continuous):
-    r"""
-    Uniform distribution.
-
-    The pdf of this distribution is
-
-    .. math:: f(x \mid lower, upper) = \frac{1}{upper-lower}
-
-    .. plot::
-        :context: close-figs
-
-        import arviz as az
-        from preliz import Uniform
-        az.style.use('arviz-doc')
-        ls = [1, -2]
-        us = [6, 2]
-        for l, u in zip(ls, us):
-            ax = Uniform(l, u).plot_pdf()
-        ax.set_ylim(0, 0.3)
-
-    ========  =====================================
-    Support   :math:`x \in [lower, upper]`
-    Mean      :math:`\dfrac{lower + upper}{2}`
-    Variance  :math:`\dfrac{(upper - lower)^2}{12}`
-    ========  =====================================
-
-    Parameters
-    ----------
-    lower: float
-        Lower limit.
-    upper: float
-        Upper limit (upper > lower).
-    """
-
-    def __init__(self, lower=None, upper=None):
-        super().__init__()
-        self.dist = copy(stats.uniform)
-        self._parametrization(lower, upper)
-
-    def _parametrization(self, lower=None, upper=None):
-        self.lower = lower
-        self.upper = upper
-        self.params = (self.lower, self.upper)
-        self.param_names = ("lower", "upper")
-        self.params_support = ((-np.inf, np.inf), (-np.inf, np.inf))
-        if lower is None:
-            self.lower = -np.inf
-        if upper is None:
-            self.upper = np.inf
-        self.support = (self.lower, self.upper)
-        if all_not_none(lower, upper):
-            self._update(lower, upper)
-            self.dist.a = self.lower
-            self.dist.b = self.upper
-        else:
-            self.lower = lower
-            self.upper = upper
-
-    def _get_frozen(self):
-        frozen = None
-        if all_not_none(self.params):
-            frozen = self.dist(self.lower, self.upper - self.lower)
-        return frozen
-
-    def _update(self, lower, upper):
-        self.lower = np.float64(lower)
-        self.upper = np.float64(upper)
-        self.params = (self.lower, self.upper)
-        self.support = (self.lower, self.upper)
-        self._update_rv_frozen()
-
-    def _fit_moments(self, mean, sigma):
-        lower = mean - 1.73205 * sigma
-        upper = mean + 1.73205 * sigma
-        self._update(lower, upper)
-
-    def _fit_mle(self, sample, **kwargs):
-        lower = np.min(sample)
-        upper = np.max(sample)
-        self._update(lower, upper)
-
-
-class VonMises(Continuous):
-    r"""
-    Univariate VonMises distribution.
-
-    The pdf of this distribution is
-
-    .. math::
-
-        f(x \mid \mu, \kappa) =
-            \frac{e^{\kappa\cos(x-\mu)}}{2\pi I_0(\kappa)}
-
-    where :math:`I_0` is the modified Bessel function of order 0.
-
-    .. plot::
-        :context: close-figs
-
-        import arviz as az
-        from preliz import VonMises
-        az.style.use('arviz-doc')
-        mus = [0., 0., 0.,  -2.5]
-        kappas = [.01, 0.5, 4., 2.]
-        for mu, kappa in zip(mus, kappas):
-            VonMises(mu, kappa).plot_pdf(support=(-np.pi,np.pi))
-
-    ========  ==========================================
-    Support   :math:`x \in [-\pi, \pi]`
-    Mean      :math:`\mu`
-    Variance  :math:`1-\frac{I_1(\kappa)}{I_0(\kappa)}`
-    ========  ==========================================
-
-    Parameters
-    ----------
-    mu : float
-        Mean.
-    kappa : float
-        Concentration (:math:`\frac{1}{\kappa}` is analogous to :math:`\sigma^2`).
-    """
-
-    def __init__(self, mu=None, kappa=None):
-        super().__init__()
-        self.dist = copy(stats.vonmises)
-        self._parametrization(mu, kappa)
-
-    def _parametrization(self, mu=None, kappa=None):
-        self.mu = mu
-        self.kappa = kappa
-        self.param_names = ("mu", "kappa")
-        self.params_support = ((-np.pi, np.pi), (eps, np.inf))
-        self.support = (-np.pi, np.pi)
-        if all_not_none(mu, kappa):
-            self._update(mu, kappa)
-
-    def _get_frozen(self):
-        frozen = None
-        if all_not_none(self.params):
-            frozen = self.dist(kappa=self.kappa, loc=self.mu)
-        return frozen
-
-    def _update(self, mu, kappa):
-        self.mu = np.float64(mu)
-        self.kappa = np.float64(kappa)
-        self.params = (self.mu, self.kappa)
-        self._update_rv_frozen()
-
-    def _fit_moments(self, mean, sigma):
-        mu = mean
-        kappa = 1 / sigma**2
-        self._update(mu, kappa)
-
-    def _fit_mle(self, sample, **kwargs):
-        kappa, mu, _ = self.dist.fit(sample, **kwargs)
-        self._update(mu, kappa)
-
-
-class Wald(Continuous):
-    r"""
-    Wald distribution.
-
-    The pdf of this distribution is
-
-    .. math::
-
-       f(x \mid \mu, \lambda) =
-           \left(\frac{\lambda}{2\pi}\right)^{1/2} x^{-3/2}
-           \exp\left\{
-               -\frac{\lambda}{2x}\left(\frac{x-\mu}{\mu}\right)^2
-           \right\}
-
-    .. plot::
-        :context: close-figs
-
-        import arviz as az
-        from preliz import Wald
-        az.style.use('arviz-doc')
-        mus = [1., 1.]
-        lams = [1., 3.]
-        for mu, lam in zip(mus, lams):
-            Wald(mu, lam).plot_pdf(support=(0,4))
-
-    ========  =============================
-    Support   :math:`x \in (0, \infty)`
-    Mean      :math:`\mu`
-    Variance  :math:`\dfrac{\mu^3}{\lambda}`
-    ========  =============================
-
-    Wald distribution has 3 alternative parametrizations. In terms of mu and lam,
-    mu and phi or lam and phi.
-
-    The link between the 3 alternatives is given by
-
-    .. math::
-
-       \phi = \dfrac{\lambda}{\mu}
-
-    Parameters
-    ----------
-    mu : float
-        Mean of the distribution (mu > 0).
-    lam : float
-        Relative precision (lam > 0).
-    phi : float
-        Shape parameter (phi > 0).
-    """
-
-    def __init__(self, mu=None, lam=None, phi=None):
-        super().__init__()
-        self.dist = copy(stats.invgauss)
-        self.support = (0, np.inf)
-        self._parametrization(mu, lam, phi)
-
-    def _parametrization(self, mu=None, lam=None, phi=None):
-        if (mu and lam and phi) is not None:
-            raise ValueError(
-                "Incompatible parametrization. Either use mu and lam or mu and phi or lam and phi."
-            )
-
-        self.param_names = ("mu", "lam")
-        self.params_support = ((eps, np.inf), (eps, np.inf))
-
-        if phi is not None:
-            self.phi = phi
-            if (mu and phi) is not None:
-                lam = self._from_mu_phi(mu, phi)
-                self.param_names = ("mu", "phi")
-
-            elif (lam and phi) is not None:
-                mu = self._from_lam_phi(lam, phi)
-                self.param_names = ("lam", "phi")
-
-        self.mu = mu
-        self.lam = lam
-        if all_not_none(self.mu, self.lam):
-            self._update(self.mu, self.lam)
-
-    def _from_mu_phi(self, mu, phi):
-        lam = mu * phi
-        return lam
-
-    def _from_lam_phi(self, lam, phi):
-        mu = lam / phi
-        return mu
-
-    def _to_phi(self, mu, lam):
-        phi = lam / mu
-        return phi
-
-    def _get_frozen(self):
-        frozen = None
-        if all_not_none(self.params):
-            frozen = self.dist(self.mu / self.lam, scale=self.lam)
-        return frozen
-
-    def _update(self, mu, lam):
-        self.mu = np.float64(mu)
-        self.lam = np.float64(lam)
-        self.phi = self._to_phi(mu, lam)
-
-        if self.param_names == ("mu", "lam"):
-            self.params = (self.mu, self.lam)
-        elif self.param_names == ("mu", "phi"):
-            self.params = (self.mu, self.phi)
-        elif self.param_names == ("lam", "phi"):
-            self.params = (self.lam, self.phi)
-
-        self._update_rv_frozen()
-
-    def _fit_moments(self, mean, sigma):
-        lam = mean**3 / sigma**2
-        self._update(mean, lam)
-
-    def _fit_mle(self, sample, **kwargs):
-        mu, _, lam = self.dist.fit(sample, **kwargs)
-        self._update(mu * lam, lam)
```

### Comparing `preliz-0.4.1/preliz/distributions/continuous_multivariate.py` & `preliz-0.5.0/preliz/distributions/continuous_multivariate.py`

 * *Files identical despite different names*

### Comparing `preliz-0.4.1/preliz/distributions/distributions.py` & `preliz-0.5.0/preliz/distributions/distributions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Parent classes for all families.
 """
 # pylint: disable=no-member
 from collections import namedtuple
+from copy import copy
 
 try:
     from ipywidgets import interactive
 except ImportError:
     pass
 import numpy as np
 
@@ -35,14 +36,18 @@
     def __init__(self):
         self.rv_frozen = None
         self.is_frozen = False
         self.opt = None
 
     def __repr__(self):
         name = self.__class__.__name__
+        if name == "Truncated":
+            name += self.dist.__class__.__name__
+        elif name == "Censored":
+            name += self.dist.__class__.__name__
         if self.is_frozen:
             bolded_name = "\033[1m" + name + "\033[0m"
 
             description = "".join(
                 f"{n}={np.round(v, 2)}," for n, v in zip(self.param_names, self.params)
             ).strip(",")
 
@@ -73,15 +78,20 @@
         """
         valid_distribution(self)
 
         if not isinstance(fmt, str):
             raise ValueError("Invalid format string.")
 
         if valid_scalar_params(self):
-            attr = namedtuple(self.__class__.__name__, ["mean", "median", "std", "lower", "upper"])
+            name = self.__class__.__name__
+            if name == "Truncated":
+                name = "Truncated" + self.dist.__class__.__name__
+            elif name == "Censored":
+                name = "Censored" + self.dist.__class__.__name__
+            attr = namedtuple(name, ["mean", "median", "std", "lower", "upper"])
             mean = float(f"{self.mean():{fmt}}")
             median = float(f"{self.median():{fmt}}")
             std = float(f"{self.std():{fmt}}")
             eti = self.eti(mass)
             lower_tail = float(f"{eti[0]:{fmt}}")
             upper_tail = float(f"{eti[1]:{fmt}}")
             return attr(mean, median, std, lower_tail, upper_tail)
@@ -136,15 +146,15 @@
         """Variance of the distribution."""
         return self.rv_frozen.var()
 
     def skewness(self):
         """Skewness of the distribution."""
         return self.stats(moment="s")
 
-    def kurtois(self):
+    def kurtosis(self):
         """Kurtosis of the distribution"""
         return self.stats(moments="k")
 
     def moments(self, types="mvsk"):
         """
         Compute moments of the distribution.
 
@@ -507,17 +517,22 @@
             Size of the figure
         """
         check_inside_notebook()
 
         if valid_scalar_params(self, check_frozen=False):
             args = dict(zip(self.param_names, self.params))
         else:
-            args = init_vals[self.__class__.__name__]
-
-        self.__init__(**args)  # pylint: disable=unnecessary-dunder-call
+            name = self.__class__.__name__
+            if name in ["Truncated", "Censored"]:
+                vals = copy(init_vals["Truncated"])
+                vals.update(init_vals[self.dist.__class__.__name__])
+                self._parametrization(**vals)
+            else:
+                args = init_vals[self.__class__.__name__]
+                self._parametrization(**args)
 
         if xy_lim == "both":
             xlim = self._finite_endpoints("full")
             xvals = self.xvals("restricted")
             if kind == "pdf":
                 max_pdf = np.max(self.pdf(xvals))
                 ylim = (-max_pdf * 0.075, max_pdf * 1.5)
@@ -545,15 +560,15 @@
         def plot(**args):  # pylint: disable=inconsistent-return-statements
             if self.__class__.__name__ == "Categorical":
                 values = list(args.values())
                 args = {list(args.keys())[0].split("_")[0]: values}
                 if np.sum(values) > 1:
                     return None
 
-            self.__init__(**args)  # pylint: disable=unnecessary-dunder-call
+            self._parametrization(**args)
 
             if kind == "pdf":
                 ax = self.plot_pdf(
                     legend=False,
                     pointinterval=pointinterval,
                     interval=interval,
                     levels=levels,
@@ -597,21 +612,18 @@
         Parameters
         ----------
         support : str
             Available options are `full` or `restricted`. If `full` the values will cover the entire
             support of the distribution, if finite, or the quantiles 0.0001 or 0.9999, if infinite.
             If `restricted` the values will cover the quantile 0.0001 to 0.9999.
         n_points : int
-            Number of values to return. The returned values may be fewer than `n_points` if
-            the actual number of discrete values in the support of the distribution is smaller than
-            `n_points`.
+            Number of values to return.
         """
         lower_ep, upper_ep = self._finite_endpoints(support)
-        x_vals = np.linspace(lower_ep, upper_ep, n_points)
-        return x_vals
+        return continuous_xvals(lower_ep, upper_ep, n_points)
 
     def _fit_mle(self, sample, **kwargs):
         """
         Estimate the parameters of the distribution from a sample by maximizing the likelihood.
 
         Parameters
         ----------
@@ -662,20 +674,15 @@
             If `restricted` the values will cover the quantile 0.0001 to 0.9999.
         n_points : int
             Number of values to return. The returned values may be fewer than `n_points` if
             the actual number of discrete values in the support of the distribution is smaller than
             `n_points`.
         """
         lower_ep, upper_ep = self._finite_endpoints(support)
-        range_x = upper_ep - lower_ep
-        if range_x <= n_points:
-            x_vals = np.arange(lower_ep, upper_ep + 1, dtype=int)
-        else:
-            x_vals = np.linspace(lower_ep, upper_ep + 1, n_points, dtype=int)
-        return x_vals
+        return discrete_xvals(lower_ep, upper_ep, n_points)
 
     def pdf(self, x, *args, **kwds):
         """Probability mass function at x.
 
         Parameters
         ----------
         x : array_like
@@ -688,7 +695,62 @@
 
         Parameters
         ----------
         x : array_like
             Values on which to evaluate the pdf
         """
         return self.rv_frozen.logpmf(x, *args, **kwds)
+
+
+class TruncatedCensored(Distribution):
+    """Base class for discrete distributions."""
+
+    def __init__(self):
+        super().__init__()
+        self.kind = self.dist.kind
+
+    def xvals(self, support, n_points=None):
+        """Provide x values in the support of the distribution. This is useful for example when
+        plotting.
+
+        Parameters
+        ----------
+        support : str
+            Available options are `full` or `restricted`. If `full` the values will cover the entire
+            support of the distribution, if finite, or the quantiles 0.0001 or 0.9999, if infinite.
+            If `restricted` the values will cover the quantile 0.0001 to 0.9999.
+        n_points : int
+            Number of values to return. For discrete distributions the returned values may be fewer
+            than `n_points` if the actual number of discrete values in the support of the
+            distribution is smaller than `n_points`.
+        """
+        lower_ep, upper_ep = self._finite_endpoints(support)
+
+        if self.kind == "continuous":
+            if n_points is None:
+                n_points = 1000
+            return continuous_xvals(lower_ep, upper_ep, n_points)
+        else:
+            if n_points is None:
+                n_points = 200
+            return discrete_xvals(lower_ep, upper_ep, n_points)
+
+    def skewness(self):
+        """Skewness of the distribution. Not implemented."""
+        return NotImplemented
+
+    def kurtosis(self):
+        """Kurtosis of the distribution. Not implemented."""
+        return NotImplemented
+
+
+def continuous_xvals(lower_ep, upper_ep, n_points):
+    return np.linspace(lower_ep, upper_ep, n_points)
+
+
+def discrete_xvals(lower_ep, upper_ep, n_points):
+    range_x = upper_ep - lower_ep
+    if range_x <= n_points:
+        x_vals = np.arange(lower_ep, upper_ep + 1, dtype=int)
+    else:
+        x_vals = np.linspace(lower_ep, upper_ep + 1, n_points, dtype=int)
+    return x_vals
```

### Comparing `preliz-0.4.1/preliz/distributions/distributions_multivariate.py` & `preliz-0.5.0/preliz/distributions/distributions_multivariate.py`

 * *Files identical despite different names*

### Comparing `preliz-0.4.1/preliz/distributions/exponential.py` & `preliz-0.5.0/preliz/distributions/exponential.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         self.lam = lam
         self.beta = beta
         if self.lam is not None:
             self._update(self.lam)
 
     def _update(self, lam):
         self.lam = np.float64(lam)
-        self.beta = 1 / lam
+        self.beta = 1 / self.lam
 
         if self.param_names[0] == "lam":
             self.params = (self.lam,)
         elif self.param_names[0] == "beta":
             self.params = (self.beta,)
 
         self.is_frozen = True
@@ -133,47 +133,47 @@
 
     def skewness(self):
         return 2
 
     def kurtosis(self):
         return 6
 
-    def rvs(self, size=1, random_state=None):
+    def rvs(self, size=None, random_state=None):
         random_state = np.random.default_rng(random_state)
         return random_state.exponential(self.beta, size)
 
     def _fit_moments(self, mean, sigma=None):  # pylint: disable=unused-argument
         lam = 1 / mean
         self._update(lam)
 
     def _fit_mle(self, sample, **kwargs):
         mean = mean_sample(sample)
         self._update(1 / mean)
 
 
-@nb.njit
+@nb.njit(cache=True)
 def nb_cdf(x, lam):
     x_lam = lam * x
     return cdf_bounds(1 - np.exp(-x_lam), x, 0, np.inf)
 
 
-@nb.njit
+@nb.njit(cache=True)
 def nb_ppf(q, beta):
     return ppf_bounds_cont(-beta * np.log(1 - q), q, 0, np.inf)
 
 
-@nb.vectorize(nopython=True)
+@nb.vectorize(nopython=True, cache=True)
 def nb_logpdf(x, lam):
     if x < 0:
         return -np.inf
     else:
         return np.log(lam) - lam * x
 
 
-@nb.njit
+@nb.njit(cache=True)
 def nb_neg_logpdf(x, lam):
     return (-nb_logpdf(x, lam)).sum()
 
 
-@nb.njit
+@nb.njit(cache=True)
 def nb_entropy(beta):
     return 1 + np.log(beta)
```

### Comparing `preliz-0.4.1/preliz/distributions/halfnormal.py` & `preliz-0.5.0/preliz/distributions/halfnormal.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # pylint: disable=attribute-defined-outside-init
 # pylint: disable=arguments-differ
 import numba as nb
 import numpy as np
-from scipy.special import erfinv  # pylint: disable=no-name-in-module
 
 from .distributions import Continuous
 from ..internal.distribution_helper import eps, to_precision, from_precision, all_not_none
-from ..internal.special import half_erf, ppf_bounds_cont
+from ..internal.special import half_erf, erfinv, ppf_bounds_cont
 
 
 class HalfNormal(Continuous):
     r"""
     HalfNormal Distribution
 
     The pdf of this distribution is
@@ -72,15 +71,15 @@
         self.sigma = sigma
         self.tau = tau
         if self.sigma is not None:
             self._update(self.sigma)
 
     def _update(self, sigma):
         self.sigma = np.float64(sigma)
-        self.tau = to_precision(sigma)
+        self.tau = to_precision(self.sigma)
 
         if self.param_names[0] == "sigma":
             self.params = (self.sigma,)
         elif self.param_names[0] == "tau":
             self.params = (self.tau,)
 
         self.is_frozen = True
@@ -92,20 +91,22 @@
         x = np.asarray(x)
         return np.exp(nb_logpdf(x, self.sigma))
 
     def cdf(self, x):
         """
         Compute the cumulative distribution function (CDF) at a given point x.
         """
+        x = np.asarray(x)
         return nb_cdf(x, self.sigma)
 
     def ppf(self, q):
         """
         Compute the percent point function (PPF) at a given probability q.
         """
+        q = np.asarray(q)
         return nb_ppf(q, self.sigma, self.support[0], self.support[1])
 
     def logpdf(self, x):
         """
         Compute the log probability density function (log PDF) at a given point x.
         """
         return nb_logpdf(x, self.sigma)
@@ -133,53 +134,50 @@
 
     def skewness(self):
         return 0.9952717464311565
 
     def kurtosis(self):
         return 0.8691773036059736
 
-    def rvs(self, size=1, random_state=None):
+    def rvs(self, size=None, random_state=None):
         random_state = np.random.default_rng(random_state)
         return np.abs(random_state.normal(0, self.sigma, size))
 
     def _fit_moments(self, mean, sigma):  # pylint: disable=unused-argument
         self._update(sigma / (1 - 2 / np.pi) ** 0.5)
 
     def _fit_mle(self, sample):
         self._update(nb_fit_mle(sample))
 
 
-@nb.njit
+@nb.njit(cache=True)
 def nb_cdf(x, sigma):
-    x = np.asarray(x)
     return half_erf(x / (sigma * 2**0.5))
 
 
-# @nb.jit
-# erfinv not supported by numba
+@nb.njit(cache=True)
 def nb_ppf(q, sigma, lower, upper):
-    q = np.asarray(q)
     x_vals = np.asarray(sigma * 2**0.5 * erfinv(q))
     return ppf_bounds_cont(x_vals, q, lower, upper)
 
 
-@nb.njit
+@nb.njit(cache=True)
 def nb_entropy(sigma):
     return 0.5 * np.log(np.pi * sigma**2.0 / 2.0) + 0.5
 
 
-@nb.njit
+@nb.njit(cache=True)
 def nb_fit_mle(sample):
     return np.mean(sample**2) ** 0.5
 
 
-@nb.vectorize(nopython=True)
+@nb.vectorize(nopython=True, cache=True)
 def nb_logpdf(x, sigma):
     if x < 0:
         return -np.inf
     else:
         return np.log(np.sqrt(2 / np.pi)) + np.log(1 / sigma) - 0.5 * ((x / sigma) ** 2)
 
 
-@nb.njit
+@nb.njit(cache=True)
 def nb_neg_logpdf(x, sigma):
     return -(nb_logpdf(x, sigma)).sum()
```

### Comparing `preliz-0.4.1/preliz/distributions/laplace.py` & `preliz-0.5.0/preliz/distributions/laplace.py`

 * *Files 7% similar despite different names*

```diff
@@ -114,58 +114,58 @@
 
     def skewness(self):
         return 0.0
 
     def kurtosis(self):
         return 3.0
 
-    def rvs(self, size=1, random_state=None):
+    def rvs(self, size=None, random_state=None):
         random_state = np.random.default_rng(random_state)
         return random_state.laplace(self.mu, self.b, size)
 
     def _fit_moments(self, mean, sigma):
         b = (sigma / 2) * (2**0.5)
         self._update(mean, b)
 
     def _fit_mle(self, sample, **kwargs):
         mu, b = nb_fit_mle(sample)
         self._update(mu, b)
 
 
-@nb.vectorize(nopython=True)
+@nb.vectorize(nopython=True, cache=True)
 def nb_cdf(x, mu, b):
     x = (x - mu) / b
     if x > 0:
         return 1.0 - 0.5 * np.exp(-x)
     return 0.5 * np.exp(x)
 
 
-@nb.vectorize(nopython=True)
+@nb.vectorize(nopython=True, cache=True)
 def nb_ppf(q, mu, b):
     if q > 0.5:
         q = -np.log(2 * (1 - q))
     else:
         q = np.log(2 * q)
     return q * b + mu
 
 
-@nb.njit
+@nb.njit(cache=True)
 def nb_logpdf(x, mu, b):
     x = (x - mu) / b
     return np.log(0.5) - np.abs(x) - np.log(b)
 
 
-@nb.njit
+@nb.njit(cache=True)
 def nb_neg_logpdf(x, mu, b):
     return (-nb_logpdf(x, mu, b)).sum()
 
 
-@nb.njit
+@nb.njit(cache=True)
 def nb_entropy(b):
     return np.log(2) + 1 + np.log(b)
 
 
-@nb.njit
+@nb.njit(cache=True)
 def nb_fit_mle(sample):
     median = np.median(sample)
     scale = np.sum(np.abs(sample - median)) / len(sample)
     return median, scale
```

### Comparing `preliz-0.4.1/preliz/distributions/negativebinomial.py` & `preliz-0.5.0/preliz/distributions/negativebinomial.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # pylint: disable=attribute-defined-outside-init
 # pylint: disable=arguments-differ
 import numba as nb
 import numpy as np
-from scipy.special import betainc, nbdtrik  # pylint: disable=no-name-in-module
+from scipy.special import nbdtrik  # pylint: disable=no-name-in-module
 
 from .distributions import Discrete
 from ..internal.distribution_helper import eps, any_not_none, all_not_none
 from ..internal.optimization import optimize_moments, optimize_ml
-from ..internal.special import gammaln, xlogy, cdf_bounds, ppf_bounds_disc
+from ..internal.special import betainc, gammaln, xlogy, cdf_bounds, ppf_bounds_disc
 
 
 class NegativeBinomial(Discrete):
     R"""
     Negative binomial distribution.
 
     The negative binomial distribution describes a Poisson random variable
@@ -167,40 +167,39 @@
 
     def skewness(self):
         return (2 - self.p) / ((1 - self.p) * self.n) ** 0.5
 
     def kurtosis(self):
         return 6 / self.n + self.p**2 / ((1 - self.p) * self.n)
 
-    def rvs(self, size=1, random_state=None):
+    def rvs(self, size=None, random_state=None):
         random_state = np.random.default_rng(random_state)
         return random_state.negative_binomial(self.n, self.p, size=size)
 
     def _fit_moments(self, mean, sigma=None):
         optimize_moments(self, mean, sigma)
 
     def _fit_mle(self, sample):
         optimize_ml(self, sample)
 
 
-# @nb.jit
-# betainc not supported by numba
+@nb.njit(cache=True)
 def nb_cdf(x, n, p, lower, upper):
     prob = betainc(n, x + 1, p)
     return cdf_bounds(prob, x, lower, upper)
 
 
 # @nb.jit
 # bdtrik not supported by numba
 def nb_ppf(q, n, p, lower, upper):
     x_vals = np.ceil(nbdtrik(q, n, p))
     return ppf_bounds_disc(x_vals, q, lower, upper)
 
 
-@nb.njit
+@nb.njit(cache=True)
 def nb_logpdf(y, n, p):
     return gammaln(y + n) - gammaln(n) - gammaln(y + 1) + xlogy(n, p) + xlogy(y, 1 - p)
 
 
-@nb.njit
+@nb.njit(cache=True)
 def nb_neg_logpdf(y, n, p):
     return -(nb_logpdf(y, n, p)).sum()
```

### Comparing `preliz-0.4.1/preliz/distributions/normal.py` & `preliz-0.5.0/preliz/distributions/normal.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # pylint: disable=arguments-differ
 import numba as nb
 import numpy as np
 from scipy.special import erf, erfinv  # pylint: disable=no-name-in-module
 
 from .distributions import Continuous
 from ..internal.distribution_helper import eps, to_precision, from_precision, all_not_none
-from ..internal.special import mean_and_std
+from ..internal.special import erf, erfinv, mean_and_std, ppf_bounds_cont
 
 
 class Normal(Continuous):
     r"""
     Normal distribution.
 
     The pdf of this distribution is
@@ -100,20 +100,22 @@
         """
         return nb_pdf(x, self.mu, self.sigma)
 
     def cdf(self, x):
         """
         Compute the cumulative distribution function (CDF) at a given point x.
         """
+        x = np.asarray(x)
         return nb_cdf(x, self.mu, self.sigma)
 
     def ppf(self, q):
         """
         Compute the percent point function (PPF) at a given probability q.
         """
+        q = np.asarray(q)
         return nb_ppf(q, self.mu, self.sigma)
 
     def logpdf(self, x):
         """
         Compute the log probability density function (log PDF) at a given point x.
         """
         return nb_logpdf(x, self.mu, self.sigma)
@@ -141,56 +143,52 @@
 
     def skewness(self):
         return 0
 
     def kurtosis(self):
         return 0
 
-    def rvs(self, size=1, random_state=None):
+    def rvs(self, size=None, random_state=None):
         random_state = np.random.default_rng(random_state)
         return random_state.normal(self.mu, self.sigma, size)
 
     def _fit_moments(self, mean, sigma):
         self._update(mean, sigma)
 
     def _fit_mle(self, sample):
         self._update(*nb_fit_mle(sample))
 
 
-# @nb.jit
-# erf not supported by numba
+@nb.njit(cache=True)
 def nb_cdf(x, mu, sigma):
-    x = np.asarray(x)
     return 0.5 * (1 + erf((x - mu) / (sigma * 2**0.5)))
 
 
-# @nb.jit
-# erfinv not supported by numba
+@nb.njit(cache=True)
 def nb_ppf(q, mu, sigma):
-    q = np.asarray(q)
-    return mu + sigma * 2**0.5 * erfinv(2 * q - 1)
+    return ppf_bounds_cont(mu + sigma * 2**0.5 * erfinv(2 * q - 1), q, -np.inf, np.inf)
 
 
-@nb.njit
+@nb.njit(cache=True)
 def nb_pdf(x, mu, sigma):
     x = np.asarray(x)
     return 1 / np.sqrt(2 * np.pi * sigma**2) * np.exp(-0.5 * ((x - mu) / sigma) ** 2)
 
 
-@nb.njit
+@nb.njit(cache=True)
 def nb_entropy(sigma):
     return 0.5 * (np.log(2 * np.pi * np.e * sigma**2))
 
 
-@nb.njit
+@nb.njit(cache=True)
 def nb_fit_mle(sample):
     return mean_and_std(sample)
 
 
-@nb.njit
+@nb.njit(cache=True)
 def nb_logpdf(x, mu, sigma):
     return -np.log(sigma) - 0.5 * np.log(2 * np.pi) - 0.5 * ((x - mu) / sigma) ** 2
 
 
-@nb.njit
+@nb.njit(cache=True)
 def nb_neg_logpdf(x, mu, sigma):
     return -(nb_logpdf(x, mu, sigma)).sum()
```

### Comparing `preliz-0.4.1/preliz/distributions/poisson.py` & `preliz-0.5.0/preliz/distributions/poisson.py`

 * *Files 6% similar despite different names*

```diff
@@ -114,15 +114,15 @@
 
     def skewness(self):
         return 1 / self.mu**0.5
 
     def kurtosis(self):
         return 1 / self.mu
 
-    def rvs(self, size=1, random_state=None):
+    def rvs(self, size=None, random_state=None):
         random_state = np.random.default_rng(random_state)
         return random_state.poisson(self.mu, size=size)
 
     def _fit_moments(self, mean, sigma=None):  # pylint: disable=unused-argument
         self._update(mean)
 
     def _fit_mle(self, sample):
@@ -143,20 +143,20 @@
     vals = np.ceil(pdtrik(q, mu))
     vals1 = np.maximum(vals - 1, 0)
     temp = pdtr(vals1, mu)
     x_vals = np.where(temp >= q, vals1, vals)
     return ppf_bounds_disc(x_vals, q, lower, upper)
 
 
-@nb.njit
+@nb.njit(cache=True)
 def nb_fit_mle(sample):
     return np.mean(sample)
 
 
-@nb.njit
+@nb.njit(cache=True)
 def nb_logpdf(x, mu):
     return xlogy(x, mu) - gammaln(x + 1) - mu
 
 
-@nb.njit
+@nb.njit(cache=True)
 def nb_neg_logpdf(x, mu):
     return -(nb_logpdf(x, mu)).sum()
```

### Comparing `preliz-0.4.1/preliz/distributions/weibull.py` & `preliz-0.5.0/preliz/distributions/weibull.py`

 * *Files 3% similar despite different names*

```diff
@@ -135,47 +135,47 @@
             (self.beta / sigma) ** 4 * gamma(1 + 4 / self.alpha)
             - 4 * skew * m_s
             - 6 * m_s**2
             - m_s**4
             - 3
         )
 
-    def rvs(self, size=1, random_state=None):
+    def rvs(self, size=None, random_state=None):
         random_state = np.random.default_rng(random_state)
         return random_state.weibull(self.alpha, size) * self.beta
 
     def _fit_moments(self, mean, sigma):
         alpha, beta = garcia_approximation(mean, sigma)
         self._update(alpha, beta)
 
     def _fit_mle(self, sample):
         mean, std = mean_and_std(sample)
         self._fit_moments(mean, std)
         optimize_ml(self, sample)
 
 
-@nb.njit
+@nb.njit(cache=True)
 def nb_cdf(x, alpha, beta, lower, upper):
     prob = 1 - np.exp(-((x / beta) ** alpha))
     return cdf_bounds(prob, x, lower, upper)
 
 
-@nb.njit
+@nb.njit(cache=True)
 def nb_ppf(q, alpha, beta, lower, upper):
     x_val = beta * (-np.log(1 - q)) ** (1 / alpha)
     return ppf_bounds_cont(x_val, q, lower, upper)
 
 
-@nb.njit
+@nb.njit(cache=True)
 def nb_entropy(alpha, beta):
     return np.euler_gamma * (1 - 1 / alpha) + np.log(beta / alpha) + 1
 
 
-@nb.njit
+@nb.njit(cache=True)
 def nb_logpdf(x, alpha, beta):
     x_b = x / beta
     return np.log(alpha / beta) + (alpha - 1) * np.log(x_b) - x_b**alpha
 
 
-@nb.njit
+@nb.njit(cache=True)
 def nb_neg_logpdf(x, alpha, beta):
     return -(nb_logpdf(x, alpha, beta)).sum()
```

### Comparing `preliz-0.4.1/preliz/distributions/zi_binomial.py` & `preliz-0.5.0/preliz/distributions/zi_binomial.py`

 * *Files 4% similar despite different names*

```diff
@@ -132,24 +132,19 @@
         # implement skewness
         return np.nan
 
     def kurtosis(self):
         # implement kurtosis
         return np.nan
 
-    def rvs(self, size=1, random_state=None):
+    def rvs(self, size=None, random_state=None):
         random_state = np.random.default_rng(random_state)
-
-        samples = np.zeros(size, dtype=int)
-        non_zero_indices = np.where(np.random.uniform(size=size) < (self.psi))[0]
-        samples[~non_zero_indices] = 0
-        samples[non_zero_indices] = random_state.binomial(
-            self.n, self.p, size=len(non_zero_indices)
-        )
-        return samples
+        zeros = random_state.uniform(size=size) > (1 - self.psi)
+        binomial = random_state.binomial(self.n, self.p, size=size)
+        return zeros * binomial
 
     def _fit_moments(self, mean, sigma):
         optimize_moments(self, mean, sigma)
 
     def _fit_mle(self, sample):
         optimize_ml(self, sample)
 
@@ -167,15 +162,15 @@
 def nb_ppf(q, psi, n, p, lower, upper):
     q = np.asarray(q)
     n_vals = np.ceil(bdtrik(q, n, p))
     x_vals = (1 - psi) + psi * n_vals
     return ppf_bounds_disc(x_vals, q, lower, upper)
 
 
-@nb.vectorize(nopython=True)
+@nb.vectorize(nopython=True, cache=True)
 def nb_logpdf(psi, n, y, p):
     if y == 0:
         return np.log((1 - psi) + psi * (1 - p) ** n)
     if y > n:
         return -np.inf
     else:
         return (
@@ -183,10 +178,10 @@
             + gammaln(n + 1)
             - (gammaln(y + 1) + gammaln(n - y + 1))
             + y * np.log(p)
             + (n - y) * np.log1p(-p)
         )
 
 
-@nb.njit
+@nb.njit(cache=True)
 def nb_neg_logpdf(psi, n, y, p):
     return -(nb_logpdf(psi, n, y, p)).sum()
```

### Comparing `preliz-0.4.1/preliz/distributions/zi_negativebinomial.py` & `preliz-0.5.0/preliz/distributions/zi_negativebinomial.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # pylint: disable=attribute-defined-outside-init
 # pylint: disable=arguments-differ
 import numba as nb
 import numpy as np
-from scipy.special import betainc, nbdtrik  # pylint: disable=no-name-in-module
+from scipy.special import nbdtrik  # pylint: disable=no-name-in-module
 
 from .distributions import Discrete
 from ..internal.distribution_helper import eps, any_not_none, all_not_none
 from ..internal.optimization import optimize_moments, optimize_ml
-from ..internal.special import gammaln, xlogy, cdf_bounds, ppf_bounds_disc
+from ..internal.special import betainc, gammaln, xlogy, cdf_bounds, ppf_bounds_disc
 
 
 class ZeroInflatedNegativeBinomial(Discrete):
     R"""
     Zero-Inflated Negative binomial distribution.
 
     The Zero-inflated version of the Negative Binomial (NB).
@@ -184,59 +184,53 @@
         # implement skewness
         return np.nan
 
     def kurtosis(self):
         # implement kurtosis
         return np.nan
 
-    def rvs(self, size=1, random_state=None):
+    def rvs(self, size=None, random_state=None):
         random_state = np.random.default_rng(random_state)
-
-        samples = np.zeros(size, dtype=int)
-        non_zero_indices = np.where(np.random.uniform(size=size) < (self.psi))[0]
-        samples[~non_zero_indices] = 0
-        samples[non_zero_indices] = random_state.negative_binomial(
-            self.n, self.p, size=len(non_zero_indices)
-        )
-        return samples
+        zeros = random_state.uniform(size=size) > (1 - self.psi)
+        nbinomial = random_state.negative_binomial(self.n, self.p, size=size)
+        return zeros * nbinomial
 
     def _fit_moments(self, mean, sigma):
         optimize_moments(self, mean, sigma)
 
     def _fit_mle(self, sample):
         optimize_ml(self, sample)
 
 
-# @nb.jit
-# betainc not supported by numba
+@nb.njit(cache=True)
 def nb_cdf(x, psi, n, p, lower, upper):
     nb_prob = betainc(n, x + 1, p)
     prob = (1 - psi) + psi * nb_prob
     return cdf_bounds(prob, x, lower, upper)
 
 
 # @nb.jit
 # bdtrik not supported by numba
 def nb_ppf(q, psi, n, p, lower, upper):
     nb_vals = np.ceil(nbdtrik(q, n, p))
     x_vals = (1 - psi) + psi * nb_vals
     return ppf_bounds_disc(x_vals, q, lower, upper)
 
 
-@nb.vectorize(nopython=True)
+@nb.vectorize(nopython=True, cache=True)
 def nb_logpdf(y, psi, n, p, mu):
     if y == 0:
         return np.log((1 - psi) + psi * (n / (n + mu)) ** n)
     else:
         return (
             np.log(psi)
             + gammaln(y + n)
             - gammaln(n)
             - gammaln(y + 1)
             + xlogy(n, p)
             + xlogy(y, 1 - p)
         )
 
 
-@nb.njit
+@nb.njit(cache=True)
 def nb_neg_logpdf(y, psi, n, p, mu):
     return -(nb_logpdf(y, psi, n, p, mu)).sum()
```

### Comparing `preliz-0.4.1/preliz/distributions/zi_poisson.py` & `preliz-0.5.0/preliz/distributions/zi_poisson.py`

 * *Files 3% similar despite different names*

```diff
@@ -142,21 +142,19 @@
 
     def skewness(self):
         return np.nan
 
     def kurtosis(self):
         return np.nan
 
-    def rvs(self, size=1, random_state=None):
+    def rvs(self, size=None, random_state=None):
         random_state = np.random.default_rng(random_state)
-        samples = np.zeros(size, dtype=int)
-        non_zero_indices = np.where(np.random.uniform(size=size) < (self.psi))[0]
-        samples[~non_zero_indices] = 0
-        samples[non_zero_indices] = random_state.poisson(self.mu, size=len(non_zero_indices))
-        return samples
+        zeros = random_state.uniform(size=size) > (1 - self.psi)
+        poisson = random_state.poisson(self.mu, size=size)
+        return zeros * poisson
 
 
 # @nb.jit
 # pdtr not supported by numba
 def nb_cdf(x, psi, mu, lower, upper):
     p_prob = pdtr(x, mu)
     prob = (1 - psi) + psi * p_prob
@@ -171,18 +169,18 @@
     vals1 = np.maximum(vals - 1, 0)
     temp = pdtr(vals1, mu)
     p_vals = np.where(temp >= q, vals1, vals)
     x_vals = (1 - psi) + psi * p_vals
     return ppf_bounds_disc(x_vals, q, lower, upper)
 
 
-@nb.vectorize(nopython=True)
+@nb.vectorize(nopython=True, cache=True)
 def nb_logpdf(x, psi, mu):
     if x == 0:
         return np.log(np.exp(-mu) * psi - psi + 1)
     else:
         return np.log(psi) + xlogy(x, mu) - gammaln(x + 1) - mu
 
 
-@nb.njit
+@nb.njit(cache=True)
 def nb_neg_logpdf(x, psi, mu):
     return -(nb_logpdf(x, psi, mu)).sum()
```

### Comparing `preliz-0.4.1/preliz/internal/distribution_helper.py` & `preliz-0.5.0/preliz/internal/distribution_helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -139,8 +139,10 @@
     "Geometric": {"p": 0.5},
     "HyperGeometric": {"N": 50, "k": 10, "n": 20},
     "NegativeBinomial": {"mu": 5.0, "alpha": 2.0},
     "Poisson": {"mu": 4.5},
     "ZeroInflatedBinomial": {"psi": 0.7, "n": 10, "p": 0.5},
     "ZeroInflatedNegativeBinomial": {"psi": 0.7, "mu": 5, "alpha": 8},
     "ZeroInflatedPoisson": {"psi": 0.8, "mu": 4.5},
+    "Truncated": {"lower": -10, "upper": 10},
+    "Censored": {"lower": -10, "upper": 10},
 }
```

### Comparing `preliz-0.4.1/preliz/internal/optimization.py` & `preliz-0.5.0/preliz/internal/optimization.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """
 Optimization routines and utilities
 """
 from sys import modules
 import warnings
+from copy import copy
 
 import numpy as np
-from scipy.optimize import minimize, least_squares
-from scipy.special import i0, i1  # pylint: disable=no-name-in-module
+from scipy.optimize import minimize, least_squares, root_scalar
+from scipy.special import i0, i1, i0e, i1e  # pylint: disable=no-name-in-module
 from .distribution_helper import init_vals as default_vals
 
 
 def optimize_max_ent(dist, lower, upper, mass, none_idx, fixed):
     def prob_bound(params, dist, lower, upper, mass):
         params = get_params(dist, params, none_idx, fixed)
         dist._parametrization(**params)
@@ -105,15 +106,21 @@
         return loss
 
     none_idx, fixed = get_fixed_params(dist)
 
     if params is not None:
         dist._update(*params)
     else:
-        dist._update(**default_vals[dist.__class__.__name__])
+        name = dist.__class__.__name__
+        if name == "Truncated":
+            vals = copy(default_vals["Truncated"])
+            vals.update(default_vals[dist.dist.__class__.__name__])
+            dist._parametrization(**vals)
+        else:
+            dist._update(**default_vals[name])
 
     init_vals = np.array(dist.params)[none_idx]
 
     if dist.__class__.__name__ in ["HyperGeometric", "BetaBinomial"]:
         opt = least_squares(func, x0=init_vals, args=(dist, mean, sigma))
     else:
         bounds = np.array(dist.params_support)[none_idx]
@@ -386,7 +393,62 @@
     for idx, p_n in enumerate(distribution.param_names):
         value = getattr(distribution, p_n)
         if value is None:
             none_idx.append(idx)
         else:
             fixed.append(value)
     return none_idx, fixed
+
+
+def find_kappa(data, mu):
+    ere = np.mean(np.cos(mu - data))
+
+    if ere > 0:
+
+        def solve_for_kappa(kappa):
+            return i1e(kappa) / i0e(kappa) - ere
+
+        root_res = root_scalar(
+            solve_for_kappa, method="brentq", bracket=(np.finfo(float).tiny, 1e16)
+        )
+        return root_res.root
+    else:
+        return np.finfo(float).tiny
+
+
+def find_ppf(dist, q):
+    """
+    Function to find the percent point function (ppf) given the
+    cumulative distribution function (cdf).
+
+    Parameters
+    ----------
+
+    dist : preliz distribution
+        The distribution for which to find the ppf.
+    q : float or list-like
+        The required quantile(s) for which to find the ppf.
+    """
+
+    def objective(x, dist, q):
+        return np.sum((dist.cdf(x) - q) ** 2)
+
+    q = np.asarray(q)
+    initial_guess, bounds = initialize_ppf(dist, q)
+    opt = minimize(objective, x0=initial_guess, method="Powell", bounds=bounds, args=(dist, q))
+
+    return opt["x"]
+
+
+def initialize_ppf(dist, q):
+    # Calculate k using the formula for Chebyshev's inequality
+    q = np.clip(q, 0.1, 0.9)
+    k = np.sqrt(1 / (1 - q))
+
+    k = np.where(q < 0.5, -k, k)
+
+    initial_guess = dist.mean() + k * dist.std()
+    lower, upper = dist.support
+    np.where(initial_guess < lower, lower, np.where(initial_guess > upper, upper, initial_guess))
+    bounds = [(lower, upper)]
+
+    return initial_guess, bounds
```

### Comparing `preliz-0.4.1/preliz/internal/parser.py` & `preliz-0.5.0/preliz/internal/parser.py`

 * *Files identical despite different names*

### Comparing `preliz-0.4.1/preliz/internal/plot_helper.py` & `preliz-0.5.0/preliz/internal/plot_helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -119,37 +119,61 @@
             ax.set_title(label)
             label = None
     else:
         label = None
 
     x = dist.xvals(support)
     if dist.kind == "continuous":
+        if dist.__class__.__name__ == "Censored":
+            lower, upper = dist.support
+            disc_vals = [None, None]
+            if np.min(x) <= lower:
+                disc_vals[0] = dist.dist.pdf(lower) * 1.5
+                disc_vals[1] = dist.dist.pdf(upper) * 1.5
+
+            x = x[x != dist.support[0]]
+            x = x[x != dist.support[1]]
+
         density = dist.pdf(x)
         ax.axhline(0, color="0.8", ls="--", zorder=0)
-        ax.plot(x, density, label=label, color=color, alpha=alpha)
+        p = ax.plot(x, density, label=label, color=color, alpha=alpha)
         ax.set_yticks([])
+
+        if dist.__class__.__name__ == "Censored":
+            if disc_vals[0] is not None:
+                ax.vlines(lower, 0, disc_vals[0], ls="--", color=p[0].get_color(), alpha=alpha)
+            if disc_vals[1] is not None:
+                ax.vlines(upper, 0, disc_vals[1], ls="--", color=p[0].get_color(), alpha=alpha)
+
     else:
         mass = dist.pdf(x)
-        x_c = np.linspace(x[0], x[-1], 1000)
-        # if new distribution, directly compute pdf at non-integer values
-        if dist.rv_frozen is None:
-            mass_c = np.clip(dist.pdf(x_c), np.min(mass), np.max(mass))
-        # if old, interpolate
+
+        if dist.__class__.__name__ in ["Categorical", "Bernoulli"]:
+            p = ax.plot(x, mass, "o", label=label, color=color, alpha=alpha)
+            ax.vlines(x, 0, mass, ls="dotted", color=p[0].get_color(), alpha=alpha)
         else:
-            if len(x) > 2:
-                interp = PchipInterpolator(x, mass)
+            x_c = np.linspace(x[0], x[-1], 1000)
+            # if new distribution, directly compute pdf at non-integer values
+            print(dist.__class__.__name__)
+            if dist.rv_frozen is None:
+                mass_c = np.clip(dist.pdf(x_c), np.min(mass), np.max(mass))
+            # if old, interpolate
             else:
-                interp = interp1d(x, mass)
+                if len(x) > 2:
+                    interp = PchipInterpolator(x, mass)
+                else:
+                    interp = interp1d(x, mass)
 
-            mass_c = np.clip(interp(x_c), np.min(mass), np.max(mass))
+                mass_c = np.clip(interp(x_c), np.min(mass), np.max(mass))
+
+            p = ax.plot(x_c, mass_c, ls="dotted", color=color, alpha=alpha)
+            ax.plot(x, mass, "o", label=label, color=p[0].get_color(), alpha=alpha)
 
-        ax.axhline(0, color="0.8", ls="--", zorder=0)
-        p = ax.plot(x_c, mass_c, ls="dotted", color=color, alpha=alpha)
-        ax.plot(x, mass, "o", label=label, color=p[0].get_color(), alpha=alpha)
         ax.xaxis.set_major_locator(MaxNLocator(integer=True))
+        ax.axhline(0, color="0.8", ls="--", zorder=0)
 
     if pointinterval:
         plot_pointinterval(dist, interval, levels, ax=ax)
 
     if legend == "legend":
         side_legend(ax)
 
@@ -423,15 +447,15 @@
         if results[0].dtype.kind == "i":
             bins = np.arange(np.min(results), np.max(results) + 1.5) - 0.5
             if len(bins) < 30:
                 ax.set_xticks(bins + 0.5)
         else:
             bins = "auto"
         ax.hist(
-            results,
+            results.T,
             alpha=alpha,
             density=True,
             color=["0.5"] * iterations,
             bins=bins,
             histtype="step",
         )
         ax.hist(
```

### Comparing `preliz-0.4.1/preliz/internal/plot_helper_multivariate.py` & `preliz-0.5.0/preliz/internal/plot_helper_multivariate.py`

 * *Files identical despite different names*

### Comparing `preliz-0.4.1/preliz/internal/predictive_helper.py` & `preliz-0.5.0/preliz/internal/predictive_helper.py`

 * *Files identical despite different names*

### Comparing `preliz-0.4.1/preliz/ppls/pymc_io.py` & `preliz-0.5.0/preliz/ppls/pymc_io.py`

 * *Files identical despite different names*

### Comparing `preliz-0.4.1/preliz/predictive/ppa.py` & `preliz-0.5.0/preliz/predictive/ppa.py`

 * *Files identical despite different names*

### Comparing `preliz-0.4.1/preliz/predictive/ppe.py` & `preliz-0.5.0/preliz/predictive/ppe.py`

 * *Files identical despite different names*

### Comparing `preliz-0.4.1/preliz/predictive/predictive_explorer.py` & `preliz-0.5.0/preliz/predictive/predictive_explorer.py`

 * *Files identical despite different names*

### Comparing `preliz-0.4.1/preliz/tests/check_inside_notebook.ipynb` & `preliz-0.5.0/preliz/tests/check_inside_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `preliz-0.4.1/preliz/tests/plot_interactive.ipynb` & `preliz-0.5.0/preliz/tests/plot_interactive.ipynb`

 * *Files identical despite different names*

### Comparing `preliz-0.4.1/preliz/tests/ppa.ipynb` & `preliz-0.5.0/preliz/tests/ppa.ipynb`

 * *Files identical despite different names*

### Comparing `preliz-0.4.1/preliz/tests/predictive_explorer.ipynb` & `preliz-0.5.0/preliz/tests/predictive_explorer.ipynb`

 * *Files identical despite different names*

### Comparing `preliz-0.4.1/preliz/tests/quartile_int.ipynb` & `preliz-0.5.0/preliz/tests/quartile_int.ipynb`

 * *Files identical despite different names*

### Comparing `preliz-0.4.1/preliz/tests/roulette.ipynb` & `preliz-0.5.0/preliz/tests/roulette.ipynb`

 * *Files identical despite different names*

### Comparing `preliz-0.4.1/preliz/tests/test_beta_mode.py` & `preliz-0.5.0/preliz/tests/test_beta_mode.py`

 * *Files identical despite different names*

### Comparing `preliz-0.4.1/preliz/tests/test_dirichlet_mode.py` & `preliz-0.5.0/preliz/tests/test_dirichlet_mode.py`

 * *Files identical despite different names*

### Comparing `preliz-0.4.1/preliz/tests/test_distributions.py` & `preliz-0.5.0/preliz/tests/test_distributions.py`

 * *Files identical despite different names*

### Comparing `preliz-0.4.1/preliz/tests/test_helper.py` & `preliz-0.5.0/preliz/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `preliz-0.4.1/preliz/tests/test_maxent.py` & `preliz-0.5.0/preliz/tests/test_maxent.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,15 +152,15 @@
         (HyperGeometric(), 2, 14, 0.9, (0, 21), (56, 21, 21)),
         (NegativeBinomial(), 0, 15, 0.9, (0, np.inf), (7.573, 2.077)),
         (NegativeBinomial(p=0.2), 0, 15, 0.9, (0, np.inf), (1.848)),
         (Poisson(), 0, 3, 0.7, (0, np.inf), (2.763)),
         (ZeroInflatedBinomial(), 1, 10, 0.9, (0, 10), (0.902, 9.0, 0.485)),
         (ZeroInflatedBinomial(psi=0.7), 1, 10, 0.7, (0, 11), (10, 0.897)),
         (ZeroInflatedNegativeBinomial(), 2, 15, 0.8, (0, np.inf), (1.0, 9.862, 3.429)),
-        (ZeroInflatedNegativeBinomial(psi=0.9), 2, 15, 0.8, (0, np.inf), (9.013, 6.307)),
+        (ZeroInflatedNegativeBinomial(psi=0.9), 2, 15, 0.8, (0, np.inf), (8.965, 6.174)),
         (ZeroInflatedPoisson(), 0, 3, 0.7, (0, np.inf), (0.8445, 3.010)),
         (ZeroInflatedPoisson(psi=0.8), 0, 3, 0.7, (0, np.inf), (3.099)),
     ],
 )
 def test_maxent(dist, lower, upper, mass, support, result):
     _, opt = maxent(dist, lower, upper, mass)
```

### Comparing `preliz-0.4.1/preliz/tests/test_mle.py` & `preliz-0.5.0/preliz/tests/test_mle.py`

 * *Files identical despite different names*

### Comparing `preliz-0.4.1/preliz/tests/test_plots.py` & `preliz-0.5.0/preliz/tests/test_plots.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,19 +35,22 @@
         a_dist.plot_cdf(**kwargs)
         kwargs.pop("support", None)
         a_dist.plot_ppf(**kwargs)
 
 
 def test_plot_interactive():
     for idx, distribution in enumerate(pz.distributions.__all__):
-        if distribution not in ["Dirichlet", "MvNormal"]:
+        if distribution not in ["Dirichlet", "MvNormal", "Truncated", "Censored"]:
             dist = getattr(pz.distributions, distribution)
             kind = ["pdf", "cdf", "ppf"][idx % 3]
             xy_lim = ["auto", "both"][idx % 2]
             dist().plot_interactive(kind=kind, xy_lim=xy_lim)
+        if distribution in ["Truncated", "Censored"]:
+            dist = getattr(pz.distributions, distribution)
+            dist(pz.Normal(0, 2), -1, 1).plot_interactive(kind="pdf", xy_lim="both")
 
 
 @pytest.mark.parametrize(
     "kwargs",
     [
         {},
         {"marginals": True},
```

### Comparing `preliz-0.4.1/preliz/tests/test_quartile.py` & `preliz-0.5.0/preliz/tests/test_quartile.py`

 * *Files identical despite different names*

### Comparing `preliz-0.4.1/preliz/tests/test_roulette.py` & `preliz-0.5.0/preliz/tests/test_roulette.py`

 * *Files identical despite different names*

### Comparing `preliz-0.4.1/preliz/unidimensional/beta_mode.py` & `preliz-0.5.0/preliz/unidimensional/beta_mode.py`

 * *Files identical despite different names*

### Comparing `preliz-0.4.1/preliz/unidimensional/dirichlet_mode.py` & `preliz-0.5.0/preliz/unidimensional/dirichlet_mode.py`

 * *Files identical despite different names*

### Comparing `preliz-0.4.1/preliz/unidimensional/maxent.py` & `preliz-0.5.0/preliz/unidimensional/maxent.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,17 +96,22 @@
 
     # Find which parameters has been fixed
     none_idx, fixed = get_fixed_params(distribution)
 
     # Heuristic to provide an initial guess for the optimization step
     # We obtain those guesses by first approximating the mean and standard deviation
     # from intervals and mass and then use those values for moment matching
-    distribution._fit_moments(  # pylint:disable=protected-access
-        mean=(lower + upper) / 2, sigma=((upper - lower) / 4) / mass
-    )
+    if distribution.__class__.__name__ == "Uniform":
+        distribution._fit_moments(  # pylint:disable=protected-access
+            mean=(lower + upper) / 2, sigma=((upper - lower) / 3.4) / mass
+        )
+    else:
+        distribution._fit_moments(  # pylint:disable=protected-access
+            mean=(lower + upper) / 2, sigma=((upper - lower) / 4) / mass
+        )
 
     opt = optimize_max_ent(distribution, lower, upper, mass, none_idx, fixed)
 
     r_error, computed_mass = relative_error(distribution, lower, upper, mass)
 
     if r_error > 0.01:
         _log.info(
```

### Comparing `preliz-0.4.1/preliz/unidimensional/mle.py` & `preliz-0.5.0/preliz/unidimensional/mle.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,16 +43,15 @@
 
     sample = np.array(sample)
     x_min = sample.min()
     x_max = sample.max()
 
     fitted = fit_to_sample(distributions, sample, x_min, x_max)
 
-    if plot > len(distributions):
-        plot = len(distributions)
+    plot = min(plot, len(distributions))
 
     idx = np.argsort(fitted.losses)
 
     if plot:
         plot_idx = idx[:plot]
         for dist in fitted.distributions[plot_idx]:
             if dist is not None:
```

### Comparing `preliz-0.4.1/preliz/unidimensional/quartile.py` & `preliz-0.5.0/preliz/unidimensional/quartile.py`

 * *Files identical despite different names*

### Comparing `preliz-0.4.1/preliz/unidimensional/quartile_int.py` & `preliz-0.5.0/preliz/unidimensional/quartile_int.py`

 * *Files identical despite different names*

### Comparing `preliz-0.4.1/preliz/unidimensional/roulette.py` & `preliz-0.5.0/preliz/unidimensional/roulette.py`

 * *Files identical despite different names*

### Comparing `preliz-0.4.1/pyproject.toml` & `preliz-0.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -12,26 +12,26 @@
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Science/Research",
     "Intended Audience :: Education",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
 ]
 dynamic = ["version"]
 description = "The place for all your prior elicitation needs."
 dependencies = [
   "arviz",
   "matplotlib>=3.5",
   "numba>=0.59",
   "numpy>=1.22",
-  "scipy>=1.9.1",
+  "scipy>=1.9.1, <1.13"
 ]
 
 [tool.flit.module]
 name = "preliz"
 
 [project.urls]
 source = "https://github.com/arviz-devs/preliz"
```

### Comparing `preliz-0.4.1/PKG-INFO` & `preliz-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: preliz
-Version: 0.4.1
+Version: 0.5.0
 Summary: The place for all your prior elicitation needs.
 Author-email: ArviZ team <arviz.devs@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: arviz
 Requires-Dist: matplotlib>=3.5
 Requires-Dist: numba>=0.59
 Requires-Dist: numpy>=1.22
-Requires-Dist: scipy>=1.9.1
+Requires-Dist: scipy>=1.9.1, <1.13
 Requires-Dist: nbclient<0.6,>=0.2 ; extra == "full"
 Requires-Dist: ipywidgets ; extra == "full"
 Requires-Dist: ipympl ; extra == "full"
 Requires-Dist: jupyterlab ; extra == "lab"
 Requires-Dist: notebook ; extra == "notebook"
 Project-URL: source, https://github.com/arviz-devs/preliz
 Project-URL: tracker, https://github.com/arviz-devs/preliz/issues
```

