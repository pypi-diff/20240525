# Comparing `tmp/tiltlib-0.0.5.tar.gz` & `tmp/tiltlib-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiltlib-0.0.5.tar", last modified: Tue Mar 12 21:30:10 2024, max compression
+gzip compressed data, was "tiltlib-0.1.tar", last modified: Sat May 25 08:49:05 2024, max compression
```

## Comparing `tiltlib-0.0.5.tar` & `tiltlib-0.1.tar`

### file list

```diff
@@ -1,23 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 21:30:10.351959 tiltlib-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-03-12 21:30:10.351959 tiltlib-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-03-12 21:29:59.000000 tiltlib-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-03-12 21:29:59.000000 tiltlib-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 21:30:10.351959 tiltlib-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 21:30:10.347959 tiltlib-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 21:30:10.347959 tiltlib-0.0.5/src/tiltlib/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-12 21:29:59.000000 tiltlib-0.0.5/src/tiltlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-12 21:29:59.000000 tiltlib-0.0.5/src/tiltlib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-03-12 21:29:59.000000 tiltlib-0.0.5/src/tiltlib/axis.py
--rw-r--r--   0 runner    (1001) docker     (127)     9840 2024-03-12 21:29:59.000000 tiltlib-0.0.5/src/tiltlib/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-03-12 21:29:59.000000 tiltlib-0.0.5/src/tiltlib/sample_holder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 21:30:10.351959 tiltlib-0.0.5/src/tiltlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-03-12 21:30:10.000000 tiltlib-0.0.5/src/tiltlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-03-12 21:30:10.000000 tiltlib-0.0.5/src/tiltlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 21:30:10.000000 tiltlib-0.0.5/src/tiltlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-12 21:30:10.000000 tiltlib-0.0.5/src/tiltlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-12 21:30:10.000000 tiltlib-0.0.5/src/tiltlib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 21:30:10.351959 tiltlib-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-03-12 21:29:59.000000 tiltlib-0.0.5/tests/test_axis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-03-12 21:29:59.000000 tiltlib-0.0.5/tests/test_rotation_generators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-03-12 21:29:59.000000 tiltlib-0.0.5/tests/test_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-03-12 21:29:59.000000 tiltlib-0.0.5/tests/test_sampleholder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 08:49:05.136474 tiltlib-0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-25 08:49:05.136474 tiltlib-0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-25 08:48:57.000000 tiltlib-0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-25 08:48:57.000000 tiltlib-0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 08:49:05.136474 tiltlib-0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 08:49:05.132474 tiltlib-0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 08:49:05.136474 tiltlib-0.1/src/tiltlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-25 08:48:57.000000 tiltlib-0.1/src/tiltlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-25 08:48:57.000000 tiltlib-0.1/src/tiltlib/axis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17167 2024-05-25 08:48:57.000000 tiltlib-0.1/src/tiltlib/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-05-25 08:48:57.000000 tiltlib-0.1/src/tiltlib/sample_holder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 08:49:05.136474 tiltlib-0.1/src/tiltlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-25 08:49:05.000000 tiltlib-0.1/src/tiltlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-25 08:49:05.000000 tiltlib-0.1/src/tiltlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 08:49:05.000000 tiltlib-0.1/src/tiltlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-25 08:49:05.000000 tiltlib-0.1/src/tiltlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-25 08:49:05.000000 tiltlib-0.1/src/tiltlib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 08:49:05.136474 tiltlib-0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-25 08:48:57.000000 tiltlib-0.1/tests/test_axis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-25 08:48:57.000000 tiltlib-0.1/tests/test_rotation_generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-05-25 08:48:57.000000 tiltlib-0.1/tests/test_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-05-25 08:48:57.000000 tiltlib-0.1/tests/test_sampleholder.py
```

### Comparing `tiltlib-0.0.5/PKG-INFO` & `tiltlib-0.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiltlib
-Version: 0.0.5
+Version: 0.1
 Summary: TEM tilt holder scripts
 Author-email: Viljar Femoen <viljarjf@stud.ntnu.no>
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -15,14 +15,20 @@
 Requires-Dist: matplotlib
 Requires-Dist: hyperspy
 Requires-Dist: scipy
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-xdist; extra == "test"
 Requires-Dist: filelock; extra == "test"
+Provides-Extra: docs
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: sphinx-rtd-theme; extra == "docs"
+Requires-Dist: nbsphinx; extra == "docs"
+Requires-Dist: IPython; extra == "docs"
+Requires-Dist: ipykernel; extra == "docs"
 
 # tiltlib
 
 Tilt TEM sample holders
 
 # Installation
```

### Comparing `tiltlib-0.0.5/pyproject.toml` & `tiltlib-0.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tiltlib"
-version = "0.0.5"
+version = "0.1"
 authors = [
   { name="Viljar Femoen", email="viljarjf@stud.ntnu.no" },
 ]
 description = "TEM tilt holder scripts"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -21,7 +21,8 @@
     "matplotlib",
     "hyperspy",
     "scipy",
 ]
 
 [project.optional-dependencies]
 test = ["pytest", "pytest-xdist", "filelock"]
+docs = ["sphinx", "sphinx-rtd-theme", "nbsphinx", "IPython", "ipykernel",]
```

### Comparing `tiltlib-0.0.5/src/tiltlib/axis.py` & `tiltlib-0.1/src/tiltlib/axis.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,14 +21,19 @@
             self.max = deg2rad(self.max)
             self.angle = deg2rad(self.angle)
             self.degrees = False
         self._initial_angle = self.angle
 
     @property
     def R(self) -> Rotation:
+        """The rotation of the axis as a quaternion
+
+        :return: rotation
+        :rtype: Rotation
+        """
         return Rotation.from_axes_angles(
             self.direction, self.angle - self._initial_angle
         )
 
     def __repr__(self) -> str:
         return f"""{self.__class__.__name__}:
         direction = [{self.direction.x[0]}, {self.direction.y[0]}, {self.direction.z[0]}]
```

### Comparing `tiltlib-0.0.5/src/tiltlib/sample_holder.py` & `tiltlib-0.1/src/tiltlib/sample_holder.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 from orix.vector import Vector3d
 
 from tiltlib.axis import Axis
 
 
 class SampleHolder:
     def __init__(self, axes: list[Axis] = None) -> None:
-        """The first axis is always extrinsic.
+        """Handles the rotation of a sample holder in a TEM.
+        The first axis is always extrinsic.
 
-        Args:
-            axes (list[Axis], optional): axes, in order
+        :param axes: Tilt axes, in order, defaults to None
+        :type axes: list[Axis], optional
+        :raises ValueError: If :code:axes contains a non-:code:Axis instance
         """
         if axes is None:
             axes = []
         if isinstance(axes, Axis):
             axes = [axes]
 
         if not all(isinstance(axis, Axis) for axis in axes):
@@ -25,28 +27,31 @@
         self.axes[0].extrinsic = True
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}:\n" + "\n".join(str(ax) for ax in self.axes)
 
     @property
     def angles(self) -> list[float]:
+        """Current tilt angles, in radians
+        """
         return list(axis.angle for axis in self.axes)
 
     @property
     def _initial_angles(self) -> list[float]:
         return list(axis._initial_angle for axis in self.axes)
 
     @angles.setter
     def angles(self, angles: list[float]):
         self._check_angles(angles)
         for i, angle in enumerate(angles):
             self.axes[i].angle = float(angle)
 
     def _check_angles(self, angles: list[float]) -> None:
-        """Raises an appropriate error if the submitted angles are incompatible with the sample holder"""
+        """Raises an appropriate error if the submitted angles are incompatible with the sample holder
+        """
         if len(angles) == 1 and isinstance(angles[0], (list, tuple, np.ndarray)):
             angles = angles[0]
         if len(angles) > len(self.angles):
             raise ValueError(
                 f"Too many angles. Expexted {len(self.angles)}, got {len(angles)}"
             )
         if len(angles) < len(self.angles):
@@ -58,34 +63,35 @@
         if not all(ax.min <= angle <= ax.max for angle, ax in zip(angles, self.axes)):
             raise IndexError(
                 "Angle out of range for one or more axes"
                 + f"\n{angles = }\n{self.angles = }\n{self.axes = }"
             )
 
     def reset_rotation(self):
-        """Resets the sample holder to the angles it was initialized with"""
+        """Resets the sample holder to the angles it was initialized with
+        """
         self.rotate_to(self._initial_angles)
 
     def rotate_to(self, *angles: float, degrees: bool = False):
         """Sets the angles of all rotation axes to the given angles
 
-        Args:
-            degrees (bool, optional): Whether the given angles are in degrees or radians. Defaults to False.
+        :param degrees: Whether angles are in degrees(True) or radians(False), defaults to False
+        :type degrees: bool, optional
         """
         if len(angles) == 1 and isinstance(angles[0], (list, tuple, np.ndarray)):
             angles = angles[0]
         if degrees:
             angles = np.deg2rad(angles)
         self.angles = angles
 
     def rotate(self, *angles: float, degrees: bool = False):
         """Rotates the sample holder by the given angles from the current position
 
-        Args:
-            degrees (bool, optional): Whether the given angles are in degrees or radians. Defaults to False.
+        :param degrees: Whether angles are in degrees(True) or radians(False), defaults to False
+        :type degrees: bool, optional
         """
         if len(angles) == 1 and isinstance(angles[0], (list, tuple, np.ndarray)):
             angles = angles[0]
         if degrees:
             angles = list(np.deg2rad(angles))
         self._check_angles(angles)
         angles = [current + target for target, current in zip(angles, self.angles)]
@@ -100,18 +106,37 @@
                 R = R * axis.R
             else:
                 R = axis.R * R
 
         return R
 
     def rotation_matrix(self) -> np.ndarray:
-        """Returns the 3x3 rotation matrix transforming the TEM coordinate system to the sample holder coordinate system"""
+        """Returns the 3x3 rotation matrix transforming the 
+        TEM coordinate system to the sample holder coordinate system
+
+        :return: Rotation matrix
+        :rtype: np.ndarray
+        """
         return self._rotation.to_matrix().squeeze()
 
     to_matrix = rotation_matrix
     as_matrix = rotation_matrix
 
     def sample_frame_to_TEM_frame(self, v: Vector3d) -> Vector3d:
+        """Convert a vector in sample coordinates to TEM coordinates
+
+        :param v: Sample vector
+        :type v: Vector3d
+        :return: TEM vector
+        :rtype: Vector3d
+        """
         return self._rotation * v
 
     def TEM_frame_to_sample_frame(self, v: Vector3d) -> Vector3d:
+        """Convert a vector in TEM coordinates to sample coordinates
+
+        :param v: TEM vector
+        :type v: Vector3d
+        :return: Sample vector
+        :rtype: Vector3d
+        """
         return ~self._rotation * v
```

### Comparing `tiltlib-0.0.5/src/tiltlib.egg-info/PKG-INFO` & `tiltlib-0.1/src/tiltlib.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiltlib
-Version: 0.0.5
+Version: 0.1
 Summary: TEM tilt holder scripts
 Author-email: Viljar Femoen <viljarjf@stud.ntnu.no>
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -15,14 +15,20 @@
 Requires-Dist: matplotlib
 Requires-Dist: hyperspy
 Requires-Dist: scipy
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-xdist; extra == "test"
 Requires-Dist: filelock; extra == "test"
+Provides-Extra: docs
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: sphinx-rtd-theme; extra == "docs"
+Requires-Dist: nbsphinx; extra == "docs"
+Requires-Dist: IPython; extra == "docs"
+Requires-Dist: ipykernel; extra == "docs"
 
 # tiltlib
 
 Tilt TEM sample holders
 
 # Installation
```

### Comparing `tiltlib-0.0.5/tests/test_axis.py` & `tiltlib-0.1/tests/test_axis.py`

 * *Files identical despite different names*

### Comparing `tiltlib-0.0.5/tests/test_rotation_generators.py` & `tiltlib-0.1/tests/test_rotation_generators.py`

 * *Files identical despite different names*

### Comparing `tiltlib-0.0.5/tests/test_sample.py` & `tiltlib-0.1/tests/test_sample.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 
 @pytest.mark.parametrize(
     "initial_angle",
     [0, -10, 10],
 )
 def test_reset_rotation(initial_angle: float, x, default_xmap):
     original_xmap = default_xmap
-    s = Sample(default_xmap, [Axis(x, -100, 100, initial_angle, degrees=True)])
+    s = Sample.from_crystal_map(
+        default_xmap, [Axis(x, -100, 100, initial_angle, degrees=True)]
+    )
 
     assert s.orientations == original_xmap.orientations.reshape(*original_xmap.shape)
 
     s.rotate(50, degrees=True)
 
     assert s.orientations != original_xmap.orientations.reshape(*original_xmap.shape)
 
@@ -29,16 +31,20 @@
         [0, 0],
         [0, 10],
         [-10, 10],
         [4, 20],
     ],
 )
 def test_initial_angle(angle_1: float, angle_2: float, default_xmap, x):
-    s1 = Sample(default_xmap, [Axis(x, -100, 100, angle_1, degrees=True)])
-    s2 = Sample(default_xmap, [Axis(x, -100, 100, angle_2, degrees=True)])
+    s1 = Sample.from_crystal_map(
+        default_xmap, [Axis(x, -100, 100, angle_1, degrees=True)]
+    )
+    s2 = Sample.from_crystal_map(
+        default_xmap, [Axis(x, -100, 100, angle_2, degrees=True)]
+    )
 
     assert s1.orientations == s2.orientations
 
     s1.rotate(5, degrees=True)
     s2.rotate(5, degrees=True)
 
     assert s1.orientations == s2.orientations
@@ -55,16 +61,16 @@
     s1.rotate_to(angle_1 - 10, degrees=True)
     s2.rotate_to(angle_2 - 10, degrees=True)
 
     assert s1.orientations == s2.orientations
 
 
 def test_rotate_to(default_xmap, x):
-    s1 = Sample(default_xmap, [Axis(x, -100, 100, degrees=True)])
-    s2 = Sample(default_xmap, [Axis(x, -100, 100, degrees=True)])
+    s1 = Sample.from_crystal_map(default_xmap, [Axis(x, -100, 100, degrees=True)])
+    s2 = Sample.from_crystal_map(default_xmap, [Axis(x, -100, 100, degrees=True)])
 
     assert s1.orientations == s2.orientations
 
     s1.rotate(5, degrees=True)
     s2.rotate_to(5, degrees=True)
 
     assert s1.orientations == s2.orientations
@@ -82,16 +88,16 @@
     s1.reset_rotation()
     s2.reset_rotation()
 
     assert s1.orientations == s2.orientations
 
 
 def test_rotate_to_with_initial_angle(x, default_xmap):
-    s1 = Sample(default_xmap, [Axis(x, -100, 100, 10, degrees=True)])
-    s2 = Sample(default_xmap, [Axis(x, -100, 100, degrees=True)])
+    s1 = Sample.from_crystal_map(default_xmap, [Axis(x, -100, 100, 10, degrees=True)])
+    s2 = Sample.from_crystal_map(default_xmap, [Axis(x, -100, 100, degrees=True)])
 
     assert s1.orientations == s2.orientations
 
     s1.rotate(-5, degrees=True)
     s2.rotate_to(5, degrees=True)
 
     assert all([a1 == a2 for a1, a2 in zip(s1.angles, s2.angles)])
@@ -113,19 +119,19 @@
 
     s2.reset_rotation()
 
     assert s1.orientations == s2.orientations
 
 
 def test_rotating_to_initial_angle(x, default_xmap):
-    s1 = Sample(default_xmap, [Axis(x, -100, 100, degrees=True)])
+    s1 = Sample.from_crystal_map(default_xmap, [Axis(x, -100, 100, degrees=True)])
 
     s1.rotate_to(5, degrees=True)
 
-    s2 = Sample(s1.xmap, [Axis(x, -100, 100, 5, degrees=True)])
+    s2 = Sample(s1.orientations, s1.phase, [Axis(x, -100, 100, 5, degrees=True)])
 
     assert s1.orientations == s2.orientations
 
     s1.reset_rotation()
     s2.rotate_to(0, degrees=True)
 
     assert s1.orientations == s2.orientations
```

### Comparing `tiltlib-0.0.5/tests/test_sampleholder.py` & `tiltlib-0.1/tests/test_sampleholder.py`

 * *Files identical despite different names*

