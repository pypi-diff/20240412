# Comparing `tmp/Red-Web-Dashboard-1.0.0.tar.gz` & `tmp/red_web_dashboard-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Red-Web-Dashboard-1.0.0.tar", last modified: Fri Apr 12 16:00:59 2024, max compression
+gzip compressed data, was "red_web_dashboard-1.1.tar", last modified: Fri Apr 12 18:11:14 2024, max compression
```

## Comparing `Red-Web-Dashboard-1.0.0.tar` & `red_web_dashboard-1.1.tar`

### file list

```diff
@@ -1,293 +1,293 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:00:59.629408 Red-Web-Dashboard-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    34625 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-04-12 16:00:59.629408 Red-Web-Dashboard-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:00:59.629408 Red-Web-Dashboard-1.0.0/Red_Web_Dashboard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-04-12 16:00:59.000000 Red-Web-Dashboard-1.0.0/Red_Web_Dashboard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15750 2024-04-12 16:00:59.000000 Red-Web-Dashboard-1.0.0/Red_Web_Dashboard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 16:00:59.000000 Red-Web-Dashboard-1.0.0/Red_Web_Dashboard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-12 16:00:59.000000 Red-Web-Dashboard-1.0.0/Red_Web_Dashboard.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-12 16:00:59.000000 Red-Web-Dashboard-1.0.0/Red_Web_Dashboard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-12 16:00:59.000000 Red-Web-Dashboard-1.0.0/Red_Web_Dashboard.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:00:59.577407 Red-Web-Dashboard-1.0.0/reddash/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:00:59.577407 Red-Web-Dashboard-1.0.0/reddash/app/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6267 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:00:59.577407 Red-Web-Dashboard-1.0.0/reddash/app/base/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35780 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/base/routes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:00:59.577407 Red-Web-Dashboard-1.0.0/reddash/app/login/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/login/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7456 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/login/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/pagination.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:00:59.569407 Red-Web-Dashboard-1.0.0/reddash/app/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:00:59.585407 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/biometric-icon.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:00:59.589407 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/css/
--rw-r--r--   0 runner    (1001) docker     (127)   480516 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/css/argon-dashboard.css
--rw-r--r--   0 runner    (1001) docker     (127)  1218638 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/css/argon-dashboard.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   381006 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/css/argon-dashboard.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/css/nucleo-icons.css
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/css/nucleo-svg.css
--rw-r--r--   0 runner    (1001) docker     (127)    10929 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/css/simplemde.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   635325 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/error-403.gif
--rw-r--r--   0 runner    (1001) docker     (127)   884014 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/error-404.gif
--rw-r--r--   0 runner    (1001) docker     (127)   824431 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/error-500.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:00:59.589407 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)    18516 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/fonts/nucleo-icons.eot
--rw-r--r--   0 runner    (1001) docker     (127)   126098 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/fonts/nucleo-icons.svg
--rw-r--r--   0 runner    (1001) docker     (127)    18292 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/fonts/nucleo-icons.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    10220 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/fonts/nucleo-icons.woff
--rw-r--r--   0 runner    (1001) docker     (127)     8580 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/fonts/nucleo-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    26524 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/fonts/nucleo.eot
--rw-r--r--   0 runner    (1001) docker     (127)    26364 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/fonts/nucleo.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    15168 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/fonts/nucleo.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12616 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/fonts/nucleo.woff2
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/gulpfile.js
--rw-r--r--   0 runner    (1001) docker     (127)    34128 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/icon-documentation.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:00:59.589407 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/js/
--rw-r--r--   0 runner    (1001) docker     (127)    27282 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/js/argon-dashboard.js
--rw-r--r--   0 runner    (1001) docker     (127)    15415 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/js/argon-dashboard.js.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:00:59.589407 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/js/core/
--rw-r--r--   0 runner    (1001) docker     (127)    48944 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/js/core/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   288580 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/js/core/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    19188 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/js/core/popper.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:00:59.593407 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/js/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/js/plugins/Chart.extension.js
--rw-r--r--   0 runner    (1001) docker     (127)    47524 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/js/plugins/Simple-Full-featured-jQuery-Pagination-System-Pagination-js.zip
--rw-r--r--   0 runner    (1001) docker     (127)    15614 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/js/plugins/bootstrap-notify.js
--rw-r--r--   0 runner    (1001) docker     (127)   176853 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/js/plugins/chartjs.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    19411 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/js/plugins/perfect-scrollbar.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    48421 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/js/plugins/smooth-scrollbar.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     7738 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/js/plugins/utils.js
--rw-r--r--   0 runner    (1001) docker     (127)   140628 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/oauth.png
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/pdf.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/random.svg
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:00:59.593407 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:00:59.601407 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_alert.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_avatars.scss
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_badge.scss
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_breadcrumbs.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_buttons.scss
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_cards.scss
--rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_dark-version.scss
--rw-r--r--   0 runner    (1001) docker     (127)     6683 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_dropdown.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_dropup.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_fixed-plugin.scss
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_footer.scss
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_forms.scss
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_gradients.scss
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_header.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_info-areas.scss
--rw-r--r--   0 runner    (1001) docker     (127)     7009 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_misc.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_nav.scss
--rw-r--r--   0 runner    (1001) docker     (127)    13929 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_navbar-vertical.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_navbar.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_pagination.scss
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_popovers.scss
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_progress.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_rtl.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_social-buttons.scss
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_tables.scss
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_tilt.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_timeline.scss
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_tooltips.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_typography.scss
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_utilities-extend.scss
--rw-r--r--   0 runner    (1001) docker     (127)    16957 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_utilities.scss
--rw-r--r--   0 runner    (1001) docker     (127)    68466 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_variables.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:00:59.605407 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_accordion.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_alert.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_badge.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_breadcrumb.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_button-group.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_buttons.scss
--rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_card.scss
--rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_carousel.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_close.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_containers.scss
--rw-r--r--   0 runner    (1001) docker     (127)     8014 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_dropdown.scss
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_forms.scss
--rw-r--r--   0 runner    (1001) docker     (127)    10558 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_functions.scss
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_grid.scss
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_helpers.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_images.scss
--rw-r--r--   0 runner    (1001) docker     (127)     6348 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_list-group.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_maps.scss
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_mixins.scss
--rw-r--r--   0 runner    (1001) docker     (127)     7762 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_modal.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_nav.scss
--rw-r--r--   0 runner    (1001) docker     (127)     8723 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_navbar.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_offcanvas.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_pagination.scss
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_placeholders.scss
--rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_popover.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_progress.scss
--rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_reboot.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_root.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_spinners.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_tables.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_toasts.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_tooltip.scss
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_transitions.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_type.scss
--rw-r--r--   0 runner    (1001) docker     (127)    14817 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_utilities.scss
--rw-r--r--   0 runner    (1001) docker     (127)    68547 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap-grid.scss
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap-reboot.scss
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap-utilities.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:00:59.609407 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_floating-labels.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-check.scss
--rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-control.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-range.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-select.scss
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-text.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_input-group.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_labels.scss
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_validation.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:00:59.609407 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_clearfix.scss
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_color-bg.scss
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_colored-links.scss
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_position.scss
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_ratio.scss
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_stacks.scss
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_stretched-link.scss
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_text-truncation.scss
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_visually-hidden.scss
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_vr.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:00:59.617407 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_alert.scss
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_backdrop.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_border-radius.scss
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_box-shadow.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_breakpoints.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_buttons.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_caret.scss
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_clearfix.scss
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_color-scheme.scss
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_container.scss
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_deprecate.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_forms.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_gradients.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_grid.scss
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_image.scss
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_list-group.scss
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_lists.scss
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_pagination.scss
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_reset-text.scss
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_resize.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_table-variants.scss
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_text-truncate.scss
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_transition.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_utilities.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_visually-hidden.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:00:59.617407 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/utilities/_api.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:00:59.617407 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/vendor/
--rw-r--r--   0 runner    (1001) docker     (127)    10029 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/vendor/_rfs.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:00:59.617407 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/cards/
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/cards/card-background.scss
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/cards/card-carousel.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:00:59.617407 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/custom/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/custom/_styles.scss
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/custom/_variables.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:00:59.617407 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/forms/
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/forms/_form-check.scss
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/forms/_form-select.scss
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/forms/_form-switch.scss
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/forms/_forms.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/forms/_input-group.scss
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/forms/_inputs.scss
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/forms/_labels.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:00:59.617407 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/mixins/_badge.scss
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/mixins/_colored-shadows.scss
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/mixins/_hover.scss
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/mixins/_social-buttons.scss
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/mixins/mixins.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:00:59.573407 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:00:59.621407 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/
--rw-r--r--   0 runner    (1001) docker     (127)    20327 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_flatpickr.scss
--rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_nouislider.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_perfect-scrollbar.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_prism.scss
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/plugins.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/theme.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:00:59.625407 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/variables/
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/variables/_animations.scss
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/variables/_avatars.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/variables/_badge.scss
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/variables/_breadcrumb.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/variables/_cards-extend.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/variables/_cards.scss
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/variables/_choices.scss
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/variables/_dark-version.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/variables/_dropdowns.scss
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/variables/_fixed-plugin.scss
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/variables/_form-switch.scss
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/variables/_full-calendar.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/variables/_header.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/variables/_info-areas.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/variables/_misc-extend.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/variables/_misc.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/variables/_navbar-vertical.scss
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/variables/_navbar.scss
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/variables/_pagination.scss
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/variables/_rtl.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/variables/_social-buttons.scss
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/variables/_table.scss
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/variables/_timeline.scss
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/variables/_utilities-extend.scss
--rw-r--r--   0 runner    (1001) docker     (127)     6884 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/variables/_utilities.scss
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/variables/_virtual-reality.scss
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard.scss
--rw-r--r--   0 runner    (1001) docker     (127)     7749 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/tasks_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:00:59.625407 Red-Web-Dashboard-1.0.0/reddash/app/templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/templates/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:00:59.625407 Red-Web-Dashboard-1.0.0/reddash/app/templates/errors/
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/templates/errors/403.html
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/templates/errors/404.html
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/templates/errors/500.html
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/templates/errors/blacklisted.html
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/templates/errors/custom.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:00:59.625407 Red-Web-Dashboard-1.0.0/reddash/app/templates/includes/
--rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/templates/includes/fixed-plugin.html
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/templates/includes/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/templates/includes/navigation.html
--rw-r--r--   0 runner    (1001) docker     (127)    11700 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/templates/includes/scripts.html
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/templates/includes/sidenav.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:00:59.625407 Red-Web-Dashboard-1.0.0/reddash/app/templates/layouts/
--rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/templates/layouts/base-fullscreen.html
--rw-r--r--   0 runner    (1001) docker     (127)     5425 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/templates/layouts/base.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:00:59.629408 Red-Web-Dashboard-1.0.0/reddash/app/templates/pages/
--rw-r--r--   0 runner    (1001) docker     (127)    28559 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/templates/pages/admin.html
--rw-r--r--   0 runner    (1001) docker     (127)    16891 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/templates/pages/commands.html
--rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/templates/pages/credits.html
--rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/templates/pages/dashboard.html
--rw-r--r--   0 runner    (1001) docker     (127)    16289 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/templates/pages/dashboard_guild.html
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/templates/pages/guild_profile.html
--rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/templates/pages/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:00:59.629408 Red-Web-Dashboard-1.0.0/reddash/app/templates/pages/login/
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/templates/pages/login/login.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:00:59.629408 Red-Web-Dashboard-1.0.0/reddash/app/templates/pages/third_parties/
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/templates/pages/third_parties/oauth.html
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/templates/pages/third_parties/third_parties.html
--rw-r--r--   0 runner    (1001) docker     (127)     6389 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/templates/pages/third_parties/third_parties_list.html
--rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/templates/pages/third_parties/third_party.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:00:59.629408 Red-Web-Dashboard-1.0.0/reddash/app/third_parties/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/third_parties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8796 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/third_parties/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)    27177 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/reddash/app/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-12 16:00:59.633407 Red-Web-Dashboard-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-12 16:00:55.000000 Red-Web-Dashboard-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.853525 red_web_dashboard-1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    34625 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-04-12 18:11:14.853525 red_web_dashboard-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.849525 red_web_dashboard-1.1/Red_Web_Dashboard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-04-12 18:11:14.000000 red_web_dashboard-1.1/Red_Web_Dashboard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15750 2024-04-12 18:11:14.000000 red_web_dashboard-1.1/Red_Web_Dashboard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 18:11:14.000000 red_web_dashboard-1.1/Red_Web_Dashboard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-12 18:11:14.000000 red_web_dashboard-1.1/Red_Web_Dashboard.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-12 18:11:14.000000 red_web_dashboard-1.1/Red_Web_Dashboard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-12 18:11:14.000000 red_web_dashboard-1.1/Red_Web_Dashboard.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.797523 red_web_dashboard-1.1/reddash/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.797523 red_web_dashboard-1.1/reddash/app/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6267 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.797523 red_web_dashboard-1.1/reddash/app/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35780 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/base/routes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.797523 red_web_dashboard-1.1/reddash/app/login/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/login/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7456 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/login/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/pagination.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.789523 red_web_dashboard-1.1/reddash/app/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.805523 red_web_dashboard-1.1/reddash/app/static/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/biometric-icon.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.809523 red_web_dashboard-1.1/reddash/app/static/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (127)   480516 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/css/argon-dashboard.css
+-rw-r--r--   0 runner    (1001) docker     (127)  1218638 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/css/argon-dashboard.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   381006 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/css/argon-dashboard.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/css/nucleo-icons.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/css/nucleo-svg.css
+-rw-r--r--   0 runner    (1001) docker     (127)    10929 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/css/simplemde.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   635325 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/error-403.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   884014 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/error-404.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   824431 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/error-500.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.809523 red_web_dashboard-1.1/reddash/app/static/assets/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)    18516 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/fonts/nucleo-icons.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   126098 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/fonts/nucleo-icons.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    18292 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/fonts/nucleo-icons.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    10220 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/fonts/nucleo-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     8580 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/fonts/nucleo-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    26524 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/fonts/nucleo.eot
+-rw-r--r--   0 runner    (1001) docker     (127)    26364 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/fonts/nucleo.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    15168 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/fonts/nucleo.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12616 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/fonts/nucleo.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/gulpfile.js
+-rw-r--r--   0 runner    (1001) docker     (127)    34128 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/icon-documentation.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.809523 red_web_dashboard-1.1/reddash/app/static/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    27282 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/js/argon-dashboard.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15415 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/js/argon-dashboard.js.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.813524 red_web_dashboard-1.1/reddash/app/static/assets/js/core/
+-rw-r--r--   0 runner    (1001) docker     (127)    48944 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/js/core/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   288580 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/js/core/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    19188 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/js/core/popper.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.813524 red_web_dashboard-1.1/reddash/app/static/assets/js/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/js/plugins/Chart.extension.js
+-rw-r--r--   0 runner    (1001) docker     (127)    47524 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/js/plugins/Simple-Full-featured-jQuery-Pagination-System-Pagination-js.zip
+-rw-r--r--   0 runner    (1001) docker     (127)    15614 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/js/plugins/bootstrap-notify.js
+-rw-r--r--   0 runner    (1001) docker     (127)   176853 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/js/plugins/chartjs.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    19411 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/js/plugins/perfect-scrollbar.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    48421 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/js/plugins/smooth-scrollbar.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7738 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/js/plugins/utils.js
+-rw-r--r--   0 runner    (1001) docker     (127)   140628 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/oauth.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/pdf.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/random.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.813524 red_web_dashboard-1.1/reddash/app/static/assets/scss/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.821524 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_alert.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_avatars.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_badge.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_breadcrumbs.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_buttons.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_cards.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_dark-version.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     6683 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_dropdown.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_dropup.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_fixed-plugin.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_footer.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_forms.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_gradients.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_header.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_info-areas.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     7009 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_misc.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_nav.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    13929 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_navbar-vertical.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_navbar.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_pagination.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_popovers.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_progress.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_rtl.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_social-buttons.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_tables.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_tilt.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_timeline.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_tooltips.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_typography.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_utilities-extend.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    16957 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_utilities.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    68466 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_variables.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.829524 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_accordion.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_alert.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_badge.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_breadcrumb.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_button-group.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_buttons.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_card.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_carousel.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_close.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_containers.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     8014 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_dropdown.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_forms.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    10558 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_functions.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_grid.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_helpers.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_images.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     6348 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_list-group.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_maps.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_mixins.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     7762 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_modal.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_nav.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     8723 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_navbar.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_offcanvas.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_pagination.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_placeholders.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_popover.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_progress.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_reboot.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_root.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_spinners.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_tables.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_toasts.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_tooltip.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_transitions.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_type.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    14817 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_utilities.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    68547 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_variables.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap-grid.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap-reboot.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap-utilities.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.829524 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_floating-labels.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-check.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-control.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-range.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-select.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-text.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_input-group.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_labels.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_validation.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.829524 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_clearfix.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_color-bg.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_colored-links.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_position.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_ratio.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_stacks.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_stretched-link.scss
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_text-truncation.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_visually-hidden.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_vr.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.837525 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_alert.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_backdrop.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_border-radius.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_box-shadow.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_breakpoints.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_buttons.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_caret.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_clearfix.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_color-scheme.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_container.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_deprecate.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_forms.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_gradients.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_grid.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_image.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_list-group.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_lists.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_pagination.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_reset-text.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_resize.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_table-variants.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_text-truncate.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_transition.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_utilities.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_visually-hidden.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.837525 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/utilities/_api.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.837525 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)    10029 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/vendor/_rfs.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.837525 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/cards/
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/cards/card-background.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/cards/card-carousel.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.837525 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/custom/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/custom/_styles.scss
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/custom/_variables.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.837525 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/forms/_form-check.scss
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/forms/_form-select.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/forms/_form-switch.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/forms/_forms.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/forms/_input-group.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/forms/_inputs.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/forms/_labels.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.837525 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/mixins/_badge.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/mixins/_colored-shadows.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/mixins/_hover.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/mixins/_social-buttons.scss
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/mixins/mixins.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.793523 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.841524 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/plugins/free/
+-rw-r--r--   0 runner    (1001) docker     (127)    20327 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_flatpickr.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_nouislider.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_perfect-scrollbar.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_prism.scss
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/plugins/free/plugins.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/theme.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.845525 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_animations.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_avatars.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_badge.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_breadcrumb.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_cards-extend.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_cards.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_choices.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_dark-version.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_dropdowns.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_fixed-plugin.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_form-switch.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_full-calendar.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_header.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_info-areas.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_misc-extend.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_misc.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_navbar-vertical.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_navbar.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_pagination.scss
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_rtl.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_social-buttons.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_table.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_timeline.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_utilities-extend.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     6884 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_utilities.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_virtual-reality.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     7749 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/tasks_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.845525 red_web_dashboard-1.1/reddash/app/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/templates/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.845525 red_web_dashboard-1.1/reddash/app/templates/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/templates/errors/403.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/templates/errors/404.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/templates/errors/500.html
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/templates/errors/blacklisted.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/templates/errors/custom.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.845525 red_web_dashboard-1.1/reddash/app/templates/includes/
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/templates/includes/fixed-plugin.html
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/templates/includes/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/templates/includes/navigation.html
+-rw-r--r--   0 runner    (1001) docker     (127)    11700 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/templates/includes/scripts.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/templates/includes/sidenav.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.845525 red_web_dashboard-1.1/reddash/app/templates/layouts/
+-rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/templates/layouts/base-fullscreen.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5425 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/templates/layouts/base.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.849525 red_web_dashboard-1.1/reddash/app/templates/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)    28559 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/templates/pages/admin.html
+-rw-r--r--   0 runner    (1001) docker     (127)    16891 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/templates/pages/commands.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/templates/pages/credits.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/templates/pages/dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (127)    16262 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/templates/pages/dashboard_guild.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/templates/pages/guild_profile.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/templates/pages/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.849525 red_web_dashboard-1.1/reddash/app/templates/pages/login/
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/templates/pages/login/login.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.849525 red_web_dashboard-1.1/reddash/app/templates/pages/third_parties/
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/templates/pages/third_parties/oauth.html
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/templates/pages/third_parties/third_parties.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/templates/pages/third_parties/third_parties_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/templates/pages/third_parties/third_party.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.849525 red_web_dashboard-1.1/reddash/app/third_parties/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/third_parties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8892 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/third_parties/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27177 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-12 18:11:14.853525 red_web_dashboard-1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/setup.py
```

### Comparing `Red-Web-Dashboard-1.0.0/LICENSE` & `red_web_dashboard-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/PKG-INFO` & `red_web_dashboard-1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: Red-Web-Dashboard
-Version: 1.0.0
+Version: 1.1.0
 Summary: An easy-to-use interactive web dashboard to control your Red bot!
-Home-page: https://github.com/Red-Dashboard/Red-Dashboard
+Home-page: https://github.com/AAA3A-AAA3A/Red-Dashboard
 Author: Neuro Assassin & AAA3A
 License: AGPL-3.0
 Project-URL: Third Party Discord Server, https://discord.gg/red-cog-support-240154543684321280
-Project-URL: Documentation, https://red-dashboard-aaa3a.readthedocs.io/en/latest/
+Project-URL: Documentation, https://red-web-dashboard.readthedocs.io/en/latest/
 Project-URL: Donate on Buy Me a Coffee, https://www.buymeacoffee.com/aaa3a
 Project-URL: Source Code, https://github.com/AAA3A-AAA3A/Red-Dashboard
 Project-URL: Red Source Code, https://github.com/Cog-Creators/Red-DiscordBot
 Project-URL: Red Discord Server, https://discord.gg/red
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: Developers
@@ -54,31 +54,31 @@
 Requires-Dist: sphinx-rtd-theme==1.0.0; extra == "docs"
 Requires-Dist: sphinx-prompt==1.5.0; extra == "docs"
 
 # Red-Dashboard (Fork of Neuro's Dashboard)
 An easy-to-use interactive web dashboard to control your Red-DiscordBot instance! Thank you very much to Neuro for the initial work!
 
 ## Overview
-This project is an easy-to-use interactive web dashboard to control your Red-DiscordBot instance, allowing for easier customization of settings and more interactive plugins to develop and get your bot ready for production. Using Discord Open Authentication, users will log into the dashboard using their Discord account, ensuring that all users are only allowed to customize and view settings that they are explicitly given permission to control, providing a safe and secure experience for all users.
+This project is an easy-to-use interactive web dashboard to control your Red-DiscordBot instance, allowing for easier customization of settings and more interactive plugins to develop and get your bot ready for production. Using Discord Open Authentication, users will log into the Dashboard using their Discord account, ensuring that all users are only allowed to customize and view settings that they are explicitly given permission to control, providing a safe and secure experience for all users.
 
 ## Installation
-To get started on setting up your Dashboard for your Red bot, please follow the installation instructions that can be found [here] (sorry, documentation not finished).
+To get started on setting up your Dashboard for your Red bot, please follow the installation instructions that can be found [here](https://red-web-dashboard.readthedocs.io/en/latest).
 
-This project is supported on Windows, Mac OS X and Linux distributions, however is recommended on Linux distributions for security reasons.  Support is not given for setting up your domain for your dashboard other than any guides given for such, and contributors to the source code are not responsible for any security issues that arise as a result of not securely setting up the software.
+This project is supported on Windows, Mac OS X and Linux distributions, however is recommended on Linux distributions for security reasons. Support is not given for setting up your domain for your Dashboard other than any guides given for such, and contributors to the source code are not responsible for any security issues that arise as a result of not securely setting up the software.
 
 ## Support
 If you wish to use this program and receive support for it, you must also give feedback and report any bugs you encounter. You can ask in the #support_aaa3a-cogs channel in the [cogs support server](https://discord.gg/GET4DVk).
 
 ## Legal
 Red-Dashboard for Red-DiscordBot is released under [Affero General Public License v3](https://github.com/AAA3A-AAA3A/Red-Dashboard/blob/main/LICENSE).
 
 For details about how this project manages your privacy, please review the following documents. By using this program, you acknowledge that you have read these documents and consent to having your data used in the ways described in such documents.
-- [Cookie Policy](https://github.com/Cog-Creators/Red-Dashboard/blob/master/documents/Cookie%20Policy.md)
-- [Privacy Policy](https://github.com/Cog-Creators/Red-Dashboard/blob/master/documents/Privacy%20Policy.md)
-- [Third Party Disclaimer](https://github.com/Cog-Creators/Red-Dashboard/blob/master/documents/Third%20Party%20Disclaimer.md)
+- [Cookie Policy](https://github.com/AAA3A-AAA3A/Red-Dashboard/blob/main/documents/Cookie%20Policy.md)
+- [Privacy Policy](https://github.com/AAA3A-AAA3A/Red-Dashboard/blob/main/documents/Privacy%20Policy.md)
+- [Third Parties Disclaimer](https://github.com/AAA3A-AAA3A/Red-Dashboard/blob/main/documents/Third%20Parties%20Disclaimer.md)
 
 ## Credits
 I would like to thank the following, for all the contributions they have made that helped this become what it is today.
 * Neuro Assassin, for its great initial work!
 * TrustyJAID for its OAuth basic integration for third parties.
 * Cog Creators, for making such an amazing bot.
 * All the people who tested the Dashboard, and gave feedback.
```

### Comparing `Red-Web-Dashboard-1.0.0/README.md` & `red_web_dashboard-1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # Red-Dashboard (Fork of Neuro's Dashboard)
 An easy-to-use interactive web dashboard to control your Red-DiscordBot instance! Thank you very much to Neuro for the initial work!
 
 ## Overview
-This project is an easy-to-use interactive web dashboard to control your Red-DiscordBot instance, allowing for easier customization of settings and more interactive plugins to develop and get your bot ready for production. Using Discord Open Authentication, users will log into the dashboard using their Discord account, ensuring that all users are only allowed to customize and view settings that they are explicitly given permission to control, providing a safe and secure experience for all users.
+This project is an easy-to-use interactive web dashboard to control your Red-DiscordBot instance, allowing for easier customization of settings and more interactive plugins to develop and get your bot ready for production. Using Discord Open Authentication, users will log into the Dashboard using their Discord account, ensuring that all users are only allowed to customize and view settings that they are explicitly given permission to control, providing a safe and secure experience for all users.
 
 ## Installation
-To get started on setting up your Dashboard for your Red bot, please follow the installation instructions that can be found [here] (sorry, documentation not finished).
+To get started on setting up your Dashboard for your Red bot, please follow the installation instructions that can be found [here](https://red-web-dashboard.readthedocs.io/en/latest).
 
-This project is supported on Windows, Mac OS X and Linux distributions, however is recommended on Linux distributions for security reasons.  Support is not given for setting up your domain for your dashboard other than any guides given for such, and contributors to the source code are not responsible for any security issues that arise as a result of not securely setting up the software.
+This project is supported on Windows, Mac OS X and Linux distributions, however is recommended on Linux distributions for security reasons. Support is not given for setting up your domain for your Dashboard other than any guides given for such, and contributors to the source code are not responsible for any security issues that arise as a result of not securely setting up the software.
 
 ## Support
 If you wish to use this program and receive support for it, you must also give feedback and report any bugs you encounter. You can ask in the #support_aaa3a-cogs channel in the [cogs support server](https://discord.gg/GET4DVk).
 
 ## Legal
 Red-Dashboard for Red-DiscordBot is released under [Affero General Public License v3](https://github.com/AAA3A-AAA3A/Red-Dashboard/blob/main/LICENSE).
 
 For details about how this project manages your privacy, please review the following documents. By using this program, you acknowledge that you have read these documents and consent to having your data used in the ways described in such documents.
-- [Cookie Policy](https://github.com/Cog-Creators/Red-Dashboard/blob/master/documents/Cookie%20Policy.md)
-- [Privacy Policy](https://github.com/Cog-Creators/Red-Dashboard/blob/master/documents/Privacy%20Policy.md)
-- [Third Party Disclaimer](https://github.com/Cog-Creators/Red-Dashboard/blob/master/documents/Third%20Party%20Disclaimer.md)
+- [Cookie Policy](https://github.com/AAA3A-AAA3A/Red-Dashboard/blob/main/documents/Cookie%20Policy.md)
+- [Privacy Policy](https://github.com/AAA3A-AAA3A/Red-Dashboard/blob/main/documents/Privacy%20Policy.md)
+- [Third Parties Disclaimer](https://github.com/AAA3A-AAA3A/Red-Dashboard/blob/main/documents/Third%20Parties%20Disclaimer.md)
 
 ## Credits
 I would like to thank the following, for all the contributions they have made that helped this become what it is today.
 * Neuro Assassin, for its great initial work!
 * TrustyJAID for its OAuth basic integration for third parties.
 * Cog Creators, for making such an amazing bot.
 * All the people who tested the Dashboard, and gave feedback.
```

### Comparing `Red-Web-Dashboard-1.0.0/Red_Web_Dashboard.egg-info/PKG-INFO` & `red_web_dashboard-1.1/Red_Web_Dashboard.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: Red-Web-Dashboard
-Version: 1.0.0
+Version: 1.1.0
 Summary: An easy-to-use interactive web dashboard to control your Red bot!
-Home-page: https://github.com/Red-Dashboard/Red-Dashboard
+Home-page: https://github.com/AAA3A-AAA3A/Red-Dashboard
 Author: Neuro Assassin & AAA3A
 License: AGPL-3.0
 Project-URL: Third Party Discord Server, https://discord.gg/red-cog-support-240154543684321280
-Project-URL: Documentation, https://red-dashboard-aaa3a.readthedocs.io/en/latest/
+Project-URL: Documentation, https://red-web-dashboard.readthedocs.io/en/latest/
 Project-URL: Donate on Buy Me a Coffee, https://www.buymeacoffee.com/aaa3a
 Project-URL: Source Code, https://github.com/AAA3A-AAA3A/Red-Dashboard
 Project-URL: Red Source Code, https://github.com/Cog-Creators/Red-DiscordBot
 Project-URL: Red Discord Server, https://discord.gg/red
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: Developers
@@ -54,31 +54,31 @@
 Requires-Dist: sphinx-rtd-theme==1.0.0; extra == "docs"
 Requires-Dist: sphinx-prompt==1.5.0; extra == "docs"
 
 # Red-Dashboard (Fork of Neuro's Dashboard)
 An easy-to-use interactive web dashboard to control your Red-DiscordBot instance! Thank you very much to Neuro for the initial work!
 
 ## Overview
-This project is an easy-to-use interactive web dashboard to control your Red-DiscordBot instance, allowing for easier customization of settings and more interactive plugins to develop and get your bot ready for production. Using Discord Open Authentication, users will log into the dashboard using their Discord account, ensuring that all users are only allowed to customize and view settings that they are explicitly given permission to control, providing a safe and secure experience for all users.
+This project is an easy-to-use interactive web dashboard to control your Red-DiscordBot instance, allowing for easier customization of settings and more interactive plugins to develop and get your bot ready for production. Using Discord Open Authentication, users will log into the Dashboard using their Discord account, ensuring that all users are only allowed to customize and view settings that they are explicitly given permission to control, providing a safe and secure experience for all users.
 
 ## Installation
-To get started on setting up your Dashboard for your Red bot, please follow the installation instructions that can be found [here] (sorry, documentation not finished).
+To get started on setting up your Dashboard for your Red bot, please follow the installation instructions that can be found [here](https://red-web-dashboard.readthedocs.io/en/latest).
 
-This project is supported on Windows, Mac OS X and Linux distributions, however is recommended on Linux distributions for security reasons.  Support is not given for setting up your domain for your dashboard other than any guides given for such, and contributors to the source code are not responsible for any security issues that arise as a result of not securely setting up the software.
+This project is supported on Windows, Mac OS X and Linux distributions, however is recommended on Linux distributions for security reasons. Support is not given for setting up your domain for your Dashboard other than any guides given for such, and contributors to the source code are not responsible for any security issues that arise as a result of not securely setting up the software.
 
 ## Support
 If you wish to use this program and receive support for it, you must also give feedback and report any bugs you encounter. You can ask in the #support_aaa3a-cogs channel in the [cogs support server](https://discord.gg/GET4DVk).
 
 ## Legal
 Red-Dashboard for Red-DiscordBot is released under [Affero General Public License v3](https://github.com/AAA3A-AAA3A/Red-Dashboard/blob/main/LICENSE).
 
 For details about how this project manages your privacy, please review the following documents. By using this program, you acknowledge that you have read these documents and consent to having your data used in the ways described in such documents.
-- [Cookie Policy](https://github.com/Cog-Creators/Red-Dashboard/blob/master/documents/Cookie%20Policy.md)
-- [Privacy Policy](https://github.com/Cog-Creators/Red-Dashboard/blob/master/documents/Privacy%20Policy.md)
-- [Third Party Disclaimer](https://github.com/Cog-Creators/Red-Dashboard/blob/master/documents/Third%20Party%20Disclaimer.md)
+- [Cookie Policy](https://github.com/AAA3A-AAA3A/Red-Dashboard/blob/main/documents/Cookie%20Policy.md)
+- [Privacy Policy](https://github.com/AAA3A-AAA3A/Red-Dashboard/blob/main/documents/Privacy%20Policy.md)
+- [Third Parties Disclaimer](https://github.com/AAA3A-AAA3A/Red-Dashboard/blob/main/documents/Third%20Parties%20Disclaimer.md)
 
 ## Credits
 I would like to thank the following, for all the contributions they have made that helped this become what it is today.
 * Neuro Assassin, for its great initial work!
 * TrustyJAID for its OAuth basic integration for third parties.
 * Cog Creators, for making such an amazing bot.
 * All the people who tested the Dashboard, and gave feedback.
```

### Comparing `Red-Web-Dashboard-1.0.0/Red_Web_Dashboard.egg-info/SOURCES.txt` & `red_web_dashboard-1.1/Red_Web_Dashboard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/pyproject.toml` & `red_web_dashboard-1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/__main__.py` & `red_web_dashboard-1.1/reddash/__main__.py`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/app.py` & `red_web_dashboard-1.1/reddash/app/app.py`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/base/routes.py` & `red_web_dashboard-1.1/reddash/app/base/routes.py`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/login/routes.py` & `red_web_dashboard-1.1/reddash/app/login/routes.py`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/pagination.py` & `red_web_dashboard-1.1/reddash/app/pagination.py`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/biometric-icon.svg` & `red_web_dashboard-1.1/reddash/app/static/assets/biometric-icon.svg`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/css/argon-dashboard.css` & `red_web_dashboard-1.1/reddash/app/static/assets/css/argon-dashboard.css`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/css/argon-dashboard.css.map` & `red_web_dashboard-1.1/reddash/app/static/assets/css/argon-dashboard.css.map`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/css/argon-dashboard.min.css` & `red_web_dashboard-1.1/reddash/app/static/assets/css/argon-dashboard.min.css`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/css/nucleo-icons.css` & `red_web_dashboard-1.1/reddash/app/static/assets/css/nucleo-icons.css`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/css/nucleo-svg.css` & `red_web_dashboard-1.1/reddash/app/static/assets/css/nucleo-svg.css`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/css/simplemde.min.css` & `red_web_dashboard-1.1/reddash/app/static/assets/css/simplemde.min.css`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/error-403.gif` & `red_web_dashboard-1.1/reddash/app/static/assets/error-403.gif`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/error-404.gif` & `red_web_dashboard-1.1/reddash/app/static/assets/error-404.gif`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/error-500.gif` & `red_web_dashboard-1.1/reddash/app/static/assets/error-500.gif`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/fonts/nucleo-icons.eot` & `red_web_dashboard-1.1/reddash/app/static/assets/fonts/nucleo-icons.eot`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/fonts/nucleo-icons.svg` & `red_web_dashboard-1.1/reddash/app/static/assets/fonts/nucleo-icons.svg`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/fonts/nucleo-icons.ttf` & `red_web_dashboard-1.1/reddash/app/static/assets/fonts/nucleo-icons.ttf`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/fonts/nucleo-icons.woff` & `red_web_dashboard-1.1/reddash/app/static/assets/fonts/nucleo-icons.woff`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/fonts/nucleo-icons.woff2` & `red_web_dashboard-1.1/reddash/app/static/assets/fonts/nucleo-icons.woff2`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/fonts/nucleo.eot` & `red_web_dashboard-1.1/reddash/app/static/assets/fonts/nucleo.eot`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/fonts/nucleo.ttf` & `red_web_dashboard-1.1/reddash/app/static/assets/fonts/nucleo.ttf`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/fonts/nucleo.woff` & `red_web_dashboard-1.1/reddash/app/static/assets/fonts/nucleo.woff`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/fonts/nucleo.woff2` & `red_web_dashboard-1.1/reddash/app/static/assets/fonts/nucleo.woff2`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/gulpfile.js` & `red_web_dashboard-1.1/reddash/app/static/assets/gulpfile.js`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/icon-documentation.svg` & `red_web_dashboard-1.1/reddash/app/static/assets/icon-documentation.svg`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/js/argon-dashboard.js` & `red_web_dashboard-1.1/reddash/app/static/assets/js/argon-dashboard.js`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/js/argon-dashboard.js.map` & `red_web_dashboard-1.1/reddash/app/static/assets/js/argon-dashboard.js.map`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/js/core/bootstrap.min.js` & `red_web_dashboard-1.1/reddash/app/static/assets/js/core/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/js/core/jquery.min.js` & `red_web_dashboard-1.1/reddash/app/static/assets/js/core/jquery.min.js`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/js/core/popper.min.js` & `red_web_dashboard-1.1/reddash/app/static/assets/js/core/popper.min.js`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/js/plugins/Chart.extension.js` & `red_web_dashboard-1.1/reddash/app/static/assets/js/plugins/Chart.extension.js`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/js/plugins/Simple-Full-featured-jQuery-Pagination-System-Pagination-js.zip` & `red_web_dashboard-1.1/reddash/app/static/assets/js/plugins/Simple-Full-featured-jQuery-Pagination-System-Pagination-js.zip`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/js/plugins/bootstrap-notify.js` & `red_web_dashboard-1.1/reddash/app/static/assets/js/plugins/bootstrap-notify.js`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/js/plugins/chartjs.min.js` & `red_web_dashboard-1.1/reddash/app/static/assets/js/plugins/chartjs.min.js`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/js/plugins/perfect-scrollbar.min.js` & `red_web_dashboard-1.1/reddash/app/static/assets/js/plugins/perfect-scrollbar.min.js`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/js/plugins/smooth-scrollbar.min.js` & `red_web_dashboard-1.1/reddash/app/static/assets/js/plugins/smooth-scrollbar.min.js`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/js/plugins/utils.js` & `red_web_dashboard-1.1/reddash/app/static/assets/js/plugins/utils.js`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/oauth.png` & `red_web_dashboard-1.1/reddash/app/static/assets/oauth.png`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/pdf.svg` & `red_web_dashboard-1.1/reddash/app/static/assets/pdf.svg`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/random.svg` & `red_web_dashboard-1.1/reddash/app/static/assets/random.svg`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_avatars.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_avatars.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_breadcrumbs.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_breadcrumbs.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_buttons.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_buttons.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_cards.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_cards.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_dark-version.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_dark-version.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_dropdown.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_dropdown.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_dropup.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_dropup.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_fixed-plugin.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_fixed-plugin.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_forms.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_forms.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_gradients.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_gradients.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_header.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_header.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_info-areas.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_info-areas.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_misc.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_misc.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_nav.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_nav.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_navbar-vertical.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_navbar-vertical.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_navbar.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_navbar.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_pagination.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_pagination.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_rtl.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_rtl.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_social-buttons.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_social-buttons.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_tables.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_tables.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_timeline.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_timeline.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_typography.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_typography.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_utilities.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_utilities.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/_variables.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_variables.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_accordion.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_accordion.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_alert.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_alert.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_badge.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_badge.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_breadcrumb.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_breadcrumb.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_button-group.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_button-group.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_buttons.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_buttons.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_card.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_card.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_carousel.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_carousel.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_close.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_close.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_containers.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_containers.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_dropdown.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_dropdown.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_functions.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_functions.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_grid.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_grid.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_images.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_images.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_list-group.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_list-group.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_maps.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_maps.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_mixins.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_mixins.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_modal.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_modal.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_nav.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_nav.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_navbar.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_navbar.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_offcanvas.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_offcanvas.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_pagination.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_pagination.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_placeholders.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_placeholders.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_popover.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_popover.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_progress.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_progress.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_reboot.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_reboot.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_root.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_root.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_spinners.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_spinners.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_tables.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_tables.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_toasts.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_toasts.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_tooltip.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_tooltip.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_type.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_type.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_utilities.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_utilities.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_variables.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_variables.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap-grid.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap-grid.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_floating-labels.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_floating-labels.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-check.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-check.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-control.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-control.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-range.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-range.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-select.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-select.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_input-group.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_input-group.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_labels.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_labels.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_position.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_position.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_border-radius.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_border-radius.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_breakpoints.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_breakpoints.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_buttons.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_buttons.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_caret.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_caret.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_deprecate.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_deprecate.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_forms.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_forms.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_gradients.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_gradients.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_grid.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_grid.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_table-variants.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_table-variants.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_transition.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_transition.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_utilities.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_utilities.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_visually-hidden.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_visually-hidden.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/utilities/_api.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/utilities/_api.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/vendor/_rfs.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/vendor/_rfs.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/cards/card-background.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/cards/card-background.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/forms/_form-check.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/forms/_form-check.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/forms/_form-switch.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/forms/_form-switch.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/forms/_input-group.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/forms/_input-group.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/mixins/_social-buttons.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/mixins/_social-buttons.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_flatpickr.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_flatpickr.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_nouislider.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_nouislider.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_perfect-scrollbar.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_perfect-scrollbar.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_prism.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_prism.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/theme.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/theme.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/variables/_animations.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_animations.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/variables/_avatars.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_avatars.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/variables/_badge.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_badge.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/variables/_cards-extend.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_cards-extend.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/variables/_cards.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_cards.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/variables/_dark-version.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_dark-version.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/variables/_dropdowns.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_dropdowns.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/variables/_header.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_header.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/variables/_info-areas.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_info-areas.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/variables/_misc-extend.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_misc-extend.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/variables/_misc.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_misc.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/variables/_navbar-vertical.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_navbar-vertical.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/variables/_navbar.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_navbar.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/variables/_pagination.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_pagination.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/variables/_social-buttons.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_social-buttons.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/variables/_table.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_table.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/variables/_timeline.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_timeline.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/variables/_utilities-extend.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_utilities-extend.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard/variables/_utilities.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_utilities.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/static/assets/scss/argon-dashboard.scss` & `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard.scss`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/tasks_manager.py` & `red_web_dashboard-1.1/reddash/app/tasks_manager.py`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/templates/errors/403.html` & `red_web_dashboard-1.1/reddash/app/templates/errors/403.html`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/templates/errors/404.html` & `red_web_dashboard-1.1/reddash/app/templates/errors/404.html`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/templates/errors/500.html` & `red_web_dashboard-1.1/reddash/app/templates/errors/500.html`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/templates/errors/blacklisted.html` & `red_web_dashboard-1.1/reddash/app/templates/errors/blacklisted.html`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/templates/errors/custom.html` & `red_web_dashboard-1.1/reddash/app/templates/errors/custom.html`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/templates/includes/fixed-plugin.html` & `red_web_dashboard-1.1/reddash/app/templates/includes/fixed-plugin.html`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/templates/includes/footer.html` & `red_web_dashboard-1.1/reddash/app/templates/includes/footer.html`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/templates/includes/navigation.html` & `red_web_dashboard-1.1/reddash/app/templates/includes/navigation.html`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/templates/includes/scripts.html` & `red_web_dashboard-1.1/reddash/app/templates/includes/scripts.html`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/templates/includes/sidenav.html` & `red_web_dashboard-1.1/reddash/app/templates/includes/sidenav.html`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/templates/layouts/base-fullscreen.html` & `red_web_dashboard-1.1/reddash/app/templates/layouts/base-fullscreen.html`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/templates/layouts/base.html` & `red_web_dashboard-1.1/reddash/app/templates/layouts/base.html`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/templates/pages/admin.html` & `red_web_dashboard-1.1/reddash/app/templates/pages/admin.html`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/templates/pages/commands.html` & `red_web_dashboard-1.1/reddash/app/templates/pages/commands.html`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/templates/pages/credits.html` & `red_web_dashboard-1.1/reddash/app/templates/pages/credits.html`

 * *Files 12% similar despite different names*

```diff
@@ -24,21 +24,21 @@
                     {{ _('An important part of internal Python RPC logic was coded by <a href="https://github.com/NeuroAssassin">Neuro Assassin#4779</a>, licensed under <a href="https://github.com/Cog-Creators/Red-Dashboard/blob/master/LICENSE">Affero General Public License v3.0</a>.')|safe }}<br />
                     {{ _('This Dashboard was made for <a href="https://github.com/Cog-Creators/Red-DiscordBot">Red Discord Bot</a>, a multifunctional, fully modular Discord bot, created by Twentysix, made great by many. Red Discord Bot is licensed under <a href="https://github.com/Cog-Creators/Red-DiscordBot/blob/V3/develop/LICENSE">GNU General Public License v3.0</a>.')|safe }}
                   </p>
                   <br />
                   <h6 class="card-category text-gray">{{ _('Policies and Disclaimers') }}</h6>
                   <ul>
                     <li>
-                      {{ _("Privacy Policy:") }} <a href="https://github.com/AAA3A-AAA3A/Red-Dashboard/blob/master/documents/Privacy%20Policy.md">https://github.com/Cog-Creators/Red-Dashboard/blob/master/documents/Privacy%20Policy.md</a>
+                      {{ _("Privacy Policy:") }} <a href="https://github.com/AAA3A-AAA3A/Red-Dashboard/blob/main/documents/Privacy%20Policy.md">https://github.com/AAA3A-AAA3A/Red-Dashboard/blob/main/documents/Privacy%20Policy.md</a>
                     </li>
                     <li>
-                      {{ _("Cookie Policy:") }} <a href="https://github.com/AAA3A-AAA3A/Red-Dashboard/blob/master/documents/Cookie%20Policy.md">https://github.com/Cog-Creators/Red-Dashboard/blob/master/documents/Cookie%20Policy.md</a>
+                      {{ _("Cookie Policy:") }} <a href="https://github.com/AAA3A-AAA3A/Red-Dashboard/blob/main/documents/Cookie%20Policy.md">https://github.com/AAA3A-AAA3A/Red-Dashboard/blob/main/documents/Cookie%20Policy.md</a>
                     </li>
                     <li>
-                      {{ _("Third Parties Disclaimer:") }} <a href="https://github.com/AAA3A-AAA3A/Red-Dashboard/blob/master/documents/Third%20Parties%20Disclaimer.md">https://github.com/Cog-Creators/Red-Dashboard/blob/master/documents/Third%20Party%20Disclaimer.md</a>
+                      {{ _("Third Parties Disclaimer:") }} <a href="https://github.com/AAA3A-AAA3A/Red-Dashboard/blob/main/documents/Third%20Parties%20Disclaimer.md">https://github.com/AAA3A-AAA3A/Red-Dashboard/blob/main/documents/Third%20Parties%20Disclaimer.md</a>
                     </li>
                   </ul>
                   <sup>{{ _("The above policies and disclaimers only apply on unmodified distributions of Red-Dashboard. Copyright holder makes no guarantee that the documents are accurate on public distributions of Red-Dashboard.") }}</sup>
                 </div>                
               </div>
             </div>
           </div>
```

#### html2text {}

```diff
@@ -9,17 +9,17 @@
 {{ _('An important part of internal Python RPC logic was coded by _N_e_u_r_o
 _A_s_s_a_s_s_i_n_#_4_7_7_9, licensed under _A_f_f_e_r_o_ _G_e_n_e_r_a_l_ _P_u_b_l_i_c_ _L_i_c_e_n_s_e_ _v_3_._0.')|safe }}
 {{ _('This Dashboard was made for _R_e_d_ _D_i_s_c_o_r_d_ _B_o_t, a multifunctional, fully
 modular Discord bot, created by Twentysix, made great by many. Red Discord Bot
 is licensed under _G_N_U_ _G_e_n_e_r_a_l_ _P_u_b_l_i_c_ _L_i_c_e_n_s_e_ _v_3_._0.')|safe }}
 
 ** {{{{ __((''PPoolliicciieess aanndd DDiissccllaaiimmeerrss'')) }}}} **
-    * {{ _("Privacy Policy:") }} _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_C_o_g_-_C_r_e_a_t_o_r_s_/_R_e_d_-_D_a_s_h_b_o_a_r_d_/
-      _b_l_o_b_/_m_a_s_t_e_r_/_d_o_c_u_m_e_n_t_s_/_P_r_i_v_a_c_y_%_2_0_P_o_l_i_c_y_._m_d
-    * {{ _("Cookie Policy:") }} _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_C_o_g_-_C_r_e_a_t_o_r_s_/_R_e_d_-_D_a_s_h_b_o_a_r_d_/
-      _b_l_o_b_/_m_a_s_t_e_r_/_d_o_c_u_m_e_n_t_s_/_C_o_o_k_i_e_%_2_0_P_o_l_i_c_y_._m_d
-    * {{ _("Third Parties Disclaimer:") }} _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_C_o_g_-_C_r_e_a_t_o_r_s_/_R_e_d_-
-      _D_a_s_h_b_o_a_r_d_/_b_l_o_b_/_m_a_s_t_e_r_/_d_o_c_u_m_e_n_t_s_/_T_h_i_r_d_%_2_0_P_a_r_t_y_%_2_0_D_i_s_c_l_a_i_m_e_r_._m_d
+    * {{ _("Privacy Policy:") }} _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_A_A_A_3_A_-_A_A_A_3_A_/_R_e_d_-_D_a_s_h_b_o_a_r_d_/
+      _b_l_o_b_/_m_a_i_n_/_d_o_c_u_m_e_n_t_s_/_P_r_i_v_a_c_y_%_2_0_P_o_l_i_c_y_._m_d
+    * {{ _("Cookie Policy:") }} _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_A_A_A_3_A_-_A_A_A_3_A_/_R_e_d_-_D_a_s_h_b_o_a_r_d_/
+      _b_l_o_b_/_m_a_i_n_/_d_o_c_u_m_e_n_t_s_/_C_o_o_k_i_e_%_2_0_P_o_l_i_c_y_._m_d
+    * {{ _("Third Parties Disclaimer:") }} _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_A_A_A_3_A_-_A_A_A_3_A_/_R_e_d_-
+      _D_a_s_h_b_o_a_r_d_/_b_l_o_b_/_m_a_i_n_/_d_o_c_u_m_e_n_t_s_/_T_h_i_r_d_%_2_0_P_a_r_t_i_e_s_%_2_0_D_i_s_c_l_a_i_m_e_r_._m_d
 {{ _("The above policies and disclaimers only apply on unmodified distributions
 of Red-Dashboard. Copyright holder makes no guarantee that the documents are
 accurate on public distributions of Red-Dashboard.") }}
 {% endblock %} {% block javascripts %} {% endblock %}
```

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/templates/pages/dashboard.html` & `red_web_dashboard-1.1/reddash/app/templates/pages/dashboard.html`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/templates/pages/dashboard_guild.html` & `red_web_dashboard-1.1/reddash/app/templates/pages/dashboard_guild.html`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 {% block content %}
   <main class="main-content position-relative border-radius-lg">
     <div class="container-fluid">
         <div class="row">
             {% include "pages/guild_profile.html" %}
 
-            <div id="guild-content" class="col-md-8 mt-4" style="margin-left: 10px;">
+            <div id="guild-content" class="col-md-8 mt-4">
                 <ul class="nav nav-pills position-relative end-0" role="tablist">
                     <li class="nav-item">
                         <a class="nav-link {% if not page or page == "overview" %}show active{% endif %}" id="overview-tab" data-toggle="pill" href="#overview" role="tab" aria-controls="overview" aria-selected="true">
                             <i class="fa fa-map opacity-10" style="vertical-align: -1px;"></i> {{ _("Overview") }}
                         </a>
                     </li>
                     <li class="nav-item">
```

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/templates/pages/guild_profile.html` & `red_web_dashboard-1.1/reddash/app/templates/pages/guild_profile.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<div id="profile" class="card card-body col-md-3 mt-4 align-items-center">
+<div id="profile" class="card card-body col-md-3 mt-4 align-items-center" style="margin-right: 10px;">
     <div {% if False %}class="row"{% endif %}>
         <br />
         <div class="col-sm-auto col-4 text-center">
             <div class="avatar avatar-xl"><img src="{{ guild.icon_url }}" class="shadow-sm border-radius-lg" style="height: 170%; width: 170%;" /></div>
         </div>
         <div class="col-sm-auto col-8 my-auto">
             <div class="h-100">
```

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/templates/pages/index.html` & `red_web_dashboard-1.1/reddash/app/templates/pages/index.html`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/templates/pages/login/login.html` & `red_web_dashboard-1.1/reddash/app/templates/pages/login/login.html`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/templates/pages/third_parties/oauth.html` & `red_web_dashboard-1.1/reddash/app/templates/pages/third_parties/oauth.html`

 * *Files 9% similar despite different names*

```diff
@@ -20,15 +20,15 @@
                     <p>{{ _("Successfully forwarded your account informations. You may now close this tab and go back to Discord.") }}</p>
                     <img src="{{ config.ASSETS_ROOT }}/oauth.png" height="250" />
                     <br /><br />
                     <a class="btn bg-gradient-success mb-1 w-30" href="{{ url_for("base_blueprint.index") }}">{{ _("Back to Home") }}</a>
                   </div>
                 </div>
                 <div class="card-footer">
-                  {{ _('This is a Third Party integration. By using this application, you acknowledge that you have read the Third Party disclaimer found <a href="{link}">here</a>').format(link="https://github.com/Cog-Creators/Red-Dashboard/blob/master/documents/Third%20Party%20Disclaimer.md") }}
+                  {{ _('This is a Third Party integration. By using this application, you acknowledge that you have read the Third Party disclaimer found <a href="{link}">here</a>').format(link="https://github.com/AAA3A-AAA3A/Red-Dashboard/blob/main/documents/Third%20Parties%20Disclaimer.md") }}
                 </div>
               </div>
             </div>
           </div>
         </div>
       </div>
     </div>
```

#### html2text {}

```diff
@@ -4,10 +4,10 @@
 {{ _("Successfully forwarded your account informations. You may now close this
 tab and go back to Discord.") }}
 [{{ config.ASSETS_ROOT }}/oauth.png]
 
 }">{{ _("Back to Home") }}
 {{ _('This is a Third Party integration. By using this application, you
 acknowledge that you have read the Third Party disclaimer found _h_e_r_e').format
-(link="https://github.com/Cog-Creators/Red-Dashboard/blob/master/documents/
-Third%20Party%20Disclaimer.md") }}
+(link="https://github.com/AAA3A-AAA3A/Red-Dashboard/blob/main/documents/
+Third%20Parties%20Disclaimer.md") }}
 {% endblock %} {% block javascripts %}{% endblock %}
```

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/templates/pages/third_parties/third_parties_list.html` & `red_web_dashboard-1.1/reddash/app/templates/pages/third_parties/third_parties_list.html`

 * *Files 2% similar despite different names*

```diff
@@ -367,34 +367,38 @@
 000016e0: 2829 207b 0a20 2020 2020 2020 2020 2020  () {.           
 000016f0: 2063 6861 6e67 6550 6167 6528 227b 7b20   changePage("{{ 
 00001700: 7461 625f 6e61 6d65 207d 7d22 293b 0a20  tab_name }}");. 
 00001710: 2020 2020 2020 207d 293b 0a20 2020 207b         });.    {
 00001720: 2520 656e 6469 6620 257d 0a20 203c 2f73  % endif %}.  </s
 00001730: 6372 6970 743e 0a20 203c 7363 7269 7074  cript>.  <script
 00001740: 3e0a 2020 2020 646f 6375 6d65 6e74 2e71  >.    document.q
-00001750: 7565 7279 5365 6c65 6374 6f72 2827 2374  uerySelector('#t
-00001760: 6869 7264 2d70 6172 7469 6573 2d74 6162  hird-parties-tab
-00001770: 7320 615b 6461 7461 2d74 6f67 676c 653d  s a[data-toggle=
-00001780: 2270 696c 6c22 5d27 292e 6164 6445 7665  "pill"]').addEve
-00001790: 6e74 4c69 7374 656e 6572 2822 7368 6f77  ntListener("show
-000017a0: 6e2e 6273 2e74 6162 222c 2066 756e 6374  n.bs.tab", funct
-000017b0: 696f 6e28 6529 207b 0a20 2020 2020 2020  ion(e) {.       
-000017c0: 2076 6172 2074 6172 6765 745f 6964 203d   var target_id =
-000017d0: 2065 2e74 6172 6765 742e 6964 2e73 6c69   e.target.id.sli
-000017e0: 6365 2830 2c20 2d34 293b 0a20 2020 2020  ce(0, -4);.     
-000017f0: 2020 2076 6172 206e 6577 5f75 726c 203d     var new_url =
-00001800: 2022 2f74 6869 7264 2d70 6172 7469 6573   "/third-parties
-00001810: 2f22 202b 2074 6172 6765 745f 6964 3b0a  /" + target_id;.
-00001820: 2020 2020 2020 2020 6966 2028 2128 7769          if (!(wi
-00001830: 6e64 6f77 2e6c 6f63 6174 696f 6e2e 7061  ndow.location.pa
-00001840: 7468 6e61 6d65 2e73 7461 7274 7357 6974  thname.startsWit
-00001850: 6828 6e65 775f 7572 6c29 2929 207b 0a20  h(new_url))) {. 
-00001860: 2020 2020 2020 2020 2020 202f 2f20 7769             // wi
-00001870: 6e64 6f77 2e6c 6f63 6174 696f 6e2e 7061  ndow.location.pa
-00001880: 7468 6e61 6d65 203d 206e 6577 5f75 726c  thname = new_url
-00001890: 3b0a 2020 2020 2020 2020 2020 2020 7769  ;.            wi
-000018a0: 6e64 6f77 2e68 6973 746f 7279 2e70 7573  ndow.history.pus
-000018b0: 6853 7461 7465 287b 7d2c 2022 222c 206e  hState({}, "", n
-000018c0: 6577 5f75 726c 293b 0a20 2020 2020 2020  ew_url);.       
-000018d0: 207d 0a20 2020 207d 290a 2020 3c2f 7363   }.    }).  </sc
-000018e0: 7269 7074 3e0a 7b25 2065 6e64 626c 6f63  ript>.{% endbloc
-000018f0: 6b20 257d 0a                             k %}.
+00001750: 7565 7279 5365 6c65 6374 6f72 416c 6c28  uerySelectorAll(
+00001760: 2723 7468 6972 642d 7061 7274 6965 732d  '#third-parties-
+00001770: 7461 6273 2061 5b64 6174 612d 746f 6767  tabs a[data-togg
+00001780: 6c65 3d22 7069 6c6c 225d 2729 2e66 6f72  le="pill"]').for
+00001790: 4561 6368 2866 756e 6374 696f 6e28 656c  Each(function(el
+000017a0: 656d 656e 7429 207b 0a20 2020 2020 2065  ement) {.      e
+000017b0: 6c65 6d65 6e74 2e61 6464 4576 656e 744c  lement.addEventL
+000017c0: 6973 7465 6e65 7228 2273 686f 776e 2e62  istener("shown.b
+000017d0: 732e 7461 6222 2c20 6675 6e63 7469 6f6e  s.tab", function
+000017e0: 2865 2920 7b0a 2020 2020 2020 2020 2020  (e) {.          
+000017f0: 7661 7220 7461 7267 6574 5f69 6420 3d20  var target_id = 
+00001800: 652e 7461 7267 6574 2e69 642e 736c 6963  e.target.id.slic
+00001810: 6528 302c 202d 3429 3b0a 2020 2020 2020  e(0, -4);.      
+00001820: 2020 2020 7661 7220 6e65 775f 7572 6c20      var new_url 
+00001830: 3d20 222f 7468 6972 642d 7061 7274 6965  = "/third-partie
+00001840: 732f 2220 2b20 7461 7267 6574 5f69 643b  s/" + target_id;
+00001850: 0a20 2020 2020 2020 2020 2069 6620 2821  .          if (!
+00001860: 2877 696e 646f 772e 6c6f 6361 7469 6f6e  (window.location
+00001870: 2e70 6174 686e 616d 652e 7374 6172 7473  .pathname.starts
+00001880: 5769 7468 286e 6577 5f75 726c 2929 2920  With(new_url))) 
+00001890: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+000018a0: 2f2f 2077 696e 646f 772e 6c6f 6361 7469  // window.locati
+000018b0: 6f6e 2e70 6174 686e 616d 6520 3d20 6e65  on.pathname = ne
+000018c0: 775f 7572 6c3b 0a20 2020 2020 2020 2020  w_url;.         
+000018d0: 2020 2020 2077 696e 646f 772e 6869 7374       window.hist
+000018e0: 6f72 792e 7075 7368 5374 6174 6528 7b7d  ory.pushState({}
+000018f0: 2c20 2222 2c20 6e65 775f 7572 6c29 3b0a  , "", new_url);.
+00001900: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+00001910: 2020 7d29 3b0a 2020 2020 7d29 3b0a 2020    });.    });.  
+00001920: 3c2f 7363 7269 7074 3e0a 7b25 2065 6e64  </script>.{% end
+00001930: 626c 6f63 6b20 257d 0a                   block %}.
```

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/third_parties/routes.py` & `red_web_dashboard-1.1/reddash/app/third_parties/routes.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,16 +212,18 @@
                     name=name, page=page, **return_guild, **result["web_content"]
                 )
             return render_template(
                 "pages/third_parties/third_party.html",
                 name=name,
                 page=page,
                 **return_guild,
+                fullscreen=result["web_content"].get("fullscreen", False),
                 source_content=render_template_string(
-                    result["web_content"].pop("source"), **result["web_content"]
+                    result["web_content"].pop("source"),
+                    **result["web_content"],
                 ),
             )
         elif "error_code" in result:
             return abort(result["error_code"], description=result.get("error_message"))
         elif "error_title" in result:
             return render_template(
                 "errors/custom.html",
```

### Comparing `Red-Web-Dashboard-1.0.0/reddash/app/utils.py` & `red_web_dashboard-1.1/reddash/app/utils.py`

 * *Files identical despite different names*

### Comparing `Red-Web-Dashboard-1.0.0/setup.cfg` & `red_web_dashboard-1.1/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 name = Red-Web-Dashboard
 version = attr: reddash.__version__
 description = An easy-to-use interactive web dashboard to control your Red bot!
 license = AGPL-3.0
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8; variant=GFM
 author = Neuro Assassin & AAA3A
-url = https://github.com/Red-Dashboard/Red-Dashboard
+url = https://github.com/AAA3A-AAA3A/Red-Dashboard
 project_urls = 
 	Third Party Discord Server = https://discord.gg/red-cog-support-240154543684321280
-	Documentation = https://red-dashboard-aaa3a.readthedocs.io/en/latest/
+	Documentation = https://red-web-dashboard.readthedocs.io/en/latest/
 	Donate on Buy Me a Coffee = https://www.buymeacoffee.com/aaa3a
 	Source Code = https://github.com/AAA3A-AAA3A/Red-Dashboard
 	Red Source Code = https://github.com/Cog-Creators/Red-DiscordBot
 	Red Discord Server = https://discord.gg/red
 classifiers = 
 	Development Status :: 3 - Alpha
 	Framework :: Flask
```

