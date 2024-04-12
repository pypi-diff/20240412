# Comparing `tmp/iop4-1.0.0.tar.gz` & `tmp/iop4-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iop4-1.0.0.tar", last modified: Wed Mar 20 17:44:40 2024, max compression
+gzip compressed data, was "iop4-1.1.0.tar", last modified: Fri Apr 12 15:19:54 2024, max compression
```

## Comparing `iop4-1.0.0.tar` & `iop4-1.1.0.tar`

### file list

```diff
@@ -1,178 +1,178 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:44:40.956865 iop4-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-20 17:44:29.000000 iop4-1.0.0/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-03-20 17:44:29.000000 iop4-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-03-20 17:44:29.000000 iop4-1.0.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-03-20 17:44:29.000000 iop4-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-20 17:44:29.000000 iop4-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-03-20 17:44:29.000000 iop4-1.0.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     9898 2024-03-20 17:44:40.956865 iop4-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7906 2024-03-20 17:44:29.000000 iop4-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:44:40.932865 iop4-1.0.0/config/
--rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-03-20 17:44:29.000000 iop4-1.0.0/config/config.example.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:44:40.932865 iop4-1.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-20 17:44:29.000000 iop4-1.0.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:44:40.932865 iop4-1.0.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    27296 2024-03-20 17:44:29.000000 iop4-1.0.0/docs/_static/jupyter.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:44:40.932865 iop4-1.0.0/docs/_static/pydata/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-20 17:44:29.000000 iop4-1.0.0/docs/_static/pydata/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-03-20 17:44:29.000000 iop4-1.0.0/docs/citations.bib
--rw-r--r--   0 runner    (1001) docker     (127)     6564 2024-03-20 17:44:29.000000 iop4-1.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-03-20 17:44:29.000000 iop4-1.0.0/docs/data_reduction_details.rst
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-03-20 17:44:29.000000 iop4-1.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-03-20 17:44:29.000000 iop4-1.0.0/docs/iop4_concepts.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-03-20 17:44:29.000000 iop4-1.0.0/docs/iop4lib.rst
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-03-20 17:44:29.000000 iop4-1.0.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:44:40.936865 iop4-1.0.0/docs/production_example/
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-03-20 17:44:29.000000 iop4-1.0.0/docs/production_example/gunicorn.service
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-20 17:44:29.000000 iop4-1.0.0/docs/production_example/gunicorn.socket
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-03-20 17:44:29.000000 iop4-1.0.0/docs/production_example/nginx_example_site
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:44:40.936865 iop4-1.0.0/docs/recipes/
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-03-20 17:44:29.000000 iop4-1.0.0/docs/recipes/01_notebook_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5428 2024-03-20 17:44:29.000000 iop4-1.0.0/docs/recipes/02_database_queries.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-03-20 17:44:29.000000 iop4-1.0.0/docs/recipes/03_manual_reduction.py
--rw-r--r--   0 runner    (1001) docker     (127)    12572 2024-03-20 17:44:29.000000 iop4-1.0.0/docs/recipes/04_details_on_astrometric_calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5782 2024-03-20 17:44:29.000000 iop4-1.0.0/docs/recipes/05_quad_matching_dipol_polarimetry_images.py
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-03-20 17:44:29.000000 iop4-1.0.0/docs/recipes/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-03-20 17:44:29.000000 iop4-1.0.0/docs/serving_iop4_in_production.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:44:40.936865 iop4-1.0.0/docs/sphinxext/
--rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-03-20 17:44:29.000000 iop4-1.0.0/docs/sphinxext/thumbnail_gallery.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:44:40.952865 iop4-1.0.0/iop4.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9898 2024-03-20 17:44:40.000000 iop4-1.0.0/iop4.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-03-20 17:44:40.000000 iop4-1.0.0/iop4.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 17:44:40.000000 iop4-1.0.0/iop4.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-20 17:44:40.000000 iop4-1.0.0/iop4.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-03-20 17:44:40.000000 iop4-1.0.0/iop4.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-20 17:44:40.000000 iop4-1.0.0/iop4.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:44:40.936865 iop4-1.0.0/iop4admin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4admin/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:44:40.940865 iop4-1.0.0/iop4admin/modeladmins/
--rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4admin/modeladmins/aperphotresult.py
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4admin/modeladmins/astrosource.py
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4admin/modeladmins/epoch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6089 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4admin/modeladmins/fitfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4admin/modeladmins/masterbias.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4admin/modeladmins/masterdark.py
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4admin/modeladmins/masterflat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4admin/modeladmins/photopolresult.py
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4admin/modeladmins/rawfit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4admin/modeladmins/reducedfit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4admin/sites.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:44:40.928865 iop4-1.0.0/iop4admin/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:44:40.940865 iop4-1.0.0/iop4admin/templates/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4admin/templates/admin/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4admin/templates/admin/base_site.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:44:40.940865 iop4-1.0.0/iop4admin/templates/iop4admin/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4admin/templates/iop4admin/base.custom.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:44:40.940865 iop4-1.0.0/iop4admin/templates/iop4admin/fits/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4admin/templates/iop4admin/fits/change_list.html
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4admin/templates/iop4admin/fits/textinput_filter.html
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4admin/templates/iop4admin/singleobj.html
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4admin/templates/iop4admin/view_astrosourcedetails.html
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4admin/templates/iop4admin/view_epochdetails.html
--rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4admin/templates/iop4admin/view_fitdetails.html
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4admin/templates/iop4admin/view_fitviewer.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:44:40.940865 iop4-1.0.0/iop4admin/views/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4admin/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4admin/views/astrosource.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4admin/views/epoch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5614 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4admin/views/fitfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4admin/views/singleobj.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:44:40.940865 iop4-1.0.0/iop4api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4api/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     7065 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4api/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4api/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:44:40.928865 iop4-1.0.0/iop4api/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:44:40.940865 iop4-1.0.0/iop4api/static/iop4api/
--rw-r--r--   0 runner    (1001) docker     (127)    12152 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4api/static/iop4api/base.css
--rw-r--r--   0 runner    (1001) docker     (127)    29760 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4api/static/iop4api/gui.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:44:40.928865 iop4-1.0.0/iop4api/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:44:40.944865 iop4-1.0.0/iop4api/templates/iop4api/
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4api/templates/iop4api/about.html
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4api/templates/iop4api/catalog.html
--rw-r--r--   0 runner    (1001) docker     (127)     5216 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4api/templates/iop4api/data.html
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4api/templates/iop4api/explore.html
--rw-r--r--   0 runner    (1001) docker     (127)    19242 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4api/templates/iop4api/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4api/templates/iop4api/login.html
--rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4api/templates/iop4api/logs.html
--rw-r--r--   0 runner    (1001) docker     (127)     9511 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4api/templates/iop4api/plot.html
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4api/templates/iop4api/query.html
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4api/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:44:40.944865 iop4-1.0.0/iop4api/views/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4api/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4api/views/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4api/views/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4api/views/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4api/views/docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4api/views/flag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4api/views/index.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4api/views/log.py
--rw-r--r--   0 runner    (1001) docker     (127)    33988 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4api/views/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:44:40.948865 iop4-1.0.0/iop4lib/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-20 17:44:40.000000 iop4-1.0.0/iop4lib/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     8765 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4lib/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:44:40.948865 iop4-1.0.0/iop4lib/db/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4lib/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4lib/db/aperphotresult.py
--rw-r--r--   0 runner    (1001) docker     (127)     6661 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4lib/db/astrosource.py
--rw-r--r--   0 runner    (1001) docker     (127)    26099 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4lib/db/epoch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4lib/db/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    10105 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4lib/db/fitfilemodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6489 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4lib/db/masterbias.py
--rw-r--r--   0 runner    (1001) docker     (127)     7116 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4lib/db/masterdark.py
--rw-r--r--   0 runner    (1001) docker     (127)     8572 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4lib/db/masterflat.py
--rw-r--r--   0 runner    (1001) docker     (127)    19370 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4lib/db/photopolresult.py
--rw-r--r--   0 runner    (1001) docker     (127)    12880 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4lib/db/rawfit.py
--rw-r--r--   0 runner    (1001) docker     (127)     9190 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4lib/db/reducedfit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4lib/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:44:40.948865 iop4-1.0.0/iop4lib/instruments/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4lib/instruments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21406 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4lib/instruments/cafos.py
--rw-r--r--   0 runner    (1001) docker     (127)    68531 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4lib/instruments/dipol.py
--rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4lib/instruments/dipol_astrometry.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    29453 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4lib/instruments/instrument.py
--rw-r--r--   0 runner    (1001) docker     (127)    21497 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4lib/instruments/osn_cameras.py
--rw-r--r--   0 runner    (1001) docker     (127)    17841 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4lib/iop4.py
--rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4lib/iop4_night_summary.html
--rw-r--r--   0 runner    (1001) docker     (127)     8757 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4lib/iop4_night_summary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:44:40.948865 iop4-1.0.0/iop4lib/telescopes/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4lib/telescopes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4lib/telescopes/cahat220.py
--rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4lib/telescopes/osnt090.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4lib/telescopes/osnt150.py
--rw-r--r--   0 runner    (1001) docker     (127)    11144 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4lib/telescopes/telescope.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:44:40.952865 iop4-1.0.0/iop4lib/utils/
--rw-r--r--   0 runner    (1001) docker     (127)    26166 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4lib/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21868 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4lib/utils/astrometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4lib/utils/filedproperty.py
--rw-r--r--   0 runner    (1001) docker     (127)    36249 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4lib/utils/host_correction_data.csv
--rw-r--r--   0 runner    (1001) docker     (127)     8173 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4lib/utils/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)    27730 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4lib/utils/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     4933 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4lib/utils/quadmatching.py
--rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4lib/utils/sourcedetection.py
--rw-r--r--   0 runner    (1001) docker     (127)    10089 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4lib/utils/sourcepairing.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4lib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:44:40.952865 iop4-1.0.0/iop4site/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:44:40.952865 iop4-1.0.0/iop4site/iop4site/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4site/iop4site/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4site/iop4site/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4site/iop4site/asgi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4site/iop4site/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4site/iop4site/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4site/iop4site/wsgi.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      664 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4site/manage.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1948 2024-03-20 17:44:29.000000 iop4-1.0.0/iop4site/resetdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-03-20 17:44:29.000000 iop4-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 17:44:40.956865 iop4-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-20 17:44:29.000000 iop4-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:44:40.952865 iop4-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 17:44:29.000000 iop4-1.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8036 2024-03-20 17:44:29.000000 iop4-1.0.0/tests/build_test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-03-20 17:44:29.000000 iop4-1.0.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-03-20 17:44:29.000000 iop4-1.0.0/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-03-20 17:44:29.000000 iop4-1.0.0/tests/test_caha_cafos.py
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-03-20 17:44:29.000000 iop4-1.0.0/tests/test_generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-03-20 17:44:29.000000 iop4-1.0.0/tests/test_osnt090_andor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7128 2024-03-20 17:44:29.000000 iop4-1.0.0/tests/test_osnt090_dipol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.834900 iop4-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-12 15:19:36.000000 iop4-1.1.0/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-12 15:19:36.000000 iop4-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-12 15:19:36.000000 iop4-1.1.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-12 15:19:36.000000 iop4-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-12 15:19:36.000000 iop4-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-12 15:19:36.000000 iop4-1.1.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    10554 2024-04-12 15:19:54.834900 iop4-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8556 2024-04-12 15:19:36.000000 iop4-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.806900 iop4-1.1.0/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-04-12 15:19:36.000000 iop4-1.1.0/config/config.example.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.810900 iop4-1.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-12 15:19:36.000000 iop4-1.1.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.810900 iop4-1.1.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    27296 2024-04-12 15:19:36.000000 iop4-1.1.0/docs/_static/jupyter.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.810900 iop4-1.1.0/docs/_static/pydata/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-12 15:19:36.000000 iop4-1.1.0/docs/_static/pydata/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-04-12 15:19:36.000000 iop4-1.1.0/docs/citations.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     6564 2024-04-12 15:19:36.000000 iop4-1.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-12 15:19:36.000000 iop4-1.1.0/docs/data_reduction_details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-12 15:19:36.000000 iop4-1.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-04-12 15:19:36.000000 iop4-1.1.0/docs/iop4_concepts.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-12 15:19:36.000000 iop4-1.1.0/docs/iop4lib.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-12 15:19:36.000000 iop4-1.1.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.810900 iop4-1.1.0/docs/production_example/
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-12 15:19:36.000000 iop4-1.1.0/docs/production_example/gunicorn.service
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-12 15:19:36.000000 iop4-1.1.0/docs/production_example/gunicorn.socket
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-12 15:19:36.000000 iop4-1.1.0/docs/production_example/nginx_example_site
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.810900 iop4-1.1.0/docs/recipes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-04-12 15:19:36.000000 iop4-1.1.0/docs/recipes/01_notebook_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5428 2024-04-12 15:19:36.000000 iop4-1.1.0/docs/recipes/02_database_queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-12 15:19:36.000000 iop4-1.1.0/docs/recipes/03_manual_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12572 2024-04-12 15:19:36.000000 iop4-1.1.0/docs/recipes/04_details_on_astrometric_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5782 2024-04-12 15:19:36.000000 iop4-1.1.0/docs/recipes/05_quad_matching_dipol_polarimetry_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-12 15:19:36.000000 iop4-1.1.0/docs/recipes/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-12 15:19:36.000000 iop4-1.1.0/docs/serving_iop4_in_production.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.810900 iop4-1.1.0/docs/sphinxext/
+-rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-04-12 15:19:36.000000 iop4-1.1.0/docs/sphinxext/thumbnail_gallery.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.830900 iop4-1.1.0/iop4.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10554 2024-04-12 15:19:54.000000 iop4-1.1.0/iop4.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-04-12 15:19:54.000000 iop4-1.1.0/iop4.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 15:19:54.000000 iop4-1.1.0/iop4.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-12 15:19:54.000000 iop4-1.1.0/iop4.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-12 15:19:54.000000 iop4-1.1.0/iop4.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-12 15:19:54.000000 iop4-1.1.0/iop4.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.814900 iop4-1.1.0/iop4admin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.814900 iop4-1.1.0/iop4admin/modeladmins/
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/modeladmins/aperphotresult.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/modeladmins/astrosource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/modeladmins/epoch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6089 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/modeladmins/fitfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/modeladmins/masterbias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/modeladmins/masterdark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/modeladmins/masterflat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/modeladmins/photopolresult.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/modeladmins/rawfit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/modeladmins/reducedfit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/sites.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.802900 iop4-1.1.0/iop4admin/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.814900 iop4-1.1.0/iop4admin/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/templates/admin/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/templates/admin/base_site.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.814900 iop4-1.1.0/iop4admin/templates/iop4admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/templates/iop4admin/base.custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.814900 iop4-1.1.0/iop4admin/templates/iop4admin/fits/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/templates/iop4admin/fits/change_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/templates/iop4admin/fits/textinput_filter.html
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/templates/iop4admin/singleobj.html
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/templates/iop4admin/view_astrosourcedetails.html
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/templates/iop4admin/view_epochdetails.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/templates/iop4admin/view_fitdetails.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/templates/iop4admin/view_fitviewer.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.818900 iop4-1.1.0/iop4admin/views/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/views/astrosource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/views/epoch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5614 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/views/fitfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/views/singleobj.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.818900 iop4-1.1.0/iop4api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4api/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7065 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4api/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4api/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.806900 iop4-1.1.0/iop4api/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.818900 iop4-1.1.0/iop4api/static/iop4api/
+-rw-r--r--   0 runner    (1001) docker     (127)    12152 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4api/static/iop4api/base.css
+-rw-r--r--   0 runner    (1001) docker     (127)    29760 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4api/static/iop4api/gui.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.806900 iop4-1.1.0/iop4api/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.818900 iop4-1.1.0/iop4api/templates/iop4api/
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4api/templates/iop4api/about.html
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4api/templates/iop4api/catalog.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5216 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4api/templates/iop4api/data.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4api/templates/iop4api/explore.html
+-rw-r--r--   0 runner    (1001) docker     (127)    19242 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4api/templates/iop4api/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4api/templates/iop4api/login.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4api/templates/iop4api/logs.html
+-rw-r--r--   0 runner    (1001) docker     (127)     9511 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4api/templates/iop4api/plot.html
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4api/templates/iop4api/query.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4api/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.822900 iop4-1.1.0/iop4api/views/
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4api/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4api/views/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4api/views/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4api/views/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4api/views/docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4api/views/flag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4api/views/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4api/views/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33988 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4api/views/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.822900 iop4-1.1.0/iop4lib/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-12 15:19:54.000000 iop4-1.1.0/iop4lib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8969 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.822900 iop4-1.1.0/iop4lib/db/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/db/aperphotresult.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6661 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/db/astrosource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26099 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/db/epoch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/db/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10105 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/db/fitfilemodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6489 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/db/masterbias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7116 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/db/masterdark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8572 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/db/masterflat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19370 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/db/photopolresult.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12880 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/db/rawfit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9190 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/db/reducedfit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.826900 iop4-1.1.0/iop4lib/instruments/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/instruments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22103 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/instruments/cafos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68531 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/instruments/dipol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/instruments/dipol_astrometry.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    29453 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/instruments/instrument.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21497 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/instruments/osn_cameras.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17863 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/iop4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/iop4_night_summary.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8798 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/iop4_night_summary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.826900 iop4-1.1.0/iop4lib/telescopes/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/telescopes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/telescopes/cahat220.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/telescopes/osnt090.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/telescopes/osnt150.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11144 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/telescopes/telescope.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.826900 iop4-1.1.0/iop4lib/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    26166 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21868 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/utils/astrometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/utils/filedproperty.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36249 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/utils/host_correction_data.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     8173 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/utils/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27730 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/utils/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4933 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/utils/quadmatching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/utils/sourcedetection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10089 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/utils/sourcepairing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.826900 iop4-1.1.0/iop4site/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.830900 iop4-1.1.0/iop4site/iop4site/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4site/iop4site/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4site/iop4site/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4site/iop4site/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4site/iop4site/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4site/iop4site/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4site/iop4site/wsgi.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      664 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4site/manage.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1948 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4site/resetdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-12 15:19:36.000000 iop4-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 15:19:54.834900 iop4-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-12 15:19:36.000000 iop4-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.830900 iop4-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:36.000000 iop4-1.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8036 2024-04-12 15:19:36.000000 iop4-1.1.0/tests/build_test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-04-12 15:19:36.000000 iop4-1.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-12 15:19:36.000000 iop4-1.1.0/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-04-12 15:19:36.000000 iop4-1.1.0/tests/test_caha_cafos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-12 15:19:36.000000 iop4-1.1.0/tests/test_generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-04-12 15:19:36.000000 iop4-1.1.0/tests/test_osnt090_andor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7128 2024-04-12 15:19:36.000000 iop4-1.1.0/tests/test_osnt090_dipol.py
```

### Comparing `iop4-1.0.0/.gitignore` & `iop4-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/CITATION.cff` & `iop4-1.1.0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/LICENSE` & `iop4-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/Makefile` & `iop4-1.1.0/Makefile`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/PKG-INFO` & `iop4-1.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iop4
-Version: 1.0.0
+Version: 1.1.0
 Summary: A rewrite of IOP3, a pipeline to work with photometry and polarimetry of optical data from CAHA and OSN.
 Author-email: Juan Escudero Pedrosa <jescudero@iaa.es>
 License: BSD-3-Clause
 Project-URL: repository, https://github.com/juanep97/iop4
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -36,15 +36,15 @@
 Requires-Dist: codecov; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Provides-Extra: doc
 Requires-Dist: numpydoc; extra == "doc"
 Requires-Dist: sphinx; extra == "doc"
 Requires-Dist: sphinx-automodapi; extra == "doc"
 Requires-Dist: sphinx-mdinclude; extra == "doc"
-Requires-Dist: pydata-sphinx-theme; extra == "doc"
+Requires-Dist: pydata-sphinx-theme<0.15.2; extra == "doc"
 Requires-Dist: sphinxcontrib-bibtex; extra == "doc"
 Requires-Dist: docutils>=0.20; extra == "doc"
 Requires-Dist: nbsphinx; extra == "doc"
 Requires-Dist: nbstripout; extra == "doc"
 Requires-Dist: jupytext; extra == "doc"
 Requires-Dist: ipykernel; extra == "doc"
 Requires-Dist: sphinx-gallery; extra == "doc"
@@ -53,57 +53,72 @@
 Requires-Dist: setuptools_scm; extra == "dev"
 Provides-Extra: all
 Requires-Dist: iop4[dev,doc,test]; extra == "all"
 
 <div>
 <a href="https://github.com/juanep97/iop4/actions/workflows/ci.yml"><img alt="CI" src="https://github.com/juanep97/iop4/actions/workflows/ci.yml/badge.svg"></img></a>
 <a href="https://zenodo.org/doi/10.5281/zenodo.10222722"><img src="https://zenodo.org/badge/636786270.svg" alt="DOI"></img></a>
+<a href="https://pypi.org/project/iop4/"><img src="https://img.shields.io/pypi/v/iop4" alt="PyPI"></img></a>
 </div>
 
 
 **IOP4** is a complete rewrite of IOP3, a pipeline to work with **photometry** and **polarimetry** of **optical data** from [CAHA](https://www.caha.es/es/) and [OSN](https://www.osn.iaa.csic.es/) observatories. It is built to ease debugging and inspection of data.
 
-IOP4 implements _Object Relational Mapping_ (**ORM**) to seamlessly integrate all information about the reduction and results in a database which can be used to query and plot results, flag data and inspect the reduction process in a integrated fashion with the whole pipeline. It also ships with an already **built-in web interface** which can be used out of the box to browse the database and supervise all pipeline processes.
+IOP4 implements _Object Relational Mapping_ (**ORM**) to seamlessly integrate all information about the reduction and results in a database which can be used to query and plot results, flag data and inspect the reduction process in an integrated fashion with the whole pipeline. It also ships with an already **built-in web interface** which can be used out of the box to browse the database and supervise all pipeline processes.
 
 
 ## Installation
+We recommend installing IOP4 in an isolated environtment as described below. IOP4 is hosted in [PyPI software repository](https://pypi.org/project/iop4/).
 
 ### Option 1: Using a virtual environment
 
 **Note:** IOP4 requires Python 3.10 or later. You can check your Python version with `python --version`. If you have a compatible version, you can skip this step.
   
 If you don't have Python 3.10 or later, you can install [pyenv](https://github.com/pyenv/pyenv) and [pyenv-virtualenv](https://github.com/pyenv/pyenv-virtualenv), which will manage python versions for you. You can use the automatic installer [pyenv-installer](https://github.com/pyenv/pyenv-installer):
 
 ```bash
     $ curl https://pyenv.run | bash
 ```
 
-Follow the instruction that these command output to add `pyenv` to `PATH` (or copy the commands from https://github.com/pyenv/pyenv for your shell). Restart your terminal, or source the file (e.g. `. ~/.bashrc` or `. ~/.zshrc`) Then, run 
+Follow the instructions that this command outputs to add `pyenv` to `PATH` (or copy the commands from https://github.com/pyenv/pyenv for your shell). Restart your terminal, or source the file (e.g. `. ~/.bashrc` or `. ~/.zshrc`) Then, run 
 ```bash 
     $ pyenv install 3.10
     $ pyenv virtualenv 3.10 iop4-venv
     $ pyenv activate iop4-venv
 ```
 Now you will have a virtual environment with the right Python version, and you can continue with the next step. To deactivate, just run `pyenv deactivate`.
 
-Now you can clone this repository and install IOP4:
+With the environment activated, you can install IOP4 latest version by running:
+```bash
+    $ pip install iop4
+```
+
+Alternatively, you can clone this repository and install IOP4:
 ```bash
     $ git clone 'git@github.com:juanep97/iop4.git'
     $ cd iop4
     $ pip install .
 ```
 or `pip install -e .` if you want to install it in developer mode.
 
 
-### Option 2: Using conda
-
-Clone this repository and run from a terminal
+### Option 2: Using conda/mamba
+As the previous option, create and activate the environment as follows:
 ```bash
     $ conda create -n iop4 python=3.10
     $ conda activate iop4
+```
+
+Then run:
+```bash
+    $ pip install iop4
+```
+
+Alternatively, you can also clone this repository and run (inside the root directory of the cloned repository):
+```bash
     $ pip install .
 ```
 or `pip install -e .` if you want to install it in developer mode.
 
 If you followed the steps in any of the two options above, you will have installed the module `iop4lib` and the `iop4` command, and the `iop4site` project. 
 
 ## Configuration
@@ -204,30 +219,31 @@
 
 ## Contribute
 
 You are welcome to contribute to IOP4. Fork and create a PR!
 
 ## Citing IOP4
 
-If you use IOP4, or any result derived with it, we kindly ask you to cite the following references:
+If you use IOP4, or any result derived from it, we kindly ask you to cite the following references:
 
 <div>
 <a href="https://zenodo.org/doi/10.5281/zenodo.10222722"><img src="https://zenodo.org/badge/636786270.svg" alt="DOI"></img></a>
 </div>
 
 You can use the following BibTeX entry:
 
 ```bibtex
-@software{juan_escudero_2023_10222723,
-  author       = {Juan Escudero and
-                  Daniel Morcuende},
-  title        = {juanep97/iop4: v0.1.0},
-  month        = nov,
-  year         = 2023,
+@software{escudero_pedrosa_2024_10845509,
+  author       = {Escudero Pedrosa, Juan and
+                  Morcuende Parrilla, Daniel and
+                  Otero-Santos, Jorge},
+  title        = {IOP4},
+  month        = mar,
+  year         = 2024,
   publisher    = {Zenodo},
-  version      = {v0.1.0},
-  doi          = {10.5281/zenodo.10222723},
-  url          = {https://doi.org/10.5281/zenodo.10222723}
+  version      = {v1.0.0},
+  doi          = {10.5281/zenodo.10222722},
+  url          = {https://zenodo.org/doi/10.5281/zenodo.10222722}
 }
 ```
 
 This might change in the future, as IOP4 is still under the process of being published in a peer-reviewed journal. Check this repository for updates :)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iop4 Version: 1.0.0 Summary: A rewrite of IOP3, a
+Metadata-Version: 2.1 Name: iop4 Version: 1.1.0 Summary: A rewrite of IOP3, a
 pipeline to work with photometry and polarimetry of optical data from CAHA and
 OSN. Author-email: Juan Escudero Pedrosa
 iaa.es> License: BSD-3-Clause Project-URL: repository, https://github.com/
 juanep97/iop4 Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: BSD License Classifier: Operating System :: OS
 Independent Requires-Python: <=3.12,>3.10 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: numpy==1.24.2 Requires-Dist:
@@ -14,54 +14,60 @@
 multiprocess==0.70.14 Requires-Dist: pypandoc Requires-Dist: termcolor
 Requires-Dist: pyyaml<5.4 Requires-Dist: psutil Provides-Extra: test Requires-
 Dist: pytest; extra == "test" Requires-Dist: pytest-django; extra == "test"
 Requires-Dist: codecov; extra == "test" Requires-Dist: pytest-cov; extra ==
 "test" Provides-Extra: doc Requires-Dist: numpydoc; extra == "doc" Requires-
 Dist: sphinx; extra == "doc" Requires-Dist: sphinx-automodapi; extra == "doc"
 Requires-Dist: sphinx-mdinclude; extra == "doc" Requires-Dist: pydata-sphinx-
-theme; extra == "doc" Requires-Dist: sphinxcontrib-bibtex; extra == "doc"
-Requires-Dist: docutils>=0.20; extra == "doc" Requires-Dist: nbsphinx; extra ==
-"doc" Requires-Dist: nbstripout; extra == "doc" Requires-Dist: jupytext; extra
-== "doc" Requires-Dist: ipykernel; extra == "doc" Requires-Dist: sphinx-
-gallery; extra == "doc" Requires-Dist: myst-nb; extra == "doc" Provides-Extra:
-dev Requires-Dist: setuptools_scm; extra == "dev" Provides-Extra: all Requires-
-Dist: iop4[dev,doc,test]; extra == "all"
-_[_C_I_]_[_D_O_I_]
+theme<0.15.2; extra == "doc" Requires-Dist: sphinxcontrib-bibtex; extra ==
+"doc" Requires-Dist: docutils>=0.20; extra == "doc" Requires-Dist: nbsphinx;
+extra == "doc" Requires-Dist: nbstripout; extra == "doc" Requires-Dist:
+jupytext; extra == "doc" Requires-Dist: ipykernel; extra == "doc" Requires-
+Dist: sphinx-gallery; extra == "doc" Requires-Dist: myst-nb; extra == "doc"
+Provides-Extra: dev Requires-Dist: setuptools_scm; extra == "dev" Provides-
+Extra: all Requires-Dist: iop4[dev,doc,test]; extra == "all"
+_[_C_I_]_[_D_O_I_]_[_P_y_P_I_]
 **IOP4** is a complete rewrite of IOP3, a pipeline to work with **photometry**
 and **polarimetry** of **optical data** from [CAHA](https://www.caha.es/es/
 ) and [OSN](https://www.osn.iaa.csic.es/) observatories. It is built to ease
 debugging and inspection of data. IOP4 implements _Object Relational Mapping_
 (**ORM**) to seamlessly integrate all information about the reduction and
 results in a database which can be used to query and plot results, flag data
-and inspect the reduction process in a integrated fashion with the whole
+and inspect the reduction process in an integrated fashion with the whole
 pipeline. It also ships with an already **built-in web interface** which can be
 used out of the box to browse the database and supervise all pipeline
-processes. ## Installation ### Option 1: Using a virtual environment **Note:**
-IOP4 requires Python 3.10 or later. You can check your Python version with
-`python --version`. If you have a compatible version, you can skip this step.
-If you don't have Python 3.10 or later, you can install [pyenv](https://
+processes. ## Installation We recommend installing IOP4 in an isolated
+environtment as described below. IOP4 is hosted in [PyPI software repository]
+(https://pypi.org/project/iop4/). ### Option 1: Using a virtual environment
+**Note:** IOP4 requires Python 3.10 or later. You can check your Python version
+with `python --version`. If you have a compatible version, you can skip this
+step. If you don't have Python 3.10 or later, you can install [pyenv](https://
 github.com/pyenv/pyenv) and [pyenv-virtualenv](https://github.com/pyenv/pyenv-
 virtualenv), which will manage python versions for you. You can use the
 automatic installer [pyenv-installer](https://github.com/pyenv/pyenv-
-installer): ```bash $ curl https://pyenv.run | bash ``` Follow the instruction
-that these command output to add `pyenv` to `PATH` (or copy the commands from
+installer): ```bash $ curl https://pyenv.run | bash ``` Follow the instructions
+that this command outputs to add `pyenv` to `PATH` (or copy the commands from
 https://github.com/pyenv/pyenv for your shell). Restart your terminal, or
 source the file (e.g. `. ~/.bashrc` or `. ~/.zshrc`) Then, run ```bash $ pyenv
 install 3.10 $ pyenv virtualenv 3.10 iop4-venv $ pyenv activate iop4-venv ```
 Now you will have a virtual environment with the right Python version, and you
 can continue with the next step. To deactivate, just run `pyenv deactivate`.
-Now you can clone this repository and install IOP4: ```bash $ git clone
-'git@github.com:juanep97/iop4.git' $ cd iop4 $ pip install . ``` or `pip
-install -e .` if you want to install it in developer mode. ### Option 2: Using
-conda Clone this repository and run from a terminal ```bash $ conda create -
-n iop4 python=3.10 $ conda activate iop4 $ pip install . ``` or `pip install -
-e .` if you want to install it in developer mode. If you followed the steps in
-any of the two options above, you will have installed the module `iop4lib` and
-the `iop4` command, and the `iop4site` project. ## Configuration After
-installation, take a look at the example configuration file (`config/
+With the environment activated, you can install IOP4 latest version by running:
+```bash $ pip install iop4 ``` Alternatively, you can clone this repository and
+install IOP4: ```bash $ git clone 'git@github.com:juanep97/iop4.git' $ cd iop4
+$ pip install . ``` or `pip install -e .` if you want to install it in
+developer mode. ### Option 2: Using conda/mamba As the previous option, create
+and activate the environment as follows: ```bash $ conda create -n iop4
+python=3.10 $ conda activate iop4 ``` Then run: ```bash $ pip install iop4 ```
+Alternatively, you can also clone this repository and run (inside the root
+directory of the cloned repository): ```bash $ pip install . ``` or `pip
+install -e .` if you want to install it in developer mode. If you followed the
+steps in any of the two options above, you will have installed the module
+`iop4lib` and the `iop4` command, and the `iop4site` project. ## Configuration
+After installation, take a look at the example configuration file (`config/
 config.example.yaml`), set the appropriate variables (path to the database,
 data directory, astrometry index files path, credentials, etc) and rename it to
 `config/config.yaml`. ### Running Tests To run the tests, first follow the
 previous steps to configure IOP4. At the moment, you will also need to download
 the `iop4testdata.tar.gz` file manually and place it under your home directory.
 Then, run ```bash $ pytest -vxs tests/ ``` If it is the first time executing
 IOP4, the astrometry index files will be downloaded to `astrometry_cache_path`
@@ -109,17 +115,17 @@
 %autoreload all import iop4lib.config iop4conf = iop4lib.Config(config_db=True,
 gonogui=False, jupytermode=True) ``` ### Tips You can get an IPython
 interactive terminal after running iop4 using the `-i` option. You can override
 any config option using the `-o` option, e.g.: ```bash $ iop4 -i -o nthreads=20
 -o log_file=test.log --epoch-list T090/230313 T090/230317 ``` ## Documentation
 To build and show the documentation, run ```bash $ make docs-sphinx $ make
 docs-show ``` ## Contribute You are welcome to contribute to IOP4. Fork and
-create a PR! ## Citing IOP4 If you use IOP4, or any result derived with it, we
+create a PR! ## Citing IOP4 If you use IOP4, or any result derived from it, we
 kindly ask you to cite the following references:
 _[_D_O_I_]
 You can use the following BibTeX entry: ```bibtex @software
-{juan_escudero_2023_10222723, author = {Juan Escudero and Daniel Morcuende},
-title = {juanep97/iop4: v0.1.0}, month = nov, year = 2023, publisher =
-{Zenodo}, version = {v0.1.0}, doi = {10.5281/zenodo.10222723}, url = {https://
-doi.org/10.5281/zenodo.10222723} } ``` This might change in the future, as IOP4
-is still under the process of being published in a peer-reviewed journal. Check
-this repository for updates :)
+{escudero_pedrosa_2024_10845509, author = {Escudero Pedrosa, Juan and Morcuende
+Parrilla, Daniel and Otero-Santos, Jorge}, title = {IOP4}, month = mar, year =
+2024, publisher = {Zenodo}, version = {v1.0.0}, doi = {10.5281/
+zenodo.10222722}, url = {https://zenodo.org/doi/10.5281/zenodo.10222722} } ```
+This might change in the future, as IOP4 is still under the process of being
+published in a peer-reviewed journal. Check this repository for updates :)
```

### Comparing `iop4-1.0.0/README.md` & `iop4-1.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,53 +1,68 @@
 <div>
 <a href="https://github.com/juanep97/iop4/actions/workflows/ci.yml"><img alt="CI" src="https://github.com/juanep97/iop4/actions/workflows/ci.yml/badge.svg"></img></a>
 <a href="https://zenodo.org/doi/10.5281/zenodo.10222722"><img src="https://zenodo.org/badge/636786270.svg" alt="DOI"></img></a>
+<a href="https://pypi.org/project/iop4/"><img src="https://img.shields.io/pypi/v/iop4" alt="PyPI"></img></a>
 </div>
 
 
 **IOP4** is a complete rewrite of IOP3, a pipeline to work with **photometry** and **polarimetry** of **optical data** from [CAHA](https://www.caha.es/es/) and [OSN](https://www.osn.iaa.csic.es/) observatories. It is built to ease debugging and inspection of data.
 
-IOP4 implements _Object Relational Mapping_ (**ORM**) to seamlessly integrate all information about the reduction and results in a database which can be used to query and plot results, flag data and inspect the reduction process in a integrated fashion with the whole pipeline. It also ships with an already **built-in web interface** which can be used out of the box to browse the database and supervise all pipeline processes.
+IOP4 implements _Object Relational Mapping_ (**ORM**) to seamlessly integrate all information about the reduction and results in a database which can be used to query and plot results, flag data and inspect the reduction process in an integrated fashion with the whole pipeline. It also ships with an already **built-in web interface** which can be used out of the box to browse the database and supervise all pipeline processes.
 
 
 ## Installation
+We recommend installing IOP4 in an isolated environtment as described below. IOP4 is hosted in [PyPI software repository](https://pypi.org/project/iop4/).
 
 ### Option 1: Using a virtual environment
 
 **Note:** IOP4 requires Python 3.10 or later. You can check your Python version with `python --version`. If you have a compatible version, you can skip this step.
   
 If you don't have Python 3.10 or later, you can install [pyenv](https://github.com/pyenv/pyenv) and [pyenv-virtualenv](https://github.com/pyenv/pyenv-virtualenv), which will manage python versions for you. You can use the automatic installer [pyenv-installer](https://github.com/pyenv/pyenv-installer):
 
 ```bash
     $ curl https://pyenv.run | bash
 ```
 
-Follow the instruction that these command output to add `pyenv` to `PATH` (or copy the commands from https://github.com/pyenv/pyenv for your shell). Restart your terminal, or source the file (e.g. `. ~/.bashrc` or `. ~/.zshrc`) Then, run 
+Follow the instructions that this command outputs to add `pyenv` to `PATH` (or copy the commands from https://github.com/pyenv/pyenv for your shell). Restart your terminal, or source the file (e.g. `. ~/.bashrc` or `. ~/.zshrc`) Then, run 
 ```bash 
     $ pyenv install 3.10
     $ pyenv virtualenv 3.10 iop4-venv
     $ pyenv activate iop4-venv
 ```
 Now you will have a virtual environment with the right Python version, and you can continue with the next step. To deactivate, just run `pyenv deactivate`.
 
-Now you can clone this repository and install IOP4:
+With the environment activated, you can install IOP4 latest version by running:
+```bash
+    $ pip install iop4
+```
+
+Alternatively, you can clone this repository and install IOP4:
 ```bash
     $ git clone 'git@github.com:juanep97/iop4.git'
     $ cd iop4
     $ pip install .
 ```
 or `pip install -e .` if you want to install it in developer mode.
 
 
-### Option 2: Using conda
-
-Clone this repository and run from a terminal
+### Option 2: Using conda/mamba
+As the previous option, create and activate the environment as follows:
 ```bash
     $ conda create -n iop4 python=3.10
     $ conda activate iop4
+```
+
+Then run:
+```bash
+    $ pip install iop4
+```
+
+Alternatively, you can also clone this repository and run (inside the root directory of the cloned repository):
+```bash
     $ pip install .
 ```
 or `pip install -e .` if you want to install it in developer mode.
 
 If you followed the steps in any of the two options above, you will have installed the module `iop4lib` and the `iop4` command, and the `iop4site` project. 
 
 ## Configuration
@@ -148,30 +163,31 @@
 
 ## Contribute
 
 You are welcome to contribute to IOP4. Fork and create a PR!
 
 ## Citing IOP4
 
-If you use IOP4, or any result derived with it, we kindly ask you to cite the following references:
+If you use IOP4, or any result derived from it, we kindly ask you to cite the following references:
 
 <div>
 <a href="https://zenodo.org/doi/10.5281/zenodo.10222722"><img src="https://zenodo.org/badge/636786270.svg" alt="DOI"></img></a>
 </div>
 
 You can use the following BibTeX entry:
 
 ```bibtex
-@software{juan_escudero_2023_10222723,
-  author       = {Juan Escudero and
-                  Daniel Morcuende},
-  title        = {juanep97/iop4: v0.1.0},
-  month        = nov,
-  year         = 2023,
+@software{escudero_pedrosa_2024_10845509,
+  author       = {Escudero Pedrosa, Juan and
+                  Morcuende Parrilla, Daniel and
+                  Otero-Santos, Jorge},
+  title        = {IOP4},
+  month        = mar,
+  year         = 2024,
   publisher    = {Zenodo},
-  version      = {v0.1.0},
-  doi          = {10.5281/zenodo.10222723},
-  url          = {https://doi.org/10.5281/zenodo.10222723}
+  version      = {v1.0.0},
+  doi          = {10.5281/zenodo.10222722},
+  url          = {https://zenodo.org/doi/10.5281/zenodo.10222722}
 }
 ```
 
-This might change in the future, as IOP4 is still under the process of being published in a peer-reviewed journal. Check this repository for updates :)
+This might change in the future, as IOP4 is still under the process of being published in a peer-reviewed journal. Check this repository for updates :)
```

#### html2text {}

```diff
@@ -1,40 +1,46 @@
-_[_C_I_]_[_D_O_I_]
+_[_C_I_]_[_D_O_I_]_[_P_y_P_I_]
 **IOP4** is a complete rewrite of IOP3, a pipeline to work with **photometry**
 and **polarimetry** of **optical data** from [CAHA](https://www.caha.es/es/
 ) and [OSN](https://www.osn.iaa.csic.es/) observatories. It is built to ease
 debugging and inspection of data. IOP4 implements _Object Relational Mapping_
 (**ORM**) to seamlessly integrate all information about the reduction and
 results in a database which can be used to query and plot results, flag data
-and inspect the reduction process in a integrated fashion with the whole
+and inspect the reduction process in an integrated fashion with the whole
 pipeline. It also ships with an already **built-in web interface** which can be
 used out of the box to browse the database and supervise all pipeline
-processes. ## Installation ### Option 1: Using a virtual environment **Note:**
-IOP4 requires Python 3.10 or later. You can check your Python version with
-`python --version`. If you have a compatible version, you can skip this step.
-If you don't have Python 3.10 or later, you can install [pyenv](https://
+processes. ## Installation We recommend installing IOP4 in an isolated
+environtment as described below. IOP4 is hosted in [PyPI software repository]
+(https://pypi.org/project/iop4/). ### Option 1: Using a virtual environment
+**Note:** IOP4 requires Python 3.10 or later. You can check your Python version
+with `python --version`. If you have a compatible version, you can skip this
+step. If you don't have Python 3.10 or later, you can install [pyenv](https://
 github.com/pyenv/pyenv) and [pyenv-virtualenv](https://github.com/pyenv/pyenv-
 virtualenv), which will manage python versions for you. You can use the
 automatic installer [pyenv-installer](https://github.com/pyenv/pyenv-
-installer): ```bash $ curl https://pyenv.run | bash ``` Follow the instruction
-that these command output to add `pyenv` to `PATH` (or copy the commands from
+installer): ```bash $ curl https://pyenv.run | bash ``` Follow the instructions
+that this command outputs to add `pyenv` to `PATH` (or copy the commands from
 https://github.com/pyenv/pyenv for your shell). Restart your terminal, or
 source the file (e.g. `. ~/.bashrc` or `. ~/.zshrc`) Then, run ```bash $ pyenv
 install 3.10 $ pyenv virtualenv 3.10 iop4-venv $ pyenv activate iop4-venv ```
 Now you will have a virtual environment with the right Python version, and you
 can continue with the next step. To deactivate, just run `pyenv deactivate`.
-Now you can clone this repository and install IOP4: ```bash $ git clone
-'git@github.com:juanep97/iop4.git' $ cd iop4 $ pip install . ``` or `pip
-install -e .` if you want to install it in developer mode. ### Option 2: Using
-conda Clone this repository and run from a terminal ```bash $ conda create -
-n iop4 python=3.10 $ conda activate iop4 $ pip install . ``` or `pip install -
-e .` if you want to install it in developer mode. If you followed the steps in
-any of the two options above, you will have installed the module `iop4lib` and
-the `iop4` command, and the `iop4site` project. ## Configuration After
-installation, take a look at the example configuration file (`config/
+With the environment activated, you can install IOP4 latest version by running:
+```bash $ pip install iop4 ``` Alternatively, you can clone this repository and
+install IOP4: ```bash $ git clone 'git@github.com:juanep97/iop4.git' $ cd iop4
+$ pip install . ``` or `pip install -e .` if you want to install it in
+developer mode. ### Option 2: Using conda/mamba As the previous option, create
+and activate the environment as follows: ```bash $ conda create -n iop4
+python=3.10 $ conda activate iop4 ``` Then run: ```bash $ pip install iop4 ```
+Alternatively, you can also clone this repository and run (inside the root
+directory of the cloned repository): ```bash $ pip install . ``` or `pip
+install -e .` if you want to install it in developer mode. If you followed the
+steps in any of the two options above, you will have installed the module
+`iop4lib` and the `iop4` command, and the `iop4site` project. ## Configuration
+After installation, take a look at the example configuration file (`config/
 config.example.yaml`), set the appropriate variables (path to the database,
 data directory, astrometry index files path, credentials, etc) and rename it to
 `config/config.yaml`. ### Running Tests To run the tests, first follow the
 previous steps to configure IOP4. At the moment, you will also need to download
 the `iop4testdata.tar.gz` file manually and place it under your home directory.
 Then, run ```bash $ pytest -vxs tests/ ``` If it is the first time executing
 IOP4, the astrometry index files will be downloaded to `astrometry_cache_path`
@@ -82,17 +88,17 @@
 %autoreload all import iop4lib.config iop4conf = iop4lib.Config(config_db=True,
 gonogui=False, jupytermode=True) ``` ### Tips You can get an IPython
 interactive terminal after running iop4 using the `-i` option. You can override
 any config option using the `-o` option, e.g.: ```bash $ iop4 -i -o nthreads=20
 -o log_file=test.log --epoch-list T090/230313 T090/230317 ``` ## Documentation
 To build and show the documentation, run ```bash $ make docs-sphinx $ make
 docs-show ``` ## Contribute You are welcome to contribute to IOP4. Fork and
-create a PR! ## Citing IOP4 If you use IOP4, or any result derived with it, we
+create a PR! ## Citing IOP4 If you use IOP4, or any result derived from it, we
 kindly ask you to cite the following references:
 _[_D_O_I_]
 You can use the following BibTeX entry: ```bibtex @software
-{juan_escudero_2023_10222723, author = {Juan Escudero and Daniel Morcuende},
-title = {juanep97/iop4: v0.1.0}, month = nov, year = 2023, publisher =
-{Zenodo}, version = {v0.1.0}, doi = {10.5281/zenodo.10222723}, url = {https://
-doi.org/10.5281/zenodo.10222723} } ``` This might change in the future, as IOP4
-is still under the process of being published in a peer-reviewed journal. Check
-this repository for updates :)
+{escudero_pedrosa_2024_10845509, author = {Escudero Pedrosa, Juan and Morcuende
+Parrilla, Daniel and Otero-Santos, Jorge}, title = {IOP4}, month = mar, year =
+2024, publisher = {Zenodo}, version = {v1.0.0}, doi = {10.5281/
+zenodo.10222722}, url = {https://zenodo.org/doi/10.5281/zenodo.10222722} } ```
+This might change in the future, as IOP4 is still under the process of being
+published in a peer-reviewed journal. Check this repository for updates :)
```

### Comparing `iop4-1.0.0/config/config.example.yaml` & `iop4-1.1.0/config/config.example.yaml`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/docs/Makefile` & `iop4-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/docs/_static/jupyter.png` & `iop4-1.1.0/docs/_static/jupyter.png`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/docs/citations.bib` & `iop4-1.1.0/docs/citations.bib`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/docs/conf.py` & `iop4-1.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/docs/data_reduction_details.rst` & `iop4-1.1.0/docs/data_reduction_details.rst`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/docs/index.rst` & `iop4-1.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/docs/iop4_concepts.rst` & `iop4-1.1.0/docs/iop4_concepts.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+.. _iop4_concepts:
+
+
 IOP4 concepts
 =============
 
 **IOP4** is a pipeline to work with
 **photometry** and **polarimetry** of **optical data** from
 `CAHA <https://www.caha.es/es/>`__ and
 `OSN <https://www.osn.iaa.csic.es/>`__ observatories. It is built to
```

### Comparing `iop4-1.0.0/docs/iop4lib.rst` & `iop4-1.1.0/docs/iop4lib.rst`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/docs/make.bat` & `iop4-1.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/docs/recipes/01_notebook_configuration.py` & `iop4-1.1.0/docs/recipes/01_notebook_configuration.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/docs/recipes/02_database_queries.py` & `iop4-1.1.0/docs/recipes/02_database_queries.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/docs/recipes/03_manual_reduction.py` & `iop4-1.1.0/docs/recipes/03_manual_reduction.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/docs/recipes/04_details_on_astrometric_calibration.py` & `iop4-1.1.0/docs/recipes/04_details_on_astrometric_calibration.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/docs/recipes/05_quad_matching_dipol_polarimetry_images.py` & `iop4-1.1.0/docs/recipes/05_quad_matching_dipol_polarimetry_images.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/docs/serving_iop4_in_production.rst` & `iop4-1.1.0/docs/serving_iop4_in_production.rst`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/docs/sphinxext/thumbnail_gallery.py` & `iop4-1.1.0/docs/sphinxext/thumbnail_gallery.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4.egg-info/PKG-INFO` & `iop4-1.1.0/iop4.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iop4
-Version: 1.0.0
+Version: 1.1.0
 Summary: A rewrite of IOP3, a pipeline to work with photometry and polarimetry of optical data from CAHA and OSN.
 Author-email: Juan Escudero Pedrosa <jescudero@iaa.es>
 License: BSD-3-Clause
 Project-URL: repository, https://github.com/juanep97/iop4
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -36,15 +36,15 @@
 Requires-Dist: codecov; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Provides-Extra: doc
 Requires-Dist: numpydoc; extra == "doc"
 Requires-Dist: sphinx; extra == "doc"
 Requires-Dist: sphinx-automodapi; extra == "doc"
 Requires-Dist: sphinx-mdinclude; extra == "doc"
-Requires-Dist: pydata-sphinx-theme; extra == "doc"
+Requires-Dist: pydata-sphinx-theme<0.15.2; extra == "doc"
 Requires-Dist: sphinxcontrib-bibtex; extra == "doc"
 Requires-Dist: docutils>=0.20; extra == "doc"
 Requires-Dist: nbsphinx; extra == "doc"
 Requires-Dist: nbstripout; extra == "doc"
 Requires-Dist: jupytext; extra == "doc"
 Requires-Dist: ipykernel; extra == "doc"
 Requires-Dist: sphinx-gallery; extra == "doc"
@@ -53,57 +53,72 @@
 Requires-Dist: setuptools_scm; extra == "dev"
 Provides-Extra: all
 Requires-Dist: iop4[dev,doc,test]; extra == "all"
 
 <div>
 <a href="https://github.com/juanep97/iop4/actions/workflows/ci.yml"><img alt="CI" src="https://github.com/juanep97/iop4/actions/workflows/ci.yml/badge.svg"></img></a>
 <a href="https://zenodo.org/doi/10.5281/zenodo.10222722"><img src="https://zenodo.org/badge/636786270.svg" alt="DOI"></img></a>
+<a href="https://pypi.org/project/iop4/"><img src="https://img.shields.io/pypi/v/iop4" alt="PyPI"></img></a>
 </div>
 
 
 **IOP4** is a complete rewrite of IOP3, a pipeline to work with **photometry** and **polarimetry** of **optical data** from [CAHA](https://www.caha.es/es/) and [OSN](https://www.osn.iaa.csic.es/) observatories. It is built to ease debugging and inspection of data.
 
-IOP4 implements _Object Relational Mapping_ (**ORM**) to seamlessly integrate all information about the reduction and results in a database which can be used to query and plot results, flag data and inspect the reduction process in a integrated fashion with the whole pipeline. It also ships with an already **built-in web interface** which can be used out of the box to browse the database and supervise all pipeline processes.
+IOP4 implements _Object Relational Mapping_ (**ORM**) to seamlessly integrate all information about the reduction and results in a database which can be used to query and plot results, flag data and inspect the reduction process in an integrated fashion with the whole pipeline. It also ships with an already **built-in web interface** which can be used out of the box to browse the database and supervise all pipeline processes.
 
 
 ## Installation
+We recommend installing IOP4 in an isolated environtment as described below. IOP4 is hosted in [PyPI software repository](https://pypi.org/project/iop4/).
 
 ### Option 1: Using a virtual environment
 
 **Note:** IOP4 requires Python 3.10 or later. You can check your Python version with `python --version`. If you have a compatible version, you can skip this step.
   
 If you don't have Python 3.10 or later, you can install [pyenv](https://github.com/pyenv/pyenv) and [pyenv-virtualenv](https://github.com/pyenv/pyenv-virtualenv), which will manage python versions for you. You can use the automatic installer [pyenv-installer](https://github.com/pyenv/pyenv-installer):
 
 ```bash
     $ curl https://pyenv.run | bash
 ```
 
-Follow the instruction that these command output to add `pyenv` to `PATH` (or copy the commands from https://github.com/pyenv/pyenv for your shell). Restart your terminal, or source the file (e.g. `. ~/.bashrc` or `. ~/.zshrc`) Then, run 
+Follow the instructions that this command outputs to add `pyenv` to `PATH` (or copy the commands from https://github.com/pyenv/pyenv for your shell). Restart your terminal, or source the file (e.g. `. ~/.bashrc` or `. ~/.zshrc`) Then, run 
 ```bash 
     $ pyenv install 3.10
     $ pyenv virtualenv 3.10 iop4-venv
     $ pyenv activate iop4-venv
 ```
 Now you will have a virtual environment with the right Python version, and you can continue with the next step. To deactivate, just run `pyenv deactivate`.
 
-Now you can clone this repository and install IOP4:
+With the environment activated, you can install IOP4 latest version by running:
+```bash
+    $ pip install iop4
+```
+
+Alternatively, you can clone this repository and install IOP4:
 ```bash
     $ git clone 'git@github.com:juanep97/iop4.git'
     $ cd iop4
     $ pip install .
 ```
 or `pip install -e .` if you want to install it in developer mode.
 
 
-### Option 2: Using conda
-
-Clone this repository and run from a terminal
+### Option 2: Using conda/mamba
+As the previous option, create and activate the environment as follows:
 ```bash
     $ conda create -n iop4 python=3.10
     $ conda activate iop4
+```
+
+Then run:
+```bash
+    $ pip install iop4
+```
+
+Alternatively, you can also clone this repository and run (inside the root directory of the cloned repository):
+```bash
     $ pip install .
 ```
 or `pip install -e .` if you want to install it in developer mode.
 
 If you followed the steps in any of the two options above, you will have installed the module `iop4lib` and the `iop4` command, and the `iop4site` project. 
 
 ## Configuration
@@ -204,30 +219,31 @@
 
 ## Contribute
 
 You are welcome to contribute to IOP4. Fork and create a PR!
 
 ## Citing IOP4
 
-If you use IOP4, or any result derived with it, we kindly ask you to cite the following references:
+If you use IOP4, or any result derived from it, we kindly ask you to cite the following references:
 
 <div>
 <a href="https://zenodo.org/doi/10.5281/zenodo.10222722"><img src="https://zenodo.org/badge/636786270.svg" alt="DOI"></img></a>
 </div>
 
 You can use the following BibTeX entry:
 
 ```bibtex
-@software{juan_escudero_2023_10222723,
-  author       = {Juan Escudero and
-                  Daniel Morcuende},
-  title        = {juanep97/iop4: v0.1.0},
-  month        = nov,
-  year         = 2023,
+@software{escudero_pedrosa_2024_10845509,
+  author       = {Escudero Pedrosa, Juan and
+                  Morcuende Parrilla, Daniel and
+                  Otero-Santos, Jorge},
+  title        = {IOP4},
+  month        = mar,
+  year         = 2024,
   publisher    = {Zenodo},
-  version      = {v0.1.0},
-  doi          = {10.5281/zenodo.10222723},
-  url          = {https://doi.org/10.5281/zenodo.10222723}
+  version      = {v1.0.0},
+  doi          = {10.5281/zenodo.10222722},
+  url          = {https://zenodo.org/doi/10.5281/zenodo.10222722}
 }
 ```
 
 This might change in the future, as IOP4 is still under the process of being published in a peer-reviewed journal. Check this repository for updates :)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iop4 Version: 1.0.0 Summary: A rewrite of IOP3, a
+Metadata-Version: 2.1 Name: iop4 Version: 1.1.0 Summary: A rewrite of IOP3, a
 pipeline to work with photometry and polarimetry of optical data from CAHA and
 OSN. Author-email: Juan Escudero Pedrosa
 iaa.es> License: BSD-3-Clause Project-URL: repository, https://github.com/
 juanep97/iop4 Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: BSD License Classifier: Operating System :: OS
 Independent Requires-Python: <=3.12,>3.10 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: numpy==1.24.2 Requires-Dist:
@@ -14,54 +14,60 @@
 multiprocess==0.70.14 Requires-Dist: pypandoc Requires-Dist: termcolor
 Requires-Dist: pyyaml<5.4 Requires-Dist: psutil Provides-Extra: test Requires-
 Dist: pytest; extra == "test" Requires-Dist: pytest-django; extra == "test"
 Requires-Dist: codecov; extra == "test" Requires-Dist: pytest-cov; extra ==
 "test" Provides-Extra: doc Requires-Dist: numpydoc; extra == "doc" Requires-
 Dist: sphinx; extra == "doc" Requires-Dist: sphinx-automodapi; extra == "doc"
 Requires-Dist: sphinx-mdinclude; extra == "doc" Requires-Dist: pydata-sphinx-
-theme; extra == "doc" Requires-Dist: sphinxcontrib-bibtex; extra == "doc"
-Requires-Dist: docutils>=0.20; extra == "doc" Requires-Dist: nbsphinx; extra ==
-"doc" Requires-Dist: nbstripout; extra == "doc" Requires-Dist: jupytext; extra
-== "doc" Requires-Dist: ipykernel; extra == "doc" Requires-Dist: sphinx-
-gallery; extra == "doc" Requires-Dist: myst-nb; extra == "doc" Provides-Extra:
-dev Requires-Dist: setuptools_scm; extra == "dev" Provides-Extra: all Requires-
-Dist: iop4[dev,doc,test]; extra == "all"
-_[_C_I_]_[_D_O_I_]
+theme<0.15.2; extra == "doc" Requires-Dist: sphinxcontrib-bibtex; extra ==
+"doc" Requires-Dist: docutils>=0.20; extra == "doc" Requires-Dist: nbsphinx;
+extra == "doc" Requires-Dist: nbstripout; extra == "doc" Requires-Dist:
+jupytext; extra == "doc" Requires-Dist: ipykernel; extra == "doc" Requires-
+Dist: sphinx-gallery; extra == "doc" Requires-Dist: myst-nb; extra == "doc"
+Provides-Extra: dev Requires-Dist: setuptools_scm; extra == "dev" Provides-
+Extra: all Requires-Dist: iop4[dev,doc,test]; extra == "all"
+_[_C_I_]_[_D_O_I_]_[_P_y_P_I_]
 **IOP4** is a complete rewrite of IOP3, a pipeline to work with **photometry**
 and **polarimetry** of **optical data** from [CAHA](https://www.caha.es/es/
 ) and [OSN](https://www.osn.iaa.csic.es/) observatories. It is built to ease
 debugging and inspection of data. IOP4 implements _Object Relational Mapping_
 (**ORM**) to seamlessly integrate all information about the reduction and
 results in a database which can be used to query and plot results, flag data
-and inspect the reduction process in a integrated fashion with the whole
+and inspect the reduction process in an integrated fashion with the whole
 pipeline. It also ships with an already **built-in web interface** which can be
 used out of the box to browse the database and supervise all pipeline
-processes. ## Installation ### Option 1: Using a virtual environment **Note:**
-IOP4 requires Python 3.10 or later. You can check your Python version with
-`python --version`. If you have a compatible version, you can skip this step.
-If you don't have Python 3.10 or later, you can install [pyenv](https://
+processes. ## Installation We recommend installing IOP4 in an isolated
+environtment as described below. IOP4 is hosted in [PyPI software repository]
+(https://pypi.org/project/iop4/). ### Option 1: Using a virtual environment
+**Note:** IOP4 requires Python 3.10 or later. You can check your Python version
+with `python --version`. If you have a compatible version, you can skip this
+step. If you don't have Python 3.10 or later, you can install [pyenv](https://
 github.com/pyenv/pyenv) and [pyenv-virtualenv](https://github.com/pyenv/pyenv-
 virtualenv), which will manage python versions for you. You can use the
 automatic installer [pyenv-installer](https://github.com/pyenv/pyenv-
-installer): ```bash $ curl https://pyenv.run | bash ``` Follow the instruction
-that these command output to add `pyenv` to `PATH` (or copy the commands from
+installer): ```bash $ curl https://pyenv.run | bash ``` Follow the instructions
+that this command outputs to add `pyenv` to `PATH` (or copy the commands from
 https://github.com/pyenv/pyenv for your shell). Restart your terminal, or
 source the file (e.g. `. ~/.bashrc` or `. ~/.zshrc`) Then, run ```bash $ pyenv
 install 3.10 $ pyenv virtualenv 3.10 iop4-venv $ pyenv activate iop4-venv ```
 Now you will have a virtual environment with the right Python version, and you
 can continue with the next step. To deactivate, just run `pyenv deactivate`.
-Now you can clone this repository and install IOP4: ```bash $ git clone
-'git@github.com:juanep97/iop4.git' $ cd iop4 $ pip install . ``` or `pip
-install -e .` if you want to install it in developer mode. ### Option 2: Using
-conda Clone this repository and run from a terminal ```bash $ conda create -
-n iop4 python=3.10 $ conda activate iop4 $ pip install . ``` or `pip install -
-e .` if you want to install it in developer mode. If you followed the steps in
-any of the two options above, you will have installed the module `iop4lib` and
-the `iop4` command, and the `iop4site` project. ## Configuration After
-installation, take a look at the example configuration file (`config/
+With the environment activated, you can install IOP4 latest version by running:
+```bash $ pip install iop4 ``` Alternatively, you can clone this repository and
+install IOP4: ```bash $ git clone 'git@github.com:juanep97/iop4.git' $ cd iop4
+$ pip install . ``` or `pip install -e .` if you want to install it in
+developer mode. ### Option 2: Using conda/mamba As the previous option, create
+and activate the environment as follows: ```bash $ conda create -n iop4
+python=3.10 $ conda activate iop4 ``` Then run: ```bash $ pip install iop4 ```
+Alternatively, you can also clone this repository and run (inside the root
+directory of the cloned repository): ```bash $ pip install . ``` or `pip
+install -e .` if you want to install it in developer mode. If you followed the
+steps in any of the two options above, you will have installed the module
+`iop4lib` and the `iop4` command, and the `iop4site` project. ## Configuration
+After installation, take a look at the example configuration file (`config/
 config.example.yaml`), set the appropriate variables (path to the database,
 data directory, astrometry index files path, credentials, etc) and rename it to
 `config/config.yaml`. ### Running Tests To run the tests, first follow the
 previous steps to configure IOP4. At the moment, you will also need to download
 the `iop4testdata.tar.gz` file manually and place it under your home directory.
 Then, run ```bash $ pytest -vxs tests/ ``` If it is the first time executing
 IOP4, the astrometry index files will be downloaded to `astrometry_cache_path`
@@ -109,17 +115,17 @@
 %autoreload all import iop4lib.config iop4conf = iop4lib.Config(config_db=True,
 gonogui=False, jupytermode=True) ``` ### Tips You can get an IPython
 interactive terminal after running iop4 using the `-i` option. You can override
 any config option using the `-o` option, e.g.: ```bash $ iop4 -i -o nthreads=20
 -o log_file=test.log --epoch-list T090/230313 T090/230317 ``` ## Documentation
 To build and show the documentation, run ```bash $ make docs-sphinx $ make
 docs-show ``` ## Contribute You are welcome to contribute to IOP4. Fork and
-create a PR! ## Citing IOP4 If you use IOP4, or any result derived with it, we
+create a PR! ## Citing IOP4 If you use IOP4, or any result derived from it, we
 kindly ask you to cite the following references:
 _[_D_O_I_]
 You can use the following BibTeX entry: ```bibtex @software
-{juan_escudero_2023_10222723, author = {Juan Escudero and Daniel Morcuende},
-title = {juanep97/iop4: v0.1.0}, month = nov, year = 2023, publisher =
-{Zenodo}, version = {v0.1.0}, doi = {10.5281/zenodo.10222723}, url = {https://
-doi.org/10.5281/zenodo.10222723} } ``` This might change in the future, as IOP4
-is still under the process of being published in a peer-reviewed journal. Check
-this repository for updates :)
+{escudero_pedrosa_2024_10845509, author = {Escudero Pedrosa, Juan and Morcuende
+Parrilla, Daniel and Otero-Santos, Jorge}, title = {IOP4}, month = mar, year =
+2024, publisher = {Zenodo}, version = {v1.0.0}, doi = {10.5281/
+zenodo.10222722}, url = {https://zenodo.org/doi/10.5281/zenodo.10222722} } ```
+This might change in the future, as IOP4 is still under the process of being
+published in a peer-reviewed journal. Check this repository for updates :)
```

### Comparing `iop4-1.0.0/iop4.egg-info/SOURCES.txt` & `iop4-1.1.0/iop4.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4.egg-info/requires.txt` & `iop4-1.1.0/iop4.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 setuptools_scm
 
 [doc]
 numpydoc
 sphinx
 sphinx-automodapi
 sphinx-mdinclude
-pydata-sphinx-theme
+pydata-sphinx-theme<0.15.2
 sphinxcontrib-bibtex
 docutils>=0.20
 nbsphinx
 nbstripout
 jupytext
 ipykernel
 sphinx-gallery
```

### Comparing `iop4-1.0.0/iop4admin/modeladmins/aperphotresult.py` & `iop4-1.1.0/iop4admin/modeladmins/aperphotresult.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4admin/modeladmins/astrosource.py` & `iop4-1.1.0/iop4admin/modeladmins/astrosource.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4admin/modeladmins/epoch.py` & `iop4-1.1.0/iop4admin/modeladmins/epoch.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4admin/modeladmins/fitfile.py` & `iop4-1.1.0/iop4admin/modeladmins/fitfile.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4admin/modeladmins/masterbias.py` & `iop4-1.1.0/iop4admin/modeladmins/masterbias.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4admin/modeladmins/masterdark.py` & `iop4-1.1.0/iop4admin/modeladmins/masterdark.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4admin/modeladmins/masterflat.py` & `iop4-1.1.0/iop4admin/modeladmins/masterflat.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4admin/modeladmins/photopolresult.py` & `iop4-1.1.0/iop4admin/modeladmins/photopolresult.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4admin/modeladmins/rawfit.py` & `iop4-1.1.0/iop4admin/modeladmins/rawfit.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4admin/modeladmins/reducedfit.py` & `iop4-1.1.0/iop4admin/modeladmins/reducedfit.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4admin/sites.py` & `iop4-1.1.0/iop4admin/sites.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4admin/templates/iop4admin/fits/change_list.html` & `iop4-1.1.0/iop4admin/templates/iop4admin/fits/change_list.html`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4admin/templates/iop4admin/fits/textinput_filter.html` & `iop4-1.1.0/iop4admin/templates/iop4admin/fits/textinput_filter.html`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4admin/templates/iop4admin/view_astrosourcedetails.html` & `iop4-1.1.0/iop4admin/templates/iop4admin/view_astrosourcedetails.html`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4admin/templates/iop4admin/view_epochdetails.html` & `iop4-1.1.0/iop4admin/templates/iop4admin/view_epochdetails.html`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4admin/templates/iop4admin/view_fitdetails.html` & `iop4-1.1.0/iop4admin/templates/iop4admin/view_fitdetails.html`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4admin/templates/iop4admin/view_fitviewer.html` & `iop4-1.1.0/iop4admin/templates/iop4admin/view_fitviewer.html`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4admin/views/astrosource.py` & `iop4-1.1.0/iop4admin/views/astrosource.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4admin/views/epoch.py` & `iop4-1.1.0/iop4admin/views/epoch.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4admin/views/fitfile.py` & `iop4-1.1.0/iop4admin/views/fitfile.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4admin/views/singleobj.py` & `iop4-1.1.0/iop4admin/views/singleobj.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4api/filters.py` & `iop4-1.1.0/iop4api/filters.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4api/static/iop4api/base.css` & `iop4-1.1.0/iop4api/static/iop4api/base.css`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4api/static/iop4api/gui.js` & `iop4-1.1.0/iop4api/static/iop4api/gui.js`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4api/templates/iop4api/about.html` & `iop4-1.1.0/iop4api/templates/iop4api/about.html`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4api/templates/iop4api/data.html` & `iop4-1.1.0/iop4api/templates/iop4api/data.html`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4api/templates/iop4api/explore.html` & `iop4-1.1.0/iop4api/templates/iop4api/explore.html`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4api/templates/iop4api/index.html` & `iop4-1.1.0/iop4api/templates/iop4api/index.html`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4api/templates/iop4api/login.html` & `iop4-1.1.0/iop4api/templates/iop4api/login.html`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4api/templates/iop4api/logs.html` & `iop4-1.1.0/iop4api/templates/iop4api/logs.html`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4api/templates/iop4api/plot.html` & `iop4-1.1.0/iop4api/templates/iop4api/plot.html`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4api/templates/iop4api/query.html` & `iop4-1.1.0/iop4api/templates/iop4api/query.html`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4api/urls.py` & `iop4-1.1.0/iop4api/urls.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4api/views/__init__.py` & `iop4-1.1.0/iop4api/views/__init__.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4api/views/auth.py` & `iop4-1.1.0/iop4api/views/auth.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4api/views/catalog.py` & `iop4-1.1.0/iop4api/views/catalog.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4api/views/data.py` & `iop4-1.1.0/iop4api/views/data.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4api/views/docs.py` & `iop4-1.1.0/iop4api/views/docs.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4api/views/flag.py` & `iop4-1.1.0/iop4api/views/flag.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4api/views/index.py` & `iop4-1.1.0/iop4api/views/index.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4api/views/log.py` & `iop4-1.1.0/iop4api/views/log.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4api/views/plot.py` & `iop4-1.1.0/iop4api/views/plot.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4lib/config.py` & `iop4-1.1.0/iop4lib/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -135,14 +135,19 @@
                 setattr(self, k, str(pathlib.Path(v).expanduser()))
 
         # If data dir does not exist, create it
         
         if not os.path.exists(self.datadir):
             os.makedirs(self.datadir)
 
+        # Check if the logs subdirectory exists, if not, create it
+        
+        if not os.path.exists(os.path.join(self.datadir, "logs")):
+            os.makedirs(os.path.join(self.datadir, "logs"))
+
         # Load OSN names from external file if indicated, load them into patterns like name*.fit, name*.fits, or name*.fts.
 
         if self.osn_source_list_path is not None and os.path.exists(self.osn_source_list_path):
             with open(self.osn_source_list_path, 'r') as f:
                 self.osn_fnames_patterns += [fr"(^{s[:-1]}.*\.fi?ts?$)" for s in f.readlines() if s[0] != '#']
 
         if config_logging:
```

### Comparing `iop4-1.0.0/iop4lib/db/aperphotresult.py` & `iop4-1.1.0/iop4lib/db/aperphotresult.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4lib/db/astrosource.py` & `iop4-1.1.0/iop4lib/db/astrosource.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4lib/db/epoch.py` & `iop4-1.1.0/iop4lib/db/epoch.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4lib/db/fields.py` & `iop4-1.1.0/iop4lib/db/fields.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4lib/db/fitfilemodel.py` & `iop4-1.1.0/iop4lib/db/fitfilemodel.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4lib/db/masterbias.py` & `iop4-1.1.0/iop4lib/db/masterbias.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4lib/db/masterdark.py` & `iop4-1.1.0/iop4lib/db/masterdark.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4lib/db/masterflat.py` & `iop4-1.1.0/iop4lib/db/masterflat.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4lib/db/photopolresult.py` & `iop4-1.1.0/iop4lib/db/photopolresult.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4lib/db/rawfit.py` & `iop4-1.1.0/iop4lib/db/rawfit.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4lib/db/reducedfit.py` & `iop4-1.1.0/iop4lib/db/reducedfit.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4lib/enums.py` & `iop4-1.1.0/iop4lib/enums.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4lib/instruments/cafos.py` & `iop4-1.1.0/iop4lib/instruments/cafos.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,18 +92,24 @@
         There are also images in the archive with INSFLNAM = 'John V' and INSFLNAM = 'John I', and INSFLNAM = 'free'
         """
 
         from iop4lib.db.rawfit import RawFit
         import astropy.io.fits as fits
 
         if 'INSFLNAM' in rawfit.header:
-            if (rawfit.header['INSFLNAM'] == 'BessellR' or 
-                rawfit.header['INSFLNAM'] == 'John R' or 
-                rawfit.header['INSFLNAM'] == 'Cous R' or rawfit.header['INSFLNAM'] == 'CousinsR'):
+            if any([rawfit.header['INSFLNAM'] == kw for kw in ['BessellR', 'John R', 'Cous R', 'CousinsR', 'JohnsonR']]):
                 rawfit.band = BANDS.R
+            elif any([rawfit.header['INSFLNAM'] == kw for kw in ['BessellI', 'John I', 'Cous I', 'CousinsI', 'JohnsonI']]):
+                rawfit.band = BANDS.I
+            elif any([rawfit.header['INSFLNAM'] == kw for kw in ['BessellV', 'John V', 'Cous V', 'CousinsV', 'JohnsonV']]):
+                rawfit.band = BANDS.V
+            elif any([rawfit.header['INSFLNAM'] == kw for kw in ['BessellB', 'John B', 'Cous B', 'CousinsB', 'JohnsonB']]):
+                rawfit.band = BANDS.B
+            elif any([rawfit.header['INSFLNAM'] == kw for kw in ['BessellU', 'John U', 'Cous U', 'CousinsU', 'JohnsonU']]):
+                rawfit.band = BANDS.U
             else:
                 logger.error(f"{rawfit}: unknown filter {rawfit.header['INSFLNAM']}.")
                 rawfit.band = BANDS.ERROR
                 raise ValueError(f"{rawfit}: unknown filter {rawfit.header['INSFLNAM']}.")
         else: 
             rawfit.band = BANDS.ERROR
             raise ValueError(f"{rawfit}: INSFLNAM keyword not present.")
@@ -122,14 +128,16 @@
 
         if rawfit.header['INSTRMOD'] == 'Polarizer' and rawfit.header['INSPOFPI'] == 'Wollaston':
             rawfit.obsmode = OBSMODES.POLARIMETRY
             rawfit.rotangle = float(rawfit.header['INSPOROT'])
 
             if rawfit.imgtype == IMGTYPES.BIAS:
                 logger.debug(f"Probably not important, but {rawfit.fileloc} is BIAS but has polarimetry keywords, does it makes sense?")
+        elif rawfit.header['INSTRMOD'] == 'Polarizer' and rawfit.header['INSPOFPI'] == 'FREE':
+            rawfit.obsmode = OBSMODES.PHOTOMETRY
         else:
             logger.error("Not implemented, please check the code.")
 
     @classmethod
     def get_header_hintcoord(cls, rawfit):
         """ Get the position hint from the FITS header as a coordinate.
```

### Comparing `iop4-1.0.0/iop4lib/instruments/dipol.py` & `iop4-1.1.0/iop4lib/instruments/dipol.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4lib/instruments/dipol_astrometry.yaml` & `iop4-1.1.0/iop4lib/instruments/dipol_astrometry.yaml`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4lib/instruments/instrument.py` & `iop4-1.1.0/iop4lib/instruments/instrument.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4lib/instruments/osn_cameras.py` & `iop4-1.1.0/iop4lib/instruments/osn_cameras.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4lib/iop4.py` & `iop4-1.1.0/iop4lib/iop4.py`

 * *Files 2% similar despite different names*

```diff
@@ -228,15 +228,15 @@
     for override in overrides:
         key, value = override.split('=')
         config[key] = value
 
     # correct the type of the config options
     for k, v in config.items():
         # interpret the log_level option
-        if k == "log_level":
+        if k == "log_level" and not v.isnumeric():
             v = config[k] = getattr(logging, v.upper())
         # check the type of the config option, if it is an int, convert it
         if k in iop4conf and isinstance(iop4conf[k], int):
             config[k] = int(v)
             
     return config
```

### Comparing `iop4-1.0.0/iop4lib/iop4_night_summary.html` & `iop4-1.1.0/iop4lib/iop4_night_summary.html`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4lib/iop4_night_summary.py` & `iop4-1.1.0/iop4lib/iop4_night_summary.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,14 +171,15 @@
     """ Send the html summary by email."""
 
     msg = email.message.EmailMessage()
 
     msg['Subject'] = f"IOP4 summary {args.date}"
     msg['From'] = args.fromaddr 
     msg['To'] = args.mailto
+    msg['reply-to'] = args.contact_email
     msg.set_content(summary_html, subtype="html")
 
     logger.debug("Sending email")
 
     with smtplib.SMTP('localhost') as s:
         s.send_message(msg)
```

### Comparing `iop4-1.0.0/iop4lib/telescopes/cahat220.py` & `iop4-1.1.0/iop4lib/telescopes/cahat220.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4lib/telescopes/osnt090.py` & `iop4-1.1.0/iop4lib/telescopes/osnt090.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4lib/telescopes/osnt150.py` & `iop4-1.1.0/iop4lib/telescopes/osnt150.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4lib/telescopes/telescope.py` & `iop4-1.1.0/iop4lib/telescopes/telescope.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4lib/utils/__init__.py` & `iop4-1.1.0/iop4lib/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4lib/utils/astrometry.py` & `iop4-1.1.0/iop4lib/utils/astrometry.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4lib/utils/filedproperty.py` & `iop4-1.1.0/iop4lib/utils/filedproperty.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4lib/utils/host_correction_data.csv` & `iop4-1.1.0/iop4lib/utils/host_correction_data.csv`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4lib/utils/parallel.py` & `iop4-1.1.0/iop4lib/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4lib/utils/plotting.py` & `iop4-1.1.0/iop4lib/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4lib/utils/quadmatching.py` & `iop4-1.1.0/iop4lib/utils/quadmatching.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4lib/utils/sourcedetection.py` & `iop4-1.1.0/iop4lib/utils/sourcedetection.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4lib/utils/sourcepairing.py` & `iop4-1.1.0/iop4lib/utils/sourcepairing.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4lib/version.py` & `iop4-1.1.0/iop4lib/version.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4site/iop4site/settings.py` & `iop4-1.1.0/iop4site/iop4site/settings.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4site/iop4site/urls.py` & `iop4-1.1.0/iop4site/iop4site/urls.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4site/manage.py` & `iop4-1.1.0/iop4site/manage.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/iop4site/resetdb.py` & `iop4-1.1.0/iop4site/resetdb.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/pyproject.toml` & `iop4-1.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     "pytest-cov",
 ]
 doc = [
     "numpydoc",
     "sphinx",
     "sphinx-automodapi",
     "sphinx-mdinclude",
-    "pydata-sphinx-theme",
+    "pydata-sphinx-theme<0.15.2",
     "sphinxcontrib-bibtex",
     "docutils>=0.20",
     "nbsphinx",
     "nbstripout",
     "jupytext",
     "ipykernel",
     "sphinx-gallery",
```

### Comparing `iop4-1.0.0/tests/build_test_dataset.py` & `iop4-1.1.0/tests/build_test_dataset.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/tests/conftest.py` & `iop4-1.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/tests/fixtures.py` & `iop4-1.1.0/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/tests/test_caha_cafos.py` & `iop4-1.1.0/tests/test_caha_cafos.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/tests/test_generic.py` & `iop4-1.1.0/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/tests/test_osnt090_andor.py` & `iop4-1.1.0/tests/test_osnt090_andor.py`

 * *Files identical despite different names*

### Comparing `iop4-1.0.0/tests/test_osnt090_dipol.py` & `iop4-1.1.0/tests/test_osnt090_dipol.py`

 * *Files identical despite different names*

