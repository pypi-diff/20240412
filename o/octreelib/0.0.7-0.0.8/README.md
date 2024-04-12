# Comparing `tmp/octreelib-0.0.7.tar.gz` & `tmp/octreelib-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octreelib-0.0.7.tar", max compression
+gzip compressed data, was "octreelib-0.0.8.tar", max compression
```

## Comparing `octreelib-0.0.7.tar` & `octreelib-0.0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    11357 2024-03-23 14:50:03.194430 octreelib-0.0.7/LICENSE
--rw-r--r--   0        0        0     1054 2024-03-23 14:50:03.194430 octreelib-0.0.7/README.md
--rw-r--r--   0        0        0        0 2024-03-23 14:50:03.198430 octreelib-0.0.7/octreelib/__init__.py
--rw-r--r--   0        0        0      310 2024-03-23 14:50:03.198430 octreelib-0.0.7/octreelib/grid/__init__.py
--rw-r--r--   0        0        0    14576 2024-03-23 14:50:03.198430 octreelib-0.0.7/octreelib/grid/grid.py
--rw-r--r--   0        0        0     7307 2024-03-23 14:50:03.198430 octreelib-0.0.7/octreelib/grid/grid_base.py
--rw-r--r--   0        0        0      578 2024-03-23 14:50:03.198430 octreelib-0.0.7/octreelib/internal/__init__.py
--rw-r--r--   0        0        0      740 2024-03-23 14:50:03.198430 octreelib-0.0.7/octreelib/internal/interfaces.py
--rw-r--r--   0        0        0      462 2024-03-23 14:50:03.198430 octreelib-0.0.7/octreelib/internal/point.py
--rw-r--r--   0        0        0       62 2024-03-23 14:50:03.198430 octreelib-0.0.7/octreelib/internal/typing.py
--rw-r--r--   0        0        0     2411 2024-03-23 14:50:03.198430 octreelib-0.0.7/octreelib/internal/voxel.py
--rw-r--r--   0        0        0      328 2024-03-23 14:50:03.198430 octreelib-0.0.7/octreelib/octree/__init__.py
--rw-r--r--   0        0        0    10556 2024-03-23 14:50:03.198430 octreelib-0.0.7/octreelib/octree/octree.py
--rw-r--r--   0        0        0     6827 2024-03-23 14:50:03.198430 octreelib-0.0.7/octreelib/octree/octree_base.py
--rw-r--r--   0        0        0      168 2024-03-23 14:50:03.198430 octreelib-0.0.7/octreelib/octree_manager/__init__.py
--rw-r--r--   0        0        0     6483 2024-03-23 14:50:03.198430 octreelib-0.0.7/octreelib/octree_manager/octree_manager.py
--rw-r--r--   0        0        0      207 2024-03-23 14:50:03.198430 octreelib-0.0.7/octreelib/ransac/__init__.py
--rw-r--r--   0        0        0     5379 2024-03-23 14:50:03.198430 octreelib-0.0.7/octreelib/ransac/cuda_ransac.py
--rw-r--r--   0        0        0     3733 2024-03-23 14:50:03.198430 octreelib-0.0.7/octreelib/ransac/util.py
--rw-r--r--   0        0        0      784 2024-03-23 14:50:27.590265 octreelib-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1988 1970-01-01 00:00:00.000000 octreelib-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-12 17:16:19.889083 octreelib-0.0.8/LICENSE
+-rw-r--r--   0        0        0     1054 2024-04-12 17:16:19.889083 octreelib-0.0.8/README.md
+-rw-r--r--   0        0        0        0 2024-04-12 17:16:19.889083 octreelib-0.0.8/octreelib/__init__.py
+-rw-r--r--   0        0        0      310 2024-04-12 17:16:19.889083 octreelib-0.0.8/octreelib/grid/__init__.py
+-rw-r--r--   0        0        0    14432 2024-04-12 17:16:19.889083 octreelib-0.0.8/octreelib/grid/grid.py
+-rw-r--r--   0        0        0     7307 2024-04-12 17:16:19.889083 octreelib-0.0.8/octreelib/grid/grid_base.py
+-rw-r--r--   0        0        0      578 2024-04-12 17:16:19.889083 octreelib-0.0.8/octreelib/internal/__init__.py
+-rw-r--r--   0        0        0      740 2024-04-12 17:16:19.889083 octreelib-0.0.8/octreelib/internal/interfaces.py
+-rw-r--r--   0        0        0      462 2024-04-12 17:16:19.889083 octreelib-0.0.8/octreelib/internal/point.py
+-rw-r--r--   0        0        0       62 2024-04-12 17:16:19.889083 octreelib-0.0.8/octreelib/internal/typing.py
+-rw-r--r--   0        0        0     2411 2024-04-12 17:16:19.889083 octreelib-0.0.8/octreelib/internal/voxel.py
+-rw-r--r--   0        0        0      328 2024-04-12 17:16:19.889083 octreelib-0.0.8/octreelib/octree/__init__.py
+-rw-r--r--   0        0        0    10556 2024-04-12 17:16:19.889083 octreelib-0.0.8/octreelib/octree/octree.py
+-rw-r--r--   0        0        0     6827 2024-04-12 17:16:19.889083 octreelib-0.0.8/octreelib/octree/octree_base.py
+-rw-r--r--   0        0        0      168 2024-04-12 17:16:19.889083 octreelib-0.0.8/octreelib/octree_manager/__init__.py
+-rw-r--r--   0        0        0     6483 2024-04-12 17:16:19.889083 octreelib-0.0.8/octreelib/octree_manager/octree_manager.py
+-rw-r--r--   0        0        0      207 2024-04-12 17:16:19.889083 octreelib-0.0.8/octreelib/ransac/__init__.py
+-rw-r--r--   0        0        0     5658 2024-04-12 17:16:19.889083 octreelib-0.0.8/octreelib/ransac/cuda_ransac.py
+-rw-r--r--   0        0        0     2376 2024-04-12 17:16:19.889083 octreelib-0.0.8/octreelib/ransac/util.py
+-rw-r--r--   0        0        0      784 2024-04-12 17:16:50.297183 octreelib-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1988 1970-01-01 00:00:00.000000 octreelib-0.0.8/PKG-INFO
```

### Comparing `octreelib-0.0.7/LICENSE` & `octreelib-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `octreelib-0.0.7/README.md` & `octreelib-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `octreelib-0.0.7/octreelib/grid/grid.py` & `octreelib-0.0.8/octreelib/grid/grid.py`

 * *Files 4% similar despite different names*

```diff
@@ -122,20 +122,22 @@
             self.__octrees[voxel_coordinates].map_leaf_points(function, pose_numbers)
 
     def map_leaf_points_cuda_ransac(
         self,
         poses_per_batch: int = 10,
         threshold: float = 0.01,
         hypotheses_number: int = 1024,
+        initial_points_number: int = 6,
     ):
         """
         transform point cloud in the node using the function
         :param poses_per_batch: Number of poses per batch.
         :param threshold: Distance threshold.
         :param hypotheses_number: Number of RANSAC iterations (<= 1024).
+        :param initial_points_number: Number of initial points to use in RANSAC.
         """
         if threshold <= 0:
             raise ValueError("Threshold must be positive")
         if hypotheses_number < 1:
             raise ValueError("Number of RANSAC hypotheses must be positive")
         if hypotheses_number > 1024:
             raise ValueError(
@@ -150,26 +152,19 @@
                     i,
                     min(i + poses_per_batch, len(self.__pose_voxel_coordinates)),
                 )
             )
             for i in range(0, len(self.__pose_voxel_coordinates), poses_per_batch)
         ]
 
-        # find the maximum number of leaf voxels across all batches
         # this is needed to initialize the random number generators on the GPU
-        max_leaf_voxels = max(
-            [
-                sum([self.n_leaves(pose_number) for pose_number in batch_pose_numbers])
-                for batch_pose_numbers in batches
-            ]
-        )
         ransac = CudaRansac(
-            max_blocks_number=max_leaf_voxels,
-            hypotheses_number=hypotheses_number,
             threshold=threshold,
+            hypotheses_number=hypotheses_number,
+            initial_points_number=initial_points_number,
         )
 
         # process each batch
         for batch_pose_numbers in batches:
             # `combined_point_cloud` is a concatenation of ALL point clouds
             # `block_sizes` is a list of sizes of point clouds for each leaf node
             # `pose_dividers` is a list of indices where combined_point_cloud is divided by pose
```

### Comparing `octreelib-0.0.7/octreelib/grid/grid_base.py` & `octreelib-0.0.8/octreelib/grid/grid_base.py`

 * *Files identical despite different names*

### Comparing `octreelib-0.0.7/octreelib/internal/__init__.py` & `octreelib-0.0.8/octreelib/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `octreelib-0.0.7/octreelib/internal/interfaces.py` & `octreelib-0.0.8/octreelib/internal/interfaces.py`

 * *Files identical despite different names*

### Comparing `octreelib-0.0.7/octreelib/internal/voxel.py` & `octreelib-0.0.8/octreelib/internal/voxel.py`

 * *Files identical despite different names*

### Comparing `octreelib-0.0.7/octreelib/octree/octree.py` & `octreelib-0.0.8/octreelib/octree/octree.py`

 * *Files identical despite different names*

### Comparing `octreelib-0.0.7/octreelib/octree/octree_base.py` & `octreelib-0.0.8/octreelib/octree/octree_base.py`

 * *Files identical despite different names*

### Comparing `octreelib-0.0.7/octreelib/octree_manager/octree_manager.py` & `octreelib-0.0.8/octreelib/octree_manager/octree_manager.py`

 * *Files identical despite different names*

### Comparing `octreelib-0.0.7/octreelib/ransac/cuda_ransac.py` & `octreelib-0.0.8/octreelib/ransac/cuda_ransac.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 import numpy as np
 import numpy.typing as npt
 import numba as nb
 from numba import cuda
-from numba.cuda.random import create_xoroshiro128p_states
 
 from octreelib.internal import PointCloud
 from octreelib.ransac.util import (
-    generate_random_indices,
     get_plane_from_points,
     measure_distance,
-    INITIAL_POINTS_NUMBER,
 )
 
 __all__ = ["CudaRansac"]
 
 
 CUDA_THREADS = 1024
 
@@ -21,30 +18,30 @@
 class CudaRansac:
     """
     RANSAC implementation using CUDA.
     """
 
     def __init__(
         self,
-        max_blocks_number: int,
         threshold: float = 0.01,
         hypotheses_number: int = CUDA_THREADS,
+        initial_points_number: int = 6,
     ):
         """
         Initialize the RANSAC parameters.
         :param threshold: Distance threshold.
         :param hypotheses_number: Number of RANSAC hypotheses. (<= 1024)
-        :param max_blocks_number: Maximum number of blocks.
+        :param initial_points_number: Number of initial points to use in RANSAC.
         """
 
         self.__threshold: float = threshold
         self.__threads_per_block = min(hypotheses_number, CUDA_THREADS)
-        # create random number generator states
-        self.__rng_states = create_xoroshiro128p_states(
-            self.__threads_per_block * max_blocks_number, seed=0
+        self.__kernel = self.__get_kernel(initial_points_number)
+        self.__random_hypotheses_cuda = cuda.to_device(
+            np.random.random((self.__threads_per_block, initial_points_number))
         )
 
     def evaluate(
         self,
         point_cloud: PointCloud,
         block_sizes: npt.NDArray,
     ):
@@ -55,104 +52,106 @@
         """
 
         blocks_number = len(block_sizes)
 
         # create result mask and copy it to the device
         result_mask_cuda = cuda.to_device(np.zeros((len(point_cloud)), dtype=np.bool_))
 
-        # create arrays to store the maximum number of inliers and the best mask indices
-        max_inliers_number_cuda = cuda.to_device(
-            np.zeros(blocks_number, dtype=np.int32)
-        )
-
         # copy point_cloud, block_sizes and block_start_indices to the device
         point_cloud_cuda = cuda.to_device(point_cloud)
         block_sizes_cuda = cuda.to_device(block_sizes)
         # block_start_indices is an array of indices where each cuda block should
         # take data from this combined with block_sizes allows it to quickly
         # find the desired part of the point cloud
         block_start_indices_cuda = cuda.to_device(
             np.cumsum(np.concatenate(([0], block_sizes[:-1])))
         )
 
-        # this mutex is needed to make sure that only one thread writes to the mask
-        mask_mutex = cuda.to_device(np.zeros(blocks_number, dtype=np.int32))
-
         # call the kernel
-        self.__ransac_kernel[blocks_number, self.__threads_per_block](
+        self.__kernel[blocks_number, self.__threads_per_block](
             point_cloud_cuda,
             block_sizes_cuda,
             block_start_indices_cuda,
+            self.__random_hypotheses_cuda,
             self.__threshold,
-            self.__rng_states,
             result_mask_cuda,
-            max_inliers_number_cuda,
-            mask_mutex,
         )
 
         # copy result mask back to the host
         result_mask = result_mask_cuda.copy_to_host()
         return result_mask
 
     @staticmethod
-    @cuda.jit
-    def __ransac_kernel(
-        point_cloud: PointCloud,
-        block_sizes: npt.NDArray,
-        block_start_indices: npt.NDArray,
-        threshold: float,
-        rng_states,
-        result_mask: npt.NDArray,
-        max_inliers_number: npt.NDArray,
-        mask_mutex: npt.NDArray,
-    ):
-        thread_id, block_id = cuda.threadIdx.x, cuda.blockIdx.x
+    def __get_kernel(initial_points_number):
+        @cuda.jit
+        def kernel(
+            point_cloud: PointCloud,
+            block_sizes: npt.NDArray,
+            block_start_indices: npt.NDArray,
+            random_hypotheses: npt.NDArray,
+            threshold: float,
+            result_mask: npt.NDArray,
+        ):
+            thread_id, block_id = cuda.threadIdx.x, cuda.blockIdx.x
 
-        if block_sizes[block_id] < INITIAL_POINTS_NUMBER:
-            return
+            if block_sizes[block_id] < initial_points_number:
+                return
 
-        # select random points as inliers
-        initial_point_indices = cuda.local.array(
-            shape=INITIAL_POINTS_NUMBER, dtype=nb.size_t
-        )
-        initial_point_indices = generate_random_indices(
-            initial_point_indices,
-            rng_states,
-            block_sizes[block_id],
-            INITIAL_POINTS_NUMBER,
-        )
-        for i in range(INITIAL_POINTS_NUMBER):
-            initial_point_indices[i] = (
-                block_start_indices[block_id] + initial_point_indices[i]
+            # select random points as inliers
+            initial_point_indices = cuda.local.array(
+                shape=initial_points_number, dtype=nb.size_t
+            )
+            for i in range(initial_points_number):
+                initial_point_indices[i] = nb.int32(
+                    random_hypotheses[thread_id][i] * block_sizes[block_id]
+                    + block_start_indices[block_id]
+                )
+
+            # calculate the plane coefficients
+            plane = cuda.local.array(shape=4, dtype=nb.float32)
+            plane[0], plane[1], plane[2], plane[3] = get_plane_from_points(
+                point_cloud, initial_point_indices
             )
 
-        # calculate the plane coefficients
-        plane = cuda.local.array(shape=4, dtype=nb.float32)
-        plane[0], plane[1], plane[2], plane[3] = get_plane_from_points(
-            point_cloud, initial_point_indices
-        )
-
-        # for each point in the block check if it is an inlier
-        inliers_number_local = 0
-        for i in range(block_sizes[block_id]):
-            point = point_cloud[block_start_indices[block_id] + i]
-            distance = measure_distance(plane, point)
-            if distance < threshold:
-                inliers_number_local += 1
-
-        # replace the maximum number of inliers if the current number is greater
-        cuda.atomic.max(max_inliers_number, block_id, inliers_number_local)
-        cuda.syncthreads()
-        # set the best mask index for this block
-        # if this thread has the maximum number of inliers
-        if (
-            inliers_number_local == max_inliers_number[block_id]
-            and cuda.atomic.cas(mask_mutex, block_id, 0, 1) == 0
-        ):
+            # for each point in the block check if it is an inlier
+            inliers_number_local = 0
             for i in range(block_sizes[block_id]):
-                if (
-                    measure_distance(
-                        plane, point_cloud[block_start_indices[block_id] + i]
-                    )
-                    < threshold
-                ):
-                    result_mask[block_start_indices[block_id] + i] = True
+                point = point_cloud[block_start_indices[block_id] + i]
+                distance = measure_distance(plane, point)
+                if distance < threshold:
+                    inliers_number_local += 1
+
+            # shared memory to store the best plane and the maximum number of inliers
+            # for all hypotheses
+            best_plane = cuda.shared.array(shape=4, dtype=nb.float32)
+            max_inliers_number = cuda.shared.array(shape=1, dtype=nb.int32)
+            # this mutex is needed to make sure that only one thread writes the best plane
+            mutex = cuda.shared.array(shape=1, dtype=nb.int32)
+            if thread_id == 0:
+                max_inliers_number[0] = 0
+                mutex[0] = 0
+            cuda.syncthreads()
+
+            # replace the maximum number of inliers if the current number is greater
+            cuda.atomic.max(max_inliers_number, 0, inliers_number_local)
+
+            # if this thread has the maximum number of inliers
+            # write this thread's plane to the shared memory
+            cuda.syncthreads()
+            if (
+                inliers_number_local == max_inliers_number[0]
+                and cuda.atomic.compare_and_swap(mutex, 0, 1) == 0
+            ):
+                for i in range(4):
+                    best_plane[i] = plane[i]
+            cuda.syncthreads()
+
+            # parallelize final mask computation among threads in the block
+            for i in range(
+                block_start_indices[block_id] + thread_id,
+                block_start_indices[block_id] + block_sizes[block_id],
+                CUDA_THREADS,
+            ):
+                if measure_distance(best_plane, point_cloud[i]) < threshold:
+                    result_mask[i] = True
+
+        return kernel
```

### Comparing `octreelib-0.0.7/pyproject.toml` & `octreelib-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "octreelib"
-version = "0.0.7"
+version = "0.0.8"
 description = "Library for representing point clouds as OcTrees in SLAM"
 authors = [
   "Kiselyov Mikhail <kiselev.0353@gmail.com>",
   "Pavel Mokeev <pav3l.mokeev@gmail.com>"
 ]
 license = "APACHE"
 readme = "README.md"
```

### Comparing `octreelib-0.0.7/PKG-INFO` & `octreelib-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octreelib
-Version: 0.0.7
+Version: 0.0.8
 Summary: Library for representing point clouds as OcTrees in SLAM
 Home-page: https://github.com/prime-slam/
 License: APACHE
 Author: Kiselyov Mikhail
 Author-email: kiselev.0353@gmail.com
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: Intended Audience :: Developers
```

