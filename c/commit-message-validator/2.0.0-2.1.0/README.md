# Comparing `tmp/commit_message_validator-2.0.0.tar.gz` & `tmp/commit_message_validator-2.1.0.tar.gz`

## Comparing `commit_message_validator-2.0.0.tar` & `commit_message_validator-2.1.0.tar`

### file list

```diff
@@ -1,79 +1,85 @@
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/CONTRIBUTING.rst
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tox.ini
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/src/commit_message_validator/__init__.py
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/src/commit_message_validator/__main__.py
--rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/src/commit_message_validator/cli.py
--rw-r--r--   0        0        0     7486 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/src/commit_message_validator/lint.py
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/src/commit_message_validator/utils.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/src/commit_message_validator/version.py
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/src/commit_message_validator/validators/__init__.py
--rw-r--r--   0        0        0     3765 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/src/commit_message_validator/validators/core.py
--rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/src/commit_message_validator/validators/github.py
--rw-r--r--   0        0        0    14950 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/src/commit_message_validator/validators/rules.py
--rw-r--r--   0        0        0     3876 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/src/commit_message_validator/validators/wikimedia.py
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/test_RulesMessageValidator.py
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/test_lint.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GerritMessageValidator/before_change_id.msg
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GerritMessageValidator/before_change_id.out
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GerritMessageValidator/bug_in_header.msg
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GerritMessageValidator/bug_in_header.out
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GerritMessageValidator/change_private_ok.msg
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GerritMessageValidator/change_private_ok.out
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GerritMessageValidator/check_message_errors.msg
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GerritMessageValidator/check_message_errors.out
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GerritMessageValidator/check_message_ok.msg
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GerritMessageValidator/cherry_pick_not_on_the_last_line.msg
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GerritMessageValidator/cherry_pick_not_on_the_last_line.out
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GerritMessageValidator/co-authored-by_ok.msg
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GerritMessageValidator/hosts_ok.msg
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GerritMessageValidator/invalid_change_id.msg
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GerritMessageValidator/invalid_change_id.out
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GerritMessageValidator/invalid_depends_on.msg
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GerritMessageValidator/invalid_depends_on.out
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GerritMessageValidator/invalid_needed_by.msg
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GerritMessageValidator/invalid_needed_by.out
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GerritMessageValidator/multiple_change_id.msg
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GerritMessageValidator/multiple_change_id.out
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GerritMessageValidator/needed-by_ok.msg
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GerritMessageValidator/note-in-message_ok.msg
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GerritMessageValidator/ok.out
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GerritMessageValidator/really_long_url_ok.msg
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GerritMessageValidator/revert_long_subject_ok.msg
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GerritMessageValidator/short_one_line.msg
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GerritMessageValidator/short_one_line.out
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GerritMessageValidator/short_two_lines.msg
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GerritMessageValidator/short_two_lines.out
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GerritMessageValidator/signed-off-by_ok.msg
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GerritMessageValidator/tag-like-in-message_ok.msg
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GerritMessageValidator/unexpected_line_in_footers.msg
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GerritMessageValidator/unexpected_line_in_footers.out
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GitHubMessageValidator/check_bug_in_header.msg
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GitHubMessageValidator/check_bug_in_header.out
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GitHubMessageValidator/check_github_close_keyword_another_repository.msg
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GitHubMessageValidator/check_github_close_keyword_another_repository.out -> github_close_keyword_error.out
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GitHubMessageValidator/check_github_closed_keyword_another_repository.msg
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GitHubMessageValidator/check_github_closed_keyword_another_repository.out -> github_close_keyword_error.out
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GitHubMessageValidator/check_github_closes_keyword_another_repository.msg
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GitHubMessageValidator/check_github_closes_keyword_another_repository.out -> github_close_keyword_error.out
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GitHubMessageValidator/check_github_fix_keyword_another_repository.msg
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GitHubMessageValidator/check_github_fix_keyword_another_repository.out -> github_close_keyword_error.out
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GitHubMessageValidator/check_github_fixed_keyword_another_repository.msg
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GitHubMessageValidator/check_github_fixed_keyword_another_repository.out -> github_close_keyword_error.out
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GitHubMessageValidator/check_github_fixes_keyword_another_repository.msg
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GitHubMessageValidator/check_github_fixes_keyword_another_repository.out -> github_close_keyword_error.out
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GitHubMessageValidator/check_github_resolve_keyword_another_repository.msg
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GitHubMessageValidator/check_github_resolve_keyword_another_repository.out -> github_close_keyword_error.out
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GitHubMessageValidator/check_github_resolved_keyword_another_repository.msg
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GitHubMessageValidator/check_github_resolved_keyword_another_repository.out -> github_close_keyword_error.out
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GitHubMessageValidator/check_github_resolves_keyword_another_repository.msg
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GitHubMessageValidator/check_github_resolves_keyword_another_repository.out -> github_close_keyword_error.out
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GitHubMessageValidator/github_close_keyword_error.out
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GitHubMessageValidator/good_commit_ok.msg
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GitHubMessageValidator/ok.out
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GitLabMessageValidator/ok.msg
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/tests/data/GitLabMessageValidator/ok.out
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/.gitignore
--rw-r--r--   0        0        0    18092 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/COPYING
--rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/README.rst
--rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     3854 2020-02-02 00:00:00.000000 commit_message_validator-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tox.ini
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/src/commit_message_validator/__init__.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/src/commit_message_validator/__main__.py
+-rw-r--r--   0        0        0     4144 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/src/commit_message_validator/cli.py
+-rw-r--r--   0        0        0     7520 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/src/commit_message_validator/lint.py
+-rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/src/commit_message_validator/utils.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/src/commit_message_validator/version.py
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/src/commit_message_validator/validators/__init__.py
+-rw-r--r--   0        0        0     3765 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/src/commit_message_validator/validators/core.py
+-rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/src/commit_message_validator/validators/github.py
+-rw-r--r--   0        0        0    15020 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/src/commit_message_validator/validators/rules.py
+-rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/src/commit_message_validator/validators/wikimedia.py
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/test_RulesMessageValidator.py
+-rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/test_lint.py
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/test_utils.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/T357188
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GerritMessageValidator/before_change_id.msg
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GerritMessageValidator/before_change_id.out
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GerritMessageValidator/bug_in_header.msg
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GerritMessageValidator/bug_in_header.out
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GerritMessageValidator/change_private_ok.msg
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GerritMessageValidator/change_private_ok.out
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GerritMessageValidator/check_message_errors.msg
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GerritMessageValidator/check_message_errors.out
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GerritMessageValidator/check_message_ok.msg
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GerritMessageValidator/cherry_pick_not_on_the_last_line.msg
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GerritMessageValidator/cherry_pick_not_on_the_last_line.out
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GerritMessageValidator/co-authored-by_ok.msg
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GerritMessageValidator/hosts_ok.msg
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GerritMessageValidator/invalid_change_id.msg
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GerritMessageValidator/invalid_change_id.out
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GerritMessageValidator/invalid_depends_on.msg
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GerritMessageValidator/invalid_depends_on.out
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GerritMessageValidator/invalid_needed_by.msg
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GerritMessageValidator/invalid_needed_by.out
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GerritMessageValidator/multiple_change_id.msg
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GerritMessageValidator/multiple_change_id.out
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GerritMessageValidator/needed-by_ok.msg
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GerritMessageValidator/note-in-message_ok.msg
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GerritMessageValidator/ok.out
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GerritMessageValidator/really_long_url_ok.msg
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GerritMessageValidator/revert_long_subject_ok.msg
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GerritMessageValidator/short_one_line.msg
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GerritMessageValidator/short_one_line.out
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GerritMessageValidator/short_two_lines.msg
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GerritMessageValidator/short_two_lines.out
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GerritMessageValidator/signed-off-by_ok.msg
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GerritMessageValidator/tag-like-in-message_ok.msg
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GerritMessageValidator/unexpected_line_in_footers.msg
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GerritMessageValidator/unexpected_line_in_footers.out
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GitHubMessageValidator/check_bug_in_header.msg
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GitHubMessageValidator/check_bug_in_header.out
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GitHubMessageValidator/check_github_close_keyword_another_repository.msg
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GitHubMessageValidator/check_github_close_keyword_another_repository.out -> github_close_keyword_error.out
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GitHubMessageValidator/check_github_closed_keyword_another_repository.msg
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GitHubMessageValidator/check_github_closed_keyword_another_repository.out -> github_close_keyword_error.out
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GitHubMessageValidator/check_github_closes_keyword_another_repository.msg
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GitHubMessageValidator/check_github_closes_keyword_another_repository.out -> github_close_keyword_error.out
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GitHubMessageValidator/check_github_fix_keyword_another_repository.msg
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GitHubMessageValidator/check_github_fix_keyword_another_repository.out -> github_close_keyword_error.out
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GitHubMessageValidator/check_github_fixed_keyword_another_repository.msg
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GitHubMessageValidator/check_github_fixed_keyword_another_repository.out -> github_close_keyword_error.out
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GitHubMessageValidator/check_github_fixes_keyword_another_repository.msg
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GitHubMessageValidator/check_github_fixes_keyword_another_repository.out -> github_close_keyword_error.out
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GitHubMessageValidator/check_github_resolve_keyword_another_repository.msg
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GitHubMessageValidator/check_github_resolve_keyword_another_repository.out -> github_close_keyword_error.out
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GitHubMessageValidator/check_github_resolved_keyword_another_repository.msg
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GitHubMessageValidator/check_github_resolved_keyword_another_repository.out -> github_close_keyword_error.out
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GitHubMessageValidator/check_github_resolves_keyword_another_repository.msg
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GitHubMessageValidator/check_github_resolves_keyword_another_repository.out -> github_close_keyword_error.out
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GitHubMessageValidator/github_close_keyword_error.out
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GitHubMessageValidator/good_commit_ok.msg
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GitHubMessageValidator/ok.out
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GitLabMessageValidator/T351253-slash.msg
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GitLabMessageValidator/T351253-slash.out
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GitLabMessageValidator/T351253-space-ok.msg
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GitLabMessageValidator/T351253-space-ok.out
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GitLabMessageValidator/ok.msg
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/tests/data/GitLabMessageValidator/ok.out
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/.gitignore
+-rw-r--r--   0        0        0    18092 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/COPYING
+-rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/README.rst
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3854 2020-02-02 00:00:00.000000 commit_message_validator-2.1.0/PKG-INFO
```

### Comparing `commit_message_validator-2.0.0/CONTRIBUTING.rst` & `commit_message_validator-2.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `commit_message_validator-2.0.0/tox.ini` & `commit_message_validator-2.1.0/tox.ini`

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,53 @@
 [tox]
-min_version = 4.0
-envlist =
+requires =
+    tox>=4.2
+env_list =
     lint
+    py312
     py311
     py310
     py39
     py38
     py37
     pkg_meta
-isolated_build = true
 skip_missing_interpreters = true
 
 [testenv]
 description = run the tests with pytest under {envname}
 deps =
     pytest
     pytest-cov
 commands =
     pytest
 
 [testenv:lint]
 description = format the code base to adhere to our styles, and complain about what we cannot do automatically
-base_python = py311
+base_python = py312
 deps =
     pre-commit>=3.2
 commands =
     pre-commit run --all-files --show-diff-on-failure {posargs}
     python -c 'print(r"hint: run {envbindir}{/}pre-commit install to add checks as pre-commit hook")'
 
 [testenv:pkg_meta]
 description = check that generated packages are valid
-base_python = py311
+base_python = py312
 skip_install = true
 deps =
     build[virtualenv]>=0.10
     check-wheel-contents>=0.4
     twine>=4.0.2
 commands =
     python3 -m build --outdir {envtmpdir} --sdist --wheel .
     twine check --strict {envtmpdir}{/}*
     check-wheel-contents {envtmpdir}
 
 [testenv:sample]
-base_python = py311
+base_python = py312
 deps =
 commands =
     commit-message-validator sample {posargs}
 
 [flake8]
 exclude = .tox
 max_line_length = 120
@@ -55,14 +56,15 @@
 addopts =
     --doctest-modules
     --verbosity=2
     --cov=commit_message_validator
     --cov-report=term
     --cov-report=html
     --cov-report=xml
+    --junitxml=dist/junit.xml
 
 [coverage:run]
 branch = True
 omit =
     **/__main__.py
 
 [coverage:report]
```

### Comparing `commit_message_validator-2.0.0/src/commit_message_validator/__init__.py` & `commit_message_validator-2.1.0/src/commit_message_validator/__init__.py`

 * *Files identical despite different names*

### Comparing `commit_message_validator-2.0.0/src/commit_message_validator/__main__.py` & `commit_message_validator-2.1.0/src/commit_message_validator/__main__.py`

 * *Files identical despite different names*

### Comparing `commit_message_validator-2.0.0/src/commit_message_validator/cli.py` & `commit_message_validator-2.1.0/src/commit_message_validator/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 )
 @click.version_option(version=__version__)
 @click.pass_context
 def cli(ctx):
     """Validate git commit messages to Wikimedia standards."""
     if ctx.invoked_subcommand is None:
         # Legacy default is to run the validate subcommand
-        ctx.invoke(validate)
+        ctx.exit(ctx.invoke(validate))
 
 
 @cli.command("install")
 @click.pass_context
 def install_hook(ctx):
     """Explain that this sub-command has been removed"""
     click.echo(
```

### Comparing `commit_message_validator-2.0.0/src/commit_message_validator/lint.py` & `commit_message_validator-2.1.0/src/commit_message_validator/lint.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 import io
 import operator
 import os
 import sys
 
 from .utils import ansi_codes
 from .utils import check_output
+from .utils import commit_message_cleanup_strip
 from .validators import GerritMessageValidator
 from .validators import GitHubMessageValidator
 from .validators import GitLabMessageValidator
 
 WIKIMEDIA_GERRIT_HOST = "gerrit.wikimedia.org"
 WIKIMEDIA_GITLAB_HOST = "gitlab.wikimedia.org"
 GERRIT_CHECK_FAIL_MESSAGE_SUGGESTION = (
@@ -161,15 +162,15 @@
     """Validate one or more commit messages.
 
     :param start_ref: Commit to start validation from
     :param end_ref: Commit to end validation before
     :param msg_path: :class:`pathlib.Path` to file with commit-message to validate
     :param validator: Validator to use
     """
-    if validator and type(validator) == str:
+    if validator and type(validator) is str:
         validator = {
             "GerritMessageValidator": GerritMessageValidator,
             "GitHubMessageValidator": GitHubMessageValidator,
             "GitLabMessageValidator": GitLabMessageValidator,
         }.get(validator)
     if validator is None:
         validator = guess_message_validator_class()
@@ -177,17 +178,17 @@
     print("commit-message-validator")
     print(f"Using {validator.__name__} to check the commit message")
 
     exit_status = 0
     if msg_path:
         # Read from file rather than git repo
         with msg_path.open(encoding="utf-8") as f:
-            lines = [line.rstrip() for line in f.readlines()]
-            if lines and not lines[-1]:
-                lines = lines[:-1]
+            lines = commit_message_cleanup_strip(
+                [line.rstrip() for line in f.readlines()],
+            )
             exit_status = check_message(lines, validator)
     else:
         sha1s = check_output(
             "git",
             "log",
             "--format=%H",
             "--no-merges",
```

### Comparing `commit_message_validator-2.0.0/src/commit_message_validator/utils.py` & `commit_message_validator-2.1.0/src/commit_message_validator/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -59,7 +59,36 @@
                 "color.commit_message_validator.error",
                 "red",
             ),
             "\x1b[0m",
         )
     except subprocess.CalledProcessError:  # pragma: no cover
         return "", ""
+
+
+def commit_message_cleanup_strip(lines):
+    """Cleanup input in the style of `git commit --cleanup=strip`.
+
+    - Strip leading and trailing empty lines
+    - Strip commentary
+    - Strip trailing whitespace
+    - Collapse consecutive empty lines
+    """
+
+    def pop_matching(predicate, idx=-1):
+        while predicate(lines[idx]):
+            lines.pop(idx)
+
+    pop_matching(lambda x: x == "", idx=0)  # Discard empty leading lines
+    pop_matching(lambda x: x == "")  # Discard empty trailing lines
+    pop_matching(lambda x: x.startswith("#"))  # Discard commentary
+    pop_matching(lambda x: x == "")  # Discard empty trailing lines
+
+    # Strip trailing whitespace and consolidate consecutive empty lines
+    prior_line = None
+    cleaned = []
+    for line in lines:
+        line = line.rstrip()
+        if line != prior_line or prior_line != "":
+            cleaned.append(line)
+        prior_line = line
+    return cleaned
```

### Comparing `commit_message_validator-2.0.0/src/commit_message_validator/version.py` & `commit_message_validator-2.1.0/src/commit_message_validator/version.py`

 * *Files identical despite different names*

### Comparing `commit_message_validator-2.0.0/src/commit_message_validator/validators/__init__.py` & `commit_message_validator-2.1.0/src/commit_message_validator/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `commit_message_validator-2.0.0/src/commit_message_validator/validators/core.py` & `commit_message_validator-2.1.0/src/commit_message_validator/validators/core.py`

 * *Files identical despite different names*

### Comparing `commit_message_validator-2.0.0/src/commit_message_validator/validators/github.py` & `commit_message_validator-2.1.0/src/commit_message_validator/validators/github.py`

 * *Files identical despite different names*

### Comparing `commit_message_validator-2.0.0/src/commit_message_validator/validators/rules.py` & `commit_message_validator-2.1.0/src/commit_message_validator/validators/rules.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,24 +20,24 @@
 import re
 import typing
 
 from .core import MessageValidator
 from .core import ValidationFailure
 
 RE_CHERRYPICK = re.compile(r"^\(cherry picked from commit [0-9a-fA-F]{40}\)$")
-RE_FOOTER = re.compile(
+RE_TRAILER = re.compile(
     r"^(?P<name>[a-z]\S+):(?P<ws>\s*)(?P<value>.*)$",
     re.IGNORECASE,
 )
 
 
 class MessageContext(Enum):
     SUBJECT = 1
     BODY = 2
-    FOOTER = 3
+    TRAILER = 3
 
 
 @dataclasses.dataclass
 class Rule:
     """A validation rule for a commit message."""
 
     id: typing.ClassVar[str]
@@ -132,110 +132,110 @@
     def validate(self, lineno, line, context):
         if context != self.ctx:
             return
         if not self.RE_URL.match(line):
             yield from super().validate(lineno, line, context)
 
 
-class FooterNoBlankLines(LineRule):
-    """No blank lines allowed between footer lines."""
+class TrailerNoBlankLines(LineRule):
+    """No blank lines allowed between trailer lines."""
 
     id = "F1"
-    name = "footer-no-blanks"
-    ctx = MessageContext.FOOTER
+    name = "trailer-no-blanks"
+    ctx = MessageContext.TRAILER
 
     def validate(self, lineno, line, context):
         if context != self.ctx:
             return
         if not line:
             yield ValidationFailure(self.id, lineno, "Unexpected blank line")
 
 
 @dataclasses.dataclass
-class FooterInBody(LineRule):
+class TrailerInBody(LineRule):
     """No '^Name: value$' lines allowed in body."""
 
     id = "F2"
-    name = "footer-in-body"
+    name = "trailer-in-body"
     ctx = MessageContext.BODY
     expected: typing.Optional[typing.Sequence[str]] = None
 
     def validate(self, lineno, line, context):
         if context != self.ctx:
             return
-        m = RE_FOOTER.match(line)
+        m = RE_TRAILER.match(line)
         if m:
             name = m.group("name")
             normalized = name.lower()
             if self.expected and normalized not in self.expected:
                 return
             yield ValidationFailure(
                 self.id,
                 lineno,
-                f"Expected '{name}:' to be in footer",
+                f"Expected '{name}:' to be in trailer",
             )
 
 
-class FooterLineRule(LineRule):
-    """A validation rule for a commit message footer line."""
+class TrailerLineRule(LineRule):
+    """A validation rule for a commit message trailer line."""
 
     def validate(self, lineno, line, context):
-        m = RE_FOOTER.match(line)
+        m = RE_TRAILER.match(line)
         if not m:
             return
         name = m.group("name")
         normalized_name = name.lower()
         ws = m.group("ws")
         value = m.group("value")
-        yield from self.validate_footer(
+        yield from self.validate_trailer(
             lineno,
             name,
             normalized_name,
             ws,
             value,
             context,
         )
 
 
 @dataclasses.dataclass
-class ExpectedFooters(FooterLineRule):
-    """Ensure that footers have expected names and formatting."""
+class ExpectedTrailers(TrailerLineRule):
+    """Ensure that trailers have expected names and formatting."""
 
     id = "F3"
-    name = "expected-footer-format"
+    name = "expected-trailer-format"
     expected: typing.Sequence[str]
     fixup: typing.Optional[typing.Dict[str, str]] = None
 
-    def validate_footer(
+    def validate_trailer(
         self,
         lineno,
         name,
         normalized_name,
         ws,
         value,  # noqa: U100 Unused argument
         context,
     ):
-        footers = {footer.lower(): footer for footer in self.expected}
+        trailers = {trailer.lower(): trailer for trailer in self.expected}
         if self.fixup and normalized_name in self.fixup:
             # Treat as the correct name for the rest of the checks
             normalized_name = self.fixup[normalized_name]
 
-        if normalized_name not in footers.keys():
-            if context is MessageContext.FOOTER:
-                supported = ", ".join(footers.values())
+        if normalized_name not in trailers.keys():
+            if context is MessageContext.TRAILER:
+                supported = ", ".join(trailers.values())
                 yield ValidationFailure(
                     self.id,
                     lineno,
-                    f"Unexpected footer '{name}'. Supported footers: {supported}",
+                    f"Unexpected trailer '{name}'. Supported trailers: {supported}",
                 )
             else:
-                # Not a expected footer, so skip additional checks
+                # Not a expected trailer, so skip additional checks
                 return
 
-        correct_name = footers.get(normalized_name)
+        correct_name = trailers.get(normalized_name)
         if correct_name and correct_name != name:
             yield ValidationFailure(
                 "F4",
                 lineno,
                 f"Use '{correct_name}:' not '{name}:'",
             )
 
@@ -244,25 +244,25 @@
                 "F5",
                 lineno,
                 f"Expected one space after '{name}:'",
             )
 
 
 @dataclasses.dataclass
-class PhabricatorTaskIdExpected(FooterLineRule):
-    """Footer value must be a Phabricator task ID"""
+class PhabricatorTaskIdExpected(TrailerLineRule):
+    """Trailer value must be a Phabricator task ID"""
 
     id = "F6"
     name = "phabricator-task-id-expected"
     names: typing.Sequence[str]
     fixup: typing.Optional[typing.Dict[str, str]] = None
 
-    RE_BUGID = re.compile("^T[0-9]+$")
+    RE_BUGID = re.compile(r"^T[0-9]+(  )?$")
 
-    def validate_footer(
+    def validate_trailer(
         self,
         lineno,
         name,  # noqa: U100 Unused argument
         normalized_name,
         ws,  # noqa: U100 Unused argument
         value,
         context,  # noqa: U100 Unused argument
@@ -275,25 +275,25 @@
                 self.id,
                 lineno,
                 "Bug: value must be a single phabricator task ID",
             )
 
 
 @dataclasses.dataclass
-class ChangeIdExpected(FooterLineRule):
-    """Footer value must be a Gerrit change id."""
+class ChangeIdExpected(TrailerLineRule):
+    """Trailer value must be a Gerrit change id."""
 
     id = "F7"
     name = "change-id-value-expected"
     names: typing.Sequence[str]
     fixup: typing.Optional[typing.Dict[str, str]] = None
 
-    RE_CHANGEID = re.compile("^I[a-f0-9]{40}$")
+    RE_CHANGEID = re.compile(r"^I[a-f0-9]{40}(  )?$")
 
-    def validate_footer(
+    def validate_trailer(
         self,
         lineno,
         name,
         normalized_name,
         ws,  # noqa: U100 Unused argument
         value,
         context,  # noqa: U100 Unused argument
@@ -305,31 +305,31 @@
             yield ValidationFailure(
                 self.id,
                 lineno,
                 f"{name}: value must be a single Gerrit change id",
             )
 
 
-class UnexpectedFooterLine(LineRule):
-    """Ensure that all footer lines are either 'name: value' or
+class UnexpectedTrailerLine(LineRule):
+    """Ensure that all trailer lines are either 'name: value' or
     a cherry-pick indicator."""
 
     id = "F8"
-    name = "unexpected-footer-line"
+    name = "unexpected-trailer-line"
 
     def validate(self, lineno, line, context):
-        if context is not MessageContext.FOOTER:
+        if context is not MessageContext.TRAILER:
             return
         if not line:
             return
-        if not RE_FOOTER.match(line) and not RE_CHERRYPICK.match(line):
+        if not RE_TRAILER.match(line) and not RE_CHERRYPICK.match(line):
             yield ValidationFailure(
                 self.id,
                 lineno,
-                "Expected footer line to follow format of 'Name: ...'",
+                "Expected trailer line to follow format of 'Name: ...'",
             )
 
 
 @dataclasses.dataclass
 class CommitRule(Rule):
     """A validation rule for an entire commit message."""
 
@@ -390,15 +390,15 @@
     id = "C4"
     name = "change-id-required"
     before: typing.Optional[typing.Sequence[str]] = None
 
     def validate(self, lines):
         changeid = False
         for lineno, line in enumerate(lines):
-            m = RE_FOOTER.match(line)
+            m = RE_TRAILER.match(line)
             if m:
                 normalized = m.group("name").lower()
                 if normalized == "change-id":
                     if not changeid:
                         changeid = lineno + 1
                     else:
                         yield ValidationFailure(
@@ -422,24 +422,24 @@
 class RulesMessageValidator(MessageValidator):
     """Validate commit messages based on configured rules."""
 
     def __init__(
         self,
         line_rules=None,
         commit_rules=None,
-        expected_footers=None,
+        expected_trailers=None,
     ):
         """
         :param line_rules: Collection of :class:`LineRule` objects
         :param commit_rules: Collection of :class:`CommitRule` objects
-        :param expected_footers: Collection of normalized footer names
+        :param expected_trailers: Collection of normalized trailer names
         """
         self._line_rules = line_rules or []
         self._commit_rules = commit_rules or []
-        self._expected_footers = expected_footers or []
+        self._expected_trailers = expected_trailers or []
         self._message_context = None
         super().__init__()
 
     def validate(self, lines):
         self._lines = lines
         yield from super().validate(lines)
 
@@ -459,31 +459,31 @@
         :param lines: commit message lines
         :return: :class:`MessageContext`
         """
         if lineno == 0:
             # First line in the commit message is subject.
             self._message_context = MessageContext.SUBJECT
 
-        elif not self._expected_footers:
+        elif not self._expected_trailers:
             self._message_context = MessageContext.BODY
 
-        elif self._message_context is not MessageContext.FOOTER:
+        elif self._message_context is not MessageContext.TRAILER:
             line = lines[lineno]
-            footer_match = RE_FOOTER.match(line)
+            trailer_match = RE_TRAILER.match(line)
             cherrypick_match = RE_CHERRYPICK.match(line)
 
             if (
                 (
-                    footer_match
-                    and footer_match.group("name").lower() in self._expected_footers
+                    trailer_match
+                    and trailer_match.group("name").lower() in self._expected_trailers
                 )
                 or cherrypick_match
             ) and not lines[lineno - 1]:
-                # If the current line is a footer ("Name: ..." formatted)
+                # If the current line is a trailer ("Name: ..." formatted)
                 # or it's a cherry pick
                 # and the previous line is a blank line.
-                # Mark the current line until the end as FOOTER.
-                self._message_context = MessageContext.FOOTER
+                # Mark the current line until the end as TRAILER.
+                self._message_context = MessageContext.TRAILER
             else:
                 self._message_context = MessageContext.BODY
 
         return self._message_context
```

### Comparing `commit_message_validator-2.0.0/src/commit_message_validator/validators/wikimedia.py` & `commit_message_validator-2.1.0/src/commit_message_validator/validators/wikimedia.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,25 +17,25 @@
 # Commit Message Validator.  If not, see <http://www.gnu.org/licenses/>.
 from .rules import BodyMaxLength
 from .rules import ChangeIdExpected
 from .rules import ChangeIdRequired
 from .rules import CherryPickLast
 from .rules import CommitMinLines
 from .rules import CommitSecondLineEmpty
-from .rules import ExpectedFooters
-from .rules import FooterInBody
-from .rules import FooterNoBlankLines
+from .rules import ExpectedTrailers
 from .rules import PhabricatorTaskIdExpected
 from .rules import RulesMessageValidator
 from .rules import SubjectMaxLength
 from .rules import SubjectNoBugOrTask
-from .rules import UnexpectedFooterLine
+from .rules import TrailerInBody
+from .rules import TrailerNoBlankLines
+from .rules import UnexpectedTrailerLine
 
 # Header-like lines that we are interested in validating
-EXPECTED_FOOTERS = [
+EXPECTED_TRAILERS = [
     "Acked-by",
     "Bug",
     "Cc",
     "Change-Id",
     "Co-Authored-by",
     "Depends-On",
     "Hosts",  # Wikimedia puppet-compiler
@@ -45,25 +45,25 @@
     "Requested-by",
     "Reviewed-by",
     "Signed-off-by",
     "Suggested-by",
     "Tested-by",
     "Thanks",
 ]
-NORMALIZED_EXPECTED_FOOTERS = [name.lower() for name in EXPECTED_FOOTERS]
+NORMALIZED_EXPECTED_TRAILERS = [name.lower() for name in EXPECTED_TRAILERS]
 
 BEFORE_CHANGE_ID = [
     "bug",
     "closes",
     "fixes",
     "task",
 ]
 
-# Invalid footer name to expected name mapping
-BAD_FOOTERS = {
+# Invalid trailer name to expected name mapping
+BAD_TRAILERS = {
     "closes": "bug",
     "fixes": "bug",
     "task": "bug",
 }
 
 
 class GerritMessageValidator(RulesMessageValidator):
@@ -71,49 +71,49 @@
 
     def __init__(self):
         super().__init__(
             line_rules=[
                 SubjectMaxLength(),
                 SubjectNoBugOrTask(),
                 BodyMaxLength(),
-                FooterInBody(
-                    expected=NORMALIZED_EXPECTED_FOOTERS + list(BAD_FOOTERS.keys()),
+                TrailerInBody(
+                    expected=NORMALIZED_EXPECTED_TRAILERS + list(BAD_TRAILERS.keys()),
                 ),
-                FooterNoBlankLines(),
-                ExpectedFooters(EXPECTED_FOOTERS, fixup=BAD_FOOTERS),
-                PhabricatorTaskIdExpected(["bug"], fixup=BAD_FOOTERS),
+                TrailerNoBlankLines(),
+                ExpectedTrailers(EXPECTED_TRAILERS, fixup=BAD_TRAILERS),
+                PhabricatorTaskIdExpected(["bug"], fixup=BAD_TRAILERS),
                 ChangeIdExpected(["depends-on", "needed-by", "change-id"]),
-                UnexpectedFooterLine(),
+                UnexpectedTrailerLine(),
             ],
             commit_rules=[
                 CommitMinLines(),
                 CommitSecondLineEmpty(),
                 CherryPickLast(),
                 ChangeIdRequired(before=BEFORE_CHANGE_ID),
             ],
-            expected_footers=NORMALIZED_EXPECTED_FOOTERS,
+            expected_trailers=NORMALIZED_EXPECTED_TRAILERS,
         )
 
 
 class GitLabMessageValidator(RulesMessageValidator):
     """Validate a GitLab remote repo commit message."""
 
     def __init__(self):
         super().__init__(
             line_rules=[
                 SubjectMaxLength(),
                 SubjectNoBugOrTask(),
                 BodyMaxLength(),
-                FooterInBody(
-                    expected=NORMALIZED_EXPECTED_FOOTERS + list(BAD_FOOTERS.keys()),
+                TrailerInBody(
+                    expected=NORMALIZED_EXPECTED_TRAILERS + list(BAD_TRAILERS.keys()),
                 ),
-                FooterNoBlankLines(),
-                ExpectedFooters(EXPECTED_FOOTERS, fixup=BAD_FOOTERS),
-                PhabricatorTaskIdExpected(["bug"], fixup=BAD_FOOTERS),
-                UnexpectedFooterLine(),
+                TrailerNoBlankLines(),
+                ExpectedTrailers(EXPECTED_TRAILERS, fixup=BAD_TRAILERS),
+                PhabricatorTaskIdExpected(["bug"], fixup=BAD_TRAILERS),
+                UnexpectedTrailerLine(),
             ],
             commit_rules=[
                 CommitSecondLineEmpty(),
                 CherryPickLast(),
             ],
-            expected_footers=NORMALIZED_EXPECTED_FOOTERS,
+            expected_trailers=NORMALIZED_EXPECTED_TRAILERS,
         )
```

### Comparing `commit_message_validator-2.0.0/tests/test_RulesMessageValidator.py` & `commit_message_validator-2.1.0/tests/test_RulesMessageValidator.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,19 +24,19 @@
         "Commit subject",
         "",
         "Commit body message",
         "",
         "Change-Id: I00d0f7c3b294c3ddc656f9a5447df89c63142203",
     ]
 
-    validator = RulesMessageValidator(expected_footers=["change-id"])
+    validator = RulesMessageValidator(expected_trailers=["change-id"])
 
     expected_result = [
         MessageContext.SUBJECT,
         MessageContext.BODY,
         MessageContext.BODY,
         MessageContext.BODY,
-        MessageContext.FOOTER,
+        MessageContext.TRAILER,
     ]
 
     result = [validator.get_context(lineno, lines) for lineno in range(len(lines))]
     assert result == expected_result
```

### Comparing `commit_message_validator-2.0.0/tests/test_lint.py` & `commit_message_validator-2.1.0/tests/test_lint.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,37 +11,52 @@
 # Commit Message Validator is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General
 # Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with
 # Commit Message Validator.  If not, see <http://www.gnu.org/licenses/>.
+import contextlib
 import io
 import os
+import pathlib
 import re
 import sys
 
 import pytest
 
 from commit_message_validator.lint import check_message
+from commit_message_validator.lint import validate
 from commit_message_validator.validators import GerritMessageValidator
 from commit_message_validator.validators import GitHubMessageValidator
 from commit_message_validator.validators import GitLabMessageValidator
-from commit_message_validator.validators.wikimedia import EXPECTED_FOOTERS
+from commit_message_validator.validators.wikimedia import EXPECTED_TRAILERS
 
 MESSAGE_VALIDATOR_MAP = {
     "GerritMessageValidator": GerritMessageValidator,
     "GitHubMessageValidator": GitHubMessageValidator,
     "GitLabMessageValidator": GitLabMessageValidator,
 }
 # Regular expression for matching ANSI escape sequences
 # https://stackoverflow.com/a/14693789/8171
 RE_ESC = re.compile(r"\x1B\[[0-?]*[ -/]*[@-~]")
 
 
+@contextlib.contextmanager
+def capture_stdout():
+    """Context manager for capturing stdout."""
+    saved_stdout = sys.stdout
+    try:
+        out = io.StringIO()
+        sys.stdout = out
+        yield out
+    finally:
+        sys.stdout = saved_stdout
+
+
 def generate_tests():
     """
     Create test class which checks the output for a message.
 
     It searches through `tests/data/` and loads all
     file pairs where there is a `.msg` and `.out` file. If both exist it'll
     create a test for this pair where the `.msg` is the commit message and the
@@ -50,15 +65,15 @@
     Filenames for tests that will pass validation must end with 'ok' and can
     omit an explict '.out' file as 'ok.out' will be assumed.
     """
     base_path = os.path.join(
         os.path.dirname(__file__),
         "data",
     )
-    footers_string = ", ".join(footer for footer in EXPECTED_FOOTERS)
+    trailers_string = ", ".join(trailer for trailer in EXPECTED_TRAILERS)
     for message_validator_name in os.listdir(base_path):
         if message_validator_name not in MESSAGE_VALIDATOR_MAP:
             continue
 
         specific_message_validator_test_path = os.path.join(
             base_path,
             message_validator_name,
@@ -80,18 +95,18 @@
                         else:
                             pytest.fail(
                                 "No .out file found for {}.msg".format(
                                     os.path.relpath(fn, base_path),
                                 ),
                             )
                     with open(out_fn) as out:
-                        # FIXME: footers_string is a gross hack now
+                        # FIXME: trailers_string is a gross hack now
                         out_text = out.read().replace(
-                            "%known_gerrit_footers%",
-                            footers_string,
+                            "%known_gerrit_trailers%",
+                            trailers_string,
                         )
                         yield pytest.param(
                             msg.read(),
                             out_text,
                             exit_code,
                             message_validator_name,
                             id=os.path.relpath(fn, base_path),
@@ -104,21 +119,30 @@
 )
 def test_validator(
     msg,
     expected,
     expected_exit_code,
     message_validator_name,
 ):
-    saved_stdout = sys.stdout
-    try:
-        out = io.StringIO()
-        sys.stdout = out
+    with capture_stdout() as out:
         exit_code = check_message(
             msg.splitlines(),
             MESSAGE_VALIDATOR_MAP[message_validator_name],
         )
         # Ignore ANSI escapes in output
         plain_out = RE_ESC.sub("", out.getvalue())
         assert plain_out == expected
         assert exit_code == expected_exit_code
-    finally:
-        sys.stdout = saved_stdout
+
+
+def test_validate_with_msg_path():
+    msg_path = pathlib.Path(__file__).parent / "data" / "T357188"
+    with capture_stdout() as out:
+        exit_code = validate(msg_path=msg_path, validator=GitLabMessageValidator)
+        # Ignore ANSI escapes in output
+        plain_out = RE_ESC.sub("", out.getvalue())
+        assert (
+            plain_out == "commit-message-validator\n"
+            "Using GitLabMessageValidator to check the commit message\n"
+            "Commit message is formatted properly! Keep up the good work!\n"
+        )
+        assert exit_code == 0
```

### Comparing `commit_message_validator-2.0.0/tests/data/GerritMessageValidator/check_message_errors.msg` & `commit_message_validator-2.1.0/tests/data/GerritMessageValidator/check_message_errors.msg`

 * *Files identical despite different names*

### Comparing `commit_message_validator-2.0.0/tests/data/GerritMessageValidator/check_message_errors.out` & `commit_message_validator-2.1.0/tests/data/GerritMessageValidator/check_message_errors.out`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 The following errors were found:
 - Line 1: Subject must be <=80 characters
 - Line 2: Second line should be empty
 - Line 3: Line exceeds max length (174>100)
-- Line 4: Expected 'Fixes:' to be in footer
+- Line 4: Expected 'Fixes:' to be in trailer
 - Line 4: Use 'Bug:' not 'Fixes:'
 - Line 4: Expected one space after 'Fixes:'
 - Line 4: Bug: value must be a single phabricator task ID
-- Line 5: Expected 'Closes:' to be in footer
+- Line 5: Expected 'Closes:' to be in trailer
 - Line 5: Use 'Bug:' not 'Closes:'
 - Line 5: Expected one space after 'Closes:'
 - Line 5: Bug: value must be a single phabricator task ID
-- Line 6: Expected 'Task:' to be in footer
+- Line 6: Expected 'Task:' to be in trailer
 - Line 6: Use 'Bug:' not 'Task:'
-- Line 7: Expected 'BUG:' to be in footer
+- Line 7: Expected 'BUG:' to be in trailer
 - Line 7: Use 'Bug:' not 'BUG:'
 - Line 7: Expected one space after 'BUG:'
 - Line 7: Bug: value must be a single phabricator task ID
-- Line 8: Expected 'Bug:' to be in footer
+- Line 8: Expected 'Bug:' to be in trailer
 - Line 8: Bug: value must be a single phabricator task ID
 - Line 12: Bug: value must be a single phabricator task ID
 - Line 13: Unexpected blank line
 - Line 15: Unexpected blank line
 - Line 16: Bug: value must be a single phabricator task ID
 - Line 19: Extra Change-Id found, first at 18
 - Line 20: Depends-On: value must be a single Gerrit change id
 - Line 21: Unexpected blank line
-- Line 22: Expected footer line to follow format of 'Name: ...'
+- Line 22: Expected trailer line to follow format of 'Name: ...'
```

### Comparing `commit_message_validator-2.0.0/tests/data/GerritMessageValidator/check_message_ok.msg` & `commit_message_validator-2.1.0/tests/data/GerritMessageValidator/check_message_ok.msg`

 * *Files 11% similar despite different names*

```diff
@@ -2,34 +2,34 @@
 
 The body of the commit message starts after a blank line. It contains just
 about any random text, but each line should not exceed 100 characters. Really
 there is no good reason for any body line to exceed 72 characters (80 column
 display with an 8 character tab leading the line) except in the case of a long
 URL that is embedded in the message.
 
-The commit message ends with a footer section containing one or more lines
+The commit message ends with a trailer section containing one or more lines
 providing parsable meta-data about the commit such as Phabricator tasks that
 it addresses and the unique Gerrit change identifier for the patch. This
-footer must be separated from the message body by a single blank line.
+trailer must be separated from the message body by a single blank line.
 
 Other checks:
 - First line <=80 characters
 - Second line blank
 - No line >100 characters (unless it is only a URL)
-- Footer lines ("Foo: ...") are capitalized and have a space after the ':'
+- Trailer lines ("Foo: ...") are capitalized and have a space after the ':'
 - "Bug: " is followed by one task id ("Tnnnn")
 - "Depends-On:" is followed by one change id ("I...")
 - "Change-Id:" is followed one change id ("I...")
 - No "Task: ", "Fixes: ", "Closes: " lines
 - Message has at least 3 lines (subject, blank, Change-Id)
-- For any footer line, next line is not blank
-- For any footer line, prior line is another footer line or blank
+- For any trailer line, next line is not blank
+- For any trailer line, prior line is another trailer line or blank
 - Exactly one "Change-Id: " line per commit
 - Any "Bug:" and "Depends-On:" lines come before "Change-Id:"
-- "(cherry picked from commit ...)" is last line in footer if present
+- "(cherry picked from commit ...)" is last line in trailer if present
 
 https://www.mediawiki.org/wiki/Gerrit/Commit_message_guidelines
 
 Bug: T109119
 Bug: T142804
 Depends-On: I2deb4cd50d50a87a34b0bf4277ad55f77e75dd0d
 Change-Id: Ifcd397165df1cbf9fa04f2044e1bb33ad7414d8d
```

### Comparing `commit_message_validator-2.0.0/tests/data/GitLabMessageValidator/ok.msg` & `commit_message_validator-2.1.0/tests/data/GitLabMessageValidator/ok.msg`

 * *Files 11% similar despite different names*

```diff
@@ -2,34 +2,34 @@
 
 The body of the commit message starts after a blank line. It contains just
 about any random text, but each line should not exceed 100 characters. Really
 there is no good reason for any body line to exceed 72 characters (80 column
 display with an 8 character tab leading the line) except in the case of a long
 URL that is embedded in the message.
 
-The commit message ends with a footer section containing one or more lines
+The commit message ends with a trailer section containing one or more lines
 providing parsable meta-data about the commit such as Phabricator tasks that
 it addresses and the unique Gerrit change identifier for the patch. This
-footer must be separated from the message body by a single blank line.
+trailer must be separated from the message body by a single blank line.
 
 Other checks:
 - First line <=80 characters
 - Second line blank
 - No line >100 characters (unless it is only a URL)
-- Footer lines ("Foo: ...") are capitalized and have a space after the ':'
+- Trailer lines ("Foo: ...") are capitalized and have a space after the ':'
 - "Bug: " is followed by one task id ("Tnnnn")
 - "Depends-On:" is followed by one change id ("I...")
 - "Change-Id:" is followed one change id ("I...")
 - No "Task: ", "Fixes: ", "Closes: " lines
 - Message has at least 3 lines (subject, blank, Change-Id)
-- For any footer line, next line is not blank
-- For any footer line, prior line is another footer line or blank
+- For any trailer line, next line is not blank
+- For any trailer line, prior line is another trailer line or blank
 - Exactly one "Change-Id: " line per commit
 - Any "Bug:" and "Depends-On:" lines come before "Change-Id:"
-- "(cherry picked from commit ...)" is last line in footer if present
+- "(cherry picked from commit ...)" is last line in trailer if present
 
 https://www.mediawiki.org/wiki/Gerrit/Commit_message_guidelines
 
 Bug: T109119
 Bug: T142804
 Depends-On: I2deb4cd50d50a87a34b0bf4277ad55f77e75dd0d
 Change-Id: Ifcd397165df1cbf9fa04f2044e1bb33ad7414d8d
```

### Comparing `commit_message_validator-2.0.0/COPYING` & `commit_message_validator-2.1.0/COPYING`

 * *Files identical despite different names*

### Comparing `commit_message_validator-2.0.0/README.rst` & `commit_message_validator-2.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `commit_message_validator-2.0.0/pyproject.toml` & `commit_message_validator-2.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -43,16 +43,16 @@
     "Topic :: Software Development :: Testing",
     "Topic :: Software Development :: Version Control :: Git",
 ]
 dynamic = [
     "version",
 ]
 dependencies = [
-    "click==8.1.3",
-    "click-aliases==1.0.1",
+    "click==8.1.7",
+    "click-aliases==1.0.4",
     "click-option-group==0.5.6",
     "importlib-metadata==6.7.0 ; python_version < \"3.8\"",
 ]
 
 [project.urls]
 Documentation = "https://www.mediawiki.org/wiki/commit-message-validator"
 Changelog = "https://gitlab.wikimedia.org/repos/ci-tools/commit-message-validator/-/blob/main/HISTORY.rst"
@@ -74,15 +74,15 @@
 ]
 
 [tool.hatch.version]
 source = "vcs"
 
 [tool.black]
 line_length = 88
-target_version = ["py36", "py37", "py38", "py39", "py310", "py311"]
+target_version = ["py36", "py37", "py38", "py39", "py310", "py311", "py312"]
 
 [tool.isort]
 src_paths = ["src", "tests"]
 line_length = 88
 profile = "black"
 force_single_line = true
 force_sort_within_sections = true
```

### Comparing `commit_message_validator-2.0.0/PKG-INFO` & `commit_message_validator-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: commit-message-validator
-Version: 2.0.0
+Version: 2.1.0
 Summary: Validate the format of a commit message to Wikimedia Gerrit standards
 Project-URL: Documentation, https://www.mediawiki.org/wiki/commit-message-validator
 Project-URL: Changelog, https://gitlab.wikimedia.org/repos/ci-tools/commit-message-validator/-/blob/main/HISTORY.rst
 Project-URL: Bug tracker, https://phabricator.wikimedia.org/tag/commit-message-validator/
 Project-URL: Source code, https://gitlab.wikimedia.org/repos/ci-tools/commit-message-validator
 Author-email: Bryan Davis <bd808@wikimedia.org>, Kunal Mehta <Legoktm@debian.org>
 Maintainer-email: Bryan Davis <bd808@wikimedia.org>, Kunal Mehta <Legoktm@debian.org>
@@ -24,17 +24,17 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Version Control :: Git
 Requires-Python: >=3.6
-Requires-Dist: click-aliases==1.0.1
+Requires-Dist: click-aliases==1.0.4
 Requires-Dist: click-option-group==0.5.6
-Requires-Dist: click==8.1.3
+Requires-Dist: click==8.1.7
 Requires-Dist: importlib-metadata==6.7.0; python_version < '3.8'
 Description-Content-Type: text/x-rst
 
 ########################
 Commit Message Validator
 ########################
```

