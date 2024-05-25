# Comparing `tmp/zebrafy-1.1.3.tar.gz` & `tmp/zebrafy-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zebrafy-1.1.3.tar", last modified: Fri May 24 03:18:33 2024, max compression
+gzip compressed data, was "zebrafy-1.1.4.tar", last modified: Sat May 25 05:00:42 2024, max compression
```

## Comparing `zebrafy-1.1.3.tar` & `zebrafy-1.1.4.tar`

### file list

```diff
@@ -1,75 +1,81 @@
-drwxr-xr-x   0 m         (1000) m         (1000)        0 2024-05-24 03:18:33.728341 zebrafy-1.1.3/
--rw-r--r--   0 m         (1000) m         (1000)      230 2023-08-07 02:54:40.000000 zebrafy-1.1.3/.editorconfig
--rw-r--r--   0 m         (1000) m         (1000)       36 2023-08-12 04:33:43.000000 zebrafy-1.1.3/.gitattributes
-drwxr-xr-x   0 m         (1000) m         (1000)        0 2024-05-24 03:18:33.712340 zebrafy-1.1.3/.github/
-drwxr-xr-x   0 m         (1000) m         (1000)        0 2024-05-24 03:18:33.712340 zebrafy-1.1.3/.github/workflows/
--rw-r--r--   0 m         (1000) m         (1000)      843 2024-05-24 03:15:43.000000 zebrafy-1.1.3/.github/workflows/ci.yml
--rw-r--r--   0 m         (1000) m         (1000)     1587 2023-08-16 03:32:25.000000 zebrafy-1.1.3/.gitignore
--rw-r--r--   0 m         (1000) m         (1000)     1165 2024-05-24 03:15:43.000000 zebrafy-1.1.3/.pre-commit-config.yaml
--rw-r--r--   0 m         (1000) m         (1000)      205 2024-05-24 03:15:43.000000 zebrafy-1.1.3/.prettierrc.yml
--rw-r--r--   0 m         (1000) m         (1000)      402 2024-05-24 01:30:45.000000 zebrafy-1.1.3/.pylintrc
--rw-r--r--   0 m         (1000) m         (1000)      730 2024-05-24 03:15:43.000000 zebrafy-1.1.3/.readthedocs.yml
--rw-r--r--   0 m         (1000) m         (1000)     7652 2023-08-06 02:30:03.000000 zebrafy-1.1.3/LICENSE.txt
--rw-r--r--   0 m         (1000) m         (1000)    11657 2024-05-24 03:18:33.728341 zebrafy-1.1.3/PKG-INFO
--rw-r--r--   0 m         (1000) m         (1000)    10083 2024-05-16 06:23:33.000000 zebrafy-1.1.3/README.rst
-drwxr-xr-x   0 m         (1000) m         (1000)        0 2024-05-24 03:18:33.716340 zebrafy-1.1.3/docs/
--rw-r--r--   0 m         (1000) m         (1000)      634 2023-08-15 03:04:59.000000 zebrafy-1.1.3/docs/Makefile
--rw-r--r--   0 m         (1000) m         (1000)     1661 2024-05-24 03:15:43.000000 zebrafy-1.1.3/docs/conf.py
--rw-r--r--   0 m         (1000) m         (1000)      249 2023-08-16 03:34:22.000000 zebrafy-1.1.3/docs/index.rst
--rw-r--r--   0 m         (1000) m         (1000)      765 2023-08-15 05:00:09.000000 zebrafy-1.1.3/docs/make.bat
--rw-r--r--   0 m         (1000) m         (1000)       50 2023-08-16 02:46:29.000000 zebrafy-1.1.3/docs/modules.rst
--rw-r--r--   0 m         (1000) m         (1000)       70 2024-05-24 03:15:43.000000 zebrafy-1.1.3/docs/requirements.in
--rw-r--r--   0 m         (1000) m         (1000)     1433 2024-05-24 03:15:43.000000 zebrafy-1.1.3/docs/requirements.txt
--rw-r--r--   0 m         (1000) m         (1000)     7859 2024-05-16 06:02:35.000000 zebrafy-1.1.3/docs/usage.rst
--rw-r--r--   0 m         (1000) m         (1000)     5962 2023-08-17 03:01:04.000000 zebrafy-1.1.3/docs/zebrafy-64.png
--rw-r--r--   0 m         (1000) m         (1000)   483090 2023-08-17 02:56:09.000000 zebrafy-1.1.3/docs/zebrafy-long.png
--rw-r--r--   0 m         (1000) m         (1000)   333682 2023-08-17 02:56:10.000000 zebrafy-1.1.3/docs/zebrafy.png
--rw-r--r--   0 m         (1000) m         (1000)      763 2023-08-17 02:19:44.000000 zebrafy-1.1.3/docs/zebrafy.rst
--rw-r--r--   0 m         (1000) m         (1000)     1826 2024-05-24 03:15:43.000000 zebrafy-1.1.3/pyproject.toml
--rw-r--r--   0 m         (1000) m         (1000)       38 2024-05-24 03:18:33.728341 zebrafy-1.1.3/setup.cfg
-drwxr-xr-x   0 m         (1000) m         (1000)        0 2024-05-24 03:18:33.716340 zebrafy-1.1.3/tests/
--rw-r--r--   0 m         (1000) m         (1000)       28 2024-05-24 03:15:43.000000 zebrafy-1.1.3/tests/__init__.py
-drwxr-xr-x   0 m         (1000) m         (1000)        0 2024-05-24 03:18:33.724341 zebrafy-1.1.3/tests/static/
--rw-r--r--   0 m         (1000) m         (1000)   261566 2023-08-12 23:38:59.000000 zebrafy-1.1.3/tests/static/test_image.png
--rw-r--r--   0 m         (1000) m         (1000)   108008 2024-03-24 00:36:09.000000 zebrafy-1.1.3/tests/static/test_image_ascii.png
--rw-r--r--   0 m         (1000) m         (1000)   409641 2024-03-24 00:36:09.000000 zebrafy-1.1.3/tests/static/test_image_ascii.zpl
--rw-r--r--   0 m         (1000) m         (1000)   108008 2024-03-24 00:36:09.000000 zebrafy-1.1.3/tests/static/test_image_b64.png
--rw-r--r--   0 m         (1000) m         (1000)   273119 2024-03-24 00:36:09.000000 zebrafy-1.1.3/tests/static/test_image_b64.zpl
--rw-r--r--   0 m         (1000) m         (1000)   409631 2023-08-12 03:28:58.000000 zebrafy-1.1.3/tests/static/test_image_broken.zpl
--rw-r--r--   0 m         (1000) m         (1000)   409641 2023-08-14 03:06:34.000000 zebrafy-1.1.3/tests/static/test_image_high_threshold.zpl
--rw-r--r--   0 m         (1000) m         (1000)   409641 2023-08-17 01:54:05.000000 zebrafy-1.1.3/tests/static/test_image_invert.zpl
--rw-r--r--   0 m         (1000) m         (1000)   409641 2023-08-17 01:54:05.000000 zebrafy-1.1.3/tests/static/test_image_invert_no_dither.zpl
--rw-r--r--   0 m         (1000) m         (1000)   409641 2023-08-14 03:06:34.000000 zebrafy-1.1.3/tests/static/test_image_low_threshold.zpl
--rw-r--r--   0 m         (1000) m         (1000)   819274 2023-08-14 03:27:47.000000 zebrafy-1.1.3/tests/static/test_image_multiple.zpl
--rw-r--r--   0 m         (1000) m         (1000)   409641 2023-08-14 03:06:34.000000 zebrafy-1.1.3/tests/static/test_image_no_dither.zpl
--rw-r--r--   0 m         (1000) m         (1000)   409645 2023-08-17 01:56:19.000000 zebrafy-1.1.3/tests/static/test_image_pos_x_pos_y.zpl
--rw-r--r--   0 m         (1000) m         (1000)   409641 2024-05-16 06:02:35.000000 zebrafy-1.1.3/tests/static/test_image_rotation.zpl
--rw-r--r--   0 m         (1000) m         (1000)    63038 2023-08-14 03:06:34.000000 zebrafy-1.1.3/tests/static/test_image_width_height.zpl
--rw-r--r--   0 m         (1000) m         (1000)   108008 2024-03-24 00:36:09.000000 zebrafy-1.1.3/tests/static/test_image_z64.png
--rw-r--r--   0 m         (1000) m         (1000)   118567 2024-03-24 00:36:09.000000 zebrafy-1.1.3/tests/static/test_image_z64.zpl
--rw-r--r--   0 m         (1000) m         (1000)   118567 2024-03-24 00:36:09.000000 zebrafy-1.1.3/tests/static/test_image_z64_broken_compression.zpl
--rw-r--r--   0 m         (1000) m         (1000)   118567 2024-03-24 00:36:09.000000 zebrafy-1.1.3/tests/static/test_image_z64_broken_crc.zpl
--rw-r--r--   0 m         (1000) m         (1000)   315326 2023-08-14 03:18:02.000000 zebrafy-1.1.3/tests/static/test_pdf.pdf
--rw-r--r--   0 m         (1000) m         (1000)   244006 2024-03-24 00:36:09.000000 zebrafy-1.1.3/tests/static/test_pdf_ascii.zpl
--rw-r--r--   0 m         (1000) m         (1000)   162712 2024-03-24 00:36:09.000000 zebrafy-1.1.3/tests/static/test_pdf_b64.zpl
--rw-r--r--   0 m         (1000) m         (1000)   244006 2023-08-14 03:06:35.000000 zebrafy-1.1.3/tests/static/test_pdf_high_threshold.zpl
--rw-r--r--   0 m         (1000) m         (1000)   244006 2023-08-14 03:06:35.000000 zebrafy-1.1.3/tests/static/test_pdf_low_threshold.zpl
--rw-r--r--   0 m         (1000) m         (1000)   244006 2023-08-14 03:06:35.000000 zebrafy-1.1.3/tests/static/test_pdf_no_dither.zpl
--rw-r--r--   0 m         (1000) m         (1000)   242422 2024-05-16 06:02:35.000000 zebrafy-1.1.3/tests/static/test_pdf_rotation.zpl
--rw-r--r--   0 m         (1000) m         (1000)   244014 2024-05-12 01:56:42.000000 zebrafy-1.1.3/tests/static/test_pdf_split_pages.zpl
--rw-r--r--   0 m         (1000) m         (1000)   460872 2023-08-14 03:06:35.000000 zebrafy-1.1.3/tests/static/test_pdf_width_height.zpl
--rw-r--r--   0 m         (1000) m         (1000)    31971 2024-03-24 00:36:09.000000 zebrafy-1.1.3/tests/static/test_pdf_z64.zpl
--rw-r--r--   0 m         (1000) m         (1000)    24019 2024-05-24 03:15:43.000000 zebrafy-1.1.3/tests/test_zebrafy.py
-drwxr-xr-x   0 m         (1000) m         (1000)        0 2024-05-24 03:18:33.728341 zebrafy-1.1.3/zebrafy/
--rw-r--r--   0 m         (1000) m         (1000)      465 2024-05-24 03:15:43.000000 zebrafy-1.1.3/zebrafy/__init__.py
--rw-r--r--   0 m         (1000) m         (1000)     3258 2024-05-24 03:15:43.000000 zebrafy-1.1.3/zebrafy/crc.py
--rw-r--r--   0 m         (1000) m         (1000)     6324 2024-05-24 03:15:43.000000 zebrafy-1.1.3/zebrafy/graphic_field.py
--rw-r--r--   0 m         (1000) m         (1000)    11048 2024-05-24 03:15:43.000000 zebrafy-1.1.3/zebrafy/zebrafy_image.py
--rw-r--r--   0 m         (1000) m         (1000)    10987 2024-05-24 03:15:43.000000 zebrafy-1.1.3/zebrafy/zebrafy_pdf.py
--rw-r--r--   0 m         (1000) m         (1000)     5553 2024-05-24 03:15:43.000000 zebrafy-1.1.3/zebrafy/zebrafy_zpl.py
-drwxr-xr-x   0 m         (1000) m         (1000)        0 2024-05-24 03:18:33.728341 zebrafy-1.1.3/zebrafy.egg-info/
--rw-r--r--   0 m         (1000) m         (1000)    11657 2024-05-24 03:18:33.000000 zebrafy-1.1.3/zebrafy.egg-info/PKG-INFO
--rw-r--r--   0 m         (1000) m         (1000)     1759 2024-05-24 03:18:33.000000 zebrafy-1.1.3/zebrafy.egg-info/SOURCES.txt
--rw-r--r--   0 m         (1000) m         (1000)        1 2024-05-24 03:18:33.000000 zebrafy-1.1.3/zebrafy.egg-info/dependency_links.txt
--rw-r--r--   0 m         (1000) m         (1000)      140 2024-05-24 03:18:33.000000 zebrafy-1.1.3/zebrafy.egg-info/requires.txt
--rw-r--r--   0 m         (1000) m         (1000)        8 2024-05-24 03:18:33.000000 zebrafy-1.1.3/zebrafy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 05:00:42.188567 zebrafy-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-25 05:00:36.000000 zebrafy-1.1.4/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-25 05:00:36.000000 zebrafy-1.1.4/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 05:00:42.160566 zebrafy-1.1.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 05:00:42.164566 zebrafy-1.1.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-25 05:00:36.000000 zebrafy-1.1.4/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-25 05:00:36.000000 zebrafy-1.1.4/.github/ISSUE_TEMPLATE/feature_request.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 05:00:42.164566 zebrafy-1.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-25 05:00:36.000000 zebrafy-1.1.4/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-25 05:00:36.000000 zebrafy-1.1.4/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-25 05:00:36.000000 zebrafy-1.1.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-25 05:00:36.000000 zebrafy-1.1.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-25 05:00:36.000000 zebrafy-1.1.4/.prettierrc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-25 05:00:36.000000 zebrafy-1.1.4/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-25 05:00:36.000000 zebrafy-1.1.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-25 05:00:36.000000 zebrafy-1.1.4/.ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-25 05:00:36.000000 zebrafy-1.1.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11806 2024-05-25 05:00:42.188567 zebrafy-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10083 2024-05-25 05:00:36.000000 zebrafy-1.1.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 05:00:42.168566 zebrafy-1.1.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-25 05:00:36.000000 zebrafy-1.1.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-25 05:00:36.000000 zebrafy-1.1.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-25 05:00:36.000000 zebrafy-1.1.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-25 05:00:36.000000 zebrafy-1.1.4/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-25 05:00:36.000000 zebrafy-1.1.4/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-25 05:00:36.000000 zebrafy-1.1.4/docs/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-25 05:00:36.000000 zebrafy-1.1.4/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7859 2024-05-25 05:00:36.000000 zebrafy-1.1.4/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5962 2024-05-25 05:00:36.000000 zebrafy-1.1.4/docs/zebrafy-64.png
+-rw-r--r--   0 runner    (1001) docker     (127)   483090 2024-05-25 05:00:36.000000 zebrafy-1.1.4/docs/zebrafy-long.png
+-rw-r--r--   0 runner    (1001) docker     (127)   333682 2024-05-25 05:00:36.000000 zebrafy-1.1.4/docs/zebrafy.png
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-25 05:00:36.000000 zebrafy-1.1.4/docs/zebrafy.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-25 05:00:36.000000 zebrafy-1.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 05:00:42.188567 zebrafy-1.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 05:00:42.168566 zebrafy-1.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-25 05:00:36.000000 zebrafy-1.1.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 05:00:42.184567 zebrafy-1.1.4/tests/static/
+-rw-r--r--   0 runner    (1001) docker     (127)   261566 2024-05-25 05:00:36.000000 zebrafy-1.1.4/tests/static/test_image.png
+-rw-r--r--   0 runner    (1001) docker     (127)   108008 2024-05-25 05:00:36.000000 zebrafy-1.1.4/tests/static/test_image_ascii.png
+-rw-r--r--   0 runner    (1001) docker     (127)   409641 2024-05-25 05:00:36.000000 zebrafy-1.1.4/tests/static/test_image_ascii.zpl
+-rw-r--r--   0 runner    (1001) docker     (127)   108008 2024-05-25 05:00:36.000000 zebrafy-1.1.4/tests/static/test_image_b64.png
+-rw-r--r--   0 runner    (1001) docker     (127)   273119 2024-05-25 05:00:36.000000 zebrafy-1.1.4/tests/static/test_image_b64.zpl
+-rw-r--r--   0 runner    (1001) docker     (127)   409631 2024-05-25 05:00:36.000000 zebrafy-1.1.4/tests/static/test_image_broken.zpl
+-rw-r--r--   0 runner    (1001) docker     (127)   409641 2024-05-25 05:00:36.000000 zebrafy-1.1.4/tests/static/test_image_high_threshold.zpl
+-rw-r--r--   0 runner    (1001) docker     (127)   409641 2024-05-25 05:00:36.000000 zebrafy-1.1.4/tests/static/test_image_invert.zpl
+-rw-r--r--   0 runner    (1001) docker     (127)   409641 2024-05-25 05:00:36.000000 zebrafy-1.1.4/tests/static/test_image_invert_no_dither.zpl
+-rw-r--r--   0 runner    (1001) docker     (127)   409641 2024-05-25 05:00:36.000000 zebrafy-1.1.4/tests/static/test_image_low_threshold.zpl
+-rw-r--r--   0 runner    (1001) docker     (127)   819274 2024-05-25 05:00:36.000000 zebrafy-1.1.4/tests/static/test_image_multiple.zpl
+-rw-r--r--   0 runner    (1001) docker     (127)   409641 2024-05-25 05:00:36.000000 zebrafy-1.1.4/tests/static/test_image_no_dither.zpl
+-rw-r--r--   0 runner    (1001) docker     (127)   409645 2024-05-25 05:00:36.000000 zebrafy-1.1.4/tests/static/test_image_pos_x_pos_y.zpl
+-rw-r--r--   0 runner    (1001) docker     (127)   409641 2024-05-25 05:00:36.000000 zebrafy-1.1.4/tests/static/test_image_rotation.zpl
+-rw-r--r--   0 runner    (1001) docker     (127)    63038 2024-05-25 05:00:36.000000 zebrafy-1.1.4/tests/static/test_image_width_height.zpl
+-rw-r--r--   0 runner    (1001) docker     (127)   108008 2024-05-25 05:00:36.000000 zebrafy-1.1.4/tests/static/test_image_z64.png
+-rw-r--r--   0 runner    (1001) docker     (127)   118567 2024-05-25 05:00:36.000000 zebrafy-1.1.4/tests/static/test_image_z64.zpl
+-rw-r--r--   0 runner    (1001) docker     (127)   118567 2024-05-25 05:00:36.000000 zebrafy-1.1.4/tests/static/test_image_z64_broken_compression.zpl
+-rw-r--r--   0 runner    (1001) docker     (127)   118567 2024-05-25 05:00:36.000000 zebrafy-1.1.4/tests/static/test_image_z64_broken_crc.zpl
+-rw-r--r--   0 runner    (1001) docker     (127)   315326 2024-05-25 05:00:36.000000 zebrafy-1.1.4/tests/static/test_pdf.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)   244006 2024-05-25 05:00:36.000000 zebrafy-1.1.4/tests/static/test_pdf_ascii.zpl
+-rw-r--r--   0 runner    (1001) docker     (127)   162712 2024-05-25 05:00:36.000000 zebrafy-1.1.4/tests/static/test_pdf_b64.zpl
+-rw-r--r--   0 runner    (1001) docker     (127)   244006 2024-05-25 05:00:36.000000 zebrafy-1.1.4/tests/static/test_pdf_high_threshold.zpl
+-rw-r--r--   0 runner    (1001) docker     (127)   244006 2024-05-25 05:00:36.000000 zebrafy-1.1.4/tests/static/test_pdf_low_threshold.zpl
+-rw-r--r--   0 runner    (1001) docker     (127)   244006 2024-05-25 05:00:36.000000 zebrafy-1.1.4/tests/static/test_pdf_no_dither.zpl
+-rw-r--r--   0 runner    (1001) docker     (127)   242422 2024-05-25 05:00:36.000000 zebrafy-1.1.4/tests/static/test_pdf_rotation.zpl
+-rw-r--r--   0 runner    (1001) docker     (127)   244014 2024-05-25 05:00:36.000000 zebrafy-1.1.4/tests/static/test_pdf_split_pages.zpl
+-rw-r--r--   0 runner    (1001) docker     (127)   460872 2024-05-25 05:00:36.000000 zebrafy-1.1.4/tests/static/test_pdf_width_height.zpl
+-rw-r--r--   0 runner    (1001) docker     (127)    31971 2024-05-25 05:00:36.000000 zebrafy-1.1.4/tests/static/test_pdf_z64.zpl
+-rw-r--r--   0 runner    (1001) docker     (127)    24069 2024-05-25 05:00:36.000000 zebrafy-1.1.4/tests/test_zebrafy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 05:00:42.184567 zebrafy-1.1.4/zebrafy/
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-25 05:00:36.000000 zebrafy-1.1.4/zebrafy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-25 05:00:42.000000 zebrafy-1.1.4/zebrafy/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-05-25 05:00:36.000000 zebrafy-1.1.4/zebrafy/crc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-25 05:00:36.000000 zebrafy-1.1.4/zebrafy/graphic_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11055 2024-05-25 05:00:36.000000 zebrafy-1.1.4/zebrafy/zebrafy_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10994 2024-05-25 05:00:36.000000 zebrafy-1.1.4/zebrafy/zebrafy_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5560 2024-05-25 05:00:36.000000 zebrafy-1.1.4/zebrafy/zebrafy_zpl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 05:00:42.184567 zebrafy-1.1.4/zebrafy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11806 2024-05-25 05:00:42.000000 zebrafy-1.1.4/zebrafy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-05-25 05:00:42.000000 zebrafy-1.1.4/zebrafy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 05:00:42.000000 zebrafy-1.1.4/zebrafy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-25 05:00:42.000000 zebrafy-1.1.4/zebrafy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-25 05:00:42.000000 zebrafy-1.1.4/zebrafy.egg-info/top_level.txt
```

### Comparing `zebrafy-1.1.3/.github/workflows/ci.yml` & `zebrafy-1.1.4/.github/workflows/ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         with:
           python-version: 3.12
       - uses: pre-commit/action@v3.0.1
   tests:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11", "3.12"]
+        python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
     steps:
       - uses: actions/checkout@v4
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
```

### Comparing `zebrafy-1.1.3/.gitignore` & `zebrafy-1.1.4/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 var/
 wheels/
 share/python-wheels/
 *.egg-info/
 .installed.cfg
 *.egg
 MANIFEST
+_version.py
 
 # Sphinx documentation
 docs/_build/
 docs/generated
 
 # PyInstaller
 #  Usually these files are written by a python script from a template
```

### Comparing `zebrafy-1.1.3/.pre-commit-config.yaml` & `zebrafy-1.1.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `zebrafy-1.1.3/.readthedocs.yml` & `zebrafy-1.1.4/.readthedocs.yml`

 * *Files 6% similar despite different names*

```diff
@@ -22,7 +22,9 @@
 
 # Optional but recommended, declare the Python requirements required
 # to build your documentation
 # See https://docs.readthedocs.io/en/stable/guides/reproducible-builds.html
 python:
   install:
     - requirements: docs/requirements.txt
+    - method: pip
+      path: .
```

### Comparing `zebrafy-1.1.3/LICENSE.txt` & `zebrafy-1.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zebrafy-1.1.3/PKG-INFO` & `zebrafy-1.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 Metadata-Version: 2.1
 Name: zebrafy
-Version: 1.1.3
+Version: 1.1.4
 Summary: Python library for converting PDF and images to Zebra Programming Language (ZPL)
 Author-email: Miika Nissi <miika@miikanissi.com>
 Maintainer-email: Miika Nissi <miika@miikanissi.com>
 License: LGPLv3
 Project-URL: Homepage, https://github.com/miikanissi/zebrafy/
 Project-URL: Documentation, https://zebrafy.readthedocs.io/
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Manufacturing
 Classifier: Topic :: Printing
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: pillow
 Requires-Dist: pypdfium2>=4.8.0
 Provides-Extra: docs
 Requires-Dist: sphinx>=7.0.0; extra == "docs"
 Requires-Dist: sphinx_autodoc_typehints>=2.0.0; extra == "docs"
 Requires-Dist: sphinx_rtd_theme>=2.0.0; extra == "docs"
 Provides-Extra: test
 Requires-Dist: pytest-cov; extra == "test"
 Provides-Extra: lint
 Requires-Dist: pre-commit; extra == "lint"
+Provides-Extra: build
+Requires-Dist: setuptools>=64; extra == "build"
+Requires-Dist: setuptools_scm>=8; extra == "build"
+Requires-Dist: wheel; extra == "build"
+Requires-Dist: build; extra == "build"
 
 |zebrafy_icon_64| Zebrafy
 =========================
 
 .. |zebrafy_icon_64| image:: https://raw.githubusercontent.com/miikanissi/zebrafy/master/docs/zebrafy-64.png
    :alt: Zebrafy Logo
```

### Comparing `zebrafy-1.1.3/README.rst` & `zebrafy-1.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `zebrafy-1.1.3/docs/Makefile` & `zebrafy-1.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zebrafy-1.1.3/docs/conf.py` & `zebrafy-1.1.4/docs/conf.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,22 +9,24 @@
 # -- Path setup --------------------------------------------------------------
 
 import os
 import sys
 
 sys.path.insert(0, os.path.abspath(".."))
 
+from zebrafy import __version__
+
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = "Zebrafy"
 copyright = "2023, Miika Nissi"
 author = "Miika Nissi"
-version = "1.1.3"
-release = version
+release = __version__
+version = __version__
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.viewcode",
```

### Comparing `zebrafy-1.1.3/docs/make.bat` & `zebrafy-1.1.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `zebrafy-1.1.3/docs/requirements.txt` & `zebrafy-1.1.4/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `zebrafy-1.1.3/docs/usage.rst` & `zebrafy-1.1.4/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `zebrafy-1.1.3/docs/zebrafy-64.png` & `zebrafy-1.1.4/docs/zebrafy-64.png`

 * *Files identical despite different names*

### Comparing `zebrafy-1.1.3/docs/zebrafy-long.png` & `zebrafy-1.1.4/docs/zebrafy-long.png`

 * *Files identical despite different names*

### Comparing `zebrafy-1.1.3/docs/zebrafy.png` & `zebrafy-1.1.4/docs/zebrafy.png`

 * *Files identical despite different names*

### Comparing `zebrafy-1.1.3/docs/zebrafy.rst` & `zebrafy-1.1.4/docs/zebrafy.rst`

 * *Files identical despite different names*

### Comparing `zebrafy-1.1.3/pyproject.toml` & `zebrafy-1.1.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,52 @@
 [build-system]
-requires = [ "setuptools>=64", "wheel"]
+requires = ["setuptools>=64", "setuptools_scm>=8", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zebrafy"
-version = "1.1.3"
+dynamic = ["version"]
 description = "Python library for converting PDF and images to Zebra Programming Language (ZPL)"
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
     "Operating System :: OS Independent",
     "Natural Language :: English",
     "Programming Language :: Python",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Intended Audience :: Developers",
     "Intended Audience :: System Administrators",
     "Intended Audience :: Manufacturing",
     "Topic :: Printing",
 ]
 dependencies = ["pillow", "pypdfium2>=4.8.0"]
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 
 [project.optional-dependencies]
 docs = [
     "sphinx>=7.0.0",
     "sphinx_autodoc_typehints>=2.0.0",
     "sphinx_rtd_theme>=2.0.0",
 ]
 test = [
     "pytest-cov",
 ]
 lint = [
     "pre-commit",
 ]
+build = [
+    "setuptools>=64",
+    "setuptools_scm>=8",
+    "wheel",
+    "build",
+]
 
 [[project.authors]]
 name = "Miika Nissi"
 email = "miika@miikanissi.com"
 
 [[project.maintainers]]
 name = "Miika Nissi"
@@ -61,12 +66,16 @@
 [tool.setuptools]
 include-package-data = false
 
 [tool.setuptools.packages.find]
 include = [ "zebrafy"]
 namespaces = false
 
+[tool.setuptools_scm]
+version_file = "zebrafy/_version.py"
+version_scheme = "no-guess-dev"
+
 [tool.pytest.ini_options]
 addopts = "--cov --cov-report html --cov-report term-missing --cov-fail-under 95"
 
 [tool.coverage.run]
 source = ["zebrafy"]
```

### Comparing `zebrafy-1.1.3/tests/static/test_image.png` & `zebrafy-1.1.4/tests/static/test_image.png`

 * *Files identical despite different names*

### Comparing `zebrafy-1.1.3/tests/static/test_image_ascii.png` & `zebrafy-1.1.4/tests/static/test_image_ascii.png`

 * *Files identical despite different names*

### Comparing `zebrafy-1.1.3/tests/static/test_image_ascii.zpl` & `zebrafy-1.1.4/tests/static/test_image_ascii.zpl`

 * *Files identical despite different names*

### Comparing `zebrafy-1.1.3/tests/static/test_image_b64.png` & `zebrafy-1.1.4/tests/static/test_image_b64.png`

 * *Files identical despite different names*

### Comparing `zebrafy-1.1.3/tests/static/test_image_b64.zpl` & `zebrafy-1.1.4/tests/static/test_image_b64.zpl`

 * *Files identical despite different names*

### Comparing `zebrafy-1.1.3/tests/static/test_image_broken.zpl` & `zebrafy-1.1.4/tests/static/test_image_broken.zpl`

 * *Files identical despite different names*

### Comparing `zebrafy-1.1.3/tests/static/test_image_high_threshold.zpl` & `zebrafy-1.1.4/tests/static/test_image_high_threshold.zpl`

 * *Files identical despite different names*

### Comparing `zebrafy-1.1.3/tests/static/test_image_invert.zpl` & `zebrafy-1.1.4/tests/static/test_image_invert.zpl`

 * *Files identical despite different names*

### Comparing `zebrafy-1.1.3/tests/static/test_image_invert_no_dither.zpl` & `zebrafy-1.1.4/tests/static/test_image_invert_no_dither.zpl`

 * *Files identical despite different names*

### Comparing `zebrafy-1.1.3/tests/static/test_image_low_threshold.zpl` & `zebrafy-1.1.4/tests/static/test_image_low_threshold.zpl`

 * *Files identical despite different names*

### Comparing `zebrafy-1.1.3/tests/static/test_image_multiple.zpl` & `zebrafy-1.1.4/tests/static/test_image_multiple.zpl`

 * *Files identical despite different names*

### Comparing `zebrafy-1.1.3/tests/static/test_image_no_dither.zpl` & `zebrafy-1.1.4/tests/static/test_image_no_dither.zpl`

 * *Files identical despite different names*

### Comparing `zebrafy-1.1.3/tests/static/test_image_pos_x_pos_y.zpl` & `zebrafy-1.1.4/tests/static/test_image_pos_x_pos_y.zpl`

 * *Files identical despite different names*

### Comparing `zebrafy-1.1.3/tests/static/test_image_rotation.zpl` & `zebrafy-1.1.4/tests/static/test_image_rotation.zpl`

 * *Files identical despite different names*

### Comparing `zebrafy-1.1.3/tests/static/test_image_width_height.zpl` & `zebrafy-1.1.4/tests/static/test_image_width_height.zpl`

 * *Files identical despite different names*

### Comparing `zebrafy-1.1.3/tests/static/test_image_z64.png` & `zebrafy-1.1.4/tests/static/test_image_z64.png`

 * *Files identical despite different names*

### Comparing `zebrafy-1.1.3/tests/static/test_image_z64.zpl` & `zebrafy-1.1.4/tests/static/test_image_z64.zpl`

 * *Files identical despite different names*

### Comparing `zebrafy-1.1.3/tests/static/test_image_z64_broken_compression.zpl` & `zebrafy-1.1.4/tests/static/test_image_z64_broken_compression.zpl`

 * *Files identical despite different names*

### Comparing `zebrafy-1.1.3/tests/static/test_image_z64_broken_crc.zpl` & `zebrafy-1.1.4/tests/static/test_image_z64_broken_crc.zpl`

 * *Files identical despite different names*

### Comparing `zebrafy-1.1.3/tests/static/test_pdf.pdf` & `zebrafy-1.1.4/tests/static/test_pdf.pdf`

 * *Files identical despite different names*

### Comparing `zebrafy-1.1.3/tests/static/test_pdf_ascii.zpl` & `zebrafy-1.1.4/tests/static/test_pdf_ascii.zpl`

 * *Files identical despite different names*

### Comparing `zebrafy-1.1.3/tests/static/test_pdf_b64.zpl` & `zebrafy-1.1.4/tests/static/test_pdf_b64.zpl`

 * *Files identical despite different names*

### Comparing `zebrafy-1.1.3/tests/static/test_pdf_high_threshold.zpl` & `zebrafy-1.1.4/tests/static/test_pdf_high_threshold.zpl`

 * *Files identical despite different names*

### Comparing `zebrafy-1.1.3/tests/static/test_pdf_low_threshold.zpl` & `zebrafy-1.1.4/tests/static/test_pdf_low_threshold.zpl`

 * *Files identical despite different names*

### Comparing `zebrafy-1.1.3/tests/static/test_pdf_no_dither.zpl` & `zebrafy-1.1.4/tests/static/test_pdf_no_dither.zpl`

 * *Files identical despite different names*

### Comparing `zebrafy-1.1.3/tests/static/test_pdf_rotation.zpl` & `zebrafy-1.1.4/tests/static/test_pdf_rotation.zpl`

 * *Files identical despite different names*

### Comparing `zebrafy-1.1.3/tests/static/test_pdf_split_pages.zpl` & `zebrafy-1.1.4/tests/static/test_pdf_split_pages.zpl`

 * *Files identical despite different names*

### Comparing `zebrafy-1.1.3/tests/static/test_pdf_width_height.zpl` & `zebrafy-1.1.4/tests/static/test_pdf_width_height.zpl`

 * *Files identical despite different names*

### Comparing `zebrafy-1.1.3/tests/static/test_pdf_z64.zpl` & `zebrafy-1.1.4/tests/static/test_pdf_z64.zpl`

 * *Files identical despite different names*

### Comparing `zebrafy-1.1.3/tests/test_zebrafy.py` & `zebrafy-1.1.4/tests/test_zebrafy.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 #
 ########################################################################################
 
 # 1. Standard library imports:
 import io
 import os
 import unittest
+from importlib.metadata import version
 from typing import Union
 
 # 2. Known third party imports:
 from PIL import Image
 
 # 3. Local imports in the relative form:
 from zebrafy import CRC, GraphicField, ZebrafyImage, ZebrafyPDF, ZebrafyZPL, __version__
@@ -49,15 +50,15 @@
             os.path.join(os.path.join(os.path.dirname(__file__), "static"), file_name),
             open_mode,
         ) as file:
             return file.read()
 
     def test_version(self):
         """Test package version."""
-        self.assertEqual(__version__, "1.1.3")
+        self.assertEqual(__version__, version("zebrafy"))
 
     ###########
     # CRC Tests
     ###########
     def test_crc_data_bytes(self):
         """Test CRC data bytes input."""
         with self.assertRaises(ValueError):
```

### Comparing `zebrafy-1.1.3/zebrafy/crc.py` & `zebrafy-1.1.4/zebrafy/crc.py`

 * *Files identical despite different names*

### Comparing `zebrafy-1.1.3/zebrafy/graphic_field.py` & `zebrafy-1.1.4/zebrafy/graphic_field.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 import operator
 import zlib
 
 # 2. Known third party imports:
 from PIL.Image import Image
 
 # 3. Local imports in the relative form:
-from .crc import CRC
+from zebrafy.crc import CRC
 
 
 class GraphicField:
     """
     Converts a PIL image to Zebra Programming Language (ZPL) graphic field data.
 
     :param PIL.Image.Image image: An instance of a PIL Image.
```

### Comparing `zebrafy-1.1.3/zebrafy/zebrafy_image.py` & `zebrafy-1.1.4/zebrafy/zebrafy_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from io import BytesIO
 from typing import Union
 
 # 2. Known third party imports:
 from PIL import Image
 
 # 3. Local imports in the relative form:
-from .graphic_field import GraphicField
+from zebrafy.graphic_field import GraphicField
 
 
 class ZebrafyImage:
     """
     Convert a PIL Image or image bytes into Zebra Programming Language (ZPL).
 
     :param image: Image as a PIL Image or bytes object.
```

### Comparing `zebrafy-1.1.3/zebrafy/zebrafy_pdf.py` & `zebrafy-1.1.4/zebrafy/zebrafy_pdf.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 # 1. Standard library imports:
 import operator
 
 # 2. Known third party imports:
 from pypdfium2 import PdfDocument
 
 # 3. Local imports in the relative form:
-from .zebrafy_image import ZebrafyImage
+from zebrafy.zebrafy_image import ZebrafyImage
 
 
 class ZebrafyPDF:
     """
     Provides a method for converting PDFs to Zebra Programming Language (ZPL).
 
     :param pdf_bytes: PDF as a bytes object.
```

### Comparing `zebrafy-1.1.3/zebrafy/zebrafy_zpl.py` & `zebrafy-1.1.4/zebrafy/zebrafy_zpl.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 import zlib
 
 # 2. Known third party imports:
 from PIL import Image
 from pypdfium2 import PdfDocument, PdfImage, PdfMatrix
 
 # 3. Local imports in the relative form:
-from .crc import CRC
+from zebrafy.crc import CRC
 
 GF_MATCHER = re.compile(
     r"\^GF([ABC]*),([1-9][0-9]*),([1-9][0-9]*),([1-9][0-9]*),(.*?(?=\^FS))\^FS"
 )
 
 if sys.version_info >= (3, 9):
     DimensionsType = tuple[int, int]
```

### Comparing `zebrafy-1.1.3/zebrafy.egg-info/PKG-INFO` & `zebrafy-1.1.4/zebrafy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 Metadata-Version: 2.1
 Name: zebrafy
-Version: 1.1.3
+Version: 1.1.4
 Summary: Python library for converting PDF and images to Zebra Programming Language (ZPL)
 Author-email: Miika Nissi <miika@miikanissi.com>
 Maintainer-email: Miika Nissi <miika@miikanissi.com>
 License: LGPLv3
 Project-URL: Homepage, https://github.com/miikanissi/zebrafy/
 Project-URL: Documentation, https://zebrafy.readthedocs.io/
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Manufacturing
 Classifier: Topic :: Printing
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: pillow
 Requires-Dist: pypdfium2>=4.8.0
 Provides-Extra: docs
 Requires-Dist: sphinx>=7.0.0; extra == "docs"
 Requires-Dist: sphinx_autodoc_typehints>=2.0.0; extra == "docs"
 Requires-Dist: sphinx_rtd_theme>=2.0.0; extra == "docs"
 Provides-Extra: test
 Requires-Dist: pytest-cov; extra == "test"
 Provides-Extra: lint
 Requires-Dist: pre-commit; extra == "lint"
+Provides-Extra: build
+Requires-Dist: setuptools>=64; extra == "build"
+Requires-Dist: setuptools_scm>=8; extra == "build"
+Requires-Dist: wheel; extra == "build"
+Requires-Dist: build; extra == "build"
 
 |zebrafy_icon_64| Zebrafy
 =========================
 
 .. |zebrafy_icon_64| image:: https://raw.githubusercontent.com/miikanissi/zebrafy/master/docs/zebrafy-64.png
    :alt: Zebrafy Logo
```

### Comparing `zebrafy-1.1.3/zebrafy.egg-info/SOURCES.txt` & `zebrafy-1.1.4/zebrafy.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 .editorconfig
 .gitattributes
 .gitignore
 .pre-commit-config.yaml
 .prettierrc.yml
 .pylintrc
 .readthedocs.yml
+.ruff.toml
 LICENSE.txt
 README.rst
 pyproject.toml
+.github/ISSUE_TEMPLATE/bug_report.yml
+.github/ISSUE_TEMPLATE/feature_request.yml
 .github/workflows/ci.yml
+.github/workflows/publish.yml
 docs/Makefile
 docs/conf.py
 docs/index.rst
 docs/make.bat
 docs/modules.rst
 docs/requirements.in
 docs/requirements.txt
@@ -49,14 +53,15 @@
 tests/static/test_pdf_low_threshold.zpl
 tests/static/test_pdf_no_dither.zpl
 tests/static/test_pdf_rotation.zpl
 tests/static/test_pdf_split_pages.zpl
 tests/static/test_pdf_width_height.zpl
 tests/static/test_pdf_z64.zpl
 zebrafy/__init__.py
+zebrafy/_version.py
 zebrafy/crc.py
 zebrafy/graphic_field.py
 zebrafy/zebrafy_image.py
 zebrafy/zebrafy_pdf.py
 zebrafy/zebrafy_zpl.py
 zebrafy.egg-info/PKG-INFO
 zebrafy.egg-info/SOURCES.txt
```

