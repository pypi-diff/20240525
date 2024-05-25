# Comparing `tmp/aioswitcher-3.4.2.tar.gz` & `tmp/aioswitcher-3.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioswitcher-3.4.2.tar", max compression
+gzip compressed data, was "aioswitcher-3.4.3.tar", max compression
```

## Comparing `aioswitcher-3.4.2.tar` & `aioswitcher-3.4.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2024-01-18 13:52:23.343084 aioswitcher-3.4.2/LICENSE
--rw-r--r--   0        0        0    11500 2024-01-18 13:52:23.343084 aioswitcher-3.4.2/README.md
--rw-r--r--   0        0        0        0 2024-01-18 13:52:23.343084 aioswitcher-3.4.2/py.typed
--rw-r--r--   0        0        0     3177 2024-01-18 13:52:41.619359 aioswitcher-3.4.2/pyproject.toml
--rwxr-xr-x   0        0        0      818 2024-01-18 13:52:23.347084 aioswitcher-3.4.2/src/aioswitcher/__init__.py
--rw-r--r--   0        0        0    28127 2024-01-18 13:52:23.347084 aioswitcher-3.4.2/src/aioswitcher/api/__init__.py
--rw-r--r--   0        0        0     9461 2024-01-18 13:52:23.347084 aioswitcher-3.4.2/src/aioswitcher/api/messages.py
--rw-r--r--   0        0        0     3924 2024-01-18 13:52:23.347084 aioswitcher-3.4.2/src/aioswitcher/api/packets.py
--rw-r--r--   0        0        0    15903 2024-01-18 13:52:23.347084 aioswitcher-3.4.2/src/aioswitcher/api/remotes.py
--rw-r--r--   0        0        0    16542 2024-01-18 13:52:23.347084 aioswitcher-3.4.2/src/aioswitcher/bridge.py
--rw-r--r--   0        0        0    11532 2024-01-18 13:52:23.347084 aioswitcher-3.4.2/src/aioswitcher/device/__init__.py
--rw-r--r--   0        0        0     4320 2024-01-18 13:52:23.347084 aioswitcher-3.4.2/src/aioswitcher/device/tools.py
--rw-r--r--   0        0        0 12947433 2024-01-18 13:52:23.375084 aioswitcher-3.4.2/src/aioswitcher/resources/irset_db.json
--rw-r--r--   0        0        0     2054 2024-01-18 13:52:23.375084 aioswitcher-3.4.2/src/aioswitcher/schedule/__init__.py
--rw-r--r--   0        0        0     4047 2024-01-18 13:52:23.375084 aioswitcher-3.4.2/src/aioswitcher/schedule/parser.py
--rw-r--r--   0        0        0     5683 2024-01-18 13:52:23.375084 aioswitcher-3.4.2/src/aioswitcher/schedule/tools.py
--rw-r--r--   0        0        0    12469 1970-01-01 00:00:00.000000 aioswitcher-3.4.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-25 14:39:44.047171 aioswitcher-3.4.3/LICENSE
+-rw-r--r--   0        0        0    11877 2024-05-25 14:39:44.047171 aioswitcher-3.4.3/README.md
+-rw-r--r--   0        0        0     3166 2024-05-25 14:40:08.403043 aioswitcher-3.4.3/pyproject.toml
+-rwxr-xr-x   0        0        0      818 2024-05-25 14:39:44.047171 aioswitcher-3.4.3/src/aioswitcher/__init__.py
+-rw-r--r--   0        0        0    28127 2024-05-25 14:39:44.047171 aioswitcher-3.4.3/src/aioswitcher/api/__init__.py
+-rw-r--r--   0        0        0     9461 2024-05-25 14:39:44.047171 aioswitcher-3.4.3/src/aioswitcher/api/messages.py
+-rw-r--r--   0        0        0     3924 2024-05-25 14:39:44.047171 aioswitcher-3.4.3/src/aioswitcher/api/packets.py
+-rw-r--r--   0        0        0    15903 2024-05-25 14:39:44.047171 aioswitcher-3.4.3/src/aioswitcher/api/remotes.py
+-rw-r--r--   0        0        0    16542 2024-05-25 14:39:44.047171 aioswitcher-3.4.3/src/aioswitcher/bridge.py
+-rw-r--r--   0        0        0    11532 2024-05-25 14:39:44.047171 aioswitcher-3.4.3/src/aioswitcher/device/__init__.py
+-rw-r--r--   0        0        0     4320 2024-05-25 14:39:44.047171 aioswitcher-3.4.3/src/aioswitcher/device/tools.py
+-rw-r--r--   0        0        0        0 2024-05-25 14:39:44.047171 aioswitcher-3.4.3/src/aioswitcher/py.typed
+-rw-r--r--   0        0        0 12947433 2024-05-25 14:39:44.075171 aioswitcher-3.4.3/src/aioswitcher/resources/irset_db.json
+-rw-r--r--   0        0        0     2054 2024-05-25 14:39:44.075171 aioswitcher-3.4.3/src/aioswitcher/schedule/__init__.py
+-rw-r--r--   0        0        0     4047 2024-05-25 14:39:44.075171 aioswitcher-3.4.3/src/aioswitcher/schedule/parser.py
+-rw-r--r--   0        0        0     5666 2024-05-25 14:39:44.075171 aioswitcher-3.4.3/src/aioswitcher/schedule/tools.py
+-rw-r--r--   0        0        0    12846 1970-01-01 00:00:00.000000 aioswitcher-3.4.3/PKG-INFO
```

### Comparing `aioswitcher-3.4.2/LICENSE` & `aioswitcher-3.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aioswitcher-3.4.2/README.md` & `aioswitcher-3.4.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,31 @@
-# Help Wanted
-
-<p align="left">
-<strong>
-Aioswitcher project is looking for maintainers and contributors!<br/>
-For various reasons, I can only keep maintaining this project as far as dependency bumps and publishing.<br/>
-As for new features and the occasional bug support, these will require other maintainers/contributors.<br/>
-<br/>
-If that's you - please feel free to ping me and I will do all I can to make the onboarding process easy.
-</strong>
-</p>
+Metadata-Version: 2.1
+Name: aioswitcher
+Version: 3.4.3
+Summary: Switcher Python Integration.
+Home-page: https://pypi.org/project/aioswitcher/
+License: Apache-2.0
+Keywords: home,automation,switcher,smart
+Author: Tomer Figenblat
+Author-email: tomer@tomfi.info
+Maintainer: Shay Levy
+Requires-Python: >=3.9.0,<4.0.0
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Home Automation
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Typing :: Typed
+Project-URL: Documentation, https://aioswitcher.tomfi.info
+Project-URL: Repository, https://github.com/tomerfi/aioswitcher
+Description-Content-Type: text/markdown
 
 # Switcher Python Integration</br>[![pypi-version]][11] [![pypi-downloads]][11] [![license-badge]][4]
 
 [![gh-build-status]][7] [![gh-pages-status]][8] [![codecov]][3]
 
 PyPi module integrating with various [Switcher][12] devices.</br>
 Check out the [wiki pages][0] for a list of supported devices.
@@ -170,20 +183,22 @@
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/aviadgolan"><img src="https://avatars.githubusercontent.com/u/17742111?v=4?s=100" width="100px;" alt="Aviad Golan"/><br /><sub><b>Aviad Golan</b></sub></a><br /><a href="#data-AviadGolan" title="Data">🔣</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/dolby360"><img src="https://avatars.githubusercontent.com/u/22151399?v=4?s=100" width="100px;" alt="Dolev Ben Aharon"/><br /><sub><b>Dolev Ben Aharon</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=dolby360" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://fabian-affolter.ch/blog/"><img src="https://avatars.githubusercontent.com/u/116184?v=4?s=100" width="100px;" alt="Fabian Affolter"/><br /><sub><b>Fabian Affolter</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=fabaff" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/oranja"><img src="https://avatars.githubusercontent.com/u/679184?v=4?s=100" width="100px;" alt="Itzik Ephraim"/><br /><sub><b>Itzik Ephraim</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=oranja" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Kesav890"><img src="https://avatars.githubusercontent.com/u/82559951?v=4?s=100" width="100px;" alt="Kesav890"/><br /><sub><b>Kesav890</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=Kesav890" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://liad.avrah.am"><img src="https://avatars.githubusercontent.com/u/7263223?v=4?s=100" width="100px;" alt="Liad Avraham"/><br /><sub><b>Liad Avraham</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=liadav" title="Code">💻</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/OrBin"><img src="https://avatars.githubusercontent.com/u/6897234?v=4?s=100" width="100px;" alt="Or Bin"/><br /><sub><b>Or Bin</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=OrBin" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/cdce8p"><img src="https://avatars.githubusercontent.com/u/30130371?v=4?s=100" width="100px;" alt="Marc Mueller"/><br /><sub><b>Marc Mueller</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=cdce8p" title="Code">💻</a></td>
     </tr>
     <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/OrBin"><img src="https://avatars.githubusercontent.com/u/6897234?v=4?s=100" width="100px;" alt="Or Bin"/><br /><sub><b>Or Bin</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=OrBin" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://exploit.co.il"><img src="https://avatars.githubusercontent.com/u/1768915?v=4?s=100" width="100px;" alt="Shai rod"/><br /><sub><b>Shai rod</b></sub></a><br /><a href="#data-nightrang3r" title="Data">🔣</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/thecode"><img src="https://avatars.githubusercontent.com/u/1858925?v=4?s=100" width="100px;" alt="Shay Levy"/><br /><sub><b>Shay Levy</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=thecode" title="Code">💻</a> <a href="#ideas-thecode" title="Ideas, Planning, & Feedback">🤔</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/thecode"><img src="https://avatars.githubusercontent.com/u/1858925?v=4?s=100" width="100px;" alt="Shay Levy"/><br /><sub><b>Shay Levy</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=thecode" title="Code">💻</a> <a href="#ideas-thecode" title="Ideas, Planning, & Feedback">🤔</a> <a href="#maintenance-thecode" title="Maintenance">🚧</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/YogevBokobza"><img src="https://avatars.githubusercontent.com/u/22839127?v=4?s=100" width="100px;" alt="YogevBokobza"/><br /><sub><b>YogevBokobza</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=YogevBokobza" title="Code">💻</a> <a href="https://github.com/TomerFi/aioswitcher/commits?author=YogevBokobza" title="Tests">⚠️</a> <a href="#maintenance-YogevBokobza" title="Maintenance">🚧</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/gmyuval"><img src="https://avatars.githubusercontent.com/u/28506179?v=4?s=100" width="100px;" alt="Yuval Moran"/><br /><sub><b>Yuval Moran</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=gmyuval" title="Code">💻</a> <a href="https://github.com/TomerFi/aioswitcher/commits?author=gmyuval" title="Tests">⚠️</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/dmatik"><img src="https://avatars.githubusercontent.com/u/5577386?v=4?s=100" width="100px;" alt="dmatik"/><br /><sub><b>dmatik</b></sub></a><br /><a href="#blog-dmatik" title="Blogposts">📝</a> <a href="#ideas-dmatik" title="Ideas, Planning, & Feedback">🤔</a> <a href="#userTesting-dmatik" title="User Testing">📓</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/jafar-atili"><img src="https://avatars.githubusercontent.com/u/19508787?v=4?s=100" width="100px;" alt="jafar-atili"/><br /><sub><b>jafar-atili</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=jafar-atili" title="Code">💻</a> <a href="https://github.com/TomerFi/aioswitcher/commits?author=jafar-atili" title="Documentation">📖</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
@@ -205,7 +220,8 @@
 [all-contributors]: https://img.shields.io/github/all-contributors/tomerfi/aioswitcher?color=ee8449&style=flat-square
 [codecov]: https://codecov.io/gh/TomerFi/aioswitcher/graph/badge.svg
 [gh-build-status]: https://github.com/TomerFi/aioswitcher/actions/workflows/stage.yml/badge.svg
 [gh-pages-status]: https://github.com/TomerFi/aioswitcher/actions/workflows/pages.yml/badge.svg
 [license-badge]: https://img.shields.io/github/license/tomerfi/aioswitcher
 [pypi-downloads]: https://img.shields.io/pypi/dm/aioswitcher.svg?logo=pypi&color=1082C2
 [pypi-version]: https://img.shields.io/pypi/v/aioswitcher?logo=pypi
+
```

### Comparing `aioswitcher-3.4.2/pyproject.toml` & `aioswitcher-3.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aioswitcher"
-version = "3.4.2"
+version = "3.4.3"
 description = "Switcher Python Integration."
 license = "Apache-2.0"
 authors = [ "Tomer Figenblat <tomer@tomfi.info>" ]
 maintainers = [ "Shay Levy" ]
 readme = "README.md"
 homepage = "https://pypi.org/project/aioswitcher/"
 repository = "https://github.com/tomerfi/aioswitcher"
@@ -13,23 +13,23 @@
 classifiers = [
   "Intended Audience :: Developers",
   "Operating System :: OS Independent",
   "Topic :: Home Automation",
   "Topic :: Software Development :: Libraries :: Python Modules",
   "Typing :: Typed"
 ]
-include = [ "py.typed" ]
+include = [ ]
 exclude = [ ]
 
   [tool.poetry.dependencies]
   python = "^3.9.0"
 
 [tool.poetry.group.dev.dependencies]
 assertpy = "^1.1"
-black = ">=22.8,<24.0"
+black = ">=22.8,<25.0"
 flake8 = ">=5.0.4,<7.0.0"
 flake8-docstrings = "^1.6.0"
 Flake8-pyproject = "^1.1.0.post0"
 isort = "^5.10.1"
 mypy = ">=0.971,<1.5"
 poethepoet = ">=0.16.1,<0.22.0"
 pytest = "^7.1.2"
```

### Comparing `aioswitcher-3.4.2/src/aioswitcher/__init__.py` & `aioswitcher-3.4.3/src/aioswitcher/__init__.py`

 * *Files identical despite different names*

### Comparing `aioswitcher-3.4.2/src/aioswitcher/api/__init__.py` & `aioswitcher-3.4.3/src/aioswitcher/api/__init__.py`

 * *Files identical despite different names*

### Comparing `aioswitcher-3.4.2/src/aioswitcher/api/messages.py` & `aioswitcher-3.4.3/src/aioswitcher/api/messages.py`

 * *Files identical despite different names*

### Comparing `aioswitcher-3.4.2/src/aioswitcher/api/packets.py` & `aioswitcher-3.4.3/src/aioswitcher/api/packets.py`

 * *Files identical despite different names*

### Comparing `aioswitcher-3.4.2/src/aioswitcher/api/remotes.py` & `aioswitcher-3.4.3/src/aioswitcher/api/remotes.py`

 * *Files identical despite different names*

### Comparing `aioswitcher-3.4.2/src/aioswitcher/bridge.py` & `aioswitcher-3.4.3/src/aioswitcher/bridge.py`

 * *Files identical despite different names*

### Comparing `aioswitcher-3.4.2/src/aioswitcher/device/__init__.py` & `aioswitcher-3.4.3/src/aioswitcher/device/__init__.py`

 * *Files identical despite different names*

### Comparing `aioswitcher-3.4.2/src/aioswitcher/device/tools.py` & `aioswitcher-3.4.3/src/aioswitcher/device/tools.py`

 * *Files identical despite different names*

### Comparing `aioswitcher-3.4.2/src/aioswitcher/resources/irset_db.json` & `aioswitcher-3.4.3/src/aioswitcher/resources/irset_db.json`

 * *Files identical despite different names*

### Comparing `aioswitcher-3.4.2/src/aioswitcher/schedule/__init__.py` & `aioswitcher-3.4.3/src/aioswitcher/schedule/__init__.py`

 * *Files identical despite different names*

### Comparing `aioswitcher-3.4.2/src/aioswitcher/schedule/parser.py` & `aioswitcher-3.4.3/src/aioswitcher/schedule/parser.py`

 * *Files identical despite different names*

### Comparing `aioswitcher-3.4.2/src/aioswitcher/schedule/tools.py` & `aioswitcher-3.4.3/src/aioswitcher/schedule/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Switcher integration schedule module tools."""
 
 import time
 from binascii import hexlify
-from datetime import datetime
+from datetime import datetime, timedelta
 from struct import pack
 from typing import Set, Union
 
 from . import Days
 
 
 def pretty_next_run(start_time: str, days: Set[Days] = set()) -> str:
@@ -69,17 +69,17 @@
     return f"Due next {weekdays[next_exc_day].value} at {start_time}"
 
 
 def calc_duration(start_time: str, end_time: str) -> str:
     """Use to calculate the delta between two time values formated as %H:%M."""
     start_datetime = datetime.strptime(start_time, "%H:%M")
     end_datetime = datetime.strptime(end_time, "%H:%M")
-    if end_datetime > start_datetime:
-        return str(end_datetime - start_datetime)
-    raise ValueError("end_time should be greater the start_time")
+    if end_datetime < start_datetime:
+        end_datetime += timedelta(days=1)
+    return str(end_datetime - start_datetime)
 
 
 def bit_summary_to_days(sum_weekdays_bit: int) -> Set[Days]:
     """Decode a weekdays bit summary to a set of weekdays.
 
     Args:
         sum_weekdays_bit: the sum of all weekdays
```

### Comparing `aioswitcher-3.4.2/PKG-INFO` & `aioswitcher-3.4.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,7 @@
-Metadata-Version: 2.1
-Name: aioswitcher
-Version: 3.4.2
-Summary: Switcher Python Integration.
-Home-page: https://pypi.org/project/aioswitcher/
-License: Apache-2.0
-Keywords: home,automation,switcher,smart
-Author: Tomer Figenblat
-Author-email: tomer@tomfi.info
-Maintainer: Shay Levy
-Requires-Python: >=3.9.0,<4.0.0
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Home Automation
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Typing :: Typed
-Project-URL: Documentation, https://aioswitcher.tomfi.info
-Project-URL: Repository, https://github.com/tomerfi/aioswitcher
-Description-Content-Type: text/markdown
-
-# Help Wanted
-
-<p align="left">
-<strong>
-Aioswitcher project is looking for maintainers and contributors!<br/>
-For various reasons, I can only keep maintaining this project as far as dependency bumps and publishing.<br/>
-As for new features and the occasional bug support, these will require other maintainers/contributors.<br/>
-<br/>
-If that's you - please feel free to ping me and I will do all I can to make the onboarding process easy.
-</strong>
-</p>
-
 # Switcher Python Integration</br>[![pypi-version]][11] [![pypi-downloads]][11] [![license-badge]][4]
 
 [![gh-build-status]][7] [![gh-pages-status]][8] [![codecov]][3]
 
 PyPi module integrating with various [Switcher][12] devices.</br>
 Check out the [wiki pages][0] for a list of supported devices.
 
@@ -195,20 +158,22 @@
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/aviadgolan"><img src="https://avatars.githubusercontent.com/u/17742111?v=4?s=100" width="100px;" alt="Aviad Golan"/><br /><sub><b>Aviad Golan</b></sub></a><br /><a href="#data-AviadGolan" title="Data">🔣</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/dolby360"><img src="https://avatars.githubusercontent.com/u/22151399?v=4?s=100" width="100px;" alt="Dolev Ben Aharon"/><br /><sub><b>Dolev Ben Aharon</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=dolby360" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://fabian-affolter.ch/blog/"><img src="https://avatars.githubusercontent.com/u/116184?v=4?s=100" width="100px;" alt="Fabian Affolter"/><br /><sub><b>Fabian Affolter</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=fabaff" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/oranja"><img src="https://avatars.githubusercontent.com/u/679184?v=4?s=100" width="100px;" alt="Itzik Ephraim"/><br /><sub><b>Itzik Ephraim</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=oranja" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Kesav890"><img src="https://avatars.githubusercontent.com/u/82559951?v=4?s=100" width="100px;" alt="Kesav890"/><br /><sub><b>Kesav890</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=Kesav890" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://liad.avrah.am"><img src="https://avatars.githubusercontent.com/u/7263223?v=4?s=100" width="100px;" alt="Liad Avraham"/><br /><sub><b>Liad Avraham</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=liadav" title="Code">💻</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/OrBin"><img src="https://avatars.githubusercontent.com/u/6897234?v=4?s=100" width="100px;" alt="Or Bin"/><br /><sub><b>Or Bin</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=OrBin" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/cdce8p"><img src="https://avatars.githubusercontent.com/u/30130371?v=4?s=100" width="100px;" alt="Marc Mueller"/><br /><sub><b>Marc Mueller</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=cdce8p" title="Code">💻</a></td>
     </tr>
     <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/OrBin"><img src="https://avatars.githubusercontent.com/u/6897234?v=4?s=100" width="100px;" alt="Or Bin"/><br /><sub><b>Or Bin</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=OrBin" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://exploit.co.il"><img src="https://avatars.githubusercontent.com/u/1768915?v=4?s=100" width="100px;" alt="Shai rod"/><br /><sub><b>Shai rod</b></sub></a><br /><a href="#data-nightrang3r" title="Data">🔣</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/thecode"><img src="https://avatars.githubusercontent.com/u/1858925?v=4?s=100" width="100px;" alt="Shay Levy"/><br /><sub><b>Shay Levy</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=thecode" title="Code">💻</a> <a href="#ideas-thecode" title="Ideas, Planning, & Feedback">🤔</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/thecode"><img src="https://avatars.githubusercontent.com/u/1858925?v=4?s=100" width="100px;" alt="Shay Levy"/><br /><sub><b>Shay Levy</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=thecode" title="Code">💻</a> <a href="#ideas-thecode" title="Ideas, Planning, & Feedback">🤔</a> <a href="#maintenance-thecode" title="Maintenance">🚧</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/YogevBokobza"><img src="https://avatars.githubusercontent.com/u/22839127?v=4?s=100" width="100px;" alt="YogevBokobza"/><br /><sub><b>YogevBokobza</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=YogevBokobza" title="Code">💻</a> <a href="https://github.com/TomerFi/aioswitcher/commits?author=YogevBokobza" title="Tests">⚠️</a> <a href="#maintenance-YogevBokobza" title="Maintenance">🚧</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/gmyuval"><img src="https://avatars.githubusercontent.com/u/28506179?v=4?s=100" width="100px;" alt="Yuval Moran"/><br /><sub><b>Yuval Moran</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=gmyuval" title="Code">💻</a> <a href="https://github.com/TomerFi/aioswitcher/commits?author=gmyuval" title="Tests">⚠️</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/dmatik"><img src="https://avatars.githubusercontent.com/u/5577386?v=4?s=100" width="100px;" alt="dmatik"/><br /><sub><b>dmatik</b></sub></a><br /><a href="#blog-dmatik" title="Blogposts">📝</a> <a href="#ideas-dmatik" title="Ideas, Planning, & Feedback">🤔</a> <a href="#userTesting-dmatik" title="User Testing">📓</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/jafar-atili"><img src="https://avatars.githubusercontent.com/u/19508787?v=4?s=100" width="100px;" alt="jafar-atili"/><br /><sub><b>jafar-atili</b></sub></a><br /><a href="https://github.com/TomerFi/aioswitcher/commits?author=jafar-atili" title="Code">💻</a> <a href="https://github.com/TomerFi/aioswitcher/commits?author=jafar-atili" title="Documentation">📖</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
@@ -230,8 +195,7 @@
 [all-contributors]: https://img.shields.io/github/all-contributors/tomerfi/aioswitcher?color=ee8449&style=flat-square
 [codecov]: https://codecov.io/gh/TomerFi/aioswitcher/graph/badge.svg
 [gh-build-status]: https://github.com/TomerFi/aioswitcher/actions/workflows/stage.yml/badge.svg
 [gh-pages-status]: https://github.com/TomerFi/aioswitcher/actions/workflows/pages.yml/badge.svg
 [license-badge]: https://img.shields.io/github/license/tomerfi/aioswitcher
 [pypi-downloads]: https://img.shields.io/pypi/dm/aioswitcher.svg?logo=pypi&color=1082C2
 [pypi-version]: https://img.shields.io/pypi/v/aioswitcher?logo=pypi
-
```

