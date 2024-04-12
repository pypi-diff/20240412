# Comparing `tmp/nvremap-0.1.0-cp36-cp36m-manylinux1_x86_64.whl.zip` & `tmp/nvremap-0.1.1-cp36-cp36m-manylinux1_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 79384 bytes, number of entries: 6
--rwxr-xr-x  2.0 unx   210552 b- defN 24-Apr-12 03:59 nvremap.cpython-36m-x86_64-linux-gnu.so
--rw-r--r--  2.0 unx     1060 b- defN 24-Apr-12 03:59 nvremap-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      673 b- defN 24-Apr-12 03:59 nvremap-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx      109 b- defN 24-Apr-12 03:59 nvremap-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 24-Apr-12 03:59 nvremap-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      483 b- defN 24-Apr-12 03:59 nvremap-0.1.0.dist-info/RECORD
-6 files, 212885 bytes uncompressed, 78510 bytes compressed:  63.1%
+Zip file size: 79787 bytes, number of entries: 6
+-rwxr-xr-x  2.0 unx   210552 b- defN 24-Apr-12 06:32 nvremap.cpython-36m-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx     1060 b- defN 24-Apr-12 06:32 nvremap-0.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1558 b- defN 24-Apr-12 06:32 nvremap-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      109 b- defN 24-Apr-12 06:32 nvremap-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-Apr-12 06:32 nvremap-0.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      484 b- defN 24-Apr-12 06:32 nvremap-0.1.1.dist-info/RECORD
+6 files, 213771 bytes uncompressed, 78913 bytes compressed:  63.1%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: nvremap.cpython-36m-x86_64-linux-gnu.so
 Comment: 
 
-Filename: nvremap-0.1.0.dist-info/LICENSE
+Filename: nvremap-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: nvremap-0.1.0.dist-info/METADATA
+Filename: nvremap-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: nvremap-0.1.0.dist-info/WHEEL
+Filename: nvremap-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: nvremap-0.1.0.dist-info/top_level.txt
+Filename: nvremap-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: nvremap-0.1.0.dist-info/RECORD
+Filename: nvremap-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nvremap.cpython-36m-x86_64-linux-gnu.so

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

### readelf --wide --symbols {}

```diff
@@ -324,15 +324,15 @@
     57: 0000000000006b80     0 FUNC    LOCAL  DEFAULT   12 __do_global_dtors_aux
     58: 0000000000229660     1 OBJECT  LOCAL  DEFAULT   29 completed.7997
     59: 0000000000228a28     0 OBJECT  LOCAL  DEFAULT   22 __do_global_dtors_aux_fini_array_entry
     60: 0000000000006bc0     0 FUNC    LOCAL  DEFAULT   12 frame_dummy
     61: 0000000000228a18     0 OBJECT  LOCAL  DEFAULT   21 __frame_dummy_init_array_entry
     62: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS link.stub
     63: 000000000001b700     0 NOTYPE  LOCAL  DEFAULT   15 fatbinData
-    64: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS tmpxft_000088cf_00000000-6_remap_kernel.compute_86.cudafe1.cpp
+    64: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS tmpxft_0000a37d_00000000-6_remap_kernel.compute_86.cudafe1.cpp
     65: 00000000002297f8     1 OBJECT  LOCAL  DEFAULT   29 _ZL22__nv_inited_managed_rt
     66: 0000000000229800     8 OBJECT  LOCAL  DEFAULT   29 _ZL32__nv_fatbinhandle_for_managed_rt
     67: 0000000000018f72    22 FUNC    LOCAL  DEFAULT   12 _ZL37__nv_save_fatbinhandle_for_managed_rtPPv
     68: 0000000000229808     8 OBJECT  LOCAL  DEFAULT   29 _ZZL22____nv_dummy_param_refPvE5__ref
     69: 0000000000019084    22 FUNC    LOCAL  DEFAULT   12 _ZL22____nv_dummy_param_refPv
     70: 0000000000024098    15 OBJECT  LOCAL  DEFAULT   16 _ZL15__module_id_str
     71: 0000000000229810     8 OBJECT  LOCAL  DEFAULT   29 _ZL20__cudaFatCubinHandle
```

### strings --all --bytes=8 {}

```diff
@@ -645,15 +645,15 @@
 __do_global_dtors_aux
 completed.7997
 __do_global_dtors_aux_fini_array_entry
 frame_dummy
 __frame_dummy_init_array_entry
 link.stub
 fatbinData
-tmpxft_000088cf_00000000-6_remap_kernel.compute_86.cudafe1.cpp
+tmpxft_0000a37d_00000000-6_remap_kernel.compute_86.cudafe1.cpp
 _ZL22__nv_inited_managed_rt
 _ZL32__nv_fatbinhandle_for_managed_rt
 _ZL37__nv_save_fatbinhandle_for_managed_rtPPv
 _ZZL22____nv_dummy_param_refPvE5__ref
 _ZL22____nv_dummy_param_refPv
 _ZL15__module_id_str
 _ZL20__cudaFatCubinHandle
```

### readelf --wide --decompress --hex-dump=.strtab {}

```diff
@@ -160,15 +160,15 @@
   0x000009d0 65642e37 39393700 5f5f646f 5f676c6f ed.7997.__do_glo
   0x000009e0 62616c5f 64746f72 735f6175 785f6669 bal_dtors_aux_fi
   0x000009f0 6e695f61 72726179 5f656e74 72790066 ni_array_entry.f
   0x00000a00 72616d65 5f64756d 6d79005f 5f667261 rame_dummy.__fra
   0x00000a10 6d655f64 756d6d79 5f696e69 745f6172 me_dummy_init_ar
   0x00000a20 7261795f 656e7472 79006c69 6e6b2e73 ray_entry.link.s
   0x00000a30 74756200 66617462 696e4461 74610074 tub.fatbinData.t
-  0x00000a40 6d707866 745f3030 30303838 63665f30 mpxft_000088cf_0
+  0x00000a40 6d707866 745f3030 30306133 37645f30 mpxft_0000a37d_0
   0x00000a50 30303030 3030302d 365f7265 6d61705f 0000000-6_remap_
   0x00000a60 6b65726e 656c2e63 6f6d7075 74655f38 kernel.compute_8
   0x00000a70 362e6375 64616665 312e6370 70005f5a 6.cudafe1.cpp._Z
   0x00000a80 4c32325f 5f6e765f 696e6974 65645f6d L22__nv_inited_m
   0x00000a90 616e6167 65645f72 74005f5a 4c33325f anaged_rt._ZL32_
   0x00000aa0 5f6e765f 66617462 696e6861 6e646c65 _nv_fatbinhandle
   0x00000ab0 5f666f72 5f6d616e 61676564 5f727400 _for_managed_rt.
```

## Comparing `nvremap-0.1.0.dist-info/LICENSE` & `nvremap-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

