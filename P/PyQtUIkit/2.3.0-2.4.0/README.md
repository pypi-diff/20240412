# Comparing `tmp/PyQtUIkit-2.3.0.tar.gz` & `tmp/PyQtUIkit-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyQtUIkit-2.3.0.tar", last modified: Thu Apr 11 14:06:11 2024, max compression
+gzip compressed data, was "PyQtUIkit-2.4.0.tar", last modified: Fri Apr 12 09:41:55 2024, max compression
```

## Comparing `PyQtUIkit-2.3.0.tar` & `PyQtUIkit-2.4.0.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 14:06:11.050149 PyQtUIkit-2.3.0/
--rw-rw-rw-   0        0        0     1090 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/LICENSE
--rw-rw-rw-   0        0        0     2938 2024-04-11 14:06:11.050149 PyQtUIkit-2.3.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-11 14:06:11.003306 PyQtUIkit-2.3.0/PyQtUIkit/
--rw-rw-rw-   0        0        0       49 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/__init__.py
--rw-rw-rw-   0        0        0     3835 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/_icons.py
-drwxrwxrwx   0        0        0        0 2024-04-11 14:06:11.003306 PyQtUIkit-2.3.0/PyQtUIkit/builder/
--rw-rw-rw-   0        0        0     1116 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/builder/__init__.py
--rw-rw-rw-   0        0        0     1825 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/builder/builder_class.py
--rw-rw-rw-   0        0        0     1383 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/builder/builder_module.py
-drwxrwxrwx   0        0        0        0 2024-04-11 14:06:11.018906 PyQtUIkit-2.3.0/PyQtUIkit/core/
--rw-rw-rw-   0        0        0       84 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/core/__init__.py
--rw-rw-rw-   0        0        0       19 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/core/_version.py
--rw-rw-rw-   0        0        0     1503 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/core/font.py
--rw-rw-rw-   0        0        0     1019 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/core/icon.py
--rw-rw-rw-   0        0        0     4655 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/core/properties.py
-drwxrwxrwx   0        0        0        0 2024-04-11 14:06:11.034532 PyQtUIkit-2.3.0/PyQtUIkit/fonts/
--rw-rw-rw-   0        0        0   168060 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/fonts/Roboto-Black.ttf
--rw-rw-rw-   0        0        0   174108 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/fonts/Roboto-BlackItalic.ttf
--rw-rw-rw-   0        0        0   167336 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/fonts/Roboto-Bold.ttf
--rw-rw-rw-   0        0        0   171508 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/fonts/Roboto-BoldItalic.ttf
--rw-rw-rw-   0        0        0   170504 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/fonts/Roboto-Italic.ttf
--rw-rw-rw-   0        0        0   167000 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/fonts/Roboto-Light.ttf
--rw-rw-rw-   0        0        0   173172 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/fonts/Roboto-LightItalic.ttf
--rw-rw-rw-   0        0        0   168644 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/fonts/Roboto-Medium.ttf
--rw-rw-rw-   0        0        0   173416 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/fonts/Roboto-MediumItalic.ttf
--rw-rw-rw-   0        0        0   168260 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/fonts/Roboto-Regular.ttf
--rw-rw-rw-   0        0        0   168488 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/fonts/Roboto-Thin.ttf
--rw-rw-rw-   0        0        0   172860 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/fonts/Roboto-ThinItalic.ttf
--rw-rw-rw-   0        0        0    87392 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/fonts/RobotoMono-Bold.ttf
--rw-rw-rw-   0        0        0    94636 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf
--rw-rw-rw-   0        0        0    88248 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf
--rw-rw-rw-   0        0        0    94016 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf
--rw-rw-rw-   0        0        0    94372 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/fonts/RobotoMono-Italic.ttf
--rw-rw-rw-   0        0        0    87980 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/fonts/RobotoMono-Light.ttf
--rw-rw-rw-   0        0        0    94256 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf
--rw-rw-rw-   0        0        0    87172 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/fonts/RobotoMono-Medium.ttf
--rw-rw-rw-   0        0        0    94412 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf
--rw-rw-rw-   0        0        0    87236 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/fonts/RobotoMono-Regular.ttf
--rw-rw-rw-   0        0        0    87496 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf
--rw-rw-rw-   0        0        0    94508 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf
--rw-rw-rw-   0        0        0    88288 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/fonts/RobotoMono-Thin.ttf
--rw-rw-rw-   0        0        0    93588 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf
-drwxrwxrwx   0        0        0        0 2024-04-11 14:06:11.034532 PyQtUIkit-2.3.0/PyQtUIkit/themes/
--rw-rw-rw-   0        0        0     2180 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/themes/__init__.py
--rw-rw-rw-   0        0        0     5879 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/themes/builtin_themes.py
--rw-rw-rw-   0        0        0  1676850 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/themes/icons.py
--rw-rw-rw-   0        0        0     1882 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/themes/svg.py
--rw-rw-rw-   0        0        0     1402 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/themes/theme.py
-drwxrwxrwx   0        0        0        0 2024-04-11 14:06:11.050149 PyQtUIkit-2.3.0/PyQtUIkit/widgets/
--rw-rw-rw-   0        0        0     1626 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/widgets/__init__.py
--rw-rw-rw-   0        0        0     3515 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/widgets/_widget.py
--rw-rw-rw-   0        0        0     1359 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/widgets/application.py
--rw-rw-rw-   0        0        0     7833 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/widgets/button.py
--rw-rw-rw-   0        0        0     2785 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/widgets/checkbox.py
--rw-rw-rw-   0        0        0    10004 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/widgets/combo_box.py
--rw-rw-rw-   0        0        0     7027 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/widgets/dialog.py
--rw-rw-rw-   0        0        0     5807 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/widgets/flow_layout.py
--rw-rw-rw-   0        0        0     2280 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/widgets/group.py
--rw-rw-rw-   0        0        0     4293 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/widgets/hbox_layout.py
--rw-rw-rw-   0        0        0     1578 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/widgets/icon_widget.py
--rw-rw-rw-   0        0        0     1100 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/widgets/label.py
--rw-rw-rw-   0        0        0     1487 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/widgets/line_edit.py
--rw-rw-rw-   0        0        0     3448 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/widgets/list_widget.py
--rw-rw-rw-   0        0        0     1424 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/widgets/main_window.py
--rw-rw-rw-   0        0        0     3302 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/widgets/menu.py
--rw-rw-rw-   0        0        0     4336 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/widgets/menu_bar.py
--rw-rw-rw-   0        0        0     7076 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/widgets/navigation.py
--rw-rw-rw-   0        0        0     2647 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/widgets/progress_bar.py
--rw-rw-rw-   0        0        0     6683 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/widgets/radio.py
--rw-rw-rw-   0        0        0     3881 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/widgets/scroll_area.py
--rw-rw-rw-   0        0        0     1486 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/widgets/separator.py
--rw-rw-rw-   0        0        0     7513 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/widgets/spin_box.py
--rw-rw-rw-   0        0        0     3580 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/widgets/spinner.py
--rw-rw-rw-   0        0        0    13356 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/widgets/tab_bar.py
--rw-rw-rw-   0        0        0     1218 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/widgets/tabs.py
--rw-rw-rw-   0        0        0     2167 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/widgets/text_edit.py
--rw-rw-rw-   0        0        0     4465 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/widgets/toggle.py
--rw-rw-rw-   0        0        0    17249 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/widgets/tree_widget.py
--rw-rw-rw-   0        0        0     4620 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/PyQtUIkit/widgets/vbox_layout.py
-drwxrwxrwx   0        0        0        0 2024-04-11 14:06:11.003306 PyQtUIkit-2.3.0/PyQtUIkit.egg-info/
--rw-rw-rw-   0        0        0     2938 2024-04-11 14:06:10.000000 PyQtUIkit-2.3.0/PyQtUIkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2537 2024-04-11 14:06:10.000000 PyQtUIkit-2.3.0/PyQtUIkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 14:06:10.000000 PyQtUIkit-2.3.0/PyQtUIkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-04-11 14:06:10.000000 PyQtUIkit-2.3.0/PyQtUIkit.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       26 2024-04-11 14:06:10.000000 PyQtUIkit-2.3.0/PyQtUIkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-11 14:06:10.000000 PyQtUIkit-2.3.0/PyQtUIkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-11 14:06:11.050149 PyQtUIkit-2.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1411 2024-04-11 14:05:23.000000 PyQtUIkit-2.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 09:41:55.144277 PyQtUIkit-2.4.0/
+-rw-rw-rw-   0        0        0     1090 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/LICENSE
+-rw-rw-rw-   0        0        0     2938 2024-04-12 09:41:55.144277 PyQtUIkit-2.4.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-12 09:41:55.097401 PyQtUIkit-2.4.0/PyQtUIkit/
+-rw-rw-rw-   0        0        0       49 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/__init__.py
+-rw-rw-rw-   0        0        0     3896 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/_icons.py
+drwxrwxrwx   0        0        0        0 2024-04-12 09:41:55.097401 PyQtUIkit-2.4.0/PyQtUIkit/builder/
+-rw-rw-rw-   0        0        0     1116 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/builder/__init__.py
+-rw-rw-rw-   0        0        0     1825 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/builder/builder_class.py
+-rw-rw-rw-   0        0        0     1383 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/builder/builder_module.py
+drwxrwxrwx   0        0        0        0 2024-04-12 09:41:55.097401 PyQtUIkit-2.4.0/PyQtUIkit/core/
+-rw-rw-rw-   0        0        0       84 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/core/__init__.py
+-rw-rw-rw-   0        0        0       19 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/core/_version.py
+-rw-rw-rw-   0        0        0     1503 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/core/font.py
+-rw-rw-rw-   0        0        0     1019 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/core/icon.py
+-rw-rw-rw-   0        0        0     4655 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/core/properties.py
+drwxrwxrwx   0        0        0        0 2024-04-12 09:41:55.113027 PyQtUIkit-2.4.0/PyQtUIkit/fonts/
+-rw-rw-rw-   0        0        0   168060 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/fonts/Roboto-Black.ttf
+-rw-rw-rw-   0        0        0   174108 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/fonts/Roboto-BlackItalic.ttf
+-rw-rw-rw-   0        0        0   167336 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/fonts/Roboto-Bold.ttf
+-rw-rw-rw-   0        0        0   171508 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/fonts/Roboto-BoldItalic.ttf
+-rw-rw-rw-   0        0        0   170504 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/fonts/Roboto-Italic.ttf
+-rw-rw-rw-   0        0        0   167000 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/fonts/Roboto-Light.ttf
+-rw-rw-rw-   0        0        0   173172 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/fonts/Roboto-LightItalic.ttf
+-rw-rw-rw-   0        0        0   168644 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/fonts/Roboto-Medium.ttf
+-rw-rw-rw-   0        0        0   173416 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/fonts/Roboto-MediumItalic.ttf
+-rw-rw-rw-   0        0        0   168260 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/fonts/Roboto-Regular.ttf
+-rw-rw-rw-   0        0        0   168488 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/fonts/Roboto-Thin.ttf
+-rw-rw-rw-   0        0        0   172860 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/fonts/Roboto-ThinItalic.ttf
+-rw-rw-rw-   0        0        0    87392 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/fonts/RobotoMono-Bold.ttf
+-rw-rw-rw-   0        0        0    94636 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf
+-rw-rw-rw-   0        0        0    88248 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf
+-rw-rw-rw-   0        0        0    94016 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf
+-rw-rw-rw-   0        0        0    94372 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/fonts/RobotoMono-Italic.ttf
+-rw-rw-rw-   0        0        0    87980 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/fonts/RobotoMono-Light.ttf
+-rw-rw-rw-   0        0        0    94256 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf
+-rw-rw-rw-   0        0        0    87172 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/fonts/RobotoMono-Medium.ttf
+-rw-rw-rw-   0        0        0    94412 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf
+-rw-rw-rw-   0        0        0    87236 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/fonts/RobotoMono-Regular.ttf
+-rw-rw-rw-   0        0        0    87496 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf
+-rw-rw-rw-   0        0        0    94508 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf
+-rw-rw-rw-   0        0        0    88288 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/fonts/RobotoMono-Thin.ttf
+-rw-rw-rw-   0        0        0    93588 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf
+drwxrwxrwx   0        0        0        0 2024-04-12 09:41:55.128656 PyQtUIkit-2.4.0/PyQtUIkit/themes/
+-rw-rw-rw-   0        0        0     2180 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/themes/__init__.py
+-rw-rw-rw-   0        0        0     5879 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/themes/builtin_themes.py
+-rw-rw-rw-   0        0        0  2340473 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/themes/icons.py
+-rw-rw-rw-   0        0        0     1470 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/themes/svg.py
+-rw-rw-rw-   0        0        0     1402 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/themes/theme.py
+drwxrwxrwx   0        0        0        0 2024-04-12 09:41:55.144277 PyQtUIkit-2.4.0/PyQtUIkit/widgets/
+-rw-rw-rw-   0        0        0     1626 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/widgets/__init__.py
+-rw-rw-rw-   0        0        0     3515 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/widgets/_widget.py
+-rw-rw-rw-   0        0        0     1359 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/widgets/application.py
+-rw-rw-rw-   0        0        0     7833 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/widgets/button.py
+-rw-rw-rw-   0        0        0     2785 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/widgets/checkbox.py
+-rw-rw-rw-   0        0        0    10059 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/widgets/combo_box.py
+-rw-rw-rw-   0        0        0     7021 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/widgets/dialog.py
+-rw-rw-rw-   0        0        0     5807 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/widgets/flow_layout.py
+-rw-rw-rw-   0        0        0     2280 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/widgets/group.py
+-rw-rw-rw-   0        0        0     4293 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/widgets/hbox_layout.py
+-rw-rw-rw-   0        0        0     1578 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/widgets/icon_widget.py
+-rw-rw-rw-   0        0        0     1100 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/widgets/label.py
+-rw-rw-rw-   0        0        0     1487 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/widgets/line_edit.py
+-rw-rw-rw-   0        0        0     3448 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/widgets/list_widget.py
+-rw-rw-rw-   0        0        0     1424 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/widgets/main_window.py
+-rw-rw-rw-   0        0        0     3302 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/widgets/menu.py
+-rw-rw-rw-   0        0        0     4336 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/widgets/menu_bar.py
+-rw-rw-rw-   0        0        0     7084 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/widgets/navigation.py
+-rw-rw-rw-   0        0        0     2647 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/widgets/progress_bar.py
+-rw-rw-rw-   0        0        0     6683 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/widgets/radio.py
+-rw-rw-rw-   0        0        0     3881 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/widgets/scroll_area.py
+-rw-rw-rw-   0        0        0     1486 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/widgets/separator.py
+-rw-rw-rw-   0        0        0     7515 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/widgets/spin_box.py
+-rw-rw-rw-   0        0        0     3580 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/widgets/spinner.py
+-rw-rw-rw-   0        0        0    13353 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/widgets/tab_bar.py
+-rw-rw-rw-   0        0        0     1218 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/widgets/tabs.py
+-rw-rw-rw-   0        0        0     2167 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/widgets/text_edit.py
+-rw-rw-rw-   0        0        0     4465 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/widgets/toggle.py
+-rw-rw-rw-   0        0        0    17251 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/widgets/tree_widget.py
+-rw-rw-rw-   0        0        0     4620 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/PyQtUIkit/widgets/vbox_layout.py
+drwxrwxrwx   0        0        0        0 2024-04-12 09:41:55.097401 PyQtUIkit-2.4.0/PyQtUIkit.egg-info/
+-rw-rw-rw-   0        0        0     2938 2024-04-12 09:41:55.000000 PyQtUIkit-2.4.0/PyQtUIkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2537 2024-04-12 09:41:55.000000 PyQtUIkit-2.4.0/PyQtUIkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 09:41:55.000000 PyQtUIkit-2.4.0/PyQtUIkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-04-12 09:41:55.000000 PyQtUIkit-2.4.0/PyQtUIkit.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       26 2024-04-12 09:41:55.000000 PyQtUIkit-2.4.0/PyQtUIkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-12 09:41:55.000000 PyQtUIkit-2.4.0/PyQtUIkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-12 09:41:55.144277 PyQtUIkit-2.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1411 2024-04-12 09:41:17.000000 PyQtUIkit-2.4.0/setup.py
```

### Comparing `PyQtUIkit-2.3.0/LICENSE` & `PyQtUIkit-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PKG-INFO` & `PyQtUIkit-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQtUIkit
-Version: 2.3.0
+Version: 2.4.0
 Summary: A PyQtUIkit package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/_icons.py` & `PyQtUIkit-2.4.0/PyQtUIkit/_icons.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         top_layout.addWidget(self.line_edit)
 
         self._spinner = KitSpinner()
         self._spinner.size = 18
         self._spinner.width = 3
         top_layout.addWidget(self._spinner)
 
-        self._icon = KitIconWidget('regular-circle-check')
+        self._icon = KitIconWidget('line-checkmark-circle')
         self._icon.setFixedSize(20, 20)
         top_layout.addWidget(self._icon)
 
         self.list_widget = KitListWidget()
         self.list_widget.currentItemChanged.connect(self.select_icon)
         right_layout.addWidget(self.list_widget)
         self.update_icons()
@@ -52,22 +52,24 @@
         right_layout = KitVBoxLayout()
         main_layout.addWidget(right_layout)
 
         self.icon_widget = KitIconWidget()
         right_layout.addWidget(self.icon_widget, 1)
 
         group = KitHGroup()
+        group.height = 24
         group.setSizePolicy(QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Minimum)
         right_layout.addWidget(group)
 
         self.copy_line = KitLineEdit()
         self.copy_line.setReadOnly(True)
         group.addItem(self.copy_line)
 
-        self.copy_button = KitIconButton('regular-copy')
+        self.copy_button = KitIconButton('line-copy')
+        self.copy_button.size = 24
         self.copy_button.clicked.connect(self.copy_icon_name)
         group.addItem(self.copy_button)
 
     def select_icon(self):
         item = self.list_widget.currentItem()
         if item:
             self.icon_widget.icon = item.text()
```

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/builder/__init__.py` & `PyQtUIkit-2.4.0/PyQtUIkit/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/builder/builder_class.py` & `PyQtUIkit-2.4.0/PyQtUIkit/builder/builder_class.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/builder/builder_module.py` & `PyQtUIkit-2.4.0/PyQtUIkit/builder/builder_module.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/core/font.py` & `PyQtUIkit-2.4.0/PyQtUIkit/core/font.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/core/icon.py` & `PyQtUIkit-2.4.0/PyQtUIkit/core/icon.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/core/properties.py` & `PyQtUIkit-2.4.0/PyQtUIkit/core/properties.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/fonts/Roboto-Black.ttf` & `PyQtUIkit-2.4.0/PyQtUIkit/fonts/Roboto-Black.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/fonts/Roboto-BlackItalic.ttf` & `PyQtUIkit-2.4.0/PyQtUIkit/fonts/Roboto-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/fonts/Roboto-Bold.ttf` & `PyQtUIkit-2.4.0/PyQtUIkit/fonts/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/fonts/Roboto-BoldItalic.ttf` & `PyQtUIkit-2.4.0/PyQtUIkit/fonts/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/fonts/Roboto-Italic.ttf` & `PyQtUIkit-2.4.0/PyQtUIkit/fonts/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/fonts/Roboto-Light.ttf` & `PyQtUIkit-2.4.0/PyQtUIkit/fonts/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/fonts/Roboto-LightItalic.ttf` & `PyQtUIkit-2.4.0/PyQtUIkit/fonts/Roboto-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/fonts/Roboto-Medium.ttf` & `PyQtUIkit-2.4.0/PyQtUIkit/fonts/Roboto-Medium.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/fonts/Roboto-MediumItalic.ttf` & `PyQtUIkit-2.4.0/PyQtUIkit/fonts/Roboto-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/fonts/Roboto-Regular.ttf` & `PyQtUIkit-2.4.0/PyQtUIkit/fonts/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/fonts/Roboto-Thin.ttf` & `PyQtUIkit-2.4.0/PyQtUIkit/fonts/Roboto-Thin.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/fonts/Roboto-ThinItalic.ttf` & `PyQtUIkit-2.4.0/PyQtUIkit/fonts/Roboto-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/fonts/RobotoMono-Bold.ttf` & `PyQtUIkit-2.4.0/PyQtUIkit/fonts/RobotoMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf` & `PyQtUIkit-2.4.0/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf` & `PyQtUIkit-2.4.0/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf` & `PyQtUIkit-2.4.0/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/fonts/RobotoMono-Italic.ttf` & `PyQtUIkit-2.4.0/PyQtUIkit/fonts/RobotoMono-Italic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/fonts/RobotoMono-Light.ttf` & `PyQtUIkit-2.4.0/PyQtUIkit/fonts/RobotoMono-Light.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf` & `PyQtUIkit-2.4.0/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/fonts/RobotoMono-Medium.ttf` & `PyQtUIkit-2.4.0/PyQtUIkit/fonts/RobotoMono-Medium.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf` & `PyQtUIkit-2.4.0/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/fonts/RobotoMono-Regular.ttf` & `PyQtUIkit-2.4.0/PyQtUIkit/fonts/RobotoMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf` & `PyQtUIkit-2.4.0/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf` & `PyQtUIkit-2.4.0/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/fonts/RobotoMono-Thin.ttf` & `PyQtUIkit-2.4.0/PyQtUIkit/fonts/RobotoMono-Thin.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf` & `PyQtUIkit-2.4.0/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/themes/__init__.py` & `PyQtUIkit-2.4.0/PyQtUIkit/themes/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/themes/builtin_themes.py` & `PyQtUIkit-2.4.0/PyQtUIkit/themes/builtin_themes.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/themes/svg.py` & `PyQtUIkit-2.4.0/PyQtUIkit/themes/svg.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,37 +2,24 @@
 
 
 class SVG:
     def __init__(self, data):
         self._data = bs4.BeautifulSoup(data, 'xml')
 
     def change_color(self, color):
-
-        tag = self._data.find('svg')
-        fill, stroke = tag.get('fill'), tag.get('stroke')
-        if fill == 'none':
-            fill = None
-        if stroke == 'none':
-            fill = None
-        if fill or stroke:
-            if fill:
+        for tag in self._data.find_all(['path', 'circle', 'polygon', 'rect', 'ellipse', 'line']):
+            fill, stroke = tag.get('fill'), tag.get('stroke')
+            if fill == 'none':
+                fill = None
+            if stroke == 'none':
+                fill = None
+            if fill or not stroke:
                 tag['fill'] = color
             if stroke:
                 tag['stroke'] = color
-        else:
-            for tag in self._data.find_all(['path', 'circle', 'polygon', 'rect', 'ellipse', 'line']):
-                fill, stroke = tag.get('fill'), tag.get('stroke')
-                if fill == 'none':
-                    fill = None
-                if stroke == 'none':
-                    fill = None
-                if fill or not stroke:
-                    tag['fill'] = color
-                if stroke:
-                    tag['stroke'] = color
 
     def set_width(self, width):
         for tag in self._data.find_all('svg'):
             tag['width'] = str(width)
 
     def set_height(self, height):
         for tag in self._data.find_all('svg'):
```

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/themes/theme.py` & `PyQtUIkit-2.4.0/PyQtUIkit/themes/theme.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/widgets/__init__.py` & `PyQtUIkit-2.4.0/PyQtUIkit/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/widgets/_widget.py` & `PyQtUIkit-2.4.0/PyQtUIkit/widgets/_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/widgets/application.py` & `PyQtUIkit-2.4.0/PyQtUIkit/widgets/application.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/widgets/button.py` & `PyQtUIkit-2.4.0/PyQtUIkit/widgets/button.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
             self.setFixedSize(x)
 
     def _apply_theme(self):
         if not self._tm or not self._tm.active:
             return
         self._icon_label.icon = self.icon
         self._icon_label._main_palette = self._main_palette
-        self.__layout.setContentsMargins(*[min(self.width(), self.height()) // 5] * 4)
+        self.__layout.setContentsMargins(*[min(self.width(), self.height()) // 6] * 4)
         self.setStyleSheet(f"""
 QPushButton {{
     background-color: {self.main_palette.main};
     border: {self.border}px solid {self.border_palette.main};
     {self._border_radius_css()}
     padding: 3px 8px 3px 8px;
 }}
```

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/widgets/checkbox.py` & `PyQtUIkit-2.4.0/PyQtUIkit/widgets/checkbox.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/widgets/combo_box.py` & `PyQtUIkit-2.4.0/PyQtUIkit/widgets/combo_box.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from PyQtUIkit.core import IntProperty, PaletteProperty, IconProperty, EnumProperty, KitFont, FontProperty, \
     MethodsProperty
 from PyQtUIkit.widgets._widget import _KitWidget as _KitWidget, KitGroupItem as _KitGroupItem
 from PyQtUIkit.widgets.icon_widget import KitIconWidget
 from PyQtUIkit.widgets.scroll_area import KitScrollArea
 from PyQtUIkit.widgets.vbox_layout import KitVBoxLayout
+from PyQtUIkit.widgets.button import KitLayoutButton
 
 
 class KitComboBoxItem(QPushButton, _KitWidget):
     selected = pyqtSignal(object)
     icon = IconProperty('icon')
     font = FontProperty('font')
     font_size = EnumProperty('font_size', KitFont.Size, KitFont.Size.MEDIUM)
@@ -80,15 +81,15 @@
         self.clicked.connect(self._show_menu)
         self.setCursor(Qt.CursorShape.PointingHandCursor)
 
         layout = QHBoxLayout()
         layout.setAlignment(Qt.AlignmentFlag.AlignRight)
         layout.setContentsMargins(0, 0, 6, 0)
         self.setLayout(layout)
-        self._arrow = KitIconWidget('solid-angle-down')
+        self._arrow = KitIconWidget('line-chevron-down')
         self._arrow._use_text_only = False
         self._arrow.setFixedSize(16, 12)
         layout.addWidget(self._arrow)
 
         for el in values:
             self.addItem(el)
```

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/widgets/dialog.py` & `PyQtUIkit-2.4.0/PyQtUIkit/widgets/dialog.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         self.__top_widget.setFixedHeight(32)
         layout.addWidget(self.__top_widget)
 
         self.__label = QLabel()
         self.__label.setFixedHeight(25)
         self.__top_widget.addWidget(self.__label)
 
-        self.__button_close = KitIconButton('solid-xmark')
+        self.__button_close = KitIconButton('line-close')
         self.__button_close.setFocusPolicy(Qt.FocusPolicy.NoFocus)
         self.__button_close.size = 25
         self.__button_close.border = 0
         self.__button_close.clicked.connect(self.reject)
         self.__top_widget.addWidget(self.__button_close)
 
         self.__widget = KitVBoxLayout()
@@ -87,32 +87,32 @@
     def question(parent, question: str, answers=('No', 'Yes'), default='No'):
         dialog = _KitAskDialog(parent, question, answers, default)
         dialog.exec()
         return dialog.answer
 
     @staticmethod
     def info(parent, title: str, text: str):
-        dialog = _KitMessageBox(parent, title, text, 'solid-circle-info')
+        dialog = _KitMessageBox(parent, title, text, 'sharp-information-circle')
         dialog.exec()
 
     @staticmethod
     def danger(parent, title: str, text: str):
-        dialog = _KitMessageBox(parent, title, text, 'solid-circle-exclamation')
+        dialog = _KitMessageBox(parent, title, text, 'sharp-alert-circle')
         dialog.icon_palette = 'Danger'
         dialog.exec()
 
     @staticmethod
     def warning(parent, title: str, text: str):
-        dialog = _KitMessageBox(parent, title, text, 'solid-triangle-exclamation')
+        dialog = _KitMessageBox(parent, title, text, 'solid-alert-triangle')
         dialog.icon_palette = 'Warning'
         dialog.exec()
 
     @staticmethod
     def success(parent, title: str, text: str):
-        dialog = _KitMessageBox(parent, title, text, 'solid-circle-check')
+        dialog = _KitMessageBox(parent, title, text, 'sharp-checkmark-circle')
         dialog.icon_palette = 'Success'
         dialog.exec()
 
 
 class _KitAskDialog(KitDialog):
     def __init__(self, parent, question: str, answers=('No', 'Yes'), default=''):
         super().__init__(parent)
@@ -128,15 +128,15 @@
 
         layout = KitHBoxLayout()
         layout.setContentsMargins(5, 5, 5, 5)
         layout.setSpacing(15)
         main_layout.addWidget(layout)
 
         self._icon_widget = KitIconWidget()
-        self._icon_widget.icon = 'solid-circle-question'
+        self._icon_widget.icon = 'sharp-help-circle'
         self._icon_widget.setFixedSize(72, 72)
         layout.addWidget(self._icon_widget)
 
         self._label = KitLabel(question)
         self._label.setWordWrap(True)
         layout.addWidget(self._label, 100)
```

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/widgets/flow_layout.py` & `PyQtUIkit-2.4.0/PyQtUIkit/widgets/flow_layout.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/widgets/group.py` & `PyQtUIkit-2.4.0/PyQtUIkit/widgets/group.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/widgets/hbox_layout.py` & `PyQtUIkit-2.4.0/PyQtUIkit/widgets/hbox_layout.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/widgets/icon_widget.py` & `PyQtUIkit-2.4.0/PyQtUIkit/widgets/icon_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/widgets/label.py` & `PyQtUIkit-2.4.0/PyQtUIkit/widgets/label.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/widgets/line_edit.py` & `PyQtUIkit-2.4.0/PyQtUIkit/widgets/line_edit.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/widgets/list_widget.py` & `PyQtUIkit-2.4.0/PyQtUIkit/widgets/list_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/widgets/main_window.py` & `PyQtUIkit-2.4.0/PyQtUIkit/widgets/main_window.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/widgets/menu.py` & `PyQtUIkit-2.4.0/PyQtUIkit/widgets/menu.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/widgets/menu_bar.py` & `PyQtUIkit-2.4.0/PyQtUIkit/widgets/menu_bar.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/widgets/navigation.py` & `PyQtUIkit-2.4.0/PyQtUIkit/widgets/navigation.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         self.__current = None
 
         self.setAlignment(Qt.AlignmentFlag.AlignTop)
         self.setContentsMargins(5, 5, 5, 5)
         self.setSpacing(5)
         self.setSizePolicy(QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding)
 
-        self.__button = KitIconButton('solid-bars')
+        self.__button = KitIconButton('line-reorder-three')
         self.__button.border = 0
         self.__button.clicked.connect(self._on_clicked)
         self.addWidget(self.__button)
 
         self.__anim = None
 
     def _on_clicked(self):
```

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/widgets/progress_bar.py` & `PyQtUIkit-2.4.0/PyQtUIkit/widgets/progress_bar.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/widgets/radio.py` & `PyQtUIkit-2.4.0/PyQtUIkit/widgets/radio.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/widgets/scroll_area.py` & `PyQtUIkit-2.4.0/PyQtUIkit/widgets/scroll_area.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/widgets/separator.py` & `PyQtUIkit-2.4.0/PyQtUIkit/widgets/separator.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/widgets/spin_box.py` & `PyQtUIkit-2.4.0/PyQtUIkit/widgets/spin_box.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,16 +149,16 @@
             border: {self.border}px solid {self.border_palette.hover};
             background-color: {self.main_palette.hover};
         }}
         QLineEdit:focus {{
             border: {self.border}px solid {self.border_palette.selected};
             background-color: {self.main_palette.hover};
         }}""")
-        self._button_up.setIcon(self._tm.icon('solid-angle-up', self.main_palette.text))
-        self._button_down.setIcon(self._tm.icon('solid-angle-down', self.main_palette.text))
+        self._button_up.setIcon(self._tm.icon('line-chevron-up', self.main_palette.text))
+        self._button_down.setIcon(self._tm.icon('line-chevron-down', self.main_palette.text))
         css = f"""
 QPushButton {{
     color: {self.main_palette.text};
     background-color: {self.main_palette.main};
     border: {self.border}px solid {self.border_palette.main};
     border-top-left-radius: 0px;
     border-bottom-left-radius: 0px;
```

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/widgets/spinner.py` & `PyQtUIkit-2.4.0/PyQtUIkit/widgets/spinner.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/widgets/tab_bar.py` & `PyQtUIkit-2.4.0/PyQtUIkit/widgets/tab_bar.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         self.__icon_widget.setFixedSize(18, 18)
         layout.addWidget(self.__icon_widget)
 
         self.__label = KitLabel(name)
         self.__label.setContentsMargins(4, 0, 4, 0)
         layout.addWidget(self.__label)
 
-        self.__button_close = KitIconButton(icon='solid-xmark')
+        self.__button_close = KitIconButton(icon='line-close')
         self.__button_close.border = 0
         self.__button_close.size = 16
         self.__button_close.radius = 8
         self.__button_close.hide()
         self.__button_close.on_click = self.closeRequested.emit
         layout.addWidget(self.__button_close)
 
@@ -150,28 +150,28 @@
         self.__tabs_closable = False
         self.__tabs_movable = False
         self.setContentsMargins(0, 0, 0, 0)
         self.radius = 0
         self.setSpacing(0)
         self._main_palette = 'Bg'
 
-        self.__button_left = KitButton(icon='solid-chevron-left')
+        self.__button_left = KitButton(icon='line-chevron-left')
         self.__button_left.border = 0
         self.__button_left.setFixedWidth(20)
         self.__button_left.clicked.connect(self._scroll_left)
         self.addWidget(self.__button_left)
 
         self.__scroll_area = KitScrollArea()
         self.addWidget(self.__scroll_area)
         self.__layout = _TabLayout(self.__tabs)
         self.__scroll_area.setWidget(self.__layout)
         self.__layout.tabMoved.connect(self.tabMoved.emit)
         self.__scroll_area.setHorizontalScrollBarPolicy(Qt.ScrollBarPolicy.ScrollBarAlwaysOff)
 
-        self.__button_right = KitButton(icon='solid-chevron-right')
+        self.__button_right = KitButton(icon='line-chevron-right')
         self.__button_right.border = 0
         self.__button_right.setFixedWidth(20)
         self.__button_right.clicked.connect(self._scroll_right)
         self.addWidget(self.__button_right)
 
     def addTab(self, tab: str | KitTab):
         self.insertTab(len(self.__tabs), tab)
```

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/widgets/tabs.py` & `PyQtUIkit-2.4.0/PyQtUIkit/widgets/tabs.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/widgets/text_edit.py` & `PyQtUIkit-2.4.0/PyQtUIkit/widgets/text_edit.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/widgets/toggle.py` & `PyQtUIkit-2.4.0/PyQtUIkit/widgets/toggle.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/widgets/tree_widget.py` & `PyQtUIkit-2.4.0/PyQtUIkit/widgets/tree_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -456,13 +456,13 @@
     def _set_tm(self, tm):
         super()._set_tm(tm)
         self.__tree._set_tm(tm)
 
     def _apply_theme(self):
         self.__tree.main_palette = self._main_palette
         self.__widget.setStyleSheet("background-color: transparent;")
-        self._icon1 = self._tm.icon('solid-angle-right', self.main_palette.text)
-        self._icon2 = self._tm.icon('solid-angle-down', self.main_palette.text)
+        self._icon1 = self._tm.icon('line-chevron-right', self.main_palette.text)
+        self._icon2 = self._tm.icon('line-chevron-down', self.main_palette.text)
         self.__tree._main_palette = self._main_palette
         self.__tree._text_palette = self._items_palette
         self.__tree._apply_theme()
         super()._apply_theme()
```

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit/widgets/vbox_layout.py` & `PyQtUIkit-2.4.0/PyQtUIkit/widgets/vbox_layout.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit.egg-info/PKG-INFO` & `PyQtUIkit-2.4.0/PyQtUIkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQtUIkit
-Version: 2.3.0
+Version: 2.4.0
 Summary: A PyQtUIkit package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `PyQtUIkit-2.3.0/PyQtUIkit.egg-info/SOURCES.txt` & `PyQtUIkit-2.4.0/PyQtUIkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.3.0/setup.py` & `PyQtUIkit-2.4.0/setup.py`

 * *Files identical despite different names*

