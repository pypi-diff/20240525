# Comparing `tmp/pybliometrics-3.6.tar.gz` & `tmp/pybliometrics-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybliometrics-3.6.tar", last modified: Fri Dec  8 09:03:56 2023, max compression
+gzip compressed data, was "pybliometrics-4.0.tar", last modified: Sat May 25 09:45:57 2024, max compression
```

## Comparing `pybliometrics-3.6.tar` & `pybliometrics-4.0.tar`

### file list

```diff
@@ -1,106 +1,108 @@
-drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-12-08 09:03:56.157818 pybliometrics-3.6/
-drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-12-08 09:03:56.125818 pybliometrics-3.6/.github/
-drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-12-08 09:03:56.129818 pybliometrics-3.6/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 panther   (1000) panther   (1000)      180 2022-01-29 14:12:14.000000 pybliometrics-3.6/.github/ISSUE_TEMPLATE/bug.md
--rw-rw-r--   0 panther   (1000) panther   (1000)      167 2022-01-29 14:12:14.000000 pybliometrics-3.6/.github/ISSUE_TEMPLATE/feature.md
--rw-rw-r--   0 panther   (1000) panther   (1000)      336 2022-01-29 14:12:14.000000 pybliometrics-3.6/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 panther   (1000) panther   (1000)      668 2020-01-13 10:35:18.000000 pybliometrics-3.6/.gitignore
--rw-rw-r--   0 panther   (1000) panther   (1000)      168 2023-04-18 19:33:38.000000 pybliometrics-3.6/.readthedocs.yaml
--rw-r--r--   0 panther   (1000) panther   (1000)     3180 2020-09-17 08:30:44.000000 pybliometrics-3.6/CONTRIBUTING.rst
--rw-r--r--   0 panther   (1000) panther   (1000)     1442 2020-01-13 10:35:18.000000 pybliometrics-3.6/LICENSE
--rw-r--r--   0 panther   (1000) panther   (1000)     5062 2023-12-08 09:03:56.157818 pybliometrics-3.6/PKG-INFO
--rw-rw-r--   0 panther   (1000) panther   (1000)     3687 2023-12-03 11:43:11.000000 pybliometrics-3.6/README.rst
-drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-12-08 09:03:56.133818 pybliometrics-3.6/docs/
--rw-r--r--   0 panther   (1000) panther   (1000)      603 2020-01-13 10:35:18.000000 pybliometrics-3.6/docs/Makefile
-drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-12-08 09:03:56.133818 pybliometrics-3.6/docs/_static/
--rw-r--r--   0 panther   (1000) panther   (1000)       29 2021-08-12 15:57:23.000000 pybliometrics-3.6/docs/_static/custom.css
-drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-12-08 09:03:56.133818 pybliometrics-3.6/docs/access/
--rw-rw-r--   0 panther   (1000) panther   (1000)     3588 2023-12-02 15:14:03.000000 pybliometrics-3.6/docs/access/errors.rst
--rw-rw-r--   0 panther   (1000) panther   (1000)     1799 2023-12-02 15:16:19.000000 pybliometrics-3.6/docs/access/general.rst
--rw-r--r--   0 panther   (1000) panther   (1000)     1059 2023-12-02 15:19:36.000000 pybliometrics-3.6/docs/access/quotas.rst
--rw-r--r--   0 panther   (1000) panther   (1000)      109 2021-07-13 23:10:52.000000 pybliometrics-3.6/docs/access.rst
--rw-r--r--   0 panther   (1000) panther   (1000)       33 2020-01-13 10:35:18.000000 pybliometrics-3.6/docs/authors.rst
--rw-r--r--   0 panther   (1000) panther   (1000)       33 2020-01-13 10:35:18.000000 pybliometrics-3.6/docs/changelog.rst
-drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-12-08 09:03:56.137818 pybliometrics-3.6/docs/classes/
--rw-rw-r--   0 panther   (1000) panther   (1000)    11980 2023-12-02 20:08:14.000000 pybliometrics-3.6/docs/classes/AbstractRetrieval.rst
--rw-rw-r--   0 panther   (1000) panther   (1000)     3167 2023-12-02 20:07:58.000000 pybliometrics-3.6/docs/classes/AffiliationRetrieval.rst
--rw-rw-r--   0 panther   (1000) panther   (1000)     5125 2023-12-02 20:25:21.000000 pybliometrics-3.6/docs/classes/AffiliationSearch.rst
--rw-rw-r--   0 panther   (1000) panther   (1000)     8343 2023-12-02 20:31:21.000000 pybliometrics-3.6/docs/classes/AuthorRetrieval.rst
--rw-rw-r--   0 panther   (1000) panther   (1000)     4668 2023-12-02 20:35:11.000000 pybliometrics-3.6/docs/classes/AuthorSearch.rst
--rw-rw-r--   0 panther   (1000) panther   (1000)     5836 2023-12-02 20:41:42.000000 pybliometrics-3.6/docs/classes/CitationOverview.rst
--rw-rw-r--   0 panther   (1000) panther   (1000)     3017 2023-12-02 20:51:44.000000 pybliometrics-3.6/docs/classes/PlumXMetrics.rst
--rw-rw-r--   0 panther   (1000) panther   (1000)    12448 2023-12-03 11:38:24.000000 pybliometrics-3.6/docs/classes/ScopusSearch.rst
--rw-rw-r--   0 panther   (1000) panther   (1000)     4225 2023-12-03 11:12:36.000000 pybliometrics-3.6/docs/classes/SerialSearch.rst
--rw-rw-r--   0 panther   (1000) panther   (1000)     7180 2023-12-02 21:00:28.000000 pybliometrics-3.6/docs/classes/SerialTitle.rst
--rw-rw-r--   0 panther   (1000) panther   (1000)     3996 2023-12-02 20:54:58.000000 pybliometrics-3.6/docs/classes/SubjectClassifications.rst
--rw-r--r--   0 panther   (1000) panther   (1000)      804 2021-07-13 09:14:45.000000 pybliometrics-3.6/docs/classes.rst
--rw-rw-r--   0 panther   (1000) panther   (1000)     2721 2023-10-17 15:25:36.000000 pybliometrics-3.6/docs/conf.py
--rw-r--r--   0 panther   (1000) panther   (1000)     5009 2023-12-02 15:20:43.000000 pybliometrics-3.6/docs/configuration.rst
--rw-r--r--   0 panther   (1000) panther   (1000)       33 2020-01-13 10:35:18.000000 pybliometrics-3.6/docs/contributing.rst
--rw-r--r--   0 panther   (1000) panther   (1000)     1644 2021-07-13 23:03:16.000000 pybliometrics-3.6/docs/index.rst
--rw-r--r--   0 panther   (1000) panther   (1000)      747 2023-12-02 15:23:25.000000 pybliometrics-3.6/docs/installation.rst
--rw-r--r--   0 panther   (1000) panther   (1000)      817 2020-01-13 10:35:18.000000 pybliometrics-3.6/docs/make.bat
--rw-rw-r--   0 panther   (1000) panther   (1000)      111 2023-10-17 15:26:54.000000 pybliometrics-3.6/docs/requirements.txt
-drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-12-08 09:03:56.141818 pybliometrics-3.6/docs/tips/
--rw-r--r--   0 panther   (1000) panther   (1000)      915 2023-12-02 15:24:12.000000 pybliometrics-3.6/docs/tips/affiliations.rst
--rw-r--r--   0 panther   (1000) panther   (1000)      133 2020-01-28 09:17:21.000000 pybliometrics-3.6/docs/tips/configuration.rst
--rw-r--r--   0 panther   (1000) panther   (1000)     1388 2023-12-02 15:27:10.000000 pybliometrics-3.6/docs/tips/database.rst
--rw-r--r--   0 panther   (1000) panther   (1000)     4617 2023-12-02 15:29:50.000000 pybliometrics-3.6/docs/tips/migration1.rst
--rw-r--r--   0 panther   (1000) panther   (1000)      491 2023-12-02 15:31:16.000000 pybliometrics-3.6/docs/tips/rename.rst
--rw-r--r--   0 panther   (1000) panther   (1000)      661 2023-12-02 15:33:11.000000 pybliometrics-3.6/docs/tips/support.rst
--rw-r--r--   0 panther   (1000) panther   (1000)      205 2021-07-18 12:31:21.000000 pybliometrics-3.6/docs/tips.rst
-drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-12-08 09:03:56.141818 pybliometrics-3.6/meta/
--rw-r--r--   0 panther   (1000) panther   (1000)   903447 2020-01-13 10:35:18.000000 pybliometrics-3.6/meta/1-s2.0-S2352711019300573-main.pdf
--rw-r--r--   0 panther   (1000) panther   (1000)      290 2020-01-13 10:35:18.000000 pybliometrics-3.6/meta/AUTHORS.rst
--rw-rw-r--   0 panther   (1000) panther   (1000)    25716 2023-12-08 08:59:32.000000 pybliometrics-3.6/meta/CHANGES.rst
-drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-12-08 09:03:56.141818 pybliometrics-3.6/pybliometrics/
--rw-rw-r--   0 panther   (1000) panther   (1000)      382 2023-04-03 19:01:18.000000 pybliometrics-3.6/pybliometrics/__init__.py
-drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-12-08 09:03:56.149818 pybliometrics-3.6/pybliometrics/scopus/
--rw-r--r--   0 panther   (1000) panther   (1000)      615 2021-02-11 11:49:49.000000 pybliometrics-3.6/pybliometrics/scopus/__init__.py
--rw-rw-r--   0 panther   (1000) panther   (1000)    12556 2023-12-02 12:07:57.000000 pybliometrics-3.6/pybliometrics/scopus/abstract_citation.py
--rw-rw-r--   0 panther   (1000) panther   (1000)    40365 2023-12-02 11:57:32.000000 pybliometrics-3.6/pybliometrics/scopus/abstract_retrieval.py
--rw-rw-r--   0 panther   (1000) panther   (1000)     6513 2023-10-20 06:41:30.000000 pybliometrics-3.6/pybliometrics/scopus/affiliation_retrieval.py
--rw-rw-r--   0 panther   (1000) panther   (1000)     5602 2023-10-20 06:41:30.000000 pybliometrics-3.6/pybliometrics/scopus/affiliation_search.py
--rw-rw-r--   0 panther   (1000) panther   (1000)    18132 2023-12-08 08:47:44.000000 pybliometrics-3.6/pybliometrics/scopus/author_retrieval.py
--rw-rw-r--   0 panther   (1000) panther   (1000)     6409 2023-10-20 06:41:30.000000 pybliometrics-3.6/pybliometrics/scopus/author_search.py
--rw-rw-r--   0 panther   (1000) panther   (1000)     2381 2022-11-17 11:15:30.000000 pybliometrics-3.6/pybliometrics/scopus/exception.py
--rw-rw-r--   0 panther   (1000) panther   (1000)     6296 2023-12-02 15:06:43.000000 pybliometrics-3.6/pybliometrics/scopus/plumx_metrics.py
--rw-rw-r--   0 panther   (1000) panther   (1000)    11145 2023-10-20 06:41:30.000000 pybliometrics-3.6/pybliometrics/scopus/scopus_search.py
--rw-rw-r--   0 panther   (1000) panther   (1000)     7094 2023-10-20 06:41:30.000000 pybliometrics-3.6/pybliometrics/scopus/serial_search.py
--rw-rw-r--   0 panther   (1000) panther   (1000)    12252 2023-11-15 19:58:25.000000 pybliometrics-3.6/pybliometrics/scopus/serial_title.py
--rw-rw-r--   0 panther   (1000) panther   (1000)     4487 2023-10-20 06:41:30.000000 pybliometrics-3.6/pybliometrics/scopus/subject_classifications.py
-drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-12-08 09:03:56.149818 pybliometrics-3.6/pybliometrics/scopus/superclasses/
--rw-r--r--   0 panther   (1000) panther   (1000)      166 2020-04-05 10:53:54.000000 pybliometrics-3.6/pybliometrics/scopus/superclasses/__init__.py
--rw-rw-r--   0 panther   (1000) panther   (1000)     8158 2023-11-15 18:42:46.000000 pybliometrics-3.6/pybliometrics/scopus/superclasses/base.py
--rw-rw-r--   0 panther   (1000) panther   (1000)     1786 2023-10-16 12:32:42.000000 pybliometrics-3.6/pybliometrics/scopus/superclasses/retrieval.py
--rw-r--r--   0 panther   (1000) panther   (1000)     2693 2022-02-18 18:57:28.000000 pybliometrics-3.6/pybliometrics/scopus/superclasses/search.py
-drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-12-08 09:03:56.153818 pybliometrics-3.6/pybliometrics/scopus/tests/
--rw-r--r--   0 panther   (1000) panther   (1000)      668 2021-07-10 22:21:27.000000 pybliometrics-3.6/pybliometrics/scopus/tests/README.md
--rw-r--r--   0 panther   (1000) panther   (1000)        0 2020-01-13 10:35:18.000000 pybliometrics-3.6/pybliometrics/scopus/tests/__init__.py
--rw-rw-r--   0 panther   (1000) panther   (1000)    19912 2023-11-15 19:10:01.000000 pybliometrics-3.6/pybliometrics/scopus/tests/test_AbstractRetrieval.py
--rw-rw-r--   0 panther   (1000) panther   (1000)     3420 2021-10-16 15:30:16.000000 pybliometrics-3.6/pybliometrics/scopus/tests/test_AffiliationRetrieval.py
--rw-r--r--   0 panther   (1000) panther   (1000)     1124 2021-07-13 22:10:31.000000 pybliometrics-3.6/pybliometrics/scopus/tests/test_AffiliationSearch.py
--rw-rw-r--   0 panther   (1000) panther   (1000)    11646 2023-12-08 08:46:04.000000 pybliometrics-3.6/pybliometrics/scopus/tests/test_AuthorRetrieval.py
--rw-rw-r--   0 panther   (1000) panther   (1000)     1245 2023-10-16 19:39:37.000000 pybliometrics-3.6/pybliometrics/scopus/tests/test_AuthorSearch.py
--rw-r--r--   0 panther   (1000) panther   (1000)     4485 2023-11-04 11:35:39.000000 pybliometrics-3.6/pybliometrics/scopus/tests/test_CitationOverview.py
--rw-r--r--   0 panther   (1000) panther   (1000)     4063 2023-12-02 15:04:02.000000 pybliometrics-3.6/pybliometrics/scopus/tests/test_PlumXMetrics.py
--rw-r--r--   0 panther   (1000) panther   (1000)     5076 2021-12-24 13:29:19.000000 pybliometrics-3.6/pybliometrics/scopus/tests/test_ScopusSearch.py
--rw-r--r--   0 panther   (1000) panther   (1000)     1309 2021-06-13 19:14:51.000000 pybliometrics-3.6/pybliometrics/scopus/tests/test_SerialSearch.py
--rw-rw-r--   0 panther   (1000) panther   (1000)     4952 2023-12-02 12:24:09.000000 pybliometrics-3.6/pybliometrics/scopus/tests/test_SerialTitle.py
--rw-r--r--   0 panther   (1000) panther   (1000)     2025 2021-02-11 11:48:13.000000 pybliometrics-3.6/pybliometrics/scopus/tests/test_SubjectClassifications.py
-drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-12-08 09:03:56.153818 pybliometrics-3.6/pybliometrics/scopus/utils/
--rw-r--r--   0 panther   (1000) panther   (1000)      311 2021-06-14 19:12:26.000000 pybliometrics-3.6/pybliometrics/scopus/utils/__init__.py
--rw-r--r--   0 panther   (1000) panther   (1000)      267 2021-02-11 07:22:49.000000 pybliometrics-3.6/pybliometrics/scopus/utils/checks.py
--rw-r--r--   0 panther   (1000) panther   (1000)     2541 2023-01-19 14:41:04.000000 pybliometrics-3.6/pybliometrics/scopus/utils/constants.py
--rw-rw-r--   0 panther   (1000) panther   (1000)     2277 2023-04-03 07:41:51.000000 pybliometrics-3.6/pybliometrics/scopus/utils/create_config.py
--rw-rw-r--   0 panther   (1000) panther   (1000)     5844 2023-11-21 11:58:45.000000 pybliometrics-3.6/pybliometrics/scopus/utils/get_content.py
--rw-rw-r--   0 panther   (1000) panther   (1000)     6008 2023-12-08 08:46:32.000000 pybliometrics-3.6/pybliometrics/scopus/utils/parse_content.py
--rw-rw-r--   0 panther   (1000) panther   (1000)      648 2022-01-01 15:13:32.000000 pybliometrics-3.6/pybliometrics/scopus/utils/startup.py
-drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-12-08 09:03:56.157818 pybliometrics-3.6/pybliometrics.egg-info/
--rw-r--r--   0 panther   (1000) panther   (1000)     5062 2023-12-08 09:03:56.000000 pybliometrics-3.6/pybliometrics.egg-info/PKG-INFO
--rw-rw-r--   0 panther   (1000) panther   (1000)     2913 2023-12-08 09:03:56.000000 pybliometrics-3.6/pybliometrics.egg-info/SOURCES.txt
--rw-rw-r--   0 panther   (1000) panther   (1000)        1 2023-12-08 09:03:56.000000 pybliometrics-3.6/pybliometrics.egg-info/dependency_links.txt
--rw-rw-r--   0 panther   (1000) panther   (1000)       22 2023-12-08 09:03:56.000000 pybliometrics-3.6/pybliometrics.egg-info/requires.txt
--rw-rw-r--   0 panther   (1000) panther   (1000)       14 2023-12-08 09:03:56.000000 pybliometrics-3.6/pybliometrics.egg-info/top_level.txt
--rw-rw-r--   0 panther   (1000) panther   (1000)     1641 2023-04-18 19:28:48.000000 pybliometrics-3.6/pyproject.toml
--rw-rw-r--   0 panther   (1000) panther   (1000)       38 2023-12-08 09:03:56.157818 pybliometrics-3.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-25 09:45:57.156659 pybliometrics-4.0/
+drwxrwxrwx   0        0        0        0 2024-05-25 09:45:56.512945 pybliometrics-4.0/.github/
+drwxrwxrwx   0        0        0        0 2024-05-25 09:45:56.577245 pybliometrics-4.0/.github/ISSUE_TEMPLATE/
+-rw-rw-rw-   0        0        0      180 2024-01-15 10:04:22.000000 pybliometrics-4.0/.github/ISSUE_TEMPLATE/bug.md
+-rw-rw-rw-   0        0        0      167 2024-01-15 10:04:22.000000 pybliometrics-4.0/.github/ISSUE_TEMPLATE/feature.md
+-rw-rw-rw-   0        0        0      336 2024-01-15 10:04:22.000000 pybliometrics-4.0/.github/ISSUE_TEMPLATE/question.md
+-rw-rw-rw-   0        0        0      668 2024-01-15 10:04:22.000000 pybliometrics-4.0/.gitignore
+-rw-rw-rw-   0        0        0      168 2024-01-15 10:04:22.000000 pybliometrics-4.0/.readthedocs.yaml
+-rw-rw-rw-   0        0        0      819 2024-01-15 10:32:31.000000 pybliometrics-4.0/CITATION.cff
+-rw-rw-rw-   0        0        0     3174 2024-05-11 19:38:20.000000 pybliometrics-4.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     1442 2024-01-15 10:04:22.000000 pybliometrics-4.0/LICENSE
+-rw-rw-rw-   0        0        0     5421 2024-05-25 09:45:57.141035 pybliometrics-4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3762 2024-05-11 19:39:03.000000 pybliometrics-4.0/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-25 09:45:56.655365 pybliometrics-4.0/docs/
+-rw-rw-rw-   0        0        0      603 2024-01-15 10:04:22.000000 pybliometrics-4.0/docs/Makefile
+drwxrwxrwx   0        0        0        0 2024-05-25 09:45:56.655365 pybliometrics-4.0/docs/_static/
+-rw-rw-rw-   0        0        0       29 2024-05-11 19:38:20.000000 pybliometrics-4.0/docs/_static/custom.css.bak
+drwxrwxrwx   0        0        0        0 2024-05-25 09:45:56.677504 pybliometrics-4.0/docs/access/
+-rw-rw-rw-   0        0        0     3592 2024-05-11 19:38:20.000000 pybliometrics-4.0/docs/access/errors.rst
+-rw-rw-rw-   0        0        0     1799 2024-01-15 10:04:22.000000 pybliometrics-4.0/docs/access/general.rst
+-rw-rw-rw-   0        0        0     1059 2024-01-15 10:04:22.000000 pybliometrics-4.0/docs/access/quotas.rst
+-rw-rw-rw-   0        0        0      109 2024-01-15 10:04:22.000000 pybliometrics-4.0/docs/access.rst
+-rw-rw-rw-   0        0        0       33 2024-01-15 10:04:22.000000 pybliometrics-4.0/docs/authors.rst
+-rw-rw-rw-   0        0        0       33 2024-01-15 10:04:22.000000 pybliometrics-4.0/docs/changelog.rst
+drwxrwxrwx   0        0        0        0 2024-05-25 09:45:56.777763 pybliometrics-4.0/docs/classes/
+-rw-rw-rw-   0        0        0    12122 2024-05-11 20:54:44.000000 pybliometrics-4.0/docs/classes/AbstractRetrieval.rst
+-rw-rw-rw-   0        0        0     3423 2024-05-11 20:53:10.000000 pybliometrics-4.0/docs/classes/AffiliationRetrieval.rst
+-rw-rw-rw-   0        0        0     5163 2024-05-23 16:04:42.000000 pybliometrics-4.0/docs/classes/AffiliationSearch.rst
+-rw-rw-rw-   0        0        0     8278 2024-05-16 13:50:57.000000 pybliometrics-4.0/docs/classes/AuthorRetrieval.rst
+-rw-rw-rw-   0        0        0     4718 2024-05-11 20:33:42.000000 pybliometrics-4.0/docs/classes/AuthorSearch.rst
+-rw-rw-rw-   0        0        0     5900 2024-05-11 20:32:07.000000 pybliometrics-4.0/docs/classes/CitationOverview.rst
+-rw-rw-rw-   0        0        0     2852 2024-05-11 20:21:33.000000 pybliometrics-4.0/docs/classes/PlumXMetrics.rst
+-rw-rw-rw-   0        0        0    12496 2024-05-11 20:18:47.000000 pybliometrics-4.0/docs/classes/ScopusSearch.rst
+-rw-rw-rw-   0        0        0     4301 2024-05-11 20:16:21.000000 pybliometrics-4.0/docs/classes/SerialSearch.rst
+-rw-rw-rw-   0        0        0     7161 2024-05-11 20:12:28.000000 pybliometrics-4.0/docs/classes/SerialTitle.rst
+-rw-rw-rw-   0        0        0     4055 2024-05-11 20:13:14.000000 pybliometrics-4.0/docs/classes/SubjectClassifications.rst
+-rw-rw-rw-   0        0        0      804 2024-01-15 10:04:22.000000 pybliometrics-4.0/docs/classes.rst
+-rw-rw-rw-   0        0        0     2658 2024-05-11 19:38:20.000000 pybliometrics-4.0/docs/conf.py
+-rw-rw-rw-   0        0        0     4357 2024-05-11 19:40:45.000000 pybliometrics-4.0/docs/configuration.rst
+-rw-rw-rw-   0        0        0       33 2024-01-15 10:04:22.000000 pybliometrics-4.0/docs/contributing.rst
+-rw-rw-rw-   0        0        0     1644 2024-01-15 10:04:22.000000 pybliometrics-4.0/docs/index.rst
+-rw-rw-rw-   0        0        0      747 2024-01-15 10:04:22.000000 pybliometrics-4.0/docs/installation.rst
+-rwxrwxrwx   0        0        0      817 2024-01-15 10:04:22.000000 pybliometrics-4.0/docs/make.bat
+-rw-rw-rw-   0        0        0      111 2024-01-15 10:04:22.000000 pybliometrics-4.0/docs/requirements.txt
+drwxrwxrwx   0        0        0        0 2024-05-25 09:45:56.824637 pybliometrics-4.0/docs/tips/
+-rw-rw-rw-   0        0        0      915 2024-01-15 10:04:22.000000 pybliometrics-4.0/docs/tips/affiliations.rst
+-rw-rw-rw-   0        0        0      133 2024-01-15 10:04:22.000000 pybliometrics-4.0/docs/tips/configuration.rst
+-rw-rw-rw-   0        0        0     1388 2024-01-15 10:04:22.000000 pybliometrics-4.0/docs/tips/database.rst
+-rw-rw-rw-   0        0        0     4617 2024-01-15 10:04:22.000000 pybliometrics-4.0/docs/tips/migration1.rst
+-rw-rw-rw-   0        0        0      933 2024-05-25 09:05:36.000000 pybliometrics-4.0/docs/tips/migration3.rst
+-rw-rw-rw-   0        0        0      491 2024-01-15 10:04:22.000000 pybliometrics-4.0/docs/tips/rename.rst
+-rw-rw-rw-   0        0        0      661 2024-01-15 10:04:22.000000 pybliometrics-4.0/docs/tips/support.rst
+-rw-rw-rw-   0        0        0      238 2024-05-25 08:43:20.000000 pybliometrics-4.0/docs/tips.rst
+drwxrwxrwx   0        0        0        0 2024-05-25 09:45:56.840260 pybliometrics-4.0/meta/
+-rw-rw-rw-   0        0        0   903447 2024-01-15 10:04:22.000000 pybliometrics-4.0/meta/1-s2.0-S2352711019300573-main.pdf
+-rw-rw-rw-   0        0        0      290 2024-01-15 10:04:22.000000 pybliometrics-4.0/meta/AUTHORS.rst
+-rw-rw-rw-   0        0        0    26438 2024-05-25 09:40:39.000000 pybliometrics-4.0/meta/CHANGES.rst
+drwxrwxrwx   0        0        0        0 2024-05-25 09:45:56.855884 pybliometrics-4.0/pybliometrics/
+-rw-rw-rw-   0        0        0      382 2024-01-15 10:04:22.000000 pybliometrics-4.0/pybliometrics/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 09:45:56.978259 pybliometrics-4.0/pybliometrics/scopus/
+-rw-rw-rw-   0        0        0      615 2024-01-15 10:04:22.000000 pybliometrics-4.0/pybliometrics/scopus/__init__.py
+-rw-rw-rw-   0        0        0    12566 2024-05-23 16:58:54.000000 pybliometrics-4.0/pybliometrics/scopus/abstract_citation.py
+-rw-rw-rw-   0        0        0    41109 2024-05-11 19:38:20.000000 pybliometrics-4.0/pybliometrics/scopus/abstract_retrieval.py
+-rw-rw-rw-   0        0        0     7155 2024-05-16 14:17:53.000000 pybliometrics-4.0/pybliometrics/scopus/affiliation_retrieval.py
+-rw-rw-rw-   0        0        0     5689 2024-05-23 16:04:42.000000 pybliometrics-4.0/pybliometrics/scopus/affiliation_search.py
+-rw-rw-rw-   0        0        0    18948 2024-05-16 13:50:57.000000 pybliometrics-4.0/pybliometrics/scopus/author_retrieval.py
+-rw-rw-rw-   0        0        0     6409 2024-01-15 10:04:22.000000 pybliometrics-4.0/pybliometrics/scopus/author_search.py
+-rw-rw-rw-   0        0        0     2381 2024-01-15 10:04:22.000000 pybliometrics-4.0/pybliometrics/scopus/exception.py
+-rw-rw-rw-   0        0        0     6296 2024-01-15 10:04:22.000000 pybliometrics-4.0/pybliometrics/scopus/plumx_metrics.py
+-rw-rw-rw-   0        0        0    11149 2024-05-11 19:38:20.000000 pybliometrics-4.0/pybliometrics/scopus/scopus_search.py
+-rw-rw-rw-   0        0        0     7085 2024-05-11 19:38:20.000000 pybliometrics-4.0/pybliometrics/scopus/serial_search.py
+-rw-rw-rw-   0        0        0    12220 2024-05-11 19:38:20.000000 pybliometrics-4.0/pybliometrics/scopus/serial_title.py
+-rw-rw-rw-   0        0        0     4485 2024-05-11 19:38:20.000000 pybliometrics-4.0/pybliometrics/scopus/subject_classifications.py
+drwxrwxrwx   0        0        0        0 2024-05-25 09:45:56.993888 pybliometrics-4.0/pybliometrics/scopus/superclasses/
+-rw-rw-rw-   0        0        0      166 2024-01-15 10:04:22.000000 pybliometrics-4.0/pybliometrics/scopus/superclasses/__init__.py
+-rw-rw-rw-   0        0        0     8212 2024-05-11 19:38:20.000000 pybliometrics-4.0/pybliometrics/scopus/superclasses/base.py
+-rw-rw-rw-   0        0        0     1915 2024-05-11 19:38:20.000000 pybliometrics-4.0/pybliometrics/scopus/superclasses/retrieval.py
+-rw-rw-rw-   0        0        0     2822 2024-05-11 19:38:20.000000 pybliometrics-4.0/pybliometrics/scopus/superclasses/search.py
+drwxrwxrwx   0        0        0        0 2024-05-25 09:45:57.094165 pybliometrics-4.0/pybliometrics/scopus/tests/
+-rw-rw-rw-   0        0        0      572 2024-05-11 19:38:20.000000 pybliometrics-4.0/pybliometrics/scopus/tests/README.md
+-rw-rw-rw-   0        0        0        0 2024-01-15 10:04:22.000000 pybliometrics-4.0/pybliometrics/scopus/tests/__init__.py
+-rw-rw-rw-   0        0        0    19483 2024-05-11 19:38:20.000000 pybliometrics-4.0/pybliometrics/scopus/tests/test_AbstractRetrieval.py
+-rw-rw-rw-   0        0        0     4198 2024-05-23 16:29:46.000000 pybliometrics-4.0/pybliometrics/scopus/tests/test_AffiliationRetrieval.py
+-rw-rw-rw-   0        0        0     1009 2024-05-23 16:04:42.000000 pybliometrics-4.0/pybliometrics/scopus/tests/test_AffiliationSearch.py
+-rw-rw-rw-   0        0        0    10585 2024-05-16 13:50:57.000000 pybliometrics-4.0/pybliometrics/scopus/tests/test_AuthorRetrieval.py
+-rw-rw-rw-   0        0        0     1130 2024-05-11 19:38:20.000000 pybliometrics-4.0/pybliometrics/scopus/tests/test_AuthorSearch.py
+-rw-rw-rw-   0        0        0     4119 2024-05-11 19:38:20.000000 pybliometrics-4.0/pybliometrics/scopus/tests/test_CitationOverview.py
+-rw-rw-rw-   0        0        0     3735 2024-05-11 19:38:20.000000 pybliometrics-4.0/pybliometrics/scopus/tests/test_PlumXMetrics.py
+-rw-rw-rw-   0        0        0     4942 2024-05-11 19:38:20.000000 pybliometrics-4.0/pybliometrics/scopus/tests/test_ScopusSearch.py
+-rw-rw-rw-   0        0        0     1184 2024-05-11 19:38:20.000000 pybliometrics-4.0/pybliometrics/scopus/tests/test_SerialSearch.py
+-rw-rw-rw-   0        0        0     4655 2024-05-11 19:38:20.000000 pybliometrics-4.0/pybliometrics/scopus/tests/test_SerialTitle.py
+-rw-rw-rw-   0        0        0     1854 2024-05-11 19:38:20.000000 pybliometrics-4.0/pybliometrics/scopus/tests/test_SubjectClassifications.py
+drwxrwxrwx   0        0        0        0 2024-05-25 09:45:57.141035 pybliometrics-4.0/pybliometrics/scopus/utils/
+-rw-rw-rw-   0        0        0      311 2024-01-15 10:04:22.000000 pybliometrics-4.0/pybliometrics/scopus/utils/__init__.py
+-rw-rw-rw-   0        0        0      267 2024-01-15 10:04:22.000000 pybliometrics-4.0/pybliometrics/scopus/utils/checks.py
+-rw-rw-rw-   0        0        0     3146 2024-05-11 19:38:20.000000 pybliometrics-4.0/pybliometrics/scopus/utils/constants.py
+-rw-rw-rw-   0        0        0     2430 2024-02-26 14:11:31.000000 pybliometrics-4.0/pybliometrics/scopus/utils/create_config.py
+-rw-rw-rw-   0        0        0     5232 2024-05-25 08:31:59.000000 pybliometrics-4.0/pybliometrics/scopus/utils/get_content.py
+-rw-rw-rw-   0        0        0     6008 2024-01-15 10:04:22.000000 pybliometrics-4.0/pybliometrics/scopus/utils/parse_content.py
+-rw-rw-rw-   0        0        0     2778 2024-05-11 19:38:20.000000 pybliometrics-4.0/pybliometrics/scopus/utils/startup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 09:45:57.141035 pybliometrics-4.0/pybliometrics.egg-info/
+-rw-rw-rw-   0        0        0     5421 2024-05-25 09:45:56.000000 pybliometrics-4.0/pybliometrics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2955 2024-05-25 09:45:56.000000 pybliometrics-4.0/pybliometrics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 09:45:56.000000 pybliometrics-4.0/pybliometrics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-05-25 09:45:56.000000 pybliometrics-4.0/pybliometrics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-25 09:45:56.000000 pybliometrics-4.0/pybliometrics.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1765 2024-05-25 09:40:39.000000 pybliometrics-4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-25 09:45:57.156659 pybliometrics-4.0/setup.cfg
```

### Comparing `pybliometrics-3.6/.gitignore` & `pybliometrics-4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.6/CONTRIBUTING.rst` & `pybliometrics-4.0/CONTRIBUTING.rst`

 * *Files 8% similar despite different names*

```diff
@@ -87,9 +87,9 @@
 
 Pull Request Guidelines
 -----------------------
 
 Before you submit a pull request, check that it meets these guidelines:
 
 1. Adhere to `PEP8 <https://www.python.org/dev/peps/pep-0008/>`_
-2. Run nosetests locally `python -m nose --verbose` (on Windows) or `nosetests3 pybliometrics/scopus/tests/ --verbose`.
+2. Run tests locally `python -m pytest --verbose` (on Windows) or `pytest pybliometrics/scopus/tests/ --verbose`.
 3. The pull request should work for Python 3.X.
```

### Comparing `pybliometrics-3.6/LICENSE` & `pybliometrics-4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.6/PKG-INFO` & `pybliometrics-4.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,139 +1,144 @@
-Metadata-Version: 2.1
-Name: pybliometrics
-Version: 3.6
-Summary: Python-based API-Wrapper to access Scopus
-Author-email: "'John Kitchin and Michael E. Rose" <Michael.Ernst.Rose@gmail.com>
-Maintainer-email: "Michael E. Rose" <Michael.Ernst.Rose@gmail.com>
-License: MIT
-Project-URL: Homepage, https://github.com/pybliometrics-dev/pybliometrics
-Project-URL: Bug Tracker, https://github.com/pybliometrics-dev/pybliometrics/issues
-Project-URL: Documentation (stable), https://pybliometrics.readthedocs.io/en/stable/
-Project-URL: Documentation (latest), https://pybliometrics.readthedocs.io/en/latest/
-Keywords: scopus
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: tqdm
-Requires-Dist: urllib3
-
-pybliometrics
-=============
-
-Enables large-scale access to Elsevier's Scopus API from Python.
-
-Documentation: https://pybliometrics.readthedocs.io
-
-Development: https://github.com/pybliometrics-dev/pybliometrics
-
-.. image:: https://badge.fury.io/py/pybliometrics.svg
-    :target: https://badge.fury.io/py/pybliometrics
-
-.. image:: https://img.shields.io/pypi/pyversions/pybliometrics.svg
-    :target: https://img.shields.io/pypi/pyversions/pybliometrics.svg
-
-.. image:: https://readthedocs.org/projects/pybliometrics/badge/?version=stable
-    :target: https://readthedocs.org/projects/pybliometrics/badge/?version=stable
-
-.. image:: https://img.shields.io/pypi/dm/pybliometrics.svg
-    :target: https://img.shields.io/pypi/dm/pybliometrics.svg
-
-.. image:: https://img.shields.io/pypi/l/pybliometrics.svg
-    :target: https://img.shields.io/pypi/l/pybliometrics.svg
-
-.. image:: https://api.codeclimate.com/v1/badges/a4d7edd206a1252dfcfe/maintainability
-   :target: https://codeclimate.com/github/pybliometrics-dev/pybliometrics/maintainability
-
-Example
-=======
-.. example-begin
-.. code:: python
-
-    >>> # Document-specific information
-    >>> from pybliometrics.scopus import AbstractRetrieval
-    >>> ab = AbstractRetrieval("10.1016/j.softx.2019.100263")
-    >>> ab.title
-    'pybliometrics: Scriptable bibliometrics using a Python interface to Scopus'
-    >>> ab.publicationName
-    'SoftwareX'
-    >>> ab.authors
-    [Author(auid=57209617104, indexed_name='Rose M.E.', surname='Rose',
-     given_name='Michael E.', affiliation='60105007'),
-     Author(auid=7004212771, indexed_name='Kitchin J.R.', surname='Kitchin',
-     given_name='John R.', affiliation='60027950')]
-    >>> 
-    >>> # Author-specific information
-    >>> from pybliometrics.scopus import AuthorRetrieval
-    >>> au2 = AuthorRetrieval(ab.authors[1].auid)
-    >>> au2.h_index
-    34
-    >>> au1 = AuthorRetrieval(ab.authors[0].auid)
-    >>> au1.affiliation_current
-    [Affiliation(id=60105007, parent=None, type='parent', relationship='author',
-     afdispname=None, preferred_name='Max Planck Institute for Innovation and Competition',
-     parent_preferred_name=None, country_code='deu', country='Germany',
-     address_part='Marstallplatz 1', city='Munich', state='Bayern',
-     postal_code='80539', org_domain='ip.mpg.de', org_URL='http://www.ip.mpg.de/')]
-    >>> 
-    >>> # Affiliation information
-    >>> from pybliometrics.scopus import AffiliationRetrieval
-    >>> aff1 = AffiliationRetrieval(au1.affiliation_current[0].id)
-    >>> aff1.author_count
-    98
-
-.. example-end
-
-Installation
-============
-
-.. installation-begin
-
-Install the stable version from PyPI:
-
-.. code-block:: bash
-
-    pip install pybliometrics
-
-or the development version from the GitHub repository (requires git on your system):
-
-.. code-block:: bash
-
-    pip install git+https://github.com/pybliometrics-dev/pybliometrics
-
-.. installation-end
-
-Citation
-========
-
-If pybliometrics helped you getting data for research, please cite our corresponding paper:
-
-* Rose, Michael E. and John R. Kitchin: "`pybliometrics: Scriptable bibliometrics using a Python interface to Scopus <./meta/1-s2.0-S2352711019300573-main.pdf>`_", SoftwareX 10 (2019) 100263.
-
-Citing the paper helps the development of pybliometrics, because it justifies funneling resources into the development.  It also signals that you obtained data from Scopus in a transparent and replicable way.
-
-Change log
-==========
-
-Please see `CHANGES.rst <./meta/CHANGES.rst>`_.
-
-Contributing
-============
-
-Please see `CONTRIBUTING.rst <CONTRIBUTING.rst>`_. For a list of contributors see
-`AUTHORS.rst <./meta/AUTHORS.rst>`_.
-
-License
-=======
-
-MIT License; see `LICENSE <LICENSE>`_.
+Metadata-Version: 2.1
+Name: pybliometrics
+Version: 4.0
+Summary: Python-based API-Wrapper to access Scopus
+Author-email: "'John Kitchin and Michael E. Rose" <Michael.Ernst.Rose@gmail.com>
+Maintainer-email: "Michael E. Rose" <Michael.Ernst.Rose@gmail.com>
+License: MIT
+Project-URL: Homepage, https://github.com/pybliometrics-dev/pybliometrics
+Project-URL: Bug Tracker, https://github.com/pybliometrics-dev/pybliometrics/issues
+Project-URL: Documentation (stable), https://pybliometrics.readthedocs.io/en/stable/
+Project-URL: Documentation (latest), https://pybliometrics.readthedocs.io/en/latest/
+Keywords: scopus
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Documentation :: Sphinx
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: tqdm
+Requires-Dist: urllib3
+
+pybliometrics
+=============
+
+Enables large-scale access to Elsevier's Scopus API from Python.
+
+Documentation: https://pybliometrics.readthedocs.io
+
+Development: https://github.com/pybliometrics-dev/pybliometrics
+
+.. image:: https://badge.fury.io/py/pybliometrics.svg
+    :target: https://badge.fury.io/py/pybliometrics
+
+.. image:: https://img.shields.io/pypi/pyversions/pybliometrics.svg
+    :target: https://img.shields.io/pypi/pyversions/pybliometrics.svg
+
+.. image:: https://readthedocs.org/projects/pybliometrics/badge/?version=stable
+    :target: https://readthedocs.org/projects/pybliometrics/badge/?version=stable
+
+.. image:: https://img.shields.io/pypi/dm/pybliometrics.svg
+    :target: https://img.shields.io/pypi/dm/pybliometrics.svg
+
+.. image:: https://img.shields.io/pypi/l/pybliometrics.svg
+    :target: https://img.shields.io/pypi/l/pybliometrics.svg
+
+.. image:: https://api.codeclimate.com/v1/badges/a4d7edd206a1252dfcfe/maintainability
+   :target: https://codeclimate.com/github/pybliometrics-dev/pybliometrics/maintainability
+
+Example
+=======
+.. example-begin
+.. code:: python
+
+    >>> import pybliometrics
+    >>> pybliometrics.init()  # read API keys
+    >>> # Document-specific information
+    >>> from pybliometrics.scopus import AbstractRetrieval
+    >>> ab = AbstractRetrieval("10.1016/j.softx.2019.100263")
+    >>> ab.title
+    'pybliometrics: Scriptable bibliometrics using a Python interface to Scopus'
+    >>> ab.publicationName
+    'SoftwareX'
+    >>> ab.authors
+    [Author(auid=57209617104, indexed_name='Rose M.E.', surname='Rose',
+     given_name='Michael E.', affiliation='60105007'),
+     Author(auid=7004212771, indexed_name='Kitchin J.R.', surname='Kitchin',
+     given_name='John R.', affiliation='60027950')]
+    >>> 
+    >>> # Author-specific information
+    >>> from pybliometrics.scopus import AuthorRetrieval
+    >>> au2 = AuthorRetrieval(ab.authors[1].auid)
+    >>> au2.h_index
+    34
+    >>> au1 = AuthorRetrieval(ab.authors[0].auid)
+    >>> au1.affiliation_current
+    [Affiliation(id=60105007, parent=None, type='parent', relationship='author',
+     afdispname=None, preferred_name='Max Planck Institute for Innovation and Competition',
+     parent_preferred_name=None, country_code='deu', country='Germany',
+     address_part='Marstallplatz 1', city='Munich', state='Bayern',
+     postal_code='80539', org_domain='ip.mpg.de', org_URL='http://www.ip.mpg.de/')]
+    >>> 
+    >>> # Affiliation information
+    >>> from pybliometrics.scopus import AffiliationRetrieval
+    >>> aff1 = AffiliationRetrieval(au1.affiliation_current[0].id)
+    >>> aff1.author_count
+    98
+
+.. example-end
+
+Installation
+============
+
+.. installation-begin
+
+Install the stable version from PyPI:
+
+.. code-block:: bash
+
+    pip install pybliometrics
+
+or the development version from the GitHub repository (requires git on your system):
+
+.. code-block:: bash
+
+    pip install git+https://github.com/pybliometrics-dev/pybliometrics
+
+.. installation-end
+
+Citation
+========
+
+If pybliometrics helped you getting data for research, please cite our corresponding paper:
+
+* Rose, Michael E. and John R. Kitchin: "`pybliometrics: Scriptable bibliometrics using a Python interface to Scopus <./meta/1-s2.0-S2352711019300573-main.pdf>`_", SoftwareX 10 (2019) 100263.
+
+Citing the paper helps the development of pybliometrics, because it justifies funneling resources into the development.  It also signals that you obtained data from Scopus in a transparent and replicable way.
+
+Change log
+==========
+
+Please see `CHANGES.rst <./meta/CHANGES.rst>`_.
+
+Contributing
+============
+
+Please see `CONTRIBUTING.rst <CONTRIBUTING.rst>`_. For a list of contributors see
+`AUTHORS.rst <./meta/AUTHORS.rst>`_.
+
+License
+=======
+
+MIT License; see `LICENSE <LICENSE>`_.
```

### Comparing `pybliometrics-3.6/README.rst` & `pybliometrics-4.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,16 @@
    :target: https://codeclimate.com/github/pybliometrics-dev/pybliometrics/maintainability
 
 Example
 =======
 .. example-begin
 .. code:: python
 
+    >>> import pybliometrics
+    >>> pybliometrics.init()  # read API keys
     >>> # Document-specific information
     >>> from pybliometrics.scopus import AbstractRetrieval
     >>> ab = AbstractRetrieval("10.1016/j.softx.2019.100263")
     >>> ab.title
     'pybliometrics: Scriptable bibliometrics using a Python interface to Scopus'
     >>> ab.publicationName
     'SoftwareX'
```

### Comparing `pybliometrics-3.6/docs/Makefile` & `pybliometrics-4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.6/docs/access/errors.rst` & `pybliometrics-4.0/docs/access/errors.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
       * `pybliometrics.scopus.exception.Scopus404Error: NOT FOUND`: The entity you are looking for does not exist.  Check that your identifier is still pointing to the item you are looking for.
 
       * `pybliometrics.scopus.exception.Scopus413Error`: The request entity is too large to be processed by the web server.  Try a less complex query.
 
       * `pybliometrics.scopus.exception.Scopus414Error: TOO LARGE`: The query string you are using is too long.  Break it up in smaller pieces.
 
-      .. _Scopus429Error:
+          .. _Scopus429Error:
 
       * `pybliometrics.scopus.exception.Scopus429Error: QUOTA EXCEEDED`: Your provided API key's weekly quota has been depleted.  If you provided multiple keys in your :doc:`configuration file <../configuration>`, this means all your keys are depleted.  In this case, wait up to week until your API key's quota has been reset.
 
       * `pybliometrics.scopus.exception.ScopusServerError`: General exception related to all Server-related exceptions defined below.  This may happen for various reasons (the internet is a noisy medium); usually it helps to wait few seconds before the next query.  Server errors are also raised if you use a non-existent fieldname in searches.  Verify that your query works in Scopus' `Advanced Search <https://www.scopus.com/search/form.uri?display=advanced>`_.  Previously `pybliometrics` used more fine-grained exceptions in the 5xx space, namely "Scopus500Error", "Scopus502Error" and "Scopus504Error".  These are deprecated, use "ScopusServerError" instead.
 
 If queries break for other reasons, exceptions of type `requests.exceptions <https://requests.readthedocs.io/en/latest/api/?highlight=exceptions#exceptions>`_ are raised, such as:
```

### Comparing `pybliometrics-3.6/docs/access/general.rst` & `pybliometrics-4.0/docs/access/general.rst`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.6/docs/access/quotas.rst` & `pybliometrics-4.0/docs/access/quotas.rst`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.6/docs/classes/AbstractRetrieval.rst` & `pybliometrics-4.0/docs/classes/AbstractRetrieval.rst`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
 `AbstractRetrieval()` implements the `Scopus Abstract Retrieval API <https://dev.elsevier.com/documentation/AbstractRetrievalAPI.wadl>`_.
 
 It accepts any identifier as the main argument.  Most commonly, this will be a `Scopus EID <http://kitchingroup.cheme.cmu.edu/blog/2015/06/07/Getting-a-Scopus-EID-from-a-DOI/>`_, but DOI, Scopus ID (the last part of the EID), PubMed identifier or Publisher Item Identifier (PII) work as well.  `AbstractRetrieval` tries to infer the class itself - to speed this up you can tell the ID type via `ID_type`.
 
 The Abstract Retrieval API allows a differing information depth via `views <https://dev.elsevier.com/guides/AbstractRetrievalViews.htm>`_, some of which are restricted.  The 'META_ABS' view is the most comprehensive among unrestricted views, encompassing all information from other unrestricted views.  It is therefore the default view.  The view with the most information content is 'FULL', which includes all information available with 'META_ABS', but is restricted.  Generally, you should always try to use `view='FULL'` when downloading an abstract and fall back to the default otherwise.
 
+In addition, the 'ENTITLED' view lets you check you whether you have access to this class.
+
 .. currentmodule:: pybliometrics.scopus
 .. contents:: Table of Contents
     :local:
 
 Documentation
 -------------
 
@@ -20,28 +22,31 @@
 
 Examples
 --------
 You initialize the class with an ID that Scopus uses, e.g. the EID:
 
 .. code-block:: python
 
+	>>> import pybliometrics
     >>> from pybliometrics.scopus import AbstractRetrieval
+	>>> pybliometrics.scopus.init()
     >>> ab = AbstractRetrieval("2-s2.0-85068268027", view='FULL')
 
 
 You can obtain basic information just by printing the object:
 
 .. code-block:: python
 
     >>> print(ab)
-    Michael E. Rose and John R. Kitchin: "pybliometrics: Scriptable bibliometrics using a Python interface to Scopus", SoftwareX, 10, (no pages found)(2019). https://doi.org/10.1016/j.softx.2019.100263.
-    34 citation(s) as of 2022-04-07
-      Affiliation(s):
-       Max Planck Institute for Innovation and Competition
-       Carnegie Mellon University
+    Michael E. Rose and John R. Kitchin: "pybliometrics: Scriptable bibliometrics using a Python interface to Scopus",
+	SoftwareX, 10, (no pages found)(2019). https://doi.org/10.1016/j.softx.2019.100263.
+	110 citation(s) as of 2024-05-11
+	  Affiliation(s):
+	   Max Planck Institute for Innovation and Competition
+	   Carnegie Mellon University
 
 
 There are 52 attributes and 8 methods to interact with.  For example, to obtain bibliographic information:
 
 .. code-block:: python
 
     >>> ab.publicationName
@@ -77,15 +82,15 @@
 
 
 To obtain the total citation count (at the time the abstract was retrieved and cached):
 
 .. code-block:: python
 
     >>> ab.citedby_count
-    34
+    110
 
 
 You can retrieve the authors as a list of `namedtuples <https://docs.python.org/3/library/collections.html#collections.namedtuple>`_, which pair conveniently with `pandas <https://pandas.pydata.org/>`_:
 
 .. code-block:: python
 
     >>> ab.authors
```

### Comparing `pybliometrics-3.6/docs/classes/AffiliationRetrieval.rst` & `pybliometrics-4.0/docs/classes/AffiliationRetrieval.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 pybliometrics.scopus.AffiliationRetrieval
 =========================================
 
 `AffiliationRetrieval()` implements the `Affiliation Retrieval API <https://dev.elsevier.com/documentation/AffiliationRetrievalAPI.wadl>`_. It provides basic information on registered affiliations, such as city, country, its members, and more.
 
+In addition, the 'ENTITLED' view lets you check you whether you have access to this class.
+
 .. currentmodule:: pybliometrics.scopus
 .. contents:: Table of Contents
     :local:
 
 Documentation
 -------------
 
@@ -17,25 +19,27 @@
 Examples
 --------
 
 You initialize the class using Scopus' Affiliation ID:
 
 .. code-block:: python
 
+    >>> import pybliometrics
     >>> from pybliometrics.scopus import AffiliationRetrieval
+	>>> pybliometrics.scopus.init()
     >>> aff = AffiliationRetrieval(60000356)
 
 
 You can obtain basic information just by printing the object:
 
 .. code-block:: python
 
     >>> print(aff)
     University of Cape Town in Cape Town in South Africa,
-    has 13,033 associated author(s) and 75,695 associated document(s) as of 2021-07-12
+    has 14,109 associated author(s) and 89,376 associated document(s) as of 2024-05-11
 
 
 The object has several of attributes but no methods.  For example, information regarding the affiliation itself:
 
 .. code-block:: python
 
     >>> aff.affiliation_name
@@ -59,39 +63,40 @@
 
 
 There are meta-information, too:
 
 .. code-block:: python
 
     >>> aff.author_count
-    13033
+    14109
     >>> aff.document_count
-    75695
+    89376
 
 
 Scopus also collects information on different names affiliated authors use for this affiliation, which `pybliometrics` returns as list of `namedtuples <https://docs.python.org/3/library/collections.html#collections.namedtuple>`_:
 
 .. code-block:: python
 
     >>> aff.name_variants
-    [Variant(name='University Of Cape Town', doc_count=60095),
-     Variant(name='Univ. Cape Town', doc_count=1659),
-     Variant(name='Univ Of Cape Town', doc_count=772),
-     Variant(name='Univ. Of Cape Town', doc_count=392)]
+    [Variant(name='University Of Cape Town', doc_count=85821),
+	 Variant(name='Univ. Cape Town', doc_count=1622),
+	 Variant(name='Univ Of Cape Town', doc_count=729),
+	 Variant(name='Institute Of Infectious Disease And Molecular Medicine', doc_count=608),
+	 Variant(name='Department Of Molecular And Cell Biology', doc_count=596)]
 
 
 Using `pandas <https://pandas.pydata.org/>`_, you can easily convert this into a DataFrame:
 
 .. code-block:: python
 
     >>> import pandas as pd
     >>> print(pd.DataFrame(aff.name_variants))
                           name doc_count
-    0  University Of Cape Town     60095
-    1          Univ. Cape Town      1659
-    2        Univ Of Cape Town       772
-    3       Univ. Of Cape Town       392
+    0  University Of Cape Town     85821
+    1          Univ. Cape Town       729
+    2        Univ Of Cape Town       608
+    3       Univ. Of Cape Town       596
 
 
 More on different types of affiliations in section `tips <../tips.html#affiliations>`_.
 
 Downloaded results are cached to expedite subsequent analyses.  This information may become outdated.  To refresh the cached results if they exist, set `refresh=True`, or provide an integer that will be interpreted as maximum allowed number of days since the last modification date.  For example, if you want to refresh all cached results older than 100 days, set `refresh=100`.  Use `ab.get_cache_file_mdate()` to obtain the date of last modification, and `ab.get_cache_file_age()` to determine the number of days since the last modification.
```

### Comparing `pybliometrics-3.6/docs/classes/AffiliationSearch.rst` & `pybliometrics-4.0/docs/classes/AffiliationSearch.rst`

 * *Files 4% similar despite different names*

```diff
@@ -17,76 +17,81 @@
 Examples
 --------
 
 The class is initialized using a search query, details of which can be found in `Affiliation Search Guide <https://dev.elsevier.com/tips/AffiliationSearchTips.htm>`_.  An invalid search query results in an error.
 
 .. code-block:: python
 
+    >>> import pybliometrics
     >>> from pybliometrics.scopus import AffiliationSearch
+	>>> pybliometrics.scopus.init()
     >>> query = "AFFIL(Max Planck Institute for Innovation and Competition Munich)"
     >>> s = AffiliationSearch(query)
 
 
 You can obtain a search summary just by printing the object:
 
 .. code-block:: python
 
     >>> print(s)
     Search 'AFFIL(Max Planck Institute for Innovation and Competition Munich)' yielded
-    2 affiliations as of 2021-01-15:
-        Max Planck Institute for Innovation and Competition
-        Max Planck Institute for Competition and Innovation
+	2 affiliations as of 2024-05-11:
+		Max Planck Institute for Innovation and Competition
+		Max Planck Insitute for Innovation and Com-petition in Munich
 
 
 The primary function of the class is to provide a list of `namedtuples <https://docs.python.org/3/library/collections.html#collections.namedtuple>`_, each storing information about the affiliation.  One of them is the affiliation ID which you can use for the :doc:`AffiliationRetrieval <../classes/AffiliationRetrieval>` class:
 
 .. code-block:: python
 
     >>> s.affiliations
-    [Affiliation(eid='10-s2.0-60105007', name='Max Planck Institute for Innovation and Competition',
-                 variant='Max Planck Institute For Innovation And Competition', documents=380,
-                 city='Munich', country='Germany', parent='0'),
-     Affiliation(eid='10-s2.0-117495104', name='Max Planck Institute for Competition and Innovation',
-                 variant='Max-plank Institut', documents=3, city='Munich', country='Germany',
-                 parent='0')]
+    [Affiliation(eid='10-s2.0-60105007',
+			     name='Max Planck Institute for Innovation and Competition',
+				 variant='Max Planck Institute For Innovation And Competition',
+				 documents=581, city='Munich', country='Germany', parent=None),
+	 Affiliation(eid='10-s2.0-117495104',
+				 name='Max Planck Insitute for Innovation and Com-petition in Munich',
+				 variant='Max-plank Institut',
+				 documents=4, city='Munich', country='Germany', parent=None)]
+
 
 
 Working with namedtuples is straightforward: using `pandas <https://pandas.pydata.org/>`_ for example you can quickly convert the results into a DataFrame:
 
 .. code-block:: python
 
     >>> import pandas as pd
     >>> pd.set_option('display.max_columns', None)
     >>> print(pd.DataFrame(s.affiliations))
                      eid                                               name  \
     0   10-s2.0-60105007  Max Planck Institute for Innovation and Compet...   
     1  10-s2.0-117495104  Max Planck Institute for Competition and Innov...   
 
                                                  variant  documents    city  \
-    0  Max Planck Institute For Innovation And Compet...        380  Munich   
-    1                                 Max-plank Institut          3  Munich   
+    0  Max Planck Institute For Innovation And Compet...        581  Munich   
+    1                                 Max-plank Institut          4  Munich   
 
        country parent  
-    0  Germany      0  
-    1  Germany      0 
+    0  Germany      None  
+    1  Germany      None 
 
 
 Comparing the EIDs, notice that the first affiliation's EID starts with 10-s2.0-6, while the other begins with 10-s2.0-1.  The latter denotes a non-org affiliation type.  
 More on different types of affiliations in section `tips <../tips.html#affiliations>`_.
 
 Downloaded results are cached to expedite subsequent analyses.  This information may become outdated.  To refresh the cached results if they exist, set `refresh=True`, or provide an integer that will be interpreted as maximum allowed number of days since the last modification date.  For example, if you want to refresh all cached results older than 100 days, set `refresh=100`.  Use `ab.get_cache_file_mdate()` to obtain the date of last modification, and `ab.get_cache_file_age()` to determine the number of days since the last modification.
 
 You can determine the number of results using the `.get_results_size()` method, even before you download the results:
 
 .. code-block:: python
 
     >>> query = "AFFIL(Max Planck Institute)"
     >>> s = AffiliationSearch(query, download=False)
     >>> s.get_results_size()
-    398
+    537
 
 
 Sometimes, information that exists in the Scopus database may be missing in the returned results.  For example, the EID may be missing, even though every element always has an EID.  This is not a bug of `pybliometrics`.  Instead it is somehow related to a problem in the download process from the Scopus database.  To check for completeness of specific fields, use parameter `integrity_fields`, which accepts any iterable.  Using the`integrity_action` parameter, you can choose between two actions if the integrity check fails: Set `integrity_action="warn"` to issue a UserWarning, or set `integrity_action="raise"` to raise an AttributeError.
 
 .. code-block:: python
 
     >>> s = AffiliationSearch(query, integrity_fields=["eid"], integrity_action="warn")
```

### Comparing `pybliometrics-3.6/docs/classes/AuthorRetrieval.rst` & `pybliometrics-4.0/docs/classes/AuthorRetrieval.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 pybliometrics.scopus.AuthorRetrieval
 ====================================
 
 `AuthorRetrieval()` implements the `Author Retrieval API <https://dev.elsevier.com/documentation/AuthorRetrievalAPI.wadl>`_. It provides a complete author record according to Scopus.
 
+In addition, the 'ENTITLED' view lets you check you whether you have access to this class.
+
 .. currentmodule:: pybliometrics.scopus
 .. contents:: Table of Contents
     :local:
 
 Documentation
 -------------
 
@@ -17,26 +19,28 @@
 Examples
 --------
 
 You initiate the class with the author's Scopus ID, which can be either an integer or a string:
 
 .. code-block:: python
 
+    >>> import pybliometrics
     >>> from pybliometrics.scopus import AuthorRetrieval
+	>>> pybliometrics.scopus.init()
     >>> au = AuthorRetrieval(7004212771)
 
 
 You can obtain basic information just by printing the object:
 
 .. code-block:: python
 
     >>> print(au)
-    Kitchin J. from Department of Chemical Engineering in United States,
-    published 108 document(s) since 1995
-    which were cited by 11,980 author(s) in 14,861 document(s) as of 2021-07-14
+    Kitchin J. from Carnegie Mellon University in United States,
+	published 126 document(s) since 1995 
+	which were cited by 20,897 author(s) in 25,490 document(s) as of 2024-05-11
 
 
 This object provides access to various data about an author, including the number of papers, h-index, current affiliation, etc.  When a list of `namedtuples <https://docs.python.org/3/library/collections.html#collections.namedtuple>`_ is returned, it can neatly be turned into a `pandas <https://pandas.pydata.org/>`_ DataFrame.
 
 Information regarding the author's names includes:
 
 .. code-block:: python
@@ -47,62 +51,63 @@
     'Kitchin'
     >>> au.given_name
     'John R.'
     >>> au.initials
     'J.R.'
     >>> au.name_variants
     [Variant(indexed_name='Kitchin J.', initials='J.R.', surname='Kitchin',
-     given_name='John R.', doc_count=90),
+     given_name='John R.', doc_count=104),
      Variant(indexed_name='Kitchin J.', initials='J.', surname='Kitchin',
-     given_name='John', doc_count=11),
+     given_name='John', doc_count=13),
      Variant(indexed_name='Kitchin J.', initials='J.R.', surname='Kitchin',
      given_name='J. R.', doc_count=8)]
     >>> au.eid
     '9-s2.0-7004212771'
 
 
 Bibliometric information includes:
 
 .. code-block:: python
 
     >>> au.citation_count
-    14861
+    25490
     >>> au.document_count
-    108
+    126
     >>> au.h_index
-    34
+    40
     >>> au.orcid
     '0000-0003-2625-9232'
     >>> au.publication_range
     (1995, 2021)
     >>> import pandas as pd
     >>> areas = pd.DataFrame(au.subject_areas)
     >>> areas.shape
-    (49, 3)
+    (55, 3)
     >>> areas.head()
-                                area abbreviation  code
-    0                Safety Research         SOCI  3311
-    1           Analytical Chemistry         CHEM  1602
-    2        Modeling and Simulation         MATH  2611
-    3        Materials Science (all)         MATE  2500
-    4  Colloid and Surface Chemistry         CENG  1505
+        area abbreviation  code
+	0              Analytical Chemistry         CHEM  1602
+	1                   Safety Research         SOCI  3311
+	2  Process Chemistry and Technology         CENG  1508
+	3           Materials Science (all)         MATE  2500
+	4           Modeling and Simulation         MATH  2611
     >>> au.classificationgroup
-    [('3311', '4'), ('1602', '1'), ('2611', '5'), ('2500', '11'),
-     ('1505', '1'), ('1605', '4'), ('1303', '2'), ('2504', '10'),
-     ('1508', '3'), ('1706', '2'), ('1712', '1'), ('2209', '5'),
-     ('2105', '1'), ('1504', '2'), ('1500', '26'), ('3309', '1'),
-     ('1600', '28'), ('2508', '14'), ('2310', '2'), ('1503', '22'),
-     ('2300', '1'), ('2102', '3'), ('3107', '3'), ('1000', '1'),
-     ('3110', '9'), ('2213', '7'), ('2505', '6'), ('3100', '9'),
-     ('1906', '1'), ('1305', '3'), ('2304', '1'), ('1604', '2'),
-     ('1909', '1'), ('2207', '2'), ('2200', '2'), ('1607', '1'),
-     ('2103', '3'), ('2308', '2'), ('3104', '21'), ('1311', '1'),
-     ('1603', '3'), ('2305', '2'), ('1606', '24'), ('2503', '1'),
-     ('2100', '11'), ('2208', '1'), ('1502', '2'), ('2104', '2'),
-     ('1710', '5')]
+    [(1602, 1), (3311, 4), (1508, 6),  (2500, 13),
+	 (2611, 6), (1505, 1), (1605, 7), (1303, 2),
+	 (1501, 2), (1706, 4), (2504, 13), (1500, 42),
+	 (1503, 33), (2105, 1), (3100, 13), (2209, 11),
+     (1712, 3), (1709, 2), (1504, 2), (1702, 2),
+	 (3309, 3), (2310, 3), (1507, 2), (2508, 17),
+	 (2300, 2), (3107, 3), (2102, 6), (3110, 9),
+	 (1000, 1), (1600, 40), (1601, 3), (2213, 7),
+	 (2505, 6), (1906, 1), (1305, 8), (2700, 6),
+	 (2304, 2), (1604, 3), (1909, 1), (2207, 2),
+	 (2200, 2), (1607, 1), (1606, 36), (2308, 3),
+	 (3104, 23), (2103, 6), (1311, 1), (1603, 3),
+	 (2503, 1), (2305, 7), (2208, 1), (2100, 16),
+	 (1502, 2), (1710, 6), (2104, 2)]
 
 
 If you request data of a merged author profile, Scopus provides information corresponding to the new, merged profile.  The cache file's name uses the provided, i.e., old, ID.  With property `.identifer` you can verify the validity of the provided Author ID.  When the provided ID belongs to a profile that has been merged, pybliometrics will throw a UserWarning (upon accessing the property `.identifer`) pointing to the ID of the new main profile.
 
 Detailed information on current and former affiliations is also provided in the form of namedtuple:
 
 .. code-block:: python
@@ -111,15 +116,15 @@
     [Affiliation(id=110785688, parent=60027950, type='dept', relationship='author',
      afdispname=None, preferred_name='Department of Chemical Engineering',
      parent_preferred_name='Carnegie Mellon University', country_code='usa',
      country='United States', address_part='5000 Forbes Avenue', city='Pittsburgh',
      state='PA', postal_code='15213-3890', org_domain='cmu.edu', org_URL='https://www.cmu.edu/')]
     >>> len(au.affiliation_history)
     16
-    >>> au.affiliation_history[10]
+    >>> au.affiliation_history[6]
     Affiliation(id=60008644, parent=None, type='parent', relationship='author',
     afdispname=None, preferred_name='Fritz Haber Institute of the Max Planck Society',
     parent_preferred_name=None, country_code='deu', country='Germany',
     address_part='Faradayweg 4-6', city='Berlin', state=None, postal_code='14195',
     org_domain='fhi.mpg.de', org_URL='https://www.fhi.mpg.de/')
 
 
@@ -142,15 +147,15 @@
 
 The `get_documents()` method is another convenient option for searching the author's publications via :doc:`ScopusSearch <../classes/ScopusSearch>` (information will be cached):
 
 .. code-block:: python
 
     >>> docs = pd.DataFrame(au.get_documents(refresh=10))
     >>> docs.shape
-    (108, 34)
+    (126, 36)
     >>> docs.columns
     Index(['eid', 'doi', 'pii', 'pubmed_id', 'title', 'subtype',
            'subtypeDescription', 'creator', 'afid', 'affilname',
            'affiliation_city', 'affiliation_country', 'author_count',
            'author_names', 'author_ids', 'author_afids', 'coverDate',
            'coverDisplayDate', 'publicationName', 'issn', 'source_id', 'eIssn',
            'aggregationType', 'volume', 'issueIdentifier', 'article_number',
@@ -176,31 +181,34 @@
 or you might be interested in the yearly number of publications:
 
 .. code-block:: python
 
     >>> docs['year'] = docs['coverDate'].str[:4]
     >>> docs['year'].value_counts().sort_index()
     1995     1
-    2002     1
-    2003     3
-    2004     4
-    2005     3
-    2006     1
-    2007     2
-    2008     7
-    2009    10
-    2010     6
-    2011    10
-    2012     8
-    2013     4
-    2014    10
-    2015    12
-    2016     7
-    2017     8
-    2018     4
-    2019     2
-    2020     2
-    2021     3
+	2002     1
+	2003     3
+	2004     4
+	2005     3
+	2006     1
+	2007     2
+	2008     7
+	2009    10
+	2010     6
+	2011     8
+	2012     8
+	2013     4
+	2014    10
+	2015    12
+	2016     7
+	2017     8
+	2018     4
+	2019     2
+	2020     2
+	2021     3
+	2022     9
+	2023     8
+	2024     3
     Name: year, dtype: int64
 
 
 If you're just interested in the EIDs of the documents, use `au.get_document_eids()`.  This method makes use of the same data available for/through `au.get_documents()`.
```

### Comparing `pybliometrics-3.6/docs/classes/AuthorSearch.rst` & `pybliometrics-4.0/docs/classes/AuthorSearch.rst`

 * *Files 2% similar despite different names*

```diff
@@ -17,35 +17,37 @@
 Examples
 --------
 
 The class is initialized using a search query, details of which can be found in `Author Search Guide <https://dev.elsevier.com/tips/AuthorSearchTips.htm>`_.  An invalid search query will result in an error.
 
 .. code-block:: python
 
+    >>> import pybliometrics
     >>> from pybliometrics.scopus import AuthorSearch
+	>>> pybliometrics.scopus.init()
     >>> s = AuthorSearch('AUTHLAST(Selten) and AUTHFIRST(Reinhard)')
 
 
 You can obtain a search summary just by printing the object:
 
 .. code-block:: python
 
     >>> print(s)
-    Search 'AUTHLAST(Selten) and AUTHFIRST(Reinhard)' yielded 2 authors as of 2021-11-12:
-        Selten, Reinhard; AUTHOR_ID:6602907525 (74 document(s))
-        Selten, Reinhard; AUTHOR_ID:57213632570 (1 document(s))
+    Search 'AUTHLAST(Selten) and AUTHFIRST(Reinhard)' yielded 2 authors as of 2024-05-11:
+		Selten, Reinhard; AUTHOR_ID:6602907525 (74 document(s))
+		Selten, Reinhard; AUTHOR_ID:57213632570 (1 document(s))
 
 
 To determine the the number of results use the `.get_results_size()` method, even before you download the results:
 
 .. code-block:: python
 
     >>> other = AuthorSearch("AUTHLAST(Selten)", download=False)
     >>> other.get_results_size()
-    29
+    27
 
 
 Primarily, the class provides a list of `namedtuples <https://docs.python.org/3/library/collections.html#collections.namedtuple>`_ storing author EIDs, which you can use for the :doc:`AuthorRetrieval <../classes/AuthorRetrieval>` class, and corresponding information:
 
 .. code-block:: python
 
     >>> s.authors[0]
```

### Comparing `pybliometrics-3.6/docs/classes/CitationOverview.rst` & `pybliometrics-4.0/docs/classes/CitationOverview.rst`

 * *Files 6% similar despite different names*

```diff
@@ -19,80 +19,82 @@
 
 The class can download yearly citation counts for up to 25 documents at once.  Simply provide a list of either the Scopus identifiers, the DOIs, the PIIs or the pubmed IDs and specify the identifier type in `id_type`.  The API needs to know for which years you want to retrieve yearly citation counts.  Therefore you need to set the year from which on `CitationOverview()` will return yearly citation counts (e.g., the publication year).  If no ending year is given, `CitationOverview()` will use the current year.  Optionally you can exclude citations by books or self-citation via `exclude`.
 
 You initialize the class with a list of identifiers:
 
 .. code-block:: python
 
+    >>> import pybliometrics
     >>> from pybliometrics.scopus import CitationOverview
+	>>> pybliometrics.scopus.init()
     >>> identifier = ["85068268027", "84930616647"]
     >>> co = CitationOverview(identifier, start=2019, end=2021)
 
 
 You can obtain basic information just by printing the object:
 
 .. code-block:: python
 
     >>> print(co)
     2 document(s) has/have the following total citation count
-    as of 2021-07-17:
-        16; 13
+    as of 2024-05-11:
+        110; 20
 
 
 The key attribute is `cc`, which provides a list of tuples storing year-wise citations to the article.  Each list corresponds to one document, in the order specified when initating the class:
 
 .. code-block:: python
 
     >>> co.cc
-    [[(2019, 0), (2020, 6), (2021, 10)],
-     [(2019, 2), (2020, 2), (2021, 1)]]
+    [[(2019, 0), (2020, 6), (2021, 25)],
+	 [(2019, 2), (2020, 2), (2021, 2)]]
 
 
 The attributes `pcc`, `rangeCount`, `lcc` and `rowTotal` provide citation summaries for each document.  `pcc` is the count of citations before the specified year, `rangeCount` the count of citations for the specified years, and `lcc` the count of citations after the specified year.  For the sum (i.e., the total number of citations by document) use `rowTotal`
 
 .. code-block:: python
 
     >>> co.pcc
     [0, 8]
     >>> co.rangeCount
-    [16, 5]
+    [31, 6]
     >>> co.lcc
-    [0, 0]
+    [79, 5]
     >>> co.rowTotal
-    [16, 13]
+    [110, 20]
 
 
 The `columnTotal` attribute represents the total number of yearly citations for all documents combined, which `rangeColumnTotal` summarizes.  Finally `grandTotal` is the total number of citations for all documents combined.
 
 .. code-block:: python
 
     >>> co.columnTotal
-    [2, 8, 11]
+    [2, 8, 27]
     >>> co.rangeColumnTotal
-    21
+    37
     >>> co.grandTotal
-    29
+    130
 
 
 With the `citation` parameter, you can exclude self-citations or citations from books:
 
 .. code-block:: python
 
     >>> co_self = CitationOverview(identifier, start=2019, end=2021,
                                    citation="exclude-self")
     >>> print(co_self)
     2 document(s) has/have the following total citation count
-    excluding self-citations as of 2021-07-17:
-        14; 11
+    excluding self-citations as of 2024-05-11:
+        110; 20
     >>> co_books = CitationOverview(identifier, start=2019, end=2021,
                                     citation="exclude-books")
     >>> print(co_books)
     2 document(s) has/have the following total citation count
-    excluding citations from books as of 2021-07-17:
-        16; 13
+    excluding citations from books as of 2024-05-11:
+        10; 20
 
 
 Author information is also stored as lists of `namedtuples <https://docs.python.org/3/library/collections.html#collections.namedtuple>`_:
 
 .. code-block:: python
 
     >>> co.authors[0]
```

### Comparing `pybliometrics-3.6/docs/classes/PlumXMetrics.rst` & `pybliometrics-4.0/docs/classes/PlumXMetrics.rst`

 * *Files 20% similar despite different names*

```diff
@@ -17,60 +17,58 @@
 Examples
 --------
 
 You initialize the class with the identifier of a document and its type:
 
 .. code-block:: python
 
+    >>> import pybliometrics
     >>> from pybliometrics.scopus import PlumXMetrics
+	>>> pybliometrics.scopus.init()
     >>> plum = PlumXMetrics("2-s2.0-85054706190", id_type='elsevierId')
 
 
 You can obtain basic information just by printing the object:
 
 .. code-block:: python
 
     >>> print(plum)
     Document with elsevierId 2-s2.0-85054706190 received:
-    - 460 citation(s) in category 'capture'
-    - 232 citation(s) in category 'citation'
-    - 2 citation(s) in category 'mention'
-    - 42 citation(s) in category 'socialMedia'
-    - 216 citation(s) in category 'usage'
-    as of 2023-10-20
+	- 469 citation(s) in category 'capture'
+	- 248 citation(s) in category 'citation'
+	- 2 citation(s) in category 'mention'
+	- 185,819 citation(s) in category 'socialMedia'
+	as of 2024-05-11
 
 
 For each of the five categories, there is a corresponding property that stores the number and origin of the metrics in `namedtuples <https://docs.python.org/3/library/collections.html#collections.namedtuple>`_.  If a category has no entries, the corresponding property will be `None`:
 
 .. code-block:: python
 
-    >>> >>> plum.capture
-    [Metric(name='READER_COUNT', total=459),
-     Metric(name='EXPORTS_SAVES', total=1)]
+    >>> plum.capture
+    [Metric(name='READER_COUNT', total=469)]
     >>> plum.citation
-    [Metric(name='Scopus', total=231),
-     Metric(name='CrossRef', total=80),
+    [Metric(name='Scopus', total=247),
+	 Metric(name='CrossRef', total=80),
      Metric(name='Policy Citation', total=1)]
     >>> plum.mention
     [Metric(name='NEWS_COUNT', total=2)]
     >>> plum.social_media
-    [Metric(name='FACEBOOK_COUNT', total=42)]
+    [Metric(name='FACEBOOK_COUNT', total=185819)]
     >>> plum.usage
-    [Metric(name='ABSTRACT_VIEWS', total=205),
-     Metric(name='LINK_OUTS', total=11)]
+    
 
 
 Finally, there is a property that totals all metrics at an aggregated level:
 
 .. code-block:: python
 
     >>> plum.category_totals
-    [Category(name='capture', total=460),
-     Category(name='citation', total=232),
-     Category(name='mention', total=2),
-     Category(name='socialMedia', total=42),
-     Category(name='usage', total=216)]
+    [Category(name='capture', total=469),
+	 Category(name='citation', total=248),
+	 Category(name='mention', total=2),
+	 Category(name='socialMedia', total=185819)]
 
 
 There are no bibliometric information such as title or author.
 
 Downloaded results are cached to expedite subsequent analyses.  This information may become outdated.  To refresh the cached results if they exist, set `refresh=True`, or provide an integer that will be interpreted as maximum allowed number of days since the last modification date.  For example, if you want to refresh all cached results older than 100 days, set `refresh=100`.  Use `ab.get_cache_file_mdate()` to obtain the date of last modification, and `ab.get_cache_file_age()` to determine the number of days since the last modification.
```

### Comparing `pybliometrics-3.6/docs/classes/ScopusSearch.rst` & `pybliometrics-4.0/docs/classes/ScopusSearch.rst`

 * *Files 1% similar despite different names*

```diff
@@ -17,27 +17,29 @@
 Examples
 --------
 
 The class is initialized with a search query.  There are but two exceptions to allowed keywords as compared to the Advanced Document Search: "LIMIT-TO()", as this only affects the display of the results on scopus.com, but not the selection of results per se; and "INDEXTERMS()".  An invalid search query will result in some `error <../tips.html#error-messages>`_.  Setting `verbose=True` informs about the download progress.
 
 .. code-block:: python
 
+    >>> import pybliometrics
     >>> from pybliometrics.scopus import ScopusSearch
+	>>> pybliometrics.scopus.init()
     >>> q = "REF(2-s2.0-85068268027)"
     >>> s = ScopusSearch(q, verbose=True)
     Downloading results for query "REF(2-s2.0-85068268027)":
-    100%|████████████████████████████████████████████████████████████████████████████████████████████████| 4/4 [00:03<00:00,  1.07s/it]
+    100%|████████████████████████████████████████████████████████████████████████████████████████████████| 5/5 [00:03<00:00,  1.07s/it]
 
 
 You can obtain a search summary just by printing the object:
 
 .. code-block:: python
 
     >>> print(s)
-    Search 'REF(2-s2.0-85068268027)' yielded 88 documents as of 2023-12-03:
+    Search 'REF(2-s2.0-85068268027)' yielded 10 documents as of 2024-95-11:
         2-s2.0-85174697039
         2-s2.0-85169560066
         2-s2.0-85163820321
         2-s2.0-85153853127
         2-s2.0-85174908092
         2-s2.0-85163278918
         2-s2.0-85169708007
@@ -52,32 +54,32 @@
 Non-subscribers must instantiate the class with `subscriber=False`.  They may only get 5,000 results per query, whereas this limit does not exist for subscribers.
 
 Users can determine the number of results programmatically using the `.get_results_size()` method:
 
 .. code-block:: python
 
     >>> s.get_results_size()
-    88
+    110
 
 
 This method works even if one chooses to not download results.  It thus helps subscribers to decide programmatically if one wants to proceed downloading or not:
 
 .. code-block:: python
 
     >>> other = ScopusSearch('AUTHLASTNAME(Brown)', download=False)
     >>> other.get_results_size()
-    311543
+    316970
 
 
 The main attribute of the class, `results`, returns a list of `namedtuples <https://docs.python.org/3/library/collections.html#collections.namedtuple>`_.  They can be efficiently converted into DataFrames using `pandas <https://pandas.pydata.org/>`_:
 
 .. code-block:: python
 
     >>> import pandas as pd
-    >>> df = pd.DataFrame(pd.DataFrame(s.results))
+    >>> df = pd.DataFrame(s.results)
     >>> df.columns
     Index(['eid', 'doi', 'pii', 'pubmed_id', 'title', 'subtype', 'subtypeDescription',
            'creator', 'afid', 'affilname', 'affiliation_city', 'affiliation_country',
            'author_count', 'author_names', 'author_ids', 'author_afids', 'coverDate',
            'coverDisplayDate', 'publicationName', 'issn', 'source_id', 'eIssn',
            'aggregationType', 'volume', 'issueIdentifier', 'article_number',
            'pageRange', 'description', 'authkeywords', 'citedby_count',
@@ -209,12 +211,12 @@
 `views <https://dev.elsevier.com/guides/ScopusSearchViews.htm>`_.  The view 'COMPLETE' is the highest unrestricted view and contains all information also included in the 'STANDARD' view.  It is therefore the default view.  However, when speed is an issue, choose the STANDARD view.
 
 For convenience, the `s.get_eids()` method returns the list of EIDs:
 
 .. code-block:: python
 
     >>> s.get_eids()
-    ['2-s2.0-85174697039', '2-s2.0-85169560066', '2-s2.0-85163820321',
-    '2-s2.0-85153853127', '2-s2.0-85174908092', '2-s2.0-85163278918',
-    '2-s2.0-85169708007', '2-s2.0-85165723386', '2-s2.0-85162924068',
+    ['2-s2.0-85184035025', '2-s2.0-85187781098', '2-s2.0-85191356593',
+     '2-s2.0-85185298843', '2-s2.0-85176114500', '2-s2.0-85187960595',
+	 '2-s2.0-85187507366', '2-s2.0-85187306554', '2-s2.0-85181899797',
     #...
     '2-s2.0-85087770000', '2-s2.0-85086243347', '2-s2.0-85084027658']
```

### Comparing `pybliometrics-3.6/docs/classes/SerialSearch.rst` & `pybliometrics-4.0/docs/classes/SerialSearch.rst`

 * *Files 9% similar despite different names*

```diff
@@ -17,24 +17,26 @@
 Examples
 --------
 
 The class is initialized with a search query dictionary.  Its keys are limited to the following set: "title", "issn", "pub", "subj", "subjCode", "content", and "oa".  No more than 200 results can be returned.
 
 .. code-block:: python
 
+    >>> import pybliometrics
     >>> from pybliometrics.scopus import SerialSearch
+	>>> pybliometrics.scopus.init()
     >>> s = SerialSearch(query={"title": "SoftwareX"})
 
 
 You can obtain basic information just by printing the object:
 
 .. code-block:: python
 
     >>> print(s)
-    Search '{'title': 'SoftwareX'}' yielded 1 source as of 2021-07-14:
+    Search '{'title': 'SoftwareX'}' yielded 1 source as of 2024-05-11:
         SoftwareX
 
 
 Users can determine the number of results programmatically using the `.get_results_size()` method:
 
 .. code-block:: python
 
@@ -45,38 +47,38 @@
 The main attribute of the class, `results`, returns a list of `OrderedDict <https://docs.python.org/3/library/collections.html#collections.OrderedDict>`_ objects.  Provided information can differ greatly between results and depending on the view (see below) they can be numerous.  Lists of OrderedDict objects can be efficiently converted into DataFrames using `pandas <https://pandas.pydata.org/>`_:
 
 .. code-block:: python
 
     >>> import pandas as pd
     >>> df = pd.DataFrame(pd.DataFrame(s.results))
     >>> df.shape
-    (1, 147)
+    (1, 162)
     >>> df.columns
     Index(['title', 'publisher', 'coverageStartYear', 'coverageEndYear',
            'aggregationType', 'source-id', 'eIssn', 'openaccess',
            'openaccessArticle', 'subject_area_codes',
            ...
            'publicationCount_2019', 'citeCountSCE_2019', 'zeroCitesSCE_2019',
            'zeroCitesPercentSCE_2019', 'revPercent_2019', 'publicationCount_2020',
            'citeCountSCE_2020', 'zeroCitesSCE_2020', 'zeroCitesPercentSCE_2020',
            'revPercent_2020'],
           dtype='object', length=142)
     >>> pd.set_option('display.max_columns', None)
     >>> df.iloc[:,:16]
        title    publisher coverageStartYear coverageEndYear aggregationType  \
-    0  SoftwareX  Elsevier BV              2015            2020         journal   
+    0  SoftwareX  Elsevier BV              2015            2024         journal   
 
          source-id      eIssn openaccess  openaccessArticle subject_area_codes  \
     0  21100422153  2352-7110          1               True          1712;1706   
 
-      subject_area_abbrevs                      subject_area_names SNIP_2018  \
-    0                 COMP  Software;Computer Science Applications     4.905   
+      subject_area_abbrevs                      subject_area_names SNIP_['@year']  \
+    0                 COMP  Software;Computer Science Applications          1.426
 
-      SJR_2018 citeScoreTracker_2019 citeScoreCurrentMetric_2018  
-    0    4.539                  2.18                       11.56 
+      SJR_['@year'] citeScoreTracker_2023 citeScoreCurrentMetric_2022
+    0         0.574                   5.4                         5.1
 
 
 The information in columns beyond the first 16 pertains to journal metrics: publication counts, citation counts, not-cited documents, share of not-cited documents, and the share of review article documents, for each year since indexation.
 
 Downloaded results are cached to expedite subsequent analyses.  This information may become outdated.  To refresh the cached results if they exist, set `refresh=True`, or provide an integer that will be interpreted as maximum allowed number of days since the last modification date.  For example, if you want to refresh all cached results older than 100 days, set `refresh=100`.  Use `ab.get_cache_file_mdate()` to obtain the date of last modification, and `ab.get_cache_file_age()` to determine the number of days since the last modification.
 
 The Serial Title API offers varying depths of information through
```

### Comparing `pybliometrics-3.6/docs/classes/SerialTitle.rst` & `pybliometrics-4.0/docs/classes/SerialTitle.rst`

 * *Files 6% similar despite different names*

```diff
@@ -17,30 +17,31 @@
 Examples
 --------
 
 You initialize the class with an ISSN or an E-ISSN (works with and without hyphen, but leading zeros are mandatory):
 
 .. code-block:: python
 
+    >>> import pybliometrics
     >>> from pybliometrics.scopus import SerialTitle
+	>>> pybliometrics.scopus.init()
     >>> source = SerialTitle("00368075")
 
 You can obtain basic information just by printing the object:
 
 .. code-block:: python
 
     >>> print(source)
-    'Science', journal published by 'American Association for the Advancement
-    of Science', is active in Multidisciplinary
-    Metrics as of 2023-11-15:
-        SJR:  year value
-              2022 13.328
-        SNIP: year value
-              2022 7.729
-        ISSN: 0036-8075, E-ISSN: 1095-9203, Scopus ID: 23571
+    'Science', journal published by 'American Association for the Advancement of Science', is active in Multidisciplinary
+	Metrics as of 2024-05-11:
+		SJR:  year value
+			  2022 13.328
+		SNIP: year value
+			  2022 7.729
+		ISSN: 0036-8075, E-ISSN: 1095-9203, Scopus ID: 23571
 
 The object has a number of attributes but no methods.  For example, information regarding the source itself:
 
 .. code-block:: python
 
     >>> source.title
     'Science'
@@ -56,30 +57,30 @@
 
 Crucially, it provides three metrics: CiteScore (see `here <https://service.elsevier.com/app/answers/detail/a_id/30562/supporthub/scopus/>`_ for further information), SCImago Journal Rank indicator (see `here <https://www.scimagojr.com/journalrank.php>`_), and Source Normalized Impact Factor (SNIP; see `here <https://blog.scopus.com/posts/journal-metrics-in-scopus-source-normalized-impact-per-paper-snip>`_).  This information is presented in lists of two-element tuples, with the first element indicating the year of metric evaluation.
 
 .. code-block:: python
 
     >>> source.citescoreyearinfolist
     [Citescoreinfolist(year=2022, citescore=59.0),
-     Citescoreinfolist(year=2023, citescore=58.8)]
+     Citescoreinfolist(year=2023, citescore=60.9)]
     >>> source.sjrlist
     [(2022, 13.328)]
     >>> source.sniplist
     [(2022, 7.729)]
 
 
 The `citescoreyearinfolist` property provides detailed information for all available years when `view="CITESCORE"` is used.  It includes the status of the metric, the document count and citation count (of the previous 4 years), the share of documents actually cited, and the rank and percentile for each related ASJC subject:
 
 .. code-block:: python
 
     >>> source_full = SerialTitle("00368075", view="CITESCORE")
     >>> info = pd.DataFrame(source_full.citescoreyearinfolist)
     >>> print(info)
         year  citescore       status  documentcount  citationcount  percentcited                             rank
-    0   2023       58.8  In-Progress           4730         278199            79                  [(1000, 2, 99)]
+    0   2023       60.9  In-Progress           4969         302467            79                  [(1000, 2, 99)]
     1   2022       59.0     Complete           4895         288748            82                  [(1000, 2, 98)]
     2   2021       57.8     Complete           4823         278545            84                  [(1000, 2, 98)]
     3   2020       46.8     Complete           4833         226134            82                  [(1000, 2, 98)]
     4   2019       45.3     Complete           4799         217261            81                  [(1000, 2, 98)]
     5   2018       47.1     Complete           4681         220642            82                  [(1000, 2, 98)]
     6   2017       49.4     Complete           4215         208286            90                  [(1000, 2, 98)]
     7   2016       49.5     Complete           4176         206665            89                  [(1000, 1, 99)]
@@ -92,25 +93,25 @@
 
 The `yearly_data` time series includes the number of documents published in a given year.  It contains the number of documents published in this year, the share of review articles thereof, the number and share of not-cited documents, and the number of distinct documents that were cited in this year.
 
 
 .. code-block:: python
 
     >>> source.yearly_data[-1]
-    Yearlydata(year=2023, publicationcount=1800, revpercent=2.94,
-               zerocitessce=1201, zerocitespercentsce=66.72222222222223,
-               citecountsce=726948)
+	Yearlydata(year=2024, publicationcount=473, revpercent=4.02,
+			   zerocitessce=400, zerocitespercentsce=84.56659619450318,
+			   citecountsce=246787)
     >>> yearly_data = pd.DataFrame(source.yearly_data)
     >>> yearly_data.head()
        year  publicationcount  revpercent  zerocitessce  zerocitespercentsce  citecountsce
-    0  1996              2395        4.97           655            27.348643        236545
-    1  1997              2833        6.28           904            31.909636        244078
-    2  1998              2816        4.69           854            30.326705        254500
-    3  1999              2373        6.28           532            22.418879        276054
-    4  2000              2402        6.99           459            19.109076        293867
+	0  1996              2395        4.97           653            27.265136        236672
+	1  1997              2833        6.28           899            31.733145        244122
+	2  1998              2816        4.69           850            30.184659        254600
+	3  1999              2373        6.28           531            22.376738        276110
+	4  2000              2401        7.00           457            19.033736        294076
 
 
 By default, `SerialTitle()` retrieves only the most recent metrics, although yearly data is availble from 1996 onwards.  If you provide a year or a range of years via the optional parameter `years`, `SerialTitle()` will retrieve information for these years (except for the CiteScore):
 
 .. code-block:: python
 
     >>> source_y = SerialTitle("00368075", years="2017-2019")
```

### Comparing `pybliometrics-3.6/docs/classes/SubjectClassifications.rst` & `pybliometrics-4.0/docs/classes/SubjectClassifications.rst`

 * *Files 2% similar despite different names*

```diff
@@ -17,25 +17,27 @@
 Examples
 --------
 
 You initialize the class with a query `dict`.  It contains the "description" (general classification of the subject), "code" (the ASJC code), "detail" (detailed name of the subject), "abbrev" (abbreviation of general classification of subject) or a combination of those:
 
 .. code-block:: python
 
+	>>> import pybliometrics
     >>> from pybliometrics.scopus import SubjectClassifications
+	>>> pybliometrics.scopus.init()
     >>> sub = SubjectClassifications({'description': 'Mathematics'})
 
 
 You can obtain basic information just by printing the object:
 
 .. code-block:: python
 
     >>> print(sub)
     Search '{'description': 'Mathematics', 'field': 'code,description,detail,abbrev'}'
-    yielded 15 subject areas as of 2021-02-11:
+    yielded 15 subject areas as of 2024-05-11:
         2600
         2601
         2602
         2603
         2604
         2605
         2606
```

### Comparing `pybliometrics-3.6/docs/classes.rst` & `pybliometrics-4.0/docs/classes.rst`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.6/docs/conf.py` & `pybliometrics-4.0/docs/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,16 +53,14 @@
 html_sidebars = {
     '**': [
         'about.html',
         'navigation.html',
         'searchbox.html',
     ]
 }
-html_static_path = ['_static']
-html_css_files = ['custom.css']
 
 # Options for HTMLHelp output
 html_show_sourcelink = True
 htmlhelp_basename = 'pybliometricsdoc'
 autoclass_content = 'both'
 
 # Option to group members of classes
```

### Comparing `pybliometrics-3.6/docs/configuration.rst` & `pybliometrics-4.0/docs/configuration.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Configuration
 -------------
 
 pybliometrics.cfg
 ~~~~~~~~~~~~~~~~~
-`pybliometrics` stores values it needs for operation in a configuration file called `pybliometrics.cfg`.  The config file saves credentials as well as directory names for folders that store downloaded results.
+`pybliometrics` stores values it needs for operation in a configuration file called `pybliometrics.cfg`.  The config file saves credentials as well as directory names for folders that store downloaded results. `pybliometrics` reads this file on startup.
 
 By default, after initial set-up (see below), the file will look like this:
 
 .. code-block:: none
 
     [Directories]
     AbstractRetrieval = PPP/.pybliometrics/Scopus/abstract_retrieval
@@ -34,76 +34,62 @@
 Section `[Authentication]` contains the API Keys which you obtain from http://dev.elsevier.com/myapikey.html.  If you provide multiple (separated by a comma), `pybliometrics` automatically replaces a depleted key with another one at random at runtime until all of them are depleted.
 
 Simply edit this file using a simple text editor; changes will take effect the next time you start pybliometrics.  Remember to indent multi-line statements.
 
 Under `pybliometrics` 2.x and before, the default paths used to be `PPP/.scopus/abstract_retrieval`.  You can safely rename the cache folder `.scopus` to `.pybliometrics` (on Windows machines, rename to `.pybliometrics.`), but remember to change the paths in the configuration file, too.
 
 
+Start-up
+~~~~~~~~
+
+You initalize `pybliometrics` like so:
+
+.. code-block:: python
+
+    import pybliometrics
+	
+	pybliometrics.scopus.init()
+
+
+This reads the configuration from the default locations.  If you store the configuration file elsewhere, you can provide the path using keyword "config_dir" (str).  You may also pass your own keys using the keyword "keys" (list).
+
+
 Set-up
 ~~~~~~
-If the configuration file does not exist, `pybliometrics` will prompt you to provide the configuration values on first import.
+If the configuration file does not exist, `pybliometrics` will prompt you to provide the configuration values the first time you execute `init()`.
 
 There are two consecutive prompts: For your API Key(s) and your InstToken.  The InstToken enables or facilitates access from outside your institution network, and you request it from Elsevier's Integration Support.  If you don't use InstToken, hit enter on the second prompt.  The InstToken, if provided, is added to the Authentication block:
 
 .. code-block:: none
 
     [Authentication]
-    APIKey = XXX, YYY, ZZZ
+    APIKey = XXX
     InstToken = WWW
 
 
 If you need to use a proxy, please edit the file manually to include a section that looks like so:
 
 .. code-block:: none
 
     [Proxy]
     http = http://127.0.0.1:1234
     https = https://127.0.0.1:1234
 
 
 The presence of this information will make use of the proxy.  Be sure to remove or comment out the block when you don't want to use a proxy.
 
-In case you build `pybliometrics` using CI or on a server where prompts aren't possible, you can provide a single optional parameter to `create_config()`.  The parameter must be a list of keys.  When this parameter is used, there will be no prompts.  Note that this only works to overwrite the existing configuration file.
-
-
-Runtime
-~~~~~~~
-
-You can easily inspect configuration values at runtime, and even set some during execution.  Simply import the config beforehand and assign new values to the keys as if the config was a dictionary:
-
-.. code-block:: python
-
-    from pybliometrics.scopus.utils import config
-
-    print(config['Authentication']['APIKey'])  # Show keys
-    config['Proxy']['https'] = 'https://127.0.0.1:1234'  # Redefine proxy
-
-Setting the keys at runtime is however not possible.
+In case you build `pybliometrics` using CI or on a server where prompts aren't possible, you can provide a optional parameters to `create_config()`: "config_dir" (str) for the location of the file, "keys" (list) for the API keys, and "insttoken" (list) for the InstTokens.  Note that this only works to overwrite the existing configuration file.
 
 
 Default location
 ~~~~~~~~~~~~~~~~
-For recent and new installations, the configuration file is located at `~/.config/`.  Folder `~/` refers to your private home directory or home path.  On many Windows machines this defaults to `C:/Document and Settings/<Your User Name>`.
+By default, the configuration file is located at `~/.config/`.  Folder `~/` refers to your private home directory or home path.  On many Windows machines this defaults to `C:/Document and Settings/<Your User Name>`.
 
 If you started with versions older than 3.5, the file was called `config.ini` and located either in `~/.pybliometrics/` or (for very old installations) in `~/.scopus/`. You can safely move and rename the file.  The location `~/.config/pybliometrics.cfg` always takes precedence.
 
 To see the location of the configuration file your current `pybliometrics` instance is using, execute this:
 
 .. code-block:: python
 
     import pybliometrics
 
     pybliometrics.scopus.utils.constants.CONFIG_FILE
-
-
-Custom location
-~~~~~~~~~~~~~~~
-
-If you prefer to have the configuration file somewhere else, you can tell `pybliometrics` where to look for it.  You will need the `environment facility <https://docs.python.org/3/library/os.html#file-names-command-line-arguments-and-environment-variables>`_ of the base package `os`.  For this to take effect you need to set the environ *before* importing pybliometrics.  `pybliometrics` uses the "PYB_CONFIG_FILE" keyword:
-
-.. code-block:: python
-
-    import os
-
-    os.environ['PYB_CONFIG_FILE'] = "C:/Custom/Location/pybliometrics.cfg"
-
-    import pybliometrics
```

### Comparing `pybliometrics-3.6/docs/index.rst` & `pybliometrics-4.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.6/docs/installation.rst` & `pybliometrics-4.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.6/docs/make.bat` & `pybliometrics-4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.6/docs/tips/affiliations.rst` & `pybliometrics-4.0/docs/tips/affiliations.rst`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.6/docs/tips/database.rst` & `pybliometrics-4.0/docs/tips/database.rst`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.6/docs/tips/migration1.rst` & `pybliometrics-4.0/docs/tips/migration1.rst`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.6/docs/tips/support.rst` & `pybliometrics-4.0/docs/tips/support.rst`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.6/meta/1-s2.0-S2352711019300573-main.pdf` & `pybliometrics-4.0/meta/1-s2.0-S2352711019300573-main.pdf`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.6/meta/CHANGES.rst` & `pybliometrics-4.0/meta/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,26 @@
 Change Log
 ----------
 
 .. toctree::
 
+4.0
+~~~
+
+2024-25-05
+
+* Introduce mandatory `pybliometrics.scopus.init()` function for start-up.
+* Introduce new view ENTITLED for `AbstractRetrieval()`, `AffiliationRetrieval()`, `AuthorRetrieval()` and `ScopusSearch()`.
+* In `AffiliationRetrieval.name_variants`, return `None` instead of an empty list.
+* In `AffiliationSearch.affiliations`, field `parent` is empty when the returned value is `'0'`.
+* In `AuthorRetrieval.name_variants`, field `doc_count` is always integer.
+* Fix bug in `AbstractRetrieval().__str__` resulting from missing citations.
+* Fix bug in `AbstractRetrieval().references` resulting from malformatted reference information.
+* Fix bug in `CitationOverview().cc` resulting from missing citations.
+
 3.6
 ~~~
 
 2023-12-08
 
 * In `AbstractRetrieval(view="FULL").references`, return all references, not just the first 40.
 * In `AbstractRetrieval().issn`, always return a namedtuple indicating the type of the returned ISSN.
```

### Comparing `pybliometrics-3.6/pybliometrics/scopus/__init__.py` & `pybliometrics-4.0/pybliometrics/scopus/__init__.py`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.6/pybliometrics/scopus/abstract_citation.py` & `pybliometrics-4.0/pybliometrics/scopus/abstract_citation.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         years, where each sub-list corresponds to one document.
         """
         _years = range(self._start, self._end+1)
         outer = []
         for doc in self._citeInfoMatrix:
             try:
                 cites = [int(d['$']) for d in doc['cc']]
-            except (AttributeError, TypeError):  # No citations
+            except (AttributeError, KeyError, TypeError):  # No citations
                 cites = [0]*len(_years)
             outer.append(list(zip(_years, cites)))
         return _maybe_return_list(outer)
 
     @property
     def citationType_long(self) -> Optional[List[str]]:
         """Type (long version) of the documents (e.g. article, review)."""
```

### Comparing `pybliometrics-3.6/pybliometrics/scopus/abstract_retrieval.py` & `pybliometrics-4.0/pybliometrics/scopus/abstract_retrieval.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from collections import defaultdict, namedtuple
 from typing import List, NamedTuple, Optional, Tuple, Union
 
 from pybliometrics.scopus.superclasses import Retrieval
 from pybliometrics.scopus.utils import chained_get, check_parameter_value,\
     deduplicate, get_id, detect_id_type, get_link, listify,\
-    make_int_if_possible, parse_date_created
+    make_int_if_possible, parse_date_created, VIEWS
 
 
 class AbstractRetrieval(Retrieval):
     @property
     def abstract(self) -> Optional[str]:
         """The abstract of a document.
         Note: If this is empty, try `description` property instead.
@@ -284,14 +284,23 @@
     def description(self) -> Optional[str]:
         """Return the description of a record.
         Note: If this is empty, try `abstract` property instead.
         """
         return chained_get(self._json, ['coredata', 'dc:description'])
 
     @property
+    def document_entitlement_status(self) -> Optional[str]:
+        """Returns the document entitlement status, i.e. tells if the requestor 
+        is entitled to the requested resource.
+        Note: Only works with `ENTITLED` view.
+        """
+        return chained_get(self._json, ['document-entitlement', 'status'])
+        
+
+    @property
     def doi(self) -> Optional[str]:
         """DOI of the document."""
         return chained_get(self._json, ['coredata', 'prism:doi'])
 
     @property
     def eid(self) -> str:
         """EID of the document."""
@@ -524,15 +533,18 @@
         out = []
         fields = 'position id doi title authors authors_auid '\
                  'authors_affiliationid sourcetitle publicationyear coverDate '\
                  'volume issue first last citedbycount type text fulltext'
         ref = namedtuple('Reference', fields)
         items = listify(self._ref.get("reference", []))
         for item in items:
-            info = item.get('ref-info', item)
+            try:
+                info = item.get('ref-info', item)
+            except AttributeError:  # item not a dictionary
+                continue
             volisspag = info.get('volisspag', {}) or {}
             if isinstance(volisspag, list):
                 volisspag = volisspag[0]
             volis = volisspag.get("voliss", {})
             if isinstance(volis, list):
                 volis = volis[0]
             # Parse author information
@@ -693,18 +705,19 @@
         :param refresh: Whether to refresh the cached file if it exists or not.
                         If int is passed, cached file will be refreshed if the
                         number of days since last modification exceeds that value.
         :param id_type: The type of used ID. Allowed values: None, 'eid', 'pii',
                         'scopus_id', 'pubmed_id', 'doi'.  If the value is None,
                         the function tries to infer the ID type itself.
         :param view: The view of the file that should be downloaded.  Allowed
-                     values: META, META_ABS, REF, FULL, where FULL includes all
+                     values: META, META_ABS, REF, FULL, ENTITLED, where FULL includes all
                      information of META_ABS view and META_ABS includes all
                      information of the META view.  For details see
                      https://dev.elsevier.com/sc_abstract_retrieval_views.html.
+                     Note: `ENTITLED` view only contains the `document_entitlement_status`.
         :param kwds: Keywords passed on as query parameters.  Must contain
                      fields and values listed in the API specification at
                      https://dev.elsevier.com/documentation/AbstractRetrievalAPI.wadl.
 
         Raises
         ------
         ValueError
@@ -715,27 +728,28 @@
         -----
         The directory for cached results is `{path}/{view}/{identifier}`,
         where `path` is specified in your configuration file.  In case
         `identifier` is a DOI, an underscore replaces the forward slash.
         """
         # Checks
         identifier = str(identifier)
-        check_parameter_value(view, ('META', 'META_ABS', 'REF', 'FULL'), "view")
+        check_parameter_value(view, VIEWS['AbstractRetrieval'], "view")
         if id_type is None:
             id_type = detect_id_type(identifier)
         else:
             allowed_id_types = ('eid', 'pii', 'scopus_id', 'pubmed_id', 'doi')
             check_parameter_value(id_type, allowed_id_types, "id_type")
 
         # Load json
         self._view = view
         self._refresh = refresh
         Retrieval.__init__(self, identifier=identifier, id_type=id_type,
                            api='AbstractRetrieval', **kwds)
-        self._json = self._json['abstracts-retrieval-response']
+        if self._view in ('META', 'META_ABS', 'REF', 'FULL'):
+            self._json = self._json['abstracts-retrieval-response']
         self._head = chained_get(self._json, ["item", "bibrecord", "head"], {})
         conf_path = ['source', 'additional-srcinfo', 'conferenceinfo', 'confevent']
         self._confevent = chained_get(self._head, conf_path, {})
         if self._view == "REF":
             ref_path = ["references"]
         else:
             ref_path = ['item', 'bibrecord', 'tail', 'bibliography']
@@ -781,24 +795,28 @@
                 s += f' https://doi.org/{self.doi}.\n'
             s += f'{self.citedby_count} citation(s) as of {date}'
             if self.affiliation:
                 s += "\n  Affiliation(s):\n   "
                 s += '\n   '.join([aff.name for aff in self.affiliation])
         
         elif self._view in ('REF'):
-            # Sort reference list by citationcount
-            top_n = 5
-            references = sorted(self.references, key=convert_citedbycount, reverse=True)
-
-            top_references = [f'{reference.title} ({get_date(reference.coverDate)}). '+
-                              f'EID: {reference.id}' for reference in references[:top_n]]
-
-            s = f'A total of {self.refcount} references were found. '
-            s += f'Top {top_n} references:\n\t'
-            s += '\n\t'.join(top_references)
+            try:
+                # Sort reference list by citationcount
+                top_n = 5
+                references = sorted(self.references, key=convert_citedbycount, reverse=True)
+
+                top_references = [f'{reference.title} ({get_date(reference.coverDate)}). '+
+                                f'EID: {reference.id}' for reference in references[:top_n]]
+            except TypeError:
+                top_n = 0
+
+            s = f'A total of {self.refcount or 0} references were found. '
+            if top_n:
+                s += f'Top {top_n} references:\n\t'
+                s += '\n\t'.join(top_references)
 
         return s
 
     def get_bibtex(self) -> str:
         """Bibliographic entry in BibTeX format.
 
         Raises
```

### Comparing `pybliometrics-3.6/pybliometrics/scopus/affiliation_retrieval.py` & `pybliometrics-4.0/pybliometrics/scopus/affiliation_retrieval.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from collections import namedtuple
 from typing import List, NamedTuple, Optional, Tuple, Union
 
 from pybliometrics.scopus.superclasses import Retrieval
 from pybliometrics.scopus.utils import chained_get, check_parameter_value,\
-    get_id, get_link, parse_date_created
+    get_id, get_link, parse_date_created, make_int_if_possible, VIEWS
 
 
 class AffiliationRetrieval(Retrieval):
     @property
     def address(self) -> Optional[str]:
         """The address of the affiliation."""
         return self._json.get('address')
@@ -16,15 +16,15 @@
     def affiliation_name(self) -> str:
         """The name of the affiliation."""
         return self._json.get('affiliation-name')
 
     @property
     def author_count(self) -> int:
         """Number of authors associated with the affiliation."""
-        return int(self._json['coredata']['author-count'])
+        return make_int_if_possible(chained_get(self._json, ['coredata', 'author-count']))
 
     @property
     def city(self) -> Optional[str]:
         """The city of the affiliation."""
         return self._json.get('city')
 
     @property
@@ -39,35 +39,44 @@
             return parse_date_created(self._profile)
         except KeyError:
             return None
 
     @property
     def document_count(self) -> int:
         """Number of documents for the affiliation."""
-        return int(self._json['coredata']['document-count'])
+        return make_int_if_possible(chained_get(self._json, ['coredata', 'document-count']))
+    
+    @property
+    def document_entitlement_status(self) -> Optional[str]:
+        """Returns the document entitlement status, i.e. tells if the requestor 
+        is entitled to the requested resource.
+        Note: Only works with `ENTITLED` view.
+        """
+        return chained_get(self._json, ['document-entitlement', 'status'])
 
     @property
     def eid(self) -> str:
         """The EID of the affiliation."""
-        return self._json['coredata']['eid']
+        return chained_get(self._json, ['coredata', 'eid'])
 
     @property
     def identifier(self) -> int:
         """The Scopus ID of the affiliation."""
         return get_id(self._json)
 
     @property
-    def name_variants(self) -> List[NamedTuple]:
+    def name_variants(self) -> Optional[List[NamedTuple]]:
         """A list of namedtuples representing variants of the `affiliation_name`
         with number of documents referring to this variant.
         """
         variant = namedtuple('Variant', 'name doc_count')
         path = ['name-variants', 'name-variant']
-        return [variant(name=var['$'], doc_count=int(var['@doc-count']))
-                for var in chained_get(self._json, path, [])]
+        variants = [variant(name=var['$'], doc_count=int(var['@doc-count']))
+                    for var in chained_get(self._json, path, [])]
+        return variants or None
 
     @property
     def org_domain(self) -> Optional[str]:
         """Internet domain of the affiliation.  Requires the STANDARD view."""
         return self._profile.get('org-domain')
 
     @property
@@ -119,34 +128,34 @@
         STANDARD view.
         """
         return self._profile.get('sort-name')
 
     @property
     def url(self) -> str:
         """URL to the affiliation's API page."""
-        return self._json['coredata'].get('prism:url')
+        return chained_get(self._json, ['coredata', 'prism:url'])
 
     def __init__(self,
                  aff_id: Union[int, str],
                  refresh: Union[bool, int] = False,
                  view: str = "STANDARD",
                  **kwds: str
                  ) -> None:
         """Interaction with the Affiliation Retrieval API.
 
         :param aff_id: Scopus ID or EID of the affiliation profile.
         :param refresh: Whether to refresh the cached file if it exists or not.
                         If int is passed, cached file will be refreshed if the
                         number of days since last modification exceeds that value.
         :param view: The view of the file that should be downloaded.  Allowed
-                     values: `LIGHT`, `STANDARD`, where `STANDARD` includes all
+                     values: `LIGHT`, `STANDARD`, `ENTITLED`, where `STANDARD` includes all
                      information of the `LIGHT` view.  For details see
                      https://dev.elsevier.com/sc_affil_retrieval_views.html.
                      Note: Neither the `BASIC` view nor `DOCUMENTS` or `AUTHORS`
-                     views are active, although documented.
+                     views are active, although documented. `ENTITLED` only contains the `document_entitlement_status`.
         :param kwds: Keywords passed on as query parameters.  Must contain
                      fields and values mentioned in the API specification at
                      https://dev.elsevier.com/documentation/AffiliationRetrievalAPI.wadl.
 
         Raises
         ------
         ValueError
@@ -155,22 +164,23 @@
 
         Notes
         -----
         The directory for cached results is `{path}/{view}/{aff_id}`,
         where `path` is specified in your configuration file.
         """
         # Checks
-        check_parameter_value(view, ('LIGHT', 'STANDARD'), "view")
+        check_parameter_value(view, VIEWS['AffiliationRetrieval'], "view")
 
         # Load json
         self._view = view
         self._refresh = refresh
         aff_id = str(int(str(aff_id).split('-')[-1]))
         Retrieval.__init__(self, aff_id, api='AffiliationRetrieval', **kwds)
-        self._json = self._json['affiliation-retrieval-response']
+        if self._view in ('LIGHT', 'STANDARD'):
+            self._json = self._json['affiliation-retrieval-response']
         self._profile = self._json.get("institution-profile", {})
 
     def __str__(self):
         """Return a summary string."""
         date = self.get_cache_file_mdate().split()[0]
         s = f"{self.affiliation_name} in {self.city} in {self.country},\nhas "\
             f"{int(self.author_count):,} associated author(s) and "\
```

### Comparing `pybliometrics-3.6/pybliometrics/scopus/affiliation_search.py` & `pybliometrics-4.0/pybliometrics/scopus/affiliation_search.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from collections import namedtuple
 from typing import List, NamedTuple, Optional, Tuple, Union
 
 from pybliometrics.scopus.superclasses import Search
 from pybliometrics.scopus.utils import check_integrity, check_parameter_value,\
-    check_field_consistency, make_search_summary
+    check_field_consistency, make_int_if_possible, make_search_summary
 
 
 class AffiliationSearch(Search):
     @property
     def affiliations(self) -> Optional[List[NamedTuple]]:
         """A list of namedtuples storing affiliation information,
         where each namedtuple corresponds to one affiliation.
         The information in each namedtuple is `(eid name variant documents city
         country parent)`.
 
-        All entries are `strings` or `None`.  Field `variant` combines variants
+        All entries are `strings`, `int` or `None`.  Field `variant` combines variants
         of names with a `";"`.
 
         Raises
         ------
         `ValueError`
             If the elements provided in `integrity_fields` do not match the
             actual field names (listed above).
@@ -29,18 +29,19 @@
         check_field_consistency(self._integrity, fields)
         # Parse elements one-by-one
         out = []
         for item in self._json:
             name = item.get('affiliation-name')
             variants = [d.get('$', "") for d in item.get('name-variant', [])
                         if d.get('$', "") != name]
+            parent = make_int_if_possible(item.get('parent-affiliation-id')) or None
             new = aff(eid=item.get('eid'), variant=";".join(variants),
                       documents=int(item['document-count']), name=name,
                       city=item.get('city'), country=item.get('country'),
-                      parent=item.get('parent-affiliation-id'))
+                      parent=parent)
             out.append(new)
         # Finalize
         check_integrity(out, self._integrity, self._action)
         return out or None
 
     def __init__(self,
                  query: str,
```

### Comparing `pybliometrics-3.6/pybliometrics/scopus/author_retrieval.py` & `pybliometrics-4.0/pybliometrics/scopus/author_retrieval.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from json import loads
 
 from .author_search import AuthorSearch
 from .scopus_search import ScopusSearch
 from pybliometrics.scopus.superclasses import Retrieval
 from pybliometrics.scopus.utils import chained_get, check_parameter_value,\
     filter_digits, get_content, get_link, html_unescape, listify, make_int_if_possible,\
-    parse_affiliation, parse_date_created
+    parse_affiliation, parse_date_created, VIEWS
 
 
 class AuthorRetrieval(Retrieval):
     @property
     def affiliation_current(self) -> Optional[List[NamedTuple]]:
         """A list of namedtuples representing the authors's current
         affiliation(s), in the form `(id parent type relationship afdispname
@@ -53,20 +53,20 @@
         has been merged.
         """
         return self._alias
 
     @property
     def citation_count(self) -> int:
         """Total number of citing items."""
-        return int(self._json['coredata']['citation-count'])
+        return make_int_if_possible(chained_get(self._json, ['coredata', 'citation-count']))
 
     @property
     def cited_by_count(self) -> int:
         """Total number of citing authors."""
-        return int(self._json['coredata']['cited-by-count'])
+        return make_int_if_possible(chained_get(self._json, ['coredata', 'cited-by-count']))
 
     @property
     def classificationgroup(self) -> Optional[List[Tuple[int, int]]]:
         """List with tuples with form`(subject group ID, number of documents)`."""
         path = ['classificationgroup', 'classifications', 'classification']
         out = [(int(filter_digits(item['$'])), int(filter_digits(item['@frequency'])))
                for item in listify(chained_get(self._profile, path, []))]
@@ -89,23 +89,31 @@
             return parse_date_created(self._profile)
         except KeyError:
             return None
 
     @property
     def document_count(self) -> int:
         """Number of documents authored (excludes book chapters and notes)."""
-        return int(self._json['coredata']['document-count'])
+        return make_int_if_possible(chained_get(self._json, ['coredata', 'document-count']))
+    
+    @property
+    def document_entitlement_status(self) -> Optional[str]:
+        """Returns the document entitlement status, i.e. tells if the requestor 
+        is entitled to the requested resource.
+        Note: Only works with `ENTITLED` view.
+        """
+        return chained_get(self._json, ['document-entitlement', 'status'])
 
     @property
     def eid(self) -> Optional[str]:
         """The EID of the author.  If it differs from the one provided,
         pybliometrics will throw a warning informing the user about
         author profile merges.
         """
-        return self._json['coredata'].get('eid')
+        return chained_get(self._json, ['coredata', 'eid'])
 
     @property
     def given_name(self) -> Optional[str]:
         """Author's preferred given name."""
         return html_unescape(chained_get(self._profile, ['preferred-name', 'given-name']))
 
     @property
@@ -118,15 +126,18 @@
         """Scopus IDs of previous profiles now compromising this profile."""
         hist = chained_get(self._json, ["coredata", 'historical-identifier'], [])
         return [int(d['$'].split(":")[-1]) for d in hist] or None
 
     @property
     def identifier(self) -> int:
         """The author's ID.  Might differ from the one provided."""
-        ident = self._json['coredata']['dc:identifier'].split(":")[-1]
+        ident = chained_get(self._json, ['coredata', 'dc:identifier'])
+        if not ident:
+            return ident
+        ident = ident.split(":")[-1]
         if ident != self._id:
             text = f"Profile with ID {self._id} has been merged and the new "\
                    f"ID is {ident}.  Please update your records manually.  "\
                    "Files have been cached with the old ID."
             warn(text, UserWarning)
         return int(ident)
 
@@ -158,23 +169,24 @@
     def name_variants(self) -> Optional[List[NamedTuple]]:
         """List of named tuples containing variants of the author name with
         number of documents published with that variant.
         """
         fields = 'indexed_name initials surname given_name doc_count'
         variant = namedtuple('Variant', fields)
         out = [variant(indexed_name=html_unescape(var['indexed-name']), surname=html_unescape(var['surname']),
-                       doc_count=var.get('@doc-count'), initials=html_unescape(var['initials']),
+                       doc_count=make_int_if_possible(var.get('@doc-count')),
+                       initials=html_unescape(var['initials']),
                        given_name=html_unescape(var.get('given-name')))
                for var in listify(self._profile.get('name-variant', []))]
         return out or None
 
     @property
     def orcid(self) -> Optional[str]:
         """The author's ORCID."""
-        return self._json['coredata'].get('orcid')
+        return chained_get(self._json, ['coredata', 'orcid'])
 
     @property
     def publication_range(self) -> Optional[Tuple[int, int]]:
         """Tuple containing years of first and last publication."""        
         if self._view in ('STANDARD', 'ENHANCED', 'LIGHT'):
             if self._view in ('STANDARD', 'ENHANCED'):
                 r = self._profile.get('publication-range')
@@ -228,35 +240,35 @@
     def surname(self) -> Optional[str]:
         """Author's preferred surname."""
         return html_unescape(chained_get(self._profile, ['preferred-name', 'surname']))
 
     @property
     def url(self) -> Optional[str]:
         """URL to the author's API page."""
-        return self._json['coredata']['prism:url']
+        return chained_get(self._json, ['coredata', 'prism:url'])
 
     def __init__(self,
                  author_id: Union[int, str],
                  refresh: Union[bool, int] = False,
                  view: str = "ENHANCED",
                  **kwds: str
                  ) -> None:
         """Interaction with the Author Retrieval API.
 
         :param author_id: The ID or the EID of the author.
         :param refresh: Whether to refresh the cached file if it exists or not.
                         If int is passed, cached file will be refreshed if the
                         number of days since last modification exceeds that value.
         :param view: The view of the file that should be downloaded.  Allowed
-                     values: `METRICS`, `LIGHT`, `STANDARD`, `ENHANCED`, where `STANDARD`
+                     values: `METRICS`, `LIGHT`, `STANDARD`, `ENHANCED`, `ENTITLED`, where `STANDARD`
                      includes all information of `LIGHT` view and `ENHANCED`
                      includes all information of any view.  For details see
                      https://dev.elsevier.com/sc_author_retrieval_views.html.
                      Note: Neither the `BASIC` nor the `DOCUMENTS` view are active,
-                     although documented.
+                     although documented. `ENTITLED` only contains the `document_entitlement_status`.
         :param kwds: Keywords passed on as query parameters.  Must contain
                      fields and values mentioned in the API specification at
                      https://dev.elsevier.com/documentation/AuthorRetrievalAPI.wadl.
 
         Raises
         ------
         ValueError
@@ -266,38 +278,40 @@
         Notes
         -----
         The directory for cached results is `{path}/ENHANCED/{author_id}`,
         where `path` is specified in your configuration file, and `author_id`
         is stripped of an eventually leading `'9-s2.0-'`.
         """
         # Checks
-        allowed_views = ('METRICS', 'LIGHT', 'STANDARD', 'ENHANCED')
-        check_parameter_value(view, allowed_views, "view")
+        check_parameter_value(view, VIEWS['AuthorRetrieval'], "view")
 
         # Load json
         self._id = str(author_id).split('-')[-1]
         self._view = view
         self._refresh = refresh
         Retrieval.__init__(self, identifier=self._id,
                            api='AuthorRetrieval', **kwds)
 
-        # Parse json
-        self._json = self._json['author-retrieval-response']
-        try:
-            self._json = self._json[0]
-        except KeyError:  # Incomplete forward
-            alias_json = listify(self._json['alias']['prism:url'])
-            self._alias = [d['$'].split(':')[-1] for d in alias_json]
-            alias_str = ', '.join(self._alias)
-            text = f'Author profile with ID {author_id} has been merged and '\
-                   f'the main profile is now one of {alias_str}.  Please update '\
-                   'your records manually.  Functionality of this object is '\
-                   'reduced.'
-            warn(text, UserWarning)
-        else:
+        if self._view in ('METRICS', 'LIGHT', 'STANDARD', 'ENHANCED'):
+            # Parse json
+            self._json = self._json['author-retrieval-response']
+            try:
+                self._json = self._json[0]
+            except KeyError:  # Incomplete forward
+                alias_json = listify(self._json['alias']['prism:url'])
+                self._alias = [d['$'].split(':')[-1] for d in alias_json]
+                alias_str = ', '.join(self._alias)
+                text = f'Author profile with ID {author_id} has been merged and '\
+                    f'the main profile is now one of {alias_str}.  Please update '\
+                    'your records manually.  Functionality of this object is '\
+                    'reduced.'
+                warn(text, UserWarning)
+            else:
+                self._alias = None
+        elif self._view == 'ENTITLED':
             self._alias = None
         self._profile = self._json.get("author-profile", {})
 
     def __str__(self):
         """Return a summary string."""
         if self._view in ('STANDARD', 'ENHANCED', 'LIGHT'):
             date = self.get_cache_file_mdate().split()[0]
```

### Comparing `pybliometrics-3.6/pybliometrics/scopus/author_search.py` & `pybliometrics-4.0/pybliometrics/scopus/author_search.py`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.6/pybliometrics/scopus/exception.py` & `pybliometrics-4.0/pybliometrics/scopus/exception.py`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.6/pybliometrics/scopus/plumx_metrics.py` & `pybliometrics-4.0/pybliometrics/scopus/plumx_metrics.py`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.6/pybliometrics/scopus/scopus_search.py` & `pybliometrics-4.0/pybliometrics/scopus/scopus_search.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from collections import namedtuple
 from typing import List, NamedTuple, Optional, Tuple, Union
 
 from pybliometrics.scopus.superclasses import Search
 from pybliometrics.scopus.utils import check_integrity, chained_get,\
     check_parameter_value, check_field_consistency, deduplicate,\
-    get_freetoread, listify, make_search_summary
+    get_freetoread, listify, make_search_summary, VIEWS
 
 
 class ScopusSearch(Search):
     @property
     def results(self) -> Optional[List[NamedTuple]]:
         """A list of namedtuples in the form `(eid doi pii pubmed_id title
         subtype subtypeDescription creator afid affilname affiliation_city
@@ -173,15 +173,15 @@
         -----
         The directory for cached results is `{path}/{view}/{fname}`,
         where `path` is specified in your configuration file and `fname` is
         the md5-hashed version of `query`.
         """
         # Checks
         if view:
-            check_parameter_value(view, ('STANDARD', 'COMPLETE'), "view")
+            check_parameter_value(view, VIEWS['ScopusSearch'], "view")
         allowed = ("warn", "raise")
         check_parameter_value(integrity_action, allowed, "integrity_action")
 
         # Parameters
         if not view:
             if subscriber:
                 view = "COMPLETE"
```

### Comparing `pybliometrics-3.6/pybliometrics/scopus/serial_search.py` & `pybliometrics-4.0/pybliometrics/scopus/serial_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from collections import OrderedDict
 from typing import Dict, List, Optional, Union
 
 from pybliometrics.scopus.superclasses import Search
-from pybliometrics.scopus.utils import check_parameter_value, make_search_summary
+from pybliometrics.scopus.utils import check_parameter_value, make_search_summary, VIEWS
 
 
 class SerialSearch(Search):
     @property
     def results(self) -> Optional[List[Dict[str, str]]]:
         """A list of OrderedDicts representing results of serial search. The
         number of keys may vary from one search result to another depending
@@ -88,15 +88,15 @@
         """
         # Checks
         allowed_query_keys = ('title', 'issn', 'date', 'pub', 'subj',
                               'subjCode', 'content', 'oa')
         invalid = [k for k in query.keys() if k not in allowed_query_keys]
         if invalid:
             raise ValueError(f'Query key(s) "{", ".join(invalid)}" invalid')
-        check_parameter_value(view, ('STANDARD', 'ENHANCED', 'CITESCORE'), "view")
+        check_parameter_value(view, VIEWS['SerialSearch'], "view")
 
         # Query
         self._query = str(query)
         self._refresh = refresh
         self._view = view
         Search.__init__(self, query=query, api='SerialSearch', **kwds)
         self._n = len(self._json['serial-metadata-response'].get('entry', []))
```

### Comparing `pybliometrics-3.6/pybliometrics/scopus/serial_title.py` & `pybliometrics-4.0/pybliometrics/scopus/serial_title.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from collections import namedtuple
 from typing import List, NamedTuple, Optional, Tuple, Union
 
 from pybliometrics.scopus.superclasses import Retrieval
 from pybliometrics.scopus.utils import chained_get, check_parameter_value,\
-    get_link, make_float_if_possible, make_int_if_possible
+    get_link, make_float_if_possible, make_int_if_possible, VIEWS
 
 
 class SerialTitle(Retrieval):
     @property
     def aggregation_type(self) -> str:
         """The type of the source."""
         return self._entry['prism:aggregationType']
@@ -223,16 +223,15 @@
 
         Notes
         -----
         The directory for cached results is `{path}/{view}/{source_id}`,
         where `path` is specified in your configuration file.
         """
         # Checks
-        views = ('STANDARD', 'ENHANCED', 'CITESCORE')
-        check_parameter_value(view, views, "view")
+        check_parameter_value(view, VIEWS['SerialTitle'], "view")
         self._view = view
 
         # Force refresh when years is specified
         if years:
             refresh = True
         self._refresh = refresh
```

### Comparing `pybliometrics-3.6/pybliometrics/scopus/subject_classifications.py` & `pybliometrics-4.0/pybliometrics/scopus/subject_classifications.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,15 +84,15 @@
                 raise ValueError("Parameter 'fields' must be one of " +
                                  f"{', '.join(allowed_query_keys)}.")
 
         # Query
         query['field'] = ','.join(self.fields)
         self._refresh = refresh
         self._query = str(query)
-        self._view = None
+        self._view = ''
         Search.__init__(self, query=query, api='SubjectClassifications', **kwds)
         path = ['subject-classifications', 'subject-classification']
         self._n = len(chained_get(self._json, path, []))
 
     def __str__(self):
         """Print a summary string."""
         areas = [r.code for r in self.results]
```

### Comparing `pybliometrics-3.6/pybliometrics/scopus/superclasses/base.py` & `pybliometrics-4.0/pybliometrics/scopus/superclasses/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -171,15 +171,18 @@
 def _get_all_refs(url: str, params: dict, verbose: bool, resp: dict, *args, **kwds) -> dict:
     """Get all references for `AbstractRetrieval` with view `REF`."""
     # startref starts at 1 (0 does not work)
     # Max refs per query are 40
     # Use of refcount leads to errors
     res = resp.json()
     path_total_references = ['abstracts-retrieval-response', 'references', '@total-references']
-    n = int(parse_content.chained_get(res, path_total_references))
+    try:
+        n = int(parse_content.chained_get(res, path_total_references))
+    except TypeError:
+        return res
 
     data  = res #data is used to gather all responses. res is a tmp variable
 
     path_reference = ['abstracts-retrieval-response', 'references', 'reference']
     ref_len = len(parse_content.chained_get(data, path_reference))
     n_chunks = ceil(n/ref_len)
```

### Comparing `pybliometrics-3.6/pybliometrics/scopus/superclasses/retrieval.py` & `pybliometrics-4.0/pybliometrics/scopus/superclasses/retrieval.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Superclass to access all Scopus retrieval APIs and dump the results."""
 
+from pathlib import Path
 from typing import Union
 
 from pybliometrics.scopus.superclasses import Base
-from pybliometrics.scopus.utils import get_folder, URLS
+from pybliometrics.scopus.utils import get_config, URLS
 
 
 class Retrieval(Base):
     def __init__(self,
                  identifier: Union[int, str],
                  api: str,
                  id_type: str = None,
@@ -37,12 +38,15 @@
         if api == 'CitationOverview':
             stem = identifier.replace("/", "")
             if self._citation:
                 identifier += "-" + self._citation
         else:
             url += identifier
             stem = identifier.replace('/', '_')
-        self._cache_file_path = get_folder(api, self._view)/stem
+        # Get cache file path
+        config = get_config()
+        parent = Path(config.get('Directories', api))
+        self._cache_file_path = parent/self._view/stem
 
         # Parse file contents
         params = {'view': self._view, **kwds}
         Base.__init__(self, params=params, url=url, api=api)
```

### Comparing `pybliometrics-3.6/pybliometrics/scopus/superclasses/search.py` & `pybliometrics-4.0/pybliometrics/scopus/superclasses/search.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Superclass to access all Scopus search APIs and dump the results."""
 
 from hashlib import md5
+from pathlib import Path
 
 from pybliometrics.scopus.superclasses import Base
-from pybliometrics.scopus.utils import get_folder, URLS
+from pybliometrics.scopus.utils import get_config, URLS
 
 
 class Search(Base):
     def __init__(self,
                  query: str,
                  api: str,
                  count: int = 200,
@@ -52,15 +53,18 @@
             params.update({'cursor': '*'})
         else:
             if "start" not in params:
                 params['start'] = 0
 
         # Construct cache file path
         stem = md5(name.encode('utf8')).hexdigest()
-        self._cache_file_path = get_folder(api, self._view)/stem
+        # Get cache file path
+        config = get_config()
+        parent = Path(config.get('Directories', api))
+        self._cache_file_path = parent/self._view/stem
 
         # Init
         Base.__init__(self, params=params, url=URLS[api], download=download,
                       api=api, verbose=verbose)
 
     def get_results_size(self) -> int:
         """Return the number of results (works even if download=False)."""
```

### Comparing `pybliometrics-3.6/pybliometrics/scopus/tests/README.md` & `pybliometrics-4.0/pybliometrics/scopus/tests/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-These testfiles are designed to test features of the various classes.  To run these tests, you need the [nosetesting package](http://nose.readthedocs.io/en/latest/).
+These testfiles are designed to test features of the various classes. The simplest way to invoke the tests is to execute
 
-The simplest way to invoke the tests is to execute
-
-    nosetests3 --verbose
+    pytest --verbose
 
 in the command line from within the pybliometrics repo.  By passing a specific filename, you can test only one suite:
 
-    nosetests3 pybliometrics/scopus/tests/test_AffiliationRetrieval.py --verbose
+    pytest pybliometrics/scopus/tests/test_AffiliationRetrieval.py --verbose
 
-Windows users should try `python -m` if nosetests3 fail.
+Windows users should try `python -m` in front of above commands.
 
 During the tests, files from the Scopus database are downloaded and cached in the usual way.  Hence, tests make use of your API Key and require a valid connection.
+
```

### Comparing `pybliometrics-3.6/pybliometrics/scopus/tests/test_AbstractRetrieval.py` & `pybliometrics-4.0/pybliometrics/scopus/tests/test_AbstractRetrieval.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
 """Tests for `scopus.AbstractRetrieval` module."""
 
 from collections import namedtuple
-from nose.tools import assert_equal, assert_true
 
-from pybliometrics.scopus import AbstractRetrieval
+from pybliometrics.scopus import AbstractRetrieval, init
+
+init()
 
 # Base information
 ab1 = AbstractRetrieval("2-s2.0-84930616647", view="FULL", refresh=30)
 # Conference proceeding and no references
 ab2 = AbstractRetrieval("2-s2.0-0029486824", view="FULL", refresh=30)
 # Issuetitle and no affiliation
 ab3 = AbstractRetrieval("2-s2.0-0001270077", view="FULL", refresh=30)
@@ -21,380 +20,392 @@
 ab6 = AbstractRetrieval("2-s2.0-85040230676", view="FULL", refresh=30)
 # Contributor group
 ab7 = AbstractRetrieval("2-s2.0-85050253030", view="FULL", refresh=30)
 # REF view
 ab8 = AbstractRetrieval("2-s2.0-84951753303", view="REF", refresh=30)
 # Collaboration
 ab9 = AbstractRetrieval("2-s2.0-85097473741", view="FULL", refresh=30)
+# ENTITLED view
+ar10 = AbstractRetrieval('10.1109/Multi-Temp.2019.8866947', view='ENTITLED', refresh=30)
+# REF view without refs
+ab11 = AbstractRetrieval('2-s2.0-0031874638', view="REF", refresh=30)
 
 
 def test_abstract():
     expected = 'In this paper we propose a Bayesian analysis of seasonal '\
         'unit roots in quarterly observed time series. Seasonal unit root '\
         'processes are useful to describe economic series with changing '\
         'seasonal fluctuations. A natural alternative model for similar '\
         'purposes contains deterministic seasonal mean shifts instead of '\
         'seasonal stochastic trends. This leads to analysing seasonal unit '\
         'roots in the presence of mean shifts using Bayesian techniques. '\
         'Our method is illustrated using several simulated and empirical data.'
-    assert_equal(ab4.abstract, expected)
-    assert_equal(ab8.abstract, None)
+    assert ab4.abstract == expected
+    assert ab8.abstract is None
 
 
 def test_affiliation():
     aff = namedtuple('Affiliation', 'id name city country')
-    expected = [aff(id=60027950, name='Carnegie Mellon University',
+    expected = [aff(id=60104842, name='College of Engineering',
                     city='Pittsburgh', country='United States')]
-    assert_equal(ab1.affiliation, expected)
-    assert_equal(ab3.affiliation, None)
-    assert_equal(ab8.affiliation, None)
+    assert ab1.affiliation == expected
+    assert ab3.affiliation is None
+    assert ab8.affiliation is None
 
 
 def test_aggregationType():
-    assert_equal(ab1.aggregationType, 'Journal')
-    assert_equal(ab2.aggregationType, 'Conference Proceeding')
-    assert_equal(ab8.aggregationType, None)
+    assert ab1.aggregationType == 'Journal'
+    assert ab2.aggregationType == 'Conference Proceeding'
+    assert ab8.aggregationType is None
 
 
 def test_authkeywords():
-    assert_equal(ab1.authkeywords, None)
+    assert ab1.authkeywords is None
     expected = ['Bayesian analysis', 'Seasonality',
                 'Structural breaks', 'Unit roots']
-    assert_equal(ab4.authkeywords, expected)
-    assert_equal(ab8.authkeywords, None)
+    assert ab4.authkeywords == expected
+    assert ab8.authkeywords is None
 
 
 def test_authorgroup():
     fields = 'affiliation_id dptid organization city postalcode addresspart '\
              'country collaboration auid orcid indexed_name surname given_name'
     auth = namedtuple('Author', fields)
-    expected = [auth(affiliation_id=60027950, dptid=110785688,
+    expected = [auth(affiliation_id=60104842, dptid=None,
         organization='Department of Chemical Engineering, Carnegie Mellon University',
         city='Pittsburgh', postalcode='15213', addresspart='5000 Forbes Avenue',
         country='United States', collaboration=None, auid=7004212771, orcid=None,
-        indexed_name='Kitchin J.', surname='Kitchin', given_name='John R.')]
-    assert_equal(ab1.authorgroup, expected)
-    assert_equal(ab8.authorgroup, None)
+        indexed_name='Kitchin J.R.', surname='Kitchin', given_name='John R.')]
+    assert ab1.authorgroup == expected
+    assert ab8.authorgroup is None
     expected = auth(affiliation_id=None, dptid=None, organization=None,
         city=None, postalcode=None, addresspart=None, country=None,
         collaboration='J-PARC-HI Collaboration', auid=7403019450, orcid=None,
         indexed_name='Ahn J.K.', surname='Ahn', given_name='J.K.')
-    assert_equal(ab9.authorgroup[0], expected)
+    assert ab9.authorgroup[0] == expected
 
 
 
 def test_authors():
     fields = 'auid indexed_name surname given_name affiliation_id'
     auth = namedtuple('Author', fields)
     expected = [auth(auid=7004212771, indexed_name='Kitchin J.R.',
                 surname='Kitchin', given_name='John R.',
-                affiliation_id='60027950')]
-    assert_equal(ab1.authors, expected)
-    assert_equal(ab8.authors, None)
+                affiliation_id='60104842')]
+    assert ab1.authors == expected
+    assert ab8.authors is None
+    assert ar10.authors is None
 
 
 def test_citedby_count():
     expected = 5
-    assert_true(ab1.citedby_count >= expected)
-    assert_equal(ab8.citedby_count, None)
+    assert ab1.citedby_count >= expected
+    assert ab8.citedby_count is None
 
 
 def test_citedby_link():
     expected = 'https://www.scopus.com/inward/citedby.uri?partnerID=HzOxMe3b'\
         '&scp=84930616647&origin=inward'
-    assert_equal(ab1.citedby_link, expected)
-    assert_equal(ab8.citedby_link, None)
+    assert ab1.citedby_link == expected
+    assert ab8.citedby_link is None
 
 
 def test_chemials():
     received = ab6.chemicals
-    assert_true(isinstance(received, list))
-    assert_equal(len(received), 6)
+    assert isinstance(received, list)
+    assert len(received) == 6
     chemical = namedtuple('Chemical', 'source chemical_name cas_registry_number')
     expected = chemical(source='esbd', cas_registry_number='126547-89-5',
         chemical_name='intercellular adhesion molecule 1')
-    assert_true(expected in received)
-    assert_equal(ab3.chemicals, None)
-    assert_equal(ab8.chemicals, None)
+    assert expected in received
+    assert ab3.chemicals is None
+    assert ab8.chemicals is None
 
 
 def test_confcode():
-    assert_equal(ab2.confcode, 44367)
-    assert_equal(ab8.confcode, None)
+    assert ab2.confcode == 44367
+    assert ab8.confcode is None
 
 
 def test_confdate():
-    assert_equal(ab2.confdate, ((1995, 12, 13), (1995, 12, 15)))
-    assert_equal(ab8.confdate, None)
+    assert ab2.confdate == ((1995, 12, 13), (1995, 12, 15))
+    assert ab8.confdate is None
 
 
 def test_conflocation():
-    assert_equal(ab2.conflocation, 'New Orleans, LA, USA')
-    assert_equal(ab8.conflocation, None)
+    assert ab2.conflocation == 'New Orleans, LA, USA'
+    assert ab8.conflocation is None
 
 
 def test_confname():
     expected2 = "Proceedings of the 1995 34th IEEE Conference on Decision "\
                 "and Control. Part 1 (of 4)"
-    assert_equal(ab2.confname, expected2)
-    assert_equal(ab3.confname, None)
+    assert ab2.confname == expected2
+    assert ab3.confname is None
     expected7 = '20th Symposium on Design, Test, Integration and Packaging '\
                 'of MEMS and MOEMS, DTIP 2018'
-    assert_equal(ab7.confname, expected7)
-    assert_equal(ab8.confname, None)
+    assert ab7.confname == expected7
+    assert ab8.confname is None
 
 
 def test_confsponsor():
-    assert_equal(ab2.confsponsor, 'IEEE')
-    assert_equal(ab3.confsponsor, None)
+    assert ab2.confsponsor == 'IEEE'
+    assert ab3.confsponsor is None
     expected7 = ['ARTOV.IMM.CNR.IT', 'CMP.IMAG.FR', 'CNRS.FR',
                  'EPS.IEEE.ORG', 'LIRMM.FR']
-    assert_equal(ab7.confsponsor, expected7)
-    assert_equal(ab8.confsponsor, None)
+    assert ab7.confsponsor == expected7
+    assert ab8.confsponsor is None
 
 
 def test_contributor_group():
     fields = 'given_name initials surname indexed_name role'
     pers = namedtuple('Contributor', fields)
     expected = pers(given_name='Romolo', initials='R.', surname='Marcelli',
                     indexed_name='Marcelli R.', role='edit')
     received = ab7.contributor_group
-    assert_equal(len(received), 7)
-    assert_true(expected in received)
-    assert_equal(ab3.contributor_group, None)
-    assert_equal(ab8.contributor_group, None)
+    assert len(received) == 7
+    assert expected in received
+    assert ab3.contributor_group is None
+    assert ab8.contributor_group is None
 
 
 def test_copyright():
-    assert_equal(ab8.copyright, None)
+    assert ab8.copyright is None
     expected = "Copyright 2021 Elsevier B.V., All rights reserved."
-    assert_equal(ab9.copyright, expected)
+    assert ab9.copyright == expected
 
 
 def test_copyright_type():
-    assert_equal(ab8.copyright_type, None)
-    assert_equal(ab9.copyright_type, "Elsevier")
+    assert ab8.copyright_type is None
+    assert ab9.copyright_type == "Elsevier"
 
 
 def test_correspondence():
     fields = 'surname initials organization country city_group'
     corr = namedtuple('Correspondence', fields)
     expected2 = corr(surname='Boukas', initials='E.K.',
         organization='Ecole Polytechnique de Montreal', country='Canada',
         city_group='Montreal')
-    assert_equal(ab2.correspondence[0], expected2)
-    assert_equal(ab3.correspondence, None)
-    assert_equal(ab8.correspondence, None)
+    assert ab2.correspondence[0] == expected2
+    assert ab3.correspondence is None
+    assert ab8.correspondence is None
 
 
 def test_coverDate():
-    assert_equal(ab1.coverDate, '2015-06-05')
-    assert_equal(ab8.coverDate, None)
+    assert ab1.coverDate == '2015-06-05'
+    assert ab8.coverDate is None
 
 
 def test_date_created():
-    assert_equal(ab8.date_created, None)
-    assert_equal(ab9.date_created, (2021, 9, 14))
+    assert ab8.date_created is None
+    assert ab9.date_created == (2021, 9, 14)
 
 
 def test_description():
     expected = 'In this paper we propose a Bayesian analysis of seasonal '\
                'unit roots in quarterly observed time series. Seasonal unit '\
                'root processes are useful to describe economic series with '\
                'changing seasonal fluctuations. A natural alternative model '\
                'for similar purposes contains deterministic seasonal mean '\
                'shifts instead of seasonal stochastic trends. This leads to '\
                'analysing seasonal unit roots in the presence of mean '\
                'shifts using Bayesian techniques. Our method is illustrated '\
                'using several simulated and empirical data.'
-    assert_equal(ab4.description, expected)
-    assert_equal(ab8.description, None)
+    assert ab4.description == expected
+    assert ab8.description is None
 
 
 def test_doi():
-    assert_equal(ab1.doi, '10.1021/acscatal.5b00538')
-    assert_equal(ab4.doi, '10.1016/s0304-4076(97)00018-3')
-    assert_equal(ab8.doi, None)
+    assert ab1.doi == '10.1021/acscatal.5b00538'
+    assert ab4.doi == '10.1016/s0304-4076(97)00018-3'
+    assert ab8.doi is None
 
 
 def test_eid():
-    assert_equal(ab1.eid, '2-s2.0-84930616647')
-    assert_equal(ab8.eid, None)
+    assert ab1.eid == '2-s2.0-84930616647'
+    assert ab8.eid is None
 
 
 def test_endingPage():
-    assert_equal(ab1.endingPage, '3899')
-    assert_equal(ab8.endingPage, None)
+    assert ab1.endingPage == '3899'
+    assert ab8.endingPage is None
+
+
+def test_entitlement():
+    assert ab8.document_entitlement_status is None
+    assert ab9.document_entitlement_status is None
+    assert ar10.document_entitlement_status == 'ENTITLED'
 
 
 def test_funding():
     received = ab6.funding
-    assert_true(isinstance(received, list))
-    assert_equal(len(received), 5)
+    assert isinstance(received, list)
+    assert len(received) == 5
     fund = namedtuple('Funding', 'agency agency_id string funding_id acronym country')
     expected6 = fund(
         agency='Deutsche Forschungsgemeinschaft',
         agency_id='http://data.elsevier.com/vocabulary/SciValFunders/501100001659',
         string='German Research Foundation', acronym='DFG',
         funding_id=['SFB685'],
         country='http://sws.geonames.org/2921044/')
-    assert_true(expected6 in received)
-    assert_equal(ab5.funding, None)
-    assert_equal(ab8.funding, None)
+    assert expected6 in received
+    assert ab5.funding is None
+    assert ab8.funding is None
 
 
 def test_funding_text():
     e = 'ACKNOWLEDGMENTS. We thank Dieter Blaas for providing ICAM-1–specific '\
         'antiserum (supersup). This work was supported by Netherlands '\
         'Organization for Scientific Research Grant NWO-VICI-91812628 '\
         '(to F.J.M.v.K.), by German Research Foundation Grant SFB685 '\
         '(to T.S. and G.Z.), and Wellcome Trust PhD Studentship support '\
         '102572/B/13/Z (to D.L.H.). All EM was performed in the Astbury '\
         'Biostructure Laboratory, which was funded by the University of '\
         'Leeds and the Wellcome Trust (108466/Z/15/Z).'
-    assert_equal(ab6.funding_text, e)
-    assert_equal(ab8.funding_text, None)
+    assert ab6.funding_text == e
+    assert ab8.funding_text is None
 
 
 def test_get_bibtex():
     e = '@article{Kaufmann1991FairnessPricing,\n  author = {Patrick J. '\
         'Kaufmann and Gwen Ortmeyer and N. Craig Smith},\n  title = {{'\
         'Fairness in consumer pricing}},\n  journal = {Journal of Consumer '\
         'Policy},\n  year = {1991},\n  volume = {14},\n  number = {2},\n  '\
         'pages = {117-140},\n  doi = {10.1007/BF00381915}}'
-    assert_equal(ab3.get_bibtex(), e)
+    assert ab3.get_bibtex() == e
 
 
 def test_get_latex():
     e = 'Philip Hans Franses, Henk Hoekh and Richard Paap, \\textit{'\
         'Bayesian analysis of seasonal unit roots and seasonal mean shifts}, '\
         'Journal of Econometrics, \\textbf{78(2)}, pp. 359-380 (1997). \\'\
         'href{https://doi.org/10.1016/s0304-4076(97)00018-3}{doi:10.1016/'\
         's0304-4076(97)00018-3}, \\href{https://www.scopus.com/inward/'\
         'record.uri?partnerID=HzOxMe3b&scp=0000016206&origin=inward}'\
         '{scopus:2-s2.0-0000016206}.'
-    assert_equal(ab4.get_latex(), e)
+    assert ab4.get_latex() == e
 
 
 def test_get_ris():
     e = 'TY  - JOUR\nTI  - Examples of effective data sharing in scientific '\
         'publishing\nJO  - ACS Catalysis\nVL  - 5\nDA  - 2015-06-05\nPY  - '\
         '2015\nSP  - 3894-3899\nAU  - Kitchin J.R.\nDO  - 10.1021/'\
         'acscatal.5b00538\nUR  - https://doi.org/10.1021/acscatal.5b00538\n'\
         'IS  - 6\nER  - \n\n'
-    assert_equal(ab1.get_ris(), e)
+    assert ab1.get_ris() == e
 
 
 def test_get_html():
     e = '<a href="https://www.scopus.com/authid/detail.url?origin=Author'\
         'Profile&authorId=7201922462">Patrick J. Kaufmann</a>, <a href="'\
         'https://www.scopus.com/authid/detail.url?origin=AuthorProfile&'\
         'authorId=16430389100">Gwen Ortmeyer</a> and <a href="https://'\
         'www.scopus.com/authid/detail.url?origin=AuthorProfile&authorId='\
         '57225963896">N. Craig Smith</a>, <a href="https://www.scopus.com/'\
         'inward/record.uri?partnerID=HzOxMe3b&scp=0001270077&origin=inward">'\
         'Fairness in consumer pricing</a>, <a href="https://www.scopus.com/'\
         'source/sourceInfo.url?sourceId=130073">Journal of Consumer Policy'\
         '</a>, <b>14(2)</b>, pp. 117-140, (1991). <a href="https://doi.org/'\
         '10.1007/BF00381915">doi:10.1007/BF00381915</a>.'
-    assert_equal(ab3.get_html(), e)
+    assert ab3.get_html() == e
 
 
 def test_isbn():
-    assert_equal(ab3.isbn, None)
-    assert_equal(ab5.isbn, ('0203881486', '9780203881484'))
-    assert_equal(ab8.isbn, None)
+    assert ab3.isbn is None
+    assert ab5.isbn == ('0203881486', '9780203881484')
+    assert ab8.isbn is None
 
 
 def test_issn():
     issn = namedtuple('ISSN', 'print electronic')
     expected1 = issn(print='21555435', electronic=None)
-    assert_equal(ab1.issn, expected1)
+    assert ab1.issn == expected1
     expected3 = issn(print='03425843', electronic='15730700')
-    assert_equal(ab3.issn, expected3)
-    assert_equal(ab5.issn, None)
-    assert_equal(ab8.issn, None)
+    assert ab3.issn == expected3
+    assert ab5.issn is None
+    assert ab8.issn is None
 
 
 def test_identifier():
-    assert_equal(ab1.identifier, 84930616647)
-    assert_equal(ab8.identifier, None)
+    assert ab1.identifier == 84930616647
+    assert ab8.identifier is None
 
 
 def test_idxterms():
     expected = ['Control variables', 'Cost function',
                 'Hamilton-Jacobi-Isaacs equation', 'Machine capacity',
                 'Stochastic manufacturing systems', 'Value function']
-    assert_equal(ab2.idxterms, expected)
-    assert_equal(ab4.idxterms, None)
+    assert ab2.idxterms == expected
+    assert ab4.idxterms is None
 
 
 def test_issueIdentifier():
-    assert_equal(ab1.issueIdentifier, '6')
-    assert_equal(ab8.issueIdentifier, None)
+    assert ab1.issueIdentifier == '6'
+    assert ab8.issueIdentifier is None
 
 
 def test_issuetitle():
-    assert_equal(ab3.issuetitle, 'Law, Economics and Behavioural Sciences')
-    assert_equal(ab8.issuetitle, None)
+    assert ab3.issuetitle == 'Law, Economics and Behavioural Sciences'
+    assert ab8.issuetitle is None
 
 
 def test_language():
-    assert_equal(ab1.language, 'eng')
-    assert_equal(ab8.language, None)
+    assert ab1.language == 'eng'
+    assert ab8.language is None
 
 
 def test_openaccess():
-    assert_equal(ab5.openaccess, 2)
-    assert_equal(ab6.openaccess, 1)
-    assert_equal(ab7.openaccess, 0)
-    assert_equal(ab8.openaccess, None)
+    assert ab5.openaccess == 2
+    assert ab6.openaccess == 1
+    assert ab7.openaccess == 0
+    assert ab8.openaccess is None
 
 
 def test_openaccessFlag():
-    assert_equal(ab5.openaccessFlag, None)
-    assert_equal(ab6.openaccessFlag, True)
-    assert_equal(ab7.openaccessFlag, False)
-    assert_equal(ab8.openaccessFlag, None)
+    assert ab5.openaccessFlag is None
+    assert ab6.openaccessFlag == True
+    assert ab7.openaccessFlag == False
+    assert ab8.openaccessFlag is None
 
 
 def test_pageRange():
-    assert_equal(ab1.pageRange, '3894-3899')
-    assert_equal(ab8.pageRange, None)
+    assert ab1.pageRange == '3894-3899'
+    assert ab8.pageRange is None
 
 
 def test_pii():
-    assert_equal(ab4.pii, 'S0304407697000183')
-    assert_equal(ab5.pii, None)
-    assert_equal(ab6.pii, None)
+    assert ab4.pii == 'S0304407697000183'
+    assert ab5.pii is None
+    assert ab6.pii is None
 
 
 def test_publicationName():
-    assert_equal(ab1.publicationName, 'ACS Catalysis')
-    assert_equal(ab8.publicationName, None)
+    assert ab1.publicationName == 'ACS Catalysis'
+    assert ab8.publicationName is None
 
 
 def test_publisher():
-    assert_equal(ab1.publisher, 'American Chemical Society')
-    assert_equal(ab8.publisher, None)
+    assert ab1.publisher == 'American Chemical Society'
+    assert ab8.publisher is None
 
 
 def test_publisheraddress():
-    assert_equal(ab2.publisheraddress, 'Piscataway, NJ, United States')
-    assert_equal(ab8.publisheraddress, None)
+    assert ab2.publisheraddress == 'Piscataway, NJ, United States'
+    assert ab8.publisheraddress is None
 
 
 def test_pubmed_id():
-    assert_equal(ab6.pubmed_id, 29284752)
-    assert_equal(ab7.pubmed_id, None)
+    assert ab6.pubmed_id == 29284752
+    assert ab7.pubmed_id is None
 
 
 def test_refcount():
-    assert_equal(ab4.refcount, 18)
-    assert_equal(ab8.refcount, 48)
+    assert ab4.refcount == 18
+    assert ab8.refcount == 48
+    assert ab11.refcount is None
 
 
 def test_references_full():
     fields = 'position id doi title authors authors_auid authors_affiliationid '\
              'sourcetitle publicationyear coverDate volume issue first last '\
              'citedbycount type text fulltext'
     ref = namedtuple('Reference', fields)
@@ -408,128 +419,126 @@
         last=None, citedbycount=None, text='Eds. Chapman and Hall/CRC: London.')
     expected7 = ref(position='1', id='85050215448', doi=None, title=None,
         authors='', authors_auid=None, authors_affiliationid=None,
         sourcetitle=None, publicationyear=None, coverDate=None, volume=None,
         issue=None, first=None, last=None, citedbycount=None, type=None,
         text='accessed 27 June 2017',
         fulltext='www. hexoskin. com, accessed 27 June 2017')
-    assert_equal(ab1.references[-1], expected1)
-    assert_equal(ab2.references, None)
-    assert_equal(ab7.references[0], expected7)
+    assert ab1.references[-1] == expected1
+    assert ab2.references is None
+    assert ab7.references[0] == expected7
 
 
 def test_references_ref():
-    assert_equal(len(ab8.references), 48)
+    assert len(ab8.references) == 48
     fields = 'position id doi title authors authors_auid authors_affiliationid '\
              'sourcetitle publicationyear coverDate volume issue first last '\
              'citedbycount type text fulltext'
     ref = namedtuple('Reference', fields)
     expected8 = ref(position='47', id='77953310709',
         doi='10.1109/INFCOM.2010.5462174', text=None, fulltext=None,
         title='Achieving secure, scalable, and fine-grained data access control in cloud computing',
         authors='Yu, Shucheng; Lou, Wenjing; Wang, Cong; Ren, Kui',
         authors_auid='55636591800; 7006030576; 35106222100; 8396435500',
         authors_affiliationid='60011410; 60011410; 60002873; 60002873',
         sourcetitle='Proceedings - IEEE INFOCOM',
         publicationyear=None, coverDate='2010-06-15', volume=None, issue=None,
         first=None, last=None, citedbycount='0', type='resolvedReference')
-    assert_equal(ab8.references[-2]._replace(citedbycount="0"), expected8)
-    assert_true(int(ab8.references[-2].citedbycount) >= 0)
+    assert ab8.references[-2]._replace(citedbycount="0") == expected8
+    assert int(ab8.references[-2].citedbycount) >= 0
+    assert ab11.references is None
 
 
 def test_scopus_link():
     expected = 'https://www.scopus.com/inward/record.uri?partnerID=HzOxMe3b&'\
         'scp=84930616647&origin=inward'
-    assert_equal(ab1.scopus_link, expected)
+    assert ab1.scopus_link == expected
 
 
 def test_self_link():
     expected = 'https://api.elsevier.com/content/abstract/scopus_id/84930616647'
-    assert_equal(ab1.self_link, expected)
-    assert_equal(ab8.self_link, None)
+    assert ab1.self_link == expected
+    assert ab8.self_link is None
 
 
 def test_sequencebank():
     received = ab6.sequencebank
-    assert_true(isinstance(received, list))
-    assert_equal(len(received), 3)
+    assert isinstance(received, list)
+    assert len(received) == 3
     bank = namedtuple('Chemical', 'name sequence_number type')
     expected = bank(name='GENBANK', sequence_number='MG272373',
                     type='referenced')
-    assert_true(expected in received)
-    assert_equal(ab3.sequencebank, None)
-    assert_equal(ab8.sequencebank, None)
+    assert expected in received
+    assert ab3.sequencebank is None
+    assert ab8.sequencebank is None
 
 
 def test_source_id():
-    assert_equal(ab1.source_id, 19700188320)
-    assert_equal(ab8.source_id, None)
+    assert ab1.source_id == 19700188320
+    assert ab8.source_id is None
 
 
 def test_sourcetitle_abbreviation():
-    assert_equal(ab1.sourcetitle_abbreviation, 'ACS Catal.')
-    assert_equal(ab8.sourcetitle_abbreviation, None)
+    assert ab1.sourcetitle_abbreviation == 'ACS Catal.'
+    assert ab8.sourcetitle_abbreviation is None
 
 
 def test_srctype():
-    assert_equal(ab1.srctype, 'j')
-    assert_equal(ab2.srctype, 'p')
-    assert_equal(ab8.srctype, None)
+    assert ab1.srctype == 'j'
+    assert ab2.srctype == 'p'
+    assert ab8.srctype is None
 
 
 def test_startingPage():
-    assert_equal(ab1.startingPage, '3894')
-    assert_equal(ab8.startingPage, None)
+    assert ab1.startingPage == '3894'
+    assert ab8.startingPage is None
 
 
 def test_subject_areas():
     area = namedtuple('Area', 'area abbreviation code')
     expected = [area(area='Catalysis', abbreviation='CENG', code=1503),
                 area(area='Chemistry (all)', abbreviation='CHEM', code=1600)]
-    assert_equal(ab1.subject_areas, expected)
-    assert_equal(ab8.subject_areas, None)
+    assert ab1.subject_areas == expected
+    assert ab8.subject_areas is None
     expected = [area(area='Nuclear and High Energy Physics',
                      abbreviation='PHYS', code=3106)]
-    assert_equal(ab9.subject_areas, expected)
+    assert ab9.subject_areas == expected
 
 
 def test_subtype():
-    assert_equal(ab1.subtype, "re")
-    assert_equal(ab2.subtype, "cp")
-    assert_equal(ab5.subtype, "bk")
-    assert_equal(ab6.subtype, "ar")
+    assert ab1.subtype == "re"
+    assert ab2.subtype == "cp"
+    assert ab5.subtype == "bk"
+    assert ab6.subtype == "ar"
+    assert ar10.subtype is None
 
 
 def test_subtypedescription():
-    assert_equal(ab1.subtypedescription, "Review")
-    assert_equal(ab2.subtypedescription, "Conference Paper")
-    assert_equal(ab5.subtypedescription, "Book")
-    assert_equal(ab6.subtypedescription, "Article")
+    assert ab1.subtypedescription == "Review"
+    assert ab2.subtypedescription == "Conference Paper"
+    assert ab5.subtypedescription == "Book"
+    assert ab6.subtypedescription == "Article"
+    assert ar10.subtypedescription is None
 
 
 def test_title():
     expected = 'Examples of effective data sharing in scientific publishing'
-    assert_equal(ab1.title, expected)
-    assert_equal(ab8.title, None)
+    assert ab1.title == expected
+    assert ab8.title is None
+    assert ar10.title is None
 
 
 def test_url():
     expected = 'https://api.elsevier.com/content/abstract/scopus_id/84930616647'
-    assert_equal(ab1.url, expected)
-    assert_equal(ab8.url, None)
+    assert ab1.url == expected
+    assert ab8.url is None
 
 
 def test_volume():
-    assert_equal(ab1.volume, '5')
-    assert_equal(ab8.volume, None)
+    assert ab1.volume == '5'
+    assert ab8.volume is None
 
 
 def test_website():
-    assert_equal(ab1.website, 'http://pubs.acs.org/page/accacs/about.html')
-    assert_equal(ab2.website, None)
-    assert_equal(ab8.website, None)
-
-
-def test_all_refs():
-    refs_downloaded = len(ab8.references)
-    expected = ab8.refcount
-    assert_equal(refs_downloaded, expected)
+    assert ab1.website == 'http://pubs.acs.org/page/accacs/about.html'
+    assert ab2.website is None
+    assert ab8.website is None
```

### Comparing `pybliometrics-3.6/pybliometrics/scopus/tests/test_AffiliationRetrieval.py` & `pybliometrics-4.0/pybliometrics/scopus/tests/test_AffiliationRetrieval.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,124 +1,150 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
 """Tests for `scopus.AffiliationRetrieval` module."""
 
-from nose.tools import assert_equal, assert_true
+from pybliometrics.scopus import AffiliationRetrieval, init
 
-from pybliometrics.scopus import AffiliationRetrieval
+init()
 
 
 light = AffiliationRetrieval('60000356', refresh=30, view="LIGHT")
 standard = AffiliationRetrieval('60000356', refresh=30, view="STANDARD")
+entitled = AffiliationRetrieval('60000356', refresh=30, view='ENTITLED')
 
 
 def test_address():
-    assert_equal(light.address, 'Private Bag X3')
-    assert_equal(standard.address, 'Private Bag X3')
+    assert light.address == 'Private Bag X3'
+    assert standard.address == 'Private Bag X3'
+    assert entitled.address is None
 
 
 def test_affiliation_name():
-    assert_equal(light.affiliation_name, 'University of Cape Town')
-    assert_equal(standard.affiliation_name, 'University of Cape Town')
+    assert light.affiliation_name == 'University of Cape Town'
+    assert standard.affiliation_name == 'University of Cape Town'
+    assert entitled.affiliation_name is None
 
 
 def test_author_count():
     expected = 12800
-    assert_true(light.author_count >= expected)
-    assert_true(standard.author_count >= expected)
+    assert light.author_count >= expected
+    assert standard.author_count >= expected
+    assert entitled.author_count is None
 
 
 def test_city():
-    assert_equal(light.city, 'Cape Town')
-    assert_equal(standard.city, 'Cape Town')
+    assert light.city == 'Cape Town'
+    assert standard.city == 'Cape Town'
+    assert entitled.city is None
 
 
 def test_country():
-    assert_equal(light.country, 'South Africa')
-    assert_equal(standard.country, 'South Africa')
+    assert light.country == 'South Africa'
+    assert standard.country == 'South Africa'
+    assert entitled.country is None
 
 
 def test_date_created():
-    assert_equal(light.date_created, None)
-    assert_equal(standard.date_created, (2008, 2, 2))
+    assert light.date_created is None
+    assert standard.date_created == (2008, 2, 2)
+    assert entitled.date_created is None
 
 
 def test_document_count():
     expected = 73581
-    assert_true(light.document_count >= expected)
-    assert_true(standard.document_count >= expected)
+    assert light.document_count >= expected
+    assert standard.document_count >= expected
+    assert entitled.document_count is None
 
 
 def test_eid():
-    assert_equal(light.eid, '10-s2.0-60000356')
-    assert_equal(standard.eid, '10-s2.0-60000356')
+    assert light.eid == '10-s2.0-60000356'
+    assert standard.eid == '10-s2.0-60000356'
+    assert entitled.eid is None
+
+
+def test_entitlement():
+    assert standard.document_entitlement_status is None
+    assert light.document_entitlement_status is None
+    assert entitled.document_entitlement_status == 'ENTITLED'
 
 
 def test_identifier():
-    assert_equal(light.identifier, 60000356)
-    assert_equal(standard.identifier, 60000356)
+    assert light.identifier == 60000356
+    assert standard.identifier == 60000356
+    assert entitled.identifier is None
 
 
 def test_name_variants():
     expected = "<class 'pybliometrics.scopus.affiliation_retrieval.Variant'>"
-    assert_equal(str(type(light.name_variants[0])), expected)
-    assert_equal(str(type(standard.name_variants[0])), expected)
+    assert str(type(light.name_variants[0])) == expected
+    assert str(type(standard.name_variants[0])) == expected
+    assert entitled.name_variants is None
 
 
 def test_org_domain():
-    assert_equal(light.org_domain, None)
-    assert_equal(standard.org_domain, 'uct.ac.za')
+    assert light.org_domain is None
+    assert standard.org_domain == 'uct.ac.za'
+    assert entitled.org_domain is None
 
 
 def test_org_type():
-    assert_equal(light.org_type, None)
-    assert_equal(standard.org_type, 'univ')
+    assert light.org_type is None
+    assert standard.org_type == 'univ'
+    assert entitled.org_type is None
 
 
 def test_org_URL():
-    assert_equal(light.org_URL, None)
-    assert_equal(standard.org_URL, 'http://www.uct.ac.za')
+    assert light.org_URL is None
+    assert standard.org_URL == 'http://www.uct.ac.za'
+    assert entitled.org_URL is None
 
 
 def test_postal_code():
-    assert_equal(light.postal_code, None)
-    assert_equal(standard.postal_code, '7701')
+    assert light.postal_code is None
+    assert standard.postal_code == '7701'
+    assert entitled.postal_code is None
 
 
 def test_scopus_affiliation_link():
     expected = 'https://www.scopus.com/affil/profile.uri?afid='\
                '60000356&partnerID=HzOxMe3b&origin=inward'
-    assert_equal(light.scopus_affiliation_link, expected)
-    assert_equal(standard.scopus_affiliation_link, expected)
+    assert light.scopus_affiliation_link == expected
+    assert standard.scopus_affiliation_link == expected
+    assert entitled.scopus_affiliation_link is None
 
 
 def test_self_link():
     expected = 'https://api.elsevier.com/content/affiliation/affiliation_id/60000356'
-    assert_equal(light.self_link, expected)
-    assert_equal(standard.self_link, expected)
+    assert light.self_link == expected
+    assert standard.self_link == expected
+    assert entitled.self_link is None
 
 
 def test_search_link():
     expected = 'https://api.elsevier.com/content/search/scopus?query=af-id%2860000356%29'
-    assert_equal(light.search_link, expected)
-    assert_equal(standard.search_link, expected)
+    assert light.search_link== expected
+    assert standard.search_link== expected
+    assert entitled.search_link is None
 
 
 def test_state():
-    assert_equal(light.state, None)
-    assert_equal(standard.state, 'Western Cape')
+    assert light.state is None
+    assert standard.state == 'Western Cape'
+    assert entitled.state is None
 
 
 def test_status():
-    assert_equal(light.status, None)
-    assert_equal(standard.status, "update")
+    assert light.status is None
+    assert standard.status == "update"
+    assert entitled.status is None
 
 
 def sort_name():
-    assert_equal(light.sort_name, None)
-    assert_equal(standard.sort_name, 'Cape Town, University of')
+    assert light.sort_name is None
+    assert standard.sort_name== 'Cape Town, University of'
+    assert entitled.sort_name is None
 
 
 def url():
     expected = 'https://api.elsevier.com/content/affiliation/affiliation_id/60000356'
-    assert_equal(light.url, expected)
-    assert_equal(standard.url, expected)
+    assert light.url== expected
+    assert standard.url== expected
+    assert entitled.url is None
```

### Comparing `pybliometrics-3.6/pybliometrics/scopus/tests/test_AffiliationSearch.py` & `pybliometrics-4.0/pybliometrics/scopus/tests/test_AffiliationSearch.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,33 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
 """Tests for `scopus.AffiliationSearch` module."""
 
 from collections import namedtuple
 
-from nose.tools import assert_equal, assert_true
+from pybliometrics.scopus import AffiliationSearch, init
 
-from pybliometrics.scopus import AffiliationSearch
+init()
 
 s1 = AffiliationSearch('AF-ID(60021784)', refresh=30)
 s2 = AffiliationSearch('AFFIL(Max Planck Munich)', download=False, refresh=True)
 
 
 def test_affiliations():
     received1 = s1.affiliations
-    assert_true(isinstance(received1, list))
+    assert isinstance(received1, list)
     order = 'eid name variant documents city country parent'
     Affiliation = namedtuple('Affiliation', order)
     expected = Affiliation(eid='10-s2.0-60021784', name='New York University',
         variant='', documents=0, city='New York', country='United States',
-        parent='0')
-    assert_true(received1[0].documents >= 90_000)
-    assert_equal(received1[0]._replace(documents=0), expected)
+        parent=None)
+    assert received1[0].documents >= 90_000
+    assert received1[0]._replace(documents=0) == expected
 
 
 def test_affiliations_nodownload():
-    assert_equal(s2.affiliations, None)
+    assert s2.affiliations is None
 
 
 def test_get_results_size():
     received1 = s1.get_results_size()
-    assert_true(received1 >= 1)
+    assert received1 >= 1
     received2 = s2.get_results_size()
-    assert_true(received2 >= 60)
+    assert received2 >= 60
```

### Comparing `pybliometrics-3.6/pybliometrics/scopus/tests/test_AuthorRetrieval.py` & `pybliometrics-4.0/pybliometrics/scopus/tests/test_AuthorRetrieval.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,24 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
 """Tests for `scopus.AuthorRetrieval` module."""
 
-import warnings
 from collections import Counter, namedtuple
-from nose.tools import assert_equal, assert_true
 
-from pybliometrics.scopus import AuthorRetrieval
+from pybliometrics.scopus import AuthorRetrieval, init
 
-warnings.simplefilter("always")
+init()
 
 metrics = AuthorRetrieval("7004212771", refresh=30, view="METRICS")
 light = AuthorRetrieval("7004212771", refresh=30, view="LIGHT")
 standard = AuthorRetrieval("7004212771", refresh=30, view="STANDARD")
 enhanced = AuthorRetrieval("7004212771", refresh=30, view="ENHANCED")
+entitled = AuthorRetrieval(36009348900, view='ENTITLED')
 
 
 def test_affiliation_current():
-    assert_equal(metrics.affiliation_current, None)
+    assert metrics.affiliation_current is None
 
     order = 'id parent type relationship afdispname preferred_name '\
             'parent_preferred_name country_code country address_part city '\
             'state postal_code org_domain org_URL'
     aff = namedtuple('Affiliation', order, defaults=(None,) * len(order.split()))
 
     expected_std_enh = aff(id=60027950, parent=None, type='parent',
@@ -34,292 +31,283 @@
         relationship=None, afdispname=None, preferred_name='Carnegie Mellon University',
         parent_preferred_name=None, country_code=None, country='United States',
         address_part=None, city='Pittsburgh', state=None,
         postal_code=None, org_domain=None, org_URL=None)
 
     for a in (standard, enhanced, light):
         received = a.affiliation_current
-        assert_true(isinstance(received, list))
-        assert_true(len(received) >= 1)
+        assert isinstance(received, list)
+        assert len(received) >= 1
 
     for a in (standard, enhanced):
         received = a.affiliation_current
-        assert_true(expected_std_enh in received)
+        assert expected_std_enh in received
 
-    assert_true(expected_lgh in light.affiliation_current)
+    assert expected_lgh in light.affiliation_current
 
 
 def test_affiliation_history():
-    assert_equal(metrics.affiliation_history, None)
-    assert_equal(light.affiliation_history, None)
+    assert metrics.affiliation_history is None
+    assert light.affiliation_history is None
     order = 'id parent type relationship afdispname preferred_name '\
             'parent_preferred_name country_code country address_part city '\
             'state postal_code org_domain org_URL'
     aff = namedtuple('Affiliation', order)
     expected = aff(id=60008644, parent=None, type='parent',
         relationship='author', afdispname=None,
         preferred_name='Fritz Haber Institute of the Max Planck Society',
         parent_preferred_name=None, country_code='deu', country='Germany',
         address_part='Faradayweg 4-6', city='Berlin', state=None,
         postal_code='14195', org_domain='fhi.mpg.de',
         org_URL='https://www.fhi.mpg.de/')
     for a in (standard, enhanced):
         received = a.affiliation_history
-        assert_true(isinstance(received, list))
-        assert_true(len(received) >= 10)
-        assert_true(expected in received)
+        assert isinstance(received, list)
+        assert len(received) >= 10
+        assert expected in received
 
 
 def test_alias():
-    assert_equal(metrics.alias, None)
-    assert_equal(light.alias, None)
-    assert_equal(standard.alias, None)
-    assert_equal(enhanced.alias, None)
+    assert metrics.alias is None
+    assert light.alias is None
+    assert standard.alias is None
+    assert enhanced.alias is None
 
 
 def test_citation_count():
     expected = 13600
-    assert_true(metrics.citation_count >= expected)
-    assert_true(light.citation_count >= expected)
-    assert_true(standard.citation_count >= expected)
-    assert_true(enhanced.citation_count >= expected)
+    assert metrics.citation_count >= expected
+    assert light.citation_count >= expected
+    assert standard.citation_count >= expected
+    assert enhanced.citation_count >= expected
 
 
 def test_cited_by_count():
     expected = 10900
-    assert_true(metrics.cited_by_count >= expected)
-    assert_true(light.cited_by_count >= expected)
-    assert_true(standard.cited_by_count >= expected)
-    assert_true(enhanced.cited_by_count >= expected)
+    assert metrics.cited_by_count >= expected
+    assert light.cited_by_count >= expected
+    assert standard.cited_by_count >= expected
+    assert enhanced.cited_by_count >= expected
 
 
 def test_classificationgroup():
-    assert_equal(metrics.classificationgroup, None)
-    assert_equal(light.classificationgroup, None)
+    assert metrics.classificationgroup is None
+    assert light.classificationgroup is None
     for a in (standard, enhanced):
         received = a.classificationgroup
-        assert_true(isinstance(received, list))
-        assert_true(len(received) > 0)
-        assert_true((1906, 1) in received)  # frequency might differ
+        assert isinstance(received, list)
+        assert len(received) > 0
+        assert (1906, 1) in received  # frequency might differ
 
 
 def test_coauthor_count():
-    assert_equal(light.coauthor_count, None)
-    assert_equal(standard.coauthor_count, None)
+    assert light.coauthor_count is None
+    assert standard.coauthor_count is None
     expected = 175
-    assert_true(metrics.coauthor_count >= expected)
-    assert_true(enhanced.coauthor_count >= expected)
+    assert metrics.coauthor_count >= expected
+    assert enhanced.coauthor_count >= expected
 
 
 def test_coauthor_link():
-    assert_equal(metrics.coauthor_link, None)
-    assert_equal(light.coauthor_link, None)
-    assert_equal(standard.coauthor_link, None)
+    assert metrics.coauthor_link is None
+    assert light.coauthor_link is None
+    assert standard.coauthor_link is None
     expected = 'http://api.elsevier.com/content/search/author?co-author=7004212771'
-    assert_equal(enhanced.coauthor_link, expected)
+    assert enhanced.coauthor_link == expected
 
 
 def test_date_created():
-    assert_equal(metrics.date_created, None)
-    assert_equal(light.date_created, None)
-    assert_equal(standard.date_created, (2005, 12, 3))
-    assert_equal(enhanced.date_created, (2005, 12, 3))
+    assert metrics.date_created is None
+    assert light.date_created is None
+    assert standard.date_created, (2005, 12, 3)
+    assert enhanced.date_created, (2005, 12, 3)
 
 
 def test_document_count():
     expected = 106
-    assert_true(light.document_count >= expected)
-    assert_true(standard.document_count >= expected)
-    assert_true(metrics.document_count >= expected)
-    assert_true(enhanced.document_count >= expected)
+    assert light.document_count >= expected
+    assert standard.document_count >= expected
+    assert metrics.document_count >= expected
+    assert enhanced.document_count >= expected
 
 
 def test_eid():
-    assert_equal(metrics.eid, None)
-    assert_equal(light.eid, '9-s2.0-7004212771')
-    assert_equal(standard.eid, '9-s2.0-7004212771')
-    assert_equal(enhanced.eid, '9-s2.0-7004212771')
+    assert metrics.eid is None
+    assert light.eid, '9-s2.0-7004212771'
+    assert standard.eid, '9-s2.0-7004212771'
+    assert enhanced.eid, '9-s2.0-7004212771'
 
 
 def test_estimate_uniqueness():
-    expected = 2
-    assert_equal(metrics.estimate_uniqueness(), 0)
-    assert_equal(light.estimate_uniqueness(), 0)
-    assert_equal(standard.estimate_uniqueness(), expected)
-    assert_equal(enhanced.estimate_uniqueness(), expected)
+    assert metrics.estimate_uniqueness() == 2
+    assert light.estimate_uniqueness() == 2
+    assert standard.estimate_uniqueness() == 1
+    assert enhanced.estimate_uniqueness() == 1
+
+
+def test_entitlement():
+    assert metrics.document_entitlement_status is None
+    assert light.document_entitlement_status is None
+    assert standard.document_entitlement_status is None
+    assert enhanced.document_entitlement_status is None
+    assert entitled.document_entitlement_status == 'ENTITLED'
 
 
 def test_given_name():
-    assert_equal(metrics.given_name, None)
-    assert_equal(light.given_name, None)
-    assert_equal(standard.given_name, 'John R.')
-    assert_equal(enhanced.given_name, 'John R.')
+    assert metrics.given_name is None
+    assert light.given_name is None
+    assert standard.given_name == 'John R.'
+    assert enhanced.given_name == 'John R.'
 
 
 def get_coauthors():
-    assert_equal(metrics.get_coauthors(), None)
-    assert_equal(light.get_coauthors(), None)
-    assert_equal(standard.get_coauthors(), None)
+    assert metrics.get_coauthors() is None
+    assert light.get_coauthors() is None
+    assert standard.get_coauthors() is None
     received = enhanced.get_coauthors()
-    assert_true(isinstance(received, list))
-    assert_true(len(received) > 155)
+    assert isinstance(received, list)
+    assert len(received) > 155
     fields = 'surname given_name id areas affiliation_id name city country'
     coauth = namedtuple('Coauthor', fields)
     expected = coauth(surname='Rose', given_name='Michael E.', id=57209617104,
         areas='Computer Science (all)', affiliation_id=60105007,
         name='Max-Planck-Institut für Innovation und Wettbewerb',
         city='Munich', country='Germany')
-    assert_true(expected in received)
+    assert expected in received
 
 
 def test_get_documents():
     subtypes = {'re', 'ed', 'no'}
     received = enhanced.get_documents(subtypes)
-    assert_equal(len(received), 7)
+    assert len(received) == 8
 
 
 def test_get_document_eids():
     expected = 100
-    assert_true(len(enhanced.get_document_eids()) >= expected)
+    assert len(enhanced.get_document_eids()) >= expected
 
 
 def test_h_index():
-    assert_equal(light.h_index, None)
-    assert_equal(standard.h_index, None)
+    assert light.h_index is None
+    assert standard.h_index is None
     expected = 34
-    assert_true(metrics.h_index >= expected)
-    assert_true(enhanced.h_index >= expected)
+    assert metrics.h_index >= expected
+    assert enhanced.h_index >= expected
+    assert entitled.h_index is None
 
 
 def test_historical_identifier():
-    assert_equal(metrics.historical_identifier, None)
-    assert_equal(light.historical_identifier, None)
-    assert_equal(standard.historical_identifier, None)
+    assert metrics.historical_identifier is None
+    assert light.historical_identifier is None
+    assert standard.historical_identifier is None
     expected = [35787230500, 36488127000, 54974425600, 55004143700,
                 55004143800, 57057263700, 56641032000, 36747787600,
                 57206217299, 57219840256, 58343886400]
-    assert_equal(enhanced.historical_identifier, expected)
+    assert enhanced.historical_identifier == expected
 
 
 def test_identifier():
     expected = 7004212771
-    assert_equal(metrics.identifier, expected)
-    assert_equal(light.identifier, expected)
-    assert_equal(standard.identifier, expected)
-    assert_equal(enhanced.identifier, expected)
+    assert metrics.identifier == expected
+    assert light.identifier == expected
+    assert standard.identifier == expected
+    assert enhanced.identifier == expected
 
 
 def test_indexed_name():
-    assert_equal(metrics.indexed_name, None)
-    assert_equal(light.indexed_name, 'Kitchin J.')
-    assert_equal(standard.indexed_name, 'Kitchin J.')
-    assert_equal(enhanced.indexed_name, 'Kitchin J.')
+    assert metrics.indexed_name is None
+    assert light.indexed_name, 'Kitchin J.'
+    assert standard.indexed_name, 'Kitchin J.'
+    assert enhanced.indexed_name, 'Kitchin J.'
 
 
 def test_initials():
-    assert_equal(metrics.initials, None)
-    assert_equal(light.initials, None)
-    assert_equal(standard.initials, 'J.R.')
-    assert_equal(enhanced.initials, 'J.R.')
+    assert metrics.initials is None
+    assert light.initials is None
+    assert standard.initials, 'J.R.'
+    assert enhanced.initials, 'J.R.'
 
 
 def test_name_variants():
-    assert_equal(metrics.name_variants, None)
-    assert_equal(light.name_variants, None)
+    assert metrics.name_variants is None
+    assert light.name_variants is None
     expected = "<class 'pybliometrics.scopus.author_retrieval.Variant'>"
     for a in (standard, enhanced):
         received = a.name_variants
-        assert_true(isinstance(received, list))
-        assert_true(len(received) > 0)
-        assert_equal(str(type(received[0])), expected)
+        assert isinstance(received, list)
+        assert len(received) > 0
+        assert str(type(received[0])) == expected
+        assert isinstance(received[0].doc_count, int)
 
 
 def test_orcid():
-    assert_equal(metrics.orcid, None)
-    assert_equal(light.orcid, '0000-0003-2625-9232')
-    assert_equal(standard.orcid, '0000-0003-2625-9232')
-    assert_equal(enhanced.orcid, '0000-0003-2625-9232')
+    assert metrics.orcid is None
+    assert light.orcid, '0000-0003-2625-9232'
+    assert standard.orcid, '0000-0003-2625-9232'
+    assert enhanced.orcid, '0000-0003-2625-9232'
 
 
 def test_publication_range():
-    assert_equal(metrics.publication_range, None)
+    assert metrics.publication_range is None
     for a in (standard, enhanced, light):
-        assert_equal(a.publication_range[0], 1995)
-        assert_true(a.publication_range[1] >= 2021)
+        assert a.publication_range[0], 1995
+        assert a.publication_range[1] >= 2021
 
 
 def test_scopus_author_link():
-    assert_equal(metrics.scopus_author_link, None)
+    assert metrics.scopus_author_link is None
     expected = 'http://api.elsevier.com/content/author/author_id/7004212771'
-    assert_equal(light.scopus_author_link, expected)
-    assert_equal(standard.scopus_author_link, expected)
-    assert_equal(enhanced.scopus_author_link, expected)
+    assert light.scopus_author_link == expected
+    assert standard.scopus_author_link == expected
+    assert enhanced.scopus_author_link == expected
 
 
 def test_search_link():
-    assert_equal(metrics.search_link, None)
+    assert metrics.search_link is None
     expected = 'http://api.elsevier.com/content/search/scopus?query='\
                'au-id%287004212771%29'
-    assert_equal(light.search_link, expected)
-    assert_equal(standard.search_link, expected)
-    assert_equal(enhanced.search_link, expected)
+    assert light.search_link == expected
+    assert standard.search_link == expected
+    assert enhanced.search_link == expected
 
 
 def test_self_link():
-    assert_equal(metrics.self_link, None)
+    assert metrics.self_link is None
     expected = 'https://www.scopus.com/authid/detail.uri?partnerID=HzOxMe3b&'\
                'authorId=7004212771&origin=inward'
-    assert_equal(light.self_link, expected)
-    assert_equal(standard.self_link, expected)
-    assert_equal(enhanced.self_link, expected)
+    assert light.self_link == expected
+    assert standard.self_link == expected
+    assert enhanced.self_link == expected
 
 
 def test_status():
-    assert_equal(metrics.status, None)
-    assert_equal(light.status, None)
+    assert metrics.status is None
+    assert light.status is None
     expected = "update"
-    assert_equal(standard.status, expected)
-    assert_equal(enhanced.status, expected)
+    assert standard.status == expected
+    assert enhanced.status == expected
 
 
 def test_subject_areas():
-    assert_equal(metrics.subject_areas, None)
-    assert_equal(light.subject_areas, None)
+    assert metrics.subject_areas is None
+    assert light.subject_areas is None
     expected = "<class 'pybliometrics.scopus.author_retrieval.Subjectarea'>"
     for a in (standard, enhanced):
         received = a.subject_areas
-        assert_true(isinstance(received, list))
-        assert_true(len(received) > 0)
-        assert_equal(str(type(received[0])), expected)
+        assert isinstance(received, list)
+        assert len(received) > 0
+        assert str(type(received[0])) == expected
 
 
 def test_surname():
-    assert_equal(metrics.surname, None)
-    assert_equal(light.surname, None)
-    assert_equal(standard.surname, 'Kitchin')
-    assert_equal(enhanced.surname, 'Kitchin')
+    assert metrics.surname is None
+    assert light.surname is None
+    assert standard.surname, 'Kitchin'
+    assert enhanced.surname, 'Kitchin'
 
 
 def test_url():
     expected = 'http://api.elsevier.com/content/author/author_id/7004212771'
-    assert_equal(metrics.url, expected)
-    assert_equal(light.url, expected)
-    assert_equal(standard.url, expected)
-    assert_equal(enhanced.url, expected)
-
-
-def test_warning_without_forwarding():
-    with warnings.catch_warnings(record=True) as w:
-        au = AuthorRetrieval("24079538400", refresh=False)
-        assert_equal(len(w), 1)
-        assert_true(issubclass(w[-1].category, UserWarning))
-        assert_true("24079538400" in str(w[-1].message))
-
-
-def test_warning_with_forwarding():
-    au = AuthorRetrieval("57191449583", refresh=False)
-    with warnings.catch_warnings(record=True) as w:
-        auth_id = au.identifier
-        assert_equal(len(w), 1)
-        assert_true(issubclass(w[-1].category, UserWarning))
-        assert_true("57191449583" in str(w[-1].message))
-    assert_equal(auth_id, 36854449200)
+    assert metrics.url == expected
+    assert light.url == expected
+    assert standard.url == expected
+    assert enhanced.url == expected
```

### Comparing `pybliometrics-3.6/pybliometrics/scopus/tests/test_AuthorSearch.py` & `pybliometrics-4.0/pybliometrics/scopus/tests/test_AuthorSearch.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,35 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
 """Tests for `scopus.AuthorSearch` module."""
 
 from collections import namedtuple
-from nose.tools import assert_equal, assert_true
 
-from pybliometrics.scopus import AuthorSearch
+from pybliometrics.scopus import AuthorSearch, init
+
+init()
 
 s1 = AuthorSearch('authlast(selten) and authfirst(reinhard)', refresh=30)
 s2 = AuthorSearch('authlast(selten)', download=False, refresh=True)
 
 
 def test_authors():
-    assert_true(isinstance(s1.authors, list))
-    assert_true(len(s1.authors) >= 2)
+    assert isinstance(s1.authors, list)
+    assert len(s1.authors) >= 2
     order = 'eid orcid surname initials givenname affiliation documents '\
             'affiliation_id city country areas'
     Author = namedtuple('Author', order)
     expected = Author(eid='9-s2.0-6602907525', orcid=None, surname='Selten',
         initials='R.', givenname='Reinhard', affiliation='Universität Bonn',
         documents=74, affiliation_id='60007493', city='Bonn',
         country='Germany', areas='ECON (76); MATH (21); BUSI (16)')
-    assert_equal(s1.authors[0], expected)
+    assert s1.authors[0] == expected
 
 
 def test_authors_nodownload():
     # Only works if query hasn't been cached
-    assert_equal(s2.authors, None)
+    assert s2.authors is None
 
 
 def test_results_size():
     received1 = s1.get_results_size()
-    assert_true(received1 >= 1)
+    assert received1 >= 1
     received2 = s2.get_results_size()
-    assert_true(received2 >= 25)
+    assert received2 >= 25
```

### Comparing `pybliometrics-3.6/pybliometrics/scopus/tests/test_PlumXMetrics.py` & `pybliometrics-4.0/pybliometrics/scopus/tests/test_PlumXMetrics.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
 """Tests for `scopus.PlumXMetrics` module."""
 
-from nose.tools import assert_equal, assert_true
+from pybliometrics.scopus import PlumXMetrics, init
 
-from pybliometrics.scopus import PlumXMetrics
+init()
 
 # A published paper. All PlumX Metrics categories are present.
 m1 = PlumXMetrics('2-s2.0-85054706190', 'elsevierId', refresh=30)
 # A published paper. No Usage and Social Media metrics.
 m2 = PlumXMetrics('10.2307/2281868', 'doi', refresh=30)
 # A published paper. No PlumX Metrics.
 m3 = PlumXMetrics('2-s2.0-84950369844', 'elsevierId', refresh=30)
@@ -17,86 +15,85 @@
 # A SSRN paper. No mention metrics.
 m5 = PlumXMetrics('3320470', 'ssrnId', refresh=30)
 
 
 def test_category_totals():
     m1_received = sorted([c.name  for c in m1.category_totals])
     m1_expected = ['capture', 'citation', 'mention', 'socialMedia']
-    assert_equal(m1_received, m1_expected)
+    assert m1_received == m1_expected
     m2_received = sorted([c.name  for c in m2.category_totals])
     m2_expected = ['capture', 'citation', 'mention']
-    assert_equal(m2_received, m2_expected)
-    assert_equal(m3.category_totals, None)
+    assert m2_received == m2_expected
+    assert m3.category_totals is None
     m5_received = sorted([c.name  for c in m5.category_totals])
     m5_expected = ['capture', 'citation', 'socialMedia', 'usage']
-    assert_equal(m5_received, m5_expected)
+    assert m5_received == m5_expected
     for plumx in (m1, m2, m4, m5):
         m_fields = set(field for ntup in plumx.category_totals for
                        field in ntup._fields)
-        assert_equal(m_fields, {'name', 'total'})
+        assert m_fields, {'name', 'total'}
         zero_totals = [i.total for i in plumx.category_totals if i.total <= 0]
-        assert_equal(zero_totals, [])
+        assert zero_totals == []
 
 
 def test_capture():
-    assert_equal(m3.capture, None)
+    assert m3.capture is None
     expected = {'name', 'total'}
     for plumx in (m1, m2, m4, m5):
-        assert_true(isinstance(plumx.capture, list))
-        assert_true(len(plumx.capture) > 0)
+        assert isinstance(plumx.capture, list)
+        assert len(plumx.capture) > 0
         m_fields = set(field for ntup in plumx.capture for field in ntup._fields)
-        assert_equal(m_fields, expected)
+        assert m_fields == expected
         zero_totals = [i.total for i in plumx.capture if i.total <= 0] 
-        assert_equal(zero_totals, [])
+        assert zero_totals == []
 
 
 def test_citation():
-    assert_equal(m3.citation, None)
+    assert m3.citation is None
     expected = {'name', 'total'}
     for plumx in (m1, m2, m4, m5):
-        assert_true(isinstance(plumx.citation, list))
-        assert_true(len(plumx.citation) > 0)
+        assert isinstance(plumx.citation, list)
+        assert len(plumx.citation) > 0
         m_fields = set(field for ntup in plumx.citation for field in ntup._fields)
-        assert_equal(m_fields, expected)
+        assert m_fields == expected
         zero_totals = [i.total for i in plumx.citation if i.total <= 0]
-        assert_equal(zero_totals, [])
+        assert zero_totals == []
 
 
 def test_mention():
-    assert_equal(m3.mention, None)
-    assert_equal(m5.mention, None)
+    assert m3.mention is None
+    assert m5.mention is None
     expected = {'name', 'total'}
     for plumx in (m1, m2, m4):
         print(plumx)
-        assert_true(isinstance(plumx.mention, list))
-        assert_true(len(plumx.mention) > 0)
+        assert isinstance(plumx.mention, list)
+        assert len(plumx.mention) > 0
         m_fields = set(field for ntup in plumx.mention for field in ntup._fields)
-        assert_equal(m_fields, expected)
+        assert m_fields == expected
         zero_totals = [i.total for i in plumx.mention if i.total <= 0]
-        assert_equal(zero_totals, [])
+        assert zero_totals == []
 
 
 def test_social_media():
-    assert_equal(m2.social_media, None)
-    assert_equal(m3.social_media, None)
-    assert_equal(m4.social_media, None)
+    assert m2.social_media is None
+    assert m3.social_media is None
+    assert m4.social_media is None
     expected = {'name', 'total'}
     for plumx in (m1, m5):
-        assert_true(isinstance(plumx.social_media, list))
-        assert_true(len(plumx.social_media) > 0)
+        assert isinstance(plumx.social_media, list)
+        assert len(plumx.social_media) > 0
         m_fields = set(field for ntup in plumx.social_media for field in ntup._fields)
-        assert_equal(m_fields, expected)
+        assert m_fields == expected
         zero_totals = [i.total for i in plumx.social_media if i.total <= 0]
-        assert_equal(zero_totals, [])
+        assert zero_totals == []
 
 
 def test_usage():
-    assert_equal(m2.usage, None)
-    assert_equal(m3.usage, None)
-    expected = {'name', 'total'}
-    for plumx in (m4, m5):
-        assert_true(isinstance(plumx.usage, list))
-        assert_true(len(plumx.usage) > 0)
-        m_fields = set(field for ntup in plumx.usage for field in ntup._fields)
-        assert_equal(m_fields, expected)
-        zero_totals = [i.total for i in plumx.usage if i.total <= 0]
-        assert_equal(zero_totals, [])
+    assert m2.usage is None
+    assert m3.usage is None
+    assert m4.usage is None
+    assert isinstance(m5.usage, list)
+    assert len(m5.usage) > 0
+    m_fields = set(field for ntup in m5.usage for field in ntup._fields)
+    assert m_fields == {'name', 'total'}
+    zero_totals = [i.total for i in m5.usage if i.total <= 0]
+    assert zero_totals == []
```

### Comparing `pybliometrics-3.6/pybliometrics/scopus/tests/test_ScopusSearch.py` & `pybliometrics-4.0/pybliometrics/scopus/tests/test_ScopusSearch.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
 """Tests for `scopus.ScopusSearch` module."""
 
 from collections import namedtuple
 
-from nose.tools import assert_equal, assert_true
+from pybliometrics.scopus import ScopusSearch, init
 
-from pybliometrics.scopus import ScopusSearch
+init()
 
 order = 'eid doi pii pubmed_id title subtype subtypeDescription creator '\
         'afid affilname  affiliation_city affiliation_country author_count '\
         'author_names author_ids author_afids coverDate coverDisplayDate '\
         'publicationName issn source_id eIssn aggregationType volume '\
         'issueIdentifier article_number pageRange description authkeywords '\
         'citedby_count openaccess freetoread freetoreadLabel fund_acr '\
@@ -22,25 +20,25 @@
 s_j = ScopusSearch('SOURCE-ID(22900) AND PUBYEAR IS 2010', refresh=30)
 q_empty = 'SOURCE-ID(19700188323) AND PUBYEAR IS 1900'
 s_empty = ScopusSearch(q_empty, refresh=30)
 
 
 def test_get_eids_author():
     expected = ['2-s2.0-85117005558', '2-s2.0-84937325266', '2-s2.0-26444452434']
-    assert_equal(s_au.get_eids(), expected)
+    assert s_au.get_eids() == expected
 
 
 def test_get_eids_journal():
-    assert_equal(len(s_j.get_eids()), 118)
+    assert len(s_j.get_eids()) == 118
 
 
 def test_get_results_size():
-    assert_equal(s_au.get_results_size(), 3)
-    assert_equal(s_j.get_results_size(), 118)
-    assert_equal(s_empty.get_results_size(), 0)
+    assert s_au.get_results_size() == 3
+    assert s_j.get_results_size() == 118
+    assert s_empty.get_results_size() == 0
 
 
 def test_results_author():
     received = s_au.results[-1]
     expected = doc(eid='2-s2.0-26444452434', doi='10.1016/0014-2921(92)90085-B',
         pii='001429219290085B', pubmed_id=None,
         title='Economists as policymakers: A round-table discussion. Introduction',
@@ -50,16 +48,16 @@
         author_afids=None, coverDate='1992-01-01', coverDisplayDate='April 1992',
         publicationName='European Economic Review', issn='00142921',
         source_id='20749', eIssn=None, aggregationType='Journal', volume='36',
         issueIdentifier='2-3', article_number=None, pageRange='307-309',
         description=None, authkeywords=None, citedby_count=0, openaccess=0,
         freetoread=None, freetoreadLabel=None, fund_acr=None,
         fund_no='undefined', fund_sponsor=None)
-    assert_true(int(received.citedby_count) > 0)
-    assert_equal(received._replace(citedby_count=0), expected)
+    assert int(received.citedby_count) > 0
+    assert received._replace(citedby_count=0) == expected
 
 
 def test_results_journal():
     received = s_j.results[-1]
     abstract = 'This paper investigates the determinants of R&D investment '\
         'at the national level with an emphasis on the roles of patent '\
         'rights protection, international technology transfer through trade '\
@@ -88,13 +86,13 @@
         coverDate='2010-01-01', coverDisplayDate='2010',
         publicationName='Research Policy', issn='00487333', source_id='22900',
         eIssn=None, aggregationType='Journal', volume='39', issueIdentifier='1',
         article_number=None, pageRange='103-116', description=abstract,
         authkeywords=keywords, citedby_count=0, openaccess=0, freetoread=None,
         freetoreadLabel=None, fund_acr='MOST', fund_no='NSC94-2415-H-194-001',
         fund_sponsor='Ministry of Science and Technology, Taiwan')
-    assert_true(int(received.citedby_count) > 60)
-    assert_equal(received._replace(citedby_count=0), expected)
+    assert int(received.citedby_count) > 60
+    assert received._replace(citedby_count=0) == expected
 
 
 def test_results_empty():
-    assert_equal(s_empty.results, None)
+    assert s_empty.results is None
```

### Comparing `pybliometrics-3.6/pybliometrics/scopus/tests/test_SerialSearch.py` & `pybliometrics-4.0/pybliometrics/scopus/tests/test_SerialSearch.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
 """Tests for `scopus.SerialSearch` module."""
 
-from nose.tools import assert_equal, assert_true
+from pybliometrics.scopus import SerialSearch, init
 
-from pybliometrics.scopus import SerialSearch
+init()
 
 
 # Search by title
 ser1 = SerialSearch({'title': 'SoftwareX'}, refresh=30)
 # Search by ISSN
 ser2 = SerialSearch({'issn': '1468-0262'}, refresh=30)
 # Search by publisher
@@ -16,29 +14,29 @@
 # Search by subject abbreviation
 ser4 = SerialSearch({'subj': 'COMP'}, refresh=30)
 # Search by subject area code
 ser5 = SerialSearch({'subjCode': '2612'}, refresh=30)
 
 
 def test_results_title():
-    assert_equal(len(ser1.results), 1)
-    assert_equal(ser1.results[0]['title'], 'SoftwareX')
+    assert len(ser1.results) == 1
+    assert ser1.results[0]['title'] == 'SoftwareX'
 
 
 def test_results_issn():
-    assert_equal(len(ser2.results), 1)
-    assert_equal(ser2.results[0]['title'], 'Econometrica')
+    assert len(ser2.results) == 1
+    assert ser2.results[0]['title'] == 'Econometrica'
 
 
 def test_results_pub():
-    assert_equal(len(ser3.results), 5)
-    assert_equal(ser3.results[0]['title'], 'African Finance Journal')
+    assert len(ser3.results) == 5
+    assert ser3.results[0]['title'] == 'African Finance Journal'
 
 
 def test_results_subj():
     ser4_subj_abbs = set(i['subject_area_abbrevs'] for i in ser4.results)
-    assert_true(False not in ['COMP' in i for i in ser4_subj_abbs])
+    assert False not in ['COMP' in i for i in ser4_subj_abbs]
 
 
 def test_results_subjcode():
     ser5_subj_codes = set(i['subject_area_codes'] for i in ser5.results)
-    assert_true(False not in ['2612' in i for i in ser5_subj_codes])
+    assert False not in ['2612' in i for i in ser5_subj_codes]
```

### Comparing `pybliometrics-3.6/pybliometrics/scopus/tests/test_SerialTitle.py` & `pybliometrics-4.0/pybliometrics/scopus/tests/test_SerialTitle.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,160 +1,159 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
 """Tests for `scopus.SerialTitle` module."""
 
 import datetime
 
 from collections import namedtuple
-from nose.tools import assert_equal, assert_true
 
-from pybliometrics.scopus import SerialTitle
+from pybliometrics.scopus import SerialTitle, init
+
+init()
 
 
 # SoftwareX
 # softwarex = SerialTitle("2352-7110", refresh=30, years="2019-2020")
 softwarex = SerialTitle("2352-7110", refresh=30)
 # OECD Economic Studies
 oecd = SerialTitle("0255-0822", refresh=30)
 # Neural Networks
-neural_networks = SerialTitle('1879-2782', view='CITESCORE')
+neural_networks = SerialTitle('1879-2782', view='CITESCORE', refresh=30)
 
 
 def test_aggregation_type():
-    assert_equal(softwarex.aggregation_type, "journal")
-    assert_equal(oecd.aggregation_type, "journal")
+    assert softwarex.aggregation_type == "journal"
+    assert oecd.aggregation_type == "journal"
 
 
 def test_citescoreyearinfolist():
     info_fields = 'year citescore'
     info = namedtuple('Citescoreinfolist', info_fields)
 
     # Test softwarex
     expected_named_tuple = [info(year=2022, citescore=5.1),
-                            info(year=2023, citescore=4.9)]
-    assert_equal(softwarex.citescoreyearinfolist, expected_named_tuple)
+                            info(year=2023, citescore=5.3)]
+    assert softwarex.citescoreyearinfolist == expected_named_tuple
 
     # Test oecd
-    assert_equal(oecd.citescoreyearinfolist[0], None)
-    assert_equal(oecd.citescoreyearinfolist[1], None)
+    assert oecd.citescoreyearinfolist[0] is None
+    assert oecd.citescoreyearinfolist[1] is None
 
     # Test CITESCORE view
     this_year = datetime.date.today().year
-    assert_equal(neural_networks.citescoreyearinfolist[0].year, this_year)
-    assert_true(type(neural_networks.citescoreyearinfolist[3].citationcount) is int)
+    assert neural_networks.citescoreyearinfolist[0].year == this_year
+    assert isinstance(neural_networks.citescoreyearinfolist[3].citationcount, int)
 
 
 def test_eissn():
-    assert_equal(softwarex.eissn, "2352-7110")
-    assert_equal(oecd.eissn, "1609-7491")
+    assert softwarex.eissn == "2352-7110"
+    assert oecd.eissn == "1609-7491"
 
 
 def test_issn():
-    assert_equal(softwarex.issn, None)
-    assert_equal(oecd.issn, "0255-0822")
+    assert softwarex.issn is None
+    assert oecd.issn == "0255-0822"
 
 
 def test_oaallowsauthorpaid():
-    assert_equal(softwarex.oaallowsauthorpaid, None)
-    assert_equal(oecd.oaallowsauthorpaid, None)
+    assert softwarex.oaallowsauthorpaid is None
+    assert oecd.oaallowsauthorpaid is None
 
 
 def test_openaccess():
-    assert_equal(softwarex.openaccess, 1)
-    assert_equal(oecd.openaccess, None)
+    assert softwarex.openaccess == 1
+    assert oecd.openaccess is None
 
 
 def test_openaccessstartdate():
-    assert_equal(softwarex.openaccessstartdate, None)
-    assert_equal(oecd.openaccessstartdate, None)
+    assert softwarex.openaccessstartdate is None
+    assert oecd.openaccessstartdate is None
 
 
 def test_openaccesstype():
-    assert_equal(softwarex.openaccesstype, None)
-    assert_equal(oecd.openaccesstype, None)
+    assert softwarex.openaccesstype is None
+    assert oecd.openaccesstype is None
 
 
 def test_openaccessarticle():
-    assert_equal(softwarex.openaccessarticle, True)
-    assert_equal(oecd.openaccessarticle, None)
+    assert softwarex.openaccessarticle == True
+    assert oecd.openaccessarticle is None
 
 
 def test_openarchivearticle():
-    assert_equal(softwarex.openarchivearticle, None)
-    assert_equal(oecd.openarchivearticle, None)
+    assert softwarex.openarchivearticle is None
+    assert oecd.openarchivearticle is None
 
 
 def test_openaccesssponsorname():
-    assert_equal(softwarex.openaccesssponsorname, None)
-    assert_equal(oecd.openaccesssponsorname, None)
+    assert softwarex.openaccesssponsorname is None
+    assert oecd.openaccesssponsorname is None
 
 
 def test_openaccessuserlicense():
-    assert_equal(softwarex.openaccessuserlicense, None)
-    assert_equal(oecd.openaccessuserlicense, None)
+    assert softwarex.openaccessuserlicense is None
+    assert oecd.openaccessuserlicense is None
 
 
 def test_publisher():
-    assert_equal(softwarex.publisher, "Elsevier BV")
-    assert_equal(oecd.publisher, "OECD")
+    assert softwarex.publisher == "Elsevier B.V."
+    assert oecd.publisher == "OECD"
 
 
 def test_scopus_source_link():
     expected1 = "https://www.scopus.com/source/sourceInfo.url?sourceId=21100422153"
-    assert_equal(softwarex.scopus_source_link, expected1)
+    assert softwarex.scopus_source_link == expected1
     expected2 = "https://www.scopus.com/source/sourceInfo.url?sourceId=24107"
-    assert_equal(oecd.scopus_source_link, expected2)
+    assert oecd.scopus_source_link == expected2
 
 
 def test_self_link():
     expected1 = "https://api.elsevier.com/content/serial/title/issn/23527110"
-    assert_equal(softwarex.self_link, expected1)
+    assert softwarex.self_link == expected1
     expected2 = "https://api.elsevier.com/content/serial/title/issn/02550822"
-    assert_equal(oecd.self_link, expected2)
+    assert oecd.self_link == expected2
 
 
 def test_sjrlist():
-    assert_equal(softwarex.sjrlist, [(2022, 0.574)])
-    assert_equal(oecd.sjrlist, [(1999, 2.723)])
+    assert softwarex.sjrlist == [(2022, 0.574)]
+    assert oecd.sjrlist == [(1999, 2.723)]
 
 
 def test_sniplist():
-    assert_equal(softwarex.sniplist, [(2022, 1.426)])
-    assert_equal(oecd.sniplist, None)
+    assert softwarex.sniplist == [(2022, 1.426)]
+    assert oecd.sniplist is None
 
 
 def test_source_id():
-    assert_equal(softwarex.source_id, 21100422153)
-    assert_equal(oecd.source_id, 24107)
+    assert softwarex.source_id == 21100422153
+    assert oecd.source_id == 24107
 
 
 def test_subject_area():
     area = namedtuple('Subjectarea', 'area abbreviation code')
     expected1 = [
         area(area='Software', abbreviation='COMP', code=1712),
         area(area='Computer Science Applications', abbreviation='COMP', code=1706)
     ]
-    assert_equal(softwarex.subject_area, expected1)
+    assert softwarex.subject_area == expected1
     expected2 = [
         area(area='Geography, Planning and Development', abbreviation='SOCI', code=3305)
     ]
-    assert_equal(oecd.subject_area, expected2)
+    assert oecd.subject_area == expected2
 
 
 def test_title():
-    assert_equal(softwarex.title, "SoftwareX")
-    assert_equal(oecd.title, "OECD Economic Studies")
+    assert softwarex.title == "SoftwareX"
+    assert oecd.title == "OECD Economic Studies"
 
 
 def test_yearly_data():
-    assert_true(type(softwarex.yearly_data) == list)
-    assert_equal(len(softwarex.yearly_data), 28)
+    assert isinstance(softwarex.yearly_data, list)
+    assert len(softwarex.yearly_data) == 29
     fields = 'year publicationcount revpercent zerocitessce '\
              'zerocitespercentsce citecountsce'
     dat = namedtuple('Yearlydata', fields)
     expected1_2020 = dat(year=2020, publicationcount=164, revpercent=0.0,
-        zerocitessce=10, zerocitespercentsce=6.097560975609756,
-        citecountsce=2571)
-    assert_equal(softwarex.yearly_data[24], expected1_2020)
+        zerocitessce=9, zerocitespercentsce=5.487804878048781,
+        citecountsce=2570)
+    assert softwarex.yearly_data[24] == expected1_2020
     expected2_1996 = dat(year=1996, publicationcount=4, revpercent=0.0,
         zerocitessce=0, zerocitespercentsce=0, citecountsce=33)
-    assert_equal(oecd.yearly_data[0], expected2_1996)
+    assert oecd.yearly_data[0] == expected2_1996
```

### Comparing `pybliometrics-3.6/pybliometrics/scopus/tests/test_SubjectClassifications.py` & `pybliometrics-4.0/pybliometrics/scopus/tests/test_SubjectClassifications.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
 """Tests for `scopus.SubjectClassifications` module."""
 
-from nose.tools import assert_equal, assert_true
+from pybliometrics.scopus import SubjectClassifications, init
 
-from pybliometrics.scopus import SubjectClassifications
+init()
 
 
 # Search by words in subject description
 sub1 = SubjectClassifications({'description': 'Physics'}, refresh=30)
 # Search by subject code
 sub2 = SubjectClassifications({'code': '2613'}, refresh=30)
 # Search by words in subject detail
@@ -19,37 +17,37 @@
 sub5 = SubjectClassifications({'description': 'Engineering', 'detail': 'Fluid'}, refresh=30)
 # Search by multiple criteria, subset returned fields
 sub6 = SubjectClassifications({'detail': 'Analysis', 'description': 'Mathematics'},
                               fields=['description', 'detail'], refresh=30)
 
 
 def test_results_desc():
-    assert_true(len(sub1.results) > 0)
-    assert_true(all(['Physics' in res.description for res in sub1.results]))
+    assert len(sub1.results) > 0
+    assert all(['Physics' in res.description for res in sub1.results])
 
 
 def test_results_code():
-    assert_equal(len(sub2.results), 1)
-    assert_equal(sub2.results[0].code, '2613')
+    assert len(sub2.results) == 1
+    assert sub2.results[0].code == '2613'
     
 
 def test_results_detail():
-    assert_true(len(sub3.results) > 0)
-    assert_true(all(['Processes' in res.detail for res in sub3.results]))
+    assert len(sub3.results) > 0
+    assert all(['Processes' in res.detail for res in sub3.results])
 
 
 def test_results_abbrev():
-    assert_true(len(sub4.results) > 0)
-    assert_true(all(['MATH' in res.abbrev for res in sub4.results]))
+    assert len(sub4.results) > 0
+    assert all(['MATH' in res.abbrev for res in sub4.results])
 
 
 def test_results_multi():
-    assert_true(len(sub5.results) > 0)
-    assert_true(all(['Engineering' in res.description for res in sub5.results]))
-    assert_true(all(['Fluid' in res.detail for res in sub5.results]))
+    assert len(sub5.results) > 0
+    assert all(['Engineering' in res.description for res in sub5.results])
+    assert all(['Fluid' in res.detail for res in sub5.results])
     
 
 def test_results_fields():
-    assert_true(len(sub6.results) > 0)
-    assert_true(all(['Mathematics' in res.description for res in sub6.results]))
-    assert_true(all(['Analysis' in res.detail for res in sub6.results]))
-    assert_true(all([set(res._fields) == set(['description', 'detail']) for res in sub6.results]))
+    assert len(sub6.results) > 0
+    assert all(['Mathematics' in res.description for res in sub6.results])
+    assert all(['Analysis' in res.detail for res in sub6.results])
+    assert all([set(res._fields) == set(['description', 'detail']) for res in sub6.results])
```

### Comparing `pybliometrics-3.6/pybliometrics/scopus/utils/constants.py` & `pybliometrics-4.0/pybliometrics/scopus/utils/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,14 +46,29 @@
     'ScopusSearch': SEARCH_BASE + 'scopus',
     'SerialSearch': RETRIEVAL_BASE + 'serial/title',
     'SerialTitle': RETRIEVAL_BASE + 'serial/title/issn/',
     'SubjectClassifications': RETRIEVAL_BASE + 'subject/scopus',
     'PlumXMetrics': 'https://api.elsevier.com/analytics/plumx/'
 }
 
+# Valid views for all classes
+VIEWS = {
+    "CitationOverview": ["STANDARD"],
+    "AbstractRetrieval": ["META", "META_ABS", "FULL", "REF", "ENTITLED"],
+    "AffiliationRetrieval": ["LIGHT", "STANDARD", "ENTITLED"],
+    "AffiliationSearch": ["STANDARD"],
+    "AuthorRetrieval": ["LIGHT", "STANDARD", "ENHANCED", "METRICS", "ENTITLED"],
+    "AuthorSearch": ["STANDARD"],
+    "PlumXMetrics": ["ENHANCED"],
+    "ScopusSearch": ["STANDARD", "COMPLETE"],
+    "SerialSearch": ["STANDARD", "ENHANCED", "CITESCORE"],
+    "SerialTitle": ["STANDARD", "ENHANCED", "CITESCORE"],
+    "SubjectClassifications": [''],
+}
+
 # Throttling limits (in queries per second) // 0 = no limit
 RATELIMITS = {
     'AbstractRetrieval': 9,
     'AffiliationRetrieval': 9,
     'AffiliationSearch': 6,
     'AuthorRetrieval': 3,
     'AuthorSearch': 2,
```

### Comparing `pybliometrics-3.6/pybliometrics/scopus/utils/create_config.py` & `pybliometrics-4.0/pybliometrics/scopus/utils/create_config.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 import configparser
 from typing import List, Optional
+from pybliometrics.scopus.utils.constants import CONFIG_FILE
 
 
-def create_config(keys: Optional[List[str]] = None,
+def create_config(config_dir: Optional[str] = None,
+                  keys: Optional[List[str]] = None,
                   insttoken: Optional[str] = None
                   ):
     """Initiates process to generate configuration file.
 
     :param keys: If you provide a list of keys, pybliometrics will skip the
                  prompt.  It will also not ask for InstToken.  This is
                  intended for workflows using CI, not for general use.
     :param insttoken: An InstToken to be used alongside the key(s).  Will only
                       be used if `keys` is not empty.
     """
-    from pybliometrics.scopus.utils.constants import CONFIG_FILE, DEFAULT_PATHS
+    from pybliometrics.scopus.utils.constants import DEFAULT_PATHS
+
+    if not config_dir:
+        config_dir = CONFIG_FILE
 
     config = configparser.ConfigParser()
     config.optionxform = str
-    print(f"Creating config file at {CONFIG_FILE} with default paths...")
+    print(f"Creating config file at {config_dir} with default paths...")
 
     # Set directories
     config.add_section('Directories')
     for api, path in DEFAULT_PATHS.items():
         config.set('Directories', api, str(path))
 
     # Set authentication
@@ -46,13 +51,13 @@
 
     # Set default values
     config.add_section('Requests')
     config.set('Requests', 'Timeout', '20')
     config.set('Requests', 'Retries', '5')
 
     # Write out
-    CONFIG_FILE.parent.mkdir(parents=True, exist_ok=True)
-    with open(CONFIG_FILE, "w") as ouf:
+    config_dir.parent.mkdir(parents=True, exist_ok=True)
+    with open(config_dir, "w") as ouf:
         config.write(ouf)
-    print(f"Configuration file successfully created at {CONFIG_FILE}\n"
+    print(f"Configuration file successfully created at {config_dir}\n"
           "For details see https://pybliometrics.rtfd.io/en/stable/configuration.html.")
     return config
```

### Comparing `pybliometrics-3.6/pybliometrics/scopus/utils/get_content.py` & `pybliometrics-4.0/pybliometrics/scopus/utils/get_content.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,37 @@
+from typing import Type
 from requests import Session
 from requests.adapters import HTTPAdapter
 from urllib3.util import Retry
 
 from pybliometrics import __version__
 from pybliometrics.scopus import exception
-from pybliometrics.scopus.utils.startup import config
+from pybliometrics.scopus.utils.startup import get_config, get_keys, _throttling_params
 
 # Define user agent string for HTTP requests
 user_agent = 'pybliometrics-v' + __version__
 
 errors = {400: exception.Scopus400Error, 401: exception.Scopus401Error,
           403: exception.Scopus403Error, 404: exception.Scopus404Error,
           407: exception.Scopus407Error, 413: exception.Scopus413Error, 
           414: exception.Scopus414Error, 429: exception.Scopus429Error}
 
-_retries = config.getint("Requests", "Retries", fallback=5)
-retry = Retry(total=_retries, status_forcelist=[500, 501, 502, 503, 504, 524],
-              backoff_factor=0.1)
-adapter = HTTPAdapter(max_retries=retry)
-session = Session()
-session.mount('http://', adapter)
-session.mount('https://', adapter)
+def get_session() -> Type[Session]:
+    """Auxiliary function to create a session"""
+    config = get_config()
+
+    _retries = config.getint("Requests", "Retries", fallback=5)
+    retry = Retry(total=_retries, backoff_factor=0.1,
+                  status_forcelist=[500, 501, 502, 503, 504, 524])
+    adapter = HTTPAdapter(max_retries=retry)
+    session = Session()
+    session.mount('http://', adapter)
+    session.mount('https://', adapter)
+    return session
+
 
 def get_content(url, api, params=None, **kwds):
     """Helper function to download a file and return its content.
 
     Parameters
     ----------
     url : str
@@ -54,19 +61,21 @@
     -------
     resp : byte-like object
         The content of the file, which needs to be serialized.
     """
     from random import shuffle
     from time import sleep, time
 
-    from pybliometrics.scopus.utils.startup import _throttling_params, KEYS
+    config = get_config()
+    keys = get_keys()
+    session = get_session()
 
     # Set header, params and proxy
     try:
-        header = {'X-ELS-APIKey': KEYS[0],
+        header = {'X-ELS-APIKey': keys[0],
                   'Accept': 'application/json',
                   'User-Agent': user_agent}
     except IndexError:
         raise errors[429]
 
     if config.has_option('Authentication', 'InstToken'):
         token = config.get('Authentication', 'InstToken')
@@ -83,24 +92,24 @@
 
     # Eventually wait bc of throttling
     if len(_throttling_params[api]) == _throttling_params[api].maxlen:
         try:
             sleep(1 - (time() - _throttling_params[api][0]))
         except (IndexError, ValueError):
             pass
-    
+
     # Perform request, eventually replacing the current key
     timeout = config.getint("Requests", "Timeout", fallback=20)
     resp = session.get(url, headers=header, proxies=proxies, params=params,
                       timeout=timeout)
     while resp.status_code == 429:
         try:
-            KEYS.pop(0)  # Remove current key
-            shuffle(KEYS)
-            header['X-ELS-APIKey'] = KEYS[0].strip()
+            keys.pop(0)  # Remove current key
+            shuffle(keys)
+            header['X-ELS-APIKey'] = keys[0].strip()
             resp = session.get(url, headers=header, proxies=proxies,
                                params=params, timeout=timeout)
         except IndexError:  # All keys depleted
             break
     _throttling_params[api].append(time())
 
     # Eventually raise error, if possible with supplied error message
@@ -150,34 +159,7 @@
             id_type = 'pubmed_id'
         else:
             id_type = 'scopus_id'
     try:
         return id_type
     except UnboundLocalError:
         raise ValueError(f'ID type detection failed for "{sid}".')
-
-
-def get_folder(api, view):
-    """Auxiliary function to get the cache folder belonging to an API,
-    eventually create the folder.
-    """
-    from configparser import NoOptionError
-    from pathlib import Path
-
-    from pybliometrics.scopus.utils import CONFIG_FILE, DEFAULT_PATHS
-    from pybliometrics.scopus.utils.create_config import create_config
-
-    if not config.has_section('Directories'):
-        create_config()
-    try:
-        parent = Path(config.get('Directories', api))
-    except NoOptionError:
-        parent = DEFAULT_PATHS[api]
-        config.set('Directories', api, str(parent))
-        with open(CONFIG_FILE, 'w') as ouf:
-            config.write(ouf)
-    try:
-        folder = parent/view
-    except TypeError:
-        folder = parent
-    folder.mkdir(parents=True, exist_ok=True)
-    return folder
```

### Comparing `pybliometrics-3.6/pybliometrics/scopus/utils/parse_content.py` & `pybliometrics-4.0/pybliometrics/scopus/utils/parse_content.py`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.6/pybliometrics.egg-info/PKG-INFO` & `pybliometrics-4.0/pybliometrics.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,139 +1,144 @@
-Metadata-Version: 2.1
-Name: pybliometrics
-Version: 3.6
-Summary: Python-based API-Wrapper to access Scopus
-Author-email: "'John Kitchin and Michael E. Rose" <Michael.Ernst.Rose@gmail.com>
-Maintainer-email: "Michael E. Rose" <Michael.Ernst.Rose@gmail.com>
-License: MIT
-Project-URL: Homepage, https://github.com/pybliometrics-dev/pybliometrics
-Project-URL: Bug Tracker, https://github.com/pybliometrics-dev/pybliometrics/issues
-Project-URL: Documentation (stable), https://pybliometrics.readthedocs.io/en/stable/
-Project-URL: Documentation (latest), https://pybliometrics.readthedocs.io/en/latest/
-Keywords: scopus
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: tqdm
-Requires-Dist: urllib3
-
-pybliometrics
-=============
-
-Enables large-scale access to Elsevier's Scopus API from Python.
-
-Documentation: https://pybliometrics.readthedocs.io
-
-Development: https://github.com/pybliometrics-dev/pybliometrics
-
-.. image:: https://badge.fury.io/py/pybliometrics.svg
-    :target: https://badge.fury.io/py/pybliometrics
-
-.. image:: https://img.shields.io/pypi/pyversions/pybliometrics.svg
-    :target: https://img.shields.io/pypi/pyversions/pybliometrics.svg
-
-.. image:: https://readthedocs.org/projects/pybliometrics/badge/?version=stable
-    :target: https://readthedocs.org/projects/pybliometrics/badge/?version=stable
-
-.. image:: https://img.shields.io/pypi/dm/pybliometrics.svg
-    :target: https://img.shields.io/pypi/dm/pybliometrics.svg
-
-.. image:: https://img.shields.io/pypi/l/pybliometrics.svg
-    :target: https://img.shields.io/pypi/l/pybliometrics.svg
-
-.. image:: https://api.codeclimate.com/v1/badges/a4d7edd206a1252dfcfe/maintainability
-   :target: https://codeclimate.com/github/pybliometrics-dev/pybliometrics/maintainability
-
-Example
-=======
-.. example-begin
-.. code:: python
-
-    >>> # Document-specific information
-    >>> from pybliometrics.scopus import AbstractRetrieval
-    >>> ab = AbstractRetrieval("10.1016/j.softx.2019.100263")
-    >>> ab.title
-    'pybliometrics: Scriptable bibliometrics using a Python interface to Scopus'
-    >>> ab.publicationName
-    'SoftwareX'
-    >>> ab.authors
-    [Author(auid=57209617104, indexed_name='Rose M.E.', surname='Rose',
-     given_name='Michael E.', affiliation='60105007'),
-     Author(auid=7004212771, indexed_name='Kitchin J.R.', surname='Kitchin',
-     given_name='John R.', affiliation='60027950')]
-    >>> 
-    >>> # Author-specific information
-    >>> from pybliometrics.scopus import AuthorRetrieval
-    >>> au2 = AuthorRetrieval(ab.authors[1].auid)
-    >>> au2.h_index
-    34
-    >>> au1 = AuthorRetrieval(ab.authors[0].auid)
-    >>> au1.affiliation_current
-    [Affiliation(id=60105007, parent=None, type='parent', relationship='author',
-     afdispname=None, preferred_name='Max Planck Institute for Innovation and Competition',
-     parent_preferred_name=None, country_code='deu', country='Germany',
-     address_part='Marstallplatz 1', city='Munich', state='Bayern',
-     postal_code='80539', org_domain='ip.mpg.de', org_URL='http://www.ip.mpg.de/')]
-    >>> 
-    >>> # Affiliation information
-    >>> from pybliometrics.scopus import AffiliationRetrieval
-    >>> aff1 = AffiliationRetrieval(au1.affiliation_current[0].id)
-    >>> aff1.author_count
-    98
-
-.. example-end
-
-Installation
-============
-
-.. installation-begin
-
-Install the stable version from PyPI:
-
-.. code-block:: bash
-
-    pip install pybliometrics
-
-or the development version from the GitHub repository (requires git on your system):
-
-.. code-block:: bash
-
-    pip install git+https://github.com/pybliometrics-dev/pybliometrics
-
-.. installation-end
-
-Citation
-========
-
-If pybliometrics helped you getting data for research, please cite our corresponding paper:
-
-* Rose, Michael E. and John R. Kitchin: "`pybliometrics: Scriptable bibliometrics using a Python interface to Scopus <./meta/1-s2.0-S2352711019300573-main.pdf>`_", SoftwareX 10 (2019) 100263.
-
-Citing the paper helps the development of pybliometrics, because it justifies funneling resources into the development.  It also signals that you obtained data from Scopus in a transparent and replicable way.
-
-Change log
-==========
-
-Please see `CHANGES.rst <./meta/CHANGES.rst>`_.
-
-Contributing
-============
-
-Please see `CONTRIBUTING.rst <CONTRIBUTING.rst>`_. For a list of contributors see
-`AUTHORS.rst <./meta/AUTHORS.rst>`_.
-
-License
-=======
-
-MIT License; see `LICENSE <LICENSE>`_.
+Metadata-Version: 2.1
+Name: pybliometrics
+Version: 4.0
+Summary: Python-based API-Wrapper to access Scopus
+Author-email: "'John Kitchin and Michael E. Rose" <Michael.Ernst.Rose@gmail.com>
+Maintainer-email: "Michael E. Rose" <Michael.Ernst.Rose@gmail.com>
+License: MIT
+Project-URL: Homepage, https://github.com/pybliometrics-dev/pybliometrics
+Project-URL: Bug Tracker, https://github.com/pybliometrics-dev/pybliometrics/issues
+Project-URL: Documentation (stable), https://pybliometrics.readthedocs.io/en/stable/
+Project-URL: Documentation (latest), https://pybliometrics.readthedocs.io/en/latest/
+Keywords: scopus
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Documentation :: Sphinx
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: tqdm
+Requires-Dist: urllib3
+
+pybliometrics
+=============
+
+Enables large-scale access to Elsevier's Scopus API from Python.
+
+Documentation: https://pybliometrics.readthedocs.io
+
+Development: https://github.com/pybliometrics-dev/pybliometrics
+
+.. image:: https://badge.fury.io/py/pybliometrics.svg
+    :target: https://badge.fury.io/py/pybliometrics
+
+.. image:: https://img.shields.io/pypi/pyversions/pybliometrics.svg
+    :target: https://img.shields.io/pypi/pyversions/pybliometrics.svg
+
+.. image:: https://readthedocs.org/projects/pybliometrics/badge/?version=stable
+    :target: https://readthedocs.org/projects/pybliometrics/badge/?version=stable
+
+.. image:: https://img.shields.io/pypi/dm/pybliometrics.svg
+    :target: https://img.shields.io/pypi/dm/pybliometrics.svg
+
+.. image:: https://img.shields.io/pypi/l/pybliometrics.svg
+    :target: https://img.shields.io/pypi/l/pybliometrics.svg
+
+.. image:: https://api.codeclimate.com/v1/badges/a4d7edd206a1252dfcfe/maintainability
+   :target: https://codeclimate.com/github/pybliometrics-dev/pybliometrics/maintainability
+
+Example
+=======
+.. example-begin
+.. code:: python
+
+    >>> import pybliometrics
+    >>> pybliometrics.init()  # read API keys
+    >>> # Document-specific information
+    >>> from pybliometrics.scopus import AbstractRetrieval
+    >>> ab = AbstractRetrieval("10.1016/j.softx.2019.100263")
+    >>> ab.title
+    'pybliometrics: Scriptable bibliometrics using a Python interface to Scopus'
+    >>> ab.publicationName
+    'SoftwareX'
+    >>> ab.authors
+    [Author(auid=57209617104, indexed_name='Rose M.E.', surname='Rose',
+     given_name='Michael E.', affiliation='60105007'),
+     Author(auid=7004212771, indexed_name='Kitchin J.R.', surname='Kitchin',
+     given_name='John R.', affiliation='60027950')]
+    >>> 
+    >>> # Author-specific information
+    >>> from pybliometrics.scopus import AuthorRetrieval
+    >>> au2 = AuthorRetrieval(ab.authors[1].auid)
+    >>> au2.h_index
+    34
+    >>> au1 = AuthorRetrieval(ab.authors[0].auid)
+    >>> au1.affiliation_current
+    [Affiliation(id=60105007, parent=None, type='parent', relationship='author',
+     afdispname=None, preferred_name='Max Planck Institute for Innovation and Competition',
+     parent_preferred_name=None, country_code='deu', country='Germany',
+     address_part='Marstallplatz 1', city='Munich', state='Bayern',
+     postal_code='80539', org_domain='ip.mpg.de', org_URL='http://www.ip.mpg.de/')]
+    >>> 
+    >>> # Affiliation information
+    >>> from pybliometrics.scopus import AffiliationRetrieval
+    >>> aff1 = AffiliationRetrieval(au1.affiliation_current[0].id)
+    >>> aff1.author_count
+    98
+
+.. example-end
+
+Installation
+============
+
+.. installation-begin
+
+Install the stable version from PyPI:
+
+.. code-block:: bash
+
+    pip install pybliometrics
+
+or the development version from the GitHub repository (requires git on your system):
+
+.. code-block:: bash
+
+    pip install git+https://github.com/pybliometrics-dev/pybliometrics
+
+.. installation-end
+
+Citation
+========
+
+If pybliometrics helped you getting data for research, please cite our corresponding paper:
+
+* Rose, Michael E. and John R. Kitchin: "`pybliometrics: Scriptable bibliometrics using a Python interface to Scopus <./meta/1-s2.0-S2352711019300573-main.pdf>`_", SoftwareX 10 (2019) 100263.
+
+Citing the paper helps the development of pybliometrics, because it justifies funneling resources into the development.  It also signals that you obtained data from Scopus in a transparent and replicable way.
+
+Change log
+==========
+
+Please see `CHANGES.rst <./meta/CHANGES.rst>`_.
+
+Contributing
+============
+
+Please see `CONTRIBUTING.rst <CONTRIBUTING.rst>`_. For a list of contributors see
+`AUTHORS.rst <./meta/AUTHORS.rst>`_.
+
+License
+=======
+
+MIT License; see `LICENSE <LICENSE>`_.
```

### Comparing `pybliometrics-3.6/pybliometrics.egg-info/SOURCES.txt` & `pybliometrics-4.0/pybliometrics.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 .gitignore
 .readthedocs.yaml
+CITATION.cff
 CONTRIBUTING.rst
 LICENSE
 README.rst
 pyproject.toml
 .github/ISSUE_TEMPLATE/bug.md
 .github/ISSUE_TEMPLATE/feature.md
 .github/ISSUE_TEMPLATE/question.md
@@ -16,15 +17,15 @@
 docs/configuration.rst
 docs/contributing.rst
 docs/index.rst
 docs/installation.rst
 docs/make.bat
 docs/requirements.txt
 docs/tips.rst
-docs/_static/custom.css
+docs/_static/custom.css.bak
 docs/access/errors.rst
 docs/access/general.rst
 docs/access/quotas.rst
 docs/classes/AbstractRetrieval.rst
 docs/classes/AffiliationRetrieval.rst
 docs/classes/AffiliationSearch.rst
 docs/classes/AuthorRetrieval.rst
@@ -35,14 +36,15 @@
 docs/classes/SerialSearch.rst
 docs/classes/SerialTitle.rst
 docs/classes/SubjectClassifications.rst
 docs/tips/affiliations.rst
 docs/tips/configuration.rst
 docs/tips/database.rst
 docs/tips/migration1.rst
+docs/tips/migration3.rst
 docs/tips/rename.rst
 docs/tips/support.rst
 meta/1-s2.0-S2352711019300573-main.pdf
 meta/AUTHORS.rst
 meta/CHANGES.rst
 pybliometrics/__init__.py
 pybliometrics.egg-info/PKG-INFO
```

### Comparing `pybliometrics-3.6/pyproject.toml` & `pybliometrics-4.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -13,24 +13,27 @@
     "requests",
     "tqdm",
     "urllib3",
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Science/Research",
+    "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Scientific/Engineering :: Information Analysis",
+    "Topic :: Documentation :: Sphinx"
 ]
 keywords = ["scopus"]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/pybliometrics-dev/pybliometrics"
 "Bug Tracker" = "https://github.com/pybliometrics-dev/pybliometrics/issues"
```

