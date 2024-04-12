# Comparing `tmp/rasterio-1.4a1.tar.gz` & `tmp/rasterio-1.4a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rasterio-1.4a1.tar", last modified: Fri Feb 16 00:42:26 2024, max compression
+gzip compressed data, was "rasterio-1.4a2.tar", last modified: Sun Mar  3 01:03:24 2024, max compression
```

## Comparing `rasterio-1.4a1.tar` & `rasterio-1.4a2.tar`

### file list

```diff
@@ -1,325 +1,325 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 00:42:26.299117 rasterio-1.4a1/
--rw-r--r--   0 root         (0) root         (0)     1990 2023-11-28 16:53:09.000000 rasterio-1.4a1/AUTHORS.txt
--rw-r--r--   0 root         (0) root         (0)    91051 2024-02-15 22:13:03.000000 rasterio-1.4a1/CHANGES.txt
--rw-r--r--   0 root         (0) root         (0)     1457 2023-11-28 16:53:09.000000 rasterio-1.4a1/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     7521 2024-02-16 00:42:26.299356 rasterio-1.4a1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6341 2024-01-16 23:55:08.000000 rasterio-1.4a1/README.rst
--rw-r--r--   0 root         (0) root         (0)        5 2024-02-16 00:42:25.000000 rasterio-1.4a1/VERSION.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 00:42:26.117827 rasterio-1.4a1/docs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 00:42:26.159705 rasterio-1.4a1/docs/api/
--rw-r--r--   0 root         (0) root         (0)       69 2023-11-28 16:53:09.000000 rasterio-1.4a1/docs/api/index.rst
--rw-r--r--   0 root         (0) root         (0)      135 2023-11-28 16:53:09.000000 rasterio-1.4a1/docs/api/rasterio._base.rst
--rw-r--r--   0 root         (0) root         (0)      132 2023-11-28 16:53:09.000000 rasterio-1.4a1/docs/api/rasterio._env.rst
--rw-r--r--   0 root         (0) root         (0)      132 2023-11-28 16:53:09.000000 rasterio-1.4a1/docs/api/rasterio._err.rst
--rw-r--r--   0 root         (0) root         (0)      144 2023-11-28 16:53:09.000000 rasterio-1.4a1/docs/api/rasterio._example.rst
--rw-r--r--   0 root         (0) root         (0)      147 2023-11-28 16:53:09.000000 rasterio-1.4a1/docs/api/rasterio._features.rst
--rw-r--r--   0 root         (0) root         (0)      165 2023-11-28 16:53:09.000000 rasterio-1.4a1/docs/api/rasterio._filepath.rst
--rw-r--r--   0 root         (0) root         (0)      135 2023-11-28 16:53:09.000000 rasterio-1.4a1/docs/api/rasterio._fill.rst
--rw-r--r--   0 root         (0) root         (0)      129 2023-11-28 16:53:09.000000 rasterio-1.4a1/docs/api/rasterio._io.rst
--rw-r--r--   0 root         (0) root         (0)      162 2023-11-28 16:53:09.000000 rasterio-1.4a1/docs/api/rasterio._loading.rst
--rw-r--r--   0 root         (0) root         (0)      168 2023-11-28 16:53:09.000000 rasterio-1.4a1/docs/api/rasterio._transform.rst
--rw-r--r--   0 root         (0) root         (0)      135 2023-11-28 16:53:09.000000 rasterio-1.4a1/docs/api/rasterio._warp.rst
--rw-r--r--   0 root         (0) root         (0)      139 2023-11-28 16:53:09.000000 rasterio-1.4a1/docs/api/rasterio.control.rst
--rw-r--r--   0 root         (0) root         (0)      136 2023-11-28 16:53:09.000000 rasterio-1.4a1/docs/api/rasterio.coords.rst
--rw-r--r--   0 root         (0) root         (0)      127 2023-11-28 16:53:09.000000 rasterio-1.4a1/docs/api/rasterio.crs.rst
--rw-r--r--   0 root         (0) root         (0)      139 2023-11-28 16:53:09.000000 rasterio-1.4a1/docs/api/rasterio.drivers.rst
--rw-r--r--   0 root         (0) root         (0)      136 2023-11-28 16:53:09.000000 rasterio-1.4a1/docs/api/rasterio.dtypes.rst
--rw-r--r--   0 root         (0) root         (0)      133 2023-11-28 16:53:09.000000 rasterio-1.4a1/docs/api/rasterio.enums.rst
--rw-r--r--   0 root         (0) root         (0)      147 2023-11-28 16:53:09.000000 rasterio-1.4a1/docs/api/rasterio.env.rst
--rw-r--r--   0 root         (0) root         (0)      136 2023-11-28 16:53:09.000000 rasterio-1.4a1/docs/api/rasterio.errors.rst
--rw-r--r--   0 root         (0) root         (0)      142 2023-11-28 16:53:09.000000 rasterio-1.4a1/docs/api/rasterio.features.rst
--rw-r--r--   0 root         (0) root         (0)      130 2023-11-28 16:53:09.000000 rasterio-1.4a1/docs/api/rasterio.fill.rst
--rw-r--r--   0 root         (0) root         (0)      144 2023-11-28 16:53:09.000000 rasterio-1.4a1/docs/api/rasterio.io.rst
--rw-r--r--   0 root         (0) root         (0)      130 2023-11-28 16:53:09.000000 rasterio-1.4a1/docs/api/rasterio.mask.rst
--rw-r--r--   0 root         (0) root         (0)      133 2023-11-28 16:53:09.000000 rasterio-1.4a1/docs/api/rasterio.merge.rst
--rw-r--r--   0 root         (0) root         (0)      130 2023-11-28 16:53:09.000000 rasterio-1.4a1/docs/api/rasterio.path.rst
--rw-r--r--   0 root         (0) root         (0)      130 2023-11-28 16:53:09.000000 rasterio-1.4a1/docs/api/rasterio.plot.rst
--rw-r--r--   0 root         (0) root         (0)      142 2023-11-28 16:53:09.000000 rasterio-1.4a1/docs/api/rasterio.profiles.rst
--rw-r--r--   0 root         (0) root         (0)       76 2023-11-28 18:25:20.000000 rasterio-1.4a1/docs/api/rasterio.rio.blocks.rst
--rw-r--r--   0 root         (0) root         (0)       76 2023-11-28 18:25:20.000000 rasterio-1.4a1/docs/api/rasterio.rio.bounds.rst
--rw-r--r--   0 root         (0) root         (0)       71 2023-11-28 18:25:20.000000 rasterio-1.4a1/docs/api/rasterio.rio.calc.rst
--rw-r--r--   0 root         (0) root         (0)       53 2023-11-28 18:25:20.000000 rasterio-1.4a1/docs/api/rasterio.rio.clip.rst
--rw-r--r--   0 root         (0) root         (0)       79 2023-11-28 18:25:20.000000 rasterio-1.4a1/docs/api/rasterio.rio.convert.rst
--rw-r--r--   0 root         (0) root         (0)       80 2023-11-28 18:25:20.000000 rasterio-1.4a1/docs/api/rasterio.rio.edit_info.rst
--rw-r--r--   0 root         (0) root         (0)       67 2023-11-28 18:25:20.000000 rasterio-1.4a1/docs/api/rasterio.rio.env.rst
--rw-r--r--   0 root         (0) root         (0)       70 2023-11-28 18:25:20.000000 rasterio-1.4a1/docs/api/rasterio.rio.gcps.rst
--rw-r--r--   0 root         (0) root         (0)       69 2023-11-28 18:25:20.000000 rasterio-1.4a1/docs/api/rasterio.rio.info.rst
--rw-r--r--   0 root         (0) root         (0)       70 2023-11-28 18:25:20.000000 rasterio-1.4a1/docs/api/rasterio.rio.insp.rst
--rw-r--r--   0 root         (0) root         (0)       70 2023-11-28 18:25:20.000000 rasterio-1.4a1/docs/api/rasterio.rio.mask.rst
--rw-r--r--   0 root         (0) root         (0)       73 2023-11-28 18:25:20.000000 rasterio-1.4a1/docs/api/rasterio.rio.merge.rst
--rw-r--r--   0 root         (0) root         (0)       82 2023-11-28 18:25:20.000000 rasterio-1.4a1/docs/api/rasterio.rio.overview.rst
--rw-r--r--   0 root         (0) root         (0)       85 2023-11-28 18:25:20.000000 rasterio-1.4a1/docs/api/rasterio.rio.rasterize.rst
--rw-r--r--   0 root         (0) root         (0)       64 2023-11-28 18:25:20.000000 rasterio-1.4a1/docs/api/rasterio.rio.rm.rst
--rw-r--r--   0 root         (0) root         (0)      533 2023-11-28 18:25:20.000000 rasterio-1.4a1/docs/api/rasterio.rio.rst
--rw-r--r--   0 root         (0) root         (0)       76 2023-11-28 18:25:20.000000 rasterio-1.4a1/docs/api/rasterio.rio.sample.rst
--rw-r--r--   0 root         (0) root         (0)       76 2023-11-28 18:25:20.000000 rasterio-1.4a1/docs/api/rasterio.rio.shapes.rst
--rw-r--r--   0 root         (0) root         (0)       74 2023-11-28 18:25:20.000000 rasterio-1.4a1/docs/api/rasterio.rio.stack.rst
--rw-r--r--   0 root         (0) root         (0)       85 2023-11-28 18:25:20.000000 rasterio-1.4a1/docs/api/rasterio.rio.transform.rst
--rw-r--r--   0 root         (0) root         (0)       70 2023-11-28 18:25:20.000000 rasterio-1.4a1/docs/api/rasterio.rio.warp.rst
--rw-r--r--   0 root         (0) root         (0)      132 2023-11-28 16:53:09.000000 rasterio-1.4a1/docs/api/rasterio.rpc.rst
--rw-r--r--   0 root         (0) root         (0)      744 2023-11-28 18:25:20.000000 rasterio-1.4a1/docs/api/rasterio.rst
--rw-r--r--   0 root         (0) root         (0)      136 2023-11-28 16:53:09.000000 rasterio-1.4a1/docs/api/rasterio.sample.rst
--rw-r--r--   0 root         (0) root         (0)      159 2023-11-28 16:53:09.000000 rasterio-1.4a1/docs/api/rasterio.session.rst
--rw-r--r--   0 root         (0) root         (0)      136 2023-11-28 16:53:09.000000 rasterio-1.4a1/docs/api/rasterio.shutil.rst
--rw-r--r--   0 root         (0) root         (0)      133 2023-11-28 16:53:09.000000 rasterio-1.4a1/docs/api/rasterio.tools.rst
--rw-r--r--   0 root         (0) root         (0)      145 2023-11-28 16:53:09.000000 rasterio-1.4a1/docs/api/rasterio.transform.rst
--rw-r--r--   0 root         (0) root         (0)      147 2023-11-28 16:53:09.000000 rasterio-1.4a1/docs/api/rasterio.vrt.rst
--rw-r--r--   0 root         (0) root         (0)      130 2023-11-28 16:53:09.000000 rasterio-1.4a1/docs/api/rasterio.warp.rst
--rw-r--r--   0 root         (0) root         (0)      136 2023-11-28 16:53:09.000000 rasterio-1.4a1/docs/api/rasterio.windows.rst
--rw-r--r--   0 root         (0) root         (0)    21803 2024-02-13 00:03:41.000000 rasterio-1.4a1/docs/cli.rst
--rw-r--r--   0 root         (0) root         (0)      407 2023-11-28 16:53:09.000000 rasterio-1.4a1/docs/contributing.rst
--rw-r--r--   0 root         (0) root         (0)     4552 2023-12-30 22:39:27.000000 rasterio-1.4a1/docs/faq.rst
--rw-r--r--   0 root         (0) root         (0)     1644 2023-11-28 16:53:09.000000 rasterio-1.4a1/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)     2771 2023-11-28 18:25:20.000000 rasterio-1.4a1/docs/installation.rst
--rw-r--r--   0 root         (0) root         (0)     2743 2023-11-28 16:53:09.000000 rasterio-1.4a1/docs/intro.rst
--rw-r--r--   0 root         (0) root         (0)    11398 2023-11-28 18:25:20.000000 rasterio-1.4a1/docs/quickstart.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 00:42:26.181399 rasterio-1.4a1/docs/topics/
--rw-r--r--   0 root         (0) root         (0)     3611 2023-11-28 16:53:09.000000 rasterio-1.4a1/docs/topics/calc.rst
--rw-r--r--   0 root         (0) root         (0)     2637 2023-11-28 18:25:20.000000 rasterio-1.4a1/docs/topics/color.rst
--rw-r--r--   0 root         (0) root         (0)     6267 2023-11-28 18:25:20.000000 rasterio-1.4a1/docs/topics/concurrency.rst
--rw-r--r--   0 root         (0) root         (0)     3379 2023-11-28 18:25:20.000000 rasterio-1.4a1/docs/topics/configuration.rst
--rw-r--r--   0 root         (0) root         (0)     1856 2023-11-28 18:25:20.000000 rasterio-1.4a1/docs/topics/datasets.rst
--rw-r--r--   0 root         (0) root         (0)     1419 2023-11-28 18:25:20.000000 rasterio-1.4a1/docs/topics/errors.rst
--rw-r--r--   0 root         (0) root         (0)     3498 2023-11-28 18:25:20.000000 rasterio-1.4a1/docs/topics/features.rst
--rw-r--r--   0 root         (0) root         (0)       78 2023-11-28 18:25:20.000000 rasterio-1.4a1/docs/topics/fillnodata.rst
--rw-r--r--   0 root         (0) root         (0)     4656 2023-11-28 18:25:20.000000 rasterio-1.4a1/docs/topics/georeferencing.rst
--rw-r--r--   0 root         (0) root         (0)     3066 2023-11-28 18:25:20.000000 rasterio-1.4a1/docs/topics/image_options.rst
--rw-r--r--   0 root         (0) root         (0)     1054 2023-11-28 16:53:09.000000 rasterio-1.4a1/docs/topics/image_processing.rst
--rw-r--r--   0 root         (0) root         (0)      443 2023-11-28 16:53:09.000000 rasterio-1.4a1/docs/topics/index.rst
--rw-r--r--   0 root         (0) root         (0)     1753 2023-11-28 18:25:20.000000 rasterio-1.4a1/docs/topics/masking-by-shapefile.rst
--rw-r--r--   0 root         (0) root         (0)     9188 2023-11-28 18:25:20.000000 rasterio-1.4a1/docs/topics/masks.rst
--rw-r--r--   0 root         (0) root         (0)     2925 2023-11-28 18:25:20.000000 rasterio-1.4a1/docs/topics/memory-files.rst
--rw-r--r--   0 root         (0) root         (0)     8374 2023-11-28 18:25:20.000000 rasterio-1.4a1/docs/topics/migrating-to-v1.rst
--rw-r--r--   0 root         (0) root         (0)     2092 2023-11-28 18:25:20.000000 rasterio-1.4a1/docs/topics/overviews.rst
--rw-r--r--   0 root         (0) root         (0)     3944 2023-11-28 18:25:20.000000 rasterio-1.4a1/docs/topics/plotting.rst
--rw-r--r--   0 root         (0) root         (0)     2307 2023-11-28 18:25:20.000000 rasterio-1.4a1/docs/topics/profiles.rst
--rw-r--r--   0 root         (0) root         (0)     4801 2023-11-28 18:25:20.000000 rasterio-1.4a1/docs/topics/reading.rst
--rw-r--r--   0 root         (0) root         (0)     8328 2023-12-30 22:37:11.000000 rasterio-1.4a1/docs/topics/reproject.rst
--rw-r--r--   0 root         (0) root         (0)     2265 2023-11-28 18:25:20.000000 rasterio-1.4a1/docs/topics/resampling.rst
--rw-r--r--   0 root         (0) root         (0)    13761 2023-11-28 18:25:20.000000 rasterio-1.4a1/docs/topics/switch.rst
--rw-r--r--   0 root         (0) root         (0)     2993 2023-11-28 18:25:20.000000 rasterio-1.4a1/docs/topics/tags.rst
--rw-r--r--   0 root         (0) root         (0)     4377 2023-11-28 18:25:20.000000 rasterio-1.4a1/docs/topics/transforms.rst
--rw-r--r--   0 root         (0) root         (0)     5888 2023-11-28 18:25:20.000000 rasterio-1.4a1/docs/topics/virtual-warping.rst
--rw-r--r--   0 root         (0) root         (0)     5056 2023-12-30 22:39:27.000000 rasterio-1.4a1/docs/topics/vsi.rst
--rw-r--r--   0 root         (0) root         (0)     8169 2023-11-28 18:25:20.000000 rasterio-1.4a1/docs/topics/windowed-rw.rst
--rw-r--r--   0 root         (0) root         (0)     2338 2023-11-28 18:25:20.000000 rasterio-1.4a1/docs/topics/writing.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 00:42:26.187390 rasterio-1.4a1/examples/
--rw-r--r--   0 root         (0) root         (0)     3247 2023-11-28 18:25:20.000000 rasterio-1.4a1/examples/async-rasterio.py
--rw-r--r--   0 root         (0) root         (0)      761 2023-11-28 16:53:09.000000 rasterio-1.4a1/examples/decimate.py
--rw-r--r--   0 root         (0) root         (0)      222 2023-11-28 16:53:09.000000 rasterio-1.4a1/examples/polygonize.py
--rw-r--r--   0 root         (0) root         (0)     1869 2023-11-28 16:53:09.000000 rasterio-1.4a1/examples/rasterio_polygonize.py
--rw-r--r--   0 root         (0) root         (0)      810 2023-11-28 16:53:09.000000 rasterio-1.4a1/examples/rasterize_geometry.py
--rw-r--r--   0 root         (0) root         (0)     1747 2023-11-28 16:53:09.000000 rasterio-1.4a1/examples/reproject.py
--rw-r--r--   0 root         (0) root         (0)     1154 2023-11-28 16:53:09.000000 rasterio-1.4a1/examples/sieve.py
--rw-r--r--   0 root         (0) root         (0)     2431 2023-11-28 18:25:20.000000 rasterio-1.4a1/examples/thread_pool_executor.py
--rw-r--r--   0 root         (0) root         (0)     1318 2023-11-28 16:53:09.000000 rasterio-1.4a1/examples/total.py
--rw-r--r--   0 root         (0) root         (0)      531 2024-02-14 18:25:56.000000 rasterio-1.4a1/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 00:42:26.204543 rasterio-1.4a1/rasterio/
--rw-r--r--   0 root         (0) root         (0)    16248 2024-02-15 22:09:51.000000 rasterio-1.4a1/rasterio/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1165 2023-11-28 16:53:09.000000 rasterio-1.4a1/rasterio/_base.pxd
--rw-r--r--   0 root         (0) root         (0)    46502 2024-02-13 00:03:41.000000 rasterio-1.4a1/rasterio/_base.pyx
--rw-r--r--   0 root         (0) root         (0)      155 2023-11-28 16:53:09.000000 rasterio-1.4a1/rasterio/_env.pxd
--rw-r--r--   0 root         (0) root         (0)    15368 2024-02-13 00:03:41.000000 rasterio-1.4a1/rasterio/_env.pyx
--rw-r--r--   0 root         (0) root         (0)      401 2024-02-13 00:03:41.000000 rasterio-1.4a1/rasterio/_err.pxd
--rw-r--r--   0 root         (0) root         (0)     9266 2024-02-13 00:03:41.000000 rasterio-1.4a1/rasterio/_err.pyx
--rw-r--r--   0 root         (0) root         (0)      804 2023-11-28 16:53:09.000000 rasterio-1.4a1/rasterio/_example.pyx
--rw-r--r--   0 root         (0) root         (0)     1479 2023-11-28 18:25:20.000000 rasterio-1.4a1/rasterio/_features.pxd
--rw-r--r--   0 root         (0) root         (0)    26598 2023-11-28 18:25:20.000000 rasterio-1.4a1/rasterio/_features.pyx
--rw-r--r--   0 root         (0) root         (0)      199 2023-11-28 16:53:09.000000 rasterio-1.4a1/rasterio/_filepath.pxd
--rw-r--r--   0 root         (0) root         (0)     8879 2023-12-30 22:39:27.000000 rasterio-1.4a1/rasterio/_filepath.pyx
--rw-r--r--   0 root         (0) root         (0)     1289 2023-11-28 16:53:09.000000 rasterio-1.4a1/rasterio/_fill.pyx
--rw-r--r--   0 root         (0) root         (0)      972 2023-11-28 16:53:09.000000 rasterio-1.4a1/rasterio/_io.pxd
--rw-r--r--   0 root         (0) root         (0)    87467 2024-02-13 02:04:33.000000 rasterio-1.4a1/rasterio/_io.pyx
--rw-r--r--   0 root         (0) root         (0)     5407 2023-11-28 16:53:09.000000 rasterio-1.4a1/rasterio/_path.py
--rw-r--r--   0 root         (0) root         (0)     2427 2024-01-02 16:19:52.000000 rasterio-1.4a1/rasterio/_show_versions.py
--rw-r--r--   0 root         (0) root         (0)    12533 2023-12-30 22:39:27.000000 rasterio-1.4a1/rasterio/_transform.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 00:42:26.092938 rasterio-1.4a1/rasterio/_vendor/
--rw-r--r--   0 root         (0) root         (0)       24 2024-02-15 22:09:51.000000 rasterio-1.4a1/rasterio/_vendor/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8141 2024-01-02 16:19:52.000000 rasterio-1.4a1/rasterio/_vendor/snuggs.py
--rw-r--r--   0 root         (0) root         (0)      502 2023-11-28 16:53:09.000000 rasterio-1.4a1/rasterio/_version.pxd
--rw-r--r--   0 root         (0) root         (0)     2171 2023-11-28 16:53:09.000000 rasterio-1.4a1/rasterio/_version.pyx
--rw-r--r--   0 root         (0) root         (0)      199 2023-12-30 22:37:11.000000 rasterio-1.4a1/rasterio/_vsiopener.pxd
--rw-r--r--   0 root         (0) root         (0)     7682 2024-02-15 22:09:43.000000 rasterio-1.4a1/rasterio/_vsiopener.pyx
--rw-r--r--   0 root         (0) root         (0)     1901 2023-11-28 16:53:09.000000 rasterio-1.4a1/rasterio/_warp.pxd
--rw-r--r--   0 root         (0) root         (0)    58992 2024-02-13 00:03:41.000000 rasterio-1.4a1/rasterio/_warp.pyx
--rw-r--r--   0 root         (0) root         (0)     2066 2023-11-28 16:53:09.000000 rasterio-1.4a1/rasterio/control.py
--rw-r--r--   0 root         (0) root         (0)     1450 2023-11-28 16:53:09.000000 rasterio-1.4a1/rasterio/coords.py
--rw-r--r--   0 root         (0) root         (0)      138 2023-11-28 16:53:09.000000 rasterio-1.4a1/rasterio/crs.pxd
--rw-r--r--   0 root         (0) root         (0)    33589 2023-12-30 22:39:27.000000 rasterio-1.4a1/rasterio/crs.pyx
--rw-r--r--   0 root         (0) root         (0)     1840 2023-11-28 18:25:20.000000 rasterio-1.4a1/rasterio/drivers.py
--rw-r--r--   0 root         (0) root         (0)     6296 2023-12-30 22:39:27.000000 rasterio-1.4a1/rasterio/dtypes.py
--rw-r--r--   0 root         (0) root         (0)     5550 2023-11-28 16:53:09.000000 rasterio-1.4a1/rasterio/enums.py
--rw-r--r--   0 root         (0) root         (0)    22489 2023-12-30 22:37:11.000000 rasterio-1.4a1/rasterio/env.py
--rw-r--r--   0 root         (0) root         (0)     4654 2024-02-13 00:03:41.000000 rasterio-1.4a1/rasterio/errors.py
--rw-r--r--   0 root         (0) root         (0)    23522 2024-02-15 22:10:59.000000 rasterio-1.4a1/rasterio/features.py
--rw-r--r--   0 root         (0) root         (0)     2742 2023-11-28 18:25:20.000000 rasterio-1.4a1/rasterio/fill.py
--rw-r--r--   0 root         (0) root         (0)    33114 2024-02-13 00:03:41.000000 rasterio-1.4a1/rasterio/gdal.pxi
--rw-r--r--   0 root         (0) root         (0)     8959 2023-12-30 22:39:27.000000 rasterio-1.4a1/rasterio/io.py
--rw-r--r--   0 root         (0) root         (0)     7562 2023-12-30 22:39:27.000000 rasterio-1.4a1/rasterio/mask.py
--rw-r--r--   0 root         (0) root         (0)    15261 2024-02-13 02:04:33.000000 rasterio-1.4a1/rasterio/merge.py
--rw-r--r--   0 root         (0) root         (0)      520 2023-11-28 16:53:09.000000 rasterio-1.4a1/rasterio/path.py
--rw-r--r--   0 root         (0) root         (0)    11135 2024-01-19 23:56:39.000000 rasterio-1.4a1/rasterio/plot.py
--rw-r--r--   0 root         (0) root         (0)     1343 2023-11-28 18:25:20.000000 rasterio-1.4a1/rasterio/profiles.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 00:42:26.112259 rasterio-1.4a1/rasterio/rio/
--rw-r--r--   0 root         (0) root         (0)       50 2023-11-28 16:53:09.000000 rasterio-1.4a1/rasterio/rio/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4876 2023-11-28 18:25:20.000000 rasterio-1.4a1/rasterio/rio/blocks.py
--rw-r--r--   0 root         (0) root         (0)     3770 2023-11-28 18:25:20.000000 rasterio-1.4a1/rasterio/rio/bounds.py
--rw-r--r--   0 root         (0) root         (0)     8322 2024-01-02 16:19:52.000000 rasterio-1.4a1/rasterio/rio/calc.py
--rw-r--r--   0 root         (0) root         (0)     6863 2023-11-28 18:25:20.000000 rasterio-1.4a1/rasterio/rio/clip.py
--rw-r--r--   0 root         (0) root         (0)     3395 2023-11-28 16:53:09.000000 rasterio-1.4a1/rasterio/rio/convert.py
--rw-r--r--   0 root         (0) root         (0)     5315 2024-02-13 00:03:41.000000 rasterio-1.4a1/rasterio/rio/create.py
--rw-r--r--   0 root         (0) root         (0)     8814 2023-12-30 22:39:27.000000 rasterio-1.4a1/rasterio/rio/edit_info.py
--rw-r--r--   0 root         (0) root         (0)     1410 2023-11-28 16:53:09.000000 rasterio-1.4a1/rasterio/rio/env.py
--rw-r--r--   0 root         (0) root         (0)     3784 2023-11-28 16:53:09.000000 rasterio-1.4a1/rasterio/rio/gcps.py
--rw-r--r--   0 root         (0) root         (0)     3598 2023-11-28 16:53:09.000000 rasterio-1.4a1/rasterio/rio/helpers.py
--rw-r--r--   0 root         (0) root         (0)     5321 2024-01-25 19:09:47.000000 rasterio-1.4a1/rasterio/rio/info.py
--rw-r--r--   0 root         (0) root         (0)     2748 2023-11-28 18:25:20.000000 rasterio-1.4a1/rasterio/rio/insp.py
--rw-r--r--   0 root         (0) root         (0)     3313 2023-11-28 18:25:20.000000 rasterio-1.4a1/rasterio/rio/main.py
--rw-r--r--   0 root         (0) root         (0)     4744 2023-11-28 16:53:09.000000 rasterio-1.4a1/rasterio/rio/mask.py
--rw-r--r--   0 root         (0) root         (0)     3268 2024-02-13 02:04:33.000000 rasterio-1.4a1/rasterio/rio/merge.py
--rw-r--r--   0 root         (0) root         (0)    12083 2024-02-13 00:03:41.000000 rasterio-1.4a1/rasterio/rio/options.py
--rw-r--r--   0 root         (0) root         (0)     4850 2023-11-28 18:25:20.000000 rasterio-1.4a1/rasterio/rio/overview.py
--rw-r--r--   0 root         (0) root         (0)    10082 2023-11-28 18:25:20.000000 rasterio-1.4a1/rasterio/rio/rasterize.py
--rw-r--r--   0 root         (0) root         (0)      946 2023-11-28 16:53:09.000000 rasterio-1.4a1/rasterio/rio/rm.py
--rw-r--r--   0 root         (0) root         (0)     2275 2023-11-28 16:53:09.000000 rasterio-1.4a1/rasterio/rio/sample.py
--rw-r--r--   0 root         (0) root         (0)     4310 2023-11-28 16:53:09.000000 rasterio-1.4a1/rasterio/rio/shapes.py
--rw-r--r--   0 root         (0) root         (0)     3959 2023-11-28 16:53:09.000000 rasterio-1.4a1/rasterio/rio/stack.py
--rw-r--r--   0 root         (0) root         (0)     2140 2023-11-28 18:25:20.000000 rasterio-1.4a1/rasterio/rio/transform.py
--rw-r--r--   0 root         (0) root         (0)    14847 2023-12-30 22:37:11.000000 rasterio-1.4a1/rasterio/rio/warp.py
--rw-r--r--   0 root         (0) root         (0)     4130 2023-11-28 18:25:20.000000 rasterio-1.4a1/rasterio/rpc.py
--rw-r--r--   0 root         (0) root         (0)     2800 2023-11-28 18:25:20.000000 rasterio-1.4a1/rasterio/sample.py
--rw-r--r--   0 root         (0) root         (0)    18259 2023-11-28 16:53:09.000000 rasterio-1.4a1/rasterio/session.py
--rw-r--r--   0 root         (0) root         (0)     7291 2023-11-28 16:53:09.000000 rasterio-1.4a1/rasterio/shutil.pyx
--rw-r--r--   0 root         (0) root         (0)     2205 2023-11-28 16:53:09.000000 rasterio-1.4a1/rasterio/tools.py
--rw-r--r--   0 root         (0) root         (0)    18324 2023-12-30 22:39:27.000000 rasterio-1.4a1/rasterio/transform.py
--rw-r--r--   0 root         (0) root         (0)    10871 2024-02-15 22:09:51.000000 rasterio-1.4a1/rasterio/vrt.py
--rw-r--r--   0 root         (0) root         (0)    21283 2023-12-30 22:39:27.000000 rasterio-1.4a1/rasterio/warp.py
--rw-r--r--   0 root         (0) root         (0)    23609 2024-02-13 02:04:33.000000 rasterio-1.4a1/rasterio/windows.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 00:42:26.209411 rasterio-1.4a1/rasterio.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7521 2024-02-16 00:42:25.000000 rasterio-1.4a1/rasterio.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7633 2024-02-16 00:42:26.000000 rasterio-1.4a1/rasterio.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-16 00:42:25.000000 rasterio-1.4a1/rasterio.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      797 2024-02-16 00:42:25.000000 rasterio-1.4a1/rasterio.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-08 16:53:08.000000 rasterio-1.4a1/rasterio.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      520 2024-02-16 00:42:25.000000 rasterio-1.4a1/rasterio.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-02-16 00:42:26.000000 rasterio-1.4a1/rasterio.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1387 2024-02-16 00:42:26.300163 rasterio-1.4a1/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)    11196 2024-02-15 22:09:51.000000 rasterio-1.4a1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 00:42:26.297247 rasterio-1.4a1/tests/
--rw-r--r--   0 root         (0) root         (0)      719 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/README.rst
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16778 2023-11-28 18:25:20.000000 rasterio-1.4a1/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 00:42:26.298337 rasterio-1.4a1/tests/data/
--rw-r--r--   0 root         (0) root         (0)      526 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/data/README.rst
--rw-r--r--   0 root         (0) root         (0)     3663 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/rangehttpserver.py
--rw-r--r--   0 root         (0) root         (0)     4241 2023-11-28 18:25:20.000000 rasterio-1.4a1/tests/test__env.py
--rw-r--r--   0 root         (0) root         (0)      755 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test__version.py
--rw-r--r--   0 root         (0) root         (0)      332 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_band.py
--rw-r--r--   0 root         (0) root         (0)     5468 2023-11-28 18:25:20.000000 rasterio-1.4a1/tests/test_band_masks.py
--rw-r--r--   0 root         (0) root         (0)     8149 2024-02-13 00:03:41.000000 rasterio-1.4a1/tests/test_blocks.py
--rw-r--r--   0 root         (0) root         (0)     7367 2023-11-28 18:25:20.000000 rasterio-1.4a1/tests/test_boundless_read.py
--rw-r--r--   0 root         (0) root         (0)     1767 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_checksum.py
--rw-r--r--   0 root         (0) root         (0)      562 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_cli_main.py
--rw-r--r--   0 root         (0) root         (0)     3062 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_colorinterp.py
--rw-r--r--   0 root         (0) root         (0)      964 2023-11-28 18:25:20.000000 rasterio-1.4a1/tests/test_colormap.py
--rw-r--r--   0 root         (0) root         (0)     2814 2023-11-28 18:25:20.000000 rasterio-1.4a1/tests/test_complex_dtypes.py
--rw-r--r--   0 root         (0) root         (0)     1378 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_coords.py
--rw-r--r--   0 root         (0) root         (0)      849 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_creation_options.py
--rw-r--r--   0 root         (0) root         (0)    21943 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_crs.py
--rw-r--r--   0 root         (0) root         (0)      344 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_data_paths.py
--rw-r--r--   0 root         (0) root         (0)     4548 2024-02-13 00:03:41.000000 rasterio-1.4a1/tests/test_dataset.py
--rw-r--r--   0 root         (0) root         (0)     6346 2023-11-28 18:25:20.000000 rasterio-1.4a1/tests/test_dataset_mask.py
--rw-r--r--   0 root         (0) root         (0)     2058 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_dataset_rw.py
--rw-r--r--   0 root         (0) root         (0)      431 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_deprecated.py
--rw-r--r--   0 root         (0) root         (0)     1018 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_descriptions.py
--rw-r--r--   0 root         (0) root         (0)     1413 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_driver_management.py
--rw-r--r--   0 root         (0) root         (0)      291 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_driver_policy.py
--rw-r--r--   0 root         (0) root         (0)     4659 2023-11-28 18:25:20.000000 rasterio-1.4a1/tests/test_dtypes.py
--rw-r--r--   0 root         (0) root         (0)      508 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_enums.py
--rw-r--r--   0 root         (0) root         (0)    36482 2023-12-30 22:37:11.000000 rasterio-1.4a1/tests/test_env.py
--rw-r--r--   0 root         (0) root         (0)     2662 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_err.py
--rw-r--r--   0 root         (0) root         (0)    37794 2024-01-16 23:55:08.000000 rasterio-1.4a1/tests/test_features.py
--rw-r--r--   0 root         (0) root         (0)     8517 2023-12-30 22:39:27.000000 rasterio-1.4a1/tests/test_filepath.py
--rw-r--r--   0 root         (0) root         (0)     1111 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_fillnodata.py
--rw-r--r--   0 root         (0) root         (0)     4712 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_gcps.py
--rw-r--r--   0 root         (0) root         (0)     3457 2023-11-28 18:25:20.000000 rasterio-1.4a1/tests/test_gdal_raster_io.py
--rw-r--r--   0 root         (0) root         (0)     1937 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_image_structure.py
--rw-r--r--   0 root         (0) root         (0)     9043 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_indexing.py
--rw-r--r--   0 root         (0) root         (0)     1576 2023-11-28 18:25:20.000000 rasterio-1.4a1/tests/test_int8.py
--rw-r--r--   0 root         (0) root         (0)     1004 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_io.py
--rw-r--r--   0 root         (0) root         (0)     3330 2023-11-28 18:25:20.000000 rasterio-1.4a1/tests/test_io_mixins.py
--rw-r--r--   0 root         (0) root         (0)    11380 2023-12-30 22:39:27.000000 rasterio-1.4a1/tests/test_mask.py
--rw-r--r--   0 root         (0) root         (0)     3335 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_mask_creation.py
--rw-r--r--   0 root         (0) root         (0)    16548 2023-12-30 22:39:27.000000 rasterio-1.4a1/tests/test_memoryfile.py
--rw-r--r--   0 root         (0) root         (0)     6530 2024-02-13 02:04:33.000000 rasterio-1.4a1/tests/test_merge.py
--rw-r--r--   0 root         (0) root         (0)      859 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_meta.py
--rw-r--r--   0 root         (0) root         (0)      914 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_no_georef.py
--rw-r--r--   0 root         (0) root         (0)     2977 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_nodata.py
--rw-r--r--   0 root         (0) root         (0)      908 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_open.py
--rw-r--r--   0 root         (0) root         (0)      810 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_open_options.py
--rw-r--r--   0 root         (0) root         (0)      597 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_open_overview_level.py
--rw-r--r--   0 root         (0) root         (0)     1439 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_open_sharing.py
--rw-r--r--   0 root         (0) root         (0)      507 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_options.py
--rw-r--r--   0 root         (0) root         (0)     5661 2023-11-28 18:25:20.000000 rasterio-1.4a1/tests/test_overviews.py
--rw-r--r--   0 root         (0) root         (0)      309 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_pad.py
--rw-r--r--   0 root         (0) root         (0)     7944 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_path.py
--rw-r--r--   0 root         (0) root         (0)     8772 2024-01-19 23:56:39.000000 rasterio-1.4a1/tests/test_plot.py
--rw-r--r--   0 root         (0) root         (0)      659 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_png.py
--rw-r--r--   0 root         (0) root         (0)      796 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_process_pool_executor.py
--rw-r--r--   0 root         (0) root         (0)     3536 2024-02-13 00:03:41.000000 rasterio-1.4a1/tests/test_profile.py
--rw-r--r--   0 root         (0) root         (0)     3727 2024-02-15 22:09:51.000000 rasterio-1.4a1/tests/test_pyopener.py
--rw-r--r--   0 root         (0) root         (0)    14849 2024-02-13 00:03:41.000000 rasterio-1.4a1/tests/test_read.py
--rw-r--r--   0 root         (0) root         (0)     5933 2023-11-28 18:25:20.000000 rasterio-1.4a1/tests/test_read_boundless.py
--rw-r--r--   0 root         (0) root         (0)     1141 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_read_dtype.py
--rw-r--r--   0 root         (0) root         (0)     4144 2023-12-30 22:39:27.000000 rasterio-1.4a1/tests/test_read_resample.py
--rw-r--r--   0 root         (0) root         (0)      720 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_reshape_image.py
--rw-r--r--   0 root         (0) root         (0)      824 2023-11-28 18:25:20.000000 rasterio-1.4a1/tests/test_revolvingdoor.py
--rw-r--r--   0 root         (0) root         (0)     4756 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_rio_blocks.py
--rw-r--r--   0 root         (0) root         (0)     1161 2023-11-28 18:25:20.000000 rasterio-1.4a1/tests/test_rio_bounds.py
--rw-r--r--   0 root         (0) root         (0)     7432 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_rio_calc.py
--rw-r--r--   0 root         (0) root         (0)     5738 2023-11-28 18:25:20.000000 rasterio-1.4a1/tests/test_rio_clip.py
--rw-r--r--   0 root         (0) root         (0)     6695 2024-02-13 00:03:41.000000 rasterio-1.4a1/tests/test_rio_convert.py
--rw-r--r--   0 root         (0) root         (0)    12940 2024-02-13 00:03:41.000000 rasterio-1.4a1/tests/test_rio_create.py
--rw-r--r--   0 root         (0) root         (0)    14474 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_rio_edit_info.py
--rw-r--r--   0 root         (0) root         (0)      753 2023-11-28 18:25:20.000000 rasterio-1.4a1/tests/test_rio_env.py
--rw-r--r--   0 root         (0) root         (0)     2506 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_rio_gcp.py
--rw-r--r--   0 root         (0) root         (0)     2093 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_rio_helpers.py
--rw-r--r--   0 root         (0) root         (0)    12172 2023-11-28 18:25:20.000000 rasterio-1.4a1/tests/test_rio_info.py
--rw-r--r--   0 root         (0) root         (0)      974 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_rio_insp.py
--rw-r--r--   0 root         (0) root         (0)      781 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_rio_main.py
--rw-r--r--   0 root         (0) root         (0)     6325 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_rio_mask.py
--rw-r--r--   0 root         (0) root         (0)    23621 2024-02-13 02:04:33.000000 rasterio-1.4a1/tests/test_rio_merge.py
--rw-r--r--   0 root         (0) root         (0)     6399 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_rio_options.py
--rw-r--r--   0 root         (0) root         (0)     3379 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_rio_overview.py
--rw-r--r--   0 root         (0) root         (0)    10961 2023-11-28 18:25:20.000000 rasterio-1.4a1/tests/test_rio_rasterize.py
--rw-r--r--   0 root         (0) root         (0)     1267 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_rio_rm.py
--rw-r--r--   0 root         (0) root         (0)     2011 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_rio_sample.py
--rw-r--r--   0 root         (0) root         (0)     6803 2024-02-13 00:03:41.000000 rasterio-1.4a1/tests/test_rio_shapes.py
--rw-r--r--   0 root         (0) root         (0)     2050 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_rio_stack.py
--rw-r--r--   0 root         (0) root         (0)      326 2023-11-28 18:25:20.000000 rasterio-1.4a1/tests/test_rio_transform.py
--rw-r--r--   0 root         (0) root         (0)    23309 2023-12-30 22:37:11.000000 rasterio-1.4a1/tests/test_rio_warp.py
--rw-r--r--   0 root         (0) root         (0)    10717 2023-11-28 18:25:20.000000 rasterio-1.4a1/tests/test_rpcs.py
--rw-r--r--   0 root         (0) root         (0)     2925 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_sampling.py
--rw-r--r--   0 root         (0) root         (0)     1595 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_scale_offset.py
--rw-r--r--   0 root         (0) root         (0)    13127 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_session.py
--rw-r--r--   0 root         (0) root         (0)     1130 2024-01-02 16:19:52.000000 rasterio-1.4a1/tests/test_show_versions.py
--rw-r--r--   0 root         (0) root         (0)     4969 2023-11-28 18:25:20.000000 rasterio-1.4a1/tests/test_shutil.py
--rw-r--r--   0 root         (0) root         (0)      856 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_statistics.py
--rw-r--r--   0 root         (0) root         (0)      825 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_subdatasets.py
--rw-r--r--   0 root         (0) root         (0)     1020 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_tag_item.py
--rw-r--r--   0 root         (0) root         (0)      468 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_tag_ns.py
--rw-r--r--   0 root         (0) root         (0)     2461 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_tags.py
--rw-r--r--   0 root         (0) root         (0)      806 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_thread_pool_executor.py
--rw-r--r--   0 root         (0) root         (0)     2146 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_threading.py
--rw-r--r--   0 root         (0) root         (0)      792 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_tools.py
--rw-r--r--   0 root         (0) root         (0)    17475 2023-12-30 22:39:27.000000 rasterio-1.4a1/tests/test_transform.py
--rw-r--r--   0 root         (0) root         (0)      875 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_units.py
--rw-r--r--   0 root         (0) root         (0)     3098 2023-11-28 18:25:20.000000 rasterio-1.4a1/tests/test_update.py
--rw-r--r--   0 root         (0) root         (0)     1227 2024-02-15 22:09:51.000000 rasterio-1.4a1/tests/test_vrt.py
--rw-r--r--   0 root         (0) root         (0)     1438 2024-02-13 00:03:41.000000 rasterio-1.4a1/tests/test_warnings.py
--rw-r--r--   0 root         (0) root         (0)    72467 2024-01-24 20:40:04.000000 rasterio-1.4a1/tests/test_warp.py
--rw-r--r--   0 root         (0) root         (0)     9922 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_warp_transform.py
--rw-r--r--   0 root         (0) root         (0)    24557 2024-01-03 20:12:31.000000 rasterio-1.4a1/tests/test_warpedvrt.py
--rw-r--r--   0 root         (0) root         (0)    22223 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_windows.py
--rw-r--r--   0 root         (0) root         (0)     3847 2023-11-28 16:53:09.000000 rasterio-1.4a1/tests/test_windows_mixins.py
--rw-r--r--   0 root         (0) root         (0)    20348 2023-11-28 18:25:20.000000 rasterio-1.4a1/tests/test_write.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-03 01:03:24.684818 rasterio-1.4a2/
+-rw-r--r--   0 root         (0) root         (0)     1990 2023-11-28 16:53:09.000000 rasterio-1.4a2/AUTHORS.txt
+-rw-r--r--   0 root         (0) root         (0)    91793 2024-03-02 15:38:31.000000 rasterio-1.4a2/CHANGES.txt
+-rw-r--r--   0 root         (0) root         (0)     1457 2023-11-28 16:53:09.000000 rasterio-1.4a2/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     7521 2024-03-03 01:03:24.685040 rasterio-1.4a2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6341 2024-01-16 23:55:08.000000 rasterio-1.4a2/README.rst
+-rw-r--r--   0 root         (0) root         (0)        5 2024-03-03 01:03:23.000000 rasterio-1.4a2/VERSION.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-03 01:03:24.502048 rasterio-1.4a2/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-03 01:03:24.539326 rasterio-1.4a2/docs/api/
+-rw-r--r--   0 root         (0) root         (0)       69 2023-11-28 16:53:09.000000 rasterio-1.4a2/docs/api/index.rst
+-rw-r--r--   0 root         (0) root         (0)      135 2023-11-28 16:53:09.000000 rasterio-1.4a2/docs/api/rasterio._base.rst
+-rw-r--r--   0 root         (0) root         (0)      132 2023-11-28 16:53:09.000000 rasterio-1.4a2/docs/api/rasterio._env.rst
+-rw-r--r--   0 root         (0) root         (0)      132 2023-11-28 16:53:09.000000 rasterio-1.4a2/docs/api/rasterio._err.rst
+-rw-r--r--   0 root         (0) root         (0)      144 2023-11-28 16:53:09.000000 rasterio-1.4a2/docs/api/rasterio._example.rst
+-rw-r--r--   0 root         (0) root         (0)      147 2023-11-28 16:53:09.000000 rasterio-1.4a2/docs/api/rasterio._features.rst
+-rw-r--r--   0 root         (0) root         (0)      165 2023-11-28 16:53:09.000000 rasterio-1.4a2/docs/api/rasterio._filepath.rst
+-rw-r--r--   0 root         (0) root         (0)      135 2023-11-28 16:53:09.000000 rasterio-1.4a2/docs/api/rasterio._fill.rst
+-rw-r--r--   0 root         (0) root         (0)      129 2023-11-28 16:53:09.000000 rasterio-1.4a2/docs/api/rasterio._io.rst
+-rw-r--r--   0 root         (0) root         (0)      162 2023-11-28 16:53:09.000000 rasterio-1.4a2/docs/api/rasterio._loading.rst
+-rw-r--r--   0 root         (0) root         (0)      168 2023-11-28 16:53:09.000000 rasterio-1.4a2/docs/api/rasterio._transform.rst
+-rw-r--r--   0 root         (0) root         (0)      135 2023-11-28 16:53:09.000000 rasterio-1.4a2/docs/api/rasterio._warp.rst
+-rw-r--r--   0 root         (0) root         (0)      139 2023-11-28 16:53:09.000000 rasterio-1.4a2/docs/api/rasterio.control.rst
+-rw-r--r--   0 root         (0) root         (0)      136 2023-11-28 16:53:09.000000 rasterio-1.4a2/docs/api/rasterio.coords.rst
+-rw-r--r--   0 root         (0) root         (0)      127 2023-11-28 16:53:09.000000 rasterio-1.4a2/docs/api/rasterio.crs.rst
+-rw-r--r--   0 root         (0) root         (0)      139 2023-11-28 16:53:09.000000 rasterio-1.4a2/docs/api/rasterio.drivers.rst
+-rw-r--r--   0 root         (0) root         (0)      136 2023-11-28 16:53:09.000000 rasterio-1.4a2/docs/api/rasterio.dtypes.rst
+-rw-r--r--   0 root         (0) root         (0)      133 2023-11-28 16:53:09.000000 rasterio-1.4a2/docs/api/rasterio.enums.rst
+-rw-r--r--   0 root         (0) root         (0)      147 2023-11-28 16:53:09.000000 rasterio-1.4a2/docs/api/rasterio.env.rst
+-rw-r--r--   0 root         (0) root         (0)      136 2023-11-28 16:53:09.000000 rasterio-1.4a2/docs/api/rasterio.errors.rst
+-rw-r--r--   0 root         (0) root         (0)      142 2023-11-28 16:53:09.000000 rasterio-1.4a2/docs/api/rasterio.features.rst
+-rw-r--r--   0 root         (0) root         (0)      130 2023-11-28 16:53:09.000000 rasterio-1.4a2/docs/api/rasterio.fill.rst
+-rw-r--r--   0 root         (0) root         (0)      144 2023-11-28 16:53:09.000000 rasterio-1.4a2/docs/api/rasterio.io.rst
+-rw-r--r--   0 root         (0) root         (0)      130 2023-11-28 16:53:09.000000 rasterio-1.4a2/docs/api/rasterio.mask.rst
+-rw-r--r--   0 root         (0) root         (0)      133 2023-11-28 16:53:09.000000 rasterio-1.4a2/docs/api/rasterio.merge.rst
+-rw-r--r--   0 root         (0) root         (0)      130 2023-11-28 16:53:09.000000 rasterio-1.4a2/docs/api/rasterio.path.rst
+-rw-r--r--   0 root         (0) root         (0)      130 2023-11-28 16:53:09.000000 rasterio-1.4a2/docs/api/rasterio.plot.rst
+-rw-r--r--   0 root         (0) root         (0)      142 2023-11-28 16:53:09.000000 rasterio-1.4a2/docs/api/rasterio.profiles.rst
+-rw-r--r--   0 root         (0) root         (0)       76 2023-11-28 18:25:20.000000 rasterio-1.4a2/docs/api/rasterio.rio.blocks.rst
+-rw-r--r--   0 root         (0) root         (0)       76 2023-11-28 18:25:20.000000 rasterio-1.4a2/docs/api/rasterio.rio.bounds.rst
+-rw-r--r--   0 root         (0) root         (0)       71 2023-11-28 18:25:20.000000 rasterio-1.4a2/docs/api/rasterio.rio.calc.rst
+-rw-r--r--   0 root         (0) root         (0)       53 2023-11-28 18:25:20.000000 rasterio-1.4a2/docs/api/rasterio.rio.clip.rst
+-rw-r--r--   0 root         (0) root         (0)       79 2023-11-28 18:25:20.000000 rasterio-1.4a2/docs/api/rasterio.rio.convert.rst
+-rw-r--r--   0 root         (0) root         (0)       80 2023-11-28 18:25:20.000000 rasterio-1.4a2/docs/api/rasterio.rio.edit_info.rst
+-rw-r--r--   0 root         (0) root         (0)       67 2023-11-28 18:25:20.000000 rasterio-1.4a2/docs/api/rasterio.rio.env.rst
+-rw-r--r--   0 root         (0) root         (0)       70 2023-11-28 18:25:20.000000 rasterio-1.4a2/docs/api/rasterio.rio.gcps.rst
+-rw-r--r--   0 root         (0) root         (0)       69 2023-11-28 18:25:20.000000 rasterio-1.4a2/docs/api/rasterio.rio.info.rst
+-rw-r--r--   0 root         (0) root         (0)       70 2023-11-28 18:25:20.000000 rasterio-1.4a2/docs/api/rasterio.rio.insp.rst
+-rw-r--r--   0 root         (0) root         (0)       70 2023-11-28 18:25:20.000000 rasterio-1.4a2/docs/api/rasterio.rio.mask.rst
+-rw-r--r--   0 root         (0) root         (0)       73 2023-11-28 18:25:20.000000 rasterio-1.4a2/docs/api/rasterio.rio.merge.rst
+-rw-r--r--   0 root         (0) root         (0)       82 2023-11-28 18:25:20.000000 rasterio-1.4a2/docs/api/rasterio.rio.overview.rst
+-rw-r--r--   0 root         (0) root         (0)       85 2023-11-28 18:25:20.000000 rasterio-1.4a2/docs/api/rasterio.rio.rasterize.rst
+-rw-r--r--   0 root         (0) root         (0)       64 2023-11-28 18:25:20.000000 rasterio-1.4a2/docs/api/rasterio.rio.rm.rst
+-rw-r--r--   0 root         (0) root         (0)      533 2023-11-28 18:25:20.000000 rasterio-1.4a2/docs/api/rasterio.rio.rst
+-rw-r--r--   0 root         (0) root         (0)       76 2023-11-28 18:25:20.000000 rasterio-1.4a2/docs/api/rasterio.rio.sample.rst
+-rw-r--r--   0 root         (0) root         (0)       76 2023-11-28 18:25:20.000000 rasterio-1.4a2/docs/api/rasterio.rio.shapes.rst
+-rw-r--r--   0 root         (0) root         (0)       74 2023-11-28 18:25:20.000000 rasterio-1.4a2/docs/api/rasterio.rio.stack.rst
+-rw-r--r--   0 root         (0) root         (0)       85 2023-11-28 18:25:20.000000 rasterio-1.4a2/docs/api/rasterio.rio.transform.rst
+-rw-r--r--   0 root         (0) root         (0)       70 2023-11-28 18:25:20.000000 rasterio-1.4a2/docs/api/rasterio.rio.warp.rst
+-rw-r--r--   0 root         (0) root         (0)      132 2023-11-28 16:53:09.000000 rasterio-1.4a2/docs/api/rasterio.rpc.rst
+-rw-r--r--   0 root         (0) root         (0)      744 2023-11-28 18:25:20.000000 rasterio-1.4a2/docs/api/rasterio.rst
+-rw-r--r--   0 root         (0) root         (0)      136 2023-11-28 16:53:09.000000 rasterio-1.4a2/docs/api/rasterio.sample.rst
+-rw-r--r--   0 root         (0) root         (0)      159 2023-11-28 16:53:09.000000 rasterio-1.4a2/docs/api/rasterio.session.rst
+-rw-r--r--   0 root         (0) root         (0)      136 2023-11-28 16:53:09.000000 rasterio-1.4a2/docs/api/rasterio.shutil.rst
+-rw-r--r--   0 root         (0) root         (0)      133 2023-11-28 16:53:09.000000 rasterio-1.4a2/docs/api/rasterio.tools.rst
+-rw-r--r--   0 root         (0) root         (0)      145 2023-11-28 16:53:09.000000 rasterio-1.4a2/docs/api/rasterio.transform.rst
+-rw-r--r--   0 root         (0) root         (0)      147 2023-11-28 16:53:09.000000 rasterio-1.4a2/docs/api/rasterio.vrt.rst
+-rw-r--r--   0 root         (0) root         (0)      130 2023-11-28 16:53:09.000000 rasterio-1.4a2/docs/api/rasterio.warp.rst
+-rw-r--r--   0 root         (0) root         (0)      136 2023-11-28 16:53:09.000000 rasterio-1.4a2/docs/api/rasterio.windows.rst
+-rw-r--r--   0 root         (0) root         (0)    21803 2024-02-13 00:03:41.000000 rasterio-1.4a2/docs/cli.rst
+-rw-r--r--   0 root         (0) root         (0)      407 2023-11-28 16:53:09.000000 rasterio-1.4a2/docs/contributing.rst
+-rw-r--r--   0 root         (0) root         (0)     4552 2023-12-30 22:39:27.000000 rasterio-1.4a2/docs/faq.rst
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-11-28 16:53:09.000000 rasterio-1.4a2/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)     2771 2023-11-28 18:25:20.000000 rasterio-1.4a2/docs/installation.rst
+-rw-r--r--   0 root         (0) root         (0)     2743 2023-11-28 16:53:09.000000 rasterio-1.4a2/docs/intro.rst
+-rw-r--r--   0 root         (0) root         (0)    11398 2023-11-28 18:25:20.000000 rasterio-1.4a2/docs/quickstart.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-03 01:03:24.558957 rasterio-1.4a2/docs/topics/
+-rw-r--r--   0 root         (0) root         (0)     3611 2023-11-28 16:53:09.000000 rasterio-1.4a2/docs/topics/calc.rst
+-rw-r--r--   0 root         (0) root         (0)     2637 2023-11-28 18:25:20.000000 rasterio-1.4a2/docs/topics/color.rst
+-rw-r--r--   0 root         (0) root         (0)     6267 2023-11-28 18:25:20.000000 rasterio-1.4a2/docs/topics/concurrency.rst
+-rw-r--r--   0 root         (0) root         (0)     3379 2023-11-28 18:25:20.000000 rasterio-1.4a2/docs/topics/configuration.rst
+-rw-r--r--   0 root         (0) root         (0)     1856 2023-11-28 18:25:20.000000 rasterio-1.4a2/docs/topics/datasets.rst
+-rw-r--r--   0 root         (0) root         (0)     1419 2023-11-28 18:25:20.000000 rasterio-1.4a2/docs/topics/errors.rst
+-rw-r--r--   0 root         (0) root         (0)     3498 2023-11-28 18:25:20.000000 rasterio-1.4a2/docs/topics/features.rst
+-rw-r--r--   0 root         (0) root         (0)       78 2023-11-28 18:25:20.000000 rasterio-1.4a2/docs/topics/fillnodata.rst
+-rw-r--r--   0 root         (0) root         (0)     4656 2023-11-28 18:25:20.000000 rasterio-1.4a2/docs/topics/georeferencing.rst
+-rw-r--r--   0 root         (0) root         (0)     3066 2023-11-28 18:25:20.000000 rasterio-1.4a2/docs/topics/image_options.rst
+-rw-r--r--   0 root         (0) root         (0)     1054 2023-11-28 16:53:09.000000 rasterio-1.4a2/docs/topics/image_processing.rst
+-rw-r--r--   0 root         (0) root         (0)      443 2023-11-28 16:53:09.000000 rasterio-1.4a2/docs/topics/index.rst
+-rw-r--r--   0 root         (0) root         (0)     1753 2023-11-28 18:25:20.000000 rasterio-1.4a2/docs/topics/masking-by-shapefile.rst
+-rw-r--r--   0 root         (0) root         (0)     9188 2023-11-28 18:25:20.000000 rasterio-1.4a2/docs/topics/masks.rst
+-rw-r--r--   0 root         (0) root         (0)     2925 2023-11-28 18:25:20.000000 rasterio-1.4a2/docs/topics/memory-files.rst
+-rw-r--r--   0 root         (0) root         (0)     8374 2023-11-28 18:25:20.000000 rasterio-1.4a2/docs/topics/migrating-to-v1.rst
+-rw-r--r--   0 root         (0) root         (0)     2092 2023-11-28 18:25:20.000000 rasterio-1.4a2/docs/topics/overviews.rst
+-rw-r--r--   0 root         (0) root         (0)     3944 2023-11-28 18:25:20.000000 rasterio-1.4a2/docs/topics/plotting.rst
+-rw-r--r--   0 root         (0) root         (0)     2307 2023-11-28 18:25:20.000000 rasterio-1.4a2/docs/topics/profiles.rst
+-rw-r--r--   0 root         (0) root         (0)     4801 2023-11-28 18:25:20.000000 rasterio-1.4a2/docs/topics/reading.rst
+-rw-r--r--   0 root         (0) root         (0)     8328 2023-12-30 22:37:11.000000 rasterio-1.4a2/docs/topics/reproject.rst
+-rw-r--r--   0 root         (0) root         (0)     2265 2023-11-28 18:25:20.000000 rasterio-1.4a2/docs/topics/resampling.rst
+-rw-r--r--   0 root         (0) root         (0)    13761 2023-11-28 18:25:20.000000 rasterio-1.4a2/docs/topics/switch.rst
+-rw-r--r--   0 root         (0) root         (0)     2993 2023-11-28 18:25:20.000000 rasterio-1.4a2/docs/topics/tags.rst
+-rw-r--r--   0 root         (0) root         (0)     4377 2023-11-28 18:25:20.000000 rasterio-1.4a2/docs/topics/transforms.rst
+-rw-r--r--   0 root         (0) root         (0)     5888 2023-11-28 18:25:20.000000 rasterio-1.4a2/docs/topics/virtual-warping.rst
+-rw-r--r--   0 root         (0) root         (0)     5692 2024-03-01 22:36:20.000000 rasterio-1.4a2/docs/topics/vsi.rst
+-rw-r--r--   0 root         (0) root         (0)     8169 2023-11-28 18:25:20.000000 rasterio-1.4a2/docs/topics/windowed-rw.rst
+-rw-r--r--   0 root         (0) root         (0)     2338 2023-11-28 18:25:20.000000 rasterio-1.4a2/docs/topics/writing.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-03 01:03:24.564312 rasterio-1.4a2/examples/
+-rw-r--r--   0 root         (0) root         (0)     3247 2023-11-28 18:25:20.000000 rasterio-1.4a2/examples/async-rasterio.py
+-rw-r--r--   0 root         (0) root         (0)      761 2023-11-28 16:53:09.000000 rasterio-1.4a2/examples/decimate.py
+-rw-r--r--   0 root         (0) root         (0)      222 2023-11-28 16:53:09.000000 rasterio-1.4a2/examples/polygonize.py
+-rw-r--r--   0 root         (0) root         (0)     1869 2023-11-28 16:53:09.000000 rasterio-1.4a2/examples/rasterio_polygonize.py
+-rw-r--r--   0 root         (0) root         (0)      810 2023-11-28 16:53:09.000000 rasterio-1.4a2/examples/rasterize_geometry.py
+-rw-r--r--   0 root         (0) root         (0)     1747 2023-11-28 16:53:09.000000 rasterio-1.4a2/examples/reproject.py
+-rw-r--r--   0 root         (0) root         (0)     1154 2023-11-28 16:53:09.000000 rasterio-1.4a2/examples/sieve.py
+-rw-r--r--   0 root         (0) root         (0)     2431 2023-11-28 18:25:20.000000 rasterio-1.4a2/examples/thread_pool_executor.py
+-rw-r--r--   0 root         (0) root         (0)     1318 2023-11-28 16:53:09.000000 rasterio-1.4a2/examples/total.py
+-rw-r--r--   0 root         (0) root         (0)      531 2024-02-14 18:25:56.000000 rasterio-1.4a2/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-03 01:03:24.580642 rasterio-1.4a2/rasterio/
+-rw-r--r--   0 root         (0) root         (0)    16248 2024-03-01 22:59:11.000000 rasterio-1.4a2/rasterio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1165 2023-11-28 16:53:09.000000 rasterio-1.4a2/rasterio/_base.pxd
+-rw-r--r--   0 root         (0) root         (0)    46502 2024-02-13 00:03:41.000000 rasterio-1.4a2/rasterio/_base.pyx
+-rw-r--r--   0 root         (0) root         (0)      155 2023-11-28 16:53:09.000000 rasterio-1.4a2/rasterio/_env.pxd
+-rw-r--r--   0 root         (0) root         (0)    15368 2024-02-13 00:03:41.000000 rasterio-1.4a2/rasterio/_env.pyx
+-rw-r--r--   0 root         (0) root         (0)      401 2024-02-13 00:03:41.000000 rasterio-1.4a2/rasterio/_err.pxd
+-rw-r--r--   0 root         (0) root         (0)     9266 2024-02-13 00:03:41.000000 rasterio-1.4a2/rasterio/_err.pyx
+-rw-r--r--   0 root         (0) root         (0)      804 2023-11-28 16:53:09.000000 rasterio-1.4a2/rasterio/_example.pyx
+-rw-r--r--   0 root         (0) root         (0)     1479 2023-11-28 18:25:20.000000 rasterio-1.4a2/rasterio/_features.pxd
+-rw-r--r--   0 root         (0) root         (0)    26598 2023-11-28 18:25:20.000000 rasterio-1.4a2/rasterio/_features.pyx
+-rw-r--r--   0 root         (0) root         (0)      199 2023-11-28 16:53:09.000000 rasterio-1.4a2/rasterio/_filepath.pxd
+-rw-r--r--   0 root         (0) root         (0)     8879 2023-12-30 22:39:27.000000 rasterio-1.4a2/rasterio/_filepath.pyx
+-rw-r--r--   0 root         (0) root         (0)     1289 2023-11-28 16:53:09.000000 rasterio-1.4a2/rasterio/_fill.pyx
+-rw-r--r--   0 root         (0) root         (0)      972 2023-11-28 16:53:09.000000 rasterio-1.4a2/rasterio/_io.pxd
+-rw-r--r--   0 root         (0) root         (0)    87467 2024-02-13 02:04:33.000000 rasterio-1.4a2/rasterio/_io.pyx
+-rw-r--r--   0 root         (0) root         (0)     5488 2024-03-01 22:36:20.000000 rasterio-1.4a2/rasterio/_path.py
+-rw-r--r--   0 root         (0) root         (0)     2427 2024-01-02 16:19:52.000000 rasterio-1.4a2/rasterio/_show_versions.py
+-rw-r--r--   0 root         (0) root         (0)    12533 2023-12-30 22:39:27.000000 rasterio-1.4a2/rasterio/_transform.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-03 01:03:24.478034 rasterio-1.4a2/rasterio/_vendor/
+-rw-r--r--   0 root         (0) root         (0)       24 2024-03-01 22:58:06.000000 rasterio-1.4a2/rasterio/_vendor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8141 2024-01-02 16:19:52.000000 rasterio-1.4a2/rasterio/_vendor/snuggs.py
+-rw-r--r--   0 root         (0) root         (0)      502 2023-11-28 16:53:09.000000 rasterio-1.4a2/rasterio/_version.pxd
+-rw-r--r--   0 root         (0) root         (0)     2171 2023-11-28 16:53:09.000000 rasterio-1.4a2/rasterio/_version.pyx
+-rw-r--r--   0 root         (0) root         (0)      197 2024-03-01 22:36:20.000000 rasterio-1.4a2/rasterio/_vsiopener.pxd
+-rw-r--r--   0 root         (0) root         (0)    16343 2024-03-01 22:36:20.000000 rasterio-1.4a2/rasterio/_vsiopener.pyx
+-rw-r--r--   0 root         (0) root         (0)     1901 2023-11-28 16:53:09.000000 rasterio-1.4a2/rasterio/_warp.pxd
+-rw-r--r--   0 root         (0) root         (0)    58992 2024-02-13 00:03:41.000000 rasterio-1.4a2/rasterio/_warp.pyx
+-rw-r--r--   0 root         (0) root         (0)     2066 2023-11-28 16:53:09.000000 rasterio-1.4a2/rasterio/control.py
+-rw-r--r--   0 root         (0) root         (0)     1450 2023-11-28 16:53:09.000000 rasterio-1.4a2/rasterio/coords.py
+-rw-r--r--   0 root         (0) root         (0)      138 2023-11-28 16:53:09.000000 rasterio-1.4a2/rasterio/crs.pxd
+-rw-r--r--   0 root         (0) root         (0)    33589 2023-12-30 22:39:27.000000 rasterio-1.4a2/rasterio/crs.pyx
+-rw-r--r--   0 root         (0) root         (0)     1840 2023-11-28 18:25:20.000000 rasterio-1.4a2/rasterio/drivers.py
+-rw-r--r--   0 root         (0) root         (0)     6296 2023-12-30 22:39:27.000000 rasterio-1.4a2/rasterio/dtypes.py
+-rw-r--r--   0 root         (0) root         (0)     5550 2023-11-28 16:53:09.000000 rasterio-1.4a2/rasterio/enums.py
+-rw-r--r--   0 root         (0) root         (0)    22489 2023-12-30 22:37:11.000000 rasterio-1.4a2/rasterio/env.py
+-rw-r--r--   0 root         (0) root         (0)     4654 2024-02-13 00:03:41.000000 rasterio-1.4a2/rasterio/errors.py
+-rw-r--r--   0 root         (0) root         (0)    23522 2024-03-01 22:58:06.000000 rasterio-1.4a2/rasterio/features.py
+-rw-r--r--   0 root         (0) root         (0)     2742 2023-11-28 18:25:20.000000 rasterio-1.4a2/rasterio/fill.py
+-rw-r--r--   0 root         (0) root         (0)    33111 2024-03-01 22:36:20.000000 rasterio-1.4a2/rasterio/gdal.pxi
+-rw-r--r--   0 root         (0) root         (0)     8959 2023-12-30 22:39:27.000000 rasterio-1.4a2/rasterio/io.py
+-rw-r--r--   0 root         (0) root         (0)     7562 2023-12-30 22:39:27.000000 rasterio-1.4a2/rasterio/mask.py
+-rw-r--r--   0 root         (0) root         (0)    15261 2024-02-13 02:04:33.000000 rasterio-1.4a2/rasterio/merge.py
+-rw-r--r--   0 root         (0) root         (0)      520 2023-11-28 16:53:09.000000 rasterio-1.4a2/rasterio/path.py
+-rw-r--r--   0 root         (0) root         (0)    11135 2024-01-19 23:56:39.000000 rasterio-1.4a2/rasterio/plot.py
+-rw-r--r--   0 root         (0) root         (0)     1343 2023-11-28 18:25:20.000000 rasterio-1.4a2/rasterio/profiles.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-03 01:03:24.497070 rasterio-1.4a2/rasterio/rio/
+-rw-r--r--   0 root         (0) root         (0)       50 2023-11-28 16:53:09.000000 rasterio-1.4a2/rasterio/rio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4876 2023-11-28 18:25:20.000000 rasterio-1.4a2/rasterio/rio/blocks.py
+-rw-r--r--   0 root         (0) root         (0)     3770 2023-11-28 18:25:20.000000 rasterio-1.4a2/rasterio/rio/bounds.py
+-rw-r--r--   0 root         (0) root         (0)     8322 2024-01-02 16:19:52.000000 rasterio-1.4a2/rasterio/rio/calc.py
+-rw-r--r--   0 root         (0) root         (0)     6863 2023-11-28 18:25:20.000000 rasterio-1.4a2/rasterio/rio/clip.py
+-rw-r--r--   0 root         (0) root         (0)     3395 2023-11-28 16:53:09.000000 rasterio-1.4a2/rasterio/rio/convert.py
+-rw-r--r--   0 root         (0) root         (0)     5315 2024-02-13 00:03:41.000000 rasterio-1.4a2/rasterio/rio/create.py
+-rw-r--r--   0 root         (0) root         (0)     8814 2023-12-30 22:39:27.000000 rasterio-1.4a2/rasterio/rio/edit_info.py
+-rw-r--r--   0 root         (0) root         (0)     1410 2023-11-28 16:53:09.000000 rasterio-1.4a2/rasterio/rio/env.py
+-rw-r--r--   0 root         (0) root         (0)     3784 2023-11-28 16:53:09.000000 rasterio-1.4a2/rasterio/rio/gcps.py
+-rw-r--r--   0 root         (0) root         (0)     3598 2023-11-28 16:53:09.000000 rasterio-1.4a2/rasterio/rio/helpers.py
+-rw-r--r--   0 root         (0) root         (0)     5321 2024-01-25 19:09:47.000000 rasterio-1.4a2/rasterio/rio/info.py
+-rw-r--r--   0 root         (0) root         (0)     2748 2023-11-28 18:25:20.000000 rasterio-1.4a2/rasterio/rio/insp.py
+-rw-r--r--   0 root         (0) root         (0)     3313 2023-11-28 18:25:20.000000 rasterio-1.4a2/rasterio/rio/main.py
+-rw-r--r--   0 root         (0) root         (0)     4744 2023-11-28 16:53:09.000000 rasterio-1.4a2/rasterio/rio/mask.py
+-rw-r--r--   0 root         (0) root         (0)     3268 2024-02-13 02:04:33.000000 rasterio-1.4a2/rasterio/rio/merge.py
+-rw-r--r--   0 root         (0) root         (0)    12040 2024-03-02 15:36:26.000000 rasterio-1.4a2/rasterio/rio/options.py
+-rw-r--r--   0 root         (0) root         (0)     4850 2023-11-28 18:25:20.000000 rasterio-1.4a2/rasterio/rio/overview.py
+-rw-r--r--   0 root         (0) root         (0)    10082 2023-11-28 18:25:20.000000 rasterio-1.4a2/rasterio/rio/rasterize.py
+-rw-r--r--   0 root         (0) root         (0)      946 2023-11-28 16:53:09.000000 rasterio-1.4a2/rasterio/rio/rm.py
+-rw-r--r--   0 root         (0) root         (0)     2275 2023-11-28 16:53:09.000000 rasterio-1.4a2/rasterio/rio/sample.py
+-rw-r--r--   0 root         (0) root         (0)     4310 2023-11-28 16:53:09.000000 rasterio-1.4a2/rasterio/rio/shapes.py
+-rw-r--r--   0 root         (0) root         (0)     3959 2023-11-28 16:53:09.000000 rasterio-1.4a2/rasterio/rio/stack.py
+-rw-r--r--   0 root         (0) root         (0)     2140 2023-11-28 18:25:20.000000 rasterio-1.4a2/rasterio/rio/transform.py
+-rw-r--r--   0 root         (0) root         (0)    14847 2023-12-30 22:37:11.000000 rasterio-1.4a2/rasterio/rio/warp.py
+-rw-r--r--   0 root         (0) root         (0)     4130 2023-11-28 18:25:20.000000 rasterio-1.4a2/rasterio/rpc.py
+-rw-r--r--   0 root         (0) root         (0)     2800 2023-11-28 18:25:20.000000 rasterio-1.4a2/rasterio/sample.py
+-rw-r--r--   0 root         (0) root         (0)    18259 2023-11-28 16:53:09.000000 rasterio-1.4a2/rasterio/session.py
+-rw-r--r--   0 root         (0) root         (0)     7291 2023-11-28 16:53:09.000000 rasterio-1.4a2/rasterio/shutil.pyx
+-rw-r--r--   0 root         (0) root         (0)     2205 2023-11-28 16:53:09.000000 rasterio-1.4a2/rasterio/tools.py
+-rw-r--r--   0 root         (0) root         (0)    18324 2023-12-30 22:39:27.000000 rasterio-1.4a2/rasterio/transform.py
+-rw-r--r--   0 root         (0) root         (0)    10871 2024-03-01 22:10:59.000000 rasterio-1.4a2/rasterio/vrt.py
+-rw-r--r--   0 root         (0) root         (0)    21283 2023-12-30 22:39:27.000000 rasterio-1.4a2/rasterio/warp.py
+-rw-r--r--   0 root         (0) root         (0)    23609 2024-02-13 02:04:33.000000 rasterio-1.4a2/rasterio/windows.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-03 01:03:24.585287 rasterio-1.4a2/rasterio.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7521 2024-03-03 01:03:24.000000 rasterio-1.4a2/rasterio.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7633 2024-03-03 01:03:24.000000 rasterio-1.4a2/rasterio.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-03 01:03:24.000000 rasterio-1.4a2/rasterio.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      797 2024-03-03 01:03:24.000000 rasterio-1.4a2/rasterio.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-12-08 16:53:08.000000 rasterio-1.4a2/rasterio.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      520 2024-03-03 01:03:24.000000 rasterio-1.4a2/rasterio.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-03-03 01:03:24.000000 rasterio-1.4a2/rasterio.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1387 2024-03-03 01:03:24.685877 rasterio-1.4a2/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)    11196 2024-03-01 22:58:06.000000 rasterio-1.4a2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-03 01:03:24.682994 rasterio-1.4a2/tests/
+-rw-r--r--   0 root         (0) root         (0)      719 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/README.rst
+-rw-r--r--   0 root         (0) root         (0)        0 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16778 2023-11-28 18:25:20.000000 rasterio-1.4a2/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-03 01:03:24.684094 rasterio-1.4a2/tests/data/
+-rw-r--r--   0 root         (0) root         (0)      526 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/data/README.rst
+-rw-r--r--   0 root         (0) root         (0)     3663 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/rangehttpserver.py
+-rw-r--r--   0 root         (0) root         (0)     4241 2023-11-28 18:25:20.000000 rasterio-1.4a2/tests/test__env.py
+-rw-r--r--   0 root         (0) root         (0)      755 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test__version.py
+-rw-r--r--   0 root         (0) root         (0)      332 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_band.py
+-rw-r--r--   0 root         (0) root         (0)     5468 2023-11-28 18:25:20.000000 rasterio-1.4a2/tests/test_band_masks.py
+-rw-r--r--   0 root         (0) root         (0)     8149 2024-02-13 00:03:41.000000 rasterio-1.4a2/tests/test_blocks.py
+-rw-r--r--   0 root         (0) root         (0)     7367 2023-11-28 18:25:20.000000 rasterio-1.4a2/tests/test_boundless_read.py
+-rw-r--r--   0 root         (0) root         (0)     1767 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_checksum.py
+-rw-r--r--   0 root         (0) root         (0)      562 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_cli_main.py
+-rw-r--r--   0 root         (0) root         (0)     3062 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_colorinterp.py
+-rw-r--r--   0 root         (0) root         (0)      964 2023-11-28 18:25:20.000000 rasterio-1.4a2/tests/test_colormap.py
+-rw-r--r--   0 root         (0) root         (0)     2814 2023-11-28 18:25:20.000000 rasterio-1.4a2/tests/test_complex_dtypes.py
+-rw-r--r--   0 root         (0) root         (0)     1378 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_coords.py
+-rw-r--r--   0 root         (0) root         (0)      849 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_creation_options.py
+-rw-r--r--   0 root         (0) root         (0)    21943 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_crs.py
+-rw-r--r--   0 root         (0) root         (0)      344 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_data_paths.py
+-rw-r--r--   0 root         (0) root         (0)     4558 2024-03-02 01:06:05.000000 rasterio-1.4a2/tests/test_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     6346 2023-11-28 18:25:20.000000 rasterio-1.4a2/tests/test_dataset_mask.py
+-rw-r--r--   0 root         (0) root         (0)     2058 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_dataset_rw.py
+-rw-r--r--   0 root         (0) root         (0)      431 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_deprecated.py
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_descriptions.py
+-rw-r--r--   0 root         (0) root         (0)     1413 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_driver_management.py
+-rw-r--r--   0 root         (0) root         (0)      291 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_driver_policy.py
+-rw-r--r--   0 root         (0) root         (0)     4659 2023-11-28 18:25:20.000000 rasterio-1.4a2/tests/test_dtypes.py
+-rw-r--r--   0 root         (0) root         (0)      508 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_enums.py
+-rw-r--r--   0 root         (0) root         (0)    36482 2023-12-30 22:37:11.000000 rasterio-1.4a2/tests/test_env.py
+-rw-r--r--   0 root         (0) root         (0)     2662 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_err.py
+-rw-r--r--   0 root         (0) root         (0)    37794 2024-01-16 23:55:08.000000 rasterio-1.4a2/tests/test_features.py
+-rw-r--r--   0 root         (0) root         (0)     8328 2024-03-01 22:36:20.000000 rasterio-1.4a2/tests/test_filepath.py
+-rw-r--r--   0 root         (0) root         (0)     1111 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_fillnodata.py
+-rw-r--r--   0 root         (0) root         (0)     4712 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_gcps.py
+-rw-r--r--   0 root         (0) root         (0)     3457 2023-11-28 18:25:20.000000 rasterio-1.4a2/tests/test_gdal_raster_io.py
+-rw-r--r--   0 root         (0) root         (0)     1937 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_image_structure.py
+-rw-r--r--   0 root         (0) root         (0)     9043 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_indexing.py
+-rw-r--r--   0 root         (0) root         (0)     1576 2023-11-28 18:25:20.000000 rasterio-1.4a2/tests/test_int8.py
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_io.py
+-rw-r--r--   0 root         (0) root         (0)     3330 2023-11-28 18:25:20.000000 rasterio-1.4a2/tests/test_io_mixins.py
+-rw-r--r--   0 root         (0) root         (0)    11380 2023-12-30 22:39:27.000000 rasterio-1.4a2/tests/test_mask.py
+-rw-r--r--   0 root         (0) root         (0)     3335 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_mask_creation.py
+-rw-r--r--   0 root         (0) root         (0)    16548 2023-12-30 22:39:27.000000 rasterio-1.4a2/tests/test_memoryfile.py
+-rw-r--r--   0 root         (0) root         (0)     6530 2024-02-13 02:04:33.000000 rasterio-1.4a2/tests/test_merge.py
+-rw-r--r--   0 root         (0) root         (0)      859 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_meta.py
+-rw-r--r--   0 root         (0) root         (0)      914 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_no_georef.py
+-rw-r--r--   0 root         (0) root         (0)     2977 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_nodata.py
+-rw-r--r--   0 root         (0) root         (0)      908 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_open.py
+-rw-r--r--   0 root         (0) root         (0)      810 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_open_options.py
+-rw-r--r--   0 root         (0) root         (0)      597 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_open_overview_level.py
+-rw-r--r--   0 root         (0) root         (0)     1439 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_open_sharing.py
+-rw-r--r--   0 root         (0) root         (0)      507 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_options.py
+-rw-r--r--   0 root         (0) root         (0)     5661 2023-11-28 18:25:20.000000 rasterio-1.4a2/tests/test_overviews.py
+-rw-r--r--   0 root         (0) root         (0)      309 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_pad.py
+-rw-r--r--   0 root         (0) root         (0)     8452 2024-03-01 22:36:20.000000 rasterio-1.4a2/tests/test_path.py
+-rw-r--r--   0 root         (0) root         (0)     8772 2024-01-19 23:56:39.000000 rasterio-1.4a2/tests/test_plot.py
+-rw-r--r--   0 root         (0) root         (0)      659 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_png.py
+-rw-r--r--   0 root         (0) root         (0)      796 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_process_pool_executor.py
+-rw-r--r--   0 root         (0) root         (0)     3536 2024-02-13 00:03:41.000000 rasterio-1.4a2/tests/test_profile.py
+-rw-r--r--   0 root         (0) root         (0)     6261 2024-03-02 01:09:02.000000 rasterio-1.4a2/tests/test_pyopener.py
+-rw-r--r--   0 root         (0) root         (0)    14849 2024-02-13 00:03:41.000000 rasterio-1.4a2/tests/test_read.py
+-rw-r--r--   0 root         (0) root         (0)     5933 2023-11-28 18:25:20.000000 rasterio-1.4a2/tests/test_read_boundless.py
+-rw-r--r--   0 root         (0) root         (0)     1141 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_read_dtype.py
+-rw-r--r--   0 root         (0) root         (0)     4144 2023-12-30 22:39:27.000000 rasterio-1.4a2/tests/test_read_resample.py
+-rw-r--r--   0 root         (0) root         (0)      720 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_reshape_image.py
+-rw-r--r--   0 root         (0) root         (0)      824 2023-11-28 18:25:20.000000 rasterio-1.4a2/tests/test_revolvingdoor.py
+-rw-r--r--   0 root         (0) root         (0)     4756 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_rio_blocks.py
+-rw-r--r--   0 root         (0) root         (0)     1161 2023-11-28 18:25:20.000000 rasterio-1.4a2/tests/test_rio_bounds.py
+-rw-r--r--   0 root         (0) root         (0)     7432 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_rio_calc.py
+-rw-r--r--   0 root         (0) root         (0)     5738 2023-11-28 18:25:20.000000 rasterio-1.4a2/tests/test_rio_clip.py
+-rw-r--r--   0 root         (0) root         (0)     6695 2024-02-13 00:03:41.000000 rasterio-1.4a2/tests/test_rio_convert.py
+-rw-r--r--   0 root         (0) root         (0)    12940 2024-02-13 00:03:41.000000 rasterio-1.4a2/tests/test_rio_create.py
+-rw-r--r--   0 root         (0) root         (0)    14474 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_rio_edit_info.py
+-rw-r--r--   0 root         (0) root         (0)      753 2023-11-28 18:25:20.000000 rasterio-1.4a2/tests/test_rio_env.py
+-rw-r--r--   0 root         (0) root         (0)     2506 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_rio_gcp.py
+-rw-r--r--   0 root         (0) root         (0)     2093 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_rio_helpers.py
+-rw-r--r--   0 root         (0) root         (0)    12172 2023-11-28 18:25:20.000000 rasterio-1.4a2/tests/test_rio_info.py
+-rw-r--r--   0 root         (0) root         (0)      974 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_rio_insp.py
+-rw-r--r--   0 root         (0) root         (0)      781 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_rio_main.py
+-rw-r--r--   0 root         (0) root         (0)     6325 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_rio_mask.py
+-rw-r--r--   0 root         (0) root         (0)    23621 2024-02-13 02:04:33.000000 rasterio-1.4a2/tests/test_rio_merge.py
+-rw-r--r--   0 root         (0) root         (0)     6399 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_rio_options.py
+-rw-r--r--   0 root         (0) root         (0)     3379 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_rio_overview.py
+-rw-r--r--   0 root         (0) root         (0)    10961 2023-11-28 18:25:20.000000 rasterio-1.4a2/tests/test_rio_rasterize.py
+-rw-r--r--   0 root         (0) root         (0)     1267 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_rio_rm.py
+-rw-r--r--   0 root         (0) root         (0)     2011 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_rio_sample.py
+-rw-r--r--   0 root         (0) root         (0)     6803 2024-02-13 00:03:41.000000 rasterio-1.4a2/tests/test_rio_shapes.py
+-rw-r--r--   0 root         (0) root         (0)     2050 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_rio_stack.py
+-rw-r--r--   0 root         (0) root         (0)      326 2023-11-28 18:25:20.000000 rasterio-1.4a2/tests/test_rio_transform.py
+-rw-r--r--   0 root         (0) root         (0)    23309 2024-03-02 01:07:15.000000 rasterio-1.4a2/tests/test_rio_warp.py
+-rw-r--r--   0 root         (0) root         (0)    10717 2023-11-28 18:25:20.000000 rasterio-1.4a2/tests/test_rpcs.py
+-rw-r--r--   0 root         (0) root         (0)     2925 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_sampling.py
+-rw-r--r--   0 root         (0) root         (0)     1595 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_scale_offset.py
+-rw-r--r--   0 root         (0) root         (0)    13127 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_session.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2024-01-02 16:19:52.000000 rasterio-1.4a2/tests/test_show_versions.py
+-rw-r--r--   0 root         (0) root         (0)     4969 2023-11-28 18:25:20.000000 rasterio-1.4a2/tests/test_shutil.py
+-rw-r--r--   0 root         (0) root         (0)      856 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_statistics.py
+-rw-r--r--   0 root         (0) root         (0)      825 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_subdatasets.py
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_tag_item.py
+-rw-r--r--   0 root         (0) root         (0)      468 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_tag_ns.py
+-rw-r--r--   0 root         (0) root         (0)     2461 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_tags.py
+-rw-r--r--   0 root         (0) root         (0)      806 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_thread_pool_executor.py
+-rw-r--r--   0 root         (0) root         (0)     2146 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_threading.py
+-rw-r--r--   0 root         (0) root         (0)      792 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_tools.py
+-rw-r--r--   0 root         (0) root         (0)    17475 2023-12-30 22:39:27.000000 rasterio-1.4a2/tests/test_transform.py
+-rw-r--r--   0 root         (0) root         (0)      875 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_units.py
+-rw-r--r--   0 root         (0) root         (0)     3098 2023-11-28 18:25:20.000000 rasterio-1.4a2/tests/test_update.py
+-rw-r--r--   0 root         (0) root         (0)     1227 2024-03-01 22:10:59.000000 rasterio-1.4a2/tests/test_vrt.py
+-rw-r--r--   0 root         (0) root         (0)     1438 2024-02-13 00:03:41.000000 rasterio-1.4a2/tests/test_warnings.py
+-rw-r--r--   0 root         (0) root         (0)    72467 2024-01-24 20:40:04.000000 rasterio-1.4a2/tests/test_warp.py
+-rw-r--r--   0 root         (0) root         (0)     9922 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_warp_transform.py
+-rw-r--r--   0 root         (0) root         (0)    24546 2024-03-02 01:30:49.000000 rasterio-1.4a2/tests/test_warpedvrt.py
+-rw-r--r--   0 root         (0) root         (0)    22223 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_windows.py
+-rw-r--r--   0 root         (0) root         (0)     3847 2023-11-28 16:53:09.000000 rasterio-1.4a2/tests/test_windows_mixins.py
+-rw-r--r--   0 root         (0) root         (0)    20348 2023-11-28 18:25:20.000000 rasterio-1.4a2/tests/test_write.py
```

### Comparing `rasterio-1.4a1/AUTHORS.txt` & `rasterio-1.4a2/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/CHANGES.txt` & `rasterio-1.4a2/CHANGES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,33 @@
 Changes
 =======
 
-1.4a1 (2024-02-15)
+1.4a2 (2024-03-02)
 ------------------
 
 Python support:
 
 - Rasterio 1.4 requires Python version 3.9 or newer.
 
+New features:
+
+- Python openers can now support discovery of auxiliary "sidecar" files like
+  .aux.xml, .msk, and .tfw files for GeoTIFFs (#3032). Additionally, filesystem
+  objects, such as those from fsspec, can be used as openers. This will become
+  the recommended usage, supplanting the use of single file openers.
+
+Bug fixes:
+
+- The rio CLI output file options no longer resolve to absolute paths.
+- gzip, tar, and zip archive URIs containing drive letters were not always
+  parsed properly on Windows, but are now.
+
+1.4a1 (2024-02-16)
+------------------
+
 Deprecations:
 
 - The is_tiled property of a dataset will be removed in a future version and
   a pending deprecation warning will be raised if it is used (#3015). This
   warning may be changed to a deprecation warning at version 1.5.0. Please
   consider copying the body of the property to your own project. It's just one
   line.
@@ -47,14 +63,17 @@
 - The output file size limits of rio-warp were made redundant by changes to the
   GTiff driver in GDAL 2.1 and have been removed (#2889). A --dry-run option
   has been added to the command. If used, the profile of the output dataset
   will be printed and no warping will occur.
 
 Bug fixes:
 
+- A nodata value passed to _boundless_vrt_doc(), used for boundless reads, has
+  been ignored in favor of the source dataset's own nodata value. It is no
+  longer ignored (#3026).
 - Avoid squeezing narrow 2-D arrays to 1-D (#3008).
 - Operations on closed MemoryFile and ZipMemoryFile objects now raise
   ValueError as with other Python file objects (#2870, #).
 - Delay clamping of I/O windows until just before GDAL methods calls to improve
   accuracy of sub-pixel reads (#2864).
 
 Other changes:
```

### Comparing `rasterio-1.4a1/LICENSE.txt` & `rasterio-1.4a2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/PKG-INFO` & `rasterio-1.4a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rasterio
-Version: 1.4a1
+Version: 1.4a2
 Summary: Fast and direct raster I/O for use with Numpy and SciPy
 Home-page: https://github.com/rasterio/rasterio
 Author: Sean Gillies
 Author-email: sean@mapbox.com
 License: BSD
 Keywords: raster gdal
 Platform: UNKNOWN
@@ -19,20 +19,20 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Graphics :: Graphics Conversion
 Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Python: >=3.9
-Provides-Extra: all
 Provides-Extra: docs
 Provides-Extra: ipython
 Provides-Extra: plot
 Provides-Extra: s3
 Provides-Extra: test
+Provides-Extra: all
 License-File: LICENSE.txt
 License-File: AUTHORS.txt
 
 ========
 Rasterio
 ========
```

### Comparing `rasterio-1.4a1/README.rst` & `rasterio-1.4a2/README.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/docs/api/rasterio.rio.rst` & `rasterio-1.4a2/docs/api/rasterio.rio.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/docs/api/rasterio.rst` & `rasterio-1.4a2/docs/api/rasterio.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/docs/cli.rst` & `rasterio-1.4a2/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/docs/faq.rst` & `rasterio-1.4a2/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/docs/index.rst` & `rasterio-1.4a2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/docs/installation.rst` & `rasterio-1.4a2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/docs/intro.rst` & `rasterio-1.4a2/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/docs/quickstart.rst` & `rasterio-1.4a2/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/docs/topics/calc.rst` & `rasterio-1.4a2/docs/topics/calc.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/docs/topics/color.rst` & `rasterio-1.4a2/docs/topics/color.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/docs/topics/concurrency.rst` & `rasterio-1.4a2/docs/topics/concurrency.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/docs/topics/configuration.rst` & `rasterio-1.4a2/docs/topics/configuration.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/docs/topics/datasets.rst` & `rasterio-1.4a2/docs/topics/datasets.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/docs/topics/errors.rst` & `rasterio-1.4a2/docs/topics/errors.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/docs/topics/features.rst` & `rasterio-1.4a2/docs/topics/features.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/docs/topics/georeferencing.rst` & `rasterio-1.4a2/docs/topics/georeferencing.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/docs/topics/image_options.rst` & `rasterio-1.4a2/docs/topics/image_options.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/docs/topics/image_processing.rst` & `rasterio-1.4a2/docs/topics/image_processing.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/docs/topics/masking-by-shapefile.rst` & `rasterio-1.4a2/docs/topics/masking-by-shapefile.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/docs/topics/masks.rst` & `rasterio-1.4a2/docs/topics/masks.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/docs/topics/memory-files.rst` & `rasterio-1.4a2/docs/topics/memory-files.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/docs/topics/migrating-to-v1.rst` & `rasterio-1.4a2/docs/topics/migrating-to-v1.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/docs/topics/overviews.rst` & `rasterio-1.4a2/docs/topics/overviews.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/docs/topics/plotting.rst` & `rasterio-1.4a2/docs/topics/plotting.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/docs/topics/profiles.rst` & `rasterio-1.4a2/docs/topics/profiles.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/docs/topics/reading.rst` & `rasterio-1.4a2/docs/topics/reading.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/docs/topics/reproject.rst` & `rasterio-1.4a2/docs/topics/reproject.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/docs/topics/resampling.rst` & `rasterio-1.4a2/docs/topics/resampling.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/docs/topics/switch.rst` & `rasterio-1.4a2/docs/topics/switch.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/docs/topics/tags.rst` & `rasterio-1.4a2/docs/topics/tags.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/docs/topics/transforms.rst` & `rasterio-1.4a2/docs/topics/transforms.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/docs/topics/virtual-warping.rst` & `rasterio-1.4a2/docs/topics/virtual-warping.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/docs/topics/vsi.rst` & `rasterio-1.4a2/docs/topics/vsi.rst`

 * *Files 11% similar despite different names*

```diff
@@ -107,16 +107,16 @@
 .. note:: AWS pricing concerns
    While this feature can reduce latency by reading fewer bytes from S3
    compared to downloading the entire TIFF and opening locally, it does
    make at least 3 GET requests to fetch a TIFF's `profile` as shown above
    and likely many more to fetch all the imagery from the TIFF. Consult the
    AWS S3 pricing guidelines before deciding if `aws.Session` is for you.
 
-Python file openers
--------------------
+Python file and filesystem openers
+----------------------------------
 
 Datasets stored in proprietary systems or addressable only through protocols
 not directly supported by GDAL can be accessed using the ``opener`` keyword
 argument of ``rasterio.open``. Here is an example of using ``fs_s3fs`` to
 access the dataset in
 ``sentinel-s2-l2a-cogs/45/C/VQ/2022/11/S2B_45CVQ_20221102_0_L2A/B01.tif`` from
 the ``sentinel-cogs`` AWS S3 bucket. Rasterio can access this without using the
@@ -144,8 +144,28 @@
 
 Read and write access is supported, with some limitations. Only one opener at
 a time may be thus registered for a filename and access mode pair. Openers are
 unregistered when the dataset is closed or its context is exited. The other
 limitation is that auxiliary and sidecar files cannot be accessed and thus
 formats depending on them cannot be used in this way.
 
+To gain support for auxiliary "sidecar" files such as .aux.xml and .msk files
+that may accompany GeoTIFFs, an fsspec-like filesystem object may be used as
+the opener.
+
+.. code-block:: python
+
+    import rasterio
+    from fsspec
+
+    fs = fsspec.filesystem("s3", anon=True)
+
+    with rasterio.open(
+        "sentinel-cogs/sentinel-s2-l2a-cogs/45/C/VQ/2022/11/S2B_45CVQ_20221102_0_L2A/B01.tif",
+        opener=fs
+    ) as src:
+        print(src.profile)
+
+This kind of filesystem opener object must provide the following methods:
+``isdir()``, ``isfile()``, ``ls()``, ``mtime()``, ``open()``, and ``size()``.
+
 *New in version 1.4.0*
```

### Comparing `rasterio-1.4a1/docs/topics/windowed-rw.rst` & `rasterio-1.4a2/docs/topics/windowed-rw.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/docs/topics/writing.rst` & `rasterio-1.4a2/docs/topics/writing.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/examples/async-rasterio.py` & `rasterio-1.4a2/examples/async-rasterio.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/examples/decimate.py` & `rasterio-1.4a2/examples/decimate.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/examples/rasterio_polygonize.py` & `rasterio-1.4a2/examples/rasterio_polygonize.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/examples/rasterize_geometry.py` & `rasterio-1.4a2/examples/rasterize_geometry.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/examples/reproject.py` & `rasterio-1.4a2/examples/reproject.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/examples/sieve.py` & `rasterio-1.4a2/examples/sieve.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/examples/thread_pool_executor.py` & `rasterio-1.4a2/examples/thread_pool_executor.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/examples/total.py` & `rasterio-1.4a2/examples/total.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/pyproject.toml` & `rasterio-1.4a2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/__init__.py` & `rasterio-1.4a2/rasterio/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
     class FilePath:
         pass
 
     have_vsi_plugin = False
 
 __all__ = ['band', 'open', 'pad', 'Band', 'Env', 'CRS']
-__version__ = "1.4a1"
+__version__ = "1.4a2"
 __gdal_version__ = gdal_version()
 __proj_version__ = ".".join([str(version) for version in get_proj_version()])
 __geos_version__ = ".".join([str(version) for version in get_geos_version()])
 
 # Rasterio attaches NullHandler to the 'rasterio' logger and its
 # descendents. See
 # https://docs.python.org/2/howto/logging.html#configuring-logging-for-a-library
```

### Comparing `rasterio-1.4a1/rasterio/_base.pxd` & `rasterio-1.4a2/rasterio/_base.pxd`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/_base.pyx` & `rasterio-1.4a2/rasterio/_base.pyx`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/_env.pyx` & `rasterio-1.4a2/rasterio/_env.pyx`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/_err.pyx` & `rasterio-1.4a2/rasterio/_err.pyx`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/_example.pyx` & `rasterio-1.4a2/rasterio/_example.pyx`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/_features.pxd` & `rasterio-1.4a2/rasterio/_features.pxd`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/_features.pyx` & `rasterio-1.4a2/rasterio/_features.pyx`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/_filepath.pyx` & `rasterio-1.4a2/rasterio/_filepath.pyx`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/_fill.pyx` & `rasterio-1.4a2/rasterio/_fill.pyx`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/_io.pxd` & `rasterio-1.4a2/rasterio/_io.pxd`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/_io.pyx` & `rasterio-1.4a2/rasterio/_io.pyx`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/_path.py` & `rasterio-1.4a2/rasterio/_path.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Dataset paths, identifiers, and filenames
 
 Note: this module is not part of Rasterio's API. It is for internal use
 only.
 
 """
 
+import os
 import pathlib
 import re
 import sys
 from urllib.parse import urlparse
 
 import attr
 
@@ -61,32 +62,39 @@
     path = attr.ib()
     archive = attr.ib()
     scheme = attr.ib()
 
     @classmethod
     def from_uri(cls, uri):
         parts = urlparse(uri)
-        path = pathlib.Path(parts.path).as_posix() if parts.path else parts.path
+        if sys.platform == "win32" and re.match(r"^[a-zA-Z]\:", parts.netloc):
+            parsed_path = f"{parts.netloc}{parts.path}"
+            parsed_netloc = None
+        else:
+            parsed_path = parts.path
+            parsed_netloc = parts.netloc
+
+        path = parsed_path
         scheme = parts.scheme or None
 
         if parts.query:
             path += "?" + parts.query
 
         if scheme and scheme.startswith(("gzip", "tar", "zip")):
             path_parts = path.split('!')
             path = path_parts.pop() if path_parts else None
             archive = path_parts.pop() if path_parts else None
         else:
             archive = None
 
-        if parts.scheme and parts.netloc:
+        if scheme and parsed_netloc:
             if archive:
-                archive = parts.netloc + archive
+                archive = parsed_netloc + archive
             else:
-                path = parts.netloc + path
+                path = parsed_netloc + path
 
         return _ParsedPath(path, archive, scheme)
 
     @property
     def name(self):
         """The parsed path's original URI"""
         if not self.scheme:
@@ -140,39 +148,29 @@
     -----
     When legacy GDAL filenames are encountered, they will be returned
     in a UnparsedPath.
 
     """
     if isinstance(path, _Path):
         return path
-
-    elif pathlib and isinstance(path, pathlib.PurePath):
-        return _ParsedPath(path.as_posix(), None, None)
-
+    elif isinstance(path, pathlib.PurePath):
+        return _ParsedPath(os.fspath(path), None, None)
     elif isinstance(path, str):
-
         if sys.platform == "win32" and re.match(r"^[a-zA-Z]\:", path):
-            if pathlib:
-                return _ParsedPath(pathlib.Path(path).as_posix(), None, None)
-            else:
-                return _UnparsedPath(path)
-
+            return _ParsedPath(path, None, None)
         elif path.startswith('/vsi'):
             return _UnparsedPath(path)
-
         else:
             parts = urlparse(path)
-
     else:
         raise PathError("invalid path '{!r}'".format(path))
 
     # if the scheme is not one of Rasterio's supported schemes, we
     # return an UnparsedPath.
     if parts.scheme:
-
         if all(p in SCHEMES for p in parts.scheme.split('+')):
             return _ParsedPath.from_uri(path)
 
     return _UnparsedPath(path)
 
 
 def _vsi_path(path):
```

### Comparing `rasterio-1.4a1/rasterio/_show_versions.py` & `rasterio-1.4a2/rasterio/_show_versions.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/_transform.pyx` & `rasterio-1.4a2/rasterio/_transform.pyx`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/_vendor/snuggs.py` & `rasterio-1.4a2/rasterio/_vendor/snuggs.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/_version.pyx` & `rasterio-1.4a2/rasterio/_version.pyx`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/_warp.pxd` & `rasterio-1.4a2/rasterio/_warp.pxd`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/_warp.pyx` & `rasterio-1.4a2/rasterio/_warp.pyx`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/control.py` & `rasterio-1.4a2/rasterio/control.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/coords.py` & `rasterio-1.4a2/rasterio/coords.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/crs.pyx` & `rasterio-1.4a2/rasterio/crs.pyx`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/drivers.py` & `rasterio-1.4a2/rasterio/drivers.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/dtypes.py` & `rasterio-1.4a2/rasterio/dtypes.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/enums.py` & `rasterio-1.4a2/rasterio/enums.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/env.py` & `rasterio-1.4a2/rasterio/env.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/errors.py` & `rasterio-1.4a2/rasterio/errors.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/features.py` & `rasterio-1.4a2/rasterio/features.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/fill.py` & `rasterio-1.4a2/rasterio/fill.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/gdal.pxi` & `rasterio-1.4a2/rasterio/gdal.pxi`

 * *Files 0% similar despite different names*

```diff
@@ -55,24 +55,22 @@
     const char *CSLFetchNameValue(char **papszStrList, const char *pszName)
     char **CSLSetNameValue(char **list, char *name, char *val)
     void CSLDestroy(char **list)
     char **CSLMerge(char **first, char **second)
     const char* CPLParseNameValue(const char *pszNameValue, char **ppszKey)
 
 
-cdef extern from "sys/stat.h" nogil:
-    struct stat:
-        pass
-
-
 cdef extern from "cpl_vsi.h" nogil:
 
     ctypedef unsigned long long vsi_l_offset
     ctypedef FILE VSILFILE
-    ctypedef stat VSIStatBufL
+    ctypedef struct VSIStatBufL:
+        long st_size
+        long st_mode
+        int st_mtime
     ctypedef enum VSIRangeStatus:
         VSI_RANGE_STATUS_UNKNOWN,
         VSI_RANGE_STATUS_DATA,
         VSI_RANGE_STATUS_HOLE,
 
     # GDAL Plugin System (GDAL 3.0+)
     # Filesystem functions
```

### Comparing `rasterio-1.4a1/rasterio/io.py` & `rasterio-1.4a2/rasterio/io.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/mask.py` & `rasterio-1.4a2/rasterio/mask.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/merge.py` & `rasterio-1.4a2/rasterio/merge.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/path.py` & `rasterio-1.4a2/rasterio/path.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/plot.py` & `rasterio-1.4a2/rasterio/plot.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/profiles.py` & `rasterio-1.4a2/rasterio/profiles.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/rio/blocks.py` & `rasterio-1.4a2/rasterio/rio/blocks.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/rio/bounds.py` & `rasterio-1.4a2/rasterio/rio/bounds.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/rio/calc.py` & `rasterio-1.4a2/rasterio/rio/calc.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/rio/clip.py` & `rasterio-1.4a2/rasterio/rio/clip.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/rio/convert.py` & `rasterio-1.4a2/rasterio/rio/convert.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/rio/create.py` & `rasterio-1.4a2/rasterio/rio/create.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/rio/edit_info.py` & `rasterio-1.4a2/rasterio/rio/edit_info.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/rio/env.py` & `rasterio-1.4a2/rasterio/rio/env.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/rio/gcps.py` & `rasterio-1.4a2/rasterio/rio/gcps.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/rio/helpers.py` & `rasterio-1.4a2/rasterio/rio/helpers.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/rio/info.py` & `rasterio-1.4a2/rasterio/rio/info.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/rio/insp.py` & `rasterio-1.4a2/rasterio/rio/insp.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/rio/main.py` & `rasterio-1.4a2/rasterio/rio/main.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/rio/mask.py` & `rasterio-1.4a2/rasterio/rio/mask.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/rio/merge.py` & `rasterio-1.4a2/rasterio/rio/merge.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/rio/options.py` & `rasterio-1.4a2/rasterio/rio/options.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,17 +218,15 @@
         return retval
 
 
 # Singular input file
 file_in_arg = click.argument('INPUT', callback=file_in_handler)
 
 # Singular output file
-file_out_arg = click.argument(
-    'OUTPUT',
-    type=click.Path(resolve_path=True))
+file_out_arg = click.argument("OUTPUT", type=click.Path())
 
 # Multiple input files.
 files_in_arg = click.argument(
     'files',
     nargs=-1,
     type=click.Path(),
     required=True,
@@ -297,15 +295,15 @@
     default=True,
     help="Evaluate expressions using masked arrays (the default) or ordinary "
          "numpy arrays.")
 
 output_opt = click.option(
     '-o', '--output',
     default=None,
-    type=click.Path(resolve_path=True),
+    type=click.Path(),
     help="Path to output file (optional alternative to a positional arg).")
 
 resolution_opt = click.option(
     '-r', '--res',
     multiple=True, type=float, default=None,
     help='Output dataset resolution in units of coordinate '
          'reference system. Pixels assumed to be square if this option '
```

### Comparing `rasterio-1.4a1/rasterio/rio/overview.py` & `rasterio-1.4a2/rasterio/rio/overview.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/rio/rasterize.py` & `rasterio-1.4a2/rasterio/rio/rasterize.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/rio/rm.py` & `rasterio-1.4a2/rasterio/rio/rm.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/rio/sample.py` & `rasterio-1.4a2/rasterio/rio/sample.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/rio/shapes.py` & `rasterio-1.4a2/rasterio/rio/shapes.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/rio/stack.py` & `rasterio-1.4a2/rasterio/rio/stack.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/rio/transform.py` & `rasterio-1.4a2/rasterio/rio/transform.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/rio/warp.py` & `rasterio-1.4a2/rasterio/rio/warp.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/rpc.py` & `rasterio-1.4a2/rasterio/rpc.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/sample.py` & `rasterio-1.4a2/rasterio/sample.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/session.py` & `rasterio-1.4a2/rasterio/session.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/shutil.pyx` & `rasterio-1.4a2/rasterio/shutil.pyx`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/tools.py` & `rasterio-1.4a2/rasterio/tools.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/transform.py` & `rasterio-1.4a2/rasterio/transform.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/vrt.py` & `rasterio-1.4a2/rasterio/vrt.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/warp.py` & `rasterio-1.4a2/rasterio/warp.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio/windows.py` & `rasterio-1.4a2/rasterio/windows.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio.egg-info/PKG-INFO` & `rasterio-1.4a2/rasterio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rasterio
-Version: 1.4a1
+Version: 1.4a2
 Summary: Fast and direct raster I/O for use with Numpy and SciPy
 Home-page: https://github.com/rasterio/rasterio
 Author: Sean Gillies
 Author-email: sean@mapbox.com
 License: BSD
 Keywords: raster gdal
 Platform: UNKNOWN
@@ -19,20 +19,20 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Graphics :: Graphics Conversion
 Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Python: >=3.9
-Provides-Extra: all
 Provides-Extra: docs
 Provides-Extra: ipython
 Provides-Extra: plot
 Provides-Extra: s3
 Provides-Extra: test
+Provides-Extra: all
 License-File: LICENSE.txt
 License-File: AUTHORS.txt
 
 ========
 Rasterio
 ========
```

### Comparing `rasterio-1.4a1/rasterio.egg-info/SOURCES.txt` & `rasterio-1.4a2/rasterio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio.egg-info/entry_points.txt` & `rasterio-1.4a2/rasterio.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/rasterio.egg-info/requires.txt` & `rasterio-1.4a2/rasterio.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 affine
 attrs
 certifi
-click-plugins
 click>=4.0
 cligj>=0.5
 numpy<2
+click-plugins
 pyparsing
 setuptools
 
 [all]
+sphinx-click
 boto3>=1.2.4
+packaging
+sphinx-rtd-theme
+numpydoc
 ghp-import
+sphinx
+pytest-cov>=2.2.0
 hypothesis
 ipython>=2.0
-matplotlib
-numpydoc
-packaging
-pytest-cov>=2.2.0
 pytest>=2.8.2
-sphinx
-sphinx-click
-sphinx-rtd-theme
+matplotlib
 
 [all:python_version < "3.12"]
 shapely
 
 [docs]
 ghp-import
 numpydoc
```

### Comparing `rasterio-1.4a1/setup.cfg` & `rasterio-1.4a2/setup.cfg`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/setup.py` & `rasterio-1.4a2/setup.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/README.rst` & `rasterio-1.4a2/tests/README.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/conftest.py` & `rasterio-1.4a2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/data/README.rst` & `rasterio-1.4a2/tests/data/README.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/rangehttpserver.py` & `rasterio-1.4a2/tests/rangehttpserver.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test__env.py` & `rasterio-1.4a2/tests/test__env.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test__version.py` & `rasterio-1.4a2/tests/test__version.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_band_masks.py` & `rasterio-1.4a2/tests/test_band_masks.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_blocks.py` & `rasterio-1.4a2/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_boundless_read.py` & `rasterio-1.4a2/tests/test_boundless_read.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_checksum.py` & `rasterio-1.4a2/tests/test_checksum.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_cli_main.py` & `rasterio-1.4a2/tests/test_cli_main.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_colorinterp.py` & `rasterio-1.4a2/tests/test_colorinterp.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_colormap.py` & `rasterio-1.4a2/tests/test_colormap.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_complex_dtypes.py` & `rasterio-1.4a2/tests/test_complex_dtypes.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_coords.py` & `rasterio-1.4a2/tests/test_coords.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_creation_options.py` & `rasterio-1.4a2/tests/test_creation_options.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_crs.py` & `rasterio-1.4a2/tests/test_crs.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_dataset.py` & `rasterio-1.4a2/tests/test_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """High level tests for Rasterio's ``GDALDataset`` abstractions."""
 
 
 import math
+import os
 from pathlib import Path
 from unittest.mock import MagicMock
 
 import pytest
 
 import rasterio
 from rasterio.coords import BoundingBox
@@ -18,15 +19,15 @@
 
 def test_files(data):
     tif = Path(data).joinpath('RGB.byte.tif')
     aux = tif.parent.joinpath(tif.name + '.aux.xml')
     with open(aux, 'w'):
         pass
     with rasterio.open(tif) as src:
-        assert src.files == [tif.as_posix(), aux.as_posix()]
+        assert src.files == [os.fspath(tif), os.fspath(aux)]
 
 
 def test_handle_closed(path_rgb_byte_tif):
     """Code that calls ``DatasetBase.handle()`` after it has been closed
     should raise an exception.
     """
     with rasterio.open(path_rgb_byte_tif) as src:
```

### Comparing `rasterio-1.4a1/tests/test_dataset_mask.py` & `rasterio-1.4a2/tests/test_dataset_mask.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_dataset_rw.py` & `rasterio-1.4a2/tests/test_dataset_rw.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_descriptions.py` & `rasterio-1.4a2/tests/test_descriptions.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_driver_management.py` & `rasterio-1.4a2/tests/test_driver_management.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_dtypes.py` & `rasterio-1.4a2/tests/test_dtypes.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_env.py` & `rasterio-1.4a2/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_err.py` & `rasterio-1.4a2/tests/test_err.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_features.py` & `rasterio-1.4a2/tests/test_features.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_filepath.py` & `rasterio-1.4a2/tests/test_filepath.py`

 * *Files 2% similar despite different names*

```diff
@@ -222,15 +222,7 @@
     """Expect no warning or error level log messages about .aux or .hdr files."""
     with caplog.at_level(logging.WARNING):
         with open(path_rgb_byte_tif, "rb") as f, FilePath(f) as vsi_file:
             with vsi_file.open() as src:
                 _ = src.profile
 
         assert "not found in virtual filesystem" not in caplog.text
-
-import io
-
-
-def test_opener(path_rgb_byte_tif):
-    """First test of vsi python plugin opener."""
-    with rasterio.open(path_rgb_byte_tif, opener=io.open) as src:
-        _ = src.profile
```

### Comparing `rasterio-1.4a1/tests/test_fillnodata.py` & `rasterio-1.4a2/tests/test_fillnodata.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_gcps.py` & `rasterio-1.4a2/tests/test_gcps.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_gdal_raster_io.py` & `rasterio-1.4a2/tests/test_gdal_raster_io.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_image_structure.py` & `rasterio-1.4a2/tests/test_image_structure.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_indexing.py` & `rasterio-1.4a2/tests/test_indexing.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_int8.py` & `rasterio-1.4a2/tests/test_int8.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_io.py` & `rasterio-1.4a2/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_io_mixins.py` & `rasterio-1.4a2/tests/test_io_mixins.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_mask.py` & `rasterio-1.4a2/tests/test_mask.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_mask_creation.py` & `rasterio-1.4a2/tests/test_mask_creation.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_memoryfile.py` & `rasterio-1.4a2/tests/test_memoryfile.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_merge.py` & `rasterio-1.4a2/tests/test_merge.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_meta.py` & `rasterio-1.4a2/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_no_georef.py` & `rasterio-1.4a2/tests/test_no_georef.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_nodata.py` & `rasterio-1.4a2/tests/test_nodata.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_open.py` & `rasterio-1.4a2/tests/test_open.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_open_options.py` & `rasterio-1.4a2/tests/test_open_options.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_open_overview_level.py` & `rasterio-1.4a2/tests/test_open_overview_level.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_open_sharing.py` & `rasterio-1.4a2/tests/test_open_sharing.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_overviews.py` & `rasterio-1.4a2/tests/test_overviews.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_path.py` & `rasterio-1.4a2/tests/test_path.py`

 * *Files 4% similar despite different names*

```diff
@@ -227,16 +227,28 @@
 
 
 def test_parse_path_win():
     pathlib = pytest.importorskip("pathlib")
     assert isinstance(_parse_path(pathlib.PureWindowsPath(r"C:\foo\bar.tif")), _ParsedPath)
 
 
-def test_parse_path_win_no_pathlib(monkeypatch):
-    monkeypatch.setattr(rasterio._path.sys, "platform", "win32")
-    monkeypatch.setattr(rasterio._path, "pathlib", None)
-    assert isinstance(_parse_path(r"C:\foo\bar.tif"), _UnparsedPath)
-
-
 def test_parse_gdal_vsi_alias():
     """Check that the alias function works"""
     assert _parse_path('/vsifoo/bar').path == '/vsifoo/bar'
+
+
+def test_parse_zip_windows(monkeypatch):
+    """Parse a zip+ Windows path."""
+    monkeypatch.setattr(sys, "platform", "win32")
+    path = _parse_path("zip://D:\\a\\Fiona\\Fiona\\tests\\data\\coutwildrnp.zip!coutwildrnp.shp")
+    vsi_path = _vsi_path(path)
+    assert vsi_path.startswith("/vsizip/D")
+    assert vsi_path.endswith("coutwildrnp.zip/coutwildrnp.shp")
+
+
+def test_parse_zip_windows(monkeypatch):
+    """Parse a tar+ Windows path."""
+    monkeypatch.setattr(sys, "platform", "win32")
+    path = _parse_path("tar://D:\\a\\Fiona\\Fiona\\tests\\data\\coutwildrnp.tar!testing/coutwildrnp.shp")
+    vsi_path = _vsi_path(path)
+    assert vsi_path.startswith("/vsitar/D")
+    assert vsi_path.endswith("coutwildrnp.tar/testing/coutwildrnp.shp")
```

### Comparing `rasterio-1.4a1/tests/test_plot.py` & `rasterio-1.4a2/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_png.py` & `rasterio-1.4a2/tests/test_png.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_process_pool_executor.py` & `rasterio-1.4a2/tests/test_process_pool_executor.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_profile.py` & `rasterio-1.4a2/tests/test_profile.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_pyopener.py` & `rasterio-1.4a2/tests/test_pyopener.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,86 +1,103 @@
 """Tests of the Python opener VSI plugin."""
 
-import zipfile
 import io
+import os
+import zipfile
 
 import fsspec
 import numpy as np
 import pytest
 
 import rasterio
 from rasterio.enums import MaskFlags
-from rasterio.errors import RasterioIOError, OpenerRegistrationError
+from rasterio.errors import OpenerRegistrationError
 
 
 def test_registration_failure():
     """Exception is raised on attempt to register a second opener for a filename and mode."""
     with pytest.raises(OpenerRegistrationError) as exc_info:
         with rasterio.open(
             "tests/data/RGB.byte.tif", opener=io.open
-        ) as a, rasterio.open("tests/data/RGB.byte.tif", opener=int) as b:
+        ) as a, rasterio.open("tests/data/RGB.byte.tif", opener=fsspec.open) as b:
             pass
 
-    assert exc_info.value.args[0] == "Opener already registered for urlpath and mode"
+    assert exc_info.value.args[0] == "Opener already registered for urlpath and mode."
 
 
 def test_opener_failure():
     """Use int as an opener :)"""
-    with pytest.raises(RasterioIOError) as exc_info:
+    with pytest.raises(OpenerRegistrationError) as exc_info:
         rasterio.open("tests/data/RGB.byte.tif", opener=int)
 
-    assert (
-        exc_info.value.args[0]
-        == "Opener failed to open file with arguments ('tests/data/RGB.byte.tif', 'rb'): TypeError(\"'str' object cannot be interpreted as an integer\")"
-    )
-
 
 def test_opener_io_open():
     """Use io.open as opener."""
     with rasterio.open("tests/data/RGB.byte.tif", opener=io.open) as src:
         profile = src.profile
         assert profile["driver"] == "GTiff"
         assert profile["count"] == 3
 
 
+def test_opener_zipfile_open():
+    """Use zipfile as opener."""
+    with zipfile.ZipFile("tests/data/files.zip") as zf:
+        with rasterio.open("RGB.byte.tif", opener=zf.open) as src:
+            profile = src.profile
+            assert profile["driver"] == "GTiff"
+            assert profile["count"] == 3
+
+
 @pytest.mark.parametrize(
     "urlpath", ["file://tests/data/RGB.byte.tif", "zip://*.tif::tests/data/files.zip"]
 )
 def test_opener_fsspec_open(urlpath):
     """Use fsspec.open as opener."""
     with rasterio.open(urlpath, opener=fsspec.open) as src:
         profile = src.profile
         assert profile["driver"] == "GTiff"
         assert profile["count"] == 3
 
 
+def test_opener_fsspec_fs_open():
+    """Use fsspec filesystem open() as opener."""
+    fs = fsspec.filesystem("file")
+    with rasterio.open("tests/data/RGB.byte.tif", opener=fs.open) as src:
+        profile = src.profile
+        assert profile["driver"] == "GTiff"
+        assert profile["count"] == 3
+
+
 def test_opener_fsspec_fs():
     """Use fsspec filesystem as opener."""
     fs = fsspec.filesystem("file")
-    with rasterio.open("tests/data/RGB.byte.tif", opener=fs.open) as src:
+    with rasterio.open("tests/data/RGB.byte.tif", opener=fs) as src:
         profile = src.profile
         assert profile["driver"] == "GTiff"
         assert profile["count"] == 3
 
 
-def test_opener_zipfile_open():
-    """Use zipfile as opener."""
-    with zipfile.ZipFile("tests/data/files.zip") as zf:
-        with rasterio.open("RGB.byte.tif", opener=zf.open) as src:
-            profile = src.profile
-            assert profile["driver"] == "GTiff"
-            assert profile["count"] == 3
+def test_opener_fsspec_http_fs():
+    """Use fsspec http filesystem as opener."""
+    fs = fsspec.filesystem("http")
+    with rasterio.open(
+        "https://raw.githubusercontent.com/rasterio/rasterio/main/tests/data/float32.tif",
+        opener=fs,
+    ) as src:
+        profile = src.profile
+        assert profile["driver"] == "GTiff"
+        assert profile["count"] == 1
 
 
-def test_opener_fsspec_fs_write(tmp_path):
-    """Use fsspec filesystem as opener for writing."""
+def test_opener_fsspec_fs_open_write(tmp_path):
+    """Use fsspec filesystem open() as opener for writing."""
     data = np.ma.masked_less_equal(np.array([[0, 1, 2]], dtype="uint8"), 1)
     fs = fsspec.filesystem("file")
     with rasterio.open(
-        (tmp_path / "test.tif").as_posix(),
+        os.fspath(tmp_path / "test.tif"),
         "w",
         driver="GTiff",
         count=1,
         width=3,
         height=1,
         dtype="uint8",
         nodata=0,
@@ -91,18 +108,42 @@
     # Expect the dataset's nodata value in the first two pixels.
     with rasterio.open(tmp_path / "test.tif") as src:
         assert src.mask_flag_enums == ([MaskFlags.nodata],)
         arr = src.read()
         assert list(arr.flatten()) == [0, 0, 2]
 
 
+def test_opener_fsspec_fs_write(tmp_path):
+    """Use fsspec filesystem open() as opener for writing."""
+    data = np.ma.masked_less_equal(np.array([[0, 1, 2]], dtype="uint8"), 1)
+    fs = fsspec.filesystem("file")
+    with rasterio.open(
+        os.fspath(tmp_path / "test.tif"),
+        "w",
+        driver="GTiff",
+        count=1,
+        width=3,
+        height=1,
+        dtype="uint8",
+        nodata=0,
+        opener=fs,
+    ) as dst:
+        dst.write(data, indexes=1)
+
+    # Expect the dataset's nodata value in the first two pixels.
+    with rasterio.open(tmp_path / "test.tif") as src:
+        assert src.mask_flag_enums == ([MaskFlags.nodata],)
+        arr = src.read()
+        assert list(arr.flatten()) == [0, 0, 2]
+
+
 def test_fp_fsspec_openfile_write(tmp_path):
     """Use an fsspec OpenFile for writing."""
     data = np.ma.masked_less_equal(np.array([[0, 1, 2]], dtype="uint8"), 1)
-    of = fsspec.open((tmp_path / "test.tif").as_posix(), "wb")
+    of = fsspec.open(os.fspath(tmp_path / "test.tif"), "wb")
     with rasterio.open(
         of,
         "w",
         driver="GTiff",
         count=1,
         width=3,
         height=1,
@@ -112,7 +153,45 @@
         dst.write(data, indexes=1)
 
     # Expect the dataset's nodata value in the first two pixels.
     with rasterio.open(tmp_path / "test.tif") as src:
         assert src.mask_flag_enums == ([MaskFlags.nodata],)
         arr = src.read()
         assert list(arr.flatten()) == [0, 0, 2]
+
+
+def test_opener_msk_sidecar():
+    """Access .msk sidecar file via opener."""
+    # This test fails before issue 3027 is resolved because
+    # RGB2.byte.tif.msk is not found.
+    with rasterio.open("tests/data/RGB2.byte.tif", opener=io.open) as src:
+        for val in src.mask_flag_enums:
+            assert val == [MaskFlags.per_dataset]
+
+
+def test_fsspec_msk_sidecar():
+    """Access .msk sidecar file via fsspec."""
+    fs = fsspec.filesystem("file")
+    with rasterio.open("tests/data/RGB2.byte.tif", opener=fs) as src:
+        for val in src.mask_flag_enums:
+            assert val == [MaskFlags.per_dataset]
+
+
+def test_fsspec_http_msk_sidecar():
+    """Use fsspec http filesystem as opener."""
+    fs = fsspec.filesystem("http")
+    with rasterio.open(
+        "https://raw.githubusercontent.com/rasterio/rasterio/main/tests/data/RGB2.byte.tif",
+        opener=fs,
+    ) as src:
+        for val in src.mask_flag_enums:
+            assert val == [MaskFlags.per_dataset]
+
+
+def test_opener_tiledb_vfs():
+    """Use tiledb virtual filesystem as opener."""
+    tiledb = pytest.importorskip("tiledb")
+    fs = tiledb.VFS()
+    with rasterio.open("tests/data/RGB.byte.tif", opener=fs) as src:
+        profile = src.profile
+        assert profile["driver"] == "GTiff"
+        assert profile["count"] == 3
```

### Comparing `rasterio-1.4a1/tests/test_read.py` & `rasterio-1.4a2/tests/test_read.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_read_boundless.py` & `rasterio-1.4a2/tests/test_read_boundless.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_read_dtype.py` & `rasterio-1.4a2/tests/test_read_dtype.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_read_resample.py` & `rasterio-1.4a2/tests/test_read_resample.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_reshape_image.py` & `rasterio-1.4a2/tests/test_reshape_image.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_revolvingdoor.py` & `rasterio-1.4a2/tests/test_revolvingdoor.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_rio_blocks.py` & `rasterio-1.4a2/tests/test_rio_blocks.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_rio_bounds.py` & `rasterio-1.4a2/tests/test_rio_bounds.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_rio_calc.py` & `rasterio-1.4a2/tests/test_rio_calc.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_rio_clip.py` & `rasterio-1.4a2/tests/test_rio_clip.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_rio_convert.py` & `rasterio-1.4a2/tests/test_rio_convert.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_rio_create.py` & `rasterio-1.4a2/tests/test_rio_create.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_rio_edit_info.py` & `rasterio-1.4a2/tests/test_rio_edit_info.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_rio_env.py` & `rasterio-1.4a2/tests/test_rio_env.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_rio_gcp.py` & `rasterio-1.4a2/tests/test_rio_gcp.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_rio_helpers.py` & `rasterio-1.4a2/tests/test_rio_helpers.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_rio_info.py` & `rasterio-1.4a2/tests/test_rio_info.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_rio_insp.py` & `rasterio-1.4a2/tests/test_rio_insp.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_rio_main.py` & `rasterio-1.4a2/tests/test_rio_main.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_rio_mask.py` & `rasterio-1.4a2/tests/test_rio_mask.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_rio_merge.py` & `rasterio-1.4a2/tests/test_rio_merge.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_rio_options.py` & `rasterio-1.4a2/tests/test_rio_options.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_rio_overview.py` & `rasterio-1.4a2/tests/test_rio_overview.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_rio_rasterize.py` & `rasterio-1.4a2/tests/test_rio_rasterize.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_rio_rm.py` & `rasterio-1.4a2/tests/test_rio_rm.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_rio_sample.py` & `rasterio-1.4a2/tests/test_rio_sample.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_rio_shapes.py` & `rasterio-1.4a2/tests/test_rio_shapes.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_rio_stack.py` & `rasterio-1.4a2/tests/test_rio_stack.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_rio_warp.py` & `rasterio-1.4a2/tests/test_rio_warp.py`

 * *Files 0% similar despite different names*

```diff
@@ -577,29 +577,29 @@
 
     print(result.output)
     assert result.exit_code == 0
 
 
 def test_unrotate(runner, tmp_path):
     """rio-warp unrotates imagery by default, like gdalwarp"""
-    outputname = tmp_path.joinpath("test.tif").as_posix()
+    outputname = os.fspath(tmp_path.joinpath("test.tif"))
     runner.invoke(main_group, ["warp", "tests/data/rotated.tif", outputname])
 
     # There is no skew in the output.
     with rasterio.open(outputname) as src:
         assert src.transform.b == 0.0
         assert src.transform.d == 0.0
 
 
 @pytest.mark.parametrize(
     "wotopt", ["--to", "--transformer-option", "--wo", "--warper-option"]
 )
 def test_coordinate_operation(runner, tmp_path, wotopt):
     """Verify that transformer coordinate operations are activated."""
-    outputname = tmp_path.joinpath("test.tif").as_posix()
+    outputname = os.fspath(tmp_path.joinpath("test.tif"))
     pipeline = "+proj=pipeline step inv proj=utm zone=11 ellps=clrk66 step proj=unitconvert xy_in=rad xy_out=deg step proj=axisswap order=2,1"
     result = runner.invoke(
         main_group,
         [
             "warp",
             "--dst-crs",
             "EPSG:4326",
```

### Comparing `rasterio-1.4a1/tests/test_rpcs.py` & `rasterio-1.4a2/tests/test_rpcs.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_sampling.py` & `rasterio-1.4a2/tests/test_sampling.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_scale_offset.py` & `rasterio-1.4a2/tests/test_scale_offset.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_session.py` & `rasterio-1.4a2/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_show_versions.py` & `rasterio-1.4a2/tests/test_show_versions.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_shutil.py` & `rasterio-1.4a2/tests/test_shutil.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_statistics.py` & `rasterio-1.4a2/tests/test_statistics.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_subdatasets.py` & `rasterio-1.4a2/tests/test_subdatasets.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_tag_item.py` & `rasterio-1.4a2/tests/test_tag_item.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_tags.py` & `rasterio-1.4a2/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_thread_pool_executor.py` & `rasterio-1.4a2/tests/test_thread_pool_executor.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_threading.py` & `rasterio-1.4a2/tests/test_threading.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_tools.py` & `rasterio-1.4a2/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_transform.py` & `rasterio-1.4a2/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_units.py` & `rasterio-1.4a2/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_update.py` & `rasterio-1.4a2/tests/test_update.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_vrt.py` & `rasterio-1.4a2/tests/test_vrt.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_warnings.py` & `rasterio-1.4a2/tests/test_warnings.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_warp.py` & `rasterio-1.4a2/tests/test_warp.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_warp_transform.py` & `rasterio-1.4a2/tests/test_warp_transform.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_warpedvrt.py` & `rasterio-1.4a2/tests/test_warpedvrt.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,15 +152,15 @@
     with rasterio.open(path_rgb_byte_tif) as src:
         vrt = WarpedVRT(src, crs=DST_CRS)
         assert vrt.crs == CRS.from_string(DST_CRS)
         assert tuple(round(x, 1) for x in vrt.bounds) == (
             -8789636.7, 2700460.0, -8524406.4, 2943560.2
         )
         assert vrt.name.startswith("WarpedVRT(")
-        assert vrt.name.endswith("tests/data/RGB.byte.tif)")
+        assert vrt.name.endswith("RGB.byte.tif)")
         assert vrt.indexes == (1, 2, 3)
         assert vrt.nodatavals == (0, 0, 0)
         assert vrt.dtypes == ("uint8", "uint8", "uint8")
         assert vrt.read().shape == (3, 736, 803)
 
 
 def test_warped_vrt_dimensions(path_rgb_byte_tif):
```

### Comparing `rasterio-1.4a1/tests/test_windows.py` & `rasterio-1.4a2/tests/test_windows.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_windows_mixins.py` & `rasterio-1.4a2/tests/test_windows_mixins.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.4a1/tests/test_write.py` & `rasterio-1.4a2/tests/test_write.py`

 * *Files identical despite different names*

