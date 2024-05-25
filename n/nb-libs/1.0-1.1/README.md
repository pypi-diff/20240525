# Comparing `tmp/nb_libs-1.0.tar.gz` & `tmp/nb_libs-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\nb_libs-1.0.tar", last modified: Thu Apr 18 03:00:52 2024, max compression
+gzip compressed data, was "nb_libs-1.1.tar", last modified: Sat May 25 15:08:46 2024, max compression
```

## Comparing `nb_libs-1.0.tar` & `nb_libs-1.1.tar`

### file list

```diff
@@ -1,26 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 03:00:52.000000 nb_libs-1.0/
--rw-rw-rw-   0        0        0       41 2024-04-18 02:51:35.000000 nb_libs-1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      995 2024-04-18 03:00:52.000000 nb_libs-1.0/PKG-INFO
--rw-rw-rw-   0        0        0      169 2024-04-18 03:00:48.000000 nb_libs-1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 03:00:52.000000 nb_libs-1.0/nb_libs/
--rw-rw-rw-   0        0        0        0 2024-04-18 02:55:05.000000 nb_libs-1.0/nb_libs/__init__.py
--rw-rw-rw-   0        0        0     3106 2023-11-17 02:18:55.000000 nb_libs-1.0/nb_libs/auto_git.py
--rw-rw-rw-   0        0        0     2041 2024-01-02 03:07:27.000000 nb_libs-1.0/nb_libs/code_line_statistics.py
--rw-rw-rw-   0        0        0      362 2023-10-23 03:14:12.000000 nb_libs-1.0/nb_libs/dict2json.py
--rw-rw-rw-   0        0        0      490 2023-10-23 03:14:12.000000 nb_libs-1.0/nb_libs/global_dict.py
--rw-rw-rw-   0        0        0      487 2024-04-16 03:39:38.000000 nb_libs-1.0/nb_libs/lazy_importer.py
--rw-rw-rw-   0        0        0       21 2024-03-20 10:00:54.000000 nb_libs-1.0/nb_libs/nb_time.py
--rw-rw-rw-   0        0        0     2841 2024-04-03 08:52:42.000000 nb_libs-1.0/nb_libs/path_helper.py
--rw-rw-rw-   0        0        0     1418 2023-03-15 02:37:59.000000 nb_libs-1.0/nb_libs/restart_programe_by_interval.py
--rw-rw-rw-   0        0        0      229 2023-11-24 10:39:15.000000 nb_libs-1.0/nb_libs/sys_frame_uitils.py
-drwxrwxrwx   0        0        0        0 2024-04-18 03:00:52.000000 nb_libs-1.0/nb_libs.egg-info/
--rw-rw-rw-   0        0        0      995 2024-04-18 03:00:50.000000 nb_libs-1.0/nb_libs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      498 2024-04-18 03:00:50.000000 nb_libs-1.0/nb_libs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 03:00:50.000000 nb_libs-1.0/nb_libs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-04-18 03:00:50.000000 nb_libs-1.0/nb_libs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-18 03:00:50.000000 nb_libs-1.0/nb_libs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 03:00:52.000000 nb_libs-1.0/setup.cfg
--rw-rw-rw-   0        0        0     1821 2024-04-18 03:00:48.000000 nb_libs-1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-18 03:00:52.000000 nb_libs-1.0/tests/
--rw-rw-rw-   0        0        0      379 2023-03-15 02:57:54.000000 nb_libs-1.0/tests/test_restart_programe_by_interval.py
--rw-rw-rw-   0        0        0      934 2024-02-29 11:16:03.000000 nb_libs-1.0/tests/tests_time.py
+drwxrwxrwx   0        0        0        0 2024-05-25 15:08:46.255695 nb_libs-1.1/
+-rw-rw-rw-   0        0        0       41 2024-05-24 14:51:14.000000 nb_libs-1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      995 2024-05-25 15:08:46.253690 nb_libs-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      169 2024-05-24 14:51:14.000000 nb_libs-1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-25 15:08:46.180666 nb_libs-1.1/nb_libs/
+-rw-rw-rw-   0        0        0        0 2024-05-24 14:51:14.000000 nb_libs-1.1/nb_libs/__init__.py
+-rw-rw-rw-   0        0        0     3106 2024-04-09 14:11:27.000000 nb_libs-1.1/nb_libs/auto_git.py
+-rw-rw-rw-   0        0        0     2041 2024-04-09 14:11:27.000000 nb_libs-1.1/nb_libs/code_line_statistics.py
+-rw-rw-rw-   0        0        0      362 2023-10-22 05:45:27.000000 nb_libs-1.1/nb_libs/dict2json.py
+-rw-rw-rw-   0        0        0      490 2023-10-22 05:47:50.000000 nb_libs-1.1/nb_libs/global_dict.py
+-rw-rw-rw-   0        0        0      487 2024-05-24 14:51:14.000000 nb_libs-1.1/nb_libs/lazy_importer.py
+-rw-rw-rw-   0        0        0     1650 2024-05-24 14:51:14.000000 nb_libs-1.1/nb_libs/markdown2pdf.py
+-rw-rw-rw-   0        0        0     3186 2024-05-24 19:36:58.000000 nb_libs-1.1/nb_libs/memory_leak_analysis.py
+-rw-rw-rw-   0        0        0       21 2024-04-09 14:11:27.000000 nb_libs-1.1/nb_libs/nb_time.py
+-rw-rw-rw-   0        0        0     3311 2024-05-24 14:51:14.000000 nb_libs-1.1/nb_libs/path_helper.py
+-rw-rw-rw-   0        0        0     3527 2024-05-24 14:51:14.000000 nb_libs-1.1/nb_libs/pydantic_helper.py
+-rw-rw-rw-   0        0        0     1418 2023-10-22 05:28:25.000000 nb_libs-1.1/nb_libs/restart_programe_by_interval.py
+-rw-rw-rw-   0        0        0     1605 2024-05-24 14:51:14.000000 nb_libs-1.1/nb_libs/sys_frame_uitils.py
+drwxrwxrwx   0        0        0        0 2024-05-25 15:08:46.202679 nb_libs-1.1/nb_libs.egg-info/
+-rw-rw-rw-   0        0        0      995 2024-05-25 15:08:45.000000 nb_libs-1.1/nb_libs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      656 2024-05-25 15:08:45.000000 nb_libs-1.1/nb_libs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 15:08:45.000000 nb_libs-1.1/nb_libs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-05-25 15:08:45.000000 nb_libs-1.1/nb_libs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-25 15:08:45.000000 nb_libs-1.1/nb_libs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-25 15:08:46.255695 nb_libs-1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1821 2024-05-25 14:55:30.000000 nb_libs-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 15:08:46.247691 nb_libs-1.1/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-24 18:29:31.000000 nb_libs-1.1/tests/__init__.py
+-rw-rw-rw-   0        0        0      760 2024-05-24 19:32:57.000000 nb_libs-1.1/tests/t_mem_leak.py
+-rw-rw-rw-   0        0        0      225 2024-05-24 18:55:50.000000 nb_libs-1.1/tests/t_mem_leak2.py
+-rw-rw-rw-   0        0        0      379 2023-10-22 05:28:25.000000 nb_libs-1.1/tests/test_restart_programe_by_interval.py
+-rw-rw-rw-   0        0        0      128 2024-05-24 14:51:14.000000 nb_libs-1.1/tests/testai.py
+-rw-rw-rw-   0        0        0      934 2024-04-09 14:11:27.000000 nb_libs-1.1/tests/tests_time.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `nb_libs-1.0/PKG-INFO` & `nb_libs-1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb_libs
-Version: 1.0
+Version: 1.1
 Summary: nb_libs 不想分开分发很多个不同功能单独的包,各种小功能杂项放在一起,具体功能看代码.
 Home-page: https://github.com/ydf0509/nb_libs
 Author: bfzs
 Author-email: ydf0509@sohu.com
 Maintainer: ydf
 Maintainer-email: ydf0509@sohu.com
 License: BSD License
```

### Comparing `nb_libs-1.0/nb_libs/auto_git.py` & `nb_libs-1.1/nb_libs/auto_git.py`

 * *Files identical despite different names*

### Comparing `nb_libs-1.0/nb_libs/code_line_statistics.py` & `nb_libs-1.1/nb_libs/code_line_statistics.py`

 * *Files identical despite different names*

### Comparing `nb_libs-1.0/nb_libs/path_helper.py` & `nb_libs-1.1/nb_libs/path_helper.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,38 +4,46 @@
 import types
 import typing
 from pathlib import Path, WindowsPath, PosixPath
 from nb_log import LoggerMixin
 
 
 class PathHelper(LoggerMixin):
-    def __init__(self, path: typing.Union[os.PathLike, str]):
-        self.path = Path(path)
+    def __init__(self, path: typing.Union[os.PathLike, str],is_always_resolve=False):
+        """
+        :param path:
+        :param is_always_resolve:  是否总是使用绝对路径.
+        """
+        self._is_always_resolve = is_always_resolve
+        path_obj = Path(path)
+        if is_always_resolve:
+            path_obj = path_obj.resolve()
+        self.path :Path= path_obj
 
-    def rglob_files(self, pattern: str, is_resolve: bool = False) -> typing.List[Path]:
+    def rglob_files(self, pattern: str, ) -> typing.List[Path]:
         entries = self.path.rglob(pattern, )
         files = []
         # 遍历文件夹和文件
         for entry in entries:
-            if is_resolve:
+            if self._is_always_resolve:
                 entry = entry.resolve()
             if entry.is_file():
                 # print('file: ', entry)
                 pass
                 files.append(entry.resolve())
             elif entry.is_dir():
                 pass
                 # print('dir: ', entry)
         return files
 
-    def rglob_dirs(self, pattern: str, is_resolve: bool = False) -> typing.List[Path]:
+    def rglob_dirs(self, pattern: str, ) -> typing.List[Path]:
         entries = self.path.rglob(pattern, )
         dirs = []
         for entry in entries:
-            if is_resolve:
+            if self._is_always_resolve:
                 entry = entry.resolve()
             if entry.is_file():
                 # print('file: ', entry)
                 pass
             elif entry.is_dir():
                 # print('dir: ', entry)
                 pass
@@ -51,22 +59,27 @@
         module_spec.loader.exec_module(module)
         return module
         # except FileNotFoundError:
         #     self.logger.exception(f"Module file '{self.path}' not found.")
         # except Exception as e:
         #     self.logger.exception(f"Failed to import module '{module_name}': {str(e)}")
 
-    def auto_import_pyfiles_in_dir(self, ) -> None:
-        for file_path in self.rglob_files('*.py'):
+    def auto_import_pyfiles_in_dir(self, pattern: str='*.py') -> None:
+        for file_path in self.rglob_files(pattern):
             self.logger.debug(f'导入模块 {file_path}')
             if Path(file_path) == Path(sys._getframe(1).f_code.co_filename):
                 self.logger.warning(f'排除导入调用PathHelper的模块自身 {file_path}')  # 否则下面的import这个文件,会造成无限懵逼死循环
                 continue
             self.__class__(file_path).import_as_module()
 
+    def __str__(self):
+        return f'''<PathHelper["{self.path}"]>'''
+
 
 if __name__ == '__main__':
     print(type(Path('/')))
-    print(list(PathHelper(r'../').rglob_files('*', is_resolve=True)))
+    print(PathHelper('./',is_always_resolve=True))
+    print(PathHelper('./',is_always_resolve=True).path)
+    print(list(PathHelper(r'../').rglob_files('*', )))
     print(PathHelper(r'D:\codes\nb_libs\nb_libs/dict2json.py').import_as_module())
 
     PathHelper(Path(__file__).parent.parent.joinpath('tests/test_import_dir')).auto_import_pyfiles_in_dir()
```

### Comparing `nb_libs-1.0/nb_libs/restart_programe_by_interval.py` & `nb_libs-1.1/nb_libs/restart_programe_by_interval.py`

 * *Files identical despite different names*

### Comparing `nb_libs-1.0/nb_libs.egg-info/PKG-INFO` & `nb_libs-1.1/nb_libs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb-libs
-Version: 1.0
+Version: 1.1
 Summary: nb_libs 不想分开分发很多个不同功能单独的包,各种小功能杂项放在一起,具体功能看代码.
 Home-page: https://github.com/ydf0509/nb_libs
 Author: bfzs
 Author-email: ydf0509@sohu.com
 Maintainer: ydf
 Maintainer-email: ydf0509@sohu.com
 License: BSD License
```

### Comparing `nb_libs-1.0/setup.py` & `nb_libs-1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # filepath = ((Path(__file__).parent / Path('README.md')).absolute()).as_posix()
 filepath = 'README.md'
 print(filepath)
 
 setup(
     name='nb_libs',  #
-    version="1.0",
+    version="1.1",
     description=('nb_libs 不想分开分发很多个不同功能单独的包,各种小功能杂项放在一起,具体功能看代码.'),
     keywords=["nb_libs",],
     # long_description=open('README.md', 'r',encoding='utf8').read(),
     long_description_content_type="text/markdown",
     long_description=open(filepath, 'r', encoding='utf8').read(),
     # data_files=[filepath],
     author='bfzs',
```

### Comparing `nb_libs-1.0/tests/tests_time.py` & `nb_libs-1.1/tests/tests_time.py`

 * *Files identical despite different names*

