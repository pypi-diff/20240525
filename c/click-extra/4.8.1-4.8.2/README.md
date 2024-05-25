# Comparing `tmp/click_extra-4.8.1.tar.gz` & `tmp/click_extra-4.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "click_extra-4.8.1.tar", max compression
+gzip compressed data, was "click_extra-4.8.2.tar", max compression
```

## Comparing `click_extra-4.8.1.tar` & `click_extra-4.8.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     7446 2024-05-23 15:24:56.651185 click_extra-4.8.1/click_extra/__init__.py
--rw-r--r--   0        0        0    31127 2024-05-23 15:24:56.651185 click_extra-4.8.1/click_extra/colorize.py
--rw-r--r--   0        0        0    15819 2024-05-23 15:24:56.651185 click_extra-4.8.1/click_extra/commands.py
--rw-r--r--   0        0        0    16508 2024-05-23 15:24:56.651185 click_extra-4.8.1/click_extra/config.py
--rw-r--r--   0        0        0     4069 2024-05-23 15:24:56.655185 click_extra-4.8.1/click_extra/decorators.py
--rw-r--r--   0        0        0     6342 2024-05-23 15:24:56.655185 click_extra-4.8.1/click_extra/docs_update.py
--rw-r--r--   0        0        0    11866 2024-05-23 15:24:56.655185 click_extra-4.8.1/click_extra/logging.py
--rw-r--r--   0        0        0    27132 2024-05-23 15:24:56.655185 click_extra-4.8.1/click_extra/parameters.py
--rw-r--r--   0        0        0    17269 2024-05-23 15:24:56.655185 click_extra-4.8.1/click_extra/platforms.py
--rw-r--r--   0        0        0        0 2024-05-23 15:24:56.655185 click_extra-4.8.1/click_extra/py.typed
--rw-r--r--   0        0        0     8034 2024-05-23 15:24:56.655185 click_extra-4.8.1/click_extra/pygments.py
--rw-r--r--   0        0        0    13209 2024-05-23 15:24:56.655185 click_extra-4.8.1/click_extra/pytest.py
--rw-r--r--   0        0        0     5237 2024-05-23 15:24:56.655185 click_extra-4.8.1/click_extra/sphinx.py
--rw-r--r--   0        0        0     6340 2024-05-23 15:24:56.655185 click_extra-4.8.1/click_extra/tabulate.py
--rw-r--r--   0        0        0     2716 2024-05-23 15:24:56.655185 click_extra-4.8.1/click_extra/telemetry.py
--rw-r--r--   0        0        0    23592 2024-05-23 15:24:56.655185 click_extra-4.8.1/click_extra/testing.py
--rw-r--r--   0        0        0     2637 2024-05-23 15:24:56.655185 click_extra-4.8.1/click_extra/timer.py
--rw-r--r--   0        0        0    17760 2024-05-23 15:24:56.655185 click_extra-4.8.1/click_extra/version.py
--rw-r--r--   0        0        0    10160 2024-05-23 15:24:56.659185 click_extra-4.8.1/pyproject.toml
--rw-r--r--   0        0        0     6735 2024-05-23 15:24:56.659185 click_extra-4.8.1/readme.md
--rw-r--r--   0        0        0    10072 1970-01-01 00:00:00.000000 click_extra-4.8.1/PKG-INFO
+-rw-r--r--   0        0        0     7446 2024-05-25 07:57:52.746823 click_extra-4.8.2/click_extra/__init__.py
+-rw-r--r--   0        0        0    31127 2024-05-25 07:57:52.746823 click_extra-4.8.2/click_extra/colorize.py
+-rw-r--r--   0        0        0    15819 2024-05-25 07:57:52.750823 click_extra-4.8.2/click_extra/commands.py
+-rw-r--r--   0        0        0    16508 2024-05-25 07:57:52.750823 click_extra-4.8.2/click_extra/config.py
+-rw-r--r--   0        0        0     4069 2024-05-25 07:57:52.750823 click_extra-4.8.2/click_extra/decorators.py
+-rw-r--r--   0        0        0     6342 2024-05-25 07:57:52.750823 click_extra-4.8.2/click_extra/docs_update.py
+-rw-r--r--   0        0        0    11866 2024-05-25 07:57:52.750823 click_extra-4.8.2/click_extra/logging.py
+-rw-r--r--   0        0        0    27132 2024-05-25 07:57:52.750823 click_extra-4.8.2/click_extra/parameters.py
+-rw-r--r--   0        0        0    17269 2024-05-25 07:57:52.750823 click_extra-4.8.2/click_extra/platforms.py
+-rw-r--r--   0        0        0        0 2024-05-25 07:57:52.750823 click_extra-4.8.2/click_extra/py.typed
+-rw-r--r--   0        0        0     8034 2024-05-25 07:57:52.750823 click_extra-4.8.2/click_extra/pygments.py
+-rw-r--r--   0        0        0    13209 2024-05-25 07:57:52.750823 click_extra-4.8.2/click_extra/pytest.py
+-rw-r--r--   0        0        0     5237 2024-05-25 07:57:52.750823 click_extra-4.8.2/click_extra/sphinx.py
+-rw-r--r--   0        0        0     6340 2024-05-25 07:57:52.750823 click_extra-4.8.2/click_extra/tabulate.py
+-rw-r--r--   0        0        0     2716 2024-05-25 07:57:52.750823 click_extra-4.8.2/click_extra/telemetry.py
+-rw-r--r--   0        0        0    23592 2024-05-25 07:57:52.750823 click_extra-4.8.2/click_extra/testing.py
+-rw-r--r--   0        0        0     2637 2024-05-25 07:57:52.750823 click_extra-4.8.2/click_extra/timer.py
+-rw-r--r--   0        0        0    17546 2024-05-25 07:57:52.750823 click_extra-4.8.2/click_extra/version.py
+-rw-r--r--   0        0        0    10160 2024-05-25 07:57:52.754823 click_extra-4.8.2/pyproject.toml
+-rw-r--r--   0        0        0     6735 2024-05-25 07:57:52.754823 click_extra-4.8.2/readme.md
+-rw-r--r--   0        0        0    10072 1970-01-01 00:00:00.000000 click_extra-4.8.2/PKG-INFO
```

### Comparing `click_extra-4.8.1/click_extra/__init__.py` & `click_extra-4.8.2/click_extra/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 """Expose package-wide elements."""
 
 import sys
 
-__version__ = "4.8.1"
+__version__ = "4.8.2"
 """Examples of valid version strings according :pep:`440#version-scheme`:
 
 .. code-block:: python
 
     __version__ = "1.2.3.dev1"  # Development release 1
     __version__ = "1.2.3a1"  # Alpha Release 1
     __version__ = "1.2.3b1"  # Beta Release 1
```

### Comparing `click_extra-4.8.1/click_extra/colorize.py` & `click_extra-4.8.2/click_extra/colorize.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.8.1/click_extra/commands.py` & `click_extra-4.8.2/click_extra/commands.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.8.1/click_extra/config.py` & `click_extra-4.8.2/click_extra/config.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.8.1/click_extra/decorators.py` & `click_extra-4.8.2/click_extra/decorators.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.8.1/click_extra/docs_update.py` & `click_extra-4.8.2/click_extra/docs_update.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.8.1/click_extra/logging.py` & `click_extra-4.8.2/click_extra/logging.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.8.1/click_extra/parameters.py` & `click_extra-4.8.2/click_extra/parameters.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.8.1/click_extra/platforms.py` & `click_extra-4.8.2/click_extra/platforms.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.8.1/click_extra/pygments.py` & `click_extra-4.8.2/click_extra/pygments.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.8.1/click_extra/pytest.py` & `click_extra-4.8.2/click_extra/pytest.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.8.1/click_extra/sphinx.py` & `click_extra-4.8.2/click_extra/sphinx.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.8.1/click_extra/tabulate.py` & `click_extra-4.8.2/click_extra/tabulate.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.8.1/click_extra/telemetry.py` & `click_extra-4.8.2/click_extra/telemetry.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.8.1/click_extra/testing.py` & `click_extra-4.8.2/click_extra/testing.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.8.1/click_extra/timer.py` & `click_extra-4.8.2/click_extra/timer.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.8.1/click_extra/version.py` & `click_extra-4.8.2/click_extra/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -253,37 +253,30 @@
     @cached_property
     def package_name(self) -> str | None:
         """Returns the package name."""
         return self.module.__package__
 
     @cached_property
     def package_version(self) -> str | None:
-        """Returns the package version if installed.
+        """Returns the package version if installed."""
+        logger = logging.getLogger("click_extra")
 
-        Will raise an error if the package is not installed, or if the package version
-        cannot be determined from the package metadata.
-        """
         if not self.package_name:
+            logger.debug("Cannot guess version from package: no package name provided.")
             return None
 
         try:
             version = metadata.version(self.package_name)
         except metadata.PackageNotFoundError:
-            msg = (
-                f"{self.package_name!r} is not installed. Try passing "
-                "'package_name' instead."
+            logger.debug(
+                f"Cannot get version: {
+                    self.package_name!r
+                } package not found or not installed."
             )
-            raise RuntimeError(msg) from None
-
-        if not version:
-            msg = (
-                f"Could not determine the version for {self.package_name!r} "
-                "automatically."
-            )
-            raise RuntimeError(msg)
+            return None
 
         return version
 
     @cached_property
     def exec_name(self) -> str:
         """User-friendly name of the executed CLI.
```

### Comparing `click_extra-4.8.1/pyproject.toml` & `click_extra-4.8.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 # Docs: https://python-poetry.org/docs/pyproject/
 name = "click-extra"
-version = "4.8.1"
+version = "4.8.2"
 description = "🌈 Extra colorization and configuration loading for Click."
 license = 'GPL-2.0-or-later'
 authors = ["Kevin Deldycke <kevin@deldycke.com>"]
 readme = "readme.md"
 homepage = 'https://github.com/kdeldycke/click-extra'
 repository = 'https://github.com/kdeldycke/click-extra'
 documentation = 'https://kdeldycke.github.io/click-extra'
@@ -219,15 +219,15 @@
 # https://coverage.readthedocs.io/en/latest/config.html
 [tool.coverage.run]
 branch = true
 [tool.coverage.report]
 precision = 2
 
 [tool.bumpversion]
-current_version = "4.8.1"
+current_version = "4.8.2"
 allow_dirty = true
 
 [[tool.bumpversion.files]]
 # Update Python package version in any __init__.py file.
 glob = "./**/__init__.py"
 ignore_missing_version = true
```

### Comparing `click_extra-4.8.1/readme.md` & `click_extra-4.8.2/readme.md`

 * *Files identical despite different names*

### Comparing `click_extra-4.8.1/PKG-INFO` & `click_extra-4.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: click-extra
-Version: 4.8.1
+Version: 4.8.2
 Summary: 🌈 Extra colorization and configuration loading for Click.
 Home-page: https://github.com/kdeldycke/click-extra
 License: GPL-2.0-or-later
 Keywords: ansi-colors,cli,cloup,colorization,configuration,console,ini,json,logging,multiplatform,pygments,pytest,python,python-tabulate,sphinx,terminal,toml,xml,yaml
 Author: Kevin Deldycke
 Author-email: kevin@deldycke.com
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: click-extra Version: 4.8.1 Summary: ð Extra
+Metadata-Version: 2.1 Name: click-extra Version: 4.8.2 Summary: ð Extra
 colorization and configuration loading for Click. Home-page: https://
 github.com/kdeldycke/click-extra License: GPL-2.0-or-later Keywords: ansi-
 colors,cli,cloup,colorization,configuration,console,ini,json,logging,multiplatform,pygments,pytest,python,python-
 tabulate,sphinx,terminal,toml,xml,yaml Author: Kevin Deldycke Author-email:
 kevin@deldycke.com Requires-Python: >=3.8,<4.0 Classifier: Development Status
 :: 5 - Production/Stable Classifier: Environment :: Console Classifier:
 Environment :: Plugins Classifier: Framework :: Pytest Classifier: Framework ::
```

