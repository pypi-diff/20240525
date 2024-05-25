# Comparing `tmp/d2cd-0.0.1a0.tar.gz` & `tmp/d2cd-0.0.3b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "d2cd-0.0.1a0.tar", last modified: Wed May  8 15:01:22 2024, max compression
+gzip compressed data, was "d2cd-0.0.3b0.tar", last modified: Sat May 25 19:46:05 2024, max compression
```

## Comparing `d2cd-0.0.1a0.tar` & `d2cd-0.0.3b0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 veerendra.kakumanu   (501) staff       (20)        0 2024-05-08 15:01:22.476503 d2cd-0.0.1a0/
--rw-r--r--   0 veerendra.kakumanu   (501) staff       (20)       75 2024-05-08 15:00:12.000000 d2cd-0.0.1a0/MANIFEST.in
--rw-r--r--   0 veerendra.kakumanu   (501) staff       (20)     3658 2024-05-08 15:01:22.476299 d2cd-0.0.1a0/PKG-INFO
--rw-r--r--   0 veerendra.kakumanu   (501) staff       (20)     2225 2024-05-08 15:00:12.000000 d2cd-0.0.1a0/README.md
-drwxr-xr-x   0 veerendra.kakumanu   (501) staff       (20)        0 2024-05-08 15:01:22.474050 d2cd-0.0.1a0/d2cd/
--rw-r--r--   0 veerendra.kakumanu   (501) staff       (20)       71 2024-05-08 15:00:12.000000 d2cd-0.0.1a0/d2cd/__init__.py
--rw-r--r--   0 veerendra.kakumanu   (501) staff       (20)      521 2024-05-08 15:00:12.000000 d2cd-0.0.1a0/d2cd/banner.py
--rw-r--r--   0 veerendra.kakumanu   (501) staff       (20)      939 2024-05-08 15:00:12.000000 d2cd-0.0.1a0/d2cd/cli.py
--rw-r--r--   0 veerendra.kakumanu   (501) staff       (20)     2135 2024-05-08 15:00:12.000000 d2cd-0.0.1a0/d2cd/config_loader.py
--rwxr-xr-x   0 veerendra.kakumanu   (501) staff       (20)     1475 2024-05-08 15:00:12.000000 d2cd-0.0.1a0/d2cd/main.py
-drwxr-xr-x   0 veerendra.kakumanu   (501) staff       (20)        0 2024-05-08 15:01:22.475593 d2cd-0.0.1a0/d2cd/utils/
--rw-r--r--   0 veerendra.kakumanu   (501) staff       (20)       43 2024-05-08 15:00:12.000000 d2cd-0.0.1a0/d2cd/utils/__init__.py
--rw-r--r--   0 veerendra.kakumanu   (501) staff       (20)     1293 2024-05-08 15:00:12.000000 d2cd-0.0.1a0/d2cd/utils/docker_compose_utils.py
--rw-r--r--   0 veerendra.kakumanu   (501) staff       (20)       77 2024-05-08 15:00:12.000000 d2cd-0.0.1a0/d2cd/utils/errors.py
--rw-r--r--   0 veerendra.kakumanu   (501) staff       (20)     2683 2024-05-08 15:00:12.000000 d2cd-0.0.1a0/d2cd/utils/git_utils.py
--rw-r--r--   0 veerendra.kakumanu   (501) staff       (20)       88 2024-05-08 15:00:12.000000 d2cd-0.0.1a0/d2cd/utils/logger.py
-drwxr-xr-x   0 veerendra.kakumanu   (501) staff       (20)        0 2024-05-08 15:01:22.476071 d2cd-0.0.1a0/d2cd.egg-info/
--rw-r--r--   0 veerendra.kakumanu   (501) staff       (20)     3658 2024-05-08 15:01:22.000000 d2cd-0.0.1a0/d2cd.egg-info/PKG-INFO
--rw-r--r--   0 veerendra.kakumanu   (501) staff       (20)      477 2024-05-08 15:01:22.000000 d2cd-0.0.1a0/d2cd.egg-info/SOURCES.txt
--rw-r--r--   0 veerendra.kakumanu   (501) staff       (20)        1 2024-05-08 15:01:22.000000 d2cd-0.0.1a0/d2cd.egg-info/dependency_links.txt
--rw-r--r--   0 veerendra.kakumanu   (501) staff       (20)       40 2024-05-08 15:01:22.000000 d2cd-0.0.1a0/d2cd.egg-info/entry_points.txt
--rw-r--r--   0 veerendra.kakumanu   (501) staff       (20)      114 2024-05-08 15:01:22.000000 d2cd-0.0.1a0/d2cd.egg-info/requires.txt
--rw-r--r--   0 veerendra.kakumanu   (501) staff       (20)        5 2024-05-08 15:01:22.000000 d2cd-0.0.1a0/d2cd.egg-info/top_level.txt
--rw-r--r--   0 veerendra.kakumanu   (501) staff       (20)      735 2024-05-08 15:00:12.000000 d2cd-0.0.1a0/pyproject.toml
--rw-r--r--   0 veerendra.kakumanu   (501) staff       (20)       38 2024-05-08 15:01:22.476549 d2cd-0.0.1a0/setup.cfg
--rwxr-xr-x   0 veerendra.kakumanu   (501) staff       (20)     2066 2024-05-08 15:00:12.000000 d2cd-0.0.1a0/setup.py
-drwxr-xr-x   0 veerendra.kakumanu   (501) staff       (20)        0 2024-05-08 15:01:22.475866 d2cd-0.0.1a0/tests/
--rw-r--r--   0 veerendra.kakumanu   (501) staff       (20)     2581 2024-05-08 15:00:12.000000 d2cd-0.0.1a0/tests/test_docker_compose_utils.py
--rw-r--r--   0 veerendra.kakumanu   (501) staff       (20)     1910 2024-05-08 15:00:12.000000 d2cd-0.0.1a0/tests/test_git_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:46:05.539167 d2cd-0.0.3b0/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-25 19:45:51.000000 d2cd-0.0.3b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-05-25 19:46:05.535167 d2cd-0.0.3b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-25 19:45:51.000000 d2cd-0.0.3b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:46:05.531167 d2cd-0.0.3b0/d2cd/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-25 19:45:51.000000 d2cd-0.0.3b0/d2cd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-25 19:45:51.000000 d2cd-0.0.3b0/d2cd/banner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-25 19:45:51.000000 d2cd-0.0.3b0/d2cd/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-05-25 19:45:51.000000 d2cd-0.0.3b0/d2cd/config_loader.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1855 2024-05-25 19:45:51.000000 d2cd-0.0.3b0/d2cd/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:46:05.535167 d2cd-0.0.3b0/d2cd/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-25 19:45:51.000000 d2cd-0.0.3b0/d2cd/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-25 19:45:51.000000 d2cd-0.0.3b0/d2cd/utils/docker_compose_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-25 19:45:51.000000 d2cd-0.0.3b0/d2cd/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-05-25 19:45:51.000000 d2cd-0.0.3b0/d2cd/utils/git_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-25 19:45:51.000000 d2cd-0.0.3b0/d2cd/utils/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:46:05.535167 d2cd-0.0.3b0/d2cd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-05-25 19:46:05.000000 d2cd-0.0.3b0/d2cd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-25 19:46:05.000000 d2cd-0.0.3b0/d2cd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 19:46:05.000000 d2cd-0.0.3b0/d2cd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-25 19:46:05.000000 d2cd-0.0.3b0/d2cd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-25 19:46:05.000000 d2cd-0.0.3b0/d2cd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-25 19:46:05.000000 d2cd-0.0.3b0/d2cd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-25 19:45:51.000000 d2cd-0.0.3b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 19:46:05.539167 d2cd-0.0.3b0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2061 2024-05-25 19:45:51.000000 d2cd-0.0.3b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:46:05.535167 d2cd-0.0.3b0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-05-25 19:45:51.000000 d2cd-0.0.3b0/tests/test_docker_compose_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-25 19:45:51.000000 d2cd-0.0.3b0/tests/test_git_utils.py
```

### Comparing `d2cd-0.0.1a0/d2cd/banner.py` & `d2cd-0.0.3b0/d2cd/banner.py`

 * *Files identical despite different names*

### Comparing `d2cd-0.0.1a0/d2cd/config_loader.py` & `d2cd-0.0.3b0/d2cd/config_loader.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python3
 
 """
 Config Loader and Config Schema Validator
 """
 
 import os
-from os.path import expanduser
 
 import yaml
 from giturlparse import parse
 from marshmallow import Schema, ValidationError, fields, validate, validates_schema
 
 
 class RepoSchema(Schema):
@@ -18,32 +17,34 @@
     branch = fields.Str(required=True)
     auth = fields.Dict(keys=fields.Str(), values=fields.Str(), required=True)
     username = fields.Str()
     password = fields.Str()
     docker_compose_paths = fields.List(fields.Str(), required=True)
 
     @validates_schema
-    def validate_auth(self, data):
+    def validate_auth(self, data, **kwargs):
         auth = data.get("auth", {})
         ssh_key_location = auth.get("ssh_key_location")
         username = auth.get("username")
         password = auth.get("password")
 
         if not (ssh_key_location or (username and password)):
             raise ValidationError(
                 "Either 'ssh_key_location' or 'username' and 'password' must be provided for authentication."
             )
 
         if ssh_key_location:
-            expanded_path = expanduser(ssh_key_location)
-            if not os.path.exists(expanded_path):
-                raise ValidationError("SSH key location does not exist.")
+            expanded_path = os.path.expanduser(ssh_key_location)
+            if not os.path.exists(ssh_key_location):
+                raise ValidationError(
+                    f"SSH key({ssh_key_location}) location does not exist."
+                )
 
     @validates_schema
-    def validate_url(self, data):
+    def validate_url(self, data, **kwargs):
         url = data.get("url")
         git_url = parse(url)
         if not git_url.valid:
             raise ValidationError("Invalid Git URL")
 
 
 class ConfigSchema(Schema):
```

### Comparing `d2cd-0.0.1a0/d2cd/main.py` & `d2cd-0.0.3b0/d2cd/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,53 +1,64 @@
 #!/usr/bin/env python3
 
 """
 Main module
 """
 
+import asyncio
 import os
-import time
+import sys
 
 from .banner import display_info
 from .cli import parse_arguments
 from .config_loader import ConfigLoader
 from .utils.docker_compose_utils import DockerComposeUtils
 from .utils.git_utils import GitUtils
 from .utils.logger import log
 
 
-def main():
-    args = parse_arguments()
-    if args.debug:
-        log.level("DEBUG")
+async def reconcile_repos(repo):
+    async with GitUtils(branch=repo["branch"], repo_url=repo["url"]) as gt:
+        if await gt.pull_changes_async():
+            for compose_path in repo["docker_compose_paths"]:
+                full_path = os.path.join(gt.repo_location, compose_path)
+                async with DockerComposeUtils(compose_files=[full_path]) as dc:
+                    await dc.up_async()
+        else:
+            log.info("No changes in upstream git repo")
 
-    cfg = ConfigLoader(config_file=args.config_file)
-    config = cfg.get_config()
 
-    display_info()
+async def reconcilation_loop(config):
+    log.info("Starting reconcilation in loop..")
+    while True:
+        await asyncio.sleep(config["sync_interval_seconds"])
+        tasks = []
+        for repo in config["repos"]:
+            tasks.append(reconcile_repos(repo))
+        await asyncio.gather(*tasks)
+
 
+def initialize_repos(config):
     for repo in config["repos"]:
         with GitUtils(
-            branch=repo["branch"],
-            repo_url=repo["url"],
-            auth=repo["auth"],
+            branch=repo["branch"], repo_url=repo["url"], auth=repo["auth"]
         ) as gt:
             gt.clone_repository()
+            for compose_path in repo["docker_compose_paths"]:
+                full_path = os.path.join(gt.repo_location, compose_path)
+                with DockerComposeUtils(compose_files=[full_path]) as dc:
+                    dc.up()
 
-    log.info("Start reconciliation in loop")
-    first_iteration = True
 
-    while True:
-        for repo in config["repos"]:
-            with GitUtils(branch=repo["branch"], repo_url=repo["url"]) as gt:
-                if gt.pull_changes():
-                    full_paths = [
-                        os.path.join(gt.repo_location, path)
-                        for path in repo["docker_compose_paths"]
-                    ]
-                    with DockerComposeUtils(compose_files=full_paths) as dc:
-                        if first_iteration:
-                            dc.up()
-                            first_iteration = False
-                else:
-                    log.info("No changes in upstream git repo")
-        time.sleep(config["sync_interval_seconds"])
+def main():
+    args = parse_arguments()
+
+    log.remove()
+    log.add(sys.stderr, level="DEBUG" if args.debug else "INFO")
+
+    cfg = ConfigLoader(config_file=args.config_file)
+    config = cfg.get_config()
+
+    display_info()
+
+    initialize_repos(config)
+    asyncio.run(reconcilation_loop(config))
```

### Comparing `d2cd-0.0.1a0/d2cd/utils/git_utils.py` & `d2cd-0.0.3b0/d2cd/utils/git_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
 
 """
 Git Utils
 """
 
+import asyncio
 import os
 
 from git import Git, InvalidGitRepositoryError, NoSuchPathError, Repo
 from giturlparse import parse
 
 from .errors import NoGitAuthenticationError
 from .logger import log
@@ -59,16 +60,18 @@
             log.info("Authentication using username and password for git")
             username = self.auth["username"]
             password = self.auth["password"]
             self.repo_url = f"https://{username}:{password}@{self.parsed_git_url.host}/{self.parsed_git_url.owner}/{self.parsed_git_url.name}.git"
         else:
             raise NoGitAuthenticationError("Authentication details not provided")
 
+        git_ssh_cmd += f" -o StrictHostKeyChecking=no"
+
         log.info(
-            f"Clone git repository {self.parsed_git_url.name} in {self.parsed_git_url}"
+            f"Clone git repository {self.parsed_git_url.name} in {self.repo_location}"
         )
         with Repo.clone_from(
             url=self.repo_url,
             to_path=self.repo_location,
             env={"GIT_SSH_COMMAND": git_ssh_cmd},
         ) as repo:
             repo.git.checkout(self.branch)
@@ -80,7 +83,19 @@
         with Repo(self.repo_location) as repo:
             old_commit_id = repo.head.commit.hexsha
             origin = repo.remotes.origin
             origin.fetch()
             repo.git.checkout(self.branch)
             origin.pull()
             return old_commit_id != repo.head.commit.hexsha
+
+    # ========================== asyncio wrapper methods ==========================
+
+    async def __aenter__(self):
+        return self
+
+    async def __aexit__(self, exc_type, exc_value, traceback):
+        pass
+
+    async def pull_changes_async(self):
+        result = await asyncio.to_thread(self.pull_changes)
+        return result
```

### Comparing `d2cd-0.0.1a0/pyproject.toml` & `d2cd-0.0.3b0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `d2cd-0.0.1a0/setup.py` & `d2cd-0.0.3b0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,33 +26,33 @@
     project_urls={
         "Changelog": "https://github.com/veerendra2/d2cd/blob/master/CHANGELOG.md",
         "Documentation": "https://d2cd.readthedocs.io/en/latest/",
     },
     keywords=["gitops", "cicd", "docker-compose", "continuous delivery"],
     license="MIT",
     classifiers=[
-        "Development Status :: 2 - Pre-Alpha",
-        "Topic :: Utilities",
+        "Development Status :: 4 - Beta",
         "Intended Audience :: System Administrators",
-        "Natural Language :: English",
         "License :: OSI Approved :: MIT License",
+        "Natural Language :: English",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3.13",
+        "Topic :: Utilities",
     ],
     install_requires=[
+        "GitPython==3.1.43",
         "loguru==0.7.2",
+        "marshmallow==3.21.1",
         "python-on-whales==0.71.0",
-        "GitPython==3.1.43",
         "giturlparse==0.12.0",
-        "marshmallow==3.21.1",
         "yamllint==1.33.0",
     ],
     python_requires=">=3.9",
     entry_points={"console_scripts": ["d2cd = d2cd.main:main"]},
 )
```

### Comparing `d2cd-0.0.1a0/tests/test_docker_compose_utils.py` & `d2cd-0.0.3b0/tests/test_docker_compose_utils.py`

 * *Files identical despite different names*

### Comparing `d2cd-0.0.1a0/tests/test_git_utils.py` & `d2cd-0.0.3b0/tests/test_git_utils.py`

 * *Files identical despite different names*

