# Comparing `tmp/odfdo-3.7.8.tar.gz` & `tmp/odfdo-3.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odfdo-3.7.8.tar", max compression
+gzip compressed data, was "odfdo-3.7.9.tar", max compression
```

## Comparing `odfdo-3.7.8.tar` & `odfdo-3.7.9.tar`

### file list

```diff
@@ -1,66 +1,72 @@
--rw-r--r--   0        0        0    11357 2022-08-19 23:34:42.000000 odfdo-3.7.8/LICENSE
--rw-r--r--   0        0        0      433 2022-08-19 23:34:42.000000 odfdo-3.7.8/NOTICE.txt
--rw-r--r--   0        0        0     3308 2024-04-01 16:01:23.803500 odfdo-3.7.8/README.md
--rw-r--r--   0        0        0     5220 2024-05-02 07:44:54.443931 odfdo-3.7.8/odfdo/__init__.py
--rw-r--r--   0        0        0     2361 2024-04-01 10:08:15.948752 odfdo-3.7.8/odfdo/bookmark.py
--rw-r--r--   0        0        0    13076 2024-04-01 10:08:15.949530 odfdo-3.7.8/odfdo/cell.py
--rw-r--r--   0        0        0    24252 2024-05-02 07:44:54.444099 odfdo-3.7.8/odfdo/const.py
--rw-r--r--   0        0        0    18030 2024-05-02 07:44:54.444263 odfdo-3.7.8/odfdo/container.py
--rw-r--r--   0        0        0     3243 2024-05-02 07:44:54.444402 odfdo-3.7.8/odfdo/content.py
--rw-r--r--   0        0        0     6668 2024-04-01 10:08:15.952639 odfdo-3.7.8/odfdo/datatype.py
--rw-r--r--   0        0        0    42015 2024-05-02 07:44:54.444601 odfdo-3.7.8/odfdo/document.py
--rw-r--r--   0        0        0     4192 2024-04-01 10:08:15.953626 odfdo-3.7.8/odfdo/draw_page.py
--rw-r--r--   0        0        0   104963 2024-05-02 07:44:54.444908 odfdo-3.7.8/odfdo/element.py
--rw-r--r--   0        0        0     8034 2024-05-02 07:44:54.445090 odfdo-3.7.8/odfdo/element_typed.py
--rw-r--r--   0        0        0    15586 2024-04-01 10:08:15.956248 odfdo-3.7.8/odfdo/frame.py
--rw-r--r--   0        0        0     3665 2024-04-01 10:08:15.956563 odfdo-3.7.8/odfdo/header.py
--rw-r--r--   0        0        0     1270 2024-04-01 10:08:15.957382 odfdo-3.7.8/odfdo/header_rows.py
--rw-r--r--   0        0        0     3524 2024-04-01 10:08:15.957701 odfdo-3.7.8/odfdo/image.py
--rw-r--r--   0        0        0     3206 2024-04-01 10:08:15.957997 odfdo-3.7.8/odfdo/link.py
--rw-r--r--   0        0        0     7129 2024-04-01 10:08:15.958225 odfdo-3.7.8/odfdo/list.py
--rw-r--r--   0        0        0     3812 2024-04-01 10:08:15.958534 odfdo-3.7.8/odfdo/manifest.py
--rw-r--r--   0        0        0    19538 2024-05-02 07:44:54.445255 odfdo-3.7.8/odfdo/meta.py
--rw-r--r--   0        0        0    11191 2024-04-01 10:08:15.958954 odfdo-3.7.8/odfdo/note.py
--rw-r--r--   0        0        0    28204 2024-04-01 10:08:15.959276 odfdo-3.7.8/odfdo/paragraph.py
--rw-r--r--   0        0        0     9443 2024-04-01 10:08:15.960044 odfdo-3.7.8/odfdo/paragraph_base.py
--rw-r--r--   0        0        0    14661 2024-04-01 10:08:15.960585 odfdo-3.7.8/odfdo/reference.py
--rw-r--r--   0        0        0    25859 2024-04-01 10:08:15.961041 odfdo-3.7.8/odfdo/row.py
--rw-r--r--   0        0        0        1 2024-04-01 10:08:15.961512 odfdo-3.7.8/odfdo/scripts/__init__.py
--rwxr-xr-x   0        0        0     3280 2024-04-01 10:08:15.962026 odfdo-3.7.8/odfdo/scripts/diff.py
--rwxr-xr-x   0        0        0     2178 2024-05-02 07:44:54.445397 odfdo-3.7.8/odfdo/scripts/folder.py
--rwxr-xr-x   0        0        0     3803 2024-04-01 10:08:15.963301 odfdo-3.7.8/odfdo/scripts/headers.py
--rwxr-xr-x   0        0        0     5832 2024-04-01 10:08:15.963611 odfdo-3.7.8/odfdo/scripts/highlight.py
--rwxr-xr-x   0        0        0     3603 2024-04-01 10:08:15.963998 odfdo-3.7.8/odfdo/scripts/replace.py
--rwxr-xr-x   0        0        0     5752 2024-04-01 10:08:15.964706 odfdo-3.7.8/odfdo/scripts/show.py
--rwxr-xr-x   0        0        0     7576 2024-04-01 10:08:15.965411 odfdo-3.7.8/odfdo/scripts/styles.py
--rwxr-xr-x   0        0        0     3442 2024-04-01 10:08:15.966077 odfdo-3.7.8/odfdo/scripts/table_shrink.py
--rw-r--r--   0        0        0     1936 2024-04-01 10:08:15.967048 odfdo-3.7.8/odfdo/scriptutils.py
--rw-r--r--   0        0        0     1939 2024-04-01 10:08:15.967336 odfdo-3.7.8/odfdo/section.py
--rw-r--r--   0        0        0    11548 2024-04-01 10:08:15.967836 odfdo-3.7.8/odfdo/shapes.py
--rw-r--r--   0        0        0     4691 2024-04-01 10:08:15.968192 odfdo-3.7.8/odfdo/smil.py
--rw-r--r--   0        0        0    38072 2024-05-02 07:44:54.445588 odfdo-3.7.8/odfdo/style.py
--rw-r--r--   0        0        0     5244 2024-04-01 10:08:15.969088 odfdo-3.7.8/odfdo/styles.py
--rw-r--r--   0        0        0   104460 2024-05-02 07:44:54.445878 odfdo-3.7.8/odfdo/table.py
--rw-r--r--   0        0        0        1 2024-04-01 10:08:15.970133 odfdo-3.7.8/odfdo/templates/__init__.py
--rw-r--r--   0        0        0     8291 2024-04-01 10:08:15.970835 odfdo-3.7.8/odfdo/templates/drawing.otg
--rw-r--r--   0        0        0    11017 2024-04-01 10:08:15.971235 odfdo-3.7.8/odfdo/templates/lpod_styles.odt
--rw-r--r--   0        0        0    16065 2024-04-01 10:08:15.971582 odfdo-3.7.8/odfdo/templates/presentation.otp
--rw-r--r--   0        0        0     7432 2024-04-01 10:08:15.972020 odfdo-3.7.8/odfdo/templates/spreadsheet.ots
--rw-r--r--   0        0        0     9620 2024-04-01 10:08:15.972500 odfdo-3.7.8/odfdo/templates/text.ott
--rw-r--r--   0        0        0    17070 2024-04-01 10:08:15.973345 odfdo-3.7.8/odfdo/toc.py
--rw-r--r--   0        0        0    24638 2024-04-01 10:08:15.973733 odfdo-3.7.8/odfdo/tracked_changes.py
--rw-r--r--   0        0        0     1318 2024-04-01 10:08:15.973907 odfdo-3.7.8/odfdo/utils/__init__.py
--rw-r--r--   0        0        0     9339 2024-04-01 10:08:15.974689 odfdo-3.7.8/odfdo/utils/cache_map.py
--rw-r--r--   0        0        0      926 2024-04-01 10:08:15.975005 odfdo-3.7.8/odfdo/utils/cached_element.py
--rw-r--r--   0        0        0     3035 2024-04-01 10:08:15.975436 odfdo-3.7.8/odfdo/utils/color.py
--rw-r--r--   0        0        0     4533 2024-04-01 10:08:15.975823 odfdo-3.7.8/odfdo/utils/coordinates.py
--rw-r--r--   0        0        0     1476 2024-04-01 10:08:15.976142 odfdo-3.7.8/odfdo/utils/formula.py
--rw-r--r--   0        0        0     1314 2024-04-01 10:08:15.976364 odfdo-3.7.8/odfdo/utils/isiterable.py
--rw-r--r--   0        0        0     1429 2024-04-01 10:08:15.976629 odfdo-3.7.8/odfdo/utils/str_convert.py
--rw-r--r--   0        0        0     2503 2024-04-01 10:08:15.976906 odfdo-3.7.8/odfdo/utils/style_constants.py
--rw-r--r--   0        0        0     4272 2024-04-01 10:08:15.977335 odfdo-3.7.8/odfdo/utils/xpath_query.py
--rw-r--r--   0        0        0    14844 2024-05-02 07:44:54.446064 odfdo-3.7.8/odfdo/variable.py
--rw-r--r--   0        0        0     1165 2024-04-01 10:08:15.977698 odfdo-3.7.8/odfdo/version.py
--rw-r--r--   0        0        0     3899 2024-05-02 07:44:54.446210 odfdo-3.7.8/odfdo/xmlpart.py
--rw-r--r--   0        0        0     3844 2024-05-02 07:44:54.446935 odfdo-3.7.8/pyproject.toml
--rw-r--r--   0        0        0     4694 1970-01-01 00:00:00.000000 odfdo-3.7.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-08-19 23:34:42.000000 odfdo-3.7.9/LICENSE
+-rw-r--r--   0        0        0      433 2022-08-19 23:34:42.000000 odfdo-3.7.9/NOTICE.txt
+-rw-r--r--   0        0        0     3308 2024-04-01 16:01:23.803500 odfdo-3.7.9/README.md
+-rw-r--r--   0        0        0     5661 2024-05-03 12:29:07.610437 odfdo-3.7.9/odfdo/__init__.py
+-rw-r--r--   0        0        0     4204 2024-05-03 12:29:07.610578 odfdo-3.7.9/odfdo/body.py
+-rw-r--r--   0        0        0     2361 2024-04-01 10:08:15.948752 odfdo-3.7.9/odfdo/bookmark.py
+-rw-r--r--   0        0        0    13076 2024-04-01 10:08:15.949530 odfdo-3.7.9/odfdo/cell.py
+-rw-r--r--   0        0        0    24252 2024-05-02 07:44:54.444099 odfdo-3.7.9/odfdo/const.py
+-rw-r--r--   0        0        0    18030 2024-05-02 07:44:54.444263 odfdo-3.7.9/odfdo/container.py
+-rw-r--r--   0        0        0     3243 2024-05-02 07:44:54.444402 odfdo-3.7.9/odfdo/content.py
+-rw-r--r--   0        0        0     6668 2024-04-01 10:08:15.952639 odfdo-3.7.9/odfdo/datatype.py
+-rw-r--r--   0        0        0    41978 2024-05-03 12:29:07.610849 odfdo-3.7.9/odfdo/document.py
+-rw-r--r--   0        0        0     4192 2024-04-01 10:08:15.953626 odfdo-3.7.9/odfdo/draw_page.py
+-rw-r--r--   0        0        0   102419 2024-05-03 12:29:07.611240 odfdo-3.7.9/odfdo/element.py
+-rw-r--r--   0        0        0     8034 2024-05-02 07:44:54.445090 odfdo-3.7.9/odfdo/element_typed.py
+-rw-r--r--   0        0        0    15586 2024-04-01 10:08:15.956248 odfdo-3.7.9/odfdo/frame.py
+-rw-r--r--   0        0        0     3665 2024-04-01 10:08:15.956563 odfdo-3.7.9/odfdo/header.py
+-rw-r--r--   0        0        0     1270 2024-04-01 10:08:15.957382 odfdo-3.7.9/odfdo/header_rows.py
+-rw-r--r--   0        0        0     3524 2024-04-01 10:08:15.957701 odfdo-3.7.9/odfdo/image.py
+-rw-r--r--   0        0        0     3206 2024-04-01 10:08:15.957997 odfdo-3.7.9/odfdo/link.py
+-rw-r--r--   0        0        0     7129 2024-04-01 10:08:15.958225 odfdo-3.7.9/odfdo/list.py
+-rw-r--r--   0        0        0     3814 2024-05-03 12:29:07.611425 odfdo-3.7.9/odfdo/manifest.py
+-rw-r--r--   0        0        0    28768 2024-05-03 12:29:07.611659 odfdo-3.7.9/odfdo/meta.py
+-rw-r--r--   0        0        0     2407 2024-05-03 12:29:07.611825 odfdo-3.7.9/odfdo/meta_auto_reload.py
+-rw-r--r--   0        0        0     2109 2024-05-03 12:29:07.611962 odfdo-3.7.9/odfdo/meta_hyperlink_behaviour.py
+-rw-r--r--   0        0        0     2433 2024-05-03 12:29:07.612099 odfdo-3.7.9/odfdo/meta_template.py
+-rw-r--r--   0        0        0     2563 2024-05-03 12:29:07.612219 odfdo-3.7.9/odfdo/mixin_dc_creator.py
+-rw-r--r--   0        0        0     2718 2024-05-03 12:29:07.612335 odfdo-3.7.9/odfdo/mixin_dc_date.py
+-rw-r--r--   0        0        0    11754 2024-05-03 12:29:07.612573 odfdo-3.7.9/odfdo/note.py
+-rw-r--r--   0        0        0    28198 2024-05-03 12:29:07.612762 odfdo-3.7.9/odfdo/paragraph.py
+-rw-r--r--   0        0        0     9446 2024-05-03 12:29:07.612987 odfdo-3.7.9/odfdo/paragraph_base.py
+-rw-r--r--   0        0        0    14661 2024-04-01 10:08:15.960585 odfdo-3.7.9/odfdo/reference.py
+-rw-r--r--   0        0        0    25859 2024-04-01 10:08:15.961041 odfdo-3.7.9/odfdo/row.py
+-rw-r--r--   0        0        0        1 2024-04-01 10:08:15.961512 odfdo-3.7.9/odfdo/scripts/__init__.py
+-rwxr-xr-x   0        0        0     3280 2024-04-01 10:08:15.962026 odfdo-3.7.9/odfdo/scripts/diff.py
+-rwxr-xr-x   0        0        0     2178 2024-05-02 07:44:54.445397 odfdo-3.7.9/odfdo/scripts/folder.py
+-rwxr-xr-x   0        0        0     3803 2024-04-01 10:08:15.963301 odfdo-3.7.9/odfdo/scripts/headers.py
+-rwxr-xr-x   0        0        0     5832 2024-04-01 10:08:15.963611 odfdo-3.7.9/odfdo/scripts/highlight.py
+-rwxr-xr-x   0        0        0     3603 2024-04-01 10:08:15.963998 odfdo-3.7.9/odfdo/scripts/replace.py
+-rwxr-xr-x   0        0        0     5752 2024-04-01 10:08:15.964706 odfdo-3.7.9/odfdo/scripts/show.py
+-rwxr-xr-x   0        0        0     7576 2024-04-01 10:08:15.965411 odfdo-3.7.9/odfdo/scripts/styles.py
+-rwxr-xr-x   0        0        0     3442 2024-04-01 10:08:15.966077 odfdo-3.7.9/odfdo/scripts/table_shrink.py
+-rw-r--r--   0        0        0     1936 2024-04-01 10:08:15.967048 odfdo-3.7.9/odfdo/scriptutils.py
+-rw-r--r--   0        0        0     1939 2024-04-01 10:08:15.967336 odfdo-3.7.9/odfdo/section.py
+-rw-r--r--   0        0        0    11548 2024-04-01 10:08:15.967836 odfdo-3.7.9/odfdo/shapes.py
+-rw-r--r--   0        0        0     4691 2024-04-01 10:08:15.968192 odfdo-3.7.9/odfdo/smil.py
+-rw-r--r--   0        0        0    38072 2024-05-02 07:44:54.445588 odfdo-3.7.9/odfdo/style.py
+-rw-r--r--   0        0        0     5244 2024-04-01 10:08:15.969088 odfdo-3.7.9/odfdo/styles.py
+-rw-r--r--   0        0        0   104460 2024-05-02 07:44:54.445878 odfdo-3.7.9/odfdo/table.py
+-rw-r--r--   0        0        0        1 2024-04-01 10:08:15.970133 odfdo-3.7.9/odfdo/templates/__init__.py
+-rw-r--r--   0        0        0     8291 2024-04-01 10:08:15.970835 odfdo-3.7.9/odfdo/templates/drawing.otg
+-rw-r--r--   0        0        0    11017 2024-04-01 10:08:15.971235 odfdo-3.7.9/odfdo/templates/lpod_styles.odt
+-rw-r--r--   0        0        0    16065 2024-04-01 10:08:15.971582 odfdo-3.7.9/odfdo/templates/presentation.otp
+-rw-r--r--   0        0        0     7432 2024-04-01 10:08:15.972020 odfdo-3.7.9/odfdo/templates/spreadsheet.ots
+-rw-r--r--   0        0        0     9620 2024-04-01 10:08:15.972500 odfdo-3.7.9/odfdo/templates/text.ott
+-rw-r--r--   0        0        0    17070 2024-04-01 10:08:15.973345 odfdo-3.7.9/odfdo/toc.py
+-rw-r--r--   0        0        0    23712 2024-05-03 12:29:07.613167 odfdo-3.7.9/odfdo/tracked_changes.py
+-rw-r--r--   0        0        0     1318 2024-04-01 10:08:15.973907 odfdo-3.7.9/odfdo/utils/__init__.py
+-rw-r--r--   0        0        0     9339 2024-04-01 10:08:15.974689 odfdo-3.7.9/odfdo/utils/cache_map.py
+-rw-r--r--   0        0        0      926 2024-04-01 10:08:15.975005 odfdo-3.7.9/odfdo/utils/cached_element.py
+-rw-r--r--   0        0        0     3035 2024-04-01 10:08:15.975436 odfdo-3.7.9/odfdo/utils/color.py
+-rw-r--r--   0        0        0     4533 2024-04-01 10:08:15.975823 odfdo-3.7.9/odfdo/utils/coordinates.py
+-rw-r--r--   0        0        0     1476 2024-04-01 10:08:15.976142 odfdo-3.7.9/odfdo/utils/formula.py
+-rw-r--r--   0        0        0     1314 2024-04-01 10:08:15.976364 odfdo-3.7.9/odfdo/utils/isiterable.py
+-rw-r--r--   0        0        0     1429 2024-04-01 10:08:15.976629 odfdo-3.7.9/odfdo/utils/str_convert.py
+-rw-r--r--   0        0        0     2503 2024-04-01 10:08:15.976906 odfdo-3.7.9/odfdo/utils/style_constants.py
+-rw-r--r--   0        0        0     4272 2024-04-01 10:08:15.977335 odfdo-3.7.9/odfdo/utils/xpath_query.py
+-rw-r--r--   0        0        0    14844 2024-05-02 07:44:54.446064 odfdo-3.7.9/odfdo/variable.py
+-rw-r--r--   0        0        0     1165 2024-04-01 10:08:15.977698 odfdo-3.7.9/odfdo/version.py
+-rw-r--r--   0        0        0     4320 2024-05-03 12:29:07.613351 odfdo-3.7.9/odfdo/xmlpart.py
+-rw-r--r--   0        0        0     3844 2024-05-03 12:29:07.614137 odfdo-3.7.9/pyproject.toml
+-rw-r--r--   0        0        0     4694 1970-01-01 00:00:00.000000 odfdo-3.7.9/PKG-INFO
```

### Comparing `odfdo-3.7.8/LICENSE` & `odfdo-3.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.8/README.md` & `odfdo-3.7.9/README.md`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.8/odfdo/__init__.py` & `odfdo-3.7.9/odfdo/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,69 +24,81 @@
 __all__ = [
     "AnimPar",
     "AnimSeq",
     "AnimTransFilter",
     "Annotation",
     "AnnotationEnd",
     "BackgroundImage",
+    "Body",
     "Bookmark",
     "BookmarkEnd",
     "BookmarkStart",
     "Cell",
     "ChangeInfo",
+    "Chart",
     "Column",
     "ConnectorShape",
     "Container",
     "Content",
     "Content",
+    "Database",
     "Document",
     "DrawFillImage",
     "DrawGroup",
     "DrawImage",
     "DrawPage",
+    "Drawing",
+    "EText",
     "Element",
     "ElementTyped",
     "EllipseShape",
     "FIRST_CHILD",
     "Frame",
     "Header",
     "HeaderRows",
+    "Image",
     "IndexTitle",
     "IndexTitleTemplate",
     "LAST_CHILD",
     "LineBreak",
     "LineShape",
     "Link",
     "List",
     "ListItem",
     "Manifest",
     "Meta",
+    "MetaAutoReload",
+    "MetaHyperlinkBehaviour",
+    "MetaTemplate",
     "NEXT_SIBLING",
     "NamedRange",
     "Note",
     "PREV_SIBLING",
     "PageBreak",
     "Paragraph",
+    "Presentation",
     "RectangleShape",
     "Reference",
     "ReferenceMark",
     "ReferenceMarkEnd",
     "ReferenceMarkStart",
     "Row",
     "RowGroup",
     "Section",
     "Spacer",
     "Span",
+    "Spreadsheet",
     "Style",
     "Styles",
     "TOC",
     "Tab",
     "TabStopStyle",
     "Table",
     "Text",
+    "Text",
     "TextChange",
     "TextChangeEnd",
     "TextChangeStart",
     "TextChangedRegion",
     "TextDeletion",
     "TextFormatChange",
     "TextInsertion",
@@ -128,30 +140,34 @@
     "hex2rgb",
     "hexa_color",
     "make_table_cell_border_string",
     "rgb2hex",
 ]
 
 
+from .body import Body, Chart, Database, Drawing, Image, Presentation, Spreadsheet, Text
 from .bookmark import Bookmark, BookmarkEnd, BookmarkStart
 from .cell import Cell
 from .container import Container
 from .content import Content
 from .document import Document
 from .draw_page import DrawPage
-from .element import FIRST_CHILD, LAST_CHILD, NEXT_SIBLING, PREV_SIBLING, Element, Text
+from .element import FIRST_CHILD, LAST_CHILD, NEXT_SIBLING, PREV_SIBLING, Element, EText
 from .element_typed import ElementTyped
 from .frame import Frame, default_frame_position_style
 from .header import Header
 from .header_rows import HeaderRows
 from .image import DrawFillImage, DrawImage
 from .link import Link
 from .list import List, ListItem
 from .manifest import Manifest
 from .meta import Meta
+from .meta_auto_reload import MetaAutoReload
+from .meta_hyperlink_behaviour import MetaHyperlinkBehaviour
+from .meta_template import MetaTemplate
 from .note import Annotation, AnnotationEnd, Note
 from .paragraph import LineBreak, PageBreak, Paragraph, Spacer, Span, Tab
 from .reference import Reference, ReferenceMark, ReferenceMarkEnd, ReferenceMarkStart
 from .section import Section
 from .shapes import ConnectorShape, DrawGroup, EllipseShape, LineShape, RectangleShape
 from .smil import AnimPar, AnimSeq, AnimTransFilter
 from .style import (
```

### Comparing `odfdo-3.7.8/odfdo/bookmark.py` & `odfdo-3.7.9/odfdo/bookmark.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.8/odfdo/cell.py` & `odfdo-3.7.9/odfdo/cell.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.8/odfdo/const.py` & `odfdo-3.7.9/odfdo/const.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.8/odfdo/container.py` & `odfdo-3.7.9/odfdo/container.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.8/odfdo/content.py` & `odfdo-3.7.9/odfdo/content.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.8/odfdo/datatype.py` & `odfdo-3.7.9/odfdo/datatype.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.8/odfdo/document.py` & `odfdo-3.7.9/odfdo/document.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,15 +167,15 @@
         - Document("presentation") -> an "empty" document of type presentation
         - Document("drawing") -> an "empty" document of type drawing
 
         Meaning of “empty”: these documents are copies of the default
         templates documents provided with this library, which, as templates,
         are not really empty. It may be useful to clear the newly created
         document: document.body.clear(), or adjust meta informations like
-        description or default language: document.meta.set_language('fr-FR')
+        description or default language: document.meta.language = 'fr-FR'
 
     If the argument is not a known template type, or is a Path,
     Document(file) will load the content of the ODF file.
 
     To explicitly create a document from a custom template, use the
     Document.new(path) method whose argument is the path to the template file.
     """
@@ -503,35 +503,36 @@
 
         # Simple values
         def print_info(name: str, value: Any) -> None:
             if value:
                 result.append(f"{name}: {value}")
 
         meta = self.meta
-        print_info("Title", meta.get_title())
-        print_info("Subject", meta.get_subject())
-        print_info("Language", meta.get_language())
-        print_info("Modification date", meta.get_modification_date())
-        print_info("Creation date", meta.get_creation_date())
-        print_info("Initial creator", meta.get_initial_creator())
-        print_info("Keyword", meta.get_keywords())
-        print_info("Editing duration", meta.get_editing_duration())
-        print_info("Editing cycles", meta.get_editing_cycles())
-        print_info("Generator", meta.get_generator())
+        print_info("Title", meta.title)
+        print_info("Subject", meta.subject)
+        print_info("Description", meta.description)
+        print_info("Language", meta.language)
+        print_info("Modification date", meta.date)
+        print_info("Creation date", meta.creation_date)
+        print_info("Initial creator", meta.initial_creator)
+        print_info("Keyword", meta.keyword)
+        print_info("Editing duration", meta.editing_duration)
+        print_info("Editing cycles", meta.editing_cycles)
+        print_info("Generator", meta.generator)
 
         # Statistic
         result.append("Statistic:")
-        statistic = meta.get_statistic()
+        statistic = meta.statistic
         if statistic:
             for name, data in statistic.items():
                 result.append(f"  - {name[5:].replace('-', ' ').capitalize()}: {data}")
 
         # User defined metadata
         result.append("User defined metadata:")
-        user_metadata = meta.get_user_defined_metadata()
+        user_metadata = meta.user_defined_metadata
         for name, data2 in user_metadata.items():
             result.append(f"  - {name}: {data2}")
 
         # And the description
         print_info("Description", meta.get_description())
 
         return "\n".join(result) + "\n"
```

### Comparing `odfdo-3.7.8/odfdo/draw_page.py` & `odfdo-3.7.9/odfdo/draw_page.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.8/odfdo/element.py` & `odfdo-3.7.9/odfdo/element.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,20 +32,15 @@
 from datetime import datetime, timedelta
 from decimal import Decimal
 from functools import cache
 from re import search
 from typing import Any, NamedTuple
 
 from lxml.etree import Element as lxml_Element
-from lxml.etree import (
-    XPath,
-    _Element,
-    fromstring,
-    tostring,
-)
+from lxml.etree import XPath, _Element, fromstring, tostring
 
 from .const import ODF_COLOR_PROPERTY, OFFICE_PREFIX, OFFICE_VERSION
 from .datatype import Boolean, DateTime
 from .utils import (
     FAMILY_MAPPING,
     FAMILY_ODF_STD,
     CachedElement,
@@ -226,15 +221,15 @@
 def _register_element_class(cls: type[Element], qname: str) -> None:
     # Turn tag name into what lxml is expecting
     tag = _get_lxml_tag(qname)
     if tag not in _class_registry:
         _class_registry[tag] = cls
 
 
-class Text(str):
+class EText(str):
     """Representation of an XML text node. Created to hide the specifics of
     lxml in searching text nodes using XPath.
 
     Constructed like any str object but only accepts lxml text objects.
     """
 
     # There's some black magic in inheriting from str
@@ -1534,26 +1529,26 @@
                 element.append(text)
             for child in children:
                 element.append(child)
             if tail is not None:
                 element.tail = tail
             return (element, True)
 
-    def xpath(self, xpath_query: str) -> list[Element | Text]:
+    def xpath(self, xpath_query: str) -> list[Element | EText]:
         """Apply XPath query to the element and its subtree. Return list of
-        Element or Text instances translated from the nodes found.
+        Element or EText instances translated from the nodes found.
         """
         element = self.__element
         xpath_instance = xpath_compile(xpath_query)
         elements = xpath_instance(element)
-        result: list[Element | Text] = []
+        result: list[Element | EText] = []
         if hasattr(elements, "__iter__"):
             for obj in elements:  # type: ignore
                 if isinstance(obj, (str, bytes)):
-                    result.append(Text(obj))
+                    result.append(EText(obj))
                 elif isinstance(obj, _Element):
                     result.append(Element.from_tag(obj))
                 # else:
                 #     result.append(obj)
         return result
 
     def clear(self) -> None:
@@ -1602,30 +1597,17 @@
         # Remove namespaces
         return self._strip_namespaces(data)
 
     # Element helpers usable from any context
 
     @property
     def document_body(self) -> Element | None:
-        """Return the document body : 'office:body'"""
+        """Return the first children of document body if any: 'office:body/*[1]'"""
         return self.get_element("//office:body/*[1]")
 
-    @document_body.setter
-    def document_body(self, new_body: Element) -> None:
-        """Change in place the full document body content."""
-        body = self.document_body
-        if body is None:
-            raise ValueError("//office:body not found in document")
-        tail = body.tail
-        body.clear()
-        for item in new_body.children:
-            body.append(item)
-        if tail:
-            body.tail = tail
-
     def get_formatted_text(self, context: dict | None = None) -> str:
         """This function should return a beautiful version of the text."""
         return ""
 
     def get_styled_elements(self, name: str = "") -> list[Element]:
         """Brute-force to find paragraphs, tables, etc. using the given style
         name (or all by default).
@@ -1658,55 +1640,14 @@
     def _set_inner_text(self, tag: str, text: str) -> None:
         element = self.get_element(tag)
         if element is None:
             element = Element.from_tag(tag)
             self.append(element)
         element.text = text
 
-    # Dublin core
-
-    @property
-    def dc_creator(self) -> str | None:
-        """Get dc:creator value.
-
-        Return: str (or None if inexistant)
-        """
-        return self._get_inner_text("dc:creator")
-
-    @dc_creator.setter
-    def dc_creator(self, creator: str) -> None:
-        """Set dc:creator value.
-
-        Arguments:
-
-            creator -- str
-        """
-        self._set_inner_text("dc:creator", creator)
-
-    @property
-    def dc_date(self) -> datetime | None:
-        """Get the dc:date value.
-
-        Return: datetime (or None if inexistant)
-        """
-        date = self._get_inner_text("dc:date")
-        if date is None:
-            return None
-        return DateTime.decode(date)
-
-    @dc_date.setter
-    def dc_date(self, date: datetime) -> None:
-        """Set the dc:date value.
-
-        Arguments:
-
-            darz -- datetime
-        """
-        self._set_inner_text("dc:date", DateTime.encode(date))
-
     # SVG
 
     @property
     def svg_title(self) -> str | None:
         return self._get_inner_text("svg:title")
 
     @svg_title.setter
@@ -2053,64 +1994,14 @@
                 return None
             # The name is supposedly unique
             return frame.get_element("draw:image")
         return self._filtered_element(
             "descendant::draw:image", position, url=url, content=content
         )
 
-    # Tables
-
-    def get_tables(
-        self,
-        style: str | None = None,
-        content: str | None = None,
-    ) -> list[Element]:
-        """Return all the tables that match the criteria.
-
-        Arguments:
-
-            style -- str
-
-            content -- str regex
-
-        Return: list of Table
-        """
-        return self._filtered_elements(
-            "descendant::table:table", table_style=style, content=content
-        )
-
-    def get_table(
-        self,
-        position: int = 0,
-        name: str | None = None,
-        content: str | None = None,
-    ) -> Element | None:
-        """Return the table that matches the criteria.
-
-        Arguments:
-
-            position -- int
-
-            name -- str
-
-            content -- str regex
-
-        Return: Table or None if not found
-        """
-        if name is None and content is None:
-            result = self._filtered_element("descendant::table:table", position)
-        else:
-            result = self._filtered_element(
-                "descendant::table:table",
-                position,
-                table_name=name,
-                content=content,
-            )
-        return result
-
     # Named Range
 
     def get_named_ranges(self) -> list[Element]:
         """Return all the tables named ranges.
 
         Return: list of odf_named_range
         """
@@ -2254,15 +2145,15 @@
         """
         annotations = []
         for annotation in self._filtered_elements(
             "descendant::office:annotation", content=content
         ):
             if creator is not None and creator != annotation.dc_creator:
                 continue
-            date = annotation.dc_date
+            date = annotation.date
             if date is None:
                 continue
             if start_date is not None and date < start_date:
                 continue
             if end_date is not None and date >= end_date:
                 continue
             annotations.append(annotation)
@@ -3105,15 +2996,15 @@
 
     # Tracked changes and text change
 
     def get_tracked_changes(self) -> Element | None:
         """Return the tracked-changes part in the text body."""
         return self.get_element("//text:tracked-changes")
 
-    def get_changes_ids(self) -> list[Element | Text]:
+    def get_changes_ids(self) -> list[Element | EText]:
         """Return a list of ids that refers to a change region in the tracked
         changes list.
         """
         # Insertion changes
         xpath_query = "descendant::text:change-start/@text:change-id"
         # Deletion changes
         xpath_query += " | descendant::text:change/@text:change-id"
```

### Comparing `odfdo-3.7.8/odfdo/element_typed.py` & `odfdo-3.7.9/odfdo/element_typed.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.8/odfdo/frame.py` & `odfdo-3.7.9/odfdo/frame.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.8/odfdo/header.py` & `odfdo-3.7.9/odfdo/header.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.8/odfdo/header_rows.py` & `odfdo-3.7.9/odfdo/header_rows.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.8/odfdo/image.py` & `odfdo-3.7.9/odfdo/image.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.8/odfdo/link.py` & `odfdo-3.7.9/odfdo/link.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.8/odfdo/list.py` & `odfdo-3.7.9/odfdo/list.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.8/odfdo/manifest.py` & `odfdo-3.7.9/odfdo/manifest.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,20 +19,20 @@
 # https://github.com/lpod/lpod-python
 # Authors: David Versmisse <david.versmisse@itaapy.com>
 #          Hervé Cauwelier <herve@itaapy.com>
 """Manifest class for manifest.xml part.
 """
 from __future__ import annotations
 
-from .element import Element, Text
+from .element import Element, EText
 from .xmlpart import XmlPart
 
 
 class Manifest(XmlPart):
-    def get_paths(self) -> list[Element | Text]:
+    def get_paths(self) -> list[Element | EText]:
         """Return the list of full paths in the manifest.
 
         Return: list of str
         """
         xpath_query = "//manifest:file-entry/attribute::manifest:full-path"
         return self.xpath(xpath_query)
```

### Comparing `odfdo-3.7.8/odfdo/meta.py` & `odfdo-3.7.9/odfdo/meta.py`

 * *Files 26% similar despite different names*

```diff
@@ -28,124 +28,181 @@
 from datetime import datetime, timedelta
 from decimal import Decimal
 from string import ascii_letters, digits
 from typing import Any
 
 from .datatype import Boolean, Date, DateTime, Duration
 from .element import Element
+from .meta_auto_reload import MetaAutoReload
+from .meta_hyperlink_behaviour import MetaHyperlinkBehaviour
+from .meta_template import MetaTemplate
+from .mixin_dc_creator import DcCreatorMixin
+from .mixin_dc_date import DcDateMixin
 from .utils import to_str
 from .version import __version__
 from .xmlpart import XmlPart
 
 GENERATOR = f"odfdo {__version__}"
 
 
-class Meta(XmlPart):
+class Meta(XmlPart, DcCreatorMixin, DcDateMixin):
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         super().__init__(*args, **kwargs)
         self._generator_modified: bool = False
 
     def get_meta_body(self) -> Element:
         return self.get_element("//office:meta")
 
     def get_title(self) -> str | None:
         """Get the title of the document.
 
         This is not the first heading but the title metadata.
 
+        (Also available as "self.title" property.)
+
         Return: str (or None if inexistant)
         """
         element = self.get_element("//dc:title")
         if element is None:
             return None
         return element.text
 
     def set_title(self, title: str) -> None:
         """Set the title of the document.
 
         This is not the first heading but the title metadata.
 
+        (Also available as "self.title" property.)
+
         Arguments:
 
             title -- str
         """
         element = self.get_element("//dc:title")
         if element is None:
             element = Element.from_tag("dc:title")
             self.get_meta_body().append(element)
         element.text = title
 
+    @property
+    def title(self) -> str | None:
+        """Get or set the title of the document <dc:title>.
+
+        Return: str (or None if inexistant)
+        """
+        return self.get_title()
+
+    @title.setter
+    def title(self, title: str) -> None:
+        return self.set_title(title)
+
     def get_description(self) -> str | None:
         """Get the description of the document. Also known as comments.
 
+        (Also available as "self.description" property.)
+
         Return: str (or None if inexistant)
         """
         element = self.get_element("//dc:description")
         if element is None:
             return None
         return element.text
 
     # As named in OOo
     get_comments = get_description
 
     def set_description(self, description: str) -> None:
         """Set the description of the document. Also known as comments.
 
+        (Also available as "self.description" property.)
+
         Arguments:
 
             description -- str
         """
         element = self.get_element("//dc:description")
         if element is None:
             element = Element.from_tag("dc:description")
             self.get_meta_body().append(element)
         element.text = description
 
     set_comments = set_description
 
+    @property
+    def description(self) -> str | None:
+        """Get or set the description of a document <dc:description>.
+
+        Return: str (or None if inexistant)
+        """
+        return self.get_description()
+
+    @description.setter
+    def description(self, description: str) -> None:
+        return self.set_description(description)
+
     def get_subject(self) -> str | None:
         """Get the subject of the document.
 
+        (Also available as "self.subject" property.)
+
         Return: str (or None if inexistant)
         """
         element = self.get_element("//dc:subject")
         if element is None:
             return None
         return element.text
 
     def set_subject(self, subject: str) -> None:
         """Set the subject of the document.
 
+        (Also available as "self.subject" property.)
+
         Arguments:
 
             subject -- str
         """
         element = self.get_element("//dc:subject")
         if element is None:
             element = Element.from_tag("dc:subject")
             self.get_meta_body().append(element)
         element.text = subject
 
+    @property
+    def subject(self) -> str | None:
+        """Get or set the subject of a document <dc:subject>.
+
+        Return: str (or None if inexistant)
+        """
+        return self.get_subject()
+
+    @subject.setter
+    def subject(self, subject: str) -> None:
+        return self.set_subject(subject)
+
     def get_language(self) -> str | None:
-        """Get the language code of the document.
+        """Get the default language of the document.
+
+        (Also available as "self.language" property.)
 
         Return: str (or None if inexistant)
 
         Example::
 
             >>> document.meta.get_language()
             fr-FR
         """
         element = self.get_element("//dc:language")
         if element is None:
             return None
         return element.text
 
     def set_language(self, language: str) -> None:
-        """Set the language code of the document.
+        """Set the default language of the document.
+
+        (Also available as "self.language" property.)
 
         Arguments:
 
             language -- str
 
         Example::
 
@@ -179,65 +236,174 @@
         parts = lang.split("-")
         if len(parts) > 3:
             return False
         if not test_part1(parts[0]):
             return False
         return all(test_part2(p) for p in parts[1:])
 
-    def get_modification_date(self) -> datetime | None:
-        """Get the last modified date of the document.
+    @property
+    def language(self) -> str | None:
+        """Get or set the default language of the document <dc:language>.
 
-        Return: datetime (or None if inexistant)
+        Return: str (or None if inexistant)
         """
-        element = self.get_element("//dc:date")
-        if element is None:
-            return None
-        modification_date = element.text
-        return DateTime.decode(modification_date)
+        return self.get_language()
 
-    def set_modification_date(self, date: datetime) -> None:
-        """Set the last modified date of the document.
-
-        Arguments:
-
-            date -- datetime
-        """
-        element = self.get_element("//dc:date")
-        if element is None:
-            element = Element.from_tag("dc:date")
-            self.get_meta_body().append(element)
-        element.text = DateTime.encode(date)
+    @language.setter
+    def language(self, language: str) -> None:
+        return self.set_language(language)
 
     def get_creation_date(self) -> datetime | None:
         """Get the creation date of the document.
 
+        (Also available as "self.creation_date" property.)
+
         Return: datetime (or None if inexistant)
         """
         element = self.get_element("//meta:creation-date")
         if element is None:
             return None
         creation_date = element.text
         return DateTime.decode(creation_date)
 
-    def set_creation_date(self, date: datetime) -> None:
+    def set_creation_date(self, date: datetime | None = None) -> None:
         """Set the creation date of the document.
 
+        If provided datetime is None, use current time.
+
+        (Also available as "self.creation_date" property.)
+
         Arguments:
 
             date -- datetime
         """
         element = self.get_element("//meta:creation-date")
         if element is None:
             element = Element.from_tag("meta:creation-date")
             self.get_meta_body().append(element)
+        if date is None:
+            date = datetime.now()
         element.text = DateTime.encode(date)
 
+    @property
+    def creation_date(self) -> datetime | None:
+        """Get or set the date and time when a document was created
+        <meta:creation-date>.
+
+        If provided datetime is None, use current time.
+
+        Return: datetime (or None if inexistant)
+        """
+        return self.get_creation_date()
+
+    @creation_date.setter
+    def creation_date(self, date: datetime | None = None) -> None:
+        return self.set_creation_date(date)
+
+    @property
+    def print_date(self) -> datetime | None:
+        """Get or set the date and time when a document when a document was last printed
+        <meta:print-date>
+
+        If provided datetime is None, use current time.
+
+        Return: datetime (or None if inexistant)
+        """
+        element = self.get_element("//meta:print-date")
+        if element is None:
+            return None
+        date = element.text
+        return DateTime.decode(date)
+
+    @print_date.setter
+    def print_date(self, date: datetime | None = None) -> None:
+        element = self.get_element("//meta:print-date")
+        if element is None:
+            element = Element.from_tag("meta:print-date")
+            self.get_meta_body().append(element)
+        if date is None:
+            date = datetime.now()
+        element.text = DateTime.encode(date)
+
+    def get_template(self) -> MetaTemplate | None:
+        """Get the MetaTemplate <meta:template> element or None."""
+        element = self.get_element("//meta:template")
+        if element is None:
+            return None
+        return element
+
+    @property
+    def template(self) -> MetaTemplate | None:
+        """Get the MetaTemplate <meta:template> element or None."""
+        return self.get_template()
+
+    def set_template(
+        self,
+        date: datetime | None = None,
+        href: str = "",
+        title: str = "",
+    ) -> None:
+        """Set the MetaTemplate <meta:template> element."""
+        template = MetaTemplate(date=date, href=href, title=title)
+        current = self.template
+        if isinstance(current, MetaTemplate):
+            current.delete()
+        self.get_meta_body().append(template)
+
+    def get_auto_reload(self) -> MetaAutoReload | None:
+        """Get the MetaAutoReload <meta:auto-reload> element or None."""
+        element = self.get_element("//meta:auto-reload")
+        if element is None:
+            return None
+        return element
+
+    @property
+    def auto_reload(self) -> MetaAutoReload | None:
+        """Get the MetaAutoReload <meta:auto-reload> element or None."""
+        return self.get_auto_reload()
+
+    def set_auto_reload(self, delay: timedelta, href: str = "") -> None:
+        """Set the MetaAutoReload <meta:auto-reload> element."""
+        autoreload = MetaAutoReload(delay=delay, href=href)
+        current = self.auto_reload
+        if isinstance(current, MetaAutoReload):
+            current.delete()
+        self.get_meta_body().append(autoreload)
+
+    def get_hyperlink_behaviour(self) -> MetaHyperlinkBehaviour | None:
+        """Get the MetaHyperlinkBehaviour <meta:hyperlink-behaviour> element or None."""
+        element = self.get_element("//meta:hyperlink-behaviour")
+        if element is None:
+            return None
+        return element
+
+    @property
+    def hyperlink_behaviour(self) -> MetaAutoReload | None:
+        """Get the MetaHyperlinkBehaviour <meta:hyperlink-behaviour> element or None."""
+        return self.get_hyperlink_behaviour()
+
+    def set_hyperlink_behaviour(
+        self,
+        target_frame_name: str = "_blank",
+        show: str = "replace",
+    ) -> None:
+        """Set the MetaHyperlinkBehaviour <meta:hyperlink-behaviour> element."""
+        behaviour = MetaHyperlinkBehaviour(
+            target_frame_name=target_frame_name, show=show
+        )
+        current = self.hyperlink_behaviour
+        if isinstance(current, MetaHyperlinkBehaviour):
+            current.delete()
+        self.get_meta_body().append(behaviour)
+
     def get_initial_creator(self) -> str | None:
         """Get the first creator of the document.
 
+        (Also available as "self.initial_creator" property.)
+
         Return: str (or None if inexistant)
 
         Example::
 
             >>> document.meta.get_initial_creator()
             Unknown
         """
@@ -245,127 +411,170 @@
         if element is None:
             return None
         return element.text
 
     def set_initial_creator(self, creator: str) -> None:
         """Set the first creator of the document.
 
+        (Also available as "self.initial_creator" property.)
+
         Arguments:
 
             creator -- str
 
         Example::
 
             >>> document.meta.set_initial_creator("Plato")
         """
         element = self.get_element("//meta:initial-creator")
         if element is None:
             element = Element.from_tag("meta:initial-creator")
             self.get_meta_body().append(element)
         element.text = creator
 
-    def get_creator(self) -> str | None:
-        """Get the creator of the document.
+    @property
+    def initial_creator(self) -> str | None:
+        """Get or set the initial creator of a document
+        <meta:initial-creator>.
 
         Return: str (or None if inexistant)
+        """
+        return self.get_initial_creator()
 
-        Example::
+    @initial_creator.setter
+    def initial_creator(self, creator: str) -> None:
+        return self.set_initial_creator(creator)
 
-            >>> document.meta.get_creator()
-            Unknown
+    @property
+    def printed_by(self) -> str | None:
+        """Get or set the name of the last person who printed a document.
+        <meta:printed-by>
+
+        Return: str (or None if inexistant)
         """
-        element = self.get_element("//dc:creator")
+        element = self.get_element("//meta:printed-by")
         if element is None:
             return None
         return element.text
 
-    def set_creator(self, creator: str) -> None:
-        """Set the creator of the document.
-
-        Arguments:
-
-            creator -- str
-
-        Example::
-
-            >>> document.meta.set_creator("Plato")
-        """
-        element = self.get_element("//dc:creator")
+    @printed_by.setter
+    def printed_by(self, printed_by: str) -> None:
+        element = self.get_element("//meta:printed-by")
         if element is None:
-            element = Element.from_tag("dc:creator")
+            element = Element.from_tag("meta:printed-by")
             self.get_meta_body().append(element)
-        element.text = creator
+        element.text = printed_by
 
     def get_keywords(self) -> str | None:
         """Get the keywords of the document. Return the field as-is, without
         any assumption on the keyword separator.
 
+        (Also available as "self.keyword" and "self.keywords" property.)
+
         Return: str (or None if inexistant)
         """
         element = self.get_element("//meta:keyword")
         if element is None:
             return None
         return element.text
 
     def set_keywords(self, keywords: str) -> None:
         """Set the keywords of the document. Although the name is plural, a
         str string is required, so join your list first.
 
+        (Also available as "self.keyword" and "self.keywords" property.)
+
         Arguments:
 
             keywords -- str
         """
         element = self.get_element("//meta:keyword")
         if element is None:
             element = Element.from_tag("meta:keyword")
             self.get_meta_body().append(element)
         element.text = keywords
 
+    @property
+    def keyword(self) -> str | None:
+        """Get or set some keyword(s) keyword pertaining to a document
+        <dc:keyword>.
+
+        Return: str (or None if inexistant)
+        """
+        return self.get_keywords()
+
+    @keyword.setter
+    def keyword(self, keyword: str) -> None:
+        return self.set_keywords(keyword)
+
+    keywords = keyword
+
     def get_editing_duration(self) -> timedelta | None:
         """Get the time the document was edited, as reported by the
         generator.
 
+        (Also available as "self.editing_duration" property.)
+
         Return: timedelta (or None if inexistant)
         """
         element = self.get_element("//meta:editing-duration")
         if element is None:
             return None
         duration = element.text
         return Duration.decode(duration)
 
     def set_editing_duration(self, duration: timedelta) -> None:
         """Set the time the document was edited.
 
+        (Also available as "self.editing_duration" property.)
+
         Arguments:
 
             duration -- timedelta
         """
         if not isinstance(duration, timedelta):
             raise TypeError("duration must be a timedelta")
         element = self.get_element("//meta:editing-duration")
         if element is None:
             element = Element.from_tag("meta:editing-duration")
             self.get_meta_body().append(element)
         element.text = Duration.encode(duration)
 
+    @property
+    def editing_duration(self) -> timedelta | None:
+        """Get or set the total time spent editing a document
+        <meta:editing-duration>.
+
+        Return: timedelta (or None if inexistant)
+        """
+        return self.get_editing_duration()
+
+    @editing_duration.setter
+    def editing_duration(self, duration: timedelta) -> None:
+        return self.set_editing_duration(duration)
+
     def get_editing_cycles(self) -> int | None:
         """Get the number of times the document was edited, as reported by
         the generator.
 
+        (Also available as "self.editing_cycles" property.)
+
         Return: int (or None if inexistant)
         """
         element = self.get_element("//meta:editing-cycles")
         if element is None:
             return None
         cycles = element.text
         return int(cycles)
 
     def set_editing_cycles(self, cycles: int) -> None:
         """Set the number of times the document was edited.
 
+        (Also available as "self.editing_cycles" property.)
+
         Arguments:
 
             cycles -- int
         """
         if not isinstance(cycles, int):
             raise TypeError("cycles must be an int")
         if cycles < 1:
@@ -373,14 +582,30 @@
         element = self.get_element("//meta:editing-cycles")
         if element is None:
             element = Element.from_tag("meta:editing-cycles")
             self.get_meta_body().append(element)
         element.text = str(cycles)
 
     @property
+    def editing_cycles(self) -> int | None:
+        """Get or set the number of times a document has been edited
+        <meta:editing-cycles>.
+
+        When a document is created, this value is set to 1. Each time
+        a document is saved, the editing-cycles number is incremented by 1.
+
+        Return: int (or None if inexistant)
+        """
+        return self.get_editing_cycles()
+
+    @editing_cycles.setter
+    def editing_cycles(self, cycles: int) -> None:
+        return self.set_editing_cycles(cycles)
+
+    @property
     def generator(self) -> str | None:
         """Get or set the signature of the software that generated this
         document.
 
         Return: str (or None if inexistant)
 
         Example::
@@ -402,29 +627,29 @@
             self.get_meta_body().append(element)
         element.text = generator
         self._generator_modified = True
 
     def get_generator(self) -> str | None:
         """Get the signature of the software that generated this document.
 
-        (Also available as "self.generator" getter/setter.)
+        (Also available as "self.generator" property.)
 
         Return: str (or None if inexistant)
 
         Example::
 
             >>> document.meta.get_generator()
             KOffice/2.0.0
         """
         return self.generator
 
     def set_generator(self, generator: str) -> None:
         """Set the signature of the software that generated this document.
 
-        (Also available as "self.generator" getter/setter.)
+        (Also available as "self.generator" property.)
 
         Arguments:
 
             generator -- str
 
         Example::
 
@@ -440,15 +665,17 @@
 
             >>> document.meta.set_generator_default()
         """
         if not self._generator_modified:
             self.generator = GENERATOR
 
     def get_statistic(self) -> dict[str, int] | None:
-        """Get the statistic from the software that generated this document.
+        """Get the statistics about a document.
+
+        (Also available as "self.statistic" property.)
 
         Return: dict (or None if inexistant)
 
         Example::
 
             >>> document.get_statistic():
             {'meta:table-count': 1,
@@ -464,16 +691,17 @@
             return None
         statistic = {}
         for key, value in element.attributes.items():
             statistic[to_str(key)] = int(value)
         return statistic
 
     def set_statistic(self, statistic: dict[str, int]) -> None:
-        """Set the statistic for the documents: number of words, paragraphs,
-        etc.
+        """Set the statistics about a document.
+
+        (Also available as "self.statistic" property.)
 
         Arguments:
 
             statistic -- dict
 
         Example::
 
@@ -492,16 +720,44 @@
         for key, value in statistic.items():
             try:
                 ivalue = int(value)
             except ValueError as e:
                 raise TypeError("Statistic value must be a int") from e
             element.set_attribute(to_str(key), str(ivalue))
 
+    @property
+    def statistic(self) -> dict[str, int] | None:
+        """Get or set the statistics about a document
+        <meta:document-statistic>.
+
+        Return: dict (or None if inexistant)
+
+        Example::
+
+            >>> document.get_statistic():
+            {'meta:table-count': 1,
+             'meta:image-count': 2,
+             'meta:object-count': 3,
+             'meta:page-count': 4,
+             'meta:paragraph-count': 5,
+             'meta:word-count': 6,
+             'meta:character-count': 7}
+        """
+        return self.get_statistic()
+
+    @statistic.setter
+    def statistic(self, statistic: dict[str, int]) -> None:
+        return self.set_statistic(statistic)
+
     def get_user_defined_metadata(self) -> dict[str, Any]:
-        """Return a dict of str/value mapping.
+        """Get all additional user-defined metadata for a document.
+
+        (Also available as "self.user_defined_metadata" property.)
+
+        Return a dict of str/value mapping.
 
         Value types can be: Decimal, date, time, boolean or str.
         """
         result: dict[str, Any] = {}
         for item in self.get_elements("//meta:user-defined"):
             if not isinstance(item, Element):
                 continue
@@ -509,14 +765,39 @@
             name = item.get_attribute_string("meta:name")
             if name is None:
                 continue
             value = self._get_meta_value(item)
             result[name] = value
         return result
 
+    def clear_user_defined_metadata(self) -> None:
+        """Remove all user-defined metadata."""
+        while True:
+            element = self.get_element("//meta:user-defined")
+            if isinstance(element, Element):
+                element.delete()
+                continue
+            break
+
+    @property
+    def user_defined_metadata(self) -> dict[str, Any]:
+        """Get or set all additional user-defined metadata for a document.
+
+        Return a dict of str/value mapping.
+
+        Value types can be: Decimal, date, time, boolean or str.
+        """
+        return self.get_user_defined_metadata()
+
+    @user_defined_metadata.setter
+    def user_defined_metadata(self, metadata: dict[str, Any]) -> None:
+        self.clear_user_defined_metadata()
+        for key, val in metadata.items():
+            self.set_user_defined_metadata(name=key, value=val)
+
     def get_user_defined_metadata_of_name(self, keyname: str) -> dict[str, Any] | None:
         """Return the content of the user defined metadata of that name.
         Return None if no name matchs or a dic of fields.
 
         Arguments:
 
             name -- string, name (meta:name content)
```

### Comparing `odfdo-3.7.8/odfdo/note.py` & `odfdo-3.7.9/odfdo/note.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 """
 from __future__ import annotations
 
 from datetime import datetime
 from typing import Any
 
 from .element import Element, PropDef, register_element_class
+from .mixin_dc_creator import DcCreatorMixin
+from .mixin_dc_date import DcDateMixin
 
 
 def get_unique_office_name(element: Element | None = None) -> str:
     """Provide an autogenerated unique "office:name" for the document."""
     if element is not None:
         body = element.document_body
     else:
@@ -139,15 +141,15 @@
         if not self.note_body:
             pass
 
 
 Note._define_attribut_property()
 
 
-class Annotation(Element):
+class Annotation(Element, DcCreatorMixin, DcDateMixin):
     """Annotation element credited to the given creator with the
     given text, optionally dated (current date by default).
     If name not provided and some parent is provided, the name is
     autogenerated.
 
     Arguments:
 
@@ -180,23 +182,41 @@
         # fixme : use offset
         # TODO allow paragraph and text styles
         super().__init__(**kwargs)
 
         if self._do_init:
             self.note_body = text_or_element  # type:ignore
             if creator:
-                self.dc_creator = creator
+                self.creator = creator
             if date is None:
                 date = datetime.now()
-            self.dc_date = date
+            self.date = date
             if not name:
                 name = get_unique_office_name(parent)
                 self.name = name
 
     @property
+    def dc_creator(self) -> str | None:
+        """Alias for self.creator property."""
+        return self.creator
+
+    @dc_creator.setter
+    def dc_creator(self, creator: str) -> None:
+        self.creator = creator
+
+    @property
+    def dc_date(self) -> datetime | None:
+        """Alias for self.date property."""
+        return self.date
+
+    @dc_date.setter
+    def dc_date(self, dtdate: datetime) -> None:
+        self.date = dtdate
+
+    @property
     def note_body(self) -> str:
         return self.text_content
 
     @note_body.setter
     def note_body(self, text_or_element: Element | str | None) -> None:
         if text_or_element is None:
             self.text_content = ""
```

### Comparing `odfdo-3.7.8/odfdo/paragraph.py` & `odfdo-3.7.9/odfdo/paragraph.py`

 * *Files 0% similar despite different names*

```diff
@@ -257,17 +257,17 @@
                 text_or_element=body, creator=creator, date=date, parent=self
             )
         else:
             # XXX clone or modify the argument?
             if body:
                 annotation_element.note_body = body
             if creator:
-                annotation_element.dc_creator = creator
+                annotation_element.creator = creator
             if date:
-                annotation_element.dc_date = date
+                annotation_element.date = date
         annotation_element.check_validity()
 
         # special case: content is an odf element (ie: a paragraph)
         if isinstance(content, Element):
             if content.is_empty():
                 content.insert(annotation_element, xmlposition=NEXT_SIBLING)
                 return annotation_element
```

### Comparing `odfdo-3.7.8/odfdo/paragraph_base.py` & `odfdo-3.7.9/odfdo/paragraph_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 "text:line-break".
 """
 from __future__ import annotations
 
 import re
 from typing import Any
 
-from .element import Element, PropDef, Text, register_element_class
+from .element import Element, EText, PropDef, register_element_class
 from .utils import to_str
 
 _rsplitter = re.compile("(\n|\t|  +)")
 _rspace = re.compile("^  +$")
 
 
 def _get_formatted_text(  # noqa: C901
@@ -43,21 +43,21 @@
 ) -> str:
     if context is None:
         context = {}
     document = context.get("document", None)
     rst_mode = context.get("rst_mode", False)
 
     result: list[str] = []
-    objects: list[Element | Text] = []
+    objects: list[Element | EText] = []
     if with_text:
         objects = element.xpath("*|text()")
     else:
         objects = [x for x in element.children]  # noqa: C416
     for obj in objects:
-        if isinstance(obj, Text):
+        if isinstance(obj, EText):
             result.append(obj)
             continue
         tag = obj.tag
         # Good tags with text
         if tag in ("text:a", "text:p"):
             result.append(_get_formatted_text(obj, context, with_text=True))
             continue
```

### Comparing `odfdo-3.7.8/odfdo/reference.py` & `odfdo-3.7.9/odfdo/reference.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.8/odfdo/row.py` & `odfdo-3.7.9/odfdo/row.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.8/odfdo/scripts/diff.py` & `odfdo-3.7.9/odfdo/scripts/diff.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.8/odfdo/scripts/folder.py` & `odfdo-3.7.9/odfdo/scripts/folder.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.8/odfdo/scripts/headers.py` & `odfdo-3.7.9/odfdo/scripts/headers.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.8/odfdo/scripts/highlight.py` & `odfdo-3.7.9/odfdo/scripts/highlight.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.8/odfdo/scripts/replace.py` & `odfdo-3.7.9/odfdo/scripts/replace.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.8/odfdo/scripts/show.py` & `odfdo-3.7.9/odfdo/scripts/show.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.8/odfdo/scripts/styles.py` & `odfdo-3.7.9/odfdo/scripts/styles.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.8/odfdo/scripts/table_shrink.py` & `odfdo-3.7.9/odfdo/scripts/table_shrink.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.8/odfdo/scriptutils.py` & `odfdo-3.7.9/odfdo/scriptutils.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.8/odfdo/section.py` & `odfdo-3.7.9/odfdo/section.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.8/odfdo/shapes.py` & `odfdo-3.7.9/odfdo/shapes.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.8/odfdo/smil.py` & `odfdo-3.7.9/odfdo/smil.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.8/odfdo/style.py` & `odfdo-3.7.9/odfdo/style.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.8/odfdo/styles.py` & `odfdo-3.7.9/odfdo/styles.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.8/odfdo/table.py` & `odfdo-3.7.9/odfdo/table.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.8/odfdo/templates/drawing.otg` & `odfdo-3.7.9/odfdo/templates/drawing.otg`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.8/odfdo/templates/lpod_styles.odt` & `odfdo-3.7.9/odfdo/templates/lpod_styles.odt`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.8/odfdo/templates/presentation.otp` & `odfdo-3.7.9/odfdo/templates/presentation.otp`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.8/odfdo/templates/spreadsheet.ots` & `odfdo-3.7.9/odfdo/templates/spreadsheet.ots`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.8/odfdo/templates/text.ott` & `odfdo-3.7.9/odfdo/templates/text.ott`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.8/odfdo/toc.py` & `odfdo-3.7.9/odfdo/toc.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.8/odfdo/tracked_changes.py` & `odfdo-3.7.9/odfdo/tracked_changes.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,20 +24,21 @@
 (ChangeInfo, TextInsertion, TextChange...).
 """
 from __future__ import annotations
 
 from datetime import datetime
 from typing import Any
 
-from .datatype import DateTime
 from .element import FIRST_CHILD, LAST_CHILD, Element, register_element_class
+from .mixin_dc_creator import DcCreatorMixin
+from .mixin_dc_date import DcDateMixin
 from .paragraph import Paragraph
 
 
-class ChangeInfo(Element):
+class ChangeInfo(Element, DcCreatorMixin, DcDateMixin):
     """The "office:change-info" element represents who made a change and when.
     It may also contain a comment (one or more Paragrah "text:p" elements)
     on the change.
 
     The comments available in the ChangeInfo are available through:
       - get_paragraphs and get_paragraph methods for actual Paragraph.
       - get_comments for a plain text version
@@ -55,47 +56,16 @@
         self,
         creator: str | None = None,
         date: datetime | None = None,
         **kwargs: Any,
     ) -> None:
         super().__init__(**kwargs)
         if self._do_init:
-            self.set_dc_creator(creator)
-            self.set_dc_date(date)
-
-    def set_dc_creator(self, creator: str | None = None) -> None:
-        """Set the creator of the change. Default for creator is 'Unknown'.
-
-        Arguments:
-
-            creator -- str (or None)
-        """
-        element = self.get_element("dc:creator")
-        if element is None:
-            element = Element.from_tag("dc:creator")
-            self.insert(element, xmlposition=FIRST_CHILD)
-        if not creator:
-            creator = "Unknown"
-        element.text = creator
-
-    def set_dc_date(self, date: datetime | None = None) -> None:
-        """Set the date of the change. If date is None, use current time.
-
-        Arguments:
-
-            date -- datetime (or None)
-        """
-        if date is None:
-            date = datetime.now()
-        dcdate = DateTime.encode(date)
-        element = self.get_element("dc:date")
-        if element is None:
-            element = Element.from_tag("dc:date")
-            self.insert(element, xmlposition=LAST_CHILD)
-        element.text = dcdate
+            self.creator = creator or "Unknown"
+            self.date = date
 
     def get_comments(self, joined: bool = True) -> str | list[str]:
         """Get text content of the comments. If joined is True (default), the
         text of different paragraphs is concatenated, else a list of strings,
         one per paragraph, is returned.
 
         Arguments:
```

### Comparing `odfdo-3.7.8/odfdo/utils/__init__.py` & `odfdo-3.7.9/odfdo/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.8/odfdo/utils/cache_map.py` & `odfdo-3.7.9/odfdo/utils/cache_map.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.8/odfdo/utils/cached_element.py` & `odfdo-3.7.9/odfdo/utils/cached_element.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.8/odfdo/utils/color.py` & `odfdo-3.7.9/odfdo/utils/color.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.8/odfdo/utils/coordinates.py` & `odfdo-3.7.9/odfdo/utils/coordinates.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.8/odfdo/utils/formula.py` & `odfdo-3.7.9/odfdo/utils/formula.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.8/odfdo/utils/isiterable.py` & `odfdo-3.7.9/odfdo/utils/isiterable.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.8/odfdo/utils/str_convert.py` & `odfdo-3.7.9/odfdo/utils/str_convert.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.8/odfdo/utils/style_constants.py` & `odfdo-3.7.9/odfdo/utils/style_constants.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.8/odfdo/utils/xpath_query.py` & `odfdo-3.7.9/odfdo/utils/xpath_query.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.8/odfdo/variable.py` & `odfdo-3.7.9/odfdo/variable.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.8/odfdo/version.py` & `odfdo-3.7.9/odfdo/version.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.8/odfdo/xmlpart.py` & `odfdo-3.7.9/odfdo/xmlpart.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from copy import deepcopy
 from io import BytesIO
 from typing import Any
 
 from lxml.etree import _ElementTree, parse, tostring
 
 from .container import Container
-from .element import Element, Text
+from .element import Element, EText
 
 
 class XmlPart:
     """Representation of an XML part.
 
     Abstraction of the XML library behind.
     """
@@ -63,35 +63,48 @@
         if self.__root is None:
             tree = self._get_tree()
             self.__root = Element.from_tag(tree.getroot())
         return self.__root
 
     @property
     def body(self) -> Element:
+        """Get or set the document body : 'office:body'"""
         body = self.root.document_body
         if not isinstance(body, Element):
-            raise ValueError(f"No body found in {self.part_name!r}")  # noqa:TRY004
+            raise TypeError(f"No body found in {self.part_name!r}")
         return body
 
-    def get_elements(self, xpath_query: str) -> list[Element | Text]:
+    @body.setter
+    def body(self, new_body: Element) -> None:
+        body = self.root.document_body
+        if not isinstance(body, Element):
+            raise TypeError("//office:body not found in document")
+        tail = body.tail
+        body.clear()
+        for item in new_body.children:
+            body.append(item)
+        if tail:
+            body.tail = tail
+
+    def get_elements(self, xpath_query: str) -> list[Element | EText]:
         root = self.root
         return root.xpath(xpath_query)
 
     def get_element(self, xpath_query: str) -> Any:
         result = self.get_elements(xpath_query)
         if not result:
             return None
         return result[0]
 
     def delete_element(self, child: Element) -> None:
         child.delete()
 
-    def xpath(self, xpath_query: str) -> list[Element | Text]:
+    def xpath(self, xpath_query: str) -> list[Element | EText]:
         """Apply XPath query to the XML part. Return list of Element or
-        Text instances translated from the nodes found.
+        EText instances translated from the nodes found.
         """
         root = self.root
         return root.xpath(xpath_query)
 
     @property
     def clone(self) -> XmlPart:
         clone = object.__new__(self.__class__)
```

### Comparing `odfdo-3.7.8/pyproject.toml` & `odfdo-3.7.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "odfdo"
-version = "3.7.8"
+version = "3.7.9"
 description = "Python library for OpenDocument Format"
 license = "Apache-2.0"
 keywords = ["python", "library", "ODF", "OpenDocument"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Developers",
```

### Comparing `odfdo-3.7.8/PKG-INFO` & `odfdo-3.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odfdo
-Version: 3.7.8
+Version: 3.7.9
 Summary: Python library for OpenDocument Format
 Home-page: https://github.com/jdum/odfdo
 License: Apache-2.0
 Keywords: python,library,ODF,OpenDocument
 Author: Jérôme Dumonteil
 Author-email: jerome.dumonteil@gmail.com
 Requires-Python: >=3.9,<4
```

