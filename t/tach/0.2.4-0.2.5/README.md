# Comparing `tmp/tach-0.2.4.tar.gz` & `tmp/tach-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tach-0.2.4.tar", last modified: Thu May 23 17:39:24 2024, max compression
+gzip compressed data, was "tach-0.2.5.tar", last modified: Fri May 24 22:52:14 2024, max compression
```

## Comparing `tach-0.2.4.tar` & `tach-0.2.5.tar`

### file list

```diff
@@ -1,136 +1,146 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:24.800980 tach-0.2.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:24.780980 tach-0.2.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:24.784980 tach-0.2.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-23 17:39:20.000000 tach-0.2.4/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-23 17:39:20.000000 tach-0.2.4/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-23 17:39:20.000000 tach-0.2.4/.github/workflows/publish_docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-23 17:39:20.000000 tach-0.2.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-23 17:39:20.000000 tach-0.2.4/.pre-commit-hooks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-23 17:39:20.000000 tach-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-05-23 17:39:24.800980 tach-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4075 2024-05-23 17:39:20.000000 tach-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-23 17:39:20.000000 tach-0.2.4/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:24.788980 tach-0.2.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-23 17:39:20.000000 tach-0.2.4/docs/configuration.md
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-23 17:39:20.000000 tach-0.2.4/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-23 17:39:20.000000 tach-0.2.4/docs/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-23 17:39:20.000000 tach-0.2.4/docs/getting-started.md
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-23 17:39:20.000000 tach-0.2.4/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-23 17:39:20.000000 tach-0.2.4/docs/strict-mode.md
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-23 17:39:20.000000 tach-0.2.4/docs/tach-ignore.md
--rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-05-23 17:39:20.000000 tach-0.2.4/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-23 17:39:20.000000 tach-0.2.4/docs/why-tach.md
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-23 17:39:20.000000 tach-0.2.4/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-05-23 17:39:20.000000 tach-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 17:39:24.800980 tach-0.2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:24.788980 tach-0.2.4/tach/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:20.000000 tach-0.2.4/tach/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6650 2024-05-23 17:39:20.000000 tach-0.2.4/tach/check.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-23 17:39:20.000000 tach-0.2.4/tach/clean.py
--rw-r--r--   0 runner    (1001) docker     (127)    12083 2024-05-23 17:39:20.000000 tach-0.2.4/tach/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:24.788980 tach-0.2.4/tach/colors/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-23 17:39:20.000000 tach-0.2.4/tach/colors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-23 17:39:20.000000 tach-0.2.4/tach/colors/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:24.788980 tach-0.2.4/tach/constants/
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-23 17:39:20.000000 tach-0.2.4/tach/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-23 17:39:20.000000 tach-0.2.4/tach/constants/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:24.792980 tach-0.2.4/tach/core/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-23 17:39:20.000000 tach-0.2.4/tach/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-05-23 17:39:20.000000 tach-0.2.4/tach/core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-23 17:39:20.000000 tach-0.2.4/tach/core/package.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-23 17:39:20.000000 tach-0.2.4/tach/core/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:24.792980 tach-0.2.4/tach/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-23 17:39:20.000000 tach-0.2.4/tach/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-23 17:39:20.000000 tach-0.2.4/tach/errors/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:24.792980 tach-0.2.4/tach/filesystem/
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-23 17:39:20.000000 tach-0.2.4/tach/filesystem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-23 17:39:20.000000 tach-0.2.4/tach/filesystem/install.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-23 17:39:20.000000 tach-0.2.4/tach/filesystem/package.py
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-23 17:39:20.000000 tach-0.2.4/tach/filesystem/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-23 17:39:20.000000 tach-0.2.4/tach/filesystem/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    10412 2024-05-23 17:39:20.000000 tach-0.2.4/tach/filesystem/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:24.792980 tach-0.2.4/tach/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-23 17:39:20.000000 tach-0.2.4/tach/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-23 17:39:20.000000 tach-0.2.4/tach/hooks/package.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)      380 2024-05-23 17:39:20.000000 tach-0.2.4/tach/hooks/pre_commit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:24.792980 tach-0.2.4/tach/interactive/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-23 17:39:20.000000 tach-0.2.4/tach/interactive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-23 17:39:20.000000 tach-0.2.4/tach/interactive/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)    19361 2024-05-23 17:39:20.000000 tach-0.2.4/tach/interactive/packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-23 17:39:20.000000 tach-0.2.4/tach/loading.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-23 17:39:20.000000 tach-0.2.4/tach/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:24.796980 tach-0.2.4/tach/parsing/
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-23 17:39:20.000000 tach-0.2.4/tach/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-23 17:39:20.000000 tach-0.2.4/tach/parsing/ast_visitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-23 17:39:20.000000 tach-0.2.4/tach/parsing/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-05-23 17:39:20.000000 tach-0.2.4/tach/parsing/imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-23 17:39:20.000000 tach-0.2.4/tach/parsing/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-23 17:39:20.000000 tach-0.2.4/tach/parsing/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-23 17:39:20.000000 tach-0.2.4/tach/parsing/packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-23 17:39:20.000000 tach-0.2.4/tach/pkg.py
--rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-05-23 17:39:20.000000 tach-0.2.4/tach/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:24.800980 tach-0.2.4/tach.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-05-23 17:39:24.000000 tach-0.2.4/tach.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-05-23 17:39:24.000000 tach-0.2.4/tach.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 17:39:24.000000 tach-0.2.4/tach.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-23 17:39:24.000000 tach-0.2.4/tach.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-23 17:39:24.000000 tach-0.2.4/tach.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-23 17:39:24.000000 tach-0.2.4/tach.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-23 17:39:20.000000 tach-0.2.4/tach.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:24.796980 tach-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:20.000000 tach-0.2.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:24.796980 tach-0.2.4/tests/example/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:20.000000 tach-0.2.4/tests/example/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:24.796980 tach-0.2.4/tests/example/domain_one/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:20.000000 tach-0.2.4/tests/example/domain_one/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:20.000000 tach-0.2.4/tests/example/domain_one/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:24.796980 tach-0.2.4/tests/example/domain_one/subdomain/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-23 17:39:20.000000 tach-0.2.4/tests/example/domain_one/subdomain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:20.000000 tach-0.2.4/tests/example/domain_one/subdomain/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:24.796980 tach-0.2.4/tests/example/domain_three/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:20.000000 tach-0.2.4/tests/example/domain_three/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-23 17:39:20.000000 tach-0.2.4/tests/example/domain_three/core.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:20.000000 tach-0.2.4/tests/example/domain_three/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:24.796980 tach-0.2.4/tests/example/domain_two/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:20.000000 tach-0.2.4/tests/example/domain_two/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:20.000000 tach-0.2.4/tests/example/domain_two/core.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:20.000000 tach-0.2.4/tests/example/domain_two/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:24.796980 tach-0.2.4/tests/example/domain_two/subdomain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:20.000000 tach-0.2.4/tests/example/domain_two/subdomain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:20.000000 tach-0.2.4/tests/example/domain_two/subdomain/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:24.796980 tach-0.2.4/tests/example/invalid/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:20.000000 tach-0.2.4/tests/example/invalid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:24.800980 tach-0.2.4/tests/example/invalid/empty/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:20.000000 tach-0.2.4/tests/example/invalid/empty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:20.000000 tach-0.2.4/tests/example/invalid/empty/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:20.000000 tach-0.2.4/tests/example/invalid/empty/tach.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:24.800980 tach-0.2.4/tests/example/invalid/hidden/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:24.800980 tach-0.2.4/tests/example/invalid/hidden/.hidden/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-23 17:39:20.000000 tach-0.2.4/tests/example/invalid/hidden/.hidden/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-23 17:39:20.000000 tach-0.2.4/tests/example/invalid/hidden/.hidden/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:20.000000 tach-0.2.4/tests/example/invalid/hidden/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-23 17:39:20.000000 tach-0.2.4/tests/example/invalid/hidden/tach.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:24.800980 tach-0.2.4/tests/example/invalid/hidden/unhidden/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:20.000000 tach-0.2.4/tests/example/invalid/hidden/unhidden/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-23 17:39:20.000000 tach-0.2.4/tests/example/invalid/hidden/unhidden/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-23 17:39:20.000000 tach-0.2.4/tests/example/invalid/hidden/unhidden/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-23 17:39:20.000000 tach-0.2.4/tests/example/invalid/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-23 17:39:20.000000 tach-0.2.4/tests/example/invalid/tach.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:24.800980 tach-0.2.4/tests/example/valid/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:20.000000 tach-0.2.4/tests/example/valid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:24.800980 tach-0.2.4/tests/example/valid/domain_one/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:20.000000 tach-0.2.4/tests/example/valid/domain_one/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-23 17:39:20.000000 tach-0.2.4/tests/example/valid/domain_one/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:24.800980 tach-0.2.4/tests/example/valid/domain_three/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-23 17:39:20.000000 tach-0.2.4/tests/example/valid/domain_three/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-23 17:39:20.000000 tach-0.2.4/tests/example/valid/domain_three/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:24.800980 tach-0.2.4/tests/example/valid/domain_two/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-23 17:39:20.000000 tach-0.2.4/tests/example/valid/domain_two/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-23 17:39:20.000000 tach-0.2.4/tests/example/valid/domain_two/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-23 17:39:20.000000 tach-0.2.4/tests/example/valid/tach.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-05-23 17:39:20.000000 tach-0.2.4/tests/test_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-05-23 17:39:20.000000 tach-0.2.4/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-23 17:39:20.000000 tach-0.2.4/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-23 17:39:20.000000 tach-0.2.4/tests/test_package_trie.py
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-05-23 17:39:20.000000 tach-0.2.4/tests/test_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 17:39:20.000000 tach-0.2.4/tests/test_show.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:52:14.652388 tach-0.2.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:52:14.632388 tach-0.2.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:52:14.636388 tach-0.2.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-24 22:52:10.000000 tach-0.2.5/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-24 22:52:10.000000 tach-0.2.5/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-24 22:52:10.000000 tach-0.2.5/.github/workflows/publish_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-05-24 22:52:10.000000 tach-0.2.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-24 22:52:10.000000 tach-0.2.5/.pre-commit-hooks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-24 22:52:10.000000 tach-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5656 2024-05-24 22:52:14.652388 tach-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-05-24 22:52:10.000000 tach-0.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-24 22:52:10.000000 tach-0.2.5/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:52:14.640388 tach-0.2.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-24 22:52:10.000000 tach-0.2.5/docs/configuration.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-24 22:52:10.000000 tach-0.2.5/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-24 22:52:10.000000 tach-0.2.5/docs/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-24 22:52:10.000000 tach-0.2.5/docs/getting-started.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-24 22:52:10.000000 tach-0.2.5/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-24 22:52:10.000000 tach-0.2.5/docs/strict-mode.md
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-24 22:52:10.000000 tach-0.2.5/docs/tach-ignore.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-05-24 22:52:10.000000 tach-0.2.5/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-24 22:52:10.000000 tach-0.2.5/docs/why-tach.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-24 22:52:10.000000 tach-0.2.5/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-24 22:52:10.000000 tach-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 22:52:14.652388 tach-0.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:52:14.640388 tach-0.2.5/tach/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 22:52:10.000000 tach-0.2.5/tach/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:52:14.640388 tach-0.2.5/tach/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-24 22:52:10.000000 tach-0.2.5/tach/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-24 22:52:10.000000 tach-0.2.5/tach/cache/access.py
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-24 22:52:10.000000 tach-0.2.5/tach/cache/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-24 22:52:10.000000 tach-0.2.5/tach/cache/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6579 2024-05-24 22:52:10.000000 tach-0.2.5/tach/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-24 22:52:10.000000 tach-0.2.5/tach/clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13109 2024-05-24 22:52:10.000000 tach-0.2.5/tach/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:52:14.644388 tach-0.2.5/tach/colors/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-24 22:52:10.000000 tach-0.2.5/tach/colors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-24 22:52:10.000000 tach-0.2.5/tach/colors/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:52:14.644388 tach-0.2.5/tach/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-24 22:52:10.000000 tach-0.2.5/tach/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-24 22:52:10.000000 tach-0.2.5/tach/constants/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:52:14.644388 tach-0.2.5/tach/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-24 22:52:10.000000 tach-0.2.5/tach/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4321 2024-05-24 22:52:10.000000 tach-0.2.5/tach/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-24 22:52:10.000000 tach-0.2.5/tach/core/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-24 22:52:10.000000 tach-0.2.5/tach/core/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:52:14.644388 tach-0.2.5/tach/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-24 22:52:10.000000 tach-0.2.5/tach/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-24 22:52:10.000000 tach-0.2.5/tach/errors/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:52:14.644388 tach-0.2.5/tach/filesystem/
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-24 22:52:10.000000 tach-0.2.5/tach/filesystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-24 22:52:10.000000 tach-0.2.5/tach/filesystem/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-24 22:52:10.000000 tach-0.2.5/tach/filesystem/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-24 22:52:10.000000 tach-0.2.5/tach/filesystem/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-24 22:52:10.000000 tach-0.2.5/tach/filesystem/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9989 2024-05-24 22:52:10.000000 tach-0.2.5/tach/filesystem/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:52:14.644388 tach-0.2.5/tach/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-24 22:52:10.000000 tach-0.2.5/tach/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-24 22:52:10.000000 tach-0.2.5/tach/hooks/package.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      380 2024-05-24 22:52:10.000000 tach-0.2.5/tach/hooks/pre_commit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:52:14.644388 tach-0.2.5/tach/interactive/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-24 22:52:10.000000 tach-0.2.5/tach/interactive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-24 22:52:10.000000 tach-0.2.5/tach/interactive/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    19399 2024-05-24 22:52:10.000000 tach-0.2.5/tach/interactive/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-24 22:52:10.000000 tach-0.2.5/tach/loading.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:52:14.644388 tach-0.2.5/tach/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-24 22:52:10.000000 tach-0.2.5/tach/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-24 22:52:10.000000 tach-0.2.5/tach/logging/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-24 22:52:10.000000 tach-0.2.5/tach/logging/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-24 22:52:10.000000 tach-0.2.5/tach/logging/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-24 22:52:10.000000 tach-0.2.5/tach/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:52:14.648388 tach-0.2.5/tach/parsing/
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-24 22:52:10.000000 tach-0.2.5/tach/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-24 22:52:10.000000 tach-0.2.5/tach/parsing/ast_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-24 22:52:10.000000 tach-0.2.5/tach/parsing/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-05-24 22:52:10.000000 tach-0.2.5/tach/parsing/imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-24 22:52:10.000000 tach-0.2.5/tach/parsing/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-24 22:52:10.000000 tach-0.2.5/tach/parsing/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-24 22:52:10.000000 tach-0.2.5/tach/parsing/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-24 22:52:10.000000 tach-0.2.5/tach/pkg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-05-24 22:52:10.000000 tach-0.2.5/tach/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:52:14.652388 tach-0.2.5/tach.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5656 2024-05-24 22:52:14.000000 tach-0.2.5/tach.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-05-24 22:52:14.000000 tach-0.2.5/tach.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 22:52:14.000000 tach-0.2.5/tach.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-24 22:52:14.000000 tach-0.2.5/tach.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-24 22:52:14.000000 tach-0.2.5/tach.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-24 22:52:14.000000 tach-0.2.5/tach.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-24 22:52:10.000000 tach-0.2.5/tach.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:52:14.648388 tach-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 22:52:10.000000 tach-0.2.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:52:14.648388 tach-0.2.5/tests/example/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 22:52:10.000000 tach-0.2.5/tests/example/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:52:14.648388 tach-0.2.5/tests/example/domain_one/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 22:52:10.000000 tach-0.2.5/tests/example/domain_one/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 22:52:10.000000 tach-0.2.5/tests/example/domain_one/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:52:14.648388 tach-0.2.5/tests/example/domain_one/subdomain/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-24 22:52:10.000000 tach-0.2.5/tests/example/domain_one/subdomain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 22:52:10.000000 tach-0.2.5/tests/example/domain_one/subdomain/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:52:14.648388 tach-0.2.5/tests/example/domain_three/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 22:52:10.000000 tach-0.2.5/tests/example/domain_three/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-24 22:52:10.000000 tach-0.2.5/tests/example/domain_three/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 22:52:10.000000 tach-0.2.5/tests/example/domain_three/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:52:14.648388 tach-0.2.5/tests/example/domain_two/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 22:52:10.000000 tach-0.2.5/tests/example/domain_two/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 22:52:10.000000 tach-0.2.5/tests/example/domain_two/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 22:52:10.000000 tach-0.2.5/tests/example/domain_two/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:52:14.648388 tach-0.2.5/tests/example/domain_two/subdomain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 22:52:10.000000 tach-0.2.5/tests/example/domain_two/subdomain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 22:52:10.000000 tach-0.2.5/tests/example/domain_two/subdomain/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:52:14.652388 tach-0.2.5/tests/example/invalid/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 22:52:10.000000 tach-0.2.5/tests/example/invalid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:52:14.652388 tach-0.2.5/tests/example/invalid/empty/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 22:52:10.000000 tach-0.2.5/tests/example/invalid/empty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 22:52:10.000000 tach-0.2.5/tests/example/invalid/empty/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 22:52:10.000000 tach-0.2.5/tests/example/invalid/empty/tach.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:52:14.652388 tach-0.2.5/tests/example/invalid/hidden/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:52:14.652388 tach-0.2.5/tests/example/invalid/hidden/.hidden/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-24 22:52:10.000000 tach-0.2.5/tests/example/invalid/hidden/.hidden/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-24 22:52:10.000000 tach-0.2.5/tests/example/invalid/hidden/.hidden/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 22:52:10.000000 tach-0.2.5/tests/example/invalid/hidden/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-24 22:52:10.000000 tach-0.2.5/tests/example/invalid/hidden/tach.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:52:14.652388 tach-0.2.5/tests/example/invalid/hidden/unhidden/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 22:52:10.000000 tach-0.2.5/tests/example/invalid/hidden/unhidden/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-24 22:52:10.000000 tach-0.2.5/tests/example/invalid/hidden/unhidden/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-24 22:52:10.000000 tach-0.2.5/tests/example/invalid/hidden/unhidden/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-24 22:52:10.000000 tach-0.2.5/tests/example/invalid/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-24 22:52:10.000000 tach-0.2.5/tests/example/invalid/tach.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:52:14.652388 tach-0.2.5/tests/example/valid/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 22:52:10.000000 tach-0.2.5/tests/example/valid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:52:14.652388 tach-0.2.5/tests/example/valid/domain_one/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 22:52:10.000000 tach-0.2.5/tests/example/valid/domain_one/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-24 22:52:10.000000 tach-0.2.5/tests/example/valid/domain_one/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:52:14.652388 tach-0.2.5/tests/example/valid/domain_three/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-24 22:52:10.000000 tach-0.2.5/tests/example/valid/domain_three/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-24 22:52:10.000000 tach-0.2.5/tests/example/valid/domain_three/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:52:14.652388 tach-0.2.5/tests/example/valid/domain_two/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-24 22:52:10.000000 tach-0.2.5/tests/example/valid/domain_two/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-24 22:52:10.000000 tach-0.2.5/tests/example/valid/domain_two/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-24 22:52:10.000000 tach-0.2.5/tests/example/valid/tach.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-05-24 22:52:10.000000 tach-0.2.5/tests/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-05-24 22:52:10.000000 tach-0.2.5/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-24 22:52:10.000000 tach-0.2.5/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-24 22:52:10.000000 tach-0.2.5/tests/test_package_trie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-24 22:52:10.000000 tach-0.2.5/tests/test_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 22:52:10.000000 tach-0.2.5/tests/test_show.py
```

### Comparing `tach-0.2.4/.github/workflows/ci.yml` & `tach-0.2.5/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `tach-0.2.4/.github/workflows/publish.yml` & `tach-0.2.5/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `tach-0.2.4/.github/workflows/publish_docs.yml` & `tach-0.2.5/.github/workflows/publish_docs.yml`

 * *Files identical despite different names*

### Comparing `tach-0.2.4/.gitignore` & `tach-0.2.5/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -161,7 +161,8 @@
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 .idea/
 
 .python-version
 .env.leave
 .DS_Store
+.pre-commit-config.yaml
```

### Comparing `tach-0.2.4/LICENSE` & `tach-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tach-0.2.4/PKG-INFO` & `tach-0.2.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tach
-Version: 0.2.4
+Version: 0.2.5
 Summary: A Python tool to maintain a modular package architecture.
 Author-email: Caelean Barnes <caeleanb@gmail.com>, Evan Doyle <evanmdoyle@gmail.com>
 Project-URL: Homepage, https://github.com/gauge-sh/tach
 Project-URL: Issues, https://github.com/gauge-sh/tach/issues
 Keywords: python,module,package,guard,enforcement,boundary,enforcer,domain,architecture
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -25,14 +25,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyyaml==6.0.1
 Requires-Dist: pydantic==2.7.1
 Requires-Dist: stdlib-list==0.10.0
 Requires-Dist: rich==13.7.1
 Requires-Dist: prompt-toolkit==3.0.43
+Requires-Dist: eval-type-backport==0.2.0
 
 [![image](https://img.shields.io/pypi/v/tach.svg)](https://pypi.Python.org/pypi/tach)
 [![image](https://img.shields.io/pypi/l/tach.svg)](https://pypi.Python.org/pypi/tach)
 [![image](https://img.shields.io/pypi/pyversions/tach.svg)](https://pypi.Python.org/pypi/tach)
 [![image](https://github.com/gauge-sh/tach/actions/workflows/ci.yml/badge.svg)](https://github.com/gauge-sh/tach/actions/workflows/ci.yml)
 [![Checked with pyright](https://microsoft.github.io/pyright/img/pyright_badge.svg)](https://microsoft.github.io/pyright/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
@@ -124,11 +125,11 @@
 Tach also supports:
 - [Manual file configuration](https://gauge-sh.github.io/tach/configuration/)
 - [Strict public interfaces for packages](https://gauge-sh.github.io/tach/strict-mode/)
 - [Inline exceptions](https://gauge-sh.github.io/tach/tach-ignore/)
 - [Pre-commit hooks](https://gauge-sh.github.io/tach/usage/#tach-install)
 
 
-More info in the [docs](https://gauge-sh.github.io/tach/).
-If you have any feedback, we'd love to hear it!
+More info in the [docs](https://gauge-sh.github.io/tach/). Tach logs anonymized usage statistics which are easily [opted out](https://gauge-sh.github.io/tach/faq/) of.
+If you have any feedback, we'd love to talk!
 
 [Discord](https://discord.gg/a58vW8dnmw)
```

### Comparing `tach-0.2.4/README.md` & `tach-0.2.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -92,11 +92,11 @@
 Tach also supports:
 - [Manual file configuration](https://gauge-sh.github.io/tach/configuration/)
 - [Strict public interfaces for packages](https://gauge-sh.github.io/tach/strict-mode/)
 - [Inline exceptions](https://gauge-sh.github.io/tach/tach-ignore/)
 - [Pre-commit hooks](https://gauge-sh.github.io/tach/usage/#tach-install)
 
 
-More info in the [docs](https://gauge-sh.github.io/tach/).
-If you have any feedback, we'd love to hear it!
+More info in the [docs](https://gauge-sh.github.io/tach/). Tach logs anonymized usage statistics which are easily [opted out](https://gauge-sh.github.io/tach/faq/) of.
+If you have any feedback, we'd love to talk!
 
 [Discord](https://discord.gg/a58vW8dnmw)
```

### Comparing `tach-0.2.4/docs/configuration.md` & `tach-0.2.5/docs/configuration.md`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,14 @@
   - scope:core
   - scope:filesystem
   - scope:parsing
 exclude:
 - tests/
 - docs/
 - build/
-exclude_hidden_paths: true
 ignore_type_checking_imports: true
 ```
 
 
 ## `package.yml`
 
 This is the package-level configuration file which should exist in each package in your project.
```

### Comparing `tach-0.2.4/docs/faq.md` & `tach-0.2.5/docs/faq.md`

 * *Files 14% similar despite different names*

```diff
@@ -11,7 +11,12 @@
 ### Are conditional imports checked?
 At the moment, `tach` will check all imports in your source files, including those which are called conditionally.
 The only exceptions are imports made within `TYPE_CHECKING` conditional blocks. If you want to disable checks for
 these imports, you can add `ignore_type_checking_imports: true` to your `tach.yml`.
 
 ### Can you catch dynamic references?
 Since `tach` uses the AST to find imports and public members, dynamic imports (e.g. using a string path) and dynamic names (e.g. using `setattr`, `locals`, `globals`) are generally not supported. If these usages cause `tach` to report incorrect errors, the [ignore directive](tach-ignore#tach-ignore) should be sufficient to reach a passing state.
+
+### What information does Tach track?
+
+Tach tracks anonymized usage and error report statistics; we ascribe to Posthog's approach as detailed [here](https://posthog.com/blog/open-source-telemetry-ethical).
+If you would like to opt out of sending anonymized info, you can set `disable_logging` to `true` in your `tach.yml`.
```

### Comparing `tach-0.2.4/docs/favicon.ico` & `tach-0.2.5/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `tach-0.2.4/docs/getting-started.md` & `tach-0.2.5/docs/getting-started.md`

 * *Files identical despite different names*

### Comparing `tach-0.2.4/docs/index.md` & `tach-0.2.5/docs/index.md`

 * *Files identical despite different names*

### Comparing `tach-0.2.4/docs/strict-mode.md` & `tach-0.2.5/docs/strict-mode.md`

 * *Files identical despite different names*

### Comparing `tach-0.2.4/docs/tach-ignore.md` & `tach-0.2.5/docs/tach-ignore.md`

 * *Files identical despite different names*

### Comparing `tach-0.2.4/docs/usage.md` & `tach-0.2.5/docs/usage.md`

 * *Files identical despite different names*

### Comparing `tach-0.2.4/docs/why-tach.md` & `tach-0.2.5/docs/why-tach.md`

 * *Files identical despite different names*

### Comparing `tach-0.2.4/mkdocs.yml` & `tach-0.2.5/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `tach-0.2.4/pyproject.toml` & `tach-0.2.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tach"
-version = "0.2.4"
+version = "0.2.5"
 authors = [
   { name="Caelean Barnes", email="caeleanb@gmail.com" },
   { name="Evan Doyle", email="evanmdoyle@gmail.com" },
 ]
 description = "A Python tool to maintain a modular package architecture."
 readme = "README.md"
 requires-python = ">=3.8"
@@ -26,30 +26,42 @@
     "Topic :: Software Development :: Quality Assurance",
 ]
 dependencies = [
     "pyyaml==6.0.1",
     "pydantic==2.7.1",
     "stdlib-list==0.10.0",
     "rich==13.7.1",
-    "prompt-toolkit==3.0.43"
+    "prompt-toolkit==3.0.43",
+    "eval-type-backport==0.2.0",
 ]
 keywords = ['python', 'module', 'package', 'guard', 'enforcement', 'boundary', 'enforcer', 'domain', 'architecture']
 
 
 [project.urls]
 Homepage = "https://github.com/gauge-sh/tach"
 Issues = "https://github.com/gauge-sh/tach/issues"
 
 [tool.ruff]
 target-version = "py38"
-lint.extend-select = ["I"]
+lint.extend-select = ["I", "TCH"]
 
 [tool.ruff.lint.isort]
 required-imports = ["from __future__ import annotations"]
 
+[tool.ruff.lint.flake8-type-checking]
+runtime-evaluated-base-classes = [
+    "pydantic.BaseModel",
+    "pydantic.RootModel",
+]
+runtime-evaluated-decorators = [
+    "pydantic.dataclasses.dataclass",
+    "dataclasses.dataclass",
+]
+exempt-modules = ["typing", "typing_extensions"]
+
 [tool.pyright]
 include = ["tach"]
 exclude = ["**/__pycache__", ".venv"]
 strict = ["tach"]
 pythonVersion = "3.8"
 
 [build-system]
```

### Comparing `tach-0.2.4/tach/check.py` & `tach-0.2.5/tach/check.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from __future__ import annotations
 
 import os
 from dataclasses import dataclass, field
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 
 from tach import errors
 from tach import filesystem as fs
-from tach.core import PackageNode, PackageTrie, ProjectConfig
 from tach.parsing import build_package_trie, get_project_imports
 
+if TYPE_CHECKING:
+    from tach.core import PackageNode, PackageTrie, ProjectConfig
+
 
 @dataclass
 class ErrorInfo:
     source_tags: list[str] = field(default_factory=list)
     invalid_tags: list[str] = field(default_factory=list)
     allowed_tags: list[str] = field(default_factory=list)
     exception_message: str = ""
@@ -117,15 +119,14 @@
     error_info: ErrorInfo
 
 
 def check(
     root: str,
     project_config: ProjectConfig,
     exclude_paths: Optional[list[str]] = None,
-    exclude_hidden_paths: Optional[bool] = True,
 ) -> list[BoundaryError]:
     if not os.path.isdir(root):
         raise errors.TachSetupError(f"The path {root} is not a valid directory.")
 
     cwd = fs.get_cwd()
     try:
         fs.chdir(root)
@@ -134,20 +135,22 @@
 
         if exclude_paths is not None and project_config.exclude is not None:
             exclude_paths.extend(project_config.exclude)
         else:
             exclude_paths = project_config.exclude
 
         package_trie = build_package_trie(
-            root, exclude_paths=exclude_paths, exclude_hidden_paths=exclude_hidden_paths
+            root,
+            exclude_paths=exclude_paths,
         )
 
         boundary_errors: list[BoundaryError] = []
         for file_path in fs.walk_pyfiles(
-            root, exclude_paths=exclude_paths, exclude_hidden_paths=exclude_hidden_paths
+            root,
+            exclude_paths=exclude_paths,
         ):
             mod_path = fs.file_to_module_path(file_path)
             nearest_package = package_trie.find_nearest(mod_path)
             if nearest_package is None:
                 continue
 
             # This should only give us imports from within our project
```

### Comparing `tach-0.2.4/tach/cli.py` & `tach-0.2.5/tach/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 from __future__ import annotations
 
 import argparse
 import os
 import sys
 from enum import Enum
 from functools import lru_cache
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 
 from tach import filesystem as fs
 from tach.check import BoundaryError, check
 from tach.clean import clean_project
 from tach.colors import BCOLORS
 from tach.constants import TOOL_NAME
-from tach.core import TagDependencyRules
 from tach.filesystem import install_pre_commit
 from tach.loading import start_spinner, stop_spinner
+from tach.logging import LogDataModel, logger
 from tach.parsing import parse_project_config
 from tach.pkg import pkg_edit_interactive
 from tach.sync import prune_dependency_constraints, sync_project
 
+if TYPE_CHECKING:
+    from tach.core import TagDependencyRules
+
 
 class TerminalEnvironment(Enum):
     UNKNOWN = 1
     JETBRAINS = 2
     VSCODE = 3
 
 
 @lru_cache()
 def detect_environment() -> TerminalEnvironment:
     if "jetbrains" in os.environ.get("TERMINAL_EMULATOR", "").lower():
         return TerminalEnvironment.JETBRAINS
     elif "vscode" in os.environ.get("TERM_PROGRAM", "").lower():
         return TerminalEnvironment.VSCODE
-
     return TerminalEnvironment.UNKNOWN
 
 
 def create_clickable_link(file_path: str, line: Optional[int] = None) -> str:
     terminal_env = detect_environment()
     abs_path = os.path.abspath(file_path)
 
@@ -211,29 +213,37 @@
 
 
 def tach_check(
     root: str = ".",
     exact: bool = False,
     exclude_paths: Optional[list[str]] = None,
 ):
+    logger.info(
+        "tach check called",
+        extra={
+            "data": LogDataModel(
+                function="tach_check",
+                parameters={"exact": exact},
+            ),
+        },
+    )
     try:
         project_config = parse_project_config(root=root)
         if exact is False and project_config.exact is True:
             exact = True
 
         if exclude_paths is not None and project_config.exclude is not None:
             exclude_paths.extend(project_config.exclude)
         else:
             exclude_paths = project_config.exclude
 
         boundary_errors: list[BoundaryError] = check(
             root,
             project_config,
             exclude_paths=exclude_paths,
-            exclude_hidden_paths=project_config.exclude_hidden_paths,
         )
 
         # If we're checking in strict mode, we want to verify that pruning constraints has no effect
         if not boundary_errors and exact:
             pruned_config = prune_dependency_constraints(
                 ".", project_config=project_config, exclude_paths=exclude_paths
             )
@@ -252,14 +262,23 @@
         print_errors(boundary_errors)
         sys.exit(1)
     print(f"✅ {BCOLORS.OKGREEN}All package dependencies validated!{BCOLORS.ENDC}")
     sys.exit(0)
 
 
 def tach_pkg(depth: Optional[int] = 1, exclude_paths: Optional[list[str]] = None):
+    logger.info(
+        "tach pkg called",
+        extra={
+            "data": LogDataModel(
+                function="tach_pkg",
+                parameters={"depth": depth},
+            ),
+        },
+    )
     try:
         saved_changes, warnings = pkg_edit_interactive(
             root=".", depth=depth, exclude_paths=exclude_paths
         )
     except Exception as e:
         print(str(e))
         sys.exit(1)
@@ -271,25 +290,43 @@
             f"✅ {BCOLORS.OKGREEN}Set packages! You may want to run '{TOOL_NAME} sync' "
             f"to automatically set boundaries.{BCOLORS.ENDC}"
         )
     sys.exit(0)
 
 
 def tach_sync(prune: bool = False, exclude_paths: Optional[list[str]] = None):
+    logger.info(
+        "tach sync called",
+        extra={
+            "data": LogDataModel(
+                function="tach_sync",
+                parameters={"prune": prune},
+            ),
+        },
+    )
     try:
         sync_project(prune=prune, exclude_paths=exclude_paths)
     except Exception as e:
         print(str(e))
         sys.exit(1)
 
     print(f"✅ {BCOLORS.OKGREEN}Synced dependencies.{BCOLORS.ENDC}")
     sys.exit(0)
 
 
 def tach_clean(force: bool = False) -> None:
+    logger.info(
+        "tach clean called",
+        extra={
+            "data": LogDataModel(
+                function="tach_clean",
+                parameters={"force": force},
+            ),
+        },
+    )
     print(
         f"{BCOLORS.WARNING}This will DELETE all existing configuration for {TOOL_NAME}.{BCOLORS.ENDC}"
     )
     root = fs.find_project_config_root(".") or "."
     print(
         f"{BCOLORS.WARNING}Deletion will occur for project with root: '{os.path.abspath(root)}'{BCOLORS.ENDC}"
     )
@@ -313,14 +350,22 @@
 
     @classmethod
     def choices(cls) -> list[str]:
         return [item.value for item in cls]
 
 
 def tach_install(path: str, target: InstallTarget, project_root: str = "") -> None:
+    logger.info(
+        "tach install called",
+        extra={
+            "data": LogDataModel(
+                function="tach_install",
+            ),
+        },
+    )
     try:
         if target == InstallTarget.PRE_COMMIT:
             installed, warning = install_pre_commit(
                 path=path, project_root=project_root
             )
         else:
             raise NotImplementedError(f"Target {target} is not supported by 'install'.")
```

### Comparing `tach-0.2.4/tach/core/config.py` & `tach-0.2.5/tach/core/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,38 +26,44 @@
     tag: str
     depends_on: List[str]
 
 
 def is_deprecated_project_config(config: dict[str, Any]) -> bool:
     if not config:
         return False
+    if "exclude_hidden_paths" in config:
+        return True
     if "constraints" in config and not (
-        set(config.keys()) - {"constraints", "exclude", "exclude_hidden_paths"}
+        set(config.keys()) - {"constraints", "exclude"}
     ):
         # This appears to be a project config object,
         # the deprecated version will have a dict of constraints
         return isinstance(config["constraints"], dict)
     return False
 
 
-def flatten_deprecated_config(config: dict[str, Any]):
-    config["constraints"] = [
-        {"tag": key, **value} for key, value in config.get("constraints", {}).items()
-    ]
+def fix_deprecated_config(config: dict[str, Any]):
+    if "constraints" in config and isinstance(config["constraints"], dict):
+        config["constraints"] = [
+            {"tag": key, **value}
+            for key, value in config.get("constraints", {}).items()
+        ]
+    if "exclude_hidden_paths" in config:
+        config.pop("exclude_hidden_paths")
 
 
 class ProjectConfig(Config):
     """
     Configuration applied globally to a project.
     """
 
     constraints: List[TagDependencyRules] = Field(default_factory=list)
     exclude: Optional[List[str]] = Field(default_factory=lambda: ["tests", "docs"])
-    exclude_hidden_paths: bool = True
     exact: bool = False
+    disable_logging: bool = False
     ignore_type_checking_imports: bool = False
 
     def dependencies_for_tag(self, tag: str) -> list[str]:
         return next(
             (
                 constraint.depends_on
                 for constraint in self.constraints
@@ -116,10 +122,10 @@
 
     @classmethod
     def factory(cls, config: dict[str, Any]) -> tuple[bool, "ProjectConfig"]:
         """
         Using this factory to catch deprecated config and flag it to the caller
         """
         if is_deprecated_project_config(config):
-            flatten_deprecated_config(config)
+            fix_deprecated_config(config)
             return True, ProjectConfig(**config)
         return False, ProjectConfig(**config)  # type: ignore
```

### Comparing `tach-0.2.4/tach/core/package.py` & `tach-0.2.5/tach/core/package.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.4/tach/filesystem/__init__.py` & `tach-0.2.5/tach/filesystem/__init__.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.4/tach/filesystem/install.py` & `tach-0.2.5/tach/filesystem/install.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.4/tach/filesystem/project.py` & `tach-0.2.5/tach/filesystem/project.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 def print_no_config_yml() -> None:
     print(
         f"{BCOLORS.FAIL} {CONFIG_FILE_NAME}.(yml|yaml) not found in {os.getcwd()}{BCOLORS.ENDC}",
         file=sys.stderr,
     )
 
 
+# TODO convert all str paths to pathlib.Path
 def get_project_config_path(root: str = ".") -> str:
     file_path = os.path.join(root, f"{CONFIG_FILE_NAME}.yml")
     if os.path.exists(file_path):
         return file_path
     file_path = os.path.join(root, f"{CONFIG_FILE_NAME}.yaml")
     if os.path.exists(file_path):
         return file_path
```

### Comparing `tach-0.2.4/tach/filesystem/service.py` & `tach-0.2.5/tach/filesystem/service.py`

 * *Files 5% similar despite different names*

```diff
@@ -157,28 +157,25 @@
 
 
 def walk(
     root: str,
     depth: Optional[int] = None,
     exclude_root: bool = True,
     exclude_paths: Optional[list[str]] = None,
-    exclude_hidden_paths: Optional[bool] = True,
 ) -> Generator[tuple[str, list[str]], None, None]:
     canonical_root = canonical(root)
     base_depth = 0 if canonical_root == "." else canonical_root.count(os.path.sep) + 1
     for dirpath, dirnames, filenames in os.walk(canonical_root):
         dirpath = canonical(dirpath)
         dirpath_for_matching = f"{dirpath}/"
 
         if exclude_root and dirpath == canonical_root:
             continue
 
-        if exclude_hidden_paths and (
-            os.path.basename(os.path.normpath(dirpath)).startswith(".")
-        ):
+        if os.path.basename(os.path.normpath(dirpath)).startswith("."):
             # This prevents recursing into child directories of hidden paths
             del dirnames[:]
             continue
 
         if exclude_paths is not None and any(
             re.match(exclude_path, dirpath_for_matching)
             for exclude_path in exclude_paths
@@ -189,15 +186,15 @@
         if depth:
             # Ignore anything past requested depth
             current_depth = dirpath.count(os.path.sep)
             if current_depth >= base_depth + depth:
                 continue
 
         def filter_filename(filename: str) -> bool:
-            if exclude_hidden_paths and filename.startswith("."):
+            if filename.startswith("."):
                 return False
             file_path = os.path.join(dirpath, filename)
             if exclude_paths is not None and any(
                 re.match(exclude_path, file_path) for exclude_path in exclude_paths
             ):
                 return False
             return True
@@ -205,55 +202,49 @@
         yield dirpath, list(filter(filter_filename, filenames))
 
 
 def walk_pyfiles(
     root: str,
     depth: Optional[int] = None,
     exclude_paths: Optional[list[str]] = None,
-    exclude_hidden_paths: Optional[bool] = True,
 ) -> Generator[str, None, None]:
     for dirpath, filenames in walk(
         root,
         depth=depth,
         exclude_paths=exclude_paths,
-        exclude_hidden_paths=exclude_hidden_paths,
     ):
         for filename in filenames:
             if filename.endswith(".py"):
                 yield os.path.join(dirpath, filename)
 
 
 def walk_pypackages(
     root: str,
     depth: Optional[int] = None,
     exclude_paths: Optional[list[str]] = None,
-    exclude_hidden_paths: Optional[bool] = True,
 ) -> Generator[str, None, None]:
     for filepath in walk_pyfiles(
         root,
         depth=depth,
         exclude_paths=exclude_paths,
-        exclude_hidden_paths=exclude_hidden_paths,
     ):
         init_file_ending = f"{os.path.sep}__init__.py"
         if filepath.endswith(init_file_ending):
             yield filepath[: -len(init_file_ending)]
 
 
 def walk_configured_packages(
     root: str,
     depth: Optional[int] = None,
     exclude_paths: Optional[list[str]] = None,
-    exclude_hidden_paths: Optional[bool] = True,
 ) -> Generator[tuple[str, str], None, None]:
     for dirpath in walk_pypackages(
         root,
         depth=depth,
         exclude_paths=exclude_paths,
-        exclude_hidden_paths=exclude_hidden_paths,
     ):
         package_yml_path = os.path.join(dirpath, "package.yml")
         if os.path.isfile(package_yml_path):
             yield dirpath, package_yml_path
 
 
 @lru_cache(maxsize=None)
```

### Comparing `tach-0.2.4/tach/interactive/packages.py` & `tach-0.2.5/tach/interactive/packages.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,20 +2,19 @@
 
 import os
 import re
 from collections import deque
 from dataclasses import dataclass, field
 from enum import Enum
 from itertools import chain
-from typing import Callable, Generator, Optional, Union
+from typing import TYPE_CHECKING, Callable, Generator, Optional, Union
 
 from prompt_toolkit import ANSI
 from prompt_toolkit.application import Application
 from prompt_toolkit.data_structures import Point
-from prompt_toolkit.formatted_text import AnyFormattedText
 from prompt_toolkit.key_binding import KeyBindings, KeyPressEvent
 from prompt_toolkit.layout import (
     Container,
     HSplit,
     Layout,
     ScrollablePane,
     VerticalAlign,
@@ -28,14 +27,17 @@
 from rich.text import Text
 from rich.tree import Tree
 
 from tach import errors
 from tach import filesystem as fs
 from tach.constants import PACKAGE_FILE_NAME
 
+if TYPE_CHECKING:
+    from prompt_toolkit.formatted_text import AnyFormattedText
+
 
 @dataclass
 class SelectedPackage:
     full_path: str
 
     @property
     def tags(self) -> list[str]:
```

### Comparing `tach-0.2.4/tach/loading.py` & `tach-0.2.5/tach/loading.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.4/tach/parsing/__init__.py` & `tach-0.2.5/tach/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.4/tach/parsing/config.py` & `tach-0.2.5/tach/parsing/config.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.4/tach/parsing/imports.py` & `tach-0.2.5/tach/parsing/imports.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.4/tach/parsing/interface.py` & `tach-0.2.5/tach/parsing/interface.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.4/tach/parsing/packages.py` & `tach-0.2.5/tach/parsing/packages.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,22 +6,20 @@
 from tach.core import PackageTrie
 from tach.parsing import parse_interface_members, parse_package_config
 
 
 def build_package_trie(
     root: str,
     exclude_paths: Optional[list[str]] = None,
-    exclude_hidden_paths: Optional[bool] = True,
 ) -> PackageTrie:
     package_trie = PackageTrie()
 
     for dir_path, _ in fs.walk_configured_packages(
         root,
         exclude_paths=exclude_paths,
-        exclude_hidden_paths=exclude_hidden_paths,
     ):
         package_config = parse_package_config(dir_path)
         if package_config is None:
             raise ValueError(f"Could not parse package config for {dir_path}")
         package_trie.insert(
             config=package_config,
             path=fs.file_to_module_path(dir_path),
```

### Comparing `tach-0.2.4/tach/pkg.py` & `tach-0.2.5/tach/pkg.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.4/tach/sync.py` & `tach-0.2.5/tach/sync.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.4/tach.egg-info/PKG-INFO` & `tach-0.2.5/tach.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tach
-Version: 0.2.4
+Version: 0.2.5
 Summary: A Python tool to maintain a modular package architecture.
 Author-email: Caelean Barnes <caeleanb@gmail.com>, Evan Doyle <evanmdoyle@gmail.com>
 Project-URL: Homepage, https://github.com/gauge-sh/tach
 Project-URL: Issues, https://github.com/gauge-sh/tach/issues
 Keywords: python,module,package,guard,enforcement,boundary,enforcer,domain,architecture
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -25,14 +25,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyyaml==6.0.1
 Requires-Dist: pydantic==2.7.1
 Requires-Dist: stdlib-list==0.10.0
 Requires-Dist: rich==13.7.1
 Requires-Dist: prompt-toolkit==3.0.43
+Requires-Dist: eval-type-backport==0.2.0
 
 [![image](https://img.shields.io/pypi/v/tach.svg)](https://pypi.Python.org/pypi/tach)
 [![image](https://img.shields.io/pypi/l/tach.svg)](https://pypi.Python.org/pypi/tach)
 [![image](https://img.shields.io/pypi/pyversions/tach.svg)](https://pypi.Python.org/pypi/tach)
 [![image](https://github.com/gauge-sh/tach/actions/workflows/ci.yml/badge.svg)](https://github.com/gauge-sh/tach/actions/workflows/ci.yml)
 [![Checked with pyright](https://microsoft.github.io/pyright/img/pyright_badge.svg)](https://microsoft.github.io/pyright/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
@@ -124,11 +125,11 @@
 Tach also supports:
 - [Manual file configuration](https://gauge-sh.github.io/tach/configuration/)
 - [Strict public interfaces for packages](https://gauge-sh.github.io/tach/strict-mode/)
 - [Inline exceptions](https://gauge-sh.github.io/tach/tach-ignore/)
 - [Pre-commit hooks](https://gauge-sh.github.io/tach/usage/#tach-install)
 
 
-More info in the [docs](https://gauge-sh.github.io/tach/).
-If you have any feedback, we'd love to hear it!
+More info in the [docs](https://gauge-sh.github.io/tach/). Tach logs anonymized usage statistics which are easily [opted out](https://gauge-sh.github.io/tach/faq/) of.
+If you have any feedback, we'd love to talk!
 
 [Discord](https://discord.gg/a58vW8dnmw)
```

### Comparing `tach-0.2.4/tach.egg-info/SOURCES.txt` & `tach-0.2.5/tach.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -28,14 +28,18 @@
 tach/sync.py
 tach.egg-info/PKG-INFO
 tach.egg-info/SOURCES.txt
 tach.egg-info/dependency_links.txt
 tach.egg-info/entry_points.txt
 tach.egg-info/requires.txt
 tach.egg-info/top_level.txt
+tach/cache/__init__.py
+tach/cache/access.py
+tach/cache/package.yml
+tach/cache/setup.py
 tach/colors/__init__.py
 tach/colors/package.yml
 tach/constants/__init__.py
 tach/constants/package.yml
 tach/core/__init__.py
 tach/core/config.py
 tach/core/package.py
@@ -50,14 +54,18 @@
 tach/filesystem/service.py
 tach/hooks/__init__.py
 tach/hooks/package.yml
 tach/hooks/pre_commit.py
 tach/interactive/__init__.py
 tach/interactive/package.yml
 tach/interactive/packages.py
+tach/logging/__init__.py
+tach/logging/api.py
+tach/logging/logger.py
+tach/logging/package.yml
 tach/parsing/__init__.py
 tach/parsing/ast_visitor.py
 tach/parsing/config.py
 tach/parsing/imports.py
 tach/parsing/interface.py
 tach/parsing/package.yml
 tach/parsing/packages.py
```

### Comparing `tach-0.2.4/tests/test_check.py` & `tach-0.2.5/tests/test_check.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.4/tests/test_cli.py` & `tach-0.2.5/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.4/tests/test_init.py` & `tach-0.2.5/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.4/tests/test_package_trie.py` & `tach-0.2.5/tests/test_package_trie.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.4/tests/test_parsing.py` & `tach-0.2.5/tests/test_parsing.py`

 * *Files 23% similar despite different names*

```diff
@@ -23,29 +23,27 @@
     assert result == ProjectConfig(
         constraints=[
             TagDependencyRules(tag="one", depends_on=["two"]),
             TagDependencyRules(tag="two", depends_on=["one"]),
             TagDependencyRules(tag="three", depends_on=[]),
         ],
         exclude=["domain_thr.*"],
-        exclude_hidden_paths=True,
     )
 
 
 def test_run_valid_project_config():
     current_dir = os.getcwd()
     try:
         project = "./example/valid/"
         fs.chdir(project)
         project_config = parse_project_config()
         results = check(
             ".",
             project_config,
             exclude_paths=project_config.exclude,
-            exclude_hidden_paths=project_config.exclude_hidden_paths,
         )
         assert results == []
     finally:
         # Make sure not to dirty the test directory state
         fs.chdir(current_dir)
 
 
@@ -78,29 +76,7 @@
     with pytest.raises(ValidationError):
         parse_package_config("example/invalid")
 
 
 def test_empty_package_config():
     with pytest.raises(ValueError):
         parse_package_config("example/invalid")
-
-
-def test_exclude_hidden_paths_fails():
-    current_dir = os.getcwd()
-    hidden_project = "./example/invalid/hidden/"
-    fs.chdir(hidden_project)
-    try:
-        project_config = parse_project_config()
-        assert project_config.exclude_hidden_paths is False
-        results = check(
-            ".",
-            project_config,
-            exclude_hidden_paths=project_config.exclude_hidden_paths,
-        )
-        assert len(results) == 1
-        assert "strict mode" in results[0].error_info.exception_message
-
-        project_config.exclude_hidden_paths = True
-        assert check(".", project_config, exclude_hidden_paths=True) == []
-    finally:
-        # Make sure not to dirty the test directory state
-        fs.chdir(current_dir)
```

