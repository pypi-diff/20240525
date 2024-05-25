# Comparing `tmp/osbot_github_actions-0.1.0.tar.gz` & `tmp/osbot_github_actions-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osbot_github_actions-0.1.0.tar", max compression
+gzip compressed data, was "osbot_github_actions-0.4.0.tar", max compression
```

## Comparing `osbot_github_actions-0.1.0.tar` & `osbot_github_actions-0.4.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2024-05-24 15:54:00.529588 osbot_github_actions-0.1.0/LICENSE
--rw-r--r--   0        0        0      110 2024-05-24 15:54:00.529588 osbot_github_actions-0.1.0/README.md
--rw-r--r--   0        0        0       16 2024-05-24 15:54:00.529588 osbot_github_actions-0.1.0/osbot_github_actions/__init__.py
--rw-r--r--   0        0        0      471 2024-05-24 15:54:00.529588 osbot_github_actions-0.1.0/osbot_github_actions/utils/Version.py
--rw-r--r--   0        0        0        0 2024-05-24 15:54:00.529588 osbot_github_actions-0.1.0/osbot_github_actions/utils/__init__.py
--rw-r--r--   0        0        0        7 2024-05-24 15:54:00.529588 osbot_github_actions-0.1.0/osbot_github_actions/version
--rw-r--r--   0        0        0      618 2024-05-24 15:54:00.529588 osbot_github_actions-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      752 1970-01-01 00:00:00.000000 osbot_github_actions-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-24 17:21:37.373282 osbot_github_actions-0.4.0/LICENSE
+-rw-r--r--   0        0        0      110 2024-05-24 17:21:37.373282 osbot_github_actions-0.4.0/README.md
+-rw-r--r--   0        0        0       16 2024-05-24 17:21:37.373282 osbot_github_actions-0.4.0/osbot_github_actions/__init__.py
+-rw-r--r--   0        0        0      471 2024-05-24 17:21:37.373282 osbot_github_actions-0.4.0/osbot_github_actions/utils/Version.py
+-rw-r--r--   0        0        0        0 2024-05-24 17:21:37.373282 osbot_github_actions-0.4.0/osbot_github_actions/utils/__init__.py
+-rw-r--r--   0        0        0        7 2024-05-24 17:21:37.373282 osbot_github_actions-0.4.0/osbot_github_actions/version
+-rw-r--r--   0        0        0      618 2024-05-24 17:21:37.373282 osbot_github_actions-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      752 1970-01-01 00:00:00.000000 osbot_github_actions-0.4.0/PKG-INFO
```

### Comparing `osbot_github_actions-0.1.0/LICENSE` & `osbot_github_actions-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `osbot_github_actions-0.1.0/pyproject.toml` & `osbot_github_actions-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name        = "osbot_github_actions"
-version     = "v0.1.0"
+version     = "v0.4.0"
 description = "OWASP Security Bot - GitHub Actions"
 authors     = ["Dinis Cruz <dinis.cruz@owasp.org>"]
 license     = "MIT"
 readme      = "README.md"
-homepage    = "https://github.com/owasp-sbot/OSBot-GitHub_Actions"
-repository  = "https://github.com/owasp-sbot/OSBot-GitHub_Actions"
+repository  = "https://github.com/owasp-sbot/OSBot-GitHub-Actions"
+homepage    = "https://github.com/owasp-sbot/OSBot-GitHub-Actions"
 
 [tool.poetry.dependencies]
 python          = "^3.11"
 python-dotenv   = "*"
 osbot_utils     = "*"
 
 [tool.poetry.group.dev.dependencies]
```

