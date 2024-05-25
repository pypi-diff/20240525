# Comparing `tmp/p2d-0.2.3a1.tar.gz` & `tmp/p2d-0.2.3a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p2d-0.2.3a1.tar", max compression
+gzip compressed data, was "p2d-0.2.3a2.tar", max compression
```

## Comparing `p2d-0.2.3a1.tar` & `p2d-0.2.3a2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1093 2024-02-08 14:43:19.274051 p2d-0.2.3a1/LICENSE
--rw-r--r--   0        0        0     3782 2024-02-08 14:43:19.274051 p2d-0.2.3a1/README.cn.md
--rw-r--r--   0        0        0     3539 2024-02-08 14:43:19.274051 p2d-0.2.3a1/README.md
--rw-r--r--   0        0        0       44 2024-02-08 14:43:19.274051 p2d-0.2.3a1/p2d/__init__.py
--rw-r--r--   0        0        0      911 2024-02-08 14:43:19.274051 p2d-0.2.3a1/p2d/asset/config.toml
--rw-r--r--   0        0        0     4506 2024-02-08 14:43:19.274051 p2d-0.2.3a1/p2d/cli.py
--rw-r--r--   0        0        0    23374 2024-02-08 14:43:19.274051 p2d-0.2.3a1/p2d/p2d.py
--rw-r--r--   0        0        0     1082 2024-02-08 14:43:19.274051 p2d-0.2.3a1/p2d/testlib/LICENSE
--rw-r--r--   0        0        0     5145 2024-02-08 14:43:19.274051 p2d-0.2.3a1/p2d/testlib/README.md
--rw-r--r--   0        0        0     5396 2024-02-08 14:43:19.274051 p2d-0.2.3a1/p2d/testlib/patch/domjudge.patch
--rw-r--r--   0        0        0      591 2024-02-08 14:43:19.274051 p2d-0.2.3a1/p2d/testlib/read.me
--rw-r--r--   0        0        0   199384 2024-02-08 14:43:19.274051 p2d-0.2.3a1/p2d/testlib/testlib.h
--rw-r--r--   0        0        0      825 2024-02-08 14:43:19.274051 p2d-0.2.3a1/p2d/typing.py
--rw-r--r--   0        0        0     1252 2024-02-08 14:43:19.274051 p2d-0.2.3a1/p2d/utils.py
--rw-r--r--   0        0        0     1462 2024-02-08 14:43:19.278051 p2d-0.2.3a1/pyproject.toml
--rw-r--r--   0        0        0     8507 1970-01-01 00:00:00.000000 p2d-0.2.3a1/PKG-INFO
+-rw-r--r--   0        0        0     1093 2024-02-09 06:16:29.345432 p2d-0.2.3a2/LICENSE
+-rw-r--r--   0        0        0     3740 2024-02-09 06:16:29.345432 p2d-0.2.3a2/README.cn.md
+-rw-r--r--   0        0        0     3498 2024-02-09 06:16:29.345432 p2d-0.2.3a2/README.md
+-rw-r--r--   0        0        0       44 2024-02-09 06:16:29.345432 p2d-0.2.3a2/p2d/__init__.py
+-rw-r--r--   0        0        0      911 2024-02-09 06:16:29.345432 p2d-0.2.3a2/p2d/asset/config.toml
+-rw-r--r--   0        0        0     4522 2024-02-09 06:16:29.345432 p2d-0.2.3a2/p2d/cli.py
+-rw-r--r--   0        0        0    23502 2024-02-09 06:16:29.345432 p2d-0.2.3a2/p2d/p2d.py
+-rw-r--r--   0        0        0     1082 2024-02-09 06:16:29.345432 p2d-0.2.3a2/p2d/testlib/LICENSE
+-rw-r--r--   0        0        0     5145 2024-02-09 06:16:29.345432 p2d-0.2.3a2/p2d/testlib/README.md
+-rw-r--r--   0        0        0     5396 2024-02-09 06:16:29.345432 p2d-0.2.3a2/p2d/testlib/patch/domjudge.patch
+-rw-r--r--   0        0        0      591 2024-02-09 06:16:29.345432 p2d-0.2.3a2/p2d/testlib/read.me
+-rw-r--r--   0        0        0   199384 2024-02-09 06:16:29.349432 p2d-0.2.3a2/p2d/testlib/testlib.h
+-rw-r--r--   0        0        0      825 2024-02-09 06:16:29.349432 p2d-0.2.3a2/p2d/typing.py
+-rw-r--r--   0        0        0     1252 2024-02-09 06:16:29.349432 p2d-0.2.3a2/p2d/utils.py
+-rw-r--r--   0        0        0     1462 2024-02-09 06:16:29.349432 p2d-0.2.3a2/pyproject.toml
+-rw-r--r--   0        0        0     8424 1970-01-01 00:00:00.000000 p2d-0.2.3a2/PKG-INFO
```

### Comparing `p2d-0.2.3a1/LICENSE` & `p2d-0.2.3a2/LICENSE`

 * *Files identical despite different names*

### Comparing `p2d-0.2.3a1/README.cn.md` & `p2d-0.2.3a2/README.cn.md`

 * *Files 6% similar despite different names*

```diff
@@ -53,36 +53,34 @@
 
 ## API 使用示例
 
 这是一个将 [`problems.yaml`](https://ccs-specs.icpc.io/draft/contest_package#problemsyaml) 中定义的比赛中的所有题目转换为 DOMjudge 题目包的示例。
 
 ```python
 import yaml
-
 from pathlib import Path
 
-from p2d import convert_polygon_to_domjudge
+from p2d import convert
 
 polygon = Path('/path/to/polygon-packages')
 domjudge = Path('/path/to/domjudge-packages')
 
 with open(domjudge / 'problems.yaml') as f:
     problems = yaml.safe_load(f)
 
 for problem in problems:
     prob_id = problem['id']
-    convert_polygon_to_domjudge(
+    convert(
         polygon / f'{prob_id}.zip',
         domjudge / f'{prob_id}.zip',
         code=problem['label'],
         color=problem['rgb'],
     )
 ```
 
-
 ## 开发
 
 ```bash
 # install
 poetry install
 
 # build
```

### Comparing `p2d-0.2.3a1/README.md` & `p2d-0.2.3a2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -55,28 +55,27 @@
 
 ## API Example
 
 This is an example to convert all problems in a contest defined in [`problems.yaml`](https://ccs-specs.icpc.io/draft/contest_package#problemsyaml) to DOMjudge package.
 
 ```python
 import yaml
-
 from pathlib import Path
 
-from p2d import convert_polygon_to_domjudge
+from p2d import convert
 
 polygon = Path('/path/to/polygon-packages')
 domjudge = Path('/path/to/domjudge-packages')
 
 with open(domjudge / 'problems.yaml') as f:
     problems = yaml.safe_load(f)
 
 for problem in problems:
     prob_id = problem['id']
-    convert_polygon_to_domjudge(
+    convert(
         polygon / f'{prob_id}.zip',
         domjudge / f'{prob_id}.zip',
         code=problem['label'],
         color=problem['rgb'],
     )
 ```
```

### Comparing `p2d-0.2.3a1/p2d/asset/config.toml` & `p2d-0.2.3a2/p2d/asset/config.toml`

 * *Files identical despite different names*

### Comparing `p2d-0.2.3a1/p2d/cli.py` & `p2d-0.2.3a2/p2d/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,44 +2,47 @@
 from argparse import ArgumentParser, ArgumentError
 from pathlib import Path
 from typing import cast, List, Optional
 
 import betterlogging as logging  # type: ignore
 
 from . import __version__
-from .p2d import convert_polygon_to_domjudge, DEFAULT_CODE, DEFAULT_COLOR
+from .p2d import convert, DEFAULT_CODE, DEFAULT_COLOR
 from .utils import load_config
 from .typing import Config
 
 
-def main(cmdline_args: Optional[List[str]] = None) -> int:
+def main(argv: Optional[List[str]] = None) -> int:
 
     parser = ArgumentParser(description='Process Polygon Package to Domjudge Package.')
     parser.add_argument('package', type=Path, help='path of the polygon package directory')
     parser.add_argument('--code', type=str, default=DEFAULT_CODE, help='problem short name in domjudge')
-    parser.add_argument('--color', type=str, default=DEFAULT_COLOR, help='problem color in domjudge (in #RRGGBB format)')
+    parser.add_argument('--color', type=str, default=DEFAULT_COLOR,
+                        help='problem color in domjudge (in #RRGGBB format)')
     parser.add_argument('-l', '--log-level', default='info',
                         help='set log level (debug, info, warning, error, critical)')
     parser.add_argument('-v', '--version', action='version', version=__version__)
     parser.add_argument('-y', '--yes', action='store_true', help='skip confirmation')
     parser.add_argument('-o', '--output', type=Path, help='path of the output package')
     parser.add_argument('--default', action='store_true', help='force use the default output validator.')
-    parser.add_argument('--validator-flags', nargs='*', help='add some flags to the output validator, only works when "--default" is set.')
-    parser.add_argument('--auto', action='store_true', help='use the default output validator if the checker is defined in config and can be replaced by the default one.')
-    parser.add_argument('--memory-limit', type=int,
-                        help='override the memory limit for DOMjudge package (in MB), default is using the memory limit defined in polygon package, -1 means use DOMjudge default')  # default use polygon default
+    parser.add_argument('--validator-flags', nargs='*',
+                        help='add some flags to the output validator, only works when "--default" is set.')
+    parser.add_argument('--auto', action='store_true',
+                        help='use the default output validator if the checker is defined in config and can be replaced by the default one.')
+    parser.add_argument('--memory-limit', type=int,  # default use polygon default
+                        help='override the memory limit for DOMjudge package (in MB), default is using the memory limit defined in polygon package, -1 means use DOMjudge default')
     parser.add_argument('--output-limit', type=int, default=-1,
                         help='override the output limit for DOMjudge package (in MB), default is using the default output limit in DOMjudge setting, -1 means use DOMjudge default')
     parser.add_argument('--replace-sample', action='store_true',
                         help='replace the sample input and output with the one shipped with problem statement (e.g. prevent the sample output is different from the main and correct solution).')
     parser.add_argument('--hide-sample', action='store_true',
                         help='hide the sample input and output from the problem statement, no sample data will be available for the contestants (force True if this is an interactive problem).')
     parser.add_argument('--config', type=Path, default='config.toml',
                         help='path of the config file to override the default config, default is using "config.toml" in current directory')
-    args = parser.parse_args(cmdline_args)
+    args = parser.parse_args(argv)
 
     logging.basic_colorized_config(level=args.log_level.upper())
     logger = logging.getLogger(__name__)
 
     try:
         config_file = Path(args.config)
         if config_file.is_file():
@@ -64,15 +67,15 @@
             'validator_flags': args.validator_flags,
             'memory_limit': args.memory_limit,
             'output_limit': args.output_limit,
             'skip_confirmation': args.yes,
             'config': config,
         }
 
-        convert_polygon_to_domjudge(
+        convert(
             args.package,
             args.output,
             **_kwargs,
         )
     except ArgumentError as e:
         logger.error(e)
         sys.exit(2)
```

### Comparing `p2d-0.2.3a1/p2d/p2d.py` & `p2d-0.2.3a2/p2d/p2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,17 @@
     ) -> None:
         self.method = method
         self.description = description
         self.cmd = cmd
         self.sample = sample
 
     def __str__(self):
-        return f'{self.description} {"[GEN] " + self.cmd if self.cmd else ""}'.strip()
+        description = self.description if self.description else ''
+        cmd = f'[GEN] {self.cmd}' if self.cmd else ''
+        return f'{description} {cmd}'.strip()
 
 
 class Problem:
     """
     The problem class.
     """
 
@@ -292,15 +294,16 @@
         ini_content = (f'short-name = {self.short_name}',
                        f'timelimit = {self._problem.timelimit}',
                        f'color = {self.color}')
         for line in ini_content:
             logger.info(line)
 
         with open(ini_file, 'w', encoding='utf-8') as f:
-            f.write('\n'.join(ini_content) + '\n')
+            f.write('\n'.join(ini_content))
+            f.write('\n')
 
         return self
 
     def _write_yaml(self) -> Polygon2DOMjudge:
         logger.debug('Add \'problem.yaml\':')
         yaml_content: Dict[str, Any] = dict(name=self._problem.name)
         memorylimit, outputlimit = self._problem.memorylimit, self._problem.outputlimit
@@ -399,14 +402,15 @@
             shutil.copyfile(input_src, input_dst)
             shutil.copyfile(output_src, output_dst)
 
             if test.__str__():
                 logger.info(f'{test.__str__()}')
                 with open(desc_dst, 'w', encoding='utf-8') as f:
                     f.write(test.__str__())
+                    f.write('\n')
 
         return self
 
     def _add_jury_solutions(self) -> Polygon2DOMjudge:
         logger.debug('Add jury solutions:')
 
         ensure_dir(self.temp_dir / 'submissions' / 'accepted')
@@ -484,27 +488,32 @@
         return self._write_ini() \
             ._write_yaml() \
             ._add_tests() \
             ._add_jury_solutions() \
             ._archive()
 
 
-def _confirm(package_dir, temp_dir, output_file, skip_confirmation=False):
+def _confirm(
+    package_dir: StrPath,
+    output_file: StrPath,
+    skip_confirmation: bool = False
+) -> None:
     logger.info('This is Polygon2DOMjudge by cubercsl.')
     logger.info('Process Polygon Package to DOMjudge Package.')
     logger.info("Version: {}".format(__version__))
 
     if sys.platform.startswith('win'):
         logger.warning('It is not recommended running on windows.')
 
     logger.info(f'Package directory: {package_dir}')
-    logger.info(f'Temp directory: {temp_dir}')
     logger.info(f'Output file: {output_file}.zip')
     if not skip_confirmation:
-        input("Press enter to continue...")
+        if input('Are you sure to continue? [y/N]').lower() == 'y':
+            return
+        sys.exit(0)
 
 
 class Options(TypedDict, total=False):
     force_default_validator: bool
     auto_detect_std_checker: bool
     validator_flags: ValidatorFlags
     replace_sample: bool
@@ -512,15 +521,15 @@
     config: Optional[Config]
     memory_limit: int
     output_limit: int
     skip_confirmation: bool
     code: str  # alias of short_name
 
 
-def convert_polygon_to_domjudge(
+def convert(
     package: StrPath, /,
     output: Optional[StrPath] = None, *,
     short_name: str = DEFAULT_CODE,
     color: str = DEFAULT_COLOR,
     **kwargs: Unpack[Options]
 ) -> None:
     """Convert a Polygon package to a DOMjudge package.
@@ -577,27 +586,27 @@
                 output_file = Path(output).resolve()
         else:
             output_file = Path.cwd() / short_name
 
         if Path(output_file.name + '.zip').resolve().exists():
             raise FileExistsError(errno.EEXIST, os.strerror(errno.EEXIST), f'{output_file.name}.zip')
 
-        _confirm(package_dir, domjudge_temp_dir, output_file, skip_confirmation=skip_confirmation)
+        _confirm(package_dir, output_file, skip_confirmation=skip_confirmation)
 
         p = Polygon2DOMjudge(package_dir, domjudge_temp_dir, output_file, short_name, color, **_kwargs)
 
         if kwargs.get('memory_limit'):
             p.override_memory_limit(cast(int, kwargs['memory_limit']))
         if kwargs.get('output_limit'):
             p.override_output_limit(cast(int, kwargs['output_limit']))
         p.process()
 
 
 __all__ = [
-    'convert_polygon_to_domjudge',
+    'convert',
     'DEFAULT_CODE',
     'DEFAULT_COLOR',
     'DEFAULT_CONFIG_FILE',
     'Options',
     'Polygon2DOMjudge',
     'ProcessError',
     'Problem',
```

### Comparing `p2d-0.2.3a1/p2d/testlib/LICENSE` & `p2d-0.2.3a2/p2d/testlib/LICENSE`

 * *Files identical despite different names*

### Comparing `p2d-0.2.3a1/p2d/testlib/README.md` & `p2d-0.2.3a2/p2d/testlib/README.md`

 * *Files identical despite different names*

### Comparing `p2d-0.2.3a1/p2d/testlib/patch/domjudge.patch` & `p2d-0.2.3a2/p2d/testlib/patch/domjudge.patch`

 * *Files identical despite different names*

### Comparing `p2d-0.2.3a1/p2d/testlib/read.me` & `p2d-0.2.3a2/p2d/testlib/read.me`

 * *Files identical despite different names*

### Comparing `p2d-0.2.3a1/p2d/testlib/testlib.h` & `p2d-0.2.3a2/p2d/testlib/testlib.h`

 * *Files identical despite different names*

### Comparing `p2d-0.2.3a1/p2d/typing.py` & `p2d-0.2.3a2/p2d/typing.py`

 * *Files identical despite different names*

### Comparing `p2d-0.2.3a1/p2d/utils.py` & `p2d-0.2.3a2/p2d/utils.py`

 * *Files identical despite different names*

### Comparing `p2d-0.2.3a1/pyproject.toml` & `p2d-0.2.3a2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "p2d"
-version = "0.2.3a1"
+version = "0.2.3a2"
 description = "Simple python script converting polygon package to domjudge(kattis) package"
 license = "MIT"
 authors = ["cubercsl <hi@cubercsl.site>"]
 maintainers = ["cubercsl <hi@cubercsl.site>", "Dup4 <hi@dup4.com>"]
 readme = ["README.md", "README.cn.md"]
 homepage = "https://github.com/cn-xcpc-tools/Polygon2DOMjudge"
 repository = "https://github.com/cn-xcpc-tools/Polygon2DOMjudge"
```

### Comparing `p2d-0.2.3a1/PKG-INFO` & `p2d-0.2.3a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p2d
-Version: 0.2.3a1
+Version: 0.2.3a2
 Summary: Simple python script converting polygon package to domjudge(kattis) package
 Home-page: https://github.com/cn-xcpc-tools/Polygon2DOMjudge
 License: MIT
 Keywords: Polygon,DOMjudge,Kattis,Codeforces
 Author: cubercsl
 Author-email: hi@cubercsl.site
 Maintainer: cubercsl
@@ -83,28 +83,27 @@
 
 ## API Example
 
 This is an example to convert all problems in a contest defined in [`problems.yaml`](https://ccs-specs.icpc.io/draft/contest_package#problemsyaml) to DOMjudge package.
 
 ```python
 import yaml
-
 from pathlib import Path
 
-from p2d import convert_polygon_to_domjudge
+from p2d import convert
 
 polygon = Path('/path/to/polygon-packages')
 domjudge = Path('/path/to/domjudge-packages')
 
 with open(domjudge / 'problems.yaml') as f:
     problems = yaml.safe_load(f)
 
 for problem in problems:
     prob_id = problem['id']
-    convert_polygon_to_domjudge(
+    convert(
         polygon / f'{prob_id}.zip',
         domjudge / f'{prob_id}.zip',
         code=problem['label'],
         color=problem['rgb'],
     )
 ```
 
@@ -184,36 +183,34 @@
 
 ## API 使用示例
 
 这是一个将 [`problems.yaml`](https://ccs-specs.icpc.io/draft/contest_package#problemsyaml) 中定义的比赛中的所有题目转换为 DOMjudge 题目包的示例。
 
 ```python
 import yaml
-
 from pathlib import Path
 
-from p2d import convert_polygon_to_domjudge
+from p2d import convert
 
 polygon = Path('/path/to/polygon-packages')
 domjudge = Path('/path/to/domjudge-packages')
 
 with open(domjudge / 'problems.yaml') as f:
     problems = yaml.safe_load(f)
 
 for problem in problems:
     prob_id = problem['id']
-    convert_polygon_to_domjudge(
+    convert(
         polygon / f'{prob_id}.zip',
         domjudge / f'{prob_id}.zip',
         code=problem['label'],
         color=problem['rgb'],
     )
 ```
 
-
 ## 开发
 
 ```bash
 # install
 poetry install
 
 # build
```

