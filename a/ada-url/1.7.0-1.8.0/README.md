# Comparing `tmp/ada-url-1.7.0.tar.gz` & `tmp/ada-url-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ada-url-1.7.0.tar", last modified: Mon Oct 23 15:45:42 2023, max compression
+gzip compressed data, was "ada-url-1.8.0.tar", last modified: Tue Nov 14 15:26:18 2023, max compression
```

## Comparing `ada-url-1.7.0.tar` & `ada-url-1.8.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 15:45:42.278805 ada-url-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2023-10-23 15:45:28.000000 ada-url-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4064 2023-10-23 15:45:42.278805 ada-url-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2023-10-23 15:45:28.000000 ada-url-1.7.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 15:45:42.274805 ada-url-1.7.0/ada_url/
--rw-r--r--   0 runner    (1001) docker     (127)      563 2023-10-23 15:45:28.000000 ada-url-1.7.0/ada_url/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   865185 2023-10-23 15:45:28.000000 ada-url-1.7.0/ada_url/ada.cpp
--rw-r--r--   0 runner    (1001) docker     (127)   253475 2023-10-23 15:45:28.000000 ada-url-1.7.0/ada_url/ada.h
--rw-r--r--   0 runner    (1001) docker     (127)    21641 2023-10-23 15:45:28.000000 ada-url-1.7.0/ada_url/ada_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2023-10-23 15:45:28.000000 ada-url-1.7.0/ada_url/ada_build.py
--rw-r--r--   0 runner    (1001) docker     (127)     7226 2023-10-23 15:45:28.000000 ada-url-1.7.0/ada_url/ada_c.h
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-23 15:45:28.000000 ada-url-1.7.0/ada_url/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 15:45:42.274805 ada-url-1.7.0/ada_url.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4064 2023-10-23 15:45:42.000000 ada-url-1.7.0/ada_url.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      355 2023-10-23 15:45:42.000000 ada-url-1.7.0/ada_url.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-23 15:45:42.000000 ada-url-1.7.0/ada_url.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-10-23 15:45:42.000000 ada-url-1.7.0/ada_url.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-10-23 15:45:42.000000 ada-url-1.7.0/ada_url.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      704 2023-10-23 15:45:28.000000 ada-url-1.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      873 2023-10-23 15:45:42.278805 ada-url-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      111 2023-10-23 15:45:28.000000 ada-url-1.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 15:45:42.278805 ada-url-1.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    21009 2023-10-23 15:45:28.000000 ada-url-1.7.0/tests/test_ada_url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 15:26:18.068654 ada-url-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2023-11-14 15:26:08.000000 ada-url-1.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4101 2023-11-14 15:26:18.068654 ada-url-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3600 2023-11-14 15:26:08.000000 ada-url-1.8.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 15:26:18.068654 ada-url-1.8.0/ada_url/
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2023-11-14 15:26:08.000000 ada-url-1.8.0/ada_url/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   870680 2023-11-14 15:26:08.000000 ada-url-1.8.0/ada_url/ada.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)   253189 2023-11-14 15:26:08.000000 ada-url-1.8.0/ada_url/ada.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21760 2023-11-14 15:26:08.000000 ada-url-1.8.0/ada_url/ada_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2023-11-14 15:26:08.000000 ada-url-1.8.0/ada_url/ada_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7226 2023-11-14 15:26:08.000000 ada-url-1.8.0/ada_url/ada_c.h
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-14 15:26:08.000000 ada-url-1.8.0/ada_url/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 15:26:18.068654 ada-url-1.8.0/ada_url.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4101 2023-11-14 15:26:18.000000 ada-url-1.8.0/ada_url.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2023-11-14 15:26:18.000000 ada-url-1.8.0/ada_url.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-14 15:26:18.000000 ada-url-1.8.0/ada_url.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2023-11-14 15:26:18.000000 ada-url-1.8.0/ada_url.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2023-11-14 15:26:18.000000 ada-url-1.8.0/ada_url.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2023-11-14 15:26:08.000000 ada-url-1.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2023-11-14 15:26:18.068654 ada-url-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2023-11-14 15:26:08.000000 ada-url-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 15:26:18.068654 ada-url-1.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    21009 2023-11-14 15:26:08.000000 ada-url-1.8.0/tests/test_ada_url.py
```

### Comparing `ada-url-1.7.0/LICENSE` & `ada-url-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ada-url-1.7.0/PKG-INFO` & `ada-url-1.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ada-url
-Version: 1.7.0
+Version: 1.8.0
 Summary: 'URL parser and manipulator based on the WHAT WG URL standard'
 Author: Bo Bayles
 Author-email: bo@bbayles.com
 License: Apache 2.0
 Project-URL: homepage, https://github.com/ada-url/ada-python
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -77,15 +77,15 @@
 
 .. code-block:: python
 
     >>> from ada_url import URL
     >>> urlobj = URL('https://example.org/path/../file.txt')
     >>> urlobj.host = 'example.com'
     >>> urlobj.href
-    'https://example.com/path/file.txt'
+    'https://example.com/file.txt'
 
 Replacing URL components with the ``replace_url`` function:
 
     >>> from ada_url import replace_url
     >>> replace_url('https://example.org/path/../file.txt', host='example.com')
     'https://example.com/file.txt'
 
@@ -140,12 +140,12 @@
     '/path2/'
 
 Contrast that with the Python standard library's ``urlib.parse`` module:
 
 .. code-block:: python
 
     >>> from urllib.parse import urlparse
-    >>> parsed_url = urlparse()
+    >>> parsed_url = urlparse('https://www.GOoglé.com/./path/../path2/')
     >>> parsed_url.hostname
     'www.googlé.com'
     >>> parsed_url.path
     '/./path/../path2/'
```

### Comparing `ada-url-1.7.0/README.rst` & `ada-url-1.8.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
 .. code-block:: python
 
     >>> from ada_url import URL
     >>> urlobj = URL('https://example.org/path/../file.txt')
     >>> urlobj.host = 'example.com'
     >>> urlobj.href
-    'https://example.com/path/file.txt'
+    'https://example.com/file.txt'
 
 Replacing URL components with the ``replace_url`` function:
 
     >>> from ada_url import replace_url
     >>> replace_url('https://example.org/path/../file.txt', host='example.com')
     'https://example.com/file.txt'
 
@@ -125,12 +125,12 @@
     '/path2/'
 
 Contrast that with the Python standard library's ``urlib.parse`` module:
 
 .. code-block:: python
 
     >>> from urllib.parse import urlparse
-    >>> parsed_url = urlparse()
+    >>> parsed_url = urlparse('https://www.GOoglé.com/./path/../path2/')
     >>> parsed_url.hostname
     'www.googlé.com'
     >>> parsed_url.path
     '/./path/../path2/'
```

### Comparing `ada-url-1.7.0/ada_url/__init__.py` & `ada-url-1.8.0/ada_url/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from ada_url.ada_adapter import (
+    URL,
     HostType,
     SchemeType,
-    URL,
     URLSearchParams,
     check_url,
     idna,
     idna_to_ascii,
     idna_to_unicode,
     join_url,
     normalize_url,
```

### Comparing `ada-url-1.7.0/ada_url/ada.cpp` & `ada-url-1.8.0/ada_url/ada.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* auto-generated on 2023-10-22 19:50:50 -0400. Do not edit! */
+/* auto-generated on 2023-11-09 19:39:05 -0500. Do not edit! */
 /* begin file src/ada.cpp */
 #include "ada.h"
 /* begin file src/checkers.cpp */
 #include <algorithm>
 
 namespace ada::checkers {
 
@@ -10613,163 +10613,300 @@
 }
 
 ada_really_inline void resize(std::string_view& input, size_t pos) noexcept {
   ADA_ASSERT_TRUE(pos <= input.size());
   input.remove_suffix(input.size() - pos);
 }
 
-// Reverse the byte order.
-ada_really_inline uint64_t swap_bytes(uint64_t val) noexcept {
-  // performance: this often compiles to a single instruction (e.g., bswap)
-  return ((((val)&0xff00000000000000ull) >> 56) |
-          (((val)&0x00ff000000000000ull) >> 40) |
-          (((val)&0x0000ff0000000000ull) >> 24) |
-          (((val)&0x000000ff00000000ull) >> 8) |
-          (((val)&0x00000000ff000000ull) << 8) |
-          (((val)&0x0000000000ff0000ull) << 24) |
-          (((val)&0x000000000000ff00ull) << 40) |
-          (((val)&0x00000000000000ffull) << 56));
-}
-
-ada_really_inline uint64_t swap_bytes_if_big_endian(uint64_t val) noexcept {
-  // performance: under little-endian systems (most systems), this function
-  // is free (just returns the input).
-#if ADA_IS_BIG_ENDIAN
-  return swap_bytes(val);
-#else
-  return val;  // unchanged (trivial)
-#endif
+// computes the number of trailing zeroes
+// this is a private inline function only defined in this source file.
+ada_really_inline int trailing_zeroes(uint32_t input_num) noexcept {
+#ifdef ADA_REGULAR_VISUAL_STUDIO
+  unsigned long ret;
+  // Search the mask data from least significant bit (LSB)
+  // to the most significant bit (MSB) for a set bit (1).
+  _BitScanForward(&ret, input_num);
+  return (int)ret;
+#else   // ADA_REGULAR_VISUAL_STUDIO
+  return __builtin_ctzl(input_num);
+#endif  // ADA_REGULAR_VISUAL_STUDIO
 }
 
 // starting at index location, this finds the next location of a character
 // :, /, \\, ? or [. If none is found, view.size() is returned.
 // For use within get_host_delimiter_location.
+#if ADA_NEON
 ada_really_inline size_t find_next_host_delimiter_special(
     std::string_view view, size_t location) noexcept {
-  // performance: if you plan to call find_next_host_delimiter more than once,
-  // you *really* want find_next_host_delimiter to be inlined, because
-  // otherwise, the constants may get reloaded each time (bad).
-  auto has_zero_byte = [](uint64_t v) {
-    return ((v - 0x0101010101010101) & ~(v)&0x8080808080808080);
-  };
-  auto index_of_first_set_byte = [](uint64_t v) {
-    return ((((v - 1) & 0x101010101010101) * 0x101010101010101) >> 56) - 1;
-  };
-  auto broadcast = [](uint8_t v) -> uint64_t {
-    return 0x101010101010101ull * v;
+  // first check for short strings in which case we do it naively.
+  if (view.size() - location < 16) {  // slow path
+    for (size_t i = location; i < view.size(); i++) {
+      if (view[i] == ':' || view[i] == '/' || view[i] == '\\' ||
+          view[i] == '?' || view[i] == '[') {
+        return i;
+      }
+    }
+    return size_t(view.size());
+  }
+  auto to_bitmask = [](uint8x16_t input) -> uint16_t {
+    uint8x16_t bit_mask = {0x01, 0x02, 0x4, 0x8, 0x10, 0x20, 0x40, 0x80,
+                           0x01, 0x02, 0x4, 0x8, 0x10, 0x20, 0x40, 0x80};
+    uint8x16_t minput = vandq_u8(input, bit_mask);
+    uint8x16_t tmp = vpaddq_u8(minput, minput);
+    tmp = vpaddq_u8(tmp, tmp);
+    tmp = vpaddq_u8(tmp, tmp);
+    return vgetq_lane_u16(vreinterpretq_u16_u8(tmp), 0);
   };
+
+  // fast path for long strings (expected to be common)
   size_t i = location;
-  uint64_t mask1 = broadcast(':');
-  uint64_t mask2 = broadcast('/');
-  uint64_t mask3 = broadcast('\\');
-  uint64_t mask4 = broadcast('?');
-  uint64_t mask5 = broadcast('[');
-  // This loop will get autovectorized under many optimizing compilers,
-  // so you get actually SIMD!
-  for (; i + 7 < view.size(); i += 8) {
-    uint64_t word{};
-    // performance: the next memcpy translates into a single CPU instruction.
-    memcpy(&word, view.data() + i, sizeof(word));
-    // performance: on little-endian systems (most systems), this next line is
-    // free.
-    word = swap_bytes_if_big_endian(word);
-    uint64_t xor1 = word ^ mask1;
-    uint64_t xor2 = word ^ mask2;
-    uint64_t xor3 = word ^ mask3;
-    uint64_t xor4 = word ^ mask4;
-    uint64_t xor5 = word ^ mask5;
-    uint64_t is_match = has_zero_byte(xor1) | has_zero_byte(xor2) |
-                        has_zero_byte(xor3) | has_zero_byte(xor4) |
-                        has_zero_byte(xor5);
-    if (is_match) {
-      return size_t(i + index_of_first_set_byte(is_match));
+  uint8x16_t low_mask = {0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00,
+                         0x00, 0x00, 0x01, 0x04, 0x04, 0x00, 0x00, 0x03};
+  uint8x16_t high_mask = {0x00, 0x00, 0x02, 0x01, 0x00, 0x04, 0x00, 0x00,
+                          0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00};
+  uint8x16_t fmask = vmovq_n_u8(0xf);
+  uint8x16_t zero{0};
+  for (; i + 15 < view.size(); i += 16) {
+    uint8x16_t word = vld1q_u8((const uint8_t*)view.data() + i);
+    uint8x16_t lowpart = vqtbl1q_u8(low_mask, vandq_u8(word, fmask));
+    uint8x16_t highpart = vqtbl1q_u8(high_mask, vshrq_n_u8(word, 4));
+    uint8x16_t classify = vandq_u8(lowpart, highpart);
+    if (vmaxvq_u8(classify) != 0) {
+      uint8x16_t is_zero = vceqq_u8(classify, zero);
+      uint16_t is_non_zero = ~to_bitmask(is_zero);
+      return i + trailing_zeroes(is_non_zero);
     }
   }
+
   if (i < view.size()) {
-    uint64_t word{};
-    // performance: the next memcpy translates into a function call, but
-    // that is difficult to avoid. Might be a bit expensive.
-    memcpy(&word, view.data() + i, view.size() - i);
-    word = swap_bytes_if_big_endian(word);
-    uint64_t xor1 = word ^ mask1;
-    uint64_t xor2 = word ^ mask2;
-    uint64_t xor3 = word ^ mask3;
-    uint64_t xor4 = word ^ mask4;
-    uint64_t xor5 = word ^ mask5;
-    uint64_t is_match = has_zero_byte(xor1) | has_zero_byte(xor2) |
-                        has_zero_byte(xor3) | has_zero_byte(xor4) |
-                        has_zero_byte(xor5);
-    if (is_match) {
-      return size_t(i + index_of_first_set_byte(is_match));
+    uint8x16_t word =
+        vld1q_u8((const uint8_t*)view.data() + view.length() - 16);
+    uint8x16_t lowpart = vqtbl1q_u8(low_mask, vandq_u8(word, fmask));
+    uint8x16_t highpart = vqtbl1q_u8(high_mask, vshrq_n_u8(word, 4));
+    uint8x16_t classify = vandq_u8(lowpart, highpart);
+    if (vmaxvq_u8(classify) != 0) {
+      uint8x16_t is_zero = vceqq_u8(classify, zero);
+      uint16_t is_non_zero = ~to_bitmask(is_zero);
+      return view.length() - 16 + trailing_zeroes(is_non_zero);
+    }
+  }
+  return size_t(view.size());
+}
+#elif ADA_SSE2
+ada_really_inline size_t find_next_host_delimiter_special(
+    std::string_view view, size_t location) noexcept {
+  // first check for short strings in which case we do it naively.
+  if (view.size() - location < 16) {  // slow path
+    for (size_t i = location; i < view.size(); i++) {
+      if (view[i] == ':' || view[i] == '/' || view[i] == '\\' ||
+          view[i] == '?' || view[i] == '[') {
+        return i;
+      }
+    }
+    return size_t(view.size());
+  }
+  // fast path for long strings (expected to be common)
+  size_t i = location;
+  const __m128i mask1 = _mm_set1_epi8(':');
+  const __m128i mask2 = _mm_set1_epi8('/');
+  const __m128i mask3 = _mm_set1_epi8('\\');
+  const __m128i mask4 = _mm_set1_epi8('?');
+  const __m128i mask5 = _mm_set1_epi8('[');
+
+  for (; i + 15 < view.size(); i += 16) {
+    __m128i word = _mm_loadu_si128((const __m128i*)(view.data() + i));
+    __m128i m1 = _mm_cmpeq_epi8(word, mask1);
+    __m128i m2 = _mm_cmpeq_epi8(word, mask2);
+    __m128i m3 = _mm_cmpeq_epi8(word, mask3);
+    __m128i m4 = _mm_cmpeq_epi8(word, mask4);
+    __m128i m5 = _mm_cmpeq_epi8(word, mask5);
+    __m128i m = _mm_or_si128(
+        _mm_or_si128(_mm_or_si128(m1, m2), _mm_or_si128(m3, m4)), m5);
+    int mask = _mm_movemask_epi8(m);
+    if (mask != 0) {
+      return i + trailing_zeroes(mask);
+    }
+  }
+  if (i < view.size()) {
+    __m128i word =
+        _mm_loadu_si128((const __m128i*)(view.data() + view.length() - 16));
+    __m128i m1 = _mm_cmpeq_epi8(word, mask1);
+    __m128i m2 = _mm_cmpeq_epi8(word, mask2);
+    __m128i m3 = _mm_cmpeq_epi8(word, mask3);
+    __m128i m4 = _mm_cmpeq_epi8(word, mask4);
+    __m128i m5 = _mm_cmpeq_epi8(word, mask5);
+    __m128i m = _mm_or_si128(
+        _mm_or_si128(_mm_or_si128(m1, m2), _mm_or_si128(m3, m4)), m5);
+    int mask = _mm_movemask_epi8(m);
+    if (mask != 0) {
+      return view.length() - 16 + trailing_zeroes(mask);
     }
   }
-  return view.size();
+  return size_t(view.length());
 }
+#else
+// : / [ \\ ?
+static constexpr bool special_host_delimiters[256] = {
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0};
+// credit: @the-moisrex recommended a table-based approach
+ada_really_inline size_t find_next_host_delimiter_special(
+    std::string_view view, size_t location) noexcept {
+  auto const str = view.substr(location);
+  for (auto pos = str.begin(); pos != str.end(); ++pos) {
+    if (special_host_delimiters[(uint8_t)*pos]) {
+      return pos - str.begin() + location;
+    }
+  }
+  return size_t(view.size());
+}
+#endif
 
 // starting at index location, this finds the next location of a character
 // :, /, ? or [. If none is found, view.size() is returned.
 // For use within get_host_delimiter_location.
+#if ADA_NEON
 ada_really_inline size_t find_next_host_delimiter(std::string_view view,
                                                   size_t location) noexcept {
-  // performance: if you plan to call find_next_host_delimiter more than once,
-  // you *really* want find_next_host_delimiter to be inlined, because
-  // otherwise, the constants may get reloaded each time (bad).
-  auto has_zero_byte = [](uint64_t v) {
-    return ((v - 0x0101010101010101) & ~(v)&0x8080808080808080);
-  };
-  auto index_of_first_set_byte = [](uint64_t v) {
-    return ((((v - 1) & 0x101010101010101) * 0x101010101010101) >> 56) - 1;
-  };
-  auto broadcast = [](uint8_t v) -> uint64_t {
-    return 0x101010101010101ull * v;
+  // first check for short strings in which case we do it naively.
+  if (view.size() - location < 16) {  // slow path
+    for (size_t i = location; i < view.size(); i++) {
+      if (view[i] == ':' || view[i] == '/' || view[i] == '?' ||
+          view[i] == '[') {
+        return i;
+      }
+    }
+    return size_t(view.size());
+  }
+  auto to_bitmask = [](uint8x16_t input) -> uint16_t {
+    uint8x16_t bit_mask = {0x01, 0x02, 0x4, 0x8, 0x10, 0x20, 0x40, 0x80,
+                           0x01, 0x02, 0x4, 0x8, 0x10, 0x20, 0x40, 0x80};
+    uint8x16_t minput = vandq_u8(input, bit_mask);
+    uint8x16_t tmp = vpaddq_u8(minput, minput);
+    tmp = vpaddq_u8(tmp, tmp);
+    tmp = vpaddq_u8(tmp, tmp);
+    return vgetq_lane_u16(vreinterpretq_u16_u8(tmp), 0);
   };
+
+  // fast path for long strings (expected to be common)
   size_t i = location;
-  uint64_t mask1 = broadcast(':');
-  uint64_t mask2 = broadcast('/');
-  uint64_t mask4 = broadcast('?');
-  uint64_t mask5 = broadcast('[');
-  // This loop will get autovectorized under many optimizing compilers,
-  // so you get actually SIMD!
-  for (; i + 7 < view.size(); i += 8) {
-    uint64_t word{};
-    // performance: the next memcpy translates into a single CPU instruction.
-    memcpy(&word, view.data() + i, sizeof(word));
-    // performance: on little-endian systems (most systems), this next line is
-    // free.
-    word = swap_bytes_if_big_endian(word);
-    uint64_t xor1 = word ^ mask1;
-    uint64_t xor2 = word ^ mask2;
-    uint64_t xor4 = word ^ mask4;
-    uint64_t xor5 = word ^ mask5;
-    uint64_t is_match = has_zero_byte(xor1) | has_zero_byte(xor2) |
-                        has_zero_byte(xor4) | has_zero_byte(xor5);
-    if (is_match) {
-      return size_t(i + index_of_first_set_byte(is_match));
+  uint8x16_t low_mask = {0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00,
+                         0x00, 0x00, 0x01, 0x04, 0x00, 0x00, 0x00, 0x03};
+  uint8x16_t high_mask = {0x00, 0x00, 0x02, 0x01, 0x00, 0x04, 0x00, 0x00,
+                          0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00};
+  uint8x16_t fmask = vmovq_n_u8(0xf);
+  uint8x16_t zero{0};
+  for (; i + 15 < view.size(); i += 16) {
+    uint8x16_t word = vld1q_u8((const uint8_t*)view.data() + i);
+    uint8x16_t lowpart = vqtbl1q_u8(low_mask, vandq_u8(word, fmask));
+    uint8x16_t highpart = vqtbl1q_u8(high_mask, vshrq_n_u8(word, 4));
+    uint8x16_t classify = vandq_u8(lowpart, highpart);
+    if (vmaxvq_u8(classify) != 0) {
+      uint8x16_t is_zero = vceqq_u8(classify, zero);
+      uint16_t is_non_zero = ~to_bitmask(is_zero);
+      return i + trailing_zeroes(is_non_zero);
     }
   }
+
   if (i < view.size()) {
-    uint64_t word{};
-    // performance: the next memcpy translates into a function call, but
-    // that is difficult to avoid. Might be a bit expensive.
-    memcpy(&word, view.data() + i, view.size() - i);
-    // performance: on little-endian systems (most systems), this next line is
-    // free.
-    word = swap_bytes_if_big_endian(word);
-    uint64_t xor1 = word ^ mask1;
-    uint64_t xor2 = word ^ mask2;
-    uint64_t xor4 = word ^ mask4;
-    uint64_t xor5 = word ^ mask5;
-    uint64_t is_match = has_zero_byte(xor1) | has_zero_byte(xor2) |
-                        has_zero_byte(xor4) | has_zero_byte(xor5);
-    if (is_match) {
-      return size_t(i + index_of_first_set_byte(is_match));
+    uint8x16_t word =
+        vld1q_u8((const uint8_t*)view.data() + view.length() - 16);
+    uint8x16_t lowpart = vqtbl1q_u8(low_mask, vandq_u8(word, fmask));
+    uint8x16_t highpart = vqtbl1q_u8(high_mask, vshrq_n_u8(word, 4));
+    uint8x16_t classify = vandq_u8(lowpart, highpart);
+    if (vmaxvq_u8(classify) != 0) {
+      uint8x16_t is_zero = vceqq_u8(classify, zero);
+      uint16_t is_non_zero = ~to_bitmask(is_zero);
+      return view.length() - 16 + trailing_zeroes(is_non_zero);
     }
   }
-  return view.size();
+  return size_t(view.size());
 }
+#elif ADA_SSE2
+ada_really_inline size_t find_next_host_delimiter(std::string_view view,
+                                                  size_t location) noexcept {
+  // first check for short strings in which case we do it naively.
+  if (view.size() - location < 16) {  // slow path
+    for (size_t i = location; i < view.size(); i++) {
+      if (view[i] == ':' || view[i] == '/' || view[i] == '?' ||
+          view[i] == '[') {
+        return i;
+      }
+    }
+    return size_t(view.size());
+  }
+  // fast path for long strings (expected to be common)
+  size_t i = location;
+  const __m128i mask1 = _mm_set1_epi8(':');
+  const __m128i mask2 = _mm_set1_epi8('/');
+  const __m128i mask4 = _mm_set1_epi8('?');
+  const __m128i mask5 = _mm_set1_epi8('[');
+
+  for (; i + 15 < view.size(); i += 16) {
+    __m128i word = _mm_loadu_si128((const __m128i*)(view.data() + i));
+    __m128i m1 = _mm_cmpeq_epi8(word, mask1);
+    __m128i m2 = _mm_cmpeq_epi8(word, mask2);
+    __m128i m4 = _mm_cmpeq_epi8(word, mask4);
+    __m128i m5 = _mm_cmpeq_epi8(word, mask5);
+    __m128i m = _mm_or_si128(_mm_or_si128(m1, m2), _mm_or_si128(m4, m5));
+    int mask = _mm_movemask_epi8(m);
+    if (mask != 0) {
+      return i + trailing_zeroes(mask);
+    }
+  }
+  if (i < view.size()) {
+    __m128i word =
+        _mm_loadu_si128((const __m128i*)(view.data() + view.length() - 16));
+    __m128i m1 = _mm_cmpeq_epi8(word, mask1);
+    __m128i m2 = _mm_cmpeq_epi8(word, mask2);
+    __m128i m4 = _mm_cmpeq_epi8(word, mask4);
+    __m128i m5 = _mm_cmpeq_epi8(word, mask5);
+    __m128i m = _mm_or_si128(_mm_or_si128(m1, m2), _mm_or_si128(m4, m5));
+    int mask = _mm_movemask_epi8(m);
+    if (mask != 0) {
+      return view.length() - 16 + trailing_zeroes(mask);
+    }
+  }
+  return size_t(view.length());
+}
+#else
+// : / [ ?
+static constexpr bool host_delimiters[256] = {
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0};
+// credit: @the-moisrex recommended a table-based approach
+ada_really_inline size_t find_next_host_delimiter(std::string_view view,
+                                                  size_t location) noexcept {
+  auto const str = view.substr(location);
+  for (auto pos = str.begin(); pos != str.end(); ++pos) {
+    if (host_delimiters[(uint8_t)*pos]) {
+      return pos - str.begin() + location;
+    }
+  }
+  return size_t(view.size());
+}
+#endif
 
 ada_really_inline std::pair<size_t, bool> get_host_delimiter_location(
     const bool is_special, std::string_view& view) noexcept {
   /**
    * The spec at https://url.spec.whatwg.org/#hostname-state expects us to
    * compute a variable called insideBrackets but this variable is only used
    * once, to check whether a ':' character was found outside brackets. Exact
@@ -11036,109 +11173,64 @@
   auto path = std::string(url.get_pathname());
   while (!path.empty() && path.back() == ' ') {
     path.resize(path.size() - 1);
   }
   url.update_base_pathname(path);
 }
 
+// @ / \\ ?
+static constexpr bool authority_delimiter_special[256] = {
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0};
+// credit: @the-moisrex recommended a table-based approach
 ada_really_inline size_t
 find_authority_delimiter_special(std::string_view view) noexcept {
-  auto has_zero_byte = [](uint64_t v) {
-    return ((v - 0x0101010101010101) & ~(v)&0x8080808080808080);
-  };
-  auto index_of_first_set_byte = [](uint64_t v) {
-    return ((((v - 1) & 0x101010101010101) * 0x101010101010101) >> 56) - 1;
-  };
-  auto broadcast = [](uint8_t v) -> uint64_t {
-    return 0x101010101010101ull * v;
-  };
-  size_t i = 0;
-  uint64_t mask1 = broadcast('@');
-  uint64_t mask2 = broadcast('/');
-  uint64_t mask3 = broadcast('?');
-  uint64_t mask4 = broadcast('\\');
-
-  for (; i + 7 < view.size(); i += 8) {
-    uint64_t word{};
-    memcpy(&word, view.data() + i, sizeof(word));
-    word = swap_bytes_if_big_endian(word);
-    uint64_t xor1 = word ^ mask1;
-    uint64_t xor2 = word ^ mask2;
-    uint64_t xor3 = word ^ mask3;
-    uint64_t xor4 = word ^ mask4;
-    uint64_t is_match = has_zero_byte(xor1) | has_zero_byte(xor2) |
-                        has_zero_byte(xor3) | has_zero_byte(xor4);
-    if (is_match) {
-      return size_t(i + index_of_first_set_byte(is_match));
+  // performance note: we might be able to gain further performance
+  // with SIMD instrinsics.
+  for (auto pos = view.begin(); pos != view.end(); ++pos) {
+    if (authority_delimiter_special[(uint8_t)*pos]) {
+      return pos - view.begin();
     }
   }
-
-  if (i < view.size()) {
-    uint64_t word{};
-    memcpy(&word, view.data() + i, view.size() - i);
-    word = swap_bytes_if_big_endian(word);
-    uint64_t xor1 = word ^ mask1;
-    uint64_t xor2 = word ^ mask2;
-    uint64_t xor3 = word ^ mask3;
-    uint64_t xor4 = word ^ mask4;
-    uint64_t is_match = has_zero_byte(xor1) | has_zero_byte(xor2) |
-                        has_zero_byte(xor3) | has_zero_byte(xor4);
-    if (is_match) {
-      return size_t(i + index_of_first_set_byte(is_match));
-    }
-  }
-
-  return view.size();
+  return size_t(view.size());
 }
 
+// @ / ?
+static constexpr bool authority_delimiter[256] = {
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+    0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0};
+// credit: @the-moisrex recommended a table-based approach
 ada_really_inline size_t
 find_authority_delimiter(std::string_view view) noexcept {
-  auto has_zero_byte = [](uint64_t v) {
-    return ((v - 0x0101010101010101) & ~(v)&0x8080808080808080);
-  };
-  auto index_of_first_set_byte = [](uint64_t v) {
-    return ((((v - 1) & 0x101010101010101) * 0x101010101010101) >> 56) - 1;
-  };
-  auto broadcast = [](uint8_t v) -> uint64_t {
-    return 0x101010101010101ull * v;
-  };
-  size_t i = 0;
-  uint64_t mask1 = broadcast('@');
-  uint64_t mask2 = broadcast('/');
-  uint64_t mask3 = broadcast('?');
-
-  for (; i + 7 < view.size(); i += 8) {
-    uint64_t word{};
-    memcpy(&word, view.data() + i, sizeof(word));
-    word = swap_bytes_if_big_endian(word);
-    uint64_t xor1 = word ^ mask1;
-    uint64_t xor2 = word ^ mask2;
-    uint64_t xor3 = word ^ mask3;
-    uint64_t is_match =
-        has_zero_byte(xor1) | has_zero_byte(xor2) | has_zero_byte(xor3);
-    if (is_match) {
-      return size_t(i + index_of_first_set_byte(is_match));
-    }
-  }
-
-  if (i < view.size()) {
-    uint64_t word{};
-    memcpy(&word, view.data() + i, view.size() - i);
-    word = swap_bytes_if_big_endian(word);
-    uint64_t xor1 = word ^ mask1;
-    uint64_t xor2 = word ^ mask2;
-    uint64_t xor3 = word ^ mask3;
-    uint64_t is_match =
-        has_zero_byte(xor1) | has_zero_byte(xor2) | has_zero_byte(xor3);
-    if (is_match) {
-      return size_t(i + index_of_first_set_byte(is_match));
+  // performance note: we might be able to gain further performance
+  // with SIMD instrinsics.
+  for (auto pos = view.begin(); pos != view.end(); ++pos) {
+    if (authority_delimiter[(uint8_t)*pos]) {
+      return pos - view.begin();
     }
   }
-
-  return view.size();
+  return size_t(view.size());
 }
 
 }  // namespace ada::helpers
 
 namespace ada {
 ada_warn_unused std::string to_string(ada::state state) {
   return ada::helpers::get_state(state);
```

### Comparing `ada-url-1.7.0/ada_url/ada.h` & `ada-url-1.8.0/ada_url/ada.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* auto-generated on 2023-10-22 19:50:50 -0400. Do not edit! */
+/* auto-generated on 2023-11-09 19:39:05 -0500. Do not edit! */
 /* begin file include/ada.h */
 /**
  * @file ada.h
  * @brief Includes all definitions for Ada.
  */
 #ifndef ADA_H
 #define ADA_H
@@ -1668,26 +1668,14 @@
  */
 template <class url_type>
 ada_really_inline void strip_trailing_spaces_from_opaque_path(
     url_type& url) noexcept;
 
 /**
  * @private
- * Reverse the order of the bytes.
- */
-ada_really_inline uint64_t swap_bytes(uint64_t val) noexcept;
-
-/**
- * @private
- * Reverse the order of the bytes but only if the system is big endian
- */
-ada_really_inline uint64_t swap_bytes_if_big_endian(uint64_t val) noexcept;
-
-/**
- * @private
  * Finds the delimiter of a view in authority state.
  */
 ada_really_inline size_t
 find_authority_delimiter_special(std::string_view view) noexcept;
 
 /**
  * @private
@@ -7084,22 +7072,22 @@
 /**
  * @file ada_version.h
  * @brief Definitions for Ada's version number.
  */
 #ifndef ADA_ADA_VERSION_H
 #define ADA_ADA_VERSION_H
 
-#define ADA_VERSION "2.7.2"
+#define ADA_VERSION "2.7.3"
 
 namespace ada {
 
 enum {
   ADA_VERSION_MAJOR = 2,
   ADA_VERSION_MINOR = 7,
-  ADA_VERSION_REVISION = 2,
+  ADA_VERSION_REVISION = 3,
 };
 
 }  // namespace ada
 
 #endif  // ADA_ADA_VERSION_H
 /* end file include/ada/ada_version.h */
 /* begin file include/ada/implementation.h */
```

### Comparing `ada-url-1.7.0/ada_url/ada_adapter.py` & `ada-url-1.8.0/ada_url/ada_adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 from enum import IntEnum
-from typing import Final, Iterable, Iterator, List, Optional, Tuple, TypedDict, Union
+from typing import (
+    Dict,
+    Final,
+    Iterable,
+    Iterator,
+    List,
+    Optional,
+    Tuple,
+    TypedDict,
+    Union,
+)
 
 from ada_url._ada_wrapper import ffi, lib
 
 URL_ATTRIBUTES = (
     'href',
     'username',
     'password',
@@ -345,14 +355,17 @@
             len(params_bytes),
         )
 
     @property
     def size(self) -> int:
         return lib.ada_search_params_size(self.paramsobj)
 
+    def __len__(self) -> int:
+        return self.size
+
     def append(self, key: str, value: str):
         key_bytes = key.encode('utf-8')
         value_bytes = value.encode('utf-8')
         lib.ada_search_params_append(
             self.paramsobj,
             key_bytes,
             len(key_bytes),
@@ -644,15 +657,15 @@
             set_result = set_func(urlobj, value_bytes, len(value_bytes))
             if (set_result is not None) and (not set_result):
                 raise ValueError(f'Invalid value for {attr}') from None
 
     return _get_str(lib.ada_get_href(urlobj))
 
 
-def parse_search_params(s: str) -> dict:
+def parse_search_params(s: str) -> Dict[str, List[str]]:
     """
     Returns a dictionary representing the parsed URL Parameters specified by *s*.
     The returned dictionary maps each key to a list of values associated with it.
 
     .. code-block:: python
 
         >>> from ada_url import parse_search_params
```

### Comparing `ada-url-1.7.0/ada_url/ada_build.py` & `ada-url-1.8.0/ada_url/ada_build.py`

 * *Files identical despite different names*

### Comparing `ada-url-1.7.0/ada_url/ada_c.h` & `ada-url-1.8.0/ada_url/ada_c.h`

 * *Files identical despite different names*

### Comparing `ada-url-1.7.0/ada_url.egg-info/PKG-INFO` & `ada-url-1.8.0/ada_url.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ada-url
-Version: 1.7.0
+Version: 1.8.0
 Summary: 'URL parser and manipulator based on the WHAT WG URL standard'
 Author: Bo Bayles
 Author-email: bo@bbayles.com
 License: Apache 2.0
 Project-URL: homepage, https://github.com/ada-url/ada-python
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -77,15 +77,15 @@
 
 .. code-block:: python
 
     >>> from ada_url import URL
     >>> urlobj = URL('https://example.org/path/../file.txt')
     >>> urlobj.host = 'example.com'
     >>> urlobj.href
-    'https://example.com/path/file.txt'
+    'https://example.com/file.txt'
 
 Replacing URL components with the ``replace_url`` function:
 
     >>> from ada_url import replace_url
     >>> replace_url('https://example.org/path/../file.txt', host='example.com')
     'https://example.com/file.txt'
 
@@ -140,12 +140,12 @@
     '/path2/'
 
 Contrast that with the Python standard library's ``urlib.parse`` module:
 
 .. code-block:: python
 
     >>> from urllib.parse import urlparse
-    >>> parsed_url = urlparse()
+    >>> parsed_url = urlparse('https://www.GOoglé.com/./path/../path2/')
     >>> parsed_url.hostname
     'www.googlé.com'
     >>> parsed_url.path
     '/./path/../path2/'
```

### Comparing `ada-url-1.7.0/setup.cfg` & `ada-url-1.8.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ada-url
-version = 1.7.0
+version = 1.8.0
 description = 'URL parser and manipulator based on the WHAT WG URL standard'
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Bo Bayles
 author_email = bo@bbayles.com
 license = Apache 2.0
 license_files =
```

### Comparing `ada-url-1.7.0/tests/test_ada_url.py` & `ada-url-1.8.0/tests/test_ada_url.py`

 * *Files identical despite different names*

