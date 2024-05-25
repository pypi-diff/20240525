# Comparing `tmp/bencode_c-0.0.8.tar.gz` & `tmp/bencode_c-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bencode_c-0.0.8.tar", last modified: Tue May 21 14:10:07 2024, max compression
+gzip compressed data, was "bencode_c-0.0.9.tar", last modified: Tue May 21 19:45:57 2024, max compression
```

## Comparing `bencode_c-0.0.8.tar` & `bencode_c-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:10:07.365729 bencode_c-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-21 14:10:07.365729 bencode_c-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-21 14:10:04.000000 bencode_c-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-21 14:10:04.000000 bencode_c-0.0.8/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 14:10:07.365729 bencode_c-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-21 14:10:04.000000 bencode_c-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:10:07.361729 bencode_c-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:10:07.361729 bencode_c-0.0.8/src/bencode_c/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-21 14:10:04.000000 bencode_c-0.0.8/src/bencode_c/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-21 14:10:04.000000 bencode_c-0.0.8/src/bencode_c/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-21 14:10:04.000000 bencode_c-0.0.8/src/bencode_c/bencode.c
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-21 14:10:04.000000 bencode_c-0.0.8/src/bencode_c/common.h
--rw-r--r--   0 runner    (1001) docker     (127)     5646 2024-05-21 14:10:04.000000 bencode_c-0.0.8/src/bencode_c/decode.h
--rw-r--r--   0 runner    (1001) docker     (127)     8266 2024-05-21 14:10:04.000000 bencode_c-0.0.8/src/bencode_c/encode.h
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 14:10:04.000000 bencode_c-0.0.8/src/bencode_c/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:10:07.365729 bencode_c-0.0.8/src/bencode_c.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-21 14:10:07.000000 bencode_c-0.0.8/src/bencode_c.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-21 14:10:07.000000 bencode_c-0.0.8/src/bencode_c.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 14:10:07.000000 bencode_c-0.0.8/src/bencode_c.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-21 14:10:07.000000 bencode_c-0.0.8/src/bencode_c.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-21 14:10:07.000000 bencode_c-0.0.8/src/bencode_c.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:10:07.365729 bencode_c-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-05-21 14:10:04.000000 bencode_c-0.0.8/tests/test_decode.py
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-21 14:10:04.000000 bencode_c-0.0.8/tests/test_encode.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-21 14:10:04.000000 bencode_c-0.0.8/tests/test_torrent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:45:57.475020 bencode_c-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-21 19:45:57.475020 bencode_c-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-21 19:45:54.000000 bencode_c-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-21 19:45:54.000000 bencode_c-0.0.9/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 19:45:57.475020 bencode_c-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-21 19:45:54.000000 bencode_c-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:45:57.471020 bencode_c-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:45:57.475020 bencode_c-0.0.9/src/bencode_c/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-21 19:45:54.000000 bencode_c-0.0.9/src/bencode_c/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-21 19:45:54.000000 bencode_c-0.0.9/src/bencode_c/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-21 19:45:54.000000 bencode_c-0.0.9/src/bencode_c/bencode.c
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-21 19:45:54.000000 bencode_c-0.0.9/src/bencode_c/common.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-05-21 19:45:54.000000 bencode_c-0.0.9/src/bencode_c/decode.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8734 2024-05-21 19:45:54.000000 bencode_c-0.0.9/src/bencode_c/encode.h
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 19:45:54.000000 bencode_c-0.0.9/src/bencode_c/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:45:57.475020 bencode_c-0.0.9/src/bencode_c.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-21 19:45:57.000000 bencode_c-0.0.9/src/bencode_c.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-21 19:45:57.000000 bencode_c-0.0.9/src/bencode_c.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 19:45:57.000000 bencode_c-0.0.9/src/bencode_c.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-21 19:45:57.000000 bencode_c-0.0.9/src/bencode_c.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-21 19:45:57.000000 bencode_c-0.0.9/src/bencode_c.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:45:57.475020 bencode_c-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-05-21 19:45:54.000000 bencode_c-0.0.9/tests/test_decode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-21 19:45:54.000000 bencode_c-0.0.9/tests/test_encode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-21 19:45:54.000000 bencode_c-0.0.9/tests/test_torrent.py
```

### Comparing `bencode_c-0.0.8/PKG-INFO` & `bencode_c-0.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: bencode-c
-Version: 0.0.8
+Version: 0.0.9
 Summary: A fast and correct bencode serialize/deserialize library
 Author-email: trim21 <trim21me@gmail.com>
 License: MIT
 Keywords: bencode,bittorrent,bit-torrent,serialize,deserialize,p2p
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: <4.0,>=3.8
 Description-Content-Type: text/markdown
```

### Comparing `bencode_c-0.0.8/pyproject.toml` & `bencode_c-0.0.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # pyproject.toml
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bencode-c"
-version = "0.0.8"
+version = "0.0.9"
 description = "A fast and correct bencode serialize/deserialize library"
 license = { text = "MIT" }
 requires-python = ">=3.8,<4.0"
 authors = [
     { name = "trim21", email = "trim21me@gmail.com" },
 ]
 readme = 'readme.md'
@@ -19,15 +19,15 @@
     "bit-torrent",
     "serialize",
     "deserialize",
     'p2p',
 ]
 
 classifiers = [
-    "Development Status :: 5 - Production/Stable",
+    "Development Status :: 2 - Pre-Alpha",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: C",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
 ]
```

### Comparing `bencode_c-0.0.8/src/bencode_c/bencode.c` & `bencode_c-0.0.9/src/bencode_c/bencode.c`

 * *Files identical despite different names*

### Comparing `bencode_c-0.0.8/src/bencode_c/decode.h` & `bencode_c-0.0.9/src/bencode_c/decode.h`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 static PyObject *BencodeDecodeError;
 
 static inline PyObject *decodingError(const char *fmt, ...);
 
 static PyObject *decodeAny(const char *buf, Py_ssize_t *index, Py_ssize_t size);
 static PyObject *decodeInt(const char *buf, Py_ssize_t *index, Py_ssize_t size);
 static PyObject *decodeBytes(const char *buf, Py_ssize_t *index, Py_ssize_t size);
-static PyObject *decodeDict(const char *buf, Py_ssize_t *index, Py_ssize_t size, PyObject *dict);
+static void decodeDict(const char *buf, Py_ssize_t *index, Py_ssize_t size, PyObject *dict);
 static PyObject *decodeList(const char *buf, Py_ssize_t *index, Py_ssize_t size);
 
 static PyObject *bdecode(PyObject *self, PyObject *b) {
   if (!PyBytes_Check(b)) {
     PyErr_SetString(PyExc_TypeError, "can only decode bytes");
     return NULL;
   }
@@ -150,49 +150,52 @@
   } else if (len1 > len2) {
     return 1;
   } else {
     return 0;
   }
 }
 
-static PyObject *decodeDict(const char *buf, Py_ssize_t *index, Py_ssize_t size, PyObject *d) {
+static void decodeDict(const char *buf, Py_ssize_t *index, Py_ssize_t size, PyObject *d) {
   *index = *index + 1;
   const char *lastKey = NULL;
   size_t lastKeyLen = 0;
   const char *currentKey;
   size_t currentKeyLen;
   while (buf[*index] != 'e') {
     PyObject *key = decodeBytes(buf, index, size);
     if (key == NULL) {
-      return NULL;
+      return;
     }
 
     PyObject *obj = decodeAny(buf, index, size);
     if (obj == NULL) {
       Py_DecRef(key);
-      return NULL;
+      return;
     }
     currentKeyLen = PyBytes_Size(key);
     currentKey = PyBytes_AsString(key);
     // skip first key
     if (lastKey != NULL) {
       int keyCmp = strCompare(currentKey, currentKeyLen, lastKey, lastKeyLen);
       if (keyCmp < 0) {
-        return decodingError("invalid dict, key not sorted. index %d", *index);
+        decodingError("invalid dict, key not sorted. index %d", *index);
+        return;
       }
       if (keyCmp == 0) {
-        return decodingError("invalid dict, find duplicated keys %.*s. index %d", currentKeyLen, currentKey, *index);
+        decodingError("invalid dict, find duplicated keys %.*s. index %d", currentKeyLen, currentKey, *index);
+        return;
       }
     }
     lastKey = currentKey;
     lastKeyLen = currentKeyLen;
     PyDict_SetItem(d, key, obj);
+    Py_DecRef(key);
+    Py_DecRef(obj);
   }
   *index = *index + 1;
-  return d;
 }
 
 static PyObject *decodeAny(const char *buf, Py_ssize_t *index, Py_ssize_t size) {
   // int
   if (buf[*index] == 'i') {
     return decodeInt(buf, index, size);
   }
@@ -203,18 +206,18 @@
   if (buf[*index] == 'l') {
     return decodeList(buf, index, size);
   }
 
   if (buf[*index] == 'd') {
     PyObject *dict = PyDict_New();
 
-    PyObject *r = decodeDict(buf, index, size, dict);
-    if (r == NULL) {
+    decodeDict(buf, index, size, dict);
+    if (dict == NULL) {
       Py_DecRef(dict);
       return NULL;
     }
 
-    return r;
+    return dict;
   }
 
   return decodingError("invalid bencode prefix '%c', index %d", buf[*index], *index);
 }
```

### Comparing `bencode_c-0.0.8/src/bencode_c/encode.h` & `bencode_c-0.0.9/src/bencode_c/encode.h`

 * *Files 4% similar despite different names*

```diff
@@ -7,20 +7,24 @@
 
 #define NON_SUPPORTED_TYPE_MESSAGE                                                                                     \
   "invalid type '%s', "                                                                                                \
   "bencode only support bytes, str, int, list, tuple, dict and bool(encoded as 0/1, decoded as int)"
 
 #define defaultBufferSize 4096
 
-#define HPyLong_Check(obj) Py_TypeCheck(obj, PyLong_Type)
 #define returnIfError(o)                                                                                               \
   if (o) {                                                                                                             \
     return o;                                                                                                          \
   }
 
+#define OperatorIF(err, op)                                                                                            \
+  if (!err) {                                                                                                          \
+    err |= op;                                                                                                         \
+  }
+
 static HPy errTypeMessage;
 
 static inline void runtimeError(const char *data) { PyErr_SetString(PyExc_RuntimeError, data); }
 
 static inline void typeError(const char *data) { PyErr_SetString(PyExc_TypeError, data); }
 
 static inline HPy bencodeError(const char *data) {
@@ -61,15 +65,14 @@
 
   buf->len = buf->len + size;
 
   return 0;
 }
 
 static int bufferWriteLong(struct buffer *buf, long long val) {
-
   int j = snprintf(NULL, 0, "%lld", val) + 1;
   char *s = (char *)malloc(sizeof(char) * j);
   snprintf(s, j, "%lld", val);
   int r = bufferWrite(buf, s, j - 1);
   free(s);
   return r;
 }
@@ -128,14 +131,19 @@
     if (tu == NULL) {
       runtimeError("can not pack key value pair");
       return 1;
     }
 
     PyList_Append(*list, tu);
     Py_DecRef(tu);
+    Py_DecRef(key);
+
+    if (keyAsBytes != key) {
+      Py_DecRef(keyAsBytes);
+    }
   }
 
   Py_DecRef(keys);
 
   if (PyObject_CallMethod(*list, "sort", NULL) == NULL) {
     return 1;
   }
@@ -150,43 +158,42 @@
     HPy keyValue = PyList_GetItem(*list, i);
     HPy key = PyTuple_GetItem(keyValue, 0);
     currentKeylen = PyBytes_Size(key);
     currentKey = PyBytes_AsString(key);
     if (lastKey != NULL) {
       if (lastKeylen == currentKeylen) {
         if (strncmp(lastKey, currentKey, lastKeylen) == 0) {
-          // Py_DecRef(keyValue);
-          // Py_DecRef(key);
           bencodeError("find duplicated keys with str and bytes in dict");
           return 1;
         }
       }
     }
 
     lastKey = currentKey;
     lastKeylen = currentKeylen;
-
-    // Py_DecRef(keyValue);
-    // Py_DecRef(key);
   }
 
   return 0;
 }
 
 // TODO: use PyUnicode_AsUTF8AndSize after 3.10
 static int encodeStr(struct buffer *buf, HPy obj) {
   HPy b = PyUnicode_AsUTF8String(obj);
 
   HPy_ssize_t size = PyBytes_Size(b);
 
   const char *data = PyBytes_AsString(b);
+  if (data == NULL) {
+    Py_DecRef(b);
+    return 1;
+  }
 
   int err = bufferWriteLong(buf, size);
-  err |= bufferWrite(buf, ":", 1);
-  err |= bufferWrite(buf, data, size);
+  OperatorIF(err, bufferWrite(buf, ":", 1));
+  OperatorIF(err, bufferWrite(buf, data, size));
 
   Py_DecRef(b);
 
   return err;
 }
 
 static int encodeBytes(struct buffer *buf, HPy obj) {
@@ -196,14 +203,15 @@
   returnIfError(bufferWriteLong(buf, size));
   returnIfError(bufferWrite(buf, ":", 1));
   return bufferWrite(buf, data, size);
 }
 
 static int encodeDict(struct buffer *buf, HPy obj) {
   returnIfError(bufferWrite(buf, "d", 1));
+
   HPy list = NULL;
   HPy_ssize_t count = 0;
   if (buildDictKeyList(obj, &list, &count)) {
     if (list != NULL) {
       Py_DecRef(list);
     }
     return 1;
@@ -246,65 +254,85 @@
     }
   }
 
   Py_DecRef(list);
   return bufferWrite(buf, "e", 1);
 }
 
+static int encodeInt(struct buffer *buf, HPy obj) {
+  long long val = PyLong_AsLongLong(obj);
+  if (PyErr_Occurred()) { // python int may overflow c long long.
+    return 1;
+  }
+
+  returnIfError(bufferWrite(buf, "i", 1));
+  returnIfError(bufferWriteLong(buf, val));
+  return bufferWrite(buf, "e", 1);
+}
+
+static int encodeList(struct buffer *buf, HPy obj) {
+  HPy_ssize_t len = PyList_Size(obj);
+  returnIfError(bufferWrite(buf, "l", 1));
+
+  for (HPy_ssize_t i = 0; i < len; i++) {
+    HPy o = PyList_GetItem(obj, i);
+    returnIfError(encodeAny(buf, o));
+  }
+
+  return bufferWrite(buf, "e", 1);
+}
+
+static int encodeTuple(struct buffer *buf, HPy obj) {
+  HPy_ssize_t len = PyTuple_Size(obj);
+  returnIfError(bufferWrite(buf, "l", 1));
+
+  for (HPy_ssize_t i = 0; i < len; i++) {
+    HPy o = PyTuple_GetItem(obj, i);
+    returnIfError(encodeAny(buf, o));
+  }
+
+  return bufferWrite(buf, "e", 1);
+}
+
 static int encodeAny(struct buffer *buf, HPy obj) {
   if (Py_True == obj) {
     return bufferWrite(buf, "i1e", 3);
-  } else if (Py_False == obj) {
+  }
+
+  if (Py_False == obj) {
     return bufferWrite(buf, "i0e", 3);
-  } else if (PyBytes_Check(obj)) {
+  }
+
+  if (PyBytes_Check(obj)) {
     return encodeBytes(buf, obj);
-  } else if (PyUnicode_Check(obj)) {
-    return encodeStr(buf, obj);
-  } else if (PyLong_Check(obj)) {
-    long long val = PyLong_AsLongLong(obj);
+  }
 
-    // python int may overflow c long long
-    if (PyErr_Occurred()) {
-      return 1;
-    }
+  if (PyUnicode_Check(obj)) {
+    return encodeStr(buf, obj);
+  }
 
-    returnIfError(bufferWrite(buf, "i", 1));
-    returnIfError(bufferWriteLong(buf, val));
-    return bufferWrite(buf, "e", 1);
-  } else if (PyList_Check(obj)) {
-    HPy_ssize_t len = PyList_Size(obj);
-    returnIfError(bufferWrite(buf, "l", 1));
-    if (len == 0) {
-      return bufferWrite(buf, "e", 1);
-    }
+  if (PyLong_Check(obj)) {
+    return encodeInt(buf, obj);
+  }
 
-    for (HPy_ssize_t i = 0; i < len; i++) {
-      HPy o = PyList_GetItem(obj, i);
-      returnIfError(encodeAny(buf, o));
-    }
-    return bufferWrite(buf, "e", 1);
-  } else if (PyTuple_Check(obj)) {
-    HPy_ssize_t len = PyTuple_Size(obj);
-    returnIfError(bufferWrite(buf, "l", 1));
-    if (len == 0) {
-      return bufferWrite(buf, "e", 1);
-    }
+  if (PyList_Check(obj)) {
+    return encodeList(buf, obj);
+  }
 
-    for (HPy_ssize_t i = 0; i < len; i++) {
-      HPy o = PyTuple_GetItem(obj, i);
-      returnIfError(encodeAny(buf, o));
-    }
-    return bufferWrite(buf, "e", 1);
+  if (PyTuple_Check(obj)) {
+    return encodeTuple(buf, obj);
+  }
 
-  } else if (PyDict_Check(obj)) {
+  if (PyDict_Check(obj)) {
     return encodeDict(buf, obj);
   }
 
-  HPy typ = PyObject_Type(obj);
+  // Unsupported type, raise TypeError
 
+  HPy typ = PyObject_Type(obj);
   if (typ == NULL) {
     runtimeError("failed to get type of object");
     return 1;
   }
 
   HPy ss = PyUnicode_Format(errTypeMessage, typ);
   if (ss == NULL) {
@@ -317,22 +345,21 @@
 
   Py_DecRef(ss);
   Py_DecRef(typ);
 
   return 1;
 }
 
-static HPy bencode(HPy self, HPy obj) {
-  // self is the module object
-
+// mod is the module object
+static HPy bencode(HPy mod, HPy obj) {
   struct buffer *buf = newBuffer();
 
+  // error when encoding
   if (encodeAny(buf, obj)) {
     freeBuffer(buf);
-    // error when encoding
     return NULL;
   }
 
   HPy res = PyBytes_FromStringAndSize(buf->buf, buf->len);
 
   freeBuffer(buf);
```

### Comparing `bencode_c-0.0.8/src/bencode_c.egg-info/PKG-INFO` & `bencode_c-0.0.9/src/bencode_c.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: bencode-c
-Version: 0.0.8
+Version: 0.0.9
 Summary: A fast and correct bencode serialize/deserialize library
 Author-email: trim21 <trim21me@gmail.com>
 License: MIT
 Keywords: bencode,bittorrent,bit-torrent,serialize,deserialize,p2p
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: <4.0,>=3.8
 Description-Content-Type: text/markdown
```

### Comparing `bencode_c-0.0.8/tests/test_decode.py` & `bencode_c-0.0.9/tests/test_decode.py`

 * *Files identical despite different names*

### Comparing `bencode_c-0.0.8/tests/test_encode.py` & `bencode_c-0.0.9/tests/test_encode.py`

 * *Files identical despite different names*

