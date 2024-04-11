# Comparing `tmp/pygerber-2.2.1.tar.gz` & `tmp/pygerber-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygerber-2.2.1.tar", max compression
+gzip compressed data, was "pygerber-2.3.0.tar", max compression
```

## Comparing `pygerber-2.2.1.tar` & `pygerber-2.3.0.tar`

### file list

```diff
@@ -1,222 +1,232 @@
--rw-r--r--   0        0        0     1069 2024-01-27 03:27:07.045241 pygerber-2.2.1/LICENSE.md
--rw-r--r--   0        0        0    13029 2024-01-27 03:27:07.045241 pygerber-2.2.1/README.md
--rw-r--r--   0        0        0    12959 2024-01-27 03:27:07.181241 pygerber-2.2.1/pyproject.toml
--rw-r--r--   0        0        0      103 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/__init__.py
--rw-r--r--   0        0        0      149 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/__main__.py
--rw-r--r--   0        0        0      858 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/backend/__init__.py
--rw-r--r--   0        0        0       61 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/backend/abstract/__init__.py
--rw-r--r--   0        0        0     4205 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/backend/abstract/aperture_handle.py
--rw-r--r--   0        0        0     6118 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/backend/abstract/backend_cls.py
--rw-r--r--   0        0        0       50 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/backend/abstract/draw_commands/__init__.py
--rw-r--r--   0        0        0     3958 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/backend/abstract/draw_commands/draw_arc.py
--rw-r--r--   0        0        0     1165 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/backend/abstract/draw_commands/draw_bounding_box.py
--rw-r--r--   0        0        0     1214 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/backend/abstract/draw_commands/draw_circle.py
--rw-r--r--   0        0        0     1007 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/backend/abstract/draw_commands/draw_command.py
--rw-r--r--   0        0        0     1226 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/backend/abstract/draw_commands/draw_paste.py
--rw-r--r--   0        0        0     1527 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/backend/abstract/draw_commands/draw_polygon.py
--rw-r--r--   0        0        0     1323 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/backend/abstract/draw_commands/draw_rectangle.py
--rw-r--r--   0        0        0     1395 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/backend/abstract/draw_commands/draw_region.py
--rw-r--r--   0        0        0     1707 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/backend/abstract/draw_commands/draw_vector_line.py
--rw-r--r--   0        0        0      793 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/backend/abstract/draw_commands_handle.py
--rw-r--r--   0        0        0     1101 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/backend/abstract/drawing_target.py
--rw-r--r--   0        0        0      280 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/backend/abstract/errors.py
--rw-r--r--   0        0        0      663 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/backend/abstract/result_handle.py
--rw-r--r--   0        0        0       65 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/backend/rasterized_2d/__init__.py
--rw-r--r--   0        0        0     2435 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/backend/rasterized_2d/aperture_handle.py
--rw-r--r--   0        0        0     8530 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/backend/rasterized_2d/backend_cls.py
--rw-r--r--   0        0        0     8070 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/backend/rasterized_2d/color_scheme.py
--rw-r--r--   0        0        0       81 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/backend/rasterized_2d/draw_commands/__init__.py
--rw-r--r--   0        0        0     1371 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/backend/rasterized_2d/draw_commands/draw_arc.py
--rw-r--r--   0        0        0     1583 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/backend/rasterized_2d/draw_commands/draw_bounding_box.py
--rw-r--r--   0        0        0     1702 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/backend/rasterized_2d/draw_commands/draw_circle.py
--rw-r--r--   0        0        0     2072 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/backend/rasterized_2d/draw_commands/draw_paste.py
--rw-r--r--   0        0        0     2139 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/backend/rasterized_2d/draw_commands/draw_polygon.py
--rw-r--r--   0        0        0     1634 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/backend/rasterized_2d/draw_commands/draw_rectangle.py
--rw-r--r--   0        0        0     1616 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/backend/rasterized_2d/draw_commands/draw_region.py
--rw-r--r--   0        0        0     1389 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/backend/rasterized_2d/draw_commands/draw_vector_line.py
--rw-r--r--   0        0        0      317 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/backend/rasterized_2d/draw_commands_handle.py
--rw-r--r--   0        0        0     4122 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/backend/rasterized_2d/drawing_target.py
--rw-r--r--   0        0        0      520 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/backend/rasterized_2d/errors.py
--rw-r--r--   0        0        0      801 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/backend/rasterized_2d/image_tools.py
--rw-r--r--   0        0        0     1589 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/backend/rasterized_2d/result_handle.py
--rw-r--r--   0        0        0       53 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/common/__init__.py
--rw-r--r--   0        0        0      202 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/common/error.py
--rw-r--r--   0        0        0      369 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/common/frozen_general_model.py
--rw-r--r--   0        0        0      364 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/common/general_model.py
--rw-r--r--   0        0        0     2179 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/common/immutable_map_model.py
--rw-r--r--   0        0        0     2860 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/common/position.py
--rw-r--r--   0        0        0     4913 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/common/rgba.py
--rw-r--r--   0        0        0       37 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/console/__init__.py
--rw-r--r--   0        0        0     3410 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/console/commands.py
--rw-r--r--   0        0        0     2950 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/console/raster_2d_style.py
--rw-r--r--   0        0        0       50 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/gerberx3/__init__.py
--rw-r--r--   0        0        0     1727 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/gerberx3/api/__init__.py
--rw-r--r--   0        0        0     1130 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/gerberx3/api/_errors.py
--rw-r--r--   0        0        0    12011 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/gerberx3/api/_layers.py
--rw-r--r--   0        0        0      248 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/gerberx3/language_server/__init__.py
--rw-r--r--   0        0        0     1248 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/gerberx3/language_server/__main__.py
--rw-r--r--   0        0        0      489 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/gerberx3/language_server/_internals/__init__.py
--rw-r--r--   0        0        0     4711 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/gerberx3/language_server/_internals/document.py
--rw-r--r--   0        0        0      167 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/gerberx3/language_server/_internals/error.py
--rw-r--r--   0        0        0      273 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/gerberx3/language_server/_internals/errors.py
--rw-r--r--   0        0        0     3891 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/gerberx3/language_server/_internals/server.py
--rw-r--r--   0        0        0       29 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/gerberx3/linter/__init__.py
--rw-r--r--   0        0        0     6540 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/gerberx3/linter/diagnostic.py
--rw-r--r--   0        0        0       40 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/gerberx3/math/__init__.py
--rw-r--r--   0        0        0     5229 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/gerberx3/math/bounding_box.py
--rw-r--r--   0        0        0     4845 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/gerberx3/math/offset.py
--rw-r--r--   0        0        0      711 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/gerberx3/math/rotate_point.py
--rw-r--r--   0        0        0     7606 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/gerberx3/math/vector_2d.py
--rw-r--r--   0        0        0       29 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/gerberx3/optimizer/__init__.py
--rw-r--r--   0        0        0       38 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/gerberx3/optimizer/optimizer_pass/__init__.py
--rw-r--r--   0        0        0       23 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/gerberx3/parser/__init__.py
--rw-r--r--   0        0        0     2282 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/gerberx3/parser/errors.py
--rw-r--r--   0        0        0     5942 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/gerberx3/parser/parser.py
--rw-r--r--   0        0        0     6100 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/gerberx3/parser/state.py
--rw-r--r--   0        0        0       36 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/gerberx3/parser2/__init__.py
--rw-r--r--   0        0        0       82 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/gerberx3/parser2/apertures2/__init__.py
--rw-r--r--   0        0        0     1204 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/gerberx3/parser2/apertures2/aperture2.py
--rw-r--r--   0        0        0     1040 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/gerberx3/parser2/apertures2/block2.py
--rw-r--r--   0        0        0     1562 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/gerberx3/parser2/apertures2/circle2.py
--rw-r--r--   0        0        0      974 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/gerberx3/parser2/apertures2/macro2.py
--rw-r--r--   0        0        0     1009 2024-01-27 03:27:07.181241 pygerber-2.2.1/src/pygerber/gerberx3/parser2/apertures2/obround2.py
--rw-r--r--   0        0        0     1204 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/parser2/apertures2/polygon2.py
--rw-r--r--   0        0        0     1155 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/parser2/apertures2/rectangle2.py
--rw-r--r--   0        0        0     8944 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/parser2/attributes2.py
--rw-r--r--   0        0        0     3423 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/parser2/command_buffer2.py
--rw-r--r--   0        0        0       88 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/parser2/commands2/__init__.py
--rw-r--r--   0        0        0      683 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/parser2/commands2/aperture_draw_command2.py
--rw-r--r--   0        0        0     2829 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/parser2/commands2/arc2.py
--rw-r--r--   0        0        0     2035 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/parser2/commands2/buffer_command2.py
--rw-r--r--   0        0        0     1606 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/parser2/commands2/command2.py
--rw-r--r--   0        0        0     1481 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/parser2/commands2/flash2.py
--rw-r--r--   0        0        0     1691 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/parser2/commands2/line2.py
--rw-r--r--   0        0        0     1472 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/parser2/commands2/region2.py
--rw-r--r--   0        0        0    23920 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/parser2/context2.py
--rw-r--r--   0        0        0     4052 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/parser2/errors2.py
--rw-r--r--   0        0        0       66 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/parser2/macro2/__init__.py
--rw-r--r--   0        0        0      729 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/parser2/macro2/assignment2.py
--rw-r--r--   0        0        0      238 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/parser2/macro2/element2.py
--rw-r--r--   0        0        0      242 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/parser2/macro2/enums.py
--rw-r--r--   0        0        0       61 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/parser2/macro2/expressions2/__init__.py
--rw-r--r--   0        0        0     1785 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/parser2/macro2/expressions2/binary2.py
--rw-r--r--   0        0        0      674 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/parser2/macro2/expressions2/constant2.py
--rw-r--r--   0        0        0     1207 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/parser2/macro2/expressions2/expression2.py
--rw-r--r--   0        0        0      957 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/parser2/macro2/expressions2/unary2.py
--rw-r--r--   0        0        0      663 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/parser2/macro2/expressions2/variable_name.py
--rw-r--r--   0        0        0      757 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/parser2/macro2/macro2.py
--rw-r--r--   0        0        0      392 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/parser2/macro2/point2.py
--rw-r--r--   0        0        0       56 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/parser2/macro2/primitives2/__init__.py
--rw-r--r--   0        0        0      749 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/parser2/macro2/primitives2/code_1_circle2.py
--rw-r--r--   0        0        0      811 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/parser2/macro2/primitives2/code_20_vector_line2.py
--rw-r--r--   0        0        0      791 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/parser2/macro2/primitives2/code_21_center_line2.py
--rw-r--r--   0        0        0      588 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/parser2/macro2/primitives2/code_22_lower_left_line2.py
--rw-r--r--   0        0        0      555 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/parser2/macro2/primitives2/code_2_vector_line2.py
--rw-r--r--   0        0        0      849 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/parser2/macro2/primitives2/code_4_outline2.py
--rw-r--r--   0        0        0      875 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/parser2/macro2/primitives2/code_5_polygon2.py
--rw-r--r--   0        0        0      532 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/parser2/macro2/primitives2/code_6_moire2.py
--rw-r--r--   0        0        0      786 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/parser2/macro2/primitives2/code_7_thermal2.py
--rw-r--r--   0        0        0      207 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/parser2/macro2/primitives2/primitive2.py
--rw-r--r--   0        0        0      891 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/parser2/macro2/statement2.py
--rw-r--r--   0        0        0     1294 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/parser2/macro2/statement_buffer2.py
--rw-r--r--   0        0        0     5052 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/parser2/parser2.py
--rw-r--r--   0        0        0    83448 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/parser2/parser2hooks.py
--rw-r--r--   0        0        0    29006 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/parser2/parser2hooks_base.py
--rw-r--r--   0        0        0    28821 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/parser2/state2.py
--rw-r--r--   0        0        0      135 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/renderer2/__init__.py
--rw-r--r--   0        0        0     4583 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/renderer2/abstract.py
--rw-r--r--   0        0        0      497 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/renderer2/errors2.py
--rw-r--r--   0        0        0    26670 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/renderer2/svg.py
--rw-r--r--   0        0        0    14537 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/revisions.py
--rw-r--r--   0        0        0     4973 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/state_enums.py
--rw-r--r--   0        0        0       27 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/__init__.py
--rw-r--r--   0        0        0      936 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/aperture_id.py
--rw-r--r--   0        0        0     1075 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/decorators.py
--rw-r--r--   0        0        0      162 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/errors.py
--rw-r--r--   0        0        0     4459 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/grammar.ebnf
--rw-r--r--   0        0        0    38338 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/grammar.py
--rw-r--r--   0        0        0       22 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/helpers/__init__.py
--rw-r--r--   0        0        0      509 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/helpers/gerber_code_enum.py
--rw-r--r--   0        0        0     2355 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokenizer.py
--rw-r--r--   0        0        0       32 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/__init__.py
--rw-r--r--   0        0        0     6972 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/ab_block_aperture.py
--rw-r--r--   0        0        0    31743 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/ad_define_aperture.py
--rw-r--r--   0        0        0     4355 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/as_axis_select.py
--rw-r--r--   0        0        0     3984 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/attribute_token.py
--rw-r--r--   0        0        0       43 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/bases/__init__.py
--rw-r--r--   0        0        0     2369 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/bases/command.py
--rw-r--r--   0        0        0     2388 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/bases/extended_command.py
--rw-r--r--   0        0        0      907 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/bases/gerber_code.py
--rw-r--r--   0        0        0     4049 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/bases/group.py
--rw-r--r--   0        0        0     4775 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/bases/token.py
--rw-r--r--   0        0        0      633 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/bases/token_accessor.py
--rw-r--r--   0        0        0     2823 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/coordinate.py
--rw-r--r--   0        0        0    10302 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/d01_draw.py
--rw-r--r--   0        0        0     4122 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/d02_move.py
--rw-r--r--   0        0        0     4219 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/d03_flash.py
--rw-r--r--   0        0        0     3199 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/dnn_select_aperture.py
--rw-r--r--   0        0        0     1486 2024-01-27 03:27:07.185242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/end_of_expression.py
--rw-r--r--   0        0        0     7836 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/fs_coordinate_format.py
--rw-r--r--   0        0        0     1933 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/g01_set_linear.py
--rw-r--r--   0        0        0     2039 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/g02_set_clockwise_circular.py
--rw-r--r--   0        0        0     2154 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/g03_set_counterclockwise_circular.py
--rw-r--r--   0        0        0     2170 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/g04_comment.py
--rw-r--r--   0        0        0     1914 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/g36_begin_region.py
--rw-r--r--   0        0        0     2158 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/g37_end_region.py
--rw-r--r--   0        0        0     1939 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/g54_select_aperture.py
--rw-r--r--   0        0        0     2554 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/g70_set_unit_inch.py
--rw-r--r--   0        0        0     2343 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/g71_set_unit_mm.py
--rw-r--r--   0        0        0     2272 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/g74_single_quadrant.py
--rw-r--r--   0        0        0     2705 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/g75_multi_quadrant.py
--rw-r--r--   0        0        0     2325 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/g90_set_coordinate_absolute.py
--rw-r--r--   0        0        0     2383 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/g91_set_coordinate_incremental.py
--rw-r--r--   0        0        0       20 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/groups/__init__.py
--rw-r--r--   0        0        0      206 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/groups/ast.py
--rw-r--r--   0        0        0     2057 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/groups/statement.py
--rw-r--r--   0        0        0     3263 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/in_image_name.py
--rw-r--r--   0        0        0     2052 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/invalid_token.py
--rw-r--r--   0        0        0     2904 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/ip_image_polarity.py
--rw-r--r--   0        0        0     2491 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/lm_load_mirroring.py
--rw-r--r--   0        0        0     3384 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/ln_load_name.py
--rw-r--r--   0        0        0     2471 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/lp_load_polarity.py
--rw-r--r--   0        0        0     3189 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/lr_load_rotation.py
--rw-r--r--   0        0        0     3184 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/ls_load_scaling.py
--rw-r--r--   0        0        0     1615 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/m00_program_stop.py
--rw-r--r--   0        0        0     1621 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/m01_optional_stop.py
--rw-r--r--   0        0        0     1607 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/m02_end_of_file.py
--rw-r--r--   0        0        0     1164 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/macro/__init__.py
--rw-r--r--   0        0        0     7925 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/macro/am_macro.py
--rw-r--r--   0        0        0       62 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/__init__.py
--rw-r--r--   0        0        0     5585 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/binary.py
--rw-r--r--   0        0        0      274 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/errors.py
--rw-r--r--   0        0        0     1776 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/macro_expression.py
--rw-r--r--   0        0        0     2135 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/numeric_constant.py
--rw-r--r--   0        0        0     3647 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/unary.py
--rw-r--r--   0        0        0     2431 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/variable_name.py
--rw-r--r--   0        0        0     3660 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/macro/macro_begin.py
--rw-r--r--   0        0        0      360 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/macro/macro_context.py
--rw-r--r--   0        0        0     1935 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/macro/point.py
--rw-r--r--   0        0        0       60 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/__init__.py
--rw-r--r--   0        0        0     4874 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_1_circle.py
--rw-r--r--   0        0        0     4264 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_20_vector_line.py
--rw-r--r--   0        0        0     4006 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_21_center_line.py
--rw-r--r--   0        0        0      944 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_22_lower_left_line.py
--rw-r--r--   0        0        0      898 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_2_vector_line.py
--rw-r--r--   0        0        0     5065 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_4_outline.py
--rw-r--r--   0        0        0     4182 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_5_polygon.py
--rw-r--r--   0        0        0      866 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_6_moire.py
--rw-r--r--   0        0        0     3980 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_7_thermal.py
--rw-r--r--   0        0        0     2204 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/comment.py
--rw-r--r--   0        0        0      370 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/primitive.py
--rw-r--r--   0        0        0      953 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/statement.py
--rw-r--r--   0        0        0     4388 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/variable_assignment.py
--rw-r--r--   0        0        0     2711 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/mo_unit_mode.py
--rw-r--r--   0        0        0     3801 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/of_image_offset.py
--rw-r--r--   0        0        0     3090 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/sr_step_repeat.py
--rw-r--r--   0        0        0     1844 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/ta_aperture_attribute.py
--rw-r--r--   0        0        0     2103 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/td_delete_attribute.py
--rw-r--r--   0        0        0     1429 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/tf_file_attribute.py
--rw-r--r--   0        0        0     1675 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/to_object_attribute.py
--rw-r--r--   0        0        0      899 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/sequence_tools.py
--rw-r--r--   0        0        0      491 2024-01-27 03:27:07.189242 pygerber-2.2.1/src/pygerber/warnings.py
--rw-r--r--   0        0        0    15765 1970-01-01 00:00:00.000000 pygerber-2.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-11 23:49:13.911182 pygerber-2.3.0/LICENSE.md
+-rw-r--r--   0        0        0    12132 2024-04-11 23:49:13.911182 pygerber-2.3.0/README.md
+-rw-r--r--   0        0        0    12976 2024-04-11 23:49:14.043183 pygerber-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0      103 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/__init__.py
+-rw-r--r--   0        0        0      149 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/__main__.py
+-rw-r--r--   0        0        0      858 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/__init__.py
+-rw-r--r--   0        0        0       61 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/abstract/__init__.py
+-rw-r--r--   0        0        0     4205 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/abstract/aperture_handle.py
+-rw-r--r--   0        0        0     6118 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/abstract/backend_cls.py
+-rw-r--r--   0        0        0       50 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/abstract/draw_commands/__init__.py
+-rw-r--r--   0        0        0     3958 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/abstract/draw_commands/draw_arc.py
+-rw-r--r--   0        0        0     1165 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/abstract/draw_commands/draw_bounding_box.py
+-rw-r--r--   0        0        0     1214 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/abstract/draw_commands/draw_circle.py
+-rw-r--r--   0        0        0     1007 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/abstract/draw_commands/draw_command.py
+-rw-r--r--   0        0        0     1226 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/abstract/draw_commands/draw_paste.py
+-rw-r--r--   0        0        0     1527 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/abstract/draw_commands/draw_polygon.py
+-rw-r--r--   0        0        0     1323 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/abstract/draw_commands/draw_rectangle.py
+-rw-r--r--   0        0        0     1395 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/abstract/draw_commands/draw_region.py
+-rw-r--r--   0        0        0     1707 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/abstract/draw_commands/draw_vector_line.py
+-rw-r--r--   0        0        0      793 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/abstract/draw_commands_handle.py
+-rw-r--r--   0        0        0     1101 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/abstract/drawing_target.py
+-rw-r--r--   0        0        0      280 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/abstract/errors.py
+-rw-r--r--   0        0        0      663 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/abstract/result_handle.py
+-rw-r--r--   0        0        0       65 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/rasterized_2d/__init__.py
+-rw-r--r--   0        0        0     2435 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/rasterized_2d/aperture_handle.py
+-rw-r--r--   0        0        0     8530 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/rasterized_2d/backend_cls.py
+-rw-r--r--   0        0        0     8452 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/rasterized_2d/color_scheme.py
+-rw-r--r--   0        0        0       81 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/rasterized_2d/draw_commands/__init__.py
+-rw-r--r--   0        0        0     1371 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/rasterized_2d/draw_commands/draw_arc.py
+-rw-r--r--   0        0        0     1583 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/rasterized_2d/draw_commands/draw_bounding_box.py
+-rw-r--r--   0        0        0     1702 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/rasterized_2d/draw_commands/draw_circle.py
+-rw-r--r--   0        0        0     2072 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/rasterized_2d/draw_commands/draw_paste.py
+-rw-r--r--   0        0        0     2139 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/rasterized_2d/draw_commands/draw_polygon.py
+-rw-r--r--   0        0        0     1634 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/rasterized_2d/draw_commands/draw_rectangle.py
+-rw-r--r--   0        0        0     1616 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/rasterized_2d/draw_commands/draw_region.py
+-rw-r--r--   0        0        0     1389 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/rasterized_2d/draw_commands/draw_vector_line.py
+-rw-r--r--   0        0        0      317 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/rasterized_2d/draw_commands_handle.py
+-rw-r--r--   0        0        0     4122 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/rasterized_2d/drawing_target.py
+-rw-r--r--   0        0        0      520 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/rasterized_2d/errors.py
+-rw-r--r--   0        0        0      801 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/rasterized_2d/image_tools.py
+-rw-r--r--   0        0        0     1589 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/rasterized_2d/result_handle.py
+-rw-r--r--   0        0        0       53 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/common/__init__.py
+-rw-r--r--   0        0        0      202 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/common/error.py
+-rw-r--r--   0        0        0      369 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/common/frozen_general_model.py
+-rw-r--r--   0        0        0      364 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/common/general_model.py
+-rw-r--r--   0        0        0     2179 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/common/immutable_map_model.py
+-rw-r--r--   0        0        0     2860 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/common/position.py
+-rw-r--r--   0        0        0     4913 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/common/rgba.py
+-rw-r--r--   0        0        0       37 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/console/__init__.py
+-rw-r--r--   0        0        0     3410 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/console/commands.py
+-rw-r--r--   0        0        0     2950 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/console/raster_2d_style.py
+-rw-r--r--   0        0        0      925 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/examples/__init__.py
+-rw-r--r--   0        0        0     1176 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/examples/shape_flashes.grb
+-rw-r--r--   0        0        0    49675 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/examples/simple_2layer-F_Cu.gbr
+-rw-r--r--   0        0        0     3742 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/examples/simple_2layer-F_Mask.gbr
+-rw-r--r--   0        0        0     2486 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/examples/simple_2layer-F_Paste.gbr
+-rw-r--r--   0        0        0     9518 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/examples/simple_2layer-F_Silkscreen.gbr
+-rw-r--r--   0        0        0    10101 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/examples/ucamco_ex_2_shapes.grb
+-rw-r--r--   0        0        0       50 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/__init__.py
+-rw-r--r--   0        0        0     1727 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/api/__init__.py
+-rw-r--r--   0        0        0     1130 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/api/_errors.py
+-rw-r--r--   0        0        0    12011 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/api/_layers.py
+-rw-r--r--   0        0        0    13437 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/api/_v2.py
+-rw-r--r--   0        0        0      981 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/api/v2.py
+-rw-r--r--   0        0        0      248 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/language_server/__init__.py
+-rw-r--r--   0        0        0     1248 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/language_server/__main__.py
+-rw-r--r--   0        0        0      489 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/language_server/_internals/__init__.py
+-rw-r--r--   0        0        0     4711 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/language_server/_internals/document.py
+-rw-r--r--   0        0        0      167 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/language_server/_internals/error.py
+-rw-r--r--   0        0        0      273 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/language_server/_internals/errors.py
+-rw-r--r--   0        0        0     3891 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/language_server/_internals/server.py
+-rw-r--r--   0        0        0       29 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/linter/__init__.py
+-rw-r--r--   0        0        0     6540 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/linter/diagnostic.py
+-rw-r--r--   0        0        0       40 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/math/__init__.py
+-rw-r--r--   0        0        0     5229 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/math/bounding_box.py
+-rw-r--r--   0        0        0     4845 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/math/offset.py
+-rw-r--r--   0        0        0      711 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/math/rotate_point.py
+-rw-r--r--   0        0        0     7968 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/math/vector_2d.py
+-rw-r--r--   0        0        0       29 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/optimizer/__init__.py
+-rw-r--r--   0        0        0       38 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/optimizer/optimizer_pass/__init__.py
+-rw-r--r--   0        0        0       23 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser/__init__.py
+-rw-r--r--   0        0        0     2282 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser/errors.py
+-rw-r--r--   0        0        0     5942 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser/parser.py
+-rw-r--r--   0        0        0     6100 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser/state.py
+-rw-r--r--   0        0        0       36 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/__init__.py
+-rw-r--r--   0        0        0       82 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/apertures2/__init__.py
+-rw-r--r--   0        0        0     1844 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/apertures2/aperture2.py
+-rw-r--r--   0        0        0     2122 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/apertures2/block2.py
+-rw-r--r--   0        0        0     2071 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/apertures2/circle2.py
+-rw-r--r--   0        0        0     2056 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/apertures2/macro2.py
+-rw-r--r--   0        0        0      789 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/apertures2/obround2.py
+-rw-r--r--   0        0        0     1635 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/apertures2/polygon2.py
+-rw-r--r--   0        0        0     1650 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/apertures2/rectangle2.py
+-rw-r--r--   0        0        0     8944 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/attributes2.py
+-rw-r--r--   0        0        0     3922 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/command_buffer2.py
+-rw-r--r--   0        0        0       88 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/commands2/__init__.py
+-rw-r--r--   0        0        0      975 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/commands2/aperture_draw_command2.py
+-rw-r--r--   0        0        0     4375 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/commands2/arc2.py
+-rw-r--r--   0        0        0     2952 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/commands2/buffer_command2.py
+-rw-r--r--   0        0        0     2258 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/commands2/command2.py
+-rw-r--r--   0        0        0     2477 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/commands2/flash2.py
+-rw-r--r--   0        0        0     2688 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/commands2/line2.py
+-rw-r--r--   0        0        0     1733 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/commands2/region2.py
+-rw-r--r--   0        0        0    24876 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/context2.py
+-rw-r--r--   0        0        0     4052 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/errors2.py
+-rw-r--r--   0        0        0       66 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/__init__.py
+-rw-r--r--   0        0        0      729 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/assignment2.py
+-rw-r--r--   0        0        0      238 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/element2.py
+-rw-r--r--   0        0        0      242 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/enums.py
+-rw-r--r--   0        0        0       61 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/expressions2/__init__.py
+-rw-r--r--   0        0        0     1785 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/expressions2/binary2.py
+-rw-r--r--   0        0        0      674 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/expressions2/constant2.py
+-rw-r--r--   0        0        0     1207 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/expressions2/expression2.py
+-rw-r--r--   0        0        0      957 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/expressions2/unary2.py
+-rw-r--r--   0        0        0      663 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/expressions2/variable_name.py
+-rw-r--r--   0        0        0      757 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/macro2.py
+-rw-r--r--   0        0        0      392 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/point2.py
+-rw-r--r--   0        0        0       56 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/primitives2/__init__.py
+-rw-r--r--   0        0        0      749 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/primitives2/code_1_circle2.py
+-rw-r--r--   0        0        0      811 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/primitives2/code_20_vector_line2.py
+-rw-r--r--   0        0        0      791 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/primitives2/code_21_center_line2.py
+-rw-r--r--   0        0        0      588 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/primitives2/code_22_lower_left_line2.py
+-rw-r--r--   0        0        0      555 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/primitives2/code_2_vector_line2.py
+-rw-r--r--   0        0        0      849 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/primitives2/code_4_outline2.py
+-rw-r--r--   0        0        0      875 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/primitives2/code_5_polygon2.py
+-rw-r--r--   0        0        0      532 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/primitives2/code_6_moire2.py
+-rw-r--r--   0        0        0      786 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/primitives2/code_7_thermal2.py
+-rw-r--r--   0        0        0      207 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/primitives2/primitive2.py
+-rw-r--r--   0        0        0      891 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/statement2.py
+-rw-r--r--   0        0        0     1294 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/statement_buffer2.py
+-rw-r--r--   0        0        0     5052 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/parser2.py
+-rw-r--r--   0        0        0    84548 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/parser2hooks.py
+-rw-r--r--   0        0        0    29008 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/parser2hooks_base.py
+-rw-r--r--   0        0        0    29444 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/state2.py
+-rw-r--r--   0        0        0      135 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/renderer2/__init__.py
+-rw-r--r--   0        0        0     4767 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/renderer2/abstract.py
+-rw-r--r--   0        0        0      497 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/renderer2/errors2.py
+-rw-r--r--   0        0        0    29641 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/renderer2/raster.py
+-rw-r--r--   0        0        0    29563 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/renderer2/svg.py
+-rw-r--r--   0        0        0    14537 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/revisions.py
+-rw-r--r--   0        0        0     5321 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/state_enums.py
+-rw-r--r--   0        0        0       27 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/__init__.py
+-rw-r--r--   0        0        0      936 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/aperture_id.py
+-rw-r--r--   0        0        0     1075 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/decorators.py
+-rw-r--r--   0        0        0      162 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/errors.py
+-rw-r--r--   0        0        0     4459 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/grammar.ebnf
+-rw-r--r--   0        0        0    38460 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/grammar.py
+-rw-r--r--   0        0        0       22 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/helpers/__init__.py
+-rw-r--r--   0        0        0      509 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/helpers/gerber_code_enum.py
+-rw-r--r--   0        0        0     2355 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokenizer.py
+-rw-r--r--   0        0        0       32 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/__init__.py
+-rw-r--r--   0        0        0     6972 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/ab_block_aperture.py
+-rw-r--r--   0        0        0    31743 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/ad_define_aperture.py
+-rw-r--r--   0        0        0     4355 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/as_axis_select.py
+-rw-r--r--   0        0        0     3984 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/attribute_token.py
+-rw-r--r--   0        0        0       43 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/bases/__init__.py
+-rw-r--r--   0        0        0     2369 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/bases/command.py
+-rw-r--r--   0        0        0     2388 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/bases/extended_command.py
+-rw-r--r--   0        0        0      907 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/bases/gerber_code.py
+-rw-r--r--   0        0        0     4049 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/bases/group.py
+-rw-r--r--   0        0        0     4775 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/bases/token.py
+-rw-r--r--   0        0        0      633 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/bases/token_accessor.py
+-rw-r--r--   0        0        0     2823 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/coordinate.py
+-rw-r--r--   0        0        0    10302 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/d01_draw.py
+-rw-r--r--   0        0        0     4122 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/d02_move.py
+-rw-r--r--   0        0        0     4219 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/d03_flash.py
+-rw-r--r--   0        0        0     3199 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/dnn_select_aperture.py
+-rw-r--r--   0        0        0     1486 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/end_of_expression.py
+-rw-r--r--   0        0        0     7836 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/fs_coordinate_format.py
+-rw-r--r--   0        0        0     1933 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/g01_set_linear.py
+-rw-r--r--   0        0        0     2039 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/g02_set_clockwise_circular.py
+-rw-r--r--   0        0        0     2154 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/g03_set_counterclockwise_circular.py
+-rw-r--r--   0        0        0     2170 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/g04_comment.py
+-rw-r--r--   0        0        0     1914 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/g36_begin_region.py
+-rw-r--r--   0        0        0     2158 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/g37_end_region.py
+-rw-r--r--   0        0        0     1939 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/g54_select_aperture.py
+-rw-r--r--   0        0        0     2554 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/g70_set_unit_inch.py
+-rw-r--r--   0        0        0     2343 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/g71_set_unit_mm.py
+-rw-r--r--   0        0        0     2272 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/g74_single_quadrant.py
+-rw-r--r--   0        0        0     2705 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/g75_multi_quadrant.py
+-rw-r--r--   0        0        0     2325 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/g90_set_coordinate_absolute.py
+-rw-r--r--   0        0        0     2383 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/g91_set_coordinate_incremental.py
+-rw-r--r--   0        0        0       20 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/groups/__init__.py
+-rw-r--r--   0        0        0      206 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/groups/ast.py
+-rw-r--r--   0        0        0     2057 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/groups/statement.py
+-rw-r--r--   0        0        0     3263 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/in_image_name.py
+-rw-r--r--   0        0        0     2052 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/invalid_token.py
+-rw-r--r--   0        0        0     2904 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/ip_image_polarity.py
+-rw-r--r--   0        0        0     2491 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/lm_load_mirroring.py
+-rw-r--r--   0        0        0     3384 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/ln_load_name.py
+-rw-r--r--   0        0        0     2471 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/lp_load_polarity.py
+-rw-r--r--   0        0        0     3189 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/lr_load_rotation.py
+-rw-r--r--   0        0        0     3184 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/ls_load_scaling.py
+-rw-r--r--   0        0        0     1615 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/m00_program_stop.py
+-rw-r--r--   0        0        0     1621 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/m01_optional_stop.py
+-rw-r--r--   0        0        0     1607 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/m02_end_of_file.py
+-rw-r--r--   0        0        0     1164 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/__init__.py
+-rw-r--r--   0        0        0     7925 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/am_macro.py
+-rw-r--r--   0        0        0       62 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/__init__.py
+-rw-r--r--   0        0        0     5585 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/binary.py
+-rw-r--r--   0        0        0      274 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/errors.py
+-rw-r--r--   0        0        0     1776 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/macro_expression.py
+-rw-r--r--   0        0        0     2135 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/numeric_constant.py
+-rw-r--r--   0        0        0     3647 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/unary.py
+-rw-r--r--   0        0        0     2431 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/variable_name.py
+-rw-r--r--   0        0        0     3660 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/macro_begin.py
+-rw-r--r--   0        0        0      360 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/macro_context.py
+-rw-r--r--   0        0        0     1935 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/point.py
+-rw-r--r--   0        0        0       60 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/__init__.py
+-rw-r--r--   0        0        0     4874 2024-04-11 23:49:14.055183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_1_circle.py
+-rw-r--r--   0        0        0     4264 2024-04-11 23:49:14.055183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_20_vector_line.py
+-rw-r--r--   0        0        0     4006 2024-04-11 23:49:14.055183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_21_center_line.py
+-rw-r--r--   0        0        0      944 2024-04-11 23:49:14.055183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_22_lower_left_line.py
+-rw-r--r--   0        0        0      898 2024-04-11 23:49:14.055183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_2_vector_line.py
+-rw-r--r--   0        0        0     5065 2024-04-11 23:49:14.055183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_4_outline.py
+-rw-r--r--   0        0        0     4182 2024-04-11 23:49:14.055183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_5_polygon.py
+-rw-r--r--   0        0        0      866 2024-04-11 23:49:14.055183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_6_moire.py
+-rw-r--r--   0        0        0     3980 2024-04-11 23:49:14.055183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_7_thermal.py
+-rw-r--r--   0        0        0     2204 2024-04-11 23:49:14.055183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/comment.py
+-rw-r--r--   0        0        0      370 2024-04-11 23:49:14.055183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/primitive.py
+-rw-r--r--   0        0        0      953 2024-04-11 23:49:14.055183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/statement.py
+-rw-r--r--   0        0        0     4388 2024-04-11 23:49:14.055183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/variable_assignment.py
+-rw-r--r--   0        0        0     2711 2024-04-11 23:49:14.055183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/mo_unit_mode.py
+-rw-r--r--   0        0        0     3801 2024-04-11 23:49:14.055183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/of_image_offset.py
+-rw-r--r--   0        0        0     3090 2024-04-11 23:49:14.055183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/sr_step_repeat.py
+-rw-r--r--   0        0        0     1892 2024-04-11 23:49:14.055183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/ta_aperture_attribute.py
+-rw-r--r--   0        0        0     2122 2024-04-11 23:49:14.055183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/td_delete_attribute.py
+-rw-r--r--   0        0        0     1477 2024-04-11 23:49:14.055183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/tf_file_attribute.py
+-rw-r--r--   0        0        0     1724 2024-04-11 23:49:14.055183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/to_object_attribute.py
+-rw-r--r--   0        0        0      899 2024-04-11 23:49:14.055183 pygerber-2.3.0/src/pygerber/sequence_tools.py
+-rw-r--r--   0        0        0      491 2024-04-11 23:49:14.055183 pygerber-2.3.0/src/pygerber/warnings.py
+-rw-r--r--   0        0        0    14868 1970-01-01 00:00:00.000000 pygerber-2.3.0/PKG-INFO
```

### Comparing `pygerber-2.2.1/LICENSE.md` & `pygerber-2.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/README.md` & `pygerber-2.3.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -109,142 +109,135 @@
 pygerber raster-2d gerber-source.grb
 ```
 
 Image will be saved to `output.png` in current working directory.
 
 ![example_pcb_image](https://github.com/Argmaster/pygerber/assets/56170852/9bca28bf-8aa6-4215-aac1-62c386490485)
 
-## API usage
+## Programmatic usage
 
-PyGerber offers a high-level API that simplifies the process of rendering Gerber files.
-Whether you're looking to save the rendered output to a file or directly into a buffer,
-PyGerber has got you covered.
-
-- **The `Layer` Class**: At its core, the `Layer` class stands for a single Gerber
-  source file, complete with its associated PyGerber configuration.
-
-  **Important** `Layer` class represents **any** Gerber file, **not** layer of PCB. For
-  example, silkscreen Gerber file will require one instance of `Layer`, paste mask will
-  require another one, copper top yet another, etc.
-
-- **Configuration Flexibility**: The configuration possibilities you get with a `Layer`
-  are driven by the backend you choose to render your source file.
-
-- **Selecting a Backend**: PyGerber provides specialized subclasses of the `Layer` class
-  each tied to one rendering backend. For instance, if you're aiming for 2D rasterized
-  images, `Rasterized2DLayer` is your go-to choice.
-
-- **Output Types**: Keep in mind, the type of your output file is closely tied to the
-  backend you select.For 2D rasterized rendering
-  [all formats supported by Pillow](https://pillow.readthedocs.io/en/stable/handbook/image-file-formats.html)
-  are accepted.
-
-### Rasterized render from file
-
-```py linenums="1" title="render_file.py"
-from pygerber.gerberx3.api import (
-      ColorScheme,
-      Rasterized2DLayer,
-      Rasterized2DLayerParams,
-)
+### JPG
+
+PyGerber can be used programmatically to render Gerber files. Below is an minimalistic
+example of how to render one of the example files included with PyGerber release to JPEG
+image:
 
-# Path to Gerber source file.
-source_path = "main_cu.grb"
+```python
+from pygerber.examples import ExamplesEnum, get_example_path
+from pygerber.gerberx3.api.v2 import GerberFile
 
-Rasterized2DLayer(
-      options=Rasterized2DLayerParams(
-            source_path=source_path,
-            colors=ColorScheme.COPPER_ALPHA,
-      ),
-).render().save("output.png")
+GerberFile.from_file(
+    get_example_path(ExamplesEnum.UCAMCO_ex_2_Shapes),
+).parse().render_raster("output.jpg")
 ```
 
-Example code above creates `Rasterized2DLayer` object, renders it with rasterized 2D
-backend and saves it as `PNG` image. Use of `Rasterized2DLayer` and
-`Rasterized2DLayerOptions` classes implicitly use 2D rasterized backend. To use
-different rendering backend with high level API, user must pick different `Layer` and
-`LayerOptions` subclasses. For other backends see
-[Target set of tools](#target-set-of-tools) section, note that only checked ones are
-available.
-
-`source_path` option accepts `str` or `Path` pointing to local Gerber file. No special
-file extension is required, content is blindly loaded from specified file, so it's user
-responsibility to provide correct path. There are also `source_code` and `source_buffer`
-parameters which allow for use of raw `str` or `bytes` objects (first one) and
-`StringIO` and `BytesIO` or file descriptors (second one). `source_code`,
-`source_buffer` and `source_path` are mutually exclusive.
-
-`ColorScheme` is a class which describes what colors should be used for rendering
-different parts of image. Additionally it has a few static members which contain
-predefined colors schemes for frequently used layer types. It is not required to use
-predefined schemes, creating and passing custom `ColorScheme` object should work
-perfectly fine.
-
-Pattern of using `<Class>` and `<Class>Options`, like above, is used in many places in
-PyGerber. When initializing object like `Rasterized2DLayer` it is only valid to pass
-`Rasterized2DLayerOptions` to constructor. Passing `LayerOptions` or `Vectorized2DLayer`
-will cause undefined behavior, most likely yielding no result or raising exception.
-
-### Rasterized render from string
-
-```py linenums="1" title="render_string.py"
-from pygerber.gerberx3.api import (
-      ColorScheme,
-      Rasterized2DLayer,
-      Rasterized2DLayerParams,
-)
+Running code above will create `output.jpg` file in current working directory which
+should look like this:
+
+<p align="center">
+  <img height="400" src="https://github.com/Argmaster/pygerber/assets/56170852/d17ebee8-e851-4c86-b110-8cd8aeca993e">
+</p>
 
-source_code = """
-%FSLAX26Y26*%
-%MOMM*%
-%ADD100R,1.5X1.0X0.5*%
-%ADD200C,1.5X1.0*%
-%ADD300O,1.5X1.0X0.6*%
-%ADD400P,1.5X3X5.0*%
-D100*
-X0Y0D03*
-D200*
-X0Y2000000D03*
-D300*
-X2000000Y0D03*
-D400*
-X2000000Y2000000D03*
-M02*
-"""
-
-Rasterized2DLayer(
-      options=Rasterized2DLayerParams(
-            source_code=source_code,
-            colors=ColorScheme.SILK,
-            dpi=3000,
-      ),
-).render().save("output.png")
+### PNG
 
+It is also possible to render Gerber files to PNG with custom resolution and different
+color schemes:
+
+```python
+from pygerber.examples import ExamplesEnum, get_example_path
+from pygerber.gerberx3.api.v2 import ColorScheme, GerberFile, PixelFormatEnum
+
+GerberFile.from_file(
+    get_example_path(ExamplesEnum.ShapeFlashes),
+).parse().render_raster(
+    "output.png",
+    dpmm=100,
+    color_scheme=ColorScheme.COPPER_ALPHA,
+    pixel_format=PixelFormatEnum.RGBA,
+)
 ```
 
 Code above renders following image:
 
 <p align="center">
-  <img width="414" height="384" src="https://github.com/Argmaster/pygerber/assets/56170852/56b6757b-0f97-4a18-9d43-f21711c71c71">
+  <img height="400" src="https://github.com/Argmaster/pygerber/assets/56170852/0a5a42f3-8792-4b9a-be61-bac12f0e1c03">
+</p>
+
+### SVG
+
+Finally you can also create SVG files with PyGerber:
+
+```python
+from pygerber.examples import ExamplesEnum, load_example
+from pygerber.gerberx3.api.v2 import GerberFile
+
+source_code = load_example(ExamplesEnum.UCAMCO_ex_2_Shapes)
+GerberFile.from_str(source_code).parse().render_svg("output.svg")
+
+```
+
+### Multiple layers
+
+PyGerber can also render multiple layers to single image. Below is an example of how to
+render four layers to single PNG image with use of `Project` class:
+
+```python
+from pygerber.examples import ExamplesEnum, load_example
+from pygerber.gerberx3.api.v2 import FileTypeEnum, GerberFile, Project
+
+Project(
+    [
+        GerberFile.from_str(
+            load_example(ExamplesEnum.simple_2layer_F_Cu),
+            FileTypeEnum.COPPER,
+        ),
+        GerberFile.from_str(
+            load_example(ExamplesEnum.simple_2layer_F_Mask),
+            FileTypeEnum.MASK,
+        ),
+        GerberFile.from_str(
+            load_example(ExamplesEnum.simple_2layer_F_Paste),
+            FileTypeEnum.PASTE,
+        ),
+        GerberFile.from_str(
+            load_example(ExamplesEnum.simple_2layer_F_Silkscreen),
+            FileTypeEnum.SILK,
+        ),
+    ],
+).parse().render_raster("output.png", dpmm=40)
+```
+
+Here is the result:
+
+<p align="center">
+  <img width="400" src="https://github.com/Argmaster/pygerber/assets/56170852/9b3f3823-67b3-49f1-8c76-e2bddaca81fe">
 </p>
 
+### Advanced usage
+
+Additionally to examples presented above which use high level API, PyGerber provides low
+level API which allows to directly access PyGerber internals and change behavior of
+parser, tokenizer and renderers. This can be used for code introspection and potentially
+other purposed. Check out documentation for more information.
+
 ## Documentation
 
 Official documentations is hosted on Github Pages and can be found
 [here](https://argmaster.github.io/pygerber/latest).
 
 ## Gerber features support
 
 Please refer to documentation for
 
 - [Tokenizer](https://argmaster.github.io/pygerber/latest/gerber/feature_support/tokenizer.html),
 - [Parser](https://argmaster.github.io/pygerber/latest/gerber/feature_support/parser.html),
 - [Rasterized2DBackend](https://argmaster.github.io/pygerber/latest/gerber/feature_support/rasterized_2d.html),
 - [Parser2](https://argmaster.github.io/pygerber/latest/gerber/feature_support/parser2.html),
 - [SvgRenderer2](https://argmaster.github.io/pygerber/latest/gerber/feature_support/svgrenderer2.html),
+- [RasterRenderer2](https://argmaster.github.io/pygerber/latest/gerber/feature_support/rasterrenderer2.html),
 
 for detailed list of features which are supported/not supported by each tool.
 
 ## Syntax feature requests
 
 All deprecated features (Mainly those from X2 format) are considered optional and
 priority to implement them will be assigned based on number of requests form community.
```

#### html2text {}

```diff
@@ -40,77 +40,67 @@
 similar to one below **â©**, where `x.y.z` should match version of PyGerber
 installed. ``` $ pygerber --version pygerber, version x.y.z ``` Use `--help` to
 display help messages with lists of subcommands and subcommand options: ```
 pygerber raster-2d --help ``` To render 2D PNG image of some gerber file you
 can simply use: ``` pygerber raster-2d gerber-source.grb ``` Image will be
 saved to `output.png` in current working directory. ![example_pcb_image](https:
 //github.com/Argmaster/pygerber/assets/56170852/9bca28bf-8aa6-4215-aac1-
-62c386490485) ## API usage PyGerber offers a high-level API that simplifies the
-process of rendering Gerber files. Whether you're looking to save the rendered
-output to a file or directly into a buffer, PyGerber has got you covered. -
-**The `Layer` Class**: At its core, the `Layer` class stands for a single
-Gerber source file, complete with its associated PyGerber configuration.
-**Important** `Layer` class represents **any** Gerber file, **not** layer of
-PCB. For example, silkscreen Gerber file will require one instance of `Layer`,
-paste mask will require another one, copper top yet another, etc. -
-**Configuration Flexibility**: The configuration possibilities you get with a
-`Layer` are driven by the backend you choose to render your source file. -
-**Selecting a Backend**: PyGerber provides specialized subclasses of the
-`Layer` class each tied to one rendering backend. For instance, if you're
-aiming for 2D rasterized images, `Rasterized2DLayer` is your go-to choice. -
-**Output Types**: Keep in mind, the type of your output file is closely tied to
-the backend you select.For 2D rasterized rendering [all formats supported by
-Pillow](https://pillow.readthedocs.io/en/stable/handbook/image-file-
-formats.html) are accepted. ### Rasterized render from file ```py linenums="1"
-title="render_file.py" from pygerber.gerberx3.api import ( ColorScheme,
-Rasterized2DLayer, Rasterized2DLayerParams, ) # Path to Gerber source file.
-source_path = "main_cu.grb" Rasterized2DLayer( options=Rasterized2DLayerParams
-( source_path=source_path, colors=ColorScheme.COPPER_ALPHA, ), ).render().save
-("output.png") ``` Example code above creates `Rasterized2DLayer` object,
-renders it with rasterized 2D backend and saves it as `PNG` image. Use of
-`Rasterized2DLayer` and `Rasterized2DLayerOptions` classes implicitly use 2D
-rasterized backend. To use different rendering backend with high level API,
-user must pick different `Layer` and `LayerOptions` subclasses. For other
-backends see [Target set of tools](#target-set-of-tools) section, note that
-only checked ones are available. `source_path` option accepts `str` or `Path`
-pointing to local Gerber file. No special file extension is required, content
-is blindly loaded from specified file, so it's user responsibility to provide
-correct path. There are also `source_code` and `source_buffer` parameters which
-allow for use of raw `str` or `bytes` objects (first one) and `StringIO` and
-`BytesIO` or file descriptors (second one). `source_code`, `source_buffer` and
-`source_path` are mutually exclusive. `ColorScheme` is a class which describes
-what colors should be used for rendering different parts of image. Additionally
-it has a few static members which contain predefined colors schemes for
-frequently used layer types. It is not required to use predefined schemes,
-creating and passing custom `ColorScheme` object should work perfectly fine.
-Pattern of using `` and `Options`, like above, is used in many places in
-PyGerber. When initializing object like `Rasterized2DLayer` it is only valid to
-pass `Rasterized2DLayerOptions` to constructor. Passing `LayerOptions` or
-`Vectorized2DLayer` will cause undefined behavior, most likely yielding no
-result or raising exception. ### Rasterized render from string ```py
-linenums="1" title="render_string.py" from pygerber.gerberx3.api import
-( ColorScheme, Rasterized2DLayer, Rasterized2DLayerParams, ) source_code = """
-%FSLAX26Y26*% %MOMM*% %ADD100R,1.5X1.0X0.5*% %ADD200C,1.5X1.0*%
-%ADD300O,1.5X1.0X0.6*% %ADD400P,1.5X3X5.0*% D100* X0Y0D03* D200* X0Y2000000D03*
-D300* X2000000Y0D03* D400* X2000000Y2000000D03* M02* """ Rasterized2DLayer
-( options=Rasterized2DLayerParams( source_code=source_code,
-colors=ColorScheme.SILK, dpi=3000, ), ).render().save("output.png") ``` Code
-above renders following image:
-[https://github.com/Argmaster/pygerber/assets/56170852/56b6757b-0f97-4a18-9d43-
-                                 f21711c71c71]
-## Documentation Official documentations is hosted on Github Pages and can be
-found [here](https://argmaster.github.io/pygerber/latest). ## Gerber features
-support Please refer to documentation for - [Tokenizer](https://
-argmaster.github.io/pygerber/latest/gerber/feature_support/tokenizer.html), -
-[Parser](https://argmaster.github.io/pygerber/latest/gerber/feature_support/
-parser.html), - [Rasterized2DBackend](https://argmaster.github.io/pygerber/
-latest/gerber/feature_support/rasterized_2d.html), - [Parser2](https://
-argmaster.github.io/pygerber/latest/gerber/feature_support/parser2.html), -
-[SvgRenderer2](https://argmaster.github.io/pygerber/latest/gerber/
-feature_support/svgrenderer2.html), for detailed list of features which are
+62c386490485) ## Programmatic usage ### JPG PyGerber can be used
+programmatically to render Gerber files. Below is an minimalistic example of
+how to render one of the example files included with PyGerber release to JPEG
+image: ```python from pygerber.examples import ExamplesEnum, get_example_path
+from pygerber.gerberx3.api.v2 import GerberFile GerberFile.from_file
+( get_example_path(ExamplesEnum.UCAMCO_ex_2_Shapes), ).parse().render_raster
+("output.jpg") ``` Running code above will create `output.jpg` file in current
+working directory which should look like this:
+[https://github.com/Argmaster/pygerber/assets/56170852/d17ebee8-e851-4c86-b110-
+                                 8cd8aeca993e]
+### PNG It is also possible to render Gerber files to PNG with custom
+resolution and different color schemes: ```python from pygerber.examples import
+ExamplesEnum, get_example_path from pygerber.gerberx3.api.v2 import
+ColorScheme, GerberFile, PixelFormatEnum GerberFile.from_file( get_example_path
+(ExamplesEnum.ShapeFlashes), ).parse().render_raster( "output.png", dpmm=100,
+color_scheme=ColorScheme.COPPER_ALPHA, pixel_format=PixelFormatEnum.RGBA, ) ```
+Code above renders following image:
+[https://github.com/Argmaster/pygerber/assets/56170852/0a5a42f3-8792-4b9a-be61-
+                                 bac12f0e1c03]
+### SVG Finally you can also create SVG files with PyGerber: ```python from
+pygerber.examples import ExamplesEnum, load_example from
+pygerber.gerberx3.api.v2 import GerberFile source_code = load_example
+(ExamplesEnum.UCAMCO_ex_2_Shapes) GerberFile.from_str(source_code).parse
+().render_svg("output.svg") ``` ### Multiple layers PyGerber can also render
+multiple layers to single image. Below is an example of how to render four
+layers to single PNG image with use of `Project` class: ```python from
+pygerber.examples import ExamplesEnum, load_example from
+pygerber.gerberx3.api.v2 import FileTypeEnum, GerberFile, Project Project(
+[ GerberFile.from_str( load_example(ExamplesEnum.simple_2layer_F_Cu),
+FileTypeEnum.COPPER, ), GerberFile.from_str( load_example
+(ExamplesEnum.simple_2layer_F_Mask), FileTypeEnum.MASK, ), GerberFile.from_str
+( load_example(ExamplesEnum.simple_2layer_F_Paste), FileTypeEnum.PASTE, ),
+GerberFile.from_str( load_example(ExamplesEnum.simple_2layer_F_Silkscreen),
+FileTypeEnum.SILK, ), ], ).parse().render_raster("output.png", dpmm=40) ```
+Here is the result:
+[https://github.com/Argmaster/pygerber/assets/56170852/9b3f3823-67b3-49f1-8c76-
+                                 e2bddaca81fe]
+### Advanced usage Additionally to examples presented above which use high
+level API, PyGerber provides low level API which allows to directly access
+PyGerber internals and change behavior of parser, tokenizer and renderers. This
+can be used for code introspection and potentially other purposed. Check out
+documentation for more information. ## Documentation Official documentations is
+hosted on Github Pages and can be found [here](https://argmaster.github.io/
+pygerber/latest). ## Gerber features support Please refer to documentation for
+- [Tokenizer](https://argmaster.github.io/pygerber/latest/gerber/
+feature_support/tokenizer.html), - [Parser](https://argmaster.github.io/
+pygerber/latest/gerber/feature_support/parser.html), - [Rasterized2DBackend]
+(https://argmaster.github.io/pygerber/latest/gerber/feature_support/
+rasterized_2d.html), - [Parser2](https://argmaster.github.io/pygerber/latest/
+gerber/feature_support/parser2.html), - [SvgRenderer2](https://
+argmaster.github.io/pygerber/latest/gerber/feature_support/svgrenderer2.html),
+- [RasterRenderer2](https://argmaster.github.io/pygerber/latest/gerber/
+feature_support/rasterrenderer2.html), for detailed list of features which are
 supported/not supported by each tool. ## Syntax feature requests All deprecated
 features (Mainly those from X2 format) are considered optional and priority to
 implement them will be assigned based on number of requests form community. If
 You needs support for syntax features which are not mentioned in `The Gerber
 Layer Format Specification. Revision 2023.08` (Available on [Ucamco's webpage]
 (https://www.ucamco.com/files/downloads/file_en/456/gerber-layer-format-
 specification-revision-2023-08_en.pdf) and in [this repository](https://
```

### Comparing `pygerber-2.2.1/pyproject.toml` & `pygerber-2.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pygerber"
-version = "2.2.1"
+version = "2.3.0"
 description = "Parsing, formatting and rendering toolkit for Gerber X3 file format"
 authors = ["Krzysztof Wisniewski <argmaster.world@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://www.facebook.com/pygerber"
 repository = "https://github.com/Argmaster/pygerber"
 documentation = "https://argmaster.github.io/pygerber/latest"
@@ -58,18 +58,18 @@
 pyyaml = "^6.0.1"
 pygls = { version = "^1.0.2", optional = true }
 lsprotocol = { version = "^2023.0.0a3", optional = true }
 drawsvg = { version = "^2.3.0", optional = true }
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.6.1"
-poethepoet = ">=0.20,<0.25"
-pytest = "^7.4.0"
-black = "^23.3.0"
-ruff = "^0.1.3"
+poethepoet = ">=0.20,<0.26"
+pytest = ">=7.4,<9.0"
+black = ">=23.3,<25.0"
+ruff = ">=0.1.3,<0.4.0"
 jinja2 = "^3.1.2"
 pyyaml = "^6.0"
 tox = "^4.6.3"
 pre-commit = "^3.3.3"
 autoflake = "^2.2.0"
 isort = "^5.12.0"
 pytest-xdist = { extras = ["psutil"], version = "^3.3.1" }
@@ -80,15 +80,15 @@
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.5.2"
 mkdocs-material = "^9.1.21"
-mkdocstrings = { extras = ["python"], version = ">=0.22,<0.24" }
+mkdocstrings = { extras = ["python"], version = ">=0.22,<0.25" }
 mkdocs-literate-nav = "^0.6.0"
 mkdocs-macros-plugin = "^1.0.2"
 mkdocs-gen-files = "^0.5.0"
 pygments = "^2.15.1"
 pymdown-extensions = "^10.3"
 mike = "^1.1.2"
```

### Comparing `pygerber-2.2.1/src/pygerber/backend/__init__.py` & `pygerber-2.3.0/src/pygerber/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/backend/abstract/aperture_handle.py` & `pygerber-2.3.0/src/pygerber/backend/abstract/aperture_handle.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/backend/abstract/backend_cls.py` & `pygerber-2.3.0/src/pygerber/backend/abstract/backend_cls.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/backend/abstract/draw_commands/draw_arc.py` & `pygerber-2.3.0/src/pygerber/backend/abstract/draw_commands/draw_arc.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/backend/abstract/draw_commands/draw_bounding_box.py` & `pygerber-2.3.0/src/pygerber/backend/abstract/draw_commands/draw_bounding_box.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/backend/abstract/draw_commands/draw_circle.py` & `pygerber-2.3.0/src/pygerber/backend/abstract/draw_commands/draw_circle.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/backend/abstract/draw_commands/draw_command.py` & `pygerber-2.3.0/src/pygerber/backend/abstract/draw_commands/draw_command.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/backend/abstract/draw_commands/draw_paste.py` & `pygerber-2.3.0/src/pygerber/backend/abstract/draw_commands/draw_paste.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/backend/abstract/draw_commands/draw_polygon.py` & `pygerber-2.3.0/src/pygerber/backend/abstract/draw_commands/draw_polygon.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/backend/abstract/draw_commands/draw_rectangle.py` & `pygerber-2.3.0/src/pygerber/backend/abstract/draw_commands/draw_rectangle.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/backend/abstract/draw_commands/draw_region.py` & `pygerber-2.3.0/src/pygerber/backend/abstract/draw_commands/draw_region.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/backend/abstract/draw_commands/draw_vector_line.py` & `pygerber-2.3.0/src/pygerber/backend/abstract/draw_commands/draw_vector_line.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/backend/abstract/draw_commands_handle.py` & `pygerber-2.3.0/src/pygerber/backend/abstract/draw_commands_handle.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/backend/abstract/drawing_target.py` & `pygerber-2.3.0/src/pygerber/backend/abstract/drawing_target.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/backend/abstract/result_handle.py` & `pygerber-2.3.0/src/pygerber/backend/abstract/result_handle.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/backend/rasterized_2d/aperture_handle.py` & `pygerber-2.3.0/src/pygerber/backend/rasterized_2d/aperture_handle.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/backend/rasterized_2d/backend_cls.py` & `pygerber-2.3.0/src/pygerber/backend/rasterized_2d/backend_cls.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/backend/rasterized_2d/color_scheme.py` & `pygerber-2.3.0/src/pygerber/backend/rasterized_2d/color_scheme.py`

 * *Files 4% similar despite different names*

```diff
@@ -198,7 +198,16 @@
     clear_color=RGBA.from_rgba(187, 8, 65, 255),
     solid_color=RGBA.from_rgba(19, 61, 145, 255),
     clear_region_color=RGBA.from_rgba(94, 52, 20, 255),
     solid_region_color=RGBA.from_rgba(21, 92, 130, 255),
     debug_1_color=RGBA.from_hex("#ababab"),
     debug_2_color=RGBA.from_hex("#7d7d7d"),
 )
+ColorScheme.DEBUG_1_ALPHA = ColorScheme(
+    background_color=RGBA.from_rgba(0, 0, 0, 0),
+    clear_color=RGBA.from_rgba(0, 0, 0, 0),
+    solid_color=RGBA.from_rgba(19, 61, 145, 255),
+    clear_region_color=RGBA.from_rgba(0, 0, 0, 0),
+    solid_region_color=RGBA.from_rgba(21, 92, 130, 255),
+    debug_1_color=RGBA.from_hex("#ababab"),
+    debug_2_color=RGBA.from_hex("#7d7d7d"),
+)
```

### Comparing `pygerber-2.2.1/src/pygerber/backend/rasterized_2d/draw_commands/draw_arc.py` & `pygerber-2.3.0/src/pygerber/backend/rasterized_2d/draw_commands/draw_arc.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/backend/rasterized_2d/draw_commands/draw_bounding_box.py` & `pygerber-2.3.0/src/pygerber/backend/rasterized_2d/draw_commands/draw_bounding_box.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/backend/rasterized_2d/draw_commands/draw_circle.py` & `pygerber-2.3.0/src/pygerber/backend/rasterized_2d/draw_commands/draw_circle.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/backend/rasterized_2d/draw_commands/draw_paste.py` & `pygerber-2.3.0/src/pygerber/backend/rasterized_2d/draw_commands/draw_paste.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/backend/rasterized_2d/draw_commands/draw_polygon.py` & `pygerber-2.3.0/src/pygerber/backend/rasterized_2d/draw_commands/draw_polygon.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/backend/rasterized_2d/draw_commands/draw_rectangle.py` & `pygerber-2.3.0/src/pygerber/backend/rasterized_2d/draw_commands/draw_rectangle.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/backend/rasterized_2d/draw_commands/draw_region.py` & `pygerber-2.3.0/src/pygerber/backend/rasterized_2d/draw_commands/draw_region.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/backend/rasterized_2d/draw_commands/draw_vector_line.py` & `pygerber-2.3.0/src/pygerber/backend/rasterized_2d/draw_commands/draw_vector_line.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/backend/rasterized_2d/drawing_target.py` & `pygerber-2.3.0/src/pygerber/backend/rasterized_2d/drawing_target.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/backend/rasterized_2d/errors.py` & `pygerber-2.3.0/src/pygerber/backend/rasterized_2d/errors.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/backend/rasterized_2d/image_tools.py` & `pygerber-2.3.0/src/pygerber/backend/rasterized_2d/image_tools.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/backend/rasterized_2d/result_handle.py` & `pygerber-2.3.0/src/pygerber/backend/rasterized_2d/result_handle.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/common/immutable_map_model.py` & `pygerber-2.3.0/src/pygerber/common/immutable_map_model.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/common/position.py` & `pygerber-2.3.0/src/pygerber/common/position.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/common/rgba.py` & `pygerber-2.3.0/src/pygerber/common/rgba.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/console/commands.py` & `pygerber-2.3.0/src/pygerber/console/commands.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/console/raster_2d_style.py` & `pygerber-2.3.0/src/pygerber/console/raster_2d_style.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/api/__init__.py` & `pygerber-2.3.0/src/pygerber/gerberx3/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/api/_errors.py` & `pygerber-2.3.0/src/pygerber/gerberx3/api/_errors.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/api/_layers.py` & `pygerber-2.3.0/src/pygerber/gerberx3/api/_layers.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/language_server/__main__.py` & `pygerber-2.3.0/src/pygerber/gerberx3/language_server/__main__.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/language_server/_internals/document.py` & `pygerber-2.3.0/src/pygerber/gerberx3/language_server/_internals/document.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/language_server/_internals/server.py` & `pygerber-2.3.0/src/pygerber/gerberx3/language_server/_internals/server.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/linter/diagnostic.py` & `pygerber-2.3.0/src/pygerber/gerberx3/linter/diagnostic.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/math/bounding_box.py` & `pygerber-2.3.0/src/pygerber/gerberx3/math/bounding_box.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/math/offset.py` & `pygerber-2.3.0/src/pygerber/gerberx3/math/offset.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/math/rotate_point.py` & `pygerber-2.3.0/src/pygerber/gerberx3/math/rotate_point.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/math/vector_2d.py` & `pygerber-2.3.0/src/pygerber/gerberx3/math/vector_2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,24 @@
     _GET_MIRRORED_DISPATCH_TABLE: ClassVar[dict[Mirroring, Callable[[Self], Self]]] = {
         Mirroring.NoMirroring: lambda s: s,
         Mirroring.X: _get_mirrored_x,
         Mirroring.Y: _get_mirrored_y,
         Mirroring.XY: _get_mirrored_xy,
     }
 
+    def get_rotated(self, angle: Decimal) -> Self:
+        """Get copy of this vector rotated around (0, 0)."""
+        return self.rotate_around_origin(angle)
+
+    def get_scaled(self, scale: Decimal) -> Vector2D:
+        """Get copy of this vector scaled by factor."""
+        if scale == Decimal("1.0"):
+            return self
+        return self * scale
+
     def as_pixels(self, dpi: int) -> tuple[int, int]:
         """Return size as pixels using given DPI for conversion."""
         return (self.x.as_pixels(dpi), self.y.as_pixels(dpi))
 
     def __eq__(self, other: object) -> bool:
         if isinstance(other, Vector2D):
             return self.x == other.x and self.y == other.y
@@ -220,18 +230,18 @@
 
         return self / self.length()
 
     def as_float_tuple(self) -> tuple[float, float]:
         """Return x, y Offset as tuple."""
         return (float(self.x.value), float(self.y.value))
 
-    def rotate_around_origin(self, angle_degrees: Decimal) -> Vector2D:
+    def rotate_around_origin(self, angle_degrees: Decimal) -> Self:
         """Return vector rotated x degrees around origin."""
         angle_radians = math.radians(angle_degrees)
-        return Vector2D(
+        return self.__class__(
             x=self.x * math.cos(angle_radians) - self.y * math.sin(angle_radians),
             y=self.x * math.sin(angle_radians) + self.y * math.cos(angle_radians),
         )
 
 
 Vector2D.NULL = Vector2D(x=Offset.NULL, y=Offset.NULL)
 Vector2D.UNIT_X = Vector2D(x=Offset(value=Decimal(1)), y=Offset.NULL)
```

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/parser/errors.py` & `pygerber-2.3.0/src/pygerber/gerberx3/parser/errors.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/parser/parser.py` & `pygerber-2.3.0/src/pygerber/gerberx3/parser/parser.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/parser/state.py` & `pygerber-2.3.0/src/pygerber/gerberx3/parser/state.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/parser2/apertures2/aperture2.py` & `pygerber-2.3.0/src/pygerber/gerberx3/parser2/apertures2/aperture2.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,29 +6,48 @@
 from pydantic import Field
 
 from pygerber.common.frozen_general_model import FrozenGeneralModel
 from pygerber.common.immutable_map_model import ImmutableMapping
 from pygerber.gerberx3.math.bounding_box import BoundingBox
 from pygerber.gerberx3.math.offset import Offset
 from pygerber.gerberx3.parser2.attributes2 import ApertureAttributes
+from pygerber.gerberx3.state_enums import Mirroring
+from pygerber.gerberx3.tokenizer.aperture_id import ApertureID
 
 if TYPE_CHECKING:
+    from decimal import Decimal
+
+    from typing_extensions import Self
+
     from pygerber.gerberx3.parser2.commands2.flash2 import Flash2
     from pygerber.gerberx3.renderer2.abstract import Renderer2
 
 
 class Aperture2(FrozenGeneralModel):
     """Parser level abstraction of aperture info."""
 
+    identifier: ApertureID
     attributes: ApertureAttributes = Field(default_factory=ImmutableMapping)
 
     def render_flash(self, renderer: Renderer2, command: Flash2) -> None:
         """Render draw operation."""
         raise NotImplementedError
 
     def get_bounding_box(self) -> BoundingBox:
         """Return bounding box of aperture."""
         raise NotImplementedError
 
     def get_stroke_width(self) -> Offset:
         """Get stroke width of command."""
         raise NotImplementedError
+
+    def get_mirrored(self, mirror: Mirroring) -> Self:  # noqa: ARG002
+        """Get mirrored aperture."""
+        return self
+
+    def get_rotated(self, angle: Decimal) -> Self:  # noqa: ARG002
+        """Get copy of this aperture rotated around (0, 0)."""
+        return self
+
+    def get_scaled(self, scale: Decimal) -> Self:  # noqa: ARG002
+        """Get copy of this aperture scaled by factor."""
+        return self
```

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/parser2/apertures2/block2.py` & `pygerber-2.3.0/src/pygerber/gerberx3/parser2/commands2/aperture_draw_command2.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,31 @@
-"""Parser level abstraction of block aperture info for Gerber AST parser, version 2."""
+"""Parser level abstraction of draw operation which utilizes apertures for Gerber AST
+parser, version 2.
+"""
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Generator
+
+from pydantic import Field
 
-from pygerber.gerberx3.math.bounding_box import BoundingBox
 from pygerber.gerberx3.parser2.apertures2.aperture2 import Aperture2
-from pygerber.gerberx3.parser2.command_buffer2 import (
-    ReadonlyCommandBuffer2,
-)
+from pygerber.gerberx3.parser2.attributes2 import ObjectAttributes
+from pygerber.gerberx3.parser2.commands2.command2 import Command2
 
 if TYPE_CHECKING:
-    from pygerber.gerberx3.parser2.commands2.flash2 import Flash2
     from pygerber.gerberx3.renderer2.abstract import Renderer2
 
 
-class Block2(Aperture2):
-    """Parser level abstraction of aperture info for block aperture."""
+class ApertureDrawCommand2(Command2):
+    """Parser level abstraction of draw operation for Gerber AST parser, version 2."""
 
-    command_buffer: ReadonlyCommandBuffer2
+    attributes: ObjectAttributes = Field(default_factory=ObjectAttributes)
+    aperture: Aperture2
 
-    def render_flash(self, renderer: Renderer2, command: Flash2) -> None:
+    def render_iter(self, hooks: Renderer2) -> Generator[Command2, None, None]:
         """Render draw operation."""
-        # Block apertures are resolved into series of commands at parser level.
-        raise NotImplementedError
+        self.render(hooks)
+        yield self
 
-    def get_bounding_box(self) -> BoundingBox:
-        """Return bounding box of aperture."""
-        return self.command_buffer.get_bounding_box()
+    def __str__(self) -> str:
+        return f"{self.__class__.__qualname__}()"
```

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/parser2/apertures2/circle2.py` & `pygerber-2.3.0/src/pygerber/gerberx3/parser2/apertures2/polygon2.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,45 +1,49 @@
-"""Parser level abstraction of circle aperture info for Gerber AST parser, version 2."""
+"""Parser level abstraction of polygon aperture info for Gerber AST parser,
+version 2.
+"""
 from __future__ import annotations
 
+from decimal import Decimal  # noqa: TCH003
 from typing import TYPE_CHECKING, Optional
 
 from pygerber.gerberx3.math.bounding_box import BoundingBox
 from pygerber.gerberx3.math.offset import Offset
 from pygerber.gerberx3.parser2.apertures2.aperture2 import Aperture2
 
 if TYPE_CHECKING:
+    from typing_extensions import Self
+
     from pygerber.gerberx3.parser2.commands2.flash2 import Flash2
     from pygerber.gerberx3.renderer2.abstract import Renderer2
 
 
-class Circle2(Aperture2):
-    """Parser level abstraction of aperture info for circle aperture."""
+class Polygon2(Aperture2):
+    """Parser level abstraction of aperture info for polygon aperture."""
 
-    diameter: Offset
+    outer_diameter: Offset
+    number_vertices: int
+    rotation: Decimal
     hole_diameter: Optional[Offset]
 
     def render_flash(self, renderer: Renderer2, command: Flash2) -> None:
         """Render draw operation."""
-        renderer.hooks.render_flash_circle(command, self)
+        renderer.hooks.render_flash_polygon(command, self)
 
     def get_bounding_box(self) -> BoundingBox:
-        """Get bounding box of draw operation."""
-        return BoundingBox.from_diameter(self.diameter)
+        """Return bounding box of aperture."""
+        return BoundingBox.from_diameter(self.outer_diameter)
 
     def get_stroke_width(self) -> Offset:
         """Get stroke width of command."""
-        return self.diameter
-
+        return self.outer_diameter
 
-class NoCircle2(Circle2):
-    """Dummy aperture representing case when aperture is not needed but has to be
-    given to denote width of draw line command.
-    """
-
-    def render_flash(self, renderer: Renderer2, command: Flash2) -> None:
-        """Render draw operation."""
-        renderer.hooks.render_flash_no_circle(command, self)
-
-    def get_bounding_box(self) -> BoundingBox:
-        """Get bounding box of draw operation."""
-        return BoundingBox.NULL
+    def get_scaled(self, scale: Decimal) -> Self:
+        """Get copy of this aperture scaled by factor."""
+        return self.model_copy(
+            update={
+                "outer_diameter": self.outer_diameter * scale,
+                "hole_diameter": (
+                    None if self.hole_diameter is None else self.hole_diameter * scale
+                ),
+            },
+        )
```

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/parser2/apertures2/polygon2.py` & `pygerber-2.3.0/src/pygerber/gerberx3/parser2/apertures2/rectangle2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,51 @@
-"""Parser level abstraction of polygon aperture info for Gerber AST parser,
+"""Parser level abstraction of rectangle aperture info for Gerber AST parser,
 version 2.
 """
+
 from __future__ import annotations
 
-from decimal import Decimal  # noqa: TCH003
 from typing import TYPE_CHECKING, Optional
 
 from pygerber.gerberx3.math.bounding_box import BoundingBox
 from pygerber.gerberx3.math.offset import Offset
 from pygerber.gerberx3.parser2.apertures2.aperture2 import Aperture2
 
 if TYPE_CHECKING:
+    from decimal import Decimal
+
+    from typing_extensions import Self
+
     from pygerber.gerberx3.parser2.commands2.flash2 import Flash2
     from pygerber.gerberx3.renderer2.abstract import Renderer2
 
 
-class Polygon2(Aperture2):
-    """Parser level abstraction of aperture info for polygon aperture."""
+class Rectangle2(Aperture2):
+    """Parser level abstraction of aperture info for rectangle aperture."""
 
-    outer_diameter: Offset
-    number_vertices: int
-    rotation: Decimal
+    x_size: Offset
+    y_size: Offset
     hole_diameter: Optional[Offset]
 
     def render_flash(self, renderer: Renderer2, command: Flash2) -> None:
         """Render draw operation."""
-        renderer.hooks.render_flash_polygon(command, self)
+        renderer.hooks.render_flash_rectangle(command, self)
+
+    def get_stroke_width(self) -> Offset:
+        """Return stroke width of aperture."""
+        return (self.x_size + self.y_size) / 2
 
     def get_bounding_box(self) -> BoundingBox:
         """Return bounding box of aperture."""
-        return BoundingBox.from_diameter(self.outer_diameter)
+        return BoundingBox.from_rectangle(self.x_size, self.y_size)
 
-    def get_stroke_width(self) -> Offset:
-        """Get stroke width of command."""
-        return self.outer_diameter
+    def get_scaled(self, scale: Decimal) -> Self:
+        """Get copy of this aperture scaled by factor."""
+        return self.model_copy(
+            update={
+                "x_size": self.x_size * scale,
+                "y_size": self.y_size * scale,
+                "hole_diameter": (
+                    None if self.hole_diameter is None else self.hole_diameter * scale
+                ),
+            },
+        )
```

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/parser2/attributes2.py` & `pygerber-2.3.0/src/pygerber/gerberx3/parser2/attributes2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/parser2/command_buffer2.py` & `pygerber-2.3.0/src/pygerber/gerberx3/parser2/command_buffer2.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 from pygerber.common.frozen_general_model import FrozenGeneralModel
 from pygerber.gerberx3.math.bounding_box import BoundingBox
 from pygerber.gerberx3.math.vector_2d import Vector2D
 from pygerber.gerberx3.parser2.commands2.command2 import Command2
 from pygerber.gerberx3.state_enums import Mirroring
 
 if TYPE_CHECKING:
+    from decimal import Decimal
+
     from typing_extensions import Self
 
     from pygerber.gerberx3.parser2.context2 import Parser2Context
 
 
 class CommandBuffer2:
     """Container for buffering draw commands."""
@@ -80,14 +82,26 @@
 
     def get_transposed(self, vector: Vector2D) -> Self:
         """Get new command buffer with all commands transposed."""
         return self.model_copy(
             update={"commands": [c.get_transposed(vector) for c in self.commands]},
         )
 
+    def get_rotated(self, angle: Decimal) -> Self:
+        """Get copy of this command rotated around (0, 0)."""
+        return self.model_copy(
+            update={"commands": [c.get_rotated(angle) for c in self.commands]},
+        )
+
+    def get_scaled(self, scale: Decimal) -> Self:
+        """Get copy of this aperture scaled by factor."""
+        return self.model_copy(
+            update={"commands": [c.get_scaled(scale) for c in self.commands]},
+        )
+
     def get_bounding_box(self) -> BoundingBox:
         """Get bounding box of command buffer."""
         bbox: Optional[BoundingBox] = None
 
         for command in self:
             if bbox is None:
                 bbox = command.get_bounding_box()
```

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/parser2/commands2/arc2.py` & `pygerber-2.3.0/src/pygerber/gerberx3/parser2/commands2/arc2.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Parser level abstraction of draw arc operation for Gerber AST parser, version 2."""
 from __future__ import annotations
 
+from decimal import Decimal
 from typing import TYPE_CHECKING
 
 from pygerber.gerberx3.math.bounding_box import BoundingBox
 from pygerber.gerberx3.math.offset import Offset
 from pygerber.gerberx3.math.vector_2d import Vector2D
 from pygerber.gerberx3.parser2.commands2.aperture_draw_command2 import (
     ApertureDrawCommand2,
@@ -48,33 +49,76 @@
             BoundingBox.from_diameter(
                 (self.get_radius() * 2) + (self.aperture.get_stroke_width() * 2),
             )
             + self.center_point
         )
 
     def get_mirrored(self, mirror: Mirroring) -> Self:
-        """Get mirrored command."""
+        """Get mirrored command.
+
+        Mirroring is a NOOP if mirror is `Mirroring.NoMirroring`.
+        """
+        if mirror == Mirroring.NoMirroring:
+            return self
+
+        new_end_point = self.end_point.get_mirrored(mirror)
+        new_start_point = self.start_point.get_mirrored(mirror)
+        new_center_point = self.center_point.get_mirrored(mirror)
+
+        if mirror == Mirroring.XY:
+            return self.model_copy(
+                update={
+                    "end_point": new_end_point,
+                    "start_point": new_start_point,
+                    "center_point": new_center_point,
+                },
+            )
+
         return self.model_copy(
             update={
-                "start_point": self.start_point.get_mirrored(mirror),
-                "end_point": self.end_point.get_mirrored(mirror),
-                "center_point": self.center_point.get_mirrored(mirror),
+                "end_point": new_start_point,
+                "start_point": new_end_point,
+                "center_point": new_center_point,
+            },
+        )
+
+    def get_rotated(self, angle: Decimal) -> Self:
+        """Get copy of this command rotated around (0, 0)."""
+        return self.model_copy(
+            update={
+                "start_point": self.start_point.get_rotated(angle),
+                "end_point": self.end_point.get_rotated(angle),
+                "center_point": self.center_point.get_rotated(angle),
             },
         )
 
     def get_transposed(self, vector: Vector2D) -> Self:
         """Get transposed command."""
         return self.model_copy(
             update={
                 "start_point": self.start_point + vector,
                 "end_point": self.end_point + vector,
                 "center_point": self.center_point + vector,
             },
         )
 
+    def get_scaled(self, scale: Decimal) -> Self:
+        """Get copy of this aperture scaled by factor."""
+        if scale == Decimal("1.0"):
+            return self
+        return self.model_copy(
+            update={
+                "start_point": self.start_point.get_scaled(scale),
+                "end_point": self.end_point.get_scaled(scale),
+                "center_point": self.center_point.get_scaled(scale),
+                "aperture": self.aperture.get_scaled(scale),
+                "transform": self.transform.get_scaled(scale),
+            },
+        )
+
     def render(self, renderer: Renderer2) -> None:
         """Render draw operation."""
         renderer.hooks.render_arc(self)
 
 
 class CCArc2(Arc2):
     """Parser level abstraction of draw counterclockwise arc operation for Gerber AST
```

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/parser2/commands2/buffer_command2.py` & `pygerber-2.3.0/src/pygerber/gerberx3/parser2/commands2/buffer_command2.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,56 +1,85 @@
 """Parser level abstraction of command that consists of multiple commands for Gerber AST
 parser, version 2.
 """
+
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Iterator
+from typing import TYPE_CHECKING, Generator, Iterator
 
 from pygerber.gerberx3.math.bounding_box import BoundingBox
 from pygerber.gerberx3.parser2.command_buffer2 import ReadonlyCommandBuffer2
 from pygerber.gerberx3.parser2.commands2.command2 import Command2
 from pygerber.gerberx3.state_enums import Mirroring
 
 if TYPE_CHECKING:
+    from decimal import Decimal
+
     from typing_extensions import Self
 
     from pygerber.gerberx3.math.vector_2d import Vector2D
     from pygerber.gerberx3.renderer2.abstract import Renderer2
 
 
 class BufferCommand2(Command2):
     """Parser level abstraction of command that consists of multiple commands for Gerber
     AST parser, version 2.
     """
 
     command_buffer: ReadonlyCommandBuffer2
 
     def get_mirrored(self, mirror: Mirroring) -> Self:
-        """Get mirrored command."""
+        """Get mirrored command.
+
+        Mirroring is a NOOP if mirror is `Mirroring.NoMirroring`.
+        """
+        if mirror == Mirroring.NoMirroring:
+            return self
         return self.model_copy(
             update={
                 "command_buffer": self.command_buffer.get_mirrored(mirror),
             },
         )
 
     def get_transposed(self, vector: Vector2D) -> Self:
         """Get transposed command."""
         return self.model_copy(
             update={
                 "command_buffer": self.command_buffer.get_transposed(vector),
             },
         )
 
+    def get_rotated(self, angle: Decimal) -> Self:
+        """Get copy of this command rotated around (0, 0)."""
+        return self.model_copy(
+            update={
+                "command_buffer": self.command_buffer.get_rotated(angle),
+            },
+        )
+
+    def get_scaled(self, scale: Decimal) -> Self:
+        """Get copy of this aperture scaled by factor."""
+        return self.model_copy(
+            update={
+                "command_buffer": self.command_buffer.get_scaled(scale),
+            },
+        )
+
     def get_bounding_box(self) -> BoundingBox:
         """Get bounding box of draw operation."""
         return self.command_buffer.get_bounding_box()
 
     def render(self, renderer: Renderer2) -> None:
         """Render draw operation."""
-        renderer.hooks.render_buffer(self)
+        for _ in renderer.hooks.render_buffer(self):
+            pass
+
+    def render_iter(self, renderer: Renderer2) -> Generator[Command2, None, None]:
+        """Render draw operation."""
+        yield from renderer.hooks.render_buffer(self)
 
     def __len__(self) -> int:
         """Return length of buffered commands."""
         return len(self.command_buffer)
 
     def __iter__(self) -> Iterator[Command2]:  # type: ignore[override]
         """Iterate over buffered draw commands."""
```

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/parser2/commands2/command2.py` & `pygerber-2.3.0/src/pygerber/gerberx3/parser2/commands2/command2.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 """Parser level abstraction of draw operation for Gerber AST parser, version 2."""
+
 from __future__ import annotations
 
 import json
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Generator
 
 from pygerber.common.frozen_general_model import FrozenGeneralModel
 from pygerber.gerberx3.math.bounding_box import BoundingBox
 from pygerber.gerberx3.math.vector_2d import Vector2D
 from pygerber.gerberx3.parser2.state2 import ApertureTransform
 from pygerber.gerberx3.state_enums import Mirroring
 
 if TYPE_CHECKING:
+    from decimal import Decimal
+
     from typing_extensions import Self
 
     from pygerber.gerberx3.renderer2.abstract import Renderer2
 
 
 class Command2(FrozenGeneralModel):
     """Parser level abstraction of draw operation for Gerber AST parser, version 2."""
@@ -22,24 +25,43 @@
     transform: ApertureTransform
 
     def get_bounding_box(self) -> BoundingBox:
         """Get bounding box of draw operation."""
         raise NotImplementedError
 
     def get_mirrored(self, mirror: Mirroring) -> Self:
-        """Get mirrored command."""
+        """Get mirrored command.
+
+        Mirroring is a NOOP if mirror is `Mirroring.NoMirroring`.
+        """
         raise NotImplementedError
 
     def get_transposed(self, vector: Vector2D) -> Self:
         """Get transposed command."""
         raise NotImplementedError
 
-    def render(self, hooks: Renderer2) -> None:
+    def get_rotated(self, angle: Decimal) -> Self:
+        """Get copy of this command rotated around (0, 0)."""
+        raise NotImplementedError
+
+    def get_scaled(self, scale: Decimal) -> Self:
+        """Get copy of this aperture scaled by factor."""
+        raise NotImplementedError
+
+    def render(self, renderer: Renderer2) -> None:
+        """Render draw operation."""
+        raise NotImplementedError
+
+    def render_iter(
+        self,
+        renderer: Renderer2,  # noqa: ARG002
+    ) -> Generator[Command2, None, None]:
         """Render draw operation."""
         raise NotImplementedError
+        yield  # type: ignore[unreachable]
 
     def command_to_json(self) -> str:
         """Dump draw operation."""
         return json.dumps(
             {
                 "cls": f"{self.__module__}.{self.__class__.__qualname__}",
                 "dict": json.loads(self.model_dump_json()),
```

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/parser2/commands2/flash2.py` & `pygerber-2.3.0/src/pygerber/gerberx3/parser2/apertures2/macro2.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,48 +1,61 @@
-"""Parser level abstraction of flash operation for Gerber AST parser, version 2."""
+"""Parser level abstraction of macro aperture info for Gerber AST parser, version 2."""
+
 from __future__ import annotations
 
+from decimal import Decimal
 from typing import TYPE_CHECKING
 
 from pygerber.gerberx3.math.bounding_box import BoundingBox
-from pygerber.gerberx3.math.vector_2d import Vector2D
-from pygerber.gerberx3.parser2.commands2.aperture_draw_command2 import (
-    ApertureDrawCommand2,
-)
+from pygerber.gerberx3.parser2.apertures2.aperture2 import Aperture2
+from pygerber.gerberx3.parser2.command_buffer2 import ReadonlyCommandBuffer2
 from pygerber.gerberx3.state_enums import Mirroring
 
 if TYPE_CHECKING:
     from typing_extensions import Self
 
+    from pygerber.gerberx3.parser2.commands2.flash2 import Flash2
     from pygerber.gerberx3.renderer2.abstract import Renderer2
 
 
-class Flash2(ApertureDrawCommand2):
-    """Parser level abstraction of flash operation for Gerber AST parser,
-    version 2.
-    """
+class Macro2(Aperture2):
+    """Parser level abstraction of aperture info for macro aperture."""
+
+    command_buffer: ReadonlyCommandBuffer2
+
+    def render_flash(self, renderer: Renderer2, command: Flash2) -> None:
+        """Render draw operation."""
+        renderer.hooks.render_flash_macro(command, self)
 
-    flash_point: Vector2D
+    def get_bounding_box(self) -> BoundingBox:
+        """Return bounding box of aperture."""
+        return self.command_buffer.get_bounding_box()
 
     def get_mirrored(self, mirror: Mirroring) -> Self:
-        """Get mirrored command."""
+        """Get mirrored aperture."""
+        if mirror == Mirroring.NoMirroring:
+            return self
         return self.model_copy(
             update={
-                "flash_point": self.flash_point.get_mirrored(mirror),
+                "command_buffer": self.command_buffer.get_mirrored(mirror),
             },
         )
 
-    def get_transposed(self, vector: Vector2D) -> Self:
-        """Get transposed command."""
+    def get_rotated(self, angle: Decimal) -> Self:
+        """Get copy of this aperture rotated around (0, 0)."""
+        if angle == Decimal("0.0"):
+            return self
         return self.model_copy(
             update={
-                "flash_point": self.flash_point + vector,
+                "command_buffer": self.command_buffer.get_rotated(angle),
             },
         )
 
-    def render(self, renderer: Renderer2) -> None:
-        """Render draw operation."""
-        self.aperture.render_flash(renderer, self)
-
-    def get_bounding_box(self) -> BoundingBox:
-        """Get bounding box of draw operation."""
-        return self.aperture.get_bounding_box() + self.flash_point
+    def get_scaled(self, scale: Decimal) -> Self:
+        """Get copy of this aperture scaled by factor."""
+        if scale == Decimal("1.0"):
+            return self
+        return self.model_copy(
+            update={
+                "command_buffer": self.command_buffer.get_scaled(scale),
+            },
+        )
```

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/parser2/commands2/line2.py` & `pygerber-2.3.0/src/pygerber/gerberx3/parser2/commands2/line2.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Parser level abstraction of draw line operation for Gerber AST parser, version 2."""
 from __future__ import annotations
 
+from decimal import Decimal
 from typing import TYPE_CHECKING
 
 from pygerber.gerberx3.math.bounding_box import BoundingBox
 from pygerber.gerberx3.math.vector_2d import Vector2D
 from pygerber.gerberx3.parser2.commands2.aperture_draw_command2 import (
     ApertureDrawCommand2,
 )
@@ -26,15 +27,20 @@
 
     def get_bounding_box(self) -> BoundingBox:
         """Return bounding box of draw operation."""
         vertex_box = self.aperture.get_bounding_box()
         return (vertex_box + self.start_point) + (vertex_box + self.end_point)
 
     def get_mirrored(self, mirror: Mirroring) -> Self:
-        """Get mirrored command."""
+        """Get mirrored command.
+
+        Mirroring is a NOOP if mirror is `Mirroring.NoMirroring`.
+        """
+        if mirror == Mirroring.NoMirroring:
+            return self
         return self.model_copy(
             update={
                 "start_point": self.start_point.get_mirrored(mirror),
                 "end_point": self.end_point.get_mirrored(mirror),
             },
         )
 
@@ -43,10 +49,32 @@
         return self.model_copy(
             update={
                 "start_point": self.start_point + vector,
                 "end_point": self.end_point + vector,
             },
         )
 
+    def get_rotated(self, angle: Decimal) -> Self:
+        """Get copy of this command rotated around (0, 0)."""
+        return self.model_copy(
+            update={
+                "start_point": self.start_point.get_rotated(angle),
+                "end_point": self.end_point.get_rotated(angle),
+            },
+        )
+
+    def get_scaled(self, scale: Decimal) -> Self:
+        """Get copy of this aperture scaled by factor."""
+        if scale == Decimal("1.0"):
+            return self
+        return self.model_copy(
+            update={
+                "start_point": self.start_point.get_scaled(scale),
+                "end_point": self.end_point.get_scaled(scale),
+                "aperture": self.aperture.get_scaled(scale),
+                "transform": self.transform.get_scaled(scale),
+            },
+        )
+
     def render(self, renderer: Renderer2) -> None:
         """Render draw operation."""
         renderer.hooks.render_line(self)
```

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/parser2/commands2/region2.py` & `pygerber-2.3.0/src/pygerber/gerberx3/parser2/commands2/region2.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """Parser level abstraction of draw region operation for Gerber AST parser,
 version 2.
 """
+
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Generator
 
 from pydantic import Field
 
 from pygerber.gerberx3.parser2.attributes2 import ApertureAttributes, ObjectAttributes
 from pygerber.gerberx3.parser2.command_buffer2 import ReadonlyCommandBuffer2
 from pygerber.gerberx3.parser2.commands2.buffer_command2 import BufferCommand2
+from pygerber.gerberx3.parser2.commands2.command2 import Command2
 
 if TYPE_CHECKING:
     from pygerber.gerberx3.renderer2.abstract import Renderer2
 
 
 class Region2(BufferCommand2):
     """Parser level abstraction of draw region operation for Gerber AST parser,
@@ -34,7 +36,12 @@
             self.command_buffer.debug_buffer_to_json(8)}
     }}
 }}"""  # noqa: E501
 
     def render(self, renderer: Renderer2) -> None:
         """Render draw operation."""
         renderer.hooks.render_region(self)
+
+    def render_iter(self, renderer: Renderer2) -> Generator[Command2, None, None]:
+        """Render draw operation."""
+        renderer.hooks.render_region(self)
+        yield self
```

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/parser2/context2.py` & `pygerber-2.3.0/src/pygerber/gerberx3/parser2/context2.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 from pygerber.gerberx3.parser2.macro2.expressions2.constant2 import Constant2
 from pygerber.gerberx3.parser2.macro2.expressions2.unary2 import Negation2, Positive2
 from pygerber.gerberx3.parser2.macro2.expressions2.variable_name import VariableName2
 from pygerber.gerberx3.parser2.macro2.macro2 import ApertureMacro2
 from pygerber.gerberx3.parser2.macro2.statement_buffer2 import StatementBuffer2
 from pygerber.gerberx3.parser2.parser2hooks import Parser2Hooks
 from pygerber.gerberx3.parser2.parser2hooks_base import Parser2HooksBase
-from pygerber.gerberx3.parser2.state2 import State2
+from pygerber.gerberx3.parser2.state2 import ApertureTransform, State2
 from pygerber.gerberx3.state_enums import AxisCorrespondence
 from pygerber.gerberx3.tokenizer.aperture_id import ApertureID
 
 if TYPE_CHECKING:
     from decimal import Decimal
 
     from pygerber.gerberx3.math.vector_2d import Vector2D
@@ -94,14 +94,15 @@
         self.macro_expressions = (
             Parser2ContextMacroExpressionFactories()
             if self.options.custom_macro_expression_factories is None
             else self.options.custom_macro_expression_factories
         )
         self.apertures: dict[ApertureID, Aperture2] = {
             REGION_OUTLINE_DEFAULT_APERTURE_ID: NoCircle2(
+                identifier=REGION_OUTLINE_DEFAULT_APERTURE_ID,
                 diameter=Offset.NULL,
                 hole_diameter=None,
             ),
         }
 
     def push_block_command_buffer(self) -> None:
         """Add new command buffer for block aperture draw commands."""
@@ -461,20 +462,43 @@
 
     def set_current_aperture_id(self, current_aperture: Optional[ApertureID]) -> None:
         """Set the current_aperture property value."""
         return self.set_state(
             self.get_state().set_current_aperture_id(current_aperture),
         )
 
-    def get_aperture(self, __key: ApertureID) -> Aperture2:
+    def get_aperture(
+        self,
+        __key: ApertureID,
+        transform: ApertureTransform,
+    ) -> Aperture2:
         """Get apertures property value."""
+        key_with_transform = ApertureID(
+            f"{__key}+{transform.get_transform_key()}",
+        )
+        transformed_aperture = self.apertures.get(key_with_transform)
+        if transformed_aperture is None:
+            # Retrieve aperture with no transform and create a transformed copy.
+            # If transform is all default, no copy is made.
+            aperture = self._get_aperture(__key)
+            transformed_aperture = (
+                aperture.get_mirrored(transform.mirroring)
+                .get_rotated(transform.rotation)
+                .get_scaled(transform.scaling)
+            )
+            self.set_aperture(key_with_transform, transformed_aperture)
+
+        return transformed_aperture
+
+    def _get_aperture(self, __key: ApertureID) -> Aperture2:
         try:
-            return self.apertures[__key]
+            aperture = self.apertures[__key]
         except KeyError as e:
             raise ApertureNotDefined2Error(self.current_token) from e
+        return aperture
 
     def set_aperture(self, __key: ApertureID, __value: Aperture2) -> None:
         """Set the apertures property value."""
         self.apertures[__key] = __value
 
     def get_macro(self, __key: str) -> ApertureMacro2:
         """Get macro property value."""
```

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/parser2/errors2.py` & `pygerber-2.3.0/src/pygerber/gerberx3/parser2/errors2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/parser2/macro2/assignment2.py` & `pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/assignment2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/parser2/macro2/expressions2/binary2.py` & `pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/expressions2/binary2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/parser2/macro2/expressions2/constant2.py` & `pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/expressions2/constant2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/parser2/macro2/expressions2/expression2.py` & `pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/expressions2/expression2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/parser2/macro2/expressions2/unary2.py` & `pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/expressions2/unary2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/parser2/macro2/expressions2/variable_name.py` & `pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/expressions2/variable_name.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/parser2/macro2/macro2.py` & `pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/macro2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/parser2/macro2/primitives2/code_1_circle2.py` & `pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/primitives2/code_1_circle2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/parser2/macro2/primitives2/code_20_vector_line2.py` & `pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/primitives2/code_20_vector_line2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/parser2/macro2/primitives2/code_21_center_line2.py` & `pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/primitives2/code_21_center_line2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/parser2/macro2/primitives2/code_22_lower_left_line2.py` & `pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/primitives2/code_22_lower_left_line2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/parser2/macro2/primitives2/code_2_vector_line2.py` & `pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/primitives2/code_2_vector_line2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/parser2/macro2/primitives2/code_4_outline2.py` & `pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/primitives2/code_4_outline2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/parser2/macro2/primitives2/code_5_polygon2.py` & `pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/primitives2/code_5_polygon2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/parser2/macro2/primitives2/code_6_moire2.py` & `pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/primitives2/code_6_moire2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/parser2/macro2/primitives2/code_7_thermal2.py` & `pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/primitives2/code_7_thermal2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/parser2/macro2/statement2.py` & `pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/statement2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/parser2/macro2/statement_buffer2.py` & `pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/statement_buffer2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/parser2/parser2.py` & `pygerber-2.3.0/src/pygerber/gerberx3/parser2/parser2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/parser2/parser2hooks.py` & `pygerber-2.3.0/src/pygerber/gerberx3/parser2/parser2hooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 from pygerber.gerberx3.state_enums import (
     DrawMode,
     ImagePolarityEnum,
     Mirroring,
     Polarity,
     Unit,
 )
+from pygerber.gerberx3.tokenizer.aperture_id import ApertureID
 from pygerber.gerberx3.tokenizer.tokens.fs_coordinate_format import (
     CoordinateParser,
 )
 
 if TYPE_CHECKING:
     from pygerber.gerberx3.parser2.context2 import Parser2Context
     from pygerber.gerberx3.tokenizer.tokens.ab_block_aperture import (
@@ -556,14 +557,15 @@
             identifier = context.get_aperture_block_id()
             if identifier is None:
                 raise UnnamedBlockApertureNotAllowedError(token)
 
             context.set_aperture(
                 identifier,
                 Block2(
+                    identifier=identifier,
                     attributes=context.aperture_attributes,
                     command_buffer=command_buffer.get_readonly(),
                 ),
             )
             # Restore context state from before the block definition.
             context.set_state(context.pop_block_state())
             return super().on_parser_visit_token(token, context)
@@ -594,14 +596,15 @@
                 if token.hole_diameter is None
                 else Offset.new(token.hole_diameter, context.get_draw_units())
             )
 
             context.set_aperture(
                 token.aperture_id,
                 Circle2(
+                    identifier=token.aperture_id,
                     attributes=context.aperture_attributes,
                     diameter=Offset.new(token.diameter, context.get_draw_units()),
                     hole_diameter=hole_diameter,
                 ),
             )
             return super().on_parser_visit_token(token, context)
 
@@ -631,14 +634,15 @@
                 if token.hole_diameter is None
                 else Offset.new(token.hole_diameter, context.get_draw_units())
             )
 
             context.set_aperture(
                 token.aperture_id,
                 Rectangle2(
+                    identifier=token.aperture_id,
                     attributes=context.aperture_attributes,
                     x_size=Offset.new(token.x_size, context.get_draw_units()),
                     y_size=Offset.new(token.y_size, context.get_draw_units()),
                     hole_diameter=hole_diameter,
                 ),
             )
             return super().on_parser_visit_token(token, context)
@@ -669,14 +673,15 @@
                 if token.hole_diameter is None
                 else Offset.new(token.hole_diameter, context.get_draw_units())
             )
 
             context.set_aperture(
                 token.aperture_id,
                 Obround2(
+                    identifier=token.aperture_id,
                     attributes=context.aperture_attributes,
                     x_size=Offset.new(token.x_size, context.get_draw_units()),
                     y_size=Offset.new(token.y_size, context.get_draw_units()),
                     hole_diameter=hole_diameter,
                 ),
             )
             return super().on_parser_visit_token(token, context)
@@ -708,14 +713,15 @@
                 else Offset.new(token.hole_diameter, context.get_draw_units())
             )
             rotation = Decimal("0.0") if token.rotation is None else token.rotation
 
             context.set_aperture(
                 token.aperture_id,
                 Polygon2(
+                    identifier=token.aperture_id,
                     attributes=context.aperture_attributes,
                     outer_diameter=Offset.new(
                         token.outer_diameter,
                         context.get_draw_units(),
                     ),
                     number_vertices=token.number_of_vertices,
                     rotation=rotation,
@@ -749,27 +755,37 @@
                 f"${i}": Decimal(param) for i, param in enumerate(token.am_param, 1)
             }
             macro.on_parser2_eval_statement(context)
 
             context.set_aperture(
                 token.aperture_id,
                 Macro2(
+                    identifier=token.aperture_id,
                     attributes=context.aperture_attributes,
                     command_buffer=context.get_macro_eval_buffer().get_readonly(),
                 ),
             )
 
             context.unset_macro_eval_buffer()
             context.macro_variable_buffer = {}
 
             return super().on_parser_visit_token(token, context)
 
     class MacroEvalHooks:
         """Hooks called when evaluating macro aperture."""
 
+        def __init__(self) -> None:
+            self.macro_id_counter = 0
+
+        def get_next_id(self) -> ApertureID:
+            """Get next aperture id for macro."""
+            next_id = ApertureID(self.macro_id_counter)
+            self.macro_id_counter += 1
+            return next_id
+
         def on_code_1_circle(
             self,
             context: Parser2Context,
             primitive: Code1Circle2,
         ) -> None:
             """Evaluate code 1 circle primitive."""
             exposure = primitive.exposure.on_parser2_eval_expression(context)
@@ -783,14 +799,15 @@
                     transform=ApertureTransform(
                         polarity=polarity,
                         mirroring=Mirroring.NoMirroring,
                         rotation=Decimal("0.0"),
                         scaling=Decimal("1.0"),
                     ),
                     aperture=Circle2(
+                        identifier=ApertureID(self.get_next_id()),
                         diameter=Offset.new(
                             primitive.diameter.on_parser2_eval_expression(context),
                             context.get_draw_units(),
                         ),
                         hole_diameter=None,
                     ),
                     flash_point=Vector2D(
@@ -828,14 +845,15 @@
             transform = ApertureTransform(
                 polarity=polarity,
                 mirroring=Mirroring.NoMirroring,
                 rotation=Decimal("0.0"),
                 scaling=Decimal("1.0"),
             )
             aperture = Circle2(
+                identifier=ApertureID(self.get_next_id()),
                 diameter=Offset.NULL,
                 hole_diameter=None,
             )
             context.get_macro_eval_buffer().add_command(
                 Region2(
                     transform=ApertureTransform(
                         polarity=polarity,
@@ -909,14 +927,15 @@
                     transform=ApertureTransform(
                         polarity=polarity,
                         mirroring=Mirroring.NoMirroring,
                         rotation=Decimal("0.0"),
                         scaling=Decimal("1.0"),
                     ),
                     aperture=Polygon2(
+                        identifier=ApertureID(self.get_next_id()),
                         outer_diameter=Offset.new(
                             primitive.diameter.on_parser2_eval_expression(
                                 context,
                             ),
                         ),
                         number_vertices=round(
                             primitive.number_of_vertices.on_parser2_eval_expression(
@@ -970,14 +989,15 @@
                     transform=ApertureTransform(
                         polarity=polarity,
                         mirroring=Mirroring.NoMirroring,
                         rotation=Decimal("0.0"),
                         scaling=Decimal("1.0"),
                     ),
                     aperture=NoCircle2(
+                        identifier=ApertureID(self.get_next_id()),
                         diameter=Offset.new(
                             primitive.width.on_parser2_eval_expression(context),
                             context.get_draw_units(),
                         ),
                         hole_diameter=None,
                     ),
                     start_point=Vector2D(
@@ -1020,14 +1040,15 @@
                     transform=ApertureTransform(
                         polarity=polarity,
                         mirroring=Mirroring.NoMirroring,
                         rotation=Decimal("0.0"),
                         scaling=Decimal("1.0"),
                     ),
                     aperture=Rectangle2(
+                        identifier=ApertureID(self.get_next_id()),
                         x_size=Offset.new(
                             primitive.width.on_parser2_eval_expression(context),
                             context.get_draw_units(),
                         ),
                         y_size=Offset.new(
                             primitive.height.on_parser2_eval_expression(context),
                             context.get_draw_units(),
@@ -1131,25 +1152,26 @@
 
             start_point = context.get_current_position()
             end_point = Vector2D(x=x, y=y)
 
             aperture_id = context.get_current_aperture_id() or throw(
                 ApertureNotSelected2Error(token),
             )
-            aperture = context.get_aperture(aperture_id)
+            transform = context.get_state().get_aperture_transform()
+            aperture = context.get_aperture(aperture_id, transform)
 
-            context.add_command(
-                Line2(
-                    attributes=context.object_attributes,
-                    aperture=aperture,
-                    start_point=start_point,
-                    end_point=end_point,
-                    transform=context.get_state().get_aperture_transform(),
-                ),
-            )
+            command = Line2(
+                attributes=context.object_attributes,
+                aperture=aperture,
+                start_point=start_point,
+                end_point=end_point,
+                transform=transform,
+            ).get_mirrored(transform.get_mirroring())
+
+            context.add_command(command)
             context.set_current_position(end_point)
 
         def on_parser_visit_token_arc(
             self,
             token: D01Draw,
             context: Parser2Context,
         ) -> None:
@@ -1219,26 +1241,26 @@
                 # use them to calculate center point relative to start point.
                 center_offset = Vector2D(x=i, y=j)
                 final_center_point = start_point + center_offset
 
             aperture_id = context.get_current_aperture_id() or throw(
                 ApertureNotSelected2Error(token),
             )
-            aperture = context.get_aperture(aperture_id)
+            transform = context.get_state().get_aperture_transform()
+            aperture = context.get_aperture(aperture_id, transform)
+            command = Arc2(
+                attributes=context.object_attributes,
+                aperture=aperture,
+                start_point=start_point,
+                end_point=end_point,
+                center_point=final_center_point,
+                transform=context.get_state().get_aperture_transform(),
+            ).get_mirrored(transform.get_mirroring())
 
-            context.add_command(
-                Arc2(
-                    attributes=context.object_attributes,
-                    aperture=aperture,
-                    start_point=start_point,
-                    end_point=end_point,
-                    center_point=final_center_point,
-                    transform=context.get_state().get_aperture_transform(),
-                ),
-            )
+            context.add_command(command)
             context.set_current_position(end_point)
 
         def on_parser_visit_token_cc_arc(
             self,
             token: D01Draw,
             context: Parser2Context,
         ) -> None:
@@ -1300,27 +1322,26 @@
             else:
                 center_offset = Vector2D(x=i, y=j)
                 final_center_point = start_point + center_offset
 
             aperture_id = context.get_current_aperture_id() or throw(
                 ApertureNotSelected2Error(token),
             )
-            aperture = context.get_aperture(aperture_id)
-
-            context.add_command(
-                CCArc2(
-                    attributes=context.object_attributes,
-                    aperture=aperture,
-                    start_point=start_point,
-                    end_point=end_point,
-                    center_point=final_center_point,
-                    transform=context.get_state().get_aperture_transform(),
-                ),
-            )
+            transform = context.get_state().get_aperture_transform()
+            aperture = context.get_aperture(aperture_id, transform)
+            command = CCArc2(
+                attributes=context.object_attributes,
+                aperture=aperture,
+                start_point=start_point,
+                end_point=end_point,
+                center_point=final_center_point,
+                transform=context.get_state().get_aperture_transform(),
+            ).get_mirrored(transform.get_mirroring())
 
+            context.add_command(command)
             context.set_current_position(end_point)
 
         DRAW_MODE_DISPATCH_TABLE = MappingProxyType(
             {
                 DrawMode.Linear: on_parser_visit_token_line,
                 DrawMode.ClockwiseCircular: on_parser_visit_token_arc,
                 DrawMode.CounterclockwiseCircular: on_parser_visit_token_cc_arc,
@@ -1381,33 +1402,33 @@
             y = state.parse_coordinate(token.y)
 
             flash_point = Vector2D(x=x, y=y)
 
             aperture_id = context.get_current_aperture_id() or throw(
                 ApertureNotSelected2Error(token),
             )
-            aperture = context.get_aperture(aperture_id)
+            transform = context.get_state().get_aperture_transform()
+            aperture = context.get_aperture(aperture_id, transform)
 
             if isinstance(aperture, Block2):
+                cmd_buffer = aperture.command_buffer.get_transposed(flash_point)
                 context.add_command(
                     BufferCommand2(
-                        transform=context.get_state().get_aperture_transform(),
-                        command_buffer=aperture.command_buffer.get_transposed(
-                            flash_point,
-                        ),
+                        transform=transform,
+                        command_buffer=cmd_buffer,
                     ),
                 )
 
             else:
                 context.add_command(
                     Flash2(
                         attributes=context.object_attributes,
                         aperture=aperture,
                         flash_point=flash_point,
-                        transform=context.get_state().get_aperture_transform(),
+                        transform=transform,
                     ),
                 )
 
             context.set_current_position(flash_point)
             return super().on_parser_visit_token(token, context)
 
     class SelectApertureTokenHooks(Parser2HooksBase.SelectApertureTokenHooks):
@@ -1425,17 +1446,14 @@
             Parameters
             ----------
             token: TokenT
                 The token that is being visited.
             context : Parser2Context
                 The context object containing information about the parser state.
             """
-            context.get_aperture(
-                token.aperture_id,
-            )  # Make sure aperture exists.
             context.set_current_aperture_id(token.aperture_id)
             return super().on_parser_visit_token(token, context)
 
     class CoordinateFormatTokenHooks(Parser2HooksBase.CoordinateFormatTokenHooks):
         """Hooks for visiting coordinate format token (FS)."""
 
         def on_parser_visit_token(
```

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/parser2/parser2hooks_base.py` & `pygerber-2.3.0/src/pygerber/gerberx3/parser2/parser2hooks_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -425,15 +425,15 @@
     def on_parser_init(self, parser: Parser2) -> None:
         """Called after parser initialization."""
 
     def pre_parse(self, context: Parser2Context) -> None:
         """Called before parsing starts."""
 
     def post_parse(self, context: Parser2Context) -> None:
-        """Called after parsing starts."""
+        """Called after parsing finishes."""
 
     def on_parser_error(self, context: Parser2Context, error: Parser2Error) -> None:
         """Called when parsing error is thrown."""
 
     def on_other_error(self, context: Parser2Context, error: Exception) -> None:
         """Called when other error is thrown."""
```

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/parser2/state2.py` & `pygerber-2.3.0/src/pygerber/gerberx3/parser2/state2.py`

 * *Files 2% similar despite different names*

```diff
@@ -236,14 +236,33 @@
         """Set the scaling property value."""
         return self.model_copy(
             update={
                 "scaling": scaling,
             },
         )
 
+    def get_scaled(self, scale: Decimal) -> Self:
+        """Get copy of object scaled by factor."""
+        return self.model_copy(
+            update={
+                "scaling": self.scaling * scale,
+            },
+        )
+
+    def get_transform_key(self) -> str:
+        """Get key describing rotation and scaling."""
+        return (
+            f"*%{self.get_rotation():.3f}*%{self.get_scaling():.3f}"
+            f"*%{self.get_mirroring()}"
+        )
+
+    def has_mirroring_enabled(self) -> bool:
+        """Check if there is any mirroring set."""
+        return self.get_mirroring() is not Mirroring.NoMirroring
+
 
 class State2MacroIndex(ImmutableMapping[str, ApertureMacro2]):
     """Index of all macros defined in Gerber AST until currently parsed token."""
 
     def set_macro(self, __id: str, __macro: ApertureMacro2) -> Self:
         """Add new macro to macros index."""
         # TODO(argmaster): Add warning handling.  # noqa: TD003
```

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/renderer2/abstract.py` & `pygerber-2.3.0/src/pygerber/gerberx3/renderer2/abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Module contains base class Rendering backend for Parser2 based Gerber data
 structures.
 """
+
 from __future__ import annotations
 
 from pathlib import Path
 from typing import TYPE_CHECKING, BinaryIO, Generator, Optional
 
 from pygerber.gerberx3.parser2.apertures2.circle2 import Circle2, NoCircle2
 from pygerber.gerberx3.parser2.apertures2.macro2 import Macro2
@@ -45,24 +46,25 @@
     def render_iter(
         self,
         command_buffer: ReadonlyCommandBuffer2,
     ) -> Generator[Command2, None, None]:
         """Iterate over commands in buffer and render image for each command."""
         self.hooks.init(self, command_buffer)
         for command in command_buffer:
-            command.render(self)
-            yield command
+            yield from command.render_iter(self)
         self.hooks.finalize()
 
 
 class Renderer2HooksABC:
     """Hooks for implementing rendering of Gerber structures to a target format."""
 
     def init(self, renderer: Renderer2, command_buffer: ReadonlyCommandBuffer2) -> None:
         """Initialize rendering."""
+        self.renderer = renderer
+        self.command_buffer = command_buffer
 
     def render_line(self, command: Line2) -> None:
         """Render line to target image."""
 
     def render_arc(self, command: Arc2) -> None:
         """Render arc to target image."""
 
@@ -83,16 +85,19 @@
 
     def render_flash_polygon(self, command: Flash2, aperture: Polygon2) -> None:
         """Render flash polygon to target image."""
 
     def render_flash_macro(self, command: Flash2, aperture: Macro2) -> None:
         """Render flash macro aperture to target image."""
 
-    def render_buffer(self, command: BufferCommand2) -> None:
+    def render_buffer(self, command: BufferCommand2) -> Generator[Command2, None, None]:
         """Render buffer command, performing no writes."""
+        for cmd in command:
+            cmd.render(self.renderer)
+            yield cmd
 
     def render_region(self, command: Region2) -> None:
         """Render region to target image."""
 
     def get_image_ref(self) -> ImageRef:
         """Get reference to render image."""
         raise NotImplementedError
```

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/renderer2/svg.py` & `pygerber-2.3.0/src/pygerber/gerberx3/renderer2/svg.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 """Module contains implementation of Gerber rendering backend outputting SVG files."""
+
 from __future__ import annotations
 
 import importlib.util
 from dataclasses import dataclass, field
 from decimal import Decimal
 from typing import BinaryIO, Optional
 
 from pygerber.backend.rasterized_2d.color_scheme import ColorScheme
 from pygerber.gerberx3.math.bounding_box import BoundingBox
 from pygerber.gerberx3.math.offset import Offset
 from pygerber.gerberx3.math.vector_2d import Vector2D
+from pygerber.gerberx3.parser2.apertures2.aperture2 import Aperture2
 from pygerber.gerberx3.parser2.apertures2.circle2 import Circle2, NoCircle2
 from pygerber.gerberx3.parser2.apertures2.macro2 import Macro2
 from pygerber.gerberx3.parser2.apertures2.obround2 import Obround2
 from pygerber.gerberx3.parser2.apertures2.polygon2 import Polygon2
 from pygerber.gerberx3.parser2.apertures2.rectangle2 import Rectangle2
 from pygerber.gerberx3.parser2.command_buffer2 import ReadonlyCommandBuffer2
 from pygerber.gerberx3.parser2.commands2.arc2 import Arc2, CCArc2
-from pygerber.gerberx3.parser2.commands2.buffer_command2 import BufferCommand2
 from pygerber.gerberx3.parser2.commands2.flash2 import Flash2
 from pygerber.gerberx3.parser2.commands2.line2 import Line2
 from pygerber.gerberx3.parser2.commands2.region2 import Region2
+from pygerber.gerberx3.parser2.state2 import ApertureTransform
 from pygerber.gerberx3.renderer2.abstract import (
     FormatOptions,
     ImageRef,
     Renderer2,
     Renderer2HooksABC,
 )
 from pygerber.gerberx3.renderer2.errors2 import DRAWSVGNotAvailableError
@@ -62,19 +64,28 @@
     class SvgRenderingFrame:
         """Rendering variable container."""
 
         command_buffer: ReadonlyCommandBuffer2
         bounding_box: BoundingBox
         normalize_origin_to_0_0: bool
         mask: drawsvg.Mask = field(default_factory=drawsvg.Mask)
-        layer: drawsvg.Group = field(default_factory=drawsvg.Group)
+        group: drawsvg.Group = field(default_factory=drawsvg.Group)
         polarity: Optional[Polarity] = None
         is_region: bool = False
         flip_y: bool = True
 
+        def get_group_or_mask(
+            self,
+            is_group: bool,  # noqa: FBT001
+        ) -> drawsvg.Group | drawsvg.Mask:
+            """Get group or mask."""
+            if is_group:
+                return self.group
+            return self.mask
+
 
 class SvgRenderer2Hooks(Renderer2HooksABC):
     """Rendering backend hooks used to render SVG images."""
 
     renderer: SvgRenderer2
 
     def __init__(
@@ -131,116 +142,173 @@
     def pop_render_frame(self) -> SvgRenderingFrame:
         """Pop segment render frame."""
         if len(self.rendering_stack) <= 1:
             raise RuntimeError
         return self.rendering_stack.pop()
 
     @property
-    def frame(self) -> SvgRenderingFrame:
+    def base_frame(self) -> SvgRenderingFrame:
+        """Get base rendering stack frame."""
+        return self.rendering_stack[0]
+
+    @property
+    def current_frame(self) -> SvgRenderingFrame:
         """Get current rendering stack frame."""
         return self.rendering_stack[-1]
 
-    def get_layer(self, polarity: Polarity) -> drawsvg.Group | drawsvg.Mask:
-        """Get image layer."""
-        if self.frame.polarity is None or polarity != self.frame.polarity:
-            self.frame.polarity = polarity
-            if polarity == Polarity.Dark:
-                self._new_layer(with_mask=False)
-            else:
-                self._new_layer(with_mask=True)
-
-        if self.frame.polarity == Polarity.Dark:
-            return self.frame.layer
+    def add_element_to_frame(
+        self,
+        polarity: Polarity,
+        element: drawsvg.DrawingBasicElement,
+    ) -> None:
+        """Add element to current frame."""
+        self.get_layer(polarity).append(element)
 
-        return self.frame.mask
+    def get_layer(self, polarity: Polarity) -> drawsvg.Group | drawsvg.Mask:
+        """Get SVG layer object corresponding to polarity."""
+        # In general what we want to do is to have a layer made of group with mask.
+        # First we fill the group with dark command, then after meeting first clear
+        # command we start filling mask with consecutive clear command until
+        # we meed dark command again. Then we create new group-mask layer to repeat the
+        # cycle.
+
+        # If frame is not initialized, initialize it.
+        if self.current_frame.polarity is None:
+            self.current_frame.polarity = polarity
+            self.add_masked_group_to_frame()
+
+            return self.current_frame.get_group_or_mask(polarity.is_solid())
+
+        if polarity.is_solid() != self.current_frame.polarity.is_solid():
+            # If polarity of frame is solid it means that mask for this group is still
+            # empty and can be filled.
+            if self.current_frame.polarity.is_solid():
+                self.current_frame.polarity = polarity
+                return self.current_frame.mask
+            # If polarity of frame is clear, it means that we already filled
+            # both group and mask and we need to create new group-mask layer.
+            self.add_masked_group_to_frame()
+            self.current_frame.polarity = polarity
+            return self.current_frame.group
+
+        # We have the same polarity as layer (and as previous commands) so we can
+        # simply add it to current layer.
+        return self.current_frame.get_group_or_mask(polarity.is_solid())
 
-    def _new_layer(self, *, with_mask: bool) -> None:
+    def add_masked_group_to_frame(self) -> None:
         """Create new layer including previous layer."""
-        if with_mask:
-            self.frame.mask = self._make_mask(self.frame.bounding_box)
-            new_layer = drawsvg.Group(mask=self.frame.mask)
-        else:
-            new_layer = drawsvg.Group()
-
-        new_layer.append(self.frame.layer)
+        self.current_frame.mask = self.create_full_mask()
+        new_layer = drawsvg.Group(mask=self.current_frame.mask)
+        new_layer.append(self.current_frame.group)
+        self.current_frame.group = new_layer
+
+    def create_full_mask(self) -> drawsvg.Mask:
+        """Create mask covering whole image."""
+        bbox = self.base_frame.bounding_box
+        mask = drawsvg.Mask()
+        mask.append(
+            drawsvg.Rectangle(
+                x=0,
+                y=0,
+                width=self.convert_size(bbox.width),
+                height=self.convert_size(bbox.height),
+                fill="white",
+            ),
+        )
+        return mask
 
-        self.frame.layer = new_layer
+    def create_mask(self, bbox: BoundingBox) -> drawsvg.Mask:
+        """Create mask covering specified bounding box."""
+        mask = drawsvg.Mask()
+        mask.append(
+            drawsvg.Rectangle(
+                x=self.convert_size(bbox.min_x),
+                y=self.convert_size(bbox.min_y),
+                width=self.convert_size(bbox.width),
+                height=self.convert_size(bbox.height),
+                fill="white",
+            ),
+        )
+        return mask
 
     def convert_x(self, x: Offset) -> Decimal:
         """Convert y offset to y coordinate in image space."""
-        if self.frame.normalize_origin_to_0_0:
-            origin_offset_x = self.frame.bounding_box.min_x.as_millimeters()
+        if self.current_frame.normalize_origin_to_0_0:
+            origin_offset_x = self.current_frame.bounding_box.min_x.as_millimeters()
         else:
             origin_offset_x = Decimal(0)
 
         corrected_position_x = x.as_millimeters() - origin_offset_x
 
         return corrected_position_x * self.scale
 
     def convert_y(self, y: Offset) -> Decimal:
         """Convert y offset to y coordinate in image space."""
         return self._convert_y(
             y,
-            normalize_origin_to_0_0=self.frame.normalize_origin_to_0_0,
-            flip_y=self.frame.flip_y,
+            normalize_origin_to_0_0=self.current_frame.normalize_origin_to_0_0,
+            flip_y=self.current_frame.flip_y,
         )
 
     def _convert_y(
         self,
         y: Offset,
         *,
         normalize_origin_to_0_0: bool,
         flip_y: bool,
     ) -> Decimal:
         """Convert y offset to pixel y coordinate."""
         if normalize_origin_to_0_0:
-            origin_offset_y = self.frame.bounding_box.min_y.as_millimeters()
+            origin_offset_y = self.current_frame.bounding_box.min_y.as_millimeters()
         else:
             origin_offset_y = Decimal(0)
 
         corrected_position_y = y.as_millimeters() - origin_offset_y
 
         if flip_y:
             flipped_position_y = (
-                self.frame.bounding_box.height.as_millimeters() - corrected_position_y
+                self.current_frame.bounding_box.height.as_millimeters()
+                - corrected_position_y
             )
             return flipped_position_y * self.scale
         return corrected_position_y * self.scale
 
     def convert_size(self, diameter: Offset) -> Decimal:
         """Convert y offset to pixel y coordinate."""
         return diameter.as_millimeters() * self.scale
 
     def get_color(self, polarity: Polarity) -> str:
         """Get color for specified polarity."""
-        if self.frame.is_region:
-            if polarity == Polarity.Dark:
+        if self.current_frame.is_region:
+            if polarity.is_solid():
                 return self.color_scheme.solid_region_color.to_hex()
             return "black"
 
-        if polarity == Polarity.Dark:
+        if polarity.is_solid():
             return self.color_scheme.solid_color.to_hex()
         return "black"
 
-    def get_aperture(self, aperture_id: int, color: str) -> Optional[drawsvg.Group]:
-        """Get SVG group representing aperture."""
-        return self.apertures.get(self._get_aperture_id(aperture_id, color))
+    def get_aperture_id(self, aperture: Aperture2, transform: ApertureTransform) -> str:
+        """Get unique ID for aperture."""
+        return (
+            f"{aperture.identifier}%"
+            f"{transform.get_transform_key()}%{transform.polarity}"
+        )
 
-    def _get_aperture_id(self, aperture_id: int, color: str) -> str:
-        """Return combined ID for listed aperture."""
-        return f"{color}+{aperture_id}"
+    def get_aperture(self, aperture_id: str) -> Optional[drawsvg.Group]:
+        """Get SVG group representing aperture."""
+        return self.apertures.get(aperture_id)
 
     def set_aperture(
         self,
-        aperture_id: int,
-        color: str,
+        aperture_id: str,
         aperture: drawsvg.Group,
     ) -> None:
         """Set SVG group representing aperture."""
-        self.apertures[self._get_aperture_id(aperture_id, color)] = aperture
+        self.apertures[aperture_id] = aperture
 
     def render_line(self, command: Line2) -> None:
         """Render line to target image."""
         color = self.get_color(command.transform.polarity)
 
         command.aperture.render_flash(
             self.renderer,
@@ -272,15 +340,15 @@
             self.convert_x(p2.x),
             self.convert_y(p2.y),
             self.convert_x(p3.x),
             self.convert_y(p3.y),
             fill=color,
             close=True,
         )
-        self.get_layer(command.transform.polarity).append(rectangle)
+        self.add_element_to_frame(command.transform.polarity, rectangle)
 
         command.aperture.render_flash(
             self.renderer,
             Flash2(
                 transform=command.transform,
                 attributes=command.attributes,
                 aperture=command.aperture,
@@ -385,15 +453,15 @@
                 center_point=command.center_point,
                 end_point=end_outer,
             ),
             arc_path,
         )
         # Close arc box by drawing line between end of outer arc and start of inner
         arc_path.Z()
-        self.get_layer(command.transform.polarity).append(arc_path)
+        self.add_element_to_frame(command.transform.polarity, arc_path)
 
         command.aperture.render_flash(
             self.renderer,
             Flash2(
                 transform=command.transform,
                 attributes=command.attributes,
                 aperture=command.aperture,
@@ -411,100 +479,109 @@
                 },
             ),
         )
 
     def render_flash_circle(self, command: Flash2, aperture: Circle2) -> None:
         """Render flash circle to target image."""
         color = self.get_color(command.transform.polarity)
-        aperture_group = self.get_aperture(id(aperture), color)
+        transform = command.transform
+        aperture_id = self.get_aperture_id(aperture, transform)
+        aperture_group = self.get_aperture(aperture_id)
 
         if aperture_group is None:
-            mask = self._make_mask(aperture.get_bounding_box(), aperture.hole_diameter)
-            aperture_group = drawsvg.Group(mask=mask)
+            aperture_group = self.create_group_for_aperture(
+                aperture.get_bounding_box(),
+                aperture.hole_diameter,
+            )
             aperture_group.append(
                 drawsvg.Circle(
                     cx=0,
                     cy=0,
                     r=self.convert_size(aperture.diameter) / Decimal("2.0"),
                     fill=color,
                 ),
             )
-            self.set_aperture(id(aperture), color, aperture_group)
+            self.set_aperture(aperture_id, aperture_group)
 
-        self.get_layer(command.transform.polarity).append(
+        self.add_element_to_frame(
+            command.transform.polarity,
             drawsvg.Use(
                 aperture_group,
                 x=self.convert_x(command.flash_point.x),
                 y=self.convert_y(command.flash_point.y),
             ),
         )
 
-    def _make_mask(
+    def create_group_for_aperture(
         self,
         bbox: BoundingBox,
-        hole_diameter: Optional[Offset] = None,
-    ) -> drawsvg.Mask:
-        mask = drawsvg.Mask()
-        mask.append(
-            drawsvg.Rectangle(
-                x=self.convert_size(bbox.min_x),
-                y=self.convert_size(bbox.min_y),
-                width=self.convert_size(bbox.width),
-                height=self.convert_size(bbox.height),
-                fill="white",
-            ),
+        hole_diameter: Optional[Offset],
+    ) -> drawsvg.Group:
+        """Create SVG group for aperture."""
+        if hole_diameter is None:
+            return drawsvg.Group()
+
+        mask = self.create_mask(bbox)
+        central_circle = drawsvg.Circle(
+            cx=0,
+            cy=0,
+            r=self.convert_size(hole_diameter) / 2,
+            fill="black",
         )
-        if hole_diameter is not None:
-            central_circle = drawsvg.Circle(
-                cx=0,
-                cy=0,
-                r=self.convert_size(hole_diameter) / 2,
-                fill="black",
-            )
-            mask.append(central_circle)
-        return mask
+        mask.append(central_circle)
+
+        return drawsvg.Group(mask=mask)
 
     def render_flash_no_circle(self, command: Flash2, aperture: NoCircle2) -> None:
         """Render flash no circle aperture to target image."""
 
     def render_flash_rectangle(self, command: Flash2, aperture: Rectangle2) -> None:
         """Render flash rectangle to target image."""
         color = self.get_color(command.transform.polarity)
-        aperture_group = self.get_aperture(id(aperture), color)
+        transform = command.transform
+        aperture_id = self.get_aperture_id(aperture, transform)
+        aperture_group = self.get_aperture(aperture_id)
 
         if aperture_group is None:
-            mask = self._make_mask(aperture.get_bounding_box(), aperture.hole_diameter)
-            aperture_group = drawsvg.Group(mask=mask)
+            aperture_group = self.create_group_for_aperture(
+                aperture.get_bounding_box(),
+                aperture.hole_diameter,
+            )
             aperture_group.append(
                 drawsvg.Rectangle(
                     -self.convert_size(aperture.x_size) / 2,
                     -self.convert_size(aperture.y_size) / 2,
                     self.convert_size(aperture.x_size),
                     self.convert_size(aperture.y_size),
                     fill=color,
                 ),
             )
-            self.set_aperture(id(aperture), color, aperture_group)
+            self.set_aperture(aperture_id, aperture_group)
 
-        self.get_layer(command.transform.polarity).append(
+        self.add_element_to_frame(
+            command.transform.polarity,
             drawsvg.Use(
                 aperture_group,
                 self.convert_x(command.flash_point.x),
                 self.convert_y(command.flash_point.y),
             ),
         )
 
     def render_flash_obround(self, command: Flash2, aperture: Obround2) -> None:
         """Render flash obround to target image."""
         color = self.get_color(command.transform.polarity)
-        aperture_group = self.get_aperture(id(aperture), color)
+        transform = command.transform
+        aperture_id = self.get_aperture_id(aperture, transform)
+        aperture_group = self.get_aperture(aperture_id)
 
         if aperture_group is None:
-            mask = self._make_mask(aperture.get_bounding_box(), aperture.hole_diameter)
-            aperture_group = drawsvg.Group(mask=mask)
+            aperture_group = self.create_group_for_aperture(
+                aperture.get_bounding_box(),
+                aperture.hole_diameter,
+            )
             x_size = self.convert_size(aperture.x_size)
             y_size = self.convert_size(aperture.y_size)
             radius = x_size.min(y_size) / Decimal("2.0")
 
             aperture_group.append(
                 drawsvg.Rectangle(
                     -self.convert_size(aperture.x_size) / 2,
@@ -512,32 +589,37 @@
                     x_size,
                     y_size,
                     fill=color,
                     rx=radius,
                     ry=radius,
                 ),
             )
-            self.set_aperture(id(aperture), color, aperture_group)
+            self.set_aperture(aperture_id, aperture_group)
 
-        self.get_layer(command.transform.polarity).append(
+        self.add_element_to_frame(
+            command.transform.polarity,
             drawsvg.Use(
                 aperture_group,
                 self.convert_x(command.flash_point.x),
                 self.convert_y(command.flash_point.y),
             ),
         )
 
     def render_flash_polygon(self, command: Flash2, aperture: Polygon2) -> None:
         """Render flash polygon to target image."""
         color = self.get_color(command.transform.polarity)
-        aperture_group = self.get_aperture(id(aperture), color)
+        transform = command.transform
+        aperture_id = self.get_aperture_id(aperture, transform)
+        aperture_group = self.get_aperture(aperture_id)
 
         if aperture_group is None:
-            mask = self._make_mask(aperture.get_bounding_box(), aperture.hole_diameter)
-            aperture_group = drawsvg.Group(mask=mask)
+            aperture_group = self.create_group_for_aperture(
+                aperture.get_bounding_box(),
+                aperture.hole_diameter,
+            )
 
             number_of_vertices = aperture.number_vertices
             initial_angle = aperture.rotation
             inner_angle = Decimal("360") / Decimal(number_of_vertices)
 
             radius_vector = Vector2D.UNIT_X * (aperture.outer_diameter / Decimal("2.0"))
             rotated_radius_vector = radius_vector.rotate_around_origin(initial_angle)
@@ -557,61 +639,59 @@
                     self.convert_size(rotated_radius_vector.x),
                     self.convert_size(rotated_radius_vector.y),
                 )
 
             p.Z()
 
             aperture_group.append(p)
-            self.set_aperture(id(aperture), color, aperture_group)
+            self.set_aperture(aperture_id, aperture_group)
 
-        self.get_layer(command.transform.polarity).append(
+        self.add_element_to_frame(
+            command.transform.polarity,
             drawsvg.Use(
                 aperture_group,
                 self.convert_x(command.flash_point.x),
                 self.convert_y(command.flash_point.y),
             ),
         )
 
     def render_flash_macro(self, command: Flash2, aperture: Macro2) -> None:
         """Render flash macro aperture to target image."""
-        color = self.get_color(command.transform.polarity)
-        aperture_group = self.get_aperture(id(aperture), color)
+        transform = command.transform
+        aperture_id = self.get_aperture_id(aperture, transform)
+        aperture_group = self.get_aperture(aperture_id)
 
         if aperture_group is None:
             self.push_render_frame(
                 aperture.command_buffer,
                 normalize_origin_to_0_0=False,
                 flip_y=False,
             )
             for cmd in aperture.command_buffer:
                 cmd.render(self.renderer)
 
             frame = self.pop_render_frame()
-            aperture_group = frame.layer
-            self.set_aperture(id(aperture), color, aperture_group)
+            aperture_group = frame.group
+            self.set_aperture(aperture_id, aperture_group)
 
-        self.get_layer(command.transform.polarity).append(
+        self.add_element_to_frame(
+            command.transform.polarity,
             drawsvg.Use(
                 aperture_group,
                 x=self.convert_x(command.flash_point.x),
                 y=self.convert_y(command.flash_point.y),
             ),
         )
 
-    def render_buffer(self, command: BufferCommand2) -> None:
-        """Render buffer command, performing no writes."""
-        for cmd in command:
-            cmd.render(self.renderer)
-
     def render_region(self, command: Region2) -> None:
         """Render region to target image."""
         if len(command.command_buffer) == 0:
             return
 
-        self.frame.is_region = True
+        self.current_frame.is_region = True
 
         color = self.get_color(command.transform.polarity)
         region = drawsvg.Path(fill=color)
 
         for cmd in command.command_buffer:
             if isinstance(cmd, (Line2, Arc2, CCArc2)):
                 region.M(
@@ -627,17 +707,17 @@
                 self.render_arc_to_path(cmd, region)
             elif isinstance(cmd, CCArc2):
                 self.render_cc_arc_to_path(cmd, region)
             else:
                 raise NotImplementedError
 
         region.Z()
-        self.get_layer(command.transform.polarity).append(region)
+        self.add_element_to_frame(command.transform.polarity, region)
 
-        self.frame.is_region = False
+        self.current_frame.is_region = False
 
     def render_line_to_path(self, command: Line2, path: drawsvg.Path) -> None:
         """Render line region boundary."""
         path.L(
             self.convert_x(command.end_point.x),
             self.convert_y(command.end_point.y),
         )
@@ -697,16 +777,16 @@
     def finalize(self) -> None:
         """Finalize rendering."""
         if len(self.rendering_stack) > 1:
             self.rendering_stack = [self.rendering_stack[0]]
         elif len(self.rendering_stack) < 1:
             raise RuntimeError
 
-        width = self.convert_size(self.frame.bounding_box.width)
-        height = self.convert_size(self.frame.bounding_box.height)
+        width = self.convert_size(self.current_frame.bounding_box.width)
+        height = self.convert_size(self.current_frame.bounding_box.height)
         self.drawing = drawsvg.Drawing(
             width=width,
             height=height,
         )
         self.drawing.append(self.get_layer(Polarity.Dark))
```

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/revisions.py` & `pygerber-2.3.0/src/pygerber/gerberx3/revisions.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/state_enums.py` & `pygerber-2.3.0/src/pygerber/gerberx3/state_enums.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """All state-defining enumerations."""
+
 from __future__ import annotations
 
 from pygerber.gerberx3.tokenizer.helpers.gerber_code_enum import GerberCodeEnum
 
 
 class DrawMode(GerberCodeEnum):
     """Drawing mode."""
@@ -63,14 +64,18 @@
         """Return region variant of polarity."""
         return _to_region_variant_map[self]
 
     def get_2d_rasterized_color(self) -> int:
         """Get color for "1" mode image."""
         return _2d_rasterized_color_map[self]
 
+    def is_solid(self) -> bool:
+        """Check if polarity represents solid surface."""
+        return _is_solid_map[self]
+
 
 _to_region_variant_map = {
     Polarity.Clear: Polarity.ClearRegion,
     Polarity.Dark: Polarity.DarkRegion,
 }
 
 _polarity_invert_map = {
@@ -90,14 +95,24 @@
     Polarity.DarkRegion: 230,
     Polarity.ClearRegion: 30,
     Polarity.Background: 0,
     Polarity.DEBUG: 127,
     Polarity.DEBUG2: 75,
 }
 
+_is_solid_map = {
+    Polarity.Clear: False,
+    Polarity.Dark: True,
+    Polarity.ClearRegion: False,
+    Polarity.DarkRegion: True,
+    Polarity.Background: True,
+    Polarity.DEBUG: True,
+    Polarity.DEBUG2: True,
+}
+
 
 class Mirroring(GerberCodeEnum):
     """Aperture mirroring."""
 
     NoMirroring = "N"
     XY = "XY"
     X = "X"
```

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/aperture_id.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/aperture_id.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/decorators.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/decorators.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/grammar.ebnf` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/grammar.ebnf`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/grammar.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/grammar.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """GerberX3 grammar."""
+
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Any, Optional, Type, TypeVar
 
 from pyparsing import (
     CharsNotIn,
@@ -883,37 +884,38 @@
     def _build_attribute_tokens(self, *, statement: bool = False) -> ParserElement:
         wrapper = self.wrapper
 
         file_attribute_name = self._build_name().set_name("file attribute name")
         aperture_attribute_name = self._build_name().set_name("aperture attribute name")
         object_attribute_name = self._build_name().set_name("object attribute name")
 
+        comma = Literal(",")
+        comma_with_field = comma + self._build_field()
+        maybe_comma_or_maybe_comma_with_field = Opt(comma_with_field | comma)
+
         # Set a file attribute.
         tf = wrapper(
             self.options.tf_file_attribute_token_cls,
             Literal("TF")
             + file_attribute_name.set_results_name("attribute_name")
-            + Literal(",")
-            + Opt(self._build_field()),
+            + maybe_comma_or_maybe_comma_with_field,
         )
         # Add an aperture attribute to the dictionary or modify it.
         ta = wrapper(
             self.options.ta_aperture_attribute_token_cls,
             Literal("TA")
             + aperture_attribute_name.set_results_name("attribute_name")
-            + Literal(",")
-            + Opt(self._build_field()),
+            + maybe_comma_or_maybe_comma_with_field,
         )
         # Add an object attribute to the dictionary or modify it.
         to = wrapper(
             self.options.to_object_attribute_token_cls,
             Literal("TO")
             + object_attribute_name.set_results_name("attribute_name")
-            + Literal(",")
-            + Opt(self._build_field()),
+            + maybe_comma_or_maybe_comma_with_field,
         )
         # Delete one or all attributes in the dictionary.
         td = wrapper(
             self.options.td_delete_attribute_token_cls,
             Literal("TD")
             + Opt(
                 file_attribute_name | aperture_attribute_name | object_attribute_name,
```

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokenizer.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokenizer.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/ab_block_aperture.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/ab_block_aperture.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/ad_define_aperture.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/ad_define_aperture.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/as_axis_select.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/as_axis_select.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/attribute_token.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/attribute_token.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/bases/command.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/bases/command.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/bases/extended_command.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/bases/extended_command.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/bases/gerber_code.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/bases/gerber_code.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/bases/group.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/bases/group.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/bases/token.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/bases/token.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/bases/token_accessor.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/bases/token_accessor.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/coordinate.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/coordinate.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/d01_draw.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/d01_draw.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/d02_move.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/d02_move.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/d03_flash.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/d03_flash.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/dnn_select_aperture.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/dnn_select_aperture.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/end_of_expression.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/end_of_expression.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/fs_coordinate_format.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/fs_coordinate_format.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/g01_set_linear.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/g01_set_linear.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/g02_set_clockwise_circular.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/g02_set_clockwise_circular.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/g03_set_counterclockwise_circular.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/g03_set_counterclockwise_circular.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/g04_comment.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/g04_comment.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/g36_begin_region.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/g36_begin_region.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/g37_end_region.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/g37_end_region.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/g54_select_aperture.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/g54_select_aperture.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/g70_set_unit_inch.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/g70_set_unit_inch.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/g71_set_unit_mm.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/g71_set_unit_mm.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/g74_single_quadrant.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/g74_single_quadrant.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/g75_multi_quadrant.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/g75_multi_quadrant.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/g90_set_coordinate_absolute.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/g90_set_coordinate_absolute.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/g91_set_coordinate_incremental.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/g91_set_coordinate_incremental.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/groups/statement.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/groups/statement.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/in_image_name.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/in_image_name.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/invalid_token.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/invalid_token.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/ip_image_polarity.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/ip_image_polarity.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/lm_load_mirroring.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/lm_load_mirroring.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/ln_load_name.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/ln_load_name.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/lp_load_polarity.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/lp_load_polarity.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/lr_load_rotation.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/lr_load_rotation.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/ls_load_scaling.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/ls_load_scaling.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/m00_program_stop.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/m00_program_stop.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/m01_optional_stop.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/m01_optional_stop.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/m02_end_of_file.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/m02_end_of_file.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/macro/__init__.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/__init__.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/macro/am_macro.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/am_macro.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/binary.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/binary.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/macro_expression.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/macro_expression.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/numeric_constant.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/numeric_constant.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/unary.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/unary.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/variable_name.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/variable_name.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/macro/macro_begin.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/macro_begin.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/macro/point.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/point.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_1_circle.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_1_circle.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_20_vector_line.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_20_vector_line.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_21_center_line.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_21_center_line.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_22_lower_left_line.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_22_lower_left_line.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_2_vector_line.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_2_vector_line.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_4_outline.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_4_outline.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_5_polygon.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_5_polygon.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_6_moire.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_6_moire.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_7_thermal.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_7_thermal.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/comment.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/comment.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/statement.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/statement.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/variable_assignment.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/variable_assignment.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/mo_unit_mode.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/mo_unit_mode.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/of_image_offset.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/of_image_offset.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/sr_step_repeat.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/sr_step_repeat.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/ta_aperture_attribute.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/ta_aperture_attribute.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Comment token."""
 
-
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from pygerber.gerberx3.tokenizer.tokens.attribute_token import (
     SetAttributeToken,
 )
@@ -35,11 +34,12 @@
 
     def get_gerber_code(
         self,
         indent: str = "",  # noqa: ARG002
         endline: str = "\n",  # noqa: ARG002
     ) -> str:
         """Get gerber code represented by this token."""
-        return f"TA{self.name},{self.value}"
+        value = f",{self.value}" if self.value else ""
+        return f"TA{self.name}{value}"
 
     def __str__(self) -> str:
         return f"{super().__str__()}::[{self.name} -> {self.value}]"
```

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/td_delete_attribute.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/td_delete_attribute.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Comment token."""
 
-
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Optional
 
 from pygerber.gerberx3.tokenizer.tokens.attribute_token import AttributeToken
 
 if TYPE_CHECKING:
@@ -51,11 +50,12 @@
 
     def get_gerber_code(
         self,
         indent: str = "",  # noqa: ARG002
         endline: str = "\n",  # noqa: ARG002
     ) -> str:
         """Get gerber code represented by this token."""
-        return f"TD{self.name if self.name is not None else ''}"
+        name = self.name if self.name is not None else ""
+        return f"TD{name}"
 
     def __str__(self) -> str:
         return f"{super().__str__()}::[{self.name}]"
```

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/tf_file_attribute.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/tf_file_attribute.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Comment token."""
 
-
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from pygerber.gerberx3.tokenizer.tokens.attribute_token import (
     SetAttributeToken,
 )
@@ -31,11 +30,12 @@
 
     def get_gerber_code(
         self,
         indent: str = "",  # noqa: ARG002
         endline: str = "\n",  # noqa: ARG002
     ) -> str:
         """Get gerber code represented by this token."""
-        return f"TF{self.name},{self.value}"
+        value = f",{self.value}" if self.value else ""
+        return f"TF{self.name}{value}"
 
     def __str__(self) -> str:
         return f"{super().__str__()}::[{self.name} -> {self.value}]"
```

### Comparing `pygerber-2.2.1/src/pygerber/gerberx3/tokenizer/tokens/to_object_attribute.py` & `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/to_object_attribute.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,11 +33,12 @@
 
     def get_gerber_code(
         self,
         indent: str = "",  # noqa: ARG002
         endline: str = "\n",  # noqa: ARG002
     ) -> str:
         """Get gerber code represented by this token."""
-        return f"TO{self.name},{self.value}"
+        value = f",{self.value}" if self.value else ""
+        return f"TO{self.name}{value}"
 
     def __str__(self) -> str:
         return f"{super().__str__()}::[{self.name} -> {self.value}]"
```

### Comparing `pygerber-2.2.1/src/pygerber/sequence_tools.py` & `pygerber-2.3.0/src/pygerber/sequence_tools.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.2.1/PKG-INFO` & `pygerber-2.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygerber
-Version: 2.2.1
+Version: 2.3.0
 Summary: Parsing, formatting and rendering toolkit for Gerber X3 file format
 Home-page: https://www.facebook.com/pygerber
 License: MIT
 Keywords: gerber,pcb,embedded,images,x3
 Author: Krzysztof Wisniewski
 Author-email: argmaster.world@gmail.com
 Requires-Python: >=3.8,<3.13
@@ -168,142 +168,135 @@
 pygerber raster-2d gerber-source.grb
 ```
 
 Image will be saved to `output.png` in current working directory.
 
 ![example_pcb_image](https://github.com/Argmaster/pygerber/assets/56170852/9bca28bf-8aa6-4215-aac1-62c386490485)
 
-## API usage
+## Programmatic usage
 
-PyGerber offers a high-level API that simplifies the process of rendering Gerber files.
-Whether you're looking to save the rendered output to a file or directly into a buffer,
-PyGerber has got you covered.
-
-- **The `Layer` Class**: At its core, the `Layer` class stands for a single Gerber
-  source file, complete with its associated PyGerber configuration.
-
-  **Important** `Layer` class represents **any** Gerber file, **not** layer of PCB. For
-  example, silkscreen Gerber file will require one instance of `Layer`, paste mask will
-  require another one, copper top yet another, etc.
-
-- **Configuration Flexibility**: The configuration possibilities you get with a `Layer`
-  are driven by the backend you choose to render your source file.
-
-- **Selecting a Backend**: PyGerber provides specialized subclasses of the `Layer` class
-  each tied to one rendering backend. For instance, if you're aiming for 2D rasterized
-  images, `Rasterized2DLayer` is your go-to choice.
-
-- **Output Types**: Keep in mind, the type of your output file is closely tied to the
-  backend you select.For 2D rasterized rendering
-  [all formats supported by Pillow](https://pillow.readthedocs.io/en/stable/handbook/image-file-formats.html)
-  are accepted.
-
-### Rasterized render from file
-
-```py linenums="1" title="render_file.py"
-from pygerber.gerberx3.api import (
-      ColorScheme,
-      Rasterized2DLayer,
-      Rasterized2DLayerParams,
-)
+### JPG
 
-# Path to Gerber source file.
-source_path = "main_cu.grb"
+PyGerber can be used programmatically to render Gerber files. Below is an minimalistic
+example of how to render one of the example files included with PyGerber release to JPEG
+image:
 
-Rasterized2DLayer(
-      options=Rasterized2DLayerParams(
-            source_path=source_path,
-            colors=ColorScheme.COPPER_ALPHA,
-      ),
-).render().save("output.png")
-```
-
-Example code above creates `Rasterized2DLayer` object, renders it with rasterized 2D
-backend and saves it as `PNG` image. Use of `Rasterized2DLayer` and
-`Rasterized2DLayerOptions` classes implicitly use 2D rasterized backend. To use
-different rendering backend with high level API, user must pick different `Layer` and
-`LayerOptions` subclasses. For other backends see
-[Target set of tools](#target-set-of-tools) section, note that only checked ones are
-available.
-
-`source_path` option accepts `str` or `Path` pointing to local Gerber file. No special
-file extension is required, content is blindly loaded from specified file, so it's user
-responsibility to provide correct path. There are also `source_code` and `source_buffer`
-parameters which allow for use of raw `str` or `bytes` objects (first one) and
-`StringIO` and `BytesIO` or file descriptors (second one). `source_code`,
-`source_buffer` and `source_path` are mutually exclusive.
-
-`ColorScheme` is a class which describes what colors should be used for rendering
-different parts of image. Additionally it has a few static members which contain
-predefined colors schemes for frequently used layer types. It is not required to use
-predefined schemes, creating and passing custom `ColorScheme` object should work
-perfectly fine.
-
-Pattern of using `<Class>` and `<Class>Options`, like above, is used in many places in
-PyGerber. When initializing object like `Rasterized2DLayer` it is only valid to pass
-`Rasterized2DLayerOptions` to constructor. Passing `LayerOptions` or `Vectorized2DLayer`
-will cause undefined behavior, most likely yielding no result or raising exception.
-
-### Rasterized render from string
-
-```py linenums="1" title="render_string.py"
-from pygerber.gerberx3.api import (
-      ColorScheme,
-      Rasterized2DLayer,
-      Rasterized2DLayerParams,
-)
+```python
+from pygerber.examples import ExamplesEnum, get_example_path
+from pygerber.gerberx3.api.v2 import GerberFile
+
+GerberFile.from_file(
+    get_example_path(ExamplesEnum.UCAMCO_ex_2_Shapes),
+).parse().render_raster("output.jpg")
+```
+
+Running code above will create `output.jpg` file in current working directory which
+should look like this:
+
+<p align="center">
+  <img height="400" src="https://github.com/Argmaster/pygerber/assets/56170852/d17ebee8-e851-4c86-b110-8cd8aeca993e">
+</p>
+
+### PNG
 
-source_code = """
-%FSLAX26Y26*%
-%MOMM*%
-%ADD100R,1.5X1.0X0.5*%
-%ADD200C,1.5X1.0*%
-%ADD300O,1.5X1.0X0.6*%
-%ADD400P,1.5X3X5.0*%
-D100*
-X0Y0D03*
-D200*
-X0Y2000000D03*
-D300*
-X2000000Y0D03*
-D400*
-X2000000Y2000000D03*
-M02*
-"""
-
-Rasterized2DLayer(
-      options=Rasterized2DLayerParams(
-            source_code=source_code,
-            colors=ColorScheme.SILK,
-            dpi=3000,
-      ),
-).render().save("output.png")
+It is also possible to render Gerber files to PNG with custom resolution and different
+color schemes:
 
+```python
+from pygerber.examples import ExamplesEnum, get_example_path
+from pygerber.gerberx3.api.v2 import ColorScheme, GerberFile, PixelFormatEnum
+
+GerberFile.from_file(
+    get_example_path(ExamplesEnum.ShapeFlashes),
+).parse().render_raster(
+    "output.png",
+    dpmm=100,
+    color_scheme=ColorScheme.COPPER_ALPHA,
+    pixel_format=PixelFormatEnum.RGBA,
+)
 ```
 
 Code above renders following image:
 
 <p align="center">
-  <img width="414" height="384" src="https://github.com/Argmaster/pygerber/assets/56170852/56b6757b-0f97-4a18-9d43-f21711c71c71">
+  <img height="400" src="https://github.com/Argmaster/pygerber/assets/56170852/0a5a42f3-8792-4b9a-be61-bac12f0e1c03">
 </p>
 
+### SVG
+
+Finally you can also create SVG files with PyGerber:
+
+```python
+from pygerber.examples import ExamplesEnum, load_example
+from pygerber.gerberx3.api.v2 import GerberFile
+
+source_code = load_example(ExamplesEnum.UCAMCO_ex_2_Shapes)
+GerberFile.from_str(source_code).parse().render_svg("output.svg")
+
+```
+
+### Multiple layers
+
+PyGerber can also render multiple layers to single image. Below is an example of how to
+render four layers to single PNG image with use of `Project` class:
+
+```python
+from pygerber.examples import ExamplesEnum, load_example
+from pygerber.gerberx3.api.v2 import FileTypeEnum, GerberFile, Project
+
+Project(
+    [
+        GerberFile.from_str(
+            load_example(ExamplesEnum.simple_2layer_F_Cu),
+            FileTypeEnum.COPPER,
+        ),
+        GerberFile.from_str(
+            load_example(ExamplesEnum.simple_2layer_F_Mask),
+            FileTypeEnum.MASK,
+        ),
+        GerberFile.from_str(
+            load_example(ExamplesEnum.simple_2layer_F_Paste),
+            FileTypeEnum.PASTE,
+        ),
+        GerberFile.from_str(
+            load_example(ExamplesEnum.simple_2layer_F_Silkscreen),
+            FileTypeEnum.SILK,
+        ),
+    ],
+).parse().render_raster("output.png", dpmm=40)
+```
+
+Here is the result:
+
+<p align="center">
+  <img width="400" src="https://github.com/Argmaster/pygerber/assets/56170852/9b3f3823-67b3-49f1-8c76-e2bddaca81fe">
+</p>
+
+### Advanced usage
+
+Additionally to examples presented above which use high level API, PyGerber provides low
+level API which allows to directly access PyGerber internals and change behavior of
+parser, tokenizer and renderers. This can be used for code introspection and potentially
+other purposed. Check out documentation for more information.
+
 ## Documentation
 
 Official documentations is hosted on Github Pages and can be found
 [here](https://argmaster.github.io/pygerber/latest).
 
 ## Gerber features support
 
 Please refer to documentation for
 
 - [Tokenizer](https://argmaster.github.io/pygerber/latest/gerber/feature_support/tokenizer.html),
 - [Parser](https://argmaster.github.io/pygerber/latest/gerber/feature_support/parser.html),
 - [Rasterized2DBackend](https://argmaster.github.io/pygerber/latest/gerber/feature_support/rasterized_2d.html),
 - [Parser2](https://argmaster.github.io/pygerber/latest/gerber/feature_support/parser2.html),
 - [SvgRenderer2](https://argmaster.github.io/pygerber/latest/gerber/feature_support/svgrenderer2.html),
+- [RasterRenderer2](https://argmaster.github.io/pygerber/latest/gerber/feature_support/rasterrenderer2.html),
 
 for detailed list of features which are supported/not supported by each tool.
 
 ## Syntax feature requests
 
 All deprecated features (Mainly those from X2 format) are considered optional and
 priority to implement them will be assigned based on number of requests form community.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pygerber Version: 2.2.1 Summary: Parsing,
+Metadata-Version: 2.1 Name: pygerber Version: 2.3.0 Summary: Parsing,
 formatting and rendering toolkit for Gerber X3 file format Home-page: https://
 www.facebook.com/pygerber License: MIT Keywords: gerber,pcb,embedded,images,x3
 Author: Krzysztof Wisniewski Author-email: argmaster.world@gmail.com Requires-
 Python: >=3.8,<3.13 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop Classifier: Intended
 Audience :: Information Technology Classifier: Intended Audience ::
@@ -77,77 +77,67 @@
 similar to one below **â©**, where `x.y.z` should match version of PyGerber
 installed. ``` $ pygerber --version pygerber, version x.y.z ``` Use `--help` to
 display help messages with lists of subcommands and subcommand options: ```
 pygerber raster-2d --help ``` To render 2D PNG image of some gerber file you
 can simply use: ``` pygerber raster-2d gerber-source.grb ``` Image will be
 saved to `output.png` in current working directory. ![example_pcb_image](https:
 //github.com/Argmaster/pygerber/assets/56170852/9bca28bf-8aa6-4215-aac1-
-62c386490485) ## API usage PyGerber offers a high-level API that simplifies the
-process of rendering Gerber files. Whether you're looking to save the rendered
-output to a file or directly into a buffer, PyGerber has got you covered. -
-**The `Layer` Class**: At its core, the `Layer` class stands for a single
-Gerber source file, complete with its associated PyGerber configuration.
-**Important** `Layer` class represents **any** Gerber file, **not** layer of
-PCB. For example, silkscreen Gerber file will require one instance of `Layer`,
-paste mask will require another one, copper top yet another, etc. -
-**Configuration Flexibility**: The configuration possibilities you get with a
-`Layer` are driven by the backend you choose to render your source file. -
-**Selecting a Backend**: PyGerber provides specialized subclasses of the
-`Layer` class each tied to one rendering backend. For instance, if you're
-aiming for 2D rasterized images, `Rasterized2DLayer` is your go-to choice. -
-**Output Types**: Keep in mind, the type of your output file is closely tied to
-the backend you select.For 2D rasterized rendering [all formats supported by
-Pillow](https://pillow.readthedocs.io/en/stable/handbook/image-file-
-formats.html) are accepted. ### Rasterized render from file ```py linenums="1"
-title="render_file.py" from pygerber.gerberx3.api import ( ColorScheme,
-Rasterized2DLayer, Rasterized2DLayerParams, ) # Path to Gerber source file.
-source_path = "main_cu.grb" Rasterized2DLayer( options=Rasterized2DLayerParams
-( source_path=source_path, colors=ColorScheme.COPPER_ALPHA, ), ).render().save
-("output.png") ``` Example code above creates `Rasterized2DLayer` object,
-renders it with rasterized 2D backend and saves it as `PNG` image. Use of
-`Rasterized2DLayer` and `Rasterized2DLayerOptions` classes implicitly use 2D
-rasterized backend. To use different rendering backend with high level API,
-user must pick different `Layer` and `LayerOptions` subclasses. For other
-backends see [Target set of tools](#target-set-of-tools) section, note that
-only checked ones are available. `source_path` option accepts `str` or `Path`
-pointing to local Gerber file. No special file extension is required, content
-is blindly loaded from specified file, so it's user responsibility to provide
-correct path. There are also `source_code` and `source_buffer` parameters which
-allow for use of raw `str` or `bytes` objects (first one) and `StringIO` and
-`BytesIO` or file descriptors (second one). `source_code`, `source_buffer` and
-`source_path` are mutually exclusive. `ColorScheme` is a class which describes
-what colors should be used for rendering different parts of image. Additionally
-it has a few static members which contain predefined colors schemes for
-frequently used layer types. It is not required to use predefined schemes,
-creating and passing custom `ColorScheme` object should work perfectly fine.
-Pattern of using `` and `Options`, like above, is used in many places in
-PyGerber. When initializing object like `Rasterized2DLayer` it is only valid to
-pass `Rasterized2DLayerOptions` to constructor. Passing `LayerOptions` or
-`Vectorized2DLayer` will cause undefined behavior, most likely yielding no
-result or raising exception. ### Rasterized render from string ```py
-linenums="1" title="render_string.py" from pygerber.gerberx3.api import
-( ColorScheme, Rasterized2DLayer, Rasterized2DLayerParams, ) source_code = """
-%FSLAX26Y26*% %MOMM*% %ADD100R,1.5X1.0X0.5*% %ADD200C,1.5X1.0*%
-%ADD300O,1.5X1.0X0.6*% %ADD400P,1.5X3X5.0*% D100* X0Y0D03* D200* X0Y2000000D03*
-D300* X2000000Y0D03* D400* X2000000Y2000000D03* M02* """ Rasterized2DLayer
-( options=Rasterized2DLayerParams( source_code=source_code,
-colors=ColorScheme.SILK, dpi=3000, ), ).render().save("output.png") ``` Code
-above renders following image:
-[https://github.com/Argmaster/pygerber/assets/56170852/56b6757b-0f97-4a18-9d43-
-                                 f21711c71c71]
-## Documentation Official documentations is hosted on Github Pages and can be
-found [here](https://argmaster.github.io/pygerber/latest). ## Gerber features
-support Please refer to documentation for - [Tokenizer](https://
-argmaster.github.io/pygerber/latest/gerber/feature_support/tokenizer.html), -
-[Parser](https://argmaster.github.io/pygerber/latest/gerber/feature_support/
-parser.html), - [Rasterized2DBackend](https://argmaster.github.io/pygerber/
-latest/gerber/feature_support/rasterized_2d.html), - [Parser2](https://
-argmaster.github.io/pygerber/latest/gerber/feature_support/parser2.html), -
-[SvgRenderer2](https://argmaster.github.io/pygerber/latest/gerber/
-feature_support/svgrenderer2.html), for detailed list of features which are
+62c386490485) ## Programmatic usage ### JPG PyGerber can be used
+programmatically to render Gerber files. Below is an minimalistic example of
+how to render one of the example files included with PyGerber release to JPEG
+image: ```python from pygerber.examples import ExamplesEnum, get_example_path
+from pygerber.gerberx3.api.v2 import GerberFile GerberFile.from_file
+( get_example_path(ExamplesEnum.UCAMCO_ex_2_Shapes), ).parse().render_raster
+("output.jpg") ``` Running code above will create `output.jpg` file in current
+working directory which should look like this:
+[https://github.com/Argmaster/pygerber/assets/56170852/d17ebee8-e851-4c86-b110-
+                                 8cd8aeca993e]
+### PNG It is also possible to render Gerber files to PNG with custom
+resolution and different color schemes: ```python from pygerber.examples import
+ExamplesEnum, get_example_path from pygerber.gerberx3.api.v2 import
+ColorScheme, GerberFile, PixelFormatEnum GerberFile.from_file( get_example_path
+(ExamplesEnum.ShapeFlashes), ).parse().render_raster( "output.png", dpmm=100,
+color_scheme=ColorScheme.COPPER_ALPHA, pixel_format=PixelFormatEnum.RGBA, ) ```
+Code above renders following image:
+[https://github.com/Argmaster/pygerber/assets/56170852/0a5a42f3-8792-4b9a-be61-
+                                 bac12f0e1c03]
+### SVG Finally you can also create SVG files with PyGerber: ```python from
+pygerber.examples import ExamplesEnum, load_example from
+pygerber.gerberx3.api.v2 import GerberFile source_code = load_example
+(ExamplesEnum.UCAMCO_ex_2_Shapes) GerberFile.from_str(source_code).parse
+().render_svg("output.svg") ``` ### Multiple layers PyGerber can also render
+multiple layers to single image. Below is an example of how to render four
+layers to single PNG image with use of `Project` class: ```python from
+pygerber.examples import ExamplesEnum, load_example from
+pygerber.gerberx3.api.v2 import FileTypeEnum, GerberFile, Project Project(
+[ GerberFile.from_str( load_example(ExamplesEnum.simple_2layer_F_Cu),
+FileTypeEnum.COPPER, ), GerberFile.from_str( load_example
+(ExamplesEnum.simple_2layer_F_Mask), FileTypeEnum.MASK, ), GerberFile.from_str
+( load_example(ExamplesEnum.simple_2layer_F_Paste), FileTypeEnum.PASTE, ),
+GerberFile.from_str( load_example(ExamplesEnum.simple_2layer_F_Silkscreen),
+FileTypeEnum.SILK, ), ], ).parse().render_raster("output.png", dpmm=40) ```
+Here is the result:
+[https://github.com/Argmaster/pygerber/assets/56170852/9b3f3823-67b3-49f1-8c76-
+                                 e2bddaca81fe]
+### Advanced usage Additionally to examples presented above which use high
+level API, PyGerber provides low level API which allows to directly access
+PyGerber internals and change behavior of parser, tokenizer and renderers. This
+can be used for code introspection and potentially other purposed. Check out
+documentation for more information. ## Documentation Official documentations is
+hosted on Github Pages and can be found [here](https://argmaster.github.io/
+pygerber/latest). ## Gerber features support Please refer to documentation for
+- [Tokenizer](https://argmaster.github.io/pygerber/latest/gerber/
+feature_support/tokenizer.html), - [Parser](https://argmaster.github.io/
+pygerber/latest/gerber/feature_support/parser.html), - [Rasterized2DBackend]
+(https://argmaster.github.io/pygerber/latest/gerber/feature_support/
+rasterized_2d.html), - [Parser2](https://argmaster.github.io/pygerber/latest/
+gerber/feature_support/parser2.html), - [SvgRenderer2](https://
+argmaster.github.io/pygerber/latest/gerber/feature_support/svgrenderer2.html),
+- [RasterRenderer2](https://argmaster.github.io/pygerber/latest/gerber/
+feature_support/rasterrenderer2.html), for detailed list of features which are
 supported/not supported by each tool. ## Syntax feature requests All deprecated
 features (Mainly those from X2 format) are considered optional and priority to
 implement them will be assigned based on number of requests form community. If
 You needs support for syntax features which are not mentioned in `The Gerber
 Layer Format Specification. Revision 2023.08` (Available on [Ucamco's webpage]
 (https://www.ucamco.com/files/downloads/file_en/456/gerber-layer-format-
 specification-revision-2023-08_en.pdf) and in [this repository](https://
```

