# Comparing `tmp/xklb-2.8.7.tar.gz` & `tmp/xklb-2.8.9.tar.gz`

## Comparing `xklb-2.8.7.tar` & `xklb-2.8.9.tar`

### file list

```diff
@@ -1,138 +1,138 @@
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 xklb-2.8.7/.gitattributes
--rw-r--r--   0        0        0   216245 2020-02-02 00:00:00.000000 xklb-2.8.7/pdm.lock
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-2.8.7/.github/FUNDING.yml
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-2.8.7/.github/LICENSE
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 xklb-2.8.7/.github/Windows.md
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 xklb-2.8.7/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 xklb-2.8.7/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 xklb-2.8.7/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0    10282 2020-02-02 00:00:00.000000 xklb-2.8.7/.github/examples/art.avif
--rw-r--r--   0        0        0    17854 2020-02-02 00:00:00.000000 xklb-2.8.7/.github/examples/extract.svg
--rw-r--r--   0        0        0    13463 2020-02-02 00:00:00.000000 xklb-2.8.7/.github/examples/tubeadd.svg
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 xklb-2.8.7/.github/workflows/green.yaml
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 xklb-2.8.7/.github/workflows/push.yaml
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/__init__.py
--rw-r--r--   0        0        0    14406 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/lb.py
--rw-r--r--   0        0        0    10626 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/media_printer.py
--rw-r--r--   0        0        0    13906 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/readme.py
--rw-r--r--   0        0        0   112540 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/usage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/createdb/__init__.py
--rw-r--r--   0        0        0     9170 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/createdb/av.py
--rw-r--r--   0        0        0    20579 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/createdb/fs_add.py
--rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/createdb/gallery_add.py
--rw-r--r--   0        0        0     8084 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/createdb/gallery_backend.py
--rw-r--r--   0        0        0     5550 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/createdb/hn_add.py
--rw-r--r--   0        0        0     9895 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/createdb/links_add.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/createdb/places_import.py
--rw-r--r--   0        0        0    13142 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/createdb/reddit_add.py
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/createdb/row_add.py
--rw-r--r--   0        0        0    10026 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/createdb/site_add.py
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/createdb/substack.py
--rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/createdb/subtitle.py
--rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/createdb/tabs_add.py
--rw-r--r--   0        0        0     5622 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/createdb/tildes.py
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/createdb/tube_add.py
--rw-r--r--   0        0        0    20249 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/createdb/tube_backend.py
--rw-r--r--   0        0        0     9874 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/createdb/web_add.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/data/__init__.py
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/data/imagemagick_errors.py
--rw-r--r--   0        0        0    17080 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/data/wordbank.py
--rw-r--r--   0        0        0     7149 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/data/yt_dlp_errors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/editdb/__init__.py
--rw-r--r--   0        0        0     4037 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/editdb/dedupe_db.py
--rw-r--r--   0        0        0    18995 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/editdb/dedupe_media.py
--rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/editdb/merge_online_local.py
--rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/editdb/mpv_watchlater.py
--rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/editdb/pushshift.py
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/editdb/reddit_selftext.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/files/__init__.py
--rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/files/christen.py
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/files/sample_compare.py
--rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/files/sample_hash.py
--rw-r--r--   0        0        0     5471 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/files/similar_files.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/folders/__init__.py
--rw-r--r--   0        0        0     7831 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/folders/big_dirs.py
--rw-r--r--   0        0        0     7830 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/folders/merge_folders.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/folders/mount_stats.py
--rw-r--r--   0        0        0     7285 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/folders/move_list.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/folders/rel_mv.py
--rw-r--r--   0        0        0    11782 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/folders/scatter.py
--rw-r--r--   0        0        0     8123 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/folders/similar_folders.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/fsdb/__init__.py
--rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/fsdb/disk_usage.py
--rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/fsdb/search_db.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/mediadb/__init__.py
--rw-r--r--   0        0        0    11549 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/mediadb/block.py
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/mediadb/db_history.py
--rw-r--r--   0        0        0    19259 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/mediadb/db_media.py
--rw-r--r--   0        0        0     8179 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/mediadb/db_playlists.py
--rw-r--r--   0        0        0     7273 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/mediadb/download.py
--rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/mediadb/download_status.py
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/mediadb/history.py
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/mediadb/history_add.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/mediadb/optimize_db.py
--rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/mediadb/playlists.py
--rw-r--r--   0        0        0     5460 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/mediadb/redownload.py
--rw-r--r--   0        0        0     4466 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/mediadb/search.py
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/mediadb/stats.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/mediafiles/__init__.py
--rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/mediafiles/media_check.py
--rw-r--r--   0        0        0     8738 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/mediafiles/process_ffmpeg.py
--rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/mediafiles/process_image.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/misc/__init__.py
--rw-r--r--   0        0        0    13877 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/misc/dedupe_czkawka.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/misc/export_text.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/multidb/__init__.py
--rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/multidb/copy_play_counts.py
--rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/multidb/merge_dbs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/playback/__init__.py
--rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/playback/links_open.py
--rw-r--r--   0        0        0    24252 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/playback/media_player.py
--rw-r--r--   0        0        0    11690 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/playback/play_actions.py
--rw-r--r--   0        0        0     9829 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/playback/playback_control.py
--rw-r--r--   0        0        0     7151 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/playback/post_actions.py
--rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/playback/surf.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/playback/tabs_open.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/scratch/__init__.py
--rw-r--r--   0        0        0     6176 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/scratch/javguru.py
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/scratch/javtiful.py
--rw-r--r--   0        0        0     8683 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/scratch/mam_search.py
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/scratch/mam_slots.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/tablefiles/__init__.py
--rw-r--r--   0        0        0     7343 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/tablefiles/eda.py
--rw-r--r--   0        0        0     4380 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/tablefiles/incremental_diff.py
--rw-r--r--   0        0        0     8163 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/tablefiles/mcda.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/text/__init__.py
--rw-r--r--   0        0        0    12694 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/text/cluster_sort.py
--rw-r--r--   0        0        0     5938 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/text/extract_links.py
--rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/text/extract_text.py
--rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/text/markdown_links.py
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/text/nouns.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/utils/__init__.py
--rw-r--r--   0        0        0     8377 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/utils/arg_utils.py
--rw-r--r--   0        0        0    29978 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/utils/arggroups.py
--rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/utils/argparse_utils.py
--rw-r--r--   0        0        0    10871 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/utils/consts.py
--rw-r--r--   0        0        0     9522 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/utils/db_utils.py
--rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/utils/devices.py
--rw-r--r--   0        0        0    15831 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/utils/file_utils.py
--rw-r--r--   0        0        0     6236 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/utils/gui.py
--rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/utils/iterables.py
--rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/utils/log_utils.py
--rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/utils/mpv_utils.py
--rw-r--r--   0        0        0     4619 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/utils/nums.py
--rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/utils/objects.py
--rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/utils/path_utils.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/utils/pd_utils.py
--rw-r--r--   0        0        0     7716 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/utils/printing.py
--rw-r--r--   0        0        0     7156 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/utils/processes.py
--rw-r--r--   0        0        0    12988 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/utils/sql_utils.py
--rw-r--r--   0        0        0    15807 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/utils/sqlgroups.py
--rw-r--r--   0        0        0     7018 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/utils/strings.py
--rw-r--r--   0        0        0    23222 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/utils/web.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/assets/__init__.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/assets/kotobago.png
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 xklb-2.8.7/.gitignore
--rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 xklb-2.8.7/pyproject.toml
--rw-r--r--   0        0        0   156256 2020-02-02 00:00:00.000000 xklb-2.8.7/.github/README.md
--rw-r--r--   0        0        0   160037 2020-02-02 00:00:00.000000 xklb-2.8.7/PKG-INFO
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 xklb-2.8.9/.gitattributes
+-rw-r--r--   0        0        0   216245 2020-02-02 00:00:00.000000 xklb-2.8.9/pdm.lock
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-2.8.9/.github/FUNDING.yml
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-2.8.9/.github/LICENSE
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 xklb-2.8.9/.github/Windows.md
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 xklb-2.8.9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 xklb-2.8.9/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 xklb-2.8.9/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0    10282 2020-02-02 00:00:00.000000 xklb-2.8.9/.github/examples/art.avif
+-rw-r--r--   0        0        0    17854 2020-02-02 00:00:00.000000 xklb-2.8.9/.github/examples/extract.svg
+-rw-r--r--   0        0        0    13463 2020-02-02 00:00:00.000000 xklb-2.8.9/.github/examples/tubeadd.svg
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 xklb-2.8.9/.github/workflows/green.yaml
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 xklb-2.8.9/.github/workflows/push.yaml
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/__init__.py
+-rw-r--r--   0        0        0    14406 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/lb.py
+-rw-r--r--   0        0        0    10689 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/media_printer.py
+-rw-r--r--   0        0        0    13906 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/readme.py
+-rw-r--r--   0        0        0   112540 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/usage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/createdb/__init__.py
+-rw-r--r--   0        0        0     9170 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/createdb/av.py
+-rw-r--r--   0        0        0    20579 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/createdb/fs_add.py
+-rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/createdb/gallery_add.py
+-rw-r--r--   0        0        0     8084 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/createdb/gallery_backend.py
+-rw-r--r--   0        0        0     5550 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/createdb/hn_add.py
+-rw-r--r--   0        0        0     9833 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/createdb/links_add.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/createdb/places_import.py
+-rw-r--r--   0        0        0    13142 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/createdb/reddit_add.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/createdb/row_add.py
+-rw-r--r--   0        0        0    10026 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/createdb/site_add.py
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/createdb/substack.py
+-rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/createdb/subtitle.py
+-rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/createdb/tabs_add.py
+-rw-r--r--   0        0        0     5622 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/createdb/tildes.py
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/createdb/tube_add.py
+-rw-r--r--   0        0        0    20214 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/createdb/tube_backend.py
+-rw-r--r--   0        0        0     9757 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/createdb/web_add.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/data/__init__.py
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/data/imagemagick_errors.py
+-rw-r--r--   0        0        0    17080 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/data/wordbank.py
+-rw-r--r--   0        0        0     7105 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/data/yt_dlp_errors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/editdb/__init__.py
+-rw-r--r--   0        0        0     4037 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/editdb/dedupe_db.py
+-rw-r--r--   0        0        0    18995 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/editdb/dedupe_media.py
+-rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/editdb/merge_online_local.py
+-rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/editdb/mpv_watchlater.py
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/editdb/pushshift.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/editdb/reddit_selftext.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/files/__init__.py
+-rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/files/christen.py
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/files/sample_compare.py
+-rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/files/sample_hash.py
+-rw-r--r--   0        0        0     5471 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/files/similar_files.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/folders/__init__.py
+-rw-r--r--   0        0        0     7831 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/folders/big_dirs.py
+-rw-r--r--   0        0        0     7830 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/folders/merge_folders.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/folders/mount_stats.py
+-rw-r--r--   0        0        0     7285 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/folders/move_list.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/folders/rel_mv.py
+-rw-r--r--   0        0        0    11782 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/folders/scatter.py
+-rw-r--r--   0        0        0     8123 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/folders/similar_folders.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/fsdb/__init__.py
+-rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/fsdb/disk_usage.py
+-rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/fsdb/search_db.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/mediadb/__init__.py
+-rw-r--r--   0        0        0    11549 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/mediadb/block.py
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/mediadb/db_history.py
+-rw-r--r--   0        0        0    19259 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/mediadb/db_media.py
+-rw-r--r--   0        0        0     8179 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/mediadb/db_playlists.py
+-rw-r--r--   0        0        0     7273 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/mediadb/download.py
+-rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/mediadb/download_status.py
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/mediadb/history.py
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/mediadb/history_add.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/mediadb/optimize_db.py
+-rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/mediadb/playlists.py
+-rw-r--r--   0        0        0     5460 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/mediadb/redownload.py
+-rw-r--r--   0        0        0     4466 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/mediadb/search.py
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/mediadb/stats.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/mediafiles/__init__.py
+-rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/mediafiles/media_check.py
+-rw-r--r--   0        0        0     8738 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/mediafiles/process_ffmpeg.py
+-rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/mediafiles/process_image.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/misc/__init__.py
+-rw-r--r--   0        0        0    13877 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/misc/dedupe_czkawka.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/misc/export_text.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/multidb/__init__.py
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/multidb/copy_play_counts.py
+-rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/multidb/merge_dbs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/playback/__init__.py
+-rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/playback/links_open.py
+-rw-r--r--   0        0        0    24252 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/playback/media_player.py
+-rw-r--r--   0        0        0    11690 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/playback/play_actions.py
+-rw-r--r--   0        0        0     9829 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/playback/playback_control.py
+-rw-r--r--   0        0        0     7151 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/playback/post_actions.py
+-rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/playback/surf.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/playback/tabs_open.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/scratch/__init__.py
+-rw-r--r--   0        0        0     6176 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/scratch/javguru.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/scratch/javtiful.py
+-rw-r--r--   0        0        0     8683 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/scratch/mam_search.py
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/scratch/mam_slots.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/tablefiles/__init__.py
+-rw-r--r--   0        0        0     7343 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/tablefiles/eda.py
+-rw-r--r--   0        0        0     4380 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/tablefiles/incremental_diff.py
+-rw-r--r--   0        0        0     8163 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/tablefiles/mcda.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/text/__init__.py
+-rw-r--r--   0        0        0    12694 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/text/cluster_sort.py
+-rw-r--r--   0        0        0     5821 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/text/extract_links.py
+-rw-r--r--   0        0        0     3498 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/text/extract_text.py
+-rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/text/markdown_links.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/text/nouns.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/utils/__init__.py
+-rw-r--r--   0        0        0     8377 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/utils/arg_utils.py
+-rw-r--r--   0        0        0    30079 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/utils/arggroups.py
+-rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/utils/argparse_utils.py
+-rw-r--r--   0        0        0    10871 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/utils/consts.py
+-rw-r--r--   0        0        0     9522 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/utils/db_utils.py
+-rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/utils/devices.py
+-rw-r--r--   0        0        0    15831 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/utils/file_utils.py
+-rw-r--r--   0        0        0     6236 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/utils/gui.py
+-rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/utils/iterables.py
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/utils/log_utils.py
+-rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/utils/mpv_utils.py
+-rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/utils/nums.py
+-rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/utils/objects.py
+-rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/utils/path_utils.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/utils/pd_utils.py
+-rw-r--r--   0        0        0     7716 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/utils/printing.py
+-rw-r--r--   0        0        0     7156 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/utils/processes.py
+-rw-r--r--   0        0        0    12988 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/utils/sql_utils.py
+-rw-r--r--   0        0        0    15895 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/utils/sqlgroups.py
+-rw-r--r--   0        0        0     7018 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/utils/strings.py
+-rw-r--r--   0        0        0    23222 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/utils/web.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/assets/__init__.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-2.8.9/xklb/assets/kotobago.png
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 xklb-2.8.9/.gitignore
+-rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 xklb-2.8.9/pyproject.toml
+-rw-r--r--   0        0        0   156256 2020-02-02 00:00:00.000000 xklb-2.8.9/.github/README.md
+-rw-r--r--   0        0        0   160037 2020-02-02 00:00:00.000000 xklb-2.8.9/PKG-INFO
```

### Comparing `xklb-2.8.7/pdm.lock` & `xklb-2.8.9/pdm.lock`

 * *Files 2% similar despite different names*

```diff
@@ -130,20 +130,20 @@
 files = [
     {file = "attrs-23.2.0-py3-none-any.whl", hash = "sha256:99b87a485a5820b23b879f04c2305b44b951b502fd64be915879d77a7e8fc6f1"},
     {file = "attrs-23.2.0.tar.gz", hash = "sha256:935dc3b529c262f6cf76e50877d35a4bd3c1de194fd41f47a2b7ae8f19971f30"},
 ]
 
 [[package]]
 name = "babelfish"
-version = "0.6.0"
-requires_python = ">=3.6,<4.0"
+version = "0.6.1"
+requires_python = "<4.0,>=3.8"
 summary = "A module to work with countries and languages"
 files = [
-    {file = "babelfish-0.6.0-py3-none-any.whl", hash = "sha256:268f1c6279f2a04a66837972e8a9f3dcc68e16f1201eec57d2a4b828a8b41b11"},
-    {file = "babelfish-0.6.0.tar.gz", hash = "sha256:2dadfadd1b205ca5fa5dc9fa637f5b7933160a0418684c7c46a7a664033208a2"},
+    {file = "babelfish-0.6.1-py3-none-any.whl", hash = "sha256:512f1501d4c8f7d38f0921f48660be7542de1a7b24abb6a6a65324a670150293"},
+    {file = "babelfish-0.6.1.tar.gz", hash = "sha256:decb67a4660888d48480ab6998309837174158d0f1aa63bebb1c2e11aab97aab"},
 ]
 
 [[package]]
 name = "beautifulsoup4"
 version = "4.12.3"
 requires_python = ">=3.6.0"
 summary = "Screen-scraping library"
@@ -1906,65 +1906,65 @@
 files = [
     {file = "rebulk-3.2.0-py3-none-any.whl", hash = "sha256:6bc31ae4b37200623c5827d2f539f9ec3e52b50431322dad8154642a39b0a53e"},
     {file = "rebulk-3.2.0.tar.gz", hash = "sha256:0d30bf80fca00fa9c697185ac475daac9bde5f646ce3338c9ff5d5dc1ebdfebc"},
 ]
 
 [[package]]
 name = "regex"
-version = "2024.4.28"
+version = "2024.5.10"
 requires_python = ">=3.8"
 summary = "Alternative regular expression module, to replace re."
 files = [
-    {file = "regex-2024.4.28-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:cd196d056b40af073d95a2879678585f0b74ad35190fac04ca67954c582c6b61"},
-    {file = "regex-2024.4.28-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:8bb381f777351bd534462f63e1c6afb10a7caa9fa2a421ae22c26e796fe31b1f"},
-    {file = "regex-2024.4.28-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:47af45b6153522733aa6e92543938e97a70ce0900649ba626cf5aad290b737b6"},
-    {file = "regex-2024.4.28-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:99d6a550425cc51c656331af0e2b1651e90eaaa23fb4acde577cf15068e2e20f"},
-    {file = "regex-2024.4.28-cp310-cp310-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:bf29304a8011feb58913c382902fde3395957a47645bf848eea695839aa101b7"},
-    {file = "regex-2024.4.28-cp310-cp310-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:92da587eee39a52c91aebea8b850e4e4f095fe5928d415cb7ed656b3460ae79a"},
-    {file = "regex-2024.4.28-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:6277d426e2f31bdbacb377d17a7475e32b2d7d1f02faaecc48d8e370c6a3ff31"},
-    {file = "regex-2024.4.28-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:28e1f28d07220c0f3da0e8fcd5a115bbb53f8b55cecf9bec0c946eb9a059a94c"},
-    {file = "regex-2024.4.28-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:aaa179975a64790c1f2701ac562b5eeb733946eeb036b5bcca05c8d928a62f10"},
-    {file = "regex-2024.4.28-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:6f435946b7bf7a1b438b4e6b149b947c837cb23c704e780c19ba3e6855dbbdd3"},
-    {file = "regex-2024.4.28-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:19d6c11bf35a6ad077eb23852827f91c804eeb71ecb85db4ee1386825b9dc4db"},
-    {file = "regex-2024.4.28-cp310-cp310-musllinux_1_1_ppc64le.whl", hash = "sha256:fdae0120cddc839eb8e3c15faa8ad541cc6d906d3eb24d82fb041cfe2807bc1e"},
-    {file = "regex-2024.4.28-cp310-cp310-musllinux_1_1_s390x.whl", hash = "sha256:e672cf9caaf669053121f1766d659a8813bd547edef6e009205378faf45c67b8"},
-    {file = "regex-2024.4.28-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:f57515750d07e14743db55d59759893fdb21d2668f39e549a7d6cad5d70f9fea"},
-    {file = "regex-2024.4.28-cp310-cp310-win32.whl", hash = "sha256:a1409c4eccb6981c7baabc8888d3550df518add6e06fe74fa1d9312c1838652d"},
-    {file = "regex-2024.4.28-cp310-cp310-win_amd64.whl", hash = "sha256:1f687a28640f763f23f8a9801fe9e1b37338bb1ca5d564ddd41619458f1f22d1"},
-    {file = "regex-2024.4.28-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:84077821c85f222362b72fdc44f7a3a13587a013a45cf14534df1cbbdc9a6796"},
-    {file = "regex-2024.4.28-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:b45d4503de8f4f3dc02f1d28a9b039e5504a02cc18906cfe744c11def942e9eb"},
-    {file = "regex-2024.4.28-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:457c2cd5a646dd4ed536c92b535d73548fb8e216ebee602aa9f48e068fc393f3"},
-    {file = "regex-2024.4.28-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:2b51739ddfd013c6f657b55a508de8b9ea78b56d22b236052c3a85a675102dc6"},
-    {file = "regex-2024.4.28-cp311-cp311-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:459226445c7d7454981c4c0ce0ad1a72e1e751c3e417f305722bbcee6697e06a"},
-    {file = "regex-2024.4.28-cp311-cp311-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:670fa596984b08a4a769491cbdf22350431970d0112e03d7e4eeaecaafcd0fec"},
-    {file = "regex-2024.4.28-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:fe00f4fe11c8a521b173e6324d862ee7ee3412bf7107570c9b564fe1119b56fb"},
-    {file = "regex-2024.4.28-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:36f392dc7763fe7924575475736bddf9ab9f7a66b920932d0ea50c2ded2f5636"},
-    {file = "regex-2024.4.28-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:23a412b7b1a7063f81a742463f38821097b6a37ce1e5b89dd8e871d14dbfd86b"},
-    {file = "regex-2024.4.28-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:f1d6e4b7b2ae3a6a9df53efbf199e4bfcff0959dbdb5fd9ced34d4407348e39a"},
-    {file = "regex-2024.4.28-cp311-cp311-musllinux_1_1_ppc64le.whl", hash = "sha256:499334ad139557de97cbc4347ee921c0e2b5e9c0f009859e74f3f77918339257"},
-    {file = "regex-2024.4.28-cp311-cp311-musllinux_1_1_s390x.whl", hash = "sha256:0940038bec2fe9e26b203d636c44d31dd8766abc1fe66262da6484bd82461ccf"},
-    {file = "regex-2024.4.28-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:66372c2a01782c5fe8e04bff4a2a0121a9897e19223d9eab30c54c50b2ebeb7f"},
-    {file = "regex-2024.4.28-cp311-cp311-win32.whl", hash = "sha256:c77d10ec3c1cf328b2f501ca32583625987ea0f23a0c2a49b37a39ee5c4c4630"},
-    {file = "regex-2024.4.28-cp311-cp311-win_amd64.whl", hash = "sha256:fc0916c4295c64d6890a46e02d4482bb5ccf33bf1a824c0eaa9e83b148291f90"},
-    {file = "regex-2024.4.28-cp312-cp312-macosx_10_9_universal2.whl", hash = "sha256:08a1749f04fee2811c7617fdd46d2e46d09106fa8f475c884b65c01326eb15c5"},
-    {file = "regex-2024.4.28-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:b8eb28995771c087a73338f695a08c9abfdf723d185e57b97f6175c5051ff1ae"},
-    {file = "regex-2024.4.28-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:dd7ef715ccb8040954d44cfeff17e6b8e9f79c8019daae2fd30a8806ef5435c0"},
-    {file = "regex-2024.4.28-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:fb0315a2b26fde4005a7c401707c5352df274460f2f85b209cf6024271373013"},
-    {file = "regex-2024.4.28-cp312-cp312-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:f2fc053228a6bd3a17a9b0a3f15c3ab3cf95727b00557e92e1cfe094b88cc662"},
-    {file = "regex-2024.4.28-cp312-cp312-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:7fe9739a686dc44733d52d6e4f7b9c77b285e49edf8570754b322bca6b85b4cc"},
-    {file = "regex-2024.4.28-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:a74fcf77d979364f9b69fcf8200849ca29a374973dc193a7317698aa37d8b01c"},
-    {file = "regex-2024.4.28-cp312-cp312-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:965fd0cf4694d76f6564896b422724ec7b959ef927a7cb187fc6b3f4e4f59833"},
-    {file = "regex-2024.4.28-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:2fef0b38c34ae675fcbb1b5db760d40c3fc3612cfa186e9e50df5782cac02bcd"},
-    {file = "regex-2024.4.28-cp312-cp312-musllinux_1_1_i686.whl", hash = "sha256:bc365ce25f6c7c5ed70e4bc674f9137f52b7dd6a125037f9132a7be52b8a252f"},
-    {file = "regex-2024.4.28-cp312-cp312-musllinux_1_1_ppc64le.whl", hash = "sha256:ac69b394764bb857429b031d29d9604842bc4cbfd964d764b1af1868eeebc4f0"},
-    {file = "regex-2024.4.28-cp312-cp312-musllinux_1_1_s390x.whl", hash = "sha256:144a1fc54765f5c5c36d6d4b073299832aa1ec6a746a6452c3ee7b46b3d3b11d"},
-    {file = "regex-2024.4.28-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:2630ca4e152c221072fd4a56d4622b5ada876f668ecd24d5ab62544ae6793ed6"},
-    {file = "regex-2024.4.28-cp312-cp312-win32.whl", hash = "sha256:7f3502f03b4da52bbe8ba962621daa846f38489cae5c4a7b5d738f15f6443d17"},
-    {file = "regex-2024.4.28-cp312-cp312-win_amd64.whl", hash = "sha256:0dd3f69098511e71880fb00f5815db9ed0ef62c05775395968299cb400aeab82"},
-    {file = "regex-2024.4.28.tar.gz", hash = "sha256:83ab366777ea45d58f72593adf35d36ca911ea8bd838483c1823b883a121b0e4"},
+    {file = "regex-2024.5.10-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:eda3dd46df535da787ffb9036b5140f941ecb91701717df91c9daf64cabef953"},
+    {file = "regex-2024.5.10-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:1d5bd666466c8f00a06886ce1397ba8b12371c1f1c6d1bef11013e9e0a1464a8"},
+    {file = "regex-2024.5.10-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:32e5f3b8e32918bfbdd12eca62e49ab3031125c454b507127ad6ecbd86e62fca"},
+    {file = "regex-2024.5.10-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:534efd2653ebc4f26fc0e47234e53bf0cb4715bb61f98c64d2774a278b58c846"},
+    {file = "regex-2024.5.10-cp310-cp310-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:193b7c6834a06f722f0ce1ba685efe80881de7c3de31415513862f601097648c"},
+    {file = "regex-2024.5.10-cp310-cp310-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:160ba087232c5c6e2a1e7ad08bd3a3f49b58c815be0504d8c8aacfb064491cd8"},
+    {file = "regex-2024.5.10-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:951be1eae7b47660412dc4938777a975ebc41936d64e28081bf2e584b47ec246"},
+    {file = "regex-2024.5.10-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:d8a0f0ab5453e409586b11ebe91c672040bc804ca98d03a656825f7890cbdf88"},
+    {file = "regex-2024.5.10-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:9e6d4d6ae1827b2f8c7200aaf7501c37cf3f3896c86a6aaf2566448397c823dd"},
+    {file = "regex-2024.5.10-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:161a206c8f3511e2f5fafc9142a2cc25d7fe9a1ec5ad9b4ad2496a7c33e1c5d2"},
+    {file = "regex-2024.5.10-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:44b3267cea873684af022822195298501568ed44d542f9a2d9bebc0212e99069"},
+    {file = "regex-2024.5.10-cp310-cp310-musllinux_1_1_ppc64le.whl", hash = "sha256:560278c9975694e1f0bc50da187abf2cdc1e4890739ea33df2bc4a85eeef143e"},
+    {file = "regex-2024.5.10-cp310-cp310-musllinux_1_1_s390x.whl", hash = "sha256:70364a097437dd0a90b31cd77f09f7387ad9ac60ef57590971f43b7fca3082a5"},
+    {file = "regex-2024.5.10-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:42be5de7cc8c1edac55db92d82b68dc8e683b204d6f5414c5a51997a323d7081"},
+    {file = "regex-2024.5.10-cp310-cp310-win32.whl", hash = "sha256:9a8625849387b9d558d528e263ecc9c0fbde86cfa5c2f0eef43fff480ae24d71"},
+    {file = "regex-2024.5.10-cp310-cp310-win_amd64.whl", hash = "sha256:903350bf44d7e4116b4d5898b30b15755d61dcd3161e3413a49c7db76f0bee5a"},
+    {file = "regex-2024.5.10-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:bf9596cba92ce7b1fd32c7b07c6e3212c7eed0edc271757e48bfcd2b54646452"},
+    {file = "regex-2024.5.10-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:45cc13d398b6359a7708986386f72bd156ae781c3e83a68a6d4cee5af04b1ce9"},
+    {file = "regex-2024.5.10-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:ad45f3bccfcb00868f2871dce02a755529838d2b86163ab8a246115e80cfb7d6"},
+    {file = "regex-2024.5.10-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:33d19f0cde6838c81acffff25c7708e4adc7dd02896c9ec25c3939b1500a1778"},
+    {file = "regex-2024.5.10-cp311-cp311-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:0a9f89d7db5ef6bdf53e5cc8e6199a493d0f1374b3171796b464a74ebe8e508a"},
+    {file = "regex-2024.5.10-cp311-cp311-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:8c6c71cf92b09e5faa72ea2c68aa1f61c9ce11cb66fdc5069d712f4392ddfd00"},
+    {file = "regex-2024.5.10-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:7467ad8b0eac0b28e52679e972b9b234b3de0ea5cee12eb50091d2b68145fe36"},
+    {file = "regex-2024.5.10-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:bc0db93ad039fc2fe32ccd3dd0e0e70c4f3d6e37ae83f0a487e1aba939bd2fbd"},
+    {file = "regex-2024.5.10-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:fa9335674d7c819674467c7b46154196c51efbaf5f5715187fd366814ba3fa39"},
+    {file = "regex-2024.5.10-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:7dda3091838206969c2b286f9832dff41e2da545b99d1cfaea9ebd8584d02708"},
+    {file = "regex-2024.5.10-cp311-cp311-musllinux_1_1_ppc64le.whl", hash = "sha256:504b5116e2bd1821efd815941edff7535e93372a098e156bb9dffde30264e798"},
+    {file = "regex-2024.5.10-cp311-cp311-musllinux_1_1_s390x.whl", hash = "sha256:91b53dea84415e8115506cc62e441a2b54537359c63d856d73cb1abe05af4c9a"},
+    {file = "regex-2024.5.10-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:1a3903128f9e17a500618e80c68165c78c741ebb17dd1a0b44575f92c3c68b02"},
+    {file = "regex-2024.5.10-cp311-cp311-win32.whl", hash = "sha256:236cace6c1903effd647ed46ce6dd5d76d54985fc36dafc5256032886736c85d"},
+    {file = "regex-2024.5.10-cp311-cp311-win_amd64.whl", hash = "sha256:12446827f43c7881decf2c126762e11425de5eb93b3b0d8b581344c16db7047a"},
+    {file = "regex-2024.5.10-cp312-cp312-macosx_10_9_universal2.whl", hash = "sha256:14905ed75c7a6edf423eb46c213ed3f4507c38115f1ed3c00f4ec9eafba50e58"},
+    {file = "regex-2024.5.10-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:4fad420b14ae1970a1f322e8ae84a1d9d89375eb71e1b504060ab2d1bfe68f3c"},
+    {file = "regex-2024.5.10-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:c46a76a599fcbf95f98755275c5527304cc4f1bb69919434c1e15544d7052910"},
+    {file = "regex-2024.5.10-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:0faecb6d5779753a6066a3c7a0471a8d29fe25d9981ca9e552d6d1b8f8b6a594"},
+    {file = "regex-2024.5.10-cp312-cp312-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:aab65121229c2ecdf4a31b793d99a6a0501225bd39b616e653c87b219ed34a49"},
+    {file = "regex-2024.5.10-cp312-cp312-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:50e7e96a527488334379e05755b210b7da4a60fc5d6481938c1fa053e0c92184"},
+    {file = "regex-2024.5.10-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:ba034c8db4b264ef1601eb33cd23d87c5013b8fb48b8161debe2e5d3bd9156b0"},
+    {file = "regex-2024.5.10-cp312-cp312-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:031219782d97550c2098d9a68ce9e9eaefe67d2d81d8ff84c8354f9c009e720c"},
+    {file = "regex-2024.5.10-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:62b5f7910b639f3c1d122d408421317c351e213ca39c964ad4121f27916631c6"},
+    {file = "regex-2024.5.10-cp312-cp312-musllinux_1_1_i686.whl", hash = "sha256:cd832bd9b6120d6074f39bdfbb3c80e416848b07ac72910f1c7f03131a6debc3"},
+    {file = "regex-2024.5.10-cp312-cp312-musllinux_1_1_ppc64le.whl", hash = "sha256:e91b1976358e17197157b405cab408a5f4e33310cda211c49fc6da7cffd0b2f0"},
+    {file = "regex-2024.5.10-cp312-cp312-musllinux_1_1_s390x.whl", hash = "sha256:571452362d552de508c37191b6abbbb660028b8b418e2d68c20779e0bc8eaaa8"},
+    {file = "regex-2024.5.10-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:5253dcb0bfda7214523de58b002eb0090cb530d7c55993ce5f6d17faf953ece7"},
+    {file = "regex-2024.5.10-cp312-cp312-win32.whl", hash = "sha256:2f30a5ab8902f93930dc6f627c4dd5da2703333287081c85cace0fc6e21c25af"},
+    {file = "regex-2024.5.10-cp312-cp312-win_amd64.whl", hash = "sha256:3799e36d60a35162bb35b2246d8bb012192b7437dff807ef79c14e7352706306"},
+    {file = "regex-2024.5.10.tar.gz", hash = "sha256:304e7e2418146ae4d0ef0e9ffa28f881f7874b45b4994cc2279b21b6e7ae50c8"},
 ]
 
 [[package]]
 name = "requests"
 version = "2.31.0"
 requires_python = ">=3.7"
 summary = "Python HTTP for Humans."
```

### Comparing `xklb-2.8.7/.github/LICENSE` & `xklb-2.8.9/.github/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/.github/Windows.md` & `xklb-2.8.9/.github/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/.github/examples/art.avif` & `xklb-2.8.9/.github/examples/art.avif`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/.github/examples/extract.svg` & `xklb-2.8.9/.github/examples/extract.svg`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/.github/examples/tubeadd.svg` & `xklb-2.8.9/.github/examples/tubeadd.svg`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/.github/workflows/push.yaml` & `xklb-2.8.9/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/lb.py` & `xklb-2.8.9/xklb/lb.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/media_printer.py` & `xklb-2.8.9/xklb/media_printer.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from copy import deepcopy
 from io import StringIO
 from numbers import Number
 from pathlib import Path
 
 from xklb.mediadb import db_history, db_media
 from xklb.playback import post_actions
-from xklb.utils import consts, db_utils, iterables, printing, processes, sql_utils, strings
+from xklb.utils import consts, db_utils, iterables, nums, printing, processes, sql_utils, strings
 from xklb.utils.consts import SC
 from xklb.utils.log_utils import log
 
 
 def filter_deleted(media):
     http_list = []
     local_list = []
@@ -112,48 +112,48 @@
         media.reverse()
 
     try:
         tables = args.db.table_names()
     except AttributeError:
         tables = []
 
-    duration = sum(m.get("duration") or 0 for m in media)
+    total_duration = sum(m.get("duration") or 0 for m in media)
     if "a" in print_args and ("Aggregate" not in media[0].get("path") or ""):
         if "count" in media[0]:
             D = {"path": "Aggregate", "count": sum(d.get("count") or 0 for d in media)}
         elif "exists" in media[0]:
             D = {"path": "Aggregate", "count": sum(d.get("exists") or 0 for d in media)}
         elif action == SC.download_status and "never_downloaded" in media[0]:
             potential_downloads = sum(d["never_downloaded"] + d["retry_queued"] for d in media)
             D = {"path": "Aggregate", "count": potential_downloads}
         else:
             D = {"path": "Aggregate", "count": len(media)}
 
         if "duration" in media[0] and action not in (SC.download_status):
-            D["duration"] = duration
-            D["avg_duration"] = duration / len(media)
+            D["duration"] = total_duration
+            D["avg_duration"] = nums.safe_mean(m.get("duration") for m in media)
 
         if hasattr(args, "action") and "history" in tables:
             if action in (SC.download, SC.download_status) and "time_downloaded" in m_columns:
                 D["download_duration"] = cadence_adjusted_items(args, D["count"], time_column="time_downloaded")
             else:
-                if duration > 0:
-                    D["cadence_adj_duration"] = cadence_adjusted_duration(args, duration)
+                if total_duration > 0:
+                    D["cadence_adj_duration"] = cadence_adjusted_duration(args, total_duration)
                 else:
                     D["cadence_adj_duration"] = cadence_adjusted_items(args, D["count"])
 
         if "size" in media[0]:
             D["size"] = sum((d.get("size") or 0) for d in media)
-            D["avg_size"] = sum((d.get("size") or 0) for d in media) / len(media)
+            D["avg_size"] = nums.safe_mean(d.get("size") for d in media)
 
         if cols:
             for c in cols:
                 if isinstance(media[0][c], Number):
                     D[f"sum_{c}"] = sum((d[c] or 0) for d in media)
-                    D[f"avg_{c}"] = sum((d[c] or 0) for d in media) / len(media)
+                    D[f"avg_{c}"] = nums.safe_mean(d[c] for d in media)
         media = [D]
 
     else:
         # NOTE: when changing/moving this code be sure to preserve the behavior that -pa does not run the code
         if getattr(args, "delete_files", False):
             marked = post_actions.delete_media(args, [d["path"] for d in media])
             log.warning(f"Deleted {marked} files")
@@ -256,18 +256,18 @@
                 + (
                     f" (limited by --limit {args.limit})"
                     if args.limit and int(args.limit) <= len(media) and len(tbl) <= int(args.limit)
                     else ""
                 ),
             )
 
-        if duration > 0:
-            duration = printing.human_duration(duration)
+        if total_duration > 0:
+            total_duration = printing.human_duration(total_duration)
             if "a" not in print_args:
-                print("Total duration:", duration)
+                print("Total duration:", total_duration)
 
 
 def printer(args, query, bindings, units=None) -> None:
     media = list(args.db.query(query, bindings))
     try:
         media_printer(args, media, units=units)
     except FileNotFoundError:
```

### Comparing `xklb-2.8.7/xklb/readme.py` & `xklb-2.8.9/xklb/readme.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/usage.py` & `xklb-2.8.9/xklb/usage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1690,15 +1690,15 @@
         library links-update links.db
 """
 
 extract_text = r"""library extract-text PATH ... [--skip-links]
 
     Sorting suggestions
 
-        lb extract-text --skip-links --local-file (cb -t text/html | psub) | lb cs --groups | jq -r '.[] | .grouped_paths | "\n" + join("\n")'
+        lb extract-text --skip-links --local-html (cb -t text/html | psub) | lb cs --groups | jq -r '.[] | .grouped_paths | "\n" + join("\n")'
 """
 
 site_add = """library site-add DATABASE PATH ... [--auto-pager] [--poke] [--local-html] [--file FILE]
 
     Extract data from website requests to a database
 
         library siteadd jobs.st.db --poke https://hk.jobsdb.com/hk/search-jobs/python/
```

### Comparing `xklb-2.8.7/xklb/createdb/av.py` & `xklb-2.8.9/xklb/createdb/av.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/createdb/fs_add.py` & `xklb-2.8.9/xklb/createdb/fs_add.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/createdb/gallery_add.py` & `xklb-2.8.9/xklb/createdb/gallery_add.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/createdb/gallery_backend.py` & `xklb-2.8.9/xklb/createdb/gallery_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/createdb/hn_add.py` & `xklb-2.8.9/xklb/createdb/hn_add.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/createdb/links_add.py` & `xklb-2.8.9/xklb/createdb/links_add.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,14 @@
     parser.add_argument("--stop-link")
 
     parser.add_argument("--page-replace")
     parser.add_argument("--page-key", default="page")
     parser.add_argument("--page-step", "--step", type=int, default=1)
     parser.add_argument("--page-start", "--start-page", "--start", type=int)
 
-    parser.add_argument("--local-file", "--local-html", action="store_true", help="Treat paths as Local HTML files")
-
     arggroups.filter_links(parser)
 
     arggroups.requests(parser)
     arggroups.selenium(parser)
     arggroups.extractor(parser)
 
     parser.add_argument("--force", action="store_true")
@@ -57,24 +55,26 @@
 
 def add_playlist(args, path):
     info = {
         "hostname": urlparse(path).hostname,
         "category": getattr(args, "category", None) or "Uncategorized",
         "time_created": consts.APPLICATION_START,
         "extractor_config": args.extractor_config,
+        "time_modified": 0,
         "time_deleted": 0,
     }
     return db_playlists.add(args, str(path), info)
 
 
 def consolidate_media(args, path: str) -> dict:
     return {
         "path": path,
         "category": getattr(args, "category", None) or "Uncategorized",
         "time_created": consts.APPLICATION_START,
+        "time_modified": 0,
         "time_deleted": 0,
     }
 
 
 def add_media(args, variadic):
     for path_or_dict in variadic:
         if isinstance(path_or_dict, str):
```

### Comparing `xklb-2.8.7/xklb/createdb/places_import.py` & `xklb-2.8.9/xklb/createdb/places_import.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/createdb/reddit_add.py` & `xklb-2.8.9/xklb/createdb/reddit_add.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/createdb/row_add.py` & `xklb-2.8.9/xklb/createdb/row_add.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/createdb/site_add.py` & `xklb-2.8.9/xklb/createdb/site_add.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/createdb/substack.py` & `xklb-2.8.9/xklb/createdb/substack.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/createdb/subtitle.py` & `xklb-2.8.9/xklb/createdb/subtitle.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/createdb/tabs_add.py` & `xklb-2.8.9/xklb/createdb/tabs_add.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/createdb/tildes.py` & `xklb-2.8.9/xklb/createdb/tildes.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/createdb/tube_add.py` & `xklb-2.8.9/xklb/createdb/tube_add.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/createdb/tube_backend.py` & `xklb-2.8.9/xklb/createdb/tube_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -365,15 +365,14 @@
 
     func_opts = {
         "ignoreerrors": ignoreerrors,
         "extractor_args": {"youtube": {"skip": ["authcheck"]}},
         "logger": DictLogger(),
         "skip_download": False,
         "postprocessors": [{"key": "FFmpegMetadata"}],
-        "restrictfilenames": True,
         "extract_flat": False,
         "lazy_playlist": True,
         "noplaylist": True,
         "playlist_items": "1",
         "playlist_end": None,
         "extractor_retries": 3,
         "retries": 12,
```

### Comparing `xklb-2.8.7/xklb/createdb/web_add.py` & `xklb-2.8.9/xklb/createdb/web_add.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,14 @@
     arggroups.db_profiles(parser)
     arggroups.requests(parser)
     arggroups.selenium(parser)
     arggroups.filter_links(parser)
     arggroups.extractor(parser)
 
     parser.add_argument("--hash", action="store_true")
-    parser.add_argument("--local-html", "--local-file", action="store_true", help="Treat paths as Local HTML files")
     parser.add_argument(
         "--sizes",
         action="append",
         help="Only grab extended metadata for files of specific sizes (uses the same syntax as fd-find)",
     )
 
     arggroups.debug(parser)
```

### Comparing `xklb-2.8.7/xklb/data/imagemagick_errors.py` & `xklb-2.8.9/xklb/data/imagemagick_errors.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/data/wordbank.py` & `xklb-2.8.9/xklb/data/wordbank.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/data/yt_dlp_errors.py` & `xklb-2.8.9/xklb/data/yt_dlp_errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 .*Did not get any data blocks
 .*Too Many Requests
 .*Postprocessing
 .*Premieres in
 .*user.*not allowed
 .*Private subreddit
 .*Upgrade now
-.*read operation timed out
+.*timed out
 .*Could not connect
 .*restricted
 .*Media check failed
 .*Internal Server Error
 .*Internal error encountered
 .*not currently available
 .*currently unavailable
@@ -170,15 +170,14 @@
 .*Video has been flagged for verification
 .*This video has been disabled
 .*The uploader has not made this video available.
 .*channel/playlist does not exist
 .*This video is DRM protected
 .*This video is protected by a password
 .*This video requires payment to watch.
-.*Unable to download webpage
 .*dashboard-only post
 .*The policy key provided does not permit this account or video
 .*live stream recording
 .*The channel is not currently live
 .*This live event will begin in a few moments
 .*nudity or sexual content
 .*policy on harassment and bullying
```

### Comparing `xklb-2.8.7/xklb/editdb/dedupe_db.py` & `xklb-2.8.9/xklb/editdb/dedupe_db.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/editdb/dedupe_media.py` & `xklb-2.8.9/xklb/editdb/dedupe_media.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/editdb/merge_online_local.py` & `xklb-2.8.9/xklb/editdb/merge_online_local.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/editdb/mpv_watchlater.py` & `xklb-2.8.9/xklb/editdb/mpv_watchlater.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/editdb/pushshift.py` & `xklb-2.8.9/xklb/editdb/pushshift.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/editdb/reddit_selftext.py` & `xklb-2.8.9/xklb/editdb/reddit_selftext.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/files/christen.py` & `xklb-2.8.9/xklb/files/christen.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/files/sample_compare.py` & `xklb-2.8.9/xklb/files/sample_compare.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/files/sample_hash.py` & `xklb-2.8.9/xklb/files/sample_hash.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/files/similar_files.py` & `xklb-2.8.9/xklb/files/similar_files.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/folders/big_dirs.py` & `xklb-2.8.9/xklb/folders/big_dirs.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/folders/merge_folders.py` & `xklb-2.8.9/xklb/folders/merge_folders.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/folders/mount_stats.py` & `xklb-2.8.9/xklb/folders/mount_stats.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/folders/move_list.py` & `xklb-2.8.9/xklb/folders/move_list.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/folders/rel_mv.py` & `xklb-2.8.9/xklb/folders/rel_mv.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/folders/scatter.py` & `xklb-2.8.9/xklb/folders/scatter.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/folders/similar_folders.py` & `xklb-2.8.9/xklb/folders/similar_folders.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/fsdb/disk_usage.py` & `xklb-2.8.9/xklb/fsdb/disk_usage.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/fsdb/search_db.py` & `xklb-2.8.9/xklb/fsdb/search_db.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/mediadb/block.py` & `xklb-2.8.9/xklb/mediadb/block.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/mediadb/db_history.py` & `xklb-2.8.9/xklb/mediadb/db_history.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/mediadb/db_media.py` & `xklb-2.8.9/xklb/mediadb/db_media.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/mediadb/db_playlists.py` & `xklb-2.8.9/xklb/mediadb/db_playlists.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/mediadb/download.py` & `xklb-2.8.9/xklb/mediadb/download.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/mediadb/download_status.py` & `xklb-2.8.9/xklb/mediadb/download_status.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/mediadb/history.py` & `xklb-2.8.9/xklb/mediadb/history.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/mediadb/history_add.py` & `xklb-2.8.9/xklb/mediadb/history_add.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/mediadb/playlists.py` & `xklb-2.8.9/xklb/mediadb/playlists.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/mediadb/redownload.py` & `xklb-2.8.9/xklb/mediadb/redownload.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/mediadb/search.py` & `xklb-2.8.9/xklb/mediadb/search.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/mediadb/stats.py` & `xklb-2.8.9/xklb/mediadb/stats.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/mediafiles/media_check.py` & `xklb-2.8.9/xklb/mediafiles/media_check.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/mediafiles/process_ffmpeg.py` & `xklb-2.8.9/xklb/mediafiles/process_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/mediafiles/process_image.py` & `xklb-2.8.9/xklb/mediafiles/process_image.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/misc/dedupe_czkawka.py` & `xklb-2.8.9/xklb/misc/dedupe_czkawka.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/misc/export_text.py` & `xklb-2.8.9/xklb/misc/export_text.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/multidb/copy_play_counts.py` & `xklb-2.8.9/xklb/multidb/copy_play_counts.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/multidb/merge_dbs.py` & `xklb-2.8.9/xklb/multidb/merge_dbs.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/playback/links_open.py` & `xklb-2.8.9/xklb/playback/links_open.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/playback/media_player.py` & `xklb-2.8.9/xklb/playback/media_player.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/playback/play_actions.py` & `xklb-2.8.9/xklb/playback/play_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/playback/playback_control.py` & `xklb-2.8.9/xklb/playback/playback_control.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/playback/post_actions.py` & `xklb-2.8.9/xklb/playback/post_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/playback/surf.py` & `xklb-2.8.9/xklb/playback/surf.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/playback/tabs_open.py` & `xklb-2.8.9/xklb/playback/tabs_open.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/scratch/javguru.py` & `xklb-2.8.9/xklb/scratch/javguru.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/scratch/javtiful.py` & `xklb-2.8.9/xklb/scratch/javtiful.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/scratch/mam_search.py` & `xklb-2.8.9/xklb/scratch/mam_search.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/scratch/mam_slots.py` & `xklb-2.8.9/xklb/scratch/mam_slots.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/tablefiles/eda.py` & `xklb-2.8.9/xklb/tablefiles/eda.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/tablefiles/incremental_diff.py` & `xklb-2.8.9/xklb/tablefiles/incremental_diff.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/tablefiles/mcda.py` & `xklb-2.8.9/xklb/tablefiles/mcda.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/text/cluster_sort.py` & `xklb-2.8.9/xklb/text/cluster_sort.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/text/extract_links.py` & `xklb-2.8.9/xklb/text/extract_links.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,14 @@
     arggroups.extractor(parser)
     arggroups.requests(parser)
     arggroups.selenium(parser)
     arggroups.filter_links(parser)
 
     parser.add_argument("--print-link-text", "--print-title", action="store_true")
     parser.add_argument("--download", action="store_true", help="Download filtered links")
-    parser.add_argument("--local-file", "--local-html", action="store_true", help="Treat paths as Local HTML files")
 
     arggroups.debug(parser)
     arggroups.paths_or_stdin(parser)
     args = parser.parse_args()
     arggroups.args_post(args, parser)
 
     arggroups.extractor_post(args)
```

### Comparing `xklb-2.8.7/xklb/text/extract_text.py` & `xklb-2.8.9/xklb/text/extract_text.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 
 def parse_args():
     parser = argparse_utils.ArgumentParser(prog="library extract-text", usage=usage.extract_text)
     arggroups.requests(parser)
     arggroups.selenium(parser)
 
+    parser.add_argument("--local-html", action="store_true", help="Treat paths as Local HTML files")
     parser.add_argument("--skip-links", action="store_true")
     parser.add_argument("--download", "--save", "--write", action="store_true")
-    parser.add_argument("--local-file", "--local-html", action="store_true", help="Treat paths as Local HTML files")
 
     arggroups.debug(parser)
     arggroups.paths_or_stdin(parser)
     args = parser.parse_args()
     arggroups.args_post(args, parser)
 
     arggroups.selenium_post(args)
```

### Comparing `xklb-2.8.7/xklb/text/markdown_links.py` & `xklb-2.8.9/xklb/text/markdown_links.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/text/nouns.py` & `xklb-2.8.9/xklb/text/nouns.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/utils/arg_utils.py` & `xklb-2.8.9/xklb/utils/arg_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/utils/arggroups.py` & `xklb-2.8.9/xklb/utils/arggroups.py`

 * *Files 0% similar despite different names*

```diff
@@ -625,14 +625,15 @@
     parser.add_argument("--case-sensitive", action="store_true", help="Filter with case sensitivity")
     parser.add_argument(
         "--no-url-decode",
         "--skip-url-decode",
         action="store_true",
         help="Skip URL-decode for --path-include/--path-exclude",
     )
+    parser.add_argument("--local-html", action="store_true", help="Treat paths as Local HTML files")
 
 
 def filter_links_post(args):
     if not args.case_sensitive:
         args.before_include = [s.lower() for s in args.before_include]
         args.path_include = [s.lower() for s in args.path_include]
         args.text_include = [s.lower() for s in args.text_include]
```

### Comparing `xklb-2.8.7/xklb/utils/argparse_utils.py` & `xklb-2.8.9/xklb/utils/argparse_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/utils/consts.py` & `xklb-2.8.9/xklb/utils/consts.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/utils/db_utils.py` & `xklb-2.8.9/xklb/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/utils/devices.py` & `xklb-2.8.9/xklb/utils/devices.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/utils/file_utils.py` & `xklb-2.8.9/xklb/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/utils/gui.py` & `xklb-2.8.9/xklb/utils/gui.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/utils/iterables.py` & `xklb-2.8.9/xklb/utils/iterables.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/utils/log_utils.py` & `xklb-2.8.9/xklb/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/utils/mpv_utils.py` & `xklb-2.8.9/xklb/utils/mpv_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/utils/nums.py` & `xklb-2.8.9/xklb/utils/nums.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,24 +51,24 @@
         return s
 
 
 def safe_median(l) -> float | None:
     if not l:
         return None
     try:
-        return statistics.median(v for v in l if v is not None)
+        return statistics.median(v for v in l if v is not None and v > 0)
     except statistics.StatisticsError:
         return None
 
 
 def safe_mean(l) -> float | None:
     if not l:
         return None
     try:
-        return statistics.mean(v for v in l if v is not None)
+        return statistics.mean(v for v in l if v is not None and v > 0)
     except statistics.StatisticsError:
         return None
 
 
 def human_to_bytes(input_str) -> int:
     byte_map = {"b": 1, "kb": 1024, "mb": 1024**2, "gb": 1024**3, "tb": 1024**4, "pb": 1024**5}
```

### Comparing `xklb-2.8.7/xklb/utils/objects.py` & `xklb-2.8.9/xklb/utils/objects.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/utils/path_utils.py` & `xklb-2.8.9/xklb/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/utils/pd_utils.py` & `xklb-2.8.9/xklb/utils/pd_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/utils/printing.py` & `xklb-2.8.9/xklb/utils/printing.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/utils/processes.py` & `xklb-2.8.9/xklb/utils/processes.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/utils/sql_utils.py` & `xklb-2.8.9/xklb/utils/sql_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/utils/sqlgroups.py` & `xklb-2.8.9/xklb/utils/sqlgroups.py`

 * *Files 1% similar despite different names*

```diff
@@ -360,15 +360,15 @@
                 {'and COALESCE(p.time_deleted, 0) = 0' if 'time_deleted' in pl_columns else ''}
                 and m.path like "http%"
                 {same_subdomain if getattr(args, 'same_domain', False) else ''}
                 {'AND (score IS NULL OR score > 7)' if 'score' in m_columns else ''}
                 {'AND (upvote_ratio IS NULL OR upvote_ratio > 0.73)' if 'upvote_ratio' in m_columns else ''}
                 {" ".join(args.filter_sql)}
             ORDER BY 1=1
-                , COALESCE(m.time_modified, 0) = 0 DESC
+                {', COALESCE(m.time_modified, 0) = 0 DESC' if 'time_modified' in m_columns else ''}
                 {', p.extractor_key IS NOT NULL DESC' if 'sort' in args.defaults else ''}
                 {', m.error IS NULL DESC' if 'error' in m_columns else ''}
                 {', random()' if 'sort' in args.defaults else ', ' + args.sort}
             {sql_utils.limit_sql(args.limit, args.offset)}
         """
     else:
         query = f"""select
@@ -388,14 +388,14 @@
                 {'and COALESCE(m.time_deleted,0) = 0' if 'time_deleted' in m_columns else ''}
                 and m.path like "http%"
                 {same_subdomain if getattr(args, 'same_domain', '') else ''}
                 {'AND (score IS NULL OR score > 7)' if 'score' in m_columns else ''}
                 {'AND (upvote_ratio IS NULL OR upvote_ratio > 0.73)' if 'upvote_ratio' in m_columns else ''}
                 {" ".join(args.filter_sql)}
             ORDER BY 1=1
-                , COALESCE(m.time_modified, 0) = 0 DESC
+                {', COALESCE(m.time_modified, 0) = 0 DESC' if 'time_modified' in m_columns else ''}
                 {', m.error IS NULL DESC' if 'error' in m_columns else ''}
                 {', random()' if 'sort' in args.defaults else ', ' + args.sort}
         {sql_utils.limit_sql(args.limit, args.offset)}
         """
 
     return query, args.filter_bindings
```

### Comparing `xklb-2.8.7/xklb/utils/strings.py` & `xklb-2.8.9/xklb/utils/strings.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/utils/web.py` & `xklb-2.8.9/xklb/utils/web.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/xklb/assets/kotobago.png` & `xklb-2.8.9/xklb/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/.gitignore` & `xklb-2.8.9/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/pyproject.toml` & `xklb-2.8.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xklb-2.8.7/.github/README.md` & `xklb-2.8.9/.github/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 To stop playing press Ctrl+C in either the terminal or mpv
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    library (v2.8.007; 72 subcommands)
+    library (v2.8.009; 72 subcommands)
 
     Create database subcommands:
     ╭───────────────┬──────────────────────────────────────────╮
     │ fs-add        │ Add local media                          │
     ├───────────────┼──────────────────────────────────────────┤
     │ tube-add      │ Add online video media (yt-dlp)          │
     ├───────────────┼──────────────────────────────────────────┤
@@ -1042,15 +1042,15 @@
 <details><summary>Extract human text from lists of web links</summary>
 
     $ library extract-text -h
     usage: library extract-text PATH ... [--skip-links]
 
     Sorting suggestions
 
-        lb extract-text --skip-links --local-file (cb -t text/html | psub) | lb cs --groups | jq -r '.[] | .grouped_paths | "\n" + join("\n")'
+        lb extract-text --skip-links --local-html (cb -t text/html | psub) | lb cs --groups | jq -r '.[] | .grouped_paths | "\n" + join("\n")'
 
 
 </details>
 
 ###### markdown-links
 
 <details><summary>Extract titles from lists of web links</summary>
```

### Comparing `xklb-2.8.7/PKG-INFO` & `xklb-2.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: xklb
-Version: 2.8.7
+Version: 2.8.9
 Summary: xk library
 Project-URL: documentation, https://github.com/chapmanjacobd/library#usage
 Project-URL: homepage, https://github.com/chapmanjacobd/library#readme
 Project-URL: repository, https://github.com/chapmanjacobd/library/
 Author-email: Jacob Chapman <7908073+chapmanjacobd@users.noreply.github.com>
 License: BSD 3-Clause No Nuclear License
         
@@ -182,15 +182,15 @@
 To stop playing press Ctrl+C in either the terminal or mpv
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    library (v2.8.007; 72 subcommands)
+    library (v2.8.009; 72 subcommands)
 
     Create database subcommands:
     ╭───────────────┬──────────────────────────────────────────╮
     │ fs-add        │ Add local media                          │
     ├───────────────┼──────────────────────────────────────────┤
     │ tube-add      │ Add online video media (yt-dlp)          │
     ├───────────────┼──────────────────────────────────────────┤
@@ -1131,15 +1131,15 @@
 <details><summary>Extract human text from lists of web links</summary>
 
     $ library extract-text -h
     usage: library extract-text PATH ... [--skip-links]
 
     Sorting suggestions
 
-        lb extract-text --skip-links --local-file (cb -t text/html | psub) | lb cs --groups | jq -r '.[] | .grouped_paths | "\n" + join("\n")'
+        lb extract-text --skip-links --local-html (cb -t text/html | psub) | lb cs --groups | jq -r '.[] | .grouped_paths | "\n" + join("\n")'
 
 
 </details>
 
 ###### markdown-links
 
 <details><summary>Extract titles from lists of web links</summary>
```

