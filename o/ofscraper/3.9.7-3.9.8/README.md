# Comparing `tmp/ofscraper-3.9.7.tar.gz` & `tmp/ofscraper-3.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofscraper-3.9.7.tar", max compression
+gzip compressed data, was "ofscraper-3.9.8.tar", max compression
```

## Comparing `ofscraper-3.9.7.tar` & `ofscraper-3.9.8.tar`

### file list

```diff
@@ -1,230 +1,232 @@
--rw-r--r--   0        0        0     1067 2024-05-12 12:52:16.784428 ofscraper-3.9.7/LICENSE
--rw-r--r--   0        0        0     4213 2024-05-12 12:52:16.784428 ofscraper-3.9.7/README.md
--rwxr-xr-x   0        0        0      283 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/__main__.py
--rw-r--r--   0        0        0     1064 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/__version__.py
--rw-r--r--   0        0        0      999 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/__version__.pye
--rw-r--r--   0        0        0    16148 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/api/archive.py
--rw-r--r--   0        0        0      274 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/api/common/logs.py
--rw-r--r--   0        0        0    14697 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/api/highlights.py
--rw-r--r--   0        0        0     1479 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/api/init.py
--rw-r--r--   0        0        0    14238 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/api/labels.py
--rw-r--r--   0        0        0     2912 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/api/me.py
--rw-r--r--   0        0        0    18425 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/api/messages.py
--rw-r--r--   0        0        0    13861 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/api/paid.py
--rw-r--r--   0        0        0     8581 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/api/pinned.py
--rw-r--r--   0        0        0     6176 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/api/profile.py
--rw-r--r--   0        0        0     1718 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/api/subscriptions/helpers.py
--rw-r--r--   0        0        0     3381 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/api/subscriptions/individual.py
--rw-r--r--   0        0        0    12660 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/api/subscriptions/lists.py
--rw-r--r--   0        0        0     8171 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/api/subscriptions/subscriptions.py
--rw-r--r--   0        0        0    17204 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/api/timeline.py
--rw-r--r--   0        0        0     1460 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/classes/base.py
--rw-r--r--   0        0        0      876 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/classes/labels.py
--rw-r--r--   0        0        0    15560 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/classes/media.py
--rw-r--r--   0        0        0     6005 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/classes/models.py
--rw-r--r--   0        0        0     1771 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/classes/multiprocessprogress.py
--rw-r--r--   0        0        0    20597 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/classes/placeholder.py
--rw-r--r--   0        0        0     5156 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/classes/posts.py
--rw-r--r--   0        0        0    18209 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/classes/sessionmanager.py
--rw-r--r--   0        0        0      156 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/classes/table/button.py
--rw-r--r--   0        0        0     1689 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/classes/table/fields/boolfield.py
--rw-r--r--   0        0        0     1370 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/classes/table/fields/datefield.py
--rw-r--r--   0        0        0      629 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/classes/table/fields/mediafield.py
--rw-r--r--   0        0        0      694 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/classes/table/fields/numfield.py
--rw-r--r--   0        0        0     1302 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/classes/table/fields/pricefield.py
--rw-r--r--   0        0        0      678 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/classes/table/fields/responsefield.py
--rw-r--r--   0        0        0     1417 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/classes/table/fields/selectfield.py
--rw-r--r--   0        0        0     1487 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/classes/table/fields/textsearch.py
--rw-r--r--   0        0        0     2460 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/classes/table/fields/timefield.py
--rw-r--r--   0        0        0     1893 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/classes/table/inputs/filterinput.py
--rw-r--r--   0        0        0      117 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/classes/table/inputs/intergerinput.py
--rw-r--r--   0        0        0      113 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/classes/table/inputs/strinput.py
--rw-r--r--   0        0        0      297 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/classes/table/row_names.py
--rw-r--r--   0        0        0     4583 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/classes/table/status.py
--rw-r--r--   0        0        0    21258 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/classes/table/table.py
--rw-r--r--   0        0        0      156 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/classes/table/table_console.py
--rw-r--r--   0        0        0        1 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/commands/actions/__init__.py
--rw-r--r--   0        0        0     6465 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/commands/actions/download/download.py
--rw-r--r--   0        0        0    21884 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/commands/actions/download/post.py
--rw-r--r--   0        0        0    11597 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/commands/actions/like.py
--rw-r--r--   0        0        0     1545 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/commands/actions/scrape_context.py
--rw-r--r--   0        0        0     1039 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/commands/add_select/add_selected.py
--rw-r--r--   0        0        0    26132 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/commands/check.py
--rw-r--r--   0        0        0    11014 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/commands/manual.py
--rw-r--r--   0        0        0     8260 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/commands/metadata.py
--rw-r--r--   0        0        0      556 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/commands/picker.py
--rwxr-xr-x   0        0        0     3785 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/commands/scraper.py
--rw-r--r--   0        0        0       53 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/const/binary.py
--rw-r--r--   0        0        0     1655 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/const/config.py
--rw-r--r--   0        0        0     1002 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/const/constants.py
--rw-r--r--   0        0        0       74 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/const/date.py
--rw-r--r--   0        0        0      190 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/const/download.py
--rw-r--r--   0        0        0      204 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/const/files.py
--rw-r--r--   0        0        0     1375 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/const/general.py
--rw-r--r--   0        0        0       93 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/const/logger.py
--rw-r--r--   0        0        0      120 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/const/metadata.py
--rw-r--r--   0        0        0      862 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/const/other_url.py
--rw-r--r--   0        0        0     1908 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/const/prompts.py
--rw-r--r--   0        0        0     1808 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/const/req.py
--rw-r--r--   0        0        0      271 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/const/table.py
--rw-r--r--   0        0        0   265533 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/const/test_constants.py
--rw-r--r--   0        0        0      248 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/const/time.py
--rw-r--r--   0        0        0     3594 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/const/url.py
--rw-r--r--   0        0        0        1 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/db/__init__.py
--rw-r--r--   0        0        0    15609 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/db/operations.py
--rw-r--r--   0        0        0      206 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/db/operations_/helpers.py
--rw-r--r--   0        0        0     8568 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/db/operations_/labels.py
--rw-r--r--   0        0        0    19852 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/db/operations_/media.py
--rw-r--r--   0        0        0    11553 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/db/operations_/merge.py
--rw-r--r--   0        0        0     8494 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/db/operations_/messages.py
--rw-r--r--   0        0        0     8928 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/db/operations_/others.py
--rw-r--r--   0        0        0    10366 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/db/operations_/posts.py
--rw-r--r--   0        0        0     6725 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/db/operations_/profile.py
--rw-r--r--   0        0        0     7485 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/db/operations_/stories.py
--rw-r--r--   0        0        0     4810 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/db/operations_/wrapper.py
--rw-r--r--   0        0        0    10881 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/download/alt_download.py
--rw-r--r--   0        0        0    10682 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/download/alt_downloadbatch.py
--rw-r--r--   0        0        0     2383 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/download/download.py
--rw-r--r--   0        0        0    17191 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/download/downloadbatch.py
--rw-r--r--   0        0        0     9094 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/download/downloadnormal.py
--rw-r--r--   0        0        0    10787 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/download/main_download.py
--rw-r--r--   0        0        0    11235 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/download/main_downloadbatch.py
--rw-r--r--   0        0        0     1414 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/download/shared/classes/retries.py
--rw-r--r--   0        0        0     1356 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/download/shared/classes/session.py
--rw-r--r--   0        0        0     3795 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/download/shared/common/alt_common.py
--rw-r--r--   0        0        0     6372 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/download/shared/common/general.py
--rw-r--r--   0        0        0     2063 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/download/shared/common/main_common.py
--rw-r--r--   0        0        0     2341 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/download/shared/globals.py
--rw-r--r--   0        0        0     9440 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/download/shared/utils/keyhelpers.py
--rw-r--r--   0        0        0     3431 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/download/shared/utils/log.py
--rw-r--r--   0        0        0      317 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/download/shared/utils/media.py
--rw-r--r--   0        0        0      790 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/download/shared/utils/message.py
--rw-r--r--   0        0        0     5698 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/download/shared/utils/metadata.py
--rw-r--r--   0        0        0     2590 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/download/shared/utils/paths.py
--rw-r--r--   0        0        0      453 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/download/shared/utils/progress.py
--rw-r--r--   0        0        0     1155 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/download/shared/utils/text.py
--rw-r--r--   0        0        0     9970 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/filters/media/helpers.py
--rw-r--r--   0        0        0     5335 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/filters/media/main.py
--rw-r--r--   0        0        0     3136 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/filters/models/date.py
--rw-r--r--   0        0        0     3143 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/filters/models/flags.py
--rw-r--r--   0        0        0      957 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/filters/models/helpers.py
--rw-r--r--   0        0        0      726 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/filters/models/other.py
--rw-r--r--   0        0        0     7561 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/filters/models/price.py
--rw-r--r--   0        0        0     1538 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/filters/models/sort.py
--rw-r--r--   0        0        0     1454 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/filters/models/subtype.py
--rw-r--r--   0        0        0     3414 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/models/retriver.py
--rw-r--r--   0        0        0     8105 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/models/selector.py
--rw-r--r--   0        0        0     2466 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/prompts/helpers/model_helpers.py
--rw-r--r--   0        0        0    15219 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/prompts/helpers/prompt_helpers.py
--rw-r--r--   0        0        0      846 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/prompts/keybindings.py
--rw-r--r--   0        0        0     7747 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/prompts/promptConvert.py
--rw-r--r--   0        0        0      917 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/prompts/prompt_groups/actions.py
--rw-r--r--   0        0        0     6834 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/prompts/prompt_groups/area.py
--rw-r--r--   0        0        0     8257 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/prompts/prompt_groups/auth.py
--rw-r--r--   0        0        0     4438 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/prompts/prompt_groups/binary.py
--rw-r--r--   0        0        0    27916 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/prompts/prompt_groups/config.py
--rw-r--r--   0        0        0     1879 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/prompts/prompt_groups/menu.py
--rw-r--r--   0        0        0     3112 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/prompts/prompt_groups/merge.py
--rw-r--r--   0        0        0    16090 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/prompts/prompt_groups/model.py
--rw-r--r--   0        0        0     4135 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/prompts/prompt_groups/profile.py
--rw-r--r--   0        0        0     7609 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/prompts/prompt_strings.py
--rw-r--r--   0        0        0    10346 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/prompts/prompt_validators.py
--rw-r--r--   0        0        0     1342 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/prompts/prompts.py
--rw-r--r--   0        0        0      567 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/runner/exit.py
--rw-r--r--   0        0        0     1578 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/runner/load.py
--rw-r--r--   0        0        0     2743 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/runner/run.py
--rw-r--r--   0        0        0        1 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/utils/__init__.py
--rw-r--r--   0        0        0     3803 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/utils/actions.py
--rw-r--r--   0        0        0     1838 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/utils/args/areas.py
--rw-r--r--   0        0        0     1089 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/utils/args/arguments/advanced_processing.py
--rw-r--r--   0        0        0     1546 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/utils/args/arguments/advanced_program.py
--rw-r--r--   0        0        0     4411 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/utils/args/arguments/advanced_user_filter.py
--rw-r--r--   0        0        0      997 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/utils/args/arguments/automatic.py
--rw-r--r--   0        0        0     5198 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/utils/args/arguments/content.py
--rw-r--r--   0        0        0      944 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/utils/args/arguments/download.py
--rw-r--r--   0        0        0      905 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/utils/args/arguments/file.py
--rw-r--r--   0        0        0     1185 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/utils/args/arguments/logging.py
--rw-r--r--   0        0        0     1282 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/utils/args/arguments/media_type.py
--rw-r--r--   0        0        0      935 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/utils/args/arguments/program.py
--rw-r--r--   0        0        0     3825 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/utils/args/arguments/user_list.py
--rw-r--r--   0        0        0     2683 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/utils/args/arguments/user_select.py
--rw-r--r--   0        0        0      971 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/utils/args/arguments/user_sort.py
--rw-r--r--   0        0        0      319 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/utils/args/bundles/advanced_common.py
--rw-r--r--   0        0        0      661 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/utils/args/bundles/common.py
--rw-r--r--   0        0        0     1020 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/utils/args/bundles/main.py
--rw-r--r--   0        0        0     1579 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/utils/args/bundles/manual.py
--rw-r--r--   0        0        0     2281 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/utils/args/bundles/message_check.py
--rw-r--r--   0        0        0     4145 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/utils/args/bundles/metadata.py
--rw-r--r--   0        0        0     1862 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/args/bundles/paid_check.py
--rw-r--r--   0        0        0     2277 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/args/bundles/post_check.py
--rw-r--r--   0        0        0     1928 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/args/bundles/story_check.py
--rw-r--r--   0        0        0      502 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/args/commands/main.py
--rw-r--r--   0        0        0      189 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/args/commands/manual.py
--rw-r--r--   0        0        0      217 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/args/commands/message.py
--rw-r--r--   0        0        0      197 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/args/commands/metadata.py
--rw-r--r--   0        0        0      205 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/args/commands/paid.py
--rw-r--r--   0        0        0      205 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/args/commands/post.py
--rw-r--r--   0        0        0      209 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/args/commands/story.py
--rw-r--r--   0        0        0       12 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/args/globals.py
--rw-r--r--   0        0        0     5616 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/args/helpers.py
--rw-r--r--   0        0        0     2031 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/args/parse.py
--rw-r--r--   0        0        0      395 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/args/quality.py
--rw-r--r--   0        0        0      960 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/args/read.py
--rw-r--r--   0        0        0      721 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/args/user.py
--rw-r--r--   0        0        0      403 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/args/write.py
--rw-r--r--   0        0        0     2148 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/auth/context.py
--rw-r--r--   0        0        0     1680 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/auth/data.py
--rw-r--r--   0        0        0     2034 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/auth/file.py
--rw-r--r--   0        0        0     2844 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/auth/helpers.py
--rw-r--r--   0        0        0     1669 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/auth/make.py
--rw-r--r--   0        0        0     6704 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/auth/request.py
--rw-r--r--   0        0        0      802 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/auth/schema.py
--rw-r--r--   0        0        0     9824 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/binaries.py
--rw-r--r--   0        0        0     1780 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/cache.py
--rw-r--r--   0        0        0     1612 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/checkers.py
--rw-r--r--   0        0        0     2952 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/config/config.py
--rw-r--r--   0        0        0     1442 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/config/context.py
--rw-r--r--   0        0        0      522 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/config/custom.py
--rw-r--r--   0        0        0    24693 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/config/data.py
--rw-r--r--   0        0        0     2146 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/config/file.py
--rw-r--r--   0        0        0     2073 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/config/menu.py
--rw-r--r--   0        0        0     4797 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/config/schema.py
--rw-r--r--   0        0        0      409 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/config/wrapper.py
--rw-r--r--   0        0        0      499 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/console.py
--rw-r--r--   0        0        0      788 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/constants.py
--rw-r--r--   0        0        0     3401 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/context/exit.py
--rw-r--r--   0        0        0     1135 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/context/run_async.py
--rw-r--r--   0        0        0     1004 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/context/stdout.py
--rw-r--r--   0        0        0     3460 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/dates.py
--rw-r--r--   0        0        0     1040 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/encoding.py
--rw-r--r--   0        0        0     1745 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/hash.py
--rw-r--r--   0        0        0     7226 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/logs/classes.py
--rw-r--r--   0        0        0     2588 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/logs/close.py
--rw-r--r--   0        0        0      477 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/logs/globals.py
--rw-r--r--   0        0        0     1670 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/logs/helpers.py
--rw-r--r--   0        0        0     2098 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/logs/logger.py
--rw-r--r--   0        0        0     1672 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/logs/logs.py
--rw-r--r--   0        0        0     5955 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/logs/other.py
--rw-r--r--   0        0        0     3652 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/logs/stdout.py
--rw-r--r--   0        0        0      601 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/manager.py
--rw-r--r--   0        0        0      576 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/me.py
--rw-r--r--   0        0        0     4167 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/menu.py
--rw-r--r--   0        0        0     1022 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/merge.py
--rw-r--r--   0        0        0     1710 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/paths/check.py
--rw-r--r--   0        0        0     3091 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/paths/common.py
--rw-r--r--   0        0        0      703 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/paths/manage.py
--rw-r--r--   0        0        0     4912 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/paths/paths.py
--rw-r--r--   0        0        0     1034 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/profiles/data.py
--rw-r--r--   0        0        0     2785 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/profiles/manage.py
--rw-r--r--   0        0        0     1583 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/profiles/tools.py
--rw-r--r--   0        0        0    10893 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/progress.py
--rw-r--r--   0        0        0     4406 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/run.py
--rw-r--r--   0        0        0        1 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/sems.py
--rw-r--r--   0        0        0     1672 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/separate.py
--rw-r--r--   0        0        0     4691 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/settings.py
--rw-r--r--   0        0        0      417 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/system/free.py
--rw-r--r--   0        0        0     3279 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/system/network.py
--rw-r--r--   0        0        0     2472 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/system/system.py
--rw-r--r--   0        0        0     2055 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/text.py
--rw-r--r--   0        0        0     2117 2024-05-12 12:52:41.864739 ofscraper-3.9.7/pyproject.toml
--rw-r--r--   0        0        0     6424 1970-01-01 00:00:00.000000 ofscraper-3.9.7/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-13 16:22:17.992203 ofscraper-3.9.8/LICENSE
+-rw-r--r--   0        0        0     4213 2024-05-13 16:22:17.992203 ofscraper-3.9.8/README.md
+-rwxr-xr-x   0        0        0      283 2024-05-13 16:22:18.000203 ofscraper-3.9.8/ofscraper/__main__.py
+-rw-r--r--   0        0        0     1064 2024-05-13 16:22:18.000203 ofscraper-3.9.8/ofscraper/__version__.py
+-rw-r--r--   0        0        0      999 2024-05-13 16:22:18.000203 ofscraper-3.9.8/ofscraper/__version__.pye
+-rw-r--r--   0        0        0    16109 2024-05-13 16:22:18.000203 ofscraper-3.9.8/ofscraper/api/archive.py
+-rw-r--r--   0        0        0      274 2024-05-13 16:22:18.000203 ofscraper-3.9.8/ofscraper/api/common/logs.py
+-rw-r--r--   0        0        0    14697 2024-05-13 16:22:18.000203 ofscraper-3.9.8/ofscraper/api/highlights.py
+-rw-r--r--   0        0        0     1479 2024-05-13 16:22:18.000203 ofscraper-3.9.8/ofscraper/api/init.py
+-rw-r--r--   0        0        0    14238 2024-05-13 16:22:18.000203 ofscraper-3.9.8/ofscraper/api/labels.py
+-rw-r--r--   0        0        0     2912 2024-05-13 16:22:18.000203 ofscraper-3.9.8/ofscraper/api/me.py
+-rw-r--r--   0        0        0    18330 2024-05-13 16:22:18.000203 ofscraper-3.9.8/ofscraper/api/messages.py
+-rw-r--r--   0        0        0    13861 2024-05-13 16:22:18.000203 ofscraper-3.9.8/ofscraper/api/paid.py
+-rw-r--r--   0        0        0     8581 2024-05-13 16:22:18.000203 ofscraper-3.9.8/ofscraper/api/pinned.py
+-rw-r--r--   0        0        0     6176 2024-05-13 16:22:18.000203 ofscraper-3.9.8/ofscraper/api/profile.py
+-rw-r--r--   0        0        0     1718 2024-05-13 16:22:18.000203 ofscraper-3.9.8/ofscraper/api/subscriptions/helpers.py
+-rw-r--r--   0        0        0     3381 2024-05-13 16:22:18.000203 ofscraper-3.9.8/ofscraper/api/subscriptions/individual.py
+-rw-r--r--   0        0        0    12660 2024-05-13 16:22:18.000203 ofscraper-3.9.8/ofscraper/api/subscriptions/lists.py
+-rw-r--r--   0        0        0     8171 2024-05-13 16:22:18.000203 ofscraper-3.9.8/ofscraper/api/subscriptions/subscriptions.py
+-rw-r--r--   0        0        0    17164 2024-05-13 16:22:18.000203 ofscraper-3.9.8/ofscraper/api/timeline.py
+-rw-r--r--   0        0        0     1460 2024-05-13 16:22:18.000203 ofscraper-3.9.8/ofscraper/classes/base.py
+-rw-r--r--   0        0        0      876 2024-05-13 16:22:18.000203 ofscraper-3.9.8/ofscraper/classes/labels.py
+-rw-r--r--   0        0        0    15560 2024-05-13 16:22:18.000203 ofscraper-3.9.8/ofscraper/classes/media.py
+-rw-r--r--   0        0        0     6005 2024-05-13 16:22:18.000203 ofscraper-3.9.8/ofscraper/classes/models.py
+-rw-r--r--   0        0        0     1771 2024-05-13 16:22:18.000203 ofscraper-3.9.8/ofscraper/classes/multiprocessprogress.py
+-rw-r--r--   0        0        0    20835 2024-05-13 16:22:18.000203 ofscraper-3.9.8/ofscraper/classes/placeholder.py
+-rw-r--r--   0        0        0     5156 2024-05-13 16:22:18.000203 ofscraper-3.9.8/ofscraper/classes/posts.py
+-rw-r--r--   0        0        0    18233 2024-05-13 16:22:18.000203 ofscraper-3.9.8/ofscraper/classes/sessionmanager.py
+-rw-r--r--   0        0        0      156 2024-05-13 16:22:18.000203 ofscraper-3.9.8/ofscraper/classes/table/button.py
+-rw-r--r--   0        0        0     1689 2024-05-13 16:22:18.000203 ofscraper-3.9.8/ofscraper/classes/table/fields/boolfield.py
+-rw-r--r--   0        0        0     1370 2024-05-13 16:22:18.000203 ofscraper-3.9.8/ofscraper/classes/table/fields/datefield.py
+-rw-r--r--   0        0        0      629 2024-05-13 16:22:18.000203 ofscraper-3.9.8/ofscraper/classes/table/fields/mediafield.py
+-rw-r--r--   0        0        0      694 2024-05-13 16:22:18.000203 ofscraper-3.9.8/ofscraper/classes/table/fields/numfield.py
+-rw-r--r--   0        0        0     1302 2024-05-13 16:22:18.000203 ofscraper-3.9.8/ofscraper/classes/table/fields/pricefield.py
+-rw-r--r--   0        0        0      678 2024-05-13 16:22:18.000203 ofscraper-3.9.8/ofscraper/classes/table/fields/responsefield.py
+-rw-r--r--   0        0        0     1417 2024-05-13 16:22:18.000203 ofscraper-3.9.8/ofscraper/classes/table/fields/selectfield.py
+-rw-r--r--   0        0        0     1487 2024-05-13 16:22:18.000203 ofscraper-3.9.8/ofscraper/classes/table/fields/textsearch.py
+-rw-r--r--   0        0        0     2460 2024-05-13 16:22:18.000203 ofscraper-3.9.8/ofscraper/classes/table/fields/timefield.py
+-rw-r--r--   0        0        0     1893 2024-05-13 16:22:18.000203 ofscraper-3.9.8/ofscraper/classes/table/inputs/filterinput.py
+-rw-r--r--   0        0        0      117 2024-05-13 16:22:18.000203 ofscraper-3.9.8/ofscraper/classes/table/inputs/intergerinput.py
+-rw-r--r--   0        0        0      113 2024-05-13 16:22:18.000203 ofscraper-3.9.8/ofscraper/classes/table/inputs/strinput.py
+-rw-r--r--   0        0        0      297 2024-05-13 16:22:18.000203 ofscraper-3.9.8/ofscraper/classes/table/row_names.py
+-rw-r--r--   0        0        0     4583 2024-05-13 16:22:18.000203 ofscraper-3.9.8/ofscraper/classes/table/status.py
+-rw-r--r--   0        0        0    21258 2024-05-13 16:22:18.000203 ofscraper-3.9.8/ofscraper/classes/table/table.py
+-rw-r--r--   0        0        0      156 2024-05-13 16:22:18.000203 ofscraper-3.9.8/ofscraper/classes/table/table_console.py
+-rw-r--r--   0        0        0        1 2024-05-13 16:22:18.000203 ofscraper-3.9.8/ofscraper/commands/actions/__init__.py
+-rw-r--r--   0        0        0     6465 2024-05-13 16:22:18.000203 ofscraper-3.9.8/ofscraper/commands/actions/download/download.py
+-rw-r--r--   0        0        0    21884 2024-05-13 16:22:18.000203 ofscraper-3.9.8/ofscraper/commands/actions/download/post.py
+-rw-r--r--   0        0        0    11597 2024-05-13 16:22:18.000203 ofscraper-3.9.8/ofscraper/commands/actions/like.py
+-rw-r--r--   0        0        0     1545 2024-05-13 16:22:18.000203 ofscraper-3.9.8/ofscraper/commands/actions/scrape_context.py
+-rw-r--r--   0        0        0     1039 2024-05-13 16:22:18.000203 ofscraper-3.9.8/ofscraper/commands/add_select/add_selected.py
+-rw-r--r--   0        0        0    26132 2024-05-13 16:22:18.004203 ofscraper-3.9.8/ofscraper/commands/check.py
+-rw-r--r--   0        0        0    11014 2024-05-13 16:22:18.004203 ofscraper-3.9.8/ofscraper/commands/manual.py
+-rw-r--r--   0        0        0     8260 2024-05-13 16:22:18.004203 ofscraper-3.9.8/ofscraper/commands/metadata.py
+-rw-r--r--   0        0        0      556 2024-05-13 16:22:18.004203 ofscraper-3.9.8/ofscraper/commands/picker.py
+-rwxr-xr-x   0        0        0     3785 2024-05-13 16:22:18.004203 ofscraper-3.9.8/ofscraper/commands/scraper.py
+-rw-r--r--   0        0        0       53 2024-05-13 16:22:18.004203 ofscraper-3.9.8/ofscraper/const/binary.py
+-rw-r--r--   0        0        0     1655 2024-05-13 16:22:18.004203 ofscraper-3.9.8/ofscraper/const/config.py
+-rw-r--r--   0        0        0     1002 2024-05-13 16:22:18.004203 ofscraper-3.9.8/ofscraper/const/constants.py
+-rw-r--r--   0        0        0       74 2024-05-13 16:22:18.004203 ofscraper-3.9.8/ofscraper/const/date.py
+-rw-r--r--   0        0        0      190 2024-05-13 16:22:18.004203 ofscraper-3.9.8/ofscraper/const/download.py
+-rw-r--r--   0        0        0      204 2024-05-13 16:22:18.004203 ofscraper-3.9.8/ofscraper/const/files.py
+-rw-r--r--   0        0        0     1375 2024-05-13 16:22:18.004203 ofscraper-3.9.8/ofscraper/const/general.py
+-rw-r--r--   0        0        0       93 2024-05-13 16:22:18.004203 ofscraper-3.9.8/ofscraper/const/logger.py
+-rw-r--r--   0        0        0      120 2024-05-13 16:22:18.004203 ofscraper-3.9.8/ofscraper/const/metadata.py
+-rw-r--r--   0        0        0      862 2024-05-13 16:22:18.004203 ofscraper-3.9.8/ofscraper/const/other_url.py
+-rw-r--r--   0        0        0     1908 2024-05-13 16:22:18.004203 ofscraper-3.9.8/ofscraper/const/prompts.py
+-rw-r--r--   0        0        0     1808 2024-05-13 16:22:18.004203 ofscraper-3.9.8/ofscraper/const/req.py
+-rw-r--r--   0        0        0      271 2024-05-13 16:22:18.004203 ofscraper-3.9.8/ofscraper/const/table.py
+-rw-r--r--   0        0        0   265533 2024-05-13 16:22:18.004203 ofscraper-3.9.8/ofscraper/const/test_constants.py
+-rw-r--r--   0        0        0      248 2024-05-13 16:22:18.004203 ofscraper-3.9.8/ofscraper/const/time.py
+-rw-r--r--   0        0        0     3594 2024-05-13 16:22:18.004203 ofscraper-3.9.8/ofscraper/const/url.py
+-rw-r--r--   0        0        0        1 2024-05-13 16:22:18.004203 ofscraper-3.9.8/ofscraper/db/__init__.py
+-rw-r--r--   0        0        0    15609 2024-05-13 16:22:18.004203 ofscraper-3.9.8/ofscraper/db/operations.py
+-rw-r--r--   0        0        0      206 2024-05-13 16:22:18.004203 ofscraper-3.9.8/ofscraper/db/operations_/helpers.py
+-rw-r--r--   0        0        0     8568 2024-05-13 16:22:18.004203 ofscraper-3.9.8/ofscraper/db/operations_/labels.py
+-rw-r--r--   0        0        0    19696 2024-05-13 16:22:18.004203 ofscraper-3.9.8/ofscraper/db/operations_/media.py
+-rw-r--r--   0        0        0    11553 2024-05-13 16:22:18.004203 ofscraper-3.9.8/ofscraper/db/operations_/merge.py
+-rw-r--r--   0        0        0     8494 2024-05-13 16:22:18.004203 ofscraper-3.9.8/ofscraper/db/operations_/messages.py
+-rw-r--r--   0        0        0     8928 2024-05-13 16:22:18.004203 ofscraper-3.9.8/ofscraper/db/operations_/others.py
+-rw-r--r--   0        0        0    10366 2024-05-13 16:22:18.004203 ofscraper-3.9.8/ofscraper/db/operations_/posts.py
+-rw-r--r--   0        0        0     6725 2024-05-13 16:22:18.004203 ofscraper-3.9.8/ofscraper/db/operations_/profile.py
+-rw-r--r--   0        0        0     7485 2024-05-13 16:22:18.004203 ofscraper-3.9.8/ofscraper/db/operations_/stories.py
+-rw-r--r--   0        0        0     4810 2024-05-13 16:22:18.004203 ofscraper-3.9.8/ofscraper/db/operations_/wrapper.py
+-rw-r--r--   0        0        0    10881 2024-05-13 16:22:18.004203 ofscraper-3.9.8/ofscraper/download/alt_download.py
+-rw-r--r--   0        0        0    10682 2024-05-13 16:22:18.004203 ofscraper-3.9.8/ofscraper/download/alt_downloadbatch.py
+-rw-r--r--   0        0        0     2383 2024-05-13 16:22:18.004203 ofscraper-3.9.8/ofscraper/download/download.py
+-rw-r--r--   0        0        0    17191 2024-05-13 16:22:18.004203 ofscraper-3.9.8/ofscraper/download/downloadbatch.py
+-rw-r--r--   0        0        0     9094 2024-05-13 16:22:18.004203 ofscraper-3.9.8/ofscraper/download/downloadnormal.py
+-rw-r--r--   0        0        0    10787 2024-05-13 16:22:18.004203 ofscraper-3.9.8/ofscraper/download/main_download.py
+-rw-r--r--   0        0        0    11235 2024-05-13 16:22:18.004203 ofscraper-3.9.8/ofscraper/download/main_downloadbatch.py
+-rw-r--r--   0        0        0     1414 2024-05-13 16:22:18.004203 ofscraper-3.9.8/ofscraper/download/shared/classes/retries.py
+-rw-r--r--   0        0        0     1356 2024-05-13 16:22:18.004203 ofscraper-3.9.8/ofscraper/download/shared/classes/session.py
+-rw-r--r--   0        0        0     3852 2024-05-13 16:22:18.004203 ofscraper-3.9.8/ofscraper/download/shared/common/alt_common.py
+-rw-r--r--   0        0        0     6372 2024-05-13 16:22:18.004203 ofscraper-3.9.8/ofscraper/download/shared/common/general.py
+-rw-r--r--   0        0        0     2100 2024-05-13 16:22:18.004203 ofscraper-3.9.8/ofscraper/download/shared/common/main_common.py
+-rw-r--r--   0        0        0     2341 2024-05-13 16:22:18.004203 ofscraper-3.9.8/ofscraper/download/shared/globals.py
+-rw-r--r--   0        0        0     9440 2024-05-13 16:22:18.004203 ofscraper-3.9.8/ofscraper/download/shared/utils/keyhelpers.py
+-rw-r--r--   0        0        0     3431 2024-05-13 16:22:18.004203 ofscraper-3.9.8/ofscraper/download/shared/utils/log.py
+-rw-r--r--   0        0        0      317 2024-05-13 16:22:18.004203 ofscraper-3.9.8/ofscraper/download/shared/utils/media.py
+-rw-r--r--   0        0        0      790 2024-05-13 16:22:18.004203 ofscraper-3.9.8/ofscraper/download/shared/utils/message.py
+-rw-r--r--   0        0        0     6768 2024-05-13 16:22:18.004203 ofscraper-3.9.8/ofscraper/download/shared/utils/metadata.py
+-rw-r--r--   0        0        0     2590 2024-05-13 16:22:18.004203 ofscraper-3.9.8/ofscraper/download/shared/utils/paths.py
+-rw-r--r--   0        0        0      453 2024-05-13 16:22:18.004203 ofscraper-3.9.8/ofscraper/download/shared/utils/progress.py
+-rw-r--r--   0        0        0     1155 2024-05-13 16:22:18.004203 ofscraper-3.9.8/ofscraper/download/shared/utils/text.py
+-rw-r--r--   0        0        0     9971 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/filters/media/helpers.py
+-rw-r--r--   0        0        0     5335 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/filters/media/main.py
+-rw-r--r--   0        0        0     3136 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/filters/models/date.py
+-rw-r--r--   0        0        0     3143 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/filters/models/flags.py
+-rw-r--r--   0        0        0      957 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/filters/models/helpers.py
+-rw-r--r--   0        0        0      726 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/filters/models/other.py
+-rw-r--r--   0        0        0     7561 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/filters/models/price.py
+-rw-r--r--   0        0        0     1538 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/filters/models/sort.py
+-rw-r--r--   0        0        0     1454 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/filters/models/subtype.py
+-rw-r--r--   0        0        0     3414 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/models/retriver.py
+-rw-r--r--   0        0        0     8105 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/models/selector.py
+-rw-r--r--   0        0        0     2466 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/prompts/helpers/model_helpers.py
+-rw-r--r--   0        0        0    15219 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/prompts/helpers/prompt_helpers.py
+-rw-r--r--   0        0        0      846 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/prompts/keybindings.py
+-rw-r--r--   0        0        0     7747 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/prompts/promptConvert.py
+-rw-r--r--   0        0        0      917 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/prompts/prompt_groups/actions.py
+-rw-r--r--   0        0        0     6834 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/prompts/prompt_groups/area.py
+-rw-r--r--   0        0        0     8257 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/prompts/prompt_groups/auth.py
+-rw-r--r--   0        0        0     4438 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/prompts/prompt_groups/binary.py
+-rw-r--r--   0        0        0    27916 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/prompts/prompt_groups/config.py
+-rw-r--r--   0        0        0     1879 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/prompts/prompt_groups/menu.py
+-rw-r--r--   0        0        0     3112 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/prompts/prompt_groups/merge.py
+-rw-r--r--   0        0        0    16090 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/prompts/prompt_groups/model.py
+-rw-r--r--   0        0        0     4135 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/prompts/prompt_groups/profile.py
+-rw-r--r--   0        0        0     7609 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/prompts/prompt_strings.py
+-rw-r--r--   0        0        0    10346 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/prompts/prompt_validators.py
+-rw-r--r--   0        0        0     1342 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/prompts/prompts.py
+-rw-r--r--   0        0        0      567 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/runner/exit.py
+-rw-r--r--   0        0        0     1578 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/runner/load.py
+-rw-r--r--   0        0        0     2743 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/runner/run.py
+-rw-r--r--   0        0        0        1 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/utils/__init__.py
+-rw-r--r--   0        0        0     3803 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/utils/actions.py
+-rw-r--r--   0        0        0     1838 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/utils/args/areas.py
+-rw-r--r--   0        0        0     1089 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/utils/args/arguments/advanced_processing.py
+-rw-r--r--   0        0        0     1546 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/utils/args/arguments/advanced_program.py
+-rw-r--r--   0        0        0     4411 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/utils/args/arguments/advanced_user_filter.py
+-rw-r--r--   0        0        0      997 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/utils/args/arguments/automatic.py
+-rw-r--r--   0        0        0     5218 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/utils/args/arguments/content.py
+-rw-r--r--   0        0        0      944 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/utils/args/arguments/download.py
+-rw-r--r--   0        0        0      905 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/utils/args/arguments/file.py
+-rw-r--r--   0        0        0     1185 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/utils/args/arguments/logging.py
+-rw-r--r--   0        0        0     1282 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/utils/args/arguments/media_type.py
+-rw-r--r--   0        0        0      935 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/utils/args/arguments/program.py
+-rw-r--r--   0        0        0     3825 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/utils/args/arguments/user_list.py
+-rw-r--r--   0        0        0     2683 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/utils/args/arguments/user_select.py
+-rw-r--r--   0        0        0      971 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/utils/args/arguments/user_sort.py
+-rw-r--r--   0        0        0      305 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/utils/args/before.py
+-rw-r--r--   0        0        0      319 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/utils/args/bundles/advanced_common.py
+-rw-r--r--   0        0        0      661 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/utils/args/bundles/common.py
+-rw-r--r--   0        0        0     1020 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/utils/args/bundles/main.py
+-rw-r--r--   0        0        0     1579 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/utils/args/bundles/manual.py
+-rw-r--r--   0        0        0     2281 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/utils/args/bundles/message_check.py
+-rw-r--r--   0        0        0     4145 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/utils/args/bundles/metadata.py
+-rw-r--r--   0        0        0     1862 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/utils/args/bundles/paid_check.py
+-rw-r--r--   0        0        0     2277 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/utils/args/bundles/post_check.py
+-rw-r--r--   0        0        0     1928 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/utils/args/bundles/story_check.py
+-rw-r--r--   0        0        0      515 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/utils/args/commands/main.py
+-rw-r--r--   0        0        0      189 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/utils/args/commands/manual.py
+-rw-r--r--   0        0        0      217 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/utils/args/commands/message.py
+-rw-r--r--   0        0        0      197 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/utils/args/commands/metadata.py
+-rw-r--r--   0        0        0      205 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/utils/args/commands/paid.py
+-rw-r--r--   0        0        0      205 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/utils/args/commands/post.py
+-rw-r--r--   0        0        0      209 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/utils/args/commands/story.py
+-rw-r--r--   0        0        0      471 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/utils/args/date.py
+-rw-r--r--   0        0        0       12 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/utils/args/globals.py
+-rw-r--r--   0        0        0     5660 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/utils/args/helpers.py
+-rw-r--r--   0        0        0     2031 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/utils/args/parse.py
+-rw-r--r--   0        0        0      395 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/utils/args/quality.py
+-rw-r--r--   0        0        0      960 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/utils/args/read.py
+-rw-r--r--   0        0        0      721 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/utils/args/user.py
+-rw-r--r--   0        0        0      403 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/utils/args/write.py
+-rw-r--r--   0        0        0     2148 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/utils/auth/context.py
+-rw-r--r--   0        0        0     1680 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/utils/auth/data.py
+-rw-r--r--   0        0        0     2034 2024-05-13 16:22:18.008203 ofscraper-3.9.8/ofscraper/utils/auth/file.py
+-rw-r--r--   0        0        0     2844 2024-05-13 16:22:18.012203 ofscraper-3.9.8/ofscraper/utils/auth/helpers.py
+-rw-r--r--   0        0        0     1669 2024-05-13 16:22:18.012203 ofscraper-3.9.8/ofscraper/utils/auth/make.py
+-rw-r--r--   0        0        0     6780 2024-05-13 16:22:18.012203 ofscraper-3.9.8/ofscraper/utils/auth/request.py
+-rw-r--r--   0        0        0      802 2024-05-13 16:22:18.012203 ofscraper-3.9.8/ofscraper/utils/auth/schema.py
+-rw-r--r--   0        0        0     9824 2024-05-13 16:22:18.012203 ofscraper-3.9.8/ofscraper/utils/binaries.py
+-rw-r--r--   0        0        0     1780 2024-05-13 16:22:18.012203 ofscraper-3.9.8/ofscraper/utils/cache.py
+-rw-r--r--   0        0        0     1612 2024-05-13 16:22:18.012203 ofscraper-3.9.8/ofscraper/utils/checkers.py
+-rw-r--r--   0        0        0     2952 2024-05-13 16:22:18.012203 ofscraper-3.9.8/ofscraper/utils/config/config.py
+-rw-r--r--   0        0        0     1442 2024-05-13 16:22:18.012203 ofscraper-3.9.8/ofscraper/utils/config/context.py
+-rw-r--r--   0        0        0      522 2024-05-13 16:22:18.012203 ofscraper-3.9.8/ofscraper/utils/config/custom.py
+-rw-r--r--   0        0        0    24693 2024-05-13 16:22:18.012203 ofscraper-3.9.8/ofscraper/utils/config/data.py
+-rw-r--r--   0        0        0     2146 2024-05-13 16:22:18.012203 ofscraper-3.9.8/ofscraper/utils/config/file.py
+-rw-r--r--   0        0        0     2073 2024-05-13 16:22:18.012203 ofscraper-3.9.8/ofscraper/utils/config/menu.py
+-rw-r--r--   0        0        0     4797 2024-05-13 16:22:18.012203 ofscraper-3.9.8/ofscraper/utils/config/schema.py
+-rw-r--r--   0        0        0      409 2024-05-13 16:22:18.012203 ofscraper-3.9.8/ofscraper/utils/config/wrapper.py
+-rw-r--r--   0        0        0      499 2024-05-13 16:22:18.012203 ofscraper-3.9.8/ofscraper/utils/console.py
+-rw-r--r--   0        0        0      788 2024-05-13 16:22:18.012203 ofscraper-3.9.8/ofscraper/utils/constants.py
+-rw-r--r--   0        0        0     3401 2024-05-13 16:22:18.012203 ofscraper-3.9.8/ofscraper/utils/context/exit.py
+-rw-r--r--   0        0        0     1135 2024-05-13 16:22:18.012203 ofscraper-3.9.8/ofscraper/utils/context/run_async.py
+-rw-r--r--   0        0        0     1004 2024-05-13 16:22:18.012203 ofscraper-3.9.8/ofscraper/utils/context/stdout.py
+-rw-r--r--   0        0        0     3460 2024-05-13 16:22:18.012203 ofscraper-3.9.8/ofscraper/utils/dates.py
+-rw-r--r--   0        0        0     1040 2024-05-13 16:22:18.012203 ofscraper-3.9.8/ofscraper/utils/encoding.py
+-rw-r--r--   0        0        0     1700 2024-05-13 16:22:18.012203 ofscraper-3.9.8/ofscraper/utils/hash.py
+-rw-r--r--   0        0        0     7226 2024-05-13 16:22:18.012203 ofscraper-3.9.8/ofscraper/utils/logs/classes.py
+-rw-r--r--   0        0        0     2588 2024-05-13 16:22:18.012203 ofscraper-3.9.8/ofscraper/utils/logs/close.py
+-rw-r--r--   0        0        0      477 2024-05-13 16:22:18.012203 ofscraper-3.9.8/ofscraper/utils/logs/globals.py
+-rw-r--r--   0        0        0     1670 2024-05-13 16:22:18.012203 ofscraper-3.9.8/ofscraper/utils/logs/helpers.py
+-rw-r--r--   0        0        0     2098 2024-05-13 16:22:18.012203 ofscraper-3.9.8/ofscraper/utils/logs/logger.py
+-rw-r--r--   0        0        0     1672 2024-05-13 16:22:18.012203 ofscraper-3.9.8/ofscraper/utils/logs/logs.py
+-rw-r--r--   0        0        0     5955 2024-05-13 16:22:18.012203 ofscraper-3.9.8/ofscraper/utils/logs/other.py
+-rw-r--r--   0        0        0     3652 2024-05-13 16:22:18.012203 ofscraper-3.9.8/ofscraper/utils/logs/stdout.py
+-rw-r--r--   0        0        0      601 2024-05-13 16:22:18.012203 ofscraper-3.9.8/ofscraper/utils/manager.py
+-rw-r--r--   0        0        0      576 2024-05-13 16:22:18.012203 ofscraper-3.9.8/ofscraper/utils/me.py
+-rw-r--r--   0        0        0     4167 2024-05-13 16:22:18.012203 ofscraper-3.9.8/ofscraper/utils/menu.py
+-rw-r--r--   0        0        0     1022 2024-05-13 16:22:18.012203 ofscraper-3.9.8/ofscraper/utils/merge.py
+-rw-r--r--   0        0        0     1710 2024-05-13 16:22:18.012203 ofscraper-3.9.8/ofscraper/utils/paths/check.py
+-rw-r--r--   0        0        0     3091 2024-05-13 16:22:18.012203 ofscraper-3.9.8/ofscraper/utils/paths/common.py
+-rw-r--r--   0        0        0      703 2024-05-13 16:22:18.012203 ofscraper-3.9.8/ofscraper/utils/paths/manage.py
+-rw-r--r--   0        0        0     4912 2024-05-13 16:22:18.012203 ofscraper-3.9.8/ofscraper/utils/paths/paths.py
+-rw-r--r--   0        0        0     1034 2024-05-13 16:22:18.012203 ofscraper-3.9.8/ofscraper/utils/profiles/data.py
+-rw-r--r--   0        0        0     2785 2024-05-13 16:22:18.012203 ofscraper-3.9.8/ofscraper/utils/profiles/manage.py
+-rw-r--r--   0        0        0     1583 2024-05-13 16:22:18.012203 ofscraper-3.9.8/ofscraper/utils/profiles/tools.py
+-rw-r--r--   0        0        0    10893 2024-05-13 16:22:18.012203 ofscraper-3.9.8/ofscraper/utils/progress.py
+-rw-r--r--   0        0        0     4497 2024-05-13 16:22:18.012203 ofscraper-3.9.8/ofscraper/utils/run.py
+-rw-r--r--   0        0        0        1 2024-05-13 16:22:18.012203 ofscraper-3.9.8/ofscraper/utils/sems.py
+-rw-r--r--   0        0        0     1672 2024-05-13 16:22:18.012203 ofscraper-3.9.8/ofscraper/utils/separate.py
+-rw-r--r--   0        0        0     4691 2024-05-13 16:22:18.012203 ofscraper-3.9.8/ofscraper/utils/settings.py
+-rw-r--r--   0        0        0      417 2024-05-13 16:22:18.012203 ofscraper-3.9.8/ofscraper/utils/system/free.py
+-rw-r--r--   0        0        0     3279 2024-05-13 16:22:18.012203 ofscraper-3.9.8/ofscraper/utils/system/network.py
+-rw-r--r--   0        0        0     2472 2024-05-13 16:22:18.012203 ofscraper-3.9.8/ofscraper/utils/system/system.py
+-rw-r--r--   0        0        0     2055 2024-05-13 16:22:18.012203 ofscraper-3.9.8/ofscraper/utils/text.py
+-rw-r--r--   0        0        0     2117 2024-05-13 16:22:44.392354 ofscraper-3.9.8/pyproject.toml
+-rw-r--r--   0        0        0     6424 1970-01-01 00:00:00.000000 ofscraper-3.9.8/PKG-INFO
```

### Comparing `ofscraper-3.9.7/LICENSE` & `ofscraper-3.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/README.md` & `ofscraper-3.9.8/README.md`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/__version__.py` & `ofscraper-3.9.8/ofscraper/__version__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/__version__.pye` & `ofscraper-3.9.8/ofscraper/__version__.pye`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/api/archive.py` & `ofscraper-3.9.8/ofscraper/api/archive.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,17 +250,15 @@
 
 
 async def get_after(model_id, username, forced_after=None):
     if forced_after is not None:
         return forced_after
     elif not settings.get_after_enabled():
         return 0
-    elif read_args.retriveArgs().after == 0:
-        return 0
-    elif read_args.retriveArgs().after:
+    elif read_args.retriveArgs().after!=None:
         return read_args.retriveArgs().after.float_timestamp
 
     elif cache.get(f"{model_id}_full_archived_scrape"):
         log.info(
             "Used --after previously. Scraping all archived posts required to make sure content is not missing"
         )
         return 0
@@ -346,17 +344,17 @@
             if max(map(lambda x: float(x["postedAtPrecise"]), posts)) >= max(
                 required_ids
             ):
                 pass
             elif float(timestamp or 0) >= max(required_ids):
                 pass
             else:
-                log.debug(f"{log_id} Required before {required_ids}")
+                log.debug(f"{log_id} Required before change:  {required_ids}")
                 [required_ids.discard(float(ele["postedAtPrecise"])) for ele in posts]
-                log.debug(f"{log_id} Required after {required_ids}")
+                log.debug(f"{log_id} Required after change: {required_ids}")
 
                 if len(required_ids) > 0:
                     new_tasks.append(
                         asyncio.create_task(
                             scrape_archived_posts(
                                 c,
                                 model_id,
```

### Comparing `ofscraper-3.9.7/ofscraper/api/highlights.py` & `ofscraper-3.9.8/ofscraper/api/highlights.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/api/init.py` & `ofscraper-3.9.8/ofscraper/api/init.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/api/labels.py` & `ofscraper-3.9.8/ofscraper/api/labels.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/api/me.py` & `ofscraper-3.9.8/ofscraper/api/me.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/api/messages.py` & `ofscraper-3.9.8/ofscraper/api/messages.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,14 +135,15 @@
     set_check(responseArray, model_id, after)
     return responseArray
 
 
 def get_filterArray(after, before, oldmessages):
     log.debug(f"[bold]Messages Cache[/bold] {len(oldmessages)} found")
     oldmessages = list(filter(lambda x: x["created_at"] is not None, oldmessages))
+    oldmessages.append({"created_at":before,"post_id":None})
     oldmessages = sorted(
         oldmessages,
         key=lambda x: arrow.get(x["created_at"] or 0),
         reverse=True,
     )
     if after > before:
         return []
@@ -212,16 +213,14 @@
             asyncio.create_task(
                 scrape_messages(
                     c,
                     model_id,
                     job_progress=job_progress,
                     message_id=(
                         splitArrays[0][0].get("post_id")
-                        if len(filteredArray) != len(oldmessages)
-                        else None
                     ),
                     required_ids=set([ele.get("created_at") for ele in splitArrays[0]]),
                 )
             )
         )
         [
             tasks.append(
@@ -414,17 +413,15 @@
 
 
 async def get_after(model_id, username, forced_after=None):
     if forced_after is not None:
         return forced_after
     elif not settings.get_after_enabled():
         return 0
-    elif read_args.retriveArgs().after == 0:
-        return 0
-    elif read_args.retriveArgs().after:
+    elif read_args.retriveArgs().after!=None:
         return read_args.retriveArgs().after.float_timestamp
     elif cache.get(f"{model_id}_scrape_messages"):
         log.debug(
             "Used --after previously. Scraping all messages required to make sure content is not missing"
         )
         return 0
     curr = await get_messages_media(model_id=model_id, username=username)
```

### Comparing `ofscraper-3.9.7/ofscraper/api/paid.py` & `ofscraper-3.9.8/ofscraper/api/paid.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/api/pinned.py` & `ofscraper-3.9.8/ofscraper/api/pinned.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/api/profile.py` & `ofscraper-3.9.8/ofscraper/api/profile.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/api/subscriptions/helpers.py` & `ofscraper-3.9.8/ofscraper/api/subscriptions/helpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/api/subscriptions/individual.py` & `ofscraper-3.9.8/ofscraper/api/subscriptions/individual.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/api/subscriptions/lists.py` & `ofscraper-3.9.8/ofscraper/api/subscriptions/lists.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/api/subscriptions/subscriptions.py` & `ofscraper-3.9.8/ofscraper/api/subscriptions/subscriptions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/api/timeline.py` & `ofscraper-3.9.8/ofscraper/api/timeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,18 +277,16 @@
             log.trace(f"post raw individual {r.json()}")
             return r.json()
 
 
 async def get_after(model_id, username, forced_after=None):
     if forced_after is not None:
         return forced_after
-    elif read_args.retriveArgs().after:
+    elif read_args.retriveArgs().after!=None:
         return read_args.retriveArgs().after.float_timestamp
-    elif read_args.retriveArgs().after == 0:
-        return 0
     elif not settings.get_after_enabled():
         return 0
     elif cache.get(f"{model_id}_full_timeline_scrape"):
         log.info(
             "Used --after previously. Scraping all timeline posts required to make sure content is not missing"
         )
         return 0
@@ -376,17 +374,17 @@
             if min(map(lambda x: float(x["postedAtPrecise"]), posts)) >= max(
                 required_ids
             ):
                 pass
             elif float(timestamp or 0) >= max(required_ids):
                 pass
             else:
-                log.debug(f"{log_id} Required before {required_ids}")
+                log.debug(f"{log_id} Required before change: {required_ids}")
                 [required_ids.discard(float(ele["postedAtPrecise"])) for ele in posts]
-                log.debug(f"{log_id} Required after {required_ids}")
+                log.debug(f"{log_id} Required after change: {required_ids}")
                 if len(required_ids) > 0:
                     new_tasks.append(
                         asyncio.create_task(
                             scrape_timeline_posts(
                                 c,
                                 model_id,
                                 job_progress=job_progress,
```

### Comparing `ofscraper-3.9.7/ofscraper/classes/base.py` & `ofscraper-3.9.8/ofscraper/classes/base.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/classes/labels.py` & `ofscraper-3.9.8/ofscraper/classes/labels.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/classes/media.py` & `ofscraper-3.9.8/ofscraper/classes/media.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/classes/models.py` & `ofscraper-3.9.8/ofscraper/classes/models.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/classes/multiprocessprogress.py` & `ofscraper-3.9.8/ofscraper/classes/multiprocessprogress.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/classes/placeholder.py` & `ofscraper-3.9.8/ofscraper/classes/placeholder.py`

 * *Files 1% similar despite different names*

```diff
@@ -372,14 +372,22 @@
             return pathlib.Path(paths.truncate(self._filepath))
         return self._filepath
 
     @property
     def trunicated_filedir(self):
         return pathlib.Path(paths.truncate(self._filepath)).parent
 
+    @property
+    def size(self):
+        if not self.trunicated_filepath:
+            return
+        elif not self.trunicated_filepath.exists():
+            return
+        else:
+            return self.trunicated_filepath.stat().st_size
 
 class Textholders(basePlaceholder):
     def __init__(self, ele, ext) -> None:
         super().__init__()
         self._filename = None
         self._mediadir = None
         self._metadata = None
```

### Comparing `ofscraper-3.9.7/ofscraper/classes/posts.py` & `ofscraper-3.9.8/ofscraper/classes/posts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/classes/sessionmanager.py` & `ofscraper-3.9.8/ofscraper/classes/sessionmanager.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,29 +109,26 @@
         sleep = self.wait_random(retry_state)
         logging.getLogger("shared").debug(f"sleeping for {sleep} seconds before retry")
         return sleep
 
     def _after_func(self, retry_state) -> None:
         exception = retry_state.outcome.exception()
         if (
-            isinstance(exception, (aiohttp.ClientResponseError, aiohttp.ClientError))
-            and (
-                getattr(exception, "status_code", None)
-                or getattr(exception, "status", None)
-            )
-            == 403
-        ) or (
-            isinstance(exception, httpx.HTTPStatusError)
-            and (
-                getattr(exception.response, "status_code", None)
-                or getattr(exception.response, "status", None)
-            )
-            == 403
-        ):
-            auth_requests.read_request_auth(forced=True)
+                isinstance(exception, (aiohttp.ClientResponseError, aiohttp.ClientError))
+                and
+                    (getattr(exception, "status_code", None) == 403
+                    or getattr(exception, "status", None) == 403)
+            or (
+                isinstance(exception, httpx.HTTPStatusError)
+                and (
+                    getattr(exception.response, "status_code", None)  == 403
+                    or getattr(exception.response, "status", None) == 403
+                )
+            )):
+                auth_requests.read_request_auth(forced=True)
 
 
 class sessionManager:
     def __init__(
         self,
         backend=None,
         connect_timeout=None,
```

### Comparing `ofscraper-3.9.7/ofscraper/classes/table/fields/boolfield.py` & `ofscraper-3.9.8/ofscraper/classes/table/fields/boolfield.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/classes/table/fields/datefield.py` & `ofscraper-3.9.8/ofscraper/classes/table/fields/datefield.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/classes/table/fields/mediafield.py` & `ofscraper-3.9.8/ofscraper/classes/table/fields/mediafield.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/classes/table/fields/numfield.py` & `ofscraper-3.9.8/ofscraper/classes/table/fields/numfield.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/classes/table/fields/pricefield.py` & `ofscraper-3.9.8/ofscraper/classes/table/fields/pricefield.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/classes/table/fields/responsefield.py` & `ofscraper-3.9.8/ofscraper/classes/table/fields/responsefield.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/classes/table/fields/selectfield.py` & `ofscraper-3.9.8/ofscraper/classes/table/fields/selectfield.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/classes/table/fields/textsearch.py` & `ofscraper-3.9.8/ofscraper/classes/table/fields/textsearch.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/classes/table/fields/timefield.py` & `ofscraper-3.9.8/ofscraper/classes/table/fields/timefield.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/classes/table/inputs/filterinput.py` & `ofscraper-3.9.8/ofscraper/classes/table/inputs/filterinput.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/classes/table/status.py` & `ofscraper-3.9.8/ofscraper/classes/table/status.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/classes/table/table.py` & `ofscraper-3.9.8/ofscraper/classes/table/table.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/commands/actions/download/download.py` & `ofscraper-3.9.8/ofscraper/commands/actions/download/download.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/commands/actions/download/post.py` & `ofscraper-3.9.8/ofscraper/commands/actions/download/post.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/commands/actions/like.py` & `ofscraper-3.9.8/ofscraper/commands/actions/like.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/commands/actions/scrape_context.py` & `ofscraper-3.9.8/ofscraper/commands/actions/scrape_context.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/commands/add_select/add_selected.py` & `ofscraper-3.9.8/ofscraper/commands/add_select/add_selected.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/commands/check.py` & `ofscraper-3.9.8/ofscraper/commands/check.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/commands/manual.py` & `ofscraper-3.9.8/ofscraper/commands/manual.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/commands/metadata.py` & `ofscraper-3.9.8/ofscraper/commands/metadata.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/commands/picker.py` & `ofscraper-3.9.8/ofscraper/commands/picker.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/commands/scraper.py` & `ofscraper-3.9.8/ofscraper/commands/scraper.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/const/config.py` & `ofscraper-3.9.8/ofscraper/const/config.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/const/constants.py` & `ofscraper-3.9.8/ofscraper/const/constants.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/const/general.py` & `ofscraper-3.9.8/ofscraper/const/general.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/const/other_url.py` & `ofscraper-3.9.8/ofscraper/const/other_url.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/const/prompts.py` & `ofscraper-3.9.8/ofscraper/const/prompts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/const/req.py` & `ofscraper-3.9.8/ofscraper/const/req.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/const/test_constants.py` & `ofscraper-3.9.8/ofscraper/const/test_constants.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/const/url.py` & `ofscraper-3.9.8/ofscraper/const/url.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/db/operations.py` & `ofscraper-3.9.8/ofscraper/db/operations.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/db/operations_/labels.py` & `ofscraper-3.9.8/ofscraper/db/operations_/labels.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/db/operations_/media.py` & `ofscraper-3.9.8/ofscraper/db/operations_/media.py`

 * *Files 2% similar despite different names*

```diff
@@ -332,15 +332,15 @@
     username=None,
     conn=None,
     filepath=None,
     filename=None,
     directory=None,
     downloaded=None,
     hashdata=None,
-    changed=False,
+    size=None,
     **kwargs,
 ):
     with contextlib.closing(conn.cursor()) as curr:
         filename=filename or (filepath.name if filepath!=None else None)
         directory=directory or (filepath.parent if filepath!=None else None)
         update_media_table_via_api_helper(
             media, curr=curr, model_id=model_id, conn=conn
@@ -351,16 +351,16 @@
             filename=filename,
             directory=directory,
             username=username,
             hashdata=hashdata,
             conn=conn,
             curr=curr,
             downloaded=downloaded,
+            size=size,
         )
-        return curr.rowcount if changed else None
 
 
 @wrapper.operation_wrapper_async
 def write_media_table_via_api_batch(medias, model_id=None, conn=None, **kwargs) -> list:
     with contextlib.closing(conn.cursor()) as curr:
         insertData = list(
             map(
@@ -540,18 +540,17 @@
     model_id,
     filename=None,
     directory=None,
     hashdata=None,
     conn=None,
     downloaded=None,
     curr=None,
+    size=None,
     **kwargs,
 ) -> list:
-    size=pathlib.Path(directory,filename).stat().st_size if directory and filename and pathlib.Path(directory,filename).exists() else None
-
     filename=str(filename) if filename else None
     directory=str(directory) if directory else None
     insertData = [
         directory,
         filename,
         size,
         downloaded,
```

### Comparing `ofscraper-3.9.7/ofscraper/db/operations_/merge.py` & `ofscraper-3.9.8/ofscraper/db/operations_/merge.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/db/operations_/messages.py` & `ofscraper-3.9.8/ofscraper/db/operations_/messages.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/db/operations_/others.py` & `ofscraper-3.9.8/ofscraper/db/operations_/others.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/db/operations_/posts.py` & `ofscraper-3.9.8/ofscraper/db/operations_/posts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/db/operations_/profile.py` & `ofscraper-3.9.8/ofscraper/db/operations_/profile.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/db/operations_/stories.py` & `ofscraper-3.9.8/ofscraper/db/operations_/stories.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/db/operations_/wrapper.py` & `ofscraper-3.9.8/ofscraper/db/operations_/wrapper.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/download/alt_download.py` & `ofscraper-3.9.8/ofscraper/download/alt_download.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/download/alt_downloadbatch.py` & `ofscraper-3.9.8/ofscraper/download/alt_downloadbatch.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/download/download.py` & `ofscraper-3.9.8/ofscraper/download/download.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/download/downloadbatch.py` & `ofscraper-3.9.8/ofscraper/download/downloadbatch.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/download/downloadnormal.py` & `ofscraper-3.9.8/ofscraper/download/downloadnormal.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/download/main_download.py` & `ofscraper-3.9.8/ofscraper/download/main_download.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/download/main_downloadbatch.py` & `ofscraper-3.9.8/ofscraper/download/main_downloadbatch.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/download/shared/classes/retries.py` & `ofscraper-3.9.8/ofscraper/download/shared/classes/retries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/download/shared/classes/session.py` & `ofscraper-3.9.8/ofscraper/download/shared/classes/session.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/download/shared/common/alt_common.py` & `ofscraper-3.9.8/ofscraper/download/shared/common/alt_common.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,14 +75,16 @@
             filepath=sharedPlaceholderObj.trunicated_filepath,
             model_id=model_id,
             username=username,
             downloaded=True,
             hashdata=await common.get_hash(
                 sharedPlaceholderObj, mediatype=ele.mediatype
             ),
+            size=sharedPlaceholderObj.size
+            ,
         )
     common.add_additional_data(sharedPlaceholderObj, ele)
     return ele.mediatype, video["total"] + audio["total"]
 
 
 async def media_item_post_process_alt(audio, video, ele, username, model_id):
     if (audio["total"] + video["total"]) == 0:
```

### Comparing `ofscraper-3.9.7/ofscraper/download/shared/common/general.py` & `ofscraper-3.9.8/ofscraper/download/shared/common/general.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/download/shared/common/main_common.py` & `ofscraper-3.9.8/ofscraper/download/shared/common/main_common.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,12 +41,13 @@
         await download_media_update(
             ele,
             filepath=path_to_file,
             model_id=model_id,
             username=username,
             downloaded=True,
             hashdata=await common.get_hash(path_to_file, mediatype=ele.mediatype),
+            size=placeholderObj.size
         )
     await common.set_profile_cache_helper(ele)
     common.add_additional_data(placeholderObj, ele)
 
     return ele.mediatype, total
```

### Comparing `ofscraper-3.9.7/ofscraper/download/shared/globals.py` & `ofscraper-3.9.8/ofscraper/download/shared/globals.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/download/shared/utils/keyhelpers.py` & `ofscraper-3.9.8/ofscraper/download/shared/utils/keyhelpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/download/shared/utils/log.py` & `ofscraper-3.9.8/ofscraper/download/shared/utils/log.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/download/shared/utils/message.py` & `ofscraper-3.9.8/ofscraper/download/shared/utils/message.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/download/shared/utils/metadata.py` & `ofscraper-3.9.8/ofscraper/download/shared/utils/metadata.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 import ofscraper.download.shared.globals as common_globals
 import ofscraper.download.shared.utils.media as media
 import ofscraper.utils.args.read as read_args
 import ofscraper.utils.cache as cache
 import ofscraper.utils.constants as constants
 from ofscraper.db.operations_.media import download_media_update,prev_download_media_data
 from ofscraper.download.shared.utils.log import get_medialog
+import ofscraper.utils.hash as hash
+
 
 
 async def force_download(ele, username, model_id):
     await download_media_update(
         ele,
         filepath=None,
         model_id=model_id,
@@ -29,25 +31,25 @@
     )
     placeholderObj = placeholderObj or await placeholderObjHelper(c, ele)
     await placeholderObj.init()
     common.add_additional_data(placeholderObj, ele)
     effected = None
     if ele.id:
         prevData=await prev_download_media_data(ele,model_id=model_id,username=username) or {}
-        effected = await download_media_update(
+        await download_media_update(
             ele,
             filename=metadata_file_helper(placeholderObj,prevData),
             directory=metadata_dir_helper(placeholderObj,prevData),
             model_id=model_id,
             username=username,
             downloaded=metadata_downloaded_helper(placeholderObj,prevData),
-            hashdata=prevData.get("hash"),
-            changed=True,
+            hashdata=metadata_hash_helper(placeholderObj,prevData,ele),
+            size=metadata_size_helper(placeholderObj,prevData),
         )
-
+        effected=prevData!=await prev_download_media_data(ele,model_id=model_id,username=username)
     return (
         (ele.mediatype if effected else "forced_skipped"),
         0,
     )
 
 
 def metadata_downloaded_helper(placeholderObj,prevData):
@@ -82,14 +84,30 @@
     elif pathlib.Path(placeholderObj.trunicated_filedir).exists():
         return str(placeholderObj.trunicated_filedir)
     elif pathlib.Path(prevData.get("directory") or "").is_dir():
         return prevData.get("directory")
     elif pathlib.Path(prevData.get("directory") or "",prevData.get("filename") or "").is_file():
         return  pathlib.Path(prevData.get("directory") or "",prevData.get("filename") or "").parent
     return str(placeholderObj.trunicated_filedir)
+
+
+def metadata_hash_helper(placeholderObj,prevData,ele):
+    if not read_args.retriveArgs().get_hash:
+        return prevData.get("hash")
+    elif pathlib.Path(placeholderObj.trunicated_filepath).is_file():
+        return hash.get_hash(pathlib.Path(placeholderObj.trunicated_filepath), mediatype=ele.mediatype)
+    elif pathlib.Path(prevData.get("directory") or "",prevData.get("filename") or "").is_file():
+        return hash.get_hash(pathlib.Path(prevData.get("directory") or "",prevData.get("filename") or ""))
+def metadata_size_helper(placeholderObj,prevData):
+    if placeholderObj.size:
+        return placeholderObj.size
+    elif pathlib.Path(prevData.get("directory") or "",prevData.get("filename") or "").is_file():
+        return pathlib.Path(prevData.get("directory") or "",prevData.get("filename") or "").stat().st_size
+    else:
+        return prevData.get("size")
 async def metadata_helper(c, ele):
     placeholderObj = None
     if not ele.url and not ele.mpd:
         placeholderObj = placeholder.Placeholders(
             ele, ext=media.content_type_missing(ele)
         )
         return placeholderObj
```

### Comparing `ofscraper-3.9.7/ofscraper/download/shared/utils/paths.py` & `ofscraper-3.9.8/ofscraper/download/shared/utils/paths.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/download/shared/utils/text.py` & `ofscraper-3.9.8/ofscraper/download/shared/utils/text.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/filters/media/helpers.py` & `ofscraper-3.9.8/ofscraper/filters/media/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,15 +208,15 @@
         return sorted(media, key=lambda x: x.text, reverse=True)
     elif item_sort == "filename-asc":
         return sorted(media, key=lambda x: x.filename)
     elif item_sort == "filename-desc":
         return sorted(media, key=lambda x: x.filename, reverse=True)
 def previous_download_filter(medialist,username=None,model_id=None):
     log = logging.getLogger("shared")
-    log.info("reading database to retrive previous download")
+    log.info("reading database to retrive previous downloads")
     medialist = seperate.seperate_by_self(medialist)
     if read_args.retriveArgs().force_all:
         log.info("forcing all media to be downloaded")
     elif read_args.retriveArgs().force_model_unique:
         log.info("Downloading unique media for model")
         media_ids = set(
             get_media_ids_downloaded_model(model_id=model_id, username=username)
```

### Comparing `ofscraper-3.9.7/ofscraper/filters/media/main.py` & `ofscraper-3.9.8/ofscraper/filters/media/main.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/filters/models/date.py` & `ofscraper-3.9.8/ofscraper/filters/models/date.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/filters/models/flags.py` & `ofscraper-3.9.8/ofscraper/filters/models/flags.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/filters/models/helpers.py` & `ofscraper-3.9.8/ofscraper/filters/models/helpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/filters/models/other.py` & `ofscraper-3.9.8/ofscraper/filters/models/other.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/filters/models/price.py` & `ofscraper-3.9.8/ofscraper/filters/models/price.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/filters/models/sort.py` & `ofscraper-3.9.8/ofscraper/filters/models/sort.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/filters/models/subtype.py` & `ofscraper-3.9.8/ofscraper/filters/models/subtype.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/models/retriver.py` & `ofscraper-3.9.8/ofscraper/models/retriver.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/models/selector.py` & `ofscraper-3.9.8/ofscraper/models/selector.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/prompts/helpers/model_helpers.py` & `ofscraper-3.9.8/ofscraper/prompts/helpers/model_helpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/prompts/helpers/prompt_helpers.py` & `ofscraper-3.9.8/ofscraper/prompts/helpers/prompt_helpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/prompts/keybindings.py` & `ofscraper-3.9.8/ofscraper/prompts/keybindings.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/prompts/promptConvert.py` & `ofscraper-3.9.8/ofscraper/prompts/promptConvert.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/prompts/prompt_groups/actions.py` & `ofscraper-3.9.8/ofscraper/prompts/prompt_groups/actions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/prompts/prompt_groups/area.py` & `ofscraper-3.9.8/ofscraper/prompts/prompt_groups/area.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/prompts/prompt_groups/auth.py` & `ofscraper-3.9.8/ofscraper/prompts/prompt_groups/auth.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/prompts/prompt_groups/binary.py` & `ofscraper-3.9.8/ofscraper/prompts/prompt_groups/binary.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/prompts/prompt_groups/config.py` & `ofscraper-3.9.8/ofscraper/prompts/prompt_groups/config.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/prompts/prompt_groups/menu.py` & `ofscraper-3.9.8/ofscraper/prompts/prompt_groups/menu.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/prompts/prompt_groups/merge.py` & `ofscraper-3.9.8/ofscraper/prompts/prompt_groups/merge.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/prompts/prompt_groups/model.py` & `ofscraper-3.9.8/ofscraper/prompts/prompt_groups/model.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/prompts/prompt_groups/profile.py` & `ofscraper-3.9.8/ofscraper/prompts/prompt_groups/profile.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/prompts/prompt_strings.py` & `ofscraper-3.9.8/ofscraper/prompts/prompt_strings.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/prompts/prompt_validators.py` & `ofscraper-3.9.8/ofscraper/prompts/prompt_validators.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/prompts/prompts.py` & `ofscraper-3.9.8/ofscraper/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/runner/exit.py` & `ofscraper-3.9.8/ofscraper/runner/exit.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/runner/load.py` & `ofscraper-3.9.8/ofscraper/runner/load.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/runner/run.py` & `ofscraper-3.9.8/ofscraper/runner/run.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/actions.py` & `ofscraper-3.9.8/ofscraper/utils/actions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/args/areas.py` & `ofscraper-3.9.8/ofscraper/utils/args/areas.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/args/arguments/advanced_processing.py` & `ofscraper-3.9.8/ofscraper/utils/args/arguments/advanced_processing.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/args/arguments/advanced_program.py` & `ofscraper-3.9.8/ofscraper/utils/args/arguments/advanced_program.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/args/arguments/advanced_user_filter.py` & `ofscraper-3.9.8/ofscraper/utils/args/arguments/advanced_user_filter.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/args/arguments/automatic.py` & `ofscraper-3.9.8/ofscraper/utils/args/arguments/automatic.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/args/arguments/content.py` & `ofscraper-3.9.8/ofscraper/utils/args/arguments/content.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import itertools
-
-import arrow
 import cloup as click
 
 import ofscraper.utils.args.helpers as helpers
+import ofscraper.utils.args.date as date_helper
+
 
 # Define individual options
 posts_option = click.option(
     "-o",
     "--posts",
     "--post",
     "posts",
@@ -147,19 +147,17 @@
     multiple=True,
 )
 before_option = click.option(
     "-be",
     "--before",
     help="Process posts at or before the given date (MM/DD/YYYY) for likes, unlikes, and downloads",
     type=helpers.arrow_helper,
-    callback=lambda ctx, param, value: value
-    or arrow.get(arrow.now().float_timestamp + 10000),
+    callback=lambda ctx, param, value: date_helper.before_callback(ctx, param, value)
 )
 
-
 after_option = click.option(
     "-af",
     "--after",
     help="Process posts at or after the given date (MM/DD/YYYY) for likes, unlikes, and downloads",
     type=helpers.arrow_helper,
 )
```

### Comparing `ofscraper-3.9.7/ofscraper/utils/args/arguments/download.py` & `ofscraper-3.9.8/ofscraper/utils/args/arguments/download.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/args/arguments/file.py` & `ofscraper-3.9.8/ofscraper/utils/args/arguments/file.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/args/arguments/logging.py` & `ofscraper-3.9.8/ofscraper/utils/args/arguments/logging.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/args/arguments/media_type.py` & `ofscraper-3.9.8/ofscraper/utils/args/arguments/media_type.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/args/arguments/program.py` & `ofscraper-3.9.8/ofscraper/utils/args/arguments/program.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/args/arguments/user_list.py` & `ofscraper-3.9.8/ofscraper/utils/args/arguments/user_list.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/args/arguments/user_select.py` & `ofscraper-3.9.8/ofscraper/utils/args/arguments/user_select.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/args/arguments/user_sort.py` & `ofscraper-3.9.8/ofscraper/utils/args/arguments/user_sort.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/args/bundles/common.py` & `ofscraper-3.9.8/ofscraper/utils/args/bundles/common.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/args/bundles/main.py` & `ofscraper-3.9.8/ofscraper/utils/args/bundles/main.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/args/bundles/manual.py` & `ofscraper-3.9.8/ofscraper/utils/args/bundles/manual.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/args/bundles/message_check.py` & `ofscraper-3.9.8/ofscraper/utils/args/bundles/message_check.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/args/bundles/metadata.py` & `ofscraper-3.9.8/ofscraper/utils/args/bundles/metadata.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/args/bundles/paid_check.py` & `ofscraper-3.9.8/ofscraper/utils/args/bundles/paid_check.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/args/bundles/post_check.py` & `ofscraper-3.9.8/ofscraper/utils/args/bundles/post_check.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/args/bundles/story_check.py` & `ofscraper-3.9.8/ofscraper/utils/args/bundles/story_check.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/args/helpers.py` & `ofscraper-3.9.8/ofscraper/utils/args/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,8 +177,10 @@
             x = re.sub("\\bday\\b", "days", x)
             x = re.sub("\\bmonth\\b", "months", x)
             x = re.sub("\\bweek\\b", "weeks", x)
             arw = arrow.utcnow()
             t = arw.dehumanize(x)
         except ValueError as E:
             raise E
-    return t if t > arrow.get("2006.6.30") else 0
+    if not t:
+        return None
+    return t if t > arrow.get("2006.6.30") else arrow.get(0)
```

### Comparing `ofscraper-3.9.7/ofscraper/utils/args/parse.py` & `ofscraper-3.9.8/ofscraper/utils/args/parse.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/args/read.py` & `ofscraper-3.9.8/ofscraper/utils/args/read.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/args/user.py` & `ofscraper-3.9.8/ofscraper/utils/args/user.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/auth/context.py` & `ofscraper-3.9.8/ofscraper/utils/auth/context.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/auth/data.py` & `ofscraper-3.9.8/ofscraper/utils/auth/data.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/auth/file.py` & `ofscraper-3.9.8/ofscraper/utils/auth/file.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/auth/helpers.py` & `ofscraper-3.9.8/ofscraper/utils/auth/helpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/auth/make.py` & `ofscraper-3.9.8/ofscraper/utils/auth/make.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/auth/request.py` & `ofscraper-3.9.8/ofscraper/utils/auth/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
                                                                                       
 """
 
 import hashlib
 import json
 import time
 from urllib.parse import urlparse
+import logging
 
 import ofscraper.classes.sessionmanager as sessionManager
 import ofscraper.utils.auth.file as auth_file
 import ofscraper.utils.cache as cache
 import ofscraper.utils.constants as constants
 import ofscraper.utils.settings as settings
 
@@ -40,15 +41,16 @@
     request_auth.update(zip(request_auth.keys(), values))
     return request_auth
 
 
 def get_request_auth(forced=False):
     if not forced and cache.get("api_onlyfans_sign"):
         return cache.get("api_onlyfans_sign")
-    elif (settings.get_dynamic_rules()) in {
+    logging.getLogger("shared").debug("getting new signature")
+    if (settings.get_dynamic_rules()) in {
         "deviint",
         "dv",
         "dev",
     }:
 
         return get_request_auth_deviint(forced=forced)
     elif (settings.get_dynamic_rules()) in {
```

### Comparing `ofscraper-3.9.7/ofscraper/utils/auth/schema.py` & `ofscraper-3.9.8/ofscraper/utils/auth/schema.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/binaries.py` & `ofscraper-3.9.8/ofscraper/utils/binaries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/cache.py` & `ofscraper-3.9.8/ofscraper/utils/cache.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/checkers.py` & `ofscraper-3.9.8/ofscraper/utils/checkers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/config/config.py` & `ofscraper-3.9.8/ofscraper/utils/config/config.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/config/context.py` & `ofscraper-3.9.8/ofscraper/utils/config/context.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/config/custom.py` & `ofscraper-3.9.8/ofscraper/utils/config/custom.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/config/data.py` & `ofscraper-3.9.8/ofscraper/utils/config/data.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/config/file.py` & `ofscraper-3.9.8/ofscraper/utils/config/file.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/config/menu.py` & `ofscraper-3.9.8/ofscraper/utils/config/menu.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/config/schema.py` & `ofscraper-3.9.8/ofscraper/utils/config/schema.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/constants.py` & `ofscraper-3.9.8/ofscraper/utils/constants.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/context/exit.py` & `ofscraper-3.9.8/ofscraper/utils/context/exit.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/context/run_async.py` & `ofscraper-3.9.8/ofscraper/utils/context/run_async.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/context/stdout.py` & `ofscraper-3.9.8/ofscraper/utils/context/stdout.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/dates.py` & `ofscraper-3.9.8/ofscraper/utils/dates.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/encoding.py` & `ofscraper-3.9.8/ofscraper/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/hash.py` & `ofscraper-3.9.8/ofscraper/utils/hash.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import io
 import logging
 import pathlib
 
 import xxhash
 
 import ofscraper.classes.placeholder as placeholder
-import ofscraper.db.operations as operations
 import ofscraper.utils.config.data as config_data
 import ofscraper.utils.constants as constants
 from ofscraper.db.operations_.media import get_dupe_media_files, get_dupe_media_hashes
 
 log = logging.getLogger("shared")
```

### Comparing `ofscraper-3.9.7/ofscraper/utils/logs/classes.py` & `ofscraper-3.9.8/ofscraper/utils/logs/classes.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/logs/close.py` & `ofscraper-3.9.8/ofscraper/utils/logs/close.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/logs/helpers.py` & `ofscraper-3.9.8/ofscraper/utils/logs/helpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/logs/logger.py` & `ofscraper-3.9.8/ofscraper/utils/logs/logger.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/logs/logs.py` & `ofscraper-3.9.8/ofscraper/utils/logs/logs.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/logs/other.py` & `ofscraper-3.9.8/ofscraper/utils/logs/other.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/logs/stdout.py` & `ofscraper-3.9.8/ofscraper/utils/logs/stdout.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/manager.py` & `ofscraper-3.9.8/ofscraper/utils/manager.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/me.py` & `ofscraper-3.9.8/ofscraper/utils/me.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/menu.py` & `ofscraper-3.9.8/ofscraper/utils/menu.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/merge.py` & `ofscraper-3.9.8/ofscraper/utils/merge.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/paths/check.py` & `ofscraper-3.9.8/ofscraper/utils/paths/check.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/paths/common.py` & `ofscraper-3.9.8/ofscraper/utils/paths/common.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/paths/manage.py` & `ofscraper-3.9.8/ofscraper/utils/paths/manage.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/paths/paths.py` & `ofscraper-3.9.8/ofscraper/utils/paths/paths.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/profiles/data.py` & `ofscraper-3.9.8/ofscraper/utils/profiles/data.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/profiles/manage.py` & `ofscraper-3.9.8/ofscraper/utils/profiles/manage.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/profiles/tools.py` & `ofscraper-3.9.8/ofscraper/utils/profiles/tools.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/progress.py` & `ofscraper-3.9.8/ofscraper/utils/progress.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/run.py` & `ofscraper-3.9.8/ofscraper/utils/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 import ofscraper.utils.actions as actions
 import ofscraper.utils.args.read as read_args
 import ofscraper.utils.checkers as checkers
 import ofscraper.utils.context.exit as exit
 import ofscraper.utils.dates as dates
 import ofscraper.utils.logs.logs as logs
 import ofscraper.utils.logs.other as other_logger
+import ofscraper.utils.args.date as before_arg
+
 
 log = logging.getLogger("shared")
 
 
 # Adds a function to the job queue
 def set_schedule(*functs):
     sleep = min(max(read_args.retriveArgs().daemon / 5, 1), 60)
@@ -45,14 +47,15 @@
             time.sleep(sleep)
 
 
 def schedule_helper(*functs):
     jobqueue.put(other_logger.updateOtherLoggerStream)
     jobqueue.put(logs.printStartValues)
     jobqueue.put(partial(userselector.getselected_usernames, rescan=True))
+    jobqueue.put(before_arg.update_before)
     for funct in functs:
         jobqueue.put(funct)
     return schedule.CancelJob
 
 
 def daemon_run_helper(*functs):
     checkers.check_auth()
```

### Comparing `ofscraper-3.9.7/ofscraper/utils/separate.py` & `ofscraper-3.9.8/ofscraper/utils/separate.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/settings.py` & `ofscraper-3.9.8/ofscraper/utils/settings.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/system/network.py` & `ofscraper-3.9.8/ofscraper/utils/system/network.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/system/system.py` & `ofscraper-3.9.8/ofscraper/utils/system/system.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/ofscraper/utils/text.py` & `ofscraper-3.9.8/ofscraper/utils/text.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.7/pyproject.toml` & `ofscraper-3.9.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ofscraper"
-version = "3.9.7"
+version = "3.9.8"
 description = "automatically scrape onlyfans"
 authors = ["datawhores <datawhores@riseup.net>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.14"
```

### Comparing `ofscraper-3.9.7/PKG-INFO` & `ofscraper-3.9.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofscraper
-Version: 3.9.7
+Version: 3.9.8
 Summary: automatically scrape onlyfans
 Author: datawhores
 Author-email: datawhores@riseup.net
 Requires-Python: >=3.11,<3.14
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ofscraper Version: 3.9.7 Summary: automatically
+Metadata-Version: 2.1 Name: ofscraper Version: 3.9.8 Summary: automatically
 scrape onlyfans Author: datawhores Author-email: datawhores@riseup.net
 Requires-Python: >=3.11,<3.14 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Provides-Extra: pyinstaller Requires-Dist: aiofiles
 (>=23.2.1,<24.0.0) Requires-Dist: aiohttp (==3.9.4) Requires-Dist:
 aioprocessing (>=2.0.1,<3.0.0) Requires-Dist: aiosqlite (>=0.20.0,<0.21.0)
 Requires-Dist: arrow (>=1.3.0,<2.0.0) Requires-Dist: browser-cookie3 (==0.19.1)
```

