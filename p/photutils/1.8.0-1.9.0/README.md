# Comparing `tmp/photutils-1.8.0.tar.gz` & `tmp/photutils-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "photutils-1.8.0.tar", last modified: Wed May 17 18:27:07 2023, max compression
+gzip compressed data, was "photutils-1.9.0.tar", last modified: Tue Aug 15 00:50:17 2023, max compression
```

## Comparing `photutils-1.8.0.tar` & `photutils-1.9.0.tar`

### file list

```diff
@@ -1,316 +1,329 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.970378 photutils-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-17 18:26:37.000000 photutils-1.8.0/.bandit.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.858373 photutils-1.8.0/.circleci/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-17 18:26:37.000000 photutils-1.8.0/.circleci/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.834372 photutils-1.8.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.858373 photutils-1.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-17 18:26:37.000000 photutils-1.8.0/.github/workflows/32bit_tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-05-17 18:26:37.000000 photutils-1.8.0/.github/workflows/ci_tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-05-17 18:26:37.000000 photutils-1.8.0/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-17 18:26:37.000000 photutils-1.8.0/.github/workflows/cron_tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-17 18:26:37.000000 photutils-1.8.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-17 18:26:37.000000 photutils-1.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-17 18:26:37.000000 photutils-1.8.0/.lgtm.yml
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-17 18:26:37.000000 photutils-1.8.0/.pep8speaks.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-05-17 18:26:37.000000 photutils-1.8.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-17 18:26:37.000000 photutils-1.8.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    73988 2023-05-17 18:26:37.000000 photutils-1.8.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-17 18:26:37.000000 photutils-1.8.0/CITATION.md
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-17 18:26:37.000000 photutils-1.8.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-05-17 18:26:37.000000 photutils-1.8.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-17 18:26:37.000000 photutils-1.8.0/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-17 18:26:37.000000 photutils-1.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-05-17 18:27:07.970378 photutils-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-05-17 18:26:37.000000 photutils-1.8.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-17 18:26:37.000000 photutils-1.8.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.870373 photutils-1.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.874374 photutils-1.8.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/_static/photutils.css
--rw-r--r--   0 runner    (1001) docker     (123)    20779 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/_static/photutils_banner-475x120.png
--rw-r--r--   0 runner    (1001) docker     (123)    25003 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/_static/photutils_banner.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    44248 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/_static/photutils_banner.svg
--rw-r--r--   0 runner    (1001) docker     (123)    16158 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/_static/photutils_banner_original.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/_static/photutils_logo-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)    15530 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/_static/photutils_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    36500 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/aperture.rst
--rw-r--r--   0 runner    (1001) docker     (123)    21448 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/background.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/centroids.rst
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/citation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/datasets.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11855 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/detection.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.874374 photutils-1.8.0/docs/dev/
--rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/dev/releasing.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12729 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/epsf.rst
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/geometry.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9976 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/grouping.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10634 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/isophote.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9538 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/isophote_faq.rst
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/morphology.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/overview.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/pixel_conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/profiles.rst
--rw-r--r--   0 runner    (1001) docker     (123)    28319 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/psf.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9255 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/psf_matching.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.882374 photutils-1.8.0/docs/psf_spec/
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/psf_spec/background_estimator.rst
--rw-r--r--   0 runner    (1001) docker     (123)   472207 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/psf_spec/block_diagram.png
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/psf_spec/block_template.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/psf_spec/culler_and_ender.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/psf_spec/finder.rst
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/psf_spec/fitter.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/psf_spec/group_maker.rst
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/psf_spec/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/psf_spec/noise_data.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/psf_spec/psf_model.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/psf_spec/scene_maker.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/psf_spec/single_object_model.rst
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/rtd_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    25920 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/segmentation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/test_function.rst
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/utils.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.886374 photutils-1.8.0/docs/whats_new/
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/whats_new/1.1.rst
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/whats_new/1.2.rst
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/whats_new/1.3.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/whats_new/1.4.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/whats_new/1.5.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/whats_new/1.6.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/whats_new/1.7.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/whats_new/1.8.rst
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/whats_new/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.886374 photutils-1.8.0/photutils/
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/CITATION.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/_astropy_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-05-17 18:27:07.000000 photutils-1.8.0/photutils/_compiler.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.894374 photutils-1.8.0/photutils/aperture/
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/aperture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6190 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/aperture/attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    11827 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/aperture/bounding_box.py
--rw-r--r--   0 runner    (1001) docker     (123)    15732 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/aperture/circle.py
--rw-r--r--   0 runner    (1001) docker     (123)    30661 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/aperture/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    21642 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/aperture/ellipse.py
--rw-r--r--   0 runner    (1001) docker     (123)    11312 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/aperture/mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/aperture/photometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    23768 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/aperture/rectangle.py
--rw-r--r--   0 runner    (1001) docker     (123)    57981 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/aperture/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.898375 photutils-1.8.0/photutils/aperture/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/aperture/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/aperture/tests/test_aperture_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/aperture/tests/test_bounding_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/aperture/tests/test_circle.py
--rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/aperture/tests/test_ellipse.py
--rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/aperture/tests/test_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)    32220 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/aperture/tests/test_photometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5743 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/aperture/tests/test_rectangle.py
--rw-r--r--   0 runner    (1001) docker     (123)    13233 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/aperture/tests/test_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.898375 photutils-1.8.0/photutils/background/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/background/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28240 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/background/background_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    23895 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/background/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/background/interpolators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.902375 photutils-1.8.0/photutils/background/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/background/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15395 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/background/tests/test_background_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/background/tests/test_core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.902375 photutils-1.8.0/photutils/centroids/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/centroids/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18869 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/centroids/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/centroids/gaussian.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.906375 photutils-1.8.0/photutils/centroids/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/centroids/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14633 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/centroids/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/centroids/tests/test_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.906375 photutils-1.8.0/photutils/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8878 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/datasets/load.py
--rw-r--r--   0 runner    (1001) docker     (123)    32633 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/datasets/make.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.906375 photutils-1.8.0/photutils/datasets/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/datasets/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/datasets/tests/test_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/datasets/tests/test_make.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.910375 photutils-1.8.0/photutils/detection/
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9750 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/detection/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    25269 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/detection/daofinder.py
--rw-r--r--   0 runner    (1001) docker     (123)    18646 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/detection/irafstarfinder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/detection/peakfinder.py
--rw-r--r--   0 runner    (1001) docker     (123)    12917 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/detection/starfinder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.910375 photutils-1.8.0/photutils/detection/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/detection/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.918375 photutils-1.8.0/photutils/detection/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/detection/tests/data/daofind_test_thresh08.0_fwhm01.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/detection/tests/data/daofind_test_thresh08.0_fwhm01.5.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/detection/tests/data/daofind_test_thresh08.0_fwhm02.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/detection/tests/data/daofind_test_thresh10.0_fwhm01.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/detection/tests/data/daofind_test_thresh10.0_fwhm01.5.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/detection/tests/data/daofind_test_thresh10.0_fwhm02.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/detection/tests/data/irafstarfind_test_thresh08.0_fwhm01.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/detection/tests/data/irafstarfind_test_thresh08.0_fwhm01.5.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/detection/tests/data/irafstarfind_test_thresh08.0_fwhm02.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/detection/tests/data/irafstarfind_test_thresh10.0_fwhm01.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/detection/tests/data/irafstarfind_test_thresh10.0_fwhm01.5.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/detection/tests/data/irafstarfind_test_thresh10.0_fwhm02.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/detection/tests/test_daofinder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/detection/tests/test_irafstarfinder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/detection/tests/test_peakfinder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/detection/tests/test_starfinder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.918375 photutils-1.8.0/photutils/extern/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/extern/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.918375 photutils-1.8.0/photutils/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8395 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/geometry/circular_overlap.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/geometry/core.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/geometry/core.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/geometry/elliptical_overlap.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/geometry/rectangular_overlap.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.922376 photutils-1.8.0/photutils/geometry/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/geometry/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/geometry/tests/test_circular_overlap_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/geometry/tests/test_elliptical_overlap_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/geometry/tests/test_rectangular_overlap_grid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.926376 photutils-1.8.0/photutils/isophote/
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34017 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/ellipse.py
--rw-r--r--   0 runner    (1001) docker     (123)    16995 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/fitter.py
--rw-r--r--   0 runner    (1001) docker     (123)    20022 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/harmonics.py
--rw-r--r--   0 runner    (1001) docker     (123)    11711 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/integrator.py
--rw-r--r--   0 runner    (1001) docker     (123)    29450 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/isophote.py
--rw-r--r--   0 runner    (1001) docker     (123)     6242 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    16093 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.930376 photutils-1.8.0/photutils/isophote/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.934376 photutils-1.8.0/photutils/isophote/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    25920 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/tests/data/M51_table.fits
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/tests/data/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    43200 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/tests/data/minimum_radius_test.fits
--rw-r--r--   0 runner    (1001) docker     (123)    28800 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/tests/data/synth_highsnr_table.fits
--rw-r--r--   0 runner    (1001) docker     (123)    28800 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/tests/data/synth_lowsnr_table.fits
--rw-r--r--   0 runner    (1001) docker     (123)    28800 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/tests/data/synth_table.fits
--rw-r--r--   0 runner    (1001) docker     (123)    80640 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/tests/data/synth_table_mean.fits
--rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/tests/data/synth_table_mean.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/tests/make_test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/tests/test_angles.py
--rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/tests/test_ellipse.py
--rw-r--r--   0 runner    (1001) docker     (123)     7782 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/tests/test_fitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/tests/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/tests/test_harmonics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/tests/test_integrator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11000 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/tests/test_isophote.py
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/tests/test_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/tests/test_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.934376 photutils-1.8.0/photutils/morphology/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/morphology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/morphology/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/morphology/non_parametric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.938376 photutils-1.8.0/photutils/morphology/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/morphology/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/morphology/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/morphology/tests/test_non_parametric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.938376 photutils-1.8.0/photutils/profiles/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10764 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/profiles/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/profiles/curve_of_growth.py
--rw-r--r--   0 runner    (1001) docker     (123)    13980 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/profiles/radial_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.942376 photutils-1.8.0/photutils/profiles/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/profiles/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/profiles/tests/test_curve_of_growth.py
--rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/profiles/tests/test_radial_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.942376 photutils-1.8.0/photutils/psf/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/psf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31883 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/psf/epsf.py
--rw-r--r--   0 runner    (1001) docker     (123)    27025 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/psf/epsf_stars.py
--rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/psf/groupstars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.946376 photutils-1.8.0/photutils/psf/matching/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/psf/matching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/psf/matching/fourier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.946376 photutils-1.8.0/photutils/psf/matching/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/psf/matching/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/psf/matching/tests/test_fourier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/psf/matching/tests/test_windows.py
--rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/psf/matching/windows.py
--rw-r--r--   0 runner    (1001) docker     (123)    42730 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/psf/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    51286 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/psf/photometry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.950377 photutils-1.8.0/photutils/psf/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/psf/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/psf/tests/test_epsf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/psf/tests/test_epsf_stars.py
--rw-r--r--   0 runner    (1001) docker     (123)    18813 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/psf/tests/test_groupstars.py
--rw-r--r--   0 runner    (1001) docker     (123)    14760 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/psf/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    37009 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/psf/tests/test_photometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     9794 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/psf/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11485 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/psf/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.954377 photutils-1.8.0/photutils/segmentation/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   135232 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/segmentation/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    52595 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/segmentation/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    21984 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/segmentation/deblend.py
--rw-r--r--   0 runner    (1001) docker     (123)    14500 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/segmentation/detect.py
--rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/segmentation/finder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.954377 photutils-1.8.0/photutils/segmentation/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/segmentation/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36763 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/segmentation/tests/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    17820 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/segmentation/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    13064 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/segmentation/tests/test_deblend.py
--rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/segmentation/tests/test_detect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/segmentation/tests/test_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/segmentation/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/segmentation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.958377 photutils-1.8.0/photutils/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.962377 photutils-1.8.0/photutils/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/_convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/_moments.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/_optional_deps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/_quantity_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/_round.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/_wcs_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/colormaps.py
--rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/cutouts.py
--rw-r--r--   0 runner    (1001) docker     (123)    20003 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/depths.py
--rw-r--r--   0 runner    (1001) docker     (123)     7764 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/footprints.py
--rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/interpolation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.970378 photutils-1.8.0/photutils/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/tests/test_colormaps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/tests/test_convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/tests/test_cutouts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/tests/test_depths.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/tests/test_footprints.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/tests/test_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/tests/test_moments.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/tests/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/tests/test_quantity_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-17 18:27:07.000000 photutils-1.8.0/photutils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.890374 photutils-1.8.0/photutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-05-17 18:27:07.000000 photutils-1.8.0/photutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-05-17 18:27:07.000000 photutils-1.8.0/photutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 18:27:07.000000 photutils-1.8.0/photutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 18:27:07.000000 photutils-1.8.0/photutils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-17 18:27:07.000000 photutils-1.8.0/photutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-17 18:27:07.000000 photutils-1.8.0/photutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-17 18:26:37.000000 photutils-1.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-05-17 18:27:07.970378 photutils-1.8.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2193 2023-05-17 18:26:37.000000 photutils-1.8.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-05-17 18:26:37.000000 photutils-1.8.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 00:50:17.481604 photutils-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-15 00:49:57.000000 photutils-1.9.0/.bandit.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 00:50:17.449604 photutils-1.9.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-08-15 00:49:57.000000 photutils-1.9.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 00:50:17.449604 photutils-1.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-08-15 00:49:57.000000 photutils-1.9.0/.github/workflows/ci_cron_daily.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-08-15 00:49:57.000000 photutils-1.9.0/.github/workflows/ci_cron_weekly.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-08-15 00:49:57.000000 photutils-1.9.0/.github/workflows/ci_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-08-15 00:49:57.000000 photutils-1.9.0/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-08-15 00:49:57.000000 photutils-1.9.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-08-15 00:49:57.000000 photutils-1.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-15 00:49:57.000000 photutils-1.9.0/.pep8speaks.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-08-15 00:49:57.000000 photutils-1.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-08-15 00:49:57.000000 photutils-1.9.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    75906 2023-08-15 00:49:57.000000 photutils-1.9.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-15 00:49:57.000000 photutils-1.9.0/CITATION.md
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-08-15 00:49:57.000000 photutils-1.9.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-08-15 00:49:57.000000 photutils-1.9.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-08-15 00:49:57.000000 photutils-1.9.0/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-08-15 00:50:17.481604 photutils-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-08-15 00:49:57.000000 photutils-1.9.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-08-15 00:49:57.000000 photutils-1.9.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 00:50:17.453604 photutils-1.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 00:50:17.453604 photutils-1.9.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/_static/photutils.css
+-rw-r--r--   0 runner    (1001) docker     (123)    20779 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/_static/photutils_banner-475x120.png
+-rw-r--r--   0 runner    (1001) docker     (123)    25003 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/_static/photutils_banner.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    44248 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/_static/photutils_banner.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    16158 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/_static/photutils_banner_original.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/_static/photutils_logo-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15530 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/_static/photutils_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    36487 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/aperture.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    21465 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/background.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/centroids.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/citation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/datasets.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11855 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/detection.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 00:50:17.453604 photutils-1.9.0/docs/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/dev/releasing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12716 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/epsf.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/geometry.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6786 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/grouping.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10626 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/isophote.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9537 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/isophote_faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/morphology.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/pixel_conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11392 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/profiles.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    25912 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/psf.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9251 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/psf_matching.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 00:50:17.453604 photutils-1.9.0/docs/psf_spec/
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/psf_spec/background_estimator.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   472207 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/psf_spec/block_diagram.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/psf_spec/block_template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/psf_spec/culler_and_ender.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/psf_spec/finder.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/psf_spec/fitter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/psf_spec/group_maker.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/psf_spec/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/psf_spec/noise_data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/psf_spec/psf_model.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/psf_spec/scene_maker.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/psf_spec/single_object_model.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    25916 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/segmentation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/test_function.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/utils.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 00:50:17.457604 photutils-1.9.0/docs/whats_new/
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/whats_new/1.1.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/whats_new/1.2.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/whats_new/1.3.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/whats_new/1.4.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/whats_new/1.5.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/whats_new/1.6.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/whats_new/1.7.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/whats_new/1.8.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/whats_new/1.9.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-08-15 00:49:57.000000 photutils-1.9.0/docs/whats_new/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 00:50:17.457604 photutils-1.9.0/photutils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/CITATION.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/_astropy_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-08-15 00:50:17.000000 photutils-1.9.0/photutils/_compiler.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 00:50:17.457604 photutils-1.9.0/photutils/aperture/
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/aperture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/aperture/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11827 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/aperture/bounding_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15732 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/aperture/circle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30661 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/aperture/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21642 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/aperture/ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11312 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/aperture/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/aperture/photometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23768 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/aperture/rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57981 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/aperture/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 00:50:17.461604 photutils-1.9.0/photutils/aperture/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/aperture/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/aperture/tests/test_aperture_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/aperture/tests/test_bounding_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/aperture/tests/test_circle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/aperture/tests/test_ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/aperture/tests/test_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32220 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/aperture/tests/test_photometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5743 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/aperture/tests/test_rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13233 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/aperture/tests/test_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 00:50:17.461604 photutils-1.9.0/photutils/background/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/background/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28240 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/background/background_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23895 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/background/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/background/interpolators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/background/local_background.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 00:50:17.461604 photutils-1.9.0/photutils/background/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/background/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15395 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/background/tests/test_background_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/background/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/background/tests/test_local_background.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 00:50:17.461604 photutils-1.9.0/photutils/centroids/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/centroids/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18866 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/centroids/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/centroids/gaussian.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 00:50:17.461604 photutils-1.9.0/photutils/centroids/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/centroids/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14633 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/centroids/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/centroids/tests/test_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 00:50:17.461604 photutils-1.9.0/photutils/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8878 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/datasets/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36798 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/datasets/make.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 00:50:17.461604 photutils-1.9.0/photutils/datasets/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/datasets/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/datasets/tests/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7764 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/datasets/tests/test_make.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 00:50:17.461604 photutils-1.9.0/photutils/detection/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9750 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/detection/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25269 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/detection/daofinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18646 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/detection/irafstarfinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/detection/peakfinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12917 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/detection/starfinder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 00:50:17.465604 photutils-1.9.0/photutils/detection/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/detection/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 00:50:17.465604 photutils-1.9.0/photutils/detection/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/detection/tests/data/daofind_test_thresh08.0_fwhm01.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/detection/tests/data/daofind_test_thresh08.0_fwhm01.5.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/detection/tests/data/daofind_test_thresh08.0_fwhm02.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/detection/tests/data/daofind_test_thresh10.0_fwhm01.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/detection/tests/data/daofind_test_thresh10.0_fwhm01.5.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/detection/tests/data/daofind_test_thresh10.0_fwhm02.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/detection/tests/data/irafstarfind_test_thresh08.0_fwhm01.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/detection/tests/data/irafstarfind_test_thresh08.0_fwhm01.5.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/detection/tests/data/irafstarfind_test_thresh08.0_fwhm02.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/detection/tests/data/irafstarfind_test_thresh10.0_fwhm01.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/detection/tests/data/irafstarfind_test_thresh10.0_fwhm01.5.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/detection/tests/data/irafstarfind_test_thresh10.0_fwhm02.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/detection/tests/test_daofinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/detection/tests/test_irafstarfinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/detection/tests/test_peakfinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/detection/tests/test_starfinder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 00:50:17.465604 photutils-1.9.0/photutils/extern/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/extern/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 00:50:17.465604 photutils-1.9.0/photutils/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8395 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/geometry/circular_overlap.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/geometry/core.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/geometry/core.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/geometry/elliptical_overlap.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/geometry/rectangular_overlap.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 00:50:17.465604 photutils-1.9.0/photutils/geometry/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/geometry/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/geometry/tests/test_circular_overlap_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/geometry/tests/test_elliptical_overlap_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/geometry/tests/test_rectangular_overlap_grid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 00:50:17.465604 photutils-1.9.0/photutils/isophote/
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/isophote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34017 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/isophote/ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16995 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/isophote/fitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20022 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/isophote/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/isophote/harmonics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11711 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/isophote/integrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29454 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/isophote/isophote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6242 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/isophote/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16093 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/isophote/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 00:50:17.469604 photutils-1.9.0/photutils/isophote/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/isophote/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 00:50:17.469604 photutils-1.9.0/photutils/isophote/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    25920 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/isophote/tests/data/M51_table.fits
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/isophote/tests/data/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    43200 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/isophote/tests/data/minimum_radius_test.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    28800 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/isophote/tests/data/synth_highsnr_table.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    28800 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/isophote/tests/data/synth_lowsnr_table.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    28800 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/isophote/tests/data/synth_table.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    80640 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/isophote/tests/data/synth_table_mean.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/isophote/tests/data/synth_table_mean.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/isophote/tests/make_test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/isophote/tests/test_angles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/isophote/tests/test_ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7782 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/isophote/tests/test_fitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/isophote/tests/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/isophote/tests/test_harmonics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/isophote/tests/test_integrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11000 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/isophote/tests/test_isophote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/isophote/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/isophote/tests/test_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/isophote/tests/test_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 00:50:17.469604 photutils-1.9.0/photutils/morphology/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/morphology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/morphology/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/morphology/non_parametric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 00:50:17.469604 photutils-1.9.0/photutils/morphology/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/morphology/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/morphology/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/morphology/tests/test_non_parametric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 00:50:17.469604 photutils-1.9.0/photutils/profiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10764 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/profiles/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/profiles/curve_of_growth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14303 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/profiles/radial_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 00:50:17.469604 photutils-1.9.0/photutils/profiles/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/profiles/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/profiles/tests/test_curve_of_growth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/profiles/tests/test_radial_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 00:50:17.473604 photutils-1.9.0/photutils/psf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/psf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31882 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/psf/epsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27025 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/psf/epsf_stars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35054 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/psf/griddedpsfmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/psf/groupers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/psf/groupstars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 00:50:17.473604 photutils-1.9.0/photutils/psf/matching/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/psf/matching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/psf/matching/fourier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 00:50:17.473604 photutils-1.9.0/photutils/psf/matching/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/psf/matching/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/psf/matching/tests/test_fourier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/psf/matching/tests/test_windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/psf/matching/windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33166 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/psf/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57626 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/psf/photometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52693 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/psf/photometry_depr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 00:50:17.473604 photutils-1.9.0/photutils/psf/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/psf/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 00:50:17.473604 photutils-1.9.0/photutils/psf/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/psf/tests/data/STDPSF_ACSWFC_F814W_mock.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/psf/tests/data/STDPSF_NRCA1_F150W_mock.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    11520 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/psf/tests/data/STDPSF_NRCSW_F150W_mock.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/psf/tests/data/STDPSF_WFC3UV_F814W_mock.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/psf/tests/data/STDPSF_WFPC2_F814W_mock.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/psf/tests/test_epsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/psf/tests/test_epsf_stars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/psf/tests/test_griddedpsfmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20387 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/psf/tests/test_groupstars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8603 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/psf/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42048 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/psf/tests/test_photometry-depr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22689 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/psf/tests/test_photometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14472 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/psf/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17524 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/psf/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 00:50:17.477604 photutils-1.9.0/photutils/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   135558 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/segmentation/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52595 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/segmentation/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21886 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/segmentation/deblend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14500 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/segmentation/detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/segmentation/finder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 00:50:17.477604 photutils-1.9.0/photutils/segmentation/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/segmentation/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37027 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/segmentation/tests/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17820 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/segmentation/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13064 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/segmentation/tests/test_deblend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/segmentation/tests/test_detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/segmentation/tests/test_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/segmentation/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/segmentation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 00:50:17.477604 photutils-1.9.0/photutils/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/tests/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 00:50:17.477604 photutils-1.9.0/photutils/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/utils/_convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/utils/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/utils/_moments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/utils/_optional_deps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/utils/_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/utils/_progress_bars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/utils/_quantity_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/utils/_round.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/utils/_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/utils/_wcs_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/utils/colormaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/utils/cutouts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20016 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/utils/depths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7764 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/utils/footprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/utils/interpolation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 00:50:17.481604 photutils-1.9.0/photutils/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/utils/tests/test_colormaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/utils/tests/test_convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/utils/tests/test_cutouts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/utils/tests/test_depths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/utils/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/utils/tests/test_footprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/utils/tests/test_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/utils/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/utils/tests/test_moments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/utils/tests/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/utils/tests/test_quantity_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-08-15 00:49:57.000000 photutils-1.9.0/photutils/utils/tests/test_round.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-15 00:50:17.000000 photutils-1.9.0/photutils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 00:50:17.457604 photutils-1.9.0/photutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-08-15 00:50:17.000000 photutils-1.9.0/photutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-08-15 00:50:17.000000 photutils-1.9.0/photutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-15 00:50:17.000000 photutils-1.9.0/photutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-15 00:50:16.000000 photutils-1.9.0/photutils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-08-15 00:50:17.000000 photutils-1.9.0/photutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-15 00:50:17.000000 photutils-1.9.0/photutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-08-15 00:49:57.000000 photutils-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-08-15 00:50:17.481604 photutils-1.9.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1651 2023-08-15 00:49:57.000000 photutils-1.9.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-08-15 00:49:57.000000 photutils-1.9.0/tox.ini
```

### Comparing `photutils-1.8.0/.github/workflows/ci_tests.yml` & `photutils-1.9.0/.github/workflows/ci_tests.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,40 @@
-name: CI
+name: CI Tests
 
 on:
   push:
     branches:
       - main
     tags:
       - '*'
   pull_request:
   schedule:
     # run every Monday at 6am UTC
     - cron: '0 6 * * 1'
   workflow_dispatch:
 
-
 concurrency:
   group: ${{ github.workflow }}-${{ github.ref }}
   cancel-in-progress: true
 
 env:
   TOXARGS: '-v'
 
 permissions:
   contents: read
 
 jobs:
-  ci-tests:
+  tests:
     name: ${{ matrix.prefix }} ${{ matrix.os }}, ${{ matrix.tox_env }}
     runs-on: ${{ matrix.os }}
     continue-on-error: ${{ matrix.allow_failure }}
     strategy:
       matrix:
         include:
           - os: ubuntu-latest
-            python: '3.8'
-            tox_env: 'py38-test-alldeps'
-            allow_failure: false
-            prefix: ''
-
-          - os: ubuntu-latest
             python: '3.9'
             tox_env: 'py39-test-alldeps'
             allow_failure: false
             prefix: ''
 
           - os: ubuntu-latest
             python: '3.10'
@@ -53,52 +46,52 @@
           - os: ubuntu-latest
             python: '3.11'
             tox_env: 'py311-test-alldeps'
             allow_failure: false
             prefix: ''
 
           - os: macos-latest
-            python: '3.10'
-            tox_env: 'py310-test-alldeps'
+            python: '3.11'
+            tox_env: 'py311-test-alldeps'
             allow_failure: false
             prefix: ''
 
           - os: windows-latest
-            python: '3.10'
-            tox_env: 'py310-test-alldeps'
+            python: '3.11'
+            tox_env: 'py311-test-alldeps'
             allow_failure: false
             prefix: ''
 
           - os: ubuntu-latest
-            python: '3.10'
-            tox_env: 'py310-test'
+            python: '3.11'
+            tox_env: 'py311-test'
             allow_failure: false
             prefix: ''
 
           - os: ubuntu-latest
-            python: '3.10'
+            python: '3.11'
             tox_env: 'codestyle'
             allow_failure: false
             prefix: ''
 
           - os: ubuntu-latest
-            python: '3.10'
+            python: '3.11'
             tox_env: 'pep517'
             allow_failure: false
             prefix: ''
 
           - os: ubuntu-latest
-            python: '3.10'
+            python: '3.11'
             tox_env: 'bandit'
             allow_failure: false
             prefix: ''
 
           - os: ubuntu-latest
-            python: '3.8'
-            tox_env: 'py38-test-alldeps-astropylts-numpy118'
+            python: '3.9'
+            tox_env: 'py39-test-alldeps-astropylts-numpy122'
             allow_failure: false
             prefix: ''
 
           - os: ubuntu-latest
             python: '3.11'
             tox_env: 'py311-test-alldeps-devdeps'
             toxposargs: --remote-data=any
@@ -126,9 +119,9 @@
         python -c "import tox; print(f'tox {tox.__version__}')"
     - name: Run tests
       run: tox -e ${{ matrix.tox_env }} -- ${{ matrix.toxposargs }}
     - name: Upload coverage to codecov
       if: ${{ contains(matrix.tox_env, '-cov') }}
       uses: codecov/codecov-action@v3
       with:
-        file: ./coverage.xml
+        files: ./coverage.xml
         verbose: true
```

### Comparing `photutils-1.8.0/.github/workflows/codeql.yml` & `photutils-1.9.0/.github/workflows/codeql.yml`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,17 @@
     branches: [ "main" ]
   pull_request:
     # The branches below must be a subset of the branches above
     branches: [ "main" ]
   schedule:
     - cron: '40 5 * * 4'
 
+permissions:
+  contents: read
+
 jobs:
   analyze:
     name: Analyze
     runs-on: ubuntu-latest
     permissions:
       actions: read
       contents: read
```

### Comparing `photutils-1.8.0/.github/workflows/cron_tests.yml` & `photutils-1.9.0/.github/workflows/ci_cron_daily.yml`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,45 @@
-name: Cron Tests
+name: Daily Cron Tests
 
 on:
   schedule:
     # run at 6am UTC on Tue-Fri (complete tests are run every Monday)
     - cron: '0 6 * * 2-5'
+  pull_request:
+    # We also want this workflow triggered if the 'Daily CI' label is added
+    # or present when PR is updated
+    types:
+      - synchronize
+      - labeled
+  push:
+    tags:
+      - '*'
   workflow_dispatch:
 
+concurrency:
+  group: ${{ github.workflow }}-${{ github.ref }}
+  cancel-in-progress: true
+
 env:
   TOXARGS: '-v'
 
 permissions:
   contents: read
 
 jobs:
-  cron-test:
+  tests:
+    if: (github.repository == 'astropy/photutils' && (github.event_name == 'schedule' || github.event_name == 'push' || github.event_name == 'workflow_dispatch' || contains(github.event.pull_request.labels.*.name, 'Daily CI')))
     name: ${{ matrix.os }}, ${{ matrix.tox_env }}
     runs-on: ${{ matrix.os }}
     continue-on-error: ${{ matrix.allow_failure }}
     strategy:
       matrix:
         include:
           - os: ubuntu-latest
-            python: '3.10'
+            python: '3.11'
             tox_env: 'linkcheck'
             allow_failure: false
 
           - os: ubuntu-latest
             python: '3.11'
             tox_env: 'py311-test-alldeps-devdeps'
             toxposargs: --remote-data=any
@@ -52,9 +66,9 @@
         python -c "import tox; print(f'tox {tox.__version__}')"
     - name: Run tests
       run: tox -e ${{ matrix.tox_env }} -- ${{ matrix.toxposargs }}
     - name: Upload coverage to codecov
       if: ${{ contains(matrix.tox_env, '-cov') }}
       uses: codecov/codecov-action@v3
       with:
-        file: ./coverage.xml
+        files: ./coverage.xml
         verbose: true
```

### Comparing `photutils-1.8.0/.github/workflows/publish.yml` & `photutils-1.9.0/.github/workflows/publish.yml`

 * *Files 6% similar despite different names*

```diff
@@ -36,38 +36,29 @@
       # We upload to PyPI for all tag pushes, except tags ending in .dev
       upload_to_pypi: ${{ startsWith(github.ref, 'refs/tags/') && !endsWith(github.ref, '.dev') && (github.event_name == 'push' || github.event_name == 'workflow_dispatch') }}
 
       test_extras: test
       test_command: pytest -p no:warnings --pyargs photutils
       targets: |
         # Linux wheels
-        - cp38-manylinux_x86_64
         - cp39-manylinux_x86_64
         - cp310-manylinux_x86_64
         - cp311-manylinux_x86_64
 
         # MacOS X wheels
         # Note that the arm64 wheels are not actually tested so we rely
         # on local manual testing of these to make sure they are ok.
-        - cp38*macosx_x86_64
         - cp39*macosx_x86_64
         - cp310*macosx_x86_64
         - cp311*macosx_x86_64
 
-        - cp38*macosx_arm64
         - cp39*macosx_arm64
         - cp310*macosx_arm64
         - cp311*macosx_arm64
 
         # Windows wheels
-        - cp38*win32
-        - cp39*win32
-        - cp310*win32
-        - cp311*win32
-
-        - cp38*win_amd64
         - cp39*win_amd64
         - cp310*win_amd64
         - cp311*win_amd64
 
     secrets:
       pypi_token: ${{ secrets.pypi_token }}
```

### Comparing `photutils-1.8.0/.gitignore` & `photutils-1.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/.pre-commit-config.yaml` & `photutils-1.9.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -48,18 +48,18 @@
         # Detect mistake of inline code touching normal text in rst.
       - id: text-unicode-replacement-char
         # Forbid files which have a UTF-8 Unicode replacement character.
       - id: python-check-blanket-noqa
         # Enforce that all noqa annotations always occur with specific codes.
 
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.1
+    rev: v3.8.0
     hooks:
       - id: pyupgrade
-        args: ["--py38-plus"]
+        args: ["--py39-plus"]
         exclude: ".*(extern.*)$"
 
   - repo: https://github.com/pycqa/isort
     rev: 5.12.0
     hooks:
       - id: isort
         name: isort (python)
@@ -72,15 +72,15 @@
   - repo: https://github.com/PyCQA/flake8
     rev: 6.0.0
     hooks:
       - id: flake8
         args: ["--ignore", "E501,W503"]
 
   - repo: https://github.com/asottile/yesqa
-    rev: v1.4.0
+    rev: v1.5.0
     hooks:
       - id: yesqa
 
   # - repo: https://github.com/MarcoGorelli/absolufy-imports
   #   rev: v0.3.1
   #   hooks:
   #   - id: absolufy-imports
```

### Comparing `photutils-1.8.0/CHANGES.rst` & `photutils-1.9.0/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,78 @@
+1.9.0 (2023-08-14)
+------------------
+
+General
+^^^^^^^
+
+- The minimum required Python is now 3.9. [#1569]
+
+- The minimum required NumPy is now 1.22. [#1572]
+
+New Features
+^^^^^^^^^^^^
+
+- ``photutils.background``
+
+  - Added ``LocalBackground`` class for computing local backgrounds in a
+    circular annulus aperture. [#1556]
+
+- ``photutils.datasets``
+
+  - Added new ``make_test_psf_data`` function. [#1558, #1582, #1585]
+
+- ``photutils.psf``
+
+  - Propagate measurement uncertainties in PSF fitting. [#1543]
+
+  - Added new ``PSFPhotometry`` and ``IterativePSFPhotometry`` classes
+    for performing PSF-fitting photometry. [#1558, #1559, #1563, #1566,
+    #1567, #1581, #1586, #1590, #1594, #1603, #1604]
+
+  - Added a new ``SourceGrouper`` class. [#1558, #1605]
+
+  - Added a ``GriddedPSFModel`` ``fill_value`` attribute. [#1583]
+
+  - Added a ``grid_from_epsfs`` function to make a ``GriddedPSFModel``
+    from ePSFs. [#1596]
+
+  - Added a ``read`` method to ``GriddedPSFModel`` for reading "STDPSF"
+    FITS files containing grids of ePSF models. [#1557]
+
+  - Added a ``plot_grid`` method to ``GriddedPSFModel`` for plotting
+    ePSF grids. [#1557]
+
+  - Added a ``STDPSFGrid`` class for reading "STDPSF" FITS files
+    containing grids of ePSF models and plotting the ePSF grids. [#1557]
+
+
+Bug Fixes
+^^^^^^^^^
+
+- ``photutils.aperture``
+
+  - Fixed a bug in the validation of ``PixelAperture`` positions. [#1553]
+
+API Changes
+^^^^^^^^^^^
+
+- ``photutils.psf``
+
+  - Deprecated the PSF photometry classes ``BasicPSFPhotometry``,
+    ``IterativelySubtractedPSFPhotometry``, and
+    ``DAOPhotPSFPhotometry``. Use the new ``PSFPhotometry`` or
+    ``IterativePSFPhotometry`` class instead. [#1578]
+
+  - Deprecated the ``DAOGroup``, ``DBSCANGroup``, and ``GroupStarsBase``
+    classes. Use the new ``SourceGrouper`` class instead. [#1578]
+
+  - Deprecated the ``get_grouped_psf_model`` and ``subtract_psf``
+    function. [#1578]
+
+
 1.8.0 (2023-05-17)
 ------------------
 
 General
 ^^^^^^^
 
 - The minimum required Numpy is now 1.21. [#1528]
```

### Comparing `photutils-1.8.0/CONTRIBUTING.rst` & `photutils-1.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/LICENSE.rst` & `photutils-1.9.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/PKG-INFO` & `photutils-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: photutils
-Version: 1.8.0
+Version: 1.9.0
 Summary: An Astropy package for source detection and photometry
 Home-page: https://github.com/astropy/photutils
 Author: Photutils Developers
 Author-email: photutils.team@gmail.com
 License: BSD-3-Clause
 Keywords: astronomy,astrophysics,photometry,aperture,psf,source detection,background,segmentation,centroids,isophote,morphology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Astronomy
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Provides-Extra: all
 Provides-Extra: test
 Provides-Extra: docs
 License-File: LICENSE.rst
 
 =========
@@ -46,20 +46,20 @@
 
 If you use Photutils for a project that leads to a publication,
 whether directly or as a dependency of another package, please include
 the following acknowledgment::
 
     This research made use of Photutils, an Astropy package for
     detection and photometry of astronomical sources (Bradley et al.
-    20XX).
+    <YEAR>).
 
-where (Bradley et al. 20XX) is a citation to the `Zenodo record
-<https://doi.org/10.5281/zenodo.596036>`_ of the Photutils version
-that was used.  We also encourage citations in the main text wherever
-appropriate.  Please see the `CITATION
+where (Bradley et al. <YEAR>) is a citation to the `Zenodo record
+<https://doi.org/10.5281/zenodo.596036>`_ of the Photutils
+version that was used. We also encourage citations in the
+main text wherever appropriate. Please see the `CITATION
 <https://github.com/astropy/photutils/blob/main/photutils/CITATION.rst>`_
 file for details and an example BibTeX entry.
 
 
 License
 -------
```

### Comparing `photutils-1.8.0/README.rst` & `photutils-1.9.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -22,20 +22,20 @@
 
 If you use Photutils for a project that leads to a publication,
 whether directly or as a dependency of another package, please include
 the following acknowledgment::
 
     This research made use of Photutils, an Astropy package for
     detection and photometry of astronomical sources (Bradley et al.
-    20XX).
+    <YEAR>).
 
-where (Bradley et al. 20XX) is a citation to the `Zenodo record
-<https://doi.org/10.5281/zenodo.596036>`_ of the Photutils version
-that was used.  We also encourage citations in the main text wherever
-appropriate.  Please see the `CITATION
+where (Bradley et al. <YEAR>) is a citation to the `Zenodo record
+<https://doi.org/10.5281/zenodo.596036>`_ of the Photutils
+version that was used. We also encourage citations in the
+main text wherever appropriate. Please see the `CITATION
 <https://github.com/astropy/photutils/blob/main/photutils/CITATION.rst>`_
 file for details and an example BibTeX entry.
 
 
 License
 -------
```

### Comparing `photutils-1.8.0/docs/Makefile` & `photutils-1.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/docs/_static/favicon.ico` & `photutils-1.9.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/docs/_static/photutils_banner-475x120.png` & `photutils-1.9.0/docs/_static/photutils_banner-475x120.png`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/docs/_static/photutils_banner.pdf` & `photutils-1.9.0/docs/_static/photutils_banner.pdf`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/docs/_static/photutils_banner.svg` & `photutils-1.9.0/docs/_static/photutils_banner.svg`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/docs/_static/photutils_banner_original.svg` & `photutils-1.9.0/docs/_static/photutils_banner_original.svg`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/docs/_static/photutils_logo-32x32.png` & `photutils-1.9.0/docs/_static/photutils_logo-32x32.png`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/docs/_static/photutils_logo.svg` & `photutils-1.9.0/docs/_static/photutils_logo.svg`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/docs/aperture.rst` & `photutils-1.9.0/docs/aperture.rst`

 * *Files 0% similar despite different names*

```diff
@@ -152,20 +152,20 @@
 
 .. _photutils-aperture-overlap:
 
 Aperture and Pixel Overlap
 --------------------------
 
 The overlap of the aperture with the data pixels can be handled in
-different ways.  For the default method (``method='exact'``), the
-exact intersection of the aperture with each pixel is calculated.  The
+different ways.  The default method (``method='exact'``) calculates the
+exact intersection of the aperture with each pixel.  The
 other options, ``'center'`` and ``'subpixel'``, are faster, but with
-the expense of less precision.  For ``'center'``, a pixel is
+the expense of less precision.  With ``'center'``, a pixel is
 considered to be entirely in or out of the aperture depending on
-whether its center is in or out of the aperture.  For ``'subpixel'``,
+whether its center is in or out of the aperture.  With ``'subpixel'``,
 pixels are divided into a number of subpixels, which are in or out of
 the aperture based on their centers.  For this method, the number of
 subpixels needs to be set with the ``subpixels`` keyword.
 
 This example uses the ``'subpixel'`` method where pixels are resampled
 by a factor of 5 (``subpixels=5``) in each dimension::
 
@@ -278,15 +278,15 @@
 also can be used to calculate morphological properties
 like :attr:`~photutils.aperture.ApertureStats.centroid`,
 :attr:`~photutils.aperture.ApertureStats.fwhm`,
 :attr:`~photutils.aperture.ApertureStats.semimajor_sigma`,
 :attr:`~photutils.aperture.ApertureStats.semiminor_sigma`,
 :attr:`~photutils.aperture.ApertureStats.orientation`, and
 :attr:`~photutils.aperture.ApertureStats.eccentricity`. Please see
-:class:`~photutils.aperture.ApertureStats` for the the complete
+:class:`~photutils.aperture.ApertureStats` for the complete
 list of properties that can be calculated. The properties can be
 accessed using `~photutils.aperture.ApertureStats` attributes
 or output to an Astropy `~astropy.table.QTable` using the
 :meth:`~photutils.aperture.ApertureStats.to_table` method.
 
 Most of the source properties are calculated using the "center"
 :ref:`aperture-mask method <photutils-aperture-overlap>`, which gives
@@ -548,15 +548,15 @@
 Finally, the local background-subtracted sum within the circular
 apertures is::
 
     >>> apersum_bkgsub = aper_stats.sum - total_bkg
     >>> print(apersum_bkgsub)  # doctest: +FLOAT_CMP
     [750.80166351 346.51586233 872.75150158]
 
-Note that if you want to compute all of the source properties (i.e., in
+Note that if you want to compute all the source properties (i.e., in
 addition to only :attr:`~photutils.aperture.ApertureStats.sum`) on the
 local-background-subtracted data, you may input the *per-pixel* local
 background values to :class:`~photutils.aperture.ApertureStats` via the
 ``local_bkg`` keyword::
 
     >>> aper_stats_bkgsub = ApertureStats(data, aperture,
     ...                                   local_bkg=bkg_stats.median)
```

### Comparing `photutils-1.8.0/docs/background.rst` & `photutils-1.9.0/docs/background.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+.. _background:
+
 Background Estimation (`photutils.background`)
 ==============================================
 
 Introduction
 ------------
 
 To accurately measure the photometry and morphological properties
@@ -209,15 +211,15 @@
 a :class:`astropy.stats.SigmaClip` object to the ``sigma_clip``
 keyword. The default is to perform sigma clipping with ``sigma=3``
 and ``maxiters=10``. Sigma clipping can be turned off by setting
 ``sigma_clip=None``.
 
 After the background level has been determined in each of the boxes, the
 low-resolution background image can be median filtered, with a window
-of size of ``filter_size``, to suppress local under- or overestimations
+of size of ``filter_size``, to suppress local under or over estimations
 (e.g., due to bright galaxies in a particular box). Likewise, the median
 filter can be applied only to those boxes where the background level is
 above a specified threshold (``filter_threshold``).
 
 The low-resolution background and background RMS images are resized to
 the original data size using the function or callable object
 input via the ``interpolator`` keyword.  Photutils provides two
```

### Comparing `photutils-1.8.0/docs/centroids.rst` & `photutils-1.9.0/docs/centroids.rst`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/docs/conf.py` & `photutils-1.9.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,8 +181,7 @@
 
 # -- Options for linkcheck output ---------------------------------------------
 linkcheck_retry = 5
 linkcheck_ignore = ['http://data.astropy.org',
                     r'https://iraf.net/*',
                     r'https://github\.com/astropy/photutils/(?:issues|pull)/\d+']
 linkcheck_timeout = 180
-linkcheck_anchors = False
```

### Comparing `photutils-1.8.0/docs/contributing.rst` & `photutils-1.9.0/docs/contributing.rst`

 * *Files 8% similar despite different names*

```diff
@@ -31,8 +31,8 @@
 contributing fixes, code, or documentation (no git or GitHub
 experience necessary):
 
 * `How to make a code contribution <https://docs.astropy.org/en/latest/development/workflow/development_workflow.html>`_
 
 * `Coding Guidelines <https://docs.astropy.org/en/latest/development/codeguide.html>`_
 
-* `Developer Documentation <https://docs.astropy.org/en/latest/#developer-documentation>`_
+* `Developer Documentation <https://docs.astropy.org/en/latest/development/index.html>`_
```

### Comparing `photutils-1.8.0/docs/datasets.rst` & `photutils-1.9.0/docs/datasets.rst`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/docs/detection.rst` & `photutils-1.9.0/docs/detection.rst`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/docs/dev/releasing.rst` & `photutils-1.9.0/docs/dev/releasing.rst`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/docs/epsf.rst` & `photutils-1.9.0/docs/epsf.rst`

 * *Files 1% similar despite different names*

```diff
@@ -20,28 +20,28 @@
 Building an ePSF
 ----------------
 
 Photutils provides tools for building an ePSF following the
 prescription of `Anderson and King (2000; PASP 112, 1360)
 <https://ui.adsabs.harvard.edu/abs/2000PASP..112.1360A/abstract>`_
 and subsequent enhancements detailed mainly
-in `Anderson (2016; WFC3 ISR 2016-12
+in `Anderson (2016; WFC3 ISR 2016-12)
 <https://ui.adsabs.harvard.edu/abs/2016wfc..rept...12A/abstract>`_. The
 process involves iterating between the ePSF itself and the stars used to
 build it.
 
 To begin, we must first define a sample of stars used to build the
-ePSF.  Ideally these stars should be bright (high S/N) and isolated to
-prevent contamination from nearby stars.  One may use the star-finding
+ePSF. Ideally these stars should be bright (high S/N) and isolated to
+prevent contamination from nearby stars. One may use the star-finding
 tools in Photutils (e.g., :class:`~photutils.detection.DAOStarFinder`
-or :class:`~photutils.detection.IRAFStarFinder`) to identify an
-initial sample of stars.  However, the step of creating a good sample
-of stars will also likely require visual inspection and manual
-selection to ensure stars are sufficiently isolated and of good
-quality (e.g., no cosmic rays, detector artifacts, etc.).
+or :class:`~photutils.detection.IRAFStarFinder`) to identify an initial
+sample of stars. However, the step of creating a good sample of stars
+generally requires visual inspection and manual selection to ensure
+stars are sufficiently isolated and of good quality (e.g., no cosmic
+rays, detector artifacts, etc.).
 
 Let's start by loading a simulated HST/WFC3 image in the F160W band::
 
     >>> from photutils.datasets import load_simulated_hst_star_image
     >>> hdu = load_simulated_hst_star_image()  # doctest: +REMOTE_DATA
     >>> data = hdu.data  # doctest: +REMOTE_DATA
 
@@ -230,23 +230,22 @@
                            squeeze=True)
     ax = ax.ravel()
     for i in range(nrows * ncols):
         norm = simple_norm(stars[i], 'log', percent=99.0)
         ax[i].imshow(stars[i], norm=norm, origin='lower', cmap='viridis')
 
 With the star cutouts in hand, we are ready to construct the ePSF with
-the :class:`~photutils.psf.EPSFBuilder` class.  We'll create an ePSF
-with an oversampling factor of 4.0.  Here we limit the maximum number
-of iterations to 3 (to limit it's run time), but in practice one
-should use about 10 or more iterations.  The
-:class:`~photutils.psf.EPSFBuilder` class has many other options to
-control the ePSF build process, including changing the centering
-function, the smoothing kernel, and the centering accuracy.  Please
-see the :class:`~photutils.psf.EPSFBuilder` documentation for further
-details.
+the :class:`~photutils.psf.EPSFBuilder` class. We'll create an ePSF
+with an oversampling factor of 4.0. Here we limit the maximum number of
+iterations to 3 (to limit its run time), but in practice one should use
+about 10 or more iterations. The :class:`~photutils.psf.EPSFBuilder`
+class has many other options to control the ePSF build process,
+including changing the centering function, the smoothing kernel, and the
+centering accuracy. Please see the :class:`~photutils.psf.EPSFBuilder`
+documentation for further details.
 
 We first initialize an :class:`~photutils.psf.EPSFBuilder` instance
 with our desired parameters and then input the cutouts of our selected
 stars to the instance:
 
 .. doctest-requires:: scipy
 
@@ -314,10 +313,10 @@
     norm = simple_norm(epsf.data, 'log', percent=99.0)
     plt.imshow(epsf.data, norm=norm, origin='lower', cmap='viridis')
     plt.colorbar()
 
 The :class:`~photutils.psf.EPSFModel` object is a subclass of
 :class:`~photutils.psf.FittableImageModel`, thus it can be used
 as a PSF model for the :ref:`PSF-fitting machinery in Photutils
-<psf_photometry>` (i.e., `~photutils.psf.BasicPSFPhotometry`,
+<psf-photometry>` (i.e., `~photutils.psf.BasicPSFPhotometry`,
 `~photutils.psf.IterativelySubtractedPSFPhotometry`, or
 `~photutils.psf.DAOPhotPSFPhotometry`).
```

### Comparing `photutils-1.8.0/docs/getting_started.rst` & `photutils-1.9.0/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/docs/index.rst` & `photutils-1.9.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/docs/install.rst` & `photutils-1.9.0/docs/install.rst`

 * *Files 2% similar despite different names*

```diff
@@ -3,46 +3,46 @@
 ************
 
 Requirements
 ============
 
 Photutils has the following strict requirements:
 
-* `Python <https://www.python.org/>`_ 3.8 or later
+* `Python <https://www.python.org/>`_ 3.9 or later
 
-* `Numpy <https://numpy.org/>`_ 1.21 or later
+* `NumPy <https://numpy.org/>`_ 1.22 or later
 
 * `Astropy`_ 5.0 or later
 
 Photutils also optionally depends on other packages for some features:
 
-* `Scipy <https://www.scipy.org/>`_ 1.7.0 or later:  To power a variety of
+* `SciPy <https://scipy.org/>`_ 1.7.0 or later:  To power a variety of
   features in several modules (strongly recommended).
 
-* `matplotlib <https://matplotlib.org/>`_ 3.5.0 or later:  To power a
+* `Matplotlib <https://matplotlib.org/>`_ 3.5.0 or later:  To power a
   variety of plotting features (e.g., plotting apertures).
 
 * `scikit-image <https://scikit-image.org/>`_ 0.19.0 or later: Used for
   deblending segmented sources.
 
-* `scikit-learn <https://scikit-learn.org/>`_ 1.0 or later:  Used in
-  `~photutils.psf.DBSCANGroup` to create star groups.
+* `scikit-learn <https://scikit-learn.org/>`_ 1.0 or later: Used in the
+  deprecated `~photutils.psf.DBSCANGroup` class to create star groups.
 
-* `gwcs <https://github.com/spacetelescope/gwcs>`_ 0.18 or later:
+* `GWCS <https://gwcs.readthedocs.io/en/stable/>`_ 0.18 or later:
   Used in `~photutils.datasets.make_gwcs` to create a simple celestial
   gwcs object.
 
-* `bottleneck <https://github.com/pydata/bottleneck>`_: Improves the
+* `Bottleneck <https://github.com/pydata/bottleneck>`_: Improves the
   performance of sigma clipping and other functionality that may require
   computing statistics on arrays with NaN values.
 
 * `tqdm <https://tqdm.github.io/>`_: Used to display optional progress
   bars.
 
-* `rasterio <https://rasterio.readthedocs.io/>`_: Used for converting
+* `Rasterio <https://rasterio.readthedocs.io/>`_: Used for converting
   source segments into polygon objects.
 
 * `Shapely <https://shapely.readthedocs.io/>`_: Used for converting
   source segments into polygon objects.
 
 Photutils depends on `pytest-astropy
 <https://github.com/astropy/pytest-astropy>`_ (0.10 or later) to run
@@ -109,15 +109,15 @@
 do not need to install any other specific build dependencies (such as
 Cython) since these will be automatically installed into a temporary
 build environment by `pip`_.
 
 On Linux, using the package manager for your distribution will usually be
 the easiest route.
 
-On MacOS X you will need the `XCode`_ command-line tools, which can be
+On macOS you will need the `XCode`_ command-line tools, which can be
 installed using::
 
     xcode-select --install
 
 Follow the onscreen instructions to install the command-line tools
 required.  Note that you do not need to install the full `XCode`_
 distribution (assuming you are using MacOS X 10.9 or later).
```

### Comparing `photutils-1.8.0/docs/isophote.rst` & `photutils-1.9.0/docs/isophote.rst`

 * *Files 0% similar despite different names*

```diff
@@ -190,25 +190,25 @@
     plt.errorbar(isolist.sma, isolist.y0, yerr=isolist.y0_err, fmt='o',
                  markersize=4)
     plt.xlabel('Semimajor Axis Length (pix)')
     plt.ylabel('y0')
 
 We can build an elliptical model image from the
 `~photutils.isophote.IsophoteList` object using the
-:func:`~photutils.isophote.build_ellipse_model` function ( NOTE: this
+:func:`~photutils.isophote.build_ellipse_model` function (NOTE: this
 function requires `scipy <https://www.scipy.org/>`_):
 
 .. doctest-requires:: scipy
 
     >>> from photutils.isophote import build_ellipse_model
     >>> model_image = build_ellipse_model(data.shape, isolist)
     >>> residual = data - model_image
 
-Finally, let's plot the original data, overplotted with some of the
-isophotes, the elliptical model image, and the residual image:
+Finally, let's plot the original data, overplotted with some isophotes,
+the elliptical model image, and the residual image:
 
 .. plot::
 
     import matplotlib.pyplot as plt
     import numpy as np
     from astropy.modeling.models import Gaussian2D
     from photutils.datasets import make_noise_image
```

### Comparing `photutils-1.8.0/docs/isophote_faq.rst` & `photutils-1.9.0/docs/isophote_faq.rst`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 .. math::
 
     {\delta}_{\epsilon} = \frac {-2 B_{2} (1 - {\epsilon})} {I' a_0}
 
 .. math::
 
-    {\delta}_{\Theta} = \frac {2 A_{2} (1 - {\epsilon})} {I' a_0 [(1 - {\epsilon}) ^ 2 - 1 ]}
+    {\delta}_{\Theta} = \frac {2 A_{2} (1 - {\epsilon})} {I' a_0 [(1 - {\epsilon}) ^ 2 - 1]}
 
 where :math:`\epsilon` is the ellipticity, :math:`\Theta` is the
 position angle, :math:`A_i` and :math:`B_i` are the harmonic
 coefficients, and :math:`I'` is the derivative of the intensity along
 the major axis direction evaluated at a semimajor axis length of
 :math:`a_0`.
 
@@ -157,15 +157,15 @@
 Even when the chosen integration mode is not bilinear, the sampling
 algorithm resorts to it in case the number of sampled pixels inside
 any given sector is less than 5. It was found that bilinear mode gives
 smoother samples in those cases.
 
 Tests performed with artificial images showed that cosmic rays and
 defective pixels can be very effectively removed from the fit by a
-combination of median sampling and sigma-clipping.
+combination of median sampling and sigma clipping.
 
 
 6. How reliable are the fluxes computed by the `~photutils.isophote.Ellipse` algorithm?
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 The integrated fluxes and areas computed by
 `~photutils.isophote.Ellipse` were checked against results produced by
```

### Comparing `photutils-1.8.0/docs/make.bat` & `photutils-1.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/docs/morphology.rst` & `photutils-1.9.0/docs/morphology.rst`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/docs/overview.rst` & `photutils-1.9.0/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/docs/pixel_conventions.rst` & `photutils-1.9.0/docs/pixel_conventions.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Pixel Coordinate Conventions
 ----------------------------
 
-In Photutils, integer pixel coordinates fall at the center of pixels and
-they are 0-indexed, matching the Python 0-based indexing. That means the
-first pixel is considered pixel ``0``, but pixel coordinate ``0`` is
+In Photutils, integer pixel coordinates fall at the center of pixels,
+and they are 0-indexed, matching the Python 0-based indexing. That means
+the first pixel is considered pixel ``0``, but pixel coordinate ``0`` is
 the *center* of that pixel. Hence, the first pixel spans pixel values
 ``-0.5`` to ``0.5``.
 
 For a 2-dimensional array, ``(x, y) = (0, 0)`` corresponds to
 the *center* of the bottom, leftmost array element. That means
 the first pixel spans the ``x`` and ``y`` pixel values from
 ``-0.5`` to ``0.5``. Note that this differs from the IRAF, `FITS
```

### Comparing `photutils-1.8.0/docs/profiles.rst` & `photutils-1.9.0/docs/profiles.rst`

 * *Files 1% similar despite different names*

```diff
@@ -102,17 +102,17 @@
 .. doctest-skip::
 
     >>> rp.plot(label='Radial Profile')
     >>> rp.plot_error()
 
 .. plot::
 
+    import matplotlib.pyplot as plt
     import numpy as np
     from astropy.modeling.models import Gaussian2D
-
     from photutils.centroids import centroid_quadratic
     from photutils.datasets import make_noise_image
     from photutils.profiles import RadialProfile
 
     # create an artificial single source
     gmodel = Gaussian2D(42.1, 47.8, 52.4, 4.7, 4.7, 0)
     yy, xx = np.mgrid[0:100, 0:100]
@@ -138,15 +138,14 @@
 
 .. plot::
 
     import matplotlib.pyplot as plt
     import numpy as np
     from astropy.modeling.models import Gaussian2D
     from astropy.visualization import simple_norm
-
     from photutils.centroids import centroid_quadratic
     from photutils.datasets import make_noise_image
     from photutils.profiles import RadialProfile
 
     # create an artificial single source
     gmodel = Gaussian2D(42.1, 47.8, 52.4, 4.7, 4.7, 0)
     yy, xx = np.mgrid[0:100, 0:100]
@@ -189,15 +188,14 @@
 class:`~photutils.profiles.RadialProfile` radial profile:
 
 .. plot::
 
     import matplotlib.pyplot as plt
     import numpy as np
     from astropy.modeling.models import Gaussian2D
-
     from photutils.centroids import centroid_quadratic
     from photutils.datasets import make_noise_image
     from photutils.profiles import RadialProfile
 
     # create an artificial single source
     gmodel = Gaussian2D(42.1, 47.8, 52.4, 4.7, 4.7, 0)
     yy, xx = np.mgrid[0:100, 0:100]
@@ -269,15 +267,14 @@
     >>> rp.plot()
     >>> rp.plot_error()
 
 .. plot::
 
     import numpy as np
     from astropy.modeling.models import Gaussian2D
-
     from photutils.centroids import centroid_quadratic
     from photutils.datasets import make_noise_image
     from photutils.profiles import CurveOfGrowth
 
     # create an artificial single source
     gmodel = Gaussian2D(42.1, 47.8, 52.4, 4.7, 4.7, 0)
     yy, xx = np.mgrid[0:100, 0:100]
@@ -301,15 +298,14 @@
 
 .. plot::
 
     import matplotlib.pyplot as plt
     import numpy as np
     from astropy.modeling.models import Gaussian2D
     from astropy.visualization import simple_norm
-
     from photutils.centroids import centroid_quadratic
     from photutils.datasets import make_noise_image
     from photutils.profiles import CurveOfGrowth
 
     # create an artificial single source
     gmodel = Gaussian2D(42.1, 47.8, 52.4, 4.7, 4.7, 0)
     yy, xx = np.mgrid[0:100, 0:100]
```

### Comparing `photutils-1.8.0/docs/psf.rst` & `photutils-1.9.0/docs/psf.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,38 @@
-.. _psf_photometry:
+.. _psf-photometry:
 
 PSF Photometry (`photutils.psf`)
 ================================
 
-The `photutils.psf` module contains tools for model-fitting photometry,
-often called "PSF photometry".
+The `photutils.psf` subpackage contains tools for model-fitting
+photometry, often called "PSF photometry".
 
 .. _psf-terminology:
 
+
 Terminology
 -----------
-Different astronomy sub-fields use the terms "PSF", "PRF", or related
+Different astronomy subfields use the terms "PSF", "PRF", or related
 terms somewhat differently, especially when colloquial usage is taken
 into account. This package aims to be at the very least internally
 consistent, following the definitions described here.
 
-For this module we take Point Spread Function (PSF), or instrumental
-Point Spread Function (iPSF) to be the infinite resolution and
-infinite signal-to-noise flux distribution from a point source on
+We take the Point Spread Function (PSF), or instrumental Point
+Spread Function (iPSF) to be the infinite-resolution and
+infinite-signal-to-noise flux distribution from a point source on
 the detector, after passing through optics, dust, atmosphere, etc.
 By contrast, the function describing the responsivity variations
 across individual *pixels* is the Pixel Response Function (sometimes
 called "PRF", but that acronym is not used here for reasons that will
 soon be apparent). The convolution of the PSF and pixel response
 function, when discretized onto the detector (i.e., a rectilinear
 CCD grid), is the effective PSF (ePSF) or Point Response Function
-(PRF). (This latter terminology is the definition used by `Spitzer
+(PRF) (this latter terminology is the definition used by `Spitzer
 <https://irsa.ipac.caltech.edu/data/SPITZER/docs/dataanalysistools/tools
-/mopex/mopexusersguide/89/>`_. In many cases the PSF/ePSF/PRF
+/mopex/mopexusersguide/89/>`_). In many cases the PSF/ePSF/PRF
 distinction is unimportant, and the ePSF/PRF are simply called
 the "PSF", but the distinction can be critical when dealing
 carefully with undersampled data or detectors with significant
 intra-pixel sensitivity variations. For a more detailed
 description of this formalism, see `Anderson & King 2000
 <https://ui.adsabs.harvard.edu/abs/2000PASP..112.1360A/abstract>`_.
 
@@ -39,596 +40,599 @@
 to the more general task of model-fitting photometry (with the effects
 of the PSF either implicitly or explicitly included in the models),
 regardless of exactly what kind of model is actually being fit. For
 brevity (e.g., ``photutils.psf``), we use "PSF photometry" in this way,
 as a shorthand for the general approach.
 
 
-Building an effective PSF (ePSF)
---------------------------------
-
-Please see :ref:`build-epsf` for documentation on how to build an ePSF.
-
-
 PSF Photometry
 --------------
 
-Photutils provides a modular set of tools to perform PSF
-photometry for different science cases. These are implemented
-as separate classes to do sub-tasks of PSF photometry. It
-also provides high-level classes that connect these pieces
-together. In particular, it contains an implementation of the
-DAOPHOT algorithm (`~photutils.psf.DAOPhotPSFPhotometry`)
-proposed by `Stetson in his seminal paper
+Photutils provides a modular set of tools to perform PSF photometry
+for different science cases. The tools are implemented as classes that
+perform various subtasks of PSF photometry. High-level classes are also
+provided to connect these pieces together.
+
+The two main PSF-photometry classes are `~photutils.psf.PSFPhotometry`
+and `~photutils.psf.IterativePSFPhotometry`.
+`~photutils.psf.PSFPhotometry` provides the framework for a flexible PSF
+photometry workflow that can find sources in an image, optionally group
+overlapping sources, fit the PSF model to the sources, and subtract the
+fit PSF models from the image. `~photutils.psf.IterativePSFPhotometry`
+is an iterative version of `~photutils.psf.PSFPhotometry` where
+after the fit sources are subtracted, the process repeats until no
+additional sources are detected or a maximum number of iterations has
+been reached. When used with the `~photutils.detection.DAOStarFinder`,
+`~photutils.psf.IterativePSFPhotometry` is essentially an implementation
+of the DAOPHOT algorithm described by Stetson in his `seminal paper
 <https://ui.adsabs.harvard.edu/abs/1987PASP...99..191S/abstract>`_ for
 crowded-field stellar photometry.
 
-The DAOPHOT algorithm consists in applying the loop FIND, GROUP, NSTAR,
-SUBTRACT, FIND until no more stars are detected or a given number of
-iterations is reached. Basically, `~photutils.psf.DAOPhotPSFPhotometry`
-works as follows. The first step is to estimate the sky background. For
-this task, photutils provides several classes to compute scalar and 2D
-backgrounds, see `~photutils.background` for details. The next step is
-to find an initial estimate of the positions of potential sources. This
-can be accomplished by using source detection algorithms, which are
-implemented in `~photutils.detection`.
+The star-finding step is controlled by the ``finder``
+keyword, where one inputs a callable function or class
+instance. Typically, this would be one of the star-detection
+classes implemented in the `photutils.detection`
+subpackage, e.g., `~photutils.detection.DAOStarFinder`,
+`~photutils.detection.IRAFStarFinder`, or
+`~photutils.detection.StarFinder`.
 
-After finding sources, one would apply a clustering algorithm in
-order to label the sources according to groups. Usually, those
+After finding sources, one can optionally apply a clustering algorithm
+to group overlapping sources using the ``grouper`` keyword. Usually,
 groups are formed by a distance criterion, which is the case of the
-grouping algorithm proposed by Stetson. In `~photutils.psf.DAOGroup`,
-we provide an implementation of that algorithm. In addition,
-`~photutils.psf.DBSCANGroup` can also be used to group sources with more
-complex distance criteria. The reason behind the construction of groups
-is illustrated as follows: imagine that one would like to fit 300 stars
-and the model for each star has three parameters to be fitted. If one
-constructs a single model to fit the 300 stars simultaneously, then the
-optimization algorithm will have to search for the solution in a 900
-dimensional space, which is computationally expensive and error-prone.
-Reducing the stars in groups effectively reduces the dimension of the
-parameter space, which facilitates the optimization process.
-
-Provided that the groups are available, the next step is
-to fit the sources simultaneously for each group. This
-task can be done using an astropy fitter, for instance,
-`~astropy.modeling.fitting.LevMarLSQFitter`.
-
-After sources are fitted, they are subtracted from the given image and,
-after fitting all sources, the residual image is analyzed by the finding
-routine again in order to check if there exist any source which has not
-been detected previously. This process goes on until no more sources are
-identified by the finding routine.
-
-.. note::
-    It is important to note the conventions on the column names of the
-    input/output astropy Tables which are passed along to the source
-    detection and photometry objects. For instance, all source detection
-    objects should output a table with columns named as ``xcentroid``
-    and ``ycentroid`` (check `~photutils.detection`). On the other
-    hand, `~photutils.psf.DAOGroup` expects columns named as ``x_0``
-    and ``y_0``, which represents the initial guesses on the sources'
-    centroids. Finally, the output of the fitting process shows columns
-    named as ``x_fit``, ``y_fit``, ``flux_fit`` for the optimum values
-    and ``x_0``, ``y_0``, ``flux_0`` for the initial guesses. Although
-    this convention implies that the columns have to be renamed along
-    the process, it has the advantage of clarity so that one can keep
-    track and easily differentiate where input/outputs came from.
-
-
-High-Level Structure
-^^^^^^^^^^^^^^^^^^^^
-
-Photutils provides three classes to perform PSF
-Photometry: `~photutils.psf.BasicPSFPhotometry`,
-`~photutils.psf.IterativelySubtractedPSFPhotometry`, and
-`~photutils.psf.DAOPhotPSFPhotometry`. Together these provide the core
-workflow to make photometric measurements given an appropriate PSF (or
-other) model.
-
-`~photutils.psf.BasicPSFPhotometry` implements the minimum tools for
-model-fitting photometry. At its core, this involves finding sources
-in an image, grouping overlapping sources into a single model, fitting
-the model to the sources, and subtracting the models from the image. In
-DAOPHOT parlance, this is essentially running the "FIND, GROUP, NSTAR,
-SUBTRACT" once. Because it is only a single cycle of that sequence, this
-class should be used when the degree of crowdedness of the field is not
-very high, for instance, when most stars are separated by a distance no
-less than one FWHM and their brightness are relatively uniform. It is
-critical to understand, though, that `~photutils.psf.BasicPSFPhotometry`
-does not actually contain the functionality to *do* all these steps -
-that is provided by other objects (or can be user-written) functions.
-Rather, it provides the framework and data structures in which these
-operations run. Because of this, `~photutils.psf.BasicPSFPhotometry` is
-particularly useful for build more complex workflows, as all the stages
-can be turned on or off or replaced with different implementations as
-the user desires.
-
-`~photutils.psf.IterativelySubtractedPSFPhotometry` is similar to
-`~photutils.psf.BasicPSFPhotometry`, but it adds a parameter called
-``n_iters`` which is the number of iterations for which the loop
-"FIND, GROUP, NSTAR, SUBTRACT, FIND..." will be performed. This class
-enables photometry in a scenario where there exists significant overlap
-between stars that are of quite different brightness. For instance,
-the detection algorithm may not be able to detect a faint and bright
-star very close together in the first iteration, but they will be
-detected in the next iteration after the brighter stars have been fit
-and subtracted. Like `~photutils.psf.BasicPSFPhotometry`, it does not
-include implementations of the stages of this process, but it provides
-the structure in which those stages run.
-
-`~photutils.psf.DAOPhotPSFPhotometry` is a special case of
-`~photutils.psf.IterativelySubtractedPSFPhotometry`. Unlike
-`~photutils.psf.IterativelySubtractedPSFPhotometry` and
-`~photutils.psf.BasicPSFPhotometry`, the class includes specific
-implementations of the stages of the photometric measurements, tuned to
-reproduce the algorithms used for the DAOPHOT code. Specifically, the
-``finder``, ``group_maker``, ``bkg_estimator`` attributes are set to
-the `~photutils.detection.DAOStarFinder`, `~photutils.psf.DAOGroup`,
-and `~photutils.background.MMMBackground`, respectively. Therefore,
-users need to input the parameters of those classes to set up a
-`~photutils.psf.DAOPhotPSFPhotometry` object, rather than providing
-objects to do these stages (which is what the other classes require).
-
-Those classes and all the classes they *use* for the steps in the
-photometry process can always be replaced by user-supplied functions
-if you wish to customize any stage of the photometry process. This
-makes the machinery very flexible, while still providing a "batteries
-included" approach with a default implementation that's suitable for
-many use cases.
-
-Basic Usage
-^^^^^^^^^^^
-
-The basic usage of, e.g.,
-`~photutils.psf.IterativelySubtractedPSFPhotometry` is as follows:
-
-.. doctest-skip::
-
-    >>> from photutils.psf import IterativelySubtractedPSFPhotometry
-    >>> my_photometry = IterativelySubtractedPSFPhotometry(
-    ...     finder=my_finder, group_maker=my_group_maker,
-    ...     bkg_estimator=my_bkg_estimator, psf_model=my_psf_model,
-    ...     fitter=my_fitter, niters=3, fitshape=(7, 7))
-    >>> # get photometry results
-    >>> photometry_results = my_photometry(image=my_image)
-    >>> # get residual image
-    >>> residual_image = my_photometry.get_residual_image()
-
-Where ``my_finder``, ``my_group_maker``, and ``my_bkg_estimator``
-may be any suitable class or callable function. This approach allows
-one to customize every part of the photometry process provided that
-their input/output are compatible with the input/output expected by
-`~photutils.psf.IterativelySubtractedPSFPhotometry`. `photutils.psf`
-provides all the necessary classes to reproduce the DAOPHOT algorithm,
-but any individual part of that algorithm can be swapped for a
-user-defined function. See the API documentation for precise details on
-what these classes or functions should look like.
+grouping algorithm proposed by Stetson. Stars that grouped are fit
+simultaneously. The reason behind the construction of groups and not
+fitting all stars simultaneously is illustrated as follows: imagine
+that one would like to fit 300 stars and the model for each star has
+three parameters to be fitted. If one constructs a single model to fit
+the 300 stars simultaneously, then the optimization algorithm will
+have to search for the solution in a 900-dimensional space, which
+is computationally expensive and error-prone. Having smaller groups
+of stars effectively reduces the dimension of the parameter space,
+which facilitates the optimization process. For more details see
+:ref:`psf-grouping`.
+
+The local background around each source can optionally be subtracted
+using the ``localbkg_estimator`` keyword. This keyword accepts a
+`~photutils.background.LocalBackground` instance that estimates the
+local statistics in a circular annulus aperture centered on each source.
+The size of the annulus and the statistic function can be configured in
+`~photutils.background.LocalBackground`.
+
+The next step is to fit the sources and/or groups. This
+task is performed using an astropy fitter, for example
+`~astropy.modeling.fitting.LevMarLSQFitter`, input via the ``fitter``
+keyword. The shape of the region to be fitted can be configured using
+the ``fit_shape`` parameter. In general, ``fit_shape`` should be set
+to a small size (e.g., (5, 5)) that covers the central star region
+with the highest flux signal-to-noise. The initial positions are
+derived from the ``finder`` algorithm. The initial flux values for the
+fit are derived from measuring the flux in a circular aperture with
+radius ``aperture_radius``. The initial positions and fluxes can be
+alternatively input via the ``init_params`` keyword when calling the
+class.
+
+After sources are fitted, a model image of the fit
+sources or a residual image can be generated using the
+:meth:`~photutils.psf.PSFPhotometry.make_model_image` and
+:meth:`~photutils.psf.PSFPhotometry.make_residual_image` methods,
+respectively.
+
+For `~photutils.psf.IterativePSFPhotometry`, the above steps can be
+repeated until no additional sources are detected (or until a maximum
+number of iterations).
+
+The `~photutils.psf.PSFPhotometry` and
+`~photutils.psf.IterativePSFPhotometry` classes provide the structure
+in which the PSF-fitting steps described above are performed, but
+all the stages can be turned on or off or replaced with different
+implementations as the user desires. This makes the tools very flexible.
+One can also bypass several of the steps by directly inputting to
+``init_params`` an astropy table containing the initial parameters for
+the source centers, fluxes, group identifiers, and local backgrounds.
+This is also useful if one is interested in fitting only one or a few
+sources in an image.
 
-Performing PSF Photometry
-^^^^^^^^^^^^^^^^^^^^^^^^^
+Example Usage
+-------------
 
-Let's take a look at a simple example with simulated stars whose PSF is
-assumed to be Gaussian.
+Let's start with a simple example using simulated stars whose PSF is
+assumed to be Gaussian. We'll create a synthetic image using tools
+provided by the :ref:`photutils.datasets <datasets>` module:
 
-First let's create an image with four overlapping stars::
+.. doctest-requires:: scipy
 
     >>> import numpy as np
-    >>> from astropy.table import Table
-    >>> from photutils.datasets import (make_gaussian_sources_image,
-    ...                                 make_noise_image)
-    >>> sigma_psf = 2.0
-    >>> sources = Table()
-    >>> sources['flux'] = [700, 800, 700, 800]
-    >>> sources['x_mean'] = [12, 17, 12, 17]
-    >>> sources['y_mean'] = [15, 15, 20, 20]
-    >>> sources['x_stddev'] = sigma_psf * np.ones(4)
-    >>> sources['y_stddev'] = sources['x_stddev']
-    >>> sources['theta'] = [0, 0, 0, 0]
-    >>> sources['id'] = [1, 2, 3, 4]
-    >>> tshape = (32, 32)
-    >>> image = (make_gaussian_sources_image(tshape, sources) +
-    ...          make_noise_image(tshape, distribution='poisson', mean=6.0,
-    ...                           seed=123) +
-    ...          make_noise_image(tshape, distribution='gaussian', mean=0.0,
-    ...                           stddev=2.0, seed=123))
-
-.. doctest-requires:: matplotlib
-
-    >>> import matplotlib.pyplot as plt
-    >>> from matplotlib import rcParams
-    >>> rcParams['font.size'] = 13
-    >>> plt.imshow(image, cmap='viridis', aspect=1, interpolation='nearest',
-    ...            origin='lower')  # doctest: +SKIP
-    >>> plt.title('Simulated data')  # doctest: +SKIP
-    >>> plt.colorbar(orientation='horizontal', fraction=0.046, pad=0.04)  # doctest: +SKIP
+    >>> from photutils.datasets import make_test_psf_data, make_noise_image
+    >>> from photutils.psf import IntegratedGaussianPRF
+    >>> psf_model = IntegratedGaussianPRF(flux=1, sigma=2.7 / 2.35)
+    >>> psf_shape = (25, 25)
+    >>> nsources = 10
+    >>> shape = (101, 101)
+    >>> data, true_params = make_test_psf_data(shape, psf_model, psf_shape,
+    ...                                        nsources, flux_range=(500, 700),
+    ...                                        min_separation=10, seed=0)
+    >>> noise = make_noise_image(data.shape, mean=0, stddev=1, seed=0)
+    >>> data += noise
+    >>> error = np.abs(noise)
+
+Let's plot the image:
 
 .. plot::
 
     import matplotlib.pyplot as plt
-    import numpy as np
-    from astropy.table import Table
-    from matplotlib import rcParams
-    from photutils.datasets import (make_gaussian_sources_image,
-                                    make_noise_image)
-
-    sigma_psf = 2.0
-    sources = Table()
-    sources['flux'] = [700, 800, 700, 800]
-    sources['x_mean'] = [12, 17, 12, 17]
-    sources['y_mean'] = [15, 15, 20, 20]
-    sources['x_stddev'] = sigma_psf * np.ones(4)
-    sources['y_stddev'] = sources['x_stddev']
-    sources['theta'] = [0, 0, 0, 0]
-    sources['id'] = [1, 2, 3, 4]
-    tshape = (32, 32)
-    image = (make_gaussian_sources_image(tshape, sources)
-             + make_noise_image(tshape, distribution='poisson', mean=6.0,
-                                seed=123)
-             + make_noise_image(tshape, distribution='gaussian', mean=0.0,
-                                stddev=2.0, seed=123))
-
-    rcParams['font.size'] = 13
-
-    plt.imshow(image, cmap='viridis', aspect=1, interpolation='nearest',
-               origin='lower')
-    plt.title('Simulated data')
-    plt.colorbar(orientation='horizontal', fraction=0.046, pad=0.04)
-
-Then let's import the required classes to set up a
-`~photutils.psf.IterativelySubtractedPSFPhotometry` object::
-
-    >>> from astropy.modeling.fitting import LevMarLSQFitter
-    >>> from astropy.stats import gaussian_sigma_to_fwhm
-    >>> from photutils.background import MADStdBackgroundRMS, MMMBackground
-    >>> from photutils.detection import IRAFStarFinder
-    >>> from photutils.psf import (DAOGroup, IntegratedGaussianPRF,
-    ...                            IterativelySubtractedPSFPhotometry)
-
-Let's then instantiate and use the objects:
-
-.. doctest-requires:: scipy
-
-    >>> bkgrms = MADStdBackgroundRMS()
-    >>> std = bkgrms(image)
-    >>> iraffind = IRAFStarFinder(threshold=3.5*std,
-    ...                           fwhm=sigma_psf * gaussian_sigma_to_fwhm,
-    ...                           minsep_fwhm=0.01, roundhi=5.0, roundlo=-5.0,
-    ...                           sharplo=0.0, sharphi=2.0)
-    >>> daogroup = DAOGroup(2.0 * sigma_psf * gaussian_sigma_to_fwhm)
-    >>> mmm_bkg = MMMBackground()
-    >>> fitter = LevMarLSQFitter()
-    >>> psf_model = IntegratedGaussianPRF(sigma=sigma_psf)
-    >>> photometry = IterativelySubtractedPSFPhotometry(finder=iraffind,
-    ...                                                 group_maker=daogroup,
-    ...                                                 bkg_estimator=mmm_bkg,
-    ...                                                 psf_model=psf_model,
-    ...                                                 fitter=LevMarLSQFitter(),
-    ...                                                 niters=1, fitshape=(11, 11))
-    >>> result_tab = photometry(image=image)
-    >>> residual_image = photometry.get_residual_image()
-
-Note that the parameters values for the finder class, i.e.,
-`~photutils.detection.IRAFStarFinder`, are completely chosen in an
-arbitrary manner and optimum values do vary according to the data.
-
-As mentioned before, the way to actually do the photometry is by using
-``photometry`` as a function-like call.
-
-It's worth noting that ``image`` does not need to be background
-subtracted. The subtraction is done during the photometry process with
-the attribute ``bkg`` that was used to set up ``photometry``.
+    from photutils.datasets import make_noise_image, make_test_psf_data
+    from photutils.psf import IntegratedGaussianPRF
 
-Now, let's compare the simulated and the residual images:
+    psf_model = IntegratedGaussianPRF(flux=1, sigma=2.7 / 2.35)
+    psf_shape = (25, 25)
+    nsources = 10
+    shape = (101, 101)
+    data, true_params = make_test_psf_data(shape, psf_model, psf_shape,
+                                           nsources, flux_range=(500, 700),
+                                           min_separation=10, seed=0)
+    noise = make_noise_image(data.shape, mean=0, stddev=1, seed=0)
+    data += noise
+    plt.imshow(data, origin='lower')
+    plt.title('Simulated Data')
+    plt.colorbar()
+
+
+Fitting multiple stars
+^^^^^^^^^^^^^^^^^^^^^^
+
+Now let's use `~photutils.psf.PSFPhotometry` to perform PSF photometry
+on the stars in this image. Note that the input image must be
+background-subtracted prior to using the photometry classes. See
+:ref:`background` for tools to subtract a global background from an
+image. This is not needed for our synthetic image because it does not
+include background.
+
+We'll use the `~photutils.detection.DAOStarFinder` class for
+source detection. We'll estimate the initial fluxes of each
+source using a circular aperture with a radius 4 pixels. The
+central 5x5 pixel region of each star will be fit using an
+`~photutils.psf.IntegratedGaussianPRF` PSF model. First, let's create an
+instance of the `~photutils.psf.PSFPhotometry` class:
 
-.. doctest-skip::
-
-    >>> plt.subplot(1, 2, 1)
-    >>> plt.imshow(image, cmap='viridis', aspect=1, interpolation='nearest',
-                   origin='lower')
-    >>> plt.title('Simulated data')
-    >>> plt.colorbar(orientation='horizontal', fraction=0.046, pad=0.04)
-    >>> plt.subplot(1, 2, 2)
-    >>> plt.imshow(residual_image, cmap='viridis', aspect=1,
-    ...            interpolation='nearest', origin='lower')
-    >>> plt.title('Residual Image')
-    >>> plt.colorbar(orientation='horizontal', fraction=0.046, pad=0.04)
-    >>> plt.show()
+.. doctest-requires:: scipy
 
-.. plot::
+    >>> from photutils.detection import DAOStarFinder
+    >>> from photutils.psf import PSFPhotometry
+    >>> psf_model = IntegratedGaussianPRF(flux=1, sigma=2.7 / 2.35)
+    >>> fit_shape = (5, 5)
+    >>> finder = DAOStarFinder(6.0, 2.0)
+    >>> psfphot = PSFPhotometry(psf_model, fit_shape, finder=finder,
+    ...                         aperture_radius=4)
+
+To perform the PSF fitting, we then call the class instance
+on the data array, and optionally an error and mask array. A
+`~astropy.nddata.NDData` object holding the data, error, and mask arrays
+can also be input into the ``data`` parameter. Note that all non-finite
+(e.g., NaN or inf) data values are automatically masked. Here we input
+the data and error arrays:
 
-    import matplotlib.pyplot as plt
-    import numpy as np
-    from astropy.modeling.fitting import LevMarLSQFitter
-    from astropy.stats import gaussian_sigma_to_fwhm
-    from astropy.table import Table
-    from matplotlib import rcParams
-    from photutils.background import MADStdBackgroundRMS, MMMBackground
-    from photutils.datasets import (make_gaussian_sources_image,
-                                    make_noise_image)
-    from photutils.detection import IRAFStarFinder
-    from photutils.psf import (DAOGroup, IntegratedGaussianPRF,
-                               IterativelySubtractedPSFPhotometry)
-
-    sigma_psf = 2.0
-    sources = Table()
-    sources['flux'] = [700, 800, 700, 800]
-    sources['x_mean'] = [12, 17, 12, 17]
-    sources['y_mean'] = [15, 15, 20, 20]
-    sources['x_stddev'] = sigma_psf * np.ones(4)
-    sources['y_stddev'] = sources['x_stddev']
-    sources['theta'] = [0, 0, 0, 0]
-    sources['id'] = [1, 2, 3, 4]
-    tshape = (32, 32)
-    image = (make_gaussian_sources_image(tshape, sources)
-             + make_noise_image(tshape, distribution='poisson', mean=6.0,
-                                seed=123)
-             + make_noise_image(tshape, distribution='gaussian', mean=0.0,
-                                stddev=2.0, seed=123))
-
-    bkgrms = MADStdBackgroundRMS()
-    std = bkgrms(image)
-    iraffind = IRAFStarFinder(threshold=3.5 * std,
-                              fwhm=sigma_psf * gaussian_sigma_to_fwhm,
-                              minsep_fwhm=0.01, roundhi=5.0, roundlo=-5.0,
-                              sharplo=0.0, sharphi=2.0)
-    daogroup = DAOGroup(2.0 * sigma_psf * gaussian_sigma_to_fwhm)
-    mmm_bkg = MMMBackground()
-    psf_model = IntegratedGaussianPRF(sigma=sigma_psf)
-    fitter = LevMarLSQFitter()
-
-    photometry = IterativelySubtractedPSFPhotometry(finder=iraffind,
-                                                    group_maker=daogroup,
-                                                    bkg_estimator=mmm_bkg,
-                                                    psf_model=psf_model,
-                                                    fitter=LevMarLSQFitter(),
-                                                    niters=1, fitshape=(11, 11))
-    result_tab = photometry(image=image)
-    residual_image = photometry.get_residual_image()
-
-    rcParams['font.size'] = 13
-    plt.subplot(1, 2, 1)
-    plt.imshow(image, cmap='viridis', aspect=1, interpolation='nearest',
-               origin='lower')
-    plt.title('Simulated data')
-    plt.colorbar(orientation='horizontal', fraction=0.046, pad=0.04)
-    plt.subplot(1, 2, 2)
-    plt.imshow(residual_image, cmap='viridis', aspect=1,
-               interpolation='nearest', origin='lower')
-    plt.title('Residual Image')
-    plt.colorbar(orientation='horizontal', fraction=0.046, pad=0.04)
-    plt.show()
+.. doctest-requires:: scipy
 
-Performing PSF Photometry with Fixed Centroids
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+    >>> phot = psfphot(data, error=error)
 
-In case that the centroids positions of the stars are known a priori,
-then they can be held fixed during the fitting process and the optimizer
-will only consider flux as a variable. To do that, one has to set the
-``fixed`` attribute for the centroid parameters in ``psf`` as ``True``.
+A table of initial PSF model parameter values can also be input when
+calling the class instance. An example of that is shown later.
 
-Consider the previous example after the line ``psf_model =
-IntegratedGaussianPRF(sigma=sigma_psf)``:
+Equivalently, one can input an `~astropy.nddata.NDData` object with any
+uncertainty object that can be converted to standard-deviation errors:
 
 .. doctest-skip::
 
-    >>> psf_model.x_0.fixed = True
-    >>> psf_model.y_0.fixed = True
-    >>> pos = Table(names=['x_0', 'y_0'], data=[sources['x_mean'],
-    ...                                         sources['y_mean']])
+    >>> from astropy.nddata import NDData, StdDevUncertainty
+    >>> uncertainty = StdDevUncertainty(error)
+    >>> nddata = NDData(data, uncertainty=uncertainty)
+    >>> phot2 = psfphot(nddata)
+
+The result is an astropy `~astropy.table.Table` with columns for the
+source and group identification numbers, the x, y, and flux initial,
+fit, and error values, local background, number of unmasked pixels
+fit, the group size, quality-of-fit metrics, and flags. See the
+`~photutils.psf.PSFPhotometry` documentation for descriptions of the
+output columns.
 
-.. doctest-skip::
+The full table cannot be shown here as it has many columns, but let's
+print the source ID along with the fit x, y, and flux values:
 
-    >>> photometry = BasicPSFPhotometry(group_maker=daogroup,
-    ...                                 bkg_estimator=mmm_bkg,
-    ...                                 psf_model=psf_model,
-    ...                                 fitter=LevMarLSQFitter(),
-    ...                                 fitshape=(11, 11))
-    >>> result_tab = photometry(image=image, init_guesses=pos)
-    >>> residual_image = photometry.get_residual_image()
+.. doctest-requires:: scipy
 
-.. doctest-skip::
+    >>> phot['x_fit'].info.format = '.4f'  # optional format
+    >>> phot['y_fit'].info.format = '.4f'
+    >>> phot['flux_fit'].info.format = '.4f'
+    >>> print(phot[('id', 'x_fit', 'y_fit', 'flux_fit')])  # doctest: +FLOAT_CMP
+     id  x_fit   y_fit  flux_fit
+    --- ------- ------- --------
+      1 32.7715 12.2210 627.4274
+      2 13.2700 14.5841 507.5778
+      3 63.6483 22.3907 640.9277
+      4 82.2847 25.5223 662.0007
+      5 41.5416 35.8893 687.8236
+      6 21.5721 41.9480 620.8562
+      7 14.1823 65.0090 681.7447
+      8 61.8363 67.5560 608.2459
+      9 74.6206 68.1855 502.8906
+     10 15.1685 78.0373 558.0204
+
+Let's create the residual image:
+
+.. doctest-requires:: scipy
 
-    >>> plt.subplot(1, 2, 1)
-    >>> plt.imshow(image, cmap='viridis', aspect=1,
-    ...            interpolation='nearest', origin='lower')
-    >>> plt.title('Simulated data')
-    >>> plt.colorbar(orientation='horizontal', fraction=0.046, pad=0.04)
-    >>> plt.subplot(1, 2, 2)
-    >>> plt.imshow(residual_image, cmap='viridis', aspect=1,
-    ...            interpolation='nearest', origin='lower')
-    >>> plt.title('Residual Image')
-    >>> plt.colorbar(orientation='horizontal', fraction=0.046, pad=0.04)
+    >>> resid = psfphot.make_residual_image(data, (25, 25))
+
+and plot it:
 
 .. plot::
 
     import matplotlib.pyplot as plt
     import numpy as np
-    from astropy.modeling.fitting import LevMarLSQFitter
-    from astropy.stats import gaussian_sigma_to_fwhm
-    from astropy.table import Table
-    from matplotlib import rcParams
-    from photutils.background import MADStdBackgroundRMS, MMMBackground
-    from photutils.datasets import (make_gaussian_sources_image,
-                                    make_noise_image)
-    from photutils.psf import (BasicPSFPhotometry, DAOGroup,
-                               IntegratedGaussianPRF)
-
-    sigma_psf = 2.0
-    sources = Table()
-    sources['flux'] = [700, 800, 700, 800]
-    sources['x_mean'] = [12, 17, 12, 17]
-    sources['y_mean'] = [15, 15, 20, 20]
-    sources['x_stddev'] = sigma_psf * np.ones(4)
-    sources['y_stddev'] = sources['x_stddev']
-    sources['theta'] = [0, 0, 0, 0]
-    sources['id'] = [1, 2, 3, 4]
-    tshape = (32, 32)
-    image = (make_gaussian_sources_image(tshape, sources)
-             + make_noise_image(tshape, distribution='poisson', mean=6.0,
-                                seed=123)
-             + make_noise_image(tshape, distribution='gaussian', mean=0.0,
-                                stddev=2.0, seed=123))
-
-    bkgrms = MADStdBackgroundRMS()
-    std = bkgrms(image)
-    daogroup = DAOGroup(2.0 * sigma_psf * gaussian_sigma_to_fwhm)
-    mmm_bkg = MMMBackground()
-    psf_model = IntegratedGaussianPRF(sigma=sigma_psf)
-
-    psf_model.x_0.fixed = True
-    psf_model.y_0.fixed = True
-
-    pos = Table(names=['x_0', 'y_0'], data=[sources['x_mean'],
-                                            sources['y_mean']])
-
-    fitter = LevMarLSQFitter()
-
-    photometry = BasicPSFPhotometry(group_maker=daogroup,
-                                    bkg_estimator=mmm_bkg,
-                                    psf_model=psf_model,
-                                    fitter=LevMarLSQFitter(),
-                                    fitshape=(11, 11))
-
-    result_tab = photometry(image=image, init_guesses=pos)
-    residual_image = photometry.get_residual_image()
-
-    rcParams['font.size'] = 13
-    plt.subplot(1, 2, 1)
-    plt.imshow(image, cmap='viridis', aspect=1, interpolation='nearest',
-               origin='lower')
-    plt.title('Simulated data')
-    plt.colorbar(orientation='horizontal', fraction=0.046, pad=0.04)
-    plt.subplot(1, 2, 2)
-    plt.imshow(residual_image, cmap='viridis', aspect=1,
-               interpolation='nearest', origin='lower')
-    plt.title('Residual Image')
-    plt.colorbar(orientation='horizontal', fraction=0.046, pad=0.04)
-    plt.show()
+    from astropy.visualization import simple_norm
+    from photutils.datasets import make_noise_image, make_test_psf_data
+    from photutils.detection import DAOStarFinder
+    from photutils.psf import IntegratedGaussianPRF, PSFPhotometry
+
+    psf_model = IntegratedGaussianPRF(flux=1, sigma=2.7 / 2.35)
+    psf_shape = (25, 25)
+    nsources = 10
+    shape = (101, 101)
+    data, true_params = make_test_psf_data(shape, psf_model, psf_shape,
+                                           nsources, flux_range=(500, 700),
+                                           min_separation=10, seed=0)
+    noise = make_noise_image(data.shape, mean=0, stddev=1, seed=0)
+    data += noise
+    error = np.abs(noise)
+
+    psf_model = IntegratedGaussianPRF(flux=1, sigma=2.7 / 2.35)
+    fit_shape = (5, 5)
+    finder = DAOStarFinder(6.0, 2.0)
+    psfphot = PSFPhotometry(psf_model, fit_shape, finder=finder,
+                            aperture_radius=4)
+    phot = psfphot(data, error=error)
+
+    resid = psfphot.make_residual_image(data, (25, 25))
+
+    fig, ax = plt.subplots(nrows=1, ncols=3, figsize=(15, 5))
+    norm = simple_norm(data, 'sqrt', percent=99)
+    ax[0].imshow(data, origin='lower', norm=norm)
+    ax[1].imshow(data - resid, origin='lower', norm=norm)
+    im = ax[2].imshow(resid, origin='lower')
+    ax[0].set_title('Data')
+    ax[1].set_title('Model')
+    ax[2].set_title('Residual Image')
+    plt.tight_layout()
+
+The residual image looks like noise, indicating good fits to the
+sources.
+
+Further details about the PSF fitting can be obtained from attributes on
+the `~photutils.psf.PSFPhotometry` instance. For example, the results
+from the ``finder`` instance called during PSF fitting can be accessed
+using the ``finder_results`` attribute (the ``finder`` returns an
+astropy table):
 
-Fitting additional parameters
------------------------------
+.. doctest-requires:: scipy
+
+    >>> psfphot.finder_results[0]['xcentroid'].info.format = '.4f'  # optional format
+    >>> psfphot.finder_results[0]['ycentroid'].info.format = '.4f'  # optional format
+    >>> psfphot.finder_results[0]['sharpness'].info.format = '.4f'  # optional format
+    >>> psfphot.finder_results[0]['peak'].info.format = '.4f'
+    >>> psfphot.finder_results[0]['flux'].info.format = '.4f'
+    >>> psfphot.finder_results[0]['mag'].info.format = '.4f'
+    >>> print(psfphot.finder_results[0])  # doctest: +FLOAT_CMP
+     id xcentroid ycentroid sharpness ... sky   peak    flux    mag
+    --- --------- --------- --------- ... --- ------- ------- -------
+      1   32.7662   12.2009    0.6116 ... 0.0 68.3302  8.7599 -2.3562
+      2   13.2605   14.5831    0.5761 ... 0.0 52.5762  6.9429 -2.1039
+      3   63.6581   22.4396    0.5810 ... 0.0 63.7761  8.1125 -2.2729
+      4   82.2983   25.4851    0.5846 ... 0.0 66.2365  8.5570 -2.3308
+      5   41.5040   35.8841    0.5925 ... 0.0 71.3016  9.1493 -2.4035
+      6   21.5235   41.9433    0.6014 ... 0.0 64.8142  8.4183 -2.3131
+      7   14.1791   64.9962    0.6275 ... 0.0 78.2702 10.3522 -2.5376
+      8   61.8323   67.5194    0.5755 ... 0.0 62.9875  8.2963 -2.2972
+      9   74.6218   68.1660    0.6043 ... 0.0 53.9404  7.1150 -2.1304
+     10   15.1527   78.0361    0.6136 ... 0.0 62.7977  8.2524 -2.2915
+
+The ``fit_results`` attribute contains a dictionary with a wealth of
+detailed information, including the fit models and any information
+returned from the ``fitter`` for each source:
+
+.. doctest-requires:: scipy
 
-The PSF photometry classes can also be used to fit more model parameters
-than just the flux and center positions. While a more realistic use case
-might be fitting sky backgrounds, or shape parameters of galaxies, here
-we use the ``sigma`` parameter in `~photutils.psf.IntegratedGaussianPRF`
-as the simplest possible example of this feature. (For actual PSF
-photometry of stars you would *not* want to do this, because the shape
-of the PSF should be set by bright stars or an optical model and held
-fixed when fitting.)
+    >>> psfphot.fit_results.keys()
+    dict_keys(['local_bkg', 'fit_infos', 'fit_param_errs', 'fit_error_indices', 'npixfit', 'nmodels', 'psfcenter_indices', 'fit_residuals'])
 
-First, let us instantiate a PSF model object:
+As an example, let's print the covariance matrix of the fit parameters
+for the first source (note that not all astropy fitters will return a
+covariance matrix):
 
 .. doctest-skip::
 
-    >>> gaussian_prf = IntegratedGaussianPRF()
+    >>> psfphot.fit_results['fit_infos'][0]['param_cov']  # doctest: +FLOAT_CMP
+    array([[ 7.27034774e-01,  8.86845334e-04,  3.98593038e-03],
+           [ 8.86845334e-04,  2.92871525e-06, -6.36805464e-07],
+           [ 3.98593038e-03, -6.36805464e-07,  4.29520185e-05]])
 
-The attribute ``fixed`` for the ``sigma`` parameter is set to ``True``
-by default, i.e., ``sigma`` is not considered during the fitting
-process. Let's first change this behavior:
 
-.. doctest-skip::
+Fitting a single source
+^^^^^^^^^^^^^^^^^^^^^^^
+
+In some cases, one may want to fit only a single source (or few sources)
+in an image. We can do that by defining a table of the sources that
+we want to fit. For this example, let's fit the single star at ``(x,
+y) = (42, 36)``. We first define a table with this position and then
+pass that table into the ``init_params`` keyword when calling the PSF
+photometry class on the data:
 
-    >>> gaussian_prf.sigma.fixed = False
+.. doctest-requires:: scipy
 
-In addition, we need to indicate the initial guess which will be used in
-during the fitting process. By the default, the initial guess is taken
-as the default value of ``sigma``, but we can change that by doing:
+    >>> from astropy.table import QTable
+    >>> init_params = QTable()
+    >>> init_params['x'] = [42]
+    >>> init_params['y'] = [36]
+    >>> phot = psfphot(data, error=error, init_params=init_params)
+
+The PSF photometry class allows for flexible input column names
+using a heuristic to identify the x, y, and flux columns. See
+`~photutils.psf.PSFPhotometry` for more details.
 
-.. doctest-skip::
+The output table contains only the fit results for the input source:
 
-    >>> gaussian_prf.sigma.value = 2.05
+.. doctest-requires:: scipy
 
-Now, let's create a simulated image which has a brighter star
-and one overlapping fainter companion so that the detection
-algorithm won't be able to identify it, and hence we should use
-`~photutils.psf.IterativelySubtractedPSFPhotometry` to measure
-the fainter star as well. Also, note that both of the stars have
-``sigma=2.0``.
+    >>> phot['x_fit'].info.format = '.4f'  # optional format
+    >>> phot['y_fit'].info.format = '.4f'
+    >>> phot['flux_fit'].info.format = '.4f'
+    >>> print(phot[('id', 'x_fit', 'y_fit', 'flux_fit')])  # doctest: +FLOAT_CMP
+     id  x_fit   y_fit  flux_fit
+    --- ------- ------- --------
+      1 41.5416 35.8893 687.8236
+
+Finally, let's show the residual image. The red circular aperture shows
+the location of the star that was fit and subtracted.
 
 .. plot::
-    :include-source:
 
     import matplotlib.pyplot as plt
-    from astropy.table import Table
-    from astropy.visualization import simple_norm
-    from photutils.datasets import (make_gaussian_sources_image,
-                                    make_noise_image)
+    import numpy as np
+    from astropy.table import QTable
+    from photutils.aperture import CircularAperture
+    from photutils.datasets import make_noise_image, make_test_psf_data
+    from photutils.detection import DAOStarFinder
+    from photutils.psf import IntegratedGaussianPRF, PSFPhotometry
+
+    psf_model = IntegratedGaussianPRF(flux=1, sigma=2.7 / 2.35)
+    psf_shape = (25, 25)
+    nsources = 10
+    shape = (101, 101)
+    data, true_params = make_test_psf_data(shape, psf_model, psf_shape,
+                                           nsources, flux_range=(500, 700),
+                                           min_separation=10, seed=0)
+    noise = make_noise_image(data.shape, mean=0, stddev=1, seed=0)
+    data += noise
+    error = np.abs(noise)
+
+    psf_model = IntegratedGaussianPRF(flux=1, sigma=2.7 / 2.35)
+    fit_shape = (5, 5)
+    finder = DAOStarFinder(6.0, 2.0)
+    psfphot = PSFPhotometry(psf_model, fit_shape, finder=finder,
+                            aperture_radius=4)
+
+    init_params = QTable()
+    init_params['x'] = [42]
+    init_params['y'] = [36]
+    phot = psfphot(data, error=error, init_params=init_params)
+
+    resid = psfphot.make_residual_image(data, (25, 25))
+    plt.imshow(resid, origin='lower')
+
+    resid = psfphot.make_residual_image(data, (25, 25))
+    aper = CircularAperture(zip(init_params['x'], init_params['y']), r=4)
+    plt.imshow(resid, origin='lower')
+    aper.plot(color='red')
 
-    sources = Table()
-    sources['flux'] = [10000, 1000]
-    sources['x_mean'] = [18, 9]
-    sources['y_mean'] = [17, 21]
-    sources['x_stddev'] = [2] * 2
-    sources['y_stddev'] = sources['x_stddev']
-    sources['theta'] = [0] * 2
-    tshape = (32, 32)
-    image = (make_gaussian_sources_image(tshape, sources)
-             + make_noise_image(tshape, distribution='poisson', mean=6.0,
-                                seed=123)
-             + make_noise_image(tshape, distribution='gaussian', mean=0.0,
-                                stddev=2.0, seed=123))
-    norm = simple_norm(image, 'sqrt', percent=98.)
-    plt.imshow(image, interpolation='nearest', origin='lower', norm=norm)
-
-Let's instantiate the necessary objects in order to use an
-`~photutils.psf.IterativelySubtractedPSFPhotometry` to perform
-photometry:
+    plt.title('Residual Image')
+    plt.colorbar()
+
+
+Forced Photometry
+^^^^^^^^^^^^^^^^^
+
+In general, the three parameters fit for each source are the x and
+y positions and the flux. However, the astropy modeling and fitting
+framework allows any of these parameters to be fixed during the fitting.
+
+Let's say you want to fix the (x, y) position for each source. You can
+do that by setting the ``fixed`` attribute on the model parameters:
 
 .. doctest-requires:: scipy
 
-    >>> daogroup = DAOGroup(crit_separation=8)
-    >>> mmm_bkg = MMMBackground()
-    >>> iraffind = IRAFStarFinder(threshold=2.5 * mmm_bkg(image), fwhm=4.5)
-    >>> fitter = LevMarLSQFitter()
-    >>> gaussian_prf = IntegratedGaussianPRF(sigma=2.05)
-    >>> gaussian_prf.sigma.fixed = False
-    >>> itr_phot_obj = IterativelySubtractedPSFPhotometry(finder=iraffind,
-    ...                                                   group_maker=daogroup,
-    ...                                                   bkg_estimator=mmm_bkg,
-    ...                                                   psf_model=gaussian_prf,
-    ...                                                   fitter=fitter,
-    ...                                                   fitshape=(11, 11),
-    ...                                                   niters=2)
-
-Now, let's use the callable ``itr_phot_obj`` to perform photometry:
+    >>> psf_model2 = IntegratedGaussianPRF(flux=1, sigma=2.7 / 2.35)
+    >>> psf_model2.x_0.fixed = True
+    >>> psf_model2.y_0.fixed = True
+    >>> psf_model2.fixed
+    {'flux': False, 'x_0': True, 'y_0': True, 'sigma': True}
+
+Now when the model is fit, the flux will be varied but, the (x, y)
+position will be fixed at its initial position for every source. Let's
+just fit a single source (defined in ``init_params``):
 
 .. doctest-requires:: scipy
 
-    >>> phot_results = itr_phot_obj(image)
-    >>> phot_results['id', 'group_id', 'iter_detected', 'x_0', 'y_0', 'flux_0']  #doctest: +SKIP
-         id group_id iter_detected      x_0           y_0          flux_0
-        --- -------- ------------- ------------- ------------- -------------
-          1        1             1 18.0045935148 17.0060558543 9437.07321281
-          1        1             2 9.06141447183 21.0680052846 977.163727416
-    >>> phot_results['sigma_0', 'sigma_fit', 'x_fit', 'y_fit', 'flux_fit']  #doctest: +SKIP
-        sigma_0   sigma_fit       x_fit         y_fit        flux_fit
-        ------- ------------- ------------- ------------- -------------
-           2.05 1.98092026939 17.9995106906 17.0039419384 10016.4470148
-           2.05 1.98516037471 9.12116345703 21.0599164498 1036.79115883
+    >>> psfphot = PSFPhotometry(psf_model2, fit_shape, finder=finder,
+    ...                         aperture_radius=4)
+    >>> phot = psfphot(data, error=error, init_params=init_params)
+
+The output table shows that the (x, y) position was unchanged, with the
+fit values being identical to the initial values. However, the flux was
+fit:
+
+.. doctest-requires:: scipy
+
+    >>> phot['flux_init'].info.format = '.4f'  # optional format
+    >>> phot['flux_fit'].info.format = '.4f'
+    >>> print(phot[('id', 'x_init', 'y_init', 'flux_init', 'x_fit',
+    ...             'y_fit', 'flux_fit')])  # doctest: +FLOAT_CMP
+     id x_init y_init flux_init x_fit y_fit flux_fit
+    --- ------ ------ --------- ----- ----- --------
+      1     42     36  701.6391  42.0  36.0 921.2168
+
+
+Source Grouping
+^^^^^^^^^^^^^^^
+
+Source grouping is an optional feature. To turn it on, create a
+`~photutils.psf.SourceGrouper` instance and input it via the ``grouper``
+keyword. Here we'll group stars that are within 20 pixels of each
+other:
+
+.. doctest-requires:: scipy, sklearn
+
+    >>> from photutils.psf import SourceGrouper
+    >>> grouper = SourceGrouper(min_separation=20)
+    >>> psfphot = PSFPhotometry(psf_model, fit_shape, finder=finder,
+    ...                         grouper=grouper, aperture_radius=4)
+    >>> phot = psfphot(data, error=error)
+
+The ``group_id`` column shows that six groups were identified (each with
+two stars). The stars in each group were simultaneously fit.
+
+.. doctest-requires:: scipy, sklearn
+
+    >>> print(phot[('id', 'group_id', 'group_size')])
+     id group_id group_size
+    --- -------- ----------
+      1        1          2
+      2        1          2
+      3        2          2
+      4        2          2
+      5        3          1
+      6        4          1
+      7        5          2
+      8        6          2
+      9        6          2
+     10        5          2
+
+Care should be taken in defining the star groups. As noted above,
+simultaneously fitting very large star groups is computationally
+expensive and error-prone. A warning will be raised if the number of
+sources in a group exceeds 25.
+
+
+Local Background Subtraction
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+To subtract a local background from each source, define a
+`~photutils.background.LocalBackground` instance and input it via
+the ``localbkg_estimator`` keyword. Here we'll use an annulus with
+an inner and outer radius of 5 and 10 pixels, respectively, with the
+`~photutils.background.MMMBackground` statistic (with its default sigma
+clipping):
+
+.. doctest-requires:: scipy, sklearn
+
+    >>> from photutils.background import LocalBackground, MMMBackground
+    >>> bkgstat = MMMBackground()
+    >>> localbkg_estimator = LocalBackground(5, 10, bkgstat)
+    >>> finder = DAOStarFinder(10.0, 2.0)
+    >>> psfphot = PSFPhotometry(psf_model, fit_shape, finder=finder,
+    ...                         grouper=grouper, aperture_radius=4,
+    ...                         localbkg_estimator=localbkg_estimator)
+    >>> phot = psfphot(data, error=error)
+
+The local background values are output in the table:
+
+.. doctest-requires:: scipy, sklearn
+
+    >>> phot['local_bkg'].info.format = '.4f'  # optional format
+    >>> print(phot[('id', 'local_bkg')])  # doctest: +FLOAT_CMP
+     id local_bkg
+    --- ---------
+      1    0.2869
+      2    0.0207
+      3   -0.1331
+      4    0.2441
+      5   -0.0371
+      6   -0.2863
+      7   -0.1639
+      8    0.0544
+      9   -0.1431
+     10   -0.0414
+
+The local background values can also be input directly using the
+``init_params`` keyword.
+
+
+Iterative PSF Photometry
+^^^^^^^^^^^^^^^^^^^^^^^^
+
+Now let's use the `~photutils.psf.IterativePSFPhotometry` class to
+iteratively fit the stars in the image. This class is useful for crowded
+fields where faint stars are very close to bright stars. The faint stars
+may not be detected until after the bright stars are subtracted.
+
+For this simple example, let's input a table of three stars for the
+first fit iteration. Subsequent iterations will use the ``finder`` to
+find additional stars:
+
+.. doctest-requires:: scipy
+
+    >>> from photutils.background import LocalBackground, MMMBackground
+    >>> from photutils.psf import IterativePSFPhotometry
+    >>> fit_shape = (5, 5)
+    >>> finder = DAOStarFinder(10.0, 2.0)
+    >>> bkgstat = MMMBackground()
+    >>> localbkg_estimator = LocalBackground(5, 10, bkgstat)
+    >>> init_params = QTable()
+    >>> init_params['x'] = [33, 13, 64]
+    >>> init_params['y'] = [12, 15, 22]
+    >>> psfphot2 = IterativePSFPhotometry(psf_model, fit_shape, finder=finder,
+    ...                                   localbkg_estimator=localbkg_estimator,
+    ...                                   aperture_radius=4)
+    >>> phot = psfphot2(data, error=error, init_params=init_params)
+
+The table output from `~photutils.psf.IterativePSFPhotometry` contains a
+column called ``iter_detected`` that returns the fit iteration in which
+the source was detected:
+
+.. doctest-requires:: scipy
 
-We can see that ``sigma_0`` (the initial guess for ``sigma``) was
-assigned to the value we used when creating the PSF model.
+    >>> phot['x_fit'].info.format = '.4f'  # optional format
+    >>> phot['y_fit'].info.format = '.4f'
+    >>> phot['flux_fit'].info.format = '.4f'
+    >>> print(phot[('id', 'iter_detected', 'x_fit', 'y_fit', 'flux_fit')])  # doctest: +FLOAT_CMP
+     id iter_detected  x_fit   y_fit  flux_fit
+    --- ------------- ------- ------- --------
+      1             1 32.7697 12.2179 623.1128
+      2             1 13.2674 14.5843 505.6723
+      3             1 63.6500 22.3870 644.4719
+      4             2 82.2881 25.5224 658.0372
+      5             2 41.5420 35.8889 688.7885
+      6             2 21.5767 41.9471 625.1697
+      7             2 14.1820 65.0087 683.7103
+      8             2 61.8352 67.5545 607.3983
+      9             2 74.6200 68.1865 506.1033
+     10             2 15.1675 78.0376 558.5847
 
 
 References
 ----------
 
 `Spitzer PSF vs. PRF
 <https://irsa.ipac.caltech.edu/data/SPITZER/docs/files/spitzer/PRF_vs_PSF.pdf>`_
 
 `The Kepler Pixel Response Function
 <https://ui.adsabs.harvard.edu/abs/2010ApJ...713L..97B/abstract>`_
 
-`Stetson, Astronomical Society of the Pacific, Publications, (ISSN
-0004-6280), vol. 99, March 1987, p. 191-222.
+`Stetson (1987 PASP 99, 191)
 <https://ui.adsabs.harvard.edu/abs/1987PASP...99..191S/abstract>`_
 
-`Anderson & King, Astronomical Society of the Pacific, Publications,
-Volume 112, Issue 776, pp. 1360-1382, Nov 2000
+`Anderson and King (2000 PASP 112, 1360)
 <https://ui.adsabs.harvard.edu/abs/2000PASP..112.1360A/abstract>`_
 
 
 Reference/API
 -------------
 
 .. automodapi:: photutils.psf
```

### Comparing `photutils-1.8.0/docs/psf_matching.rst` & `photutils-1.9.0/docs/psf_matching.rst`

 * *Files 1% similar despite different names*

```diff
@@ -58,23 +58,22 @@
     g1 /= g1.sum()
     g2 /= g2.sum()
 
     kernel = create_matching_kernel(g1, g2)
     plt.imshow(kernel, cmap='Greys_r', origin='lower')
     plt.colorbar()
 
-We quickly observe that the result is not as expected.  This is
-because of high-frequency noise in the Fourier transforms (even though
-these are noiseless PSFs, there is floating-point noise in the
-ratios).  Using the Fourier ratio method, one must filter the
-high-frequency noise from the Fourier ratios.  This is performed by
-inputing a `window function
-<https://en.wikipedia.org/wiki/Window_function>`_, which may be a
-function or a callable object.  In general, the user will need to
-exercise some care when defining a window function.  For more
+We quickly observe that the result is not as expected. This is because
+of high-frequency noise in the Fourier transforms (even though these
+are noiseless PSFs, there is floating-point noise in the ratios). Using
+the Fourier ratio method, one must filter the high-frequency noise
+from the Fourier ratios. This is performed by inputting a `window
+function <https://en.wikipedia.org/wiki/Window_function>`_, which
+may be a function or a callable object. In general, the user will
+need to exercise some care when defining a window function. For more
 information, please see `Aniano et al. 2011`_.
 
 Photutils provides the following window classes:
 
 * `~photutils.psf.matching.HanningWindow`
 * `~photutils.psf.matching.TukeyWindow`
 * `~photutils.psf.matching.CosineBellWindow`
@@ -279,15 +278,15 @@
 
     plt.imshow(kernel, norm=norm, cmap='viridis', origin='lower')
     plt.colorbar()
     plt.title('Matching kernel')
 
 The Spitzer/IRAC channel 1 image could then be convolved with this
 matching kernel to produce an image with the same resolution as the
-channel 4 image.
+channel-4 image.
 
 
 Reference/API
 -------------
 
 .. automodapi:: photutils.psf.matching
     :no-heading:
```

### Comparing `photutils-1.8.0/docs/psf_spec/background_estimator.rst` & `photutils-1.9.0/docs/psf_spec/background_estimator.rst`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 This block requires no methods beyond ``__call__()``.
 
 
 Example Usage
 -------------
 
 A variety of implementations of this block already exist in ``photutils``. A
-canononical example is the mode estimation algorithm ``3 * median - 2 * mean``.
+canonical example is the mode estimation algorithm ``3 * median - 2 * mean``.
 This can be done on an array called  ``image_data`` by using the block like so::
 
     from photutils.background import ModeEstimatorBackground
     bkg_estimator = ModeEstimatorBackground()
     bkg_value = bkg_estimator(image_data)
 
 The median/mean parameter values can be adjusted as keyword arguments to the
```

### Comparing `photutils-1.8.0/docs/psf_spec/block_diagram.png` & `photutils-1.9.0/docs/psf_spec/block_diagram.png`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/docs/psf_spec/block_template.rst` & `photutils-1.9.0/docs/psf_spec/block_template.rst`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/docs/psf_spec/culler_and_ender.rst` & `photutils-1.9.0/docs/psf_spec/culler_and_ender.rst`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/docs/psf_spec/finder.rst` & `photutils-1.9.0/docs/psf_spec/finder.rst`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/docs/psf_spec/group_maker.rst` & `photutils-1.9.0/docs/psf_spec/group_maker.rst`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/docs/psf_spec/noise_data.rst` & `photutils-1.9.0/docs/psf_spec/noise_data.rst`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/docs/psf_spec/psf_model.rst` & `photutils-1.9.0/docs/psf_spec/psf_model.rst`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/docs/psf_spec/scene_maker.rst` & `photutils-1.9.0/docs/psf_spec/scene_maker.rst`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/docs/psf_spec/single_object_model.rst` & `photutils-1.9.0/docs/psf_spec/single_object_model.rst`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/docs/segmentation.rst` & `photutils-1.9.0/docs/segmentation.rst`

 * *Files 0% similar despite different names*

```diff
@@ -324,15 +324,15 @@
     Length: 94
     labels: [ 1  2  3  4  5 ... 90 91 92 93 94]
 
 The source properties can be accessed using
 `~photutils.segmentation.SourceCatalog` attributes or
 output to an Astropy `~astropy.table.QTable` using the
 :meth:`~photutils.segmentation.SourceCatalog.to_table` method. Please
-see :class:`~photutils.segmentation.SourceCatalog` for the the many
+see :class:`~photutils.segmentation.SourceCatalog` for the many
 properties that can be calculated for each source. More properties are
 likely to be added in the future.
 
 Here we'll use the
 :meth:`~photutils.segmentation.SourceCatalog.to_table` method to
 generate a `~astropy.table.QTable` of source properties. Each row in the
 table represents a source. The columns represent the calculated source
```

### Comparing `photutils-1.8.0/docs/whats_new/1.1.rst` & `photutils-1.9.0/docs/whats_new/1.1.rst`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     * 'maxval_xpos' -> 'maxval_xindex'
     * 'maxval_ypos' -> 'maxval_yindex'
     * 'semimajor_axis_sigma' -> 'semimajor_sigma'
     * 'semiminor_axis_sigma' -> 'semiminor_sigma'
     * 'source_sum' -> 'segment_flux'
     * 'source_sum_err' -> 'segment_fluxerr'
 
-Also the 'centroid' and 'cutout_centroid' properties now return
+Also, the 'centroid' and 'cutout_centroid' properties now return
 centroids in (x, y) order to be consistent with the tools in
 ``photutils.centroid``.
 
 New methods and attributes
 --------------------------
 The new `~photutils.segmentation.SourceCatalog` class has the following
 new methods:
```

### Comparing `photutils-1.8.0/docs/whats_new/1.4.rst` & `photutils-1.9.0/docs/whats_new/1.4.rst`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/docs/whats_new/1.5.rst` & `photutils-1.9.0/docs/whats_new/1.5.rst`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/docs/whats_new/1.6.rst` & `photutils-1.9.0/docs/whats_new/1.6.rst`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/docs/whats_new/1.7.rst` & `photutils-1.9.0/docs/whats_new/1.7.rst`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/docs/whats_new/1.8.rst` & `photutils-1.9.0/docs/whats_new/1.8.rst`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/CITATION.rst` & `photutils-1.9.0/photutils/CITATION.rst`

 * *Files 13% similar despite different names*

```diff
@@ -5,43 +5,43 @@
 whether directly or as a dependency of another package, please include
 the following acknowledgment:
 
 .. code-block:: text
 
     This research made use of Photutils, an Astropy package for
     detection and photometry of astronomical sources (Bradley et al.
-    20XX).
+    <YEAR>).
 
-where (Bradley et al. 20XX) is a citation to the `Zenodo record
+where (Bradley et al. <YEAR>) is a citation to the `Zenodo record
 <https://doi.org/10.5281/zenodo.596036>`_ of the Photutils version
 that was used. We also encourage citations in the main text wherever
 appropriate.
 
-All Photutils versions and citation formats can be found at
+BibTex files for all Photutils versions can be found at
 https://doi.org/10.5281/zenodo.596036. For example, for Photutils
-v1.5.0 one would cite Bradley et al. 2022 with the BibTeX entry
-(https://zenodo.org/record/6825092/export/hx):
+v1.8.0 one should cite Bradley et al. 2023 with the BibTeX entry
+(https://zenodo.org/record/7946442/export/hx):
 
 .. code-block:: text
 
-    @software{larry_bradley_2022_6825092,
+    @software{larry_bradley_2023_7946442,
     author       = {Larry Bradley and
-                    Brigitta Sipőcz and
+                    Brigitta Sip{\H o}cz and
                     Thomas Robitaille and
                     Erik Tollerud and
-                    Zé Vinícius and
+                    Z\`e Vin{\'{\i}}cius and
                     Christoph Deil and
                     Kyle Barbary and
                     Tom J Wilson and
                     Ivo Busko and
                     Axel Donath and
-                    Hans Moritz Günther and
+                    Hans Moritz G{\"u}nther and
                     Mihai Cara and
                     P. L. Lim and
-                    Sebastian Meßlinger and
+                    Sebastian Me{\ss}linger and
                     Simon Conseil and
                     Azalee Bostroem and
                     Michael Droettboom and
                     E. M. Bray and
                     Lars Andersen Bratholm and
                     Geert Barentsen and
                     Matt Craig and
@@ -50,15 +50,15 @@
                     Gabriel Perren and
                     Iskren Y. Georgiev and
                     Miguel de Val-Borro and
                     Wolfgang Kerzendorf and
                     Yoonsoo P. Bach and
                     Bruno Quint and
                     Harrison Souchereau},
-    title        = {astropy/photutils: 1.5.0},
-    month        = jul,
-    year         = 2022,
+    title        = {astropy/photutils: 1.8.0},
+    month        = may,
+    year         = 2023,
     publisher    = {Zenodo},
-    version      = {1.5.0},
-    doi          = {10.5281/zenodo.6825092},
-    url          = {https://doi.org/10.5281/zenodo.6825092}
+    version      = {1.8.0},
+    doi          = {10.5281/zenodo.7946442},
+    url          = {https://doi.org/10.5281/zenodo.7946442}
     }
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `photutils-1.8.0/photutils/__init__.py` & `photutils-1.9.0/photutils/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,16 +75,15 @@
 
 
 def __getattr__(attr):
     if attr in __depr_attrs__:
         obj, message = __depr_attrs__[attr]
         warnings.warn(message, DeprecationWarning, stacklevel=2)
         return obj
-    raise AttributeError('module {!r} has no attribute {!r}'
-                         .format(__name__, attr))
+    raise AttributeError(f'module {__name__!r} has no attribute {attr!r}')
 
 
 # Set the bibtex entry to the article referenced in CITATION.rst.
 def _get_bibtex():
     import os
     citation_file = os.path.join(os.path.dirname(__file__), 'CITATION.rst')
```

### Comparing `photutils-1.8.0/photutils/_compiler.c` & `photutils-1.9.0/photutils/_compiler.c`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/aperture/attributes.py` & `photutils-1.9.0/photutils/aperture/attributes.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,18 +88,18 @@
             raise TypeError(f'{self.name!r} must not be a Quantity')
 
         if np.any(~np.isfinite(value)):
             raise ValueError(f'{self.name!r} must not contain any non-finite '
                              '(e.g., NaN or inf) positions')
 
         value = np.atleast_2d(value)
-        if value.ndim > 2 and value.shape[1] != 2:
-            raise TypeError(f'{self.name!r} must be a (x, y) pixel position '
-                            'or a list or array of (x, y) pixel positions, '
-                            'e.g., [(x1, y1), (x2, y2), (x3, y3)]')
+        if value.ndim > 2 or value.shape[1] != 2:
+            raise ValueError(f'{self.name!r} must be a (x, y) pixel position '
+                             'or a list or array of (x, y) pixel positions, '
+                             'e.g., [(x1, y1), (x2, y2), (x3, y3)]')
 
 
 class SkyCoordPositions(ApertureAttribute):
     """
     Check that value is a `~astropy.coordinates.SkyCoord`.
     """
 
@@ -129,15 +129,15 @@
         if isinstance(value, u.Quantity):
             if not value.isscalar:
                 raise ValueError(f'{self.name!r} must be a scalar')
 
             if not value.unit.physical_type == 'angle':
                 raise ValueError(f'{self.name!r} must have angular units')
         else:
-            raise TypeError(f'{self.name!r} must be a scalar angle')
+            raise ValueError(f'{self.name!r} must be a scalar angle')
 
 
 class PositiveScalarAngle(ApertureAttribute):
     """
     Check that value is a positive scalar angle, either as a
     `~astropy.coordinates.Angle` or `~astropy.units.Quantity` with
     angular units.
@@ -150,15 +150,15 @@
         if isinstance(value, u.Quantity):
             if not value.isscalar:
                 raise ValueError(f'{self.name!r} must be a scalar')
 
             if not value.unit.physical_type == 'angle':
                 raise ValueError(f'{self.name!r} must have angular units')
         else:
-            raise TypeError(f'{self.name!r} must be a scalar angle')
+            raise ValueError(f'{self.name!r} must be a scalar angle')
 
 
 class ScalarAngleOrValue(ApertureAttribute):
     """
     Check that value is a scalar angle, either as a
     `~astropy.coordinates.Angle` or `~astropy.units.Quantity` with
     angular units, or a scalar float.
@@ -182,9 +182,9 @@
             if not value.isscalar:
                 raise ValueError(f'{self.name!r} must be a scalar')
 
             if not value.unit.physical_type == 'angle':
                 raise ValueError(f'{self.name!r} must have angular units')
         else:
             if not np.isscalar(value):
-                raise TypeError(f'If not an angle Quantity, {self.name!r} '
-                                'must be a scalar float in radians')
+                raise ValueError(f'If not an angle Quantity, {self.name!r} '
+                                 'must be a scalar float in radians')
```

### Comparing `photutils-1.8.0/photutils/aperture/bounding_box.py` & `photutils-1.9.0/photutils/aperture/bounding_box.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/aperture/circle.py` & `photutils-1.9.0/photutils/aperture/circle.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/aperture/core.py` & `photutils-1.9.0/photutils/aperture/core.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/aperture/ellipse.py` & `photutils-1.9.0/photutils/aperture/ellipse.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/aperture/mask.py` & `photutils-1.9.0/photutils/aperture/mask.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/aperture/photometry.py` & `photutils-1.9.0/photutils/aperture/photometry.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/aperture/rectangle.py` & `photutils-1.9.0/photutils/aperture/rectangle.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/aperture/stats.py` & `photutils-1.9.0/photutils/aperture/stats.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/aperture/tests/test_aperture_common.py` & `photutils-1.9.0/photutils/aperture/tests/test_aperture_common.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/aperture/tests/test_bounding_box.py` & `photutils-1.9.0/photutils/aperture/tests/test_bounding_box.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/aperture/tests/test_circle.py` & `photutils-1.9.0/photutils/aperture/tests/test_circle.py`

 * *Files 6% similar despite different names*

```diff
@@ -171,7 +171,24 @@
     areas = aper.area_overlap(data, mask=mask)
     areas_exp = np.array([10.304636, np.pi * 9.0, np.nan]) - 2.0
     assert_allclose(areas, areas_exp)
 
     with pytest.raises(ValueError):
         mask = np.zeros((3, 3), dtype=bool)
         aper.area_overlap(data, mask=mask)
+
+
+def test_invalid_positions():
+    with pytest.raises(ValueError):
+        _ = CircularAperture([], r=3)
+
+    with pytest.raises(ValueError):
+        _ = CircularAperture([1], r=3)
+
+    with pytest.raises(ValueError):
+        _ = CircularAperture([[1]], r=3)
+
+    with pytest.raises(ValueError):
+        _ = CircularAperture([1, 2, 3], r=3)
+
+    with pytest.raises(ValueError):
+        _ = CircularAperture([[1, 2, 3]], r=3)
```

### Comparing `photutils-1.8.0/photutils/aperture/tests/test_ellipse.py` & `photutils-1.9.0/photutils/aperture/tests/test_ellipse.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/aperture/tests/test_mask.py` & `photutils-1.9.0/photutils/aperture/tests/test_mask.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/aperture/tests/test_photometry.py` & `photutils-1.9.0/photutils/aperture/tests/test_photometry.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/aperture/tests/test_rectangle.py` & `photutils-1.9.0/photutils/aperture/tests/test_rectangle.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/aperture/tests/test_stats.py` & `photutils-1.9.0/photutils/aperture/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/background/background_2d.py` & `photutils-1.9.0/photutils/background/background_2d.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/background/core.py` & `photutils-1.9.0/photutils/background/core.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/background/interpolators.py` & `photutils-1.9.0/photutils/background/interpolators.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/background/tests/test_background_2d.py` & `photutils-1.9.0/photutils/background/tests/test_background_2d.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/background/tests/test_core.py` & `photutils-1.9.0/photutils/background/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/centroids/core.py` & `photutils-1.9.0/photutils/centroids/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import warnings
 
 import numpy as np
 from astropy.nddata.utils import overlap_slices
 from astropy.utils.exceptions import AstropyUserWarning
 
 from photutils.utils._parameters import as_pair
-from photutils.utils._round import _py2intround
+from photutils.utils._round import py2intround
 
 __all__ = ['centroid_com', 'centroid_quadratic', 'centroid_sources']
 
 
 def centroid_com(data, mask=None):
     """
     Calculate the centroid of an n-dimensional array as its "center of
@@ -185,16 +185,16 @@
     if np.prod(fit_boxsize) < 6:
         raise ValueError('fit_boxsize is too small.  6 values are required '
                          'to fit a 2D quadratic polynomial.')
 
     if xpeak is None or ypeak is None:
         yidx, xidx = np.unravel_index(np.nanargmax(data), data.shape)
     else:
-        xidx = _py2intround(xpeak)
-        yidx = _py2intround(ypeak)
+        xidx = py2intround(xpeak)
+        yidx = py2intround(ypeak)
 
         if search_boxsize is not None:
             search_boxsize = as_pair('search_boxsize', search_boxsize,
                                      lower_bound=(0, 1),
                                      upper_bound=data.shape, check_odd=True)
 
             slc_data, _ = overlap_slices(data.shape, search_boxsize,
```

### Comparing `photutils-1.8.0/photutils/centroids/gaussian.py` & `photutils-1.9.0/photutils/centroids/gaussian.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/centroids/tests/test_core.py` & `photutils-1.9.0/photutils/centroids/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/centroids/tests/test_gaussian.py` & `photutils-1.9.0/photutils/centroids/tests/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/conftest.py` & `photutils-1.9.0/photutils/conftest.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/datasets/load.py` & `photutils-1.9.0/photutils/datasets/load.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/datasets/make.py` & `photutils-1.9.0/photutils/datasets/make.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 # Licensed under a 3-clause BSD style license - see LICENSE.rst
 """
 This module provides tools for making example datasets for examples and
 tests.
 """
 
+import warnings
+
 import astropy.units as u
 import numpy as np
 from astropy import coordinates as coord
 from astropy.convolution import discretize_model
 from astropy.io import fits
 from astropy.modeling import models
+from astropy.nddata import overlap_slices
 from astropy.table import QTable
+from astropy.utils.exceptions import AstropyUserWarning
 from astropy.wcs import WCS
 
 from photutils.psf import IntegratedGaussianPRF
 from photutils.utils._misc import _get_version_info
+from photutils.utils._progress_bars import add_progress_bar
 
 __all__ = ['apply_poisson_noise', 'make_noise_image',
            'make_random_models_table', 'make_random_gaussians_table',
            'make_model_sources_image', 'make_gaussian_sources_image',
            'make_4gaussians_image', 'make_100gaussians_image',
            'make_wcs', 'make_gwcs', 'make_imagehdu',
-           'make_gaussian_prf_sources_image']
+           'make_gaussian_prf_sources_image',
+           'make_test_psf_data']
 
 __doctest_requires__ = {('make_gwcs'): ['gwcs']}
 
 
 def apply_poisson_noise(data, seed=None):
     """
     Apply Poisson noise to an array, where the value of each element in
@@ -938,7 +944,132 @@
 
     if wcs is not None:
         header = wcs.to_header()
     else:
         header = None
 
     return fits.ImageHDU(data, header=header)
+
+
+def _make_nonoverlap_coords(xrange, yrange, ncoords, min_separation, seed=0):
+    from scipy.spatial import KDTree
+
+    rng = np.random.default_rng(seed)
+
+    xycoords = np.zeros((0, 2))
+    niter = 1
+
+    while xycoords.shape[0] < ncoords:
+        if niter > 20:
+            break
+
+        x_new = rng.uniform(xrange[0], xrange[1], ncoords)
+        y_new = rng.uniform(yrange[0], yrange[1], ncoords)
+        new_xycoords = np.transpose((x_new, y_new))
+        if niter == 1:
+            xycoords = new_xycoords
+        else:
+            xycoords = np.vstack((xycoords, new_xycoords))
+
+        dist, _ = KDTree(xycoords).query(xycoords, k=[2])
+        mask = (dist >= min_separation).squeeze()
+        xycoords = xycoords[mask]
+        niter += 1
+
+    xycoords = xycoords[0:ncoords]
+    if len(xycoords) < ncoords:
+        warnings.warn(f'Unable to produce {ncoords!r} coordinates.',
+                      AstropyUserWarning)
+
+    return xycoords
+
+
+def make_test_psf_data(shape, psf_model, psf_shape, nsources,
+                       flux_range=(100, 1000), min_separation=1, seed=0,
+                       progress_bar=False):
+    """
+    Make an example image containing PSF model images.
+
+    Source positions and fluxes are randomly generated using an optional
+    ``seed``.
+
+    Parameters
+    ----------
+    shape : 2-tuple of int
+        The shape of the output image.
+
+    psf_model : `astropy.modeling.Fittable2DModel`
+        The PSF model.
+
+    psf_shape : 2-tuple of int
+        The shape around the center of the star that will used to
+        evaluate the ``psf_model``.
+
+    nsources : int
+        The number of sources to generate.
+
+    flux_range : tuple, optional
+        The lower and upper bounds of the flux range.
+
+    min_separation : float, optional
+        The minimum separation between the centers of two sources. Note
+        that if the minimum separation is too large, the number of
+        sources generated may be less than ``nsources``.
+
+    seed : int, optional
+        A seed to initialize the `numpy.random.BitGenerator`. If `None`,
+        then fresh, unpredictable entropy will be pulled from the OS.
+
+    progress_bar : bool, optional
+        Whether to display a progress bar when creating the sources. The
+        progress bar requires that the `tqdm <https://tqdm.github.io/>`_
+        optional dependency be installed. Note that the progress
+        bar does not currently work in the Jupyter console due to
+        limitations in ``tqdm``.
+
+    Returns
+    -------
+    data : 2D `~numpy.ndarray`
+        The simulated image.
+
+    table : `~astropy.table.Table`
+        A table containing the parameters of the generated sources.
+    """
+    hshape = (np.array(psf_shape) - 1) // 2
+    xrange = (hshape[1], shape[1] - hshape[1])
+    yrange = (hshape[0], shape[0] - hshape[0])
+
+    xycoords = _make_nonoverlap_coords(xrange, yrange, nsources,
+                                       min_separation=min_separation,
+                                       seed=seed)
+    x, y = np.transpose(xycoords)
+
+    rng = np.random.default_rng(seed)
+    flux = rng.uniform(flux_range[0], flux_range[1], nsources)
+    flux = flux[:len(x)]
+
+    sources = QTable()
+    sources['x_0'] = x
+    sources['y_0'] = y
+    sources['flux'] = flux
+
+    data = np.zeros(shape, dtype=float)
+
+    sources_iter = sources
+    if progress_bar:  # pragma: no cover
+        desc = 'Adding sources'
+        sources_iter = add_progress_bar(sources, desc=desc)
+
+    for source in sources_iter:
+        for param in ('x_0', 'y_0', 'flux'):
+            setattr(psf_model, param, source[param])
+        xcen = source['x_0']
+        ycen = source['y_0']
+        slc_lg, _ = overlap_slices(shape, psf_shape, (ycen, xcen), mode='trim')
+        yy, xx = np.mgrid[slc_lg]
+        data[slc_lg] += psf_model(xx, yy)
+
+    sources.rename_column('x_0', 'x')
+    sources.rename_column('y_0', 'y')
+    sources.rename_column('flux', 'flux')
+
+    return data, sources
```

### Comparing `photutils-1.8.0/photutils/datasets/tests/test_make.py` & `photutils-1.9.0/photutils/datasets/tests/test_make.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,23 +3,26 @@
 Tests for the make module.
 """
 
 import numpy as np
 import pytest
 from astropy.modeling.models import Moffat2D
 from astropy.table import Table
+from astropy.utils.exceptions import AstropyUserWarning
 from numpy.testing import assert_allclose
 
 from photutils.datasets import (apply_poisson_noise, make_4gaussians_image,
                                 make_100gaussians_image,
                                 make_gaussian_prf_sources_image,
                                 make_gaussian_sources_image, make_gwcs,
                                 make_model_sources_image, make_noise_image,
                                 make_random_gaussians_table,
-                                make_random_models_table, make_wcs)
+                                make_random_models_table, make_test_psf_data,
+                                make_wcs)
+from photutils.psf import IntegratedGaussianPRF
 from photutils.utils._optional_deps import HAS_GWCS, HAS_SCIPY
 
 SOURCE_TABLE = Table()
 SOURCE_TABLE['flux'] = [1, 2, 3]
 SOURCE_TABLE['x_mean'] = [30, 50, 70.5]
 SOURCE_TABLE['y_mean'] = [50, 50, 50.5]
 SOURCE_TABLE['x_stddev'] = [1, 2, 3.5]
@@ -199,7 +202,31 @@
     wcs = make_wcs(shape)
     gwcs_obj = make_gwcs(shape)
     sc1 = wcs.pixel_to_world((50, 75), (50, 100))
     sc2 = gwcs_obj.pixel_to_world((50, 75), (50, 100))
 
     assert_allclose(sc1.ra, sc2.ra)
     assert_allclose(sc1.dec, sc2.dec)
+
+
+@pytest.mark.skipif(not HAS_SCIPY, reason='scipy is required')
+def test_make_test_psf_data():
+    psf_model = IntegratedGaussianPRF(flux=100, sigma=1.5)
+    psf_shape = (5, 5)
+    nsources = 10
+    shape = (100, 100)
+    data, true_params = make_test_psf_data(shape, psf_model, psf_shape,
+                                           nsources, flux_range=(500, 1000),
+                                           min_separation=10, seed=0)
+
+    assert isinstance(data, np.ndarray)
+    assert data.shape == shape
+    assert isinstance(true_params, Table)
+    assert len(true_params) == nsources
+    assert true_params['x'].min() >= 0
+    assert true_params['y'].min() >= 0
+
+    match = 'Unable to produce'
+    with pytest.warns(AstropyUserWarning, match=match):
+        nsources = 100
+        make_test_psf_data(shape, psf_model, psf_shape, nsources,
+                           flux_range=(500, 1000), min_separation=10, seed=0)
```

### Comparing `photutils-1.8.0/photutils/detection/core.py` & `photutils-1.9.0/photutils/detection/core.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/detection/daofinder.py` & `photutils-1.9.0/photutils/detection/daofinder.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/detection/irafstarfinder.py` & `photutils-1.9.0/photutils/detection/irafstarfinder.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/detection/peakfinder.py` & `photutils-1.9.0/photutils/detection/peakfinder.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/detection/starfinder.py` & `photutils-1.9.0/photutils/detection/starfinder.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/detection/tests/data/daofind_test_thresh08.0_fwhm01.0.txt` & `photutils-1.9.0/photutils/detection/tests/data/daofind_test_thresh08.0_fwhm01.0.txt`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/detection/tests/data/daofind_test_thresh08.0_fwhm01.5.txt` & `photutils-1.9.0/photutils/detection/tests/data/daofind_test_thresh08.0_fwhm01.5.txt`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/detection/tests/data/daofind_test_thresh08.0_fwhm02.0.txt` & `photutils-1.9.0/photutils/detection/tests/data/daofind_test_thresh08.0_fwhm02.0.txt`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/detection/tests/data/daofind_test_thresh10.0_fwhm01.0.txt` & `photutils-1.9.0/photutils/detection/tests/data/daofind_test_thresh10.0_fwhm01.0.txt`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/detection/tests/data/daofind_test_thresh10.0_fwhm01.5.txt` & `photutils-1.9.0/photutils/detection/tests/data/daofind_test_thresh10.0_fwhm01.5.txt`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/detection/tests/data/daofind_test_thresh10.0_fwhm02.0.txt` & `photutils-1.9.0/photutils/detection/tests/data/daofind_test_thresh10.0_fwhm02.0.txt`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/detection/tests/data/irafstarfind_test_thresh08.0_fwhm01.0.txt` & `photutils-1.9.0/photutils/detection/tests/data/irafstarfind_test_thresh08.0_fwhm01.0.txt`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/detection/tests/data/irafstarfind_test_thresh08.0_fwhm01.5.txt` & `photutils-1.9.0/photutils/detection/tests/data/irafstarfind_test_thresh08.0_fwhm01.5.txt`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/detection/tests/data/irafstarfind_test_thresh08.0_fwhm02.0.txt` & `photutils-1.9.0/photutils/detection/tests/data/irafstarfind_test_thresh08.0_fwhm02.0.txt`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/detection/tests/data/irafstarfind_test_thresh10.0_fwhm01.0.txt` & `photutils-1.9.0/photutils/detection/tests/data/irafstarfind_test_thresh10.0_fwhm01.0.txt`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/detection/tests/data/irafstarfind_test_thresh10.0_fwhm01.5.txt` & `photutils-1.9.0/photutils/detection/tests/data/irafstarfind_test_thresh10.0_fwhm01.5.txt`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/detection/tests/data/irafstarfind_test_thresh10.0_fwhm02.0.txt` & `photutils-1.9.0/photutils/detection/tests/data/irafstarfind_test_thresh10.0_fwhm02.0.txt`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/detection/tests/test_daofinder.py` & `photutils-1.9.0/photutils/detection/tests/test_daofinder.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/detection/tests/test_irafstarfinder.py` & `photutils-1.9.0/photutils/detection/tests/test_irafstarfinder.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # Licensed under a 3-clause BSD style license - see LICENSE.rst
 """
 Tests for IRAFStarFinder.
 """
 
 import itertools
 import os.path as op
+from contextlib import nullcontext
 
 import numpy as np
 import pytest
 from astropy.table import Table
 from numpy.testing import assert_allclose
 
 from photutils.datasets import make_100gaussians_image
 from photutils.detection.irafstarfinder import IRAFStarFinder
+from photutils.tests.helper import PYTEST_LT_80
 from photutils.utils._optional_deps import HAS_SCIPY
 from photutils.utils.exceptions import NoDetectionsWarning
 
 DATA = make_100gaussians_image()
 THRESHOLDS = [8.0, 10.0]
 FWHMS = [1.0, 1.5, 2.0]
 
@@ -77,16 +79,22 @@
 
     def test_irafstarfind_sky(self):
         starfinder = IRAFStarFinder(threshold=25.0, fwhm=2.0, sky=10.0)
         tbl = starfinder(DATA)
         assert len(tbl) == 4
 
     def test_irafstarfind_largesky(self):
-        with pytest.warns(NoDetectionsWarning,
-                          match='Sources were found, but none pass'):
+        match1 = 'Sources were found, but none pass'
+        ctx1 = pytest.warns(NoDetectionsWarning, match=match1)
+        if PYTEST_LT_80:
+            ctx2 = nullcontext()
+        else:
+            match2 = 'invalid value encountered in divide'
+            ctx2 = pytest.warns(RuntimeWarning, match=match2)
+        with ctx1, ctx2:
             starfinder = IRAFStarFinder(threshold=25.0, fwhm=2.0, sky=100.0)
             tbl = starfinder(DATA)
             assert tbl is None
 
     def test_irafstarfind_peakmax_filtering(self):
         """
         Regression test that objects with ``peak`` >= ``peakmax`` are
```

### Comparing `photutils-1.8.0/photutils/detection/tests/test_peakfinder.py` & `photutils-1.9.0/photutils/detection/tests/test_peakfinder.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/detection/tests/test_starfinder.py` & `photutils-1.9.0/photutils/detection/tests/test_starfinder.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/geometry/circular_overlap.pyx` & `photutils-1.9.0/photutils/geometry/circular_overlap.pyx`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/geometry/core.pxd` & `photutils-1.9.0/photutils/geometry/core.pxd`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/geometry/core.pyx` & `photutils-1.9.0/photutils/geometry/core.pyx`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/geometry/elliptical_overlap.pyx` & `photutils-1.9.0/photutils/geometry/elliptical_overlap.pyx`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/geometry/rectangular_overlap.pyx` & `photutils-1.9.0/photutils/geometry/rectangular_overlap.pyx`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/geometry/tests/test_circular_overlap_grid.py` & `photutils-1.9.0/photutils/geometry/tests/test_circular_overlap_grid.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/geometry/tests/test_elliptical_overlap_grid.py` & `photutils-1.9.0/photutils/geometry/tests/test_elliptical_overlap_grid.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/geometry/tests/test_rectangular_overlap_grid.py` & `photutils-1.9.0/photutils/geometry/tests/test_rectangular_overlap_grid.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/isophote/ellipse.py` & `photutils-1.9.0/photutils/isophote/ellipse.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/isophote/fitter.py` & `photutils-1.9.0/photutils/isophote/fitter.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/isophote/geometry.py` & `photutils-1.9.0/photutils/isophote/geometry.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/isophote/harmonics.py` & `photutils-1.9.0/photutils/isophote/harmonics.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/isophote/integrator.py` & `photutils-1.9.0/photutils/isophote/integrator.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/isophote/isophote.py` & `photutils-1.9.0/photutils/isophote/isophote.py`

 * *Files 1% similar despite different names*

```diff
@@ -791,15 +791,15 @@
     result : `dict`
         An dictionary with the list of the isophote_list properties.
     """
     properties = {}
     for an_item in isophote_list.__class__.__dict__:
         p_type = isophote_list.__class__.__dict__[an_item]
         # Exclude the sample property
-        if type(p_type) == property and 'sample' not in an_item:
+        if isinstance(p_type, property) and 'sample' not in an_item:
             properties[str(an_item)] = str(an_item)
     return properties
 
 
 def _isophote_list_to_table(isophote_list, columns='main'):
     """
     Convert an `~photutils.isophote.IsophoteList` instance to
```

### Comparing `photutils-1.8.0/photutils/isophote/model.py` & `photutils-1.9.0/photutils/isophote/model.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/isophote/sample.py` & `photutils-1.9.0/photutils/isophote/sample.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/isophote/tests/data/M51_table.fits` & `photutils-1.9.0/photutils/isophote/tests/data/M51_table.fits`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/isophote/tests/data/minimum_radius_test.fits` & `photutils-1.9.0/photutils/isophote/tests/data/minimum_radius_test.fits`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/isophote/tests/data/synth_highsnr_table.fits` & `photutils-1.9.0/photutils/isophote/tests/data/synth_highsnr_table.fits`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/isophote/tests/data/synth_lowsnr_table.fits` & `photutils-1.9.0/photutils/isophote/tests/data/synth_lowsnr_table.fits`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/isophote/tests/data/synth_table.fits` & `photutils-1.9.0/photutils/isophote/tests/data/synth_table.fits`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/isophote/tests/data/synth_table_mean.fits` & `photutils-1.9.0/photutils/isophote/tests/data/synth_table_mean.fits`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/isophote/tests/data/synth_table_mean.txt` & `photutils-1.9.0/photutils/isophote/tests/data/synth_table_mean.txt`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/isophote/tests/make_test_data.py` & `photutils-1.9.0/photutils/isophote/tests/make_test_data.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/isophote/tests/test_angles.py` & `photutils-1.9.0/photutils/isophote/tests/test_angles.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/isophote/tests/test_ellipse.py` & `photutils-1.9.0/photutils/isophote/tests/test_ellipse.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 # Licensed under a 3-clause BSD style license - see LICENSE.rst
 """
 Tests for the ellipse module.
 """
 
 import math
+from contextlib import nullcontext
 
 import numpy as np
 import pytest
 from astropy.io import fits
 from astropy.modeling.models import Gaussian2D
+from astropy.utils.exceptions import AstropyUserWarning
 
 from photutils.datasets import get_path, make_noise_image
 from photutils.isophote.ellipse import Ellipse
 from photutils.isophote.geometry import EllipseGeometry
 from photutils.isophote.isophote import Isophote, IsophoteList
 from photutils.isophote.tests.make_test_data import make_test_image
+from photutils.tests.helper import PYTEST_LT_80
 from photutils.utils._optional_deps import HAS_SCIPY
 
 # define an off-center position and a tilted sma
 POS = 384
 PA = 10.0 / 180.0 * np.pi
 
 # build off-center test data. It's fine to have a single np array to use
@@ -87,18 +90,31 @@
         assert isophote.valid
 
     def test_offcenter_fail(self):
         # A first guess ellipse that is centered in the image frame.
         # This should result in failure since the real galaxy
         # image is off-center by a large offset.
         ellipse = Ellipse(OFFSET_GALAXY)
-        with pytest.warns(RuntimeWarning, match='Degrees of freedom'):
-            isophote_list = ellipse.fit_image()
 
-        assert len(isophote_list) == 0
+        match1 = 'Degrees of freedom'
+        ctx1 = pytest.warns(RuntimeWarning, match=match1)
+        if PYTEST_LT_80:
+            ctx2 = nullcontext()
+            ctx3 = nullcontext()
+            ctx4 = nullcontext()
+        else:
+            match2 = 'Mean of empty slice'
+            match3 = 'invalid value encountered'
+            match4 = 'No meaningful fit was possible'
+            ctx2 = pytest.warns(RuntimeWarning, match=match2)
+            ctx3 = pytest.warns(RuntimeWarning, match=match3)
+            ctx4 = pytest.warns(AstropyUserWarning, match=match4)
+        with ctx1, ctx2, ctx3, ctx4:
+            isophote_list = ellipse.fit_image()
+            assert len(isophote_list) == 0
 
     def test_offcenter_fit(self):
         # A first guess ellipse that is roughly centered on the
         # offset galaxy image.
         g = EllipseGeometry(POS + 5, POS + 5, 10.0, eps=0.2, pa=PA, astep=0.1)
         ellipse = Ellipse(OFFSET_GALAXY, geometry=g)
         isophote_list = ellipse.fit_image()
```

### Comparing `photutils-1.8.0/photutils/isophote/tests/test_fitter.py` & `photutils-1.9.0/photutils/isophote/tests/test_fitter.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/isophote/tests/test_geometry.py` & `photutils-1.9.0/photutils/isophote/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/isophote/tests/test_harmonics.py` & `photutils-1.9.0/photutils/isophote/tests/test_harmonics.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/isophote/tests/test_integrator.py` & `photutils-1.9.0/photutils/isophote/tests/test_integrator.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/isophote/tests/test_isophote.py` & `photutils-1.9.0/photutils/isophote/tests/test_isophote.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/isophote/tests/test_model.py` & `photutils-1.9.0/photutils/isophote/tests/test_model.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 # Licensed under a 3-clause BSD style license - see LICENSE.rst
 """
 Tests for the model module.
 """
 
 import warnings
+from contextlib import nullcontext
 
 import numpy as np
 import pytest
 from astropy.io import fits
 from astropy.utils.data import get_pkg_data_filename
 
 from photutils.datasets import get_path
 from photutils.isophote.ellipse import Ellipse
 from photutils.isophote.geometry import EllipseGeometry
 from photutils.isophote.model import build_ellipse_model
 from photutils.isophote.tests.make_test_data import make_test_image
+from photutils.tests.helper import PYTEST_LT_80
 from photutils.utils._optional_deps import HAS_SCIPY
 
 
 @pytest.mark.remote_data
 @pytest.mark.skipif(not HAS_SCIPY, reason='scipy is required')
 def test_model():
     path = get_path('isophote/M105-S001-RGB.fits',
@@ -69,21 +71,31 @@
     # This test requires a "defective" image that drives the
     # model building algorithm into a corner, where it fails.
     # With the algorithm fixed, it bypasses the failure and
     # succeeds in building the model image.
     filepath = get_pkg_data_filename('data/minimum_radius_test.fits')
     with fits.open(filepath) as hdu:
         data = hdu[0].data
-
         g = EllipseGeometry(50.0, 45, 530.0, 0.1, 10.0 / 180.0 * np.pi)
         g.find_center(data)
         ellipse = Ellipse(data, geometry=g)
-        with pytest.warns(RuntimeWarning, match='Degrees of freedom'):
-            isophote_list = ellipse.fit_image(sma0=40, minsma=0, maxsma=350.0,
-                                              step=0.4, nclip=3)
+
+        match1 = 'Degrees of freedom'
+        ctx1 = pytest.warns(RuntimeWarning, match=match1)
+        if PYTEST_LT_80:
+            ctx2 = nullcontext()
+            ctx3 = nullcontext()
+        else:
+            match2 = 'Mean of empty slice'
+            match3 = 'invalid value encountered'
+            ctx2 = pytest.warns(RuntimeWarning, match=match2)
+            ctx3 = pytest.warns(RuntimeWarning, match=match3)
+        with ctx1, ctx2, ctx3:
+            isophote_list = ellipse.fit_image(sma0=40, minsma=0,
+                                              maxsma=350.0, step=0.4, nclip=3)
 
         model = build_ellipse_model(data.shape, isophote_list,
                                     fill=np.mean(data[0:50, 0:50]))
 
         # It's enough that the algorithm reached this point. The
         # actual accuracy of the modelling is being tested elsewhere.
         assert data.shape == model.shape
```

### Comparing `photutils-1.8.0/photutils/isophote/tests/test_regression.py` & `photutils-1.9.0/photutils/isophote/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/isophote/tests/test_sample.py` & `photutils-1.9.0/photutils/isophote/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/morphology/core.py` & `photutils-1.9.0/photutils/morphology/core.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/morphology/non_parametric.py` & `photutils-1.9.0/photutils/morphology/non_parametric.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/morphology/tests/test_core.py` & `photutils-1.9.0/photutils/morphology/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/profiles/core.py` & `photutils-1.9.0/photutils/profiles/core.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/profiles/curve_of_growth.py` & `photutils-1.9.0/photutils/profiles/curve_of_growth.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/profiles/radial_profile.py` & `photutils-1.9.0/photutils/profiles/radial_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -284,14 +284,21 @@
     """
 
     @lazyproperty
     def radius(self):
         """
         The profile radius (bin centers) in pixels as a 1D
         `~numpy.ndarray`.
+
+        The returned radius values are defined as the arithmetic means
+        of the input radial-bins edges (``radii``).
+
+        For logarithmically-spaced input ``radii``, one could instead
+        use a radius array defined using the geometric mean of the bin
+        edges, i.e. ``np.sqrt(radii[:-1] * radii[1:])``.
         """
         # define the radial bin centers from the radial bin edges
         return (self.radii[:-1] + self.radii[1:]) / 2
 
     @lazyproperty
     def apertures(self):
         """
```

### Comparing `photutils-1.8.0/photutils/profiles/tests/test_curve_of_growth.py` & `photutils-1.9.0/photutils/profiles/tests/test_curve_of_growth.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/profiles/tests/test_radial_profile.py` & `photutils-1.9.0/photutils/profiles/tests/test_radial_profile.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/psf/__init__.py` & `photutils-1.9.0/photutils/psf/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 # Licensed under a 3-clause BSD style license - see LICENSE.rst
 """
 This subpackage contains tools to perform point-spread-function (PSF)
 photometry.
 """
 
-from . import epsf, epsf_stars, groupstars, models, photometry, utils
+from . import (epsf, epsf_stars, griddedpsfmodel, groupers, groupstars,
+               models, photometry, photometry_depr, utils)
 from .epsf import *  # noqa: F401, F403
 from .epsf_stars import *  # noqa: F401, F403
+from .griddedpsfmodel import *  # noqa: F401, F403
+from .groupers import *  # noqa: F401, F403
 from .groupstars import *  # noqa: F401, F403
 from .matching import *  # noqa: F401, F403
 from .models import *  # noqa: F401, F403
 from .photometry import *  # noqa: F401, F403
+from .photometry_depr import *  # noqa: F401, F403
 from .utils import *  # noqa: F401, F403
 
 # exclude matching from this list to avoid sphinx warnings
 __all__ = []
 __all__.extend(epsf.__all__)
 __all__.extend(epsf_stars.__all__)
+__all__.extend(griddedpsfmodel.__all__)
+__all__.extend(groupers.__all__)
 __all__.extend(groupstars.__all__)
 __all__.extend(models.__all__)
 __all__.extend(photometry.__all__)
+__all__.extend(photometry_depr.__all__)
 __all__.extend(utils.__all__)
```

### Comparing `photutils-1.8.0/photutils/psf/epsf.py` & `photutils-1.9.0/photutils/psf/epsf.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,18 @@
 from astropy.stats import SigmaClip
 from astropy.utils.exceptions import AstropyUserWarning
 
 from photutils.centroids import centroid_com
 from photutils.psf.epsf_stars import EPSFStar, EPSFStars, LinkedEPSFStar
 from photutils.psf.models import EPSFModel
 from photutils.psf.utils import _interpolate_missing_data
-from photutils.utils._optional_deps import HAS_BOTTLENECK, HAS_TQDM
+from photutils.utils._optional_deps import HAS_BOTTLENECK
 from photutils.utils._parameters import as_pair
-from photutils.utils._round import _py2intround
+from photutils.utils._progress_bars import add_progress_bar
+from photutils.utils._round import py2intround
 
 __all__ = ['EPSFFitter', 'EPSFBuilder']
 
 
 class EPSFFitter:
     """
     Class to fit an ePSF model to one or more stars.
@@ -449,16 +450,16 @@
                     - epsf.evaluate(x=x, y=y, flux=1.0, x_0=0.0, y_0=0.0))
 
         x = epsf.oversampling[1] * star._xidx_centered
         y = epsf.oversampling[0] * star._yidx_centered
 
         epsf_xcenter, epsf_ycenter = (int((epsf.data.shape[1] - 1) / 2),
                                       int((epsf.data.shape[0] - 1) / 2))
-        xidx = _py2intround(x + epsf_xcenter)
-        yidx = _py2intround(y + epsf_ycenter)
+        xidx = py2intround(x + epsf_xcenter)
+        yidx = py2intround(y + epsf_ycenter)
 
         resampled_img = np.full(epsf.shape, np.nan)
 
         mask = np.logical_and(np.logical_and(xidx >= 0, xidx < epsf.shape[1]),
                               np.logical_and(yidx >= 0, yidx < epsf.shape[0]))
         xidx_ = xidx[mask]
         yidx_ = yidx[mask]
@@ -754,20 +755,18 @@
         iter_num = 0
         n_stars = stars.n_stars
         fit_failed = np.zeros(n_stars, dtype=bool)
         epsf = init_epsf
         center_dist_sq = self.center_accuracy_sq + 1.0
         centers = stars.cutout_center_flat
 
-        if self.progress_bar and HAS_TQDM:
-            from tqdm.auto import tqdm
-            pbar_desc = f'EPSFBuilder ({self.maxiters} maxiters)'
-            pbar = tqdm(total=self.maxiters, desc=pbar_desc)
-        else:
-            pbar = None
+        pbar = None
+        if self.progress_bar:
+            desc = f'EPSFBuilder ({self.maxiters} maxiters)'
+            pbar = add_progress_bar(total=self.maxiters, desc=desc)  # pragma: no cover
 
         while (iter_num < self.maxiters and not np.all(fit_failed)
                and np.max(center_dist_sq) >= self.center_accuracy_sq):
 
             iter_num += 1
 
             # build/improve the ePSF
```

### Comparing `photutils-1.8.0/photutils/psf/epsf_stars.py` & `photutils-1.9.0/photutils/psf/epsf_stars.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/psf/groupstars.py` & `photutils-1.9.0/photutils/psf/groupstars.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,18 +3,20 @@
 This module provides classes to perform grouping of stars.
 """
 
 import abc
 
 import numpy as np
 from astropy.table import Column
+from astropy.utils.decorators import deprecated
 
 __all__ = ['DAOGroup', 'DBSCANGroup', 'GroupStarsBase']
 
 
+@deprecated('1.9.0', alternative='`photutils.psf.SourceGrouper`')
 class GroupStarsBase(metaclass=abc.ABCMeta):
     """
     This base class provides the basic interface for subclasses that
     are capable of classifying stars in groups.
     """
 
     def __call__(self, starlist):
@@ -55,14 +57,15 @@
             ``starlist`` with an additional column named ``group_id``
             whose unique values represent groups of mutually overlapping
             stars.
         """
         raise NotImplementedError('Needs to be implemented in a subclass.')
 
 
+@deprecated('1.9.0', alternative='`photutils.psf.SourceGrouper`')
 class DAOGroup(GroupStarsBase):
     """
     This class implements the DAOGROUP algorithm presented by
     Stetson (1987).
 
     The method ``group_stars`` divides an entire starlist into sets of
     distinct, self-contained groups of mutually overlapping stars.
@@ -170,14 +173,15 @@
         """
         star_distance = np.hypot(star['x_0'] - starlist['x_0'],
                                  star['y_0'] - starlist['y_0'])
         distance_criteria = star_distance < self.crit_separation
         return np.asarray(starlist[distance_criteria]['id'])
 
 
+@deprecated('1.9.0', alternative='`photutils.psf.SourceGrouper`')
 class DBSCANGroup(GroupStarsBase):
     """
     Class to create star groups according to a distance criteria using
     the Density-based Spatial Clustering of Applications with Noise
     (DBSCAN) from scikit-learn.
 
     Parameters
```

### Comparing `photutils-1.8.0/photutils/psf/matching/fourier.py` & `photutils-1.9.0/photutils/psf/matching/fourier.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/psf/matching/tests/test_fourier.py` & `photutils-1.9.0/photutils/psf/matching/tests/test_fourier.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/psf/matching/tests/test_windows.py` & `photutils-1.9.0/photutils/psf/matching/tests/test_windows.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,16 +39,15 @@
     assert_allclose(data[1, :], ref)
 
 
 @pytest.mark.skipif(not HAS_SCIPY, reason='scipy is required')
 def test_tukey_scipy():
     """Test Tukey window against 1D scipy version."""
 
-    # scipy.signal.tukey was introduced in Scipy v0.16.0
-    from scipy.signal import tukey
+    from scipy.signal.windows import tukey
 
     size = 101
     cen = (size - 1) // 2
     shape = (size, size)
     alpha = 0.4
     win = TukeyWindow(alpha=alpha)
     data = win(shape)
```

### Comparing `photutils-1.8.0/photutils/psf/matching/windows.py` & `photutils-1.9.0/photutils/psf/matching/windows.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/psf/models.py` & `photutils-1.9.0/photutils/psf/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 # Licensed under a 3-clause BSD style license - see LICENSE.rst
 """
 This module provides models for doing PSF/PRF-fitting photometry.
 """
 
 import copy
-import itertools
 import warnings
-from functools import lru_cache
 
 import numpy as np
 from astropy.modeling import Fittable2DModel, Parameter
-from astropy.nddata import NDData
 from astropy.utils.exceptions import AstropyWarning
 
 from photutils.aperture import CircularAperture
 from photutils.utils._parameters import as_pair
 
 __all__ = ['NonNormalizable', 'FittableImageModel', 'EPSFModel',
-           'GriddedPSFModel', 'IntegratedGaussianPRF', 'PRFAdapter']
+           'IntegratedGaussianPRF', 'PRFAdapter']
 
 
 class NonNormalizable(AstropyWarning):
     """
     Used to indicate that a :py:class:`FittableImageModel` model is
     non-normalizable.
     """
@@ -678,258 +675,14 @@
                        | ((yi < 0) | (yi > (self._ny - 1)
                                       / self.oversampling[0])))
             evaluated_model[invalid] = self._fill_value
 
         return evaluated_model
 
 
-class GriddedPSFModel(Fittable2DModel):
-    """
-    A fittable 2D model containing a grid PSF models defined at specific
-    locations that are interpolated to evaluate a PSF at an arbitrary
-    (x, y) position.
-
-    Parameters
-    ----------
-    data : `~astropy.nddata.NDData`
-        An `~astropy.nddata.NDData` object containing the grid of
-        reference PSF arrays.  The data attribute must contain a 3D
-        `~numpy.ndarray` containing a stack of the 2D PSFs (the data
-        shape should be (N_psf, PSF_ny, PSF_nx)).  The meta
-        attribute must be `dict` containing the following:
-
-            * ``'grid_xypos'``:  A list of the (x, y) grid positions of
-              each reference PSF.  The order of positions should match
-              the first axis of the 3D `~numpy.ndarray` of PSFs.  In
-              other words, ``grid_xypos[i]`` should be the (x, y)
-              position of the reference PSF defined in ``data[i]``.
-            * ``'oversampling'``:  The integer oversampling factor of the
-               PSF.
-
-        The meta attribute may contain other properties such as the
-        telescope, instrument, detector, and filter of the PSF.
-    """
-
-    flux = Parameter(description='Intensity scaling factor for the PSF '
-                     'model.', default=1.0)
-    x_0 = Parameter(description='x position in the output coordinate grid '
-                    'where the model is evaluated.', default=0.0)
-    y_0 = Parameter(description='y position in the output coordinate grid '
-                    'where the model is evaluated.', default=0.0)
-
-    def __init__(self, data, *, flux=flux.default, x_0=x_0.default,
-                 y_0=y_0.default, fill_value=0.0):
-
-        if not isinstance(data, NDData):
-            raise TypeError('data must be an NDData instance.')
-
-        if data.data.ndim != 3:
-            raise ValueError('The NDData data attribute must be a 3D numpy '
-                             'ndarray')
-
-        if 'grid_xypos' not in data.meta:
-            raise ValueError('"grid_xypos" must be in the nddata meta '
-                             'dictionary.')
-        if len(data.meta['grid_xypos']) != data.data.shape[0]:
-            raise ValueError('The length of grid_xypos must match the number '
-                             'of input PSFs.')
-
-        if 'oversampling' not in data.meta:
-            raise ValueError('"oversampling" must be in the nddata meta '
-                             'dictionary.')
-        if not np.isscalar(data.meta['oversampling']):
-            raise ValueError('oversampling must be a scalar value')
-
-        self.data = np.array(data.data, copy=True, dtype=float)
-        self.meta = data.meta
-        self.grid_xypos = data.meta['grid_xypos']
-        self.oversampling = data.meta['oversampling']
-        self._fill_value = fill_value
-
-        self._grid_xpos, self._grid_ypos = np.transpose(self.grid_xypos)
-        self._xgrid = np.unique(self._grid_xpos)  # also sorts values
-        self._ygrid = np.unique(self._grid_ypos)  # also sorts values
-
-        if (len(list(itertools.product(self._xgrid, self._ygrid)))
-                != len(self.grid_xypos)):
-            raise ValueError('"grid_xypos" must form a regular grid.')
-
-        self._xgrid_min = self._xgrid[0]
-        self._xgrid_max = self._xgrid[-1]
-        self._ygrid_min = self._ygrid[0]
-        self._ygrid_max = self._ygrid[-1]
-        self._ref_indices = None
-        self._psf_interp = None
-
-        # NOTE: replace @lru_cache with @cache for Python 3.9+;
-        # Here we avoid decorating the instance method with
-        # @lru_cache/cache to prevent memory leaks
-        self._compute_local_model = lru_cache(maxsize=128)(
-            self._compute_local_model_uncached)
-
-        super().__init__(flux, x_0, y_0)
-
-    @staticmethod
-    def _find_start_idx(data, x):
-        """
-        Find the index of the lower bound where ``x`` should be inserted
-        into ``a`` to maintain order.
-
-        The index of the upper bound is the index of the lower bound
-        plus 2.  Both bound indices must be within the array.
-
-        Parameters
-        ----------
-        data : 1D `~numpy.ndarray`
-            The 1D array to search.
-
-        x : float
-            The value to insert.
-
-        Returns
-        -------
-        index : int
-            The index of the lower bound.
-        """
-        idx = np.searchsorted(data, x)
-        if idx == 0:
-            idx0 = 0
-        elif idx == len(data):  # pragma: no cover
-            idx0 = idx - 2
-        else:
-            idx0 = idx - 1
-        return idx0
-
-    def _find_bounding_points(self, x, y):
-        """
-        Find the indices of the grid points that bound the input
-        ``(x, y)`` position.
-
-        Parameters
-        ----------
-        x, y : float
-            The ``(x, y)`` position where the PSF is to be evaluated.
-            The position must be inside the region defined by the grid
-            of PSF positions.
-
-        Returns
-        -------
-        indices : list of int
-            A list of indices of the bounding grid points.
-        """
-        x0 = self._find_start_idx(self._xgrid, x)
-        y0 = self._find_start_idx(self._ygrid, y)
-        xypoints = list(itertools.product(self._xgrid[x0:x0 + 2],
-                                          self._ygrid[y0:y0 + 2]))
-
-        # find the grid_xypos indices of the reference xypoints
-        indices = []
-        for xx, yy in xypoints:
-            indices.append(np.argsort(np.hypot(self._grid_xpos - xx,
-                                               self._grid_ypos - yy))[0])
-
-        return indices
-
-    @staticmethod
-    def _bilinear_interp(xyref, zref, xi, yi):
-        """
-        Perform bilinear interpolation of four 2D arrays located at
-        points on a regular grid.
-
-        Parameters
-        ----------
-        xyref : list of 4 (x, y) pairs
-            A list of 4 ``(x, y)`` pairs that form a rectangle.
-
-        zref : 3D `~numpy.ndarray`
-            A 3D `~numpy.ndarray` of shape ``(4, nx, ny)``. The first
-            axis corresponds to ``xyref``, i.e., ``refdata[0, :, :]`` is
-            the 2D array located at ``xyref[0]``.
-
-        xi, yi : float
-            The ``(xi, yi)`` point at which to perform the
-            interpolation.  The ``(xi, yi)`` point must lie within the
-            rectangle defined by ``xyref``.
-
-        Returns
-        -------
-        result : 2D `~numpy.ndarray`
-            The 2D interpolated array.
-        """
-        xyref = [tuple(i) for i in xyref]
-        idx = sorted(range(len(xyref)), key=xyref.__getitem__)
-        xyref = sorted(xyref)  # sort by x, then y
-        (x0, y0), (_x0, y1), (x1, _y0), (_x1, _y1) = xyref
-
-        if x0 != _x0 or x1 != _x1 or y0 != _y0 or y1 != _y1:
-            raise ValueError('The refxy points do not form a rectangle.')
-
-        if not np.isscalar(xi):
-            xi = xi[0]
-        if not np.isscalar(yi):
-            yi = yi[0]
-
-        if not x0 <= xi <= x1 or not y0 <= yi <= y1:
-            raise ValueError('The (x, y) input is not within the rectangle '
-                             'defined by xyref.')
-
-        data = np.asarray(zref)[idx]
-        weights = np.array([(x1 - xi) * (y1 - yi), (x1 - xi) * (yi - y0),
-                            (xi - x0) * (y1 - yi), (xi - x0) * (yi - y0)])
-        norm = (x1 - x0) * (y1 - y0)
-
-        return np.sum(data * weights[:, None, None], axis=0) / norm
-
-    def _compute_local_model_uncached(self, x_0, y_0):
-        """
-        Return `FittableImageModel` for interpolated PSF at some (x_0, y_0).
-        """
-        if (x_0 < self._xgrid_min or x_0 > self._xgrid_max
-                or y_0 < self._ygrid_min or y_0 > self._ygrid_max):
-            # position is outside of the grid, so simply use the
-            # closest reference PSF
-            self._ref_index = np.argsort(np.hypot(self._grid_xpos - x_0,
-                                                  self._grid_ypos - y_0))[0]
-            self._psf_interp = self.data[self._ref_index, :, :]
-        else:
-            # find the four bounding reference PSFs and interpolate
-            self._ref_indices = self._find_bounding_points(x_0, y_0)
-            xyref = np.array(self.grid_xypos)[self._ref_indices]
-            psfs = self.data[self._ref_indices, :, :]
-
-            self._psf_interp = self._bilinear_interp(xyref, psfs, x_0, y_0)
-
-        # Construct the model using the interpolated supersampled data
-        psfmodel = FittableImageModel(self._psf_interp,
-                                      oversampling=self.oversampling)
-        return psfmodel
-
-    def evaluate(self, x, y, flux, x_0, y_0):
-        """
-        Evaluate the `GriddedPSFModel` for the input parameters.
-        """
-        # NOTE: the astropy base Model.__call__() method converts scalar
-        # inputs to size-1 arrays before calling evaluate().
-        if not np.isscalar(flux):
-            flux = flux[0]
-        if not np.isscalar(x_0):
-            x_0 = x_0[0]
-        if not np.isscalar(y_0):
-            y_0 = y_0[0]
-
-        # Calculate the local (interpolated) PSF at (x_0, y_0) from the
-        # grid of PSF models. Only the integer part of the position is
-        # input so that the local model can be cached.
-        psfmodel = self._compute_local_model(int(x_0), int(y_0))
-
-        # now evaluate the PSF at the (x_0, y_0) subpixel position on
-        # the input (x, y) values
-        return psfmodel.evaluate(x, y, flux, x_0, y_0)
-
-
 class IntegratedGaussianPRF(Fittable2DModel):
     r"""
     Circular Gaussian model integrated over pixels.
 
     Because it is integrated, this model is considered a PRF, *not* a
     PSF (see :ref:`psf-terminology` for more about the terminology used
     here.)
```

### Comparing `photutils-1.8.0/photutils/psf/photometry.py` & `photutils-1.9.0/photutils/psf/photometry_depr.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,33 +3,36 @@
 This module provides classes to perform PSF-fitting photometry.
 """
 
 import warnings
 
 import numpy as np
 from astropy.modeling.fitting import LevMarLSQFitter
+from astropy.nddata import StdDevUncertainty
 from astropy.nddata.utils import NoOverlapError, overlap_slices
 from astropy.stats import SigmaClip, gaussian_sigma_to_fwhm
 from astropy.table import Column, QTable, hstack, vstack
+from astropy.utils.decorators import deprecated
 from astropy.utils.exceptions import AstropyUserWarning
 
 from photutils.aperture import CircularAperture, aperture_photometry
 from photutils.background import MMMBackground
 from photutils.detection import DAOStarFinder
 from photutils.psf.groupstars import DAOGroup
 from photutils.psf.utils import (_extract_psf_fitting_names,
                                  get_grouped_psf_model, subtract_psf)
 from photutils.utils._misc import _get_version_info
-from photutils.utils._optional_deps import HAS_TQDM
+from photutils.utils._progress_bars import add_progress_bar
 from photutils.utils.exceptions import NoDetectionsWarning
 
 __all__ = ['BasicPSFPhotometry', 'IterativelySubtractedPSFPhotometry',
            'DAOPhotPSFPhotometry']
 
 
+@deprecated('1.9.0', alternative='`photutils.psf.PSFPhotometry`')
 class BasicPSFPhotometry:
     """
     This class implements a PSF photometry algorithm that can find
     sources in an image, group overlapping sources into a single model,
     fit the model to the sources, and subtracting the models from the
     image. This is roughly equivalent to the DAOPHOT routines FIND,
     GROUP, NSTAR, and SUBTRACT.  This implementation allows a flexible
@@ -278,24 +281,25 @@
             if np.any(finite_mask):
                 warnings.warn('Input data contains unmasked non-finite '
                               'values (NaN or inf), which were '
                               'automatically ignored.', AstropyUserWarning)
         return mask
 
     def __call__(self, image, *, mask=None, init_guesses=None,
-                 progress_bar=False):
+                 progress_bar=False, uncertainty=None):
         """
         Perform PSF photometry. See `do_photometry` for more details
         including the `__call__` signature.
         """
         return self.do_photometry(image, mask=mask, init_guesses=init_guesses,
-                                  progress_bar=progress_bar)
+                                  progress_bar=progress_bar,
+                                  uncertainty=uncertainty)
 
     def do_photometry(self, image, *, mask=None, init_guesses=None,
-                      progress_bar=False):
+                      progress_bar=False, uncertainty=None):
         """
         Perform PSF photometry in ``image``.
 
         This method assumes that ``psf_model`` has centroids and flux
         parameters which will be fitted to the data provided in
         ``image``. A compound model, in fact a sum of ``psf_model``,
         will be fitted to groups of stars automatically identified by
@@ -330,14 +334,16 @@
             ``image`` is masked.
         progress_bar : bool, optional
             Whether to display a progress bar when fitting the
             star groups. The progress bar requires that the `tqdm
             <https://tqdm.github.io/>`_ optional dependency be
             installed. Note that the progress bar does not currently
             work in the Jupyter console due to limitations in ``tqdm``.
+        uncertainty : 2D `~numpy.ndarray`, optional
+            Stddev uncertainty for each element in ``image``.
 
         Returns
         -------
         output_tab : `~astropy.table.Table` or None
             Table with the photometry results, i.e., centroids and
             fluxes estimations and the initial estimates used to start
             the fitting process. Uncertainties on the fitted parameters
@@ -426,15 +432,17 @@
 
         if skip_group_maker:
             star_groups = init_guesses
         else:
             star_groups = self.group_maker(init_guesses)
 
         output_tab, self._residual_image = self.nstar(
-            image, star_groups, mask=mask, progress_bar=progress_bar)
+            image, star_groups, mask=mask, progress_bar=progress_bar,
+            uncertainty=uncertainty
+        )
         star_groups = star_groups.group_by('group_id')
 
         if hasattr(output_tab, 'update'):  # requires Astropy >= 5.0
             star_groups.update(output_tab)
         else:
             common_cols = set(star_groups.colnames).intersection(
                 output_tab.colnames)
@@ -444,15 +452,16 @@
                 else:
                     star_groups.add_column(col, name=name, copy=True)
 
         star_groups.meta = {'version': _get_version_info()}
 
         return star_groups
 
-    def nstar(self, image, star_groups, *, mask=None, progress_bar=False):
+    def nstar(self, image, star_groups, *, mask=None, progress_bar=False,
+              uncertainty=None):
         """
         Fit, as appropriate, a compound or single model to the given
         ``star_groups``. Groups are fitted sequentially from the
         smallest to the biggest. In each iteration, ``image`` is
         subtracted by the previous fitted group.
 
         Parameters
@@ -478,14 +487,17 @@
         progress_bar : bool, optional
             Use a progress bar to show progress over the star groups.
             The progress bar requires that the `tqdm
             <https://tqdm.github.io/>`_ optional dependency be
             installed. Note that the progress bar does not currently
             work in the Jupyter console due to limitations in ``tqdm``.
 
+        uncertainty : 2D `~numpy.ndarray`, optional
+            Stddev uncertainty for each element in ``image``.
+
         Returns
         -------
         result_tab : `~astropy.table.QTable`
             Astropy table that contains photometry results.
 
         image : 2D `~numpy.ndarray`
             Residual image.
@@ -499,18 +511,17 @@
             if not isfixed:
                 unc_tab.add_column(Column(name=param + "_unc"))
 
         y, x = np.indices(image.shape)
 
         star_groups = star_groups.group_by('group_id')
         group_iter = star_groups.groups
-        if progress_bar and HAS_TQDM:
-            from tqdm.auto import tqdm  # pragma: no cover
 
-            group_iter = tqdm(group_iter, desc='Star Group')  # pragma: no cover
+        if progress_bar:
+            group_iter = add_progress_bar(group_iter, desc='Fit source/group')  # pragma: no cover
 
         for group in group_iter:
             group_psf = get_grouped_psf_model(self.psf_model, group,
                                               self._pars_to_set)
             usepixel = np.zeros_like(image, dtype=bool)
 
             for row in group:
@@ -518,16 +529,24 @@
                                         small_array_shape=self.fitshape,
                                         position=(row['y_0'], row['x_0']),
                                         mode='trim')[0]] = True
 
             if mask is not None:
                 usepixel &= ~mask
 
+            if hasattr(image, 'uncertainty'):
+                sigma = image.uncertainty.represent_as(StdDevUncertainty).array
+                weights = 1 / sigma[usepixel]
+            elif uncertainty is not None:
+                weights = 1 / uncertainty[usepixel]
+            else:
+                weights = None
+
             fit_model = self.fitter(group_psf, x[usepixel], y[usepixel],
-                                    image[usepixel])
+                                    image[usepixel], weights=weights)
             param_table = self._model_params2table(fit_model, group)
             result_tab = vstack([result_tab, param_table])
             unc_tab = vstack([unc_tab, self._get_uncertainties(len(group))])
 
             # do not subtract if the fitting did not go well
             try:
                 image = subtract_psf(image, self.psf_model, param_table,
@@ -664,14 +683,15 @@
             for param_tab_name, param_name in self._pars_to_output.items():
                 param_tab[param_tab_name] = getattr(fit_model,
                                                     param_name).value
 
         return param_tab
 
 
+@deprecated('1.9.0', alternative='`photutils.psf.IterativePSFPhotometry`')
 class IterativelySubtractedPSFPhotometry(BasicPSFPhotometry):
     """
     This class implements an iterative algorithm to perform point spread
     function photometry in crowded fields. This consists of applying a
     loop of find sources, make groups, fit groups, subtract groups, and
     then repeat until no more stars are detected or a given number of
     iterations is reached.
@@ -802,15 +822,15 @@
             raise ValueError("finder cannot be None for "
                              "IterativelySubtractedPSFPhotometry - you may "
                              "want to use BasicPSFPhotometry. Please see the "
                              "Detection section on photutils documentation.")
         self._finder = value
 
     def do_photometry(self, image, *, mask=None, init_guesses=None,
-                      progress_bar=False):
+                      progress_bar=False, uncertainty=None):
         """
         Perform PSF photometry in ``image``.
 
         This method assumes that ``psf_model`` has centroids and flux
         parameters which will be fitted to the data provided in
         ``image``. A compound model, in fact a sum of ``psf_model``,
         will be fitted to groups of stars automatically identified by
@@ -839,14 +859,16 @@
             ``extra_output_cols`` the initial values are used; if the columns
             specified in ``extra_output_cols`` are not given in
             ``init_guesses`` then NaNs will be returned.
         mask : 2D bool `~numpy.ndarray`, optional
             A boolean mask with the same shape as ``image``, where
             a `True` value indicates the corresponding element of
             ``image`` is masked.
+        uncertainty : 2D `~numpy.ndarray`, optional
+            Stddev uncertainty for each element in ``image``.
 
         Returns
         -------
         output_table : `~astropy.table.Table` or None
             A table with the photometry results, i.e., centroids and
             fluxes estimations and the initial estimates used to start
             the fitting process. Uncertainties on the fitted parameters
@@ -856,39 +878,43 @@
             covariance matrix.
         """
         mask = super()._make_mask(image, mask)
 
         if init_guesses is not None:
             table = super().do_photometry(image, mask=mask,
                                           init_guesses=init_guesses,
-                                          progress_bar=progress_bar)
+                                          progress_bar=progress_bar,
+                                          uncertainty=uncertainty)
             table['iter_detected'] = np.ones(table['x_fit'].shape, dtype=int)
 
             # n_start = 2 because it starts in the second iteration
             # since the first iteration is above
             output_table = self._do_photometry(n_start=2, mask=mask,
-                                               progress_bar=progress_bar)
+                                               progress_bar=progress_bar,
+                                               uncertainty=uncertainty)
             output_table = vstack([table, output_table])
         else:
             if self.bkg_estimator is not None:
                 self._residual_image = image - self.bkg_estimator(image)
             else:
                 self._residual_image = image
 
             if self.aperture_radius is None:
                 self.set_aperture_radius()
 
             output_table = self._do_photometry(mask=mask,
-                                               progress_bar=progress_bar)
+                                               progress_bar=progress_bar,
+                                               uncertainty=uncertainty)
 
         output_table.meta = {'version': _get_version_info()}
 
         return QTable(output_table)
 
-    def _do_photometry(self, n_start=1, mask=None, progress_bar=False):
+    def _do_photometry(self, n_start=1, mask=None, progress_bar=False,
+                       uncertainty=None):
         """
         Helper function which performs the iterations of the photometry
         process.
 
         Parameters
         ----------
         n_start : int
@@ -934,15 +960,15 @@
                         Column(name=param_tab_name,
                                data=(getattr(self.psf_model, param_name)
                                      * np.ones(len(sources)))))
 
             star_groups = self.group_maker(init_guess_tab)
             table, self._residual_image = super().nstar(
                 self._residual_image, star_groups, mask=mask,
-                progress_bar=progress_bar)
+                progress_bar=progress_bar, uncertainty=uncertainty)
 
             star_groups = star_groups.group_by('group_id')
             table = hstack([star_groups, table])
 
             table['iter_detected'] = n * np.ones(table['x_fit'].shape,
                                                  dtype=int)
 
@@ -954,14 +980,15 @@
                 sources = self.finder(self._residual_image, mask=mask)
 
             n += 1
 
         return output_table
 
 
+@deprecated('1.9.0', alternative='`photutils.psf.IterativePSFPhotometry`')
 class DAOPhotPSFPhotometry(IterativelySubtractedPSFPhotometry):
     """
     This class implements  an iterative algorithm based on the DAOPHOT
     algorithm presented by Stetson (1987) to perform point spread
     function photometry in crowded fields. This consists of applying a
     loop of find sources, make groups, fit groups, subtract groups, and
     then repeat until no more stars are detected or a given number of
```

### Comparing `photutils-1.8.0/photutils/psf/tests/test_epsf.py` & `photutils-1.9.0/photutils/psf/tests/test_epsf.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/psf/tests/test_epsf_stars.py` & `photutils-1.9.0/photutils/psf/tests/test_epsf_stars.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/psf/tests/test_groupstars.py` & `photutils-1.9.0/photutils/psf/tests/test_groupstars.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 """
 Tests for the groupstars module.
 """
 
 import numpy as np
 import pytest
 from astropy.table import Table, vstack
+from astropy.utils.exceptions import AstropyDeprecationWarning
 from numpy.testing import assert_almost_equal
 
 from photutils.psf.groupstars import DAOGroup, DBSCANGroup
 from photutils.utils._optional_deps import HAS_SKLEARN
 
 
 def assert_table_almost_equal(table1, table2):
@@ -38,30 +39,30 @@
              |  *            *                        *             *  |
              +---------+--------+---------+---------+--------+---------+
                        0       0.5        1        1.5       2
 
         x and y axis are in pixel coordinates. Each asterisk represents
         the centroid of a star.
         """
-
-        x_0 = np.array([0, np.sqrt(2) / 4, np.sqrt(2) / 4, -np.sqrt(2) / 4,
-                        -np.sqrt(2) / 4])
-        y_0 = np.array([0, np.sqrt(2) / 4, -np.sqrt(2) / 4, np.sqrt(2) / 4,
-                        -np.sqrt(2) / 4])
-        x_1 = x_0 + 2.0
-        first_group = Table([x_0, y_0, np.arange(len(x_0)) + 1,
-                            np.ones(len(x_0), dtype=int)],
-                            names=('x_0', 'y_0', 'id', 'group_id'))
-        second_group = Table([x_1, y_0, len(x_0) + np.arange(len(x_0)) + 1,
-                              2 * np.ones(len(x_0), dtype=int)],
-                             names=('x_0', 'y_0', 'id', 'group_id'))
-        starlist = vstack([first_group, second_group])
-        daogroup = DAOGroup(crit_separation=0.6)
-        test_starlist = daogroup(starlist['x_0', 'y_0', 'id'])
-        assert_table_almost_equal(starlist, test_starlist)
+        with pytest.warns(AstropyDeprecationWarning):
+            x_0 = np.array([0, np.sqrt(2) / 4, np.sqrt(2) / 4, -np.sqrt(2) / 4,
+                            -np.sqrt(2) / 4])
+            y_0 = np.array([0, np.sqrt(2) / 4, -np.sqrt(2) / 4, np.sqrt(2) / 4,
+                            -np.sqrt(2) / 4])
+            x_1 = x_0 + 2.0
+            first_group = Table([x_0, y_0, np.arange(len(x_0)) + 1,
+                                 np.ones(len(x_0), dtype=int)],
+                                names=('x_0', 'y_0', 'id', 'group_id'))
+            second_group = Table([x_1, y_0, len(x_0) + np.arange(len(x_0)) + 1,
+                                  2 * np.ones(len(x_0), dtype=int)],
+                                 names=('x_0', 'y_0', 'id', 'group_id'))
+            starlist = vstack([first_group, second_group])
+            daogroup = DAOGroup(crit_separation=0.6)
+            test_starlist = daogroup(starlist['x_0', 'y_0', 'id'])
+            assert_table_almost_equal(starlist, test_starlist)
 
     def test_daogroup_two(self):
         """
             +--------------+--------------+-------------+--------------+
           3 +                             *                            +
             |                             *                            |
         2.5 +                             *                            +
@@ -74,25 +75,25 @@
             |                             *                            |
         0.5 +                             *                            +
             |                             *                            |
           0 +                             *                            +
             +--------------+--------------+-------------+--------------+
            -1            -0.5             0            0.5             1
         """
-
-        first_group = Table([np.zeros(5), np.linspace(0, 1, 5),
-                             np.arange(5) + 1, np.ones(5, dtype=int)],
-                            names=('x_0', 'y_0', 'id', 'group_id'))
-        second_group = Table([np.zeros(5), np.linspace(2, 3, 5),
-                              6 + np.arange(5), 2 * np.ones(5, dtype=int)],
-                             names=('x_0', 'y_0', 'id', 'group_id'))
-        starlist = vstack([first_group, second_group])
-        daogroup = DAOGroup(crit_separation=0.3)
-        test_starlist = daogroup(starlist['x_0', 'y_0', 'id'])
-        assert_table_almost_equal(starlist, test_starlist)
+        with pytest.warns(AstropyDeprecationWarning):
+            first_group = Table([np.zeros(5), np.linspace(0, 1, 5),
+                                 np.arange(5) + 1, np.ones(5, dtype=int)],
+                                names=('x_0', 'y_0', 'id', 'group_id'))
+            second_group = Table([np.zeros(5), np.linspace(2, 3, 5),
+                                  6 + np.arange(5), 2 * np.ones(5, dtype=int)],
+                                 names=('x_0', 'y_0', 'id', 'group_id'))
+            starlist = vstack([first_group, second_group])
+            daogroup = DAOGroup(crit_separation=0.3)
+            test_starlist = daogroup(starlist['x_0', 'y_0', 'id'])
+            assert_table_almost_equal(starlist, test_starlist)
 
     def test_daogroup_three(self):
         """
            1 +--+-------+--------+--------+--------+-------+--------+--+
              |                                                         |
              |                                                         |
              |                                                         |
@@ -105,25 +106,25 @@
         -0.5 +                                                         +
              |                                                         |
              |                                                         |
              |                                                         |
           -1 +--+-------+--------+--------+--------+-------+--------+--+
                 0      0.5       1       1.5       2      2.5       3
         """
-
-        first_group = Table([np.linspace(0, 1, 5), np.zeros(5),
-                             np.arange(5) + 1, np.ones(5, dtype=int)],
-                            names=('x_0', 'y_0', 'id', 'group_id'))
-        second_group = Table([np.linspace(2, 3, 5), np.zeros(5),
-                              6 + np.arange(5), 2 * np.ones(5, dtype=int)],
-                             names=('x_0', 'y_0', 'id', 'group_id'))
-        starlist = vstack([first_group, second_group])
-        daogroup = DAOGroup(crit_separation=0.3)
-        test_starlist = daogroup(starlist['x_0', 'y_0', 'id'])
-        assert_table_almost_equal(starlist, test_starlist)
+        with pytest.warns(AstropyDeprecationWarning):
+            first_group = Table([np.linspace(0, 1, 5), np.zeros(5),
+                                 np.arange(5) + 1, np.ones(5, dtype=int)],
+                                names=('x_0', 'y_0', 'id', 'group_id'))
+            second_group = Table([np.linspace(2, 3, 5), np.zeros(5),
+                                  6 + np.arange(5), 2 * np.ones(5, dtype=int)],
+                                 names=('x_0', 'y_0', 'id', 'group_id'))
+            starlist = vstack([first_group, second_group])
+            daogroup = DAOGroup(crit_separation=0.3)
+            test_starlist = daogroup(starlist['x_0', 'y_0', 'id'])
+            assert_table_almost_equal(starlist, test_starlist)
 
     def test_daogroup_four(self):
         """
              +-+---------+---------+---------+---------+-+
            1 +                     *                     +
              |           *                   *           |
              |                                           |
@@ -139,25 +140,25 @@
              |                                           |
              |                                           |
              |           *                   *           |
           -1 +                     *                     +
              +-+---------+---------+---------+---------+-+
               -1       -0.5        0        0.5        1
         """
-
-        x = np.linspace(-1.0, 1.0, 5)
-        y = np.sqrt(1.0 - x**2)
-        xx = np.hstack((x, x))
-        yy = np.hstack((y, -y))
-        starlist = Table([xx, yy, np.arange(10) + 1,
-                          np.ones(10, dtype=int)],
-                         names=('x_0', 'y_0', 'id', 'group_id'))
-        daogroup = DAOGroup(crit_separation=2.5)
-        test_starlist = daogroup(starlist['x_0', 'y_0', 'id'])
-        assert_table_almost_equal(starlist, test_starlist)
+        with pytest.warns(AstropyDeprecationWarning):
+            x = np.linspace(-1.0, 1.0, 5)
+            y = np.sqrt(1.0 - x**2)
+            xx = np.hstack((x, x))
+            yy = np.hstack((y, -y))
+            starlist = Table([xx, yy, np.arange(10) + 1,
+                              np.ones(10, dtype=int)],
+                             names=('x_0', 'y_0', 'id', 'group_id'))
+            daogroup = DAOGroup(crit_separation=2.5)
+            test_starlist = daogroup(starlist['x_0', 'y_0', 'id'])
+            assert_table_almost_equal(starlist, test_starlist)
 
     def test_daogroup_five(self):
         """
             +--+--------+--------+-------+--------+--------+--------+--+
           3 +                            *                             +
             |                            *                             |
         2.5 +                            *                             +
@@ -170,32 +171,33 @@
             |                            *                             |
         0.5 +                            *                             +
             |                            *                             |
           0 +                            *                             +
             +--+--------+--------+-------+--------+--------+--------+--+
                0       0.5       1      1.5       2       2.5       3
         """
-
-        first_group = Table([1.5 * np.ones(5), np.linspace(0, 1, 5),
-                             np.arange(5) + 1, np.ones(5, dtype=int)],
-                            names=('x_0', 'y_0', 'id', 'group_id'))
-        second_group = Table([1.5 * np.ones(5), np.linspace(2, 3, 5),
-                              6 + np.arange(5), 2 * np.ones(5, dtype=int)],
-                             names=('x_0', 'y_0', 'id', 'group_id'))
-        third_group = Table([np.linspace(0, 1, 5), 1.5 * np.ones(5),
-                             11 + np.arange(5), 3 * np.ones(5, dtype=int)],
-                            names=('x_0', 'y_0', 'id', 'group_id'))
-        fourth_group = Table([np.linspace(2, 3, 5), 1.5 * np.ones(5),
-                              16 + np.arange(5), 4 * np.ones(5, dtype=int)],
-                             names=('x_0', 'y_0', 'id', 'group_id'))
-        starlist = vstack([first_group, second_group, third_group,
-                           fourth_group])
-        daogroup = DAOGroup(crit_separation=0.3)
-        test_starlist = daogroup(starlist['x_0', 'y_0', 'id'])
-        assert_table_almost_equal(starlist, test_starlist)
+        with pytest.warns(AstropyDeprecationWarning):
+            first_group = Table([1.5 * np.ones(5), np.linspace(0, 1, 5),
+                                 np.arange(5) + 1, np.ones(5, dtype=int)],
+                                names=('x_0', 'y_0', 'id', 'group_id'))
+            second_group = Table([1.5 * np.ones(5), np.linspace(2, 3, 5),
+                                  6 + np.arange(5), 2 * np.ones(5, dtype=int)],
+                                 names=('x_0', 'y_0', 'id', 'group_id'))
+            third_group = Table([np.linspace(0, 1, 5), 1.5 * np.ones(5),
+                                 11 + np.arange(5), 3 * np.ones(5, dtype=int)],
+                                names=('x_0', 'y_0', 'id', 'group_id'))
+            fourth_group = Table([np.linspace(2, 3, 5), 1.5 * np.ones(5),
+                                  16 + np.arange(5),
+                                  4 * np.ones(5, dtype=int)],
+                                 names=('x_0', 'y_0', 'id', 'group_id'))
+            starlist = vstack([first_group, second_group, third_group,
+                               fourth_group])
+            daogroup = DAOGroup(crit_separation=0.3)
+            test_starlist = daogroup(starlist['x_0', 'y_0', 'id'])
+            assert_table_almost_equal(starlist, test_starlist)
 
     def test_daogroup_six(self):
         """
              +------+----------+----------+----------+----------+------+
              |  *       *             *       *             *       *  |
              |                                                         |
          0.2 +                                                         +
@@ -208,144 +210,153 @@
              |                                                         |
         -0.2 +                                                         +
              |                                                         |
              |  *       *             *       *             *       *  |
              +------+----------+----------+----------+----------+------+
                     0          1          2          3          4
         """
-
-        x_0 = np.array([0, np.sqrt(2) / 4, np.sqrt(2) / 4, -np.sqrt(2) / 4,
-                        -np.sqrt(2) / 4])
-        y_0 = np.array([0, np.sqrt(2) / 4, -np.sqrt(2) / 4, np.sqrt(2) / 4,
-                        -np.sqrt(2) / 4])
-        x_1 = x_0 + 2.0
-        x_2 = x_0 + 4.0
-        first_group = Table([x_0, y_0, np.arange(5) + 1,
-                             np.ones(5, dtype=int)],
-                            names=('x_0', 'y_0', 'id', 'group_id'))
-        second_group = Table([x_1, y_0, 6 + np.arange(5),
-                              2 * np.ones(5, dtype=int)],
-                             names=('x_0', 'y_0', 'id', 'group_id'))
-        third_group = Table([x_2, y_0, 11 + np.arange(5),
-                             3 * np.ones(5, dtype=int)],
-                            names=('x_0', 'y_0', 'id', 'group_id'))
-        starlist = vstack([first_group, second_group, third_group])
-        daogroup = DAOGroup(crit_separation=0.6)
-        test_starlist = daogroup(starlist['x_0', 'y_0', 'id'])
-        assert_table_almost_equal(starlist, test_starlist)
+        with pytest.warns(AstropyDeprecationWarning):
+            x_0 = np.array([0, np.sqrt(2) / 4, np.sqrt(2) / 4, -np.sqrt(2) / 4,
+                            -np.sqrt(2) / 4])
+            y_0 = np.array([0, np.sqrt(2) / 4, -np.sqrt(2) / 4, np.sqrt(2) / 4,
+                            -np.sqrt(2) / 4])
+            x_1 = x_0 + 2.0
+            x_2 = x_0 + 4.0
+            first_group = Table([x_0, y_0, np.arange(5) + 1,
+                                 np.ones(5, dtype=int)],
+                                names=('x_0', 'y_0', 'id', 'group_id'))
+            second_group = Table([x_1, y_0, 6 + np.arange(5),
+                                  2 * np.ones(5, dtype=int)],
+                                 names=('x_0', 'y_0', 'id', 'group_id'))
+            third_group = Table([x_2, y_0, 11 + np.arange(5),
+                                 3 * np.ones(5, dtype=int)],
+                                names=('x_0', 'y_0', 'id', 'group_id'))
+            starlist = vstack([first_group, second_group, third_group])
+            daogroup = DAOGroup(crit_separation=0.6)
+            test_starlist = daogroup(starlist['x_0', 'y_0', 'id'])
+            assert_table_almost_equal(starlist, test_starlist)
 
     def test_isolated_sources(self):
         """
         Test case when all sources are isolated.
         """
-        x_0 = np.array([0, np.sqrt(2) / 4, np.sqrt(2) / 4, -np.sqrt(2) / 4,
-                        -np.sqrt(2) / 4])
-        y_0 = np.array([0, np.sqrt(2) / 4, -np.sqrt(2) / 4, np.sqrt(2) / 4,
-                        -np.sqrt(2) / 4])
-        starlist = Table([x_0, y_0, np.arange(len(x_0)) + 1,
-                          np.arange(len(x_0)) + 1],
-                         names=('x_0', 'y_0', 'id', 'group_id'))
-        daogroup = DAOGroup(crit_separation=0.01)
-        test_starlist = daogroup(starlist['x_0', 'y_0', 'id'])
-        assert_table_almost_equal(starlist, test_starlist)
+        with pytest.warns(AstropyDeprecationWarning):
+            x_0 = np.array([0, np.sqrt(2) / 4, np.sqrt(2) / 4, -np.sqrt(2) / 4,
+                            -np.sqrt(2) / 4])
+            y_0 = np.array([0, np.sqrt(2) / 4, -np.sqrt(2) / 4, np.sqrt(2) / 4,
+                            -np.sqrt(2) / 4])
+            starlist = Table([x_0, y_0, np.arange(len(x_0)) + 1,
+                              np.arange(len(x_0)) + 1],
+                             names=('x_0', 'y_0', 'id', 'group_id'))
+            daogroup = DAOGroup(crit_separation=0.01)
+            test_starlist = daogroup(starlist['x_0', 'y_0', 'id'])
+            assert_table_almost_equal(starlist, test_starlist)
 
     def test_id_column(self):
-        x_0 = np.array([0, np.sqrt(2) / 4, np.sqrt(2) / 4, -np.sqrt(2) / 4,
-                        -np.sqrt(2) / 4])
-        y_0 = np.array([0, np.sqrt(2) / 4, -np.sqrt(2) / 4, np.sqrt(2) / 4,
-                        -np.sqrt(2) / 4])
-        starlist = Table([x_0, y_0, np.arange(len(x_0)) + 1,
-                          np.arange(len(x_0)) + 1],
-                         names=('x_0', 'y_0', 'id', 'group_id'))
-        daogroup = DAOGroup(crit_separation=0.01)
-        test_starlist = daogroup(starlist['x_0', 'y_0'])
-        assert_table_almost_equal(starlist, test_starlist)
+        with pytest.warns(AstropyDeprecationWarning):
+            x_0 = np.array([0, np.sqrt(2) / 4, np.sqrt(2) / 4, -np.sqrt(2) / 4,
+                            -np.sqrt(2) / 4])
+            y_0 = np.array([0, np.sqrt(2) / 4, -np.sqrt(2) / 4, np.sqrt(2) / 4,
+                            -np.sqrt(2) / 4])
+            starlist = Table([x_0, y_0, np.arange(len(x_0)) + 1,
+                              np.arange(len(x_0)) + 1],
+                             names=('x_0', 'y_0', 'id', 'group_id'))
+            daogroup = DAOGroup(crit_separation=0.01)
+            test_starlist = daogroup(starlist['x_0', 'y_0'])
+            assert_table_almost_equal(starlist, test_starlist)
 
     def test_id_column_raise_error(self):
-        x_0 = np.array([0, np.sqrt(2) / 4, np.sqrt(2) / 4, -np.sqrt(2) / 4,
-                        -np.sqrt(2) / 4])
-        y_0 = np.array([0, np.sqrt(2) / 4, -np.sqrt(2) / 4, np.sqrt(2) / 4,
-                        -np.sqrt(2) / 4])
-        starlist = Table([x_0, y_0, np.arange(len(x_0)),
-                          np.arange(len(x_0)) + 1],
-                         names=('x_0', 'y_0', 'id', 'group_id'))
-        daogroup = DAOGroup(crit_separation=0.01)
-        with pytest.raises(ValueError):
-            daogroup(starlist['x_0', 'y_0', 'id'])
+        with pytest.warns(AstropyDeprecationWarning):
+            x_0 = np.array([0, np.sqrt(2) / 4, np.sqrt(2) / 4, -np.sqrt(2) / 4,
+                            -np.sqrt(2) / 4])
+            y_0 = np.array([0, np.sqrt(2) / 4, -np.sqrt(2) / 4, np.sqrt(2) / 4,
+                            -np.sqrt(2) / 4])
+            starlist = Table([x_0, y_0, np.arange(len(x_0)),
+                              np.arange(len(x_0)) + 1],
+                             names=('x_0', 'y_0', 'id', 'group_id'))
+            daogroup = DAOGroup(crit_separation=0.01)
+            with pytest.raises(ValueError):
+                daogroup(starlist['x_0', 'y_0', 'id'])
 
 
 @pytest.mark.skipif(not HAS_SKLEARN, reason='sklearn is required')
 class TestDBSCANGroup:
     def test_group_stars_one(self):
-        x_0 = np.array([0, np.sqrt(2) / 4, np.sqrt(2) / 4, -np.sqrt(2) / 4,
-                        -np.sqrt(2) / 4])
-        y_0 = np.array([0, np.sqrt(2) / 4, -np.sqrt(2) / 4, np.sqrt(2) / 4,
-                        -np.sqrt(2) / 4])
-        x_1 = x_0 + 2.0
-        first_group = Table([x_0, y_0, np.arange(len(x_0)) + 1,
-                            np.ones(len(x_0), dtype=int)],
-                            names=('x_0', 'y_0', 'id', 'group_id'))
-        second_group = Table([x_1, y_0, len(x_0) + np.arange(len(x_0)) + 1,
-                              2 * np.ones(len(x_0), dtype=int)],
-                             names=('x_0', 'y_0', 'id', 'group_id'))
-        starlist = vstack([first_group, second_group])
-        dbscan = DBSCANGroup(crit_separation=0.6)
-        test_starlist = dbscan(starlist['x_0', 'y_0', 'id'])
-        assert_table_almost_equal(starlist, test_starlist)
+        with pytest.warns(AstropyDeprecationWarning):
+            x_0 = np.array([0, np.sqrt(2) / 4, np.sqrt(2) / 4, -np.sqrt(2) / 4,
+                            -np.sqrt(2) / 4])
+            y_0 = np.array([0, np.sqrt(2) / 4, -np.sqrt(2) / 4, np.sqrt(2) / 4,
+                            -np.sqrt(2) / 4])
+            x_1 = x_0 + 2.0
+            first_group = Table([x_0, y_0, np.arange(len(x_0)) + 1,
+                                np.ones(len(x_0), dtype=int)],
+                                names=('x_0', 'y_0', 'id', 'group_id'))
+            second_group = Table([x_1, y_0, len(x_0) + np.arange(len(x_0)) + 1,
+                                  2 * np.ones(len(x_0), dtype=int)],
+                                 names=('x_0', 'y_0', 'id', 'group_id'))
+            starlist = vstack([first_group, second_group])
+            dbscan = DBSCANGroup(crit_separation=0.6)
+            test_starlist = dbscan(starlist['x_0', 'y_0', 'id'])
+            assert_table_almost_equal(starlist, test_starlist)
 
     def test_group_stars_two(self):
-        first_group = Table([1.5 * np.ones(5), np.linspace(0, 1, 5),
-                             np.arange(5) + 1, np.ones(5, dtype=int)],
-                            names=('x_0', 'y_0', 'id', 'group_id'))
-        second_group = Table([1.5 * np.ones(5), np.linspace(2, 3, 5),
-                              6 + np.arange(5), 2 * np.ones(5, dtype=int)],
-                             names=('x_0', 'y_0', 'id', 'group_id'))
-        third_group = Table([np.linspace(0, 1, 5), 1.5 * np.ones(5),
-                             11 + np.arange(5), 3 * np.ones(5, dtype=int)],
-                            names=('x_0', 'y_0', 'id', 'group_id'))
-        fourth_group = Table([np.linspace(2, 3, 5), 1.5 * np.ones(5),
-                              16 + np.arange(5), 4 * np.ones(5, dtype=int)],
-                             names=('x_0', 'y_0', 'id', 'group_id'))
-        starlist = vstack([first_group, second_group, third_group,
-                           fourth_group])
-        dbscan = DBSCANGroup(crit_separation=0.3)
-        test_starlist = dbscan(starlist['x_0', 'y_0', 'id'])
-        assert_table_almost_equal(starlist, test_starlist)
+        with pytest.warns(AstropyDeprecationWarning):
+            first_group = Table([1.5 * np.ones(5), np.linspace(0, 1, 5),
+                                 np.arange(5) + 1, np.ones(5, dtype=int)],
+                                names=('x_0', 'y_0', 'id', 'group_id'))
+            second_group = Table([1.5 * np.ones(5), np.linspace(2, 3, 5),
+                                  6 + np.arange(5), 2 * np.ones(5, dtype=int)],
+                                 names=('x_0', 'y_0', 'id', 'group_id'))
+            third_group = Table([np.linspace(0, 1, 5), 1.5 * np.ones(5),
+                                 11 + np.arange(5), 3 * np.ones(5, dtype=int)],
+                                names=('x_0', 'y_0', 'id', 'group_id'))
+            fourth_group = Table([np.linspace(2, 3, 5), 1.5 * np.ones(5),
+                                  16 + np.arange(5),
+                                  4 * np.ones(5, dtype=int)],
+                                 names=('x_0', 'y_0', 'id', 'group_id'))
+            starlist = vstack([first_group, second_group, third_group,
+                               fourth_group])
+            dbscan = DBSCANGroup(crit_separation=0.3)
+            test_starlist = dbscan(starlist['x_0', 'y_0', 'id'])
+            assert_table_almost_equal(starlist, test_starlist)
 
     def test_isolated_sources(self):
         """
         Test case when all sources are isolated.
         """
-        x_0 = np.array([0, np.sqrt(2) / 4, np.sqrt(2) / 4, -np.sqrt(2) / 4,
-                        -np.sqrt(2) / 4])
-        y_0 = np.array([0, np.sqrt(2) / 4, -np.sqrt(2) / 4, np.sqrt(2) / 4,
-                        -np.sqrt(2) / 4])
-        starlist = Table([x_0, y_0, np.arange(len(x_0)) + 1,
-                          np.arange(len(x_0)) + 1],
-                         names=('x_0', 'y_0', 'id', 'group_id'))
-        dbscan = DBSCANGroup(crit_separation=0.01)
-        test_starlist = dbscan(starlist['x_0', 'y_0', 'id'])
-        assert_table_almost_equal(starlist, test_starlist)
+        with pytest.warns(AstropyDeprecationWarning):
+            x_0 = np.array([0, np.sqrt(2) / 4, np.sqrt(2) / 4, -np.sqrt(2) / 4,
+                            -np.sqrt(2) / 4])
+            y_0 = np.array([0, np.sqrt(2) / 4, -np.sqrt(2) / 4, np.sqrt(2) / 4,
+                            -np.sqrt(2) / 4])
+            starlist = Table([x_0, y_0, np.arange(len(x_0)) + 1,
+                              np.arange(len(x_0)) + 1],
+                             names=('x_0', 'y_0', 'id', 'group_id'))
+            dbscan = DBSCANGroup(crit_separation=0.01)
+            test_starlist = dbscan(starlist['x_0', 'y_0', 'id'])
+            assert_table_almost_equal(starlist, test_starlist)
 
     def test_id_column(self):
-        x_0 = np.array([0, np.sqrt(2) / 4, np.sqrt(2) / 4, -np.sqrt(2) / 4,
-                        -np.sqrt(2) / 4])
-        y_0 = np.array([0, np.sqrt(2) / 4, -np.sqrt(2) / 4, np.sqrt(2) / 4,
-                        -np.sqrt(2) / 4])
-        starlist = Table([x_0, y_0, np.arange(len(x_0)) + 1,
-                          np.arange(len(x_0)) + 1],
-                         names=('x_0', 'y_0', 'id', 'group_id'))
-        dbscan = DBSCANGroup(crit_separation=0.01)
-        test_starlist = dbscan(starlist['x_0', 'y_0'])
-        assert_table_almost_equal(starlist, test_starlist)
+        with pytest.warns(AstropyDeprecationWarning):
+            x_0 = np.array([0, np.sqrt(2) / 4, np.sqrt(2) / 4, -np.sqrt(2) / 4,
+                            -np.sqrt(2) / 4])
+            y_0 = np.array([0, np.sqrt(2) / 4, -np.sqrt(2) / 4, np.sqrt(2) / 4,
+                            -np.sqrt(2) / 4])
+            starlist = Table([x_0, y_0, np.arange(len(x_0)) + 1,
+                              np.arange(len(x_0)) + 1],
+                             names=('x_0', 'y_0', 'id', 'group_id'))
+            dbscan = DBSCANGroup(crit_separation=0.01)
+            test_starlist = dbscan(starlist['x_0', 'y_0'])
+            assert_table_almost_equal(starlist, test_starlist)
 
     def test_id_column_raise_error(self):
-        x_0 = np.array([0, np.sqrt(2) / 4, np.sqrt(2) / 4, -np.sqrt(2) / 4,
-                        -np.sqrt(2) / 4])
-        y_0 = np.array([0, np.sqrt(2) / 4, -np.sqrt(2) / 4, np.sqrt(2) / 4,
-                        -np.sqrt(2) / 4])
-        starlist = Table([x_0, y_0, np.arange(len(x_0)),
-                          np.arange(len(x_0)) + 1],
-                         names=('x_0', 'y_0', 'id', 'group_id'))
-        dbscan = DBSCANGroup(crit_separation=0.01)
-        with pytest.raises(ValueError):
-            dbscan(starlist['x_0', 'y_0', 'id'])
+        with pytest.warns(AstropyDeprecationWarning):
+            x_0 = np.array([0, np.sqrt(2) / 4, np.sqrt(2) / 4, -np.sqrt(2) / 4,
+                            -np.sqrt(2) / 4])
+            y_0 = np.array([0, np.sqrt(2) / 4, -np.sqrt(2) / 4, np.sqrt(2) / 4,
+                            -np.sqrt(2) / 4])
+            starlist = Table([x_0, y_0, np.arange(len(x_0)),
+                              np.arange(len(x_0)) + 1],
+                             names=('x_0', 'y_0', 'id', 'group_id'))
+            dbscan = DBSCANGroup(crit_separation=0.01)
+            with pytest.raises(ValueError):
+                dbscan(starlist['x_0', 'y_0', 'id'])
```

### Comparing `photutils-1.8.0/photutils/psf/tests/test_photometry.py` & `photutils-1.9.0/photutils/psf/tests/test_photometry-depr.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,74 +1,79 @@
 # Licensed under a 3-clause BSD style license - see LICENSE.rst
 """
 Tests for the photometry module.
 """
 
+from contextlib import nullcontext
+
+import astropy
 import numpy as np
 import pytest
 from astropy.convolution.utils import discretize_model
 from astropy.modeling import Fittable2DModel, Parameter
 from astropy.modeling.fitting import LevMarLSQFitter, SimplexLSQFitter
 from astropy.modeling.models import Gaussian2D, Moffat2D
 from astropy.stats import SigmaClip, gaussian_sigma_to_fwhm
 from astropy.table import Table
-from astropy.utils.exceptions import AstropyUserWarning
+from astropy.utils import minversion
+from astropy.utils.exceptions import (AstropyDeprecationWarning,
+                                      AstropyUserWarning)
 from numpy.testing import assert_allclose, assert_array_equal, assert_equal
 
 from photutils.background import MMMBackground, StdBackgroundRMS
 from photutils.datasets import (make_gaussian_prf_sources_image,
                                 make_noise_image)
 from photutils.detection import DAOStarFinder, IRAFStarFinder
 from photutils.psf.groupstars import DAOGroup
 from photutils.psf.models import FittableImageModel, IntegratedGaussianPRF
-from photutils.psf.photometry import (BasicPSFPhotometry, DAOPhotPSFPhotometry,
-                                      IterativelySubtractedPSFPhotometry)
+from photutils.psf.photometry_depr import (BasicPSFPhotometry,
+                                           DAOPhotPSFPhotometry,
+                                           IterativelySubtractedPSFPhotometry)
 from photutils.psf.utils import prepare_psf_model
+from photutils.tests.helper import PYTEST_LT_80
 from photutils.utils._optional_deps import HAS_SCIPY
 
 
 def make_psf_photometry_objs(std=1, sigma_psf=1):
     """
     Produces baseline photometry objects which are then
     modified as-needed in specific tests below
     """
+    with pytest.warns(AstropyDeprecationWarning):
+        daofind = DAOStarFinder(threshold=5.0 * std,
+                                fwhm=sigma_psf * gaussian_sigma_to_fwhm)
+        daogroup = DAOGroup(1.5 * sigma_psf * gaussian_sigma_to_fwhm)
+        threshold = 5.0 * std
+        fwhm = sigma_psf * gaussian_sigma_to_fwhm
+        crit_separation = 1.5 * sigma_psf * gaussian_sigma_to_fwhm
+
+        daofind = DAOStarFinder(threshold=threshold, fwhm=fwhm)
+        daogroup = DAOGroup(crit_separation)
+        mode_bkg = MMMBackground()
+        psf_model = IntegratedGaussianPRF(sigma=sigma_psf)
+        fitter = LevMarLSQFitter()
+
+        basic_phot_obj = BasicPSFPhotometry(finder=daofind,
+                                            group_maker=daogroup,
+                                            bkg_estimator=mode_bkg,
+                                            psf_model=psf_model,
+                                            fitter=fitter,
+                                            fitshape=(11, 11))
+
+        iter_phot_obj = IterativelySubtractedPSFPhotometry(
+            finder=daofind, group_maker=daogroup, bkg_estimator=mode_bkg,
+            psf_model=psf_model, fitter=fitter, niters=1, fitshape=(11, 11))
 
-    daofind = DAOStarFinder(threshold=5.0 * std,
-                            fwhm=sigma_psf * gaussian_sigma_to_fwhm)
-    daogroup = DAOGroup(1.5 * sigma_psf * gaussian_sigma_to_fwhm)
-    threshold = 5.0 * std
-    fwhm = sigma_psf * gaussian_sigma_to_fwhm
-    crit_separation = 1.5 * sigma_psf * gaussian_sigma_to_fwhm
-
-    daofind = DAOStarFinder(threshold=threshold, fwhm=fwhm)
-    daogroup = DAOGroup(crit_separation)
-    mode_bkg = MMMBackground()
-    psf_model = IntegratedGaussianPRF(sigma=sigma_psf)
-    fitter = LevMarLSQFitter()
-
-    basic_phot_obj = BasicPSFPhotometry(finder=daofind,
-                                        group_maker=daogroup,
-                                        bkg_estimator=mode_bkg,
-                                        psf_model=psf_model,
-                                        fitter=fitter,
-                                        fitshape=(11, 11))
-
-    iter_phot_obj = IterativelySubtractedPSFPhotometry(finder=daofind,
-                                                       group_maker=daogroup,
-                                                       bkg_estimator=mode_bkg,
-                                                       psf_model=psf_model,
-                                                       fitter=fitter, niters=1,
-                                                       fitshape=(11, 11))
-
-    dao_phot_obj = DAOPhotPSFPhotometry(crit_separation=crit_separation,
-                                        threshold=threshold, fwhm=fwhm,
-                                        psf_model=psf_model, fitshape=(11, 11),
-                                        niters=1)
+        dao_phot_obj = DAOPhotPSFPhotometry(crit_separation=crit_separation,
+                                            threshold=threshold, fwhm=fwhm,
+                                            psf_model=psf_model,
+                                            fitshape=(11, 11),
+                                            niters=1)
 
-    return (basic_phot_obj, iter_phot_obj, dao_phot_obj)
+        return (basic_phot_obj, iter_phot_obj, dao_phot_obj)
 
 
 sigma_psfs = []
 
 # A group of two overlapped stars and an isolated one
 sigma_psfs.append(2)
 sources1 = Table()
@@ -124,16 +129,17 @@
     bkgrms = StdBackgroundRMS(sigma_clip)
     std = bkgrms(image)
 
     phot_obj = make_psf_photometry_objs(std, sigma_psf)[1:3]
     for iter_phot_obj in phot_obj:
         iter_phot_obj.niters = None
 
-        result_tab = iter_phot_obj(image)
-        residual_image = iter_phot_obj.get_residual_image()
+        with pytest.warns(AstropyDeprecationWarning):
+            result_tab = iter_phot_obj(image)
+            residual_image = iter_phot_obj.get_residual_image()
 
         assert (result_tab['x_0_unc'] < 1.96 * sigma_psf
                 / np.sqrt(sources['flux'])).all()
         assert (result_tab['y_0_unc'] < 1.96 * sigma_psf
                 / np.sqrt(sources['flux'])).all()
         assert (result_tab['flux_unc'] < 1.96
                 * np.sqrt(sources['flux'])).all()
@@ -176,16 +182,17 @@
 
     sigma_clip = SigmaClip(sigma=3.0)
     bkgrms = StdBackgroundRMS(sigma_clip)
     std = bkgrms(image)
     phot_objs = make_psf_photometry_objs(std, sigma_psf)
 
     for phot_proc in phot_objs:
-        result_tab = phot_proc(image)
-        residual_image = phot_proc.get_residual_image()
+        with pytest.warns(AstropyDeprecationWarning):
+            result_tab = phot_proc(image)
+            residual_image = phot_proc.get_residual_image()
         assert (result_tab['x_0_unc'] < 1.96 * sigma_psf
                 / np.sqrt(sources['flux'])).all()
         assert (result_tab['y_0_unc'] < 1.96 * sigma_psf
                 / np.sqrt(sources['flux'])).all()
         assert (result_tab['flux_unc'] < 1.96
                 * np.sqrt(sources['flux'])).all()
         assert_allclose(result_tab['x_fit'], sources['x_0'], rtol=1e-1)
@@ -199,16 +206,17 @@
         phot_proc.psf_model.x_0.fixed = True
         phot_proc.psf_model.y_0.fixed = True
 
         pos = Table(names=['x_0', 'y_0'], data=[sources['x_0'],
                                                 sources['y_0']])
         cp_pos = pos.copy()
 
-        result_tab = phot_proc(image, init_guesses=pos)
-        residual_image = phot_proc.get_residual_image()
+        with pytest.warns(AstropyDeprecationWarning):
+            result_tab = phot_proc(image, init_guesses=pos)
+            residual_image = phot_proc.get_residual_image()
         assert 'x_0_unc' not in result_tab.colnames
         assert 'y_0_unc' not in result_tab.colnames
         assert (result_tab['flux_unc'] < 1.96
                 * np.sqrt(sources['flux'])).all()
         assert_array_equal(result_tab['x_fit'], sources['x_0'])
         assert_array_equal(result_tab['y_fit'], sources['y_0'])
         assert_allclose(result_tab['flux_fit'], sources['flux'], rtol=1e-1)
@@ -280,44 +288,50 @@
     # test that a ValueError is raised if aperture_radius is non positive
     with pytest.raises(ValueError):
         basic_phot_obj.aperture_radius = -3
 
 
 @pytest.mark.skipif(not HAS_SCIPY, reason='scipy is required')
 def test_finder_errors():
-    iter_phot_obj = make_psf_photometry_objs()[1]
+    with pytest.warns(AstropyDeprecationWarning):
+        iter_phot_obj = make_psf_photometry_objs()[1]
 
-    with pytest.raises(ValueError):
-        iter_phot_obj.finder = None
+        with pytest.raises(ValueError):
+            iter_phot_obj.finder = None
 
-    with pytest.raises(ValueError):
-        iter_phot_obj = IterativelySubtractedPSFPhotometry(
-            finder=None, group_maker=DAOGroup(1),
-            bkg_estimator=MMMBackground(),
-            psf_model=IntegratedGaussianPRF(1), fitshape=(11, 11))
+        with pytest.raises(ValueError):
+            iter_phot_obj = IterativelySubtractedPSFPhotometry(
+                finder=None, group_maker=DAOGroup(1),
+                bkg_estimator=MMMBackground(),
+                psf_model=IntegratedGaussianPRF(1), fitshape=(11, 11))
 
 
 @pytest.mark.skipif(not HAS_SCIPY, reason='scipy is required')
 def test_finder_positions_warning():
     basic_phot_obj = make_psf_photometry_objs(sigma_psf=2)[0]
     positions = Table()
     positions['x_0'] = [12.8, 18.2, 25.3]
     positions['y_0'] = [15.7, 16.5, 25.1]
 
     image = (make_gaussian_prf_sources_image((32, 32), sources1)
              + make_noise_image((32, 32), distribution='poisson', mean=6.0,
                                 seed=0))
 
-    with pytest.warns(AstropyUserWarning, match='Both init_guesses and '
-                      'finder are different than None'):
+    match = 'Both init_guesses and finder are different than None'
+    ctx1 = pytest.warns(AstropyUserWarning, match=match)
+    if PYTEST_LT_80:
+        ctx2 = nullcontext()
+    else:
+        ctx2 = pytest.warns(AstropyDeprecationWarning)
+    with ctx1, ctx2:
         result_tab = basic_phot_obj(image=image, init_guesses=positions)
-    assert_array_equal(result_tab['x_0'], positions['x_0'])
-    assert_array_equal(result_tab['y_0'], positions['y_0'])
-    assert_allclose(result_tab['x_fit'], positions['x_0'], rtol=1e-1)
-    assert_allclose(result_tab['y_fit'], positions['y_0'], rtol=1e-1)
+        assert_array_equal(result_tab['x_0'], positions['x_0'])
+        assert_array_equal(result_tab['y_0'], positions['y_0'])
+        assert_allclose(result_tab['x_fit'], positions['x_0'], rtol=1e-1)
+        assert_allclose(result_tab['y_fit'], positions['y_0'], rtol=1e-1)
 
     basic_phot_obj.finder = None
     with pytest.raises(ValueError):
         result_tab = basic_phot_obj(image=image)
 
 
 @pytest.mark.filterwarnings('ignore:The fit may be unsuccessful')
@@ -347,15 +361,16 @@
             super().__init__(fwhm=fwhm)
 
         def evaluate(self, x, y, x_0, y_0, flux, fwhm):
             return flux / (fwhm * (x - x_0)**2 * (y - y_0)**2)
 
     psf_model = PSFModelWithFWHM()
     basic_phot_obj.psf_model = psf_model
-    basic_phot_obj(image)
+    with pytest.warns(AstropyDeprecationWarning):
+        basic_phot_obj(image)
     assert_equal(basic_phot_obj.aperture_radius, psf_model.fwhm.value)
 
 
 PARS_TO_SET_0 = {'x_0': 'x_0', 'y_0': 'y_0', 'flux_0': 'flux'}
 PARS_TO_OUTPUT_0 = {'x_fit': 'x_0', 'y_fit': 'y_0', 'flux_fit': 'flux'}
 PARS_TO_SET_1 = PARS_TO_SET_0.copy()
 PARS_TO_SET_1['sigma_0'] = 'sigma'
@@ -373,15 +388,16 @@
                                 is_sigma_fixed):
     psf_model = IntegratedGaussianPRF()
     psf_model.sigma.fixed = is_sigma_fixed
 
     basic_phot_obj = make_psf_photometry_objs()[0]
     basic_phot_obj.psf_model = psf_model
 
-    basic_phot_obj._define_fit_param_names()
+    with pytest.warns(AstropyDeprecationWarning):
+        basic_phot_obj._define_fit_param_names()
     assert_equal(basic_phot_obj._pars_to_set, actual_pars_to_set)
     assert_equal(basic_phot_obj._pars_to_output, actual_pars_to_output)
 
 
 # tests previously written to psf_photometry
 
 PSF_SIZE = 11
@@ -440,219 +456,236 @@
             x = np.mean(xs)
             y = np.mean(ys)
             table.add_row([int(n + 1), x, y, f * 9])
         table.sort(['flux'])
 
         return table
 
-    prf = np.zeros((7, 7), float)
-    prf[2:5, 2:5] = 1 / 9
-    prf = FittableImageModel(prf)
-
-    img = np.zeros((50, 50), float)
-    x0 = [38, 20, 35]
-    y0 = [20, 5, 40]
-    f0 = [50, 100, 200]
-    for x, y, f in zip(x0, y0, f0):
-        img[y - 1:y + 2, x - 1:x + 2] = f / 9
-
-    intab = Table(data=[[37, 19.6, 34.9], [19.6, 4.5, 40.1]],
-                  names=['x_0', 'y_0'])
-
-    basic_phot = BasicPSFPhotometry(group_maker=DAOGroup(2),
-                                    bkg_estimator=None, psf_model=prf,
-                                    fitshape=7, finder=tophatfinder)
-    # Test for init_guesses is None
-    with pytest.warns(AstropyUserWarning, match='aperture_radius is None and '
-                                                'could not be determined'):
-        results = basic_phot(image=img)
-    assert_allclose(results['flux_fit'], f0, rtol=0.05)
-
-    # Have to reset the object or it saves any updates, and we wish to
-    # re-verify the aperture_radius assignment
-    basic_phot = BasicPSFPhotometry(group_maker=DAOGroup(2),
-                                    bkg_estimator=None, psf_model=prf,
-                                    fitshape=7)
-
-    # Test for init_guesses is not None, but lacks a flux_0 column
-    with pytest.warns(AstropyUserWarning, match='aperture_radius is None and '
-                                                'could not be determined'):
-        results = basic_phot(image=img, init_guesses=intab)
-    assert_allclose(results['flux_fit'], f0, rtol=0.05)
-
-    iter_phot = IterativelySubtractedPSFPhotometry(finder=tophatfinder,
-                                                   group_maker=DAOGroup(2),
-                                                   bkg_estimator=None,
-                                                   psf_model=prf,
-                                                   fitshape=7, niters=2)
-    # Test for init_guesses is not None, but lacks a flux_0 column
-    with pytest.warns(AstropyUserWarning, match='aperture_radius is None and '
-                                                'could not be determined'):
-        results = iter_phot(image=img, init_guesses=intab)
-    assert_allclose(results['flux_fit'], f0, rtol=0.05)
-
-    iter_phot = IterativelySubtractedPSFPhotometry(finder=tophatfinder,
-                                                   group_maker=DAOGroup(2),
-                                                   bkg_estimator=None,
-                                                   psf_model=prf,
-                                                   fitshape=7, niters=2)
-
-    # Test for init_guesses is None
-    with pytest.warns(AstropyUserWarning, match='aperture_radius is None and '
-                                                'could not be determined'):
-        results = iter_phot(image=img)
-    assert_allclose(results['flux_fit'], f0, rtol=0.05)
+    with pytest.warns(AstropyDeprecationWarning):
+        prf = np.zeros((7, 7), float)
+        prf[2:5, 2:5] = 1 / 9
+        prf = FittableImageModel(prf)
+
+        img = np.zeros((50, 50), float)
+        x0 = [38, 20, 35]
+        y0 = [20, 5, 40]
+        f0 = [50, 100, 200]
+        for x, y, f in zip(x0, y0, f0):
+            img[y - 1:y + 2, x - 1:x + 2] = f / 9
+
+        intab = Table(data=[[37, 19.6, 34.9], [19.6, 4.5, 40.1]],
+                      names=['x_0', 'y_0'])
+
+        basic_phot = BasicPSFPhotometry(group_maker=DAOGroup(2),
+                                        bkg_estimator=None, psf_model=prf,
+                                        fitshape=7, finder=tophatfinder)
+        # Test for init_guesses is None
+        match = 'aperture_radius is None and could not be determined'
+        with pytest.warns(AstropyUserWarning, match=match):
+            results = basic_phot(image=img)
+        assert_allclose(results['flux_fit'], f0, rtol=0.05)
+
+        # Have to reset the object or it saves any updates, and we wish to
+        # re-verify the aperture_radius assignment
+        basic_phot = BasicPSFPhotometry(group_maker=DAOGroup(2),
+                                        bkg_estimator=None, psf_model=prf,
+                                        fitshape=7)
+
+        # Test for init_guesses is not None, but lacks a flux_0 column
+        match = 'aperture_radius is None and could not be determined'
+        with pytest.warns(AstropyUserWarning, match=match):
+            results = basic_phot(image=img, init_guesses=intab)
+        assert_allclose(results['flux_fit'], f0, rtol=0.05)
+
+        iter_phot = IterativelySubtractedPSFPhotometry(finder=tophatfinder,
+                                                       group_maker=DAOGroup(2),
+                                                       bkg_estimator=None,
+                                                       psf_model=prf,
+                                                       fitshape=7, niters=2)
+
+        match1 = 'aperture_radius is None and could not be determined'
+        ctx1 = pytest.warns(AstropyUserWarning, match=match1)
+        if PYTEST_LT_80:
+            ctx2 = nullcontext()
+        else:
+            match2 = 'Both init_guesses and finder are different than None'
+            ctx2 = pytest.warns(AstropyUserWarning, match=match2)
+        with ctx1, ctx2:
+            results = iter_phot(image=img, init_guesses=intab)
+            assert_allclose(results['flux_fit'], f0, rtol=0.05)
+
+        iter_phot = IterativelySubtractedPSFPhotometry(
+            finder=tophatfinder, group_maker=DAOGroup(2), bkg_estimator=None,
+            psf_model=prf, fitshape=7, niters=2)
+
+        # Test for init_guesses is None
+        match = 'aperture_radius is None and could not be determined'
+        with pytest.warns(AstropyUserWarning, match=match):
+            results = iter_phot(image=img)
+        assert_allclose(results['flux_fit'], f0, rtol=0.05)
 
 
 @pytest.mark.skipif(not HAS_SCIPY, reason='scipy is required')
 def test_psf_boundary_gaussian():
     """
     Test psf_photometry with discrete PRF model at the boundary of the data.
     """
-    psf = IntegratedGaussianPRF(GAUSSIAN_WIDTH)
+    with pytest.warns(AstropyDeprecationWarning):
+        psf = IntegratedGaussianPRF(GAUSSIAN_WIDTH)
 
-    basic_phot = BasicPSFPhotometry(group_maker=DAOGroup(2),
-                                    bkg_estimator=None, psf_model=psf,
-                                    fitshape=7)
-
-    intab = Table(data=[[1], [1]], names=['x_0', 'y_0'])
-    f = basic_phot(image=image, init_guesses=intab)
-    assert_allclose(f['flux_fit'], 0, atol=1e-8)
+        basic_phot = BasicPSFPhotometry(group_maker=DAOGroup(2),
+                                        bkg_estimator=None, psf_model=psf,
+                                        fitshape=7)
+
+        intab = Table(data=[[1], [1]], names=['x_0', 'y_0'])
+        f = basic_phot(image=image, init_guesses=intab)
+        assert_allclose(f['flux_fit'], 0, atol=1e-8)
 
 
 @pytest.mark.skipif(not HAS_SCIPY, reason='scipy is required')
 def test_psf_photometry_gaussian():
     """
     Test psf_photometry with Gaussian PSF model.
     """
-    psf = IntegratedGaussianPRF(sigma=GAUSSIAN_WIDTH)
+    with pytest.warns(AstropyDeprecationWarning):
+        psf = IntegratedGaussianPRF(sigma=GAUSSIAN_WIDTH)
 
-    basic_phot = BasicPSFPhotometry(group_maker=DAOGroup(2),
-                                    bkg_estimator=None, psf_model=psf,
-                                    fitshape=7)
-    f = basic_phot(image=image, init_guesses=INTAB)
-    for n in ['x', 'y', 'flux']:
-        assert_allclose(f[n + '_0'], f[n + '_fit'], rtol=1e-3)
+        basic_phot = BasicPSFPhotometry(group_maker=DAOGroup(2),
+                                        bkg_estimator=None, psf_model=psf,
+                                        fitshape=7)
+        f = basic_phot(image=image, init_guesses=INTAB)
+        for n in ['x', 'y', 'flux']:
+            assert_allclose(f[n + '_0'], f[n + '_fit'], rtol=1e-3)
 
 
 @pytest.mark.skipif(not HAS_SCIPY, reason='scipy is required')
 @pytest.mark.parametrize("renormalize_psf", (True, False))
 def test_psf_photometry_gaussian2(renormalize_psf):
     """
     Test psf_photometry with Gaussian PSF model from Astropy.
     """
-    psf = Gaussian2D(1.0 / (2 * np.pi * GAUSSIAN_WIDTH ** 2), PSF_SIZE // 2,
-                     PSF_SIZE // 2, GAUSSIAN_WIDTH, GAUSSIAN_WIDTH)
-    psf = prepare_psf_model(psf, xname='x_mean', yname='y_mean',
-                            renormalize_psf=renormalize_psf)
-
-    basic_phot = BasicPSFPhotometry(group_maker=DAOGroup(2),
-                                    bkg_estimator=None, psf_model=psf,
-                                    fitshape=7)
-    with pytest.warns(AstropyUserWarning, match='aperture_radius is None and '
-                      'could not be determined by psf_model'):
-        f = basic_phot(image=image, init_guesses=INTAB)
-
-    for n in ['x', 'y']:
-        assert_allclose(f[n + '_0'], f[n + '_fit'], rtol=1e-1)
-    assert_allclose(f['flux_0'], f['flux_fit'], rtol=1e-1)
+    with pytest.warns(AstropyDeprecationWarning):
+        psf = Gaussian2D(1.0 / (2 * np.pi * GAUSSIAN_WIDTH ** 2),
+                         PSF_SIZE // 2, PSF_SIZE // 2, GAUSSIAN_WIDTH,
+                         GAUSSIAN_WIDTH)
+        psf = prepare_psf_model(psf, xname='x_mean', yname='y_mean',
+                                renormalize_psf=renormalize_psf)
+
+        basic_phot = BasicPSFPhotometry(group_maker=DAOGroup(2),
+                                        bkg_estimator=None, psf_model=psf,
+                                        fitshape=7)
+        match = ('aperture_radius is None and could not be determined by '
+                 'psf_model')
+        with pytest.warns(AstropyUserWarning, match=match):
+            f = basic_phot(image=image, init_guesses=INTAB)
+
+        for n in ['x', 'y']:
+            assert_allclose(f[n + '_0'], f[n + '_fit'], rtol=1e-1)
+        assert_allclose(f['flux_0'], f['flux_fit'], rtol=1e-1)
 
 
 @pytest.mark.skipif(not HAS_SCIPY, reason='scipy is required')
 def test_psf_photometry_moffat():
     """
     Test psf_photometry with Moffat PSF model from Astropy.
     """
-    psf = Moffat2D(1.0 / (2 * np.pi * GAUSSIAN_WIDTH ** 2), PSF_SIZE // 2,
-                   PSF_SIZE // 2, 1, 1)
-    psf = prepare_psf_model(psf, xname='x_0', yname='y_0',
-                            renormalize_psf=False)
-
-    basic_phot = BasicPSFPhotometry(group_maker=DAOGroup(2),
-                                    bkg_estimator=None, psf_model=psf,
-                                    fitshape=7)
-    with pytest.warns(AstropyUserWarning, match='aperture_radius is None and '
-                      'could not be determined by psf_model'):
-        f = basic_phot(image=image, init_guesses=INTAB)
-    f.pprint(max_width=-1)
-
-    for n in ['x', 'y']:
-        assert_allclose(f[n + '_0'], f[n + '_fit'], rtol=1e-3)
-    # image was created with a gaussian, so flux won't match exactly
-    assert_allclose(f['flux_0'], f['flux_fit'], rtol=1e-1)
+    with pytest.warns(AstropyDeprecationWarning):
+        psf = Moffat2D(1.0 / (2 * np.pi * GAUSSIAN_WIDTH ** 2), PSF_SIZE // 2,
+                       PSF_SIZE // 2, 1, 1)
+        psf = prepare_psf_model(psf, xname='x_0', yname='y_0',
+                                renormalize_psf=False)
+
+        basic_phot = BasicPSFPhotometry(group_maker=DAOGroup(2),
+                                        bkg_estimator=None, psf_model=psf,
+                                        fitshape=7)
+        match = ('aperture_radius is None and could not be determined by '
+                 'psf_model')
+        with pytest.warns(AstropyUserWarning, match=match):
+            f = basic_phot(image=image, init_guesses=INTAB)
+        f.pprint(max_width=-1)
+
+        for n in ['x', 'y']:
+            assert_allclose(f[n + '_0'], f[n + '_fit'], rtol=1e-3)
+        # image was created with a gaussian, so flux won't match exactly
+        assert_allclose(f['flux_0'], f['flux_fit'], rtol=1e-1)
 
 
 @pytest.mark.skipif(not HAS_SCIPY, reason='scipy is required')
 def test_psf_fitting_data_on_edge():
     """
     No mask is input explicitly here, but source 2 is so close to the
     edge that the subarray that's extracted gets a mask internally.
     """
-    psf_guess = IntegratedGaussianPRF(flux=1, sigma=WIDE_GAUSSIAN_WIDTH)
-    psf_guess.flux.fixed = psf_guess.x_0.fixed = psf_guess.y_0.fixed = False
-    basic_phot = BasicPSFPhotometry(group_maker=DAOGroup(2),
-                                    bkg_estimator=None, psf_model=psf_guess,
-                                    fitshape=7)
-
-    outtab = basic_phot(image=wide_image, init_guesses=WIDE_INTAB)
-
-    for n in ['x', 'y', 'flux']:
-        assert_allclose(outtab[n + '_0'], outtab[n + '_fit'],
-                        rtol=0.05, atol=0.1)
+    with pytest.warns(AstropyDeprecationWarning):
+        psf_guess = IntegratedGaussianPRF(flux=1, sigma=WIDE_GAUSSIAN_WIDTH)
+        psf_guess.flux.fixed = psf_guess.x_0.fixed = False
+        psf_guess.y_0.fixed = False
+        basic_phot = BasicPSFPhotometry(group_maker=DAOGroup(2),
+                                        bkg_estimator=None,
+                                        psf_model=psf_guess, fitshape=7)
+
+        outtab = basic_phot(image=wide_image, init_guesses=WIDE_INTAB)
+
+        for n in ['x', 'y', 'flux']:
+            assert_allclose(outtab[n + '_0'], outtab[n + '_fit'],
+                            rtol=0.05, atol=0.1)
 
 
 @pytest.mark.filterwarnings('ignore:Both init_guesses and finder '
                             'are different than None')
 @pytest.mark.skipif(not HAS_SCIPY, reason='scipy is required')
 @pytest.mark.parametrize("sigma_psf, sources", [(sigma_psfs[2], sources3)])
 def test_psf_extra_output_cols(sigma_psf, sources):
     """
     Test the handling of a non-None extra_output_cols
     """
-    psf_model = IntegratedGaussianPRF(sigma=sigma_psf)
-    tshape = (32, 32)
-    image = (make_gaussian_prf_sources_image(tshape, sources)
-             + make_noise_image(tshape, distribution='poisson', mean=6.0,
-                                seed=0)
-             + make_noise_image(tshape, distribution='gaussian', mean=0.0,
-                                stddev=2.0, seed=0))
-
-    init_guess1 = None
-    init_guess2 = Table(names=['x_0', 'y_0', 'sharpness', 'roundness1',
-                               'roundness2'],
-                        data=[[17.4], [16], [0.4], [0], [0]])
-    init_guess3 = Table(names=['x_0', 'y_0'],
-                        data=[[17.4], [16]])
-    init_guess4 = Table(names=['x_0', 'y_0', 'sharpness'],
-                        data=[[17.4], [16], [0.4]])
-    for i, init_guesses in enumerate([init_guess1, init_guess2, init_guess3,
-                                      init_guess4]):
-        dao_phot = DAOPhotPSFPhotometry(crit_separation=8, threshold=40,
-                                        fwhm=4 * np.sqrt(2 * np.log(2)),
-                                        psf_model=psf_model, fitshape=(11, 11),
-                                        extra_output_cols=['sharpness',
-                                                           'roundness1',
-                                                           'roundness2'])
-        phot_results = dao_phot(image, init_guesses=init_guesses)
-        # test that the original required columns are also passed back, as well
-        # as extra_output_cols
-        assert np.all([name in phot_results.colnames for name in
-                       ['x_0', 'y_0']])
-        assert np.all([name in phot_results.colnames for name in
-                       ['sharpness', 'roundness1', 'roundness2']])
-        assert len(phot_results) == 2
-        # checks to verify that half-passing init_guesses results in NaN output
-        # for extra_output_cols not passed as initial guesses
-        if i == 2:  # init_guess3
-            assert np.all(np.all(np.isnan(phot_results[o])) for o in
-                          ['sharpness', 'roundness1', 'roundness2'])
-        if i == 3:  # init_guess4
-            assert np.all(np.all(np.isnan(phot_results[o])) for o in
-                          ['roundness1', 'roundness2'])
-            assert np.all(~np.isnan(phot_results['sharpness']))
+    with pytest.warns(AstropyDeprecationWarning):
+        psf_model = IntegratedGaussianPRF(sigma=sigma_psf)
+        tshape = (32, 32)
+        image = (make_gaussian_prf_sources_image(tshape, sources)
+                 + make_noise_image(tshape, distribution='poisson', mean=6.0,
+                                    seed=0)
+                 + make_noise_image(tshape, distribution='gaussian', mean=0.0,
+                                    stddev=2.0, seed=0))
+
+        init_guess1 = None
+        init_guess2 = Table(names=['x_0', 'y_0', 'sharpness', 'roundness1',
+                                   'roundness2'],
+                            data=[[17.4], [16], [0.4], [0], [0]])
+        init_guess3 = Table(names=['x_0', 'y_0'],
+                            data=[[17.4], [16]])
+        init_guess4 = Table(names=['x_0', 'y_0', 'sharpness'],
+                            data=[[17.4], [16], [0.4]])
+        for i, init_guesses in enumerate([init_guess1, init_guess2,
+                                          init_guess3, init_guess4]):
+            dao_phot = DAOPhotPSFPhotometry(crit_separation=8, threshold=40,
+                                            fwhm=4 * np.sqrt(2 * np.log(2)),
+                                            psf_model=psf_model,
+                                            fitshape=(11, 11),
+                                            extra_output_cols=['sharpness',
+                                                               'roundness1',
+                                                               'roundness2'])
+            phot_results = dao_phot(image, init_guesses=init_guesses)
+            # test that the original required columns are also passed
+            # back, as well as extra_output_cols
+            assert np.all([name in phot_results.colnames for name in
+                           ['x_0', 'y_0']])
+            assert np.all([name in phot_results.colnames for name in
+                           ['sharpness', 'roundness1', 'roundness2']])
+            assert len(phot_results) == 2
+            # checks to verify that half-passing init_guesses results
+            # in NaN output for extra_output_cols not passed as initial
+            # guesses
+            if i == 2:  # init_guess3
+                assert np.all(np.all(np.isnan(phot_results[o])) for o in
+                              ['sharpness', 'roundness1', 'roundness2'])
+            if i == 3:  # init_guess4
+                assert np.all(np.all(np.isnan(phot_results[o])) for o in
+                              ['roundness1', 'roundness2'])
+                assert np.all(~np.isnan(phot_results['sharpness']))
 
 
 @pytest.fixture(params=[2, 3])
 def overlap_image(request):
     if request.param == 2:
         close_tab = Table([[50.0, 53.0], [50.0, 50.0], [25.0, 25.0]],
                           names=['x_0', 'y_0', 'flux_0'])
@@ -674,37 +707,39 @@
 
 @pytest.mark.skipif(not HAS_SCIPY, reason='scipy is required')
 def test_psf_fitting_group(overlap_image):
     """
     Test psf_photometry when two input stars are close and need to be
     fit together.
     """
-    from photutils.background import MADStdBackgroundRMS
+    with pytest.warns(AstropyDeprecationWarning):
+        from photutils.background import MADStdBackgroundRMS
 
-    # There are a few models here that fail, be it something
-    # created by EPSFBuilder or simpler the Moffat2D one
-    # unprepared_psf = Moffat2D(amplitude=1, gamma=2, alpha=2.8, x_0=0, y_0=0)
-    # psf = prepare_psf_model(unprepared_psf, xname='x_0', yname='y_0',
-    #                         fluxname=None)
-    psf = prepare_psf_model(Gaussian2D(), renormalize_psf=False)
-
-    psf.fwhm = Parameter('fwhm', 'this is not the way to add this I think')
-    psf.fwhm.value = 10
-
-    separation_crit = 10
-
-    # choose low threshold and fwhm to find stars no matter what
-    basic_phot = BasicPSFPhotometry(finder=DAOStarFinder(1, 1),
-                                    group_maker=DAOGroup(separation_crit),
-                                    bkg_estimator=MADStdBackgroundRMS(),
-                                    fitter=LevMarLSQFitter(),
-                                    psf_model=psf,
-                                    fitshape=31)
-    # this should not raise AttributeError: Attribute "offset_0_0" not found
-    basic_phot(image=overlap_image)
+        # There are a few models here that fail, be it something created
+        # by EPSFBuilder or simpler the Moffat2D one unprepared_psf =
+        # Moffat2D(amplitude=1, gamma=2, alpha=2.8, x_0=0, y_0=0) psf =
+        # prepare_psf_model(unprepared_psf, xname='x_0', yname='y_0',
+        # fluxname=None)
+        psf = prepare_psf_model(Gaussian2D(), renormalize_psf=False)
+
+        psf.fwhm = Parameter('fwhm', 'this is not the way to add this I think')
+        psf.fwhm.value = 10
+
+        separation_crit = 10
+
+        # choose low threshold and fwhm to find stars no matter what
+        basic_phot = BasicPSFPhotometry(finder=DAOStarFinder(1, 1),
+                                        group_maker=DAOGroup(separation_crit),
+                                        bkg_estimator=MADStdBackgroundRMS(),
+                                        fitter=LevMarLSQFitter(),
+                                        psf_model=psf,
+                                        fitshape=31)
+        # this should not raise AttributeError: Attribute "offset_0_0"
+        # not found
+        basic_phot(image=overlap_image)
 
 
 @pytest.mark.skipif(not HAS_SCIPY, reason='scipy is required')
 def test_finder_return_none():
     """
     Test psf_photometry with finder that does not return None if no
     sources are detected, to test Iterative PSF fitting.
@@ -720,59 +755,62 @@
             x = np.mean(xs)
             y = np.mean(ys)
             table.add_row([int(n + 1), x, y, f * 9])
         table.sort(['flux'])
 
         return table
 
-    prf = np.zeros((7, 7), float)
-    prf[2:5, 2:5] = 1 / 9
-    prf = FittableImageModel(prf)
-
-    img = np.zeros((50, 50), float)
-    x0 = [38, 20, 35]
-    y0 = [20, 5, 40]
-    f0 = [50, 100, 200]
-    for x, y, f in zip(x0, y0, f0):
-        img[y - 1:y + 2, x - 1:x + 2] = f / 9
-
-    intab = Table(data=[[37, 19.6, 34.9], [19.6, 4.5, 40.1], [45, 103, 210]],
-                  names=['x_0', 'y_0', 'flux_0'])
-
-    iter_phot = IterativelySubtractedPSFPhotometry(finder=tophatfinder,
-                                                   group_maker=DAOGroup(2),
-                                                   bkg_estimator=None,
-                                                   psf_model=prf,
-                                                   fitshape=7, niters=2,
-                                                   aperture_radius=3)
-
-    with pytest.warns(AstropyUserWarning, match='Both init_guesses and finder '
-                      'are different than None'):
-        results = iter_phot(image=img, init_guesses=intab)
-    assert_allclose(results['flux_fit'], f0, rtol=0.05)
+    with pytest.warns(AstropyDeprecationWarning):
+        prf = np.zeros((7, 7), float)
+        prf[2:5, 2:5] = 1 / 9
+        prf = FittableImageModel(prf)
+
+        img = np.zeros((50, 50), float)
+        x0 = [38, 20, 35]
+        y0 = [20, 5, 40]
+        f0 = [50, 100, 200]
+        for x, y, f in zip(x0, y0, f0):
+            img[y - 1:y + 2, x - 1:x + 2] = f / 9
+
+        intab = Table(data=[[37, 19.6, 34.9], [19.6, 4.5, 40.1],
+                            [45, 103, 210]], names=['x_0', 'y_0', 'flux_0'])
+
+        iter_phot = IterativelySubtractedPSFPhotometry(finder=tophatfinder,
+                                                       group_maker=DAOGroup(2),
+                                                       bkg_estimator=None,
+                                                       psf_model=prf,
+                                                       fitshape=7, niters=2,
+                                                       aperture_radius=3)
+
+        match = 'Both init_guesses and finder are different than None'
+        with pytest.warns(AstropyUserWarning, match=match):
+            results = iter_phot(image=img, init_guesses=intab)
+        assert_allclose(results['flux_fit'], f0, rtol=0.05)
 
 
 @pytest.mark.skipif(not HAS_SCIPY, reason='scipy is required')
 def test_psf_photometry_uncertainties():
     """
     Test an Astropy fitter that does not return a parameter
     covariance matrix (param_cov). The output table should not
     contain flux_unc, x_0_unc, and y_0_unc columns.
     """
-    psf = IntegratedGaussianPRF(sigma=GAUSSIAN_WIDTH)
+    with pytest.warns(AstropyDeprecationWarning):
+        psf = IntegratedGaussianPRF(sigma=GAUSSIAN_WIDTH)
 
-    basic_phot = BasicPSFPhotometry(group_maker=DAOGroup(2),
-                                    bkg_estimator=None, psf_model=psf,
-                                    fitter=SimplexLSQFitter(),
-                                    fitshape=7)
-    with pytest.warns(AstropyUserWarning, match='The fit may be unsuccessful'):
-        phot_tbl = basic_phot(image=image, init_guesses=INTAB)
-    columns = ('flux_unc', 'x_0_unc', 'y_0_unc')
-    for column in columns:
-        assert column not in phot_tbl.colnames
+        basic_phot = BasicPSFPhotometry(group_maker=DAOGroup(2),
+                                        bkg_estimator=None, psf_model=psf,
+                                        fitter=SimplexLSQFitter(),
+                                        fitshape=7)
+        match = 'The fit may be unsuccessful'
+        with pytest.warns(AstropyUserWarning, match=match):
+            phot_tbl = basic_phot(image=image, init_guesses=INTAB)
+        columns = ('flux_unc', 'x_0_unc', 'y_0_unc')
+        for column in columns:
+            assert column not in phot_tbl.colnames
 
 
 @pytest.mark.skipif(not HAS_SCIPY, reason='scipy is required')
 def test_re_use_result_as_initial_guess():
     img_shape = (32, 32)
     # generate image with read-out noise (Gaussian) and
     # background noise (Poisson)
@@ -780,122 +818,190 @@
              + make_noise_image(img_shape, distribution='poisson', mean=6.0,
                                 seed=0)
              + make_noise_image(img_shape, distribution='gaussian', mean=0.0,
                                 stddev=2.0, seed=0))
 
     _, _, dao_phot_obj = make_psf_photometry_objs()
 
-    with pytest.warns(AstropyUserWarning, match='The fit may be unsuccessful'):
+    match = 'The fit may be unsuccessful'
+    ctx1 = pytest.warns(AstropyUserWarning, match=match)
+    if PYTEST_LT_80:
+        ctx2 = nullcontext()
+    else:
+        ctx2 = pytest.warns(AstropyDeprecationWarning)
+    with ctx1, ctx2:
         result_table = dao_phot_obj(image)
-    result_table['x'] = result_table['x_fit']
-    result_table['y'] = result_table['y_fit']
-    result_table['flux'] = result_table['flux_fit']
-    with pytest.warns(AstropyUserWarning, match='Both init_guesses and finder '
-                      'are different than None'):
+        result_table['x'] = result_table['x_fit']
+        result_table['y'] = result_table['y_fit']
+        result_table['flux'] = result_table['flux_fit']
+
+    match1 = 'Both init_guesses and finder are different than None'
+    ctx1 = pytest.warns(AstropyUserWarning, match=match1)
+    if PYTEST_LT_80:
+        ctx2 = nullcontext()
+        ctx3 = nullcontext()
+        ctx4 = nullcontext()
+    else:
+        match2 = 'init_guesses contains a "group_id" column'
+        match3 = 'The fit may be unsuccessful; check fit_info'
+        ctx2 = pytest.warns(AstropyUserWarning, match=match2)
+        ctx3 = pytest.warns(AstropyUserWarning, match=match3)
+        ctx4 = pytest.warns(AstropyDeprecationWarning)
+    with ctx1, ctx2, ctx3, ctx4:
         second_result = dao_phot_obj(image, init_guesses=result_table)
-    assert second_result
+        assert second_result
 
 
 @pytest.mark.skipif(not HAS_SCIPY, reason='scipy is required')
 def test_photometry_mask_nan():
-    size = 64
-    sources1 = Table()
-    sources1['flux'] = [800]
-    sources1['x_0'] = [size / 2]
-    sources1['y_0'] = [size / 2]
-    sources1['sigma'] = [6]
-    sources1['theta'] = [0]
-
-    img_shape = (size, size)
-    data = make_gaussian_prf_sources_image(img_shape, sources1)
-    data[30, 20:40] = np.nan
-
-    daogroup = DAOGroup(3.0)
-    psf_model = IntegratedGaussianPRF(sigma=2.0)
-    psfphot = BasicPSFPhotometry(group_maker=daogroup, finder=None,
-                                 bkg_estimator=None, psf_model=psf_model,
-                                 fitshape=(11, 11))
-
-    init = Table()
-    init['x_0'] = [30]
-    init['y_0'] = [30]
-    init['flux_0'] = [200.0]
-
-    mask = ~np.isfinite(data)
-    tbl = psfphot(data, init_guesses=init, mask=mask)
-    assert tbl['x_fit'] != init['x_0']
-    assert tbl['y_fit'] != init['y_0']
-    assert tbl['flux_fit'] != init['flux_0']
-
-    with pytest.warns(AstropyUserWarning, match='Input data contains unmasked '
-                      'non-finite values'):
-        tbl2 = psfphot(data, init_guesses=init)
-        assert tbl == tbl2
+    with pytest.warns(AstropyDeprecationWarning):
+        size = 64
+        sources1 = Table()
+        sources1['flux'] = [800]
+        sources1['x_0'] = [size / 2]
+        sources1['y_0'] = [size / 2]
+        sources1['sigma'] = [6]
+        sources1['theta'] = [0]
+
+        img_shape = (size, size)
+        data = make_gaussian_prf_sources_image(img_shape, sources1)
+        data[30, 20:40] = np.nan
+
+        daogroup = DAOGroup(3.0)
+        psf_model = IntegratedGaussianPRF(sigma=2.0)
+        psfphot = BasicPSFPhotometry(group_maker=daogroup, finder=None,
+                                     bkg_estimator=None, psf_model=psf_model,
+                                     fitshape=(11, 11))
+
+        init = Table()
+        init['x_0'] = [30]
+        init['y_0'] = [30]
+        init['flux_0'] = [200.0]
+
+        mask = ~np.isfinite(data)
+        tbl = psfphot(data, init_guesses=init, mask=mask)
+        assert tbl['x_fit'] != init['x_0']
+        assert tbl['y_fit'] != init['y_0']
+        assert tbl['flux_fit'] != init['flux_0']
+
+        match = 'Input data contains unmasked non-finite values'
+        with pytest.warns(AstropyUserWarning, match=match):
+            tbl2 = psfphot(data, init_guesses=init)
+            assert tbl == tbl2
 
 
 @pytest.mark.skipif(not HAS_SCIPY, reason='scipy is required')
 def test_photometry_subshape():
-    size = 21
-    cen = (size - 1) // 2
-    sigma = 2.0
-    sources = Table()
-    sources['flux'] = [1]
-    sources['x_0'] = [cen]
-    sources['y_0'] = [cen]
-    sources['sigma'] = [sigma]
-    psf = make_gaussian_prf_sources_image((size, size), sources)
-    psf_model = FittableImageModel(psf)
-
-    sources = Table()
-    sources['flux'] = [2000, 1000]
-    sources['x_0'] = [18, 7]
-    sources['y_0'] = [17, 25]
-    sources['sigma'] = [sigma, sigma]
-    shape = (33, 33)
-    image = make_gaussian_prf_sources_image(shape, sources)
-
-    daogroup = DAOGroup(crit_separation=8)
-    mmm_bkg = MMMBackground()
-    iraffind = IRAFStarFinder(threshold=10, fwhm=5, roundlo=-1, minsep_fwhm=1)
-    fitter = LevMarLSQFitter()
-
-    pobj1 = BasicPSFPhotometry(finder=iraffind, group_maker=daogroup,
-                               bkg_estimator=mmm_bkg, psf_model=psf_model,
-                               fitter=fitter, fitshape=(7, 7),
-                               aperture_radius=5, subshape=(3, 3))
-    pobj2 = BasicPSFPhotometry(finder=iraffind, group_maker=daogroup,
-                               bkg_estimator=mmm_bkg, psf_model=psf_model,
-                               fitter=fitter, fitshape=(7, 7),
-                               aperture_radius=5, subshape=5)
-    pobj3 = BasicPSFPhotometry(finder=iraffind, group_maker=daogroup,
-                               bkg_estimator=mmm_bkg, psf_model=psf_model,
-                               fitter=fitter, fitshape=(7, 7),
-                               aperture_radius=5, subshape=None)
-    pobj4 = BasicPSFPhotometry(finder=iraffind, group_maker=daogroup,
-                               bkg_estimator=mmm_bkg, psf_model=psf_model,
-                               fitter=fitter, fitshape=(7, 7),
-                               aperture_radius=5, subshape=7)
-
-    _ = pobj1(image)
-    _ = pobj2(image)
-    _ = pobj3(image)
-    _ = pobj4(image)
-    resid1 = pobj1.get_residual_image()
-    resid2 = pobj2.get_residual_image()
-    resid3 = pobj3.get_residual_image()
-    resid4 = pobj4.get_residual_image()
-    assert np.sum(resid1) > np.sum(resid2)
-    assert_allclose(np.sum(resid3), np.sum(resid4))
+    with pytest.warns(AstropyDeprecationWarning):
+        size = 21
+        cen = (size - 1) // 2
+        sigma = 2.0
+        sources = Table()
+        sources['flux'] = [1]
+        sources['x_0'] = [cen]
+        sources['y_0'] = [cen]
+        sources['sigma'] = [sigma]
+        psf = make_gaussian_prf_sources_image((size, size), sources)
+        psf_model = FittableImageModel(psf)
+
+        sources = Table()
+        sources['flux'] = [2000, 1000]
+        sources['x_0'] = [18, 7]
+        sources['y_0'] = [17, 25]
+        sources['sigma'] = [sigma, sigma]
+        shape = (33, 33)
+        image = make_gaussian_prf_sources_image(shape, sources)
+
+        daogroup = DAOGroup(crit_separation=8)
+        mmm_bkg = MMMBackground()
+        iraffind = IRAFStarFinder(threshold=10, fwhm=5, roundlo=-1,
+                                  minsep_fwhm=1)
+        fitter = LevMarLSQFitter()
+
+        pobj1 = BasicPSFPhotometry(finder=iraffind, group_maker=daogroup,
+                                   bkg_estimator=mmm_bkg, psf_model=psf_model,
+                                   fitter=fitter, fitshape=(7, 7),
+                                   aperture_radius=5, subshape=(3, 3))
+        pobj2 = BasicPSFPhotometry(finder=iraffind, group_maker=daogroup,
+                                   bkg_estimator=mmm_bkg, psf_model=psf_model,
+                                   fitter=fitter, fitshape=(7, 7),
+                                   aperture_radius=5, subshape=5)
+        pobj3 = BasicPSFPhotometry(finder=iraffind, group_maker=daogroup,
+                                   bkg_estimator=mmm_bkg, psf_model=psf_model,
+                                   fitter=fitter, fitshape=(7, 7),
+                                   aperture_radius=5, subshape=None)
+        pobj4 = BasicPSFPhotometry(finder=iraffind, group_maker=daogroup,
+                                   bkg_estimator=mmm_bkg, psf_model=psf_model,
+                                   fitter=fitter, fitshape=(7, 7),
+                                   aperture_radius=5, subshape=7)
+
+        _ = pobj1(image)
+        _ = pobj2(image)
+        _ = pobj3(image)
+        _ = pobj4(image)
+        resid1 = pobj1.get_residual_image()
+        resid2 = pobj2.get_residual_image()
+        resid3 = pobj3.get_residual_image()
+        resid4 = pobj4.get_residual_image()
+        assert np.sum(resid1) > np.sum(resid2)
+        assert_allclose(np.sum(resid3), np.sum(resid4))
 
 
 @pytest.mark.skipif(not HAS_SCIPY, reason='scipy is required')
 def test_subshape_invalid():
     basic_phot_obj = make_psf_photometry_objs()[0]
 
     with pytest.raises(ValueError):
         basic_phot_obj.subshape = (2, 2)
     with pytest.raises(ValueError):
         basic_phot_obj.subshape = 2
     with pytest.raises(ValueError):
         basic_phot_obj.subshape = (-1, 0)
     with pytest.raises(ValueError):
         basic_phot_obj.subshape = (3, 3, 3)
+
+
+@pytest.mark.filterwarnings('ignore:Both init_guesses and finder are '
+                            'different than None')
+@pytest.mark.filterwarnings('ignore:No sources were found')
+@pytest.mark.skipif(not HAS_SCIPY, reason='scipy is required')
+@pytest.mark.skipif(not minversion(astropy, '5.3'),
+                    reason='astropy 5.3 is required')
+@pytest.mark.parametrize("sigma_psf, sources",
+                         [(sigma_psfs[0], sources1),
+                          (sigma_psfs[1], sources2)])
+def test_psf_photometry_oneiter_uncert(sigma_psf, sources):
+    """
+    Make an image with a group of two overlapped stars and an
+    isolated one, and check that the best-fit fluxes have smaller
+    uncertainties when the measured fluxes have smaller uncertainties.
+    """
+    img_shape = (32, 32)
+    # generate image with read-out noise (Gaussian) and
+    # background noise (Poisson)
+    image = (make_gaussian_prf_sources_image(img_shape, sources)
+             + make_noise_image(img_shape, distribution='poisson', mean=6.0,
+                                seed=0)
+             + make_noise_image(img_shape, distribution='gaussian', mean=0.0,
+                                stddev=2.0, seed=0))
+
+    sigma_clip = SigmaClip(sigma=3.0)
+    bkgrms = StdBackgroundRMS(sigma_clip)
+    std = bkgrms(image)
+    phot_objs = make_psf_photometry_objs(std, sigma_psf)
+
+    flux_uncertainties_0 = []
+    flux_uncertainties_1 = []
+
+    for uncertainty_scale_factor, flux_uncert in zip(
+        [1e-5, 0.1], [flux_uncertainties_0, flux_uncertainties_1]
+    ):
+        for phot_proc in phot_objs:
+            uncertainty = (
+                uncertainty_scale_factor * np.std(image) * np.ones_like(image)
+            )
+            with pytest.warns(AstropyDeprecationWarning):
+                result_tab = phot_proc(image, uncertainty=uncertainty)
+            flux_uncert.append(np.array(result_tab['flux_unc']))
+
+    for uncert_0, uncert_1 in zip(flux_uncertainties_0, flux_uncertainties_1):
+        assert np.all(uncert_0 < uncert_1)
```

### Comparing `photutils-1.8.0/photutils/psf/tests/test_utils.py` & `photutils-1.9.0/photutils/psf/tests/test_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,22 +3,27 @@
 Tests for the utils module.
 """
 
 import numpy as np
 import pytest
 from astropy.convolution.utils import discretize_model
 from astropy.modeling.models import Gaussian2D
+from astropy.nddata import NDData
 from astropy.table import Table
+from astropy.utils.exceptions import AstropyDeprecationWarning
 from numpy.testing import assert_allclose
 
+from photutils import datasets
+from photutils.detection import find_peaks
+from photutils.psf import EPSFBuilder, extract_stars
 from photutils.psf.groupstars import DAOGroup
 from photutils.psf.models import IntegratedGaussianPRF
-from photutils.psf.photometry import BasicPSFPhotometry
-from photutils.psf.utils import (get_grouped_psf_model, prepare_psf_model,
-                                 subtract_psf)
+from photutils.psf.photometry_depr import BasicPSFPhotometry
+from photutils.psf.utils import (get_grouped_psf_model, grid_from_epsfs,
+                                 prepare_psf_model, subtract_psf)
 from photutils.utils._optional_deps import HAS_SCIPY
 
 PSF_SIZE = 11
 GAUSSIAN_WIDTH = 1.0
 IMAGE_SIZE = 101
 
 # Position and FLUXES of test sources
@@ -145,78 +150,80 @@
 @pytest.mark.filterwarnings('ignore:aperture_radius is None and could not '
                             'be determined by psf_model')
 @pytest.mark.skipif(not HAS_SCIPY, reason='scipy is required')
 def test_prepare_psf_model_offset():
     """
     Regression test to ensure the offset is in the correct direction.
     """
-    norm = False
-    sigma = 3.0
-    amplitude = 1.0 / (2 * np.pi * sigma**2)
-    xcen = ycen = 0.0
-    psf0 = Gaussian2D(amplitude, xcen, ycen, sigma, sigma)
-    psf1 = prepare_psf_model(psf0, xname='x_mean', yname='y_mean',
-                             renormalize_psf=norm)
-    psf2 = prepare_psf_model(psf0, renormalize_psf=norm)
-    psf3 = prepare_psf_model(psf0, xname='x_mean', renormalize_psf=norm)
-    psf4 = prepare_psf_model(psf0, yname='y_mean', renormalize_psf=norm)
-
-    yy, xx = np.mgrid[0:101, 0:101]
-    psf = psf1.copy()
-    xval = 48
-    yval = 52
-    flux = 14.51
-    psf.x_mean_2 = xval
-    psf.y_mean_2 = yval
-    data = psf(xx, yy) * flux
-
-    group_maker = DAOGroup(2)
-    bkg_estimator = None
-    fitshape = 7
-    init_guesses = Table([[46.1], [57.3], [7.1]],
-                         names=['x_0', 'y_0', 'flux_0'])
-
-    phot1 = BasicPSFPhotometry(group_maker=group_maker,
-                               bkg_estimator=bkg_estimator, fitshape=fitshape,
-                               psf_model=psf1)
-    tbl1 = phot1(image=data, init_guesses=init_guesses)
-
-    phot2 = BasicPSFPhotometry(group_maker=group_maker,
-                               bkg_estimator=bkg_estimator, fitshape=fitshape,
-                               psf_model=psf2)
-    tbl2 = phot2(image=data, init_guesses=init_guesses)
-
-    phot3 = BasicPSFPhotometry(group_maker=group_maker,
-                               bkg_estimator=bkg_estimator, fitshape=fitshape,
-                               psf_model=psf3)
-    tbl3 = phot3(image=data, init_guesses=init_guesses)
-
-    phot4 = BasicPSFPhotometry(group_maker=group_maker,
-                               bkg_estimator=bkg_estimator, fitshape=fitshape,
-                               psf_model=psf4)
-    tbl4 = phot4(image=data, init_guesses=init_guesses)
-
-    assert_allclose((tbl1['x_fit'][0], tbl1['y_fit'][0], tbl1['flux_fit'][0]),
-                    (xval, yval, flux))
-    assert_allclose((tbl2['x_fit'][0], tbl2['y_fit'][0], tbl2['flux_fit'][0]),
-                    (xval, yval, flux))
-    assert_allclose((tbl3['x_fit'][0], tbl3['y_fit'][0], tbl3['flux_fit'][0]),
-                    (xval, yval, flux))
-    assert_allclose((tbl4['x_fit'][0], tbl4['y_fit'][0], tbl4['flux_fit'][0]),
-                    (xval, yval, flux))
+    with pytest.warns(AstropyDeprecationWarning):
+        norm = False
+        sigma = 3.0
+        amplitude = 1.0 / (2 * np.pi * sigma**2)
+        xcen = ycen = 0.0
+        psf0 = Gaussian2D(amplitude, xcen, ycen, sigma, sigma)
+        psf1 = prepare_psf_model(psf0, xname='x_mean', yname='y_mean',
+                                 renormalize_psf=norm)
+        psf2 = prepare_psf_model(psf0, renormalize_psf=norm)
+        psf3 = prepare_psf_model(psf0, xname='x_mean', renormalize_psf=norm)
+        psf4 = prepare_psf_model(psf0, yname='y_mean', renormalize_psf=norm)
+
+        yy, xx = np.mgrid[0:101, 0:101]
+        psf = psf1.copy()
+        xval = 48
+        yval = 52
+        flux = 14.51
+        psf.x_mean_2 = xval
+        psf.y_mean_2 = yval
+        data = psf(xx, yy) * flux
+
+        group_maker = DAOGroup(2)
+        bkg_estimator = None
+        fitshape = 7
+        init_guesses = Table([[46.1], [57.3], [7.1]],
+                             names=['x_0', 'y_0', 'flux_0'])
+
+        phot1 = BasicPSFPhotometry(group_maker=group_maker,
+                                   bkg_estimator=bkg_estimator,
+                                   fitshape=fitshape, psf_model=psf1)
+        tbl1 = phot1(image=data, init_guesses=init_guesses)
+
+        phot2 = BasicPSFPhotometry(group_maker=group_maker,
+                                   bkg_estimator=bkg_estimator,
+                                   fitshape=fitshape, psf_model=psf2)
+        tbl2 = phot2(image=data, init_guesses=init_guesses)
+
+        phot3 = BasicPSFPhotometry(group_maker=group_maker,
+                                   bkg_estimator=bkg_estimator,
+                                   fitshape=fitshape, psf_model=psf3)
+        tbl3 = phot3(image=data, init_guesses=init_guesses)
+
+        phot4 = BasicPSFPhotometry(group_maker=group_maker,
+                                   bkg_estimator=bkg_estimator,
+                                   fitshape=fitshape, psf_model=psf4)
+        tbl4 = phot4(image=data, init_guesses=init_guesses)
+
+        assert_allclose((tbl1['x_fit'][0], tbl1['y_fit'][0],
+                         tbl1['flux_fit'][0]), (xval, yval, flux))
+        assert_allclose((tbl2['x_fit'][0], tbl2['y_fit'][0],
+                         tbl2['flux_fit'][0]), (xval, yval, flux))
+        assert_allclose((tbl3['x_fit'][0], tbl3['y_fit'][0],
+                         tbl3['flux_fit'][0]), (xval, yval, flux))
+        assert_allclose((tbl4['x_fit'][0], tbl4['y_fit'][0],
+                         tbl4['flux_fit'][0]), (xval, yval, flux))
 
 
 @pytest.mark.skipif(not HAS_SCIPY, reason='scipy is required')
 def test_get_grouped_psf_model():
     igp = IntegratedGaussianPRF(sigma=1.2)
     tab = Table(names=['x_0', 'y_0', 'flux_0'],
                 data=[[1, 2], [3, 4], [0.5, 1]])
     pars_to_set = {'x_0': 'x_0', 'y_0': 'y_0', 'flux_0': 'flux'}
 
-    gpsf = get_grouped_psf_model(igp, tab, pars_to_set)
+    with pytest.warns(AstropyDeprecationWarning):
+        gpsf = get_grouped_psf_model(igp, tab, pars_to_set)
 
     assert gpsf.x_0_0 == 1
     assert gpsf.y_0_1 == 4
     assert gpsf.flux_0 == 0.5
     assert gpsf.flux_1 == 1
     assert gpsf.sigma_0 == gpsf.sigma_1 == 1.2
 
@@ -234,24 +241,129 @@
 @pytest.mark.skipif(not HAS_SCIPY, reason='scipy is required')
 def test_get_grouped_psf_model_submodel_names(prf_model):
     """Verify that submodel tagging works"""
     tab = Table(names=['x_0', 'y_0', 'flux_0'],
                 data=[[1, 2], [3, 4], [0.5, 1]])
     pars_to_set = {'x_0': 'x_0', 'y_0': 'y_0', 'flux_0': 'flux'}
 
-    gpsf = get_grouped_psf_model(prf_model, tab, pars_to_set)
-    # There should be two submodels one named 0 and one named 1
-    assert len([submodel for submodel in gpsf.traverse_postorder()
-                if submodel.name == 0]) == 1
-    assert len([submodel for submodel in gpsf.traverse_postorder()
-                if submodel.name == 1]) == 1
+    with pytest.warns(AstropyDeprecationWarning):
+        gpsf = get_grouped_psf_model(prf_model, tab, pars_to_set)
+        # There should be two submodels one named 0 and one named 1
+        assert len([submodel for submodel in gpsf.traverse_postorder()
+                    if submodel.name == 0]) == 1
+        assert len([submodel for submodel in gpsf.traverse_postorder()
+                    if submodel.name == 1]) == 1
 
 
 @pytest.mark.skipif(not HAS_SCIPY, reason='scipy is required')
 def test_subtract_psf():
     """Test subtract_psf."""
-    psf = IntegratedGaussianPRF(sigma=1.0)
-    posflux = INTAB.copy()
-    for n in posflux.colnames:
-        posflux.rename_column(n, n.split('_')[0] + '_fit')
-    residuals = subtract_psf(image, psf, posflux)
-    assert np.max(np.abs(residuals)) < 0.0052
+    with pytest.warns(AstropyDeprecationWarning):
+        psf = IntegratedGaussianPRF(sigma=1.0)
+        posflux = INTAB.copy()
+        for n in posflux.colnames:
+            posflux.rename_column(n, n.split('_')[0] + '_fit')
+        residuals = subtract_psf(image, psf, posflux)
+        assert np.max(np.abs(residuals)) < 0.0052
+
+
+@pytest.mark.remote_data
+class TestGridFromEPSFs:
+    """Tests for `photutils.psf.utils.grid_from_epsfs`."""
+
+    def setup_class(self, cutout_size=25):
+        # make a set of 4 EPSF models
+
+        self.cutout_size = cutout_size
+
+        # make simulated image
+        hdu = datasets.load_simulated_hst_star_image()
+        data = hdu.data
+
+        # break up the image into four quadrants
+        q1 = data[0:500, 0:500]
+        q2 = data[0:500, 500:1000]
+        q3 = data[500:1000, 0:500]
+        q4 = data[500:1000, 500:1000]
+
+        # select some starts from each quadrant to use to build the epsf
+        quad_stars = {'q1': {'data': q1, 'fiducial': (0., 0.), 'epsf': None},
+                      'q2': {'data': q2, 'fiducial': (1000., 1000.), 'epsf': None},
+                      'q3': {'data': q3, 'fiducial': (1000., 0.), 'epsf': None},
+                      'q4': {'data': q4, 'fiducial': (0., 1000.), 'epsf': None}}
+
+        for q in ['q1', 'q2', 'q3', 'q4']:
+            quad_data = quad_stars[q]['data']
+            peaks_tbl = find_peaks(quad_data, threshold=500.)
+
+            # filter out sources near edge
+            size = cutout_size
+            hsize = (size - 1) / 2
+            x = peaks_tbl['x_peak']
+            y = peaks_tbl['y_peak']
+            mask = ((x > hsize) & (x < (quad_data.shape[1] - 1 - hsize))
+                    & (y > hsize) & (y < (quad_data.shape[0] - 1 - hsize)))
+
+            stars_tbl = Table()
+            stars_tbl['x'] = peaks_tbl['x_peak'][mask]
+            stars_tbl['y'] = peaks_tbl['y_peak'][mask]
+
+            stars = extract_stars(NDData(quad_data), stars_tbl,
+                                  size=cutout_size)
+
+            epsf_builder = EPSFBuilder(oversampling=4, maxiters=3,
+                                       progress_bar=False)
+            epsf, fitted_stars = epsf_builder(stars)
+
+            # set x_0, y_0 to fiducial point
+            epsf.y_0 = quad_stars[q]['fiducial'][0]
+            epsf.x_0 = quad_stars[q]['fiducial'][1]
+
+            quad_stars[q]['epsf'] = epsf
+
+        self.epsfs = [quad_stars[x]['epsf'] for x in quad_stars]
+        self.grid_xypos = [quad_stars[x]['fiducial'] for x in quad_stars]
+
+    def test_basic_test_grid_from_epsfs(self):
+
+        psf_grid = grid_from_epsfs(self.epsfs)
+
+        assert np.all(psf_grid.oversampling == self.epsfs[0].oversampling)
+        assert psf_grid.data.shape == (4, psf_grid.oversampling * 25 + 1,
+                                       psf_grid.oversampling * 25 + 1)
+
+    def test_grid_xypos(self):
+        """Test both options for setting PSF locations"""
+
+        # default option x_0 and y_0s on input EPSFs
+        psf_grid = grid_from_epsfs(self.epsfs)
+
+        assert psf_grid.meta['grid_xypos'] == [(0.0, 0.0), (1000.0, 1000.0),
+                                               (0.0, 1000.0), (1000.0, 0.0)]
+
+        # or pass in a list
+        grid_xypos = [(250.0, 250.0), (750.0, 750.0),
+                      (250.0, 750.0), (750.0, 250.0)]
+
+        psf_grid = grid_from_epsfs(self.epsfs, grid_xypos=grid_xypos)
+        assert psf_grid.meta['grid_xypos'] == grid_xypos
+
+    def test_meta(self):
+        """Test the option for setting 'meta'"""
+
+        keys = ['grid_xypos', 'oversampling', 'fill_value']
+
+        # when 'meta' isn't provided, there should be just three keys
+        psf_grid = grid_from_epsfs(self.epsfs)
+        for key in keys:
+            assert key in psf_grid.meta
+
+        # when meta is provided, those new keys should exist and anything
+        # in the list above should be overwritten
+        meta = {'grid_xypos': 0.0, 'oversampling': 0.0,
+                'fill_value': -999, 'extra_key': 'extra'}
+        psf_grid = grid_from_epsfs(self.epsfs, meta=meta)
+        for key in keys + ['extra_key']:
+            assert key in psf_grid.meta
+        assert psf_grid.meta['grid_xypos'].sort() == self.grid_xypos.sort()
+        assert psf_grid.meta['oversampling'] == 4
+        assert psf_grid.meta['fill_value'] == 0.0
```

### Comparing `photutils-1.8.0/photutils/segmentation/catalog.py` & `photutils-1.9.0/photutils/segmentation/catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
                                 EllipticalAperture, RectangularAnnulus)
 from photutils.background import SExtractorBackground
 from photutils.centroids import centroid_quadratic
 from photutils.segmentation.core import SegmentationImage
 from photutils.utils._convolution import _filter_data
 from photutils.utils._misc import _get_meta
 from photutils.utils._moments import _moments, _moments_central
-from photutils.utils._optional_deps import HAS_TQDM
+from photutils.utils._progress_bars import add_progress_bar
 from photutils.utils._quantity_helpers import process_quantities
 from photutils.utils.cutouts import CutoutImage
 
 __all__ = ['SourceCatalog']
 __doctest_requires__ = {('SourceCatalog', 'SourceCatalog.*'): ['scipy']}
 
 
@@ -428,20 +428,14 @@
         self._apermask_kwargs = {
             'circ': {'method': 'subpixel', 'subpixels': 5},
             'kron': {'method': 'center'},
             'fluxfrac': {'method': 'subpixel', 'subpixels': 5},
             'cen_win': {'method': 'subpixel', 'subpixels': 11}
         }
 
-    def _progress_bar(self, iterable, desc=''):
-        if self.progress_bar and HAS_TQDM:
-            from tqdm.auto import tqdm  # pragma: no cover
-            iterable = tqdm(iterable, desc=desc)
-        return iterable
-
     @property
     def _properties(self):
         """
         A list of all class properties, include lazyproperties (even in
         superclasses).
         """
         def isproperty(obj):
@@ -1364,17 +1358,21 @@
         if self.isscalar:
             radius_hl = np.array([radius_hl])
         min_radius = 0.5  # define minimum half-light radius
         mask = (radius_hl < min_radius) | ~np.isfinite(radius_hl)
         radius_hl[mask] = min_radius
         kwargs = self._apermask_kwargs['cen_win']
 
+        labels = self.labels
+        if self.progress_bar:
+            desc = 'centroid_win'
+            labels = add_progress_bar(labels, desc=desc)  # pragma: no cover
+
         xcen_win = []
         ycen_win = []
-        labels = self._progress_bar(self.labels, 'centroid_win')
         for label, xcen, ycen, rad_hl in zip(labels, self._xcentroid,
                                              self._ycentroid, radius_hl):
 
             if np.any(~np.isfinite((xcen, ycen))):
                 xcen_win.append(np.nan)
                 ycen_win.append(np.nan)
                 continue
@@ -1541,16 +1539,19 @@
             #   - quadratic fit failed
             #   - quadratic fit does not have a maximum
             #   - quadratic fit maximum falls outside image
             #   - not enough unmasked data points (6 are required)
             #   - maximum value is at the edge of the data
             warnings.simplefilter('ignore', AstropyUserWarning)
 
-            cutouts = self._progress_bar(self._data_cutouts,
-                                         'centroid_quad')
+            cutouts = self._data_cutouts
+            if self.progress_bar:
+                desc = 'centroid_quad'
+                cutouts = add_progress_bar(cutouts, desc=desc)  # pragma: no cover
+
             for data, mask in zip(cutouts, self._cutout_total_masks):
                 try:
                     centroid = centroid_quadratic(data, mask=mask,
                                                   fit_boxsize=3)
                 except ValueError:
                     centroid = (np.nan, np.nan)
                 centroid_quad.append(centroid)
@@ -2988,16 +2989,20 @@
         cxy = self.cxy.value
         cyy = self.cyy.value
         if self.isscalar:
             cxx = (cxx,)
             cxy = (cxy,)
             cyy = (cyy,)
 
+        labels = self.labels
+        if self.progress_bar:
+            desc = 'kron_radius'
+            labels = add_progress_bar(labels, desc=desc)  # pragma: no cover
+
         kron_radius = []
-        labels = self._progress_bar(self.labels, 'kron_radius')
         for (label, aperture, cxx_, cxy_, cyy_) in zip(labels, apertures,
                                                        cxx, cxy, cyy):
             if aperture is None:
                 kron_radius.append(np.nan)
                 continue
 
             xcen, ycen = aperture.positions
@@ -3288,17 +3293,20 @@
             ``to_mask`` method.
 
         Returns
         -------
         flux, fluxerr : 1D `~numpy.ndaray`
             The flux and flux error arrays.
         """
+        labels = self.labels
+        if self.progress_bar:
+            labels = add_progress_bar(labels, desc=desc)  # pragma: no cover
+
         flux = []
         fluxerr = []
-        labels = self._progress_bar(self.labels, desc=desc)
         for label, aperture, bkg in zip(labels, apertures,
                                         self._local_background):
             # return NaN for completely masked sources or sources where
             # the centroid is not finite
             if aperture is None:
                 flux.append(np.nan)
                 fluxerr.append(np.nan)
@@ -3516,16 +3524,20 @@
     @lazyproperty
     @use_detcat
     def _fluxfrac_optimizer_args(self):
         kron_flux = self._kron_photometry[:, 0]  # unitless
         max_radius = self._max_circular_kron_radius
         kwargs = self._apermask_kwargs['fluxfrac']
 
+        labels = self.labels
+        if self.progress_bar:
+            desc = 'fluxfrac_radius prep'
+            labels = add_progress_bar(labels, desc=desc)  # pragma: no cover
+
         args = []
-        labels = self._progress_bar(self.labels, 'fluxfrac_radius prep')
         for label, xcen, ycen, kronflux, bkg, max_radius_ in zip(
                 labels, self._xcentroid, self._ycentroid,
                 kron_flux, self._local_background, max_radius):
 
             if (np.any(~np.isfinite((xcen, ycen, kronflux, max_radius_)))
                     or kronflux == 0):
                 args.append(None)
@@ -3575,17 +3587,20 @@
             or where the Kron flux is zero or non-finite.
         """
         if fluxfrac <= 0 or fluxfrac > 1:
             raise ValueError('fluxfrac must be > 0 and <= 1')
 
         from scipy.optimize import root_scalar
 
+        args = self._fluxfrac_optimizer_args
+        if self.progress_bar:
+            desc = 'fluxfrac_radius'
+            args = add_progress_bar(args, desc=desc)  # pragma: no cover
+
         radius = []
-        args = self._progress_bar(self._fluxfrac_optimizer_args,
-                                  'fluxfrac_radius')
         for fluxfrac_args in args:
             if fluxfrac_args is None:
                 radius.append(np.nan)
                 continue
 
             max_radius = fluxfrac_args[-1]
             args = fluxfrac_args[:-1]
```

### Comparing `photutils-1.8.0/photutils/segmentation/core.py` & `photutils-1.9.0/photutils/segmentation/core.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/segmentation/deblend.py` & `photutils-1.9.0/photutils/segmentation/deblend.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import numpy as np
 from astropy.units import Quantity
 from astropy.utils.exceptions import AstropyUserWarning
 
 from photutils.segmentation.core import SegmentationImage
 from photutils.segmentation.detect import _detect_sources
 from photutils.segmentation.utils import _make_binary_structure
-from photutils.utils._optional_deps import HAS_TQDM
+from photutils.utils._progress_bars import add_progress_bar
 
 __all__ = ['deblend_sources']
 
 
 def deblend_sources(data, segment_img, npixels, *, labels=None, nlevels=32,
                     contrast=0.001, mode='exponential', connectivity=8,
                     relabel=True, nproc=1, progress_bar=True):
@@ -155,17 +155,14 @@
     labels = labels[mask]
 
     footprint = _make_binary_structure(data.ndim, connectivity)
 
     if nproc is None:
         nproc = cpu_count()  # pragma: no cover
 
-    if progress_bar and HAS_TQDM:
-        from tqdm.auto import tqdm  # pragma: no cover
-
     segm_deblended = object.__new__(SegmentationImage)
     segm_deblended._data = np.copy(segment_img.data)
     last_label = segment_img.max_label
     indices = segment_img.get_indices(labels)
 
     all_source_data = []
     all_source_segments = []
@@ -177,17 +174,17 @@
         source_segment._data = segment_img.data[source_slice]
         source_segment.keep_labels(label)  # include only one label
         all_source_data.append(source_data)
         all_source_segments.append(source_segment)
         all_source_slices.append(source_slice)
 
     if nproc == 1:
-        if progress_bar and HAS_TQDM:
-            all_source_data = tqdm(all_source_data,
-                                   desc='Deblending')  # pragma: no cover
+        if progress_bar:
+            desc = 'Deblending'
+            all_source_data = add_progress_bar(all_source_data, desc=desc)  # pragma: no cover
 
         all_source_deblends = []
         for source_data, source_segment in zip(all_source_data,
                                                all_source_segments):
             deblender = _Deblender(source_data, source_segment, npixels,
                                    footprint, nlevels, contrast, mode)
             source_deblended = deblender.deblend_source()
@@ -195,17 +192,18 @@
 
     else:
         nlabels = len(labels)
         args_all = zip(all_source_data, all_source_segments,
                        (npixels,) * nlabels, (footprint,) * nlabels,
                        (nlevels,) * nlabels, (contrast,) * nlabels,
                        (mode,) * nlabels)
-        if progress_bar and HAS_TQDM:
-            args_all = tqdm(args_all, total=nlabels,
-                            desc='Deblending')  # pragma: no cover
+
+        if progress_bar:
+            desc = 'Deblending'
+            args_all = add_progress_bar(args_all, total=nlabels, desc=desc)  # pragma: no cover
 
         with get_context('spawn').Pool(processes=nproc) as executor:
             all_source_deblends = executor.starmap(_deblend_source, args_all)
 
     nonposmin_labels = []
     nmarkers_labels = []
     for (label, source_deblended, source_slice) in zip(
```

### Comparing `photutils-1.8.0/photutils/segmentation/detect.py` & `photutils-1.9.0/photutils/segmentation/detect.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/segmentation/finder.py` & `photutils-1.9.0/photutils/segmentation/finder.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/segmentation/tests/test_catalog.py` & `photutils-1.9.0/photutils/segmentation/tests/test_catalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,16 @@
                                 make_noise_image, make_wcs)
 from photutils.segmentation.catalog import SourceCatalog
 from photutils.segmentation.core import SegmentationImage
 from photutils.segmentation.detect import detect_sources
 from photutils.segmentation.finder import SourceFinder
 from photutils.segmentation.utils import make_2dgaussian_kernel
 from photutils.utils._convolution import _filter_data
-from photutils.utils._optional_deps import HAS_GWCS, HAS_MATPLOTLIB, HAS_SCIPY
+from photutils.utils._optional_deps import (HAS_GWCS, HAS_MATPLOTLIB,
+                                            HAS_SCIPY, HAS_SKIMAGE)
 from photutils.utils.cutouts import CutoutImage
 
 
 @pytest.mark.skipif(not HAS_SCIPY, reason='scipy is required')
 class TestSourceCatalog:
     def setup_class(self):
         xcen = 51.0
@@ -772,14 +773,15 @@
         aper2 = self.cat.make_kron_apertures((2.0, 1.4))
         assert len(aper2) == len(self.cat)
 
         obj = self.cat[1]
         aper = obj.make_kron_apertures()
         assert isinstance(aper, EllipticalAperture)
 
+    @pytest.mark.skipif(not HAS_SKIMAGE, reason='skimage is required')
     def test_make_cutouts(self):
         data = make_100gaussians_image()
         bkg_estimator = MedianBackground()
         bkg = Background2D(data, (50, 50), filter_size=(3, 3),
                            bkg_estimator=bkg_estimator)
         data -= bkg.background  # subtract the background
         threshold = 1.5 * bkg.background_rms
@@ -831,14 +833,15 @@
     def test_semode(self):
         self.cat._set_semode()
         tbl = self.cat.to_table()
         assert len(tbl) == 7
 
 
 @pytest.mark.skipif(not HAS_SCIPY, reason='scipy is required')
+@pytest.mark.skipif(not HAS_SKIMAGE, reason='skimage is required')
 def test_kron_params():
     data = make_100gaussians_image()
     bkg_estimator = MedianBackground()
     bkg = Background2D(data, (50, 50), filter_size=(3, 3),
                        bkg_estimator=bkg_estimator)
     data -= bkg.background  # subtract the background
 
@@ -885,14 +888,15 @@
     assert_allclose(cat.kron_flux.min(), 246.91339096556538)
     rh = cat.fluxfrac_radius(0.5)
     assert_allclose(rh.value.min(), 1.3649418211298536)
     assert isinstance(cat.kron_aperture[0], CircularAperture)
 
 
 @pytest.mark.skipif(not HAS_SCIPY, reason='scipy is required')
+@pytest.mark.skipif(not HAS_SKIMAGE, reason='skimage is required')
 def test_centroid_win():
     g1 = Gaussian2D(1621, 6.29, 10.95, 1.55, 1.29, 0.296706)
     g2 = Gaussian2D(3596, 13.81, 8.29, 1.44, 1.27, 0.628319)
     m = g1 + g2
     yy, xx = np.mgrid[0:21, 0:21]
     data = m(xx, yy)
     noise = make_noise_image(data.shape, mean=0, stddev=65.0, seed=123)
```

### Comparing `photutils-1.8.0/photutils/segmentation/tests/test_core.py` & `photutils-1.9.0/photutils/segmentation/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/segmentation/tests/test_deblend.py` & `photutils-1.9.0/photutils/segmentation/tests/test_deblend.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/segmentation/tests/test_detect.py` & `photutils-1.9.0/photutils/segmentation/tests/test_detect.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/segmentation/tests/test_finder.py` & `photutils-1.9.0/photutils/segmentation/tests/test_finder.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/segmentation/tests/test_utils.py` & `photutils-1.9.0/photutils/segmentation/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/segmentation/utils.py` & `photutils-1.9.0/photutils/segmentation/utils.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/utils/_convolution.py` & `photutils-1.9.0/photutils/utils/_convolution.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/utils/_misc.py` & `photutils-1.9.0/photutils/utils/_misc.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/utils/_moments.py` & `photutils-1.9.0/photutils/utils/_moments.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/utils/_optional_deps.py` & `photutils-1.9.0/photutils/utils/_optional_deps.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/utils/_parameters.py` & `photutils-1.9.0/photutils/utils/_parameters.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/utils/_quantity_helpers.py` & `photutils-1.9.0/photutils/utils/_quantity_helpers.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/utils/_stats.py` & `photutils-1.9.0/photutils/utils/_stats.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/utils/_wcs_helpers.py` & `photutils-1.9.0/photutils/utils/_wcs_helpers.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/utils/colormaps.py` & `photutils-1.9.0/photutils/utils/colormaps.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/utils/cutouts.py` & `photutils-1.9.0/photutils/utils/cutouts.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/utils/depths.py` & `photutils-1.9.0/photutils/utils/depths.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,20 +6,19 @@
 import warnings
 
 import astropy.units as u
 import numpy as np
 from astropy.stats import SigmaClip
 from astropy.utils.exceptions import AstropyUserWarning
 
-# pylint: disable-next=E0611
-from photutils.utils._optional_deps import HAS_TQDM
+from photutils.utils._progress_bars import add_progress_bar
 from photutils.utils.footprints import circular_footprint
 
 __all__ = ['ImageDepth']
-__doctest_requires__ = {('ImageDepth', 'ImageDepth.*'): ['scipy']}
+__doctest_requires__ = {('ImageDepth', 'ImageDepth.*'): ['scipy', 'skimage']}
 
 
 class ImageDepth:
     r"""
     Class to calculate the limiting flux and magnitude of an image.
 
     Parameters
@@ -83,21 +82,22 @@
     apertures : list of `~photutils.aperture.CircularAperture`
         A list of circular apertures for each iteration.
 
     napers_used : int
         A list of the number of apertures used for each iteration.
 
     fluxes : list of `~numpy.ndarray`
-        A list of the flux measurements for each iteration.
+        A list of arrays containing the flux measurements for each
+        iteration.
 
-    flux_limits : list
-        A list of the flux limits for each iteration.
+    flux_limits : 1D `~numpy.ndarray`
+        An array of the flux limits for each iteration.
 
-    mag_limits : list
-        A list of the magnitude limits for each iteration.
+    mag_limits : 1D `~numpy.ndarray`
+        An array of the magnitude limits for each iteration.
 
     Notes
     -----
     The image depth is calculated by placing random circular apertures
     with the specified radius on blank regions of the image. The number
     of apertures is specified by the ``napers`` keyword. The blank
     regions are calculated from an input mask, which should mask both
@@ -240,34 +240,33 @@
             The flux and magnitude limits. The flux limit is returned in
             the same units as the input ``data``. The magnitude limit is
             calculated from the flux limit and the input ``zeropoint``.
         """
         # prevent circular import
         from photutils.aperture import CircularAperture
 
-        iter_range = range(self.niters)
-        if self.progress_bar and HAS_TQDM:
-            from tqdm.auto import tqdm  # pragma: no cover
-
-            iter_range = tqdm(iter_range, desc='Image Depths')  # pragma: no cover
-
         if mask is None or not np.any(mask):
             all_xycoords = self._make_all_coords_no_mask(data.shape)
         else:
             all_xycoords = self._make_all_coords(mask)
 
         if len(all_xycoords) == 0:
             raise ValueError('There are no unmasked pixel values (including '
                              'the masked image borders).')
 
         napers = self.napers
         if not self.overlap:
             napers2 = 1.5 * self.napers
             napers = int(min(napers2, 0.1 * len(all_xycoords)))
 
+        iter_range = range(self.niters)
+        if self.progress_bar:
+            desc = 'Image Depths'
+            iter_range = add_progress_bar(iter_range, desc=desc)  # pragma: no cover
+
         fluxes = []
         flux_limits = []
         apertures = []
         for _ in iter_range:
             if self.overlap:
                 xycoords = self._make_coords(all_xycoords, napers)
             else:
```

### Comparing `photutils-1.8.0/photutils/utils/errors.py` & `photutils-1.9.0/photutils/utils/errors.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/utils/footprints.py` & `photutils-1.9.0/photutils/utils/footprints.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/utils/interpolation.py` & `photutils-1.9.0/photutils/utils/interpolation.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/utils/tests/test_colormaps.py` & `photutils-1.9.0/photutils/utils/tests/test_colormaps.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/utils/tests/test_convolution.py` & `photutils-1.9.0/photutils/utils/tests/test_convolution.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/utils/tests/test_cutouts.py` & `photutils-1.9.0/photutils/utils/tests/test_cutouts.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/utils/tests/test_depths.py` & `photutils-1.9.0/photutils/utils/tests/test_depths.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,21 +11,22 @@
 from astropy.convolution import convolve
 from astropy.tests.helper import assert_quantity_allclose
 from astropy.utils.exceptions import AstropyUserWarning
 from numpy.testing import assert_allclose
 
 from photutils.datasets import make_100gaussians_image
 from photutils.segmentation import SourceFinder, make_2dgaussian_kernel
-from photutils.utils._optional_deps import HAS_SCIPY
+from photutils.utils._optional_deps import HAS_SCIPY, HAS_SKIMAGE
 from photutils.utils.depths import ImageDepth
 
 bool_vals = (True, False)
 
 
 @pytest.mark.skipif(not HAS_SCIPY, reason='scipy is required')
+@pytest.mark.skipif(not HAS_SKIMAGE, reason='skimage is required')
 class TestImageDepth:
     def setup_class(self):
         bkg = 5.0
         data = make_100gaussians_image() - bkg
         kernel = make_2dgaussian_kernel(3.0, size=5)
         convolved_data = convolve(data, kernel)
```

### Comparing `photutils-1.8.0/photutils/utils/tests/test_errors.py` & `photutils-1.9.0/photutils/utils/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/utils/tests/test_footprints.py` & `photutils-1.9.0/photutils/utils/tests/test_footprints.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/utils/tests/test_interpolation.py` & `photutils-1.9.0/photutils/utils/tests/test_interpolation.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/utils/tests/test_misc.py` & `photutils-1.9.0/photutils/utils/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/utils/tests/test_moments.py` & `photutils-1.9.0/photutils/utils/tests/test_moments.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/utils/tests/test_parameters.py` & `photutils-1.9.0/photutils/utils/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils/utils/tests/test_quantity_helpers.py` & `photutils-1.9.0/photutils/utils/tests/test_quantity_helpers.py`

 * *Files identical despite different names*

### Comparing `photutils-1.8.0/photutils.egg-info/PKG-INFO` & `photutils-1.9.0/photutils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: photutils
-Version: 1.8.0
+Version: 1.9.0
 Summary: An Astropy package for source detection and photometry
 Home-page: https://github.com/astropy/photutils
 Author: Photutils Developers
 Author-email: photutils.team@gmail.com
 License: BSD-3-Clause
 Keywords: astronomy,astrophysics,photometry,aperture,psf,source detection,background,segmentation,centroids,isophote,morphology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Astronomy
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Provides-Extra: all
 Provides-Extra: test
 Provides-Extra: docs
 License-File: LICENSE.rst
 
 =========
@@ -46,20 +46,20 @@
 
 If you use Photutils for a project that leads to a publication,
 whether directly or as a dependency of another package, please include
 the following acknowledgment::
 
     This research made use of Photutils, an Astropy package for
     detection and photometry of astronomical sources (Bradley et al.
-    20XX).
+    <YEAR>).
 
-where (Bradley et al. 20XX) is a citation to the `Zenodo record
-<https://doi.org/10.5281/zenodo.596036>`_ of the Photutils version
-that was used.  We also encourage citations in the main text wherever
-appropriate.  Please see the `CITATION
+where (Bradley et al. <YEAR>) is a citation to the `Zenodo record
+<https://doi.org/10.5281/zenodo.596036>`_ of the Photutils
+version that was used. We also encourage citations in the
+main text wherever appropriate. Please see the `CITATION
 <https://github.com/astropy/photutils/blob/main/photutils/CITATION.rst>`_
 file for details and an example BibTeX entry.
 
 
 License
 -------
```

### Comparing `photutils-1.8.0/photutils.egg-info/SOURCES.txt` & `photutils-1.9.0/photutils.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 .bandit.yaml
 .gitignore
-.lgtm.yml
 .pep8speaks.yml
 .pre-commit-config.yaml
 .readthedocs.yml
 CHANGES.rst
 CITATION.md
 CODE_OF_CONDUCT.rst
 CONTRIBUTING.rst
 LICENSE.rst
-MANIFEST.in
 README.rst
 codecov.yml
 pyproject.toml
 setup.cfg
 setup.py
 tox.ini
 ./photutils/geometry/circular_overlap.pyx
 ./photutils/geometry/core.pyx
 ./photutils/geometry/elliptical_overlap.pyx
 ./photutils/geometry/rectangular_overlap.pyx
-.circleci/config.yml
-.github/workflows/32bit_tests.yml
+.github/dependabot.yml
+.github/workflows/ci_cron_daily.yml
+.github/workflows/ci_cron_weekly.yml
 .github/workflows/ci_tests.yml
 .github/workflows/codeql.yml
-.github/workflows/cron_tests.yml
 .github/workflows/publish.yml
 docs/Makefile
 docs/aperture.rst
 docs/background.rst
 docs/centroids.rst
 docs/changelog.rst
 docs/citation.rst
@@ -48,15 +46,14 @@
 docs/make.bat
 docs/morphology.rst
 docs/overview.rst
 docs/pixel_conventions.rst
 docs/profiles.rst
 docs/psf.rst
 docs/psf_matching.rst
-docs/rtd_requirements.txt
 docs/segmentation.rst
 docs/test_function.rst
 docs/utils.rst
 docs/_static/favicon.ico
 docs/_static/photutils.css
 docs/_static/photutils_banner-475x120.png
 docs/_static/photutils_banner.pdf
@@ -81,14 +78,15 @@
 docs/whats_new/1.2.rst
 docs/whats_new/1.3.rst
 docs/whats_new/1.4.rst
 docs/whats_new/1.5.rst
 docs/whats_new/1.6.rst
 docs/whats_new/1.7.rst
 docs/whats_new/1.8.rst
+docs/whats_new/1.9.rst
 docs/whats_new/index.rst
 photutils/CITATION.rst
 photutils/__init__.py
 photutils/_astropy_init.py
 photutils/_compiler.c
 photutils/conftest.py
 photutils/version.py
@@ -117,17 +115,19 @@
 photutils/aperture/tests/test_photometry.py
 photutils/aperture/tests/test_rectangle.py
 photutils/aperture/tests/test_stats.py
 photutils/background/__init__.py
 photutils/background/background_2d.py
 photutils/background/core.py
 photutils/background/interpolators.py
+photutils/background/local_background.py
 photutils/background/tests/__init__.py
 photutils/background/tests/test_background_2d.py
 photutils/background/tests/test_core.py
+photutils/background/tests/test_local_background.py
 photutils/centroids/__init__.py
 photutils/centroids/core.py
 photutils/centroids/gaussian.py
 photutils/centroids/tests/__init__.py
 photutils/centroids/tests/test_core.py
 photutils/centroids/tests/test_gaussian.py
 photutils/datasets/__init__.py
@@ -211,31 +211,41 @@
 photutils/profiles/radial_profile.py
 photutils/profiles/tests/__init__.py
 photutils/profiles/tests/test_curve_of_growth.py
 photutils/profiles/tests/test_radial_profile.py
 photutils/psf/__init__.py
 photutils/psf/epsf.py
 photutils/psf/epsf_stars.py
+photutils/psf/griddedpsfmodel.py
+photutils/psf/groupers.py
 photutils/psf/groupstars.py
 photutils/psf/models.py
 photutils/psf/photometry.py
+photutils/psf/photometry_depr.py
 photutils/psf/utils.py
 photutils/psf/matching/__init__.py
 photutils/psf/matching/fourier.py
 photutils/psf/matching/windows.py
 photutils/psf/matching/tests/__init__.py
 photutils/psf/matching/tests/test_fourier.py
 photutils/psf/matching/tests/test_windows.py
 photutils/psf/tests/__init__.py
 photutils/psf/tests/test_epsf.py
 photutils/psf/tests/test_epsf_stars.py
+photutils/psf/tests/test_griddedpsfmodel.py
 photutils/psf/tests/test_groupstars.py
 photutils/psf/tests/test_models.py
+photutils/psf/tests/test_photometry-depr.py
 photutils/psf/tests/test_photometry.py
 photutils/psf/tests/test_utils.py
+photutils/psf/tests/data/STDPSF_ACSWFC_F814W_mock.fits
+photutils/psf/tests/data/STDPSF_NRCA1_F150W_mock.fits
+photutils/psf/tests/data/STDPSF_NRCSW_F150W_mock.fits
+photutils/psf/tests/data/STDPSF_WFC3UV_F814W_mock.fits
+photutils/psf/tests/data/STDPSF_WFPC2_F814W_mock.fits
 photutils/segmentation/__init__.py
 photutils/segmentation/catalog.py
 photutils/segmentation/core.py
 photutils/segmentation/deblend.py
 photutils/segmentation/detect.py
 photutils/segmentation/finder.py
 photutils/segmentation/utils.py
@@ -243,20 +253,22 @@
 photutils/segmentation/tests/test_catalog.py
 photutils/segmentation/tests/test_core.py
 photutils/segmentation/tests/test_deblend.py
 photutils/segmentation/tests/test_detect.py
 photutils/segmentation/tests/test_finder.py
 photutils/segmentation/tests/test_utils.py
 photutils/tests/__init__.py
+photutils/tests/helper.py
 photutils/utils/__init__.py
 photutils/utils/_convolution.py
 photutils/utils/_misc.py
 photutils/utils/_moments.py
 photutils/utils/_optional_deps.py
 photutils/utils/_parameters.py
+photutils/utils/_progress_bars.py
 photutils/utils/_quantity_helpers.py
 photutils/utils/_round.py
 photutils/utils/_stats.py
 photutils/utils/_wcs_helpers.py
 photutils/utils/colormaps.py
 photutils/utils/cutouts.py
 photutils/utils/depths.py
@@ -271,8 +283,9 @@
 photutils/utils/tests/test_depths.py
 photutils/utils/tests/test_errors.py
 photutils/utils/tests/test_footprints.py
 photutils/utils/tests/test_interpolation.py
 photutils/utils/tests/test_misc.py
 photutils/utils/tests/test_moments.py
 photutils/utils/tests/test_parameters.py
-photutils/utils/tests/test_quantity_helpers.py
+photutils/utils/tests/test_quantity_helpers.py
+photutils/utils/tests/test_round.py
```

### Comparing `photutils-1.8.0/setup.cfg` & `photutils-1.9.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -20,18 +20,17 @@
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Topic :: Scientific/Engineering :: Astronomy
 
 [options]
 zip_safe = False
 packages = find:
-python_requires = >=3.8
-setup_requires = setuptools_scm
+python_requires = >=3.9
 install_requires = 
-	numpy>=1.21
+	numpy>=1.22
 	astropy>=5.0
 
 [options.extras_require]
 all = 
 	scipy>=1.7.0
 	matplotlib>=3.5.0
 	scikit-image>=0.19.0
@@ -55,25 +54,28 @@
 	shapely
 
 [options.package_data]
 photutils = CITATION.rst
 photutils.datasets = data/*
 photutils.detection.tests = data/*
 photutils.isophote.tests = data/*
+photutils.psf.tests = data/*
 
 [tool:pytest]
+minversion = 7.0
 testpaths = "photutils" "docs"
 norecursedirs = 
 	"docs[\/]_build"
 	"docs[\/]generated"
 	"photutils[\/]extern"
 astropy_header = true
 doctest_plus = enabled
 text_file_format = rst
-addopts = --doctest-rst
+addopts = --color=yes --doctest-rst
+xfail_strict = true
 remote_data_strict = true
 filterwarnings = 
 	error
 	ignore:numpy\.ufunc size changed:RuntimeWarning
 	ignore:numpy\.ndarray size changed:RuntimeWarning
 	ignore:`np.bool8` is a deprecated alias for `np.bool_`:DeprecationWarning
```

### Comparing `photutils-1.8.0/setup.py` & `photutils-1.9.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -55,29 +55,14 @@
   http://docs.astropy.org/en/latest/install.html#builddocs
 """
 
 if 'build_docs' in sys.argv or 'build_sphinx' in sys.argv:
     print(DOCS_HELP)
     sys.exit(1)
 
-VERSION_TEMPLATE = """
-# Note that we need to fall back to the hard-coded version if either
-# setuptools_scm can't be imported or setuptools_scm can't determine the
-# version, so we catch the generic 'Exception'.
-try:
-    from setuptools_scm import get_version
-    version = get_version(root='..', relative_to=__file__)
-except Exception:
-    version = '{version}'
-""".lstrip()
-
-
 # Import these after the above checks to ensure they are printed even if
 # extensions_helpers is not installed
-import os  # noqa: E402
+from setuptools import setup  # noqa: E402
 
 from extension_helpers import get_extensions  # noqa: E402
-from setuptools import setup  # noqa: E402
 
-setup(use_scm_version={'write_to': os.path.join('photutils', 'version.py'),
-                       'write_to_template': VERSION_TEMPLATE},
-      ext_modules=get_extensions())
+setup(ext_modules=get_extensions())
```

### Comparing `photutils-1.8.0/tox.ini` & `photutils-1.9.0/tox.ini`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 [tox]
 envlist =
-    py{38,39,310,311}-test{,-alldeps,-devdeps,-oldestdeps}{,-cov}
-    py{38,39,310,311}-test-numpy{121,122,123,124}
-    py{38,39,310,311}-test-astropy{50,lts}
-    32bit
+    py{39,310,311}-test{,-alldeps,-devdeps,-oldestdeps,-devinfra}{,-cov}
+    py{39,310,311}-test-numpy{122,123,124,125}
+    py{39,310,311}-test-astropy{50,lts}
     build_docs
     linkcheck
     codestyle
     pep517
     bandit
 requires =
     setuptools >= 30.3.0
     pip >= 19.3.1
 isolated_build = true
 
 [testenv]
 # Suppress display of matplotlib plots generated during docs build
 setenv =
     MPLBACKEND=agg
-    devdeps: PIP_EXTRA_INDEX_URL = https://pypi.anaconda.org/scipy-wheels-nightly/simple
+    devdeps: PIP_EXTRA_INDEX_URL = https://pypi.anaconda.org/scientific-python-nightly-wheels/simple https://pypi.anaconda.org/astropy/simple
 
 # Pass through the following environment variables which may be needed
 # for the CI
 passenv = HOME,WINDIR,LC_ALL,LC_CTYPE,CC,CI
 
 # Run the tests in a temporary directory to make sure that we don't
 # import this package from the source tree
@@ -36,75 +35,76 @@
 #
 #     tox -l -v
 #
 description =
     run tests
     alldeps: with all optional dependencies
     devdeps: with the latest developer version of key dependencies
+    devinfra: like devdeps but also dev version of infrastructure
     oldestdeps: with the oldest supported version of key dependencies
     cov: and test coverage
-    numpy121: with numpy 1.21.*
     numpy122: with numpy 1.22.*
     numpy123: with numpy 1.23.*
     numpy124: with numpy 1.24.*
+    numpy125: with numpy 1.25.*
 
     astropy50: with astropy 5.0.*
     astropylts: with the latest astropy LTS
 
 # The following provides some specific pinnings for key packages
 deps =
-    32bit: numpy==1.21.*
-    32bit: git+https://github.com/astropy/astropy.git#egg=astropy
-
-    cov: coverage
-
-    numpy121: numpy==1.21.*
     numpy122: numpy==1.22.*
     numpy123: numpy==1.23.*
     numpy124: numpy==1.24.*
+    numpy125: numpy==1.25.*
 
     astropy50: astropy==5.0.*
     astropylts: astropy==5.0.*
 
-    oldestdeps: numpy==1.21
+    oldestdeps: numpy==1.22
     oldestdeps: astropy==5.0
     oldestdeps: scipy==1.7.0
     oldestdeps: matplotlib==3.5.0
     oldestdeps: scikit-image==0.19.0
     oldestdeps: scikit-learn==1.0
     oldestdeps: gwcs==0.18
     oldestdeps: pytest-astropy==0.10
 
     devdeps: numpy>=0.0.dev0
     devdeps: scipy>=0.0.dev0
+    devdeps: scikit-image>=0.0.dev0
+    devdeps: scikit-learn>=0.0.dev0
     devdeps: matplotlib>=0.0.dev0
+    devdeps: astropy>=0.0.dev0
     devdeps: git+https://github.com/spacetelescope/gwcs.git
 
+    # Latest developer version of infrastructure packages.
+    devinfra: git+https://github.com/pytest-dev/pytest.git
+    devinfra: git+https://github.com/astropy/extension-helpers.git
+    devinfra: git+https://github.com/astropy/pytest-doctestplus.git
+    devinfra: git+https://github.com/astropy/pytest-remotedata.git
+    devinfra: git+https://github.com/astropy/pytest-astropy-header.git
+    devinfra: git+https://github.com/astropy/pytest-arraydiff.git
+    devinfra: git+https://github.com/astropy/pytest-filter-subpackage.git
+    devinfra: git+https://github.com/matplotlib/pytest-mpl.git
+    devinfra: git+https://github.com/astropy/pytest-astropy.git
+
 # The following indicates which extras_require from setup.cfg will be
 # installed
 extras =
     test: test
     alldeps: all
     build_docs: docs
 
 commands =
-    devdeps: pip install -U -i https://pypi.anaconda.org/astropy/simple astropy --pre
-    devdeps: pip install -U -i https://pypi.anaconda.org/scipy-wheels-nightly/simple scikit-learn
     pip freeze
-    !cov: pytest --pyargs photutils {toxinidir}/docs {posargs}
-    cov: pytest --pyargs photutils {toxinidir}/docs --cov photutils --cov-config={toxinidir}/setup.cfg {posargs}
-    cov: coverage xml -o {toxinidir}/coverage.xml
 
-[testenv:32bit]
-changedir = .tmp/{envname}
-description = 32-bit tests
-extras = test
-commands =
-    pip freeze
-    !cov: pytest --pyargs photutils {toxinidir}/docs {posargs}
+    pytest --pyargs photutils {toxinidir}/docs \
+    cov: --cov photutils --cov-config={toxinidir}/setup.cfg --cov-report xml:{toxinidir}/coverage.xml \
+    {posargs}
 
 [testenv:build_docs]
 changedir = docs
 description = invoke sphinx-build to build the HTML docs
 extras = docs
 commands =
     pip freeze
```

