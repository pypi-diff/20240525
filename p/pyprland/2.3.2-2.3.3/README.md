# Comparing `tmp/pyprland-2.3.2.tar.gz` & `tmp/pyprland-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprland-2.3.2.tar", max compression
+gzip compressed data, was "pyprland-2.3.3.tar", max compression
```

## Comparing `pyprland-2.3.2.tar` & `pyprland-2.3.3.tar`

### file list

```diff
@@ -1,38 +1,39 @@
--rw-r--r--   0        0        0     1070 2024-02-16 16:53:56.731771 pyprland-2.3.2/LICENSE
--rw-r--r--   0        0        0     5431 2024-05-20 14:30:47.518292 pyprland-2.3.2/README.md
--rw-r--r--   0        0        0       24 2024-05-16 19:14:17.152144 pyprland-2.3.2/pyprland/__init__.py
--rw-r--r--   0        0        0       38 2024-05-16 19:14:17.148810 pyprland-2.3.2/pyprland/adapters/__init__.py
--rw-r--r--   0        0        0      386 2024-05-16 19:14:17.148810 pyprland-2.3.2/pyprland/adapters/colors.py
--rw-r--r--   0        0        0     4848 2024-05-19 09:02:05.262228 pyprland-2.3.2/pyprland/adapters/menus.py
--rw-r--r--   0        0        0     1462 2024-05-16 20:28:22.384986 pyprland-2.3.2/pyprland/adapters/units.py
--rw-r--r--   0        0        0    18490 2024-05-18 23:11:38.369254 pyprland-2.3.2/pyprland/command.py
--rw-r--r--   0        0        0     8849 2024-05-20 16:29:06.584044 pyprland-2.3.2/pyprland/common.py
--rw-r--r--   0        0        0     8097 2024-05-19 00:15:04.411549 pyprland-2.3.2/pyprland/ipc.py
--rw-r--r--   0        0        0       49 2024-05-16 19:14:17.152144 pyprland-2.3.2/pyprland/plugins/__init__.py
--rw-r--r--   0        0        0      115 2024-05-16 19:14:17.152144 pyprland-2.3.2/pyprland/plugins/experimental.py
--rw-r--r--   0        0        0     1658 2024-05-16 20:12:25.826075 pyprland-2.3.2/pyprland/plugins/expose.py
--rw-r--r--   0        0        0     1370 2024-05-16 19:14:17.152144 pyprland-2.3.2/pyprland/plugins/fetch_client_menu.py
--rw-r--r--   0        0        0     2723 2024-05-17 21:51:17.035559 pyprland-2.3.2/pyprland/plugins/gbar.py
--rw-r--r--   0        0        0     2657 2024-05-19 00:11:17.726169 pyprland-2.3.2/pyprland/plugins/interface.py
--rw-r--r--   0        0        0     8084 2024-05-18 12:50:01.915976 pyprland-2.3.2/pyprland/plugins/layout_center.py
--rw-r--r--   0        0        0     1731 2024-05-16 20:31:35.359564 pyprland-2.3.2/pyprland/plugins/lost_windows.py
--rw-r--r--   0        0        0     2519 2024-05-20 13:22:13.839156 pyprland-2.3.2/pyprland/plugins/magnify.py
--rw-r--r--   0        0        0    12344 2024-05-20 16:05:49.299731 pyprland-2.3.2/pyprland/plugins/monitors.py
--rw-r--r--   0        0        0     3817 2024-05-16 19:14:17.152144 pyprland-2.3.2/pyprland/plugins/monitors_v0.py
--rw-r--r--   0        0        0     3121 2024-05-16 20:27:48.054173 pyprland-2.3.2/pyprland/plugins/pyprland.py
--rw-r--r--   0        0        0    31614 2024-05-18 23:58:44.507673 pyprland-2.3.2/pyprland/plugins/scratchpads/__init__.py
--rw-r--r--   0        0        0     2842 2024-05-17 17:55:08.207991 pyprland-2.3.2/pyprland/plugins/scratchpads/animations.py
--rw-r--r--   0        0        0     2702 2024-05-18 12:34:55.300430 pyprland-2.3.2/pyprland/plugins/scratchpads/helpers.py
--rw-r--r--   0        0        0     4036 2024-05-18 13:07:36.207295 pyprland-2.3.2/pyprland/plugins/scratchpads/lookup.py
--rw-r--r--   0        0        0     6033 2024-05-18 23:57:10.361129 pyprland-2.3.2/pyprland/plugins/scratchpads/objects.py
--rw-r--r--   0        0        0     1103 2024-05-16 20:02:45.022300 pyprland-2.3.2/pyprland/plugins/shift_monitors.py
--rw-r--r--   0        0        0     4245 2024-05-18 12:58:41.979853 pyprland-2.3.2/pyprland/plugins/shortcuts_menu.py
--rw-r--r--   0        0        0     4804 2024-05-16 20:40:18.898697 pyprland-2.3.2/pyprland/plugins/system_notifier.py
--rw-r--r--   0        0        0      570 2024-05-16 19:14:17.152144 pyprland-2.3.2/pyprland/plugins/toggle_dpms.py
--rw-r--r--   0        0        0     1120 2024-05-16 19:55:58.745845 pyprland-2.3.2/pyprland/plugins/toggle_special.py
--rw-r--r--   0        0        0     5828 2024-05-20 14:35:57.473856 pyprland-2.3.2/pyprland/plugins/wallpapers.py
--rw-r--r--   0        0        0     2496 2024-05-16 19:55:44.465502 pyprland-2.3.2/pyprland/plugins/workspaces_follow_focus.py
--rw-r--r--   0        0        0     1459 2024-05-17 22:24:00.284438 pyprland-2.3.2/pyprland/types.py
--rw-r--r--   0        0        0       42 2024-05-20 16:36:25.329685 pyprland-2.3.2/pyprland/version.py
--rw-r--r--   0        0        0     2124 2024-05-20 16:36:25.323018 pyprland-2.3.2/pyproject.toml
--rw-r--r--   0        0        0     5970 1970-01-01 00:00:00.000000 pyprland-2.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-02-16 16:53:56.731771 pyprland-2.3.3/LICENSE
+-rw-r--r--   0        0        0     5553 2024-05-23 18:58:37.218905 pyprland-2.3.3/README.md
+-rw-r--r--   0        0        0       24 2024-05-16 19:14:17.152144 pyprland-2.3.3/pyprland/__init__.py
+-rw-r--r--   0        0        0       38 2024-05-16 19:14:17.148810 pyprland-2.3.3/pyprland/adapters/__init__.py
+-rw-r--r--   0        0        0      386 2024-05-16 19:14:17.148810 pyprland-2.3.3/pyprland/adapters/colors.py
+-rw-r--r--   0        0        0     4848 2024-05-19 09:02:05.262228 pyprland-2.3.3/pyprland/adapters/menus.py
+-rw-r--r--   0        0        0     1462 2024-05-16 20:28:22.384986 pyprland-2.3.3/pyprland/adapters/units.py
+-rw-r--r--   0        0        0    18490 2024-05-22 23:20:39.841357 pyprland-2.3.3/pyprland/command.py
+-rw-r--r--   0        0        0     8849 2024-05-20 16:29:06.584044 pyprland-2.3.3/pyprland/common.py
+-rw-r--r--   0        0        0     8097 2024-05-19 00:15:04.411549 pyprland-2.3.3/pyprland/ipc.py
+-rw-r--r--   0        0        0       49 2024-05-16 19:14:17.152144 pyprland-2.3.3/pyprland/plugins/__init__.py
+-rw-r--r--   0        0        0      115 2024-05-16 19:14:17.152144 pyprland-2.3.3/pyprland/plugins/experimental.py
+-rw-r--r--   0        0        0     1658 2024-05-16 20:12:25.826075 pyprland-2.3.3/pyprland/plugins/expose.py
+-rw-r--r--   0        0        0     1370 2024-05-16 19:14:17.152144 pyprland-2.3.3/pyprland/plugins/fetch_client_menu.py
+-rw-r--r--   0        0        0     2723 2024-05-17 21:51:17.035559 pyprland-2.3.3/pyprland/plugins/gbar.py
+-rw-r--r--   0        0        0     2657 2024-05-19 00:11:17.726169 pyprland-2.3.3/pyprland/plugins/interface.py
+-rw-r--r--   0        0        0     8084 2024-05-18 12:50:01.915976 pyprland-2.3.3/pyprland/plugins/layout_center.py
+-rw-r--r--   0        0        0     1731 2024-05-16 20:31:35.359564 pyprland-2.3.3/pyprland/plugins/lost_windows.py
+-rw-r--r--   0        0        0     2743 2024-05-23 22:10:42.465750 pyprland-2.3.3/pyprland/plugins/magnify.py
+-rw-r--r--   0        0        0      853 2024-05-23 17:45:08.310387 pyprland-2.3.3/pyprland/plugins/magnify.py.rej
+-rw-r--r--   0        0        0    12344 2024-05-23 17:45:08.310387 pyprland-2.3.3/pyprland/plugins/monitors.py
+-rw-r--r--   0        0        0     3817 2024-05-16 19:14:17.152144 pyprland-2.3.3/pyprland/plugins/monitors_v0.py
+-rw-r--r--   0        0        0     4043 2024-05-23 22:04:00.478257 pyprland-2.3.3/pyprland/plugins/pyprland.py
+-rw-r--r--   0        0        0    33252 2024-05-23 21:00:25.232123 pyprland-2.3.3/pyprland/plugins/scratchpads/__init__.py
+-rw-r--r--   0        0        0     3029 2024-05-23 20:18:07.804666 pyprland-2.3.3/pyprland/plugins/scratchpads/animations.py
+-rw-r--r--   0        0        0     2702 2024-05-18 12:34:55.300430 pyprland-2.3.3/pyprland/plugins/scratchpads/helpers.py
+-rw-r--r--   0        0        0     4036 2024-05-18 13:07:36.207295 pyprland-2.3.3/pyprland/plugins/scratchpads/lookup.py
+-rw-r--r--   0        0        0     6118 2024-05-24 16:27:21.239418 pyprland-2.3.3/pyprland/plugins/scratchpads/objects.py
+-rw-r--r--   0        0        0     1103 2024-05-16 20:02:45.022300 pyprland-2.3.3/pyprland/plugins/shift_monitors.py
+-rw-r--r--   0        0        0     4245 2024-05-18 12:58:41.979853 pyprland-2.3.3/pyprland/plugins/shortcuts_menu.py
+-rw-r--r--   0        0        0     4804 2024-05-16 20:40:18.898697 pyprland-2.3.3/pyprland/plugins/system_notifier.py
+-rw-r--r--   0        0        0      570 2024-05-16 19:14:17.152144 pyprland-2.3.3/pyprland/plugins/toggle_dpms.py
+-rw-r--r--   0        0        0     1120 2024-05-16 19:55:58.745845 pyprland-2.3.3/pyprland/plugins/toggle_special.py
+-rw-r--r--   0        0        0     5828 2024-05-20 14:35:57.473856 pyprland-2.3.3/pyprland/plugins/wallpapers.py
+-rw-r--r--   0        0        0     2496 2024-05-16 19:55:44.465502 pyprland-2.3.3/pyprland/plugins/workspaces_follow_focus.py
+-rw-r--r--   0        0        0     1471 2024-05-23 19:18:57.916054 pyprland-2.3.3/pyprland/types.py
+-rw-r--r--   0        0        0       42 2024-05-24 16:31:22.172513 pyprland-2.3.3/pyprland/version.py
+-rw-r--r--   0        0        0     2124 2024-05-24 16:31:22.165846 pyprland-2.3.3/pyproject.toml
+-rw-r--r--   0        0        0     6092 1970-01-01 00:00:00.000000 pyprland-2.3.3/PKG-INFO
```

### Comparing `pyprland-2.3.2/LICENSE` & `pyprland-2.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.2/README.md` & `pyprland-2.3.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 Contributing
 </summary>
 
 Check out the [creating a pull request](https://docs.github.com/fr/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request) document for guidance.
 
 - Report bugs or propose features [here](https://github.com/hyprland-community/pyprland/issues)
 - Improve our [wiki](https://github.com/hyprland-community/pyprland/wiki)
+- Read the [internal ticket list](https://github.com/hyprland-community/pyprland/blob/main/tickets.rst) for some PR ideas
 
 and if you have coding skills you can also
 
 - Enhance the coverage of our [tests](https://github.com/hyprland-community/pyprland/tree/main/tests)
 - Propose & write new plugins or enhancements
 
 </details>
```

### Comparing `pyprland-2.3.2/pyprland/adapters/menus.py` & `pyprland-2.3.3/pyprland/adapters/menus.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.2/pyprland/adapters/units.py` & `pyprland-2.3.3/pyprland/adapters/units.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.2/pyprland/command.py` & `pyprland-2.3.3/pyprland/command.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.2/pyprland/common.py` & `pyprland-2.3.3/pyprland/common.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.2/pyprland/ipc.py` & `pyprland-2.3.3/pyprland/ipc.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.2/pyprland/plugins/expose.py` & `pyprland-2.3.3/pyprland/plugins/expose.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.2/pyprland/plugins/fetch_client_menu.py` & `pyprland-2.3.3/pyprland/plugins/fetch_client_menu.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.2/pyprland/plugins/gbar.py` & `pyprland-2.3.3/pyprland/plugins/gbar.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.2/pyprland/plugins/interface.py` & `pyprland-2.3.3/pyprland/plugins/interface.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.2/pyprland/plugins/layout_center.py` & `pyprland-2.3.3/pyprland/plugins/layout_center.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.2/pyprland/plugins/lost_windows.py` & `pyprland-2.3.3/pyprland/plugins/lost_windows.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.2/pyprland/plugins/magnify.py` & `pyprland-2.3.3/pyprland/plugins/magnify.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 """Toggles workspace zooming."""
 
 import asyncio
 from collections.abc import Iterable
 
+from ..common import state
+from ..types import VersionInfo
 from .interface import Plugin
 
 
-class Extension(Plugin):  # pylint: disable=missing-class-docstring
+class Extension(Plugin):
     """Control workspace zooming."""
 
     zoomed = False
 
     cur_factor = 1.0
 
+    keyword = "cursor:zoom_factor"
+
+    async def init(self) -> None:
+        """Initialization code."""
+        if state.hyprland_version < VersionInfo(0, 41, 0):
+            self.keyword = "misc:cursor_zoom_factor"
+
     def ease_out_quad(self, step: float, start: int, end: int, duration: int) -> float:
         """Easing function for animations."""
         step /= duration
         return -end * step * (step - 2) + start
 
     def animated_eased_zoom(self, start: int, end: int, duration: int) -> Iterable[float]:
         """Add easing to an animation.
@@ -60,12 +69,12 @@
 
         self.cur_factor = max(self.cur_factor, 1)
 
         if animated:
             start = (2.0 ** (prev_factor - 1) if expo else prev_factor) * 10
             end = (2.0 ** (self.cur_factor - 1) if expo else self.cur_factor) * 10
             for i in self.animated_eased_zoom(start, end, duration):
-                await self.hyprctl(f"misc:cursor_zoom_factor {i / 10}", "keyword")
+                await self.hyprctl(f"{self.keyword} {i / 10:.4f}", "keyword")
                 await asyncio.sleep(1.0 / 60)
         self.zoomed = self.cur_factor != 1
         factor = 2 ** (self.cur_factor - 1) if expo else self.cur_factor
-        await self.hyprctl(f"misc:cursor_zoom_factor {factor}", "keyword")
+        await self.hyprctl(f"{self.keyword} {factor:.4f}", "keyword")
```

### Comparing `pyprland-2.3.2/pyprland/plugins/monitors.py` & `pyprland-2.3.3/pyprland/plugins/monitors.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         if centered:
             x += int((scaled_om_w - scaled_m_w) / 2)
         elif "end" in place:
             x += int(scaled_om_w - scaled_m_w)
     elif centered:
         y += int((scaled_om_h - scaled_m_h) / 2)
     elif "end" in place:
-        y += scaled_m_h - scaled_om_h
+        y -= scaled_m_h - scaled_om_h
 
     return (x, y)
 
 
 def build_graph(config: dict[str, dict[str, list[str]]]) -> dict[str, list[str]]:
     """Make a sorted graph based on the cleaned_config."""
     graph = defaultdict(list)
@@ -107,29 +107,29 @@
         monitors = await self.hyprctl_json("monitors")
         if self.cast_bool(self.config.get("startup_relayout"), True):
             await self.run_relayout(monitors)
 
         for mon in state.monitors:
             await self._hotplug_command(name=mon, monitors=monitors)
 
-    # Command
-
     def _build_monitor_command(self, monitor: MonitorInfo, config: dict[str, dict[str, Any]], every_monitor: dict[str, MonitorInfo]) -> str:
         """Build the monitor command."""
         name = monitor["name"]
         this_config = config.get(name, {})
         rate = this_config.get("rate", every_monitor[name]["refreshRate"])
         res = this_config.get("resolution", f"{every_monitor[name]['width']}x{every_monitor[name]['height']}")
         if isinstance(res, list):
             res = f"{res[0]}x{res[1]}"
         scale = this_config.get("scale", every_monitor[name]["scale"])
         position = f"{monitor['x']}x{monitor['y']}"
         transform = this_config.get("transform", every_monitor[name]["transform"])
         return f"monitor {name},{res}@{rate},{position},{scale},transform,{transform}"
 
+    # Command
+
     async def run_relayout(self, monitors: list[MonitorInfo] | str | None = None) -> bool:
         """Recompute & apply every monitors's layout."""
         if isinstance(monitors, str):
             self.log.error("relayout doesn't take any argument")
             await self.notify_error("relayout doesn't take any argument")
             return False
```

### Comparing `pyprland-2.3.2/pyprland/plugins/monitors_v0.py` & `pyprland-2.3.3/pyprland/plugins/monitors_v0.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.2/pyprland/plugins/pyprland.py` & `pyprland-2.3.3/pyprland/plugins/pyprland.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,40 +2,53 @@
 
 import json
 
 from ..common import MINIMUM_ADDR_LEN, state
 from ..types import VersionInfo
 from .interface import Plugin
 
+DEFAULT_VERSION = VersionInfo(9, 9, 9)
+
 
 class Extension(Plugin):
     """Internal built-in plugin allowing caching states and implementing special commands."""
 
     async def init(self) -> None:
         """Initialize the plugin."""
         state.active_window = ""
+        # Examples:
+        # "tag": "v0.40.0-127-g4e42107d", (for git)
+        # "tag": "v0.40.0", (stable)
+        version_str = ""
+        auto_increment = False
         try:
-            version_info = await self.hyprctl_json("version")
+            version_info: None | dict[str, str | bool | list] = await self.hyprctl_json("version")
+            assert isinstance(version_info, dict)
         except json.JSONDecodeError:
             self.log.exception("Fail to parse hyprctl version")
-            await self.notify_error("Error: 'hyprctl version': incorrect JSON data")
-            version = "v0.0.0"
+            await self.notify_error("Error: 'hyprctl version' didn't print valid data")
         else:
-            if version_info.get("tag"):
-                version = version_info["tag"].split("-", 1)[0]
-            else:
-                version = "v9.9.9"
-                self.log.warning("No tag available, assuming a recent git version.")
-
-        try:
-            state.hyprland_version = VersionInfo(*(int(i) for i in version[1:].split(".")[:3]))
-        except Exception:  # pylint: disable=broad-except
-            self.log.exception('Fail to parse version tag "%s"', version)
-            await self.notify_error(f"Failed to parse hyprctl version tag: {version}")
-            state.hyprland_version = VersionInfo(0, 0, 0)
+            _tag = version_info.get("tag")
+            if _tag:
+                assert isinstance(_tag, str)
+                version_str = _tag.split("-", 1)[0]
+                if len(version_str) < len(_tag):
+                    auto_increment = True
+
+        if version_str:
+            try:
+                self.__set_hyprland_version(version_str[1:], auto_increment)
+            except Exception:  # pylint: disable=broad-except
+                self.log.exception('Fail to parse version tag "%s"', version_str)
+                await self.notify_error(f"Failed to parse hyprctl version tag: {version_str}")
+                version_str = ""
+
+        if not version_str:
+            self.log.error("Fail to parse version information: %s", version_info)
+            state.hyprland_version = DEFAULT_VERSION
 
         state.active_workspace = (await self.hyprctl_json("activeworkspace"))["name"]
         monitors = await self.hyprctl_json("monitors")
         state.monitors = [mon["name"] for mon in monitors]
         state.active_monitor = next(mon["name"] for mon in monitors if mon["focused"])
 
     async def event_monitoradded(self, name: str) -> None:
@@ -45,31 +58,41 @@
     async def event_monitorremoved(self, name: str) -> None:
         """Track monitor."""
         state.monitors.remove(name)
 
     async def on_reload(self) -> None:
         """Reload the plugin."""
         state.variables = self.config.get("variables", {})
+        version_override = self.config.get("hyprland_version")
+        if version_override:
+            self.__set_hyprland_version(version_override)
 
     async def event_activewindowv2(self, addr: str) -> None:
         """Keep track of the focused client."""
         if not addr or len(addr) < MINIMUM_ADDR_LEN:
             self.log.warning("Active window is incorrect: %s.", addr)
             state.active_window = ""
         else:
             state.active_window = "0x" + addr
             self.log.debug("active_window = %s", state.active_window)
 
-    async def event_workspace(self, wrkspace: str) -> None:
+    async def event_workspace(self, workspace: str) -> None:
         """Track the active workspace."""
-        state.active_workspace = wrkspace
+        state.active_workspace = workspace
         self.log.debug("active_workspace = %s", state.active_workspace)
 
     async def event_focusedmon(self, mon: str) -> None:
         """Track the active workspace."""
         state.active_monitor, state.active_workspace = mon.rsplit(",", 1)
         self.log.debug("active_monitor = %s", state.active_monitor)
 
     def set_commands(self, **cmd_map) -> None:
         """Set some commands, made available as run_`name` methods."""
         for name, fn in cmd_map.items():
             setattr(self, f"run_{name}", fn)
+
+    def __set_hyprland_version(self, version_str: str, auto_increment: bool = False) -> None:
+        """Set the hyprland version."""
+        split_version = [int(i) for i in version_str.split(".")[:3]]
+        if auto_increment:
+            split_version[-1] += 1
+        state.hyprland_version = VersionInfo(*split_version)
```

### Comparing `pyprland-2.3.2/pyprland/plugins/scratchpads/__init__.py` & `pyprland-2.3.3/pyprland/plugins/scratchpads/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,51 @@
 """Scratchpads addon."""
 
 import asyncio
 import contextlib
+import enum
 import time
 from dataclasses import dataclass
 from functools import partial
 from typing import cast
 
 from ...adapters.units import convert_coords, convert_monitor_dimension
 from ...common import MINIMUM_ADDR_LEN, CastBoolMixin, apply_variables, is_rotated, state
 from ...ipc import get_client_props, get_focused_monitor_props, notify_error
 from ...types import ClientInfo, MonitorInfo
 from ..interface import Plugin
-from .animations import Animations
+from .animations import Placement
 from .helpers import get_active_space_identifier, get_all_space_identifiers, get_match_fn
 from .lookup import ScratchDB
 from .objects import Scratch
 
 AFTER_SHOW_INHIBITION = 0.3  # 300ms of ignorance after a show
 DEFAULT_MARGIN = 60  # in pixels
 DEFAULT_HIDE_DELAY = 0.2  # in seconds
 DEFAULT_HYSTERESIS = 0.4  # in seconds
 
 
+class AnimationTarget(enum.Enum):
+    """Animation type (selects between main window and satellite windows)."""
+
+    MAIN = "main"
+    EXTRA = "extra"
+    ALL = "all"
+
+
+def compute_offset(pos1: tuple[int, int], pos2: tuple[int, int]) -> tuple[int, int]:
+    """Compute the offset between two positions."""
+    return pos1[0] - pos2[0], pos1[1] - pos2[1]
+
+
+def apply_offset(pos: tuple[int, int], offset: tuple[int, int]) -> tuple[int, int]:
+    """Apply the offset to the position."""
+    return pos[0] + offset[0], pos[1] + offset[1]
+
+
 @dataclass
 class FocusTracker:
     """Focus tracking object."""
 
     prev_focused_window: str
     prev_focused_window_wrkspc: str
 
@@ -481,19 +500,22 @@
         return True
 
     async def _slide_animation(
         self,
         animation_type: str,
         scratch: Scratch,
         offset: tuple[int, int],
-        only_secondary: bool = False,
+        target: AnimationTarget = AnimationTarget.ALL,
     ) -> None:
         """Slides the window `offset` pixels respecting `animation_type`."""
-        addresses = [] if only_secondary else [scratch.full_address]
-        addresses.extend(scratch.extra_addr)
+        addresses: list[str] = []
+        if target != AnimationTarget.MAIN:
+            addresses.extend(scratch.extra_addr)
+        if target != AnimationTarget.EXTRA:
+            addresses.append(scratch.full_address)
         off_x, off_y = offset
 
         animation_actions = {
             "fromright": f"movewindowpixel {off_x} 0",
             "fromleft": f"movewindowpixel {-off_x} 0",
             "frombottom": f"movewindowpixel 0 {off_y}",
             "fromtop": f"movewindowpixel 0 {-off_y}",
@@ -577,15 +599,15 @@
         if should_set_aspect:
             await self._fix_size(scratch, monitor)
         position_fixed = False
         if should_set_aspect:
             position_fixed = await self._fix_position(scratch, monitor)
 
         clients = await self.hyprctl_json("clients")
-        await self._handle_multiwindow(scratch, clients)  # not very useful but cheap
+        await self._handle_multiwindow(scratch, clients)
         # move
         move_commands = [
             f"moveworkspacetomonitor special:scratch_{scratch.uid} {monitor['name']}",
             f"movetoworkspacesilent {wrkspc},address:{scratch.full_address}",
             f"alterzorder top,address:{scratch.full_address}",
         ]
         for addr in scratch.extra_addr:
@@ -625,32 +647,43 @@
                     break
             else:
                 self.log.exception("Lost the client info for %s", scratch.uid)
 
     async def _animate_show(self, scratch: Scratch, monitor: MonitorInfo, relative_animation: bool) -> None:
         """Animate the show transition."""
         animation_type = get_animation_type(scratch)
+        multiwin_enabled = self.cast_bool(scratch.conf.get("multi"), True)
         if animation_type:
-            offset = cast(tuple[int, int], tuple(-1 * n for n in await self.get_offsets(scratch, monitor)))
             if relative_animation:
+                offset = cast(tuple[int, int], tuple(-1 * n for n in await self.get_offsets(scratch, monitor)))
                 # Relative positioning
                 if "size" not in scratch.client_info:
                     await self.update_scratch_info(scratch)  # type: ignore
 
-                await self._slide_animation(animation_type, scratch, offset)
+                await self._slide_animation(
+                    animation_type, scratch, offset, target=AnimationTarget.ALL if multiwin_enabled else AnimationTarget.MAIN
+                )
             else:
                 # Absolute positioning
-                command = getattr(Animations, animation_type)(
+                commands = []
+                position = Placement.get(
+                    animation_type,
                     monitor,
                     scratch.client_info,
-                    "address:" + scratch.full_address,
                     scratch.conf.get("margin", DEFAULT_MARGIN),
                 )
-                await self.hyprctl(command)
-                await self._slide_animation(animation_type, scratch, offset, only_secondary=True)
+                commands.append(f"movewindowpixel exact {position[0]} {position[1]},address:{scratch.full_address}")
+
+                if multiwin_enabled:
+                    for address in scratch.extra_addr:
+                        off = scratch.meta.extra_positions.get(address)
+                        if off:
+                            pos = apply_offset(position, off)
+                            commands.append(f"movewindowpixel exact {pos[0]} {pos[1]},address:{address}")
+                await self.hyprctl(commands)
         else:
             self.log.warning(
                 "No position and no animation provided for %s, don't know where to place it.",
                 scratch.uid,
             )
 
     async def _fix_size(self, scratch: Scratch, monitor: MonitorInfo) -> None:
@@ -691,15 +724,23 @@
             return
         if not scratch.visible and not force and not autohide:
             await notify_error(f"Scratchpad '{uid}' is not visible, will not hide.")
             self.log.warning("%s is already hidden", uid)
             return
         # collects window which have been created by the app
         if self.cast_bool(scratch.conf.get("multi"), True):
-            await self._handle_multiwindow(scratch, await self.hyprctl_json("clients"))
+            clients = await self.hyprctl_json("clients")
+            await self._handle_multiwindow(scratch, clients)
+            await scratch.update_client_info(clients=clients)
+            ref_position = scratch.client_info["at"]
+            positions = {}
+            for sub_client in clients:
+                if sub_client["address"] in scratch.extra_addr:
+                    positions[sub_client["address"]] = compute_offset(sub_client["at"], ref_position)
+            scratch.meta.extra_positions = positions
         scratch.visible = False
         scratch.meta.should_hide = False
         self.log.info("Hiding %s", uid)
         await self._hide_transition(scratch, scratch.meta.monitor_info)
 
         await self.hyprctl(f"movetoworkspacesilent special:scratch_{uid},address:{scratch.full_address}")
```

### Comparing `pyprland-2.3.2/pyprland/plugins/scratchpads/helpers.py` & `pyprland-2.3.3/pyprland/plugins/scratchpads/helpers.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.2/pyprland/plugins/scratchpads/lookup.py` & `pyprland-2.3.3/pyprland/plugins/scratchpads/lookup.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.2/pyprland/plugins/scratchpads/objects.py` & `pyprland-2.3.3/pyprland/plugins/scratchpads/objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Scratchpad object definition."""
 
 __all__ = ["Scratch"]
 
 import logging
 import os
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from typing import TYPE_CHECKING, Any, Protocol, cast
 
 from aiofiles import open as aiopen
 from aiofiles import os as aios
 
 from ...common import CastBoolMixin, state
 from ...ipc import notify_error
@@ -33,14 +33,15 @@
 
     initialized: bool = False
     should_hide: bool = False
     no_pid: bool = False
     last_shown: float | int = 0
     space_identifier: tuple[str, str] = ("", "")
     monitor_info: MonitorInfo = None  # type: ignore
+    extra_positions: dict[str, tuple[int, int]] = field(default_factory=dict)
 
 
 class Scratch(CastBoolMixin):  # {{{
     """A scratchpad state including configuration & client state."""
 
     log = logging.getLogger("scratch")
     get_client_props: "ClientPropGetter"
```

### Comparing `pyprland-2.3.2/pyprland/plugins/shift_monitors.py` & `pyprland-2.3.3/pyprland/plugins/shift_monitors.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.2/pyprland/plugins/shortcuts_menu.py` & `pyprland-2.3.3/pyprland/plugins/shortcuts_menu.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.2/pyprland/plugins/system_notifier.py` & `pyprland-2.3.3/pyprland/plugins/system_notifier.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.2/pyprland/plugins/toggle_dpms.py` & `pyprland-2.3.3/pyprland/plugins/toggle_dpms.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.2/pyprland/plugins/toggle_special.py` & `pyprland-2.3.3/pyprland/plugins/toggle_special.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.2/pyprland/plugins/wallpapers.py` & `pyprland-2.3.3/pyprland/plugins/wallpapers.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.2/pyprland/plugins/workspaces_follow_focus.py` & `pyprland-2.3.3/pyprland/plugins/workspaces_follow_focus.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.2/pyprland/types.py` & `pyprland-2.3.3/pyprland/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 
 class ClientInfo(TypedDict):
     """Client information as returned by Hyprland."""
 
     address: str
     mapped: bool
     hidden: bool
-    at: list[int]
-    size: list[int]
+    at: tuple[int, int]
+    size: tuple[int, int]
     workspace: WorkspaceDf
     floating: bool
     monitor: int
     class_: str
     title: str
     initialClass: str
     initialTitle: str
```

### Comparing `pyprland-2.3.2/pyproject.toml` & `pyprland-2.3.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pyprland"
-version = "2.3.2"
+version = "2.3.3"
 description = "Hyperland plugin system - batteries included"
 authors = ["fdev31 <fdev31@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pyprland"}]
 homepage = "https://github.com/hyprland-community/pyprland/"
```

### Comparing `pyprland-2.3.2/PKG-INFO` & `pyprland-2.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyprland
-Version: 2.3.2
+Version: 2.3.3
 Summary: Hyperland plugin system - batteries included
 Home-page: https://github.com/hyprland-community/pyprland/
 License: MIT
 Author: fdev31
 Author-email: fdev31@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -54,14 +54,15 @@
 Contributing
 </summary>
 
 Check out the [creating a pull request](https://docs.github.com/fr/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request) document for guidance.
 
 - Report bugs or propose features [here](https://github.com/hyprland-community/pyprland/issues)
 - Improve our [wiki](https://github.com/hyprland-community/pyprland/wiki)
+- Read the [internal ticket list](https://github.com/hyprland-community/pyprland/blob/main/tickets.rst) for some PR ideas
 
 and if you have coding skills you can also
 
 - Enhance the coverage of our [tests](https://github.com/hyprland-community/pyprland/tree/main/tests)
 - Propose & write new plugins or enhancements
 
 </details>
```

