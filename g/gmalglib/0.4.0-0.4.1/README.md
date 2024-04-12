# Comparing `tmp/gmalglib-0.4.0.tar.gz` & `tmp/gmalglib-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmalglib-0.4.0.tar", last modified: Fri Apr 12 13:01:22 2024, max compression
+gzip compressed data, was "gmalglib-0.4.1.tar", last modified: Fri Apr 12 17:26:29 2024, max compression
```

## Comparing `gmalglib-0.4.0.tar` & `gmalglib-0.4.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:01:22.727690 gmalglib-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-12 13:01:16.000000 gmalglib-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-12 13:01:22.727690 gmalglib-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-12 13:01:16.000000 gmalglib-0.4.0/README.en.md
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-12 13:01:16.000000 gmalglib-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:01:22.719690 gmalglib-0.4.0/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:01:22.723690 gmalglib-0.4.0/include/gmalglib/
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-12 13:01:16.000000 gmalglib-0.4.0/include/gmalglib/bignum.h
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-12 13:01:16.000000 gmalglib-0.4.0/include/gmalglib/random.h
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-04-12 13:01:16.000000 gmalglib-0.4.0/include/gmalglib/sm2.h
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-12 13:01:16.000000 gmalglib-0.4.0/include/gmalglib/sm2curve.h
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-12 13:01:16.000000 gmalglib-0.4.0/include/gmalglib/sm3.h
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-12 13:01:16.000000 gmalglib-0.4.0/include/gmalglib/sm4.h
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-12 13:01:16.000000 gmalglib-0.4.0/include/gmalglib/zuc.h
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-12 13:01:16.000000 gmalglib-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 13:01:22.727690 gmalglib-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-12 13:01:16.000000 gmalglib-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:01:22.719690 gmalglib-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:01:22.723690 gmalglib-0.4.0/src/gmalglib/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-12 13:01:16.000000 gmalglib-0.4.0/src/gmalglib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:01:22.727690 gmalglib-0.4.0/src/gmalglib/core/
--rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-04-12 13:01:16.000000 gmalglib-0.4.0/src/gmalglib/core/bignum.c
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-12 13:01:16.000000 gmalglib-0.4.0/src/gmalglib/core/random.c
--rw-r--r--   0 runner    (1001) docker     (127)    12617 2024-04-12 13:01:16.000000 gmalglib-0.4.0/src/gmalglib/core/sm2.c
--rw-r--r--   0 runner    (1001) docker     (127)    19150 2024-04-12 13:01:16.000000 gmalglib-0.4.0/src/gmalglib/core/sm2curve.c
--rw-r--r--   0 runner    (1001) docker     (127)     5862 2024-04-12 13:01:16.000000 gmalglib-0.4.0/src/gmalglib/core/sm3.c
--rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-04-12 13:01:16.000000 gmalglib-0.4.0/src/gmalglib/core/sm4.c
--rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-04-12 13:01:16.000000 gmalglib-0.4.0/src/gmalglib/core/zuc.c
--rw-r--r--   0 runner    (1001) docker     (127)    28068 2024-04-12 13:01:16.000000 gmalglib-0.4.0/src/gmalglib/coremodule.c
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-12 13:01:16.000000 gmalglib-0.4.0/src/gmalglib/sm2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-04-12 13:01:16.000000 gmalglib-0.4.0/src/gmalglib/sm2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-12 13:01:16.000000 gmalglib-0.4.0/src/gmalglib/sm3.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-12 13:01:16.000000 gmalglib-0.4.0/src/gmalglib/sm3.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-12 13:01:16.000000 gmalglib-0.4.0/src/gmalglib/sm4.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-12 13:01:16.000000 gmalglib-0.4.0/src/gmalglib/sm4.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-12 13:01:16.000000 gmalglib-0.4.0/src/gmalglib/zuc.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-12 13:01:16.000000 gmalglib-0.4.0/src/gmalglib/zuc.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:01:22.727690 gmalglib-0.4.0/src/gmalglib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-12 13:01:22.000000 gmalglib-0.4.0/src/gmalglib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-12 13:01:22.000000 gmalglib-0.4.0/src/gmalglib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 13:01:22.000000 gmalglib-0.4.0/src/gmalglib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 13:01:22.000000 gmalglib-0.4.0/src/gmalglib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:29.097212 gmalglib-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-12 17:26:23.000000 gmalglib-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-12 17:26:29.097212 gmalglib-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-12 17:26:23.000000 gmalglib-0.4.1/README.en.md
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-12 17:26:23.000000 gmalglib-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:29.089212 gmalglib-0.4.1/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:29.093212 gmalglib-0.4.1/include/gmalglib/
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-12 17:26:23.000000 gmalglib-0.4.1/include/gmalglib/bignum.h
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-12 17:26:23.000000 gmalglib-0.4.1/include/gmalglib/random.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-04-12 17:26:23.000000 gmalglib-0.4.1/include/gmalglib/sm2.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-12 17:26:23.000000 gmalglib-0.4.1/include/gmalglib/sm2curve.h
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-12 17:26:23.000000 gmalglib-0.4.1/include/gmalglib/sm3.h
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-12 17:26:23.000000 gmalglib-0.4.1/include/gmalglib/sm4.h
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-12 17:26:23.000000 gmalglib-0.4.1/include/gmalglib/zuc.h
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-12 17:26:23.000000 gmalglib-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 17:26:29.097212 gmalglib-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-12 17:26:23.000000 gmalglib-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:29.089212 gmalglib-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:29.093212 gmalglib-0.4.1/src/gmalglib/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-12 17:26:23.000000 gmalglib-0.4.1/src/gmalglib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:29.097212 gmalglib-0.4.1/src/gmalglib/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-04-12 17:26:23.000000 gmalglib-0.4.1/src/gmalglib/core/bignum.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-12 17:26:23.000000 gmalglib-0.4.1/src/gmalglib/core/random.c
+-rw-r--r--   0 runner    (1001) docker     (127)    12617 2024-04-12 17:26:23.000000 gmalglib-0.4.1/src/gmalglib/core/sm2.c
+-rw-r--r--   0 runner    (1001) docker     (127)    19150 2024-04-12 17:26:23.000000 gmalglib-0.4.1/src/gmalglib/core/sm2curve.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6957 2024-04-12 17:26:23.000000 gmalglib-0.4.1/src/gmalglib/core/sm3.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-04-12 17:26:23.000000 gmalglib-0.4.1/src/gmalglib/core/sm4.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-04-12 17:26:23.000000 gmalglib-0.4.1/src/gmalglib/core/zuc.c
+-rw-r--r--   0 runner    (1001) docker     (127)    29971 2024-04-12 17:26:23.000000 gmalglib-0.4.1/src/gmalglib/coremodule.c
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-12 17:26:23.000000 gmalglib-0.4.1/src/gmalglib/sm2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-04-12 17:26:23.000000 gmalglib-0.4.1/src/gmalglib/sm2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-12 17:26:23.000000 gmalglib-0.4.1/src/gmalglib/sm3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-12 17:26:23.000000 gmalglib-0.4.1/src/gmalglib/sm3.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-12 17:26:23.000000 gmalglib-0.4.1/src/gmalglib/sm4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-12 17:26:23.000000 gmalglib-0.4.1/src/gmalglib/sm4.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-12 17:26:23.000000 gmalglib-0.4.1/src/gmalglib/zuc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-12 17:26:23.000000 gmalglib-0.4.1/src/gmalglib/zuc.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:29.097212 gmalglib-0.4.1/src/gmalglib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-12 17:26:29.000000 gmalglib-0.4.1/src/gmalglib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-12 17:26:29.000000 gmalglib-0.4.1/src/gmalglib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 17:26:29.000000 gmalglib-0.4.1/src/gmalglib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 17:26:29.000000 gmalglib-0.4.1/src/gmalglib.egg-info/top_level.txt
```

### Comparing `gmalglib-0.4.0/LICENSE` & `gmalglib-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gmalglib-0.4.0/PKG-INFO` & `gmalglib-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmalglib
-Version: 0.4.0
+Version: 0.4.1
 Summary: Python package implementing GM algorithms in C.
 Author-email: ww-rm <ww-rm@qq.com>
 Project-URL: Homepage, https://github.com/ww-rm/gmalglib
 Project-URL: Issues, https://github.com/ww-rm/gmalglib/issues
 Project-URL: Documentation, https://gmalglib.readthedocs.io
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gmalglib-0.4.0/include/gmalglib/bignum.h` & `gmalglib-0.4.1/include/gmalglib/bignum.h`

 * *Files identical despite different names*

### Comparing `gmalglib-0.4.0/include/gmalglib/random.h` & `gmalglib-0.4.1/include/gmalglib/random.h`

 * *Files identical despite different names*

### Comparing `gmalglib-0.4.0/include/gmalglib/sm2.h` & `gmalglib-0.4.1/include/gmalglib/sm2.h`

 * *Files identical despite different names*

### Comparing `gmalglib-0.4.0/include/gmalglib/sm2curve.h` & `gmalglib-0.4.1/include/gmalglib/sm2curve.h`

 * *Files identical despite different names*

### Comparing `gmalglib-0.4.0/pyproject.toml` & `gmalglib-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gmalglib-0.4.0/setup.py` & `gmalglib-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `gmalglib-0.4.0/src/gmalglib/core/bignum.c` & `gmalglib-0.4.1/src/gmalglib/core/bignum.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.4.0/src/gmalglib/core/random.c` & `gmalglib-0.4.1/src/gmalglib/core/random.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.4.0/src/gmalglib/core/sm2.c` & `gmalglib-0.4.1/src/gmalglib/core/sm2.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.4.0/src/gmalglib/core/sm2curve.c` & `gmalglib-0.4.1/src/gmalglib/core/sm2curve.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.4.0/src/gmalglib/core/sm3.c` & `gmalglib-0.4.1/src/gmalglib/core/sm3.c`

 * *Files 13% similar despite different names*

```diff
@@ -233,7 +233,59 @@
     ExpandAndCompress(msg_buffer, value);
 
     for (i = 0; i < 8; i++)
     {
         TO_BE(value[i], digest + i * 4);
     }
 }
+
+int SM3_DeriveKey(SM3* self, uint64_t klen, uint8_t* key)
+{
+    uint64_t i = 0;
+    SM3 copy;
+    uint32_t ct = 0x00000001;
+    uint8_t ct_bytes[4] = { 0 };
+    uint8_t tail[SM3_DIGEST_LENGTH] = { 0 };
+
+    if (klen > SM3_KDF_MAX_LENGTH)
+        return SM3_ERR_KDF_OVERFLOW;
+
+    if (self->msg_bitlen + 32 < self->msg_bitlen)
+        return SM3_ERR_OVERFLOW;
+
+    while (klen > 0)
+    {
+        copy = *self;
+        TO_BE(ct, ct_bytes);
+        SM3_Update(&copy, ct_bytes, 4);
+
+        if (klen >= SM3_DIGEST_LENGTH)
+        {
+            SM3_Digest(&copy, key);
+            key += SM3_DIGEST_LENGTH;
+            klen -= SM3_DIGEST_LENGTH;
+        }
+        else
+        {
+            SM3_Digest(&copy, tail);
+            for (i = 0; i < klen; i++)
+            {
+                key[i] = tail[i];
+            }
+            klen = 0;
+        }
+        ct++;
+    }
+
+    return 0;
+}
+
+int SM3_Mac(SM3* self, const uint8_t* key, uint64_t klen, uint8_t* mac)
+{
+    SM3 copy = *self;
+    int err = SM3_Update(&copy, key, klen);;
+
+    if (err) return err;
+
+    SM3_Digest(&copy, mac);
+    return 0;
+}
```

### Comparing `gmalglib-0.4.0/src/gmalglib/core/sm4.c` & `gmalglib-0.4.1/src/gmalglib/core/sm4.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.4.0/src/gmalglib/core/zuc.c` & `gmalglib-0.4.1/src/gmalglib/core/zuc.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.4.0/src/gmalglib/coremodule.c` & `gmalglib-0.4.1/src/gmalglib/coremodule.c`

 * *Files 2% similar despite different names*

```diff
@@ -76,19 +76,77 @@
     if (!other)
         return NULL;
 
     other->sm3 = self->sm3;
     return (PyObject*)other;
 }
 
+static PyObject* PySM3_derive_key(PySM3Object* self, PyObject* args, PyObject* kwargs)
+{
+    char* keys[] = { "klen", NULL };
+    uint8_t* key_buffer = NULL;
+    uint64_t klen = 0;
+    PyObject* ret = NULL;
+    int sm3_ret = 0;
+
+    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "K:derive_key", keys, &klen))
+        return NULL;
+
+    key_buffer = (uint8_t*)PyMem_RawCalloc(klen, sizeof(uint8_t));
+    if (!key_buffer)
+        return PyErr_NoMemory();
+
+    sm3_ret = SM3_DeriveKey(&self->sm3, klen, key_buffer);
+    if (sm3_ret == SM3_ERR_OVERFLOW)
+    {
+        PyErr_SetString(PyExc_OverflowError, "Data too long.");
+        goto cleanup;
+    }
+    if (sm3_ret == SM3_ERR_KDF_OVERFLOW)
+    {
+        PyErr_SetString(PyExc_OverflowError, "Key stream too long.");
+        goto cleanup;
+    }
+
+    ret = PyBytes_FromStringAndSize((char*)key_buffer, klen);
+
+cleanup:
+    PyMem_RawFree(key_buffer);
+    return ret;
+}
+
+static PyObject* PySM3_mac(PySM3Object* self, PyObject* args, PyObject* kwargs)
+{
+    char* keys[] = { "key", NULL };
+    Py_buffer py_buffer_key = { 0 };
+    uint8_t mac[SM3_MAC_LENGTH] = { 0 };
+    int ret = 0;
+
+    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "y*:mac", keys, &py_buffer_key))
+        return NULL;
+
+    ret = SM3_Mac(&self->sm3, py_buffer_key.buf, py_buffer_key.len, mac);
+    PyBuffer_Release(&py_buffer_key);
+
+    if (ret == SM3_ERR_OVERFLOW)
+    {
+        PyErr_SetString(PyExc_OverflowError, "Data too long.");
+        return NULL;
+    }
+
+    return PyBytes_FromStringAndSize((char*)mac, SM3_MAC_LENGTH);
+}
+
 static PyMethodDef py_methods_def_SM3[] = {
     {"update", (PyCFunction)PySM3_update, METH_VARARGS | METH_KEYWORDS, PyDoc_STR("Update internal state with data stream.")},
     {"digest", (PyCFunction)PySM3_digest, METH_NOARGS, PyDoc_STR("Get digest.")},
     {"reset", (PyCFunction)PySM3_reset, METH_NOARGS, PyDoc_STR("Reset internal state to empty.")},
     {"copy", (PyCFunction)PySM3_copy, METH_NOARGS, PyDoc_STR("Copy state to a new object.")},
+    {"derive_key", (PyCFunction)PySM3_derive_key, METH_VARARGS | METH_KEYWORDS, PyDoc_STR("Key derivation function.")},
+    {"mac", (PyCFunction)PySM3_mac, METH_VARARGS | METH_KEYWORDS, PyDoc_STR("SM3 MAC.")},
     {NULL}
 };
 
 static PyTypeObject py_type_SM3 = {
     .ob_base = PyVarObject_HEAD_INIT(NULL, 0)
     .tp_name = "gmalglib.core.SM3",
     .tp_doc = PyDoc_STR("SM3 Object."),
@@ -107,14 +165,16 @@
     if (PyType_Ready(&py_type_SM3) < 0) return 0;
 
     Py_INCREF(&py_type_SM3);
     if (PyModule_AddObject(py_module, "SM3", (PyObject*)&py_type_SM3) < 0) goto error;
     if (!(py_long_SM3_MAX_MSG_BITLEN = PyLong_FromUnsignedLongLong(SM3_MAX_MSG_BITLEN))) goto error;
     if (PyModule_AddObject(py_module, "SM3_MAX_MSG_BITLEN", py_long_SM3_MAX_MSG_BITLEN) < 0) goto error;
     if (PyModule_AddIntMacro(py_module, SM3_DIGEST_LENGTH) < 0) goto error;
+    if (PyModule_AddIntMacro(py_module, SM3_KDF_MAX_LENGTH) < 0) goto error;
+    if (PyModule_AddIntMacro(py_module, SM3_MAC_LENGTH) < 0) goto error;
 
     return 1;
 
 error:
     Py_XDECREF(py_long_SM3_MAX_MSG_BITLEN);
     Py_DECREF(&py_type_SM3);
     return 0;
@@ -485,15 +545,15 @@
 
 static PyObject* PySM2_is_sk_valid(PySM2Object* self, PyObject* args, PyObject* kwargs)
 {
     char* keys[] = { "sk", NULL };
     Py_buffer py_buffer_sk = { 0 };
     int is_valid = 0;
 
-    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "|y*:is_sk_valid", keys, &py_buffer_sk))
+    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "y*:is_sk_valid", keys, &py_buffer_sk))
         return NULL;
 
     if (py_buffer_sk.len != SM2_SK_LENGTH)
     {
         PyErr_SetString(PyExc_ValueError, "Incorrect secret key length.");
         PyBuffer_Release(&py_buffer_sk);
         return NULL;
@@ -510,15 +570,15 @@
 static PyObject* PySM2_is_pk_valid(PySM2Object* self, PyObject* args, PyObject* kwargs)
 {
     char* keys[] = { "pk", NULL };
     Py_buffer py_buffer_pk = { 0 };
 
     int is_valid = 0;
 
-    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "|y*:is_pk_valid", keys, &py_buffer_pk))
+    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "y*:is_pk_valid", keys, &py_buffer_pk))
         return NULL;
 
     if (py_buffer_pk.len != SM2_PK_HALF_LENGTH && py_buffer_pk.len != SM2_PK_FULL_LENGTH)
     {
         PyErr_SetString(PyExc_ValueError, "Incorrect public key length.");
         PyBuffer_Release(&py_buffer_pk);
         return NULL;
@@ -537,15 +597,15 @@
     char* keys[] = { "sk", "pc_mode", NULL};
     Py_buffer py_buffer_sk = { 0 };
     int pc_mode = 0;
     uint8_t pk[SM2_PK_FULL_LENGTH] = { 0 };
 
     int sm2_ret = 0;
 
-    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "|y*$i:get_pk", keys, &py_buffer_sk, &pc_mode))
+    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "y*|$i:get_pk", keys, &py_buffer_sk, &pc_mode))
         return NULL;
 
     if (py_buffer_sk.len != SM2_SK_LENGTH)
     {
         PyErr_SetString(PyExc_ValueError, "Incorrect secret key length.");
         PyBuffer_Release(&py_buffer_sk);
         return NULL;
@@ -593,15 +653,15 @@
 {
     char* keys[] = { "digest", NULL };
     Py_buffer py_buffer_digest = { 0 };
     uint8_t signature[SM2_SIGNATURE_LENGTH] = { 0 };
     PyObject* ret = NULL;
     int sm2_ret = 0;
 
-    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "|y*:sign_digest", keys, &py_buffer_digest))
+    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "y*:sign_digest", keys, &py_buffer_digest))
         return NULL;
 
     if (py_buffer_digest.len != SM3_DIGEST_LENGTH)
     {
         PyErr_SetString(PyExc_ValueError, "Incorrect digest length.");
         goto cleanup;
     }
@@ -628,15 +688,15 @@
 static PyObject* PySM2_verify_digest(PySM2Object* self, PyObject* args, PyObject* kwargs)
 {
     char* keys[] = { "digest", "signature", NULL };
     Py_buffer py_buffer_digest = { 0 };
     Py_buffer py_buffer_signature = { 0 };
     int sm2_ret = -1;
 
-    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "|y*y*:verify_digest", keys, &py_buffer_digest, &py_buffer_signature))
+    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "y*y*:verify_digest", keys, &py_buffer_digest, &py_buffer_signature))
         return NULL;
 
     if (py_buffer_digest.len != SM3_DIGEST_LENGTH)
     {
         PyErr_SetString(PyExc_ValueError, "Incorrect digest length.");
         PyBuffer_Release(&py_buffer_digest);
         PyBuffer_Release(&py_buffer_signature);
@@ -671,15 +731,15 @@
 {
     char* keys[] = { "message", NULL };
     Py_buffer py_buffer_message = { 0 };
     uint8_t signature[SM2_SIGNATURE_LENGTH] = { 0 };
     PyObject* ret = NULL;
     int sm2_ret = 0;
 
-    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "|y*:sign", keys, &py_buffer_message))
+    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "y*:sign", keys, &py_buffer_message))
         return NULL;
 
     sm2_ret = SM2_Sign(&self->sm2, py_buffer_message.buf, py_buffer_message.len, signature);
     if (sm2_ret == SM2_ERR_NEED_SK)
     {
         PyErr_SetString(PyExc_AttributeError, "Need secret key.");
         goto cleanup;
@@ -710,15 +770,15 @@
 static PyObject* PySM2_verify(PySM2Object* self, PyObject* args, PyObject* kwargs)
 {
     char* keys[] = { "message", "signature", NULL };
     Py_buffer py_buffer_message = { 0 };
     Py_buffer py_buffer_signature = { 0 };
     int sm2_ret = -1;
 
-    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "|y*y*:verify", keys, &py_buffer_message, &py_buffer_signature))
+    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "y*y*:verify", keys, &py_buffer_message, &py_buffer_signature))
         return NULL;
 
     if (py_buffer_signature.len != SM2_SIGNATURE_LENGTH)
     {
         PyErr_SetString(PyExc_ValueError, "Incorrect signature length.");
         PyBuffer_Release(&py_buffer_message);
         PyBuffer_Release(&py_buffer_signature);
```

### Comparing `gmalglib-0.4.0/src/gmalglib/sm2.py` & `gmalglib-0.4.1/src/gmalglib/sm2.py`

 * *Files identical despite different names*

### Comparing `gmalglib-0.4.0/src/gmalglib/sm2.pyi` & `gmalglib-0.4.1/src/gmalglib/sm2.pyi`

 * *Files identical despite different names*

### Comparing `gmalglib-0.4.0/src/gmalglib/sm3.pyi` & `gmalglib-0.4.1/src/gmalglib/sm3.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 SM3_MAX_MSG_BITLEN: int
 SM3_DIGEST_LENGTH: int
+SM3_KDF_MAX_LENGTH: int
+SM3_MAC_LENGTH: int
 
 
 class SM3:
     """SM3 算法对象."""
 
     def __init__(self, data: bytes = b"") -> None:
         """SM3 算法对象.
@@ -19,7 +21,13 @@
         """获取当前状态哈希值."""
 
     def reset(self) -> None:
         """重置内部状态."""
 
     def copy(self) -> SM3:
         """拷贝当前对象及其内部状态."""
+
+    def derive_key(self, klen: int) -> bytes:
+        """密钥派生函数."""
+
+    def mac(self, key: bytes) -> bytes:
+        """消息认证码."""
```

### Comparing `gmalglib-0.4.0/src/gmalglib.egg-info/PKG-INFO` & `gmalglib-0.4.1/src/gmalglib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmalglib
-Version: 0.4.0
+Version: 0.4.1
 Summary: Python package implementing GM algorithms in C.
 Author-email: ww-rm <ww-rm@qq.com>
 Project-URL: Homepage, https://github.com/ww-rm/gmalglib
 Project-URL: Issues, https://github.com/ww-rm/gmalglib/issues
 Project-URL: Documentation, https://gmalglib.readthedocs.io
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gmalglib-0.4.0/src/gmalglib.egg-info/SOURCES.txt` & `gmalglib-0.4.1/src/gmalglib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

