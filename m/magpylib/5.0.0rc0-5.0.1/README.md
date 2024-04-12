# Comparing `tmp/magpylib-5.0.0rc0.tar.gz` & `tmp/magpylib-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magpylib-5.0.0rc0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "magpylib-5.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `magpylib-5.0.0rc0.tar` & `magpylib-5.0.1.tar`

### file list

```diff
@@ -1,247 +1,248 @@
--rw-r--r--   0        0        0       20 2024-03-13 10:06:10.299513 magpylib-5.0.0rc0/.binder/apt.txt
--rw-r--r--   0        0        0      171 2024-03-13 10:06:10.299513 magpylib-5.0.0rc0/.binder/labconfig/default_setting_overrides.json
--rw-r--r--   0        0        0      207 2024-03-13 10:06:10.299513 magpylib-5.0.0rc0/.binder/postBuild
--rw-r--r--   0        0        0        8 2024-03-13 10:06:10.299513 magpylib-5.0.0rc0/.binder/requirements.txt
--rw-r--r--   0        0        0      187 2024-03-13 10:06:10.299513 magpylib-5.0.0rc0/.binder/start
--rw-r--r--   0        0        0     1562 2024-03-13 10:06:10.299513 magpylib-5.0.0rc0/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-r--r--   0        0        0      910 2024-03-13 10:06:10.299513 magpylib-5.0.0rc0/.github/ISSUE_TEMPLATE/feature_request.yaml
--rw-r--r--   0        0        0      573 2024-03-13 10:06:10.299513 magpylib-5.0.0rc0/.github/ISSUE_TEMPLATE/question_magnetics.yaml
--rw-r--r--   0        0        0       27 2024-03-13 10:06:10.299513 magpylib-5.0.0rc0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0       59 2024-03-13 10:06:10.299513 magpylib-5.0.0rc0/.github/codeql/codeql-config.yml
--rw-r--r--   0        0        0     1000 2024-03-13 10:06:10.299513 magpylib-5.0.0rc0/.github/workflows/codeql.yml
--rw-r--r--   0        0        0     2145 2024-03-13 10:06:10.299513 magpylib-5.0.0rc0/.github/workflows/python-app.yml
--rw-r--r--   0        0        0     1690 2024-03-13 10:06:10.299513 magpylib-5.0.0rc0/.gitignore
--rw-r--r--   0        0        0     1116 2024-03-13 10:06:10.299513 magpylib-5.0.0rc0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    16348 2024-03-13 10:06:10.299513 magpylib-5.0.0rc0/.pylintrc
--rw-r--r--   0        0        0      806 2024-03-13 10:06:10.299513 magpylib-5.0.0rc0/.readthedocs.yaml
--rw-r--r--   0        0        0    33215 2024-03-13 10:06:10.303513 magpylib-5.0.0rc0/CHANGELOG.md
--rw-r--r--   0        0        0     4790 2024-03-13 10:06:10.303513 magpylib-5.0.0rc0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     3287 2024-03-13 10:06:10.303513 magpylib-5.0.0rc0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1332 2024-03-13 10:06:10.303513 magpylib-5.0.0rc0/LICENSE
--rw-r--r--   0        0        0       68 2024-03-13 10:06:10.303513 magpylib-5.0.0rc0/MANIFEST.in
--rw-r--r--   0        0        0     6953 2024-03-13 10:06:10.303513 magpylib-5.0.0rc0/README.md
--rw-r--r--   0        0        0      602 2024-03-13 10:06:10.303513 magpylib-5.0.0rc0/docs/Makefile
--rw-r--r--   0        0        0     1720 2024-03-13 10:06:10.303513 magpylib-5.0.0rc0/docs/README.md
--rw-r--r--   0        0        0    40241 2024-03-13 10:06:10.303513 magpylib-5.0.0rc0/docs/_pages/docu/docu_graphics.md
--rw-r--r--   0        0        0      733 2024-03-13 10:06:10.303513 magpylib-5.0.0rc0/docs/_pages/docu/docu_index.md
--rw-r--r--   0        0        0    39520 2024-03-13 10:06:10.303513 magpylib-5.0.0rc0/docs/_pages/docu/docu_magpylib_api.md
--rw-r--r--   0        0        0    10878 2024-03-13 10:06:10.303513 magpylib-5.0.0rc0/docs/_pages/docu/docu_physics.md
--rw-r--r--   0        0        0     2687 2024-03-13 10:06:10.303513 magpylib-5.0.0rc0/docs/_pages/gallery/gallery_app_end_of_shaft.md
--rw-r--r--   0        0        0      477 2024-03-13 10:06:10.303513 magpylib-5.0.0rc0/docs/_pages/gallery/gallery_app_halbach.md
--rw-r--r--   0        0        0     4762 2024-03-13 10:06:10.303513 magpylib-5.0.0rc0/docs/_pages/gallery/gallery_app_helmholtz.md
--rw-r--r--   0        0        0      426 2024-03-13 10:06:10.303513 magpylib-5.0.0rc0/docs/_pages/gallery/gallery_app_scales.md
--rw-r--r--   0        0        0     5018 2024-03-13 10:06:10.303513 magpylib-5.0.0rc0/docs/_pages/gallery/gallery_index.md
--rw-r--r--   0        0        0     5938 2024-03-13 10:06:10.303513 magpylib-5.0.0rc0/docs/_pages/gallery/gallery_misc_compound.md
--rw-r--r--   0        0        0     5283 2024-03-13 10:06:10.303513 magpylib-5.0.0rc0/docs/_pages/gallery/gallery_misc_field_interpolation.md
--rw-r--r--   0        0        0      372 2024-03-13 10:06:10.303513 magpylib-5.0.0rc0/docs/_pages/gallery/gallery_misc_inhom.md
--rw-r--r--   0        0        0      367 2024-03-13 10:06:10.303513 magpylib-5.0.0rc0/docs/_pages/gallery/gallery_shapes_3d_models.md
--rw-r--r--   0        0        0     1297 2024-03-13 10:06:10.303513 magpylib-5.0.0rc0/docs/_pages/gallery/gallery_shapes_convex_hull.md
--rw-r--r--   0        0        0     3878 2024-03-13 10:06:10.303513 magpylib-5.0.0rc0/docs/_pages/gallery/gallery_shapes_pyvista.md
--rw-r--r--   0        0        0     6628 2024-03-13 10:06:10.303513 magpylib-5.0.0rc0/docs/_pages/gallery/gallery_shapes_superpos.md
--rw-r--r--   0        0        0     8369 2024-03-13 10:06:10.303513 magpylib-5.0.0rc0/docs/_pages/gallery/gallery_shapes_triangle.md
--rw-r--r--   0        0        0     8058 2024-03-13 10:06:10.303513 magpylib-5.0.0rc0/docs/_pages/gallery/gallery_tutorial_collection.md
--rw-r--r--   0        0        0     7509 2024-03-13 10:06:10.303513 magpylib-5.0.0rc0/docs/_pages/gallery/gallery_tutorial_custom.md
--rw-r--r--   0        0        0     7845 2024-03-13 10:06:10.303513 magpylib-5.0.0rc0/docs/_pages/gallery/gallery_tutorial_field_computation.md
--rw-r--r--   0        0        0    10548 2024-03-13 10:06:10.303513 magpylib-5.0.0rc0/docs/_pages/gallery/gallery_tutorial_modelling_magnets.md
--rw-r--r--   0        0        0     6804 2024-03-13 10:06:10.303513 magpylib-5.0.0rc0/docs/_pages/gallery/gallery_tutorial_paths.md
--rw-r--r--   0        0        0      394 2024-03-13 10:06:10.303513 magpylib-5.0.0rc0/docs/_pages/gallery/gallery_vis_animations.md
--rw-r--r--   0        0        0     3963 2024-03-13 10:06:10.303513 magpylib-5.0.0rc0/docs/_pages/gallery/gallery_vis_mpl_streamplot.md
--rw-r--r--   0        0        0     1657 2024-03-13 10:06:10.303513 magpylib-5.0.0rc0/docs/_pages/gallery/gallery_vis_pv_streamlines.md
--rw-r--r--   0        0        0      545 2024-03-13 10:06:10.303513 magpylib-5.0.0rc0/docs/_pages/gallery/gallery_vis_subplots.md
--rw-r--r--   0        0        0       89 2024-03-13 10:06:10.303513 magpylib-5.0.0rc0/docs/_pages/reso_changelog.md
--rw-r--r--   0        0        0      102 2024-03-13 10:06:10.303513 magpylib-5.0.0rc0/docs/_pages/reso_code_of_conduct.md
--rw-r--r--   0        0        0       95 2024-03-13 10:06:10.303513 magpylib-5.0.0rc0/docs/_pages/reso_contributing.md
--rw-r--r--   0        0        0     7718 2024-03-13 10:06:10.303513 magpylib-5.0.0rc0/docs/_pages/reso_get_started.md
--rw-r--r--   0        0        0      383 2024-03-13 10:06:10.303513 magpylib-5.0.0rc0/docs/_pages/reso_license.md
--rw-r--r--   0        0        0      279 2024-03-13 10:06:10.303513 magpylib-5.0.0rc0/docs/_pages/reso_site_notice.md
--rw-r--r--   0        0        0      252 2024-03-13 10:06:10.303513 magpylib-5.0.0rc0/docs/_static/custom.css
--rw-r--r--   0        0        0    21562 2024-03-13 10:06:10.303513 magpylib-5.0.0rc0/docs/_static/images/docu_classes_init_collection.png
--rw-r--r--   0        0        0    17761 2024-03-13 10:06:10.303513 magpylib-5.0.0rc0/docs/_static/images/docu_classes_init_cuboid.png
--rw-r--r--   0        0        0    20351 2024-03-13 10:06:10.303513 magpylib-5.0.0rc0/docs/_static/images/docu_classes_init_custom.png
--rw-r--r--   0        0        0    19925 2024-03-13 10:06:10.303513 magpylib-5.0.0rc0/docs/_static/images/docu_classes_init_cylinder.png
--rw-r--r--   0        0        0    26491 2024-03-13 10:06:10.303513 magpylib-5.0.0rc0/docs/_static/images/docu_classes_init_cylindersegment.png
--rw-r--r--   0        0        0    16339 2024-03-13 10:06:10.303513 magpylib-5.0.0rc0/docs/_static/images/docu_classes_init_dipole.png
--rw-r--r--   0        0        0    13734 2024-03-13 10:06:10.303513 magpylib-5.0.0rc0/docs/_static/images/docu_classes_init_global_local.png
--rw-r--r--   0        0        0    21266 2024-03-13 10:06:10.303513 magpylib-5.0.0rc0/docs/_static/images/docu_classes_init_line.png
--rw-r--r--   0        0        0    18823 2024-03-13 10:06:10.303513 magpylib-5.0.0rc0/docs/_static/images/docu_classes_init_loop.png
--rw-r--r--   0        0        0    20182 2024-03-13 10:06:10.303513 magpylib-5.0.0rc0/docs/_static/images/docu_classes_init_sensor.png
--rw-r--r--   0        0        0    19936 2024-03-13 10:06:10.303513 magpylib-5.0.0rc0/docs/_static/images/docu_classes_init_sphere.png
--rw-r--r--   0        0        0    23461 2024-03-13 10:06:10.303513 magpylib-5.0.0rc0/docs/_static/images/docu_classes_init_tetra.png
--rw-r--r--   0        0        0    21231 2024-03-13 10:06:10.303513 magpylib-5.0.0rc0/docs/_static/images/docu_classes_init_triangle.png
--rw-r--r--   0        0        0    27786 2024-03-13 10:06:10.307513 magpylib-5.0.0rc0/docs/_static/images/docu_classes_init_trimesh.png
--rw-r--r--   0        0        0   249417 2024-03-13 10:06:10.307513 magpylib-5.0.0rc0/docs/_static/images/docu_field_comp_flow.png
--rw-r--r--   0        0        0    18560 2024-03-13 10:06:10.307513 magpylib-5.0.0rc0/docs/_static/images/docu_field_superpos_cutout.png
--rw-r--r--   0        0        0    18079 2024-03-13 10:06:10.307513 magpylib-5.0.0rc0/docs/_static/images/docu_field_superpos_union.png
--rw-r--r--   0        0        0   236681 2024-03-13 10:06:10.307513 magpylib-5.0.0rc0/docs/_static/images/docu_index_icon_magpylib.png
--rw-r--r--   0        0        0    91437 2024-03-13 10:06:10.307513 magpylib-5.0.0rc0/docs/_static/images/docu_index_icon_magpylib_show.png
--rw-r--r--   0        0        0   319986 2024-03-13 10:06:10.307513 magpylib-5.0.0rc0/docs/_static/images/docu_index_icon_physics.png
--rw-r--r--   0        0        0    49387 2024-03-13 10:06:10.307513 magpylib-5.0.0rc0/docs/_static/images/docu_position_sketch.png
--rw-r--r--   0        0        0    13848 2024-03-13 10:06:10.307513 magpylib-5.0.0rc0/docs/_static/images/favicons/android-chrome-192x192.png
--rw-r--r--   0        0        0    59132 2024-03-13 10:06:10.311513 magpylib-5.0.0rc0/docs/_static/images/favicons/android-chrome-512x512.png
--rw-r--r--   0        0        0    12328 2024-03-13 10:06:10.311513 magpylib-5.0.0rc0/docs/_static/images/favicons/apple-touch-icon.png
--rw-r--r--   0        0        0      708 2024-03-13 10:06:10.311513 magpylib-5.0.0rc0/docs/_static/images/favicons/favicon-16x16.png
--rw-r--r--   0        0        0     1470 2024-03-13 10:06:10.311513 magpylib-5.0.0rc0/docs/_static/images/favicons/favicon-32x32.png
--rw-r--r--   0        0        0    15406 2024-03-13 10:06:10.311513 magpylib-5.0.0rc0/docs/_static/images/favicons/favicon.ico
--rw-r--r--   0        0        0    29951 2024-03-13 10:06:10.311513 magpylib-5.0.0rc0/docs/_static/images/gallery_icon_WIP.png
--rw-r--r--   0        0        0    36788 2024-03-13 10:06:10.311513 magpylib-5.0.0rc0/docs/_static/images/gallery_icon_app_end_of_shaft.png
--rw-r--r--   0        0        0   142838 2024-03-13 10:06:10.311513 magpylib-5.0.0rc0/docs/_static/images/gallery_icon_app_helmholtz.png
--rw-r--r--   0        0        0   126489 2024-03-13 10:06:10.311513 magpylib-5.0.0rc0/docs/_static/images/gallery_icon_ext_custom_quadrupole.png
--rw-r--r--   0        0        0    52664 2024-03-13 10:06:10.311513 magpylib-5.0.0rc0/docs/_static/images/gallery_icon_misc_compound.png
--rw-r--r--   0        0        0    19393 2024-03-13 10:06:10.311513 magpylib-5.0.0rc0/docs/_static/images/gallery_icon_misc_field_interpolation.png
--rw-r--r--   0        0        0    28378 2024-03-13 10:06:10.311513 magpylib-5.0.0rc0/docs/_static/images/gallery_icon_shapes_convex_hull.png
--rw-r--r--   0        0        0    26107 2024-03-13 10:06:10.311513 magpylib-5.0.0rc0/docs/_static/images/gallery_icon_shapes_pyvista.png
--rw-r--r--   0        0        0    16589 2024-03-13 10:06:10.311513 magpylib-5.0.0rc0/docs/_static/images/gallery_icon_shapes_superpos.png
--rw-r--r--   0        0        0    31361 2024-03-13 10:06:10.311513 magpylib-5.0.0rc0/docs/_static/images/gallery_icon_shapes_triangle.png
--rw-r--r--   0        0        0    49507 2024-03-13 10:06:10.311513 magpylib-5.0.0rc0/docs/_static/images/gallery_icon_tutorial_collection.png
--rw-r--r--   0        0        0   270663 2024-03-13 10:06:10.311513 magpylib-5.0.0rc0/docs/_static/images/gallery_icon_tutorial_custom.png
--rw-r--r--   0        0        0    37618 2024-03-13 10:06:10.311513 magpylib-5.0.0rc0/docs/_static/images/gallery_icon_tutorial_field_computation.png
--rw-r--r--   0        0        0    58417 2024-03-13 10:06:10.311513 magpylib-5.0.0rc0/docs/_static/images/gallery_icon_tutorial_modelling_magnets.png
--rw-r--r--   0        0        0    32221 2024-03-13 10:06:10.311513 magpylib-5.0.0rc0/docs/_static/images/gallery_icon_tutorial_paths.png
--rw-r--r--   0        0        0   133213 2024-03-13 10:06:10.315513 magpylib-5.0.0rc0/docs/_static/images/gallery_icon_viz_mpl_streamplot.png
--rw-r--r--   0        0        0   101122 2024-03-13 10:06:10.315513 magpylib-5.0.0rc0/docs/_static/images/gallery_icon_viz_pv_streamlines.png
--rw-r--r--   0        0        0   125215 2024-03-13 10:06:10.315513 magpylib-5.0.0rc0/docs/_static/images/gallery_tutorial_magnet_LDratio.png
--rw-r--r--   0        0        0   192104 2024-03-13 10:06:10.315513 magpylib-5.0.0rc0/docs/_static/images/gallery_tutorial_magnet_datasheet.png
--rw-r--r--   0        0        0   115449 2024-03-13 10:06:10.315513 magpylib-5.0.0rc0/docs/_static/images/gallery_tutorial_magnet_datasheet2.png
--rw-r--r--   0        0        0   105716 2024-03-13 10:06:10.315513 magpylib-5.0.0rc0/docs/_static/images/gallery_tutorial_magnet_fieldcomparison.png
--rw-r--r--   0        0        0    82273 2024-03-13 10:06:10.315513 magpylib-5.0.0rc0/docs/_static/images/gallery_tutorial_magnet_hysteresis.png
--rw-r--r--   0        0        0    60218 2024-03-13 10:06:10.319513 magpylib-5.0.0rc0/docs/_static/images/gallery_tutorial_magnet_table.png
--rw-r--r--   0        0        0    42153 2024-03-13 10:06:10.319513 magpylib-5.0.0rc0/docs/_static/images/getting_started_animation.png
--rw-r--r--   0        0        0   107905 2024-03-13 10:06:10.319513 magpylib-5.0.0rc0/docs/_static/images/getting_started_complex_shapes.png
--rw-r--r--   0        0        0   101291 2024-03-13 10:06:10.319513 magpylib-5.0.0rc0/docs/_static/images/getting_started_fundamentals1.png
--rw-r--r--   0        0        0   114836 2024-03-13 10:06:10.319513 magpylib-5.0.0rc0/docs/_static/images/getting_started_styles.png
--rw-r--r--   0        0        0   240757 2024-03-13 10:06:10.319513 magpylib-5.0.0rc0/docs/_static/images/index_flowchart.png
--rw-r--r--   0        0        0   323052 2024-03-13 10:06:10.319513 magpylib-5.0.0rc0/docs/_static/images/index_head.png
--rw-r--r--   0        0        0     7837 2024-03-13 10:06:10.319513 magpylib-5.0.0rc0/docs/_static/images/index_icon_academic.png
--rw-r--r--   0        0        0     5281 2024-03-13 10:06:10.319513 magpylib-5.0.0rc0/docs/_static/images/index_icon_contributing.png
--rw-r--r--   0        0        0     8741 2024-03-13 10:06:10.319513 magpylib-5.0.0rc0/docs/_static/images/index_icon_docu.png
--rw-r--r--   0        0        0    12683 2024-03-13 10:06:10.319513 magpylib-5.0.0rc0/docs/_static/images/index_icon_gallery.png
--rw-r--r--   0        0        0     9752 2024-03-13 10:06:10.323513 magpylib-5.0.0rc0/docs/_static/images/index_icon_getting_started.png
--rw-r--r--   0        0        0     7864 2024-03-13 10:06:10.323513 magpylib-5.0.0rc0/docs/_static/images/index_icon_github.png
--rw-r--r--   0        0        0   167515 2024-03-13 10:06:10.323513 magpylib-5.0.0rc0/docs/_static/images/magpylib_flag.png
--rw-r--r--   0        0        0    22705 2024-03-13 10:06:10.323513 magpylib-5.0.0rc0/docs/_static/images/magpylib_logo.png
--rw-r--r--   0        0        0   526695 2024-03-13 10:06:10.323513 magpylib-5.0.0rc0/docs/_static/videos/axis.mp4
--rw-r--r--   0        0        0     2970 2024-03-13 10:06:10.327513 magpylib-5.0.0rc0/docs/_static/webcode/copybutton.js
--rw-r--r--   0        0        0      447 2024-03-13 10:06:10.327513 magpylib-5.0.0rc0/docs/_static/webcode/summaryOpen.js
--rw-r--r--   0        0        0    10243 2024-03-13 10:06:10.327513 magpylib-5.0.0rc0/docs/conf.py
--rw-r--r--   0        0        0     2316 2024-03-13 10:06:10.327513 magpylib-5.0.0rc0/docs/index.md
--rw-r--r--   0        0        0     6715 2024-03-13 10:06:10.327513 magpylib-5.0.0rc0/docs/make.bat
--rw-r--r--   0        0        0     1919 2024-03-13 10:06:10.327513 magpylib-5.0.0rc0/magpylib/__init__.py
--rw-r--r--   0        0        0       11 2024-03-13 10:06:10.327513 magpylib-5.0.0rc0/magpylib/_src/__init__.py
--rw-r--r--   0        0        0       22 2024-03-13 10:06:10.327513 magpylib-5.0.0rc0/magpylib/_src/defaults/__init__.py
--rw-r--r--   0        0        0     9448 2024-03-13 10:06:10.327513 magpylib-5.0.0rc0/magpylib/_src/defaults/defaults_classes.py
--rw-r--r--   0        0        0    13989 2024-03-13 10:06:10.327513 magpylib-5.0.0rc0/magpylib/_src/defaults/defaults_utility.py
--rw-r--r--   0        0        0     5981 2024-03-13 10:06:10.327513 magpylib-5.0.0rc0/magpylib/_src/defaults/defaults_values.py
--rw-r--r--   0        0        0       22 2024-03-13 10:06:10.327513 magpylib-5.0.0rc0/magpylib/_src/display/__init__.py
--rw-r--r--   0        0        0    14530 2024-03-13 10:06:10.327513 magpylib-5.0.0rc0/magpylib/_src/display/backend_matplotlib.py
--rw-r--r--   0        0        0    10746 2024-03-13 10:06:10.327513 magpylib-5.0.0rc0/magpylib/_src/display/backend_plotly.py
--rw-r--r--   0        0        0    12228 2024-03-13 10:06:10.327513 magpylib-5.0.0rc0/magpylib/_src/display/backend_pyvista.py
--rw-r--r--   0        0        0    17456 2024-03-13 10:06:10.327513 magpylib-5.0.0rc0/magpylib/_src/display/display.py
--rw-r--r--   0        0        0    11170 2024-03-13 10:06:10.327513 magpylib-5.0.0rc0/magpylib/_src/display/sensor_mesh.py
--rw-r--r--   0        0        0    21819 2024-03-13 10:06:10.327513 magpylib-5.0.0rc0/magpylib/_src/display/traces_base.py
--rw-r--r--   0        0        0    22486 2024-03-13 10:06:10.327513 magpylib-5.0.0rc0/magpylib/_src/display/traces_core.py
--rw-r--r--   0        0        0    33281 2024-03-13 10:06:10.327513 magpylib-5.0.0rc0/magpylib/_src/display/traces_generic.py
--rw-r--r--   0        0        0    26148 2024-03-13 10:06:10.327513 magpylib-5.0.0rc0/magpylib/_src/display/traces_utility.py
--rw-r--r--   0        0        0      458 2024-03-13 10:06:10.327513 magpylib-5.0.0rc0/magpylib/_src/exceptions.py
--rw-r--r--   0        0        0      312 2024-03-13 10:06:10.327513 magpylib-5.0.0rc0/magpylib/_src/fields/__init__.py
--rw-r--r--   0        0        0     3696 2024-03-13 10:06:10.327513 magpylib-5.0.0rc0/magpylib/_src/fields/field_BH_circle.py
--rw-r--r--   0        0        0     8994 2024-03-13 10:06:10.327513 magpylib-5.0.0rc0/magpylib/_src/fields/field_BH_cuboid.py
--rw-r--r--   0        0        0    11016 2024-03-13 10:06:10.327513 magpylib-5.0.0rc0/magpylib/_src/fields/field_BH_cylinder.py
--rw-r--r--   0        0        0    77680 2024-03-13 10:06:10.327513 magpylib-5.0.0rc0/magpylib/_src/fields/field_BH_cylinder_segment.py
--rw-r--r--   0        0        0     2360 2024-03-13 10:06:10.327513 magpylib-5.0.0rc0/magpylib/_src/fields/field_BH_dipole.py
--rw-r--r--   0        0        0     7223 2024-03-13 10:06:10.327513 magpylib-5.0.0rc0/magpylib/_src/fields/field_BH_polyline.py
--rw-r--r--   0        0        0     2762 2024-03-13 10:06:10.327513 magpylib-5.0.0rc0/magpylib/_src/fields/field_BH_sphere.py
--rw-r--r--   0        0        0     3775 2024-03-13 10:06:10.327513 magpylib-5.0.0rc0/magpylib/_src/fields/field_BH_tetrahedron.py
--rw-r--r--   0        0        0     6453 2024-03-13 10:06:10.327513 magpylib-5.0.0rc0/magpylib/_src/fields/field_BH_triangle.py
--rw-r--r--   0        0        0    19051 2024-03-13 10:06:10.327513 magpylib-5.0.0rc0/magpylib/_src/fields/field_BH_triangularmesh.py
--rw-r--r--   0        0        0    48295 2024-03-13 10:06:10.327513 magpylib-5.0.0rc0/magpylib/_src/fields/field_wrap_BH.py
--rw-r--r--   0        0        0     4396 2024-03-13 10:06:10.327513 magpylib-5.0.0rc0/magpylib/_src/fields/special_cel.py
--rw-r--r--   0        0        0    17650 2024-03-13 10:06:10.327513 magpylib-5.0.0rc0/magpylib/_src/fields/special_el3.py
--rw-r--r--   0        0        0    20724 2024-03-13 10:06:10.327513 magpylib-5.0.0rc0/magpylib/_src/input_checks.py
--rw-r--r--   0        0        0       23 2024-03-13 10:06:10.327513 magpylib-5.0.0rc0/magpylib/_src/obj_classes/__init__.py
--rw-r--r--   0        0        0     4090 2024-03-13 10:06:10.327513 magpylib-5.0.0rc0/magpylib/_src/obj_classes/class_BaseDisplayRepr.py
--rw-r--r--   0        0        0    19372 2024-03-13 10:06:10.327513 magpylib-5.0.0rc0/magpylib/_src/obj_classes/class_BaseExcitations.py
--rw-r--r--   0        0        0    12717 2024-03-13 10:06:10.327513 magpylib-5.0.0rc0/magpylib/_src/obj_classes/class_BaseGeo.py
--rw-r--r--   0        0        0    34491 2024-03-13 10:06:10.327513 magpylib-5.0.0rc0/magpylib/_src/obj_classes/class_BaseTransform.py
--rw-r--r--   0        0        0    35904 2024-03-13 10:06:10.327513 magpylib-5.0.0rc0/magpylib/_src/obj_classes/class_Collection.py
--rw-r--r--   0        0        0    18854 2024-03-13 10:06:10.327513 magpylib-5.0.0rc0/magpylib/_src/obj_classes/class_Sensor.py
--rw-r--r--   0        0        0     5043 2024-03-13 10:06:10.327513 magpylib-5.0.0rc0/magpylib/_src/obj_classes/class_current_Circle.py
--rw-r--r--   0        0        0     5456 2024-03-13 10:06:10.327513 magpylib-5.0.0rc0/magpylib/_src/obj_classes/class_current_Polyline.py
--rw-r--r--   0        0        0     4421 2024-03-13 10:06:10.327513 magpylib-5.0.0rc0/magpylib/_src/obj_classes/class_magnet_Cuboid.py
--rw-r--r--   0        0        0     5006 2024-03-13 10:06:10.327513 magpylib-5.0.0rc0/magpylib/_src/obj_classes/class_magnet_Cylinder.py
--rw-r--r--   0        0        0     6828 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/magpylib/_src/obj_classes/class_magnet_CylinderSegment.py
--rw-r--r--   0        0        0     4681 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/magpylib/_src/obj_classes/class_magnet_Sphere.py
--rw-r--r--   0        0        0     6030 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/magpylib/_src/obj_classes/class_magnet_Tetrahedron.py
--rw-r--r--   0        0        0    36933 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/magpylib/_src/obj_classes/class_magnet_TriangularMesh.py
--rw-r--r--   0        0        0     3520 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/magpylib/_src/obj_classes/class_misc_CustomSource.py
--rw-r--r--   0        0        0     4530 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/magpylib/_src/obj_classes/class_misc_Dipole.py
--rw-r--r--   0        0        0     5934 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/magpylib/_src/obj_classes/class_misc_Triangle.py
--rw-r--r--   0        0        0    77585 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/magpylib/_src/style.py
--rw-r--r--   0        0        0    12334 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/magpylib/_src/utility.py
--rw-r--r--   0        0        0     1048 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/magpylib/core/__init__.py
--rw-r--r--   0        0        0      398 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/magpylib/current/__init__.py
--rw-r--r--   0        0        0      260 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/magpylib/graphics/__init__.py
--rw-r--r--   0        0        0      835 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/magpylib/graphics/model3d/__init__.py
--rw-r--r--   0        0        0      353 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/magpylib/graphics/style/__init__.py
--rw-r--r--   0        0        0      632 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/magpylib/magnet/__init__.py
--rw-r--r--   0        0        0      335 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/magpylib/misc/__init__.py
--rw-r--r--   0        0        0     2332 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/pyproject.toml
--rw-r--r--   0        0        0       14 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/tests/__init__.py
--rw-r--r--   0        0        0    25344 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/tests/test_BHMJ_level.py
--rw-r--r--   0        0        0     7672 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/tests/test_BaseTransform.py
--rw-r--r--   0        0        0     5503 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/tests/test_Coumpound_setters.py
--rw-r--r--   0        0        0     2035 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/tests/test_CustomSource.py
--rw-r--r--   0        0        0      760 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/tests/test__missing_optional_modules.py
--rw-r--r--   0        0        0      465 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/tests/test_core.py
--rw-r--r--   0        0        0    17752 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/tests/test_core_physics_consistency.py
--rw-r--r--   0        0        0     7060 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/tests/test_default_utils.py
--rw-r--r--   0        0        0    10824 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/tests/test_defaults.py
--rw-r--r--   0        0        0    21282 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/tests/test_display_matplotlib.py
--rw-r--r--   0        0        0    13771 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/tests/test_display_plotly.py
--rw-r--r--   0        0        0     4507 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/tests/test_display_pyvista.py
--rw-r--r--   0        0        0     3181 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/tests/test_display_utility.py
--rw-r--r--   0        0        0     3453 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/tests/test_elliptics.py
--rw-r--r--   0        0        0     8864 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/tests/test_exceptions.py
--rw-r--r--   0        0        0    15385 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/tests/test_field_cylinder.py
--rw-r--r--   0        0        0    13402 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/tests/test_getBH_dict.py
--rw-r--r--   0        0        0    12328 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/tests/test_getBH_interfaces.py
--rw-r--r--   0        0        0    19579 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/tests/test_getBH_level2.py
--rw-r--r--   0        0        0    25249 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/tests/test_input_checks.py
--rw-r--r--   0        0        0      346 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/tests/test_misc.py
--rw-r--r--   0        0        0      737 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/tests/test_numerical_stability.py
--rw-r--r--   0        0        0    20450 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/tests/test_obj_BaseGeo.py
--rw-r--r--   0        0        0    12300 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/tests/test_obj_BaseGeo_v4motion.py
--rw-r--r--   0        0        0     2208 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/tests/test_obj_Circle.py
--rw-r--r--   0        0        0    15445 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/tests/test_obj_Collection.py
--rw-r--r--   0        0        0    10301 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/tests/test_obj_Collection_child_parent.py
--rw-r--r--   0        0        0    25232 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/tests/test_obj_Collection_v4motion.py
--rw-r--r--   0        0        0     4516 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/tests/test_obj_Cuboid.py
--rw-r--r--   0        0        0     4140 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/tests/test_obj_Cylinder.py
--rw-r--r--   0        0        0     1087 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/tests/test_obj_CylinderSegment.py
--rw-r--r--   0        0        0     1038 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/tests/test_obj_Dipole.py
--rw-r--r--   0        0        0     3787 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/tests/test_obj_Polyline.py
--rw-r--r--   0        0        0     3719 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/tests/test_obj_Sensor.py
--rw-r--r--   0        0        0     3105 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/tests/test_obj_Sphere.py
--rw-r--r--   0        0        0     2467 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/tests/test_obj_Tetrahedron.py
--rw-r--r--   0        0        0     2446 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/tests/test_obj_Triangle.py
--rw-r--r--   0        0        0    16212 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/tests/test_obj_TriangularMesh.py
--rw-r--r--   0        0        0     1654 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/tests/test_path.py
--rw-r--r--   0        0        0    10338 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/tests/test_physics_consistency.py
--rw-r--r--   0        0        0      661 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/tests/test_scaling.py
--rw-r--r--   0        0        0     2633 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/tests/test_utility.py
--rw-r--r--   0        0        0     2966 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/tests/test_vs_mag2.py
--rw-r--r--   0        0        0    14641 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/tests/testdata/testdata_Collection.p
--rw-r--r--   0        0        0     1568 2024-03-13 10:06:10.331513 magpylib-5.0.0rc0/tests/testdata/testdata_Collection_setter.npy
--rw-r--r--   0        0        0  1747640 2024-03-13 10:06:10.343513 magpylib-5.0.0rc0/tests/testdata/testdata_Cuboid.p
--rw-r--r--   0        0        0  1746038 2024-03-13 10:06:10.351513 magpylib-5.0.0rc0/tests/testdata/testdata_Sphere.p
--rw-r--r--   0        0        0    17225 2024-03-13 10:06:10.351513 magpylib-5.0.0rc0/tests/testdata/testdata_compound_setter_cases.npy
--rw-r--r--   0        0        0  1095577 2024-03-13 10:06:10.359513 magpylib-5.0.0rc0/tests/testdata/testdata_cy_cases.npy
--rw-r--r--   0        0        0   320128 2024-03-13 10:06:10.359513 magpylib-5.0.0rc0/tests/testdata/testdata_el3.npy
--rw-r--r--   0        0        0  1534592 2024-03-13 10:06:10.363513 magpylib-5.0.0rc0/tests/testdata/testdata_el3_angle.npy
--rw-r--r--   0        0        0    13056 2024-03-13 10:06:10.363513 magpylib-5.0.0rc0/tests/testdata/testdata_femDat_cylinder_tile2.npy
--rw-r--r--   0        0        0   102475 2024-03-13 10:06:10.363513 magpylib-5.0.0rc0/tests/testdata/testdata_field_BH_cuboid.p
--rw-r--r--   0        0        0   240606 2024-03-13 10:06:10.363513 magpylib-5.0.0rc0/tests/testdata/testdata_field_BH_cylinder.p
--rw-r--r--   0        0        0     9728 2024-03-13 10:06:10.363513 magpylib-5.0.0rc0/tests/testdata/testdata_full_cyl.npy
--rw-r--r--   0        0        0     1022 2024-03-13 10:06:10.363513 magpylib-5.0.0rc0/tests/testdata/testdata_path_BaseGeo.p
--rw-r--r--   0        0        0     7362 2024-03-13 10:06:10.363513 magpylib-5.0.0rc0/tests/testdata/testdata_vs_mag2.p
--rw-r--r--   0        0        0      606 2024-03-13 10:06:10.363513 magpylib-5.0.0rc0/tox.ini
--rw-r--r--   0        0        0     9413 1970-01-01 00:00:00.000000 magpylib-5.0.0rc0/PKG-INFO
+-rw-r--r--   0        0        0       20 2024-04-12 06:52:54.515146 magpylib-5.0.1/.binder/apt.txt
+-rw-r--r--   0        0        0      171 2024-04-12 06:52:54.515146 magpylib-5.0.1/.binder/labconfig/default_setting_overrides.json
+-rw-r--r--   0        0        0      207 2024-04-12 06:52:54.515146 magpylib-5.0.1/.binder/postBuild
+-rw-r--r--   0        0        0        8 2024-04-12 06:52:54.515146 magpylib-5.0.1/.binder/requirements.txt
+-rw-r--r--   0        0        0      187 2024-04-12 06:52:54.515146 magpylib-5.0.1/.binder/start
+-rw-r--r--   0        0        0     1562 2024-04-12 06:52:54.515146 magpylib-5.0.1/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0        0        0      910 2024-04-12 06:52:54.515146 magpylib-5.0.1/.github/ISSUE_TEMPLATE/feature_request.yaml
+-rw-r--r--   0        0        0      573 2024-04-12 06:52:54.515146 magpylib-5.0.1/.github/ISSUE_TEMPLATE/question_magnetics.yaml
+-rw-r--r--   0        0        0       27 2024-04-12 06:52:54.515146 magpylib-5.0.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0       59 2024-04-12 06:52:54.515146 magpylib-5.0.1/.github/codeql/codeql-config.yml
+-rw-r--r--   0        0        0     1000 2024-04-12 06:52:54.515146 magpylib-5.0.1/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0     2145 2024-04-12 06:52:54.515146 magpylib-5.0.1/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0     1690 2024-04-12 06:52:54.515146 magpylib-5.0.1/.gitignore
+-rw-r--r--   0        0        0     1116 2024-04-12 06:52:54.515146 magpylib-5.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    16348 2024-04-12 06:52:54.515146 magpylib-5.0.1/.pylintrc
+-rw-r--r--   0        0        0      806 2024-04-12 06:52:54.515146 magpylib-5.0.1/.readthedocs.yaml
+-rw-r--r--   0        0        0    33573 2024-04-12 06:52:54.515146 magpylib-5.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0     4790 2024-04-12 06:52:54.515146 magpylib-5.0.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3287 2024-04-12 06:52:54.515146 magpylib-5.0.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1332 2024-04-12 06:52:54.515146 magpylib-5.0.1/LICENSE
+-rw-r--r--   0        0        0       68 2024-04-12 06:52:54.515146 magpylib-5.0.1/MANIFEST.in
+-rw-r--r--   0        0        0     6947 2024-04-12 06:52:54.519146 magpylib-5.0.1/README.md
+-rw-r--r--   0        0        0      602 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/Makefile
+-rw-r--r--   0        0        0     1720 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/README.md
+-rw-r--r--   0        0        0    40241 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/docu/docu_graphics.md
+-rw-r--r--   0        0        0      733 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/docu/docu_index.md
+-rw-r--r--   0        0        0    39553 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/docu/docu_magpylib_api.md
+-rw-r--r--   0        0        0    10878 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/docu/docu_physics.md
+-rw-r--r--   0        0        0     2687 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/gallery/gallery_app_end_of_shaft.md
+-rw-r--r--   0        0        0      477 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/gallery/gallery_app_halbach.md
+-rw-r--r--   0        0        0     4757 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/gallery/gallery_app_helmholtz.md
+-rw-r--r--   0        0        0      426 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/gallery/gallery_app_scales.md
+-rw-r--r--   0        0        0     5029 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/gallery/gallery_index.md
+-rw-r--r--   0        0        0     5938 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/gallery/gallery_misc_compound.md
+-rw-r--r--   0        0        0     5283 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/gallery/gallery_misc_field_interpolation.md
+-rw-r--r--   0        0        0      372 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/gallery/gallery_misc_inhom.md
+-rw-r--r--   0        0        0      367 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/gallery/gallery_shapes_3d_models.md
+-rw-r--r--   0        0        0     1297 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/gallery/gallery_shapes_convex_hull.md
+-rw-r--r--   0        0        0     3878 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/gallery/gallery_shapes_pyvista.md
+-rw-r--r--   0        0        0     6628 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/gallery/gallery_shapes_superpos.md
+-rw-r--r--   0        0        0     8369 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/gallery/gallery_shapes_triangle.md
+-rw-r--r--   0        0        0     8058 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/gallery/gallery_tutorial_collection.md
+-rw-r--r--   0        0        0     7509 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/gallery/gallery_tutorial_custom.md
+-rw-r--r--   0        0        0     7845 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/gallery/gallery_tutorial_field_computation.md
+-rw-r--r--   0        0        0    10548 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/gallery/gallery_tutorial_modelling_magnets.md
+-rw-r--r--   0        0        0     6804 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/gallery/gallery_tutorial_paths.md
+-rw-r--r--   0        0        0     1313 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/gallery/gallery_vis_animations.md
+-rw-r--r--   0        0        0     4091 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/gallery/gallery_vis_mpl_streamplot.md
+-rw-r--r--   0        0        0     1657 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/gallery/gallery_vis_pv_streamlines.md
+-rw-r--r--   0        0        0      545 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/gallery/gallery_vis_subplots.md
+-rw-r--r--   0        0        0       89 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/reso_changelog.md
+-rw-r--r--   0        0        0      102 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/reso_code_of_conduct.md
+-rw-r--r--   0        0        0       95 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/reso_contributing.md
+-rw-r--r--   0        0        0     7718 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/reso_get_started.md
+-rw-r--r--   0        0        0      383 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/reso_license.md
+-rw-r--r--   0        0        0      279 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/reso_site_notice.md
+-rw-r--r--   0        0        0      252 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_static/custom.css
+-rw-r--r--   0        0        0    21562 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_static/images/docu_classes_init_collection.png
+-rw-r--r--   0        0        0    17761 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_static/images/docu_classes_init_cuboid.png
+-rw-r--r--   0        0        0    20351 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_static/images/docu_classes_init_custom.png
+-rw-r--r--   0        0        0    19925 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_static/images/docu_classes_init_cylinder.png
+-rw-r--r--   0        0        0    26491 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_static/images/docu_classes_init_cylindersegment.png
+-rw-r--r--   0        0        0    16339 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_static/images/docu_classes_init_dipole.png
+-rw-r--r--   0        0        0    13734 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_static/images/docu_classes_init_global_local.png
+-rw-r--r--   0        0        0    21266 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_static/images/docu_classes_init_line.png
+-rw-r--r--   0        0        0    18823 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_static/images/docu_classes_init_loop.png
+-rw-r--r--   0        0        0    20182 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_static/images/docu_classes_init_sensor.png
+-rw-r--r--   0        0        0    19936 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_static/images/docu_classes_init_sphere.png
+-rw-r--r--   0        0        0    23461 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_static/images/docu_classes_init_tetra.png
+-rw-r--r--   0        0        0    21231 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_static/images/docu_classes_init_triangle.png
+-rw-r--r--   0        0        0    27786 2024-04-12 06:52:54.523146 magpylib-5.0.1/docs/_static/images/docu_classes_init_trimesh.png
+-rw-r--r--   0        0        0   249417 2024-04-12 06:52:54.523146 magpylib-5.0.1/docs/_static/images/docu_field_comp_flow.png
+-rw-r--r--   0        0        0    18560 2024-04-12 06:52:54.523146 magpylib-5.0.1/docs/_static/images/docu_field_superpos_cutout.png
+-rw-r--r--   0        0        0    18079 2024-04-12 06:52:54.523146 magpylib-5.0.1/docs/_static/images/docu_field_superpos_union.png
+-rw-r--r--   0        0        0   236681 2024-04-12 06:52:54.523146 magpylib-5.0.1/docs/_static/images/docu_index_icon_magpylib.png
+-rw-r--r--   0        0        0    91437 2024-04-12 06:52:54.523146 magpylib-5.0.1/docs/_static/images/docu_index_icon_magpylib_show.png
+-rw-r--r--   0        0        0   319986 2024-04-12 06:52:54.523146 magpylib-5.0.1/docs/_static/images/docu_index_icon_physics.png
+-rw-r--r--   0        0        0    49387 2024-04-12 06:52:54.523146 magpylib-5.0.1/docs/_static/images/docu_position_sketch.png
+-rw-r--r--   0        0        0    13848 2024-04-12 06:52:54.523146 magpylib-5.0.1/docs/_static/images/favicons/android-chrome-192x192.png
+-rw-r--r--   0        0        0    59132 2024-04-12 06:52:54.527146 magpylib-5.0.1/docs/_static/images/favicons/android-chrome-512x512.png
+-rw-r--r--   0        0        0    12328 2024-04-12 06:52:54.527146 magpylib-5.0.1/docs/_static/images/favicons/apple-touch-icon.png
+-rw-r--r--   0        0        0      708 2024-04-12 06:52:54.527146 magpylib-5.0.1/docs/_static/images/favicons/favicon-16x16.png
+-rw-r--r--   0        0        0     1470 2024-04-12 06:52:54.527146 magpylib-5.0.1/docs/_static/images/favicons/favicon-32x32.png
+-rw-r--r--   0        0        0    15406 2024-04-12 06:52:54.527146 magpylib-5.0.1/docs/_static/images/favicons/favicon.ico
+-rw-r--r--   0        0        0    29951 2024-04-12 06:52:54.527146 magpylib-5.0.1/docs/_static/images/gallery_icon_WIP.png
+-rw-r--r--   0        0        0    36788 2024-04-12 06:52:54.527146 magpylib-5.0.1/docs/_static/images/gallery_icon_app_end_of_shaft.png
+-rw-r--r--   0        0        0   142838 2024-04-12 06:52:54.527146 magpylib-5.0.1/docs/_static/images/gallery_icon_app_helmholtz.png
+-rw-r--r--   0        0        0   126489 2024-04-12 06:52:54.527146 magpylib-5.0.1/docs/_static/images/gallery_icon_ext_custom_quadrupole.png
+-rw-r--r--   0        0        0    52664 2024-04-12 06:52:54.527146 magpylib-5.0.1/docs/_static/images/gallery_icon_misc_compound.png
+-rw-r--r--   0        0        0    19393 2024-04-12 06:52:54.527146 magpylib-5.0.1/docs/_static/images/gallery_icon_misc_field_interpolation.png
+-rw-r--r--   0        0        0    28378 2024-04-12 06:52:54.527146 magpylib-5.0.1/docs/_static/images/gallery_icon_shapes_convex_hull.png
+-rw-r--r--   0        0        0    26107 2024-04-12 06:52:54.527146 magpylib-5.0.1/docs/_static/images/gallery_icon_shapes_pyvista.png
+-rw-r--r--   0        0        0    16589 2024-04-12 06:52:54.527146 magpylib-5.0.1/docs/_static/images/gallery_icon_shapes_superpos.png
+-rw-r--r--   0        0        0    31361 2024-04-12 06:52:54.527146 magpylib-5.0.1/docs/_static/images/gallery_icon_shapes_triangle.png
+-rw-r--r--   0        0        0    49507 2024-04-12 06:52:54.527146 magpylib-5.0.1/docs/_static/images/gallery_icon_tutorial_collection.png
+-rw-r--r--   0        0        0   270663 2024-04-12 06:52:54.527146 magpylib-5.0.1/docs/_static/images/gallery_icon_tutorial_custom.png
+-rw-r--r--   0        0        0    37618 2024-04-12 06:52:54.527146 magpylib-5.0.1/docs/_static/images/gallery_icon_tutorial_field_computation.png
+-rw-r--r--   0        0        0    58417 2024-04-12 06:52:54.531146 magpylib-5.0.1/docs/_static/images/gallery_icon_tutorial_modelling_magnets.png
+-rw-r--r--   0        0        0    32221 2024-04-12 06:52:54.531146 magpylib-5.0.1/docs/_static/images/gallery_icon_tutorial_paths.png
+-rw-r--r--   0        0        0    29154 2024-04-12 06:52:54.531146 magpylib-5.0.1/docs/_static/images/gallery_icon_viz_animations.png
+-rw-r--r--   0        0        0   133213 2024-04-12 06:52:54.531146 magpylib-5.0.1/docs/_static/images/gallery_icon_viz_mpl_streamplot.png
+-rw-r--r--   0        0        0   101122 2024-04-12 06:52:54.531146 magpylib-5.0.1/docs/_static/images/gallery_icon_viz_pv_streamlines.png
+-rw-r--r--   0        0        0   125215 2024-04-12 06:52:54.531146 magpylib-5.0.1/docs/_static/images/gallery_tutorial_magnet_LDratio.png
+-rw-r--r--   0        0        0   192104 2024-04-12 06:52:54.531146 magpylib-5.0.1/docs/_static/images/gallery_tutorial_magnet_datasheet.png
+-rw-r--r--   0        0        0   115449 2024-04-12 06:52:54.531146 magpylib-5.0.1/docs/_static/images/gallery_tutorial_magnet_datasheet2.png
+-rw-r--r--   0        0        0   105716 2024-04-12 06:52:54.531146 magpylib-5.0.1/docs/_static/images/gallery_tutorial_magnet_fieldcomparison.png
+-rw-r--r--   0        0        0    82273 2024-04-12 06:52:54.535146 magpylib-5.0.1/docs/_static/images/gallery_tutorial_magnet_hysteresis.png
+-rw-r--r--   0        0        0    60218 2024-04-12 06:52:54.535146 magpylib-5.0.1/docs/_static/images/gallery_tutorial_magnet_table.png
+-rw-r--r--   0        0        0    42153 2024-04-12 06:52:54.535146 magpylib-5.0.1/docs/_static/images/getting_started_animation.png
+-rw-r--r--   0        0        0   107905 2024-04-12 06:52:54.535146 magpylib-5.0.1/docs/_static/images/getting_started_complex_shapes.png
+-rw-r--r--   0        0        0   101291 2024-04-12 06:52:54.535146 magpylib-5.0.1/docs/_static/images/getting_started_fundamentals1.png
+-rw-r--r--   0        0        0   114836 2024-04-12 06:52:54.535146 magpylib-5.0.1/docs/_static/images/getting_started_styles.png
+-rw-r--r--   0        0        0   240757 2024-04-12 06:52:54.535146 magpylib-5.0.1/docs/_static/images/index_flowchart.png
+-rw-r--r--   0        0        0   323052 2024-04-12 06:52:54.539146 magpylib-5.0.1/docs/_static/images/index_head.png
+-rw-r--r--   0        0        0     7837 2024-04-12 06:52:54.539146 magpylib-5.0.1/docs/_static/images/index_icon_academic.png
+-rw-r--r--   0        0        0     5281 2024-04-12 06:52:54.539146 magpylib-5.0.1/docs/_static/images/index_icon_contributing.png
+-rw-r--r--   0        0        0     8741 2024-04-12 06:52:54.539146 magpylib-5.0.1/docs/_static/images/index_icon_docu.png
+-rw-r--r--   0        0        0    12683 2024-04-12 06:52:54.539146 magpylib-5.0.1/docs/_static/images/index_icon_gallery.png
+-rw-r--r--   0        0        0     9752 2024-04-12 06:52:54.539146 magpylib-5.0.1/docs/_static/images/index_icon_getting_started.png
+-rw-r--r--   0        0        0     7864 2024-04-12 06:52:54.539146 magpylib-5.0.1/docs/_static/images/index_icon_github.png
+-rw-r--r--   0        0        0   167515 2024-04-12 06:52:54.539146 magpylib-5.0.1/docs/_static/images/magpylib_flag.png
+-rw-r--r--   0        0        0    22705 2024-04-12 06:52:54.539146 magpylib-5.0.1/docs/_static/images/magpylib_logo.png
+-rw-r--r--   0        0        0   526695 2024-04-12 06:52:54.543146 magpylib-5.0.1/docs/_static/videos/axis.mp4
+-rw-r--r--   0        0        0     2970 2024-04-12 06:52:54.543146 magpylib-5.0.1/docs/_static/webcode/copybutton.js
+-rw-r--r--   0        0        0      447 2024-04-12 06:52:54.543146 magpylib-5.0.1/docs/_static/webcode/summaryOpen.js
+-rw-r--r--   0        0        0    10243 2024-04-12 06:52:54.543146 magpylib-5.0.1/docs/conf.py
+-rw-r--r--   0        0        0     2316 2024-04-12 06:52:54.543146 magpylib-5.0.1/docs/index.md
+-rw-r--r--   0        0        0     6715 2024-04-12 06:52:54.543146 magpylib-5.0.1/docs/make.bat
+-rw-r--r--   0        0        0     1916 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/__init__.py
+-rw-r--r--   0        0        0       11 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/defaults/__init__.py
+-rw-r--r--   0        0        0     9448 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/defaults/defaults_classes.py
+-rw-r--r--   0        0        0    13989 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/defaults/defaults_utility.py
+-rw-r--r--   0        0        0     5981 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/defaults/defaults_values.py
+-rw-r--r--   0        0        0       22 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/display/__init__.py
+-rw-r--r--   0        0        0    14530 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/display/backend_matplotlib.py
+-rw-r--r--   0        0        0    10746 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/display/backend_plotly.py
+-rw-r--r--   0        0        0    12228 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/display/backend_pyvista.py
+-rw-r--r--   0        0        0    17456 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/display/display.py
+-rw-r--r--   0        0        0    11170 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/display/sensor_mesh.py
+-rw-r--r--   0        0        0    21819 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/display/traces_base.py
+-rw-r--r--   0        0        0    22486 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/display/traces_core.py
+-rw-r--r--   0        0        0    33281 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/display/traces_generic.py
+-rw-r--r--   0        0        0    26175 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/display/traces_utility.py
+-rw-r--r--   0        0        0      458 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/exceptions.py
+-rw-r--r--   0        0        0      312 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/fields/__init__.py
+-rw-r--r--   0        0        0     3696 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/fields/field_BH_circle.py
+-rw-r--r--   0        0        0     8994 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/fields/field_BH_cuboid.py
+-rw-r--r--   0        0        0    11016 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/fields/field_BH_cylinder.py
+-rw-r--r--   0        0        0    77680 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/fields/field_BH_cylinder_segment.py
+-rw-r--r--   0        0        0     2360 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/fields/field_BH_dipole.py
+-rw-r--r--   0        0        0     7223 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/fields/field_BH_polyline.py
+-rw-r--r--   0        0        0     2762 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/fields/field_BH_sphere.py
+-rw-r--r--   0        0        0     3775 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/fields/field_BH_tetrahedron.py
+-rw-r--r--   0        0        0     6453 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/fields/field_BH_triangle.py
+-rw-r--r--   0        0        0    19051 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/fields/field_BH_triangularmesh.py
+-rw-r--r--   0        0        0    48296 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/fields/field_wrap_BH.py
+-rw-r--r--   0        0        0     4396 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/fields/special_cel.py
+-rw-r--r--   0        0        0    17650 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/fields/special_el3.py
+-rw-r--r--   0        0        0    20724 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/input_checks.py
+-rw-r--r--   0        0        0       23 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/obj_classes/__init__.py
+-rw-r--r--   0        0        0     4090 2024-04-12 06:52:54.547146 magpylib-5.0.1/magpylib/_src/obj_classes/class_BaseDisplayRepr.py
+-rw-r--r--   0        0        0    19372 2024-04-12 06:52:54.547146 magpylib-5.0.1/magpylib/_src/obj_classes/class_BaseExcitations.py
+-rw-r--r--   0        0        0    12717 2024-04-12 06:52:54.547146 magpylib-5.0.1/magpylib/_src/obj_classes/class_BaseGeo.py
+-rw-r--r--   0        0        0    34491 2024-04-12 06:52:54.547146 magpylib-5.0.1/magpylib/_src/obj_classes/class_BaseTransform.py
+-rw-r--r--   0        0        0    36312 2024-04-12 06:52:54.547146 magpylib-5.0.1/magpylib/_src/obj_classes/class_Collection.py
+-rw-r--r--   0        0        0    18854 2024-04-12 06:52:54.547146 magpylib-5.0.1/magpylib/_src/obj_classes/class_Sensor.py
+-rw-r--r--   0        0        0     5043 2024-04-12 06:52:54.547146 magpylib-5.0.1/magpylib/_src/obj_classes/class_current_Circle.py
+-rw-r--r--   0        0        0     5456 2024-04-12 06:52:54.547146 magpylib-5.0.1/magpylib/_src/obj_classes/class_current_Polyline.py
+-rw-r--r--   0        0        0     4421 2024-04-12 06:52:54.547146 magpylib-5.0.1/magpylib/_src/obj_classes/class_magnet_Cuboid.py
+-rw-r--r--   0        0        0     5006 2024-04-12 06:52:54.547146 magpylib-5.0.1/magpylib/_src/obj_classes/class_magnet_Cylinder.py
+-rw-r--r--   0        0        0     6828 2024-04-12 06:52:54.547146 magpylib-5.0.1/magpylib/_src/obj_classes/class_magnet_CylinderSegment.py
+-rw-r--r--   0        0        0     4681 2024-04-12 06:52:54.547146 magpylib-5.0.1/magpylib/_src/obj_classes/class_magnet_Sphere.py
+-rw-r--r--   0        0        0     6030 2024-04-12 06:52:54.547146 magpylib-5.0.1/magpylib/_src/obj_classes/class_magnet_Tetrahedron.py
+-rw-r--r--   0        0        0    36933 2024-04-12 06:52:54.547146 magpylib-5.0.1/magpylib/_src/obj_classes/class_magnet_TriangularMesh.py
+-rw-r--r--   0        0        0     3520 2024-04-12 06:52:54.547146 magpylib-5.0.1/magpylib/_src/obj_classes/class_misc_CustomSource.py
+-rw-r--r--   0        0        0     4530 2024-04-12 06:52:54.547146 magpylib-5.0.1/magpylib/_src/obj_classes/class_misc_Dipole.py
+-rw-r--r--   0        0        0     5934 2024-04-12 06:52:54.547146 magpylib-5.0.1/magpylib/_src/obj_classes/class_misc_Triangle.py
+-rw-r--r--   0        0        0    77585 2024-04-12 06:52:54.547146 magpylib-5.0.1/magpylib/_src/style.py
+-rw-r--r--   0        0        0    12334 2024-04-12 06:52:54.547146 magpylib-5.0.1/magpylib/_src/utility.py
+-rw-r--r--   0        0        0     1048 2024-04-12 06:52:54.547146 magpylib-5.0.1/magpylib/core/__init__.py
+-rw-r--r--   0        0        0      398 2024-04-12 06:52:54.547146 magpylib-5.0.1/magpylib/current/__init__.py
+-rw-r--r--   0        0        0      260 2024-04-12 06:52:54.547146 magpylib-5.0.1/magpylib/graphics/__init__.py
+-rw-r--r--   0        0        0      835 2024-04-12 06:52:54.547146 magpylib-5.0.1/magpylib/graphics/model3d/__init__.py
+-rw-r--r--   0        0        0      353 2024-04-12 06:52:54.547146 magpylib-5.0.1/magpylib/graphics/style/__init__.py
+-rw-r--r--   0        0        0      632 2024-04-12 06:52:54.547146 magpylib-5.0.1/magpylib/magnet/__init__.py
+-rw-r--r--   0        0        0      335 2024-04-12 06:52:54.547146 magpylib-5.0.1/magpylib/misc/__init__.py
+-rw-r--r--   0        0        0     2332 2024-04-12 06:52:54.547146 magpylib-5.0.1/pyproject.toml
+-rw-r--r--   0        0        0       14 2024-04-12 06:52:54.547146 magpylib-5.0.1/tests/__init__.py
+-rw-r--r--   0        0        0    25344 2024-04-12 06:52:54.547146 magpylib-5.0.1/tests/test_BHMJ_level.py
+-rw-r--r--   0        0        0     7672 2024-04-12 06:52:54.547146 magpylib-5.0.1/tests/test_BaseTransform.py
+-rw-r--r--   0        0        0     5503 2024-04-12 06:52:54.547146 magpylib-5.0.1/tests/test_Coumpound_setters.py
+-rw-r--r--   0        0        0     2035 2024-04-12 06:52:54.547146 magpylib-5.0.1/tests/test_CustomSource.py
+-rw-r--r--   0        0        0      760 2024-04-12 06:52:54.547146 magpylib-5.0.1/tests/test__missing_optional_modules.py
+-rw-r--r--   0        0        0      465 2024-04-12 06:52:54.547146 magpylib-5.0.1/tests/test_core.py
+-rw-r--r--   0        0        0    17752 2024-04-12 06:52:54.547146 magpylib-5.0.1/tests/test_core_physics_consistency.py
+-rw-r--r--   0        0        0     7060 2024-04-12 06:52:54.547146 magpylib-5.0.1/tests/test_default_utils.py
+-rw-r--r--   0        0        0    10824 2024-04-12 06:52:54.547146 magpylib-5.0.1/tests/test_defaults.py
+-rw-r--r--   0        0        0    21282 2024-04-12 06:52:54.547146 magpylib-5.0.1/tests/test_display_matplotlib.py
+-rw-r--r--   0        0        0    13771 2024-04-12 06:52:54.547146 magpylib-5.0.1/tests/test_display_plotly.py
+-rw-r--r--   0        0        0     4507 2024-04-12 06:52:54.547146 magpylib-5.0.1/tests/test_display_pyvista.py
+-rw-r--r--   0        0        0     3181 2024-04-12 06:52:54.547146 magpylib-5.0.1/tests/test_display_utility.py
+-rw-r--r--   0        0        0     3453 2024-04-12 06:52:54.547146 magpylib-5.0.1/tests/test_elliptics.py
+-rw-r--r--   0        0        0     8864 2024-04-12 06:52:54.547146 magpylib-5.0.1/tests/test_exceptions.py
+-rw-r--r--   0        0        0    15385 2024-04-12 06:52:54.547146 magpylib-5.0.1/tests/test_field_cylinder.py
+-rw-r--r--   0        0        0    13402 2024-04-12 06:52:54.547146 magpylib-5.0.1/tests/test_getBH_dict.py
+-rw-r--r--   0        0        0    12196 2024-04-12 06:52:54.547146 magpylib-5.0.1/tests/test_getBH_interfaces.py
+-rw-r--r--   0        0        0    19579 2024-04-12 06:52:54.547146 magpylib-5.0.1/tests/test_getBH_level2.py
+-rw-r--r--   0        0        0    25249 2024-04-12 06:52:54.547146 magpylib-5.0.1/tests/test_input_checks.py
+-rw-r--r--   0        0        0      346 2024-04-12 06:52:54.547146 magpylib-5.0.1/tests/test_misc.py
+-rw-r--r--   0        0        0      737 2024-04-12 06:52:54.547146 magpylib-5.0.1/tests/test_numerical_stability.py
+-rw-r--r--   0        0        0    20450 2024-04-12 06:52:54.547146 magpylib-5.0.1/tests/test_obj_BaseGeo.py
+-rw-r--r--   0        0        0    12300 2024-04-12 06:52:54.547146 magpylib-5.0.1/tests/test_obj_BaseGeo_v4motion.py
+-rw-r--r--   0        0        0     2208 2024-04-12 06:52:54.551146 magpylib-5.0.1/tests/test_obj_Circle.py
+-rw-r--r--   0        0        0    15913 2024-04-12 06:52:54.551146 magpylib-5.0.1/tests/test_obj_Collection.py
+-rw-r--r--   0        0        0    10301 2024-04-12 06:52:54.551146 magpylib-5.0.1/tests/test_obj_Collection_child_parent.py
+-rw-r--r--   0        0        0    25232 2024-04-12 06:52:54.551146 magpylib-5.0.1/tests/test_obj_Collection_v4motion.py
+-rw-r--r--   0        0        0     4516 2024-04-12 06:52:54.551146 magpylib-5.0.1/tests/test_obj_Cuboid.py
+-rw-r--r--   0        0        0     4140 2024-04-12 06:52:54.551146 magpylib-5.0.1/tests/test_obj_Cylinder.py
+-rw-r--r--   0        0        0     1087 2024-04-12 06:52:54.551146 magpylib-5.0.1/tests/test_obj_CylinderSegment.py
+-rw-r--r--   0        0        0     1038 2024-04-12 06:52:54.551146 magpylib-5.0.1/tests/test_obj_Dipole.py
+-rw-r--r--   0        0        0     3787 2024-04-12 06:52:54.551146 magpylib-5.0.1/tests/test_obj_Polyline.py
+-rw-r--r--   0        0        0     3719 2024-04-12 06:52:54.551146 magpylib-5.0.1/tests/test_obj_Sensor.py
+-rw-r--r--   0        0        0     3105 2024-04-12 06:52:54.551146 magpylib-5.0.1/tests/test_obj_Sphere.py
+-rw-r--r--   0        0        0     2467 2024-04-12 06:52:54.551146 magpylib-5.0.1/tests/test_obj_Tetrahedron.py
+-rw-r--r--   0        0        0     2446 2024-04-12 06:52:54.551146 magpylib-5.0.1/tests/test_obj_Triangle.py
+-rw-r--r--   0        0        0    16212 2024-04-12 06:52:54.551146 magpylib-5.0.1/tests/test_obj_TriangularMesh.py
+-rw-r--r--   0        0        0     1654 2024-04-12 06:52:54.551146 magpylib-5.0.1/tests/test_path.py
+-rw-r--r--   0        0        0    10338 2024-04-12 06:52:54.551146 magpylib-5.0.1/tests/test_physics_consistency.py
+-rw-r--r--   0        0        0      661 2024-04-12 06:52:54.551146 magpylib-5.0.1/tests/test_scaling.py
+-rw-r--r--   0        0        0     2633 2024-04-12 06:52:54.551146 magpylib-5.0.1/tests/test_utility.py
+-rw-r--r--   0        0        0     2966 2024-04-12 06:52:54.551146 magpylib-5.0.1/tests/test_vs_mag2.py
+-rw-r--r--   0        0        0    14641 2024-04-12 06:52:54.551146 magpylib-5.0.1/tests/testdata/testdata_Collection.p
+-rw-r--r--   0        0        0     1568 2024-04-12 06:52:54.551146 magpylib-5.0.1/tests/testdata/testdata_Collection_setter.npy
+-rw-r--r--   0        0        0  1747640 2024-04-12 06:52:54.559146 magpylib-5.0.1/tests/testdata/testdata_Cuboid.p
+-rw-r--r--   0        0        0  1746038 2024-04-12 06:52:54.571146 magpylib-5.0.1/tests/testdata/testdata_Sphere.p
+-rw-r--r--   0        0        0    17225 2024-04-12 06:52:54.571146 magpylib-5.0.1/tests/testdata/testdata_compound_setter_cases.npy
+-rw-r--r--   0        0        0  1095577 2024-04-12 06:52:54.575146 magpylib-5.0.1/tests/testdata/testdata_cy_cases.npy
+-rw-r--r--   0        0        0   320128 2024-04-12 06:52:54.575146 magpylib-5.0.1/tests/testdata/testdata_el3.npy
+-rw-r--r--   0        0        0  1534592 2024-04-12 06:52:54.583146 magpylib-5.0.1/tests/testdata/testdata_el3_angle.npy
+-rw-r--r--   0        0        0    13056 2024-04-12 06:52:54.583146 magpylib-5.0.1/tests/testdata/testdata_femDat_cylinder_tile2.npy
+-rw-r--r--   0        0        0   102475 2024-04-12 06:52:54.583146 magpylib-5.0.1/tests/testdata/testdata_field_BH_cuboid.p
+-rw-r--r--   0        0        0   240606 2024-04-12 06:52:54.583146 magpylib-5.0.1/tests/testdata/testdata_field_BH_cylinder.p
+-rw-r--r--   0        0        0     9728 2024-04-12 06:52:54.583146 magpylib-5.0.1/tests/testdata/testdata_full_cyl.npy
+-rw-r--r--   0        0        0     1022 2024-04-12 06:52:54.583146 magpylib-5.0.1/tests/testdata/testdata_path_BaseGeo.p
+-rw-r--r--   0        0        0     7362 2024-04-12 06:52:54.583146 magpylib-5.0.1/tests/testdata/testdata_vs_mag2.p
+-rw-r--r--   0        0        0      606 2024-04-12 06:52:54.583146 magpylib-5.0.1/tox.ini
+-rw-r--r--   0        0        0     9404 1970-01-01 00:00:00.000000 magpylib-5.0.1/PKG-INFO
```

### Comparing `magpylib-5.0.0rc0/.github/ISSUE_TEMPLATE/bug_report.yaml` & `magpylib-5.0.1/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/.github/ISSUE_TEMPLATE/feature_request.yaml` & `magpylib-5.0.1/.github/ISSUE_TEMPLATE/feature_request.yaml`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/.github/ISSUE_TEMPLATE/question_magnetics.yaml` & `magpylib-5.0.1/.github/ISSUE_TEMPLATE/question_magnetics.yaml`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/.github/workflows/codeql.yml` & `magpylib-5.0.1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/.github/workflows/python-app.yml` & `magpylib-5.0.1/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/.gitignore` & `magpylib-5.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/.pre-commit-config.yaml` & `magpylib-5.0.1/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: check-yaml
       - id: end-of-file-fixer
         types: [file, python]
       - id: trailing-whitespace
         types: [file, python]
       - id: check-added-large-files
@@ -14,22 +14,22 @@
   - repo: https://github.com/pycqa/isort
     rev: 5.13.2
     hooks:
       - id: isort
         name: isort (python)
 
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.15.1
+    rev: v3.15.2
     hooks:
       - id: pyupgrade
         args: [--py38-plus]
 
 
   - repo: https://github.com/psf/black
-    rev: "24.2.0"
+    rev: "24.3.0"
     hooks:
       - id: black
 
 
   # - repo: local
   #   hooks:
   #     - id: pylint
```

### Comparing `magpylib-5.0.0rc0/.pylintrc` & `magpylib-5.0.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/.readthedocs.yaml` & `magpylib-5.0.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/CHANGELOG.md` & `magpylib-5.0.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 All notable changes to magpylib are documented here.
 
 
 # Changelog
 
-## [5.0.0rc0] - 2024-03-13
+## [5.0.1] - 2024-04-12
+- Fixed a bug where `getBHJM` of a Collection would produce one extra dimension ([#753](https://github.com/magpylib/magpylib/issues/753))
+- Fixed a bug where the legend of a deeply nested Collection would be wrong ([#756](https://github.com/magpylib/magpylib/issues/756))
+
+## [5.0.0] - 2024-03-13
 ### ⚠️ Breaking Changes ⚠️
 - The Magpylib inputs and outputs are now in **SI Units**.
 - The `magnetization` parameter has also been redefined to reflect the true physical magnetization quantity in units of A/m.
 ### Other Improvements
 - The `magnetization` parameter is now codependent with the new `polarization` parameter that is the physical magnetic polarization ([#712](https://github.com/magpylib/magpylib/issues/712)) in units of Tesla.
 - Added `getM` (magnetization) and `getJ` (polarization) top level functions and class methods reminiscent of `getB` and `getH`.
 - The `in_out` (inside/outside) parameter is added to all field functions (`getBHJM`) to specify the location of the observers relative to the magnet body in order to increase performance ([#717](https://github.com/magpylib/magpylib/issues/717), [#608](https://github.com/magpylib/magpylib/issues/608))
@@ -448,15 +452,16 @@
    - Loop Current
    - Current Line
    - Dipole
 - Collection class
 
 ---
 
-[5.0.0rc0]:https://github.com/magpylib/magpylib/compare/4.5.1...HEAD
+[5.0.1]:https://github.com/magpylib/magpylib/compare/5.0.0...HEAD
+[5.0.0]:https://github.com/magpylib/magpylib/compare/4.5.1...5.0.0
 [4.5.1]:https://github.com/magpylib/magpylib/compare/4.5.0...4.5.1
 [4.5.0]:https://github.com/magpylib/magpylib/compare/4.4.0...4.5.0
 [4.4.1]:https://github.com/magpylib/magpylib/compare/4.4.0...4.4.1
 [4.4.0]:https://github.com/magpylib/magpylib/compare/4.3.0...4.4.0
 [4.3.0]:https://github.com/magpylib/magpylib/compare/4.2.0...4.3.0
 [4.2.0]:https://github.com/magpylib/magpylib/compare/4.1.2...4.2.0
 [4.1.2]:https://github.com/magpylib/magpylib/compare/4.1.1...4.1.2
```

### Comparing `magpylib-5.0.0rc0/CODE_OF_CONDUCT.md` & `magpylib-5.0.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/CONTRIBUTING.md` & `magpylib-5.0.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/LICENSE` & `magpylib-5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/README.md` & `magpylib-5.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 </a>
 <a href="https://codecov.io/gh/magpylib/magpylib"> <img src="https://codecov.io/gh/magpylib/magpylib/branch/main/graph/badge.svg">
 </a>
 <a href="https://pypi.org/project/magpylib/"> <img src="https://badge.fury.io/py/magpylib.svg" alt="PyPI version" height="18">
 </a>
 <a href="https://anaconda.org/conda-forge/magpylib"> <img src="https://anaconda.org/conda-forge/magpylib/badges/version.svg" alt="Conda Cloud" height="18">
 </a>
-<a href="https://mybinder.org/v2/gh/magpylib/magpylib/5.0.0rc0?filepath=docs%2Fexamples"> <img src="https://mybinder.org/badge_logo.svg" alt="MyBinder link" height="18">
+<a href="https://mybinder.org/v2/gh/magpylib/magpylib/5.0.0?filepath=docs%2Fexamples"> <img src="https://mybinder.org/badge_logo.svg" alt="MyBinder link" height="18">
 </a>
 <a href="https://github.com/psf/black"> <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="black" height="18">
 </a>
 </div>
 
 Magpylib is a Python package for calculating **3D static magnetic fields** of magnets, line currents and other sources. The computation is based on explicit expressions and is therefore **extremely fast**. A **user friendly API** enables convenient positioning of sources and observers.
 
@@ -132,11 +132,11 @@
 A valid software citation could be
 
 ```
 @software{magpylib,
     author = {{Michael-Ortner et al.}},
     title = {magpylib},
     url = {https://magpylib.readthedocs.io/en/latest/},
-    version = {5.0.0rc0},
+    version = {5.0.1},
     date = {2023-06-25},
 }
 ```
```

#### html2text {}

```diff
@@ -72,9 +72,9 @@
 bibtex entry for the [2020 open-access paper](https://www.sciencedirect.com/
 science/article/pii/S2352711020300170) would be ``` @article
 {ortner2020magpylib, title={Magpylib: A free Python package for magnetic field
 computation}, author={Ortner, Michael and Bandeira, Lucas Gabriel Coliado},
 journal={SoftwareX}, volume={11}, pages={100466}, year={2020}, publisher=
 {Elsevier} } ``` A valid software citation could be ``` @software{magpylib,
 author = {{Michael-Ortner et al.}}, title = {magpylib}, url = {https://
-magpylib.readthedocs.io/en/latest/}, version = {5.0.0rc0}, date = {2023-06-25},
-} ```
+magpylib.readthedocs.io/en/latest/}, version = {5.0.1}, date = {2023-06-25}, }
+```
```

### Comparing `magpylib-5.0.0rc0/docs/Makefile` & `magpylib-5.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/README.md` & `magpylib-5.0.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_pages/docu/docu_graphics.md` & `magpylib-5.0.1/docs/_pages/docu/docu_graphics.md`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_pages/docu/docu_index.md` & `magpylib-5.0.1/docs/_pages/docu/docu_index.md`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_pages/docu/docu_magpylib_api.md` & `magpylib-5.0.1/docs/_pages/docu/docu_magpylib_api.md`

 * *Files 1% similar despite different names*

```diff
@@ -40,16 +40,17 @@
 
 ::::
 
 ```{warning}
 Up to version 4, Magpylib was unfortunately contributing to the naming confusion in magnetism that is explained well [here](https://www.e-magnetica.pl/doku.php/confusion_between_b_and_h). The input `magnetization` in Magpylib < v5 was referring to the magnetic polarization (and not the magnetization), the difference being only in the physical unit. From version 5 onwards this is fixed.
 ```
 
-```{note}
-All input and output units in Magpylib (version 5 and higher) are SI-based, see table above. However, for advanced use one should be aware that the analytical solutions are scale invariant - _"a magnet with 1 mm sides creates the same field at 1 mm distance as a magnet with 1 m sides at 1 m distance"_. The choice of length input unit is therefore not relevant, but it is critical to keep the same length unit for all inputs in one computation.
+(docu-api-scale-invariance)=
+```{hint}
+All input and output units in Magpylib (version 5 and higher) are SI-based, see table above. However, for advanced use one should be aware that the analytical solutions are **scale invariant** - _"a magnet with 1 mm sides creates the same field at 1 mm distance as a magnet with 1 m sides at 1 m distance"_. The choice of length input unit is therefore not relevant, but it is critical to keep the same length unit for all inputs in one computation.
 
 In addition, `getB` returns the same unit as given by the `polarization` input. With polarization input in mT, getB will return mT as well. At the same time when the `magnetization` input is kA/m, then `getH` returns kA/m as well. The B/H-field outputs are related to a M/J-inputs via a factor of $µ_0$.
 ```
 
 ```{note}
 The connection between the magnetic polarization J, the magnetization M and the material parameters of a real permanent magnet are shown in {ref}`gallery-tutorial-modelling-magnets`.
 ```
```

### Comparing `magpylib-5.0.0rc0/docs/_pages/docu/docu_physics.md` & `magpylib-5.0.1/docs/_pages/docu/docu_physics.md`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_pages/gallery/gallery_app_end_of_shaft.md` & `magpylib-5.0.1/docs/_pages/gallery/gallery_app_end_of_shaft.md`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_pages/gallery/gallery_app_helmholtz.md` & `magpylib-5.0.1/docs/_pages/gallery/gallery_app_helmholtz.md`

 * *Files 2% similar despite different names*

```diff
@@ -105,19 +105,19 @@
 from matplotlib.patches import Rectangle
 for loc in [(4,4), (4,-6), (-6,4), (-6,-6)]:
     ax.add_patch(Rectangle(loc, 2, 2, color='k', zorder=10))
 
 # figure styling
 ax.set(
     title='Magnetic field of Helmholtz',
-    xlabel='x-position (mm)',
-    ylabel='z-position (mm)',
+    xlabel='x-position (m)',
+    ylabel='z-position (m)',
     aspect=1,
 )
-plt.colorbar(sp.lines, ax=ax, label='(mT)')
+plt.colorbar(sp.lines, ax=ax, label='(T)')
 
 plt.tight_layout()
 plt.show()
 ```
 
 ## Helmholtz field homogeneity
 
@@ -140,16 +140,16 @@
 
 # plot error on grid
 sp = ax.contourf(grid[:,:,0], grid[:,:,2], err*100)
 
 # figure styling
 ax.set(
     title='Helmholtz homogeneity error',
-    xlabel='x-position (mm)',
-    ylabel='z-position (mm)',
+    xlabel='x-position (m)',
+    ylabel='z-position (m)',
     aspect=1,
 )
 plt.colorbar(sp, ax=ax, label='(% of B0)')
 
 plt.tight_layout()
 plt.show()
 ```
```

### Comparing `magpylib-5.0.0rc0/docs/_pages/gallery/gallery_index.md` & `magpylib-5.0.1/docs/_pages/gallery/gallery_index.md`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 :::
 
 :::{grid-item-card} {ref}`gallery-vis-animations`
 :text-align: center
 :link: gallery-vis-animations
 :link-type: ref
 :link-alt: link to example
-:img-bottom: ../../_static/images/gallery_icon_WIP.png
+:img-bottom: ../../_static/images/gallery_icon_viz_animations.png
 :::
 
 :::{grid-item-card} {ref}`gallery-vis-subplots`
 :text-align: center
 :link: gallery-vis-subplots
 :link-type: ref
 :link-alt: link to example
```

### Comparing `magpylib-5.0.0rc0/docs/_pages/gallery/gallery_misc_compound.md` & `magpylib-5.0.1/docs/_pages/gallery/gallery_misc_compound.md`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_pages/gallery/gallery_misc_field_interpolation.md` & `magpylib-5.0.1/docs/_pages/gallery/gallery_misc_field_interpolation.md`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_pages/gallery/gallery_shapes_convex_hull.md` & `magpylib-5.0.1/docs/_pages/gallery/gallery_shapes_convex_hull.md`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_pages/gallery/gallery_shapes_pyvista.md` & `magpylib-5.0.1/docs/_pages/gallery/gallery_shapes_pyvista.md`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_pages/gallery/gallery_shapes_superpos.md` & `magpylib-5.0.1/docs/_pages/gallery/gallery_shapes_superpos.md`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_pages/gallery/gallery_shapes_triangle.md` & `magpylib-5.0.1/docs/_pages/gallery/gallery_shapes_triangle.md`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_pages/gallery/gallery_tutorial_collection.md` & `magpylib-5.0.1/docs/_pages/gallery/gallery_tutorial_collection.md`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_pages/gallery/gallery_tutorial_custom.md` & `magpylib-5.0.1/docs/_pages/gallery/gallery_tutorial_custom.md`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_pages/gallery/gallery_tutorial_field_computation.md` & `magpylib-5.0.1/docs/_pages/gallery/gallery_tutorial_field_computation.md`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_pages/gallery/gallery_tutorial_modelling_magnets.md` & `magpylib-5.0.1/docs/_pages/gallery/gallery_tutorial_modelling_magnets.md`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_pages/gallery/gallery_tutorial_paths.md` & `magpylib-5.0.1/docs/_pages/gallery/gallery_tutorial_paths.md`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_pages/gallery/gallery_vis_mpl_streamplot.md` & `magpylib-5.0.1/docs/_pages/gallery/gallery_vis_mpl_streamplot.md`

 * *Files 16% similar despite different names*

```diff
@@ -16,55 +16,57 @@
 
 # Matplotlib Streamplot
 
 ## Example 1: Cuboid Magnet
 
 In this example we show the B-field of a cuboid magnet using Matplotlib streamlines. Streamlines are not magnetic field lines in the sense that the field amplitude cannot be derived from their density. However, Matplotlib streamlines can show the field amplitude via color and line thickness. One must be careful that streamlines can only display two components of the field. In the following example the third field component is always zero - but this is generally not the case.
 
+In the example we make use of the [scaling property](docu-api-scale-invariance). We assume that all length inputs are in units of mm, and that the polarization input is in units of millitesla. The resulting `getB` output will also be in millitesla. One must be careful with scaling - the conversion to H would ofc give units of mA/m.
+
 ```{code-cell} ipython3
 import matplotlib.pyplot as plt
 import numpy as np
 
 import magpylib as magpy
 
 # Create a Matplotlib figure
 fig, ax = plt.subplots()
 
 # Create an observer grid in the xz-symmetry plane
-ts = np.linspace(-0.05, 0.05, 40)
+ts = np.linspace(-5, 5, 40)
 grid = np.array([[(x, 0, z) for x in ts] for z in ts])
 
 # Compute the B-field of a cube magnet on the grid
-cube = magpy.magnet.Cuboid(polarization=(0.5, 0, 0.5), dimension=(0.02, 0.02, 0.02))
+cube = magpy.magnet.Cuboid(polarization=(500,0,500), dimension=(2,2,2))
 B = cube.getB(grid)
 log10_norm_B = np.log10(np.linalg.norm(B, axis=2))
 
 # Display the B-field with streamplot using log10-scaled
 # color function and linewidth
 splt = ax.streamplot(
-    grid[:, :, 0]*1000, # m -> mm
-    grid[:, :, 2]*1000, # m -> mm
-    B[:, :, 0]*1000, # T -> mT
-    B[:, :, 2]*1000, # T -> mT
+    grid[:, :, 0],
+    grid[:, :, 2],
+    B[:, :, 0],
+    B[:, :, 2],
+    density=1.5,
     color=log10_norm_B,
-    density=1,
-    linewidth=log10_norm_B * 2,
+    linewidth=log10_norm_B,
     cmap="autumn",
 )
 
 # Add colorbar with logarithmic labels
 cb = fig.colorbar(splt.lines, ax=ax, label="|B| (mT)")
 ticks = np.array([3, 10, 30, 100, 300])
 cb.set_ticks(np.log10(ticks))
 cb.set_ticklabels(ticks)
 
 # Outline magnet boundary
 ax.plot(
-    np.array([1, 1, -1, -1, 1]) * 10, # mm
-    np.array([1, -1, -1, 1, 1]) * 10, # mm
+    [1, 1, -1, -1, 1],
+    [1, -1, -1, 1, 1],
     "k--",
     lw=2,
 )
 
 # Figure styling
 ax.set(
     xlabel="x-position (mm)",
@@ -104,43 +106,43 @@
     polarization=(0.1, 0, 0),
 )
 B = B.reshape(grid.shape)
 normB = np.linalg.norm(B, axis=2)
 
 # combine streamplot with contourf
 cp = ax.contourf(
-    X * 1000,  # m -> mm
-    Y * 1000,  # m -> mm
-    normB,
+    X,
+    Y,
+    normB*1000, #T->mT
     cmap="rainbow",
     levels=100,
     zorder=1,
 )
 splt = ax.streamplot(
-    X* 1000,  # m -> mm,
-    Y* 1000,  # m -> mm,
-    B[:, :, 0], # T -> mT
-    B[:, :, 1], # T -> mT
+    X,
+    Y,
+    B[:, :, 0],
+    B[:, :, 1],
     color="k",
     density=1.5,
     linewidth=1,
     zorder=3,
 )
 
 # Add colorbar
 fig.colorbar(cp, ax=ax, label="|B| (mT)")
 
 # Outline magnet boundary
 ts = np.linspace(0, 2 * np.pi, 50)
-ax.plot(30 * np.cos(ts), 30 * np.sin(ts), "w-", lw=2, zorder=2)
-ax.plot(20 * np.cos(ts), 20 * np.sin(ts), "w-", lw=2, zorder=2)
+ax.plot(.03*np.cos(ts), .03*np.sin(ts), "w-", lw=2, zorder=2)
+ax.plot(.02*np.cos(ts), .02*np.sin(ts), "w-", lw=2, zorder=2)
 
 # Figure styling
 ax.set(
-    xlabel="x-position (mm)",
-    ylabel="z-position (mm)",
+    xlabel="x-position (m)",
+    ylabel="z-position (m)",
     aspect=1,
 )
 
 plt.tight_layout()
 plt.show()
 ```
```

### Comparing `magpylib-5.0.0rc0/docs/_pages/gallery/gallery_vis_pv_streamlines.md` & `magpylib-5.0.1/docs/_pages/gallery/gallery_vis_pv_streamlines.md`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_pages/gallery/gallery_vis_subplots.md` & `magpylib-5.0.1/docs/_pages/gallery/gallery_vis_subplots.md`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_pages/reso_get_started.md` & `magpylib-5.0.1/docs/_pages/reso_get_started.md`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/docu_classes_init_collection.png` & `magpylib-5.0.1/docs/_static/images/docu_classes_init_collection.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/docu_classes_init_cuboid.png` & `magpylib-5.0.1/docs/_static/images/docu_classes_init_cuboid.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/docu_classes_init_custom.png` & `magpylib-5.0.1/docs/_static/images/docu_classes_init_custom.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/docu_classes_init_cylinder.png` & `magpylib-5.0.1/docs/_static/images/docu_classes_init_cylinder.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/docu_classes_init_cylindersegment.png` & `magpylib-5.0.1/docs/_static/images/docu_classes_init_cylindersegment.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/docu_classes_init_dipole.png` & `magpylib-5.0.1/docs/_static/images/docu_classes_init_dipole.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/docu_classes_init_global_local.png` & `magpylib-5.0.1/docs/_static/images/docu_classes_init_global_local.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/docu_classes_init_line.png` & `magpylib-5.0.1/docs/_static/images/docu_classes_init_line.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/docu_classes_init_loop.png` & `magpylib-5.0.1/docs/_static/images/docu_classes_init_loop.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/docu_classes_init_sensor.png` & `magpylib-5.0.1/docs/_static/images/docu_classes_init_sensor.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/docu_classes_init_sphere.png` & `magpylib-5.0.1/docs/_static/images/docu_classes_init_sphere.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/docu_classes_init_tetra.png` & `magpylib-5.0.1/docs/_static/images/docu_classes_init_tetra.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/docu_classes_init_triangle.png` & `magpylib-5.0.1/docs/_static/images/docu_classes_init_triangle.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/docu_classes_init_trimesh.png` & `magpylib-5.0.1/docs/_static/images/docu_classes_init_trimesh.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/docu_field_comp_flow.png` & `magpylib-5.0.1/docs/_static/images/docu_field_comp_flow.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/docu_field_superpos_cutout.png` & `magpylib-5.0.1/docs/_static/images/docu_field_superpos_cutout.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/docu_field_superpos_union.png` & `magpylib-5.0.1/docs/_static/images/docu_field_superpos_union.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/docu_index_icon_magpylib.png` & `magpylib-5.0.1/docs/_static/images/docu_index_icon_magpylib.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/docu_index_icon_magpylib_show.png` & `magpylib-5.0.1/docs/_static/images/docu_index_icon_magpylib_show.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/docu_index_icon_physics.png` & `magpylib-5.0.1/docs/_static/images/docu_index_icon_physics.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/docu_position_sketch.png` & `magpylib-5.0.1/docs/_static/images/docu_position_sketch.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/favicons/android-chrome-192x192.png` & `magpylib-5.0.1/docs/_static/images/favicons/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/favicons/android-chrome-512x512.png` & `magpylib-5.0.1/docs/_static/images/favicons/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/favicons/apple-touch-icon.png` & `magpylib-5.0.1/docs/_static/images/favicons/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/favicons/favicon-16x16.png` & `magpylib-5.0.1/docs/_static/images/favicons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/favicons/favicon-32x32.png` & `magpylib-5.0.1/docs/_static/images/favicons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/favicons/favicon.ico` & `magpylib-5.0.1/docs/_static/images/favicons/favicon.ico`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/gallery_icon_WIP.png` & `magpylib-5.0.1/docs/_static/images/gallery_icon_WIP.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/gallery_icon_app_end_of_shaft.png` & `magpylib-5.0.1/docs/_static/images/gallery_icon_app_end_of_shaft.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/gallery_icon_app_helmholtz.png` & `magpylib-5.0.1/docs/_static/images/gallery_icon_app_helmholtz.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/gallery_icon_ext_custom_quadrupole.png` & `magpylib-5.0.1/docs/_static/images/gallery_icon_ext_custom_quadrupole.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/gallery_icon_misc_compound.png` & `magpylib-5.0.1/docs/_static/images/gallery_icon_misc_compound.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/gallery_icon_misc_field_interpolation.png` & `magpylib-5.0.1/docs/_static/images/gallery_icon_misc_field_interpolation.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/gallery_icon_shapes_convex_hull.png` & `magpylib-5.0.1/docs/_static/images/gallery_icon_shapes_convex_hull.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/gallery_icon_shapes_pyvista.png` & `magpylib-5.0.1/docs/_static/images/gallery_icon_shapes_pyvista.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/gallery_icon_shapes_superpos.png` & `magpylib-5.0.1/docs/_static/images/gallery_icon_shapes_superpos.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/gallery_icon_shapes_triangle.png` & `magpylib-5.0.1/docs/_static/images/gallery_icon_shapes_triangle.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/gallery_icon_tutorial_collection.png` & `magpylib-5.0.1/docs/_static/images/gallery_icon_tutorial_collection.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/gallery_icon_tutorial_custom.png` & `magpylib-5.0.1/docs/_static/images/gallery_icon_tutorial_custom.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/gallery_icon_tutorial_field_computation.png` & `magpylib-5.0.1/docs/_static/images/gallery_icon_tutorial_field_computation.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/gallery_icon_tutorial_modelling_magnets.png` & `magpylib-5.0.1/docs/_static/images/gallery_icon_tutorial_modelling_magnets.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/gallery_icon_tutorial_paths.png` & `magpylib-5.0.1/docs/_static/images/gallery_icon_tutorial_paths.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/gallery_icon_viz_mpl_streamplot.png` & `magpylib-5.0.1/docs/_static/images/gallery_icon_viz_mpl_streamplot.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/gallery_icon_viz_pv_streamlines.png` & `magpylib-5.0.1/docs/_static/images/gallery_icon_viz_pv_streamlines.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/gallery_tutorial_magnet_LDratio.png` & `magpylib-5.0.1/docs/_static/images/gallery_tutorial_magnet_LDratio.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/gallery_tutorial_magnet_datasheet.png` & `magpylib-5.0.1/docs/_static/images/gallery_tutorial_magnet_datasheet.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/gallery_tutorial_magnet_datasheet2.png` & `magpylib-5.0.1/docs/_static/images/gallery_tutorial_magnet_datasheet2.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/gallery_tutorial_magnet_fieldcomparison.png` & `magpylib-5.0.1/docs/_static/images/gallery_tutorial_magnet_fieldcomparison.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/gallery_tutorial_magnet_hysteresis.png` & `magpylib-5.0.1/docs/_static/images/gallery_tutorial_magnet_hysteresis.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/gallery_tutorial_magnet_table.png` & `magpylib-5.0.1/docs/_static/images/gallery_tutorial_magnet_table.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/getting_started_animation.png` & `magpylib-5.0.1/docs/_static/images/getting_started_animation.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/getting_started_complex_shapes.png` & `magpylib-5.0.1/docs/_static/images/getting_started_complex_shapes.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/getting_started_fundamentals1.png` & `magpylib-5.0.1/docs/_static/images/getting_started_fundamentals1.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/getting_started_styles.png` & `magpylib-5.0.1/docs/_static/images/getting_started_styles.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/index_flowchart.png` & `magpylib-5.0.1/docs/_static/images/index_flowchart.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/index_head.png` & `magpylib-5.0.1/docs/_static/images/index_head.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/index_icon_academic.png` & `magpylib-5.0.1/docs/_static/images/index_icon_academic.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/index_icon_contributing.png` & `magpylib-5.0.1/docs/_static/images/index_icon_contributing.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/index_icon_docu.png` & `magpylib-5.0.1/docs/_static/images/index_icon_docu.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/index_icon_gallery.png` & `magpylib-5.0.1/docs/_static/images/index_icon_gallery.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/index_icon_getting_started.png` & `magpylib-5.0.1/docs/_static/images/index_icon_getting_started.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/index_icon_github.png` & `magpylib-5.0.1/docs/_static/images/index_icon_github.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/magpylib_flag.png` & `magpylib-5.0.1/docs/_static/images/magpylib_flag.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/images/magpylib_logo.png` & `magpylib-5.0.1/docs/_static/images/magpylib_logo.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/videos/axis.mp4` & `magpylib-5.0.1/docs/_static/videos/axis.mp4`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/_static/webcode/copybutton.js` & `magpylib-5.0.1/docs/_static/webcode/copybutton.js`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/conf.py` & `magpylib-5.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/index.md` & `magpylib-5.0.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/docs/make.bat` & `magpylib-5.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/magpylib/__init__.py` & `magpylib-5.0.1/magpylib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 The original software publication (version 2):
 
 https://www.sciencedirect.com/science/article/pii/S2352711020300170
 
 """
 # module level dunders
-__version__ = "5.0.0rc0"
+__version__ = "5.0.1"
 __author__ = "Michael Ortner & Alexandre Boisselet"
 __credits__ = "The Magpylib community"
 __all__ = [
     "magnet",
     "current",
     "misc",
     "getB",
```

### Comparing `magpylib-5.0.0rc0/magpylib/_src/defaults/defaults_classes.py` & `magpylib-5.0.1/magpylib/_src/defaults/defaults_classes.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/magpylib/_src/defaults/defaults_utility.py` & `magpylib-5.0.1/magpylib/_src/defaults/defaults_utility.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/magpylib/_src/defaults/defaults_values.py` & `magpylib-5.0.1/magpylib/_src/defaults/defaults_values.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/magpylib/_src/display/backend_matplotlib.py` & `magpylib-5.0.1/magpylib/_src/display/backend_matplotlib.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/magpylib/_src/display/backend_plotly.py` & `magpylib-5.0.1/magpylib/_src/display/backend_plotly.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/magpylib/_src/display/backend_pyvista.py` & `magpylib-5.0.1/magpylib/_src/display/backend_pyvista.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/magpylib/_src/display/display.py` & `magpylib-5.0.1/magpylib/_src/display/display.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/magpylib/_src/display/sensor_mesh.py` & `magpylib-5.0.1/magpylib/_src/display/sensor_mesh.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/magpylib/_src/display/traces_base.py` & `magpylib-5.0.1/magpylib/_src/display/traces_base.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/magpylib/_src/display/traces_core.py` & `magpylib-5.0.1/magpylib/_src/display/traces_core.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/magpylib/_src/display/traces_generic.py` & `magpylib-5.0.1/magpylib/_src/display/traces_generic.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/magpylib/_src/display/traces_utility.py` & `magpylib-5.0.1/magpylib/_src/display/traces_utility.py`

 * *Files 1% similar despite different names*

```diff
@@ -278,30 +278,31 @@
         color_cycle = cycle(colorsequence)
     flat_objs = {}
     for subobj in obj_list_semi_flat:
         isCollection = getattr(subobj, "children", None) is not None
         style = get_style(subobj, default_settings, **kwargs)
         if style.label is None:
             style.label = str(type(subobj).__name__)
-        if parent_legendgroup is not None:
-            legendgroup = parent_legendgroup
-        else:
-            legendgroup = f"{subobj}"
+        legendgroup = f"{subobj}" if parent_legendgroup is None else parent_legendgroup
+        label = (
+            get_legend_label(subobj, style=style)
+            if parent_label is None
+            else parent_label
+        )
         if parent_color is not None and style.color is None:
             style.color = parent_color
         elif style.color is None:
             style.color = next(color_cycle)
         flat_objs[subobj] = {
             "legendgroup": legendgroup,
             "style": style,
-            "legendtext": parent_label,
+            "legendtext": label,
             "showlegend": parent_showlegend,
         }
         if isCollection:
-            label = get_legend_label(subobj, style=style)
             flat_objs.update(
                 get_flatten_objects_properties_recursive(
                     *subobj.children,
                     colorsequence=colorsequence,
                     color_cycle=color_cycle,
                     parent_legendgroup=legendgroup,
                     parent_color=style.color,
```

### Comparing `magpylib-5.0.0rc0/magpylib/_src/fields/field_BH_circle.py` & `magpylib-5.0.1/magpylib/_src/fields/field_BH_circle.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/magpylib/_src/fields/field_BH_cuboid.py` & `magpylib-5.0.1/magpylib/_src/fields/field_BH_cuboid.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/magpylib/_src/fields/field_BH_cylinder.py` & `magpylib-5.0.1/magpylib/_src/fields/field_BH_cylinder.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/magpylib/_src/fields/field_BH_cylinder_segment.py` & `magpylib-5.0.1/magpylib/_src/fields/field_BH_cylinder_segment.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/magpylib/_src/fields/field_BH_dipole.py` & `magpylib-5.0.1/magpylib/_src/fields/field_BH_dipole.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/magpylib/_src/fields/field_BH_polyline.py` & `magpylib-5.0.1/magpylib/_src/fields/field_BH_polyline.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/magpylib/_src/fields/field_BH_sphere.py` & `magpylib-5.0.1/magpylib/_src/fields/field_BH_sphere.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/magpylib/_src/fields/field_BH_tetrahedron.py` & `magpylib-5.0.1/magpylib/_src/fields/field_BH_tetrahedron.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/magpylib/_src/fields/field_BH_triangle.py` & `magpylib-5.0.1/magpylib/_src/fields/field_BH_triangle.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/magpylib/_src/fields/field_BH_triangularmesh.py` & `magpylib-5.0.1/magpylib/_src/fields/field_BH_triangularmesh.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/magpylib/_src/fields/field_wrap_BH.py` & `magpylib-5.0.1/magpylib/_src/fields/field_wrap_BH.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,14 +237,15 @@
                         "An open mesh may return bad results."
                     )
 
     # format observers input:
     #   allow only bare sensor, collection, pos_vec or list thereof
     #   transform input into an ordered list of sensors (pos_vec->pixel)
     #   check if all pixel shapes are similar - or else if pixel_agg is given
+
     pixel_agg_func = check_format_pixel_agg(pixel_agg)
     sensors, pix_shapes = check_format_input_observers(observers, pixel_agg)
     pix_nums = [
         int(np.prod(ps[:-1])) for ps in pix_shapes
     ]  # number of pixel for each sensor
     pix_inds = np.cumsum([0] + pix_nums)  # cumulative indices of pixel for each sensor
     pix_all_same = len(set(pix_shapes)) == 1
```

### Comparing `magpylib-5.0.0rc0/magpylib/_src/fields/special_cel.py` & `magpylib-5.0.1/magpylib/_src/fields/special_cel.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/magpylib/_src/fields/special_el3.py` & `magpylib-5.0.1/magpylib/_src/fields/special_el3.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/magpylib/_src/input_checks.py` & `magpylib-5.0.1/magpylib/_src/input_checks.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/magpylib/_src/obj_classes/class_BaseDisplayRepr.py` & `magpylib-5.0.1/magpylib/_src/obj_classes/class_BaseDisplayRepr.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/magpylib/_src/obj_classes/class_BaseExcitations.py` & `magpylib-5.0.1/magpylib/_src/obj_classes/class_BaseExcitations.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/magpylib/_src/obj_classes/class_BaseGeo.py` & `magpylib-5.0.1/magpylib/_src/obj_classes/class_BaseGeo.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/magpylib/_src/obj_classes/class_BaseTransform.py` & `magpylib-5.0.1/magpylib/_src/obj_classes/class_BaseTransform.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/magpylib/_src/obj_classes/class_Collection.py` & `magpylib-5.0.1/magpylib/_src/obj_classes/class_Collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -497,30 +497,42 @@
                 for k, v in style_kwargs.items()
                 if k.split("_")[0] in child.style.as_dict()
             }
             child.style.update(**style_kwargs_specific, _match_properties=True)
         return self
 
     def _validate_getBH_inputs(self, *inputs):
-        """validate Collection.getBH inputs"""
+        """
+        select correct sources and observers for getBHJM_level2
+        """
         # pylint: disable=protected-access
         # pylint: disable=too-many-branches
         current_sources = format_obj_input(self, allow="sources")
         current_sensors = format_obj_input(self, allow="sensors")
+
+        # if collection includes source and observer objects, select itself as
+        #   source and observer in gethBH
         if current_sensors and current_sources:
             sources, sensors = self, self
             if inputs:
                 raise MagpylibBadUserInput(
                     "Collections with sensors and sources do not allow `collection.getB()` inputs."
                     "Consider using `magpy.getB()` instead."
                 )
+        # if collection has no sources, *inputs must be the sources
         elif not current_sources:
             sources, sensors = inputs, self
+
+        # if collection has no sensors, *inputs must be the observers
         elif not current_sensors:
-            sources, sensors = self, inputs
+            if len(inputs) == 1:
+                sources, sensors = self, inputs[0]
+            else:
+                sources, sensors = self, inputs
+
         return sources, sensors
 
     def getB(
         self, *inputs, squeeze=True, pixel_agg=None, output="ndarray", in_out="auto"
     ):
         """Compute B-field for given sources and observers.
 
@@ -592,15 +604,14 @@
           [0.         0.         0.08333333]]
         <BLANKLINE>
          [[0.         0.         0.08333333]
           [0.         0.         0.08333333]]]
         """
 
         sources, sensors = self._validate_getBH_inputs(*inputs)
-
         return getBH_level2(
             sources,
             sensors,
             field="B",
             sumup=False,
             squeeze=squeeze,
             pixel_agg=pixel_agg,
```

### Comparing `magpylib-5.0.0rc0/magpylib/_src/obj_classes/class_Sensor.py` & `magpylib-5.0.1/magpylib/_src/obj_classes/class_Sensor.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/magpylib/_src/obj_classes/class_current_Circle.py` & `magpylib-5.0.1/magpylib/_src/obj_classes/class_current_Circle.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/magpylib/_src/obj_classes/class_current_Polyline.py` & `magpylib-5.0.1/magpylib/_src/obj_classes/class_current_Polyline.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/magpylib/_src/obj_classes/class_magnet_Cuboid.py` & `magpylib-5.0.1/magpylib/_src/obj_classes/class_magnet_Cuboid.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/magpylib/_src/obj_classes/class_magnet_Cylinder.py` & `magpylib-5.0.1/magpylib/_src/obj_classes/class_magnet_Cylinder.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/magpylib/_src/obj_classes/class_magnet_CylinderSegment.py` & `magpylib-5.0.1/magpylib/_src/obj_classes/class_magnet_CylinderSegment.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/magpylib/_src/obj_classes/class_magnet_Sphere.py` & `magpylib-5.0.1/magpylib/_src/obj_classes/class_magnet_Sphere.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/magpylib/_src/obj_classes/class_magnet_Tetrahedron.py` & `magpylib-5.0.1/magpylib/_src/obj_classes/class_magnet_Tetrahedron.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/magpylib/_src/obj_classes/class_magnet_TriangularMesh.py` & `magpylib-5.0.1/magpylib/_src/obj_classes/class_magnet_TriangularMesh.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/magpylib/_src/obj_classes/class_misc_CustomSource.py` & `magpylib-5.0.1/magpylib/_src/obj_classes/class_misc_CustomSource.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/magpylib/_src/obj_classes/class_misc_Dipole.py` & `magpylib-5.0.1/magpylib/_src/obj_classes/class_misc_Dipole.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/magpylib/_src/obj_classes/class_misc_Triangle.py` & `magpylib-5.0.1/magpylib/_src/obj_classes/class_misc_Triangle.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/magpylib/_src/style.py` & `magpylib-5.0.1/magpylib/_src/style.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/magpylib/_src/utility.py` & `magpylib-5.0.1/magpylib/_src/utility.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/magpylib/core/__init__.py` & `magpylib-5.0.1/magpylib/core/__init__.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/magpylib/graphics/model3d/__init__.py` & `magpylib-5.0.1/magpylib/graphics/model3d/__init__.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/magpylib/magnet/__init__.py` & `magpylib-5.0.1/magpylib/magnet/__init__.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/pyproject.toml` & `magpylib-5.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/tests/test_BHMJ_level.py` & `magpylib-5.0.1/tests/test_BHMJ_level.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/tests/test_BaseTransform.py` & `magpylib-5.0.1/tests/test_BaseTransform.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/tests/test_Coumpound_setters.py` & `magpylib-5.0.1/tests/test_Coumpound_setters.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/tests/test_CustomSource.py` & `magpylib-5.0.1/tests/test_CustomSource.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/tests/test__missing_optional_modules.py` & `magpylib-5.0.1/tests/test__missing_optional_modules.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/tests/test_core_physics_consistency.py` & `magpylib-5.0.1/tests/test_core_physics_consistency.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/tests/test_default_utils.py` & `magpylib-5.0.1/tests/test_default_utils.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/tests/test_defaults.py` & `magpylib-5.0.1/tests/test_defaults.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/tests/test_display_matplotlib.py` & `magpylib-5.0.1/tests/test_display_matplotlib.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/tests/test_display_plotly.py` & `magpylib-5.0.1/tests/test_display_plotly.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/tests/test_display_pyvista.py` & `magpylib-5.0.1/tests/test_display_pyvista.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/tests/test_display_utility.py` & `magpylib-5.0.1/tests/test_display_utility.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/tests/test_elliptics.py` & `magpylib-5.0.1/tests/test_elliptics.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/tests/test_exceptions.py` & `magpylib-5.0.1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/tests/test_field_cylinder.py` & `magpylib-5.0.1/tests/test_field_cylinder.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/tests/test_getBH_dict.py` & `magpylib-5.0.1/tests/test_getBH_dict.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/tests/test_getBH_interfaces.py` & `magpylib-5.0.1/tests/test_getBH_interfaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -360,25 +360,24 @@
         MagpylibMissingInput,
         match=rf"Parameter `{missing_arg}` of .* must be set.",
     ):
         getattr(getattr(magpy, module), class_)(**kwargs).getB([0, 0, 0])
 
 
 @pytest.mark.parametrize("field", ("H", "B", "M", "J"))
-@pytest.mark.parametrize("in_out", ("auto", "inside", "outside"))
-def test_getHBMJ_self_consistency(field, in_out):
+def test_getHBMJ_self_consistency(field):
     """test getHBMJ self consistency"""
     sources = [
         magpy.magnet.Cuboid(dimension=(1, 1, 1), polarization=(0, 0, 1)),
         magpy.current.Circle(diameter=1, current=1),
     ]
     sens = magpy.Sensor(position=np.linspace((-1, 0, 0), (1, 0, 0), 10))
     src = sources[0]
 
-    F1 = getattr(magpy, f"get{field}")(src, sens, in_out=in_out)
-    F2 = getattr(sens, f"get{field}")(src, in_out=in_out)
-    F3 = getattr(src, f"get{field}")(sens, in_out=in_out)
-    F4 = getattr(magpy.Collection(src, sens), f"get{field}")(in_out=in_out)
+    F1 = getattr(magpy, f"get{field}")(src, sens)
+    F2 = getattr(sens, f"get{field}")(src)
+    F3 = getattr(src, f"get{field}")(sens)
+    F4 = getattr(magpy.Collection(src, sens), f"get{field}")()
 
     np.testing.assert_allclose(F1, F2)
     np.testing.assert_allclose(F1, F3)
     np.testing.assert_allclose(F1, F4)
```

### Comparing `magpylib-5.0.0rc0/tests/test_getBH_level2.py` & `magpylib-5.0.1/tests/test_getBH_level2.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/tests/test_input_checks.py` & `magpylib-5.0.1/tests/test_input_checks.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/tests/test_numerical_stability.py` & `magpylib-5.0.1/tests/test_numerical_stability.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/tests/test_obj_BaseGeo.py` & `magpylib-5.0.1/tests/test_obj_BaseGeo.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/tests/test_obj_BaseGeo_v4motion.py` & `magpylib-5.0.1/tests/test_obj_BaseGeo_v4motion.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/tests/test_obj_Circle.py` & `magpylib-5.0.1/tests/test_obj_Circle.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/tests/test_obj_Collection.py` & `magpylib-5.0.1/tests/test_obj_Collection.py`

 * *Files 4% similar despite different names*

```diff
@@ -446,7 +446,24 @@
         "        • magnetization: None A/m",
         "        • polarization: None T",
     ]
     assert "".join(test) == re.sub("id=*[0-9]*[0-9]", "id=REGEX", "".join(desc))
 
     desc = cc.describe()
     assert desc is None
+
+
+def test_col_getBH_input_format():
+    """
+    Collections should produce the same BHJM shapes as individual
+    sources.
+    """
+    cube = magpy.magnet.Cuboid(
+        polarization=(0, 0, 1),
+        dimension=(2, 2, 2),
+    )
+    coll = magpy.Collection(cube)
+
+    for obs in [(0, 0, 0), [(0, 0, 0)], [[(0, 0, 0)]]]:
+        shape1 = cube.getB(obs, squeeze=False).shape
+        shape2 = coll.getB(obs, squeeze=False).shape
+        assert np.all(shape1 == shape2)
```

### Comparing `magpylib-5.0.0rc0/tests/test_obj_Collection_child_parent.py` & `magpylib-5.0.1/tests/test_obj_Collection_child_parent.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/tests/test_obj_Collection_v4motion.py` & `magpylib-5.0.1/tests/test_obj_Collection_v4motion.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/tests/test_obj_Cuboid.py` & `magpylib-5.0.1/tests/test_obj_Cuboid.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/tests/test_obj_Cylinder.py` & `magpylib-5.0.1/tests/test_obj_Cylinder.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/tests/test_obj_CylinderSegment.py` & `magpylib-5.0.1/tests/test_obj_CylinderSegment.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/tests/test_obj_Dipole.py` & `magpylib-5.0.1/tests/test_obj_Dipole.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/tests/test_obj_Polyline.py` & `magpylib-5.0.1/tests/test_obj_Polyline.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/tests/test_obj_Sensor.py` & `magpylib-5.0.1/tests/test_obj_Sensor.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/tests/test_obj_Sphere.py` & `magpylib-5.0.1/tests/test_obj_Sphere.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/tests/test_obj_Tetrahedron.py` & `magpylib-5.0.1/tests/test_obj_Tetrahedron.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/tests/test_obj_Triangle.py` & `magpylib-5.0.1/tests/test_obj_Triangle.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/tests/test_obj_TriangularMesh.py` & `magpylib-5.0.1/tests/test_obj_TriangularMesh.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/tests/test_path.py` & `magpylib-5.0.1/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/tests/test_physics_consistency.py` & `magpylib-5.0.1/tests/test_physics_consistency.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/tests/test_scaling.py` & `magpylib-5.0.1/tests/test_scaling.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/tests/test_utility.py` & `magpylib-5.0.1/tests/test_utility.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/tests/test_vs_mag2.py` & `magpylib-5.0.1/tests/test_vs_mag2.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/tests/testdata/testdata_Collection.p` & `magpylib-5.0.1/tests/testdata/testdata_Collection.p`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/tests/testdata/testdata_Collection_setter.npy` & `magpylib-5.0.1/tests/testdata/testdata_Collection_setter.npy`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/tests/testdata/testdata_Cuboid.p` & `magpylib-5.0.1/tests/testdata/testdata_Cuboid.p`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/tests/testdata/testdata_Sphere.p` & `magpylib-5.0.1/tests/testdata/testdata_Sphere.p`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/tests/testdata/testdata_compound_setter_cases.npy` & `magpylib-5.0.1/tests/testdata/testdata_compound_setter_cases.npy`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/tests/testdata/testdata_cy_cases.npy` & `magpylib-5.0.1/tests/testdata/testdata_cy_cases.npy`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/tests/testdata/testdata_el3.npy` & `magpylib-5.0.1/tests/testdata/testdata_el3.npy`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/tests/testdata/testdata_el3_angle.npy` & `magpylib-5.0.1/tests/testdata/testdata_el3_angle.npy`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/tests/testdata/testdata_femDat_cylinder_tile2.npy` & `magpylib-5.0.1/tests/testdata/testdata_femDat_cylinder_tile2.npy`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/tests/testdata/testdata_field_BH_cuboid.p` & `magpylib-5.0.1/tests/testdata/testdata_field_BH_cuboid.p`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/tests/testdata/testdata_field_BH_cylinder.p` & `magpylib-5.0.1/tests/testdata/testdata_field_BH_cylinder.p`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/tests/testdata/testdata_full_cyl.npy` & `magpylib-5.0.1/tests/testdata/testdata_full_cyl.npy`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/tests/testdata/testdata_path_BaseGeo.p` & `magpylib-5.0.1/tests/testdata/testdata_path_BaseGeo.p`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/tests/testdata/testdata_vs_mag2.p` & `magpylib-5.0.1/tests/testdata/testdata_vs_mag2.p`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/tox.ini` & `magpylib-5.0.1/tox.ini`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.0rc0/PKG-INFO` & `magpylib-5.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magpylib
-Version: 5.0.0rc0
+Version: 5.0.1
 Summary: Free Python3 package to compute magnetic fields.
 Keywords: magnetism,physics,analytical,electromagnetic,magnetic-field,B-field
 Author-email: Michael Ortner <magpylib@gmail.com>
 Maintainer-email: Alexandre Boisselet <alexabois+magpylib@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
@@ -72,15 +72,15 @@
 </a>
 <a href="https://codecov.io/gh/magpylib/magpylib"> <img src="https://codecov.io/gh/magpylib/magpylib/branch/main/graph/badge.svg">
 </a>
 <a href="https://pypi.org/project/magpylib/"> <img src="https://badge.fury.io/py/magpylib.svg" alt="PyPI version" height="18">
 </a>
 <a href="https://anaconda.org/conda-forge/magpylib"> <img src="https://anaconda.org/conda-forge/magpylib/badges/version.svg" alt="Conda Cloud" height="18">
 </a>
-<a href="https://mybinder.org/v2/gh/magpylib/magpylib/5.0.0rc0?filepath=docs%2Fexamples"> <img src="https://mybinder.org/badge_logo.svg" alt="MyBinder link" height="18">
+<a href="https://mybinder.org/v2/gh/magpylib/magpylib/5.0.0?filepath=docs%2Fexamples"> <img src="https://mybinder.org/badge_logo.svg" alt="MyBinder link" height="18">
 </a>
 <a href="https://github.com/psf/black"> <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="black" height="18">
 </a>
 </div>
 
 Magpylib is a Python package for calculating **3D static magnetic fields** of magnets, line currents and other sources. The computation is based on explicit expressions and is therefore **extremely fast**. A **user friendly API** enables convenient positioning of sources and observers.
 
@@ -188,12 +188,12 @@
 A valid software citation could be
 
 ```
 @software{magpylib,
     author = {{Michael-Ortner et al.}},
     title = {magpylib},
     url = {https://magpylib.readthedocs.io/en/latest/},
-    version = {5.0.0rc0},
+    version = {5.0.1},
     date = {2023-06-25},
 }
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: magpylib Version: 5.0.0rc0 Summary: Free Python3
+Metadata-Version: 2.1 Name: magpylib Version: 5.0.1 Summary: Free Python3
 package to compute magnetic fields. Keywords:
 magnetism,physics,analytical,electromagnetic,magnetic-field,B-field Author-
 email: Michael Ortner
 gmail.com> Maintainer-email: Alexandre Boisselet
 magpylib@gmail.com> Requires-Python: >=3.8 Description-Content-Type: text/
 markdown Classifier: Development Status :: 5 - Production/Stable Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
@@ -106,9 +106,9 @@
 bibtex entry for the [2020 open-access paper](https://www.sciencedirect.com/
 science/article/pii/S2352711020300170) would be ``` @article
 {ortner2020magpylib, title={Magpylib: A free Python package for magnetic field
 computation}, author={Ortner, Michael and Bandeira, Lucas Gabriel Coliado},
 journal={SoftwareX}, volume={11}, pages={100466}, year={2020}, publisher=
 {Elsevier} } ``` A valid software citation could be ``` @software{magpylib,
 author = {{Michael-Ortner et al.}}, title = {magpylib}, url = {https://
-magpylib.readthedocs.io/en/latest/}, version = {5.0.0rc0}, date = {2023-06-25},
-} ```
+magpylib.readthedocs.io/en/latest/}, version = {5.0.1}, date = {2023-06-25}, }
+```
```

