# Comparing `tmp/watchgha-2.3.0.tar.gz` & `tmp/watchgha-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/ned/watchgha/dist/.tmp-ci_dahsk/watchgha-2.3.0.tar", last modified: Wed Apr 10 17:25:22 2024, max compression
+gzip compressed data, was "/Users/ned/watchgha/dist/.tmp-026l5l1a/watchgha-2.3.1.tar", last modified: Sat May 25 11:16:01 2024, max compression
```

## Comparing `watchgha-2.3.0.tar` & `watchgha-2.3.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 ned        (501) wheel        (0)        0 2024-04-10 17:25:22.000000 watchgha-2.3.0/
--rw-r--r--   0 ned        (501) wheel        (0)      515 2022-12-02 14:22:28.000000 watchgha-2.3.0/.editorconfig
--rw-r--r--   0 ned        (501) wheel        (0)    10177 2022-12-02 14:18:16.000000 watchgha-2.3.0/LICENSE.txt
--rw-r--r--   0 ned        (501) wheel        (0)       86 2023-07-02 23:07:34.000000 watchgha-2.3.0/MANIFEST.in
--rw-r--r--   0 ned        (501) wheel        (0)     3292 2024-02-03 17:53:04.000000 watchgha-2.3.0/Makefile
--rw-r--r--   0 ned        (501) wheel        (0)    12978 2024-04-10 17:25:22.000000 watchgha-2.3.0/PKG-INFO
--rw-r--r--   0 ned        (501) wheel        (0)    12030 2024-04-10 17:23:28.000000 watchgha-2.3.0/README.rst
--rw-r--r--   0 ned        (501) wheel        (0)       91 2023-06-30 21:19:24.000000 watchgha-2.3.0/dev-requirements.txt
--rw-r--r--   0 ned        (501) wheel        (0)     1443 2023-07-05 11:21:51.000000 watchgha-2.3.0/pyproject.toml
--rw-r--r--   0 ned        (501) wheel        (0)       38 2024-04-10 17:25:22.000000 watchgha-2.3.0/setup.cfg
-drwxr-xr-x   0 ned        (501) wheel        (0)        0 2024-04-10 17:25:22.000000 watchgha-2.3.0/src/
-drwxr-xr-x   0 ned        (501) wheel        (0)        0 2024-04-10 17:25:22.000000 watchgha-2.3.0/src/watchgha/
--rw-r--r--   0 ned        (501) wheel        (0)       22 2024-04-10 17:23:45.000000 watchgha-2.3.0/src/watchgha/__init__.py
--rw-r--r--   0 ned        (501) wheel        (0)      729 2023-09-07 19:35:47.000000 watchgha-2.3.0/src/watchgha/bucketer.py
--rw-r--r--   0 ned        (501) wheel        (0)     7311 2024-04-02 13:27:28.000000 watchgha-2.3.0/src/watchgha/data_core.py
--rw-r--r--   0 ned        (501) wheel        (0)     3438 2023-09-07 19:42:56.000000 watchgha-2.3.0/src/watchgha/demo.py
--rw-r--r--   0 ned        (501) wheel        (0)      620 2024-02-03 17:51:00.000000 watchgha-2.3.0/src/watchgha/git_help.py
--rw-r--r--   0 ned        (501) wheel        (0)     3338 2024-01-12 00:10:20.000000 watchgha-2.3.0/src/watchgha/http_help.py
--rw-r--r--   0 ned        (501) wheel        (0)     1109 2023-09-07 19:42:56.000000 watchgha-2.3.0/src/watchgha/utils.py
--rw-r--r--   0 ned        (501) wheel        (0)     6296 2024-04-10 17:13:14.000000 watchgha-2.3.0/src/watchgha/watch_runs.py
-drwxr-xr-x   0 ned        (501) wheel        (0)        0 2024-04-10 17:25:22.000000 watchgha-2.3.0/src/watchgha.egg-info/
--rw-r--r--   0 ned        (501) wheel        (0)    12978 2024-04-10 17:25:22.000000 watchgha-2.3.0/src/watchgha.egg-info/PKG-INFO
--rw-r--r--   0 ned        (501) wheel        (0)      518 2024-04-10 17:25:22.000000 watchgha-2.3.0/src/watchgha.egg-info/SOURCES.txt
--rw-r--r--   0 ned        (501) wheel        (0)        1 2024-04-10 17:25:22.000000 watchgha-2.3.0/src/watchgha.egg-info/dependency_links.txt
--rw-r--r--   0 ned        (501) wheel        (0)       60 2024-04-10 17:25:22.000000 watchgha-2.3.0/src/watchgha.egg-info/entry_points.txt
--rw-r--r--   0 ned        (501) wheel        (0)       53 2024-04-10 17:25:22.000000 watchgha-2.3.0/src/watchgha.egg-info/requires.txt
--rw-r--r--   0 ned        (501) wheel        (0)        9 2024-04-10 17:25:22.000000 watchgha-2.3.0/src/watchgha.egg-info/top_level.txt
--rw-r--r--   0 ned        (501) wheel        (0)   401606 2024-01-13 04:02:39.000000 watchgha-2.3.0/watch.gif
+drwxr-xr-x   0 ned        (501) wheel        (0)        0 2024-05-25 11:16:01.000000 watchgha-2.3.1/
+-rw-r--r--   0 ned        (501) wheel        (0)      515 2022-12-02 14:22:28.000000 watchgha-2.3.1/.editorconfig
+-rw-r--r--   0 ned        (501) wheel        (0)    10177 2022-12-02 14:18:16.000000 watchgha-2.3.1/LICENSE.txt
+-rw-r--r--   0 ned        (501) wheel        (0)       86 2023-07-02 23:07:34.000000 watchgha-2.3.1/MANIFEST.in
+-rw-r--r--   0 ned        (501) wheel        (0)     3292 2024-02-03 17:53:04.000000 watchgha-2.3.1/Makefile
+-rw-r--r--   0 ned        (501) wheel        (0)    13309 2024-05-25 11:16:01.000000 watchgha-2.3.1/PKG-INFO
+-rw-r--r--   0 ned        (501) wheel        (0)    12259 2024-05-25 11:11:31.000000 watchgha-2.3.1/README.rst
+-rw-r--r--   0 ned        (501) wheel        (0)       91 2023-06-30 21:19:24.000000 watchgha-2.3.1/dev-requirements.txt
+-rw-r--r--   0 ned        (501) wheel        (0)     1535 2024-05-25 11:13:05.000000 watchgha-2.3.1/pyproject.toml
+-rw-r--r--   0 ned        (501) wheel        (0)       38 2024-05-25 11:16:01.000000 watchgha-2.3.1/setup.cfg
+drwxr-xr-x   0 ned        (501) wheel        (0)        0 2024-05-25 11:16:01.000000 watchgha-2.3.1/src/
+drwxr-xr-x   0 ned        (501) wheel        (0)        0 2024-05-25 11:16:01.000000 watchgha-2.3.1/src/watchgha/
+-rw-r--r--   0 ned        (501) wheel        (0)       22 2024-05-25 11:11:38.000000 watchgha-2.3.1/src/watchgha/__init__.py
+-rw-r--r--   0 ned        (501) wheel        (0)      729 2023-09-07 19:35:47.000000 watchgha-2.3.1/src/watchgha/bucketer.py
+-rw-r--r--   0 ned        (501) wheel        (0)     7329 2024-05-24 22:33:51.000000 watchgha-2.3.1/src/watchgha/data_core.py
+-rw-r--r--   0 ned        (501) wheel        (0)     3438 2023-09-07 19:42:56.000000 watchgha-2.3.1/src/watchgha/demo.py
+-rw-r--r--   0 ned        (501) wheel        (0)      620 2024-02-03 17:51:00.000000 watchgha-2.3.1/src/watchgha/git_help.py
+-rw-r--r--   0 ned        (501) wheel        (0)     3338 2024-05-24 22:32:17.000000 watchgha-2.3.1/src/watchgha/http_help.py
+-rw-r--r--   0 ned        (501) wheel        (0)     1109 2023-09-07 19:42:56.000000 watchgha-2.3.1/src/watchgha/utils.py
+-rw-r--r--   0 ned        (501) wheel        (0)     6297 2024-05-24 22:32:27.000000 watchgha-2.3.1/src/watchgha/watch_runs.py
+drwxr-xr-x   0 ned        (501) wheel        (0)        0 2024-05-25 11:16:01.000000 watchgha-2.3.1/src/watchgha.egg-info/
+-rw-r--r--   0 ned        (501) wheel        (0)    13309 2024-05-25 11:16:01.000000 watchgha-2.3.1/src/watchgha.egg-info/PKG-INFO
+-rw-r--r--   0 ned        (501) wheel        (0)      518 2024-05-25 11:16:01.000000 watchgha-2.3.1/src/watchgha.egg-info/SOURCES.txt
+-rw-r--r--   0 ned        (501) wheel        (0)        1 2024-05-25 11:16:01.000000 watchgha-2.3.1/src/watchgha.egg-info/dependency_links.txt
+-rw-r--r--   0 ned        (501) wheel        (0)       60 2024-05-25 11:16:01.000000 watchgha-2.3.1/src/watchgha.egg-info/entry_points.txt
+-rw-r--r--   0 ned        (501) wheel        (0)       53 2024-05-25 11:16:01.000000 watchgha-2.3.1/src/watchgha.egg-info/requires.txt
+-rw-r--r--   0 ned        (501) wheel        (0)        9 2024-05-25 11:16:01.000000 watchgha-2.3.1/src/watchgha.egg-info/top_level.txt
+-rw-r--r--   0 ned        (501) wheel        (0)   401606 2024-01-13 04:02:39.000000 watchgha-2.3.1/watch.gif
```

### Comparing `watchgha-2.3.0/.editorconfig` & `watchgha-2.3.1/.editorconfig`

 * *Files identical despite different names*

### Comparing `watchgha-2.3.0/LICENSE.txt` & `watchgha-2.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `watchgha-2.3.0/Makefile` & `watchgha-2.3.1/Makefile`

 * *Files identical despite different names*

### Comparing `watchgha-2.3.0/PKG-INFO` & `watchgha-2.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchgha
-Version: 2.3.0
+Version: 2.3.1
 Summary: Watch GitHub action runs
 Author-email: Ned Batchelder <ned@nedbatchelder.com>
 License: Apache-2.0
 Project-URL: Source code, https://github.com/nedbat/watchgha
 Project-URL: Issue tracker, https://github.com/nedbat/watchgha/issues
 Project-URL: Mastodon, https://hachyderm.io/@nedbat
 Project-URL: Funding, https://github.com/sponsors/nedbat
@@ -13,14 +13,16 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
 ########################
 Watch GitHub Action runs
 ########################
@@ -199,20 +201,28 @@
 
 
 Changelog
 =========
 
 .. Release process:
     - This changelog is updated manually, not with scriv.
+    - Bump the version in src/watchgha/__init__.py
     - Comments are added manually to GitHub issues and pull requests.
     - Use `make check_release` to see if everything is ready for a release.
     - Use `make release` to release a new version.
 
 .. scriv-start-here
 
+2.3.1 – 2024-05-25
+------------------
+
+- Workflows with many jobs could be truncated.  There is still a limit of 100
+  jobs, but that is better than the earlier limit of 30.
+
+
 2.3.0 – 2024-04-10
 ------------------
 
 - GitHub Enterprise is supported via ``GITHUB_SERVER_URL`` and
   ``GITHUB_API_URL`` environment variables.
   Thanks, `Colin Marquardt <pull 21_>`_.
```

### Comparing `watchgha-2.3.0/README.rst` & `watchgha-2.3.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -176,20 +176,28 @@
 
 
 Changelog
 =========
 
 .. Release process:
     - This changelog is updated manually, not with scriv.
+    - Bump the version in src/watchgha/__init__.py
     - Comments are added manually to GitHub issues and pull requests.
     - Use `make check_release` to see if everything is ready for a release.
     - Use `make release` to release a new version.
 
 .. scriv-start-here
 
+2.3.1 – 2024-05-25
+------------------
+
+- Workflows with many jobs could be truncated.  There is still a limit of 100
+  jobs, but that is better than the earlier limit of 30.
+
+
 2.3.0 – 2024-04-10
 ------------------
 
 - GitHub Enterprise is supported via ``GITHUB_SERVER_URL`` and
   ``GITHUB_API_URL`` environment variables.
   Thanks, `Colin Marquardt <pull 21_>`_.
```

### Comparing `watchgha-2.3.0/pyproject.toml` & `watchgha-2.3.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,16 @@
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
+    "Programming Language :: Python :: 3.13",
 ]
 
 requires-python = ">= 3.7"
 
 dependencies = [
     "click",
     "dulwich",
```

### Comparing `watchgha-2.3.0/src/watchgha/bucketer.py` & `watchgha-2.3.1/src/watchgha/bucketer.py`

 * *Files identical despite different names*

### Comparing `watchgha-2.3.0/src/watchgha/data_core.py` & `watchgha-2.3.1/src/watchgha/data_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,15 +147,15 @@
                 if not event_runs:
                     continue
 
             events.append(event_runs)
             run_names_seen.update(these_runs_names)
 
             async def load_run(run):
-                run["jobs"] = json.loads(await datafn(run["jobs_url"]))["jobs"]
+                run["jobs"] = json.loads(await datafn(run["jobs_url"] + "?per_page=100"))["jobs"]
 
             for run in event_runs:
                 summary, _, _ = summary_style_icon(run)
                 if summary != "success":
                     nursery.start_soon(load_run, run)
 
     return events
```

### Comparing `watchgha-2.3.0/src/watchgha/demo.py` & `watchgha-2.3.1/src/watchgha/demo.py`

 * *Files identical despite different names*

### Comparing `watchgha-2.3.0/src/watchgha/git_help.py` & `watchgha-2.3.1/src/watchgha/git_help.py`

 * *Files identical despite different names*

### Comparing `watchgha-2.3.0/src/watchgha/http_help.py` & `watchgha-2.3.1/src/watchgha/http_help.py`

 * *Files identical despite different names*

### Comparing `watchgha-2.3.0/src/watchgha/utils.py` & `watchgha-2.3.1/src/watchgha/utils.py`

 * *Files identical despite different names*

### Comparing `watchgha-2.3.0/src/watchgha/watch_runs.py` & `watchgha-2.3.1/src/watchgha/watch_runs.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
     elif ":" in repo:
         repo_urls = [repo]
         if branch is None:
             fatal(f"Branch is required for URL repo")
     else:
         fatal(f"Don't understand repo {repo!r}")
 
-    params = {"per_page": "40"}
+    params = {"per_page": "100"}
     if sha:
         params["head_sha"] = sha
     else:
         assert branch is not None
         params["branch"] = branch
     url_args = urllib.parse.urlencode(params)
```

### Comparing `watchgha-2.3.0/src/watchgha.egg-info/PKG-INFO` & `watchgha-2.3.1/src/watchgha.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchgha
-Version: 2.3.0
+Version: 2.3.1
 Summary: Watch GitHub action runs
 Author-email: Ned Batchelder <ned@nedbatchelder.com>
 License: Apache-2.0
 Project-URL: Source code, https://github.com/nedbat/watchgha
 Project-URL: Issue tracker, https://github.com/nedbat/watchgha/issues
 Project-URL: Mastodon, https://hachyderm.io/@nedbat
 Project-URL: Funding, https://github.com/sponsors/nedbat
@@ -13,14 +13,16 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
 ########################
 Watch GitHub Action runs
 ########################
@@ -199,20 +201,28 @@
 
 
 Changelog
 =========
 
 .. Release process:
     - This changelog is updated manually, not with scriv.
+    - Bump the version in src/watchgha/__init__.py
     - Comments are added manually to GitHub issues and pull requests.
     - Use `make check_release` to see if everything is ready for a release.
     - Use `make release` to release a new version.
 
 .. scriv-start-here
 
+2.3.1 – 2024-05-25
+------------------
+
+- Workflows with many jobs could be truncated.  There is still a limit of 100
+  jobs, but that is better than the earlier limit of 30.
+
+
 2.3.0 – 2024-04-10
 ------------------
 
 - GitHub Enterprise is supported via ``GITHUB_SERVER_URL`` and
   ``GITHUB_API_URL`` environment variables.
   Thanks, `Colin Marquardt <pull 21_>`_.
```

### Comparing `watchgha-2.3.0/src/watchgha.egg-info/SOURCES.txt` & `watchgha-2.3.1/src/watchgha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `watchgha-2.3.0/watch.gif` & `watchgha-2.3.1/watch.gif`

 * *Files identical despite different names*

