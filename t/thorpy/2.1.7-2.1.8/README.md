# Comparing `tmp/thorpy-2.1.7.tar.gz` & `tmp/thorpy-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thorpy-2.1.7.tar", last modified: Wed Feb 28 15:35:54 2024, max compression
+gzip compressed data, was "thorpy-2.1.8.tar", last modified: Fri Apr 12 12:31:10 2024, max compression
```

## Comparing `thorpy-2.1.7.tar` & `thorpy-2.1.8.tar`

### file list

```diff
@@ -1,86 +1,102 @@
-drwxrwxrwx   0        0        0        0 2024-02-28 15:35:54.392514 thorpy-2.1.7/
--rw-rw-rw-   0        0        0     1093 2023-04-18 20:35:49.000000 thorpy-2.1.7/LICENSE
--rw-rw-rw-   0        0        0      378 2024-02-28 15:35:54.391513 thorpy-2.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     3341 2023-12-05 07:59:41.000000 thorpy-2.1.7/README.md
--rw-rw-rw-   0        0        0       42 2024-02-28 15:35:54.392514 thorpy-2.1.7/setup.cfg
--rw-rw-rw-   0        0        0      748 2024-02-28 15:33:36.000000 thorpy-2.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-28 15:35:54.326875 thorpy-2.1.7/thorpy/
--rw-rw-rw-   0        0        0     4950 2024-02-28 15:30:35.000000 thorpy-2.1.7/thorpy/__init__.py
--rw-rw-rw-   0        0        0    68339 2024-02-28 15:33:29.000000 thorpy-2.1.7/thorpy/canonical.py
--rw-rw-rw-   0        0        0   143061 2024-02-28 12:15:55.000000 thorpy-2.1.7/thorpy/elements.py
-drwxrwxrwx   0        0        0        0 2024-02-28 15:35:54.390515 thorpy-2.1.7/thorpy/examples/
--rw-rw-rw-   0        0        0        0 2023-05-11 18:30:45.000000 thorpy-2.1.7/thorpy/examples/__init__.py
--rw-rw-rw-   0        0        0     1132 2023-08-03 20:52:52.000000 thorpy-2.1.7/thorpy/examples/_example_alert.py
--rw-rw-rw-   0        0        0     1959 2023-08-29 06:32:12.000000 thorpy-2.1.7/thorpy/examples/_example_alert2.py
--rw-rw-rw-   0        0        0     1245 2023-10-05 08:12:13.000000 thorpy-2.1.7/thorpy/examples/_example_anim_move.py
--rw-rw-rw-   0        0        0     1707 2023-08-29 06:44:41.000000 thorpy-2.1.7/thorpy/examples/_example_animatedgif.py
--rw-rw-rw-   0        0        0      990 2023-10-04 00:47:25.000000 thorpy-2.1.7/thorpy/examples/_example_box.py
--rw-rw-rw-   0        0        0      861 2023-09-09 14:09:55.000000 thorpy-2.1.7/thorpy/examples/_example_button_helloworld.py
--rw-rw-rw-   0        0        0      876 2023-10-05 09:24:46.000000 thorpy-2.1.7/thorpy/examples/_example_color_gradient.py
--rw-rw-rw-   0        0        0     1183 2023-08-29 06:45:55.000000 thorpy-2.1.7/thorpy/examples/_example_colorpicker.py
--rw-rw-rw-   0        0        0     2400 2023-05-11 18:30:45.000000 thorpy-2.1.7/thorpy/examples/_example_colorpicker2.py
--rw-rw-rw-   0        0        0     2402 2023-10-05 22:09:14.000000 thorpy-2.1.7/thorpy/examples/_example_colorpicker_fine_tuning.py
--rw-rw-rw-   0        0        0     3297 2023-08-29 06:46:52.000000 thorpy-2.1.7/thorpy/examples/_example_create_style.py
--rw-rw-rw-   0        0        0     3425 2023-08-29 06:47:09.000000 thorpy-2.1.7/thorpy/examples/_example_create_style2.py
--rw-rw-rw-   0        0        0     2286 2023-10-04 17:33:53.000000 thorpy-2.1.7/thorpy/examples/_example_custom_theme.py
--rw-rw-rw-   0        0        0      957 2023-09-09 14:45:14.000000 thorpy-2.1.7/thorpy/examples/_example_discrete_lifebar.py
--rw-rw-rw-   0        0        0     1836 2023-09-09 14:39:39.000000 thorpy-2.1.7/thorpy/examples/_example_discrete_lifebar_fine_tuned.py
--rw-rw-rw-   0        0        0     2088 2023-10-23 19:03:54.000000 thorpy-2.1.7/thorpy/examples/_example_dropdownlist.py
--rw-rw-rw-   0        0        0     1790 2023-10-04 17:28:01.000000 thorpy-2.1.7/thorpy/examples/_example_events.py
--rw-rw-rw-   0        0        0     1177 2023-05-11 18:30:45.000000 thorpy-2.1.7/thorpy/examples/_example_filebrowser.py
--rw-rw-rw-   0        0        0     2207 2023-09-08 22:18:02.000000 thorpy-2.1.7/thorpy/examples/_example_fx_light_emitting_image.py
--rw-rw-rw-   0        0        0     3249 2023-11-14 10:42:13.000000 thorpy-2.1.7/thorpy/examples/_example_fx_lights.py
--rw-rw-rw-   0        0        0     1210 2024-01-02 14:56:15.000000 thorpy-2.1.7/thorpy/examples/_example_fx_sine_deformation.py
--rw-rw-rw-   0        0        0     1984 2023-05-11 18:30:45.000000 thorpy-2.1.7/thorpy/examples/_example_get_value_from_elements.py
--rw-rw-rw-   0        0        0     1376 2023-05-11 18:30:45.000000 thorpy-2.1.7/thorpy/examples/_example_grouping.py
--rw-rw-rw-   0        0        0     1112 2023-05-11 18:30:45.000000 thorpy-2.1.7/thorpy/examples/_example_grouping_without_sorting.py
--rw-rw-rw-   0        0        0     2575 2023-10-23 18:10:17.000000 thorpy-2.1.7/thorpy/examples/_example_groups_of_groups.py
--rw-rw-rw-   0        0        0     4418 2023-10-24 00:53:45.000000 thorpy-2.1.7/thorpy/examples/_example_guess_the_number.py
--rw-rw-rw-   0        0        0     1573 2023-10-23 17:10:26.000000 thorpy-2.1.7/thorpy/examples/_example_helper.py
--rw-rw-rw-   0        0        0      999 2023-09-10 02:55:55.000000 thorpy-2.1.7/thorpy/examples/_example_heterogeneous_texts.py
--rw-rw-rw-   0        0        0      684 2023-08-29 06:49:06.000000 thorpy-2.1.7/thorpy/examples/_example_image_with_text.py
--rw-rw-rw-   0        0        0     1322 2023-05-11 18:30:45.000000 thorpy-2.1.7/thorpy/examples/_example_imagebutton.py
--rw-rw-rw-   0        0        0     1560 2023-10-24 01:01:35.000000 thorpy-2.1.7/thorpy/examples/_example_integration_in_existing_code.py
--rw-rw-rw-   0        0        0     1316 2023-08-09 18:22:49.000000 thorpy-2.1.7/thorpy/examples/_example_labels.py
--rw-rw-rw-   0        0        0     3028 2023-05-11 18:30:45.000000 thorpy-2.1.7/thorpy/examples/_example_launch.py
--rw-rw-rw-   0        0        0     1287 2023-10-24 01:36:57.000000 thorpy-2.1.7/thorpy/examples/_example_lifebar.py
--rw-rw-rw-   0        0        0     2092 2023-10-24 18:47:13.000000 thorpy-2.1.7/thorpy/examples/_example_listview.py
--rw-rw-rw-   0        0        0     2037 2024-02-28 15:30:59.000000 thorpy-2.1.7/thorpy/examples/_example_listview2.py
--rw-rw-rw-   0        0        0     1305 2023-05-11 18:30:45.000000 thorpy-2.1.7/thorpy/examples/_example_look_tune.py
--rw-rw-rw-   0        0        0     1472 2023-08-31 07:03:07.000000 thorpy-2.1.7/thorpy/examples/_example_opacity.py
--rw-rw-rw-   0        0        0     2297 2023-08-30 15:23:07.000000 thorpy-2.1.7/thorpy/examples/_example_rich_text.py
--rw-rw-rw-   0        0        0     1573 2023-08-09 18:51:20.000000 thorpy-2.1.7/thorpy/examples/_example_rotations.py
--rw-rw-rw-   0        0        0     1307 2023-05-11 18:30:45.000000 thorpy-2.1.7/thorpy/examples/_example_set_default_font.py
--rw-rw-rw-   0        0        0     2128 2023-08-29 06:52:03.000000 thorpy-2.1.7/thorpy/examples/_example_shadows.py
--rw-rw-rw-   0        0        0     3129 2023-10-24 01:38:22.000000 thorpy-2.1.7/thorpy/examples/_example_showcase_themes.py
--rw-rw-rw-   0        0        0     3184 2023-10-05 08:07:55.000000 thorpy-2.1.7/thorpy/examples/_example_showcase_themes2.py
--rw-rw-rw-   0        0        0     2175 2023-09-09 14:20:08.000000 thorpy-2.1.7/thorpy/examples/_example_showcase_themes_buttons.py
--rw-rw-rw-   0        0        0     1500 2023-05-11 18:30:45.000000 thorpy-2.1.7/thorpy/examples/_example_showfps.py
--rw-rw-rw-   0        0        0     1660 2023-10-24 00:53:48.000000 thorpy-2.1.7/thorpy/examples/_example_slider.py
--rw-rw-rw-   0        0        0     2373 2023-09-23 10:07:44.000000 thorpy-2.1.7/thorpy/examples/_example_text_input.py
--rw-rw-rw-   0        0        0     1738 2023-09-10 02:35:47.000000 thorpy-2.1.7/thorpy/examples/_example_text_outliner.py
--rw-rw-rw-   0        0        0     2765 2023-05-11 18:30:45.000000 thorpy-2.1.7/thorpy/examples/_example_text_width.py
--rw-rw-rw-   0        0        0     1987 2023-09-23 10:07:06.000000 thorpy-2.1.7/thorpy/examples/_example_textinput_direct_launch.py
--rw-rw-rw-   0        0        0     1278 2023-09-09 14:19:47.000000 thorpy-2.1.7/thorpy/examples/_example_theme_outlined.py
--rw-rw-rw-   0        0        0     1402 2023-10-24 16:28:11.000000 thorpy-2.1.7/thorpy/examples/_example_togglables_pool.py
--rw-rw-rw-   0        0        0     1105 2023-10-01 16:49:18.000000 thorpy-2.1.7/thorpy/examples/_example_user_choices.py
--rw-rw-rw-   0        0        0     1431 2023-05-11 18:30:45.000000 thorpy-2.1.7/thorpy/examples/_example_user_choices2.py
--rw-rw-rw-   0        0        0     2051 2023-05-11 18:30:45.000000 thorpy-2.1.7/thorpy/examples/_example_user_chooses_font.py
--rw-rw-rw-   0        0        0     2222 2023-10-24 01:37:29.000000 thorpy-2.1.7/thorpy/examples/_example_waiting_bar.py
--rw-rw-rw-   0        0        0     5805 2023-10-29 10:20:31.000000 thorpy-2.1.7/thorpy/gametools.py
--rw-rw-rw-   0        0        0    47298 2024-01-02 14:56:19.000000 thorpy-2.1.7/thorpy/graphics.py
--rw-rw-rw-   0        0        0     6879 2023-10-23 18:04:42.000000 thorpy-2.1.7/thorpy/loops.py
--rw-rw-rw-   0        0        0     2408 2023-12-07 17:47:20.000000 thorpy-2.1.7/thorpy/monitoring.py
--rw-rw-rw-   0        0        0      833 2023-11-14 09:24:11.000000 thorpy-2.1.7/thorpy/parameters.py
--rw-rw-rw-   0        0        0      625 2023-08-28 16:22:16.000000 thorpy-2.1.7/thorpy/setup.py
--rw-rw-rw-   0        0        0     3716 2023-10-14 10:30:59.000000 thorpy-2.1.7/thorpy/shadows.py
--rw-rw-rw-   0        0        0     3825 2024-02-28 15:27:17.000000 thorpy-2.1.7/thorpy/sorting.py
--rw-rw-rw-   0        0        0     2307 2023-08-28 16:22:16.000000 thorpy-2.1.7/thorpy/sound.py
--rw-rw-rw-   0        0        0    36958 2023-10-24 01:39:53.000000 thorpy-2.1.7/thorpy/styles.py
--rw-rw-rw-   0        0        0    36393 2023-10-24 14:56:57.000000 thorpy-2.1.7/thorpy/themes.py
--rw-rw-rw-   0        0        0     1315 2023-10-23 17:47:37.000000 thorpy-2.1.7/thorpy/thorpytypehints.py
-drwxrwxrwx   0        0        0        0 2024-02-28 15:35:54.340810 thorpy-2.1.7/thorpy.egg-info/
--rw-rw-rw-   0        0        0      378 2024-02-28 15:35:54.000000 thorpy-2.1.7/thorpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2845 2024-02-28 15:35:54.000000 thorpy-2.1.7/thorpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-28 15:35:54.000000 thorpy-2.1.7/thorpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-02-28 15:35:54.000000 thorpy-2.1.7/thorpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 12:31:10.365908 thorpy-2.1.8/
+-rw-rw-rw-   0        0        0     1093 2023-04-18 20:35:49.000000 thorpy-2.1.8/LICENSE
+-rw-rw-rw-   0        0        0      357 2024-04-12 12:31:10.364906 thorpy-2.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3341 2023-12-05 07:59:41.000000 thorpy-2.1.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-12 12:31:10.365908 thorpy-2.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      748 2024-04-12 12:28:40.000000 thorpy-2.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 12:31:10.254850 thorpy-2.1.8/thorpy/
+-rw-rw-rw-   0        0        0     4950 2024-04-12 12:27:45.000000 thorpy-2.1.8/thorpy/__init__.py
+-rw-rw-rw-   0        0        0    68257 2024-04-06 19:18:46.000000 thorpy-2.1.8/thorpy/canonical.py
+drwxrwxrwx   0        0        0        0 2024-04-12 12:31:10.317798 thorpy-2.1.8/thorpy/data/
+-rw-rw-rw-   0        0        0  1970691 2023-05-11 18:30:45.000000 thorpy-2.1.8/thorpy/data/bck.jpg
+-rw-rw-rw-   0        0        0      174 2023-05-11 18:30:45.000000 thorpy-2.1.8/thorpy/data/check.png
+-rw-rw-rw-   0        0        0      486 2020-02-21 08:51:41.000000 thorpy-2.1.8/thorpy/data/coin.png
+-rw-rw-rw-   0        0        0      486 2020-02-21 08:51:41.000000 thorpy-2.1.8/thorpy/data/coin_32.png
+-rw-rw-rw-   0        0        0    35713 2023-05-11 18:30:45.000000 thorpy-2.1.8/thorpy/data/explosion.gif
+-rw-rw-rw-   0        0        0      192 2023-09-29 11:49:27.000000 thorpy-2.1.8/thorpy/data/heart_empty_16.png
+-rw-rw-rw-   0        0        0      291 2023-09-09 14:42:57.000000 thorpy-2.1.8/thorpy/data/heart_empty_32.png
+-rw-rw-rw-   0        0        0      201 2023-09-29 11:50:17.000000 thorpy-2.1.8/thorpy/data/heart_full_16.png
+-rw-rw-rw-   0        0        0      978 2023-09-09 14:43:38.000000 thorpy-2.1.8/thorpy/data/heart_full_32.png
+-rw-rw-rw-   0        0        0      718 2023-05-11 18:30:45.000000 thorpy-2.1.8/thorpy/data/my_img.png
+-rw-rw-rw-   0        0        0      192 2023-09-08 22:56:01.000000 thorpy-2.1.8/thorpy/data/star_empty_16.png
+-rw-rw-rw-   0        0        0      369 2023-09-08 22:43:00.000000 thorpy-2.1.8/thorpy/data/star_empty_32.png
+-rw-rw-rw-   0        0        0      195 2023-09-08 22:56:20.000000 thorpy-2.1.8/thorpy/data/star_full_16.png
+-rw-rw-rw-   0        0        0      390 2023-09-08 22:42:38.000000 thorpy-2.1.8/thorpy/data/star_full_32.png
+-rw-rw-rw-   0        0        0   143151 2024-04-06 19:14:54.000000 thorpy-2.1.8/thorpy/elements.py
+drwxrwxrwx   0        0        0        0 2024-04-12 12:31:10.363909 thorpy-2.1.8/thorpy/examples/
+-rw-rw-rw-   0        0        0        0 2023-05-11 18:30:45.000000 thorpy-2.1.8/thorpy/examples/__init__.py
+-rw-rw-rw-   0        0        0     1132 2024-04-06 19:24:00.000000 thorpy-2.1.8/thorpy/examples/_example_alert.py
+-rw-rw-rw-   0        0        0     1959 2023-08-29 06:32:12.000000 thorpy-2.1.8/thorpy/examples/_example_alert2.py
+-rw-rw-rw-   0        0        0     1245 2023-10-05 08:12:13.000000 thorpy-2.1.8/thorpy/examples/_example_anim_move.py
+-rw-rw-rw-   0        0        0     1707 2023-08-29 06:44:41.000000 thorpy-2.1.8/thorpy/examples/_example_animatedgif.py
+-rw-rw-rw-   0        0        0      990 2023-10-04 00:47:25.000000 thorpy-2.1.8/thorpy/examples/_example_box.py
+-rw-rw-rw-   0        0        0      861 2023-09-09 14:09:55.000000 thorpy-2.1.8/thorpy/examples/_example_button_helloworld.py
+-rw-rw-rw-   0        0        0      876 2023-10-05 09:24:46.000000 thorpy-2.1.8/thorpy/examples/_example_color_gradient.py
+-rw-rw-rw-   0        0        0     1183 2023-08-29 06:45:55.000000 thorpy-2.1.8/thorpy/examples/_example_colorpicker.py
+-rw-rw-rw-   0        0        0     2400 2023-05-11 18:30:45.000000 thorpy-2.1.8/thorpy/examples/_example_colorpicker2.py
+-rw-rw-rw-   0        0        0     2402 2023-10-05 22:09:14.000000 thorpy-2.1.8/thorpy/examples/_example_colorpicker_fine_tuning.py
+-rw-rw-rw-   0        0        0     3297 2023-08-29 06:46:52.000000 thorpy-2.1.8/thorpy/examples/_example_create_style.py
+-rw-rw-rw-   0        0        0     3425 2023-08-29 06:47:09.000000 thorpy-2.1.8/thorpy/examples/_example_create_style2.py
+-rw-rw-rw-   0        0        0     2286 2023-10-04 17:33:53.000000 thorpy-2.1.8/thorpy/examples/_example_custom_theme.py
+-rw-rw-rw-   0        0        0      957 2023-09-09 14:45:14.000000 thorpy-2.1.8/thorpy/examples/_example_discrete_lifebar.py
+-rw-rw-rw-   0        0        0     1836 2023-09-09 14:39:39.000000 thorpy-2.1.8/thorpy/examples/_example_discrete_lifebar_fine_tuned.py
+-rw-rw-rw-   0        0        0     2088 2023-10-23 19:03:54.000000 thorpy-2.1.8/thorpy/examples/_example_dropdownlist.py
+-rw-rw-rw-   0        0        0     1790 2023-10-04 17:28:01.000000 thorpy-2.1.8/thorpy/examples/_example_events.py
+-rw-rw-rw-   0        0        0     1177 2023-05-11 18:30:45.000000 thorpy-2.1.8/thorpy/examples/_example_filebrowser.py
+-rw-rw-rw-   0        0        0     2192 2024-04-06 19:23:42.000000 thorpy-2.1.8/thorpy/examples/_example_fx_light_emitting_image.py
+-rw-rw-rw-   0        0        0     3249 2023-11-14 10:42:13.000000 thorpy-2.1.8/thorpy/examples/_example_fx_lights.py
+-rw-rw-rw-   0        0        0     1210 2024-01-02 14:56:15.000000 thorpy-2.1.8/thorpy/examples/_example_fx_sine_deformation.py
+-rw-rw-rw-   0        0        0     1984 2023-05-11 18:30:45.000000 thorpy-2.1.8/thorpy/examples/_example_get_value_from_elements.py
+-rw-rw-rw-   0        0        0     1376 2023-05-11 18:30:45.000000 thorpy-2.1.8/thorpy/examples/_example_grouping.py
+-rw-rw-rw-   0        0        0     1112 2023-05-11 18:30:45.000000 thorpy-2.1.8/thorpy/examples/_example_grouping_without_sorting.py
+-rw-rw-rw-   0        0        0     2575 2023-10-23 18:10:17.000000 thorpy-2.1.8/thorpy/examples/_example_groups_of_groups.py
+-rw-rw-rw-   0        0        0     4418 2023-10-24 00:53:45.000000 thorpy-2.1.8/thorpy/examples/_example_guess_the_number.py
+-rw-rw-rw-   0        0        0     1573 2023-10-23 17:10:26.000000 thorpy-2.1.8/thorpy/examples/_example_helper.py
+-rw-rw-rw-   0        0        0      999 2023-09-10 02:55:55.000000 thorpy-2.1.8/thorpy/examples/_example_heterogeneous_texts.py
+-rw-rw-rw-   0        0        0      684 2023-08-29 06:49:06.000000 thorpy-2.1.8/thorpy/examples/_example_image_with_text.py
+-rw-rw-rw-   0        0        0     1322 2023-05-11 18:30:45.000000 thorpy-2.1.8/thorpy/examples/_example_imagebutton.py
+-rw-rw-rw-   0        0        0     1560 2023-10-24 01:01:35.000000 thorpy-2.1.8/thorpy/examples/_example_integration_in_existing_code.py
+-rw-rw-rw-   0        0        0     1316 2023-08-09 18:22:49.000000 thorpy-2.1.8/thorpy/examples/_example_labels.py
+-rw-rw-rw-   0        0        0     3028 2023-05-11 18:30:45.000000 thorpy-2.1.8/thorpy/examples/_example_launch.py
+-rw-rw-rw-   0        0        0     1287 2023-10-24 01:36:57.000000 thorpy-2.1.8/thorpy/examples/_example_lifebar.py
+-rw-rw-rw-   0        0        0     2092 2023-10-24 18:47:13.000000 thorpy-2.1.8/thorpy/examples/_example_listview.py
+-rw-rw-rw-   0        0        0     2037 2024-02-28 15:30:59.000000 thorpy-2.1.8/thorpy/examples/_example_listview2.py
+-rw-rw-rw-   0        0        0     1305 2023-05-11 18:30:45.000000 thorpy-2.1.8/thorpy/examples/_example_look_tune.py
+-rw-rw-rw-   0        0        0     1472 2023-08-31 07:03:07.000000 thorpy-2.1.8/thorpy/examples/_example_opacity.py
+-rw-rw-rw-   0        0        0     2297 2023-08-30 15:23:07.000000 thorpy-2.1.8/thorpy/examples/_example_rich_text.py
+-rw-rw-rw-   0        0        0     1573 2023-08-09 18:51:20.000000 thorpy-2.1.8/thorpy/examples/_example_rotations.py
+-rw-rw-rw-   0        0        0     1307 2023-05-11 18:30:45.000000 thorpy-2.1.8/thorpy/examples/_example_set_default_font.py
+-rw-rw-rw-   0        0        0     2128 2023-08-29 06:52:03.000000 thorpy-2.1.8/thorpy/examples/_example_shadows.py
+-rw-rw-rw-   0        0        0     3129 2023-10-24 01:38:22.000000 thorpy-2.1.8/thorpy/examples/_example_showcase_themes.py
+-rw-rw-rw-   0        0        0     3184 2024-04-06 19:24:11.000000 thorpy-2.1.8/thorpy/examples/_example_showcase_themes2.py
+-rw-rw-rw-   0        0        0     2175 2023-09-09 14:20:08.000000 thorpy-2.1.8/thorpy/examples/_example_showcase_themes_buttons.py
+-rw-rw-rw-   0        0        0     1500 2023-05-11 18:30:45.000000 thorpy-2.1.8/thorpy/examples/_example_showfps.py
+-rw-rw-rw-   0        0        0     1660 2023-10-24 00:53:48.000000 thorpy-2.1.8/thorpy/examples/_example_slider.py
+-rw-rw-rw-   0        0        0     2373 2023-09-23 10:07:44.000000 thorpy-2.1.8/thorpy/examples/_example_text_input.py
+-rw-rw-rw-   0        0        0     1738 2023-09-10 02:35:47.000000 thorpy-2.1.8/thorpy/examples/_example_text_outliner.py
+-rw-rw-rw-   0        0        0     2765 2023-05-11 18:30:45.000000 thorpy-2.1.8/thorpy/examples/_example_text_width.py
+-rw-rw-rw-   0        0        0     1987 2023-09-23 10:07:06.000000 thorpy-2.1.8/thorpy/examples/_example_textinput_direct_launch.py
+-rw-rw-rw-   0        0        0     1278 2023-09-09 14:19:47.000000 thorpy-2.1.8/thorpy/examples/_example_theme_outlined.py
+-rw-rw-rw-   0        0        0     1402 2023-10-24 16:28:11.000000 thorpy-2.1.8/thorpy/examples/_example_togglables_pool.py
+-rw-rw-rw-   0        0        0     1105 2023-10-01 16:49:18.000000 thorpy-2.1.8/thorpy/examples/_example_user_choices.py
+-rw-rw-rw-   0        0        0     1431 2023-05-11 18:30:45.000000 thorpy-2.1.8/thorpy/examples/_example_user_choices2.py
+-rw-rw-rw-   0        0        0     2051 2023-05-11 18:30:45.000000 thorpy-2.1.8/thorpy/examples/_example_user_chooses_font.py
+-rw-rw-rw-   0        0        0     2222 2023-10-24 01:37:29.000000 thorpy-2.1.8/thorpy/examples/_example_waiting_bar.py
+-rw-rw-rw-   0        0        0     5805 2023-10-29 10:20:31.000000 thorpy-2.1.8/thorpy/gametools.py
+-rw-rw-rw-   0        0        0    48631 2024-04-06 19:17:14.000000 thorpy-2.1.8/thorpy/graphics.py
+-rw-rw-rw-   0        0        0     6879 2023-10-23 18:04:42.000000 thorpy-2.1.8/thorpy/loops.py
+-rw-rw-rw-   0        0        0     2408 2023-12-07 17:47:20.000000 thorpy-2.1.8/thorpy/monitoring.py
+-rw-rw-rw-   0        0        0      833 2023-11-14 09:24:11.000000 thorpy-2.1.8/thorpy/parameters.py
+-rw-rw-rw-   0        0        0        0 2023-10-04 16:26:55.000000 thorpy-2.1.8/thorpy/py.typed
+-rw-rw-rw-   0        0        0      625 2023-08-28 16:22:16.000000 thorpy-2.1.8/thorpy/setup.py
+-rw-rw-rw-   0        0        0     3716 2023-10-14 10:30:59.000000 thorpy-2.1.8/thorpy/shadows.py
+-rw-rw-rw-   0        0        0     3825 2024-02-28 15:27:17.000000 thorpy-2.1.8/thorpy/sorting.py
+-rw-rw-rw-   0        0        0     2307 2023-08-28 16:22:16.000000 thorpy-2.1.8/thorpy/sound.py
+-rw-rw-rw-   0        0        0    36954 2024-04-06 19:24:02.000000 thorpy-2.1.8/thorpy/styles.py
+-rw-rw-rw-   0        0        0    36393 2023-10-24 14:56:57.000000 thorpy-2.1.8/thorpy/themes.py
+-rw-rw-rw-   0        0        0     1315 2023-10-23 17:47:37.000000 thorpy-2.1.8/thorpy/thorpytypehints.py
+drwxrwxrwx   0        0        0        0 2024-04-12 12:31:10.363909 thorpy-2.1.8/thorpy.egg-info/
+-rw-rw-rw-   0        0        0      357 2024-04-12 12:31:10.000000 thorpy-2.1.8/thorpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3237 2024-04-12 12:31:10.000000 thorpy-2.1.8/thorpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 12:31:10.000000 thorpy-2.1.8/thorpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-12 12:31:10.000000 thorpy-2.1.8/thorpy.egg-info/top_level.txt
```

### Comparing `thorpy-2.1.7/LICENSE` & `thorpy-2.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/README.md` & `thorpy-2.1.8/README.md`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/setup.py` & `thorpy-2.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages, setup
 
 # import thorpy
 # print("VERSION", thorpy.__version__)
 
-version = "2.1.7"
+version = "2.1.8"
 # assert thorpy.__version__ == version #security control
 
 setup(name='thorpy',
       version=version,
       description='GUI library for pygame',
       long_description='ThorPy is a non-intrusive, straightforward GUI kit for Pygame.',
       author='Yann Thorimbert',
```

### Comparing `thorpy-2.1.7/thorpy/__init__.py` & `thorpy-2.1.8/thorpy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "2.1.7"
+__version__ = "2.1.8"
 
 import os
 from . import elements
 from . import styles
 from . import loops
 from .loops import Loop
 from . import parameters
```

### Comparing `thorpy-2.1.7/thorpy/canonical.py` & `thorpy-2.1.8/thorpy/canonical.py`

 * *Files 1% similar despite different names*

```diff
@@ -1003,18 +1003,15 @@
        
     def get_current_shadow_frame(self)->Optional[pygame.Surface]:
         return self.shadows.get(self.state)[self.i_frame] #type:ignore #guaranteed
    
     def get_rect(self)->pygame.Rect:
         """_Returns (and updates!) the current rect of the element, using its current state."""
         if self.get_current_style():
-            current_center = self.rect.center
-            r = self.get_current_frame().get_rect()
-            r.center = current_center
-            return r
+            return self.get_current_frame().get_rect(center=self.rect.center)
         else:
             return self.rect
 
     def extract_all_helpers(self)->List["Element"]:
         """_Get a list of all the descendants helpers."""
         helpers = [e.helper for e in self.get_all_descendants() if e.helper]
         return helpers
```

### Comparing `thorpy-2.1.7/thorpy/elements.py` & `thorpy-2.1.8/thorpy/elements.py`

 * *Files 1% similar despite different names*

```diff
@@ -1327,24 +1327,27 @@
 
     def update(self,  mouse_delta):
         dragged = Element.update(self,  mouse_delta)
         if self.event_parent.state == "hover":
             self.time_before_launch -= 1
             self.last_parent_state_was_hover = True
         elif self.last_parent_state_was_hover:
-            self.time_before_launch = self.countdown
-            self.anchor = None
+            self.reset_countdown_and_anchor()
         #
 
         if self.time_before_launch <= 0:
             if not self.anchor or self.follow_mouse:
                 self.anchor = pygame.mouse.get_pos()
             self.set_center(*self.anchor)
             self.move(*self.offset)
         return dragged
+    
+    def reset_countdown_and_anchor(self):
+        self.time_before_launch = self.countdown
+        self.anchor = None
 
 class ColorPicker(Element):
     """Allows the user to pick a color in a pseudo continuum of colors.
     ***Optional arguments***
     <mode> : either 'google', 'red', 'green' or 'blue'.
     <initial_value> : initial color of the color picker. Experimental : may not be very accurate in some cases.
     <slider_align> : either 'h' or 'v' for horizontal or vertical slider bar.
@@ -3241,8 +3244,8 @@
 class _ColorFrameForColorPicker(DeadButton):
     ...
 
 class _ButtonColor(Button):
     ...
 
 class _SelectButton(ToggleButton):
-    ...
+    ...
```

### Comparing `thorpy-2.1.7/thorpy/examples/_example_alert.py` & `thorpy-2.1.8/thorpy/examples/_example_alert.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/examples/_example_alert2.py` & `thorpy-2.1.8/thorpy/examples/_example_alert2.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/examples/_example_anim_move.py` & `thorpy-2.1.8/thorpy/examples/_example_anim_move.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/examples/_example_animatedgif.py` & `thorpy-2.1.8/thorpy/examples/_example_animatedgif.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/examples/_example_box.py` & `thorpy-2.1.8/thorpy/examples/_example_box.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/examples/_example_button_helloworld.py` & `thorpy-2.1.8/thorpy/examples/_example_button_helloworld.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/examples/_example_color_gradient.py` & `thorpy-2.1.8/thorpy/examples/_example_color_gradient.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/examples/_example_colorpicker.py` & `thorpy-2.1.8/thorpy/examples/_example_colorpicker.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/examples/_example_colorpicker2.py` & `thorpy-2.1.8/thorpy/examples/_example_colorpicker2.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/examples/_example_colorpicker_fine_tuning.py` & `thorpy-2.1.8/thorpy/examples/_example_colorpicker_fine_tuning.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/examples/_example_create_style.py` & `thorpy-2.1.8/thorpy/examples/_example_create_style.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/examples/_example_create_style2.py` & `thorpy-2.1.8/thorpy/examples/_example_create_style2.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/examples/_example_custom_theme.py` & `thorpy-2.1.8/thorpy/examples/_example_custom_theme.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/examples/_example_discrete_lifebar.py` & `thorpy-2.1.8/thorpy/examples/_example_discrete_lifebar.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/examples/_example_discrete_lifebar_fine_tuned.py` & `thorpy-2.1.8/thorpy/examples/_example_discrete_lifebar_fine_tuned.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/examples/_example_dropdownlist.py` & `thorpy-2.1.8/thorpy/examples/_example_dropdownlist.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/examples/_example_events.py` & `thorpy-2.1.8/thorpy/examples/_example_events.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/examples/_example_filebrowser.py` & `thorpy-2.1.8/thorpy/examples/_example_filebrowser.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/examples/_example_fx_light_emitting_image.py` & `thorpy-2.1.8/thorpy/examples/_example_fx_light_emitting_image.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """We show here how to make an object emit light"""
 #tags: light, fx, light emitter, light emission, lighting, emit light, oscillating light, oscillating, generate_oscillating_lights, image
-import pygame, sys, thorpy as tp
+import pygame, thorpy as tp
 
 from thorpy.graphics import generate_oscillating_lights as gen_lights
 
 pygame.init()
 W, H = 800,600
 screen = pygame.display.set_mode((W, H))
 
@@ -46,17 +46,16 @@
 while playing:
     screen.blit(bck, (0,0))
     # screen.blit(my_img, my_img_rect) #blit base image (instead of e.draw if you want)
     e.draw()
     #get and blit the bright image around
     if iteration % 2 == 0: #choose the speed of the animation
         i_light = (i_light+1)%len(my_img_lights)
-    r = my_img_lights[i_light].get_rect()
+    r = my_img_lights[i_light].get_rect(center=e.rect.center)
     # r.center = my_img_rect.center #move base image (instead of e if you want)
-    r.center = e.rect.center
     screen.blit(my_img_lights[i_light], r.topleft)
 
     events = pygame.event.get()
     for event in events:
         if event.type == pygame.QUIT:
             playing = False
     ... #your stuff goes here
```

### Comparing `thorpy-2.1.7/thorpy/examples/_example_fx_lights.py` & `thorpy-2.1.8/thorpy/examples/_example_fx_lights.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/examples/_example_fx_sine_deformation.py` & `thorpy-2.1.8/thorpy/examples/_example_fx_sine_deformation.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/examples/_example_get_value_from_elements.py` & `thorpy-2.1.8/thorpy/examples/_example_get_value_from_elements.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/examples/_example_grouping.py` & `thorpy-2.1.8/thorpy/examples/_example_grouping.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/examples/_example_grouping_without_sorting.py` & `thorpy-2.1.8/thorpy/examples/_example_grouping_without_sorting.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/examples/_example_groups_of_groups.py` & `thorpy-2.1.8/thorpy/examples/_example_groups_of_groups.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/examples/_example_guess_the_number.py` & `thorpy-2.1.8/thorpy/examples/_example_guess_the_number.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/examples/_example_helper.py` & `thorpy-2.1.8/thorpy/examples/_example_helper.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/examples/_example_heterogeneous_texts.py` & `thorpy-2.1.8/thorpy/examples/_example_heterogeneous_texts.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/examples/_example_image_with_text.py` & `thorpy-2.1.8/thorpy/examples/_example_image_with_text.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/examples/_example_imagebutton.py` & `thorpy-2.1.8/thorpy/examples/_example_imagebutton.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/examples/_example_integration_in_existing_code.py` & `thorpy-2.1.8/thorpy/examples/_example_integration_in_existing_code.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/examples/_example_labels.py` & `thorpy-2.1.8/thorpy/examples/_example_labels.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/examples/_example_launch.py` & `thorpy-2.1.8/thorpy/examples/_example_launch.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/examples/_example_lifebar.py` & `thorpy-2.1.8/thorpy/examples/_example_lifebar.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/examples/_example_listview.py` & `thorpy-2.1.8/thorpy/examples/_example_listview.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/examples/_example_listview2.py` & `thorpy-2.1.8/thorpy/examples/_example_listview2.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/examples/_example_look_tune.py` & `thorpy-2.1.8/thorpy/examples/_example_look_tune.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/examples/_example_opacity.py` & `thorpy-2.1.8/thorpy/examples/_example_opacity.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/examples/_example_rich_text.py` & `thorpy-2.1.8/thorpy/examples/_example_rich_text.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/examples/_example_rotations.py` & `thorpy-2.1.8/thorpy/examples/_example_rotations.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/examples/_example_set_default_font.py` & `thorpy-2.1.8/thorpy/examples/_example_set_default_font.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/examples/_example_shadows.py` & `thorpy-2.1.8/thorpy/examples/_example_shadows.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/examples/_example_showcase_themes.py` & `thorpy-2.1.8/thorpy/examples/_example_showcase_themes.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/examples/_example_showcase_themes2.py` & `thorpy-2.1.8/thorpy/examples/_example_showcase_themes2.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/examples/_example_showcase_themes_buttons.py` & `thorpy-2.1.8/thorpy/examples/_example_showcase_themes_buttons.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/examples/_example_showfps.py` & `thorpy-2.1.8/thorpy/examples/_example_showfps.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/examples/_example_slider.py` & `thorpy-2.1.8/thorpy/examples/_example_slider.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/examples/_example_text_input.py` & `thorpy-2.1.8/thorpy/examples/_example_text_input.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/examples/_example_text_outliner.py` & `thorpy-2.1.8/thorpy/examples/_example_text_outliner.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/examples/_example_text_width.py` & `thorpy-2.1.8/thorpy/examples/_example_text_width.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/examples/_example_textinput_direct_launch.py` & `thorpy-2.1.8/thorpy/examples/_example_textinput_direct_launch.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/examples/_example_theme_outlined.py` & `thorpy-2.1.8/thorpy/examples/_example_theme_outlined.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/examples/_example_togglables_pool.py` & `thorpy-2.1.8/thorpy/examples/_example_togglables_pool.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/examples/_example_user_choices.py` & `thorpy-2.1.8/thorpy/examples/_example_user_choices.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/examples/_example_user_choices2.py` & `thorpy-2.1.8/thorpy/examples/_example_user_choices2.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/examples/_example_user_chooses_font.py` & `thorpy-2.1.8/thorpy/examples/_example_user_chooses_font.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/examples/_example_waiting_bar.py` & `thorpy-2.1.8/thorpy/examples/_example_waiting_bar.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/gametools.py` & `thorpy-2.1.8/thorpy/gametools.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/graphics.py` & `thorpy-2.1.8/thorpy/graphics.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,19 +53,19 @@
     <color> : 3-tuple or 4-tuple color.
     ***Optional arguments***
     <factor> : (float) how much of the color we want to increase. E.g. 1.2 means we want
     to get 120% of the original color.
     <min_value> : minimum value of color components in 255 bytes format.
     also_alpha : (bool) specify whether you also want alpha to be affected."""
     color = get_main_color(color)
-    assert factor >= 1
+    assert factor >= 1, "Factor for color enlightment must be >= 1"
     def mc(value):
         return min(int(value*factor + min_value),255)
     if len(color) > 3:
-        color = cast(RGBA, color)  # Explicitly tell mypy that color is RGBA in this block
+
         if also_alpha:
             return mc(color[0]), mc(color[1]), mc(color[2]), mc(color[3])
         else:
             return mc(color[0]), mc(color[1]), mc(color[2]), color[3]
     else:
         return mc(color[0]), mc(color[1]), mc(color[2])
 
@@ -86,15 +86,15 @@
         gradient_color = cast(RGBA, gradient_color)
         return gradient_color, None # type: ignore
     
 
 
 def get_main_color(gradient_color:GradientColor)->RGB_OR_RGBA:
     all_colors, orientation = process_gradient_color(gradient_color)
-    if orientation:
+    if orientation: #orientation is None if the color is a simple RGB or RGBA tuple
         return all_colors[0] # type: ignore
     return all_colors # type: ignore
 
 def interpolate_2colors(c1:RGB_OR_RGBA, c2:RGB_OR_RGBA, k:float)->RGB_OR_RGBA:
     """Returns a color that is in between c1 and c2, with a factor k.
     For instance, if k = 0.75, then the color will be made of 75% of c1 and 25% of c2.
     Note that c1 and c2 must be of the same length in RGB or RGBA format.
@@ -142,17 +142,19 @@
 # def is_color_gradient(color:GradientColor)->bool:
 #     return isinstance(color, Gradient)
 #     # if isinstance(color[0],int) or isinstance(color[0],float):
 #     #     return False
 #     # return True
 
 def is_color_gradient(color:GradientColor)->bool:
-    if isinstance(color[0],int) or isinstance(color[0],float):
-        return False
-    return True
+    # return not isinstance(color[0], (int, float))
+    return not np.issubdtype(type(color[0]), np.number) #type:ignore (à garder dans version finale)
+    # if isinstance(color[0],int) or isinstance(color[0],float):
+    #     return False
+    # return True
 
 def get_alpha(color:RGB_OR_RGBA)->float:
     color = get_main_color(color)
     if len(color) < 4:
         return 255
     color = cast(RGBA, color)
     return color[3]
@@ -1048,14 +1050,35 @@
             color = surface.get_at((x,y))
             if color != color_empty:
                 new_color = darken(color, factor) #type:ignore #pygame casts it
                 #maybe surface.set_at(...) is more performant than gfx.pixel
                 gfx.pixel(surface, x, y, new_color) #type:ignore #pygame casts it
     return surface
 
+def darken_every_color_except_ip(surface:pygame.Surface,
+                          factor:float=0.5,
+                          except_colors:list[RGB_OR_RGBA_OR_NONE]=None,
+                          color_empty:RGB_OR_RGBA_OR_NONE=None)->pygame.Surface:
+    """This function is very slow and intended to be used once and for all before any loop,
+    most suitably on small sprites. If <color_empty> is None, then it detects the default colorkey
+    of the surface."""
+    if not color_empty:
+        color_empty = surface.get_colorkey()
+    if not color_empty:
+        raise Exception("You must provide <color_empty> or a surface with non-None colorkey")
+    w,h = surface.get_size()
+    for x in range(w): #columns from top to bottom
+        for y in range(h):
+            color = surface.get_at((x,y))
+            if color != color_empty and not(color in except_colors):
+                new_color = darken(color, factor) #type:ignore #pygame casts it
+                #maybe surface.set_at(...) is more performant than gfx.pixel
+                gfx.pixel(surface, x, y, new_color) #type:ignore #pygame casts it
+    return surface
+
 
 TWO_PI:float = 2 * math.pi
 
 def sine_wave_y_on_img(src:pygame.Surface, amplitude:int, step:int, phase:float, dst=None) -> pygame.Surface:
     """Returns a new surface with a sine deformation."""
     w,h = src.get_size()
     if not dst:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `thorpy-2.1.7/thorpy/loops.py` & `thorpy-2.1.8/thorpy/loops.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/monitoring.py` & `thorpy-2.1.8/thorpy/monitoring.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/parameters.py` & `thorpy-2.1.8/thorpy/parameters.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/setup.py` & `thorpy-2.1.8/thorpy/setup.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/shadows.py` & `thorpy-2.1.8/thorpy/shadows.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/sorting.py` & `thorpy-2.1.8/thorpy/sorting.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/sound.py` & `thorpy-2.1.8/thorpy/sound.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/styles.py` & `thorpy-2.1.8/thorpy/styles.py`

 * *Files 0% similar despite different names*

```diff
@@ -505,16 +505,14 @@
         else:
             r_button = pygame.Rect((0,0), self.size)
 
         # s = graphics.color_rect(self.bck_color, r_button.size)
         r_img = img.get_rect()
         r_button.center = r_img.center
         s = img
-
-
         r_text.center = r_button.center
         if not arrow:
             self.blit_text(s,lines,r_text)
         else:
             s.blit(s_text, r_text)
         return [self.offset_surface(s)]
```

### Comparing `thorpy-2.1.7/thorpy/themes.py` & `thorpy-2.1.8/thorpy/themes.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy/thorpytypehints.py` & `thorpy-2.1.8/thorpy/thorpytypehints.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.1.7/thorpy.egg-info/SOURCES.txt` & `thorpy-2.1.8/thorpy.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -5,25 +5,40 @@
 thorpy/canonical.py
 thorpy/elements.py
 thorpy/gametools.py
 thorpy/graphics.py
 thorpy/loops.py
 thorpy/monitoring.py
 thorpy/parameters.py
+thorpy/py.typed
 thorpy/setup.py
 thorpy/shadows.py
 thorpy/sorting.py
 thorpy/sound.py
 thorpy/styles.py
 thorpy/themes.py
 thorpy/thorpytypehints.py
 thorpy.egg-info/PKG-INFO
 thorpy.egg-info/SOURCES.txt
 thorpy.egg-info/dependency_links.txt
 thorpy.egg-info/top_level.txt
+thorpy/data/bck.jpg
+thorpy/data/check.png
+thorpy/data/coin.png
+thorpy/data/coin_32.png
+thorpy/data/explosion.gif
+thorpy/data/heart_empty_16.png
+thorpy/data/heart_empty_32.png
+thorpy/data/heart_full_16.png
+thorpy/data/heart_full_32.png
+thorpy/data/my_img.png
+thorpy/data/star_empty_16.png
+thorpy/data/star_empty_32.png
+thorpy/data/star_full_16.png
+thorpy/data/star_full_32.png
 thorpy/examples/__init__.py
 thorpy/examples/_example_alert.py
 thorpy/examples/_example_alert2.py
 thorpy/examples/_example_anim_move.py
 thorpy/examples/_example_animatedgif.py
 thorpy/examples/_example_box.py
 thorpy/examples/_example_button_helloworld.py
```

