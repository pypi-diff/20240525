# Comparing `tmp/pytom3d-0.0.0rc4.tar.gz` & `tmp/pytom3d-0.0.0rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytom3d-0.0.0rc4.tar", last modified: Sat May  4 10:11:18 2024, max compression
+gzip compressed data, was "pytom3d-0.0.0rc5.tar", last modified: Sat May 25 15:17:23 2024, max compression
```

## Comparing `pytom3d-0.0.0rc4.tar` & `pytom3d-0.0.0rc5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2024-05-04 10:11:18.130973 pytom3d-0.0.0rc4/
--rw-rw-r--   0 ale       (1000) ale       (1000)    32473 2024-05-04 08:43:07.000000 pytom3d-0.0.0rc4/LICENSE
--rw-r--r--   0 ale       (1000) ale       (1000)     1566 2024-05-04 10:11:18.130973 pytom3d-0.0.0rc4/PKG-INFO
--rw-rw-r--   0 ale       (1000) ale       (1000)      613 2024-05-04 08:43:07.000000 pytom3d-0.0.0rc4/README.md
--rw-rw-r--   0 ale       (1000) ale       (1000)       86 2024-05-04 08:43:07.000000 pytom3d-0.0.0rc4/pyproject.toml
--rw-rw-r--   0 ale       (1000) ale       (1000)       38 2024-05-04 10:11:18.130973 pytom3d-0.0.0rc4/setup.cfg
--rw-rw-r--   0 ale       (1000) ale       (1000)     1123 2024-05-04 10:10:43.000000 pytom3d-0.0.0rc4/setup.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2024-05-04 10:11:18.130973 pytom3d-0.0.0rc4/src/
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2024-05-04 10:11:18.130973 pytom3d-0.0.0rc4/src/pytom3d/
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2024-05-04 08:43:07.000000 pytom3d-0.0.0rc4/src/pytom3d/__init__.py
--rw-rw-r--   0 ale       (1000) ale       (1000)    20583 2024-05-04 08:58:19.000000 pytom3d-0.0.0rc4/src/pytom3d/core.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     3259 2024-05-04 09:30:21.000000 pytom3d-0.0.0rc4/src/pytom3d/scan.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     2214 2024-05-04 08:43:07.000000 pytom3d-0.0.0rc4/src/pytom3d/stats.py
--rw-rw-r--   0 ale       (1000) ale       (1000)    13968 2024-05-04 08:46:58.000000 pytom3d-0.0.0rc4/src/pytom3d/util.py
--rw-rw-r--   0 ale       (1000) ale       (1000)    20103 2024-05-04 09:42:43.000000 pytom3d-0.0.0rc4/src/pytom3d/viewer.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2024-05-04 10:11:18.130973 pytom3d-0.0.0rc4/src/pytom3d.egg-info/
--rw-r--r--   0 ale       (1000) ale       (1000)     1566 2024-05-04 10:11:18.000000 pytom3d-0.0.0rc4/src/pytom3d.egg-info/PKG-INFO
--rw-rw-r--   0 ale       (1000) ale       (1000)      342 2024-05-04 10:11:18.000000 pytom3d-0.0.0rc4/src/pytom3d.egg-info/SOURCES.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)        1 2024-05-04 10:11:18.000000 pytom3d-0.0.0rc4/src/pytom3d.egg-info/dependency_links.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)      112 2024-05-04 10:11:18.000000 pytom3d-0.0.0rc4/src/pytom3d.egg-info/requires.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)        8 2024-05-04 10:11:18.000000 pytom3d-0.0.0rc4/src/pytom3d.egg-info/top_level.txt
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2024-05-25 15:17:23.796239 pytom3d-0.0.0rc5/
+-rw-rw-r--   0 ale       (1000) ale       (1000)    32473 2024-05-24 07:24:27.000000 pytom3d-0.0.0rc5/LICENSE
+-rw-r--r--   0 ale       (1000) ale       (1000)     1566 2024-05-25 15:17:23.796239 pytom3d-0.0.0rc5/PKG-INFO
+-rw-rw-r--   0 ale       (1000) ale       (1000)      613 2024-05-24 07:24:27.000000 pytom3d-0.0.0rc5/README.md
+-rw-rw-r--   0 ale       (1000) ale       (1000)       86 2024-05-24 07:24:27.000000 pytom3d-0.0.0rc5/pyproject.toml
+-rw-rw-r--   0 ale       (1000) ale       (1000)       38 2024-05-25 15:17:23.796239 pytom3d-0.0.0rc5/setup.cfg
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1123 2024-05-25 15:16:58.000000 pytom3d-0.0.0rc5/setup.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2024-05-25 15:17:23.792239 pytom3d-0.0.0rc5/src/
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2024-05-25 15:17:23.792239 pytom3d-0.0.0rc5/src/pytom3d/
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2024-05-24 07:24:27.000000 pytom3d-0.0.0rc5/src/pytom3d/__init__.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)    20583 2024-05-24 07:24:27.000000 pytom3d-0.0.0rc5/src/pytom3d/core.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     3535 2024-05-25 15:04:47.000000 pytom3d-0.0.0rc5/src/pytom3d/scan.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2214 2024-05-24 07:24:27.000000 pytom3d-0.0.0rc5/src/pytom3d/stats.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)    15042 2024-05-24 08:25:48.000000 pytom3d-0.0.0rc5/src/pytom3d/util.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)    28326 2024-05-25 15:15:31.000000 pytom3d-0.0.0rc5/src/pytom3d/viewer.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2024-05-25 15:17:23.792239 pytom3d-0.0.0rc5/src/pytom3d.egg-info/
+-rw-r--r--   0 ale       (1000) ale       (1000)     1566 2024-05-25 15:17:23.000000 pytom3d-0.0.0rc5/src/pytom3d.egg-info/PKG-INFO
+-rw-rw-r--   0 ale       (1000) ale       (1000)      342 2024-05-25 15:17:23.000000 pytom3d-0.0.0rc5/src/pytom3d.egg-info/SOURCES.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        1 2024-05-25 15:17:23.000000 pytom3d-0.0.0rc5/src/pytom3d.egg-info/dependency_links.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)      112 2024-05-25 15:17:23.000000 pytom3d-0.0.0rc5/src/pytom3d.egg-info/requires.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        8 2024-05-25 15:17:23.000000 pytom3d-0.0.0rc5/src/pytom3d.egg-info/top_level.txt
```

### Comparing `pytom3d-0.0.0rc4/LICENSE` & `pytom3d-0.0.0rc5/LICENSE`

 * *Files identical despite different names*

### Comparing `pytom3d-0.0.0rc4/PKG-INFO` & `pytom3d-0.0.0rc5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytom3d
-Version: 0.0.0rc4
+Version: 0.0.0rc5
 Summary: PyToM-3D: Python Topography Manipulator in 3D
 Home-page: https://github.com/aletgn/pytom-3d.git
 Author: Alessandro Tognan
 Author-email: alessandro.tognan@gmail.com
 Project-URL: Bug Tracker, https://github.com/aletgn/pytom-3d/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `pytom3d-0.0.0rc4/README.md` & `pytom3d-0.0.0rc5/README.md`

 * *Files identical despite different names*

### Comparing `pytom3d-0.0.0rc4/setup.py` & `pytom3d-0.0.0rc5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="pytom3d",
-    version="0.0.0rc4",
+    version="0.0.0rc5",
     description="PyToM-3D: Python Topography Manipulator in 3D",
     long_description=long_description,
     long_description_content_type="text/markdown",
         
     author="Alessandro Tognan",
     author_email="alessandro.tognan@gmail.com",
     url="https://github.com/aletgn/pytom-3d.git",
```

### Comparing `pytom3d-0.0.0rc4/src/pytom3d/core.py` & `pytom3d-0.0.0rc5/src/pytom3d/core.py`

 * *Files identical despite different names*

### Comparing `pytom3d-0.0.0rc4/src/pytom3d/scan.py` & `pytom3d-0.0.0rc5/src/pytom3d/scan.py`

 * *Files 5% similar despite different names*

```diff
@@ -94,33 +94,39 @@
     None
     """
     for s in scans:
         data = reader(s, **kwargs)
         data.to_excel(path, index=False)
 
 
-def scan_stat_factory(*scan: List):
+def scan_stat_factory(name: str = "av", color: str = "k", linestyle: str = "-", *scan: List):
     """
     Create a scan object representing the statistical summary of multiple scans.
 
     Parameters
     ----------
-    *scan : variable number of Scan objects
-        Scan objects to be summarized.
+    name: str
+        Name to be assigned to the output scan
+    color: str
+        Color to be assigned to the output scan
+    linestyle:
+        Linestyle to be assigned to the output scan
+    scan : variable number of Scan objects
+        Scan objects to be processed.
 
     Returns
     -------
     av_scan : Scan object
         Scan object representing the statistical summary of the input scans.
 
     """
     x = scan[0].x
     values = np.array([s.y for s in scan])
     squared_uncertainty = np.array([np.square(s.y_err) for s in scan])
 
     mean = values.mean(axis=0)
     quad = np.sqrt(squared_uncertainty.sum(axis=0))/len(scan)
 
-    av_scan = Scan(name="av")
+    av_scan = Scan(name=name, line=linestyle, color=color)
     av_scan.load_data(x, mean, quad)
 
     return av_scan
```

### Comparing `pytom3d-0.0.0rc4/src/pytom3d/stats.py` & `pytom3d-0.0.0rc5/src/pytom3d/stats.py`

 * *Files identical despite different names*

### Comparing `pytom3d-0.0.0rc4/src/pytom3d/util.py` & `pytom3d-0.0.0rc5/src/pytom3d/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import functools
 import glob
 import pickle
 import numpy as np
 import pandas as pd
 import re
 from typing import Tuple, List, Any
+from matplotlib import pyplot as plt
 
 from pytom3d.stats import running_mean, running_std
 
 
 def export_regressor(regressor, folder: str = "./", filename: str = "my_regressor", extension: str = ".rg",
                      excluded_keys: List[str] = [], forced_values: List[Any] = []) -> None:
     """
@@ -499,7 +500,41 @@
     data = recursive_search(path, match=match, pop_first=True, take_first=False)
 
     mean = running_mean(3, None, *data)
     std = running_std(3, None, 1, *data)
     x = get_coordinates([0], *data)
 
     return x.reshape(-1), mean, std
+
+
+def printer(func: callable):
+    """
+    A decorator for class methods that saves a figure if 'save' is True.
+
+    Borrowed from https://github.com/aletgn/b-fade/blob/master/src/bfade/util.py
+
+    This decorator wraps a method that generates a figure and a title,
+    and it saves the figure to the specified location if 'save' is True.
+
+    Parameters
+    ----------
+    func : callable
+        The function to be decorated, which generates a figure and a title.
+
+    Returns
+    -------
+    callable
+        The decorated function.
+    """
+    @functools.wraps(func) # <- preserve function signature
+    def saver(self, *args, **kwargs):
+        fig, title = func(self, *args, **kwargs)
+        if self.save == True:
+            fig.savefig(self.folder + title + "." + self.fmt,
+                        format = self.fmt,
+                        dpi = self.dpi,
+                        bbox_inches='tight')
+            print(f"SAVE: {title}")
+        else:
+            print(f"SHOW: {title}")
+            plt.show()
+    return saver
```

### Comparing `pytom3d-0.0.0rc4/src/pytom3d/viewer.py` & `pytom3d-0.0.0rc5/src/pytom3d/viewer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from pytom3d.core import Topography
+from pytom3d.util import printer
 # from util import summation, distance, distance2
 from matplotlib import pyplot as plt
 from typing import List, Tuple
 import matplotlib
 from matplotlib import ticker
 import matplotlib.cm as cm
 from matplotlib.gridspec import GridSpec
@@ -37,15 +38,96 @@
             None
 
         """
         self.name = name
         self.x_lim = None
         self.y_lim = None
         self.z_lim = None
-        
+        self.config()
+        self.config_3d()
+
+    def config(self, save: bool = False, folder: str = "./", fmt: str = "png", dpi: int = 300) -> None:
+        """
+        Configure settings for saving plots.
+
+        Borrowed from https://github.com/aletgn/b-fade/
+
+        Parameters
+        ----------
+        save : bool, optional
+            Flag indicating whether to save plots. The default is False.
+        folder : str, optional
+            Folder path where plots will be saved. The default is "./".
+        fmt : str, optional
+            Format for saving plots. The default is "png".
+        dpi : int, optional
+            Dots per inch for saving plots. The default is 300.
+
+        Returns
+        -------
+        None
+
+        """
+        self.save = save
+        self.folder = folder
+        self.fmt = fmt
+        self.dpi = dpi
+
+    def config_3d(self, point_size: float = 0.3, cmap: str = "RdYlBu_r",
+                  xlabel: str = r'$x_g$ [mm]',
+                  ylabel: str = r'$y_g$ [mm]',
+                  zlabel: str = r'$u(x_g, y_g)$ [mm]',
+                  x_lim: List = [-110, 110],
+                  y_lim: List = [-38, 38],
+                  z_lim: List = None,
+                  zticks: int = 10,
+                  zoom: float = 1) -> None:
+        """
+        Configure the 3D plot parameters.
+
+        Parameters
+        ----------
+        point_size : float, optional
+            Size of the points in the plot (default is 0.3).
+        cmap : str, optional
+            Colormap for the plot (default is "RdYlBu_r").
+        xlabel : str, optional
+            Label for the x-axis (default is r'$x_g$ [mm]').
+        ylabel : str, optional
+            Label for the y-axis (default is r'$y_g$ [mm]').
+        zlabel : str, optional
+            Label for the z-axis (default is r'$u(x_g, y_g)$ [mm]').
+        x_lim : list of int, optional
+            Limits for the x-axis (default is [-110, 110]).
+        y_lim : list of int, optional
+            Limits for the y-axis (default is [-38, 38]).
+        z_lim : list of int or None, optional
+            Limits for the z-axis (default is None).
+        zticks : int, optional
+            Number of ticks on the z-axis (default is 10).
+        zoom : float, optional
+            Zoom level for the plot (default is 1).
+
+        Returns
+        -------
+        None
+
+        """
+        self.point_size = point_size
+        self.cmap = cmap
+        self.xlabel = xlabel
+        self.ylabel = ylabel
+        self.zlabel = zlabel
+        self.x_lim = x_lim
+        self.y_lim = y_lim
+        self.z_lim = z_lim
+        self.zticks = zticks
+        self.zoom = zoom
+
+
     def set_limits(self, x: List[float] = None, y: List[float] = None, z: List[float] = None) -> None:
         """
         Set the limits for the x, y, and z axes.
     
         Parameters
         ----------
         x : List[float], optional
@@ -99,14 +181,15 @@
             plt.scatter(d.P[:, 1], d.P[:, 2], s=1, alpha=1)
             plt.title('yz plane')
             plt.xlabel('y')
             plt.ylabel('z')
         plt.gcf().tight_layout(pad=1)
         plt.show()
 
+    @printer
     def scatter3D(self, *data: List[Topography]) -> None:
         """
         Generate a 3D scatter plot for the given Topography data.
 
         Parameters
         ----------
         data : List[Topography]
@@ -135,44 +218,48 @@
             vmin = self.z_lim[0]
             vmax = self.z_lim[1]
         else:
             vmin = np.array([h.m[2] for h in data]).min()
             vmax = np.array([h.M[2] for h in data]).max()
             ax.set_zlim([vmin, vmax])
 
-        ax.set_xlabel("x [mm]")
-        ax.set_ylabel("y [mm]")
-        ax.set_zlabel("z [mm]")
+        ax.set_xlabel(self.xlabel)
+        ax.set_ylabel(self.ylabel)
+        ax.set_zlabel(self.zlabel)
 
         ax.xaxis.pane.set_color('w')
         ax.yaxis.pane.set_edgecolor('w')
         ax.zaxis.pane.set_edgecolor('w')
         ax.xaxis.pane.set_color('w')
         ax.yaxis.pane.set_color('w')
         ax.zaxis.pane.set_color('w')
 
         plt.gca().xaxis.set_major_formatter(ticker.StrMethodFormatter("{x:.0f}"))
-        plt.gca().yaxis.set_major_formatter(ticker.StrMethodFormatter("{x:.1f}"))
+        plt.gca().yaxis.set_major_formatter(ticker.StrMethodFormatter("{x:.0f}"))
         plt.gca().zaxis.set_major_formatter(ticker.StrMethodFormatter("{x:.2f}"))
     
-        ax.grid(True)
+        ax.xaxis._axinfo['grid'].update(color = 'grey', linestyle = ':', linewidth = 0.5)
+        ax.yaxis._axinfo['grid'].update(color = 'grey', linestyle = ':', linewidth = 0.5)
+        ax.zaxis._axinfo['grid'].update(color = 'grey', linestyle = ':', linewidth = 0.5)
 
         for d in data:
-            sc = ax.scatter3D(d.P[:, 0], d.P[:, 1], d.P[:, 2], s=0.5, alpha=1,
-                              vmin=vmin, vmax=vmax, c=d.P[:, 2])
-
-        cbar = fig.colorbar(sc, ax=ax, orientation="vertical",
-                            pad=0.12, format="%.2f",
-                            ticks=list(np.linspace(vmin,
-                                                   vmax, 11)),
-                            label='Altitude')
-        cbar.ax.tick_params(direction='in', right=1, left=1, size=2.5)
-
-        ax.axis('tight')
-        plt.show()
+            sc = ax.scatter(d.P[:, 0], d.P[:, 1], d.P[:, 2], s=self.point_size, alpha=1,
+                              vmin=vmin, vmax=vmax, c=d.P[:, 2],  marker="o",
+                              cmap=self.cmap)
+
+        # cbar = fig.colorbar(sc, ax=ax, orientation="vertical",
+        #                     pad=0.12, format="%.2f",
+        #                     ticks=list(np.linspace(vmin,
+        #                                            vmax, 11)),
+        #                     label=self.zlabel)
+        # cbar.ax.tick_params(direction='in', right=1, left=1, size=2.5)
+
+        # ax.axis('tight')
+        ax.set_box_aspect(None, zoom=self.zoom)
+        return fig, self.name
 
     def scatter3DRegression(self, regression: Topography, reference: Topography = None) -> None:
         fig = plt.figure(dpi=300)
         ax = fig.add_subplot(1, 1, 1, projection='3d')
 
         ax.set_xlabel("x [mm]")
         ax.set_ylabel("y [mm]")
@@ -223,29 +310,64 @@
     def __init__(self, **kwargs) -> None:
 
         try:
             self.name = kwargs.pop("name")
         except KeyError:
             self.name = "Untitled"
 
+        self.config()
+        self.config_scan_view()
         self.config_canvas()
 
+    def config(self, save: bool = False, folder: str = "./", fmt: str = "png", dpi: int = 300) -> None:
+        """
+        Configure settings for saving plots.
+
+        Borrowed from https://github.com/aletgn/b-fade/
+
+        Parameters
+        ----------
+        save : bool, optional
+            Flag indicating whether to save plots. The default is False.
+        folder : str, optional
+            Folder path where plots will be saved. The default is "./".
+        fmt : str, optional
+            Format for saving plots. The default is "png".
+        dpi : int, optional
+            Dots per inch for saving plots. The default is 300.
+
+        Returns
+        -------
+        None
 
-    def config_canvas(self, dpi: int = 300, cmap: str = "RdYlBu_r", levels: int = 8,
+        """
+        self.save = save
+        self.folder = folder
+        self.fmt = fmt
+        self.dpi = dpi
+
+    def config_scan_view(self, xlabel=r'$x$ [mm]', ylabel=r'$y$ [mm]', x_lim=[-20, 20], 
+                         y_lim=[-70, 70], legend_config = None):
+
+        self.xlabel = xlabel
+        self.ylabel = ylabel
+        self.x_lim = x_lim
+        self.y_lim = y_lim
+        self.legend_config = legend_config
+
+    def config_canvas(self, cmap: str = "RdYlBu_r", levels: int = 8,
                       x_lim: List[float] = [-100, 100], y_lim_top: List[float] = [10,20],
                       y_lim_bot: List[float] = [-10,-20], y_lim_scan: str = [-140, 140],
                       cbar_lim: List[float] = [-140, 140], loc: str = "best",
                       bbox_to_anchor: List[float] = None) -> None:
         """
         Configure canvas for plotting.
 
         Parameters
         ----------
-        dpi : int, optional
-            Dots per inch for the plot resolution. Default is 300.
         cmap : str, optional
             Colormap to use for plotting. Default is "RdYlBu_r".
         levels : int, optional
             Number of levels for the colorbar. Default is 8.
         x_lim : List[float], optional
             Limits for the x-axis. Default is [-100, 100].
         y_lim_top : List[float], optional
@@ -262,16 +384,14 @@
             Anchor point for the legend bounding box. Default is None.
 
         Returns
         -------
         None
             This function does not return anything. It only sets instance attributes.
         """
-        self.dpi = dpi
-
         self.cmap = cmap
         self.levels = levels
 
         self.x_lim = x_lim
         self.y_lim_top = y_lim_top
         self.y_lim_bot = y_lim_bot
         self.y_lim_scan = y_lim_scan
@@ -354,44 +474,145 @@
             else:
                 if s.y_err is not None:
                     ax.fill_between(s.x, s.y-s.y_err, s.y+s.y_err, alpha=0.5, edgecolor="none")
                 ax.plot(s.x, s.y)
 
         plt.show()
 
+    @printer
     def scan_view_and_bar(self, swap: bool = False, *scan: List) -> None:
         """
         Plot scan data with error bars.
 
         Parameters
         ----------
         swap : bool, optional
             If True, swap x and y axes in the plot. Default is False.
-        *scan : List
+        scan : List
             List of scan data to plot. Each scan data should be provided as a list-like object.
 
         Returns
         -------
         None
 
         """
         fig, ax = plt.subplots(dpi=300)
         for s in scan:
             if swap:
                 if s.y_err is not None:
-                    ax.errorbar(s.y, s.x, xerr=s.y_err, yerr=None, fmt="-o",
+                    ax.errorbar(s.y, s.x, xerr=s.y_err, yerr=None, fmt="o",
                                 markersize=3, capsize=3, capthick=1, linewidth=0.8)
                 pass
 
             else:
                 if s.y_err is not None:
-                    ax.errorbar(s.x, s.y, xerr=None, yerr=s.y_err, fmt="-o",
-                                markersize=3, capsize=3, capthick=1, linewidth=0.8)
+                    ax.errorbar(s.x, s.y, xerr=None, yerr=s.y_err, fmt="o", c=s.color,
+                                linestyle=s.line, markersize=3, capsize=3, capthick=1, linewidth=0.8, label=s.name)
 
-        plt.show()
+        ax.set_xlabel(self.xlabel)
+        ax.set_ylabel(self.ylabel)
+        ax.set_xlim(self.x_lim)
+        ax.set_ylim(self.y_lim)
+        try:
+            ax.legend(**self.legend_config)
+        except:
+            pass
+
+        return fig, self.name
+
+    @printer
+    def scan_compare(self, fills: List, bars: List) -> Tuple:
+        """
+        Compare scans by plotting filled regions and error bars.
+
+        Parameters
+        ----------
+        fills : list of scans
+            List of data for the filled regions.
+        bars : list of scans
+            List of data for the error bars.
+
+        Returns
+        -------
+        fig : Figure
+            The matplotlib figure object.
+        name : str
+            The name associated with the plot.
+
+        """
+        fig, ax = plt.subplots(dpi=300)
+        for f in fills:
+            ax.fill_between(f.x, f.y-f.y_err, f.y+f.y_err, color=f.color, alpha=f.alpha, edgecolor="none")
+            ax.plot(f.x, f.y, color=f.color, label=f.name)
+        for b in bars:
+            ax.errorbar(b.x, b.y, xerr=None, yerr=b.y_err, fmt="o", c=b.color,
+                                    linestyle=b.line, markersize=3, capsize=3,
+                                    capthick=1, linewidth=0.8, label=b.name)
+
+        ax.legend(**self.legend_config)
+        ax.set_xlim(self.x_lim)
+        ax.set_ylim(self.y_lim)
+        ax.set_xlabel(self.xlabel)
+        ax.set_ylabel(self.ylabel)
+
+        return fig, self.name
+
+    @printer
+    def contour(self, top_cnt, bot_cnt) -> Tuple:
+        """
+        Create contour plots for the provided data.
+
+        Parameters
+        ----------
+        top_cnt : Topography object
+            Data for the top contour plot.
+        bot_cnt : Topography object
+            Data for the bottom contour plot.
+
+        Returns
+        -------
+        fig : Figure
+            The matplotlib figure object.
+        name : str
+            The name associated with the plot.
+
+        """
+        fig = plt.figure(dpi=self.dpi, figsize=(4,4))
+        gs = GridSpec(4, 2, figure=fig,
+                        width_ratios=[0.975, 0.025],
+                        height_ratios=[0.25, 0.25, 0.25, 0.25])
+        ax1 = fig.add_subplot(gs[0, 0])
+        ax2 = fig.add_subplot(gs[1, 0])
+        ax3 = fig.add_subplot(gs[0:2, 1])
+        ax4 = fig.add_subplot(gs[2, 0])
+        ax5 = fig.add_subplot(gs[3, 0])
+        ax6 = fig.add_subplot(gs[2:4, 1])
+
+        im12, norm12 = discrete_colorbar(self.cmap, self.mean_lim[0], self.mean_lim[1], self.levels)
+        a1 = ax1.tricontourf(top_cnt.P[:,0], top_cnt.P[:,1], top_cnt.P[:,2], levels=self.levels, cmap=self.cmap, norm=norm12)
+        a2 = ax2.tricontourf(bot_cnt.P[:,0], bot_cnt.P[:,1], bot_cnt.P[:,2], levels=self.levels, cmap=self.cmap, norm=norm12)
+        cb1 = fig.colorbar(im12, ax=[a1,a2], cax=ax3, orientation='vertical', label="Expected Value", format="%.0f", pad=0.1, fraction=0.5,
+                        ticks=(np.linspace(self.mean_lim[0], self.mean_lim[1], self.levels)))
+
+        im45, norm45 = discrete_colorbar(self.cmap, self.std_lim[0], self.std_lim[1], self.levels)
+        a4 = ax4.tricontourf(top_cnt.P[:,0], top_cnt.P[:,1], top_cnt.unc, levels=self.levels, cmap=self.cmap, norm=norm45)
+        a5 = ax5.tricontourf(bot_cnt.P[:,0], bot_cnt.P[:,1], bot_cnt.unc, levels=self.levels, cmap=self.cmap, norm=norm45)
+        cb2 = fig.colorbar(im45, cax=ax6, orientation='vertical', label="Uncertainty", format="%.0f", pad=0.1,
+                        ticks=list(np.linspace(self.std_lim[0], self.std_lim[1], self.levels)))
+
+        for a in [ax1, ax2, ax4, ax5]:
+            a.tick_params(direction="in", top=1, right=1, color="k") # pad=5
+            a.set_xlabel(r"$x$ [mm]")
+            a.set_ylabel(r"$y$ [mm]")
+
+        for c in [cb1, cb2]:
+            c.ax.tick_params(direction='in', right=1, left=1, size=1.5, labelsize=8)
+
+        plt.tight_layout()
+        return fig, self.name
 
     def contour_and_scan_2(self, top_cnt, bot_cnt, top_scan = None, bot_scan = None,
                            top_err = None, bot_err = None) -> None:
         """
         Plot contour and scan data.
 
         Parameters
@@ -495,14 +716,16 @@
         # plt.savefig("/home/ale/Desktop/exp/test.png", dpi=300, format="png")
 
 
 def cfg_matplotlib(font_size: int = 12, font_family: str = 'sans-serif', use_latex: bool = False, interactive: bool = False) -> None:
     """
     Set Matplotlib RC parameters for font size, font family, and LaTeX usage.
 
+    Borrowed from https://github.com/aletgn/b-fade/blob/master/src/bfade/util.py
+
     Parameters
     ----------
     font_size : int, optional
         Font size. The default is 12.
 
     font_family : str, optional
         Font family. The default is 'sans-serif'.
@@ -517,14 +740,15 @@
     -------
     None
 
     """
     matplotlib.rcParams['font.size'] = font_size
     matplotlib.rcParams['font.family'] = font_family
     matplotlib.rcParams['text.usetex'] = use_latex
+    matplotlib.rcParams["interactive"] = interactive
 
 
 def cbar_bounds(v: np.ndarray, w: np.ndarray) -> Tuple[float]:
     """
     Calculate the lower and upper bounds for color bar.
 
     Parameters
```

### Comparing `pytom3d-0.0.0rc4/src/pytom3d.egg-info/PKG-INFO` & `pytom3d-0.0.0rc5/src/pytom3d.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytom3d
-Version: 0.0.0rc4
+Version: 0.0.0rc5
 Summary: PyToM-3D: Python Topography Manipulator in 3D
 Home-page: https://github.com/aletgn/pytom-3d.git
 Author: Alessandro Tognan
 Author-email: alessandro.tognan@gmail.com
 Project-URL: Bug Tracker, https://github.com/aletgn/pytom-3d/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

