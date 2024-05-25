# Comparing `tmp/notolog-0.9.1b7.tar.gz` & `tmp/notolog-0.9.1b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notolog-0.9.1b7.tar", last modified: Sun May 19 22:52:17 2024, max compression
+gzip compressed data, was "notolog-0.9.1b8.tar", last modified: Sat May 25 16:39:30 2024, max compression
```

## Comparing `notolog-0.9.1b7.tar` & `notolog-0.9.1b8.tar`

### file list

```diff
@@ -1,357 +1,361 @@
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:52:17.448300 notolog-0.9.1b7/
--rw-r--r--   0 vadikus    (501) staff       (20)     9022 2024-05-19 18:30:10.000000 notolog-0.9.1b7/CHANGELOG.md
--rw-r--r--   0 vadikus    (501) staff       (20)     3490 2024-05-11 12:17:28.000000 notolog-0.9.1b7/CODE_OF_CONDUCT.md
--rw-r--r--   0 vadikus    (501) staff       (20)     1073 2024-05-04 21:27:31.000000 notolog-0.9.1b7/LICENSE
--rw-r--r--   0 vadikus    (501) staff       (20)      433 2024-05-11 12:17:28.000000 notolog-0.9.1b7/MANIFEST.in
--rw-r--r--   0 vadikus    (501) staff       (20)    20127 2024-05-19 22:52:17.446785 notolog-0.9.1b7/PKG-INFO
--rw-r--r--   0 vadikus    (501) staff       (20)    18001 2024-05-19 22:31:49.000000 notolog-0.9.1b7/README.md
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:52:15.875377 notolog-0.9.1b7/docs/
--rw-r--r--   0 vadikus    (501) staff       (20)     8633 2024-05-19 18:30:10.000000 notolog-0.9.1b7/docs/Examples.md
--rw-r--r--   0 vadikus    (501) staff       (20)   241693 2024-05-19 18:30:10.000000 notolog-0.9.1b7/docs/notolog-ui-settings-strawberry-ja.png
--rw-r--r--   0 vadikus    (501) staff       (20)   247033 2024-05-04 21:27:32.000000 notolog-0.9.1b7/docs/notolog-ui-settings.png
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:52:15.909499 notolog-0.9.1b7/notolog/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     8264 2024-05-19 22:52:01.000000 notolog-0.9.1b7/notolog/app_config.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:52:15.929906 notolog-0.9.1b7/notolog/assets/
--rw-r--r--   0 vadikus    (501) staff       (20)     4202 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/notolog-example-image.png
--rw-r--r--   0 vadikus    (501) staff       (20)    88211 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/notolog-logo.png
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:52:15.851675 notolog-0.9.1b7/notolog/assets/themes/
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:52:15.973672 notolog-0.9.1b7/notolog/assets/themes/calligraphy/
--rw-r--r--   0 vadikus    (501) staff       (20)      777 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/calligraphy/about_popup.css
--rw-r--r--   0 vadikus    (501) staff       (20)      365 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/calligraphy/ai_assistant.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2767 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/calligraphy/default.ini
--rw-r--r--   0 vadikus    (501) staff       (20)       56 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/calligraphy/editor.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2311 2024-05-11 12:17:28.000000 notolog-0.9.1b7/notolog/assets/themes/calligraphy/md.ini
--rw-r--r--   0 vadikus    (501) staff       (20)      885 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/calligraphy/settings_dialog.css
--rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/calligraphy/statusbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)     6818 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/calligraphy/styles.css
--rw-r--r--   0 vadikus    (501) staff       (20)      221 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/calligraphy/toolbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)      743 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/calligraphy/tree_view.css
--rw-r--r--   0 vadikus    (501) staff       (20)       28 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/calligraphy/viewer.css
--rw-r--r--   0 vadikus    (501) staff       (20)       80 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/calligraphy/viewer.ini
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:52:15.992440 notolog-0.9.1b7/notolog/assets/themes/default/
--rw-r--r--   0 vadikus    (501) staff       (20)      798 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/about_popup.css
--rw-r--r--   0 vadikus    (501) staff       (20)      253 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/ai_assistant.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2775 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/default.ini
--rw-r--r--   0 vadikus    (501) staff       (20)      174 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/editor.css
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:52:16.056625 notolog-0.9.1b7/notolog/assets/themes/default/icons/
--rw-r--r--   0 vadikus    (501) staff       (20)     1093 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/icons/LICENSE
--rw-r--r--   0 vadikus    (501) staff       (20)      349 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/icons/arrow-clockwise.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      567 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/icons/arrow-repeat.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      736 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/icons/balloon-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      797 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/icons/balloon.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      812 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/icons/bandaid-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      959 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/icons/bandaid.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      528 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/icons/box-arrow-up-right.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      538 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/icons/box-arrow-up.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      265 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/icons/caret-down-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      265 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/icons/caret-up-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      455 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/icons/code-slash.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      694 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/icons/cursor-text.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      459 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/icons/eyedropper.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      403 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/icons/eyeglasses.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      479 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/icons/file-earmark-lock2.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      394 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/icons/file-earmark-plus-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      481 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/icons/file-earmark-x.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      294 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/icons/file-earmark.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      547 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/icons/filetype-html.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      705 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/icons/filetype-md.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      524 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/icons/filetype-txt.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      401 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/icons/floppy2-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      606 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/icons/floppy2.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      428 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/icons/folder-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      708 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/icons/folder-symlink.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      527 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/icons/folder.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      708 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/icons/github.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      518 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/icons/link-45deg.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      666 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/icons/linkedin.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      575 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/icons/pencil-square.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      261 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/icons/power.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      582 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/icons/quote.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      996 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/icons/robot.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      316 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/icons/share-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      653 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/icons/shield-lock-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)     1057 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/icons/shield-lock.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      399 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/icons/star-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      623 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/icons/star.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      272 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/icons/three-dots.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      577 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/icons/trash3-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      656 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/icons/trash3.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      301 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/icons/twitter-x.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      465 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/icons/type-bold.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      351 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/icons/type-italic.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      574 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/icons/type-strikethrough.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      319 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/icons/type-underline.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      351 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/icons/x-circle-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      397 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/icons/x-square-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      491 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/icons/x-square.svg
--rw-r--r--   0 vadikus    (501) staff       (20)     2363 2024-05-11 12:17:28.000000 notolog-0.9.1b7/notolog/assets/themes/default/md.ini
--rw-r--r--   0 vadikus    (501) staff       (20)      721 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/settings_dialog.css
--rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/statusbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)     8472 2024-05-11 12:17:28.000000 notolog-0.9.1b7/notolog/assets/themes/default/styles.css
--rw-r--r--   0 vadikus    (501) staff       (20)      221 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/toolbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)      744 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/tree_view.css
--rw-r--r--   0 vadikus    (501) staff       (20)       28 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/viewer.css
--rw-r--r--   0 vadikus    (501) staff       (20)       82 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/default/viewer.ini
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:52:16.285559 notolog-0.9.1b7/notolog/assets/themes/noir_dark/
--rw-r--r--   0 vadikus    (501) staff       (20)      777 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/noir_dark/about_popup.css
--rw-r--r--   0 vadikus    (501) staff       (20)      347 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/noir_dark/ai_assistant.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2745 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/noir_dark/default.ini
--rw-r--r--   0 vadikus    (501) staff       (20)       56 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/noir_dark/editor.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2480 2024-05-11 12:17:28.000000 notolog-0.9.1b7/notolog/assets/themes/noir_dark/md.ini
--rw-r--r--   0 vadikus    (501) staff       (20)     1435 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/noir_dark/settings_dialog.css
--rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/noir_dark/statusbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)     6935 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/noir_dark/styles.css
--rw-r--r--   0 vadikus    (501) staff       (20)      280 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/noir_dark/toolbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)      711 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/noir_dark/tree_view.css
--rw-r--r--   0 vadikus    (501) staff       (20)       28 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/noir_dark/viewer.css
--rw-r--r--   0 vadikus    (501) staff       (20)       76 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/noir_dark/viewer.ini
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:52:16.344677 notolog-0.9.1b7/notolog/assets/themes/strawberry/
--rw-r--r--   0 vadikus    (501) staff       (20)      790 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/strawberry/about_popup.css
--rw-r--r--   0 vadikus    (501) staff       (20)      317 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/strawberry/ai_assistant.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2775 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/strawberry/default.ini
--rw-r--r--   0 vadikus    (501) staff       (20)       50 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/strawberry/editor.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2408 2024-05-11 12:17:28.000000 notolog-0.9.1b7/notolog/assets/themes/strawberry/md.ini
--rw-r--r--   0 vadikus    (501) staff       (20)      753 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/strawberry/settings_dialog.css
--rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/strawberry/statusbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)     8451 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/strawberry/styles.css
--rw-r--r--   0 vadikus    (501) staff       (20)      221 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/strawberry/toolbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)      764 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/strawberry/tree_view.css
--rw-r--r--   0 vadikus    (501) staff       (20)       60 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/strawberry/viewer.css
--rw-r--r--   0 vadikus    (501) staff       (20)       84 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/assets/themes/strawberry/viewer.ini
--rw-r--r--   0 vadikus    (501) staff       (20)     3774 2024-05-19 18:30:10.000000 notolog-0.9.1b7/notolog/async_highlighter.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7959 2024-05-19 18:30:10.000000 notolog-0.9.1b7/notolog/edit_widget.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4247 2024-05-19 18:30:10.000000 notolog-0.9.1b7/notolog/editor_state.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:52:16.353974 notolog-0.9.1b7/notolog/encrypt/
--rw-r--r--   0 vadikus    (501) staff       (20)      152 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/encrypt/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4345 2024-05-19 18:30:10.000000 notolog-0.9.1b7/notolog/encrypt/enc_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5603 2024-05-19 18:30:10.000000 notolog-0.9.1b7/notolog/encrypt/enc_new_password_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)      626 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/encrypt/enc_password.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3686 2024-05-19 18:30:10.000000 notolog-0.9.1b7/notolog/encrypt/enc_password_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3215 2024-05-19 18:30:10.000000 notolog-0.9.1b7/notolog/encrypt/enc_password_reset_dialog.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:52:16.366618 notolog-0.9.1b7/notolog/enums/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/enums/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1433 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/enums/ai_model_names.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5624 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/enums/colors.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1125 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/enums/enum_base.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1367 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/enums/languages.py
--rw-r--r--   0 vadikus    (501) staff       (20)      451 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/enums/themes.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4500 2024-05-19 18:30:10.000000 notolog-0.9.1b7/notolog/etree_extension.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:52:16.368883 notolog-0.9.1b7/notolog/exceptions/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/exceptions/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)       52 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/exceptions/file_header_empty_exception.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7563 2024-05-19 18:30:10.000000 notolog-0.9.1b7/notolog/file_header.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2860 2024-05-19 18:30:10.000000 notolog-0.9.1b7/notolog/file_system_watcher.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:52:16.399603 notolog-0.9.1b7/notolog/helpers/
--rw-r--r--   0 vadikus    (501) staff       (20)       36 2024-05-19 18:30:10.000000 notolog-0.9.1b7/notolog/helpers/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)      187 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/helpers/clipboard_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4221 2024-05-19 18:30:10.000000 notolog-0.9.1b7/notolog/helpers/file_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3338 2024-05-19 18:30:10.000000 notolog-0.9.1b7/notolog/helpers/settings_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5644 2024-05-19 18:30:10.000000 notolog-0.9.1b7/notolog/helpers/theme_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1036 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/helpers/tooltip_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7538 2024-05-19 22:50:01.000000 notolog-0.9.1b7/notolog/helpers/update_helper.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:52:16.405511 notolog-0.9.1b7/notolog/highlight/
--rw-r--r--   0 vadikus    (501) staff       (20)      126 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/highlight/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     9219 2024-05-19 18:30:10.000000 notolog-0.9.1b7/notolog/highlight/main_highlighter.py
--rw-r--r--   0 vadikus    (501) staff       (20)    51824 2024-05-19 18:30:10.000000 notolog-0.9.1b7/notolog/highlight/md_highlighter.py
--rw-r--r--   0 vadikus    (501) staff       (20)     8475 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/highlight/view_highlighter.py
--rw-r--r--   0 vadikus    (501) staff       (20)    10886 2024-05-19 18:30:10.000000 notolog-0.9.1b7/notolog/image_downloader.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:52:16.408347 notolog-0.9.1b7/notolog/lexemes/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/__init__.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:52:16.423672 notolog-0.9.1b7/notolog/lexemes/de/
--rw-r--r--   0 vadikus    (501) staff       (20)      830 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/de/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7202 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/de/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6586 2024-05-11 12:17:28.000000 notolog-0.9.1b7/notolog/lexemes/de/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2267 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/de/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3788 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/de/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1225 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/de/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2757 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/de/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:52:16.434374 notolog-0.9.1b7/notolog/lexemes/en/
--rw-r--r--   0 vadikus    (501) staff       (20)      827 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/en/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7096 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/en/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6051 2024-05-11 12:17:28.000000 notolog-0.9.1b7/notolog/lexemes/en/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2181 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/en/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3586 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/en/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1201 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/en/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2573 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/en/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:52:16.447203 notolog-0.9.1b7/notolog/lexemes/es/
--rw-r--r--   0 vadikus    (501) staff       (20)      882 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/es/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7309 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/es/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6560 2024-05-11 12:17:28.000000 notolog-0.9.1b7/notolog/lexemes/es/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2316 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/es/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3890 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/es/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1222 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/es/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2793 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/es/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:52:16.583907 notolog-0.9.1b7/notolog/lexemes/fi/
--rw-r--r--   0 vadikus    (501) staff       (20)      856 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/fi/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7559 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/fi/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6292 2024-05-11 12:17:28.000000 notolog-0.9.1b7/notolog/lexemes/fi/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2261 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/fi/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3759 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/fi/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1334 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/fi/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2662 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/fi/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:52:16.596221 notolog-0.9.1b7/notolog/lexemes/fr/
--rw-r--r--   0 vadikus    (501) staff       (20)      886 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/fr/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7247 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/fr/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6716 2024-05-11 12:17:28.000000 notolog-0.9.1b7/notolog/lexemes/fr/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2344 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/fr/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3978 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/fr/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1236 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/fr/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2824 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/fr/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:52:16.632032 notolog-0.9.1b7/notolog/lexemes/ge/
--rw-r--r--   0 vadikus    (501) staff       (20)     1323 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/ge/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)    10627 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/ge/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     9735 2024-05-11 12:17:28.000000 notolog-0.9.1b7/notolog/lexemes/ge/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3459 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/ge/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5742 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/ge/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1583 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/ge/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4107 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/ge/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:52:16.644763 notolog-0.9.1b7/notolog/lexemes/gr/
--rw-r--r--   0 vadikus    (501) staff       (20)     1100 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/gr/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     8990 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/gr/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     8668 2024-05-11 12:17:28.000000 notolog-0.9.1b7/notolog/lexemes/gr/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2907 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/gr/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5016 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/gr/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1561 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/gr/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3679 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/gr/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:52:16.653838 notolog-0.9.1b7/notolog/lexemes/in/
--rw-r--r--   0 vadikus    (501) staff       (20)     1208 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/in/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     9434 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/in/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)    10078 2024-05-11 12:17:28.000000 notolog-0.9.1b7/notolog/lexemes/in/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3124 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/in/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5546 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/in/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1549 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/in/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3828 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/in/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:52:16.662845 notolog-0.9.1b7/notolog/lexemes/it/
--rw-r--r--   0 vadikus    (501) staff       (20)      864 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/it/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7263 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/it/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6366 2024-05-11 12:17:28.000000 notolog-0.9.1b7/notolog/lexemes/it/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2302 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/it/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3825 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/it/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1238 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/it/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2780 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/it/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:52:16.675824 notolog-0.9.1b7/notolog/lexemes/ja/
--rw-r--r--   0 vadikus    (501) staff       (20)      931 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/ja/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     8464 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/ja/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7248 2024-05-11 12:17:28.000000 notolog-0.9.1b7/notolog/lexemes/ja/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2443 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/ja/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4014 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/ja/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1242 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/ja/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3000 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/ja/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:52:16.703066 notolog-0.9.1b7/notolog/lexemes/ko/
--rw-r--r--   0 vadikus    (501) staff       (20)      848 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/ko/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7597 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/ko/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6775 2024-05-11 12:17:28.000000 notolog-0.9.1b7/notolog/lexemes/ko/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2268 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/ko/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3697 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/ko/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1221 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/ko/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2666 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/ko/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:52:16.735379 notolog-0.9.1b7/notolog/lexemes/la/
--rw-r--r--   0 vadikus    (501) staff       (20)      842 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/la/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7538 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/la/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6245 2024-05-11 12:17:28.000000 notolog-0.9.1b7/notolog/lexemes/la/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2297 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/la/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3753 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/la/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1257 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/la/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2736 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/la/toolbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3842 2024-05-19 18:30:10.000000 notolog-0.9.1b7/notolog/lexemes/lexemes.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:52:16.829852 notolog-0.9.1b7/notolog/lexemes/nl/
--rw-r--r--   0 vadikus    (501) staff       (20)      840 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/nl/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7094 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/nl/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6475 2024-05-11 12:17:28.000000 notolog-0.9.1b7/notolog/lexemes/nl/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2229 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/nl/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3673 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/nl/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1220 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/nl/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2647 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/nl/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:52:16.971458 notolog-0.9.1b7/notolog/lexemes/pt/
--rw-r--r--   0 vadikus    (501) staff       (20)      898 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/pt/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7304 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/pt/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6357 2024-05-11 12:17:28.000000 notolog-0.9.1b7/notolog/lexemes/pt/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2326 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/pt/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3830 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/pt/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1223 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/pt/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2830 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/pt/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:52:17.050524 notolog-0.9.1b7/notolog/lexemes/ru/
--rw-r--r--   0 vadikus    (501) staff       (20)      997 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/ru/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     9135 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/ru/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7938 2024-05-11 12:17:28.000000 notolog-0.9.1b7/notolog/lexemes/ru/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2883 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/ru/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4896 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/ru/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1428 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/ru/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3453 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/ru/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:52:17.119450 notolog-0.9.1b7/notolog/lexemes/se/
--rw-r--r--   0 vadikus    (501) staff       (20)      835 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/se/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7048 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/se/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6253 2024-05-11 12:17:28.000000 notolog-0.9.1b7/notolog/lexemes/se/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2216 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/se/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3627 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/se/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1220 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/se/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2611 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/se/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:52:17.132635 notolog-0.9.1b7/notolog/lexemes/tr/
--rw-r--r--   0 vadikus    (501) staff       (20)      809 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/tr/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7401 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/tr/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6154 2024-05-11 12:17:28.000000 notolog-0.9.1b7/notolog/lexemes/tr/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2276 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/tr/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3733 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/tr/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1240 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/tr/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2735 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/tr/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:52:17.261270 notolog-0.9.1b7/notolog/lexemes/zh/
--rw-r--r--   0 vadikus    (501) staff       (20)      792 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/zh/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7074 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/zh/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5777 2024-05-11 12:17:28.000000 notolog-0.9.1b7/notolog/lexemes/zh/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2175 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/zh/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3476 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/zh/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1202 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/zh/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2559 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/lexemes/zh/toolbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3290 2024-05-19 18:30:10.000000 notolog-0.9.1b7/notolog/main.py
--rw-r--r--   0 vadikus    (501) staff       (20)   175256 2024-05-19 22:50:01.000000 notolog-0.9.1b7/notolog/notolog_editor.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7318 2024-05-19 18:30:10.000000 notolog-0.9.1b7/notolog/settings.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3481 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/text_block_data.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5977 2024-05-19 18:30:10.000000 notolog-0.9.1b7/notolog/theme.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:52:17.413884 notolog-0.9.1b7/notolog/ui/
--rw-r--r--   0 vadikus    (501) staff       (20)      152 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/ui/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     8248 2024-05-19 18:30:10.000000 notolog-0.9.1b7/notolog/ui/about_popup.py
--rw-r--r--   0 vadikus    (501) staff       (20)    17345 2024-05-19 18:30:10.000000 notolog-0.9.1b7/notolog/ui/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2103 2024-05-19 18:30:10.000000 notolog-0.9.1b7/notolog/ui/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3551 2024-05-19 18:30:10.000000 notolog-0.9.1b7/notolog/ui/common_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1306 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/ui/enum_combo_box.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5615 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/ui/file_system_model.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7001 2024-05-19 18:30:10.000000 notolog-0.9.1b7/notolog/ui/line_numbers.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2614 2024-05-19 18:30:10.000000 notolog-0.9.1b7/notolog/ui/rename_file_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1229 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/ui/rotating_label.py
--rw-r--r--   0 vadikus    (501) staff       (20)    37315 2024-05-19 18:30:10.000000 notolog-0.9.1b7/notolog/ui/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3248 2024-05-19 18:30:10.000000 notolog-0.9.1b7/notolog/ui/sort_filter_proxy_model.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6844 2024-05-19 18:30:10.000000 notolog-0.9.1b7/notolog/ui/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)    12808 2024-05-19 18:30:10.000000 notolog-0.9.1b7/notolog/ui/toolbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)      455 2024-05-11 09:19:41.000000 notolog-0.9.1b7/notolog/ui/vertical_line_spacer.py
--rw-r--r--   0 vadikus    (501) staff       (20)     8195 2024-05-19 18:30:10.000000 notolog-0.9.1b7/notolog/view_decorator.py
--rw-r--r--   0 vadikus    (501) staff       (20)    16117 2024-05-19 18:30:10.000000 notolog-0.9.1b7/notolog/view_processor.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2452 2024-05-19 18:30:10.000000 notolog-0.9.1b7/notolog/view_widget.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:52:17.445329 notolog-0.9.1b7/notolog.egg-info/
--rw-r--r--   0 vadikus    (501) staff       (20)    20127 2024-05-19 22:52:15.000000 notolog-0.9.1b7/notolog.egg-info/PKG-INFO
--rw-r--r--   0 vadikus    (501) staff       (20)    11632 2024-05-19 22:52:15.000000 notolog-0.9.1b7/notolog.egg-info/SOURCES.txt
--rw-r--r--   0 vadikus    (501) staff       (20)        1 2024-05-19 22:52:15.000000 notolog-0.9.1b7/notolog.egg-info/dependency_links.txt
--rw-r--r--   0 vadikus    (501) staff       (20)       46 2024-05-19 22:52:15.000000 notolog-0.9.1b7/notolog.egg-info/entry_points.txt
--rw-r--r--   0 vadikus    (501) staff       (20)      335 2024-05-19 22:52:15.000000 notolog-0.9.1b7/notolog.egg-info/requires.txt
--rw-r--r--   0 vadikus    (501) staff       (20)       14 2024-05-19 22:52:15.000000 notolog-0.9.1b7/notolog.egg-info/top_level.txt
--rw-r--r--   0 vadikus    (501) staff       (20)      335 2024-05-19 18:30:10.000000 notolog-0.9.1b7/requirements.txt
--rw-r--r--   0 vadikus    (501) staff       (20)       38 2024-05-19 22:52:17.449268 notolog-0.9.1b7/setup.cfg
--rw-r--r--   0 vadikus    (501) staff       (20)     2384 2024-05-19 22:52:01.000000 notolog-0.9.1b7/setup.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:52:17.441175 notolog-0.9.1b7/tests/
--rw-r--r--   0 vadikus    (501) staff       (20)     1245 2024-05-19 18:30:10.000000 notolog-0.9.1b7/tests/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6151 2024-05-19 18:30:10.000000 notolog-0.9.1b7/tests/test_enc_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2309 2024-05-11 09:19:41.000000 notolog-0.9.1b7/tests/test_enc_password.py
--rw-r--r--   0 vadikus    (501) staff       (20)     9948 2024-05-19 18:30:10.000000 notolog-0.9.1b7/tests/test_file_header.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3983 2024-05-19 18:30:10.000000 notolog-0.9.1b7/tests/test_html_view.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5814 2024-05-11 09:19:41.000000 notolog-0.9.1b7/tests/test_lexemes.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5857 2024-05-19 18:30:10.000000 notolog-0.9.1b7/tests/test_notolog_editor.py
--rw-r--r--   0 vadikus    (501) staff       (20)      903 2024-05-12 14:50:00.000000 notolog-0.9.1b7/tests/test_pkg_integration.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2203 2024-05-19 18:30:10.000000 notolog-0.9.1b7/tests/test_qt_async.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1959 2024-05-19 18:30:10.000000 notolog-0.9.1b7/tests/test_settings.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4975 2024-05-11 09:19:41.000000 notolog-0.9.1b7/tests/test_text_block_data.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4461 2024-05-19 18:30:10.000000 notolog-0.9.1b7/tests/test_theme_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6412 2024-05-19 18:30:10.000000 notolog-0.9.1b7/tests/test_themes.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:52:17.444035 notolog-0.9.1b7/tests/ui_tests/
--rw-r--r--   0 vadikus    (501) staff       (20)     1226 2024-05-19 18:30:10.000000 notolog-0.9.1b7/tests/ui_tests/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2544 2024-05-19 18:30:10.000000 notolog-0.9.1b7/tests/ui_tests/test_ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2325 2024-05-19 18:30:10.000000 notolog-0.9.1b7/tests/ui_tests/test_qt_ui.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-25 16:39:30.831169 notolog-0.9.1b8/
+-rw-r--r--   0 vadikus    (501) staff       (20)    10799 2024-05-25 15:57:51.000000 notolog-0.9.1b8/CHANGELOG.md
+-rw-r--r--   0 vadikus    (501) staff       (20)     3490 2024-05-11 12:17:28.000000 notolog-0.9.1b8/CODE_OF_CONDUCT.md
+-rw-r--r--   0 vadikus    (501) staff       (20)     1073 2024-05-04 21:27:31.000000 notolog-0.9.1b8/LICENSE
+-rw-r--r--   0 vadikus    (501) staff       (20)      439 2024-05-25 15:57:51.000000 notolog-0.9.1b8/MANIFEST.in
+-rw-r--r--   0 vadikus    (501) staff       (20)    22891 2024-05-25 16:39:30.830119 notolog-0.9.1b8/PKG-INFO
+-rw-r--r--   0 vadikus    (501) staff       (20)    19947 2024-05-25 15:57:51.000000 notolog-0.9.1b8/README.md
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-25 16:39:30.342524 notolog-0.9.1b8/docs/
+-rw-r--r--   0 vadikus    (501) staff       (20)     8633 2024-05-19 18:30:10.000000 notolog-0.9.1b8/docs/Examples.md
+-rw-r--r--   0 vadikus    (501) staff       (20)   241693 2024-05-19 18:30:10.000000 notolog-0.9.1b8/docs/notolog-ui-settings-strawberry-ja.png
+-rw-r--r--   0 vadikus    (501) staff       (20)   247033 2024-05-04 21:27:32.000000 notolog-0.9.1b8/docs/notolog-ui-settings.png
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-25 16:39:30.391719 notolog-0.9.1b8/notolog/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8787 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/app_config.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-25 16:39:30.405203 notolog-0.9.1b8/notolog/assets/
+-rw-r--r--   0 vadikus    (501) staff       (20)     4202 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/notolog-example-image.png
+-rw-r--r--   0 vadikus    (501) staff       (20)    88211 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/notolog-logo.png
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-25 16:39:30.300826 notolog-0.9.1b8/notolog/assets/themes/
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-25 16:39:30.430247 notolog-0.9.1b8/notolog/assets/themes/calligraphy/
+-rw-r--r--   0 vadikus    (501) staff       (20)      777 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/calligraphy/about_popup.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      365 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/calligraphy/ai_assistant.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2767 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/calligraphy/default.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)       56 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/calligraphy/editor.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2311 2024-05-11 12:17:28.000000 notolog-0.9.1b8/notolog/assets/themes/calligraphy/md.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)      885 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/calligraphy/settings_dialog.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/calligraphy/statusbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     6818 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/calligraphy/styles.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      221 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/calligraphy/toolbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      743 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/calligraphy/tree_view.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       28 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/calligraphy/viewer.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       80 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/calligraphy/viewer.ini
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-25 16:39:30.442006 notolog-0.9.1b8/notolog/assets/themes/default/
+-rw-r--r--   0 vadikus    (501) staff       (20)      798 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/about_popup.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      253 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/ai_assistant.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2775 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/default.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)      174 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/editor.css
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-25 16:39:30.535527 notolog-0.9.1b8/notolog/assets/themes/default/icons/
+-rw-r--r--   0 vadikus    (501) staff       (20)     1093 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/icons/LICENSE
+-rw-r--r--   0 vadikus    (501) staff       (20)      349 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/icons/arrow-clockwise.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      567 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/icons/arrow-repeat.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      736 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/icons/balloon-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      797 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/icons/balloon.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      812 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/icons/bandaid-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      959 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/icons/bandaid.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      528 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/icons/box-arrow-up-right.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      538 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/icons/box-arrow-up.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      265 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/icons/caret-down-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      265 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/icons/caret-up-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      455 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/icons/code-slash.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      694 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/icons/cursor-text.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      459 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/icons/eyedropper.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      403 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/icons/eyeglasses.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      479 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/icons/file-earmark-lock2.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      394 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/icons/file-earmark-plus-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      481 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/icons/file-earmark-x.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      294 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/icons/file-earmark.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      547 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/icons/filetype-html.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      705 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/icons/filetype-md.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      524 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/icons/filetype-txt.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      401 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/icons/floppy2-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      606 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/icons/floppy2.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      428 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/icons/folder-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      708 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/icons/folder-symlink.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      527 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/icons/folder.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      708 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/icons/github.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      518 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/icons/link-45deg.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      666 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/icons/linkedin.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      575 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/icons/pencil-square.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      261 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/icons/power.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      582 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/icons/quote.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      996 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/icons/robot.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      316 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/icons/share-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      653 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/icons/shield-lock-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)     1057 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/icons/shield-lock.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      399 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/icons/star-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      623 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/icons/star.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      272 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/icons/three-dots.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      577 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/icons/trash3-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      656 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/icons/trash3.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      301 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/icons/twitter-x.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      465 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/icons/type-bold.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      351 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/icons/type-italic.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      574 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/icons/type-strikethrough.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      319 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/icons/type-underline.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      351 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/icons/x-circle-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      397 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/icons/x-square-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      491 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/icons/x-square.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)     2363 2024-05-11 12:17:28.000000 notolog-0.9.1b8/notolog/assets/themes/default/md.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)      721 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/settings_dialog.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/statusbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     8472 2024-05-11 12:17:28.000000 notolog-0.9.1b8/notolog/assets/themes/default/styles.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      221 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/toolbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      744 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/tree_view.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       28 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/viewer.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       82 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/default/viewer.ini
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-25 16:39:30.550649 notolog-0.9.1b8/notolog/assets/themes/noir_dark/
+-rw-r--r--   0 vadikus    (501) staff       (20)      777 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/noir_dark/about_popup.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      347 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/noir_dark/ai_assistant.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2745 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/noir_dark/default.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)       56 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/noir_dark/editor.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2480 2024-05-11 12:17:28.000000 notolog-0.9.1b8/notolog/assets/themes/noir_dark/md.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)     1435 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/noir_dark/settings_dialog.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/noir_dark/statusbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     6935 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/noir_dark/styles.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      280 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/noir_dark/toolbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      711 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/noir_dark/tree_view.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       28 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/noir_dark/viewer.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       76 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/noir_dark/viewer.ini
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-25 16:39:30.574982 notolog-0.9.1b8/notolog/assets/themes/strawberry/
+-rw-r--r--   0 vadikus    (501) staff       (20)      790 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/strawberry/about_popup.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      317 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/strawberry/ai_assistant.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2775 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/strawberry/default.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)       50 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/strawberry/editor.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2408 2024-05-11 12:17:28.000000 notolog-0.9.1b8/notolog/assets/themes/strawberry/md.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)      753 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/strawberry/settings_dialog.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/strawberry/statusbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     8451 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/strawberry/styles.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      221 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/strawberry/toolbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      764 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/strawberry/tree_view.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       60 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/strawberry/viewer.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       84 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/assets/themes/strawberry/viewer.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)     3817 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/async_highlighter.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8441 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/edit_widget.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4247 2024-05-19 18:30:10.000000 notolog-0.9.1b8/notolog/editor_state.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-25 16:39:30.602825 notolog-0.9.1b8/notolog/encrypt/
+-rw-r--r--   0 vadikus    (501) staff       (20)      152 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/encrypt/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4345 2024-05-19 18:30:10.000000 notolog-0.9.1b8/notolog/encrypt/enc_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5603 2024-05-19 18:30:10.000000 notolog-0.9.1b8/notolog/encrypt/enc_new_password_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)      626 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/encrypt/enc_password.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3686 2024-05-19 18:30:10.000000 notolog-0.9.1b8/notolog/encrypt/enc_password_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3215 2024-05-19 18:30:10.000000 notolog-0.9.1b8/notolog/encrypt/enc_password_reset_dialog.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-25 16:39:30.610511 notolog-0.9.1b8/notolog/enums/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/enums/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1433 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/enums/ai_model_names.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5624 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/enums/colors.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1125 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/enums/enum_base.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1367 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/enums/languages.py
+-rw-r--r--   0 vadikus    (501) staff       (20)      451 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/enums/themes.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4500 2024-05-19 18:30:10.000000 notolog-0.9.1b8/notolog/etree_extension.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-25 16:39:30.612237 notolog-0.9.1b8/notolog/exceptions/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/exceptions/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)       52 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/exceptions/file_header_empty_exception.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7563 2024-05-19 18:30:10.000000 notolog-0.9.1b8/notolog/file_header.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2860 2024-05-19 18:30:10.000000 notolog-0.9.1b8/notolog/file_system_watcher.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-25 16:39:30.629783 notolog-0.9.1b8/notolog/helpers/
+-rw-r--r--   0 vadikus    (501) staff       (20)       35 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/helpers/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)      187 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/helpers/clipboard_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4221 2024-05-19 18:30:10.000000 notolog-0.9.1b8/notolog/helpers/file_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3669 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/helpers/settings_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5644 2024-05-19 18:30:10.000000 notolog-0.9.1b8/notolog/helpers/theme_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1036 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/helpers/tooltip_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7489 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/helpers/update_helper.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-25 16:39:30.646270 notolog-0.9.1b8/notolog/highlight/
+-rw-r--r--   0 vadikus    (501) staff       (20)      126 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/highlight/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     9349 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/highlight/main_highlighter.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    52061 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/highlight/md_highlighter.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8596 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/highlight/view_highlighter.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    11558 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/image_downloader.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-25 16:39:30.648162 notolog-0.9.1b8/notolog/lexemes/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/__init__.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-25 16:39:30.655200 notolog-0.9.1b8/notolog/lexemes/de/
+-rw-r--r--   0 vadikus    (501) staff       (20)      831 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/lexemes/de/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7202 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/de/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6502 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/lexemes/de/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2267 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/de/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3789 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/lexemes/de/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1225 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/de/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2757 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/de/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-25 16:39:30.660862 notolog-0.9.1b8/notolog/lexemes/en/
+-rw-r--r--   0 vadikus    (501) staff       (20)      828 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/lexemes/en/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7097 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/lexemes/en/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6051 2024-05-11 12:17:28.000000 notolog-0.9.1b8/notolog/lexemes/en/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2181 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/en/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3595 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/lexemes/en/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1201 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/en/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2573 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/en/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-25 16:39:30.670751 notolog-0.9.1b8/notolog/lexemes/es/
+-rw-r--r--   0 vadikus    (501) staff       (20)      891 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/lexemes/es/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7309 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/es/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6476 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/lexemes/es/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2316 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/es/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3891 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/lexemes/es/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1222 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/es/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2793 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/es/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-25 16:39:30.683444 notolog-0.9.1b8/notolog/lexemes/fi/
+-rw-r--r--   0 vadikus    (501) staff       (20)      856 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/fi/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7559 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/fi/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6292 2024-05-11 12:17:28.000000 notolog-0.9.1b8/notolog/lexemes/fi/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2261 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/fi/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3759 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/fi/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1333 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/lexemes/fi/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2662 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/fi/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-25 16:39:30.691687 notolog-0.9.1b8/notolog/lexemes/fr/
+-rw-r--r--   0 vadikus    (501) staff       (20)      887 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/lexemes/fr/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7247 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/fr/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6646 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/lexemes/fr/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2344 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/fr/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3979 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/lexemes/fr/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1236 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/fr/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2824 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/fr/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-25 16:39:30.699545 notolog-0.9.1b8/notolog/lexemes/ge/
+-rw-r--r--   0 vadikus    (501) staff       (20)     1323 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/ge/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    10627 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/ge/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     9593 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/lexemes/ge/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3459 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/ge/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5742 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/ge/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1591 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/lexemes/ge/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4107 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/ge/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-25 16:39:30.705623 notolog-0.9.1b8/notolog/lexemes/gr/
+-rw-r--r--   0 vadikus    (501) staff       (20)     1101 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/lexemes/gr/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8991 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/lexemes/gr/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8542 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/lexemes/gr/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2907 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/gr/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5041 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/lexemes/gr/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1561 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/gr/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3679 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/gr/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-25 16:39:30.711410 notolog-0.9.1b8/notolog/lexemes/in/
+-rw-r--r--   0 vadikus    (501) staff       (20)     1208 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/in/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     9434 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/in/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    10078 2024-05-11 12:17:28.000000 notolog-0.9.1b8/notolog/lexemes/in/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3124 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/in/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5547 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/lexemes/in/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1549 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/in/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3828 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/in/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-25 16:39:30.719676 notolog-0.9.1b8/notolog/lexemes/it/
+-rw-r--r--   0 vadikus    (501) staff       (20)      865 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/lexemes/it/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7263 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/it/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6282 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/lexemes/it/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2303 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/lexemes/it/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3834 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/lexemes/it/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1238 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/it/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2780 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/it/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-25 16:39:30.729281 notolog-0.9.1b8/notolog/lexemes/ja/
+-rw-r--r--   0 vadikus    (501) staff       (20)      932 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/lexemes/ja/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8464 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/ja/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7248 2024-05-11 12:17:28.000000 notolog-0.9.1b8/notolog/lexemes/ja/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2443 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/ja/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4015 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/lexemes/ja/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1242 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/ja/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3000 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/ja/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-25 16:39:30.736063 notolog-0.9.1b8/notolog/lexemes/ko/
+-rw-r--r--   0 vadikus    (501) staff       (20)      849 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/lexemes/ko/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7597 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/ko/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6775 2024-05-11 12:17:28.000000 notolog-0.9.1b8/notolog/lexemes/ko/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2268 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/ko/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3698 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/lexemes/ko/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1221 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/ko/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2666 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/ko/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-25 16:39:30.744559 notolog-0.9.1b8/notolog/lexemes/la/
+-rw-r--r--   0 vadikus    (501) staff       (20)      843 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/lexemes/la/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7538 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/la/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6153 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/lexemes/la/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2297 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/la/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3770 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/lexemes/la/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1257 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/la/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2736 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/la/toolbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3842 2024-05-19 18:30:10.000000 notolog-0.9.1b8/notolog/lexemes/lexemes.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-25 16:39:30.750962 notolog-0.9.1b8/notolog/lexemes/nl/
+-rw-r--r--   0 vadikus    (501) staff       (20)      840 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/nl/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7094 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/nl/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6321 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/lexemes/nl/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2229 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/nl/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3673 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/nl/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1219 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/lexemes/nl/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2647 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/nl/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-25 16:39:30.756902 notolog-0.9.1b8/notolog/lexemes/pt/
+-rw-r--r--   0 vadikus    (501) staff       (20)      899 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/lexemes/pt/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7304 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/pt/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6273 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/lexemes/pt/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2326 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/pt/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3831 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/lexemes/pt/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1223 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/pt/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2830 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/pt/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-25 16:39:30.763062 notolog-0.9.1b8/notolog/lexemes/ru/
+-rw-r--r--   0 vadikus    (501) staff       (20)      998 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/lexemes/ru/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     9135 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/ru/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7848 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/lexemes/ru/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2883 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/ru/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4897 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/lexemes/ru/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1428 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/ru/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3453 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/ru/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-25 16:39:30.774314 notolog-0.9.1b8/notolog/lexemes/se/
+-rw-r--r--   0 vadikus    (501) staff       (20)      835 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/se/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7048 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/se/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6253 2024-05-11 12:17:28.000000 notolog-0.9.1b8/notolog/lexemes/se/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2216 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/se/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3627 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/se/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1220 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/se/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2611 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/se/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-25 16:39:30.782336 notolog-0.9.1b8/notolog/lexemes/tr/
+-rw-r--r--   0 vadikus    (501) staff       (20)      810 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/lexemes/tr/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7402 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/lexemes/tr/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6062 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/lexemes/tr/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2276 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/tr/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3733 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/tr/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1240 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/tr/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2735 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/tr/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-25 16:39:30.789816 notolog-0.9.1b8/notolog/lexemes/zh/
+-rw-r--r--   0 vadikus    (501) staff       (20)      793 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/lexemes/zh/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7074 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/zh/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5777 2024-05-11 12:17:28.000000 notolog-0.9.1b8/notolog/lexemes/zh/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2175 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/zh/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3477 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/lexemes/zh/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1202 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/zh/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2559 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/lexemes/zh/toolbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3608 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/main.py
+-rw-r--r--   0 vadikus    (501) staff       (20)   175821 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/notolog_editor.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7388 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/settings.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3479 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/text_block_data.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5977 2024-05-19 18:30:10.000000 notolog-0.9.1b8/notolog/theme.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-25 16:39:30.808383 notolog-0.9.1b8/notolog/ui/
+-rw-r--r--   0 vadikus    (501) staff       (20)      152 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/ui/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8248 2024-05-19 18:30:10.000000 notolog-0.9.1b8/notolog/ui/about_popup.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    17349 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/ui/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2103 2024-05-19 18:30:10.000000 notolog-0.9.1b8/notolog/ui/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3551 2024-05-19 18:30:10.000000 notolog-0.9.1b8/notolog/ui/common_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1306 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/ui/enum_combo_box.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5602 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/ui/file_system_model.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7178 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/ui/line_numbers.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2606 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/ui/rename_file_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1229 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/ui/rotating_label.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    37497 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/ui/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3248 2024-05-19 18:30:10.000000 notolog-0.9.1b8/notolog/ui/sort_filter_proxy_model.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6949 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/ui/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    12970 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/ui/toolbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)      455 2024-05-11 09:19:41.000000 notolog-0.9.1b8/notolog/ui/vertical_line_spacer.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8324 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/view_decorator.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    16195 2024-05-25 15:57:51.000000 notolog-0.9.1b8/notolog/view_processor.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2452 2024-05-19 18:30:10.000000 notolog-0.9.1b8/notolog/view_widget.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-25 16:39:30.828640 notolog-0.9.1b8/notolog.egg-info/
+-rw-r--r--   0 vadikus    (501) staff       (20)    22891 2024-05-25 16:39:30.000000 notolog-0.9.1b8/notolog.egg-info/PKG-INFO
+-rw-r--r--   0 vadikus    (501) staff       (20)    11754 2024-05-25 16:39:30.000000 notolog-0.9.1b8/notolog.egg-info/SOURCES.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)        1 2024-05-25 16:39:30.000000 notolog-0.9.1b8/notolog.egg-info/dependency_links.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)       46 2024-05-25 16:39:30.000000 notolog-0.9.1b8/notolog.egg-info/entry_points.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)      307 2024-05-25 16:39:30.000000 notolog-0.9.1b8/notolog.egg-info/requires.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)       14 2024-05-25 16:39:30.000000 notolog-0.9.1b8/notolog.egg-info/top_level.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)      307 2024-05-25 15:57:51.000000 notolog-0.9.1b8/requirements.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)       38 2024-05-25 16:39:30.831352 notolog-0.9.1b8/setup.cfg
+-rw-r--r--   0 vadikus    (501) staff       (20)     3239 2024-05-25 15:57:51.000000 notolog-0.9.1b8/setup.py
+-rw-r--r--   0 vadikus    (501) staff       (20)      155 2024-05-25 15:57:51.000000 notolog-0.9.1b8/test_requirements.txt
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-25 16:39:30.823938 notolog-0.9.1b8/tests/
+-rw-r--r--   0 vadikus    (501) staff       (20)      448 2024-05-25 15:57:51.000000 notolog-0.9.1b8/tests/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6152 2024-05-25 15:57:51.000000 notolog-0.9.1b8/tests/test_enc_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2324 2024-05-25 15:57:51.000000 notolog-0.9.1b8/tests/test_enc_password.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    10181 2024-05-25 15:57:51.000000 notolog-0.9.1b8/tests/test_file_header.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3990 2024-05-25 15:57:51.000000 notolog-0.9.1b8/tests/test_html_view.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    11144 2024-05-25 15:57:51.000000 notolog-0.9.1b8/tests/test_image_downloader.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7672 2024-05-25 15:57:51.000000 notolog-0.9.1b8/tests/test_lexemes.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5858 2024-05-25 15:57:51.000000 notolog-0.9.1b8/tests/test_notolog_editor.py
+-rw-r--r--   0 vadikus    (501) staff       (20)      904 2024-05-25 15:57:51.000000 notolog-0.9.1b8/tests/test_pkg_integration.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2394 2024-05-25 15:57:51.000000 notolog-0.9.1b8/tests/test_qt_async.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2159 2024-05-25 15:57:51.000000 notolog-0.9.1b8/tests/test_settings.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4739 2024-05-25 15:57:51.000000 notolog-0.9.1b8/tests/test_settings_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4975 2024-05-11 09:19:41.000000 notolog-0.9.1b8/tests/test_text_block_data.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4689 2024-05-25 15:57:51.000000 notolog-0.9.1b8/tests/test_theme_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6412 2024-05-19 18:30:10.000000 notolog-0.9.1b8/tests/test_themes.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-25 16:39:30.827748 notolog-0.9.1b8/tests/ui_tests/
+-rw-r--r--   0 vadikus    (501) staff       (20)     1123 2024-05-25 15:57:51.000000 notolog-0.9.1b8/tests/ui_tests/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2625 2024-05-25 15:57:51.000000 notolog-0.9.1b8/tests/ui_tests/test_ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2393 2024-05-25 15:57:51.000000 notolog-0.9.1b8/tests/ui_tests/test_qt_ui.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3565 2024-05-25 15:57:51.000000 notolog-0.9.1b8/tests/ui_tests/test_settings_dialog.py
```

### Comparing `notolog-0.9.1b7/CHANGELOG.md` & `notolog-0.9.1b8/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,33 @@
 # Changelog
 All notologable changes to this project will be documented in this file.
 
+## [0.9.1b8] - 2024-05-25
+
+### Added
+- Added `typing_extensions` package, which is also automatically installed with the `emoji` package.
+- New tests and test-related updates, particularly complex async tests for `ImageDownloader`.
+
+### Updated
+- Updated the following packages to their latest versions: `PySide6` (including `PySide6_Addons` and `PySide6_Essentials`) to version 6.7.1, `pytest` to version 8.2.1, `pytest-asyncio` to version 0.23.7, `cffi` to version 1.17.0rc1, and `Emoji lib` to version 2.12.1.
+- Added processing for the Shift + Enter keyboard combination to avoid soft line breaks, which may alter the perception of how soft line breaks function.
+- Updated the package's `setup.py` to include supported languages and additional package information.
+- Updated the functionality for getting and storing protected fields in settings, including refactoring and error fixes (re-setup of corresponding values may be required).
+- Updated `AppConfig` with additional settings-related options.
+- Various `Flake8` linter fixes to ensure the code meets the PEP 8 style guide, along with McCabe complexity updates (current complexity check level is 15).
+- Updated and optimized the content of the `README.md` file to enhance the sections on third-party components, and tests-related topics.
+
+### Changed
+- Slightly reduced the await time for the async highlighter to make the editing mode more responsive to changes involved in syntax highlighting (experimental).
+- Improved the error-proofing of async queue processing upon app closing, particularly if background processes like highlighting or others are still in progress.
+
+### Fixed
+- Fixed an issue where resources might be downloaded twice.
+- Resolved a problem with the toolbar context menu being unresponsive.
+
 ## [0.9.1b5] - 2024-05-19
 
 ### Added
 - Introduced a GitHub workflow for tests, incorporating Flake8 and pytest coverage reports to maintain high standards of code quality and ensure comprehensive test coverage.
 - Added the app's organization name, app name, and version to facilitate correct settings storage.
 - Added a media directory to the app_config.toml.
 - App settings now support encrypted values to keep sensitive data, like API keys, secure. The encryption key is generated once and stored in the app config file. A Settings helper class was also added.
```

### Comparing `notolog-0.9.1b7/CODE_OF_CONDUCT.md` & `notolog-0.9.1b8/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/LICENSE` & `notolog-0.9.1b8/LICENSE`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/PKG-INFO` & `notolog-0.9.1b8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,63 +1,82 @@
 Metadata-Version: 2.1
 Name: notolog
-Version: 0.9.1b7
+Version: 0.9.1b8
 Summary: Notolog - Python Markdown Editor
 Home-page: https://github.com/notolog/notolog-editor
 Author: Vadim Bakhrenkov
 License: MIT
 Project-URL: Bug Reports, https://github.com/notolog/notolog-editor/issues
 Project-URL: Source, https://github.com/notolog/notolog-editor/
 Keywords: notolog,python,markdown,editor,ai,text,notes
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Topic :: Text Editors
 Classifier: Topic :: Text Editors :: Documentation
 Classifier: Topic :: Text Editors :: Emacs
 Classifier: Topic :: Text Editors :: Integrated Development Environments (IDE)
 Classifier: Topic :: Text Editors :: Text Processing
 Classifier: Topic :: Text Editors :: Word Processors
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Text Processing :: General
 Classifier: Topic :: Text Processing :: Markup :: Markdown
+Classifier: Natural Language :: Chinese (Simplified)
+Classifier: Natural Language :: Dutch
+Classifier: Natural Language :: English
+Classifier: Natural Language :: Finnish
+Classifier: Natural Language :: French
+Classifier: Natural Language :: Georgian
+Classifier: Natural Language :: German
+Classifier: Natural Language :: Greek
+Classifier: Natural Language :: Hindi
+Classifier: Natural Language :: Italian
+Classifier: Natural Language :: Japanese
+Classifier: Natural Language :: Korean
+Classifier: Natural Language :: Latin
+Classifier: Natural Language :: Portuguese
+Classifier: Natural Language :: Russian
+Classifier: Natural Language :: Spanish
+Classifier: Natural Language :: Swedish
+Classifier: Natural Language :: Turkish
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: cffi==1.16.0
+Requires-Dist: cffi==1.17.0rc1
 Requires-Dist: click==8.1.7
 Requires-Dist: cryptography==42.0.7
-Requires-Dist: emoji==2.11.1
+Requires-Dist: emoji==2.12.1
 Requires-Dist: iniconfig==2.0.0
 Requires-Dist: Markdown==3.6
 Requires-Dist: packaging==24.0
 Requires-Dist: pluggy==1.5.0
 Requires-Dist: pycparser==2.22
 Requires-Dist: Pygments==2.18.0
-Requires-Dist: PySide6==6.7.0
-Requires-Dist: PySide6_Addons==6.7.0
-Requires-Dist: PySide6_Essentials==6.7.0
-Requires-Dist: pytest==8.2.0
-Requires-Dist: pytest-asyncio==0.23.6
-Requires-Dist: pytest-mock==3.14.0
+Requires-Dist: PySide6==6.7.1
+Requires-Dist: PySide6_Addons==6.7.1
+Requires-Dist: PySide6_Essentials==6.7.1
 Requires-Dist: qasync==0.27.1
-Requires-Dist: shiboken6==6.7.0
+Requires-Dist: shiboken6==6.7.1
 Requires-Dist: tomli==2.0.1
 Requires-Dist: tomli_w==1.0.0
+Requires-Dist: typing_extensions==4.12.0
 
-<!-- {"notolog.app": {"created": "2023-12-25 18:59:43.806614", "updated": "2024-05-19 23:29:34.439703"}} -->
+<!-- {"notolog.app": {"created": "2023-12-25 18:59:43.806614", "updated": "2024-05-25 16:38:26.173086"}} -->
 # Notolog
 
 ![Notolog - Python Markdown Editor](https://raw.githubusercontent.com/notolog/notolog-editor/main/notolog/assets/notolog-example-image.png)
 
 ## Python Markdown Editor
 
 [![PyPI - Version](https://img.shields.io/pypi/v/notolog)](https://pypi.org/project/notolog/) [![GitHub License](https://img.shields.io/github/license/notolog/notolog-editor)](https://github.com/notolog/notolog-editor/blob/master/LICENSE) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/notolog)](https://pypi.org/project/notolog/) [![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/notolog/notolog-editor/tests.yaml)](https://github.com/notolog/notolog-editor/actions/workflows/tests.yaml)
@@ -131,14 +150,15 @@
 * Swedish
 * Turkish
 
 Here's an example of what it looks like in the actual UI, featuring the lovely Strawberry theme and Japanese translation:
 
 ![Notolog UI translation example](https://raw.githubusercontent.com/notolog/notolog-editor/main/docs/notolog-ui-settings-strawberry-ja.png)
 
+
 ## Prerequisites
 
 **Python 3.9 or higher installed on your system.**
 
 Ensure Python 3.9 or higher is installed on your system. Visit [python.org](https://python.org) for more details.
 
 Check the version of Python available with this command `python3 -V`.
@@ -178,25 +198,47 @@
 
 ```sh
 pip install -r requirements.txt
 ```
 
 That's it! Starting the app is as simple as `python -m notolog.main` form the project's root directory.
 
+### Tests and Test Coverage
+
+To minimize installation overhead and streamline dependency management, dependencies required solely for testing are isolated in `test_requirements.txt`. This separation helps manage test dependencies independently from the main application dependencies.
+
+```sh
+pip install -r test_requirements.txt
+```
+
 <details>
-<summary>Run tests</summary>
+<summary>Run Tests</summary>
 
-To run all available tests:
+To execute all available tests:
 ```sh
 pytest
 ```
 
-To run a particular file's tests:
+To run tests from a specific file:
 ```sh
-pytest tests/test_notolog_editor.py
+pytest tests/test_pkg_integration.py
+```
+</details>
+
+<details>
+<summary>Run Tests with Coverage Reports</summary>
+
+To run all tests with a coverage report:
+```sh
+pytest tests/ --cov=notolog --cov-report=term
+```
+
+Alternatively, to exclude UI tests from execution:
+```sh
+pytest tests/ --cov=notolog --cov-report=term --ignore=tests/ui_tests/
 ```
 </details>
 
 ### Virtual Environments
 
 The instructions below contain steps of how to set up **venv** virtual environment to run a Python app safely. Starting from Python 3.6 **venv** is a recommended way to create virtual environments. For more information check [Creation of virtual environments](https://docs.python.org/3/library/venv.html). Alternatively, you can execute the Notolog code and set up virtual environment with your favorite Python code editor.
 
@@ -260,110 +302,116 @@
 _Mind the environment name (**notolog** or any other selected before)._
 
 
 ## Contributing
 
 If you encounter any issues or would like to contribute to the project, please don't hesitate to [open an issue](https://github.com/notolog/notolog-editor/issues) or submit a [pull request](https://github.com/notolog/notolog-editor/pulls) on the project's [GitHub page](https://github.com/notolog/notolog-editor).
 
+
 ## License
 
 The Notolog project is licensed under the MIT License - see the [LICENSE](https://github.com/notolog/notolog-editor/blob/main/LICENSE) file for details.
 
+
 ## Third-Party Components
 
 ### Libraries and Licenses
 
-This project utilizes numerous third-party libraries, each with its own licensing terms. Below is a detailed list of these libraries grouped by license type to help clarify what each license permits and requires. This categorization aids in ensuring compliance with legal terms for use, modification, and distribution of these software components.
+This project incorporates numerous third-party libraries, each subject to its own licensing terms. Below is a detailed list of these libraries, categorized by license type to facilitate understanding of what each license permits and requires. This organization helps ensure compliance with legal terms for the use, modification, and distribution of these components.
 
 #### GNU LGPLv3, GNU GPLv2, or Commercial License
 
-- **Qt (open-source)**: Framework for graphical user interfaces and more. [Project Details](https://www.qt.io), [Qt Licensing](https://www.qt.io/licensing)
-- **PySide6**: GUI creation with Qt6 in Python. [Project and License Details](https://pyside.org/), [PyPI](https://pypi.org/project/PySide6/)
-- **PySide6_Addons**: Additional modules for PySide6. [Project and License Details](https://pyside.org/), [PyPI](https://pypi.org/project/PySide6-Addons/)
+- **Qt (open-source)**: A framework for graphical user interfaces and more. [Project Details](https://www.qt.io), [Qt Licensing](https://www.qt.io/licensing)
+- **PySide6**: Enables GUI creation with Qt6 in Python. [Project and License Details](https://pyside.org/), [PyPI](https://pypi.org/project/PySide6/)
+- **PySide6_Addons**: Provides additional modules for PySide6. [Project and License Details](https://pyside.org/), [PyPI](https://pypi.org/project/PySide6-Addons/)
 - **PySide6_Essentials**: Core libraries for PySide6. [Project and License Details](https://pyside.org/), [PyPI](https://pypi.org/project/PySide6-Essentials/)
-- **shiboken6**: Binding generator for Qt framework. [Project and License Details](https://pyside.org/), [PyPI](https://pypi.org/project/shiboken6/)
+- **shiboken6**: Binding generator for the Qt framework. [Project and License Details](https://pyside.org/), [PyPI](https://pypi.org/project/shiboken6/)
 
 #### MIT License
 
 - **Bootstrap Icons**: Icons for UI elements. [Project Details](https://icons.getbootstrap.com/), [License Details](https://github.com/twbs/icons/blob/main/LICENSE)
-- **pytest**: Used for unit testing. It provides powerful features like fixtures, assertions, and test parameterization to facilitate writing and running Python tests. [Project Details](https://pytest.org/), [License Details](https://docs.pytest.org/en/8.0.x/license.html)
-- **pytest-mock**: Enhances pytest for unit tests by offering a simple interface to powerful mocking functionalities. [License Details](https://github.com/pytest-dev/pytest-mock/blob/main/LICENSE), [PyPI](https://pypi.org/project/pytest-mock/)
-- **cffi**: Used for interfacing with C code. [License Details](https://github.com/python-cffi/cffi/blob/main/LICENSE), [PyPI](https://pypi.org/project/cffi/)
-- **iniconfig**: For parsing and working with INI configuration files. [License Details](https://github.com/pytest-dev/iniconfig/blob/main/LICENSE), [PyPI](https://pypi.org/project/iniconfig/)
-- **tomli**: A Python library used for parsing TOML configuration files effortlessly. [License Details](https://github.com/hukkin/tomli/blob/master/LICENSE), [PyPI](https://pypi.org/project/tomli/)
-- **tomli_w**: A Python library used for writing TOML configuration files effortlessly. [License Details](https://github.com/hukkin/tomli-w/blob/master/LICENSE), [PyPI](https://pypi.org/project/tomli-w/)
-- **pluggy**: For creating and managing plugin systems in Python applications. [License Details](https://github.com/pytest-dev/pluggy/blob/main/LICENSE), [PyPI](https://pypi.org/project/pluggy/)
+- **cffi**: For interfacing with C code. [License Details](https://github.com/python-cffi/cffi/blob/main/LICENSE), [PyPI](https://pypi.org/project/cffi/)
+- **iniconfig**: For parsing and managing INI configuration files. [License Details](https://github.com/pytest-dev/iniconfig/blob/main/LICENSE), [PyPI](https://pypi.org/project/iniconfig/)
+- **tomli**: Effortlessly parses TOML configuration files. [License Details](https://github.com/hukkin/tomli/blob/master/LICENSE), [PyPI](https://pypi.org/project/tomli/)
+- **tomli_w**: For writing TOML configuration files effortlessly. [License Details](https://github.com/hukkin/tomli-w/blob/master/LICENSE), [PyPI](https://pypi.org/project/tomli-w/)
+- **pluggy**: Facilitates the creation and management of plugin systems. [License Details](https://github.com/pytest-dev/pluggy/blob/main/LICENSE), [PyPI](https://pypi.org/project/pluggy/)
 
 #### BSD Licenses
 
-- **Python-Markdown**: Markdown to HTML conversion. [Project Details](https://python-markdown.github.io/), [BSD 3-Clause License](https://github.com/Python-Markdown/markdown/blob/master/LICENSE.md)
-- **Emoji library**: Converts emoji text-code to emojis. [New BSD License](https://github.com/carpedm20/emoji/blob/master/LICENSE.txt), [PyPI](https://pypi.org/project/emoji/)
-- **qasync**: Async support for Python. [BSD 2-Clause "Simplified" License](https://github.com/CabbageDevelopment/qasync/blob/master/LICENSE), [PyPI](https://pypi.org/project/qasync/)
-- **Pygments**: Syntax highlighting for programming languages. [Project Details](https://pygments.org/), [BSD 2-Clause "Simplified" License](https://github.com/pygments/pygments/blob/master/LICENSE)
-- **click**: Used for creating command-line interfaces. [Project Details](https://palletsprojects.com/p/click/), [BSD-3-Clause License](https://click.palletsprojects.com/en/8.1.x/license/)
-- **pycparser**: C code parser and for generating Abstract Syntax Trees (AST) in Python. [BSD 3-Clause License](https://github.com/eliben/pycparser/blob/main/LICENSE), [PyPI](https://pypi.org/project/pycparser/)
-
-#### Apache License 2.0
-
-- **pytest-asyncio**: A library that provides support for testing asyncio code with pytest. [License Details](https://github.com/pytest-dev/pytest-asyncio/blob/main/LICENSE) , [PyPI](https://pypi.org/project/pytest-asyncio/)
+- **Python-Markdown**: Converts Markdown to HTML. [Project Details](https://python-markdown.github.io/), [BSD 3-Clause License](https://github.com/Python-Markdown/markdown/blob/master/LICENSE.md)
+- **Emoji library**: Converts emoji text-codes to emojis. [New BSD License](https://github.com/carpedm20/emoji/blob/master/LICENSE.txt), [PyPI](https://pypi.org/project/emoji/)
+- **qasync**: Adds async support to Python. [BSD 2-Clause "Simplified" License](https://github.com/CabbageDevelopment/qasync/blob/master/LICENSE), [PyPI](https://pypi.org/project/qasync/)
+- **Pygments**: Provides syntax highlighting for programming languages. [Project Details](https://pygments.org/), [BSD 2-Clause "Simplified" License](https://github.com/pygments/pygments/blob/master/LICENSE)
+- **click**: Creates command-line interfaces. [Project Details](https://palletsprojects.com/p/click/), [BSD-3-Clause License](https://click.palletsprojects.com/en/8.1.x/license/)
+- **pycparser**: A C code parser; generates Abstract Syntax Trees in Python. [BSD 3-Clause License](https://github.com/eliben/pycparser/blob/main/LICENSE), [PyPI](https://pypi.org/project/pycparser/)
 
 #### Other Dual Licensed
 
 - **cryptography**: Provides cryptographic functions and primitives. [Apache License 2.0](https://github.com/pyca/cryptography/blob/main/LICENSE.APACHE) and [BSD 3-Clause License](https://github.com/pyca/cryptography/blob/main/LICENSE.BSD), [PyPI](https://pypi.org/project/cryptography/)
-- **packaging**: Python package metadata and distribution utilities. [Apache License 2.0](https://github.com/pypa/packaging/blob/main/LICENSE.APACHE) and [BSD 2-Clause "Simplified" License](https://github.com/pypa/packaging/blob/main/LICENSE.BSD), [PyPI](https://pypi.org/project/packaging/)
-
-#### Python Standard Library
+- **packaging**: Handles metadata and distribution for Python packages. [Apache License 2.0](https://github.com/pypa/packaging/blob/main/LICENSE.APACHE) and [BSD 2-Clause "Simplified" License](https://github.com/pypa/packaging/blob/main/LICENSE.BSD), [PyPI](https://pypi.org/project/packaging/)
 
-- **asyncio**: Part of the Python standard library, licensed under the [Python Software Foundation License](https://docs.python.org/3/license.html#psf-license).
+#### Python Software Foundation License
+- **typing_extensions**: Enhances support for type hints on older versions of Python. Licensed under the [Python Software Foundation License](https://github.com/python/typing_extensions/blob/main/LICENSE), [PyPI](https://pypi.org/project/typing-extensions/).
+- **Standard Python Libraries**: Includes commonly used libraries such as `asyncio` and `unittest`. All are part of the Python standard library and are licensed under the [Python Software Foundation License](https://docs.python.org/3/license.html#psf-license). This includes any other standard libraries not explicitly mentioned but used in the project.
 
 #### The Unlicense
 
-- **Codehilite CSS Themes**: Base themes for code highlighting. [The Unlicense](https://github.com/richleland/pygments-css/blob/master/UNLICENSE.txt)
+- **Codehilite CSS Themes**: Basic themes for code highlighting. [The Unlicense](https://github.com/richleland/pygments-css/blob/master/UNLICENSE.txt)
 
 Please note that while the majority of this project is licensed under the MIT License, certain components may have different licensing terms. Always refer to the documentation of each library for detailed information about its license and terms of use.
 
+
 ### APIs
 
 #### OpenAI API Disclaimer
 
 **Disclaimer:** This project is independent and not affiliated with, endorsed by, or sponsored by OpenAI. The integration of the OpenAI API is provided on an "as is" basis, and the creators disclaim all liability for any misuse or consequences resulting from the use of the OpenAI API.
 
 **Usage:** This project uses the OpenAI API to access AI assistant capabilities and enhance natural language processing. Users must provide their own OpenAI API keys and should refer to the [OpenAI API reference](https://platform.openai.com/docs/api-reference) for detailed usage guidelines.
 
 **Responsibility:** Users are responsible for obtaining and managing their OpenAI API keys in compliance with OpenAI's terms of service.
 
 **Security:** Users are expected to handle their API keys securely to avoid unauthorized access.
 
 *This section was generated with the assistance of AI to ensure accurate and concise information regarding the use of the OpenAI API.*
 
+
 ## Security Disclaimer
 
 This application is designed for educational purposes and offers security features through optional file encryption and protected application settings.
 
 ### Optional File Encryption
 
-* **Encryption Details:** The application uses PBKDF2HMAC for key derivation and Fernet for encryption, utilizing AES-128 in CBC mode. Although the key material generated is 256 bits, only the first 128 bits (16 bytes) are used for encryption.
-* **File Headers:** The encryption salt and iteration counts are stored unencrypted in the file's header. This approach is primarily intended for non-critical applications where data exposure has limited risk.
-* **Strong Passwords:** Users are encouraged to use strong passwords to enhance the protection of their encrypted data.
+- **Encryption Details**: The application uses PBKDF2HMAC for key derivation and Fernet for encryption, utilizing AES-128 in CBC mode. Although the key material generated is 256 bits, only the first 128 bits (16 bytes) are used for encryption.
+- **File Headers**: The encryption salt and iteration counts are stored unencrypted in the file's header. This approach is primarily intended for non-critical applications where data exposure has limited risk.
+- **Strong Passwords**: Users are encouraged to use strong passwords to enhance the protection of their encrypted data.
 
 ### Protected Application Settings
 
-* **Settings Encryption:** The application may encrypt sensitive data like API keys because these Qt app settings might otherwise be stored as open data. However, the encryption key used is stored on the PC and can be accessed by anyone with physical or user-level access to the computer. This could expose sensitive data to potential unauthorized access.
+- **Settings Encryption**: The application may encrypt sensitive data like API keys because these Qt app settings might otherwise be stored as open data. However, the encryption key used is stored on the PC and can be accessed by anyone with physical or user-level access to the computer. This could expose sensitive data to potential unauthorized access.
 
 ### General Information
 
-* **Open Source:** This application is open-source and distributed under the MIT License. Users must comply with applicable laws and regulations when using this software.
-* **Liability:** The developers disclaim any liability for misuse or legal non-compliance related to the use of this software.
+- **Open Source**: This application is open-source and distributed under the MIT License. Users must comply with applicable laws and regulations when using this software.
+- **Liability**: The developers disclaim any liability for misuse or legal non-compliance related to the use of this software.
 
 
-## Code Quality and Test Coverage
+## Development and Testing Tools
 
 To maintain high standards of code quality and ensure comprehensive test coverage, we use several tools:
 
-- **Flake8**: A tool that enforces coding style and checks the quality of Python code by combining PyFlakes, pycodestyle, and McCabe's complexity checker. [MIT License](https://github.com/PyCQA/flake8/blob/main/LICENSE)
-- **coverage**: Measures the effectiveness of tests by showing which parts of your code are being executed and which are not. [Apache License 2.0](https://github.com/nedbat/coveragepy/blob/master/LICENSE.txt)
-- **pytest-cov**: A pytest plugin that provides test coverage reports, extending pytest to measure code coverage alongside running tests. [MIT License](https://github.com/pytest-dev/pytest-cov/blob/master/LICENSE)
+- **coverage**: Measures the code coverage of our tests, helping to ensure that all parts of the application are properly tested. [License](https://github.com/nedbat/coveragepy/blob/master/LICENSE.txt), [PyPI](https://pypi.org/project/coverage/).
+- **flake8**: A tool that enforces coding style and checks the quality of Python code by combining PyFlakes, pycodestyle, and McCabe's complexity checker. [MIT License](https://github.com/PyCQA/flake8/blob/main/LICENSE), [PyPI](https://pypi.org/project/flake8/).
+  - **mccabe**: Analyzes code complexity, which can help in identifying overly complex code that may need simplification. [License](https://github.com/PyCQA/mccabe/blob/master/LICENSE), [PyPI](https://pypi.org/project/mccabe/).
+  - **pycodestyle**: A tool to check Python code against coding style conventions in PEP 8. [License](https://github.com/PyCQA/pycodestyle/blob/main/LICENSE), [PyPI](https://pypi.org/project/pycodestyle/).
+  - **pyflakes**: Analyzes Python programs and detects various errors like undefined names. [License](https://github.com/PyCQA/pyflakes/blob/main/LICENSE), [PyPI](https://pypi.org/project/pyflakes/).
+- **pytest**: Provides a powerful framework for writing and running Python tests, including support for complex test setups. [License](https://docs.pytest.org/en/8.0.x/license.html), [PyPI](https://pypi.org/project/pytest/).
+- **pytest-asyncio**: Enables testing of asyncio Python code with pytest, making it easier to test asynchronous functions and classes. [License](https://github.com/pytest-dev/pytest-asyncio/blob/main/LICENSE), [PyPI](https://pypi.org/project/pytest-asyncio/).
+- **pytest-cov**: A pytest plugin that produces test coverage reports, showing how well the tests cover the code. [License](https://github.com/pytest-dev/pytest-cov/blob/master/LICENSE), [PyPI](https://pypi.org/project/pytest-cov/).
+- **pytest-mock**: Enhances pytest with mock functionality for unit tests, providing a simpler interface to powerful mocking tools. [License](https://github.com/pytest-dev/pytest-mock/blob/main/LICENSE), [PyPI](https://pypi.org/project/pytest-mock/).
+
+### Additional Notes
 
-These tools help us maintain a clean and reliable codebase by catching potential issues early and documenting where our tests might be lacking.
+These tools are essential for maintaining high standards of code quality and ensuring that all functionality is robustly tested. For each package, the versions listed within the `test_requirements.txt` are those currently in use; updates may be applied as newer versions are released.
 
 ---
 _This README.md file has been carefully crafted and edited using the Notolog editor itself._
```

### Comparing `notolog-0.9.1b7/README.md` & `notolog-0.9.1b8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!-- {"notolog.app": {"created": "2023-12-25 18:59:43.806614", "updated": "2024-05-19 23:29:34.439703"}} -->
+<!-- {"notolog.app": {"created": "2023-12-25 18:59:43.806614", "updated": "2024-05-25 16:38:26.173086"}} -->
 # Notolog
 
 ![Notolog - Python Markdown Editor](https://raw.githubusercontent.com/notolog/notolog-editor/main/notolog/assets/notolog-example-image.png)
 
 ## Python Markdown Editor
 
 [![PyPI - Version](https://img.shields.io/pypi/v/notolog)](https://pypi.org/project/notolog/) [![GitHub License](https://img.shields.io/github/license/notolog/notolog-editor)](https://github.com/notolog/notolog-editor/blob/master/LICENSE) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/notolog)](https://pypi.org/project/notolog/) [![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/notolog/notolog-editor/tests.yaml)](https://github.com/notolog/notolog-editor/actions/workflows/tests.yaml)
@@ -76,14 +76,15 @@
 * Swedish
 * Turkish
 
 Here's an example of what it looks like in the actual UI, featuring the lovely Strawberry theme and Japanese translation:
 
 ![Notolog UI translation example](https://raw.githubusercontent.com/notolog/notolog-editor/main/docs/notolog-ui-settings-strawberry-ja.png)
 
+
 ## Prerequisites
 
 **Python 3.9 or higher installed on your system.**
 
 Ensure Python 3.9 or higher is installed on your system. Visit [python.org](https://python.org) for more details.
 
 Check the version of Python available with this command `python3 -V`.
@@ -123,25 +124,47 @@
 
 ```sh
 pip install -r requirements.txt
 ```
 
 That's it! Starting the app is as simple as `python -m notolog.main` form the project's root directory.
 
+### Tests and Test Coverage
+
+To minimize installation overhead and streamline dependency management, dependencies required solely for testing are isolated in `test_requirements.txt`. This separation helps manage test dependencies independently from the main application dependencies.
+
+```sh
+pip install -r test_requirements.txt
+```
+
 <details>
-<summary>Run tests</summary>
+<summary>Run Tests</summary>
 
-To run all available tests:
+To execute all available tests:
 ```sh
 pytest
 ```
 
-To run a particular file's tests:
+To run tests from a specific file:
 ```sh
-pytest tests/test_notolog_editor.py
+pytest tests/test_pkg_integration.py
+```
+</details>
+
+<details>
+<summary>Run Tests with Coverage Reports</summary>
+
+To run all tests with a coverage report:
+```sh
+pytest tests/ --cov=notolog --cov-report=term
+```
+
+Alternatively, to exclude UI tests from execution:
+```sh
+pytest tests/ --cov=notolog --cov-report=term --ignore=tests/ui_tests/
 ```
 </details>
 
 ### Virtual Environments
 
 The instructions below contain steps of how to set up **venv** virtual environment to run a Python app safely. Starting from Python 3.6 **venv** is a recommended way to create virtual environments. For more information check [Creation of virtual environments](https://docs.python.org/3/library/venv.html). Alternatively, you can execute the Notolog code and set up virtual environment with your favorite Python code editor.
 
@@ -205,110 +228,116 @@
 _Mind the environment name (**notolog** or any other selected before)._
 
 
 ## Contributing
 
 If you encounter any issues or would like to contribute to the project, please don't hesitate to [open an issue](https://github.com/notolog/notolog-editor/issues) or submit a [pull request](https://github.com/notolog/notolog-editor/pulls) on the project's [GitHub page](https://github.com/notolog/notolog-editor).
 
+
 ## License
 
 The Notolog project is licensed under the MIT License - see the [LICENSE](https://github.com/notolog/notolog-editor/blob/main/LICENSE) file for details.
 
+
 ## Third-Party Components
 
 ### Libraries and Licenses
 
-This project utilizes numerous third-party libraries, each with its own licensing terms. Below is a detailed list of these libraries grouped by license type to help clarify what each license permits and requires. This categorization aids in ensuring compliance with legal terms for use, modification, and distribution of these software components.
+This project incorporates numerous third-party libraries, each subject to its own licensing terms. Below is a detailed list of these libraries, categorized by license type to facilitate understanding of what each license permits and requires. This organization helps ensure compliance with legal terms for the use, modification, and distribution of these components.
 
 #### GNU LGPLv3, GNU GPLv2, or Commercial License
 
-- **Qt (open-source)**: Framework for graphical user interfaces and more. [Project Details](https://www.qt.io), [Qt Licensing](https://www.qt.io/licensing)
-- **PySide6**: GUI creation with Qt6 in Python. [Project and License Details](https://pyside.org/), [PyPI](https://pypi.org/project/PySide6/)
-- **PySide6_Addons**: Additional modules for PySide6. [Project and License Details](https://pyside.org/), [PyPI](https://pypi.org/project/PySide6-Addons/)
+- **Qt (open-source)**: A framework for graphical user interfaces and more. [Project Details](https://www.qt.io), [Qt Licensing](https://www.qt.io/licensing)
+- **PySide6**: Enables GUI creation with Qt6 in Python. [Project and License Details](https://pyside.org/), [PyPI](https://pypi.org/project/PySide6/)
+- **PySide6_Addons**: Provides additional modules for PySide6. [Project and License Details](https://pyside.org/), [PyPI](https://pypi.org/project/PySide6-Addons/)
 - **PySide6_Essentials**: Core libraries for PySide6. [Project and License Details](https://pyside.org/), [PyPI](https://pypi.org/project/PySide6-Essentials/)
-- **shiboken6**: Binding generator for Qt framework. [Project and License Details](https://pyside.org/), [PyPI](https://pypi.org/project/shiboken6/)
+- **shiboken6**: Binding generator for the Qt framework. [Project and License Details](https://pyside.org/), [PyPI](https://pypi.org/project/shiboken6/)
 
 #### MIT License
 
 - **Bootstrap Icons**: Icons for UI elements. [Project Details](https://icons.getbootstrap.com/), [License Details](https://github.com/twbs/icons/blob/main/LICENSE)
-- **pytest**: Used for unit testing. It provides powerful features like fixtures, assertions, and test parameterization to facilitate writing and running Python tests. [Project Details](https://pytest.org/), [License Details](https://docs.pytest.org/en/8.0.x/license.html)
-- **pytest-mock**: Enhances pytest for unit tests by offering a simple interface to powerful mocking functionalities. [License Details](https://github.com/pytest-dev/pytest-mock/blob/main/LICENSE), [PyPI](https://pypi.org/project/pytest-mock/)
-- **cffi**: Used for interfacing with C code. [License Details](https://github.com/python-cffi/cffi/blob/main/LICENSE), [PyPI](https://pypi.org/project/cffi/)
-- **iniconfig**: For parsing and working with INI configuration files. [License Details](https://github.com/pytest-dev/iniconfig/blob/main/LICENSE), [PyPI](https://pypi.org/project/iniconfig/)
-- **tomli**: A Python library used for parsing TOML configuration files effortlessly. [License Details](https://github.com/hukkin/tomli/blob/master/LICENSE), [PyPI](https://pypi.org/project/tomli/)
-- **tomli_w**: A Python library used for writing TOML configuration files effortlessly. [License Details](https://github.com/hukkin/tomli-w/blob/master/LICENSE), [PyPI](https://pypi.org/project/tomli-w/)
-- **pluggy**: For creating and managing plugin systems in Python applications. [License Details](https://github.com/pytest-dev/pluggy/blob/main/LICENSE), [PyPI](https://pypi.org/project/pluggy/)
+- **cffi**: For interfacing with C code. [License Details](https://github.com/python-cffi/cffi/blob/main/LICENSE), [PyPI](https://pypi.org/project/cffi/)
+- **iniconfig**: For parsing and managing INI configuration files. [License Details](https://github.com/pytest-dev/iniconfig/blob/main/LICENSE), [PyPI](https://pypi.org/project/iniconfig/)
+- **tomli**: Effortlessly parses TOML configuration files. [License Details](https://github.com/hukkin/tomli/blob/master/LICENSE), [PyPI](https://pypi.org/project/tomli/)
+- **tomli_w**: For writing TOML configuration files effortlessly. [License Details](https://github.com/hukkin/tomli-w/blob/master/LICENSE), [PyPI](https://pypi.org/project/tomli-w/)
+- **pluggy**: Facilitates the creation and management of plugin systems. [License Details](https://github.com/pytest-dev/pluggy/blob/main/LICENSE), [PyPI](https://pypi.org/project/pluggy/)
 
 #### BSD Licenses
 
-- **Python-Markdown**: Markdown to HTML conversion. [Project Details](https://python-markdown.github.io/), [BSD 3-Clause License](https://github.com/Python-Markdown/markdown/blob/master/LICENSE.md)
-- **Emoji library**: Converts emoji text-code to emojis. [New BSD License](https://github.com/carpedm20/emoji/blob/master/LICENSE.txt), [PyPI](https://pypi.org/project/emoji/)
-- **qasync**: Async support for Python. [BSD 2-Clause "Simplified" License](https://github.com/CabbageDevelopment/qasync/blob/master/LICENSE), [PyPI](https://pypi.org/project/qasync/)
-- **Pygments**: Syntax highlighting for programming languages. [Project Details](https://pygments.org/), [BSD 2-Clause "Simplified" License](https://github.com/pygments/pygments/blob/master/LICENSE)
-- **click**: Used for creating command-line interfaces. [Project Details](https://palletsprojects.com/p/click/), [BSD-3-Clause License](https://click.palletsprojects.com/en/8.1.x/license/)
-- **pycparser**: C code parser and for generating Abstract Syntax Trees (AST) in Python. [BSD 3-Clause License](https://github.com/eliben/pycparser/blob/main/LICENSE), [PyPI](https://pypi.org/project/pycparser/)
-
-#### Apache License 2.0
-
-- **pytest-asyncio**: A library that provides support for testing asyncio code with pytest. [License Details](https://github.com/pytest-dev/pytest-asyncio/blob/main/LICENSE) , [PyPI](https://pypi.org/project/pytest-asyncio/)
+- **Python-Markdown**: Converts Markdown to HTML. [Project Details](https://python-markdown.github.io/), [BSD 3-Clause License](https://github.com/Python-Markdown/markdown/blob/master/LICENSE.md)
+- **Emoji library**: Converts emoji text-codes to emojis. [New BSD License](https://github.com/carpedm20/emoji/blob/master/LICENSE.txt), [PyPI](https://pypi.org/project/emoji/)
+- **qasync**: Adds async support to Python. [BSD 2-Clause "Simplified" License](https://github.com/CabbageDevelopment/qasync/blob/master/LICENSE), [PyPI](https://pypi.org/project/qasync/)
+- **Pygments**: Provides syntax highlighting for programming languages. [Project Details](https://pygments.org/), [BSD 2-Clause "Simplified" License](https://github.com/pygments/pygments/blob/master/LICENSE)
+- **click**: Creates command-line interfaces. [Project Details](https://palletsprojects.com/p/click/), [BSD-3-Clause License](https://click.palletsprojects.com/en/8.1.x/license/)
+- **pycparser**: A C code parser; generates Abstract Syntax Trees in Python. [BSD 3-Clause License](https://github.com/eliben/pycparser/blob/main/LICENSE), [PyPI](https://pypi.org/project/pycparser/)
 
 #### Other Dual Licensed
 
 - **cryptography**: Provides cryptographic functions and primitives. [Apache License 2.0](https://github.com/pyca/cryptography/blob/main/LICENSE.APACHE) and [BSD 3-Clause License](https://github.com/pyca/cryptography/blob/main/LICENSE.BSD), [PyPI](https://pypi.org/project/cryptography/)
-- **packaging**: Python package metadata and distribution utilities. [Apache License 2.0](https://github.com/pypa/packaging/blob/main/LICENSE.APACHE) and [BSD 2-Clause "Simplified" License](https://github.com/pypa/packaging/blob/main/LICENSE.BSD), [PyPI](https://pypi.org/project/packaging/)
-
-#### Python Standard Library
+- **packaging**: Handles metadata and distribution for Python packages. [Apache License 2.0](https://github.com/pypa/packaging/blob/main/LICENSE.APACHE) and [BSD 2-Clause "Simplified" License](https://github.com/pypa/packaging/blob/main/LICENSE.BSD), [PyPI](https://pypi.org/project/packaging/)
 
-- **asyncio**: Part of the Python standard library, licensed under the [Python Software Foundation License](https://docs.python.org/3/license.html#psf-license).
+#### Python Software Foundation License
+- **typing_extensions**: Enhances support for type hints on older versions of Python. Licensed under the [Python Software Foundation License](https://github.com/python/typing_extensions/blob/main/LICENSE), [PyPI](https://pypi.org/project/typing-extensions/).
+- **Standard Python Libraries**: Includes commonly used libraries such as `asyncio` and `unittest`. All are part of the Python standard library and are licensed under the [Python Software Foundation License](https://docs.python.org/3/license.html#psf-license). This includes any other standard libraries not explicitly mentioned but used in the project.
 
 #### The Unlicense
 
-- **Codehilite CSS Themes**: Base themes for code highlighting. [The Unlicense](https://github.com/richleland/pygments-css/blob/master/UNLICENSE.txt)
+- **Codehilite CSS Themes**: Basic themes for code highlighting. [The Unlicense](https://github.com/richleland/pygments-css/blob/master/UNLICENSE.txt)
 
 Please note that while the majority of this project is licensed under the MIT License, certain components may have different licensing terms. Always refer to the documentation of each library for detailed information about its license and terms of use.
 
+
 ### APIs
 
 #### OpenAI API Disclaimer
 
 **Disclaimer:** This project is independent and not affiliated with, endorsed by, or sponsored by OpenAI. The integration of the OpenAI API is provided on an "as is" basis, and the creators disclaim all liability for any misuse or consequences resulting from the use of the OpenAI API.
 
 **Usage:** This project uses the OpenAI API to access AI assistant capabilities and enhance natural language processing. Users must provide their own OpenAI API keys and should refer to the [OpenAI API reference](https://platform.openai.com/docs/api-reference) for detailed usage guidelines.
 
 **Responsibility:** Users are responsible for obtaining and managing their OpenAI API keys in compliance with OpenAI's terms of service.
 
 **Security:** Users are expected to handle their API keys securely to avoid unauthorized access.
 
 *This section was generated with the assistance of AI to ensure accurate and concise information regarding the use of the OpenAI API.*
 
+
 ## Security Disclaimer
 
 This application is designed for educational purposes and offers security features through optional file encryption and protected application settings.
 
 ### Optional File Encryption
 
-* **Encryption Details:** The application uses PBKDF2HMAC for key derivation and Fernet for encryption, utilizing AES-128 in CBC mode. Although the key material generated is 256 bits, only the first 128 bits (16 bytes) are used for encryption.
-* **File Headers:** The encryption salt and iteration counts are stored unencrypted in the file's header. This approach is primarily intended for non-critical applications where data exposure has limited risk.
-* **Strong Passwords:** Users are encouraged to use strong passwords to enhance the protection of their encrypted data.
+- **Encryption Details**: The application uses PBKDF2HMAC for key derivation and Fernet for encryption, utilizing AES-128 in CBC mode. Although the key material generated is 256 bits, only the first 128 bits (16 bytes) are used for encryption.
+- **File Headers**: The encryption salt and iteration counts are stored unencrypted in the file's header. This approach is primarily intended for non-critical applications where data exposure has limited risk.
+- **Strong Passwords**: Users are encouraged to use strong passwords to enhance the protection of their encrypted data.
 
 ### Protected Application Settings
 
-* **Settings Encryption:** The application may encrypt sensitive data like API keys because these Qt app settings might otherwise be stored as open data. However, the encryption key used is stored on the PC and can be accessed by anyone with physical or user-level access to the computer. This could expose sensitive data to potential unauthorized access.
+- **Settings Encryption**: The application may encrypt sensitive data like API keys because these Qt app settings might otherwise be stored as open data. However, the encryption key used is stored on the PC and can be accessed by anyone with physical or user-level access to the computer. This could expose sensitive data to potential unauthorized access.
 
 ### General Information
 
-* **Open Source:** This application is open-source and distributed under the MIT License. Users must comply with applicable laws and regulations when using this software.
-* **Liability:** The developers disclaim any liability for misuse or legal non-compliance related to the use of this software.
+- **Open Source**: This application is open-source and distributed under the MIT License. Users must comply with applicable laws and regulations when using this software.
+- **Liability**: The developers disclaim any liability for misuse or legal non-compliance related to the use of this software.
 
 
-## Code Quality and Test Coverage
+## Development and Testing Tools
 
 To maintain high standards of code quality and ensure comprehensive test coverage, we use several tools:
 
-- **Flake8**: A tool that enforces coding style and checks the quality of Python code by combining PyFlakes, pycodestyle, and McCabe's complexity checker. [MIT License](https://github.com/PyCQA/flake8/blob/main/LICENSE)
-- **coverage**: Measures the effectiveness of tests by showing which parts of your code are being executed and which are not. [Apache License 2.0](https://github.com/nedbat/coveragepy/blob/master/LICENSE.txt)
-- **pytest-cov**: A pytest plugin that provides test coverage reports, extending pytest to measure code coverage alongside running tests. [MIT License](https://github.com/pytest-dev/pytest-cov/blob/master/LICENSE)
+- **coverage**: Measures the code coverage of our tests, helping to ensure that all parts of the application are properly tested. [License](https://github.com/nedbat/coveragepy/blob/master/LICENSE.txt), [PyPI](https://pypi.org/project/coverage/).
+- **flake8**: A tool that enforces coding style and checks the quality of Python code by combining PyFlakes, pycodestyle, and McCabe's complexity checker. [MIT License](https://github.com/PyCQA/flake8/blob/main/LICENSE), [PyPI](https://pypi.org/project/flake8/).
+  - **mccabe**: Analyzes code complexity, which can help in identifying overly complex code that may need simplification. [License](https://github.com/PyCQA/mccabe/blob/master/LICENSE), [PyPI](https://pypi.org/project/mccabe/).
+  - **pycodestyle**: A tool to check Python code against coding style conventions in PEP 8. [License](https://github.com/PyCQA/pycodestyle/blob/main/LICENSE), [PyPI](https://pypi.org/project/pycodestyle/).
+  - **pyflakes**: Analyzes Python programs and detects various errors like undefined names. [License](https://github.com/PyCQA/pyflakes/blob/main/LICENSE), [PyPI](https://pypi.org/project/pyflakes/).
+- **pytest**: Provides a powerful framework for writing and running Python tests, including support for complex test setups. [License](https://docs.pytest.org/en/8.0.x/license.html), [PyPI](https://pypi.org/project/pytest/).
+- **pytest-asyncio**: Enables testing of asyncio Python code with pytest, making it easier to test asynchronous functions and classes. [License](https://github.com/pytest-dev/pytest-asyncio/blob/main/LICENSE), [PyPI](https://pypi.org/project/pytest-asyncio/).
+- **pytest-cov**: A pytest plugin that produces test coverage reports, showing how well the tests cover the code. [License](https://github.com/pytest-dev/pytest-cov/blob/master/LICENSE), [PyPI](https://pypi.org/project/pytest-cov/).
+- **pytest-mock**: Enhances pytest with mock functionality for unit tests, providing a simpler interface to powerful mocking tools. [License](https://github.com/pytest-dev/pytest-mock/blob/main/LICENSE), [PyPI](https://pypi.org/project/pytest-mock/).
+
+### Additional Notes
 
-These tools help us maintain a clean and reliable codebase by catching potential issues early and documenting where our tests might be lacking.
+These tools are essential for maintaining high standards of code quality and ensuring that all functionality is robustly tested. For each package, the versions listed within the `test_requirements.txt` are those currently in use; updates may be applied as newer versions are released.
 
 ---
 _This README.md file has been carefully crafted and edited using the Notolog editor itself._
```

### Comparing `notolog-0.9.1b7/docs/Examples.md` & `notolog-0.9.1b8/docs/Examples.md`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/docs/notolog-ui-settings-strawberry-ja.png` & `notolog-0.9.1b8/docs/notolog-ui-settings-strawberry-ja.png`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/docs/notolog-ui-settings.png` & `notolog-0.9.1b8/docs/notolog-ui-settings.png`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/app_config.py` & `notolog-0.9.1b8/notolog/app_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,29 +7,34 @@
 
 from typing import Any
 from threading import Lock
 
 toml_base_app_config = """
 [app]
 name = "Notolog"
-version = "0.9.1b7"
+version = "0.9.1b8"
 license = "MIT License"
 date = "2024"
 website = "https://notolog.app"
 repository = "https://github.com/notolog/notolog-editor"
 pypi = "https://pypi.org/project/notolog"
 author = "Vadim Bakhrenkov"
 
 [repository]
 
     [repository.github]
     username = "notolog"
     project = "notolog-editor"
     release_url = "https://api.github.com/repos/notolog/notolog-editor/releases/latest"
     bug_report_url = "https://github.com/notolog/notolog-editor/issues"
+
+[settings]
+org_name = "Notolog"
+org_domain = "notolog.app"
+app_name = "notolog_editor"
 """
 
 toml_app_config_header = """# Notolog
 # An open-source markdown editor developed in Python.
 
 # Application-Level Configuration
 # --------------------------------
@@ -197,14 +202,26 @@
 
     def get_repository_github_release_url(self) -> str:
         return self.base_app_config['repository']['github']['release_url']
 
     def get_repository_github_bug_report_url(self) -> str:
         return self.base_app_config['repository']['github']['bug_report_url']
 
+    def get_settings_org_name(self) -> str:
+        return self.base_app_config['settings']['org_name']
+
+    def get_settings_org_domain(self) -> str:
+        return self.base_app_config['settings']['org_domain']
+
+    def get_settings_app_name(self) -> str:
+        return self.base_app_config['settings']['app_name']
+
+    def get_settings_app_name_qa(self) -> str:
+        return f"{self.base_app_config['settings']['app_name']}_qa"
+
     def get_font_base_size(self) -> int:
         return self.app_config['font']['base_size']
 
     def get_editor_media_dir(self) -> str:
         return self.app_config['editor']['media_dir']
 
     """
```

### Comparing `notolog-0.9.1b7/notolog/assets/notolog-example-image.png` & `notolog-0.9.1b8/notolog/assets/notolog-example-image.png`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/assets/notolog-logo.png` & `notolog-0.9.1b8/notolog/assets/notolog-logo.png`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/assets/themes/calligraphy/about_popup.css` & `notolog-0.9.1b8/notolog/assets/themes/calligraphy/about_popup.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/assets/themes/calligraphy/default.ini` & `notolog-0.9.1b8/notolog/assets/themes/calligraphy/default.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/assets/themes/calligraphy/md.ini` & `notolog-0.9.1b8/notolog/assets/themes/calligraphy/md.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/assets/themes/calligraphy/settings_dialog.css` & `notolog-0.9.1b8/notolog/assets/themes/calligraphy/settings_dialog.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/assets/themes/calligraphy/styles.css` & `notolog-0.9.1b8/notolog/assets/themes/calligraphy/styles.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/assets/themes/calligraphy/tree_view.css` & `notolog-0.9.1b8/notolog/assets/themes/calligraphy/tree_view.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/assets/themes/default/about_popup.css` & `notolog-0.9.1b8/notolog/assets/themes/default/about_popup.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/assets/themes/default/default.ini` & `notolog-0.9.1b8/notolog/assets/themes/default/default.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/assets/themes/default/icons/LICENSE` & `notolog-0.9.1b8/notolog/assets/themes/default/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/assets/themes/default/icons/arrow-repeat.svg` & `notolog-0.9.1b8/notolog/assets/themes/default/icons/arrow-repeat.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/assets/themes/default/icons/balloon-fill.svg` & `notolog-0.9.1b8/notolog/assets/themes/default/icons/balloon-fill.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/assets/themes/default/icons/balloon.svg` & `notolog-0.9.1b8/notolog/assets/themes/default/icons/balloon.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/assets/themes/default/icons/bandaid-fill.svg` & `notolog-0.9.1b8/notolog/assets/themes/default/icons/bandaid-fill.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/assets/themes/default/icons/bandaid.svg` & `notolog-0.9.1b8/notolog/assets/themes/default/icons/bandaid.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/assets/themes/default/icons/box-arrow-up-right.svg` & `notolog-0.9.1b8/notolog/assets/themes/default/icons/box-arrow-up-right.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/assets/themes/default/icons/box-arrow-up.svg` & `notolog-0.9.1b8/notolog/assets/themes/default/icons/box-arrow-up.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/assets/themes/default/icons/cursor-text.svg` & `notolog-0.9.1b8/notolog/assets/themes/default/icons/cursor-text.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/assets/themes/default/icons/filetype-html.svg` & `notolog-0.9.1b8/notolog/assets/themes/default/icons/filetype-html.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/assets/themes/default/icons/filetype-md.svg` & `notolog-0.9.1b8/notolog/assets/themes/default/icons/filetype-md.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/assets/themes/default/icons/filetype-txt.svg` & `notolog-0.9.1b8/notolog/assets/themes/default/icons/filetype-txt.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/assets/themes/default/icons/floppy2.svg` & `notolog-0.9.1b8/notolog/assets/themes/default/icons/floppy2.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/assets/themes/default/icons/folder-symlink.svg` & `notolog-0.9.1b8/notolog/assets/themes/default/icons/folder-symlink.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/assets/themes/default/icons/folder.svg` & `notolog-0.9.1b8/notolog/assets/themes/default/icons/folder.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/assets/themes/default/icons/github.svg` & `notolog-0.9.1b8/notolog/assets/themes/default/icons/github.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/assets/themes/default/icons/link-45deg.svg` & `notolog-0.9.1b8/notolog/assets/themes/default/icons/link-45deg.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/assets/themes/default/icons/linkedin.svg` & `notolog-0.9.1b8/notolog/assets/themes/default/icons/linkedin.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/assets/themes/default/icons/pencil-square.svg` & `notolog-0.9.1b8/notolog/assets/themes/default/icons/pencil-square.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/assets/themes/default/icons/quote.svg` & `notolog-0.9.1b8/notolog/assets/themes/default/icons/quote.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/assets/themes/default/icons/robot.svg` & `notolog-0.9.1b8/notolog/assets/themes/default/icons/robot.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/assets/themes/default/icons/shield-lock-fill.svg` & `notolog-0.9.1b8/notolog/assets/themes/default/icons/shield-lock-fill.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/assets/themes/default/icons/shield-lock.svg` & `notolog-0.9.1b8/notolog/assets/themes/default/icons/shield-lock.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/assets/themes/default/icons/star.svg` & `notolog-0.9.1b8/notolog/assets/themes/default/icons/star.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/assets/themes/default/icons/trash3-fill.svg` & `notolog-0.9.1b8/notolog/assets/themes/default/icons/trash3-fill.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/assets/themes/default/icons/trash3.svg` & `notolog-0.9.1b8/notolog/assets/themes/default/icons/trash3.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/assets/themes/default/icons/type-strikethrough.svg` & `notolog-0.9.1b8/notolog/assets/themes/default/icons/type-strikethrough.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/assets/themes/default/md.ini` & `notolog-0.9.1b8/notolog/assets/themes/default/md.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/assets/themes/default/settings_dialog.css` & `notolog-0.9.1b8/notolog/assets/themes/default/settings_dialog.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/assets/themes/default/styles.css` & `notolog-0.9.1b8/notolog/assets/themes/default/styles.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/assets/themes/default/tree_view.css` & `notolog-0.9.1b8/notolog/assets/themes/default/tree_view.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/assets/themes/noir_dark/about_popup.css` & `notolog-0.9.1b8/notolog/assets/themes/noir_dark/about_popup.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/assets/themes/noir_dark/default.ini` & `notolog-0.9.1b8/notolog/assets/themes/noir_dark/default.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/assets/themes/noir_dark/md.ini` & `notolog-0.9.1b8/notolog/assets/themes/noir_dark/md.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/assets/themes/noir_dark/settings_dialog.css` & `notolog-0.9.1b8/notolog/assets/themes/noir_dark/settings_dialog.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/assets/themes/noir_dark/styles.css` & `notolog-0.9.1b8/notolog/assets/themes/noir_dark/styles.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/assets/themes/noir_dark/tree_view.css` & `notolog-0.9.1b8/notolog/assets/themes/noir_dark/tree_view.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/assets/themes/strawberry/about_popup.css` & `notolog-0.9.1b8/notolog/assets/themes/strawberry/about_popup.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/assets/themes/strawberry/default.ini` & `notolog-0.9.1b8/notolog/assets/themes/strawberry/default.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/assets/themes/strawberry/md.ini` & `notolog-0.9.1b8/notolog/assets/themes/strawberry/md.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/assets/themes/strawberry/settings_dialog.css` & `notolog-0.9.1b8/notolog/assets/themes/strawberry/settings_dialog.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/assets/themes/strawberry/styles.css` & `notolog-0.9.1b8/notolog/assets/themes/strawberry/styles.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/assets/themes/strawberry/tree_view.css` & `notolog-0.9.1b8/notolog/assets/themes/strawberry/tree_view.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/async_highlighter.py` & `notolog-0.9.1b8/notolog/async_highlighter.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,16 +24,24 @@
         self.rehighlight_tasks = []
 
         self.loop = asyncio.get_event_loop()
 
     @asyncSlot()
     async def rehighlight_in_queue(self, full_rehighlight: bool = False) -> Any:
         """
+        Re-highlight code asynchronously here.
         More info about asyncio tasks: https://docs.python.org/3/library/asyncio-task.html
         """
+
+        # Check async loop is running
+        if not asyncio.get_event_loop().is_running():
+            if self.logging:
+                self.logger.debug('Async loop is not running, skip task')
+            return
+
         if self.debug:
             self.logger.debug('Re-highlight %d tasks in queue' % len(self.rehighlight_tasks))
 
         postpone = False if len(self.rehighlight_tasks) == 0 else True
         if self.debug:
             self.logger.debug('Re-highlight is to postpone "%r"' % postpone)
 
@@ -43,57 +51,53 @@
             task = asyncio.ensure_future(self.rehighlight_async(full_rehighlight, postpone))
             # task = asyncio.create_task(self.rehighlight_async(full_rehighlight, postpone))
             # Add task to the local pool first
             self.rehighlight_tasks.append(task)
             # Callback method to set up further actions
             task.add_done_callback(lambda _task: self.rehighlight_task_callback(_task))
 
-        done, pending = await asyncio.wait(
-            self.rehighlight_tasks,
-            return_when=asyncio.ALL_COMPLETED,  # There is no pending tasks check
-        )
-
-        if self.debug:
-            self.logger.debug(f'Re-highlight tasks progress. Done {len(done)}, pending {len(pending)}')
+        try:
+            done, pending = await asyncio.wait(
+                self.rehighlight_tasks,
+                return_when=asyncio.ALL_COMPLETED,  # There is no pending tasks check
+            )
+            if self.debug:
+                self.logger.debug(f'Re-highlight tasks progress. Done {len(done)}, pending {len(pending)}')
+        except asyncio.CancelledError:
+            # All tasks will be cancelled later upon close event
+            pass
 
         return task
 
     def rehighlight_task_callback(self, task) -> None:
         if self.debug:
             self.logger.debug('%s from total %d completed with callback'
                               % (task.get_name(), len(self.rehighlight_tasks)))
 
         self.rehighlight_tasks.remove(task)
 
         if len(self.rehighlight_tasks) == 0:
-            QTimer.singleShot(750, lambda: self.callback(True))
+            QTimer.singleShot(500, lambda: self.callback(True))
 
     async def rehighlight_async(self, full_rehighlight: bool = False, postpone: bool = False) -> None:
         """
         Run this method not too often to avoid overwhelming the system.
         """
-        # Postpone before re-highlighting set
-        if postpone:
+        try:
+            # Postpone before re-highlighting set
+            if postpone:
+                if self.debug:
+                    self.logger.debug('Re-highlighting the text > postpone')
+                # Keep this method particular amount of time to avoid overwhelming
+                await asyncio.sleep(0.15, self.loop)
+            # Re-highlight
+            self.callback(full_rehighlight)
+            if self.debug:
+                self.logger.debug('Async re-highlighting queue task processed')
+            # Postpone after re-highlighting to keep the queue busy
             if self.debug:
-                self.logger.debug('Re-highlighting the text > postpone')
+                self.logger.debug('Re-highlighting the text > wait to return')
             # Keep this method particular amount of time to avoid overwhelming
-            await asyncio.sleep(0.25, self.loop)
-        # Re-highlight
-        self.callback(full_rehighlight)
-        if self.debug:
-            self.logger.debug('Async re-highlighting queue task processed')
-        # Postpone after re-highlighting to keep the queue busy
-        if self.debug:
-            self.logger.debug('Re-highlighting the text > wait to return')
-        # Keep this method particular amount of time to avoid overwhelming
-        await asyncio.sleep(0.5, self.loop)
-
-    async def cancel_tasks(self):
-        tasks_total = len(self.rehighlight_tasks)
-        for i, task in enumerate(self.rehighlight_tasks):
-            if not task.done():
-                task_res = task.cancel()
-                if self.logging:
-                    self.logger.info(
-                        f'[{i + 1}/{tasks_total}] Pending task "{task.get_name()}" canceled with result "{task_res}"')
-                # Gather all tasks to ensure they are completed before closing
-                await asyncio.gather(*self.rehighlight_tasks, return_exceptions=True)
+            await asyncio.sleep(0.3, self.loop)
+        except asyncio.CancelledError:
+            # All tasks will be cancelled later upon close event
+            pass
```

### Comparing `notolog-0.9.1b7/notolog/edit_widget.py` & `notolog-0.9.1b8/notolog/edit_widget.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from typing import TYPE_CHECKING, Union
 
 from .app_config import AppConfig
 
 import logging
 
 if TYPE_CHECKING:
-    from PySide6.QtGui import QTextBlockUserData  # noqa
-    from .text_block_data import TextBlockData  # noqa
+    from PySide6.QtGui import QTextBlockUserData  # noqa: F401
+    from .text_block_data import TextBlockData  # noqa: F401
 
 
 class EditWidget(QPlainTextEdit):
     # Class to extend or to modify of the original QPlainTextEdit
 
     content_set = Signal()
 
@@ -31,14 +31,19 @@
         self.setFont(font)
 
         self.logger = logging.getLogger('edit_widget')
 
         self.logging = AppConfig().get_logging()
         self.debug = AppConfig().get_debug()
 
+        # Disable line wrapping
+        # self.setLineWrapMode(QPlainTextEdit.LineWrapMode.NoWrap)
+        # Disable word wrapping
+        # self.setWordWrapMode(QTextOption.WrapMode.NoWrap)
+
     def setDocument(self, document):
         # Override setDocument() to allow additional actions like emit the document set signal
         super().setDocument(document)
         # Emit document set signal to notify listeners
         self.content_set.emit()
 
     def setPlainText(self, text):
@@ -80,19 +85,22 @@
         """
         This method handle key press events.
 
         Args:
             event (QKeyEvent): Event object
         """
         if event.key() == Qt.Key.Key_Backtab:
-            """
-            Shift + Tab action to shift the text block left either on a one tab or 4 spaces.
-            """
+            # Shift + Tab action to shift the text block left either on a one tab or 4 spaces.
             self.process_back_tab()
+        elif event.key() == Qt.Key.Key_Return and (event.modifiers() & Qt.KeyboardModifier.ShiftModifier):
+            # Process Shift + Enter combination to allow Enter-style behaviour
+            self.insertPlainText("\n")
+            event.accept()
         else:
+            # Default behavior for all other key events
             return QPlainTextEdit.keyPressEvent(self, event)
 
     def process_back_tab(self) -> None:
         """
         Shift the text block left either on a one tab or 4 spaces.
         """
         find_cursor = self.textCursor()
```

### Comparing `notolog-0.9.1b7/notolog/editor_state.py` & `notolog-0.9.1b8/notolog/editor_state.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/encrypt/enc_helper.py` & `notolog-0.9.1b8/notolog/encrypt/enc_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/encrypt/enc_new_password_dialog.py` & `notolog-0.9.1b8/notolog/encrypt/enc_new_password_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/encrypt/enc_password.py` & `notolog-0.9.1b8/notolog/encrypt/enc_password.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/encrypt/enc_password_dialog.py` & `notolog-0.9.1b8/notolog/encrypt/enc_password_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/encrypt/enc_password_reset_dialog.py` & `notolog-0.9.1b8/notolog/encrypt/enc_password_reset_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/enums/ai_model_names.py` & `notolog-0.9.1b8/notolog/enums/ai_model_names.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/enums/colors.py` & `notolog-0.9.1b8/notolog/enums/colors.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/enums/enum_base.py` & `notolog-0.9.1b8/notolog/enums/enum_base.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/enums/languages.py` & `notolog-0.9.1b8/notolog/enums/languages.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/etree_extension.py` & `notolog-0.9.1b8/notolog/etree_extension.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/file_header.py` & `notolog-0.9.1b8/notolog/file_header.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/file_system_watcher.py` & `notolog-0.9.1b8/notolog/file_system_watcher.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/helpers/file_helper.py` & `notolog-0.9.1b8/notolog/helpers/file_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/helpers/settings_helper.py` & `notolog-0.9.1b8/notolog/helpers/settings_helper.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,29 +3,30 @@
 
 from . import AppConfig
 
 from typing import Union
 
 import os
 import logging
-import base64
 
 
 class SettingsHelper:
     """
     Settings helper to perform additional operations like encrypting/decrypting sensitive data with
     symmetric encryption algorithm to store it in settings, as settings file may be exposed.
     """
 
+    env_secret_name = "NOTOLOG_APP_SECRET_KEY"
+
     def __init__(self):
         super().__init__()
 
         self.logger = logging.getLogger('settings_helper')
 
-        self.logging = AppConfig().get_logging()  # TODO check
+        self.logging = AppConfig().get_logging()
         self.debug = AppConfig().get_debug()
 
         if self.debug:
             self.logger.info('Settings helper is engaged')
 
         self.key = self.get_app_key()
 
@@ -49,42 +50,53 @@
         except (InvalidToken, InvalidSignature, TypeError) as e:
             if self.logging:
                 self.logger.warning(f'Settings helper encryption token error: {e}')
         return None
 
     def get_app_key(self) -> bytes:
         # Get the key from the system env first
-        app_key = os.getenv("NOTOLOG_APP_SECRET_KEY")
+        app_key_str = os.getenv(self.env_secret_name)
 
         # Trying to access key via the app config
-        if app_key is None:
-            app_key = AppConfig().get_security_app_secret()
-            if app_key:
+        if app_key_str is None:
+            app_key_str = AppConfig().get_security_app_secret()
+            if app_key_str:
                 # Store key with system envs
-                os.environ["NOTOLOG_APP_SECRET_KEY"] = app_key
+                os.environ[self.env_secret_name] = app_key_str
 
         # If no key found create a new one
-        if not app_key:
+        if not app_key_str:
             if self.logging:
                 self.logger.info("Creating app new secret key")
-            # Generate app new key
+            # Generate app new key. This is a base64-encoded bytes string
             app_key = self.generate_app_key()
-            # Encode this binary data to a Base64 string (still bytes)
-            encoded_key = base64.urlsafe_b64encode(app_key)
-            # Convert bytes to a string (decoding by ASCII)
-            encoded_key_str = encoded_key.decode('ascii')
-            # Store key in system envs
-            os.environ["NOTOLOG_APP_SECRET_KEY"] = encoded_key_str
-            # Store key in app config
-            AppConfig().set_security_app_secret(encoded_key_str)
-            # Return new key
+            # Set up app new key
+            self.setup_app_key(app_key)
+            # Return new 32 url-safe base64-encoded bytes key
             return app_key
         else:
             # Convert the retrieved string back to bytes
-            app_key_bytes = app_key.encode('ascii')
-            # Decode the Base64 bytes back to the original binary data
-            return base64.urlsafe_b64decode(app_key_bytes)
+            return app_key_str.encode('ascii')
+
+    def setup_app_key(self, app_key: bytes) -> None:
+        # Convert bytes to a string (decoding by ASCII)
+        app_key_str = app_key.decode('ascii')
+        # Store key in system envs
+        os.environ[self.env_secret_name] = app_key_str
+        # Store key in app config
+        AppConfig().set_security_app_secret(app_key_str)
 
     @staticmethod
     def generate_app_key() -> bytes:
         # Generate a key without password, for app needs.
         return Fernet.generate_key()
+
+    def _recreate_app_key(self):
+        """
+        Proof-of-Concept method; Avoid to use it in scenarios different from data repairing.
+        """
+        _new_app_key = self.generate_app_key()
+        self.setup_app_key(_new_app_key)
+        self.key = _new_app_key
+        # Update settings value(s) upon that
+        # value = self.encrypt_data(value)
+        # settings.setValue(param_name, value)
```

### Comparing `notolog-0.9.1b7/notolog/helpers/theme_helper.py` & `notolog-0.9.1b8/notolog/helpers/theme_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/helpers/tooltip_helper.py` & `notolog-0.9.1b8/notolog/helpers/tooltip_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/helpers/update_helper.py` & `notolog-0.9.1b8/notolog/helpers/update_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from . import AppConfig
 
 from ..settings import Settings
 from ..lexemes.lexemes import Lexemes
 
 if TYPE_CHECKING:
-    from PySide6.QtCore import QByteArray  # noqa
+    from PySide6.QtCore import QByteArray  # noqa: F401
 
 
 class UpdateHelper(QObject):
     """
     # How to use example:
     update_helper = UpdateHelper()
     update_helper.new_version_available.connect(lambda v:
@@ -75,76 +75,15 @@
         if self.debug:
             self.logger.debug(f'Update response, reply: {reply}, error_code: {error_code}, status_code: {status_code}')
 
         reply.deleteLater()  # Clean up the QNetworkReply object
 
         # Make sure there is no error
         if reply.error() == QNetworkReply.NetworkError.NoError:
-            # The request was successful
-            data = reply.readAll()  # type: QByteArray
-            """
-            # Or like this:
-            data = reply.readAll().data().decode('utf-8')
-            json_data = json.loads(data)
-            """
-
-            if self.debug:
-                self.logger.debug(f'Raw RESPONSE [{status_code}]: {data}')
-
-            # json_document = QJsonDocument.fromJson(data)
-            # json_data = json_document.object()
-
-            # Convert QByteArray to string
-            res_string = data.toStdString()  # Or: str(data.data(), encoding='utf-8')
-            if self.debug:
-                self.logger.debug(f'Result multi-line STRING: {res_string}')
-
-            # Clean up the string and make one line
-            json_str = ''.join(line.strip() for line in res_string.splitlines())
-
-            if self.debug:
-                self.logger.debug(f'Result STRING: {json_str}')
-
-            result_message = self.lexemes.get('network_connection_error_empty')
-            # Parse JSON response
-            try:
-                json_data = json.loads(json_str)
-                if self.debug:
-                    self.logger.debug(f"Result JSON: {json_data}")
-
-                latest_version_str = json_data['tag_name']
-                latest_version = version.parse(latest_version_str)
-
-                if latest_version > self.current_version:
-                    update_link = ('<a href="%s">%s</a>'
-                                   % (AppConfig().get_repository_github_release_url(), latest_version))
-                    result_message = self.lexemes.get('update_helper_new_version_is_available',
-                                                      latest_version=update_link)
-                    if self.logging:
-                        self.logger.info("New version of the app is available: %s. Current version is %s. Response: %s}"
-                                         % (latest_version, self.current_version, reply.errorString()))
-                    # Emit the new version signal
-                    self.new_version_check_response.emit(
-                        {'status': self.STATUS_OK, 'msg': result_message,
-                         'current_version': self.current_version,
-                         # Check new version by this var
-                         'new_version': latest_version_str})
-                else:
-                    result_message = self.lexemes.get('update_helper_latest_version_installed')
-                    if self.logging:
-                        self.logger.info(
-                            "No new version of the app is available, the current version is %s. Response: %s}"
-                            % (self.current_version, reply.errorString()))
-                    # Emit the same version signal
-                    self.new_version_check_response.emit(
-                        {'status': self.STATUS_OK, 'msg': result_message, 'current_version': self.current_version})
-
-            except json.JSONDecodeError as e:
-                if self.logging:
-                    self.logger.warning("Error decoding JSON: %s" % e)
+            result_message = self.process_response(reply, status_code)
         elif reply.error() == QNetworkReply.NetworkError.HostNotFoundError:
             # The host was not found, indicating possible DNS issues or no internet connection
             result_message = self.lexemes.get('network_connection_error_connection_or_dns')
         elif reply.error() == QNetworkReply.NetworkError.ConnectionRefusedError:
             # Connection was refused, indicating the server might be down or there are network issues
             result_message = self.lexemes.get('network_connection_error_connection_refused')
         elif reply.error() == QNetworkReply.NetworkError.TimeoutError:
@@ -160,7 +99,71 @@
 
         if error_code is not None:
             if self.logging:
                 self.logger.warning(result_message)
                 self.logger.warning(f"Failed to fetch update information: {reply.errorString()}")
             # Emit error signal
             self.new_version_check_response.emit({'status': self.STATUS_ERROR, 'msg': result_message})
+
+    def process_response(self, reply: QNetworkReply, status_code) -> str:
+        # The request was successful
+        data = reply.readAll()  # type: QByteArray
+        # Or like this:
+        # data = reply.readAll().data().decode('utf-8')
+        # json_data = json.loads(data)
+
+        if self.debug:
+            self.logger.debug(f'Raw RESPONSE [{status_code}]: {data}')
+
+        # json_document = QJsonDocument.fromJson(data)
+        # json_data = json_document.object()
+
+        # Convert QByteArray to string
+        res_string = data.toStdString()  # Or: str(data.data(), encoding='utf-8')
+        if self.debug:
+            self.logger.debug(f'Result multi-line STRING: {res_string}')
+
+        # Clean up the string and make one line
+        json_str = ''.join(line.strip() for line in res_string.splitlines())
+
+        if self.debug:
+            self.logger.debug(f'Result STRING: {json_str}')
+
+        result_message = self.lexemes.get('network_connection_error_empty')
+        # Parse JSON response
+        try:
+            json_data = json.loads(json_str)
+            if self.debug:
+                self.logger.debug(f"Result JSON: {json_data}")
+
+            latest_version_str = json_data['tag_name']
+            latest_version = version.parse(latest_version_str)
+
+            if latest_version > self.current_version:
+                update_link = ('<a href="%s">%s</a>'
+                               % (AppConfig().get_repository_github_release_url(), latest_version))
+                result_message = self.lexemes.get('update_helper_new_version_is_available',
+                                                  latest_version=update_link)
+                if self.logging:
+                    self.logger.info("New version of the app is available: %s. Current version is %s. Response: %s}"
+                                     % (latest_version, self.current_version, reply.errorString()))
+                # Emit the new version signal
+                self.new_version_check_response.emit(
+                    {'status': self.STATUS_OK, 'msg': result_message,
+                     'current_version': self.current_version,
+                     # Check new version by this var
+                     'new_version': latest_version_str})
+            else:
+                result_message = self.lexemes.get('update_helper_latest_version_installed')
+                if self.logging:
+                    self.logger.info(
+                        "No new version of the app is available, the current version is %s. Response: %s}"
+                        % (self.current_version, reply.errorString()))
+                # Emit the same version signal
+                self.new_version_check_response.emit(
+                    {'status': self.STATUS_OK, 'msg': result_message, 'current_version': self.current_version})
+
+        except json.JSONDecodeError as e:
+            if self.logging:
+                self.logger.warning("Error decoding JSON: %s" % e)
+
+        return result_message
```

### Comparing `notolog-0.9.1b7/notolog/highlight/main_highlighter.py` & `notolog-0.9.1b8/notolog/highlight/main_highlighter.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,25 +11,29 @@
 # - PyPI: https://pypi.org/project/notolog
 # - WebSite: https://notolog.app
 # - Author: Vadim Bakhrenkov
 # - Copyright 2024 Vadim Bakhrenkov
 # - License: MIT License
 
 from PySide6.QtCore import Qt, QRegularExpression
-from PySide6.QtGui import QTextDocument, QSyntaxHighlighter, QTextBlockUserData, QTextBlock, QTextCharFormat
+from PySide6.QtGui import QTextDocument, QSyntaxHighlighter, QTextCharFormat
 from PySide6.QtGui import QColor, QBrush, QFont
 
-from typing import Union
+from typing import TYPE_CHECKING
 
 from . import AppConfig
-from . import TextBlockData
 from . import ThemeHelper
 
 import logging
 
+if TYPE_CHECKING:
+    from typing import Union  # noqa: F401
+    from . import TextBlockData  # noqa: F401
+    from PySide6.QtGui import QTextBlock, QTextBlockUserData  # noqa: F401
+
 
 class MainHighlighter(QSyntaxHighlighter):
     """
     Syntax highlighter class
     """
 
     theme = {}
@@ -92,15 +96,15 @@
         if not hasattr(cls, 'highlightBlock'):
             raise NotImplementedError(f'Method highlightBlock() have to be implemented in subclass {cls.__name__}.')
 
     def override_colors(self):
         for item in self.theme:
             """
             Proof of concept method of how to override the colors set to highlighter's syntax.
-            Consider to override the whole map with styles like background pattern.
+            Consider overriding the whole map with styles like background pattern.
             """
             # Get color values from the theme helper
             # For example: 'md_color_h1_text', where the 'md' is the theme prefix, and the 'h1_text' is the item
             _color = self.theme_helper.get_color(f'{self.theme_ini_prefix}_color_{item}')
             _background_color = self.theme_helper.get_color(f'{self.theme_ini_prefix}_background_color_{item}')
             if self.debug:
                 self.logger.debug(
```

### Comparing `notolog-0.9.1b7/notolog/highlight/md_highlighter.py` & `notolog-0.9.1b8/notolog/highlight/md_highlighter.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,23 +17,26 @@
 # - PyPI: https://pypi.org/project/notolog
 # - WebSite: https://notolog.app
 # - Author: Vadim Bakhrenkov
 # - Copyright 2024 Vadim Bakhrenkov
 # - License: MIT License
 
 from PySide6.QtCore import Qt
-from PySide6.QtGui import QTextBlockUserData
 
 from .main_highlighter import MainHighlighter
 from . import TextBlockData
 
-from typing import Union
+from typing import TYPE_CHECKING
 
 import re
 
+if TYPE_CHECKING:
+    from typing import Union  # noqa: F401
+    from PySide6.QtGui import QTextBlockUserData  # noqa: F401
+
 
 class MdHighlighter(MainHighlighter):
     """
     Syntax highlighter class for the Markdown language
     """
 
     theme = {
@@ -64,29 +67,32 @@
         'h5_text': {'color': 'darkCyan', 'font_size_ratio': 1.4, 'style': 'bold'},
         'h6': {'color': 'white', 'font_size_ratio': 1.3,
                'bg': {'color': 'darkCyan', 'pattern': Qt.BrushStyle.Dense4Pattern}},
         'h6_text': {'color': 'darkCyan', 'font_size_ratio': 1.3, 'style': 'bold'},
         's': {'color': 'grey', 'style': 'strikethrough'},
         'u': {'color': 'black', 'style': 'underline'},
         'code': {'color': 'magenta', 'bg': {'color': 'magenta', 'pattern': Qt.BrushStyle.Dense6Pattern}},
-        'codel': {'color': 'yellow', 'style': 'monospace', 'bg': {'color': 'darkMagenta', 'pattern': Qt.BrushStyle.Dense2Pattern}},
-        'codelf': {'color': 'white', 'style': 'monospace', 'bg': {'color': 'magenta', 'pattern': Qt.BrushStyle.Dense2Pattern}},
+        'codel': {'color': 'yellow', 'style': 'monospace',
+                  'bg': {'color': 'darkMagenta', 'pattern': Qt.BrushStyle.Dense2Pattern}},
+        'codelf': {'color': 'white', 'style': 'monospace',
+                   'bg': {'color': 'magenta', 'pattern': Qt.BrushStyle.Dense2Pattern}},
         'code_lang': {'color': 'magenta', 'style': 'bold'},
         'code_indent': {'bg': {'color': 'pink', 'pattern': Qt.BrushStyle.Dense6Pattern}},
         'code_content': {'color': 'brown'},
         # Debug: 'bg': {'color': 'darkGrey', 'pattern': Qt.BrushStyle.Dense2Pattern}
         'wrong_indent': {'bg': {'color': 'red', 'pattern': Qt.BrushStyle.DiagCrossPattern}},
         'comment': {'color': 'grey', 'bg': {'color': 'lightGrey', 'pattern': Qt.BrushStyle.Dense6Pattern}},
         'table_h': {'style': ['bold', 'monospace'], 'bg': {'color': 'lightGrey'}},
         'table_d': {'style': 'monospace', 'bg': {'color': 'whiteSmoke'}},
         'img': {'color': 'green'},
         'ref': {'color': 'white', 'bg': {'color': 'green', 'pattern': Qt.BrushStyle.Dense3Pattern}},
         # 'ref_data': {'color': 'green', 'bg': {'color': 'yellow', 'pattern': Qt.BrushStyle.Dense6Pattern}},
         'abbr': {'color': 'white', 'bg': {'color': 'dodgerBlue', 'pattern': Qt.BrushStyle.SolidPattern}},
-        'abbr_text': {'color': 'white', 'style': 'bold', 'bg': {'color': 'dodgerBlue', 'pattern': Qt.BrushStyle.SolidPattern}},
+        'abbr_text': {'color': 'white', 'style': 'bold',
+                      'bg': {'color': 'dodgerBlue', 'pattern': Qt.BrushStyle.SolidPattern}},
         'link': {'color': 'white', 'style': 'italic', 'bg': 'blue'},
         'list': {'color': 'white', 'bg': 'darkMagenta'},
         'list_text': {'color': 'darkMagenta'},
         'list_indent': {'bg': {'color': 'darkMagenta', 'pattern': Qt.BrushStyle.Dense6Pattern}},
         'hr': {'color': 'white', 'style': 'strikethrough', 'bg': {'color': 'darkOrange'}},
         'blockquote': {'color': 'white', 'bg': {'color': 'grey', 'pattern': Qt.BrushStyle.Dense2Pattern},
                        # Blockquote friendly elements inherited this background
@@ -125,15 +131,16 @@
         (r'^(\s+|\>{1}\s+|)([0-9]{1,}\.|[\*\+\-]{1})(\s.*?)$', 3, 'list_text', 'list', False, theme['list_text'], None),
         (r'^(\s+|\>{1}\s+|)([0-9]{1,}\.|[\*\+\-]{1})\s.*?$',
          1, 'list_indent', 'list', False, theme['list_indent'], None),
         # Code ``` (fenced)
         (r'(?:^|\s|\W|[^`\#])(?<!`)(```(?!`).*?(?<!`)```)(?!`)(?:\s|\W|[^`]|$)',
          1, 'codel', 'code', False, theme['codelf'], None),
         (r'^(?<!\#)((?:[\s]*?)```)[a-z\-_\+#\s\.{}]*?(?!```)$', 1, 'code', 'code', True, theme['code'], None),
-        (r'^(?<!\#)((?:[\s]*?)```)(\s*?\{?[a-z\-_\+#\s\.^{}]+\}?)$', 2, 'code_lang', 'code', False, theme['code_lang'], None),
+        (r'^(?<!\#)((?:[\s]*?)```)(\s*?\{?[a-z\-_\+#\s\.^{}]+\}?)$',
+         2, 'code_lang', 'code', False, theme['code_lang'], None),
         (r'^([\s]{1,})```([\S]+|)$', 1, 'wrong_indent', 'code', False, theme['wrong_indent'], None),
         # Code ::::
         (r'^(([\s]{4,}|[\t]{1,})(::::))[\S]*?\s*?$', 3, 'codec', 'code', False, theme['code'], None),
         (r'^(([\s]{4,}|[\t]{1,})::::)([\S]+)\s*?$', 3, 'code_lang', 'code', False, theme['code_lang'], None),
         (r'^([\s]{4,}|[\t]{1,})::::[\S]*?\s*?$', 1, 'code_indent', 'code', False, theme['code_indent'], None),
         # Italic (asterisk)
         (r'(?<!\*)(\*[^\s\*][^\*]*?[^\s]?\*)(?!\*)', 1, 'i', 'i', False, theme['i'], None),  # between
@@ -288,15 +295,15 @@
     def get_nl_closing_tokens(self):
         """
         Block open tokens closing with a new empty line.
         The order in the row is matter because of processing one-by-one.
         """
         return ['rn', 'codec', 'blockquote', 'list']
 
-    def highlightBlock(self, text_str):
+    def highlightBlock(self, text_str):  # noqa: C901 - consider simplifying this method
         """
         Apply a syntax highlighting to each line of the text.
         * https://doc.qt.io/qt-6/qsyntaxhighlighter.html#highlightBlock
         """
 
         # Get the current block and associated user data
         self.current_block = self.currentBlock()
@@ -473,15 +480,16 @@
             * rn
             * blockquote
             * codec
             * list
             Notice: Do not processing it when located within a code block, like this:
             if (self.is_in_code() and tag not in {'codec'}):
                 continue
-            Causing a "jumping" syntax, so better to leave the blocks within the code block but re-write their style completely.
+            Causing a "jumping" syntax, so better to leave the blocks within the code block
+            but re-write their style accordingly.
             """
             if tag not in self.get_nl_closing_tokens():
                 continue
 
             if tag not in self.tokens:
                 self.tokens[tag] = {'cnt': 0, 'o': False}
 
@@ -590,15 +598,15 @@
 
         try:
             """
             Try to save block data to allow future processing
             """
             self.current_block.setUserData(self.user_data)
         except (TypeError, RuntimeError, ValueError) as e:
-            self.logger.error('Cannot setup block data "%s"' % self.user_data)
+            self.logger.error(f'Cannot setup block data "{self.user_data}", error occurred: {e}')
 
         format_map = {}  # To apply formatting after the whole line processed
         for pattern, nth, tag, group, duple, cf_data, reckon in self.rules:
 
             if self.is_in_code() and group not in {'code', 'comment', 'coop', 'rn'}:
                 """
                 Ignore non-code tags if within a code block
```

### Comparing `notolog-0.9.1b7/notolog/highlight/view_highlighter.py` & `notolog-0.9.1b8/notolog/highlight/view_highlighter.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,21 @@
 
 from PySide6.QtCore import Qt
 from PySide6.QtGui import QTextBlock
 
 from .main_highlighter import MainHighlighter
 from . import TextBlockData
 
-from typing import Match
+from typing import TYPE_CHECKING
 
 import re
 
+if TYPE_CHECKING:
+    from typing import Match  # noqa: F401
+
 
 class ViewHighlighter(MainHighlighter):
     """
     Syntax highlighter class for the view mode
     """
 
     theme = {
@@ -65,15 +68,15 @@
         return pattern
 
     def get_open_close_token_map(self):
         return [
             {'group': 's', 'open': 's_open', 'close': 's_close', 'theme': 's'}
         ]
 
-    def highlightBlock(self, text_str):
+    def highlightBlock(self, text_str):  # noqa: C901 - consider simplifying this method
         """
         Apply a syntax highlighting to each line of the text.
         https://doc.qt.io/qt-6/qsyntaxhighlighter.html#highlightBlock
         """
 
         # Get the current block and associated user data
         current_block = self.currentBlock()
@@ -96,15 +99,15 @@
         self.clear_formatted()
 
         # Keep all line numbers even if no tags there
         if line_number not in self.line_tokens:
             self.line_tokens[line_number] = {}
 
         # Groups of tokens for correction (they have similar approach in rules)
-        oct_groups = [r.get('group') for r in self.get_open_close_token_map()]
+        # oct_groups = [r.get('group') for r in self.get_open_close_token_map()]
         open_tokens = [r.get('open') for r in self.get_open_close_token_map()]
         close_tokens = [r.get('close') for r in self.get_open_close_token_map()]
 
         for pattern, nth, tag, group, duple, cf_data, reckon in self.rules:
             """
             Regular Python regular expression operations instead of QRegularExpression, QRegularExpressionMatchIterator
             and QRegularExpressionMatch as sometimes it doesn't work properly.
```

### Comparing `notolog-0.9.1b7/notolog/image_downloader.py` & `notolog-0.9.1b8/notolog/image_downloader.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,40 +25,40 @@
     downloaded = Signal(dict)
 
     # Signal to emit upon all downloading tasks in queue have been finished
     finished = Signal(int)
 
     RESOURCE_DIR = AppConfig().get_editor_media_dir()
 
-    def __init__(self, base_folder: str = None):
+    event_loop = None  # async event loop
+    resource_tasks: list = []  # async downloads task queue
+    folder: Union[QDir, None] = None  # active folder to work with resources
+    base_folder: str = None  # base folder to work with
+    downloaded_cnt: int = 0  # downloads counter, counts till finished emitted
+    network_manager: QNetworkAccessManager = None
 
+    def __init__(self, base_folder: str = None):
         super().__init__()
 
         self.settings = Settings(parent=self)
 
         self.logger = logging.getLogger('image_downloader')
 
         self.logging = AppConfig().get_logging()
         self.debug = AppConfig().get_debug()
 
         self.lexemes = Lexemes()
 
-        # Async event loop
-        self.event_loop = asyncio.get_event_loop()
-        # async download tasks queue
-        self.resource_tasks = []
-
-        # Active folder to work with resources
-        self.folder = Union[QDir, None]
+        self.base_folder = base_folder
 
-        # Downloaded counter till finished emitted
-        self.downloaded_cnt = 0
-
-        self.update_resource_folder(base_folder)
+        # Setup start up params
+        self.initialize()
 
+    def initialize(self):
+        self.update_resource_folder(self.base_folder)
         self.network_manager = QNetworkAccessManager()
 
     def get_resource_folder(self, base_folder: str = None) -> QDir:
         # Check folder and make it QDir
         if base_folder:
             folder = os.path.join(base_folder, self.RESOURCE_DIR)
         else:
@@ -77,45 +77,48 @@
     def download_image(self, url: str) -> None:
         if not self.is_external_url(url):
             if self.debug:
                 self.logger.debug(f"Skip downloading as the provided url is not an external url: {url}")
             return
 
         if self.debug:
-            self.logger.debug(f"Downloading {url}")
+            self.logger.debug(f'Downloading resource from "{url}"')
 
         request = QNetworkRequest(QUrl(url))
         reply = self.network_manager.get(request)
 
         # Connecting finished signal
         reply.finished.connect(lambda _reply=reply: self.handle_network_reply(_reply))
         # Connecting error signal
-        reply.errorOccurred.connect(lambda error, _reply=reply: self.handle_network_reply(_reply, error))
+        reply.errorOccurred.connect(lambda error, _reply=reply: self.handle_network_reply_error(_reply, error))
 
     def save_image(self, url: str, data: QByteArray) -> None:
         # file_name = os.path.basename(url)
         file_name = self.url_to_filename(url)
+        # Alternative approach:
+        # file_extension = self.mime_to_extension(mime_type)
+        # file_name = f"{file_name}{file_extension}"
         # Create resource folder if not yet created
         os.makedirs(self.folder.path(), exist_ok=True)
         # File path to save
         file_path = os.path.join(self.folder.path(), file_name)
         # Save received data
         if save_file(file_path, data, as_bytearray=True):
             if self.debug:
                 self.logger.debug(f"Resource saved {url} to {file_path} [{size_f(len(data))}]")
         else:
             if self.debug:
                 self.logger.debug(f"Resource not saved {url} to {file_path} [{size_f(len(data))}]")
 
-    def handle_network_reply(self, reply, error_code=None):
+    def handle_network_reply(self, reply):
         # Get received status code, say 200
         status_code = reply.attribute(QNetworkRequest.Attribute.HttpStatusCodeAttribute)
 
         if self.debug:
-            self.logger.debug(f'Update response, reply: {reply}, error_code: {error_code}, status_code: {status_code}')
+            self.logger.debug(f'Network reply, reply: {reply}, status_code: {status_code}')
 
         reply.deleteLater()  # Clean up the QNetworkReply object
 
         # Make sure there is no error
         if reply.error() == QNetworkReply.NetworkError.NoError:
             # No error, processing the image
             result_message = self.lexemes.get('network_connection_error_empty')
@@ -123,36 +126,44 @@
                 self.logger.debug(result_message)
 
             # Check if the resource is an image
             mime_type = reply.header(QNetworkRequest.KnownHeaders.ContentTypeHeader)
             if 'image' in mime_type:
                 url = reply.url().toString()
                 data = reply.readAll()  # type: QByteArray
+
                 if self.debug:
                     self.logger.debug(f"Resource data downloaded {url} [{size_f(len(data))}]")
 
                 # Store the image within the app's cache first
-                pixmap = QPixmap()
-                pixmap.loadFromData(data)
-                QPixmapCache.insert(url, pixmap)
-
-                self.downloaded.emit({'resource_name': url})
-                self.downloaded_cnt += 1
+                self.cache_pixmap(url, data)
 
+                # Save file if settings allow
                 if self.settings.viewer_save_resources:
                     # Saving downloaded files
                     self.save_image(url, data)
 
-                """
-                base_name = self.url_to_filename(url)
-                file_extension = self.mime_to_extension(mime_type)
-                file_name = f"{base_name}{file_extension}"
-                """
+                # Emit the file downloaded signal
+                self.downloaded.emit({'resource_name': url})
+                self.downloaded_cnt += 1
+
+    def cache_pixmap(self, url: str, data: QByteArray):
+        # Store the image within the app's cache first
+        pixmap = QPixmap()
+        pixmap.loadFromData(data)
+        QPixmapCache.insert(url, pixmap)
 
-        elif reply.error() == QNetworkReply.NetworkError.HostNotFoundError:
+    def handle_network_reply_error(self, reply, error_code=None):
+        # Get received status code, say 404
+        status_code = reply.attribute(QNetworkRequest.Attribute.HttpStatusCodeAttribute)
+
+        if self.debug:
+            self.logger.debug(f'Network reply, reply: {reply}, error_code: {error_code}, status_code: {status_code}')
+
+        if reply.error() == QNetworkReply.NetworkError.HostNotFoundError:
             # The host was not found, indicating possible DNS issues or no internet connection
             result_message = self.lexemes.get('network_connection_error_connection_or_dns')
         elif reply.error() == QNetworkReply.NetworkError.ConnectionRefusedError:
             # Connection was refused, indicating the server might be down or there are network issues
             result_message = self.lexemes.get('network_connection_error_connection_refused')
         elif reply.error() == QNetworkReply.NetworkError.TimeoutError:
             # The connection timed out, indicating network issues
@@ -161,43 +172,55 @@
             # The requested page or resource is not found
             result_message = self.lexemes.get('network_connection_error_connection_404_error')
         else:
             # Handle other errors
             result_message = self.lexemes.get('network_connection_error_generic_with_status_code',
                                               status_code=status_code)
 
-        if error_code is not None:
-            if self.logging:
-                self.logger.warning(result_message)
-                self.logger.warning(f"Failed to download resource: {reply.errorString()}")
+        if self.logging:
+            self.logger.warning(result_message)
+            self.logger.warning(f'Failed to download resource "{reply.errorString()}" with error code [{error_code}]')
 
     @asyncSlot()
     async def download_resource_in_queue(self, resource_url) -> None:
+        # Check async loop is running
+        if not asyncio.get_event_loop().is_running():
+            if self.logging:
+                self.logger.debug('Async loop is not running, skip task')
+            return
+
         if self.debug:
             self.logger.debug('Downloading resource %d tasks in queue' % len(self.resource_tasks))
 
-        task = asyncio.ensure_future(self.resource_download_async(resource_url))
+        task = asyncio.ensure_future(self.resource_download_async(resource_url))  # task: .download_resource_in_queue()
         # Add task to the local pool first
         self.resource_tasks.append(task)
         # Callback method to set up further actions
-        task.add_done_callback(lambda _task: self.resource_task_callback(_task))
-
-        done, pending = await asyncio.wait(
-            self.resource_tasks,
-            return_when=asyncio.ALL_COMPLETED,  # There is no pending tasks check
-            # timeout = 1.5  # to return after the timeout, some task could be pending
-        )
+        task.add_done_callback(lambda _task: self.resource_task_callback(_task))  # task: .resource_download_async()
 
-        if self.debug:
-            self.logger.debug(f'Downloading resource tasks progress. Done {len(done)}, pending {len(pending)}')
+        try:
+            done, pending = await asyncio.wait(
+                self.resource_tasks,
+                return_when=asyncio.ALL_COMPLETED,  # There is no pending tasks check
+                # timeout = 1.5  # to return after the timeout, some task could be pending
+            )
+            if self.debug:
+                self.logger.debug(f'Downloading resource tasks progress. Done {len(done)}, pending {len(pending)}')
+        except asyncio.CancelledError:
+            # All tasks will be cancelled later upon close event
+            pass
 
         if len(self.resource_tasks) <= 1:
             # Hold this method a particular amount of time to allow completed tasks to settle as this step is
             # typically ahead.
-            await asyncio.sleep(0.25, self.event_loop)
+            try:
+                await asyncio.sleep(0.25, self.event_loop)
+            except asyncio.CancelledError:
+                # All tasks will be cancelled later upon close event
+                pass
             if self.downloaded_cnt > 0:
                 # All tasks in queue have finished
                 self.finished.emit(self.downloaded_cnt)
                 self.downloaded_cnt = 0
 
     def resource_task_callback(self, task):
         if self.debug:
@@ -209,25 +232,14 @@
 
     async def resource_download_async(self, image_url) -> None:
         """
         Downloading resource which will be processed by resource_downloaded_handler() then.
         """
         self.download_image(image_url)
 
-    async def cancel_tasks(self):
-        tasks_total = len(self.resource_tasks)
-        for i, task in enumerate(self.resource_tasks):
-            if not task.done():
-                task_res = task.cancel()
-                if self.logging:
-                    self.logger.info(
-                        f'[{i + 1}/{tasks_total}] Pending task "{task.get_name()}" canceled with result "{task_res}"')
-                # Gather all tasks to ensure they are completed before closing
-                await asyncio.gather(*self.resource_tasks, return_exceptions=True)
-
     @staticmethod
     def is_external_url(url, base_domain='example.com'):
         """
         Determine if the given URL is an external URL.
         """
         parsed_url = urlparse(url)
         return not (parsed_url.netloc == '' or parsed_url.netloc.endswith(base_domain))
```

### Comparing `notolog-0.9.1b7/notolog/lexemes/de/ai_assistant.py` & `notolog-0.9.1b8/notolog/lexemes/de/ai_assistant.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 
     "dialog_usage_model_label": "MODELL",
     "dialog_usage_tokens_label": "TOKENS",
     "dialog_usage_tokens_prompt": "prompt: {tokens}",
     "dialog_usage_tokens_answer": "Antwort: {tokens}",
     "dialog_usage_tokens_total": "gesamt: {tokens}",
     "dialog_button_send_request": "Anfrage senden",
-}
+}
```

### Comparing `notolog-0.9.1b7/notolog/lexemes/de/color_picker_dialog.py` & `notolog-0.9.1b8/notolog/lexemes/de/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/de/common.py` & `notolog-0.9.1b8/notolog/lexemes/de/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,17 +49,18 @@
     "dialog_decrypt_file_rewrite_existing_title": "Vorhandene Datei überschreiben",
     "dialog_decrypt_file_rewrite_existing_text": "Vorhandene Datei \"{file_path}\" überschreiben?",
 
     "dialog_encrypt_new_password_title": "Neues Passwort",
     "dialog_encrypt_new_password_label": "Passwort:",
     "dialog_encrypt_new_password_input_placeholder_text": "Neues Passwort eingeben",
     "dialog_encrypt_new_password_hint_label": "Hinweis:",
-    "dialog_encrypt_new_password_hint_label_description": "Der Hinweis ist nicht verschlüsselt und kann aus der Datei gelesen werden! "
-                                                          "\nVerwenden Sie keine offensichtlichen Hinweise, die leicht erraten werden können, wie Geburtsdaten. "
-                                                          "\nVersuchen Sie, eine Referenz zu verwenden, die nicht leicht mit Ihnen in Verbindung gebracht werden kann.",
+    "dialog_encrypt_new_password_hint_label_description":
+        "Der Hinweis ist nicht verschlüsselt und kann aus der Datei gelesen werden! "
+        "\nVerwenden Sie keine offensichtlichen Hinweise, die leicht erraten werden können, wie Geburtsdaten. "
+        "\nVersuchen Sie, eine Referenz zu verwenden, die nicht leicht mit Ihnen in Verbindung gebracht werden kann.",
     "dialog_encrypt_new_password_hint_input_placeholder_text": "Hinweis eingeben (optional)",
     "dialog_encrypt_new_password_button_ok": "OK",
     "dialog_encrypt_new_password_button_cancel": "Abbrechen",
     "dialog_encrypt_new_password_warning_empty_title": "Warnung",
     "dialog_encrypt_new_password_warning_empty_text": "Das Passwortfeld darf nicht leer sein!",
     "dialog_encrypt_new_password_warning_too_long_title": "Warnung",
     "dialog_encrypt_new_password_warning_too_long_text": "Das Hinweisfeld ist zu lang, maximal {symbols} Zeichen!",
@@ -68,15 +69,16 @@
     "dialog_encrypt_password_label": "Passwort:",
     "dialog_encrypt_password_input_placeholder_text": "Passwort eingeben",
     "dialog_encrypt_password_hint_label": "Hinweis:",
     "dialog_encrypt_password_button_ok": "OK",
     "dialog_encrypt_password_button_cancel": "Abbrechen",
 
     "dialog_encrypt_password_reset_title": "Verschlüsselungspasswort zurücksetzen",
-    "dialog_encrypt_password_reset_text": "Sind Sie sicher, dass Sie das aktuelle Verschlüsselungspasswort zurücksetzen möchten?",
+    "dialog_encrypt_password_reset_text":
+        "Sind Sie sicher, dass Sie das aktuelle Verschlüsselungspasswort zurücksetzen möchten?",
     "dialog_encrypt_password_reset_button_cancel": "Abbrechen",
     "dialog_encrypt_password_reset_button_yes": "Ja",
 
     "dialog_open_link_title": "Link",
     "dialog_open_link_text": "Link \"{url}\" in einem Browser öffnen?",
 
     "load_file_encryption_password_mismatch": "Verschlüsselungspasswort stimmt nicht überein!",
```

### Comparing `notolog-0.9.1b7/notolog/lexemes/de/main_menu.py` & `notolog-0.9.1b8/notolog/lexemes/de/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/de/settings_dialog.py` & `notolog-0.9.1b8/notolog/lexemes/de/settings_dialog.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -57,8 +57,8 @@
     "ai_config_base_system_prompt_label": "Systemaufforderung",
     "ai_config_base_system_prompt_edit_placeholder_text": "Grundsystemaufforderung, die jeder Anfrage vorausgeht",
     "ai_config_base_system_prompt_edit_accessible_description":
         "Grundsystemaufforderung, die jeder Anfrage vorausgeht. Reiner Text.",
     "ai_config_base_response_max_tokens_label": "Maximale Antwort-Token",
     "ai_config_base_response_max_tokens_input_accessible_description":
         "Maximale Anzahl von Token, die in der Antwort empfangen werden",
-}
+}
```

### Comparing `notolog-0.9.1b7/notolog/lexemes/de/statusbar.py` & `notolog-0.9.1b8/notolog/lexemes/de/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/de/toolbar.py` & `notolog-0.9.1b8/notolog/lexemes/de/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/en/ai_assistant.py` & `notolog-0.9.1b8/notolog/lexemes/en/ai_assistant.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 
     "dialog_usage_model_label": "MODEL",
     "dialog_usage_tokens_label": "TOKENS",
     "dialog_usage_tokens_prompt": "prompt: {tokens}",
     "dialog_usage_tokens_answer": "answer: {tokens}",
     "dialog_usage_tokens_total": "total: {tokens}",
     "dialog_button_send_request": "Send Request",
-}
+}
```

### Comparing `notolog-0.9.1b7/notolog/lexemes/en/color_picker_dialog.py` & `notolog-0.9.1b8/notolog/lexemes/en/color_picker_dialog.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -139,8 +139,8 @@
     "color_picker_color_thistle": "Thistle",
     "color_picker_color_tomato": "Tomato",
     "color_picker_color_turquoise": "Turquoise",
     "color_picker_color_violet": "Violet",
     "color_picker_color_wheat": "Wheat",
     "color_picker_color_whitesmoke": "White Smoke",
     "color_picker_color_yellowgreen": "Yellow Green",
-}
+}
```

### Comparing `notolog-0.9.1b7/notolog/lexemes/en/common.py` & `notolog-0.9.1b8/notolog/lexemes/en/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/en/main_menu.py` & `notolog-0.9.1b8/notolog/lexemes/en/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/en/settings_dialog.py` & `notolog-0.9.1b8/notolog/lexemes/en/settings_dialog.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,9 +55,10 @@
 
     "ai_config_base_label": "Base Parameters",
     "ai_config_base_system_prompt_label": "System Prompt",
     "ai_config_base_system_prompt_edit_placeholder_text": "Base system prompt that precedes each request",
     "ai_config_base_system_prompt_edit_accessible_description":
         "Base system prompt that precedes each request. This is plain text.",
     "ai_config_base_response_max_tokens_label": "Maximum Response Tokens",
-    "ai_config_base_response_max_tokens_input_accessible_description": "Maximum number of tokens to receive in response",
-}
+    "ai_config_base_response_max_tokens_input_accessible_description":
+        "Maximum number of tokens to receive in response",
+}
```

### Comparing `notolog-0.9.1b7/notolog/lexemes/en/statusbar.py` & `notolog-0.9.1b8/notolog/lexemes/en/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/en/toolbar.py` & `notolog-0.9.1b8/notolog/lexemes/en/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/es/ai_assistant.py` & `notolog-0.9.1b8/notolog/lexemes/es/ai_assistant.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 lexemes = {
     # Asistente IA
     "dialog_title": "Solicitud a IA",
     "dialog_prompt_input_placeholder_text": "Solicitud",
     "dialog_prompt_input_accessible_description": "Ingrese la solicitud para dar un contexto al asistente IA",
     "dialog_response_output_placeholder_text": "Datos de respuesta",
     "dialog_response_output_accessible_description": "Los datos de respuesta aparecerán en este campo",
-    "dialog_response_output_notice_empty_text": "Proporcione una entrada de texto para obtener una respuesta de aproximadamente...",
+    "dialog_response_output_notice_empty_text":
+        "Proporcione una entrada de texto para obtener una respuesta de aproximadamente...",
 
     "dialog_usage_model_label": "MODELO",
     "dialog_usage_tokens_label": "TOKENS",
     "dialog_usage_tokens_prompt": "prompt: {tokens}",
     "dialog_usage_tokens_answer": "respuesta: {tokens}",
     "dialog_usage_tokens_total": "total: {tokens}",
     "dialog_button_send_request": "Enviar solicitud",
-}
+}
```

### Comparing `notolog-0.9.1b7/notolog/lexemes/es/color_picker_dialog.py` & `notolog-0.9.1b8/notolog/lexemes/es/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/es/common.py` & `notolog-0.9.1b8/notolog/lexemes/es/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,24 +49,26 @@
     "dialog_decrypt_file_rewrite_existing_title": "Reescribir archivo existente",
     "dialog_decrypt_file_rewrite_existing_text": "¿Reescribir archivo existente \"{file_path}\"?",
 
     "dialog_encrypt_new_password_title": "Nueva Contraseña",
     "dialog_encrypt_new_password_label": "Contraseña:",
     "dialog_encrypt_new_password_input_placeholder_text": "Introduzca la nueva contraseña",
     "dialog_encrypt_new_password_hint_label": "Pista:",
-    "dialog_encrypt_new_password_hint_label_description": "¡La pista no está cifrada y puede ser leída desde el archivo! "
-                                                          "\nEvite pistas obvias que se puedan adivinar fácilmente, como fechas de nacimiento. "
-                                                          "\nIntente utilizar una referencia que no se asocie fácilmente con usted.",
+    "dialog_encrypt_new_password_hint_label_description":
+        "¡La pista no está cifrada y puede ser leída desde el archivo! "
+        "\nEvite pistas obvias que se puedan adivinar fácilmente, como fechas de nacimiento. "
+        "\nIntente utilizar una referencia que no se asocie fácilmente con usted.",
     "dialog_encrypt_new_password_hint_input_placeholder_text": "Introduzca una pista (opcional)",
     "dialog_encrypt_new_password_button_ok": "Aceptar",
     "dialog_encrypt_new_password_button_cancel": "Cancelar",
     "dialog_encrypt_new_password_warning_empty_title": "Advertencia",
     "dialog_encrypt_new_password_warning_empty_text": "¡El campo de contraseña no puede estar vacío!",
     "dialog_encrypt_new_password_warning_too_long_title": "Advertencia",
-    "dialog_encrypt_new_password_warning_too_long_text": "El campo de la pista es demasiado largo, ¡máximo de {symbols} caracteres!",
+    "dialog_encrypt_new_password_warning_too_long_text":
+        "El campo de la pista es demasiado largo, ¡máximo de {symbols} caracteres!",
 
     "dialog_encrypt_password_title": "Introducir Contraseña",
     "dialog_encrypt_password_label": "Contraseña:",
     "dialog_encrypt_password_input_placeholder_text": "Introducir contraseña",
     "dialog_encrypt_password_hint_label": "Pista:",
     "dialog_encrypt_password_button_ok": "Aceptar",
     "dialog_encrypt_password_button_cancel": "Cancelar",
```

### Comparing `notolog-0.9.1b7/notolog/lexemes/es/main_menu.py` & `notolog-0.9.1b8/notolog/lexemes/es/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/es/settings_dialog.py` & `notolog-0.9.1b8/notolog/lexemes/es/settings_dialog.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -58,8 +58,8 @@
     "ai_config_base_system_prompt_label": "Prompt del sistema",
     "ai_config_base_system_prompt_edit_placeholder_text": "Prompt del sistema base que precede a cada solicitud",
     "ai_config_base_system_prompt_edit_accessible_description":
         "Prompt del sistema base que precede a cada solicitud. Texto plano.",
     "ai_config_base_response_max_tokens_label": "Máximo de tokens de respuesta",
     "ai_config_base_response_max_tokens_input_accessible_description":
         "Número máximo de tokens para recibir en la respuesta",
-}
+}
```

### Comparing `notolog-0.9.1b7/notolog/lexemes/es/statusbar.py` & `notolog-0.9.1b8/notolog/lexemes/es/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/es/toolbar.py` & `notolog-0.9.1b8/notolog/lexemes/es/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/fi/ai_assistant.py` & `notolog-0.9.1b8/notolog/lexemes/fi/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/fi/color_picker_dialog.py` & `notolog-0.9.1b8/notolog/lexemes/fi/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/fi/common.py` & `notolog-0.9.1b8/notolog/lexemes/fi/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/fi/main_menu.py` & `notolog-0.9.1b8/notolog/lexemes/fi/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/fi/settings_dialog.py` & `notolog-0.9.1b8/notolog/lexemes/fi/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/fi/statusbar.py` & `notolog-0.9.1b8/notolog/lexemes/fi/statusbar.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,8 +19,7 @@
     "statusbar_encryption_label_encryption_encrypted": "Salattu",
 
     "statusbar_cursor_label": "rivi: {line} → sar: {column}",
     "statusbar_cursor_label_selected": "rivi: {line} → sar: {column} → val: {selected}",
     "statusbar_cursor_label_with_global": "rivi: {line} → sar: {column} → pos: {position}",
     "statusbar_cursor_label_selected_with_global": "rivi: {line} → sar: {column} → pos: {position} → val: {selected}",
 }
-
```

### Comparing `notolog-0.9.1b7/notolog/lexemes/fi/toolbar.py` & `notolog-0.9.1b8/notolog/lexemes/fi/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/fr/ai_assistant.py` & `notolog-0.9.1b8/notolog/lexemes/fr/ai_assistant.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 
     "dialog_usage_model_label": "MODÈLE",
     "dialog_usage_tokens_label": "JETONS",
     "dialog_usage_tokens_prompt": "invite : {tokens}",
     "dialog_usage_tokens_answer": "réponse : {tokens}",
     "dialog_usage_tokens_total": "total : {tokens}",
     "dialog_button_send_request": "Envoyer la requête",
-}
+}
```

### Comparing `notolog-0.9.1b7/notolog/lexemes/fr/color_picker_dialog.py` & `notolog-0.9.1b8/notolog/lexemes/fr/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/fr/common.py` & `notolog-0.9.1b8/notolog/lexemes/fr/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,34 +49,37 @@
     "dialog_decrypt_file_rewrite_existing_title": "Réécrire sur le fichier existant",
     "dialog_decrypt_file_rewrite_existing_text": "Réécrire sur le fichier existant \"{file_path}\" ?",
 
     "dialog_encrypt_new_password_title": "Nouveau mot de passe",
     "dialog_encrypt_new_password_label": "Mot de passe :",
     "dialog_encrypt_new_password_input_placeholder_text": "Entrez un nouveau mot de passe",
     "dialog_encrypt_new_password_hint_label": "Indice :",
-    "dialog_encrypt_new_password_hint_label_description": "L'indice n'est pas crypté et peut être lu dans le fichier ! "
-                                                           "\nÉvitez des indices évidents faciles à deviner, comme la date de naissance. "
-                                                           "\nEssayez d'utiliser une référence qui n'est pas facilement associable à vous.",
+    "dialog_encrypt_new_password_hint_label_description":
+        "L'indice n'est pas crypté et peut être lu dans le fichier ! "
+        "\nÉvitez des indices évidents faciles à deviner, comme la date de naissance. "
+        "\nEssayez d'utiliser une référence qui n'est pas facilement associable à vous.",
     "dialog_encrypt_new_password_hint_input_placeholder_text": "Entrez un indice (facultatif)",
     "dialog_encrypt_new_password_button_ok": "OK",
     "dialog_encrypt_new_password_button_cancel": "Annuler",
     "dialog_encrypt_new_password_warning_empty_title": "Avertissement",
     "dialog_encrypt_new_password_warning_empty_text": "Le champ du mot de passe ne peut pas être vide !",
     "dialog_encrypt_new_password_warning_too_long_title": "Avertissement",
-    "dialog_encrypt_new_password_warning_too_long_text": "Le champ d'indice est trop long, {symbols} caractères maximum !",
+    "dialog_encrypt_new_password_warning_too_long_text":
+        "Le champ d'indice est trop long, {symbols} caractères maximum !",
 
     "dialog_encrypt_password_title": "Entrez le mot de passe",
     "dialog_encrypt_password_label": "Mot de passe :",
     "dialog_encrypt_password_input_placeholder_text": "Entrez le mot de passe",
     "dialog_encrypt_password_hint_label": "Indice :",
     "dialog_encrypt_password_button_ok": "OK",
     "dialog_encrypt_password_button_cancel": "Annuler",
 
     "dialog_encrypt_password_reset_title": "Réinitialiser le mot de passe de chiffrement",
-    "dialog_encrypt_password_reset_text": "Êtes-vous sûr de vouloir réinitialiser le mot de passe de chiffrement actuel ?",
+    "dialog_encrypt_password_reset_text":
+        "Êtes-vous sûr de vouloir réinitialiser le mot de passe de chiffrement actuel ?",
     "dialog_encrypt_password_reset_button_cancel": "Annuler",
     "dialog_encrypt_password_reset_button_yes": "Oui",
 
     "dialog_open_link_title": "Lien",
     "dialog_open_link_text": "Ouvrir le lien \"{url}\" dans un navigateur ?",
 
     "load_file_encryption_password_mismatch": "Non-concordance du mot de passe de chiffrement !",
@@ -103,12 +106,13 @@
     "update_helper_latest_version_installed": "La dernière version de l'application est installée",
 
     "network_connection_error_empty": "Impossible d'obtenir des informations de réponse",
     "network_connection_error_connection_or_dns":
         "Hôte introuvable. Il pourrait y avoir un problème avec la connexion Internet ou le DNS.",
     "network_connection_error_connection_refused":
         "Connexion refusée. Le serveur pourrait être hors service ou il pourrait y avoir des problèmes de réseau.",
-    "network_connection_error_connection_timed_out": "La connexion a expiré. Il pourrait y avoir des problèmes de réseau.",
+    "network_connection_error_connection_timed_out":
+        "La connexion a expiré. Il pourrait y avoir des problèmes de réseau.",
     "network_connection_error_connection_404_error":
         "Erreur 404 de connexion. La page ou la ressource demandée n'est pas trouvée.",
     "network_connection_error_generic_with_status_code": "Échec de la requête avec le code d'état : {status_code}",
 }
```

### Comparing `notolog-0.9.1b7/notolog/lexemes/fr/main_menu.py` & `notolog-0.9.1b8/notolog/lexemes/fr/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/fr/settings_dialog.py` & `notolog-0.9.1b8/notolog/lexemes/fr/settings_dialog.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -57,8 +57,8 @@
     "ai_config_base_label": "Paramètres de base",
     "ai_config_base_system_prompt_label": "Invite de système",
     "ai_config_base_system_prompt_edit_placeholder_text": "Invite de système de base qui précède chaque demande",
     "ai_config_base_system_prompt_edit_accessible_description":
         "Invite de système de base qui précède chaque demande. Texte brut.",
     "ai_config_base_response_max_tokens_label": "Nombre maximal de jetons de réponse",
     "ai_config_base_response_max_tokens_input_accessible_description": "Nombre maximal de jetons à recevoir en réponse",
-}
+}
```

### Comparing `notolog-0.9.1b7/notolog/lexemes/fr/statusbar.py` & `notolog-0.9.1b8/notolog/lexemes/fr/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/fr/toolbar.py` & `notolog-0.9.1b8/notolog/lexemes/fr/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/ge/ai_assistant.py` & `notolog-0.9.1b8/notolog/lexemes/ge/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/ge/color_picker_dialog.py` & `notolog-0.9.1b8/notolog/lexemes/ge/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/ge/common.py` & `notolog-0.9.1b8/notolog/lexemes/ge/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,18 +49,19 @@
     "dialog_decrypt_file_rewrite_existing_title": "არსებული ფაილის გადაწერა",
     "dialog_decrypt_file_rewrite_existing_text": "გადაწერეთ არსებული ფაილი \"{file_path}\"?",
 
     "dialog_encrypt_new_password_title": "ახალი პაროლი",
     "dialog_encrypt_new_password_label": "პაროლი:",
     "dialog_encrypt_new_password_input_placeholder_text": "შეიყვანეთ ახალი პაროლი",
     "dialog_encrypt_new_password_hint_label": "მინიშნება:",
-    "dialog_encrypt_new_password_hint_label_description": "მინიშნება არ არის დაშიფრული და ფაილიდან იკითხება!"
-                                                          "\nარ გამოიყენოთ მინიშნები, რომლებიც ადვილად შეიმჩნევა, როგორიცაა"
-                                                          "\nდაბადების თარიღი."
-                                                          "\nსცადეთ გამოიყენოთ რეფერენცია, რომელიც ადვილად არ არის თქვენთან გაიგიანებელი.",
+    "dialog_encrypt_new_password_hint_label_description":
+        "მინიშნება არ არის დაშიფრული და ფაილიდან იკითხება!"
+        "\nარ გამოიყენოთ მინიშნები, რომლებიც ადვილად შეიმჩნევა, როგორიცაა"
+        "\nდაბადების თარიღი."
+        "\nსცადეთ გამოიყენოთ რეფერენცია, რომელიც ადვილად არ არის თქვენთან გაიგიანებელი.",
     "dialog_encrypt_new_password_hint_input_placeholder_text": "შეიყვანეთ მინიშნება (არასავალდებულო)",
     "dialog_encrypt_new_password_button_ok": "კარგი",
     "dialog_encrypt_new_password_button_cancel": "გაუქმება",
     "dialog_encrypt_new_password_warning_empty_title": "გაფრთხილება",
     "dialog_encrypt_new_password_warning_empty_text": "პაროლის ველი ცარიელი ვერ დარჩება!",
     "dialog_encrypt_new_password_warning_too_long_title": "გაფრთხილება",
     "dialog_encrypt_new_password_warning_too_long_text": "მინიშნების ველი ძალიან გრძელია, მაქსიმუმი {symbols} სიმბოლო!",
```

### Comparing `notolog-0.9.1b7/notolog/lexemes/ge/main_menu.py` & `notolog-0.9.1b8/notolog/lexemes/ge/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/ge/settings_dialog.py` & `notolog-0.9.1b8/notolog/lexemes/ge/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/ge/statusbar.py` & `notolog-0.9.1b8/notolog/lexemes/ge/statusbar.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,9 +17,10 @@
     "statusbar_encryption_label": "{encryption} {icon}",
     "statusbar_encryption_label_encryption_plain": "უშიფრადი",
     "statusbar_encryption_label_encryption_encrypted": "დაშიფრული",
 
     "statusbar_cursor_label": "ხაზი: {line} → სვეტი: {column}",
     "statusbar_cursor_label_selected": "ხაზი: {line} → სვეტი: {column} → არჩეული: {selected}",
     "statusbar_cursor_label_with_global": "ხაზი: {line} → სვეტი: {column} → პოზიცია: {position}",
-    "statusbar_cursor_label_selected_with_global": "ხაზი: {line} → სვეტი: {column} → პოზიცია: {position} → არჩეული: {selected}",
+    "statusbar_cursor_label_selected_with_global":
+        "ხაზი: {line} → სვეტი: {column} → პოზიცია: {position} → არჩეული: {selected}",
 }
```

### Comparing `notolog-0.9.1b7/notolog/lexemes/ge/toolbar.py` & `notolog-0.9.1b8/notolog/lexemes/ge/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/gr/ai_assistant.py` & `notolog-0.9.1b8/notolog/lexemes/gr/ai_assistant.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 
     "dialog_usage_model_label": "ΜΟΝΤΕΛΟ",
     "dialog_usage_tokens_label": "ΔΙΑΚΡΙΤΙΚΑ",
     "dialog_usage_tokens_prompt": "prompt: {tokens}",
     "dialog_usage_tokens_answer": "answer: {tokens}",
     "dialog_usage_tokens_total": "total: {tokens}",
     "dialog_button_send_request": "Αποστολή Αιτήματος",
-}
+}
```

### Comparing `notolog-0.9.1b7/notolog/lexemes/gr/color_picker_dialog.py` & `notolog-0.9.1b8/notolog/lexemes/gr/color_picker_dialog.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -139,8 +139,8 @@
     "color_picker_color_thistle": "Γαϊδουράγκαθο",
     "color_picker_color_tomato": "Ντομάτα",
     "color_picker_color_turquoise": "Τυρκουάζ",
     "color_picker_color_violet": "Βιολετί",
     "color_picker_color_wheat": "Σιτάρι",
     "color_picker_color_whitesmoke": "Λευκός Καπνός",
     "color_picker_color_yellowgreen": "Κίτρινο Πράσινο",
-}
+}
```

### Comparing `notolog-0.9.1b7/notolog/lexemes/gr/common.py` & `notolog-0.9.1b8/notolog/lexemes/gr/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,35 +49,38 @@
     "dialog_decrypt_file_rewrite_existing_title": "Επανεγγραφή υπάρχοντος αρχείου",
     "dialog_decrypt_file_rewrite_existing_text": "Επανεγγραφή υπάρχοντος αρχείου \"{file_path}\";",
 
     "dialog_encrypt_new_password_title": "Νέος Κωδικός",
     "dialog_encrypt_new_password_label": "Κωδικός:",
     "dialog_encrypt_new_password_input_placeholder_text": "Εισάγετε νέο κωδικό",
     "dialog_encrypt_new_password_hint_label": "Υπόδειξη:",
-    "dialog_encrypt_new_password_hint_label_description": "Η υπόδειξη δεν είναι κρυπτογραφημένη και μπορεί να διαβαστεί "
-                                                          "από το αρχείο!\nΑποφύγετε προφανείς υποδείξεις που μπορεί να "
-                                                          "μαντευτούν εύκολα, όπως ημερομηνίες γέννησης.\nΠροσπαθήστε "
-                                                          "να χρησιμοποιήσετε μια αναφορά που δεν συνδέεται εύκολα με εσάς.",
+    "dialog_encrypt_new_password_hint_label_description":
+        "Η υπόδειξη δεν είναι κρυπτογραφημένη και μπορεί να διαβαστεί "
+        "από το αρχείο!\nΑποφύγετε προφανείς υποδείξεις που μπορεί να "
+        "μαντευτούν εύκολα, όπως ημερομηνίες γέννησης.\nΠροσπαθήστε "
+        "να χρησιμοποιήσετε μια αναφορά που δεν συνδέεται εύκολα με εσάς.",
     "dialog_encrypt_new_password_hint_input_placeholder_text": "Εισάγετε υπόδειξη (προαιρετικά)",
     "dialog_encrypt_new_password_button_ok": "Εντάξει",
     "dialog_encrypt_new_password_button_cancel": "Ακύρωση",
     "dialog_encrypt_new_password_warning_empty_title": "Προειδοποίηση",
     "dialog_encrypt_new_password_warning_empty_text": "Το πεδίο του κωδικού δεν μπορεί να είναι άδειο!",
     "dialog_encrypt_new_password_warning_too_long_title": "Προειδοποίηση",
-    "dialog_encrypt_new_password_warning_too_long_text": "Το πεδίο της υπόδειξης είναι πολύ μακρύ, μέγιστο {symbols} χαρακτήρες!",
+    "dialog_encrypt_new_password_warning_too_long_text":
+        "Το πεδίο της υπόδειξης είναι πολύ μακρύ, μέγιστο {symbols} χαρακτήρες!",
 
     "dialog_encrypt_password_title": "Εισαγωγή Κωδικού",
     "dialog_encrypt_password_label": "Κωδικός:",
     "dialog_encrypt_password_input_placeholder_text": "Εισάγετε κωδικό",
     "dialog_encrypt_password_hint_label": "Υπόδειξη:",
     "dialog_encrypt_password_button_ok": "Εντάξει",
     "dialog_encrypt_password_button_cancel": "Ακύρωση",
 
     "dialog_encrypt_password_reset_title": "Επαναφορά Κωδικού Κρυπτογράφησης",
-    "dialog_encrypt_password_reset_text": "Είστε σίγουροι ότι θέλετε να επαναφέρετε τον τρέχοντα κωδικό κρυπτογράφησης;",
+    "dialog_encrypt_password_reset_text":
+        "Είστε σίγουροι ότι θέλετε να επαναφέρετε τον τρέχοντα κωδικό κρυπτογράφησης;",
     "dialog_encrypt_password_reset_button_cancel": "Ακύρωση",
     "dialog_encrypt_password_reset_button_yes": "Ναι",
 
     "dialog_open_link_title": "Σύνδεσμος",
     "dialog_open_link_text": "Άνοιγμα συνδέσμου \"{url}\" σε πρόγραμμα περιήγησης;",
 
     "load_file_encryption_password_mismatch": "Αναντιστοιχία κωδικού κρυπτογράφησης!",
```

### Comparing `notolog-0.9.1b7/notolog/lexemes/gr/main_menu.py` & `notolog-0.9.1b8/notolog/lexemes/gr/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/gr/settings_dialog.py` & `notolog-0.9.1b8/notolog/lexemes/gr/settings_dialog.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,28 +17,30 @@
     "general_app_theme_label": "Θέμα",
     "general_app_theme_combo_placeholder_text": "Επιλέξτε θέμα",
     "general_app_theme_combo_accessible_description": "Θέμα διεπαφής της εφαρμογής",
     "general_app_main_menu_label": "Κύριο Μενού",
     "general_app_main_menu_checkbox": "Εμφάνιση Κύριου Μενού",
     "general_app_main_menu_checkbox_accessible_description": "Εμφάνιση του κύριου αναδυόμενου μενού της εφαρμογής",
     "general_app_font_size_label": "Μέγεθος Γραμματοσειράς: {size}pt",
-    "general_app_font_size_slider_accessible_description": "Ρύθμιση του παγκόσμιου μεγέθους γραμματοσειράς της εφαρμογής",
+    "general_app_font_size_slider_accessible_description":
+        "Ρύθμιση του παγκόσμιου μεγέθους γραμματοσειράς της εφαρμογής",
 
     "general_statusbar_label": "Γραμμή Κατάστασης",
     "general_statusbar_show_global_cursor_position_checkbox": "Εμφάνιση Παγκόσμιας Θέσης Δρομέα",
     "general_statusbar_show_global_cursor_position_checkbox_accessible_description":
         "Εμφάνιση της παγκόσμιας θέσης του δρομέα στη γραμμή κατάστασης",
 
     "editor_config_label": "Ρυθμίσεις Επεξεργαστή",
     "editor_config_show_line_numbers_checkbox": "Εμφάνιση Αριθμών Γραμμών",
     "editor_config_show_line_numbers_checkbox_accessible_description": "Εμφάνιση αριθμών γραμμών στον επεξεργαστή",
 
     "viewer_config_label": "Ρυθμίσεις Προβολέα",
     "viewer_config_process_emojis_checkbox": "Μετατροπή Εικονιδίων Κειμένου σε Γραφικά",
-    "viewer_config_process_emojis_checkbox_accessible_description": "Μετατροπή εικονιδίων κειμένου σε γραφικές αναπαραστάσεις",
+    "viewer_config_process_emojis_checkbox_accessible_description":
+        "Μετατροπή εικονιδίων κειμένου σε γραφικές αναπαραστάσεις",
     "viewer_config_highlight_todos_checkbox": "Επισήμανση Σημειώσεων TODO",
     "viewer_config_highlight_todos_checkbox_accessible_description": "Επισήμανση ετικετών TODO μέσα στο κείμενο",
     "viewer_config_open_link_confirmation_checkbox": "Απαίτηση Επιβεβαίωσης για Άνοιγμα Συνδέσμων",
     "viewer_config_open_link_confirmation_checkbox_accessible_description":
         "Ζήτηση επιβεβαίωσης πριν το άνοιγμα συνδέσμων",
     "viewer_config_save_resources_checkbox": "Αυτόματη αποθήκευση εξωτερικών εικόνων στον δίσκο",
     "viewer_config_save_resources_checkbox_accessible_description":
@@ -55,9 +57,10 @@
 
     "ai_config_base_label": "Βασικοί Παράμετροι",
     "ai_config_base_system_prompt_label": "Σύστημα Προτροπής",
     "ai_config_base_system_prompt_edit_placeholder_text": "Βασική προτροπή συστήματος που προηγείται κάθε αιτήματος",
     "ai_config_base_system_prompt_edit_accessible_description":
         "Βασική προτροπή συστήματος που προηγείται κάθε αιτήματος. Απλό κείμενο.",
     "ai_config_base_response_max_tokens_label": "Μέγιστοι Διακριτικοί Απόκρισης",
-    "ai_config_base_response_max_tokens_input_accessible_description": "Μέγιστος αριθμός διακριτικών για λήψη σε απόκριση",
-}
+    "ai_config_base_response_max_tokens_input_accessible_description":
+        "Μέγιστος αριθμός διακριτικών για λήψη σε απόκριση",
+}
```

### Comparing `notolog-0.9.1b7/notolog/lexemes/gr/statusbar.py` & `notolog-0.9.1b8/notolog/lexemes/gr/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/gr/toolbar.py` & `notolog-0.9.1b8/notolog/lexemes/gr/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/in/ai_assistant.py` & `notolog-0.9.1b8/notolog/lexemes/in/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/in/color_picker_dialog.py` & `notolog-0.9.1b8/notolog/lexemes/in/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/in/common.py` & `notolog-0.9.1b8/notolog/lexemes/in/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/in/main_menu.py` & `notolog-0.9.1b8/notolog/lexemes/in/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/in/settings_dialog.py` & `notolog-0.9.1b8/notolog/lexemes/in/settings_dialog.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -56,8 +56,8 @@
     "ai_config_base_system_prompt_label": "सिस्टम प्रॉम्प्ट",
     "ai_config_base_system_prompt_edit_placeholder_text": "प्रत्येक अनुरोध से पहले मूल सिस्टम प्रॉम्प्ट",
     "ai_config_base_system_prompt_edit_accessible_description":
         "प्रत्येक अनुरोध से पहले मूल सिस्टम प्रॉम्प्ट। यह सादा पाठ है।",
     "ai_config_base_response_max_tokens_label": "अधिकतम प्रतिसाद टोकन्स",
     "ai_config_base_response_max_tokens_input_accessible_description":
         "प्रतिसाद में प्राप्त करने के लिए अधिकतम टोकन्स की संख्या"
-}
+}
```

### Comparing `notolog-0.9.1b7/notolog/lexemes/in/statusbar.py` & `notolog-0.9.1b8/notolog/lexemes/in/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/in/toolbar.py` & `notolog-0.9.1b8/notolog/lexemes/in/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/it/ai_assistant.py` & `notolog-0.9.1b8/notolog/lexemes/it/ai_assistant.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 
     "dialog_usage_model_label": "MODELLO",
     "dialog_usage_tokens_label": "TOKEN",
     "dialog_usage_tokens_prompt": "prompt: {tokens}",
     "dialog_usage_tokens_answer": "risposta: {tokens}",
     "dialog_usage_tokens_total": "totale: {tokens}",
     "dialog_button_send_request": "Invia richiesta",
-}
+}
```

### Comparing `notolog-0.9.1b7/notolog/lexemes/it/color_picker_dialog.py` & `notolog-0.9.1b8/notolog/lexemes/it/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/it/common.py` & `notolog-0.9.1b8/notolog/lexemes/it/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,24 +49,26 @@
     "dialog_decrypt_file_rewrite_existing_title": "Sovrascrivi file esistente",
     "dialog_decrypt_file_rewrite_existing_text": "Sovrascrivere il file esistente \"{file_path}\"?",
 
     "dialog_encrypt_new_password_title": "Nuova password",
     "dialog_encrypt_new_password_label": "Password:",
     "dialog_encrypt_new_password_input_placeholder_text": "Inserisci la nuova password",
     "dialog_encrypt_new_password_hint_label": "Suggerimento:",
-    "dialog_encrypt_new_password_hint_label_description": "Il suggerimento non è criptato e può essere letto dal file!"
-                                                          "\nNon utilizzare suggerimenti ovvi che possono essere indovinati, come"
-                                                          "\nla data di nascita, ecc. Prova a usare un riferimento.",
+    "dialog_encrypt_new_password_hint_label_description":
+        "Il suggerimento non è criptato e può essere letto dal file!"
+        "\nNon utilizzare suggerimenti ovvi che possono essere indovinati, come"
+        "\nla data di nascita, ecc. Prova a usare un riferimento.",
     "dialog_encrypt_new_password_hint_input_placeholder_text": "Inserisci un suggerimento (opzionale)",
     "dialog_encrypt_new_password_button_ok": "OK",
     "dialog_encrypt_new_password_button_cancel": "Annulla",
     "dialog_encrypt_new_password_warning_empty_title": "Avviso",
     "dialog_encrypt_new_password_warning_empty_text": "Il campo della password non può essere vuoto!",
     "dialog_encrypt_new_password_warning_too_long_title": "Avviso",
-    "dialog_encrypt_new_password_warning_too_long_text": "Il campo del suggerimento è troppo lungo, massimo {symbols} caratteri!",
+    "dialog_encrypt_new_password_warning_too_long_text":
+        "Il campo del suggerimento è troppo lungo, massimo {symbols} caratteri!",
 
     "dialog_encrypt_password_title": "Inserisci password",
     "dialog_encrypt_password_label": "Password:",
     "dialog_encrypt_password_input_placeholder_text": "Inserisci password",
     "dialog_encrypt_password_hint_label": "Suggerimento:",
     "dialog_encrypt_password_button_ok": "OK",
     "dialog_encrypt_password_button_cancel": "Annulla",
```

### Comparing `notolog-0.9.1b7/notolog/lexemes/it/main_menu.py` & `notolog-0.9.1b8/notolog/lexemes/it/main_menu.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -40,8 +40,8 @@
     "actions_help_accessible_name_md_syntax": "Sintassi Markdown",
     "actions_help_label_check_for_updates": "Controlla aggiornamenti",
     "actions_help_accessible_name_check_for_updates": "Controlla aggiornamenti",
     "actions_help_label_bug_report": "Segnala bug",
     "actions_help_accessible_name_bug_report": "Invia segnalazione di bug",
     "actions_help_label_about": "Informazioni",
     "actions_help_accessible_name_about": "Informazioni",
-}
+}
```

### Comparing `notolog-0.9.1b7/notolog/lexemes/it/settings_dialog.py` & `notolog-0.9.1b8/notolog/lexemes/it/settings_dialog.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,9 +56,10 @@
 
     "ai_config_base_label": "Parametri Base",
     "ai_config_base_system_prompt_label": "Prompt del Sistema",
     "ai_config_base_system_prompt_edit_placeholder_text": "Prompt di sistema base che precede ogni richiesta",
     "ai_config_base_system_prompt_edit_accessible_description":
         "Prompt di sistema base che precede ogni richiesta. Testo semplice.",
     "ai_config_base_response_max_tokens_label": "Massimo di Token di Risposta",
-    "ai_config_base_response_max_tokens_input_accessible_description": "Numero massimo di token da ricevere in risposta",
-}
+    "ai_config_base_response_max_tokens_input_accessible_description":
+        "Numero massimo di token da ricevere in risposta",
+}
```

### Comparing `notolog-0.9.1b7/notolog/lexemes/it/statusbar.py` & `notolog-0.9.1b8/notolog/lexemes/it/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/it/toolbar.py` & `notolog-0.9.1b8/notolog/lexemes/it/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/ja/ai_assistant.py` & `notolog-0.9.1b8/notolog/lexemes/ja/ai_assistant.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 
     "dialog_usage_model_label": "モデル",
     "dialog_usage_tokens_label": "トークン",
     "dialog_usage_tokens_prompt": "プロンプト: {tokens}",
     "dialog_usage_tokens_answer": "回答: {tokens}",
     "dialog_usage_tokens_total": "合計: {tokens}",
     "dialog_button_send_request": "リクエストを送信",
-}
+}
```

### Comparing `notolog-0.9.1b7/notolog/lexemes/ja/color_picker_dialog.py` & `notolog-0.9.1b8/notolog/lexemes/ja/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/ja/common.py` & `notolog-0.9.1b8/notolog/lexemes/ja/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/ja/main_menu.py` & `notolog-0.9.1b8/notolog/lexemes/ja/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/ja/settings_dialog.py` & `notolog-0.9.1b8/notolog/lexemes/ja/settings_dialog.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -55,8 +55,8 @@
     "ai_config_base_label": "基本パラメータ",
     "ai_config_base_system_prompt_label": "システムプロンプト",
     "ai_config_base_system_prompt_edit_placeholder_text": "各リクエストに先立つ基本システムプロンプト",
     "ai_config_base_system_prompt_edit_accessible_description":
         "各リクエストに先立つ基本システムプロンプト。プレーンテキスト。",
     "ai_config_base_response_max_tokens_label": "応答の最大トークン数",
     "ai_config_base_response_max_tokens_input_accessible_description": "応答で受け取る最大トークン数",
-}
+}
```

### Comparing `notolog-0.9.1b7/notolog/lexemes/ja/statusbar.py` & `notolog-0.9.1b8/notolog/lexemes/ja/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/ja/toolbar.py` & `notolog-0.9.1b8/notolog/lexemes/ja/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/ko/ai_assistant.py` & `notolog-0.9.1b8/notolog/lexemes/ko/ai_assistant.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 
     "dialog_usage_model_label": "모델",
     "dialog_usage_tokens_label": "토큰",
     "dialog_usage_tokens_prompt": "프롬프트: {tokens}",
     "dialog_usage_tokens_answer": "답변: {tokens}",
     "dialog_usage_tokens_total": "총계: {tokens}",
     "dialog_button_send_request": "요청 보내기",
-}
+}
```

### Comparing `notolog-0.9.1b7/notolog/lexemes/ko/color_picker_dialog.py` & `notolog-0.9.1b8/notolog/lexemes/ko/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/ko/common.py` & `notolog-0.9.1b8/notolog/lexemes/ko/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/ko/main_menu.py` & `notolog-0.9.1b8/notolog/lexemes/ko/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/ko/settings_dialog.py` & `notolog-0.9.1b8/notolog/lexemes/ko/settings_dialog.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -56,8 +56,8 @@
     "ai_config_base_label": "기본 매개변수",
     "ai_config_base_system_prompt_label": "시스템 프롬프트",
     "ai_config_base_system_prompt_edit_placeholder_text": "각 요청에 앞서는 기본 시스템 프롬프트",
     "ai_config_base_system_prompt_edit_accessible_description":
         "각 요청에 앞서는 기본 시스템 프롬프트. 일반 텍스트.",
     "ai_config_base_response_max_tokens_label": "응답 최대 토큰 수",
     "ai_config_base_response_max_tokens_input_accessible_description": "응답에서 받을 수 있는 최대 토큰 수",
-}
+}
```

### Comparing `notolog-0.9.1b7/notolog/lexemes/ko/statusbar.py` & `notolog-0.9.1b8/notolog/lexemes/ko/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/ko/toolbar.py` & `notolog-0.9.1b8/notolog/lexemes/ko/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/la/ai_assistant.py` & `notolog-0.9.1b8/notolog/lexemes/la/ai_assistant.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 
     "dialog_usage_model_label": "EXEMPLAR",
     "dialog_usage_tokens_label": "SIGNA",
     "dialog_usage_tokens_prompt": "promptus: {tokens}",
     "dialog_usage_tokens_answer": "responsio: {tokens}",
     "dialog_usage_tokens_total": "totum: {tokens}",
     "dialog_button_send_request": "Postulationem mittere",
-}
+}
```

### Comparing `notolog-0.9.1b7/notolog/lexemes/la/color_picker_dialog.py` & `notolog-0.9.1b8/notolog/lexemes/la/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/la/common.py` & `notolog-0.9.1b8/notolog/lexemes/la/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,17 +49,18 @@
     "dialog_decrypt_file_rewrite_existing_title": "Fasciculum exsistentem rescribere",
     "dialog_decrypt_file_rewrite_existing_text": "Fasciculum exsistentem \"{file_path}\" rescribere?",
 
     "dialog_encrypt_new_password_title": "Novum Signum",
     "dialog_encrypt_new_password_label": "Signum:",
     "dialog_encrypt_new_password_input_placeholder_text": "Novum signum ingredere",
     "dialog_encrypt_new_password_hint_label": "Monitum:",
-    "dialog_encrypt_new_password_hint_label_description": "Monitum non est cryptatum et legi potest ex archivo!"
-                                                          "\nNoli uti monitis perspicuis quae facile divinari possunt, ut"
-                                                          "\nnatale diem vel similia. Conare uti referentia non facile associata.",
+    "dialog_encrypt_new_password_hint_label_description":
+        "Monitum non est cryptatum et legi potest ex archivo!"
+        "\nNoli uti monitis perspicuis quae facile divinari possunt, ut"
+        "\nnatale diem vel similia. Conare uti referentia non facile associata.",
     "dialog_encrypt_new_password_hint_input_placeholder_text": "Ingredere monitum (non necessarium)",
     "dialog_encrypt_new_password_button_ok": "OK",
     "dialog_encrypt_new_password_button_cancel": "Cancellare",
     "dialog_encrypt_new_password_warning_empty_title": "Monitio",
     "dialog_encrypt_new_password_warning_empty_text": "Area signi vacua esse non potest!",
     "dialog_encrypt_new_password_warning_too_long_title": "Monitio",
     "dialog_encrypt_new_password_warning_too_long_text": "Area moniti nimis longa est, maximum {symbols} signa!",
```

### Comparing `notolog-0.9.1b7/notolog/lexemes/la/main_menu.py` & `notolog-0.9.1b8/notolog/lexemes/la/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/la/settings_dialog.py` & `notolog-0.9.1b8/notolog/lexemes/la/settings_dialog.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,13 +52,15 @@
     "ai_config_openai_api_key_input_accessible_description": "Clavis API OpenAI",
     "ai_config_openai_api_supported_models_label": "Modela sustenta",
     "ai_config_ai_model_names_combo_placeholder_text": "Modelum elige",
     "ai_config_ai_model_names_combo_accessible_description": "Modela sustenta ad eligendum",
 
     "ai_config_base_label": "Parametri Principes",
     "ai_config_base_system_prompt_label": "Systēma Monitum",
-    "ai_config_base_system_prompt_edit_placeholder_text": "Monitum systēmatis basis quod præcedit singulas postulationes",
+    "ai_config_base_system_prompt_edit_placeholder_text":
+        "Monitum systēmatis basis quod præcedit singulas postulationes",
     "ai_config_base_system_prompt_edit_accessible_description":
         "Monitum systēmatis basis quod præcedit singulas postulationes. Textus simpliciter.",
     "ai_config_base_response_max_tokens_label": "Maxima Responsionis Signa",
-    "ai_config_base_response_max_tokens_input_accessible_description": "Maximum signorum quæ in responsione accipiuntur",
-}
+    "ai_config_base_response_max_tokens_input_accessible_description":
+        "Maximum signorum quæ in responsione accipiuntur",
+}
```

### Comparing `notolog-0.9.1b7/notolog/lexemes/la/statusbar.py` & `notolog-0.9.1b8/notolog/lexemes/la/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/la/toolbar.py` & `notolog-0.9.1b8/notolog/lexemes/la/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/lexemes.py` & `notolog-0.9.1b8/notolog/lexemes/lexemes.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/nl/ai_assistant.py` & `notolog-0.9.1b8/notolog/lexemes/nl/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/nl/color_picker_dialog.py` & `notolog-0.9.1b8/notolog/lexemes/nl/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/nl/common.py` & `notolog-0.9.1b8/notolog/lexemes/nl/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,18 +49,18 @@
     "dialog_decrypt_file_rewrite_existing_title": "Bestaand bestand herschrijven",
     "dialog_decrypt_file_rewrite_existing_text": "Bestaand bestand \"{file_path}\" herschrijven?",
 
     "dialog_encrypt_new_password_title": "Nieuw wachtwoord",
     "dialog_encrypt_new_password_label": "Wachtwoord:",
     "dialog_encrypt_new_password_input_placeholder_text": "Nieuw wachtwoord invoeren",
     "dialog_encrypt_new_password_hint_label": "Hint:",
-    "dialog_encrypt_new_password_hint_label_description": "De hint is niet versleuteld en kan uit het bestand worden gelezen!"
-                                                          "\nVermijd voor de hand liggende hints die gemakkelijk geraden kunnen worden, zoals"
-                                                          "\ngeboortedata."
-                                                          "\nProbeer een referentie te gebruiken die niet gemakkelijk met u in verband wordt gebracht.",
+    "dialog_encrypt_new_password_hint_label_description":
+        "De hint is niet versleuteld en kan uit het bestand worden gelezen!"
+        "\nVermijd voor de hand liggende hints die gemakkelijk geraden kunnen worden, zoals geboortedata."
+        "\nProbeer een referentie te gebruiken die niet gemakkelijk met u in verband wordt gebracht.",
     "dialog_encrypt_new_password_hint_input_placeholder_text": "Hint invoeren (optioneel)",
     "dialog_encrypt_new_password_button_ok": "OK",
     "dialog_encrypt_new_password_button_cancel": "Annuleren",
     "dialog_encrypt_new_password_warning_empty_title": "Waarschuwing",
     "dialog_encrypt_new_password_warning_empty_text": "Het wachtwoordveld mag niet leeg zijn!",
     "dialog_encrypt_new_password_warning_too_long_title": "Waarschuwing",
     "dialog_encrypt_new_password_warning_too_long_text": "Het hintveld is te lang, maximaal {symbols} tekens!",
```

### Comparing `notolog-0.9.1b7/notolog/lexemes/nl/main_menu.py` & `notolog-0.9.1b8/notolog/lexemes/nl/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/nl/settings_dialog.py` & `notolog-0.9.1b8/notolog/lexemes/nl/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/nl/statusbar.py` & `notolog-0.9.1b8/notolog/lexemes/nl/statusbar.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,8 +19,7 @@
     "statusbar_encryption_label_encryption_encrypted": "Versleuteld",
 
     "statusbar_cursor_label": "regel: {line} → kol: {column}",
     "statusbar_cursor_label_selected": "regel: {line} → kol: {column} → sel: {selected}",
     "statusbar_cursor_label_with_global": "regel: {line} → kol: {column} → pos: {position}",
     "statusbar_cursor_label_selected_with_global": "regel: {line} → kol: {column} → pos: {position} → sel: {selected}",
 }
-
```

### Comparing `notolog-0.9.1b7/notolog/lexemes/nl/toolbar.py` & `notolog-0.9.1b8/notolog/lexemes/nl/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/pt/ai_assistant.py` & `notolog-0.9.1b8/notolog/lexemes/pt/ai_assistant.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 
     "dialog_usage_model_label": "MODELO",
     "dialog_usage_tokens_label": "TOKENS",
     "dialog_usage_tokens_prompt": "solicitação: {tokens}",
     "dialog_usage_tokens_answer": "resposta: {tokens}",
     "dialog_usage_tokens_total": "total: {tokens}",
     "dialog_button_send_request": "Enviar solicitação",
-}
+}
```

### Comparing `notolog-0.9.1b7/notolog/lexemes/pt/color_picker_dialog.py` & `notolog-0.9.1b8/notolog/lexemes/pt/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/pt/common.py` & `notolog-0.9.1b8/notolog/lexemes/pt/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,24 +49,26 @@
     "dialog_decrypt_file_rewrite_existing_title": "Sobrescrever arquivo existente",
     "dialog_decrypt_file_rewrite_existing_text": "Sobrescrever arquivo existente \"{file_path}\"?",
 
     "dialog_encrypt_new_password_title": "Nova senha",
     "dialog_encrypt_new_password_label": "Senha:",
     "dialog_encrypt_new_password_input_placeholder_text": "Digite a nova senha",
     "dialog_encrypt_new_password_hint_label": "Dica:",
-    "dialog_encrypt_new_password_hint_label_description": "A dica não é criptografada e pode ser lida do arquivo!"
-                                                          "\nNão use dicas óbvias que possam ser adivinhadas, como"
-                                                          "\na data de nascimento, ou algo do tipo. Tente usar uma referência.",
+    "dialog_encrypt_new_password_hint_label_description":
+        "A dica não é criptografada e pode ser lida do arquivo!"
+        "\nNão use dicas óbvias que possam ser adivinhadas, como"
+        "\na data de nascimento, ou algo do tipo. Tente usar uma referência.",
     "dialog_encrypt_new_password_hint_input_placeholder_text": "Digite uma dica (opcional)",
     "dialog_encrypt_new_password_button_ok": "OK",
     "dialog_encrypt_new_password_button_cancel": "Cancelar",
     "dialog_encrypt_new_password_warning_empty_title": "Aviso",
     "dialog_encrypt_new_password_warning_empty_text": "O campo de senha não pode ficar vazio!",
     "dialog_encrypt_new_password_warning_too_long_title": "Aviso",
-    "dialog_encrypt_new_password_warning_too_long_text": "O campo de dica é muito longo, máximo de {symbols} caracteres!",
+    "dialog_encrypt_new_password_warning_too_long_text":
+        "O campo de dica é muito longo, máximo de {symbols} caracteres!",
 
     "dialog_encrypt_password_title": "Digite a senha",
     "dialog_encrypt_password_label": "Senha:",
     "dialog_encrypt_password_input_placeholder_text": "Digite a senha",
     "dialog_encrypt_password_hint_label": "Dica:",
     "dialog_encrypt_password_button_ok": "OK",
     "dialog_encrypt_password_button_cancel": "Cancelar",
```

### Comparing `notolog-0.9.1b7/notolog/lexemes/pt/main_menu.py` & `notolog-0.9.1b8/notolog/lexemes/pt/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/pt/settings_dialog.py` & `notolog-0.9.1b8/notolog/lexemes/pt/settings_dialog.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -57,8 +57,8 @@
     "ai_config_base_label": "Parâmetros Base",
     "ai_config_base_system_prompt_label": "Prompt do Sistema",
     "ai_config_base_system_prompt_edit_placeholder_text": "Prompt do sistema base que antecede cada solicitação",
     "ai_config_base_system_prompt_edit_accessible_description":
         "Prompt do sistema base que antecede cada solicitação. Texto simples.",
     "ai_config_base_response_max_tokens_label": "Máximo de Tokens de Resposta",
     "ai_config_base_response_max_tokens_input_accessible_description": "Número máximo de tokens a receber em resposta",
-}
+}
```

### Comparing `notolog-0.9.1b7/notolog/lexemes/pt/statusbar.py` & `notolog-0.9.1b8/notolog/lexemes/pt/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/pt/toolbar.py` & `notolog-0.9.1b8/notolog/lexemes/pt/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/ru/ai_assistant.py` & `notolog-0.9.1b8/notolog/lexemes/ru/ai_assistant.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 
     "dialog_usage_model_label": "МОДЕЛЬ",
     "dialog_usage_tokens_label": "ТОКЕНЫ",
     "dialog_usage_tokens_prompt": "запрос: {tokens}",
     "dialog_usage_tokens_answer": "ответ: {tokens}",
     "dialog_usage_tokens_total": "всего: {tokens}",
     "dialog_button_send_request": "Отправить запрос",
-}
+}
```

### Comparing `notolog-0.9.1b7/notolog/lexemes/ru/color_picker_dialog.py` & `notolog-0.9.1b8/notolog/lexemes/ru/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/ru/common.py` & `notolog-0.9.1b8/notolog/lexemes/ru/common.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,17 +49,18 @@
     "dialog_decrypt_file_rewrite_existing_title": "Перезаписать существующий файл",
     "dialog_decrypt_file_rewrite_existing_text": "Перезаписать существующий файл \"{file_path}\"?",
 
     "dialog_encrypt_new_password_title": "Новый пароль",
     "dialog_encrypt_new_password_label": "Пароль:",
     "dialog_encrypt_new_password_input_placeholder_text": "Введите новый пароль",
     "dialog_encrypt_new_password_hint_label": "Подсказка:",
-    "dialog_encrypt_new_password_hint_label_description": "Подсказка не зашифрована и может быть прочитана из файла!"
-                                                          "\nНе используйте очевидные подсказки, которые можно легко угадать, например,"
-                                                          "\nдату рождения и т.д. Попробуйте использовать ссылку.",
+    "dialog_encrypt_new_password_hint_label_description":
+        "Подсказка не зашифрована и может быть прочитана из файла!"
+        "\nНе используйте очевидные подсказки, которые можно легко угадать,"
+        "\nнапример, дату рождения и т.д. Попробуйте использовать отсылку.",
     "dialog_encrypt_new_password_hint_input_placeholder_text": "Введите подсказку (необязательно)",
     "dialog_encrypt_new_password_button_ok": "ОК",
     "dialog_encrypt_new_password_button_cancel": "Отмена",
     "dialog_encrypt_new_password_warning_empty_title": "Предупреждение",
     "dialog_encrypt_new_password_warning_empty_text": "Поле пароля не может быть пустым!",
     "dialog_encrypt_new_password_warning_too_long_title": "Предупреждение",
     "dialog_encrypt_new_password_warning_too_long_text": "Поле подсказки слишком длинное, максимум {symbols} символов!",
```

### Comparing `notolog-0.9.1b7/notolog/lexemes/ru/main_menu.py` & `notolog-0.9.1b8/notolog/lexemes/ru/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/ru/settings_dialog.py` & `notolog-0.9.1b8/notolog/lexemes/ru/settings_dialog.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -58,8 +58,8 @@
     "ai_config_base_system_prompt_label": "Системный запрос",
     "ai_config_base_system_prompt_edit_placeholder_text": "Базовый системный запрос, предшествующий каждому запросу",
     "ai_config_base_system_prompt_edit_accessible_description":
         "Базовый системный запрос, предшествующий каждому запросу. Простой текст.",
     "ai_config_base_response_max_tokens_label": "Максимальное количество токенов ответа",
     "ai_config_base_response_max_tokens_input_accessible_description":
         "Максимальное количество токенов для получения в ответе",
-}
+}
```

### Comparing `notolog-0.9.1b7/notolog/lexemes/ru/statusbar.py` & `notolog-0.9.1b8/notolog/lexemes/ru/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/ru/toolbar.py` & `notolog-0.9.1b8/notolog/lexemes/ru/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/se/ai_assistant.py` & `notolog-0.9.1b8/notolog/lexemes/se/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/se/color_picker_dialog.py` & `notolog-0.9.1b8/notolog/lexemes/se/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/se/common.py` & `notolog-0.9.1b8/notolog/lexemes/se/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/se/main_menu.py` & `notolog-0.9.1b8/notolog/lexemes/se/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/se/settings_dialog.py` & `notolog-0.9.1b8/notolog/lexemes/se/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/se/statusbar.py` & `notolog-0.9.1b8/notolog/lexemes/se/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/se/toolbar.py` & `notolog-0.9.1b8/notolog/lexemes/se/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/tr/ai_assistant.py` & `notolog-0.9.1b8/notolog/lexemes/tr/ai_assistant.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 
     "dialog_usage_model_label": "MODEL",
     "dialog_usage_tokens_label": "TOKENLAR",
     "dialog_usage_tokens_prompt": "istek: {tokens}",
     "dialog_usage_tokens_answer": "cevap: {tokens}",
     "dialog_usage_tokens_total": "toplam: {tokens}",
     "dialog_button_send_request": "İstek Gönder",
-}
+}
```

### Comparing `notolog-0.9.1b7/notolog/lexemes/tr/color_picker_dialog.py` & `notolog-0.9.1b8/notolog/lexemes/tr/color_picker_dialog.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -139,8 +139,8 @@
     "color_picker_color_thistle": "Devedikeni",
     "color_picker_color_tomato": "Domates",
     "color_picker_color_turquoise": "Turkuaz",
     "color_picker_color_violet": "Menekşe",
     "color_picker_color_wheat": "Buğday",
     "color_picker_color_whitesmoke": "Beyaz Duman",
     "color_picker_color_yellowgreen": "Sarı Yeşil",
-}
+}
```

### Comparing `notolog-0.9.1b7/notolog/lexemes/tr/common.py` & `notolog-0.9.1b8/notolog/lexemes/tr/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,17 +49,18 @@
     "dialog_decrypt_file_rewrite_existing_title": "Mevcut dosyayı yeniden yaz",
     "dialog_decrypt_file_rewrite_existing_text": "\"{file_path}\" mevcut dosyayı yeniden yaz?",
 
     "dialog_encrypt_new_password_title": "Yeni Şifre",
     "dialog_encrypt_new_password_label": "Şifre:",
     "dialog_encrypt_new_password_input_placeholder_text": "Yeni Şifre Girin",
     "dialog_encrypt_new_password_hint_label": "İpucu:",
-    "dialog_encrypt_new_password_hint_label_description": "İpucu şifrelenmez ve dosyadan okunabilir!\nKolay tahmin "
-                                                          "edilebilecek açık ipuçları kullanmayın, örneğin doğum "
-                                                          "tarihleri gibi.\nKolayca ilişkilendirilemeyecek bir referans kullanın.",
+    "dialog_encrypt_new_password_hint_label_description":
+        "İpucu şifrelenmez ve dosyadan okunabilir!"
+        "\nKolay tahmin edilebilecek açık ipuçları kullanmayın, örneğin doğum tarihleri gibi."
+        "\nKolayca ilişkilendirilemeyecek bir referans kullanın.",
     "dialog_encrypt_new_password_hint_input_placeholder_text": "İpucu Girin (İsteğe Bağlı)",
     "dialog_encrypt_new_password_button_ok": "Tamam",
     "dialog_encrypt_new_password_button_cancel": "İptal",
     "dialog_encrypt_new_password_warning_empty_title": "Uyarı",
     "dialog_encrypt_new_password_warning_empty_text": "Şifre alanı boş olamaz!",
     "dialog_encrypt_new_password_warning_too_long_title": "Uyarı",
     "dialog_encrypt_new_password_warning_too_long_text": "İpucu alanı çok uzun, maksimum {symbols} karakter!",
```

### Comparing `notolog-0.9.1b7/notolog/lexemes/tr/main_menu.py` & `notolog-0.9.1b8/notolog/lexemes/tr/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/tr/settings_dialog.py` & `notolog-0.9.1b8/notolog/lexemes/tr/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/tr/statusbar.py` & `notolog-0.9.1b8/notolog/lexemes/tr/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/tr/toolbar.py` & `notolog-0.9.1b8/notolog/lexemes/tr/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/zh/ai_assistant.py` & `notolog-0.9.1b8/notolog/lexemes/zh/ai_assistant.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 
     "dialog_usage_model_label": "模型",
     "dialog_usage_tokens_label": "令牌",
     "dialog_usage_tokens_prompt": "提示：{tokens}",
     "dialog_usage_tokens_answer": "答案：{tokens}",
     "dialog_usage_tokens_total": "总计：{tokens}",
     "dialog_button_send_request": "发送请求",
-}
+}
```

### Comparing `notolog-0.9.1b7/notolog/lexemes/zh/color_picker_dialog.py` & `notolog-0.9.1b8/notolog/lexemes/zh/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/zh/common.py` & `notolog-0.9.1b8/notolog/lexemes/zh/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/zh/main_menu.py` & `notolog-0.9.1b8/notolog/lexemes/zh/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/zh/settings_dialog.py` & `notolog-0.9.1b8/notolog/lexemes/zh/settings_dialog.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -55,8 +55,8 @@
     "ai_config_base_label": "基础参数",
     "ai_config_base_system_prompt_label": "系统提示",
     "ai_config_base_system_prompt_edit_placeholder_text": "基础系统提示，位于每个请求之前",
     "ai_config_base_system_prompt_edit_accessible_description":
         "基础系统提示，位于每个请求之前。纯文本。",
     "ai_config_base_response_max_tokens_label": "响应的最大令牌数",
     "ai_config_base_response_max_tokens_input_accessible_description": "响应中接收的最大令牌数",
-}
+}
```

### Comparing `notolog-0.9.1b7/notolog/lexemes/zh/statusbar.py` & `notolog-0.9.1b8/notolog/lexemes/zh/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/lexemes/zh/toolbar.py` & `notolog-0.9.1b8/notolog/lexemes/zh/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/main.py` & `notolog-0.9.1b8/notolog/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -58,16 +58,19 @@
     if AppConfig().get_logging():
         logger.info("%s v%s" % (AppConfig().get_app_name(), AppConfig().get_app_version()))
         logger.info("%s" % (AppConfig().get_app_license()))
 
     # Main application
     app = QApplication(sys.argv)
     # To correctly set up app settings
-    app.setOrganizationName('Notolog')
-    app.setApplicationName('notolog_editor')
+    app.setOrganizationName(AppConfig().get_settings_org_name())
+    app.setOrganizationDomain(AppConfig().get_settings_org_domain())
+    # Consider different app names for pip package and for the source files run,
+    # as the settings storage depends on it.
+    app.setApplicationName(AppConfig().get_settings_app_name())
     app.setApplicationVersion(AppConfig().get_app_version())
 
     # Detect the operating system to choose the style
     current_os = platform.system()
     if current_os == "Windows":
         app.setStyle(QStyleFactory.create("WindowsVista"))
     # elif current_os == "Darwin":  # macOS
@@ -75,15 +78,16 @@
     else:  # Or: current_os == "Linux"
         app.setStyle(QStyleFactory.create("Fusion"))  # Fusion is a cross-platform choice
 
     # Maintain a unique style regardless of the user's system settings
     app.setDesktopSettingsAware(False)
 
     if AppConfig().get_debug():
-        logger.debug('Application dir path "%s"' % QApplication.applicationDirPath())
+        # E.g. /usr/bin and /usr/bin/python3.11
+        logger.debug(f'Application dir path "{app.applicationDirPath()}"; file path "{app.applicationFilePath()}"')
 
     # Get the screen to pass it to the main module
     screen = app.screens()[0]
 
     # Main loop
     loop = QEventLoop(app)
     asyncio.set_event_loop(loop)
```

### Comparing `notolog-0.9.1b7/notolog/notolog_editor.py` & `notolog-0.9.1b8/notolog/notolog_editor.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,49 +59,53 @@
 from .encrypt.enc_password_reset_dialog import EncPasswordResetDialog
 from cryptography.fernet import InvalidToken, InvalidSignature
 
 # Helpers
 from .helpers.theme_helper import ThemeHelper
 from .helpers.clipboard_helper import ClipboardHelper
 from .helpers.update_helper import UpdateHelper
-from .helpers.file_helper import res_path, size_f, read_file, save_file
+from .helpers.file_helper import res_path, size_f, save_file
 
 # Lexemes
 from .lexemes.lexemes import Lexemes
 
 # Editor state
 from .editor_state import EditorState, Mode, Source, Encryption
 
 from PySide6.QtCore import Slot, Qt, QDir, QPoint, QTimer, QSize, QUrl
 from PySide6.QtCore import QRegularExpression, QItemSelectionModel, QFileSystemWatcher
 from PySide6.QtGui import QGuiApplication, QIcon, QAction, QColor, QPalette, QShortcut, QFont, QKeySequence
 from PySide6.QtGui import QTextDocument, QTextCursor, QTextBlock, QDesktopServices, QPixmap, QPixmapCache
 from PySide6.QtWidgets import QWidget, QMainWindow, QVBoxLayout, QSplitter, QListView, QTextBrowser
-from PySide6.QtWidgets import QPlainTextEdit, QToolButton, QSizePolicy, QStatusBar, QCheckBox, QToolBar
-from PySide6.QtWidgets import QLabel, QLineEdit, QPushButton, QMenu, QDialog, QMessageBox, QStyle
+from PySide6.QtWidgets import QPlainTextEdit, QSizePolicy
+from PySide6.QtWidgets import QLineEdit, QMenu, QDialog, QMessageBox, QStyle
 from PySide6.QtWidgets import QAbstractItemView, QFileSystemModel, QFileDialog
 
-from qasync import asyncSlot, asyncClose
+from qasync import asyncClose
 import asyncio
 
 # Markdown library
 import markdown
 # Markdown library extensions
 from markdown.extensions.codehilite import CodeHiliteExtension
 # Custom markdown extension to process element tree
 from .etree_extension import ElementTreeExtension
 
 # Emojis support
 import emoji
 
 import os
-from typing import Union, Optional, Callable, List, Dict, Any
+from typing import TYPE_CHECKING, Union, Optional, Callable, List, Dict, Any
 
 import logging
 
+if TYPE_CHECKING:
+    from PySide6.QtGui import QScreen  # noqa: F401
+    from PySide6.QtWidgets import QStatusBar, QToolBar  # noqa: F401
+
 
 class NotologEditor(QMainWindow):
     """
     Main UI class to set up the application's UI and to process any user actions.
     """
 
     AREA_WEIGHT = 5
@@ -140,15 +144,15 @@
 
     More info https://python-markdown.github.io/extensions/extra/
     """
     md_extensions = [
         'markdown.extensions.extra',  # Or 'extra'
     ]
 
-    def __init__(self, parent = None, **kwargs):
+    def __init__(self, parent=None, **kwargs):
         super(NotologEditor, self).__init__(parent=parent)
 
         self.logger = logging.getLogger('notolog')
 
         self.logging = AppConfig().get_logging()
         self.debug = AppConfig().get_debug()
 
@@ -159,15 +163,15 @@
         Set theme:
         self.settings.theme = 'bordo'
         """
 
         # Default language setup, change to settings value to modify it via UI
         self.lexemes = Lexemes(self.settings.app_language)
 
-        self.screen = None
+        self.screen = None  # type: Union[QScreen, None]
         if 'screen' in kwargs:
             self.screen = kwargs['screen']
 
         """
         The `self.devicePixelRatio()` is also available through the `app.devicePixelRatio()`
         """
         self.dpr = self.devicePixelRatio()
@@ -399,15 +403,16 @@
             self.estate.refresh()
             # Update window title
             self.set_app_title()  # Generic title without sub part
             # Update toolbar
             self.create_icons_toolbar(refresh=True)
             if hasattr(self.toolbar, 'search_input'):
                 # Search field placeholder to empty
-                self.toolbar.search_input.setPlaceholderText(self.lexemes.get('search_input_placeholder_text', scope='toolbar'))
+                self.toolbar.search_input.setPlaceholderText(
+                    self.lexemes.get('search_input_placeholder_text', scope='toolbar'))
             # Re-draw main menu
             self.draw_menu()
 
         if 'app_theme' in data and hasattr(self, 'theme_helper'):
             self.theme_helper = ThemeHelper()
             # Update app's palette styles
             self.init_palette()
@@ -453,15 +458,15 @@
             # View widget
             view_widget = self.get_view_widget()  # type: Union[ViewWidget, QTextBrowser]
             # Disconnect previous lambda
             view_widget.anchorClicked.disconnect()
             # Set up connection again
             view_widget.anchorClicked.connect(self.open_link_dialog_proxy())
 
-    def editor_state_update_handler(self, data: dict) -> None:
+    def editor_state_update_handler(self, data: dict) -> None:  # noqa: C901 - consider simplifying this method
         """
         Perform actions belonging to the editor state changed, say mode toggle event.
         When switching between VIEW and EDIT mode some icons and texts may look differ, have different actions, etc.
         """
 
         if self.debug:
             self.logger.debug('Editor state update handler is in use "%s"' % data)
@@ -480,15 +485,16 @@
                 encryption_symbol_encrypted = self.lexemes.get('statusbar_encryption_symbol_encrypted_label',
                                                                scope='statusbar')
                 encryption_symbol_unencrypted = self.lexemes.get('statusbar_encryption_symbol_unencrypted_label',
                                                                  scope='statusbar')
                 encryption_symbol = encryption_symbol_encrypted if self.get_encryption() == Encryption.ENCRYPTED\
                     else encryption_symbol_unencrypted
                 encryption_status = self.lexemes.get('statusbar_encryption_label_encryption_%s'
-                                              % Encryption(self.get_encryption()).name.lower(), scope='statusbar')
+                                                     % Encryption(self.get_encryption()).name.lower(),
+                                                     scope='statusbar')
                 encryption_label_text = self.lexemes.get('statusbar_encryption_label', scope='statusbar',
                                                          encryption=encryption_status, icon=encryption_symbol)
                 self.statusbar['encryption_label'].setText(encryption_label_text)
             # Show cursor position data
             self.statusbar['cursor_label'].setText(self.get_cursor_label_text())
             # Restore litter bin state
             self.statusbar.set_litter_bin_visibility(visible=self.settings.show_deleted_files)
@@ -1055,45 +1061,49 @@
             self.logger.debug('Context menu for %s' % tree_view)
 
         # Save any unsaved changes
         self.save_active_file(clear_after=False)
 
         global_pos = tree_view.mapToGlobal(pos)
         tree_index = tree_view.indexAt(pos)
-        tree_index_row = tree_view.indexAt(pos).row()
+        # tree_index_row = tree_view.indexAt(pos).row()
         # self.tree_view.currentIndex()
 
         # QSortFilterProxyModel self.tree_proxy_model | tree_view.model()
         file_index = self.tree_proxy_model.mapToSource(tree_index)
         file_path = self.file_model.filePath(file_index)
 
         if not os.path.isfile(file_path):
             self.logger.warning('Trying to create context menu on a file that does not exist "%s"' % file_path)
             return
 
         menu = QMenu(self)
         menu.setFont(self.font())
-        rename_icon = self.theme_helper.get_icon(theme_icon='cursor-text.svg', system_icon='document-properties',
+        rename_icon = self.theme_helper.get_icon(
+            theme_icon='cursor-text.svg', system_icon='document-properties',
             color=QColor(self.theme_helper.get_color('main_tree_context_menu_rename')))
         menu.addAction(rename_icon, self.lexemes.get('menu_action_rename'),
                        lambda: self.rename_file_dialog(file_path))
         if self.is_file_safely_deleted(file_path):
             # Restore deleted file context action
-            restore_icon = self.theme_helper.get_icon(theme_icon='box-arrow-up.svg', system_icon='edit-undo',
+            restore_icon = self.theme_helper.get_icon(
+                theme_icon='box-arrow-up.svg', system_icon='edit-undo',
                 color=QColor(self.theme_helper.get_color('main_tree_context_menu_restore')))
             menu.addAction(restore_icon, self.lexemes.get('menu_action_restore'),
                            lambda: self.restore_file_dialog(file_path))
             # Delete completely file context action
-            delete_icon = self.theme_helper.get_icon(theme_icon='x-square-fill.svg', system_icon='edit-delete',
+            delete_icon = self.theme_helper.get_icon(
+                theme_icon='x-square-fill.svg', system_icon='edit-delete',
                 color=QColor(self.theme_helper.get_color('main_tree_context_menu_delete_completely')))
             menu.addAction(delete_icon, self.lexemes.get('menu_action_delete_completely'),
                            lambda: self.delete_completely_file_dialog(file_path))
         else:
             # Delete file context action
-            delete_icon = self.theme_helper.get_icon(theme_icon='x-square.svg', system_icon='edit-delete',
+            delete_icon = self.theme_helper.get_icon(
+                theme_icon='x-square.svg', system_icon='edit-delete',
                 color=QColor(self.theme_helper.get_color('main_tree_context_menu_delete')))
             menu.addAction(delete_icon, self.lexemes.get('menu_action_delete'),
                            lambda: self.delete_file_dialog(file_path))
 
         menu.exec(global_pos)
 
     def rename_file_dialog(self, file_path: str) -> None:
@@ -1707,21 +1717,34 @@
         return self.text_view
 
     @asyncClose
     async def closeEvent(self, event):
         if self.logging:
             self.logger.info('Stopping events loop, closing the app... Sayonara!')
 
-        # Cancel all re-highlight tasks if they are exist
-        if hasattr(self, 'async_highlighter') and self.async_highlighter:
-            await self.async_highlighter.cancel_tasks()
-
-        # Cancel all resource downloading tasks if they are exist
-        if hasattr(self, 'resource_downloader') and self.resource_downloader:
-            await self.resource_downloader.cancel_tasks()
+        async def cleanup_tasks():
+            if not asyncio.get_event_loop().is_running():
+                return
+            tasks = asyncio.all_tasks()
+            tasks_total = len(tasks)
+            # Cancel and clean up all pending asyncio tasks
+            for i, task in enumerate(tasks):
+                # Or: not task.done()
+                if (task is not asyncio.current_task()
+                        # But not the final task set at main
+                        and not (hasattr(task, 'get_coro') and task.get_coro().__qualname__ == 'Event.wait')):
+                    task_res = task.cancel()
+                    try:
+                        await task
+                    except asyncio.CancelledError:
+                        print(f'[{i + 1}/{tasks_total}] Pending task {task.get_name()} '
+                              f'was cancelled with result "{task_res}"')
+                        pass
+        # Await tasks to complete
+        await cleanup_tasks()
 
         if self.get_mode() == Mode.EDIT:
             # Save any unsaved changes
             self.save_active_file(clear_after=False)
         else:
             # Save cursor position (block start)
             self.store_doc_cursor_pos(self.get_mode())
@@ -1973,20 +1996,20 @@
                  'label': self.lexemes.get('actions_file_label_open', scope='main_menu'),
                  'accessible_name': self.lexemes.get('actions_file_accessible_name_open', scope='main_menu'),
                  'action': self.action_open_file},
                 {'type': 'action', 'name': 'actions_file_label_save',
                  'system_icon': 'media-floppy', 'theme_icon': 'floppy2-fill.svg',
                  'label': self.lexemes.get('actions_file_label_save', scope='main_menu'),
                  'accessible_name': self.lexemes.get('actions_file_accessible_name_save', scope='main_menu'),
-                 'action': self.action_save_file,},
+                 'action': self.action_save_file},
                 {'type': 'action', 'name': 'actions_file_label_save_as',
                  'system_icon': 'media-floppy', 'theme_icon': 'floppy2.svg',
                  'label': self.lexemes.get('actions_file_label_save_as', scope='main_menu'),
                  'accessible_name': self.lexemes.get('actions_file_accessible_name_save_as', scope='main_menu'),
-                 'action': self.action_save_as_file,},
+                 'action': self.action_save_as_file},
                 {'type': 'delimiter'},
                 {'type': 'action', 'name': 'actions_file_label_exit',
                  'system_icon': 'application-exit', 'theme_icon': 'power.svg',
                  'label': self.lexemes.get('actions_file_label_exit', scope='main_menu'),
                  'accessible_name': self.lexemes.get('actions_file_accessible_name_exit', scope='main_menu'),
                  'action': self.action_exit},
             ]},
@@ -2881,18 +2904,18 @@
             self.logger.debug('Sending bug report...')
 
         url = AppConfig().get_repository_github_bug_report_url()
 
         self.common_dialog(
             self.lexemes.get('dialog_open_link_title'),
             self.lexemes.get(name='dialog_open_link_text', url=url),
-                # Open url with system browser
-                callback=lambda dialog_callback:
-                # Open link in a system browser and run dialog's callback
-                (QDesktopServices.openUrl(url), dialog_callback()))
+            # Open url with system browser
+            callback=lambda dialog_callback:
+            # Open link in a system browser and run dialog's callback
+            (QDesktopServices.openUrl(url), dialog_callback()))
 
     def action_about(self) -> None:
         """
         Show about the App info.
         """
 
         if self.debug:
@@ -2978,15 +3001,15 @@
         else:
             if self.logging:
                 self.logger.warning('Unrecognized mode %s' % self.get_mode())
 
         # Set cursor back
         self.setCursor(Qt.CursorShape.ArrowCursor)
 
-    def load_file(self, file_path: str) -> bool:
+    def load_file(self, file_path: str) -> bool:  # noqa: C901 - consider simplifying this method
         """
         Helper: Load content of the file.
         """
 
         if not os.path.isabs(file_path):
             file_path = os.path.abspath(file_path)  # Make sure it's an absolute path
 
@@ -3216,15 +3239,15 @@
         Helper: Save file content.
         """
         if self.debug:
             self.logger.debug('Saving file "%s"' % file_path)
 
         return save_file(file_path, content)
 
-    def save_active_file(self, clear_after: bool = False, allow_save_empty_content: bool = None) -> None:
+    def save_active_file(self, clear_after: bool = False, allow_save_empty_content: bool = None) -> None:  # noqa: C901
         """
         Helper: Save currently opened file.
         @param clear_after: bool, clear edit field after saving (when applicable, say switching view mode)
         @param allow_save_empty_content: bool, dialog answer of either to allow to save an empty file or not
         @return: None
         """
 
@@ -3248,95 +3271,94 @@
             self.logger.debug(f"Save active file '{current_file_path}' (clear field after: '{clear_after}')")
 
         if not os.path.exists(current_file_path):
             if self.logging:
                 self.logger.warning(f"Cannot save active file '{current_file_path}', check if it was moved or deleted")
             return
 
-        with open(current_file_path, 'r', encoding='utf-8') as file:
-            # Edit widget
-            edit_widget = self.get_edit_widget()  # type: Union[EditWidget, QPlainTextEdit]
-            file_content = edit_widget.toPlainText()
+        # Edit widget
+        edit_widget = self.get_edit_widget()  # type: Union[EditWidget, QPlainTextEdit]
+        file_content = edit_widget.toPlainText()
 
-            # If new content is empty ask confirmation to be sure
-            if (not file_content
-                    # Previous content not the same as a current one
-                    and self.content != file_content
-                    # Allow empty content dialog not answered
-                    and (self.estate.allow_save_empty is None)):
-                # Set this globally to avoid a lot of annoying dialogs
-                self.estate.allow_save_empty = False
-                # Dialog with a callback back to the file and closing dialog sub-callback
-                self.common_dialog(
-                    self.lexemes.get('dialog_save_empty_file_title'),
-                    self.lexemes.get('dialog_save_empty_file_text'),
-                    callback=lambda dialog_callback:
-                        (self.save_active_file(clear_after=clear_after, allow_save_empty_content=True),
-                         # Close dialog sub-callback
-                         dialog_callback()))
-
-            # Save if any changes
-            if (file_content or self.estate.allow_save_empty) and self.content != file_content:
-                # Show saving progress in the status bar
+        # If new content is empty ask confirmation to be sure
+        if (not file_content
+                # Previous content not the same as a current one
+                and self.content != file_content
+                # Allow empty content dialog not answered
+                and (self.estate.allow_save_empty is None)):
+            # Set this globally to avoid a lot of annoying dialogs
+            self.estate.allow_save_empty = False
+            # Dialog with a callback back to the file and closing dialog sub-callback
+            self.common_dialog(
+                self.lexemes.get('dialog_save_empty_file_title'),
+                self.lexemes.get('dialog_save_empty_file_text'),
+                callback=lambda dialog_callback:
+                    (self.save_active_file(clear_after=clear_after, allow_save_empty_content=True),
+                     # Close dialog sub-callback
+                     dialog_callback()))
+
+        # Save if any changes
+        if (file_content or self.estate.allow_save_empty) and self.content != file_content:
+            # Show saving progress in the status bar
+            if hasattr(self, 'statusbar'):
+                self.statusbar['save_progress_label'].setVisible(True)
+            # Grayscale save button(s) at the toolbar
+            if hasattr(self.toolbar, 'toolbar_save_button'):
+                self.toolbar.toolbar_save_button.setDisabled(True)
+
+            def restore_saving_ui_state() -> None:
                 if hasattr(self, 'statusbar'):
-                    self.statusbar['save_progress_label'].setVisible(True)
-                # Grayscale save button(s) at the toolbar
-                if hasattr(self.toolbar, 'toolbar_save_button'):
-                    self.toolbar.toolbar_save_button.setDisabled(True)
-
-                def restore_saving_ui_state() -> None:
-                    if hasattr(self, 'statusbar'):
-                        self.statusbar['save_progress_label'].setVisible(False)
-                    # Keep it switched off to explicitly show the nothing to save state
-                    # self.toolbar.toolbar_save_button.setEnabled(True)
-                # Restore saving UI state automatically.
-                QTimer.singleShot(1500, restore_saving_ui_state)
-
-                if self.header is None or not self.header.is_valid():
-                    # Get empty file header here, it's needed for compatibility and will not be applied to the file
-                    header = FileHeader()
-                    if self.logging:
-                        self.logger.info('File "%s" has no header info' % current_file_path)
-                else:
-                    header = self.header
+                    self.statusbar['save_progress_label'].setVisible(False)
+                # Keep it switched off to explicitly show the nothing to save state
+                # self.toolbar.toolbar_save_button.setEnabled(True)
+            # Restore saving UI state automatically.
+            QTimer.singleShot(1500, restore_saving_ui_state)
+
+            if self.header is None or not self.header.is_valid():
+                # Get empty file header here, it's needed for compatibility and will not be applied to the file
+                header = FileHeader()
+                if self.logging:
+                    self.logger.info('File "%s" has no header info' % current_file_path)
+            else:
+                header = self.header
 
-                # Update the header with a new date
-                header.refresh()
+            # Update the header with a new date
+            header.refresh()
 
-                # To keep initial content unencrypted
-                content = file_content
-                if self.get_encryption() == Encryption.ENCRYPTED:
-                    # Check file header contains salt and the other params. May update migration params.
-                    # Only if the file is encrypted!
-                    try:
-                        header.validate_enc()
-                    except Exception as e:
-                        if self.logging:
-                            self.logger.error('File header cannot be validated "%s"' % e)
-                    # Get file specific salt
-                    file_salt = header.get_enc_param('slt')
-                    file_iterations = int(header.get_enc_param('itr'))
-
-                    # Encrypt
-                    encrypted_content_b = self.get_encrypt_helper(
-                        salt=file_salt, iterations=file_iterations).encrypt_data(content.encode("utf-8"))
-                    if encrypted_content_b:
-                        content = encrypted_content_b.decode("utf-8")
-
-                content = header.pack(content)
-                save_result = self.save_file_content(current_file_path, content)
-
-                if save_result:
-                    self.header = header
-                    self.content = file_content
-                    # Clear field's data
-                    if clear_after:
-                        edit_widget.clear()
-                else:
-                    self.message_box(self.lexemes.get('save_active_file_error_occurred'), icon_type=2)
+            # To keep initial content unencrypted
+            content = file_content
+            if self.get_encryption() == Encryption.ENCRYPTED:
+                # Check file header contains salt and the other params. May update migration params.
+                # Only if the file is encrypted!
+                try:
+                    header.validate_enc()
+                except Exception as e:
+                    if self.logging:
+                        self.logger.error('File header cannot be validated "%s"' % e)
+                # Get file specific salt
+                file_salt = header.get_enc_param('slt')
+                file_iterations = int(header.get_enc_param('itr'))
+
+                # Encrypt
+                encrypted_content_b = self.get_encrypt_helper(
+                    salt=file_salt, iterations=file_iterations).encrypt_data(content.encode("utf-8"))
+                if encrypted_content_b:
+                    content = encrypted_content_b.decode("utf-8")
+
+            content = header.pack(content)
+            save_result = self.save_file_content(current_file_path, content)
+
+            if save_result:
+                self.header = header
+                self.content = file_content
+                # Clear field's data
+                if clear_after:
+                    edit_widget.clear()
+            else:
+                self.message_box(self.lexemes.get('save_active_file_error_occurred'), icon_type=2)
 
             # Grayscale save button at the toolbar
             if hasattr(self.toolbar, 'toolbar_save_button'):
                 self.toolbar.toolbar_save_button.setDisabled(True)
 
     def toggle_mode(self) -> None:
         """
```

### Comparing `notolog-0.9.1b7/notolog/settings.py` & `notolog-0.9.1b8/notolog/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,21 @@
 
 from .app_config import AppConfig
 from .enums.themes import Themes
 from .enums.languages import Languages
 from .enums.ai_model_names import AiModelNames
 from .helpers.settings_helper import SettingsHelper
 
-from typing import Any, Union
+from typing import TYPE_CHECKING, Any
 
 import logging
 
+if TYPE_CHECKING:
+    from typing import Union  # noqa: F401
+
 
 class Settings(QSettings):
     """
     Class to store app settings params.
     """
 
     value_changed = Signal(object)  # type: Signal[Union[object, QSettings]]
```

### Comparing `notolog-0.9.1b7/notolog/text_block_data.py` & `notolog-0.9.1b8/notolog/text_block_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,26 +38,26 @@
         if existing_data is not None:
             existing_data.update({'opened': opened, 'within': within, 'closed': closed, 'start': start, 'end': end})
             self.data[tag][index] = existing_data
 
     def get_one(self, tag=str, index=0) -> Any:
         """
         This method returns a single piece of list data.
-        Consider to use it with code blocks only where the multiple occurrences are not supported.
+        Consider using it with code blocks only where the multiple occurrences are not supported.
         """
         if (tag in self.data
                 and self.data[tag]
                 and 0 <= index < len(self.data[tag])):
             return self.data[tag][index]
         return None
 
     def get_all(self, tag=str) -> Any:
         """
         This method returns all stored pieces of list data.
-        Consider to use it with the multiple occurrences, like a few strikethrough elements within one line.
+        Consider using it with the multiple occurrences, like a few strikethrough elements within one line.
         """
         if tag in self.data and self.data[tag]:
             return self.data[tag]
         return None
 
     def get_param(self, tag=str, param=str) -> Any:
         item = self.get_one(tag)
```

### Comparing `notolog-0.9.1b7/notolog/theme.py` & `notolog-0.9.1b8/notolog/theme.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/ui/about_popup.py` & `notolog-0.9.1b8/notolog/ui/about_popup.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/ui/ai_assistant.py` & `notolog-0.9.1b8/notolog/ui/ai_assistant.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,62 +192,17 @@
         if self.debug:
             self.logger.debug(f'AI assistant response: {reply}, {error_code}, {status_code}')
 
         # Return the QNetworkReply object that emitted the signal.
         # For example: NetworkError.UnknownNetworkError
         # reply = self.sender()  # type: QNetworkReply
 
-        error = None
         # Make sure there is no error
         if reply.error() == QNetworkReply.NetworkError.NoError:
-            # The request was successful
-            data = reply.readAll()  # type: QByteArray
-
-            if self.debug:
-                self.logger.debug(f'Raw RESPONSE [{status_code}]: {data}')
-
-            reply.deleteLater()  # Clean up the QNetworkReply object
-
-            # json_document = QJsonDocument.fromJson(data)
-            # json_data = json_document.object()
-
-            # Convert QByteArray to string
-            res_string = data.toStdString()  # Or: str(data.data(), encoding='utf-8')
-            if self.debug:
-                self.logger.debug(f'Result multi-line STRING: {res_string}')
-
-            # Clean up the string and make one line
-            json_str = ''.join(line.strip() for line in res_string.splitlines())
-
-            if self.debug:
-                self.logger.debug(f'Result STRING: {json_str}')
-
-            result_message = self.lexemes.get('network_connection_error_empty', scope='common')
-            # Parse JSON response
-            try:
-                json_data = json.loads(json_str)
-                if self.debug:
-                    self.logger.debug(f"Result JSON: {json_data}")
-                if ('choices' in json_data
-                        and len(json_data['choices']) > 0
-                        # Legacy completions
-                        # and 'text' in json_data['choices'][0]):
-                        and 'message' in json_data['choices'][0]
-                        and 'content' in json_data['choices'][0]['message']):
-                    # Legacy completions
-                    # self.response_output.setPlainText(str(json_data['choices'][0]['text']).strip())
-                    self.response_output.setPlainText(str(json_data['choices'][0]['message']['content']).strip())
-                if 'usage' in json_data:
-                    self.update_usage(json_data['usage'])
-                if 'model' in json_data:
-                    if hasattr(self, 'model_label'):
-                        self.model_label.setText(json_data['model'] if len(json_data['model']) > 0 else '?')
-            except json.JSONDecodeError as e:
-                if self.logging:
-                    self.logger.warning("Error decoding JSON: %s" % e)
+            result_message = self.process_response(reply, status_code)
         elif reply.error() == QNetworkReply.NetworkError.HostNotFoundError:
             # The host was not found, indicating possible DNS issues or no internet connection
             result_message = self.lexemes.get('network_connection_error_connection_or_dns', scope='common')
         elif reply.error() == QNetworkReply.NetworkError.ConnectionRefusedError:
             # Connection was refused, indicating the server might be down or there are network issues
             result_message = self.lexemes.get('network_connection_error_connection_refused', scope='common')
         elif reply.error() == QNetworkReply.NetworkError.TimeoutError:
@@ -266,14 +221,63 @@
                 self.logger.warning(result_message)
                 self.logger.warning(f"Failed to fetch update information: {reply.errorString()}")
             # Set up response status visible within response field
             self.response_output.setPlainText(result_message)
 
         self.set_status_ready()
 
+    def process_response(self, reply: QNetworkReply, status_code) -> str:
+        # The request was successful
+        data = reply.readAll()  # type: QByteArray
+
+        if self.debug:
+            self.logger.debug(f'Raw RESPONSE [{status_code}]: {data}')
+
+        reply.deleteLater()  # Clean up the QNetworkReply object
+
+        # json_document = QJsonDocument.fromJson(data)
+        # json_data = json_document.object()
+
+        # Convert QByteArray to string
+        res_string = data.toStdString()  # Or: str(data.data(), encoding='utf-8')
+        if self.debug:
+            self.logger.debug(f'Result multi-line STRING: {res_string}')
+
+        # Clean up the string and make one line
+        json_str = ''.join(line.strip() for line in res_string.splitlines())
+
+        if self.debug:
+            self.logger.debug(f'Result STRING: {json_str}')
+
+        result_message = self.lexemes.get('network_connection_error_empty', scope='common')
+        # Parse JSON response
+        try:
+            json_data = json.loads(json_str)
+            if self.debug:
+                self.logger.debug(f"Result JSON: {json_data}")
+            if ('choices' in json_data
+                    and len(json_data['choices']) > 0
+                    # Legacy completions
+                    # and 'text' in json_data['choices'][0]):
+                    and 'message' in json_data['choices'][0]
+                    and 'content' in json_data['choices'][0]['message']):
+                # Legacy completions
+                # self.response_output.setPlainText(str(json_data['choices'][0]['text']).strip())
+                self.response_output.setPlainText(str(json_data['choices'][0]['message']['content']).strip())
+            if 'usage' in json_data:
+                self.update_usage(json_data['usage'])
+            if 'model' in json_data:
+                if hasattr(self, 'model_label'):
+                    self.model_label.setText(json_data['model'] if len(json_data['model']) > 0 else '?')
+        except json.JSONDecodeError as e:
+            if self.logging:
+                self.logger.warning("Error decoding JSON: %s" % e)
+
+        return result_message
+
     def update_usage(self, usage: dict = None):
         if hasattr(self, 'tokens_prompt_label'):
             prompt_tokens_cnt = (usage['prompt_tokens'] if usage and 'prompt_tokens' in usage else 0)
             self.tokens_prompt_label.setText(self.lexemes.get('dialog_usage_tokens_prompt',
                                                               tokens=prompt_tokens_cnt))
         if hasattr(self, 'tokens_answer_label'):
             answer_tokens_cnt = (usage['completion_tokens'] if usage and 'completion_tokens' in usage else 0)
```

### Comparing `notolog-0.9.1b7/notolog/ui/color_picker_dialog.py` & `notolog-0.9.1b8/notolog/ui/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/ui/common_dialog.py` & `notolog-0.9.1b8/notolog/ui/common_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/ui/enum_combo_box.py` & `notolog-0.9.1b8/notolog/ui/enum_combo_box.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/ui/file_system_model.py` & `notolog-0.9.1b8/notolog/ui/file_system_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from PySide6.QtCore import Qt, QModelIndex
+from PySide6.QtCore import Qt
 from PySide6.QtGui import QColor
 from PySide6.QtWidgets import QFileSystemModel
 
 import os
 
 from typing import Any
```

### Comparing `notolog-0.9.1b7/notolog/ui/line_numbers.py` & `notolog-0.9.1b8/notolog/ui/line_numbers.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,25 +2,29 @@
 # The bale functions are:
 # - Show line/block number for better text recognition.
 # - Highlight current line where the cursor located.
 
 # If used with PyQt6 make sure slots and signals are declared correctly, as there are some differences:
 # from PyQt6.QtCore import pyqtSlot as Slot
 
-from PySide6.QtCore import Qt, QObject, QRect, QSize, Slot
+from PySide6.QtCore import Qt, QRect, QSize, Slot
 from PySide6.QtWidgets import QWidget, QTextEdit, QPlainTextEdit
-from PySide6.QtGui import QPainter, QColor, QTextFormat, QTextCharFormat, QFont
+from PySide6.QtGui import QPainter, QColor, QTextFormat
 
-from typing import Union
+from typing import TYPE_CHECKING, Union
 
 from . import Settings
 from . import ThemeHelper
 
 from ..edit_widget import EditWidget
 
+if TYPE_CHECKING:
+    from PySide6.QtCore import QObject  # noqa: F401
+    from PySide6.QtGui import QTextCharFormat  # noqa: F401
+
 
 class LineNumbers(QWidget):
     def __init__(self, editor: Union[EditWidget, QPlainTextEdit] = None):
         QWidget.__init__(self, editor)
 
         self.editor = editor
 
@@ -36,15 +40,16 @@
         self.theme_helper = ThemeHelper()
 
         # Settings
         self.settings = Settings(parent=self)
 
         editor.updateRequest.connect(self.update_request)
         editor.blockCountChanged.connect(self.update_width)
-        # TODO set up in settings and find out the better way to highlight the line (when mixing backgrounds)
+        # TODO: Improve line highlighting on hover.
+        # Current method of mixing background colors does not yield clear results.
         # editor.cursorPositionChanged.connect(self.highlight_current_line)
 
         # Init object with direct updates
         self.update_numbers()
 
         # self.highlight_current_line()
 
@@ -75,16 +80,17 @@
             if not selection:
                 return
             selection.cursor = self.editor.textCursor()
             selection.cursor.clearSelection()
             # Set selection properties
             # line_color = QColor(Qt.GlobalColor.green).lighter(175)  # As an example of how to shift base color tone
             line_color = QColor(self.theme_helper.get_color('edit_widget_line_numbers_active_line_background'))
-            selection.format.setBackground(line_color)
-            selection.format.setProperty(QTextFormat.Property.FullWidthSelection, True)
+            _format = selection.format  # type: ignore
+            _format.setBackground(line_color)
+            _format.setProperty(QTextFormat.Property.FullWidthSelection, True)
             # extra_selections.append(selection)
             self.editor.setExtraSelections([selection])
 
     def update_numbers(self) -> None:
         # Get element parent's contents size as the text edit widget may not be resized yet
         parent_obj = self.editor.parent()  # type: Union[QObject, QWidget]
         element_cr = parent_obj.contentsRect()
@@ -157,8 +163,8 @@
 
         digits = max(2, len(str(self.editor.blockCount())))
         # '5' is an overall value of left and right padding
         space = 5 + self.fontMetrics().horizontalAdvance("0") * digits
         return space
 
     def visible(self) -> bool:
-        return self.settings.show_line_numbers
+        return self.settings.show_line_numbers
```

### Comparing `notolog-0.9.1b7/notolog/ui/rename_file_dialog.py` & `notolog-0.9.1b8/notolog/ui/rename_file_dialog.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from PySide6.QtCore import Signal, QSize
+from PySide6.QtCore import QSize
 from PySide6.QtWidgets import QInputDialog, QLineEdit, QDialogButtonBox, QSizePolicy
 
 from . import Settings
 from . import AppConfig
 from . import Lexemes
 
 import logging
```

### Comparing `notolog-0.9.1b7/notolog/ui/rotating_label.py` & `notolog-0.9.1b8/notolog/ui/rotating_label.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/ui/settings_dialog.py` & `notolog-0.9.1b8/notolog/ui/settings_dialog.py`

 * *Files 0% similar despite different names*

```diff
@@ -337,15 +337,16 @@
     def apply_props(self, widget, properties):
         for prop, value in properties.items():
             # Get the method based on the property name
             setter = getattr(widget, prop, None)
             if callable(setter):
                 setter(value)  # Call the setter with the provided value
 
-    def create_setting_field(self, conf) -> Union[QCheckBox, QLineEdit, QPlainTextEdit, QComboBox, QSpinBox, QSlider]:
+    def create_setting_field(self, conf) \
+            -> Union[QCheckBox, QLineEdit, QPlainTextEdit, QComboBox, QSpinBox, QSlider]:  # noqa: C901
         """
         Method to create setting field with ease.
         @param conf: Config of the field. As the param bounded to the particular method it will be called then.
         @return: Any object instance
         """
         args = conf['args'] if 'args' in conf else [self]
         obj = conf['type'](*args)  # type: conf['type']
@@ -379,14 +380,15 @@
             if isinstance(params, tuple):
                 obj.setSizePolicy(*params)  # Contains a few params
             else:
                 obj.setSizePolicy(params)
         if 'alignment' in conf:
             obj.setAlignment(conf['alignment'])
         if 'callback' in conf and callable(conf['callback']):
+            # Add object to the layout via the callback
             conf['callback'](obj)
         if 'style' in conf:
             styles = []
             if 'bold' in conf['style']:
                 styles.append('font-weight: bold;')  # Bold
             if 'italic' in conf['style']:
                 styles.append('font-style: italic;')  # Italic
@@ -411,15 +413,15 @@
             else:
                 if self.logging:
                     self.logger.warning(f"Object name in a wrong format {object_name}")
         else:
             # lexeme_key, setting_name
             return object_name, object_name
 
-    def connect_widgets(self):
+    def connect_widgets(self):  # noqa: C901 - consider simplifying this method
         # Find children of type QCheckBox
         checkboxes = self.findChildren(QCheckBox)
         for checkbox in checkboxes:
             if isinstance(checkbox, QCheckBox):
                 # Parse object name in case it consists of composed data of lexeme and setting names
                 _lexeme_key, setting_name = self.parse_object_name(checkbox.objectName())
                 if hasattr(self.settings, setting_name):
@@ -483,15 +485,15 @@
             if isinstance(slider, QSlider):
                 # Parse object name in case it consists of composed data of lexeme and setting names
                 _lexeme_key, setting_name = self.parse_object_name(slider.objectName())
                 if hasattr(self.settings, setting_name):
                     slider.setValue(getattr(self.settings, setting_name, 0))
                 slider.valueChanged.connect(self.save_settings)
 
-    def save_settings(self):
+    def save_settings(self):  # noqa: C901 - consider simplifying this method
         # Signal sender
         sender = self.sender()
 
         # Determine which widget emitted the signal by the object name set
         sender_widget = self.sender()
         sender_name = sender_widget.objectName()
```

### Comparing `notolog-0.9.1b7/notolog/ui/sort_filter_proxy_model.py` & `notolog-0.9.1b8/notolog/ui/sort_filter_proxy_model.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog/ui/statusbar.py` & `notolog-0.9.1b8/notolog/ui/statusbar.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 from PySide6.QtCore import Qt
 from PySide6.QtGui import QColor
 from PySide6.QtWidgets import QStatusBar, QWidget, QLabel, QPushButton, QSizePolicy
 
 import logging
-from typing import Union
+from typing import TYPE_CHECKING
 
 from . import Settings
 from . import AppConfig
 from . import Lexemes
 from . import ThemeHelper
 
 from .sort_filter_proxy_model import SortFilterProxyModel
 from .vertical_line_spacer import VerticalLineSpacer
 
+if TYPE_CHECKING:
+    from typing import Union  # noqa
+
 
 class StatusBar(QStatusBar):
     def __init__(self, parent=None):
         super().__init__(parent)
 
         self.parent = parent
 
@@ -122,21 +125,23 @@
                 and hasattr(self.parent, 'tree_proxy_model')
                 and isinstance(self.parent.tree_proxy_model, SortFilterProxyModel)):
             # Get tree proxy model to obtain the data
             tree_proxy_model = self.parent.tree_proxy_model  # type: SortFilterProxyModel
             if visible:
                 # Add 'deleted' extension to the tree
                 tree_proxy_model.add_extension('del'),
-                self.litter_bin_label.setIcon(self.theme_helper.get_icon(theme_icon='trash3-fill.svg',
+                self.litter_bin_label.setIcon(self.theme_helper.get_icon(
+                    theme_icon='trash3-fill.svg',
                     color=QColor(self.theme_helper.get_color('statusbar_litter_bin_icon_color_active'))))
                 self.settings.show_deleted_files = True
             else:
                 # Remove 'deleted' extension from the tree
                 tree_proxy_model.remove_extension('del'),
-                self.litter_bin_label.setIcon(self.theme_helper.get_icon(theme_icon='trash3.svg',
+                self.litter_bin_label.setIcon(self.theme_helper.get_icon(
+                    theme_icon='trash3.svg',
                     color=QColor(self.theme_helper.get_color('statusbar_litter_bin_icon_color'))))
                 self.settings.show_deleted_files = False
 
     def __getitem__(self, name) -> QLabel:
         """
         To get items like:
             self.statusbar['mode_label']
@@ -160,8 +165,7 @@
         else:
             if (isinstance(value, QLabel)
                     or isinstance(value, QPushButton)
                     or value is None):
                 self._elements[name] = value
             elif self.logging:
                 self.logger.warning(f'Trying to set object that is not a QLabel type {type(value)}')
-
```

### Comparing `notolog-0.9.1b7/notolog/ui/toolbar.py` & `notolog-0.9.1b8/notolog/ui/toolbar.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,21 @@
 from PySide6.QtWidgets import QSizePolicy
 
 from . import Settings
 from . import AppConfig
 from . import Lexemes
 from . import ThemeHelper
 
-from typing import Union
+from typing import TYPE_CHECKING
 
 import logging
 
+if TYPE_CHECKING:
+    from typing import Union  # noqa
+
 
 class ToolBar(QToolBar):
     # Main window toolbar class
 
     def __init__(self, parent=None, actions=None, buttons=None, refresh=None):
         """
         Args:
@@ -254,24 +257,28 @@
             if _weights & settings_weight:
                 # The item is already added or the active state item that shouldn't be duplicated
                 continue
 
             button = QAction(label['label'], self)
             button.setFont(self.font())
 
-            slot = lambda checked, i=label['weight']: self.toolbar_menu_item(checked, i)
+            # Method def instead of lambda
+            def slot(checked, i=label['weight']):
+                self.toolbar_menu_item(checked, i)
+
             # Check button.toggled.connect()
             button.triggered[bool].connect(slot)
             button.setCheckable(True)
             # Check the item is in the settings weights
             button.setChecked(self.settings.toolbar_icons & settings_weight)
 
             menu.addAction(button)
 
-            self.buttons[index] = button
+            if index in self.buttons:
+                self.buttons[index] = button
 
             # Collect items already added to the context menu
             _weights |= settings_weight
 
         # PoC remove element from the toolbar
         # delete_action  = menu.addAction("Hide")
```

### Comparing `notolog-0.9.1b7/notolog/view_decorator.py` & `notolog-0.9.1b8/notolog/view_decorator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,22 @@
-from PySide6.QtCore import Qt, QObject
-from PySide6.QtGui import QTextCursor, QSyntaxHighlighter, QTextBlockUserData
-from PySide6.QtWidgets import QTextBrowser
+from PySide6.QtGui import QTextCursor, QSyntaxHighlighter
 
 import logging
 
-from typing import Union
+from typing import TYPE_CHECKING, Union
 
 from .settings import Settings
 from .app_config import AppConfig
 from .highlight.view_highlighter import ViewHighlighter
-from .text_block_data import TextBlockData
+
+if TYPE_CHECKING:
+    from PySide6.QtCore import QObject  # noqa: F401
+    from PySide6.QtGui import QTextBlockUserData  # noqa: F401
+    from PySide6.QtWidgets import QTextBrowser  # noqa: F401
+    from .text_block_data import TextBlockData  # noqa: F401
 
 
 class ViewDecorator:
     """
     View mode result decoration by modifying loaded QTextDocument.
     The source of the data comes from the userData() attached to a block within ViewHighlighter.
     """
@@ -69,15 +72,15 @@
     def process(self):
         cursor = QTextCursor(self.doc)
         cursor.movePosition(QTextCursor.MoveOperation.Start)
         while not (cursor.atEnd()
                    # Sometimes, cursor.atEnd() doesn't work as the cursor unable to move next block at the very end
                    or (cursor.block().blockNumber() > 0 and cursor.block().blockNumber() == self.doc.blockCount() - 1)):
             current_block = cursor.block()
-            current_block_number = current_block.blockNumber()
+            # current_block_number = current_block.blockNumber()
             block_pos = current_block.position()
 
             for tag, oi, ci, fmt_key, repl in self.rules:
                 if tag == 'todo' and not self.settings.viewer_highlight_todos:
                     continue
                 if repl is None:
                     repl = ""
```

### Comparing `notolog-0.9.1b7/notolog/view_processor.py` & `notolog-0.9.1b8/notolog/view_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,25 @@
-from PySide6.QtCore import Qt, QObject, QUrl
+from PySide6.QtCore import Qt, QUrl
 from PySide6.QtWidgets import QTextBrowser
 from PySide6.QtGui import QTextCursor, QSyntaxHighlighter, QTextCharFormat
 
 import logging
 import re
 import base64
 
-from typing import Union
+from typing import TYPE_CHECKING, Union
 
 from .settings import Settings
 from .app_config import AppConfig
 from .highlight.view_highlighter import ViewHighlighter
 from .lexemes.lexemes import Lexemes
 
+if TYPE_CHECKING:
+    from PySide6.QtCore import QObject  # noqa: F401
+
 
 class ViewProcessor:
     """
     View mode pre-result procession by modifying loaded QTextDocument
     """
 
     def __init__(self, highlighter: Union[QSyntaxHighlighter, ViewHighlighter]):
```

### Comparing `notolog-0.9.1b7/notolog/view_widget.py` & `notolog-0.9.1b8/notolog/view_widget.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/notolog.egg-info/PKG-INFO` & `notolog-0.9.1b8/notolog.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,63 +1,82 @@
 Metadata-Version: 2.1
 Name: notolog
-Version: 0.9.1b7
+Version: 0.9.1b8
 Summary: Notolog - Python Markdown Editor
 Home-page: https://github.com/notolog/notolog-editor
 Author: Vadim Bakhrenkov
 License: MIT
 Project-URL: Bug Reports, https://github.com/notolog/notolog-editor/issues
 Project-URL: Source, https://github.com/notolog/notolog-editor/
 Keywords: notolog,python,markdown,editor,ai,text,notes
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Topic :: Text Editors
 Classifier: Topic :: Text Editors :: Documentation
 Classifier: Topic :: Text Editors :: Emacs
 Classifier: Topic :: Text Editors :: Integrated Development Environments (IDE)
 Classifier: Topic :: Text Editors :: Text Processing
 Classifier: Topic :: Text Editors :: Word Processors
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Text Processing :: General
 Classifier: Topic :: Text Processing :: Markup :: Markdown
+Classifier: Natural Language :: Chinese (Simplified)
+Classifier: Natural Language :: Dutch
+Classifier: Natural Language :: English
+Classifier: Natural Language :: Finnish
+Classifier: Natural Language :: French
+Classifier: Natural Language :: Georgian
+Classifier: Natural Language :: German
+Classifier: Natural Language :: Greek
+Classifier: Natural Language :: Hindi
+Classifier: Natural Language :: Italian
+Classifier: Natural Language :: Japanese
+Classifier: Natural Language :: Korean
+Classifier: Natural Language :: Latin
+Classifier: Natural Language :: Portuguese
+Classifier: Natural Language :: Russian
+Classifier: Natural Language :: Spanish
+Classifier: Natural Language :: Swedish
+Classifier: Natural Language :: Turkish
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: cffi==1.16.0
+Requires-Dist: cffi==1.17.0rc1
 Requires-Dist: click==8.1.7
 Requires-Dist: cryptography==42.0.7
-Requires-Dist: emoji==2.11.1
+Requires-Dist: emoji==2.12.1
 Requires-Dist: iniconfig==2.0.0
 Requires-Dist: Markdown==3.6
 Requires-Dist: packaging==24.0
 Requires-Dist: pluggy==1.5.0
 Requires-Dist: pycparser==2.22
 Requires-Dist: Pygments==2.18.0
-Requires-Dist: PySide6==6.7.0
-Requires-Dist: PySide6_Addons==6.7.0
-Requires-Dist: PySide6_Essentials==6.7.0
-Requires-Dist: pytest==8.2.0
-Requires-Dist: pytest-asyncio==0.23.6
-Requires-Dist: pytest-mock==3.14.0
+Requires-Dist: PySide6==6.7.1
+Requires-Dist: PySide6_Addons==6.7.1
+Requires-Dist: PySide6_Essentials==6.7.1
 Requires-Dist: qasync==0.27.1
-Requires-Dist: shiboken6==6.7.0
+Requires-Dist: shiboken6==6.7.1
 Requires-Dist: tomli==2.0.1
 Requires-Dist: tomli_w==1.0.0
+Requires-Dist: typing_extensions==4.12.0
 
-<!-- {"notolog.app": {"created": "2023-12-25 18:59:43.806614", "updated": "2024-05-19 23:29:34.439703"}} -->
+<!-- {"notolog.app": {"created": "2023-12-25 18:59:43.806614", "updated": "2024-05-25 16:38:26.173086"}} -->
 # Notolog
 
 ![Notolog - Python Markdown Editor](https://raw.githubusercontent.com/notolog/notolog-editor/main/notolog/assets/notolog-example-image.png)
 
 ## Python Markdown Editor
 
 [![PyPI - Version](https://img.shields.io/pypi/v/notolog)](https://pypi.org/project/notolog/) [![GitHub License](https://img.shields.io/github/license/notolog/notolog-editor)](https://github.com/notolog/notolog-editor/blob/master/LICENSE) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/notolog)](https://pypi.org/project/notolog/) [![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/notolog/notolog-editor/tests.yaml)](https://github.com/notolog/notolog-editor/actions/workflows/tests.yaml)
@@ -131,14 +150,15 @@
 * Swedish
 * Turkish
 
 Here's an example of what it looks like in the actual UI, featuring the lovely Strawberry theme and Japanese translation:
 
 ![Notolog UI translation example](https://raw.githubusercontent.com/notolog/notolog-editor/main/docs/notolog-ui-settings-strawberry-ja.png)
 
+
 ## Prerequisites
 
 **Python 3.9 or higher installed on your system.**
 
 Ensure Python 3.9 or higher is installed on your system. Visit [python.org](https://python.org) for more details.
 
 Check the version of Python available with this command `python3 -V`.
@@ -178,25 +198,47 @@
 
 ```sh
 pip install -r requirements.txt
 ```
 
 That's it! Starting the app is as simple as `python -m notolog.main` form the project's root directory.
 
+### Tests and Test Coverage
+
+To minimize installation overhead and streamline dependency management, dependencies required solely for testing are isolated in `test_requirements.txt`. This separation helps manage test dependencies independently from the main application dependencies.
+
+```sh
+pip install -r test_requirements.txt
+```
+
 <details>
-<summary>Run tests</summary>
+<summary>Run Tests</summary>
 
-To run all available tests:
+To execute all available tests:
 ```sh
 pytest
 ```
 
-To run a particular file's tests:
+To run tests from a specific file:
 ```sh
-pytest tests/test_notolog_editor.py
+pytest tests/test_pkg_integration.py
+```
+</details>
+
+<details>
+<summary>Run Tests with Coverage Reports</summary>
+
+To run all tests with a coverage report:
+```sh
+pytest tests/ --cov=notolog --cov-report=term
+```
+
+Alternatively, to exclude UI tests from execution:
+```sh
+pytest tests/ --cov=notolog --cov-report=term --ignore=tests/ui_tests/
 ```
 </details>
 
 ### Virtual Environments
 
 The instructions below contain steps of how to set up **venv** virtual environment to run a Python app safely. Starting from Python 3.6 **venv** is a recommended way to create virtual environments. For more information check [Creation of virtual environments](https://docs.python.org/3/library/venv.html). Alternatively, you can execute the Notolog code and set up virtual environment with your favorite Python code editor.
 
@@ -260,110 +302,116 @@
 _Mind the environment name (**notolog** or any other selected before)._
 
 
 ## Contributing
 
 If you encounter any issues or would like to contribute to the project, please don't hesitate to [open an issue](https://github.com/notolog/notolog-editor/issues) or submit a [pull request](https://github.com/notolog/notolog-editor/pulls) on the project's [GitHub page](https://github.com/notolog/notolog-editor).
 
+
 ## License
 
 The Notolog project is licensed under the MIT License - see the [LICENSE](https://github.com/notolog/notolog-editor/blob/main/LICENSE) file for details.
 
+
 ## Third-Party Components
 
 ### Libraries and Licenses
 
-This project utilizes numerous third-party libraries, each with its own licensing terms. Below is a detailed list of these libraries grouped by license type to help clarify what each license permits and requires. This categorization aids in ensuring compliance with legal terms for use, modification, and distribution of these software components.
+This project incorporates numerous third-party libraries, each subject to its own licensing terms. Below is a detailed list of these libraries, categorized by license type to facilitate understanding of what each license permits and requires. This organization helps ensure compliance with legal terms for the use, modification, and distribution of these components.
 
 #### GNU LGPLv3, GNU GPLv2, or Commercial License
 
-- **Qt (open-source)**: Framework for graphical user interfaces and more. [Project Details](https://www.qt.io), [Qt Licensing](https://www.qt.io/licensing)
-- **PySide6**: GUI creation with Qt6 in Python. [Project and License Details](https://pyside.org/), [PyPI](https://pypi.org/project/PySide6/)
-- **PySide6_Addons**: Additional modules for PySide6. [Project and License Details](https://pyside.org/), [PyPI](https://pypi.org/project/PySide6-Addons/)
+- **Qt (open-source)**: A framework for graphical user interfaces and more. [Project Details](https://www.qt.io), [Qt Licensing](https://www.qt.io/licensing)
+- **PySide6**: Enables GUI creation with Qt6 in Python. [Project and License Details](https://pyside.org/), [PyPI](https://pypi.org/project/PySide6/)
+- **PySide6_Addons**: Provides additional modules for PySide6. [Project and License Details](https://pyside.org/), [PyPI](https://pypi.org/project/PySide6-Addons/)
 - **PySide6_Essentials**: Core libraries for PySide6. [Project and License Details](https://pyside.org/), [PyPI](https://pypi.org/project/PySide6-Essentials/)
-- **shiboken6**: Binding generator for Qt framework. [Project and License Details](https://pyside.org/), [PyPI](https://pypi.org/project/shiboken6/)
+- **shiboken6**: Binding generator for the Qt framework. [Project and License Details](https://pyside.org/), [PyPI](https://pypi.org/project/shiboken6/)
 
 #### MIT License
 
 - **Bootstrap Icons**: Icons for UI elements. [Project Details](https://icons.getbootstrap.com/), [License Details](https://github.com/twbs/icons/blob/main/LICENSE)
-- **pytest**: Used for unit testing. It provides powerful features like fixtures, assertions, and test parameterization to facilitate writing and running Python tests. [Project Details](https://pytest.org/), [License Details](https://docs.pytest.org/en/8.0.x/license.html)
-- **pytest-mock**: Enhances pytest for unit tests by offering a simple interface to powerful mocking functionalities. [License Details](https://github.com/pytest-dev/pytest-mock/blob/main/LICENSE), [PyPI](https://pypi.org/project/pytest-mock/)
-- **cffi**: Used for interfacing with C code. [License Details](https://github.com/python-cffi/cffi/blob/main/LICENSE), [PyPI](https://pypi.org/project/cffi/)
-- **iniconfig**: For parsing and working with INI configuration files. [License Details](https://github.com/pytest-dev/iniconfig/blob/main/LICENSE), [PyPI](https://pypi.org/project/iniconfig/)
-- **tomli**: A Python library used for parsing TOML configuration files effortlessly. [License Details](https://github.com/hukkin/tomli/blob/master/LICENSE), [PyPI](https://pypi.org/project/tomli/)
-- **tomli_w**: A Python library used for writing TOML configuration files effortlessly. [License Details](https://github.com/hukkin/tomli-w/blob/master/LICENSE), [PyPI](https://pypi.org/project/tomli-w/)
-- **pluggy**: For creating and managing plugin systems in Python applications. [License Details](https://github.com/pytest-dev/pluggy/blob/main/LICENSE), [PyPI](https://pypi.org/project/pluggy/)
+- **cffi**: For interfacing with C code. [License Details](https://github.com/python-cffi/cffi/blob/main/LICENSE), [PyPI](https://pypi.org/project/cffi/)
+- **iniconfig**: For parsing and managing INI configuration files. [License Details](https://github.com/pytest-dev/iniconfig/blob/main/LICENSE), [PyPI](https://pypi.org/project/iniconfig/)
+- **tomli**: Effortlessly parses TOML configuration files. [License Details](https://github.com/hukkin/tomli/blob/master/LICENSE), [PyPI](https://pypi.org/project/tomli/)
+- **tomli_w**: For writing TOML configuration files effortlessly. [License Details](https://github.com/hukkin/tomli-w/blob/master/LICENSE), [PyPI](https://pypi.org/project/tomli-w/)
+- **pluggy**: Facilitates the creation and management of plugin systems. [License Details](https://github.com/pytest-dev/pluggy/blob/main/LICENSE), [PyPI](https://pypi.org/project/pluggy/)
 
 #### BSD Licenses
 
-- **Python-Markdown**: Markdown to HTML conversion. [Project Details](https://python-markdown.github.io/), [BSD 3-Clause License](https://github.com/Python-Markdown/markdown/blob/master/LICENSE.md)
-- **Emoji library**: Converts emoji text-code to emojis. [New BSD License](https://github.com/carpedm20/emoji/blob/master/LICENSE.txt), [PyPI](https://pypi.org/project/emoji/)
-- **qasync**: Async support for Python. [BSD 2-Clause "Simplified" License](https://github.com/CabbageDevelopment/qasync/blob/master/LICENSE), [PyPI](https://pypi.org/project/qasync/)
-- **Pygments**: Syntax highlighting for programming languages. [Project Details](https://pygments.org/), [BSD 2-Clause "Simplified" License](https://github.com/pygments/pygments/blob/master/LICENSE)
-- **click**: Used for creating command-line interfaces. [Project Details](https://palletsprojects.com/p/click/), [BSD-3-Clause License](https://click.palletsprojects.com/en/8.1.x/license/)
-- **pycparser**: C code parser and for generating Abstract Syntax Trees (AST) in Python. [BSD 3-Clause License](https://github.com/eliben/pycparser/blob/main/LICENSE), [PyPI](https://pypi.org/project/pycparser/)
-
-#### Apache License 2.0
-
-- **pytest-asyncio**: A library that provides support for testing asyncio code with pytest. [License Details](https://github.com/pytest-dev/pytest-asyncio/blob/main/LICENSE) , [PyPI](https://pypi.org/project/pytest-asyncio/)
+- **Python-Markdown**: Converts Markdown to HTML. [Project Details](https://python-markdown.github.io/), [BSD 3-Clause License](https://github.com/Python-Markdown/markdown/blob/master/LICENSE.md)
+- **Emoji library**: Converts emoji text-codes to emojis. [New BSD License](https://github.com/carpedm20/emoji/blob/master/LICENSE.txt), [PyPI](https://pypi.org/project/emoji/)
+- **qasync**: Adds async support to Python. [BSD 2-Clause "Simplified" License](https://github.com/CabbageDevelopment/qasync/blob/master/LICENSE), [PyPI](https://pypi.org/project/qasync/)
+- **Pygments**: Provides syntax highlighting for programming languages. [Project Details](https://pygments.org/), [BSD 2-Clause "Simplified" License](https://github.com/pygments/pygments/blob/master/LICENSE)
+- **click**: Creates command-line interfaces. [Project Details](https://palletsprojects.com/p/click/), [BSD-3-Clause License](https://click.palletsprojects.com/en/8.1.x/license/)
+- **pycparser**: A C code parser; generates Abstract Syntax Trees in Python. [BSD 3-Clause License](https://github.com/eliben/pycparser/blob/main/LICENSE), [PyPI](https://pypi.org/project/pycparser/)
 
 #### Other Dual Licensed
 
 - **cryptography**: Provides cryptographic functions and primitives. [Apache License 2.0](https://github.com/pyca/cryptography/blob/main/LICENSE.APACHE) and [BSD 3-Clause License](https://github.com/pyca/cryptography/blob/main/LICENSE.BSD), [PyPI](https://pypi.org/project/cryptography/)
-- **packaging**: Python package metadata and distribution utilities. [Apache License 2.0](https://github.com/pypa/packaging/blob/main/LICENSE.APACHE) and [BSD 2-Clause "Simplified" License](https://github.com/pypa/packaging/blob/main/LICENSE.BSD), [PyPI](https://pypi.org/project/packaging/)
-
-#### Python Standard Library
+- **packaging**: Handles metadata and distribution for Python packages. [Apache License 2.0](https://github.com/pypa/packaging/blob/main/LICENSE.APACHE) and [BSD 2-Clause "Simplified" License](https://github.com/pypa/packaging/blob/main/LICENSE.BSD), [PyPI](https://pypi.org/project/packaging/)
 
-- **asyncio**: Part of the Python standard library, licensed under the [Python Software Foundation License](https://docs.python.org/3/license.html#psf-license).
+#### Python Software Foundation License
+- **typing_extensions**: Enhances support for type hints on older versions of Python. Licensed under the [Python Software Foundation License](https://github.com/python/typing_extensions/blob/main/LICENSE), [PyPI](https://pypi.org/project/typing-extensions/).
+- **Standard Python Libraries**: Includes commonly used libraries such as `asyncio` and `unittest`. All are part of the Python standard library and are licensed under the [Python Software Foundation License](https://docs.python.org/3/license.html#psf-license). This includes any other standard libraries not explicitly mentioned but used in the project.
 
 #### The Unlicense
 
-- **Codehilite CSS Themes**: Base themes for code highlighting. [The Unlicense](https://github.com/richleland/pygments-css/blob/master/UNLICENSE.txt)
+- **Codehilite CSS Themes**: Basic themes for code highlighting. [The Unlicense](https://github.com/richleland/pygments-css/blob/master/UNLICENSE.txt)
 
 Please note that while the majority of this project is licensed under the MIT License, certain components may have different licensing terms. Always refer to the documentation of each library for detailed information about its license and terms of use.
 
+
 ### APIs
 
 #### OpenAI API Disclaimer
 
 **Disclaimer:** This project is independent and not affiliated with, endorsed by, or sponsored by OpenAI. The integration of the OpenAI API is provided on an "as is" basis, and the creators disclaim all liability for any misuse or consequences resulting from the use of the OpenAI API.
 
 **Usage:** This project uses the OpenAI API to access AI assistant capabilities and enhance natural language processing. Users must provide their own OpenAI API keys and should refer to the [OpenAI API reference](https://platform.openai.com/docs/api-reference) for detailed usage guidelines.
 
 **Responsibility:** Users are responsible for obtaining and managing their OpenAI API keys in compliance with OpenAI's terms of service.
 
 **Security:** Users are expected to handle their API keys securely to avoid unauthorized access.
 
 *This section was generated with the assistance of AI to ensure accurate and concise information regarding the use of the OpenAI API.*
 
+
 ## Security Disclaimer
 
 This application is designed for educational purposes and offers security features through optional file encryption and protected application settings.
 
 ### Optional File Encryption
 
-* **Encryption Details:** The application uses PBKDF2HMAC for key derivation and Fernet for encryption, utilizing AES-128 in CBC mode. Although the key material generated is 256 bits, only the first 128 bits (16 bytes) are used for encryption.
-* **File Headers:** The encryption salt and iteration counts are stored unencrypted in the file's header. This approach is primarily intended for non-critical applications where data exposure has limited risk.
-* **Strong Passwords:** Users are encouraged to use strong passwords to enhance the protection of their encrypted data.
+- **Encryption Details**: The application uses PBKDF2HMAC for key derivation and Fernet for encryption, utilizing AES-128 in CBC mode. Although the key material generated is 256 bits, only the first 128 bits (16 bytes) are used for encryption.
+- **File Headers**: The encryption salt and iteration counts are stored unencrypted in the file's header. This approach is primarily intended for non-critical applications where data exposure has limited risk.
+- **Strong Passwords**: Users are encouraged to use strong passwords to enhance the protection of their encrypted data.
 
 ### Protected Application Settings
 
-* **Settings Encryption:** The application may encrypt sensitive data like API keys because these Qt app settings might otherwise be stored as open data. However, the encryption key used is stored on the PC and can be accessed by anyone with physical or user-level access to the computer. This could expose sensitive data to potential unauthorized access.
+- **Settings Encryption**: The application may encrypt sensitive data like API keys because these Qt app settings might otherwise be stored as open data. However, the encryption key used is stored on the PC and can be accessed by anyone with physical or user-level access to the computer. This could expose sensitive data to potential unauthorized access.
 
 ### General Information
 
-* **Open Source:** This application is open-source and distributed under the MIT License. Users must comply with applicable laws and regulations when using this software.
-* **Liability:** The developers disclaim any liability for misuse or legal non-compliance related to the use of this software.
+- **Open Source**: This application is open-source and distributed under the MIT License. Users must comply with applicable laws and regulations when using this software.
+- **Liability**: The developers disclaim any liability for misuse or legal non-compliance related to the use of this software.
 
 
-## Code Quality and Test Coverage
+## Development and Testing Tools
 
 To maintain high standards of code quality and ensure comprehensive test coverage, we use several tools:
 
-- **Flake8**: A tool that enforces coding style and checks the quality of Python code by combining PyFlakes, pycodestyle, and McCabe's complexity checker. [MIT License](https://github.com/PyCQA/flake8/blob/main/LICENSE)
-- **coverage**: Measures the effectiveness of tests by showing which parts of your code are being executed and which are not. [Apache License 2.0](https://github.com/nedbat/coveragepy/blob/master/LICENSE.txt)
-- **pytest-cov**: A pytest plugin that provides test coverage reports, extending pytest to measure code coverage alongside running tests. [MIT License](https://github.com/pytest-dev/pytest-cov/blob/master/LICENSE)
+- **coverage**: Measures the code coverage of our tests, helping to ensure that all parts of the application are properly tested. [License](https://github.com/nedbat/coveragepy/blob/master/LICENSE.txt), [PyPI](https://pypi.org/project/coverage/).
+- **flake8**: A tool that enforces coding style and checks the quality of Python code by combining PyFlakes, pycodestyle, and McCabe's complexity checker. [MIT License](https://github.com/PyCQA/flake8/blob/main/LICENSE), [PyPI](https://pypi.org/project/flake8/).
+  - **mccabe**: Analyzes code complexity, which can help in identifying overly complex code that may need simplification. [License](https://github.com/PyCQA/mccabe/blob/master/LICENSE), [PyPI](https://pypi.org/project/mccabe/).
+  - **pycodestyle**: A tool to check Python code against coding style conventions in PEP 8. [License](https://github.com/PyCQA/pycodestyle/blob/main/LICENSE), [PyPI](https://pypi.org/project/pycodestyle/).
+  - **pyflakes**: Analyzes Python programs and detects various errors like undefined names. [License](https://github.com/PyCQA/pyflakes/blob/main/LICENSE), [PyPI](https://pypi.org/project/pyflakes/).
+- **pytest**: Provides a powerful framework for writing and running Python tests, including support for complex test setups. [License](https://docs.pytest.org/en/8.0.x/license.html), [PyPI](https://pypi.org/project/pytest/).
+- **pytest-asyncio**: Enables testing of asyncio Python code with pytest, making it easier to test asynchronous functions and classes. [License](https://github.com/pytest-dev/pytest-asyncio/blob/main/LICENSE), [PyPI](https://pypi.org/project/pytest-asyncio/).
+- **pytest-cov**: A pytest plugin that produces test coverage reports, showing how well the tests cover the code. [License](https://github.com/pytest-dev/pytest-cov/blob/master/LICENSE), [PyPI](https://pypi.org/project/pytest-cov/).
+- **pytest-mock**: Enhances pytest with mock functionality for unit tests, providing a simpler interface to powerful mocking tools. [License](https://github.com/pytest-dev/pytest-mock/blob/main/LICENSE), [PyPI](https://pypi.org/project/pytest-mock/).
+
+### Additional Notes
 
-These tools help us maintain a clean and reliable codebase by catching potential issues early and documenting where our tests might be lacking.
+These tools are essential for maintaining high standards of code quality and ensuring that all functionality is robustly tested. For each package, the versions listed within the `test_requirements.txt` are those currently in use; updates may be applied as newer versions are released.
 
 ---
 _This README.md file has been carefully crafted and edited using the Notolog editor itself._
```

### Comparing `notolog-0.9.1b7/notolog.egg-info/SOURCES.txt` & `notolog-0.9.1b8/notolog.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 CHANGELOG.md
 CODE_OF_CONDUCT.md
 LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
+test_requirements.txt
 docs/Examples.md
 docs/notolog-ui-settings-strawberry-ja.png
 docs/notolog-ui-settings.png
 notolog/__init__.py
 notolog/app_config.py
 notolog/async_highlighter.py
 notolog/edit_widget.py
@@ -300,18 +301,21 @@
 notolog/ui/toolbar.py
 notolog/ui/vertical_line_spacer.py
 tests/__init__.py
 tests/test_enc_helper.py
 tests/test_enc_password.py
 tests/test_file_header.py
 tests/test_html_view.py
+tests/test_image_downloader.py
 tests/test_lexemes.py
 tests/test_notolog_editor.py
 tests/test_pkg_integration.py
 tests/test_qt_async.py
 tests/test_settings.py
+tests/test_settings_helper.py
 tests/test_text_block_data.py
 tests/test_theme_helper.py
 tests/test_themes.py
 tests/ui_tests/__init__.py
 tests/ui_tests/test_ai_assistant.py
-tests/ui_tests/test_qt_ui.py
+tests/ui_tests/test_qt_ui.py
+tests/ui_tests/test_settings_dialog.py
```

### Comparing `notolog-0.9.1b7/tests/test_enc_helper.py` & `notolog-0.9.1b8/tests/test_enc_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # tests/test_enc_helper.py
+
 from notolog.encrypt.enc_helper import EncHelper
 from notolog.encrypt.enc_password import EncPassword
 
 from cryptography.fernet import Fernet
 
 from logging import Logger
```

### Comparing `notolog-0.9.1b7/tests/test_enc_password.py` & `notolog-0.9.1b8/tests/test_enc_password.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # tests/test_enc_password.py
+
 from notolog.encrypt.enc_password import EncPassword
 
 import pytest
 
 
 class TestEncPassword:
 
@@ -59,9 +60,9 @@
             (('>pass>', 'some-hint-here'), False),
             (('01234567', None), True),
             (('some>pass>here', None), True),
             (('some>pass>here', 'some-hint-here'), True),
         ],
         indirect=True
     )
-    def test_enc_password_is_valid(self, test_obj_enc_password, test_exp_is_valid_fixture):
-        assert test_obj_enc_password.is_valid() == test_exp_is_valid_fixture
+    def test_enc_password_is_valid(self, test_obj_enc_password: EncPassword, test_exp_is_valid_fixture):
+        assert test_obj_enc_password.is_valid() == test_exp_is_valid_fixture
```

### Comparing `notolog-0.9.1b7/tests/test_file_header.py` & `notolog-0.9.1b8/tests/test_file_header.py`

 * *Files 10% similar despite different names*

```diff
@@ -105,38 +105,50 @@
 
         yield param_value
 
     @pytest.mark.parametrize(
         "test_obj_file_header_load, test_exp_fixture",
         [
             (
-                '<!-- {"notolog.app": {"created": "2024-02-08 22:10:13.277826", "updated": "2024-02-08 22:10:13.277837"}} -->',
-                '<!-- {"notolog.app": {"created": "2024-02-08 22:10:13.277826", "updated": "2024-02-08 22:10:13.277837"}} -->'
+                '<!-- {"notolog.app": {"created": "2024-02-08 22:10:13.277826",'
+                ' "updated": "2024-02-08 22:10:13.277837"}} -->',
+                '<!-- {"notolog.app": {"created": "2024-02-08 22:10:13.277826",'
+                ' "updated": "2024-02-08 22:10:13.277837"}} -->'
             ),
             (
-                    # New line but nothing else
-                    '<!-- {"notolog.app": {"created": "2024-02-08 22:10:13.277826", "updated": "2024-02-08 22:10:13.277837"}} -->\n',
-                    '<!-- {"notolog.app": {"created": "2024-02-08 22:10:13.277826", "updated": "2024-02-08 22:10:13.277837"}} -->'
+                # New line but nothing else
+                '<!-- {"notolog.app": {"created": "2024-02-08 22:10:13.277826",'
+                ' "updated": "2024-02-08 22:10:13.277837"}} -->\n',
+                '<!-- {"notolog.app": {"created": "2024-02-08 22:10:13.277826",'
+                ' "updated": "2024-02-08 22:10:13.277837"}} -->'
             ),
             (
-                    # New line with return
-                    '<!-- {"notolog.app": {"created": "2024-02-08 22:10:13.277826", "updated": "2024-02-08 22:10:13.277837"}} -->\n\r',
-                    '<!-- {"notolog.app": {"created": "2024-02-08 22:10:13.277826", "updated": "2024-02-08 22:10:13.277837"}} -->\n'
+                # New line with return
+                '<!-- {"notolog.app": {"created": "2024-02-08 22:10:13.277826",'
+                ' "updated": "2024-02-08 22:10:13.277837"}} -->\n\r',
+                '<!-- {"notolog.app": {"created": "2024-02-08 22:10:13.277826",'
+                ' "updated": "2024-02-08 22:10:13.277837"}} -->\n'
             ),
             (
-                '<!-- {"notolog.app": {"created": "2024-02-08 22:10:13.277826", "updated": "2024-02-08 22:10:13.277837"}} -->\ntest content',
-                '<!-- {"notolog.app": {"created": "2024-02-08 22:10:13.277826", "updated": "2024-02-08 22:10:13.277837"}} -->\ntest content'
+                '<!-- {"notolog.app": {"created": "2024-02-08 22:10:13.277826",'
+                ' "updated": "2024-02-08 22:10:13.277837"}} -->\ntest content',
+                '<!-- {"notolog.app": {"created": "2024-02-08 22:10:13.277826",'
+                ' "updated": "2024-02-08 22:10:13.277837"}} -->\ntest content'
             ),
             (
-                '<!-- {"notolog.app": {"created": "2024-02-08 22:10:13.277826", "updated": "2024-02-08 22:10:13.277837", "slt": "qwerty789ABC"}} -->',
-                '<!-- {"notolog.app": {"created": "2024-02-08 22:10:13.277826", "updated": "2024-02-08 22:10:13.277837", "slt": "qwerty789ABC"}} -->'
+                '<!-- {"notolog.app": {"created": "2024-02-08 22:10:13.277826",'
+                ' "updated": "2024-02-08 22:10:13.277837", "slt": "qwerty789ABC"}} -->',
+                '<!-- {"notolog.app": {"created": "2024-02-08 22:10:13.277826",'
+                ' "updated": "2024-02-08 22:10:13.277837", "slt": "qwerty789ABC"}} -->'
             ),
             (
-                '<!-- {"notolog.app": {"created": "2024-02-08 22:10:13.277826", "updated": "2024-02-08 22:10:13.277837", "smth123": "!!!"}} -->',
-                '<!-- {"notolog.app": {"created": "2024-02-08 22:10:13.277826", "updated": "2024-02-08 22:10:13.277837", "smth123": "!!!"}} -->'
+                '<!-- {"notolog.app": {"created": "2024-02-08 22:10:13.277826",'
+                ' "updated": "2024-02-08 22:10:13.277837", "smth123": "!!!"}} -->',
+                '<!-- {"notolog.app": {"created": "2024-02-08 22:10:13.277826",'
+                ' "updated": "2024-02-08 22:10:13.277837", "smth123": "!!!"}} -->'
             ),
         ],
         indirect=True
     )
     def test_file_header_loaded(self, test_obj_file_header_load, test_exp_fixture):
         _file_header, _file_content = test_obj_file_header_load
 
@@ -212,25 +224,28 @@
         except Exception:
             pytest.fail("The method raised an unexpected exception")
 
     @pytest.mark.parametrize(
         "test_obj_file_header_load, test_exp_fixture",
         [
             (
-                    '<!-- {"notolog.app": {"created": "2024-02-08 22:10:13.277826", "updated": "2024-02-08 22:10:13.277837"}} -->',
-                    False
+                '<!-- {"notolog.app": {"created": "2024-02-08 22:10:13.277826",'
+                ' "updated": "2024-02-08 22:10:13.277837"}} -->',
+                False
             ),
             (
-                    '<!-- {"notolog.app": {"created": "2024-02-08 22:10:13.277826", "updated": "2024-02-08 22:10:13.277837", "slt": "qwerty789ABC"}} -->',
-                    False
+                '<!-- {"notolog.app": {"created": "2024-02-08 22:10:13.277826",'
+                ' "updated": "2024-02-08 22:10:13.277837", "slt": "qwerty789ABC"}} -->',
+                False
             ),
             (
-                    '<!-- {"notolog.app": {"created": "2024-02-08 22:10:13.277826", "updated": "2024-02-08 22:10:13.277837",'
-                    '"enc": {"slt": "qwerty789ABC", "itr": "123456", "hint": "..."}}} -->',
-                    True
+                '<!-- {"notolog.app": {"created": "2024-02-08 22:10:13.277826",'
+                ' "updated": "2024-02-08 22:10:13.277837",'
+                '"enc": {"slt": "qwerty789ABC", "itr": "123456", "hint": "..."}}} -->',
+                True
             ),
         ],
         indirect=True
     )
     def test_file_header_is_file_encrypted(self, test_obj_file_header_load, test_exp_fixture):
         _file_header, _file_content = test_obj_file_header_load
```

### Comparing `notolog-0.9.1b7/tests/test_html_view.py` & `notolog-0.9.1b8/tests/test_html_view.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # tests/test_html_view.py
+
 from PySide6.QtGui import QTextDocument, QFont
 
 from notolog.highlight.view_highlighter import ViewHighlighter
 from notolog.view_processor import ViewProcessor
 from notolog.view_decorator import ViewDecorator
 
 import pytest
@@ -60,15 +61,15 @@
     @pytest.mark.parametrize(
         "test_obj_doc, test_text_fixture, test_style_fixture",
         [
             (("<b>Test text bold</b>", "setHtml"), "text", "bold"),
             (("<i>Test text italic</i>", "setHtml"), "text", "italic"),
             (("<u>Test text underline</u>", "setHtml"), "text", "underline"),
             (("<s>Test text strikethrough</s>", "setHtml"), "text", "strikeOut"),
-            #(("~~Test text strikethrough~~", "setHtml"), "text", "strikeOut"), # TODO decorator result
+            # (("~~Test text strikethrough~~", "setHtml"), "text", "strikeOut"),  # TODO decorator result
             # Markdown is a proof of concept here as it is not in use for result rendering
             (("**Test text bold**", "setMarkdown"), "text", "bold"),
             (("*Test text bold*", "setMarkdown"), "text", "italic"),
             (("***Test text bold***", "setMarkdown"), "text", "bold"),
             (("***Test text bold***", "setMarkdown"), "text", "italic"),
             (("~~Test text strikethrough~~", "setMarkdown"), "text", "strikeOut"),
         ],
@@ -84,24 +85,24 @@
         """
 
         """
         * https://doc.qt.io/qt-6/qtextdocument.html#find-1
         """
         cursor = test_obj_doc.find(test_text_fixture)
 
-        format = cursor.charFormat()
+        _format = cursor.charFormat()
         assert cursor.selectedText()
         """
         test_style_fixture is a method name
         * https://doc.qt.io/qt-6/qfont.html#bold
         * https://doc.qt.io/qt-6/qfont.html#italic
         * https://doc.qt.io/qt-6/qfont.html#strikeOut
         * ...
         """
-        assert callable(getattr(format.font(), test_style_fixture))
-        assert getattr(format.font(), test_style_fixture)()
+        assert callable(getattr(_format.font(), test_style_fixture))
+        assert getattr(_format.font(), test_style_fixture)()
 
         """
         Assertion like ',-1,-1,5,700,0,0,0,0,0,0,0,0,0,0,1'
         * https://doc.qt.io/qt-6/qfont.html#toString
         """
-        #assert not format.font().toString() == '...'
+        # assert not format.font().toString() == '...'
```

### Comparing `notolog-0.9.1b7/tests/test_notolog_editor.py` & `notolog-0.9.1b8/tests/test_notolog_editor.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,15 @@
         mode, file_path, isfile, content, res_path_call_cnt = test_exp_params_fixture
 
         mocker.patch.object(test_obj_notolog_editor, 'get_mode', return_value=mode)
         mocker.patch.object(test_obj_notolog_editor, 'toggle_mode', return_value=None)
         setattr(test_obj_notolog_editor, 'debug', False)
 
         mock_res_path = mocker.patch.object(test_obj_notolog_editor, 'get_active_dir', return_value=file_path)
-        #mock_res_path = mocker.patch('app.notolog_editor.res_path', return_value=file_path)
+        # mock_res_path = mocker.patch('app.notolog_editor.res_path', return_value=file_path)
         # fixture arg: monkeypatch
         # monkeypatch.setattr('app.notolog_editor.res_path', lambda _file_path: _file_path == file_path)
         mocker.patch.object(os.path, 'isfile', return_value=isfile)
 
         mock_save_file_content = mocker.patch.object(test_obj_notolog_editor, 'save_file_content', return_value=None)
         mocker.patch.object(test_obj_notolog_editor, 'load_file', return_value=None)
```

### Comparing `notolog-0.9.1b7/tests/test_pkg_integration.py` & `notolog-0.9.1b8/tests/test_pkg_integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # tests/test_pkg_integration.py
+
 import pytest
 
 import emoji
 import markdown
 
 
 @pytest.fixture
```

### Comparing `notolog-0.9.1b7/tests/test_qt_async.py` & `notolog-0.9.1b8/tests/test_qt_async.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,24 @@
+# tests/test_qt_async.py
+
 import asyncio
 
 from notolog.async_highlighter import AsyncHighlighter
 
 import pytest
 
 
 class TestQtAsync:
 
     @pytest.fixture
     def async_highlighter_obj(self):
-        # Fixture to create and return main window instance
+        # To avoid: There is no current event loop when self.loop = asyncio.get_event_loop()
+        loop = asyncio.new_event_loop()
+        asyncio.set_event_loop(loop)
+        # Fixture to create and return object instance
         async_highlighter = AsyncHighlighter(callback=lambda check: check)
         yield async_highlighter
 
     @pytest.fixture
     async def cleanup_tasks(self):
         yield
         # Cancel and clean up all pending asyncio tasks
```

### Comparing `notolog-0.9.1b7/tests/test_settings.py` & `notolog-0.9.1b8/tests/test_settings.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # tests/test_settings.py
 
 from notolog.settings import Settings
+from notolog.app_config import AppConfig
 
-from . import test_app
+from . import test_core_app  # noqa: F401
 
 import os
 import pytest
 
 
 class TestSettings:
 
     @pytest.fixture(scope="function")
-    def test_obj_settings(self, test_app):
+    def test_obj_settings(self, test_core_app):  # noqa: F811 redefinition of unused 'test_app'
+        # The test_app fixture sets up the app environment explicitly.
         settings = Settings()
         settings.clear()
         yield settings
 
     def test_settings_defaults(self, test_obj_settings):
         assert test_obj_settings.ui_width == 0
         assert test_obj_settings.ui_height == 0
@@ -49,12 +51,12 @@
         assert settings.ui_pos_y == 44
         assert settings.file_path == os.path.normpath('test/path/file.txt')
         assert settings.toolbar_icons == 8
 
         # Linux: /home/runner/.config/Notolog/notolog_editor_tests.conf
         # macOS: '/Users/runner/Library/Preferences/com.notolog.notolog_editor_tests.plist'
         # Windows: '\\HKEY_CURRENT_USER\\Software\\Notolog\\notolog_editor_tests'
-        assert 'notolog_editor_tests' in settings.fileName()
+        assert AppConfig().get_settings_app_name_qa() in settings.fileName()
         assert test_obj_settings.fileName() == settings.fileName()
 
         # Reset to restore
         settings.clear()
```

### Comparing `notolog-0.9.1b7/tests/test_text_block_data.py` & `notolog-0.9.1b8/tests/test_text_block_data.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/tests/test_theme_helper.py` & `notolog-0.9.1b8/tests/test_theme_helper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,27 @@
-# tests/test_themes.py
+# tests/test_theme_helper.py
 
 from notolog.helpers.theme_helper import ThemeHelper
 from notolog.theme import Theme
 from notolog.settings import Settings
 from notolog.app_config import AppConfig
 
 from logging import Logger
 
+from . import test_core_app  # noqa: F401
+
 import os
 import pytest
 
 
 class TestThemeHelper:
 
     @pytest.fixture(autouse=True)
-    def test_settings_fixture(self, request):
+    def test_settings_fixture(self, request, test_core_app):  # noqa: F811 redefinition of unused 'test_app'
+        # The test_app fixture sets up the app environment explicitly.
         setting = Settings()
         # Get the parameter value(s) from the request
         setting.app_theme = request.param
         yield setting
 
     @pytest.fixture(autouse=True)
     def test_obj_theme_helper(self, mocker, test_settings_fixture):
@@ -54,21 +57,22 @@
         yield param_values
 
     @pytest.mark.parametrize(
         "test_settings_fixture, test_obj_theme_helper, test_exp_params_fixture",
         [
             ((None), (None), ('default')),
             ((''), (None), ('default')),
-            (('default'), (None), ('default')),  # Because of method default()
+            (('default'), (None), ('default')),  # Because of default() method
             (('DEFAULT'), (None), ('default')),
             (('anyval'), (None), ('default')),
         ],
         indirect=True
     )
-    def test_theme_helper_init(self,test_settings_fixture,  test_obj_theme_helper, test_exp_params_fixture):
+    def test_theme_helper_init(self, test_settings_fixture, test_obj_theme_helper: ThemeHelper,
+                               test_exp_params_fixture):
         """
         Test and check initial params are exist in the testing object.
         """
         assert isinstance(test_obj_theme_helper.logger, Logger)
 
         exp_theme = test_exp_params_fixture
 
@@ -113,8 +117,8 @@
     )
     def test_themes_get_css(self, test_settings_fixture, test_obj_theme_helper, test_exp_params_fixture):
         """
         Test getter for correctly loaded and really existent theme's css files.
         """
         param_css_name, exp_result = test_exp_params_fixture
 
-        assert test_obj_theme_helper.get_css(param_css_name) == exp_result
+        assert test_obj_theme_helper.get_css(param_css_name) == exp_result
```

### Comparing `notolog-0.9.1b7/tests/test_themes.py` & `notolog-0.9.1b8/tests/test_themes.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b7/tests/ui_tests/test_ai_assistant.py` & `notolog-0.9.1b8/tests/ui_tests/test_ai_assistant.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-# tests/ui/test_ai_assistant.py
+# tests/ui_tests/test_ai_assistant.py
 
 from PySide6.QtCore import Qt
 from PySide6.QtTest import QTest
 
 from notolog.ui.ai_assistant import AIAssistant
 from notolog.notolog_editor import NotologEditor
 from notolog.settings import Settings
 from notolog.enums.languages import Languages
 
-from . import test_app
+from . import test_app  # noqa: F401
 
 import pytest
 
 
 class TestAiAssistant:
 
     @pytest.fixture
     def settings_obj(self):
         # Fixture to create and return settings instance
         settings = Settings()
         yield settings
 
     @pytest.fixture
-    def main_window(self, mocker, test_app):
+    def main_window(self, mocker, test_app):  # noqa: F811 redefinition of unused 'test_app'
         # Force to override system language as a default
         mocker.patch.object(Languages, 'default', return_value='la')
 
         # Do not show actual window; return object instance only
         mocker.patch.object(NotologEditor, 'show', return_value=None)
 
         # Fixture to create and return main window instance
@@ -35,15 +35,15 @@
 
     @pytest.fixture(autouse=True)
     def ui_obj(self, main_window):
         # Fixture to initialize object.
         ui_obj = AIAssistant(parent=main_window)
         yield ui_obj
 
-    def test_ui_object_state(self, mocker, ui_obj, settings_obj):
+    def test_ui_object_state(self, mocker, ui_obj: AIAssistant, settings_obj):
         # Check app language set correctly
         assert settings_obj.app_language == 'la'
         # Check default AI model
         assert ui_obj.inference_model == 'gpt-3.5-turbo'
 
         # Check default window title
         assert ui_obj.windowTitle() == "Postulatio ad AI"
```

### Comparing `notolog-0.9.1b7/tests/ui_tests/test_qt_ui.py` & `notolog-0.9.1b8/tests/ui_tests/test_qt_ui.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-# tests/ui/test_qt_ui.py
+# tests/ui_tests/test_qt_ui.py
 
 from PySide6.QtCore import Qt
 from PySide6.QtTest import QTest
 
 from notolog.notolog_editor import NotologEditor
 from notolog.settings import Settings
 from notolog.enums.languages import Languages
 
-from . import test_app
+from . import test_app  # noqa: F401
 
 import pytest
 
 
 class TestQtUi:
 
     @pytest.fixture
     def settings_obj(self):
         # Fixture to create and return settings instance
         settings = Settings()
         yield settings
 
     @pytest.fixture
-    def main_window(self, mocker, test_app):
+    def main_window(self, mocker, test_app):  # noqa: F811 redefinition of unused 'test_app'
         # Force to override system language as a default
         mocker.patch.object(Languages, 'default', return_value='la')
 
         # Do not show actual window; return object instance only
         mocker.patch.object(NotologEditor, 'show', return_value=None)
 
         # Fixture to create and return main window instance
```

