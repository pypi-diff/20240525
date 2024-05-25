# Comparing `tmp/stefutils-0.8.2.tar.gz` & `tmp/stefutils-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stefutils-0.8.2.tar", last modified: Tue Jun  7 22:19:40 2022, max compression
+gzip compressed data, was "stefutils-0.9.0.tar", last modified: Mon Jun 13 19:22:42 2022, max compression
```

## Comparing `stefutils-0.8.2.tar` & `stefutils-0.9.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2022-06-07 22:19:40.966256 stefutils-0.8.2/
--rw-r--r--   0 stefanhg   (501) staff       (20)     1075 2022-04-25 19:27:11.000000 stefutils-0.8.2/LICENSE
--rw-r--r--   0 stefanhg   (501) staff       (20)      769 2022-06-07 22:19:40.966417 stefutils-0.8.2/PKG-INFO
--rw-r--r--   0 stefanhg   (501) staff       (20)      981 2022-04-25 21:38:31.000000 stefutils-0.8.2/README.md
--rw-r--r--   0 stefanhg   (501) staff       (20)       79 2022-06-07 22:19:40.966999 stefutils-0.8.2/setup.cfg
--rw-r--r--   0 stefanhg   (501) staff       (20)     1185 2022-06-07 22:19:32.000000 stefutils-0.8.2/setup.py
-drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2022-06-07 22:19:40.963446 stefutils-0.8.2/stefutil/
--rw-r--r--   0 stefanhg   (501) staff       (20)      261 2022-05-17 15:05:34.000000 stefutils-0.8.2/stefutil/__init__.py
--rw-r--r--   0 stefanhg   (501) staff       (20)      544 2022-04-25 16:47:44.000000 stefutils-0.8.2/stefutil/built_in.py
--rw-r--r--   0 stefanhg   (501) staff       (20)     1266 2022-04-25 23:26:33.000000 stefutils-0.8.2/stefutil/check_args.py
--rw-r--r--   0 stefanhg   (501) staff       (20)     5671 2022-05-17 20:26:52.000000 stefutils-0.8.2/stefutil/concurrency.py
--rw-r--r--   0 stefanhg   (501) staff       (20)     3987 2022-04-26 20:22:48.000000 stefutils-0.8.2/stefutil/container.py
--rw-r--r--   0 stefanhg   (501) staff       (20)      887 2022-04-29 18:26:28.000000 stefutils-0.8.2/stefutil/function.py
--rw-r--r--   0 stefanhg   (501) staff       (20)      739 2022-04-25 19:20:36.000000 stefutils-0.8.2/stefutil/ml.py
--rw-r--r--   0 stefanhg   (501) staff       (20)      490 2022-04-25 23:56:05.000000 stefutils-0.8.2/stefutil/os_n_file.py
--rw-r--r--   0 stefanhg   (501) staff       (20)     4185 2022-05-28 02:09:17.000000 stefutils-0.8.2/stefutil/plot.py
--rw-r--r--   0 stefanhg   (501) staff       (20)    17124 2022-06-07 22:18:22.000000 stefutils-0.8.2/stefutil/prettier.py
--rw-r--r--   0 stefanhg   (501) staff       (20)      906 2022-04-25 16:42:50.000000 stefutils-0.8.2/stefutil/primitive.py
--rw-r--r--   0 stefanhg   (501) staff       (20)     2732 2022-05-10 00:48:53.000000 stefutils-0.8.2/stefutil/project.py
-drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2022-06-07 22:19:40.965901 stefutils-0.8.2/stefutils.egg-info/
--rw-r--r--   0 stefanhg   (501) staff       (20)      769 2022-06-07 22:19:40.000000 stefutils-0.8.2/stefutils.egg-info/PKG-INFO
--rw-r--r--   0 stefanhg   (501) staff       (20)      449 2022-06-07 22:19:40.000000 stefutils-0.8.2/stefutils.egg-info/SOURCES.txt
--rw-r--r--   0 stefanhg   (501) staff       (20)        1 2022-06-07 22:19:40.000000 stefutils-0.8.2/stefutils.egg-info/dependency_links.txt
--rw-r--r--   0 stefanhg   (501) staff       (20)       87 2022-06-07 22:19:40.000000 stefutils-0.8.2/stefutils.egg-info/requires.txt
--rw-r--r--   0 stefanhg   (501) staff       (20)        9 2022-06-07 22:19:40.000000 stefutils-0.8.2/stefutils.egg-info/top_level.txt
+drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2022-06-13 19:22:42.424502 stefutils-0.9.0/
+-rw-r--r--   0 stefanhg   (501) staff       (20)     1075 2022-04-25 19:27:11.000000 stefutils-0.9.0/LICENSE
+-rw-r--r--   0 stefanhg   (501) staff       (20)      769 2022-06-13 19:22:42.424623 stefutils-0.9.0/PKG-INFO
+-rw-r--r--   0 stefanhg   (501) staff       (20)      981 2022-04-25 21:38:31.000000 stefutils-0.9.0/README.md
+-rw-r--r--   0 stefanhg   (501) staff       (20)       79 2022-06-13 19:22:42.425018 stefutils-0.9.0/setup.cfg
+-rw-r--r--   0 stefanhg   (501) staff       (20)     1185 2022-06-13 19:21:54.000000 stefutils-0.9.0/setup.py
+drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2022-06-13 19:22:42.422780 stefutils-0.9.0/stefutil/
+-rw-r--r--   0 stefanhg   (501) staff       (20)      261 2022-05-17 15:05:34.000000 stefutils-0.9.0/stefutil/__init__.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)      544 2022-04-25 16:47:44.000000 stefutils-0.9.0/stefutil/built_in.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)     1266 2022-04-25 23:26:33.000000 stefutils-0.9.0/stefutil/check_args.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)     5671 2022-05-17 20:26:52.000000 stefutils-0.9.0/stefutil/concurrency.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)     3987 2022-04-26 20:22:48.000000 stefutils-0.9.0/stefutil/container.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)      887 2022-04-29 18:26:28.000000 stefutils-0.9.0/stefutil/function.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)      739 2022-04-25 19:20:36.000000 stefutils-0.9.0/stefutil/ml.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)      490 2022-04-25 23:56:05.000000 stefutils-0.9.0/stefutil/os_n_file.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)     4185 2022-05-28 02:09:17.000000 stefutils-0.9.0/stefutil/plot.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)    17701 2022-06-13 19:21:00.000000 stefutils-0.9.0/stefutil/prettier.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)      906 2022-04-25 16:42:50.000000 stefutils-0.9.0/stefutil/primitive.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)     2799 2022-06-13 19:19:50.000000 stefutils-0.9.0/stefutil/project.py
+drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2022-06-13 19:22:42.424282 stefutils-0.9.0/stefutils.egg-info/
+-rw-r--r--   0 stefanhg   (501) staff       (20)      769 2022-06-13 19:22:41.000000 stefutils-0.9.0/stefutils.egg-info/PKG-INFO
+-rw-r--r--   0 stefanhg   (501) staff       (20)      449 2022-06-13 19:22:42.000000 stefutils-0.9.0/stefutils.egg-info/SOURCES.txt
+-rw-r--r--   0 stefanhg   (501) staff       (20)        1 2022-06-13 19:22:42.000000 stefutils-0.9.0/stefutils.egg-info/dependency_links.txt
+-rw-r--r--   0 stefanhg   (501) staff       (20)       87 2022-06-13 19:22:42.000000 stefutils-0.9.0/stefutils.egg-info/requires.txt
+-rw-r--r--   0 stefanhg   (501) staff       (20)        9 2022-06-13 19:22:42.000000 stefutils-0.9.0/stefutils.egg-info/top_level.txt
```

### Comparing `stefutils-0.8.2/LICENSE` & `stefutils-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stefutils-0.8.2/PKG-INFO` & `stefutils-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: stefutils
-Version: 0.8.2
+Version: 0.9.0
 Summary: Machine Learning project startup utilities
 Home-page: https://github.com/StefanHeng/stef-util
-Download-URL: https://github.com/StefanHeng/stef-util/archive/refs/tags/0.8.2.tar.gz
+Download-URL: https://github.com/StefanHeng/stef-util/archive/refs/tags/0.9.0.tar.gz
 Author: Yuzhao Stefan Heng
 Author-email: stefan.hg@outlook.com
 License: MIT
 Keywords: python,nlp,machine-learning,deep-learning
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: MacOS X
```

### Comparing `stefutils-0.8.2/README.md` & `stefutils-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `stefutils-0.8.2/setup.py` & `stefutils-0.9.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.8.2'
+VERSION = '0.9.0'
 DESCRIPTION = 'Machine Learning project startup utilities'
 LONG_DESCRIPTION = 'My commonly used utilities for machine learning projects'
 
 setup(
     name='stefutils',
     version=VERSION,
     license='MIT',
     author='Yuzhao Stefan Heng',
     author_email='stefan.hg@outlook.com',
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     url='https://github.com/StefanHeng/stef-util',
-    download_url='https://github.com/StefanHeng/stef-util/archive/refs/tags/0.8.2.tar.gz',
+    download_url='https://github.com/StefanHeng/stef-util/archive/refs/tags/0.9.0.tar.gz',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'sty', 'colorama', 'pygments',
         'numpy', 'pandas', 'torch', 'transformers',
         'matplotlib', 'seaborn',
         'tqdm', 'icecream'
```

### Comparing `stefutils-0.8.2/stefutil/built_in.py` & `stefutils-0.9.0/stefutil/built_in.py`

 * *Files identical despite different names*

### Comparing `stefutils-0.8.2/stefutil/check_args.py` & `stefutils-0.9.0/stefutil/check_args.py`

 * *Files identical despite different names*

### Comparing `stefutils-0.8.2/stefutil/concurrency.py` & `stefutils-0.9.0/stefutil/concurrency.py`

 * *Files identical despite different names*

### Comparing `stefutils-0.8.2/stefutil/container.py` & `stefutils-0.9.0/stefutil/container.py`

 * *Files identical despite different names*

### Comparing `stefutils-0.8.2/stefutil/function.py` & `stefutils-0.9.0/stefutil/function.py`

 * *Files identical despite different names*

### Comparing `stefutils-0.8.2/stefutil/ml.py` & `stefutils-0.9.0/stefutil/ml.py`

 * *Files identical despite different names*

### Comparing `stefutils-0.8.2/stefutil/plot.py` & `stefutils-0.9.0/stefutil/plot.py`

 * *Files identical despite different names*

### Comparing `stefutils-0.8.2/stefutil/prettier.py` & `stefutils-0.9.0/stefutil/prettier.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 from stefutil.primitive import is_float
 
 
 __all__ = [
     'fmt_num', 'fmt_sizeof', 'fmt_delta', 'sec2mmss', 'round_up_1digit', 'nth_sig_digit', 'now',
     'MyIceCreamDebugger', 'mic',
-    'log', 'log_s', 'logi', 'log_dict', 'log_dict_nc', 'log_dict_id', 'log_dict_pg', 'log_dict_p',
+    'log', 'log_s', 'logi', 'log_list', 'log_dict', 'log_dict_nc', 'log_dict_id', 'log_dict_pg', 'log_dict_p',
     'hex2rgb', 'MyTheme', 'MyFormatter', 'get_logger',
     'MlPrettier', 'MyProgressCallback'
 ]
 
 
 pd.set_option('expand_frame_repr', False)
 pd.set_option('display.precision', 2)
@@ -172,21 +172,31 @@
 def logi(s):
     """
     Syntactic sugar for logging `info` as string
     """
     return log_s(s, c='i')
 
 
+def log_list(lst: List, with_color=True):
+    pref, post = '[', ']'
+    if with_color:
+        pref, post = log_s(pref, c='m'), log_s(post, c='m')
+    lst = [logi(e) for e in lst]
+    return f'{pref}{", ".join(lst)}{post}'
+
+
 def log_dict(d: Dict = None, with_color=True, pad_float: int = 5, sep=': ', **kwargs) -> str:
     """
     Syntactic sugar for logging dict with coloring for console output
     """
     def _log_val(v):
         if isinstance(v, dict):
             return log_dict(v, with_color=with_color)
+        elif isinstance(v, list):
+            return log_list(v, with_color=with_color)
         else:
             if is_float(v):  # Pad only normal, expected floats, intended for metric logging
                 if is_float(v, no_int=True, no_sci=True):
                     v = float(v)
                     return log(v, c='i', as_str=True, pad=pad_float) if with_color else f'{v:>{pad_float}}'
                 else:
                     return logi(v) if with_color else v
@@ -348,15 +358,17 @@
     """
     assert typ in ['stdout', 'file-write']
     logger = logging.getLogger(f'{name} file write' if typ == 'file-write' else name)
     logger.handlers = []  # A crude way to remove prior handlers, ensure only 1 handler per logger
     logger.setLevel(logging.DEBUG)
     if typ == 'stdout':
         handler = logging.StreamHandler(stream=sys.stdout)  # stdout for my own coloring
-    else:
+    else:  # `file-write`
+        if not file_path:
+            raise ValueError(f'{logi(file_path)} must be specified for {logi("file-write")} logging')
         os.makedirs(os.path.dirname(file_path), exist_ok=True)
         handler = logging.FileHandler(file_path)
     handler.setLevel(logging.DEBUG)
     handler.setFormatter(MyFormatter(with_color=typ == 'stdout'))
     logger.addHandler(handler)
     return logger
 
@@ -497,9 +509,14 @@
             _ = logs.pop("total_flos", None)
 
     def on_train_end(self, args, state, control, **kwargs):
         pass
 
 
 if __name__ == '__main__':
-    lg = get_logger('test')
-    lg.info('test')
+    # lg = get_logger('test')
+    # lg.info('test')
+
+    def check_log_lst():
+        lst = ['sda', 'asd']
+        print(log_list(lst))
+    check_log_lst()
```

### Comparing `stefutils-0.8.2/stefutil/primitive.py` & `stefutils-0.9.0/stefutil/primitive.py`

 * *Files identical despite different names*

### Comparing `stefutils-0.8.2/stefutil/project.py` & `stefutils-0.9.0/stefutil/project.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,17 @@
 
 
 class StefUtil:
     """
     Effectively curried functions with my enforced project & dataset structure
         Pass in file paths
     """
+    plot_dir = 'plot'
+    eval_dir = 'eval'
+
     def __init__(
             self, base_path: str = None, project_dir: str = None, package_name: str = None,
             dataset_dir: str = None, model_dir: str = None
     ):
         """
         :param base_path: Absolute system path for root directory that contains a project folder & a data folder
         :param project_dir: Project root directory name that contains a folder for main source files
@@ -54,16 +57,16 @@
         self.pkg_nm = package_name
         self.dset_dir = dataset_dir
         self.model_dir = model_dir
 
         self.proj_path = os_join(self.base_path, self.proj_dir)
         self.dset_path = os_join(self.base_path, self.dset_dir)
         self.model_path = os_join(self.base_path, self.model_dir)
-        self.plot_path = os_join(self.base_path, self.proj_dir, 'plot')
-        self.eval_path = os_join(self.base_path, self.proj_dir, 'eval')
+        self.plot_path = os_join(self.base_path, self.proj_dir, StefUtil.plot_dir)
+        self.eval_path = os_join(self.base_path, self.proj_dir, StefUtil.eval_dir)
         os.makedirs(self.plot_path, exist_ok=True)
         os.makedirs(self.eval_path, exist_ok=True)
 
     def save_fig(self, title, save=True, prefix_time: bool = True):
         """
         :param title: Rendered figure title
         :param save: If true, figure is saved to project plot directory
```

### Comparing `stefutils-0.8.2/stefutils.egg-info/PKG-INFO` & `stefutils-0.9.0/stefutils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: stefutils
-Version: 0.8.2
+Version: 0.9.0
 Summary: Machine Learning project startup utilities
 Home-page: https://github.com/StefanHeng/stef-util
-Download-URL: https://github.com/StefanHeng/stef-util/archive/refs/tags/0.8.2.tar.gz
+Download-URL: https://github.com/StefanHeng/stef-util/archive/refs/tags/0.9.0.tar.gz
 Author: Yuzhao Stefan Heng
 Author-email: stefan.hg@outlook.com
 License: MIT
 Keywords: python,nlp,machine-learning,deep-learning
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: MacOS X
```

