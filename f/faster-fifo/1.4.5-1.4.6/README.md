# Comparing `tmp/faster-fifo-1.4.5.tar.gz` & `tmp/faster_fifo-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faster-fifo-1.4.5.tar", last modified: Sat Mar 25 02:15:36 2023, max compression
+gzip compressed data, was "faster_fifo-1.4.6.tar", last modified: Sat May 25 08:14:43 2024, max compression
```

## Comparing `faster-fifo-1.4.5.tar` & `faster_fifo-1.4.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 aleksei_petrenko   (501) staff       (20)        0 2023-03-25 02:15:36.908678 faster-fifo-1.4.5/
--rw-r--r--   0 aleksei_petrenko   (501) staff       (20)     1073 2023-03-25 02:04:33.000000 faster-fifo-1.4.5/LICENSE
--rw-r--r--   0 aleksei_petrenko   (501) staff       (20)       63 2023-03-25 02:04:33.000000 faster-fifo-1.4.5/MANIFEST.in
--rw-r--r--   0 aleksei_petrenko   (501) staff       (20)     7475 2023-03-25 02:15:36.908565 faster-fifo-1.4.5/PKG-INFO
--rw-r--r--   0 aleksei_petrenko   (501) staff       (20)     7073 2023-03-25 02:13:27.000000 faster-fifo-1.4.5/README.md
-drwxr-xr-x   0 aleksei_petrenko   (501) staff       (20)        0 2023-03-25 02:15:36.907250 faster-fifo-1.4.5/cpp_faster_fifo/
--rw-r--r--   0 aleksei_petrenko   (501) staff       (20)        0 2023-03-25 02:04:33.000000 faster-fifo-1.4.5/cpp_faster_fifo/__init__.py
-drwxr-xr-x   0 aleksei_petrenko   (501) staff       (20)        0 2023-03-25 02:15:36.907458 faster-fifo-1.4.5/cpp_faster_fifo/cpp_lib/
--rw-r--r--   0 aleksei_petrenko   (501) staff       (20)     9636 2023-03-25 02:04:33.000000 faster-fifo-1.4.5/cpp_faster_fifo/cpp_lib/faster_fifo.cpp
--rw-r--r--   0 aleksei_petrenko   (501) staff       (20)      779 2023-03-25 02:04:33.000000 faster-fifo-1.4.5/cpp_faster_fifo/cpp_lib/faster_fifo.hpp
-drwxr-xr-x   0 aleksei_petrenko   (501) staff       (20)        0 2023-03-25 02:15:36.907797 faster-fifo-1.4.5/cpp_faster_fifo/tests/
--rw-r--r--   0 aleksei_petrenko   (501) staff       (20)        0 2023-03-25 02:04:33.000000 faster-fifo-1.4.5/cpp_faster_fifo/tests/__init__.py
--rw-r--r--   0 aleksei_petrenko   (501) staff       (20)     8284 2023-03-25 02:04:33.000000 faster-fifo-1.4.5/cpp_faster_fifo/tests/comparison_tests.py
--rw-r--r--   0 aleksei_petrenko   (501) staff       (20)     9382 2023-03-25 02:04:33.000000 faster-fifo-1.4.5/cpp_faster_fifo/tests/test_faster_fifo.py
--rw-r--r--   0 aleksei_petrenko   (501) staff       (20)   530208 2023-03-25 02:15:35.000000 faster-fifo-1.4.5/faster_fifo.cpp
-drwxr-xr-x   0 aleksei_petrenko   (501) staff       (20)        0 2023-03-25 02:15:36.908318 faster-fifo-1.4.5/faster_fifo.egg-info/
--rw-r--r--   0 aleksei_petrenko   (501) staff       (20)     7475 2023-03-25 02:15:36.000000 faster-fifo-1.4.5/faster_fifo.egg-info/PKG-INFO
--rw-r--r--   0 aleksei_petrenko   (501) staff       (20)      539 2023-03-25 02:15:36.000000 faster-fifo-1.4.5/faster_fifo.egg-info/SOURCES.txt
--rw-r--r--   0 aleksei_petrenko   (501) staff       (20)        1 2023-03-25 02:15:36.000000 faster-fifo-1.4.5/faster_fifo.egg-info/dependency_links.txt
--rw-r--r--   0 aleksei_petrenko   (501) staff       (20)       64 2023-03-25 02:15:36.000000 faster-fifo-1.4.5/faster_fifo.egg-info/requires.txt
--rw-r--r--   0 aleksei_petrenko   (501) staff       (20)       50 2023-03-25 02:15:36.000000 faster-fifo-1.4.5/faster_fifo.egg-info/top_level.txt
--rw-r--r--   0 aleksei_petrenko   (501) staff       (20)    10083 2023-03-25 02:04:33.000000 faster-fifo-1.4.5/faster_fifo.pyx
--rw-r--r--   0 aleksei_petrenko   (501) staff       (20)      896 2023-03-25 02:04:33.000000 faster-fifo-1.4.5/faster_fifo_def.pxd
-drwxr-xr-x   0 aleksei_petrenko   (501) staff       (20)        0 2023-03-25 02:15:36.908424 faster-fifo-1.4.5/faster_fifo_reduction/
--rw-r--r--   0 aleksei_petrenko   (501) staff       (20)      952 2023-03-25 02:04:33.000000 faster-fifo-1.4.5/faster_fifo_reduction/__init__.py
--rw-r--r--   0 aleksei_petrenko   (501) staff       (20)      100 2023-03-25 02:04:33.000000 faster-fifo-1.4.5/pyproject.toml
--rw-r--r--   0 aleksei_petrenko   (501) staff       (20)       38 2023-03-25 02:15:36.908710 faster-fifo-1.4.5/setup.cfg
--rw-r--r--   0 aleksei_petrenko   (501) staff       (20)     1228 2023-03-25 02:13:27.000000 faster-fifo-1.4.5/setup.py
+drwxrwxr-x   0 aleksei   (1000) aleksei   (1000)        0 2024-05-25 08:14:43.847386 faster_fifo-1.4.6/
+-rw-rw-r--   0 aleksei   (1000) aleksei   (1000)     1073 2024-05-25 07:59:56.000000 faster_fifo-1.4.6/LICENSE
+-rw-rw-r--   0 aleksei   (1000) aleksei   (1000)       63 2024-05-25 07:59:56.000000 faster_fifo-1.4.6/MANIFEST.in
+-rw-r--r--   0 aleksei   (1000) aleksei   (1000)     7756 2024-05-25 08:14:43.847386 faster_fifo-1.4.6/PKG-INFO
+-rw-rw-r--   0 aleksei   (1000) aleksei   (1000)     7205 2024-05-25 08:07:02.000000 faster_fifo-1.4.6/README.md
+drwxrwxr-x   0 aleksei   (1000) aleksei   (1000)        0 2024-05-25 08:14:43.847386 faster_fifo-1.4.6/cpp_faster_fifo/
+-rw-rw-r--   0 aleksei   (1000) aleksei   (1000)        0 2024-05-25 07:59:56.000000 faster_fifo-1.4.6/cpp_faster_fifo/__init__.py
+drwxrwxr-x   0 aleksei   (1000) aleksei   (1000)        0 2024-05-25 08:14:43.847386 faster_fifo-1.4.6/cpp_faster_fifo/cpp_lib/
+-rw-rw-r--   0 aleksei   (1000) aleksei   (1000)    10035 2024-05-25 07:59:56.000000 faster_fifo-1.4.6/cpp_faster_fifo/cpp_lib/faster_fifo.cpp
+-rw-rw-r--   0 aleksei   (1000) aleksei   (1000)      795 2024-05-25 07:59:56.000000 faster_fifo-1.4.6/cpp_faster_fifo/cpp_lib/faster_fifo.hpp
+drwxrwxr-x   0 aleksei   (1000) aleksei   (1000)        0 2024-05-25 08:14:43.847386 faster_fifo-1.4.6/cpp_faster_fifo/tests/
+-rw-rw-r--   0 aleksei   (1000) aleksei   (1000)        0 2024-05-25 07:59:56.000000 faster_fifo-1.4.6/cpp_faster_fifo/tests/__init__.py
+-rw-rw-r--   0 aleksei   (1000) aleksei   (1000)     9898 2024-05-25 07:59:56.000000 faster_fifo-1.4.6/cpp_faster_fifo/tests/comparison_tests.py
+-rw-rw-r--   0 aleksei   (1000) aleksei   (1000)    11715 2024-05-25 07:59:56.000000 faster_fifo-1.4.6/cpp_faster_fifo/tests/test_faster_fifo.py
+-rw-rw-r--   0 aleksei   (1000) aleksei   (1000)   747602 2024-05-25 08:14:40.000000 faster_fifo-1.4.6/faster_fifo.cpp
+drwxrwxr-x   0 aleksei   (1000) aleksei   (1000)        0 2024-05-25 08:14:43.847386 faster_fifo-1.4.6/faster_fifo.egg-info/
+-rw-r--r--   0 aleksei   (1000) aleksei   (1000)     7756 2024-05-25 08:14:43.000000 faster_fifo-1.4.6/faster_fifo.egg-info/PKG-INFO
+-rw-rw-r--   0 aleksei   (1000) aleksei   (1000)      539 2024-05-25 08:14:43.000000 faster_fifo-1.4.6/faster_fifo.egg-info/SOURCES.txt
+-rw-rw-r--   0 aleksei   (1000) aleksei   (1000)        1 2024-05-25 08:14:43.000000 faster_fifo-1.4.6/faster_fifo.egg-info/dependency_links.txt
+-rw-rw-r--   0 aleksei   (1000) aleksei   (1000)       64 2024-05-25 08:14:43.000000 faster_fifo-1.4.6/faster_fifo.egg-info/requires.txt
+-rw-rw-r--   0 aleksei   (1000) aleksei   (1000)       50 2024-05-25 08:14:43.000000 faster_fifo-1.4.6/faster_fifo.egg-info/top_level.txt
+-rw-rw-r--   0 aleksei   (1000) aleksei   (1000)    10401 2024-05-25 07:59:56.000000 faster_fifo-1.4.6/faster_fifo.pyx
+-rw-rw-r--   0 aleksei   (1000) aleksei   (1000)      912 2024-05-25 07:59:56.000000 faster_fifo-1.4.6/faster_fifo_def.pxd
+drwxrwxr-x   0 aleksei   (1000) aleksei   (1000)        0 2024-05-25 08:14:43.847386 faster_fifo-1.4.6/faster_fifo_reduction/
+-rw-rw-r--   0 aleksei   (1000) aleksei   (1000)      952 2024-05-25 07:59:56.000000 faster_fifo-1.4.6/faster_fifo_reduction/__init__.py
+-rw-rw-r--   0 aleksei   (1000) aleksei   (1000)      100 2024-05-25 07:59:56.000000 faster_fifo-1.4.6/pyproject.toml
+-rw-rw-r--   0 aleksei   (1000) aleksei   (1000)       38 2024-05-25 08:14:43.847386 faster_fifo-1.4.6/setup.cfg
+-rw-rw-r--   0 aleksei   (1000) aleksei   (1000)     1228 2024-05-25 08:04:29.000000 faster_fifo-1.4.6/setup.py
```

### Comparing `faster-fifo-1.4.5/LICENSE` & `faster_fifo-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `faster-fifo-1.4.5/PKG-INFO` & `faster_fifo-1.4.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: faster-fifo
-Version: 1.4.5
-Summary: A faster alternative to Python's standard multiprocessing.Queue (IPC FIFO queue)
-Home-page: https://github.com/alex-petrenko/faster-fifo
-Author: Aleksei Petrenko & Tushar Kumar
-License: MIT
-Keywords: multiprocessing data structures
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 [![tests](https://github.com/alex-petrenko/faster-fifo/actions/workflows/test-ci.yml/badge.svg)](https://github.com/alex-petrenko/faster-fifo/actions/workflows/test-ci.yml)
 [![Downloads](https://pepy.tech/badge/faster-fifo)](https://pepy.tech/project/faster-fifo)
 [<img src="https://img.shields.io/discord/987232982798598164?label=discord">](https://discord.gg/d9VZmMWejh)
 
 <!-- [![codecov](https://codecov.io/gh/alex-petrenko/faster-fifo/branch/master/graph/badge.svg)](https://codecov.io/gh/alex-petrenko/faster-fifo) -->
 
 # faster-fifo
@@ -32,15 +19,15 @@
 - Python 3.6 or newer
 - GCC 4.9.0 or newer
 
 ## Installation
 
 ```pip install faster-fifo```
 
-(on a fresh Linux installation you might need some basic compiling tools `sudo apt install --reinstall build-essential`)
+(on a fresh Linux installation you might need some basic compiling tools `sudo apt install --reinstall build-essential gcc g++`)
 
 ## Manual build instructions
 
 ```
 pip install Cython
 python setup.py build_ext --inplace
 pip install -e .
@@ -120,14 +107,18 @@
 
 `python -m unittest`
 
 (there are also C++ unit tests, should run them if C++ code was altered)
 
 ## Recent PyPI releases
 
+##### v1.4.6
+
+* Added missing `<cstdio>` causing issues with newer g++. Thank you [mesaglio](https://github.com/mesaglio)!
+
 ##### v1.4.5
 
 * Added method `data_size()` to query the total size of the messages in queue (in bytes). Thank you [@LucaNicosia](https://github.com/LucaNicosia)!
 
 ##### v1.4.4
 
 * Fixed an obscure issue with the TLSBuffer ctor being called without arguments (guessing it's Cython's weirdness)
```

### Comparing `faster-fifo-1.4.5/README.md` & `faster_fifo-1.4.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: faster-fifo
+Version: 1.4.6
+Summary: A faster alternative to Python's standard multiprocessing.Queue (IPC FIFO queue)
+Home-page: https://github.com/alex-petrenko/faster-fifo
+Author: Aleksei Petrenko & Tushar Kumar
+License: MIT
+Keywords: multiprocessing data structures
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: setuptools>=45.2.0
+Requires-Dist: cython>=0.29
+Provides-Extra: dev
+Requires-Dist: twine; extra == "dev"
+Requires-Dist: numpy<2.0,>=1.18.1; extra == "dev"
+
 [![tests](https://github.com/alex-petrenko/faster-fifo/actions/workflows/test-ci.yml/badge.svg)](https://github.com/alex-petrenko/faster-fifo/actions/workflows/test-ci.yml)
 [![Downloads](https://pepy.tech/badge/faster-fifo)](https://pepy.tech/project/faster-fifo)
 [<img src="https://img.shields.io/discord/987232982798598164?label=discord">](https://discord.gg/d9VZmMWejh)
 
 <!-- [![codecov](https://codecov.io/gh/alex-petrenko/faster-fifo/branch/master/graph/badge.svg)](https://codecov.io/gh/alex-petrenko/faster-fifo) -->
 
 # faster-fifo
@@ -19,15 +36,15 @@
 - Python 3.6 or newer
 - GCC 4.9.0 or newer
 
 ## Installation
 
 ```pip install faster-fifo```
 
-(on a fresh Linux installation you might need some basic compiling tools `sudo apt install --reinstall build-essential`)
+(on a fresh Linux installation you might need some basic compiling tools `sudo apt install --reinstall build-essential gcc g++`)
 
 ## Manual build instructions
 
 ```
 pip install Cython
 python setup.py build_ext --inplace
 pip install -e .
@@ -107,14 +124,18 @@
 
 `python -m unittest`
 
 (there are also C++ unit tests, should run them if C++ code was altered)
 
 ## Recent PyPI releases
 
+##### v1.4.6
+
+* Added missing `<cstdio>` causing issues with newer g++. Thank you [mesaglio](https://github.com/mesaglio)!
+
 ##### v1.4.5
 
 * Added method `data_size()` to query the total size of the messages in queue (in bytes). Thank you [@LucaNicosia](https://github.com/LucaNicosia)!
 
 ##### v1.4.4
 
 * Fixed an obscure issue with the TLSBuffer ctor being called without arguments (guessing it's Cython's weirdness)
```

### Comparing `faster-fifo-1.4.5/cpp_faster_fifo/cpp_lib/faster_fifo.cpp` & `faster_fifo-1.4.6/cpp_faster_fifo/cpp_lib/faster_fifo.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 #include <mutex>
 #include <cassert>
 #include <cstring>
+#include <cstdio>
 
 #include <pthread.h>
 #include <sys/time.h>
 
 #include "faster_fifo.hpp"
 
+#include <stdio.h>
+
 
 // Logs the error message to stderr and in debug mode triggers assert if the condition is false.
 #define LOG_ASSERT(cond, msg) \
     if (!(cond)) { \
         fprintf(stderr, "%s:%d %s\n", __FILE__, __LINE__, (msg)); \
         assert(((msg), (cond))); \
     }
 
 
 struct Queue {
-    explicit Queue(size_t max_size_bytes) : max_size_bytes(max_size_bytes) {
+    explicit Queue(size_t max_size_bytes, size_t maxsize) : max_size_bytes(max_size_bytes), maxsize(maxsize) {
         pthread_mutexattr_init(&mutex_attr);
         pthread_mutexattr_setpshared(&mutex_attr, PTHREAD_PROCESS_SHARED);
         pthread_mutex_init(&mutex, &mutex_attr);
 
         pthread_condattr_init(&cond_attr);
         pthread_condattr_setpshared(&cond_attr, PTHREAD_PROCESS_SHARED);
 
@@ -31,18 +34,25 @@
 
     ~Queue() = default;
 
     [[nodiscard]] size_t get_max_buffer_size() const {
         return max_size_bytes;
     }
 
-    [[nodiscard]] bool can_fit(size_t data_size) const {
-        return size + data_size <= max_size_bytes;
+    [[nodiscard]] size_t get_max_size() const {
+        return maxsize;
     }
 
+[[nodiscard]] bool can_fit(size_t data_size, size_t additional_size) const {
+    const bool cond_size = size + data_size <= max_size_bytes;
+    const bool cond_num = num_elem + additional_size <= maxsize;
+
+    return cond_size && cond_num;
+}
+
     /// This function does not check if there is enough space in the circular buffer, assuming the check
     /// has been performed.
     void circular_buffer_write(uint8_t *buffer, const uint8_t *data, const size_t data_size) {
         if (tail + data_size < max_size_bytes) {
             // all data fits before the wrapping point
             memcpy(buffer + tail, data, data_size);
             tail += data_size;
@@ -72,26 +82,27 @@
             memcpy(data + before_wrap, buffer, after_wrap);
             new_head = after_wrap;
         }
 
         const auto new_size = size - read_size;
 
         LOG_ASSERT(new_head < max_size_bytes, "Circular buffer head pointer is incorrect");
-        LOG_ASSERT(new_size >= 0 && new_size < max_size_bytes, "New size is incorrect after reading from buffer");
+        LOG_ASSERT(new_size >= 0 && new_size <= max_size_bytes, "New size is incorrect after reading from buffer");
 
         if (pop_message) {
             head = new_head;
             size = new_size;
         }
     }
 
 public:
     // 9 bytes is the min message size. 8 bytes for the size and 1 for the minimal message
     static const size_t MIN_MSG_SIZE = sizeof(size_t) + 1;
     size_t max_size_bytes;
+    size_t maxsize;
     size_t head = 0, tail = 0, size = 0;
     size_t num_elem = 0;
 
     pthread_mutexattr_t mutex_attr{};
     pthread_mutex_t mutex{};
 
     pthread_condattr_t cond_attr{};
@@ -114,16 +125,16 @@
 };
 
 
 size_t queue_object_size() {
     return sizeof(Queue);
 }
 
-void create_queue(void *queue_obj_memory, size_t max_size_bytes) {
-    new(queue_obj_memory) Queue(max_size_bytes);  // placement new
+void create_queue(void *queue_obj_memory, size_t max_size_bytes, size_t maxsize) {
+    new(queue_obj_memory) Queue(max_size_bytes, maxsize); 
 }
 
 struct timeval float_seconds_to_timeval(float seconds) {
     struct timeval wait_timeval{};
 
     constexpr uint64_t million = 1000000UL;
     const auto wait_us = uint64_t(seconds * million);
@@ -163,15 +174,16 @@
 
     {
         size_t total_size = num_msgs * sizeof(size_t);
         for (size_t i = 0; i < num_msgs; ++i)
             total_size += msg_sizes[i];
 
         auto wait_remaining = float_seconds_to_timeval(timeout);
-        while (!q->can_fit(total_size)) {
+        while (!q->can_fit(total_size, num_msgs)) {
+            
             if (!block || !timer_positive(wait_remaining))
                 return Q_FULL;
 
             // If there are any consumers waiting, wake them up!
             if (q->not_empty_n_waiters > 0)
                 pthread_cond_signal(&q->not_empty);
 
@@ -188,15 +200,15 @@
 
         // Increment count by one as one element has been added
         ++q->num_elem;
     }
     
     if (q->not_empty_n_waiters > 0)
         pthread_cond_signal(&q->not_empty);
-    else if (q->not_full_n_waiters && q->can_fit(Queue::MIN_MSG_SIZE)) {
+    else if (q->not_full_n_waiters && q->can_fit(Queue::MIN_MSG_SIZE, 1)) {
         // In the case of many producers and one batched consumer, producers
         // should wake each other up as the batched consumer is only guaranteed to
         // wake up 1 producer its pthread_cond_signal(&q->not_full).
 
         pthread_cond_signal(&q->not_full);
     }
 
@@ -277,9 +289,10 @@
     auto q = (Queue *)queue_obj;
     return q->size;
 }
 
 bool is_queue_full(void *queue_obj) {
     auto q = (Queue *)queue_obj;
     constexpr size_t min_message_size = 1;
-    return !q->can_fit(min_message_size + sizeof(min_message_size));
+    constexpr size_t min_messages_count = 1;
+    return !q->can_fit(min_message_size + sizeof(min_message_size), min_messages_count);
 }
```

### Comparing `faster-fifo-1.4.5/cpp_faster_fifo/cpp_lib/faster_fifo.hpp` & `faster_fifo-1.4.6/cpp_faster_fifo/cpp_lib/faster_fifo.hpp`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 constexpr int Q_SUCCESS = 0,
               Q_EMPTY = -1,
               Q_FULL = -2,
               Q_MSG_BUFFER_TOO_SMALL = -3;
 
 
 size_t queue_object_size();
-void create_queue(void *queue_obj, size_t max_size_bytes);
+void create_queue(void *queue_obj, size_t max_size_bytes, size_t maxsize);
 
 int queue_put(void *queue_obj, void *buffer, const void **msgs_data, const size_t *msg_sizes, size_t num_msgs, int block, float timeout);
 
 int queue_get(void *queue_obj, void *buffer,
               void *msg_buffer, size_t msg_buffer_size,
               size_t max_messages_to_get, size_t max_bytes_to_get,
               size_t *messages_read, size_t *bytes_read, size_t *messages_size,
```

### Comparing `faster-fifo-1.4.5/cpp_faster_fifo/tests/comparison_tests.py` & `faster_fifo-1.4.6/cpp_faster_fifo/tests/comparison_tests.py`

 * *Files 14% similar despite different names*

```diff
@@ -169,7 +169,27 @@
 # i5-4200U (dual-core CPU)
 # [2020-05-22 18:03:55,061][09146] Configuration (1, 1, 200000), timing [ff: 2.09s, ff_many: 2.20s, mp.queue: 7.86s]
 # [2020-05-22 18:03:55,061][09146] Configuration (1, 10, 200000), timing [ff: 4.01s, ff_many: 3.88s, mp.queue: 11.68s]
 # [2020-05-22 18:03:55,061][09146] Configuration (10, 1, 100000), timing [ff: 16.68s, ff_many: 5.98s, mp.queue: 44.48s]
 # [2020-05-22 18:03:55,061][09146] Configuration (3, 20, 100000), timing [ff: 7.83s, ff_many: 7.49s, mp.queue: 22.59s]
 # [2020-05-22 18:03:55,061][09146] Configuration (20, 3, 50000), timing [ff: 22.30s, ff_many: 6.35s, mp.queue: 66.30s]
 # [2020-05-22 18:03:55,061][09146] Configuration (20, 20, 50000), timing [ff: 14.39s, ff_many: 15.78s, mp.queue: 78.75s]
+
+
+# Update (2023.08.11)
+# Ubuntu 18, Intel(R) Xeon(R) CPU E5-2650, Python 3.9.16
+# [2023-08-11 17:37:58,796][40648] Configuration (1, 1, 200000), timing [ff: 2.28s, ff_many: 2.46s, mp.queue: 3.48s]
+# [2023-08-11 17:37:58,796][40648] Configuration (1, 10, 200000), timing [ff: 2.71s, ff_many: 2.82s, mp.queue: 11.65s]
+# [2023-08-11 17:37:58,796][40648] Configuration (10, 1, 100000), timing [ff: 13.69s, ff_many: 1.95s, mp.queue: 18.39s]
+# [2023-08-11 17:37:58,796][40648] Configuration (3, 20, 100000), timing [ff: 2.97s, ff_many: 2.30s, mp.queue: 21.10s]
+# [2023-08-11 17:37:58,796][40648] Configuration (20, 3, 50000), timing [ff: 19.75s, ff_many: 1.08s, mp.queue: 23.24s]
+# [2023-08-11 17:37:58,796][40648] Configuration (20, 20, 50000), timing [ff: 2.81s, ff_many: 3.73s, mp.queue: 70.49s]
+# Ran 1 test in 206.923s
+
+# Ubuntu 18, Intel(R) Xeon(R) CPU E5-2650, Python 3.11.4
+# [2023-08-11 17:46:36,056][42634] Configuration (1, 1, 200000), timing [ff: 1.67s, ff_many: 1.77s, mp.queue: 2.45s]
+# [2023-08-11 17:46:36,056][42634] Configuration (1, 10, 200000), timing [ff: 2.27s, ff_many: 2.31s, mp.queue: 5.61s]
+# [2023-08-11 17:46:36,056][42634] Configuration (10, 1, 100000), timing [ff: 13.15s, ff_many: 1.86s, mp.queue: 14.05s]
+# [2023-08-11 17:46:36,056][42634] Configuration (3, 20, 100000), timing [ff: 2.97s, ff_many: 2.23s, mp.queue: 12.71s]
+# [2023-08-11 17:46:36,056][42634] Configuration (20, 3, 50000), timing [ff: 19.22s, ff_many: 0.99s, mp.queue: 17.28s]
+# [2023-08-11 17:46:36,056][42634] Configuration (20, 20, 50000), timing [ff: 2.60s, ff_many: 3.52s, mp.queue: 43.30s]
+# Ran 1 test in 149.972s
```

### Comparing `faster-fifo-1.4.5/cpp_faster_fifo/tests/test_faster_fifo.py` & `faster_fifo-1.4.6/cpp_faster_fifo/tests/test_faster_fifo.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from faster_fifo import Queue
 
 
 ch = logging.StreamHandler()
 ch.setLevel(logging.DEBUG)
 
-log = logging.getLogger('rl')
+log = logging.getLogger("rl")
 log.setLevel(logging.DEBUG)
 log.handlers = []  # No duplicated handlers
 log.propagate = False  # workaround for duplicated logs in ipython
 log.addHandler(ch)
 
 MSG_SIZE = 5
 BIG_MSG_MAX_SIZE = int(1e7)
@@ -34,50 +34,54 @@
 
 def produce(q, p_idx, num_messages, make_msg_fn: Callable = make_msg):
     i = 0
     while i < num_messages:
         try:
             q.put(make_msg_fn(i), timeout=0.01)
             if i % 50000 == 0:
-                log.info('Produce: %d %d', i, p_idx)
+                log.info("Produce: %d %d", i, p_idx)
             i += 1
         except Full:
             # time.sleep(0.001)
             pass
-    log.info('Done! %d', p_idx)
+    log.info("Done! %d", p_idx)
 
 
 def consume(q, p_idx, consume_many, total_num_messages=int(1e9)):
     messages_received = 0
     while True:
         try:
             msgs = q.get_many(timeout=0.01, max_messages_to_get=consume_many)
             for msg in msgs:
                 messages_received += 1
                 if msg[0] % 50000 == 0:
-                    log.info('Consume: %r %d num_msgs: %d', msg, p_idx, len(msgs))
+                    log.info("Consume: %r %d num_msgs: %d", msg, p_idx, len(msgs))
             if messages_received >= total_num_messages:
                 break
         except Empty:
             if q.is_closed():
                 break
-    log.info('Done! %d', p_idx)
+    log.info("Done! %d", p_idx)
 
 
 class TestFastQueue(TestCase):
     def test_singleproc(self):
         q = Queue()
         produce(q, 0, num_messages=20)
         consume(q, 0, consume_many=2, total_num_messages=20)
         q.close()
         self.assertIsNone(q.last_error)
 
     def run_producer_consumer(
-            self, n_producers: int, n_consumers: int, n_msg: int, execution_medium: type,
-            make_msg_fn: Callable,
+        self,
+        n_producers: int,
+        n_consumers: int,
+        n_msg: int,
+        execution_medium: type,
+        make_msg_fn: Callable,
     ):
         q = Queue()
         consume_many = 1000
         producers = []
         consumers = []
         for j in range(n_producers):
             p = execution_medium(target=produce, args=(q, j, n_msg, make_msg_fn))
@@ -92,97 +96,116 @@
         for p in producers:
             p.join()
         q.close()
         for c in consumers:
             c.join()
 
         self.assertIsNone(q.last_error)
-        log.info('Exit...')
+        log.info("Exit...")
 
     def test_multiprocessing(self):
         self.run_producer_consumer(
-            20, 3, 100001, execution_medium=multiprocessing.Process, make_msg_fn=make_msg,
+            20,
+            3,
+            100001,
+            execution_medium=multiprocessing.Process,
+            make_msg_fn=make_msg,
         )
 
     def test_multithreading(self):
         self.run_producer_consumer(
-            20, 3, 100001, execution_medium=threading.Thread, make_msg_fn=make_msg,
+            20,
+            3,
+            100001,
+            execution_medium=threading.Thread,
+            make_msg_fn=make_msg,
         )
 
     def test_multiprocessing_big_msg(self):
         self.run_producer_consumer(
-            20, 3, 1001, execution_medium=multiprocessing.Process, make_msg_fn=make_big_msg,
+            20,
+            3,
+            1001,
+            execution_medium=multiprocessing.Process,
+            make_msg_fn=make_big_msg,
         )
 
     def test_multithreading_big_msg(self):
         self.run_producer_consumer(
-            20, 20, 101, execution_medium=threading.Thread, make_msg_fn=make_big_msg,
+            20,
+            20,
+            101,
+            execution_medium=threading.Thread,
+            make_msg_fn=make_big_msg,
         )
 
     def test_msg(self):
         q = Queue(max_size_bytes=1000)
 
-        py_obj = dict(a=42, b=33, c=(1, 2, 3), d=[1, 2, 3], e='123', f=b'kkk')
+        py_obj = dict(a=42, b=33, c=(1, 2, 3), d=[1, 2, 3], e="123", f=b"kkk")
         q.put_nowait(py_obj)
         res = q.get_nowait()
-        log.debug('got object %r', res)
+        log.debug("got object %r", res)
         self.assertEqual(py_obj, res)
 
     def test_msg_many(self):
         q = Queue(max_size_bytes=100000)
 
-        py_objs = [dict(a=42, b=33, c=(1, 2, 3), d=[1, 2, 3], e='123', f=b'kkk') for _ in range(5)]
+        py_objs = [
+            dict(a=42, b=33, c=(1, 2, 3), d=[1, 2, 3], e="123", f=b"kkk")
+            for _ in range(5)
+        ]
         q.put_many_nowait(py_objs)
         res = q.get_many_nowait()
 
         while not q.empty():
             res.extend(q.get_many_nowait())
 
-        log.debug('Got object %r', res)
+        log.debug("Got object %r", res)
         self.assertEqual(py_objs, res)
 
         q.put_nowait(py_objs)
         res = q.get_nowait()
         self.assertEqual(py_objs, res)
 
     def test_queue_size(self):
         q = Queue(max_size_bytes=1000)
         py_obj_1 = dict(a=10, b=20)
         py_obj_2 = dict(a=30, b=40)
         q.put_nowait(py_obj_1)
         q.put_nowait(py_obj_2)
         q_size_bef = q.qsize()
-        log.debug('Queue size after put -  %d', q_size_bef)
+        log.debug("Queue size after put -  %d", q_size_bef)
         num_messages = 0
         want_to_read = 2
         while num_messages < want_to_read:
             msgs = q.get_many()
             print(msgs)
             num_messages += len(msgs)
         self.assertEqual(type(q_size_bef), int)
         q_size_af = q.qsize()
-        log.debug('Queue size after get -  %d', q_size_af)
+        log.debug("Queue size after get -  %d", q_size_af)
         self.assertEqual(q_size_af, 0)
 
     def test_queue_empty(self):
         q = Queue(max_size_bytes=1000)
         self.assertTrue(q.empty())
-        py_obj = dict(a=42, b=33, c=(1, 2, 3), d=[1, 2, 3], e='123', f=b'kkk')
+        py_obj = dict(a=42, b=33, c=(1, 2, 3), d=[1, 2, 3], e="123", f=b"kkk")
         q.put_nowait(py_obj)
         q_empty = q.empty()
         self.assertFalse(q_empty)
 
     def test_queue_data_size(self):
         q = Queue(max_size_bytes=1000)
         py_obj = dict(a=10, b=20)
         q.put_nowait(py_obj)
         py_obj_size = q.data_size()
-        log.debug('Queue data size after put -  %d', py_obj_size)
+        log.debug("Queue data size after put -  %d", py_obj_size)
         q.put_nowait(py_obj)
-        self.assertTrue(q.data_size(), 2*py_obj_size)
+        self.assertTrue(q.data_size(), 2 * py_obj_size)
 
     def test_queue_full(self):
         q = Queue(max_size_bytes=60)
         self.assertFalse(q.full())
         py_obj = (1, 2)
         while True:
             try:
@@ -191,43 +214,113 @@
                 self.assertTrue(q.full())
                 break
 
     def test_queue_usage(self):
         q = Queue(1000 * 1000)  # specify the size of the circular buffer in the ctor
 
         # any pickle-able Python object can be added to the queue
-        py_obj = dict(a=42, b=33, c=(1, 2, 3), d=[1, 2, 3], e='123', f=b'kkk')
+        py_obj = dict(a=42, b=33, c=(1, 2, 3), d=[1, 2, 3], e="123", f=b"kkk")
         q.put(py_obj)
         assert q.qsize() == 1
 
         retrieved = q.get()
         assert q.empty()
         assert py_obj == retrieved
 
         for i in range(100):
             try:
                 q.put(py_obj, timeout=0.1)
             except Full:
-                log.debug('Queue is full!')
+                log.debug("Queue is full!")
 
         num_received = 0
         while num_received < 100:
             # get multiple messages at once, returns a list of messages for better performance in many-to-few scenarios
             # get_many does not guarantee that all max_messages_to_get will be received on the first call, in fact
             # no such guarantee can be made in multiprocessing systems.
             # get_many() will retrieve as many messages as there are available AND can fit in the pre-allocated memory
             # buffer. The size of the buffer is increased gradually to match demand.
             messages = q.get_many(max_messages_to_get=100)
             num_received += len(messages)
 
         try:
             q.get(timeout=0.1)
-            assert True, 'This won\'t be called'
+            assert True, "This won't be called"
         except Empty:
-            log.debug('Queue is empty')
+            log.debug("Queue is empty")
+
+    def test_max_size(self):
+        q = Queue(
+            max_size_bytes=1000, maxsize=5
+        )  # Create a queue with a maximum of 5 messages
+
+        for i in range(5):
+            q.put_nowait(make_msg(i))  # Add 5 messages to the queue
+
+        q_size_bef = q.qsize()
+        log.debug("Queue size after put -  %d", q_size_bef)
+
+        self.assertTrue(q.full())  # Check that the queue is full
+
+        with self.assertRaises(
+            Full
+        ):  # Check that adding another message raises the Full exception
+            q.put_nowait(make_msg(5))
+        q.get_many()
+        self.assertFalse(q.full())  # Check that the queue is not full
+
+    def test_queue_full_msgs(self):
+        q = Queue(maxsize=5)
+        self.assertFalse(q.full())
+        py_obj = (1, 2)
+        for _ in range(5):
+            q.put_nowait(py_obj)
+        self.assertTrue(q.full())
+        with self.assertRaises(Full):
+            q.put_nowait(py_obj)
+
+    def test_producer_consumer_msgs(self):
+        self.run_producer_consumer_msgs(
+            1,
+            1,
+            10,
+            threading.Thread,
+            make_msg,
+        )
+
+    def run_producer_consumer_msgs(
+        self,
+        n_producers: int,
+        n_consumers: int,
+        n_msg: int,
+        execution_medium: type,
+        make_msg_fn: Callable,
+    ):
+        q = Queue(maxsize=n_msg * n_producers)
+        consume_many = 5
+        producers = []
+        consumers = []
+        for j in range(n_producers):
+            p = execution_medium(target=produce, args=(q, j, n_msg, make_msg_fn))
+            producers.append(p)
+        for j in range(n_consumers):
+            p = execution_medium(target=consume, args=(q, j, consume_many))
+            consumers.append(p)
+        for c in consumers:
+            c.start()
+        for p in producers:
+            p.start()
+        for p in producers:
+            p.join()
+        q.close()
+        for c in consumers:
+            c.join()
+
+        self.assertIsNone(q.last_error)
+        log.info("Exit...")
 
 
 def spawn_producer(data_q_):
     for i in range(10):
         data = [1, 2, 3, i]
         data_q_.put(data)
 
@@ -236,25 +329,23 @@
     i = 0
     while True:
         try:
             data = data_q_.get(timeout=0.5)
             print(data)
             i += 1
         except Empty:
-            print('Read', i, 'messages')
+            print("Read", i, "messages")
             break
 
 
 class TestSpawn(TestCase):
     def test_spawn_ctx(self):
-        ctx = multiprocessing.get_context('spawn')
+        ctx = multiprocessing.get_context("spawn")
         data_q = Queue(1000 * 1000)
-        procs = [
-            ctx.Process(target=spawn_producer, args=(data_q,)) for _ in range(2)
-        ]
+        procs = [ctx.Process(target=spawn_producer, args=(data_q,)) for _ in range(2)]
         procs.append(ctx.Process(target=spawn_consumer, args=(data_q,)))
 
         # add data to the queue and read some of it back to make sure all buffers are initialized before
         # the new process is spawned (such that we need to pickle everything)
         for i in range(10):
             data_q.put(self.test_spawn_ctx.__name__)
         msgs = data_q.get_many(max_messages_to_get=2)
@@ -265,24 +356,28 @@
         for p in procs:
             p.join()
 
 
 # this can actually be used instead of Pickle if we know that we need to support only specific data types
 # should be significantly faster
 def custom_int_deserializer(msg_bytes):
-    return int.from_bytes(msg_bytes, 'big')
+    return int.from_bytes(msg_bytes, "big")
 
 
 def custom_int_serializer(x):
-    return x.to_bytes(4, 'big')
+    return x.to_bytes(4, "big")
 
 
 class TestCustomSerializer(TestCase):
     def test_custom_loads_dumps(self):
-        q = Queue(max_size_bytes=100000, loads=custom_int_deserializer, dumps=custom_int_serializer)
+        q = Queue(
+            max_size_bytes=100000,
+            loads=custom_int_deserializer,
+            dumps=custom_int_serializer,
+        )
         for i in range(32767):
             q.put(i)
             deserialized_i = q.get()
             assert i == deserialized_i
 
 
 class SubQueue(Queue):
@@ -291,20 +386,23 @@
 
 def worker_test_subclass(_x: Queue, _y: Queue):
     pass
 
 
 class TestSubclass(TestCase):
     def test_subclass(self):
-        ctx = multiprocessing.get_context('spawn')
+        ctx = multiprocessing.get_context("spawn")
 
         q = Queue()
         q.put(1)
         q.get()
         qs = SubQueue()  # Works with Queue()
         qs.put(2)
         qs.get()
 
         from multiprocessing.pool import Pool as MpPool
-        pool = MpPool(2, initializer=worker_test_subclass, initargs=(q, qs), context=ctx)
+
+        pool = MpPool(
+            2, initializer=worker_test_subclass, initargs=(q, qs), context=ctx
+        )
         pool.close()
         pool.join()
```

### Comparing `faster-fifo-1.4.5/faster_fifo.egg-info/PKG-INFO` & `faster_fifo-1.4.6/faster_fifo.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 Metadata-Version: 2.1
 Name: faster-fifo
-Version: 1.4.5
+Version: 1.4.6
 Summary: A faster alternative to Python's standard multiprocessing.Queue (IPC FIFO queue)
 Home-page: https://github.com/alex-petrenko/faster-fifo
 Author: Aleksei Petrenko & Tushar Kumar
 License: MIT
 Keywords: multiprocessing data structures
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: setuptools>=45.2.0
+Requires-Dist: cython>=0.29
+Provides-Extra: dev
+Requires-Dist: twine; extra == "dev"
+Requires-Dist: numpy<2.0,>=1.18.1; extra == "dev"
 
 [![tests](https://github.com/alex-petrenko/faster-fifo/actions/workflows/test-ci.yml/badge.svg)](https://github.com/alex-petrenko/faster-fifo/actions/workflows/test-ci.yml)
 [![Downloads](https://pepy.tech/badge/faster-fifo)](https://pepy.tech/project/faster-fifo)
 [<img src="https://img.shields.io/discord/987232982798598164?label=discord">](https://discord.gg/d9VZmMWejh)
 
 <!-- [![codecov](https://codecov.io/gh/alex-petrenko/faster-fifo/branch/master/graph/badge.svg)](https://codecov.io/gh/alex-petrenko/faster-fifo) -->
 
@@ -32,15 +36,15 @@
 - Python 3.6 or newer
 - GCC 4.9.0 or newer
 
 ## Installation
 
 ```pip install faster-fifo```
 
-(on a fresh Linux installation you might need some basic compiling tools `sudo apt install --reinstall build-essential`)
+(on a fresh Linux installation you might need some basic compiling tools `sudo apt install --reinstall build-essential gcc g++`)
 
 ## Manual build instructions
 
 ```
 pip install Cython
 python setup.py build_ext --inplace
 pip install -e .
@@ -120,14 +124,18 @@
 
 `python -m unittest`
 
 (there are also C++ unit tests, should run them if C++ code was altered)
 
 ## Recent PyPI releases
 
+##### v1.4.6
+
+* Added missing `<cstdio>` causing issues with newer g++. Thank you [mesaglio](https://github.com/mesaglio)!
+
 ##### v1.4.5
 
 * Added method `data_size()` to query the total size of the messages in queue (in bytes). Thank you [@LucaNicosia](https://github.com/LucaNicosia)!
 
 ##### v1.4.4
 
 * Fixed an obscure issue with the TLSBuffer ctor being called without arguments (guessing it's Cython's weirdness)
```

### Comparing `faster-fifo-1.4.5/faster_fifo.egg-info/SOURCES.txt` & `faster_fifo-1.4.6/faster_fifo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `faster-fifo-1.4.5/faster_fifo.pyx` & `faster_fifo-1.4.6/faster_fifo.pyx`

 * *Files 5% similar despite different names*

```diff
@@ -56,31 +56,32 @@
 
 cdef size_t bytes_to_ptr(b):
     ptr = ctypes.cast(b, ctypes.POINTER(ctypes.c_byte))
     return ctypes.addressof(ptr.contents)
 
 
 class Queue:
-    def __init__(self, max_size_bytes=DEFAULT_CIRCULAR_BUFFER_SIZE, loads=None, dumps=None):
+    def __init__(self, max_size_bytes=DEFAULT_CIRCULAR_BUFFER_SIZE, maxsize=int(1e9), loads=None, dumps=None):
         self.max_size_bytes = max_size_bytes
+        self.maxsize = maxsize  # default maxsize
         self.max_bytes_to_read = self.max_size_bytes  # by default, read the whole queue if necessary
 
         # allow per-instance serializer overriding
         if loads is not None:
             self.loads = loads
         if dumps is not None:
             self.dumps = dumps
 
         self.closed = multiprocessing.RawValue(ctypes.c_bool, False)
 
         queue_obj_size = Q.queue_object_size()
         self.queue_obj_buffer = multiprocessing.RawArray(ctypes.c_ubyte, queue_obj_size)
         self.shared_memory = multiprocessing.RawArray(ctypes.c_ubyte, max_size_bytes)
 
-        Q.create_queue(<void *> q_addr(self), max_size_bytes)
+        Q.create_queue(<void *> q_addr(self), max_size_bytes, maxsize)
 
         self.message_buffer: TLSBuffer = TLSBuffer(None)
 
         self.last_error: Optional[str] = None
 
     def _error(self, message):
         self.last_error = message
@@ -146,21 +147,31 @@
             pass
         elif status == Q.Q_FULL:
             raise Full()
         else:
             raise Exception(f'Unexpected queue error {status}')
 
     def put(self, x, block=True, timeout=DEFAULT_TIMEOUT):
-        return self.put_many([x], block, timeout)
+        status = self.put_many([x], block, timeout)
+        if status == Q.Q_FULL:
+            raise Full()
+        return status
 
     def put_many_nowait(self, xs):
-        return self.put_many(xs, block=False)
+        status = self.put_many(xs, block=False)
+        if status == Q.Q_FULL:
+            raise Full()
+        return status
 
     def put_nowait(self, x):
-        return self.put_many_nowait([x])
+        status = self.put_many_nowait([x])
+        if status == Q.Q_FULL:
+            raise Full()
+        return status
+
 
     def get_many(self, block=True, timeout=DEFAULT_TIMEOUT, max_messages_to_get=int(1e9)):
         if self.message_buffer.val is None:
             self.reallocate_msg_buffer(INITIAL_RECV_BUFFER_SIZE)  # initialize a small buffer at first, it will be increased later if needed
 
         messages_read = ctypes.c_size_t(0)
         cdef size_t messages_read_ptr = ctypes.addressof(messages_read)
```

### Comparing `faster-fifo-1.4.5/faster_fifo_def.pxd` & `faster_fifo-1.4.6/faster_fifo_def.pxd`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # cython: language_level=3
 # cython: boundscheck=False
 from libcpp cimport bool
 cdef extern from 'cpp_faster_fifo/cpp_lib/faster_fifo.hpp':
     int Q_SUCCESS = 0, Q_EMPTY = -1, Q_FULL = -2, Q_MSG_BUFFER_TOO_SMALL = -3;
 
     size_t queue_object_size();
-    void create_queue(void *queue_obj_memory, size_t max_size_bytes);
+    void create_queue(void *queue_obj_memory, size_t max_size_bytes, size_t maxsize);
 
     int queue_put(void *queue_obj, void *buffer, const void **msgs_data, const size_t *msg_sizes, size_t num_msgs, int block, float timeout) nogil;
     int queue_get(void *queue_obj, void *buffer,
                   void *msg_buffer, size_t msg_buffer_size,
                   size_t max_messages_to_get, size_t max_bytes_to_get,
                   size_t *messages_read, size_t *bytes_read, size_t *messages_size, int block, float timeout) nogil;
     size_t get_queue_size(void *queue_obj);
```

### Comparing `faster-fifo-1.4.5/faster_fifo_reduction/__init__.py` & `faster_fifo-1.4.6/faster_fifo_reduction/__init__.py`

 * *Files identical despite different names*

### Comparing `faster-fifo-1.4.5/setup.py` & `faster_fifo-1.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     # Information
     name='faster-fifo',
-    version='1.4.5',
+    version='1.4.6',
     url='https://github.com/alex-petrenko/faster-fifo',
     author='Aleksei Petrenko & Tushar Kumar',
     license='MIT',
     keywords='multiprocessing data structures',
     description='A faster alternative to Python\'s standard multiprocessing.Queue (IPC FIFO queue)',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

