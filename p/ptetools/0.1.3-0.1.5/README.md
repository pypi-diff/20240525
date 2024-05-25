# Comparing `tmp/ptetools-0.1.3.tar.gz` & `tmp/ptetools-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptetools-0.1.3.tar", last modified: Tue Mar 19 20:47:37 2024, max compression
+gzip compressed data, was "ptetools-0.1.5.tar", last modified: Sat May 25 19:34:53 2024, max compression
```

## Comparing `ptetools-0.1.3.tar` & `ptetools-0.1.5.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-03-19 20:47:37.966512 ptetools-0.1.3/
--rw-rw-rw-   0        0        0     1119 2024-03-19 10:32:33.000000 ptetools-0.1.3/LICENSE.md
--rw-rw-rw-   0        0        0     1236 2024-03-19 20:47:37.965513 ptetools-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      330 2024-03-19 10:32:33.000000 ptetools-0.1.3/README.md
--rw-rw-rw-   0        0        0     2212 2024-03-19 20:47:28.000000 ptetools-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-19 20:47:37.967512 ptetools-0.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-19 20:47:37.917508 ptetools-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2024-03-19 20:47:37.930510 ptetools-0.1.3/src/ptetools/
--rw-rw-rw-   0        0        0       49 2024-03-19 10:32:33.000000 ptetools-0.1.3/src/ptetools/__init__.py
--rw-rw-rw-   0        0        0     8797 2024-03-19 10:32:33.000000 ptetools-0.1.3/src/ptetools/optimization.py
--rw-rw-rw-   0        0        0     2257 2024-03-19 10:32:33.000000 ptetools-0.1.3/src/ptetools/qi.py
--rw-rw-rw-   0        0        0    12177 2024-03-19 20:42:00.000000 ptetools-0.1.3/src/ptetools/tools.py
--rw-rw-rw-   0        0        0       23 2024-03-19 10:32:33.000000 ptetools-0.1.3/src/ptetools/version.py
-drwxrwxrwx   0        0        0        0 2024-03-19 20:47:37.963512 ptetools-0.1.3/src/ptetools.egg-info/
--rw-rw-rw-   0        0        0     1236 2024-03-19 20:47:37.000000 ptetools-0.1.3/src/ptetools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      397 2024-03-19 20:47:37.000000 ptetools-0.1.3/src/ptetools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-19 20:47:37.000000 ptetools-0.1.3/src/ptetools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       71 2024-03-19 20:47:37.000000 ptetools-0.1.3/src/ptetools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-03-19 20:47:37.000000 ptetools-0.1.3/src/ptetools.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-19 20:47:37.960510 ptetools-0.1.3/tests/
--rw-rw-rw-   0        0        0     2002 2024-03-19 10:32:33.000000 ptetools-0.1.3/tests/test_optimization.py
--rw-rw-rw-   0        0        0      406 2024-03-19 10:32:33.000000 ptetools-0.1.3/tests/test_qi.py
--rw-rw-rw-   0        0        0      914 2024-03-19 10:40:19.000000 ptetools-0.1.3/tests/test_tools.py
+drwxrwxrwx   0        0        0        0 2024-05-25 19:34:53.224110 ptetools-0.1.5/
+-rw-rw-rw-   0        0        0     1119 2024-03-19 10:32:33.000000 ptetools-0.1.5/LICENSE.md
+-rw-rw-rw-   0        0        0     1236 2024-05-25 19:34:53.223094 ptetools-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      330 2024-03-19 10:32:33.000000 ptetools-0.1.5/README.md
+-rw-rw-rw-   0        0        0     2227 2024-04-11 08:52:10.000000 ptetools-0.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-25 19:34:53.224110 ptetools-0.1.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-25 19:34:53.080359 ptetools-0.1.5/src/
+drwxrwxrwx   0        0        0        0 2024-05-25 19:34:53.124252 ptetools-0.1.5/src/ptetools/
+-rw-rw-rw-   0        0        0       49 2024-03-19 10:32:33.000000 ptetools-0.1.5/src/ptetools/__init__.py
+-rw-rw-rw-   0        0        0     8797 2024-03-19 10:32:33.000000 ptetools-0.1.5/src/ptetools/optimization.py
+-rw-rw-rw-   0        0        0     2257 2024-03-19 10:32:33.000000 ptetools-0.1.5/src/ptetools/qi.py
+-rw-rw-rw-   0        0        0     1164 2024-05-25 19:33:15.000000 ptetools-0.1.5/src/ptetools/qiskit.py
+-rw-rw-rw-   0        0        0    12792 2024-04-11 08:52:10.000000 ptetools-0.1.5/src/ptetools/tools.py
+-rw-rw-rw-   0        0        0       23 2024-05-25 19:33:32.000000 ptetools-0.1.5/src/ptetools/version.py
+drwxrwxrwx   0        0        0        0 2024-05-25 19:34:53.207452 ptetools-0.1.5/src/ptetools.egg-info/
+-rw-rw-rw-   0        0        0     1236 2024-05-25 19:34:53.000000 ptetools-0.1.5/src/ptetools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      441 2024-05-25 19:34:53.000000 ptetools-0.1.5/src/ptetools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 19:34:53.000000 ptetools-0.1.5/src/ptetools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2024-05-25 19:34:53.000000 ptetools-0.1.5/src/ptetools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-25 19:34:53.000000 ptetools-0.1.5/src/ptetools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-25 19:34:53.207452 ptetools-0.1.5/tests/
+-rw-rw-rw-   0        0        0     2002 2024-03-19 10:32:33.000000 ptetools-0.1.5/tests/test_optimization.py
+-rw-rw-rw-   0        0        0      406 2024-03-19 10:32:33.000000 ptetools-0.1.5/tests/test_qi.py
+-rw-rw-rw-   0        0        0      424 2024-04-11 08:52:10.000000 ptetools-0.1.5/tests/test_qiskit.py
+-rw-rw-rw-   0        0        0     1432 2024-04-11 08:52:10.000000 ptetools-0.1.5/tests/test_tools.py
```

### Comparing `ptetools-0.1.3/LICENSE.md` & `ptetools-0.1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ptetools-0.1.3/PKG-INFO` & `ptetools-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptetools
-Version: 0.1.3
+Version: 0.1.5
 Summary: Python package with various tools. 
 Maintainer-email: Pieter Eendebak <pieter.eendebak@gmail.com>
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
```

### Comparing `ptetools-0.1.3/pyproject.toml` & `ptetools-0.1.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -97,43 +97,44 @@
 00000600: 786d 6c20 7465 7374 7322 0d0a 6f6d 6974  xml tests"..omit
 00000610: 203d 205b 5d0d 0a0d 0a5b 746f 6f6c 2e63   = []....[tool.c
 00000620: 6f76 6572 6167 652e 7265 706f 7274 5d0d  overage.report].
 00000630: 0a73 686f 775f 6d69 7373 696e 6720 3d20  .show_missing = 
 00000640: 7472 7565 0d0a 6661 696c 5f75 6e64 6572  true..fail_under
 00000650: 203d 2038 300d 0a0d 0a5b 746f 6f6c 2e72   = 80....[tool.r
 00000660: 7566 665d 0d0a 7372 6320 3d20 5b22 7372  uff]..src = ["sr
-00000670: 6322 5d0d 0a73 656c 6563 7420 3d20 5b22  c"]..select = ["
-00000680: 4522 2c20 2246 222c 2022 5550 222c 2022  E", "F", "UP", "
-00000690: 4922 5d0d 0a69 676e 6f72 6520 3d20 5b20  I"]..ignore = [ 
-000006a0: 2255 5030 3338 222c 2023 2055 7365 2060  "UP038", # Use `
-000006b0: 5820 7c20 5960 2069 6e20 6069 7369 6e73  X | Y` in `isins
-000006c0: 7461 6e63 6560 2063 616c 6c20 696e 7374  tance` call inst
-000006d0: 6561 6420 6f66 2060 2858 2c20 5929 602c  ead of `(X, Y)`,
-000006e0: 2069 676e 6f72 6520 666f 7220 7065 7266   ignore for perf
-000006f0: 6f72 6d61 6e63 650d 0a20 2020 2020 2020  ormance..       
-00000700: 2020 2020 2245 3731 3222 2023 2068 7474      "E712" # htt
-00000710: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000720: 6173 7472 616c 2d73 682f 7275 6666 2f69  astral-sh/ruff/i
-00000730: 7373 7565 732f 3435 3630 0d0a 2020 2020  ssues/4560..    
-00000740: 2020 2020 5d0d 0a6c 696e 652d 6c65 6e67      ]..line-leng
-00000750: 7468 203d 2031 3230 0d0a 7461 7267 6574  th = 120..target
-00000760: 2d76 6572 7369 6f6e 203d 2022 7079 3331  -version = "py31
-00000770: 3022 0d0a 696e 636c 7564 6520 3d20 5b22  0"..include = ["
-00000780: 2a2e 7079 222c 2022 2a2e 7079 6922 2c20  *.py", "*.pyi", 
-00000790: 222a 2a2f 7079 7072 6f6a 6563 742e 746f  "**/pyproject.to
-000007a0: 6d6c 222c 2022 2a2e 6970 796e 6222 5d0d  ml", "*.ipynb"].
-000007b0: 0a0d 0a70 6572 2d66 696c 652d 6967 6e6f  ...per-file-igno
-000007c0: 7265 7320 3d20 7b20 222a 2e69 7079 6e62  res = { "*.ipynb
-000007d0: 2220 3d20 5b22 4537 3033 222c 2022 4230  " = ["E703", "B0
-000007e0: 3135 222c 2022 4230 3138 225d 207d 2023  15", "B018"] } #
-000007f0: 2073 6565 2068 7474 7073 3a2f 2f67 6974   see https://git
-00000800: 6875 622e 636f 6d2f 6173 7472 616c 2d73  hub.com/astral-s
-00000810: 682f 7275 6666 2f69 7373 7565 732f 3733  h/ruff/issues/73
-00000820: 3030 0d0a 0d0a 0d0a 5b74 6f6f 6c2e 6d79  00......[tool.my
-00000830: 7079 5d0d 0a6d 7970 795f 7061 7468 3d22  py]..mypy_path="
-00000840: 2e2f 7372 6322 0d0a 6967 6e6f 7265 5f6d  ./src"..ignore_m
-00000850: 6973 7369 6e67 5f69 6d70 6f72 7473 203d  issing_imports =
-00000860: 2074 7275 650d 0a65 7863 6c75 6465 203d   true..exclude =
-00000870: 2022 282e 2a2f 756e 7469 746c 6564 2e2a   "(.*/untitled.*
-00000880: 7c2e 2a2f 6465 6275 675f 2e2a 2e70 797c  |.*/debug_.*.py|
-00000890: 2e2a 2f64 6576 656c 6f70 5f2e 2a2e 7079  .*/develop_.*.py
-000008a0: 2922 0d0a                                )"..
+00000670: 6322 5d0d 0a6c 696e 742e 7365 6c65 6374  c"]..lint.select
+00000680: 203d 205b 2245 222c 2022 4622 2c20 2255   = ["E", "F", "U
+00000690: 5022 2c20 2249 225d 0d0a 6c69 6e74 2e69  P", "I"]..lint.i
+000006a0: 676e 6f72 6520 3d20 5b20 2255 5030 3338  gnore = [ "UP038
+000006b0: 222c 2023 2055 7365 2060 5820 7c20 5960  ", # Use `X | Y`
+000006c0: 2069 6e20 6069 7369 6e73 7461 6e63 6560   in `isinstance`
+000006d0: 2063 616c 6c20 696e 7374 6561 6420 6f66   call instead of
+000006e0: 2060 2858 2c20 5929 602c 2069 676e 6f72   `(X, Y)`, ignor
+000006f0: 6520 666f 7220 7065 7266 6f72 6d61 6e63  e for performanc
+00000700: 650d 0a20 2020 2020 2020 2020 2020 2245  e..           "E
+00000710: 3731 3222 2023 2068 7474 7073 3a2f 2f67  712" # https://g
+00000720: 6974 6875 622e 636f 6d2f 6173 7472 616c  ithub.com/astral
+00000730: 2d73 682f 7275 6666 2f69 7373 7565 732f  -sh/ruff/issues/
+00000740: 3435 3630 0d0a 2020 2020 2020 2020 5d0d  4560..        ].
+00000750: 0a6c 696e 652d 6c65 6e67 7468 203d 2031  .line-length = 1
+00000760: 3230 0d0a 7461 7267 6574 2d76 6572 7369  20..target-versi
+00000770: 6f6e 203d 2022 7079 3331 3022 0d0a 696e  on = "py310"..in
+00000780: 636c 7564 6520 3d20 5b22 2a2e 7079 222c  clude = ["*.py",
+00000790: 2022 2a2e 7079 6922 2c20 222a 2a2f 7079   "*.pyi", "**/py
+000007a0: 7072 6f6a 6563 742e 746f 6d6c 222c 2022  project.toml", "
+000007b0: 2a2e 6970 796e 6222 5d0d 0a0d 0a6c 696e  *.ipynb"]....lin
+000007c0: 742e 7065 722d 6669 6c65 2d69 676e 6f72  t.per-file-ignor
+000007d0: 6573 203d 207b 2022 2a2e 6970 796e 6222  es = { "*.ipynb"
+000007e0: 203d 205b 2245 3730 3322 2c20 2242 3031   = ["E703", "B01
+000007f0: 3522 2c20 2242 3031 3822 5d20 7d20 2320  5", "B018"] } # 
+00000800: 7365 6520 6874 7470 733a 2f2f 6769 7468  see https://gith
+00000810: 7562 2e63 6f6d 2f61 7374 7261 6c2d 7368  ub.com/astral-sh
+00000820: 2f72 7566 662f 6973 7375 6573 2f37 3330  /ruff/issues/730
+00000830: 300d 0a0d 0a0d 0a5b 746f 6f6c 2e6d 7970  0......[tool.myp
+00000840: 795d 0d0a 6d79 7079 5f70 6174 683d 222e  y]..mypy_path=".
+00000850: 2f73 7263 220d 0a69 676e 6f72 655f 6d69  /src"..ignore_mi
+00000860: 7373 696e 675f 696d 706f 7274 7320 3d20  ssing_imports = 
+00000870: 7472 7565 0d0a 6578 636c 7564 6520 3d20  true..exclude = 
+00000880: 2228 2e2a 2f75 6e74 6974 6c65 642e 2a7c  "(.*/untitled.*|
+00000890: 2e2a 2f64 6562 7567 5f2e 2a2e 7079 7c2e  .*/debug_.*.py|.
+000008a0: 2a2f 6465 7665 6c6f 705f 2e2a 2e70 7929  */develop_.*.py)
+000008b0: 220d 0a                                  "..
```

### Comparing `ptetools-0.1.3/src/ptetools/optimization.py` & `ptetools-0.1.5/src/ptetools/optimization.py`

 * *Files identical despite different names*

### Comparing `ptetools-0.1.3/src/ptetools/qi.py` & `ptetools-0.1.5/src/ptetools/qi.py`

 * *Files identical despite different names*

### Comparing `ptetools-0.1.3/src/ptetools/tools.py` & `ptetools-0.1.5/src/ptetools/tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,20 +2,32 @@
 import tempfile
 import time
 from collections.abc import Callable, Sequence
 from types import TracebackType
 from typing import Any, Literal
 
 import matplotlib
-import matplotlib.pyplot as plt
 import matplotlib.pylab as pylab
+import matplotlib.pyplot as plt
 import numpy as np
 import qtpy
 from termcolor import colored
 
+
+def make_blocks(size: int, block_size: int) -> list[tuple[int, int]]:
+    """Create blocks of specified size"""
+    number_of_blocks = (size + block_size - 1) // block_size
+    blocks = [(ii * block_size, min(size, (ii + 1) * block_size)) for ii in range(number_of_blocks)]
+    return blocks
+
+
+def sorted_dictionary(d: dict[Any, Any]) -> dict[Any, Any]:
+    return {k: d[k] for k in sorted(d)}
+
+
 def cprint(s: str, color: str = "cyan", *args, **kwargs):
     """Colored print of string"""
     print(colored(s, color=color), *args, **kwargs)
 
 
 def plotLabels(points, labels: None | Sequence[str] = None, **kwargs: Any):
     """Plot labels next to points
@@ -278,15 +290,21 @@
         self.dt = time.perf_counter() - self.start_time
 
         if self.message is not None:
             print(f"{self.message} {self.dt:.3f} [s]")
 
         return False
 
+    def _repr_pretty_(self, p: Any, cycle: bool) -> None:
+        del cycle
+        s = f"<{self.__class__.__name__} at 0x{id(self):x}: dt {self.delta_time:.3f}>\n"
+        p.text(s)
+
 
+# %%
 def profile_expression(expression: str, N: int | None = 1, gui: str = "snakeviz") -> tuple[str, Any]:
     """Profile an expression with cProfile and display the results using snakeviz
 
     Args:
         expression: Code to be profiled
         N: Number of iterations. If None, then automatically determine a suitable number of iterations
         gui: Can be `tuna` or `snakeviz`
@@ -324,40 +342,40 @@
 
     print(f"profiling: {N} iterations, {dt:.2f} [s]")
     r = subprocess.Popen([gui, statsfile])
 
     return statsfile, r
 
 
-def ginput(number_of_points=1, marker : str | None='.', linestyle='', **kwargs) :
-    """ Select points from matplotlib figure
+def ginput(number_of_points=1, marker: str | None = ".", linestyle="", **kwargs):
+    """Select points from matplotlib figure
 
     Press middle mouse button to stop selection
 
     Arguments:
         number_of_points: number of points to select
         marker: Marker style for plotting. If None, do not plot
         kwargs : Arguments passed to plot function
     Returns:
         Numpy array with selected points
     """
-    kwargs = {'linestyle': ''} | kwargs 
-    xx = np.ones(( number_of_points, 2)) * np.nan
+    kwargs = {"linestyle": ""} | kwargs
+    xx = np.ones((number_of_points, 2)) * np.nan
     for ii in range(number_of_points):
         x = pylab.ginput(1)
         if len(x) == 0:
             break
         x = np.asarray(x)
         xx[ii, :] = x.flat
         if marker is not None:
-            plt.plot(xx[:ii+1, 0].T, xx[:ii+1, 1].T, marker=marker, **kwargs)
+            plt.plot(xx[: ii + 1, 0].T, xx[: ii + 1, 1].T, marker=marker, **kwargs)
             plt.draw()
     plt.pause(1e-3)
     return xx
 
-if __name__=='__main__':
-    plt.figure(10); plt.clf()
-    plt.plot([0,1,2,3], [0,3,1,3], '.-')
-    plt.draw()
-    x=ginput(7)
-    
 
+if __name__ == "__main__":
+    plt.figure(10)
+    plt.clf()
+    plt.plot([0, 1, 2, 3], [0, 3, 1, 3], ".-")
+    plt.draw()
+    x = ginput(7)
```

### Comparing `ptetools-0.1.3/src/ptetools.egg-info/PKG-INFO` & `ptetools-0.1.5/src/ptetools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptetools
-Version: 0.1.3
+Version: 0.1.5
 Summary: Python package with various tools. 
 Maintainer-email: Pieter Eendebak <pieter.eendebak@gmail.com>
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
```

### Comparing `ptetools-0.1.3/tests/test_optimization.py` & `ptetools-0.1.5/tests/test_optimization.py`

 * *Files identical despite different names*

