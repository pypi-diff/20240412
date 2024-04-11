# Comparing `tmp/betty-0.3.2.tar.gz` & `tmp/betty-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betty-0.3.2.tar", last modified: Thu Mar 28 00:13:32 2024, max compression
+gzip compressed data, was "betty-0.3.3.tar", last modified: Thu Apr 11 22:30:12 2024, max compression
```

## Comparing `betty-0.3.2.tar` & `betty-0.3.3.tar`

### file list

```diff
@@ -1,295 +1,300 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.839191 betty-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)    32453 2024-03-28 00:12:25.000000 betty-0.3.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    42623 2024-03-28 00:13:32.839191 betty-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-03-28 00:12:25.000000 betty-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.803191 betty-0.3.2/betty/
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-03-28 00:12:25.000000 betty-0.3.2/betty/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.787191 betty-0.3.2/betty/_package/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.803191 betty-0.3.2/betty/_package/pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-03-28 00:12:25.000000 betty-0.3.2/betty/_package/pyinstaller/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.803191 betty-0.3.2/betty/_package/pyinstaller/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-28 00:12:25.000000 betty-0.3.2/betty/_package/pyinstaller/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-28 00:12:25.000000 betty-0.3.2/betty/_package/pyinstaller/hooks/hook-betty.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-03-28 00:12:25.000000 betty-0.3.2/betty/_package/pyinstaller/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-03-28 00:12:25.000000 betty-0.3.2/betty/_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-03-28 00:12:25.000000 betty-0.3.2/betty/_resizeimage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-03-28 00:12:25.000000 betty-0.3.2/betty/about.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.803191 betty-0.3.2/betty/app/
--rw-r--r--   0 runner    (1001) docker     (127)    15063 2024-03-28 00:12:25.000000 betty-0.3.2/betty/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.807191 betty-0.3.2/betty/app/extension/
--rw-r--r--   0 runner    (1001) docker     (127)    12813 2024-03-28 00:12:25.000000 betty-0.3.2/betty/app/extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-03-28 00:12:25.000000 betty-0.3.2/betty/app/extension/requirement.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.807191 betty-0.3.2/betty/assets/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-28 00:12:39.000000 betty-0.3.2/betty/assets/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)    21116 2024-03-28 00:12:25.000000 betty-0.3.2/betty/assets/betty.pot
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.787191 betty-0.3.2/betty/assets/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.807191 betty-0.3.2/betty/assets/locale/de-DE/
--rw-r--r--   0 runner    (1001) docker     (127)    36322 2024-03-28 00:12:25.000000 betty-0.3.2/betty/assets/locale/de-DE/betty.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.807191 betty-0.3.2/betty/assets/locale/fr-FR/
--rw-r--r--   0 runner    (1001) docker     (127)    25573 2024-03-28 00:12:25.000000 betty-0.3.2/betty/assets/locale/fr-FR/betty.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.807191 betty-0.3.2/betty/assets/locale/nl-NL/
--rw-r--r--   0 runner    (1001) docker     (127)    36157 2024-03-28 00:12:25.000000 betty-0.3.2/betty/assets/locale/nl-NL/betty.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.807191 betty-0.3.2/betty/assets/locale/uk/
--rw-r--r--   0 runner    (1001) docker     (127)    25598 2024-03-28 00:12:25.000000 betty-0.3.2/betty/assets/locale/uk/betty.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.791191 betty-0.3.2/betty/assets/public/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.807191 betty-0.3.2/betty/assets/public/localized/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-03-28 00:12:25.000000 betty-0.3.2/betty/assets/public/localized/index.html.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.807191 betty-0.3.2/betty/assets/public/static/
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-03-28 00:12:25.000000 betty-0.3.2/betty/assets/public/static/betty-16x16.png
--rw-r--r--   0 runner    (1001) docker     (127)     8229 2024-03-28 00:12:25.000000 betty-0.3.2/betty/assets/public/static/betty-192x192.png
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-03-28 00:12:25.000000 betty-0.3.2/betty/assets/public/static/betty-32x32.png
--rw-r--r--   0 runner    (1001) docker     (127)    19708 2024-03-28 00:12:25.000000 betty-0.3.2/betty/assets/public/static/betty-512x512.png
--rw-r--r--   0 runner    (1001) docker     (127)   152126 2024-03-28 00:12:25.000000 betty-0.3.2/betty/assets/public/static/betty.ico
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-03-28 00:12:25.000000 betty-0.3.2/betty/assets/public/static/index.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-28 00:12:25.000000 betty-0.3.2/betty/assets/public/static/robots.txt.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.807191 betty-0.3.2/betty/assets/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-03-28 00:12:25.000000 betty-0.3.2/betty/assets/templates/base.html.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.807191 betty-0.3.2/betty/assets/templates/entity/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-03-28 00:12:25.000000 betty-0.3.2/betty/assets/templates/entity/page-list.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-03-28 00:12:25.000000 betty-0.3.2/betty/assets/templates/entity/page.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-03-28 00:12:25.000000 betty-0.3.2/betty/assets/templates/head.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-03-28 00:12:25.000000 betty-0.3.2/betty/assets/templates/linked-data.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-28 00:12:25.000000 betty-0.3.2/betty/assets/templates/sitemap-index.xml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-03-28 00:12:25.000000 betty-0.3.2/betty/assets/templates/sitemap.xml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-03-28 00:12:25.000000 betty-0.3.2/betty/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-03-28 00:12:25.000000 betty-0.3.2/betty/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-03-28 00:12:25.000000 betty-0.3.2/betty/classtools.py
--rw-r--r--   0 runner    (1001) docker     (127)     9941 2024-03-28 00:12:25.000000 betty-0.3.2/betty/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-03-28 00:12:25.000000 betty-0.3.2/betty/concurrent.py
--rw-r--r--   0 runner    (1001) docker     (127)    22487 2024-03-28 00:12:25.000000 betty-0.3.2/betty/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    10802 2024-03-28 00:12:25.000000 betty-0.3.2/betty/deriver.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-03-28 00:12:25.000000 betty-0.3.2/betty/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-03-28 00:12:25.000000 betty-0.3.2/betty/documentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-03-28 00:12:25.000000 betty-0.3.2/betty/error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.811191 betty-0.3.2/betty/extension/
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.811191 betty-0.3.2/betty/extension/cotton_candy/
--rw-r--r--   0 runner    (1001) docker     (127)    14934 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.791191 betty-0.3.2/betty/extension/cotton_candy/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.791191 betty-0.3.2/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.815191 betty-0.3.2/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/accessibility.scss
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/citation.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/entity.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/file.js
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/file.scss
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/main.js
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/main.scss
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/meta.scss
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/overlay.scss
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/package.json
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/page.scss
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/permalink.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/person.scss
--rw-r--r--   0 runner    (1001) docker     (127)     6321 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/search.js
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/search.scss
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/show.js
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/show.scss
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/text.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/variables.scss.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/webpack.config.js
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/webpack.config.json.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.791191 betty-0.3.2/betty/extension/cotton_candy/assets/public/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.815191 betty-0.3.2/betty/extension/cotton_candy/assets/public/localized/
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/public/localized/index.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/public/localized/search-index.json.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.815191 betty-0.3.2/betty/extension/cotton_candy/assets/public/static/
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/public/static/betty.webmanifest
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/public/static/search-configuration.json.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.815191 betty-0.3.2/betty/extension/cotton_candy/assets/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     6717 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/templates/base.html.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.823191 betty-0.3.2/betty/extension/cotton_candy/assets/templates/entity/
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/templates/entity/featured--place.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/templates/entity/featured.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/templates/entity/label--citation.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/templates/entity/label--event.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/templates/entity/label--person-name.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/templates/entity/label--person.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/templates/entity/label--place.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/templates/entity/label--source.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/templates/entity/label.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/templates/entity/list--event.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/templates/entity/list--file.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/templates/entity/list--person.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/templates/entity/list--place.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/templates/entity/meta--citation.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/templates/entity/meta--event.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/templates/entity/meta--file.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/templates/entity/meta--person.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/templates/entity/meta--place.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/templates/entity/meta--source.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/templates/entity/page--citation.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/templates/entity/page--event.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/templates/entity/page--file.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)    12475 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/templates/entity/page--person.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/templates/entity/page--place.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/templates/entity/page--source.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/templates/entity/page-list--event.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/templates/entity/page-list--file.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/templates/entity/page-list--person.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/templates/entity/page-list--place.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/templates/entity/page-list--source.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/templates/event-dimensions.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/templates/file-extended--application--pdf.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/templates/file-extended--image.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/templates/file-extended.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/templates/file-summary--application--pdf.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/templates/file-summary--image.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/templates/file-summary.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/templates/file.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/templates/footer.html.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.823191 betty-0.3.2/betty/extension/cotton_candy/assets/templates/macro/
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/templates/macro/citation.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/templates/media.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/templates/permalink.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/templates/references.html.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.823191 betty-0.3.2/betty/extension/cotton_candy/assets/templates/search/
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/templates/search/result-file.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/templates/search/result-person.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/templates/search/result-place.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/templates/search/result-with-image.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/templates/search/result.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/templates/search/results.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/templates/section-notes.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/templates/show-countable.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/templates/show.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/assets/templates/timeline.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/cotton_candy/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.823191 betty-0.3.2/betty/extension/demo/
--rw-r--r--   0 runner    (1001) docker     (127)    15653 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/demo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.823191 betty-0.3.2/betty/extension/deriver/
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/deriver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.823191 betty-0.3.2/betty/extension/gramps/
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/gramps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/gramps/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6348 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/gramps/gui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.823191 betty-0.3.2/betty/extension/http_api_doc/
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/http_api_doc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.791191 betty-0.3.2/betty/extension/http_api_doc/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.791191 betty-0.3.2/betty/extension/http_api_doc/assets/betty.extension.npm._Npm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.823191 betty-0.3.2/betty/extension/http_api_doc/assets/betty.extension.npm._Npm/src/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/http_api_doc/assets/betty.extension.npm._Npm/src/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.791191 betty-0.3.2/betty/extension/http_api_doc/assets/public/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.791191 betty-0.3.2/betty/extension/http_api_doc/assets/public/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.823191 betty-0.3.2/betty/extension/http_api_doc/assets/public/static/api/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/http_api_doc/assets/public/static/api/index.html.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.823191 betty-0.3.2/betty/extension/maps/
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/maps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.791191 betty-0.3.2/betty/extension/maps/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.791191 betty-0.3.2/betty/extension/maps/assets/betty.extension.npm._Npm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.827191 betty-0.3.2/betty/extension/maps/assets/betty.extension.npm._Npm/src/
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/maps/assets/betty.extension.npm._Npm/src/maps.css
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/maps/assets/betty.extension.npm._Npm/src/maps.js
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/maps/assets/betty.extension.npm._Npm/src/package.json
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/maps/assets/betty.extension.npm._Npm/src/webpack.config.js
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/maps/assets/betty.extension.npm._Npm/src/webpack.config.json.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.827191 betty-0.3.2/betty/extension/nginx/
--rw-r--r--   0 runner    (1001) docker     (127)     7658 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/nginx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/nginx/artifact.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.827191 betty-0.3.2/betty/extension/nginx/assets/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/nginx/assets/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/nginx/assets/content_negotiation.lua
--rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/nginx/assets/nginx.conf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/nginx/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/nginx/serve.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.827191 betty-0.3.2/betty/extension/npm/
--rw-r--r--   0 runner    (1001) docker     (127)     8924 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/npm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.827191 betty-0.3.2/betty/extension/privatizer/
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/privatizer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.827191 betty-0.3.2/betty/extension/trees/
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/trees/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.795191 betty-0.3.2/betty/extension/trees/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.795191 betty-0.3.2/betty/extension/trees/assets/betty.extension.npm._Npm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.827191 betty-0.3.2/betty/extension/trees/assets/betty.extension.npm._Npm/src/
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/trees/assets/betty.extension.npm._Npm/src/package.json
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/trees/assets/betty.extension.npm._Npm/src/trees.css
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/trees/assets/betty.extension.npm._Npm/src/trees.js
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/trees/assets/betty.extension.npm._Npm/src/webpack.config.js
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/trees/assets/betty.extension.npm._Npm/src/webpack.config.json.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.795191 betty-0.3.2/betty/extension/trees/assets/public/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.827191 betty-0.3.2/betty/extension/trees/assets/public/localized/
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/trees/assets/public/localized/people.json.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.827191 betty-0.3.2/betty/extension/wikipedia/
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/wikipedia/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.795191 betty-0.3.2/betty/extension/wikipedia/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.827191 betty-0.3.2/betty/extension/wikipedia/assets/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-03-28 00:12:25.000000 betty-0.3.2/betty/extension/wikipedia/assets/templates/wikipedia.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-03-28 00:12:25.000000 betty-0.3.2/betty/fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-03-28 00:12:25.000000 betty-0.3.2/betty/functools.py
--rw-r--r--   0 runner    (1001) docker     (127)    13505 2024-03-28 00:12:25.000000 betty-0.3.2/betty/generate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.831191 betty-0.3.2/betty/gramps/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-28 00:12:25.000000 betty-0.3.2/betty/gramps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-28 00:12:25.000000 betty-0.3.2/betty/gramps/error.py
--rw-r--r--   0 runner    (1001) docker     (127)    31084 2024-03-28 00:12:25.000000 betty-0.3.2/betty/gramps/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.831191 betty-0.3.2/betty/gui/
--rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-03-28 00:12:25.000000 betty-0.3.2/betty/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12620 2024-03-28 00:12:25.000000 betty-0.3.2/betty/gui/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-03-28 00:12:25.000000 betty-0.3.2/betty/gui/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-03-28 00:12:25.000000 betty-0.3.2/betty/gui/locale.py
--rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-03-28 00:12:25.000000 betty-0.3.2/betty/gui/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-03-28 00:12:25.000000 betty-0.3.2/betty/gui/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    31377 2024-03-28 00:12:25.000000 betty-0.3.2/betty/gui/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-03-28 00:12:25.000000 betty-0.3.2/betty/gui/serve.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-03-28 00:12:25.000000 betty-0.3.2/betty/gui/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-03-28 00:12:25.000000 betty-0.3.2/betty/gui/window.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-03-28 00:12:25.000000 betty-0.3.2/betty/html.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-03-28 00:12:25.000000 betty-0.3.2/betty/importlib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.831191 betty-0.3.2/betty/jinja2/
--rw-r--r--   0 runner    (1001) docker     (127)    10099 2024-03-28 00:12:25.000000 betty-0.3.2/betty/jinja2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14880 2024-03-28 00:12:25.000000 betty-0.3.2/betty/jinja2/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-03-28 00:12:25.000000 betty-0.3.2/betty/jinja2/test.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-03-28 00:12:25.000000 betty-0.3.2/betty/job.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.831191 betty-0.3.2/betty/json/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-28 00:12:25.000000 betty-0.3.2/betty/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-03-28 00:12:25.000000 betty-0.3.2/betty/json/linked_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4512 2024-03-28 00:12:25.000000 betty-0.3.2/betty/json/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-03-28 00:12:25.000000 betty-0.3.2/betty/load.py
--rw-r--r--   0 runner    (1001) docker     (127)    36927 2024-03-28 00:12:25.000000 betty-0.3.2/betty/locale.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-03-28 00:12:25.000000 betty-0.3.2/betty/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-03-28 00:12:25.000000 betty-0.3.2/betty/media_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.831191 betty-0.3.2/betty/model/
--rw-r--r--   0 runner    (1001) docker     (127)    35221 2024-03-28 00:12:25.000000 betty-0.3.2/betty/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    56373 2024-03-28 00:12:25.000000 betty-0.3.2/betty/model/ancestry.py
--rw-r--r--   0 runner    (1001) docker     (127)     7118 2024-03-28 00:12:25.000000 betty-0.3.2/betty/model/event_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-03-28 00:12:25.000000 betty-0.3.2/betty/openapi.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-03-28 00:12:25.000000 betty-0.3.2/betty/os.py
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-03-28 00:12:25.000000 betty-0.3.2/betty/path.py
--rw-r--r--   0 runner    (1001) docker     (127)    10139 2024-03-28 00:12:25.000000 betty-0.3.2/betty/privatizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    28975 2024-03-28 00:12:25.000000 betty-0.3.2/betty/project.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 00:12:25.000000 betty-0.3.2/betty/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-03-28 00:12:25.000000 betty-0.3.2/betty/render.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.835191 betty-0.3.2/betty/serde/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-28 00:12:25.000000 betty-0.3.2/betty/serde/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-03-28 00:12:25.000000 betty-0.3.2/betty/serde/dump.py
--rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-03-28 00:12:25.000000 betty-0.3.2/betty/serde/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-03-28 00:12:25.000000 betty-0.3.2/betty/serde/format.py
--rw-r--r--   0 runner    (1001) docker     (127)    15310 2024-03-28 00:12:25.000000 betty-0.3.2/betty/serde/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     7603 2024-03-28 00:12:25.000000 betty-0.3.2/betty/serve.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.835191 betty-0.3.2/betty/sphinx/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-28 00:12:25.000000 betty-0.3.2/betty/sphinx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.835191 betty-0.3.2/betty/sphinx/extension/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-28 00:12:25.000000 betty-0.3.2/betty/sphinx/extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-03-28 00:12:25.000000 betty-0.3.2/betty/sphinx/extension/replacements.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-03-28 00:12:25.000000 betty-0.3.2/betty/string.py
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-03-28 00:12:25.000000 betty-0.3.2/betty/subprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-03-28 00:12:25.000000 betty-0.3.2/betty/url.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-03-28 00:12:25.000000 betty-0.3.2/betty/warnings.py
--rw-r--r--   0 runner    (1001) docker     (127)    16214 2024-03-28 00:12:25.000000 betty-0.3.2/betty/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.835191 betty-0.3.2/betty.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    42623 2024-03-28 00:13:32.000000 betty-0.3.2/betty.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10279 2024-03-28 00:13:32.000000 betty-0.3.2/betty.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 00:13:32.000000 betty-0.3.2/betty.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-03-28 00:13:32.000000 betty-0.3.2/betty.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-03-28 00:13:32.000000 betty-0.3.2/betty.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-28 00:13:32.000000 betty-0.3.2/betty.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.835191 betty-0.3.2/documentation/
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-03-28 00:12:25.000000 betty-0.3.2/documentation/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.795191 betty-0.3.2/node_modules/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.795191 betty-0.3.2/node_modules/flatted/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:13:32.835191 betty-0.3.2/node_modules/flatted/python/
--rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-03-28 00:13:21.000000 betty-0.3.2/node_modules/flatted/python/flatted.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-03-28 00:13:21.000000 betty-0.3.2/node_modules/flatted/python/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-03-28 00:12:25.000000 betty-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 00:13:32.839191 betty-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-28 00:12:25.000000 betty-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.238239 betty-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    32453 2024-04-11 22:29:12.000000 betty-0.3.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    43400 2024-04-11 22:30:12.238239 betty-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-11 22:29:12.000000 betty-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.202239 betty-0.3.3/betty/
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-11 22:29:12.000000 betty-0.3.3/betty/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.186239 betty-0.3.3/betty/_package/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.202239 betty-0.3.3/betty/_package/pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-04-11 22:29:12.000000 betty-0.3.3/betty/_package/pyinstaller/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.202239 betty-0.3.3/betty/_package/pyinstaller/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-11 22:29:12.000000 betty-0.3.3/betty/_package/pyinstaller/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-11 22:29:12.000000 betty-0.3.3/betty/_package/pyinstaller/hooks/hook-betty.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-11 22:29:12.000000 betty-0.3.3/betty/_package/pyinstaller/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-11 22:29:12.000000 betty-0.3.3/betty/_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-11 22:29:12.000000 betty-0.3.3/betty/_resizeimage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-11 22:29:12.000000 betty-0.3.3/betty/about.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.202239 betty-0.3.3/betty/app/
+-rw-r--r--   0 runner    (1001) docker     (127)    18342 2024-04-11 22:29:12.000000 betty-0.3.3/betty/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.202239 betty-0.3.3/betty/app/extension/
+-rw-r--r--   0 runner    (1001) docker     (127)    12813 2024-04-11 22:29:12.000000 betty-0.3.3/betty/app/extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-04-11 22:29:12.000000 betty-0.3.3/betty/app/extension/requirement.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.202239 betty-0.3.3/betty/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-11 22:29:21.000000 betty-0.3.3/betty/assets/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)    21162 2024-04-11 22:29:12.000000 betty-0.3.3/betty/assets/betty.pot
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.186239 betty-0.3.3/betty/assets/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.202239 betty-0.3.3/betty/assets/locale/de-DE/
+-rw-r--r--   0 runner    (1001) docker     (127)    36368 2024-04-11 22:29:12.000000 betty-0.3.3/betty/assets/locale/de-DE/betty.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.202239 betty-0.3.3/betty/assets/locale/fr-FR/
+-rw-r--r--   0 runner    (1001) docker     (127)    25619 2024-04-11 22:29:12.000000 betty-0.3.3/betty/assets/locale/fr-FR/betty.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.206239 betty-0.3.3/betty/assets/locale/nl-NL/
+-rw-r--r--   0 runner    (1001) docker     (127)    36229 2024-04-11 22:29:12.000000 betty-0.3.3/betty/assets/locale/nl-NL/betty.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.206239 betty-0.3.3/betty/assets/locale/uk/
+-rw-r--r--   0 runner    (1001) docker     (127)    25644 2024-04-11 22:29:12.000000 betty-0.3.3/betty/assets/locale/uk/betty.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.186239 betty-0.3.3/betty/assets/public/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.206239 betty-0.3.3/betty/assets/public/localized/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-11 22:29:12.000000 betty-0.3.3/betty/assets/public/localized/index.html.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.206239 betty-0.3.3/betty/assets/public/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-11 22:29:12.000000 betty-0.3.3/betty/assets/public/static/betty-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8229 2024-04-11 22:29:12.000000 betty-0.3.3/betty/assets/public/static/betty-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-11 22:29:12.000000 betty-0.3.3/betty/assets/public/static/betty-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19708 2024-04-11 22:29:12.000000 betty-0.3.3/betty/assets/public/static/betty-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (127)   152126 2024-04-11 22:29:12.000000 betty-0.3.3/betty/assets/public/static/betty.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-11 22:29:12.000000 betty-0.3.3/betty/assets/public/static/index.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-11 22:29:12.000000 betty-0.3.3/betty/assets/public/static/robots.txt.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.206239 betty-0.3.3/betty/assets/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-11 22:29:12.000000 betty-0.3.3/betty/assets/templates/base.html.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.206239 betty-0.3.3/betty/assets/templates/entity/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-11 22:29:12.000000 betty-0.3.3/betty/assets/templates/entity/page-list.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-11 22:29:12.000000 betty-0.3.3/betty/assets/templates/entity/page.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-04-11 22:29:12.000000 betty-0.3.3/betty/assets/templates/head.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-11 22:29:12.000000 betty-0.3.3/betty/assets/templates/linked-data.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-11 22:29:12.000000 betty-0.3.3/betty/assets/templates/sitemap-index.xml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-11 22:29:12.000000 betty-0.3.3/betty/assets/templates/sitemap.xml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-11 22:29:12.000000 betty-0.3.3/betty/asyncio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.206239 betty-0.3.3/betty/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)     3326 2024-04-11 22:29:12.000000 betty-0.3.3/betty/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-04-11 22:29:12.000000 betty-0.3.3/betty/cache/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-04-11 22:29:12.000000 betty-0.3.3/betty/cache/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-11 22:29:12.000000 betty-0.3.3/betty/cache/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-11 22:29:12.000000 betty-0.3.3/betty/classtools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10453 2024-04-11 22:29:12.000000 betty-0.3.3/betty/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-04-11 22:29:12.000000 betty-0.3.3/betty/concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22568 2024-04-11 22:29:12.000000 betty-0.3.3/betty/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-11 22:29:12.000000 betty-0.3.3/betty/contextlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10802 2024-04-11 22:29:12.000000 betty-0.3.3/betty/deriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-11 22:29:12.000000 betty-0.3.3/betty/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-04-11 22:29:12.000000 betty-0.3.3/betty/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-11 22:29:12.000000 betty-0.3.3/betty/error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.206239 betty-0.3.3/betty/extension/
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.210239 betty-0.3.3/betty/extension/cotton_candy/
+-rw-r--r--   0 runner    (1001) docker     (127)    14934 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.190239 betty-0.3.3/betty/extension/cotton_candy/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.190239 betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.210239 betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/accessibility.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/citation.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/entity.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/file.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/file.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/main.js
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/main.scss
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/meta.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/overlay.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/page.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/permalink.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/person.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     6321 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/search.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/search.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/show.js
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/show.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/text.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/variables.scss.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/webpack.config.js
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/webpack.config.json.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.190239 betty-0.3.3/betty/extension/cotton_candy/assets/public/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.210239 betty-0.3.3/betty/extension/cotton_candy/assets/public/localized/
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/public/localized/index.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/public/localized/search-index.json.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.214239 betty-0.3.3/betty/extension/cotton_candy/assets/public/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/public/static/betty.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/public/static/search-configuration.json.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.214239 betty-0.3.3/betty/extension/cotton_candy/assets/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     6717 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/base.html.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.218239 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/featured--place.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/featured.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/label--citation.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/label--event.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/label--person-name.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/label--person.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/label--place.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/label--source.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/label.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/list--event.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/list--file.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/list--person.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/list--place.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/meta--citation.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/meta--event.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/meta--file.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/meta--person.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/meta--place.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/meta--source.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/page--citation.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/page--event.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/page--file.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)    12475 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/page--person.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/page--place.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/page--source.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/page-list--event.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/page-list--file.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/page-list--person.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/page-list--place.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/page-list--source.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/event-dimensions.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/file-extended--application--pdf.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/file-extended--image.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/file-extended.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/file-summary--application--pdf.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/file-summary--image.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/file-summary.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/file.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/footer.html.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.218239 betty-0.3.3/betty/extension/cotton_candy/assets/templates/macro/
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/macro/citation.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/media.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/permalink.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/references.html.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.222239 betty-0.3.3/betty/extension/cotton_candy/assets/templates/search/
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/search/result-file.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/search/result-person.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/search/result-place.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/search/result-with-image.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/search/result.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/search/results.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/section-notes.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/show-countable.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/show.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/timeline.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.222239 betty-0.3.3/betty/extension/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)    16485 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/demo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.222239 betty-0.3.3/betty/extension/deriver/
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/deriver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.222239 betty-0.3.3/betty/extension/gramps/
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/gramps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/gramps/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6348 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/gramps/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.222239 betty-0.3.3/betty/extension/http_api_doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/http_api_doc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.190239 betty-0.3.3/betty/extension/http_api_doc/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.190239 betty-0.3.3/betty/extension/http_api_doc/assets/betty.extension.npm._Npm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.222239 betty-0.3.3/betty/extension/http_api_doc/assets/betty.extension.npm._Npm/src/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/http_api_doc/assets/betty.extension.npm._Npm/src/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.190239 betty-0.3.3/betty/extension/http_api_doc/assets/public/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.190239 betty-0.3.3/betty/extension/http_api_doc/assets/public/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.222239 betty-0.3.3/betty/extension/http_api_doc/assets/public/static/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/http_api_doc/assets/public/static/api/index.html.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.222239 betty-0.3.3/betty/extension/maps/
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/maps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.190239 betty-0.3.3/betty/extension/maps/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.190239 betty-0.3.3/betty/extension/maps/assets/betty.extension.npm._Npm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.222239 betty-0.3.3/betty/extension/maps/assets/betty.extension.npm._Npm/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/maps/assets/betty.extension.npm._Npm/src/maps.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/maps/assets/betty.extension.npm._Npm/src/maps.js
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/maps/assets/betty.extension.npm._Npm/src/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/maps/assets/betty.extension.npm._Npm/src/webpack.config.js
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/maps/assets/betty.extension.npm._Npm/src/webpack.config.json.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.222239 betty-0.3.3/betty/extension/nginx/
+-rw-r--r--   0 runner    (1001) docker     (127)     7658 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/nginx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/nginx/artifact.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.226239 betty-0.3.3/betty/extension/nginx/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/nginx/assets/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/nginx/assets/content_negotiation.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/nginx/assets/nginx.conf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/nginx/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/nginx/serve.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.226239 betty-0.3.3/betty/extension/npm/
+-rw-r--r--   0 runner    (1001) docker     (127)     8979 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/npm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.226239 betty-0.3.3/betty/extension/privatizer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/privatizer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.226239 betty-0.3.3/betty/extension/trees/
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/trees/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.194239 betty-0.3.3/betty/extension/trees/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.194239 betty-0.3.3/betty/extension/trees/assets/betty.extension.npm._Npm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.226239 betty-0.3.3/betty/extension/trees/assets/betty.extension.npm._Npm/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/trees/assets/betty.extension.npm._Npm/src/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/trees/assets/betty.extension.npm._Npm/src/trees.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/trees/assets/betty.extension.npm._Npm/src/trees.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/trees/assets/betty.extension.npm._Npm/src/webpack.config.js
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/trees/assets/betty.extension.npm._Npm/src/webpack.config.json.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.194239 betty-0.3.3/betty/extension/trees/assets/public/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.226239 betty-0.3.3/betty/extension/trees/assets/public/localized/
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/trees/assets/public/localized/people.json.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.226239 betty-0.3.3/betty/extension/wikipedia/
+-rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/wikipedia/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.194239 betty-0.3.3/betty/extension/wikipedia/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.226239 betty-0.3.3/betty/extension/wikipedia/assets/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/wikipedia/assets/templates/wikipedia.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-04-11 22:29:12.000000 betty-0.3.3/betty/fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-04-11 22:29:12.000000 betty-0.3.3/betty/functools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13505 2024-04-11 22:29:12.000000 betty-0.3.3/betty/generate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.226239 betty-0.3.3/betty/gramps/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-11 22:29:12.000000 betty-0.3.3/betty/gramps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-11 22:29:12.000000 betty-0.3.3/betty/gramps/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31162 2024-04-11 22:29:12.000000 betty-0.3.3/betty/gramps/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.230239 betty-0.3.3/betty/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)     5076 2024-04-11 22:29:12.000000 betty-0.3.3/betty/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12727 2024-04-11 22:29:12.000000 betty-0.3.3/betty/gui/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6310 2024-04-11 22:29:12.000000 betty-0.3.3/betty/gui/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-04-11 22:29:12.000000 betty-0.3.3/betty/gui/locale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-04-11 22:29:12.000000 betty-0.3.3/betty/gui/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-04-11 22:29:12.000000 betty-0.3.3/betty/gui/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31464 2024-04-11 22:29:12.000000 betty-0.3.3/betty/gui/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5545 2024-04-11 22:29:12.000000 betty-0.3.3/betty/gui/serve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-11 22:29:12.000000 betty-0.3.3/betty/gui/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-11 22:29:12.000000 betty-0.3.3/betty/gui/window.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-11 22:29:12.000000 betty-0.3.3/betty/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-11 22:29:12.000000 betty-0.3.3/betty/importlib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.230239 betty-0.3.3/betty/jinja2/
+-rw-r--r--   0 runner    (1001) docker     (127)    10099 2024-04-11 22:29:12.000000 betty-0.3.3/betty/jinja2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15988 2024-04-11 22:29:12.000000 betty-0.3.3/betty/jinja2/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-11 22:29:12.000000 betty-0.3.3/betty/jinja2/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-11 22:29:12.000000 betty-0.3.3/betty/job.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.230239 betty-0.3.3/betty/json/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-11 22:29:12.000000 betty-0.3.3/betty/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-11 22:29:12.000000 betty-0.3.3/betty/json/linked_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4512 2024-04-11 22:29:12.000000 betty-0.3.3/betty/json/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-11 22:29:12.000000 betty-0.3.3/betty/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36985 2024-04-11 22:29:12.000000 betty-0.3.3/betty/locale.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-11 22:29:12.000000 betty-0.3.3/betty/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-11 22:29:12.000000 betty-0.3.3/betty/media_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.230239 betty-0.3.3/betty/model/
+-rw-r--r--   0 runner    (1001) docker     (127)    35361 2024-04-11 22:29:12.000000 betty-0.3.3/betty/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56370 2024-04-11 22:29:12.000000 betty-0.3.3/betty/model/ancestry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7118 2024-04-11 22:29:12.000000 betty-0.3.3/betty/model/event_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-04-11 22:29:12.000000 betty-0.3.3/betty/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-11 22:29:12.000000 betty-0.3.3/betty/os.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-11 22:29:12.000000 betty-0.3.3/betty/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10139 2024-04-11 22:29:12.000000 betty-0.3.3/betty/privatizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29182 2024-04-11 22:29:12.000000 betty-0.3.3/betty/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 22:29:12.000000 betty-0.3.3/betty/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-11 22:29:12.000000 betty-0.3.3/betty/render.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.230239 betty-0.3.3/betty/serde/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-11 22:29:12.000000 betty-0.3.3/betty/serde/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-04-11 22:29:12.000000 betty-0.3.3/betty/serde/dump.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-04-11 22:29:12.000000 betty-0.3.3/betty/serde/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-11 22:29:12.000000 betty-0.3.3/betty/serde/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15310 2024-04-11 22:29:12.000000 betty-0.3.3/betty/serde/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7603 2024-04-11 22:29:12.000000 betty-0.3.3/betty/serve.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.230239 betty-0.3.3/betty/sphinx/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-11 22:29:12.000000 betty-0.3.3/betty/sphinx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.230239 betty-0.3.3/betty/sphinx/extension/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-11 22:29:12.000000 betty-0.3.3/betty/sphinx/extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-11 22:29:12.000000 betty-0.3.3/betty/sphinx/extension/replacements.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-11 22:29:12.000000 betty-0.3.3/betty/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-11 22:29:12.000000 betty-0.3.3/betty/subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-04-11 22:29:12.000000 betty-0.3.3/betty/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-11 22:29:12.000000 betty-0.3.3/betty/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16686 2024-04-11 22:29:12.000000 betty-0.3.3/betty/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.230239 betty-0.3.3/betty.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    43400 2024-04-11 22:30:11.000000 betty-0.3.3/betty.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10371 2024-04-11 22:30:12.000000 betty-0.3.3/betty.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 22:30:11.000000 betty-0.3.3/betty.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-11 22:30:11.000000 betty-0.3.3/betty.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-11 22:30:11.000000 betty-0.3.3/betty.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-11 22:30:11.000000 betty-0.3.3/betty.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.230239 betty-0.3.3/documentation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-04-11 22:29:12.000000 betty-0.3.3/documentation/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.194239 betty-0.3.3/node_modules/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.194239 betty-0.3.3/node_modules/flatted/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.230239 betty-0.3.3/node_modules/flatted/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-04-11 22:29:59.000000 betty-0.3.3/node_modules/flatted/python/flatted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-11 22:29:59.000000 betty-0.3.3/node_modules/flatted/python/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4873 2024-04-11 22:29:12.000000 betty-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 22:30:12.238239 betty-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-11 22:29:12.000000 betty-0.3.3/setup.py
```

### Comparing `betty-0.3.2/LICENSE.txt` & `betty-0.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/PKG-INFO` & `betty-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betty
-Version: 0.3.2
+Version: 0.3.3
 Summary: Betty helps you visualize and publish your family history by building interactive genealogy websites out of your Gramps and GECOM family trees
 Author-email: Bart Feenstra <bar@bartfeenstra.com>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -625,25 +625,33 @@
         
                              END OF TERMS AND CONDITIONS
         
 Project-URL: Documentation, https://betty.readthedocs.io
 Project-URL: Github, https://github.com/bartfeenstra/betty
 Project-URL: Twitter, https://twitter.com/BettyProject
 Project-URL: X, https://twitter.com/BettyProject
+Classifier: Environment :: Console
+Classifier: Environment :: X11 Applications :: Qt
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Lua
 Classifier: Programming Language :: JavaScript
+Classifier: Programming Language :: Unix Shell
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Internet
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Sociology :: Genealogy
+Classifier: Topic :: Sociology :: History
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Natural Language :: Dutch
 Classifier: Natural Language :: English
 Classifier: Natural Language :: French
 Classifier: Natural Language :: German
 Classifier: Natural Language :: Ukrainian
 Classifier: Typing :: Typed 
@@ -661,19 +669,20 @@
 Requires-Dist: langcodes>=3.3.0,~=3.3
 Requires-Dist: markupsafe>=2.1.1,~=2.1
 Requires-Dist: pdf2image>=1.16.0,~=1.16
 Requires-Dist: polib>=1.2.0,~=1.2
 Requires-Dist: Pillow>=10.1.0,~=10.1
 Requires-Dist: PyQt6>=6.5.0,~=6.5
 Requires-Dist: pyyaml>=6.0.0,~=6.0
-Requires-Dist: referencing~=0.34.0
-Requires-Dist: sphinx~=7.2.6
-Requires-Dist: sphinx-design~=0.5.0
-Requires-Dist: sphinx-immaterial~=0.11.10
-Requires-Dist: sphinx-autodoc-typehints~=2.0.0
+Requires-Dist: referencing>=0.34.0,~=0.34
+Requires-Dist: sphinx>=7.2.6,~=7.2
+Requires-Dist: sphinx-design>=0.5.0,~=0.5
+Requires-Dist: sphinx-immaterial>=0.11.10,~=0.11
+Requires-Dist: sphinx-autodoc-typehints>=2.0.0,~=2.0
+Requires-Dist: typing_extensions>=4.10.0,~=4.10
 Provides-Extra: pyinstaller
 Requires-Dist: pyinstaller>=6.1.0,~=6.1; extra == "pyinstaller"
 Provides-Extra: setuptools
 Requires-Dist: setuptools~=69.0; extra == "setuptools"
 Requires-Dist: twine~=5.0; extra == "setuptools"
 Requires-Dist: wheel>=0.40.0,~=0.40; extra == "setuptools"
 Provides-Extra: test
@@ -689,18 +698,23 @@
 Requires-Dist: pytest>=7.3.1,~=7.3; extra == "test"
 Requires-Dist: pytest-aioresponses>=0.2.0,~=0.2; extra == "test"
 Requires-Dist: pytest-asyncio>=0.23.4,~=0.23; extra == "test"
 Requires-Dist: pytest-cov~=5.0; extra == "test"
 Requires-Dist: pytest-mock>=3.10.0,~=3.10; extra == "test"
 Requires-Dist: pytest-qt>=4.2.0,~=4.2; extra == "test"
 Requires-Dist: pytest-xvfb>=3.0.0,~=3.0; extra == "test"
-Requires-Dist: types-aiofiles>=23.2.0.0,~=23.2; extra == "test"
+Requires-Dist: types-aiofiles>=23.2.0.20240403,~=23.2; extra == "test"
+Requires-Dist: types-babel>=2.11.0.15,~=2.11; extra == "test"
 Requires-Dist: types-click>=7.1.8,~=7.1; extra == "test"
+Requires-Dist: types-html5lib>=1.1.11.20240228,~=1.1; extra == "test"
+Requires-Dist: types-jsonschema>=4.21.0.20240331,~=4.21; extra == "test"
+Requires-Dist: types-lxml>=2024.3.27; extra == "test"
 Requires-Dist: types-mock>=5.0.0.6,~=5.0; extra == "test"
 Requires-Dist: types-polib>=1.2.0.0,~=1.2; extra == "test"
+Requires-Dist: types-pyinstaller>=6.5.0.20240311,~=6.5; extra == "test"
 Requires-Dist: types-pyyaml>=6.0.6,~=6.0; extra == "test"
 Requires-Dist: types-requests>=2.29.0.0,~=2.29; extra == "test"
 Requires-Dist: types-setuptools~=69.0; extra == "test"
 Requires-Dist: betty[pyinstaller]; extra == "test"
 Requires-Dist: betty[setuptools]; extra == "test"
 Provides-Extra: development
 Requires-Dist: pytest-repeat>=0.9.1,~=0.9; extra == "development"
```

### Comparing `betty-0.3.2/README.md` & `betty-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/_package/pyinstaller/__init__.py` & `betty-0.3.3/betty/_package/pyinstaller/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 async def _build_assets() -> None:
     npm_builder_extension_types: list[type[_NpmBuilder & Extension]] = [
         extension_type
         for extension_type
         in discover_extension_types()
         if issubclass(extension_type, _NpmBuilder)
     ]
-    async with App() as app:
+    async with (App.new_temporary() as app, app):
         app.project.configuration.extensions.append(ExtensionConfiguration(_Npm))
         for extension_type in npm_builder_extension_types:
             app.project.configuration.extensions.append(ExtensionConfiguration(extension_type))
         await gather(*([
             build_assets(app.extensions[extension_type])  # type: ignore[arg-type]
             for extension_type
             in npm_builder_extension_types
```

### Comparing `betty-0.3.2/betty/_patch.py` & `betty-0.3.3/betty/_patch.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/_resizeimage.py` & `betty-0.3.3/betty/_resizeimage.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/about.py` & `betty-0.3.3/betty/about.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/app/__init__.py` & `betty-0.3.3/betty/app/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 """Define Betty's core application functionality."""
 
 from __future__ import annotations
 
 import operator
 import weakref
+from collections.abc import AsyncIterator
 from concurrent.futures import Executor, ProcessPoolExecutor
-from contextlib import suppress
+from contextlib import suppress, asynccontextmanager
 from functools import reduce
 from graphlib import CycleError, TopologicalSorter
 from multiprocessing import get_context
 from pathlib import Path
 from types import TracebackType
-from typing import TYPE_CHECKING, Mapping, Self, final
+from typing import TYPE_CHECKING, Mapping, Self, Any, final
 
 import aiohttp
+from aiofiles.tempfile import TemporaryDirectory
 
 from betty import fs
 from betty.app.extension import ListExtensions, Extension, Extensions, build_extension_type_graph, \
     CyclicDependencyError, ExtensionDispatcher, ConfigurableExtension, discover_extension_types
-from betty.asyncio import sync, wait
-from betty.cache import FileCache
+from betty.asyncio import wait_to_thread
+from betty.cache import Cache, FileCache
+from betty.cache.file import BinaryFileCache, PickledFileCache
 from betty.config import Configurable, FileBasedConfiguration
 from betty.dispatch import Dispatcher
-from betty.fs import FileSystem, ASSETS_DIRECTORY_PATH
+from betty.fs import FileSystem, CACHE_DIRECTORY_PATH
 from betty.locale import LocalizerRepository, get_data, DEFAULT_LOCALE, Localizer, Str
 from betty.model import Entity, EntityTypeProvider
 from betty.model.event_type import EventType, EventTypeProvider, Birth, Baptism, Adoption, Death, Funeral, Cremation, \
     Burial, Will, Engagement, Marriage, MarriageAnnouncement, Divorce, DivorceAnnouncement, Residence, Immigration, \
     Emigration, Occupation, Retirement, Correspondence, Confirmation
 from betty.project import Project
 from betty.render import Renderer, SequentialRenderer
-from betty.serde.dump import minimize, void_none, Dump, VoidableDump, Void
+from betty.serde.dump import minimize, void_none, Dump, VoidableDump
 from betty.serde.load import AssertionFailed, Fields, Assertions, OptionalField, Asserter
+from betty.warnings import deprecate
 
 if TYPE_CHECKING:
     from betty.jinja2 import Environment
     from betty.serve import Server
     from betty.url import StaticUrlGenerator, LocalizedUrlGenerator
 
 CONFIGURATION_DIRECTORY_PATH = fs.HOME_DIRECTORY_PATH / 'configuration'
@@ -48,23 +52,31 @@
     def _update(self, extensions: list[list[Extension]]) -> None:
         self._extensions = extensions
 
 
 class AppConfiguration(FileBasedConfiguration):
     def __init__(
         self,
+        configuration_directory_path: Path | None = None,
         *,
         locale: str | None = None,
     ):
+        if configuration_directory_path is None:
+            deprecate(
+                f'Initializing {type(self)} without a configuration directory path is deprecated as of Betty 0.3.3, and will be removed in Betty 0.4.x.',
+                stacklevel=2,
+            )
+            configuration_directory_path = CONFIGURATION_DIRECTORY_PATH
         super().__init__()
+        self._configuration_directory_path = configuration_directory_path
         self._locale: str | None = locale
 
     @property
     def configuration_file_path(self) -> Path:
-        return CONFIGURATION_DIRECTORY_PATH / 'app.json'
+        return self._configuration_directory_path / 'app.json'
 
     @configuration_file_path.setter
     def configuration_file_path(self, __) -> None:
         pass
 
     @configuration_file_path.deleter
     def configuration_file_path(self) -> None:
@@ -109,75 +121,132 @@
 
     def dump(self) -> VoidableDump:
         return minimize({
             'locale': void_none(self.locale)
         }, True)
 
 
+class _BackwardsCompatiblePickledFileCache(PickledFileCache[Any], FileCache):
+    """
+    Provide a Backwards Compatible cache.
+
+    .. deprecated:: 0.3.3
+       This class is deprecated as of Betty 0.3.3, and will be removed in Betty 0.4.x.
+    """
+
+    @property
+    def path(self) -> Path:
+        return self._path
+
+
 @final
 class App(Configurable[AppConfiguration]):
     def __init__(
         self,
         configuration: AppConfiguration | None = None,
         project: Project | None = None,
+        cache_directory_path: Path | None = None,
     ):
         super().__init__()
         self._started = False
+        if configuration is None:
+            deprecate(
+                f'Initializing {type(self)} without `configuration` is deprecated as of Betty 0.3.2, and will be removed in Betty 0.4.x.',
+                stacklevel=2,
+            )
+        if cache_directory_path is None:
+            deprecate(
+                f'Initializing {type(self)} without `cache_directory_path` is deprecated as of Betty 0.3.2, and will be removed in Betty 0.4.x.',
+                stacklevel=2,
+            )
         self._configuration = configuration or AppConfiguration()
         self._configuration.on_change(self._on_locale_change)
         self._assets: FileSystem | None = None
         self._extensions = _AppExtensions()
         self._extensions_initialized = False
         self._localization_initialized = False
         self._localizer: Localizer | None = None
         self._localizers: LocalizerRepository | None = None
         with suppress(FileNotFoundError):
-            wait(self.configuration.read())
+            wait_to_thread(self.configuration.read())
         self._project = project or Project()
         self.project.configuration.extensions.on_change(self._update_extensions)
 
         self._dispatcher: ExtensionDispatcher | None = None
         self._entity_types: set[type[Entity]] | None = None
         self._event_types: set[type[EventType]] | None = None
         self._url_generator: LocalizedUrlGenerator | None = None
         self._static_url_generator: StaticUrlGenerator | None = None
         self._jinja2_environment: Environment | None = None
         self._renderer: Renderer | None = None
         self._http_client: aiohttp.ClientSession | None = None
-        self._cache: FileCache | None = None
+        self._cache_directory_path = CACHE_DIRECTORY_PATH if cache_directory_path is None else cache_directory_path
+        self._cache: Cache[Any] & FileCache | None = None
+        self._binary_file_cache: BinaryFileCache | None = None
         self._process_pool: Executor | None = None
 
     @classmethod
-    def _unreduce(cls, dumped_app_configuration: VoidableDump, project: Project) -> Self:
-        if dumped_app_configuration is Void:
-            app_configuration = None
-        else:
-            app_configuration = AppConfiguration.load(
-                dumped_app_configuration,  # type: ignore[arg-type]
-            )
-        return App(
-            app_configuration,
+    @asynccontextmanager
+    async def new_from_environment(
+        cls,
+        *,
+        project: Project | None = None,
+    ) -> AsyncIterator[Self]:
+        yield cls(
+            AppConfiguration(CONFIGURATION_DIRECTORY_PATH),
             project,
+            CACHE_DIRECTORY_PATH,
         )
 
+    @classmethod
+    @asynccontextmanager
+    async def new_from_app(
+        cls,
+        app: App,
+        *,
+        project: Project | None = None,
+    ) -> AsyncIterator[Self]:
+        yield cls(
+            AppConfiguration(app.configuration._configuration_directory_path),
+            app.project if project is None else project,
+            app._cache_directory_path,
+        )
+
+    @classmethod
+    @asynccontextmanager
+    async def new_temporary(
+        cls,
+        *,
+        project: Project | None = None,
+    ) -> AsyncIterator[Self]:
+        async with (
+            TemporaryDirectory() as configuration_directory_path_str,
+            TemporaryDirectory() as cache_directory_path_str,
+        ):
+            yield cls(
+                AppConfiguration(Path(configuration_directory_path_str)),
+                project,
+                cache_directory_path=Path(cache_directory_path_str),
+            )
+
     async def __aenter__(self) -> Self:
         await self.start()
         return self
 
     async def __aexit__(self, exc_type: type[BaseException] | None, exc_val: BaseException | None, exc_tb: TracebackType | None) -> None:
         await self.stop()
 
     async def start(self) -> None:
         if self._started:
             raise RuntimeError('This app has started already.')
         self._started = True
 
     async def stop(self) -> None:
-        self._started = False
         del self.http_client
+        self._started = False
 
     def __del__(self) -> None:
         if self._started:
             raise RuntimeError(f'{self} was started, but never stopped.')
 
     def _on_locale_change(self) -> None:
         del self.localizer
@@ -224,29 +293,29 @@
             for extension_type in extension_types_batch:
                 if issubclass(extension_type, ConfigurableExtension) and extension_type in self.project.configuration.extensions:
                     extension: Extension = extension_type(self, configuration=self.project.configuration.extensions[extension_type].extension_configuration)
                 else:
                     extension = extension_type(self)
                 extensions_batch.append(extension)
                 extension_types_sorter.done(extension_type)
-            extensions.append(extensions_batch)
+            extensions.append(sorted(extensions_batch, key=lambda extension: extension.name()))
         self._extensions._update(extensions)
         del self.assets
         del self.localizers
         del self.localizer
         del self.jinja2_environment
         del self.renderer
         del self.entity_types
         del self.event_types
 
     @property
     def assets(self) -> FileSystem:
         if self._assets is None:
             assets = FileSystem()
-            assets.prepend(ASSETS_DIRECTORY_PATH, 'utf-8')
+            assets.prepend(fs.ASSETS_DIRECTORY_PATH, 'utf-8')
             for extension in self.extensions.flatten():
                 extension_assets_directory_path = extension.assets_directory_path()
                 if extension_assets_directory_path is not None:
                     assets.prepend(extension_assets_directory_path, 'utf-8')
             assets.prepend(self.project.configuration.assets_directory_path)
             self._assets = assets
         return self._assets
@@ -280,20 +349,22 @@
 
     @property
     def localizer(self) -> Localizer:
         """
         Get the application's localizer.
         """
         if self._localizer is None:
-            self._localizer = wait(self.localizers.get_negotiated(self.configuration.locale or DEFAULT_LOCALE))
+            self._localizer = wait_to_thread(self.localizers.get_negotiated(self.configuration.locale or DEFAULT_LOCALE))
         return self._localizer
 
     @localizer.deleter
     def localizer(self) -> None:
         self._localizer = None
+        del self.cache
+        del self.binary_file_cache
 
     @property
     def localizers(self) -> LocalizerRepository:
         if self._localizers is None:
             self._localizers = LocalizerRepository(self.assets)
         return self._localizers
 
@@ -333,29 +404,29 @@
         if not self._http_client:
             self._http_client = aiohttp.ClientSession(
                 connector=aiohttp.TCPConnector(limit_per_host=5),
                 headers={
                     'User-Agent': f'Betty (https://github.com/bartfeenstra/betty) on behalf of {self._project.configuration.base_url}{self._project.configuration.root_path}',
                 },
             )
-            weakref.finalize(self, sync(self._http_client.close))
+            weakref.finalize(self, lambda: None if self._http_client is None else wait_to_thread(self._http_client.close()))
         return self._http_client
 
     @http_client.deleter
     def http_client(self) -> None:
         if self._http_client is not None:
-            wait(self._http_client.close())
+            wait_to_thread(self._http_client.close())
             self._http_client = None
 
     @property
     def entity_types(self) -> set[type[Entity]]:
         if self._entity_types is None:
             from betty.model.ancestry import Citation, Enclosure, Event, File, Note, Person, PersonName, Presence, Place, Source
 
-            self._entity_types = reduce(operator.or_, wait(self.dispatcher.dispatch(EntityTypeProvider)()), set()) | {
+            self._entity_types = reduce(operator.or_, wait_to_thread(self.dispatcher.dispatch(EntityTypeProvider)()), set()) | {
                 Citation,
                 Enclosure,
                 Event,
                 File,
                 Note,
                 Person,
                 PersonName,
@@ -368,15 +439,15 @@
     @entity_types.deleter
     def entity_types(self) -> None:
         self._entity_types = None
 
     @property
     def event_types(self) -> set[type[EventType]]:
         if self._event_types is None:
-            self._event_types = set(wait(self.dispatcher.dispatch(EventTypeProvider)())) | {
+            self._event_types = set(wait_to_thread(self.dispatcher.dispatch(EventTypeProvider)())) | {
                 Birth,
                 Baptism,
                 Adoption,
                 Death,
                 Funeral,
                 Cremation,
                 Burial,
@@ -412,24 +483,38 @@
                 *(
                     server
                     for extension in self.extensions.flatten()
                     if isinstance(extension, serve.ServerProvider)
                     for server in extension.servers
                 ),
                 serve.BuiltinAppServer(self),
-                DemoServer(),
+                DemoServer(app=self),
             ]
         }
 
     @property
-    def cache(self) -> FileCache:
+    def cache(self) -> Cache[Any] & FileCache:
         if self._cache is None:
-            self._cache = FileCache(self.localizer, fs.CACHE_DIRECTORY_PATH)
+            self._cache = _BackwardsCompatiblePickledFileCache(self.localizer, self._cache_directory_path)
         return self._cache
 
+    @cache.deleter
+    def cache(self) -> None:
+        self._cache = None
+
+    @property
+    def binary_file_cache(self) -> BinaryFileCache:
+        if self._binary_file_cache is None:
+            self._binary_file_cache = BinaryFileCache(self.localizer, self._cache_directory_path)
+        return self._binary_file_cache
+
+    @binary_file_cache.deleter
+    def binary_file_cache(self) -> None:
+        self._binary_file_cache = None
+
     @property
     def process_pool(self) -> Executor:
         if self._process_pool is None:
             # Avoid `fork` so as not to start worker processes with unneeded resources.
             # Settle for `spawn` so all environments use the same start method.
             self._process_pool = ProcessPoolExecutor(mp_context=get_context('spawn'))
         return self._process_pool
```

### Comparing `betty-0.3.2/betty/app/extension/__init__.py` & `betty-0.3.3/betty/app/extension/__init__.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/app/extension/requirement.py` & `betty-0.3.3/betty/app/extension/requirement.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/assets/betty.pot` & `betty-0.3.3/betty/assets/betty.pot`

 * *Files 0% similar despite different names*

```diff
@@ -62,14 +62,17 @@
 
 msgid "\"{locale}\" is not a valid IETF BCP 47 language tag."
 msgstr ""
 
 msgid "\"{path}\" is not a directory."
 msgstr ""
 
+msgid "\"{scope}\" cache cleared."
+msgstr ""
+
 #, python-format
 msgid "%(date)s in %(place)s"
 msgstr ""
 
 #, python-format
 msgid "%(event)s of %(subjects)s"
 msgstr ""
```

### Comparing `betty-0.3.2/betty/assets/locale/de-DE/betty.po` & `betty-0.3.3/betty/assets/locale/de-DE/betty.po`

 * *Files 0% similar despite different names*

```diff
@@ -100,14 +100,17 @@
 
 msgid "\"{locale}\" is not a valid IETF BCP 47 language tag."
 msgstr "\"{locale}\" ist kein gültiger IETF BCP 47 language tag."
 
 msgid "\"{path}\" is not a directory."
 msgstr "\"{path}\" ist kein Verzeichnis."
 
+msgid "\"{scope}\" cache cleared."
+msgstr ""
+
 #, python-format
 msgid "%(date)s in %(place)s"
 msgstr "%(date)s in %(place)s"
 
 #, python-format
 msgid "%(event)s of %(subjects)s"
 msgstr "%(event)s von %(subjects)s"
```

### Comparing `betty-0.3.2/betty/assets/locale/fr-FR/betty.po` & `betty-0.3.3/betty/assets/locale/fr-FR/betty.po`

 * *Files 0% similar despite different names*

```diff
@@ -74,14 +74,17 @@
 
 msgid "\"{locale}\" is not a valid IETF BCP 47 language tag."
 msgstr ""
 
 msgid "\"{path}\" is not a directory."
 msgstr ""
 
+msgid "\"{scope}\" cache cleared."
+msgstr ""
+
 #, python-format
 msgid "%(date)s in %(place)s"
 msgstr "%(date)s à %(place)s"
 
 #, python-format
 msgid "%(event)s of %(subjects)s"
 msgstr "%(event)s de  %(subjects)s"
```

### Comparing `betty-0.3.2/betty/assets/locale/nl-NL/betty.po` & `betty-0.3.3/betty/assets/locale/nl-NL/betty.po`

 * *Files 0% similar despite different names*

```diff
@@ -99,14 +99,17 @@
 
 msgid "\"{locale}\" is not a valid IETF BCP 47 language tag."
 msgstr "\"{locale}\" is geen geldige IETF BCP 47 taaltag."
 
 msgid "\"{path}\" is not a directory."
 msgstr "\"{path}\" is geen directory."
 
+msgid "\"{scope}\" cache cleared."
+msgstr "\"{scope}\"-cache geleegd."
+
 #, python-format
 msgid "%(date)s in %(place)s"
 msgstr "%(date)s te %(place)s"
 
 #, python-format
 msgid "%(event)s of %(subjects)s"
 msgstr "%(event)s van %(subjects)s"
```

### Comparing `betty-0.3.2/betty/assets/locale/uk/betty.po` & `betty-0.3.3/betty/assets/locale/uk/betty.po`

 * *Files 0% similar despite different names*

```diff
@@ -75,14 +75,17 @@
 
 msgid "\"{locale}\" is not a valid IETF BCP 47 language tag."
 msgstr ""
 
 msgid "\"{path}\" is not a directory."
 msgstr ""
 
+msgid "\"{scope}\" cache cleared."
+msgstr ""
+
 #, python-format
 msgid "%(date)s in %(place)s"
 msgstr "%(date)s в %(place)s"
 
 #, python-format
 msgid "%(event)s of %(subjects)s"
 msgstr "%(event)s %(subjects)s"
```

### Comparing `betty-0.3.2/betty/assets/public/static/betty-16x16.png` & `betty-0.3.3/betty/assets/public/static/betty-16x16.png`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/assets/public/static/betty-192x192.png` & `betty-0.3.3/betty/assets/public/static/betty-192x192.png`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/assets/public/static/betty-32x32.png` & `betty-0.3.3/betty/assets/public/static/betty-32x32.png`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/assets/public/static/betty-512x512.png` & `betty-0.3.3/betty/assets/public/static/betty-512x512.png`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/assets/public/static/betty.ico` & `betty-0.3.3/betty/assets/public/static/betty.ico`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/assets/templates/head.html.j2` & `betty-0.3.3/betty/assets/templates/head.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/asyncio.py` & `betty-0.3.3/betty/asyncio.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """
 Provide asynchronous programming utilities.
 """
 from __future__ import annotations
 
-import asyncio
-from asyncio import TaskGroup
+from asyncio import TaskGroup, get_running_loop, run
 from functools import wraps
 from threading import Thread
 from typing import Callable, Awaitable, TypeVar, Generic, cast, ParamSpec, Coroutine, Any
 
+from betty.warnings import deprecated
+
 P = ParamSpec('P')
 T = TypeVar('T')
 
 
 async def gather(*coroutines: Coroutine[Any, None, T]) -> tuple[T, ...]:
     """
     Gather multiple coroutines.
@@ -26,55 +27,66 @@
     return tuple(
         task.result()
         for task
         in tasks
     )
 
 
+@deprecated('This function is deprecated as of Betty 0.3.3, and will be removed in Betty 0.4.x. Instead, use `betty.asyncio.wait_to_thread()` or `asyncio.run()`.')
 def wait(f: Awaitable[T]) -> T:
     """
-    Wait for an awaitable.
+    Wait for an awaitable, either in a new event loop or another thread.
     """
     try:
-        loop = asyncio.get_running_loop()
+        loop = get_running_loop()
     except RuntimeError:
         loop = None
     if loop:
-        synced = _SyncedAwaitable(f)
-        synced.start()
-        synced.join()
-        return synced.return_value
+        return wait_to_thread(f)
     else:
-        return asyncio.run(
+        return run(
             f,  # type: ignore[arg-type]
         )
 
 
+def wait_to_thread(f: Awaitable[T]) -> T:
+    """
+    Wait for an awaitable in another thread.
+    """
+    synced = _WaiterThread(f)
+    synced.start()
+    synced.join()
+    return synced.return_value
+
+
+@deprecated('This function is deprecated as of Betty 0.3.3, and will be removed in Betty 0.4.x. Instead, use `betty.asyncio.wait_to_thread()` or `asyncio.run()`.')
 def sync(f: Callable[P, Awaitable[T]]) -> Callable[P, T]:
     """
     Decorate an asynchronous callable to become synchronous.
     """
     @wraps(f)
     def _synced(*args: P.args, **kwargs: P.kwargs) -> T:
         return wait(f(*args, **kwargs))
     return _synced
 
 
-class _SyncedAwaitable(Thread, Generic[T]):
+class _WaiterThread(Thread, Generic[T]):
     def __init__(self, awaitable: Awaitable[T]):
         super().__init__()
         self._awaitable = awaitable
         self._return_value: T | None = None
         self._e: BaseException | None = None
 
     @property
     def return_value(self) -> T:
         if self._e:
             raise self._e
         return cast(T, self._return_value)
 
-    @sync
-    async def run(self) -> None:
+    def run(self) -> None:
+        run(self._run())
+
+    async def _run(self) -> None:
         try:
             self._return_value = await self._awaitable
         except BaseException as e:
             self._e = e
```

### Comparing `betty-0.3.2/betty/cli.py` & `betty-0.3.3/betty/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,17 +11,18 @@
 from pathlib import Path
 from typing import Callable, TypeVar, cast, Iterator, Awaitable, ParamSpec, Concatenate
 
 import click
 from PyQt6.QtWidgets import QMainWindow
 from click import get_current_context, Context, Option, Command, Parameter
 
-from betty import about, generate, load, documentation, fs
+from betty import about, generate, load, documentation
 from betty.app import App
-from betty.asyncio import sync, wait
+from betty.asyncio import wait_to_thread
+from betty.contextlib import SynchronizedContextManager
 from betty.error import UserFacingError
 from betty.extension import demo
 from betty.gui import BettyApplication
 from betty.gui.app import WelcomeWindow
 from betty.gui.project import ProjectWindow
 from betty.locale import update_translations, init_translation, Str
 from betty.logging import CliHandler
@@ -44,16 +45,15 @@
     Catch and log all exceptions.
     """
     try:
         yield
     except KeyboardInterrupt:
         print('Quitting...')
         sys.exit(0)
-        pass
-    except Exception as e:
+    except BaseException as e:
         logger = logging.getLogger(__name__)
         if isinstance(e, UserFacingError):
             logger.error(str(e))
         else:
             logger.exception(e)
         sys.exit(1)
 
@@ -69,16 +69,16 @@
             # We must get the current Click context from the main thread.
             # Once that is done, we can wait for the async commands to complete, which MAY be done in a thread.
             app = get_current_context().obj['app']
 
             async def _app_command():
                 async with app:
                     await f(app, *args, **kwargs)
-            return wait(_app_command())
-        return wait(f(*args, **kwargs))
+            return wait_to_thread(_app_command())
+        return wait_to_thread(f(*args, **kwargs))
     return _command
 
 
 def global_command(f: Callable[P, Awaitable[None]]) -> Callable[P, None]:
     """
     Decorate a command to be global.
     """
@@ -89,37 +89,45 @@
     """
     Decorate a command to receive an app.
     """
     return _command(f, True)
 
 
 @catch_exceptions()
-@sync
-async def _init_ctx_app(
+def _init_ctx_app(
     ctx: Context,
     __: Option | Parameter | None = None,
     configuration_file_path: str | None = None,
 ) -> None:
+    wait_to_thread(__init_ctx_app(ctx, configuration_file_path))
+
+
+async def __init_ctx_app(
+    ctx: Context,
+    configuration_file_path: str | None = None,
+) -> None:
     ctx.ensure_object(dict)
 
     if 'initialized' in ctx.obj:
         return
     ctx.obj['initialized'] = True
 
     logging.getLogger().addHandler(CliHandler())
     logger = logging.getLogger(__name__)
 
-    app = App()
+    app = ctx.with_resource(  # type: ignore[attr-defined]
+        SynchronizedContextManager(App.new_from_environment())
+    )
     ctx.obj['commands'] = {
         'docs': _docs,
         'clear-caches': _clear_caches,
         'demo': _demo,
         'gui': _gui,
     }
-    if wait(about.is_development()):
+    if wait_to_thread(about.is_development()):
         ctx.obj['commands']['init-translation'] = _init_translation
         ctx.obj['commands']['update-translations'] = _update_translations
     ctx.obj['app'] = app
 
     if configuration_file_path is None:
         try_configuration_file_paths = [
             Path.cwd() / f'betty{extension}'
@@ -224,36 +232,35 @@
     is_eager=True,
     default=False,
     is_flag=True,
     help='Show most verbose output, including all log messages.',
     callback=_build_init_ctx_verbosity(logging.NOTSET, logging.NOTSET),
 )
 @click.version_option(
-    wait(about.version_label()),
-    message=wait(about.report()),
+    wait_to_thread(about.version_label()),
+    message=wait_to_thread(about.report()),
     prog_name='Betty',
 )
 def main(app: App, verbose: bool, more_verbose: bool, most_verbose: bool) -> None:
     """
     Launch Betty's Command-Line Interface.
     """
     pass
 
 
 @click.command(help='Clear all caches.')
-@global_command
-async def _clear_caches() -> None:
-    async with App() as app:
-        await app.cache.clear()
+@app_command
+async def _clear_caches(app: App) -> None:
+    await app.cache.clear()
 
 
 @click.command(help='Explore a demonstration site.')
-@global_command
-async def _demo() -> None:
-    async with demo.DemoServer() as server:
+@app_command
+async def _demo(app: App) -> None:
+    async with demo.DemoServer(app=app) as server:
         await server.show()
         while True:
             await asyncio.sleep(999)
 
 
 @click.command(help="Open Betty's graphical user interface (GUI).")
 @click.option(
@@ -262,24 +269,24 @@
     'configuration_file_path',
     is_eager=True,
     help='The path to a Betty project configuration file. Defaults to betty.json|yaml|yml in the current working directory.',
     callback=lambda _, __, configuration_file_path: Path(configuration_file_path) if configuration_file_path else None,
 )
 @global_command
 async def _gui(configuration_file_path: Path | None) -> None:
-    async with App() as app:
-        qapp = BettyApplication([sys.argv[0]], app=app)
-        window: QMainWindow
-        if configuration_file_path is None:
-            window = WelcomeWindow(app)
-        else:
-            await app.project.configuration.read(configuration_file_path)
-            window = ProjectWindow(app)
-        window.show()
-        sys.exit(qapp.exec())
+    async with App.new_from_environment() as app:
+        async with BettyApplication([sys.argv[0]]).with_app(app) as qapp:
+            window: QMainWindow
+            if configuration_file_path is None:
+                window = WelcomeWindow(app)
+            else:
+                await app.project.configuration.read(configuration_file_path)
+                window = ProjectWindow(app)
+            window.show()
+            sys.exit(qapp.exec())
 
 
 @click.command(help='Generate a static site.')
 @app_command
 async def _generate(app: App) -> None:
     await load.load(app)
     await generate.generate(app)
@@ -293,26 +300,27 @@
         while True:
             await asyncio.sleep(999)
 
 
 @click.command(help='View the documentation.')
 @global_command
 async def _docs():
-    async with App() as app:
-        server = documentation.DocumentationServer(
-            fs.CACHE_DIRECTORY_PATH,
-            localizer=app.localizer,
-        )
-        async with server:
-            await server.show()
-            while True:
-                await asyncio.sleep(999)
+    async with App.new_from_environment() as app:
+        async with app:
+            server = documentation.DocumentationServer(
+                app.binary_file_cache.path,
+                localizer=app.localizer,
+            )
+            async with server:
+                await server.show()
+                while True:
+                    await asyncio.sleep(999)
 
 
-if wait(about.is_development()):
+if wait_to_thread(about.is_development()):
     @click.command(short_help='Initialize a new translation', help='Initialize a new translation.\n\nThis is available only when developing Betty.')
     @click.argument('locale')
     @global_command
     async def _init_translation(locale: str) -> None:
         await init_translation(locale)
 
     @click.command(short_help='Update all existing translations', help='Update all existing translations.\n\nThis is available only when developing Betty.')
```

### Comparing `betty-0.3.2/betty/config.py` & `betty-0.3.3/betty/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from tempfile import TemporaryDirectory
 from typing import Generic, Iterable, Iterator, SupportsIndex, Hashable, \
     MutableSequence, MutableMapping, TypeVar, Any, Sequence, overload, cast, Self, TypeAlias
 
 import aiofiles
 from aiofiles.os import makedirs
 
-from betty.asyncio import wait, sync
+from betty.asyncio import wait_to_thread
 from betty.classtools import repr_instance
 from betty.functools import slice_to_range
 from betty.locale import Str
 from betty.serde.dump import Dumpable, Dump, minimize, VoidableDump, Void
 from betty.serde.error import SerdeErrorCollection
 from betty.serde.format import FormatRepository
 from betty.serde.load import Asserter, Assertion, Assertions
@@ -84,15 +84,15 @@
 
 ConfigurationT = TypeVar('ConfigurationT', bound=Configuration)
 
 
 class FileBasedConfiguration(Configuration):
     def __init__(self):
         super().__init__()
-        self._project_directory: TemporaryDirectory | None = None  # type: ignore[type-arg]
+        self._configuration_directory: TemporaryDirectory | None = None  # type: ignore[type-arg]
         self._configuration_file_path: Path | None = None
         self._autowrite = False
 
     @property
     def autowrite(self) -> bool:
         return self._autowrite
 
@@ -101,17 +101,16 @@
         if autowrite:
             if not self._autowrite:
                 self.on_change(self._on_change_write)
         else:
             self.remove_on_change(self._on_change_write)
         self._autowrite = autowrite
 
-    @sync
-    async def _on_change_write(self) -> None:
-        await self.write()
+    def _on_change_write(self) -> None:
+        wait_to_thread(self.write())
 
     async def write(self, configuration_file_path: Path | None = None) -> None:
         if configuration_file_path is not None:
             self.configuration_file_path = configuration_file_path
 
         await self._write(self.configuration_file_path)
 
@@ -140,28 +139,29 @@
                 async with aiofiles.open(self.configuration_file_path) as f:
                     read_configuration = await f.read()
                 with errors.catch(Str.plain(
                     'in {configuration_file_path}',
                     configuration_file_path=str(self.configuration_file_path.resolve()),
                 )):
                     loaded_configuration = self.load(
-                        formats.format_for(self.configuration_file_path.suffix[1:]).load(read_configuration)
+                        formats.format_for(self.configuration_file_path.suffix[1:]).load(read_configuration),
+                        self,
                     )
         self.update(loaded_configuration)
 
     def __del__(self) -> None:
-        if hasattr(self, '_project_directory') and self._project_directory is not None:
-            self._project_directory.cleanup()
+        if hasattr(self, '_configuration_directory') and self._configuration_directory is not None:
+            self._configuration_directory.cleanup()
 
     @property
     def configuration_file_path(self) -> Path:
         if self._configuration_file_path is None:
-            if self._project_directory is None:
-                self._project_directory = TemporaryDirectory()
-            wait(self._write(Path(self._project_directory.name) / f'{type(self).__name__}.json'))
+            if self._configuration_directory is None:
+                self._configuration_directory = TemporaryDirectory()
+            wait_to_thread(self._write(Path(self._configuration_directory.name) / f'{type(self).__name__}.json'))
         return cast(Path, self._configuration_file_path)
 
     @configuration_file_path.setter
     def configuration_file_path(self, configuration_file_path: Path) -> None:
         if configuration_file_path == self._configuration_file_path:
             return
         formats = FormatRepository()
```

### Comparing `betty-0.3.2/betty/deriver.py` & `betty-0.3.3/betty/deriver.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/documentation.py` & `betty-0.3.3/betty/documentation.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,16 @@
                     str(ROOT_DIRECTORY_PATH / 'betty' / 'tests'),
                 ],
                 cwd=working_directory_path,
             )
             await run_process(
                 [
                     'sphinx-build',
+                    '-j',
+                    'auto',
                     '-b',
                     'dirhtml',
                     str(source_directory_path),
                     str(output_directory_path),
                 ],
                 cwd=working_directory_path,
             )
```

### Comparing `betty-0.3.2/betty/error.py` & `betty-0.3.3/betty/error.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/__init__.py` & `betty-0.3.3/betty/extension/__init__.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/cotton_candy/__init__.py` & `betty-0.3.3/betty/extension/cotton_candy/__init__.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/citation.scss` & `betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/citation.scss`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/entity.scss` & `betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/entity.scss`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/file.js` & `betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/file.js`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/file.scss` & `betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/file.scss`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/overlay.scss` & `betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/overlay.scss`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/package.json` & `betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/package.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9951923076923077%*

 * *Differences: {"'dependencies'": "{'css-loader': '^7.1.0'}"}*

```diff
@@ -1,15 +1,15 @@
 {
     "dependencies": {
         "@babel/core": "^7.19.6",
         "@babel/preset-env": "^7.19.4",
         "babel-loader": "^9.1.0",
         "clean-webpack-plugin": "^4.0.0",
         "core-js": "^3.26.0",
-        "css-loader": "^6.7.1",
+        "css-loader": "^7.1.0",
         "mini-css-extract-plugin": "^2.6.1",
         "postcss-loader": "^8.0.0",
         "sass": "^1.56.1",
         "sass-loader": "^14.0.0",
         "style-loader": "^3.3.1",
         "webpack": "^5.74.0",
         "webpack-cli": "^5.1.4"
```

### Comparing `betty-0.3.2/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/page.scss` & `betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/page.scss`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/person.scss` & `betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/person.scss`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/search.js` & `betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/search.js`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/search.scss` & `betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/search.scss`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/show.js` & `betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/show.js`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/text.scss` & `betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/text.scss`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/variables.scss.j2` & `betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/variables.scss.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/webpack.config.js` & `betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/webpack.config.js`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/cotton_candy/assets/public/localized/index.html.j2` & `betty-0.3.3/betty/extension/cotton_candy/assets/public/localized/index.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/cotton_candy/assets/public/static/betty.webmanifest` & `betty-0.3.3/betty/extension/cotton_candy/assets/public/static/betty.webmanifest`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/cotton_candy/assets/templates/base.html.j2` & `betty-0.3.3/betty/extension/cotton_candy/assets/templates/base.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/cotton_candy/assets/templates/entity/featured--place.html.j2` & `betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/featured--place.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/cotton_candy/assets/templates/entity/featured.html.j2` & `betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/featured.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/cotton_candy/assets/templates/entity/label--citation.html.j2` & `betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/label--citation.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/cotton_candy/assets/templates/entity/label--event.html.j2` & `betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/label--event.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/cotton_candy/assets/templates/entity/label--person-name.html.j2` & `betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/label--person-name.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/cotton_candy/assets/templates/entity/label--person.html.j2` & `betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/label--person.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/cotton_candy/assets/templates/entity/label--place.html.j2` & `betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/label--place.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/cotton_candy/assets/templates/entity/list--event.html.j2` & `betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/list--event.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/cotton_candy/assets/templates/entity/list--place.html.j2` & `betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/list--place.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/cotton_candy/assets/templates/entity/meta--person.html.j2` & `betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/meta--person.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/cotton_candy/assets/templates/entity/meta--place.html.j2` & `betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/meta--place.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/cotton_candy/assets/templates/entity/page--citation.html.j2` & `betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/page--citation.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/cotton_candy/assets/templates/entity/page--event.html.j2` & `betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/page--event.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/cotton_candy/assets/templates/entity/page--file.html.j2` & `betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/page--file.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/cotton_candy/assets/templates/entity/page--person.html.j2` & `betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/page--person.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/cotton_candy/assets/templates/entity/page--place.html.j2` & `betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/page--place.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/cotton_candy/assets/templates/entity/page--source.html.j2` & `betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/page--source.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/cotton_candy/assets/templates/entity/page-list--source.html.j2` & `betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/page-list--source.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/cotton_candy/assets/templates/event-dimensions.html.j2` & `betty-0.3.3/betty/extension/cotton_candy/assets/templates/event-dimensions.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/cotton_candy/assets/templates/file.html.j2` & `betty-0.3.3/betty/extension/cotton_candy/assets/templates/file.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/cotton_candy/assets/templates/references.html.j2` & `betty-0.3.3/betty/extension/cotton_candy/assets/templates/references.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/cotton_candy/assets/templates/search/result-file.html.j2` & `betty-0.3.3/betty/extension/cotton_candy/assets/templates/search/result-file.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/cotton_candy/assets/templates/search/result-with-image.html.j2` & `betty-0.3.3/betty/extension/cotton_candy/assets/templates/search/result-with-image.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/cotton_candy/gui.py` & `betty-0.3.3/betty/extension/cotton_candy/gui.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/cotton_candy/search.py` & `betty-0.3.3/betty/extension/cotton_candy/search.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/demo/__init__.py` & `betty-0.3.3/betty/extension/demo/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,21 +4,22 @@
 from contextlib import AsyncExitStack
 
 from betty import load, generate, serve
 from betty.app import App
 from betty.app.extension import Extension
 from betty.extension.cotton_candy import CottonCandyConfiguration
 from betty.load import Loader
-from betty.locale import Date, DateRange, Str
+from betty.locale import Date, DateRange, Str, DEFAULT_LOCALIZER
 from betty.model import Entity
 from betty.model.ancestry import Place, PlaceName, Person, Presence, Subject, PersonName, Link, Source, Citation, Event, \
     Enclosure, Note
 from betty.model.event_type import Marriage, Birth, Death
 from betty.project import LocaleConfiguration, ExtensionConfiguration, EntityReference, Project
 from betty.serve import Server, NoPublicUrlBecauseServerNotStartedError
+from betty.warnings import deprecate
 
 
 class _Demo(Extension, Loader):
     @classmethod
     def depends_on(cls) -> set[type[Extension]]:
         from betty.extension import CottonCandy, HttpApiDoc, Maps, Trees, Wikipedia
 
@@ -401,41 +402,62 @@
             individual='Bart',
             affiliation='Feenstra',
         ))
         self._load(bart_feenstra)
 
 
 class DemoServer(Server):
-    def __init__(self):
-        from betty.extension import Demo
-
-        self._app = App(None, Demo.project())
-        super().__init__(localizer=self._app.localizer)
+    def __init__(
+        self,
+        *,
+        app: App | None = None,
+    ):
+        super().__init__(localizer=DEFAULT_LOCALIZER)
+        self._app = app
         self._server: Server | None = None
         self._exit_stack = AsyncExitStack()
+        if app is None:
+            deprecate(
+                f'Initializing {type(self)} with a project ID is deprecated as of Betty 0.3.2, and will be removed in Betty 0.4.x. Instead, set {type(self)}.configuration.name.',
+                stacklevel=2,
+            )
 
     @classmethod
     def label(cls) -> Str:
         return Str._('Demo')
 
     @property
     def public_url(self) -> str:
         if self._server is not None:
             return self._server.public_url
         raise NoPublicUrlBecauseServerNotStartedError()
 
     async def start(self) -> None:
+        from betty.extension import Demo
+
         await super().start()
+        project = Demo.project()
+        if self._app is None:
+            isolated_app_factory = App.new_from_environment(
+                project=project,
+            )
+        else:
+            isolated_app_factory = App.new_from_app(
+                self._app,
+                project=project,
+            )
         try:
-            await self._exit_stack.enter_async_context(self._app)
-            await load.load(self._app)
-            self._server = serve.BuiltinAppServer(self._app)
+            isolated_app = await self._exit_stack.enter_async_context(isolated_app_factory)
+            await self._exit_stack.enter_async_context(isolated_app)
+            self._localizer = isolated_app.localizer
+            await load.load(isolated_app)
+            self._server = serve.BuiltinAppServer(isolated_app)
             await self._exit_stack.enter_async_context(self._server)
-            self._app.project.configuration.base_url = self._server.public_url
-            await generate.generate(self._app)
+            isolated_app.project.configuration.base_url = self._server.public_url
+            await generate.generate(isolated_app)
         except BaseException:
             await self.stop()
             raise
         await self.assert_available()
 
     async def stop(self) -> None:
         await self._exit_stack.aclose()
```

### Comparing `betty-0.3.2/betty/extension/deriver/__init__.py` & `betty-0.3.3/betty/extension/deriver/__init__.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/gramps/__init__.py` & `betty-0.3.3/betty/extension/gramps/__init__.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/gramps/config.py` & `betty-0.3.3/betty/extension/gramps/config.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/gramps/gui.py` & `betty-0.3.3/betty/extension/gramps/gui.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/http_api_doc/__init__.py` & `betty-0.3.3/betty/extension/http_api_doc/__init__.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/http_api_doc/assets/public/static/api/index.html.j2` & `betty-0.3.3/betty/extension/http_api_doc/assets/public/static/api/index.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/maps/__init__.py` & `betty-0.3.3/betty/extension/maps/__init__.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/maps/assets/betty.extension.npm._Npm/src/maps.js` & `betty-0.3.3/betty/extension/maps/assets/betty.extension.npm._Npm/src/maps.js`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/maps/assets/betty.extension.npm._Npm/src/package.json` & `betty-0.3.3/betty/extension/maps/assets/betty.extension.npm._Npm/src/package.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9951923076923077%*

 * *Differences: {"'dependencies'": "{'css-loader': '^7.1.0'}"}*

```diff
@@ -1,15 +1,15 @@
 {
     "dependencies": {
         "@babel/core": "^7.19.6",
         "@babel/preset-env": "^7.19.4",
         "babel-loader": "^9.1.0",
         "clean-webpack-plugin": "^4.0.0",
         "core-js": "^3.26.0",
-        "css-loader": "^6.7.1",
+        "css-loader": "^7.1.0",
         "leaflet": "^1.9.2",
         "leaflet-gesture-handling": "^1.2.2",
         "leaflet.fullscreen": "^3.0.0",
         "leaflet.markercluster": "^1.5.3",
         "mini-css-extract-plugin": "^2.6.1",
         "webpack": "^5.74.0",
         "webpack-cli": "^5.1.4"
```

### Comparing `betty-0.3.2/betty/extension/maps/assets/betty.extension.npm._Npm/src/webpack.config.js` & `betty-0.3.3/betty/extension/maps/assets/betty.extension.npm._Npm/src/webpack.config.js`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/nginx/__init__.py` & `betty-0.3.3/betty/extension/nginx/__init__.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/nginx/artifact.py` & `betty-0.3.3/betty/extension/nginx/artifact.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/nginx/assets/content_negotiation.lua` & `betty-0.3.3/betty/extension/nginx/assets/content_negotiation.lua`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/nginx/assets/nginx.conf.j2` & `betty-0.3.3/betty/extension/nginx/assets/nginx.conf.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/nginx/docker.py` & `betty-0.3.3/betty/extension/nginx/docker.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/nginx/serve.py` & `betty-0.3.3/betty/extension/nginx/serve.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,73 +1,76 @@
 """
 Integrate the nginx extension with Betty's Serve API.
 """
 import logging
+from contextlib import AsyncExitStack
 from pathlib import Path
-from typing import Any
 
 import docker
-from aiofiles.tempfile import TemporaryDirectory, AiofilesContextManagerTempDir
+from aiofiles.tempfile import TemporaryDirectory
 from docker.errors import DockerException
 
 from betty.app import App
 from betty.extension.nginx.artifact import generate_dockerfile_file, generate_configuration_file
 from betty.extension.nginx.docker import Container
 from betty.project import Project
-from betty.serve import NoPublicUrlBecauseServerNotStartedError, AppServer
+from betty.serve import NoPublicUrlBecauseServerNotStartedError, Server
 
 
-class DockerizedNginxServer(AppServer):
+class DockerizedNginxServer(Server):
     def __init__(self, app: App) -> None:
-        from betty.extension import Nginx
-
-        project = Project(ancestry=app.project.ancestry)
-        project.configuration.autowrite = False
-        project.configuration.configuration_file_path = app.project.configuration.configuration_file_path
-        project.configuration.update(app.project.configuration)
-        project.configuration.debug = True
-        app = App(app.configuration, project)
-        # Work around https://github.com/bartfeenstra/betty/issues/1056.
-        app.extensions[Nginx].configuration.https = False
-        super().__init__(app)
+        super().__init__(app.localizer)
+        self._app = app
+        self._exit_stack = AsyncExitStack()
         self._container: Container | None = None
-        self._output_directory: AiofilesContextManagerTempDir[None, Any, Any] | None = None
 
     async def start(self) -> None:
+        from betty.extension import Nginx
+
         await super().start()
         logging.getLogger(__name__).info('Starting a Dockerized nginx web server...')
-        self._output_directory = TemporaryDirectory()
-        output_directory_name = await self._output_directory.__aenter__()
-        nginx_configuration_file_path = Path(output_directory_name) / 'nginx.conf'
-        docker_directory_path = Path(output_directory_name)
+
+        output_directory_path_str = await self._exit_stack.enter_async_context(TemporaryDirectory())
+
+        isolated_project = Project(ancestry=self._app.project.ancestry)
+        isolated_project.configuration.autowrite = False
+        isolated_project.configuration.configuration_file_path = self._app.project.configuration.configuration_file_path
+        isolated_project.configuration.update(self._app.project.configuration)
+        isolated_project.configuration.debug = True
+
+        isolated_app = await self._exit_stack.enter_async_context(App.new_from_app(self._app, project=isolated_project))
+        await self._exit_stack.enter_async_context(isolated_app)
+        isolated_app.configuration.update(self._app.configuration)
+        # Work around https://github.com/bartfeenstra/betty/issues/1056.
+        isolated_app.extensions[Nginx].configuration.https = False
+
+        nginx_configuration_file_path = Path(output_directory_path_str) / 'nginx.conf'
+        docker_directory_path = Path(output_directory_path_str)
         dockerfile_file_path = docker_directory_path / 'Dockerfile'
 
         await generate_configuration_file(
-            self._app,
+            isolated_app,
             destination_file_path=nginx_configuration_file_path,
             https=False,
             www_directory_path='/var/www/betty',
         )
         await generate_dockerfile_file(
-            self._app,
+            isolated_app,
             destination_file_path=dockerfile_file_path,
         )
         self._container = Container(
-            self._app.project.configuration.www_directory_path,
+            isolated_app.project.configuration.www_directory_path,
             docker_directory_path,
             nginx_configuration_file_path,
         )
-        await self._container.start()
+        await self._exit_stack.enter_async_context(self._container)
         await self.assert_available()
 
     async def stop(self) -> None:
-        if self._container is not None:
-            await self._container.stop()
-        if self._output_directory is not None:
-            await self._output_directory.__aexit__(None, None, None)
+        await self._exit_stack.aclose()
 
     @property
     def public_url(self) -> str:
         if self._container is not None:
             return 'http://%s' % self._container.ip
         raise NoPublicUrlBecauseServerNotStartedError()
```

### Comparing `betty-0.3.2/betty/extension/npm/__init__.py` & `betty-0.3.3/betty/extension/npm/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 from subprocess import CalledProcessError
 from typing import Sequence
 
 from aiofiles.tempfile import TemporaryDirectory
 
 from betty.app.extension import Extension, discover_extension_types
 from betty.app.extension.requirement import Requirement, AnyRequirement, AllRequirements
-from betty.asyncio import wait
+from betty.asyncio import wait_to_thread
+from betty.cache.file import BinaryFileCache
 from betty.fs import iterfiles
 from betty.locale import Str, DEFAULT_LOCALIZER
 from betty.subprocess import run_process
 
 
 async def npm(
     arguments: Sequence[str],
@@ -57,15 +58,15 @@
     @classmethod
     def _unmet_summary(cls) -> Str:
         return Str._('`npm` is not available')
 
     @classmethod
     def check(cls) -> _NpmRequirement:
         try:
-            wait(npm(['--version']))
+            wait_to_thread(npm(['--version']))
             logging.getLogger(__name__).debug(cls._met_summary().localize(DEFAULT_LOCALIZER))
             return cls(True)
         except (CalledProcessError, FileNotFoundError):
             logging.getLogger(__name__).debug(cls._unmet_summary().localize(DEFAULT_LOCALIZER))
             return cls(False)
 
     def is_met(self) -> bool:
@@ -220,30 +221,30 @@
             working_directory_path,
             dirs_exist_ok=True,
         )
         async for file_path in iterfiles(working_directory_path):
             await self._app.renderer.render_file(file_path)
         await npm(['install', '--production'], cwd=working_directory_path)
 
-    def _get_cached_assets_build_directory_path(self, extension_type: type[_NpmBuilder & Extension]) -> Path:
-        path = self._app.cache.path / self.name() / extension_type.name()
+    def _get_assets_build_cache(self, extension_type: type[_NpmBuilder & Extension]) -> BinaryFileCache:
+        cache = self._app.binary_file_cache.with_scope(self.name()).with_scope(extension_type.name())
         if extension_type.npm_cache_scope() == _NpmBuilderCacheScope.PROJECT:
-            path /= self.app.project.name
-        return path
+            cache = cache.with_scope(self.app.project.name)
+        return cache
 
     async def ensure_assets(self, extension: _NpmBuilder & Extension) -> Path:
         assets_build_directory_paths = [
             _get_assets_build_directory_path(type(extension)),
-            self._get_cached_assets_build_directory_path(type(extension)),
+            self._get_assets_build_cache(type(extension)).path,
         ]
         for assets_build_directory_path in assets_build_directory_paths:
             if is_assets_build_directory_path(assets_build_directory_path):
                 return assets_build_directory_path
 
         if self._npm_requirement:
             self._npm_requirement.assert_met()
-        return await self._build_cached_assets(extension)
+        return (await self._build_cached_assets(extension)).path
 
-    async def _build_cached_assets(self, extension: _NpmBuilder & Extension) -> Path:
-        assets_directory_path = self._get_cached_assets_build_directory_path(type(extension))
-        await _build_assets_to_directory_path(extension, assets_directory_path)
-        return assets_directory_path
+    async def _build_cached_assets(self, extension: _NpmBuilder & Extension) -> BinaryFileCache:
+        cache = self._get_assets_build_cache(type(extension))
+        await _build_assets_to_directory_path(extension, cache.path)
+        return cache
```

### Comparing `betty-0.3.2/betty/extension/privatizer/__init__.py` & `betty-0.3.3/betty/extension/privatizer/__init__.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/trees/__init__.py` & `betty-0.3.3/betty/extension/trees/__init__.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/trees/assets/betty.extension.npm._Npm/src/trees.js` & `betty-0.3.3/betty/extension/trees/assets/betty.extension.npm._Npm/src/trees.js`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/trees/assets/betty.extension.npm._Npm/src/webpack.config.js` & `betty-0.3.3/betty/extension/trees/assets/betty.extension.npm._Npm/src/webpack.config.js`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/extension/trees/assets/public/localized/people.json.j2` & `betty-0.3.3/betty/extension/trees/assets/public/localized/people.json.j2`

 * *Files 2% similar despite different names*

```diff
@@ -12,8 +12,8 @@
             'url': person | url,
             'parentIds': person.parents | map(attribute='id') | list,
             'childIds': person.children | map(attribute='id') | list,
             'private': person.private,
         }
     }) %}
 {% endfor %}
-{{ ns.people | json }}
+{{ ns.people | json | safe }}
```

### Comparing `betty-0.3.2/betty/extension/wikipedia/__init__.py` & `betty-0.3.3/betty/extension/wikipedia/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,19 @@
     async def post_load(self) -> None:
         populator = wikipedia._Populator(self.app, self._retriever)
         await populator.populate()
 
     @property
     def _retriever(self) -> wikipedia._Retriever:
         if self.__retriever is None:
-            self.__retriever = wikipedia._Retriever(self.app.http_client, self._app.cache.path / self.name())
+            self.__retriever = wikipedia._Retriever(
+                self.app.http_client,
+                self._app.cache,
+                self._app.binary_file_cache.with_scope(self.name()),
+            )
         return self.__retriever
 
     @_retriever.deleter
     def _retriever(self) -> None:
         self.__retriever = None
 
     @property
```

### Comparing `betty-0.3.2/betty/fs.py` & `betty-0.3.3/betty/fs.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,14 +26,21 @@
 ASSETS_DIRECTORY_PATH = ROOT_DIRECTORY_PATH / 'betty' / 'assets'
 
 
 HOME_DIRECTORY_PATH = Path.home() / '.betty'
 
 
 CACHE_DIRECTORY_PATH = HOME_DIRECTORY_PATH / 'cache'
+"""
+Define the path to the cache directory.
+
+.. deprecated:: 0.3.3
+   This constant is deprecated as of Betty 0.3.3, and will be removed in Betty 0.4.x.
+   Instead, use :py:class:`betty.cache.file.BinaryFileCache`.
+"""
 
 
 async def iterfiles(path: Path) -> AsyncIterable[Path]:
     """
     Recursively iterate over any files found in a directory.
     """
     for dir_path, _, filenames in os.walk(str(path)):
```

### Comparing `betty-0.3.2/betty/functools.py` & `betty-0.3.3/betty/functools.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/generate.py` & `betty-0.3.3/betty/generate.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -16,23 +16,23 @@
 from typing import cast, AsyncContextManager, ParamSpec, Callable, Awaitable, Sequence
 
 import aiofiles
 from aiofiles.os import makedirs
 from aiofiles.threadpool.text import AsyncTextIOWrapper
 
 from betty.app import App
+from betty.job import Context
 from betty.json.linked_data import LinkedDataDumpable
 from betty.json.schema import Schema
 from betty.locale import get_display_name
 from betty.model import get_entity_type_name, UserFacingEntity, Entity, GeneratedEntityId
 from betty.model.ancestry import is_public
 from betty.openapi import Specification
 from betty.serde.dump import DictDump, Dump
 from betty.string import camel_case_to_kebab_case, camel_case_to_snake_case, upper_camel_case_to_lower_camel_case
-from betty.job import Context
 from betty.warnings import deprecated
 
 
 @deprecated('This function is deprecated as of Betty 0.3.2, and will be removed in Betty 0.4.x. Instead, use `logging.logging.getLogger(__name__)`.')
 def getLogger() -> logging.Logger:
     """
     Get the site generation logger.
@@ -58,18 +58,18 @@
 async def generate(app: App) -> None:
     """
     Generate a new site.
     """
     logger = logging.getLogger(__name__)
     job_context = GenerationContext(app)
 
+    logger.info(app.localizer._('Generating your site to {output_directory}.').format(output_directory=app.project.configuration.output_directory_path))
     with suppress(FileNotFoundError):
         await asyncio.to_thread(shutil.rmtree, app.project.configuration.output_directory_path)
     await makedirs(app.project.configuration.output_directory_path, exist_ok=True)
-    logger.info(app.localizer._('Generating your site to {output_directory}.').format(output_directory=app.project.configuration.output_directory_path))
 
     # The static public assets may be overridden depending on the number of locales rendered, so ensure they are
     # generated before anything else.
     await _generate_static_public(app, job_context)
 
     jobs = [job async for job in _run_jobs(app, job_context)]
     log_job = create_task(_log_jobs_forever(app, jobs))
@@ -97,16 +97,16 @@
         completed_job_percentage=floor(completed_job_count / (total_job_count / 100)),
     ))
 
 
 async def _log_jobs_forever(app: App, jobs: Sequence[Task[None]]) -> None:
     with suppress(CancelledError):
         while True:
-            await sleep(5)
             await _log_jobs(app, jobs)
+            await sleep(5)
 
 
 _JobP = ParamSpec('_JobP')
 
 
 def _run_job(semaphore: Semaphore, f: Callable[_JobP, Awaitable[None]], *args: _JobP.args, **kwargs: _JobP.kwargs) -> Task[None]:
     async def _job():
```

### Comparing `betty-0.3.2/betty/gramps/loader.py` & `betty-0.3.3/betty/gramps/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -583,15 +583,15 @@
         except KeyError:
             event_type = UnknownEventType
             getLogger(__name__).warning(self._localizer._(
                 'Betty is unfamiliar with Gramps event "{event_id}"\'s type of "{gramps_event_type}". The event was imported, but its type was set to "{betty_event_type}".',
             ).format(
                 event_id=event_id,
                 gramps_event_type=gramps_type,
-                betty_event_type=event_type.label(),
+                betty_event_type=event_type.label().localize(self._localizer),
             ))
 
         event = Event(
             id=event_id,
             event_type=event_type,
         )
 
@@ -765,17 +765,17 @@
         if privacy_value == 'public':
             entity.public = True
             return
         getLogger(__name__).warning(self._localizer._(
             'The betty:privacy Gramps attribute must have a value of "public" or "private", but "{privacy_value}" was given for {entity_type} {entity_id} ({entity_label}), which was ignored.',
         ).format(
             privacy_value=privacy_value,
-            entity_type=entity.entity_type_label(),
+            entity_type=entity.entity_type_label().localize(self._localizer),
             entity_id=entity.id,
-            entity_label=entity.label,
+            entity_label=entity.label.localize(self._localizer),
         ))
 
     def _load_attribute(self, name: str, element: ElementTree.Element, tag: str) -> str | None:
         prefixes = ['betty']
         if self._project is not None and self._project.configuration.name is not None:
             prefixes.insert(0, f'betty-{self._project.configuration.name}')
         for prefix in prefixes:
```

### Comparing `betty-0.3.2/betty/gui/__init__.py` & `betty-0.3.3/betty/gui/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Provide the Graphical User Interface (GUI) for Betty Desktop."""
 from __future__ import annotations
 
 import pickle
-from typing import Any, TypeVar
+from collections.abc import AsyncIterator
+from contextlib import asynccontextmanager
+from typing import Any, TypeVar, Self
 
-from PyQt6.QtCore import pyqtSlot, QObject
+from PyQt6.QtCore import pyqtSlot, QObject, QCoreApplication
 from PyQt6.QtGui import QPalette
 from PyQt6.QtWidgets import QApplication, QWidget
 
 from betty.app import App
 from betty.gui.error import ExceptionError, _UnexpectedExceptionError
 from betty.locale import Str
 from betty.serde.format import FormatRepository
@@ -52,14 +54,20 @@
     """
     widget.setProperty('invalid', 'true')
     widget.setStyle(widget.style())
     widget.setToolTip(reason)
 
 
 class BettyApplication(QApplication):
+    def __init__(self, *args: Any, **kwargs: Any):
+        super().__init__(*args, **kwargs)
+        self._app: App | None = None
+        self.setApplicationName('Betty')
+        self.setStyleSheet(self._stylesheet())
+
     def _is_dark_mode(self) -> bool:
         palette = self.palette()
         window_lightness = palette.color(QPalette.ColorRole.Window).lightness()
         window_text_lightness = palette.color(QPalette.ColorRole.WindowText).lightness()
         return window_lightness < window_text_lightness
 
     def _stylesheet(self) -> str:
@@ -120,35 +128,29 @@
             }}
 
             _WelcomeAction {{
                 padding: 10px;
             }}
             """
 
-    def __init__(self, *args: Any, app: App, **kwargs: Any):
-        super().__init__(*args, **kwargs)
-        self.setApplicationName('Betty')
-        self.setStyleSheet(self._stylesheet())
-        self._app = app
-
     @pyqtSlot(
         type,
         bytes,
         QObject,
         bool,
     )
     def _show_user_facing_error(
         self,
         error_type: type[Exception],
         pickled_error_message: bytes,
         parent: QObject,
         close_parent: bool,
     ) -> None:
         error_message = pickle.loads(pickled_error_message)
-        window = ExceptionError(self._app, error_message, error_type, parent=parent, close_parent=close_parent)
+        window = ExceptionError(self.app, error_message, error_type, parent=parent, close_parent=close_parent)
         window.show()
 
     @pyqtSlot(
         type,
         str,
         str,
         QObject,
@@ -158,9 +160,29 @@
         self,
         error_type: type[Exception],
         error_message: str,
         error_traceback: str,
         parent: QObject,
         close_parent: bool,
     ) -> None:
-        window = _UnexpectedExceptionError(self._app, error_type, error_message, error_traceback, parent=parent, close_parent=close_parent)
+        window = _UnexpectedExceptionError(self.app, error_type, error_message, error_traceback, parent=parent, close_parent=close_parent)
         window.show()
+
+    @classmethod
+    def instance(cls) -> Self:
+        qapp = QCoreApplication.instance()
+        assert isinstance(qapp, cls)
+        return qapp
+
+    @asynccontextmanager
+    async def with_app(self, app: App) -> AsyncIterator[Self]:
+        if self._app is not None:
+            raise RuntimeError(f'This {type(self)} already has an {App}.')
+        self._app = app
+        yield self
+        self._app = None
+
+    @property
+    def app(self) -> App:
+        if self._app is None:
+            raise RuntimeError(f'This {type(self)} does not have an {App} yet.')
+        return self._app
```

### Comparing `betty-0.3.2/betty/gui/app.py` & `betty-0.3.3/betty/gui/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from PyQt6.QtCore import Qt, QCoreApplication, QObject
 from PyQt6.QtGui import QIcon, QAction
 from PyQt6.QtWidgets import QFormLayout, QWidget, QVBoxLayout, QHBoxLayout, QFileDialog, QPushButton
 
 from betty import about
 from betty.about import report
 from betty.app import App
-from betty.asyncio import sync, wait
+from betty.asyncio import wait_to_thread
 from betty.gui import get_configuration_file_filter
 from betty.gui.error import ExceptionCatcher
 from betty.gui.locale import TranslationsLocaleCollector
 from betty.gui.serve import ServeDemoWindow, ServeDocsWindow
 from betty.gui.text import Text
 from betty.gui.window import BettyMainWindow
 from betty.locale import Str, Localizable
@@ -174,15 +174,15 @@
                 self,
                 self._app.localizer._('Open your project from...'),
                 '',
                 get_configuration_file_filter().localize(self._app.localizer),
             )
             if not configuration_file_path_str:
                 return
-            wait(self._app.project.configuration.read(Path(configuration_file_path_str)))
+            wait_to_thread(self._app.project.configuration.read(Path(configuration_file_path_str)))
             project_window = ProjectWindow(self._app)
             project_window.show()
             self.close()
 
     def new_project(self) -> None:
         with ExceptionCatcher(self):
             from betty.gui.project import ProjectWindow
@@ -192,26 +192,28 @@
                 self._app.localizer._('Save your new project to...'),
                 '',
                 get_configuration_file_filter().localize(self._app.localizer),
             )
             if not configuration_file_path_str:
                 return
             configuration = ProjectConfiguration()
-            wait(configuration.write(Path(configuration_file_path_str)))
+            wait_to_thread(configuration.write(Path(configuration_file_path_str)))
             project_window = ProjectWindow(self._app)
             project_window.show()
             self.close()
 
     def _demo(self) -> None:
         with ExceptionCatcher(self):
             serve_window = ServeDemoWindow(self._app, parent=self)
             serve_window.show()
 
-    @sync
-    async def clear_caches(self) -> None:
+    def clear_caches(self) -> None:
+        wait_to_thread(self._clear_caches())
+
+    async def _clear_caches(self) -> None:
         async with ExceptionCatcher(self):
             await self._app.cache.clear()
 
     def open_application_configuration(self) -> None:
         with ExceptionCatcher(self):
             window = ApplicationConfiguration(self._app, parent=self)
             window.show()
@@ -311,15 +313,15 @@
         self._label.setAlignment(Qt.AlignmentFlag.AlignCenter)
         self.setCentralWidget(self._label)
 
     def _set_translatables(self) -> None:
         super()._set_translatables()
         self._label.setText(''.join(map(lambda x: '<p>%s</p>' % x, [
             self._app.localizer._('Version: {version}').format(
-                version=wait(about.version_label()),
+                version=wait_to_thread(about.version_label()),
             ),
             self._app.localizer._('Copyright 2019-{year} Bart Feenstra & contributors. Betty is made available to you under the <a href="https://www.gnu.org/licenses/gpl-3.0.en.html">GNU General Public License, Version 3</a> (GPLv3).').format(
                 year=datetime.now().year,
             ),
             self._app.localizer._('Follow Betty on <a href="https://twitter.com/Betty_Project">Twitter</a> and <a href="https://github.com/bartfeenstra/betty">Github</a>.'),
         ])))
```

### Comparing `betty-0.3.2/betty/gui/error.py` & `betty-0.3.3/betty/gui/error.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,14 +154,17 @@
         parent: QObject,
         close_parent: bool = False,
     ):
         super().__init__(app, message, parent=parent, close_parent=close_parent)
         self.error_type = error_type
 
 
+ExceptionErrorT = TypeVar('ExceptionErrorT', bound=ExceptionError)
+
+
 class _UnexpectedExceptionError(ExceptionError):
     def __init__(
         self,
         app: App,
         error_type: type[Exception],
         error_message: str,
         error_traceback: str,
```

### Comparing `betty-0.3.2/betty/gui/locale.py` & `betty-0.3.3/betty/gui/locale.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from typing import Any
 
 from PyQt6 import QtGui
 from PyQt6.QtWidgets import QComboBox, QLabel, QWidget
 
 from betty.app import App
-from betty.asyncio import wait
+from betty.asyncio import wait_to_thread
 from betty.gui.text import Caption
 from betty.locale import negotiate_locale, get_display_name
 
 
 class LocalizedObject:
     def __init__(self, app: App, *args: Any, **kwargs: Any):
         super().__init__(*args, **kwargs)
@@ -83,15 +83,15 @@
                 list(localizers.locales),
             )
             if translations_locale is None:
                 self._configuration_locale_caption.setText(localizer._('There are no translations for {locale_name}.').format(
                     locale_name=get_display_name(locale, localizer.locale),
                 ))
             else:
-                negotiated_locale_translations_coverage = wait(localizers.coverage(translations_locale))
+                negotiated_locale_translations_coverage = wait_to_thread(localizers.coverage(translations_locale))
                 if negotiated_locale_translations_coverage[1] == 0:
                     negotiated_locale_translations_coverage_percentage = 0
                 else:
                     negotiated_locale_translations_coverage_percentage = round(100 / (negotiated_locale_translations_coverage[1] / negotiated_locale_translations_coverage[0]))
                 self._configuration_locale_caption.setText(localizer._('The translations for {locale_name} are {coverage_percentage}%% complete.').format(
                     locale_name=get_display_name(translations_locale, localizer.locale),
                     coverage_percentage=round(negotiated_locale_translations_coverage_percentage)
```

### Comparing `betty-0.3.2/betty/gui/logging.py` & `betty-0.3.3/betty/gui/logging.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/gui/model.py` & `betty-0.3.3/betty/gui/model.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/gui/project.py` & `betty-0.3.3/betty/gui/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     QGridLayout, QCheckBox, QFormLayout, QLabel, QLineEdit, QButtonGroup, QRadioButton, QFrame, QScrollArea, QSizePolicy
 from babel import Locale
 from babel.localedata import locale_identifiers
 
 from betty import load, generate
 from betty.app import App
 from betty.app.extension import UserFacingExtension
-from betty.asyncio import sync, wait
+from betty.asyncio import wait_to_thread
 from betty.gui import get_configuration_file_filter, GuiBuilder, mark_invalid, mark_valid
 from betty.gui.app import BettyPrimaryWindow
 from betty.gui.error import ExceptionCatcher
 from betty.gui.locale import LocalizedObject
 from betty.gui.locale import TranslationsLocaleCollector
 from betty.gui.logging import LogRecordViewerHandler, LogRecordViewer
 from betty.gui.serve import ServeProjectWindow
@@ -588,15 +588,15 @@
         with ExceptionCatcher(self):
             configuration_file_path_str, __ = QFileDialog.getSaveFileName(
                 self,
                 self._app.localizer._('Save your project to...'),
                 '',
                 get_configuration_file_filter().localize(self._app.localizer),
             )
-            wait(self._app.project.configuration.write(Path(configuration_file_path_str)))
+            wait_to_thread(self._app.project.configuration.write(Path(configuration_file_path_str)))
 
     def _generate(self) -> None:
         with ExceptionCatcher(self):
             generate_window = _GenerateWindow(self._app, parent=self)
             generate_window.show()
 
     def _serve(self) -> None:
@@ -608,23 +608,25 @@
 class _GenerateThread(QThread):
     def __init__(self, project: Project, generate_window: _GenerateWindow):
         super().__init__()
         self._project = project
         self._generate_window = generate_window
         self._task: Task[None] | None = None
 
-    @sync
-    async def run(self) -> None:
+    def run(self) -> None:
+        asyncio.run(self._run())
+
+    async def _run(self) -> None:
         with suppress(CancelledError):
             self._task = asyncio.create_task(self._generate())
             await self._task
 
     async def _generate(self) -> None:
         with ExceptionCatcher(self._generate_window, close_parent=True):
-            async with App(project=self._project) as app:
+            async with App.new_from_environment(project=self._project) as app:
                 await load.load(app)
                 await generate.generate(app)
 
     def cancel(self) -> None:
         if self._task:
             self._task.cancel()
```

### Comparing `betty-0.3.2/betty/gui/serve.py` & `betty-0.3.3/betty/gui/serve.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """
 Integrate Betty's Graphical User Interface with the Serve API.
 """
 from __future__ import annotations
 
+import asyncio
 from typing import Any
 
 from PyQt6.QtCore import Qt, QThread, pyqtSignal, QObject
 from PyQt6.QtWidgets import QVBoxLayout, QWidget, QPushButton
 
-from betty import documentation, fs
+from betty import documentation
 from betty.app import App
-from betty.asyncio import sync
+from betty.asyncio import wait_to_thread
 from betty.extension import demo
 from betty.gui.error import ExceptionCatcher
 from betty.gui.text import Text
 from betty.gui.window import BettyMainWindow
 from betty.locale import Str, Localizable
 from betty.project import Project
 from betty.serve import Server, AppServer
@@ -30,25 +31,26 @@
         self._serve_window = serve_window
         self._app: App | None = None
 
     @property
     def server(self) -> Server:
         return self._server
 
-    @sync
-    async def run(self) -> None:
+    def run(self) -> None:
+        asyncio.run(self._run())
+
+    async def _run(self) -> None:
         with ExceptionCatcher(self._serve_window, close_parent=True):
-            async with App(project=self._project) as self._app:
+            async with App.new_from_environment(project=self._project) as self._app:
                 await self._server.start()
                 self.server_started.emit()
                 await self._server.show()
 
-    @sync
-    async def stop(self) -> None:
-        await self._server.stop()
+    def stop(self) -> None:
+        wait_to_thread(self._server.stop())
 
 
 class _ServeWindow(BettyMainWindow):
     window_width = 500
     window_height = 100
 
     def __init__(
@@ -137,30 +139,30 @@
         return self._app.localizer._('You can now view your site at <a href="{url}">{url}</a>.').format(
             url=self._thread.server.public_url,
         )
 
 
 class ServeDemoWindow(_ServeWindow):
     def _server(self) -> Server:
-        return demo.DemoServer()
+        return demo.DemoServer(app=self._app)
 
     def _build_instruction(self) -> str:
         return self._app.localizer._('You can now view a Betty demonstration site at <a href="{url}">{url}</a>.').format(
             url=self._thread.server.public_url,
         )
 
     @property
     def window_title(self) -> Localizable:
         return Str._('Serving the Betty demo...')
 
 
 class ServeDocsWindow(_ServeWindow):
     def _server(self) -> Server:
         return documentation.DocumentationServer(
-            fs.CACHE_DIRECTORY_PATH,
+            self._app.binary_file_cache.path,
             localizer=self._app.localizer,
         )
 
     def _build_instruction(self) -> str:
         return self._app.localizer._('You can now view the documentation at <a href="{url}">{url}</a>.').format(
             url=self._thread.server.public_url,
         )
```

### Comparing `betty-0.3.2/betty/gui/text.py` & `betty-0.3.3/betty/gui/text.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/gui/window.py` & `betty-0.3.3/betty/gui/window.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/importlib.py` & `betty-0.3.3/betty/importlib.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/jinja2/__init__.py` & `betty-0.3.3/betty/jinja2/__init__.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/jinja2/filter.py` & `betty-0.3.3/betty/jinja2/filter.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Provide Betty's default Jinja2 filters.
 """
 from __future__ import annotations
 
 import json as stdjson
 import re
 import warnings
-from asyncio import get_running_loop
+from asyncio import get_running_loop, run
 from base64 import b64encode
 from collections.abc import Awaitable
 from contextlib import suppress
 from io import BytesIO
 from pathlib import Path
 from typing import Callable, Iterable, Any, Iterator, TypeVar, AsyncIterator
 from urllib.parse import quote
@@ -27,15 +27,14 @@
 from jinja2.filters import prepare_map, make_attrgetter
 from jinja2.nodes import EvalContext
 from jinja2.runtime import Context, Macro
 from markupsafe import Markup, escape
 from pdf2image.pdf2image import convert_from_path
 
 from betty import _resizeimage
-from betty.asyncio import sync
 from betty.fs import hashfile
 from betty.functools import walk
 from betty.locale import negotiate_localizeds, Localized, Datey, negotiate_locale, Localey, get_data, Localizable
 from betty.media_type import MediaType
 from betty.model import get_entity_type_name
 from betty.model.ancestry import File, Dated
 from betty.os import link_or_copy
@@ -202,15 +201,23 @@
     :return: The public path to the preprocessed file. This can be used on a web page.
     """
     from betty.jinja2 import context_app, context_job_context
 
     app = context_app(context)
     job_context = context_job_context(context)
 
-    if job_context is None or job_context.claim(f'filter_file:{file.id}'):
+    execute_filter = True
+    if job_context:
+        job_cache_item_id = f'filter_file:{file.id}'
+        async with job_context.cache.getset(job_cache_item_id, wait=False) as (cache_item, setter):
+            if cache_item is None and setter is not None:
+                await setter(None)
+            else:
+                execute_filter = False
+    if execute_filter:
         file_destination_path = app.project.configuration.www_directory_path / 'file' / file.id / 'file' / file.path.name
         await makedirs(file_destination_path.parent, exist_ok=True)
         await link_or_copy(file.path, file_destination_path)
 
     return f'/file/{quote(file.id)}/file/{quote(file.path.name)}'
 
 
@@ -255,63 +262,90 @@
             image_loader = _load_image_application_pdf
             destination_name += '.' + 'jpg'
         else:
             raise ValueError(f'Cannot convert a file of media type "{file.media_type}" to an image.')
     else:
         raise ValueError('Cannot convert a file without a media type to an image.')
 
-    cache_item_id = f'filter_image:{hashfile(file.path)}:{"" if width is None else width}:{"" if height is None else height}'
-    if job_context is None or job_context.claim(cache_item_id):
+    cache_item_id = f'{hashfile(file.path)}:{"" if width is None else width}:{"" if height is None else height}'
+    execute_filter = True
+    if job_context:
+        async with job_context.cache.with_scope('filter_image').getset(cache_item_id, wait=False) as (cache_item, setter):
+            if cache_item is None and setter is not None:
+                await setter(True)
+            else:
+                execute_filter = False
+    if execute_filter:
         loop = get_running_loop()
         await loop.run_in_executor(
             app.process_pool,
             _execute_filter_image,
             image_loader,
             file.path,
             file.media_type,
-            app.cache.path / 'image' / filter_base64(cache_item_id),
+            app.binary_file_cache.with_scope('image').cache_item_file_path(cache_item_id),
             file_directory_path,
             destination_name,
             width,
             height,
         )
-
     destination_public_path = f'/file/{quote(destination_name)}'
 
     return destination_public_path
 
 
 async def _load_image_image(
     file_path: Path,
     media_type: MediaType,
-) -> Image:
+) -> Image.Image:
     # We want to read the image asynchronously and prevent Pillow from keeping too many file
     # descriptors open simultaneously, so we read the image ourselves and store the contents
     # in a synchronous file object.
     async with aiofiles.open(file_path, 'rb') as f:
         image_f = BytesIO(await f.read())
     # Ignore warnings about decompression bombs, because we know where the files come from.
     with warnings.catch_warnings(action='ignore', category=DecompressionBombWarning):
         image = Image.open(image_f, formats=[media_type.subtype])
     return image
 
 
 async def _load_image_application_pdf(
     file_path: Path,
     media_type: MediaType,
-) -> Image:
+) -> Image.Image:
     # Ignore warnings about decompression bombs, because we know where the files come from.
     with warnings.catch_warnings(action='ignore', category=DecompressionBombWarning):
         image = convert_from_path(file_path, fmt='jpeg')[0]
     return image
 
 
-@sync
-async def _execute_filter_image(
-    image_loader: Callable[[Path, MediaType], Awaitable[Image]],
+def _execute_filter_image(
+    image_loader: Callable[[Path, MediaType], Awaitable[Image.Image]],
+    file_path: Path,
+    media_type: MediaType,
+    cache_item_file_path: Path,
+    destination_directory_path: Path,
+    destination_name: str,
+    width: int | None,
+    height: int | None,
+) -> None:
+    run(__execute_filter_image(
+        image_loader,
+        file_path,
+        media_type,
+        cache_item_file_path,
+        destination_directory_path,
+        destination_name,
+        width,
+        height,
+    ))
+
+
+async def __execute_filter_image(
+    image_loader: Callable[[Path, MediaType], Awaitable[Image.Image]],
     file_path: Path,
     media_type: MediaType,
     cache_item_file_path: Path,
     destination_directory_path: Path,
     destination_name: str,
     width: int | None,
     height: int | None,
@@ -335,18 +369,18 @@
         finally:
             image.close()
             del image
         await link_or_copy(cache_item_file_path, destination_file_path)
 
 
 async def _execute_filter_image_convert(
-    image: Image,
+    image: Image.Image,
     width: int | None,
     height: int | None,
-) -> Image:
+) -> Image.Image:
     if width is not None and height is not None:
         return _resizeimage.resize_cover(image, (width, height))
     if width is not None:
         return _resizeimage.resize_width(image, width)
     if height is not None:
         return _resizeimage.resize_height(image, height)
     raise ValueError('Width and height cannot both be None.')
```

### Comparing `betty-0.3.2/betty/jinja2/test.py` & `betty-0.3.3/betty/jinja2/test.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/json/linked_data.py` & `betty-0.3.3/betty/json/linked_data.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/json/schema.py` & `betty-0.3.3/betty/json/schema.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/load.py` & `betty-0.3.3/betty/load.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/locale.py` & `betty-0.3.3/betty/locale.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,27 +26,27 @@
 from aiofiles.ospath import exists
 from babel import dates, Locale
 from babel.messages.frontend import CommandLineInterface
 from langcodes import Language
 from polib import pofile
 
 from betty import fs
-from betty.asyncio import wait
-from betty.fs import hashfile, FileSystem, ASSETS_DIRECTORY_PATH, ROOT_DIRECTORY_PATH
+from betty.asyncio import wait_to_thread
+from betty.fs import hashfile, FileSystem, ROOT_DIRECTORY_PATH
 from betty.json.linked_data import LinkedDataDumpable, dump_context, add_json_ld
 from betty.json.schema import ref_locale, add_property
 from betty.serde.dump import DictDump, Dump, dump_default
 
 if TYPE_CHECKING:
     from betty.app import App
 
 
 DEFAULT_LOCALE = 'en-US'
 
-_LOCALE_DIRECTORY_PATH = ASSETS_DIRECTORY_PATH / 'locale'
+_LOCALE_DIRECTORY_PATH = fs.ASSETS_DIRECTORY_PATH / 'locale'
 
 
 class LocaleNotFoundError(RuntimeError):
     def __init__(self, locale: str) -> None:
         super().__init__(f'Cannot find locale "{locale}"')
         self.locale = locale
 
@@ -669,15 +669,15 @@
             return await self._build_translation(locale)
 
     def __getitem__(self, locale: Localey) -> Localizer:
         locale = to_locale(locale)
         try:
             return self._localizers[locale]
         except KeyError:
-            return wait(self._build_translation(locale))
+            return wait_to_thread(self._build_translation(locale))
 
     async def get_negotiated(self, *preferred_locales: str) -> Localizer:
         preferred_locales = (*preferred_locales, DEFAULT_LOCALE)
         negotiated_locale = negotiate_locale(
             preferred_locales,
             [
                 str(get_data(locale))
@@ -760,15 +760,18 @@
 
 class Localizable:
     def localize(self, localizer: Localizer) -> str:
         raise NotImplementedError
 
     def __str__(self) -> str:
         localized = self.localize(DEFAULT_LOCALIZER)
-        warn(f'{type(self)} ("{localized}") SHOULD NOT be cast to a string. Instead, call {type(self)}.localize() to ensure it is always formatted in the desired locale.')
+        warn(
+            f'{type(self)} ("{localized}") SHOULD NOT be cast to a string. Instead, call {type(self)}.localize() to ensure it is always formatted in the desired locale.',
+            stacklevel=2,
+        )
         return localized
 
 
 class Str(Localizable):
     def _localize_format_kwargs(self, localizer: Localizer, **format_kwargs: str | Localizable) -> dict[str, str]:
         return {
             key: value.localize(localizer) if isinstance(value, Localizable) else value
@@ -908,26 +911,26 @@
 
         locale_data = get_data(locale)
         CommandLineInterface().run([
             '',
             'init',
             '--no-wrap',
             '-i',
-            str(ASSETS_DIRECTORY_PATH / 'betty.pot'),
+            str(fs.ASSETS_DIRECTORY_PATH / 'betty.pot'),
             '-o',
             str(po_file_path),
             '-l',
             str(locale_data),
             '-D',
             'betty',
         ])
         logging.getLogger(__name__).info(f'Translations for {locale} initialized at {po_file_path}.')
 
 
-async def update_translations(_output_assets_directory_path: Path = ASSETS_DIRECTORY_PATH) -> None:
+async def update_translations(_output_assets_directory_path: Path = fs.ASSETS_DIRECTORY_PATH) -> None:
     """
     Update all existing translations based on changes in translatable strings.
     """
     source_paths = glob.glob('betty/*')
     # Remove the tests directory from the extraction,
     # or we'll be seeing some unusual additions to the translations.
     source_paths.remove(str(Path('betty') / 'tests'))
@@ -947,15 +950,15 @@
                 '--project',
                 'Betty',
                 '--copyright-holder',
                 'Bart Feenstra & contributors',
                 *source_paths,
             ])
             for po_file_path_str in glob.glob('betty/assets/locale/*/betty.po'):
-                po_file_path = (_output_assets_directory_path / (ROOT_DIRECTORY_PATH / po_file_path_str).relative_to(ASSETS_DIRECTORY_PATH)).resolve()
+                po_file_path = (_output_assets_directory_path / (ROOT_DIRECTORY_PATH / po_file_path_str).relative_to(fs.ASSETS_DIRECTORY_PATH)).resolve()
                 await makedirs(po_file_path.parent, exist_ok=True)
                 po_file_path.touch()
                 locale = po_file_path.parent.name
                 locale_data = get_data(locale)
                 CommandLineInterface().run([
                     '',
                     'update',
```

### Comparing `betty-0.3.2/betty/logging.py` & `betty-0.3.3/betty/logging.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/media_type.py` & `betty-0.3.3/betty/media_type.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/model/__init__.py` & `betty-0.3.3/betty/model/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,14 +187,16 @@
     """
 
     def __init__(self, entity_type: type):
         super().__init__(f'{entity_type.__module__}.{entity_type.__name__} is not an entity type class. Entity types must extend {Entity.__module__}.{Entity.__name__} directly.')
 
 
 class EntityCollection(Generic[TargetT]):
+    __slots__ = ()
+
     def __init__(self):
         super().__init__()
 
     def _on_add(self, *entities: TargetT & Entity) -> None:
         pass
 
     def _on_remove(self, *entities: TargetT & Entity) -> None:
@@ -685,14 +687,16 @@
     def finalize(cls, *owners: Entity) -> None:
         for owner in owners:
             for association in cls.get_all_associations(owner):
                 association.finalize(owner)
 
 
 class SingleTypeEntityCollection(Generic[TargetT], EntityCollection[TargetT]):
+    __slots__ = '_entities', '_target_type'
+
     def __init__(
         self,
         target_type: type[TargetT],
     ):
         super().__init__()
         self._entities: list[TargetT & Entity] = []
         self._target_type = target_type
@@ -791,14 +795,16 @@
         return False
 
 
 SingleTypeEntityCollectionT = TypeVar('SingleTypeEntityCollectionT', bound=SingleTypeEntityCollection[AssociateT])
 
 
 class MultipleTypesEntityCollection(Generic[TargetT], EntityCollection[TargetT]):
+    __slots__ = '_collections'
+
     def __init__(self):
         super().__init__()
         self._collections: dict[type[Entity], SingleTypeEntityCollection[Entity]] = {}
 
     @recursive_repr()
     def __repr__(self) -> str:
         return repr_instance(
@@ -920,14 +926,16 @@
         for collection in self._collections.values():
             collection.clear()
         if removed_entities:
             self._on_remove(*removed_entities)
 
 
 class _BidirectionalAssociateCollection(Generic[AssociateT, OwnerT], SingleTypeEntityCollection[AssociateT]):
+    __slots__ = '__owner', '_association'
+
     def __init__(
         self,
         owner: OwnerT & Entity,
         association: BidirectionalEntityTypeAssociation[OwnerT, AssociateT],
     ):
         super().__init__(association.associate_type)
         self._association = association
```

### Comparing `betty-0.3.2/betty/model/ancestry.py` & `betty-0.3.3/betty/model/ancestry.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 from enum import Enum
 from pathlib import Path
 from reprlib import recursive_repr
 from typing import Iterable, Any, TYPE_CHECKING
 from urllib.parse import quote
 
 from geopy import Point
-from typing_extensions import deprecated
 
 from betty.classtools import repr_instance
 from betty.json.linked_data import LinkedDataDumpable, dump_context, dump_link, add_json_ld
 from betty.json.schema import add_property, ref_json_schema
 from betty.locale import Localized, Datey, Str, Localizable, ref_datey
 from betty.media_type import MediaType
 from betty.model import many_to_many, Entity, one_to_many, many_to_one, many_to_one_to_many, \
     MultipleTypesEntityCollection, EntityCollection, UserFacingEntity, EntityTypeAssociationRegistry, \
     GeneratedEntityId, get_entity_type_name
 from betty.model.event_type import EventType, UnknownEventType
 from betty.serde.dump import DictDump, Dump, dump_default
 from betty.string import camel_case_to_kebab_case
+from betty.warnings import deprecated
 
 if TYPE_CHECKING:
     from betty.app import App
 
 
 class Privacy(Enum):
     PUBLIC = 1
```

### Comparing `betty-0.3.2/betty/model/event_type.py` & `betty-0.3.3/betty/model/event_type.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/openapi.py` & `betty-0.3.3/betty/openapi.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/os.py` & `betty-0.3.3/betty/os.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/privatizer.py` & `betty-0.3.3/betty/privatizer.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/project.py` & `betty-0.3.3/betty/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,14 +207,19 @@
         self._enabled = enabled
         self._dispatch_change()
 
     @property
     def extension_configuration(self) -> Configuration | None:
         return self._extension_configuration
 
+    def update(self, other: Self) -> None:
+        self._extension_type = other._extension_type
+        self._enabled = other._enabled
+        self._extension_configuration = other._extension_configuration
+
     @classmethod
     def load(
         cls,
         dump: Dump,
         configuration: Self | None = None,
     ) -> Self:
         asserter = Asserter()
```

### Comparing `betty-0.3.2/betty/render.py` & `betty-0.3.3/betty/render.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/serde/dump.py` & `betty-0.3.3/betty/serde/dump.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/serde/error.py` & `betty-0.3.3/betty/serde/error.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/serde/format.py` & `betty-0.3.3/betty/serde/format.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/serde/load.py` & `betty-0.3.3/betty/serde/load.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/serve.py` & `betty-0.3.3/betty/serve.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/sphinx/extension/replacements.py` & `betty-0.3.3/betty/sphinx/extension/replacements.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/string.py` & `betty-0.3.3/betty/string.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/subprocess.py` & `betty-0.3.3/betty/subprocess.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/url.py` & `betty-0.3.3/betty/url.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/warnings.py` & `betty-0.3.3/betty/warnings.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty/wikipedia.py` & `betty-0.3.3/betty/wikipedia.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 """
 from __future__ import annotations
 
 import asyncio
 import hashlib
 import json
 import logging
-import mimetypes
 import re
-from collections.abc import Sequence, MutableSequence
+from collections.abc import Sequence, MutableSequence, Callable, Awaitable
 from contextlib import suppress
-from os.path import getmtime
 from pathlib import Path
 from time import time
 from typing import cast, Any
 from urllib.parse import quote
 
-import aiofiles
 import aiohttp
+from aiohttp import ClientResponse
 from geopy import Point
 
 from betty.app import App
 from betty.asyncio import gather
+from betty.cache import Cache, CacheItemValueT
+from betty.cache.file import BinaryFileCache
 from betty.concurrent import RateLimiter
 from betty.functools import filter_suppress
 from betty.locale import Localized, negotiate_locale, to_locale, get_data, LocaleNotFoundError, Localey
 from betty.media_type import MediaType
 from betty.model.ancestry import Link, HasLinks, Place, File, HasFiles
 
 
@@ -102,65 +102,90 @@
         return self._title
 
     @property
     def wikimedia_commons_url(self) -> str:
         return self._wikimedia_commons_url
 
 
-class _Retriever:
+class _Fetcher:
+    _WIKIPEDIA_RATE_LIMIT = 200
+
     def __init__(
         self,
         http_client: aiohttp.ClientSession,
-        cache_directory_path: Path,
+        cache: Cache[str],
+        binary_file_cache: BinaryFileCache,
         # Default to seven days.
         ttl: int = 86400 * 7,
     ):
-        self._cache_directory_path = cache_directory_path
-        self._cache_directory_path.mkdir(exist_ok=True, parents=True)
+        self._cache = cache
+        self._binary_file_cache = binary_file_cache
         self._ttl = ttl
         self._http_client = http_client
-        self._rate_limiter = RateLimiter(200)
+        self._rate_limiter = RateLimiter(self._WIKIPEDIA_RATE_LIMIT)
         self._images: dict[str, Image | None] = {}
+        self._logger = logging.getLogger(__name__)
 
-    async def _request(self, url: str, extension: str | None = None) -> Any:
-        cache_file_path = self._cache_directory_path / hashlib.md5(url.encode("utf-8")).hexdigest()
-        if extension:
-            cache_file_path = cache_file_path.with_suffix(f'.{extension}')
-
-        response_data = None
-        with suppress(FileNotFoundError):
-            if getmtime(cache_file_path) + self._ttl > time():
-                async with aiofiles.open(cache_file_path, mode='r+b') as f:
-                    response_data = await f.read()
-
-        if response_data is None:
-            logger = logging.getLogger(__name__)
-            try:
-                logger.debug(f'Fetching {url}...')
+    async def _fetch(
+        self,
+        url: str,
+        cache: Cache[CacheItemValueT],
+        response_mapper: Callable[[ClientResponse], Awaitable[CacheItemValueT]],
+    ) -> tuple[CacheItemValueT, str]:
+        cache_item_id = hashlib.md5(url.encode('utf-8')).hexdigest()
+
+        response_data: CacheItemValueT | None = None
+        async with cache.getset(cache_item_id) as (cache_item, setter):
+            if cache_item and cache_item.modified + self._ttl > time():
+                response_data = await cache_item.value()
+            else:
                 async with self._rate_limiter:
-                    async with self._http_client.get(url) as response:
-                        response_data = await response.read()
-                async with aiofiles.open(cache_file_path, 'w+b') as f:
-                    await f.write(response_data)
-            except aiohttp.ClientError as error:
-                logger.warning(f'Could not successfully connect to Wikipedia at {url}: {error}')
-            except asyncio.TimeoutError:
-                logger.warning(f'Timeout when connecting to Wikipedia at {url}')
+                    self._logger.debug(f'Fetching {url}...')
+                    try:
+                        async with self._http_client.get(url) as response:
+                            response_data = await response_mapper(response)
+                    except aiohttp.ClientError as error:
+                        self._logger.warning(f'Could not successfully connect to {url}: {error}')
+                    except asyncio.TimeoutError:
+                        self._logger.warning(f'Timeout when connecting to {url}')
+                    else:
+                        await setter(response_data)
 
         if response_data is None:
-            try:
-                async with aiofiles.open(cache_file_path, mode='r+b') as f:
-                    response_data = await f.read()
-            except FileNotFoundError:
-                raise RetrievalError('Could neither fetch %s, nor find an old version in the cache.' % url)
+            if cache_item:
+                response_data = await cache_item.value()
+            else:
+                raise RetrievalError(f'Could neither fetch {url}, nor find an old version in the cache.')
+
+        return response_data, cache_item_id
 
+    async def fetch(self, url: str) -> str:
+        response_data, _ = await self._fetch(url, self._cache, ClientResponse.text)
         return response_data
 
+    async def fetch_file(self, url: str) -> Path:
+        _, cache_item_id = await self._fetch(url, self._binary_file_cache, ClientResponse.read)
+        return self._binary_file_cache.cache_item_file_path(cache_item_id)
+
+
+class _Retriever:
+    def __init__(
+        self,
+        http_client: aiohttp.ClientSession,
+        cache: Cache[str],
+        binary_file_cache: BinaryFileCache,
+        # Default to seven days.
+        ttl: int = 86400 * 7,
+    ):
+        self._fetcher = _Fetcher(http_client, cache, binary_file_cache, ttl)
+        self._images: dict[str, Image | None] = {}
+
     async def _get_query_api_data(self, url: str) -> dict[str, Any]:
-        api_data = json.loads(await self._request(url))
+        response_data = await self._fetcher.fetch(url)
+        api_data = json.loads(response_data)
         try:
             return api_data['query']['pages'][0]  # type: ignore[no-any-return]
         except (LookupError, TypeError) as error:
             raise RetrievalError(f'Could not successfully parse the JSON format returned by {url}: {error}')
 
     async def _get_page_query_api_data(self, page_language: str, page_name: str) -> dict[str, Any]:
         return await self._get_query_api_data(
@@ -181,17 +206,17 @@
             return {}
         return {translation_data['lang']: translation_data['title'] for translation_data in translations_data}
 
     async def get_summary(self, page_language: str, page_name: str) -> Summary | None:
         logger = logging.getLogger(__name__)
         try:
             url = f'https://{page_language}.wikipedia.org/api/rest_v1/page/summary/{page_name}'
-            request_data = await self._request(url)
+            response_data = await self._fetcher.fetch(url)
             try:
-                api_data = json.loads(request_data)
+                api_data = json.loads(response_data)
                 return Summary(
                     page_language,
                     page_name,
                     api_data['titles']['normalized'],
                     api_data['extract_html'] if 'extract_html' in api_data else api_data['extract'],
                 )
             except (json.JSONDecodeError, KeyError) as error:
@@ -216,23 +241,16 @@
             image_info_api_data = await self._get_query_api_data(url)
 
             try:
                 image_info = image_info_api_data['imageinfo'][0]
             except KeyError as error:
                 raise RetrievalError(f'Could not successfully parse the JSON content returned by {url}: {error}')
 
-            extension = None
-            for mimetypes_extension, mimetypes_media_type in mimetypes.types_map.items():
-                if mimetypes_media_type == image_info['mime']:
-                    extension = mimetypes_extension
-            await self._request(image_info['url'], extension)
-
-            file_path = (self._cache_directory_path / hashlib.md5(image_info['url'].encode("utf-8")).hexdigest()).with_suffix(f'.{extension}')
             image = Image(
-                file_path,
+                await self._fetcher.fetch_file(image_info['url']),
                 MediaType(image_info['mime']),
                 # Strip "File:" or any translated equivalent from the beginning of the image's title.
                 image_info['canonicaltitle'][image_info['canonicaltitle'].index(':') + 1:],
                 image_info['descriptionurl'],
             )
 
             return image
```

### Comparing `betty-0.3.2/betty.egg-info/PKG-INFO` & `betty-0.3.3/betty.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betty
-Version: 0.3.2
+Version: 0.3.3
 Summary: Betty helps you visualize and publish your family history by building interactive genealogy websites out of your Gramps and GECOM family trees
 Author-email: Bart Feenstra <bar@bartfeenstra.com>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -625,25 +625,33 @@
         
                              END OF TERMS AND CONDITIONS
         
 Project-URL: Documentation, https://betty.readthedocs.io
 Project-URL: Github, https://github.com/bartfeenstra/betty
 Project-URL: Twitter, https://twitter.com/BettyProject
 Project-URL: X, https://twitter.com/BettyProject
+Classifier: Environment :: Console
+Classifier: Environment :: X11 Applications :: Qt
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Lua
 Classifier: Programming Language :: JavaScript
+Classifier: Programming Language :: Unix Shell
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Internet
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Sociology :: Genealogy
+Classifier: Topic :: Sociology :: History
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Natural Language :: Dutch
 Classifier: Natural Language :: English
 Classifier: Natural Language :: French
 Classifier: Natural Language :: German
 Classifier: Natural Language :: Ukrainian
 Classifier: Typing :: Typed 
@@ -661,19 +669,20 @@
 Requires-Dist: langcodes>=3.3.0,~=3.3
 Requires-Dist: markupsafe>=2.1.1,~=2.1
 Requires-Dist: pdf2image>=1.16.0,~=1.16
 Requires-Dist: polib>=1.2.0,~=1.2
 Requires-Dist: Pillow>=10.1.0,~=10.1
 Requires-Dist: PyQt6>=6.5.0,~=6.5
 Requires-Dist: pyyaml>=6.0.0,~=6.0
-Requires-Dist: referencing~=0.34.0
-Requires-Dist: sphinx~=7.2.6
-Requires-Dist: sphinx-design~=0.5.0
-Requires-Dist: sphinx-immaterial~=0.11.10
-Requires-Dist: sphinx-autodoc-typehints~=2.0.0
+Requires-Dist: referencing>=0.34.0,~=0.34
+Requires-Dist: sphinx>=7.2.6,~=7.2
+Requires-Dist: sphinx-design>=0.5.0,~=0.5
+Requires-Dist: sphinx-immaterial>=0.11.10,~=0.11
+Requires-Dist: sphinx-autodoc-typehints>=2.0.0,~=2.0
+Requires-Dist: typing_extensions>=4.10.0,~=4.10
 Provides-Extra: pyinstaller
 Requires-Dist: pyinstaller>=6.1.0,~=6.1; extra == "pyinstaller"
 Provides-Extra: setuptools
 Requires-Dist: setuptools~=69.0; extra == "setuptools"
 Requires-Dist: twine~=5.0; extra == "setuptools"
 Requires-Dist: wheel>=0.40.0,~=0.40; extra == "setuptools"
 Provides-Extra: test
@@ -689,18 +698,23 @@
 Requires-Dist: pytest>=7.3.1,~=7.3; extra == "test"
 Requires-Dist: pytest-aioresponses>=0.2.0,~=0.2; extra == "test"
 Requires-Dist: pytest-asyncio>=0.23.4,~=0.23; extra == "test"
 Requires-Dist: pytest-cov~=5.0; extra == "test"
 Requires-Dist: pytest-mock>=3.10.0,~=3.10; extra == "test"
 Requires-Dist: pytest-qt>=4.2.0,~=4.2; extra == "test"
 Requires-Dist: pytest-xvfb>=3.0.0,~=3.0; extra == "test"
-Requires-Dist: types-aiofiles>=23.2.0.0,~=23.2; extra == "test"
+Requires-Dist: types-aiofiles>=23.2.0.20240403,~=23.2; extra == "test"
+Requires-Dist: types-babel>=2.11.0.15,~=2.11; extra == "test"
 Requires-Dist: types-click>=7.1.8,~=7.1; extra == "test"
+Requires-Dist: types-html5lib>=1.1.11.20240228,~=1.1; extra == "test"
+Requires-Dist: types-jsonschema>=4.21.0.20240331,~=4.21; extra == "test"
+Requires-Dist: types-lxml>=2024.3.27; extra == "test"
 Requires-Dist: types-mock>=5.0.0.6,~=5.0; extra == "test"
 Requires-Dist: types-polib>=1.2.0.0,~=1.2; extra == "test"
+Requires-Dist: types-pyinstaller>=6.5.0.20240311,~=6.5; extra == "test"
 Requires-Dist: types-pyyaml>=6.0.6,~=6.0; extra == "test"
 Requires-Dist: types-requests>=2.29.0.0,~=2.29; extra == "test"
 Requires-Dist: types-setuptools~=69.0; extra == "test"
 Requires-Dist: betty[pyinstaller]; extra == "test"
 Requires-Dist: betty[setuptools]; extra == "test"
 Provides-Extra: development
 Requires-Dist: pytest-repeat>=0.9.1,~=0.9; extra == "development"
```

### Comparing `betty-0.3.2/betty.egg-info/SOURCES.txt` & `betty-0.3.3/betty.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 pyproject.toml
 setup.py
 betty/__init__.py
 betty/_patch.py
 betty/_resizeimage.py
 betty/about.py
 betty/asyncio.py
-betty/cache.py
 betty/classtools.py
 betty/cli.py
 betty/concurrent.py
 betty/config.py
+betty/contextlib.py
 betty/deriver.py
 betty/dispatch.py
 betty/documentation.py
 betty/error.py
 betty/fs.py
 betty/functools.py
 betty/generate.py
@@ -69,14 +69,18 @@
 betty/assets/templates/base.html.j2
 betty/assets/templates/head.html.j2
 betty/assets/templates/linked-data.html.j2
 betty/assets/templates/sitemap-index.xml.j2
 betty/assets/templates/sitemap.xml.j2
 betty/assets/templates/entity/page-list.html.j2
 betty/assets/templates/entity/page.html.j2
+betty/cache/__init__.py
+betty/cache/_base.py
+betty/cache/file.py
+betty/cache/memory.py
 betty/extension/__init__.py
 betty/extension/cotton_candy/__init__.py
 betty/extension/cotton_candy/gui.py
 betty/extension/cotton_candy/search.py
 betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/accessibility.scss
 betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/citation.scss
 betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/entity.scss
```

### Comparing `betty-0.3.2/betty.egg-info/entry_points.txt` & `betty-0.3.3/betty.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/betty.egg-info/requires.txt` & `betty-0.3.3/betty.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -9,19 +9,20 @@
 langcodes>=3.3.0,~=3.3
 markupsafe>=2.1.1,~=2.1
 pdf2image>=1.16.0,~=1.16
 polib>=1.2.0,~=1.2
 Pillow>=10.1.0,~=10.1
 PyQt6>=6.5.0,~=6.5
 pyyaml>=6.0.0,~=6.0
-referencing~=0.34.0
-sphinx~=7.2.6
-sphinx-design~=0.5.0
-sphinx-immaterial~=0.11.10
-sphinx-autodoc-typehints~=2.0.0
+referencing>=0.34.0,~=0.34
+sphinx>=7.2.6,~=7.2
+sphinx-design>=0.5.0,~=0.5
+sphinx-immaterial>=0.11.10,~=0.11
+sphinx-autodoc-typehints>=2.0.0,~=2.0
+typing_extensions>=4.10.0,~=4.10
 
 [ci]
 codecov>=2.1.12,~=2.1
 betty[test]
 
 [development]
 pytest-repeat>=0.9.1,~=0.9
@@ -47,18 +48,23 @@
 pytest>=7.3.1,~=7.3
 pytest-aioresponses>=0.2.0,~=0.2
 pytest-asyncio>=0.23.4,~=0.23
 pytest-cov~=5.0
 pytest-mock>=3.10.0,~=3.10
 pytest-qt>=4.2.0,~=4.2
 pytest-xvfb>=3.0.0,~=3.0
-types-aiofiles>=23.2.0.0,~=23.2
+types-aiofiles>=23.2.0.20240403,~=23.2
+types-babel>=2.11.0.15,~=2.11
 types-click>=7.1.8,~=7.1
+types-html5lib>=1.1.11.20240228,~=1.1
+types-jsonschema>=4.21.0.20240331,~=4.21
+types-lxml>=2024.3.27
 types-mock>=5.0.0.6,~=5.0
 types-polib>=1.2.0.0,~=1.2
+types-pyinstaller>=6.5.0.20240311,~=6.5
 types-pyyaml>=6.0.6,~=6.0
 types-requests>=2.29.0.0,~=2.29
 types-setuptools~=69.0
 betty[pyinstaller]
 betty[setuptools]
 
 [test:sys_platform != "win32"]
```

### Comparing `betty-0.3.2/documentation/conf.py` & `betty-0.3.3/documentation/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import sys
 from os import path
 
 import betty
-from betty import about
-from betty.asyncio import wait
-from betty.fs import ROOT_DIRECTORY_PATH, FileSystem, ASSETS_DIRECTORY_PATH
+from betty import about, fs
+from betty.asyncio import wait_to_thread
+from betty.fs import ROOT_DIRECTORY_PATH, FileSystem
 from betty.locale import LocalizerRepository
 
 betty_replacements: dict[str, str] = {}
 
 assets = FileSystem()
-assets.prepend(ASSETS_DIRECTORY_PATH, 'utf-8')
+assets.prepend(fs.ASSETS_DIRECTORY_PATH, 'utf-8')
 localizers = LocalizerRepository(assets)
 for locale in localizers.locales:
-    coverage = wait(localizers.coverage(locale))
+    coverage = wait_to_thread(localizers.coverage(locale))
     betty_replacements[f'translation-coverage-{locale}'] = str(int(round(100 / (coverage[1] / coverage[0]))))
 
 sys.path.insert(0, path.dirname(path.dirname(betty.__file__)))
 project = 'Betty'
-version = wait(about.version()) or ''
-release = wait(about.version_label())
+version = wait_to_thread(about.version()) or ''
+release = wait_to_thread(about.version_label())
 copyright = 'Bart Feenstra and contributors'
 intersphinx_mapping = {
     'python': ('https://docs.python.org/3/', None),
     'jinja2': ('https://jinja.palletsprojects.com/en/latest/', None),
 }
 html_favicon = str(ROOT_DIRECTORY_PATH / 'betty' / 'assets' / 'public' / 'static' / 'betty.ico')
 html_logo = str(ROOT_DIRECTORY_PATH / 'betty' / 'assets' / 'public' / 'static' / 'betty-32x32.png')
```

### Comparing `betty-0.3.2/node_modules/flatted/python/flatted.py` & `betty-0.3.3/node_modules/flatted/python/flatted.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/node_modules/flatted/python/test.py` & `betty-0.3.3/node_modules/flatted/python/test.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.2/pyproject.toml` & `betty-0.3.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -28,32 +28,41 @@
     'langcodes ~= 3.3, >= 3.3.0',
     'markupsafe ~= 2.1, >= 2.1.1',
     'pdf2image ~= 1.16, >= 1.16.0',
     'polib ~= 1.2, >= 1.2.0',
     'Pillow ~= 10.1, >= 10.1.0',
     'PyQt6 ~= 6.5, >= 6.5.0',
     'pyyaml ~= 6.0, >= 6.0.0',
-    'referencing ~= 0.34.0',
-    'sphinx ~= 7.2.6',
-    'sphinx-design ~= 0.5.0',
-    'sphinx-immaterial ~= 0.11.10',
-    'sphinx-autodoc-typehints ~= 2.0.0',
+    'referencing ~= 0.34, >= 0.34.0',
+    'sphinx ~= 7.2, >= 7.2.6',
+    'sphinx-design ~= 0.5, >= 0.5.0',
+    'sphinx-immaterial ~= 0.11, >= 0.11.10',
+    'sphinx-autodoc-typehints ~= 2.0, >= 2.0.0',
+    'typing_extensions ~= 4.10, >= 4.10.0',
 ]
 classifiers = [
+    'Environment :: Console',
+    'Environment :: X11 Applications :: Qt',
+    'Intended Audience :: Developers',
+    'Intended Audience :: End Users/Desktop',
+    'Intended Audience :: Science/Research',
     'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
     'Programming Language :: JavaScript',
     'Programming Language :: Python :: 3.11',
     'Programming Language :: Python :: 3.12',
+    'Programming Language :: Lua',
     'Programming Language :: JavaScript',
+    'Programming Language :: Unix Shell',
     'Operating System :: MacOS :: MacOS X',
     'Operating System :: POSIX :: Linux',
     'Operating System :: Microsoft :: Windows',
     'Topic :: Internet',
     'Topic :: Scientific/Engineering :: Visualization',
     'Topic :: Sociology :: Genealogy',
+    'Topic :: Sociology :: History',
     'Topic :: Software Development :: Code Generators',
     'Natural Language :: Dutch',
     'Natural Language :: English',
     'Natural Language :: French',
     'Natural Language :: German',
     'Natural Language :: Ukrainian',
     'Typing :: Typed ',
@@ -101,18 +110,23 @@
     'pytest ~= 7.3, >= 7.3.1',
     'pytest-aioresponses ~= 0.2, >= 0.2.0 ',
     'pytest-asyncio ~= 0.23, >= 0.23.4 ',
     'pytest-cov ~= 5.0',
     'pytest-mock ~= 3.10, >= 3.10.0',
     'pytest-qt ~= 4.2, >= 4.2.0',
     'pytest-xvfb ~= 3.0, >= 3.0.0',
-    'types-aiofiles ~= 23.2, >= 23.2.0.0',
+    'types-aiofiles ~= 23.2, >= 23.2.0.20240403 ',
+    'types-babel ~= 2.11, >= 2.11.0.15',
     'types-click ~= 7.1, >= 7.1.8',
+    'types-html5lib ~= 1.1, >= 1.1.11.20240228',
+    'types-jsonschema ~= 4.21, >= 4.21.0.20240331',
+    'types-lxml >= 2024.3.27 ',
     'types-mock ~= 5.0, >= 5.0.0.6',
     'types-polib ~= 1.2, >= 1.2.0.0',
+    'types-pyinstaller ~= 6.5, >= 6.5.0.20240311',
     'types-pyyaml ~= 6.0, >= 6.0.6',
     'types-requests ~= 2.29, >= 2.29.0.0',
     'types-setuptools ~= 69.0',
     'betty[pyinstaller]',
     'betty[setuptools]',
 ]
 development = [
```

