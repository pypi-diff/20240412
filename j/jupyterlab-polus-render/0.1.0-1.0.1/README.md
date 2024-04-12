# Comparing `tmp/jupyterlab_polus_render-0.1.0.tar.gz` & `tmp/jupyterlab_polus_render-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterlab_polus_render-0.1.0.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `jupyterlab_polus_render-0.1.0.tar` & `jupyterlab_polus_render-1.0.1.tar`

### file list

```diff
@@ -1,6 +1,61 @@
--rw-r--r--   0        0        0     1074 2023-12-07 16:09:36.186259 jupyterlab_polus_render-0.1.0/LICENSE
--rw-r--r--   0        0        0     5623 2023-12-07 16:11:24.737110 jupyterlab_polus_render-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-12-07 16:09:36.411331 jupyterlab_polus_render-0.1.0/polus/__init__.py
--rw-r--r--   0        0        0     2709 2023-12-07 16:09:36.412316 jupyterlab_polus_render-0.1.0/polus/polus_render.py
--rw-r--r--   0        0        0      487 2023-12-07 18:36:47.666504 jupyterlab_polus_render-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     6301 1970-01-01 00:00:00.000000 jupyterlab_polus_render-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/.eslintignore
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/.eslintrc.js
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/.npmignore
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/.prettierignore
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/.prettierrc
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/.yarnrc.yml
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/MANIFEST.in
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/babel.config.js
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/install.json
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/jest.config.js
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/jupyterlab_polus_render.json
+-rw-r--r--   0        0        0     4067 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/package.json
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/setup.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/tsconfig.eslint.json
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/tsconfig.json
+-rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/webpack.config.js
+-rw-r--r--   0        0        0   379169 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/yarn.lock
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/css/widget.css
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/examples/intro.ipynb
+-rw-r--r--   0        0        0  4152900 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/images/image.png
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/jupyter-config/server-config/jupyterlab_polus_render.json
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/jupyterlab_polus_render/__init__.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/jupyterlab_polus_render/_frontend.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/jupyterlab_polus_render/_version.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/jupyterlab_polus_render/handlers.py
+-rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/jupyterlab_polus_render/render.py
+-rw-r--r--   0        0        0     4183 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/jupyterlab_polus_render/labextension/package.json
+-rw-r--r--   0        0        0     9908 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/jupyterlab_polus_render/labextension/static/122.3be7638fdd123cfe081f.js
+-rw-r--r--   0        0        0  2407145 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/jupyterlab_polus_render/labextension/static/227.68aed46569fe18401c29.js
+-rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/jupyterlab_polus_render/labextension/static/227.68aed46569fe18401c29.js.LICENSE.txt
+-rw-r--r--   0        0        0    23486 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/jupyterlab_polus_render/labextension/static/285.5e764e4155c3275578cb.js
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/jupyterlab_polus_render/labextension/static/285.5e764e4155c3275578cb.js.LICENSE.txt
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/jupyterlab_polus_render/labextension/static/359.7f6dcf75b8dac8108799.js
+-rw-r--r--   0        0        0    45941 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/jupyterlab_polus_render/labextension/static/501.128f3cca45f259356cd3.js
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/jupyterlab_polus_render/labextension/static/501.128f3cca45f259356cd3.js.LICENSE.txt
+-rw-r--r--   0        0        0     9484 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/jupyterlab_polus_render/labextension/static/509.03a69eab877004c42e01.js
+-rw-r--r--   0        0        0    12092 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/jupyterlab_polus_render/labextension/static/563.0f78313e7ba40f04be46.js
+-rw-r--r--   0        0        0    34234 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/jupyterlab_polus_render/labextension/static/574.c56b3d0e2b33f2396646.js
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/jupyterlab_polus_render/labextension/static/665.43d3ab6083cfaeef23a4.js
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/jupyterlab_polus_render/labextension/static/778.db9385935611d6411a63.js
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/jupyterlab_polus_render/labextension/static/811.b8ea280b183a962acd74.js
+-rw-r--r--   0        0        0    75477 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/jupyterlab_polus_render/labextension/static/895.4925b5772d35cdb0722d.js
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/jupyterlab_polus_render/labextension/static/943.9edb4058fc9ac473ed45.js
+-rw-r--r--   0        0        0     8946 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/jupyterlab_polus_render/labextension/static/961.070096ddc26d2e1b9c63.js
+-rw-r--r--   0        0        0     8138 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/jupyterlab_polus_render/labextension/static/remoteEntry.dd5a371026c79f77b0e0.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/jupyterlab_polus_render/labextension/static/style.js
+-rw-r--r--   0        0        0    60654 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/jupyterlab_polus_render/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/jupyterlab_polus_render/nbextension/extension.js
+-rw-r--r--   0        0        0  3281242 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/jupyterlab_polus_render/nbextension/index.js
+-rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/jupyterlab_polus_render/nbextension/index.js.LICENSE.txt
+-rw-r--r--   0        0        0  8377628 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/jupyterlab_polus_render/nbextension/index.js.map
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/src/extension.ts
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/src/index.ts
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/src/plugin.ts
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/src/version.ts
+-rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/src/widget.ts
+-rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/LICENSE.txt
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/README.md
+-rw-r--r--   0        0        0     3300 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     7293 2020-02-02 00:00:00.000000 jupyterlab_polus_render-1.0.1/PKG-INFO
```

### Comparing `jupyterlab_polus_render-0.1.0/LICENSE` & `jupyterlab_polus_render-1.0.1/LICENSE.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2023 LabShare
+Copyright (c) 2024 PolusAI
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

