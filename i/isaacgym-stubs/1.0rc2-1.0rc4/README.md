# Comparing `tmp/isaacgym_stubs-1rc2.tar.gz` & `tmp/isaacgym-stubs-1.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isaacgym_stubs-1rc2.tar", last modified: Fri Apr 12 17:39:15 2024, max compression
+gzip compressed data, was "isaacgym-stubs-1.0rc4.tar", last modified: Sat Feb 25 07:19:29 2023, max compression
```

## Comparing `isaacgym_stubs-1rc2.tar` & `isaacgym-stubs-1.0rc4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 yuzhe     (1000) yuzhe     (1000)        0 2024-04-12 17:39:15.838683 isaacgym_stubs-1rc2/
--rw-rw-r--   0 yuzhe     (1000) yuzhe     (1000)     1067 2023-02-25 07:12:02.000000 isaacgym_stubs-1rc2/LICENSE
--rw-r--r--   0 yuzhe     (1000) yuzhe     (1000)     2805 2024-04-12 17:39:15.838683 isaacgym_stubs-1rc2/PKG-INFO
--rw-rw-r--   0 yuzhe     (1000) yuzhe     (1000)     2340 2023-10-15 02:33:00.000000 isaacgym_stubs-1rc2/README.md
-drwxrwxr-x   0 yuzhe     (1000) yuzhe     (1000)        0 2024-04-12 17:39:15.838683 isaacgym_stubs-1rc2/isaacgym-stubs/
--rw-rw-r--   0 yuzhe     (1000) yuzhe     (1000)       22 2023-02-24 05:20:42.000000 isaacgym_stubs-1rc2/isaacgym-stubs/__init__.py
--rw-rw-r--   0 yuzhe     (1000) yuzhe     (1000)    66910 2024-04-11 00:00:11.000000 isaacgym_stubs-1rc2/isaacgym-stubs/gymapi.pyi
-drwxrwxr-x   0 yuzhe     (1000) yuzhe     (1000)        0 2024-04-12 17:39:15.838683 isaacgym_stubs-1rc2/isaacgym_stubs.egg-info/
--rw-r--r--   0 yuzhe     (1000) yuzhe     (1000)     2805 2024-04-12 17:39:15.000000 isaacgym_stubs-1rc2/isaacgym_stubs.egg-info/PKG-INFO
--rw-rw-r--   0 yuzhe     (1000) yuzhe     (1000)      246 2024-04-12 17:39:15.000000 isaacgym_stubs-1rc2/isaacgym_stubs.egg-info/SOURCES.txt
--rw-rw-r--   0 yuzhe     (1000) yuzhe     (1000)        1 2024-04-12 17:39:15.000000 isaacgym_stubs-1rc2/isaacgym_stubs.egg-info/dependency_links.txt
--rw-rw-r--   0 yuzhe     (1000) yuzhe     (1000)       15 2024-04-12 17:39:15.000000 isaacgym_stubs-1rc2/isaacgym_stubs.egg-info/top_level.txt
--rw-rw-r--   0 yuzhe     (1000) yuzhe     (1000)      489 2024-04-12 17:38:08.000000 isaacgym_stubs-1rc2/pyproject.toml
--rw-rw-r--   0 yuzhe     (1000) yuzhe     (1000)       38 2024-04-12 17:39:15.838683 isaacgym_stubs-1rc2/setup.cfg
--rw-rw-r--   0 yuzhe     (1000) yuzhe     (1000)      307 2024-04-12 04:25:37.000000 isaacgym_stubs-1rc2/setup.py
+drwxrwxr-x   0 yuzhe     (1000) yuzhe     (1000)        0 2023-02-25 07:19:29.789794 isaacgym-stubs-1.0rc4/
+-rw-rw-r--   0 yuzhe     (1000) yuzhe     (1000)     1067 2023-02-25 07:12:02.000000 isaacgym-stubs-1.0rc4/LICENSE
+-rw-rw-r--   0 yuzhe     (1000) yuzhe     (1000)     1648 2023-02-25 07:19:29.789794 isaacgym-stubs-1.0rc4/PKG-INFO
+-rw-rw-r--   0 yuzhe     (1000) yuzhe     (1000)     1183 2023-02-25 07:13:13.000000 isaacgym-stubs-1.0rc4/README.md
+drwxrwxr-x   0 yuzhe     (1000) yuzhe     (1000)        0 2023-02-25 07:19:29.789794 isaacgym-stubs-1.0rc4/isaacgym-stubs/
+-rw-rw-r--   0 yuzhe     (1000) yuzhe     (1000)       22 2023-02-24 05:20:42.000000 isaacgym-stubs-1.0rc4/isaacgym-stubs/__init__.py
+-rw-rw-r--   0 yuzhe     (1000) yuzhe     (1000)    68303 2023-02-24 05:02:26.000000 isaacgym-stubs-1.0rc4/isaacgym-stubs/gymapi.pyi
+drwxrwxr-x   0 yuzhe     (1000) yuzhe     (1000)        0 2023-02-25 07:19:29.789794 isaacgym-stubs-1.0rc4/isaacgym_stubs.egg-info/
+-rw-rw-r--   0 yuzhe     (1000) yuzhe     (1000)     1648 2023-02-25 07:19:29.000000 isaacgym-stubs-1.0rc4/isaacgym_stubs.egg-info/PKG-INFO
+-rw-rw-r--   0 yuzhe     (1000) yuzhe     (1000)      246 2023-02-25 07:19:29.000000 isaacgym-stubs-1.0rc4/isaacgym_stubs.egg-info/SOURCES.txt
+-rw-rw-r--   0 yuzhe     (1000) yuzhe     (1000)        1 2023-02-25 07:19:29.000000 isaacgym-stubs-1.0rc4/isaacgym_stubs.egg-info/dependency_links.txt
+-rw-rw-r--   0 yuzhe     (1000) yuzhe     (1000)       15 2023-02-25 07:19:29.000000 isaacgym-stubs-1.0rc4/isaacgym_stubs.egg-info/top_level.txt
+-rw-rw-r--   0 yuzhe     (1000) yuzhe     (1000)      489 2023-02-25 07:19:26.000000 isaacgym-stubs-1.0rc4/pyproject.toml
+-rw-rw-r--   0 yuzhe     (1000) yuzhe     (1000)       38 2023-02-25 07:19:29.789794 isaacgym-stubs-1.0rc4/setup.cfg
+-rw-rw-r--   0 yuzhe     (1000) yuzhe     (1000)      307 2023-02-25 06:26:03.000000 isaacgym-stubs-1.0rc4/setup.py
```

### Comparing `isaacgym_stubs-1rc2/LICENSE` & `isaacgym-stubs-1.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `isaacgym_stubs-1rc2/README.md` & `isaacgym-stubs-1.0rc4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,57 +1,47 @@
-Isaac Gym Python Stubs for Code Completion
+Metadata-Version: 2.1
+Name: isaacgym-stubs
+Version: 1.0rc4
+Summary: Isaac Gym Python Stubs for Code Completion
+Author: Yuzhe Qin
+Author-email: Yuzhe Qin <y1qin@ucsd.edu>
+Project-URL: Homepage, https://github.com/yzqin/isaacgym-stubs
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
 
-[![PyPI version](https://badge.fury.io/py/isaacgym-stubs.svg)](https://badge.fury.io/py/isaacgym-stubs)
+Isaac Gym Python Stubs for Code Completion
 ==========================================
 
-Enable code completion for IsaacGym simply with `pip install isaacgym-stubs`, even without IsaacGym itself!
+Code completion for IsaacGym with one line `pip install`, even without IsaacGym itself.
 
 ```bash
-# Install from PyPi
-pip3 install isaacgym-stubs
-
-# Alternatively, install from Github
-# pip3 install git+https://github.com/yzqin/isaacgym-stubs.git
+pip3 install git+https://github.com/yzqin/isaacgym-stubs.git
 ```
 
-Begin your code with the typical `from isaacgym import gymapi` and enjoy auto-completion.
+Depending on which IDE you are using, sometimes you may need to restart the IDE after `pip install` for re-indexing.
 
-The magic of `stub` is that you even **do not need to pip install IsaacGym itself**.
-
-For example, you may want to run IsaacGym on server but develop the code on a MacBook.
-IsaacGym may not support Mac. But you can still install this repo on MacBook and get smooth code completion during
-development!
+The magic of `stub` is that you even **do not need to pip install IsaacGym itself** to write the code.
+For example, you may need to run IsaacGym on server for training but develop the code on your MacBook.
+IsaacGym does not support Mac. But you can still install this repo and get smooth code completion to write IsaacGym
+code on that MacBook!
 
 ### Demo
 
 **VsCode**
 
 ![VsCode Demo](files/vscode.gif)
 
 **PyCharm**
 
 ![PyCharm Demo](files/pycharm.gif)
 
-### Troubleshooting
-
-1. The Python interpreter specified in your IDE should be the Python where isaacgym-stubs is installed. For
-   example, if you install this repository with conda Python but select the system Python as the interpreter in your
-   IDE, you won't have any code auto-completion. Follow the official instruction
-   [here](https://code.visualstudio.com/docs/python/environments) for VSCode
-   and [here](https://www.jetbrains.com/help/pycharm/configuring-python-interpreter.html) for PyCharm.
-2. Code auto-completion will not function if there's a directory named `issacgym` in your workspace. In this
-   case, the isaacgym symbol in your import will point to the directory instead of this package, disrupting the
-   auto-completion. Ensure that there's no `isaacgym` directory in your IDE workspace.
-3. Depending on which IDE you are using, sometimes you may need to restart the IDE after `pip install` for re-indexing.
-
 ### Overview
 
 This repository contains the `pyi` stub for the IsaacGym library, which can be used for code completion and type
 checking.
 According to the guidelines outlined in [PEP-561](https://peps.python.org/pep-0561/), Python stub files contain only
 type information and no runtime code.
 The `stub` in this repo is generated based on IsaacGym version `1.0rc4`.
-
-### How to Generate This `pyi`
-
-See [here](./STUB.md) for more explanation.
-
```

### Comparing `isaacgym_stubs-1rc2/isaacgym-stubs/gymapi.pyi` & `isaacgym-stubs-1.0rc4/isaacgym-stubs/gymapi.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 AXIS_TRANSLATION: int
 AXIS_TWIST: int
 AXIS_X: int
 AXIS_Y: int
 AXIS_Z: int
 CC_ALL_SUBSTEPS: ContactCollection
 CC_LAST_SUBSTEP: ContactCollection
+CC_NEVER: ContactCollection
 COMPUTE_PER_FACE: MeshNormalMode
 COMPUTE_PER_VERTEX: MeshNormalMode
 DEFAULT_VIEWER_HEIGHT: int
 DEFAULT_VIEWER_WIDTH: int
 DOF_INVALID: DofType
 DOF_MODE_EFFORT: DofDriveMode
 DOF_MODE_NONE: DofDriveMode
@@ -174,14 +175,15 @@
 MOUSE_RIGHT_BUTTON: MouseInput
 MOUSE_SCROLL_DOWN: MouseInput
 MOUSE_SCROLL_LEFT: MouseInput
 MOUSE_SCROLL_RIGHT: MouseInput
 MOUSE_SCROLL_UP: MouseInput
 RIGID_BODY_DISABLE_GRAVITY: int
 RIGID_BODY_DISABLE_SIMULATION: int
+RIGID_BODY_ENABLE_GYROSCOPIC_FORCES: int
 RIGID_BODY_NONE: int
 SIM_FLEX: SimType
 SIM_PHYSX: SimType
 STATE_ALL: int
 STATE_NONE: int
 STATE_POS: int
 STATE_VEL: int
@@ -229,14 +231,15 @@
     angular_damping: float
     armature: float
     collapse_fixed_joints: bool
     convex_decomposition_from_submeshes: bool
     default_dof_drive_mode: int
     density: float
     disable_gravity: bool
+    enable_gyroscopic_forces: bool
     fix_base_link: bool
     flip_visual_attachments: bool
     linear_damping: float
     max_angular_velocity: float
     max_linear_velocity: float
     mesh_normal_mode: MeshNormalMode
     min_particle_mass: float
@@ -331,14 +334,15 @@
     def __setstate__(self, arg0: tuple) -> None: ...
 
 
 class ContactCollection:
     __members__: ClassVar[dict] = ...  # read-only
     CC_ALL_SUBSTEPS: ClassVar[ContactCollection] = ...
     CC_LAST_SUBSTEP: ClassVar[ContactCollection] = ...
+    CC_NEVER: ClassVar[ContactCollection] = ...
     __entries: ClassVar[dict] = ...
 
     def __init__(self, arg0: int) -> None: ...
 
     def __eq__(self, other) -> Any: ...
 
     def __ge__(self, other) -> Any: ...
@@ -539,14 +543,22 @@
     def __init__(self) -> None: ...
 
     def get_forces(self) -> SpatialForce: ...
 
     def get_global_index(self) -> int: ...
 
 
+class ForceSensorProperties:
+    enable_constraint_solver_forces: bool
+    enable_forward_dynamics_forces: bool
+    use_world_frame: bool
+
+    def __init__(self) -> None: ...
+
+
 class Gym:
     def __init__(self, *args, **kwargs) -> None: ...
 
     def acquire_actor_root_state_tensor(self, arg0: Sim) -> Tensor: ...
 
     def acquire_dof_force_tensor(self, arg0: Sim) -> Tensor: ...
 
@@ -566,22 +578,27 @@
 
     def acquire_pneumatic_target_tensor(self, arg0: Sim) -> Tensor: ...
 
     def acquire_rigid_body_state_tensor(self, arg0: Sim) -> Tensor: ...
 
     def add_ground(self, sim: Sim, params: PlaneParams) -> None: ...
 
+    def add_heightfield(self, arg0: Sim, arg1: numpy.ndarray[int16], arg2: HeightFieldParams) -> None: ...
+
     @overload
     def add_lines(self, arg0: Viewer, arg1: Env, arg2: int, arg3: numpy.ndarray[float32],
                   arg4: numpy.ndarray[float32]) -> None: ...
 
     @overload
     def add_lines(self, arg0: Viewer, arg1: Env, arg2: int, arg3: numpy.ndarray[Vec3],
                   arg4: numpy.ndarray[Vec3]) -> None: ...
 
+    def add_triangle_mesh(self, arg0: Sim, arg1: numpy.ndarray[float32], arg2: numpy.ndarray[uint32],
+                          arg3: TriangleMeshParams) -> None: ...
+
     def apply_actor_dof_efforts(self, arg0: Env, arg1: int, arg2: numpy.ndarray[float32]) -> bool: ...
 
     def apply_body_force_at_pos(self, env: Env, rigidHandle: int, force: Vec3, pos: Vec3 = ...,
                                 space: CoordinateSpace = ...) -> None: ...
 
     def apply_body_forces(self, env: Env, rigidHandle: int, force: Vec3 = ..., torque: Vec3 = ...,
                           space: CoordinateSpace = ...) -> None: ...
@@ -604,26 +621,26 @@
     def clear_lines(self, arg0: Viewer) -> None: ...
 
     def create_actor(self, env: Env, asset: Asset, pose: Transform, name: str = ..., group: int = ...,
                      filter: int = ..., segmentationId: int = ...) -> int: ...
 
     def create_aggregate(self, arg0: Env, arg1: List[int]) -> bool: ...
 
+    def create_asset_force_sensor(self, *args, **kwargs) -> Any: ...
+
     def create_box(self, sim: Sim, width: float, height: float, depth: float, options: AssetOptions = ...) -> Asset: ...
 
     def create_camera_sensor(self, arg0: Env, arg1: CameraProperties) -> int: ...
 
     def create_capsule(self, sim: Sim, radius: float, width: float, options: AssetOptions = ...) -> Asset: ...
 
     def create_cloth_grid(self, arg0: Sim, arg1: int, arg2: int, arg3: float, arg4: float) -> Asset: ...
 
     def create_env(self, arg0: Sim, arg1: Vec3, arg2: Vec3, arg3: int) -> Env: ...
 
-    def create_force_sensor(self, *args, **kwargs) -> Any: ...
-
     def create_performance_timers(self, arg0: Sim) -> int: ...
 
     def create_rigid_body_attractor(self, arg0: Env, arg1: AttractorProperties) -> int: ...
 
     def create_sim(self, compute_device: int = ..., graphics_device: int = ..., type: SimType = ...,
                    params: SimParams = ...) -> Sim: ...
 
@@ -724,15 +741,15 @@
 
     def get_actor_count(self, arg0: Env) -> int: ...
 
     def get_actor_dof_count(self, arg0: Env, arg1: int) -> int: ...
 
     def get_actor_dof_dict(self, arg0: Env, arg1: int) -> Dict[str, int]: ...
 
-    def get_actor_dof_forces(self, arg0: Env, arg1: int) -> numpy.ndarray[float32]: ...
+    def get_actor_dof_forces(self, arg0: Env, arg1: int) -> numpy.ndarray[numpy.float32]: ...
 
     def get_actor_dof_frames(self, arg0: Env, arg1: int) -> numpy.ndarray[DofFrame]: ...
 
     def get_actor_dof_handle(self, arg0: Env, arg1: int, arg2: int) -> int: ...
 
     def get_actor_dof_index(self, arg0: Env, arg1: int, arg2: int, arg3: IndexDomain) -> int: ...
 
@@ -746,14 +763,18 @@
 
     def get_actor_dof_velocity_targets(self, *args, **kwargs) -> Any: ...
 
     def get_actor_fixed_tendon_joint_coefficients(self, arg0: Env, arg1: int, arg2: int) -> List[float]: ...
 
     def get_actor_fixed_tendon_joint_name(self, arg0: Env, arg1: int, arg2: int, arg3: int) -> str: ...
 
+    def get_actor_force_sensor(self, arg0: Env, arg1: int, arg2: int) -> ForceSensor: ...
+
+    def get_actor_force_sensor_count(self, arg0: Env, arg1: int) -> int: ...
+
     def get_actor_handle(self, arg0: Env, arg1: int) -> int: ...
 
     def get_actor_index(self, arg0: Env, arg1: int, arg2: IndexDomain) -> int: ...
 
     def get_actor_joint_count(self, arg0: Env, arg1: int) -> int: ...
 
     def get_actor_joint_dict(self, arg0: Env, arg1: int) -> Dict[str, int]: ...
@@ -868,19 +889,19 @@
 
     def get_attractor_properties(self, arg0: Env, arg1: int) -> AttractorProperties: ...
 
     def get_camera_image(self, arg0: Sim, arg1: Env, arg2: int, arg3: ImageType) -> object: ...
 
     def get_camera_image_gpu_tensor(self, arg0: Sim, arg1: Env, arg2: int, arg3: ImageType) -> object: ...
 
-    def get_camera_proj_matrix(self, arg0: Sim, arg1: Env, arg2: int) -> numpy.ndarray[float32]: ...
+    def get_camera_proj_matrix(self, arg0: Sim, arg1: Env, arg2: int) -> numpy.ndarray[numpy.float32]: ...
 
     def get_camera_transform(self, arg0: Sim, arg1: Env, arg2: int) -> Transform: ...
 
-    def get_camera_view_matrix(self, arg0: Sim, arg1: Env, arg2: int) -> numpy.ndarray[float32]: ...
+    def get_camera_view_matrix(self, arg0: Sim, arg1: Env, arg2: int) -> numpy.ndarray[numpy.float32]: ...
 
     def get_dof_frame(self, arg0: Env, arg1: int) -> DofFrame: ...
 
     def get_dof_position(self, arg0: Env, arg1: int) -> float: ...
 
     def get_dof_target_position(self, arg0: Env, arg1: int) -> float: ...
 
@@ -1193,14 +1214,29 @@
     def viewer_camera_look_at(self, arg0: Viewer, arg1: Env, arg2: Vec3, arg3: Vec3) -> None: ...
 
     def write_camera_image_to_file(self, arg0: Sim, arg1: Env, arg2: int, arg3: ImageType, arg4: str) -> None: ...
 
     def write_viewer_image_to_file(self, arg0: Viewer, arg1: str) -> None: ...
 
 
+class HeightFieldParams:
+    column_scale: float
+    dynamic_friction: float
+    nbColumns: int
+    nbRows: int
+    restitution: float
+    row_scale: float
+    segmentation_id: int
+    static_friction: float
+    transform: Transform
+    vertical_scale: float
+
+    def __init__(self) -> None: ...
+
+
 class ImageType:
     __members__: ClassVar[dict] = ...  # read-only
     IMAGE_COLOR: ClassVar[ImageType] = ...
     IMAGE_DEPTH: ClassVar[ImageType] = ...
     IMAGE_OPTICAL_FLOW: ClassVar[ImageType] = ...
     IMAGE_SEGMENTATION: ClassVar[ImageType] = ...
     __entries: ClassVar[dict] = ...
@@ -1809,16 +1845,18 @@
 
     @property
     def torsion_friction(self) -> float: ...
 
 
 class RigidShapeProperties:
     compliance: float
+    contact_offset: float
     filter: int
     friction: float
+    rest_offset: float
     restitution: float
     rolling_friction: float
     thickness: float
     torsion_friction: float
 
     def __init__(self) -> None: ...
 
@@ -2117,14 +2155,26 @@
     def __getstate__(self) -> tuple: ...
 
     def __mul__(self, arg0: Transform) -> Transform: ...
 
     def __setstate__(self, arg0: tuple) -> None: ...
 
 
+class TriangleMeshParams:
+    dynamic_friction: float
+    nb_triangles: int
+    nb_vertices: int
+    restitution: float
+    segmentation_id: int
+    static_friction: float
+    transform: Transform
+
+    def __init__(self) -> None: ...
+
+
 class UpAxis:
     __members__: ClassVar[dict] = ...  # read-only
     UP_AXIS_Y: ClassVar[UpAxis] = ...
     UP_AXIS_Z: ClassVar[UpAxis] = ...
     __entries: ClassVar[dict] = ...
 
     def __init__(self, arg0: int) -> None: ...
@@ -2316,29 +2366,29 @@
     def __init__(self) -> None: ...
 
 
 class Viewer:
     def __init__(self, *args, **kwargs) -> None: ...
 
 
-def acquire_gym(*args, **kwargs) -> Any: ...
+def acquire_gym(*args, **kwargs) -> Gym: ...
 
 
 def carb_init(config_str: str = ...) -> bool: ...
 
 
 def cross(*args, **kwargs) -> Any: ...
 
 
 @overload
-def dot(arg0, arg1) -> numpy.ndarray[float32]: ...
+def dot(arg0, arg1) -> numpy.ndarray[numpy.float32]: ...
 
 
 @overload
-def dot(arg0, arg1) -> numpy.ndarray[float32]: ...
+def dot(arg0, arg1) -> numpy.ndarray[numpy.float32]: ...
 
 
 def eulers_to_quats_zyx(*args, **kwargs) -> Any: ...
 
 
 def quats_to_eulers_zyx(*args, **kwargs) -> Any: ...
```

