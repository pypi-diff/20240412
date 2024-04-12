# Comparing `tmp/fast_gauss-0.0.5.tar.gz` & `tmp/fast_gauss-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_gauss-0.0.5.tar", last modified: Tue Apr  9 15:59:33 2024, max compression
+gzip compressed data, was "fast_gauss-0.0.6.tar", last modified: Fri Apr 12 07:52:37 2024, max compression
```

## Comparing `fast_gauss-0.0.5.tar` & `fast_gauss-0.0.6.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:59:33.273899 fast_gauss-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     6504 2024-04-09 15:59:33.273899 fast_gauss-0.0.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:59:33.273899 fast_gauss-0.0.5/fast_gauss/
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-09 15:59:25.000000 fast_gauss-0.0.5/fast_gauss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26098 2024-04-09 15:59:25.000000 fast_gauss-0.0.5/fast_gauss/console_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-09 15:59:25.000000 fast_gauss-0.0.5/fast_gauss/cuda_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    19045 2024-04-09 15:59:25.000000 fast_gauss-0.0.5/fast_gauss/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11276 2024-04-09 15:59:25.000000 fast_gauss-0.0.5/fast_gauss/egl_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-09 15:59:25.000000 fast_gauss-0.0.5/fast_gauss/gaussian_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-04-09 15:59:25.000000 fast_gauss-0.0.5/fast_gauss/gl_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17533 2024-04-09 15:59:25.000000 fast_gauss-0.0.5/fast_gauss/gsplat_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6687 2024-04-09 15:59:25.000000 fast_gauss-0.0.5/fast_gauss/math_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10858 2024-04-09 15:59:25.000000 fast_gauss-0.0.5/fast_gauss/sh_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:59:33.273899 fast_gauss-0.0.5/fast_gauss/shaders/
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-09 15:59:25.000000 fast_gauss-0.0.5/fast_gauss/shaders/gsplat.frag
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-09 15:59:25.000000 fast_gauss-0.0.5/fast_gauss/shaders/gsplat.geom
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-09 15:59:25.000000 fast_gauss-0.0.5/fast_gauss/shaders/gsplat.vert
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:59:33.273899 fast_gauss-0.0.5/fast_gauss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6504 2024-04-09 15:59:33.000000 fast_gauss-0.0.5/fast_gauss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-09 15:59:33.000000 fast_gauss-0.0.5/fast_gauss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 15:59:33.000000 fast_gauss-0.0.5/fast_gauss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-09 15:59:33.000000 fast_gauss-0.0.5/fast_gauss.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-09 15:59:33.000000 fast_gauss-0.0.5/fast_gauss.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-09 15:59:25.000000 fast_gauss-0.0.5/license
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-09 15:59:25.000000 fast_gauss-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-04-09 15:59:25.000000 fast_gauss-0.0.5/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 15:59:25.000000 fast_gauss-0.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 15:59:33.273899 fast_gauss-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:52:37.731333 fast_gauss-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     9690 2024-04-12 07:52:37.731333 fast_gauss-0.0.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:52:37.731333 fast_gauss-0.0.6/fast_gauss/
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-12 07:52:28.000000 fast_gauss-0.0.6/fast_gauss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-04-12 07:52:28.000000 fast_gauss-0.0.6/fast_gauss/base_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26294 2024-04-12 07:52:28.000000 fast_gauss-0.0.6/fast_gauss/console_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-12 07:52:28.000000 fast_gauss-0.0.6/fast_gauss/cuda_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19045 2024-04-12 07:52:28.000000 fast_gauss-0.0.6/fast_gauss/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11276 2024-04-12 07:52:28.000000 fast_gauss-0.0.6/fast_gauss/egl_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-12 07:52:28.000000 fast_gauss-0.0.6/fast_gauss/gaussian_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-04-12 07:52:28.000000 fast_gauss-0.0.6/fast_gauss/gl_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18994 2024-04-12 07:52:28.000000 fast_gauss-0.0.6/fast_gauss/gsplat_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6687 2024-04-12 07:52:28.000000 fast_gauss-0.0.6/fast_gauss/math_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10858 2024-04-12 07:52:28.000000 fast_gauss-0.0.6/fast_gauss/sh_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:52:37.731333 fast_gauss-0.0.6/fast_gauss/shaders/
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-12 07:52:28.000000 fast_gauss-0.0.6/fast_gauss/shaders/gsplat.frag
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-12 07:52:28.000000 fast_gauss-0.0.6/fast_gauss/shaders/gsplat.geom
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-12 07:52:28.000000 fast_gauss-0.0.6/fast_gauss/shaders/gsplat.vert
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:52:37.731333 fast_gauss-0.0.6/fast_gauss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9690 2024-04-12 07:52:37.000000 fast_gauss-0.0.6/fast_gauss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-12 07:52:37.000000 fast_gauss-0.0.6/fast_gauss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 07:52:37.000000 fast_gauss-0.0.6/fast_gauss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-12 07:52:37.000000 fast_gauss-0.0.6/fast_gauss.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-12 07:52:37.000000 fast_gauss-0.0.6/fast_gauss.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-12 07:52:28.000000 fast_gauss-0.0.6/license
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-12 07:52:28.000000 fast_gauss-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     8215 2024-04-12 07:52:28.000000 fast_gauss-0.0.6/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 07:52:28.000000 fast_gauss-0.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 07:52:37.731333 fast_gauss-0.0.6/setup.cfg
```

### Comparing `fast_gauss-0.0.5/PKG-INFO` & `fast_gauss-0.0.6/readme.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,59 +1,36 @@
-Metadata-Version: 2.1
-Name: fast_gauss
-Version: 0.0.5
-Summary: CUDA global sort + CUDA-GL interop + geometry shader quad emitting + hardware rasterization + CUDA-GL interop = fast gaussian splatting
-Author: Zhen Xu
-Author-email: zhenx@zju.edu.cn
-License: Copyright 2022-2023 3D Vision Group at the State Key Lab of CAD&CG,  
-        Zhejiang University. All Rights Reserved. 
-        
-        For more information see <https://github.com/dendenxu/fast-gaussian-splatting> 
-        If you use this software, please cite the corresponding publications   
-        listed on the above website. 
-        
-        Permission to use, copy, modify and distribute this software and its 
-        documentation for educational, research and non-profit purposes only. 
-        Any modification based on this work must be open-source and prohibited 
-        for commercial use. 
-        You must retain, in the source form of any derivative works that you  
-        distribute, all copyright, patent, trademark, and attribution notices  
-        from the source form of this work. 
-         
-        For commercial uses of this software, please send email to xwzhou@zju.edu.cn
-Project-URL: homepage, https://github.com/dendenxu/fast-gaussian-rasterization
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Requires-Dist: torch
-Requires-Dist: numpy
-Requires-Dist: cuda-python
-Requires-Dist: PyGLM
-Requires-Dist: PyOpenGL
-
 # Fast Gaussian Rasterization
 
 - **Can be 5-10x faster than the original software CUDA rasterizer ([diff-gaussian-rasterization](https://github.com/graphdeco-inria/diff-gaussian-rasterization)).**
 - **Can be 2-3x faster if using offline rendering. (Bottleneck: copying rendered images around, thinking about improvements.)**
-- **Speedup most visible with high pixel-to-point ratio (large gaussians, small point count, high-res rendering).**
+- **Speedup most visible with high pixel-to-point ratio (large Gaussians, small point count, high-res rendering).**
 
 https://github.com/dendenxu/fast-gaussian-splatting/assets/43734697/f50afd6f-bbd5-4e18-aca6-a7356a5d3f75
 
 No backward pass is supported yet. 
 Will think of ways to add a backward. 
 Depth-peeling ([4K4D](https://zju3dv.github.io/4k4d)) is too slow.
 Discussion welcomed.
 
 ## Installation
 
-No CUDA compilation is required.
+Install the latest release from PyPI:
 
 ```shell
 pip install fast_gauss
 ```
 
+Or the latest commit from GitHub:
+
+```shell
+pip install git+https://github.com/dendenxu/fast-gaussian-rasterization
+```
+
+No CUDA compilation is required to build `fast_gauss` since we're only shader-based for now.
+
 ## Usage
 
 Replace the original import of `diff_gaussian_rasterization` with `fast_gauss`.
 
 For example, replace this:
 
 ```python
@@ -69,57 +46,94 @@
 And you're good to go.
 
 ## Tips
 
 **Note: for the ultimate 5-10x performance increase, you'll need to let `fast_gauss`'s shader directly write to your desired framebuffer.**
 
 Currently, we are trying to automatically detect whether you're managing your own OpenGL context (i.e. opening up a GUI) by checking for the module `OpenGL` during the import of `fast_gauss`.
-
-If detected, all rendering command will return `None`s and we will directly write to the bound framebuffer at the time of the draw call.
-
+If detected, all rendering commands will return `None`s and we will directly write to the bound framebuffer at the time of the draw call.
 Thus if you're running in a GUI (OpenGL-based) environment, the output of our rasterizer will be `None`s and does not require further processing.
 
 - [ ] TODO: Improve offline rendering performance.
 - [ ] TODO: Add a warning to the user if they're performing further processing on the returned values.
 
-**Note: the speedup is mostly visible when the pixel-to-point ratio is high.**
-
-That is, when there're large gaussians and very high resolution rendering, the speedup is more visible.
+**Note: the speedup is the most visible when the pixel-to-point ratio is high.**
 
+That is, when there are large Gaussians and very high-resolution rendering, the speedup is more visible.
 The CUDA-based software implementation is more resolution sensitive and for some extremely dense point clouds (> 1 million points), the CUDA implementation might be faster.
+This is because the typical rasterization-based pipeline on modern graphics hardware is [not well-optimized for small triangles](https://www.youtube.com/watch?v=hf27qsQPRLQ&list=WL).
+
+**Note: for best performance, cache the persistent results (for example, the 6 elements of the covariance matrix).**
+
+This is more of a general tip and not directly related to `fast_gauss`.
+However, the impact is more observable here since we haven't implemented a fast 3D covariance computation (from scales and rotations) in the shader yet.
+Only PyTorch implementation is available for now.
 
-This is because the typical rasterization-based pipeline on modern graphics are [not well-optimized for small triangles](https://www.youtube.com/watch?v=hf27qsQPRLQ&list=WL).
+When the point count increases, even the smallest `precomputation` can help.
+An example is the concatenation of the base 0-degree SH parameter and the rest, that small maneuver might cost us 10ms on a 3060 with 5 million points.
+Thus, store the concatenated tensors instead and avoid concatenating them in every frame.
 
-**Note: it's recommended to pass in a CPU tensor in the GaussianRasterizationSettings to avoid explicit synchronizations for even better performance.**
+- [ ] TODO: Implement SH eval in the vertex shader.
+- [ ] TODO: Warn users if they're not properly precomputing the covariance matrix.
+- [ ] TODO: Implement a more optimized `OptimizedGaussians` for precomputing things and apply a cache. Similar to that of the vertex shader (see [Invokation frequency](https://www.khronos.org/opengl/wiki/Vertex_Shader)).
+
+**Note: it's recommended to pass in a CPU tensor in the `GaussianRasterizationSettings` to avoid explicit synchronizations for even better performance.**
 
 - [ ] TODO: Add a warning to the user if GPU tensors are detected.
 
 **Note: the second output of the `GaussianRasterizer` is not radii anymore (since we're not gonna use it for the backward pass), but the alpha values of the rendered image instead.**
 
 And the alpha channel content seems to be bugged currently, will debug.
 
-- [ ] TODO: Debug alpha channel
+- [ ] TODO: Debug alpha channel values
 
 ## TODOs
 
 - [ ] TODO: Apply more of the optimization techniques used by similar shaders, including packing the data into a texture and bit reduction during computation.
 - [ ] TODO: Thinks of ways for a backward pass. Welcome to discuss!
-- [ ] TODO: Compute covariance from scaling and rotation in the shader, currently it's on the CUDA side.
-- [ ] TODO: Compute SH in the shader, currently it's on the CUDA side.
+- [ ] TODO: Compute covariance from scaling and rotation in the shader, currently it's on the CUDA (PyTorch) side.
+- [ ] TODO: Compute SH in the shader, currently it's on the CUDA (PyTorch) side.
+- [ ] TODO: Try to align the rendering results at the pixel level, small deviation exists currently.
+- [ ] TODO: Use indexed draw calls to minimize data passing and shuffling.
+- [ ] TODO: Do incremental sorting based on viewport change, currently it's a full resort on with CUDA (PyTorch).
+
+## Implementation
+
+**Guidelines**
+
+- Let the professionals do the work.
+  - Let GPU do the large-scale sorting.
+  - Let the graphics pipeline do the rasterization for us, not the other way around.
+  - Let OpenGL directly write to your framebuffer.
+- Minimize repeated work.
+  - Compute the 3D to 2D covariance projection only once for each Gaussian, instead of 4 times for the quad, enabled by the geometry shader.
+- Minimize stalls (minimize explicit synchronizations between GPU and CPU).
+  - Enabled by using `non_blocking=True` data passing and moving sync points to as early as possible.
+  - Boosted by the fact that we're sorting on the GPU, thus no need to perform synchronized host-to-device copies.
+
+**Why does a global sort work?**
+
+The OpenGL specification is somewhat vague but there's this reference:
+(in the 4th paragraph of section 2.1 of chapter 2 of this specification: https://registry.khronos.org/OpenGL/specs/gl/glspec44.core.pdf)
+
+> Commands are always processed in the order in which they are received, although there may be an indeterminate delay before the effects of a command are realized. This means, for example, that one primitive must be drawn completely before any subsequent one can affect the framebuffer.
+
+Thus if the order of the data in the vertex buffer (or as specified by an index buffer) is back-to-front, and alpha blending is enabled, you can count on OpenGL to correctly update the framebuffer in the correct back to front order.
+
+- [ ] TODO: Expand implementation details.
 
 ## Environment
 
 This project requires you to have an NVIDIA GPU with the ability to interop between CUDA and OpenGL.
 Thus, WSL is [not supported](https://docs.nvidia.com/cuda/wsl-user-guide/index.html#features-not-yet-supported) and OSX (MacOS) is not supported.
+Tested on Linux and Windows.
 
 For offline rendering (the drop-in replacement of the original CUDA rasterizer), we also need a valid EGL environment.
 It can sometimes be hard to set up for virtualized machines. [Potential fix](https://github.com/zju3dv/4K4D/issues/27#issuecomment-2026747401).
 
-- [ ] TODO: Test on more platforms.
-
 ## Credits
 
 Inspired by those insanely fast WebGL-based 3DGS viewers:
 
 - [GaussianSplats3D](https://github.com/mkkellogg/GaussianSplats3D) for inspiring our vertex-geometry-fragment shader pipeline.
 - [gsplat.tech](https://gsplat.tech/).
 - [splat](https://github.com/antimatter15/splat).
@@ -135,13 +149,13 @@
 - [EasyVolcap](https://github.com/zju3dv/EasyVolcap) for the collection of utilities, including EGL setup.
 - [nvdiffrast](https://nvlabs.github.io/nvdiffrast) for their EGL context setup and CUDA-GL interop setup.
 
 ## Citation
 
 ```bibtex
 @misc{fast_gauss,  
-    title = {Fast Gaussian Splatting},
+    title = {Fast Gaussian Rasterization},
     howpublished = {GitHub},  
     year = {2024},
     url = {https://github.com/dendenxu/fast-gaussian-rasterization}
 }
 ```
```

### Comparing `fast_gauss-0.0.5/fast_gauss/__init__.py` & `fast_gauss-0.0.6/fast_gauss/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_gauss-0.0.5/fast_gauss/console_utils.py` & `fast_gauss-0.0.6/fast_gauss/console_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 from rich.console import Console
 from rich.progress import Progress
 from rich.table import Table, Column
 from rich.pretty import Pretty, pretty_repr, pprint
 from rich.progress import BarColumn, TimeElapsedColumn, TimeRemainingColumn, filesize, ProgressColumn
 from tqdm.std import tqdm as std_tqdm
 from tqdm.rich import tqdm_rich, FractionColumn, RateColumn
-from easyvolcap.utils.base_utils import default_dotdict, dotdict, DoNothing
+from .base_utils import default_dotdict, dotdict, DoNothing
 
 pdbr_theme = 'ansi_dark'
 pdbr.utils.set_traceback(pdbr_theme)
 RichPdb._theme = pdbr_theme
 # fmt: on
 
 
@@ -783,7 +783,15 @@
         elif isinstance(v, bool):
             t = 'no_' + k if v else k
             parser.add_argument(f'--{t}', action='store_false' if v else 'store_true', dest=k, help=markup_to_ansi(help_pattern.format(v)))
         else:
             parser.add_argument(f'--{k}', type=type(v), default=v, help=markup_to_ansi(help_pattern.format(v)))
 
     return parser
+
+
+def warn_once(message: str):
+    if not hasattr(warn_once, 'warned'):
+        warn_once.warned = set()
+    if message not in warn_once.warned:
+        log(yellow(message))
+        warn_once.warned.add(message)
```

### Comparing `fast_gauss-0.0.5/fast_gauss/cuda_utils.py` & `fast_gauss-0.0.6/fast_gauss/cuda_utils.py`

 * *Files identical despite different names*

### Comparing `fast_gauss-0.0.5/fast_gauss/data_utils.py` & `fast_gauss-0.0.6/fast_gauss/data_utils.py`

 * *Files identical despite different names*

### Comparing `fast_gauss-0.0.5/fast_gauss/egl_utils.py` & `fast_gauss-0.0.6/fast_gauss/egl_utils.py`

 * *Files identical despite different names*

### Comparing `fast_gauss-0.0.5/fast_gauss/gaussian_utils.py` & `fast_gauss-0.0.6/fast_gauss/gaussian_utils.py`

 * *Files identical despite different names*

### Comparing `fast_gauss-0.0.5/fast_gauss/gl_utils.py` & `fast_gauss-0.0.6/fast_gauss/gl_utils.py`

 * *Files identical despite different names*

### Comparing `fast_gauss-0.0.5/fast_gauss/gsplat_utils.py` & `fast_gauss-0.0.6/fast_gauss/gsplat_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,14 +50,21 @@
 
         self.compile_shaders()
         self.use_gl_program(self.gsplat_program)
         self.opengl_options()
         self.resize_buffers(init_buffer_size)
         self.resize_textures(*init_texture_size)
 
+        log(green_slim(f'GSplatContextManager initialized with attribute dtype: {self.dtype}, texture dtype: {self.tex_dtype}, offline rendering: {self.offline_rendering}, buffer size: {init_buffer_size}, texture size: {init_texture_size}'))
+
+        if not self.offline_rendering:
+            log(green_slim('Using online rendering mode, in this mode, calling the rendering function of fast_gauss will write directly to the currently bound framebuffer'))
+            log(green_slim('In this mode, the output of all rasterization calls will be None (same output count). Please do not perform further processing on them.'))
+            log(green_slim('Please make sure to set up the correct GUI environment before calling the rasterization function, see more in readme.md'))
+
     def opengl_options(self):
         # Performs face culling
         gl.glDisable(gl.GL_CULL_FACE)
 
         # Performs z-buffer testing
         gl.glDisable(gl.GL_DEPTH_TEST)
         gl.glDisable(gl.GL_ALPHA_TEST)
@@ -216,14 +223,21 @@
         if not hasattr(self, 'max_verts'): self.max_verts = 0
         if v > self.max_verts:
             if v > self.max_verts: self.max_verts = int(v * 1.05)
             self.init_gl_buffers(self.max_verts)
 
     @torch.no_grad()
     def render(self, xyz3: torch.Tensor, cov6: torch.Tensor, rgb3: torch.Tensor, occ1: torch.Tensor, raster_settings: 'GaussianRasterizationSettings'):
+        if xyz3.dtype != self.dtype:
+            warn_once(yellow(f'Input tensors has dtype {xyz3.dtype}, expected {self.dtype}, will cast to {self.dtype}'))
+            xyz3, cov6, rgb3, occ1 = xyz3.to(self.dtype), cov6.to(self.dtype), rgb3.to(self.dtype), occ1.to(self.dtype)
+            for key in raster_settings:
+                if isinstance(raster_settings[key], torch.Tensor):
+                    raster_settings[key] = raster_settings[key].to(self.dtype)
+
         # Prepare OpenGL texture size
         H, W = raster_settings.image_height, raster_settings.image_width
         self.resize_textures(H, W)
         self.resize_buffers(len(xyz3))
         timer.record('resize')
 
         # Compute GS
@@ -233,15 +247,15 @@
         view = point_padding(xyz3) @ raster_settings.viewmatrix.to('cuda', non_blocking=True)
         idx = view[..., 2].argsort(descending=True)  # S, sorted
         data = data[idx].ravel().contiguous()  # sorted data on gpu
         timer.record('sorting')
 
         # Upload sorted data to OpenGL for rendering
         from cuda import cudart
-        from easyvolcap.utils.cuda_utils import CHECK_CUDART_ERROR, FORMAT_CUDART_ERROR
+        from .cuda_utils import CHECK_CUDART_ERROR, FORMAT_CUDART_ERROR
         kind = cudart.cudaMemcpyKind.cudaMemcpyDeviceToDevice
 
         CHECK_CUDART_ERROR(cudart.cudaGraphicsMapResources(1, self.cu_vbo, torch.cuda.current_stream().cuda_stream))
         cu_vbo_ptr, cu_vbo_size = CHECK_CUDART_ERROR(cudart.cudaGraphicsResourceGetMappedPointer(self.cu_vbo))
 
         CHECK_CUDART_ERROR(cudart.cudaMemcpyAsync(cu_vbo_ptr,
                                                   data.data_ptr(),
@@ -289,14 +303,18 @@
                                                                  0,  # hOffset
                                                                  W * 4 * rgba_map.element_size(),  # width Width of matrix transfer (columns in bytes)
                                                                  H,  # height
                                                                  kind,  # kind
                                                                  torch.cuda.current_stream().cuda_stream))  # stream
             CHECK_CUDART_ERROR(cudart.cudaGraphicsUnmapResources(1, cu_tex, torch.cuda.current_stream().cuda_stream))
 
+            if rgba_map.dtype != xyz3.dtype:
+                warn_once(yellow(f'Using texture dtype {rgba_map.dtype}, expected {xyz3.dtype} for the output, will cast to {xyz3.dtype}'))
+                rgba_map = rgba_map.to(xyz3.dtype)
+
             return rgba_map  # H, W, 4
         else:
             return None
 
     def rasterize_gaussians(
         self,
         means3D: torch.Tensor,  # N, 3
```

### Comparing `fast_gauss-0.0.5/fast_gauss/math_utils.py` & `fast_gauss-0.0.6/fast_gauss/math_utils.py`

 * *Files identical despite different names*

### Comparing `fast_gauss-0.0.5/fast_gauss/sh_utils.py` & `fast_gauss-0.0.6/fast_gauss/sh_utils.py`

 * *Files identical despite different names*

### Comparing `fast_gauss-0.0.5/fast_gauss/shaders/gsplat.frag` & `fast_gauss-0.0.6/fast_gauss/shaders/gsplat.frag`

 * *Files identical despite different names*

### Comparing `fast_gauss-0.0.5/fast_gauss/shaders/gsplat.geom` & `fast_gauss-0.0.6/fast_gauss/shaders/gsplat.geom`

 * *Files identical despite different names*

### Comparing `fast_gauss-0.0.5/fast_gauss/shaders/gsplat.vert` & `fast_gauss-0.0.6/fast_gauss/shaders/gsplat.vert`

 * *Files identical despite different names*

### Comparing `fast_gauss-0.0.5/fast_gauss.egg-info/SOURCES.txt` & `fast_gauss-0.0.6/fast_gauss.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 license
 pyproject.toml
 readme.md
 requirements.txt
 fast_gauss/__init__.py
+fast_gauss/base_utils.py
 fast_gauss/console_utils.py
 fast_gauss/cuda_utils.py
 fast_gauss/data_utils.py
 fast_gauss/egl_utils.py
 fast_gauss/gaussian_utils.py
 fast_gauss/gl_utils.py
 fast_gauss/gsplat_utils.py
```

### Comparing `fast_gauss-0.0.5/license` & `fast_gauss-0.0.6/license`

 * *Files identical despite different names*

