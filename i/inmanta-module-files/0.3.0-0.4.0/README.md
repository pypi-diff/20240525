# Comparing `tmp/inmanta_module_files-0.3.0-py3-none-any.whl.zip` & `tmp/inmanta_module_files-0.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 21581 bytes, number of entries: 19
--rw-r--r--  2.0 unx      602 b- defN 24-Apr-27 22:30 inmanta_plugins/files/__init__.py
--rw-r--r--  2.0 unx     2624 b- defN 24-Apr-27 22:30 inmanta_plugins/files/base.py
--rw-r--r--  2.0 unx     3188 b- defN 24-Apr-27 22:30 inmanta_plugins/files/directory.py
--rw-r--r--  2.0 unx     6585 b- defN 24-Apr-27 22:30 inmanta_plugins/files/host.py
--rw-r--r--  2.0 unx     7436 b- defN 24-Apr-27 22:30 inmanta_plugins/files/json.py
--rw-r--r--  2.0 unx     2170 b- defN 24-Apr-27 22:31 inmanta_plugins/files/setup.cfg
--rw-r--r--  2.0 unx     2258 b- defN 24-Apr-27 22:30 inmanta_plugins/files/systemd_unit.py
--rw-r--r--  2.0 unx     2200 b- defN 24-Apr-27 22:30 inmanta_plugins/files/text.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-27 22:30 inmanta_plugins/files/files/.gitkeep
--rw-r--r--  2.0 unx     3856 b- defN 24-Apr-27 22:30 inmanta_plugins/files/model/_init.cf
--rw-r--r--  2.0 unx     1661 b- defN 24-Apr-27 22:30 inmanta_plugins/files/model/host.cf
--rw-r--r--  2.0 unx     1586 b- defN 24-Apr-27 22:30 inmanta_plugins/files/model/json.cf
--rw-r--r--  2.0 unx    10884 b- defN 24-Apr-27 22:30 inmanta_plugins/files/model/systemd_unit.cf
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-27 22:30 inmanta_plugins/files/templates/.gitkeep
--rw-r--r--  2.0 unx     2950 b- defN 24-Apr-27 22:30 inmanta_plugins/files/templates/systemd_unit.j2
--rw-r--r--  2.0 unx      742 b- defN 24-Apr-27 22:31 inmanta_module_files-0.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-27 22:31 inmanta_module_files-0.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 24-Apr-27 22:31 inmanta_module_files-0.3.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1721 b- defN 24-Apr-27 22:31 inmanta_module_files-0.3.0.dist-info/RECORD
-19 files, 50571 bytes uncompressed, 18709 bytes compressed:  63.0%
+Zip file size: 22098 bytes, number of entries: 19
+-rw-r--r--  2.0 unx      602 b- defN 24-May-25 14:15 inmanta_plugins/files/__init__.py
+-rw-r--r--  2.0 unx     2624 b- defN 24-May-25 14:15 inmanta_plugins/files/base.py
+-rw-r--r--  2.0 unx     3188 b- defN 24-May-25 14:15 inmanta_plugins/files/directory.py
+-rw-r--r--  2.0 unx     6585 b- defN 24-May-25 14:15 inmanta_plugins/files/host.py
+-rw-r--r--  2.0 unx     7436 b- defN 24-May-25 14:15 inmanta_plugins/files/json.py
+-rw-r--r--  2.0 unx     2170 b- defN 24-May-25 14:15 inmanta_plugins/files/setup.cfg
+-rw-r--r--  2.0 unx     2258 b- defN 24-May-25 14:15 inmanta_plugins/files/systemd_unit.py
+-rw-r--r--  2.0 unx     2200 b- defN 24-May-25 14:15 inmanta_plugins/files/text.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-25 14:15 inmanta_plugins/files/files/.gitkeep
+-rw-r--r--  2.0 unx     3963 b- defN 24-May-25 14:15 inmanta_plugins/files/model/_init.cf
+-rw-r--r--  2.0 unx     1661 b- defN 24-May-25 14:15 inmanta_plugins/files/model/host.cf
+-rw-r--r--  2.0 unx     1586 b- defN 24-May-25 14:15 inmanta_plugins/files/model/json.cf
+-rw-r--r--  2.0 unx    12045 b- defN 24-May-25 14:15 inmanta_plugins/files/model/systemd_unit.cf
+-rw-r--r--  2.0 unx        0 b- defN 24-May-25 14:15 inmanta_plugins/files/templates/.gitkeep
+-rw-r--r--  2.0 unx     3451 b- defN 24-May-25 14:15 inmanta_plugins/files/templates/systemd_unit.j2
+-rw-r--r--  2.0 unx      742 b- defN 24-May-25 14:15 inmanta_module_files-0.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-25 14:15 inmanta_module_files-0.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 24-May-25 14:15 inmanta_module_files-0.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1721 b- defN 24-May-25 14:15 inmanta_module_files-0.4.0.dist-info/RECORD
+19 files, 52340 bytes uncompressed, 19226 bytes compressed:  63.3%
```

## zipnote {}

```diff
@@ -39,20 +39,20 @@
 
 Filename: inmanta_plugins/files/templates/.gitkeep
 Comment: 
 
 Filename: inmanta_plugins/files/templates/systemd_unit.j2
 Comment: 
 
-Filename: inmanta_module_files-0.3.0.dist-info/METADATA
+Filename: inmanta_module_files-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: inmanta_module_files-0.3.0.dist-info/WHEEL
+Filename: inmanta_module_files-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: inmanta_module_files-0.3.0.dist-info/top_level.txt
+Filename: inmanta_module_files-0.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: inmanta_module_files-0.3.0.dist-info/RECORD
+Filename: inmanta_module_files-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## inmanta_plugins/files/setup.cfg

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = inmanta-module-files
-version = 0.3.0
+version = 0.4.0
 description = Simple module containing various types of resource to manage files.
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Guillaume Everarts de Velp
 author_email = edvgui@gmail.com
 license = ASL 2.0
 copyright = 2023 Guillaume Everarts de Velp
```

## inmanta_plugins/files/model/_init.cf

```diff
@@ -125,14 +125,19 @@
 """
 
 SystemdUnitFile.install [0:1] -- files::systemd_unit::Install
 """
 Compose the [install] section of the file
 """
 
+SystemdUnitFile.timer [0:1] -- files::systemd_unit::Timer
+"""
+Compose the [timer] section of the file
+"""
+
 index SystemdUnitFile(host, path)
 
 implement SystemdUnitFile using std::none
 
 
 entity Directory extends BaseFile:
     """
```

## inmanta_plugins/files/model/systemd_unit.cf

```diff
@@ -15,15 +15,15 @@
 
     Contact: edvgui@gmail.com
 """
 import std
 import files
 
 
-typedef service_type_t as string matching self in ["simple", "forking", "oneshot", "dbus", "notify", "idle"]
+typedef service_type_t as string matching self in ["simple", "forking", "oneshot", "dbus", "notify", "idle", "exec"]
 """
 One of the basic things that should be specified within the [Service] section is the Type= of the service.
 This categorizes services by their process and daemonizing behavior. This is important because it tells
 systemd how to correctly manage the servie and find out its state.
 
 The Type= directive can be one of the following:
 
@@ -38,15 +38,16 @@
         for the process to exit before continuing on with other units. This is the default Type= and
         ExecStart= are not set. It is used for one-off tasks.
     dbus: This indicates that unit will take a name on the D-Bus bus. When this happens, systemd will
         continue to process the next unit.
     notify: This indicates that the service will issue a notification when it has finished starting up.
         The systemd process will wait for this to happen before proceeding to other units.
     idle: This indicates that the service will not be run until all jobs are dispatched.
-
+    exec: The exec type is similar to simple, but the service manager will consider the unit started
+        immediately after the main service binary has been executed. 
 """
 
 
 entity Unit:
     """
     The first section found in most unit files is the [Unit] section. This is generally used for
     defining metadata for the unit and configuring the relationship of the unit to other units.
@@ -167,23 +168,42 @@
     """
     string[]? alias = null
     string[] wanted_by = []
     string[] required_by = []
 end
 
 
+entity Timer:
+    """
+    A unit configuration file whose name ends in ".timer" encodes information about a timer controlled and supervised by systemd,
+    for timer-based activation.
+
+    :attr on_calendar: Defines realtime (i.e. wallclock) timers with calendar event expressions. See systemd.time(7) for more
+        information on the syntax of calendar event expressions. Otherwise, the semantics are similar to OnActiveSec= and related settings.
+    :attr accuracy_sec: Specify the accuracy the timer shall elapse with. Defaults to 1min.
+    :attr randomized_delay_sec: Delay the timer by a randomly selected, evenly distributed amount of time between 0 and the specified time value.
+    :attr unit: The unit to activate when this timer elapses. The argument is a unit name, whose suffix is not ".timer".
+    """
+    string? on_calendar = null
+    string? accuracy_sec = null
+    string? randomized_delay_sec = null
+    string? unit = null
+end
+
+
 implementation file_content for files::SystemdUnitFile:
     """
     Resolve the content of the unit file, generate it from a jinja template.
     """
     # Define a variable that can be accessed in the template
     unit_file = self
 
     # Load the content based on the template
     self.content = std::template("files/systemd_unit.j2")
 end
 
 
 implement Unit using std::none
 implement Service using std::none
+implement Timer using std::none
 implement Install using std::none
 implement files::SystemdUnitFile using file_content
```

## inmanta_plugins/files/templates/systemd_unit.j2

```diff
@@ -73,14 +73,31 @@
 {%- endif %}
 {%- if unit_file.service.pid_file is not none %}
 PIDFile={{ unit_file.service.pid_file }}
 {%- endif %}
 
 {% endif -%}
 
+{% if unit_file.timer is defined -%}
+[Timer]
+{%- if unit_file.timer.on_calendar is not none %}
+OnCalendar={{ unit_file.timer.on_calendar }}
+{%- endif %}
+{%- if unit_file.timer.accuracy_sec is not none %}
+AccuracySec={{ unit_file.timer.accuracy_sec }}
+{%- endif %}
+{%- if unit_file.timer.randomized_delay_sec is not none %}
+RandomizedDelaySec={{ unit_file.timer.randomized_delay_sec }}
+{%- endif %}
+{%- if unit_file.timer.unit is not none %}
+Unit={{ unit_file.timer.unit }}
+{%- endif %}
+
+{% endif -%}
+
 {%- if unit_file.install is defined -%}
 [Install]
 {%- if unit_file.install.alias is not none %}
 Alias={{ unit_file.install.alias | join(' ') }}
 {%- endif %}
 {%- for wanted_by in unit_file.install.wanted_by %}
 WantedBy={{ wanted_by }}
```

## Comparing `inmanta_module_files-0.3.0.dist-info/METADATA` & `inmanta_module_files-0.4.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inmanta-module-files
-Version: 0.3.0
+Version: 0.4.0
 Summary: Simple module containing various types of resource to manage files.
 Author: Guillaume Everarts de Velp
 Author-email: edvgui@gmail.com
 License: ASL 2.0
 Description-Content-Type: text/markdown
 Requires-Dist: inmanta-module-std
```

## Comparing `inmanta_module_files-0.3.0.dist-info/RECORD` & `inmanta_module_files-0.4.0.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 inmanta_plugins/files/__init__.py,sha256=BUgfj_qgct0U3NELQUglCpB81sjkDRMCrHtloSL4ylM,602
 inmanta_plugins/files/base.py,sha256=nIuZ5q3mj876P6n6aeZ_ramQUHzR7NjJ4G_tsuRPKrc,2624
 inmanta_plugins/files/directory.py,sha256=pqCVFBLz_zQUHQ6e5rG43ht0njicMop-4GCXBsWYo_w,3188
 inmanta_plugins/files/host.py,sha256=c4pcP8zroNLc2RbVgOnQYlA5mdqQnP45cnS8941cMHk,6585
 inmanta_plugins/files/json.py,sha256=0RCdzY1sOGMd9j_bmTdnpmd1jhZOjjsa-JnjTWBpm94,7436
-inmanta_plugins/files/setup.cfg,sha256=k2DifyK03qLRtKYBRW7W7ODfTH3YcSzmTG8MZGf1XBI,2170
+inmanta_plugins/files/setup.cfg,sha256=2mVMvOprH47hTEPzS-iqIRtrojRvwcyrtIXE3XuV4mI,2170
 inmanta_plugins/files/systemd_unit.py,sha256=x_-yy9Bl_8O_SNViIkwtpH8ma-NZskmqlGkGBzkSoN4,2258
 inmanta_plugins/files/text.py,sha256=h6ZoDGtZYlC2yEGiLpopL96rOMKUrw-AxPULEysO8-I,2200
 inmanta_plugins/files/files/.gitkeep,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-inmanta_plugins/files/model/_init.cf,sha256=OPZT5KC2BW_Tvnk9MXLyzJY6JbhmgrigiY1nafLok_w,3856
+inmanta_plugins/files/model/_init.cf,sha256=ka-AHRapKx1uTGrUnyleHoSeXVXx5DofOFvKF-jnyXA,3963
 inmanta_plugins/files/model/host.cf,sha256=tpW8EhP9ECeZ_Q97Q7giwIrjj6HlVd9XzvchFkCS4XA,1661
 inmanta_plugins/files/model/json.cf,sha256=6Om8bihPKrZX7-hfyZLZ_rn7G-CLwf0BNvggJOdkTx8,1586
-inmanta_plugins/files/model/systemd_unit.cf,sha256=prsWy4r9ofpeQoHcszIc89usgkGl_UtC3gcRILpQ4QQ,10884
+inmanta_plugins/files/model/systemd_unit.cf,sha256=x5fyQpsdfJgSgEMjVmg51veRXftWRQ10s4rMTZk7Jnc,12045
 inmanta_plugins/files/templates/.gitkeep,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-inmanta_plugins/files/templates/systemd_unit.j2,sha256=fp-_5ggm2U_YPCGhPzKWrOigQZMbqTJ6AdhwUd7nQ9A,2950
-inmanta_module_files-0.3.0.dist-info/METADATA,sha256=i-8skP-RD48uU-pu18kR-1fB9Ukw83O3_Ihj0PYYTmk,742
-inmanta_module_files-0.3.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-inmanta_module_files-0.3.0.dist-info/top_level.txt,sha256=rb9c6eWQS8KFuSa3ktEcXpk-oSsCL9ZCVAgv7S0Eg_w,16
-inmanta_module_files-0.3.0.dist-info/RECORD,,
+inmanta_plugins/files/templates/systemd_unit.j2,sha256=FB3TwKdV1Y-eYCkc3GTVqPVjBr7pAlNgGpRzawAtUyw,3451
+inmanta_module_files-0.4.0.dist-info/METADATA,sha256=3Qkc26pUSb7rbS-tb7ylF8yZR6NBVkksbObdKAx8r3s,742
+inmanta_module_files-0.4.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+inmanta_module_files-0.4.0.dist-info/top_level.txt,sha256=rb9c6eWQS8KFuSa3ktEcXpk-oSsCL9ZCVAgv7S0Eg_w,16
+inmanta_module_files-0.4.0.dist-info/RECORD,,
```

