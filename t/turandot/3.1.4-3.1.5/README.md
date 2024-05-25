# Comparing `tmp/turandot-3.1.4.tar.gz` & `tmp/turandot-3.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turandot-3.1.4.tar", last modified: Wed Apr 17 16:11:11 2024, max compression
+gzip compressed data, was "turandot-3.1.5.tar", last modified: Sat May 25 18:54:47 2024, max compression
```

## Comparing `turandot-3.1.4.tar` & `turandot-3.1.5.tar`

### file list

```diff
@@ -1,160 +1,159 @@
-drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2024-04-17 16:11:11.445917 turandot-3.1.4/
--rw-r--r--   0 dinu      (1000) dinu      (1000)    35075 2023-02-28 11:23:16.000000 turandot-3.1.4/LICENSE.txt
--rw-r--r--   0 dinu      (1000) dinu      (1000)       21 2023-02-28 11:23:16.000000 turandot-3.1.4/MANIFEST.in
--rw-r--r--   0 dinu      (1000) dinu      (1000)     2028 2024-04-17 16:11:11.444918 turandot-3.1.4/PKG-INFO
--rw-r--r--   0 dinu      (1000) dinu      (1000)     1073 2023-02-28 11:23:16.000000 turandot-3.1.4/README.md
--rw-r--r--   0 dinu      (1000) dinu      (1000)       38 2024-04-17 16:11:11.445917 turandot-3.1.4/setup.cfg
--rw-r--r--   0 dinu      (1000) dinu      (1000)     2329 2024-04-17 16:03:03.000000 turandot-3.1.4/setup.py
-drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2024-04-17 16:11:11.167914 turandot-3.1.4/turandot/
--rw-r--r--   0 dinu      (1000) dinu      (1000)      294 2024-04-17 16:03:03.000000 turandot-3.1.4/turandot/__init__.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     1705 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/__main__.py
-drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2024-04-17 16:11:11.192914 turandot-3.1.4/turandot/assets/
--rw-r--r--   0 dinu      (1000) dinu      (1000)        0 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/assets/__init__.py
-drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2024-04-17 16:11:11.192914 turandot-3.1.4/turandot/assets/__pycache__/
--rw-r--r--   0 dinu      (1000) dinu      (1000)      169 2023-05-28 13:16:13.000000 turandot-3.1.4/turandot/assets/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 dinu      (1000) dinu      (1000)      836 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/assets/about.txt
--rw-r--r--   0 dinu      (1000) dinu      (1000)     2663 2024-03-03 22:01:22.000000 turandot-3.1.4/turandot/assets/default.yaml
-drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2024-04-17 16:11:11.192914 turandot-3.1.4/turandot/assets/extract/
--rw-r--r--   0 dinu      (1000) dinu      (1000)        0 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/assets/extract/__init__.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     1250 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/assets/extract/__main__.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)       90 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/assets/gtk4.css
--rw-r--r--   0 dinu      (1000) dinu      (1000)      233 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/assets/turandot.desktop
--rw-r--r--   0 dinu      (1000) dinu      (1000)     9430 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/assets/turandot.png
--rw-r--r--   0 dinu      (1000) dinu      (1000)       74 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/assets/turandot.sh
--rw-r--r--   0 dinu      (1000) dinu      (1000)    20902 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/assets/turandot.svg
--rw-r--r--   0 dinu      (1000) dinu      (1000)      243 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/assets/uninstall.sh
--rw-r--r--   0 dinu      (1000) dinu      (1000)      235 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/assets/update.sh
--rw-r--r--   0 dinu      (1000) dinu      (1000)     2836 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/assets/windows_fonts.conf
--rw-r--r--   0 dinu      (1000) dinu      (1000)      568 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/exceptions.py
-drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2024-04-17 16:11:11.195914 turandot-3.1.4/turandot/gtk4/
--rw-r--r--   0 dinu      (1000) dinu      (1000)      154 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/gtk4/__init__.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     1018 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/gtk4/__main__.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     1113 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/gtk4/catcher.py
-drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2024-04-17 16:11:11.213914 turandot-3.1.4/turandot/gtk4/controllers/
--rw-r--r--   0 dinu      (1000) dinu      (1000)      441 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/gtk4/controllers/__init__.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)      178 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/gtk4/controllers/basecontroller.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     2992 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/gtk4/controllers/conversionupdater.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     6713 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/gtk4/controllers/convertercontroller.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     2943 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/gtk4/controllers/cslcontroller.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)      814 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/gtk4/controllers/headerbarcontroller.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     3855 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/gtk4/controllers/templatecontroller.py
-drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2024-04-17 16:11:11.216915 turandot-3.1.4/turandot/gtk4/dialogs/
--rw-r--r--   0 dinu      (1000) dinu      (1000)      333 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/gtk4/dialogs/__init__.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     1507 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/gtk4/dialogs/aboutdialog.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     1613 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/gtk4/dialogs/confirmationdialog.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     1624 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/gtk4/dialogs/errordialog.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     2774 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/gtk4/dialogs/filechooser.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     3106 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/gtk4/dialogs/settingsdialog.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)      953 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/gtk4/dialogs/templateeditor.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)      992 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/gtk4/enumlocalization.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     2987 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/gtk4/filefilters.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)      281 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/gtk4/guithread.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     4804 2023-08-21 16:17:47.000000 turandot-3.1.4/turandot/gtk4/mainwindow.py
-drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2024-04-17 16:11:11.218915 turandot-3.1.4/turandot/gtk4/presentations/
--rw-r--r--   0 dinu      (1000) dinu      (1000)      377 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/gtk4/presentations/__init__.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)      670 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/gtk4/presentations/enumdropdown.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     1027 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/gtk4/presentations/observerdropdown.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     1728 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/gtk4/presentations/observerlistviews.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     5197 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/gtk4/presentations/settingspresentation.py
-drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2024-04-17 16:11:11.219915 turandot-3.1.4/turandot/gtk4/representations/
--rw-r--r--   0 dinu      (1000) dinu      (1000)      194 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/gtk4/representations/__init__.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)      654 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/gtk4/representations/dbobservables.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)      508 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/gtk4/representations/observerbase.py
-drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2024-04-17 16:11:11.221915 turandot-3.1.4/turandot/gtk4/views/
--rw-r--r--   0 dinu      (1000) dinu      (1000)      277 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/gtk4/views/__init__.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     8328 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/gtk4/views/convertertab.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     3151 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/gtk4/views/csltab.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)      845 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/gtk4/views/headerbarview.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     4641 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/gtk4/views/templatetab.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)      747 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/gtk4/views/viewcomponent.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)      280 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/meta.py
-drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2024-04-17 16:11:11.237915 turandot-3.1.4/turandot/model/
--rw-r--r--   0 dinu      (1000) dinu      (1000)     1571 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/model/__init__.py
-drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2024-04-17 16:11:11.252915 turandot-3.1.4/turandot/model/config/
--rw-r--r--   0 dinu      (1000) dinu      (1000)        1 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/model/config/__init__.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     2241 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/model/config/config.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     2381 2024-03-03 17:12:18.000000 turandot-3.1.4/turandot/model/config/configdict.py
-drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2024-04-17 16:11:11.347916 turandot-3.1.4/turandot/model/converter/
--rw-r--r--   0 dinu      (1000) dinu      (1000)        0 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/model/converter/__init__.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     3596 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/model/converter/applytemplate.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     3801 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/model/converter/conversionprocessor.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     3594 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/model/converter/converterbase.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     1284 2024-03-03 22:47:37.000000 turandot-3.1.4/turandot/model/converter/converterchain.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     3852 2024-03-03 21:35:42.000000 turandot-3.1.4/turandot/model/converter/convtohtml.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     2716 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/model/converter/copytemplate.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)      841 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/model/converter/frontendstrategy.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     4051 2024-03-03 21:35:01.000000 turandot-3.1.4/turandot/model/converter/gatherdata.py
-drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2024-04-17 16:11:11.392917 turandot-3.1.4/turandot/model/converter/optional/
--rw-r--r--   0 dinu      (1000) dinu      (1000)      252 2024-03-03 22:32:49.000000 turandot-3.1.4/turandot/model/converter/optional/__init__.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     1043 2024-03-03 23:18:15.000000 turandot-3.1.4/turandot/model/converter/optional/listoffigurescollector.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     1020 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/model/converter/optional/tocpagination.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     1587 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/model/converter/optional/unifiedmath.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     3150 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/model/converter/weasytopdf.py
-drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2024-04-17 16:11:11.397917 turandot-3.1.4/turandot/model/datastructures/
--rw-r--r--   0 dinu      (1000) dinu      (1000)        0 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/model/datastructures/__init__.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     1448 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/model/datastructures/baseasset.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     1392 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/model/datastructures/companiondata.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     1717 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/model/datastructures/conversionjob.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     1509 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/model/datastructures/cslasset.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     1255 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/model/datastructures/dbasset.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     1075 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/model/datastructures/enums.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     2123 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/model/datastructures/queuemsg.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)      646 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/model/datastructures/sourceasset.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)      256 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/model/datastructures/textasset.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     4205 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/model/datastructures/tmplasset.py
-drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2024-04-17 16:11:11.421917 turandot-3.1.4/turandot/model/sql/
--rw-r--r--   0 dinu      (1000) dinu      (1000)      222 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/model/sql/__init__.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)       82 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/model/sql/base.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     1491 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/model/sql/engine.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     4475 2023-05-28 13:28:06.000000 turandot-3.1.4/turandot/model/sql/repository.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)      811 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/model/sql/tables.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     1170 2023-05-28 14:13:52.000000 turandot-3.1.4/turandot/model/util.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     2436 2023-05-28 14:09:13.000000 turandot-3.1.4/turandot/model/zoteroconnector.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     1225 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/sysinfo.py
-drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2024-04-17 16:11:11.434917 turandot-3.1.4/turandot/ttk/
--rw-r--r--   0 dinu      (1000) dinu      (1000)       91 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/ttk/__init__.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     1206 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/ttk/__main__.py
-drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2024-04-17 16:11:11.437917 turandot-3.1.4/turandot/ttk/controllers/
--rw-r--r--   0 dinu      (1000) dinu      (1000)      591 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/ttk/controllers/__init__.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     1277 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/ttk/controllers/aboutcontroller.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)      238 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/ttk/controllers/basecontroller.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     4300 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/ttk/controllers/conversionupdater.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     4852 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/ttk/controllers/convertercontroller.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     7532 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/ttk/controllers/dbdropdowncontroller.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)      871 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/ttk/controllers/exceptioncontroller.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     3992 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/ttk/controllers/exportcontroller.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     3033 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/ttk/controllers/settingscontroller.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)      593 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/ttk/filetypes.py
-drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2024-04-17 16:11:11.439917 turandot-3.1.4/turandot/ttk/presentations/
--rw-r--r--   0 dinu      (1000) dinu      (1000)      644 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/ttk/presentations/__init__.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     5979 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/ttk/presentations/configpresentations.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)      788 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/ttk/presentations/dbfedpicker.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     1969 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/ttk/presentations/dropdownobservables.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     2138 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/ttk/presentations/dropdownobservers.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)      594 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/ttk/presentations/enumcombobox.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     1923 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/ttk/presentations/kvcombobox.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)      434 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/ttk/tkcatcher.py
-drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2024-04-17 16:11:11.442917 turandot-3.1.4/turandot/ttk/view/
--rw-r--r--   0 dinu      (1000) dinu      (1000)      159 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/ttk/view/__init__.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)      574 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/ttk/view/abouttab.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     6302 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/ttk/view/convertertab.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     2607 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/ttk/view/csltab.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     4709 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/ttk/view/processframe.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     2075 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/ttk/view/settingstab.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     1402 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/ttk/view/styles.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     3702 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/ttk/view/templatetab.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     4805 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/ttk/view/ttkview.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)      355 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/ttk/view/viewcomponent.py
-drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2024-04-17 16:11:11.444918 turandot-3.1.4/turandot/ui/
--rw-r--r--   0 dinu      (1000) dinu      (1000)      330 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/ui/__init__.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)      780 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/ui/background.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     1246 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/ui/enumtranslations.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     1266 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/ui/exceptioncatcher.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)      220 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/ui/frontend.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)      968 2023-02-28 11:23:16.000000 turandot-3.1.4/turandot/ui/utils.py
-drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2024-04-17 16:11:11.169914 turandot-3.1.4/turandot.egg-info/
--rw-r--r--   0 dinu      (1000) dinu      (1000)     2028 2024-04-17 16:11:10.000000 turandot-3.1.4/turandot.egg-info/PKG-INFO
--rw-r--r--   0 dinu      (1000) dinu      (1000)     4827 2024-04-17 16:11:11.000000 turandot-3.1.4/turandot.egg-info/SOURCES.txt
--rw-r--r--   0 dinu      (1000) dinu      (1000)        1 2024-04-17 16:11:10.000000 turandot-3.1.4/turandot.egg-info/dependency_links.txt
--rw-r--r--   0 dinu      (1000) dinu      (1000)      529 2024-04-17 16:11:10.000000 turandot-3.1.4/turandot.egg-info/requires.txt
--rw-r--r--   0 dinu      (1000) dinu      (1000)        9 2024-04-17 16:11:10.000000 turandot-3.1.4/turandot.egg-info/top_level.txt
+drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2024-05-25 18:54:47.511465 turandot-3.1.5/
+-rw-r--r--   0 dinu      (1000) dinu      (1000)    35075 2023-03-19 21:13:03.000000 turandot-3.1.5/LICENSE.txt
+-rw-r--r--   0 dinu      (1000) dinu      (1000)       21 2023-03-19 21:13:03.000000 turandot-3.1.5/MANIFEST.in
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     2028 2024-05-25 18:54:47.511465 turandot-3.1.5/PKG-INFO
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1073 2023-03-19 21:13:03.000000 turandot-3.1.5/README.md
+-rw-r--r--   0 dinu      (1000) dinu      (1000)       38 2024-05-25 18:54:47.511465 turandot-3.1.5/setup.cfg
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     2329 2024-05-25 18:45:37.000000 turandot-3.1.5/setup.py
+drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2024-05-25 18:54:47.504465 turandot-3.1.5/turandot/
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      294 2024-05-25 18:45:37.000000 turandot-3.1.5/turandot/__init__.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1705 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/__main__.py
+drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2024-05-25 18:54:47.505465 turandot-3.1.5/turandot/assets/
+-rw-r--r--   0 dinu      (1000) dinu      (1000)        0 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/assets/__init__.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      836 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/assets/about.txt
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     2663 2024-05-25 18:45:37.000000 turandot-3.1.5/turandot/assets/default.yaml
+drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2024-05-25 18:54:47.505465 turandot-3.1.5/turandot/assets/extract/
+-rw-r--r--   0 dinu      (1000) dinu      (1000)        0 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/assets/extract/__init__.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1250 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/assets/extract/__main__.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)       90 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/assets/gtk4.css
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      233 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/assets/turandot.desktop
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     9430 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/assets/turandot.png
+-rw-r--r--   0 dinu      (1000) dinu      (1000)       74 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/assets/turandot.sh
+-rw-r--r--   0 dinu      (1000) dinu      (1000)    20902 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/assets/turandot.svg
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      243 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/assets/uninstall.sh
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      235 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/assets/update.sh
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     2836 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/assets/windows_fonts.conf
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      568 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/exceptions.py
+drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2024-05-25 18:54:47.506465 turandot-3.1.5/turandot/gtk4/
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      154 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/gtk4/__init__.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1018 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/gtk4/__main__.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1113 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/gtk4/catcher.py
+drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2024-05-25 18:54:47.506465 turandot-3.1.5/turandot/gtk4/controllers/
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      441 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/gtk4/controllers/__init__.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      178 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/gtk4/controllers/basecontroller.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     2992 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/gtk4/controllers/conversionupdater.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     6713 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/gtk4/controllers/convertercontroller.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     2943 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/gtk4/controllers/cslcontroller.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      814 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/gtk4/controllers/headerbarcontroller.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     3855 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/gtk4/controllers/templatecontroller.py
+drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2024-05-25 18:54:47.506465 turandot-3.1.5/turandot/gtk4/dialogs/
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      333 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/gtk4/dialogs/__init__.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1507 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/gtk4/dialogs/aboutdialog.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1613 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/gtk4/dialogs/confirmationdialog.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1624 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/gtk4/dialogs/errordialog.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     2774 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/gtk4/dialogs/filechooser.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     3106 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/gtk4/dialogs/settingsdialog.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      953 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/gtk4/dialogs/templateeditor.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      992 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/gtk4/enumlocalization.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     2987 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/gtk4/filefilters.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      281 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/gtk4/guithread.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     4804 2024-05-25 18:45:37.000000 turandot-3.1.5/turandot/gtk4/mainwindow.py
+drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2024-05-25 18:54:47.507465 turandot-3.1.5/turandot/gtk4/presentations/
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      377 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/gtk4/presentations/__init__.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      670 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/gtk4/presentations/enumdropdown.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1027 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/gtk4/presentations/observerdropdown.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1728 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/gtk4/presentations/observerlistviews.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     5197 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/gtk4/presentations/settingspresentation.py
+drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2024-05-25 18:54:47.507465 turandot-3.1.5/turandot/gtk4/representations/
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      194 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/gtk4/representations/__init__.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      654 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/gtk4/representations/dbobservables.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      508 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/gtk4/representations/observerbase.py
+drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2024-05-25 18:54:47.507465 turandot-3.1.5/turandot/gtk4/views/
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      277 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/gtk4/views/__init__.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     8328 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/gtk4/views/convertertab.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     3151 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/gtk4/views/csltab.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      845 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/gtk4/views/headerbarview.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     4641 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/gtk4/views/templatetab.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      747 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/gtk4/views/viewcomponent.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      280 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/meta.py
+drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2024-05-25 18:54:47.507465 turandot-3.1.5/turandot/model/
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1571 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/model/__init__.py
+drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2024-05-25 18:54:47.507465 turandot-3.1.5/turandot/model/config/
+-rw-r--r--   0 dinu      (1000) dinu      (1000)        1 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/model/config/__init__.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     2241 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/model/config/config.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     2381 2024-05-25 18:45:37.000000 turandot-3.1.5/turandot/model/config/configdict.py
+drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2024-05-25 18:54:47.508465 turandot-3.1.5/turandot/model/converter/
+-rw-r--r--   0 dinu      (1000) dinu      (1000)        0 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/model/converter/__init__.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     3596 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/model/converter/applytemplate.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     3801 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/model/converter/conversionprocessor.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     3594 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/model/converter/converterbase.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1383 2024-05-25 18:45:37.000000 turandot-3.1.5/turandot/model/converter/converterchain.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     3852 2024-05-25 18:45:37.000000 turandot-3.1.5/turandot/model/converter/convtohtml.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     2716 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/model/converter/copytemplate.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      841 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/model/converter/frontendstrategy.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     4051 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/model/converter/gatherdata.py
+drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2024-05-25 18:54:47.508465 turandot-3.1.5/turandot/model/converter/optional/
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      342 2024-05-25 18:45:37.000000 turandot-3.1.5/turandot/model/converter/optional/__init__.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     2083 2024-05-25 18:45:37.000000 turandot-3.1.5/turandot/model/converter/optional/listoffigurescollector.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      601 2024-05-25 18:45:37.000000 turandot-3.1.5/turandot/model/converter/optional/listoftablescollector.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1020 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/model/converter/optional/tocpagination.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1587 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/model/converter/optional/unifiedmath.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     3150 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/model/converter/weasytopdf.py
+drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2024-05-25 18:54:47.509465 turandot-3.1.5/turandot/model/datastructures/
+-rw-r--r--   0 dinu      (1000) dinu      (1000)        0 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/model/datastructures/__init__.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1448 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/model/datastructures/baseasset.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1392 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/model/datastructures/companiondata.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1717 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/model/datastructures/conversionjob.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1509 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/model/datastructures/cslasset.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1255 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/model/datastructures/dbasset.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1075 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/model/datastructures/enums.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     2123 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/model/datastructures/queuemsg.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      646 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/model/datastructures/sourceasset.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      256 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/model/datastructures/textasset.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     4205 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/model/datastructures/tmplasset.py
+drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2024-05-25 18:54:47.509465 turandot-3.1.5/turandot/model/sql/
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      222 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/model/sql/__init__.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)       82 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/model/sql/base.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1491 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/model/sql/engine.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     4475 2024-05-25 18:45:37.000000 turandot-3.1.5/turandot/model/sql/repository.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      811 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/model/sql/tables.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1170 2024-05-25 18:45:37.000000 turandot-3.1.5/turandot/model/util.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     2436 2024-05-25 18:45:37.000000 turandot-3.1.5/turandot/model/zoteroconnector.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1225 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/sysinfo.py
+drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2024-05-25 18:54:47.509465 turandot-3.1.5/turandot/ttk/
+-rw-r--r--   0 dinu      (1000) dinu      (1000)       91 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/ttk/__init__.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1206 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/ttk/__main__.py
+drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2024-05-25 18:54:47.509465 turandot-3.1.5/turandot/ttk/controllers/
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      591 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/ttk/controllers/__init__.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1277 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/ttk/controllers/aboutcontroller.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      238 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/ttk/controllers/basecontroller.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     4300 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/ttk/controllers/conversionupdater.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     4852 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/ttk/controllers/convertercontroller.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     7532 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/ttk/controllers/dbdropdowncontroller.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      871 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/ttk/controllers/exceptioncontroller.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     3992 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/ttk/controllers/exportcontroller.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     3033 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/ttk/controllers/settingscontroller.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      593 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/ttk/filetypes.py
+drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2024-05-25 18:54:47.510465 turandot-3.1.5/turandot/ttk/presentations/
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      644 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/ttk/presentations/__init__.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     5979 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/ttk/presentations/configpresentations.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      788 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/ttk/presentations/dbfedpicker.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1969 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/ttk/presentations/dropdownobservables.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     2138 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/ttk/presentations/dropdownobservers.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      594 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/ttk/presentations/enumcombobox.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1923 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/ttk/presentations/kvcombobox.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      434 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/ttk/tkcatcher.py
+drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2024-05-25 18:54:47.510465 turandot-3.1.5/turandot/ttk/view/
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      159 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/ttk/view/__init__.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      574 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/ttk/view/abouttab.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     6302 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/ttk/view/convertertab.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     2607 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/ttk/view/csltab.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     4709 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/ttk/view/processframe.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     2075 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/ttk/view/settingstab.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1402 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/ttk/view/styles.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     3702 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/ttk/view/templatetab.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     4805 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/ttk/view/ttkview.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      355 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/ttk/view/viewcomponent.py
+drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2024-05-25 18:54:47.510465 turandot-3.1.5/turandot/ui/
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      330 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/ui/__init__.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      780 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/ui/background.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1246 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/ui/enumtranslations.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1266 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/ui/exceptioncatcher.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      220 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/ui/frontend.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      968 2023-03-19 21:13:03.000000 turandot-3.1.5/turandot/ui/utils.py
+drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2024-05-25 18:54:47.505465 turandot-3.1.5/turandot.egg-info/
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     2028 2024-05-25 18:54:47.000000 turandot-3.1.5/turandot.egg-info/PKG-INFO
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     4833 2024-05-25 18:54:47.000000 turandot-3.1.5/turandot.egg-info/SOURCES.txt
+-rw-r--r--   0 dinu      (1000) dinu      (1000)        1 2024-05-25 18:54:47.000000 turandot-3.1.5/turandot.egg-info/dependency_links.txt
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      529 2024-05-25 18:54:47.000000 turandot-3.1.5/turandot.egg-info/requires.txt
+-rw-r--r--   0 dinu      (1000) dinu      (1000)        9 2024-05-25 18:54:47.000000 turandot-3.1.5/turandot.egg-info/top_level.txt
```

### Comparing `turandot-3.1.4/LICENSE.txt` & `turandot-3.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/PKG-INFO` & `turandot-3.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turandot
-Version: 3.1.4
+Version: 3.1.5
 Summary: Turandot Markdown Converter
 Home-page: https://turandot.readthedocs.io
 Author: Martin Obrist
 Author-email: dev@obrist.email
 License: GPLv3
 Project-URL: Documentation, https://turandot.readthedocs.io
 Project-URL: Source Code, https://gitlab.com/dinuthehuman/turandot
```

### Comparing `turandot-3.1.4/README.md` & `turandot-3.1.5/README.md`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/setup.py` & `turandot-3.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages, setup
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='turandot',
-    version='3.1.4',
+    version='3.1.5',
     description='Turandot Markdown Converter',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="GPLv3",
     author='Martin Obrist',
     author_email='dev@obrist.email',
     url='https://turandot.readthedocs.io',
```

### Comparing `turandot-3.1.4/turandot/__main__.py` & `turandot-3.1.5/turandot/__main__.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/assets/about.txt` & `turandot-3.1.5/turandot/assets/about.txt`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/assets/default.yaml` & `turandot-3.1.5/turandot/assets/default.yaml`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/assets/extract/__main__.py` & `turandot-3.1.5/turandot/assets/extract/__main__.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/assets/turandot.png` & `turandot-3.1.5/turandot/assets/turandot.png`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/assets/turandot.svg` & `turandot-3.1.5/turandot/assets/turandot.svg`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/assets/windows_fonts.conf` & `turandot-3.1.5/turandot/assets/windows_fonts.conf`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/exceptions.py` & `turandot-3.1.5/turandot/exceptions.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/gtk4/__main__.py` & `turandot-3.1.5/turandot/gtk4/__main__.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/gtk4/catcher.py` & `turandot-3.1.5/turandot/gtk4/catcher.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/gtk4/controllers/conversionupdater.py` & `turandot-3.1.5/turandot/gtk4/controllers/conversionupdater.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/gtk4/controllers/convertercontroller.py` & `turandot-3.1.5/turandot/gtk4/controllers/convertercontroller.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/gtk4/controllers/cslcontroller.py` & `turandot-3.1.5/turandot/gtk4/controllers/cslcontroller.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/gtk4/controllers/headerbarcontroller.py` & `turandot-3.1.5/turandot/gtk4/controllers/headerbarcontroller.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/gtk4/controllers/templatecontroller.py` & `turandot-3.1.5/turandot/gtk4/controllers/templatecontroller.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/gtk4/dialogs/aboutdialog.py` & `turandot-3.1.5/turandot/gtk4/dialogs/aboutdialog.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/gtk4/dialogs/confirmationdialog.py` & `turandot-3.1.5/turandot/gtk4/dialogs/confirmationdialog.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/gtk4/dialogs/errordialog.py` & `turandot-3.1.5/turandot/gtk4/dialogs/errordialog.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/gtk4/dialogs/filechooser.py` & `turandot-3.1.5/turandot/gtk4/dialogs/filechooser.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/gtk4/dialogs/settingsdialog.py` & `turandot-3.1.5/turandot/gtk4/dialogs/settingsdialog.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/gtk4/dialogs/templateeditor.py` & `turandot-3.1.5/turandot/gtk4/dialogs/templateeditor.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/gtk4/enumlocalization.py` & `turandot-3.1.5/turandot/gtk4/enumlocalization.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/gtk4/filefilters.py` & `turandot-3.1.5/turandot/gtk4/filefilters.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/gtk4/mainwindow.py` & `turandot-3.1.5/turandot/gtk4/mainwindow.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/gtk4/presentations/enumdropdown.py` & `turandot-3.1.5/turandot/gtk4/presentations/enumdropdown.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/gtk4/presentations/observerdropdown.py` & `turandot-3.1.5/turandot/gtk4/presentations/observerdropdown.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/gtk4/presentations/observerlistviews.py` & `turandot-3.1.5/turandot/gtk4/presentations/observerlistviews.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/gtk4/presentations/settingspresentation.py` & `turandot-3.1.5/turandot/gtk4/presentations/settingspresentation.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/gtk4/representations/dbobservables.py` & `turandot-3.1.5/turandot/gtk4/representations/dbobservables.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/gtk4/views/convertertab.py` & `turandot-3.1.5/turandot/gtk4/views/convertertab.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/gtk4/views/csltab.py` & `turandot-3.1.5/turandot/gtk4/views/csltab.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/gtk4/views/headerbarview.py` & `turandot-3.1.5/turandot/gtk4/views/headerbarview.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/gtk4/views/templatetab.py` & `turandot-3.1.5/turandot/gtk4/views/templatetab.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/gtk4/views/viewcomponent.py` & `turandot-3.1.5/turandot/gtk4/views/viewcomponent.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/model/__init__.py` & `turandot-3.1.5/turandot/model/__init__.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/model/config/config.py` & `turandot-3.1.5/turandot/model/config/config.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/model/config/configdict.py` & `turandot-3.1.5/turandot/model/config/configdict.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/model/converter/applytemplate.py` & `turandot-3.1.5/turandot/model/converter/applytemplate.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/model/converter/conversionprocessor.py` & `turandot-3.1.5/turandot/model/converter/conversionprocessor.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/model/converter/converterbase.py` & `turandot-3.1.5/turandot/model/converter/converterbase.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/model/converter/converterchain.py` & `turandot-3.1.5/turandot/model/converter/converterchain.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from turandot import TurandotConversionException
 from turandot.model import ConverterBase, GatherData, CopyTemplate, ConversionAlgorithm, ConvertToHtml, OptionalStage, ApplyTemplate, WeasyprintToPdf
-from turandot.model.converter.optional import UnifiedMathMarker, TocPaginationContainers, ListOfFiguresCollector
+from turandot.model.converter.optional import UnifiedMathMarker, TocPaginationContainers, ListOfFiguresCollector, ListOfTablesCollector
 
 
 class ConverterChain:
 
     @staticmethod
     def build_chain(alg: ConversionAlgorithm) -> ConverterBase:
         """Build a chain of converter for a specified algorithm"""
@@ -16,13 +16,14 @@
     def _build_weasyprint() -> ConverterBase:
         """Build Weasyprint PDF conversion algorithm chain"""
         chain = GatherData()
         chain.chain_append(CopyTemplate())
         html = ConvertToHtml()
         html.register_optional(UnifiedMathMarker(), OptionalStage.PRE)
         html.register_optional(ListOfFiguresCollector(), OptionalStage.POST)
+        html.register_optional(ListOfTablesCollector(), OptionalStage.POST)
         chain.chain_append(html)
         tmpl = ApplyTemplate()
         tmpl.register_optional(TocPaginationContainers(), OptionalStage.POST)
         chain.chain_append(tmpl)
         chain.chain_append(WeasyprintToPdf())
         return chain
```

### Comparing `turandot-3.1.4/turandot/model/converter/convtohtml.py` & `turandot-3.1.5/turandot/model/converter/convtohtml.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/model/converter/copytemplate.py` & `turandot-3.1.5/turandot/model/converter/copytemplate.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/model/converter/frontendstrategy.py` & `turandot-3.1.5/turandot/model/converter/frontendstrategy.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/model/converter/gatherdata.py` & `turandot-3.1.5/turandot/model/converter/gatherdata.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/model/converter/optional/tocpagination.py` & `turandot-3.1.5/turandot/model/converter/optional/tocpagination.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/model/converter/optional/unifiedmath.py` & `turandot-3.1.5/turandot/model/converter/optional/unifiedmath.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/model/converter/weasytopdf.py` & `turandot-3.1.5/turandot/model/converter/weasytopdf.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/model/datastructures/baseasset.py` & `turandot-3.1.5/turandot/model/datastructures/baseasset.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/model/datastructures/companiondata.py` & `turandot-3.1.5/turandot/model/datastructures/companiondata.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/model/datastructures/conversionjob.py` & `turandot-3.1.5/turandot/model/datastructures/conversionjob.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/model/datastructures/cslasset.py` & `turandot-3.1.5/turandot/model/datastructures/cslasset.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/model/datastructures/dbasset.py` & `turandot-3.1.5/turandot/model/datastructures/dbasset.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/model/datastructures/enums.py` & `turandot-3.1.5/turandot/model/datastructures/enums.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/model/datastructures/queuemsg.py` & `turandot-3.1.5/turandot/model/datastructures/queuemsg.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/model/datastructures/sourceasset.py` & `turandot-3.1.5/turandot/model/datastructures/sourceasset.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/model/datastructures/tmplasset.py` & `turandot-3.1.5/turandot/model/datastructures/tmplasset.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/model/sql/engine.py` & `turandot-3.1.5/turandot/model/sql/engine.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/model/sql/repository.py` & `turandot-3.1.5/turandot/model/sql/repository.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/model/sql/tables.py` & `turandot-3.1.5/turandot/model/sql/tables.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/model/util.py` & `turandot-3.1.5/turandot/model/util.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/model/zoteroconnector.py` & `turandot-3.1.5/turandot/model/zoteroconnector.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/sysinfo.py` & `turandot-3.1.5/turandot/sysinfo.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/ttk/__main__.py` & `turandot-3.1.5/turandot/ttk/__main__.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/ttk/controllers/__init__.py` & `turandot-3.1.5/turandot/ttk/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/ttk/controllers/aboutcontroller.py` & `turandot-3.1.5/turandot/ttk/controllers/aboutcontroller.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/ttk/controllers/conversionupdater.py` & `turandot-3.1.5/turandot/ttk/controllers/conversionupdater.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/ttk/controllers/convertercontroller.py` & `turandot-3.1.5/turandot/ttk/controllers/convertercontroller.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/ttk/controllers/dbdropdowncontroller.py` & `turandot-3.1.5/turandot/ttk/controllers/dbdropdowncontroller.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/ttk/controllers/exceptioncontroller.py` & `turandot-3.1.5/turandot/ttk/controllers/exceptioncontroller.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/ttk/controllers/exportcontroller.py` & `turandot-3.1.5/turandot/ttk/controllers/exportcontroller.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/ttk/controllers/settingscontroller.py` & `turandot-3.1.5/turandot/ttk/controllers/settingscontroller.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/ttk/filetypes.py` & `turandot-3.1.5/turandot/ttk/filetypes.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/ttk/presentations/__init__.py` & `turandot-3.1.5/turandot/ttk/presentations/__init__.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/ttk/presentations/configpresentations.py` & `turandot-3.1.5/turandot/ttk/presentations/configpresentations.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/ttk/presentations/dbfedpicker.py` & `turandot-3.1.5/turandot/ttk/presentations/dbfedpicker.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/ttk/presentations/dropdownobservables.py` & `turandot-3.1.5/turandot/ttk/presentations/dropdownobservables.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/ttk/presentations/dropdownobservers.py` & `turandot-3.1.5/turandot/ttk/presentations/dropdownobservers.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/ttk/presentations/enumcombobox.py` & `turandot-3.1.5/turandot/ttk/presentations/enumcombobox.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/ttk/presentations/kvcombobox.py` & `turandot-3.1.5/turandot/ttk/presentations/kvcombobox.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/ttk/view/abouttab.py` & `turandot-3.1.5/turandot/ttk/view/abouttab.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/ttk/view/convertertab.py` & `turandot-3.1.5/turandot/ttk/view/convertertab.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/ttk/view/csltab.py` & `turandot-3.1.5/turandot/ttk/view/csltab.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/ttk/view/processframe.py` & `turandot-3.1.5/turandot/ttk/view/processframe.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/ttk/view/settingstab.py` & `turandot-3.1.5/turandot/ttk/view/settingstab.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/ttk/view/styles.py` & `turandot-3.1.5/turandot/ttk/view/styles.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/ttk/view/templatetab.py` & `turandot-3.1.5/turandot/ttk/view/templatetab.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/ttk/view/ttkview.py` & `turandot-3.1.5/turandot/ttk/view/ttkview.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/ui/background.py` & `turandot-3.1.5/turandot/ui/background.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/ui/enumtranslations.py` & `turandot-3.1.5/turandot/ui/enumtranslations.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/ui/exceptioncatcher.py` & `turandot-3.1.5/turandot/ui/exceptioncatcher.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot/ui/utils.py` & `turandot-3.1.5/turandot/ui/utils.py`

 * *Files identical despite different names*

### Comparing `turandot-3.1.4/turandot.egg-info/PKG-INFO` & `turandot-3.1.5/turandot.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turandot
-Version: 3.1.4
+Version: 3.1.5
 Summary: Turandot Markdown Converter
 Home-page: https://turandot.readthedocs.io
 Author: Martin Obrist
 Author-email: dev@obrist.email
 License: GPLv3
 Project-URL: Documentation, https://turandot.readthedocs.io
 Project-URL: Source Code, https://gitlab.com/dinuthehuman/turandot
```

### Comparing `turandot-3.1.4/turandot.egg-info/SOURCES.txt` & `turandot-3.1.5/turandot.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 turandot/assets/turandot.desktop
 turandot/assets/turandot.png
 turandot/assets/turandot.sh
 turandot/assets/turandot.svg
 turandot/assets/uninstall.sh
 turandot/assets/update.sh
 turandot/assets/windows_fonts.conf
-turandot/assets/__pycache__/__init__.cpython-311.pyc
 turandot/assets/extract/__init__.py
 turandot/assets/extract/__main__.py
 turandot/gtk4/__init__.py
 turandot/gtk4/__main__.py
 turandot/gtk4/catcher.py
 turandot/gtk4/enumlocalization.py
 turandot/gtk4/filefilters.py
@@ -75,14 +74,15 @@
 turandot/model/converter/convtohtml.py
 turandot/model/converter/copytemplate.py
 turandot/model/converter/frontendstrategy.py
 turandot/model/converter/gatherdata.py
 turandot/model/converter/weasytopdf.py
 turandot/model/converter/optional/__init__.py
 turandot/model/converter/optional/listoffigurescollector.py
+turandot/model/converter/optional/listoftablescollector.py
 turandot/model/converter/optional/tocpagination.py
 turandot/model/converter/optional/unifiedmath.py
 turandot/model/datastructures/__init__.py
 turandot/model/datastructures/baseasset.py
 turandot/model/datastructures/companiondata.py
 turandot/model/datastructures/conversionjob.py
 turandot/model/datastructures/cslasset.py
```

### Comparing `turandot-3.1.4/turandot.egg-info/requires.txt` & `turandot-3.1.5/turandot.egg-info/requires.txt`

 * *Files identical despite different names*

