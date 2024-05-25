# Comparing `tmp/PyFunceble-dev-4.2.7.tar.gz` & `tmp/PyFunceble-dev-4.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyFunceble-dev-4.2.7.tar", last modified: Sun Jan 14 20:46:53 2024, max compression
+gzip compressed data, was "PyFunceble-dev-4.2.9.tar", last modified: Tue Mar 26 16:56:05 2024, max compression
```

## Comparing `PyFunceble-dev-4.2.7.tar` & `PyFunceble-dev-4.2.9.tar`

### file list

```diff
@@ -1,350 +1,350 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:53.100445 PyFunceble-dev-4.2.7/
--rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10796 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12340 2024-01-14 20:46:53.100445 PyFunceble-dev-4.2.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:53.060445 PyFunceble-dev-4.2.7/PyFunceble/
--rw-r--r--   0 runner    (1001) docker     (127)    22813 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:53.060445 PyFunceble-dev-4.2.7/PyFunceble/checker/
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/checker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:53.060445 PyFunceble-dev-4.2.7/PyFunceble/checker/availability/
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/checker/availability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39346 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/checker/availability/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7475 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/checker/availability/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     6603 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/checker/availability/domain_and_ip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:53.064445 PyFunceble-dev-4.2.7/PyFunceble/checker/availability/extras/
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/checker/availability/extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15579 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/checker/availability/extras/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6844 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/checker/availability/extras/dns.py
--rw-r--r--   0 runner    (1001) docker     (127)    10096 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/checker/availability/extras/etoxic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/checker/availability/extras/parked.py
--rw-r--r--   0 runner    (1001) docker     (127)     9859 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/checker/availability/extras/rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/checker/availability/extras/subject_switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     7066 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/checker/availability/ip.py
--rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/checker/availability/params.py
--rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/checker/availability/status.py
--rw-r--r--   0 runner    (1001) docker     (127)    11351 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/checker/availability/url.py
--rw-r--r--   0 runner    (1001) docker     (127)    13677 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/checker/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/checker/complex_json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/checker/params_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:53.064445 PyFunceble-dev-4.2.7/PyFunceble/checker/reputation/
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/checker/reputation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12222 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/checker/reputation/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/checker/reputation/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/checker/reputation/domain_and_ip.py
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/checker/reputation/ip.py
--rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/checker/reputation/params.py
--rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/checker/reputation/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/checker/reputation/url.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/checker/status_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:53.068445 PyFunceble-dev-4.2.7/PyFunceble/checker/syntax/
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/checker/syntax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/checker/syntax/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/checker/syntax/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/checker/syntax/domain_and_ip.py
--rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/checker/syntax/domain_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5614 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/checker/syntax/ip.py
--rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/checker/syntax/ipv4.py
--rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/checker/syntax/ipv6.py
--rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/checker/syntax/params.py
--rw-r--r--   0 runner    (1001) docker     (127)     4706 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/checker/syntax/second_lvl_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/checker/syntax/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/checker/syntax/subdomain.py
--rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/checker/syntax/url.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:53.068445 PyFunceble-dev-4.2.7/PyFunceble/checker/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/checker/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/checker/utils/whois.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:53.068445 PyFunceble-dev-4.2.7/PyFunceble/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:53.068445 PyFunceble-dev-4.2.7/PyFunceble/cli/continuous_integration/
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/continuous_integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38948 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/continuous_integration/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/continuous_integration/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/continuous_integration/github_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/continuous_integration/gitlab_ci.py
--rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/continuous_integration/jenkins.py
--rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/continuous_integration/travis_ci.py
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/continuous_integration/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10606 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/credential_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:53.068445 PyFunceble-dev-4.2.7/PyFunceble/cli/entry_points/
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/entry_points/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5167 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/entry_points/clean.py
--rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/entry_points/iana.py
--rw-r--r--   0 runner    (1001) docker     (127)     5678 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/entry_points/production.py
--rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/entry_points/public_suffix.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:53.068445 PyFunceble-dev-4.2.7/PyFunceble/cli/entry_points/pyfunceble/
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/entry_points/pyfunceble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4762 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/entry_points/pyfunceble/argsparser.py
--rw-r--r--   0 runner    (1001) docker     (127)    45944 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/entry_points/pyfunceble/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/execution_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/facility.py
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    18290 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/file_preloader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:53.072445 PyFunceble-dev-4.2.7/PyFunceble/cli/filesystem/
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/filesystem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/filesystem/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (127)     6977 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/filesystem/counter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/filesystem/dir_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:53.072445 PyFunceble-dev-4.2.7/PyFunceble/cli/filesystem/dir_structure/
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/filesystem/dir_structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/filesystem/dir_structure/backup.py
--rw-r--r--   0 runner    (1001) docker     (127)     5376 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/filesystem/dir_structure/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/filesystem/dir_structure/restore.py
--rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/filesystem/json_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:53.072445 PyFunceble-dev-4.2.7/PyFunceble/cli/filesystem/printer/
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/filesystem/printer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10789 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/filesystem/printer/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6825 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/filesystem/printer/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     7681 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/filesystem/printer/stdout.py
--rw-r--r--   0 runner    (1001) docker     (127)     5738 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/filesystem/registrar_counter.py
--rw-r--r--   0 runner    (1001) docker     (127)    24652 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/filesystem/status_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:53.072445 PyFunceble-dev-4.2.7/PyFunceble/cli/migrators/
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/migrators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7523 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/migrators/alembic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/migrators/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:53.072445 PyFunceble-dev-4.2.7/PyFunceble/cli/migrators/csv_file/
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/migrators/csv_file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5788 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/migrators/csv_file/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/migrators/csv_file/inactive_source_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/migrators/csv_file/whois_registrar_add.py
--rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/migrators/db_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:53.076445 PyFunceble-dev-4.2.7/PyFunceble/cli/migrators/file_cleanup/
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/migrators/file_cleanup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/migrators/file_cleanup/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/migrators/file_cleanup/hashes_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/migrators/file_cleanup/mining_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/migrators/file_cleanup/production_config_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:53.076445 PyFunceble-dev-4.2.7/PyFunceble/cli/migrators/json2csv/
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/migrators/json2csv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/migrators/json2csv/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6159 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/migrators/json2csv/inactive.py
--rw-r--r--   0 runner    (1001) docker     (127)     5700 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/migrators/json2csv/whois.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:53.076445 PyFunceble-dev-4.2.7/PyFunceble/cli/migrators/mariadb/
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/migrators/mariadb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/migrators/mariadb/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7116 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/migrators/mariadb/file_and_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/migrators/mariadb/whois_record_idna_subject.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:53.076445 PyFunceble-dev-4.2.7/PyFunceble/cli/processes/
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/processes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15652 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/processes/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/processes/chancy_producer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/processes/chancy_tester.py
--rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/processes/dir_files_sorter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/processes/file_sorter.py
--rw-r--r--   0 runner    (1001) docker     (127)    16956 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/processes/migrator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/processes/miner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/processes/producer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/processes/tester.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:53.080445 PyFunceble-dev-4.2.7/PyFunceble/cli/processes/workers/
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/processes/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13962 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/processes/workers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/processes/workers/chancy_producer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/processes/workers/chancy_tester.py
--rw-r--r--   0 runner    (1001) docker     (127)     6012 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/processes/workers/dir_files_sorter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4146 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/processes/workers/file_sorter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8042 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/processes/workers/file_sorter_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/processes/workers/migrator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7127 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/processes/workers/miner.py
--rw-r--r--   0 runner    (1001) docker     (127)    16995 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/processes/workers/producer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11751 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/processes/workers/tester.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:53.080445 PyFunceble-dev-4.2.7/PyFunceble/cli/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9991 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/scripts/iana.py
--rw-r--r--   0 runner    (1001) docker     (127)    17919 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/scripts/production.py
--rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/scripts/public_suffix.py
--rw-r--r--   0 runner    (1001) docker     (127)    11886 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/storage_facility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:53.080445 PyFunceble-dev-4.2.7/PyFunceble/cli/system/
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4888 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/system/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9257 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/system/integrator.py
--rw-r--r--   0 runner    (1001) docker     (127)    42782 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/system/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:53.080445 PyFunceble-dev-4.2.7/PyFunceble/cli/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/utils/ascii_logo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/utils/sort.py
--rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/utils/stdout.py
--rw-r--r--   0 runner    (1001) docker     (127)    10214 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (127)    13358 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/cli/utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:53.080445 PyFunceble-dev-4.2.7/PyFunceble/config/
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13047 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/config/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)    14772 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/config/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:53.084445 PyFunceble-dev-4.2.7/PyFunceble/converter/
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12939 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/converter/adblock_input_line2subject.py
--rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/converter/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/converter/cidr2subject.py
--rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/converter/input_line2subject.py
--rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/converter/internal_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/converter/rpz_input_line2subject.py
--rw-r--r--   0 runner    (1001) docker     (127)     9567 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/converter/rpz_policy2subject.py
--rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/converter/subject2complements.py
--rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/converter/url2netloc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/converter/wildcard2subject.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:53.084445 PyFunceble-dev-4.2.7/PyFunceble/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:53.084445 PyFunceble-dev-4.2.7/PyFunceble/data/alembic/
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/data/alembic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:53.084445 PyFunceble-dev-4.2.7/PyFunceble/data/alembic/mysql/
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/data/alembic/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/data/alembic/mysql/env.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/data/alembic/mysql/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:53.084445 PyFunceble-dev-4.2.7/PyFunceble/data/alembic/mysql/versions/
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/data/alembic/mysql/versions/35c79626ecb9_fix_some_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/data/alembic/mysql/versions/3a4c55a9320d_add_continue_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/data/alembic/mysql/versions/3d6f4a33cdb2_add_inactive_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/data/alembic/mysql/versions/45713fea8097_deletion_uneeded_columns_from_whois_.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/data/alembic/mysql/versions/459a0d7b8f09_add_idna_subject_column_into_whois.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/data/alembic/mysql/versions/6f4729deaf03_delete_inactive_source_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/data/alembic/mysql/versions/7bcf7fa64ba1_rename_created_to_created_at_and.py
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/data/alembic/mysql/versions/83ada95132bf_delete_the_file_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/data/alembic/mysql/versions/912bbcb77a6c_add_registrar_column.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/data/alembic/mysql/versions/95dc17ddd729_introduction_of_the_session_id_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/data/alembic/mysql/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/data/alembic/mysql/versions/ade87195b0a0_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/data/alembic/mysql/versions/bef7bcaac3f2_make_id_a_bigint.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/data/alembic/mysql/versions/d8893cd406db_allow_whois_record_to_be_empty_null.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/data/alembic/mysql/versions/e04e8301d1a2_deletion_of_the_mined_table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:53.088445 PyFunceble-dev-4.2.7/PyFunceble/data/alembic/postgresql/
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/data/alembic/postgresql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/data/alembic/postgresql/env.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/data/alembic/postgresql/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:53.088445 PyFunceble-dev-4.2.7/PyFunceble/data/alembic/postgresql/versions/
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/data/alembic/postgresql/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/data/alembic/postgresql/versions/a32ac5d66eee_initial_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:53.088445 PyFunceble-dev-4.2.7/PyFunceble/data/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (127)    11497 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/data/infrastructure/.PyFunceble_production.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/data/infrastructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/data/infrastructure/dir_structure_production.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:53.088445 PyFunceble-dev-4.2.7/PyFunceble/database/
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/database/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:53.088445 PyFunceble-dev-4.2.7/PyFunceble/database/credential/
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/database/credential/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12180 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/database/credential/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/database/credential/mariadb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/database/credential/mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/database/credential/postgresql.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:53.088445 PyFunceble-dev-4.2.7/PyFunceble/database/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/database/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/database/schemas/autocontinue.py
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/database/schemas/inactive.py
--rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/database/schemas/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/database/schemas/whois_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     7503 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/database/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:53.088445 PyFunceble-dev-4.2.7/PyFunceble/database/sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/database/sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/database/sqlalchemy/all_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/database/sqlalchemy/base_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:53.092445 PyFunceble-dev-4.2.7/PyFunceble/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/dataset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:53.092445 PyFunceble-dev-4.2.7/PyFunceble/dataset/autocontinue/
--rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/dataset/autocontinue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/dataset/autocontinue/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/dataset/autocontinue/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/dataset/autocontinue/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/dataset/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9688 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/dataset/csv_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9417 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/dataset/db_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/dataset/iana.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:53.092445 PyFunceble-dev-4.2.7/PyFunceble/dataset/inactive/
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/dataset/inactive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/dataset/inactive/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4012 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/dataset/inactive/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/dataset/inactive/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/dataset/ipv4_reputation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/dataset/public_suffix.py
--rw-r--r--   0 runner    (1001) docker     (127)    10535 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/dataset/sql_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8052 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/dataset/user_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:53.092445 PyFunceble-dev-4.2.7/PyFunceble/dataset/whois/
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/dataset/whois/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/dataset/whois/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/dataset/whois/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     6261 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/dataset/whois/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:53.092445 PyFunceble-dev-4.2.7/PyFunceble/downloader/
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8849 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/downloader/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/downloader/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/downloader/iana.py
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/downloader/ipv4_reputation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/downloader/public_suffix.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/downloader/user_agents.py
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/facility.py
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:53.096445 PyFunceble-dev-4.2.7/PyFunceble/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7644 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/helpers/command.py
--rw-r--r--   0 runner    (1001) docker     (127)    13783 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/helpers/dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     5990 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/helpers/directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     7491 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/helpers/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     7327 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/helpers/environment_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/helpers/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/helpers/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/helpers/hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/helpers/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     6060 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/helpers/merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     6937 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/helpers/regex.py
--rw-r--r--   0 runner    (1001) docker     (127)    16829 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:53.096445 PyFunceble-dev-4.2.7/PyFunceble/query/
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20321 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/query/collection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:53.096445 PyFunceble-dev-4.2.7/PyFunceble/query/dns/
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/query/dns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9796 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/query/dns/nameserver.py
--rw-r--r--   0 runner    (1001) docker     (127)    32795 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/query/dns/query_tool.py
--rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/query/dns/resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)    11777 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/query/http_status_code.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:53.096445 PyFunceble-dev-4.2.7/PyFunceble/query/netinfo/
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/query/netinfo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/query/netinfo/address.py
--rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/query/netinfo/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/query/netinfo/hostbyaddr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:53.096445 PyFunceble-dev-4.2.7/PyFunceble/query/record/
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/query/record/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/query/record/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/query/record/dns.py
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/query/record/whois.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:53.096445 PyFunceble-dev-4.2.7/PyFunceble/query/requests/
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/query/requests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:53.100445 PyFunceble-dev-4.2.7/PyFunceble/query/requests/adapter/
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/query/requests/adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9581 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/query/requests/adapter/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5667 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/query/requests/adapter/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     6142 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/query/requests/adapter/https.py
--rw-r--r--   0 runner    (1001) docker     (127)    18042 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/query/requests/requester.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:53.100445 PyFunceble-dev-4.2.7/PyFunceble/query/whois/
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/query/whois/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:53.100445 PyFunceble-dev-4.2.7/PyFunceble/query/whois/converter/
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/query/whois/converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/query/whois/converter/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/query/whois/converter/digit2digits.py
--rw-r--r--   0 runner    (1001) docker     (127)    13426 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/query/whois/converter/expiration_date.py
--rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/query/whois/converter/month2unified.py
--rw-r--r--   0 runner    (1001) docker     (127)     4735 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/query/whois/converter/registrar.py
--rw-r--r--   0 runner    (1001) docker     (127)    14658 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/query/whois/query_tool.py
--rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6290 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4833 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/storage_facility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:53.100445 PyFunceble-dev-4.2.7/PyFunceble/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3920 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/utils/platform.py
--rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/utils/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     8330 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/PyFunceble/utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 20:46:53.100445 PyFunceble-dev-4.2.7/PyFunceble_dev.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12340 2024-01-14 20:46:53.000000 PyFunceble-dev-4.2.7/PyFunceble_dev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11861 2024-01-14 20:46:53.000000 PyFunceble-dev-4.2.7/PyFunceble_dev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-14 20:46:53.000000 PyFunceble-dev-4.2.7/PyFunceble_dev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-01-14 20:46:53.000000 PyFunceble-dev-4.2.7/PyFunceble_dev.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-01-14 20:46:53.000000 PyFunceble-dev-4.2.7/PyFunceble_dev.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-01-14 20:46:53.000000 PyFunceble-dev-4.2.7/PyFunceble_dev.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11295 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/requirements.dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/requirements.docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/requirements.test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/requirements.win.txt
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-01-14 20:46:53.100445 PyFunceble-dev-4.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    10898 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-01-14 20:46:42.000000 PyFunceble-dev-4.2.7/version.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:56:05.478598 PyFunceble-dev-4.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10796 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12340 2024-03-26 16:56:05.478598 PyFunceble-dev-4.2.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:56:05.434597 PyFunceble-dev-4.2.9/PyFunceble/
+-rw-r--r--   0 runner    (1001) docker     (127)    22813 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:56:05.434597 PyFunceble-dev-4.2.9/PyFunceble/checker/
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/checker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:56:05.438597 PyFunceble-dev-4.2.9/PyFunceble/checker/availability/
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/checker/availability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39105 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/checker/availability/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7474 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/checker/availability/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6603 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/checker/availability/domain_and_ip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:56:05.438597 PyFunceble-dev-4.2.9/PyFunceble/checker/availability/extras/
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/checker/availability/extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15583 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/checker/availability/extras/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6844 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/checker/availability/extras/dns.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10096 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/checker/availability/extras/etoxic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/checker/availability/extras/parked.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9866 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/checker/availability/extras/rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/checker/availability/extras/subject_switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7065 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/checker/availability/ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/checker/availability/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/checker/availability/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11350 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/checker/availability/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13677 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/checker/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/checker/complex_json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/checker/params_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:56:05.438597 PyFunceble-dev-4.2.9/PyFunceble/checker/reputation/
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/checker/reputation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12221 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/checker/reputation/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/checker/reputation/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/checker/reputation/domain_and_ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/checker/reputation/ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/checker/reputation/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/checker/reputation/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/checker/reputation/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/checker/status_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:56:05.442597 PyFunceble-dev-4.2.9/PyFunceble/checker/syntax/
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/checker/syntax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/checker/syntax/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/checker/syntax/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/checker/syntax/domain_and_ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/checker/syntax/domain_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5614 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/checker/syntax/ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/checker/syntax/ipv4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/checker/syntax/ipv6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/checker/syntax/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/checker/syntax/second_lvl_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/checker/syntax/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/checker/syntax/subdomain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/checker/syntax/url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:56:05.442597 PyFunceble-dev-4.2.9/PyFunceble/checker/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/checker/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/checker/utils/whois.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:56:05.442597 PyFunceble-dev-4.2.9/PyFunceble/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:56:05.442597 PyFunceble-dev-4.2.9/PyFunceble/cli/continuous_integration/
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/continuous_integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38948 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/continuous_integration/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/continuous_integration/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/continuous_integration/github_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/continuous_integration/gitlab_ci.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/continuous_integration/jenkins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/continuous_integration/travis_ci.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/continuous_integration/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10606 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/credential_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:56:05.446597 PyFunceble-dev-4.2.9/PyFunceble/cli/entry_points/
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/entry_points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5167 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/entry_points/clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/entry_points/iana.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5678 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/entry_points/production.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/entry_points/public_suffix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:56:05.446597 PyFunceble-dev-4.2.9/PyFunceble/cli/entry_points/pyfunceble/
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/entry_points/pyfunceble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4762 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/entry_points/pyfunceble/argsparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45944 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/entry_points/pyfunceble/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/execution_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/facility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18292 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/file_preloader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:56:05.446597 PyFunceble-dev-4.2.9/PyFunceble/cli/filesystem/
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/filesystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/filesystem/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6977 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/filesystem/counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/filesystem/dir_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:56:05.446597 PyFunceble-dev-4.2.9/PyFunceble/cli/filesystem/dir_structure/
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/filesystem/dir_structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/filesystem/dir_structure/backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5376 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/filesystem/dir_structure/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/filesystem/dir_structure/restore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/filesystem/json_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:56:05.446597 PyFunceble-dev-4.2.9/PyFunceble/cli/filesystem/printer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/filesystem/printer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10789 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/filesystem/printer/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6825 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/filesystem/printer/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7681 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/filesystem/printer/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5738 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/filesystem/registrar_counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24652 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/filesystem/status_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:56:05.446597 PyFunceble-dev-4.2.9/PyFunceble/cli/migrators/
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/migrators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7523 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/migrators/alembic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/migrators/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:56:05.450597 PyFunceble-dev-4.2.9/PyFunceble/cli/migrators/csv_file/
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/migrators/csv_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5788 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/migrators/csv_file/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/migrators/csv_file/inactive_source_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/migrators/csv_file/whois_registrar_add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/migrators/db_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:56:05.450597 PyFunceble-dev-4.2.9/PyFunceble/cli/migrators/file_cleanup/
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/migrators/file_cleanup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/migrators/file_cleanup/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/migrators/file_cleanup/hashes_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/migrators/file_cleanup/mining_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/migrators/file_cleanup/production_config_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:56:05.450597 PyFunceble-dev-4.2.9/PyFunceble/cli/migrators/json2csv/
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/migrators/json2csv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/migrators/json2csv/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6159 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/migrators/json2csv/inactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5700 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/migrators/json2csv/whois.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:56:05.450597 PyFunceble-dev-4.2.9/PyFunceble/cli/migrators/mariadb/
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/migrators/mariadb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/migrators/mariadb/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7116 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/migrators/mariadb/file_and_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/migrators/mariadb/whois_record_idna_subject.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:56:05.450597 PyFunceble-dev-4.2.9/PyFunceble/cli/processes/
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/processes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15652 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/processes/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/processes/chancy_producer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/processes/chancy_tester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/processes/dir_files_sorter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/processes/file_sorter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16956 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/processes/migrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/processes/miner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/processes/producer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/processes/tester.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:56:05.454598 PyFunceble-dev-4.2.9/PyFunceble/cli/processes/workers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/processes/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13964 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/processes/workers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/processes/workers/chancy_producer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/processes/workers/chancy_tester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6012 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/processes/workers/dir_files_sorter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4146 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/processes/workers/file_sorter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8042 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/processes/workers/file_sorter_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/processes/workers/migrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7127 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/processes/workers/miner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16995 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/processes/workers/producer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11751 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/processes/workers/tester.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:56:05.454598 PyFunceble-dev-4.2.9/PyFunceble/cli/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9991 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/scripts/iana.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17920 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/scripts/production.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/scripts/public_suffix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11910 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/storage_facility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:56:05.454598 PyFunceble-dev-4.2.9/PyFunceble/cli/system/
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4888 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/system/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9257 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/system/integrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42782 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/system/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:56:05.454598 PyFunceble-dev-4.2.9/PyFunceble/cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/utils/ascii_logo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/utils/sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/utils/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10198 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13358 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/cli/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:56:05.458598 PyFunceble-dev-4.2.9/PyFunceble/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13047 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/config/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14772 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/config/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:56:05.458598 PyFunceble-dev-4.2.9/PyFunceble/converter/
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12939 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/converter/adblock_input_line2subject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/converter/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/converter/cidr2subject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/converter/input_line2subject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/converter/internal_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/converter/rpz_input_line2subject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9567 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/converter/rpz_policy2subject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/converter/subject2complements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/converter/url2netloc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/converter/wildcard2subject.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:56:05.458598 PyFunceble-dev-4.2.9/PyFunceble/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:56:05.458598 PyFunceble-dev-4.2.9/PyFunceble/data/alembic/
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/data/alembic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:56:05.458598 PyFunceble-dev-4.2.9/PyFunceble/data/alembic/mysql/
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/data/alembic/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/data/alembic/mysql/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/data/alembic/mysql/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:56:05.462598 PyFunceble-dev-4.2.9/PyFunceble/data/alembic/mysql/versions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/data/alembic/mysql/versions/35c79626ecb9_fix_some_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/data/alembic/mysql/versions/3a4c55a9320d_add_continue_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/data/alembic/mysql/versions/3d6f4a33cdb2_add_inactive_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/data/alembic/mysql/versions/45713fea8097_deletion_uneeded_columns_from_whois_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/data/alembic/mysql/versions/459a0d7b8f09_add_idna_subject_column_into_whois.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/data/alembic/mysql/versions/6f4729deaf03_delete_inactive_source_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/data/alembic/mysql/versions/7bcf7fa64ba1_rename_created_to_created_at_and.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/data/alembic/mysql/versions/83ada95132bf_delete_the_file_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/data/alembic/mysql/versions/912bbcb77a6c_add_registrar_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/data/alembic/mysql/versions/95dc17ddd729_introduction_of_the_session_id_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/data/alembic/mysql/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/data/alembic/mysql/versions/ade87195b0a0_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/data/alembic/mysql/versions/bef7bcaac3f2_make_id_a_bigint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/data/alembic/mysql/versions/d8893cd406db_allow_whois_record_to_be_empty_null.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/data/alembic/mysql/versions/e04e8301d1a2_deletion_of_the_mined_table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:56:05.462598 PyFunceble-dev-4.2.9/PyFunceble/data/alembic/postgresql/
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/data/alembic/postgresql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/data/alembic/postgresql/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/data/alembic/postgresql/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:56:05.462598 PyFunceble-dev-4.2.9/PyFunceble/data/alembic/postgresql/versions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/data/alembic/postgresql/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/data/alembic/postgresql/versions/a32ac5d66eee_initial_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:56:05.462598 PyFunceble-dev-4.2.9/PyFunceble/data/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (127)    11497 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/data/infrastructure/.PyFunceble_production.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/data/infrastructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/data/infrastructure/dir_structure_production.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:56:05.462598 PyFunceble-dev-4.2.9/PyFunceble/database/
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/database/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:56:05.462598 PyFunceble-dev-4.2.9/PyFunceble/database/credential/
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/database/credential/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12180 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/database/credential/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/database/credential/mariadb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/database/credential/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/database/credential/postgresql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:56:05.462598 PyFunceble-dev-4.2.9/PyFunceble/database/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/database/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/database/schemas/autocontinue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/database/schemas/inactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/database/schemas/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/database/schemas/whois_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7503 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/database/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:56:05.466598 PyFunceble-dev-4.2.9/PyFunceble/database/sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/database/sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/database/sqlalchemy/all_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/database/sqlalchemy/base_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:56:05.466598 PyFunceble-dev-4.2.9/PyFunceble/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/dataset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:56:05.466598 PyFunceble-dev-4.2.9/PyFunceble/dataset/autocontinue/
+-rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/dataset/autocontinue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/dataset/autocontinue/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/dataset/autocontinue/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/dataset/autocontinue/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/dataset/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9688 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/dataset/csv_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9417 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/dataset/db_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/dataset/iana.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:56:05.466598 PyFunceble-dev-4.2.9/PyFunceble/dataset/inactive/
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/dataset/inactive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/dataset/inactive/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4012 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/dataset/inactive/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/dataset/inactive/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/dataset/ipv4_reputation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/dataset/public_suffix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10535 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/dataset/sql_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8052 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/dataset/user_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:56:05.466598 PyFunceble-dev-4.2.9/PyFunceble/dataset/whois/
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/dataset/whois/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/dataset/whois/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/dataset/whois/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6261 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/dataset/whois/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:56:05.470598 PyFunceble-dev-4.2.9/PyFunceble/downloader/
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8849 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/downloader/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/downloader/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/downloader/iana.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/downloader/ipv4_reputation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/downloader/public_suffix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/downloader/user_agents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/facility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:56:05.470598 PyFunceble-dev-4.2.9/PyFunceble/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7644 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/helpers/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13783 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/helpers/dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5990 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/helpers/directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7491 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/helpers/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7327 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/helpers/environment_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/helpers/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/helpers/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/helpers/hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/helpers/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6060 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/helpers/merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6937 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/helpers/regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16829 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:56:05.470598 PyFunceble-dev-4.2.9/PyFunceble/query/
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22748 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/query/collection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:56:05.470598 PyFunceble-dev-4.2.9/PyFunceble/query/dns/
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/query/dns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9796 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/query/dns/nameserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32795 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/query/dns/query_tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/query/dns/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11777 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/query/http_status_code.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:56:05.470598 PyFunceble-dev-4.2.9/PyFunceble/query/netinfo/
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/query/netinfo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/query/netinfo/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/query/netinfo/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/query/netinfo/hostbyaddr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:56:05.474598 PyFunceble-dev-4.2.9/PyFunceble/query/record/
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/query/record/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/query/record/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/query/record/dns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/query/record/whois.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:56:05.474598 PyFunceble-dev-4.2.9/PyFunceble/query/requests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/query/requests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:56:05.474598 PyFunceble-dev-4.2.9/PyFunceble/query/requests/adapter/
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/query/requests/adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9581 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/query/requests/adapter/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5667 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/query/requests/adapter/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/query/requests/adapter/https.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18042 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/query/requests/requester.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:56:05.474598 PyFunceble-dev-4.2.9/PyFunceble/query/whois/
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/query/whois/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:56:05.474598 PyFunceble-dev-4.2.9/PyFunceble/query/whois/converter/
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/query/whois/converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/query/whois/converter/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/query/whois/converter/digit2digits.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13426 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/query/whois/converter/expiration_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/query/whois/converter/month2unified.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4735 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/query/whois/converter/registrar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14658 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/query/whois/query_tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6298 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4833 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/storage_facility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:56:05.474598 PyFunceble-dev-4.2.9/PyFunceble/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3920 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/utils/platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/utils/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8330 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/PyFunceble/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:56:05.474598 PyFunceble-dev-4.2.9/PyFunceble_dev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12340 2024-03-26 16:56:05.000000 PyFunceble-dev-4.2.9/PyFunceble_dev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11861 2024-03-26 16:56:05.000000 PyFunceble-dev-4.2.9/PyFunceble_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 16:56:05.000000 PyFunceble-dev-4.2.9/PyFunceble_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-26 16:56:05.000000 PyFunceble-dev-4.2.9/PyFunceble_dev.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-03-26 16:56:05.000000 PyFunceble-dev-4.2.9/PyFunceble_dev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-26 16:56:05.000000 PyFunceble-dev-4.2.9/PyFunceble_dev.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11295 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/requirements.dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/requirements.docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/requirements.test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/requirements.win.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-03-26 16:56:05.478598 PyFunceble-dev-4.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    10898 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-03-26 16:55:56.000000 PyFunceble-dev-4.2.9/version.yaml
```

### Comparing `PyFunceble-dev-4.2.7/CODE_OF_CONDUCT.rst` & `PyFunceble-dev-4.2.9/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/CONTRIBUTING.rst` & `PyFunceble-dev-4.2.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/LICENSE` & `PyFunceble-dev-4.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PKG-INFO` & `PyFunceble-dev-4.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFunceble-dev
-Version: 4.2.7
+Version: 4.2.9
 Summary: The tool to check the availability or syntax of domain, IP or URL.
 Home-page: https://github.com/funilrys/PyFunceble
 Author: funilrys
 Author-email: contact@funilrys.com
 License: Apache 2.0
 Project-URL: Documentation, https://pyfunceble.readthedocs.io/en/dev/
 Project-URL: Funding, https://github.com/sponsors/funilrys
```

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/__init__.py` & `PyFunceble-dev-4.2.9/PyFunceble/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/checker/__init__.py` & `PyFunceble-dev-4.2.9/PyFunceble/checker/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/checker/availability/__init__.py` & `PyFunceble-dev-4.2.9/PyFunceble/checker/availability/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/checker/availability/base.py` & `PyFunceble-dev-4.2.9/PyFunceble/checker/availability/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,14 @@
 from PyFunceble.checker.availability.params import AvailabilityCheckerParams
 from PyFunceble.checker.availability.status import AvailabilityCheckerStatus
 from PyFunceble.checker.base import CheckerBase
 from PyFunceble.checker.syntax.domain import DomainSyntaxChecker
 from PyFunceble.checker.syntax.ip import IPSyntaxChecker
 from PyFunceble.checker.syntax.url import URLSyntaxChecker
 from PyFunceble.converter.url2netloc import Url2Netloc
-from PyFunceble.helpers.regex import RegexHelper
 from PyFunceble.query.dns.query_tool import DNSQueryTool
 from PyFunceble.query.http_status_code import HTTPStatusCode
 from PyFunceble.query.netinfo.address import AddressInfo
 from PyFunceble.query.netinfo.hostbyaddr import HostByAddrInfo
 from PyFunceble.query.whois.query_tool import WhoisQueryTool
 
 
@@ -915,20 +914,15 @@
             "Started to try to query the status of %r from: HTTP Status code Lookup",
             self.status.idna_subject,
         )
 
         if from_domain_test and self.status.url_syntax:
             return self
 
-        if not self.status.url_syntax and not RegexHelper("[^a-z0-9._]").match(
-            self.idna_subject, return_match=False
-        ):
-            # The regex is there because while testing for domain, sometime we
-            # may see something like mailto:xxx@yyy.de
-
+        if not self.status.url_syntax and not self.idna_subject.startswith("http"):
             self.http_status_code_query_tool.set_subject(
                 f"http://{self.idna_subject}:80"
             )
 
         lookup_result = self.http_status_code_query_tool.get_status_code()
 
         if (
```

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/checker/availability/domain.py` & `PyFunceble-dev-4.2.9/PyFunceble/checker/availability/domain.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,14 @@
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
-
 import PyFunceble.facility
 import PyFunceble.factory
 import PyFunceble.storage
 from PyFunceble.checker.availability.base import AvailabilityCheckerBase
 from PyFunceble.checker.reputation.domain import DomainReputationChecker
```

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/checker/availability/domain_and_ip.py` & `PyFunceble-dev-4.2.9/PyFunceble/checker/availability/domain_and_ip.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/checker/availability/extras/__init__.py` & `PyFunceble-dev-4.2.9/PyFunceble/checker/availability/extras/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/checker/availability/extras/base.py` & `PyFunceble-dev-4.2.9/PyFunceble/checker/availability/extras/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,14 @@
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
-
 import functools
 import socket
 from typing import Callable, Dict, List, Optional, Union
 
 import requests
 
 import PyFunceble.factory
@@ -419,15 +418,15 @@
         self, status_code: Union[int, List[int]]
     ) -> "ExtraRuleHandlerBase":
         """
         Switches the status to inactive if the caught status code matches one
         of the given one.
         """
 
-        if not isinstance(status_code, (list, tuple)):
+        if not isinstance(status_code, (list, tuple, set)):
             status_code = [status_code]
 
         if any(self.status.http_status_code == x for x in status_code):
             self.switch_to_down()
 
         return self
```

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/checker/availability/extras/dns.py` & `PyFunceble-dev-4.2.9/PyFunceble/checker/availability/extras/dns.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/checker/availability/extras/etoxic.py` & `PyFunceble-dev-4.2.9/PyFunceble/checker/availability/extras/etoxic.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/checker/availability/extras/parked.py` & `PyFunceble-dev-4.2.9/PyFunceble/checker/availability/extras/parked.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/checker/availability/extras/rules.py` & `PyFunceble-dev-4.2.9/PyFunceble/checker/availability/extras/rules.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
     regex_active2inactive: dict = {}
     http_codes_dataset: Optional[Box] = None
 
     def __init__(self, status: Optional[AvailabilityCheckerStatus] = None) -> None:
         self.regex_active2inactive = {
             r"\.000webhostapp\.com": [
-                (self.switch_to_down_if_status_code, 410),
+                (self.switch_to_down_if_status_code, {410, 424}),
             ],
             r"\.24\.eu$": [(self.switch_to_down_if_status_code, 503)],
             r"\.altervista\.org$": [(self.switch_to_down_if_status_code, 403)],
             r"\.angelfire\.com$": [(self.switch_to_down_if_status_code, 404)],
             r"\.blogspot\.": [self.handle_blogspot],
             r"\.canalblog\.com$": [(self.switch_to_down_if_status_code, 404)],
             r"\.dr\.ag$": [(self.switch_to_down_if_status_code, 503)],
```

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/checker/availability/extras/subject_switch.py` & `PyFunceble-dev-4.2.9/PyFunceble/checker/availability/extras/subject_switch.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/checker/availability/ip.py` & `PyFunceble-dev-4.2.9/PyFunceble/checker/availability/ip.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,14 @@
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
-
 import PyFunceble.facility
 import PyFunceble.factory
 import PyFunceble.storage
 from PyFunceble.checker.availability.base import AvailabilityCheckerBase
 from PyFunceble.checker.reputation.ip import IPReputationChecker
```

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/checker/availability/params.py` & `PyFunceble-dev-4.2.9/PyFunceble/checker/availability/params.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/checker/availability/status.py` & `PyFunceble-dev-4.2.9/PyFunceble/checker/availability/status.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/checker/availability/url.py` & `PyFunceble-dev-4.2.9/PyFunceble/checker/availability/url.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,14 @@
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
-
 import PyFunceble.facility
 import PyFunceble.factory
 import PyFunceble.storage
 from PyFunceble.checker.availability.base import AvailabilityCheckerBase
 from PyFunceble.checker.availability.status import AvailabilityCheckerStatus
 from PyFunceble.checker.reputation.url import URLReputationChecker
 from PyFunceble.checker.syntax.url import URLSyntaxChecker
```

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/checker/base.py` & `PyFunceble-dev-4.2.9/PyFunceble/checker/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/checker/complex_json_encoder.py` & `PyFunceble-dev-4.2.9/PyFunceble/checker/complex_json_encoder.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/checker/params_base.py` & `PyFunceble-dev-4.2.9/PyFunceble/checker/params_base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/checker/reputation/__init__.py` & `PyFunceble-dev-4.2.9/PyFunceble/checker/reputation/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/checker/reputation/base.py` & `PyFunceble-dev-4.2.9/PyFunceble/checker/reputation/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,14 @@
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
-
 from typing import List, Optional
 
 from sqlalchemy.orm import Session
 
 import PyFunceble.facility
 import PyFunceble.factory
 import PyFunceble.storage
```

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/checker/reputation/domain.py` & `PyFunceble-dev-4.2.9/PyFunceble/checker/reputation/domain.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,14 @@
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
-
 from typing import List, Optional
 
 from PyFunceble.checker.reputation.base import ReputationCheckerBase
 
 
 class DomainReputationChecker(ReputationCheckerBase):
     """
```

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/checker/reputation/domain_and_ip.py` & `PyFunceble-dev-4.2.9/PyFunceble/checker/reputation/domain_and_ip.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/checker/reputation/ip.py` & `PyFunceble-dev-4.2.9/PyFunceble/checker/reputation/ip.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,14 @@
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
-
 from typing import List, Optional
 
 from PyFunceble.checker.reputation.base import ReputationCheckerBase
 
 
 class IPReputationChecker(ReputationCheckerBase):
     """
```

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/checker/reputation/params.py` & `PyFunceble-dev-4.2.9/PyFunceble/checker/reputation/params.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/checker/reputation/status.py` & `PyFunceble-dev-4.2.9/PyFunceble/checker/reputation/status.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/checker/reputation/url.py` & `PyFunceble-dev-4.2.9/PyFunceble/checker/reputation/url.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,14 @@
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
-
 from typing import List, Optional
 
 from PyFunceble.checker.reputation.base import ReputationCheckerBase
 from PyFunceble.checker.syntax.ip import IPSyntaxChecker
 from PyFunceble.converter.url2netloc import Url2Netloc
```

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/checker/status_base.py` & `PyFunceble-dev-4.2.9/PyFunceble/checker/status_base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/checker/syntax/__init__.py` & `PyFunceble-dev-4.2.9/PyFunceble/checker/syntax/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/checker/syntax/base.py` & `PyFunceble-dev-4.2.9/PyFunceble/checker/syntax/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/checker/syntax/domain.py` & `PyFunceble-dev-4.2.9/PyFunceble/checker/syntax/domain.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/checker/syntax/domain_and_ip.py` & `PyFunceble-dev-4.2.9/PyFunceble/checker/syntax/domain_and_ip.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/checker/syntax/domain_base.py` & `PyFunceble-dev-4.2.9/PyFunceble/checker/syntax/domain_base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/checker/syntax/ip.py` & `PyFunceble-dev-4.2.9/PyFunceble/checker/syntax/ip.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/checker/syntax/ipv4.py` & `PyFunceble-dev-4.2.9/PyFunceble/checker/syntax/ipv4.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/checker/syntax/ipv6.py` & `PyFunceble-dev-4.2.9/PyFunceble/checker/syntax/ipv6.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/checker/syntax/params.py` & `PyFunceble-dev-4.2.9/PyFunceble/checker/syntax/params.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/checker/syntax/second_lvl_domain.py` & `PyFunceble-dev-4.2.9/PyFunceble/checker/syntax/second_lvl_domain.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,16 +61,20 @@
     Provides an interface to check the syntax of a second domain.
 
     :param str subject:
         Optional, The subject to work with.
     """
 
     # pylint: disable=line-too-long
-    REGEX_VALID_DOMAIN: str = r"^(?=.{0,253}$)(([a-z0-9][a-z0-9-]{0,61}[a-z0-9]|[a-z0-9])\.)+((?=.*[^0-9])([a-z0-9][a-z0-9-]{0,61}[a-z0-9](?:\.)?|[a-z0-9](?:\.)?))$"
-    REGEX_VALID_RELAXED_DOMAIN: str = r"^(?=.{0,253}$)(([a-z0-9][a-z0-9_-]{0,61}[a-z0-9_-]|[a-z0-9])\.)+((?=.*[^0-9])([a-z0-9][a-z0-9-]{0,61}[a-z0-9](?:\.)?|[a-z0-9](?:\.)?))$"
+    REGEX_VALID_DOMAIN: str = (
+        r"^(?=.{0,253}$)(([a-z0-9][a-z0-9-]{0,61}[a-z0-9]|[a-z0-9])\.)+((?=.*[^0-9])([a-z0-9][a-z0-9-]{0,61}[a-z0-9](?:\.)?|[a-z0-9](?:\.)?))$"
+    )
+    REGEX_VALID_RELAXED_DOMAIN: str = (
+        r"^(?=.{0,253}$)(([a-z0-9][a-z0-9_-]{0,61}[a-z0-9_-]|[a-z0-9])\.)+((?=.*[^0-9])([a-z0-9][a-z0-9-]{0,61}[a-z0-9](?:\.)?|[a-z0-9](?:\.)?))$"
+    )
 
     last_point_index: Optional[int] = None
     """
     Saves the index of the last point.
     """
 
     @DomainSyntaxCheckerBase.ensure_subject_is_given
```

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/checker/syntax/status.py` & `PyFunceble-dev-4.2.9/PyFunceble/checker/syntax/status.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
+
 import dataclasses
 from typing import Optional
 
 import PyFunceble.storage
 from PyFunceble.checker.status_base import CheckerStatusBase
```

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/checker/syntax/subdomain.py` & `PyFunceble-dev-4.2.9/PyFunceble/checker/syntax/subdomain.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,17 @@
     Provides an interface to check the syntax of a subdomain.
 
     :param str subject:
         Optional, The subject to work with.
     """
 
     # pylint: disable=line-too-long
-    REGEX_VALID_SUBDOMAIN: str = r"^(?=.{0,253}$)(([a-z0-9_][a-z0-9-_]{0,61}[a-z0-9_-]|[a-z0-9])\.)+((?=.*)([a-z0-9][a-z0-9-]{0,61}[a-z0-9](?:\.)?|[a-z0-9](?:\.)?))$"
+    REGEX_VALID_SUBDOMAIN: str = (
+        r"^(?=.{0,253}$)(([a-z0-9_][a-z0-9-_]{0,61}[a-z0-9_-]|[a-z0-9])\.)+((?=.*)([a-z0-9][a-z0-9-]{0,61}[a-z0-9](?:\.)?|[a-z0-9](?:\.)?))$"
+    )
 
     @DomainSyntaxCheckerBase.ensure_subject_is_given
     def is_valid(self) -> bool:
         """
         Validate the given subject if exists.
         """
```

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/checker/syntax/url.py` & `PyFunceble-dev-4.2.9/PyFunceble/checker/syntax/url.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,14 @@
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
-
 import urllib.parse
 from typing import Optional
 
 from PyFunceble.checker.base import CheckerBase
 from PyFunceble.checker.syntax.base import SyntaxCheckerBase
 from PyFunceble.checker.syntax.domain import DomainSyntaxChecker
 from PyFunceble.checker.syntax.ip import IPSyntaxChecker
```

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/checker/utils/__init__.py` & `PyFunceble-dev-4.2.9/PyFunceble/checker/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/checker/utils/whois.py` & `PyFunceble-dev-4.2.9/PyFunceble/checker/utils/whois.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/__init__.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/continuous_integration/__init__.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/continuous_integration/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/continuous_integration/base.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/continuous_integration/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/continuous_integration/exceptions.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/continuous_integration/exceptions.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/continuous_integration/github_actions.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/continuous_integration/github_actions.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/continuous_integration/gitlab_ci.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/continuous_integration/gitlab_ci.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/continuous_integration/jenkins.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/continuous_integration/jenkins.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/continuous_integration/travis_ci.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/continuous_integration/travis_ci.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/continuous_integration/utils.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/continuous_integration/utils.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/credential_loader.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/credential_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -262,17 +262,17 @@
             Ignore questions to end-user.
         """
 
         if not isinstance(self.credential, CredentialBase) and self.authorized:
             # We directly share the credential object into the DBSession object.
             # This will let us use the DBSession without having to think about
             # any other headache.
-            self.credential = (
-                PyFunceble.cli.factory.DBSession.credential
-            ) = self.DB_TYPE2OBJ[self.db_type]()
+            self.credential = PyFunceble.cli.factory.DBSession.credential = (
+                self.DB_TYPE2OBJ[self.db_type]()
+            )
 
             env_var_helper = EnvironmentVariableHelper(
                 env_file_path=self.credential.get_dot_env_file()
             )
 
             for cred_var, env_var in self.credential.VAR2ENV.items():
                 if env_var_helper.set_name(env_var).exists():
```

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/entry_points/__init__.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/entry_points/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/entry_points/clean.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/entry_points/clean.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/entry_points/iana.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/entry_points/iana.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/entry_points/production.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/entry_points/production.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/entry_points/public_suffix.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/entry_points/public_suffix.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/entry_points/pyfunceble/__init__.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/entry_points/pyfunceble/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/entry_points/pyfunceble/argsparser.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/entry_points/pyfunceble/argsparser.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/entry_points/pyfunceble/cli.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/entry_points/pyfunceble/cli.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/execution_time.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/execution_time.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/facility.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/facility.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/factory.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/factory.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/file_preloader.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/file_preloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -477,14 +477,14 @@
                         self.__description[self.__matching_index]["line_number"] += 1
                         line_num += 1
             except KeyboardInterrupt as exception:
                 self.__save_description()
                 raise exception
 
         if not broken:
-            self.__description[self.__matching_index][
-                "previous_hash"
-            ] = self.__description[self.__matching_index]["hash"]
+            self.__description[self.__matching_index]["previous_hash"] = (
+                self.__description[self.__matching_index]["hash"]
+            )
 
         self.__save_description()
 
         return self
```

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/filesystem/__init__.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/filesystem/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/filesystem/cleanup.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/filesystem/cleanup.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/filesystem/counter.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/filesystem/counter.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/filesystem/dir_base.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/filesystem/dir_base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/filesystem/dir_structure/__init__.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/filesystem/dir_structure/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/filesystem/dir_structure/backup.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/filesystem/dir_structure/backup.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/filesystem/dir_structure/base.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/filesystem/dir_structure/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/filesystem/dir_structure/restore.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/filesystem/dir_structure/restore.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/filesystem/json_base.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/filesystem/json_base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/filesystem/printer/__init__.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/filesystem/printer/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/filesystem/printer/base.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/filesystem/printer/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/filesystem/printer/file.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/filesystem/printer/file.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/filesystem/printer/stdout.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/filesystem/printer/stdout.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/filesystem/registrar_counter.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/filesystem/registrar_counter.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/filesystem/status_file.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/filesystem/status_file.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/migrators/__init__.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/migrators/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/migrators/alembic.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/migrators/alembic.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/migrators/base.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/migrators/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,14 @@
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
-
 from typing import Optional
 
 from sqlalchemy.orm import Session
 
 from PyFunceble.cli.continuous_integration.base import ContinuousIntegrationBase
```

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/migrators/csv_file/__init__.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/migrators/csv_file/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/migrators/csv_file/base.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/migrators/csv_file/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/migrators/csv_file/inactive_source_delete.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/migrators/csv_file/inactive_source_delete.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/migrators/csv_file/whois_registrar_add.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/migrators/csv_file/whois_registrar_add.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/migrators/db_base.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/migrators/db_base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/migrators/file_cleanup/__init__.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/migrators/file_cleanup/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/migrators/file_cleanup/base.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/migrators/file_cleanup/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/migrators/file_cleanup/hashes_file.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/migrators/file_cleanup/hashes_file.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/migrators/file_cleanup/mining_file.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/migrators/file_cleanup/mining_file.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/migrators/file_cleanup/production_config_file.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/migrators/file_cleanup/production_config_file.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/migrators/json2csv/__init__.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/migrators/json2csv/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/migrators/json2csv/base.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/migrators/json2csv/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/migrators/json2csv/inactive.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/migrators/json2csv/inactive.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/migrators/json2csv/whois.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/migrators/json2csv/whois.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/migrators/mariadb/__init__.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/migrators/mariadb/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/migrators/mariadb/base.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/migrators/mariadb/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/migrators/mariadb/file_and_status.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/migrators/mariadb/file_and_status.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/migrators/mariadb/whois_record_idna_subject.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/migrators/mariadb/whois_record_idna_subject.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/processes/__init__.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/processes/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/processes/base.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/processes/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/processes/chancy_producer.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/processes/chancy_producer.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/processes/chancy_tester.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/processes/chancy_tester.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/processes/dir_files_sorter.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/processes/dir_files_sorter.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/processes/file_sorter.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/processes/file_sorter.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/processes/migrator.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/processes/migrator.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/processes/miner.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/processes/miner.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/processes/producer.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/processes/producer.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/processes/tester.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/processes/tester.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/processes/workers/__init__.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/processes/workers/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/processes/workers/base.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/processes/workers/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,17 +111,17 @@
         continuous_integration: Optional[ContinuousIntegrationBase] = None,
         configuration: Optional[dict] = None,
     ) -> None:
         self.configuration = self._params["configuration"] = configuration
         self.input_queue = self._params["input_queue"] = input_queue
         self.output_queue = self._params["output_queue"] = output_queue
 
-        self.continuous_integration = self._params[
-            "continuous_integration"
-        ] = continuous_integration
+        self.continuous_integration = self._params["continuous_integration"] = (
+            continuous_integration
+        )
 
         self.global_exit_event = self._params["global_exit_event"] = global_exit_event
         self.exit_it = multiprocessing.Event()
 
         self._parent_connection, self._child_connection = multiprocessing.Pipe()
         self._exception = None
```

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/processes/workers/chancy_producer.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/processes/workers/chancy_producer.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/processes/workers/chancy_tester.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/processes/workers/chancy_tester.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/processes/workers/dir_files_sorter.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/processes/workers/dir_files_sorter.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/processes/workers/file_sorter.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/processes/workers/file_sorter.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/processes/workers/file_sorter_base.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/processes/workers/file_sorter_base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/processes/workers/migrator.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/processes/workers/migrator.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/processes/workers/miner.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/processes/workers/miner.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/processes/workers/producer.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/processes/workers/producer.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/processes/workers/tester.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/processes/workers/tester.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/scripts/__init__.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/scripts/iana.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/scripts/iana.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/scripts/production.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/scripts/production.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,14 @@
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
-
 import copy
 import functools
 import os
 import pathlib
 from typing import List, Optional
 
 import PyFunceble.cli.storage
@@ -512,17 +511,17 @@
             to_append = ".".join(
                 self.version_utility.get_splitted(self.version_utility.local_version)[0]
             )
 
             if to_append not in self.version_file_content["deprecated"]:
                 self.version_file_content["deprecated"].append(to_append)
 
-        self.version_file_content[
-            "current_version"
-        ] = PyFunceble.storage.PROJECT_VERSION
+        self.version_file_content["current_version"] = (
+            PyFunceble.storage.PROJECT_VERSION
+        )
 
         self.dict_helper.set_subject(self.version_file_content).to_yaml_file(
             self.VERSION_FILE_PATH
         )
 
         PyFunceble.facility.Logger.info(
             "Finished to update version file.",
```

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/scripts/public_suffix.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/scripts/public_suffix.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/storage.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -249,17 +249,19 @@
     },
     "parent_directory": "output",
     "merged_directory": "merged_results",
     "splitted": {"directory": "splitted"},
 }
 
 OUTPUTS: Optional[Box] = Box(
-    Merge(UNIX_OUTPUTS).into(UNIVERSAL_OUTPUTS)
-    if PlatformUtility.is_unix()
-    else Merge(WIN_OUTPUTS).into(UNIVERSAL_OUTPUTS),
+    (
+        Merge(UNIX_OUTPUTS).into(UNIVERSAL_OUTPUTS)
+        if PlatformUtility.is_unix()
+        else Merge(WIN_OUTPUTS).into(UNIVERSAL_OUTPUTS)
+    ),
     frozen_box=True,
 )
 
 OUTPUT_DIRECTORY: str = os.path.join(
     PyFunceble.cli.storage_facility.get_output_directory(),
     OUTPUTS.parent_directory,
 )
```

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/storage_facility.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/storage_facility.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/system/__init__.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/system/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/system/base.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/system/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/system/integrator.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/system/integrator.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/system/launcher.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/system/launcher.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/utils/__init__.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/utils/ascii_logo.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/utils/ascii_logo.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/utils/sort.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/utils/sort.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/utils/stdout.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/utils/stdout.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/utils/testing.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/utils/testing.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,17 +228,15 @@
         url2netloc = Url2Netloc(
             aggressive=bool(PyFunceble.storage.CONFIGURATION.cli_decoding.aggressive)
         )
 
     if cidr2subject is None:
         cidr2subject = CIDR2Subject()
 
-    adblock_inputline2subject.aggressive = (
-        wildcard2subject.aggressive
-    ) = (
+    adblock_inputline2subject.aggressive = wildcard2subject.aggressive = (
         rpz_inputline2subject.aggressive
     ) = inputline2subject.aggressive = url2netloc.aggressive = bool(
         PyFunceble.storage.CONFIGURATION.cli_decoding.aggressive
     )
 
     if inputline2subject.aggressive and subject_type == "url":
         # URL Decoder doesn't have an aggressive mode.
```

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/cli/utils/version.py` & `PyFunceble-dev-4.2.9/PyFunceble/cli/utils/version.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/config/__init__.py` & `PyFunceble-dev-4.2.9/PyFunceble/config/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/config/compare.py` & `PyFunceble-dev-4.2.9/PyFunceble/config/compare.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/config/loader.py` & `PyFunceble-dev-4.2.9/PyFunceble/config/loader.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/converter/__init__.py` & `PyFunceble-dev-4.2.9/PyFunceble/converter/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/converter/adblock_input_line2subject.py` & `PyFunceble-dev-4.2.9/PyFunceble/converter/adblock_input_line2subject.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/converter/base.py` & `PyFunceble-dev-4.2.9/PyFunceble/converter/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/converter/cidr2subject.py` & `PyFunceble-dev-4.2.9/PyFunceble/converter/cidr2subject.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/converter/input_line2subject.py` & `PyFunceble-dev-4.2.9/PyFunceble/converter/input_line2subject.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/converter/internal_url.py` & `PyFunceble-dev-4.2.9/PyFunceble/converter/internal_url.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/converter/rpz_input_line2subject.py` & `PyFunceble-dev-4.2.9/PyFunceble/converter/rpz_input_line2subject.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/converter/rpz_policy2subject.py` & `PyFunceble-dev-4.2.9/PyFunceble/converter/rpz_policy2subject.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/converter/subject2complements.py` & `PyFunceble-dev-4.2.9/PyFunceble/converter/subject2complements.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/converter/url2netloc.py` & `PyFunceble-dev-4.2.9/PyFunceble/converter/url2netloc.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/converter/wildcard2subject.py` & `PyFunceble-dev-4.2.9/PyFunceble/converter/wildcard2subject.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/data/alembic/__init__.py` & `PyFunceble-dev-4.2.9/PyFunceble/data/alembic/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/data/alembic/mysql/__init__.py` & `PyFunceble-dev-4.2.9/PyFunceble/data/alembic/mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/data/alembic/mysql/env.py` & `PyFunceble-dev-4.2.9/PyFunceble/data/alembic/mysql/env.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/data/alembic/mysql/versions/35c79626ecb9_fix_some_columns.py` & `PyFunceble-dev-4.2.9/PyFunceble/data/alembic/mysql/versions/35c79626ecb9_fix_some_columns.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Fix some columns
 
 Revision ID: 35c79626ecb9
 Revises: ade87195b0a0
 Create Date: 2020-08-21 11:42:07.044762
 
 """
+
 from alembic import op
 from sqlalchemy.exc import OperationalError
 
 # pylint: skip-file
 
 # revision identifiers, used by Alembic.
 revision = "35c79626ecb9"
```

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/data/alembic/mysql/versions/3a4c55a9320d_add_continue_table.py` & `PyFunceble-dev-4.2.9/PyFunceble/data/alembic/mysql/versions/3a4c55a9320d_add_continue_table.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Add continue table.
 
 Revision ID: 3a4c55a9320d
 Revises: 3d6f4a33cdb2
 Create Date: 2020-12-13 22:52:56.968513
 
 """
+
 import sqlalchemy as sa
 from alembic import op
 
 # pylint: skip-file
 
 # revision identifiers, used by Alembic.
 revision = "3a4c55a9320d"
```

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/data/alembic/mysql/versions/3d6f4a33cdb2_add_inactive_table.py` & `PyFunceble-dev-4.2.9/PyFunceble/data/alembic/mysql/versions/3d6f4a33cdb2_add_inactive_table.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Add inactive table.
 
 Revision ID: 3d6f4a33cdb2
 Revises: 7bcf7fa64ba1
 Create Date: 2020-12-13 19:45:41.893657
 
 """
+
 import sqlalchemy as sa
 from alembic import op
 
 # pylint: skip-file
 
 
 # revision identifiers, used by Alembic.
```

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/data/alembic/mysql/versions/45713fea8097_deletion_uneeded_columns_from_whois_.py` & `PyFunceble-dev-4.2.9/PyFunceble/data/alembic/mysql/versions/45713fea8097_deletion_uneeded_columns_from_whois_.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Deletion uneeded columns from whois record
 
 Revision ID: 45713fea8097
 Revises: e04e8301d1a2
 Create Date: 2020-12-07 12:36:04.818466
 
 """
+
 import sqlalchemy as sa
 from alembic import op
 from sqlalchemy.dialects import mysql
 
 # pylint: skip-file
 
 # revision identifiers, used by Alembic.
```

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/data/alembic/mysql/versions/459a0d7b8f09_add_idna_subject_column_into_whois.py` & `PyFunceble-dev-4.2.9/PyFunceble/data/alembic/mysql/versions/459a0d7b8f09_add_idna_subject_column_into_whois.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Add idna_subject column into whois record
 
 Revision ID: 459a0d7b8f09
 Revises: 45713fea8097
 Create Date: 2020-12-07 12:37:52.018637
 
 """
+
 import sqlalchemy as sa
 from alembic import op
 
 # pylint: skip-file
 
 # revision identifiers, used by Alembic.
 revision = "459a0d7b8f09"
```

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/data/alembic/mysql/versions/6f4729deaf03_delete_inactive_source_column.py` & `PyFunceble-dev-4.2.9/PyFunceble/data/alembic/mysql/versions/6f4729deaf03_delete_inactive_source_column.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Delete inactive.source column
 
 Revision ID: 6f4729deaf03
 Revises: 95dc17ddd729
 Create Date: 2021-02-13 12:21:00.493002
 
 """
+
 import sqlalchemy as sa
 from alembic import op
 from sqlalchemy.dialects import mysql
 
 # pylint: skip-file
 
 # revision identifiers, used by Alembic.
```

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/data/alembic/mysql/versions/7bcf7fa64ba1_rename_created_to_created_at_and.py` & `PyFunceble-dev-4.2.9/PyFunceble/data/alembic/mysql/versions/7bcf7fa64ba1_rename_created_to_created_at_and.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Rename created to created_at and modified_to_modified_at
 
 Revision ID: 7bcf7fa64ba1
 Revises: 83ada95132bf
 Create Date: 2020-12-08 17:34:59.349943
 
 """
+
 import sqlalchemy as sa
 from alembic import op
 from sqlalchemy.dialects import mysql
 
 # pylint: skip-file
 
 # revision identifiers, used by Alembic.
```

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/data/alembic/mysql/versions/83ada95132bf_delete_the_file_table.py` & `PyFunceble-dev-4.2.9/PyFunceble/data/alembic/mysql/versions/83ada95132bf_delete_the_file_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Delete the file table.
 
 Revision ID: 83ada95132bf
 Revises: 459a0d7b8f09
 Create Date: 2020-12-07 12:49:48.797794
 
 """
+
 import sqlalchemy as sa
 from alembic import op
 from sqlalchemy.dialects import mysql
 
 # pylint: skip-file
 
 # revision identifiers, used by Alembic.
```

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/data/alembic/mysql/versions/912bbcb77a6c_add_registrar_column.py` & `PyFunceble-dev-4.2.9/PyFunceble/data/alembic/mysql/versions/912bbcb77a6c_add_registrar_column.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Add registrar column
 
 Revision ID: 912bbcb77a6c
 Revises: 6f4729deaf03
 Create Date: 2021-12-04 23:52:11.861732
 
 """
+
 import sqlalchemy as sa
 from alembic import op
 
 # pylint: skip-file
 
 # revision identifiers, used by Alembic.
 revision = "912bbcb77a6c"
```

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/data/alembic/mysql/versions/95dc17ddd729_introduction_of_the_session_id_column.py` & `PyFunceble-dev-4.2.9/PyFunceble/data/alembic/mysql/versions/95dc17ddd729_introduction_of_the_session_id_column.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Introduction of the session_id column
 
 Revision ID: 95dc17ddd729
 Revises: bef7bcaac3f2
 Create Date: 2020-12-23 02:26:21.647125
 
 """
+
 import sqlalchemy as sa
 from alembic import op
 
 # pylint: skip-file
 
 # revision identifiers, used by Alembic.
 revision = "95dc17ddd729"
```

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/data/alembic/mysql/versions/__init__.py` & `PyFunceble-dev-4.2.9/PyFunceble/data/alembic/mysql/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/data/alembic/mysql/versions/ade87195b0a0_base.py` & `PyFunceble-dev-4.2.9/PyFunceble/data/alembic/mysql/versions/ade87195b0a0_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Base
 
 Revision ID: ade87195b0a0
 Revises:
 Create Date: 2020-08-15 20:12:26.768419
 
 """
+
 import sqlalchemy as sa
 from alembic import op
 
 # pylint: skip-file
 
 # revision identifiers, used by Alembic.
 revision = "ade87195b0a0"
```

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/data/alembic/mysql/versions/bef7bcaac3f2_make_id_a_bigint.py` & `PyFunceble-dev-4.2.9/PyFunceble/data/alembic/mysql/versions/bef7bcaac3f2_make_id_a_bigint.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Make id a bigint.
 
 Revision ID: bef7bcaac3f2
 Revises: 3a4c55a9320d
 Create Date: 2020-12-16 19:09:41.212679
 
 """
+
 import sqlalchemy as sa
 from alembic import op
 from sqlalchemy.dialects import mysql
 
 # pylint: skip-file
 
 # revision identifiers, used by Alembic.
```

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/data/alembic/mysql/versions/d8893cd406db_allow_whois_record_to_be_empty_null.py` & `PyFunceble-dev-4.2.9/PyFunceble/data/alembic/mysql/versions/d8893cd406db_allow_whois_record_to_be_empty_null.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Allow whois record to be empty/NULL
 
 Revision ID: d8893cd406db
 Revises: 35c79626ecb9
 Create Date: 2020-08-22 17:27:52.087506
 
 """
+
 from alembic import op
 from sqlalchemy.dialects import mysql
 
 # pylint: skip-file
 
 # revision identifiers, used by Alembic.
 revision = "d8893cd406db"
```

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/data/alembic/mysql/versions/e04e8301d1a2_deletion_of_the_mined_table.py` & `PyFunceble-dev-4.2.9/PyFunceble/data/alembic/mysql/versions/e04e8301d1a2_deletion_of_the_mined_table.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Deletion of the mined table
 
 Revision ID: e04e8301d1a2
 Revises: d8893cd406db
 Create Date: 2020-12-07 12:33:43.650514
 
 """
+
 import sqlalchemy as sa
 from alembic import op
 from sqlalchemy.dialects import mysql
 
 # pylint: skip-file
 
 # revision identifiers, used by Alembic.
```

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/data/alembic/postgresql/__init__.py` & `PyFunceble-dev-4.2.9/PyFunceble/data/alembic/postgresql/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/data/alembic/postgresql/env.py` & `PyFunceble-dev-4.2.9/PyFunceble/data/alembic/postgresql/env.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/data/alembic/postgresql/versions/__init__.py` & `PyFunceble-dev-4.2.9/PyFunceble/data/alembic/postgresql/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/data/alembic/postgresql/versions/a32ac5d66eee_initial_version.py` & `PyFunceble-dev-4.2.9/PyFunceble/data/alembic/postgresql/versions/a32ac5d66eee_initial_version.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Initial Version
 
 Revision ID: a32ac5d66eee
 Revises:
 Create Date: 2022-12-28 07:20:50.310072
 
 """
+
 import sqlalchemy as sa
 from alembic import op
 
 # pylint: skip-file
 
 # revision identifiers, used by Alembic.
 revision = "a32ac5d66eee"
```

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/data/infrastructure/.PyFunceble_production.yaml` & `PyFunceble-dev-4.2.9/PyFunceble/data/infrastructure/.PyFunceble_production.yaml`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/data/infrastructure/dir_structure_production.json` & `PyFunceble-dev-4.2.9/PyFunceble/data/infrastructure/dir_structure_production.json`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/database/__init__.py` & `PyFunceble-dev-4.2.9/PyFunceble/database/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/database/credential/__init__.py` & `PyFunceble-dev-4.2.9/PyFunceble/database/credential/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/database/credential/base.py` & `PyFunceble-dev-4.2.9/PyFunceble/database/credential/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/database/credential/mariadb.py` & `PyFunceble-dev-4.2.9/PyFunceble/database/credential/mariadb.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/database/credential/mysql.py` & `PyFunceble-dev-4.2.9/PyFunceble/database/credential/mysql.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/database/credential/postgresql.py` & `PyFunceble-dev-4.2.9/PyFunceble/database/credential/postgresql.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/database/schemas/__init__.py` & `PyFunceble-dev-4.2.9/PyFunceble/database/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/database/schemas/autocontinue.py` & `PyFunceble-dev-4.2.9/PyFunceble/database/schemas/autocontinue.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/database/schemas/inactive.py` & `PyFunceble-dev-4.2.9/PyFunceble/database/schemas/inactive.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/database/schemas/status.py` & `PyFunceble-dev-4.2.9/PyFunceble/database/schemas/status.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/database/schemas/whois_record.py` & `PyFunceble-dev-4.2.9/PyFunceble/database/schemas/whois_record.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/database/session.py` & `PyFunceble-dev-4.2.9/PyFunceble/database/session.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/database/sqlalchemy/__init__.py` & `PyFunceble-dev-4.2.9/PyFunceble/database/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/database/sqlalchemy/all_schemas.py` & `PyFunceble-dev-4.2.9/PyFunceble/database/sqlalchemy/all_schemas.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/database/sqlalchemy/base_schema.py` & `PyFunceble-dev-4.2.9/PyFunceble/database/sqlalchemy/base_schema.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/dataset/__init__.py` & `PyFunceble-dev-4.2.9/PyFunceble/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/dataset/autocontinue/__init__.py` & `PyFunceble-dev-4.2.9/PyFunceble/dataset/autocontinue/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/dataset/autocontinue/base.py` & `PyFunceble-dev-4.2.9/PyFunceble/dataset/autocontinue/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/dataset/autocontinue/csv.py` & `PyFunceble-dev-4.2.9/PyFunceble/dataset/autocontinue/csv.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/dataset/autocontinue/sql.py` & `PyFunceble-dev-4.2.9/PyFunceble/dataset/autocontinue/sql.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/dataset/base.py` & `PyFunceble-dev-4.2.9/PyFunceble/dataset/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/dataset/csv_base.py` & `PyFunceble-dev-4.2.9/PyFunceble/dataset/csv_base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/dataset/db_base.py` & `PyFunceble-dev-4.2.9/PyFunceble/dataset/db_base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/dataset/iana.py` & `PyFunceble-dev-4.2.9/PyFunceble/dataset/iana.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/dataset/inactive/__init__.py` & `PyFunceble-dev-4.2.9/PyFunceble/dataset/inactive/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/dataset/inactive/base.py` & `PyFunceble-dev-4.2.9/PyFunceble/dataset/inactive/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/dataset/inactive/csv.py` & `PyFunceble-dev-4.2.9/PyFunceble/dataset/inactive/csv.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/dataset/inactive/sql.py` & `PyFunceble-dev-4.2.9/PyFunceble/dataset/inactive/sql.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/dataset/ipv4_reputation.py` & `PyFunceble-dev-4.2.9/PyFunceble/dataset/ipv4_reputation.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/dataset/public_suffix.py` & `PyFunceble-dev-4.2.9/PyFunceble/dataset/public_suffix.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/dataset/sql_base.py` & `PyFunceble-dev-4.2.9/PyFunceble/dataset/sql_base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/dataset/user_agent.py` & `PyFunceble-dev-4.2.9/PyFunceble/dataset/user_agent.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/dataset/whois/__init__.py` & `PyFunceble-dev-4.2.9/PyFunceble/dataset/whois/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/dataset/whois/base.py` & `PyFunceble-dev-4.2.9/PyFunceble/dataset/whois/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/dataset/whois/csv.py` & `PyFunceble-dev-4.2.9/PyFunceble/dataset/whois/csv.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/dataset/whois/sql.py` & `PyFunceble-dev-4.2.9/PyFunceble/dataset/whois/sql.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/downloader/__init__.py` & `PyFunceble-dev-4.2.9/PyFunceble/downloader/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/downloader/base.py` & `PyFunceble-dev-4.2.9/PyFunceble/downloader/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/downloader/exceptions.py` & `PyFunceble-dev-4.2.9/PyFunceble/downloader/exceptions.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/downloader/iana.py` & `PyFunceble-dev-4.2.9/PyFunceble/downloader/iana.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/downloader/ipv4_reputation.py` & `PyFunceble-dev-4.2.9/PyFunceble/downloader/ipv4_reputation.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/downloader/public_suffix.py` & `PyFunceble-dev-4.2.9/PyFunceble/downloader/public_suffix.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/downloader/user_agents.py` & `PyFunceble-dev-4.2.9/PyFunceble/downloader/user_agents.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/exceptions.py` & `PyFunceble-dev-4.2.9/PyFunceble/exceptions.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/facility.py` & `PyFunceble-dev-4.2.9/PyFunceble/facility.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/factory.py` & `PyFunceble-dev-4.2.9/PyFunceble/factory.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/helpers/__init__.py` & `PyFunceble-dev-4.2.9/PyFunceble/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/helpers/command.py` & `PyFunceble-dev-4.2.9/PyFunceble/helpers/command.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/helpers/dict.py` & `PyFunceble-dev-4.2.9/PyFunceble/helpers/dict.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/helpers/directory.py` & `PyFunceble-dev-4.2.9/PyFunceble/helpers/directory.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/helpers/download.py` & `PyFunceble-dev-4.2.9/PyFunceble/helpers/download.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/helpers/environment_variable.py` & `PyFunceble-dev-4.2.9/PyFunceble/helpers/environment_variable.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/helpers/exceptions.py` & `PyFunceble-dev-4.2.9/PyFunceble/helpers/exceptions.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/helpers/file.py` & `PyFunceble-dev-4.2.9/PyFunceble/helpers/file.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/helpers/hash.py` & `PyFunceble-dev-4.2.9/PyFunceble/helpers/hash.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/helpers/list.py` & `PyFunceble-dev-4.2.9/PyFunceble/helpers/list.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/helpers/merge.py` & `PyFunceble-dev-4.2.9/PyFunceble/helpers/merge.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/helpers/regex.py` & `PyFunceble-dev-4.2.9/PyFunceble/helpers/regex.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/logger.py` & `PyFunceble-dev-4.2.9/PyFunceble/logger.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/query/__init__.py` & `PyFunceble-dev-4.2.9/PyFunceble/query/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/query/collection.py` & `PyFunceble-dev-4.2.9/PyFunceble/query/collection.py`

 * *Files 5% similar despite different names*

```diff
@@ -84,14 +84,15 @@
     """
 
     SUPPORTED_CHECKERS: List[str] = ["syntax", "reputation", "availability"]
     SUPPORTED_STATUS_ORIGIN: List[str] = ["frequent", "latest", "recommended"]
 
     STD_URL_BASE: str = "http://localhost:8001"
     STD_PREFERRED_STATUS_ORIGIN: str = "frequent"
+    STD_TIMEOUT: float = 5.0
 
     _token: Optional[str] = None
     """
     The token to use while communicating with the collection API.
     """
 
     _url_base: Optional[str] = None
@@ -105,22 +106,28 @@
     """
 
     _is_modern_api: Optional[bool] = None
     """
     Whether we are working with the modern or legacy API.
     """
 
+    _timeout: float = 5.0
+    """
+    The timeout to use while communicating with the API.
+    """
+
     session: Optional[requests.Session] = None
 
     def __init__(
         self,
         *,
         token: Optional[str] = None,
         url_base: Optional[str] = None,
         preferred_status_origin: Optional[str] = None,
+        timeout: Optional[float] = None,
     ) -> None:
         if token is not None:
             self.token = token
         else:
             self.token = EnvironmentVariableHelper(
                 "PYFUNCEBLE_COLLECTION_API_TOKEN"
             ).get_value(default="")
@@ -131,14 +138,19 @@
             self.guess_and_set_url_base()
 
         if preferred_status_origin is not None:
             self.preferred_status_origin = preferred_status_origin
         else:
             self.guess_and_set_preferred_status_origin()
 
+        if timeout is not None:
+            self.timeout = timeout
+        else:
+            self.guess_and_set_timeout()
+
         self.session = requests.Session()
         self.session.headers.update(
             {
                 "Authorization": f"Bearer {self.token}" if self.token else None,
                 "X-Pyfunceble-Version": PyFunceble.storage.PROJECT_VERSION,
                 "Content-Type": "application/json",
             }
@@ -279,14 +291,51 @@
             The value to set.
         """
 
         self.is_modern_api = value
 
         return self
 
+    @property
+    def timeout(self) -> float:
+        """
+        Provides the value of the :code:`_timeout` attribute.
+        """
+
+        return self._timeout
+
+    @timeout.setter
+    def timeout(self, value: float) -> None:
+        """
+        Sets the value of the :code:`_timeout` attribute.
+
+        :param value:
+            The value to set.
+
+        :raise TypeError:
+            When the given :code:`value` is not a :py:class:`float`.
+        """
+
+        if not isinstance(value, (int, float)):
+            raise TypeError(f"<value> should be {float}, {type(value)} given.")
+
+        self._timeout = value
+
+    def set_timeout(self, value: float) -> "CollectionQueryTool":
+        """
+        Sets the value of the :code:`_timeout` attribute.
+
+        :param value:
+            The value to set.
+        """
+
+        self.timeout = value
+
+        return self
+
     def guess_and_set_url_base(self) -> "CollectionQueryTool":
         """
         Try to guess the URL base to work with.
         """
 
         if PyFunceble.facility.ConfigLoader.is_already_loaded():
             if isinstance(PyFunceble.storage.CONFIGURATION.collection.url_base, str):
@@ -303,24 +352,30 @@
         return self
 
     def guess_and_set_is_modern_api(self) -> "CollectionQueryTool":
         """
         Try to guess if we are working with a legacy version.
         """
 
-        try:
-            response = self.session.get(
-                f"{self.url_base}/v1/stats/subject",
-            )
+        if self.token:
+            try:
+                response = self.session.get(
+                    f"{self.url_base}/v1/stats/subject",
+                    timeout=self.timeout,
+                )
 
-            response.raise_for_status()
+                response.raise_for_status()
 
+                self.is_modern_api = False
+            except (requests.RequestException, json.decoder.JSONDecodeError):
+                self.is_modern_api = True
+        else:
             self.is_modern_api = False
-        except (requests.RequestException, json.decoder.JSONDecodeError):
-            self.is_modern_api = True
+
+        return self
 
     @property
     def preferred_status_origin(self) -> Optional[str]:
         """
         Provides the value of the :code:`_preferred_status_origin` attribute.
         """
 
@@ -376,14 +431,26 @@
             else:
                 self.preferred_status_origin = self.STD_PREFERRED_STATUS_ORIGIN
         else:
             self.preferred_status_origin = self.STD_PREFERRED_STATUS_ORIGIN
 
         return self
 
+    def guess_and_set_timeout(self) -> "CollectionQueryTool":
+        """
+        Try to guess the timeout to use.
+        """
+
+        if PyFunceble.facility.ConfigLoader.is_already_loaded():
+            self.timeout = PyFunceble.storage.CONFIGURATION.lookup.timeout
+        else:
+            self.timeout = self.STD_TIMEOUT
+
+        return self
+
     def ensure_is_modern_api_is_set(func):  # pylint: disable=no-self-argument
         """
         Ensures that the :code:`is_modern_api` attribute is set before running
         the decorated method.
         """
 
         def wrapper(self, *args, **kwargs):
@@ -422,14 +489,15 @@
         else:
             url = f"{self.url_base}/v1/subject/search"
 
         try:
             response = self.session.post(
                 url,
                 json={"subject": subject},
+                timeout=self.timeout,
             )
 
             response_json = response.json()
 
             if response.status_code == 200:
                 PyFunceble.facility.Logger.debug(
                     "Successfully search subject: %r. Response: %r",
@@ -570,19 +638,34 @@
             url = f"{self.url_base}/v1/status/{checker_type}"
 
         try:
             if isinstance(data, dict):
                 response = self.session.post(
                     url,
                     json=data,
+                    timeout=self.timeout,
+                )
+            elif isinstance(
+                data,
+                (
+                    AvailabilityCheckerStatus,
+                    SyntaxCheckerStatus,
+                    ReputationCheckerStatus,
+                ),
+            ):
+                response = self.session.post(
+                    url,
+                    json=data.to_dict(),
+                    timeout=self.timeout,
                 )
             else:
                 response = self.session.post(
                     url,
                     data=data,
+                    timeout=self.timeout,
                 )
 
             response_json = response.json()
 
             if response.status_code == 200:
                 PyFunceble.facility.Logger.debug(
                     "Successfully submitted data: %r to %s", data, url
@@ -618,25 +701,32 @@
         :raise ValueError:
             When the given :code:`checker_type` is not a subject checker type.
         """
 
         if not self.token:
             return None
 
+        if isinstance(
+            data,
+            (AvailabilityCheckerStatus, SyntaxCheckerStatus, ReputationCheckerStatus),
+        ):
+            data = data.to_dict()
+
         if not isinstance(data, dict):  # pragma: no cover ## Should never happen
             raise TypeError(f"<data> should be {dict}, {type(data)} given.")
 
         PyFunceble.facility.Logger.info("Starting to submit WHOIS: %r", data)
 
         url = f"{self.url_base}/v1/status/whois"
 
         try:
             response = self.session.post(
                 url,
                 json=data,
+                timeout=self.timeout,
             )
 
             response_json = response.json()
 
             if response.status_code == 200:
                 PyFunceble.facility.Logger.debug(
                     "Successfully submitted WHOIS data: %r to %s", data, url
```

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/query/dns/__init__.py` & `PyFunceble-dev-4.2.9/PyFunceble/query/dns/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/query/dns/nameserver.py` & `PyFunceble-dev-4.2.9/PyFunceble/query/dns/nameserver.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/query/dns/query_tool.py` & `PyFunceble-dev-4.2.9/PyFunceble/query/dns/query_tool.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/query/dns/resolver.py` & `PyFunceble-dev-4.2.9/PyFunceble/query/dns/resolver.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/query/http_status_code.py` & `PyFunceble-dev-4.2.9/PyFunceble/query/http_status_code.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/query/netinfo/__init__.py` & `PyFunceble-dev-4.2.9/PyFunceble/query/netinfo/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/query/netinfo/address.py` & `PyFunceble-dev-4.2.9/PyFunceble/query/netinfo/address.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/query/netinfo/base.py` & `PyFunceble-dev-4.2.9/PyFunceble/query/netinfo/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/query/netinfo/hostbyaddr.py` & `PyFunceble-dev-4.2.9/PyFunceble/query/netinfo/hostbyaddr.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/query/record/__init__.py` & `PyFunceble-dev-4.2.9/PyFunceble/query/record/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/query/record/base.py` & `PyFunceble-dev-4.2.9/PyFunceble/query/record/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/query/record/dns.py` & `PyFunceble-dev-4.2.9/PyFunceble/query/record/dns.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/query/record/whois.py` & `PyFunceble-dev-4.2.9/PyFunceble/query/record/whois.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/query/requests/__init__.py` & `PyFunceble-dev-4.2.9/PyFunceble/query/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/query/requests/adapter/__init__.py` & `PyFunceble-dev-4.2.9/PyFunceble/query/requests/adapter/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/query/requests/adapter/base.py` & `PyFunceble-dev-4.2.9/PyFunceble/query/requests/adapter/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/query/requests/adapter/http.py` & `PyFunceble-dev-4.2.9/PyFunceble/query/requests/adapter/http.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/query/requests/adapter/https.py` & `PyFunceble-dev-4.2.9/PyFunceble/query/requests/adapter/https.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,20 +109,20 @@
             if hostname_ip:
                 request.url = request.url.replace(
                     f"{parsed_url.scheme}://{parsed_url.hostname}",
                     f"{parsed_url.scheme}://{hostname_ip}",
                 )
 
             if parsed_url.scheme == "https":
-                self.poolmanager.connection_pool_kw[
-                    "server_hostname"
-                ] = parsed_url.hostname
-                self.poolmanager.connection_pool_kw[
-                    "assert_hostname"
-                ] = parsed_url.hostname
+                self.poolmanager.connection_pool_kw["server_hostname"] = (
+                    parsed_url.hostname
+                )
+                self.poolmanager.connection_pool_kw["assert_hostname"] = (
+                    parsed_url.hostname
+                )
 
             # Ensure that the Hosts header is present. Otherwise, connection might
             # not work.
             request.headers["Host"] = parsed_url.hostname
         else:
             self.poolmanager.connection_pool_kw.pop(
                 "server_hostname", PyFunceble.storage.NOT_RESOLVED_STD_HOSTNAME
```

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/query/requests/requester.py` & `PyFunceble-dev-4.2.9/PyFunceble/query/requests/requester.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/query/whois/__init__.py` & `PyFunceble-dev-4.2.9/PyFunceble/query/whois/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/query/whois/converter/__init__.py` & `PyFunceble-dev-4.2.9/PyFunceble/query/whois/converter/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/query/whois/converter/base.py` & `PyFunceble-dev-4.2.9/PyFunceble/query/whois/converter/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/query/whois/converter/digit2digits.py` & `PyFunceble-dev-4.2.9/PyFunceble/query/whois/converter/digit2digits.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
+
 # pylint: enable=line-too-long
 
 from typing import Any
 
 from PyFunceble.query.whois.converter.base import ConverterBase
```

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/query/whois/converter/expiration_date.py` & `PyFunceble-dev-4.2.9/PyFunceble/query/whois/converter/expiration_date.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/query/whois/converter/month2unified.py` & `PyFunceble-dev-4.2.9/PyFunceble/query/whois/converter/month2unified.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/query/whois/converter/registrar.py` & `PyFunceble-dev-4.2.9/PyFunceble/query/whois/converter/registrar.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/query/whois/query_tool.py` & `PyFunceble-dev-4.2.9/PyFunceble/query/whois/query_tool.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/sessions.py` & `PyFunceble-dev-4.2.9/PyFunceble/sessions.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/storage.py` & `PyFunceble-dev-4.2.9/PyFunceble/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
 from box import Box
 from dotenv import load_dotenv
 
 from PyFunceble.storage_facility import get_config_directory
 
 PROJECT_NAME: str = "PyFunceble"
-PROJECT_VERSION: str = "4.2.7.dev (Blue Duckling: Ixora)"
+PROJECT_VERSION: str = "4.2.9.dev (Blue Duckling: Ixora)"
 
 DISTRIBUTED_CONFIGURATION_FILENAME: str = ".PyFunceble_production.yaml"
 DISTRIBUTED_DIR_STRUCTURE_FILENAME: str = "dir_structure_production.json"
 
 IANA_DUMP_FILENAME: str = "iana-domains-db.json"
 PUBLIC_SUFFIX_DUMP_FILENAME: str = "public-suffix.json"
 CONFIGURATION_FILENAME: str = ".PyFunceble.yaml"
@@ -75,15 +75,17 @@
 USER_AGENT_FILENAME: str = "user_agents.json"
 IPV4_REPUTATION_FILENAME: str = "ipv4_reputation.data"
 
 # pylint: disable=line-too-long
 IANA_DUMP_LINK: str = (
     "https://raw.githubusercontent.com/PyFunceble/iana/master/iana-domains-db.json"
 )
-PUBLIC_SUFFIX_DUMP_LINK: str = "https://raw.githubusercontent.com/PyFunceble/public-suffix/master/public-suffix.json"
+PUBLIC_SUFFIX_DUMP_LINK: str = (
+    "https://raw.githubusercontent.com/PyFunceble/public-suffix/master/public-suffix.json"
+)
 USER_AGENT_DUMP_LINK: str = (
     "https://raw.githubusercontent.com/PyFunceble/user_agents/master/user_agents.json"
 )
 IPV4_REPUTATION_DUMP_LINK: str = "https://reputation.alienvault.com/reputation.data"
 
 SHORT_REPO_LINK: str = "https://pyfunceble.github.io"
 REPO_LINK: str = "https://github.com/funilrys/PyFunceble"
```

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/storage_facility.py` & `PyFunceble-dev-4.2.9/PyFunceble/storage_facility.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/utils/__init__.py` & `PyFunceble-dev-4.2.9/PyFunceble/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/utils/platform.py` & `PyFunceble-dev-4.2.9/PyFunceble/utils/platform.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/utils/profile.py` & `PyFunceble-dev-4.2.9/PyFunceble/utils/profile.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble/utils/version.py` & `PyFunceble-dev-4.2.9/PyFunceble/utils/version.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/PyFunceble_dev.egg-info/PKG-INFO` & `PyFunceble-dev-4.2.9/PyFunceble_dev.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFunceble-dev
-Version: 4.2.7
+Version: 4.2.9
 Summary: The tool to check the availability or syntax of domain, IP or URL.
 Home-page: https://github.com/funilrys/PyFunceble
 Author: funilrys
 Author-email: contact@funilrys.com
 License: Apache 2.0
 Project-URL: Documentation, https://pyfunceble.readthedocs.io/en/dev/
 Project-URL: Funding, https://github.com/sponsors/funilrys
```

### Comparing `PyFunceble-dev-4.2.7/PyFunceble_dev.egg-info/SOURCES.txt` & `PyFunceble-dev-4.2.9/PyFunceble_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/README.rst` & `PyFunceble-dev-4.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/setup.py` & `PyFunceble-dev-4.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.7/version.yaml` & `PyFunceble-dev-4.2.9/version.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-current_version: '4.2.7.dev (Blue Duckling: Ixora)'
+current_version: '4.2.9.dev (Blue Duckling: Ixora)'
 deprecated:
 - 3.0.21
 - 3.1.20
 - 3.2.13
 - 4.0.0a1
 - 4.1.0b1
 - 4.2.0a1
```

