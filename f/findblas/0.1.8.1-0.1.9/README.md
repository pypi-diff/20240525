# Comparing `tmp/findblas-0.1.8.1.tar.gz` & `tmp/findblas-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/findblas-0.1.8.1.tar", last modified: Tue Mar 17 21:00:33 2020, max compression
+gzip compressed data, was "dist/findblas-0.1.9.tar", last modified: Sun May  3 07:51:58 2020, max compression
```

## Comparing `findblas-0.1.8.1.tar` & `findblas-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2020-03-17 21:00:33.000000 findblas-0.1.8.1/
--rw-r--r--   0 david     (1000) david     (1000)     1317 2020-01-21 19:21:26.000000 findblas-0.1.8.1/LICENSE
--rw-r--r--   0 david     (1000) david     (1000)       56 2020-01-21 19:21:30.000000 findblas-0.1.8.1/MANIFEST.in
--rw-r--r--   0 david     (1000) david     (1000)      222 2020-03-17 21:00:33.000000 findblas-0.1.8.1/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)     7210 2020-01-24 16:08:40.000000 findblas-0.1.8.1/README.md
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2020-03-17 21:00:33.000000 findblas-0.1.8.1/findblas/
--rw-r--r--   0 david     (1000) david     (1000)    24445 2020-03-17 20:59:39.000000 findblas-0.1.8.1/findblas/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)     5581 2020-03-12 07:36:36.000000 findblas-0.1.8.1/findblas/distutils.py
--rw-r--r--   0 david     (1000) david     (1000)    34256 2020-03-10 09:35:03.000000 findblas-0.1.8.1/findblas/findblas.h
--rw-r--r--   0 david     (1000) david     (1000)    34912 2020-01-21 19:21:30.000000 findblas-0.1.8.1/findblas/rtd_mock.h
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2020-03-17 21:00:33.000000 findblas-0.1.8.1/findblas.egg-info/
--rw-r--r--   0 david     (1000) david     (1000)      222 2020-03-17 21:00:33.000000 findblas-0.1.8.1/findblas.egg-info/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)      249 2020-03-17 21:00:33.000000 findblas-0.1.8.1/findblas.egg-info/SOURCES.txt
--rw-r--r--   0 david     (1000) david     (1000)        1 2020-03-17 21:00:33.000000 findblas-0.1.8.1/findblas.egg-info/dependency_links.txt
--rw-r--r--   0 david     (1000) david     (1000)        9 2020-03-17 21:00:33.000000 findblas-0.1.8.1/findblas.egg-info/top_level.txt
--rw-r--r--   0 david     (1000) david     (1000)       38 2020-03-17 21:00:33.000000 findblas-0.1.8.1/setup.cfg
--rw-r--r--   0 david     (1000) david     (1000)      362 2020-03-17 20:59:46.000000 findblas-0.1.8.1/setup.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2020-05-03 07:51:58.000000 findblas-0.1.9/
+-rw-r--r--   0 david     (1000) david     (1000)       56 2020-05-03 07:49:52.000000 findblas-0.1.9/MANIFEST.in
+-rw-r--r--   0 david     (1000) david     (1000)      220 2020-05-03 07:51:58.000000 findblas-0.1.9/PKG-INFO
+-rw-r--r--   0 david     (1000) david     (1000)     7210 2020-05-03 07:49:52.000000 findblas-0.1.9/README.md
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2020-05-03 07:51:58.000000 findblas-0.1.9/findblas/
+-rw-r--r--   0 david     (1000) david     (1000)    24445 2020-05-03 07:49:52.000000 findblas-0.1.9/findblas/__init__.py
+-rw-r--r--   0 david     (1000) david     (1000)     5621 2020-05-03 07:50:51.000000 findblas-0.1.9/findblas/distutils.py
+-rw-r--r--   0 david     (1000) david     (1000)    34256 2020-05-03 07:49:52.000000 findblas-0.1.9/findblas/findblas.h
+-rw-r--r--   0 david     (1000) david     (1000)    34912 2020-05-03 07:49:52.000000 findblas-0.1.9/findblas/rtd_mock.h
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2020-05-03 07:51:58.000000 findblas-0.1.9/findblas.egg-info/
+-rw-r--r--   0 david     (1000) david     (1000)      220 2020-05-03 07:51:58.000000 findblas-0.1.9/findblas.egg-info/PKG-INFO
+-rw-r--r--   0 david     (1000) david     (1000)      241 2020-05-03 07:51:58.000000 findblas-0.1.9/findblas.egg-info/SOURCES.txt
+-rw-r--r--   0 david     (1000) david     (1000)        1 2020-05-03 07:51:58.000000 findblas-0.1.9/findblas.egg-info/dependency_links.txt
+-rw-r--r--   0 david     (1000) david     (1000)        9 2020-05-03 07:51:58.000000 findblas-0.1.9/findblas.egg-info/top_level.txt
+-rw-r--r--   0 david     (1000) david     (1000)       38 2020-05-03 07:51:58.000000 findblas-0.1.9/setup.cfg
+-rw-r--r--   0 david     (1000) david     (1000)      360 2020-05-03 07:51:07.000000 findblas-0.1.9/setup.py
```

### Comparing `findblas-0.1.8.1/README.md` & `findblas-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `findblas-0.1.8.1/findblas/__init__.py` & `findblas-0.1.9/findblas/__init__.py`

 * *Files identical despite different names*

### Comparing `findblas-0.1.8.1/findblas/distutils.py` & `findblas-0.1.9/findblas/distutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,16 @@
                 txt += "\nHowever, it is missing .lib files - please install them with 'pip install mkl-devel'."
                 raise ValueError(txt)
             elif bool(re.search(r"\.dll$", blas_file)):
                 txt = "Found BLAS library at:\n" + os.path.join(blas_path, blas_file)
                 txt += "\nBut .lib files are missing! Please reinstall it (e.g. 'pip install mkl-devel')."
                 raise ValueError(txt)
             else:
-                print("Installation: Using BLAS library found in:\n" + os.path.join(blas_path, blas_file) + "\n\n")
+            	if platform[:3] != "win":
+                	print("Installation: Using BLAS library found in:\n" + os.path.join(blas_path, blas_file) + "\n\n")
         else:
             flags = ['_FOR_RTD']
             blas_path, blas_file, incl_path, incl_file = [None]*4
 
         ## if no CBLAS and no functions are present, there will be no prototypes for the cblas API
         if "NO_CBLAS" in flags:
             raise ValueError(nocblas_err_msg)
```

### Comparing `findblas-0.1.8.1/findblas/findblas.h` & `findblas-0.1.9/findblas/findblas.h`

 * *Files identical despite different names*

### Comparing `findblas-0.1.8.1/findblas/rtd_mock.h` & `findblas-0.1.9/findblas/rtd_mock.h`

 * *Files identical despite different names*

