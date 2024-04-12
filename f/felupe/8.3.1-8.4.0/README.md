# Comparing `tmp/felupe-8.3.1.tar.gz` & `tmp/felupe-8.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "felupe-8.3.1.tar", last modified: Sat Apr  6 21:27:46 2024, max compression
+gzip compressed data, was "felupe-8.4.0.tar", last modified: Fri Apr 12 12:09:25 2024, max compression
```

## Comparing `felupe-8.3.1.tar` & `felupe-8.4.0.tar`

### file list

```diff
@@ -1,143 +1,145 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:27:46.487674 felupe-8.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35081 2024-04-06 21:27:42.000000 felupe-8.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    55811 2024-04-06 21:27:46.487674 felupe-8.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12855 2024-04-06 21:27:42.000000 felupe-8.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-06 21:27:42.000000 felupe-8.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 21:27:46.487674 felupe-8.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:27:46.463674 felupe-8.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:27:46.467674 felupe-8.3.1/src/felupe/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:27:46.467674 felupe-8.3.1/src/felupe/assembly/
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/assembly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9292 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/assembly/_axi.py
--rw-r--r--   0 runner    (1001) docker     (127)     7316 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/assembly/_cartesian.py
--rw-r--r--   0 runner    (1001) docker     (127)     9937 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/assembly/_integral.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:27:46.467674 felupe-8.3.1/src/felupe/assembly/expression/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/assembly/expression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/assembly/expression/_basis.py
--rw-r--r--   0 runner    (1001) docker     (127)     4790 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/assembly/expression/_bilinear.py
--rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/assembly/expression/_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/assembly/expression/_expression.py
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/assembly/expression/_linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/assembly/expression/_mixed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:27:46.471674 felupe-8.3.1/src/felupe/constitution/
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/constitution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7133 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/constitution/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6327 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/constitution/_kinematics.py
--rw-r--r--   0 runner    (1001) docker     (127)    24929 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/constitution/_mixed.py
--rw-r--r--   0 runner    (1001) docker     (127)    17741 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/constitution/_models_hyperelasticity.py
--rw-r--r--   0 runner    (1001) docker     (127)    16167 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/constitution/_models_hyperelasticity_ad.py
--rw-r--r--   0 runner    (1001) docker     (127)    18221 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/constitution/_models_linear_elasticity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/constitution/_models_linear_elasticity_large_strain.py
--rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/constitution/_models_pseudo_elasticity.py
--rw-r--r--   0 runner    (1001) docker     (127)    17580 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/constitution/_user_materials.py
--rw-r--r--   0 runner    (1001) docker     (127)    12214 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/constitution/_user_materials_hyperelastic.py
--rw-r--r--   0 runner    (1001) docker     (127)     7556 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/constitution/_user_materials_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    18055 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/constitution/_view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:27:46.471674 felupe-8.3.1/src/felupe/dof/
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/dof/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8920 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/dof/_boundary.py
--rw-r--r--   0 runner    (1001) docker     (127)    20346 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/dof/_loadcase.py
--rw-r--r--   0 runner    (1001) docker     (127)     7373 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/dof/_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:27:46.471674 felupe-8.3.1/src/felupe/element/
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/element/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4460 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/element/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    18387 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/element/_hexahedron.py
--rw-r--r--   0 runner    (1001) docker     (127)    11420 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/element/_lagrange.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/element/_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/element/_quad.py
--rw-r--r--   0 runner    (1001) docker     (127)     7853 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/element/_tetra.py
--rw-r--r--   0 runner    (1001) docker     (127)     6797 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/element/_triangle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:27:46.475674 felupe-8.3.1/src/felupe/field/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/field/_axi.py
--rw-r--r--   0 runner    (1001) docker     (127)    12182 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/field/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11297 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/field/_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/field/_dual.py
--rw-r--r--   0 runner    (1001) docker     (127)     5861 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/field/_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/field/_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/field/_indices.py
--rw-r--r--   0 runner    (1001) docker     (127)     5761 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/field/_planestrain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:27:46.475674 felupe-8.3.1/src/felupe/math/
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/math/_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/math/_math.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/math/_spatial.py
--rw-r--r--   0 runner    (1001) docker     (127)    45047 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/math/_tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:27:46.475674 felupe-8.3.1/src/felupe/mechanics/
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/mechanics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8210 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/mechanics/_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/mechanics/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/mechanics/_item.py
--rw-r--r--   0 runner    (1001) docker     (127)    12227 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/mechanics/_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     7056 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/mechanics/_multipoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/mechanics/_pointload.py
--rw-r--r--   0 runner    (1001) docker     (127)    11473 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/mechanics/_solidbody.py
--rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/mechanics/_solidbody_gravity.py
--rw-r--r--   0 runner    (1001) docker     (127)    18763 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/mechanics/_solidbody_incompressible.py
--rw-r--r--   0 runner    (1001) docker     (127)     5007 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/mechanics/_solidbody_pressure.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/mechanics/_step.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:27:46.479674 felupe-8.3.1/src/felupe/mesh/
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/mesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9944 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/mesh/_container.py
--rw-r--r--   0 runner    (1001) docker     (127)    17192 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/mesh/_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     5577 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/mesh/_discrete_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/mesh/_dual.py
--rw-r--r--   0 runner    (1001) docker     (127)    15620 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/mesh/_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/mesh/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/mesh/_line_rectangle_cube.py
--rw-r--r--   0 runner    (1001) docker     (127)    48808 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/mesh/_mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/mesh/_read.py
--rw-r--r--   0 runner    (1001) docker     (127)    32323 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/mesh/_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:27:46.479674 felupe-8.3.1/src/felupe/quadrature/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/quadrature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7233 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/quadrature/_gausslegendre.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/quadrature/_scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/quadrature/_sphere.py
--rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/quadrature/_tetra.py
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/quadrature/_triangle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:27:46.479674 felupe-8.3.1/src/felupe/region/
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/region/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14750 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/region/_boundary.py
--rw-r--r--   0 runner    (1001) docker     (127)    10703 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/region/_region.py
--rw-r--r--   0 runner    (1001) docker     (127)    19319 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/region/_templates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:27:46.479674 felupe-8.3.1/src/felupe/solve/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/solve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/solve/_solve.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:27:46.483674 felupe-8.3.1/src/felupe/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/tools/_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    13311 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/tools/_newton.py
--rw-r--r--   0 runner    (1001) docker     (127)    20214 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/tools/_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/tools/_post.py
--rw-r--r--   0 runner    (1001) docker     (127)    14006 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/tools/_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/tools/_save.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-06 21:27:42.000000 felupe-8.3.1/src/felupe/tools/_solve.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:27:46.487674 felupe-8.3.1/src/felupe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    55811 2024-04-06 21:27:46.000000 felupe-8.3.1/src/felupe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-04-06 21:27:46.000000 felupe-8.3.1/src/felupe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 21:27:46.000000 felupe-8.3.1/src/felupe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-06 21:27:46.000000 felupe-8.3.1/src/felupe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-06 21:27:46.000000 felupe-8.3.1/src/felupe.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:27:46.487674 felupe-8.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-06 21:27:42.000000 felupe-8.3.1/tests/test_basis.py
--rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-04-06 21:27:42.000000 felupe-8.3.1/tests/test_bilinearform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3794 2024-04-06 21:27:42.000000 felupe-8.3.1/tests/test_composite.py
--rw-r--r--   0 runner    (1001) docker     (127)    15877 2024-04-06 21:27:42.000000 felupe-8.3.1/tests/test_constitution.py
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-04-06 21:27:42.000000 felupe-8.3.1/tests/test_dof.py
--rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-04-06 21:27:42.000000 felupe-8.3.1/tests/test_element.py
--rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-04-06 21:27:42.000000 felupe-8.3.1/tests/test_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     8348 2024-04-06 21:27:42.000000 felupe-8.3.1/tests/test_form.py
--rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-04-06 21:27:42.000000 felupe-8.3.1/tests/test_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-04-06 21:27:42.000000 felupe-8.3.1/tests/test_math.py
--rw-r--r--   0 runner    (1001) docker     (127)    15767 2024-04-06 21:27:42.000000 felupe-8.3.1/tests/test_mechanics.py
--rw-r--r--   0 runner    (1001) docker     (127)    15972 2024-04-06 21:27:42.000000 felupe-8.3.1/tests/test_mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     7771 2024-04-06 21:27:42.000000 felupe-8.3.1/tests/test_mpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-04-06 21:27:42.000000 felupe-8.3.1/tests/test_planestrain.py
--rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-04-06 21:27:42.000000 felupe-8.3.1/tests/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-04-06 21:27:42.000000 felupe-8.3.1/tests/test_quadrature.py
--rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-04-06 21:27:42.000000 felupe-8.3.1/tests/test_readme.py
--rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-04-06 21:27:42.000000 felupe-8.3.1/tests/test_region.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-06 21:27:42.000000 felupe-8.3.1/tests/test_solve.py
--rw-r--r--   0 runner    (1001) docker     (127)    16175 2024-04-06 21:27:42.000000 felupe-8.3.1/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:09:25.886152 felupe-8.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35081 2024-04-12 12:09:18.000000 felupe-8.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    55811 2024-04-12 12:09:25.886152 felupe-8.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12855 2024-04-12 12:09:18.000000 felupe-8.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-12 12:09:18.000000 felupe-8.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 12:09:25.886152 felupe-8.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:09:25.858152 felupe-8.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:09:25.858152 felupe-8.4.0/src/felupe/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:09:25.862152 felupe-8.4.0/src/felupe/assembly/
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/assembly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9292 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/assembly/_axi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7316 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/assembly/_cartesian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9937 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/assembly/_integral.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:09:25.862152 felupe-8.4.0/src/felupe/assembly/expression/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/assembly/expression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/assembly/expression/_basis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4790 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/assembly/expression/_bilinear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/assembly/expression/_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/assembly/expression/_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/assembly/expression/_linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/assembly/expression/_mixed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:09:25.866152 felupe-8.4.0/src/felupe/constitution/
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/constitution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7133 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/constitution/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6327 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/constitution/_kinematics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24929 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/constitution/_mixed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17741 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/constitution/_models_hyperelasticity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16167 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/constitution/_models_hyperelasticity_ad.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18221 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/constitution/_models_linear_elasticity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/constitution/_models_linear_elasticity_large_strain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/constitution/_models_pseudo_elasticity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17580 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/constitution/_user_materials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12214 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/constitution/_user_materials_hyperelastic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7556 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/constitution/_user_materials_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18040 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/constitution/_view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:09:25.866152 felupe-8.4.0/src/felupe/dof/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/dof/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8920 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/dof/_boundary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20346 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/dof/_loadcase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7373 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/dof/_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:09:25.866152 felupe-8.4.0/src/felupe/element/
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/element/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4460 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/element/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18387 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/element/_hexahedron.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11420 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/element/_lagrange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/element/_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/element/_quad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7853 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/element/_tetra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6797 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/element/_triangle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:09:25.870152 felupe-8.4.0/src/felupe/field/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/field/_axi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12182 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/field/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11297 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/field/_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/field/_dual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5861 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/field/_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/field/_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/field/_indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5761 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/field/_planestrain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:09:25.870152 felupe-8.4.0/src/felupe/math/
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/math/_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/math/_math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/math/_solve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/math/_spatial.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45047 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/math/_tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:09:25.874152 felupe-8.4.0/src/felupe/mechanics/
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/mechanics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8496 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/mechanics/_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/mechanics/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/mechanics/_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12227 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/mechanics/_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7056 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/mechanics/_multipoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/mechanics/_pointload.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11473 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/mechanics/_solidbody.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/mechanics/_solidbody_gravity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18763 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/mechanics/_solidbody_incompressible.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5007 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/mechanics/_solidbody_pressure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/mechanics/_step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:09:25.874152 felupe-8.4.0/src/felupe/mesh/
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/mesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9944 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/mesh/_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17192 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/mesh/_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5577 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/mesh/_discrete_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/mesh/_dual.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15620 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/mesh/_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/mesh/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/mesh/_line_rectangle_cube.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48808 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/mesh/_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/mesh/_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32323 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/mesh/_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:09:25.878152 felupe-8.4.0/src/felupe/quadrature/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/quadrature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7233 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/quadrature/_gausslegendre.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/quadrature/_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/quadrature/_sphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/quadrature/_tetra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/quadrature/_triangle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:09:25.878152 felupe-8.4.0/src/felupe/region/
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/region/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14750 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/region/_boundary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10703 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/region/_region.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19319 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/region/_templates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:09:25.878152 felupe-8.4.0/src/felupe/solve/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/solve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/solve/_solve.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:09:25.878152 felupe-8.4.0/src/felupe/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/tools/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13311 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/tools/_newton.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20261 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/tools/_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/tools/_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14006 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/tools/_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/tools/_save.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/tools/_solve.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:09:25.882152 felupe-8.4.0/src/felupe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    55811 2024-04-12 12:09:25.000000 felupe-8.4.0/src/felupe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-04-12 12:09:25.000000 felupe-8.4.0/src/felupe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:09:25.000000 felupe-8.4.0/src/felupe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-12 12:09:25.000000 felupe-8.4.0/src/felupe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 12:09:25.000000 felupe-8.4.0/src/felupe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:09:25.882152 felupe-8.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-12 12:09:18.000000 felupe-8.4.0/tests/test_basis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-04-12 12:09:18.000000 felupe-8.4.0/tests/test_bilinearform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3794 2024-04-12 12:09:18.000000 felupe-8.4.0/tests/test_composite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15877 2024-04-12 12:09:18.000000 felupe-8.4.0/tests/test_constitution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-12 12:09:18.000000 felupe-8.4.0/tests/test_constitution_newton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-04-12 12:09:18.000000 felupe-8.4.0/tests/test_dof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-04-12 12:09:18.000000 felupe-8.4.0/tests/test_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-04-12 12:09:18.000000 felupe-8.4.0/tests/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8348 2024-04-12 12:09:18.000000 felupe-8.4.0/tests/test_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-04-12 12:09:18.000000 felupe-8.4.0/tests/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-04-12 12:09:18.000000 felupe-8.4.0/tests/test_math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15767 2024-04-12 12:09:18.000000 felupe-8.4.0/tests/test_mechanics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15972 2024-04-12 12:09:18.000000 felupe-8.4.0/tests/test_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7771 2024-04-12 12:09:18.000000 felupe-8.4.0/tests/test_mpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-04-12 12:09:18.000000 felupe-8.4.0/tests/test_planestrain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-04-12 12:09:18.000000 felupe-8.4.0/tests/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-04-12 12:09:18.000000 felupe-8.4.0/tests/test_quadrature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-04-12 12:09:18.000000 felupe-8.4.0/tests/test_readme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-04-12 12:09:18.000000 felupe-8.4.0/tests/test_region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-12 12:09:18.000000 felupe-8.4.0/tests/test_solve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16175 2024-04-12 12:09:18.000000 felupe-8.4.0/tests/test_tools.py
```

### Comparing `felupe-8.3.1/LICENSE` & `felupe-8.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/PKG-INFO` & `felupe-8.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: felupe
-Version: 8.3.1
+Version: 8.4.0
 Summary: Finite Element Analysis
 Author: Andreas Dutzler
 Author-email: a.dutzler@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `felupe-8.3.1/README.md` & `felupe-8.4.0/README.md`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/pyproject.toml` & `felupe-8.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/__init__.py` & `felupe-8.4.0/src/felupe/__init__.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/assembly/_axi.py` & `felupe-8.4.0/src/felupe/assembly/_axi.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/assembly/_cartesian.py` & `felupe-8.4.0/src/felupe/assembly/_cartesian.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/assembly/_integral.py` & `felupe-8.4.0/src/felupe/assembly/_integral.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/assembly/expression/_basis.py` & `felupe-8.4.0/src/felupe/assembly/expression/_basis.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/assembly/expression/_bilinear.py` & `felupe-8.4.0/src/felupe/assembly/expression/_bilinear.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/assembly/expression/_decorator.py` & `felupe-8.4.0/src/felupe/assembly/expression/_decorator.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/assembly/expression/_expression.py` & `felupe-8.4.0/src/felupe/assembly/expression/_expression.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/assembly/expression/_linear.py` & `felupe-8.4.0/src/felupe/assembly/expression/_linear.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/assembly/expression/_mixed.py` & `felupe-8.4.0/src/felupe/assembly/expression/_mixed.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/constitution/__init__.py` & `felupe-8.4.0/src/felupe/constitution/__init__.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/constitution/_base.py` & `felupe-8.4.0/src/felupe/constitution/_base.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/constitution/_kinematics.py` & `felupe-8.4.0/src/felupe/constitution/_kinematics.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/constitution/_mixed.py` & `felupe-8.4.0/src/felupe/constitution/_mixed.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/constitution/_models_hyperelasticity.py` & `felupe-8.4.0/src/felupe/constitution/_models_hyperelasticity.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/constitution/_models_hyperelasticity_ad.py` & `felupe-8.4.0/src/felupe/constitution/_models_hyperelasticity_ad.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/constitution/_models_linear_elasticity.py` & `felupe-8.4.0/src/felupe/constitution/_models_linear_elasticity.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/constitution/_models_linear_elasticity_large_strain.py` & `felupe-8.4.0/src/felupe/constitution/_models_linear_elasticity_large_strain.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/constitution/_models_pseudo_elasticity.py` & `felupe-8.4.0/src/felupe/constitution/_models_pseudo_elasticity.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/constitution/_user_materials.py` & `felupe-8.4.0/src/felupe/constitution/_user_materials.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/constitution/_user_materials_hyperelastic.py` & `felupe-8.4.0/src/felupe/constitution/_user_materials_hyperelastic.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/constitution/_user_materials_models.py` & `felupe-8.4.0/src/felupe/constitution/_user_materials_models.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/constitution/_view.py` & `felupe-8.4.0/src/felupe/constitution/_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,20 +88,19 @@
                 if callable(fun):
                     label = [name.title() for name in fun.__name__.split("_")]
                 title += " (" + " ".join(label) + ")"
             fig.suptitle(title)
 
         if show_kwargs:
             if hasattr(self.umat, "kwargs"):
-                ax.set_title(
-                    ", ".join(
-                        [f"{key}={value}" for key, value in self.umat.kwargs.items()]
-                    ),
-                    fontdict=dict(fontsize="small"),
+                parameters = ", ".join(
+                    [f"{key}={value}" for key, value in self.umat.kwargs.items()]
                 )
+                ax.set_title(parameters, fontdict=dict(fontsize="small"), wrap=True)
+
         return ax
 
 
 class ViewMaterial(PlotMaterial):
     """Create views on normal force per undeformed area vs. stretch curves for the
     elementary homogeneous deformations uniaxial tension/compression, planar shear and
     biaxial tension of a given isotropic material formulation.
```

### Comparing `felupe-8.3.1/src/felupe/dof/_boundary.py` & `felupe-8.4.0/src/felupe/dof/_boundary.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/dof/_loadcase.py` & `felupe-8.4.0/src/felupe/dof/_loadcase.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/dof/_tools.py` & `felupe-8.4.0/src/felupe/dof/_tools.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/element/__init__.py` & `felupe-8.4.0/src/felupe/element/__init__.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/element/_base.py` & `felupe-8.4.0/src/felupe/element/_base.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/element/_hexahedron.py` & `felupe-8.4.0/src/felupe/element/_hexahedron.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/element/_lagrange.py` & `felupe-8.4.0/src/felupe/element/_lagrange.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/element/_line.py` & `felupe-8.4.0/src/felupe/element/_line.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/element/_quad.py` & `felupe-8.4.0/src/felupe/element/_quad.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/element/_tetra.py` & `felupe-8.4.0/src/felupe/element/_tetra.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/element/_triangle.py` & `felupe-8.4.0/src/felupe/element/_triangle.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/field/_axi.py` & `felupe-8.4.0/src/felupe/field/_axi.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/field/_base.py` & `felupe-8.4.0/src/felupe/field/_base.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/field/_container.py` & `felupe-8.4.0/src/felupe/field/_container.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/field/_dual.py` & `felupe-8.4.0/src/felupe/field/_dual.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/field/_evaluate.py` & `felupe-8.4.0/src/felupe/field/_evaluate.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/field/_fields.py` & `felupe-8.4.0/src/felupe/field/_fields.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/field/_indices.py` & `felupe-8.4.0/src/felupe/field/_indices.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/field/_planestrain.py` & `felupe-8.4.0/src/felupe/field/_planestrain.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/math/__init__.py` & `felupe-8.4.0/src/felupe/math/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     interpolate,
     norm,
     strain,
     strain_stretch_1d,
     values,
 )
 from ._math import linsteps
+from ._solve import solve_2d
 from ._spatial import rotation_matrix
 from ._tensor import (
     cdya,
     cdya_ik,
     cdya_il,
     cof,
     cross,
@@ -73,8 +74,9 @@
     "majortranspose",
     "ravel",
     "reshape",
     "sym",
     "tovoigt",
     "trace",
     "transpose",
+    "solve_2d",
 ]
```

### Comparing `felupe-8.3.1/src/felupe/math/_field.py` & `felupe-8.4.0/src/felupe/math/_field.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/math/_math.py` & `felupe-8.4.0/src/felupe/math/_math.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/math/_spatial.py` & `felupe-8.4.0/src/felupe/math/_spatial.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/math/_tensor.py` & `felupe-8.4.0/src/felupe/math/_tensor.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/mechanics/__init__.py` & `felupe-8.4.0/src/felupe/mechanics/__init__.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/mechanics/_curve.py` & `felupe-8.4.0/src/felupe/mechanics/_curve.py`

 * *Files 4% similar despite different names*

```diff
@@ -118,14 +118,16 @@
         y=None,
         xaxis=0,
         yaxis=0,
         xlabel=None,
         ylabel=None,
         xscale=1.0,
         yscale=1.0,
+        xoffset=0.0,
+        yoffset=0.0,
         gradient=False,
         swapaxes=False,
         ax=None,
         items=None,
         **kwargs,
     ):
         """Plot force-displacement characteristic curves on a pre-evaluated job,
@@ -150,14 +152,18 @@
             The label of the x-axis (default is None).
         ylabel : str or None, optional
             The label of the y-axis (default is None).
         xscale : float, optional
             A scaling factor for the displacement data (default is 1.0).
         yscale : float, optional
             A scaling factor the reaction force data (default is 1.0).
+        xoffset : float, optional
+            An offset for the displacement data (default is 0.0).
+        yoffset : float, optional
+            An offset for the reaction force data (default is 0.0).
         gradient : bool, optional
             A flag to plot the gradient of the y-data. Uses
             ``numpy.gradient(edge_order=2)``. The gradient data is set to ``np.nan`` for
             absolute values greater than the mean value plus two times the standard
             deviation. Default is False.
         swapaxes : bool, optional
             A flag to flip the plot (x, y) to (y, x). Also changes the labels.
@@ -209,15 +215,17 @@
 
         if swapaxes:
             x, y = y, x
             xlabel, ylabel = ylabel, xlabel
             xaxis, yaxis = yaxis, xaxis
             xscale, yscale = yscale, xscale
 
-        ax.plot(x[:, xaxis] * xscale, y[:, yaxis] * yscale, **kwargs)
+        ax.plot(
+            xoffset + x[:, xaxis] * xscale, yoffset + y[:, yaxis] * yscale, **kwargs
+        )
 
         if xlabel is not None:
             ax.set_xlabel(xlabel)
 
         if ylabel is not None:
             ax.set_ylabel(ylabel)
```

### Comparing `felupe-8.3.1/src/felupe/mechanics/_helpers.py` & `felupe-8.4.0/src/felupe/mechanics/_helpers.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/mechanics/_item.py` & `felupe-8.4.0/src/felupe/mechanics/_item.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/mechanics/_job.py` & `felupe-8.4.0/src/felupe/mechanics/_job.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/mechanics/_multipoint.py` & `felupe-8.4.0/src/felupe/mechanics/_multipoint.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/mechanics/_pointload.py` & `felupe-8.4.0/src/felupe/mechanics/_pointload.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/mechanics/_solidbody.py` & `felupe-8.4.0/src/felupe/mechanics/_solidbody.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/mechanics/_solidbody_gravity.py` & `felupe-8.4.0/src/felupe/mechanics/_solidbody_gravity.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/mechanics/_solidbody_incompressible.py` & `felupe-8.4.0/src/felupe/mechanics/_solidbody_incompressible.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/mechanics/_solidbody_pressure.py` & `felupe-8.4.0/src/felupe/mechanics/_solidbody_pressure.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/mechanics/_step.py` & `felupe-8.4.0/src/felupe/mechanics/_step.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/mesh/__init__.py` & `felupe-8.4.0/src/felupe/mesh/__init__.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/mesh/_container.py` & `felupe-8.4.0/src/felupe/mesh/_container.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/mesh/_convert.py` & `felupe-8.4.0/src/felupe/mesh/_convert.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/mesh/_discrete_geometry.py` & `felupe-8.4.0/src/felupe/mesh/_discrete_geometry.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/mesh/_dual.py` & `felupe-8.4.0/src/felupe/mesh/_dual.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/mesh/_geometry.py` & `felupe-8.4.0/src/felupe/mesh/_geometry.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/mesh/_helpers.py` & `felupe-8.4.0/src/felupe/mesh/_helpers.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/mesh/_line_rectangle_cube.py` & `felupe-8.4.0/src/felupe/mesh/_line_rectangle_cube.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/mesh/_mesh.py` & `felupe-8.4.0/src/felupe/mesh/_mesh.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/mesh/_read.py` & `felupe-8.4.0/src/felupe/mesh/_read.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/mesh/_tools.py` & `felupe-8.4.0/src/felupe/mesh/_tools.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/quadrature/_gausslegendre.py` & `felupe-8.4.0/src/felupe/quadrature/_gausslegendre.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/quadrature/_scheme.py` & `felupe-8.4.0/src/felupe/quadrature/_scheme.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/quadrature/_sphere.py` & `felupe-8.4.0/src/felupe/quadrature/_sphere.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/quadrature/_tetra.py` & `felupe-8.4.0/src/felupe/quadrature/_tetra.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/quadrature/_triangle.py` & `felupe-8.4.0/src/felupe/quadrature/_triangle.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/region/__init__.py` & `felupe-8.4.0/src/felupe/region/__init__.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/region/_boundary.py` & `felupe-8.4.0/src/felupe/region/_boundary.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/region/_region.py` & `felupe-8.4.0/src/felupe/region/_region.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/region/_templates.py` & `felupe-8.4.0/src/felupe/region/_templates.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/solve/_solve.py` & `felupe-8.4.0/src/felupe/solve/_solve.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/tools/__init__.py` & `felupe-8.4.0/src/felupe/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/tools/_misc.py` & `felupe-8.4.0/src/felupe/tools/_misc.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/tools/_newton.py` & `felupe-8.4.0/src/felupe/tools/_newton.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/tools/_plot.py` & `felupe-8.4.0/src/felupe/tools/_plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,14 +183,15 @@
                         "ZX",
                         "ZY",
                         "ZZ",
                     ],
                 }
 
                 if "Principal Values of " in data_label:
+                    data[:] = np.flip(np.sort(data, axis=-1), axis=-1)
                     component_labels_dict[2] = [
                         "(Max. Principal)",
                         "(Min. Principal)",
                     ]
                     component_labels_dict[3] = [
                         "(Max. Principal)",
                         "(Int. Principal)",
@@ -430,27 +431,27 @@
                 .T,
                 "Logarithmic Strain": field.evaluate.strain(tensor=True, asvoigt=True)
                 .mean(-2)
                 .T,
                 "Principal Values of Logarithmic Strain": field.evaluate.strain(
                     tensor=False
                 )
-                .mean(-2)[::-1]
+                .mean(-2)
                 .T,
             }
         elif callable(project):
             point_data_from_field = {
                 "Deformation Gradient": project(
                     field.evaluate.deformation_gradient(), field.region
                 ),
                 "Logarithmic Strain": project(
                     field.evaluate.strain(tensor=True, asvoigt=True), field.region
                 ),
                 "Principal Values of Logarithmic Strain": project(
-                    field.evaluate.strain(tensor=False)[::-1], field.region
+                    field.evaluate.strain(tensor=False), field.region
                 ),
             }
         else:
             raise TypeError("The project-argument must be callable or None.")
 
         point_data_from_field["Displacement"] = displacement(field)
 
@@ -534,26 +535,26 @@
             }
             stress = stress_from_field[stress_type.lower()](field)
             stress_label = f"{stress_type.title()} Stress"
 
             if project is None:
                 cell_data_from_solid[stress_label] = tovoigt(stress.mean(-2)).T
                 cell_data_from_solid[f"Principal Values of {stress_label}"] = (
-                    eigvalsh(stress).mean(-2)[::-1].T
+                    eigvalsh(stress).mean(-2).T
                 )
                 cell_data_from_solid[f"Equivalent of {stress_label}"] = (
                     equivalent_von_mises(stress).mean(-2).T
                 )
 
             elif callable(project):
                 point_data_from_solid[stress_label] = project(
                     tovoigt(stress), solid.field.region
                 )
                 point_data_from_solid[f"Principal Values of {stress_label}"] = project(
-                    eigvalsh(stress)[::-1], solid.field.region
+                    eigvalsh(stress), solid.field.region
                 )
                 point_data_from_solid[f"Equivalent of {stress_label}"] = project(
                     equivalent_von_mises(stress), solid.field.region
                 )
             else:
                 raise TypeError("The project-argument must be callable or None.")
```

### Comparing `felupe-8.3.1/src/felupe/tools/_post.py` & `felupe-8.4.0/src/felupe/tools/_post.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/tools/_project.py` & `felupe-8.4.0/src/felupe/tools/_project.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/tools/_save.py` & `felupe-8.4.0/src/felupe/tools/_save.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe/tools/_solve.py` & `felupe-8.4.0/src/felupe/tools/_solve.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/src/felupe.egg-info/PKG-INFO` & `felupe-8.4.0/src/felupe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: felupe
-Version: 8.3.1
+Version: 8.4.0
 Summary: Finite Element Analysis
 Author: Andreas Dutzler
 Author-email: a.dutzler@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `felupe-8.3.1/src/felupe.egg-info/SOURCES.txt` & `felupe-8.4.0/src/felupe.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 src/felupe/field/_evaluate.py
 src/felupe/field/_fields.py
 src/felupe/field/_indices.py
 src/felupe/field/_planestrain.py
 src/felupe/math/__init__.py
 src/felupe/math/_field.py
 src/felupe/math/_math.py
+src/felupe/math/_solve.py
 src/felupe/math/_spatial.py
 src/felupe/math/_tensor.py
 src/felupe/mechanics/__init__.py
 src/felupe/mechanics/_curve.py
 src/felupe/mechanics/_helpers.py
 src/felupe/mechanics/_item.py
 src/felupe/mechanics/_job.py
@@ -101,14 +102,15 @@
 src/felupe/tools/_project.py
 src/felupe/tools/_save.py
 src/felupe/tools/_solve.py
 tests/test_basis.py
 tests/test_bilinearform.py
 tests/test_composite.py
 tests/test_constitution.py
+tests/test_constitution_newton.py
 tests/test_dof.py
 tests/test_element.py
 tests/test_field.py
 tests/test_form.py
 tests/test_job.py
 tests/test_math.py
 tests/test_mechanics.py
```

### Comparing `felupe-8.3.1/tests/test_basis.py` & `felupe-8.4.0/tests/test_basis.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/tests/test_bilinearform.py` & `felupe-8.4.0/tests/test_bilinearform.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/tests/test_composite.py` & `felupe-8.4.0/tests/test_composite.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/tests/test_constitution.py` & `felupe-8.4.0/tests/test_constitution.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/tests/test_dof.py` & `felupe-8.4.0/tests/test_dof.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/tests/test_element.py` & `felupe-8.4.0/tests/test_element.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/tests/test_field.py` & `felupe-8.4.0/tests/test_field.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/tests/test_form.py` & `felupe-8.4.0/tests/test_form.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/tests/test_job.py` & `felupe-8.4.0/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/tests/test_math.py` & `felupe-8.4.0/tests/test_math.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/tests/test_mechanics.py` & `felupe-8.4.0/tests/test_mechanics.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/tests/test_mesh.py` & `felupe-8.4.0/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/tests/test_mpc.py` & `felupe-8.4.0/tests/test_mpc.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/tests/test_planestrain.py` & `felupe-8.4.0/tests/test_planestrain.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/tests/test_plot.py` & `felupe-8.4.0/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/tests/test_quadrature.py` & `felupe-8.4.0/tests/test_quadrature.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/tests/test_readme.py` & `felupe-8.4.0/tests/test_readme.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/tests/test_region.py` & `felupe-8.4.0/tests/test_region.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/tests/test_solve.py` & `felupe-8.4.0/tests/test_solve.py`

 * *Files identical despite different names*

### Comparing `felupe-8.3.1/tests/test_tools.py` & `felupe-8.4.0/tests/test_tools.py`

 * *Files identical despite different names*

