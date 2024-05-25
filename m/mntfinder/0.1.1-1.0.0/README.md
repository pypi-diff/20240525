# Comparing `tmp/mntfinder-0.1.1.tar.gz` & `tmp/mntfinder-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mntfinder-0.1.1.tar", last modified: Sun Jan  7 18:56:21 2024, max compression
+gzip compressed data, was "mntfinder-1.0.0.tar", last modified: Sat May 25 17:02:35 2024, max compression
```

## Comparing `mntfinder-0.1.1.tar` & `mntfinder-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwx------   0 miketsu   (1000) miketsu   (1000)        0 2024-01-07 18:56:21.065195 mntfinder-0.1.1/
--rw-------   0 miketsu   (1000) miketsu   (1000)     1094 2024-01-04 17:03:50.000000 mntfinder-0.1.1/LICENSE
--rw-r--r--   0 miketsu   (1000) miketsu   (1000)     3920 2024-01-07 18:56:21.065195 mntfinder-0.1.1/PKG-INFO
--rw-------   0 miketsu   (1000) miketsu   (1000)     1982 2024-01-07 18:46:09.000000 mntfinder-0.1.1/README.md
--rw-------   0 miketsu   (1000) miketsu   (1000)     1004 2024-01-07 18:46:09.000000 mntfinder-0.1.1/pyproject.toml
--rw-------   0 miketsu   (1000) miketsu   (1000)        6 2024-01-07 18:51:16.000000 mntfinder-0.1.1/requirements.txt
--rw-------   0 miketsu   (1000) miketsu   (1000)       38 2024-01-07 18:56:21.065195 mntfinder-0.1.1/setup.cfg
-drwx------   0 miketsu   (1000) miketsu   (1000)        0 2024-01-07 18:56:21.064195 mntfinder-0.1.1/src/
-drwx------   0 miketsu   (1000) miketsu   (1000)        0 2024-01-07 18:56:21.065195 mntfinder-0.1.1/src/mntfinder.egg-info/
--rw-r--r--   0 miketsu   (1000) miketsu   (1000)     3920 2024-01-07 18:56:21.000000 mntfinder-0.1.1/src/mntfinder.egg-info/PKG-INFO
--rw-------   0 miketsu   (1000) miketsu   (1000)      250 2024-01-07 18:56:21.000000 mntfinder-0.1.1/src/mntfinder.egg-info/SOURCES.txt
--rw-------   0 miketsu   (1000) miketsu   (1000)        1 2024-01-07 18:56:21.000000 mntfinder-0.1.1/src/mntfinder.egg-info/dependency_links.txt
--rw-------   0 miketsu   (1000) miketsu   (1000)        6 2024-01-07 18:56:21.000000 mntfinder-0.1.1/src/mntfinder.egg-info/requires.txt
--rw-------   0 miketsu   (1000) miketsu   (1000)       10 2024-01-07 18:56:21.000000 mntfinder-0.1.1/src/mntfinder.egg-info/top_level.txt
--rw-------   0 miketsu   (1000) miketsu   (1000)     6502 2024-01-07 18:44:04.000000 mntfinder-0.1.1/src/mntfinder.py
+drwx------   0 miketsu   (1000) miketsu   (1000)        0 2024-05-25 17:02:35.542869 mntfinder-1.0.0/
+-rw-------   0 miketsu   (1000) miketsu   (1000)     1094 2024-01-04 17:03:50.000000 mntfinder-1.0.0/LICENSE
+-rw-r--r--   0 miketsu   (1000) miketsu   (1000)     7351 2024-05-25 17:02:35.542869 mntfinder-1.0.0/PKG-INFO
+-rw-------   0 miketsu   (1000) miketsu   (1000)     5413 2024-05-25 17:02:13.000000 mntfinder-1.0.0/README.md
+-rw-------   0 miketsu   (1000) miketsu   (1000)     1004 2024-01-07 18:46:09.000000 mntfinder-1.0.0/pyproject.toml
+-rw-------   0 miketsu   (1000) miketsu   (1000)        6 2024-01-07 18:51:16.000000 mntfinder-1.0.0/requirements.txt
+-rw-------   0 miketsu   (1000) miketsu   (1000)       38 2024-05-25 17:02:35.542869 mntfinder-1.0.0/setup.cfg
+drwx------   0 miketsu   (1000) miketsu   (1000)        0 2024-05-25 17:02:35.541869 mntfinder-1.0.0/src/
+drwx------   0 miketsu   (1000) miketsu   (1000)        0 2024-05-25 17:02:35.542869 mntfinder-1.0.0/src/mntfinder.egg-info/
+-rw-r--r--   0 miketsu   (1000) miketsu   (1000)     7351 2024-05-25 17:02:35.000000 mntfinder-1.0.0/src/mntfinder.egg-info/PKG-INFO
+-rw-------   0 miketsu   (1000) miketsu   (1000)      250 2024-05-25 17:02:35.000000 mntfinder-1.0.0/src/mntfinder.egg-info/SOURCES.txt
+-rw-------   0 miketsu   (1000) miketsu   (1000)        1 2024-05-25 17:02:35.000000 mntfinder-1.0.0/src/mntfinder.egg-info/dependency_links.txt
+-rw-------   0 miketsu   (1000) miketsu   (1000)        6 2024-05-25 17:02:35.000000 mntfinder-1.0.0/src/mntfinder.egg-info/requires.txt
+-rw-------   0 miketsu   (1000) miketsu   (1000)       10 2024-05-25 17:02:35.000000 mntfinder-1.0.0/src/mntfinder.egg-info/top_level.txt
+-rw-------   0 miketsu   (1000) miketsu   (1000)     6139 2024-05-25 17:02:13.000000 mntfinder-1.0.0/src/mntfinder.py
```

### Comparing `mntfinder-0.1.1/LICENSE` & `mntfinder-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mntfinder-0.1.1/pyproject.toml` & `mntfinder-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mntfinder-0.1.1/src/mntfinder.py` & `mntfinder-1.0.0/src/mntfinder.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,56 +1,90 @@
 # -*- encoding: utf-8 -*-
 import os
 from pathlib import PosixPath as Path
 from typing import Iterator
 
 import attrs
 
-__all__ = ['MountPoint', 'findMountPointByTarget', 'listAllMountPoints', 'isMountPoint']
+__all__ = ['MountPointInfo', 'getMountPoint', 'getAllMountPoints', 'isAMountPoint']
 
-__version__ = '0.1.1'
+__version__ = '1.0.0'
 
 
-@attrs.frozen(slots=True, kw_only=True)
-class MountPoint(os.PathLike[str]):
+@attrs.define(slots=True, kw_only=True, eq=False, order=False)
+class MountPointInfo(os.PathLike[str]):
     """
-    Represents a mount point in the file system.
+    A class representing information about a mount point.
+
+    The instance can be used as path-like objects by ``os.path.*``, ``pathlib.Path``, etc.
+    When the instance is used as a path, it reflects the value of the attribute ``target``.
 
     Attributes:
-        source (str): The source of the mount point (e.g., device or network location).
-        target (Path): The target directory where the mount point is mounted.
+        source (str): The source of the mount point.
+        target (Path): The target path of the mount point.
         fstype (str): The file system type of the mount point.
-        options (tuple[str, ...]): The options for the mount point (e.g., read-write, noatime).
-        freq (int): The frequency of file system checks (0 for no checks).
-        passno (int): The pass number for file system checks (0 for no checks).
-    """
-
-    source: str = attrs.field(validator=attrs.validators.instance_of(str))
-    target: Path = attrs.field(validator=attrs.validators.instance_of(Path))
-    fstype: str = attrs.field(validator=attrs.validators.instance_of(str))
+        options (tuple[str, ...]): The options associated with the mount point.
+        freq (int): The frequency of filesystem checks.
+        passno (int): The pass number used by the filesystem checker.
+
+    Methods:
+        isStillMounted(self) -> bool:
+            Returns ``False`` when called if attribute ``target`` is no longer a mount point; otherwise it returns ``True``.
+
+            Once this method starts returning ``False``, it will not return ``True`` on any subsequent calls.
+    """
+    source: str = attrs.field(validator=attrs.validators.instance_of(str), on_setattr=attrs.setters.frozen)
+    target: Path = attrs.field(validator=attrs.validators.instance_of(Path), on_setattr=attrs.setters.frozen)
+    fstype: str = attrs.field(validator=attrs.validators.instance_of(str), on_setattr=attrs.setters.frozen)
     options: tuple[str, ...] = attrs.field(
         validator=attrs.validators.deep_iterable(
             attrs.validators.instance_of(str),
             attrs.validators.instance_of(tuple)
-        )
+        ),
+        on_setattr=attrs.setters.frozen
     )
-    freq: int = attrs.field(validator=attrs.validators.instance_of(int))
-    passno: int = attrs.field(validator=attrs.validators.instance_of(int))
+    freq: int = attrs.field(validator=attrs.validators.instance_of(int), on_setattr=attrs.setters.frozen)
+    passno: int = attrs.field(validator=attrs.validators.instance_of(int), on_setattr=attrs.setters.frozen)
+    __mounted: bool = attrs.field(init=False, repr=False, default=True)
+
+    def __eq__(self, other: 'MountPointInfo', /) -> bool:
+        if type(other) is not type(self):
+            return NotImplemented
+        if not self.isStillMounted():
+            return NotImplemented
+        if not other.isStillMounted():
+            return NotImplemented
+        return (
+                other.source == self.source
+                and other.target == self.target
+                and other.fstype == self.fstype
+                and other.options == self.options
+                and other.freq == self.freq
+                and other.passno == self.passno
+        )
 
     def __fspath__(self) -> str:
+        return os.fspath(self.target)
+
+    def isStillMounted(self) -> bool:
         """
-        Returns the target of the mount point as a string path.
+        Returns ``False`` when called if attribute ``target`` is no longer a mount point; otherwise it returns ``True``.
 
-        Returns:
-            str: The target of the mount point as a string path.
+        Once this method starts returning ``False``, it will not return ``True`` on any subsequent calls.
         """
-        return os.fspath(self.target)
+        if not self.__mounted:
+            return self.__mounted
 
+        mounted = self.target.is_mount()
+        if not mounted:
+            self.__mounted = mounted
+        return mounted
 
-def _parseLineOfMountInfoFile(line: str) -> MountPoint:
+
+def _mountsFileLineToMountPointInfo(line: str) -> MountPointInfo:
     line_parts = [s.replace('\\040', ' ').replace('\\012', '\n') for s in line.strip(' \n').split(' ')]
     if len(line_parts) != 6:
         raise ValueError(f'Not a valid line of mount info: {line!r}')
 
     source = line_parts[0]
     raw_target = line_parts[1]
     fstype = line_parts[2]
@@ -62,103 +96,65 @@
     raw_passno = line_parts[5]
     if not raw_passno.isdigit():
         raise ValueError(f'Invalid value of fs_passno: {raw_passno!r}')
     passno = int(raw_passno)
 
     target = Path(str(bytes(raw_target, encoding='raw_unicode_escape'), encoding='unicode_escape')).resolve()
 
-    return MountPoint(source=source, target=target, fstype=fstype, options=options, freq=freq, passno=passno)
+    return MountPointInfo(source=source, target=target, fstype=fstype, options=options, freq=freq, passno=passno)
 
 
-def _iteratedParseMountInfoFile(*, pid: int | None = None) -> Iterator[MountPoint]:
-    if pid is None:
-        mount_info_file = Path('/proc/mounts')
-    elif isinstance(pid, int):
-        mount_info_file = Path('/proc') / str(int(pid)) / 'mounts'
-    else:
-        raise TypeError('{!r} must be int or None (got {!r})'.format('pid', type(pid)))
+def _iteratedParseMountInfoFile() -> Iterator[MountPointInfo]:
+    mount_info_file = Path('/proc') / 'mounts'
 
     with open(mount_info_file, mode='r', newline='') as f:
         mount_info_text = f.read()
 
     for line in mount_info_text.split('\n'):
         if line:
-            yield _parseLineOfMountInfoFile(line)
+            mount_point_info = _mountsFileLineToMountPointInfo(line)
+            if mount_point_info.isStillMounted():
+                yield mount_point_info
 
 
-def findMountPointByTarget(target: str | bytes | os.PathLike, *, pid: int | None = None) -> MountPoint | None:
+def getMountPoint(target: str | bytes | os.PathLike) -> MountPointInfo | None:
     """
-    Find the mount point object corresponding to the target path.
+    Get the ``MountPointInfo`` object corresponding to the given target path.
 
-    Args:
-        target (str, bytes or os.PathLike): The target path of the mount point to find.
-        pid (int, optional): Optional process ID to filter mount points by. Defaults to None.
+    Parameters:
+        target (str | bytes | os.PathLike): The target path for which to retrieve the ``MountPointInfo`` object.
 
     Returns:
-        MountPoint or None: The mount point object corresponding to the target path, or None if not found.
+        MountPointInfo | None: The ``MountPointInfo`` object corresponding to the target path, or ``None`` if not found.
     """
     target_path = Path(os.fsdecode(target)).resolve()
 
-    for mountpoint in _iteratedParseMountInfoFile(pid=pid):
-        if mountpoint.target != target_path:
+    for mount_point_info in _iteratedParseMountInfoFile():
+        if mount_point_info.target != target_path:
             continue
 
-        return mountpoint
+        return mount_point_info
 
 
-def listAllMountPoints(*, source: str | None = None,
-                       target: str | bytes | os.PathLike | None = None,
-                       fstype: str | None = None,
-                       pid: int | None = None
-                       ) -> list[MountPoint]:
-    """
-    Retrieves a list of mount points in the file system based on specified criteria.
-
-    Args:
-        source (str, optional): The source of the mount point (e.g., device or network location). Defaults to None.
-        target (str | bytes | os.PathLike, optional): The target directory where the mount point is mounted. Defaults to None.
-        fstype (str | None, optional): The file system type of the mount point. Defaults to None.
-        pid (int | None, optional): The process ID for which to retrieve mount points. Defaults to None.
+def getAllMountPoints() -> list[MountPointInfo]:
+    """
+    Return a list of all current mount points on the system.
 
     Returns:
-        list[MountPoint]: A list of MountPoint objects representing the mount points in the file system that match the specified criteria.
+        list[MountPointInfo]: A list of ``MountPointInfo`` objects representing information about each mounted mount point.
     """
-    mountpoints: list[MountPoint] = []
-    target_path = None if target is None else Path(os.fsdecode(target)).resolve()
-
-    for mountpoint in _iteratedParseMountInfoFile(pid=pid):
-        if source is not None and mountpoint.source != source:
-            continue
-        if target_path is not None and mountpoint.target != target_path:
-            continue
-        if fstype is not None and mountpoint.fstype != fstype:
-            continue
-        mountpoints.append(mountpoint)
-
-    return mountpoints
+    return list(_iteratedParseMountInfoFile())
 
 
-def isMountPoint(target: str | bytes | os.PathLike,
-                 *, source: str | None = None,
-                 fstype: str | None = None,
-                 pid: int | None = None
-                 ) -> bool:
+def isAMountPoint(target: str | bytes | os.PathLike | MountPointInfo) -> bool:
     """
-    Check if a given target path is a mount point in the file system.
+    Check if the given ``target`` is a mount point or not.
 
-    Args:
-        target (str, bytes or os.PathLike): The target path to check if it is a mount point.
-        source (str, optional): Optional source of the mount point to filter by. Defaults to None.
-        fstype (str, optional): Optional file system type of the mount point to filter by. Defaults to None.
-        pid (int, optional): Optional process ID to filter mount points by. Defaults to None.
+    Parameters:
+        target (str | bytes | os.PathLike | MountPointInfo): The target to check if it is a mount point or not.
 
     Returns:
-        bool: True if the target path is a mount point that matches the provided filters. False otherwise.
+        bool: ``True`` if the ``target`` is a mount point and still mounted, ``False`` otherwise.
     """
-    if mountpoint := findMountPointByTarget(target, pid=pid):
-        if source is not None and mountpoint.source != source:
-            return False
-        if fstype is not None and mountpoint.fstype != fstype:
-            return False
-        return True
-    else:
-        return False
+    if isinstance(target, MountPointInfo):
+        return target.isStillMounted()
+    return bool(getMountPoint(target))
```

